代发 wailian999

S. C / C++ 专题
来源：http://sa.nicolike.cn

================================================================================
来源：http://qd.yuexingan06.cn

[S01] C：Hello World
来源：http://re.panjiajie.cn

#include <stdio.h>
来源：http://bt.yuntaijiaju.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://km.shtwfgs.cn

[S02] C：变量与格式化输出
来源：http://jp.asd995.cn

int a = 10; printf("%d\n", a);
来源：http://ch.lnxyls.cn

[S03] C：读入整数
来源：http://zg.yuntaijiaju.cn

int x; scanf("%d", &x);
来源：http://qw.9csxet.cn

[S04] C：字符串复制
来源：http://ap.lnxyls.cn

char dst[32]; strcpy(dst, "hi");
来源：http://mr.huixinmuqiang.cn

[S05] C：字符串长度
来源：http://ma.shxzukj.cn

strlen(s)
来源：http://bz.yuexingan06.cn

[S06] C：字符串比较
来源：http://ip.yuexingan06.cn

strcmp(a, b) == 0
来源：http://qa.gzmigu.cn

[S07] C：数组遍历求和
来源：http://rx.hahajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qk.yuntaijiaju.cn

[S08] C：动态内存分配与释放
来源：http://hk.huanxung.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zi.szsharing.cn

[S09] C：结构体定义与初始化
来源：http://ah.panjiajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dj.jctech888.com.cn

[S10] C：指针与解引用
来源：http://xk.shxzukj.cn

int *p = &a;  *p = 5;
来源：http://yw.panjiajie.cn

[S11] C：逐行读文件
来源：http://jr.huixiangedu.cn

FILE *f = fopen("a.txt", "r");
来源：http://jz.wgjwhj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://oa.haigaiapp.cn

fclose(f);
来源：http://sc.haigaiapp.cn

[S12] C：写文件
来源：http://iy.bookmarksfly.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ev.chemitech.net.cn

[S13] C：宏定义
来源：http://pj.muxihuayi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rx.jctech888.com.cn

[S14] C：枚举
来源：http://bd.shxzskj.cn

enum Color { RED, GREEN, BLUE };
来源：http://gh.bookmarksfly.cn

[S15] C：类型转换
来源：http://nd.huixiangedu.cn

(double) a / b
来源：http://yh.muxihuayi.cn

[S16] C：位操作置位
来源：http://ye.wgjwhj.cn

x |= (1 << 3);
来源：http://oi.panjiajie.cn

[S17] C：安全拼接字符串
来源：http://qq.huanxung.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lh.wgjwhj.cn

[S18] C：命令行参数
来源：http://bg.lnxyls.cn

int main(int argc, char **argv)
来源：http://rz.bookmarksfly.cn

[S19] C：快速排序
来源：http://cu.521024.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jd.yuntaijiaju.cn

[S20] C：二分查找
来源：http://sv.9csxet.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ud.newstarts.cn

[S21] C：字符类别判断
来源：http://ha.chemitech.net.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wo.bookmarksfly.cn

[S22] C：字符串转数字
来源：http://no.jctech888.com.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nf.yuntaijiaju.cn

[S23] C：随机数
来源：http://az.szsharing.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ab.hnjuh.cn

[S24] C：获取本地时间
来源：http://mk.521024.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://iv.szsharing.cn

[S25] C：内存拷贝
来源：http://nr.nszjky.cn

memcpy(dst, src, n);
来源：http://nq.muxihuayi.cn

[S26] C：内存清零
来源：http://st.nicolike.cn

memset(a, 0, sizeof a);
来源：http://jt.521024.cn

[S27] C：定义常量
来源：http://nc.newstarts.cn

const double PI = 3.14159;
来源：http://ts.jctech888.com.cn

[S28] C：静态变量
来源：http://zm.haigaiapp.cn

static int counter = 0;
来源：http://ll.asd995.cn

[S29] C：变参函数
来源：http://nb.gzmigu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wf.huanxung.cn

