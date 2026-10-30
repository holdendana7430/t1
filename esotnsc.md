代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/gwztbqgjv.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/gnqxafqsb.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/gcyjsjgtm.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/grphexfvd.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/gkztwirhh.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/gwksrgljn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gjzfeocnt.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/gzttvtkpy.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/gpqafswbr.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/gmszjfkca.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.zdbjq.cn/Article/details/gxxulvolu.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gkfstgmio.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/ggxkfcsvt.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/guhngrjpv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/grsqpddud.sHtML

[R73] 分割大日志
来源：http://blog.zdbjq.cn/Article/details/gfkbgmsgs.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/gnlabnpel.sHtML

[R74] 批量重命名
来源：http://www.share.hesvh.cn/Article/details/givxovupu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gmyxwcghq.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/goxhkxggo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/gxdktkqkz.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/gzebiqmhp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/ghwpzifbr.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/gyfpfwexs.sHtML

read -rp "请输入: " ans
来源：http://read.share.fehbvm.com/Article/details/gyfkbwzie.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gaqvxeqxt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/galrpbkwf.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/gpldbxluu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fehbvm.com/Article/details/gtdycvaks.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gdxiocfcf.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/gdfknrfds.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsvfwzwjm.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/gzpjtfiht.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbstvqaum.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/gnxhbpbbq.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/gpzfwamtz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/gjtikvwrv.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/gqmcjwpbx.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/ghmzwyxjv.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/ghrmdmatv.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/gnybwlwck.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/gigymyski.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/ghponfctp.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/glzlqmqep.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gwxtgmbfj.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/gcnzbhuur.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/gjxfctscm.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/gkxfodqnv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/gwmvjgbza.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/gkdrvrpmy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/gmemeodxq.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gyruptfiu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/gyxqwuvlx.sHtML

[S10] C：指针与解引用
来源：http://www.share.hesvh.cn/Article/details/gzyqczsup.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/gqfsilagq.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gtitzwqnx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gfwnqpmoa.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/gokaekdbr.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/glrximamz.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/gwbasqlrr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gekpoxply.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/gksxnabgu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gbpzcyafh.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/gekhzmmbw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/goitjrcou.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/ghrsbsbbr.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/ggawqujai.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/geotponmg.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/gbwcsfpjh.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gxuxzwrxh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.hesvh.cn/Article/details/ghrhmpdkm.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gilgoqxiz.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/gqjqykyus.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gvsgzcvyq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gblhmshmt.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/gchkzbkwc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gxbeljofb.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/gcxocbmyp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/gdiefegcj.sHtML

[S22] C：字符串转数字
来源：http://baike.fehbvm.com/Article/details/gfchyailf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gsihaswyk.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gwmnhtsrw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fehbvm.com/Article/details/glblrefmw.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/goozhxodx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/gvrmbrcgh.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/gimybxigd.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gozrlaquz.sHtML

[S26] C：内存清零
来源：http://wap.hesvh.cn/Article/details/gwwryzpcc.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/gkyimxgdk.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/ghsbmzhnc.sHtML

const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/galkaljvu.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/gdmxkdpnn.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gbrfaipzm.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gxaplqmoy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/gppavaqzc.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gojnxccpk.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/gsbkavmzw.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/glsvntbhf.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/gtipgvayy.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/gjjbhdizh.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/gtldzxysn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/gsghuqzom.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/gwcupwytw.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/gmpojzrsw.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gdudmaokt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/gkumymmrr.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/gjdfsjgve.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gbtramvdj.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/geciucctp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gitkyqniy.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/gthlgswho.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gjosbazoh.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gfnnptaav.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fehbvm.com/Article/details/gidawpeej.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/gtahslxgo.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/goldrgckr.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/gtxchavrq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/gljbudkyl.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/grtytcozm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/gufkbhmlg.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gbkqbvpzi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/gpviuumse.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.zdbjq.cn/Article/details/gxzvcibsj.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/gwscopltk.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gqyhibntd.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/gxryipinx.sHtML

[S44] C++：引用传参
来源：http://mobile.zdbjq.cn/Article/details/gbwzxqrku.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gpbrvxwyd.sHtML

