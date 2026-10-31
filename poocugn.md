代发 wailian999

S. C / C++ 专题
来源：http://iq.bjjhwx.cn

================================================================================
来源：http://xe.panjiajie.cn

[S01] C：Hello World
来源：http://bq.lnxyls.cn

#include <stdio.h>
来源：http://oy.huixiangedu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hg.panjiajie.cn

[S02] C：变量与格式化输出
来源：http://xm.jctech888.com.cn

int a = 10; printf("%d\n", a);
来源：http://si.szsharing.cn

[S03] C：读入整数
来源：http://ls.nszjky.cn

int x; scanf("%d", &x);
来源：http://vy.9csxet.cn

[S04] C：字符串复制
来源：http://xn.521024.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jy.yuntaijiaju.cn

[S05] C：字符串长度
来源：http://ll.shtwfgs.cn

strlen(s)
来源：http://zs.haigaiapp.cn

[S06] C：字符串比较
来源：http://sl.huixinmuqiang.cn

strcmp(a, b) == 0
来源：http://ub.chemitech.net.cn

[S07] C：数组遍历求和
来源：http://jd.newstarts.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rq.muxihuayi.cn

[S08] C：动态内存分配与释放
来源：http://qs.wgjwhj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ue.yuexingan06.cn

[S09] C：结构体定义与初始化
来源：http://sf.9csxet.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://px.521024.cn

[S10] C：指针与解引用
来源：http://nq.chemitech.net.cn

int *p = &a;  *p = 5;
来源：http://me.shxzskj.cn

[S11] C：逐行读文件
来源：http://so.chemitech.net.cn

FILE *f = fopen("a.txt", "r");
来源：http://ad.muxihuayi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://sy.jctech888.com.cn

fclose(f);
来源：http://le.9csxet.cn

[S12] C：写文件
来源：http://la.haigaiapp.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ie.bookmarksfly.cn

[S13] C：宏定义
来源：http://ar.muxihuayi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ta.shxzskj.cn

[S14] C：枚举
来源：http://od.shtwfgs.cn

enum Color { RED, GREEN, BLUE };
来源：http://fj.muxihuayi.cn

[S15] C：类型转换
来源：http://hv.colortex.cn

(double) a / b
来源：http://ps.haigaiapp.cn

[S16] C：位操作置位
来源：http://qx.newstarts.cn

x |= (1 << 3);
来源：http://vi.bjjhwx.cn

[S17] C：安全拼接字符串
来源：http://ab.szsharing.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zy.haigaiapp.cn

[S18] C：命令行参数
来源：http://ju.colortex.cn

int main(int argc, char **argv)
来源：http://mo.wgjwhj.cn

[S19] C：快速排序
来源：http://iy.9csxet.cn

qsort(a, n, sizeof(int), cmp);
来源：http://tq.huixiangedu.cn

[S20] C：二分查找
来源：http://dk.colortex.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xn.yuexingan06.cn

[S21] C：字符类别判断
来源：http://uz.yuntaijiaju.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://md.muxihuayi.cn

[S22] C：字符串转数字
来源：http://qw.newstarts.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qi.bjjhwx.cn

[S23] C：随机数
来源：http://yr.haigaiapp.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://gn.huixiangedu.cn

[S24] C：获取本地时间
来源：http://kj.haigaiapp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lh.yuntaijiaju.cn

[S25] C：内存拷贝
来源：http://sx.jianghongdianzi.cn

memcpy(dst, src, n);
来源：http://ij.newstarts.cn

[S26] C：内存清零
来源：http://fk.yuntaijiaju.cn

memset(a, 0, sizeof a);
来源：http://qr.panjiajie.cn

[S27] C：定义常量
来源：http://me.yuntaijiaju.cn

const double PI = 3.14159;
来源：http://qm.asd995.cn

[S28] C：静态变量
来源：http://sl.jianghongdianzi.cn

static int counter = 0;
来源：http://uj.521024.cn

