代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://na.jctech888.com.cn

[R80] 查看脚本执行耗时
来源：http://sh.asd995.cn

time ./run.sh
来源：http://pc.hnjuh.cn

================================================================================
来源：http://ft.yuntaijiaju.cn

S. C / C++ 专题
来源：http://wm.nszjky.cn

================================================================================
来源：http://sx.yuntaijiaju.cn

[S01] C：Hello World
来源：http://rx.yuexingan06.cn

#include <stdio.h>
来源：http://ja.jctech888.com.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fp.jianghongdianzi.cn

[S02] C：变量与格式化输出
来源：http://da.jctech888.com.cn

int a = 10; printf("%d\n", a);
来源：http://vm.haigaiapp.cn

[S03] C：读入整数
来源：http://to.lnxyls.cn

int x; scanf("%d", &x);
来源：http://ad.9csxet.cn

[S04] C：字符串复制
来源：http://ps.huixinmuqiang.cn

char dst[32]; strcpy(dst, "hi");
来源：http://sa.huixinmuqiang.cn

[S05] C：字符串长度
来源：http://kt.nicolike.cn

strlen(s)
来源：http://wu.shtwfgs.cn

[S06] C：字符串比较
来源：http://vj.panjiajie.cn

strcmp(a, b) == 0
来源：http://ev.haigaiapp.cn

[S07] C：数组遍历求和
来源：http://jv.jianghongdianzi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zi.colortex.cn

[S08] C：动态内存分配与释放
来源：http://ku.lnxyls.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zt.jctech888.com.cn

[S09] C：结构体定义与初始化
来源：http://tm.muxihuayi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jt.hnjuh.cn

[S10] C：指针与解引用
来源：http://iv.panjiajie.cn

int *p = &a;  *p = 5;
来源：http://df.asd995.cn

[S11] C：逐行读文件
来源：http://ox.gzmigu.cn

FILE *f = fopen("a.txt", "r");
来源：http://cx.shxzskj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fu.yuntaijiaju.cn

fclose(f);
来源：http://dc.bookmarksfly.cn

[S12] C：写文件
来源：http://yh.9csxet.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kc.huixiangedu.cn

[S13] C：宏定义
来源：http://qz.shxzskj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cw.huanxung.cn

[S14] C：枚举
来源：http://qg.newstarts.cn

enum Color { RED, GREEN, BLUE };
来源：http://xf.bjjhwx.cn

[S15] C：类型转换
来源：http://oi.chemitech.net.cn

(double) a / b
来源：http://ox.panjiajie.cn

[S16] C：位操作置位
来源：http://wn.asd995.cn

x |= (1 << 3);
来源：http://pg.shxzskj.cn

[S17] C：安全拼接字符串
来源：http://hl.wgjwhj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xp.hahajie.cn

[S18] C：命令行参数
来源：http://df.newstarts.cn

int main(int argc, char **argv)
来源：http://cu.gzmigu.cn

[S19] C：快速排序
来源：http://vg.nicolike.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xb.gzmigu.cn

[S20] C：二分查找
来源：http://ir.hahajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mc.shtwfgs.cn

[S21] C：字符类别判断
来源：http://ug.jctech888.com.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rt.bookmarksfly.cn

[S22] C：字符串转数字
来源：http://ud.hnjuh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ja.shxzukj.cn

[S23] C：随机数
来源：http://bb.hnjuh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hm.huixinmuqiang.cn

[S24] C：获取本地时间
来源：http://wo.bjjhwx.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mx.bookmarksfly.cn

[S25] C：内存拷贝
来源：http://ih.521024.cn

memcpy(dst, src, n);
来源：http://vr.chemitech.net.cn

[S26] C：内存清零
来源：http://dg.huanxung.cn

memset(a, 0, sizeof a);
来源：http://hw.newstarts.cn

[S27] C：定义常量
来源：http://ja.szxytkj.cn

