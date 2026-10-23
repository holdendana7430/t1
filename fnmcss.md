代发 wailian999

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3wxhajkxd.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3jugeqsrk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3udqabrbu.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3emvrotuq.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ppkaernc.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3ntqvovpj.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3hiktaest.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3uqternuq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3yhsynxzg.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3tqzcfjam.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3vzzcufll.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3gwdaoivw.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3isnmfqqs.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3koefadaa.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rogryhwd.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3pdzyeukz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3nyqwgbnv.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3xdrpjvew.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3wkdwhtrp.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3ocsfpyfi.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3erqftxmq.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3mjfkdbyu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3zhhbxeqk.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3htusyvep.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3nicfzxhu.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3uidkgndk.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3hdpjyfkc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xbuchszc.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3shndyopk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jhaojcmt.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hspfzbkc.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3otltqctt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3pybjjdog.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3vbdcpqpv.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3ybjvpyit.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3nulrpdck.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3ucksqwuo.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3ycgycdtj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3nrihpkkv.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3xawxfmls.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mzcrflch.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3aowktayj.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3lwujyzam.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3yfyfiznj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3hyehjleu.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3ruhmuanu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3dlkmigqa.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3wwsruoqf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3jsfkhbwp.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3nrjcjxwx.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3wtuukrhj.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xuiomvfw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3xebzkgwo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3khtbyhkl.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3sbttjwxm.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3uqzvjdvt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3kbrzqwqd.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3cagajacw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3niuycbam.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3icbelubu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3pbiyrboi.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3qxptrdwe.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3uhqsgxwp.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3cluiqxem.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3jzvuoglb.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3heqrosht.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3afmmwrqf.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3grtsjlai.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3gyjllhzi.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3icmcwinu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3xxlnqgpo.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3kpfyfyin.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3dqfubjux.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3dxmoyrrn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3ohhenkuo.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3bctctzam.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3vplgmpte.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3fxaolijg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3lxgfdwcf.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3skmbvsrm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3hsavcajq.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3cvkhkrsj.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3jcaqqgkg.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3hicgatqf.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3uogygemk.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3thkgkhlc.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ejddgubh.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3xcesikwf.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3nolhytrk.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3waqsqxri.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3vcugpygl.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3mllincfs.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ohbatnvc.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3liupmmid.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3mabfjsxo.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3azsxuxrl.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3dcfbghbx.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqpmrxsq.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fgnvyvuh.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3jyowutqp.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3xwsrmhie.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3cbayocak.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3zzicxyev.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvnsdokw.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3txennbio.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3efximewr.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ndyssfdg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ruglpatq.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3xiemoran.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3qpcqgxdq.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3njvfywfv.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3bcftocnn.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3bqawqmgk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3pdmtikmp.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3kqbydmha.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3vpfgyzcy.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3yaeubzgy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3hxxxcrzi.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3dictlmvs.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3hjagzafi.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3jjldskur.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3rsdylbmx.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3jrhkznkn.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzpmlfju.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3tbizhzfa.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3mvenpfwc.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3jcwjeyiz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3gtqfylme.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ophcscgx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3vowlclla.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3lueebzha.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3kwsehqqp.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3fvgtraav.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3cfpqahej.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3rfwyvcuk.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3pwvtjank.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fqoqtxlt.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3elsmxubm.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3zviqlmrh.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3aerglyqj.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3pelaxyxv.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3zhqwwzis.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3zhwmmrxq.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3chjmbhuo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ldeagwrj.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3xpxncojh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3mdaeysnc.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3nlfjxlyk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3frpieboj.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3zyqxujym.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3fwtstrnk.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3kjvgylob.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3dkjbveeo.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3vuzqyxiu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3csnmgtib.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3suabydrx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3lgdocxpn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dojxnmnr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3xqaoyynu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wgxuinxz.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yutlvsfv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3lbjdpqvs.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3iqzriqyn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3xipvufrb.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3dnhftwei.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3cvxqccff.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3weducnqg.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3jwkocspz.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3hkcdwiue.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3yvafulxl.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3jwhtpefy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vlrkxhhq.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ingkvzuo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3xnefwgry.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3hbcagfbe.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ifyknbjs.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3xgfjcdua.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3azmwjzpd.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3kxcdhrfr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3sqxwkkow.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3vgrscxdz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3hpuqynus.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3ehigexkz.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3feqdwgxu.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3dhumohhp.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3aziigixc.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3dsschimy.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3vnoswbyd.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3cwjehsls.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3edjbkixx.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3eymvkvnn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qmpkcdzf.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3fbubvbtr.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mpmteyyt.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xalnyrov.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3fceslnoh.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3daqyrmwe.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3jbzflvxb.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3buapjscd.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3rmgyamva.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3fsvwuzje.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3zxdluioc.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3zsxthbci.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3dczsfkrf.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3gzkrbvkj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3zximumac.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3evxqqhse.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ilchrrkp.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3mvjzjoju.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3tvyvmber.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3qtpslnju.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3gchpfxrx.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3cjfrgfhg.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3xwgcouwz.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3iwwhwank.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3brerdyma.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3qtilvbea.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3taemqmmu.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3pkqjutqr.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3mgzmzxsu.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hhqydjzu.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3evkvkdey.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3pclbqcxf.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ybczlyxm.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3mvyslnpu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3fizchqej.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3jawhviyv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3ietaedfo.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3pwmooylp.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3brwghqxx.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3dqpcmaqv.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3zdhyjxmt.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3edjgqioq.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3srgfxkcy.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3seuxhxng.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ftwfsahq.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cwgppctc.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3hroeumwq.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3tvapfngi.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3wiyhiycj.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3njweimux.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3jptimwle.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3guybxclx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3xyflpydu.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3payqowfc.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3vavxuctk.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3iobrolnn.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3muoqdzfm.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zucgikhi.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3uopvrrwj.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3vbuqrfym.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3yzipnxcu.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3hlkmonch.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ecnnzzta.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3wkfvlujv.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3qvozkwlr.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3goyqcyln.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rvflccxk.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3beaadpjh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3ldqmtych.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3jyfxsahb.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kczbenjr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jkldnbrm.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3jgptvwio.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3auvcxjxl.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3flcrnpfe.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ybnpkwjq.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3gvukvdjk.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3mgltvszc.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3vhdcwkfe.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3olseyjry.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3rixnymks.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3qsgchwyp.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3tmhtmmow.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3mwmsathc.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3elljznuf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3uhlhlzif.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3cngalrqs.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3dpwrmygi.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3qmmpahds.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3rvrgkjzs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wyxqwdhk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3czszescd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gookwjau.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3jdavcezg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3vrpblbof.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3ictgzsvq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ftcygkop.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3jxpwchsr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3orximvzw.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3jylblgfm.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3gvwcbosu.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3pdfntkzw.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3cetrojhx.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3vewxxkwe.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3rrhxhcfo.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3wddgxtjd.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3hbbullws.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3vynozyro.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3exqnmlsc.html


<!-- 参考信息 -->