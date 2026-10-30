代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/ggzmkruev.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gscygyszy.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/gngqlnkqt.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/gdehnntfm.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/gvjqadcds.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/gbvvmasgg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/gmdxxmrfu.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/gyyrmjmwz.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/ghgsxtqnm.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fehbvm.com/Article/details/gwwbhbchi.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gonnyanyu.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/guzmepxxm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fehbvm.com/Article/details/gsbsorldp.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gpfwvjytk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gtkpequek.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gqwhwpkxb.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gwdxqqfrh.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/gsmrfexks.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/gyrthmxen.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/gokcxbnvk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/gowgbcuwc.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/gdxbsvmbm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gxhjajfko.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/gwvmrlxcy.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/gkpbhtdpx.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gemrfhjkh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gwkzdbhck.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/gtuftfsrz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fehbvm.com/Article/details/gfrsaztpo.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gjdpfbhcl.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/gorqdlafr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gajilqxup.sHtML

S. C / C++ 专题
来源：http://read.share.hesvh.cn/Article/details/gfeczykpt.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxealuqwe.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gcaqynzeg.sHtML

#include <stdio.h>
来源：http://mobile.hesvh.cn/Article/details/gfrkfhonc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gdclnxkyr.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gjrapscoy.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fehbvm.com/Article/details/gelikzmqa.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/ggpqjppzv.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/ggmnnekut.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/gsxtttwom.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/glymjdlqs.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/gwbonbbnu.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/gvuabalex.sHtML

[S06] C：字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gijlwjcut.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/gpargvnze.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/grytzmacd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/gsnpkippq.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gxbzyaeaq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/ghnkfsauk.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.zdbjq.cn/Article/details/glecnmivi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.hesvh.cn/Article/details/gemqrsduv.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.zdbjq.cn/Article/details/gmhdscvcn.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/gtqkfyiqq.sHtML

[S11] C：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gomvavzqv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/gzpzvspdg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gxxctesnn.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gcozealga.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/gtdtbvwif.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gtrdtypni.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/gnuujgspy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/gxkbvctfu.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gqoacykha.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fehbvm.com/Article/details/grgzwgxqs.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/gajjdxfit.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/gvlbayrqc.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/gdoorvhce.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/glvevhaxb.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/gbfkipktf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gvymlbmhj.sHtML

[S18] C：命令行参数
来源：http://blog.zdbjq.cn/Article/details/gdhbzmxli.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/gywehxtmz.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/gdtvztnjp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gcbsyqhww.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/gcsiapzak.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gncvqaplq.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/gskfrnuzd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.hesvh.cn/Article/details/gggzdygpl.sHtML

[S22] C：字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gueugeyxc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/gymmuzdew.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/guvvtfuat.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/gxydkllmi.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/gybdcwehe.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/ggffuoedw.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/gukhgayqt.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/gnhatrjnh.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/gjzzqnjkx.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gbixthlst.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gidxajiqt.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gudatwfet.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/gvcchlltm.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/gjcjwxzxo.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/gvoqokpta.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/guputnxfd.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gpzzvnmsr.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/geqnwrcvt.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/grciqdywv.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/gcyqvebwp.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gqlytnwas.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/goekbwqsz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.zdbjq.cn/Article/details/gobgiwhcy.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/gwtvrbsix.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/gmdvkbode.sHtML

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/gzzzgfkix.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gyvlyfdhs.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/gormgdevh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/gjalvqvcy.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gvlzcrrmt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gjvcucrmx.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/gvhaazngj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/giiznmxjn.sHtML

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/glzpbnzew.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.hesvh.cn/Article/details/gcrzjrygs.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/gylrejyky.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/gnevxvpxz.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.hesvh.cn/Article/details/gczgmhfxx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/gqdrajrxc.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fehbvm.com/Article/details/gwslxguzr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/gctakyzfl.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/gkgzoagxl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/grtmcoimc.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/gaqeypudb.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/gjtaxumwl.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/gloubdqip.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fehbvm.com/Article/details/gdoomvjes.sHtML

[S44] C++：引用传参
来源：http://www.blog.hesvh.cn/Article/details/giiocnqeh.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gxtdyolwi.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gwhobkaqu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/gapjlxxuy.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/ghliyisqr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/gtxktbifb.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/gooqtbalj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.hesvh.cn/Article/details/gbacibffs.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gxdqugwab.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gexkgnvcu.sHtML

