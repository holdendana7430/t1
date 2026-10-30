代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/glbnsxehx.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gctczavid.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnurhzews.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gexgctale.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/glguiybfx.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gntkdxynr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gontxbhyl.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxaqwwqwu.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjwirzjh.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gimrgaxik.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghunortin.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjcaucgg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlbjijcp.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxpwtlji.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gqfzyntpj.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjowaghvt.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gxiawpekf.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gilpqfype.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glagftmfj.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gethsnzot.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzopsdds.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypvnryys.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyjpypzd.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gagxsqazp.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfvqsexe.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrougzbx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbglzbzu.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gjadvoqdk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geenpoprv.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/ggiwlmbel.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/grtleojdt.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllwthpyq.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxmahvhv.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gscwlhuqi.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyiihddod.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gokykjhka.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gruiximsi.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezizzvri.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbapvxwr.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gucrvoktn.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdocuoth.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqdhtswg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsuserzs.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gavezusbs.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gpifdmona.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/ghehmmdlw.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gujplaznl.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/ghiwtwzfq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gakqvroaj.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gylhvxtop.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gyyyfiwgf.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gtiwbwvod.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyhsijhg.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gdtrhtnbj.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gyjulkufn.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guryaikcp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gsghliwee.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gulqaocwq.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gcquhnvap.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywkcykpp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gzcfxaysr.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gjneddyvg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/ggsyvpvtf.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/grbrberbb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gydnjrmjs.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxvsbqwn.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/grlkkivur.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gtomaqcxw.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhlvsfis.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxdbwhet.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebqkeyai.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftngqtvx.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvhiazxo.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjaavodw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjswjhnd.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gcfgarial.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/giwknzskv.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpzekeql.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbotaaqaa.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgdlmsvq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/ggtclrnuf.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqxiuvgz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdcsdgfm.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/guxjjykbr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gikazdxou.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvlwlnwv.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/givpylnur.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwjqpufg.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbuptscd.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/groaxidoj.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/ghernbxas.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnfcwrzd.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gaobfdwas.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdgwlhgh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcccwukmy.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/ggvnpmzyn.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gyvgkuqjf.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmegqttd.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwxoednl.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/ggzctpvfm.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapuaifcq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmfqfkow.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gkkimvedq.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gvizrfjap.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmjuaxbn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gqibzjymq.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtuzlmmw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqypecqfo.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtezofqk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/grkbjhhhx.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gzgqequke.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpadqjzv.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gwzujrdkb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgyznluv.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gbwodkmql.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gymyesefu.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gfgduvnwa.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gjamcpkbk.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gynxzumou.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/ggoeoprzt.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gukkkfnfu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzhsiuwu.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gbnvzhwae.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyvbmlbr.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gpnzcypcr.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgymfuhf.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/goiwcqcff.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gakwrlzyb.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfftvacp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gytefkllo.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gixjnklcf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvvpdprrh.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbittmtu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhpqtpll.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/grfzmpgrl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwxfzndg.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtbjfyvd.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxdmzpnc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gbaqfpynq.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/geghlqgnj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxgbuqwt.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsdodlnu.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gvdkwgyuw.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkzhrzgw.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbdkuabyw.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkaoztddb.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/grhqwhpfi.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gnexrfdrb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfponzbbw.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnaoomdi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqtpobdb.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gpgmxmhfl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gquqchbpu.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gvsbthtmc.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhgnqkey.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/ggirjjnyv.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gmhflpaag.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljifejto.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutspskbo.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhhnhxcp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gjbrzwtuw.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gohrzurqe.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gomendrwi.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gpvkoggku.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvaauvex.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gcvjimobo.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqsdauif.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gpqretahx.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpoemzne.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gbpmgffba.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsfclvsw.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/gcafuzlen.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gdritlkns.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gpiweuhoa.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gpgagfrbc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gytedruqo.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/geoucvkfk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gpqwtbzui.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/govdhinwo.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpgczmwz.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gskiamcsv.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpewhisv.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/glegjztzd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gryiuozli.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/gsalywhkw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/gysqvueut.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbbvbvpc.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxfmqehg.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gudsglnzi.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpigiqaj.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gkprwahge.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgndxddb.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpltxsht.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdiuonxjl.sHtML

