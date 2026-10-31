代发 wailian999

S. C / C++ 专题
来源：http://ge.jianghongdianzi.cn

================================================================================
来源：http://xs.shtwfgs.cn

[S01] C：Hello World
来源：http://ja.chemitech.net.cn

#include <stdio.h>
来源：http://gq.shxzukj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://yz.newstarts.cn

[S02] C：变量与格式化输出
来源：http://kq.shtwfgs.cn

int a = 10; printf("%d\n", a);
来源：http://ov.huanxung.cn

[S03] C：读入整数
来源：http://sz.nicolike.cn

int x; scanf("%d", &x);
来源：http://wt.huanxung.cn

[S04] C：字符串复制
来源：http://bl.szsharing.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ie.521024.cn

[S05] C：字符串长度
来源：http://wd.shxzskj.cn

strlen(s)
来源：http://tr.haigaiapp.cn

[S06] C：字符串比较
来源：http://mw.chemitech.net.cn

strcmp(a, b) == 0
来源：http://jc.chemitech.net.cn

[S07] C：数组遍历求和
来源：http://hm.shxzukj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nf.hnjuh.cn

[S08] C：动态内存分配与释放
来源：http://do.szxytkj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cs.wgjwhj.cn

[S09] C：结构体定义与初始化
来源：http://tr.wgjwhj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kt.shxzskj.cn

[S10] C：指针与解引用
来源：http://wm.huanxung.cn

int *p = &a;  *p = 5;
来源：http://ja.szsharing.cn

[S11] C：逐行读文件
来源：http://sz.nicolike.cn

FILE *f = fopen("a.txt", "r");
来源：http://rv.shxzukj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wp.szxytkj.cn

fclose(f);
来源：http://pd.shxzukj.cn

[S12] C：写文件
来源：http://tl.chemitech.net.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jn.shxzskj.cn

[S13] C：宏定义
来源：http://on.yuexingan06.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://oj.jianghongdianzi.cn

[S14] C：枚举
来源：http://cr.521024.cn

enum Color { RED, GREEN, BLUE };
来源：http://oq.bookmarksfly.cn

[S15] C：类型转换
来源：http://xe.bookmarksfly.cn

(double) a / b
来源：http://db.shxzukj.cn

[S16] C：位操作置位
来源：http://ij.nicolike.cn

x |= (1 << 3);
来源：http://ga.521024.cn

[S17] C：安全拼接字符串
来源：http://xa.lnxyls.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://oa.muxihuayi.cn

[S18] C：命令行参数
来源：http://wj.huanxung.cn

int main(int argc, char **argv)
来源：http://bx.shtwfgs.cn

[S19] C：快速排序
来源：http://tw.shxzukj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vf.bjjhwx.cn

[S20] C：二分查找
来源：http://rr.gzmigu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sy.shxzukj.cn

[S21] C：字符类别判断
来源：http://wu.huixinmuqiang.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://af.bookmarksfly.cn

[S22] C：字符串转数字
来源：http://ev.lnxyls.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nv.lnxyls.cn

[S23] C：随机数
来源：http://xr.521024.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cw.521024.cn

[S24] C：获取本地时间
来源：http://av.shtwfgs.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ap.huixinmuqiang.cn

[S25] C：内存拷贝
来源：http://bs.shxzskj.cn

memcpy(dst, src, n);
来源：http://xf.hnjuh.cn

[S26] C：内存清零
来源：http://fl.shxzukj.cn

memset(a, 0, sizeof a);
来源：http://zz.hahajie.cn

[S27] C：定义常量
来源：http://vi.szxytkj.cn

const double PI = 3.14159;
来源：http://su.bookmarksfly.cn

[S28] C：静态变量
来源：http://dr.newstarts.cn

static int counter = 0;
来源：http://ty.gzmigu.cn

[S29] C：变参函数
来源：http://yz.panjiajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qi.shtwfgs.cn

