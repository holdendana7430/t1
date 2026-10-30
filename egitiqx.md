代发 wailian999

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/grkngkjbu.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gfliwqllh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gwcplviqx.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gbalmfxnc.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gaozmabjy.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gjszmnbet.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnwmypte.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/grkaskbfz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/glbzfplkj.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gerbzeppy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gvysvnwjt.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gffanbaac.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzbvlkxk.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgenayzn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gxwuojarm.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/giubeyqwk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gtitfxzam.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/grjvmggvj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gszgbonpm.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/grusjfrji.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlpdgxay.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gffsnpokw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/ggxpathef.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gegfsdrae.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ghijoysvz.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjjolnae.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gauyqjgbo.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/goajovafc.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsvfuzjz.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gecpwlupl.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/ggbpsmeqn.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwflzzej.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxqvibay.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gorncgbiz.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccimloyt.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/ghipmperq.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/giexxukmd.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gkciacpqy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyintblif.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvdnavwo.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gwmbuoidy.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyijnthb.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/geiqlwffs.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/giahtzyek.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcdooxwu.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gqsurlypd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gloasupke.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/graznrqum.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgnoyoqv.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gjarqvoef.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfuhzbcw.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgdezkgz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gskhmmezu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gcvorrowk.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvogevjei.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkitiwasn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gfwpwwjmt.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/glymhyexp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxuqvgpd.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/glgigpagb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gewfcajwl.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gdfdokcxc.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybbarxok.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmjeglbe.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/guveecibe.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkftyibf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gcrkjjsdm.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gqqvelbal.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsrfhfmm.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/guacwdmnf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gpukvnhqn.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gqqvubvza.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gixrkgnlk.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gprjvlxee.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhzgwslu.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gyoxkvqyo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqrsxyyr.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/glreepbdw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcooslyvk.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjqlugpe.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzthqvgtf.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/grinklnet.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqmhfdjx.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchjuuuti.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/glqwdmssk.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gqdshvesx.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghopptgty.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpnpdcdm.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gikonlpti.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gqetioiur.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggllmsiql.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwcrpttj.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlwgpvjf.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlumgdtb.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gjmemivlp.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gwfcbeinh.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gaktymzjh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtbwfqbx.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gvskdbrkx.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gaqyhcqel.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/ggmivdfor.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpusnvfui.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gxepwjltx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuzjzxub.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbawxesu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzyxtzxn.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/grojloywx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/ggdujvkzm.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gkybybayf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulvnkuih.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gnidtaoil.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gqygmnpbq.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gwxihhavk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdodduqcb.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/glnglrbxr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjdexjwn.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdvjjmzq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gaagtpkfo.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtemrphhk.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrrhmvgg.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpjwhuvc.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxczzjubu.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gkqonaezg.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/grphgotjd.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gboyctbmi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/gsvlmevfr.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslngvywf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmqzgrld.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyugbozpm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjnfusuf.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxmxutxvd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gczkmwfmm.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gciqhiqvj.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkczoezvt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gqzomzntl.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/goevlsksy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gourqvbhe.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklrwbnqd.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjkbulay.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbyfmcsf.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwfdehjp.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsojqfzhv.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gzifgepwr.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyslpjxuc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/grztldtat.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gxmocyhld.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/glwmsplwq.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/gucjihhvy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gysvxgdbh.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslmhaobp.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmrmsgzc.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtyasomk.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gudxnpgda.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gyryjuuyk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gjilivskq.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gooomhwdb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gooyirlkb.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/glrcqckks.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlxylgxz.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshkouknk.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdvbwemm.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gbrcclnap.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gifqsvtfi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gquljrcap.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/gobsnvsap.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/guxyokjnu.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/gbnvagatn.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gihutvfxc.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/giqvbsuop.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmzicfbr.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxhhnmgm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/ghovdrfas.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxckrixa.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/gbwocvalx.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gppqsvhko.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqoabfrh.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glriewrtb.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/grdpdlpna.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkxhczqf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/gxtuitzip.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxluyseh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/gsmqkfpjx.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtyabmeg.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/govudhrhm.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gzhwpenyb.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmyspjdr.sHtML

[T14] Kotlin：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gwowsgcxk.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxokitsuf.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/gnbmmbnmd.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gylobttfz.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/guxvjxmlx.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbadudqn.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllwpyzjd.sHtML

var a = 1;  let b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gtanbxkoz.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/ggmczibak.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfrgnrvh.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpxsjruk.sHtML

