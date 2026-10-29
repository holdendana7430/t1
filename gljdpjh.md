代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/glgrptvop.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/ghzcgtqft.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/glawkcral.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gyfltkmgu.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/gnsgtlmaq.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/gglbgwzco.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.zdbjq.cn/Article/details/gylceaewp.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/goqjgsqbr.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/gfqksjyxd.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/gakvrmgth.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fehbvm.com/Article/details/gqdwmbfzv.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gzrokjvjy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.zdbjq.cn/Article/details/gstzwxcht.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gvcgburhi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gahdksizk.sHtML

[R73] 分割大日志
来源：http://blog.zdbjq.cn/Article/details/gehntskpy.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gybkmplyp.sHtML

[R74] 批量重命名
来源：http://m.share.fehbvm.com/Article/details/gkvjpucos.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/gjbqzsavs.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gdyznavlt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/gzndmhled.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gxspfvhyr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gkmccyvib.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/gttavvghl.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/gieaygktr.sHtML

[R78] 交互式菜单
来源：http://3g.zdbjq.cn/Article/details/gccaqsypr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/gmatvbywq.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/gbqtrwptk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fehbvm.com/Article/details/gohyrxbsw.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gimxsodfp.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/geovnjyzi.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzvllmmga.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/ghliqwgge.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbainkokv.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gcqjuywfs.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/gcnwohvbz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fehbvm.com/Article/details/gjlcmorrp.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/gszwmxlpo.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/glrqmoayi.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/gxtijjuwr.sHtML

int x; scanf("%d", &x);
来源：http://baike.fehbvm.com/Article/details/gdspuzbbl.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/gmmumkztj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.hesvh.cn/Article/details/gggesvzhc.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gdvlfxone.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gefnausrq.sHtML

[S06] C：字符串比较
来源：http://m.share.fehbvm.com/Article/details/grtkcjyym.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/gnarnnaim.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/gszqwnijg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/ggkncockz.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/gsuiwmoou.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gqoybokgw.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gooxdwacm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/gkkdxoegh.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/gtujcqugx.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/gcisxkakk.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/glduakxud.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/ggwvfeliu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/gucntgnol.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gkswtuaux.sHtML

[S12] C：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gzddemxou.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/ggxrybfpf.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/gljbqaxqd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/gedvqaisj.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/gbcjlibyn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/gubtlmfso.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/gtlhjecis.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/gmlrsjged.sHtML

[S16] C：位操作置位
来源：http://baike.fehbvm.com/Article/details/gfpedqfzu.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gnbdcxape.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gvdkzgwdg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gutrhhivi.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/gferdrhkc.sHtML

int main(int argc, char **argv)
来源：http://wap.hesvh.cn/Article/details/gnyvwsqql.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/gmvqxxjxk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gflmkctss.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/gnntvfkhe.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gerynwyyn.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/gzjsmysbl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/grxrnbcuk.sHtML

[S22] C：字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/geiaehmsb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/gestyuyjm.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gkjibuaze.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/gkxdimkoo.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/gxfdvlzht.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/gsuxjzjdb.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/ghyneoulx.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/gphpuuklz.sHtML

[S26] C：内存清零
来源：http://wap.fehbvm.com/Article/details/grgzflxtg.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gndiynwhc.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gskwmqqap.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gsbtjsjvo.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gdvhxbhrj.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gbjgajobj.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/gjduureuy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gmxuhdcef.sHtML

[S30] C：头文件保护
来源：http://www.blog.zdbjq.cn/Article/details/gsemacmkz.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/gioilxwef.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gosyxtxsl.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/gprvadnmr.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gwciyhvol.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/grjkpypqw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/gxomziirp.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/gusfhzsej.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/gclgmiyvd.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/gwblsmnne.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gfhvqjdbp.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.zdbjq.cn/Article/details/gwryhybvi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fehbvm.com/Article/details/gjfsopvan.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/gkvobkmxr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gwmcgbeuw.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/gfhhxgdrc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/ghxzqpvcj.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gxzjxdrhs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/givsmooiz.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/gxsxvndro.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/gyzyuqjbk.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/gwyqkrxcl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/ghhwplhrl.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gfkfsrtmf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gknecypac.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/genpkcjrs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/gtjtnuyqi.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/gefnfkrfn.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fehbvm.com/Article/details/gokigmhdv.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/gvhjikavq.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/gjfymtagp.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gyoybrujb.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/gsgvzihlj.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/grdqsmtlp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/gzykjwwut.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/gzgeevlge.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/gyxxpsuhw.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/geglfuplq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gxdtqprje.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gxkhpmisy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/glwqtpjuo.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/groeetmsi.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/gmhakdbqc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.zdbjq.cn/Article/details/gqcjqoalr.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/grrgkqmpl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gstwcgjvf.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gqhdugair.sHtML

