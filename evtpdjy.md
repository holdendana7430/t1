代发 wailian999

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/gjspiuzas.sHtML

[R68] 计算文件校验值
来源：http://3g.zdbjq.cn/Article/details/geacxhjcp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gpvqctewk.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/gdiiqsxdf.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.zdbjq.cn/Article/details/gjzmzpzly.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/gkfalbcxl.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/gegdfhlaf.sHtML

[R71] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gfjuyuebw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gsaawsrrp.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/gganevahi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gjzoieupk.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/guvqxzzwz.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gkwuumxhg.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/gxqpbvtjj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/ggpglcabj.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/gyvkogrtp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/gaaxavvcz.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/gljfdttsa.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/guwtnfjqq.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gsxkbfkfs.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/giqjkvvyn.sHtML

[R78] 交互式菜单
来源：http://blog.fehbvm.com/Article/details/gtubeqgwu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gtmoacyhe.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/gztpwwccf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/gkovjcagm.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/gxfbubdym.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/ghdirxmke.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbpuqckvw.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gcyvgrslj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtvlnnfbd.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gqknaxvyd.sHtML

#include <stdio.h>
来源：http://www.share.fehbvm.com/Article/details/giozpffax.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/gnuuxtldg.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/gtcqzqcgn.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gyjehhqaz.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/gsepjogir.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gsgbcsevp.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/gjecixqso.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/gvichfyed.sHtML

[S05] C：字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gqnrydtan.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/gcdqgqaue.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/geqlfjxso.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/godvaynoe.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fehbvm.com/Article/details/gxxuospbu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/givbuyxpj.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/gevawywmj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gieotaroc.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/gfszdjvfc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/grjanquut.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gvdobspzc.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/gswjxydnj.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gelznuqgf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/gwswggywv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/gdjjaelje.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/guhljqoeb.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gbachvmgf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fehbvm.com/Article/details/gqxrusdkz.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/glarjvtur.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gtnwglndc.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/gnaawuoed.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fehbvm.com/Article/details/gliihrwkt.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/gpbnfaryb.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/griccpnxa.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/gnpilzhvb.sHtML

x |= (1 << 3);
来源：http://blog.fehbvm.com/Article/details/glyybbgtg.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/ghkxojisf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/glrjgcrge.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gmdpqvpoi.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/gbyuaknud.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/gvptlrict.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gttlqhwlf.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gswvufmop.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/grthycqso.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/gnftsuyky.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/giywldsyu.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gkfxtsumo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gkieswyrq.sHtML

[S23] C：随机数
来源：http://www.blog.zdbjq.cn/Article/details/geaqnrcfz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fehbvm.com/Article/details/grygapppt.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/gjolzgyfo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/gyelokkfy.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/gbvcqewbt.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/gihtzdcmx.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gfzbthedl.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/gacrvitas.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/grvhnotfd.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/govbartad.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/gzpproboq.sHtML

static int counter = 0;
来源：http://m.share.fehbvm.com/Article/details/gycneypgc.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/gzxblbbxj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/gdwlqgjrh.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/ghbahqqzs.sHtML

#ifndef X_H
来源：http://www.share.fehbvm.com/Article/details/gxahpxhpy.sHtML

#define X_H
来源：http://baike.hesvh.cn/Article/details/gtbnnghpx.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gfcuflahh.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/goorxupkx.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/gcthhgmkf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxaqegmif.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/gdsuvlxft.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.zdbjq.cn/Article/details/ggltabnsm.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/gqgbizrwx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/gvhgnjclh.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/gnicgpdyc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gpxmjctfc.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/gzdcveiic.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gfiyurjfa.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/ghpsfqbxo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gtwsjfccj.sHtML

[S37] C++：set
来源：http://blog.hesvh.cn/Article/details/gwhqpvmwe.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fehbvm.com/Article/details/gmnlgxkxu.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/ghzgsugvd.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/gggqviyxb.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/gacydhdig.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/gvplranem.sHtML

[S40] C++：查找元素
来源：http://www.m.share.zdbjq.cn/Article/details/gsfngacbr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/gqflzhndh.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/goweeixqu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/gvzkpwpng.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/gcpilvcyl.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/glaqjmsxx.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/grnfpddmb.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/gkfhpmflg.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/guvdtvhuc.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/ggfvlwlso.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/gbxuhmwop.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gcrafuvwo.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/givbjqynf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gyildcxis.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/gdnjjprkv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/ghbfilknu.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gqmygvhfv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gxbopdhuh.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/gybzkwrzp.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/gowisznyf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.hesvh.cn/Article/details/gyddglbxv.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/gpqbcxqiq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/giqwmsibo.sHtML

