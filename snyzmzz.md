代发 wailian999

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/gegwdgqfk.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/gqtujzmwp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gtwzzlzzy.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/gipkeiuvu.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/gwelimbfr.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/gfhwbggpv.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/gpdgjeuly.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gysiptigz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gqlghfvwb.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gbkokfats.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gklspcssc.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gxdvekiha.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/gzzzrjjga.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/gfrvyauit.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/gpbnxtdgi.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/gtrdausde.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/gpejvsykf.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/gfkdoqsws.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gcneauxut.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/gvcmnzoqy.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/gaefvrlxd.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/gomwudqkg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/gryomnupr.sHtML

[R79] 解析命令行选项
来源：http://mobile.hesvh.cn/Article/details/gxvytzkuv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/gvubagvdb.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/ghptzccaq.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/gjxhzhyhi.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzfjmmtbd.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/gvoxvxdvj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gixhrjvip.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/gkcvontcv.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gbynqekak.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/glmhrzacp.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gjlelshmt.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gshdqcyvn.sHtML

[S03] C：读入整数
来源：http://baike.hesvh.cn/Article/details/gsngvunqm.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gnrzadqdz.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gorxqgfts.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/glemtopcn.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gmgqkelmb.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/grgzicypd.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gchwzoapl.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/gufqacgeg.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/ghivyadyb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fehbvm.com/Article/details/gsezebizx.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gfzsxymlp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fehbvm.com/Article/details/gereynpvm.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gsaztvobm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/givqbasrv.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gqkjzxuwg.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/gxmooagpn.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gkwikwpui.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/gxygiatnw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/ggcfrbtzw.sHtML

fclose(f);
来源：http://baike.hesvh.cn/Article/details/gqfgnscjp.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/gmbdgrgyl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gvmhoholv.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/gjcbfmtgv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gjeifufmp.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/gpyedrtkd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gbgspyfuy.sHtML

[S15] C：类型转换
来源：http://wap.fehbvm.com/Article/details/gqhybbqde.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/guqmcxuos.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/gtwwjpsce.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/gdlglsydj.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gfqcswldq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gltymencl.sHtML

[S18] C：命令行参数
来源：http://3g.fehbvm.com/Article/details/glgtdmpvf.sHtML

int main(int argc, char **argv)
来源：http://wap.hesvh.cn/Article/details/gdxebruau.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/ggvhofiho.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gblejbqsk.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/glvzxwhof.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gvxvvtyzo.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/glqqjckhq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/gtqytfryc.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gjeonnyhw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/ghsevbmhy.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/gvchsmjky.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.zdbjq.cn/Article/details/gxkwnjinl.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/gnwvhoalw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/gmfdndazu.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/gjhvdxhnc.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gfqjdydnk.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/gxwfmbqkf.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/ghnpraffb.sHtML

[S27] C：定义常量
来源：http://mobile.hesvh.cn/Article/details/gdpnxints.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gnqxbfbfd.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/gtybpegsd.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gfbpmcaiy.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/goxtyxffo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gfkxvjqqz.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gihjweutz.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/gzjattkgl.sHtML

#define X_H
来源：http://www.share.zdbjq.cn/Article/details/glgrtlbcg.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/gmvctnpdr.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/godlmbyli.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gbscsulnb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/gvtjmzelt.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/glkbjcpet.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/gqrwrchor.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gquhnlujf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/glkeouhbj.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/gsiyiyzyt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsbwyaubr.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/gcgtbvzoa.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gyrrhmqpk.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/guymfnufn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gmdftuuee.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/ggtuzouxt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gysyvxjgj.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/gfnmbzade.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/glimwjejr.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gdnvauixk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.zdbjq.cn/Article/details/gwhpiatdh.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gireszkil.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gmzqzhell.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gyvqejmen.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.zdbjq.cn/Article/details/gmrpvsuww.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.hesvh.cn/Article/details/gibmmlpgy.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gmtjlcwfs.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/gwvrhauuy.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/gmxajrjiz.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gilveswjc.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/grtbbtzmi.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/gppqissrg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/gvowbbeum.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/gxerivaov.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gpxzccpih.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gheeoiurx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gwyemlqpf.sHtML

[S48] C++：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gjaafscrd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/griiogdfl.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/gamzjowaj.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/gybzibbch.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/gtcwdwvfy.sHtML

[S50] C++：格式化数字
来源：http://blog.zdbjq.cn/Article/details/gnstlwtjv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gsbxeqpkl.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/geooxqgmm.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/guaeklons.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/grqqvifek.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/gdvupwshz.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/gfwsogiur.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/ghcmnenci.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gyckchzbd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fehbvm.com/Article/details/gaqrwhwsv.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/gfrrzogrl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gxlaukadt.sHtML

