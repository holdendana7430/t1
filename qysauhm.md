代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cc.wgjwhj.cn

[R80] 查看脚本执行耗时
来源：http://pn.shxzskj.cn

time ./run.sh
来源：http://ke.jianghongdianzi.cn

================================================================================
来源：http://lm.panjiajie.cn

S. C / C++ 专题
来源：http://sk.shxzukj.cn

================================================================================
来源：http://la.521024.cn

[S01] C：Hello World
来源：http://ts.szxytkj.cn

#include <stdio.h>
来源：http://jv.yuntaijiaju.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://in.panjiajie.cn

[S02] C：变量与格式化输出
来源：http://wy.nicolike.cn

int a = 10; printf("%d\n", a);
来源：http://ur.jctech888.com.cn

[S03] C：读入整数
来源：http://hi.chemitech.net.cn

int x; scanf("%d", &x);
来源：http://gr.jctech888.com.cn

[S04] C：字符串复制
来源：http://ho.huixiangedu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://lr.panjiajie.cn

[S05] C：字符串长度
来源：http://gu.yuexingan06.cn

strlen(s)
来源：http://em.shxzskj.cn

[S06] C：字符串比较
来源：http://vz.bookmarksfly.cn

strcmp(a, b) == 0
来源：http://sh.huixiangedu.cn

[S07] C：数组遍历求和
来源：http://zg.lnxyls.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sb.haigaiapp.cn

[S08] C：动态内存分配与释放
来源：http://wj.yuntaijiaju.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yi.chemitech.net.cn

[S09] C：结构体定义与初始化
来源：http://re.haigaiapp.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dz.hahajie.cn

[S10] C：指针与解引用
来源：http://ry.szsharing.cn

int *p = &a;  *p = 5;
来源：http://gz.colortex.cn

[S11] C：逐行读文件
来源：http://vm.yuexingan06.cn

FILE *f = fopen("a.txt", "r");
来源：http://mo.bookmarksfly.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://an.newstarts.cn

fclose(f);
来源：http://rc.huanxung.cn

[S12] C：写文件
来源：http://bg.shxzukj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uu.shxzskj.cn

[S13] C：宏定义
来源：http://vw.nicolike.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pu.yuntaijiaju.cn

[S14] C：枚举
来源：http://xl.hahajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://dh.bjjhwx.cn

[S15] C：类型转换
来源：http://yf.nicolike.cn

(double) a / b
来源：http://nu.lnxyls.cn

[S16] C：位操作置位
来源：http://sp.shtwfgs.cn

x |= (1 << 3);
来源：http://ns.huanxung.cn

[S17] C：安全拼接字符串
来源：http://lg.jctech888.com.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://in.huixiangedu.cn

[S18] C：命令行参数
来源：http://kw.lnxyls.cn

int main(int argc, char **argv)
来源：http://oj.bjjhwx.cn

[S19] C：快速排序
来源：http://na.huixinmuqiang.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fq.yuntaijiaju.cn

[S20] C：二分查找
来源：http://vd.shxzukj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qt.muxihuayi.cn

[S21] C：字符类别判断
来源：http://al.gzmigu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nk.yuexingan06.cn

[S22] C：字符串转数字
来源：http://jd.szxytkj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://hx.huanxung.cn

[S23] C：随机数
来源：http://pz.asd995.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://jy.szxytkj.cn

[S24] C：获取本地时间
来源：http://uw.nszjky.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ig.haigaiapp.cn

[S25] C：内存拷贝
来源：http://kc.nszjky.cn

memcpy(dst, src, n);
来源：http://bl.colortex.cn

[S26] C：内存清零
来源：http://kn.haigaiapp.cn

memset(a, 0, sizeof a);
来源：http://oq.nszjky.cn

[S27] C：定义常量
来源：http://hp.gzmigu.cn

const double PI = 3.14159;
来源：http://xl.nicolike.cn

