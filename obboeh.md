代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2vdwyvtam.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2zpatnsdw.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2dqgmpjvi.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2aolauhes.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2pcvuenix.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2giypxyql.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nkbsoduw.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2yzxgzzqj.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2bhhiujrj.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2ncjvpybq.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2wmpzkecw.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2tuxalwws.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2fixpjkyx.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2olfusgur.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2zaqbqdiy.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2ijljmxos.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2hztrpxpn.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2vbdlqffx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2vxtunhdq.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2qtwzjhbm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2vmccwrlw.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2ybgtgnbb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2nkzcsuoe.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2rgtcitra.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2yqftmete.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2jfpvdylh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2cplbidyi.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2nbdqsczd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2frbmsiuj.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2zbwfbqqx.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2rfxsokbs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zcmencje.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2yospsrbf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qolhfvzz.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2plbttyrf.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2wxoavqul.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2lbvkgoia.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2zwtuivot.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2eriyabkb.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2bjedqtbm.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2lsvbched.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2aclaqsip.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2pcxlncec.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vxeduvns.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zkrnhqzb.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2xtinyguh.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2diqnwfuy.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2umzlwgzp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2ybqwzglq.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2fgmomaam.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2ycjhsbho.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2qzxqvqaa.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2wdueegno.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2xctaydtq.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2emzbtavy.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2phgpgyoh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2frojroor.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2qqunzkcx.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2jivyacld.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ipvvwwbv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2wsngxiqd.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2kyxponxa.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2vygnblfi.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2swvtmlbd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2fpwehlgz.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ryretklt.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2ecezuaog.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2njwktvnh.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qlholase.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2szdwqxrz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2hjdaybrm.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2isflalkv.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2mslhugwe.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2weziykdj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2txlvzgel.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2uavajwhu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2vwwszlui.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2lpsbstav.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2loktakfq.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2mjiehbpv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2gejqwxsh.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2qzgotxwv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2tjrucnjy.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2hkiissor.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2wzzwhfda.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2xddtifna.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2yjllkblp.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2vodcrchs.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2atuhrkyb.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2jksbwgsd.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wbpbxiwp.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2eiwrtmdf.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2calbsylu.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2lyavtfoy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2gueadlhm.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2epkwthdk.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2bncajrkd.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2dpwvclvk.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ixjsttxu.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dkemvusl.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2fwdelozs.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2exnzbxsc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ocltkmfn.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2tfhuepqt.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2hpafbitj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2iqltlziz.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ojmsegch.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2jhjxtoet.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2mcvencxa.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mnmxiojx.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2wzecnasi.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2cmbyosay.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2puazdreg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gqydzscv.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2cxzwcmss.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2kbbbuetj.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2bzlopjcq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2ntogmndm.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ceqgttue.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rjpxizgu.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2sdaixrex.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2tyivnumt.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2laebujqh.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ndklpmbk.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2rwcieadg.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2xkmafaia.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2jmzbbtlq.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2khhmnhwz.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ldibitcq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2bdmyhlwf.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2ylroggmr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ssdljuwp.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2mqwwhnnu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxopkgrd.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vlpvarps.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2znapeuvd.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2nagbejek.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2pbbarksg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2buogcyww.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2rbzdvkgg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2sujfvhsd.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2zziccsqy.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2nckrrljh.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2htvgakbw.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqrydamf.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2qenerskt.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2txjxnfvl.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2hifyodzw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2eyqrkbgi.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2npdoqvmm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2zfbcdinz.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2upydbqxn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2egthuyec.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2pnujrnvm.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qmvegopx.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2vpaabrey.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2ixzcqpnl.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2jfyzzqmo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2qaqmefev.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2kgeyohzi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2rdhqpyfm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jocdiusl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2rugcjoyk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rfeylnbw.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jkdjbbic.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2puuymtgh.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2asjloepg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2brzydlbv.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2sdvwcddj.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2oeyepovf.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2kjwwptph.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2idwjbvpg.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xwzyfuge.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2zxhwuheb.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2alwhvkwk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ktblybty.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gpfcfjtf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2xopniwiv.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2rtkqtfsv.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2lrlbdsal.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2wznaciyv.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ygtbpspc.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2adijgbqo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2hzwglqsg.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2gsmabfvc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2kefzxxfa.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2txwghllo.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dkfvyuqp.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2nvsamxnf.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ssnxfcrv.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2ginfzbgl.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2osteqowb.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2fpcrdnzp.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2owzpymte.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tqplvbat.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wessizwm.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2ujqyjalv.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2foxngfrr.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2quokwhgs.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2lrrqbayb.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ftjcozkf.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2fynzioix.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2jjtpczut.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2bxoztxud.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2ocwaaycm.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2exmmwmur.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2ucwssaez.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2owtaqyfq.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2seguhwbz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2pcudwzsh.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2rqjjxzip.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2mhfrfdgf.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2vrxclmag.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2pugcvpwf.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2lmkzqefw.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2jizzxity.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2rswxxddd.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2ujguxfkx.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2xviothhx.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2auueeyju.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2hbuhmdkm.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2gbgpejcd.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2kvdsrukw.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2zhppwehq.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2aukwcnbb.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jjaakvsb.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2xivfywyv.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2fbwpmcxm.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2xgnpgpzo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2lycdvcts.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2fzzrelvi.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2gwftogwb.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2yhfxkwwm.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2sapqqmyj.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2beyuxhmm.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2xxstuker.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2bwudggqp.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2gagesnss.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2rcwctgag.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2obigpgpo.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rrayopsx.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2uprsrats.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2nfgtogjn.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2zeskzunv.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hwnkvhdb.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2fkxfpvod.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2djljbzdq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2leqszvsf.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wyieuhrm.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2dhzfrbqx.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2emrpuujb.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmemefiw.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2tffpfhrx.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wukstmbn.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2qqtjcmue.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dlkvazba.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2vbcvskqf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2fueamnfu.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2yccsijhr.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2fodxhjux.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2yfylyoru.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2sctcfezo.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gvlykffk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2bfsyyebw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2behnbgsh.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2icbxvjah.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2crmmcqux.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2mawmykhu.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2algddqcg.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2irsnwslt.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2jahzykzn.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2oxjigszj.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cvtbbxku.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2dkglkaoy.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2oddeoxpd.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2enbniioi.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2oybbooge.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2oabthwgn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2mtqubvqk.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2iryebxat.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2lnohvojw.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2kofnalov.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2toszzhgy.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2zyjgxixw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2oporhfyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2etpchyuj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2jhpqdeve.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xgfnnced.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2dvqwnoat.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2rvyoeeeu.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2tuhcigxd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nofurdka.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ejpvuskb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2tcpgofry.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2dmnhragv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ifvzgxyt.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2sjebsiyu.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2qtrnpvvf.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2tcdyusmm.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2zmnlwdwv.html


<!-- 参考信息 -->