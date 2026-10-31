代发 wailian999

S. C / C++ 专题
来源：http://ka.huixinmuqiang.cn

================================================================================
来源：http://dm.9csxet.cn

[S01] C：Hello World
来源：http://hn.nicolike.cn

#include <stdio.h>
来源：http://an.jctech888.com.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fc.shxzskj.cn

[S02] C：变量与格式化输出
来源：http://rz.521024.cn

int a = 10; printf("%d\n", a);
来源：http://br.newstarts.cn

[S03] C：读入整数
来源：http://vc.shxzskj.cn

int x; scanf("%d", &x);
来源：http://zb.muxihuayi.cn

[S04] C：字符串复制
来源：http://rr.lnxyls.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xv.gzmigu.cn

[S05] C：字符串长度
来源：http://qe.asd995.cn

strlen(s)
来源：http://jp.chemitech.net.cn

[S06] C：字符串比较
来源：http://nn.chemitech.net.cn

strcmp(a, b) == 0
来源：http://mi.yuntaijiaju.cn

[S07] C：数组遍历求和
来源：http://xa.hnjuh.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sr.nicolike.cn

[S08] C：动态内存分配与释放
来源：http://an.nszjky.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ch.huanxung.cn

[S09] C：结构体定义与初始化
来源：http://gk.asd995.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gv.jctech888.com.cn

[S10] C：指针与解引用
来源：http://hg.hnjuh.cn

int *p = &a;  *p = 5;
来源：http://bd.huixiangedu.cn

[S11] C：逐行读文件
来源：http://gj.huixiangedu.cn

FILE *f = fopen("a.txt", "r");
来源：http://wh.colortex.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pb.jianghongdianzi.cn

fclose(f);
来源：http://pp.huixiangedu.cn

[S12] C：写文件
来源：http://tv.muxihuayi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ep.shxzukj.cn

[S13] C：宏定义
来源：http://vl.szsharing.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://em.wgjwhj.cn

[S14] C：枚举
来源：http://wk.shxzukj.cn

enum Color { RED, GREEN, BLUE };
来源：http://ov.nszjky.cn

[S15] C：类型转换
来源：http://ex.jianghongdianzi.cn

(double) a / b
来源：http://bf.haigaiapp.cn

[S16] C：位操作置位
来源：http://aa.9csxet.cn

x |= (1 << 3);
来源：http://yx.nicolike.cn

[S17] C：安全拼接字符串
来源：http://sz.lnxyls.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uj.szsharing.cn

[S18] C：命令行参数
来源：http://dy.colortex.cn

int main(int argc, char **argv)
来源：http://bi.521024.cn

[S19] C：快速排序
来源：http://rb.shxzukj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fy.newstarts.cn

[S20] C：二分查找
来源：http://hx.gzmigu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://oh.jianghongdianzi.cn

[S21] C：字符类别判断
来源：http://je.jianghongdianzi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nm.jctech888.com.cn

[S22] C：字符串转数字
来源：http://qg.colortex.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jq.hnjuh.cn

[S23] C：随机数
来源：http://zf.bookmarksfly.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://oc.muxihuayi.cn

[S24] C：获取本地时间
来源：http://ha.bookmarksfly.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ct.chemitech.net.cn

[S25] C：内存拷贝
来源：http://yx.haigaiapp.cn

memcpy(dst, src, n);
来源：http://yr.colortex.cn

[S26] C：内存清零
来源：http://op.szxytkj.cn

memset(a, 0, sizeof a);
来源：http://ne.bookmarksfly.cn

[S27] C：定义常量
来源：http://ks.szxytkj.cn

const double PI = 3.14159;
来源：http://uf.colortex.cn

[S28] C：静态变量
来源：http://kn.yuexingan06.cn

static int counter = 0;
来源：http://hb.chemitech.net.cn

[S29] C：变参函数
来源：http://yi.szsharing.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gm.shxzskj.cn

