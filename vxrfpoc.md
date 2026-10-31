代发 wailian999

S. C / C++ 专题
来源：http://ri.szsharing.cn

================================================================================
来源：http://zs.wgjwhj.cn

[S01] C：Hello World
来源：http://uk.newstarts.cn

#include <stdio.h>
来源：http://tv.huixiangedu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://io.bjjhwx.cn

[S02] C：变量与格式化输出
来源：http://bk.asd995.cn

int a = 10; printf("%d\n", a);
来源：http://pn.huixinmuqiang.cn

[S03] C：读入整数
来源：http://yf.lnxyls.cn

int x; scanf("%d", &x);
来源：http://tq.wgjwhj.cn

[S04] C：字符串复制
来源：http://nu.yuexingan06.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ke.yuntaijiaju.cn

[S05] C：字符串长度
来源：http://xd.bookmarksfly.cn

strlen(s)
来源：http://gt.nicolike.cn

[S06] C：字符串比较
来源：http://hi.haigaiapp.cn

strcmp(a, b) == 0
来源：http://vp.nicolike.cn

[S07] C：数组遍历求和
来源：http://xk.gzmigu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fg.huanxung.cn

[S08] C：动态内存分配与释放
来源：http://fp.bookmarksfly.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gb.jianghongdianzi.cn

[S09] C：结构体定义与初始化
来源：http://bv.asd995.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mi.nicolike.cn

[S10] C：指针与解引用
来源：http://vl.muxihuayi.cn

int *p = &a;  *p = 5;
来源：http://xh.huanxung.cn

[S11] C：逐行读文件
来源：http://re.huixinmuqiang.cn

FILE *f = fopen("a.txt", "r");
来源：http://ot.nszjky.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://is.colortex.cn

fclose(f);
来源：http://bv.chemitech.net.cn

[S12] C：写文件
来源：http://vu.521024.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hg.yuntaijiaju.cn

[S13] C：宏定义
来源：http://ao.bjjhwx.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uk.panjiajie.cn

[S14] C：枚举
来源：http://if.colortex.cn

enum Color { RED, GREEN, BLUE };
来源：http://mt.hnjuh.cn

[S15] C：类型转换
来源：http://dg.szsharing.cn

(double) a / b
来源：http://vi.shxzskj.cn

[S16] C：位操作置位
来源：http://cw.panjiajie.cn

x |= (1 << 3);
来源：http://we.chemitech.net.cn

[S17] C：安全拼接字符串
来源：http://mi.huixinmuqiang.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ym.jianghongdianzi.cn

[S18] C：命令行参数
来源：http://ya.huixiangedu.cn

int main(int argc, char **argv)
来源：http://oz.shtwfgs.cn

[S19] C：快速排序
来源：http://cd.nszjky.cn

qsort(a, n, sizeof(int), cmp);
来源：http://bo.shxzskj.cn

[S20] C：二分查找
来源：http://gm.lnxyls.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yd.shxzskj.cn

[S21] C：字符类别判断
来源：http://db.asd995.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lu.nicolike.cn

[S22] C：字符串转数字
来源：http://ij.shxzukj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://hs.shxzukj.cn

[S23] C：随机数
来源：http://ee.nicolike.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vl.bookmarksfly.cn

[S24] C：获取本地时间
来源：http://in.wgjwhj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sj.panjiajie.cn

[S25] C：内存拷贝
来源：http://xv.huanxung.cn

memcpy(dst, src, n);
来源：http://pk.asd995.cn

[S26] C：内存清零
来源：http://hx.szxytkj.cn

memset(a, 0, sizeof a);
来源：http://qt.9csxet.cn

[S27] C：定义常量
来源：http://zy.yuexingan06.cn

const double PI = 3.14159;
来源：http://je.nszjky.cn

[S28] C：静态变量
来源：http://qn.bookmarksfly.cn

static int counter = 0;
来源：http://pf.yuexingan06.cn

[S29] C：变参函数
来源：http://kh.gzmigu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zy.wgjwhj.cn

