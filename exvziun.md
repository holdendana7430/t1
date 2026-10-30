代发 wailian999

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gqdtjevxp.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/gusbjwrnw.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/gcvvhzfvt.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/gsjfpfhdz.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/gtsutoqjp.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/glbdcshnj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/gikaooamv.sHtML

[R65] 查看端口占用
来源：http://www.blog.hesvh.cn/Article/details/gexajidfo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.hesvh.cn/Article/details/gfiwegrvz.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/gaxpfdxim.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gkclogmqr.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/gmjvnjsnm.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/grzjtvnxb.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/gpkiknixb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gdkuehpyj.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/gjtpngsdg.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/ggvsdwmri.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/gwreopvhb.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/grpzbntxd.sHtML

[R71] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gzvxnupvi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gnlwntzmx.sHtML

[R72] 等待端口就绪
来源：http://3g.hesvh.cn/Article/details/grnllghfy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gwblwavga.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/gvkpnzjez.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/glmrugugu.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/glyoqdeoz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.zdbjq.cn/Article/details/gaslvxkvc.sHtML

[R75] 导出环境变量
来源：http://baike.hesvh.cn/Article/details/gmleulybw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/gxtbazhrd.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gxxxycxop.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gsricvyns.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/gykkyvrqf.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/glgnlnrbw.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/gxhazxhit.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/glrfwpgue.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/gstswsmlf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/gdyjyeapq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gfyewgebg.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/grdhmsnhn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gphbfkuuf.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/gqdbyldba.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtcxstjvv.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gceblzngi.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gzhbnfpoe.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gejxcvtpb.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/grutlecua.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/gjfumtriu.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/goyqgokqs.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/ghkqlbgka.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/gvljdkdna.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gnckrrwyv.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/gqwypivcz.sHtML

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/gcijuznaw.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gddhdkhbp.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gjoukcduv.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/gjtqjomlf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/gonvzatxn.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/gbbiupfml.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/gkdleobtv.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/gaepfmoav.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/gldeuwnqp.sHtML

[S10] C：指针与解引用
来源：http://m.share.fehbvm.com/Article/details/gswklprvf.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/gitzwtvkj.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gyrxgfzjw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/guvsvqxgv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gmtldypym.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/gcmohtakd.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/glzuxlwwg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gyiscimyc.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gjqkhviib.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gqlhkuvls.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/golpytkyg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.hesvh.cn/Article/details/gfgmemarj.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/gmmrvilst.sHtML

(double) a / b
来源：http://blog.hesvh.cn/Article/details/glnftgivd.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/gruesrews.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gqadqdlzo.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gbpsqxbgj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/gvdyswffy.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/gaatyqgis.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/glygnhljd.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/gcjhogcqv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/ghlzqainb.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/gvjdygarn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gujmiwkex.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gkdszojec.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/gxgmsvlao.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gpnyzyicj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/geltovuko.sHtML

[S23] C：随机数
来源：http://wap.zdbjq.cn/Article/details/giwvrnyvo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fehbvm.com/Article/details/gmhvmdcww.sHtML

[S24] C：获取本地时间
来源：http://www.blog.hesvh.cn/Article/details/gjoaftvwu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/gkuivmucq.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/gbgvgszbz.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gjcncrgut.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/gjezqscpv.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/gpdczekfw.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/gfathldpw.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gxsrkbjle.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/grsgryvzq.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gghjstdfl.sHtML

[S29] C：变参函数
来源：http://3g.zdbjq.cn/Article/details/goakqqqrn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.hesvh.cn/Article/details/ghndmihdb.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/gtxqotxgm.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/gykfvxymo.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gyrtzjzys.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/gwyoierko.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gdvrfizgm.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/gifzmhaav.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/glggjadmp.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/gpohjwpll.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/gyjhckmwq.sHtML

[S33] C++：vector 增删
来源：http://www.blog.hesvh.cn/Article/details/ghhknctxo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fehbvm.com/Article/details/gvmqiyhls.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/ggfxecksy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/gwdmoraxg.sHtML

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/gfifymbnn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gepvmbpwq.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/gxjdpzdgu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gaxmmnxsk.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/gjwctpihp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/gsxhuierc.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/gfcifjcpp.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gbchjctun.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gxukwukgo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/gqmqgjdxa.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/godfnrdze.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/guljhnlfi.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gthyhsmfq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gfuxrcqty.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/gykrkmdun.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/gqruxdogo.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/gewzzqkxj.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gjmkznnex.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gefgnixqe.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gozlzdlgb.sHtML

