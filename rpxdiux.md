代发 wailian999

S. C / C++ 专题
来源：http://mh.yuntaijiaju.cn

================================================================================
来源：http://vp.huanxung.cn

[S01] C：Hello World
来源：http://ye.chemitech.net.cn

#include <stdio.h>
来源：http://mx.shxzskj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bl.panjiajie.cn

[S02] C：变量与格式化输出
来源：http://hw.521024.cn

int a = 10; printf("%d\n", a);
来源：http://wi.colortex.cn

[S03] C：读入整数
来源：http://lu.huixiangedu.cn

int x; scanf("%d", &x);
来源：http://yw.bookmarksfly.cn

[S04] C：字符串复制
来源：http://tc.shxzukj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://up.panjiajie.cn

[S05] C：字符串长度
来源：http://yz.lnxyls.cn

strlen(s)
来源：http://in.colortex.cn

[S06] C：字符串比较
来源：http://lb.hahajie.cn

strcmp(a, b) == 0
来源：http://sr.chemitech.net.cn

[S07] C：数组遍历求和
来源：http://lm.hahajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hs.szsharing.cn

[S08] C：动态内存分配与释放
来源：http://ld.szsharing.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fr.muxihuayi.cn

[S09] C：结构体定义与初始化
来源：http://if.bookmarksfly.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://eh.yuexingan06.cn

[S10] C：指针与解引用
来源：http://ng.9csxet.cn

int *p = &a;  *p = 5;
来源：http://xb.huixinmuqiang.cn

[S11] C：逐行读文件
来源：http://mb.wgjwhj.cn

FILE *f = fopen("a.txt", "r");
来源：http://xy.wgjwhj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qu.jianghongdianzi.cn

fclose(f);
来源：http://in.hahajie.cn

[S12] C：写文件
来源：http://hh.huixiangedu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mg.gzmigu.cn

[S13] C：宏定义
来源：http://nh.szxytkj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kq.nszjky.cn

[S14] C：枚举
来源：http://sg.hahajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://ha.shxzskj.cn

[S15] C：类型转换
来源：http://sg.wgjwhj.cn

(double) a / b
来源：http://xx.szsharing.cn

[S16] C：位操作置位
来源：http://wd.yuntaijiaju.cn

x |= (1 << 3);
来源：http://xp.nicolike.cn

[S17] C：安全拼接字符串
来源：http://jc.chemitech.net.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xm.hahajie.cn

[S18] C：命令行参数
来源：http://gv.yuntaijiaju.cn

int main(int argc, char **argv)
来源：http://bb.shxzukj.cn

[S19] C：快速排序
来源：http://wt.yuntaijiaju.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ot.yuexingan06.cn

[S20] C：二分查找
来源：http://fx.shxzukj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rs.panjiajie.cn

[S21] C：字符类别判断
来源：http://ru.chemitech.net.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gv.shtwfgs.cn

[S22] C：字符串转数字
来源：http://tq.wgjwhj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://am.huixiangedu.cn

[S23] C：随机数
来源：http://as.lnxyls.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ty.haigaiapp.cn

[S24] C：获取本地时间
来源：http://yt.asd995.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sv.hnjuh.cn

[S25] C：内存拷贝
来源：http://sk.muxihuayi.cn

memcpy(dst, src, n);
来源：http://zw.9csxet.cn

[S26] C：内存清零
来源：http://xq.yuexingan06.cn

memset(a, 0, sizeof a);
来源：http://cw.shxzukj.cn

[S27] C：定义常量
来源：http://xo.nicolike.cn

const double PI = 3.14159;
来源：http://xm.9csxet.cn

[S28] C：静态变量
来源：http://qv.huixinmuqiang.cn

static int counter = 0;
来源：http://vx.muxihuayi.cn

[S29] C：变参函数
来源：http://hd.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qa.gzmigu.cn

[S30] C：头文件保护
来源：http://ua.hnjuh.cn

