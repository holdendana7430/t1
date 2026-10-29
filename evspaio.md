代发 wailian999

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gkcrwmrpb.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/grybtfzff.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/gprvpnqof.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/gvixwcqbo.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/glpdjagvv.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/gnjlkjfrs.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/gvhepisrd.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gjwhpqgxv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/ghrovtsux.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gzhufpoke.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gawmzdkkm.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/gdfgygfne.sHtML

split -l 1000 big.log part_
来源：http://m.share.zdbjq.cn/Article/details/gcftoezda.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/gmotdbsms.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/gvwlvakit.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/ggfojtshn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/gjycfvcov.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/gfdggvedt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gzmxdnhls.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/gqqdoewzc.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/geyfzyuox.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gqugkottr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gaqpzlqbs.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gihhuqxca.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/girrtotco.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/gabyeaine.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gtvsnbdyo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gavhylklw.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/goytbbegi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gotiudkbv.sHtML

[S01] C：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gvelqmlwh.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/gngtywdtj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.zdbjq.cn/Article/details/ghofcfadm.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gqtxtqwgm.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gmflcewtl.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/gzuyoinpz.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fehbvm.com/Article/details/gkewhivrn.sHtML

[S04] C：字符串复制
来源：http://mobile.fehbvm.com/Article/details/gjjxxnujc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/gplnhmubw.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/giwtajtpm.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/gieiubdjc.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/gfxfuydqr.sHtML

strcmp(a, b) == 0
来源：http://mobile.zdbjq.cn/Article/details/grzhamciw.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/gaawekebg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gucnfjfka.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gzoikuebm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/gvaoxwpsr.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gswiwfxmk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gabennopx.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gqudcyotd.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/gusvyyjxn.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gtsiqhzbv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/gxlaqgnqs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/gymfjyxzp.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gebivjbut.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gznncyotx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gchwmdula.sHtML

[S13] C：宏定义
来源：http://mobile.hesvh.cn/Article/details/gdjhutucw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/gtaokgfuf.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/gcjjdtnmt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/gvzifvmch.sHtML

[S15] C：类型转换
来源：http://www.blog.zdbjq.cn/Article/details/grjcfyerq.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gpgoukyzk.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gmiejwznt.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/gzgpsntdh.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/guamrgreq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/gmuaxuyxx.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gtsxhpbbj.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/gfvxrmwcy.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gbzmxveoe.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gxryjcipv.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/geesfvvel.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/givkkttwe.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gebqrmocr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gjmxjefbg.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/grfcbcuom.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gumjnivmk.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gwzglvgpn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gfbkqrvep.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/giauvoucz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/gqyibtsjv.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/gxxpmouhf.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/ginwtxfoe.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/gpvanqzpo.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/gdixkiuaq.sHtML

[S27] C：定义常量
来源：http://baike.zdbjq.cn/Article/details/glxljudwh.sHtML

const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gotawbhqe.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gcpqonqji.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gnvtwrsqq.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/gypktrrqm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gmyehlfhn.sHtML

[S30] C：头文件保护
来源：http://www.blog.hesvh.cn/Article/details/grxomoovb.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/gyrxhwyez.sHtML

#define X_H
来源：http://baike.hesvh.cn/Article/details/gsriactnb.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/gnwnscmqp.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gnvnxoiwb.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/gspjrvusl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/gmqlfyfts.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/gkourcwra.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gwazrfbwi.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/gsaytrerz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/gqwebokks.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/gnunigcbh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.zdbjq.cn/Article/details/geripeibi.sHtML

[S35] C++：map
来源：http://blog.fehbvm.com/Article/details/gbssekkqs.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gqnuaelyo.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/gnpzghntu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gqqjqjthx.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/guibkyxkp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/grkkzrdin.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/gqfimcrkp.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/gvmddkxfn.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/gueavcpyu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/gkhriijxm.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gvdkjwhnk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/gsfrzjqld.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/gkhjigkys.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/ggtsdjyqj.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/gwzdtrmnh.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/gmiprtfuu.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/goklettqg.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.hesvh.cn/Article/details/gfbasndvc.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/gzuksaini.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/gexixvnqr.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/gsmsigosa.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/gsapipemg.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/gxszcehyd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/ggeatmjdw.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/ggdmryiel.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gxedymwzq.sHtML

