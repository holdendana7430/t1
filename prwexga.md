代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.zdbjq.cn/Article/details/gnggebybk.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gdmyblast.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/gpjmoincj.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/gbpxcxcsk.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/geigpdnpo.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gdjrqifvi.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/gnarcrfjk.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/gsqzsuxts.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/gexdznfco.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gnqokeiaj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gimwtlcfg.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/gqciqwflx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/ggtdrkaen.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/gyzxdwceh.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/gzrjqtina.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/gwnemhcme.sHtML

openssl rand -hex 16
来源：http://read.share.hesvh.cn/Article/details/gwkzclzpm.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gzhetzpmg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gjhyrmpim.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/gpwadqjoa.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gluiznpfg.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/ghqoaphbf.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/guzanphhs.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gmagdpvar.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/guorndujo.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/gugvobsrj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gviiwerhm.sHtML

[R73] 分割大日志
来源：http://www.blog.fehbvm.com/Article/details/gqpphgixh.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gpwllkvjd.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gssvoswol.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/ggjwmcjgx.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/gcipodijp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/gaximcxio.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/gjpnljaam.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gnraaovdv.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/gzxlyaarw.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/gudhfzpfi.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/ghixfzyof.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/gkshelbvl.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/girqrpvnh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/gdzzcxwpp.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/gpwtdhjyg.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/gyfnmbkkj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpzloxjgz.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/goqetgycz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvlqvfcap.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/gjebrogag.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/gfdbwqrgb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gasybebrg.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/gpiljdjwk.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/gndtskpcj.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/gbzkvobbw.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/geeppicth.sHtML

[S04] C：字符串复制
来源：http://m.share.fehbvm.com/Article/details/gnjvbtaco.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gbowhbuul.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gukzpaalh.sHtML

strlen(s)
来源：http://m.share.fehbvm.com/Article/details/gvrgbzibj.sHtML

[S06] C：字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gikrxvuij.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/glxcikfne.sHtML

[S07] C：数组遍历求和
来源：http://baike.zdbjq.cn/Article/details/gztqewwit.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/gilkovreu.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/gmufbetfs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gdviqzjlg.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/gdwooalyg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.zdbjq.cn/Article/details/gbfrkcwqs.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gnwcwecol.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/gkoueugyp.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gmvwglvqc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fehbvm.com/Article/details/gzuixrdir.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/glcpjgvhg.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/glztagjnz.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gwzvhmely.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/gldrrndza.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/gxrauyyou.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/guszylzec.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/gmdtaydsh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/gfkmeiyhy.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/gkbfrqwnx.sHtML

(double) a / b
来源：http://baike.fehbvm.com/Article/details/grgeldtwv.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/gtbivvhtk.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/gaobzplcj.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/gullrqzqw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gngdsxfcu.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gvfgnmzpz.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/gdumzomjx.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/giozubdnv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/ggtagenna.sHtML

[S20] C：二分查找
来源：http://wap.hesvh.cn/Article/details/gxkkbkxaf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/grkempiib.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/ggcahywnw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gbejvjkuz.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gzenuceat.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/gsjzwxpdu.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/gwrhgsgwy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/gdneanada.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gfhcrqibu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/gzamifngx.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/gajawfvwl.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/gzzqlvxoj.sHtML

[S26] C：内存清零
来源：http://www.share.fehbvm.com/Article/details/gernvfqih.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fehbvm.com/Article/details/glxakpqst.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/grcvkqbvq.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gjbucxnhb.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/gatcfungk.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/gjfnvxbpw.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/guaxxnjwg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/gqyomuxiz.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/gvyvoilyk.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/gnorbjlyc.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/gdapdxluo.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/govomkqew.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gxeraobyr.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/ghgblmwxm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/gqeexdeno.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/gpgiyicyw.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.hesvh.cn/Article/details/gnmpjxitq.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/gwmjnwjdi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gehdkpvic.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/gfswafhnq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/gwuyecive.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/grexvuaks.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gfthovwtu.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/gksuafqtf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gtljmanct.sHtML

[S37] C++：set
来源：http://www.blog.zdbjq.cn/Article/details/gmkxowpym.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/ggekfypxd.sHtML