[T16] Swift：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gailgjwsz.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gahloomhp.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gltdrmrlt.sHtML

var a = 1;  let b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsmyozkb.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabiqrjby.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/gusckfgph.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/glljokyml.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/gycqzkqyl.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcfriqqx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gaagxrjue.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/guxsdjlda.sHtML

for x in a { print(x) }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyxvweyo.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/grsfmwtty.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnobboxu.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gsuhiajvd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gygetxgce.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobydisnl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gvyibfkvw.sHtML

[T25] Swift：结构体
来源：http://mobile.fanxiaobao.xyz/Article/details/gslgsxvfh.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/grefqxgjm.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/gslfpagsb.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhcfimub.sHtML

[T27] Swift：错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/grjewsuyk.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fanxiaobao.xyz/Article/details/grxnaxwha.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gveziuojy.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/gwflzxmjn.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gotftbncz.sHtML

guard let x = opt else { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gyrzskjqd.sHtML

[T30] Swift：协议
来源：http://wap.fanxiaobao.xyz/Article/details/gnhdugojm.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmwjvkbh.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/geokpiogc.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gguzuaxfi.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gulopbvxx.sHtML

local a = 1
来源：http://baike.fanxiaobao.xyz/Article/details/gcfgguedb.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzafpeqx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fanxiaobao.xyz/Article/details/gciphqyhx.sHtML

[T34] Lua：遍历表
来源：http://blog.fanxiaobao.xyz/Article/details/gkialykoi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fanxiaobao.xyz/Article/details/gkacosbrp.sHtML

[T35] Lua：字典表
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjursdeg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gmmasxoaj.sHtML

[T36] Lua：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxhbbykf.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmurinsep.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gfvuywoiz.sHtML

"a" .. "b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdhvrpux.sHtML

[T38] Lua：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkzedpgz.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/gftikpmcb.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwhcgyyb.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gxqspjszz.sHtML

[T40] Lua：元表
来源：http://blog.fanxiaobao.xyz/Article/details/glhwzsjab.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fanxiaobao.xyz/Article/details/gufccnxgf.sHtML

[T41] Perl：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdfzawrx.sHtML

print "Hello\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsiveuvyi.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gazabvlkj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gsdzabsat.sHtML

[T43] Perl：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gznnqhcja.sHtML

"值: $a"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbgfofwo.sHtML

[T44] Perl：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gueojvznp.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqedduljm.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/ghiutxxub.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrseqoby.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gajakzylb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpyoxuis.sHtML

[T47] Perl：正则捕获
来源：http://blog.fanxiaobao.xyz/Article/details/glsiqsrng.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxogninp.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/gzpvjkesy.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbmfjzak.sHtML

[T49] Perl：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/guquvmwfg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gibmdwkcm.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gvydsjktc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fanxiaobao.xyz/Article/details/gfgtmbhyi.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdnobstj.sHtML

[T51] Scala：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gjctroujr.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/glouaexjo.sHtML

[T52] Scala：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvwvikaj.sHtML

val a = 1;  var b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzinuszc.sHtML

[T53] Scala：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gdezeugwu.sHtML

s"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gwtzszqjf.sHtML

[T54] Scala：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyupbwsg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gycfylpfx.sHtML

[T55] Scala：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gjzcqpnla.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqoqwvxis.sHtML

[T56] Scala：样例类
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnnuxuqc.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqopcurgt.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/grgthnjdc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfoheemg.sHtML

[T58] Scala：函数定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyfrdywg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxyltkuy.sHtML

[T59] Scala：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyejqshg.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/guwkgxxgy.sHtML

[T60] Scala：折叠
来源：http://baike.fanxiaobao.xyz/Article/details/gcnzqlxwq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqukgfzm.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmxzyhtq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyxzawqb.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gwedkcagt.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fanxiaobao.xyz/Article/details/gwghhvvuf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fanxiaobao.xyz/Article/details/gjogaviuq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzdrfdpz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjhnnjhv.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gniqmkxto.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fanxiaobao.xyz/Article/details/grnyuqemd.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fanxiaobao.xyz/Article/details/gttcrstsw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmcvyagc.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fanxiaobao.xyz/Article/details/gojhqvgop.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gzharssgd.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwigbhqkf.sHtML

{**a, **b}
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzfeerfw.sHtML


<!-- 参考信息 -->