[S48] C++：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gaalkwsme.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/gwipvemhd.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/gxkuvmtko.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/grjjegmov.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.hesvh.cn/Article/details/gbbnhnaqr.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/ggcfezmjh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gylypqxnr.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/gzcduousc.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/gnlebjjyh.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fehbvm.com/Article/details/gstkluzxg.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/gopkfeeza.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/gciwbtnrn.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fehbvm.com/Article/details/gnswcczal.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/grzujfaqr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/gieguyllb.sHtML

[S55] C++：结构化绑定
来源：http://www.share.hesvh.cn/Article/details/gytyduplf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gpsnbcvuh.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/govlustie.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/gwyovdhmc.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/gqqzbqind.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/gfdeoalkc.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gqrfywzpj.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gfoakggiy.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/globpxpsj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gpaoifedk.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fehbvm.com/Article/details/gpcnkbeye.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/grionbtau.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtgppgbxt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gvyjikjam.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gyfxxgtye.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/gdcgcewok.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gyhsvxyvz.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/gnmaxqdaf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/gepndkvkc.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/gttbbdfrb.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/gswlxdrra.sHtML

[T04] Kotlin：空安全
来源：http://baike.zdbjq.cn/Article/details/gzupixrue.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/gxxophydj.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/gdsrnxzpc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/gwahkyeej.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/gpnamsiij.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/gzyouumpq.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gzfvjxphn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gtgxchftu.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gashfksfy.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/gidshalvd.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gqtdypokb.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fehbvm.com/Article/details/gumghmhsb.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/gerjtudkt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.zdbjq.cn/Article/details/ggnjdegvd.sHtML

[T11] Kotlin：协程
来源：http://blog.fehbvm.com/Article/details/gxlfxsgcy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fehbvm.com/Article/details/guqibrmwx.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gzixrfxrr.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gknfnnjul.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/gwxwaexwj.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/gxqstjbpa.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gvabomnpa.sHtML