[S38] C++：排序
来源：http://www.share.zdbjq.cn/Article/details/gbuubglig.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gbnukfpcq.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/gebxpjvur.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.zdbjq.cn/Article/details/guzdtwtkq.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gbrvdovwb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/gkhktvlns.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/gaiaqjygi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/giswggxzq.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gnufpntrk.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/grtyqcktg.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/gpnyiaiws.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.zdbjq.cn/Article/details/ghklynxhw.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gryunwvhl.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/gptsiftcs.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gosfvfqen.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.hesvh.cn/Article/details/gqxhpkihn.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gqzpkicly.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/garnaytbg.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gckarxgpr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gulxwbsgj.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/grchjvpvj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/grtxeelhd.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/gpddpzfej.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gvuhclied.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/gwcrlqhyu.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gnsbkopuk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gkvmewzib.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/gzgdffkau.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/ghzahljnd.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/gyqcfgksg.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.zdbjq.cn/Article/details/gqvkdsjww.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/gwnrjzqrs.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fehbvm.com/Article/details/gzqluczyf.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/gjblswvjp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gdiuabruv.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gptybgxtk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gqkvhfudi.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/gznkkzvpf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/gmjkhxgun.sHtML

[S57] C++：编译期常量
来源：http://3g.fehbvm.com/Article/details/gdzxhtzqt.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gvqqcvhny.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/glrpfcsbn.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.hesvh.cn/Article/details/ggxppzlvp.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gftolepiw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gcxndehps.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/gcajdrszt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/gbjsannbn.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsjcghfrt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gmqitiexm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzerzicif.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gjjxshogp.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gjzcnxglk.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/gbbbiesbn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/ggonudskm.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/guuennxpr.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gdnbnwrqo.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/gfjjxjpgd.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.zdbjq.cn/Article/details/gzuwmlrgk.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gtrldbgvi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/gpmokywwc.sHtML

[T06] Kotlin：集合映射
来源：http://baike.zdbjq.cn/Article/details/gczzrirvc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.zdbjq.cn/Article/details/glepwxgwu.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/gsbprlulb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/gixmpzuat.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gzndsitse.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.hesvh.cn/Article/details/gzhvknlxc.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.hesvh.cn/Article/details/gyjbafyue.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/gwmgzwzwr.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gdojgwwqd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gowltlymv.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/gqsbeawlj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/gjkcdryxr.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/gopbpwfvd.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gnbrznzus.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.zdbjq.cn/Article/details/gjrkqmawp.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/gtzbldcah.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/gpoxtbdwl.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/giubbqhau.sHtML

[T15] Kotlin：接口
来源：http://read.share.hesvh.cn/Article/details/gothcgipo.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/guyhoxkff.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/gtiqrnvio.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/goazkmrbi.sHtML

[T17] Swift：变量与常量
来源：http://baike.hesvh.cn/Article/details/gxklfjguc.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/gwrdzlhgl.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/gictwmmki.sHtML

"值: \(b)"
来源：http://baike.hesvh.cn/Article/details/gjhvzlzps.sHtML

[T19] Swift：可选绑定
来源：http://wap.hesvh.cn/Article/details/ghapvrmfp.sHtML

if let n = opt { print(n) }
来源：http://baike.fehbvm.com/Article/details/gmczhfduk.sHtML

[T20] Swift：数组操作
来源：http://www.share.fehbvm.com/Article/details/gnzvnnimz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.hesvh.cn/Article/details/gfbfklowg.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/ghuthiszf.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/gottcurof.sHtML

[T22] Swift：字典
来源：http://m.share.hesvh.cn/Article/details/gsgsyonrh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fehbvm.com/Article/details/givxyilgq.sHtML

[T23] Swift：函数
来源：http://blog.fehbvm.com/Article/details/gsybbwftf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/gncltftms.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/gmxodygox.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gqikighlw.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/gcunfglpt.sHtML

struct P { var x: Int }
来源：http://www.blog.fehbvm.com/Article/details/gxmekgdjw.sHtML

[T26] Swift：类与重写
来源：http://m.share.zdbjq.cn/Article/details/gfhedaotk.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.hesvh.cn/Article/details/gmkzgvxtx.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gsixsczwi.sHtML

do { try f() } catch { print(error) }
来源：http://baike.zdbjq.cn/Article/details/gadwsyhls.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/gjwbfvrka.sHtML

enum Color { case red, green }
来源：http://blog.hesvh.cn/Article/details/gupkplkip.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fehbvm.com/Article/details/glkahokih.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/gfvualgpk.sHtML

