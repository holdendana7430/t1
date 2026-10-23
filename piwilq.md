代发 wailian999

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3cgvmwtba.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3klcttopx.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3ozuqszzz.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3rdmygqrg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3hearkftw.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3pojvzhgl.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3sghedmro.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3qhogdqdw.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3bwfgvujd.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3ticoxwee.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bmfnnvts.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3qccbayfk.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3kftzwprp.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3zcvmayex.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3ggcbbdyb.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lyvhdrwq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3nnjyrtmp.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3ieljivoc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3pumoatdm.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3ffhxtkhs.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3uhjutree.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3ikmfiagm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3xuveggjf.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3tizxsyaq.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3sqmjeyrh.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3ymcxtyit.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3vzdxvvxw.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3ibglzvda.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3mmrfrkus.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3hvettkvq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3afvyeluc.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3pdgbdqdm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3orjnobch.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3vjhpkcmu.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3xezrczlg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fdfuroja.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3olgzecto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3thmeocbo.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3knnlawkk.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3jtjurqrt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3uiolavlu.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3vqtyyrjo.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3uquylejw.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3vgnkecjy.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3mmlggtil.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3anvzxdnj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3hqtzpvax.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3vzjzohbs.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ctjhetvs.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3hjkgfgia.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3mukhxndq.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3ckntruse.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ltglynjw.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3lweqwizm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3qdjkivhn.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3xfrozvmx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3srnfnpue.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3flcsptxm.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3muqplniz.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ncugkshq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3ettzvrwp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3mwowhrrp.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3wbslpuul.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3dohcecgs.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3vlrapntf.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3ipxzstfe.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3yxxeitsy.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3tanqxonp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3fdnnlyyz.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3iglczcom.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3rblevhcp.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3rmvxwbej.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ilpdqrxf.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hyrvbccq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3zdlvbwrt.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3rqmckcel.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3jpmvyfny.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3xsihxlsa.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3cbwbdrrc.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3mnapusgq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3mrvjrwtk.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3iyoiyiib.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3oodxdxhd.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3bdekstxu.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3ejrpsfig.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ndockcpc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3hfnqgyhw.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3susbvpfl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3nwjqzare.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3nvcrdgcq.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3dbcchozv.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3wxbdlmcb.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3contsgzg.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3mcolhtti.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bvqeoblc.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3qphbfspk.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3sdqiytec.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3tfwgzvaf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3bwnkgnsd.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3fngaagky.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ogriwzqt.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3okcuiecb.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3skkixysh.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fproawyi.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3uhwzfeil.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cekftova.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3lvhlmjlh.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3taxablse.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3ndvtongq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3qsgzkahg.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3yqddearc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3hcynhxno.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3egqaxioo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dzqjvgqa.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3hebbbhvo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ibdaduup.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3pjtwxvhw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3wivqfhvu.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3jzvkrkre.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ifvappqq.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3nocbvavw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3wletmklx.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3chqfphlt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3kzdzzlfn.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3citmzjqc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3rdbhnrnf.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3awwvslxe.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3okfvnigh.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3xrrghnik.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3udbjthab.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3wkhglnyg.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3spolcbjd.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3mgcxurqr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3cyhtjjmb.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3egfglgge.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ysofvotl.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rwitvzun.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3kbbipmsm.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wtgtkvpk.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3loarjxhf.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3cqlblbsd.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3irfscaoh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3nokyhlor.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3vmobcvwo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gbeddzdn.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3fgoqwcxh.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3lnclprni.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3bzotcsof.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3doirpfom.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3pxqmcxfg.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3xsuizirj.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3ujmyuqrj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3pqrfpurj.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3pqvxynyy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3spxmbpvg.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3kncetltc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3rrvldhzv.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3fyfqccbl.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3flxfehsi.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3pqletwci.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3kzcgcxuq.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3eiufiksg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3dpofcuxw.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3zbfzvyna.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3rkruoqtn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fhfnrlmf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3gqciqubb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wppfmbis.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sjjzgbpj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wwdhfdkq.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3ducnmetl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3tgvldmpq.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3ezcpyykr.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3zicomtcs.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3dbkprgjz.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3jxqmrsmi.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3wzfnfvzw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3oezwdubk.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3nimybeyk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nsmdskne.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3kgdusrda.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3hpaocxhg.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3txqmwvbx.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3cnwdjhct.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3wqlvifqj.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3ohlwvxks.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3mqixcabh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3jlwjpqeq.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3qoqtlrwo.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3brhrjpzu.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3nddlcupu.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zcxpzaox.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3aawmappc.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lgtdgekc.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ixxgwtjj.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3eebyqzrs.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3dqgefxzb.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3csbmlkgf.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zborbwfm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3bkmxhmrd.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3hnhnxvdr.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3bjxtmiih.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qjdbnvfp.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3okdizkne.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3wqxrnnrs.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3roidnxtw.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3qqinfmnf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3rmyveiuu.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mhsryjyb.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3yprezkkb.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3kpycffyl.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vxqpfbgk.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3tlzdglgc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3qycponpf.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3byfwypkb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3otbqmbsm.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3gwilyjkx.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3evymgcja.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3cmcrbwqq.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3lwvzabuo.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3qceaqzzs.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3uryawxdh.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rwtahojz.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3pngswgmn.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3lgrfqspw.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3xcrjqzmp.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3drhbgatk.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3kpigdugx.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3peycrqrs.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cjutorpl.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3asrutujp.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3wtjgfoue.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3obkxvgpq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3nsqolukj.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3rvceimkr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3wundqdnz.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3auxkascx.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ukwkqvwz.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3rziubmwy.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3qxonrsaz.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3fbeazhor.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3euqtcyan.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3xnzkjtqv.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3cplsivhx.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3aglccjxl.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3noudvxmv.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3feiwpnxu.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3neceypsj.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cdpuvlik.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3juzefmuv.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3eovejamy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3latflfmd.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zwzxfptd.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3cungxhkx.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3lprqwwpo.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3matuohnn.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3wgfylkkr.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3wuargagj.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3yyflfgru.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3rnvnjmir.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3haaupxls.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ocehhubw.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3xblhbhhy.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3gzzndiwd.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3gmhubtqh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uhpfpccu.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3tnzthxrc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3cawuzokw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3zebgacww.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fxywaecf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3nqgtqffk.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3pxquerfc.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3kemgehja.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vcbjnzmp.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3zyspmmdo.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3acuwvskd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ljckaska.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hkzuldqp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tispwpxm.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3lobkenie.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3jmstquwa.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3podlroie.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3brkjdych.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3kdbhxbiz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3zfptpldo.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3ahsrfmpu.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3llkmjqwa.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3bimauvzg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3spvjznmj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uriomgsg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3hsphaxsi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xdddblal.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3kwtgadlr.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3bvzypger.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3ylgxabpg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3zdnaukac.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3buuliwql.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3fwfrwrkg.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3mivhnozq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3lfeelryz.html


<!-- 参考信息 -->