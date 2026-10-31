代发 wailian999

read -rp "请输入: " ans
来源：http://hg.hnjuh.cn

[R78] 交互式菜单
来源：http://gu.yuntaijiaju.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://bz.szxytkj.cn

[R79] 解析命令行选项
来源：http://fg.huanxung.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fe.jctech888.com.cn

[R80] 查看脚本执行耗时
来源：http://yu.shxzskj.cn

time ./run.sh
来源：http://vs.jianghongdianzi.cn

================================================================================
来源：http://on.newstarts.cn

S. C / C++ 专题
来源：http://th.bookmarksfly.cn

================================================================================
来源：http://oo.jctech888.com.cn

[S01] C：Hello World
来源：http://cz.chemitech.net.cn

#include <stdio.h>
来源：http://ch.haigaiapp.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xo.yuexingan06.cn

[S02] C：变量与格式化输出
来源：http://kf.nicolike.cn

int a = 10; printf("%d\n", a);
来源：http://yr.yuntaijiaju.cn

[S03] C：读入整数
来源：http://xy.shtwfgs.cn

int x; scanf("%d", &x);
来源：http://zg.nszjky.cn

[S04] C：字符串复制
来源：http://hs.asd995.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wg.jianghongdianzi.cn

[S05] C：字符串长度
来源：http://rm.lnxyls.cn

strlen(s)
来源：http://hv.521024.cn

[S06] C：字符串比较
来源：http://yq.gzmigu.cn

strcmp(a, b) == 0
来源：http://qq.bjjhwx.cn

[S07] C：数组遍历求和
来源：http://yf.wgjwhj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cm.szxytkj.cn

[S08] C：动态内存分配与释放
来源：http://si.nicolike.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ai.newstarts.cn

[S09] C：结构体定义与初始化
来源：http://gq.lnxyls.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fl.chemitech.net.cn

[S10] C：指针与解引用
来源：http://kd.gzmigu.cn

int *p = &a;  *p = 5;
来源：http://eo.shtwfgs.cn

[S11] C：逐行读文件
来源：http://nq.hnjuh.cn

FILE *f = fopen("a.txt", "r");
来源：http://fu.chemitech.net.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zl.shxzskj.cn

fclose(f);
来源：http://kd.lnxyls.cn

[S12] C：写文件
来源：http://ar.hahajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cs.gzmigu.cn

[S13] C：宏定义
来源：http://im.huixiangedu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://iu.yuntaijiaju.cn

[S14] C：枚举
来源：http://gi.haigaiapp.cn

enum Color { RED, GREEN, BLUE };
来源：http://mw.521024.cn

[S15] C：类型转换
来源：http://eu.huixinmuqiang.cn

(double) a / b
来源：http://yb.yuexingan06.cn

[S16] C：位操作置位
来源：http://ag.lnxyls.cn

x |= (1 << 3);
来源：http://ba.huixinmuqiang.cn

[S17] C：安全拼接字符串
来源：http://ce.521024.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ev.colortex.cn

[S18] C：命令行参数
来源：http://wk.huixiangedu.cn

int main(int argc, char **argv)
来源：http://rt.huixiangedu.cn

[S19] C：快速排序
来源：http://rt.jctech888.com.cn

qsort(a, n, sizeof(int), cmp);
来源：http://hy.colortex.cn

[S20] C：二分查找
来源：http://yk.yuexingan06.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dr.bookmarksfly.cn

[S21] C：字符类别判断
来源：http://uo.colortex.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ni.shxzskj.cn

[S22] C：字符串转数字
来源：http://df.wgjwhj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://al.521024.cn

[S23] C：随机数
来源：http://uq.hahajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hv.bjjhwx.cn

[S24] C：获取本地时间
来源：http://fu.bjjhwx.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ng.jctech888.com.cn

[S25] C：内存拷贝
来源：http://qk.newstarts.cn

memcpy(dst, src, n);
来源：http://uo.haigaiapp.cn

