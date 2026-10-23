代发 wailian999

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3gubtwpbi.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3ozobbovj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pxtnxbua.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3rprddggu.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3ieodvdza.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3teihkpwh.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3nuhxnkar.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ajpawmsg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3urdeqose.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3vcocjxcm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ikcwkihc.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3kokqzvpa.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3woqeunlf.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3oplcdxtn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xezxpzrs.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3umnmrwwm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3ewrazyhu.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3jqbljxbl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3lmwjlmkh.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3sqnizdrq.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3gvybiyyi.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3efcvftpl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3pzthmylf.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3dqzpytua.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3wsxjeijo.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3roadgxmh.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3epxwpvts.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xyqwvbyl.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3uvmtivfk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3avqkzjol.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rvfgbhtw.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3onyqzysn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3tlvyimdx.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3pbkprewn.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3ixtwkqix.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3pushlobm.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3suaxhcso.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3dsmgzhkx.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3pkhtpbww.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3hlutfyyi.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ciwnsvha.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3srkbhneu.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ethwrxjr.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3fjygfgfh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3jqliqlqp.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3vbdhbwxq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ijpajumf.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3dxjgefsl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3iokworrc.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3qtktvbfy.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3kpekpfbn.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fhrlaczn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3bfhuunls.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3lvthsffb.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3swhpdvhm.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3jycjqymh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3nppibdvd.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3ugttkkrb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3nwgnzukc.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lpmzmjcu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3yhnethim.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3fmbmupjs.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3jdfhefcf.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3hbpijsmd.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3xcindfwz.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wewncorx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3oravorji.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3wugrtwla.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3auihabvf.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3vhucxnlb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3fixkadkw.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3nqxcetrm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3epaecfkx.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3xqomorqa.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3xjvoaylh.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3yiiolevy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3bpzimyyx.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3axsjxwit.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3vgdrhtrb.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3ppznvbal.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3wljszyfv.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3pbjqbaxu.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3mubkfqwi.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3exwiuhtu.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3tcxlnuzh.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3udvpdfjx.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nsjztows.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3rqskgkxv.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3dwwmdfuj.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ihlueudg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3wxouyrhp.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3gmbwgdrs.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3lplxpzzo.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3fxhdligt.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3hctflwca.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3grdcxgom.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3autrsqgo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfhwfwxb.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fujfjpsg.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3kyqyporo.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3osabccyh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ritfwlrq.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3qisfacqs.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3yuktwvlv.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3sfrjjkeo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kylwgfsi.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3gzjjzbdf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dpvymgwy.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3wyxywbow.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3nerolxih.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3lfwqtfhl.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3vghegbrh.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3jevvxovf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3wcoyurjj.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3vpbichwl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3exjzlsof.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3cmdbssmk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3lbrnwkpg.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3blpymrtr.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3tnggwypd.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3dpirpelh.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3soxqfowg.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3sformvdh.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3wnewicgm.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3zzwrobii.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3sjwssuhj.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3mozdcawo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3nyxijbrz.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mcyyusam.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3wjrswgap.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wdyjuqsr.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3pnhvgcjz.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3bdugpzrp.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3zjyslszk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3cadbhrzg.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3uikrcmcm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3kyinpagv.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3gcittchs.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3jokgrsyf.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3uppcnxva.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3qduoztxy.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3fcftertw.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3crctbgok.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3hcnocjtx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3jmtafaix.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3vrzszleh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3itcszqof.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3gzixsegu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvsvwasx.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3yeigtwmi.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3hjybaujx.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3essojfud.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rrfmnjxk.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3lmahataq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3tkshzqop.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3tsljpqgs.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3vzprbima.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rbtqhzyc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3wucvizzb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iqwfiocp.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cgtnqsun.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ecdgdtnq.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ocoocxrq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3dokqiurj.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3nccaiecj.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3gscgibhx.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3pjcfqwsw.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3vaecetez.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3yzunyrcy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3prwlzhci.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3brnjvsbr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zbrhlilz.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lpieiuvq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3jaefvwoh.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ppsudpey.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3wrplgemk.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3fkqbihlh.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3qxfkqben.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3pzmgjxhs.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3yckktlyi.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3yykckfqb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3lfpqvybw.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3xlekxmlo.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3osvvywlz.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3vdfvaycv.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3hzuzuxnu.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3rwbbuabw.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3niijthpi.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3dbcayfhh.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3hepruvuh.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qnpkurqq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zsqbnyre.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3swtiqokx.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xjfinkgb.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3nzryfcds.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3tcdnwhaq.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3vtgdkuqa.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3jozauynv.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3varrqjtz.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3rnhrpoqr.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ewigehml.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3xuzsdwuj.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3kxsjuxwz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3qqauhigm.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3mkmudyyv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3epwvprni.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3zxubzplh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hfqujbno.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3ouaaxcdk.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3mssumgmk.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3iypedlmg.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3zcwcqvwb.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3wxclskrv.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3zxnpnwze.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3eeouzvvl.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3vetjderf.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3whsfrtgm.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3xagvyoxn.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3xiqkklqx.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3acnjiwjz.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rgbglhdm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fkpnkfuo.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ajxlokxr.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ihyygoft.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3qqprbdfs.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3adjvupau.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3qqsoclcx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3pejfwxnu.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3xrijzgze.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3cdljouls.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3muwfaxlg.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3vcvwqxmj.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3xawjlfti.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3wpcegncb.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3olhaevhl.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3acauygkw.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pxdkyuue.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3znckayvb.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3vivlnatc.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3sczqftqa.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cfpochxp.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3cegogekm.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3tybmclfn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3gdmxyhia.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xwhskouu.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3bgjpvelc.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3uqjeksjf.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3cefytzly.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mzyeegnm.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdkmwazl.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3xvifnguj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3wqfolhfs.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3vekydliq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3yysbtsbv.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3msljzory.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3mvxcmwrr.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3hfnxilob.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3bisjnflz.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vclsmznm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3taafnqpp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkxwglbn.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ljzjahed.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3nrmfohby.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ypveabxi.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3yipgdpdu.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3mpzfzutj.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3wlcmkfnp.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3jqpzmrqa.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ujpkvdjq.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pbwvsrse.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3teotwvry.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3uffvdokj.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3csbqzmme.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3dcrssmfa.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3fkplzpeb.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3bhvnxqim.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qkeefxra.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ezxykinh.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3hkbxoshg.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3dtgqqomu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3ofsyhdzs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tsbtmxkv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3keyzjkfi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3isinkcxl.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3ibpfjwla.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3unxkdgmk.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3rfdtqvoz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vkkjmwhk.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3bqfidalr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3nchqyvmj.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3tluwmzlp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3olmhpjmz.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3bicgmhpu.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3nnawhfrq.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3bosjfhkz.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3cjmqzlki.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3wgukhaji.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3zawaixur.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3nekrzrpu.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3vhdmlgfi.html


<!-- 参考信息 -->