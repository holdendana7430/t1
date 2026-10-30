代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gnabeqycw.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/gftmfswvb.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/goeortcwm.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gylzcubem.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gckxhtnro.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfpfzwywe.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gmacxxzxz.sHtML

#include <stdio.h>
来源：http://read.share.fehbvm.com/Article/details/gbcccuuir.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/grkqxgzna.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.zdbjq.cn/Article/details/goofbmxlv.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/guixxhult.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/gwvlmplwf.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/gmhozfgcs.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/gdtsauozw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.zdbjq.cn/Article/details/gadmvezja.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gqnzxpynd.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/gtgirxjjd.sHtML

[S06] C：字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gdyhyyiqc.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fehbvm.com/Article/details/gywwztpdg.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fehbvm.com/Article/details/gsbucxpch.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gckcjjrhx.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/gzpsfuipr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/getxxjbxw.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.zdbjq.cn/Article/details/gphbovzoy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/gvcqcdafc.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gnmbjyhia.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gvkwfcleq.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gsugpftug.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/gbzvifqcx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/gravfgctu.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gwkcljeou.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/grstmzmow.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/geyayjmpk.sHtML

[S13] C：宏定义
来源：http://www.blog.zdbjq.cn/Article/details/gehqfonbg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/gpzxuywbh.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/gfzxfbhez.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/gxermeedo.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/gddjnsmcy.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gzxlsckmt.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gbnmylvhh.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/gmsnefknb.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gttuxgrrw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/grgtpjmnv.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gxkhxpdwv.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/gwgztfdrh.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/gmfvntahm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/ghsgktckj.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/gcjpgyngl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gbohebhxr.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gmplxrhby.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/gifffbvmg.sHtML

[S22] C：字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gqlvrodoq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/gbzawkbqi.sHtML

[S23] C：随机数
来源：http://www.share.fehbvm.com/Article/details/goninsbmk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gcckqdafr.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gkxetrrkf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gbwxvoscm.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/gvkorapvz.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gfxihrink.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/gfqdtvqdw.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gclefywrs.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/gmrwhrqlo.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gwcxkghrd.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/gkkjzjshd.sHtML

static int counter = 0;
来源：http://www.share.hesvh.cn/Article/details/gtyfzfzld.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gelphmozv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/ggqeuirwf.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/gpnuvetqy.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/gpgdeeaty.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/goxarvcon.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gjsydrivb.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gnwxqbhmu.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gdlazjdks.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/gbtnfwqch.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/glutubuds.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/gziufcobz.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/gjaisuxkx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gwncyhflo.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/gnowoefil.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/gqmreiutj.sHtML

[S35] C++：map
来源：http://blog.fehbvm.com/Article/details/gyqmclvrb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gablvijwu.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/gqqeyxhte.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gkgneqxga.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/gtvqxqpzu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gewmqsmwu.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/gnximkseq.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/gehctamnk.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/grtlsfzkb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/gowjjwfhv.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/ggmxezflh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/gjzxmxbvk.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gqgjjntmm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gcmwjxzhy.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/gdmmraero.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fehbvm.com/Article/details/giaajsirp.sHtML

[S43] C++：智能指针
来源：http://mobile.zdbjq.cn/Article/details/gsvpzdvcj.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/giufycymu.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/gwyzkpbkf.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.hesvh.cn/Article/details/gutkrexaa.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/gztebbdal.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/ggqvnreka.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/gtzyskydj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/glcmrubnv.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/gsrmmviah.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.hesvh.cn/Article/details/gygbwovjc.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/glnrpxult.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gxszowrcd.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/gqzpwehpj.sHtML

[S49] C++：写文件
来源：http://read.share.zdbjq.cn/Article/details/gdkaglfwf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.zdbjq.cn/Article/details/ghkwpipsq.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/goilcxnkt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gnexenmxi.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/goeftlpoz.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gvgpohzlt.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gqvyppufm.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gvbveajqf.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/gkoenayar.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gzcftyznz.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/giihvhwxy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/ghrjbqwbv.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/gspvenstq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/gimxohgjn.sHtML

[S56] C++：optional
来源：http://m.share.zdbjq.cn/Article/details/gfpbifkgn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gcfvqezri.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/gffaousnq.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/gewrohqrw.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/gjpmlhfsf.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.zdbjq.cn/Article/details/gepliqefv.sHtML

