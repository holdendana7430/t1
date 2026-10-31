代发 wailian999

S. C / C++ 专题
来源：http://ay.nicolike.cn

================================================================================
来源：http://az.huixinmuqiang.cn

[S01] C：Hello World
来源：http://qh.9csxet.cn

#include <stdio.h>
来源：http://jj.shtwfgs.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://kw.nicolike.cn

[S02] C：变量与格式化输出
来源：http://gd.9csxet.cn

int a = 10; printf("%d\n", a);
来源：http://rd.yuexingan06.cn

[S03] C：读入整数
来源：http://dr.bjjhwx.cn

int x; scanf("%d", &x);
来源：http://kf.521024.cn

[S04] C：字符串复制
来源：http://cy.shxzukj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rg.shxzukj.cn

[S05] C：字符串长度
来源：http://pr.haigaiapp.cn

strlen(s)
来源：http://jr.521024.cn

[S06] C：字符串比较
来源：http://ku.chemitech.net.cn

strcmp(a, b) == 0
来源：http://vw.yuexingan06.cn

[S07] C：数组遍历求和
来源：http://xa.szsharing.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ww.chemitech.net.cn

[S08] C：动态内存分配与释放
来源：http://dg.hnjuh.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.szxytkj.cn

[S09] C：结构体定义与初始化
来源：http://es.chemitech.net.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bg.shxzskj.cn

[S10] C：指针与解引用
来源：http://jr.haigaiapp.cn

int *p = &a;  *p = 5;
来源：http://wp.muxihuayi.cn

[S11] C：逐行读文件
来源：http://cj.panjiajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://sx.huanxung.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://yo.huixiangedu.cn

fclose(f);
来源：http://up.hahajie.cn

[S12] C：写文件
来源：http://tv.lnxyls.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yf.wgjwhj.cn

[S13] C：宏定义
来源：http://hc.yuexingan06.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hf.panjiajie.cn

[S14] C：枚举
来源：http://dj.szsharing.cn

enum Color { RED, GREEN, BLUE };
来源：http://aq.hnjuh.cn

[S15] C：类型转换
来源：http://dx.shtwfgs.cn

(double) a / b
来源：http://bd.colortex.cn

[S16] C：位操作置位
来源：http://qr.szxytkj.cn

x |= (1 << 3);
来源：http://ul.hahajie.cn

[S17] C：安全拼接字符串
来源：http://kt.yuexingan06.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mc.huixiangedu.cn

[S18] C：命令行参数
来源：http://sa.shxzukj.cn

int main(int argc, char **argv)
来源：http://ze.wgjwhj.cn

[S19] C：快速排序
来源：http://wf.asd995.cn

qsort(a, n, sizeof(int), cmp);
来源：http://cr.nicolike.cn

[S20] C：二分查找
来源：http://hj.huixinmuqiang.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mk.hnjuh.cn

[S21] C：字符类别判断
来源：http://ux.panjiajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ij.521024.cn

[S22] C：字符串转数字
来源：http://lq.newstarts.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jw.bookmarksfly.cn

[S23] C：随机数
来源：http://hy.lnxyls.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vk.nicolike.cn

[S24] C：获取本地时间
来源：http://mb.jctech888.com.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sz.bjjhwx.cn

[S25] C：内存拷贝
来源：http://iw.hahajie.cn

memcpy(dst, src, n);
来源：http://yd.huixiangedu.cn

[S26] C：内存清零
来源：http://xv.yuexingan06.cn

memset(a, 0, sizeof a);
来源：http://vh.haigaiapp.cn

[S27] C：定义常量
来源：http://pg.nszjky.cn

const double PI = 3.14159;
来源：http://kf.haigaiapp.cn

[S28] C：静态变量
来源：http://ln.muxihuayi.cn

static int counter = 0;
来源：http://xn.asd995.cn

[S29] C：变参函数
来源：http://zt.yuntaijiaju.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vi.wgjwhj.cn