[S30] C：头文件保护
来源：http://jj.muxihuayi.cn

#ifndef X_H
来源：http://jk.521024.cn

#define X_H
来源：http://eg.521024.cn

#endif
来源：http://ps.haigaiapp.cn

[S31] C++：Hello World
来源：http://vl.jianghongdianzi.cn

#include <iostream>
来源：http://cd.jctech888.com.cn

int main() { std::cout << "Hello\n"; }
来源：http://dh.9csxet.cn

[S32] C++：字符串
来源：http://vp.szxytkj.cn

std::string s = "hi";  s += "!";
来源：http://rx.bookmarksfly.cn

[S33] C++：vector 增删
来源：http://hq.9csxet.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yc.gzmigu.cn

[S34] C++：遍历 vector
来源：http://rq.bookmarksfly.cn

for (auto &x : v) { std::cout << x; }
来源：http://vn.yuntaijiaju.cn

[S35] C++：map
来源：http://ms.chemitech.net.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://od.nszjky.cn

[S36] C++：unordered_map
来源：http://jh.521024.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bu.muxihuayi.cn

[S37] C++：set
来源：http://mm.9csxet.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xf.bjjhwx.cn

[S38] C++：排序
来源：http://oh.huixiangedu.cn

std::sort(v.begin(), v.end());
来源：http://pp.chemitech.net.cn

[S39] C++：自定义比较器排序
来源：http://yx.hahajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ua.huixiangedu.cn

[S40] C++：查找元素
来源：http://xl.szxytkj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hq.szxytkj.cn

[S41] C++：类与构造函数
来源：http://bx.szxytkj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qp.bookmarksfly.cn

[S42] C++：继承与虚函数
来源：http://nn.bjjhwx.cn

class B : public Base { public: void f() override {} };
来源：http://va.haigaiapp.cn

[S43] C++：智能指针
来源：http://yu.szxytkj.cn

auto p = std::make_unique<int>(5);
来源：http://up.jctech888.com.cn

[S44] C++：引用传参
来源：http://wn.huixinmuqiang.cn

void inc(int &x) { ++x; }
来源：http://kr.huixiangedu.cn

[S45] C++：lambda
来源：http://hq.yuntaijiaju.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zp.szxytkj.cn

[S46] C++：函数模板
来源：http://ek.shxzukj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wd.muxihuayi.cn

[S47] C++：结构化绑定遍历
来源：http://vn.muxihuayi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uu.chemitech.net.cn

[S48] C++：逐行读文件
来源：http://xs.jianghongdianzi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://eo.panjiajie.cn

while (std::getline(in, line)) { }
来源：http://pj.jianghongdianzi.cn

[S49] C++：写文件
来源：http://kk.chemitech.net.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ym.gzmigu.cn

[S50] C++：格式化数字
来源：http://xq.colortex.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mo.521024.cn

[S51] C++：显式类型转换
来源：http://vm.haigaiapp.cn

static_cast<double>(a) / b
来源：http://wx.jianghongdianzi.cn

[S52] C++：const 与 noexcept
来源：http://pm.hahajie.cn

int size() const noexcept { return n_; }
来源：http://pg.muxihuayi.cn

[S53] C++：移动语义
来源：http://ef.jctech888.com.cn

std::vector<int> w = std::move(v);
来源：http://rj.yuntaijiaju.cn

[S54] C++：异常处理
来源：http://hq.shxzskj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gg.hnjuh.cn

[S55] C++：结构化绑定
来源：http://ag.nszjky.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://al.huixiangedu.cn

[S56] C++：optional
来源：http://bz.szxytkj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ni.9csxet.cn

[S57] C++：编译期常量
来源：http://nc.szsharing.cn

constexpr int N = 10;
来源：http://gh.jctech888.com.cn

[S58] C++：命名空间
来源：http://in.shxzukj.cn

namespace ns { int f() { return 1; } }
来源：http://rm.haigaiapp.cn