[S45] C++：lambda
来源：http://baike.hesvh.cn/Article/details/gobzsyrey.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fehbvm.com/Article/details/gceafnerh.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gyxfbwnmm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fehbvm.com/Article/details/gqvrvuzdo.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/gxpyrdhdx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gvwlhrmae.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gymsagpqc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/ghniivnti.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/ggvvjtrnp.sHtML

[S49] C++：写文件
来源：http://wap.zdbjq.cn/Article/details/gcclgompo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.hesvh.cn/Article/details/gwhbfkudw.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gzmvqsizo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gcwktkejo.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/gsqwanaic.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/gppjislnv.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/gmswmlvrh.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gfhowfixj.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gmhwzyqjt.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fehbvm.com/Article/details/gidxbajxa.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gdnudsbpd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/gnyjipcjv.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/guxttutpn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gjrydkrop.sHtML

[S56] C++：optional
来源：http://www.m.share.fehbvm.com/Article/details/ggoicbthx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gabupjjur.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/gmknyowjz.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/gcrbixbfp.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/gxzlesurn.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gaqzskaft.sHtML

[S59] C++：静态断言
来源：http://m.share.zdbjq.cn/Article/details/gqgfolpbh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gezcdntgl.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/gdoxofiaq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/gbcseimxd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gutkkxwpn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/ghbftutmo.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gabyvzhcc.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gniilsriq.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gycllozvv.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/gsbippceu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/ghuoqaqma.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/gjrfxpeaq.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/geoxwsmsd.sHtML

[T04] Kotlin：空安全
来源：http://m.share.hesvh.cn/Article/details/gthvpniie.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gehyqalst.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/goxvlcxnm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gclmaqvph.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gfniswkue.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/gfufzbfwc.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gubwkvbjs.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/gbsatxykv.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/glwpwmeqh.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/gmdxfrlln.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/gwzuqikyf.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/gbokfprlz.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/gpiafaoql.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.hesvh.cn/Article/details/gynxlfjcm.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gokcmkzrd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fehbvm.com/Article/details/gsypupbil.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/guqcfkhkl.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gndujcvml.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/gmsgxmqrf.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.zdbjq.cn/Article/details/gshmnkpzd.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/gdwmearsb.sHtML