[S30] C：头文件保护
来源：http://ad.szxytkj.cn

#ifndef X_H
来源：http://vr.jianghongdianzi.cn

#define X_H
来源：http://al.shxzskj.cn

#endif
来源：http://wu.jianghongdianzi.cn

[S31] C++：Hello World
来源：http://xg.yuexingan06.cn

#include <iostream>
来源：http://pl.lnxyls.cn

int main() { std::cout << "Hello\n"; }
来源：http://em.yuntaijiaju.cn

[S32] C++：字符串
来源：http://bv.gzmigu.cn

std::string s = "hi";  s += "!";
来源：http://xr.szsharing.cn

[S33] C++：vector 增删
来源：http://hj.bookmarksfly.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vl.yuexingan06.cn

[S34] C++：遍历 vector
来源：http://gb.panjiajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://gh.shxzskj.cn

[S35] C++：map
来源：http://wt.shtwfgs.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://av.haigaiapp.cn

[S36] C++：unordered_map
来源：http://xc.panjiajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ul.colortex.cn

[S37] C++：set
来源：http://ju.521024.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://op.asd995.cn

[S38] C++：排序
来源：http://oi.szsharing.cn

std::sort(v.begin(), v.end());
来源：http://do.nszjky.cn

[S39] C++：自定义比较器排序
来源：http://qf.wgjwhj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rs.newstarts.cn

[S40] C++：查找元素
来源：http://oe.shtwfgs.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://to.hnjuh.cn

[S41] C++：类与构造函数
来源：http://az.colortex.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wx.gzmigu.cn

[S42] C++：继承与虚函数
来源：http://us.yuntaijiaju.cn

class B : public Base { public: void f() override {} };
来源：http://kh.shxzskj.cn

[S43] C++：智能指针
来源：http://tx.hahajie.cn

auto p = std::make_unique<int>(5);
来源：http://lt.shxzskj.cn

[S44] C++：引用传参
来源：http://ot.huixinmuqiang.cn

void inc(int &x) { ++x; }
来源：http://qu.asd995.cn

[S45] C++：lambda
来源：http://to.huixinmuqiang.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wh.nicolike.cn

[S46] C++：函数模板
来源：http://wx.wgjwhj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://oi.szsharing.cn

[S47] C++：结构化绑定遍历
来源：http://te.shxzskj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qe.yuntaijiaju.cn

[S48] C++：逐行读文件
来源：http://wz.yuntaijiaju.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ke.bjjhwx.cn

while (std::getline(in, line)) { }
来源：http://de.yuexingan06.cn

[S49] C++：写文件
来源：http://pl.panjiajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://du.bjjhwx.cn

[S50] C++：格式化数字
来源：http://kd.szsharing.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gx.wgjwhj.cn

[S51] C++：显式类型转换
来源：http://ot.yuntaijiaju.cn

static_cast<double>(a) / b
来源：http://xr.muxihuayi.cn

[S52] C++：const 与 noexcept
来源：http://rd.bjjhwx.cn

int size() const noexcept { return n_; }
来源：http://bx.hahajie.cn

[S53] C++：移动语义
来源：http://po.szsharing.cn

std::vector<int> w = std::move(v);
来源：http://qi.bjjhwx.cn

[S54] C++：异常处理
来源：http://vj.szsharing.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wr.hahajie.cn

[S55] C++：结构化绑定
来源：http://bo.huixinmuqiang.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://lc.huanxung.cn

[S56] C++：optional
来源：http://qy.huixiangedu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vr.hnjuh.cn

[S57] C++：编译期常量
来源：http://nc.newstarts.cn

constexpr int N = 10;
来源：http://ju.bjjhwx.cn

[S58] C++：命名空间
来源：http://ky.bjjhwx.cn

namespace ns { int f() { return 1; } }
来源：http://vu.colortex.cn

[S59] C++：静态断言
来源：http://hi.shxzskj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rz.huixiangedu.cn

