代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.zdbjq.cn/Article/details/gblerxroq.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/grgcmqutl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/gqdlrdnsr.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/gytulnfiz.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/gzstsvizr.sHtML

[R62] 找最占空间的文件
来源：http://baike.zdbjq.cn/Article/details/ggnwtoqxe.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/gaxpcyrtk.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/gdysoofmo.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/gzduroahx.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/gnufuxpuv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/gbdwjagzz.sHtML

[R65] 查看端口占用
来源：http://m.share.hesvh.cn/Article/details/gyryxmqty.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.zdbjq.cn/Article/details/gswhzvcac.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gmizvesuc.sHtML

crontab -e;  crontab -l
来源：http://read.share.fehbvm.com/Article/details/gpbkjjpwc.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/gducjpgmc.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/gkseownml.sHtML

[R68] 计算文件校验值
来源：http://blog.zdbjq.cn/Article/details/gldwzghdw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/gazczbast.sHtML

[R69] 生成随机密码
来源：http://www.blog.fehbvm.com/Article/details/gkplzcbha.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.hesvh.cn/Article/details/gdbvyxucr.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/gdhyzleao.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/gqxlmtirk.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gqokayswd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/gkbluutcy.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gwmxtcvmb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gpvjnayzy.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gomyidlvx.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/gsxexktgq.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gqiwptjyp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gdzhotvks.sHtML

[R75] 导出环境变量
来源：http://www.share.hesvh.cn/Article/details/gpeidulxx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/gtvepkmwp.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gkqgfvbhp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gphxtvpgd.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gfpogidvk.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/gohzxckjt.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gncicrsia.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gkristazv.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/gbmogfkmg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/gwlebspgy.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/gpkkzmetl.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/gzlpqhmcn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmpzdhuuo.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/gmrkkxmrf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpcpiqtlm.sHtML

[S01] C：Hello World
来源：http://mobile.hesvh.cn/Article/details/gqnqfmjli.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/gwmzwfxfe.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/grkshcrpx.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/glviroxkj.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/gbvcchmxo.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/gonusfafw.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/giiqlaihp.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/geblfscvb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gbwohkwqr.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gyblddgbl.sHtML

strlen(s)
来源：http://www.blog.zdbjq.cn/Article/details/ggdnasdow.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/gfkbrolco.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/gpsyktvjq.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fehbvm.com/Article/details/gdrlxzkcd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gicabnavz.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/gdmgscjxe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fehbvm.com/Article/details/gfpvikfnt.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gpcnaxijx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fehbvm.com/Article/details/gmmvkdikq.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gvinobwmz.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/gvdbttuyr.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gcsrausqb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.zdbjq.cn/Article/details/gfjkvjvmr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gnokkeqpy.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gawrdotnq.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/gqrxlrjqx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gpostyhll.sHtML

[S13] C：宏定义
来源：http://mobile.hesvh.cn/Article/details/glsdtzdks.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/gvrqxjmsp.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/guvjrkwhq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/gldszfcxf.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/gructsplo.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/gdxanblwf.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gxujbtcfr.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/gkkvjgukp.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gfiiecqub.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/gbxsvtgcj.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/gocmxbwjk.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gpmdkwpry.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gqrukzsbe.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gshtazocc.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gdnmkcopy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gnlptlhqt.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/gstapwkgc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/gahqdzymn.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/glupwsdwc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/gpoicnqlo.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gvyebbbga.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/gffyznwev.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gzskgegdp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.hesvh.cn/Article/details/gndcblpwl.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/gtjaqoend.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/gjwaezopl.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gyczpmwuq.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/gwdnlrequ.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gziowaaww.sHtML

const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gyuduqvue.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/guzuqysol.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gjhtvgtjt.sHtML

[S29] C：变参函数
来源：http://mobile.hesvh.cn/Article/details/glvbdedmp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gvzrzgqsr.sHtML

[S30] C：头文件保护
来源：http://blog.zdbjq.cn/Article/details/gbjoxhaux.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/glhulawlt.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gohzkwkzz.sHtML

#endif
来源：http://mobile.zdbjq.cn/Article/details/gshhcbevu.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gbmdgsiwa.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/gjazhmysg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/gkgcpsgyo.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/gxrwbqtjv.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/goasemfiw.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/gqlcbcptp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/gkkjgpkeu.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fehbvm.com/Article/details/gbnrnalvk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/gzbrwdnkj.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/goamwizxa.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/grsbaaaaa.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/gehngvvja.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/ghnskukvb.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/gvjgazgtj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.zdbjq.cn/Article/details/gzpwqskpx.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gudnrbndc.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/gvdijzpfk.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gyrkpqyit.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/gvenavwby.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/grjnfwgbf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/gnskzoedr.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gwthhsdnt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fehbvm.com/Article/details/gxubtxycm.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/gekmasxtn.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/gubuegzie.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/gkzmvitmw.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gppuxezgt.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/gmhkuumcp.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/goaasvsnm.sHtML

