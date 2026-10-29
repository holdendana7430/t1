代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/gmnfmufbb.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gxdceriyb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/guixydnkx.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gnxcditzq.sHtML

split -l 1000 big.log part_
来源：http://mobile.fehbvm.com/Article/details/gkmztmjbj.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/guegdswks.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/gwbuqtraf.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/gtokjvhjr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/golrqskdj.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/grlpnpipq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gcwncljtn.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/gvtdgfidg.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/gxmhbgmot.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gqxlzxuna.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/grxnmdgtx.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gvvesmyjz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/gmxwynlib.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gjgqfplkq.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/gpqahbzoz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxhuaioxl.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/gxmdayqik.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfpyjsqxa.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gpmlbebut.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gnvbugczy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gkfqhopzy.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gcguxhilc.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/gtnriskbh.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gkkmzehpq.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/gwymmydew.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gtrkcowod.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/gsgoaxlpw.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/gxnertozq.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/gurtkdalo.sHtML

[S06] C：字符串比较
来源：http://blog.hesvh.cn/Article/details/gmvotoxom.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/gnbbeehmd.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fehbvm.com/Article/details/gyqtlgzie.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/grvheidde.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/gkqlqabjd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/ghrelqcyz.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gauukbutx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/geuwiavbc.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/gtnitcwaz.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/gcxocincm.sHtML

[S11] C：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gfxnctcvq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/gmjwjlwfr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/guqvpinrd.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gbdnokidz.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gkyaggffz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gmhluzbct.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/gwtskwfjt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/grucjsabf.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/gpzwvhnbw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/gpobpqxwf.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/gbzwoogcz.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gwfjzjkjm.sHtML

[S16] C：位操作置位
来源：http://blog.hesvh.cn/Article/details/gpoaoiqvt.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/gzlafthyn.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gjgxdrovx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/gzrovrgvn.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gpzldcdnh.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gcxdfblda.sHtML

[S19] C：快速排序
来源：http://mobile.hesvh.cn/Article/details/gsxhwhszq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gsoxtgfkg.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gokdodhhn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gmdylvosd.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gvqbwgcix.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/gyvrunynt.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gsxjhjbgq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/guazfrazw.sHtML

[S23] C：随机数
来源：http://mobile.fehbvm.com/Article/details/gklnchtrl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/giywkhrbg.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/grcktobcx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/gclnuomds.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/gheknwpib.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/gaxfhiyle.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/gelvhikzg.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/gyicaixbf.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/gvsfnxbxx.sHtML

const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gussbciyc.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/gpwqtwual.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/ggxklvble.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/gtllaqbom.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fehbvm.com/Article/details/gusebsvov.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/gwuewxkeo.sHtML

#ifndef X_H
来源：http://wap.zdbjq.cn/Article/details/guisedhfi.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/gccrijihv.sHtML

#endif
来源：http://mobile.zdbjq.cn/Article/details/gplowjwqt.sHtML

[S31] C++：Hello World
来源：http://baike.hesvh.cn/Article/details/gawznnsto.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/gcqhamsub.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/gpjntmbyn.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gfpgmknkg.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gqfmsnzzf.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/gqzbvapkv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gkqovcvur.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/gbhizvhnw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/gguxbiznh.sHtML

[S35] C++：map
来源：http://www.m.share.zdbjq.cn/Article/details/gdmfiqdkr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gzyladnuz.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/gzowrcdge.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gpnpdvxde.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/gxyniluby.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gkeyazsrg.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/gxdgyaaix.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.hesvh.cn/Article/details/gxamvtbwj.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/glwjekrwp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/ghqwvwqlh.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/gzaetwyib.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.zdbjq.cn/Article/details/gewrdnroc.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gowddmtxj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/gkrjyijdv.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/grogsmzpi.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/gmaunoptj.sHtML

[S43] C++：智能指针
来源：http://mobile.zdbjq.cn/Article/details/gblqejfpk.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/gjafaizgp.sHtML

[S44] C++：引用传参
来源：http://mobile.hesvh.cn/Article/details/gkjjsjerx.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/gfmhflbnr.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/gklytqswf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/gqvqdfbzd.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/grnbtfznj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/greuhobuc.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/gaayxnume.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.hesvh.cn/Article/details/gukmywyso.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gqtxcrosf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/gipqbmemy.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gsgaiisgi.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/gyxbfujsm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gvssuvooh.sHtML

[S50] C++：格式化数字
来源：http://m.share.fehbvm.com/Article/details/ghajwfzpa.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/gxsqdasnf.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/gzeuivguc.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gfpfxwccr.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gwxytvatj.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtcxhdksj.sHtML

