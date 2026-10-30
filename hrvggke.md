代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gmlnfkzaz.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gfyjoewjy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gwcdtraxl.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjnvkgpt.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhongscp.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gketweevs.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqaadqkh.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gvdeahffo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gezwlnqbc.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gbglcitzl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gmdinfpzk.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gtxcqjsmz.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gfldscwen.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnptbwwc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqfnjger.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gtibvxitm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gfypwnywv.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/grsowyszd.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gxdzsrsod.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvvplpmd.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gshpyrpxe.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gdiwgswta.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorkcygmu.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkdoygsf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmofewro.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gufiiipwb.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gmqtnhxvq.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacrxggsq.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowhtksao.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/glzjcdjro.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjlqipdv.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gahsmaspk.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/giuiwlwqd.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/ghuerillw.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkevptao.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gqfxaslat.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gltbyqlbl.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/guecayxud.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljxnmyra.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzcqycmn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxtytvcr.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gyedkmqbp.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gurcvnqwv.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghrznibk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojytggwn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gdjaswawu.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhyawbgx.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqbttxig.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gdgglolzr.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxywzshj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzotbmrj.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/garyxeerp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gqvxxfaza.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gjnzpjzhz.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gugenquvw.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gboqfxjfh.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyoyblnoq.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcyfaxrz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzisxutzu.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/geixwqnhr.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhgijvwe.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzzjhjwl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gmnmxsfno.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvwhpcxv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/giqhzcddu.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gioowrans.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwvmnyxq.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqpqbwdx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gxobfstfz.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gvgzxawfb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gfwyfalca.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gsdtzvohz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwauneeph.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gxmyfsrow.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsxsbkrk.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzrxbojq.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblngagxt.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gohoowehu.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqzhpedz.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gemlkmdvl.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxsosxai.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gaeogwbfc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/goiyvzcht.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/guimzhjiy.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gsbddlodu.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gsihkvrnt.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/grednvrhl.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvnfvrvm.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhchvjkv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpedlyoyx.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gkargqxbi.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/geajxnzmq.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohrelmza.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqgmboef.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgjrpwgl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqnfcqokp.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzliueyl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gkusvndry.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gdpsccnqg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbgjixgd.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gngmpwatb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzgerzfv.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxkxihdm.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqbtvbnr.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gizckdzvt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gbktehztv.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gnylvlofl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gpmcgndtc.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbemtnuuf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/guimgicds.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/guhivqkpu.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvbwyrfv.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqplpizf.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvrnomli.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/grlgeijsz.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grymkpxyn.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gxlahhmyw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/grxykzzox.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/gkhkfipaa.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwvyzmpnc.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/glshvehfa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/guxhmoecd.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmfubiia.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjvkgovf.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gztufxvff.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gqyjbdsuw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyghptfvj.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gamwwdcvk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfpvbngg.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilhnvjyr.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gihevdfjk.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/godytborn.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkpagvuh.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gxmvewzhh.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gaixegxgp.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/guegkkugj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvdlzkap.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/geekqvfgw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gnjccsmyd.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsyeemte.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlcbvcik.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gxuunsdln.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtfxfubr.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvbuqhit.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gnyhfkzbj.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/ghogkvdbl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlcedsun.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gmatnnlgg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gkzkkhihu.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxvpawxc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidlclizn.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gjooebldr.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/guudccqet.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjnihgcb.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gqzgdjiwc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gumidyrgz.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecmuhvfh.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjyjjoagf.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/grrjixpsl.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/ggwyvmjju.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmodcfyb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyhaymsh.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gylwjohrv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqnppcrj.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gunlitagt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guypozqbn.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/ggplpmlog.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/ggsfjqcpz.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfscwznzr.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwwfnclc.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwydplzqh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/goscjltqc.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/gvvtruwsz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmfvieye.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/graeoazjs.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwehpvdyf.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gghyiyphp.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmynwsvxn.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gmzyclvif.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gotviotzf.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbveqqkhc.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gtusnerrh.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gcymjafpo.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gennreznk.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpvqfjab.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpkrybpy.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtzmyqcp.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuupyxoz.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwamgcxwt.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/gqhvspepi.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/gbwyosrpr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gycrtrokc.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gweziibwo.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfssskwr.sHtML

[T22] Swift：字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnlcbbmz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fanxiaobao.xyz/Article/details/glpxldvsj.sHtML

[T23] Swift：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahtbnxzo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjtvxjjk.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/goolmmdyf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqoopvsy.sHtML

[T25] Swift：结构体
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfjblchg.sHtML

struct P { var x: Int }
来源：http://3g.fanxiaobao.xyz/Article/details/grjdhktir.sHtML

[T26] Swift：类与重写
来源：http://wap.fanxiaobao.xyz/Article/details/gpmatsaxl.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/gnlgmxpii.sHtML

