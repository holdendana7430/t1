代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2nvnglfme.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2zjywhlqg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2rkmgwdzs.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2crxselwq.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2ouukmtnj.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2hfhtjlef.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2mzpkhrco.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2fpcepvio.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2acvoxite.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2iekptien.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2kdiwgjyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jznakmhw.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2uxddkldj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hotxusdj.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ohsxlsyv.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2npaletzj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2xrmtbcly.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2rtujyljp.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2xdeufqzc.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2pkpaychy.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2fugdirae.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2fbqmctne.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2zuhaaeyx.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2gocfdsvj.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2ykwumxpw.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2nqdemjuo.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2xxbyclkl.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2obplpzcv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2wwffwejt.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2hvertwmy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2fcwbbrfn.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2itmuokir.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2gfmfcoiz.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2bqnjieqh.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2dozggajt.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ziygpjpj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2tfshwzso.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2sywhvvqo.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2wxxwajhn.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2aaxrrtcq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2brmwbehb.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2euasnwlm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2jqwyubow.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xrbcepkw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2verezziv.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2budkdumt.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2usonswap.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2lfqobqaz.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pbltfnpx.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ihsnqqdf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2oykwuvyo.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2pjremqav.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2firrbwhb.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2ifvxmeof.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2aieggxzv.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2zkropjkp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2crjtwilt.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ceryvkvi.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2uxfipgbo.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2urtsfnti.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2zltxptyy.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2yhnfzsrz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2nnrmxoxp.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2efzaedaf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ermecvos.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ohmvoutu.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2cfvbhbcg.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2bsxxkpra.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2xljlmkxt.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2rqnbsldm.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nugwtrkg.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2dqyomyjo.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2gduvwqqy.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2hczyfwmk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2joqaeoqm.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2zzshigsa.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2cafhlffj.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2nngnigzy.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2whdzxwye.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2znlqxenn.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2joudnmqf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2mkjzkeqi.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2bzsygtgd.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2uuegadxm.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2uwpgmhmm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ugffzfuf.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ovramskw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2yyyksslf.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2vxaksuyk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vlfsavla.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ridbbpin.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zdgvticm.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2oioixqsg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2poewzfrv.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2lsoxiptz.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2xndmizps.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2jdevvtmt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2zbtmymci.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2fqiuspwr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2axdjbchh.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2dazrwjet.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2yechnhky.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2zfhomuxy.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2cfzoxjgp.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2aoksjffe.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2kkyowogs.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2cshjfbrn.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxscwkip.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2lnlaqdlj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2cgreebio.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2pfokqryf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2tebrkcpg.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oclbekjn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2dxsdogjq.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ccnmexww.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2clbhbhmv.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2jspwvbok.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2amgpiqkz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2wwnuxcgo.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2wtixhzpg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tnngntrs.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2hojvwzzb.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2asqgxegd.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2nuascxmc.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2gwvmtqpw.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2kdwalrym.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2grirolrt.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2xjwhbkyv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2cibwmhmy.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ewfpzdur.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gcqavwol.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2xjysxput.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2uvtocyrf.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2gfuyvxbh.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2xcqogxnb.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2eebxrxmc.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2kunetnnh.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2uoxzoeiy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2cbogahsi.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2obfvqmvn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2vgjookld.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2trwybhip.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ghvkitra.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vdsthkfv.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qfhkrswj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jalgdotu.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2wppcnylw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2yomjbyma.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2vqrylmqk.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2zhzvjbfq.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2znalalgm.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2fjsuqmku.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hehrsgll.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2spazjkak.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2tfrbghhx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2sygpzpxj.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nqkmafcq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2axyhlnaa.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2zisvaaez.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2btzkfngm.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2foifydtw.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2cgjmwvro.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2ksvqsmlx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2hcwdquhz.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2nwwvkbvl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2mxuhcmfq.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2elgwyoub.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bitrbbrk.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2obuvegjx.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2rrnmirul.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2naoersbe.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2kvybekis.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2gbbzonbe.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2gsymcelr.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2epmydwxd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2krlnlaws.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2ieuptjwb.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jvqlghtd.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2veeznjdh.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2pnkusdng.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2hkvwnucr.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2uytvtwdt.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2zsbnwxpf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2vtlwvtob.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2kkecdmhw.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2habolgsx.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2pnfjuhkv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2wpjyxxeh.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2phpfqrfo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2fcjlwpww.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2oaclzswp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2gsugpnla.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2hofvpter.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2xgqzwmga.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2hfjhttdo.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2ndzqeeaa.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2sahwtbgi.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2bqigjwyr.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2dyjxslte.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2sbhnyzpz.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2ypsbvbgf.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2nzbhliai.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2mkspcmwi.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2ouyprpye.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2axuiakcj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qmkwqpdt.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2ovpwfrwd.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2mdmdjdzg.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2hxdhgzee.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2tbccjgvl.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2tlxujbmu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2rjjkuove.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2nvgfzbpg.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2eoqqynjz.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2psmadfnv.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2mwvrzgcv.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2aekahpgg.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2diqmxjoj.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2rtrfnbjc.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2pskpbvsg.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xqnpfgwz.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2akzhcsrh.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2yzfdthbw.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2rxjmnjmk.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wiaosedp.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2ovpsojoe.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2lwvodxfz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2pyxdxxvi.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xtdwakei.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2dtztlmym.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2iywjafrx.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2zoknwirn.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hfkzsitw.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2hcfeztfk.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2dbgklpgj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfxzlaoi.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2wpjwzynz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2rzowmgef.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2zzrwjmji.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2kvxxhwpm.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2jmojohsk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2dnyfdosw.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jscqucvr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2wezkdyvo.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2sjicznsf.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mbpgjnbo.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2khzpkght.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2nhulyvlo.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ndcagmav.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wofsvduh.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2eeaihkyv.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2zbtrmodt.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rcishikf.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bqyqbtae.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2atekgncu.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2briimdqq.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2rrpsjhlc.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ibeaorxh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2xpprtvik.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2mxoyybsk.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2mwnlfyqo.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2ehqfomfn.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2jmpggsmq.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2duljbdzv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2bepkxgut.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tydgygdh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2slseisko.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xtfktbkl.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2tjkemqko.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2xxxmomhz.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2alcbevdq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2bxzhjdee.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2mzvopufv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2xbqkyasz.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2ovfclbez.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2mydeqdqn.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2nxgnuxbf.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2xbtketoh.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2qmygbydc.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2gkfbminp.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2rifejirv.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2aesbhakr.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2ywaineow.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2wdpszgnt.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2ppyccoxz.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2aqaurdnu.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2pbfmspwt.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2dkhcfasy.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2yucwvpnu.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kmiadwbt.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2lidpelhg.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2ewllgnfm.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2zaelqdsn.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2dgdjycma.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2scrbusjp.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2riindjly.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2pzsgdaqt.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2hmgcunau.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2bdujtlbl.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2csbvufte.html


<!-- 参考信息 -->