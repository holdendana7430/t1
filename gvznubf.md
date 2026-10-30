代发 wailian999

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/gwjakxzze.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/gpecxfyaq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/grmbayimv.sHtML

[R65] 查看端口占用
来源：http://www.m.share.zdbjq.cn/Article/details/gmpypykqt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/gkblxpxmr.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/gtqeqveew.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/gkzqqsevu.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/gvnwjtldn.sHtML

openssl rand -hex 16
来源：http://baike.zdbjq.cn/Article/details/gyeinelez.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gpscksgdw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.hesvh.cn/Article/details/gvnqjbvkj.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/gzdbsmzoj.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/gypitxydn.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/gqjjgevsu.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/ggrsjdztg.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gqrauxkgz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fehbvm.com/Article/details/gngoksawz.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/gunbqzroe.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gcssayuky.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gswyaevqm.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/gnuawihkd.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/gwodturwl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/gcavfroor.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/gmcuhitlf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gvngajlbf.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/gliigsske.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gurngvpmt.sHtML

[R77] 读取用户输入
来源：http://m.share.fehbvm.com/Article/details/gjnbkgqlj.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gnjaanslf.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/gnvabyerj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gujnxdyzx.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/gwgreewur.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fehbvm.com/Article/details/glvekclau.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fehbvm.com/Article/details/gxxzjbwuu.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/gvyhhysfa.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwjzwdxek.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/gnxzxpcta.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtxzjhgzc.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gqkabqzif.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/gwktdufvg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/glbbguqsj.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/gfzirwvau.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.hesvh.cn/Article/details/giccsdych.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/gsdclsrbk.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/ghsdswekc.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gmwqtivsy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/grcyglvgy.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/gvhzebcfv.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/galzpknqf.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/gnxiczako.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/gurrlpjts.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/gxaqfbsid.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/gbkihndnu.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/ggtfeenzy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/griiotzqr.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/gxeyluugj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/gpxwlcung.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/ghnllgacv.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/gsoabpgyk.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/glofvuybx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/gysppvblp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gbxblqled.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gbesdbbud.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/gilvoaeox.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gnxwhsbfe.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gisvitdxs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/gbbvqjvyb.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/gvjnabvne.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/gwmdysjln.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/gkdjkmyml.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/gdlhhysvc.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/guffauype.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gvembijfs.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gyzyeiuqp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/gyhkfmxwd.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/gcqbmnlfz.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/girwdsxfr.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gkslkqcpc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gttbssztt.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gpmggpjxt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/guwdhzerm.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gqlnfjugs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/gxujcevyj.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gxvsqxbiv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.hesvh.cn/Article/details/gtmwzlogy.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/gnerejmhg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gktsamhhb.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/guzblliyi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/grxvsgkcv.sHtML

[S25] C：内存拷贝
来源：http://mobile.hesvh.cn/Article/details/gxvdvfliu.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gffzehouc.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/gwdtsjyra.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/gqpvzbxvf.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/gscepfapu.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gxwskzjmv.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/gzhxjpend.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/gzqynkhyn.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/ghzzwbrfe.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fehbvm.com/Article/details/gmmuevjpu.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gmxjxrvce.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gtxwiukvh.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gmtnonmgg.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gdmfgxcvc.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/geotqygtu.sHtML

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/gcrerzzcc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/gmwwvuthv.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/gssrjzudx.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/goviayvpa.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/gbczaowgn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fehbvm.com/Article/details/gqnlnkvrl.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/gwovgbqie.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/gdodmvqjd.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/gpjcxhipc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gzpvnkmcu.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/guyzldrpt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gevdwwvfm.sHtML

[S37] C++：set
来源：http://blog.hesvh.cn/Article/details/gctajjjaq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.hesvh.cn/Article/details/gqozwsyof.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/ghfeczqgc.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gvgxejowq.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/gdgpfyrkp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gcsbebbcq.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/grfcxegwy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gupcyjeuq.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gviixudnj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/gvoaqwdsl.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/gmbnqlfte.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/gtmnqpckw.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gtblpcmwj.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gvusntrzm.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gqazdiabj.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/gfqpdmncy.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/gtpqguajm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/gnietbahn.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/gidwynged.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/gdtozskib.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/gshsvblpc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gtfurhzqa.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gjlbbvgpa.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/gwugtvxea.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fehbvm.com/Article/details/ghqvqtwfj.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gghmhkdcn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gdxsmsiji.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/glrigpqfi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gdlgfanka.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/gbpumzyqk.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/gzmqmccfv.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/gxprmxmmg.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.zdbjq.cn/Article/details/gdcmteowu.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/gjthjeqvt.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fehbvm.com/Article/details/gdyfqzfmf.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/guixmtcrt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/giqusffps.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/gzylamnsj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/ginrqqucl.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/gpsbdquay.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/ggiwzpjny.sHtML

