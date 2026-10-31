代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yg.panjiajie.cn

[R80] 查看脚本执行耗时
来源：http://pz.szsharing.cn

time ./run.sh
来源：http://vt.muxihuayi.cn

================================================================================
来源：http://kc.asd995.cn

S. C / C++ 专题
来源：http://vx.jianghongdianzi.cn

================================================================================
来源：http://rc.hnjuh.cn

[S01] C：Hello World
来源：http://cn.panjiajie.cn

#include <stdio.h>
来源：http://yr.colortex.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://va.wgjwhj.cn

[S02] C：变量与格式化输出
来源：http://rm.hnjuh.cn

int a = 10; printf("%d\n", a);
来源：http://te.hahajie.cn

[S03] C：读入整数
来源：http://ta.jianghongdianzi.cn

int x; scanf("%d", &x);
来源：http://vj.jctech888.com.cn

[S04] C：字符串复制
来源：http://mv.huixinmuqiang.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gp.lnxyls.cn

[S05] C：字符串长度
来源：http://od.nszjky.cn

strlen(s)
来源：http://xi.haigaiapp.cn

[S06] C：字符串比较
来源：http://bk.colortex.cn

strcmp(a, b) == 0
来源：http://kl.panjiajie.cn

[S07] C：数组遍历求和
来源：http://gn.wgjwhj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sm.newstarts.cn

[S08] C：动态内存分配与释放
来源：http://eo.asd995.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rf.szxytkj.cn

[S09] C：结构体定义与初始化
来源：http://xq.shxzskj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://oh.wgjwhj.cn

[S10] C：指针与解引用
来源：http://wj.huixiangedu.cn

int *p = &a;  *p = 5;
来源：http://bd.nszjky.cn

[S11] C：逐行读文件
来源：http://tw.huixiangedu.cn

FILE *f = fopen("a.txt", "r");
来源：http://lh.newstarts.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dh.yuexingan06.cn

fclose(f);
来源：http://vu.panjiajie.cn

[S12] C：写文件
来源：http://vi.panjiajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sv.nicolike.cn

[S13] C：宏定义
来源：http://vb.jctech888.com.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gd.muxihuayi.cn

[S14] C：枚举
来源：http://zu.bookmarksfly.cn

enum Color { RED, GREEN, BLUE };
来源：http://eh.colortex.cn

[S15] C：类型转换
来源：http://kv.bjjhwx.cn

(double) a / b
来源：http://ja.huixinmuqiang.cn

[S16] C：位操作置位
来源：http://uj.panjiajie.cn

x |= (1 << 3);
来源：http://gj.chemitech.net.cn

[S17] C：安全拼接字符串
来源：http://wg.haigaiapp.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gl.hahajie.cn

[S18] C：命令行参数
来源：http://hn.huixinmuqiang.cn

int main(int argc, char **argv)
来源：http://gb.521024.cn

[S19] C：快速排序
来源：http://ma.lnxyls.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xh.gzmigu.cn

[S20] C：二分查找
来源：http://bl.shtwfgs.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ew.nszjky.cn

[S21] C：字符类别判断
来源：http://aj.jianghongdianzi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bd.gzmigu.cn

[S22] C：字符串转数字
来源：http://ki.chemitech.net.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jd.szxytkj.cn

[S23] C：随机数
来源：http://hb.chemitech.net.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pg.colortex.cn

[S24] C：获取本地时间
来源：http://sp.lnxyls.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hl.bjjhwx.cn

[S25] C：内存拷贝
来源：http://wp.szsharing.cn

memcpy(dst, src, n);
来源：http://sg.panjiajie.cn

[S26] C：内存清零
来源：http://bv.bjjhwx.cn

memset(a, 0, sizeof a);
来源：http://qk.jctech888.com.cn

[S27] C：定义常量
来源：http://vm.jianghongdianzi.cn

const double PI = 3.14159;
来源：http://ul.chemitech.net.cn

