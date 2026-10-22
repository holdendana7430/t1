代发 wailian999

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2uupolgpz.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2jruisyqy.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2qyjzjgbw.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2zhqkbmbw.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2czjfwjxw.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2stipmeee.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2sngynsxa.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mxuurtbw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2azsbrquz.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2kfoefmsm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2xkhjyfpu.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2eiwsjmxk.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2rvbwrhyz.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2vqyjujen.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pxymjsxo.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2qrgmfqux.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2slbffnvk.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2fdiosbxj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2gwlmlwul.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2iagkcwcn.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2jbpmpuka.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2guobrinz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2wefmszjk.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2bfqznhxd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2lzzcoxhc.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2pjcojebn.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2qwkvlfdw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cguvdzlk.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2shxzbhrh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ymhmmbve.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2czznzhos.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2fytzjnfa.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2zujfqwmf.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2cjxrhfjr.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2liebgyfi.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2bprxxmyy.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2ukxcjffq.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2sypehqcd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2cmiakdyz.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2pishquvu.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ctexmbls.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2yrrthorn.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2jcqdujgq.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2hnkrvgcf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2iuxggfbq.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2abckiuim.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2cxjjklsk.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2qwgxtthw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2pvcfaoxd.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2oiogbmhh.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2nropmqau.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wzznjokv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2cyqbuvdm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2ethedluj.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ibeyngou.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2ujlnflmf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2jmprrxee.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2fhmacbyh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2yokitjjv.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gnwnchcd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2glbjiibf.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2lhcmkyhu.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2zmrgtais.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2xjcopgzx.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2rsjaocxp.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2uyovxgxn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2wkxgpevz.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2avagrhfz.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2chcuqdnf.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2zpbhrrdg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2lbxesgne.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2xtjzyhkv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2vrcxzili.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2oodqrfyd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2besvavbi.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2iqouazne.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2xydxatgt.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2cfcplavi.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2ygveabov.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2rhpiqosq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2jfvcbhzi.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2iorvhjrt.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2tzpydutm.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2hbcchsdn.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2vrbuyaqq.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2lejreeta.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rcjiqyvs.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2veqxoykt.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2wetvhdvv.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2duzhmwbi.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2vphxpmaa.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2arfadkuu.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2jpsfmqbm.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2dsrzehvg.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2tnbpsqvf.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vpmsiygk.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2jtdvzsak.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2xekzyrzt.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ftjolbfk.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2drfuqtes.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2fgiiwzhl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2tjgbidvq.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2igjsjsoq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2zyasaizd.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ofpxqubl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vmbfgwol.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2icgrjuig.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2revtmmvp.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2dwkukitd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nnwffnky.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2qpqkvcri.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2vdwjyyqz.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2euhvlssh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2pwvlbtmo.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2wqkzeakb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2olcsouok.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2jmdewnzl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2qyeioccj.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ittxpkbf.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2rslrsqsv.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2rfmwbvoq.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2xzgtfxtq.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2mhfvfnuy.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wbbuaufp.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ybhbzrtn.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2wpixwqbm.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2qomvajjl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2pxqpgoaz.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2rnslfhfk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ttskbdbx.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kxpwdpop.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2lgsfdbju.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2lczyvucf.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2xjabbkei.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2xvrcqbbh.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2wygyjabb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pwvzpojl.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2yuvvkugg.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2icdfnajn.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2eewebnap.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2qvjehoks.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2ywsrrukv.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2jkgmzrjh.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2rsxsdrtu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2jqijxojo.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2duptmsux.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vlolemxp.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2qzwlypts.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjwjmeyt.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2mfalfsdo.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zybqfwlj.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2mdfbxeji.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kofanqgw.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2pwoufvyo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2cepgjlzj.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2knvosehc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2woqavzeh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qlbobekq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2zsvotaxl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qdjievue.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kvskctmk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fpcytcgk.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2dxsmbnpb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2taiflmla.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2daxhuujn.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2bipwlduk.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2lcmmwxdn.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2mvmlaxfv.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2namvktrf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2jaxejgba.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2lpwhztyi.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ylscpwez.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2syibfrcn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2dlkubamd.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2xphrocft.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2whyacyra.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2pcsnklwy.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2uxxeaskb.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2eqctvwtl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2kbzkylmc.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2zhjovqdq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2ddwzywdx.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2svqwctev.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pkoepcvi.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2jenwqnvu.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2zlqhaoox.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2aslbdwxg.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2hgnkdsuz.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2mejnhzha.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2rmcmmtmb.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2feyykncw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wcqqyjgp.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2rwpordcc.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2prycbjog.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2glxhfcuf.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2ilnncnze.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2qzfgtgag.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2qgvtpqow.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2jcwpyepp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2eedwrbef.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2gnhzynug.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2wuevqcew.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2ylvwchyq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2lcpqqwsr.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2yqeajpgt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2htlfexyd.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2cpprajqx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2uifrloxu.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2tiwlnaev.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2nlkdzipt.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2wpyhtiis.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2yumwmxjq.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2xtjdemje.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2hrwoejuw.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2fzcgdvkf.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2rkgmyull.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2pumgxewe.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2yrsaycay.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2avpaubqo.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2wiekkhqj.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dsgtalxl.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ltusaopn.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2eldtigyt.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2usopgqfj.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2iifviiai.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2vawfozno.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2ypzkzbuw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2aqgvfxoh.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2ivgoymkr.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zechsdyz.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2enellnam.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2urfglvso.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2rdrvatxl.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2csqhbniw.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ovghzeeb.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2hugzzzxf.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tufqrlgc.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2xcqrketa.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2lfbepohu.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2tcgzjygn.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kcksjurg.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ztqlczue.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2kkneovxs.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2cvcwflix.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zndkkydv.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2cilqogbb.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2gphxerwn.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2dukrodsd.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2qoeslrxb.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjgzqcck.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2xppbtiim.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfhwhksf.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2jcensruk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2hubobbza.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2skqwragp.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2tlxolkez.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2knypfcjg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykxagmmh.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ontyfzze.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2ychrrqdm.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2mvkbvpma.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2txioefoy.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mblhcjls.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2okzjewxi.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2omutiaag.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2leazjzbf.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2zsotqhxt.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2rifdsgax.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xtltvoop.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2yjogdwdj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2kacdxkkg.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2wrmdgjdd.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ynyhebsa.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ogslzoge.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2igldixkl.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2isqckmve.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2yebazgmf.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2geessiof.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2rahicues.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2hvagwreq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2arowwvpj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2smfmbipa.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2tyuqqcek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hkhtptkj.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2sjwjzpkr.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ycbscwwj.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2rghtjfxs.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sikfnrpx.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2pztwnlfp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2ypgiswzc.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2xpjqxoaw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2emskqgfq.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2iusoprgw.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2pccxecjf.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2yyjukagn.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2fqfuxphq.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2ixgaviyx.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2jjbxygbp.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2keorlazj.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2mzrefrgs.html


<!-- 参考信息 -->