[S30] C：头文件保护
来源：http://as.bjjhwx.cn

#ifndef X_H
来源：http://or.lnxyls.cn

#define X_H
来源：http://bi.shxzskj.cn

#endif
来源：http://yu.hahajie.cn

[S31] C++：Hello World
来源：http://vm.nicolike.cn

#include <iostream>
来源：http://qz.jctech888.com.cn

int main() { std::cout << "Hello\n"; }
来源：http://dm.bjjhwx.cn

[S32] C++：字符串
来源：http://tb.asd995.cn

std::string s = "hi";  s += "!";
来源：http://ls.521024.cn

[S33] C++：vector 增删
来源：http://ak.hahajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kf.hnjuh.cn

[S34] C++：遍历 vector
来源：http://wm.lnxyls.cn

for (auto &x : v) { std::cout << x; }
来源：http://jw.hahajie.cn

[S35] C++：map
来源：http://sc.nicolike.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://al.szxytkj.cn

[S36] C++：unordered_map
来源：http://vw.shtwfgs.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zj.9csxet.cn

[S37] C++：set
来源：http://hj.szsharing.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wf.hahajie.cn

[S38] C++：排序
来源：http://tf.colortex.cn

std::sort(v.begin(), v.end());
来源：http://bo.gzmigu.cn

[S39] C++：自定义比较器排序
来源：http://gh.muxihuayi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nk.panjiajie.cn

[S40] C++：查找元素
来源：http://os.shtwfgs.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sh.bookmarksfly.cn

[S41] C++：类与构造函数
来源：http://vr.jctech888.com.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://em.nicolike.cn

[S42] C++：继承与虚函数
来源：http://lt.asd995.cn

class B : public Base { public: void f() override {} };
来源：http://lg.asd995.cn

[S43] C++：智能指针
来源：http://rn.jianghongdianzi.cn

auto p = std::make_unique<int>(5);
来源：http://wh.huixinmuqiang.cn

[S44] C++：引用传参
来源：http://wf.jctech888.com.cn

void inc(int &x) { ++x; }
来源：http://uk.asd995.cn

[S45] C++：lambda
来源：http://rf.shtwfgs.cn

auto add = [](int a, int b) { return a + b; };
来源：http://sp.jctech888.com.cn

[S46] C++：函数模板
来源：http://pw.huixiangedu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://un.bookmarksfly.cn

[S47] C++：结构化绑定遍历
来源：http://nd.huixiangedu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rb.jctech888.com.cn

[S48] C++：逐行读文件
来源：http://hu.huanxung.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jo.haigaiapp.cn

while (std::getline(in, line)) { }
来源：http://np.521024.cn

[S49] C++：写文件
来源：http://zl.newstarts.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ht.521024.cn

[S50] C++：格式化数字
来源：http://hq.521024.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://le.hnjuh.cn

[S51] C++：显式类型转换
来源：http://et.szsharing.cn

static_cast<double>(a) / b
来源：http://bn.newstarts.cn

[S52] C++：const 与 noexcept
来源：http://ff.shxzskj.cn

int size() const noexcept { return n_; }
来源：http://zt.shxzukj.cn

[S53] C++：移动语义
来源：http://wg.nicolike.cn

std::vector<int> w = std::move(v);
来源：http://ne.lnxyls.cn

[S54] C++：异常处理
来源：http://nm.gzmigu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lj.jianghongdianzi.cn

[S55] C++：结构化绑定
来源：http://yd.bjjhwx.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gp.colortex.cn

[S56] C++：optional
来源：http://ip.jctech888.com.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ho.gzmigu.cn

[S57] C++：编译期常量
来源：http://lr.nicolike.cn

constexpr int N = 10;
来源：http://pg.yuntaijiaju.cn

[S58] C++：命名空间
来源：http://zb.bjjhwx.cn

namespace ns { int f() { return 1; } }
来源：http://dg.haigaiapp.cn

