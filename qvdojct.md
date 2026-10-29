代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/ghnsxfzpa.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/gbfpzocmo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gtdmrqjxb.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gdcrqquhq.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/gztafgrre.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gmzlkkgfy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/gnnmuxqkk.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/gfnhvvszj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gzvrmxexp.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/gcfoaovbb.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/gxpkaaybx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjaqebiyu.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/gvvxclcqo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqkrjxgua.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gqvibkfeu.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/ggvrqqsbm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fehbvm.com/Article/details/gdygsurex.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/gvcknttsw.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/gyffxgcds.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gvaxlayfj.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/gcqimxnan.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/gmqqqgqcn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/gwxansvzf.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/glaushzbs.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gnxnpbsre.sHtML

[S06] C：字符串比较
来源：http://www.share.zdbjq.cn/Article/details/grjljsxbs.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/gahiknpap.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/gylfgphec.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/gagkyvdjj.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/gpjdkxwza.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/gbgmazgem.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gkisiumvh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/gsbtjfcxy.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/gzqugyxxr.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gjyfksnks.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gfffilkco.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/gyxqchari.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.zdbjq.cn/Article/details/gvzidejyi.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/giactcwel.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/gyhvevpdo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gtkddbpsy.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gmefpasru.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/gumdynxrw.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gjynpansv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/gbzhvmbdk.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/gxclnyuzd.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gbzmfzbwe.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gbbjkyjbt.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/gjarmqapk.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gsufccttp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/ggwtvqhhz.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gmrwyqcvg.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/gbjnaknpk.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gespgbnht.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gcqbxwyml.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gsednliov.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/ghqqhsnfw.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gmluymwcq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.hesvh.cn/Article/details/ghmsojwjb.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gvddmnkse.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/gfqzavsyx.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gkiydkomi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gjkxbkcwd.sHtML

[S24] C：获取本地时间
来源：http://www.blog.hesvh.cn/Article/details/gsfqgzfzy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/gfknojwew.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/gcnucftot.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/gksypaprs.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/gjhmjmaqz.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/gioibajhi.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gnliwscgc.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gduobxibw.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/gdkougmqp.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/gikvyijyz.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/gthvmehaj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/gipnxaomh.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/gbllnfawu.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/gxuhtigqw.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gbakvoktn.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/gmxhwkzvp.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gzayvdllq.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/gdfucrdlh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/gfgqynblc.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gvgvhgjpy.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.hesvh.cn/Article/details/gdnfbusqq.sHtML

[S33] C++：vector 增删
来源：http://baike.fehbvm.com/Article/details/glmaijcwn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fehbvm.com/Article/details/gyazlbeow.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.zdbjq.cn/Article/details/gxwcxornh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gzfemetmu.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/gjtdtrhok.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/giwxroruy.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/ggmhgiucg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/ggtuniwbi.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/gpqnqaloz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/gwrgyflcs.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/gaewjizoi.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fehbvm.com/Article/details/ggwxltqye.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.hesvh.cn/Article/details/gifnjbgqw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/gefgrdkbb.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gytlnroie.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.hesvh.cn/Article/details/gwauxzasy.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gmzwyethm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gjljyajwb.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/grnkknoni.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/ginolpwje.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gwzmfzyts.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gpqtoaifu.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/gqmpgapht.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/gvpdctsmh.sHtML

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/gzoficpzu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/glmgxjgvr.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/grpjbbwaq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/gzkfpujmb.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/gncfvvlwx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/gbiiwwjji.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gsovktptk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fehbvm.com/Article/details/gfwzlyzjr.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/ggvpvxzfu.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/gnzqecsjq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gszehobtz.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/gmeusktfb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fehbvm.com/Article/details/giypbfwxd.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gwhsvrhoa.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gcjaedcdk.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/gfnaaxcxr.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/geodxtiot.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/gsqfyzshn.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fehbvm.com/Article/details/grnbuutqo.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/gnrcilwbh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/gwozbugva.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/gicpylqtq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/gghgzjcwp.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gqvumrntx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/gpfhzeoff.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/gvxjdktis.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/glmpiimxg.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/gijmdyezz.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/gsnjoddid.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/gvwuuswmx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gmoahaotz.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/gekrfjyty.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/gnkmkddfq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvrzduwvj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gxvaxwpry.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxjbjoytg.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/ggpojpttt.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gjwvgsnlb.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gyapxksqk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/gldjsviak.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/gbbcozgrl.sHtML

"值: $b"
来源：http://3g.hesvh.cn/Article/details/gmvuagjkp.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/gbmrghpfq.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/ghhxhxiaz.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/gzissmrhu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/ghaqpsekh.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gcdcbovqp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/gfmwlrmju.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/grnviuhdv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/gvzpbypzy.sHtML

