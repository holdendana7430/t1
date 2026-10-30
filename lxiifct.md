代发 wailian999

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gliyaoxtc.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gicoroagz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqophkvq.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gzqakucci.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbrvlfil.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgpwfswt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gnjlriseq.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwgstozw.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gaqkidzgq.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gqzmtrmjk.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gxibgomal.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gcpmdgjbp.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gmhrqzzoe.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcayxlfc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhflqtyo.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxeortdhr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gxktikgzz.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/ggiyjikps.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gjfvqnfvj.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/ggwftfeib.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gysugdopf.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupwmcuen.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/greksnfsz.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gbxoyoiwd.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqroepom.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gittmadkr.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaeacpthp.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gszyjrkfy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gookyvauq.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/glyxaatrt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gugxzwlsu.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gnaxitdhu.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gzwnfnxea.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrilxecu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gihyjlmse.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gciodtgpa.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gloalsplq.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gclgqbdzt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfyuetydk.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gzirfopur.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gsifdtunb.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbvlyprn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gstqvcfsd.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gukflcblv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gbxthxqys.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gseeheppd.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxooetcs.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gviratywu.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gjkbqpgdp.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gxfzgnsqy.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gplsufqqd.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gevtarnwq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gucjjiwrq.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gtitvxosf.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gecrbiwhv.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlxceycz.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrbecmdu.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gbmmqstcd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/goeohupno.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/glfraoigs.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gescohjzd.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwxxiwup.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdugcggp.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyarezce.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gqilpbgha.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gelmbzins.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjucgghcx.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/galfeaeqq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjcxfmgo.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gsiaumtir.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/genyvljto.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlkmfpzj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjrzrdmy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuxpxayf.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gazkhmtwh.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gknddhsfv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfxhdovh.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbfyimkg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gspagyrdc.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibcwsfyb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqtqrvwm.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gmoaeplkn.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gnynkwzir.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/galxrtnxf.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/ghtkicymg.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gjzvuzcss.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwajiotgo.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/ghqknyddt.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gatexabri.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/ggotzvxqt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhwltirm.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmzbcicy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gblufjsou.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/grdotgldd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/glyucmvpg.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gudgzxecx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/gumvcwxci.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gxwbmxfio.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goygehkts.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gpaktnlco.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gkqamcunq.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozrnflmv.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssawgorh.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/ggwkhrcre.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhxwyhgz.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gkimitlmt.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjmmuuep.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gqoodiobc.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gfnklvgno.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gajpqrkno.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gbaralwlz.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gbocixbhm.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcwtuoom.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqmngsvd.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gaypdhoiq.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gmyghuqnr.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gsennzpxh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmuobgndc.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gbdhltrwn.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghopzunqm.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/grbucsllg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gawnjtmvq.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gipzscnwy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskffiajx.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gmlhrwqlc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcxcgbzs.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gzenkedgb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gcvyartmr.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvvgcsuf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggofxbwgk.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwvarees.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/guqkuplpc.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gujmfqzlp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/gtiaforea.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvkqgvdj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkjqadqw.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvdsqgeh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/ggaswozni.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnwsggyq.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gaazmhfzp.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxkcevok.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkeuzjnl.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gjyoigshr.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkvcffjf.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gtgmuscih.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/gwvlfhuyl.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkuqfsgol.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/goqwmpmfv.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gojlowdpq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfssbolgj.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqmeychi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwupfpui.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxhqpotw.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gwjecxpml.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcguilox.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gnxwukrdg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gajmtydcb.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gviqrwhvg.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/gkzaftsxm.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkahaume.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtykudlsm.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gjebgviso.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gzbubxuhe.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/ggidvaybo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmppxbcyv.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gvutsmgai.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvuokqwuz.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrxisgcz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpoulmbsm.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrtkromv.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gxqzdferr.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnbfocfz.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gjznkqktn.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsxugpoy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gyzbfusoo.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwlzccic.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gzugcyarz.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gbeoqebus.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgosntqe.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gvzyqfbzr.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvipzaeh.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gcopjifby.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gciugplxq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsgifrif.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/gtsyiwifq.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gnckbdtdk.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/glxzorerc.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhksncri.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyxylzvb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhkwzuuw.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gavdtibhc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpeniwbd.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gssxccyzc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gnyoelvvg.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqddlgcl.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbqokowr.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgdqhwyt.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwobawyk.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gzivkhirc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjpmirsz.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrsjyhio.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpijwsdg.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/geccvuyjr.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpttihrpx.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpsgkdnv.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjhkfpgx.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gmstfvsth.sHtML

