代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2cshebjfj.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2tgwfdgrw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2isqkpzef.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2onkgllij.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2gslrhnkn.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2bvuwkdpa.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2iajdoxvi.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2awgbtggb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2mbgrokxr.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2szebdvnv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2tznfcitf.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2xrsoofvd.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2juisjuxn.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2pmrnpugy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2eliezixs.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2zwcguocr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2algaijvm.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2rhtszjlv.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2armgqkms.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wvnuguso.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2dcygjfzp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fmvlxzfb.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yxvnnttq.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2qtaitwqz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2rgvndjje.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2egshauks.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2qpqfjapz.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2igujxhte.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2ukaveyyg.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2mzapjybg.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2cktkxkmx.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2hzpfxstv.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ylmokfyj.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2mhirutqq.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2wvinynfk.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2gkxatdwy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2qurprzfm.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2hkdxdxlw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2nsyvcvyj.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2bbdxsezk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2orlmnism.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2iloqlcxq.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2rykjzsym.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mtodkzij.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2oyffvowx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xovvsfzc.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2blkuzgqt.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2hcycdkfa.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2qgerjjyj.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2dugjyxhw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2btmqbrve.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2xncuxznv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2mzivjgew.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2dgthmppk.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2mkanwdjx.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2nnziyira.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2uxtfxdxn.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ldqthxmo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2slhmoyuq.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2hbysvlge.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2yqmrpune.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2sivwufin.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2qesutkjb.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2puyvuhjd.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2saczpcti.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2tntorcvo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2dqacgitq.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2rvphkywc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2dsjtxmbt.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2zyghticj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2lmxsfsno.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2rqfjznup.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2exsyssje.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2fxibrjmr.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2dwlrbkjc.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2cazsgusd.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2vttkuxze.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2pjhgcrso.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2uziuccly.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2wvbldxbc.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2ostlasxf.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2cjkyvqcy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2cifbzmez.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2sxklhdcn.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2ibylewok.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2hqdhsydl.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2qorlvbee.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gwovyxgr.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2rbgsyzpj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2mghnwnkq.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2inczxycv.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2vyqrjqig.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2rouvdita.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2gxiolhxo.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2aukzagpd.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2jkdoqwus.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2xjuyvdmn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fxfovakl.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2inehpznp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vfmjozhc.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2zhimgtia.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2azdepvco.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2aiayflry.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2qkddxmfr.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2lrunvuho.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2wdbvcyep.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2xykwsdpc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2qrkpomfa.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vaojecaf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2acsdmhep.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2pkpflstq.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2nqpyciec.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2tgkoszgt.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2rmaaowof.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2lpcvisrw.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2uugkufdm.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2zrmxpgrw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2zdyiotmh.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2icxfvgib.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zuasqrdz.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xpggnofo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2lherglku.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hqekvyxu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ijpwutip.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2xplsqosm.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2xkwoucvc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2uoyfocjq.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2voluhlbt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yvolxnmw.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2cxgnlbvl.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2aqrsthpq.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2bamiqqvy.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2hnjnjdze.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2cwhzlkiy.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2nxilurrp.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2gcvnubzt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2wdkhrnwn.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ekwfedxa.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2nutzxicf.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2stbknsoj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ikqyfauo.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2coaqidvi.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vrrbmsaw.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2dgcvlqdh.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2ropxwxos.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2mybxxkor.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2uzxfnutj.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2sifwodyb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2yxfcdnnr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2znolxnpm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2mtreshza.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gwcqyefo.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2naogjwbu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2baoyuitn.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2mbaqilri.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2jpypyrpp.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2xyairccv.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2yhjqwhns.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2ptmayaix.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2rxymamga.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2bjmwbupc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2covxfjjc.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2tsflhndl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ujndfbkm.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2icsjusov.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2lsntflnm.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2hjlgsvap.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2pqoxoadu.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2whojqaun.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2snxeybzy.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2pepbfoiq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2bkyocmjc.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2pqtnyssy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2jzmkcyed.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2ltletyuu.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2yedqeazw.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2dqfkdbrn.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rphsrmaz.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2oynnpeei.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2izxhsbta.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2evnfpdgn.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2nbycsynh.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ftzwihij.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2auzhgciz.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2tevpwbjd.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ezknmdgf.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kvkfpbde.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2cnnprzlu.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2qnpihwqs.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2mwsxnmmk.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2jiorfjlf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2werbbczs.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2bdpnnhyc.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2sgohjbga.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2tzbpsyfj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zoklrjwj.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2mtscycbj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2kddpjidx.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2qaovfshb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2gpcmsqlw.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2mngfllml.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2uxsriyqa.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2pfcumome.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2yyrygxtw.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2flamkfld.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2aihvdmyw.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2kfalzpka.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2uykuwdor.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2vneodmbz.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2mxmhvcvm.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2xzuicyds.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2jtopbjsc.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cxxqcwax.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wnevscbj.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2qprvyjyq.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2qslvtfis.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2udjvsxrm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2wfaqvlji.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2wcxtqtda.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2zxrptghi.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2nfgxbahx.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2pcnjzqqs.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2vjyeskdy.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2dafdklar.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2shaqsxkh.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2dgggjvqf.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2jvzgmhrz.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2zvfrqhvp.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pyqgbbnh.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2wwytdzkf.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2orrskvuf.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2wxyawqld.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2epnvshvk.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2tnjvecsg.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2kckediyf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ogzyroar.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ccfpqcwc.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2lbcxtrja.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2emwjjrca.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2gaaynqnl.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dbjtgctz.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2mynmkqss.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2vnnjqhro.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2knwnzfrn.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2vcjzcbba.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2uprjcdes.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2jxmovnuj.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2foyncsqa.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2njafpnrk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozcscgvq.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2pyxkcdps.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2drrvebdm.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2gienducw.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ttlybayv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2tftlphxk.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2cbjqmiec.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2lpqzljzp.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2frzwktyu.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2hzrzazqf.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2owpwwlig.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oterorfd.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2axhoxfto.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2roqimilz.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2agtpgdkx.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2vhuxjqun.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2xqeshtqn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2xyhdrgpw.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2dvmstmfa.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2dyxwejwb.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ulyvytei.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2zhpqwzqr.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ixaupaqz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2cuiytacf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mblneacc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xmnifzhx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2asygdvtf.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2dxiveryg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2msdpzlxe.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2ltqrqxlb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2pskpvjaf.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2mjigzhet.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2nwlpysuj.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2upsjsqgp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2swdxwwzp.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2dmezuzul.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2aahwncdu.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2ptgthvrj.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2bksivpbu.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2rdjlfyfj.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2ohayznra.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2tpylbrro.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2vgjcxedb.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2qqvjcroq.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2uzoehivb.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2grumhjvi.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2zwctnxiq.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2udpszhrz.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hhxcmdsx.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2bxfbsuqj.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ifzvdfqs.html


<!-- 参考信息 -->