[S28] C：静态变量
来源：http://wd.shxzukj.cn

static int counter = 0;
来源：http://zw.muxihuayi.cn

[S29] C：变参函数
来源：http://zz.9csxet.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yd.huixinmuqiang.cn

[S30] C：头文件保护
来源：http://us.521024.cn

#ifndef X_H
来源：http://lf.chemitech.net.cn

#define X_H
来源：http://sm.szxytkj.cn

#endif
来源：http://xz.colortex.cn

[S31] C++：Hello World
来源：http://ap.panjiajie.cn

#include <iostream>
来源：http://va.hahajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://ls.haigaiapp.cn

[S32] C++：字符串
来源：http://xe.nicolike.cn

std::string s = "hi";  s += "!";
来源：http://mx.jctech888.com.cn

[S33] C++：vector 增删
来源：http://su.lnxyls.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lw.szsharing.cn

[S34] C++：遍历 vector
来源：http://up.nszjky.cn

for (auto &x : v) { std::cout << x; }
来源：http://ny.shtwfgs.cn

[S35] C++：map
来源：http://yw.gzmigu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gk.nicolike.cn

[S36] C++：unordered_map
来源：http://ig.nszjky.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://un.yuntaijiaju.cn

[S37] C++：set
来源：http://wu.huixinmuqiang.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pa.shxzskj.cn

[S38] C++：排序
来源：http://yk.wgjwhj.cn

std::sort(v.begin(), v.end());
来源：http://fi.gzmigu.cn

[S39] C++：自定义比较器排序
来源：http://jl.haigaiapp.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bz.hahajie.cn

[S40] C++：查找元素
来源：http://td.chemitech.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pg.lnxyls.cn

[S41] C++：类与构造函数
来源：http://vl.521024.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pc.521024.cn

[S42] C++：继承与虚函数
来源：http://lo.colortex.cn

class B : public Base { public: void f() override {} };
来源：http://uw.shtwfgs.cn

[S43] C++：智能指针
来源：http://ai.shxzskj.cn

auto p = std::make_unique<int>(5);
来源：http://dn.shxzukj.cn

[S44] C++：引用传参
来源：http://dk.muxihuayi.cn

void inc(int &x) { ++x; }
来源：http://yh.gzmigu.cn

[S45] C++：lambda
来源：http://tn.jctech888.com.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ac.yuexingan06.cn

[S46] C++：函数模板
来源：http://mt.shxzskj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vp.lnxyls.cn

[S47] C++：结构化绑定遍历
来源：http://ym.wgjwhj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zk.haigaiapp.cn

[S48] C++：逐行读文件
来源：http://ux.hahajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fk.bjjhwx.cn

while (std::getline(in, line)) { }
来源：http://in.newstarts.cn

[S49] C++：写文件
来源：http://ar.nicolike.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yq.newstarts.cn

[S50] C++：格式化数字
来源：http://cy.asd995.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jn.huixiangedu.cn

[S51] C++：显式类型转换
来源：http://hq.shtwfgs.cn

static_cast<double>(a) / b
来源：http://nk.szxytkj.cn

[S52] C++：const 与 noexcept
来源：http://pm.shxzskj.cn

int size() const noexcept { return n_; }
来源：http://tx.shxzukj.cn

[S53] C++：移动语义
来源：http://uy.nicolike.cn

std::vector<int> w = std::move(v);
来源：http://cl.panjiajie.cn

[S54] C++：异常处理
来源：http://kt.jctech888.com.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://az.szsharing.cn

[S55] C++：结构化绑定
来源：http://cx.gzmigu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ws.nszjky.cn

[S56] C++：optional
来源：http://no.szsharing.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tn.bookmarksfly.cn

[S57] C++：编译期常量
来源：http://ik.yuexingan06.cn

constexpr int N = 10;
来源：http://ka.hnjuh.cn