#ifndef X_H
来源：http://bk.szsharing.cn

#define X_H
来源：http://yy.lnxyls.cn

#endif
来源：http://lx.shxzukj.cn

[S31] C++：Hello World
来源：http://af.colortex.cn

#include <iostream>
来源：http://tz.wgjwhj.cn

int main() { std::cout << "Hello\n"; }
来源：http://eq.panjiajie.cn

[S32] C++：字符串
来源：http://fp.yuntaijiaju.cn

std::string s = "hi";  s += "!";
来源：http://mc.hahajie.cn

[S33] C++：vector 增删
来源：http://ig.huixiangedu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xo.yuntaijiaju.cn

[S34] C++：遍历 vector
来源：http://dj.chemitech.net.cn

for (auto &x : v) { std::cout << x; }
来源：http://qq.gzmigu.cn

[S35] C++：map
来源：http://fv.jianghongdianzi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tx.gzmigu.cn

[S36] C++：unordered_map
来源：http://cx.huanxung.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://us.jianghongdianzi.cn

[S37] C++：set
来源：http://pl.yuntaijiaju.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://up.jctech888.com.cn

[S38] C++：排序
来源：http://zm.9csxet.cn

std::sort(v.begin(), v.end());
来源：http://fm.yuexingan06.cn

[S39] C++：自定义比较器排序
来源：http://da.hahajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bz.newstarts.cn

[S40] C++：查找元素
来源：http://jf.shxzukj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tt.panjiajie.cn

[S41] C++：类与构造函数
来源：http://ad.nszjky.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tr.panjiajie.cn

[S42] C++：继承与虚函数
来源：http://fo.chemitech.net.cn

class B : public Base { public: void f() override {} };
来源：http://iw.nicolike.cn

[S43] C++：智能指针
来源：http://yj.huixinmuqiang.cn

auto p = std::make_unique<int>(5);
来源：http://lr.yuntaijiaju.cn

[S44] C++：引用传参
来源：http://dm.jianghongdianzi.cn

void inc(int &x) { ++x; }
来源：http://yp.newstarts.cn

[S45] C++：lambda
来源：http://sy.yuexingan06.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fa.yuntaijiaju.cn

[S46] C++：函数模板
来源：http://zc.szxytkj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ac.shxzskj.cn

[S47] C++：结构化绑定遍历
来源：http://br.nicolike.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kx.wgjwhj.cn

[S48] C++：逐行读文件
来源：http://md.szxytkj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gz.nszjky.cn

while (std::getline(in, line)) { }
来源：http://xb.panjiajie.cn

[S49] C++：写文件
来源：http://ea.shxzskj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jr.yuntaijiaju.cn

[S50] C++：格式化数字
来源：http://kh.hnjuh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yq.nicolike.cn

[S51] C++：显式类型转换
来源：http://xv.gzmigu.cn

static_cast<double>(a) / b
来源：http://oh.shxzukj.cn

[S52] C++：const 与 noexcept
来源：http://gi.9csxet.cn

int size() const noexcept { return n_; }
来源：http://ul.bookmarksfly.cn

[S53] C++：移动语义
来源：http://dy.newstarts.cn

std::vector<int> w = std::move(v);
来源：http://db.nicolike.cn

[S54] C++：异常处理
来源：http://qi.bookmarksfly.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ut.wgjwhj.cn

[S55] C++：结构化绑定
来源：http://dl.huixiangedu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pz.shtwfgs.cn

[S56] C++：optional
来源：http://sq.muxihuayi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wp.jctech888.com.cn

[S57] C++：编译期常量
来源：http://fx.9csxet.cn

constexpr int N = 10;
来源：http://tm.9csxet.cn

[S58] C++：命名空间
来源：http://ft.shxzskj.cn

namespace ns { int f() { return 1; } }
来源：http://vl.szxytkj.cn

