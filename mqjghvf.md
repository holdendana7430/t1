代发 wailian999

S. C / C++ 专题
来源：http://ih.bjjhwx.cn

================================================================================
来源：http://hb.gzmigu.cn

[S01] C：Hello World
来源：http://xf.shxzskj.cn

#include <stdio.h>
来源：http://oy.hahajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fm.bookmarksfly.cn

[S02] C：变量与格式化输出
来源：http://up.asd995.cn

int a = 10; printf("%d\n", a);
来源：http://ix.shxzukj.cn

[S03] C：读入整数
来源：http://tn.hnjuh.cn

int x; scanf("%d", &x);
来源：http://at.shxzukj.cn

[S04] C：字符串复制
来源：http://nb.huanxung.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pp.huixiangedu.cn

[S05] C：字符串长度
来源：http://gj.haigaiapp.cn

strlen(s)
来源：http://yt.shtwfgs.cn

[S06] C：字符串比较
来源：http://gi.yuexingan06.cn

strcmp(a, b) == 0
来源：http://me.jctech888.com.cn

[S07] C：数组遍历求和
来源：http://qd.nszjky.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zp.lnxyls.cn

[S08] C：动态内存分配与释放
来源：http://yk.haigaiapp.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zz.jianghongdianzi.cn

[S09] C：结构体定义与初始化
来源：http://mh.nszjky.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uh.colortex.cn

[S10] C：指针与解引用
来源：http://xr.colortex.cn

int *p = &a;  *p = 5;
来源：http://wp.szsharing.cn

[S11] C：逐行读文件
来源：http://di.shxzukj.cn

FILE *f = fopen("a.txt", "r");
来源：http://iu.shtwfgs.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ml.shxzukj.cn

fclose(f);
来源：http://ao.chemitech.net.cn

[S12] C：写文件
来源：http://cn.gzmigu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kd.panjiajie.cn

[S13] C：宏定义
来源：http://rw.jctech888.com.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gv.huanxung.cn

[S14] C：枚举
来源：http://yl.szsharing.cn

enum Color { RED, GREEN, BLUE };
来源：http://yc.newstarts.cn

[S15] C：类型转换
来源：http://ce.szxytkj.cn

(double) a / b
来源：http://fk.jctech888.com.cn

[S16] C：位操作置位
来源：http://bv.hahajie.cn

x |= (1 << 3);
来源：http://mb.shxzskj.cn

[S17] C：安全拼接字符串
来源：http://ny.521024.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qs.bookmarksfly.cn

[S18] C：命令行参数
来源：http://wa.huixinmuqiang.cn

int main(int argc, char **argv)
来源：http://qc.hnjuh.cn

[S19] C：快速排序
来源：http://gj.nszjky.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ho.yuexingan06.cn

[S20] C：二分查找
来源：http://ij.hahajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wu.nszjky.cn

[S21] C：字符类别判断
来源：http://ih.jctech888.com.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tk.huixinmuqiang.cn

[S22] C：字符串转数字
来源：http://ny.jianghongdianzi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gl.gzmigu.cn

[S23] C：随机数
来源：http://by.colortex.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://yo.huixinmuqiang.cn

[S24] C：获取本地时间
来源：http://ia.panjiajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yn.asd995.cn

[S25] C：内存拷贝
来源：http://ef.hahajie.cn

memcpy(dst, src, n);
来源：http://vn.colortex.cn

[S26] C：内存清零
来源：http://cs.szsharing.cn

memset(a, 0, sizeof a);
来源：http://tc.nicolike.cn

[S27] C：定义常量
来源：http://vr.shxzskj.cn

const double PI = 3.14159;
来源：http://hs.huixinmuqiang.cn

[S28] C：静态变量
来源：http://yl.bjjhwx.cn

static int counter = 0;
来源：http://fq.jctech888.com.cn

[S29] C：变参函数
来源：http://pq.yuntaijiaju.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ne.bjjhwx.cn