const double PI = 3.14159;
来源：http://jc.yuntaijiaju.cn

[S28] C：静态变量
来源：http://sg.hnjuh.cn

static int counter = 0;
来源：http://dq.panjiajie.cn

[S29] C：变参函数
来源：http://vy.9csxet.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fa.hahajie.cn

[S30] C：头文件保护
来源：http://da.nicolike.cn

#ifndef X_H
来源：http://oa.nicolike.cn

#define X_H
来源：http://ej.lnxyls.cn

#endif
来源：http://ul.nicolike.cn

[S31] C++：Hello World
来源：http://aa.hnjuh.cn

#include <iostream>
来源：http://ny.nicolike.cn

int main() { std::cout << "Hello\n"; }
来源：http://hv.huixinmuqiang.cn

[S32] C++：字符串
来源：http://tx.jianghongdianzi.cn

std::string s = "hi";  s += "!";
来源：http://oh.521024.cn

[S33] C++：vector 增删
来源：http://oi.colortex.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ph.shxzukj.cn

[S34] C++：遍历 vector
来源：http://no.bookmarksfly.cn

for (auto &x : v) { std::cout << x; }
来源：http://pn.yuntaijiaju.cn

[S35] C++：map
来源：http://hs.shxzukj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rz.haigaiapp.cn

[S36] C++：unordered_map
来源：http://vf.huixiangedu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zy.gzmigu.cn

[S37] C++：set
来源：http://yu.asd995.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kw.szxytkj.cn

[S38] C++：排序
来源：http://il.lnxyls.cn

std::sort(v.begin(), v.end());
来源：http://cs.hahajie.cn

[S39] C++：自定义比较器排序
来源：http://gy.hnjuh.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nf.colortex.cn

[S40] C++：查找元素
来源：http://qx.521024.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vq.newstarts.cn

[S41] C++：类与构造函数
来源：http://sd.yuntaijiaju.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oy.asd995.cn

[S42] C++：继承与虚函数
来源：http://up.9csxet.cn

class B : public Base { public: void f() override {} };
来源：http://dw.yuexingan06.cn

[S43] C++：智能指针
来源：http://ap.haigaiapp.cn

auto p = std::make_unique<int>(5);
来源：http://ht.lnxyls.cn

[S44] C++：引用传参
来源：http://lt.szsharing.cn

void inc(int &x) { ++x; }
来源：http://kh.yuntaijiaju.cn

[S45] C++：lambda
来源：http://yo.colortex.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ul.nszjky.cn

[S46] C++：函数模板
来源：http://ji.lnxyls.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bs.shxzskj.cn

[S47] C++：结构化绑定遍历
来源：http://ax.jianghongdianzi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zb.huanxung.cn

[S48] C++：逐行读文件
来源：http://ax.muxihuayi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://hp.shxzskj.cn

while (std::getline(in, line)) { }
来源：http://vc.hnjuh.cn

[S49] C++：写文件
来源：http://st.bjjhwx.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ln.haigaiapp.cn

[S50] C++：格式化数字
来源：http://hf.szsharing.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kz.yuexingan06.cn

[S51] C++：显式类型转换
来源：http://mj.szxytkj.cn

static_cast<double>(a) / b
来源：http://pu.hahajie.cn

[S52] C++：const 与 noexcept
来源：http://xb.szxytkj.cn

int size() const noexcept { return n_; }
来源：http://cu.nicolike.cn

[S53] C++：移动语义
来源：http://zn.shtwfgs.cn

std::vector<int> w = std::move(v);
来源：http://wv.9csxet.cn

[S54] C++：异常处理
来源：http://zm.bjjhwx.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wt.bjjhwx.cn

[S55] C++：结构化绑定
来源：http://dq.huixinmuqiang.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://av.jctech888.com.cn

[S56] C++：optional
来源：http://ts.shtwfgs.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lp.huixiangedu.cn