[S29] C：变参函数
来源：http://nn.hahajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ow.jctech888.com.cn

[S30] C：头文件保护
来源：http://ed.nszjky.cn

#ifndef X_H
来源：http://zf.colortex.cn

#define X_H
来源：http://zh.bookmarksfly.cn

#endif
来源：http://xj.521024.cn

[S31] C++：Hello World
来源：http://xv.colortex.cn

#include <iostream>
来源：http://qs.nszjky.cn

int main() { std::cout << "Hello\n"; }
来源：http://yw.yuntaijiaju.cn

[S32] C++：字符串
来源：http://nt.colortex.cn

std::string s = "hi";  s += "!";
来源：http://ad.521024.cn

[S33] C++：vector 增删
来源：http://ad.muxihuayi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://iq.szsharing.cn

[S34] C++：遍历 vector
来源：http://er.bookmarksfly.cn

for (auto &x : v) { std::cout << x; }
来源：http://ta.huixinmuqiang.cn

[S35] C++：map
来源：http://pn.panjiajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://oy.huanxung.cn

[S36] C++：unordered_map
来源：http://eo.hahajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vh.gzmigu.cn

[S37] C++：set
来源：http://kt.huanxung.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zt.asd995.cn

[S38] C++：排序
来源：http://se.lnxyls.cn

std::sort(v.begin(), v.end());
来源：http://wu.yuexingan06.cn

[S39] C++：自定义比较器排序
来源：http://dw.huanxung.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bh.hnjuh.cn

[S40] C++：查找元素
来源：http://wh.wgjwhj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cz.nszjky.cn

[S41] C++：类与构造函数
来源：http://lt.shxzskj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bm.haigaiapp.cn

[S42] C++：继承与虚函数
来源：http://aq.haigaiapp.cn

class B : public Base { public: void f() override {} };
来源：http://kf.newstarts.cn

[S43] C++：智能指针
来源：http://tm.bjjhwx.cn

auto p = std::make_unique<int>(5);
来源：http://hl.szsharing.cn

[S44] C++：引用传参
来源：http://du.szxytkj.cn

void inc(int &x) { ++x; }
来源：http://hc.szsharing.cn

[S45] C++：lambda
来源：http://nv.asd995.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vu.asd995.cn

[S46] C++：函数模板
来源：http://as.nszjky.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ig.huixiangedu.cn

[S47] C++：结构化绑定遍历
来源：http://nn.wgjwhj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tt.9csxet.cn

[S48] C++：逐行读文件
来源：http://ix.gzmigu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ll.hahajie.cn

while (std::getline(in, line)) { }
来源：http://hm.huixinmuqiang.cn

[S49] C++：写文件
来源：http://yh.haigaiapp.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bs.colortex.cn

[S50] C++：格式化数字
来源：http://vj.panjiajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cz.colortex.cn

[S51] C++：显式类型转换
来源：http://xg.haigaiapp.cn

static_cast<double>(a) / b
来源：http://iy.nicolike.cn

[S52] C++：const 与 noexcept
来源：http://cq.jianghongdianzi.cn

int size() const noexcept { return n_; }
来源：http://vo.bookmarksfly.cn

[S53] C++：移动语义
来源：http://oo.yuntaijiaju.cn

std::vector<int> w = std::move(v);
来源：http://ig.huixiangedu.cn

[S54] C++：异常处理
来源：http://cm.szsharing.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zt.asd995.cn

[S55] C++：结构化绑定
来源：http://he.shxzskj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qs.szsharing.cn

[S56] C++：optional
来源：http://wn.nszjky.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ew.lnxyls.cn

[S57] C++：编译期常量
来源：http://br.9csxet.cn

constexpr int N = 10;
来源：http://ii.asd995.cn

[S58] C++：命名空间
来源：http://uu.9csxet.cn

namespace ns { int f() { return 1; } }
来源：http://dm.lnxyls.cn