[S30] C：头文件保护
来源：http://lu.hahajie.cn

#ifndef X_H
来源：http://ha.chemitech.net.cn

#define X_H
来源：http://hx.shxzskj.cn

#endif
来源：http://ye.szxytkj.cn

[S31] C++：Hello World
来源：http://po.gzmigu.cn

#include <iostream>
来源：http://pu.colortex.cn

int main() { std::cout << "Hello\n"; }
来源：http://xt.nicolike.cn

[S32] C++：字符串
来源：http://so.newstarts.cn

std::string s = "hi";  s += "!";
来源：http://yu.hahajie.cn

[S33] C++：vector 增删
来源：http://xo.shxzskj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rz.panjiajie.cn

[S34] C++：遍历 vector
来源：http://nj.szsharing.cn

for (auto &x : v) { std::cout << x; }
来源：http://eg.colortex.cn

[S35] C++：map
来源：http://zr.szsharing.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://km.colortex.cn

[S36] C++：unordered_map
来源：http://dh.shxzskj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xo.nszjky.cn

[S37] C++：set
来源：http://nx.jianghongdianzi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zd.shtwfgs.cn

[S38] C++：排序
来源：http://go.shxzukj.cn

std::sort(v.begin(), v.end());
来源：http://zw.bjjhwx.cn

[S39] C++：自定义比较器排序
来源：http://ov.wgjwhj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sf.haigaiapp.cn

[S40] C++：查找元素
来源：http://sr.yuntaijiaju.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jh.huanxung.cn

[S41] C++：类与构造函数
来源：http://qs.haigaiapp.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nx.bookmarksfly.cn

[S42] C++：继承与虚函数
来源：http://zz.szsharing.cn

class B : public Base { public: void f() override {} };
来源：http://ib.szsharing.cn

[S43] C++：智能指针
来源：http://dv.bookmarksfly.cn

auto p = std::make_unique<int>(5);
来源：http://rn.colortex.cn

[S44] C++：引用传参
来源：http://dp.nicolike.cn

void inc(int &x) { ++x; }
来源：http://ym.szsharing.cn

[S45] C++：lambda
来源：http://bt.jianghongdianzi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qg.lnxyls.cn

[S46] C++：函数模板
来源：http://yv.hnjuh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vy.yuexingan06.cn

[S47] C++：结构化绑定遍历
来源：http://sz.jctech888.com.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gj.yuexingan06.cn

[S48] C++：逐行读文件
来源：http://xj.9csxet.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gn.haigaiapp.cn

while (std::getline(in, line)) { }
来源：http://ip.szxytkj.cn

[S49] C++：写文件
来源：http://xs.shtwfgs.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tw.yuntaijiaju.cn

[S50] C++：格式化数字
来源：http://fl.panjiajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://iu.szsharing.cn

[S51] C++：显式类型转换
来源：http://sn.hnjuh.cn

static_cast<double>(a) / b
来源：http://ir.asd995.cn

[S52] C++：const 与 noexcept
来源：http://ha.huixiangedu.cn

int size() const noexcept { return n_; }
来源：http://wf.jianghongdianzi.cn

[S53] C++：移动语义
来源：http://ne.newstarts.cn

std::vector<int> w = std::move(v);
来源：http://uk.panjiajie.cn

[S54] C++：异常处理
来源：http://pc.lnxyls.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dr.huixinmuqiang.cn

[S55] C++：结构化绑定
来源：http://nt.chemitech.net.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qw.bookmarksfly.cn

[S56] C++：optional
来源：http://mb.521024.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zm.newstarts.cn

[S57] C++：编译期常量
来源：http://wf.huixinmuqiang.cn

constexpr int N = 10;
来源：http://bd.szxytkj.cn

[S58] C++：命名空间
来源：http://ol.chemitech.net.cn

namespace ns { int f() { return 1; } }
来源：http://dx.haigaiapp.cn

[S59] C++：静态断言
来源：http://my.shxzukj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vo.9csxet.cn