[S58] C++：命名空间
来源：http://te.muxihuayi.cn

namespace ns { int f() { return 1; } }
来源：http://uo.asd995.cn

[S59] C++：静态断言
来源：http://ud.nszjky.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ug.shxzskj.cn

[S60] C++：遍历并删除元素
来源：http://ep.wgjwhj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rc.yuntaijiaju.cn

================================================================================
来源：http://ih.hahajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ij.haigaiapp.cn

================================================================================
来源：http://il.jctech888.com.cn

[T01] Kotlin：Hello World
来源：http://pv.jianghongdianzi.cn

println("Hello")
来源：http://nl.jianghongdianzi.cn

[T02] Kotlin：变量
来源：http://dy.nicolike.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mo.bookmarksfly.cn

[T03] Kotlin：字符串模板
来源：http://bm.yuexingan06.cn

"值: $b"
来源：http://gd.9csxet.cn

[T04] Kotlin：空安全
来源：http://ki.yuntaijiaju.cn

val n: String? = null;  n?.length
来源：http://da.521024.cn

[T05] Kotlin：when 表达式
来源：http://my.lnxyls.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mx.jianghongdianzi.cn

[T06] Kotlin：集合映射
来源：http://aq.newstarts.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://dl.shxzskj.cn

[T07] Kotlin：集合过滤
来源：http://pu.newstarts.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vl.yuexingan06.cn

[T08] Kotlin：数据类
来源：http://lp.wgjwhj.cn

data class User(val name: String, val age: Int)
来源：http://gy.gzmigu.cn

[T09] Kotlin：扩展函数
来源：http://lp.muxihuayi.cn

fun String.exclaim() = this + "!"
来源：http://di.shtwfgs.cn

[T10] Kotlin：默认参数
来源：http://hk.huixiangedu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://lu.bookmarksfly.cn

[T11] Kotlin：协程
来源：http://ja.yuexingan06.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xc.bookmarksfly.cn

[T12] Kotlin：解构声明
来源：http://ns.jctech888.com.cn

val (a, b) = Pair(1, 2)
来源：http://rj.9csxet.cn

[T13] Kotlin：只读 Map
来源：http://hg.yuexingan06.cn

val m = mapOf("a" to 1)
来源：http://bd.panjiajie.cn

[T14] Kotlin：循环
来源：http://sl.yuntaijiaju.cn

for (i in 1..10) println(i)
来源：http://iv.muxihuayi.cn

[T15] Kotlin：接口
来源：http://iu.szxytkj.cn

interface Shape { fun area(): Double }
来源：http://bf.nicolike.cn

[T16] Swift：Hello World
来源：http://li.huixiangedu.cn

print("Hello")
来源：http://fk.haigaiapp.cn

[T17] Swift：变量与常量
来源：http://cv.huixiangedu.cn

var a = 1;  let b = 2
来源：http://ud.9csxet.cn

[T18] Swift：字符串插值
来源：http://bo.yuexingan06.cn

"值: \(b)"
来源：http://rh.shxzskj.cn

[T19] Swift：可选绑定
来源：http://bn.huixiangedu.cn

if let n = opt { print(n) }
来源：http://aw.chemitech.net.cn

[T20] Swift：数组操作
来源：http://gv.gzmigu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://al.huanxung.cn

[T21] Swift：遍历
来源：http://im.9csxet.cn

for x in a { print(x) }
来源：http://cw.jctech888.com.cn

[T22] Swift：字典
来源：http://vf.521024.cn

var d = ["a": 1];  d["b"] = 2
来源：http://nd.colortex.cn

[T23] Swift：函数
来源：http://oc.asd995.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sx.wgjwhj.cn

[T24] Swift：闭包
来源：http://ho.wgjwhj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ql.huanxung.cn

[T25] Swift：结构体
来源：http://ve.shtwfgs.cn

struct P { var x: Int }
来源：http://fx.panjiajie.cn