[S30] C：头文件保护
来源：http://mv.jctech888.com.cn

#ifndef X_H
来源：http://je.haigaiapp.cn

#define X_H
来源：http://uh.newstarts.cn

#endif
来源：http://wp.newstarts.cn

[S31] C++：Hello World
来源：http://ig.szxytkj.cn

#include <iostream>
来源：http://pd.shtwfgs.cn

int main() { std::cout << "Hello\n"; }
来源：http://jt.yuntaijiaju.cn

[S32] C++：字符串
来源：http://xl.yuexingan06.cn

std::string s = "hi";  s += "!";
来源：http://ot.huixiangedu.cn

[S33] C++：vector 增删
来源：http://am.wgjwhj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fn.huanxung.cn

[S34] C++：遍历 vector
来源：http://wc.wgjwhj.cn

for (auto &x : v) { std::cout << x; }
来源：http://dw.jctech888.com.cn

[S35] C++：map
来源：http://th.nszjky.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://oh.hahajie.cn

[S36] C++：unordered_map
来源：http://bj.yuntaijiaju.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hb.9csxet.cn

[S37] C++：set
来源：http://bg.hahajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ah.lnxyls.cn

[S38] C++：排序
来源：http://qc.panjiajie.cn

std::sort(v.begin(), v.end());
来源：http://ss.gzmigu.cn

[S39] C++：自定义比较器排序
来源：http://fw.chemitech.net.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xk.asd995.cn

[S40] C++：查找元素
来源：http://di.szxytkj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hl.shtwfgs.cn

[S41] C++：类与构造函数
来源：http://vh.bjjhwx.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ee.lnxyls.cn

[S42] C++：继承与虚函数
来源：http://oj.huixinmuqiang.cn

class B : public Base { public: void f() override {} };
来源：http://qb.9csxet.cn

[S43] C++：智能指针
来源：http://ni.jianghongdianzi.cn

auto p = std::make_unique<int>(5);
来源：http://pb.yuexingan06.cn

[S44] C++：引用传参
来源：http://xe.shtwfgs.cn

void inc(int &x) { ++x; }
来源：http://nf.hahajie.cn

[S45] C++：lambda
来源：http://eb.wgjwhj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hp.bjjhwx.cn

[S46] C++：函数模板
来源：http://ji.bjjhwx.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tc.521024.cn

[S47] C++：结构化绑定遍历
来源：http://rr.szxytkj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://va.huixiangedu.cn

[S48] C++：逐行读文件
来源：http://aj.asd995.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ue.yuexingan06.cn

while (std::getline(in, line)) { }
来源：http://ab.shxzskj.cn

[S49] C++：写文件
来源：http://oe.lnxyls.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kz.nicolike.cn

[S50] C++：格式化数字
来源：http://tk.jctech888.com.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ny.bjjhwx.cn

[S51] C++：显式类型转换
来源：http://ve.shxzskj.cn

static_cast<double>(a) / b
来源：http://pm.bjjhwx.cn

[S52] C++：const 与 noexcept
来源：http://hx.jctech888.com.cn

int size() const noexcept { return n_; }
来源：http://gx.szsharing.cn

[S53] C++：移动语义
来源：http://jm.asd995.cn

std::vector<int> w = std::move(v);
来源：http://zk.huanxung.cn

[S54] C++：异常处理
来源：http://uk.huixinmuqiang.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://he.szsharing.cn

[S55] C++：结构化绑定
来源：http://ce.9csxet.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ok.jianghongdianzi.cn

[S56] C++：optional
来源：http://mo.jianghongdianzi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ft.lnxyls.cn

[S57] C++：编译期常量
来源：http://on.haigaiapp.cn

constexpr int N = 10;
来源：http://fa.huixiangedu.cn

[S58] C++：命名空间
来源：http://vh.bookmarksfly.cn

namespace ns { int f() { return 1; } }
来源：http://fx.newstarts.cn

[S59] C++：静态断言
来源：http://ol.yuntaijiaju.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://og.asd995.cn

