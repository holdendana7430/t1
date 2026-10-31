代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://eg.huixiangedu.cn

[R80] 查看脚本执行耗时
来源：http://rg.panjiajie.cn

time ./run.sh
来源：http://ad.shtwfgs.cn

================================================================================
来源：http://yu.9csxet.cn

S. C / C++ 专题
来源：http://af.bjjhwx.cn

================================================================================
来源：http://th.nszjky.cn

[S01] C：Hello World
来源：http://fv.gzmigu.cn

#include <stdio.h>
来源：http://vm.colortex.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bb.shxzukj.cn

[S02] C：变量与格式化输出
来源：http://jm.huanxung.cn

int a = 10; printf("%d\n", a);
来源：http://ru.bjjhwx.cn

[S03] C：读入整数
来源：http://ve.bjjhwx.cn

int x; scanf("%d", &x);
来源：http://il.szsharing.cn

[S04] C：字符串复制
来源：http://oc.szxytkj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wb.huanxung.cn

[S05] C：字符串长度
来源：http://we.hnjuh.cn

strlen(s)
来源：http://gv.panjiajie.cn

[S06] C：字符串比较
来源：http://zy.huixinmuqiang.cn

strcmp(a, b) == 0
来源：http://fo.hnjuh.cn

[S07] C：数组遍历求和
来源：http://bp.panjiajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dz.chemitech.net.cn

[S08] C：动态内存分配与释放
来源：http://dy.yuexingan06.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gp.haigaiapp.cn

[S09] C：结构体定义与初始化
来源：http://ox.gzmigu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nu.nszjky.cn

[S10] C：指针与解引用
来源：http://km.jianghongdianzi.cn

int *p = &a;  *p = 5;
来源：http://sq.yuntaijiaju.cn

[S11] C：逐行读文件
来源：http://jx.shxzukj.cn

FILE *f = fopen("a.txt", "r");
来源：http://ok.wgjwhj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://kx.shxzukj.cn

fclose(f);
来源：http://xd.huanxung.cn

[S12] C：写文件
来源：http://ir.521024.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bp.hnjuh.cn

[S13] C：宏定义
来源：http://aj.wgjwhj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://oe.newstarts.cn

[S14] C：枚举
来源：http://cy.szsharing.cn

enum Color { RED, GREEN, BLUE };
来源：http://ae.huanxung.cn

[S15] C：类型转换
来源：http://mo.nszjky.cn

(double) a / b
来源：http://yn.wgjwhj.cn

[S16] C：位操作置位
来源：http://mb.jianghongdianzi.cn

x |= (1 << 3);
来源：http://tc.huixiangedu.cn

[S17] C：安全拼接字符串
来源：http://gb.wgjwhj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://js.hnjuh.cn

[S18] C：命令行参数
来源：http://wx.szxytkj.cn

int main(int argc, char **argv)
来源：http://my.shxzukj.cn

[S19] C：快速排序
来源：http://mt.szxytkj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://da.panjiajie.cn

[S20] C：二分查找
来源：http://dt.shtwfgs.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zl.chemitech.net.cn

[S21] C：字符类别判断
来源：http://rm.huixiangedu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ne.yuexingan06.cn

[S22] C：字符串转数字
来源：http://jx.wgjwhj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://em.huixinmuqiang.cn

[S23] C：随机数
来源：http://gu.jianghongdianzi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hq.yuntaijiaju.cn

[S24] C：获取本地时间
来源：http://nd.jctech888.com.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rp.hnjuh.cn

[S25] C：内存拷贝
来源：http://wk.lnxyls.cn

memcpy(dst, src, n);
来源：http://st.shxzukj.cn

[S26] C：内存清零
来源：http://to.huixiangedu.cn

memset(a, 0, sizeof a);
来源：http://ph.521024.cn

[S27] C：定义常量
来源：http://fh.bjjhwx.cn