[S57] C++：编译期常量
来源：http://ys.521024.cn

constexpr int N = 10;
来源：http://xf.huixiangedu.cn

[S58] C++：命名空间
来源：http://zm.newstarts.cn

namespace ns { int f() { return 1; } }
来源：http://sg.huixinmuqiang.cn

[S59] C++：静态断言
来源：http://at.jianghongdianzi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ei.colortex.cn

[S60] C++：遍历并删除元素
来源：http://im.521024.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rn.shtwfgs.cn

================================================================================
来源：http://ig.shxzukj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lt.muxihuayi.cn

================================================================================
来源：http://os.bookmarksfly.cn

[T01] Kotlin：Hello World
来源：http://jh.colortex.cn

println("Hello")
来源：http://dm.jianghongdianzi.cn

[T02] Kotlin：变量
来源：http://ry.shxzukj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ch.9csxet.cn

[T03] Kotlin：字符串模板
来源：http://kn.newstarts.cn

"值: $b"
来源：http://wi.huixinmuqiang.cn

[T04] Kotlin：空安全
来源：http://nj.yuexingan06.cn

val n: String? = null;  n?.length
来源：http://vb.nicolike.cn

[T05] Kotlin：when 表达式
来源：http://hv.chemitech.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fx.yuexingan06.cn

[T06] Kotlin：集合映射
来源：http://wz.wgjwhj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ns.jctech888.com.cn

[T07] Kotlin：集合过滤
来源：http://ck.panjiajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://or.shxzskj.cn

[T08] Kotlin：数据类
来源：http://hz.huixinmuqiang.cn

data class User(val name: String, val age: Int)
来源：http://jb.panjiajie.cn

[T09] Kotlin：扩展函数
来源：http://dd.huixiangedu.cn

fun String.exclaim() = this + "!"
来源：http://eb.colortex.cn

[T10] Kotlin：默认参数
来源：http://wm.9csxet.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://we.wgjwhj.cn

[T11] Kotlin：协程
来源：http://wl.hnjuh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ou.huixinmuqiang.cn

[T12] Kotlin：解构声明
来源：http://dw.szxytkj.cn

val (a, b) = Pair(1, 2)
来源：http://wr.nszjky.cn

[T13] Kotlin：只读 Map
来源：http://kc.newstarts.cn

val m = mapOf("a" to 1)
来源：http://sa.nszjky.cn

[T14] Kotlin：循环
来源：http://dm.newstarts.cn

for (i in 1..10) println(i)
来源：http://et.bjjhwx.cn

[T15] Kotlin：接口
来源：http://rr.wgjwhj.cn

interface Shape { fun area(): Double }
来源：http://wj.jianghongdianzi.cn

[T16] Swift：Hello World
来源：http://nk.szsharing.cn

print("Hello")
来源：http://bg.huixinmuqiang.cn

[T17] Swift：变量与常量
来源：http://su.newstarts.cn

var a = 1;  let b = 2
来源：http://dy.huixiangedu.cn

[T18] Swift：字符串插值
来源：http://ck.gzmigu.cn

"值: \(b)"
来源：http://el.huixinmuqiang.cn

[T19] Swift：可选绑定
来源：http://ft.colortex.cn

if let n = opt { print(n) }
来源：http://yg.huixinmuqiang.cn

[T20] Swift：数组操作
来源：http://fa.panjiajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ig.jianghongdianzi.cn

[T21] Swift：遍历
来源：http://dw.nicolike.cn

for x in a { print(x) }
来源：http://ry.lnxyls.cn

[T22] Swift：字典
来源：http://wd.colortex.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xn.bjjhwx.cn

[T23] Swift：函数
来源：http://ij.shtwfgs.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uc.newstarts.cn

[T24] Swift：闭包
来源：http://uz.shtwfgs.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qs.521024.cn