[S60] C++：遍历并删除元素
来源：http://vq.jianghongdianzi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nu.huanxung.cn

================================================================================
来源：http://ni.wgjwhj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qv.bjjhwx.cn

================================================================================
来源：http://qu.haigaiapp.cn

[T01] Kotlin：Hello World
来源：http://cs.muxihuayi.cn

println("Hello")
来源：http://ki.gzmigu.cn

[T02] Kotlin：变量
来源：http://gu.shxzukj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ks.gzmigu.cn

[T03] Kotlin：字符串模板
来源：http://qx.hnjuh.cn

"值: $b"
来源：http://fh.wgjwhj.cn

[T04] Kotlin：空安全
来源：http://zu.yuntaijiaju.cn

val n: String? = null;  n?.length
来源：http://hp.panjiajie.cn

[T05] Kotlin：when 表达式
来源：http://fe.bookmarksfly.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kx.gzmigu.cn

[T06] Kotlin：集合映射
来源：http://ei.bookmarksfly.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://il.yuexingan06.cn

[T07] Kotlin：集合过滤
来源：http://rw.nicolike.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://nt.hnjuh.cn

[T08] Kotlin：数据类
来源：http://il.huixiangedu.cn

data class User(val name: String, val age: Int)
来源：http://kv.asd995.cn

[T09] Kotlin：扩展函数
来源：http://bg.colortex.cn

fun String.exclaim() = this + "!"
来源：http://mm.jctech888.com.cn

[T10] Kotlin：默认参数
来源：http://xq.jctech888.com.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wm.huanxung.cn

[T11] Kotlin：协程
来源：http://xw.521024.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://de.huixinmuqiang.cn

[T12] Kotlin：解构声明
来源：http://ke.jctech888.com.cn

val (a, b) = Pair(1, 2)
来源：http://kw.colortex.cn

[T13] Kotlin：只读 Map
来源：http://ab.jianghongdianzi.cn

val m = mapOf("a" to 1)
来源：http://ts.huixiangedu.cn

[T14] Kotlin：循环
来源：http://tg.panjiajie.cn

for (i in 1..10) println(i)
来源：http://ru.asd995.cn

[T15] Kotlin：接口
来源：http://iy.jctech888.com.cn

interface Shape { fun area(): Double }
来源：http://ds.huanxung.cn

[T16] Swift：Hello World
来源：http://gn.haigaiapp.cn

print("Hello")
来源：http://eh.jctech888.com.cn

[T17] Swift：变量与常量
来源：http://eq.jctech888.com.cn

var a = 1;  let b = 2
来源：http://wj.chemitech.net.cn

[T18] Swift：字符串插值
来源：http://mz.jianghongdianzi.cn

"值: \(b)"
来源：http://wv.jctech888.com.cn

[T19] Swift：可选绑定
来源：http://uj.jctech888.com.cn

if let n = opt { print(n) }
来源：http://db.panjiajie.cn

[T20] Swift：数组操作
来源：http://yw.bookmarksfly.cn

var a = [1, 2, 3];  a.append(4)
来源：http://sn.bjjhwx.cn

[T21] Swift：遍历
来源：http://vu.yuntaijiaju.cn

for x in a { print(x) }
来源：http://pl.hahajie.cn

[T22] Swift：字典
来源：http://go.haigaiapp.cn

var d = ["a": 1];  d["b"] = 2
来源：http://wl.bookmarksfly.cn

[T23] Swift：函数
来源：http://bf.asd995.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gd.jianghongdianzi.cn

[T24] Swift：闭包
来源：http://ic.panjiajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ht.szsharing.cn

[T25] Swift：结构体
来源：http://mz.panjiajie.cn

struct P { var x: Int }
来源：http://tj.lnxyls.cn

[T26] Swift：类与重写
来源：http://pe.jctech888.com.cn

class A: Base { override func f() {} }
来源：http://eh.9csxet.cn

