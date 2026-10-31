代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sw.wgjwhj.cn

[R80] 查看脚本执行耗时
来源：http://ga.yuexingan06.cn

time ./run.sh
来源：http://xw.nicolike.cn

================================================================================
来源：http://hm.haigaiapp.cn

S. C / C++ 专题
来源：http://au.shxzskj.cn

================================================================================
来源：http://cv.haigaiapp.cn

[S01] C：Hello World
来源：http://cf.huanxung.cn

#include <stdio.h>
来源：http://ki.shxzskj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://di.chemitech.net.cn

[S02] C：变量与格式化输出
来源：http://re.hnjuh.cn

int a = 10; printf("%d\n", a);
来源：http://ks.9csxet.cn

[S03] C：读入整数
来源：http://nb.jianghongdianzi.cn

int x; scanf("%d", &x);
来源：http://un.shxzukj.cn

[S04] C：字符串复制
来源：http://sn.haigaiapp.cn

char dst[32]; strcpy(dst, "hi");
来源：http://bo.9csxet.cn

[S05] C：字符串长度
来源：http://gz.newstarts.cn

strlen(s)
来源：http://ll.shxzskj.cn

[S06] C：字符串比较
来源：http://pk.jctech888.com.cn

strcmp(a, b) == 0
来源：http://qv.szxytkj.cn

[S07] C：数组遍历求和
来源：http://jd.asd995.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://oy.colortex.cn

[S08] C：动态内存分配与释放
来源：http://tp.haigaiapp.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://os.shxzskj.cn

[S09] C：结构体定义与初始化
来源：http://ti.nicolike.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qj.szxytkj.cn

[S10] C：指针与解引用
来源：http://te.jctech888.com.cn

int *p = &a;  *p = 5;
来源：http://cw.newstarts.cn

[S11] C：逐行读文件
来源：http://ad.newstarts.cn

FILE *f = fopen("a.txt", "r");
来源：http://oq.chemitech.net.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ne.hahajie.cn

fclose(f);
来源：http://nw.colortex.cn

[S12] C：写文件
来源：http://yf.chemitech.net.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://iu.gzmigu.cn

[S13] C：宏定义
来源：http://bg.gzmigu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fm.panjiajie.cn

[S14] C：枚举
来源：http://mh.yuexingan06.cn

enum Color { RED, GREEN, BLUE };
来源：http://yi.lnxyls.cn

[S15] C：类型转换
来源：http://up.yuexingan06.cn

(double) a / b
来源：http://gs.nicolike.cn

[S16] C：位操作置位
来源：http://sh.hahajie.cn

x |= (1 << 3);
来源：http://pz.bjjhwx.cn

[S17] C：安全拼接字符串
来源：http://go.szsharing.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cl.panjiajie.cn

[S18] C：命令行参数
来源：http://fb.jianghongdianzi.cn

int main(int argc, char **argv)
来源：http://bp.hahajie.cn

[S19] C：快速排序
来源：http://ek.hahajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://uo.haigaiapp.cn

[S20] C：二分查找
来源：http://vr.yuntaijiaju.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mb.panjiajie.cn

[S21] C：字符类别判断
来源：http://pz.521024.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ll.jctech888.com.cn

[S22] C：字符串转数字
来源：http://vg.gzmigu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wa.szxytkj.cn

[S23] C：随机数
来源：http://zp.nszjky.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hj.wgjwhj.cn

[S24] C：获取本地时间
来源：http://yv.wgjwhj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xo.asd995.cn

[S25] C：内存拷贝
来源：http://yl.shxzukj.cn

memcpy(dst, src, n);
来源：http://ge.shxzskj.cn

[S26] C：内存清零
来源：http://ii.shxzskj.cn

memset(a, 0, sizeof a);
来源：http://ov.panjiajie.cn

[S27] C：定义常量
来源：http://wd.newstarts.cn

