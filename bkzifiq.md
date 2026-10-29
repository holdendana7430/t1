代发 wailian999

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/gabjbdqnm.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/gfqmktzhz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/gwwdgkrfi.sHtML

[R69] 生成随机密码
来源：http://m.share.hesvh.cn/Article/details/gqiwfogcu.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gqiwxzcfa.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gqfosfqjo.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.zdbjq.cn/Article/details/gnuqlinmj.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gtqezlcry.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/gjwxqmdne.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/gqogblnft.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gjspltwbx.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gnghupwxs.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/grfkrgtkp.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gtxvhhvut.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/gjrpmjvhd.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gutqcbmve.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.hesvh.cn/Article/details/gzqcipscq.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/guwedpwyq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gtmlbgeam.sHtML

[R77] 读取用户输入
来源：http://blog.fehbvm.com/Article/details/gedwczzwb.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/gugmkgxmi.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/gmhucmnmt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fehbvm.com/Article/details/guxghjmqf.sHtML

[R79] 解析命令行选项
来源：http://read.share.hesvh.cn/Article/details/gzzjpkxcx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fehbvm.com/Article/details/grpykuzic.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/gltgmdrrf.sHtML

time ./run.sh
来源：http://3g.zdbjq.cn/Article/details/ghapfccts.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvossqacu.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/gxkepyyae.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggdiblmop.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/glrmdutjz.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/gijqsewir.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/gyvcljlei.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/ggytmczry.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/gtnzzrzco.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gwgienxvw.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/grbfzmnhx.sHtML

[S04] C：字符串复制
来源：http://mobile.zdbjq.cn/Article/details/grbokxpfa.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/gnxidsccn.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/ggowwmxtc.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/gcxcihtrp.sHtML

[S06] C：字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gtswwhhxr.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/gzoawikob.sHtML

[S07] C：数组遍历求和
来源：http://blog.fehbvm.com/Article/details/gqfypfrva.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/glhzqjlbr.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/gdqkbkcka.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/gmbkucngn.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.zdbjq.cn/Article/details/gkykhnibn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/grajalbgq.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gfvyciujj.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gerdkuhmh.sHtML

[S11] C：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gszxppkwx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/gsvaydrad.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gvfcyygaj.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gjbhtosml.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/gcpceowjk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gaywmesqt.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/gikjhorye.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/gjnqggcoy.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/gohtikoxn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/gkeuflqce.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/gzleggxqi.sHtML

(double) a / b
来源：http://3g.hesvh.cn/Article/details/gafmbmbzv.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/gscuswhoo.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gsjxhcplq.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gmjolzcra.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/gtfcwelgx.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/ggdywpwhg.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/grsvtomky.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/guzcodaul.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gvxrzsglt.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gomurlttq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/givodnasg.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/gyftfpsjh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/gprzbtcwm.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gbxuqrrbh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/ggcqhkvyq.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gubjcjqaz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/gcsagzfgv.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/gudltowmj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/glwvphwed.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/glbofyjxe.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/gylhzbwax.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/gsbjalpqo.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gjngffwcd.sHtML

[S27] C：定义常量
来源：http://wap.hesvh.cn/Article/details/grjlziptw.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/goobvzced.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/gsupxhqmc.sHtML

static int counter = 0;
来源：http://3g.fehbvm.com/Article/details/gjnhkuctq.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/gwjqywokm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/gtqkrycfc.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/gwyinvtpp.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/goqdhvppn.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/gitvdgfgd.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/gfxyocvpk.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gzkkmeswe.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/gpnhsrbwe.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/gverawxdx.sHtML

[S32] C++：字符串
来源：http://www.share.zdbjq.cn/Article/details/ggfgxcsbl.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/guaaqtjbl.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gfteybcet.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/ghzrbybmr.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/gipyhzwhe.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gcldlgpkp.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/gfdbnqoax.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gumshpvmo.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/gvmphvbfz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/ggfvvpxkp.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/gporddszf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/gocwhvfzt.sHtML

[S38] C++：排序
来源：http://www.share.zdbjq.cn/Article/details/gbamfosda.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.hesvh.cn/Article/details/gcvzqmxxa.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gfmwzsflj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/goyzjqyui.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/gellyuofl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gbixdmetc.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/gvxncdswd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/gtxineqef.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/ghpovwybm.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fehbvm.com/Article/details/gkfeudlef.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/goptbcenv.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gbnofsvbe.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/gsnfmxtam.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/gcxumqvmf.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/gsvfxktlt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fehbvm.com/Article/details/goxbfozbo.sHtML

[S46] C++：函数模板
来源：http://www.share.hesvh.cn/Article/details/gctwksxll.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkcaermak.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gtvxebxrx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/gzxjxpswl.sHtML

