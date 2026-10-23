代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3kcrrxopi.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3tsjecxlq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3yjahormv.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3hezlbwjk.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3sxgeubar.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3vewlyvtl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3nexhwiry.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3nyliwrya.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3tpoujgrc.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3pfzjzqof.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3tdbrmbvi.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3kfxwbkxz.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3aerlefsy.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3vmerhlms.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3qezozwgr.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3phbbypwa.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3gjrwdgiv.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3dupwcxoe.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3rmrbnssw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3drwxnmsy.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3kpocnygf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ydfbqqox.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pzkwucro.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3hlbxnkrq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqgyovuu.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3lyjdwezi.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3czvqjcly.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3opqxoyxl.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3sorciipr.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3gmqlbdrm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3ilnephko.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3annqivib.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qsozhsog.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3syresppa.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3ltjowzta.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3nyuytkga.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3mwyfpkyl.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3kbckgvmf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3qcayjjqg.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3npttztxa.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3uikegpng.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3vltycxzh.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3xdcsizwx.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3subkiuvo.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3qaloqaxl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3nticpqae.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3mzsmwolc.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3finzymtl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3xjkzreoj.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3konhexgo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3xusirybh.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fxjbencf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3rnvhxxrr.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3iztejzoe.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3zcrwdyto.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3ahrgfnks.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3laxljutr.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kbbfbqcr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3psvgphxd.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3xehyizmw.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3sctlttlx.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3jjnjlqsu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3xnhkxkhz.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3wjtqsgks.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3dbkprdho.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3xhtactxo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3bqghmvjh.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3mwleohsd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3ccfmclku.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3zfyxbkdi.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3rlnelesq.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3bbckzjhn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3szzhblte.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3feldpnyy.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3hchjiazk.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3zuxzungc.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3mdgwlhst.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3gbdklqgd.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gawrzdhz.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3gizgzrtn.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3zwchksxn.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3jaoxbctr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ngmffexq.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3sqkdgstz.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3xiwalhzu.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3btmoptqg.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3puddhbof.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gbjkdbzs.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3buqaaqej.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwzodquf.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vlpdhjib.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3wrlcejze.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3aofnzzmv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zxkfkomh.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3hwdfnmga.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwowntct.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3nfgqetmi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yxizauax.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3zfkbarxn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mzjvhxiq.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3mthqogki.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3retdhzjy.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3vkoflykn.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3cmvdgwuh.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3wdmgvmse.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3qhepyhmx.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3bmjefopq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ouonowxc.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ggpbwnjh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3bquekles.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3itkdried.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3mnletipa.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3gnvpejdo.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3scvdqjzk.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3aedmzytw.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjmcpzwz.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3vtuaoiuy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3jesozbza.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3itzdkztq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cniqflgu.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3bhxcinye.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3fmcwuuoc.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kbzbzegk.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3dstgpamx.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3kjvogjpo.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3mhqdbmbr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ulksjtxd.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3vhqymyyf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tyhatqdf.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3oqvapxie.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3yakgisjv.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3zlrolqaf.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3yuodmtdr.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3bfojzdfu.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3jrbwobxk.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3cdnddnzq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3tryurmbx.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ogphbwdm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3griybrvl.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3ywicannm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ucvuivtj.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3ppropznm.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3hmmgvzvd.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3ykeusbzr.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3byueowkg.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3yfqkchbf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3awnhcvnj.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3gseeuyqf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3crmaubac.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ytybzjwp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3kwhllwvg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jfbmmspr.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3iwngbdaz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mgghkibo.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3sxcmwsgd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3gmklxinm.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3ogjjawqt.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3luhymzcp.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3lqqpsqxt.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3wvwkfirg.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3pdukfbrd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3zeyitdbr.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3lghauzcu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tdrnxace.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lqsnjjxc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3wotlbqfg.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3jqygoesq.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ptuwysyo.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3ppgqfchn.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3bnipccli.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3pjuiodhb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3narnijqk.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3tiasulqb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3uzjtcsam.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3asvzpqyf.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3sdwixuac.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3vzdarxnh.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3itursmkz.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3uypzcjdb.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ikoolgwc.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3wmermpah.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3rzijcfvg.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cqcbuckz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3efqojmfe.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3mqxwbzvt.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3yibtcowp.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3pqlijvys.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3lfutgohn.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3sgqavgmg.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3gjkfyjvj.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3xoubyivj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3fgqoetaq.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3tasuookx.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3giknwjvo.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3kqkmmwzh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3knhrecjd.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3mnchexej.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3uosnezna.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3tcdkyuqn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3rxqvxwoj.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3msmyvlxc.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3gkkmdorg.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3prqghwux.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3llidemmi.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3qbbcaehi.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3clwvjkxj.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3hnhsaxqd.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3btoqmfeu.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3izplqdcz.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3nchmdtng.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3gxwcuxih.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3xukjedhd.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3smziobjz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ypsnbnks.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3jbharyvi.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ipnoimuq.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3aqkougwf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3xixzpxkc.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3joygbmfl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3zkdopdxt.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3fsikixvz.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3vyefhbwj.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3nedbhkrl.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3afmvxgmf.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3vkstfvqf.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3rfminzqh.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3qyyolzqs.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3bmrtsdpt.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ujurftbm.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3dbxfbili.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3vorxdcww.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3zttsxrfd.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ordvbmuy.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3jfwlyeqf.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ftpjdzvf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3hrvzifjn.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rongvhdt.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3kzhungcs.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3mzkaqhcf.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3fvenitxb.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3qplwhpzh.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3irtjizyg.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3nxmhwaxg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnpvfiby.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3twdpwwuu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ipfawvwk.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3wqxnjqln.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3xxyofmjd.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3lypzeiwu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3umlitgem.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3yuhghxys.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3geplawjf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ozfgboib.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hjhmvngw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xfnjjvac.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3ulecymhh.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3allncgep.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ooejpvcd.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3yxwkqjiz.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3zshflmil.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3tmxhyxcs.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ntsdtldg.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pefeydit.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3phblcnxs.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3sdfcsnlv.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3thwjmlgx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3tkbabnxi.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3vgnktije.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3qxhrgmnh.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ctkztyjp.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3vvamhuzm.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3pcaxzvjq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3xkssigpc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3upzaomni.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ocunstrw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ggvdhvyf.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3qzngmybw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3rvpnxpuu.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3mtuhbpxg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3rqaqykbd.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3nqetxvjm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3wdihlonu.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3cdqckrcz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3gimxqlit.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3grtqzhgj.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3illsiqiu.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3hrgoqvtl.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3tdpklfxm.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3tboiqssx.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3mburezlq.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3zwkdnghv.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3ymqhkfhx.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3bprwdspt.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3zrwertts.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3hkirwqzs.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3zprjmzwm.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3yctescpq.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3auxjxage.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3oaywwlwb.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3tpmmrqqq.html


<!-- 参考信息 -->