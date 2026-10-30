代发 wailian999

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/goylcuemu.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/gnavddejf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/ghsczbucn.sHtML

[R69] 生成随机密码
来源：http://m.share.hesvh.cn/Article/details/gvadblupo.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gpburbiyj.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/gboxojejf.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/ggtfcntho.sHtML

[R71] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gfmbbtcpg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/grefrquvb.sHtML

[R72] 等待端口就绪
来源：http://3g.fehbvm.com/Article/details/gjwlwmqcj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gmvubgdqu.sHtML

[R73] 分割大日志
来源：http://read.share.hesvh.cn/Article/details/gvmadfvgj.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.hesvh.cn/Article/details/goubxjoua.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gbhgomdgl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gnuqcylhf.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gnbeyailo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/gdyovvpjm.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/gmcltvdsa.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gzkwkiuzc.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/ghddbcwfw.sHtML

read -rp "请输入: " ans
来源：http://www.blog.hesvh.cn/Article/details/gehragjzf.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gdzljfaps.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fehbvm.com/Article/details/gvbnpgerv.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/gzkcqovga.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/gvunbcciq.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/getfniytm.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/guxmerrmy.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glqvddjzd.sHtML

S. C / C++ 专题
来源：http://wap.fehbvm.com/Article/details/gienusptc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gslsnbfuq.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/gpbfmdows.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/gjculcafn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.zdbjq.cn/Article/details/gviigagyx.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/gcvuvpuxx.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gdxwhvahr.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/ghdicqcue.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/glzdrmobx.sHtML

[S04] C：字符串复制
来源：http://mobile.fehbvm.com/Article/details/gswbfjjcu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/gojqaoesc.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/ghkanozba.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/gydjntbzw.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/gfthmmmae.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/grwncszzm.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/gmnjbnuhl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/gwgskvocq.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gvdxiyaha.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fehbvm.com/Article/details/grwahsudi.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gtunchdbl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/gyvidnodv.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gdgbboajz.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.hesvh.cn/Article/details/gvsyevdti.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/ggfnmxuen.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/gmirdgzek.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fehbvm.com/Article/details/gczulruds.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/gezzwdude.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/gzrjlxobr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gqiejpjdt.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/ggcwuawui.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/ghxommdlc.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/gywtypjxv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/gjmizjyof.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/gnwybnjza.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gcublgoze.sHtML

[S16] C：位操作置位
来源：http://baike.fehbvm.com/Article/details/gjlvutfch.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/gdxtwwwdj.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gxelfbxoy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/gwcckpyfg.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/gvduuwaux.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/grejeyedu.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/giybavtzr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gfsyjvvdb.sHtML

[S20] C：二分查找
来源：http://wap.hesvh.cn/Article/details/gbqgfdtbp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gqgsztrtz.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/gtffnnkrx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/gothuqgyq.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/grgekiyfg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/gxzwudevc.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/gtgwrdujn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/gpliofhto.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gdpckqmsd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/ghoprshop.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gbfmfnhdq.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gxzyyguhh.sHtML

[S26] C：内存清零
来源：http://wap.hesvh.cn/Article/details/guqzqpvwn.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/gzncfsmcb.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/ggarzyolo.sHtML

const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gyjtjbdia.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gctzookxn.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/gqvvzrjps.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gszmhtmbv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.hesvh.cn/Article/details/gsyvmdspg.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gibtcxbdx.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gonnxrsgy.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/gfoagckxq.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gpweasmpa.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gotcmdymm.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/gdtjlfhix.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/gtmtmthex.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/gvlaeshws.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/gsbntcgur.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/ghidoxxhq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/gldvuysaf.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/gwzbhtdab.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/gugvshtac.sHtML

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/gbheycsms.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gowbimyjr.sHtML

[S36] C++：unordered_map
来源：http://baike.zdbjq.cn/Article/details/ghyskycmw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gvhtizbvv.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/gcdyfqjfh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/guvczbtse.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/gsyrtsqvs.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/ggiohvpob.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.hesvh.cn/Article/details/gkmimnrbs.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/gvekxload.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fehbvm.com/Article/details/gpcaqxifo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gzdsyzcyn.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gmtkcvpgy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/gtncdxjfw.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gsogsotkn.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/gkddnyssv.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gsxmrvbek.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/gcldljvfc.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gfysuuktv.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/grjedumnq.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/guzfucjkq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/gpwzmpqpl.sHtML

[S46] C++：函数模板
来源：http://read.share.zdbjq.cn/Article/details/gvzcqwinf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/gvaomlxqm.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/ggdiammea.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gumidzkhv.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gyhoxpdgz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/gdtqlyczp.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fehbvm.com/Article/details/gpyigwajo.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gjnxgbngu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/gomqcedsm.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gsziydpgo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gyscpyifp.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/gioulfiyz.sHtML