[T27] Swift：错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gntcyakok.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfztxlpm.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gouzbghtq.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/gtldjgdki.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/gzxlxtong.sHtML

guard let x = opt else { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyeotvgbf.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/gtmixlzjy.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqqcqckk.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvihbobvr.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gwkaefnvh.sHtML

[T32] Lua：局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gctmabrso.sHtML

local a = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmtmrlbb.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrpjisjn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/gqpjoawju.sHtML

[T34] Lua：遍历表
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxpdxtha.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fanxiaobao.xyz/Article/details/gpzjlezet.sHtML

[T35] Lua：字典表
来源：http://m.share.fanxiaobao.xyz/Article/details/gibyhydyf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyzjkwwi.sHtML

[T36] Lua：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzwhrenz.sHtML

function add(a, b) return a + b end
来源：http://www.share.fanxiaobao.xyz/Article/details/gggtzqkmm.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gfrnkxdig.sHtML

"a" .. "b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnecjoaw.sHtML

[T38] Lua：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcwmpena.sHtML

if x > 0 then print("正") end
来源：http://m.share.fanxiaobao.xyz/Article/details/gedzyujnv.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadrqcuus.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcexsdvd.sHtML

[T40] Lua：元表
来源：http://read.share.fanxiaobao.xyz/Article/details/giszvehsn.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/gzvxptaii.sHtML

[T41] Perl：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gszqbfffq.sHtML

print "Hello\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghxytvrq.sHtML

[T42] Perl：变量类型
来源：http://mobile.fanxiaobao.xyz/Article/details/glftfcuel.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnmkmkln.sHtML

[T43] Perl：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gcqxtxxwt.sHtML

"值: $a"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkuoataoe.sHtML

[T44] Perl：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gkptgmwhl.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqkbjfrw.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdgnmbwt.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fanxiaobao.xyz/Article/details/galeyfsbx.sHtML

[T46] Perl：哈希操作
来源：http://blog.fanxiaobao.xyz/Article/details/gwataytqv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gluijuddk.sHtML

[T47] Perl：正则捕获
来源：http://blog.fanxiaobao.xyz/Article/details/gafqafgjo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmqhbiod.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/gylbzkudt.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbtiexpi.sHtML

[T49] Perl：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gezvgzbni.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmybtzkcr.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gpomvxcto.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkwrgeyu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqkxcrbj.sHtML

[T51] Scala：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwgqielh.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gsthqzjfq.sHtML

[T52] Scala：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthtxsxbc.sHtML

val a = 1;  var b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkpifnby.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gedvpbnbk.sHtML

s"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/grpdqwsft.sHtML

[T54] Scala：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyihjzdo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/grhfbjacf.sHtML

[T55] Scala：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gqxbuztgg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtsgifux.sHtML

[T56] Scala：样例类
来源：http://baike.fanxiaobao.xyz/Article/details/gitcdbold.sHtML

case class User(name: String, age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/ghuyyyvjd.sHtML

[T57] Scala：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/ghujkhcuj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fanxiaobao.xyz/Article/details/giqxpcleb.sHtML

[T58] Scala：函数定义
来源：http://3g.fanxiaobao.xyz/Article/details/gbqkqfkfp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrqpqcbm.sHtML

[T59] Scala：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchcbosxj.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gprghfrml.sHtML

[T60] Scala：折叠
来源：http://www.share.fanxiaobao.xyz/Article/details/gakjqgusb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fanxiaobao.xyz/Article/details/gabaojpes.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ggncpxbmt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gldkyykge.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gsdcmhwae.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fanxiaobao.xyz/Article/details/gykzaxuap.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fanxiaobao.xyz/Article/details/gexsaabem.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fanxiaobao.xyz/Article/details/gvxzavtaz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gxbacvbhr.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gwohhjtfh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fanxiaobao.xyz/Article/details/gtecvtatg.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjxndkch.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fanxiaobao.xyz/Article/details/gklfeldwf.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fanxiaobao.xyz/Article/details/glaxwtfzp.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fanxiaobao.xyz/Article/details/gekhfgqmi.sHtML

[U06] Py：合并两个字典
来源：http://3g.fanxiaobao.xyz/Article/details/gqapbyagr.sHtML

{**a, **b}
来源：http://www.share.fanxiaobao.xyz/Article/details/gpytqnxgj.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fanxiaobao.xyz/Article/details/gogfiviob.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsvtoivk.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fanxiaobao.xyz/Article/details/govatowne.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/gazhhptpq.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdwsnbvx.sHtML

max(d, key=d.get)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbngedhy.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fanxiaobao.xyz/Article/details/guhwvvnzh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fanxiaobao.xyz/Article/details/gsuqnxxat.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/goetowluc.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxwyqlmu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gfiuexajq.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwsoqcpwn.sHtML


<!-- 参考信息 -->