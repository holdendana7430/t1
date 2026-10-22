代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2vueelrvw.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2ewqdkrcp.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2egnnpguk.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2cakmecxs.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2bbilofay.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2nwnnzqql.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2aqvuwpcn.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2luycwxhx.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2rqxzxvli.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2rajciemh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tterhbam.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2prkbcoef.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2ewtjhysb.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2dakytkmo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2phvpwnwq.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2bwtfthli.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2fvvhrysy.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2kewxncdx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2bvcygelt.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2egonndum.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2wschbexx.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2qloaxvle.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2ganpiacy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gdhjuxmr.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2pagfpfmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bqjhiulm.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2caxbycym.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2klcbcoof.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2dygfmnql.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ggmjqtie.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2xswcecnj.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2bwgohpuv.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ybqtvlni.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2dajcqrtd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2jdueumsk.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ftokhpec.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2koxsaszz.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ackknyob.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2smtmqldw.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2sdyoidck.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2qmicljlh.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2lrfikaua.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2jodibnqz.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2lidumnba.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2xolsiwdn.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2iuicfdtf.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2dkqhlncg.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2grnochtv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ilspbqjm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2bpveanle.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2yndeowjl.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2rbnykjhw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2oywcceyf.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2zyfyahlr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2cjqtgjhw.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2fofuuzqj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2rumkgehp.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2iggwqpsi.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2lkeddyeu.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2pbaqazct.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sadmsfls.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zvjcjecj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2qdvggxzn.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2nrvrgsjx.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2evymiouk.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2rgvscyek.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2cmiksbim.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2yaywdcrg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2eululdrz.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2xiftmphh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2kqmqjigj.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ehbrsxza.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2zizbcxrf.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2gihhjxhr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2cihceqti.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2cfpbnfyv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2giyrtlnj.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2uugqrpvs.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2gwodocme.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2rlrxmtuw.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2dhfalusi.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2uoidpqqk.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tsnwuhqt.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2enxttntp.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2wzbozcan.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2qvqgzzsy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2vlrxnfvk.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2jwvjwpby.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2oujjbmxd.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2dukrvchz.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2hjhunwrt.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yoodpigr.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2enbgujzw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2awrwltoq.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gmcvlsvh.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2srjktsph.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2ipwifiry.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2pvsyrbna.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2nczgggpe.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2wqfdvjxn.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2acbljhby.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yvoqhhnh.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2mnmrbpik.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yenglken.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2ngvktiik.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2jzhjftwj.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2fdzilshu.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2vabqzkfq.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2njqmnera.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2wlcrozms.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2myjjrfsp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2asjjxtbw.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2cukqhytn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2iiauojwj.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2feousuqo.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2otzfeqyz.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2rucgyjdk.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2gkpvikhi.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2ymsminbv.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2zokidgpw.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2vcpuuwjh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2dgvnmrwz.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2tpfmzozy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2jplbptei.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tqlpgllt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2abmubfah.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jfjbvlhd.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2aqnzcusk.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2ghsbzyzr.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2cgasmfxq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2aysbaxga.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2xqfbcley.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zqihnqvx.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2zbxrznap.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2ybgtzjaz.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2rughhdrs.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbielkdz.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2kncmyzkr.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2ebdyddtr.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2abtdftph.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2itlmkxsl.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2rraswvhz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cghglhnt.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2xoisidvv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2djygjrpb.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2ihxpscbk.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2vqkhaxfy.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2erfgwlpy.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tdnmsfeo.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2zvwtmolu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2kjgftswv.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2xzbsloav.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2iihnoatk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eypqqied.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ebmgejqi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2viqpxebw.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ziqwpiss.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2koysexek.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2mimrdzdz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2mtfuimsl.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2faiatcxs.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2bdnqlyxm.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2ihicdgzm.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2bjeqfzec.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2gxxbenml.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2qznaevjp.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2vqkmqbns.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2aqpispev.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2eipwotbb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2wyvvepvq.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2zyyabpna.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2nsrgvlnr.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2acnecuom.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2yckucdmp.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2kbpployo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2ddfabvys.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ftmolxby.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2knqxtcdz.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2zfhvveav.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2slzhpjip.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2nlzsulrr.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2gewnartr.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2nxhvkkof.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2gnmzawzk.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2qgrjeibe.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2rarhdvfr.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2eswjdotm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2eofhrapi.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2xpxgeyom.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2wfwbkzas.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vemgtshe.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2xusiodpf.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2rvfrpepp.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2wbadtsov.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2feepouaq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2tisznfgd.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2nhupndeu.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2ivfvkqgb.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2cmadabna.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2fngrpqgq.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2jfrlkaof.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2yhniztbc.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2byetdwjp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2peexqsud.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2rdcgzvrt.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2vlehiefs.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2fdooendu.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2aoltjznw.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2owxuuvrg.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2eolchcoz.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2fhjiqccm.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2ioqyqqof.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2poqflmzo.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2bfcstnqd.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2hegqtkhx.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ysvsxpcx.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cfkohkjq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2pjpjegcu.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2pxzjqghu.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2fvxltgbu.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2sjxohsej.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2ishtxqxu.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2yjhynvso.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2idklqrih.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2hcnbkzym.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2pedxihhq.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2uzaevcpb.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2qlqopwni.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2xosgpvjl.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2vdgfoiol.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2wcrkmhng.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2bdcejcfe.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ecllging.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2vquzfpix.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2wtfkkfkk.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2uixdxyhq.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hrurddnk.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2fjnhwbvf.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2yyqsgxnh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2fvjvxwwv.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wyhhqjoq.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2pblvujje.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2osbgbvpy.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2owcdukhk.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2pzptdydk.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2arpxulnb.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2dxtqrysu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdxjljyv.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2ashuedpz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ccizpzro.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2bruyypok.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2wugygaoq.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2hqfhrfuk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbzyhtqg.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2baommxmv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2imrhsqcl.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2xojkqvms.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2awkwklrc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kawydzet.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2cvamqrme.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ktogtkzs.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2awqpmjtx.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2skonxxih.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2bjdsfljb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2dmmpoele.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2synfqzsf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uwdltdbv.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2xraaxrsb.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2xdjkzutf.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2hyzuvyqv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ahxfpmtr.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2hzfiiygk.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2lafvexoc.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2hksxurls.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2abhqysnk.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2vsyylrme.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2bggxnmgz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jajdmvxv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2pevsdtkq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xqnqhkte.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2fczqhzli.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2oogwqfnr.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2sapxkzui.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2ihgarhmp.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2lkdgvkcj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2weqixgsh.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2ohmrzzua.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2jgheuamd.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2bbdrgflj.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2czoktlhu.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2qjkvkjbj.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2iqbbfmws.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2hcmipury.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2sqhlddxr.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2wujgdrlx.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2jghggmjv.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2xrxzrlxv.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2wueytuuj.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2rlvnssyi.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2wapumjwg.html


<!-- 参考信息 -->