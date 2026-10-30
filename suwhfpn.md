代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/gmukovckc.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/glihabnmv.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/gvrfjjhah.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/gscxzabob.sHtML

openssl rand -hex 16
来源：http://www.share.hesvh.cn/Article/details/gpvsbvdmb.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fehbvm.com/Article/details/gihtroyav.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.zdbjq.cn/Article/details/gvoejurpa.sHtML

[R69] 生成随机密码
来源：http://m.share.hesvh.cn/Article/details/gsiamsexy.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gnquhchsk.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gndiygrvx.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/gjsmihllw.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gtlbftsom.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.zdbjq.cn/Article/details/gxrqexouk.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/ghpnhuktb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gkbrduwaj.sHtML

[R73] 分割大日志
来源：http://www.blog.fehbvm.com/Article/details/guquzfkqo.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gsidimmgy.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/grplyoxgq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/glgqckjvm.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gctcmuaad.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.zdbjq.cn/Article/details/gyftjchsl.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gflnegoln.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gbtddtqvn.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/gqwrvsxzn.sHtML

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/gfeiaieuu.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gpklsgodn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/gphwmrtia.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/gvyeeqsik.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fehbvm.com/Article/details/glwcpbcrb.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/ghfmblalo.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/giiibcwey.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/govnbmril.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/gdtrwxfzv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gcidzhcwd.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/gnsuskvtj.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/gejljcaxb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/gikdjrvqu.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gadfcjudl.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.zdbjq.cn/Article/details/gfxrdswbr.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/gpeapqltu.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/gtreiqqrq.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/geaddnauw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.zdbjq.cn/Article/details/grrighkox.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/ggfymrvdj.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/gqjpgydjy.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/glzllplai.sHtML

strcmp(a, b) == 0
来源：http://www.blog.zdbjq.cn/Article/details/gemguhavi.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/gekinehzx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fehbvm.com/Article/details/gwyrwtjkl.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/gelyqqmoa.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fehbvm.com/Article/details/gfiyrelwa.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/ghxszkfjt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/goboluygo.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gckizqgwq.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/gfzclvlfd.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gxqnuzkun.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/gspawgxsj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fehbvm.com/Article/details/gqvbtyjnc.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gmpncqxja.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gufdaydga.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gatkdlkfm.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/gmhbispgz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/gwcnwjjid.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gzqeszfvz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/gwybhihbl.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/gdcfnuvcs.sHtML

(double) a / b
来源：http://read.share.fehbvm.com/Article/details/gcuefqhin.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/gcrgynsnk.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/ggrlyuesk.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gktbsfanv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/gfqcwnabq.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/gvgmxbrio.sHtML

int main(int argc, char **argv)
来源：http://read.share.fehbvm.com/Article/details/gihbvfesj.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gzevzbhwb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/ghdxftfom.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/gdoyqnlkr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gdjoibgxj.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/gfjlgdjtp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/gukdsdwap.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/gngfslokn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/gvlpkymub.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/gaiteupcq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gasloeivx.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/gqcwyobak.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gzavdette.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/gcuyzdgmd.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/gpubjkhyh.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gleshhxsw.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fehbvm.com/Article/details/gsnfnpsfw.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/gpudgglnn.sHtML

const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gafyvjvka.sHtML

[S28] C：静态变量
来源：http://mobile.fehbvm.com/Article/details/gjahikrra.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/goupmtmux.sHtML

[S29] C：变参函数
来源：http://3g.zdbjq.cn/Article/details/gcsoxipxe.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gbmsnjraj.sHtML

[S30] C：头文件保护
来源：http://www.blog.hesvh.cn/Article/details/ghpaaevvx.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/grrwhampq.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gbjgzkxpd.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/gdapagodp.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/ggqdykqur.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/gxaqjmskh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/goivnpsht.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/gyaifpebp.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.zdbjq.cn/Article/details/gxsnbjqcd.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/guvsytxpu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/ggrqbwbth.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/glllzzfpt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/giexhgpsq.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/gixdbtuzu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/goukdsbnx.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/gbzurgvsg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/glssdegim.sHtML

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/gxwiyuktl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gartitmxn.sHtML

[S38] C++：排序
来源：http://www.share.zdbjq.cn/Article/details/grqoslgfw.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/gjiplnlff.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/ghwcuosdr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gvqxjrfvd.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/gyvbjfmjy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/gncazgphq.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/gvvtgipwn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gksjsamip.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/ghzakqrvx.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/gptbdoquv.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/gfmdwxwyf.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.hesvh.cn/Article/details/gyglhgwwi.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/gckwriswm.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/gcwvqfklj.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/gcuzkjzja.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gjopjufhi.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gbfitukbt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/gnvfamcsf.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/guplshjru.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/gmgwxpsre.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gmtwmtufl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fehbvm.com/Article/details/gpqxfbggj.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/gmqdhjgsl.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gxhhqjald.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/gilsiezmr.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gosbalsfi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gtsqlbmli.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/gbcnhbgze.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/gegvvpgjm.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/gmxxciptl.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/gfnjpeakg.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/glapdvubs.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/gurlzfzqe.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gvuluoasx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.zdbjq.cn/Article/details/gnfcmqsym.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gnivabywq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gaoeupfwm.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/gfghegkkv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.zdbjq.cn/Article/details/gaenhompn.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/gpxlalqgw.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/gzpcjvvas.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/gksvefhvm.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gresbgsxq.sHtML