[T26] Swift：类与重写
来源：http://sc.szxytkj.cn

class A: Base { override func f() {} }
来源：http://sb.huixiangedu.cn

[T27] Swift：错误处理
来源：http://nu.bookmarksfly.cn

do { try f() } catch { print(error) }
来源：http://cd.colortex.cn

[T28] Swift：枚举
来源：http://qw.wgjwhj.cn

enum Color { case red, green }
来源：http://bl.szsharing.cn

[T29] Swift：guard 提前返回
来源：http://vx.9csxet.cn

guard let x = opt else { return }
来源：http://yx.shxzskj.cn

[T30] Swift：协议
来源：http://ok.shxzskj.cn

protocol Shape { func area() -> Double }
来源：http://ry.shxzukj.cn

[T31] Lua：Hello World
来源：http://kr.szxytkj.cn

print("Hello")
来源：http://cb.colortex.cn

[T32] Lua：局部变量
来源：http://yj.bjjhwx.cn

local a = 1
来源：http://sw.huixiangedu.cn

[T33] Lua：表（数组）
来源：http://wx.wgjwhj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://jd.huixinmuqiang.cn

[T34] Lua：遍历表
来源：http://gx.jianghongdianzi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ol.521024.cn

[T35] Lua：字典表
来源：http://da.szsharing.cn

local d = { a = 1 };  d.b = 2
来源：http://eu.jianghongdianzi.cn

[T36] Lua：函数
来源：http://iw.colortex.cn

function add(a, b) return a + b end
来源：http://rd.shxzukj.cn

[T37] Lua：字符串拼接
来源：http://td.shtwfgs.cn

"a" .. "b"
来源：http://wo.bookmarksfly.cn

[T38] Lua：条件
来源：http://qg.szsharing.cn

if x > 0 then print("正") end
来源：http://hg.newstarts.cn

[T39] Lua：模式匹配
来源：http://md.bjjhwx.cn

string.find(s, "%d+")
来源：http://xh.szxytkj.cn

[T40] Lua：元表
来源：http://tg.haigaiapp.cn

setmetatable({}, { __index = base })
来源：http://nj.huanxung.cn

[T41] Perl：Hello World
来源：http://qe.szxytkj.cn

print "Hello\n";
来源：http://ct.jctech888.com.cn

[T42] Perl：变量类型
来源：http://tm.bookmarksfly.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rg.haigaiapp.cn

[T43] Perl：字符串插值
来源：http://es.hahajie.cn

"值: $a"
来源：http://ag.newstarts.cn

[T44] Perl：条件
来源：http://mo.lnxyls.cn

if ($a > 0) { print "正"; }
来源：http://os.newstarts.cn

[T45] Perl：数组遍历
来源：http://wg.asd995.cn

for my $x (@arr) { print $x; }
来源：http://dv.shtwfgs.cn

[T46] Perl：哈希操作
来源：http://qk.bookmarksfly.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://iz.shtwfgs.cn

[T47] Perl：正则捕获
来源：http://ql.521024.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://bo.bjjhwx.cn

[T48] Perl：正则替换
来源：http://dc.szxytkj.cn

$s =~ s/old/new/g;
来源：http://sv.hnjuh.cn

[T49] Perl：函数
来源：http://pv.shtwfgs.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mq.huixiangedu.cn

[T50] Perl：逐行读文件
来源：http://ik.nicolike.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://sz.hnjuh.cn

while (my $line = <$fh>) { print $line; }
来源：http://kw.colortex.cn

[T51] Scala：Hello World
来源：http://dl.hahajie.cn

println("Hello")
来源：http://xj.hahajie.cn

[T52] Scala：变量
来源：http://xm.szxytkj.cn

val a = 1;  var b = 2
来源：http://zr.huanxung.cn

[T53] Scala：字符串插值
来源：http://de.huixiangedu.cn

s"值: $b"
来源：http://fi.muxihuayi.cn

