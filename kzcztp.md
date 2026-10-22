代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2aezvxgju.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2euoqwoen.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2opvudmlq.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2hyywarqf.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2iodjtlxc.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2oupuegpt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2whmfmdcx.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2uitiktep.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2dzhjdfmi.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2byuxgbhl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2bghmkcvr.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ixiuekqn.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2syaylepl.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2repkdifl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2yqrplexy.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2lhajdgqe.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2pyslkmeo.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2pghedncz.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2oeddnwnn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yoouttyv.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2unttqlty.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hlkuoceu.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ahfagzoo.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2tylphjhl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2tpbjiqgh.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ejznvcpd.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2hhyckqlm.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2djsvijrt.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2puubnkbd.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2jcnvqgbi.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2bzlezuhz.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ubjwloyf.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2revohovc.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2tczzmcob.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2qgezbsnn.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2zbdvxmhu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2mifmtjhv.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2uyjtoxcb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2kzutgray.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2spyjbkgt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2vdveicse.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2bowhxhhm.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2exwxuira.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lldwtsut.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2hpeskziv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vennxjtg.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2elnofdvo.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2feobrevk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2iyjzqnpn.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2hubmqpmj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2nrcrdhjv.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2hcoqgaqt.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2ajrgffvh.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2nplhepxu.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2bzzatpxl.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2itkboaas.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2vmtulzub.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2usmwofmj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2atsehzip.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2xxineibo.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2oncyqlee.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2smfmmpuj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2elizrowh.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2mttlvomr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2tgntftwo.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2mwmfqwlh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ptwtebqd.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2wuqwcnup.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2fcccgaxp.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2osqiskaq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2eynutqfy.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2aeghdvcw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2gtuekcac.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2kedlexel.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2vsdaeymr.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2bfjrolbf.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2wspwvgdu.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2pueubkem.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nyezazrq.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2icfzqoqr.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2cexqzlvw.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2kaknfkml.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2vugrxtvr.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2rwlndvbt.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2ojuipuvx.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2oreoghkk.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2gbhittse.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rwrpycad.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2uxygntzl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2oocpjvfc.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2vsdqotjl.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2npwyxeuk.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2vruwfvox.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2odbwkevt.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2zdfiibvu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2jurpwwqz.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2vpiikbjx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2oyqikofv.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2tednerbt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ngmoprjw.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2bvymteyk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2janbtgyv.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2sbkymiar.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2behiuwym.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2huqibact.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2pasiwosp.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2ouynoswz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2agasbxnx.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2lffnvpcj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2gmwmvzjc.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2dvvtwgin.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2jehtzeyu.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2lzbmjzdp.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2iefsakln.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2fizzconx.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2aizwpoql.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2hkciutcs.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ytdulobi.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2ztwlllxf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tezugfgn.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2kstczmzf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2glbyobgr.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rpkhhisf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2puvgliun.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2buivooku.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2vczzuwcf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2mqmbldlu.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2duxbutdb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ullkdnnm.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2wvzpxyvg.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2uzsnylpn.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2vxrvlziu.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2wlqihofd.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2tdyimpog.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2akqfbtdn.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2znvjjmke.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xbqtwftj.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2crpexybw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2chcybvbj.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2rtuhioqd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2goohfnia.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2eghgtbtq.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2lksuruxz.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2qjrguzrl.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2djaskksc.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2ggdttwxb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2vjfmyzsz.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2keqtjqfv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2fmjlmtnw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2taatoowy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2zqlvjmzl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2flwqgtvv.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2huunfuti.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ntptdcub.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2yvtijsgw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ktzotvvd.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2mpmxstud.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2twxxoifs.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2begiwgaw.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2pqetjehg.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2llxdmffs.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2wjnzwsre.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2sdnhkwvy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bfstfisa.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zmvdymjp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2uiyatblg.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2heyyxaff.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2yiilbyvz.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2ivhveyiy.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2pczvbkgv.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2xfjzgktq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2mxlhgpvl.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2qiswiedz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2kivuymrd.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2mwtveqzw.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vznagujr.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2sxeixurz.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wtdptxka.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2mmzsmhxi.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2bboahmuk.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2iklaxdny.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2jshayzee.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dorqkstz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2fopoaoiw.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2cqmebyvr.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2okbdgfsf.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2whrurzgt.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2gthawmws.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2sfjuixmo.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2zxattyde.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2ajkpzssb.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2utbhvuei.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2hblugryo.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2phxpdpmt.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2ifoheqhz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2slklcenp.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2hcgctnru.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2gqedouby.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2hnbrrnfs.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2torybrsm.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2hcjmuapz.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2ruaewans.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2wzhotjdy.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2vgoziybg.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ouugqiqj.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2qywfxvjp.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2tnaynvqv.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2thkfoqjw.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ijnxkidl.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2mwzojqgf.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2psoemgui.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2igcajwai.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lcoymrjc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2brmwqjmo.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2qjuswojv.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2vltwgwuy.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2vkkciuuu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2cwrhgnsl.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2odyoogwh.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2diarhaat.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2sichpere.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ogzxzuzs.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2yspxvhez.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2nhyndxez.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2qbkahqiu.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2pdzzumig.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2tvqwgydy.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2jfjeuzbb.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2etkamkcl.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2whqesqmc.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2dtraicfa.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2epmozhwq.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2erpqrcxl.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2cnqqbsun.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2szaxvufo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ymydtcpu.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2byzbwbje.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2ginqpoyq.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2nfjjzpqd.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2yybcbxui.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hrkphuqp.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2gkjfmnwg.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2nwwcwwym.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jijdenuf.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2jwlbhwqo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsxvdcvn.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2uqslcfux.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2wjaksdps.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qxaucszr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2veugwmor.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dpmmbgdv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2wzmbtfak.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2izzzekaq.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wkfollmt.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2pclemnpt.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ycgktnnc.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2cbpxffhy.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2nukmoexw.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2slfdtaxq.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2bilqdpef.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2cpwshpzf.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2xejuqykw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2hrvcxlui.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2bhprynbp.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2wahsyqyy.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vajeeyvt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2tgvmmvgh.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2rxmqmnmz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2fmjypvmo.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2kcfgcdaa.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ydikptfj.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2cubiljcx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2biqxaxuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mqhzrblg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2tyvguohb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2banotqql.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2jqkvybga.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2cuvfijvg.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2jijqwjhg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2mxujparv.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2bmxtqzal.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2tblvsvej.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2wlsdypdt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2wkoiyotl.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2sppcgkdp.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2xrzndshy.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2bilukcyn.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2gpzdzame.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2kccdryiq.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2ipswlrww.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2gymmlzdn.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2skjktuea.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2ptarjxpz.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2uwozeant.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2rvldwytx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2buycbici.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2kfeomoqd.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2gtdalfer.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2tbexfesa.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2flyanuoj.html


<!-- 参考信息 -->