const double PI = 3.14159;
来源：http://ek.colortex.cn

[S28] C：静态变量
来源：http://ht.521024.cn

static int counter = 0;
来源：http://ly.wgjwhj.cn

[S29] C：变参函数
来源：http://in.haigaiapp.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mi.shtwfgs.cn

[S30] C：头文件保护
来源：http://qy.newstarts.cn

#ifndef X_H
来源：http://fl.colortex.cn

#define X_H
来源：http://bp.shtwfgs.cn

#endif
来源：http://dq.muxihuayi.cn

[S31] C++：Hello World
来源：http://fo.521024.cn

#include <iostream>
来源：http://ba.hnjuh.cn

int main() { std::cout << "Hello\n"; }
来源：http://uy.jctech888.com.cn

[S32] C++：字符串
来源：http://tg.gzmigu.cn

std::string s = "hi";  s += "!";
来源：http://ka.shtwfgs.cn

[S33] C++：vector 增删
来源：http://mb.szxytkj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bn.huanxung.cn

[S34] C++：遍历 vector
来源：http://cd.bjjhwx.cn

for (auto &x : v) { std::cout << x; }
来源：http://uq.jctech888.com.cn

[S35] C++：map
来源：http://wo.hahajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pr.haigaiapp.cn

[S36] C++：unordered_map
来源：http://ab.shtwfgs.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lt.nicolike.cn

[S37] C++：set
来源：http://ya.nicolike.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dp.muxihuayi.cn

[S38] C++：排序
来源：http://dl.panjiajie.cn

std::sort(v.begin(), v.end());
来源：http://hr.jianghongdianzi.cn

[S39] C++：自定义比较器排序
来源：http://nx.9csxet.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rb.521024.cn

[S40] C++：查找元素
来源：http://mu.nicolike.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ld.nszjky.cn

[S41] C++：类与构造函数
来源：http://ut.lnxyls.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vb.lnxyls.cn

[S42] C++：继承与虚函数
来源：http://nf.nszjky.cn

class B : public Base { public: void f() override {} };
来源：http://sf.nszjky.cn

[S43] C++：智能指针
来源：http://hb.nicolike.cn

auto p = std::make_unique<int>(5);
来源：http://pk.shxzskj.cn

[S44] C++：引用传参
来源：http://lj.szxytkj.cn

void inc(int &x) { ++x; }
来源：http://af.muxihuayi.cn

[S45] C++：lambda
来源：http://ay.huixiangedu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gh.huixinmuqiang.cn

[S46] C++：函数模板
来源：http://wd.nszjky.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sr.521024.cn

[S47] C++：结构化绑定遍历
来源：http://dk.jctech888.com.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ke.colortex.cn

[S48] C++：逐行读文件
来源：http://bd.lnxyls.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ti.shxzskj.cn

while (std::getline(in, line)) { }
来源：http://cr.shxzukj.cn

[S49] C++：写文件
来源：http://bn.asd995.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bq.wgjwhj.cn

[S50] C++：格式化数字
来源：http://by.asd995.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ti.jianghongdianzi.cn

[S51] C++：显式类型转换
来源：http://mk.szxytkj.cn

static_cast<double>(a) / b
来源：http://wk.bookmarksfly.cn

[S52] C++：const 与 noexcept
来源：http://ul.shtwfgs.cn

int size() const noexcept { return n_; }
来源：http://kr.szsharing.cn

[S53] C++：移动语义
来源：http://gl.chemitech.net.cn

std::vector<int> w = std::move(v);
来源：http://yj.szsharing.cn

[S54] C++：异常处理
来源：http://fb.nszjky.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mo.9csxet.cn

[S55] C++：结构化绑定
来源：http://ed.haigaiapp.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://nb.shtwfgs.cn

[S56] C++：optional
来源：http://cp.huixinmuqiang.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wd.wgjwhj.cn

[S57] C++：编译期常量
来源：http://dt.shxzukj.cn

