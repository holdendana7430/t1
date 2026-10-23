代发 wailian999

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3vogcqrxb.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3bggixxji.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3dkaezpeg.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3hjusvunt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3gfjerxaw.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3jvhbkbuf.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3actbvgtt.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3ulwjlfjc.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3dfxkdugk.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3bfouhzuo.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vrifrfob.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3yicwuqkm.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3ahmnztmy.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3jtfjfpcm.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3xbyrarqn.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3pgcyiwuo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3sugleila.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3ufwekcaw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3iudhwfia.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3ruwfpxgy.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3rkmtodtb.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3heedhhti.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3ewbdteem.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3upxfrrnn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3dmemcnuo.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3xtibfjdo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3apfzcyik.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3ybjyfxxn.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3jblkakci.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3gdewbhyi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3cvydaxag.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3pylxoscq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3nbrangwt.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3lcbusevy.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3sksewwtr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hwyvaxrp.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3jrzoajaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pdyrvtmn.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nnoqrjrj.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3gplofihf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3lpkflabo.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3znzuwcui.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3nxzpsork.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3sooncbbz.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3zwhhricx.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3fuggbfcb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3hwsfkqlh.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3vnthiggf.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3rdaimwxv.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3akptjrss.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3ypdvtwdv.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3pugwqedy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3srgnkbwp.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3bpcrswum.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3heqoqrxy.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3clhgyxgx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3anrwgtwo.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3pdfzpjxy.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3cfgwpqfh.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rjihceez.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3dbtytdgk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3bqjrmbqs.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3qpblevmn.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3hvjmfeyk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3rnqqkiqg.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3yqcllegt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3lpkuppup.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3udbfupjr.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3ejpgmjas.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3aouqrcpw.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3xvwowjsx.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3tlcyfsao.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3wczabjvx.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ltxgohqq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3dcvesgdf.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ynwzwngv.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3jiecowtn.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3yiukqsxy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ouwxfrmc.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3tsizztyp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3bfpkxqxq.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3jfjfskfw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3jqxtpdmc.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3dtxedhig.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3ikncqyra.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3vyuritru.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3vefpksmj.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3xcbwkexr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3kxbginvd.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3htgmchus.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3bciurhip.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3idlxatrb.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3ctbykuok.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3mfbouuht.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3weahmryt.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3wpttztkb.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ttnetsgs.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3gvxazmcm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3cjfjazwz.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3eekimrov.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3pvfceggg.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3tmkvrwmk.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3slbrzfwu.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qbwousnw.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3vkmgopyo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dywbuopn.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3cvsdilcx.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3viobwoce.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3lldydpkt.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3onibrkjf.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3tatnqzcl.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3cornysmq.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3vomgjmxa.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3elgmunqe.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3srypails.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lmfxhlsv.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3pecneulm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ehycsirx.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3ketjnrwu.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3zockmrci.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3tycbwhwh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3unmjyolz.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3fiimysov.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nuevcffo.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3fqjpores.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3husffzig.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3radldjbm.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3ydnmwwvn.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3qldzsyuy.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3hlhxnbbs.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3jmbwlkuu.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3eegycikm.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3vakisnhu.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3fdcpqxvk.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3yernkhwe.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mcxjelax.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ryembsay.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwzvnkfp.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3gwtwlmio.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3peqklgwi.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qatktmtr.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3rzdfcrip.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3xgcwqlgp.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3utfssvpn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gpllojlf.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3cxvawlaz.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3vfsvkoep.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3nyhtybee.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3mfbvbzas.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3spmsjhpy.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3zwcyaham.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3uxlsnyph.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3luwynsty.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3jmyqedpr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xbpwzchv.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3cxplscag.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3caeoionp.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3yptnwmra.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3oijejnzo.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3pgjwstvq.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3pbqvlvrs.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3qybvlmli.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3vhqzuptq.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3pmdmjphk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3kfxpnwxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vlmdnfex.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3uwbbizbp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pdaxumps.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vrvuuhcm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3nzsisvmb.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3oqeaggvs.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3kvptapeo.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3zssrwfsd.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3oeneacbj.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3bzwwyhtu.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3jvjcixvz.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3aeyyffyv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3renzwfio.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3lazevgqs.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3uebfdbbf.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ttpwphzr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3qghhfupu.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3lyrnxihs.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3tangrweq.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3vtvvmwbg.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3caceizht.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3ctkpzgup.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3xnnjnmjd.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3pepwxvdi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3cwztbyrs.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3ewcdjrrw.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3przcdskj.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3ddlpxfdq.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3nfuncdgv.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3exgsmrxp.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3kpocxpim.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3rhjncmpz.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ywlstntc.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wwhtbefk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3yhkpzfyi.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3mzfcxhod.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mneuvvky.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3mhdfpfhd.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3ruttunez.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3ctkaetvw.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3dkpwgxcl.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3xexqavlh.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3qrdpxbxx.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3gcfnbnas.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3jzzmmlgv.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3heotjkgs.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3lrkklndn.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3xbxgsgre.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3iibsgsuj.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3lgmanwix.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bezcwvdd.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3dxvfbght.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3dlcxyojs.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3mnbysuvo.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3fpfcsuiy.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3umakgzxs.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3nlmtqgjl.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3wffyebcy.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3nbnhyjjz.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3smderrsa.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3tiinhrhm.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3wikmermp.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3lqcmwyme.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jusocqyf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3bveqfwzp.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ezfrwywq.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3rbhrnkds.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3rxwfpymo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3pegiiifs.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3slkhtegx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3kmdrmrir.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3zcyjpcno.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3nyfayivq.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3nyozfkqj.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3oaqgfhqa.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3rvfzzjoj.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3jtjfajll.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3kbxgcaxu.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3zuasaego.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fshgjwwv.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3qcljijkv.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3lvmhswkw.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3wmpuqnsv.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ycyiffwr.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3qnjdoceu.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3tlslxjqh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3ajxvoebw.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xfbwhzob.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3jprmuuxs.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3jrdxivcl.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3hdxjsgne.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3idnudwkd.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3juujuwlb.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3osumtdiw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrapmdwu.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3dmspkdfs.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytntofus.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ebajtxoz.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3unjrqmgu.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zpqywyzj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrzteeko.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3piovzpze.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3hruhfxsn.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3igapmahu.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qtcvbluq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3eenoagrq.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3bgsaktfn.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3nvtndmnq.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xsobqgpq.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3kjxikhhn.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3kfmqutmp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3tnnslwzg.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ktymolci.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hajarupx.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3rxxgwgoq.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3psgsokqy.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hgwksrvl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3uachuzhr.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3ljfcfmft.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3vjhwomvn.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3lbakujqx.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3dsywxkvw.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3jhudgeue.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3valtkomb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3txisdzyn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ueluwxiz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kchpyhnp.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3yypsgtkb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3bdoyzxxv.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3qiddkgef.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kjduyzku.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3lqyuvuyd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3ortjgbta.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3fpvsdqdq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3jkuzhqri.html


<!-- 参考信息 -->