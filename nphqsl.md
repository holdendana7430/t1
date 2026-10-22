代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2zxrjijfy.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ywoftozr.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2yrdatrcp.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2fehpxpyh.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2igsisosu.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2yaebgzwy.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ifgtvixv.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2kgocmvqu.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2nbgeuuij.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2mumasnxp.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2ilxulgrw.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2sdbvhvrr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2uoefgbbs.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2txizbuyq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2qdnsqrhn.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2oforqmhv.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2diirwqwd.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2vwqplpwb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2vwrxfqgd.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2gvicjdhw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2oqhzmvmc.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2solspoas.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2owvnqyuy.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2gklwtwlb.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2kxemmxrw.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2gtxvxryr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2limvnujt.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2mqdsylaf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2admxzfka.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2negsmstw.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2mwyatobm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gwjnrbrn.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2pyddijwr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qcvyqpre.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yanffqyz.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2zrptgncr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2gndoxrxy.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2diujjqwy.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2dwmiyttn.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2xxoipgmj.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2pczgzvkz.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2lrsfxyyy.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2clxckezp.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2mihymchc.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uvmexunj.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2cnjuwexd.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2pcwptghl.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2qgnoadps.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2mzlksivt.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2lquyivwq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2jcemlxwy.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2xhwylbgq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2axrxqfkz.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2ptdetmtl.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2wyjdddvw.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2aawtqcpp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2eztfofnh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2aiounipm.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2dhfaddsk.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2yptzqyhr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2taducxbb.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2sdgsayil.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2pqbjzkcp.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2knrxnbmb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2axlnxpol.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2keigoefa.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2dwftzpln.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2xzoaziau.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vaovckwp.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2fhsfudpz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2zwfblqep.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2hmdmgoed.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ymiqkskz.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2hjwiujbe.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2lmccsulk.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2tjnaefhn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2mcvsyiwy.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2uzunwshi.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2gvxhjlyd.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2blmgfxsf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2fnxhsbsn.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2cvxjoaua.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2kctvxahz.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2hgkjvsac.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2yugndvgh.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2zkmhycxz.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2jlepdwcn.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2rxxplchu.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2fcbljryo.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2vrwjzqpk.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2necdrosh.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2ssxtwzmz.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2afxsiyen.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2lxfrbshc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2hykkggde.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2urkajtrk.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2jgnypcpq.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2wjssxpfz.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ycrxhuzd.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2euntglcm.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2ihscrgvb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dgicptuz.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2cjplftvc.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2wwbkhnca.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2qvyggidv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qgqqadqv.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2rzwfqaek.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2fznpfkkn.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2zgbhvlrx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ftnnsrvv.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2qmwoxyap.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gzhodrlc.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2jlxzxdav.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ibfbpifu.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2xyxnbweq.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2zuazlnlg.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2jaoihrln.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2acdqzwuy.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2yvlnfnub.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2znfoohlz.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2lpayyjwp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2eblhtuwh.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2qkbjrzsh.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2avehwfgz.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2xpubtkmo.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2yzqhnmoj.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2isyxdiok.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2kaknpdcm.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2kkcwblqd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2xqyrxnzg.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2ubrwbiey.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2pjnkkjvy.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ihyhwdyu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2qcxbnqjr.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gcxcvvki.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2eyzghdtn.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2lembqsjm.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2lbwalagm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ezbrreqw.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2cgwrlvsz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wxfybzgr.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2jrcgioyc.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2xpbxfbbe.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2arbclhch.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2vrpzvdhe.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2vziwqazp.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2plhyzkeh.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2einozuar.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2zvyhnbgb.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2hxlhadfp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2ggiflddc.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2dtjdtnct.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2ddzhjpiy.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2vkhzezom.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ubtjofae.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2srslnssq.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vsitphqf.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2wqdwxayt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2ifcnqmcw.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2jldxjjym.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2nicznfgg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iatuvrjg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ksjlfjkt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dzgsfoyo.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sgsokqgd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wjzjwnpa.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2dvwuucnh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2gilctkzk.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2hkienmdv.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2zmxtlrrx.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2ftgkzhcx.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2suhjyayj.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2gtgkgvmt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2uohgvkkv.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2gwfvubwe.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bizoacen.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gcsyufkh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2uxheopai.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2apdnmfih.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2aonoglsu.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2ishwzriz.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2brxzimfj.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2xgtbvrrv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2zupazzum.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2bmqqgvam.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2qvankaaa.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2opevvdoh.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tchfuriz.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2xchvhpbl.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wefbcctr.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2qvhvqyoq.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2guczfike.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2klswbxtx.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2sfgjwmuu.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mlavvuaf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2crratldj.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2scckiqak.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2yjdqhmtj.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mphslvzc.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2aqymrqvt.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2nfbsvaob.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2ttcwtmlq.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2bvwraxnq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2qixujhhk.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2zozbxkio.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2yrupongx.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2kfdqpoqh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2feevlexx.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2dmmrftri.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2emozuvwv.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2lcwjdmfh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2oxamlfsl.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2geznczjz.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2xgijzoch.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2vtuhjtqz.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2suiczjjg.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2cdzkejux.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2avuvtgvv.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2gratnifx.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2ivpzktdj.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2jewwcwjg.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2ywlltbsq.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2dmmkcigv.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2bcntlcfc.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pkralfny.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2kgbzmypl.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2oopxzkkm.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2afefaysh.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2xlqnxbmr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2wmwflfcl.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2ffyggvic.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2uzvzrwdi.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2vhftqmlv.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2bgabdxeo.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2csurjpgm.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2xrzuntkb.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ckefeaxm.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2pofvuncc.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2qkuecwez.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2hckgtpgi.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2altettoq.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2loendakg.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2tbxgqcpk.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2snxljqtw.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2eejlfewq.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2imwheyvm.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ricfuswm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2fptjjvgj.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2npqfltgj.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2ptbqchbb.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2mwbdsbli.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghkcikrs.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2byawgtyb.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2ziybhdkz.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2qjoilxfu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2hfbzuvet.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2lzwspfdg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2ruruflsw.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2llpswaam.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2twjidfzp.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2fhoogdwn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2nvrgbjah.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dyntyoyv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2ctrollbw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2leeyttyp.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2eipoiwln.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ftdohniv.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2lrryrxmy.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2ewcqmker.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2rxsgmbaw.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2vgxdsyeh.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2dfaxrcxc.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2iqtvmxbo.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2pecwgfdq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2sizjhfqc.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2cqaemhep.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2xyonxbnp.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2mjceidky.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2bnynfzea.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2mpaezows.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2fpdtmlnz.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ibicjdvm.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2wdcouqbm.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2lfnaetqf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2krnzphan.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ubvellrw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2yxbhntit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uhauhhad.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2sjechcln.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2nqvyvufe.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2znynyidg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2edgnnzez.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2nledatre.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2gzdkhmeh.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2hevscjit.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ruggrork.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ggrhtwth.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ctjbuwcf.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2ardaurpq.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2eldtuobs.html


<!-- 参考信息 -->