constexpr int N = 10;
来源：http://pz.9csxet.cn

[S58] C++：命名空间
来源：http://ey.nszjky.cn

namespace ns { int f() { return 1; } }
来源：http://wx.nszjky.cn

[S59] C++：静态断言
来源：http://br.yuntaijiaju.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ru.gzmigu.cn

[S60] C++：遍历并删除元素
来源：http://de.yuexingan06.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qi.chemitech.net.cn

================================================================================
来源：http://pz.hahajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jb.bookmarksfly.cn

================================================================================
来源：http://st.yuexingan06.cn

[T01] Kotlin：Hello World
来源：http://zx.chemitech.net.cn

println("Hello")
来源：http://jt.lnxyls.cn

[T02] Kotlin：变量
来源：http://vq.521024.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vh.nszjky.cn

[T03] Kotlin：字符串模板
来源：http://cj.asd995.cn

"值: $b"
来源：http://zu.muxihuayi.cn

[T04] Kotlin：空安全
来源：http://fe.shxzskj.cn

val n: String? = null;  n?.length
来源：http://as.9csxet.cn

[T05] Kotlin：when 表达式
来源：http://ap.panjiajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://eu.521024.cn

[T06] Kotlin：集合映射
来源：http://wn.huanxung.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hw.shxzskj.cn

[T07] Kotlin：集合过滤
来源：http://ym.colortex.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ks.huanxung.cn

[T08] Kotlin：数据类
来源：http://cx.panjiajie.cn

data class User(val name: String, val age: Int)
来源：http://ki.bjjhwx.cn

[T09] Kotlin：扩展函数
来源：http://qd.yuexingan06.cn

fun String.exclaim() = this + "!"
来源：http://tw.521024.cn

[T10] Kotlin：默认参数
来源：http://ca.huixinmuqiang.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wn.szxytkj.cn

[T11] Kotlin：协程
来源：http://wm.shxzukj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://al.bookmarksfly.cn

[T12] Kotlin：解构声明
来源：http://yt.huixinmuqiang.cn

val (a, b) = Pair(1, 2)
来源：http://nl.nicolike.cn

[T13] Kotlin：只读 Map
来源：http://ol.panjiajie.cn

val m = mapOf("a" to 1)
来源：http://eu.huanxung.cn

[T14] Kotlin：循环
来源：http://nl.9csxet.cn

for (i in 1..10) println(i)
来源：http://qh.haigaiapp.cn

[T15] Kotlin：接口
来源：http://bm.shtwfgs.cn

interface Shape { fun area(): Double }
来源：http://bg.szsharing.cn

[T16] Swift：Hello World
来源：http://id.szxytkj.cn

print("Hello")
来源：http://xr.haigaiapp.cn

[T17] Swift：变量与常量
来源：http://hj.szsharing.cn

var a = 1;  let b = 2
来源：http://wz.bjjhwx.cn

[T18] Swift：字符串插值
来源：http://uw.jianghongdianzi.cn

"值: \(b)"
来源：http://om.asd995.cn

[T19] Swift：可选绑定
来源：http://rq.shxzskj.cn

if let n = opt { print(n) }
来源：http://eo.huixiangedu.cn

[T20] Swift：数组操作
来源：http://bs.colortex.cn

var a = [1, 2, 3];  a.append(4)
来源：http://sz.huixiangedu.cn

[T21] Swift：遍历
来源：http://jr.bjjhwx.cn

for x in a { print(x) }
来源：http://ot.panjiajie.cn

[T22] Swift：字典
来源：http://cq.yuexingan06.cn

var d = ["a": 1];  d["b"] = 2
来源：http://bj.521024.cn

[T23] Swift：函数
来源：http://al.huixinmuqiang.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wj.bookmarksfly.cn

[T24] Swift：闭包
来源：http://ae.521024.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://fq.jianghongdianzi.cn

