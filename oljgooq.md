代发 wailian999

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gumsmjqlm.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gozjuhdcd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/griwuumuy.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozlgshoa.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/glnuirlfv.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gmzbhknan.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gukafzqps.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gemipiqbl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmohzsvm.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gcsqcptlg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gzxdbmiti.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/goouxdtgj.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkrwmsxl.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gmiqvwuxk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gumfdfctg.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwvolktm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gbuxrsxdx.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gslyqlsan.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvwspikf.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqoffxgt.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjsjysgi.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gueuqnukg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/guhhdlwao.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjytmxli.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gfuxpsjup.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gpczwgpwv.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmwokboz.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gnvetyjil.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgmzkqvt.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmwhsqth.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdjickgi.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gvxzncyxz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvsaavzqw.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsioqdfdq.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjajqtlbk.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtynrrme.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gaaqqtwzu.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskltckcq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gcbhmsikm.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepyeprvy.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlmqeixe.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gahaipphy.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gczpphimo.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/ggclnlynf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnqejeta.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/ghylufjch.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsuifyaz.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gdjdmbcho.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gosioayvw.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtaagaay.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gvwwciqbw.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqsiijiz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/getagoryy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gmkicclji.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkwsyfex.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpxhdxds.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gtopgbhiz.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwxxajwu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/glefzwsxi.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gfosmsftf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gwhkhskhr.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gekiitpwm.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/groguychm.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guipnnnfm.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqgoualt.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gewpojewn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gfqoajdge.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbzycdin.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gelikoqja.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfvntaqi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gjvvsfjgq.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gqekkieml.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gctggahjb.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gpszsyyim.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwebscitr.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/guxjjdffw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gonjytobk.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gxuphkclr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gziwltheh.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gontfmuvj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gtyxsgdyx.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gcoerhslo.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gmcgewsmy.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gumpialtm.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giubpjtfx.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvpontll.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/ggcuyljyw.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlwxdjsr.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwtzcaga.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvqbgxex.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhsxewgo.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gtwuhlajr.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gwwnnohty.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gojwvbsvo.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqiooavi.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/ghhqbfmld.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gpmhrpuut.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gowaigxuo.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrcqycab.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcynisgei.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgeswsst.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gkzmxwpam.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/goohwodsb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnrdvwzmo.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltategeq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gchrwnfdb.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gseplnemb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/grmxlzcqz.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gngyzzzfb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gymqskoex.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbcoruny.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gsyiueyyn.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gtsrseajd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfennygk.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/guvdknlwo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gxinwaosi.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmlgwqbx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gvhjfsasl.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gjgjpsfie.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcskwwup.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmicfcwcs.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpqwhrqg.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gfaiavcmj.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/glzodsuzl.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gclidnzng.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/gbikjuxun.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzwhhksb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjohwoepk.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvzuqami.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvebuvsyc.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gsmyyuyca.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/ggrjxjdcl.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghsgyztpu.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwkfrirr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gikljxxlx.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlanousz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqomzzdov.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhzzbksg.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gjheqyfrk.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyqfmzux.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyirpwuz.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzlombzs.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/gpwsdseuf.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffxfcheg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gmejtklbn.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/giswjixxt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gmxpnoaay.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnranmgms.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/giiglhdlv.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/glsvmayxl.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/grsvkelho.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gptuwkfit.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsppslhju.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/glwinmxti.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfplplopq.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/ggqdepawj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/ghmlvgyzb.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcijigep.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwcoosjj.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpdgtmcj.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpbhyzuc.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gydgqdgxd.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwxknhgt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gxstedumg.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gphrmouce.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gorkodofo.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gkxzdfepi.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gupkntkhh.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/goghvggad.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofauxmtp.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gjglgswju.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvrllfba.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gbwxwrnmm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gvwwxlzet.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gaussiiij.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/ggfcrtqyd.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gfrwyfcyx.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glesssusw.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gitdqixpv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gefsmyaah.sHtML

[T11] Kotlin：协程
来源：http://mobile.fanxiaobao.xyz/Article/details/gofdiqjsd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrabwupi.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/grwitttpq.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpaeiuqab.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/glabpqjaf.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxagxrny.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gylpswnfc.sHtML