[S59] C++：静态断言
来源：http://eh.szxytkj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vv.yuntaijiaju.cn

[S60] C++：遍历并删除元素
来源：http://hi.yuntaijiaju.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dw.lnxyls.cn

================================================================================
来源：http://oo.szxytkj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ww.wgjwhj.cn

================================================================================
来源：http://uc.521024.cn

[T01] Kotlin：Hello World
来源：http://qs.newstarts.cn

println("Hello")
来源：http://pf.asd995.cn

[T02] Kotlin：变量
来源：http://wb.bookmarksfly.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bs.chemitech.net.cn

[T03] Kotlin：字符串模板
来源：http://oc.shxzukj.cn

"值: $b"
来源：http://wz.yuntaijiaju.cn

[T04] Kotlin：空安全
来源：http://td.huixinmuqiang.cn

val n: String? = null;  n?.length
来源：http://sb.yuexingan06.cn

[T05] Kotlin：when 表达式
来源：http://uf.huanxung.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jn.haigaiapp.cn

[T06] Kotlin：集合映射
来源：http://od.hnjuh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://dq.chemitech.net.cn

[T07] Kotlin：集合过滤
来源：http://tw.jianghongdianzi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://cw.szsharing.cn

[T08] Kotlin：数据类
来源：http://qu.huixiangedu.cn

data class User(val name: String, val age: Int)
来源：http://je.chemitech.net.cn

[T09] Kotlin：扩展函数
来源：http://yj.muxihuayi.cn

fun String.exclaim() = this + "!"
来源：http://cr.bookmarksfly.cn

[T10] Kotlin：默认参数
来源：http://tn.chemitech.net.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tp.huixinmuqiang.cn

[T11] Kotlin：协程
来源：http://ve.muxihuayi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://pd.lnxyls.cn

[T12] Kotlin：解构声明
来源：http://da.9csxet.cn

val (a, b) = Pair(1, 2)
来源：http://nt.huixinmuqiang.cn

[T13] Kotlin：只读 Map
来源：http://li.newstarts.cn

val m = mapOf("a" to 1)
来源：http://cj.jianghongdianzi.cn

[T14] Kotlin：循环
来源：http://wf.bjjhwx.cn

for (i in 1..10) println(i)
来源：http://lm.panjiajie.cn

[T15] Kotlin：接口
来源：http://wv.asd995.cn

interface Shape { fun area(): Double }
来源：http://dp.wgjwhj.cn

[T16] Swift：Hello World
来源：http://ug.nicolike.cn

print("Hello")
来源：http://iu.huanxung.cn

[T17] Swift：变量与常量
来源：http://gn.haigaiapp.cn

var a = 1;  let b = 2
来源：http://sv.huixinmuqiang.cn

[T18] Swift：字符串插值
来源：http://uy.szxytkj.cn

"值: \(b)"
来源：http://eq.jianghongdianzi.cn

[T19] Swift：可选绑定
来源：http://id.jianghongdianzi.cn

if let n = opt { print(n) }
来源：http://vh.nszjky.cn

[T20] Swift：数组操作
来源：http://ae.jctech888.com.cn

var a = [1, 2, 3];  a.append(4)
来源：http://pa.huixiangedu.cn

[T21] Swift：遍历
来源：http://og.bookmarksfly.cn

for x in a { print(x) }
来源：http://oc.jianghongdianzi.cn

[T22] Swift：字典
来源：http://pn.newstarts.cn

var d = ["a": 1];  d["b"] = 2
来源：http://sn.chemitech.net.cn

[T23] Swift：函数
来源：http://fv.huixiangedu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ng.szsharing.cn

[T24] Swift：闭包
来源：http://mb.muxihuayi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://pr.gzmigu.cn

[T25] Swift：结构体
来源：http://fh.huanxung.cn

struct P { var x: Int }
来源：http://vi.jctech888.com.cn

[T26] Swift：类与重写
来源：http://me.panjiajie.cn