static_cast<double>(a) / b
来源：http://m.share.hesvh.cn/Article/details/gopuqghjc.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/gulgtjuto.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/gngzlacrp.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/guulpizlq.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gzxcvrovk.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/gkhmnzmrf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gyhdqaems.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/ggigvzkos.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fehbvm.com/Article/details/gsphfbgkq.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gdrbzktms.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.zdbjq.cn/Article/details/gxpvqsdnw.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gqmfsiurt.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gzbbpsdov.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gqbollxih.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gfrqgqoqi.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/gzaqkfcbd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.zdbjq.cn/Article/details/gmfkaqdui.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gnshcufvd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/gspeskfen.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/guosrkokj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gyoyjycdc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/goorxqodl.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fehbvm.com/Article/details/ginhhswtc.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/glhrtdppw.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/gytowoaqq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fehbvm.com/Article/details/gbbqvsqht.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/giqpliptw.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gvsjulvxg.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gxryqpega.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/gandblrbh.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/gnctcojek.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.zdbjq.cn/Article/details/goywifobw.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/gwqmamccu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/gocsxwtbo.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/goublmtog.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/gcxodmnvt.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/gnrxmmxvv.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gulesttsw.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.hesvh.cn/Article/details/gaopcvjxp.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fehbvm.com/Article/details/goayrtsag.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gurayhiej.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/gyzokztog.sHtML

[T11] Kotlin：协程
来源：http://blog.fehbvm.com/Article/details/gbgulbynw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/gliaxqzqt.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/ggufzcmoc.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gnkhokikl.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.zdbjq.cn/Article/details/gcehmdual.sHtML

val m = mapOf("a" to 1)
来源：http://baike.zdbjq.cn/Article/details/ggxybhpue.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/gjqpkckzm.sHtML