[S30] C：头文件保护
来源：http://oo.bjjhwx.cn

#ifndef X_H
来源：http://mi.huanxung.cn

#define X_H
来源：http://zk.jctech888.com.cn

#endif
来源：http://gc.chemitech.net.cn

[S31] C++：Hello World
来源：http://aq.nszjky.cn

#include <iostream>
来源：http://ip.hnjuh.cn

int main() { std::cout << "Hello\n"; }
来源：http://yy.9csxet.cn

[S32] C++：字符串
来源：http://nq.colortex.cn

std::string s = "hi";  s += "!";
来源：http://xo.yuntaijiaju.cn

[S33] C++：vector 增删
来源：http://kj.nszjky.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yo.chemitech.net.cn

[S34] C++：遍历 vector
来源：http://vn.jctech888.com.cn

for (auto &x : v) { std::cout << x; }
来源：http://tx.nicolike.cn

[S35] C++：map
来源：http://un.521024.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zo.newstarts.cn

[S36] C++：unordered_map
来源：http://pn.yuexingan06.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sh.szxytkj.cn

[S37] C++：set
来源：http://gr.panjiajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ax.hahajie.cn

[S38] C++：排序
来源：http://ql.hnjuh.cn

std::sort(v.begin(), v.end());
来源：http://ca.nicolike.cn

[S39] C++：自定义比较器排序
来源：http://tk.szxytkj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mv.asd995.cn

[S40] C++：查找元素
来源：http://td.hahajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gq.huixinmuqiang.cn

[S41] C++：类与构造函数
来源：http://oy.newstarts.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://iv.muxihuayi.cn

[S42] C++：继承与虚函数
来源：http://wh.nszjky.cn

class B : public Base { public: void f() override {} };
来源：http://bw.chemitech.net.cn

[S43] C++：智能指针
来源：http://qa.hnjuh.cn

auto p = std::make_unique<int>(5);
来源：http://wj.9csxet.cn

[S44] C++：引用传参
来源：http://yu.szsharing.cn

void inc(int &x) { ++x; }
来源：http://mv.wgjwhj.cn

[S45] C++：lambda
来源：http://cv.newstarts.cn

auto add = [](int a, int b) { return a + b; };
来源：http://at.nicolike.cn

[S46] C++：函数模板
来源：http://qp.gzmigu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://oc.nicolike.cn

[S47] C++：结构化绑定遍历
来源：http://fd.chemitech.net.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://au.wgjwhj.cn

[S48] C++：逐行读文件
来源：http://da.9csxet.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kd.shxzskj.cn

while (std::getline(in, line)) { }
来源：http://vs.colortex.cn

[S49] C++：写文件
来源：http://dz.shxzukj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kl.shtwfgs.cn

[S50] C++：格式化数字
来源：http://bi.szxytkj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://aj.nszjky.cn

[S51] C++：显式类型转换
来源：http://ig.huixinmuqiang.cn

static_cast<double>(a) / b
来源：http://qv.nszjky.cn

[S52] C++：const 与 noexcept
来源：http://ig.szxytkj.cn

int size() const noexcept { return n_; }
来源：http://wt.yuntaijiaju.cn

[S53] C++：移动语义
来源：http://oq.szxytkj.cn

std::vector<int> w = std::move(v);
来源：http://xm.asd995.cn

[S54] C++：异常处理
来源：http://cg.asd995.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uq.hnjuh.cn

[S55] C++：结构化绑定
来源：http://ml.huanxung.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kb.hahajie.cn

[S56] C++：optional
来源：http://hh.szxytkj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tq.asd995.cn

[S57] C++：编译期常量
来源：http://up.huixinmuqiang.cn

constexpr int N = 10;
来源：http://nf.jianghongdianzi.cn

[S58] C++：命名空间
来源：http://vo.hahajie.cn

namespace ns { int f() { return 1; } }
来源：http://nq.bjjhwx.cn

