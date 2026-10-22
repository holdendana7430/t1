代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2ryrcyseh.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2uwmpebde.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2qcwbcarv.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2ewycikqk.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2epojatmi.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2fgfzeuye.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hrievmxi.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2qppifimo.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2tcfvnfos.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2euzzxmel.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2jborlkou.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ygylgpbm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2bjadqcjd.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2cqcrylry.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2movhtwfu.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2jsibryrf.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2ksitsauv.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2yxxatbbq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2iigdbtfu.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2iaixbxvg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2xkpzcppg.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2wxwgwqsv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2gjucbugr.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2otuuedap.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2wercdadr.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2ezneyekf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2qcnduifp.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2mqdifrfi.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2cefziiyh.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2nxwomxyp.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2jpxyabbh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bnofgdky.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2luqfyseu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xvfhpvcf.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jtkhmpyb.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2lrybnrnb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2nucvlxex.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2kscpunbh.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2xpnveaxy.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2nvqmggju.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2diodbrjp.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2gnelckig.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2rlwlfmry.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2lsgluhyx.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yyhtsgwh.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2anqdxaql.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2lfqbvcry.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2wxmvhomc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2vizekdro.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2mwajyrbm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2uurnnjlh.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2zyqxasmw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2zckwmbkc.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2jjyadsei.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2chhxsdak.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vzzpotii.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2cavhthic.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2sphlyxth.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2kxnflaus.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2auuzytoq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2xhyxeuop.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2myiwyxnv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2bsceenwx.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2bgsptdpj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2ttplytqt.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2hhjikbsy.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2xitkaccg.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2qqtmpkpg.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2oiuusvkh.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ulriarun.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2hsoasbxv.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2udkydbnp.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2wnarwban.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2qdccpgsv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ujpwgmcn.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2xkcbyyzv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2htgersgu.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2pificekk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2fqvplcyq.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2lccrqvwv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2ppcmhemq.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2nuvezbjw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2hsczkanx.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2lqpxnxwv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2dnnhhomf.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2acyjhrue.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2hhtjwzft.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2dounzjtn.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2motrlwje.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2uovlwbdr.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ewqyjfjy.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2jcdhzmys.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2qvduciiy.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2pyjphseo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2ytqyncny.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2ciajdtan.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2binfldad.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2gniyhvbi.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2rfaxpmko.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gmpuethm.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2bdwhwgao.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydlesgyl.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2iocclkju.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2fgfmkxqq.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2gtkpkfvt.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2bqlqfnbr.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2lfzochka.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2nviqohrf.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2uumurpoh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tjmnsbqo.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2okcnluko.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xcevzevy.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2mqilsmbn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2nsmlcrxb.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2genzinnb.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2lbuszzly.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2dpozoibe.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2molqefry.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2qslnkdhm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2gyasdaql.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2wkcakuom.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2bywizmll.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2viuozdnw.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2chvizbtf.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2noowdweh.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2jifmgclw.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2vrwrkern.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2idorvqjz.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2wfaufbay.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2mbjvkbrh.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2zmhzawgo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2gewxwuqu.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oanxwcrq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2rgfbdvni.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2kksxjgoc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2gurtfciu.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2wdqivgeb.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2lspgyzbt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2vszhqsrn.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2lmwetdul.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rofjmmjt.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2urjcffnr.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2lbydiaxh.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2ufhjxijt.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzlokwrh.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2gmwetbbh.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2kmdfxhsf.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2hcftkccq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2uhcdtjvn.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ykemjxpo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2iupzzfhh.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2kopksroj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2azmbgbib.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2sladldxq.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2peidneds.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2vsckwdxd.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ryeapwyt.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2ovvgaspk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2qxmwvvsy.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2crhjnlph.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2clczafpe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mtheexsz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2hvsavvgd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xlkoiqts.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ennhcmbk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wjqjxlep.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2uimhtyog.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2effnotub.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2cemdmoau.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2caybbels.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2wwyarlks.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2lbmvyuyq.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2easlmixc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2kkvzbred.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2fjucvlrw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2gutvakyd.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ekyfdalm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2cdilyqic.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2xpzuucfe.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2yvljhxcf.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2sfhimlds.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2amwgbwqn.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2oddznmbx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2bgdpmmso.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2rfqwzqpd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2poadksbm.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2ueefdkot.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2shspbmlq.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2qdqdicro.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2qmttacsd.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2rxihhuuy.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2bxuqynfb.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2sufaxtkn.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2nircxoga.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rjiycmia.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ryxcsnor.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2iyidcwet.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2rrqckqpz.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mgyuxgsf.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2rbqjbcji.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2ymxfgyej.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2eilugnmn.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2glyffynv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2gfoaemhd.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dfrjfpjz.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2xsgnublg.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2mdbofrwq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rqjcsbmb.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2ymfnhins.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2zvcagsgl.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2cnoenjsn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2algxsaux.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2urwgocjh.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2ukqlrbxy.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2iizcrhlo.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2oxlxmdab.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2rnxibljl.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2ujneoeiw.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2huiztycb.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2gzhckweq.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2qlqxjcer.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2nrbgeegz.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2gcnqovya.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2xhhzvxzt.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bcuunsvq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2azwxqixy.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2nmbdctng.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2cacnnixs.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2nplxsyiz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2zufkmecm.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2cglqupmj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2jwzpvomt.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2gexpuebr.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2dpxzedrp.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2isaslptm.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2kyduqean.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2fwmhptho.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2umfghklb.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2wffwgkqa.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2pakwdpcm.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2abdjhyxi.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2pvwvhykg.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2tupfrxnl.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2tzccbmgj.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2slzctrbt.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2bevvbghl.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2dojxcnwb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2mnqsynut.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2goqgyxlu.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2uzbuflzi.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2wtpcwkcq.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2vqbuuyjo.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2wesntddf.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2gpkvjtxi.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2zurwgnug.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zzpgsqzq.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2zocshlie.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxawyorz.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2qfneiurd.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2ldkvqhct.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2okbcnpua.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wyrszvkn.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2icjcutmj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2siqxfbut.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2cijtfvak.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vwtxwdib.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qqldlrsf.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2eqdyylwe.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mfxtlkfp.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2tlieyxku.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2mfwuztov.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2xrargqgl.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sztgkxhw.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2phegvgjq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ekaghgov.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2piipijia.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2oplddqxb.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xhajtuqr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2qkuygfkj.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2vvpeyftc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2orxgulhp.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2oouyrrmu.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2nwcumfif.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2lrifyzrn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2dcwtwdib.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2prsipiyo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2fjcshfig.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vlcuppdi.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2oteiebvy.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2irpoqyux.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2vyqxfplw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2lcuytnzq.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2qxvlgbrl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2bnrjdprx.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2ruxptyvx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2thyjfzjw.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2nutpdnhi.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2hreijidz.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2dijpewiq.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2tzjdovwe.html


<!-- 参考信息 -->