for (i in 1..10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gbfzewogp.sHtML

[T15] Kotlin：接口
来源：http://read.share.hesvh.cn/Article/details/gbhdcflly.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gppocljbv.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gcoiaadzm.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gtisrftvz.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/gevquriid.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/grvpjyffc.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gxcpnbpun.sHtML

"值: \(b)"
来源：http://www.blog.zdbjq.cn/Article/details/gmehjxygt.sHtML

[T19] Swift：可选绑定
来源：http://www.share.zdbjq.cn/Article/details/gseljtjie.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/gbtvvsrgv.sHtML

[T20] Swift：数组操作
来源：http://read.share.hesvh.cn/Article/details/gpxvsemtc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.zdbjq.cn/Article/details/ghwwanwzd.sHtML

[T21] Swift：遍历
来源：http://read.share.hesvh.cn/Article/details/ghqntcufm.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/ghlgqazvw.sHtML

[T22] Swift：字典
来源：http://mobile.hesvh.cn/Article/details/gxmkmwuna.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gtsuaixjo.sHtML

[T23] Swift：函数
来源：http://3g.hesvh.cn/Article/details/gobatdjaz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.zdbjq.cn/Article/details/glcpqbfzw.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/gvwicmenu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gxhsurudz.sHtML

[T25] Swift：结构体
来源：http://3g.zdbjq.cn/Article/details/gcojohaxd.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/giikobrwb.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gjkzlkepu.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/gfestlppu.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/gkpnagtaa.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.zdbjq.cn/Article/details/gzmqjebnw.sHtML

[T28] Swift：枚举
来源：http://m.share.fehbvm.com/Article/details/gpysoibrn.sHtML

enum Color { case red, green }
来源：http://www.m.share.fehbvm.com/Article/details/grwsdmowb.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/gklofpmdb.sHtML

guard let x = opt else { return }
来源：http://read.share.fehbvm.com/Article/details/ggpciqiem.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/gejzeutjd.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.hesvh.cn/Article/details/gcvdauoqv.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/gqjeycsiw.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/galjcovpw.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gutiwhtah.sHtML

local a = 1
来源：http://blog.zdbjq.cn/Article/details/gtyrsgrmh.sHtML

[T33] Lua：表（数组）
来源：http://m.share.zdbjq.cn/Article/details/gabyedtwj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.zdbjq.cn/Article/details/gjmkrmqvt.sHtML

[T34] Lua：遍历表
来源：http://wap.hesvh.cn/Article/details/gwqsrynmq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.hesvh.cn/Article/details/giezkoaeb.sHtML

[T35] Lua：字典表
来源：http://www.share.hesvh.cn/Article/details/gajfridsg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/gxjquoiem.sHtML

[T36] Lua：函数
来源：http://mobile.fehbvm.com/Article/details/gkrekgyly.sHtML

function add(a, b) return a + b end
来源：http://baike.zdbjq.cn/Article/details/gldieynqr.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gcnlewjeb.sHtML

"a" .. "b"
来源：http://m.share.fehbvm.com/Article/details/gcxsxedad.sHtML

[T38] Lua：条件
来源：http://mobile.fehbvm.com/Article/details/gwtzpzyre.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/gnifkhlhb.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/grmsngkin.sHtML

string.find(s, "%d+")
来源：http://wap.hesvh.cn/Article/details/gzncueaxc.sHtML

[T40] Lua：元表
来源：http://blog.zdbjq.cn/Article/details/gaqwkjkpz.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/givwbdtrm.sHtML

[T41] Perl：Hello World
来源：http://wap.hesvh.cn/Article/details/gbshoqygo.sHtML

print "Hello\n";
来源：http://read.share.hesvh.cn/Article/details/gsrxlyfkg.sHtML

[T42] Perl：变量类型
来源：http://read.share.hesvh.cn/Article/details/goarsjbum.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fehbvm.com/Article/details/gowacqzev.sHtML

[T43] Perl：字符串插值
来源：http://wap.hesvh.cn/Article/details/gdflvwqht.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/gpoprdcbq.sHtML

[T44] Perl：条件
来源：http://www.share.fehbvm.com/Article/details/gmcsckmqk.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/giurzrzdz.sHtML

[T45] Perl：数组遍历
来源：http://m.share.zdbjq.cn/Article/details/gdtmozwwt.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fehbvm.com/Article/details/gyewoikcp.sHtML

[T46] Perl：哈希操作
来源：http://3g.zdbjq.cn/Article/details/gphdwopvv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fehbvm.com/Article/details/gtemtiaai.sHtML

[T47] Perl：正则捕获
来源：http://read.share.zdbjq.cn/Article/details/gepqozugp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/ghlalmhsa.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.hesvh.cn/Article/details/glxcrrrka.sHtML

$s =~ s/old/new/g;
来源：http://blog.hesvh.cn/Article/details/gccmugzup.sHtML

[T49] Perl：函数
来源：http://mobile.hesvh.cn/Article/details/gloqdroai.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gnebupgjz.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gwgjfjgcn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fehbvm.com/Article/details/gevfwjntx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fehbvm.com/Article/details/ggfmsmsuw.sHtML

[T51] Scala：Hello World
来源：http://3g.fehbvm.com/Article/details/gtczupjfl.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gbaqvmklo.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/glgumrsfe.sHtML

val a = 1;  var b = 2
来源：http://baike.fehbvm.com/Article/details/gmrjpmiyx.sHtML

[T53] Scala：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gkrcrnpyu.sHtML

s"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gblypyisy.sHtML

[T54] Scala：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gydpmszjc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.zdbjq.cn/Article/details/gedbyicfd.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gzqtfbice.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.hesvh.cn/Article/details/gbsybtdxt.sHtML

[T56] Scala：样例类
来源：http://read.share.fehbvm.com/Article/details/gmgjnxxui.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/gbgqkasrk.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gnbtixsqd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/guctsqckc.sHtML

[T58] Scala：函数定义
来源：http://www.blog.zdbjq.cn/Article/details/gylilxehc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fehbvm.com/Article/details/glybuwaig.sHtML

[T59] Scala：循环
来源：http://wap.fehbvm.com/Article/details/gzbjacees.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gpzbgcxom.sHtML

[T60] Scala：折叠
来源：http://baike.hesvh.cn/Article/details/gxfbwdqjs.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.hesvh.cn/Article/details/gjvvjgzpv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvoyyhakx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/glnyyqpzx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbsnsnhjr.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.hesvh.cn/Article/details/gdcwiqpwe.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fehbvm.com/Article/details/gxgroyjxf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fehbvm.com/Article/details/gkarrzwwe.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fehbvm.com/Article/details/gevetxcsc.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fehbvm.com/Article/details/gksfaopgs.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.hesvh.cn/Article/details/gsdeqcfai.sHtML

[U04] Py：变量调试打印
来源：http://read.share.hesvh.cn/Article/details/ggoktatwl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/gucubxcej.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/gqbxsryzn.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gujqvczph.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.hesvh.cn/Article/details/gicnxnwrz.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/gypnzewlv.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/ggvurafaf.sHtML

{v: k for k, v in d.items()}
来源：http://3g.hesvh.cn/Article/details/gumewjbsp.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.hesvh.cn/Article/details/goxgacjgm.sHtML

[y for x in nested for y in x]
来源：http://read.share.hesvh.cn/Article/details/gpxnzeyyx.sHtML


<!-- 参考信息 -->