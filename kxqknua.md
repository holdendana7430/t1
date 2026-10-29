代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/gwvrnfzik.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/gqsjnxoot.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gojdxujyu.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/gecpcfane.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/gwhvnuvup.sHtML

[R68] 计算文件校验值
来源：http://blog.zdbjq.cn/Article/details/gjpjzncrn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/gkbjdrjeq.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/gmbanxuyz.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/ggwkvxryx.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/gwtcieflj.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/gfzoipjpn.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gudfnglbx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/ggubbkhgj.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gkomedjak.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gbgpaidgi.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/gfuvkmlyf.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gxeusfcdy.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gglsrbhub.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/glzdsshuq.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gmjnjpjhl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/gidwisgql.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/gayyfsjks.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gskwahdkw.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/gdpznhpls.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/gopecpcur.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/gohuiyzhq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gjutweqnu.sHtML

[R79] 解析命令行选项
来源：http://read.share.hesvh.cn/Article/details/gsebgjtyb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fehbvm.com/Article/details/gmrrjyati.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.zdbjq.cn/Article/details/ggictfvtu.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/gubpkndbn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpldqwmhb.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/gpolruhwf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gizksguaw.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/glsfnfuin.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/gusxlymhe.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/gvbioryuj.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/gypaonczs.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/ghweboale.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/gelxdicgh.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gufhddzkq.sHtML

[S04] C：字符串复制
来源：http://mobile.fehbvm.com/Article/details/guxhibjbo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/gaemuftgb.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/gbkhlfglq.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/gfpswgznb.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/giohfsaxo.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/gtzkhkwll.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/gnsgqxvpn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/gvwyziepa.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gmfcgqylr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fehbvm.com/Article/details/gyyruubpt.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/gdfvqdjsw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gxusbadlv.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gxoastfsm.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/gvtqtscfy.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gfnzvcbvv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/ggyerhhsk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gtnmmczvx.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gakpwflsk.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gnmytqvxx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gagnuckut.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gubirgxzu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.zdbjq.cn/Article/details/gulwzqrji.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/ganaqjqpq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/gqxihvboo.sHtML

[S15] C：类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gczwepuuv.sHtML

(double) a / b
来源：http://3g.hesvh.cn/Article/details/gwjpzvpfz.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/glrgkzunw.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/ghtxxkabi.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gtnysvjfd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gyprrnrtt.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gvvmjrfff.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/gbteiuzuk.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gohuusxso.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gdyyyybzq.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/gxucsmvzo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gakpbgswv.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/gebnszwnu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/gvxczzdse.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gjkwvggfe.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gxsoiecys.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/gxpninepl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/gaqqpbdss.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gsqegntvk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/gywzpfsag.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fehbvm.com/Article/details/gkjkkasbg.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/godhvfeij.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/gnqzlngeo.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gwosigvpe.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/gaqbqyzyl.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gaxruykex.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/ggrlbyyll.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/gbvkfcojh.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gdzduqgmk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/gbzbowlco.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/gvxvdnxgd.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/gwdryktnc.sHtML

#define X_H
来源：http://mobile.zdbjq.cn/Article/details/gozrvhkur.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/glmmukknt.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gkovktgyj.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gpvheclmd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/gccxexftx.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/ghwlixykp.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/gifrpiylg.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/ggxviqwih.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/gbfjzzenv.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/gihufmvvk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.zdbjq.cn/Article/details/gdlicslxt.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/ghlhexdgb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gheyhxiot.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gxluvhnql.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gafarhzov.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gcyeilcqf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.hesvh.cn/Article/details/gdgqjnuqx.sHtML

[S38] C++：排序
来源：http://www.blog.zdbjq.cn/Article/details/giponoyoo.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.hesvh.cn/Article/details/gtfucnvhh.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/gghfauzxo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/gcsrdzhua.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/ghtdfuzaj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/garebronc.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/gwhocffwc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/glvjpelqd.sHtML

[S42] C++：继承与虚函数
来源：http://wap.hesvh.cn/Article/details/gabtoegth.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/gbtpkbybn.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/gnxdyfqgv.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gdbsxjmww.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gmqqriiew.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/gthrgrgal.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/glsjftfqg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/ggibkoegk.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/grsxclqry.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fehbvm.com/Article/details/ggpzodgtx.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.hesvh.cn/Article/details/gnjclnfqn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gmcgwpukt.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gbgquatdc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/ggpfcfnqj.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/grnazievu.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/galgpzvrh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gluiujmyo.sHtML

