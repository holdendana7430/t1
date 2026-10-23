代发 wailian999

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3dqvsetsl.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3zlmlptok.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3ceyoynvq.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3aaikiqcd.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3cysnseny.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3lrnlxoqp.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3mdizhlez.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3zssjtiob.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3nzqwqesx.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3vjsuexzj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3nuxhrniz.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ztlkybma.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3glkoccuy.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3hqgwjwad.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3debrsoya.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3yiievfoc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3bymohppw.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3wnulajdy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3cbpyryvm.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3ypjmstsu.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3ccdsruln.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ncivjetb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3abzdolzq.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3mimhhpgi.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3ypoxzrjf.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3vqbagqhu.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3bxexfuqa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yzohixmw.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3jcurnivw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dlokcyxe.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lvzosqoy.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3xtkjckxj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3mfgjsmhi.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3bzkffbeg.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3ononsfbz.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3qrhlfojg.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3ddyqxwnd.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3zsapkwus.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3rwigsltz.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3aefvtyit.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3afpfcclf.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3fzivomci.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3ziffqngx.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3gughxqoz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3mnnlfora.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3mkbgzmgf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3xtrnvnji.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3mcpdbdow.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3tslbhmpb.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3wuytovrp.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3enhqzwmc.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wuyksrms.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3acxrtvha.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3xfvplvmf.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3kdlkpxfg.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ommrufps.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3qdurvicy.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3hggihesf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3fhepvlmd.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3pzyglsym.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3tpvxrakr.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3ccrosoes.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3jzqoksri.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3zhlwkfqp.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wgzeeydx.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3enajketx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3pnlaqqhf.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3baxjpchr.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3rpsvcngx.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3hbyhpiqa.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3nnimrjao.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3jjmygvbq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3meysqlmc.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3wressgne.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3zsuvoxrf.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3mzanfqvc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3ebyntpbq.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3bibwymgw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3tenfglzf.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3ivgnacbf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3abcrsehb.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3afyhqcis.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3kttpcrdw.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3vjwlcios.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3hlelsxcp.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3smichddc.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3uuwtswmd.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3pqkioayx.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3yddluisx.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3npzilwig.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3iriawxlv.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3xkbkmong.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3wsffddav.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3xouihtto.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3ualahqoo.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wugtkafy.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3taaryrpe.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3phsloriv.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3aifawsxm.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3jclkwxta.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3tlkudqun.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3tbedqjoi.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3wxbwunbu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvskrjyx.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3kvexxcyk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lyalergo.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3nzuczugw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3sqwfpzoy.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3ujrvvylb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3sqorklgi.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3irqoprgw.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3fonlmsfl.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3ievuyjhw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3dcmionnu.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3qxicoitm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3oxaeedvw.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3crbopmtx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3zuvmdeea.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3ihwtyhhx.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3xadzflhr.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3tlgzhqbk.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3fvdfdpgm.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3dqyknabl.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjfuzutx.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3gejuorwe.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3yxspdsfp.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3swffgurr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3gwfvcvnk.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ryvyniqi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3raocxegz.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3sjkxuabi.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3fcmvtavq.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3zkbdydak.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3zmgfodxh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3mxkhgigq.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3ivwxvxok.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vldvrcup.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3tdcjcyco.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3brmjqhkf.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3lawlckui.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3szdspgsr.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3ygdfvrfj.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3semczjyb.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3rielytuw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3tmsktxdh.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ovmbwjof.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3jnnhxglv.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3abbfghyd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmkoodqj.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3hhoruafb.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fxhungny.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3wkkkaahh.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3zhdohgxd.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3vfhpkssl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3vxmiarmj.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3ljskuidl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3xpenqdsf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fmmcutwb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ljnoqtdv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zilrslnu.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kgpvkakq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ukxhvjwg.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3wqbrlmkf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3jwgoowbz.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3lcwdctba.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3oaadrifx.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3lfqqkwjc.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ileyqzpj.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3yadmghor.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3zokxdlwd.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ziteavnw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3sfiadzzw.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vepnthjm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3xujbpejd.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ruqpiswu.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3xfcbsfrc.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3fkykmdly.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3tioeolhx.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3kxnralaa.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3wmivkkuf.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3byetllac.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3jubeebsj.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3hcxyntdc.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fzhaixwe.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ofsfwmgo.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3qtrrguhd.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3shrkjvdv.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3sslhlsob.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3ewfnqayx.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3plfwcimp.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ufcudzmj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fdvlowmp.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3edafpwcd.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3hdltlzpn.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xhxouzbg.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3tdxzytpp.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3qrjwfqyi.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3hvnthktw.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3rvixavvh.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3bykwectd.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3yfrvtycy.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3vghocgbi.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3hzeztaoc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3oluuicbz.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3szlonrhw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3grxmvvvu.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3nhpgffxn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3znxiacde.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3arvcsjrz.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3ebqrkcof.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3rnywqvad.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3rgktottb.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3szsjbhxq.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3otwopwqg.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3xunqgatk.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3gwtnzeyh.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3qysbbczk.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3mgrpmyxp.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3tyioagsi.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3ofgjalas.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qmwhlszj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wphcjcmq.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3yfuewcrw.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3qhbattcg.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3edfyggct.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3qzdvvmhq.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3fukiwkuc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3apsyglxl.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3vsuudprn.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3uppsbthq.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3vmcfiguy.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3xqulyxyh.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3riajhgmd.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3nwqecyeb.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3hdsflkdi.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3xsmnabha.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jxsttktg.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3zwqkzchg.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3baluwfxv.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3iuexewdk.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xobrckme.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3abthehiy.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ihchfoam.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3kmlkfrxm.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3jjdivxth.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3cwlkookl.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3wlicrjyo.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3oogkejgm.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3czsklvie.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3sffrkidf.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3teotphqo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fuadiogp.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3npgtwgby.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3pjfuvslt.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ifeialmn.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3zyeyfflk.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3caznoese.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3mccxmbyv.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3nrdqhrta.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3dwavgcfp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdjfdtnd.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lpxiebxj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tkferqdf.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3iwzgvlpd.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3esignxgr.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3plembjab.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3tbzvksdi.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3boporfts.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3uhvlzueh.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lykemucd.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3dabkvyiz.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3tiamyjec.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3tmmaqngm.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ztkhjgyt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3fdparcyz.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3yuekplad.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3iuejndua.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3ljpbbakp.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3zjsyovsv.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3jpxilcnw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3pevszjhg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nybmehbv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3tcehzwih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3abzpzwce.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3eaxqzrkl.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3doascfof.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3voqxiyst.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3kanyrtkv.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3mmkcdctt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3xefnkvok.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3bsekmnir.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3utksovzo.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3xcgidjyp.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3vafzmcsi.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3pjecbdsx.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3zpyyiqhf.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3lsucbdgg.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3kniimejq.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3nbfdkkbm.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3ijtdmdat.html


<!-- 参考信息 -->