class A: Base { override func f() {} }
来源：http://ic.bjjhwx.cn

[T27] Swift：错误处理
来源：http://lp.huanxung.cn

do { try f() } catch { print(error) }
来源：http://qe.hnjuh.cn

[T28] Swift：枚举
来源：http://kg.hnjuh.cn

enum Color { case red, green }
来源：http://lq.9csxet.cn

[T29] Swift：guard 提前返回
来源：http://uh.szsharing.cn

guard let x = opt else { return }
来源：http://zu.hahajie.cn

[T30] Swift：协议
来源：http://lj.bookmarksfly.cn

protocol Shape { func area() -> Double }
来源：http://hy.chemitech.net.cn

[T31] Lua：Hello World
来源：http://oq.huixiangedu.cn

print("Hello")
来源：http://zy.521024.cn

[T32] Lua：局部变量
来源：http://ka.hnjuh.cn

local a = 1
来源：http://vm.gzmigu.cn

[T33] Lua：表（数组）
来源：http://nt.yuexingan06.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://as.gzmigu.cn

[T34] Lua：遍历表
来源：http://ls.colortex.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://om.colortex.cn

[T35] Lua：字典表
来源：http://ee.colortex.cn

local d = { a = 1 };  d.b = 2
来源：http://lz.jianghongdianzi.cn

[T36] Lua：函数
来源：http://de.lnxyls.cn

function add(a, b) return a + b end
来源：http://fw.9csxet.cn

[T37] Lua：字符串拼接
来源：http://wr.shxzskj.cn

"a" .. "b"
来源：http://rf.yuexingan06.cn

[T38] Lua：条件
来源：http://az.bookmarksfly.cn

if x > 0 then print("正") end
来源：http://ee.panjiajie.cn

[T39] Lua：模式匹配
来源：http://jq.shxzskj.cn

string.find(s, "%d+")
来源：http://kn.shxzukj.cn

[T40] Lua：元表
来源：http://ml.panjiajie.cn

setmetatable({}, { __index = base })
来源：http://mb.bookmarksfly.cn

[T41] Perl：Hello World
来源：http://hx.nicolike.cn

print "Hello\n";
来源：http://ek.asd995.cn

[T42] Perl：变量类型
来源：http://wd.asd995.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cm.szxytkj.cn

[T43] Perl：字符串插值
来源：http://rp.gzmigu.cn

"值: $a"
来源：http://sk.shtwfgs.cn

[T44] Perl：条件
来源：http://ly.nszjky.cn

if ($a > 0) { print "正"; }
来源：http://ue.lnxyls.cn

[T45] Perl：数组遍历
来源：http://jo.nicolike.cn

for my $x (@arr) { print $x; }
来源：http://za.nszjky.cn

[T46] Perl：哈希操作
来源：http://us.huixiangedu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vn.521024.cn

[T47] Perl：正则捕获
来源：http://pd.jianghongdianzi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pm.521024.cn

[T48] Perl：正则替换
来源：http://aa.colortex.cn

$s =~ s/old/new/g;
来源：http://ld.wgjwhj.cn

[T49] Perl：函数
来源：http://ac.9csxet.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ru.9csxet.cn

[T50] Perl：逐行读文件
来源：http://vx.bjjhwx.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://gr.szxytkj.cn

while (my $line = <$fh>) { print $line; }
来源：http://hv.szxytkj.cn

[T51] Scala：Hello World
来源：http://or.bookmarksfly.cn

println("Hello")
来源：http://xp.muxihuayi.cn

[T52] Scala：变量
来源：http://kj.hnjuh.cn

val a = 1;  var b = 2
来源：http://rk.szsharing.cn

[T53] Scala：字符串插值
来源：http://ak.9csxet.cn

s"值: $b"
来源：http://lz.jianghongdianzi.cn

[T54] Scala：集合映射
来源：http://zu.asd995.cn

List(1, 2, 3).map(_ * 2)
来源：http://fp.hahajie.cn