const double PI = 3.14159;
来源：http://fz.huixiangedu.cn

[S28] C：静态变量
来源：http://cq.nszjky.cn

static int counter = 0;
来源：http://pu.panjiajie.cn

[S29] C：变参函数
来源：http://ue.huixinmuqiang.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jp.wgjwhj.cn

[S30] C：头文件保护
来源：http://iu.yuexingan06.cn

#ifndef X_H
来源：http://is.bjjhwx.cn

#define X_H
来源：http://vi.nicolike.cn

#endif
来源：http://gn.wgjwhj.cn

[S31] C++：Hello World
来源：http://gs.wgjwhj.cn

#include <iostream>
来源：http://of.gzmigu.cn

int main() { std::cout << "Hello\n"; }
来源：http://px.lnxyls.cn

[S32] C++：字符串
来源：http://nj.haigaiapp.cn

std::string s = "hi";  s += "!";
来源：http://ww.jctech888.com.cn

[S33] C++：vector 增删
来源：http://yg.jianghongdianzi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lf.szxytkj.cn

[S34] C++：遍历 vector
来源：http://km.jctech888.com.cn

for (auto &x : v) { std::cout << x; }
来源：http://uz.wgjwhj.cn

[S35] C++：map
来源：http://ys.colortex.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://if.yuexingan06.cn

[S36] C++：unordered_map
来源：http://dg.lnxyls.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lu.newstarts.cn

[S37] C++：set
来源：http://dc.huixiangedu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ea.9csxet.cn

[S38] C++：排序
来源：http://bp.newstarts.cn

std::sort(v.begin(), v.end());
来源：http://ma.haigaiapp.cn

[S39] C++：自定义比较器排序
来源：http://nd.chemitech.net.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hg.521024.cn

[S40] C++：查找元素
来源：http://ux.shxzskj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ff.nszjky.cn

[S41] C++：类与构造函数
来源：http://qs.nszjky.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rs.lnxyls.cn

[S42] C++：继承与虚函数
来源：http://hd.bookmarksfly.cn

class B : public Base { public: void f() override {} };
来源：http://ws.hnjuh.cn

[S43] C++：智能指针
来源：http://by.521024.cn

auto p = std::make_unique<int>(5);
来源：http://we.bjjhwx.cn

[S44] C++：引用传参
来源：http://lx.szxytkj.cn

void inc(int &x) { ++x; }
来源：http://gc.bjjhwx.cn

[S45] C++：lambda
来源：http://rx.nicolike.cn

auto add = [](int a, int b) { return a + b; };
来源：http://lm.nszjky.cn

[S46] C++：函数模板
来源：http://ng.wgjwhj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sn.gzmigu.cn

[S47] C++：结构化绑定遍历
来源：http://vn.panjiajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bs.lnxyls.cn

[S48] C++：逐行读文件
来源：http://ci.bjjhwx.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ll.shxzskj.cn

while (std::getline(in, line)) { }
来源：http://kf.chemitech.net.cn

[S49] C++：写文件
来源：http://uk.hahajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tp.gzmigu.cn

[S50] C++：格式化数字
来源：http://cg.shxzskj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ap.wgjwhj.cn

[S51] C++：显式类型转换
来源：http://zx.yuntaijiaju.cn

static_cast<double>(a) / b
来源：http://xd.bjjhwx.cn

[S52] C++：const 与 noexcept
来源：http://fu.wgjwhj.cn

int size() const noexcept { return n_; }
来源：http://gx.hnjuh.cn

[S53] C++：移动语义
来源：http://ns.yuntaijiaju.cn

std::vector<int> w = std::move(v);
来源：http://ek.9csxet.cn

[S54] C++：异常处理
来源：http://ax.yuntaijiaju.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gu.jctech888.com.cn

[S55] C++：结构化绑定
来源：http://sn.shxzukj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://oc.shxzskj.cn