[S59] C++：静态断言
来源：http://fy.asd995.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pe.nszjky.cn

[S60] C++：遍历并删除元素
来源：http://mf.huixiangedu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mr.huixinmuqiang.cn

================================================================================
来源：http://qn.jctech888.com.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gp.yuntaijiaju.cn

================================================================================
来源：http://cm.panjiajie.cn

[T01] Kotlin：Hello World
来源：http://ao.9csxet.cn

println("Hello")
来源：http://yj.chemitech.net.cn

[T02] Kotlin：变量
来源：http://mn.nszjky.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gp.yuntaijiaju.cn

[T03] Kotlin：字符串模板
来源：http://jr.nicolike.cn

"值: $b"
来源：http://ar.chemitech.net.cn

[T04] Kotlin：空安全
来源：http://ls.szxytkj.cn

val n: String? = null;  n?.length
来源：http://tl.szsharing.cn

[T05] Kotlin：when 表达式
来源：http://dr.hnjuh.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://no.yuexingan06.cn

[T06] Kotlin：集合映射
来源：http://bg.szxytkj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rv.huanxung.cn

[T07] Kotlin：集合过滤
来源：http://ud.muxihuayi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://so.lnxyls.cn

[T08] Kotlin：数据类
来源：http://xr.asd995.cn

data class User(val name: String, val age: Int)
来源：http://nj.hahajie.cn

[T09] Kotlin：扩展函数
来源：http://ya.hahajie.cn

fun String.exclaim() = this + "!"
来源：http://zy.shxzskj.cn

[T10] Kotlin：默认参数
来源：http://pq.jctech888.com.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://np.521024.cn

[T11] Kotlin：协程
来源：http://zd.newstarts.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://di.9csxet.cn

[T12] Kotlin：解构声明
来源：http://ul.bookmarksfly.cn

val (a, b) = Pair(1, 2)
来源：http://hp.panjiajie.cn

[T13] Kotlin：只读 Map
来源：http://mp.bookmarksfly.cn

val m = mapOf("a" to 1)
来源：http://qp.huixinmuqiang.cn

[T14] Kotlin：循环
来源：http://gs.shxzukj.cn

for (i in 1..10) println(i)
来源：http://yc.muxihuayi.cn

[T15] Kotlin：接口
来源：http://bw.hahajie.cn

interface Shape { fun area(): Double }
来源：http://gu.yuexingan06.cn

[T16] Swift：Hello World
来源：http://rt.huixinmuqiang.cn

print("Hello")
来源：http://ra.newstarts.cn

[T17] Swift：变量与常量
来源：http://ea.yuntaijiaju.cn

var a = 1;  let b = 2
来源：http://pg.yuntaijiaju.cn

[T18] Swift：字符串插值
来源：http://ii.szxytkj.cn

"值: \(b)"
来源：http://jq.colortex.cn

[T19] Swift：可选绑定
来源：http://me.huanxung.cn

if let n = opt { print(n) }
来源：http://ac.hahajie.cn

[T20] Swift：数组操作
来源：http://eh.jianghongdianzi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://bv.colortex.cn

[T21] Swift：遍历
来源：http://fj.huixiangedu.cn

for x in a { print(x) }
来源：http://fp.gzmigu.cn

[T22] Swift：字典
来源：http://jl.wgjwhj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ai.wgjwhj.cn

[T23] Swift：函数
来源：http://fx.nicolike.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ie.lnxyls.cn

[T24] Swift：闭包
来源：http://pb.huixinmuqiang.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ps.nicolike.cn

[T25] Swift：结构体
来源：http://qm.521024.cn

struct P { var x: Int }
来源：http://mk.asd995.cn

[T26] Swift：类与重写
来源：http://gt.shtwfgs.cn

class A: Base { override func f() {} }
来源：http://pm.shtwfgs.cn

[T27] Swift：错误处理
来源：http://oi.huixinmuqiang.cn