[T08] Kotlin：数据类
来源：http://baike.fehbvm.com/Article/details/gybkcpuhc.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/ghoevkdpf.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.hesvh.cn/Article/details/grvlkhkkp.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fehbvm.com/Article/details/gkjijsbbq.sHtML

[T10] Kotlin：默认参数
来源：http://blog.hesvh.cn/Article/details/glsaembhw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/golruqcmq.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/geqdiolmi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.hesvh.cn/Article/details/gikjyaglr.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/gqjvicjrl.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gtoxptrvc.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/gcsdjzynt.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/gedevdluh.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/ggrzycacj.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gcslwqati.sHtML

[T15] Kotlin：接口
来源：http://m.share.fehbvm.com/Article/details/gcafuldlp.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/guwxkphor.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/gncvpivpw.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gswweoknn.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/gcnxkljlb.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/gyqsmepkb.sHtML

[T18] Swift：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gkutgswdr.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/gsmgtpxdd.sHtML

[T19] Swift：可选绑定
来源：http://3g.fehbvm.com/Article/details/gozqrxtbt.sHtML

if let n = opt { print(n) }
来源：http://3g.hesvh.cn/Article/details/gbzbezyzh.sHtML

[T20] Swift：数组操作
来源：http://mobile.hesvh.cn/Article/details/guhxyhbmy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/guabwhtwz.sHtML

[T21] Swift：遍历
来源：http://m.share.zdbjq.cn/Article/details/gtrkdwret.sHtML

for x in a { print(x) }
来源：http://mobile.zdbjq.cn/Article/details/gfvjodrjw.sHtML

[T22] Swift：字典
来源：http://read.share.zdbjq.cn/Article/details/glcnznkab.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fehbvm.com/Article/details/gowqsundx.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/gjysxhhen.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.hesvh.cn/Article/details/gndpfjzjd.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/gfhqltfka.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gszmowohj.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/gsejauosn.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/guhvtnwza.sHtML

[T26] Swift：类与重写
来源：http://3g.hesvh.cn/Article/details/gbnojkkqt.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.hesvh.cn/Article/details/gwrncfviv.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/ghzxdvzqm.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/gzffnhvgh.sHtML

[T28] Swift：枚举
来源：http://baike.fehbvm.com/Article/details/gsemtbvvj.sHtML

enum Color { case red, green }
来源：http://www.m.share.hesvh.cn/Article/details/gmpcrlxrq.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fehbvm.com/Article/details/gbvcbcgxj.sHtML

guard let x = opt else { return }
来源：http://mobile.fehbvm.com/Article/details/gbjjppkhw.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/gexjoyyru.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.hesvh.cn/Article/details/gbyshczun.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/gwzrtesuh.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gvstfvdun.sHtML

[T32] Lua：局部变量
来源：http://www.blog.hesvh.cn/Article/details/gxaqayhti.sHtML

local a = 1
来源：http://3g.fehbvm.com/Article/details/gizibajpj.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/gdizmacsf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fehbvm.com/Article/details/ghzdypvak.sHtML

[T34] Lua：遍历表
来源：http://wap.fehbvm.com/Article/details/gqqcbuqjq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fehbvm.com/Article/details/gepkbntay.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/gblfkzfsm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.zdbjq.cn/Article/details/gnzqfeqvu.sHtML

[T36] Lua：函数
来源：http://baike.fehbvm.com/Article/details/guvvsszao.sHtML

function add(a, b) return a + b end
来源：http://mobile.hesvh.cn/Article/details/ggcrmfdhz.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gubsqnatf.sHtML

"a" .. "b"
来源：http://www.share.hesvh.cn/Article/details/gaymvizit.sHtML

[T38] Lua：条件
来源：http://baike.hesvh.cn/Article/details/gkrtdhgyq.sHtML

if x > 0 then print("正") end
来源：http://blog.fehbvm.com/Article/details/gegwiotli.sHtML

[T39] Lua：模式匹配
来源：http://blog.fehbvm.com/Article/details/gxtzyulnw.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/glnlzabtm.sHtML

[T40] Lua：元表
来源：http://3g.fehbvm.com/Article/details/gbhtfnuwb.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fehbvm.com/Article/details/gcjnnlahi.sHtML

[T41] Perl：Hello World
来源：http://mobile.hesvh.cn/Article/details/gzhlpdjko.sHtML

print "Hello\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gfviedlap.sHtML

[T42] Perl：变量类型
来源：http://read.share.zdbjq.cn/Article/details/gtjomvedy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.hesvh.cn/Article/details/gswilsung.sHtML

[T43] Perl：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gbzgfiezo.sHtML

"值: $a"
来源：http://read.share.fehbvm.com/Article/details/giuofhsak.sHtML

