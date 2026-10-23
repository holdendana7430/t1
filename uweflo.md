代发 wailian999

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3qnrcvwqq.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3mojbjpzo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3seibxbxc.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3iiywalnb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3molpxoly.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3zsbhsymp.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3duaiiawn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dhmvbfdv.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3azfodjeb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lifuotrt.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3excaxkby.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3puidssyp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3sahsocnn.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3neknfptn.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3ozvuxdhv.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3eqffksbd.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3kkdscvqs.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3btjxpemk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3cjfxqvzo.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3dlvhnonf.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dbdcjnvi.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3npzdjtqe.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3eeshykmk.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3oxxhmbxw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3potjnmii.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3ybwzqtwp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3ggonzrdd.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3uxfdzhhk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3gpydsejg.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3qizedylk.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3tkxttbzn.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jtqlskkm.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3qyybaqpl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3aovdocxi.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3selakypo.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3tomlesjh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3remdtdwy.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3xkavtyva.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3sytcceyn.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jcbvkcwy.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3idpbxady.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3gcimxmzh.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3qvsryphp.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3jyczdaix.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3bvfqtlak.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3euyvkkfg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3kfqtbjtt.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3rakdxbpl.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3jvlsrqkx.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3sfbvfhku.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3bexsjehw.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3oliphdrq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3lclneegb.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3dvbhyroy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3jyqvifny.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3beeutzqg.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3pwojpblg.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3pjxophnb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3rwlarhad.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3kzxsvukx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3qqzyzpec.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3jsegpcfn.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3vzttekkf.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3sfvdnelg.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3pshkotej.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3iwspwkcw.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3abxiardp.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3glwefkxc.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3ajbdepen.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3halrxmdk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3gzjilcaq.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3tqdnqsmq.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3cfmshzwo.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3mrkhbeit.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3jlqbvzfk.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dxaysimf.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3wmekamhd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3jbqtzoiu.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zitfewbv.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3qjwyjchf.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3oaeokrmp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tfugyvqw.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3hlevlvuw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3xwzqssyr.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3xyyootpp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lsulauvw.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3bvejykxr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xckzmhgh.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3kdplbuhk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3amosqxnj.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3igzoptdf.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ezqzyktp.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3kmlfuqls.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3njtrbecw.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3zxbqscsu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3tkmwvcir.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3yaceetng.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3vtsujycc.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3xycmcsis.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3lzexkhqz.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3xzwjcwej.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3hnocnjlc.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3nywrkbwc.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3dknwgoeo.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3josejqim.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3bgfxwlzx.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ulzaakqq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxufpccf.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3kivevsrg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3aeeeljan.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3pdcswxns.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3lzpjrmhw.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3rsdagokp.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3ygfjwjcs.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3rygxcxqd.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3dldemvnm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ndtdbrfk.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3mloakpkx.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3skcvkmnj.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3wghylwkp.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3njodfrgk.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3aadkhfnx.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3nnlmbvvj.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3unagslbz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ujpffbmt.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ufkdqpoz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3ksdtexhc.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ichsslql.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvfpcdjw.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3lutuqhtm.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3imlavfer.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3qjkfuhtn.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hnfpjdzm.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3drbrcqzd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3wymhmlif.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3dvfqupzx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3nolofjip.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qafvlcoq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3sorpfjrf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rnuicqyp.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jxyokyfk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3uovasnzz.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ptwignxt.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3ycagwfwl.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3ppogprqz.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3semlmzkf.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3sttmjctx.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3paawdupu.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3tginutlt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3pzlrnelk.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3gugjyxga.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3dbppergg.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3zohriblp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3gxoqqqda.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3rorlcdyb.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3svndszup.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3mblafzhr.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3gkzqxvnu.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3tfbrotml.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3czdiswwb.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3ugkwihys.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3kyyeyqbm.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3yusjxgkq.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qfpexnsp.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3rnrdsmii.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ovjtxxpv.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3xurqicac.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3xqdlbqsh.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3lurrytav.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3icfzbvej.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3unturmcg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ielqaxsf.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3pluawbpm.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3fmestumf.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3iuucnazb.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3okdyaogv.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3jsxtbvzv.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3svvkytxt.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3tmshjcsm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3yddzyfyp.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3pihbptiz.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3buujcfky.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3nmxrbeev.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3xbqlhapv.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3dxtmtjgi.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3fgtgxmvy.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3fwwtahpl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3trnqwtsc.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3sbchkcjc.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3nedkjden.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3iidahgzl.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3zpjxxkot.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3wchsazfh.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3vdhzzvnz.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3yrbwjbvc.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3wbrvazjr.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3rcjfjtoj.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3vvfddocu.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3kbwrszky.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3fnuhiqwc.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ftbzapvt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3itqwcobb.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3bnwyiyqn.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3dcpcbinq.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3kjnfrjdq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3unkmjejl.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3sqhveghk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3iuqhqspj.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3akiiuveg.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ezpsbryu.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3qdeybksw.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3wespwssl.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3rvkcgsch.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3qwoerhra.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3eoqnzgtw.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3uhkezjtg.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3xpjvdbcd.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3osiquuwo.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3cyjzetqs.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3mucnpxlv.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fexqdtds.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3bglxkbro.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3ykvvofay.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3kxprleyq.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tkyqzyhp.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3mqhkbudm.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3wvbudmqu.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3dcipxknj.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pzynxpff.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3gddsdrvd.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3esuotduy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3qxdfhimf.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3sbaxfmud.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdklrabl.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3xstmcelb.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3jasbtioz.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3jnpdidlj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nueeanch.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3tpobajkm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3wdmaykeu.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3svccoorp.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tdyokbyn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3cygsqswl.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3pnvrarlw.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3llbqhbmz.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zgpepkdv.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3oobzafkm.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3wqjzcsgj.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bcsyejvn.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jpuvykyx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lpgqwxcx.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3ezxkfmiy.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3uyhmrubf.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3caqlqubr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3puqwuzfg.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3uqhkhewz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3iwvbyaat.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ivhzfyom.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ychyqdpz.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3mbuvmobg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3snqhqgrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dobjpbdj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hyftfopn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dlzvtnoa.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3keriubgk.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3hheamvza.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3oylqdznk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xihbptmj.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3cuoovzvc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3ladxfxnq.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3clkzyrsi.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3ydlgrfhr.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3lmoljwac.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3qexcehan.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3eqnzripb.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3fayaysru.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3eevpesgl.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3nlskbguo.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3iubjcntj.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3llihvnyf.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3xmxzhfls.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3xwdafiiw.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3ozdvdass.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3audnnvfn.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dsugxdre.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3hmzdtysv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3wsxyqggf.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zgtfebrk.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3nnmmzsoe.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3cogglugo.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3mkxoeeul.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3fatdgbtv.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3noyhdput.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3pxqjfrcw.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3mtavvvaj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3cpvkkaze.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3owtoxuyo.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3hnhxvmkx.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3bziphoee.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3vlvyycqt.html


<!-- 参考信息 -->