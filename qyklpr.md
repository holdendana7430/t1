代发 wailian999

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2lxglqdcs.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2mcmmxdrj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2icuwoznb.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2zyhycugm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2rasaamfm.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2jojimhhc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2iqojxevg.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2makdqmzz.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2dtflmyqb.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2pfusbojk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2hkfonbjj.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2xsbcayww.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2tqxtmfpk.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2icyrrels.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2zkzvqhra.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2goqcfhfy.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2fxguzomk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dlblqswg.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fqgmsxcu.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2jaymauxw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmwdpvzi.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2mceexgda.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2qdzuwixw.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2yibkxlup.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2ukioqhtc.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2itatlqvz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2jybxnsud.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2junczvqo.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vggtupqs.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2wnrneoeq.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2twtwmbal.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2zsllynoz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2xgkvhajg.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2umxgmemr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2myxeotas.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2thntzwyp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2otufgnlv.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2zmcjbdll.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2rkwnvbsk.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gpantkib.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2fflgxmfy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2xafeuptm.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ojnwwkoa.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2egdpwaqo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ruophpsh.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2ffxykysj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2lqbmbsva.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2egdtlkpo.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2cectjnqa.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2yzjftehn.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2orvcumnq.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2dfatgkdr.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pspmnbqy.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2jpvdfnly.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2pclzvgth.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2jglqxhgf.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ymxpqbho.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2ddwjhmse.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rvhuyllx.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2fsugwvms.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2dmybwdhl.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2wukvgffy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2fpqpbjbf.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2lhzfmkhg.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2bgnpjrwp.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2qjjbhygv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2snnhdlsk.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2pzttwawn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2lhmnoycg.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2mvffqhqw.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2ipwkcdzv.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2dyggkoax.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2qcyudzri.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2ahkljqqc.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2stxoegln.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2wcokwsyo.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2arhgrsbi.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2rcnsmkzd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2kwqgmdoc.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2ozeosbpo.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2vehetwdj.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2itbuxpqr.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2tdoxphbv.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2drnxtxar.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2krhixxkd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkyxixrp.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2tyvxutpk.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2cdmhsyfw.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2mgftgkmq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ntpgdsdy.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2trhxndhf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwrbewxe.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2zecivbua.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2svwtkmzg.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2veicdsbt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wrpghlbr.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2tohljpil.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2pwyzkqul.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2fckaqybl.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2imqpihvp.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2kbrfggsx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2pcajdsja.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2ultqmaef.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2jmqqqupl.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2dwahdiyg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2kehjfaxv.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2mfesuejm.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2fcyfqxug.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2tdatlwuq.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2hrutmuda.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ehgotfbk.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2avnalpsp.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2pygpfwuz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2gmwalxib.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2hsreergo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2axvazemx.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tesumnwi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihkadqis.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wazhczqq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2wiawvauv.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2tdxcgzrg.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2cemtvtem.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ezedgtxo.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2uaqkyhwh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ilztxofv.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ilfodydw.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2vfzaopxo.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2vrhbdhhl.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2yxtkguir.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2tjpthuih.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2veinfogg.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2qpblfizw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2qvfoaoxb.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2wdrsorlj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2gheqnrov.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2yhaeaode.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzymcasl.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2warovzni.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2hvatapvq.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2hkcyyieb.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2uxmawknt.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2coiddkyh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2dydzvswd.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2xdcrciqg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2hcwuoulw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fqwgynbq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2hzpwxpav.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kaflcnze.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lkexdnyg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2euvkxzdb.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2uhcbtfjn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2ioykcsfu.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2qtltfpbf.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2kkvhbhtu.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2thzpfkqz.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2ocidwfxf.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2cyrboito.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2vzabvmpj.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2yznagmql.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dyixdqzu.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2jkuxfevt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2ktfhztfv.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2pavsekmy.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2weafgrkw.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2qmwlwnsf.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2serxjfkj.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2vqnflhso.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2kfxqqxto.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2jjeqngkr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2eafdjyvi.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2xyyyfjsy.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nxpymrml.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2bzfaqqxh.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wmxwyqeb.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2hevnyrkz.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2yuioahre.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2kvmciddt.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2wayzpsia.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pzdpevty.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2kuzvmdua.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2zbmynwyx.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2qosfkqin.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2tdrmgufh.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2ezwxbfag.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2tynqklzn.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2lshwnlab.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2tcpmcajt.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2zirxelgu.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2bjohoghk.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2jkohptfz.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2npepgfwi.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2hszsvvqu.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2dkfignae.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2ryqtqcob.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2bfnmwxcj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2spombedv.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2qdopwiuf.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2isuozggl.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2dodnflkk.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2dvhuemsv.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2sqciwoow.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2miivilwh.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2yxdxvnhz.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2sfbpcbbo.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2nhwjkygt.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2jxsswqly.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2qczqkclm.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2qivozklp.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hmskchkw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jfupsavp.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2cklldrqh.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2dylhprnd.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2xvlwsjly.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2bakcjdxs.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2ylbriydm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2vrcyqsjv.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2zarclbdq.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2xmkovkjp.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2nyasmnze.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2zmaiwdoe.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2nytqquuy.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2byqfdtej.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2sxatpgel.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2uqhqlmjs.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dqlluapv.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2jjkaqdcy.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2wygqylju.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2jtstffmy.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ndauodyp.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2lnhrpyct.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2knwxdpiq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2dayjltph.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ujqjuqzu.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2orxbcfaj.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2jtjmvpad.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bodcalag.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vowrmrfg.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2qvmhlftd.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2mshkvvkb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fyqwynql.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2ibuvfvnx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2lzrvgarb.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2zzzpazuo.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2nnxcuzqt.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2yvlctzeh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2rszmtntc.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2cxetakqx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2dnkzrrrk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2nmarqfzg.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wawkycbv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hsqpdbai.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2jpepynhe.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2wsuywdxl.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vvjsjxdp.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2skjhbgum.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2wzvysjct.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zgblvqjp.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2nsjcxgtg.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lfccsxpy.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2cnedmrfw.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2jhojagke.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2htoryffs.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2xxowpfvx.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2qdwmdueo.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2mluopcwd.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2fdrdtvww.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2poqosefm.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2mkrfnddh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2sxwgfsfd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kvacahti.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2hvcsvmbk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eixjxkzs.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2tzikehxs.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2aejwkvjx.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2hpzqxrii.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jjirojhz.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2fngvcbgg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2orwbrwin.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2itghdatm.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2ovtnmsdv.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2orrwmyqw.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ouovbzjj.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2uggrjjhh.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2zfkvecdm.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2hcjxfmqy.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2tgdcfobo.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2ucpyoxbm.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2edgiecmr.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2vsetzijk.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2kdlbzwkr.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2sdftfyjp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2gwptvsoo.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2llfjdqto.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pdcktbgh.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2gyugzvnr.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2vixcmghw.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2dziuknft.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2kkyvnnxs.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2aautejlr.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2pvbhlqfy.html


<!-- 参考信息 -->