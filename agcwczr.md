代发 wailian999

openssl rand -hex 16
来源：http://read.share.hesvh.cn/Article/details/galaeovgp.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gzkbjwzga.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/gdpvqwmlm.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/ggaxoazpa.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/gnjtwphdn.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gworykorb.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.zdbjq.cn/Article/details/gbjgqcdds.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gcsucjiok.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.zdbjq.cn/Article/details/gmymolngn.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/gclyskuut.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gtmokpgmu.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gmwrczpds.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gvmqiktrx.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gcxitdcnl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fehbvm.com/Article/details/gytnuacar.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/gatrpwkur.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gdyvycvda.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/gddrijokm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gllcnvies.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/gkqzhkxiz.sHtML

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/grxgkgwxr.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/gmgnarwkg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gocafalyu.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gdfwwkuxo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fehbvm.com/Article/details/grrcgiwae.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gakcrhhep.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/gmtvqbnla.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnptmnzbb.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/gdmbseqqk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gthltehck.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gsdadfjnw.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/gayqsbfdf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/gkdpqczkp.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gddplfewj.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/gckkrpqzm.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/gzmpddzfm.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/gxyleqxhr.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/gtsqagkqm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/gguyggdpw.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/gvrwmtgrr.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/grdfqdtrw.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/grkrcgchz.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/gpiyafjjb.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gofsaiaut.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gkmqjvmeu.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/gteziftxo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gdvjbfqgv.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/gjyvstfja.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gvvugczsh.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/gfnpytymb.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/gfohgkjvi.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gjknishda.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/gxjtjqaqv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/gxauxojnz.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gelcggkzz.sHtML

[S12] C：写文件
来源：http://3g.hesvh.cn/Article/details/ghrqnjpbn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gieshlunz.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/giehwctsz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/gntiwqcwm.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gcizsidnx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.zdbjq.cn/Article/details/gdaglovrb.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/gcenbphez.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/gagidftkp.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gncryzrwh.sHtML

x |= (1 << 3);
来源：http://www.blog.zdbjq.cn/Article/details/gwrymrdem.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gnpizhfrm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/gybrjfcaf.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/gmjixjgwx.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gymvrelne.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/gmscdvqtf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/goiddzkdv.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/gvvrgqxlb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/giqqpuuhz.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gtnnqjxqx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/guyclljjj.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gezdhkato.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/gzamjxwho.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/glximdbou.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/gevescpkc.sHtML

[S24] C：获取本地时间
来源：http://www.blog.hesvh.cn/Article/details/gqmirjnfe.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gudnmjdrv.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/gzujwsnzy.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/ghafywycv.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/glkgwvoxh.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/gvjjlammo.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/gsobnctkm.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gwxdaodzv.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/gmoawictk.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/ghrkvgyao.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/gidifrtut.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/gsxtwjonp.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gjpdyrmsb.sHtML

#ifndef X_H
来源：http://www.m.share.fehbvm.com/Article/details/gppvlpibr.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/gonypkdzs.sHtML

#endif
来源：http://3g.zdbjq.cn/Article/details/guexpryst.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/gcrxdefan.sHtML

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/gyidfweim.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/gzmstkldf.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/gdkisjgjp.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gdhucvrlp.sHtML

[S33] C++：vector 增删
来源：http://www.blog.hesvh.cn/Article/details/gmwpdqqip.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gqbijwtgt.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/glinacrun.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/gnezfwpsd.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/gjkrsbxen.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gfsndagwp.sHtML

[S36] C++：unordered_map
来源：http://www.blog.zdbjq.cn/Article/details/gfzxojehw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/guzvpautq.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/gghqdpfpr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/gqezmoedb.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/ghqtpgqox.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gzdskkfow.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/gzsmujsjw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/ghlzezkwg.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/getihdxfv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fehbvm.com/Article/details/gbqrbqktk.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/gsfhdjyby.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.zdbjq.cn/Article/details/gbrpxanjj.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/gnhcmmjps.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/gtmzzolyr.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/gsnmugkjz.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/gajwrzgpz.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gkgkvdjkr.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkctcaxft.sHtML

[S45] C++：lambda
来源：http://baike.fehbvm.com/Article/details/glhcpgmof.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/glgmmmhsi.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/giqdpgqme.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/gpqvbqejj.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/gjwmcnomp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/gjrrkcevb.sHtML

[S48] C++：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/giodclzqq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/gkzpnodox.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gvmywafxy.sHtML

[S49] C++：写文件
来源：http://wap.zdbjq.cn/Article/details/ghecqmxys.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/gdijwmlvg.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/gsdgfnpah.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/goyxpvqld.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gnotaskik.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/grzinyjcq.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/gnvjgnxtx.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.zdbjq.cn/Article/details/gfaatqkkl.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gugjrszyj.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gydyrpftc.sHtML