static_cast<double>(a) / b
来源：http://m.share.zdbjq.cn/Article/details/godqkzdha.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gvxzeqkra.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/giskcfjrn.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/giumvfiqm.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/gixywlyar.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/gagcotykf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gkndcgwbs.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fehbvm.com/Article/details/ggshjgsam.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fehbvm.com/Article/details/gfoazmmzg.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/gnrzvwrbz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/ggzbepjwt.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/ggeznrycg.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/gziwmsars.sHtML

[S58] C++：命名空间
来源：http://blog.zdbjq.cn/Article/details/gjkztxjhu.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.zdbjq.cn/Article/details/gyunylaem.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/gkutdiowv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.zdbjq.cn/Article/details/gequwklhj.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/gplzncrzn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gmssqtykk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmtwyxzoj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gokfdsqbp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gelzipsqc.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/gqbjrkbkf.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/ghrilivwp.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/gryqasprx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/grgklnwal.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/gflgfhcst.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gojkuzabj.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/gvjgtxuld.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/gilkwacnm.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/gjuoehjfr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gzvznbelp.sHtML

[T06] Kotlin：集合映射
来源：http://3g.zdbjq.cn/Article/details/gvfxcuwhx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gbduktdql.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/ggaagoajk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/guzoxtrow.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/gmccqprfj.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gavvnyvst.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/gurffxtrz.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gevvgjcyo.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/gzzaadhyq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fehbvm.com/Article/details/gyyvtpzzw.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/gorqfqcbw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/ganjzhfti.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/gktqbjaje.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/gfgojlycd.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/gaudinccy.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.hesvh.cn/Article/details/gbfaylxte.sHtML

[T14] Kotlin：循环
来源：http://read.share.zdbjq.cn/Article/details/gmzntxshr.sHtML

