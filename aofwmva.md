代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://le.chemitech.net.cn

[R80] 查看脚本执行耗时
来源：http://du.yuntaijiaju.cn

time ./run.sh
来源：http://eq.shtwfgs.cn

================================================================================
来源：http://fv.szxytkj.cn

S. C / C++ 专题
来源：http://na.nszjky.cn

================================================================================
来源：http://ys.lnxyls.cn

[S01] C：Hello World
来源：http://sh.asd995.cn

#include <stdio.h>
来源：http://lr.gzmigu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://zo.bookmarksfly.cn

[S02] C：变量与格式化输出
来源：http://oz.521024.cn

int a = 10; printf("%d\n", a);
来源：http://mn.bookmarksfly.cn

[S03] C：读入整数
来源：http://sp.jctech888.com.cn

int x; scanf("%d", &x);
来源：http://qf.hnjuh.cn

[S04] C：字符串复制
来源：http://ct.szsharing.cn

char dst[32]; strcpy(dst, "hi");
来源：http://em.nszjky.cn

[S05] C：字符串长度
来源：http://zr.huixiangedu.cn

strlen(s)
来源：http://sa.huixiangedu.cn

[S06] C：字符串比较
来源：http://rq.nicolike.cn

strcmp(a, b) == 0
来源：http://qo.9csxet.cn

[S07] C：数组遍历求和
来源：http://xe.szsharing.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gx.newstarts.cn

[S08] C：动态内存分配与释放
来源：http://kh.wgjwhj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://az.bjjhwx.cn

[S09] C：结构体定义与初始化
来源：http://gx.521024.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mn.shxzukj.cn

[S10] C：指针与解引用
来源：http://ke.yuntaijiaju.cn

int *p = &a;  *p = 5;
来源：http://mv.panjiajie.cn

[S11] C：逐行读文件
来源：http://ac.nicolike.cn

FILE *f = fopen("a.txt", "r");
来源：http://xb.bjjhwx.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xb.colortex.cn

fclose(f);
来源：http://av.bookmarksfly.cn

[S12] C：写文件
来源：http://xl.yuexingan06.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hu.hnjuh.cn

[S13] C：宏定义
来源：http://fi.panjiajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mv.wgjwhj.cn

[S14] C：枚举
来源：http://sa.haigaiapp.cn

enum Color { RED, GREEN, BLUE };
来源：http://vv.bookmarksfly.cn

[S15] C：类型转换
来源：http://qy.szxytkj.cn

(double) a / b
来源：http://nv.asd995.cn

[S16] C：位操作置位
来源：http://xn.yuexingan06.cn

x |= (1 << 3);
来源：http://qs.huanxung.cn

[S17] C：安全拼接字符串
来源：http://fa.hahajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://od.hnjuh.cn

[S18] C：命令行参数
来源：http://ho.huixiangedu.cn

int main(int argc, char **argv)
来源：http://jc.chemitech.net.cn

[S19] C：快速排序
来源：http://gm.yuntaijiaju.cn

qsort(a, n, sizeof(int), cmp);
来源：http://iw.yuntaijiaju.cn

[S20] C：二分查找
来源：http://hw.hahajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yj.newstarts.cn

[S21] C：字符类别判断
来源：http://wd.huanxung.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bw.521024.cn

[S22] C：字符串转数字
来源：http://ib.yuexingan06.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nu.huixinmuqiang.cn

[S23] C：随机数
来源：http://xt.newstarts.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vc.newstarts.cn

[S24] C：获取本地时间
来源：http://ax.chemitech.net.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bo.jianghongdianzi.cn

[S25] C：内存拷贝
来源：http://yf.muxihuayi.cn

memcpy(dst, src, n);
来源：http://bj.hnjuh.cn

[S26] C：内存清零
来源：http://nx.asd995.cn

memset(a, 0, sizeof a);
来源：http://jv.haigaiapp.cn

[S27] C：定义常量
来源：http://ee.lnxyls.cn