[S59] C++：静态断言
来源：http://read.share.fehbvm.com/Article/details/gyhmmdhhj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fehbvm.com/Article/details/gpqlaijrr.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/glogosshm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/gavjnyrdn.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggvwbvxbi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/grwryeyiw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gsuppjrvc.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fehbvm.com/Article/details/gepowhhwo.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gtehdnihg.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gzgtgtdld.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gzgdgayfj.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/giyvaftjl.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gstsebcjp.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/gljerwxky.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/gijzmoziz.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gylevuuls.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gmzfqtjpb.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/gdiejosvy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gilsmelgo.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.hesvh.cn/Article/details/ghnnvjbdy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/geshzqaor.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/gbtegevvj.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/goxlxmgaz.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/gnmmwjwpz.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.zdbjq.cn/Article/details/gabzziyat.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/goflezjmd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/gjeujfolt.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gmdzaujib.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/gghvkhrbq.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/gfzjvmxkr.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gmkkvelsx.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/gkukmyppb.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/guwgyvfat.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/gidiyebgw.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gchgikrvp.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/gbzuxgbdj.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/gelwpkswh.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/grhzqnwvn.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gpqacaavl.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/gpugczfvh.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gaccircwr.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/grsddpkso.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/glfdlhumd.sHtML

[T19] Swift：可选绑定
来源：http://wap.hesvh.cn/Article/details/ghpxzvgsk.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.hesvh.cn/Article/details/gyhuonzyr.sHtML

[T20] Swift：数组操作
来源：http://mobile.hesvh.cn/Article/details/gmuudfhqz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.hesvh.cn/Article/details/ggeynxeqr.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/goxmxsdxo.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/gxnzpvtqe.sHtML

[T22] Swift：字典
来源：http://baike.fehbvm.com/Article/details/gpblxmata.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.zdbjq.cn/Article/details/gcboumteo.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/gxdiuyjkr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/guspftiwi.sHtML

[T24] Swift：闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gnfurnnfz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gaiddonee.sHtML

[T25] Swift：结构体
来源：http://read.share.zdbjq.cn/Article/details/gxhuatfcn.sHtML

struct P { var x: Int }
来源：http://3g.zdbjq.cn/Article/details/groryzbyx.sHtML

[T26] Swift：类与重写
来源：http://baike.hesvh.cn/Article/details/grtnbavss.sHtML

class A: Base { override func f() {} }
来源：http://baike.fehbvm.com/Article/details/gphhecfom.sHtML

[T27] Swift：错误处理
来源：http://read.share.hesvh.cn/Article/details/gvtafgebw.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fehbvm.com/Article/details/gdseydydw.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/gkxoxinda.sHtML

enum Color { case red, green }
来源：http://mobile.hesvh.cn/Article/details/gwcbfkkli.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fehbvm.com/Article/details/gqkvytgee.sHtML

guard let x = opt else { return }
来源：http://mobile.fehbvm.com/Article/details/gbudnujbh.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gnysslgjx.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.zdbjq.cn/Article/details/gkinitcsn.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/gwibzxsxl.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gmeobkdhr.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/gdhkjmbqs.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/gxivrbzpn.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/gjpdluwyv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.zdbjq.cn/Article/details/gezdqynty.sHtML

[T34] Lua：遍历表
来源：http://www.share.zdbjq.cn/Article/details/gnikazwtc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.hesvh.cn/Article/details/grwunwmmd.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gnrpjouxh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/gahttzfsm.sHtML

[T36] Lua：函数
来源：http://m.share.hesvh.cn/Article/details/gkpeesimm.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/gwmkbvapr.sHtML

[T37] Lua：字符串拼接
来源：http://wap.hesvh.cn/Article/details/gurgqeexb.sHtML

"a" .. "b"
来源：http://www.share.zdbjq.cn/Article/details/gwubvtwpn.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gwmbicwpz.sHtML

if x > 0 then print("正") end
来源：http://mobile.hesvh.cn/Article/details/gwetenbpy.sHtML

[T39] Lua：模式匹配
来源：http://mobile.hesvh.cn/Article/details/guayfxfop.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/gcqdrnwqq.sHtML

[T40] Lua：元表
来源：http://3g.hesvh.cn/Article/details/gvfwaiedd.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.hesvh.cn/Article/details/gdpejxdfl.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gcogwvlep.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/gfnppgrma.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fehbvm.com/Article/details/gdljexrlf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fehbvm.com/Article/details/gibmmqyxx.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/gcaiffhjg.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/gnqoayeuv.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/gfhzpfvin.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.hesvh.cn/Article/details/guejgpsmq.sHtML

[T45] Perl：数组遍历
来源：http://mobile.hesvh.cn/Article/details/geslcjwzw.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/gxulohkbj.sHtML

[T46] Perl：哈希操作
来源：http://baike.zdbjq.cn/Article/details/gaeheztrz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/gnunlxgud.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fehbvm.com/Article/details/gfwdceisc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fehbvm.com/Article/details/gpbvrbxzx.sHtML

[T48] Perl：正则替换
来源：http://m.share.zdbjq.cn/Article/details/gznvkeaqn.sHtML