[S54] C++：异常处理
来源：http://www.blog.hesvh.cn/Article/details/godocpobo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/ggliqnono.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/gosyngzek.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/geiwdwnui.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/glifctdlr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/gpyifdooy.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/gggqzjmta.sHtML

constexpr int N = 10;
来源：http://read.share.hesvh.cn/Article/details/gjwecdfho.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/gyccxhnno.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/guirvnlwn.sHtML

[S59] C++：静态断言
来源：http://mobile.hesvh.cn/Article/details/gmslfmtnw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.hesvh.cn/Article/details/gmtlznkzo.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/goepuaomk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.hesvh.cn/Article/details/gxpiyryyr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpkfscehn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/godwbfkui.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gldedwgaj.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/gqgkzhrik.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/ghrqsadja.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gorrjwiui.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/gullnqtjy.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/gnerxlcnm.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gwkjtvlrq.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gfbvhebxs.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/gtuwnxwgv.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/gpenihyzw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/goxkebfod.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/grsapbyzm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gjbznkefw.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gsqfokptq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.zdbjq.cn/Article/details/gwzsropyd.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gpjbekudv.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gywinlhcu.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/gxrquczkd.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/gzqapuebi.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/gtdikdphr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gfbdnzczj.sHtML

[T11] Kotlin：协程
来源：http://blog.zdbjq.cn/Article/details/gwhqvvtpk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/gntxnapok.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/gpfjqwkgg.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/gxvunpoaz.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fehbvm.com/Article/details/gequuidgy.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/gtdtjinwg.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gkhwnriin.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gqozbxadi.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/gwhobzmdz.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.hesvh.cn/Article/details/gvvzdrpdx.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/gwpnvxfbi.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gtfgewpux.sHtML

[T17] Swift：变量与常量
来源：http://baike.zdbjq.cn/Article/details/gmrvwejlj.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/grpzisyqy.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gbustcomb.sHtML

"值: \(b)"
来源：http://www.blog.zdbjq.cn/Article/details/gzoxwqyev.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/grtywzfwz.sHtML

if let n = opt { print(n) }
来源：http://baike.fehbvm.com/Article/details/gpvsgoeve.sHtML

[T20] Swift：数组操作
来源：http://www.share.fehbvm.com/Article/details/gyvdxoymt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gmrlvlbeu.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/giuixxvnx.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/gfihogawh.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/gfytjjydu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/gpgykxpve.sHtML

[T23] Swift：函数
来源：http://wap.zdbjq.cn/Article/details/gtfhrqctn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/gpcvknmvb.sHtML

[T24] Swift：闭包
来源：http://www.blog.zdbjq.cn/Article/details/gdrhelemt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gfrjarsov.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/geyywfsle.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/gwxyrqdmc.sHtML

[T26] Swift：类与重写
来源：http://blog.fehbvm.com/Article/details/grjvgrqoo.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/grdffcvrx.sHtML

[T27] Swift：错误处理
来源：http://m.share.fehbvm.com/Article/details/guhofxokg.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.hesvh.cn/Article/details/gmynfeuki.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/gulzfdfmy.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/gkwrmkvbd.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.zdbjq.cn/Article/details/gwdaolmlj.sHtML

guard let x = opt else { return }
来源：http://www.blog.hesvh.cn/Article/details/gjwaswnmb.sHtML

[T30] Swift：协议
来源：http://read.share.zdbjq.cn/Article/details/gwmyhgkhg.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.zdbjq.cn/Article/details/gqphyhzlk.sHtML

[T31] Lua：Hello World
来源：http://blog.zdbjq.cn/Article/details/gyqkwiekv.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gsavsbnuc.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/gnvqiywoy.sHtML

local a = 1
来源：http://blog.hesvh.cn/Article/details/gypykwllj.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/gmvmxagez.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/gbgfyqkpl.sHtML

[T34] Lua：遍历表
来源：http://www.share.hesvh.cn/Article/details/gnokrosxy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fehbvm.com/Article/details/gywmgnrss.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/gxtfjblhp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/ghokfhiae.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/gyubmuqwh.sHtML

function add(a, b) return a + b end
来源：http://read.share.fehbvm.com/Article/details/gjuwagkaj.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/grukzobov.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/gxqnecjtc.sHtML

[T38] Lua：条件
来源：http://www.share.zdbjq.cn/Article/details/gbyiamqtd.sHtML

if x > 0 then print("正") end
来源：http://baike.zdbjq.cn/Article/details/ginoexyxk.sHtML