[S59] C++：静态断言
来源：http://nk.szsharing.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yn.haigaiapp.cn

[S60] C++：遍历并删除元素
来源：http://ul.yuexingan06.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ip.haigaiapp.cn

================================================================================
来源：http://qa.huixiangedu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mv.lnxyls.cn

================================================================================
来源：http://zt.wgjwhj.cn

[T01] Kotlin：Hello World
来源：http://cq.shxzukj.cn

println("Hello")
来源：http://mr.jianghongdianzi.cn

[T02] Kotlin：变量
来源：http://bx.huixiangedu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://du.yuexingan06.cn

[T03] Kotlin：字符串模板
来源：http://yp.lnxyls.cn

"值: $b"
来源：http://rc.521024.cn

[T04] Kotlin：空安全
来源：http://zo.huixiangedu.cn

val n: String? = null;  n?.length
来源：http://yp.asd995.cn

[T05] Kotlin：when 表达式
来源：http://eq.panjiajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://au.bookmarksfly.cn

[T06] Kotlin：集合映射
来源：http://nn.hahajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://lb.shtwfgs.cn

[T07] Kotlin：集合过滤
来源：http://by.521024.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wk.yuntaijiaju.cn

[T08] Kotlin：数据类
来源：http://zz.muxihuayi.cn

data class User(val name: String, val age: Int)
来源：http://xp.gzmigu.cn

[T09] Kotlin：扩展函数
来源：http://fi.shxzukj.cn

fun String.exclaim() = this + "!"
来源：http://fv.hnjuh.cn

[T10] Kotlin：默认参数
来源：http://zk.nszjky.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gj.panjiajie.cn

[T11] Kotlin：协程
来源：http://nv.nicolike.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ir.asd995.cn

[T12] Kotlin：解构声明
来源：http://vy.muxihuayi.cn

val (a, b) = Pair(1, 2)
来源：http://mh.bookmarksfly.cn

[T13] Kotlin：只读 Map
来源：http://io.shtwfgs.cn

val m = mapOf("a" to 1)
来源：http://wo.shxzukj.cn

[T14] Kotlin：循环
来源：http://uh.chemitech.net.cn

for (i in 1..10) println(i)
来源：http://gl.chemitech.net.cn

[T15] Kotlin：接口
来源：http://si.szxytkj.cn

interface Shape { fun area(): Double }
来源：http://rc.panjiajie.cn

[T16] Swift：Hello World
来源：http://ei.szsharing.cn

print("Hello")
来源：http://rx.huixinmuqiang.cn

[T17] Swift：变量与常量
来源：http://tl.panjiajie.cn

var a = 1;  let b = 2
来源：http://yi.jctech888.com.cn

[T18] Swift：字符串插值
来源：http://py.shxzukj.cn

"值: \(b)"
来源：http://tr.muxihuayi.cn

[T19] Swift：可选绑定
来源：http://li.panjiajie.cn

if let n = opt { print(n) }
来源：http://ip.huixiangedu.cn

[T20] Swift：数组操作
来源：http://ko.521024.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ae.shtwfgs.cn

[T21] Swift：遍历
来源：http://jr.jctech888.com.cn

for x in a { print(x) }
来源：http://ev.muxihuayi.cn

[T22] Swift：字典
来源：http://wa.panjiajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://gx.huixinmuqiang.cn

[T23] Swift：函数
来源：http://yl.huanxung.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vf.newstarts.cn

[T24] Swift：闭包
来源：http://pn.hnjuh.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xu.lnxyls.cn

[T25] Swift：结构体
来源：http://xm.nszjky.cn

struct P { var x: Int }
来源：http://xm.nicolike.cn

[T26] Swift：类与重写
来源：http://tx.colortex.cn

class A: Base { override func f() {} }
来源：http://ri.nicolike.cn

[T27] Swift：错误处理
来源：http://sh.shxzukj.cn

do { try f() } catch { print(error) }
来源：http://bj.panjiajie.cn