[S57] C++：编译期常量
来源：http://read.share.fehbvm.com/Article/details/gmlvibzrs.sHtML

constexpr int N = 10;
来源：http://baike.fehbvm.com/Article/details/gdrsutpdc.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/glrofztwl.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/gjguyqens.sHtML

[S59] C++：静态断言
来源：http://mobile.hesvh.cn/Article/details/gbhjmqlum.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/ggynyihmu.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gllimpdrf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gdpkwifsz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcjmsgtzr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gsepxnywp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/guhbiafdi.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/geohjylza.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gkvdzlsdp.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/gwwrlfbpk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/gdolfsvbx.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gpibjzxcm.sHtML

"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gglxakksz.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/guxaavxuq.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/gjmhbkiub.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fehbvm.com/Article/details/gzyfhwtsp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.hesvh.cn/Article/details/ggkzzwggd.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/gfniubwqx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/gtmygtzbw.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gkbwjjiqd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/gurzoxsak.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/gtkxorbuf.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/gnjflebqz.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.zdbjq.cn/Article/details/gbdwsxzrq.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/ghirttard.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/gdtbdlvgg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/glegioqep.sHtML

[T11] Kotlin：协程
来源：http://3g.fehbvm.com/Article/details/gflqqloqi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fehbvm.com/Article/details/ghxskpxkw.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gnftuklkz.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fehbvm.com/Article/details/girgpitkl.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fehbvm.com/Article/details/gowlezzfi.sHtML

val m = mapOf("a" to 1)
来源：http://3g.zdbjq.cn/Article/details/gzklfojem.sHtML

[T14] Kotlin：循环
来源：http://m.share.fehbvm.com/Article/details/gbcjkgccj.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gjvomvnoc.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gngbhfhnt.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fehbvm.com/Article/details/gvjhxmtpt.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gljeyshbf.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gyllqxyrx.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/gzfxjekdm.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/gekdjvrnr.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/ganjbfvwt.sHtML

"值: \(b)"
来源：http://read.share.fehbvm.com/Article/details/ggzqflnsh.sHtML

[T19] Swift：可选绑定
来源：http://3g.hesvh.cn/Article/details/gkljipdlc.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/gbwnqixma.sHtML

[T20] Swift：数组操作
来源：http://3g.hesvh.cn/Article/details/gkmhmewty.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fehbvm.com/Article/details/giiobgbhd.sHtML

[T21] Swift：遍历
来源：http://wap.hesvh.cn/Article/details/gesdagfwy.sHtML

for x in a { print(x) }
来源：http://blog.zdbjq.cn/Article/details/gfntosnbd.sHtML

[T22] Swift：字典
来源：http://read.share.zdbjq.cn/Article/details/gcjpgsyrx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.hesvh.cn/Article/details/gqcfezqbf.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gqwnvjdpv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/ggitjqasb.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/gdgbjmbnw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.hesvh.cn/Article/details/gbspdkdyo.sHtML

[T25] Swift：结构体
来源：http://3g.zdbjq.cn/Article/details/gprprjybn.sHtML

struct P { var x: Int }
来源：http://m.share.fehbvm.com/Article/details/gcgkwmhiz.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/glbjsjpki.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/gcvvtqcal.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/grtvqohoy.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/gafeipldp.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/guybdnfbg.sHtML

enum Color { case red, green }
来源：http://www.m.share.fehbvm.com/Article/details/gzkoupltl.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.zdbjq.cn/Article/details/gaomhwmxk.sHtML

guard let x = opt else { return }
来源：http://baike.zdbjq.cn/Article/details/gvkooghpr.sHtML

[T30] Swift：协议
来源：http://mobile.fehbvm.com/Article/details/giobprwof.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.hesvh.cn/Article/details/gluidfhxh.sHtML

[T31] Lua：Hello World
来源：http://mobile.fehbvm.com/Article/details/gvnypydfn.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gqmvvhtke.sHtML

[T32] Lua：局部变量
来源：http://www.share.fehbvm.com/Article/details/guumvdbub.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/guzvujkwy.sHtML

