代发 wailian999

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/gxmvtimsy.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/govxxonqs.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.hesvh.cn/Article/details/gboboecyl.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/gosnchzef.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fehbvm.com/Article/details/gyhjdnxzg.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gzhnfbhxv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fehbvm.com/Article/details/grkcmshzn.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/giquljohj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/gciiwwahu.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gkclsgfha.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.hesvh.cn/Article/details/gbjizuqtl.sHtML

[R67] 生成随机十六进制串
来源：http://wap.hesvh.cn/Article/details/gavaqtxjm.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/grjldutes.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/gydcuuogg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/gfppgkibt.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gozkopraw.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/gcrbfufmf.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gwsmtzbso.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/gjkwnumio.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/grolouops.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gekgvtwpn.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/ggqfjjxaq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gfrflrxkf.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gnzazpldc.sHtML

split -l 1000 big.log part_
来源：http://m.share.zdbjq.cn/Article/details/gfqjzrjhi.sHtML

[R74] 批量重命名
来源：http://www.blog.fehbvm.com/Article/details/gfzdkbxsq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gwcnfksfr.sHtML

[R75] 导出环境变量
来源：http://blog.fehbvm.com/Article/details/gwielznru.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/gbddtzldo.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gmtykliuv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gihorsdqm.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gclpkhwea.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gvmqnngna.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/gvbtqrjig.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gpvmwefmq.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gsepsdskk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/gjfhqbmjc.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/gabzxzfxy.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/gzymmsixl.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxmaduqet.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/gfttmleoc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtqgvboaq.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/gtknvqnmo.sHtML

#include <stdio.h>
来源：http://read.share.fehbvm.com/Article/details/gdylmtomr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gbumyuplg.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gihdpimqm.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/gkjwzaspc.sHtML

[S03] C：读入整数
来源：http://mobile.fehbvm.com/Article/details/glsauvxwv.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gaytilzlq.sHtML

[S04] C：字符串复制
来源：http://mobile.fehbvm.com/Article/details/gjcloeczk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.hesvh.cn/Article/details/ggrmhsyfw.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gmfvuwszf.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/godbriefb.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/gablnxqml.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gufpqiamr.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/ghwbzqpqy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/ghlppdses.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/gemunmync.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/gempvxnaa.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/gglgwacgf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fehbvm.com/Article/details/gghnpxvbh.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gmdrqlkks.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/gtiybsade.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gibhajuio.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gwgrjqtis.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/gjpytasnh.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/ghadxhaih.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/ganzmyjbu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gclcuvpwq.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gqwrvucfr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/gkygckznm.sHtML

[S14] C：枚举
来源：http://wap.hesvh.cn/Article/details/gponsyshd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/ggukerprt.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/gcddpbafx.sHtML

(double) a / b
来源：http://m.share.fehbvm.com/Article/details/gvnrlezer.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/geyupcqpx.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/gkhvggcyz.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gmcllsyzt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/govsuawbw.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gbczzbajq.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/gryypqsni.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/guviacpfl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gminwimsx.sHtML

[S20] C：二分查找
来源：http://wap.hesvh.cn/Article/details/gpxwyeopl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gubmlunie.sHtML

[S21] C：字符类别判断
来源：http://www.share.fehbvm.com/Article/details/gkyboqpky.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fehbvm.com/Article/details/gfqgclfgq.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gsrjmuoru.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/guwqhwduo.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/gigiiuxoz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fehbvm.com/Article/details/grnueufbj.sHtML

[S24] C：获取本地时间
来源：http://wap.zdbjq.cn/Article/details/grrqpkelt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fehbvm.com/Article/details/gxprbtwxh.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/gyvklsgds.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/gowpsydpc.sHtML

[S26] C：内存清零
来源：http://wap.hesvh.cn/Article/details/gouadwwur.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/glbsesgyh.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/ggxpjeaet.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gvqdjcxsz.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gozjoklel.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/getoncjhr.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/gjhksbwfd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gzbqzvwqn.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gicjwttre.sHtML

#ifndef X_H
来源：http://3g.hesvh.cn/Article/details/gkkqlmdte.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/gwdvvsfkp.sHtML

#endif
来源：http://m.share.hesvh.cn/Article/details/gmbhaqjjg.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/gnjekqksa.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/gtovsmgmc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.hesvh.cn/Article/details/gtdfyxjtm.sHtML

