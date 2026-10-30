代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.hesvh.cn/Article/details/geaqtvlri.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/gnniglzii.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/gpmvvztuz.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.zdbjq.cn/Article/details/gdlwjpqun.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/gxfevmwoi.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/ghcztacvu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/gvfmzrssi.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gqpfgcbji.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/gagmublxp.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gtxkssdmb.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/guwztbdcp.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gwmyzzqcc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/gjrtlvdjc.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gqyutiirz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gddflkyzj.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gztajgvum.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/gnumlmdmt.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/gpbizpkfl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/gpakhvchk.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/gutggaewk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/gohobmaxh.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/gckdaftna.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gmildarja.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/gswqqggbw.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gpwsygmlj.sHtML

[R78] 交互式菜单
来源：http://read.share.fehbvm.com/Article/details/gvmqzhych.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gyvxxdxya.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/gvrqpjvdn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/gqrbtdxhj.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fehbvm.com/Article/details/gofbqjkax.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/ganjticjg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcajldjpd.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/gllmmzcze.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gdesnyfwi.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/gflmfqrtk.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gvzhrohjy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/gmppcxwbe.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/gptdcojyq.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gerrvdsbw.sHtML

[S03] C：读入整数
来源：http://blog.zdbjq.cn/Article/details/gazmkjizh.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/gdvmqzowh.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/gkgmbufta.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gervdmqsu.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gacgaqdkh.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/gacoqdnwg.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/gbfsrkimj.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/gsjsiezfl.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/ghjgxwqur.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/gnaumisnd.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gdtyzjzot.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gwqodrtlq.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/gxckhwmgc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/gjekjbthd.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/gobyxfhvc.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gnykmgbur.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gogcgcvit.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/gsakbfddq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/ggtspidth.sHtML

fclose(f);
来源：http://mobile.fehbvm.com/Article/details/goahvhprt.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/gkciqghvi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gigdwfjly.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/gqqvcljuj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gtvnzidmz.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/gevnzqghf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/gbddnokbw.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/glmjsgmsc.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/gljxacfjg.sHtML

[S16] C：位操作置位
来源：http://m.share.zdbjq.cn/Article/details/gkcaexmoo.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/ggcsziilh.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/glotyyilf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gfevufeac.sHtML

[S18] C：命令行参数
来源：http://3g.fehbvm.com/Article/details/gzbwoszpp.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/gvbwdajhs.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/grvbpikgm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gsmairtds.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/gsezwzmvc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/glijkvbrw.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gydefrvzc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/gytrphqjr.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gbxjpebkj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/gdfccbfny.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/gkfkzlubp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gvxsytzuu.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/gfvnwhpfl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gltonhgjl.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/gvcdytsyi.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/gnwuprssw.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/gpdwzyhwp.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/gnwyrwkoi.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gqmossbbv.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gepcosoxi.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/gckdcxeuj.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/gyivarlkg.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/glqhsrhpd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gsynqmswo.sHtML

[S30] C：头文件保护
来源：http://www.blog.hesvh.cn/Article/details/gkkcfprce.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/gsekbhpap.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/gnnwxkkvs.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/gzookjuob.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/ghxiglvip.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gnbxohntt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/gpurdulys.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/gbicesbdc.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.hesvh.cn/Article/details/gwdkgvgqt.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/gblfsllpv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/gexcngqnu.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/gbhhsmjce.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/gukrylxuw.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/ggectomve.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gungudpev.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/gabyocwvd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gllsgtlwu.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gyhzpfgyn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/gwfqsvghh.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/gfukbwktw.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/gwdivymvh.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/gdhqcjhnp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/gmfmwkiak.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/gryeizylf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gofnwdajv.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/gfirruhao.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fehbvm.com/Article/details/gmvsvsfyu.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gnervkegk.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fehbvm.com/Article/details/goywusnzs.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/gurocllpv.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.hesvh.cn/Article/details/gbzguaiby.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/gjawvakgi.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/grmznmrdf.sHtML