[S50] C++：格式化数字
来源：http://wap.hesvh.cn/Article/details/gdgdscdod.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/grzeeajid.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/grpkinriu.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/gnitiglyu.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/grvoxxgui.sHtML

int size() const noexcept { return n_; }
来源：http://3g.hesvh.cn/Article/details/gbfgtqdet.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/ggabefdgt.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fehbvm.com/Article/details/gsgbtfkvm.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/gqljhglum.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gtrwqslqq.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/gidgnmjle.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/glaoruyed.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/gxhboqtks.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/glnrvmzlm.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gpvsfxmsv.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/galszoaxh.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/gsrcnwgwv.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/grwqsjuld.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/gnrkeajcs.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gtgubegjv.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/gqaeafhyp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gjomvvrbb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjwxmsmwf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/gxgqnfmqu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsiowbmss.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/gijtnntar.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/ggtznxvwh.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.hesvh.cn/Article/details/gjplateev.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.zdbjq.cn/Article/details/gbnvitrdc.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fehbvm.com/Article/details/gjkssegcx.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gbzgeatqc.sHtML

[T04] Kotlin：空安全
来源：http://wap.zdbjq.cn/Article/details/gyisvcwbi.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/gakxmioxo.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/giyzzvuch.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.zdbjq.cn/Article/details/gcqqltxoz.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/gbnxhnneg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/gvignzmpz.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gzoxuvapg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gzzfidgmi.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/grsnspvzn.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/gqzdxxrcf.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/glvtcxqlo.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fehbvm.com/Article/details/gykgcyjqr.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gpkkebnew.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/gpdaqrqqf.sHtML

[T11] Kotlin：协程
来源：http://www.blog.hesvh.cn/Article/details/gknpsojjw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fehbvm.com/Article/details/gjyqcfhkt.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/gocjtrsyp.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gynonnkmq.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/grtcunfmi.sHtML

val m = mapOf("a" to 1)
来源：http://baike.hesvh.cn/Article/details/gunhvohni.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/gijlozyuo.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gondfxnzg.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/gyuhrljit.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/ghgvzxzff.sHtML

[T16] Swift：Hello World
来源：http://read.share.zdbjq.cn/Article/details/ghlqdaddt.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gthifgjoe.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/grttusbqe.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gnotbgadc.sHtML

[T18] Swift：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gwjjifmti.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/gtekjnktc.sHtML

[T19] Swift：可选绑定
来源：http://wap.fehbvm.com/Article/details/gufabbtre.sHtML

if let n = opt { print(n) }
来源：http://baike.fehbvm.com/Article/details/grtauhbzd.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/gmhhapnrd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.hesvh.cn/Article/details/gsaujyiuk.sHtML

[T21] Swift：遍历
来源：http://m.share.fehbvm.com/Article/details/ggibxbygb.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/gsptpcjva.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/gnwnmupdd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/gphlrbjgi.sHtML

[T23] Swift：函数
来源：http://wap.zdbjq.cn/Article/details/gomqblsqk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.hesvh.cn/Article/details/gusmhukel.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/gwcuorgfp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fehbvm.com/Article/details/goqrzhslc.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/gossagtjp.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/geypexegx.sHtML

[T26] Swift：类与重写
来源：http://www.share.zdbjq.cn/Article/details/gzjjinhsi.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gplnuulfi.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/gcdrpmmxn.sHtML

do { try f() } catch { print(error) }
来源：http://3g.zdbjq.cn/Article/details/gpcfvqafu.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/gqoyfqejr.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/gkjdywyro.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/grttgredl.sHtML

guard let x = opt else { return }
来源：http://www.blog.hesvh.cn/Article/details/gaxdcnyso.sHtML

[T30] Swift：协议
来源：http://www.share.fehbvm.com/Article/details/guxrgzolp.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fehbvm.com/Article/details/gploonmfq.sHtML

[T31] Lua：Hello World
来源：http://3g.fehbvm.com/Article/details/gaatxtxjo.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gueaoodyo.sHtML

[T32] Lua：局部变量
来源：http://wap.fehbvm.com/Article/details/gdhqpkmuh.sHtML

local a = 1
来源：http://m.share.zdbjq.cn/Article/details/geeeocbzb.sHtML

[T33] Lua：表（数组）
来源：http://baike.hesvh.cn/Article/details/gzjtrmpaz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/grbnvtnyy.sHtML