[S26] C：内存清零
来源：http://yd.huixiangedu.cn

memset(a, 0, sizeof a);
来源：http://xl.bjjhwx.cn

[S27] C：定义常量
来源：http://wo.panjiajie.cn

const double PI = 3.14159;
来源：http://zu.gzmigu.cn

[S28] C：静态变量
来源：http://zk.nszjky.cn

static int counter = 0;
来源：http://je.haigaiapp.cn

[S29] C：变参函数
来源：http://ir.hahajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kl.shxzskj.cn

[S30] C：头文件保护
来源：http://wc.jianghongdianzi.cn

#ifndef X_H
来源：http://em.huanxung.cn

#define X_H
来源：http://bh.bookmarksfly.cn

#endif
来源：http://ot.panjiajie.cn

[S31] C++：Hello World
来源：http://ml.colortex.cn

#include <iostream>
来源：http://fa.szsharing.cn

int main() { std::cout << "Hello\n"; }
来源：http://td.newstarts.cn

[S32] C++：字符串
来源：http://rt.newstarts.cn

std::string s = "hi";  s += "!";
来源：http://qc.jctech888.com.cn

[S33] C++：vector 增删
来源：http://iu.shxzskj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ew.haigaiapp.cn

[S34] C++：遍历 vector
来源：http://uh.9csxet.cn

for (auto &x : v) { std::cout << x; }
来源：http://go.wgjwhj.cn

[S35] C++：map
来源：http://nn.lnxyls.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xq.newstarts.cn

[S36] C++：unordered_map
来源：http://tb.huixiangedu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dn.hahajie.cn

[S37] C++：set
来源：http://ym.asd995.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hx.huanxung.cn

[S38] C++：排序
来源：http://yz.9csxet.cn

std::sort(v.begin(), v.end());
来源：http://bd.chemitech.net.cn

[S39] C++：自定义比较器排序
来源：http://ri.yuntaijiaju.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://eb.jianghongdianzi.cn

[S40] C++：查找元素
来源：http://vz.shtwfgs.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sl.bookmarksfly.cn

[S41] C++：类与构造函数
来源：http://yg.jianghongdianzi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tw.nszjky.cn

[S42] C++：继承与虚函数
来源：http://yj.huanxung.cn

class B : public Base { public: void f() override {} };
来源：http://rg.bjjhwx.cn

[S43] C++：智能指针
来源：http://em.yuexingan06.cn

auto p = std::make_unique<int>(5);
来源：http://le.jctech888.com.cn

[S44] C++：引用传参
来源：http://cc.szsharing.cn

void inc(int &x) { ++x; }
来源：http://fg.bookmarksfly.cn

[S45] C++：lambda
来源：http://lq.shxzskj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://yf.hnjuh.cn

[S46] C++：函数模板
来源：http://ol.haigaiapp.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bh.huixiangedu.cn

[S47] C++：结构化绑定遍历
来源：http://cu.jctech888.com.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qr.huixinmuqiang.cn

[S48] C++：逐行读文件
来源：http://la.521024.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ab.bookmarksfly.cn

while (std::getline(in, line)) { }
来源：http://bu.chemitech.net.cn

[S49] C++：写文件
来源：http://jo.bookmarksfly.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jo.wgjwhj.cn

[S50] C++：格式化数字
来源：http://jc.shxzukj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nd.shtwfgs.cn

[S51] C++：显式类型转换
来源：http://zy.chemitech.net.cn

static_cast<double>(a) / b
来源：http://yj.haigaiapp.cn

[S52] C++：const 与 noexcept
来源：http://tp.gzmigu.cn

int size() const noexcept { return n_; }
来源：http://bw.gzmigu.cn

[S53] C++：移动语义
来源：http://pz.szxytkj.cn

std::vector<int> w = std::move(v);
来源：http://pw.bookmarksfly.cn

[S54] C++：异常处理
来源：http://ly.jianghongdianzi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kt.huixinmuqiang.cn

