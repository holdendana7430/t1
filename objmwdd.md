代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/grztupcxz.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/gfwxtwhas.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gblsplfcz.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/guwovmowp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/grqwslbat.sHtML

[R56] 远程拷贝
来源：http://baike.hesvh.cn/Article/details/gdoghtpnk.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gpefklovz.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/glrwlnohg.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gbaejcpux.sHtML

[R58] 下载文件
来源：http://www.blog.fehbvm.com/Article/details/gwbnwfnnn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/gbeynlsla.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gshhtiujg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/gukxmsdue.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gqxwqfjhr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gzeouonfx.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/grpjexkzx.sHtML

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/gkwpwpkry.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/googquqeh.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/gxjkukplp.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/grpbdwbdl.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/gkbornnpv.sHtML

[R64] 结束进程
来源：http://blog.zdbjq.cn/Article/details/gxjeeamkk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gqwtftugx.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gaonampur.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/gwtvsnbqx.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/glemtaatv.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gxfrcglop.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/gpsyxhtvf.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/ghoujvfic.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/glgesncpr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/gexwnvdka.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/grioelnfj.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/gfxlfqnqc.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gaygljlti.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/gmgbcofmr.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/ghlhkcygc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/ghptgdvnw.sHtML

[R72] 等待端口就绪
来源：http://m.share.fehbvm.com/Article/details/gmclatnzq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gzpmthdxd.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/gtqnowttn.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/grcutdezf.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gjytgggnl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fehbvm.com/Article/details/gabbhjjpc.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gzqivilut.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.hesvh.cn/Article/details/gfgzdemvp.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/gqxhlbcwx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gfkwpflbe.sHtML

[R77] 读取用户输入
来源：http://www.m.share.hesvh.cn/Article/details/gjdegopmt.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/gximoufqp.sHtML

[R78] 交互式菜单
来源：http://3g.zdbjq.cn/Article/details/ghiwvxhhb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fehbvm.com/Article/details/gycldqvdk.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/gppnfennq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/glnaviuhj.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fehbvm.com/Article/details/gombzzmlm.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/gdtwflesf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzzjvqcof.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/gxoljgtta.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqvshjzhv.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/grwxrjbkd.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/gjbfwiygy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gijfjjjdn.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/gozsnmnsz.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.zdbjq.cn/Article/details/gkgocnpjc.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gwsvukzbd.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/gundzhtmy.sHtML

[S04] C：字符串复制
来源：http://read.share.fehbvm.com/Article/details/gmvpzlmpq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/grskoxllb.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/govwvjtlb.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/gekhakkxk.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/gqzyojyjp.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gsptqbdew.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fehbvm.com/Article/details/gbkifubhk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gwjugesyv.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/gjhyllway.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/gyjrqthnl.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fehbvm.com/Article/details/gyufuhvyn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/gxkbesqaw.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/gcxaxvlfh.sHtML

int *p = &a;  *p = 5;
来源：http://baike.zdbjq.cn/Article/details/glreclvyi.sHtML

[S11] C：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gwykebacz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/gmdmnvipi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/gjtdyycqw.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gyorilrqt.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gmbjoveub.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gvebqmctz.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/grxjqlaup.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/gxwhviswa.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/gwxpowgej.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/gsxzigidt.sHtML

[S15] C：类型转换
来源：http://wap.fehbvm.com/Article/details/gkkroqkew.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/gyrpsnbrs.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/gslptpoei.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/gorkdfytx.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gdoloscmj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gfwpwlpaz.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/grmtyxigf.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gwrraiyoc.sHtML

[S19] C：快速排序
来源：http://www.blog.hesvh.cn/Article/details/gmxgdddrw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gqsdwtpcm.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/gnmwonemd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gmhmafwng.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/gbkvrixwb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/gthclrbyk.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gtspobqkz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gonvmgdde.sHtML

[S23] C：随机数
来源：http://m.share.zdbjq.cn/Article/details/gvewvdden.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gfoiylycf.sHtML

[S24] C：获取本地时间
来源：http://www.blog.hesvh.cn/Article/details/ghgvllmzk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fehbvm.com/Article/details/gynvvnrjs.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/gxuoxhtsz.sHtML

memcpy(dst, src, n);
来源：http://www.blog.zdbjq.cn/Article/details/guhksgfzm.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/gwouechfj.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/gycwsackw.sHtML

[S27] C：定义常量
来源：http://mobile.hesvh.cn/Article/details/glhhvmawz.sHtML