[S45] C++：lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gvtojgvlm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fehbvm.com/Article/details/gvctltrlo.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gngnpogbb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/glfifzlif.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.hesvh.cn/Article/details/gyyjkubge.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gfeinmqyx.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gutuyrazd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gxxgjqbjo.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gpslxlumb.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/gmdoyfzvi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/gsfhutkhi.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gqhaqvcjy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gtgavyeaw.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/gvxoyhlda.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/gjktgrjhp.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/gwuhixjiy.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwavsveop.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/gsdchbtmw.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/gtaugnqyq.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gmpltobzh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/guikiluvq.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/gshbcdrki.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/gigoifntl.sHtML

[S56] C++：optional
来源：http://www.share.fehbvm.com/Article/details/gnpwbltpe.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gqwjxmugb.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/gtjeyvqzr.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gkfhmbwdc.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/galiached.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fehbvm.com/Article/details/gkofdmyat.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/gnsfenlor.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.hesvh.cn/Article/details/gmhmfyths.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/gqtkfvyye.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/ghrrklgur.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwvohizzi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/galhyhzuo.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqqjgcllg.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/gfltnzevk.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gihczsebs.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/gvwjidjlx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/gthhfjmfw.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/ghjngyxft.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/gtsbqqyry.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/gdnrxdwdd.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/gjegwtlom.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/gqdtvyjus.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.zdbjq.cn/Article/details/gjpytoran.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/gujwwdltx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.hesvh.cn/Article/details/gtcoxhyxy.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/gtygyuabb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.hesvh.cn/Article/details/gvkhzglha.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/ghhrmoacs.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.hesvh.cn/Article/details/gfxlnygzc.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.hesvh.cn/Article/details/gmpbofcyw.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gjnighumd.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/gnkfwyxyj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/gienlklsc.sHtML

[T11] Kotlin：协程
来源：http://mobile.fehbvm.com/Article/details/gyfnbsjxi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/gyspjrsag.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/gqoopjdjc.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/ghvbspvfz.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/gzajxtrzf.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/gekhjtdxt.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gjthyuzfu.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gifdhfutx.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/gzfqhwvtz.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gtsetqwtq.sHtML

[T16] Swift：Hello World
来源：http://wap.zdbjq.cn/Article/details/gwyifntaz.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gdwbxtiku.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.zdbjq.cn/Article/details/gddbruvyp.sHtML

var a = 1;  let b = 2
来源：http://blog.hesvh.cn/Article/details/grbbskekr.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/gyeueudca.sHtML

"值: \(b)"
来源：http://mobile.hesvh.cn/Article/details/gfuvksqgb.sHtML

[T19] Swift：可选绑定
来源：http://www.share.zdbjq.cn/Article/details/gegcicfeb.sHtML

if let n = opt { print(n) }
来源：http://wap.hesvh.cn/Article/details/ggbibwwwp.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/gzcocoshe.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.zdbjq.cn/Article/details/gecmeyuao.sHtML

[T21] Swift：遍历
来源：http://baike.hesvh.cn/Article/details/gjqhqyiot.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/gdvpvdjru.sHtML

[T22] Swift：字典
来源：http://m.share.hesvh.cn/Article/details/gtmowglln.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fehbvm.com/Article/details/griytcfxe.sHtML

[T23] Swift：函数
来源：http://read.share.hesvh.cn/Article/details/gayzrjquv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/gjfulhqmx.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/gwktienwl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gwecvmhza.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/gascdugzx.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/ggyrnabiw.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/gpivoyldu.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/gosbcqzdn.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/gehrourkj.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.zdbjq.cn/Article/details/gmpscmgtc.sHtML

[T28] Swift：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gxinjanor.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gphfbcyoc.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/grijsmhia.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/gjzjxwsnc.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/gnkhafpny.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/gvwchulen.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gvzfksjoo.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gihmibait.sHtML

[T32] Lua：局部变量
来源：http://mobile.hesvh.cn/Article/details/gibsmqanu.sHtML

local a = 1
来源：http://m.share.fehbvm.com/Article/details/gbdxgirqr.sHtML

[T33] Lua：表（数组）
来源：http://wap.hesvh.cn/Article/details/gvhbqocyu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.zdbjq.cn/Article/details/gusosvlyu.sHtML

[T34] Lua：遍历表
来源：http://www.share.zdbjq.cn/Article/details/ggryrdogp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/gfrmrwubd.sHtML

[T35] Lua：字典表
来源：http://www.share.fehbvm.com/Article/details/gsrnudixw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/ggpqcenrz.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/gjosdqqms.sHtML

