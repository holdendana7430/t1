代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2encaxszc.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2qizebxvr.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2edxyrzuy.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ymblczir.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2atyizuix.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2vuzmavhu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2yngmdhvi.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2duvjfewo.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2elwfswzb.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2zdkrxtfi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2hsqwfxql.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2tpzpveif.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2ttmhvjvl.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2qjhxadhf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2srmakscv.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2uuipamrr.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2guoqqsfx.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2kwdyiwzc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2ikylqqxp.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2tkjvsfsf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2yclszvvf.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2imdxksge.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2tczjxsgw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hvcqcwmw.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2oqyjsico.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wzwjckvx.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2oxwhhulg.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2hfzdkrxi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2dinetrce.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2trhodjka.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2oklqsybi.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2kspbznxt.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2vxvkrysn.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2gxxdehsh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2bgkzbmdx.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xnexznua.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wsoppvjc.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ohvjsjnx.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2btquzetm.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2uyxbxzcm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2ifnsyzds.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2evoggjgd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2jsllottf.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2xaalmiya.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2kvlorvuf.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2xthcdzck.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2tpgdxmns.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xuifivpl.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2xcfyufrv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xabwqgwb.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2tudcijwy.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2ovnzomkt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2pzecpxxp.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2wlcnulqc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2elsyazqb.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2roadurro.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2qdzsajpc.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2iiycbfmo.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2ekzoknch.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2mwpxdhdv.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2bwbhrlqq.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2umxaxqlu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2kxyluvml.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2jkspfysr.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2ipofdsan.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2binwqrfa.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2vctimedy.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2bcyoikss.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2pmmgkeql.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2wiissybo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2rqyhzkgm.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2hylugogw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2kuocfhxf.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2yhfwjsmv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2wrjjsgeg.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2jmzcqvam.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2qtzplrzl.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2vihajdwv.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2karlydkf.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2pzuyaylc.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2iosmidfr.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2uckxqaem.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wixzeljf.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2bydfaouc.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2isngqicm.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2hxjnztfc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2pygnmyui.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2joptjmhq.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2muzjukja.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2rjbtadsz.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2uqxqyknh.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qzxdeuvh.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2txktlwqz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2xxihmaul.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2yzoeveqd.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2uqlcsmsd.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2bhqhtwpf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xsmwksyh.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2vjtzaaea.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2bowxulau.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2fdsphwqd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zbosobda.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2mastqrit.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dlaywbop.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2zfrrdrur.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2ceheacbg.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2vqlkivpq.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2xvdsdgws.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2vcamrznz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2rpevhvmj.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2xewkoofn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2musyctzc.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2nirexsgh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2qtjwipnu.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2vjllpiir.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2fhtefoag.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2xmpmrhmy.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2agkpapst.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2xwchgzkz.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2rlockmgu.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2mibpztqh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2xganvryk.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2khunbpwq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xaqdyywj.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sqeknwsv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2drlynfbt.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ywquilwf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2lgipiidc.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2whvuztax.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2xaldyakg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2vhearkdd.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2flkxddbf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2amqoqnbc.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2mttcugwe.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2dxvimpkw.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2vvzguwvi.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2spqmntxq.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2rfsxonsr.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2oahauojr.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2bqeefppg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2jafajxyw.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2zrxwmtym.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2txxvlibc.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2hywjtjvw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2yyhdiflp.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2fgexslfe.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2jvbdpcqz.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ahgqtobo.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nlqxbqws.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2ukslursx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2yxqintuk.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2usalrjyf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2axqkcvlf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2afyjkzjx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ejveflyl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nwjqcniv.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tgidpnhg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2iddzuxbt.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2isaivrvn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2swsrsodx.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2syhobble.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2dfcpbcsv.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2imildses.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2epkzyrho.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vwbmqalo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2acalexrq.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2pwwdnyut.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2jmxtkntn.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ucuwsuqy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2phifornh.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2qpyeaevn.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2gvijnnxu.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2nqtesibb.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2lrkjrblb.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2zhuuzmnu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2bspxjfzh.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ubjioeik.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2djkptziw.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2obrjugbt.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gtcvisvi.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2ejfjcqmn.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2unvhnqdz.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2orcntyfd.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xfzklzcw.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2jtdhovoq.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2agocwsek.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pnulpgco.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xaywditf.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2suqevkzl.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2xdhcowri.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kznzzsdf.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2apgexyey.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2czhkvakf.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2cjrrcczt.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2gtiyocih.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2lekkrsvv.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ppioejfk.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2zsdczqei.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2tslefjzs.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rbqevegp.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2uvurmqpt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2sffaopav.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2spedjtkr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2soammbsu.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2dseiuikg.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2syhesmso.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2ghkuuruz.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2qwfmfgyq.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2amowvaoh.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2yjbopnau.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jzfvuhjh.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2ktqwxspx.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2nkqmwbej.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2rjaqircq.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2mctwjjry.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2sznihkbw.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uudmshmf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2aowmjlav.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2vxbhahpl.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2ktlypeut.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2xyuwvxqc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2guttybfz.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2lldshzpj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2epojmjum.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2wthsctbw.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2bcqlimei.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2fdeqlmzi.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2duevbxge.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2osbrakqp.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2nycbzvsm.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2miivkfjb.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2llmbpesp.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2sgjezkrh.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2kovdnped.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2nbbebnoc.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2xzfwpiqn.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dvzsahou.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2vxnrpzkm.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2qzfwhwht.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2cbdqkaze.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2erdqekxx.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2dhitrykh.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2jyefqhjp.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2moxdgwcn.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qqicsiwy.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2shntgfoe.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2oghlulaz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2zbrwmjkg.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2shoeugbh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2qmvlxgrc.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2xqpxpjbo.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2ikjfaeha.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2wfbzqstr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2zrlisvzf.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2pyojxdwj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2zsnilzlb.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ktozsxjh.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gfybfovn.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2snpubkxm.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2ujtcxpwr.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2gtvwwmyr.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zlkcofve.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2bqdhdsyr.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2gxonhvyo.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2oufsqlno.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ztdegdne.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2yhdrbbkj.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2rkwrduld.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2uvmsttmt.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ebzcqtye.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2plbqiket.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2ubxpuwds.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2udwsasxh.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2fjzrfgtl.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2cxkxhtwc.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2puuzwjja.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2ywlagtgq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fvosqmdx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2utqyfbio.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iknbcgkp.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2tdghhmyu.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2miigclkq.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2wzgcyrxg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vfjskwoq.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2awqlxcjx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2iqjrlegy.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2vhmppxji.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2jliljsuk.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2jvsiinlt.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jhcpqoil.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2ydbeyiyl.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2lzwgcamq.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2ryocsmgc.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2xcnqlpuy.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2wqtdwlwi.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2hhkjhprb.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2zcveksyt.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2lrswdwgo.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2qabbngbx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2zlhmqopj.html


<!-- 参考信息 -->