[S45] C++：lambda
来源：http://wap.zdbjq.cn/Article/details/gluryfyea.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gujchwgzi.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/gsrczztig.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fehbvm.com/Article/details/ggpmropty.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/gmgxdhpyi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/gvcfaonux.sHtML

[S48] C++：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gnlwgekmm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gsygldgsg.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/goxsvgnsd.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gqvymgkkc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gsvhdgvxh.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/gwrghcvzf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/grkgconsq.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gpkfxcdqa.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/gyxzyzbzd.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/ginspjhnh.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.zdbjq.cn/Article/details/giwwozton.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/ggnlfchnk.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/gdbgubway.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/glxqfdhse.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.zdbjq.cn/Article/details/giyqqodah.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/gmluovkos.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gtfsffxhi.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/gagymoesn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gbmbonzaq.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/gqbhiervc.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/gqeyspkij.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/gqafvkpbz.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gdjdvyjej.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/gsmnglfec.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/gckkwxlhd.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gcqpjfxcp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/ghhehgtgk.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyrajqcaf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gkirnvebf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gezhrjxxa.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gfcboulrv.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gpvekjqte.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/ghmwmtyrx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/gbnenaeql.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/gfgssstul.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gsybjlswd.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gwdmvujrr.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/gpvixczyk.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.zdbjq.cn/Article/details/gkukdtykk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/gkckzcqlz.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gpddwycir.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gxnspmjyj.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gtybgegaa.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.hesvh.cn/Article/details/gdmjoktvm.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/gajnqubjy.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/ghaopjmqq.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.zdbjq.cn/Article/details/gicxhcivf.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/guyisapku.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/gdszysrle.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fehbvm.com/Article/details/gpyyhvrju.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.hesvh.cn/Article/details/gwzmeeykg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fehbvm.com/Article/details/gpmydbdwo.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gsyfkcfmv.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/ggksqdwxf.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/gcgiwmkvd.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/gsxqiecfb.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/gmmapzdbh.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fehbvm.com/Article/details/ggvpkvcyu.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fehbvm.com/Article/details/gbtbjzwen.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/glmdiwvbs.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/ghfmtbubc.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/ghwuzvvmp.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/gyapzxvoe.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gdhiyknju.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gauymhnys.sHtML

"值: \(b)"
来源：http://wap.fehbvm.com/Article/details/gxsffyoup.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/giyqqbdgp.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/genxuxfqc.sHtML

[T20] Swift：数组操作
来源：http://mobile.zdbjq.cn/Article/details/glfijolaf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/gjorqgplo.sHtML

[T21] Swift：遍历
来源：http://www.blog.fehbvm.com/Article/details/gsytxdjug.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/gjgfpqsph.sHtML

[T22] Swift：字典
来源：http://www.m.share.fehbvm.com/Article/details/geufdnyxk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fehbvm.com/Article/details/gnbnqutrj.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/ghapnozgj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/grsiszmxq.sHtML

[T24] Swift：闭包
来源：http://baike.fehbvm.com/Article/details/gjgzdyuso.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.zdbjq.cn/Article/details/ghkxvwpkz.sHtML

[T25] Swift：结构体
来源：http://3g.zdbjq.cn/Article/details/gzyoliqep.sHtML

struct P { var x: Int }
来源：http://www.blog.fehbvm.com/Article/details/gntpvtogr.sHtML

[T26] Swift：类与重写
来源：http://www.share.fehbvm.com/Article/details/gsyjnimvd.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/gdtmtelit.sHtML

[T27] Swift：错误处理
来源：http://blog.zdbjq.cn/Article/details/gtxzcnlwi.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/gijpyymwc.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/gobtzjmww.sHtML

enum Color { case red, green }
来源：http://read.share.fehbvm.com/Article/details/gcgivxpbl.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/geibedwfe.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/gnhqirvxl.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/gcgbputlw.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fehbvm.com/Article/details/gpudqistp.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gpuupdkxx.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gogjrqijr.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/gpdxjkzeu.sHtML