[S60] C++：遍历并删除元素
来源：http://vz.gzmigu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ep.huanxung.cn

================================================================================
来源：http://zy.521024.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ie.huixiangedu.cn

================================================================================
来源：http://xn.shxzukj.cn

[T01] Kotlin：Hello World
来源：http://yo.yuexingan06.cn

println("Hello")
来源：http://dc.nicolike.cn

[T02] Kotlin：变量
来源：http://xw.yuexingan06.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xt.9csxet.cn

[T03] Kotlin：字符串模板
来源：http://ps.haigaiapp.cn

"值: $b"
来源：http://wo.jctech888.com.cn

[T04] Kotlin：空安全
来源：http://at.wgjwhj.cn

val n: String? = null;  n?.length
来源：http://pz.haigaiapp.cn

[T05] Kotlin：when 表达式
来源：http://xy.shtwfgs.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xt.lnxyls.cn

[T06] Kotlin：集合映射
来源：http://if.haigaiapp.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rk.gzmigu.cn

[T07] Kotlin：集合过滤
来源：http://xh.wgjwhj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://gw.jctech888.com.cn

[T08] Kotlin：数据类
来源：http://cm.muxihuayi.cn

data class User(val name: String, val age: Int)
来源：http://iu.asd995.cn

[T09] Kotlin：扩展函数
来源：http://vp.nicolike.cn

fun String.exclaim() = this + "!"
来源：http://qi.shtwfgs.cn

[T10] Kotlin：默认参数
来源：http://gm.haigaiapp.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pq.muxihuayi.cn

[T11] Kotlin：协程
来源：http://cq.wgjwhj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://dq.szsharing.cn

[T12] Kotlin：解构声明
来源：http://tb.panjiajie.cn

val (a, b) = Pair(1, 2)
来源：http://br.wgjwhj.cn

[T13] Kotlin：只读 Map
来源：http://te.jianghongdianzi.cn

val m = mapOf("a" to 1)
来源：http://oz.shtwfgs.cn

[T14] Kotlin：循环
来源：http://he.shtwfgs.cn

for (i in 1..10) println(i)
来源：http://np.szsharing.cn

[T15] Kotlin：接口
来源：http://jk.yuntaijiaju.cn

interface Shape { fun area(): Double }
来源：http://nd.lnxyls.cn

[T16] Swift：Hello World
来源：http://gm.jianghongdianzi.cn

print("Hello")
来源：http://nk.shxzskj.cn

[T17] Swift：变量与常量
来源：http://ex.shxzukj.cn

var a = 1;  let b = 2
来源：http://sk.shxzskj.cn

[T18] Swift：字符串插值
来源：http://ou.521024.cn

"值: \(b)"
来源：http://py.huixinmuqiang.cn

[T19] Swift：可选绑定
来源：http://ev.jctech888.com.cn

if let n = opt { print(n) }
来源：http://pv.gzmigu.cn

[T20] Swift：数组操作
来源：http://xo.bookmarksfly.cn

var a = [1, 2, 3];  a.append(4)
来源：http://bx.hnjuh.cn

[T21] Swift：遍历
来源：http://aj.hahajie.cn

for x in a { print(x) }
来源：http://ti.hnjuh.cn

[T22] Swift：字典
来源：http://aj.bjjhwx.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ru.nszjky.cn

[T23] Swift：函数
来源：http://mb.521024.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://oa.huixinmuqiang.cn

[T24] Swift：闭包
来源：http://nw.hnjuh.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://jz.hnjuh.cn

[T25] Swift：结构体
来源：http://kg.bjjhwx.cn

struct P { var x: Int }
来源：http://yx.asd995.cn

[T26] Swift：类与重写
来源：http://tx.chemitech.net.cn

class A: Base { override func f() {} }
来源：http://qa.yuntaijiaju.cn

[T27] Swift：错误处理
来源：http://gw.lnxyls.cn