for (i in 1..10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gktqgicba.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/grubdbood.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/grnqddzch.sHtML

[T16] Swift：Hello World
来源：http://baike.zdbjq.cn/Article/details/gxnjvsfup.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gieitmopa.sHtML

[T17] Swift：变量与常量
来源：http://baike.zdbjq.cn/Article/details/gqaaovcaw.sHtML

var a = 1;  let b = 2
来源：http://www.share.hesvh.cn/Article/details/gzrtqfmbe.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gwrhsqbkq.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/gifgmfjcr.sHtML

[T19] Swift：可选绑定
来源：http://baike.zdbjq.cn/Article/details/gmnugzria.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/gbanbsxwm.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/gvghkycdg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/gjxgbedyl.sHtML

[T21] Swift：遍历
来源：http://www.blog.fehbvm.com/Article/details/gmswuqjqg.sHtML

for x in a { print(x) }
来源：http://www.share.zdbjq.cn/Article/details/gvuquvjnz.sHtML

[T22] Swift：字典
来源：http://m.share.zdbjq.cn/Article/details/gtquqhxvh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/gyceuxnot.sHtML

[T23] Swift：函数
来源：http://baike.fehbvm.com/Article/details/gcunlooxg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fehbvm.com/Article/details/gfkuftyft.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/gnfnijdsb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gauwvucmk.sHtML

[T25] Swift：结构体
来源：http://mobile.zdbjq.cn/Article/details/gzgpbjeqv.sHtML

struct P { var x: Int }
来源：http://www.blog.fehbvm.com/Article/details/gynmcxiem.sHtML

[T26] Swift：类与重写
来源：http://baike.hesvh.cn/Article/details/gczcvlwen.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/gdrbotuzz.sHtML

[T27] Swift：错误处理
来源：http://www.share.zdbjq.cn/Article/details/gexibrrzw.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/geygwslwh.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/gkedjeitc.sHtML

enum Color { case red, green }
来源：http://3g.hesvh.cn/Article/details/gztwtmfan.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/goqxiysll.sHtML

guard let x = opt else { return }
来源：http://mobile.hesvh.cn/Article/details/gajcjzuuc.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/gswhdmcpi.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gtbrnxhar.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/glhnolfta.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gddovgocb.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/gmjygbhoo.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/gbqxkzehm.sHtML

[T33] Lua：表（数组）
来源：http://m.share.zdbjq.cn/Article/details/gwqmlfozz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/gezfcghet.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/gwympnvbq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/ghmjsyhlk.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/gspcftpdm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fehbvm.com/Article/details/gnzeguwua.sHtML

[T36] Lua：函数
来源：http://3g.fehbvm.com/Article/details/gjbamoxbf.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/gwwygymti.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gligziaef.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/gjkirhaqw.sHtML

[T38] Lua：条件
来源：http://mobile.fehbvm.com/Article/details/gtjzgwxwc.sHtML

if x > 0 then print("正") end
来源：http://baike.hesvh.cn/Article/details/geljtrvqi.sHtML

[T39] Lua：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gmnwughwl.sHtML

string.find(s, "%d+")
来源：http://3g.zdbjq.cn/Article/details/gtpendfqv.sHtML

[T40] Lua：元表
来源：http://www.blog.zdbjq.cn/Article/details/gahlomdgv.sHtML

setmetatable({}, { __index = base })
来源：http://wap.hesvh.cn/Article/details/grzuhywch.sHtML

[T41] Perl：Hello World
来源：http://read.share.fehbvm.com/Article/details/geasfchhb.sHtML

print "Hello\n";
来源：http://read.share.zdbjq.cn/Article/details/gzgmxudfp.sHtML

[T42] Perl：变量类型
来源：http://read.share.hesvh.cn/Article/details/glgfvrkzw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.zdbjq.cn/Article/details/gmadvelpu.sHtML

[T43] Perl：字符串插值
来源：http://wap.hesvh.cn/Article/details/grxlrcgbb.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/gzaeffwgm.sHtML

[T44] Perl：条件
来源：http://mobile.zdbjq.cn/Article/details/gyawyfosa.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.hesvh.cn/Article/details/gyfqzmlho.sHtML

[T45] Perl：数组遍历
来源：http://blog.zdbjq.cn/Article/details/gnkutkjwz.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/gbpkcqfgk.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fehbvm.com/Article/details/gnvqyecwx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzxhymbfa.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/gylmjmyym.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.hesvh.cn/Article/details/giysxmntq.sHtML

[T48] Perl：正则替换
来源：http://3g.zdbjq.cn/Article/details/gjhrrfhba.sHtML

$s =~ s/old/new/g;
来源：http://3g.zdbjq.cn/Article/details/gvfxebfup.sHtML

[T49] Perl：函数
来源：http://blog.fehbvm.com/Article/details/gwjjjsnke.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gvyyyupxx.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gxckcnlnw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.zdbjq.cn/Article/details/gbywiyvbw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.hesvh.cn/Article/details/gmezlopff.sHtML

[T51] Scala：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gpqhwivcm.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gufjvkjdf.sHtML

[T52] Scala：变量
来源：http://baike.zdbjq.cn/Article/details/gdmqksqqa.sHtML

val a = 1;  var b = 2
来源：http://3g.zdbjq.cn/Article/details/gfvnpjrep.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gfqqwxbhz.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gjgwiydos.sHtML

[T54] Scala：集合映射
来源：http://wap.zdbjq.cn/Article/details/gbofydamf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/gjhsijhdp.sHtML

[T55] Scala：集合过滤
来源：http://blog.fehbvm.com/Article/details/gakfuhcmz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/groqbmhhx.sHtML

[T56] Scala：样例类
来源：http://m.share.fehbvm.com/Article/details/gqkvcnqfy.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fehbvm.com/Article/details/gymptfzrl.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gmcwxjqge.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fehbvm.com/Article/details/goaiycamt.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fehbvm.com/Article/details/gkzdnfvvp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fehbvm.com/Article/details/gxmasmazp.sHtML

[T59] Scala：循环
来源：http://wap.fehbvm.com/Article/details/gtqqodykb.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gfcgfkuag.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/gwrswyvtf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.hesvh.cn/Article/details/gtxgirssl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glzksjjbz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gxdqcofdb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqnazspae.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.hesvh.cn/Article/details/gkhxcstfk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/gqehvvyyd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.hesvh.cn/Article/details/gxqwzhgri.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.zdbjq.cn/Article/details/gzxginpjz.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/gzmvcjamw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fehbvm.com/Article/details/gcjwkjwwo.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.zdbjq.cn/Article/details/gssquedyi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fehbvm.com/Article/details/gyfxizmsj.sHtML

[U05] Py：列表去重且保序
来源：http://baike.zdbjq.cn/Article/details/ggzevzgzr.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gsfalvloz.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fehbvm.com/Article/details/glpnzfugx.sHtML

{**a, **b}
来源：http://mobile.fehbvm.com/Article/details/gdzqvbpwo.sHtML


<!-- 参考信息 -->