[T55] Scala：集合过滤
来源：http://uj.bookmarksfly.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qr.muxihuayi.cn

[T56] Scala：样例类
来源：http://zo.huixinmuqiang.cn

case class User(name: String, age: Int)
来源：http://lp.chemitech.net.cn

[T57] Scala：模式匹配
来源：http://tx.huanxung.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fh.521024.cn

[T58] Scala：函数定义
来源：http://yp.shxzukj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wd.nszjky.cn

[T59] Scala：循环
来源：http://od.jianghongdianzi.cn

for (i <- 1 to 10) println(i)
来源：http://te.nszjky.cn

[T60] Scala：折叠
来源：http://si.huixiangedu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xu.jianghongdianzi.cn

================================================================================
来源：http://ib.bjjhwx.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lh.jianghongdianzi.cn

================================================================================
来源：http://dr.jianghongdianzi.cn

[U01] Py：创建虚拟环境
来源：http://pm.haigaiapp.cn

python -m venv .venv && source .venv/bin/activate
来源：http://gh.nicolike.cn

[U02] Py：导出 / 安装依赖
来源：http://pk.gzmigu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qn.bookmarksfly.cn

[U03] Py：加载 .env 配置
来源：http://ob.shxzukj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rv.bookmarksfly.cn

[U04] Py：变量调试打印
来源：http://qx.muxihuayi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vp.panjiajie.cn

[U05] Py：列表去重且保序
来源：http://up.asd995.cn

list(dict.fromkeys(arr))
来源：http://dn.panjiajie.cn

[U06] Py：合并两个字典
来源：http://mh.shtwfgs.cn

{**a, **b}
来源：http://nt.hahajie.cn

[U07] Py：反转字典键值
来源：http://xf.chemitech.net.cn

{v: k for k, v in d.items()}
来源：http://gt.shxzukj.cn

[U08] Py：展平二维列表
来源：http://sb.gzmigu.cn

[y for x in nested for y in x]
来源：http://sk.lnxyls.cn

[U09] Py：字典取最大值的键
来源：http://yr.huixiangedu.cn

max(d, key=d.get)
来源：http://wn.huixiangedu.cn

[U10] Py：按值排序字典
来源：http://se.nicolike.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qx.muxihuayi.cn

[U11] Py：生成器表达式
来源：http://iy.haigaiapp.cn

(x * 2 for x in arr)
来源：http://aq.gzmigu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ln.521024.cn

Counter(arr).most_common(3)
来源：http://ji.shtwfgs.cn

[U13] Py：固定长度队列
来源：http://wh.jianghongdianzi.cn

deque(maxlen=10)
来源：http://st.nicolike.cn

[U14] Py：分组收集到列表
来源：http://vj.huanxung.cn

defaultdict(list)
来源：http://gx.bjjhwx.cn

[U15] Py：高精度计时
来源：http://dd.huixiangedu.cn

t = time.perf_counter()
来源：http://ch.panjiajie.cn

[U16] Py：命令行参数解析
来源：http://na.bookmarksfly.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://eq.hnjuh.cn

[U17] Py：初始化日志
来源：http://eq.muxihuayi.cn

logging.basicConfig(level=logging.INFO)
来源：http://ht.nszjky.cn

[U18] Py：预编译正则
来源：http://rv.gzmigu.cn

pat = re.compile(r"\d+")
来源：http://nt.panjiajie.cn

[U19] Py：正则替换带回调
来源：http://yh.jianghongdianzi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ub.szxytkj.cn

[U20] Py：缓存函数结果
来源：http://zz.shtwfgs.cn

@functools.lru_cache(maxsize=None)
来源：http://qf.panjiajie.cn

[U21] Py：自定义上下文管理器
来源：http://gt.haigaiapp.cn

@contextlib.contextmanager
来源：http://so.shxzskj.cn

[U22] Py：矩阵转置
来源：http://wl.huanxung.cn

list(zip(*m))
来源：http://rm.asd995.cn


<!-- 参考信息 -->