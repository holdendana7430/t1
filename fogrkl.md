代发 wailian999

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2phkpqncc.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2jevcjwkf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xkfmfkiw.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2kbbgjodw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ucwdxrmz.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2djjucqnf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2urkjydve.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2jupoiqqy.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2xoafthdv.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2dxgiaoia.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2qrlttwrj.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2lrqegvif.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2pkleaxhw.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2bkggfxti.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2ybqhzqmt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cisislfg.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2qgdfjgim.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bhnezykt.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2addehaiz.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2fdzubyjw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfqyzzbk.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2wfdvzzty.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2wvpmicvb.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2qjvfqmbf.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2bosiueib.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2qwumqilh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2ytodmktw.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2uiswbogf.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cmsmhhsd.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2danafxnx.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2rmgpirot.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2mwshwgfv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2bzgigmjp.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2wluggwhh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2ddmtbsze.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2kwwafjjg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2kcyexzdn.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2oscxanoa.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2pgdlwkgz.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2trpzmjpj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2thtxvjly.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2atbubcft.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2kzjzyesa.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2mcpvpxym.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ecdnrztd.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2citbzeaz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2eqwiyyfo.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2rfiomzko.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2krzcxoga.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2rugmxzwu.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2dasahbuq.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2peivamqp.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2hinscwfk.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2mjmnzaoz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2phaotrqj.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ntyvihuf.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2esqrqqow.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2gsfhdnlw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xtvgtvec.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2lfgjbcfm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ctzjwhpu.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2ujjcnqer.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2vsfnwfpn.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2xlnmeqtj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2huocyxmg.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2zadmwwcy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2okjpzxvw.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2peaqfckq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2nkhbbfla.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2mncerxvx.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2yisyrmiv.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2cvqvsybg.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2fvoiyivp.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2dvtopmuq.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2odtqcpdt.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2avwjvzdl.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2andwuuyb.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2yvavbqab.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2pcejewlx.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2wavxqsbc.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2iicqfzbp.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2vmqdwhbr.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2zyehehqs.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kdbxbffq.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2dqdwwphe.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2sczumrfa.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2kydfwjuh.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2qazsftrb.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2lzgofzca.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zoczaqlx.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2qwdfuhfh.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2bhjaazor.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ymldqjxj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2phybbdoi.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2reihgjom.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2asqcedbl.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2ehexjzvu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rusqopnv.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2hgkiofgi.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2vbauucdh.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2yptzdzyp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2dnnfhfud.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2pjjnwyug.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fihndkes.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2mtoyuwcw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2hiabfhvi.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2kuoshzxt.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2xteygprj.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2zlcuxlpn.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2aefmlrsj.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2xcznmygp.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2puxacayh.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2tdrlhvcl.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2zfjccqgg.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2osbqyrni.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2mfmyqqoa.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2ybsooafu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2odfuhksn.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2czeahxie.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2rucwdcom.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2xxojkfvi.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2magtikih.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2nyyhvhkp.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2lzaifnjo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lsknlipp.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2funfclrr.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2hfhscwyp.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2aksigwso.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2wstebmtp.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2hdbcpved.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2bylsouqp.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2qvgysnxt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2uhqhpcok.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2honzodrg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2eytllyjr.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2eypwxoeg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2lonxqcxb.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2fhcosjoh.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jltffcaq.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2dvhmezqd.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zoqnryrf.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2eipcxqvs.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2cinyiuga.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2mpfytkny.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2dvtzuxry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uehtmaqf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2vfygkhvk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xecuxrfb.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hhvwobpp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2uaqqimhc.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ibmlpbyj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2iuwotvkg.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2egezriaq.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2selgslag.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2tovnoaaj.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2ffhuuizx.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2tzuewned.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2gbsmoyvw.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ueelsxwr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vwzagqjk.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cdodmqfp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2dvacfmve.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2twcxhqru.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2wgagjuqm.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2xavprrij.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2mwyztryn.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2qbnotoli.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ldzeklfm.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2rikjfkgm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2frlvdtnb.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2mhzjngyl.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vmemmjpc.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2ovdvesmp.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hretcucf.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2bfmuztye.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2bizvjqoy.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2ieezplwr.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2hoegjutt.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rwyvsxbe.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lnarrzcl.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2wgyzwuhk.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2asddfnzw.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2coxxkoxn.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2motnouvp.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2vxjhirtc.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2qamjwkip.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2dhhvroxl.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ikmzixpa.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2hwlngqaq.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2rodmmlqz.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2mkgggzhg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2xoklxpwt.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2fcecrhtg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2udphihmh.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2inuztegu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2aaudxpzw.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2wnxgjyly.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2oehjsfjr.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2gtzxfxry.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2dsfovlgd.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2vyrcjepu.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2fzjsdoeg.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ijqwfarw.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2hyksnewk.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2bmlqmmzm.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2uxtcduwg.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2shrvmwsz.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2udhzuwbb.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tihhyvnu.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2lolbqwoa.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2nvgaygbf.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2gajpgpmq.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2ofkthclj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2xwdquybm.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2ryaznnzi.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2usvhvmos.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2bklbhngw.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2couifzib.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2hrijpiyz.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2fptqawgk.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2opzpfsjl.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2evbqycta.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2uuyzbhmn.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2rkzsoabh.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nfhxecdd.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2zgqemthw.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2rougnomt.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2dbjanxco.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jqovqpyg.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2kyvhpukl.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2qavpoizv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2iplxxeke.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kyggalqj.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2zhsnbpdg.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2dztponzu.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2nnbsrvtk.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fbvquktt.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqqsjosh.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2ousfwqlw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2evvamsko.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2jpkjowdk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2czljklln.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2fgaetbxr.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2drtcsitq.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2yryfcpvf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2odkytjzn.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xregtlwk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2rsdjkytd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmmzquvp.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fzrenbwx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2yqcdedpj.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2xfntwqpx.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gwfpgyuf.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2pfogzjmn.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2kwranivb.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2xgcrbvsy.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2zlbhcibm.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2jouroned.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2nqosdqpl.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2cykcjgxu.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2jodgbqtu.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2buibgsid.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2lhdcujjg.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2ibsomtdc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2qguzgdgn.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2yjbgiayk.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2yrqawfzm.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2wdwlxjmk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2tzssvnpn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tnuwonsy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2ypbqltsh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oowpyazs.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2vnlzeszo.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2gphmewrn.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2wxrfxuao.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2quliyppt.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2gozmldnj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2rroafaew.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2qnvnwcra.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2gujeclhy.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2qexjyrop.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2qpafjbev.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2jhxxfrzk.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2gmaytdxo.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2uftfpwhd.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2bzhjtpgp.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2phqjydya.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2dulpuoqa.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2nysdqbhd.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2byiqmwzm.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2dipabqln.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2tfxupbvp.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2xoqthgeb.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xfsdsczh.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2ykqzcwlb.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2jgztioay.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2bzusmbqj.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2bqjrcuhp.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2gtvqxqoc.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2yujcfvzr.html


<!-- 参考信息 -->