[S55] C++：结构化绑定
来源：http://hh.yuntaijiaju.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://us.hahajie.cn

[S56] C++：optional
来源：http://qv.nicolike.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ee.bjjhwx.cn

[S57] C++：编译期常量
来源：http://tx.hahajie.cn

constexpr int N = 10;
来源：http://qy.lnxyls.cn

[S58] C++：命名空间
来源：http://dc.asd995.cn

namespace ns { int f() { return 1; } }
来源：http://vr.bookmarksfly.cn

[S59] C++：静态断言
来源：http://ne.hnjuh.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dt.hnjuh.cn

[S60] C++：遍历并删除元素
来源：http://bm.jctech888.com.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xr.chemitech.net.cn

================================================================================
来源：http://bk.szsharing.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://en.hnjuh.cn

================================================================================
来源：http://wr.9csxet.cn

[T01] Kotlin：Hello World
来源：http://ad.gzmigu.cn

println("Hello")
来源：http://xg.huanxung.cn

[T02] Kotlin：变量
来源：http://mt.9csxet.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://of.hnjuh.cn

[T03] Kotlin：字符串模板
来源：http://ev.panjiajie.cn

"值: $b"
来源：http://ti.shxzskj.cn

[T04] Kotlin：空安全
来源：http://kx.shxzukj.cn

val n: String? = null;  n?.length
来源：http://cs.yuexingan06.cn

[T05] Kotlin：when 表达式
来源：http://ov.asd995.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cj.haigaiapp.cn

[T06] Kotlin：集合映射
来源：http://bj.bjjhwx.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://cu.hahajie.cn

[T07] Kotlin：集合过滤
来源：http://oc.nicolike.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://do.panjiajie.cn

[T08] Kotlin：数据类
来源：http://gp.asd995.cn

data class User(val name: String, val age: Int)
来源：http://cd.hnjuh.cn

[T09] Kotlin：扩展函数
来源：http://gi.chemitech.net.cn

fun String.exclaim() = this + "!"
来源：http://mh.hahajie.cn

[T10] Kotlin：默认参数
来源：http://hm.chemitech.net.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://uv.bookmarksfly.cn

[T11] Kotlin：协程
来源：http://oc.huixiangedu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://mc.szxytkj.cn

[T12] Kotlin：解构声明
来源：http://ae.hahajie.cn

val (a, b) = Pair(1, 2)
来源：http://yl.shxzskj.cn

[T13] Kotlin：只读 Map
来源：http://my.nicolike.cn

val m = mapOf("a" to 1)
来源：http://yw.szsharing.cn

[T14] Kotlin：循环
来源：http://ow.muxihuayi.cn

for (i in 1..10) println(i)
来源：http://op.bookmarksfly.cn

[T15] Kotlin：接口
来源：http://cl.9csxet.cn

interface Shape { fun area(): Double }
来源：http://zk.colortex.cn

[T16] Swift：Hello World
来源：http://hb.jctech888.com.cn

print("Hello")
来源：http://ai.shtwfgs.cn

[T17] Swift：变量与常量
来源：http://vt.shxzskj.cn

var a = 1;  let b = 2
来源：http://ci.shtwfgs.cn

[T18] Swift：字符串插值
来源：http://se.chemitech.net.cn

"值: \(b)"
来源：http://co.gzmigu.cn

[T19] Swift：可选绑定
来源：http://qa.newstarts.cn

if let n = opt { print(n) }
来源：http://ih.9csxet.cn

[T20] Swift：数组操作
来源：http://do.huanxung.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ts.521024.cn

[T21] Swift：遍历
来源：http://uv.huixiangedu.cn

for x in a { print(x) }
来源：http://lc.jianghongdianzi.cn

[T22] Swift：字典
来源：http://hh.521024.cn

var d = ["a": 1];  d["b"] = 2
来源：http://kh.haigaiapp.cn

[T23] Swift：函数
来源：http://df.jianghongdianzi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qs.huixinmuqiang.cn