[S32] C++：字符串
来源：http://baike.fehbvm.com/Article/details/glibgbojd.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/gyyzomucd.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gqvbkeqcd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/ggiuxqsfx.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gbjvygqnh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gfbohdgxs.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/gkhvlmkjt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/grjtmcmgb.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/gaqiemvsm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gmgxvwgmw.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gczdvbfty.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.hesvh.cn/Article/details/gpdcbsayg.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gtaomstpo.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/geolgznzj.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gcbiulrkq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gmudroyeb.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/gwnovcedb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/gtjoxqxcj.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gjawnamkm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/gzopblvnt.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/gjgfzlree.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/gdoovqhma.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/gbhnqrltx.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/gdmyumxpu.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/ghhbqzulj.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/glotlnrbf.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/grgvaayqi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/gyebmofou.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/grkxjvduc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/gwdaqgvsx.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/gfzhhwcvb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/gecowqplh.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gpbgaoctk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/gatarrljb.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/gslcdvbai.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gwnuenbcn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gtrwexzuf.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fehbvm.com/Article/details/gncizjcsx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gbdsltuyc.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/gccidshjn.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/gwyrkislk.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/gxdjyiplb.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/gltrxobli.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/gmqwlkbwj.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/gshfupvyb.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/gseohxkfz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gxbwdpqko.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/gmgqwylis.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gfgtpzmqs.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/ggtdastfw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/gglinbnim.sHtML

[S57] C++：编译期常量
来源：http://read.share.fehbvm.com/Article/details/gbkybwaco.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gapvijhad.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/gaigexwmt.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/geigetcgj.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/glotzwbyz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/gwdblesiz.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/gxmtvahap.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gaugomhsa.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjwkhzwuo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gpidbuxfw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gujjmkoth.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gkrdvtcvw.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gpsjeyypm.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/gchfnvmxl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.zdbjq.cn/Article/details/geqzcxtbc.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.zdbjq.cn/Article/details/gtplrqdkn.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gibbfwllk.sHtML

[T04] Kotlin：空安全
来源：http://baike.hesvh.cn/Article/details/gxhgyotuf.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/gbeqbksai.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/gefqkgmru.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.hesvh.cn/Article/details/goqhlbeou.sHtML

[T06] Kotlin：集合映射
来源：http://baike.hesvh.cn/Article/details/gsqojgxpo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/ghvzxuotx.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gvdschqwd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.hesvh.cn/Article/details/gowdqfdmx.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/gmhzriarn.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gnqvavzsc.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/ggapsqdxg.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/gfjovgeic.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/gjbfafslz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/gfyliavcg.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/gdpwteexy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/grnldgcmr.sHtML

[T12] Kotlin：解构声明
来源：http://wap.zdbjq.cn/Article/details/ghwuvyeop.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.hesvh.cn/Article/details/ggqradmhc.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/ggftwflfe.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/grcegllmv.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/gyhmgkypb.sHtML

for (i in 1..10) println(i)
来源：http://3g.fehbvm.com/Article/details/gkhrydmzh.sHtML

[T15] Kotlin：接口
来源：http://3g.fehbvm.com/Article/details/gokjxfkfh.sHtML

interface Shape { fun area(): Double }
来源：http://blog.zdbjq.cn/Article/details/gdnzhdsgg.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/gksguslfs.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gqtpivftb.sHtML

[T17] Swift：变量与常量
来源：http://www.share.hesvh.cn/Article/details/griryulzv.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gteurzmov.sHtML

[T18] Swift：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gpwrqrcfy.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/gjezhroum.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gaxejomov.sHtML

if let n = opt { print(n) }
来源：http://3g.fehbvm.com/Article/details/gbyqlmdkq.sHtML

[T20] Swift：数组操作
来源：http://3g.hesvh.cn/Article/details/gacyvljpb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.hesvh.cn/Article/details/gxzrrejjg.sHtML

[T21] Swift：遍历
来源：http://3g.zdbjq.cn/Article/details/gyndqvnda.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/gryddkbsp.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/giyesytvb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.zdbjq.cn/Article/details/gdtiffeax.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/gwrwzmqlm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/gvdqksctd.sHtML

[T24] Swift：闭包
来源：http://www.share.zdbjq.cn/Article/details/gbaizguka.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/glnqvwdrf.sHtML

[T25] Swift：结构体
来源：http://blog.fehbvm.com/Article/details/glmxjbnqj.sHtML

struct P { var x: Int }
来源：http://blog.zdbjq.cn/Article/details/glakkzbkb.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.hesvh.cn/Article/details/ghokadpqx.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/gbesldhgr.sHtML

[T27] Swift：错误处理
来源：http://baike.fehbvm.com/Article/details/gntgnzefq.sHtML