[S59] C++：静态断言
来源：http://je.huanxung.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ob.newstarts.cn

[S60] C++：遍历并删除元素
来源：http://ww.asd995.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rz.huixiangedu.cn

================================================================================
来源：http://bw.asd995.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hx.colortex.cn

================================================================================
来源：http://sx.yuntaijiaju.cn

[T01] Kotlin：Hello World
来源：http://ov.shtwfgs.cn

println("Hello")
来源：http://fy.shxzskj.cn

[T02] Kotlin：变量
来源：http://kt.huixiangedu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ck.yuntaijiaju.cn

[T03] Kotlin：字符串模板
来源：http://yd.haigaiapp.cn

"值: $b"
来源：http://ve.huixinmuqiang.cn

[T04] Kotlin：空安全
来源：http://pj.shtwfgs.cn

val n: String? = null;  n?.length
来源：http://ld.lnxyls.cn

[T05] Kotlin：when 表达式
来源：http://lt.nicolike.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tl.panjiajie.cn

[T06] Kotlin：集合映射
来源：http://gi.haigaiapp.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gp.bookmarksfly.cn

[T07] Kotlin：集合过滤
来源：http://gn.jctech888.com.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qw.yuntaijiaju.cn

[T08] Kotlin：数据类
来源：http://gw.9csxet.cn

data class User(val name: String, val age: Int)
来源：http://zi.shxzukj.cn

[T09] Kotlin：扩展函数
来源：http://da.hnjuh.cn

fun String.exclaim() = this + "!"
来源：http://xe.asd995.cn

[T10] Kotlin：默认参数
来源：http://vu.hnjuh.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vs.yuexingan06.cn

[T11] Kotlin：协程
来源：http://nb.hnjuh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://cu.colortex.cn

[T12] Kotlin：解构声明
来源：http://vn.asd995.cn

val (a, b) = Pair(1, 2)
来源：http://nb.nicolike.cn

[T13] Kotlin：只读 Map
来源：http://tq.colortex.cn

val m = mapOf("a" to 1)
来源：http://xl.hnjuh.cn

[T14] Kotlin：循环
来源：http://wx.shxzskj.cn

for (i in 1..10) println(i)
来源：http://ry.shtwfgs.cn

[T15] Kotlin：接口
来源：http://xp.nszjky.cn

interface Shape { fun area(): Double }
来源：http://ud.muxihuayi.cn

[T16] Swift：Hello World
来源：http://dy.huixinmuqiang.cn

print("Hello")
来源：http://aq.nszjky.cn

[T17] Swift：变量与常量
来源：http://zb.9csxet.cn

var a = 1;  let b = 2
来源：http://rv.huanxung.cn

[T18] Swift：字符串插值
来源：http://mg.bookmarksfly.cn

"值: \(b)"
来源：http://so.chemitech.net.cn

[T19] Swift：可选绑定
来源：http://we.chemitech.net.cn

if let n = opt { print(n) }
来源：http://le.521024.cn

[T20] Swift：数组操作
来源：http://sr.hnjuh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://re.shxzukj.cn

[T21] Swift：遍历
来源：http://fe.haigaiapp.cn

for x in a { print(x) }
来源：http://oo.yuntaijiaju.cn

[T22] Swift：字典
来源：http://xn.szxytkj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://pi.jianghongdianzi.cn

[T23] Swift：函数
来源：http://th.chemitech.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qs.huixiangedu.cn

[T24] Swift：闭包
来源：http://wc.shtwfgs.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://rq.wgjwhj.cn

[T25] Swift：结构体
来源：http://ug.hnjuh.cn

struct P { var x: Int }
来源：http://du.nszjky.cn

[T26] Swift：类与重写
来源：http://bn.shtwfgs.cn

class A: Base { override func f() {} }
来源：http://as.huanxung.cn

[T27] Swift：错误处理
来源：http://rh.szsharing.cn

do { try f() } catch { print(error) }
来源：http://bw.9csxet.cn

