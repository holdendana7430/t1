代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3biawpbdm.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3xmubjobm.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3ilcqjjxf.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3vbhzemwr.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3incbkgqv.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3cgkbhnjg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3gzoasqau.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3kdkntdwv.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3kjsmqmxu.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3zfxjrazg.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3fdyogvye.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jjueuasg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3wzwonjmf.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3miyfbdqo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3iknrvpci.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3vpxxhpng.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3teherhav.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3tbbcquxf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ehfjhwyl.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3lchrmvzf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3vonhjwuh.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ybipuowp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3wzlsazam.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3geslvpls.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3ykbqorgt.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3hdmxlxvo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3muevawlv.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3dfgqfuez.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3uzhxguyi.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3qqtkzrng.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3avxwmvrj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sqratevg.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3lubzeiwm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3glmnnemd.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ktxwtzic.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3qvisotef.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpkssiuv.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3uraunnug.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3bgrsjtcg.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3ywfsvrmy.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3wkogwepk.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3wuhxlnor.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3sjtpeonr.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3utmtfdev.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3olfscoyt.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3qkdvfyya.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3ucelmjex.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ncyyvzbt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3dzjdyome.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3qwfclvqg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3bwhuckmh.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3caxkegng.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3lfllxofy.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3yjsjkeen.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3nxxjehyd.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ikmsztis.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3kdgpichb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3dlioosqd.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3uzkfvlud.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3tnzgktdc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3tvrmaqxk.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3ougdcvyo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3pqszuqzv.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3xaexbnqa.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3jwrxftgt.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3goperkwx.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3iwfiuncb.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3ufyyzbcb.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cbldgoss.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3sehzdihp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3jnpmwmgw.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3frizzprl.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3rdjjqyaa.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3arnhtgnv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zzovwoij.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3gzsihjyt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3njnruwmr.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3uqqosuoq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3jxznghkl.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3fjqpmrev.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3nroamido.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3xnyzpjvu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3oaylcdas.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3pjemayxl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3vvqgabxg.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3kyrsndsl.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3tqajfgda.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3txyaumyi.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3fixzsour.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3dpzgatut.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vxkyomaz.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3bttkrfzj.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3ifvkwxfh.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3nbrtwspb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3bepefazy.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3wqlrmwzd.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3wezqikbk.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3jvzvlnlz.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3mcbjrgri.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dbbyopwi.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3kqfkgccc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fcydrlim.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3qnflkukn.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3iqfmonxc.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3sknzglxo.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3siqbkcil.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3twgdwhbv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3yzgixadv.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3poqcodhm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ueiamkdp.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3supeaval.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dmpjhvmf.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3vtupgwyo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vfrhwqlv.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3jzdciodh.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3dkiledgj.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3iqzobmtu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3vjrxcufj.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3ukyurgbm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3jypmlfyu.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3fnbtvbgs.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3kbhmbiwc.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3ajhtndng.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3sjlqttse.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3vofexvpq.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3slhcickd.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3arxydlov.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qngtaeuc.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3uqdiywba.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3kjzrowra.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3xojzsdtk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxcnjzoq.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ehupybti.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3ypqipyhq.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dwkfqjeg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3enkgfzry.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3zykpvtah.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3hqklymvt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3mamykvmn.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3fgpzqfhy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3brrkspdz.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3mymmjbxv.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3kwvlfyfe.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3yytotzcm.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3dvttxcuu.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3kuqzfbgw.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3jasuhxeu.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3kzbfwyvp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3gzvdwmjn.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ooifycvp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3iigahgzw.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3bayjyceg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3cqwczisn.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3btvoiikq.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3srtkpohs.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ncmdauhu.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vvfbfzow.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3ouulxemc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3ncnzhxaz.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3azspneye.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3pvzdycul.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nphcivcf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3dwepkybc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yslmmbjv.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vtxijnfh.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vjpxbdpf.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ikcyzzlo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3viqeyxsh.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3mjhofxfd.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3mdchdwdu.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3tcxzebhv.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3yyzfzwzd.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3akxpxajc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3umvkvlvp.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3xinmcdso.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3egtyzncw.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3oektdsub.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3zzkgeyhu.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3vdhxnuqr.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3rhpdidsm.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3bsqkhefd.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3nxuwonvh.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3arhqnlqw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3bfpyzefq.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3buyjlhmw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3ssrmznud.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3gfxjixdv.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fuivzdpp.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3cbqdsbva.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3icqpzefz.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3ybdegizi.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3mfdubobz.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3yuxtyqeu.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3gqgjjvcy.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jmytqsit.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hvgxwbky.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3ihauyvqq.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3jkjtinug.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3cyynimyt.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3dkjiqrsp.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3bqmqbumr.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3bmsbkthl.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3zoqwsvxh.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3lgjovqdx.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lojxobty.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3amvxrnfa.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3qczkeuoq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3opzoapkw.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3jnclqxpf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3psbfgnkl.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3bpwcllqq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3kujpjhcv.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3brtgejvm.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3ntnpccrz.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3mhwdgjsh.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3jruswvyy.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ydtcthmt.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3idpvkydz.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3uqtzteln.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3ufmdqzvo.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ojxobsjh.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3lxafwuaq.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3fzgctfqs.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3rughtzpc.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qwfimzxr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ljkoudoy.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ppsuemta.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3xfmqrmzm.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3yjlyoykj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3ddlaymmv.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3cwvvhcrq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3rvoolbxv.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3ugoejubi.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3bihiamil.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3hftueyha.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3lqouogtp.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3auxiyvza.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3cinedxqv.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3soxflyxb.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3enjqswrp.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dnccjpwn.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3aqwczqxi.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3dqxsmhod.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3ajoisyoa.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rojloasy.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3tuehiyar.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3rkbpoalu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3mhkhawdf.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3sfjiuzhq.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3emxopdnz.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3fydmwrqa.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vavchgly.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jtwsapzl.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3okomelcp.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3ptmqydla.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hamhguby.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3tlyscpjk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zdbyqsnp.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3mtnibqcm.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3unufutdi.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3rxjzzmmy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3yreokshn.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vnwjnnks.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3cpndheku.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3itjbippj.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fweloynr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hjyvftak.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3ojnuaprh.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3tfpqirgv.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jxlymarz.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3psdddjiu.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3bkubqlye.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3iitknyja.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dtmpdeoh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kcnpwlro.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3vpqdxkfj.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3fbgeifya.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3itfritco.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3esrgfxaa.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3ylmprvar.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3nbsrhvpk.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3plmrbqvf.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3gydttkmo.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3gozbgnle.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3yofoyxbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3amjfyiki.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3edeqenkp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uctlgvuj.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3nsvcfxmo.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3ocytxdfl.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3ccgvbzwe.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3iyhvrtft.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3yhqjpiup.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3kuoanrzl.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3lymftdfq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3vzywixay.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3atfmoknc.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3sgiryubn.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3gkqhgyrm.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3upasvgtf.html


<!-- 参考信息 -->