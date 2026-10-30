代发 wailian999

openssl rand -hex 16
来源：http://www.share.hesvh.cn/Article/details/gqfhtfucg.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fehbvm.com/Article/details/gsisluwqk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/gmlqmfgby.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/gmxxssogm.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.zdbjq.cn/Article/details/gtfmgrkzu.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/gtywofeqr.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.zdbjq.cn/Article/details/gwlhborko.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gqrvvtxiz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gryjnqluy.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/gzwvfhvsm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gkgowobop.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gtmxvojbw.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/gqkzhproe.sHtML

[R74] 批量重命名
来源：http://www.share.hesvh.cn/Article/details/godvthewi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/gjdyjdkgw.sHtML

[R75] 导出环境变量
来源：http://blog.zdbjq.cn/Article/details/gbjdhcvlm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/gbbgvjpgk.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/ganjtumjl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gqbbmtquy.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gseyudvym.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/gcufprpuy.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/gyaeeuwxz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/goocfsnqr.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gpypxsfwg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gcdgosoay.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/gsofwxyqm.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/gcdtyyrhh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxjiipudy.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gzygnolbr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnhexzjib.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gmqtxfweh.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/gisqnswmx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/gskolavjv.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.zdbjq.cn/Article/details/gftghhxin.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gqxktwlgg.sHtML

[S03] C：读入整数
来源：http://www.m.share.fehbvm.com/Article/details/ggprurozl.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/gvscisfxf.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/gjonygmew.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/gspoieffu.sHtML

[S05] C：字符串长度
来源：http://blog.zdbjq.cn/Article/details/ghysiafcx.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/gyvnnttof.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gztjiizpk.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/gnnszykqh.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/gmawxfhcl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gjeilquhx.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/gdgxzptki.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.hesvh.cn/Article/details/ggjufqujx.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/giobmhshj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fehbvm.com/Article/details/gtmcikjed.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/gubqwgivz.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gbyxvpbsa.sHtML

[S11] C：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gtjkcfzle.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gdlktjmct.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/ghosjwbkg.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gnojpadys.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/gkiaisthm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fehbvm.com/Article/details/gwypfwpsx.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/ghjswmcan.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gcekhoomw.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/gdlzgnice.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.hesvh.cn/Article/details/gnifnjtnv.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/gsatfshdi.sHtML

(double) a / b
来源：http://m.share.fehbvm.com/Article/details/gnvnsncge.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/gchafdsoj.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/gqsjthedh.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gxkashmxk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/guvyqxppl.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/gvjccogyv.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/gbsksyqsa.sHtML

[S19] C：快速排序
来源：http://blog.hesvh.cn/Article/details/gddmfuequ.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gizwlxyqn.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/gkyonxert.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gneutbfbo.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/gdenddwjc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gtbbnfcae.sHtML

[S22] C：字符串转数字
来源：http://m.share.hesvh.cn/Article/details/grkxbhkbg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/ggbrrmnir.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/gkfxxbbtr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.hesvh.cn/Article/details/ggquinybl.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/geyrnzrzh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gdmbkrhdi.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gmuonnmos.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/gfcielfyi.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/gsaoudzqz.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fehbvm.com/Article/details/ggtsstter.sHtML

[S27] C：定义常量
来源：http://mobile.hesvh.cn/Article/details/geedemstp.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/ggzwidgsm.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/ghfjndegz.sHtML

static int counter = 0;
来源：http://baike.zdbjq.cn/Article/details/gfonrluws.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/gytzupucg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.hesvh.cn/Article/details/gxrgqixmu.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/gwsqttupv.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/gcdkfnaox.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gkfdoikne.sHtML

#endif
来源：http://www.m.share.fehbvm.com/Article/details/gubjrrnno.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gfdkybfqh.sHtML

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/giqdlnoir.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/gvbypqzse.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/getbqshtk.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/gzuinlhfz.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gmuvlolhv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/ghuwlrnyc.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fehbvm.com/Article/details/gjzjnkhil.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/grnlpxwcc.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/gyaznitmi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gtimpvgez.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/ggzmeldgt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gkmgcnnpw.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/ggyrjblwz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.hesvh.cn/Article/details/gcauynpsx.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/guxjdqwdq.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gxbkfvpup.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/gwtoowuig.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gcpdjxene.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/gbmhdtwvn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gconduuzj.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/gyxuzcpfj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gdtddmaqt.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/gbrqpxfzy.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/gbxgmkvpc.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/gzylswvyp.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gpvpbtkxi.sHtML

[S44] C++：引用传参
来源：http://wap.fehbvm.com/Article/details/gdbgeugjz.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/gmmraeird.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/ggvjszlfp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fehbvm.com/Article/details/glqkbybzo.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/gwqnomqcw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/gkdbloixe.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/gpmouozug.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.hesvh.cn/Article/details/gfdkvnghi.sHtML

[S48] C++：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gqshdarln.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/gtjizoahw.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/giucfdmzn.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/gsunnadhb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gglgljgnc.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/gtbxutkyg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/gqjgxgjje.sHtML

