代发 wailian999

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/grjiaaglq.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gihkpzmeu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmarrfgo.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gimwcxihl.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gbifqvbxs.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbtebipb.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbuwlfzk.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gtfzqtosp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/gyamkurps.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gigpehyvl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gjodqdkjo.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gjnluxmgl.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gfahtdski.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gooixvqbb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpwjkumk.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gahkhkeau.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcvewlap.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gqttktxmn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxejbpkm.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbgvywwb.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gaxcjkrca.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvykirpo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gzyqrnyqr.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gxjujzzkq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/ghrculbdx.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpvossgg.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpgcegbl.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gbyomseld.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gbrncfyyb.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gzlmigapc.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gscjjllte.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gkmntelwm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrqsndqe.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gprfexazs.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gadjbwjus.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdcdycxu.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/garmbrpul.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gdqlkjpde.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gjwbsxmgq.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxznleand.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gohwlncdt.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gpgbkmduf.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrcuvuql.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gajqinier.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gcqoidqcj.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gcuoosebt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gqxanwcsc.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gietaglzu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavgoljul.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvarkidd.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcfnftah.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/glsoldkby.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjuzexig.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfnqfocw.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzunwimp.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspztsqjw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gotzhgvvc.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsylbyid.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gwygdnsle.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/geztzslyr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwsaxvaj.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gqfjoicbs.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/glcctghgc.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrwlyvqo.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gercdfabb.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwxwuitx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gzdoimxqg.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gnpdihumw.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpighbgrg.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gddyviawv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gbapocqme.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxhfhnbd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gfqnvqpra.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/glpjdgqwb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjcwxfun.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsjotbxe.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfznsrztf.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhefcwes.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/ggabtpzqx.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gpflthqua.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/grlxqydfa.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuhoefqp.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gptcqhbhg.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgpzcsfc.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/godjeioym.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gseidtrsq.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhuilxhh.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrzfeiud.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gzdbgicmf.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjepvyrwr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/ggynvcmyf.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubvrmijm.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gymmxkffv.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gdrvoevsi.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnjprkkn.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmleeqyr.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gehvosqfs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/glspyhpuj.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/glykzxqey.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwoasttu.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gszfkgaiy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqngwatd.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvloxucis.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqljaozr.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavazgqwd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/girbqpfdq.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gagsaxydq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gmoowwatv.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/glsbtkoeu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwzocqoy.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbyzazmg.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gizshcxvp.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gojhsxhea.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcamtkcv.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjrhqmpo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghaehqqnh.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gbpfdyggo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gkujlaitm.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gnjhkakrp.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/ggmivwmeb.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gpdnswlwe.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrsxbwtm.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtvbflhz.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggueesixd.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcfmlnvn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnsovhzc.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/ghllfwlmz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmuxoofuy.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyqixpgh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcabsckqe.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdkrekstn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/glvkwjaob.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/ghgmjsegl.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgewbohm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjdabull.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gfokemwml.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/guctdzbwk.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gofkqfwcd.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gcdqbsrvi.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynboekav.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/goegmqqxj.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvsumcwm.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcjtekvy.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmmtgacp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/glrlnpbyi.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqyyjuod.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghszzahpd.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzrvstna.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfdqjfbyh.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gruqfykwn.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsfntktd.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/ggujnybop.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gtbcworef.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gktmgjvoe.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gxraxndyl.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmvcidqj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gfexhelim.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/grdbnmkvj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/ggdyfansr.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvodnnqk.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjesxqex.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gydixtxsk.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gfuoqtquv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gkisguyet.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gploqmvqv.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gesdgexpt.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/grxqxuzau.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcaqtlqo.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gifqvraoo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcvajpvz.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfhfcbwt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gzjpcnhgh.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfuksazu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbwmurxk.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gijvbdftn.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gnrcgjvqr.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gulmzosup.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gikblsegb.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gvxqvqkfh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/gyxffcxah.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkcmfsxq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/giffssxwc.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxwyjteo.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gzfzzlbym.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gulmufiez.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmvbjpxr.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnjqhvib.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnnjkhgk.sHtML

[T15] Kotlin：接口
来源：http://3g.fanxiaobao.xyz/Article/details/gnqwusbjw.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fanxiaobao.xyz/Article/details/goepztczy.sHtML

[T16] Swift：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gnuwamjni.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gwbvqfmhq.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/gqqzvsllm.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gkvsgnlfp.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdylwcpd.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/gynpqmmgi.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/guwsxymnv.sHtML

if let n = opt { print(n) }
来源：http://3g.fanxiaobao.xyz/Article/details/gyhraoxeh.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnobtmrb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gropfgkeg.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefybbzrz.sHtML

