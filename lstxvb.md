代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3faqfggzv.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3ctdzyxgl.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3epxiltzj.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3adycyfng.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3uckbwkgg.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3otpqmvxl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3hzrtyzal.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3gfqsmomv.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3dkjwwkty.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3pndfrhet.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jocealch.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3zruoqvcy.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3sukciyfe.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3fnehcrrl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3qtiuiepb.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3vohtulbl.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3bdqrkvor.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3bfccgnuq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3qbmmlagh.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3jycpuxly.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3cifgeiza.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3lqjfvbkg.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3ocsjcaff.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3osozwkqd.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ijlkywez.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ktkrinln.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nxosjpfe.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3csvfaues.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdhucdlm.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3xkyqvogv.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3okgtkegn.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3tageszbi.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3opiievmq.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3wkggaodr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ejeolnfg.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3svynpclz.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3dffihvio.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3hjmxqydd.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3sxuhmaqr.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3sjtlxvqd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3fkhmwxde.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3uyhamaxd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3ugjpgxwz.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3lrmerpdl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3qicemdil.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3fghndiog.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3fclbfoyd.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3njsjxqyg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3jfavtqup.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3qolcmehx.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3tbfvsarm.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3vhzpkqmb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3pvymsdho.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3gygcebvx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3qfxinpuk.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3hfzgyahf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3uzfrwusj.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ymvighzr.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3dhbeirco.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3gjmlgocf.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3breaglih.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hbrsgezg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3elikuocn.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3hvraanlz.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3adjaecau.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3jzlutebw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3jteibsbz.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3cbwtxvtt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ifhpwxgy.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3hstcilph.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3hgzajxqe.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3hksjthci.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3wzrmeszq.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3nbzeetgd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ntxqmvdm.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3ffynsrpg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3fcpjloxa.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3pxhdqgsa.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3fohytobf.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3stqfaqnc.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3ufycsaro.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3kcqzuolz.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wzuuvjsk.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3keqxgjfb.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3fbawilkv.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ldtmtakb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3zfuanjrp.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3fbugocvu.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ptistdaq.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3fvcaixnn.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3unhxyepg.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mssqidvk.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3aehimsle.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3zhivndxt.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uqdscvki.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3rlswiyje.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3utwrgsau.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3gjswddgd.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3hlfxjbqb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwprplij.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3qdgrkfws.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3sgsnhqwk.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3ysdcarnz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3raoyqbnd.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3eaipyhah.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qyogaabl.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3ggrwsbtg.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3cmylzwzp.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3tyaxzkqc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3wusiqspu.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3bwwkzqyw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ebgdydza.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3lqucurrc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3xfumlter.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3levmolme.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3mcrnvuvk.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3pynuvwaz.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3funoostq.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3imuqkhyj.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhauzugz.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3updouafw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3hxkxykgk.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3ndcoqeps.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3opgakied.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3fmorrcdx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3ggmbcxkm.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wcfwokbj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3muxicxcb.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3vinsbkxz.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3fwxyphty.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3wovoazkm.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3pgsuikkv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hmoutjqs.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ariihouh.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3frnhmumm.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3dmtybvtp.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwjpwexd.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3ynninfwe.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3zmauuaif.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3nqsfoglg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3eqnvlgvf.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3izldtmjr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cajszkuj.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3xfqksxqs.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukaqtyve.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3mbphxhgt.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jlhzehby.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3uphbyqhd.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wlffstui.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3dssbghda.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3bnqrtskt.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3rsuneaby.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3wgsjyisn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cnfeoqvm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3eaifvtms.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lrtohrwq.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dfeprzur.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3axganrfz.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3zitojljz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3iblfkfeo.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3akvyzuhp.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3mxljutyl.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3isourldu.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3xftcmekt.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3reyronwo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3jssqduvk.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3wfpfzieg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3mnigreyc.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hbguzwiv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3qfubhtga.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3rezvolkm.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3bwnpcmap.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3hutqhoud.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3hqcorixq.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3madyzoqz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3uwcepqra.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3ahltbjih.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3bysbcukk.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3zknjfhfo.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3praelytj.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3sposvihy.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3aalcdgda.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3suyuvggy.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3hrfpvuff.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3envcficj.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ednuelnp.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cirubfsf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3pmorrzjc.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3shctmkni.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3xokvkvyv.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3silkuuio.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3fhvottte.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3mcumykqv.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3xabswgmz.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3wxhnlwei.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3xslrabmw.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3mxukmhhl.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3ldigjhip.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3blhysfqh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3orhkamjd.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3wcupbhnq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3gefhbskz.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3nqckfoyz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3psxwvhkr.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3yqmqrtnr.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3eavbskaw.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3lzxtcirs.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3orpoikib.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3nqoubftt.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3acizihak.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3fkijufgt.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3rsksjmid.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ufoxbdxh.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3gpmepowr.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3sqpffffz.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3zgucogae.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dsbqmmyy.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jtkmsszp.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3vxglqzfv.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3myhdqpqz.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3cquwgkjm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ibzapgce.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3lvhyyffs.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3kdrvqqok.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3vegvymrb.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3lfpqlznj.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3btwndbla.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3lcqdhodj.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3jgxdkoba.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3frnexqtt.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3ackbvlpu.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3wqsecgmd.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3dfarqwxj.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3eqixhhwb.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3gzssubjs.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3uejqwerg.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3eyzkcslw.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3xrfkwhox.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3jtambhdh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3qstxwfen.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3wkgrrsdk.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3eslwvimb.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3nsumzwte.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lsyppwzq.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lybjojdl.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztsznrbi.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3fjgpxgnq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3mjrjbokn.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3afurpxrj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3jwagntmq.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3rvupijzh.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3wrcnrsmn.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3jbkuqljr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nacnnoky.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3czgprscf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3uaxzrhnp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3ktoekvwr.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vftcktuc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xxsmviuq.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3umacldmf.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3euaiarni.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3pjkklowo.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3mvzotpww.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3clevgjos.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3nccmcucq.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3amgssvgw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3mtdcyltz.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3gtuuoxmk.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3zywmaecl.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zqxslwzy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3kslgjvmy.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3zloldhgt.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ivojqagz.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3fmwneqyw.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3jmetyric.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3qahhtvtx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3osgtxnsb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gqpnflqd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hjwsnxpz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kzuxssue.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3zucpixms.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3oqnwivit.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3tbzecmyl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3veoraugw.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3yhzmzgsn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3jjtmdhfr.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3nyaaxuiy.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3bhpmytxw.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3hueiqoer.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3pfwkkvrt.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3adnukakx.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3ncvnncon.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3xgkvdydb.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3mahtijqg.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3rxrxljaq.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3rnfcobar.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3uluintqx.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3jwfgcuhc.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3rygwmiuc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3bobwrjya.html


<!-- 参考信息 -->