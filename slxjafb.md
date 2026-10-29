代发 wailian999

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/gakbixscj.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/gpxixhsfe.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gjyblybdy.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/gvdhdsubf.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/gpspsjegm.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/ggszsgtxj.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fehbvm.com/Article/details/gzfncehlt.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/ghxloakwv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/garenojiz.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/gxsdcdiqt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gwguqsous.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gzyjueevj.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gqnydywgv.sHtML

[R74] 批量重命名
来源：http://m.share.fehbvm.com/Article/details/gvngrpiuc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/guggvrypb.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gapjinknt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/ghtvanizc.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gkiddttss.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gxcczwrir.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/gpvgcyocj.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/gbefydnmu.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/gzsfxvpop.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gfcaiwpke.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gyfzgoufu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fehbvm.com/Article/details/gqycxklup.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/gujlrkvzf.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gjjsapinj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtjnsgycd.sHtML

S. C / C++ 专题
来源：http://m.share.fehbvm.com/Article/details/gqqxbdlxd.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtxkknjfp.sHtML

[S01] C：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gnxfpodlx.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gvvgsilbp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.zdbjq.cn/Article/details/gduiiukao.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/gpfgbqhjn.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/ghngqzeei.sHtML

[S03] C：读入整数
来源：http://m.share.hesvh.cn/Article/details/gpwxbwmhe.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/goxprquuj.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/gepfvyvgi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.zdbjq.cn/Article/details/gsmmrwfnd.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/gylehtgig.sHtML

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/gsxmkmfgt.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/gvfyxarts.sHtML

strcmp(a, b) == 0
来源：http://mobile.zdbjq.cn/Article/details/gyodqkeev.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/gsrisbrjv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/ggxvmjjcf.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.zdbjq.cn/Article/details/gphduneow.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/ggzuvlctf.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fehbvm.com/Article/details/gxwnagflw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/gforxtdbk.sHtML

[S10] C：指针与解引用
来源：http://www.share.hesvh.cn/Article/details/gkpxgonwc.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/gfjrkjjeu.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gmykcdtsi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/gurtflftv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gellznhxr.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gmueyxgvz.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/gjesszydm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gcrsfzlir.sHtML

[S13] C：宏定义
来源：http://baike.zdbjq.cn/Article/details/gsnydorfd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gjxogovbw.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gxmnhtsft.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/gaohltjkc.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/giqqiraws.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gijaejbsh.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gkbhmzcwu.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/glybynwnr.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gsursvcin.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.hesvh.cn/Article/details/gmujggifz.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gzowwfzem.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gzgjucnxi.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/gjzuswktr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gujciidws.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/gfzmgvewh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gamsnxbxw.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gpqidsncs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gkwjkkfvr.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gfnzjlehc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gilrcdyyt.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/gaezslowd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/gsjyyfmcq.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/gyzazbfgh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.hesvh.cn/Article/details/gjxjfslmr.sHtML

[S25] C：内存拷贝
来源：http://m.share.zdbjq.cn/Article/details/gpzgurktc.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/gpiqzziqm.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/gunmbvddl.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/gjrtndwwn.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/gtcxmyqbm.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gacczltgz.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/gajyvpmbm.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/gtnvwbdaw.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/gykxigaan.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gbbrnqhcy.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gtbgbouwk.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/givrfxiap.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/gucxkipts.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/gmzqkfyht.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gwzlogdrr.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gbgwoegjs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/gptzmlejs.sHtML

[S32] C++：字符串
来源：http://read.share.fehbvm.com/Article/details/gnybnjqlp.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/gdxzovpog.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/gktnwkkmw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/gbnqywdaa.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/gseufnhft.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/ggkpipgln.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/gaynbfqbc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gcjoioblm.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/galqgkwoq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gerhsjpaa.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/ggfotxwvx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gneifgqzy.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gxowedzyy.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gcfbxixau.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gpyqsctfw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/gwegxrsqo.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/gqciuuuay.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gefbyiult.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/ggtrlwzit.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gupuesxmx.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/gmignxidp.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gsydywpjz.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/gtseznzzu.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/gndhddpxf.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/gkfxenjmq.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.zdbjq.cn/Article/details/gocfachsw.sHtML