[S56] C++：optional
来源：http://gb.shtwfgs.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dg.wgjwhj.cn

[S57] C++：编译期常量
来源：http://ot.hahajie.cn

constexpr int N = 10;
来源：http://iz.521024.cn

[S58] C++：命名空间
来源：http://hn.huixinmuqiang.cn

namespace ns { int f() { return 1; } }
来源：http://kf.huixinmuqiang.cn

[S59] C++：静态断言
来源：http://cw.colortex.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rk.huixiangedu.cn

[S60] C++：遍历并删除元素
来源：http://sv.yuntaijiaju.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://px.shxzskj.cn

================================================================================
来源：http://kf.9csxet.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ko.lnxyls.cn

================================================================================
来源：http://uj.nszjky.cn

[T01] Kotlin：Hello World
来源：http://rj.shxzukj.cn

println("Hello")
来源：http://gt.asd995.cn

[T02] Kotlin：变量
来源：http://ak.panjiajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xh.newstarts.cn

[T03] Kotlin：字符串模板
来源：http://ki.muxihuayi.cn

"值: $b"
来源：http://sz.hnjuh.cn

[T04] Kotlin：空安全
来源：http://oe.gzmigu.cn

val n: String? = null;  n?.length
来源：http://sn.huixiangedu.cn

[T05] Kotlin：when 表达式
来源：http://sb.hahajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pq.colortex.cn

[T06] Kotlin：集合映射
来源：http://nr.newstarts.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ge.hnjuh.cn

[T07] Kotlin：集合过滤
来源：http://og.wgjwhj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ox.shxzskj.cn

[T08] Kotlin：数据类
来源：http://iu.shtwfgs.cn

data class User(val name: String, val age: Int)
来源：http://jh.huixinmuqiang.cn

[T09] Kotlin：扩展函数
来源：http://co.shxzukj.cn

fun String.exclaim() = this + "!"
来源：http://fz.bookmarksfly.cn

[T10] Kotlin：默认参数
来源：http://tb.asd995.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ck.szxytkj.cn

[T11] Kotlin：协程
来源：http://zm.shxzukj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://iy.asd995.cn

[T12] Kotlin：解构声明
来源：http://bp.shxzskj.cn

val (a, b) = Pair(1, 2)
来源：http://so.bookmarksfly.cn

[T13] Kotlin：只读 Map
来源：http://vq.lnxyls.cn

val m = mapOf("a" to 1)
来源：http://cb.lnxyls.cn

[T14] Kotlin：循环
来源：http://dd.huixinmuqiang.cn

for (i in 1..10) println(i)
来源：http://yl.shxzskj.cn

[T15] Kotlin：接口
来源：http://kj.jctech888.com.cn

interface Shape { fun area(): Double }
来源：http://gi.bookmarksfly.cn

[T16] Swift：Hello World
来源：http://xc.nicolike.cn

print("Hello")
来源：http://kn.chemitech.net.cn

[T17] Swift：变量与常量
来源：http://fg.asd995.cn

var a = 1;  let b = 2
来源：http://eg.gzmigu.cn

[T18] Swift：字符串插值
来源：http://fr.newstarts.cn

"值: \(b)"
来源：http://hm.shxzskj.cn

[T19] Swift：可选绑定
来源：http://ij.wgjwhj.cn

if let n = opt { print(n) }
来源：http://bb.newstarts.cn

[T20] Swift：数组操作
来源：http://lu.hnjuh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://wo.nszjky.cn

[T21] Swift：遍历
来源：http://un.jctech888.com.cn

for x in a { print(x) }
来源：http://hv.szsharing.cn

[T22] Swift：字典
来源：http://pn.jianghongdianzi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ig.shtwfgs.cn

[T23] Swift：函数
来源：http://wv.jctech888.com.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://my.nicolike.cn

[T24] Swift：闭包
来源：http://ux.521024.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://oo.yuntaijiaju.cn