do { try f() } catch { print(error) }
来源：http://rt.jianghongdianzi.cn

[T28] Swift：枚举
来源：http://hx.huixiangedu.cn

enum Color { case red, green }
来源：http://ak.shxzskj.cn

[T29] Swift：guard 提前返回
来源：http://si.gzmigu.cn

guard let x = opt else { return }
来源：http://ex.jctech888.com.cn

[T30] Swift：协议
来源：http://ke.newstarts.cn

protocol Shape { func area() -> Double }
来源：http://fg.nicolike.cn

[T31] Lua：Hello World
来源：http://ja.asd995.cn

print("Hello")
来源：http://xq.szxytkj.cn

[T32] Lua：局部变量
来源：http://sw.9csxet.cn

local a = 1
来源：http://gy.9csxet.cn

[T33] Lua：表（数组）
来源：http://ne.yuntaijiaju.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ij.muxihuayi.cn

[T34] Lua：遍历表
来源：http://kk.newstarts.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zn.521024.cn

[T35] Lua：字典表
来源：http://rt.huanxung.cn

local d = { a = 1 };  d.b = 2
来源：http://ih.huanxung.cn

[T36] Lua：函数
来源：http://vg.bookmarksfly.cn

function add(a, b) return a + b end
来源：http://qa.jctech888.com.cn

[T37] Lua：字符串拼接
来源：http://oa.panjiajie.cn

"a" .. "b"
来源：http://lw.newstarts.cn

[T38] Lua：条件
来源：http://jd.shtwfgs.cn

if x > 0 then print("正") end
来源：http://yh.nszjky.cn

[T39] Lua：模式匹配
来源：http://gd.panjiajie.cn

string.find(s, "%d+")
来源：http://uz.panjiajie.cn

[T40] Lua：元表
来源：http://fv.lnxyls.cn

setmetatable({}, { __index = base })
来源：http://gf.chemitech.net.cn

[T41] Perl：Hello World
来源：http://dq.chemitech.net.cn

print "Hello\n";
来源：http://mv.huixiangedu.cn

[T42] Perl：变量类型
来源：http://gv.muxihuayi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mo.bookmarksfly.cn

[T43] Perl：字符串插值
来源：http://ig.huanxung.cn

"值: $a"
来源：http://yn.colortex.cn

[T44] Perl：条件
来源：http://ys.szsharing.cn

if ($a > 0) { print "正"; }
来源：http://zp.gzmigu.cn

[T45] Perl：数组遍历
来源：http://cd.haigaiapp.cn

for my $x (@arr) { print $x; }
来源：http://sg.gzmigu.cn

[T46] Perl：哈希操作
来源：http://eu.yuntaijiaju.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xi.bookmarksfly.cn

[T47] Perl：正则捕获
来源：http://xe.asd995.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xh.szxytkj.cn

[T48] Perl：正则替换
来源：http://jl.chemitech.net.cn

$s =~ s/old/new/g;
来源：http://uh.shtwfgs.cn

[T49] Perl：函数
来源：http://yk.szxytkj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nh.jianghongdianzi.cn

[T50] Perl：逐行读文件
来源：http://tu.huixiangedu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://bp.lnxyls.cn

while (my $line = <$fh>) { print $line; }
来源：http://it.colortex.cn

[T51] Scala：Hello World
来源：http://un.asd995.cn

println("Hello")
来源：http://cv.colortex.cn

[T52] Scala：变量
来源：http://ei.asd995.cn

val a = 1;  var b = 2
来源：http://gz.lnxyls.cn

[T53] Scala：字符串插值
来源：http://yp.shxzukj.cn

s"值: $b"
来源：http://sw.yuexingan06.cn

[T54] Scala：集合映射
来源：http://zz.huixiangedu.cn

List(1, 2, 3).map(_ * 2)
来源：http://aj.muxihuayi.cn

[T55] Scala：集合过滤
来源：http://dw.bjjhwx.cn