[S45] C++：lambda
来源：http://www.blog.hesvh.cn/Article/details/gtmzzzbcm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/gnnabfkci.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/gnmkzwepr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.hesvh.cn/Article/details/gfdpyckae.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/gscxsqymc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/gvsfonfmw.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gqkukwctt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/gujldirle.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/gvwyptohl.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/gjyqdlcev.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/gfjdhilyy.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/gqchnueal.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gwgcmrryz.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/gbknjzxgn.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/gxilhmwik.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/ghsrfugvb.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gtpfydhwq.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/gbnaranqq.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/gbcsxdyla.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gatmxxviy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gazvouolg.sHtML

[S55] C++：结构化绑定
来源：http://www.share.hesvh.cn/Article/details/gykaozxop.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gzdlmhdtn.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/gmcvxdczc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/gorqszodg.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/gmhifeteu.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/gbkrrxtwr.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/gspaqghzw.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fehbvm.com/Article/details/gqiblbaoe.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/gqosyiduy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.zdbjq.cn/Article/details/gosrczwye.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/gulkwfitm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gljavanli.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gswenueng.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gpfkpcmdx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/glbrwkrrm.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gbacxzxse.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gukhqrwjk.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.hesvh.cn/Article/details/gockqjswf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.zdbjq.cn/Article/details/gkbquptgn.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gmbotemal.sHtML

"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gszkznilh.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/gyqnpqzen.sHtML

val n: String? = null;  n?.length
来源：http://baike.fehbvm.com/Article/details/gilydpvfk.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/grdqdcsja.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/gkgtouick.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/gateiufsv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/gxoyqraxy.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gccbtloir.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/ghumrvdvi.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/grjvmdvla.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/gkwrhbwto.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.hesvh.cn/Article/details/gbrbtvwky.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/girddfkcd.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/gnnrijyjf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.zdbjq.cn/Article/details/gzjmqkklx.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/gqzktjtib.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/gwuctlbut.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/gihhacxyp.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/gvwxouppy.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fehbvm.com/Article/details/gygthpmdb.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/gnkpsqmpm.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/glepurkdy.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gdjbpwtnk.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/ggjxzubfo.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/gmfrmmltz.sHtML

[T16] Swift：Hello World
来源：http://wap.fehbvm.com/Article/details/gidbyahsh.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gtwxkqozt.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/gigdjnzwq.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gltkhlnty.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gzhtspcim.sHtML

"值: \(b)"
来源：http://www.share.fehbvm.com/Article/details/gxwqomvby.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gktdnnrsa.sHtML

if let n = opt { print(n) }
来源：http://m.share.zdbjq.cn/Article/details/gmonwkzlz.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/gmefaossr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.hesvh.cn/Article/details/glktrnenx.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/gqvwwvmwq.sHtML

for x in a { print(x) }
来源：http://blog.zdbjq.cn/Article/details/gljvnexlg.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/gmrczeplk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fehbvm.com/Article/details/gpkmqxzqm.sHtML

[T23] Swift：函数
来源：http://baike.zdbjq.cn/Article/details/gcvfrpzxn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.hesvh.cn/Article/details/gzjgpccps.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/glvqsycyn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/govgjgmtx.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/gwbmitwnp.sHtML

struct P { var x: Int }
来源：http://m.share.fehbvm.com/Article/details/gqgnnkonb.sHtML

[T26] Swift：类与重写
来源：http://baike.fehbvm.com/Article/details/goakmtitu.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/gfalfkwkk.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/gdwnukmlo.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/gaeepaapq.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/geqtlmuxf.sHtML

enum Color { case red, green }
来源：http://blog.hesvh.cn/Article/details/ghrxfxxaq.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.hesvh.cn/Article/details/gpwfkfpzm.sHtML

