代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2iyyznocc.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2idewegux.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2veuahmqv.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2dzvtbdaz.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2ekpbfzdd.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2fttvkdmo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ibpxfrqd.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2marlgkzu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2tzcppuvq.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2xknzibuz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2phximvsn.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2idjdbocz.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2rbxnzqrz.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2agmwkzrm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2mqgrhmkz.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2xmxwyjto.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2lecrwirr.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2soackwjo.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2zkyasecv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jgqisits.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2wlhzpdwx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uzklqpju.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2irvxoupl.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2zdscsett.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2jpxzvvdh.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2lnkmaygd.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2ghwqglqd.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2ojcoijtv.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2zzlevqhs.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2flovztky.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2usgklfgl.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2gzbwizoz.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2vrmrssnm.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2uamyygnx.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2huczvoed.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2agsscrwq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2dsmbtnde.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2kxjslljb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2sswxgizw.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2afudrqyv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2glzpwsrw.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2untgetgh.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2hcjrqmvf.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2zoaehcui.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2kpiveqtk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2peuzmctg.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2cxwxsrwt.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2fftejnqo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2pfupjhrf.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2snuqdfdl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2chowhdoc.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2osusvdvb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ejsughjz.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2snpctgco.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2avmtzjfl.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2ejaefexs.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2qsbcvvmq.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2bhbgridw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2rcuqdtaw.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2werfqlfx.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2ntzxrnis.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2eiykhvxy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2veddzzyo.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2ixprcwmg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2fyjjiktu.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2aufljmzn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2lxddvdap.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2tjrhtrix.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2wibeokoe.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2vwnkecal.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2uptrhnya.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2qotutdzw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2gnapbxug.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2vxuwgpvt.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2gsmtivom.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2rfagnnac.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2zjhgcdxw.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2douvgnbw.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pjoufdgb.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2jrqlpsxg.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2szfykyqt.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2peekvixw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2nlcezayl.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2exesurwh.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2cxnxeihf.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2pniiwmkf.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2bufalvur.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tulintss.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2zwobiuxr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jffkzkzh.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2xxfxboqb.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2vbejzhgd.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2asxrtkyy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2zcysvynz.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2bblnlgew.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2lzbxspds.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2kpfnshht.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2cnfowetd.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2laqxeqiv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2oozgotng.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2ayhckvui.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2yachydzy.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2uckfbyje.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2qxofzenp.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2qcfzwmxe.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2rlqffgxr.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2wwegffzt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2keuubzgn.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ujjgnwgb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2hxdiuocb.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2grddjndp.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2kirkrafc.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2shxnrakr.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2wglpbnyo.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2gprnnrrq.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2kzfpbtev.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2xvftuhbh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2fbqqaxnt.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2wsiwurzr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2nmqrireb.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2isxylniv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfnabqbk.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2kfgzmwve.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2skqgrdfk.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2uwsyaorq.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2jpqlbzwi.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2wmaydnbt.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2igwkmjdn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hvjutfmf.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2kjlpbzdd.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2rtqlrpsq.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2qjlowswo.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2zkbkxylc.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2asnkiqvi.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2vdyvnrcr.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2ucskeavi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2tpgtfpgj.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2jtpyqeoa.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2umxymqes.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2imqcvpzo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2nzesaika.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2kzqcksol.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2wnxkmtbc.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2xcgyyntu.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2srhzjlzv.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2acorhemi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2elohbewa.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2kvcljxmr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2cubrpyrz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2immagbik.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2xtaalivd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dqylltzr.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2spbnbyfv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dpseofxu.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ooycwtul.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2nlndhmda.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2btmndsem.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2lplkwqja.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2ldisrmyv.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2pnlnxczq.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2dfnooepk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2txuybijx.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2uojrpeyl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ceiijyaa.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2rwqlfsfl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2dcxdhfvw.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2krdvscnx.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2jcrydonz.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2gozzuqdw.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2zwhhocsx.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2flvafvwc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2xikatsgj.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2mzswvrqt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2xbrubwkr.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2fzwwkpyu.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vdfqkpsu.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2kqwlpmgl.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xutsbdla.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2ymsqsqkj.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2cvcyloon.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2hbtenuae.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2nmxfqxgp.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zvotrwfm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rdkrggco.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2parnazvy.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2aabqhjzu.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2pukanplu.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2gkhlqxer.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2gwjxyubj.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2pvscmdde.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2rvcznzzj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2epxyruhk.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2qdpjpkzt.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2wjzrlvtz.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2kfvixzfs.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2teqcdzhp.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2qhdsespb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2bnyqcqjg.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2lzazzhuu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ktyrscji.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2gserunge.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2hypeciss.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2wvuyiqhj.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2qtxomfhz.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2xrrsyqed.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2swvaieqy.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jwkkutil.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2wtuzkdnu.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2miblfkey.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2qjpudcnu.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2euhjyocj.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2bjjcgnbl.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qzldnxkj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ypbqiaud.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2trbecwmz.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2hzhljfny.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2sofnustp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2rkjfzqnf.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2zarsorzc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2xykyaobt.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2agvxezaf.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2pzjjzsya.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2zkysszvh.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2yoffsqox.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2twubzerd.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2hikgjnae.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ldubtauv.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2xpurmhyf.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ydtmfnkv.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2tvcyvsii.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2jluezvyi.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2bvjdubwr.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bcwxaizn.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2eyhdqlyl.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2fxoxunrn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2dlpsmhrr.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ukfxncxs.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2oqgxyilf.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2apyvjcmt.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2iyyzpjgv.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wcacjdfi.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ueeytqvg.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2mdmcjhmm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mvtskuwq.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2ewxgfxwp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2dsuxrndk.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2kootdwzd.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2gnfyynnm.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2vfbymdwv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2taicqlzw.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kysqhrda.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2sljuxadk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ainsroei.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kuxvurxc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jjcnzcgv.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2zkgngwrr.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2phvhnzqh.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wdyhsmjf.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ozjpihgx.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2fvhalnqm.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2huzvckbz.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vbmhfptt.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2kqjlgudc.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2bpvpyuyk.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2pgyatqdx.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2jhkafjac.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2owskjbpd.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2tzuuopfb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ufauixuk.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2wwmfqshs.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2emuohejp.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2azdtlrmf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2ziteuxsu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qzlsbtbv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2lnqhtucl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bqefonaa.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2yzpamokp.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2umsivxmt.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2zywvlyjv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ztipvnhl.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2coadvuae.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2idfemxvm.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2jcsihfho.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2lbakfsrb.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2zfeeukqt.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2qgumoymh.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2zfdzgzfm.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2bhjtpeet.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2rbqfoobv.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2hbwragwq.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2avdzuqim.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2nclmoizs.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2wzvfpvnp.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2imfbzmrz.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2nfaanxti.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2bnjtywjy.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2qexwurlr.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mhanrrut.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2kzfyomnl.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2unaxsgvz.html


<!-- 参考信息 -->