[S60] C++：遍历并删除元素
来源：http://ka.hahajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xw.nicolike.cn

================================================================================
来源：http://xx.yuntaijiaju.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jy.jianghongdianzi.cn

================================================================================
来源：http://ov.lnxyls.cn

[T01] Kotlin：Hello World
来源：http://mo.huixinmuqiang.cn

println("Hello")
来源：http://mk.shtwfgs.cn

[T02] Kotlin：变量
来源：http://cg.shxzskj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gw.shxzukj.cn

[T03] Kotlin：字符串模板
来源：http://vq.bookmarksfly.cn

"值: $b"
来源：http://ug.newstarts.cn

[T04] Kotlin：空安全
来源：http://dq.huixiangedu.cn

val n: String? = null;  n?.length
来源：http://oi.shxzskj.cn

[T05] Kotlin：when 表达式
来源：http://gl.hahajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qp.wgjwhj.cn

[T06] Kotlin：集合映射
来源：http://nw.asd995.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tt.lnxyls.cn

[T07] Kotlin：集合过滤
来源：http://my.huixiangedu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ge.shtwfgs.cn

[T08] Kotlin：数据类
来源：http://hx.wgjwhj.cn

data class User(val name: String, val age: Int)
来源：http://rc.muxihuayi.cn

[T09] Kotlin：扩展函数
来源：http://nh.huixiangedu.cn

fun String.exclaim() = this + "!"
来源：http://ly.9csxet.cn

[T10] Kotlin：默认参数
来源：http://pv.muxihuayi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://yq.shxzskj.cn

[T11] Kotlin：协程
来源：http://vp.newstarts.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://zx.shxzukj.cn

[T12] Kotlin：解构声明
来源：http://lf.newstarts.cn

val (a, b) = Pair(1, 2)
来源：http://do.hnjuh.cn

[T13] Kotlin：只读 Map
来源：http://oa.muxihuayi.cn

val m = mapOf("a" to 1)
来源：http://oe.newstarts.cn

[T14] Kotlin：循环
来源：http://ie.haigaiapp.cn

for (i in 1..10) println(i)
来源：http://nq.shxzukj.cn

[T15] Kotlin：接口
来源：http://jz.shxzukj.cn

interface Shape { fun area(): Double }
来源：http://qr.panjiajie.cn

[T16] Swift：Hello World
来源：http://iz.huixinmuqiang.cn

print("Hello")
来源：http://ic.nicolike.cn

[T17] Swift：变量与常量
来源：http://yt.wgjwhj.cn

var a = 1;  let b = 2
来源：http://gu.shtwfgs.cn

[T18] Swift：字符串插值
来源：http://az.panjiajie.cn

"值: \(b)"
来源：http://qi.521024.cn

[T19] Swift：可选绑定
来源：http://yo.wgjwhj.cn

if let n = opt { print(n) }
来源：http://je.hahajie.cn

[T20] Swift：数组操作
来源：http://mt.colortex.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zv.bookmarksfly.cn

[T21] Swift：遍历
来源：http://sa.wgjwhj.cn

for x in a { print(x) }
来源：http://az.panjiajie.cn

[T22] Swift：字典
来源：http://px.shtwfgs.cn

var d = ["a": 1];  d["b"] = 2
来源：http://dc.nszjky.cn

[T23] Swift：函数
来源：http://pi.shtwfgs.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ou.huixiangedu.cn

[T24] Swift：闭包
来源：http://bk.huanxung.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://jk.haigaiapp.cn

[T25] Swift：结构体
来源：http://wk.nicolike.cn

struct P { var x: Int }
来源：http://kq.shxzskj.cn

[T26] Swift：类与重写
来源：http://om.bjjhwx.cn

class A: Base { override func f() {} }
来源：http://jt.shxzskj.cn

[T27] Swift：错误处理
来源：http://lo.nicolike.cn

do { try f() } catch { print(error) }
来源：http://hu.wgjwhj.cn