const double PI = 3.14159;
来源：http://yf.hahajie.cn

[S28] C：静态变量
来源：http://bu.gzmigu.cn

static int counter = 0;
来源：http://ll.nszjky.cn

[S29] C：变参函数
来源：http://ee.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kr.huixiangedu.cn

[S30] C：头文件保护
来源：http://xx.nszjky.cn

#ifndef X_H
来源：http://tp.colortex.cn

#define X_H
来源：http://fn.gzmigu.cn

#endif
来源：http://kw.chemitech.net.cn

[S31] C++：Hello World
来源：http://cb.yuntaijiaju.cn

#include <iostream>
来源：http://rf.bjjhwx.cn

int main() { std::cout << "Hello\n"; }
来源：http://zt.gzmigu.cn

[S32] C++：字符串
来源：http://cg.shtwfgs.cn

std::string s = "hi";  s += "!";
来源：http://pu.shxzukj.cn

[S33] C++：vector 增删
来源：http://ov.shtwfgs.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://no.9csxet.cn

[S34] C++：遍历 vector
来源：http://vc.huixiangedu.cn

for (auto &x : v) { std::cout << x; }
来源：http://yv.bjjhwx.cn

[S35] C++：map
来源：http://er.shxzukj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bi.asd995.cn

[S36] C++：unordered_map
来源：http://hj.hahajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://th.jianghongdianzi.cn

[S37] C++：set
来源：http://zl.jctech888.com.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vu.shxzskj.cn

[S38] C++：排序
来源：http://mh.lnxyls.cn

std::sort(v.begin(), v.end());
来源：http://qh.gzmigu.cn

[S39] C++：自定义比较器排序
来源：http://ra.yuexingan06.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dr.lnxyls.cn

[S40] C++：查找元素
来源：http://lb.bookmarksfly.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gk.asd995.cn

[S41] C++：类与构造函数
来源：http://do.9csxet.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tu.szxytkj.cn

[S42] C++：继承与虚函数
来源：http://yz.gzmigu.cn

class B : public Base { public: void f() override {} };
来源：http://lw.bookmarksfly.cn

[S43] C++：智能指针
来源：http://fd.colortex.cn

auto p = std::make_unique<int>(5);
来源：http://vn.wgjwhj.cn

[S44] C++：引用传参
来源：http://sv.shtwfgs.cn

void inc(int &x) { ++x; }
来源：http://hd.521024.cn

[S45] C++：lambda
来源：http://le.panjiajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://sv.huanxung.cn

[S46] C++：函数模板
来源：http://ib.hnjuh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qk.huixinmuqiang.cn

[S47] C++：结构化绑定遍历
来源：http://kr.gzmigu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yn.jianghongdianzi.cn

[S48] C++：逐行读文件
来源：http://yo.bjjhwx.cn

std::ifstream in("a.txt");  std::string line;
来源：http://up.jctech888.com.cn

while (std::getline(in, line)) { }
来源：http://rc.wgjwhj.cn

[S49] C++：写文件
来源：http://ak.shxzskj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cb.huixiangedu.cn

[S50] C++：格式化数字
来源：http://ff.huixinmuqiang.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ma.yuexingan06.cn

[S51] C++：显式类型转换
来源：http://xx.muxihuayi.cn

static_cast<double>(a) / b
来源：http://fp.szsharing.cn

[S52] C++：const 与 noexcept
来源：http://re.colortex.cn

int size() const noexcept { return n_; }
来源：http://oo.huixinmuqiang.cn

[S53] C++：移动语义
来源：http://kd.yuexingan06.cn

std::vector<int> w = std::move(v);
来源：http://eh.wgjwhj.cn

[S54] C++：异常处理
来源：http://yh.asd995.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nr.muxihuayi.cn

[S55] C++：结构化绑定
来源：http://yv.haigaiapp.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cq.yuntaijiaju.cn

[S56] C++：optional
来源：http://rh.bookmarksfly.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cy.newstarts.cn