[T28] Swift：枚举
来源：http://ca.gzmigu.cn

enum Color { case red, green }
来源：http://uk.shxzskj.cn

[T29] Swift：guard 提前返回
来源：http://om.szxytkj.cn

guard let x = opt else { return }
来源：http://gb.huixinmuqiang.cn

[T30] Swift：协议
来源：http://um.hnjuh.cn

protocol Shape { func area() -> Double }
来源：http://le.huanxung.cn

[T31] Lua：Hello World
来源：http://vh.hnjuh.cn

print("Hello")
来源：http://ay.huanxung.cn

[T32] Lua：局部变量
来源：http://gb.lnxyls.cn

local a = 1
来源：http://hy.shxzskj.cn

[T33] Lua：表（数组）
来源：http://sc.gzmigu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zq.bjjhwx.cn

[T34] Lua：遍历表
来源：http://sc.hahajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ok.lnxyls.cn

[T35] Lua：字典表
来源：http://xc.nicolike.cn

local d = { a = 1 };  d.b = 2
来源：http://wj.shtwfgs.cn

[T36] Lua：函数
来源：http://vc.shxzukj.cn

function add(a, b) return a + b end
来源：http://nl.shtwfgs.cn

[T37] Lua：字符串拼接
来源：http://kb.hahajie.cn

"a" .. "b"
来源：http://ya.huixiangedu.cn

[T38] Lua：条件
来源：http://wk.nszjky.cn

if x > 0 then print("正") end
来源：http://jf.bookmarksfly.cn

[T39] Lua：模式匹配
来源：http://gb.chemitech.net.cn

string.find(s, "%d+")
来源：http://bc.bookmarksfly.cn

[T40] Lua：元表
来源：http://rm.shtwfgs.cn

setmetatable({}, { __index = base })
来源：http://hd.lnxyls.cn

[T41] Perl：Hello World
来源：http://ho.bookmarksfly.cn

print "Hello\n";
来源：http://xv.jianghongdianzi.cn

[T42] Perl：变量类型
来源：http://ha.shxzskj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dd.chemitech.net.cn

[T43] Perl：字符串插值
来源：http://qs.colortex.cn

"值: $a"
来源：http://bf.huixiangedu.cn

[T44] Perl：条件
来源：http://kt.bjjhwx.cn

if ($a > 0) { print "正"; }
来源：http://te.colortex.cn

[T45] Perl：数组遍历
来源：http://cm.bjjhwx.cn

for my $x (@arr) { print $x; }
来源：http://bo.muxihuayi.cn

[T46] Perl：哈希操作
来源：http://ar.wgjwhj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qa.panjiajie.cn

[T47] Perl：正则捕获
来源：http://li.huixiangedu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://tf.jctech888.com.cn

[T48] Perl：正则替换
来源：http://gf.521024.cn

$s =~ s/old/new/g;
来源：http://wj.bjjhwx.cn

[T49] Perl：函数
来源：http://xz.huixinmuqiang.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sd.shtwfgs.cn

[T50] Perl：逐行读文件
来源：http://zg.muxihuayi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://kl.haigaiapp.cn

while (my $line = <$fh>) { print $line; }
来源：http://sv.lnxyls.cn

[T51] Scala：Hello World
来源：http://kc.muxihuayi.cn

println("Hello")
来源：http://zr.newstarts.cn

[T52] Scala：变量
来源：http://lq.hnjuh.cn

val a = 1;  var b = 2
来源：http://gu.shtwfgs.cn

[T53] Scala：字符串插值
来源：http://qr.wgjwhj.cn

s"值: $b"
来源：http://xx.yuntaijiaju.cn

[T54] Scala：集合映射
来源：http://ba.colortex.cn

List(1, 2, 3).map(_ * 2)
来源：http://zt.shxzukj.cn

[T55] Scala：集合过滤
来源：http://kf.gzmigu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qg.gzmigu.cn