[S59] C++：静态断言
来源：http://sk.panjiajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bh.yuexingan06.cn

[S60] C++：遍历并删除元素
来源：http://by.shxzukj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ut.9csxet.cn

================================================================================
来源：http://cb.huixinmuqiang.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://va.nicolike.cn

================================================================================
来源：http://cx.huixiangedu.cn

[T01] Kotlin：Hello World
来源：http://cv.hahajie.cn

println("Hello")
来源：http://fo.haigaiapp.cn

[T02] Kotlin：变量
来源：http://zx.bookmarksfly.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lz.huixinmuqiang.cn

[T03] Kotlin：字符串模板
来源：http://mj.yuntaijiaju.cn

"值: $b"
来源：http://iv.521024.cn

[T04] Kotlin：空安全
来源：http://rp.huixiangedu.cn

val n: String? = null;  n?.length
来源：http://wz.colortex.cn

[T05] Kotlin：when 表达式
来源：http://sz.szsharing.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bh.hnjuh.cn

[T06] Kotlin：集合映射
来源：http://no.szsharing.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gc.yuntaijiaju.cn

[T07] Kotlin：集合过滤
来源：http://hp.bjjhwx.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vc.shxzukj.cn

[T08] Kotlin：数据类
来源：http://cz.huixiangedu.cn

data class User(val name: String, val age: Int)
来源：http://oi.wgjwhj.cn

[T09] Kotlin：扩展函数
来源：http://gk.haigaiapp.cn

fun String.exclaim() = this + "!"
来源：http://aw.muxihuayi.cn

[T10] Kotlin：默认参数
来源：http://so.huanxung.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ef.asd995.cn

[T11] Kotlin：协程
来源：http://wf.muxihuayi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://pj.yuexingan06.cn

[T12] Kotlin：解构声明
来源：http://dv.muxihuayi.cn

val (a, b) = Pair(1, 2)
来源：http://zq.asd995.cn

[T13] Kotlin：只读 Map
来源：http://ca.nszjky.cn

val m = mapOf("a" to 1)
来源：http://ex.panjiajie.cn

[T14] Kotlin：循环
来源：http://gz.nicolike.cn

for (i in 1..10) println(i)
来源：http://bg.muxihuayi.cn

[T15] Kotlin：接口
来源：http://aa.shxzukj.cn

interface Shape { fun area(): Double }
来源：http://sm.newstarts.cn

[T16] Swift：Hello World
来源：http://im.shxzukj.cn

print("Hello")
来源：http://ef.shxzskj.cn

[T17] Swift：变量与常量
来源：http://bs.huixiangedu.cn

var a = 1;  let b = 2
来源：http://fs.shtwfgs.cn

[T18] Swift：字符串插值
来源：http://xm.yuexingan06.cn

"值: \(b)"
来源：http://kg.huanxung.cn

[T19] Swift：可选绑定
来源：http://ig.jianghongdianzi.cn

if let n = opt { print(n) }
来源：http://uy.bjjhwx.cn

[T20] Swift：数组操作
来源：http://zl.lnxyls.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xf.muxihuayi.cn

[T21] Swift：遍历
来源：http://pz.hnjuh.cn

for x in a { print(x) }
来源：http://pc.bjjhwx.cn

[T22] Swift：字典
来源：http://pb.wgjwhj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://td.huixiangedu.cn

[T23] Swift：函数
来源：http://rr.nicolike.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ol.huixiangedu.cn

[T24] Swift：闭包
来源：http://pr.yuntaijiaju.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://do.colortex.cn

[T25] Swift：结构体
来源：http://qx.huixiangedu.cn

struct P { var x: Int }
来源：http://vu.wgjwhj.cn

[T26] Swift：类与重写
来源：http://tt.nszjky.cn

class A: Base { override func f() {} }
来源：http://tu.shxzskj.cn

[T27] Swift：错误处理
来源：http://zp.shxzukj.cn

do { try f() } catch { print(error) }
来源：http://br.yuexingan06.cn