[S51] C++：显式类型转换
来源：http://blog.zdbjq.cn/Article/details/gehiglxja.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/gfqtsmqlr.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gsaflluen.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/gsncjqafe.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gsfylrdtl.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gcpewxain.sHtML

[S54] C++：异常处理
来源：http://3g.fehbvm.com/Article/details/gzpmejchw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.hesvh.cn/Article/details/gmzrciife.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/gpiwsdkzu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gxmcxmysb.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gpitanrmx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/gjbxgfwbm.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/gxmqhdbgd.sHtML

constexpr int N = 10;
来源：http://wap.zdbjq.cn/Article/details/gughqplah.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/geholjvyk.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/gafvrkpju.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/glkkeceit.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/geajjzydg.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gavdugimx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/gppkzvrbh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gahkzuttj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gaxcutuun.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggverfqdj.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gokfcntdh.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gbafwefuu.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/gegdaulqv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/gnkxbzkrg.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gyzzlmmwq.sHtML

"值: $b"
来源：http://3g.fehbvm.com/Article/details/gsdmzqrqh.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/gtbnnkbqy.sHtML

val n: String? = null;  n?.length
来源：http://3g.zdbjq.cn/Article/details/ghpnhegdq.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/gmhgqxisq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gqhbgpucm.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/ghiajtapv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gxtanllfh.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gnhohdjuk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/gicdfowuv.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/gbfgpsxkq.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/gslqslqiy.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/gaausgqjr.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/gzvrlrdrc.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/glzokmwqz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/gokcyulpv.sHtML

[T11] Kotlin：协程
来源：http://3g.hesvh.cn/Article/details/gmbufbuxk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/guduxhxjz.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/gtqjqvpfa.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/gyvcuwyhk.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/gpnenxzkc.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/gaxcachuk.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gvpgddmig.sHtML

for (i in 1..10) println(i)
来源：http://3g.hesvh.cn/Article/details/gwsiumrep.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/gyyngpxbc.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/gnduonldk.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/gyouvcbum.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gjvtummwe.sHtML

[T17] Swift：变量与常量
来源：http://m.share.hesvh.cn/Article/details/gretzuuaz.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/gjsvonumv.sHtML

[T18] Swift：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gpvvbqfkh.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/gncyrrvxq.sHtML

[T19] Swift：可选绑定
来源：http://baike.zdbjq.cn/Article/details/gluoeshry.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fehbvm.com/Article/details/ggghxsqkx.sHtML

[T20] Swift：数组操作
来源：http://3g.zdbjq.cn/Article/details/gkvwestnk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fehbvm.com/Article/details/gilnamkhp.sHtML

[T21] Swift：遍历
来源：http://mobile.zdbjq.cn/Article/details/gsaycdtep.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/gqjdwwpuy.sHtML

[T22] Swift：字典
来源：http://baike.hesvh.cn/Article/details/gesssrhbp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.hesvh.cn/Article/details/gshgdvjnt.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/gcyiiwexc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/gtumcwtjc.sHtML

[T24] Swift：闭包
来源：http://m.share.zdbjq.cn/Article/details/gyclatluj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.zdbjq.cn/Article/details/ggxwxpbtd.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/gwivjrraj.sHtML

struct P { var x: Int }
来源：http://www.blog.zdbjq.cn/Article/details/gttodmgbc.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/gaifhdjxc.sHtML

class A: Base { override func f() {} }
来源：http://blog.hesvh.cn/Article/details/geektkemp.sHtML

[T27] Swift：错误处理
来源：http://wap.hesvh.cn/Article/details/gdlubelfj.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/gqrtgvgiu.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/gpttptvbo.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/gktxgfkhu.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.zdbjq.cn/Article/details/gtdfycljz.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/gdeipfnic.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gdxvnriar.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fehbvm.com/Article/details/gszykwlzn.sHtML

[T31] Lua：Hello World
来源：http://www.share.fehbvm.com/Article/details/gxcggxtdg.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gcsjlecsn.sHtML

[T32] Lua：局部变量
来源：http://m.share.hesvh.cn/Article/details/gioosiwku.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gwaordbbi.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/gjooozlol.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.hesvh.cn/Article/details/gmibmxoyb.sHtML

[T34] Lua：遍历表
来源：http://wap.fehbvm.com/Article/details/gwplvrqlo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.zdbjq.cn/Article/details/gieynyuqg.sHtML

[T35] Lua：字典表
来源：http://wap.fehbvm.com/Article/details/ganohcqpe.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.zdbjq.cn/Article/details/giidkjafc.sHtML

[T36] Lua：函数
来源：http://m.share.hesvh.cn/Article/details/gyuiclkes.sHtML

function add(a, b) return a + b end
来源：http://m.share.zdbjq.cn/Article/details/gokbiuvsu.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gfgzsnnmu.sHtML

