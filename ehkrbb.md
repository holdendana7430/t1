代发 wailian999

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3idgfjhav.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3voacmbva.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3gyplsjkl.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3hgbbbfij.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3hymetaor.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3uuupmxcp.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3vywelvcy.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3qdicwcjn.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3jjvcfdal.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3anvzzryq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lskwfiqa.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3rbsfibtt.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ayaehirz.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3kkxurjtl.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3ogzcskxj.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3zsgacjhr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3gqvcuwta.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3eyifkrzp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3vaikzuiu.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3lvkvpris.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3aybhegtl.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3khqkiusl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3ewnulnra.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3qjhkzksx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3lidahxus.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ceniffin.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3bssiirwr.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3uwqbofvy.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3puuxzwwd.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3icyfqeme.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3wxlbmcru.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3bmnymgnc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3pnyiguin.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3tasmkrcd.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3wndsehcu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vckpgdfs.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3xribdiyd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jfwngxhd.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ofketiuw.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3nvyltifl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3ryvilkcc.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3sotpvbob.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3ufapwlfq.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3smtlycsd.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3rjixkfnw.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3zzhecpdy.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3twxspwnp.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3uidaaxcd.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ycjkljaw.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3wcvgwykn.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3eqdaavbb.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3xacpzplr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3vaaubvjn.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3uhxhipev.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3mfmjdpxx.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3xvxhoexw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3sghhubts.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3tnjwdlyb.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3mynkrjfe.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zzrvwiqy.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3lqroniqn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3vhkbljwl.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3bqlzrtff.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3qyukcqdv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3lcctpuwh.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3tnrtbkkb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3ycecwtyz.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3evkchjbi.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3ltxtomix.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3flxrjtpw.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3aibalvul.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3vjqxzqyt.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ozrpjjju.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3eforwqmd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3tqtfwijv.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3obgjxzwx.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3ofhyxdcg.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3gfvymfvq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3kpivgycx.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3qejkgejh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3bctydeuk.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3dafkxnzw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3wagicccb.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ihhimwsk.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3yeyangmv.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3acyvaoqj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3parojgru.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3ddkueteo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3feqdcydw.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3hqljvfci.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3gfxmjlgs.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3mmtnwdmq.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3lxnvaxts.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3yjnrtidb.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jfwvyjgg.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3kvpfulre.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3zpbgznxw.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3grabnrza.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3xobnkxmm.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3gtdwygjo.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3gczoawcd.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ueqxbbqm.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3upfgbtbo.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3peiktnog.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3tynggzhi.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3trbasagp.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3zapknqin.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3nfrcnnvt.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3asegucwy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3nlnzgyvn.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3wlbzxcep.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3aibssqyr.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3ckwhixkn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3krkfwftp.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3mlnolqvb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3paqmxesx.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3xinsjtdj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3sguxatjw.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3zbjymnim.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3wnxqyehe.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ivxbwuuh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3spovdfjf.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3obmlxcpk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3scwqcvdp.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3fghtmhhd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3pwstquoc.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3yxxwdtxw.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ctraniet.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3coyaxeyg.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3vlxvpuae.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3gxfjnhfv.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vydbjfyd.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3jpluilyg.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3rlmytndj.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3jwchktqj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3xjmbxvrl.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ovxzbgss.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3fnmiplbv.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jhnpyzrz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3xykggrka.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3dngcmzjp.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3nikfiont.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3tmfogccq.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3jbgbpndc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mjjodjlb.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3xuiubunl.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3negxmyjv.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3dgjkusie.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ojlkdwsy.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3ssgipsqc.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3ogkziajx.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3gcjpmbpt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3lpbqpypa.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3wsvvjeqf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3qtomasgq.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3ojzhirdx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjzonrph.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3nevvkznr.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ukjacjbt.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3tkrxbdsk.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tquengkb.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3txuwgrmf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3sldadgfw.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3jiybgsih.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3iykqtmam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3toydwfft.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3vzhcemfj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kydrjtlt.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vqebxuzx.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zbeagtcg.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3txzguwdv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3iimzwzfa.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3yprjivll.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3niqnuiwp.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3ukwiddbb.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3vrvnllrh.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3xnyonokw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3gsuqpjvh.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3rrsyiihk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qppdsvsh.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3mlscgfcj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3whhijinm.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3odxsvzws.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ukhvcbqo.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3ihudnqvf.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3pijoorle.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3pzndhxnd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3vkqargrf.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3faszemua.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3rkufgqor.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3ainqxryu.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3baftxegf.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3swwklacf.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3hokrzwvu.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3qhijcrjm.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qhfkatfp.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3qfinbieb.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3kgiwvpii.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3swhrtzhu.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3razrsxfd.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3tuwkghhn.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3pmhqyzcu.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tdvltvmv.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3xvdqbclw.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3qyomkcjg.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3utftoexv.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3nkhznczt.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3okbuvxho.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3leexchrl.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3bzqlrkrx.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3qwgozyvw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3oxyaoyyt.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3tekbrdfd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3cgveqeio.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3mgqindks.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3stnmvwip.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3lzoghgqo.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3twdehkxw.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3gxstqrkv.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3mcpgcqky.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3uqjaptac.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3ytvdtvmy.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3oydqsruc.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3hmofkbnt.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3wlmpvksh.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3cprpjepr.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3janettyy.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3uccghatv.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3eihkbjau.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wxyiexal.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3nbhbojsl.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3yrhfyeqe.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3hyhafwkm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3amkaejqe.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3hrjnihwj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3treutftq.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3smhqbvpj.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3chuwankl.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3gclzausb.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3lfsvlnhx.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3boahtfsi.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3wauhcghi.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3zuxzxald.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3cpfcfwnp.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3aweoyyux.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3vxbxlafw.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3fygwhnxn.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3qzhsxyqq.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3knsnxsac.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3rpfydhmi.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3kkbfydjf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3aqfoiahm.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zecdhtxz.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3eqiagjcw.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3mvvegdlm.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iyrxjdnc.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mhbbjlrv.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3gazqmpic.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3yuttqhrs.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3lbvlvcbc.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3gneyhixd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3kfpgxsbp.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3mnwzumch.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3rvlwbpsf.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3fgnpyidi.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggdiixbo.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mcpjzqsi.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3htupoaqq.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3skqzyvxw.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ekatmemr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ppdnhqgn.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3aetpfhjc.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3eyhztvwo.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gtktqihf.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3dfwtiqbj.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3vkxybyxf.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3akbclawz.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3zkaehpdu.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3abixwpzj.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3ibhefdna.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3mqwlyjgg.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3slaujupl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3pyxweidp.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3kzowelet.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3cokocdwl.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3slnycsgd.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3vqwbxnjy.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3ouxdfusp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3kzccelyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kbdvnczz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jcwtnzsq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pilgoavu.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3wfzsdyxq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3rtuhlrcl.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3shgonqjk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xefhfsjs.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3qbissado.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3ggsmkfyv.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3tmdruzpl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3gatvvahi.html


<!-- 参考信息 -->