[T25] Swift：结构体
来源：http://mr.shtwfgs.cn

struct P { var x: Int }
来源：http://bv.shxzskj.cn

[T26] Swift：类与重写
来源：http://qn.szsharing.cn

class A: Base { override func f() {} }
来源：http://vb.lnxyls.cn

[T27] Swift：错误处理
来源：http://rq.huixiangedu.cn

do { try f() } catch { print(error) }
来源：http://ra.chemitech.net.cn

[T28] Swift：枚举
来源：http://ln.wgjwhj.cn

enum Color { case red, green }
来源：http://zc.szsharing.cn

[T29] Swift：guard 提前返回
来源：http://wq.panjiajie.cn

guard let x = opt else { return }
来源：http://zk.shxzukj.cn

[T30] Swift：协议
来源：http://so.9csxet.cn

protocol Shape { func area() -> Double }
来源：http://md.asd995.cn

[T31] Lua：Hello World
来源：http://jj.wgjwhj.cn

print("Hello")
来源：http://cq.newstarts.cn

[T32] Lua：局部变量
来源：http://tb.521024.cn

local a = 1
来源：http://ce.hnjuh.cn

[T33] Lua：表（数组）
来源：http://cp.szsharing.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ot.yuntaijiaju.cn

[T34] Lua：遍历表
来源：http://ze.szsharing.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://pa.szsharing.cn

[T35] Lua：字典表
来源：http://sw.shxzskj.cn

local d = { a = 1 };  d.b = 2
来源：http://bs.szsharing.cn

[T36] Lua：函数
来源：http://fh.9csxet.cn

function add(a, b) return a + b end
来源：http://km.wgjwhj.cn

[T37] Lua：字符串拼接
来源：http://ax.huixiangedu.cn

"a" .. "b"
来源：http://id.huixiangedu.cn

[T38] Lua：条件
来源：http://my.shxzukj.cn

if x > 0 then print("正") end
来源：http://op.huixiangedu.cn

[T39] Lua：模式匹配
来源：http://xc.muxihuayi.cn

string.find(s, "%d+")
来源：http://da.shxzskj.cn

[T40] Lua：元表
来源：http://ji.panjiajie.cn

setmetatable({}, { __index = base })
来源：http://hf.haigaiapp.cn

[T41] Perl：Hello World
来源：http://xa.jianghongdianzi.cn

print "Hello\n";
来源：http://nm.gzmigu.cn

[T42] Perl：变量类型
来源：http://fy.huixinmuqiang.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://aq.521024.cn

[T43] Perl：字符串插值
来源：http://gj.hahajie.cn

"值: $a"
来源：http://zf.yuntaijiaju.cn

[T44] Perl：条件
来源：http://zp.newstarts.cn

if ($a > 0) { print "正"; }
来源：http://zz.jctech888.com.cn

[T45] Perl：数组遍历
来源：http://dy.panjiajie.cn

for my $x (@arr) { print $x; }
来源：http://za.hnjuh.cn

[T46] Perl：哈希操作
来源：http://ae.bookmarksfly.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vl.9csxet.cn

[T47] Perl：正则捕获
来源：http://uu.hnjuh.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://tb.asd995.cn

[T48] Perl：正则替换
来源：http://ru.panjiajie.cn

$s =~ s/old/new/g;
来源：http://fb.bjjhwx.cn

[T49] Perl：函数
来源：http://po.nszjky.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ej.shxzukj.cn

[T50] Perl：逐行读文件
来源：http://mo.shxzskj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rc.nicolike.cn

while (my $line = <$fh>) { print $line; }
来源：http://ir.shtwfgs.cn

[T51] Scala：Hello World
来源：http://ru.bookmarksfly.cn

println("Hello")
来源：http://ar.jctech888.com.cn

[T52] Scala：变量
来源：http://ro.colortex.cn

val a = 1;  var b = 2
来源：http://aj.huixiangedu.cn