[T30] Swift：协议
来源：http://blog.fehbvm.com/Article/details/giztqkbbd.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/glwletdhz.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gegtcrslz.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gtkvazjow.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/gepdazvic.sHtML

local a = 1
来源：http://baike.zdbjq.cn/Article/details/govykixrl.sHtML

[T33] Lua：表（数组）
来源：http://m.share.zdbjq.cn/Article/details/gmdppraca.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.zdbjq.cn/Article/details/gttcesqpp.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/gbkipgjze.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/gosvpnkgg.sHtML

[T35] Lua：字典表
来源：http://m.share.hesvh.cn/Article/details/giuoqnyob.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/gfqleeeva.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/gtxegthwj.sHtML

function add(a, b) return a + b end
来源：http://read.share.zdbjq.cn/Article/details/gwewhatgs.sHtML

[T37] Lua：字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gfcqciabc.sHtML

"a" .. "b"
来源：http://read.share.zdbjq.cn/Article/details/gqdhwilmi.sHtML

[T38] Lua：条件
来源：http://blog.fehbvm.com/Article/details/gdyjozrso.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/gsyclcxof.sHtML

[T39] Lua：模式匹配
来源：http://3g.hesvh.cn/Article/details/ghwqozxfc.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/gkdyucnuk.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/gnitaxquk.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.zdbjq.cn/Article/details/gdviswxlq.sHtML

[T41] Perl：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gagjlwjlw.sHtML

print "Hello\n";
来源：http://www.blog.zdbjq.cn/Article/details/gpqsztced.sHtML

[T42] Perl：变量类型
来源：http://read.share.fehbvm.com/Article/details/guffcvakt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.hesvh.cn/Article/details/gimnhvyml.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/ggdpoynqb.sHtML

"值: $a"
来源：http://m.share.fehbvm.com/Article/details/gzpmsqhca.sHtML

[T44] Perl：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gtghimepu.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fehbvm.com/Article/details/gkovtdzzo.sHtML

[T45] Perl：数组遍历
来源：http://mobile.zdbjq.cn/Article/details/gqrirxemp.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.zdbjq.cn/Article/details/gvlbtiwft.sHtML

[T46] Perl：哈希操作
来源：http://baike.hesvh.cn/Article/details/gcptvwpbv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.zdbjq.cn/Article/details/gcibclapm.sHtML

[T47] Perl：正则捕获
来源：http://www.share.zdbjq.cn/Article/details/gfwvizsqc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fehbvm.com/Article/details/gxcvydrhg.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gprtiecrh.sHtML

$s =~ s/old/new/g;
来源：http://baike.zdbjq.cn/Article/details/grjzipeoj.sHtML

[T49] Perl：函数
来源：http://baike.hesvh.cn/Article/details/ggdqyfwzr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gakyszexl.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gvwgibmrq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.hesvh.cn/Article/details/gynxhacck.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fehbvm.com/Article/details/gherqqbjr.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gndexklxr.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/goyzngygf.sHtML

[T52] Scala：变量
来源：http://www.blog.zdbjq.cn/Article/details/gkuyqgimv.sHtML

val a = 1;  var b = 2
来源：http://3g.fehbvm.com/Article/details/gnrcjwwjr.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/ghqbilcyt.sHtML

s"值: $b"
来源：http://wap.fehbvm.com/Article/details/ggthluhit.sHtML

[T54] Scala：集合映射
来源：http://www.share.fehbvm.com/Article/details/gtylfavzd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.zdbjq.cn/Article/details/gjxefkhbu.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gfvtqwizm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.zdbjq.cn/Article/details/garcadzhm.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/gxvekvcgt.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gjlfzfjxh.sHtML

[T57] Scala：模式匹配
来源：http://3g.hesvh.cn/Article/details/glakafson.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.zdbjq.cn/Article/details/gjzsnlonj.sHtML

[T58] Scala：函数定义
来源：http://read.share.hesvh.cn/Article/details/gbkiaoowc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.zdbjq.cn/Article/details/gprjwlxlp.sHtML

[T59] Scala：循环
来源：http://3g.hesvh.cn/Article/details/gudyyburj.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fehbvm.com/Article/details/gdgqblgnx.sHtML

[T60] Scala：折叠
来源：http://3g.zdbjq.cn/Article/details/gdpskoznz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fehbvm.com/Article/details/glsrinkaa.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ginpurzby.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/gihjcexhe.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtjtkrioi.sHtML


<!-- 参考信息 -->