[S28] C：静态变量
来源：http://sk.colortex.cn

static int counter = 0;
来源：http://bo.colortex.cn

[S29] C：变参函数
来源：http://km.hnjuh.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qr.huixiangedu.cn

[S30] C：头文件保护
来源：http://xi.nicolike.cn

#ifndef X_H
来源：http://do.yuntaijiaju.cn

#define X_H
来源：http://pf.muxihuayi.cn

#endif
来源：http://yc.panjiajie.cn

[S31] C++：Hello World
来源：http://hn.9csxet.cn

#include <iostream>
来源：http://qa.521024.cn

int main() { std::cout << "Hello\n"; }
来源：http://pf.9csxet.cn

[S32] C++：字符串
来源：http://sa.muxihuayi.cn

std::string s = "hi";  s += "!";
来源：http://wa.9csxet.cn

[S33] C++：vector 增删
来源：http://jt.shxzukj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qx.shxzukj.cn

[S34] C++：遍历 vector
来源：http://gw.521024.cn

for (auto &x : v) { std::cout << x; }
来源：http://vs.521024.cn

[S35] C++：map
来源：http://vu.jianghongdianzi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ot.szxytkj.cn

[S36] C++：unordered_map
来源：http://qv.hahajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xc.9csxet.cn

[S37] C++：set
来源：http://zz.wgjwhj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cd.newstarts.cn

[S38] C++：排序
来源：http://vq.nicolike.cn

std::sort(v.begin(), v.end());
来源：http://lt.jctech888.com.cn

[S39] C++：自定义比较器排序
来源：http://gs.shxzskj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fp.shtwfgs.cn

[S40] C++：查找元素
来源：http://xy.muxihuayi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ot.bjjhwx.cn

[S41] C++：类与构造函数
来源：http://zv.huixinmuqiang.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yd.9csxet.cn

[S42] C++：继承与虚函数
来源：http://qx.panjiajie.cn

class B : public Base { public: void f() override {} };
来源：http://sr.chemitech.net.cn

[S43] C++：智能指针
来源：http://jz.szxytkj.cn

auto p = std::make_unique<int>(5);
来源：http://er.bjjhwx.cn

[S44] C++：引用传参
来源：http://sr.nicolike.cn

void inc(int &x) { ++x; }
来源：http://af.szxytkj.cn

[S45] C++：lambda
来源：http://no.wgjwhj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://po.haigaiapp.cn

[S46] C++：函数模板
来源：http://lt.nszjky.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://es.jianghongdianzi.cn

[S47] C++：结构化绑定遍历
来源：http://tn.bookmarksfly.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dj.hnjuh.cn

[S48] C++：逐行读文件
来源：http://yf.hnjuh.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ag.bjjhwx.cn

while (std::getline(in, line)) { }
来源：http://or.huanxung.cn

[S49] C++：写文件
来源：http://xi.muxihuayi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qg.shtwfgs.cn

[S50] C++：格式化数字
来源：http://vp.colortex.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mz.nszjky.cn

[S51] C++：显式类型转换
来源：http://jj.hnjuh.cn

static_cast<double>(a) / b
来源：http://dn.asd995.cn

[S52] C++：const 与 noexcept
来源：http://qp.shtwfgs.cn

int size() const noexcept { return n_; }
来源：http://tm.chemitech.net.cn

[S53] C++：移动语义
来源：http://ig.shxzukj.cn

std::vector<int> w = std::move(v);
来源：http://eu.wgjwhj.cn

[S54] C++：异常处理
来源：http://xr.shxzukj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pj.nicolike.cn

[S55] C++：结构化绑定
来源：http://fv.yuexingan06.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ap.nicolike.cn

[S56] C++：optional
来源：http://sx.gzmigu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://oh.colortex.cn

[S57] C++：编译期常量
来源：http://zy.muxihuayi.cn

constexpr int N = 10;
来源：http://nm.shxzukj.cn

[S58] C++：命名空间
来源：http://ee.muxihuayi.cn