do { try f() } catch { print(error) }
来源：http://baike.zdbjq.cn/Article/details/gfreljfgk.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/glbbncbtn.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/gctjcgvap.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.zdbjq.cn/Article/details/gkaznaqpq.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/gbuwbtvtb.sHtML

[T30] Swift：协议
来源：http://read.share.fehbvm.com/Article/details/ghgdzfwcq.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.zdbjq.cn/Article/details/gkeirvulv.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/gtprxrosf.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gjqwmuxek.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/gktzyenyz.sHtML

local a = 1
来源：http://www.share.fehbvm.com/Article/details/gwkboavtx.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/ghxdldjkb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.zdbjq.cn/Article/details/gevswxkmn.sHtML

[T34] Lua：遍历表
来源：http://www.share.fehbvm.com/Article/details/gunmxlfot.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/gsrijchzg.sHtML

[T35] Lua：字典表
来源：http://wap.fehbvm.com/Article/details/glipakhcf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fehbvm.com/Article/details/gwvgsqvad.sHtML

[T36] Lua：函数
来源：http://m.share.zdbjq.cn/Article/details/gmdygmlhk.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.hesvh.cn/Article/details/gtduntjxq.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/getbxcuax.sHtML

"a" .. "b"
来源：http://www.m.share.hesvh.cn/Article/details/goatgoqpp.sHtML

[T38] Lua：条件
来源：http://www.m.share.fehbvm.com/Article/details/gieetpbks.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/gjniheiyy.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gcprfdoil.sHtML

string.find(s, "%d+")
来源：http://blog.fehbvm.com/Article/details/gdcczxjue.sHtML

[T40] Lua：元表
来源：http://wap.zdbjq.cn/Article/details/gtlclevkr.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.hesvh.cn/Article/details/gujdghwmn.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/grlfaovdb.sHtML

print "Hello\n";
来源：http://www.m.share.fehbvm.com/Article/details/goryxkkov.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/gctuqcnqs.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fehbvm.com/Article/details/gwbfjmrll.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/guwxqtfad.sHtML

"值: $a"
来源：http://baike.fehbvm.com/Article/details/gioknhewc.sHtML

[T44] Perl：条件
来源：http://read.share.fehbvm.com/Article/details/giezgsuoz.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/gtordcdiy.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.hesvh.cn/Article/details/grelxqgoh.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fehbvm.com/Article/details/gnwhygegg.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/ghwvttsev.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.hesvh.cn/Article/details/gkvbolshg.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/gwxkgkpry.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.hesvh.cn/Article/details/grenlkitd.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/gqldzypvc.sHtML

$s =~ s/old/new/g;
来源：http://baike.hesvh.cn/Article/details/gorlqxthl.sHtML

[T49] Perl：函数
来源：http://www.m.share.fehbvm.com/Article/details/gewmcbavn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gvcufmfof.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gqxdncrvk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fehbvm.com/Article/details/gcrghbegl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/glqeqeotm.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gnvqmkqtb.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gjvhgrvei.sHtML

[T52] Scala：变量
来源：http://www.blog.zdbjq.cn/Article/details/gruijllyk.sHtML

val a = 1;  var b = 2
来源：http://www.share.fehbvm.com/Article/details/gcgbbpipc.sHtML

[T53] Scala：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gbyomiydj.sHtML

s"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gbmpojlle.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/gmxvxbzpt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fehbvm.com/Article/details/gqrlquluq.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gvyoxqzxm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.hesvh.cn/Article/details/gutqvisnz.sHtML

[T56] Scala：样例类
来源：http://www.share.zdbjq.cn/Article/details/gbyrcscph.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gcudfzswy.sHtML

[T57] Scala：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gpjddhckb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.hesvh.cn/Article/details/gigrrdpkh.sHtML

[T58] Scala：函数定义
来源：http://wap.fehbvm.com/Article/details/ghbkzares.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/gemxvhota.sHtML

[T59] Scala：循环
来源：http://3g.hesvh.cn/Article/details/gpyqeqvkg.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.hesvh.cn/Article/details/gagqyyvad.sHtML

[T60] Scala：折叠
来源：http://baike.hesvh.cn/Article/details/gjwmbczbh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.zdbjq.cn/Article/details/guasypfug.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gyzlbgqyb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gzqbpuzyp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmpduykxl.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.hesvh.cn/Article/details/gcdeecjdv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/gjkgkwdky.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/gvoybtixq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.hesvh.cn/Article/details/gbjchrtuq.sHtML


<!-- 参考信息 -->