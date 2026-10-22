代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2kcravaac.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2papywoew.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2rkudoynv.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2fupcxcid.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2cpcngcee.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2gkxtfuqm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2ikpiqgmv.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2hyetrazo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2qozhtgoh.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2hrodryro.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2khtcdpml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pbtqnnpy.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2fzwxwxbe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qhvfmwcu.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xfhxeyna.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2rjnibihi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ueiktkdh.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ekwnbbvk.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2zvkowyiy.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2ufclirrz.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2cqusbdhf.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2suczijsz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2trvqujad.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2szmulhzs.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2gjsdxxpb.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2hyfiwwuz.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2byeoaozi.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2ifguypje.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2osdvuydy.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2zwcrpuhz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2usgbosux.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2kshpnevz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2sgxjtzos.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2slbcpolz.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2kgrsnkpr.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2pfezqsxz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2bdsjsetn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2gzrqdzhx.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2zuhqfydi.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2bnvuborw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2zlazqpkh.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2agcpeaep.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2euftaljz.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2yxwptirs.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2zvuezsio.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2tepseeju.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2bbzeqfpk.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2zetdsmqq.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2pplnfedd.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vxydtyjl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2vxjljekq.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2pbpupvnl.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2ldkcicbm.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2grpgzkbu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2dulxxrfy.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2bnatmmie.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2qcjlneih.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2kkgpnokp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2gevtjywm.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2uvusddfg.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2kvrvddbh.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2qkbwhtyr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2avftlrvk.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2bdueolcm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2douleucf.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2btnwkbur.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2kmekuxvq.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2oicnfsxv.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2fubldyaq.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2nctijzdr.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pxmibxgu.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2curupnxl.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2lpwwsrkm.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2qsbmlwqb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2kaytrxyi.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2qwvnumhj.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2gzgmwjyk.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2xxhkzvyj.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2lfxrdrpm.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hqlkkkxd.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2bjrtytka.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cozzmtka.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kioqiskk.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2hrdfosvf.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2tepsiyex.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2roncdemj.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2fwgfowle.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2ufigxmzx.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2mkhehdyk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vogwjwqc.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2yvbnfgbs.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bdkqzlld.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2jlvsfuyg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2pemcnybw.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2gbzgakue.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2hcemzhto.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2hibrhnwt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2xwpkqlpz.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2fekphndn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2utvqtmpt.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2arkydtxg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2lgielvnl.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2kssuppdz.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2meusboiw.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2psfbgpfk.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2foxjiouv.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ydkncire.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbbqmttu.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2yzpxfeyo.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2zxrmotmv.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2vmoipwik.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ravtldiu.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tanujhva.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2myzxahyk.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ztglmife.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2ghjwuxwg.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2sfgvnujb.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2ngamexqp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2rvpzkwvl.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2rqcwysut.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2sucjgvjx.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2vrgmapwg.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2xjxdsyvt.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2cboegkpv.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufzmaksz.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2mkrhipxi.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2bhysajyi.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2fjmtylac.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2zrotsubt.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2udbggotp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jcrmkqnr.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2irycpdpz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2alekauow.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2jmzagjjj.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2owjuxbal.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2rwwwsqja.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2aylzklyj.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2wizawtkn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2tqwzvfuf.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2nfblgvmr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2eydktqeg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ydjlxsam.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2lxghfuix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ldmjdhmj.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vpwhasaj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zbwphegw.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2nbfuurzs.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2xwpuixae.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2abreqees.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2kymdztea.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2cembbbzc.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2vwjknika.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2zimrqhjq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2yvtuaevo.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2qchrgzuj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ybtrmxmr.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2divyfhws.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2yqenbnet.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2vtxapgmy.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ezrbnukn.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2prjgarhv.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2snooizpk.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2ptqxlngk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2atkcfzps.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2buegymiz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2giqbsdbg.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2aeqzxntl.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mkcxpmde.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2ndaznipf.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uptitclm.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2mmyirpia.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2mvnscqsi.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2xkbyammx.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2mhrovphh.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2sghekfmg.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2unwrllck.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2obsjwhsx.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2qileegvm.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2pequvbty.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2iwrcqhdf.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2qcprjkoe.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2jnxaseah.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2cmmelfub.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2dozetukz.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ifhzstrh.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2fyjgqypo.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2zfhigqwh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2mtxrjvkl.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2vhwbdchn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2zsourjrr.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2usxxtcuk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2jtiqeoxk.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2jnbayute.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2wilgmkxk.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2dtwukgxg.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2cowofkdv.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2niexvako.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2hrgnrkoy.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vnyjkztt.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2vobeijhg.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2fjhfpggu.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2ttlnlbra.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2lutshrns.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2mzypeifn.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2oltkosen.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2sxjmfeed.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2civgeugz.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2yjaiunig.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2uyykktzr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2avwzqpso.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2myzlnvwc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2auhonjjj.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2uvhbdniq.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2mccmpkmf.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2sowtvuhk.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2beomxiyn.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2bhysjuvt.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2kcigdcrn.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2dprfdfov.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2pqfnrfqp.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2dmuipmqu.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2aqlojenc.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2ukljqsjq.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2idzaydzb.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2skppkodt.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2hwpyufxe.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2npcxepnv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2aobmzeoe.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2uihbuxzi.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2yxntzxyd.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2eeqmaorf.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpbdkdkm.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2njoduuly.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2ikdwbynn.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2gimnwrga.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2esslrprp.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2julmyjod.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2ypksetop.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2imambeak.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2kvqhcjqe.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2oiunlqty.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bkqzlhbm.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ijzdawtk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2kildfsqb.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssuigopp.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kcmucpic.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ohzsmptm.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2mbqtrnak.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2yzaufugc.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2helzyxpo.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2espuazar.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2rzmajgak.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gzlzpxre.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kzrrqgyi.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2uqukvqhe.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2ibjajikz.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2rtvteslh.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2cxmfxpxv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ucgqqgqa.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2gvkbwvao.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2aehzfisr.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2zrpynkfe.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2whswoqxn.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2cdhfpxuw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2qplwgkrv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pwvefaot.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2uexpmmkj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2awguyauv.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2wekkqope.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2jdhriuge.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2cdgzsgjb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2zsgiooky.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2funwphla.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2jwyeysls.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2esettljk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2ixbiwtjk.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2afnfzgiq.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2mlhybjrq.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2dlvyrsyc.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2xjrhfxvs.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2kzeallqu.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2fheyjryc.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2kbgwwlsc.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2amgbdmpp.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2zeyycpxx.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2jydxfjid.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2yjnvkcjq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2mnzwaqrh.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2ctessymj.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ivgphhjv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2lbnlqbqs.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2duvizcxt.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2woqlswwq.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2satibsff.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2ybfyibyy.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2wuffelwl.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2vhcjjfmh.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2hsvtagvq.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2ssbqhssc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2ylphcnmu.html


<!-- 参考信息 -->