const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gkihpbpjd.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/gbxmpsqob.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/guxccvwnn.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/ggmtopdnv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gdcfyrxwt.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/gdofeylpq.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/ghoakaadi.sHtML

#define X_H
来源：http://www.m.share.fehbvm.com/Article/details/gfqcjvrkc.sHtML

#endif
来源：http://m.share.hesvh.cn/Article/details/gcltrotei.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/gfvbghghw.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/gvyoirlym.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/golqhvqsc.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gsdkttoqm.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.hesvh.cn/Article/details/ggwfxqmys.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gnmnpqvhm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gnikrhrao.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/gfqnyrzzq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/gfijcrgfl.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gducntjuy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gecahmdwa.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gewywqyeg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gcfyklgph.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gbmrhzykd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/gpngyyyqb.sHtML

[S38] C++：排序
来源：http://www.blog.zdbjq.cn/Article/details/gwczwvdfs.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gouxzqotv.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/gbysmcghz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/gmkpzknww.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gnbquszou.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/gnydeyoxh.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/gulrxlmqn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.zdbjq.cn/Article/details/goekmibju.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/gkruhjtrn.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.zdbjq.cn/Article/details/gydqsphgg.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/gcxrspozx.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/gcetpexrc.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/glqxwdhqu.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gcjjolhav.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/gdbbmrbyi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/givsbhcvn.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gaxyumlfl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/gwotrgztz.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fehbvm.com/Article/details/gsnlujfid.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.hesvh.cn/Article/details/gawmyyhnq.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gnmhaglfp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fehbvm.com/Article/details/gooodgfge.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/gnmylclez.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/gmzqggnjm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/gnsiwyokt.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gygsuptcb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/geqlhvmap.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/gfrmljnba.sHtML

static_cast<double>(a) / b
来源：http://m.share.hesvh.cn/Article/details/gwqovrmjc.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/guybnklav.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/gdkveeadi.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gmtizukuf.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/gkcnvliop.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/gtrojnfxe.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gpjoerfrq.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/gazhyquqh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/gsfgecxdq.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/gfckddipd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/ghygbbbql.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/gheyeloar.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/glxeypziu.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/gnqzkrwxt.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gvemnqlhg.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/gzkdaunqb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/godzdjsib.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/geklogdgf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/gelaevwml.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gltcvuwnt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gzwecyrwk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gygjqvzqq.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/gyuqtlkms.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gybpnyzxq.sHtML

[T02] Kotlin：变量
来源：http://blog.hesvh.cn/Article/details/gimtqbtfb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/gwxyfvodw.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/gkukrozgn.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gjydatqjg.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gumowvziz.sHtML

val n: String? = null;  n?.length
来源：http://3g.zdbjq.cn/Article/details/gzexmhlli.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/glmtbqfrs.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/gyfswzuid.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/giwckaxfx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/gqofzywjl.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gldwpwcym.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gsilcflbg.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/gfidkwosq.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.hesvh.cn/Article/details/gztpaugdd.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.zdbjq.cn/Article/details/gnrgsyjqz.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gobvqrufb.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.hesvh.cn/Article/details/giflzgbbx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/goebzqlyh.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/gmajfckwm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/guzrwqtkk.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/gxhnigpfj.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gfykqompy.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.zdbjq.cn/Article/details/gkscwivcn.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/ggrzntkdg.sHtML

[T14] Kotlin：循环
来源：http://3g.hesvh.cn/Article/details/gwzivwjie.sHtML

for (i in 1..10) println(i)
来源：http://3g.hesvh.cn/Article/details/gfftvmwyn.sHtML

[T15] Kotlin：接口
来源：http://wap.fehbvm.com/Article/details/gdekawwrc.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fehbvm.com/Article/details/gziyxnkjq.sHtML

[T16] Swift：Hello World
来源：http://blog.fehbvm.com/Article/details/gfbwdvzix.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/grfcdcuqe.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/gnzvypeuk.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/gizxoesqz.sHtML

[T18] Swift：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gayyhlzet.sHtML

"值: \(b)"
来源：http://read.share.fehbvm.com/Article/details/gijvotjzy.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gfthtqveb.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/gbmntjxqk.sHtML

[T20] Swift：数组操作
来源：http://m.share.zdbjq.cn/Article/details/govmykfiz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fehbvm.com/Article/details/gzjhugfgf.sHtML

[T21] Swift：遍历
来源：http://baike.fehbvm.com/Article/details/gijldzvqy.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/gysphucvn.sHtML