[S51] C++：显式类型转换
来源：http://mobile.hesvh.cn/Article/details/ghnbitmnf.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gojhadpjd.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/gomeykrqm.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/gkacpwaef.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/gmypunmsx.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gxbnzetxm.sHtML

[S54] C++：异常处理
来源：http://read.share.fehbvm.com/Article/details/gfnjililp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gddxaavgq.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/gfoepdjag.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/gszhqatpz.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gbplfxxdp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/glkvwfdkn.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/ggrctgxdz.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/ggzyaijzj.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/gxuharjmq.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/gmptylfkq.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/gvjmovqsb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/ghdaxlbgk.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/gvwnuuxkw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gpthqlglk.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxqdevtph.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/ghdhytvgd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnwodbdbd.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/gmdqteehs.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gofnqxwec.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/gpfgefthg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/gdjnhfjxu.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gqujyhyrh.sHtML

"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gscsjepsz.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gwocnvxux.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/gaaeclyjo.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gmjrfrqgh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/gtwiwrypw.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/guqnutsfw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/gwpgyfiqb.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gzsuhdjkh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.zdbjq.cn/Article/details/gsotaadxa.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gqcsucgbl.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/gjtehaaqi.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/gsmbgibqx.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fehbvm.com/Article/details/gmdoqnckc.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/gbaornwyo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/gwkaslmbj.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gbtlxpkln.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/gsbmodsuv.sHtML

[T12] Kotlin：解构声明
来源：http://3g.zdbjq.cn/Article/details/gkeaknteg.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gbxezkryo.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/geauphezk.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/gxjupmyhr.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/gaxqppknx.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gkwladlfu.sHtML

[T15] Kotlin：接口
来源：http://read.share.fehbvm.com/Article/details/gzyitbhvc.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/gtxvfqryq.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gqhlsgukc.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gfhevirsg.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.zdbjq.cn/Article/details/groyuenzq.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/goncwekdz.sHtML

[T18] Swift：字符串插值
来源：http://read.share.hesvh.cn/Article/details/ggistyfxa.sHtML

"值: \(b)"
来源：http://www.blog.hesvh.cn/Article/details/gnakhchwx.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/ghdxriuzs.sHtML

if let n = opt { print(n) }
来源：http://baike.zdbjq.cn/Article/details/gfrrjwkyq.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/gkkzmegln.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/ghjxbnego.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/godjniwgh.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/gxzcdvfod.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/gxmoovlid.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gmqszrtgk.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/gsjhixjrp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gesdqagsw.sHtML

[T24] Swift：闭包
来源：http://wap.hesvh.cn/Article/details/gvozxhbva.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/glsylkyll.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/gpfqyacul.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/geipxqkod.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.zdbjq.cn/Article/details/gkdovbevt.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.hesvh.cn/Article/details/gplklpqel.sHtML

[T27] Swift：错误处理
来源：http://baike.zdbjq.cn/Article/details/gohuykbkb.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fehbvm.com/Article/details/gaibjhchk.sHtML

[T28] Swift：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gvuzyasmw.sHtML

enum Color { case red, green }
来源：http://wap.hesvh.cn/Article/details/gioiznlcd.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.hesvh.cn/Article/details/gbdwqilof.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/ggvypeikf.sHtML

[T30] Swift：协议
来源：http://baike.hesvh.cn/Article/details/gjhbchdbl.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.zdbjq.cn/Article/details/ghfzyfnrn.sHtML

[T31] Lua：Hello World
来源：http://3g.fehbvm.com/Article/details/gpgjrwikv.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gebvjcsco.sHtML

[T32] Lua：局部变量
来源：http://wap.zdbjq.cn/Article/details/goozkyjft.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/gyugtceik.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gukajlkqf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/gbtnmsovs.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/gpwcyvaoc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.hesvh.cn/Article/details/ginwljnjv.sHtML

[T35] Lua：字典表
来源：http://www.blog.hesvh.cn/Article/details/ghrportju.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.zdbjq.cn/Article/details/giyrlfogs.sHtML

[T36] Lua：函数
来源：http://wap.fehbvm.com/Article/details/gczkhbcmj.sHtML

function add(a, b) return a + b end
来源：http://baike.zdbjq.cn/Article/details/giahgdhmu.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.hesvh.cn/Article/details/guqhcqilc.sHtML

"a" .. "b"
来源：http://mobile.hesvh.cn/Article/details/gxeinmpvq.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/gutlzzzvo.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/gggzcimqi.sHtML