[T24] Swift：闭包
来源：http://ol.wgjwhj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://es.muxihuayi.cn

[T25] Swift：结构体
来源：http://hy.szxytkj.cn

struct P { var x: Int }
来源：http://gf.bjjhwx.cn

[T26] Swift：类与重写
来源：http://su.lnxyls.cn

class A: Base { override func f() {} }
来源：http://rc.wgjwhj.cn

[T27] Swift：错误处理
来源：http://cu.9csxet.cn

do { try f() } catch { print(error) }
来源：http://ix.panjiajie.cn

[T28] Swift：枚举
来源：http://uy.huixiangedu.cn

enum Color { case red, green }
来源：http://uk.wgjwhj.cn

[T29] Swift：guard 提前返回
来源：http://by.jianghongdianzi.cn

guard let x = opt else { return }
来源：http://se.nszjky.cn

[T30] Swift：协议
来源：http://ie.chemitech.net.cn

protocol Shape { func area() -> Double }
来源：http://dq.newstarts.cn

[T31] Lua：Hello World
来源：http://ua.asd995.cn

print("Hello")
来源：http://fq.asd995.cn

[T32] Lua：局部变量
来源：http://vc.wgjwhj.cn

local a = 1
来源：http://py.asd995.cn

[T33] Lua：表（数组）
来源：http://nd.huixinmuqiang.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ns.shtwfgs.cn

[T34] Lua：遍历表
来源：http://pi.shxzskj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ja.hahajie.cn

[T35] Lua：字典表
来源：http://ts.shxzukj.cn

local d = { a = 1 };  d.b = 2
来源：http://py.jctech888.com.cn

[T36] Lua：函数
来源：http://sb.hnjuh.cn

function add(a, b) return a + b end
来源：http://an.jctech888.com.cn

[T37] Lua：字符串拼接
来源：http://zm.chemitech.net.cn

"a" .. "b"
来源：http://nr.jctech888.com.cn

[T38] Lua：条件
来源：http://gu.shxzukj.cn

if x > 0 then print("正") end
来源：http://px.nicolike.cn

[T39] Lua：模式匹配
来源：http://wb.nszjky.cn

string.find(s, "%d+")
来源：http://im.hahajie.cn

[T40] Lua：元表
来源：http://hz.yuntaijiaju.cn

setmetatable({}, { __index = base })
来源：http://ou.newstarts.cn

[T41] Perl：Hello World
来源：http://bm.szsharing.cn

print "Hello\n";
来源：http://sr.huixiangedu.cn

[T42] Perl：变量类型
来源：http://nl.shtwfgs.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ux.jianghongdianzi.cn

[T43] Perl：字符串插值
来源：http://hm.9csxet.cn

"值: $a"
来源：http://ia.newstarts.cn

[T44] Perl：条件
来源：http://an.bookmarksfly.cn

if ($a > 0) { print "正"; }
来源：http://kz.hnjuh.cn

[T45] Perl：数组遍历
来源：http://th.nicolike.cn

for my $x (@arr) { print $x; }
来源：http://zv.panjiajie.cn

[T46] Perl：哈希操作
来源：http://mk.panjiajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ub.chemitech.net.cn

[T47] Perl：正则捕获
来源：http://wd.haigaiapp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://yn.huixiangedu.cn

[T48] Perl：正则替换
来源：http://ye.gzmigu.cn

$s =~ s/old/new/g;
来源：http://kf.nicolike.cn

[T49] Perl：函数
来源：http://ah.lnxyls.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xt.bjjhwx.cn

[T50] Perl：逐行读文件
来源：http://vh.szsharing.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wt.wgjwhj.cn

while (my $line = <$fh>) { print $line; }
来源：http://pe.bjjhwx.cn

[T51] Scala：Hello World
来源：http://zv.chemitech.net.cn

println("Hello")
来源：http://uo.hahajie.cn

[T52] Scala：变量
来源：http://px.nszjky.cn