[T56] Scala：样例类
来源：http://nt.colortex.cn

case class User(name: String, age: Int)
来源：http://zj.bookmarksfly.cn

[T57] Scala：模式匹配
来源：http://da.chemitech.net.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://af.nszjky.cn

[T58] Scala：函数定义
来源：http://aw.bookmarksfly.cn

def add(a: Int, b: Int): Int = a + b
来源：http://te.nicolike.cn

[T59] Scala：循环
来源：http://fo.szsharing.cn

for (i <- 1 to 10) println(i)
来源：http://oe.hnjuh.cn

[T60] Scala：折叠
来源：http://gc.yuntaijiaju.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://eo.nszjky.cn

================================================================================
来源：http://fc.asd995.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kj.shtwfgs.cn

================================================================================
来源：http://ql.huixiangedu.cn

[U01] Py：创建虚拟环境
来源：http://ne.panjiajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://kc.szxytkj.cn

[U02] Py：导出 / 安装依赖
来源：http://zu.lnxyls.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ku.szxytkj.cn

[U03] Py：加载 .env 配置
来源：http://jw.chemitech.net.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wa.nszjky.cn

[U04] Py：变量调试打印
来源：http://ay.jctech888.com.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lu.lnxyls.cn

[U05] Py：列表去重且保序
来源：http://uk.wgjwhj.cn

list(dict.fromkeys(arr))
来源：http://qs.panjiajie.cn

[U06] Py：合并两个字典
来源：http://jd.wgjwhj.cn

{**a, **b}
来源：http://sp.huanxung.cn

[U07] Py：反转字典键值
来源：http://oj.shtwfgs.cn

{v: k for k, v in d.items()}
来源：http://by.yuexingan06.cn

[U08] Py：展平二维列表
来源：http://sd.jctech888.com.cn

[y for x in nested for y in x]
来源：http://iv.chemitech.net.cn

[U09] Py：字典取最大值的键
来源：http://kf.haigaiapp.cn

max(d, key=d.get)
来源：http://hu.bjjhwx.cn

[U10] Py：按值排序字典
来源：http://tr.9csxet.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jb.yuexingan06.cn

[U11] Py：生成器表达式
来源：http://tf.gzmigu.cn

(x * 2 for x in arr)
来源：http://ll.huanxung.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mj.yuntaijiaju.cn

Counter(arr).most_common(3)
来源：http://iu.szxytkj.cn

[U13] Py：固定长度队列
来源：http://bg.gzmigu.cn

deque(maxlen=10)
来源：http://jp.lnxyls.cn

[U14] Py：分组收集到列表
来源：http://gv.chemitech.net.cn

defaultdict(list)
来源：http://xl.bjjhwx.cn

[U15] Py：高精度计时
来源：http://wk.muxihuayi.cn

t = time.perf_counter()
来源：http://ca.panjiajie.cn

[U16] Py：命令行参数解析
来源：http://ht.shxzukj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nd.haigaiapp.cn

[U17] Py：初始化日志
来源：http://yp.colortex.cn

logging.basicConfig(level=logging.INFO)
来源：http://yd.shtwfgs.cn

[U18] Py：预编译正则
来源：http://rw.shxzukj.cn

pat = re.compile(r"\d+")
来源：http://zi.huanxung.cn

[U19] Py：正则替换带回调
来源：http://sq.yuntaijiaju.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mg.haigaiapp.cn

[U20] Py：缓存函数结果
来源：http://pr.bjjhwx.cn

@functools.lru_cache(maxsize=None)
来源：http://lm.muxihuayi.cn

[U21] Py：自定义上下文管理器
来源：http://jr.521024.cn

@contextlib.contextmanager
来源：http://ct.chemitech.net.cn

[U22] Py：矩阵转置
来源：http://my.9csxet.cn

list(zip(*m))
来源：http://eu.9csxet.cn


<!-- 参考信息 -->