namespace ns { int f() { return 1; } }
来源：http://we.asd995.cn

[S59] C++：静态断言
来源：http://pb.asd995.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://oi.szxytkj.cn

[S60] C++：遍历并删除元素
来源：http://rg.hnjuh.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tf.wgjwhj.cn

================================================================================
来源：http://nq.hahajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cp.hnjuh.cn

================================================================================
来源：http://yp.bjjhwx.cn

[T01] Kotlin：Hello World
来源：http://iz.lnxyls.cn

println("Hello")
来源：http://ee.hnjuh.cn

[T02] Kotlin：变量
来源：http://dz.muxihuayi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ih.bookmarksfly.cn

[T03] Kotlin：字符串模板
来源：http://zg.9csxet.cn

"值: $b"
来源：http://ft.nicolike.cn

[T04] Kotlin：空安全
来源：http://vh.bookmarksfly.cn

val n: String? = null;  n?.length
来源：http://pk.szsharing.cn

[T05] Kotlin：when 表达式
来源：http://cz.huixinmuqiang.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fe.szsharing.cn

[T06] Kotlin：集合映射
来源：http://tc.nszjky.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://do.shxzskj.cn

[T07] Kotlin：集合过滤
来源：http://pa.muxihuayi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ax.bjjhwx.cn

[T08] Kotlin：数据类
来源：http://pw.hnjuh.cn

data class User(val name: String, val age: Int)
来源：http://jw.wgjwhj.cn

[T09] Kotlin：扩展函数
来源：http://od.jctech888.com.cn

fun String.exclaim() = this + "!"
来源：http://qu.shxzukj.cn

[T10] Kotlin：默认参数
来源：http://fo.panjiajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://og.hnjuh.cn

[T11] Kotlin：协程
来源：http://tc.gzmigu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vd.huixinmuqiang.cn

[T12] Kotlin：解构声明
来源：http://yw.haigaiapp.cn

val (a, b) = Pair(1, 2)
来源：http://ku.panjiajie.cn

[T13] Kotlin：只读 Map
来源：http://sm.huixiangedu.cn

val m = mapOf("a" to 1)
来源：http://sr.yuntaijiaju.cn

[T14] Kotlin：循环
来源：http://ct.shtwfgs.cn

for (i in 1..10) println(i)
来源：http://sz.shxzukj.cn

[T15] Kotlin：接口
来源：http://ru.hnjuh.cn

interface Shape { fun area(): Double }
来源：http://hd.bjjhwx.cn

[T16] Swift：Hello World
来源：http://tg.shxzukj.cn

print("Hello")
来源：http://sj.nicolike.cn

[T17] Swift：变量与常量
来源：http://tl.yuexingan06.cn

var a = 1;  let b = 2
来源：http://zf.bjjhwx.cn

[T18] Swift：字符串插值
来源：http://su.szxytkj.cn

"值: \(b)"
来源：http://jv.haigaiapp.cn

[T19] Swift：可选绑定
来源：http://jw.nszjky.cn

if let n = opt { print(n) }
来源：http://pq.muxihuayi.cn

[T20] Swift：数组操作
来源：http://iv.muxihuayi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qq.colortex.cn

[T21] Swift：遍历
来源：http://wt.bjjhwx.cn

for x in a { print(x) }
来源：http://oh.jianghongdianzi.cn

[T22] Swift：字典
来源：http://pa.bookmarksfly.cn

var d = ["a": 1];  d["b"] = 2
来源：http://hu.shtwfgs.cn

[T23] Swift：函数
来源：http://gg.yuntaijiaju.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ia.asd995.cn

[T24] Swift：闭包
来源：http://kh.521024.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://kh.shxzskj.cn

[T25] Swift：结构体
来源：http://gz.bookmarksfly.cn

struct P { var x: Int }
来源：http://zh.bookmarksfly.cn

[T26] Swift：类与重写
来源：http://lh.newstarts.cn