[S57] C++：编译期常量
来源：http://sm.huanxung.cn

constexpr int N = 10;
来源：http://nw.huixinmuqiang.cn

[S58] C++：命名空间
来源：http://el.huixiangedu.cn

namespace ns { int f() { return 1; } }
来源：http://jz.shxzukj.cn

[S59] C++：静态断言
来源：http://uj.wgjwhj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ze.shxzukj.cn

[S60] C++：遍历并删除元素
来源：http://dg.shxzukj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cf.chemitech.net.cn

================================================================================
来源：http://ka.szxytkj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xq.szxytkj.cn

================================================================================
来源：http://hf.wgjwhj.cn

[T01] Kotlin：Hello World
来源：http://eo.newstarts.cn

println("Hello")
来源：http://fd.hahajie.cn

[T02] Kotlin：变量
来源：http://wz.lnxyls.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jp.yuntaijiaju.cn

[T03] Kotlin：字符串模板
来源：http://as.jianghongdianzi.cn

"值: $b"
来源：http://ny.shxzskj.cn

[T04] Kotlin：空安全
来源：http://iy.gzmigu.cn

val n: String? = null;  n?.length
来源：http://lk.521024.cn

[T05] Kotlin：when 表达式
来源：http://ka.jianghongdianzi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jb.muxihuayi.cn

[T06] Kotlin：集合映射
来源：http://zw.shtwfgs.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://jq.chemitech.net.cn

[T07] Kotlin：集合过滤
来源：http://ay.huanxung.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://is.bjjhwx.cn

[T08] Kotlin：数据类
来源：http://lg.haigaiapp.cn

data class User(val name: String, val age: Int)
来源：http://xy.muxihuayi.cn

[T09] Kotlin：扩展函数
来源：http://hb.521024.cn

fun String.exclaim() = this + "!"
来源：http://fu.shxzskj.cn

[T10] Kotlin：默认参数
来源：http://bv.chemitech.net.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pj.huixiangedu.cn

[T11] Kotlin：协程
来源：http://wh.muxihuayi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://mo.colortex.cn

[T12] Kotlin：解构声明
来源：http://jk.muxihuayi.cn

val (a, b) = Pair(1, 2)
来源：http://di.shtwfgs.cn

[T13] Kotlin：只读 Map
来源：http://bc.chemitech.net.cn

val m = mapOf("a" to 1)
来源：http://oo.muxihuayi.cn

[T14] Kotlin：循环
来源：http://oc.shxzukj.cn

for (i in 1..10) println(i)
来源：http://ni.szsharing.cn

[T15] Kotlin：接口
来源：http://el.shxzskj.cn

interface Shape { fun area(): Double }
来源：http://er.huixiangedu.cn

[T16] Swift：Hello World
来源：http://xy.nicolike.cn

print("Hello")
来源：http://it.nszjky.cn

[T17] Swift：变量与常量
来源：http://jb.shtwfgs.cn

var a = 1;  let b = 2
来源：http://nb.haigaiapp.cn

[T18] Swift：字符串插值
来源：http://ef.bookmarksfly.cn

"值: \(b)"
来源：http://bh.jctech888.com.cn

[T19] Swift：可选绑定
来源：http://wr.szsharing.cn

if let n = opt { print(n) }
来源：http://gb.bjjhwx.cn

[T20] Swift：数组操作
来源：http://oj.huixiangedu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://yh.szxytkj.cn

[T21] Swift：遍历
来源：http://yk.hnjuh.cn

for x in a { print(x) }
来源：http://kj.nszjky.cn

[T22] Swift：字典
来源：http://wx.jctech888.com.cn

var d = ["a": 1];  d["b"] = 2
来源：http://nr.lnxyls.cn

[T23] Swift：函数
来源：http://ot.huixinmuqiang.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://en.bookmarksfly.cn

[T24] Swift：闭包
来源：http://og.shtwfgs.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ca.yuntaijiaju.cn