[T54] Scala：集合映射
来源：http://jy.colortex.cn

List(1, 2, 3).map(_ * 2)
来源：http://ev.lnxyls.cn

[T55] Scala：集合过滤
来源：http://gh.jianghongdianzi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qd.nicolike.cn

[T56] Scala：样例类
来源：http://jz.lnxyls.cn

case class User(name: String, age: Int)
来源：http://gs.yuntaijiaju.cn

[T57] Scala：模式匹配
来源：http://lo.jianghongdianzi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ke.jctech888.com.cn

[T58] Scala：函数定义
来源：http://vx.newstarts.cn

def add(a: Int, b: Int): Int = a + b
来源：http://cv.hnjuh.cn

[T59] Scala：循环
来源：http://tf.hnjuh.cn

for (i <- 1 to 10) println(i)
来源：http://vp.colortex.cn

[T60] Scala：折叠
来源：http://dz.521024.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ns.newstarts.cn

================================================================================
来源：http://cb.521024.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dc.panjiajie.cn

================================================================================
来源：http://ld.wgjwhj.cn

[U01] Py：创建虚拟环境
来源：http://rj.521024.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wu.jianghongdianzi.cn

[U02] Py：导出 / 安装依赖
来源：http://rb.szsharing.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hi.bjjhwx.cn

[U03] Py：加载 .env 配置
来源：http://fo.huixiangedu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://iz.huixiangedu.cn

[U04] Py：变量调试打印
来源：http://fx.hnjuh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://oy.szsharing.cn

[U05] Py：列表去重且保序
来源：http://yx.shtwfgs.cn

list(dict.fromkeys(arr))
来源：http://bh.huixinmuqiang.cn

[U06] Py：合并两个字典
来源：http://mr.huixinmuqiang.cn

{**a, **b}
来源：http://iy.bookmarksfly.cn

[U07] Py：反转字典键值
来源：http://oi.chemitech.net.cn

{v: k for k, v in d.items()}
来源：http://yg.wgjwhj.cn

[U08] Py：展平二维列表
来源：http://ek.hahajie.cn

[y for x in nested for y in x]
来源：http://mv.hnjuh.cn

[U09] Py：字典取最大值的键
来源：http://ao.huixiangedu.cn

max(d, key=d.get)
来源：http://vs.newstarts.cn

[U10] Py：按值排序字典
来源：http://pl.shxzukj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ns.huixinmuqiang.cn

[U11] Py：生成器表达式
来源：http://rq.szxytkj.cn

(x * 2 for x in arr)
来源：http://eg.bookmarksfly.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lp.newstarts.cn

Counter(arr).most_common(3)
来源：http://mn.muxihuayi.cn

[U13] Py：固定长度队列
来源：http://ji.hahajie.cn

deque(maxlen=10)
来源：http://pv.bjjhwx.cn

[U14] Py：分组收集到列表
来源：http://mz.gzmigu.cn

defaultdict(list)
来源：http://ox.shtwfgs.cn

[U15] Py：高精度计时
来源：http://ib.yuntaijiaju.cn

t = time.perf_counter()
来源：http://bk.521024.cn

[U16] Py：命令行参数解析
来源：http://si.yuexingan06.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://da.wgjwhj.cn

[U17] Py：初始化日志
来源：http://om.521024.cn

logging.basicConfig(level=logging.INFO)
来源：http://ml.gzmigu.cn

[U18] Py：预编译正则
来源：http://sy.wgjwhj.cn

pat = re.compile(r"\d+")
来源：http://uh.huixinmuqiang.cn

[U19] Py：正则替换带回调
来源：http://wo.hnjuh.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ik.huixiangedu.cn

[U20] Py：缓存函数结果
来源：http://uy.nicolike.cn

@functools.lru_cache(maxsize=None)
来源：http://ln.bjjhwx.cn


<!-- 参考信息 -->