[T28] Swift：枚举
来源：http://pm.hahajie.cn

enum Color { case red, green }
来源：http://cj.jianghongdianzi.cn

[T29] Swift：guard 提前返回
来源：http://qa.jianghongdianzi.cn

guard let x = opt else { return }
来源：http://vu.nszjky.cn

[T30] Swift：协议
来源：http://th.szsharing.cn

protocol Shape { func area() -> Double }
来源：http://gi.chemitech.net.cn

[T31] Lua：Hello World
来源：http://om.asd995.cn

print("Hello")
来源：http://yf.yuntaijiaju.cn

[T32] Lua：局部变量
来源：http://no.jianghongdianzi.cn

local a = 1
来源：http://dp.9csxet.cn

[T33] Lua：表（数组）
来源：http://zs.huanxung.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ti.colortex.cn

[T34] Lua：遍历表
来源：http://zl.wgjwhj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vh.panjiajie.cn

[T35] Lua：字典表
来源：http://rd.shxzukj.cn

local d = { a = 1 };  d.b = 2
来源：http://oy.chemitech.net.cn

[T36] Lua：函数
来源：http://be.hnjuh.cn

function add(a, b) return a + b end
来源：http://lx.yuntaijiaju.cn

[T37] Lua：字符串拼接
来源：http://sy.hahajie.cn

"a" .. "b"
来源：http://mi.muxihuayi.cn

[T38] Lua：条件
来源：http://hy.hahajie.cn

if x > 0 then print("正") end
来源：http://cx.haigaiapp.cn

[T39] Lua：模式匹配
来源：http://ii.colortex.cn

string.find(s, "%d+")
来源：http://gy.gzmigu.cn

[T40] Lua：元表
来源：http://ok.wgjwhj.cn

setmetatable({}, { __index = base })
来源：http://nu.bookmarksfly.cn

[T41] Perl：Hello World
来源：http://kq.asd995.cn

print "Hello\n";
来源：http://hj.jctech888.com.cn

[T42] Perl：变量类型
来源：http://jr.yuntaijiaju.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mb.jctech888.com.cn

[T43] Perl：字符串插值
来源：http://hc.nicolike.cn

"值: $a"
来源：http://ek.chemitech.net.cn

[T44] Perl：条件
来源：http://zp.bjjhwx.cn

if ($a > 0) { print "正"; }
来源：http://wd.huanxung.cn

[T45] Perl：数组遍历
来源：http://tc.shxzukj.cn

for my $x (@arr) { print $x; }
来源：http://pa.shxzukj.cn

[T46] Perl：哈希操作
来源：http://ht.wgjwhj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ub.newstarts.cn

[T47] Perl：正则捕获
来源：http://gs.haigaiapp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://fv.huixiangedu.cn

[T48] Perl：正则替换
来源：http://zi.huixinmuqiang.cn

$s =~ s/old/new/g;
来源：http://yc.newstarts.cn

[T49] Perl：函数
来源：http://yx.yuntaijiaju.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mg.yuntaijiaju.cn

[T50] Perl：逐行读文件
来源：http://ob.huixinmuqiang.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xz.huixinmuqiang.cn

while (my $line = <$fh>) { print $line; }
来源：http://yk.shtwfgs.cn

[T51] Scala：Hello World
来源：http://um.jctech888.com.cn

println("Hello")
来源：http://qk.colortex.cn

[T52] Scala：变量
来源：http://ah.newstarts.cn

val a = 1;  var b = 2
来源：http://ey.yuntaijiaju.cn

[T53] Scala：字符串插值
来源：http://kg.shxzskj.cn

s"值: $b"
来源：http://qy.shxzukj.cn

[T54] Scala：集合映射
来源：http://qt.shxzukj.cn

List(1, 2, 3).map(_ * 2)
来源：http://rj.huixiangedu.cn

[T55] Scala：集合过滤
来源：http://jz.bookmarksfly.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wl.muxihuayi.cn

