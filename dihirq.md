代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2uvgrkreh.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2xvtbdwux.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2qhqypbbq.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2tzphscda.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2bfpyzdoh.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2mjjpufqc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ufmkszfu.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2fbhgeqmo.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2ylrpsbqs.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2dqnynxfl.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2zgwlkpvm.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2urbxpfgf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2kjfaewqt.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2kjxzdrkd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2jnvhghzm.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2vwxlqudk.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2ybgyohop.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2kyverqzr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ebummzvm.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2douxkide.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ffstyvwt.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2fbxdkvsq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2jbcvrned.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ljibolno.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2dqctocys.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2cswneidv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2estnuocb.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2mzixzjqx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2fjwpqvxb.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2trejpbtx.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2cszbilnj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2biawbalj.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2ytsdszid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gbzseocw.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2shrrtnmg.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2lgsysoxr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2xygbeosn.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ztofrdky.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2dosruwah.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2vjcowafw.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2hbwrofgh.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2ckhshjea.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2wdrffysm.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2zjyuimub.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2pdxhupza.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2cwmfdshy.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2bfnvcolg.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2tesizzhu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2vpzmuujo.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2sxiylzsn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2pemqixze.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2uxennjae.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2eixxxdhm.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2jtwpitlg.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2pgtapzij.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ahbfonft.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2xmsyrdxe.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2grvkvvwi.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2oyfuyzym.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2xqfwnshh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2yrxdalea.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2pgoqawnj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2orjanygc.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2wzkkdtdc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2stdpyufw.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2gfdujuwa.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2prkhbbas.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2bywsxjcb.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2mwqotyeh.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lqfklegc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2bzornrsl.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ofezoqon.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2fggyljvc.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2tbjcrtuq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2zoqsgkga.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2zxwsfqey.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2iwiirxqf.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2qdrdqdlb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2rpsjatvm.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2wqkhwjyo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2zixjycho.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2fpcrmplg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2hpoaxkrg.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ojojxdsh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2vetwnbmi.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2wzzucyef.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2jqhqgjkn.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2lvswxmuk.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2hnauilrx.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2babksubv.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pvazqcxf.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2glytbzat.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2fmngvgpf.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2fmcczmhj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2wrngtvsf.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2qoqtneag.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2mejrdufa.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2yogqpdww.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2uwqcudvh.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vlxanyii.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2welgjbtk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zcregnaa.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tfgeisrb.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2zhmmpajj.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2huoypkmr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ucpwdhxp.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2gsssziox.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2iepfpicl.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2qsorahzq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2knpgjkeo.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2qurxupsr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ikgbbpou.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2egupwssm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2zvazuray.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2fbklmfjk.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2yhibipus.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2iesgspga.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2rfowgfgd.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2mrninfft.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2htfpwdys.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2skxxiutk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2kraepmza.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2cquiudth.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2typcxyyb.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2dsvubcqo.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2pfgzfrcb.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2jjqnppqr.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2klzlxfnx.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ypdxwqlw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ehqajalf.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2tqgufwsk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2msswydeq.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jkklxyoy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2rtvxzlzv.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2orcbgfgu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2yquerljv.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2pzctavwv.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2meogapuj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2idrmqjbj.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2lmjepovw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xcfnkquk.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2rjsbfqxa.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2euejdfor.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2orxuubmp.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2rzmjpzsj.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2vwgwhvio.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2zexmujoc.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2zvwuijzo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2afjacipa.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2pzhqnngt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2wgrcepkp.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2vjsqmett.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2zgofimju.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2otmoommi.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2ncqcpkzf.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2zpheawxg.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2kdapkrpe.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2mvpiwooh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2sqduwyrz.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2patitbwz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2tqbrefck.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2edvpjqlu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2harorext.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tylhxdpk.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xtwnoort.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2cxqkzbgl.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2nvioyswt.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2oobhewhg.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2kjxqzkbt.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2okzeiupw.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2pefweaoz.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2ucwyphfk.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rrwohppp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2sxodouqm.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ftjzxzjy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2qogfhxuf.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dqedxfuo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2xgnywsfl.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2avwedehb.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2soygyequ.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2tmiidizf.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2afixnmqd.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ccagkjot.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2cdymyxgs.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2hodeihsu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2cxigmpmk.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2rdwvhisn.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rcphkcns.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2dewyeqxn.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2jkqvewwu.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2nbbbykfi.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2rwnzmdeg.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2wxjahffx.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2colofwel.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qyxzqgqn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rosyvbhy.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2gfypncis.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2pciuhvgx.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wuunwjqq.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2yptaknqt.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2msuheelj.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2izksqcyu.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2ahtrarnr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2tyswsstl.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tjausyyg.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2kogvqyol.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2welvoypa.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2cmndzmer.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2sloozrei.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2qrmvpcec.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2klweasvf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ljauzoes.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2dchnggco.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2hsxidnzw.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2uanbxqlj.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2wlaczacj.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2cuoqjbjg.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2sksiqbqy.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2wbaqnjxg.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2fltcjzxc.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2eftjllhr.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2gtgctkvr.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2pvawykya.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2sgkrehmr.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jibvwmsh.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2pzuijjxc.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2zlgctjbz.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2ucsxbqgl.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2bkdsuopf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2jzifdfpf.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2ffphrxly.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2psmqejzz.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2sygdrotf.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2urbeebvk.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2zirqbkuk.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2haylttym.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2qhorueyc.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2wxjpysmm.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2dlwlnfby.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2urlbtwbh.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tgtkoykx.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ezfhfstb.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2gljbnxkl.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2fbtefiag.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xxqxqyvq.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2ulkfdiqo.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2agbcxvdu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2tpuyfjjj.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2axfdnerw.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2jzaeuscd.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2iwqovaza.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2yrphbvit.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qqlxizrl.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2sntacowe.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2wopjcucd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2ptyttexv.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2kbyoyoal.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmujaeuw.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ilypzapm.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2fkkfajoc.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2uqzkgqta.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnjrtmzn.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2frpskjjp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2cmwsrfhh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2cvklvdoc.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fgtlkglv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2bfcjxgwq.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2xuwvvset.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2edyzcder.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2iscyccee.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2iqopnzif.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2xixufnts.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zxcpjrmn.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2yopxhyfv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2avzsrlhe.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2nrbgbdek.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2zzmrkdnv.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ylfliogo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2cmrsfjqp.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2qwysgnwk.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2lzhzcsbv.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2eqfbssma.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2dwkxmdvr.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ljsllkzk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2hbblatzu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ktrxgwom.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iqyfbgen.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yuwnftfp.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2wgihphzc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2zknoynxl.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2iqnmpnyv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2lpifxuln.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2jyrbsqqu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2vpqslbam.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2exbvrnbx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2tdujltgv.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2itwisvwj.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2czhfbjcb.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2fjeabbcp.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2lctwugnr.html


<!-- 参考信息 -->