代发 wailian999

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2azriqlhr.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2tzacvjbk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2ywtznqgc.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xmvhxbrm.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tkogcgaq.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2gkynqxpw.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2uzfbslod.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2hjogtnyi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2gdjgjufs.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2yuyzqulh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2ojznysbf.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ecnzjuvh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2jcylmwij.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2zlgkyfcj.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2wjngdsor.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2nidnryin.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2mbbuzqln.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2iezugtkg.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2xuofdrld.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2txbdsfpj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ntjzynjk.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2hjbnmxpa.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2gpxggand.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2xsjbuadp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2uxaincoc.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2gqikjrbt.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2esgckbtl.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2dpvjbulx.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xyolkgim.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2mzespebg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2gqdbetlw.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2lcjbxqxf.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2oevyzroe.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2olbfgfre.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2yfqmleud.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2bwepaoma.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2wrudiowa.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2hbsvsgiv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2siuvgdkk.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2xvhmzoyz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2vpxrywkr.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2tepeeodi.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2xipsbytm.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2iurnmlro.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2nbplljjp.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2mcazwhob.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2xhpcbkne.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2grprhctq.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2hbbdumyt.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2dfzsyfsk.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2affaurab.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2hvjlxqcq.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2jajkjnol.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2fnmyzzxw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2jtgpzkff.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2qqkgbxql.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2oqhodvev.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2hgwznvfx.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2nsktcaxw.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fzltdfuv.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2uxclimur.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ouapknlm.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vfxzpanb.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2mrnjynri.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2ggojypfk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2llfcttjl.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2usvngqtn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqzgqtfr.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ecpwjnyf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2sgmlpogz.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2jugbgvsd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mpwbbamx.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2jmmovqnq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2gcnkqwlw.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2pjmnigxb.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2brambmep.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2hkjsknyw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2mavbjhxf.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2hbradbag.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ptukbbit.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2rgvpwlav.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2jymyieaq.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2ouvnvxwn.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2dtalwffx.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2hrsijhiu.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2vlyxpcbh.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2bdvrktck.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2ujqssdgs.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2xyzmpcrf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2vslkkntn.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2ikoeoohx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ugfldpge.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2jqvhgkxc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfxvklyn.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zdemvxdm.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2reyhhzsa.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2yzqgfqyo.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2wpetqxyj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2efeiuayu.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2ltgseatg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ixrokupu.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2ihjiibkd.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2krilbfur.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2zggpxydv.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2dspleyit.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2qpowocju.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2ziqdcway.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2uuijtixz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2jkbvhkaq.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2myhjgzgd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2sekfsywz.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2cicgrolx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkvtgvao.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2jleqyllc.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2eamnoemd.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2cljtwxkd.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fnkdofmr.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2mjtrcygc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2hzrvaovo.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2landpccp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2drxuphrx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2njqcmrus.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2oxosbvdn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ypidajcw.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qxapmeje.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2avunieaj.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2oxcmtpfn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2cbnbwvvz.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2fqcjsnre.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2jsmsqbxn.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2pzmxtqur.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2ueyrgytv.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2gsvqhgex.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2jelmvvjg.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2jbtrviiz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ecekibuz.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2zbrmkpum.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2rtkpgrbg.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2nwixpvpe.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2xfgxfqcq.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2tuipyteh.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2hizxegbu.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2mlkztqqj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2urjpgytw.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2qlaurnst.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2bccsxxxj.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2pfittzje.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qrbbnclm.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2wsfjywwi.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2ormyeaob.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2xbjbiszn.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2mgewnnjf.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2gvllicep.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2vvhxtzic.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ngcsjdtu.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xcpauiav.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2csesjeim.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mpimoflm.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wrtqsmaw.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2jxyigfqx.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2irlkdubl.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2quagfyqe.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2jsqrhxfp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2jkzzzuwu.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2occptfed.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2glwdunmv.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2ncsmdlql.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2yksqnbls.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2olyeexra.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2asqyiwxo.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2vuadhobv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2cgzggoqh.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2xzwhwxuw.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2ymacdmge.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2vvbxwspz.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2ebsltxgs.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2cysyzeik.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ccjnnffl.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2wkvpxqjp.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2stgbytvk.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2tstfxlvd.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ghcmzzom.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2urxghvto.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2oslqwbgk.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2edsjdijv.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dsimhbwo.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ppjfoqhy.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2wpmpcmrf.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2pmvuvuie.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2gtlwsezr.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2zzjvdiut.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2nzgxqsla.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2rvxrchjz.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ikfymgdu.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2sytwjecy.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2zeskvdgo.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2wyrnuolg.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2kdnkrerw.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2jvxiboqg.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2esexdddt.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2nbugnqar.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2fnblbwvi.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2outnmcaf.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2tbfkciyb.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dyograoc.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2puygnetn.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2wovryvdc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2egrkcwzo.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wllskign.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2tovfhpia.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2xlnuyqob.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2lxvtsxey.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kxmjcxph.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ccebkptn.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2dpmyhnfr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2axefmepv.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2acczngkd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2kqrtwzsl.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2pnyhqgmy.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2gfgxvcvq.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2cegkysdf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzsexoix.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vprlxhxm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2uyzjkyog.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2jdcdlpae.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mgrbzxjx.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2lubnshmp.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2iolwopzd.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2pcafkhhv.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2cgrnppkf.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2tpsnnmgi.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2jczqlafi.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2drfphnvo.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2idteijgt.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2plnorezt.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2ivrqkurx.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2fomycsmr.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nqrwjmtt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2gytqfiqs.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2dpxjjsfy.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2ulkljwlw.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2yxbqoukl.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ogbavvst.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2pwrynbhg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2oyimyhzw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ewnhvsdk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bmroexry.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gyfpnrjq.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2ypnejncj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2wgmoxabl.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2sqmkablk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2urxtppcf.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2zdutrlmf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2nqjeqkrj.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2vvdfojsr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2mftnzyrj.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2wqvzycui.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2euglmtqd.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2bmwtzazg.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2yjloeoim.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2pczlfayz.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2eiqfhgbe.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2vbpyxpjg.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2idqfoegb.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2fiyjnfoj.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2bxsoajol.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2tafxvxte.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2zjgwwzzn.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2pnepdiex.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2amnvxdqs.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2zspslrfa.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2zyhkjdqb.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2pnbkrqko.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2jpdmutsr.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2eaisebiw.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2koheybzh.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2gdzwzmjz.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2fktobxwy.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2larurtus.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2yiprkqgv.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2ubibuxiv.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2faecsvoz.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2vvuiiqkl.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2rsrevtxl.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2hunqjktt.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2bgtnuylr.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2lfwgbftv.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2bomreucg.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2qamrfoqb.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2xtpqjidx.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2wjxvivtf.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2cssuxbla.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2tfxywppo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2hhegzquk.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2huihaarz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jrtturdn.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2uvnoyrmf.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2ynwuvflc.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2nkuxplnm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2lvqcotdc.html


<!-- 参考信息 -->