[T53] Scala：字符串插值
来源：http://jl.szsharing.cn

s"值: $b"
来源：http://kp.bjjhwx.cn

[T54] Scala：集合映射
来源：http://wd.huixiangedu.cn

List(1, 2, 3).map(_ * 2)
来源：http://kn.yuexingan06.cn

[T55] Scala：集合过滤
来源：http://fr.hahajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://op.szxytkj.cn

[T56] Scala：样例类
来源：http://xh.hnjuh.cn

case class User(name: String, age: Int)
来源：http://pg.jianghongdianzi.cn

[T57] Scala：模式匹配
来源：http://hw.bjjhwx.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://eh.lnxyls.cn

[T58] Scala：函数定义
来源：http://xf.wgjwhj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wn.jianghongdianzi.cn

[T59] Scala：循环
来源：http://wi.szxytkj.cn

for (i <- 1 to 10) println(i)
来源：http://cf.bjjhwx.cn

[T60] Scala：折叠
来源：http://dz.hahajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tr.521024.cn

================================================================================
来源：http://nx.huixinmuqiang.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xi.nicolike.cn

================================================================================
来源：http://po.colortex.cn

[U01] Py：创建虚拟环境
来源：http://bz.wgjwhj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ot.shxzskj.cn

[U02] Py：导出 / 安装依赖
来源：http://jt.shxzskj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mg.nicolike.cn

[U03] Py：加载 .env 配置
来源：http://cc.asd995.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://td.colortex.cn

[U04] Py：变量调试打印
来源：http://ap.nicolike.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hu.shtwfgs.cn

[U05] Py：列表去重且保序
来源：http://up.yuntaijiaju.cn

list(dict.fromkeys(arr))
来源：http://jf.lnxyls.cn

[U06] Py：合并两个字典
来源：http://lr.bjjhwx.cn

{**a, **b}
来源：http://aq.yuntaijiaju.cn

[U07] Py：反转字典键值
来源：http://ar.bookmarksfly.cn

{v: k for k, v in d.items()}
来源：http://gl.shxzukj.cn

[U08] Py：展平二维列表
来源：http://qh.jctech888.com.cn

[y for x in nested for y in x]
来源：http://db.bookmarksfly.cn

[U09] Py：字典取最大值的键
来源：http://bw.nicolike.cn

max(d, key=d.get)
来源：http://vh.521024.cn

[U10] Py：按值排序字典
来源：http://xf.shxzukj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bh.huanxung.cn

[U11] Py：生成器表达式
来源：http://kx.shxzukj.cn

(x * 2 for x in arr)
来源：http://kx.hnjuh.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qk.yuexingan06.cn

Counter(arr).most_common(3)
来源：http://uu.panjiajie.cn

[U13] Py：固定长度队列
来源：http://tu.huixiangedu.cn

deque(maxlen=10)
来源：http://jt.gzmigu.cn

[U14] Py：分组收集到列表
来源：http://eb.wgjwhj.cn

defaultdict(list)
来源：http://ee.shxzskj.cn

[U15] Py：高精度计时
来源：http://fo.jianghongdianzi.cn

t = time.perf_counter()
来源：http://zz.shxzukj.cn

[U16] Py：命令行参数解析
来源：http://lk.nszjky.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://po.haigaiapp.cn

[U17] Py：初始化日志
来源：http://rn.newstarts.cn

logging.basicConfig(level=logging.INFO)
来源：http://pj.521024.cn

[U18] Py：预编译正则
来源：http://ca.huanxung.cn

pat = re.compile(r"\d+")
来源：http://bf.huanxung.cn

[U19] Py：正则替换带回调
来源：http://hq.shxzskj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kz.bjjhwx.cn

[U20] Py：缓存函数结果
来源：http://nr.asd995.cn

@functools.lru_cache(maxsize=None)
来源：http://xd.521024.cn


<!-- 参考信息 -->