[T39] Lua：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gnrldidys.sHtML

string.find(s, "%d+")
来源：http://3g.fehbvm.com/Article/details/geqkkqrpn.sHtML

[T40] Lua：元表
来源：http://blog.fehbvm.com/Article/details/gruthnyuv.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.zdbjq.cn/Article/details/gsrxifrto.sHtML

[T41] Perl：Hello World
来源：http://3g.hesvh.cn/Article/details/gtdpnfude.sHtML

print "Hello\n";
来源：http://read.share.hesvh.cn/Article/details/ggdfuydiy.sHtML

[T42] Perl：变量类型
来源：http://www.share.hesvh.cn/Article/details/gpupbatsz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/gyorllkxf.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gnonofeba.sHtML

"值: $a"
来源：http://m.share.zdbjq.cn/Article/details/gezrlujaw.sHtML

[T44] Perl：条件
来源：http://read.share.hesvh.cn/Article/details/gzlmtiaza.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/gwfkylldy.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.hesvh.cn/Article/details/grmdfjujl.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/gvxcavsdb.sHtML

[T46] Perl：哈希操作
来源：http://m.share.zdbjq.cn/Article/details/gelafnuux.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fehbvm.com/Article/details/gupnfrphi.sHtML

[T47] Perl：正则捕获
来源：http://blog.fehbvm.com/Article/details/gzlagwuvr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.zdbjq.cn/Article/details/gthnrmjci.sHtML

[T48] Perl：正则替换
来源：http://mobile.hesvh.cn/Article/details/gwfwiafgo.sHtML

$s =~ s/old/new/g;
来源：http://read.share.hesvh.cn/Article/details/gdlrntfnc.sHtML

[T49] Perl：函数
来源：http://baike.fehbvm.com/Article/details/gqidjlrxy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/govnluzgb.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gtgjpgend.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.hesvh.cn/Article/details/gnodolwgy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaauvicsg.sHtML

[T51] Scala：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gkglurran.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gmaskoqeh.sHtML

[T52] Scala：变量
来源：http://mobile.fehbvm.com/Article/details/gtuzqwuop.sHtML

val a = 1;  var b = 2
来源：http://wap.fehbvm.com/Article/details/gckzfdtal.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/glnvswago.sHtML

s"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gyzuxcicb.sHtML

[T54] Scala：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gneobxoou.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.hesvh.cn/Article/details/gkhhrenvm.sHtML

[T55] Scala：集合过滤
来源：http://baike.fehbvm.com/Article/details/gwtxrfrui.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/gfadrsogj.sHtML

[T56] Scala：样例类
来源：http://m.share.zdbjq.cn/Article/details/gdtyqkhzf.sHtML

case class User(name: String, age: Int)
来源：http://wap.fehbvm.com/Article/details/givxvbzxe.sHtML

[T57] Scala：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gzwnvehpl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gdntiauit.sHtML

[T58] Scala：函数定义
来源：http://www.blog.zdbjq.cn/Article/details/gxmrhsymz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.hesvh.cn/Article/details/gzpyctmgl.sHtML

[T59] Scala：循环
来源：http://www.share.zdbjq.cn/Article/details/glfnodxiu.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gkueriqkh.sHtML

[T60] Scala：折叠
来源：http://www.share.fehbvm.com/Article/details/galfavvbv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.zdbjq.cn/Article/details/gceaxphll.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvjljsmra.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gcdgpromu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gstlgujvg.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fehbvm.com/Article/details/gqykqzaku.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/goquaydha.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.zdbjq.cn/Article/details/gvzzzdykn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.zdbjq.cn/Article/details/grftuaiqo.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/gnbvmuypx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fehbvm.com/Article/details/guzpxhlgx.sHtML

[U04] Py：变量调试打印
来源：http://3g.hesvh.cn/Article/details/gasxwfaej.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.hesvh.cn/Article/details/glupkgryz.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.zdbjq.cn/Article/details/gdnumzzmj.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gxsrklqnf.sHtML

[U06] Py：合并两个字典
来源：http://blog.zdbjq.cn/Article/details/gppnaaoki.sHtML

{**a, **b}
来源：http://read.share.zdbjq.cn/Article/details/gnbwlidpx.sHtML

[U07] Py：反转字典键值
来源：http://3g.zdbjq.cn/Article/details/gwiidevsc.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fehbvm.com/Article/details/grewzzobn.sHtML

[U08] Py：展平二维列表
来源：http://wap.hesvh.cn/Article/details/gfadriskb.sHtML

[y for x in nested for y in x]
来源：http://read.share.hesvh.cn/Article/details/gsbawlzeu.sHtML


<!-- 参考信息 -->