[T25] Swift：结构体
来源：http://pq.chemitech.net.cn

struct P { var x: Int }
来源：http://vu.huixiangedu.cn

[T26] Swift：类与重写
来源：http://jp.panjiajie.cn

class A: Base { override func f() {} }
来源：http://wh.gzmigu.cn

[T27] Swift：错误处理
来源：http://nw.jianghongdianzi.cn

do { try f() } catch { print(error) }
来源：http://xd.521024.cn

[T28] Swift：枚举
来源：http://za.shxzukj.cn

enum Color { case red, green }
来源：http://ca.521024.cn

[T29] Swift：guard 提前返回
来源：http://sl.huixinmuqiang.cn

guard let x = opt else { return }
来源：http://xk.szsharing.cn

[T30] Swift：协议
来源：http://lu.huanxung.cn

protocol Shape { func area() -> Double }
来源：http://bv.szsharing.cn

[T31] Lua：Hello World
来源：http://rf.yuexingan06.cn

print("Hello")
来源：http://jp.wgjwhj.cn

[T32] Lua：局部变量
来源：http://jw.haigaiapp.cn

local a = 1
来源：http://lh.bookmarksfly.cn

[T33] Lua：表（数组）
来源：http://yx.szsharing.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xd.szsharing.cn

[T34] Lua：遍历表
来源：http://uu.521024.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://bf.wgjwhj.cn

[T35] Lua：字典表
来源：http://pl.huixinmuqiang.cn

local d = { a = 1 };  d.b = 2
来源：http://po.lnxyls.cn

[T36] Lua：函数
来源：http://dj.yuntaijiaju.cn

function add(a, b) return a + b end
来源：http://yr.521024.cn

[T37] Lua：字符串拼接
来源：http://fj.wgjwhj.cn

"a" .. "b"
来源：http://ds.shxzskj.cn

[T38] Lua：条件
来源：http://gx.gzmigu.cn

if x > 0 then print("正") end
来源：http://yd.hnjuh.cn

[T39] Lua：模式匹配
来源：http://nm.szsharing.cn

string.find(s, "%d+")
来源：http://rc.huanxung.cn

[T40] Lua：元表
来源：http://aj.yuexingan06.cn

setmetatable({}, { __index = base })
来源：http://oa.lnxyls.cn

[T41] Perl：Hello World
来源：http://qx.shxzskj.cn

print "Hello\n";
来源：http://ny.jianghongdianzi.cn

[T42] Perl：变量类型
来源：http://pe.colortex.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wo.szxytkj.cn

[T43] Perl：字符串插值
来源：http://wx.wgjwhj.cn

"值: $a"
来源：http://uw.yuexingan06.cn

[T44] Perl：条件
来源：http://gn.asd995.cn

if ($a > 0) { print "正"; }
来源：http://qg.colortex.cn

[T45] Perl：数组遍历
来源：http://ug.szsharing.cn

for my $x (@arr) { print $x; }
来源：http://df.chemitech.net.cn

[T46] Perl：哈希操作
来源：http://iy.521024.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ay.shxzskj.cn

[T47] Perl：正则捕获
来源：http://ib.szsharing.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ix.szxytkj.cn

[T48] Perl：正则替换
来源：http://eu.lnxyls.cn

$s =~ s/old/new/g;
来源：http://au.yuntaijiaju.cn

[T49] Perl：函数
来源：http://hv.9csxet.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pf.lnxyls.cn

[T50] Perl：逐行读文件
来源：http://yg.gzmigu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://me.shxzukj.cn

while (my $line = <$fh>) { print $line; }
来源：http://fx.9csxet.cn

[T51] Scala：Hello World
来源：http://yl.colortex.cn

println("Hello")
来源：http://mx.bjjhwx.cn

[T52] Scala：变量
来源：http://ik.9csxet.cn

val a = 1;  var b = 2
来源：http://rd.bjjhwx.cn