[T25] Swift：结构体
来源：http://wn.521024.cn

struct P { var x: Int }
来源：http://ts.muxihuayi.cn

[T26] Swift：类与重写
来源：http://di.jctech888.com.cn

class A: Base { override func f() {} }
来源：http://wp.bjjhwx.cn

[T27] Swift：错误处理
来源：http://fc.asd995.cn

do { try f() } catch { print(error) }
来源：http://jt.bookmarksfly.cn

[T28] Swift：枚举
来源：http://tu.chemitech.net.cn

enum Color { case red, green }
来源：http://cr.muxihuayi.cn

[T29] Swift：guard 提前返回
来源：http://wi.jctech888.com.cn

guard let x = opt else { return }
来源：http://do.huixinmuqiang.cn

[T30] Swift：协议
来源：http://jw.haigaiapp.cn

protocol Shape { func area() -> Double }
来源：http://we.huixinmuqiang.cn

[T31] Lua：Hello World
来源：http://ne.muxihuayi.cn

print("Hello")
来源：http://ea.shxzskj.cn

[T32] Lua：局部变量
来源：http://pd.nicolike.cn

local a = 1
来源：http://zc.shxzukj.cn

[T33] Lua：表（数组）
来源：http://bx.lnxyls.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://mo.hahajie.cn

[T34] Lua：遍历表
来源：http://md.huixiangedu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gp.hahajie.cn

[T35] Lua：字典表
来源：http://lk.gzmigu.cn

local d = { a = 1 };  d.b = 2
来源：http://oh.9csxet.cn

[T36] Lua：函数
来源：http://za.bjjhwx.cn

function add(a, b) return a + b end
来源：http://ay.szsharing.cn

[T37] Lua：字符串拼接
来源：http://bt.szxytkj.cn

"a" .. "b"
来源：http://il.lnxyls.cn

[T38] Lua：条件
来源：http://mt.lnxyls.cn

if x > 0 then print("正") end
来源：http://ir.521024.cn

[T39] Lua：模式匹配
来源：http://fu.hnjuh.cn

string.find(s, "%d+")
来源：http://zu.colortex.cn

[T40] Lua：元表
来源：http://mg.huixinmuqiang.cn

setmetatable({}, { __index = base })
来源：http://df.bookmarksfly.cn

[T41] Perl：Hello World
来源：http://jx.huixiangedu.cn

print "Hello\n";
来源：http://if.9csxet.cn

[T42] Perl：变量类型
来源：http://tq.huixinmuqiang.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zo.muxihuayi.cn

[T43] Perl：字符串插值
来源：http://sn.panjiajie.cn

"值: $a"
来源：http://hz.huixiangedu.cn

[T44] Perl：条件
来源：http://ll.shtwfgs.cn

if ($a > 0) { print "正"; }
来源：http://md.asd995.cn

[T45] Perl：数组遍历
来源：http://ke.hahajie.cn

for my $x (@arr) { print $x; }
来源：http://ud.huixiangedu.cn

[T46] Perl：哈希操作
来源：http://fp.jctech888.com.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bq.9csxet.cn

[T47] Perl：正则捕获
来源：http://qf.huixinmuqiang.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jd.wgjwhj.cn

[T48] Perl：正则替换
来源：http://mr.wgjwhj.cn

$s =~ s/old/new/g;
来源：http://kt.nszjky.cn

[T49] Perl：函数
来源：http://ej.bjjhwx.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yl.lnxyls.cn

[T50] Perl：逐行读文件
来源：http://fd.szxytkj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xx.szxytkj.cn

while (my $line = <$fh>) { print $line; }
来源：http://jx.huanxung.cn

[T51] Scala：Hello World
来源：http://fz.gzmigu.cn

println("Hello")
来源：http://fr.yuexingan06.cn

[T52] Scala：变量
来源：http://bj.haigaiapp.cn

val a = 1;  var b = 2
来源：http://uk.gzmigu.cn

[T53] Scala：字符串插值
来源：http://lc.nicolike.cn