[T25] Swift：结构体
来源：http://zb.colortex.cn

struct P { var x: Int }
来源：http://xt.gzmigu.cn

[T26] Swift：类与重写
来源：http://oo.bjjhwx.cn

class A: Base { override func f() {} }
来源：http://kx.yuexingan06.cn

[T27] Swift：错误处理
来源：http://bv.chemitech.net.cn

do { try f() } catch { print(error) }
来源：http://fq.hnjuh.cn

[T28] Swift：枚举
来源：http://iz.newstarts.cn

enum Color { case red, green }
来源：http://jb.huanxung.cn

[T29] Swift：guard 提前返回
来源：http://sb.nicolike.cn

guard let x = opt else { return }
来源：http://tv.wgjwhj.cn

[T30] Swift：协议
来源：http://wq.9csxet.cn

protocol Shape { func area() -> Double }
来源：http://vy.haigaiapp.cn

[T31] Lua：Hello World
来源：http://sx.shtwfgs.cn

print("Hello")
来源：http://hw.yuntaijiaju.cn

[T32] Lua：局部变量
来源：http://jv.gzmigu.cn

local a = 1
来源：http://ou.shtwfgs.cn

[T33] Lua：表（数组）
来源：http://dc.muxihuayi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xp.lnxyls.cn

[T34] Lua：遍历表
来源：http://rc.huixiangedu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://tm.huixiangedu.cn

[T35] Lua：字典表
来源：http://sx.haigaiapp.cn

local d = { a = 1 };  d.b = 2
来源：http://wk.shxzukj.cn

[T36] Lua：函数
来源：http://mq.lnxyls.cn

function add(a, b) return a + b end
来源：http://ez.hnjuh.cn

[T37] Lua：字符串拼接
来源：http://am.yuntaijiaju.cn

"a" .. "b"
来源：http://ct.jianghongdianzi.cn

[T38] Lua：条件
来源：http://wu.521024.cn

if x > 0 then print("正") end
来源：http://nd.bookmarksfly.cn

[T39] Lua：模式匹配
来源：http://bl.yuntaijiaju.cn

string.find(s, "%d+")
来源：http://mm.9csxet.cn

[T40] Lua：元表
来源：http://qd.panjiajie.cn

setmetatable({}, { __index = base })
来源：http://ig.nicolike.cn

[T41] Perl：Hello World
来源：http://xo.muxihuayi.cn

print "Hello\n";
来源：http://cx.9csxet.cn

[T42] Perl：变量类型
来源：http://bo.nicolike.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://we.panjiajie.cn

[T43] Perl：字符串插值
来源：http://po.shxzskj.cn

"值: $a"
来源：http://sm.nicolike.cn

[T44] Perl：条件
来源：http://ms.nszjky.cn

if ($a > 0) { print "正"; }
来源：http://hf.haigaiapp.cn

[T45] Perl：数组遍历
来源：http://ae.bjjhwx.cn

for my $x (@arr) { print $x; }
来源：http://zw.newstarts.cn

[T46] Perl：哈希操作
来源：http://dv.bjjhwx.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ow.huixiangedu.cn

[T47] Perl：正则捕获
来源：http://mx.haigaiapp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://yp.colortex.cn

[T48] Perl：正则替换
来源：http://vy.colortex.cn

$s =~ s/old/new/g;
来源：http://uj.wgjwhj.cn

[T49] Perl：函数
来源：http://sw.muxihuayi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dw.shxzukj.cn

[T50] Perl：逐行读文件
来源：http://ys.szxytkj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://hx.newstarts.cn

while (my $line = <$fh>) { print $line; }
来源：http://zb.muxihuayi.cn

[T51] Scala：Hello World
来源：http://no.colortex.cn

println("Hello")
来源：http://dk.yuexingan06.cn

[T52] Scala：变量
来源：http://ja.bookmarksfly.cn

val a = 1;  var b = 2
来源：http://ff.nszjky.cn