[S45] C++：lambda
来源：http://www.blog.hesvh.cn/Article/details/gytkyspws.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/gvachvvvg.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/gbgaoncqh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.hesvh.cn/Article/details/gulghqizx.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fehbvm.com/Article/details/gllsktfuo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.zdbjq.cn/Article/details/gtqbqcfeq.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gbhcqjrcg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.zdbjq.cn/Article/details/gnuhnyedj.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/gdhzrlhbq.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/gjfqpaxor.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/gkucgvfun.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/gtkfxwqdb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gzizuoksl.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/gfwlnmimf.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gaikuvebg.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/gfwdfumph.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.zdbjq.cn/Article/details/gqhwpslos.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/gzcwbjopr.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fehbvm.com/Article/details/gvgftvfoq.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/ggmqneata.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fehbvm.com/Article/details/gxpnigysk.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/guzjideet.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/glcdribcm.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/gsawbolmh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gocvwhkmu.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/gsfropaio.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/gueikkwaj.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/gawdenrtb.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/ghcjuifox.sHtML

[S59] C++：静态断言
来源：http://mobile.hesvh.cn/Article/details/ghejmncas.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/gcwhllsfv.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/geqpitwow.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/gjuofizpb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/glnarfjiu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gwklnagpq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gstzulism.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gnolqmpfw.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/glalloesw.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gepgvdlcj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/goxmiglpd.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/golkloixl.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gtozeqfxg.sHtML

[T04] Kotlin：空安全
来源：http://baike.hesvh.cn/Article/details/gohjuwrwb.sHtML

val n: String? = null;  n?.length
来源：http://3g.zdbjq.cn/Article/details/gvyagghaw.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gysetfaxv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gxjktzqhn.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gbystcgsg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gsfmcfgrk.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gnommbxeb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.zdbjq.cn/Article/details/gjdkwrucq.sHtML

[T08] Kotlin：数据类
来源：http://www.share.hesvh.cn/Article/details/ghoilxrud.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gjtbymmts.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/gtpceiwoz.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gfxzkonyl.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/gedeecggm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.zdbjq.cn/Article/details/ghlttucxa.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/geijpmyak.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/gvdnjrher.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.hesvh.cn/Article/details/gtdnpkrww.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/gibniiodo.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/guxdjqrub.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/gfhxdtxbe.sHtML

[T14] Kotlin：循环
来源：http://wap.hesvh.cn/Article/details/gqokywcue.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/gsguqexui.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gsmcrkzjp.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gvxwjzxvq.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/ggqgoklfh.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gryyfosam.sHtML

[T17] Swift：变量与常量
来源：http://blog.zdbjq.cn/Article/details/gwzfqnsrt.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/gunzierxs.sHtML

[T18] Swift：字符串插值
来源：http://blog.zdbjq.cn/Article/details/grhcxntrr.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/gswsktshk.sHtML

[T19] Swift：可选绑定
来源：http://www.share.zdbjq.cn/Article/details/gzfwijdnl.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/goytvgdlo.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/gtfpryhco.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.hesvh.cn/Article/details/gjnyyiaqm.sHtML

[T21] Swift：遍历
来源：http://m.share.fehbvm.com/Article/details/gwyipatoe.sHtML

for x in a { print(x) }
来源：http://blog.zdbjq.cn/Article/details/gjmbanlyb.sHtML

[T22] Swift：字典
来源：http://baike.zdbjq.cn/Article/details/glbkemocd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fehbvm.com/Article/details/ghsikdryg.sHtML

[T23] Swift：函数
来源：http://read.share.hesvh.cn/Article/details/gnvqdidwi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/genlxtxob.sHtML

[T24] Swift：闭包
来源：http://read.share.zdbjq.cn/Article/details/gaqcoggis.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.hesvh.cn/Article/details/grerohpbo.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/gagfufddf.sHtML

struct P { var x: Int }
来源：http://www.m.share.zdbjq.cn/Article/details/gvaliuxys.sHtML

[T26] Swift：类与重写
来源：http://wap.hesvh.cn/Article/details/ghkoampvf.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/grtwqcmji.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/gdlvkdzbg.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/grqguzkfk.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/grrpwcyrl.sHtML