s"值: $b"
来源：http://ks.yuexingan06.cn

[T54] Scala：集合映射
来源：http://mq.hahajie.cn

List(1, 2, 3).map(_ * 2)
来源：http://az.colortex.cn

[T55] Scala：集合过滤
来源：http://sw.wgjwhj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://cu.jctech888.com.cn

[T56] Scala：样例类
来源：http://df.bookmarksfly.cn

case class User(name: String, age: Int)
来源：http://ee.chemitech.net.cn

[T57] Scala：模式匹配
来源：http://sx.huixinmuqiang.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://sc.szsharing.cn

[T58] Scala：函数定义
来源：http://ek.panjiajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ww.lnxyls.cn

[T59] Scala：循环
来源：http://ua.yuntaijiaju.cn

for (i <- 1 to 10) println(i)
来源：http://fr.hnjuh.cn

[T60] Scala：折叠
来源：http://ke.wgjwhj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vt.hnjuh.cn

================================================================================
来源：http://df.huixiangedu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tg.hnjuh.cn

================================================================================
来源：http://sg.jianghongdianzi.cn

[U01] Py：创建虚拟环境
来源：http://il.huanxung.cn

python -m venv .venv && source .venv/bin/activate
来源：http://no.shtwfgs.cn

[U02] Py：导出 / 安装依赖
来源：http://sb.bookmarksfly.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hi.9csxet.cn

[U03] Py：加载 .env 配置
来源：http://np.huixinmuqiang.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://dh.newstarts.cn

[U04] Py：变量调试打印
来源：http://wx.9csxet.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qg.chemitech.net.cn

[U05] Py：列表去重且保序
来源：http://xf.shxzskj.cn

list(dict.fromkeys(arr))
来源：http://cc.huanxung.cn

[U06] Py：合并两个字典
来源：http://ao.yuexingan06.cn

{**a, **b}
来源：http://qt.nszjky.cn

[U07] Py：反转字典键值
来源：http://pg.nicolike.cn

{v: k for k, v in d.items()}
来源：http://vh.nicolike.cn

[U08] Py：展平二维列表
来源：http://ax.shtwfgs.cn

[y for x in nested for y in x]
来源：http://kw.521024.cn

[U09] Py：字典取最大值的键
来源：http://hk.nicolike.cn

max(d, key=d.get)
来源：http://ft.shtwfgs.cn

[U10] Py：按值排序字典
来源：http://vt.hahajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wq.bjjhwx.cn

[U11] Py：生成器表达式
来源：http://ig.huixinmuqiang.cn

(x * 2 for x in arr)
来源：http://wp.colortex.cn

[U12] Py：取出现最多的 3 个元素
来源：http://yd.gzmigu.cn

Counter(arr).most_common(3)
来源：http://fm.shxzukj.cn

[U13] Py：固定长度队列
来源：http://ci.521024.cn

deque(maxlen=10)
来源：http://fk.wgjwhj.cn

[U14] Py：分组收集到列表
来源：http://nf.newstarts.cn

defaultdict(list)
来源：http://wf.colortex.cn

[U15] Py：高精度计时
来源：http://wi.521024.cn

t = time.perf_counter()
来源：http://nv.huixiangedu.cn

[U16] Py：命令行参数解析
来源：http://qm.521024.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xv.jianghongdianzi.cn

[U17] Py：初始化日志
来源：http://cr.shtwfgs.cn

logging.basicConfig(level=logging.INFO)
来源：http://dh.asd995.cn

[U18] Py：预编译正则
来源：http://cg.bjjhwx.cn

pat = re.compile(r"\d+")
来源：http://sf.huixiangedu.cn

[U19] Py：正则替换带回调
来源：http://xg.wgjwhj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bb.shtwfgs.cn

[U20] Py：缓存函数结果
来源：http://fg.shxzskj.cn

@functools.lru_cache(maxsize=None)
来源：http://wa.9csxet.cn


<!-- 参考信息 -->