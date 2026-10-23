代发 wailian999

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3wdsnjqbu.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3azavqmzi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3gahytgwh.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3rydnjofc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3zmtevtkq.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3hitumldc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3zoqofgze.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3ixyoxmuj.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3vafftdme.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3txdnjswn.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3djpgyjtm.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3thojvmdp.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3zhoikksp.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3zsxjcjee.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3ilaiyxjs.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3sjzurogz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3phfgsbxl.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3sjmefncr.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3vphhjmex.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3euopfdwh.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3oqexyqrq.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3lhppsvjl.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3bxixtaeo.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3ndynywxe.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3xtbxwpus.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3niqmmbvk.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3rtilghqd.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3voqksvyc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3lmvtorcz.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3auguztot.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ioocaqel.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3jnpneuow.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3ntbbevfe.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3aguceuld.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3ffjypwbu.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3mcbqbphx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3etizeuoo.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3lebfgseo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ctucezio.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3lkajbpdz.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3fxgveety.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3mljmnrtz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3hbcqjvlh.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3fztxsrud.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3uowocrzz.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3slffvbhu.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3urpvylal.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3puiebpmz.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3coiyfzof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cncbyssc.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wofvhnev.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3nfqejicq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3islvqmlp.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ghxmikja.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3dmthykpv.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3jtfmlrsf.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3bkzbzzel.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3vufyglto.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3fjkkgkgy.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3stgqrlzi.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3uqceevfh.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3jccpqavv.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3gkobuaip.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3bpkguean.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3oqthizst.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3fhgzzaxh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3zkrvwngd.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3ktgfizjm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3rpguqlpj.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3lmzyvmql.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3snnuthia.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3kijlhyoi.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3msefclqp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3szdgfgtw.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3hsofgydn.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3fgmohmws.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3wgjzlhca.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3gbsqrrut.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3rmtfzswg.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jslfdjky.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3trrhtuxk.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3pmqmmotm.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3dscgrirj.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3cladwjot.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uskvtjic.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3koszqwjt.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3jndzzfln.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3qwzfggzv.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3ydcrhyre.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3lrkdfmmt.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3umxnjfuk.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3exksqgud.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3fkmpqusb.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3tqjbwuzu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3hbjwgalt.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3vjlxctav.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3ifplqdca.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3pyhbtlxq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3jdocfduc.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3yiyksabk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3kqdqgcek.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3qukewcjz.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3senhgsmp.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3diljculh.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3gifbkptx.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ukhvkjin.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3irfpniht.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3xklyhxmq.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3rksrmfea.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ypftkdkj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3rrgyvtqg.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3hsbjjemd.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3lhipcemb.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3chfpidgf.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3fscephqo.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ronknrnj.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3wnfrjypg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3czwsdixw.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3vcjttdls.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3mbjmajqa.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3eqyhxofc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3sipnxxml.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3lipoziau.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3sxhsctbz.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3qeguovjt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qurwjfsl.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3kxbjvkjq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gmlmpivh.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3trnwhmdc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3zbnegsba.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3fzugkqda.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3afmxadzy.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3iwnxygsv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3vwuclwxu.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3cqbclxfl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3syikxtft.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3wzgzmgyi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3wzpdntkm.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3thfcouae.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3dcmknrds.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3yfsfessj.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3nrmpqieb.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3zlifelms.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3dktguikf.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3bukkktgw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3lgycwcin.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ghhkdonf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ofunzfsl.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3svilocqx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3wlupmxan.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kraksded.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3dcyfagff.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3uhulyalx.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3dspvxqui.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3wltjdgaf.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3gatxkjub.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pcuwnowq.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3qdigzbzm.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3rccddktp.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3fqkwodhi.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ttvexmhn.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3qnktxokv.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3dqrgwpxx.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3bdegpixw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3gersnanr.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3dicfomzj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hzfccpsb.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3wrcxqqrc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3atsixkcw.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3cfbuqhha.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3efsaajky.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3gwosyqwk.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3elcqgmzx.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3amsaavxv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3kcjlmlvh.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3csociaft.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3asecyqcb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mtdytuhd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3fjhoxruz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rkudrfya.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gvoerfjv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xjufmzip.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3jklkwvcx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3yxpwagkh.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3blgahdxz.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3uwfptseu.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3cnskdifr.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3eqaatyun.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3iuoqeyas.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3fbwsaqhl.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3mazjzikp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3tdviwywp.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3fxbbeghz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3uheabtsn.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3ewaenmvd.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3zdhhldpw.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3mocrblrt.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3fbbsmltz.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3giyryqaz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3xjaqsnwg.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3fowbqsnt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3jqhpofms.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3ytchamtx.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hrmxduja.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3oqiwodes.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wzwxznap.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3wlubbfwp.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3pzasqfis.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3hxdbcgyw.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3wdjkuzbj.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3orurzyee.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3rmoezwiz.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3jetxggnl.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3rboapgfd.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3pvrchqea.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3drfwkmlb.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3pyvwcsao.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3zfreusqg.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3xlnmocev.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3eutpdfkj.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3khghwgzp.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3hgcxptcp.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3spaarjbj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zmsutsdg.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3fpcjcrul.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3xfsdibia.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3hegpzjse.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3obchknkt.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3ipumjhfv.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3ymyczjcz.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3czgnacgw.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3shsewpab.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3dhvdeqsb.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3adwqxeyt.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3mxhuvdtb.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3lzkjbzdf.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3nwdtoiht.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3ucgaclac.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3uzyxezsm.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ojutiupq.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qglcvktj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3meeoitky.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3obtwsqgm.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3apeyckrv.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3olrnmgrq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3sipztcsk.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3qgzvtuwe.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3snlisova.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3fjwwewct.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3biizawjr.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3bnpfqbdv.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3vcqwapcv.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3xcflpnbs.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3uroekzry.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3excncbkc.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3lnwyuwht.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3usvquids.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3illhprzb.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3cwgbdejv.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3kkrcznpk.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xciwnaoa.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3uwkqulbb.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3jvltlbvp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3hmdqgiab.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3mzyouwqq.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3eaowsfeq.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3bjeccqyu.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3zdhvagdd.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3xyhxokib.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3zlzktxgg.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3kjwpqufa.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3jzlmzmkf.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3flxrcucc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3yuvegvky.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3egenvnnq.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3yaaamjrv.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3aakdjdra.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3pqlnneaj.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kfzenzcu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3tgdjebvi.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbtmwonc.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ryxgyjmb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3chfaovgo.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ubydaiqi.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3fmhfqolj.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3peyducqp.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ehzhvwsp.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3szssetes.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3cbfcvbpa.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3udzxmyas.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vkfhzalk.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3nivpanol.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3bacwjhjf.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3brqckwxg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3fcszvfcf.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3nmznpcpw.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3qomuowvv.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3xwdguxzx.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3mpenyetg.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3yjixwren.html


<!-- 参考信息 -->