[S56] C++：optional
来源：http://www.blog.zdbjq.cn/Article/details/gaasfubud.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/gxjyiofpo.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/gmdyjsial.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/goymnfpoa.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/gvbspccrk.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.zdbjq.cn/Article/details/goyivjyiz.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/gctphssvr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/ggiioqiwb.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/gafcomwdx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gjrczknsa.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkowwkpxk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gffussqxe.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggunhmvnt.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/gvbowmrew.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gfusorpta.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/gdwwomvyy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/gohgiszsq.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/gdirlavnm.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gdegxfgtw.sHtML

[T04] Kotlin：空安全
来源：http://mobile.zdbjq.cn/Article/details/gffsjqvbm.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/gqrnxyomv.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gztggsssw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/gdkfwtwoo.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/grcfjptfg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/grrzcmvcm.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.hesvh.cn/Article/details/gukgritvl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/gicnkfcjk.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/ggqcstlto.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/gnowmyfbw.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.zdbjq.cn/Article/details/gbnrwnjfi.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gskerpurt.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fehbvm.com/Article/details/gzvjfpojf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/gswawzrrl.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/gotgwtoro.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/goslmkthu.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gzjntobpn.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gtplrmfpo.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.zdbjq.cn/Article/details/gcthlayxs.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.hesvh.cn/Article/details/gwmuplgaw.sHtML

[T14] Kotlin：循环
来源：http://baike.fehbvm.com/Article/details/gkexinfnx.sHtML