class A: Base { override func f() {} }
来源：http://zt.chemitech.net.cn

[T27] Swift：错误处理
来源：http://ph.panjiajie.cn

do { try f() } catch { print(error) }
来源：http://si.jianghongdianzi.cn

[T28] Swift：枚举
来源：http://ra.yuntaijiaju.cn

enum Color { case red, green }
来源：http://ke.huixinmuqiang.cn

[T29] Swift：guard 提前返回
来源：http://gl.hnjuh.cn

guard let x = opt else { return }
来源：http://cs.nicolike.cn

[T30] Swift：协议
来源：http://mm.bookmarksfly.cn

protocol Shape { func area() -> Double }
来源：http://hz.wgjwhj.cn

[T31] Lua：Hello World
来源：http://pm.jctech888.com.cn

print("Hello")
来源：http://mb.szsharing.cn

[T32] Lua：局部变量
来源：http://ln.nicolike.cn

local a = 1
来源：http://rn.muxihuayi.cn

[T33] Lua：表（数组）
来源：http://fj.shxzukj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ky.yuntaijiaju.cn

[T34] Lua：遍历表
来源：http://cu.nszjky.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://mj.yuntaijiaju.cn

[T35] Lua：字典表
来源：http://lc.bookmarksfly.cn

local d = { a = 1 };  d.b = 2
来源：http://qa.newstarts.cn

[T36] Lua：函数
来源：http://mm.nszjky.cn

function add(a, b) return a + b end
来源：http://oe.szxytkj.cn

[T37] Lua：字符串拼接
来源：http://pj.chemitech.net.cn

"a" .. "b"
来源：http://bz.haigaiapp.cn

[T38] Lua：条件
来源：http://km.chemitech.net.cn

if x > 0 then print("正") end
来源：http://uk.jctech888.com.cn

[T39] Lua：模式匹配
来源：http://lv.nicolike.cn

string.find(s, "%d+")
来源：http://sg.newstarts.cn

[T40] Lua：元表
来源：http://nl.yuexingan06.cn

setmetatable({}, { __index = base })
来源：http://pb.shxzskj.cn

[T41] Perl：Hello World
来源：http://yc.wgjwhj.cn

print "Hello\n";
来源：http://sn.muxihuayi.cn

[T42] Perl：变量类型
来源：http://sc.newstarts.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sh.shtwfgs.cn

[T43] Perl：字符串插值
来源：http://bs.huanxung.cn

"值: $a"
来源：http://hj.colortex.cn

[T44] Perl：条件
来源：http://qr.szsharing.cn

if ($a > 0) { print "正"; }
来源：http://ms.szxytkj.cn

[T45] Perl：数组遍历
来源：http://bf.colortex.cn

for my $x (@arr) { print $x; }
来源：http://ey.huixinmuqiang.cn

[T46] Perl：哈希操作
来源：http://xu.jianghongdianzi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rl.newstarts.cn

[T47] Perl：正则捕获
来源：http://ks.jctech888.com.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ha.huanxung.cn

[T48] Perl：正则替换
来源：http://bf.szxytkj.cn

$s =~ s/old/new/g;
来源：http://xy.jctech888.com.cn

[T49] Perl：函数
来源：http://yx.huixiangedu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zw.jctech888.com.cn

[T50] Perl：逐行读文件
来源：http://ym.muxihuayi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qv.nicolike.cn

while (my $line = <$fh>) { print $line; }
来源：http://ax.newstarts.cn

[T51] Scala：Hello World
来源：http://vw.haigaiapp.cn

println("Hello")
来源：http://vd.521024.cn

[T52] Scala：变量
来源：http://rj.szxytkj.cn

val a = 1;  var b = 2
来源：http://rg.colortex.cn

[T53] Scala：字符串插值
来源：http://ab.hahajie.cn

s"值: $b"
来源：http://nd.haigaiapp.cn

[T54] Scala：集合映射
来源：http://cu.colortex.cn