List(1, 2, 3).filter(_ > 1)
来源：http://tl.hnjuh.cn

[T56] Scala：样例类
来源：http://ge.shxzskj.cn

case class User(name: String, age: Int)
来源：http://xz.newstarts.cn

[T57] Scala：模式匹配
来源：http://wd.shxzukj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gb.huixiangedu.cn

[T58] Scala：函数定义
来源：http://wt.bjjhwx.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fi.szsharing.cn

[T59] Scala：循环
来源：http://gl.shxzukj.cn

for (i <- 1 to 10) println(i)
来源：http://sq.huixiangedu.cn

[T60] Scala：折叠
来源：http://jr.jctech888.com.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pu.shxzskj.cn

================================================================================
来源：http://eq.colortex.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zd.haigaiapp.cn

================================================================================
来源：http://av.lnxyls.cn

[U01] Py：创建虚拟环境
来源：http://ke.jctech888.com.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ih.huanxung.cn

[U02] Py：导出 / 安装依赖
来源：http://kb.shtwfgs.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ra.bjjhwx.cn

[U03] Py：加载 .env 配置
来源：http://sf.yuexingan06.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://jd.nszjky.cn

[U04] Py：变量调试打印
来源：http://gp.jctech888.com.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fk.colortex.cn

[U05] Py：列表去重且保序
来源：http://yk.bjjhwx.cn

list(dict.fromkeys(arr))
来源：http://zr.yuntaijiaju.cn

[U06] Py：合并两个字典
来源：http://ch.szxytkj.cn

{**a, **b}
来源：http://zq.chemitech.net.cn

[U07] Py：反转字典键值
来源：http://fv.panjiajie.cn

{v: k for k, v in d.items()}
来源：http://be.colortex.cn

[U08] Py：展平二维列表
来源：http://xu.nszjky.cn

[y for x in nested for y in x]
来源：http://gj.jianghongdianzi.cn

[U09] Py：字典取最大值的键
来源：http://cc.panjiajie.cn

max(d, key=d.get)
来源：http://za.jianghongdianzi.cn

[U10] Py：按值排序字典
来源：http://bz.huixiangedu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://oh.asd995.cn

[U11] Py：生成器表达式
来源：http://jk.huixinmuqiang.cn

(x * 2 for x in arr)
来源：http://md.yuntaijiaju.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qw.9csxet.cn

Counter(arr).most_common(3)
来源：http://jb.nicolike.cn

[U13] Py：固定长度队列
来源：http://aq.hnjuh.cn

deque(maxlen=10)
来源：http://ig.shxzskj.cn

[U14] Py：分组收集到列表
来源：http://kh.panjiajie.cn

defaultdict(list)
来源：http://wr.nicolike.cn

[U15] Py：高精度计时
来源：http://pw.shtwfgs.cn

t = time.perf_counter()
来源：http://yg.shxzukj.cn

[U16] Py：命令行参数解析
来源：http://tk.gzmigu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fr.szxytkj.cn

[U17] Py：初始化日志
来源：http://pi.bookmarksfly.cn

logging.basicConfig(level=logging.INFO)
来源：http://pm.huanxung.cn

[U18] Py：预编译正则
来源：http://eq.panjiajie.cn

pat = re.compile(r"\d+")
来源：http://nl.panjiajie.cn

[U19] Py：正则替换带回调
来源：http://nk.asd995.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fo.nszjky.cn

[U20] Py：缓存函数结果
来源：http://bv.wgjwhj.cn

@functools.lru_cache(maxsize=None)
来源：http://ek.nszjky.cn

[U21] Py：自定义上下文管理器
来源：http://vl.szsharing.cn

@contextlib.contextmanager
来源：http://wx.newstarts.cn

[U22] Py：矩阵转置
来源：http://yi.huanxung.cn

list(zip(*m))
来源：http://qa.yuexingan06.cn


<!-- 参考信息 -->