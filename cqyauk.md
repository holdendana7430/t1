代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3sfjbvyew.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3zegfssox.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3zgkthino.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3qfodquwn.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3gayalbaq.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3takibugw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3ryvuecpp.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3bilxtgyb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3llouitue.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3lzdxqabu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3usetfqod.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3ofupqvvl.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3yamoaxtx.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3ldpwjopr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3lsvuwuim.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3rzvgwhzs.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3flydnchj.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3amsmuzuy.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3vjfgueef.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qlaqcsqj.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3fizvioln.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vuizscql.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nuxbcgnh.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3vtthfnqu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3buzwxzqz.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3nwqauarq.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3nnkjgucu.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3kdjfspsx.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3wibjuzww.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3vjmfsxet.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ucrqfjez.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ddbyneoi.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bkqmzyui.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3fnshigbc.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ckvxywnj.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3gtzbdati.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3tjistial.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3tdjfkdiv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3uzizqgux.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3aexmcuya.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3gxukkhxp.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3whzthasu.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3jflprwbd.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jwsribyn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3xrosmuhv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3xendsmao.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3fimaxxyh.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3knoakntj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3dugbfvwq.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3cmfqoxnh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3gciuajth.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3fhlmlxiq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3dxtplnhm.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3dhjokyir.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3smjxxeod.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3jhzjarhl.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cnaslbod.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3rfpewpxn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3fwmwmewo.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3vbczejjc.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3qrzabtvm.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3lzwtmwga.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3jjsazppt.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3fgtddprs.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3szfumyxy.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3bcsgdprl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3mukdjenn.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3lvpifyyp.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3bbvbhkdg.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ryiwqyps.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3htycjqtm.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3hfhnsejd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3nntqtgys.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3rawbmtqn.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3lyrmaqgg.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3pcgdcfag.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3pkdjxftw.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3vshxpnyt.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rgganbiw.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3tzwteqqt.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3tfxbbflh.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3hggpgrzp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3dcfkcynm.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3xcujgrpq.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3nnmyjkcu.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ckbexoly.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3nksbcqbb.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qugazvln.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3iyehrwiz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3uepyvdzd.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3rthknxiy.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3kbculppf.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3tyiytisk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vvvacrxu.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3cnpbdscu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3zsybyjgb.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3jytdamvc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ledomiku.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3gxxatpch.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qeukxsxk.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3ujcfsayh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dkmndhfv.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3pvbmayoj.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ysnlhezj.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3lsezdsso.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3rtkennlj.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3trcaskno.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3pkdouqdd.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3jagdcyjz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3tvaxpvpw.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3mwxqwewl.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3elwslwcc.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3ywgcnzrp.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3fedqaicd.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3rspmhpwf.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbkgmvia.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3azudizqo.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3wnxhhtes.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ugzoxqhq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3pgevlrmt.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ubilafpr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3abilswuh.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3cwgpxsxv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3gqktzpwb.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ahupgkjp.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3emgekzeq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3bhdoxvmh.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3piapmswj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hocjsple.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3dzklokzs.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3wymhfydr.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3belruyiz.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3sluezbhf.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3lcbojrmt.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3ckbfuamp.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3eecovjbk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3uvrsvjuw.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3uuczofvl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pqajator.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3kgutihno.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3qcdxwmvi.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3hsoryarl.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3oizlokab.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3nrhzcwfu.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3oysxepfg.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3qwxppclx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3droptfmw.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3pfcsqnol.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3fjnzgmjz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3edqybyhr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3mftwldwv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kcmateji.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cuhvjrex.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ueaursif.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3nvxaalgb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3hzzpbekz.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3jzhsktbk.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3swjvhoqs.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3jcrkkghs.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3fnnabnqq.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3redaafvc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3vwxfsoxy.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ombdlaqe.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3alowqvda.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3awlqnyzs.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3pqpgwqna.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3xajvnbww.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3pgkppykc.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3mijgqemx.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3sydvmhbe.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3jwoqqfmv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3dqpkpmhw.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3ttpbaiuz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ejlzktwj.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3eimciybd.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qdnwaqmu.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3miycqljy.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qhsfbypr.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3udebcbqf.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3dztyyzwb.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3zdzrjvdq.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3mupkzzhe.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fvkjvzur.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3cnzdqhuc.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3erfvaahd.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3wewfbepw.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3syudwjiu.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3pzvbpuxe.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3fdqcyyjc.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3vrsrevet.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3tbbwflsf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ufwvqevp.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rpkhcvhz.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3yidujmei.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3xivdguqj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3yummddcp.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3lyirbnwh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3jgnjudqz.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3omrotfld.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3rqglemlw.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3flepjnyx.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3bwrtclon.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3fhnlrkps.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3dcotvtcr.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3jexpzafh.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3adarmwpb.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3rjrjhbhh.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3yuydoqbn.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3fkhfkekf.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3kdnfxflg.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3efaudvsc.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3wbhksuug.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lqgjuygj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3pitqovpc.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3gynhfwes.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3pcljdnrq.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3kudvcalm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3lfixpkwe.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3vgrlbsag.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3pfuwcfam.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3tddsjphg.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qzmvjgno.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3zekyinnt.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3idapthuh.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3oqtlfhej.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3atzxyuwz.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3eihsmban.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3xoawlakl.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3imhkvbsg.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3qmarvxuy.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3mrferzsv.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3ukrnnqqy.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yxkbpmrb.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3quzazcje.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3jcywyzuy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3vhfsvkkj.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3oxrufeyk.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3lgugeapu.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3jjtkzbds.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3tdwgjrde.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bycsbjat.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3iuojddha.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3xtaklfek.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vhqutkjn.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3xiomeghh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3pmtckzob.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3icwtxqjo.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3zqoegqlj.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3elhrwjdy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3deckigvx.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fjlirsmj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3umgqfjbg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3kozqfkah.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jdfaahhl.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zhflhedz.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3qcczovnh.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3txkbwxal.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3uxtvnrtr.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3cxeewfvi.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3fdiiksxi.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sbdnyjmv.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3bsfwwuwe.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3tmvnyjtp.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3irhqtwlm.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3kdhzrinc.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3iuorggga.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3biljhojv.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3usqmopnb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3doudyrfr.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3qjenutcl.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ijamomnb.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3pbergkgz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3kpvdlwxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lgxacaly.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mpjdxiwb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cntrpnte.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3xgtkgkgd.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3jiedoqbr.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3lvdvtntp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3alblrboa.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3aytigurx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3unvrozvd.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3clciciiz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3scuqaemr.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3ckfreubw.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mkioahwi.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3xkqmaflo.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3eqiuvxzl.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3mlfltvqg.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3nbgriktq.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3qridughu.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3mzpmshlg.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3gaxkofrj.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3qeqcigdn.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3gjdbozav.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3jfwcunwg.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3aoqrnaru.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3wyjltpuq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3nkgoyixb.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3vzhkffdp.html


<!-- 参考信息 -->