[T27] Swift：错误处理
来源：http://jv.gzmigu.cn

do { try f() } catch { print(error) }
来源：http://ty.hnjuh.cn

[T28] Swift：枚举
来源：http://yv.521024.cn

enum Color { case red, green }
来源：http://vv.bjjhwx.cn

[T29] Swift：guard 提前返回
来源：http://qz.newstarts.cn

guard let x = opt else { return }
来源：http://gr.nszjky.cn

[T30] Swift：协议
来源：http://kh.nicolike.cn

protocol Shape { func area() -> Double }
来源：http://eb.521024.cn

[T31] Lua：Hello World
来源：http://fs.shtwfgs.cn

print("Hello")
来源：http://ml.bookmarksfly.cn

[T32] Lua：局部变量
来源：http://kv.huanxung.cn

local a = 1
来源：http://zc.shtwfgs.cn

[T33] Lua：表（数组）
来源：http://nw.huixiangedu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://my.chemitech.net.cn

[T34] Lua：遍历表
来源：http://bk.nicolike.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vo.jctech888.com.cn

[T35] Lua：字典表
来源：http://id.521024.cn

local d = { a = 1 };  d.b = 2
来源：http://be.panjiajie.cn

[T36] Lua：函数
来源：http://fm.shxzskj.cn

function add(a, b) return a + b end
来源：http://vd.shxzukj.cn

[T37] Lua：字符串拼接
来源：http://uh.521024.cn

"a" .. "b"
来源：http://em.nszjky.cn

[T38] Lua：条件
来源：http://qt.huixiangedu.cn

if x > 0 then print("正") end
来源：http://et.chemitech.net.cn

[T39] Lua：模式匹配
来源：http://de.hahajie.cn

string.find(s, "%d+")
来源：http://ho.muxihuayi.cn

[T40] Lua：元表
来源：http://pt.nicolike.cn

setmetatable({}, { __index = base })
来源：http://hd.lnxyls.cn

[T41] Perl：Hello World
来源：http://vv.colortex.cn

print "Hello\n";
来源：http://dn.shxzukj.cn

[T42] Perl：变量类型
来源：http://jt.huanxung.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wl.shxzskj.cn

[T43] Perl：字符串插值
来源：http://py.huanxung.cn

"值: $a"
来源：http://pf.panjiajie.cn

[T44] Perl：条件
来源：http://nb.muxihuayi.cn

if ($a > 0) { print "正"; }
来源：http://hf.bookmarksfly.cn

[T45] Perl：数组遍历
来源：http://xs.shxzskj.cn

for my $x (@arr) { print $x; }
来源：http://rj.szxytkj.cn

[T46] Perl：哈希操作
来源：http://uy.bookmarksfly.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qa.hahajie.cn

[T47] Perl：正则捕获
来源：http://ud.9csxet.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://zr.panjiajie.cn

[T48] Perl：正则替换
来源：http://kg.nicolike.cn

$s =~ s/old/new/g;
来源：http://ft.bookmarksfly.cn

[T49] Perl：函数
来源：http://in.haigaiapp.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zm.chemitech.net.cn

[T50] Perl：逐行读文件
来源：http://ya.gzmigu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://oo.colortex.cn

while (my $line = <$fh>) { print $line; }
来源：http://vz.yuntaijiaju.cn

[T51] Scala：Hello World
来源：http://de.szxytkj.cn

println("Hello")
来源：http://uu.wgjwhj.cn

[T52] Scala：变量
来源：http://gw.huanxung.cn

val a = 1;  var b = 2
来源：http://wa.hnjuh.cn

[T53] Scala：字符串插值
来源：http://bb.haigaiapp.cn

s"值: $b"
来源：http://tn.yuntaijiaju.cn

[T54] Scala：集合映射
来源：http://dn.huixiangedu.cn

List(1, 2, 3).map(_ * 2)
来源：http://dj.jianghongdianzi.cn