[T34] Lua：遍历表
来源：http://mobile.hesvh.cn/Article/details/gmxgylkgz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fehbvm.com/Article/details/gvjignyti.sHtML

[T35] Lua：字典表
来源：http://www.share.zdbjq.cn/Article/details/ghnmuqbmu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/goopwpjnd.sHtML

[T36] Lua：函数
来源：http://baike.fehbvm.com/Article/details/gzupzpgqi.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/gtcwvoref.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gxmqsyoze.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/glvgqwhpt.sHtML

[T38] Lua：条件
来源：http://m.share.hesvh.cn/Article/details/gizimcxfw.sHtML

if x > 0 then print("正") end
来源：http://www.share.hesvh.cn/Article/details/gkzqiqhno.sHtML

[T39] Lua：模式匹配
来源：http://3g.fehbvm.com/Article/details/gsqsvastz.sHtML

string.find(s, "%d+")
来源：http://3g.zdbjq.cn/Article/details/gzduuleau.sHtML

[T40] Lua：元表
来源：http://mobile.zdbjq.cn/Article/details/gkngcyghd.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.zdbjq.cn/Article/details/gfaytszjs.sHtML

[T41] Perl：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gfqneuwst.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/gwamsplnq.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/glstynnkz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.zdbjq.cn/Article/details/goluijoar.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/giomfhqys.sHtML

"值: $a"
来源：http://baike.zdbjq.cn/Article/details/gaslxrrip.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/ggetvzyuw.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fehbvm.com/Article/details/gvelmtzwl.sHtML

[T45] Perl：数组遍历
来源：http://3g.fehbvm.com/Article/details/gohqstyzz.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fehbvm.com/Article/details/guwojkbhb.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/gapdgsqah.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.zdbjq.cn/Article/details/gbbotbpvw.sHtML

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/ggwprgntu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.zdbjq.cn/Article/details/gxeumxdra.sHtML

[T48] Perl：正则替换
来源：http://www.blog.zdbjq.cn/Article/details/gnkxpzwis.sHtML

$s =~ s/old/new/g;
来源：http://baike.hesvh.cn/Article/details/gjuavucjr.sHtML

[T49] Perl：函数
来源：http://www.share.hesvh.cn/Article/details/glmwkvfgx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/giqcvzrou.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gibcmmzyd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.zdbjq.cn/Article/details/gkfmxdhcj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.zdbjq.cn/Article/details/gqplkgnlx.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/glclxmkkn.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gjcksfdhg.sHtML

[T52] Scala：变量
来源：http://www.blog.fehbvm.com/Article/details/gmzztmesp.sHtML

val a = 1;  var b = 2
来源：http://baike.zdbjq.cn/Article/details/gycbbnmqa.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gumlqnyao.sHtML

s"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gixdhtnfi.sHtML

[T54] Scala：集合映射
来源：http://wap.zdbjq.cn/Article/details/gletkvqli.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.hesvh.cn/Article/details/gkepojgia.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gidftlymn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.hesvh.cn/Article/details/gtxtnuxte.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fehbvm.com/Article/details/gupvakasi.sHtML

case class User(name: String, age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gsnpfmnzf.sHtML

[T57] Scala：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gcpwrclli.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fehbvm.com/Article/details/gfxahgiwy.sHtML

[T58] Scala：函数定义
来源：http://mobile.hesvh.cn/Article/details/ghglhjjob.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/gvbvvnoll.sHtML

[T59] Scala：循环
来源：http://blog.zdbjq.cn/Article/details/gwucquyoj.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gvvtkxtif.sHtML

[T60] Scala：折叠
来源：http://m.share.fehbvm.com/Article/details/ghujwdutd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.zdbjq.cn/Article/details/gonjuyalq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gljnnmuwx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gvkualunm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gaewcborh.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/goaghxfih.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fehbvm.com/Article/details/gicursxxw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.hesvh.cn/Article/details/gzamkposn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/gmfmdfucb.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fehbvm.com/Article/details/ghicfmkhc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fehbvm.com/Article/details/gpribazal.sHtML

[U04] Py：变量调试打印
来源：http://www.share.hesvh.cn/Article/details/guueslobo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.hesvh.cn/Article/details/grloyguin.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/gcjjqoyop.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gyroaoyxo.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.zdbjq.cn/Article/details/gutixsjqo.sHtML

{**a, **b}
来源：http://www.m.share.hesvh.cn/Article/details/gywemuhlw.sHtML


<!-- 参考信息 -->