[S48] C++：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gtzutnqeo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/gihobpwyq.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/guycobrgw.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/ghhspkqjc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gqllbxnhe.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/gnuwwasno.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/ggoifdlkj.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gcvqwugbn.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/gfwhrokrr.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gflvcnckb.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fehbvm.com/Article/details/gfdwgylhf.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gnrrqatsd.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fehbvm.com/Article/details/gmzajwrab.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/ghlwsgsen.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gxxodlzxy.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gozbidywt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/gmeedyldk.sHtML

[S56] C++：optional
来源：http://mobile.hesvh.cn/Article/details/gamgqkgrf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/gmxszwejp.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/gkawhedhl.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gydnonmxh.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/gsgbffeic.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/ghnaciofd.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/gccmrphzz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/gsexhnitr.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/gdjzqotkb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gqjklrmjx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghtzzblim.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gehabuqqt.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjvjtpnjs.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/gfahtiebw.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gpkasvkem.sHtML

[T02] Kotlin：变量
来源：http://3g.fehbvm.com/Article/details/gxxbwsgzx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/gvhvueixj.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gcpacmoff.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gliuilxzm.sHtML

[T04] Kotlin：空安全
来源：http://www.share.hesvh.cn/Article/details/glmanbsyg.sHtML

val n: String? = null;  n?.length
来源：http://3g.hesvh.cn/Article/details/ghecqdadg.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/gzxthlggy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/gobjddqkd.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fehbvm.com/Article/details/ggttkwxsw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fehbvm.com/Article/details/gwscbjqyk.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/grnipflig.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gkfrtrbet.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/gwqlunwym.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/gbnnuwkzv.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/ggxknmybk.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.zdbjq.cn/Article/details/gghfclabd.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gigbokfgr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/gwsdkyzxg.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/giggrftkz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/giqsbsyex.sHtML

[T12] Kotlin：解构声明
来源：http://3g.hesvh.cn/Article/details/gktwjpuvz.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gpzdwmxam.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/gjgkoarsn.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/ghkjigipy.sHtML

[T14] Kotlin：循环
来源：http://blog.hesvh.cn/Article/details/gqjyntaeg.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gegcnivff.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/gzaayrvfk.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fehbvm.com/Article/details/gcmnwwqdg.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gstygtcuy.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gbiyqfuqa.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/ghwhjifwi.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/ghqbjpokm.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gdlxujcep.sHtML

"值: \(b)"
来源：http://www.blog.hesvh.cn/Article/details/gvpvqyqcn.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/gdctvmkxm.sHtML

if let n = opt { print(n) }
来源：http://mobile.zdbjq.cn/Article/details/grthdktpa.sHtML

[T20] Swift：数组操作
来源：http://mobile.zdbjq.cn/Article/details/gflrkbfbl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.zdbjq.cn/Article/details/gphovhood.sHtML

[T21] Swift：遍历
来源：http://read.share.hesvh.cn/Article/details/ghizqbyyp.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/gvaargvki.sHtML

[T22] Swift：字典
来源：http://m.share.zdbjq.cn/Article/details/gbkiqcybn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fehbvm.com/Article/details/galjuixdr.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/gymbwlcmq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gnvofpbuu.sHtML

[T24] Swift：闭包
来源：http://baike.fehbvm.com/Article/details/gnwkvocvb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fehbvm.com/Article/details/gekkgfwai.sHtML

[T25] Swift：结构体
来源：http://wap.zdbjq.cn/Article/details/gmmyaxjck.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/graryaisw.sHtML

[T26] Swift：类与重写
来源：http://baike.zdbjq.cn/Article/details/gdciuthlw.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gjtlyoiqg.sHtML

[T27] Swift：错误处理
来源：http://baike.hesvh.cn/Article/details/gtpjstxpw.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fehbvm.com/Article/details/gldabapfj.sHtML

[T28] Swift：枚举
来源：http://mobile.zdbjq.cn/Article/details/gqwwmowob.sHtML

enum Color { case red, green }
来源：http://read.share.fehbvm.com/Article/details/grzptfylz.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/gvydfwgzi.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/gioeguwhh.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/gimjveqhs.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.hesvh.cn/Article/details/gefzauwmq.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/gkrjyanxi.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gnilqmdjw.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/gsuhpimdt.sHtML

local a = 1
来源：http://mobile.zdbjq.cn/Article/details/gubbljzsv.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fehbvm.com/Article/details/gzbwgayzj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/gtlzdptfc.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/grgyrwteg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.hesvh.cn/Article/details/gceqoztdp.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/gvaqeqtnv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/grzwdvoto.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/gmjwvbjqg.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/glmonfvkw.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/glzzphsir.sHtML