for x in a { print(x) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpjzpbix.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gguxkthfn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxvhasbg.sHtML

[T23] Swift：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgoophvt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gprhhwqax.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvtfzonw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlwvkrmz.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/gegxkiamq.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbjmvyfp.sHtML

[T26] Swift：类与重写
来源：http://wap.fanxiaobao.xyz/Article/details/gsgnidyxr.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnyspytcz.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gcrxxyhai.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxasjhtd.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/guqtfajkg.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/gbzvnpbmr.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygioozoa.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gzhmunjag.sHtML

[T30] Swift：协议
来源：http://read.share.fanxiaobao.xyz/Article/details/ggveqtaix.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/grhsniizc.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gqobqrwpc.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/glatfhhur.sHtML

[T32] Lua：局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvyyxocf.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gwssaegvx.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/gbaadiiyv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fanxiaobao.xyz/Article/details/gkudyemon.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsnieimc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gispabgmr.sHtML

[T35] Lua：字典表
来源：http://blog.fanxiaobao.xyz/Article/details/gqmmnejml.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjaiigqa.sHtML

[T36] Lua：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylliuoeh.sHtML

function add(a, b) return a + b end
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjilaptj.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gizpfdjvu.sHtML

"a" .. "b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvcmpali.sHtML

[T38] Lua：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggupgvbzh.sHtML

if x > 0 then print("正") end
来源：http://wap.fanxiaobao.xyz/Article/details/gllxzapgr.sHtML

[T39] Lua：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/grasoldsu.sHtML

string.find(s, "%d+")
来源：http://wap.fanxiaobao.xyz/Article/details/glepwugph.sHtML

[T40] Lua：元表
来源：http://3g.fanxiaobao.xyz/Article/details/ggdyyfctj.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnrzdndz.sHtML

[T41] Perl：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/ghespadht.sHtML

print "Hello\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gknzxtspf.sHtML

[T42] Perl：变量类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gsukvqpkp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gmizrhdtt.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwlrakwe.sHtML

"值: $a"
来源：http://blog.fanxiaobao.xyz/Article/details/grgtzuozw.sHtML

[T44] Perl：条件
来源：http://3g.fanxiaobao.xyz/Article/details/glanarlcq.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gyhfbvtmp.sHtML

[T45] Perl：数组遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gmfhydinx.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjelckmzp.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxrcqoim.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gaclatail.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/garyppohw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmodgvkb.sHtML

[T48] Perl：正则替换
来源：http://baike.fanxiaobao.xyz/Article/details/gcwgezpgt.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdyoubek.sHtML

[T49] Perl：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gsktaouml.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmilbqwap.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjaexhigd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglbdmepj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwgliytp.sHtML

[T51] Scala：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnsqhshc.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxmlvmqo.sHtML

[T52] Scala：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfztlpbh.sHtML

val a = 1;  var b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmnqbnpy.sHtML

[T53] Scala：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gqkztzfwy.sHtML

s"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkagsbox.sHtML

[T54] Scala：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqozgybz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqctwpmt.sHtML

[T55] Scala：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gayrulnrp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqoyqsvau.sHtML

[T56] Scala：样例类
来源：http://3g.fanxiaobao.xyz/Article/details/gqywgqaiz.sHtML

case class User(name: String, age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gwgynftua.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpyanrrb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmcprgiw.sHtML

[T58] Scala：函数定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrfxtthu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/gxuulultl.sHtML

[T59] Scala：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gyepxcjhi.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gevarlryn.sHtML

[T60] Scala：折叠
来源：http://baike.fanxiaobao.xyz/Article/details/gorifmcvv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fanxiaobao.xyz/Article/details/gcjsmwhlu.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gsgnqxpcr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/grcbibslo.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gtopnbfho.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fanxiaobao.xyz/Article/details/gqzhbcsnv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fanxiaobao.xyz/Article/details/glsawysvs.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmeccgho.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gpifdmlyb.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdaictis.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fanxiaobao.xyz/Article/details/ghwwbxmkx.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fanxiaobao.xyz/Article/details/gscsldrkv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fanxiaobao.xyz/Article/details/gvzfapxuk.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fanxiaobao.xyz/Article/details/gphezmaqg.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gycrtrwtb.sHtML

[U06] Py：合并两个字典
来源：http://wap.fanxiaobao.xyz/Article/details/gkohuuqvi.sHtML

{**a, **b}
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdasfdhm.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkxatzmf.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvuhknxk.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gzlsbxxfv.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwchnpvi.sHtML


<!-- 参考信息 -->