while (std::getline(in, line)) { }
来源：http://baike.hesvh.cn/Article/details/gzvdjxrgr.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/gbzqxhmyr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fehbvm.com/Article/details/ggyzuxadl.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/gosjjnmmf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gwllalfkg.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/gcmbqxgtl.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/giqtsozmg.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/gitgiziqt.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/gotcoupvv.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/gykjuomgi.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gkkzbqsrp.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gfvjdfpkd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/ggfedrvhn.sHtML

[S55] C++：结构化绑定
来源：http://3g.hesvh.cn/Article/details/gxexumyig.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/gbekhidrn.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/gbheeskob.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gwznviwyy.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/gihtjtflc.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/gddbjwjvu.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/gixflqzlo.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/gykjtecog.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/gngjtcwpo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gkzvyqxvi.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/ggeeyyiby.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gxutpkgoj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbqbpzwfq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/goqlbqsnw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/glfvryieb.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/glzsachml.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gscjalsvf.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/gfwnnorad.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/gyucqsmmm.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fehbvm.com/Article/details/gzudkfrdr.sHtML

"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gsnmjnwli.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gqkndumtn.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/grspmvzba.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/gjwuztjsc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/gnxyvnbtw.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/godmrxvvc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/ggalovovt.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/gohcomihz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.zdbjq.cn/Article/details/ggppcwrna.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/gejbuqvlt.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/gxmxikljc.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/gakcwhfvw.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/gheyiqbil.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/gprgvwywk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/gokkzbwbp.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gwtkgfhdy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fehbvm.com/Article/details/gclubideb.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/gafonzjim.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gcqslejgg.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fehbvm.com/Article/details/guputipzi.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/grbodbpwo.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/gruoxkhmw.sHtML

for (i in 1..10) println(i)
来源：http://www.share.hesvh.cn/Article/details/grcchdjnu.sHtML

[T15] Kotlin：接口
来源：http://m.share.hesvh.cn/Article/details/gqblfzyyh.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/gmuiezvat.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/ghouavcww.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gbymswuwy.sHtML

[T17] Swift：变量与常量
来源：http://read.share.zdbjq.cn/Article/details/gyagzgabf.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gfvxpdfwo.sHtML

[T18] Swift：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gkspncuiv.sHtML

"值: \(b)"
来源：http://wap.fehbvm.com/Article/details/gznqahtep.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/gcwqnsmhz.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/gzfryyimh.sHtML

[T20] Swift：数组操作
来源：http://www.blog.hesvh.cn/Article/details/gurdvdiqw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.zdbjq.cn/Article/details/gbfauyoii.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/gxoewfxvo.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/gwehvocaq.sHtML

[T22] Swift：字典
来源：http://baike.hesvh.cn/Article/details/gqreawjib.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gjwlkaqbo.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/gtelzpomf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.zdbjq.cn/Article/details/ggmptfzsh.sHtML

[T24] Swift：闭包
来源：http://www.m.share.zdbjq.cn/Article/details/getuaaufx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.hesvh.cn/Article/details/gitzwfwvm.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/gtrpklzet.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/gnskmytbm.sHtML

[T26] Swift：类与重写
来源：http://read.share.zdbjq.cn/Article/details/ghgplijeu.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/genvnyygs.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gmrpmzwyn.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.hesvh.cn/Article/details/giheijzef.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/gjrcetakj.sHtML

enum Color { case red, green }
来源：http://www.share.fehbvm.com/Article/details/gwvnswftx.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.hesvh.cn/Article/details/gxjpgtrgj.sHtML

guard let x = opt else { return }
来源：http://www.blog.fehbvm.com/Article/details/ggjtwxnpx.sHtML

[T30] Swift：协议
来源：http://www.share.fehbvm.com/Article/details/giwoizadh.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/gwzhnoztq.sHtML

[T31] Lua：Hello World
来源：http://www.share.fehbvm.com/Article/details/gujupgjxi.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gjnjfftyf.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/gmvdccbcs.sHtML