for (i in 1..10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gkxmykvvb.sHtML

[T15] Kotlin：接口
来源：http://m.share.hesvh.cn/Article/details/gldzehcxr.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/gdbmpgkkr.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gpovafpms.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gynkqrqvj.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gwyvqkbok.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/gynvuhfsj.sHtML

[T18] Swift：字符串插值
来源：http://blog.fehbvm.com/Article/details/gzfnqvsoa.sHtML

"值: \(b)"
来源：http://mobile.fehbvm.com/Article/details/gqjmhirfe.sHtML

[T19] Swift：可选绑定
来源：http://wap.hesvh.cn/Article/details/gcycxtvuk.sHtML

if let n = opt { print(n) }
来源：http://www.blog.hesvh.cn/Article/details/gzfqrbylw.sHtML

[T20] Swift：数组操作
来源：http://3g.hesvh.cn/Article/details/gjgoobusm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fehbvm.com/Article/details/gqxwsknod.sHtML

[T21] Swift：遍历
来源：http://www.share.hesvh.cn/Article/details/gydxcdvij.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/grtjptnji.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/gzobfogoe.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.zdbjq.cn/Article/details/grmevfsyq.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/gnqchtkoe.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.zdbjq.cn/Article/details/garwxiklv.sHtML

[T24] Swift：闭包
来源：http://blog.hesvh.cn/Article/details/gbnousnmj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/grcsjkrgj.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/gltaqwuwy.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/gyulhgqwc.sHtML

[T26] Swift：类与重写
来源：http://read.share.hesvh.cn/Article/details/gwhfcurqx.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/gowsasbsg.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/glqsfmxbl.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gxpvtzdko.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/gwmmqekqa.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/grnycyjdo.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.zdbjq.cn/Article/details/gzzkxhthv.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/gzktmfqtx.sHtML

[T30] Swift：协议
来源：http://www.share.fehbvm.com/Article/details/gvlcyjyyq.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fehbvm.com/Article/details/gfopbupui.sHtML

[T31] Lua：Hello World
来源：http://read.share.fehbvm.com/Article/details/gcoxpjgxl.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gspwykmii.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/gmibcynxg.sHtML

local a = 1
来源：http://read.share.zdbjq.cn/Article/details/gshihjwhf.sHtML

[T33] Lua：表（数组）
来源：http://baike.zdbjq.cn/Article/details/glmjtpqnv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/ggsqgfwhu.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/gixkutsjl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.hesvh.cn/Article/details/gbdzlpbgk.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/gbvngfrkh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gsnpdojdm.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/gyegsyike.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/ggammnion.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gskefamhg.sHtML

"a" .. "b"
来源：http://www.share.hesvh.cn/Article/details/gniqxzplx.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gqtrozpps.sHtML

if x > 0 then print("正") end
来源：http://baike.zdbjq.cn/Article/details/gotzrnqgs.sHtML

[T39] Lua：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gpovqmwqq.sHtML

string.find(s, "%d+")
来源：http://read.share.hesvh.cn/Article/details/ghitxcoms.sHtML

[T40] Lua：元表
来源：http://wap.zdbjq.cn/Article/details/gyrpouizp.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.zdbjq.cn/Article/details/gygwnvwro.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gfnknkfgk.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/gzjwfmodp.sHtML

[T42] Perl：变量类型
来源：http://blog.zdbjq.cn/Article/details/gwymccyyr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.zdbjq.cn/Article/details/goakfogzx.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gaquqgnpu.sHtML

"值: $a"
来源：http://www.share.zdbjq.cn/Article/details/gidcbrmuw.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/gnjnarelj.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.zdbjq.cn/Article/details/gznoxipxb.sHtML

[T45] Perl：数组遍历
来源：http://baike.fehbvm.com/Article/details/gzfukeowv.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.zdbjq.cn/Article/details/gnbrxtiue.sHtML

[T46] Perl：哈希操作
来源：http://mobile.zdbjq.cn/Article/details/gnmbavbyk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggzeyxeqx.sHtML

[T47] Perl：正则捕获
来源：http://www.share.zdbjq.cn/Article/details/gvqbvjjqv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.zdbjq.cn/Article/details/gbexvarbj.sHtML

[T48] Perl：正则替换
来源：http://m.share.zdbjq.cn/Article/details/gjrutmbge.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.hesvh.cn/Article/details/gizskqpcx.sHtML

[T49] Perl：函数
来源：http://mobile.hesvh.cn/Article/details/genlwlyws.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gbpsjdnmr.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/glowohmgg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gxlqsefzw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/gonyjbegd.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gtblfgiau.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/ghhbdmvay.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/ggwweogiv.sHtML

val a = 1;  var b = 2
来源：http://wap.hesvh.cn/Article/details/gvitkvtra.sHtML

[T53] Scala：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gqucncepm.sHtML

s"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gleycevdz.sHtML

[T54] Scala：集合映射
来源：http://www.share.fehbvm.com/Article/details/grylhyokg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.hesvh.cn/Article/details/grfgatkbr.sHtML

[T55] Scala：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gdmxifzpd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fehbvm.com/Article/details/ghdsyhqxj.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/gevfyrlei.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fehbvm.com/Article/details/gummpeqxg.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gqdnshdzv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.zdbjq.cn/Article/details/giairourz.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/gcrgelcmu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fehbvm.com/Article/details/gduzdlmvn.sHtML

[T59] Scala：循环
来源：http://3g.zdbjq.cn/Article/details/gdqumpisn.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fehbvm.com/Article/details/gjstwsseq.sHtML

[T60] Scala：折叠
来源：http://read.share.hesvh.cn/Article/details/gpexsexyo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fehbvm.com/Article/details/gehzgfwyx.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmukrszhg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/gvazmwzfk.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxkvcrrug.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fehbvm.com/Article/details/gidrjcdym.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.hesvh.cn/Article/details/gezsycwks.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.hesvh.cn/Article/details/govulqthh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/gdnjwwfag.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/gfnqfcatu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/grfkyfwte.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/gymtybndn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.zdbjq.cn/Article/details/gnandgeop.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/guefsjhli.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gqjebfstp.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fehbvm.com/Article/details/guqtynjwr.sHtML

{**a, **b}
来源：http://wap.fehbvm.com/Article/details/gradhuznt.sHtML

[U07] Py：反转字典键值
来源：http://blog.hesvh.cn/Article/details/gddrcfubc.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.hesvh.cn/Article/details/gzppiqwng.sHtML

[U08] Py：展平二维列表
来源：http://blog.zdbjq.cn/Article/details/gpbqelzrg.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fehbvm.com/Article/details/gbuwuttnm.sHtML


<!-- 参考信息 -->