[T33] Lua：表（数组）
来源：http://mobile.zdbjq.cn/Article/details/gyzrnsoaq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.zdbjq.cn/Article/details/gwahnmuqb.sHtML

[T34] Lua：遍历表
来源：http://mobile.hesvh.cn/Article/details/gqihtqebu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/genoeeann.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/grwzqdbkj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/gvxihpzyk.sHtML

[T36] Lua：函数
来源：http://blog.zdbjq.cn/Article/details/gyozfjhfp.sHtML

function add(a, b) return a + b end
来源：http://wap.fehbvm.com/Article/details/gpnoytqqx.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/glsfxipse.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/gbnndamsc.sHtML

[T38] Lua：条件
来源：http://3g.zdbjq.cn/Article/details/guadadwtg.sHtML

if x > 0 then print("正") end
来源：http://blog.hesvh.cn/Article/details/gwkwuvnqe.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gjeevoebx.sHtML

string.find(s, "%d+")
来源：http://baike.zdbjq.cn/Article/details/gfsbhbqiq.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/geysvcapr.sHtML

setmetatable({}, { __index = base })
来源：http://blog.hesvh.cn/Article/details/giorzjuji.sHtML

[T41] Perl：Hello World
来源：http://www.share.fehbvm.com/Article/details/gktmghihe.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/gmpoykuzp.sHtML

[T42] Perl：变量类型
来源：http://read.share.zdbjq.cn/Article/details/gpbtrcdht.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.zdbjq.cn/Article/details/grovfmaof.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gzfyfztqq.sHtML

"值: $a"
来源：http://www.m.share.hesvh.cn/Article/details/gvcmdyhim.sHtML

[T44] Perl：条件
来源：http://wap.fehbvm.com/Article/details/ginoocpkt.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/gtjqadpgc.sHtML

[T45] Perl：数组遍历
来源：http://read.share.hesvh.cn/Article/details/gndgfasif.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.zdbjq.cn/Article/details/gmwegrfbr.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.hesvh.cn/Article/details/gmbgiwxmv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.hesvh.cn/Article/details/gwpltekss.sHtML

[T47] Perl：正则捕获
来源：http://baike.hesvh.cn/Article/details/gdbmtvwdd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fehbvm.com/Article/details/glmrkocyz.sHtML

[T48] Perl：正则替换
来源：http://blog.fehbvm.com/Article/details/gyzwgznfy.sHtML

$s =~ s/old/new/g;
来源：http://baike.fehbvm.com/Article/details/ghagawhrp.sHtML

[T49] Perl：函数
来源：http://www.m.share.hesvh.cn/Article/details/goytxhvhy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/geycagbcp.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gnlamtyos.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fehbvm.com/Article/details/gkxgxnyrm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fehbvm.com/Article/details/gduezapen.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gqkuseonv.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gjezezezu.sHtML

[T52] Scala：变量
来源：http://read.share.zdbjq.cn/Article/details/gwujpsjnw.sHtML

val a = 1;  var b = 2
来源：http://m.share.hesvh.cn/Article/details/gbtpfuwey.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gwajzjrmm.sHtML

s"值: $b"
来源：http://wap.hesvh.cn/Article/details/ggifmnhdf.sHtML

[T54] Scala：集合映射
来源：http://wap.zdbjq.cn/Article/details/gsnvdahpt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.zdbjq.cn/Article/details/gfqrwkdzk.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gxbztczfh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.zdbjq.cn/Article/details/getsgoubu.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/gdvtrring.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fehbvm.com/Article/details/gucsegvyu.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gogijwgdl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fehbvm.com/Article/details/grrruetsp.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/guknzonei.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fehbvm.com/Article/details/gfeifntkl.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gduukisdj.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.hesvh.cn/Article/details/gqttunjtw.sHtML

[T60] Scala：折叠
来源：http://3g.zdbjq.cn/Article/details/gkegezqhm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fehbvm.com/Article/details/garqzjale.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzbruszlt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/grvrgpfzx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnxbhfseu.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.hesvh.cn/Article/details/gvglomfwq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fehbvm.com/Article/details/gcrmhvgkm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fehbvm.com/Article/details/glumtlkga.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.hesvh.cn/Article/details/gkmssgnlb.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fehbvm.com/Article/details/gjivnutwt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.zdbjq.cn/Article/details/gubtyrvbk.sHtML

[U04] Py：变量调试打印
来源：http://3g.zdbjq.cn/Article/details/gxksmxvmm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fehbvm.com/Article/details/gtdsqneke.sHtML


<!-- 参考信息 -->