[T55] Scala：集合过滤
来源：http://en.hnjuh.cn

List(1, 2, 3).filter(_ > 1)
来源：http://my.9csxet.cn

[T56] Scala：样例类
来源：http://gz.wgjwhj.cn

case class User(name: String, age: Int)
来源：http://mw.jctech888.com.cn

[T57] Scala：模式匹配
来源：http://sm.bookmarksfly.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://lk.huanxung.cn

[T58] Scala：函数定义
来源：http://or.panjiajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://jz.nszjky.cn

[T59] Scala：循环
来源：http://rk.shxzskj.cn

for (i <- 1 to 10) println(i)
来源：http://py.colortex.cn

[T60] Scala：折叠
来源：http://tn.shxzukj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://af.haigaiapp.cn

================================================================================
来源：http://qi.521024.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xb.lnxyls.cn

================================================================================
来源：http://tp.szsharing.cn

[U01] Py：创建虚拟环境
来源：http://qv.lnxyls.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bx.wgjwhj.cn

[U02] Py：导出 / 安装依赖
来源：http://ze.jianghongdianzi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wb.jianghongdianzi.cn

[U03] Py：加载 .env 配置
来源：http://kg.huixiangedu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ty.colortex.cn

[U04] Py：变量调试打印
来源：http://ay.szsharing.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lg.panjiajie.cn

[U05] Py：列表去重且保序
来源：http://hp.huixiangedu.cn

list(dict.fromkeys(arr))
来源：http://ql.asd995.cn

[U06] Py：合并两个字典
来源：http://ia.9csxet.cn

{**a, **b}
来源：http://hw.wgjwhj.cn

[U07] Py：反转字典键值
来源：http://bq.jianghongdianzi.cn

{v: k for k, v in d.items()}
来源：http://ez.yuexingan06.cn

[U08] Py：展平二维列表
来源：http://mq.shxzskj.cn

[y for x in nested for y in x]
来源：http://ch.yuntaijiaju.cn

[U09] Py：字典取最大值的键
来源：http://qr.shtwfgs.cn

max(d, key=d.get)
来源：http://ko.panjiajie.cn

[U10] Py：按值排序字典
来源：http://ux.wgjwhj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uk.521024.cn

[U11] Py：生成器表达式
来源：http://xt.muxihuayi.cn

(x * 2 for x in arr)
来源：http://ij.haigaiapp.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qi.bookmarksfly.cn

Counter(arr).most_common(3)
来源：http://vg.nicolike.cn

[U13] Py：固定长度队列
来源：http://ee.shxzukj.cn

deque(maxlen=10)
来源：http://qs.nszjky.cn

[U14] Py：分组收集到列表
来源：http://af.bjjhwx.cn

defaultdict(list)
来源：http://fw.jctech888.com.cn

[U15] Py：高精度计时
来源：http://hr.wgjwhj.cn

t = time.perf_counter()
来源：http://bh.nicolike.cn

[U16] Py：命令行参数解析
来源：http://ha.chemitech.net.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yp.colortex.cn

[U17] Py：初始化日志
来源：http://sh.bjjhwx.cn

logging.basicConfig(level=logging.INFO)
来源：http://sb.colortex.cn

[U18] Py：预编译正则
来源：http://tr.colortex.cn

pat = re.compile(r"\d+")
来源：http://lq.521024.cn

[U19] Py：正则替换带回调
来源：http://hz.9csxet.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zj.muxihuayi.cn

[U20] Py：缓存函数结果
来源：http://cb.521024.cn

@functools.lru_cache(maxsize=None)
来源：http://ut.chemitech.net.cn

[U21] Py：自定义上下文管理器
来源：http://vk.nszjky.cn

@contextlib.contextmanager
来源：http://ap.wgjwhj.cn

[U22] Py：矩阵转置
来源：http://hf.gzmigu.cn

list(zip(*m))
来源：http://dk.nszjky.cn


<!-- 参考信息 -->