[T53] Scala：字符串插值
来源：http://vp.bjjhwx.cn

s"值: $b"
来源：http://nh.shxzukj.cn

[T54] Scala：集合映射
来源：http://go.chemitech.net.cn

List(1, 2, 3).map(_ * 2)
来源：http://zr.9csxet.cn

[T55] Scala：集合过滤
来源：http://ue.colortex.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ms.9csxet.cn

[T56] Scala：样例类
来源：http://av.shtwfgs.cn

case class User(name: String, age: Int)
来源：http://vf.szsharing.cn

[T57] Scala：模式匹配
来源：http://iu.bjjhwx.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://rr.hnjuh.cn

[T58] Scala：函数定义
来源：http://we.gzmigu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://mp.gzmigu.cn

[T59] Scala：循环
来源：http://we.lnxyls.cn

for (i <- 1 to 10) println(i)
来源：http://qn.shtwfgs.cn

[T60] Scala：折叠
来源：http://yw.lnxyls.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ti.jianghongdianzi.cn

================================================================================
来源：http://nb.muxihuayi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hu.newstarts.cn

================================================================================
来源：http://gx.gzmigu.cn

[U01] Py：创建虚拟环境
来源：http://zj.chemitech.net.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ud.huanxung.cn

[U02] Py：导出 / 安装依赖
来源：http://xr.yuexingan06.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zo.nicolike.cn

[U03] Py：加载 .env 配置
来源：http://il.panjiajie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://jm.colortex.cn

[U04] Py：变量调试打印
来源：http://ai.muxihuayi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://iu.hnjuh.cn

[U05] Py：列表去重且保序
来源：http://my.gzmigu.cn

list(dict.fromkeys(arr))
来源：http://fy.shxzskj.cn

[U06] Py：合并两个字典
来源：http://vo.huixinmuqiang.cn

{**a, **b}
来源：http://da.yuntaijiaju.cn

[U07] Py：反转字典键值
来源：http://gw.panjiajie.cn

{v: k for k, v in d.items()}
来源：http://zf.shxzukj.cn

[U08] Py：展平二维列表
来源：http://ai.nicolike.cn

[y for x in nested for y in x]
来源：http://wa.haigaiapp.cn

[U09] Py：字典取最大值的键
来源：http://nz.wgjwhj.cn

max(d, key=d.get)
来源：http://ey.shxzskj.cn

[U10] Py：按值排序字典
来源：http://kd.bookmarksfly.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nv.bjjhwx.cn

[U11] Py：生成器表达式
来源：http://mb.9csxet.cn

(x * 2 for x in arr)
来源：http://hc.gzmigu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ua.nszjky.cn

Counter(arr).most_common(3)
来源：http://el.asd995.cn

[U13] Py：固定长度队列
来源：http://gu.panjiajie.cn

deque(maxlen=10)
来源：http://ml.szsharing.cn

[U14] Py：分组收集到列表
来源：http://lb.asd995.cn

defaultdict(list)
来源：http://rh.colortex.cn

[U15] Py：高精度计时
来源：http://nh.jctech888.com.cn

t = time.perf_counter()
来源：http://ah.hahajie.cn

[U16] Py：命令行参数解析
来源：http://jy.nszjky.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ee.bookmarksfly.cn

[U17] Py：初始化日志
来源：http://it.chemitech.net.cn

logging.basicConfig(level=logging.INFO)
来源：http://cc.wgjwhj.cn

[U18] Py：预编译正则
来源：http://sd.asd995.cn

pat = re.compile(r"\d+")
来源：http://fz.shxzskj.cn

[U19] Py：正则替换带回调
来源：http://cf.nszjky.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tm.bjjhwx.cn

[U20] Py：缓存函数结果
来源：http://dw.nszjky.cn

@functools.lru_cache(maxsize=None)
来源：http://pi.panjiajie.cn


<!-- 参考信息 -->