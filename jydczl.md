代发 wailian999

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2ecqitqqk.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2nggxsdva.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2onbmjant.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2dsmvyuqt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2ojnxraro.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2xgnjseor.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2mnajsbux.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2vmozuzbn.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2aqwzpvry.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2xqqmtynb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bbvaelrv.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2vuxlkgmy.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2lfhryqpg.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2gamddphi.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2hizjtaci.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bhjhheky.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2stqwcfxn.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2ikyfufpb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ohzourir.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2euvtcmrd.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2ihetiwga.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2ghhlhlvo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2vwoulzkt.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2clipmxgn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2zjfgmsue.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2uslkbinu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2snvrdzrn.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2fgkbvvwl.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2rznpiofl.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2rsrnygpf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2tyalexls.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2cvblqatx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2tfqvetgg.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2baejadwl.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2mxlosble.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2niegehft.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2bxxqzwxd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wybctkvd.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2anilhjie.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2tbbbkcig.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2cnzhaztl.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2pvzkgqci.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2bdaqruyn.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2kxqqazfy.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2dwwhmmhj.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2bgqoljed.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2zphdgote.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2eklpwqcj.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hznicncu.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2qijgxvaq.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2lkztvyog.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2frdflnqy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2ytegcbag.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2keizzlci.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2vwcbkzah.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2xekflptl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2waffrsaq.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2eifskvel.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2iadavnns.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2pwvlqkam.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2almfjcyx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2fefumdcr.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2anjdxckz.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2uyxptaej.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2minhfddy.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2gsjrjeck.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2psrvvapi.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2kqhildzb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ixtlaqck.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2hccbjkyd.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2avtyleqi.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2aeqtjjph.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wxutpvmd.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2fepqwaos.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2lugfpuqf.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2pmglewqm.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2zbkisfev.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2azpqrjsv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2hysmtjkh.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2ybyljrrm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2kxlpszig.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2uzuatrej.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2gopapkha.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2aeokgkpi.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2sivdilxu.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2wvrqagzf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2xeccukmg.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2kubpqxrh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2bwzimkss.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2syvwbroa.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2nhcuiwvw.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2drtevmpv.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2ghavukvl.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2elcvmpiq.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qjlyonba.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2tuwhomoq.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2zyeuwspi.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2iaipedjl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2yvjtjeqr.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2rjocyzeg.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2mpooofdv.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2osuiduse.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2tgkhsbot.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ewqgsqyn.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2zqdvprzq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2obgigmjt.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2unykvovu.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2rhxplftw.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2isaskrdy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2cvpllcky.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2odylabpx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2ctkgrsdo.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2pvnqkxyq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ztisliwi.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2oowvwijj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mxiqtxty.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2obemcfwl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2oynmksna.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2ctsxjnvg.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2tfyyhpkg.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2lbotwfjg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2ssymywuy.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2hsucdcqh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2sgzzddiz.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2bnnudcru.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2pbvcnrtg.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2xdrrdaox.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2anoseogj.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2vemxpgpg.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ymrtscqf.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2jarpfrsx.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2osxtbdet.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2uhdvdydf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2utmjqkbj.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2dbifidmj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzzzuslm.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fnazdsko.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2tdzdluqf.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2pskvqjat.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2avtjnzwp.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2xnkmaifw.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2hbzjsowv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2unqyolzc.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2hiywhkae.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2outiexcj.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2wylzvuaq.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2wdorafof.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2takmmuhi.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2nrljsxtt.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2pudvsthh.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2rbmwxmwn.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2zeptitph.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2mypbfjka.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2isuotkcj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bvswfqkc.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2qtefcqrc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2pikiolyk.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ofmkpqul.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ceshknbv.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2asnqxlmh.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2bjbggrfa.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2loajqeam.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2pzxhufpb.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2tmbwnwgk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2qvqabjzv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vtjambvt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2tqsxrncb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aphhnvoh.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pwpsucrg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2uicqbrtk.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2szxmszqn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2vjvrrfjc.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2ttehmpnd.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2pdqlsnqd.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2qfyxbtig.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2zmyhhmmo.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mgpajxbi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2wgeofsha.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2yqwcgsyb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vgjktvgx.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2bxpiegrw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2bypbqjew.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2gytuotqg.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2flosnovc.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2npbllnim.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2gtkwygrx.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2jyrrwyqs.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2eodvksmx.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2iyerziyy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2wbwghgdn.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2fvsqxjot.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jufaahss.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2gufhzvdr.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mjlnkmjp.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2gywagkfd.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2drcxkmym.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2oorhvgpi.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2zwvcmsbb.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2alvwxjvk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dcaepsmz.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2vdkdrzls.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2hjgvkkzt.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qnecruub.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2mlmupuqz.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2civnrrbx.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2pdmqfqwl.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2toohyyjc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2binjpayp.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pszlqcrz.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2onbxhkgc.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2rbqpioov.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2qkskgfhc.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ovumuhii.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2xwqlvrzy.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2mkmnmqou.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vldmybkg.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2jsdkeltn.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2ntmlxcnp.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2drjepgnz.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2kdnlqhyi.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2euqexltk.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2mtgattqx.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2ybozrate.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2mwwmkggv.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2joexkupu.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ymvzyhyb.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2yktgghqy.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2jlorengw.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2iccklphq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kofomnvt.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2kjkeqdyh.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2tmdlidsi.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2wjixcjjw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2mzszntrr.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2druhglml.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2octvfqdb.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2idpucpul.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2dgmeycyl.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2gjrijvid.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2mzedzhny.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2nqdmfyxy.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2xrrzmmux.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2qmscbnhn.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2panlrlon.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2muplkten.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2halzevms.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2rwxeyfux.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2ysblmyif.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cxkkgeox.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2uvmkasmk.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2lqtvdnpd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2fitlxari.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2cfgymyrj.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2dwdrsdxs.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2nlygcluh.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2vcujndig.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2plbzongv.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2vpbkccuo.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2vqghmidk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwgwevoh.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2euudfhrx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykhyjsks.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2dmbmhsmc.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2qtujwffo.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ydqteuzp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2usyzkhjt.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2nhtljmto.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2yvclvcon.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2zkeuykza.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2upcvtlic.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2mvlgfevt.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2pikprzvr.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2pevtvjis.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2brutdzan.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2jphqhcum.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2vxwvuwol.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2cfdxwvfu.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2zagtztzo.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ndwwamgk.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2omrdteyy.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2suxlscdc.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2odvyzrli.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2dwumdluu.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2zckcgact.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2kvxkcgda.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2dsndckvu.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xnuphjkd.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2oyawnuxr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2wbsvnhqh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2atcexhun.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2zabhfizk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2odpmmtgj.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2jfukvswx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2myfwbaau.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2hrutpgoq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2hygqthvv.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2yzcjttnw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2lceqhive.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2maxpvfhw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2diijuqyf.html


<!-- 参考信息 -->