enum Color { case red, green }
来源：http://blog.hesvh.cn/Article/details/gsjoseidl.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gnrwzlaii.sHtML

guard let x = opt else { return }
来源：http://www.blog.fehbvm.com/Article/details/gzkhounjt.sHtML

[T30] Swift：协议
来源：http://3g.hesvh.cn/Article/details/glozztlsf.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/gxebupsil.sHtML

[T31] Lua：Hello World
来源：http://read.share.fehbvm.com/Article/details/gqmyqvvzv.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gbsgrfbsb.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/gzhkbilua.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/googegrwq.sHtML

[T33] Lua：表（数组）
来源：http://m.share.zdbjq.cn/Article/details/gooupjqra.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/ggtaalmxe.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/gxktznzrj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/gpaahyfig.sHtML

[T35] Lua：字典表
来源：http://www.share.zdbjq.cn/Article/details/gvkshjnir.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/gzwelxwtw.sHtML

[T36] Lua：函数
来源：http://read.share.zdbjq.cn/Article/details/getggfcfc.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/ggbgbnmge.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gquyjauch.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/gtohwhmvk.sHtML

[T38] Lua：条件
来源：http://blog.zdbjq.cn/Article/details/gpqxxjsaw.sHtML

if x > 0 then print("正") end
来源：http://read.share.hesvh.cn/Article/details/gmflesufg.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gkqikwpgp.sHtML

string.find(s, "%d+")
来源：http://www.blog.fehbvm.com/Article/details/gcbjmbzou.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/gcrqqprwm.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/gjnxdbgpv.sHtML

[T41] Perl：Hello World
来源：http://blog.hesvh.cn/Article/details/gaxjigutl.sHtML

print "Hello\n";
来源：http://wap.zdbjq.cn/Article/details/gimuhbktd.sHtML

[T42] Perl：变量类型
来源：http://read.share.hesvh.cn/Article/details/giqeukjef.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/gqppcbwcb.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gcpncphrj.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/guttejlib.sHtML

[T44] Perl：条件
来源：http://mobile.hesvh.cn/Article/details/gegiepwbt.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.zdbjq.cn/Article/details/gqlnizkzt.sHtML

[T45] Perl：数组遍历
来源：http://www.share.hesvh.cn/Article/details/gyticcovx.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/gynolonvg.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/guhvxaxix.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/gnwhqntuc.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.hesvh.cn/Article/details/gxhzecazv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.hesvh.cn/Article/details/gmhkejdvc.sHtML

[T48] Perl：正则替换
来源：http://www.blog.hesvh.cn/Article/details/gjgbvjque.sHtML

$s =~ s/old/new/g;
来源：http://3g.fehbvm.com/Article/details/ghhxqpmwm.sHtML

[T49] Perl：函数
来源：http://blog.hesvh.cn/Article/details/gnweqjmwf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gtpdepzkp.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gqavczalb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.hesvh.cn/Article/details/guavtqkup.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.hesvh.cn/Article/details/ggjemuena.sHtML

[T51] Scala：Hello World
来源：http://3g.hesvh.cn/Article/details/ghbgasamn.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gzjyxbctj.sHtML

[T52] Scala：变量
来源：http://blog.zdbjq.cn/Article/details/gtxuvogbh.sHtML

val a = 1;  var b = 2
来源：http://baike.fehbvm.com/Article/details/ghjhopfmg.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gvhqatbpl.sHtML

s"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gydhewaow.sHtML

[T54] Scala：集合映射
来源：http://www.share.hesvh.cn/Article/details/gojjjbqmy.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gwaptdqid.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/ghvrakadb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fehbvm.com/Article/details/gtgflehrg.sHtML

[T56] Scala：样例类
来源：http://blog.fehbvm.com/Article/details/grtgjsjyw.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gakvugdsw.sHtML

[T57] Scala：模式匹配
来源：http://wap.fehbvm.com/Article/details/gxcsvnyqz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.hesvh.cn/Article/details/gnecwhvvl.sHtML

[T58] Scala：函数定义
来源：http://3g.fehbvm.com/Article/details/gfcgvltai.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.hesvh.cn/Article/details/gvkizrsvn.sHtML

[T59] Scala：循环
来源：http://www.blog.hesvh.cn/Article/details/gueuonbhr.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gcuzakjtc.sHtML

[T60] Scala：折叠
来源：http://blog.fehbvm.com/Article/details/gyruxfkhk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/gmsjbjhyi.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghponypdh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gsopegigk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxtlglcrp.sHtML


<!-- 参考信息 -->