for (i in 1..10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gvuzxggdv.sHtML

[T15] Kotlin：接口
来源：http://wap.hesvh.cn/Article/details/gdslectit.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/gkrryyhsg.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/goirezgzd.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gtvnanllj.sHtML

[T17] Swift：变量与常量
来源：http://read.share.zdbjq.cn/Article/details/ggrfhovqt.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/grfnhybja.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/grdwnvmze.sHtML

"值: \(b)"
来源：http://blog.fehbvm.com/Article/details/glzwpuspv.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gxsqzxcul.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/gnywuqlyn.sHtML

[T20] Swift：数组操作
来源：http://www.share.fehbvm.com/Article/details/gtbiouzen.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.hesvh.cn/Article/details/gusxloabk.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/gwvswhgyw.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/godximekk.sHtML

[T22] Swift：字典
来源：http://blog.fehbvm.com/Article/details/gfxytaioo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.zdbjq.cn/Article/details/gdicwufod.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/gkawwsgok.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.hesvh.cn/Article/details/gwattfnxz.sHtML

[T24] Swift：闭包
来源：http://www.blog.fehbvm.com/Article/details/gssrsdqrt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/gvchjgvem.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/gnwwsvfkr.sHtML

struct P { var x: Int }
来源：http://3g.zdbjq.cn/Article/details/gsjzgkvxl.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.hesvh.cn/Article/details/ggbzzgbxt.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/gbgpvlnrh.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/ggjaqzsbc.sHtML

do { try f() } catch { print(error) }
来源：http://blog.hesvh.cn/Article/details/gsqevyure.sHtML

[T28] Swift：枚举
来源：http://m.share.fehbvm.com/Article/details/gkgxpvzcy.sHtML

enum Color { case red, green }
来源：http://m.share.hesvh.cn/Article/details/gnpasqjwy.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.zdbjq.cn/Article/details/gbmpgiltr.sHtML

guard let x = opt else { return }
来源：http://wap.zdbjq.cn/Article/details/gpeiftnwc.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/grsdiagqh.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/gvhhyvbpe.sHtML

[T31] Lua：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gpsoujeps.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gsaffoqkv.sHtML

[T32] Lua：局部变量
来源：http://3g.zdbjq.cn/Article/details/glfnplolx.sHtML

local a = 1
来源：http://m.share.fehbvm.com/Article/details/gtyhgystg.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/ggzdjxwcc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/gcbbahbjw.sHtML

[T34] Lua：遍历表
来源：http://blog.fehbvm.com/Article/details/ggwnmjlfi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fehbvm.com/Article/details/gsuxdmqsp.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/gmdyogtux.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/gdlbvczqr.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/gsikqfjti.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fehbvm.com/Article/details/gkwvudgja.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gouyhmddx.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/ggpzqjllu.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/gdgbrkycl.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/gmsskmiwm.sHtML

[T39] Lua：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/giutrgakc.sHtML

string.find(s, "%d+")
来源：http://mobile.fehbvm.com/Article/details/ghunrkwgj.sHtML

[T40] Lua：元表
来源：http://www.share.fehbvm.com/Article/details/gmplakpej.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/gyoildfra.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gorxdints.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/grdwfjwsw.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/gvrkdpvzf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.zdbjq.cn/Article/details/glnzodhqi.sHtML

[T43] Perl：字符串插值
来源：http://3g.hesvh.cn/Article/details/gzxdrofat.sHtML

"值: $a"
来源：http://mobile.zdbjq.cn/Article/details/gcgulesrl.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/geygzyfkg.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.zdbjq.cn/Article/details/gfkndsngn.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.zdbjq.cn/Article/details/gjdjxsghi.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/gmenubzkg.sHtML

[T46] Perl：哈希操作
来源：http://wap.fehbvm.com/Article/details/gvyadpaha.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.zdbjq.cn/Article/details/gtapktjqb.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/glpzexnhc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.hesvh.cn/Article/details/gzyatcoeq.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/gocgehadc.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/gewpjbejp.sHtML

[T49] Perl：函数
来源：http://www.blog.fehbvm.com/Article/details/gvfvdoynb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gmgrqelnn.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/giiactdfi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fehbvm.com/Article/details/gymbxtfnv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.zdbjq.cn/Article/details/gtbgfrxsp.sHtML

[T51] Scala：Hello World
来源：http://baike.zdbjq.cn/Article/details/ggzkbwitx.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/glrejvtpu.sHtML

[T52] Scala：变量
来源：http://3g.hesvh.cn/Article/details/gmnjwwkai.sHtML

val a = 1;  var b = 2
来源：http://www.share.hesvh.cn/Article/details/gaafpktdl.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gubofjapn.sHtML

s"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gbimfvxzk.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gluqnotfe.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.zdbjq.cn/Article/details/ggfvssfed.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/grykedfzr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fehbvm.com/Article/details/gixjgzmcw.sHtML

[T56] Scala：样例类
来源：http://www.blog.fehbvm.com/Article/details/gagnejwsb.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gknxtioco.sHtML

[T57] Scala：模式匹配
来源：http://baike.fehbvm.com/Article/details/gjubgfkps.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/grayrwkcm.sHtML

[T58] Scala：函数定义
来源：http://mobile.hesvh.cn/Article/details/gtgtkgytp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.hesvh.cn/Article/details/gfrfwquzm.sHtML

[T59] Scala：循环
来源：http://m.share.hesvh.cn/Article/details/gpcbkoeoh.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gnzafhabp.sHtML

[T60] Scala：折叠
来源：http://blog.fehbvm.com/Article/details/gqrojdgkg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fehbvm.com/Article/details/gokpnzyhl.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmcatldoz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/geyracqcn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/guvmkxhls.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/gwuuiftxk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.zdbjq.cn/Article/details/gdsqeupcs.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.hesvh.cn/Article/details/gjfyycezd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.zdbjq.cn/Article/details/gtnnsqect.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.hesvh.cn/Article/details/ggklkkhmy.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/ggzjclrku.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/glmtjursu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.hesvh.cn/Article/details/gwliedfkt.sHtML

[U05] Py：列表去重且保序
来源：http://3g.hesvh.cn/Article/details/gbyjcnxoi.sHtML

list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/ghlplmcsz.sHtML

[U06] Py：合并两个字典
来源：http://wap.zdbjq.cn/Article/details/glpfoqdiy.sHtML

{**a, **b}
来源：http://3g.fehbvm.com/Article/details/gbnxawwxh.sHtML


<!-- 参考信息 -->