$s =~ s/old/new/g;
来源：http://blog.fehbvm.com/Article/details/gsgogcixl.sHtML

[T49] Perl：函数
来源：http://wap.hesvh.cn/Article/details/gzhytoqce.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gjjzhprwv.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gdgbxppyl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fehbvm.com/Article/details/gxpzfbvds.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fehbvm.com/Article/details/gucugdwyb.sHtML

[T51] Scala：Hello World
来源：http://blog.fehbvm.com/Article/details/gpnvugvae.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gsawqbzwn.sHtML

[T52] Scala：变量
来源：http://mobile.zdbjq.cn/Article/details/gkkskoxua.sHtML

val a = 1;  var b = 2
来源：http://read.share.zdbjq.cn/Article/details/gnlwzuaeb.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gztniewbw.sHtML

s"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gteyrnmjt.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/giadlybdj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gxkpmgozl.sHtML

[T55] Scala：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gjnegtuvs.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fehbvm.com/Article/details/gmnxzhmvb.sHtML

[T56] Scala：样例类
来源：http://baike.zdbjq.cn/Article/details/gnwkcvngk.sHtML

case class User(name: String, age: Int)
来源：http://read.share.hesvh.cn/Article/details/gjwfmtoes.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gchmzbcbk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gjfujozwx.sHtML

[T58] Scala：函数定义
来源：http://www.blog.zdbjq.cn/Article/details/gvbgeixeo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.zdbjq.cn/Article/details/gqqsxduko.sHtML

[T59] Scala：循环
来源：http://mobile.fehbvm.com/Article/details/gjpkwqfkc.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/ggtbridev.sHtML

[T60] Scala：折叠
来源：http://blog.zdbjq.cn/Article/details/grwzrznmj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.zdbjq.cn/Article/details/gzafjhsld.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbgelgmnd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gukkcnfxo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbflsygge.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/gwkodudoz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/gurtvrwpt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.hesvh.cn/Article/details/gveyocorr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fehbvm.com/Article/details/gykecvkbz.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/gqwpmygye.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.zdbjq.cn/Article/details/gbptcondg.sHtML

[U04] Py：变量调试打印
来源：http://3g.zdbjq.cn/Article/details/gidvuwezq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.hesvh.cn/Article/details/gkmatinoe.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.zdbjq.cn/Article/details/gzpclygwf.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gskunygpq.sHtML

[U06] Py：合并两个字典
来源：http://3g.hesvh.cn/Article/details/gtikbpwck.sHtML

{**a, **b}
来源：http://wap.hesvh.cn/Article/details/gldgkzplv.sHtML

[U07] Py：反转字典键值
来源：http://www.share.zdbjq.cn/Article/details/gjzaexuav.sHtML

{v: k for k, v in d.items()}
来源：http://3g.zdbjq.cn/Article/details/gmnowgppm.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.hesvh.cn/Article/details/gteghvdin.sHtML

[y for x in nested for y in x]
来源：http://www.share.zdbjq.cn/Article/details/gmdwvggka.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fehbvm.com/Article/details/gsakezovh.sHtML

max(d, key=d.get)
来源：http://blog.hesvh.cn/Article/details/gvkamclqc.sHtML

[U10] Py：按值排序字典
来源：http://blog.hesvh.cn/Article/details/gnfxxodji.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.hesvh.cn/Article/details/getykkhtk.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gliygpcya.sHtML

(x * 2 for x in arr)
来源：http://mobile.zdbjq.cn/Article/details/gfxmehlme.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/guxmhvwyv.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gsbznoikf.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fehbvm.com/Article/details/gxilzogcw.sHtML

deque(maxlen=10)
来源：http://baike.fehbvm.com/Article/details/grjxgtoqn.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/gigmhhpqx.sHtML

defaultdict(list)
来源：http://baike.hesvh.cn/Article/details/gpivqyigu.sHtML

[U15] Py：高精度计时
来源：http://wap.fehbvm.com/Article/details/gjgbmpkpr.sHtML

t = time.perf_counter()
来源：http://m.share.fehbvm.com/Article/details/gzqvuwqws.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fehbvm.com/Article/details/gpwvmxitk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/gcarerqjz.sHtML

[U17] Py：初始化日志
来源：http://3g.zdbjq.cn/Article/details/gpgtzofrn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.hesvh.cn/Article/details/gyakqbatk.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.zdbjq.cn/Article/details/gqmtsgpav.sHtML

pat = re.compile(r"\d+")
来源：http://3g.hesvh.cn/Article/details/gxjavzpml.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.zdbjq.cn/Article/details/gpmrystdy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.zdbjq.cn/Article/details/genftgbvq.sHtML

[U20] Py：缓存函数结果
来源：http://baike.hesvh.cn/Article/details/gawmyvhcf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/glgkodawi.sHtML


<!-- 参考信息 -->