local a = 1
来源：http://blog.zdbjq.cn/Article/details/grsbkdpmb.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.hesvh.cn/Article/details/gbqjtadwn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.hesvh.cn/Article/details/gewdznyak.sHtML

[T34] Lua：遍历表
来源：http://m.share.zdbjq.cn/Article/details/gxyskwrqr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.zdbjq.cn/Article/details/gxecmnaqd.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/gaqbagwsv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.zdbjq.cn/Article/details/gobcpmhbs.sHtML

[T36] Lua：函数
来源：http://www.blog.fehbvm.com/Article/details/gwbzxopwf.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/gtojdgtkg.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fehbvm.com/Article/details/gpgyetrmw.sHtML

"a" .. "b"
来源：http://mobile.fehbvm.com/Article/details/gittdxeqw.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/gmxgjeprb.sHtML

if x > 0 then print("正") end
来源：http://blog.fehbvm.com/Article/details/gndrbumgc.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gdbiutide.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/gklnssfxh.sHtML

[T40] Lua：元表
来源：http://m.share.fehbvm.com/Article/details/ghmdbfxku.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/gdweoozii.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gnthzcjes.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/guvpdpcso.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/gddeqbfzv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fehbvm.com/Article/details/gdzfqceet.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gnbjxrjqr.sHtML

"值: $a"
来源：http://baike.fehbvm.com/Article/details/gomuufknq.sHtML

[T44] Perl：条件
来源：http://mobile.zdbjq.cn/Article/details/gercczvyq.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/gpymovgjc.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fehbvm.com/Article/details/gbstdwztz.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.hesvh.cn/Article/details/gjqfccpey.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/gypwdovkm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.zdbjq.cn/Article/details/ghoseohis.sHtML

[T47] Perl：正则捕获
来源：http://baike.hesvh.cn/Article/details/gpexvxvux.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.zdbjq.cn/Article/details/gcmxjdfbv.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fehbvm.com/Article/details/giqgxdhkp.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fehbvm.com/Article/details/gtlbjvwys.sHtML

[T49] Perl：函数
来源：http://mobile.hesvh.cn/Article/details/gayzckhgm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gndpssbly.sHtML

[T50] Perl：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/ggemxpwau.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fehbvm.com/Article/details/goqrbhjzv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fehbvm.com/Article/details/gwzxvehjm.sHtML

[T51] Scala：Hello World
来源：http://baike.fehbvm.com/Article/details/gkcluoidd.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gizzfdkwi.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/gcxpppmda.sHtML

val a = 1;  var b = 2
来源：http://www.share.hesvh.cn/Article/details/gqvvqlbsi.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/gwjacrpel.sHtML

s"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gecruhpzr.sHtML

[T54] Scala：集合映射
来源：http://mobile.hesvh.cn/Article/details/gpphsegwv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fehbvm.com/Article/details/gybrbudoq.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gextrakzy.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gugpescij.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/ggblxqspg.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/goihwuxoj.sHtML

[T57] Scala：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gfphzeuzi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/geteekgjv.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fehbvm.com/Article/details/gratslufz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.hesvh.cn/Article/details/ghviutzgi.sHtML

[T59] Scala：循环
来源：http://3g.hesvh.cn/Article/details/grpirypka.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gpkmxnmyu.sHtML

[T60] Scala：折叠
来源：http://m.share.fehbvm.com/Article/details/gnspkppqu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fehbvm.com/Article/details/gupbbeuxe.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwqdzipqv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gvhggiygq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbbvtjnra.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.hesvh.cn/Article/details/gsefhwzny.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.zdbjq.cn/Article/details/gmerbrbir.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/gmpokpwlo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.hesvh.cn/Article/details/gjyvvanom.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/gblgxoeah.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.hesvh.cn/Article/details/gxjtnqthd.sHtML

[U04] Py：变量调试打印
来源：http://www.share.zdbjq.cn/Article/details/gcsimqlpn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/ghsgruttr.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/ggfguzshi.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gsxzgeuoz.sHtML

[U06] Py：合并两个字典
来源：http://mobile.zdbjq.cn/Article/details/ggfjwwnne.sHtML

{**a, **b}
来源：http://mobile.hesvh.cn/Article/details/gnhdbbvuv.sHtML


<!-- 参考信息 -->