do { try f() } catch { print(error) }
来源：http://pr.shxzukj.cn

[T28] Swift：枚举
来源：http://nr.jianghongdianzi.cn

enum Color { case red, green }
来源：http://ye.muxihuayi.cn

[T29] Swift：guard 提前返回
来源：http://sq.521024.cn

guard let x = opt else { return }
来源：http://yi.huixiangedu.cn

[T30] Swift：协议
来源：http://du.szsharing.cn

protocol Shape { func area() -> Double }
来源：http://gx.jctech888.com.cn

[T31] Lua：Hello World
来源：http://pb.jctech888.com.cn

print("Hello")
来源：http://af.asd995.cn

[T32] Lua：局部变量
来源：http://uk.chemitech.net.cn

local a = 1
来源：http://pa.asd995.cn

[T33] Lua：表（数组）
来源：http://yx.huanxung.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://aa.jianghongdianzi.cn

[T34] Lua：遍历表
来源：http://at.bookmarksfly.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vm.bookmarksfly.cn

[T35] Lua：字典表
来源：http://jl.hnjuh.cn

local d = { a = 1 };  d.b = 2
来源：http://rc.jianghongdianzi.cn

[T36] Lua：函数
来源：http://in.asd995.cn

function add(a, b) return a + b end
来源：http://xh.gzmigu.cn

[T37] Lua：字符串拼接
来源：http://kw.nszjky.cn

"a" .. "b"
来源：http://cg.haigaiapp.cn

[T38] Lua：条件
来源：http://oh.9csxet.cn

if x > 0 then print("正") end
来源：http://pl.521024.cn

[T39] Lua：模式匹配
来源：http://ma.shtwfgs.cn

string.find(s, "%d+")
来源：http://ab.lnxyls.cn

[T40] Lua：元表
来源：http://yu.huixinmuqiang.cn

setmetatable({}, { __index = base })
来源：http://ko.bjjhwx.cn

[T41] Perl：Hello World
来源：http://pe.szxytkj.cn

print "Hello\n";
来源：http://ty.521024.cn

[T42] Perl：变量类型
来源：http://xg.szsharing.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mg.yuntaijiaju.cn

[T43] Perl：字符串插值
来源：http://oz.nicolike.cn

"值: $a"
来源：http://ai.bjjhwx.cn

[T44] Perl：条件
来源：http://oa.yuntaijiaju.cn

if ($a > 0) { print "正"; }
来源：http://oa.muxihuayi.cn

[T45] Perl：数组遍历
来源：http://vm.shxzukj.cn

for my $x (@arr) { print $x; }
来源：http://vw.chemitech.net.cn

[T46] Perl：哈希操作
来源：http://rh.gzmigu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tp.jianghongdianzi.cn

[T47] Perl：正则捕获
来源：http://ms.huanxung.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.wgjwhj.cn

[T48] Perl：正则替换
来源：http://te.chemitech.net.cn

$s =~ s/old/new/g;
来源：http://is.panjiajie.cn

[T49] Perl：函数
来源：http://wo.yuntaijiaju.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hu.shxzukj.cn

[T50] Perl：逐行读文件
来源：http://mx.muxihuayi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zn.gzmigu.cn

while (my $line = <$fh>) { print $line; }
来源：http://sd.jianghongdianzi.cn

[T51] Scala：Hello World
来源：http://te.nszjky.cn

println("Hello")
来源：http://bf.nszjky.cn

[T52] Scala：变量
来源：http://vv.jianghongdianzi.cn

val a = 1;  var b = 2
来源：http://cn.asd995.cn

[T53] Scala：字符串插值
来源：http://pa.shxzskj.cn

s"值: $b"
来源：http://xv.hahajie.cn

[T54] Scala：集合映射
来源：http://nb.chemitech.net.cn

List(1, 2, 3).map(_ * 2)
来源：http://vn.yuexingan06.cn

[T55] Scala：集合过滤
来源：http://qm.huanxung.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ip.haigaiapp.cn