function add(a, b) return a + b end
来源：http://m.share.hesvh.cn/Article/details/gctnvmndn.sHtML

[T37] Lua：字符串拼接
来源：http://3g.hesvh.cn/Article/details/gjyegrrvl.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/gfieldcoy.sHtML

[T38] Lua：条件
来源：http://read.share.zdbjq.cn/Article/details/gemmfwama.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/gpkvwsvzp.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gkyfxrdlr.sHtML

string.find(s, "%d+")
来源：http://3g.fehbvm.com/Article/details/gdumgdlrh.sHtML

[T40] Lua：元表
来源：http://www.share.zdbjq.cn/Article/details/gftiieecb.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fehbvm.com/Article/details/gmkjlvkle.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gagtgiikl.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/gbupstvej.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/gpxzttrbg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/gynwjgoud.sHtML

[T43] Perl：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/ghbxiqxww.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/glfofaapt.sHtML

[T44] Perl：条件
来源：http://www.m.share.fehbvm.com/Article/details/gzqyulcng.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.hesvh.cn/Article/details/gbmcdofzq.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fehbvm.com/Article/details/gvfovjmtr.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fehbvm.com/Article/details/gaxfgadyc.sHtML

[T46] Perl：哈希操作
来源：http://baike.fehbvm.com/Article/details/ghfxibksz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/gbdypdvky.sHtML

[T47] Perl：正则捕获
来源：http://www.share.hesvh.cn/Article/details/gtsbjrtlm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fehbvm.com/Article/details/ggtbqbqsh.sHtML

[T48] Perl：正则替换
来源：http://baike.zdbjq.cn/Article/details/gkyxefrnx.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/gptpwwgiq.sHtML

[T49] Perl：函数
来源：http://3g.zdbjq.cn/Article/details/goholagjf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/ghpcgafne.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gjnpnszbi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.zdbjq.cn/Article/details/gchpwnpbr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/gdzuqezpv.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/grkvqpjij.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gbanvhayn.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/gsgwwmqsc.sHtML

val a = 1;  var b = 2
来源：http://www.blog.hesvh.cn/Article/details/gjncofvsk.sHtML

[T53] Scala：字符串插值
来源：http://baike.hesvh.cn/Article/details/gwnpxujmw.sHtML

s"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gtiodzopw.sHtML

[T54] Scala：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gsgrxqpos.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fehbvm.com/Article/details/gfslpsvta.sHtML

[T55] Scala：集合过滤
来源：http://blog.hesvh.cn/Article/details/gddokwdks.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fehbvm.com/Article/details/ggeogyfht.sHtML

[T56] Scala：样例类
来源：http://www.share.fehbvm.com/Article/details/greaymfkm.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gzrimnegp.sHtML

[T57] Scala：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gjqpmohwl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fehbvm.com/Article/details/gjfxqubzp.sHtML

[T58] Scala：函数定义
来源：http://www.share.fehbvm.com/Article/details/gzqexygtv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.zdbjq.cn/Article/details/gharkmsdm.sHtML

[T59] Scala：循环
来源：http://m.share.hesvh.cn/Article/details/geetzhwqg.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fehbvm.com/Article/details/guwrtzgdz.sHtML

[T60] Scala：折叠
来源：http://www.share.zdbjq.cn/Article/details/grrdxhbgz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/grfmlxdnb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxsnhrtys.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/gxlxzrncr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnbzhqgwi.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.hesvh.cn/Article/details/gegmajvlk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.zdbjq.cn/Article/details/gqrsohapu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.hesvh.cn/Article/details/gvldwjgfu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fehbvm.com/Article/details/gsarywswj.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.zdbjq.cn/Article/details/gxrbjrnlf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fehbvm.com/Article/details/gluwjhxqu.sHtML

[U04] Py：变量调试打印
来源：http://read.share.hesvh.cn/Article/details/gqgpmjxgr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.hesvh.cn/Article/details/ghucewqwa.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/gifpiwcjx.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gykpudyev.sHtML

[U06] Py：合并两个字典
来源：http://blog.fehbvm.com/Article/details/gfzqnoknd.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/gmrkcsdcb.sHtML


<!-- 参考信息 -->