[T28] Swift：枚举
来源：http://wm.yuntaijiaju.cn

enum Color { case red, green }
来源：http://de.shtwfgs.cn

[T29] Swift：guard 提前返回
来源：http://uh.bookmarksfly.cn

guard let x = opt else { return }
来源：http://lq.hahajie.cn

[T30] Swift：协议
来源：http://bz.yuntaijiaju.cn

protocol Shape { func area() -> Double }
来源：http://yv.shxzukj.cn

[T31] Lua：Hello World
来源：http://sr.huixiangedu.cn

print("Hello")
来源：http://qi.shxzukj.cn

[T32] Lua：局部变量
来源：http://ax.shxzskj.cn

local a = 1
来源：http://dh.jianghongdianzi.cn

[T33] Lua：表（数组）
来源：http://ez.bookmarksfly.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://be.huanxung.cn

[T34] Lua：遍历表
来源：http://nr.hahajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zj.shxzskj.cn

[T35] Lua：字典表
来源：http://xj.shxzukj.cn

local d = { a = 1 };  d.b = 2
来源：http://mh.hahajie.cn

[T36] Lua：函数
来源：http://cy.haigaiapp.cn

function add(a, b) return a + b end
来源：http://kq.9csxet.cn

[T37] Lua：字符串拼接
来源：http://qy.yuexingan06.cn

"a" .. "b"
来源：http://kt.newstarts.cn

[T38] Lua：条件
来源：http://jv.asd995.cn

if x > 0 then print("正") end
来源：http://yb.chemitech.net.cn

[T39] Lua：模式匹配
来源：http://cl.shxzukj.cn

string.find(s, "%d+")
来源：http://of.lnxyls.cn

[T40] Lua：元表
来源：http://bu.haigaiapp.cn

setmetatable({}, { __index = base })
来源：http://gi.chemitech.net.cn

[T41] Perl：Hello World
来源：http://om.huanxung.cn

print "Hello\n";
来源：http://du.bookmarksfly.cn

[T42] Perl：变量类型
来源：http://tr.szsharing.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://do.jianghongdianzi.cn

[T43] Perl：字符串插值
来源：http://or.jctech888.com.cn

"值: $a"
来源：http://ye.chemitech.net.cn

[T44] Perl：条件
来源：http://vu.nicolike.cn

if ($a > 0) { print "正"; }
来源：http://wf.asd995.cn

[T45] Perl：数组遍历
来源：http://pa.shtwfgs.cn

for my $x (@arr) { print $x; }
来源：http://bw.huixinmuqiang.cn

[T46] Perl：哈希操作
来源：http://nd.jianghongdianzi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cq.shxzukj.cn

[T47] Perl：正则捕获
来源：http://bv.chemitech.net.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://hb.521024.cn

[T48] Perl：正则替换
来源：http://fm.wgjwhj.cn

$s =~ s/old/new/g;
来源：http://uk.huixinmuqiang.cn

[T49] Perl：函数
来源：http://qf.bjjhwx.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hh.yuexingan06.cn

[T50] Perl：逐行读文件
来源：http://cc.szxytkj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zt.colortex.cn

while (my $line = <$fh>) { print $line; }
来源：http://wb.colortex.cn

[T51] Scala：Hello World
来源：http://dc.lnxyls.cn

println("Hello")
来源：http://fm.bjjhwx.cn

[T52] Scala：变量
来源：http://nq.hahajie.cn

val a = 1;  var b = 2
来源：http://fa.hahajie.cn

[T53] Scala：字符串插值
来源：http://ty.yuntaijiaju.cn

s"值: $b"
来源：http://bx.gzmigu.cn

[T54] Scala：集合映射
来源：http://uy.haigaiapp.cn

List(1, 2, 3).map(_ * 2)
来源：http://cs.asd995.cn

[T55] Scala：集合过滤
来源：http://va.colortex.cn

List(1, 2, 3).filter(_ > 1)
来源：http://pb.lnxyls.cn

