代发 wailian999

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2unfmitru.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2ogqchgpp.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2estibxqj.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2hnbhtpqx.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2abfszxhb.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2mqwfqlvt.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2dkienwev.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2tfmqjcgg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2wtrcuexr.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2gvwaehrm.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2feciqbva.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2pzxkaowo.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2xngnmlqs.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2trnbevvk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2gcbxojrj.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2swsxhyvn.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2yvhvnhzc.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2ejveajmy.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2mibkpxqp.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2cbtjmnot.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2xsbppzln.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2dfrnhhmn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2zkonsqvf.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2nadodbmy.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2eadaumya.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2onhbvdyh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2yrtbqwoo.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2cvaxyksc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ynqxlknz.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2hqidigtu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ulfzilak.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2zkgkubwk.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2bunqxdtd.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2nhzltsef.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2pewntpdw.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2gzgpkgaz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ikthaqrj.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2qjnpypsk.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2gvacxesz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dxupjgec.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2zvcqrjqm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ujsqqacq.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mxnxroye.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2zckrlhre.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2hjvzukuw.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ndwccswy.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2fclgdamt.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2andzdilp.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2gbnmhheu.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2ibncpwwg.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2gtxjfvof.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2oyrzrcwv.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2baomnyzt.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2jzsmpubi.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2oxkcyhhq.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2lmihgalb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2lhrprbvb.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2tkzoegac.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2iahdnmte.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2ruipiiij.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2ijfiyavt.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2lyvehjhc.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2eigdomzr.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ucfvlhys.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ncvbkcdq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2lqsbclbi.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2uoxmlzvv.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2ncpfbvju.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2twdxglac.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2wzgxktaa.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2lhxpnkpz.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2yexyrgvk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2lrgrlxvx.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2cpxjgapy.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2pjcnpsbi.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2neodhjss.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vgujlnzy.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ybzfmjoa.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2hsobxsoo.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2rmqccrly.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2mobivpey.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2pptvdykq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2fzfblaiy.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2rpooceyk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rzdpswae.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2quzgswmj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2grdnbqpj.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2twsspdlg.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2tltcswqk.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2zydupnun.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2yqmmnogr.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2cdewbbuy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2ficelbif.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2ebxjfsye.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2itictilq.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2fcoyitou.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2ojvwqvoz.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2jemekxyi.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2korsptmf.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2ihtxrdud.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2nbgapzkh.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2otdkiwpp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2bsggozqd.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2zzrawdjg.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2cuqazozb.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2jnarzcpv.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2autdlkdq.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2saebcznc.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2frkxeswo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ytehmlmn.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2dpehrjta.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2bwwgzdav.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2ynzjivva.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xcysruss.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2rryvecwq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfmgnnbf.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2rdojnvhy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2awugxize.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2njmcyknp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bwcrqaot.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2avlibvlj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2enkecxpf.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2dcsvgklh.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2aiaomkvx.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2fcgqhxlq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2xlcgzrap.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2ygbatrtn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2ipygvfgq.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2rpativrn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2cdeootke.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2wyazxczb.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2jvenxlwo.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2bzqjjtom.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2shzttdjc.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2drrjpzme.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2fwotztbr.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2cdrpodgt.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2jqpwposm.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2cmqgebbk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2tffgmfnw.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2bqxwwpqi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2sezxedhf.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2uyrfaohi.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2mzesjxmf.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2tqaaucia.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2gunzvjbd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2dwsvdioi.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2ejweghpr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rdykafoi.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2rtbmvyis.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2jinsqupo.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2bgrpgzrw.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2fgorsaee.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2jzggdlms.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2vwkmuwqi.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2hhbhsskg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2tzcfbtkc.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ptihlqep.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ltfwqvfh.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2byzfhmlh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2gxagvxnr.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2tukhstyq.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ybtyrdqm.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2aunstczg.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2efmujiyx.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2zveknjiz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2pipbfboz.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2uwmbbwbr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2aiurpcyz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sjpoibhm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ohyjljzv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2klardmnm.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ljnyehan.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ebkbxqlk.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2bkwuhsky.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2wsdtjleu.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2xzwkqayj.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2vwzurfuu.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2wtwvdfms.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2wuhgvgrr.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2irhqkqvg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2rjttzpgt.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2bxlwnlfe.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bjpfrzsf.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2nqsoknlp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2voqoqofh.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ollpfxvz.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2jckjftjm.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2csznfxgi.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2nbnphbxc.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2ccvbhshs.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2ytuzjghd.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2rlrwrmpo.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2azcbitbl.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2qhxwpdkk.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2lhfpyfsh.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2bnslmxlg.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2cedpvekj.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2dtjsavrk.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2cjghqeyr.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2lyxhjsvh.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2mjoyktwo.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qitujugv.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2opjwenbq.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2ebrepwpi.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2mghprklm.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fgpibapk.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2quyzhimv.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2qbqjoyam.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2axsbyxxu.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2qjsxxkpi.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2bospglzc.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ddarunxz.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2zgtrhtbq.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2pfsrtlhj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2tbgknkon.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2aavonuqa.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2ypkbxffm.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2spzuzgeu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2fggetnwd.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2ghteksml.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2ezufhlbm.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2dmmjghel.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2bxgamdnz.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2mbxqenwz.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2umdjhwqz.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ezrrdmnv.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2cdunobyu.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2lvsxwjwr.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2qxjczutj.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2wshnickg.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2lbqqnbcs.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2icxuoulp.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2txzjxsmb.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2vnclocqq.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2tjqqsykp.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2dzrjgxgg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2oaumhvyg.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2iixsydqw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2npffbjrm.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2lkzljbrq.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2fvffzlwl.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xuccjlsx.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2irtkrvqs.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2hwdgwjjz.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2nbugchwy.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2lprmpgve.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2qqkqscmi.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2uhmjrzvy.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2nkannwrq.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2mzxfazeq.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2upjheoat.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2azwgfyaa.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2jprfnxib.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2fikvnkij.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2olhzzzrg.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2yogrkafw.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2arjsndre.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2tlnknhyt.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldmwzmkg.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2qqebnrwd.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2jlszbkud.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2moiqftyv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2zstsdwob.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2hjkfgtoh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2rplimeul.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2qvoktylm.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2ryvcocnq.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2mlrwcjzm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vwyogerx.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2nhvpgsaf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2hhwnqpnc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2rjbqjjzi.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ctfmgbix.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2bkbyclrk.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2dmsrflzh.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2awywxjjh.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2acdhcole.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2pzqxraxx.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2dzjzyxuq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kfecnpol.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kbxubomo.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2drkjygzc.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2dkqxvjtb.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ditplmmw.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2vzoychrr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2npijmuji.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2ppiavqcy.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2twdodwxu.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2rdkulkvq.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qfvdtzql.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2jeaccaay.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2tjryijkr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fqixkudg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2yjdkygqt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wytclxxv.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2gxwvmxxx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2pbptjedc.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2fyhcvjmg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2iybmlhwc.html


<!-- 参考信息 -->