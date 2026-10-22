代发 wailian999

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2ekewbfds.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2ysidvuol.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vhodecbe.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2jrfdoghv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2mvrtdvfe.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2bfwosljk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2vlelkkse.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2pasixwij.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2zadtxuxy.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2wvsfktgc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2chhfgawn.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2dsxetorl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2qtgdrblt.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2nnpzvgiu.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2ustezycz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qchgxbiu.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2yyjezgxy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kaqrmujk.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2voasfwut.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2kqewayhh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2ucbwtctr.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2gsqxigis.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2muqxnmps.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2weifcxmf.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2xcbnyoes.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2asacvabi.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2izqrtrps.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2gsuliocl.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2byidlcnu.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ktirktuz.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2odmmyhdt.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2nagdbqqv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2bynsoqst.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2nqzdchai.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2jsyxqmgf.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2qbxyllfb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2cdbyutwa.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2njxcijlj.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2cysgntgr.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2muhwldse.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2rdpzyecm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vqnprvid.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2xxcomxdl.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ehkicqcd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2xjtbuwsf.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2lcoftghg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2gmxgyver.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2hxtxhqyv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2fpmgjujb.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2xuxrirlc.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2gulystdg.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2kofzorku.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2dqofssxz.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2hoehikrj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2ccymrtvb.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2xolwqoyc.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2nfklclfr.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2thlcicqr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2esfhlxft.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2xhnoiuaq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2etorcpgf.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2lzurynmi.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2wbjvvmtg.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2bniyuyyk.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2oemyenky.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2xexggqhu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ydoyqlts.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2bcxbtjrb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2iqtrthyv.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2gfurbcak.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2quonifuj.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2tdotrqkk.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2leknbxty.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2ilxgyldf.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xyajcrua.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2mcntrwvo.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ztuxqzac.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2tsthndus.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2vflxcxgh.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2vbsonoxd.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2dxvmxuzw.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2cvrpobwb.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ftvhsnqm.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vktmrmpf.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2nyhcfjkw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2viyeyozj.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2brknvudv.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2qklocfho.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2wlqtiwul.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2pcrbmjpz.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2jasimcad.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2isevtrad.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ovnshgnr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zhbvcnla.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2kdifvbtl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2udgpemsk.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2gvqcpmwb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2myanbszn.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2kbaojapv.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ainwmyxj.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2cbvfkzsp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2sdmitbgk.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2iaqsozqk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2kriyxfjb.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2asrdosmz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2euvcaixb.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2fmypdnsy.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2vfreihgb.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2hvljpfjq.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2ygwqlinh.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2dbbddfdz.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2mvxwjdqz.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2alpznbtm.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2qgstkvld.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2vpmirqso.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2zvfdcxnk.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pomvkddr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2hlrgwyqo.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jbbfkskd.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ycvuvrfq.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2kqvgzsqc.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2kgukzdqb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2imupbesi.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2wceatfmh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fiwaybel.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2yttmwdpe.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2shhyahce.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2pvgfdgsc.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2xqsyxpcr.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2ojzyvafx.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2slfyflpq.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2hfwxerkt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2mvnehqhk.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2xegsjchy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ypatorzo.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2bkuzxdvm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2rcancdlj.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2psmmfkqr.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2karrxqbb.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2hamhbmoy.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2lvgmahzs.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2wralyqio.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2fjwxbhjp.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2wqacfqum.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2tfkvcwia.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xarjtaae.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2fhfcfjsy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ntzmlkhf.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qnkccsft.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2yupcueuj.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2khyjebnn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2smxsrnpy.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2kjmyppzc.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2efgwpyvx.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2xgfsdqyv.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2kcwictfj.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2lkuibpdd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2ggoqfeau.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2cdwctffd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2oczmkoxl.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2dtjswogl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2iumfvggm.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2yigdxfcf.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2orcrigor.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2mzlsodmb.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2vgxtoewp.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2pklaxnon.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2nnoalrlf.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2sspyzqil.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2mxuqvffq.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2gnrdmsdr.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jtaxbuow.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2kyvcsiea.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2yfzkxcuw.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2sqkmkxpi.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ajwzzxmx.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2zhgcpmfo.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2crcodkzc.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2oqbuhujv.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ewxytyaf.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2ctjpearc.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2eoxeqkcc.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ubnbdcoi.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2jdptsnuz.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2hbpzanni.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ynermygj.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2lcparuno.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2iktsvbqi.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2tciybxsz.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2wrnjnswk.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2gssoccoy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2beexyuqf.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ntvhcjus.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2lmcijesf.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2zshuwups.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xroccjob.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2beyqpaha.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2zkkzduus.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2vzujnhrq.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2wyykjovz.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2whpvbjrq.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2zzljyrzk.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lkneyqck.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2etbpmuid.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2jvdxbwyh.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2nlipytve.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2pjrkenlu.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2hdksrpgn.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2sqcnghju.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2iqnydzzo.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2skahscny.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2upuoueqo.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2qhsdahtq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2rlmgrhar.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2idynltqz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2okqwqssr.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2jfzrfqls.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2hueokoew.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2dkwfulmj.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2xwudazbo.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2yrzvbren.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2ihuucvml.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2hgluobom.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2sgxqatth.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2llepmyoi.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2rmxugypn.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2isqtxqta.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2nohviyvl.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bwothvwr.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2cgosluso.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2zuslntwz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2uhuvpdfh.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2xermoqtk.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2tnekpsgo.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2khukxzjo.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2lwjjxkdq.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2ivwdivku.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2tgfaqxws.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2wwvobpck.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rpbyrgry.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2elwjpbew.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2oxxurvji.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2qadwgxyd.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2heepdjas.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2rnvporbs.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ngejcmvr.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hafaggtt.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2ekrhbzkm.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2zplpzjoh.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2adyhznsq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2oupmczyp.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2qiohqouf.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qlvgzbad.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2nhrzhbqi.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2tmuyencj.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2jncxxtod.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2yanrgjuk.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2npeubfir.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2scorflhf.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2pxxgnxge.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2xjtpmrqq.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2vuslqckb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2iirhyjqq.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2ykexkurw.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2khhberel.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2sljynzmp.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2llyxkkrv.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2vceflpcz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2qhlstbkz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2roxkcvls.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rgroycma.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sllufvdx.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2yfwcfatm.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2whrdhobb.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2zcvxfroq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ilykqjus.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2oxfmjaoc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2kwbvjnsi.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2caejlcvz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2thktvzqm.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2jyhtqdrx.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rkhcddha.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2zrewbeun.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2niqufayx.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2bhvcekad.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2pkumjfhl.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2yncgcvkz.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2ipcvxydg.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2tnoaprpe.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2oywjppag.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2wmdesrct.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2opwckgru.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2damodzjs.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2tpoteqku.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2oukcoenm.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hwlnjycv.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2vmpkftaq.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2utolegbf.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2qslgaglk.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2sahecgme.html


<!-- 参考信息 -->