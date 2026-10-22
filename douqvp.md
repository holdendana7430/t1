代发 wailian999

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2pvvdlhww.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2mswwyxfg.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2pyypzuih.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2zahfhjye.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2bvgacslt.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2lciwlbip.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2ghwmqdkz.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2gxdxagby.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2fgkhrybg.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2pkwexejj.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2mxblhwiz.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2xhmeqtny.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2ncagegyg.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ghgakswb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tpvdrmpd.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2dlregkkw.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2wvbkocij.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2msvktdnk.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2sixjdhry.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2twkiasvz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2oockgwhi.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2zivktamd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2bxbofiil.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2zrlohtqw.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2kwzztnta.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2rwuatqim.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2pkuvybbz.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2hddgvpzl.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2erzgofmh.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2oeasdqza.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2jaltsbfa.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2osuyohjn.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2wlpwhmld.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2nhkagkdg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2uzwmbjbc.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2bbnpnvfj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ocstbuvm.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2fwwfuols.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2ojnezfaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iknlsipb.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2mspzytbs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xpguzkkj.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qkyafeqs.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2psptadod.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmkjjymn.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2lhrcjdzm.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2txqqgyys.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2krpaofrx.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2wopebuui.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2twnhylmx.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2nkxieswm.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2tvttzwle.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ltkuflsy.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2woyblhlq.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2kyzycutu.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2ucrwwrsm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2khkwrtki.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2kfrfgbpf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2kpgrevhd.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2dqdnhudh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2lejwfdvj.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2jmtlluks.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2qysbstbj.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2appksvjp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2otcmjatr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2sixacgat.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2engybcjb.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2fyplgyho.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2dtkgduse.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2azdtfscz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2hbeabcwb.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gnqwkjtz.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2aqvrvgax.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2qprjfuvp.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2zkrcuokx.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2pppmhwpf.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2hqxmrcuv.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2neklznvl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ttgwgskr.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2whaskcha.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2hgrrxaej.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2bihqkkhj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ectllwvv.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2oagobkuv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2vijgfouy.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2wotxecvz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2fymnyvof.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2wjpqclhm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2fnowvnhq.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2jllthueu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2valraxau.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2mcumbbdh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2ggjpfzlp.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2gstkprmf.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2avpygyra.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2dbmrfprw.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2fycqiabu.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2ptvaaurt.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2slinttez.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2ueiayeob.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2qopcyfgf.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2rkcpbegp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2elsqrotm.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2ntrjuuwi.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ctccncgs.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2tkygnrij.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2pudxosyl.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fravpfyl.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2owqtaqer.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yuithnka.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2ibazjxbz.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2soltqbho.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2uidalzpy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gevwuiay.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2sjluswul.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2kexsfbbs.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2butglvqi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zzvbpcqu.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2fqxeielp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zjeiyxhl.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2kzjaqcmk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2sdugzzjo.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2tnmomeqf.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2xwukzuam.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2sbblfvds.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2bzpgdjuf.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2hvtukukx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2ozvienvx.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2jwpzuarz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2fuoievum.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2moluwrqy.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2hwjohtxr.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2eswyncwc.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2zxpuxujv.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2jjgiapdg.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2snashqck.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2fxmcyloh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2pqiekrjh.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2nsjjgrdm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ieexujxt.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2mqvzmokb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2lnbiubdr.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qdneqysq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ysdrodbt.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ecllwqfp.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2ujromjqk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ftuodcqg.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2byglwwsr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bvuvbgdv.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2dmzoxyyn.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2ejicwlso.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2mhucwcwc.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbtityhx.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2ukfhqyzi.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2oogeunyi.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2taekuzxx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2phdlyvhh.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2mprhpqeh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gmbbxmgo.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2gdrfytks.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ucuvxele.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2qptqoubi.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2iqdxistp.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2sbisekpk.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2chxjzdey.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2ftjemiar.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2woktqyih.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2iymxqvnk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ivqrcyqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tqenmaou.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ylysuchj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eubsjjgb.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bkracwcu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wizfrzqe.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2dfxextpg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2mcqgrkqn.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2mwcjnlnd.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2dvuubytp.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2wnkwvdod.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2fffbiodu.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2cuwbjrzt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2eliakqpf.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2kpzrjipk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vdddfzjw.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ynnndbzw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2jiojnzla.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2akjxvqis.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2zqgzntiu.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2hsripxsx.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2nbadgrnt.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2oozypkjw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2nxvfpmhl.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2wpdmowci.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2efkjnvdc.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2lyjwwkby.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hlhqtujm.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2xavpptsi.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2gczzmqyz.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2pedkxiun.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2lccjdshh.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2lxluqnnf.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2zimdmkoj.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mfpscqsg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2thzfoeau.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2newwrnkt.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2pfszvsqb.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2yiralgwq.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2qcnlolyx.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2uvuhvzam.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2lzwoomaw.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2oplfxefi.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2nkpisrlp.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oyejriva.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2rwlgvzcb.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2bxaimigy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2pdxtjatv.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2aurckswd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2pjopcqxi.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2tsqtnoyf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2oewpgqig.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2jglqolhe.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2ryynfuij.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2ggvnuxce.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ruvgmlda.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2garlmixl.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2eojxlxwy.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2zofeikjf.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2dpnlmbri.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2mropkrab.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2xzizcpla.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2ynryfyga.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2swzkebll.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2htnefkmt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2adoytnky.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2wekdfleg.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2rzdxtthh.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2ovifwyvf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2rjbdiruj.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2prensbmk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2nprbzheg.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2iptzcgnd.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jhtcyjsd.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2lfpzwlhc.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2zzmcltbt.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2xgicvshv.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2ccnniwkv.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2peqbkrmj.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2smlriiuu.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2kiuijayk.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ljlteyrk.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2affofqgj.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2znppfgvz.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2buaqhnij.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2tbpswhwn.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2iisgybym.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2kgxvcdom.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hegakjzi.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2fhuobvys.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2totljzss.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2djxqzanx.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2boxfhkmf.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2fdckmewg.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2lxhkdkhb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2lwzglvdf.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2velbedhd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2kyomebml.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ztvzqomv.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2ldbapcsz.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qhoqggew.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2armtmote.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vwpqqemv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2nugcrxfq.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmtzlsjm.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zqjpxsac.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hdvphrrq.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2ssncieif.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2smwyffbn.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wvkzwngk.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ofkekidi.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2hisjhvkp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2fxeckqfg.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2qbycxsoy.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zmqlescd.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2pruhxrkw.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2hneenhst.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2rgcwyeio.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2yztxpdwh.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2omorjemt.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2pynwhgwk.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2fwpflasj.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2lwqqsdzd.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2jcjbtqcx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2lgngpylr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kwfvctjq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2bztazkfi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nufgapwq.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2xeznvznm.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2afverqkl.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2ksodgjin.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rwsawdfh.html


<!-- 参考信息 -->