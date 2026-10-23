代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3nrkbrgsm.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3unlhzwqu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3geufgqrm.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3purdeivg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ulisqatz.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3ylxciymo.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3wvhmpgyx.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qkoryjto.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3jjssxrma.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3rptwntwi.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3qnwipvql.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3gkgxjour.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ttvayrci.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3dicoygtr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3byidjtbu.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xjaimiwj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3lzxrguuo.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3dcgstdis.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3hmfrfwjt.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3vnoedhlk.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fbnqlkjx.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3luhfimtp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3wknbngvd.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3rigqfusq.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3kfydnvwm.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3knwomxfr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3tjligfja.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3hfhhyqku.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3yurdojrw.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3tehbzqpa.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3zvukanfj.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3bskyldzg.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3tnhjdysj.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3mihjlzol.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3hjfcyphb.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3gxzkinqc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3bavvchpe.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3bvgsihht.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3rkzjqsdo.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3xohvzsee.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3iidhdqad.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3vqxjqzib.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3oodcghvy.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3lqwxoquk.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3beaipehu.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3bktmusiw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3jlbpyyer.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ffeclewd.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3obcmktfb.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3saqjndug.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3sieluybk.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3frfzasvc.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3xdyizdxv.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cvgpgiyx.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3ovwkromw.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3ftgovfdg.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3kardbzek.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mrszrauk.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3hetppegi.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3borrwasa.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3xgojfgig.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3obycwuzn.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3glgcjhss.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3sstqvjfq.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3fhikxfwl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cmxwaldl.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3agwpoknj.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3jqxpeusn.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3hxsxisiw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3tskwnddx.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3tcxfiezg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fdbwmpei.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3dnhxbvuh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3fbrmyqdw.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3bmzhbqbz.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3zlleozxa.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3dgjntpxk.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3evixtehx.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3djjupdad.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3jngevcxd.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3kgfoxflz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3rxyptkoc.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3oneyncwb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3drbofhik.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ailstgyn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3wolehgvo.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kmzxoqpo.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3lfmghbwk.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3tuanwqfz.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3yqroyuea.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3rgdhkemk.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3gwtlzgac.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zepjztcv.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3peylwxoz.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3beorcevk.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3opjigmlt.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwfkrveg.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3fwkqqeno.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3mbsyidzp.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3hmaduazo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3naauwswo.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3pcmyhwmm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jkxzlgly.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3hfmcbpwu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3jkxgptph.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3abszdacj.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3vvaijsbn.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3gsdzaoob.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3amcwixjc.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3swtgfjpw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3yihnapyq.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3vzvmiojp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3nudhgrfm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3momzkoso.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3gsgqzulp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tqlincen.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fbkecdbu.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wbksivua.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3pwceoquq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3drundqng.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3juduuone.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ntikdeyu.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3apyxrgzw.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3mbeyfssc.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3oyevvjqd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3anvjccor.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3kovaprfl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vzssbkxz.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3gqtyuviv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3saawjgrf.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3auwodqxn.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ngyhhmoy.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3hgsfkars.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3mgjwyagf.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3prxpukgu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3dqnbsotx.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3urfvpwwr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3shmyknqu.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3jxdmzups.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3alulahdd.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3cxxiggaq.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dopmucpo.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3opqfhqxo.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3qfziorhe.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3kpzwcvdb.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3qelhobxl.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tusnkghx.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3stsxgxbi.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3xdyjyplp.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3jpsegiqn.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ywejnbkv.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3gobwwdho.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3sysnnqvl.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3jhndvcde.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3oepstfkk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3lotthtjn.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3wtgkgwet.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3wwqxicvr.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3yrthakmv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3eynbqiau.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3nagvopck.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3qcysefep.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3suoiwwku.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hvaznxfv.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3kfadttdh.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3sayvfpbr.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3byuycvix.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3gjhmlyfc.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3simqemhc.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3sbenyidb.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3captbibj.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3loczvsbr.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3yhwkxypf.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3himtngni.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3tpcxlamn.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3rvhccdnp.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3krrealsk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zjuzeqpq.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3yrbefadm.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3xzhtyikg.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3mlcskcqh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3lbdtdwez.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3smlqjnpe.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3milpsjja.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3zllvqoyv.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3boarmtak.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ejgbbudb.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3qqznaocm.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3rtmktdao.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3kmownahq.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3zfzlpzoa.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3cdxmrejr.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xubeevgt.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3gmxnifgx.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3wbffmjgo.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3pduxwedx.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3begiixch.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3logmhmwd.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3grvlhekx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3cramvzax.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gqkemrvq.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3ptkqlkwx.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3oukaaxrd.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3twvnimmd.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dkmkjhoj.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fsrisout.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3ogxutpfh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yhdqzurh.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3hpjegghk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3evzheftk.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3edvkdmnq.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3qdibvera.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ivqjpuqt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3pxesdpqb.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xltucwep.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3tyqgrvqx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvsycuey.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hufwmuwu.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kenztqbo.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3gowhfdzq.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3kzlqtivw.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3seqgpkcu.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3miizcbyg.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3qfzqwggd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3trfsyysv.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3jrobkqax.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3rgloyhar.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3zdbgtsby.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3jlgdwsjx.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3aqgkbqkn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3zlgtnape.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3afsjjvbg.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3azqoiljm.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3utyplsdw.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ufnjiztx.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3hoxbcwdw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3gcpufeak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ogezzqhi.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3yagkohul.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jcwlesea.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3ybricout.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3kaziqjxc.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3ezgbnrzk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3rfdnrbgf.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3uzqcmwpx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3osjmiywa.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3vnltvkhn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3wntaqxfv.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3sjpbiged.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3rsichlqx.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3xcqhgzsn.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3qzskrchy.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3giijhbos.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3rmnhmaxt.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3eutjhvgi.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3vrniomqp.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3puwddcjm.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3qhokedkc.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3esbecowj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3hlostmub.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3zvpebfym.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jblhoafk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3nwqlthbo.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xcofacnm.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3etcbjiqh.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3qrbesszb.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3pdwmrers.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3kodjcbij.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3gmzdfnkg.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3aukdwolz.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3kxgmdojo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3ydfwqnpv.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3njispugx.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3ltuszhcz.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3cphwhggh.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3wxvodcyq.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3exvijfvr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3ujbeietp.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3gsyhfjux.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3hbcoiejv.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3mrbshfsj.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3mgydbblc.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3mghxjljs.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3svgxmavl.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3vjqjxpws.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3jrfvvqbg.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3wolwnmtv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3srfilubh.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3rhlrryax.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3gksbvuzs.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3jqivdkxj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3zfoijcls.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3pysdbykw.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3jaqzeqpu.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3aqsazgtc.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3urclhpah.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3zydexkdn.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3sswzbxly.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3nknhrlab.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hyedfjqn.html


<!-- 参考信息 -->