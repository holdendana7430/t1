代发 wailian999

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3trhtosbf.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3thpkmkzf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3kznljrlj.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3acfnioke.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3aiykqjri.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3qrpnyfhe.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3lczpiqem.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3szohxdkt.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3vquoqtxu.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3yjtxrmnr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3kwfhjfix.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3xlvjpbne.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3hyrildfg.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3gdjevirm.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3pchvybyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dravtoot.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3xmoqdzlc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sjlhotje.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wgemgkbu.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3yithdlkf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3flkrxzpx.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ysooihnx.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3lbvvtehg.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3uanbympz.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3qrgitimh.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3mbhtwyjs.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3gtynmsyc.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3vhcqmabr.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vwrlrjkp.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3hxpcbaav.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ipvmsmzx.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3lygxldln.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3puokjxhu.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3djspmbxj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3stybloap.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3wlvwgxte.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3daoaniyy.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3tivgbxvg.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3aulgzqaz.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xpmoeewr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3crwjonsi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3mhlqgran.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3kdkfmbue.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ggwhpkyb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3eeyusdwq.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3prvwdybk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3tamegxcx.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dyileuuy.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3wzfrnuku.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3jocoypzk.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3yxjjfzqk.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3xpebaisl.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3aiurqgpp.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jrbapzwa.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3kouwffig.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3awwstakq.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3lybgkqpm.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3hibrnpwn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3reaiyxut.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3snidplua.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ffkjsoin.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3vryvekuf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3dyqjiarq.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3vnxrbzmm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3kdxhgecy.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3vezsdwai.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3wwocuffq.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3sxazaszi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3ozdndvyt.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3stpdyqtb.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3gysdqzba.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3vioqosyt.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3xwpqxwxn.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ikukwvwd.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xrnzwuks.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3phgforau.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3irxiztcb.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3blqtpwhx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3oeauvkwo.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3ufuatpjz.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3taxrgndr.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3lyepubcm.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3avlacukf.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hqqklqqh.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3fxomznpi.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3bpiitiqx.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3pskwmhsd.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3lanvdznf.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3hmdnesvd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hngyjxcl.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3nphgsrtv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3rnzrfdjn.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3xgrblijn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3pvbnrgkl.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3kysodmnj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3trnttnyg.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3fdoragzw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3strkfqia.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3vrodlnpm.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3haggfwag.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3qcmxcwff.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3umchfcqa.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3nqutnkzc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yjzakrxp.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3jgccknvw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3yhyjddbx.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3pssprhzd.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3domsxewc.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3bjtdicow.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3plljyzjr.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3sellnqac.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ydruldsr.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3nygwdiwr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3xibdzgrp.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3qyvxbkjj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wunuytkf.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3bgvhjaia.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3psrhygnf.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qaiircdr.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3kdowuqnq.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ryssdblp.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3jfpaxgjx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3mteypouf.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3zxrptsud.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ejaszxif.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3ynxnjuxa.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ahrwpzgo.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3mbziiusn.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3owmmrruc.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3inqyfvmd.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3ahatkeex.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3optyfchd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3tmdinprt.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3rgnggqsx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3zmbiydzg.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3sjcbrquf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbuecihm.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3fdpywjhm.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wrmsprph.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3whaqzsox.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qzaaomqo.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3tdsdurrf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3vbfgztvm.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3rsomiwqc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3rxiyxuro.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kfvurtbx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3efhxtrfy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zfqvfcew.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ghtarkwe.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ywthhgrr.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3tdcauoyt.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3zhgqtwyx.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3ppqiyeoh.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3byfqavox.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3axwaqoxm.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3lqzlzqql.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3gitcubbd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3udjkfbeu.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3wnizkwjn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3awolmgzu.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3jeoemctz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3hpqlvubs.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3fkrptong.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3wfkdzeav.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3hnedfdrz.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3jnckixvm.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3zdeihejn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3xueeoefu.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3uhtzkvyq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3newaxtcb.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3oqtqgsct.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kxsccjoz.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3nmhxkobd.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3udfoibin.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3sduvwyqq.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3rjbugzdt.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3kftqbbbr.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3mxeuoabn.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jwrlbbow.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3axwpswpo.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3hrpbbzei.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ubmquxnt.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vcbpbfzr.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3rvedreer.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3lahdmbjk.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3jvnkmnuf.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3xvgxxepf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3liesmnhv.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lkeamuqt.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3hqrrbfku.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3jimrjtar.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3hrjhrpbp.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3qrgbcoac.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3lowwwtin.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3pupkbnqn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zzjefvoh.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3yamwoftb.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3etpceepa.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3twhsvsee.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3vuedvmfd.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3nbkeqpbf.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3bzktokeb.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3sagvivyx.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3ozitrhaj.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3wlhhpfdg.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3gbftvqkh.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ikuscipr.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3mfyxnrke.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3caymyykg.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3whkemlby.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3dcncaaqo.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3vabvuqdf.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3rlhendfz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3udsywrtc.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3kvsadmod.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3gwfsuzmr.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3vuqiaoff.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3btywijyf.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ftgxcyqw.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3sdrsnaya.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3dhxnkbvh.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3nicusgif.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3wuobdbge.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3dzqtkkft.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ojcuzmeo.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3qlkqmpiq.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3kpldxunj.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3gjfehofh.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3oluemcnv.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3tnoffqse.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3rqfycfdv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3gmzkanij.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3wnyknaym.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3soiyvahn.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3cpbzwyeq.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3phkgynci.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3cenglqtq.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3bbvotuma.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3uwtalnnf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjsopekt.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3cwtasvrj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3mcobxsmv.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3lxdaaxfv.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3jutvejlo.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ycdxzmnb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dfewctkc.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ebtgyern.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3vowwwkxn.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3lrgmvkwn.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uuiovqri.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3gixvxqwt.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3xytssige.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zhpctgsr.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kbnhuetf.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3eeqahiis.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3twqakjlw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3psbyejpq.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3mmepazor.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3zjesanzd.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3ngnmuobj.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3xrvqlwen.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3rshowjrx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3qofnasdt.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3oxiepnwh.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3yvhuyzit.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3pfjynerz.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3xghiquxq.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3vdywsutw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3emdarrjd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3whbouhpw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3xeiifnem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wposlgec.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3njerwadi.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3aqjblzcm.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3vpgzuknf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3xgifbzar.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3xgmvdylr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3yeqnbajo.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3dzjqumui.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3iyzulnkj.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3hmgxwpjo.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fyolyjik.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3iojpewwh.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3qgbdghci.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3sabjepxn.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3coywfstu.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3qslhkteg.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3aihpghwx.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3zurtxkkc.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3aqxzgvfg.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3uarbwqbb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3hvmjxupu.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3gjmluaxk.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bwfckamj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3huyhqwjy.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3fekjkbop.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3zoanayoa.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3vtsuvsob.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3ldhuwske.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3hwmxzccv.html


<!-- 参考信息 -->