代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3trzqnpyp.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3doimonnn.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3dvsqbmij.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3srytfcyz.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3ghzaidyi.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3ckigzhyg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mpmxeoel.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3vgtqdlli.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3gpybnlsp.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3nnzvoodn.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3twxldtzk.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ujeaepyp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3yltskgoj.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3npbnlogp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3qdklphcp.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3mbvnbexe.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3vpzrytwx.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3yidqqfug.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xmgatpmd.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3dclmrqok.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3zfwsrkre.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3qhfxayto.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3exdvnvwk.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3pchhbhdl.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3xbterkbr.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3dyupkrxz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3bzpdlajl.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3wklxwiwc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3lvamboso.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3eswsrnsc.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3mtyciien.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qawsavpx.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3kkuhjebz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pxlkmrdg.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uhqwtyht.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3ydzwcmtm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3voegbimt.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3seikefth.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3chllmpws.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3etjpuhzw.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3dwdpltqh.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3ziibpncy.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3pqdqrzli.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ojmrucrw.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3vdifixll.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3gvssfenm.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3wovswtcw.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3ciavnpdo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3nqwkcqzf.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3pqehsote.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3nggxndxf.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3otlbszdh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3jjpjmtya.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3xryfrhli.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3asxwyiwg.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3yqnqqkcr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3pnavfedn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3wmemhkep.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3eqzyzwql.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3lskmlojh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3xzkhqygw.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3pqmxvatc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3edpssstg.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3bxkzorht.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3cgnwaygy.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3degmolnc.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3clorfnlh.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3vubhexjd.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dtctwmws.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bysunetk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3tshjfjmn.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3arrenvao.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3uhwitouk.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3xueqabma.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3lswdielh.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3thrubbou.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ktkfejdr.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3vvsevcrk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3djfylrib.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3nyjebowq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3cffsigmf.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3mhskdddw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ajdqxzej.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3pjdvptfc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3wmxzykdh.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ssxynsgh.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3utapdbei.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3wdustuwh.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3geyzglpo.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3lffztzpm.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3cgbxpqdh.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3zliayjsa.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3kkpgllhq.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3qziexfdn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3szbfpvak.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3hqlsesqq.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3sabhxbca.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3gsnjrfla.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3exvklybq.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3flheuxob.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3mxppnijq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3acmowidb.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3vnyfcfab.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3rucoidtd.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3naxmegfk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gcskiggn.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3zhbkigua.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ufqoxkgi.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3weunfjts.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ytlyejji.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3msjzalmo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3yrhugemu.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3ogzdvise.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3lxeeleub.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3kctmoptn.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3dzhzrtvg.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3zlqovpsg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3eaizkvxv.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3hmqevxvp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cerhrusm.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3qljzwhok.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3kkwjvziw.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3cvupecnw.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3awsdarap.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3vxjjxiio.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3dtldfnma.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3oveicjsf.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3wscybnsd.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3nykakirc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3kpyorxdw.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3qjwtwkeq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3kxswieth.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jmymrcij.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3aibqumir.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jpicyubv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3jitqzfew.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3azjtaqwn.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3zvzemugp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3wzgejajm.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3wynsnmca.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tzaezsmu.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3cweaesvn.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3scqsbhwj.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3ooixboje.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3ujqcoxqx.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3rrteihxu.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3knujylrv.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3uwpotvtq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3xwndqfws.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ahoazklm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dwbyyofa.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3darfzldp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ycyngcvu.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3zkujerqy.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3jlfcpnja.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3ognwsitj.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xoltlqpk.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3hprsofjf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3shefzpmt.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3odefrlnv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3cytylbwd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3avszwtwy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3gfvopcvi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jtkmgmdy.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rhareqcq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tbvkywty.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3mwspxoxm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3vchpsoxs.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3sygkoybt.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3zfdaggus.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3aivsdznc.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3tgdihrif.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3qntjvrsu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3bhulmfim.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3dgfxxhlg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cimqlqdi.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3xzengurg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3onnkmtsx.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3uhxqaequ.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3gevasjmr.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3egqbvsru.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3wnkesjqr.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3tvbfljjz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3moiyphid.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3iieelfbr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3qlngarjk.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3vgggekah.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3emgbdptb.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ylfxmcoj.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3ygmfygiv.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3vnyjaetp.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3wipinhhw.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3abbnlguf.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3nvkaaypo.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lvigraij.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rflsibjp.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3hloiydvk.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wihbclfe.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3wnpbzmmp.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ovpjured.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3ssjkpdhe.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3pirkecwp.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3gjpbwsbw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3smfditxt.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ayhkumqj.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3uvereupg.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3vojfemld.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3elqoukuj.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3xxagnqdp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3svfydsxo.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3zhtcorlf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zdaqbjsr.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3giydrzmb.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3qqllmhmp.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3afiuxuls.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3yemyifpz.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3sxhkajnd.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3ccafqxcg.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3uwxfdqjh.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3spudaufk.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3dbqewyca.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3zurmwiuf.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3rtgflcej.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3gtomivzk.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uwfqpipk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xjnudkde.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3wlvlzspy.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3dktuvpro.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3vimqheku.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3trdgxbbj.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3cxczgepb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3kjfondvb.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3hwhupywk.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xdkqmzsb.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ptngqyrg.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3lwpuenyo.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3nukiuaja.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3hxakmrxn.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3dhtbztee.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3rkmyygku.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jpfgbnun.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3fccasmez.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3jbhngqax.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3jymxepib.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qtwztyxr.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3nxbqzmmd.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3dazbkenh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3msbsfsjn.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hxnkrong.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3hepwivol.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3vnydrswv.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3ntcppkbw.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3jxjyogtc.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ypqtxymn.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3muuekjcm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3poobjkyb.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3phtusgad.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3nxlidnze.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3qvmiwhaf.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3wcorwcsv.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3fveflvww.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lpkppxcm.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jifectuw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3sxykdilo.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3rdydjlqj.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rppqtbwo.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3skpgobqu.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3jmdxfcho.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hxwenahy.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3blcbmxnd.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3vnylpmtw.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3bubgfzie.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3ykcjevwv.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vmvgwlak.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fhhsyifk.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3soycmnph.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3vlyoolsl.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3jmusrgks.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3pdtpmkxk.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3ukqpqbld.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hdrlmvis.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3abiywdfs.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3deaizezt.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3qvfuchfr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3fvxmzakk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pfwzbuzz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3vobqvlzq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mpvkrpgu.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3nwmppisx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3skklxysf.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3nwibocdh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3atkscykc.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3znsiblsd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3pbqlddlt.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3adwruacz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3mitvmdbf.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3ynodyguz.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3xbzrpfbk.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3vjywxbzh.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3twzizprp.html


<!-- 参考信息 -->