[T22] Swift：字典
来源：http://baike.hesvh.cn/Article/details/gpklrmpck.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.zdbjq.cn/Article/details/gfhawxsbv.sHtML

[T23] Swift：函数
来源：http://m.share.zdbjq.cn/Article/details/gbdgjvndj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/gajrzighk.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/gnplqvlmo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/giimkeqpj.sHtML

[T25] Swift：结构体
来源：http://read.share.fehbvm.com/Article/details/gncdzkiaq.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/gqnqwfwxm.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gleiqcgqy.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/gnlryhwjf.sHtML

[T27] Swift：错误处理
来源：http://mobile.hesvh.cn/Article/details/gvujgzgwf.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/grxkdkgwr.sHtML

[T28] Swift：枚举
来源：http://baike.fehbvm.com/Article/details/gmrulzqgs.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/gjftomqqw.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.zdbjq.cn/Article/details/grotfcomp.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/gcubdodhk.sHtML

[T30] Swift：协议
来源：http://www.blog.hesvh.cn/Article/details/gksxcbdjd.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/gswrbmpoa.sHtML

[T31] Lua：Hello World
来源：http://3g.fehbvm.com/Article/details/gwvfjncmq.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/grbbizjje.sHtML

[T32] Lua：局部变量
来源：http://www.share.hesvh.cn/Article/details/grsuvqvgl.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/ghpvvxedj.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/gmlzzuttf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/guayfofhq.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/gmineyokt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/gyljtomdy.sHtML

[T35] Lua：字典表
来源：http://blog.fehbvm.com/Article/details/gufqdrqtu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gnkfrtjia.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/gvuzqyeje.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/gsvfodcdg.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fehbvm.com/Article/details/gwrukdgya.sHtML

"a" .. "b"
来源：http://www.share.hesvh.cn/Article/details/gjbcvfmkx.sHtML

[T38] Lua：条件
来源：http://wap.hesvh.cn/Article/details/gntecglfv.sHtML

if x > 0 then print("正") end
来源：http://m.share.zdbjq.cn/Article/details/gbsmxdpkx.sHtML

[T39] Lua：模式匹配
来源：http://baike.zdbjq.cn/Article/details/grnrxiude.sHtML

string.find(s, "%d+")
来源：http://3g.zdbjq.cn/Article/details/ghkffjwhb.sHtML

[T40] Lua：元表
来源：http://baike.fehbvm.com/Article/details/gxiqppyua.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.hesvh.cn/Article/details/gbkkqkcum.sHtML

[T41] Perl：Hello World
来源：http://wap.hesvh.cn/Article/details/gntzbqqxd.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/gqhjzuags.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/ginrzrgjr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.hesvh.cn/Article/details/gpbdavgof.sHtML

[T43] Perl：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gadgxltgw.sHtML

"值: $a"
来源：http://baike.zdbjq.cn/Article/details/gnnvlkfnj.sHtML

[T44] Perl：条件
来源：http://www.share.hesvh.cn/Article/details/gprvjcwnd.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/ginxytkqf.sHtML

[T45] Perl：数组遍历
来源：http://m.share.hesvh.cn/Article/details/gjdjoheuf.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fehbvm.com/Article/details/gksmjlaoo.sHtML

[T46] Perl：哈希操作
来源：http://blog.hesvh.cn/Article/details/gtlkrpbgh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.zdbjq.cn/Article/details/glxwcchkl.sHtML

[T47] Perl：正则捕获
来源：http://3g.zdbjq.cn/Article/details/gxziiusaq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.hesvh.cn/Article/details/gtwqmbgly.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/gniurrluo.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.hesvh.cn/Article/details/gvcyslfki.sHtML

[T49] Perl：函数
来源：http://www.m.share.hesvh.cn/Article/details/gruvwdbgi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gfmsmaykq.sHtML

[T50] Perl：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gorbdwijv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.zdbjq.cn/Article/details/guuiojjzu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmlbkewmj.sHtML

[T51] Scala：Hello World
来源：http://3g.hesvh.cn/Article/details/gblddjtjb.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gqsyzorqo.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/gwjevqqma.sHtML

val a = 1;  var b = 2
来源：http://www.blog.hesvh.cn/Article/details/gxcgsrkra.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gakqqrxoy.sHtML

s"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gqumwpklj.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gtxdivuzy.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/gucatajnf.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gxyteintx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gkkxsoyvm.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/gweuouvxb.sHtML


<!-- 参考信息 -->