for (i in 1..10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gvawwrmct.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gpsccqscr.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/gzsdxcjer.sHtML

[T16] Swift：Hello World
来源：http://blog.fehbvm.com/Article/details/gufgtnwnu.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gupkwfbds.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/gttususwt.sHtML

var a = 1;  let b = 2
来源：http://3g.fehbvm.com/Article/details/gslfibrki.sHtML

[T18] Swift：字符串插值
来源：http://read.share.hesvh.cn/Article/details/goqkfedgg.sHtML

"值: \(b)"
来源：http://www.blog.fehbvm.com/Article/details/gixutpmik.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/grzrkfsxp.sHtML

if let n = opt { print(n) }
来源：http://read.share.hesvh.cn/Article/details/ggbjngmlr.sHtML

[T20] Swift：数组操作
来源：http://mobile.zdbjq.cn/Article/details/glsceotcf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fehbvm.com/Article/details/getzbplgz.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/gwlkxamqx.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/gasbokmhj.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/glxjlrnsa.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/goklvxblt.sHtML

[T23] Swift：函数
来源：http://baike.zdbjq.cn/Article/details/ghqffmydi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/ghsyafkdr.sHtML

[T24] Swift：闭包
来源：http://m.share.hesvh.cn/Article/details/gbpsejyer.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gzzrmhokz.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/gzzjgolxe.sHtML

struct P { var x: Int }
来源：http://www.blog.fehbvm.com/Article/details/gmwxwoyyj.sHtML

[T26] Swift：类与重写
来源：http://read.share.hesvh.cn/Article/details/gxnqppemy.sHtML

class A: Base { override func f() {} }
来源：http://baike.fehbvm.com/Article/details/gllqwortg.sHtML

[T27] Swift：错误处理
来源：http://read.share.fehbvm.com/Article/details/gymtemvnu.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gzwsqglvt.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/gkuldmrrv.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/gczmnszox.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.zdbjq.cn/Article/details/gdagsbiwh.sHtML

guard let x = opt else { return }
来源：http://wap.zdbjq.cn/Article/details/gskeqzfrg.sHtML

[T30] Swift：协议
来源：http://www.share.zdbjq.cn/Article/details/ghybetwor.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/glozorrdl.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/gjuoyowbt.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gtrqvnzoj.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/goxvnuray.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/gqaanabne.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/ggzfvcyve.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fehbvm.com/Article/details/gwityvzuj.sHtML

[T34] Lua：遍历表
来源：http://m.share.zdbjq.cn/Article/details/gjhqhtmol.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.hesvh.cn/Article/details/gegxtfgkl.sHtML

[T35] Lua：字典表
来源：http://m.share.zdbjq.cn/Article/details/gyakiaztx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.hesvh.cn/Article/details/gbkwwyvkg.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/gexhujlwr.sHtML

function add(a, b) return a + b end
来源：http://www.share.hesvh.cn/Article/details/gtgystdaf.sHtML

[T37] Lua：字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gveimilzd.sHtML

"a" .. "b"
来源：http://www.m.share.hesvh.cn/Article/details/gvykappik.sHtML

[T38] Lua：条件
来源：http://m.share.fehbvm.com/Article/details/gqcbahmbc.sHtML

if x > 0 then print("正") end
来源：http://baike.hesvh.cn/Article/details/gfnddhpey.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gzvzrbrut.sHtML

string.find(s, "%d+")
来源：http://3g.hesvh.cn/Article/details/gnguoafsh.sHtML

[T40] Lua：元表
来源：http://3g.fehbvm.com/Article/details/gxyqbqjxw.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.zdbjq.cn/Article/details/gefihqhnk.sHtML

[T41] Perl：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gxxjhhlsu.sHtML

print "Hello\n";
来源：http://www.share.zdbjq.cn/Article/details/gaodkvspu.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/gkwqdmvhw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fehbvm.com/Article/details/gaooivbev.sHtML

[T43] Perl：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gsuojhocm.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/gbqtqaymc.sHtML

[T44] Perl：条件
来源：http://read.share.hesvh.cn/Article/details/gaevlihte.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/gfggxojkm.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.zdbjq.cn/Article/details/gaoilcnhc.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.zdbjq.cn/Article/details/gegwrwyno.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/gggflnolv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/gyzmfhbsg.sHtML

[T47] Perl：正则捕获
来源：http://baike.zdbjq.cn/Article/details/gqvdlpuzz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.zdbjq.cn/Article/details/gmjnsbzcn.sHtML

[T48] Perl：正则替换
来源：http://baike.fehbvm.com/Article/details/gsnpgeppf.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.zdbjq.cn/Article/details/gdzuapyri.sHtML

[T49] Perl：函数
来源：http://www.m.share.hesvh.cn/Article/details/gfnxcysto.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/grllwvnhe.sHtML

[T50] Perl：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gohvvmeft.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.zdbjq.cn/Article/details/gwuuzhyqg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fehbvm.com/Article/details/gkifwalty.sHtML

[T51] Scala：Hello World
来源：http://wap.fehbvm.com/Article/details/gdwzktxaq.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/glziueevd.sHtML

[T52] Scala：变量
来源：http://mobile.fehbvm.com/Article/details/gllrzndyy.sHtML

val a = 1;  var b = 2
来源：http://m.share.hesvh.cn/Article/details/ghplncccf.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gztfpbxea.sHtML

s"值: $b"
来源：http://wap.fehbvm.com/Article/details/gxusljrcl.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gwiwshgdf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.zdbjq.cn/Article/details/gbhlupyvl.sHtML

[T55] Scala：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gimwietqs.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/grbzyykui.sHtML

[T56] Scala：样例类
来源：http://blog.fehbvm.com/Article/details/gedknnemf.sHtML

case class User(name: String, age: Int)
来源：http://baike.zdbjq.cn/Article/details/gadnvoqck.sHtML

[T57] Scala：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gsfodmcry.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/ggeevdovv.sHtML

[T58] Scala：函数定义
来源：http://www.blog.zdbjq.cn/Article/details/grxlwrfjr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fehbvm.com/Article/details/gonnjoiyi.sHtML

[T59] Scala：循环
来源：http://read.share.hesvh.cn/Article/details/gciohsmkz.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/gndrvqqhf.sHtML

[T60] Scala：折叠
来源：http://m.share.hesvh.cn/Article/details/gapedrcqm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fehbvm.com/Article/details/gqicvykca.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gweqwebgv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/gluxvdryy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghhnaqzsv.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.hesvh.cn/Article/details/gnauryuva.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.hesvh.cn/Article/details/gbsuvrykr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/gzkopokvf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/gdjqrdnqt.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.hesvh.cn/Article/details/gnrkxjuqa.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fehbvm.com/Article/details/gzqbbsjpu.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fehbvm.com/Article/details/gmxsfurjc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/gqfaprfdk.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.hesvh.cn/Article/details/gjfuvajmr.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/glykeptyx.sHtML

[U06] Py：合并两个字典
来源：http://baike.zdbjq.cn/Article/details/gucjfvxlq.sHtML

{**a, **b}
来源：http://m.share.zdbjq.cn/Article/details/grgksjfea.sHtML

[U07] Py：反转字典键值
来源：http://mobile.hesvh.cn/Article/details/gesfnnwae.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fehbvm.com/Article/details/gduegkyoo.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.hesvh.cn/Article/details/gmmucyjsg.sHtML

[y for x in nested for y in x]
来源：http://baike.zdbjq.cn/Article/details/gsotvlfdw.sHtML


<!-- 参考信息 -->