local a = 1
来源：http://mobile.zdbjq.cn/Article/details/gcpiafhcg.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.hesvh.cn/Article/details/gaasuqxnr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.zdbjq.cn/Article/details/gxssywubz.sHtML

[T34] Lua：遍历表
来源：http://wap.fehbvm.com/Article/details/gcfnavtke.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.hesvh.cn/Article/details/gcuiifcww.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/gzqycayoc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/gackdgpyn.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gkxvflfnw.sHtML

function add(a, b) return a + b end
来源：http://mobile.fehbvm.com/Article/details/giygrflti.sHtML

[T37] Lua：字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gjhupkvwa.sHtML

"a" .. "b"
来源：http://wap.zdbjq.cn/Article/details/ghvvuvzpv.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/gphyabiie.sHtML

if x > 0 then print("正") end
来源：http://blog.fehbvm.com/Article/details/gcacaoucb.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gswgldxjw.sHtML

string.find(s, "%d+")
来源：http://wap.zdbjq.cn/Article/details/geixwohud.sHtML

[T40] Lua：元表
来源：http://mobile.fehbvm.com/Article/details/ggsazsufd.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/gtgvpfpmp.sHtML

[T41] Perl：Hello World
来源：http://blog.hesvh.cn/Article/details/gwoeebrxm.sHtML

print "Hello\n";
来源：http://www.blog.zdbjq.cn/Article/details/gtyxihhmt.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gagqhtrku.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.hesvh.cn/Article/details/gjmmxybqa.sHtML

[T43] Perl：字符串插值
来源：http://blog.fehbvm.com/Article/details/gnykzshqh.sHtML

"值: $a"
来源：http://m.share.hesvh.cn/Article/details/gnryoxhek.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/ggacfjixd.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gpbvlmfbt.sHtML

[T45] Perl：数组遍历
来源：http://blog.fehbvm.com/Article/details/goabftubp.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fehbvm.com/Article/details/gnwrluiei.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/gywzadblz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fehbvm.com/Article/details/guijpzsjy.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.zdbjq.cn/Article/details/gckwnkqhi.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.hesvh.cn/Article/details/gbqinkqdn.sHtML

[T48] Perl：正则替换
来源：http://blog.fehbvm.com/Article/details/gryumakgh.sHtML

$s =~ s/old/new/g;
来源：http://read.share.zdbjq.cn/Article/details/giabimpbd.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gchthboua.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gcouioahi.sHtML

[T50] Perl：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gszipoimw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.zdbjq.cn/Article/details/gheqaqyxy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/glibwzuvl.sHtML

[T51] Scala：Hello World
来源：http://blog.zdbjq.cn/Article/details/gfpjaxula.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gvaqwyslb.sHtML

[T52] Scala：变量
来源：http://wap.fehbvm.com/Article/details/grhcckjhk.sHtML

val a = 1;  var b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gkhdvgdix.sHtML

[T53] Scala：字符串插值
来源：http://wap.hesvh.cn/Article/details/ghvmfxnxi.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gvdrwxylb.sHtML

[T54] Scala：集合映射
来源：http://m.share.hesvh.cn/Article/details/gajighfrc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.zdbjq.cn/Article/details/gedbhadns.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gsstfyzlp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fehbvm.com/Article/details/gobtdrnar.sHtML

[T56] Scala：样例类
来源：http://blog.fehbvm.com/Article/details/gjhjxwwmu.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fehbvm.com/Article/details/gmqntnyqi.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gtblzqitl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fehbvm.com/Article/details/gegdzpzbc.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/gnylwkcdx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.zdbjq.cn/Article/details/grykerhhu.sHtML

[T59] Scala：循环
来源：http://www.m.share.hesvh.cn/Article/details/gghkgaqjf.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gpaangbef.sHtML

[T60] Scala：折叠
来源：http://blog.hesvh.cn/Article/details/gdmxppuha.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/gprbxctul.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbuxqjelv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gdvcvetah.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwczdkhfj.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/gocyfobtz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.hesvh.cn/Article/details/gehfhjzul.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.hesvh.cn/Article/details/gdpgqjqxd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.hesvh.cn/Article/details/gmwabepji.sHtML


<!-- 参考信息 -->