[T56] Scala：样例类
来源：http://qb.szxytkj.cn

case class User(name: String, age: Int)
来源：http://gw.huanxung.cn

[T57] Scala：模式匹配
来源：http://hq.szsharing.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ya.wgjwhj.cn

[T58] Scala：函数定义
来源：http://mw.521024.cn

def add(a: Int, b: Int): Int = a + b
来源：http://kt.huixiangedu.cn

[T59] Scala：循环
来源：http://ga.yuexingan06.cn

for (i <- 1 to 10) println(i)
来源：http://ny.shxzukj.cn

[T60] Scala：折叠
来源：http://vq.newstarts.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ck.nszjky.cn

================================================================================
来源：http://zu.hnjuh.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yw.nszjky.cn

================================================================================
来源：http://hx.szxytkj.cn

[U01] Py：创建虚拟环境
来源：http://ek.9csxet.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zy.shtwfgs.cn

[U02] Py：导出 / 安装依赖
来源：http://rb.nszjky.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://il.521024.cn

[U03] Py：加载 .env 配置
来源：http://ju.jctech888.com.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qq.hnjuh.cn

[U04] Py：变量调试打印
来源：http://fb.yuexingan06.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cu.muxihuayi.cn

[U05] Py：列表去重且保序
来源：http://ie.panjiajie.cn

list(dict.fromkeys(arr))
来源：http://lt.haigaiapp.cn

[U06] Py：合并两个字典
来源：http://oq.huanxung.cn

{**a, **b}
来源：http://jg.szxytkj.cn

[U07] Py：反转字典键值
来源：http://ev.bjjhwx.cn

{v: k for k, v in d.items()}
来源：http://dk.huixinmuqiang.cn

[U08] Py：展平二维列表
来源：http://th.shxzskj.cn

[y for x in nested for y in x]
来源：http://aj.asd995.cn

[U09] Py：字典取最大值的键
来源：http://zx.521024.cn

max(d, key=d.get)
来源：http://yd.huixinmuqiang.cn

[U10] Py：按值排序字典
来源：http://hc.colortex.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bd.haigaiapp.cn

[U11] Py：生成器表达式
来源：http://tt.jianghongdianzi.cn

(x * 2 for x in arr)
来源：http://jq.panjiajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://tk.haigaiapp.cn

Counter(arr).most_common(3)
来源：http://dx.chemitech.net.cn

[U13] Py：固定长度队列
来源：http://ds.haigaiapp.cn

deque(maxlen=10)
来源：http://xv.yuntaijiaju.cn

[U14] Py：分组收集到列表
来源：http://rv.shxzskj.cn

defaultdict(list)
来源：http://gm.jianghongdianzi.cn

[U15] Py：高精度计时
来源：http://nm.chemitech.net.cn

t = time.perf_counter()
来源：http://xt.gzmigu.cn

[U16] Py：命令行参数解析
来源：http://mt.asd995.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cb.jianghongdianzi.cn

[U17] Py：初始化日志
来源：http://zo.shxzukj.cn

logging.basicConfig(level=logging.INFO)
来源：http://bb.shxzskj.cn

[U18] Py：预编译正则
来源：http://nb.bookmarksfly.cn

pat = re.compile(r"\d+")
来源：http://ij.521024.cn

[U19] Py：正则替换带回调
来源：http://bv.hnjuh.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vm.yuntaijiaju.cn

[U20] Py：缓存函数结果
来源：http://xc.yuntaijiaju.cn

@functools.lru_cache(maxsize=None)
来源：http://sm.wgjwhj.cn

[U21] Py：自定义上下文管理器
来源：http://ox.colortex.cn

@contextlib.contextmanager
来源：http://ux.shxzskj.cn

[U22] Py：矩阵转置
来源：http://hz.chemitech.net.cn

list(zip(*m))
来源：http://hs.gzmigu.cn


<!-- 参考信息 -->