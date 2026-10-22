代发 wailian999

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2wpffvxhi.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2ufnzkaka.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2dhipmvlo.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2hyjlhbkd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2ufyzdeui.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2zndgupsc.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2ypzvheny.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2myujvpzd.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2jnsdeugd.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2cjgksfcv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2rclexwzk.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2fpjmpamd.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2dajiukzt.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2qmmcqnbw.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2cneokcxt.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2rpwaeumu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2nlhqxtjs.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2kytcbhct.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2qvgrqwwg.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2kdtpdnit.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2oekywtwm.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2chqzwphx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2jyspjhdo.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2dnzjtyre.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2tatyqgcw.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2tsvgllhq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2uudlpffb.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2tuvyblzc.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2xjfseign.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2jhsukige.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2ttqniuqt.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2jomureis.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2pqhgoyic.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2dsskgorf.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2pfkzyvtg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ionumcrv.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2elquxygm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lmaafxow.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tjnysmjb.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2uvbporsg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2albeenqn.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2chewprcs.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2epdbunkh.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2rcrzzzwf.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2yucpwymm.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2dqqvxpot.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2izvjvqvl.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2jpawzfaq.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2xhojskmb.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2wdjrvoth.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2turupikg.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2muiwuvuz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2auqsaynh.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2hvhxqryz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2fzujmnmj.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ghgpsodp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2groeacjr.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2gmpnxtpd.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2tmvmxzde.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hzjxgoen.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2amwjwpok.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2wmkusqvc.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2okypelyt.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2zeynrdym.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2lqrneyhc.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2gmxwsnxq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2jwzprddf.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2ajjxsoce.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2mrpyocxv.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2kankamms.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2cmjojfxc.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2cijbahxd.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2zwuiwezp.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hnjkkkdx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2fsdehqfu.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ukruwyew.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2byryapzk.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2szhixwxh.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2kpmehazq.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2refvjwhw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2kslwgyxk.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2hsksmdqs.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2jrjmhkdw.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2fzmctuot.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2nmfhkpeq.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2lzzgpbov.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2rjgeouwe.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2tyvjiixz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2ihsljsck.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2euxtmaku.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2pdzjwpxf.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2yxkohoeg.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2lzrghihv.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2qdyobdms.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2eqwxkmex.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2xmvgrfeo.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2wafhxxtg.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2xltuvmuk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2urhgzlzp.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2alpsjzca.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2onhkqbii.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2pjoqodnp.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2eewysuhn.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pdykshvk.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2jojyfshk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftvspipo.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2crzcjefp.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2meddykqs.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2chgrkmov.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xtrzfrxq.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2zdtzmhnq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrdljbmb.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2aoybrsxw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ifxlycwi.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2sqhmgopf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wkcciggs.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2ufwsagvb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2kngqkytg.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2xnynzkgu.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2dcakdoad.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2ccedcsaa.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2agynrbeu.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2eacmymlj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jzjkshvg.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2sgjylvtc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2vdizyyce.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2tpsveviq.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2lolccqht.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2jnedilue.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2kcqkhzad.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2zsxjvcbg.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvorazbn.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2bqxxwmde.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ogwekuzv.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2uijfxkmf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2drmruzns.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2moplcrqf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2jegeaysy.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2maqqzgcd.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2vegfwqal.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2fwnntmdr.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ntnvtoub.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2mgttxrqs.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2rkmxnpna.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hnghhfhl.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2gvraogoa.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2axwlyczg.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2tutrjgoh.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkbcupem.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2eguwdybn.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2eywxystu.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2ahxndbpw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2nzybroyj.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2vqyjxjtp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kaxsunut.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2dkhjtfsb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2vvoxuuao.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ozbibrhx.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ouwgfvwr.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2dqxuiqfm.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2heafqwhw.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2eedhqxzq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2qfmdtkpe.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2zlztnqui.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2cbhtsydu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cgzvowmr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2vykmfdcf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iliskpzj.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2itaimlwt.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wtuvfgtu.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2bhqudlny.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2mwlanhfx.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2qlwjzzch.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2nfebnrql.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2kylweeec.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2wyuwjbcd.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zrywqjcb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2lmqnkltn.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2bahukdse.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vizdmqjq.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2xbxxnuch.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2mmruwcuv.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2krjzhdcn.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2iwzcjysv.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2aqvtcppw.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ecoscxwh.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2hzsyqkaf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2uyqzfrjg.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2uacuoasf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2bkkcfnkc.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2ojlzepgz.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xtfhsqsm.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2kflwccfu.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bnqabrte.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2bvssxjbu.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2yhslnlzz.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2wjktwqwz.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2drnngyob.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xtftjemw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nckrhbtx.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2gwwdabzu.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2uinyqgzu.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hyvnyqeo.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2iepdglcd.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2tosvigqj.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2gunsuxia.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2utjcuyok.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2bdhsuxrm.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2dnfrosqb.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2mnagkhax.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2brjywumh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2ekxicbqd.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ztnfshwd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2kwlwemuv.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2ovoqndnn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2scxaektj.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2mjnrtgih.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2henywctk.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2irozxewa.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2bozzchog.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2dwpmtxgw.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ixpwhmbz.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lgxtlayh.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2tybnicbx.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2qlfmycms.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2evssfanu.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2yprrnxwr.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2fwbwozbp.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ycxwnhoi.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lhmprdkf.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2bkrbskhl.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2eurtucwz.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2poufzuny.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2onzvjeyc.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2ccmlsdto.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2qwemhhgy.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2scobmmgo.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2yypzzkeg.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2dyvokvkm.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2bcatahuu.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2hcjhsoda.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2mqvsiyrf.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ptyuzpzl.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2ihcpomnr.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2hdmyagll.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2nhmofzlb.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2yjqhgfsn.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2chhpcpbn.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nugkexqx.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2doxamydx.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2bupqhxdo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2izzdsldw.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2gtxlsxqn.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2jwbzndis.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2wtszmwmr.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjplpjqo.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2oqvapwwo.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2smgowayh.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2qknkijue.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2kqxvgqed.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2nvxqfdhe.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gyvzuwdx.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2eordfnsx.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2seyadwye.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2hahaxcpl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2gdfplouj.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2cofkvgif.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2sifjmakh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2atgnrtzj.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ljelhgrg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hbxyduux.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2hdwesoxw.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2bhgajhvk.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2nfjjpjji.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2igvvzvow.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2vuysikxm.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2piaodypg.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fltstcpf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jjjxdrvn.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2rasvtnjr.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ktmbuwae.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2olaxhdnp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2mimwwzbw.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2qforyrsz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2prnwqiyb.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2wubxaqbh.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2oawsxktc.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2oiomxavt.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2dpxghqtp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bevtjkvp.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2azjjrbsh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2efguwoob.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2hqmprubf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2wmsazxhx.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2bwzobjsf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2vgqppdeo.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2sarurqzl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2bwuvnyjr.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2hqlsckdu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2sjfzawwj.html


<!-- 参考信息 -->