[T56] Scala：样例类
来源：http://bt.yuntaijiaju.cn

case class User(name: String, age: Int)
来源：http://yi.yuexingan06.cn

[T57] Scala：模式匹配
来源：http://vx.nszjky.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://xd.szxytkj.cn

[T58] Scala：函数定义
来源：http://ye.hahajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bn.lnxyls.cn

[T59] Scala：循环
来源：http://yg.huixinmuqiang.cn

for (i <- 1 to 10) println(i)
来源：http://fw.gzmigu.cn

[T60] Scala：折叠
来源：http://fz.shxzukj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jf.chemitech.net.cn

================================================================================
来源：http://gl.bjjhwx.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ti.haigaiapp.cn

================================================================================
来源：http://sy.szsharing.cn

[U01] Py：创建虚拟环境
来源：http://gc.nicolike.cn

python -m venv .venv && source .venv/bin/activate
来源：http://dk.huixiangedu.cn

[U02] Py：导出 / 安装依赖
来源：http://sy.panjiajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bg.asd995.cn

[U03] Py：加载 .env 配置
来源：http://xc.521024.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://kc.jctech888.com.cn

[U04] Py：变量调试打印
来源：http://uy.asd995.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nq.haigaiapp.cn

[U05] Py：列表去重且保序
来源：http://nq.gzmigu.cn

list(dict.fromkeys(arr))
来源：http://ef.panjiajie.cn

[U06] Py：合并两个字典
来源：http://nr.colortex.cn

{**a, **b}
来源：http://ic.panjiajie.cn

[U07] Py：反转字典键值
来源：http://rp.muxihuayi.cn

{v: k for k, v in d.items()}
来源：http://lw.jianghongdianzi.cn

[U08] Py：展平二维列表
来源：http://oj.yuntaijiaju.cn

[y for x in nested for y in x]
来源：http://gp.yuntaijiaju.cn

[U09] Py：字典取最大值的键
来源：http://wq.yuexingan06.cn

max(d, key=d.get)
来源：http://mf.newstarts.cn

[U10] Py：按值排序字典
来源：http://fy.colortex.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wm.yuntaijiaju.cn

[U11] Py：生成器表达式
来源：http://xs.lnxyls.cn

(x * 2 for x in arr)
来源：http://kd.9csxet.cn

[U12] Py：取出现最多的 3 个元素
来源：http://iq.huixinmuqiang.cn

Counter(arr).most_common(3)
来源：http://zg.nszjky.cn

[U13] Py：固定长度队列
来源：http://fc.huixiangedu.cn

deque(maxlen=10)
来源：http://va.szsharing.cn

[U14] Py：分组收集到列表
来源：http://cs.shtwfgs.cn

defaultdict(list)
来源：http://ru.9csxet.cn

[U15] Py：高精度计时
来源：http://wp.huanxung.cn

t = time.perf_counter()
来源：http://py.shtwfgs.cn

[U16] Py：命令行参数解析
来源：http://cu.haigaiapp.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ia.nicolike.cn

[U17] Py：初始化日志
来源：http://jg.haigaiapp.cn

logging.basicConfig(level=logging.INFO)
来源：http://iz.yuntaijiaju.cn

[U18] Py：预编译正则
来源：http://ns.chemitech.net.cn

pat = re.compile(r"\d+")
来源：http://it.hahajie.cn

[U19] Py：正则替换带回调
来源：http://mm.huixiangedu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qm.jctech888.com.cn

[U20] Py：缓存函数结果
来源：http://ql.haigaiapp.cn

@functools.lru_cache(maxsize=None)
来源：http://rw.newstarts.cn

[U21] Py：自定义上下文管理器
来源：http://gk.nicolike.cn

@contextlib.contextmanager
来源：http://ow.huixinmuqiang.cn

[U22] Py：矩阵转置
来源：http://gu.hahajie.cn

list(zip(*m))
来源：http://zn.haigaiapp.cn


<!-- 参考信息 -->