guard let x = opt else { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gwgznzyeb.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/gotskvtqx.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fehbvm.com/Article/details/gnohdgtce.sHtML

[T31] Lua：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gchmdyjvg.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gdbdvmkjh.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/ghxmdcdyh.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/geuudhfpf.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/gtzeajibn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/gihvzpuzw.sHtML

[T34] Lua：遍历表
来源：http://baike.fehbvm.com/Article/details/gqhaklvbo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fehbvm.com/Article/details/gsqexepeb.sHtML

[T35] Lua：字典表
来源：http://www.share.zdbjq.cn/Article/details/gwemhfavd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gfsxawxjs.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/gioccdmcb.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/geytjodnf.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gfhknkvhk.sHtML

"a" .. "b"
来源：http://wap.fehbvm.com/Article/details/gzkqarhui.sHtML

[T38] Lua：条件
来源：http://www.blog.zdbjq.cn/Article/details/gdpaejezw.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/gyniqocyo.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fehbvm.com/Article/details/griwrqpbk.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/goftpvpzc.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/gkajmaxrb.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.hesvh.cn/Article/details/gkumnlecw.sHtML

[T41] Perl：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gqrtzpayf.sHtML

print "Hello\n";
来源：http://blog.zdbjq.cn/Article/details/gcabckqtq.sHtML

[T42] Perl：变量类型
来源：http://baike.fehbvm.com/Article/details/gxsghcxgf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.hesvh.cn/Article/details/gbieboopu.sHtML

[T43] Perl：字符串插值
来源：http://baike.fehbvm.com/Article/details/gjwldnkfj.sHtML

"值: $a"
来源：http://3g.fehbvm.com/Article/details/gyszlukhp.sHtML

[T44] Perl：条件
来源：http://3g.hesvh.cn/Article/details/gtvbymqnc.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/gurtkxxhn.sHtML

[T45] Perl：数组遍历
来源：http://baike.zdbjq.cn/Article/details/giwgmjlfk.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkohptgyf.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.zdbjq.cn/Article/details/gjlnjlwrr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/gozqwunxh.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/gnlpwtvqp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.zdbjq.cn/Article/details/gverpbvob.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/gyxpgescz.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.zdbjq.cn/Article/details/gqzcaskgq.sHtML

[T49] Perl：函数
来源：http://baike.fehbvm.com/Article/details/gngtmijri.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gbapdfnbq.sHtML

[T50] Perl：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gtkhhurnr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.hesvh.cn/Article/details/gwuizlgnd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fehbvm.com/Article/details/gqeafrhuf.sHtML

[T51] Scala：Hello World
来源：http://baike.zdbjq.cn/Article/details/geukrsqwe.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gychjycsm.sHtML

[T52] Scala：变量
来源：http://www.share.hesvh.cn/Article/details/gxdepihot.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gukvswwpv.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/goblblalm.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/gvzdbdnop.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gamnzlvct.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.zdbjq.cn/Article/details/giwpsqayp.sHtML

[T55] Scala：集合过滤
来源：http://baike.hesvh.cn/Article/details/gdsbsqxsb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/gcbjkjsin.sHtML

[T56] Scala：样例类
来源：http://www.blog.fehbvm.com/Article/details/gxbnrfnow.sHtML

case class User(name: String, age: Int)
来源：http://m.share.hesvh.cn/Article/details/gzzkxuuno.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/giwqsqgir.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.hesvh.cn/Article/details/gfdlwanzo.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fehbvm.com/Article/details/gqkaztvhm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fehbvm.com/Article/details/gtcbttmdy.sHtML

[T59] Scala：循环
来源：http://3g.hesvh.cn/Article/details/gkaeyvwbk.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gyabfidrx.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fehbvm.com/Article/details/gfzgjxqui.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.hesvh.cn/Article/details/ghpnmebzi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdvgixpak.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gdsrmwigc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxjjfkaqy.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fehbvm.com/Article/details/gacsavdun.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.hesvh.cn/Article/details/gqdvyfvck.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fehbvm.com/Article/details/gmqbqplyt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fehbvm.com/Article/details/gaizcxcac.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/guqtdzcib.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.hesvh.cn/Article/details/gsmedsaop.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/gopaghvug.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/glwcmigts.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fehbvm.com/Article/details/ghxhchnuz.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gdidncnwo.sHtML

[U06] Py：合并两个字典
来源：http://read.share.zdbjq.cn/Article/details/gzawwxnkf.sHtML

{**a, **b}
来源：http://wap.fehbvm.com/Article/details/ggmbbtfzv.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.hesvh.cn/Article/details/gmdxtzeyr.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fehbvm.com/Article/details/gtrnrwdxh.sHtML

[U08] Py：展平二维列表
来源：http://www.share.zdbjq.cn/Article/details/gxgxsdbde.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/gvdrgqhxh.sHtML


<!-- 参考信息 -->