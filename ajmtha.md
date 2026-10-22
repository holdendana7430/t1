代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2npvxptdz.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2pivumdiy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2mlkrlozi.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2dvrgasux.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2bykhrghq.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2nvqonhxa.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2jryjmlwi.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2ymzyzuou.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2pmjiflqn.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2qlulrpnm.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2jyyoruhy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bfwhzkdm.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2aiulmhjl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jlxxbzcv.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yatuopil.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2gxwhgcdl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2tmcxsoyv.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2uzniaqzu.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2dmdvvboq.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2bzcdblts.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2skotwxfi.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2hvztznxd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ujpsvbwq.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2pqqirlff.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2sztvzltr.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2twgmkpvi.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2byiossaa.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2obbiqlsu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2hrxifwod.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2vsiowwgn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2lnltowhf.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2dppyjlcu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2imymuicq.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2jialhbgh.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2vupibwni.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ldduskcy.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2lixkfghb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vlfuaexz.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2rebblfez.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2uxllxwrw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2yeifxfab.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2akjzjovi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2pnmljzsz.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2zlfahjwg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2kztonymk.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2ffajoqkt.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2fmswpxom.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2ipdgsuun.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wdjduemk.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ejeqklqm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2qvcizmfa.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2swgnerbm.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2vplcqiwp.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2tvgxpcil.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2nucpkpsv.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2wzbtvqbn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2vuddiyvy.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2kianlykf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2hmsmaviy.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ebottpzz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2ddewzltu.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2kafvkmgt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2gvvkewdj.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2rajfqgvd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2xuxpayal.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2fwtxidfm.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2hvahtlfl.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2biglacpa.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2wipyjzgw.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2xitkssnk.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gfgbkpgc.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2gvrnnpnu.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2ghesaqqn.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2gtyqgukz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2ynbkfxwk.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2czgpvdqf.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2oohqsqsr.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2dpjsmpqp.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2sxiofkuc.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ryzlbzbw.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2niqandxb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2thclyyjk.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pkmknsor.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2wsyfzgpu.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2gjxdkcoi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2webpwrds.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2dexclxxi.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2bfklvdbi.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2zziuwwib.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ufljlmwi.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ztrsqknw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xbmrinys.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2aghfrkxh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2ppikopph.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2sotgztcy.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2weqcuwds.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2pmzbqbei.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2topehhyu.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2mufyuvow.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vgwidazh.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2njpxaptx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2gjfqfyci.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2xgluhkfx.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2jhpfgabl.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2wgbnedyp.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2gpthxyzz.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2svsbytxz.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2eajcnwig.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2sxcrtwpu.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2nphyvwsi.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2dghtkbxw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2telbzktv.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2fcsutfks.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2enwsnvup.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2eutyjfzf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2hndegged.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2skgrorih.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2jierylcj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2epkngcxb.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2vjqymaug.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fjzzyebi.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2iwmsifkg.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2ukgnbzbg.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2dtsjsfph.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjczboyj.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2gpiztxbx.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2crybqlzi.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2vrczegxt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2yeiujjpo.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2xhogzbdg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2tsktltaq.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2zasisxiw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2glgnumfa.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2itgityaq.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ypobkxkk.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2qrhoelbg.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2arnegpdy.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2rvxnedbu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2dnzqqnmm.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2tvvnzcrx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2osjklerm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hvttpkfz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2leukdjim.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vwpwoyfr.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vovnrzsi.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2poetyllo.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2pueitsdz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2ldnsrdsq.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2sidoiyap.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2lkecibfr.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2qutomtyk.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2wudobuuz.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2akpyjwrn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2eivqtvtt.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2uhnacpfm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gppxxlew.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2lijbwuax.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2iohlwtia.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ovfmcrea.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ygiyekrz.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2ngbdxils.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ojonxrgl.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2hylhfcmt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ugpxsrtg.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2qxumzpgs.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2zpnujdkj.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2evesutth.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mthjhqsv.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2xlqxleki.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2btismwdc.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2lhbwlfqq.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ddjgorpt.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2xgsczexn.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2rykgiioy.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zlpjffrc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2djrqsxuu.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2fmfygarc.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2urtahkln.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vqqjmskq.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2bxqaaoar.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2nvetxxqi.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2vhvxhhnr.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2ugoqbpzo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2mwcuuvoe.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jhgppaop.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2vxfzobyx.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2rpmusjuj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2okmdmxfb.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2wusqwypl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2gdxmeppb.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2vrljmpgr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2cfoqxgsx.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2mmrufduy.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2xeocnnmm.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2nbmmducf.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2kgqjlxax.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2fkznfuek.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2rkfzzasv.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2ywsanxoq.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2pmonrwyx.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2ezjxjnlo.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2jrmvyxcb.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2zovogocv.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2msjoqgog.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xktpzpvo.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vbcoxwpq.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2awnncjyc.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2nqiicwry.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2zviorqiy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2sqhphtlh.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2atomaoyz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2snwiwryw.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2emciqdhk.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2cmwbbxok.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2umtemspb.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2lnyxnovq.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2vtjoehwo.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2cvwgbbtn.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2fycbiomk.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2rogefjoj.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2yqzseuhn.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2yrqszdky.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2wjziwpbd.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2ivyingpq.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lffzjten.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2cuaepykw.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2zryjqbox.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2bltdbbmq.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2iymhsexd.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2rszzhgdw.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2fwduyumm.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ehoqpgyv.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2xuzmpdrs.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2ncehwkqn.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2aetrwtbo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2pafzdefj.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2jrofzlbm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2oovffdgs.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2lfmdnaho.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2objacxls.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2mqaazvbm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xgohmgrw.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tnnlsllg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2qxkhdvef.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2kflesufz.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yfcqujcl.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2imzdpoiw.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2kylstfou.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2yugsfimm.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qkqqjrzf.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2jalxwfvj.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2hwpabdmo.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2azscvzhw.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2jrwxpxsy.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2izwrlceo.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2sdcvbmse.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2knzlhbho.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2euepqjom.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2hrnxgobv.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2fmxapmpr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2mqnqtzts.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2fjmupthm.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2kuoplame.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2lgchocte.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2djbpscyr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dxgfyijj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nrmcyyps.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xtiyswgc.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2soebogqe.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2dnjzorzh.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2cugerlbc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2poodekbu.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2fmtrrxok.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2rgzxwnnd.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2zzhfscgb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2wlwmvdqf.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2yooelipa.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2zmkiigzs.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2oxzwmztd.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2tkajqihl.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2inevloda.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2tsvixacl.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2dhemgrft.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2wmjboohy.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2qwgvyirb.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2iltcsmov.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2xvagykua.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2ezdxcsuc.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2whcmhdvn.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2cvcthtro.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2zbaczzmc.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2qzpvyavl.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2wtdcgdwp.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2euyzshui.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2gsrporqc.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2kghsqdoo.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2gnqupked.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2gnrcceuh.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2etzvaqil.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2oivnkyel.html


<!-- 参考信息 -->