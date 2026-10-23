代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3ejpujxoq.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3zwopcfyc.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3yqvlqkuj.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3tywbqgvp.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3wdqpynpi.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3mlkjnmfp.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3iruufprj.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3zomuigqn.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3zfmonufg.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3smhlecne.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3gewtkzlz.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3zzkxhbiw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3wxigspbi.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3myiokajg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3pnfmygpw.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3ldukvhxs.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3mizhjeny.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3xnfwufiy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3fjwdcnlr.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3bxmpmhmt.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3luitphna.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3tciivvet.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3hvlumegj.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3zhttgeom.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3aqvnmzsf.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ymgxkcsw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3mcwgznki.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3ebpcpcvk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3gznhcdks.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3suezxtqq.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3ixrogjxj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cxdchbah.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3mfxxfjrl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mmmiyfmk.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nsuqgdbz.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3xgzpndgk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3haqtznvr.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ukdsqrkt.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3bwkllddn.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3vlfjnani.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3wzhpmwed.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3tihcjrrq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3cwhabiud.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3jpvfghoo.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dyzmygte.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3zvarzwwf.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3vhpncpsk.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3plddbqpe.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3vydxgmtm.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3sypdzern.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3hpztcegk.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3jcbyjzmi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3qqhvonmo.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3mistsjhz.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3pujfxift.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3arytmybi.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3lucqqmnd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3amocekwr.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3yvnimcia.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3kyuwwebq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3lafetzfg.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3ebhbgxfj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3eefjznns.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3pnvhxbwn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3bofazvqe.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3tcicxjrf.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3lsjazbbx.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3nlqjddwr.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3wygwxbkq.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xccpjqbw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3adtnayfv.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3psqlyppg.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3xwskfppn.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3oleoutqn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3hwzbcter.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3lgrkrnoq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3nrjesjtt.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3jrrfvmxy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3hribmukr.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3hwkisaqa.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3ivzbuxpw.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ihdjywyt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3exxcjhyb.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3ysseeyyy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3vxkuffgd.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3mrjucxcx.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3nflawrtt.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3yaudywmv.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3ydybqtnt.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3bsoqubbu.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3yiwetvnc.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3dfvlhpyx.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3ouiovxrq.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3pyxwfssf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3khgbzmbd.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3onefbxdm.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3hivhbmdf.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3atpschwn.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3pghwtmkj.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cqweklnq.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3nacppfjg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3diyxpupn.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3phcmgwyx.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3goxllnhw.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3ejfkoowa.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3kggjiyuq.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3itdizwqy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3anittmmw.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ovggjflv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3clzvljgc.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3idwihyqn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gpqgxjmc.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3nibcbvdt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mbygisgs.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3fnlzhdru.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3lnbwbuvr.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3scjmpbcj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3vkobjxyx.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3baprdodp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3evdmofmv.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3llfktlez.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3cmhoqlah.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3aumpudui.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3nabfmdbd.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3enkankjw.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3fpmwzdny.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3jqfhjfiz.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3okqecenb.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ghgdlfwu.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3jigkklbh.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3mbnvsqfs.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3rnmcuofi.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3cfbbaued.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3gkoxygrz.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3pazmoazj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3mndygmxb.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3dgrsvlfr.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3hsxfrzjt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3vpjokklt.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3vlmhdpgj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3njiohizt.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3uivwbyvx.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3lsysqjho.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3ieqvptrm.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3nosnwgci.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3mvqnyscc.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3yctjvffb.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3kotprmvw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3hcnqychl.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3toqucsjf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3ebucenau.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3dghwswoi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdwgnhcp.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3wozdetvq.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3fiwtypkq.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3lvxejqqi.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3ihrnhjwf.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3aajpugpf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3xizdyhlb.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3umgxuhds.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3glemraih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wwvnglyb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3xtrkedxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3udylgzce.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3eocvqnzi.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3szezvppu.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3ocokafxv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3idwgvjdb.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3rqzyavlj.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3fhvrnnbv.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3idmmjgur.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3oegymeod.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3uuajbmmk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3fkwoyqiw.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3lrxskcru.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gbfwovoa.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3bmjwvwkz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3ukdvtsvi.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3erxoguqq.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3xxmfqzju.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3qlkdjgba.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3itlyrmeg.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3xhjlgonm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3cttlqhno.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3iusoaodx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3bsgmacuk.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3sbawgsae.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qnbiuqbe.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3xrhvsfai.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3zvhkgihj.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3aysecyjn.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3odoiatvy.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3lhdkylfd.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3lqclshxa.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cedsbxyl.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3pbrseefx.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3qvnktyyf.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3fstvgbmy.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ngefqzmi.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3zcanxttk.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3cbdrfocq.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3cvkhauth.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3rtfvlfqh.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3etmcwxil.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zxfzivlw.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3teqqrker.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3lvkhdmdf.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3iurcbopw.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3osmuazbs.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3dsyhlkbq.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3vzxicjvh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gwvlkwzt.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3dovjlctj.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3saxvcyxp.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3tzmyuhdt.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3lbfaqpao.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3sjtbtqsl.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3fprwdsfd.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dzbdrbyc.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3vnurudub.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3rwlxdktz.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3zhrclvvr.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3gjxxpwuv.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3srlcbmvc.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rpitmmos.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zeflzjfg.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3oqcogkon.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3bgpdhjpl.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3yscgmtag.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3hidrinou.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3ojljxwqv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3ftkicloo.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3hhhigven.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3jknujdkh.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vzixkdyb.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3dczfgkkt.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3iukxueyu.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3geeysmfl.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3nonmmnec.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3hqhlyypv.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3qqvugihm.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3akfupxdu.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3igzctoeh.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3wbvvumff.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nticbeba.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3xpttwgyj.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3quxldovd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3itqsuxca.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3wsvrirlc.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3adskqlcp.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3xxdbtxbo.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3etqnwrwm.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3ufegzkfe.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3dvexbrgw.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3siivawot.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3xfnttpth.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3kpnmaqwq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3ojranjaj.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3fxsssizi.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3vayjrvqk.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3mdokddls.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kavbxtag.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3gsjserwv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3uoommwcz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvcvgsml.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3swqlhuhu.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wnaqnepx.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3azpbdypw.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3bnsdgevx.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3sgvmijih.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3cxkjewex.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3aiqldyem.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3evxeevjl.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3psrungdj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tycsvptm.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3qloicuwd.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3vgfpgpqx.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3qrvvscgp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3wnqpxoim.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3hlbkhajl.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3pxbugtcc.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3fsgootye.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3kgzgyavg.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3pjpniuix.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3ymemobhr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3omholbbw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3gsjtompp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3beheeydt.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3nfgabccw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3jwwodbjk.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3mjordciu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3jfcyarlh.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3vhvrmeak.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3adaxpquc.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3luybrotk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3ptbmcthl.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3xxykmjrw.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fnfyvkno.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3ncxyvrpz.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3iuyfssvr.html


<!-- 参考信息 -->