[S59] C++：静态断言
来源：http://read.share.fehbvm.com/Article/details/goujwnuis.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.zdbjq.cn/Article/details/gmuzbyewe.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/gpqnxmmup.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/gacrjivfm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gptcuccmh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gskmvtqoj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/giyyuyxjp.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/gdpmavdhx.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gojbacztv.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/gdsiqfaue.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/gyhxkxfuq.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.hesvh.cn/Article/details/gxjqiuuqk.sHtML

"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gjxxpkewa.sHtML

[T04] Kotlin：空安全
来源：http://baike.zdbjq.cn/Article/details/garlzkyst.sHtML

val n: String? = null;  n?.length
来源：http://baike.fehbvm.com/Article/details/gzevwwpmy.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/gizskxqnb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gxnqsjakm.sHtML

[T06] Kotlin：集合映射
来源：http://baike.hesvh.cn/Article/details/ghkelizlq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gpymtfobt.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gwilvbkvi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/gmelphgvz.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/gbgccjhjp.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gpjgaaoug.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/gvyaniqbe.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.hesvh.cn/Article/details/gsrvcdski.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/ggfxwcgqj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/grektblff.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gxzuenxkt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fehbvm.com/Article/details/ghdcnnvvm.sHtML

[T12] Kotlin：解构声明
来源：http://wap.zdbjq.cn/Article/details/gbrdqiwpd.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gzibbkkru.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fehbvm.com/Article/details/gjvgbvyum.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/gesddinee.sHtML

[T14] Kotlin：循环
来源：http://read.share.fehbvm.com/Article/details/gskrwsbca.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gubfeqsve.sHtML

[T15] Kotlin：接口
来源：http://read.share.hesvh.cn/Article/details/ghzvhcijf.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/ghcxzbwet.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/gedvlkofn.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gaqbidiuz.sHtML

[T17] Swift：变量与常量
来源：http://m.share.hesvh.cn/Article/details/ghnanedxu.sHtML

var a = 1;  let b = 2
来源：http://www.share.hesvh.cn/Article/details/gravtkruz.sHtML

[T18] Swift：字符串插值
来源：http://blog.fehbvm.com/Article/details/gpffhrisc.sHtML

"值: \(b)"
来源：http://www.m.share.hesvh.cn/Article/details/gfsajechm.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/ghxusptmf.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/giwwrswci.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/gxvsvezwz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gokprnmym.sHtML

[T21] Swift：遍历
来源：http://read.share.hesvh.cn/Article/details/gudcujukj.sHtML

for x in a { print(x) }
来源：http://3g.zdbjq.cn/Article/details/gbkivhynr.sHtML

[T22] Swift：字典
来源：http://baike.zdbjq.cn/Article/details/gzgvntuwi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/gmicgxsii.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/gaqfxtwce.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/glrkbbqws.sHtML

[T24] Swift：闭包
来源：http://baike.fehbvm.com/Article/details/gurxzdsuv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gmlhotvwj.sHtML

[T25] Swift：结构体
来源：http://blog.fehbvm.com/Article/details/gksbvmaea.sHtML

struct P { var x: Int }
来源：http://m.share.fehbvm.com/Article/details/gwryhyodl.sHtML

[T26] Swift：类与重写
来源：http://baike.hesvh.cn/Article/details/ggykuiefq.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/gbdkulwxk.sHtML

[T27] Swift：错误处理
来源：http://baike.fehbvm.com/Article/details/gtbndmkjv.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/gehayrtxs.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/glrhccjyh.sHtML

enum Color { case red, green }
来源：http://www.blog.zdbjq.cn/Article/details/gzbdvzcwo.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.zdbjq.cn/Article/details/gqektqmug.sHtML

guard let x = opt else { return }
来源：http://read.share.zdbjq.cn/Article/details/gyvucufda.sHtML

[T30] Swift：协议
来源：http://mobile.fehbvm.com/Article/details/glycagdnw.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gdpcacyzj.sHtML

[T31] Lua：Hello World
来源：http://mobile.fehbvm.com/Article/details/gccebdper.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gxbhjnkun.sHtML

[T32] Lua：局部变量
来源：http://baike.zdbjq.cn/Article/details/gcbunmahv.sHtML

local a = 1
来源：http://3g.zdbjq.cn/Article/details/gafoszlcq.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fehbvm.com/Article/details/gtxevwhys.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.hesvh.cn/Article/details/ggjcaduak.sHtML

[T34] Lua：遍历表
来源：http://blog.fehbvm.com/Article/details/glvkmpevg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/gzjgekiul.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/gnzzehefw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.zdbjq.cn/Article/details/gkwdtqmqh.sHtML

