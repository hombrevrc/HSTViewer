��ʷ(HST)�ļ���ʽ
http://blog.sina.com.cn/s/blog_dd41b3150101dk2m.html
http://blog.csdn.net/u012285618/article/details/54847146
https://github.com/hamling-ling/FxResearches/tree/master/hstconverter

2013.4.15���£�
���˱��ĵĹؼ�֮�������������ֱ�Ӷ�ȡmt4��hst��ʷ�ļ�����ȡ���ݣ��ͱ����ȸ�����ö������ļ������ݸ�ʽ��
��������Ҫ���漰��C++��PHP����ȡmt4����ʷ�ļ������ԣ�������Binary Viewer�򿪸����͵��ļ�������һЩ������
0-147�ֽڣ�Ϊ�ļ�ͷ��
struct Header
{
00    int           version;               // �汾��
04    char        copyright[64];     // ��Ȩ��Ϣ
68    char        symbol[12];         // ���Ҷ����ƣ���"EURUSD"
80    int           period;                // �������ڣ�15���� M15����
84    int           digits;                 // ���ݸ�ʽ��С����λ��     //����5��������Чֵ��С����5λ��1.
88    time_t     time sign;           // �ļ��Ĵ���ʱ��
...     ...
...     ...
};
��148�ֽڿ�ʼ�����������У�ÿ������Ϊ44�ֽڣ��ṹ����:
��һ������
struct RateInfo
{
148    time_t       ctm;                 // ������㵱ǰʱ��
152    double      open;
160    double      low;
168    double      high;
176    double      close;
184    double      vol;
};
�ڶ������ݣ�
192    time_t       ctm; 
196    double      open;
...       ......
...       ......
ע��mt4�ն˹رպ����mt4�ն��Ѵ򿪵�ͼ����ʷ���ݻᱣ������Ӧ��hst�ļ��С