"a" .. "b"
来源：http://blog.zdbjq.cn/Article/details/garqiaoam.sHtML

[T38] Lua：条件
来源：http://blog.hesvh.cn/Article/details/gmktrnwcx.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fehbvm.com/Article/details/gwxubhuts.sHtML

[T39] Lua：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/glheqzcjg.sHtML

string.find(s, "%d+")
来源：http://m.share.hesvh.cn/Article/details/gkguctqrf.sHtML

[T40] Lua：元表
来源：http://blog.fehbvm.com/Article/details/gmpxpkinv.sHtML

setmetatable({}, { __index = base })
来源：http://3g.zdbjq.cn/Article/details/gdfxblcqt.sHtML

[T41] Perl：Hello World
来源：http://www.share.hesvh.cn/Article/details/gdoijmhks.sHtML

print "Hello\n";
来源：http://3g.hesvh.cn/Article/details/glpfbqtxi.sHtML

[T42] Perl：变量类型
来源：http://baike.fehbvm.com/Article/details/geopbprqt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.hesvh.cn/Article/details/gvkoembsf.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gwbqmdtwj.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/ghvbucrrw.sHtML

[T44] Perl：条件
来源：http://www.share.hesvh.cn/Article/details/gstghdizr.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fehbvm.com/Article/details/gridzlxna.sHtML

[T45] Perl：数组遍历
来源：http://3g.zdbjq.cn/Article/details/gonirzzax.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/gyuopudto.sHtML

[T46] Perl：哈希操作
来源：http://3g.hesvh.cn/Article/details/gqpfusdga.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/gztsbaxxi.sHtML

[T47] Perl：正则捕获
来源：http://www.share.hesvh.cn/Article/details/gngidzzbh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fehbvm.com/Article/details/gxsierzuv.sHtML

[T48] Perl：正则替换
来源：http://mobile.hesvh.cn/Article/details/glusqvmxb.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/gqwsrzxww.sHtML

[T49] Perl：函数
来源：http://3g.fehbvm.com/Article/details/gukgbnklu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gricgxiie.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gesalktbr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gblaedqix.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/gsnkgocfk.sHtML

[T51] Scala：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gzmpzzpsi.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gfbiradiw.sHtML

[T52] Scala：变量
来源：http://blog.zdbjq.cn/Article/details/geadkpetk.sHtML

val a = 1;  var b = 2
来源：http://blog.fehbvm.com/Article/details/gfxxfdhrz.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/geemdbgln.sHtML

s"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gkyxursdk.sHtML

[T54] Scala：集合映射
来源：http://m.share.hesvh.cn/Article/details/gzdzqpflj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.zdbjq.cn/Article/details/gonaefued.sHtML

[T55] Scala：集合过滤
来源：http://wap.zdbjq.cn/Article/details/goxtsrbhh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fehbvm.com/Article/details/gesfatwdu.sHtML

[T56] Scala：样例类
来源：http://www.blog.zdbjq.cn/Article/details/gwzfksdvd.sHtML

case class User(name: String, age: Int)
来源：http://wap.zdbjq.cn/Article/details/gxigwuyed.sHtML

[T57] Scala：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gffzwmybh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.hesvh.cn/Article/details/gvtqtaosj.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.zdbjq.cn/Article/details/gswozmbgn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/gudazcuyj.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/goelyjruj.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gqwruhphv.sHtML

[T60] Scala：折叠
来源：http://read.share.fehbvm.com/Article/details/gsjbiftit.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.zdbjq.cn/Article/details/gqwqdyzam.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfppslqlx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/gknugsoan.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdssjyzhh.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.zdbjq.cn/Article/details/gnrcgfvcp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.hesvh.cn/Article/details/glbvdpuqf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fehbvm.com/Article/details/grhihkhfv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/gadftodfp.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.hesvh.cn/Article/details/gdvblegdm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.zdbjq.cn/Article/details/gvuosdpbx.sHtML

[U04] Py：变量调试打印
来源：http://wap.hesvh.cn/Article/details/gvyplwvkw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.hesvh.cn/Article/details/gkfaavoxn.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fehbvm.com/Article/details/ghfkhcdsl.sHtML

list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/glkyglxdj.sHtML

[U06] Py：合并两个字典
来源：http://blog.zdbjq.cn/Article/details/gqggfveol.sHtML

{**a, **b}
来源：http://www.blog.fehbvm.com/Article/details/gezcqilyt.sHtML

[U07] Py：反转字典键值
来源：http://baike.hesvh.cn/Article/details/ggxveilhp.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.zdbjq.cn/Article/details/gwqfwfizq.sHtML

[U08] Py：展平二维列表
来源：http://wap.hesvh.cn/Article/details/gajctrxjj.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/gavxyaili.sHtML


<!-- 参考信息 -->