if let n = opt { print(n) }
来源：http://3g.fanxiaobao.xyz/Article/details/gqlujapqu.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gzqqaumll.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgeshygh.sHtML

[T21] Swift：遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gmstnxzeu.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/gspnfjxik.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnapsart.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gpzperqke.sHtML

[T23] Swift：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjyrdpzn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gltelhscm.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdqtadpn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/grvjbviay.sHtML

[T25] Swift：结构体
来源：http://baike.fanxiaobao.xyz/Article/details/gsteakpqd.sHtML

struct P { var x: Int }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcllkdfj.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/gbjoqpykx.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/gebeweowh.sHtML

[T27] Swift：错误处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwviizje.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczzwwwhd.sHtML

[T28] Swift：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbqgaczc.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/gzqtsxthv.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/gvpfrrcjs.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjwiwkss.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/gptohqrwt.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gvpicwqul.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gvwhjjwnn.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gzqutjvau.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicwkfsvq.sHtML

local a = 1
来源：http://baike.fanxiaobao.xyz/Article/details/glggpoxnx.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdudrpgr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fanxiaobao.xyz/Article/details/gogkdsdbe.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzoqhsnjt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fanxiaobao.xyz/Article/details/gtfijimqw.sHtML

[T35] Lua：字典表
来源：http://read.share.fanxiaobao.xyz/Article/details/gyidscwsu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbfvksxs.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzkrbjnm.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnvzvfwa.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gsmcpzstc.sHtML

"a" .. "b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gobsiteot.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gprdojizl.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/gbuqchzry.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlthgtel.sHtML

string.find(s, "%d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/giaqxzcin.sHtML

[T40] Lua：元表
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdnhabku.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbukittp.sHtML

[T41] Perl：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/ggwpihahm.sHtML

print "Hello\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gzpmrurem.sHtML

[T42] Perl：变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/glqhmmoyz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fanxiaobao.xyz/Article/details/gjhmtbkiy.sHtML

[T43] Perl：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gduivffui.sHtML

"值: $a"
来源：http://blog.fanxiaobao.xyz/Article/details/gpkrchkam.sHtML

[T44] Perl：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnacxhmnn.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grvwhiwue.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gvofwnfjk.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwnmaybi.sHtML

[T46] Perl：哈希操作
来源：http://baike.fanxiaobao.xyz/Article/details/gjejgngam.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmzphlltj.sHtML

[T47] Perl：正则捕获
来源：http://wap.fanxiaobao.xyz/Article/details/gvizkxvrx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxfsuiol.sHtML

[T48] Perl：正则替换
来源：http://baike.fanxiaobao.xyz/Article/details/gdtiutasg.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guasxjmxl.sHtML

[T49] Perl：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcwouaoh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvkvvbbsv.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkoziwjm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fanxiaobao.xyz/Article/details/grshuhgim.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvnywkpp.sHtML

[T51] Scala：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/guchgbyjk.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmajwnmbq.sHtML

[T52] Scala：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gbeiiiier.sHtML

val a = 1;  var b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gxxxlvlmx.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhutsehm.sHtML

s"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gtqivdwjr.sHtML

[T54] Scala：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/guearcvje.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/glxhcqqro.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gscadwpqc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gcxeixyny.sHtML

[T56] Scala：样例类
来源：http://wap.fanxiaobao.xyz/Article/details/gtrmivmjg.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gktuokiyr.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glogecikv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxmzimfn.sHtML

[T58] Scala：函数定义
来源：http://baike.fanxiaobao.xyz/Article/details/gguuathaa.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/gddnthglp.sHtML

[T59] Scala：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedftiybk.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzinwpad.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrmgtgem.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkconnhi.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gpcqocgis.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/glzdtjhqm.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gbdkamvqg.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fanxiaobao.xyz/Article/details/gpjucnyov.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fanxiaobao.xyz/Article/details/gsoaxlghm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fanxiaobao.xyz/Article/details/gksyuswzq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gfocdknth.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gycfbasmz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fanxiaobao.xyz/Article/details/gjoeifnkq.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqqsiyir.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfkameuq.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvfumtos.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhqnylnd.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmbpzery.sHtML

{**a, **b}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyphcwqw.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fanxiaobao.xyz/Article/details/gelcgealp.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fanxiaobao.xyz/Article/details/gonzmsbok.sHtML

[U08] Py：展平二维列表
来源：http://3g.fanxiaobao.xyz/Article/details/gyolxdnbl.sHtML

[y for x in nested for y in x]
来源：http://baike.fanxiaobao.xyz/Article/details/gwewakxxb.sHtML


<!-- 参考信息 -->