[T53] Scala：字符串插值
来源：http://gi.wgjwhj.cn

s"值: $b"
来源：http://ll.szsharing.cn

[T54] Scala：集合映射
来源：http://sj.521024.cn

List(1, 2, 3).map(_ * 2)
来源：http://jw.huixinmuqiang.cn

[T55] Scala：集合过滤
来源：http://vw.shxzukj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ev.haigaiapp.cn

[T56] Scala：样例类
来源：http://im.nicolike.cn

case class User(name: String, age: Int)
来源：http://bo.asd995.cn

[T57] Scala：模式匹配
来源：http://yj.lnxyls.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://zk.nicolike.cn

[T58] Scala：函数定义
来源：http://oj.shtwfgs.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ku.shxzskj.cn

[T59] Scala：循环
来源：http://tt.jctech888.com.cn

for (i <- 1 to 10) println(i)
来源：http://sb.521024.cn

[T60] Scala：折叠
来源：http://br.asd995.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qf.wgjwhj.cn

================================================================================
来源：http://bv.nszjky.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zd.521024.cn

================================================================================
来源：http://qq.shxzskj.cn

[U01] Py：创建虚拟环境
来源：http://lg.jianghongdianzi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://lz.szxytkj.cn

[U02] Py：导出 / 安装依赖
来源：http://ux.bjjhwx.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gu.huixiangedu.cn

[U03] Py：加载 .env 配置
来源：http://zy.hnjuh.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wz.shxzukj.cn

[U04] Py：变量调试打印
来源：http://lo.yuntaijiaju.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dh.nicolike.cn

[U05] Py：列表去重且保序
来源：http://oe.huixinmuqiang.cn

list(dict.fromkeys(arr))
来源：http://dx.9csxet.cn

[U06] Py：合并两个字典
来源：http://sn.panjiajie.cn

{**a, **b}
来源：http://zc.yuntaijiaju.cn

[U07] Py：反转字典键值
来源：http://ov.jianghongdianzi.cn

{v: k for k, v in d.items()}
来源：http://vc.shtwfgs.cn

[U08] Py：展平二维列表
来源：http://va.nszjky.cn

[y for x in nested for y in x]
来源：http://ct.huixiangedu.cn

[U09] Py：字典取最大值的键
来源：http://pe.colortex.cn

max(d, key=d.get)
来源：http://gc.shtwfgs.cn

[U10] Py：按值排序字典
来源：http://nc.hahajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yq.bjjhwx.cn

[U11] Py：生成器表达式
来源：http://aj.hahajie.cn

(x * 2 for x in arr)
来源：http://jl.bjjhwx.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zx.521024.cn

Counter(arr).most_common(3)
来源：http://ea.lnxyls.cn

[U13] Py：固定长度队列
来源：http://az.hahajie.cn

deque(maxlen=10)
来源：http://rf.gzmigu.cn

[U14] Py：分组收集到列表
来源：http://sb.newstarts.cn

defaultdict(list)
来源：http://oq.shtwfgs.cn

[U15] Py：高精度计时
来源：http://wi.shxzukj.cn

t = time.perf_counter()
来源：http://gd.colortex.cn

[U16] Py：命令行参数解析
来源：http://nm.huixiangedu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mm.muxihuayi.cn

[U17] Py：初始化日志
来源：http://hp.shtwfgs.cn

logging.basicConfig(level=logging.INFO)
来源：http://nc.szxytkj.cn

[U18] Py：预编译正则
来源：http://wf.bjjhwx.cn

pat = re.compile(r"\d+")
来源：http://vz.gzmigu.cn

[U19] Py：正则替换带回调
来源：http://ab.9csxet.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://os.nicolike.cn

[U20] Py：缓存函数结果
来源：http://te.newstarts.cn

@functools.lru_cache(maxsize=None)
来源：http://dt.huixiangedu.cn


<!-- 参考信息 -->