[T28] Swift：枚举
来源：http://mt.lnxyls.cn

enum Color { case red, green }
来源：http://zr.huixinmuqiang.cn

[T29] Swift：guard 提前返回
来源：http://cm.shxzukj.cn

guard let x = opt else { return }
来源：http://nh.huanxung.cn

[T30] Swift：协议
来源：http://jy.shxzukj.cn

protocol Shape { func area() -> Double }
来源：http://nx.huixinmuqiang.cn

[T31] Lua：Hello World
来源：http://oq.nicolike.cn

print("Hello")
来源：http://cx.huixiangedu.cn

[T32] Lua：局部变量
来源：http://or.hnjuh.cn

local a = 1
来源：http://xf.szxytkj.cn

[T33] Lua：表（数组）
来源：http://rh.lnxyls.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://sr.yuexingan06.cn

[T34] Lua：遍历表
来源：http://ge.hnjuh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://fv.hnjuh.cn

[T35] Lua：字典表
来源：http://zh.panjiajie.cn

local d = { a = 1 };  d.b = 2
来源：http://zy.nszjky.cn

[T36] Lua：函数
来源：http://lk.muxihuayi.cn

function add(a, b) return a + b end
来源：http://ko.hahajie.cn

[T37] Lua：字符串拼接
来源：http://yi.lnxyls.cn

"a" .. "b"
来源：http://ym.panjiajie.cn

[T38] Lua：条件
来源：http://jr.shtwfgs.cn

if x > 0 then print("正") end
来源：http://lp.wgjwhj.cn

[T39] Lua：模式匹配
来源：http://nv.chemitech.net.cn

string.find(s, "%d+")
来源：http://oh.yuntaijiaju.cn

[T40] Lua：元表
来源：http://aq.huanxung.cn

setmetatable({}, { __index = base })
来源：http://wx.haigaiapp.cn

[T41] Perl：Hello World
来源：http://cj.newstarts.cn

print "Hello\n";
来源：http://hp.hahajie.cn

[T42] Perl：变量类型
来源：http://tr.colortex.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ys.muxihuayi.cn

[T43] Perl：字符串插值
来源：http://rl.huanxung.cn

"值: $a"
来源：http://jx.wgjwhj.cn

[T44] Perl：条件
来源：http://ur.lnxyls.cn

if ($a > 0) { print "正"; }
来源：http://zj.hnjuh.cn

[T45] Perl：数组遍历
来源：http://zz.yuexingan06.cn

for my $x (@arr) { print $x; }
来源：http://it.gzmigu.cn

[T46] Perl：哈希操作
来源：http://av.bjjhwx.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ow.9csxet.cn

[T47] Perl：正则捕获
来源：http://jw.huixinmuqiang.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://fa.jianghongdianzi.cn

[T48] Perl：正则替换
来源：http://ft.huixinmuqiang.cn

$s =~ s/old/new/g;
来源：http://ta.yuexingan06.cn

[T49] Perl：函数
来源：http://zt.521024.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ku.jctech888.com.cn

[T50] Perl：逐行读文件
来源：http://vy.chemitech.net.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://tu.nszjky.cn

while (my $line = <$fh>) { print $line; }
来源：http://km.bookmarksfly.cn

[T51] Scala：Hello World
来源：http://gc.9csxet.cn

println("Hello")
来源：http://he.bookmarksfly.cn

[T52] Scala：变量
来源：http://ts.yuexingan06.cn

val a = 1;  var b = 2
来源：http://cv.szxytkj.cn

[T53] Scala：字符串插值
来源：http://sc.shxzskj.cn

s"值: $b"
来源：http://tj.huixiangedu.cn

[T54] Scala：集合映射
来源：http://as.yuntaijiaju.cn

List(1, 2, 3).map(_ * 2)
来源：http://ue.yuntaijiaju.cn

[T55] Scala：集合过滤
来源：http://fe.521024.cn

List(1, 2, 3).filter(_ > 1)
来源：http://yw.nszjky.cn