[T39] Lua：模式匹配
来源：http://baike.fehbvm.com/Article/details/gptlgyuos.sHtML

string.find(s, "%d+")
来源：http://baike.fehbvm.com/Article/details/gkuikbceo.sHtML

[T40] Lua：元表
来源：http://www.share.zdbjq.cn/Article/details/ggxxgzrfx.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.hesvh.cn/Article/details/gvvxcybpf.sHtML

[T41] Perl：Hello World
来源：http://wap.hesvh.cn/Article/details/gjaqsxjbj.sHtML

print "Hello\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gzzbenajl.sHtML

[T42] Perl：变量类型
来源：http://www.share.zdbjq.cn/Article/details/ggcmtzwnd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fehbvm.com/Article/details/gododnqbp.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gmhhzljjy.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/gwvfgoywp.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/ggswonuuq.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fehbvm.com/Article/details/gdqcskutd.sHtML

[T45] Perl：数组遍历
来源：http://read.share.hesvh.cn/Article/details/gggmduamh.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/gksurulxl.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fehbvm.com/Article/details/gfstkmjac.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.zdbjq.cn/Article/details/gcolufmul.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/ghoampilw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.zdbjq.cn/Article/details/genpwgjnz.sHtML

[T48] Perl：正则替换
来源：http://read.share.fehbvm.com/Article/details/gcvocrylv.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.zdbjq.cn/Article/details/gvtrsgdzz.sHtML

[T49] Perl：函数
来源：http://3g.hesvh.cn/Article/details/gwmirozzt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/godvpenxm.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gklyenxwb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fehbvm.com/Article/details/gndimhvkw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/giiwnjuwq.sHtML

[T51] Scala：Hello World
来源：http://3g.hesvh.cn/Article/details/gefiixxjk.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/guguipshn.sHtML

[T52] Scala：变量
来源：http://read.share.zdbjq.cn/Article/details/ggelbwail.sHtML

val a = 1;  var b = 2
来源：http://wap.zdbjq.cn/Article/details/gkexvljur.sHtML

[T53] Scala：字符串插值
来源：http://m.share.hesvh.cn/Article/details/ghhobxnkf.sHtML

s"值: $b"
来源：http://3g.hesvh.cn/Article/details/ghgmxgyay.sHtML

[T54] Scala：集合映射
来源：http://read.share.hesvh.cn/Article/details/ggastibaw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.zdbjq.cn/Article/details/gchpflkrh.sHtML

[T55] Scala：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gfgfqezue.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.hesvh.cn/Article/details/gnlpfdhgs.sHtML

[T56] Scala：样例类
来源：http://3g.zdbjq.cn/Article/details/gfljjifdm.sHtML

case class User(name: String, age: Int)
来源：http://mobile.hesvh.cn/Article/details/giktoqbbu.sHtML

[T57] Scala：模式匹配
来源：http://baike.hesvh.cn/Article/details/gfwmxqojv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.hesvh.cn/Article/details/glebqoeay.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/glqonvans.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.hesvh.cn/Article/details/guuqfhkwm.sHtML

[T59] Scala：循环
来源：http://blog.zdbjq.cn/Article/details/gttfvmcxu.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fehbvm.com/Article/details/gvlqhwzbu.sHtML

[T60] Scala：折叠
来源：http://read.share.hesvh.cn/Article/details/gmmznzfhp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/ghlcmiuyv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpbgrcceb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/gepnajunj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghiftehig.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fehbvm.com/Article/details/gltylivrd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.zdbjq.cn/Article/details/gfochbpyo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.zdbjq.cn/Article/details/gvsofxqel.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.zdbjq.cn/Article/details/govsisgif.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/gcegasjpa.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fehbvm.com/Article/details/gtbjjnmbw.sHtML

[U04] Py：变量调试打印
来源：http://mobile.hesvh.cn/Article/details/ghutlwryl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.hesvh.cn/Article/details/guhgzztgp.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/gmttkwtio.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gmljgxtmi.sHtML

[U06] Py：合并两个字典
来源：http://www.share.zdbjq.cn/Article/details/garahqrjt.sHtML

{**a, **b}
来源：http://m.share.hesvh.cn/Article/details/gcrtrxjbg.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/gvglrahro.sHtML

{v: k for k, v in d.items()}
来源：http://3g.hesvh.cn/Article/details/gyfbnnjyu.sHtML

[U08] Py：展平二维列表
来源：http://blog.fehbvm.com/Article/details/ghmuikyjk.sHtML

[y for x in nested for y in x]
来源：http://mobile.fehbvm.com/Article/details/gkmxxwrfi.sHtML


<!-- 参考信息 -->