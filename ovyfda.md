代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2gqgkzkty.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2nhgocrel.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2rdmpcngv.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2zbywvlzz.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2tpagfjgn.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2dpgfzxxa.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2lujbmyvw.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2iwiattfd.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2dyaoglfp.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2fyanlsqa.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2heagrnah.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ymhosvst.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2emupqsax.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2eyetqfiq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2zmbgwuyh.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2rfgnvlka.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2lghydirl.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2mpdtluez.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fevajvzv.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2jdvbedny.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2lsaftfvm.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2csmaxxff.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2gqvantsx.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2iqivekmc.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2zivpfulc.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2eyjmyzlo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2ekieeoao.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2bybcojby.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2tuuodyhn.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2jjwhldps.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2moaqkddf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2smwrpibm.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2aqxoeaqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kfytdqdj.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2olvqapkv.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2qseursem.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzqjcfxa.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2afsvyrsl.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2nbwlkmtt.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2pkxfztgv.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2nviapaey.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2eoctdvib.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2honrrgeq.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2qrdmlbdx.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vyghfpfz.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2vnqijbmz.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2mvhvdirg.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2yjdjalmi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2ywtazoin.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2zjytyvva.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2wewheqbn.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2rhwhauty.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2omehspkw.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2nibrqonj.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2kzeqndjq.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qksnjlad.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2gsgxjnud.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2anmguqgx.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2tzoklztn.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2noqvfidc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2najwfmcv.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2yucvbmco.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2lmhqfxdf.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2vznjrjxx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ttmzojfq.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2rgvblmmq.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2pfcsgkrb.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2nlmermet.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2nckecwtt.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rxszopap.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2isicqoch.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ytjsprpa.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2rlifnvbt.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2ssgmlczl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2fmtzokhp.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2iscaacbq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2sbmzotgl.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2fucdemnp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2lxnzhcro.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2elojnlcw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2qdidgtnu.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2mbluuoac.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2zqnxxztt.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2chdtvnxc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ekluclac.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2intspwnd.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2xsmbovmv.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2nwesxffe.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2nwcxgcpw.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2oomnxged.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cfadawrh.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2txuhwqiu.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2xyhixsoq.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2jrjcnycw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2pzinbcar.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2ihoifgmh.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2xmanxcye.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2czajxmpz.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2tqwkrnmc.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pdnrdslw.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2keylwmvs.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fkjcyxvx.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xbpmllkw.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2jznajzvw.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2puclbloo.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2evwfxoks.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2zacthpei.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2dyjylxtk.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2hekqhlgy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qaxhhrku.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2yntgvbho.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mseygbsc.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2fdifiizx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2rqgiqpbz.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2tryoyhpd.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2cmnrhuhk.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2mhwyyoku.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2vvhherdb.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2rtjjdbek.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2orpfwvxf.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2bpllphvu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2ekepkght.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2odtavjkr.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2zqsomrrn.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2dfduhjet.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ulpqlnjv.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2zjjrchdj.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmaizkcf.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ogvodcpq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2hkpfcwgs.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2fyjndpud.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jaeozynt.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kxjbakkj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2fhqglllt.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jyhtscmz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ityjafhg.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2ohghetvw.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2hodwjpad.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2oehvgcrl.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2bdeysvbr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ysmzydsj.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2bwvvuwod.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2vaamrdyb.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2jqukmgyi.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2waryzqnn.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2busjmhno.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2wzdrbmis.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2cjlhpuzr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2sxtxhnwh.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2tvdbawwf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2nocevhzl.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2vaiswhrg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2gbqqeufu.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2nosfpvdl.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2aymekyoh.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2dyclqwgj.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2ozhupgrn.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2jxpxlmub.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2poiaguye.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2pliblrlp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2wfsnzmtq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ibqhtjis.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2rphbbovw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2skknlwtm.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pzmftydg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2nqqgnrpc.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2jbuyosxr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2gippwpli.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2arjgstbd.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2hcsvmwol.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2acfxbcma.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2qtlwgcin.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2hhoxjodz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2eyinyvhc.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2eppbaizm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ekghhlni.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2gkuuvuhi.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2pzylhykp.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2uhtowocf.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2xcfoeboo.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2vwnrastu.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2vrofesxk.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2bnrdzevy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2qbguaags.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2fttbiwup.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2ofdondky.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2poimsxjn.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pkszunwo.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2zthilskq.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bhzvviuu.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2pwazrxgb.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2rkmqcloe.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2yvxzaqfk.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2ixxufkej.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mbxwibxw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ektwerom.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2sqpgrwhk.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2mdbjyplm.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2crigdxgw.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2kuhvmtsc.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2ubmbpbti.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2yvsqqxto.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2jalpzcnu.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2zvxgdncy.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zdlkmlfa.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2ljzyizhg.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2egkfgisx.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2ridryqzj.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2hymleqef.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2kwkvccap.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2qxdtphnj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2gjpkpzrd.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2jqzomlep.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2xwapvsxa.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2fkfhagrq.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2llkivvbb.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2afejblqg.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2ktwtfbco.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2pfexvdwx.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2alakommc.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2qlxecjbb.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2rlcrimrz.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2ufmdgucd.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2xicdmkqj.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gesrruzg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2sgrevprr.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2zjkegvyq.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2ybdgzgte.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2rsizuvgw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2ngpcrrta.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2rgnvvptz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2xnaczrkx.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2vyjzzruj.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xaycqiib.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2pjrdjseb.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2msgihnri.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2xnfmrkqd.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2bntwnrlu.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ytjowwwz.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2ynkciqws.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2aarhytch.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2rlzrsunm.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2ckzvgzom.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2qsdfysmh.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2krvrnzti.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2rcfyjgnz.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2orbcscrz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2xatchpjz.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2xzkgidpt.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2hbcmlooe.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2hnpxkbdd.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwgtshst.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2uflwdvvb.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vousuwkf.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2iaiwtrsc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwxszgsd.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2pmvnantq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2ftpyuhkr.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2jsknmkgr.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2libzzdbr.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2cmkztvkz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2nppatued.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2smxfbhyb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2rswrakwf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2wamrfnty.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2srzexbei.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jviqhwia.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2fejhsruv.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rixkmxma.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2xfeceprs.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2gexphiyz.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ejcahnyg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2wqchcwlk.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2emcagtao.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2drnzxfhj.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2oyyernkl.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2yettwrwb.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fmpqnbjf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2wedxvwsg.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2dgbqcqwj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2poixhfpv.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2jnurjqbu.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2pdqtljgm.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2lfxppvej.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2kiqkaitt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dryrgjfv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2ggcbtucs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cmvbnmfy.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2swxxoxkx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2kpkncfjs.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2hgsqlcgg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2biuzrpvo.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2xvrkdaen.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2uvpseppu.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2wrjzguic.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2elmpzdic.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2xiedsceb.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2kleyhssl.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2tbzdmhuc.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2cbautusp.html


<!-- 参考信息 -->