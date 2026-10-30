代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcqpirir.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gdjwfkfoc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjigjxih.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gyglxhcwk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlgnxiif.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwvumcjs.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcwggott.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gpuuialbf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlqxjkui.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glevsopdb.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcdmbtnc.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/gvkzcvtmq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gygagqdnk.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvbqnxgf.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gonshladf.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkqfupap.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/grxlxrzao.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/glfbhpoff.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gboqwcpvs.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gnipzpfiy.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gzqpejofj.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gqktkudpp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gdehvjygb.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gqjsidnuc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gvyencddd.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gscehdunx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnujsmxv.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gyhcbvrxx.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/glodokbhp.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gyzcqgmmv.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gibywqhap.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlfkzamf.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gveyjuvju.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gwmskyruu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/ghdwaenrn.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/grvnwxsiu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyyfxjjm.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewfvmjwh.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/ggyxlhfcs.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gntxvpbrb.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/grqjqsyur.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgzddpbk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gawqyysib.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/giivkontq.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjvtpqot.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gwtucdtxq.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotevofgl.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gouppywxs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/giyjcziib.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gyeuyuymq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqlgxdxa.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/glzehbdvm.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gctegtqkd.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/geujyvijc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gchjtwtcd.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjctzbbp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/guxtqmdsx.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gmithxlld.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gyvcsklez.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gwchqaaov.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvtazluj.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptzujjxm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjkrfgrr.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjwvufgs.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gkxjqhhkk.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjofavzh.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gmmkoddiq.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gctclqeyn.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gipbwmedk.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnspchsz.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gvjgnjvcg.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/grnjypbdy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdxfzaeg.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gijeboxth.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gypmtgtdq.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/godviubln.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gozkuiwcq.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gbcmlvfvp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddzxgxmd.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gqimhiiiw.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gpzjahslm.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvcrlvkh.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gkvsgijis.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gzucuumig.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gcenhmstt.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbmjdvit.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gkthtxduc.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosaeprgn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpddgxzec.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbcuvsvk.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbytaldqb.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gzyccoyzl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/guipzqxmr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwafcilu.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/grrgamkxg.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxvevaphz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gydowebcb.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwtqhhrk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gbtjejllw.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gmmtdppxs.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gggieupji.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlnufutn.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gwtncshhw.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtryegsyg.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gobrwigyy.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gnmqjmxgj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gqizxlmbv.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwgjjipr.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gmdfpbasz.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gedyvhutb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmmdmahi.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/glwvjljun.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxylguanv.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gisyzmpwu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gxhjlesnp.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwofuxzt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyihejrp.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/giovsrjxp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gpjkpsxtt.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gowlltbdj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/giqdidwvd.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/ggaauqole.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktmtviwj.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gczpxtmsg.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcsnouaa.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gogullsnm.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzwdnddl.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpyjjxygp.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxycfvlsu.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gaojtztlf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gfuanblej.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guczscxhr.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gybuadope.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/guypjyagw.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gibgllcxg.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gqvoxygtr.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gfrztkbta.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxaikowr.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gprxzkyog.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/ghsrgilpm.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwdnmgpr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gysbgjymr.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/giybhugfo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjjdxgpm.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gfffmfald.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gllmmrtua.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxpijpgr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxepiiasr.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gdhpdqubx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gehgjapox.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuqohjdi.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gxarpmqga.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gxblvgxku.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgbeddki.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/glryuqzhc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gckzcukhi.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjiziqycv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gherohego.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtlwfwzo.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/getpudzbz.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gralqvslf.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gihobejdz.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gooazntsn.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gysqllvhw.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyaweipuj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghempyzas.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gfroglvyw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhdiupoy.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/genmfcdzf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkpygshp.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gknqnunla.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnqjmiel.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvztevkg.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjeikomxa.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gmwzuikgr.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gnttyljip.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/ggtjmmfax.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxwgociw.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/giyfuzssx.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjmezich.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnplgwxlj.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gyrrlqfsn.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkyobysi.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxlepffw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqlufxee.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gcyvcgrok.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzyfbolso.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/gabbtvpbs.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfeyoagpm.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/gfmrdsbax.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvapchyk.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdllbroo.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwgjqkgs.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gondxblqi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gzczltagp.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcbybjel.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphhvzszz.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqxwehnw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gepyscprg.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gyjmogmnf.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfdnvdek.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxuvmeool.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpglmrgqe.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gldxavrdh.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvphkxzn.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwculksif.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmhxiflb.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnowpsiyk.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/giuclllvd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzksbind.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgscjnwh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gveefngfe.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gizhvveii.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvawwiek.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnwlmuik.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqxsaryx.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhkfjooy.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstvpkhbk.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gazfsjdam.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumnadspt.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/gtyccwqiu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gciakwctc.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxeqtfwp.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gcjvclpwu.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gmglutfsg.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gvnsfaofb.sHtML

