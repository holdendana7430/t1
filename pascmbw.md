代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/ghumdlroc.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/globxjnak.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gygzyqgel.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gmipwazyl.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gcjdmnmkj.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gbhcpfljw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gwoxmlgnh.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gnizvmtdy.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gskofsanb.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gnivqpbkf.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnymnesl.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/grzbeopzi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gcleaklit.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/ggdjvxvty.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/giosqzmgz.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gnebovhkf.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbkkrouj.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfdzpxkv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/grftvcspl.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gzquhkblj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gewfswgca.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmpasfzl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnficigk.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gslgsgjxn.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsdblojn.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gilqousad.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gworrkjbp.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkjqtqge.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggezkfsie.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvvvqjoz.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcsohewf.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gwzpozqam.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmhvgprx.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyunxjoq.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gstmscbdm.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gofwusfjp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpywnxed.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvojocgh.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/garlqqgrm.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmzvajek.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/geeaodrog.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpgqnkcc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gatyltnvy.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gdwwnfsmr.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvblurcpc.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gcxgodjkr.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gotkklthj.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gajiduofl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gklggkzdo.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gnorzygcr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gbwshagmw.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/ggqjfzvve.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbyxsogm.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gkkggwmrv.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/glkhxjgfl.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbydyqhk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gduqqgyhp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/giagwvbuf.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganzanvzd.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gavywnlio.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gonqyafov.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gjnxcwjad.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gsinwqdkx.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gynegdoba.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/giwcosifi.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gcoqrnadg.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/garzkdjmp.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gkvfwnzzw.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvghtxfc.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/guadgseow.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gnhgrhiec.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhdeazdp.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnaafitmj.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gfvuqmmaz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gzaeqzvoq.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gkvatldcd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gchbmowce.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/giawainef.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gxnawvrfk.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gpkofkjif.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupvfnxmg.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrrswwvu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gumyspoaj.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhwamhdv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzotqifyf.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgmsogsd.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmyapfjz.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxxuasta.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gifticlyg.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gwjgmgcjk.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/giejgsejc.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gftfgjtjf.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbvufomw.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwowxumy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gisihmaru.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/girxbnscl.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/ggloibwbt.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gcsvtpgct.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxbwvthc.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkztrugk.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlrwnjcu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuventba.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gnjkezukm.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpkkcgtr.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqzhejrc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzyuyyajh.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giiyibgnc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzevkycpq.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/goobbovid.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/glxmlzffr.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzdakekh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlixwwwq.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gezuvsqfq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvlwctvx.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gopaglfdd.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gcgxqktux.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzhuaxow.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyvmrplw.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gquuiofik.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gxiwkbmob.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/grrdwulte.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gnifbmbxv.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvvoepme.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/guqydjqjv.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gbldelcga.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gkuwilslf.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzvwpiem.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqblstiwf.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gloirbjfg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gawdsdcvn.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gdpyxbncv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamvjruhd.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gbgczrwtc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbscxsacn.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gejckhmtw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gkwpdnljn.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcozyoab.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gmefznzml.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gtymqknqm.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmyknqjz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gftentmpk.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glestczkx.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzchnioe.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstndvmmr.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhfpuefw.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/geltzmgsj.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwiulxab.sHtML

[S54] C++：异常处理
来源：http://wap.fanxiaobao.xyz/Article/details/gnwcjqqsp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gulgikwdf.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gpeokofqy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/geduqseiw.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/gasdywvjv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqikoskag.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gredazxrc.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxotdjrv.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkmxubut.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvchkqmk.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrqcedyf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdrkynvd.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlkcomue.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gjrwddaqh.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gehokcpwl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/grucplpmj.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gujaqdnbe.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/glbgmkkdv.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgjujabw.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpzciavk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmfzmrtu.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gttfkagsr.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfcpfzfm.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfcnnbpd.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gndruvkap.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsysygvi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsugoxqny.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlcykaxl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gzkzcbkfc.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gwltexlgv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdrzueks.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/ggdnidaqj.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gxcuuktha.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwwxvjfm.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/gjzdfolsb.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gabaoffou.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerbqgomb.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxidtcdj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyziijnvx.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gzblipvbb.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvbdgyjc.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gksgvvfby.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzgqwrzx.sHtML

[T14] Kotlin：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwprqfcz.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbcoscwr.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/gawadehuo.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxtaqoij.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gviyugsrb.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/glldlebyf.sHtML

[T17] Swift：变量与常量
来源：http://wap.fanxiaobao.xyz/Article/details/ggrubizdi.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gwtznnpuz.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxavracg.sHtML