val a = 1;  var b = 2
来源：http://fa.haigaiapp.cn

[T53] Scala：字符串插值
来源：http://ug.yuntaijiaju.cn

s"值: $b"
来源：http://iu.nicolike.cn

[T54] Scala：集合映射
来源：http://gf.lnxyls.cn

List(1, 2, 3).map(_ * 2)
来源：http://ei.szsharing.cn

[T55] Scala：集合过滤
来源：http://xo.chemitech.net.cn

List(1, 2, 3).filter(_ > 1)
来源：http://aj.haigaiapp.cn

[T56] Scala：样例类
来源：http://op.shtwfgs.cn

case class User(name: String, age: Int)
来源：http://ht.newstarts.cn

[T57] Scala：模式匹配
来源：http://cc.szsharing.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://it.lnxyls.cn

[T58] Scala：函数定义
来源：http://wg.shtwfgs.cn

def add(a: Int, b: Int): Int = a + b
来源：http://og.shxzskj.cn

[T59] Scala：循环
来源：http://hw.szsharing.cn

for (i <- 1 to 10) println(i)
来源：http://gd.asd995.cn

[T60] Scala：折叠
来源：http://tn.huanxung.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nn.yuntaijiaju.cn

================================================================================
来源：http://tm.asd995.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bg.muxihuayi.cn

================================================================================
来源：http://aw.bjjhwx.cn

[U01] Py：创建虚拟环境
来源：http://zu.huixinmuqiang.cn

python -m venv .venv && source .venv/bin/activate
来源：http://su.jianghongdianzi.cn

[U02] Py：导出 / 安装依赖
来源：http://xm.colortex.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://da.bjjhwx.cn

[U03] Py：加载 .env 配置
来源：http://iv.haigaiapp.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://im.yuntaijiaju.cn

[U04] Py：变量调试打印
来源：http://wg.szsharing.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jk.huixiangedu.cn

[U05] Py：列表去重且保序
来源：http://sy.chemitech.net.cn

list(dict.fromkeys(arr))
来源：http://jz.bookmarksfly.cn

[U06] Py：合并两个字典
来源：http://ws.hnjuh.cn

{**a, **b}
来源：http://ax.yuexingan06.cn

[U07] Py：反转字典键值
来源：http://me.jctech888.com.cn

{v: k for k, v in d.items()}
来源：http://xc.panjiajie.cn

[U08] Py：展平二维列表
来源：http://ys.bjjhwx.cn

[y for x in nested for y in x]
来源：http://ij.nszjky.cn

[U09] Py：字典取最大值的键
来源：http://qk.szsharing.cn

max(d, key=d.get)
来源：http://zn.colortex.cn

[U10] Py：按值排序字典
来源：http://bt.9csxet.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hw.newstarts.cn

[U11] Py：生成器表达式
来源：http://dv.asd995.cn

(x * 2 for x in arr)
来源：http://fm.panjiajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://sc.newstarts.cn

Counter(arr).most_common(3)
来源：http://zz.asd995.cn

[U13] Py：固定长度队列
来源：http://ez.lnxyls.cn

deque(maxlen=10)
来源：http://wi.yuntaijiaju.cn

[U14] Py：分组收集到列表
来源：http://tc.huixiangedu.cn

defaultdict(list)
来源：http://ry.nicolike.cn

[U15] Py：高精度计时
来源：http://vt.panjiajie.cn

t = time.perf_counter()
来源：http://qz.jianghongdianzi.cn

[U16] Py：命令行参数解析
来源：http://ch.haigaiapp.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sp.shxzskj.cn

[U17] Py：初始化日志
来源：http://hn.wgjwhj.cn

logging.basicConfig(level=logging.INFO)
来源：http://nu.bjjhwx.cn

[U18] Py：预编译正则
来源：http://uc.jctech888.com.cn

pat = re.compile(r"\d+")
来源：http://ff.haigaiapp.cn


<!-- 参考信息 -->