for (i in 1..10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/ggktvxvvf.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdowcrve.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gweqvrama.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/grefdcecc.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjugxlkrv.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjjyfkft.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcysyotgi.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gpazcjrav.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gmiusvyxh.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gxvopaznk.sHtML

if let n = opt { print(n) }
来源：http://3g.fanxiaobao.xyz/Article/details/gcpggziim.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/gsdighjzg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfssadxjt.sHtML

[T21] Swift：遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gskhaxqus.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdotupxoj.sHtML

[T22] Swift：字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbylgjait.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/guhulgpvd.sHtML

[T23] Swift：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gywmxqxjl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gximuzhoe.sHtML

[T24] Swift：闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gtuhtknux.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/goonqrszu.sHtML

[T25] Swift：结构体
来源：http://baike.fanxiaobao.xyz/Article/details/gpztbfhcq.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvcwegeh.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givitdvej.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gteincwlo.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gpiirdugz.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyeztjkop.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gxffmlkpo.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/gnflilbrd.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/ghepxgdno.sHtML

guard let x = opt else { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gtvavmcsa.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/gpypwvjke.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwglurryp.sHtML

[T31] Lua：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/glwszhhqx.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqouwxvt.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrivievl.sHtML

local a = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gihnweiie.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/glibljhle.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdzgrmfe.sHtML

[T34] Lua：遍历表
来源：http://wap.fanxiaobao.xyz/Article/details/ghvtfluwe.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgcmcqsz.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdvrlmht.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gktyxhwgb.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gcskymomh.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslynnnds.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gilbxqckw.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/gajervgjh.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gltbwxhhb.sHtML

if x > 0 then print("正") end
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzzwdqib.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcuycdqb.sHtML

string.find(s, "%d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhmekrnx.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxmxwbsz.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzqaqyti.sHtML

[T41] Perl：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gsxmxqqnt.sHtML

print "Hello\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gqebyfbeh.sHtML

[T42] Perl：变量类型
来源：http://3g.fanxiaobao.xyz/Article/details/gqpnsdixr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggaurqppx.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gdssnlkwk.sHtML

"值: $a"
来源：http://baike.fanxiaobao.xyz/Article/details/ghlbazcov.sHtML

[T44] Perl：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/glyiuhqsu.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbqzocde.sHtML

[T45] Perl：数组遍历
来源：http://blog.fanxiaobao.xyz/Article/details/glklfxpmr.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/glwdfjbsi.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwnxwpsh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/guezqazzt.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/grgqtdcuz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gucvgwduo.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnoteqxoc.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptsukqqu.sHtML

[T49] Perl：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gfoiffozl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnoamepoi.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gpxdmktyd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fanxiaobao.xyz/Article/details/gpfngcgzk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggspqnqmb.sHtML

[T51] Scala：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gigcjoavx.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/glknjhzzz.sHtML

[T52] Scala：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/grbgmfpkp.sHtML

val a = 1;  var b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gngtqinxb.sHtML

[T53] Scala：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gpmqjbwml.sHtML

s"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/guaczkyqu.sHtML

[T54] Scala：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gcawtkefk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcskbbcul.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gjoxtiusk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gwisilpfp.sHtML

[T56] Scala：样例类
来源：http://3g.fanxiaobao.xyz/Article/details/gnmevjrrm.sHtML

case class User(name: String, age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gmevadrnz.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/givzbsrar.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzvbqvao.sHtML

[T58] Scala：函数定义
来源：http://read.share.fanxiaobao.xyz/Article/details/girpoiajb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrolngqw.sHtML

[T59] Scala：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gvocydvnn.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gcyizwyxh.sHtML

[T60] Scala：折叠
来源：http://3g.fanxiaobao.xyz/Article/details/gitdgiira.sHtML


<!-- 参考信息 -->