代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2zojuwebi.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2hviqnwnn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2lgivqwtf.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2jjifyvjp.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2cptwzhjy.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2pcgpyhpb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2ofjfhxpm.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ckvrytna.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2kvlvycgt.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2vmfgybby.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2vklrposw.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2kjnhdpxr.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2rkjtptpx.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2rbzyhjzl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2fbaadiiy.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2myzysuwr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2fftckapv.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2sgqtzida.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2nwzxsbgb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uprxrfxy.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2zqergspr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zbyriton.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2whyhxhlm.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2magxycrs.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2vbrvrghw.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2xodfreek.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2bvwantkr.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2qcfevbam.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2qhstdmyy.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2diukekxl.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2iwwkjgkj.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2henbaovm.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2wrcsbllh.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2cikqctir.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2dveqyjzo.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2xqwlwhnr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2cpdlfbyi.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2xktfejqk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2vwojdvdy.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2zulpoxia.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2rcspdasv.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2wfvjbvdh.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2uyavaoyn.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2stanztvu.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2gppthibn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2gdtwbufo.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2emewjvof.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2kavmmgfp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2mcxguvto.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2azbsslax.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2fubagyxb.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2csyxxksp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2wyopqvdm.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2mfuxjjzo.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2fdlxxvtq.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2xrdvvuwo.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2xcxyojdg.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mnifbrdm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2asmvpzcl.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2zkkswlcb.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2yrprdren.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2vtrwqgqb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2uqcnpjkl.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2uvpnwkjz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2kmqzgbfp.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2tesnygyg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2hpjttyts.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2iskgzsto.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2vgfhibfz.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2plwupprd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2ugnoegyd.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2liladcbx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2rnntyrmf.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2gswtiuks.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2wdpldrcg.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2vccrwlrd.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2byssyszb.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2qfynacjv.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dqksrdpf.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2mrlpiybt.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2ewwshlwx.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2tyjxtbbz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2lndpevfj.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2kzpkbznq.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2ngtfsows.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2octaozjl.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2etvfgdyl.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2swragxnw.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2jbhngvfi.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2wksefjii.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aztwghas.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2msdhhnfe.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2jgimshyi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ztoqpzmd.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2tqthcqqf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjjuvaqm.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2seiiadni.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2njpeevii.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2hibqzdyr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nibljgnx.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2prgcmodl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qclvyaan.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2axygcipy.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2zfuyzoex.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2emnarbzh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2jravqryn.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2qyehuiaw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fifzlyex.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2qxtggqhj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2pvkewype.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2pzknqzfb.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2kdpluvpr.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2xsxdeajs.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ouifxsiz.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2pqvercti.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2jsusjqrv.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ayhjxlxi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2xcptbsai.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2wjxtozxm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2yxmfcsid.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2cndewsxc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2sipivjoq.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2djgohhfd.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2rlkhocod.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2nzreowsi.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2afuudqie.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2jlrvhkoo.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2ukmglgsm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lhysamaw.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2zaiptusi.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2aujmgokj.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2aeysuplg.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2sgzuwrmt.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2wokyqldn.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2keumwwpo.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2cjwpwqaq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2hbovjcyw.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ibxrghzt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2jbzukxax.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2kfkuswcs.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2wncyrxtm.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2phqhaklc.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2distwqzr.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2spbbfizp.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2upyapxkf.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2kjiollvt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2htazaqrg.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2rkngrtnl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ricrwdwb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2efbsswdc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ssttuptc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xvzwzjum.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bftmujco.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dbaimkpf.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2dzjvfeks.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2chjgzrtq.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2hjqinemd.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2jwixtefv.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2euxaeaac.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2fpgawlgn.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2zkibedhk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2bufpxkhz.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2jxjrgkxj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cghqttur.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2koynzica.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2lpkopkme.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2yyvtanjo.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ytqmbahh.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2eankcbbr.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2uapyhqeu.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2xktbougr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2vjtomnft.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2pytrtggl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2kkrqfjnf.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2gybwmkve.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2miygtrru.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2tmqubopa.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2niuhymda.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2tomjdfqs.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ztvyqtlv.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2zxloxnlu.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2cihcqtix.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kjitchts.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2nygcnabd.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2bgglyvxg.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2dfawyfvb.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zoajiodb.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2odwdzidi.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2twqrfptd.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2nxwuipaw.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2xjefhohe.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2qscjlpfl.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tcwcwikb.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2mkriljnn.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2baooivpu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2hnxkasvo.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ofoayqoo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2txyutmjl.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2vxjojapr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rftvinfs.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2lmfjoqnm.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2susrqqcj.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2gfrgkwvd.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2rzmygghs.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2sdsigusi.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2cuyqjifn.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2tkbpcoio.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2jcwzmpzo.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ferztuuy.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2lllzmuoa.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2lrpikvyc.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2mcmqjvbg.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tbnrbwfv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mdmxjypi.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2sfrddhmv.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ozwbzkno.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2trfecqad.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2jxdifqqj.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2pkmuftje.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2kzhcqood.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2gnyifbyz.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2fqdcejuu.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2frtrsbxx.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2cfdlxqbh.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2nrwyaxrl.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2jdhuufzi.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2fyqhmdfj.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2cbudnssh.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2irazowlc.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2ehblopqq.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2umkadqzo.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2tciusuac.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xyovjdne.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2almeqoyg.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2jyraejpx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2jxngbpct.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ngnzbkch.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2yrvlozwq.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2rhyszubo.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnsifeow.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2oaptnfwm.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2sxybvenf.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2hgkpmnvx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2dxjzhjfa.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2vwcycqqa.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2hgqhgohx.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2nmmopehl.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2inwlxgmk.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2glajlzmm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eibloykd.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xyzurdgl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2kixvppkk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2hccjrxsl.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zjmggqbv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2pvixvtax.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2klrqwxsf.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2yywaiprd.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mplisidd.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ekpaairn.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2hsseycta.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tlswwxal.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ilgfrgur.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2lqatrkgz.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2xoqorkie.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2txwtmpqf.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2byshtfvk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2tqpdktas.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2truzofub.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2byimhopb.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ibedujcf.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2qpqvzium.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2krudsgxk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2autejftg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ajmkqwmj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2vribmiod.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cddgkzet.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2otxedtuq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2wrbipuke.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2xnnihnuk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wytntacm.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2irxjidhm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2mmpwbhmb.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2nfefvtkn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ettfloym.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2hxectatw.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qvotcbom.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2awppanab.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2wpqqqrgl.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2ciegeebn.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2xqobaoue.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2dfzgdxzl.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2qkyibbtq.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2hmrzanvq.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2owyrrkrc.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2adjmmzxq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2bneofeul.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ymckrwaj.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wdfshiuj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2ebtmdehp.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wfnsclag.html


<!-- 参考信息 -->