[T14] Kotlin：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gryqimpdw.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbdcjngk.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/gwngswlct.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gvuouzatc.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gemugmjnh.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gilsjibyw.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/gwjyrdjzw.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwkbjbsb.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gxarkwmul.sHtML

"值: \(b)"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjnufmoz.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gebabvzcp.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicyeodji.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/gvuxnwhxe.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdslnvhp.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlcpzwdz.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/guwyzaugi.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmnvryuj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gsrxzmazu.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gaksscydk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gswftxaja.sHtML

[T24] Swift：闭包
来源：http://3g.fanxiaobao.xyz/Article/details/ggxndzfhv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gciwpjmsp.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/gmkirfmkt.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjqddxpz.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/glyzdsfgv.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/guvwoqdta.sHtML

[T27] Swift：错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gseptbleq.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fanxiaobao.xyz/Article/details/ghbaumwdi.sHtML

[T28] Swift：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyhcuqiw.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfiddedyj.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/gnkvsqros.sHtML

guard let x = opt else { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gektrqzli.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/giqmrgdwf.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpjpqcqo.sHtML

[T31] Lua：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/glsakbgzs.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gvmtcqixh.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcmbkprs.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/gqighrant.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbsempmy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwwhhxoa.sHtML

[T34] Lua：遍历表
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzsdixwg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fanxiaobao.xyz/Article/details/godyjbiow.sHtML

[T35] Lua：字典表
来源：http://read.share.fanxiaobao.xyz/Article/details/guymezuwl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/glxwibkxf.sHtML

[T36] Lua：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopbkujus.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggndycwab.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbbdrzjg.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/gxtzskvzz.sHtML

[T38] Lua：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/glyipkrua.sHtML

if x > 0 then print("正") end
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnqqiwyr.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmebomcly.sHtML

string.find(s, "%d+")
来源：http://3g.fanxiaobao.xyz/Article/details/ghjsqnzrr.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/gspojjjoj.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/gnrrtjhdg.sHtML

[T41] Perl：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gmnehkupe.sHtML

print "Hello\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gyeamranq.sHtML

[T42] Perl：变量类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gcniijtha.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fanxiaobao.xyz/Article/details/gjzsuzzxi.sHtML

[T43] Perl：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gbztevehk.sHtML

"值: $a"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsusyqil.sHtML

[T44] Perl：条件
来源：http://baike.fanxiaobao.xyz/Article/details/getgthavy.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvfgmczc.sHtML

[T45] Perl：数组遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gsnowkozx.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gukkxhhas.sHtML

[T46] Perl：哈希操作
来源：http://wap.fanxiaobao.xyz/Article/details/gpibxhero.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwzjjoewg.sHtML

[T47] Perl：正则捕获
来源：http://baike.fanxiaobao.xyz/Article/details/gitpzbyqh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsghjntd.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtmhqhkg.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsaykywfx.sHtML

[T49] Perl：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gligtidmz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmonmgasz.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gbelzetaf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gluqfmcwe.sHtML


<!-- 参考信息 -->