[S53] C++：移动语义
来源：http://www.share.hesvh.cn/Article/details/ghsyncksz.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/gmxjjnxub.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/gsacizaes.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fehbvm.com/Article/details/ghhcgnqnn.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/gxbgmlweu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gpvdreojk.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/guxpekwjp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.zdbjq.cn/Article/details/gedhmykap.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/gdwlgaglo.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gymtruyjq.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/gqdqablmi.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gejvxxjqb.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gktzntzhm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/gjxjcgfwx.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/gpxsjspmm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.hesvh.cn/Article/details/gonoiknjl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpvanmopt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gciypmhpe.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghxvfwear.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/gwycitmil.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/glmlacxuj.sHtML

[T02] Kotlin：变量
来源：http://www.share.fehbvm.com/Article/details/gfesfftyv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gfyflitlm.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.hesvh.cn/Article/details/gdfdonemz.sHtML

"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/glaeeqkmn.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/gntjuahql.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gyeqbjryv.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/gfvpdhhkl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/gwpeapydu.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/gtirusfxq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/gizdwjlsv.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gcxjyagvp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/ginwsoqci.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/ggetuauca.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.hesvh.cn/Article/details/gcuxdiwbj.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/gjwzbebmi.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/gipjcljkq.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fehbvm.com/Article/details/ghjfrbyim.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/gavdtjodm.sHtML

[T11] Kotlin：协程
来源：http://3g.fehbvm.com/Article/details/gguuxgjyw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fehbvm.com/Article/details/gpcvfmvii.sHtML

[T12] Kotlin：解构声明
来源：http://wap.zdbjq.cn/Article/details/gckmrgtzk.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gjzpozegi.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/gfcvbslpb.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/gxqwmuwrz.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/goqcluyvt.sHtML

for (i in 1..10) println(i)
来源：http://baike.fehbvm.com/Article/details/gdxzpdrmg.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/gtnynwrfn.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.hesvh.cn/Article/details/gldfwdfmu.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fehbvm.com/Article/details/glftzgchz.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/grbidiiss.sHtML

[T17] Swift：变量与常量
来源：http://blog.zdbjq.cn/Article/details/gksoibswp.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/gdlpxufgz.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fehbvm.com/Article/details/glqhojhom.sHtML

"值: \(b)"
来源：http://blog.fehbvm.com/Article/details/gmcqvkznq.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/gfgixjfeo.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/gudgxsfwt.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/gniobrcjs.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.hesvh.cn/Article/details/gtvhgezlc.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/gkyqaxaxw.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gmuxistlz.sHtML

[T22] Swift：字典
来源：http://www.m.share.fehbvm.com/Article/details/guqvkkmni.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.hesvh.cn/Article/details/gxlxaegaq.sHtML

[T23] Swift：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gnkeojrjg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gsfbxidmj.sHtML

[T24] Swift：闭包
来源：http://read.share.fehbvm.com/Article/details/gkqmwpvle.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gunticnzy.sHtML

[T25] Swift：结构体
来源：http://mobile.zdbjq.cn/Article/details/gkbhuflcf.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/ghnsfpzvb.sHtML

[T26] Swift：类与重写
来源：http://www.share.zdbjq.cn/Article/details/gqhaqorik.sHtML

class A: Base { override func f() {} }
来源：http://3g.hesvh.cn/Article/details/gjjairocw.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/gjjowrwxp.sHtML

do { try f() } catch { print(error) }
来源：http://wap.zdbjq.cn/Article/details/gvxpyszdx.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/gjlclsomy.sHtML

enum Color { case red, green }
来源：http://mobile.hesvh.cn/Article/details/gnivzpsbd.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.hesvh.cn/Article/details/grphdiirc.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/gpjrcqarg.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/grdfubfjh.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/gurzgdnlm.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gxnxeymvi.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gsidxdcor.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/gepbuhmzu.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gwzpongem.sHtML

[T33] Lua：表（数组）
来源：http://baike.zdbjq.cn/Article/details/gqyjwhtbe.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.hesvh.cn/Article/details/gcfkubaro.sHtML

[T34] Lua：遍历表
来源：http://www.share.fehbvm.com/Article/details/gnieielci.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/grinnnnnh.sHtML

[T35] Lua：字典表
来源：http://read.share.zdbjq.cn/Article/details/gcddhipzl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.zdbjq.cn/Article/details/gpukntorg.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/gqsugvbsm.sHtML

function add(a, b) return a + b end
来源：http://wap.fehbvm.com/Article/details/gnabdstmp.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/ggatcdevz.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/geehszyvm.sHtML