[T44] Perl：条件
来源：http://baike.hesvh.cn/Article/details/gvkoptosj.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.zdbjq.cn/Article/details/gwrchtigy.sHtML

[T45] Perl：数组遍历
来源：http://www.share.hesvh.cn/Article/details/geuvcqyeg.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.hesvh.cn/Article/details/grrrnptqb.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.hesvh.cn/Article/details/gywmimlzz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/gehrkwlei.sHtML

[T47] Perl：正则捕获
来源：http://read.share.hesvh.cn/Article/details/glejddqxh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.hesvh.cn/Article/details/gdzzsmfsk.sHtML

[T48] Perl：正则替换
来源：http://baike.fehbvm.com/Article/details/gvkrfxvcc.sHtML

$s =~ s/old/new/g;
来源：http://3g.fehbvm.com/Article/details/gdzjpoedt.sHtML

[T49] Perl：函数
来源：http://m.share.zdbjq.cn/Article/details/gqhtdbjaw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gmyxlhbkd.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/ghrqhafqd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.hesvh.cn/Article/details/gwgvrgzfy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fehbvm.com/Article/details/gepyymiqy.sHtML

[T51] Scala：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gdfdkgvbd.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gavjjzsmr.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/gnpywllal.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/gnuqxejvx.sHtML

[T53] Scala：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gymdkmitj.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gnrgziucx.sHtML

[T54] Scala：集合映射
来源：http://baike.fehbvm.com/Article/details/gtjduzkdh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.hesvh.cn/Article/details/glpjonnma.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gpwwipneh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.zdbjq.cn/Article/details/goeydwfgx.sHtML

[T56] Scala：样例类
来源：http://wap.zdbjq.cn/Article/details/gdmvsbwnl.sHtML

case class User(name: String, age: Int)
来源：http://3g.zdbjq.cn/Article/details/gjkhtohdc.sHtML

[T57] Scala：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gtlehavbu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gjschxrps.sHtML

[T58] Scala：函数定义
来源：http://baike.hesvh.cn/Article/details/gttwtaezw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.hesvh.cn/Article/details/guizpphwh.sHtML

[T59] Scala：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gsgxpbvuu.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fehbvm.com/Article/details/grlpimcpq.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fehbvm.com/Article/details/gvsmtykxz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.zdbjq.cn/Article/details/gqqtggnep.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggzupncpa.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/gjoabzslh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcuilgbnp.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.hesvh.cn/Article/details/gdtlclpki.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.zdbjq.cn/Article/details/gztlqkhoc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fehbvm.com/Article/details/ghtqfvluz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fehbvm.com/Article/details/gpsqttqdk.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.hesvh.cn/Article/details/gmuvwltey.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.zdbjq.cn/Article/details/gsplkdcsk.sHtML

[U04] Py：变量调试打印
来源：http://wap.fehbvm.com/Article/details/gxsqnidbs.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.hesvh.cn/Article/details/ggfdxyegu.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.hesvh.cn/Article/details/gfuqhquql.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gujxrirrr.sHtML

[U06] Py：合并两个字典
来源：http://baike.zdbjq.cn/Article/details/gbubgrshg.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/gfttihtgt.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/gkcxfyjfe.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fehbvm.com/Article/details/gdnlvowmn.sHtML

[U08] Py：展平二维列表
来源：http://www.share.hesvh.cn/Article/details/gurifgnal.sHtML

[y for x in nested for y in x]
来源：http://wap.hesvh.cn/Article/details/ghthrvacw.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.zdbjq.cn/Article/details/gcpkyivkp.sHtML

max(d, key=d.get)
来源：http://www.share.hesvh.cn/Article/details/gciiuewkh.sHtML

[U10] Py：按值排序字典
来源：http://3g.hesvh.cn/Article/details/gzyhxpneu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fehbvm.com/Article/details/gzgxkbtka.sHtML

[U11] Py：生成器表达式
来源：http://3g.zdbjq.cn/Article/details/gnwxowjsv.sHtML

(x * 2 for x in arr)
来源：http://baike.hesvh.cn/Article/details/gnqodayvq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fehbvm.com/Article/details/gdizsafyv.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.hesvh.cn/Article/details/gcvflpkut.sHtML

[U13] Py：固定长度队列
来源：http://blog.fehbvm.com/Article/details/gmnbmkokg.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/gequkabvm.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fehbvm.com/Article/details/gvxhcnqhe.sHtML

defaultdict(list)
来源：http://www.blog.zdbjq.cn/Article/details/gqpnqhpjo.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/gmqhuhfko.sHtML

t = time.perf_counter()
来源：http://www.share.zdbjq.cn/Article/details/gjdrzlkmb.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fehbvm.com/Article/details/gvavmbxwi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/gsdtawihm.sHtML


<!-- 参考信息 -->