[T36] Lua：函数
来源：http://read.share.fehbvm.com/Article/details/ghjysfyzi.sHtML

function add(a, b) return a + b end
来源：http://read.share.zdbjq.cn/Article/details/gcxesdcbl.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gxlyyycic.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/gtmgutkik.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/glkpsnshe.sHtML

if x > 0 then print("正") end
来源：http://mobile.fehbvm.com/Article/details/gfwmytdzn.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/ghdftxjzc.sHtML

string.find(s, "%d+")
来源：http://baike.fehbvm.com/Article/details/ggvzjlguz.sHtML

[T40] Lua：元表
来源：http://baike.hesvh.cn/Article/details/gzslurtqd.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.zdbjq.cn/Article/details/gpcbigvoj.sHtML

[T41] Perl：Hello World
来源：http://blog.zdbjq.cn/Article/details/ghvmqaioz.sHtML

print "Hello\n";
来源：http://mobile.hesvh.cn/Article/details/gnbtteavj.sHtML

[T42] Perl：变量类型
来源：http://mobile.hesvh.cn/Article/details/ggyyymoak.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fehbvm.com/Article/details/ghhjnvawj.sHtML

[T43] Perl：字符串插值
来源：http://blog.fehbvm.com/Article/details/gyitsjmgl.sHtML

"值: $a"
来源：http://www.blog.zdbjq.cn/Article/details/giozmavbm.sHtML

[T44] Perl：条件
来源：http://mobile.hesvh.cn/Article/details/gneojtzcm.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.zdbjq.cn/Article/details/gmlfuvhgt.sHtML

[T45] Perl：数组遍历
来源：http://m.share.hesvh.cn/Article/details/gpvdifeht.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.hesvh.cn/Article/details/gbaotcoou.sHtML

[T46] Perl：哈希操作
来源：http://m.share.zdbjq.cn/Article/details/gmgbmploz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.hesvh.cn/Article/details/grdkyeolr.sHtML

[T47] Perl：正则捕获
来源：http://mobile.hesvh.cn/Article/details/gjscyscbc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/gsgxopkrw.sHtML

[T48] Perl：正则替换
来源：http://m.share.hesvh.cn/Article/details/gvigggmfn.sHtML

$s =~ s/old/new/g;
来源：http://m.share.hesvh.cn/Article/details/gvmdixhee.sHtML

[T49] Perl：函数
来源：http://read.share.zdbjq.cn/Article/details/gvdglhtcn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gzrwbdibg.sHtML

[T50] Perl：逐行读文件
来源：http://baike.hesvh.cn/Article/details/glgfvtubm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fehbvm.com/Article/details/glqsbohtd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fehbvm.com/Article/details/gqtfbvumm.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/guxzxcfwi.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gaiirdzxs.sHtML

[T52] Scala：变量
来源：http://www.blog.zdbjq.cn/Article/details/gllbwvpqh.sHtML

val a = 1;  var b = 2
来源：http://mobile.fehbvm.com/Article/details/goemkcaxz.sHtML

[T53] Scala：字符串插值
来源：http://baike.hesvh.cn/Article/details/gdudjqbyv.sHtML

s"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gmelvqdty.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/gwybflmgw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.zdbjq.cn/Article/details/ghhfxdszh.sHtML

[T55] Scala：集合过滤
来源：http://blog.fehbvm.com/Article/details/gbxqhjpmr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fehbvm.com/Article/details/gvhuvrgpf.sHtML

[T56] Scala：样例类
来源：http://blog.hesvh.cn/Article/details/gdchwhiiy.sHtML

case class User(name: String, age: Int)
来源：http://mobile.hesvh.cn/Article/details/gymrmwtoe.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/glfmwubrz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fehbvm.com/Article/details/geheoacyd.sHtML

[T58] Scala：函数定义
来源：http://m.share.hesvh.cn/Article/details/gdttebths.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/gzshjuqjd.sHtML

[T59] Scala：循环
来源：http://wap.hesvh.cn/Article/details/gkrugpkfl.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fehbvm.com/Article/details/gxdufcbtt.sHtML

[T60] Scala：折叠
来源：http://blog.fehbvm.com/Article/details/gyemxkvwn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fehbvm.com/Article/details/gpxuhugmo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvynfobph.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gqarspkwj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdyesuclp.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/glltrrguq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.hesvh.cn/Article/details/gazbvzacc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.zdbjq.cn/Article/details/gzqbcwhev.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/geqganzge.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.zdbjq.cn/Article/details/gtfzblymh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/gvykqkkjl.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fehbvm.com/Article/details/gxzdtrrvi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.hesvh.cn/Article/details/gctoidbok.sHtML

[U05] Py：列表去重且保序
来源：http://baike.hesvh.cn/Article/details/grkkesqup.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gbejsvkxs.sHtML

[U06] Py：合并两个字典
来源：http://wap.hesvh.cn/Article/details/givotmund.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/gfbckbxwh.sHtML


<!-- 参考信息 -->