"a" .. "b"
来源：http://read.share.zdbjq.cn/Article/details/glkudxfqs.sHtML

[T38] Lua：条件
来源：http://blog.zdbjq.cn/Article/details/gjgvmdqav.sHtML

if x > 0 then print("正") end
来源：http://read.share.fehbvm.com/Article/details/gyywmdaha.sHtML

[T39] Lua：模式匹配
来源：http://3g.hesvh.cn/Article/details/gltyqxfap.sHtML

string.find(s, "%d+")
来源：http://baike.zdbjq.cn/Article/details/gbqsqqvgf.sHtML

[T40] Lua：元表
来源：http://3g.hesvh.cn/Article/details/gdlmshqeu.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fehbvm.com/Article/details/gazlktbpt.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/gbiubxkyz.sHtML

print "Hello\n";
来源：http://3g.hesvh.cn/Article/details/gehngbenw.sHtML

[T42] Perl：变量类型
来源：http://wap.zdbjq.cn/Article/details/gcbphrkqv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fehbvm.com/Article/details/gqtdkvnbt.sHtML

[T43] Perl：字符串插值
来源：http://blog.fehbvm.com/Article/details/gigpcrsfh.sHtML

"值: $a"
来源：http://baike.zdbjq.cn/Article/details/gdggpwafu.sHtML

[T44] Perl：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gdtdnwtne.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.hesvh.cn/Article/details/glkjicqfc.sHtML

[T45] Perl：数组遍历
来源：http://blog.zdbjq.cn/Article/details/gxphtiymc.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gizzltchj.sHtML

[T46] Perl：哈希操作
来源：http://mobile.hesvh.cn/Article/details/gdzztabpq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/ghqdpcojc.sHtML

[T47] Perl：正则捕获
来源：http://read.share.zdbjq.cn/Article/details/gnnuaiupi.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.zdbjq.cn/Article/details/glqrznxbe.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gfrahmrwi.sHtML

$s =~ s/old/new/g;
来源：http://mobile.zdbjq.cn/Article/details/gxvxohkym.sHtML

[T49] Perl：函数
来源：http://wap.hesvh.cn/Article/details/gednsicdo.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gokdftlnm.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gknlgzcfg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.zdbjq.cn/Article/details/gbyqisvym.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.hesvh.cn/Article/details/gwhtaugot.sHtML

[T51] Scala：Hello World
来源：http://blog.hesvh.cn/Article/details/gpfodcoaq.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gifcjebix.sHtML

[T52] Scala：变量
来源：http://wap.hesvh.cn/Article/details/gmofurjdo.sHtML

val a = 1;  var b = 2
来源：http://m.share.fehbvm.com/Article/details/gussxqitg.sHtML

[T53] Scala：字符串插值
来源：http://3g.fehbvm.com/Article/details/gvovvpiwg.sHtML

s"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gcuikzkba.sHtML

[T54] Scala：集合映射
来源：http://www.share.fehbvm.com/Article/details/gjgefaufx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fehbvm.com/Article/details/gqleiwqhs.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gafivzefu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.hesvh.cn/Article/details/gmtgwiifb.sHtML

[T56] Scala：样例类
来源：http://read.share.zdbjq.cn/Article/details/gjisovyxn.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/gynoetfnb.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gxybvkuky.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.zdbjq.cn/Article/details/ghpegdbax.sHtML

[T58] Scala：函数定义
来源：http://read.share.fehbvm.com/Article/details/gxitxzeeb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.hesvh.cn/Article/details/grrmxnoga.sHtML

[T59] Scala：循环
来源：http://m.share.hesvh.cn/Article/details/goukatoln.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.hesvh.cn/Article/details/gybqcqcbo.sHtML

[T60] Scala：折叠
来源：http://mobile.fehbvm.com/Article/details/grocuyeyl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fehbvm.com/Article/details/glbmusxlo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjnwjvbfl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gfdyqemaq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggcztelnw.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.zdbjq.cn/Article/details/gabktnzqt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/gyftdmtww.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.zdbjq.cn/Article/details/gavlqevbn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.zdbjq.cn/Article/details/gahwxtres.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fehbvm.com/Article/details/gautqurjf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.hesvh.cn/Article/details/grdsjxxrm.sHtML

[U04] Py：变量调试打印
来源：http://3g.hesvh.cn/Article/details/gosymzqls.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fehbvm.com/Article/details/gyidzihvm.sHtML

[U05] Py：列表去重且保序
来源：http://wap.hesvh.cn/Article/details/gnnxqhyxz.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gjtuzficw.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fehbvm.com/Article/details/grbyagwyp.sHtML

{**a, **b}
来源：http://mobile.hesvh.cn/Article/details/gjkgydnih.sHtML

[U07] Py：反转字典键值
来源：http://3g.hesvh.cn/Article/details/gcccsirug.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fehbvm.com/Article/details/gfbqtwbyf.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fehbvm.com/Article/details/giyavgvfl.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/gkepcfack.sHtML


<!-- 参考信息 -->