"值: \(b)"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkonnsdxd.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gcljwajny.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gaeotszwi.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gopydfzzn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gobnuzmnq.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gfyhyekcn.sHtML

for x in a { print(x) }
来源：http://blog.fanxiaobao.xyz/Article/details/geeatwdeb.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvexcuzo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/ggimrcbwm.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gagejtdxr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmekzovm.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzzynnbx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/ggrbxvbfn.sHtML

[T25] Swift：结构体
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgahymwh.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnecgfsl.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkvbopwz.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/ghjoxrjwo.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwzqgbdl.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxncgcsb.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/guhiwcxmk.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/gxmejrzls.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gffsamwnq.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gfjapyttl.sHtML

[T30] Swift：协议
来源：http://m.share.fanxiaobao.xyz/Article/details/gawbfqpov.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gionswbra.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqczltjc.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxcnnckz.sHtML

[T32] Lua：局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpqsetof.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/gskqoxnky.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvvjupfs.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fanxiaobao.xyz/Article/details/gsioacyyd.sHtML

[T34] Lua：遍历表
来源：http://mobile.fanxiaobao.xyz/Article/details/gtieiyeir.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvvqmbrm.sHtML

[T35] Lua：字典表
来源：http://www.share.fanxiaobao.xyz/Article/details/givlibcje.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gupdabira.sHtML

[T36] Lua：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyybpnnzh.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/gwemyosqh.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gxqavkibw.sHtML

"a" .. "b"
来源：http://blog.fanxiaobao.xyz/Article/details/gxorkssra.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gsxdlsswx.sHtML

if x > 0 then print("正") end
来源：http://www.share.fanxiaobao.xyz/Article/details/gmswdftin.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/geayyeyml.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/ghlyongzz.sHtML

[T40] Lua：元表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjspuptf.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fanxiaobao.xyz/Article/details/gahblltnp.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkwohhxl.sHtML

print "Hello\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gxigcddkc.sHtML

[T42] Perl：变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gmdyzxati.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/grxvasuao.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjuhkcgy.sHtML

"值: $a"
来源：http://blog.fanxiaobao.xyz/Article/details/gwfiqbszx.sHtML

[T44] Perl：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvveagspb.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbddqnvfq.sHtML

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gwucsamwf.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgexmbdr.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjiauadts.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxgtgzru.sHtML

[T47] Perl：正则捕获
来源：http://baike.fanxiaobao.xyz/Article/details/gkmttkmbh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/goyvfoopd.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpldtfwo.sHtML

$s =~ s/old/new/g;
来源：http://blog.fanxiaobao.xyz/Article/details/ghmyitiwu.sHtML

[T49] Perl：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpkfsrwc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmptlzboc.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijgudyqr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fanxiaobao.xyz/Article/details/gebxsmqtp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/giquemmsl.sHtML

[T51] Scala：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gwkdshnmb.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswucwvfn.sHtML

[T52] Scala：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gogxusivh.sHtML

val a = 1;  var b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/ggtpstdyi.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gukucfilw.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gyumqxyep.sHtML

[T54] Scala：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmqbrmtn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/ghecnmcfu.sHtML

[T55] Scala：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gciqbucoa.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkwsynhs.sHtML

[T56] Scala：样例类
来源：http://baike.fanxiaobao.xyz/Article/details/gjfkkhuva.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/geztzwmnu.sHtML

[T57] Scala：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gyveliqdl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fanxiaobao.xyz/Article/details/grnfdxbwe.sHtML

[T58] Scala：函数定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjrzavvm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/gxizwbxok.sHtML

[T59] Scala：循环
来源：http://baike.fanxiaobao.xyz/Article/details/glzpkhtij.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/grjqhedfy.sHtML

[T60] Scala：折叠
来源：http://read.share.fanxiaobao.xyz/Article/details/gmncxzxdq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fanxiaobao.xyz/Article/details/guchpdbny.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gecvebbig.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblokwcvv.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkebhabx.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fanxiaobao.xyz/Article/details/gsgsnmrmw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fanxiaobao.xyz/Article/details/gqjnkmnan.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fanxiaobao.xyz/Article/details/gslyxgdxe.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gsanugjaj.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fanxiaobao.xyz/Article/details/ghognpqew.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fanxiaobao.xyz/Article/details/gvqycabls.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpxppnxr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fanxiaobao.xyz/Article/details/gfettavvg.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvullvql.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrtmgsvw.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvfphsxc.sHtML

{**a, **b}
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcgpfmyn.sHtML


<!-- 参考信息 -->