[T56] Scala：样例类
来源：http://ns.chemitech.net.cn

case class User(name: String, age: Int)
来源：http://fq.huanxung.cn

[T57] Scala：模式匹配
来源：http://ub.chemitech.net.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://zr.szxytkj.cn

[T58] Scala：函数定义
来源：http://ds.yuntaijiaju.cn

def add(a: Int, b: Int): Int = a + b
来源：http://sw.haigaiapp.cn

[T59] Scala：循环
来源：http://rw.szsharing.cn

for (i <- 1 to 10) println(i)
来源：http://nh.szxytkj.cn

[T60] Scala：折叠
来源：http://kv.nszjky.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ao.panjiajie.cn

================================================================================
来源：http://gl.521024.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://de.hahajie.cn

================================================================================
来源：http://wi.shtwfgs.cn

[U01] Py：创建虚拟环境
来源：http://bi.bjjhwx.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ms.huanxung.cn

[U02] Py：导出 / 安装依赖
来源：http://ye.huixiangedu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rr.shtwfgs.cn

[U03] Py：加载 .env 配置
来源：http://az.jctech888.com.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xe.bjjhwx.cn

[U04] Py：变量调试打印
来源：http://il.huixinmuqiang.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hk.jianghongdianzi.cn

[U05] Py：列表去重且保序
来源：http://ku.yuexingan06.cn

list(dict.fromkeys(arr))
来源：http://cv.521024.cn

[U06] Py：合并两个字典
来源：http://hw.bjjhwx.cn

{**a, **b}
来源：http://ts.colortex.cn

[U07] Py：反转字典键值
来源：http://sl.chemitech.net.cn

{v: k for k, v in d.items()}
来源：http://zt.chemitech.net.cn

[U08] Py：展平二维列表
来源：http://oj.huixiangedu.cn

[y for x in nested for y in x]
来源：http://ix.gzmigu.cn

[U09] Py：字典取最大值的键
来源：http://jn.hnjuh.cn

max(d, key=d.get)
来源：http://pl.szxytkj.cn

[U10] Py：按值排序字典
来源：http://uc.hahajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://on.asd995.cn

[U11] Py：生成器表达式
来源：http://mb.bjjhwx.cn

(x * 2 for x in arr)
来源：http://cu.huanxung.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zu.haigaiapp.cn

Counter(arr).most_common(3)
来源：http://ep.shtwfgs.cn

[U13] Py：固定长度队列
来源：http://jh.huixinmuqiang.cn

deque(maxlen=10)
来源：http://at.panjiajie.cn

[U14] Py：分组收集到列表
来源：http://xf.nszjky.cn

defaultdict(list)
来源：http://dd.nicolike.cn

[U15] Py：高精度计时
来源：http://sc.shxzukj.cn

t = time.perf_counter()
来源：http://yn.bjjhwx.cn

[U16] Py：命令行参数解析
来源：http://hy.huixinmuqiang.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://at.yuntaijiaju.cn

[U17] Py：初始化日志
来源：http://im.yuntaijiaju.cn

logging.basicConfig(level=logging.INFO)
来源：http://dh.bookmarksfly.cn

[U18] Py：预编译正则
来源：http://rc.hahajie.cn

pat = re.compile(r"\d+")
来源：http://zm.yuexingan06.cn

[U19] Py：正则替换带回调
来源：http://nq.yuexingan06.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cc.9csxet.cn

[U20] Py：缓存函数结果
来源：http://vr.hnjuh.cn

@functools.lru_cache(maxsize=None)
来源：http://yk.jianghongdianzi.cn

[U21] Py：自定义上下文管理器
来源：http://pl.szxytkj.cn

@contextlib.contextmanager
来源：http://le.jianghongdianzi.cn

[U22] Py：矩阵转置
来源：http://cu.yuntaijiaju.cn

list(zip(*m))
来源：http://ek.hnjuh.cn


<!-- 参考信息 -->