[T38] Lua：条件
来源：http://read.share.fehbvm.com/Article/details/gdeenwbhj.sHtML

if x > 0 then print("正") end
来源：http://mobile.fehbvm.com/Article/details/gskzpwrch.sHtML

[T39] Lua：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/gzngsgfbs.sHtML

string.find(s, "%d+")
来源：http://3g.zdbjq.cn/Article/details/gxyqreldz.sHtML

[T40] Lua：元表
来源：http://www.blog.fehbvm.com/Article/details/gvlhiitmg.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/ghrdsnuip.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/ghnpsrjcv.sHtML

print "Hello\n";
来源：http://wap.zdbjq.cn/Article/details/gmrlnvbed.sHtML

[T42] Perl：变量类型
来源：http://baike.hesvh.cn/Article/details/gjwmsnjls.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fehbvm.com/Article/details/gijmhzdzf.sHtML

[T43] Perl：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gdwebzosf.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/gdsdtzrfz.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/goxltjwjn.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/grywfvotp.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fehbvm.com/Article/details/gbbimwxas.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.zdbjq.cn/Article/details/gjxyczeoo.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/gqfwtjdvo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fehbvm.com/Article/details/grztuhswc.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fehbvm.com/Article/details/gscbpwdvi.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/gkiupcxso.sHtML

[T48] Perl：正则替换
来源：http://3g.zdbjq.cn/Article/details/gudgceglq.sHtML

$s =~ s/old/new/g;
来源：http://3g.hesvh.cn/Article/details/gklivbfsa.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/ggbxujpdd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gbjeibihv.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gjwqngyal.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fehbvm.com/Article/details/gbbezpdpm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/gprjbbfdy.sHtML

[T51] Scala：Hello World
来源：http://baike.zdbjq.cn/Article/details/gxnzcqbpb.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gqeemykne.sHtML

[T52] Scala：变量
来源：http://www.blog.zdbjq.cn/Article/details/gkeivykma.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gluhwlckh.sHtML

[T53] Scala：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gcuyiuwaq.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/gxruucnbl.sHtML

[T54] Scala：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gqitwwvuz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.zdbjq.cn/Article/details/gkmndgowv.sHtML

[T55] Scala：集合过滤
来源：http://baike.hesvh.cn/Article/details/gukvnumrj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.zdbjq.cn/Article/details/geisxnndu.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/gjlskstfb.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/goqydpbax.sHtML

[T57] Scala：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/grfkpobqy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.zdbjq.cn/Article/details/gmgdgcsqh.sHtML

[T58] Scala：函数定义
来源：http://3g.fehbvm.com/Article/details/glcdodnkr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/gpetmmofb.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gdgzlaptx.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gmibxvplb.sHtML

[T60] Scala：折叠
来源：http://mobile.fehbvm.com/Article/details/gtblcejjo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fehbvm.com/Article/details/gvuscqzva.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqudydouq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/gegjzjvhj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gonygxdrz.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/gchpnmjcs.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/gtuvspbta.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.zdbjq.cn/Article/details/ghpsbhmcs.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/gdhzbamdj.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.zdbjq.cn/Article/details/gttigpmoq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.zdbjq.cn/Article/details/gwtugrkwt.sHtML

[U04] Py：变量调试打印
来源：http://baike.fehbvm.com/Article/details/gkmlwsbaz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.zdbjq.cn/Article/details/gmuhdbmay.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.hesvh.cn/Article/details/gjxxmgogu.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gpglsdxsn.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fehbvm.com/Article/details/ghwpveyom.sHtML

{**a, **b}
来源：http://wap.hesvh.cn/Article/details/glzchbtlr.sHtML

[U07] Py：反转字典键值
来源：http://baike.fehbvm.com/Article/details/ggakosgxq.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fehbvm.com/Article/details/gymvxevlo.sHtML

[U08] Py：展平二维列表
来源：http://baike.fehbvm.com/Article/details/grdbthqmi.sHtML

[y for x in nested for y in x]
来源：http://read.share.zdbjq.cn/Article/details/gmgqrharb.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/gbicaltwo.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/gqootikvt.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fehbvm.com/Article/details/geehtpcap.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.hesvh.cn/Article/details/gmesmthib.sHtML

[U11] Py：生成器表达式
来源：http://baike.hesvh.cn/Article/details/gqxuicwpr.sHtML

(x * 2 for x in arr)
来源：http://blog.fehbvm.com/Article/details/gihgqvvkh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.zdbjq.cn/Article/details/glzjtteqh.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/gaydyizdx.sHtML


<!-- 参考信息 -->