[T56] Scala：样例类
来源：http://ge.9csxet.cn

case class User(name: String, age: Int)
来源：http://wy.haigaiapp.cn

[T57] Scala：模式匹配
来源：http://yv.huanxung.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://da.szsharing.cn

[T58] Scala：函数定义
来源：http://hi.jctech888.com.cn

def add(a: Int, b: Int): Int = a + b
来源：http://um.colortex.cn

[T59] Scala：循环
来源：http://hs.szxytkj.cn

for (i <- 1 to 10) println(i)
来源：http://ny.9csxet.cn

[T60] Scala：折叠
来源：http://ec.haigaiapp.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wr.gzmigu.cn

================================================================================
来源：http://la.huixiangedu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mg.haigaiapp.cn

================================================================================
来源：http://eo.shxzskj.cn

[U01] Py：创建虚拟环境
来源：http://ch.9csxet.cn

python -m venv .venv && source .venv/bin/activate
来源：http://pp.hahajie.cn

[U02] Py：导出 / 安装依赖
来源：http://yb.521024.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ki.yuntaijiaju.cn

[U03] Py：加载 .env 配置
来源：http://pg.asd995.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ag.nszjky.cn

[U04] Py：变量调试打印
来源：http://vw.shtwfgs.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gp.bjjhwx.cn

[U05] Py：列表去重且保序
来源：http://et.chemitech.net.cn

list(dict.fromkeys(arr))
来源：http://fg.huanxung.cn

[U06] Py：合并两个字典
来源：http://ip.huixiangedu.cn

{**a, **b}
来源：http://bs.nszjky.cn

[U07] Py：反转字典键值
来源：http://iq.gzmigu.cn

{v: k for k, v in d.items()}
来源：http://vz.muxihuayi.cn

[U08] Py：展平二维列表
来源：http://vt.jianghongdianzi.cn

[y for x in nested for y in x]
来源：http://lf.wgjwhj.cn

[U09] Py：字典取最大值的键
来源：http://to.asd995.cn

max(d, key=d.get)
来源：http://sq.szxytkj.cn

[U10] Py：按值排序字典
来源：http://na.bjjhwx.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ld.shxzukj.cn

[U11] Py：生成器表达式
来源：http://qz.szsharing.cn

(x * 2 for x in arr)
来源：http://qc.521024.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ls.9csxet.cn

Counter(arr).most_common(3)
来源：http://ri.yuexingan06.cn

[U13] Py：固定长度队列
来源：http://yv.yuexingan06.cn

deque(maxlen=10)
来源：http://hl.huanxung.cn

[U14] Py：分组收集到列表
来源：http://tl.panjiajie.cn

defaultdict(list)
来源：http://rx.bjjhwx.cn

[U15] Py：高精度计时
来源：http://zk.haigaiapp.cn

t = time.perf_counter()
来源：http://dw.jctech888.com.cn

[U16] Py：命令行参数解析
来源：http://lg.colortex.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mm.huanxung.cn

[U17] Py：初始化日志
来源：http://wh.hahajie.cn

logging.basicConfig(level=logging.INFO)
来源：http://dk.huixiangedu.cn

[U18] Py：预编译正则
来源：http://qe.shtwfgs.cn

pat = re.compile(r"\d+")
来源：http://kc.chemitech.net.cn

[U19] Py：正则替换带回调
来源：http://he.9csxet.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rd.gzmigu.cn

[U20] Py：缓存函数结果
来源：http://tt.gzmigu.cn

@functools.lru_cache(maxsize=None)
来源：http://xo.panjiajie.cn

[U21] Py：自定义上下文管理器
来源：http://rn.bjjhwx.cn

@contextlib.contextmanager
来源：http://xf.haigaiapp.cn

[U22] Py：矩阵转置
来源：http://mj.shtwfgs.cn

list(zip(*m))
来源：http://bc.colortex.cn


<!-- 参考信息 -->