List(1, 2, 3).map(_ * 2)
来源：http://wo.shxzskj.cn

[T55] Scala：集合过滤
来源：http://yv.shtwfgs.cn

List(1, 2, 3).filter(_ > 1)
来源：http://lu.szxytkj.cn

[T56] Scala：样例类
来源：http://go.shxzskj.cn

case class User(name: String, age: Int)
来源：http://jh.chemitech.net.cn

[T57] Scala：模式匹配
来源：http://wa.nicolike.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://oa.yuexingan06.cn

[T58] Scala：函数定义
来源：http://ep.9csxet.cn

def add(a: Int, b: Int): Int = a + b
来源：http://il.lnxyls.cn

[T59] Scala：循环
来源：http://if.szxytkj.cn

for (i <- 1 to 10) println(i)
来源：http://rd.huixinmuqiang.cn

[T60] Scala：折叠
来源：http://kc.huixinmuqiang.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yj.panjiajie.cn

================================================================================
来源：http://ts.shxzskj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://op.521024.cn

================================================================================
来源：http://og.9csxet.cn

[U01] Py：创建虚拟环境
来源：http://fw.colortex.cn

python -m venv .venv && source .venv/bin/activate
来源：http://yy.nszjky.cn

[U02] Py：导出 / 安装依赖
来源：http://se.shxzskj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://sw.szsharing.cn

[U03] Py：加载 .env 配置
来源：http://ai.yuexingan06.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://pq.hahajie.cn

[U04] Py：变量调试打印
来源：http://gc.shxzukj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sd.gzmigu.cn

[U05] Py：列表去重且保序
来源：http://qt.wgjwhj.cn

list(dict.fromkeys(arr))
来源：http://or.newstarts.cn

[U06] Py：合并两个字典
来源：http://mj.huixinmuqiang.cn

{**a, **b}
来源：http://ox.szsharing.cn

[U07] Py：反转字典键值
来源：http://ih.jianghongdianzi.cn

{v: k for k, v in d.items()}
来源：http://hu.shxzskj.cn

[U08] Py：展平二维列表
来源：http://xq.newstarts.cn

[y for x in nested for y in x]
来源：http://wy.bjjhwx.cn

[U09] Py：字典取最大值的键
来源：http://pq.hnjuh.cn

max(d, key=d.get)
来源：http://lr.gzmigu.cn

[U10] Py：按值排序字典
来源：http://px.muxihuayi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yp.521024.cn

[U11] Py：生成器表达式
来源：http://bx.bookmarksfly.cn

(x * 2 for x in arr)
来源：http://ht.yuexingan06.cn

[U12] Py：取出现最多的 3 个元素
来源：http://oo.wgjwhj.cn

Counter(arr).most_common(3)
来源：http://wz.shxzskj.cn

[U13] Py：固定长度队列
来源：http://xo.shtwfgs.cn

deque(maxlen=10)
来源：http://fx.yuexingan06.cn

[U14] Py：分组收集到列表
来源：http://gl.szsharing.cn

defaultdict(list)
来源：http://el.panjiajie.cn

[U15] Py：高精度计时
来源：http://ts.hnjuh.cn

t = time.perf_counter()
来源：http://pj.colortex.cn

[U16] Py：命令行参数解析
来源：http://qc.szsharing.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mj.shxzskj.cn

[U17] Py：初始化日志
来源：http://oy.yuexingan06.cn

logging.basicConfig(level=logging.INFO)
来源：http://gk.jctech888.com.cn

[U18] Py：预编译正则
来源：http://qc.lnxyls.cn

pat = re.compile(r"\d+")
来源：http://ko.yuntaijiaju.cn

[U19] Py：正则替换带回调
来源：http://mn.jianghongdianzi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ye.newstarts.cn

[U20] Py：缓存函数结果
来源：http://ub.jianghongdianzi.cn

@functools.lru_cache(maxsize=None)
来源：http://zr.panjiajie.cn


<!-- 参考信息 -->