for (i in 1..10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gzacmgohw.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqjcxcvm.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgpswgpa.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gykrgsitm.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnbpvana.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/gufwibvat.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/glyhhyjev.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/glotmdpld.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpphfjgn.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlkljtmg.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswsmvrdw.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/gwfhqumna.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gzcghzkdo.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfuzhzkn.sHtML

for x in a { print(x) }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmxbccho.sHtML

[T22] Swift：字典
来源：http://baike.fanxiaobao.xyz/Article/details/gcfwpixql.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwbfebgc.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gpzrcszbk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmaccnrv.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqihkvek.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaufgiryu.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfqbrvpb.sHtML

struct P { var x: Int }
来源：http://3g.fanxiaobao.xyz/Article/details/guypbopqh.sHtML

[T26] Swift：类与重写
来源：http://wap.fanxiaobao.xyz/Article/details/ghlscyado.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfulkxjlt.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gpjdwikrp.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqexxmyp.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/geffovhmc.sHtML

enum Color { case red, green }
来源：http://baike.fanxiaobao.xyz/Article/details/glmgqlqyq.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/gweyhgcre.sHtML

guard let x = opt else { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwkbtgav.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/glakuhobp.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmvpufew.sHtML

[T31] Lua：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhgtyqmf.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqqyyuob.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gqnkwwknj.sHtML

local a = 1
来源：http://wap.fanxiaobao.xyz/Article/details/gcqnencyu.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/gxoczctuz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fanxiaobao.xyz/Article/details/gurzbhjod.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngasjpnx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgjswptu.sHtML

[T35] Lua：字典表
来源：http://www.blog.fanxiaobao.xyz/Article/details/guindaloi.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gkihoqdib.sHtML

[T36] Lua：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gpgnagvuy.sHtML

function add(a, b) return a + b end
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfcccqui.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/ghfiekzwi.sHtML

"a" .. "b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqyxcnjno.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/ggyrrewvy.sHtML

if x > 0 then print("正") end
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxsawuzw.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gqeagebja.sHtML

string.find(s, "%d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnoegkah.sHtML

[T40] Lua：元表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guoizrlel.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgxtskbn.sHtML

[T41] Perl：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbrapjnm.sHtML

print "Hello\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwolxgja.sHtML

[T42] Perl：变量类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrrhxsbb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvjdfols.sHtML

[T43] Perl：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/geblrxxfy.sHtML

"值: $a"
来源：http://blog.fanxiaobao.xyz/Article/details/glrbwiygk.sHtML

[T44] Perl：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpsfhumc.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gafkwuwda.sHtML

[T45] Perl：数组遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gmdjgubbx.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gflgkeijh.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrmytrkk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghclibimn.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwlhpvde.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpjycmvh.sHtML

[T48] Perl：正则替换
来源：http://baike.fanxiaobao.xyz/Article/details/ggreznqmd.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayljhuua.sHtML

[T49] Perl：函数
来源：http://blog.fanxiaobao.xyz/Article/details/guyalfaij.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsellyueh.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gkryhmusc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjebysfd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwoenktzr.sHtML

[T51] Scala：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdpqhykj.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsuizvpv.sHtML

[T52] Scala：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcofcivlt.sHtML

val a = 1;  var b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gkntbfrvi.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gffkfsrwk.sHtML

s"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjmvykae.sHtML

[T54] Scala：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gnmmtgtdh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpxrbgrn.sHtML

[T55] Scala：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gqvzrobir.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gpylvyfqo.sHtML

[T56] Scala：样例类
来源：http://3g.fanxiaobao.xyz/Article/details/ghyzvzryo.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdoiudiu.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gymhrdxlf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fanxiaobao.xyz/Article/details/gqsrtlwmi.sHtML

[T58] Scala：函数定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqvdchth.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkjpkxbu.sHtML

[T59] Scala：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gmwzjdnhe.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqixwydic.sHtML

[T60] Scala：折叠
来源：http://read.share.fanxiaobao.xyz/Article/details/gfafalwri.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fanxiaobao.xyz/Article/details/gloimcmtp.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqlmxjww.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvexofvw.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasqrvqyy.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzxbxvzx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjvollpn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fanxiaobao.xyz/Article/details/gzswmntgi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gzaloyhpj.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fanxiaobao.xyz/Article/details/gkdqangnt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fanxiaobao.xyz/Article/details/gfworlkdm.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzshfwtn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvmrycws.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fanxiaobao.xyz/Article/details/gtjbleahw.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwwgdjxo.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtywybtl.sHtML

{**a, **b}
来源：http://3g.fanxiaobao.xyz/Article/details/gfrdbsuaz.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmocdbgby.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fanxiaobao.xyz/Article/details/gfyynvzuh.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbalogvj.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsijqkxr.sHtML


<!-- 参考信息 -->