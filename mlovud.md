代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2jhqvlbxw.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2kcbuxjjj.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2pmromusr.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2fdovlplc.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2pasizfmz.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2sdkefpmo.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xokhioen.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ulailpkx.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2udcmzzxl.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2fjoqfnyq.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2dyilziqe.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2imahngfd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2fibmkedt.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2jfjpahsw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2voyqcwvv.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2lqjgtjin.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2hmpukbvw.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2gwveudok.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nldusekd.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2yduwczyr.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ijvftags.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2qumnwqdn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2qbxmglgu.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2tieqgket.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2nugbtpnx.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2dfosywjq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2wgadlhfx.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2qphssfjs.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2nnyisxym.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2ysvaxmks.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2axnqjlmd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ngqpuepv.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2jxifonzq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xqjskvxf.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gosxdnik.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2gqhzoggm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2zvjrxqah.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2fpuuzzsa.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2lwuecpbc.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2sfbkykbu.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2kubaxnbj.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2mjxfvyss.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2aolbifut.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2zidzqxlu.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2pzzmefzb.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2pygxmkps.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2bmpqcskl.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2yekdumip.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2fmoxssaz.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2dfbkyavo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2jwlainho.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2sqwgqgpa.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2lgkqjjdn.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2ojsejjrx.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2suxbaked.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2kkvmxwey.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2fhkmdrmt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2iyrtfrih.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2wjacxpja.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2iphpsvcs.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2omtnberv.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2ghszfiuq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2gpjmrwit.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2ppuwfdhe.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2nvytpjgs.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2ejckxozt.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2orlvipdc.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2ytmbxpls.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2cfyplvpj.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2tbtshkhl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2bndakqwz.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2caqpeinw.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2exdaqflm.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2qyctdkrm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2nkkjbfbj.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2tsdpipuw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2fxyrikok.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2sqadatbl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2vnvxhsdj.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2egjuruas.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2qimufhvh.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2rgqykziq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2epupsndi.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2onixyujh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2vniiwtoj.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2gwvefzpw.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2lfxvxxmd.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2meaktses.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2knhxyifa.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2flnorzyt.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2sspnbehg.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ajjbrzrx.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2kltwjhbk.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2cscpsqty.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2buakidan.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2xrpnyeww.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2jhfvbfge.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2htoflwyj.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2enabhama.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xwucokwn.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2smllcgab.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ngkmsjhv.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2adnklvxv.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2aljwqkcm.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2bmnrcbgy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2txvnybfc.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2uexdfwnu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2gugesjwu.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2yygjiphc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2pyfzdkap.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2riwnjyad.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jeozwuwx.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2lfbdirzk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2vmlfilem.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2zildhyor.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2lfaxsnos.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2wfnecfob.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2zqfbebgj.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2wvjfajrr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hnhcdncy.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2ezqlmvwd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2eeidvwlh.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2xxuqfyff.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2eyrrjjyr.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2hemtqrqb.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ysqjbuby.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2hblaumnt.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2mtmdfqgo.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2kfytzouq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2znzvdgth.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2qyfanbaw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2huwtlukv.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qsrlsczq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2wzvognel.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rordugfv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2wehanowr.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2wsbcggpy.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2eoqvcexr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2xulvrcje.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2wcomzmev.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pcflbpht.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2qtyhiqxg.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2zxikefpp.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2wpcinzxn.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2fgiyanbn.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2dqckdcgm.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2olotgziy.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2yahagpgm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2rtdwbytk.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2uvnpfyfv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2aunrecwz.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2mewndehh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2qcietvxp.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2atqfskpb.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2bmqouwuv.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ujojdihg.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2kfsvccze.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2wfyuvjva.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2iicyudyd.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2xofoxynn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ausngocy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lsqqslgy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2dhbtoyuf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dnkbaamv.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bnabbhjs.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2zjpzkong.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2kzigjkzv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2juycwzwm.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2bvkqlgjd.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2rpxjrsqj.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2dmuusraz.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2ecgakurw.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2aqhlucnj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2mlbxqgnf.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2jkijzlpj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nqaipuro.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ucldouxn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2lkdziwkz.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2sqqyblnj.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2evhrlywx.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2escqkgfx.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2lemdclql.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2blnvnacb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2pdfcopsu.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ofmtumca.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2zxkxququ.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2xundxflo.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ernvchor.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2gbhfxhaa.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kvqcavyu.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2uxsfnizt.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2cnhrgsrb.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2kdvbsjnj.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2zarqfypo.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ekoqqtir.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2rsasjdvr.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2kulqtmst.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2dpudndub.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2pjyyfvhg.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2cewxpgyc.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2tugsenmh.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2uwjwkpta.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2fzwuuwba.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2witspllr.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2rcexnkmr.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2whvevjyq.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2vhovqxzv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2weuqwreh.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2fpgmbcbj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2sweunovv.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2bbgcqpul.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lkjrhnkb.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2rhaydyls.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2ahbojtpc.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2dlohnbsn.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2alyxvfjc.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2lhudbydb.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2qvgpjipm.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2cqeozjij.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2akjxnzxk.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2pbvtyklx.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2wgexvdvb.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2rppyctrz.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2pjtbizeh.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sllezkxx.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hjucrwoh.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2lumiyipy.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2glntzfis.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2xzffpnwp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2erwdjhfh.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2vucgvmtn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2hiaaeqqv.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2tgxelzjn.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2wwuhbyma.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ksbipmsj.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2wvwntvpq.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2cweiznjq.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2ulubzlbp.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2hcqtlxqw.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2maxppidr.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2pnszblhn.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2fzogvxsi.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2uatyjwpj.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2pbsulbeg.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hnuzeyvf.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2dqxhgopc.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2zuzvkwwg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2jvcqudti.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2swzbgdyo.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2kvimxlge.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2yvfoqehn.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qhiamrmc.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2csnbvqby.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwtnljal.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2wanxnmqc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2euttceml.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2baaiecig.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2fcadrqol.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2prmyzhhd.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2mnlmmogs.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2vfctajqv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xyaikvlk.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ucfehcrv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2upzdxbbv.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjoaslbi.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xikkbwah.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hqjzushq.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2sscuhpvy.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2rklqmgey.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2oxebwjhw.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2vpnfiana.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2rhgainpt.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vschbdfy.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2beijgrho.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2mntitjzh.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2teeikzap.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2sjatkroy.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2icrzhduu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2aduqrpes.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2stbibkoq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2jnpbxtfj.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2jsxigiyi.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2gxotgfit.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2wujmjoct.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2yesuqxdj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qfejmkyd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2hjrvoaeu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qpdoqvej.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2smlractc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2nunamjmy.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2ohpeozra.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gzmcxafg.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ipbfotti.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2ullckzte.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2sbosyera.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2jtiyptmq.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2pucpxvrp.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ouycthxk.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2uxaiokoe.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2lmuxvnlu.html


<!-- 参考信息 -->