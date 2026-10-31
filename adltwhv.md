代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://qf.shxzskj.cn

[S02] C：变量与格式化输出
来源：http://ti.hahajie.cn

int a = 10; printf("%d\n", a);
来源：http://gt.9csxet.cn

[S03] C：读入整数
来源：http://gw.gzmigu.cn

int x; scanf("%d", &x);
来源：http://fk.huixinmuqiang.cn

[S04] C：字符串复制
来源：http://jh.shxzukj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://vz.szsharing.cn

[S05] C：字符串长度
来源：http://wv.huixiangedu.cn

strlen(s)
来源：http://hl.hahajie.cn

[S06] C：字符串比较
来源：http://fr.nszjky.cn

strcmp(a, b) == 0
来源：http://bs.wgjwhj.cn

[S07] C：数组遍历求和
来源：http://ol.wgjwhj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sh.asd995.cn

[S08] C：动态内存分配与释放
来源：http://wi.muxihuayi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ka.jianghongdianzi.cn

[S09] C：结构体定义与初始化
来源：http://jg.bookmarksfly.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ge.chemitech.net.cn

[S10] C：指针与解引用
来源：http://fc.muxihuayi.cn

int *p = &a;  *p = 5;
来源：http://fa.jctech888.com.cn

[S11] C：逐行读文件
来源：http://zm.szsharing.cn

FILE *f = fopen("a.txt", "r");
来源：http://nj.haigaiapp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ny.shtwfgs.cn

fclose(f);
来源：http://mg.shxzskj.cn

[S12] C：写文件
来源：http://qb.newstarts.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://iu.huixiangedu.cn

[S13] C：宏定义
来源：http://fp.gzmigu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pl.shxzukj.cn

[S14] C：枚举
来源：http://nd.asd995.cn

enum Color { RED, GREEN, BLUE };
来源：http://ix.yuntaijiaju.cn

[S15] C：类型转换
来源：http://ci.asd995.cn

(double) a / b
来源：http://qf.9csxet.cn

[S16] C：位操作置位
来源：http://rv.asd995.cn

x |= (1 << 3);
来源：http://jt.521024.cn

[S17] C：安全拼接字符串
来源：http://wo.szsharing.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://aq.lnxyls.cn

[S18] C：命令行参数
来源：http://pq.panjiajie.cn

int main(int argc, char **argv)
来源：http://ym.521024.cn

[S19] C：快速排序
来源：http://uq.szxytkj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://tv.shxzskj.cn

[S20] C：二分查找
来源：http://tf.bjjhwx.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lx.lnxyls.cn

[S21] C：字符类别判断
来源：http://dl.muxihuayi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ie.yuntaijiaju.cn

[S22] C：字符串转数字
来源：http://fb.haigaiapp.cn

atoi("42");  strtod("3.14", NULL);
来源：http://bl.wgjwhj.cn

[S23] C：随机数
来源：http://ay.huixiangedu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://io.szsharing.cn

[S24] C：获取本地时间
来源：http://ug.hnjuh.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vt.hnjuh.cn

[S25] C：内存拷贝
来源：http://yz.shtwfgs.cn

memcpy(dst, src, n);
来源：http://zu.521024.cn

[S26] C：内存清零
来源：http://ov.bjjhwx.cn

memset(a, 0, sizeof a);
来源：http://ty.hnjuh.cn

[S27] C：定义常量
来源：http://gu.huixinmuqiang.cn

const double PI = 3.14159;
来源：http://yt.nicolike.cn

[S28] C：静态变量
来源：http://ho.shxzukj.cn

static int counter = 0;
来源：http://kx.huixinmuqiang.cn

[S29] C：变参函数
来源：http://zr.lnxyls.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tf.9csxet.cn

[S30] C：头文件保护
来源：http://rd.shxzukj.cn

#ifndef X_H
来源：http://jq.huixiangedu.cn

#define X_H
来源：http://mq.nicolike.cn

#endif
来源：http://fp.szxytkj.cn

[S31] C++：Hello World
来源：http://et.yuexingan06.cn

#include <iostream>
来源：http://fx.521024.cn

int main() { std::cout << "Hello\n"; }
来源：http://dk.yuntaijiaju.cn

[S32] C++：字符串
来源：http://vj.shxzukj.cn

std::string s = "hi";  s += "!";
来源：http://yi.yuexingan06.cn

[S33] C++：vector 增删
来源：http://pf.muxihuayi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://la.yuexingan06.cn

[S34] C++：遍历 vector
来源：http://ua.hnjuh.cn

for (auto &x : v) { std::cout << x; }
来源：http://ov.wgjwhj.cn

[S35] C++：map
来源：http://ij.gzmigu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lp.newstarts.cn

[S36] C++：unordered_map
来源：http://nf.wgjwhj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://je.panjiajie.cn

[S37] C++：set
来源：http://xx.nszjky.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mi.asd995.cn

[S38] C++：排序
来源：http://qz.muxihuayi.cn

std::sort(v.begin(), v.end());
来源：http://lu.asd995.cn

[S39] C++：自定义比较器排序
来源：http://xa.shtwfgs.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ck.hnjuh.cn

[S40] C++：查找元素
来源：http://vw.szsharing.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dj.huixinmuqiang.cn

[S41] C++：类与构造函数
来源：http://oe.9csxet.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hx.huixinmuqiang.cn

[S42] C++：继承与虚函数
来源：http://nm.9csxet.cn

class B : public Base { public: void f() override {} };
来源：http://fi.jctech888.com.cn

[S43] C++：智能指针
来源：http://iq.nicolike.cn

auto p = std::make_unique<int>(5);
来源：http://ic.nicolike.cn

[S44] C++：引用传参
来源：http://it.521024.cn

void inc(int &x) { ++x; }
来源：http://jj.chemitech.net.cn

[S45] C++：lambda
来源：http://mo.gzmigu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://js.lnxyls.cn

[S46] C++：函数模板
来源：http://wx.shxzukj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cf.jctech888.com.cn

[S47] C++：结构化绑定遍历
来源：http://rg.jianghongdianzi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://eg.9csxet.cn

[S48] C++：逐行读文件
来源：http://yz.asd995.cn

std::ifstream in("a.txt");  std::string line;
来源：http://nz.muxihuayi.cn

while (std::getline(in, line)) { }
来源：http://hv.colortex.cn

[S49] C++：写文件
来源：http://we.nszjky.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ox.huanxung.cn

[S50] C++：格式化数字
来源：http://dc.jctech888.com.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gi.szsharing.cn

[S51] C++：显式类型转换
来源：http://qn.yuexingan06.cn

static_cast<double>(a) / b
来源：http://qw.jctech888.com.cn

[S52] C++：const 与 noexcept
来源：http://ae.wgjwhj.cn

int size() const noexcept { return n_; }
来源：http://ow.huixinmuqiang.cn

[S53] C++：移动语义
来源：http://tq.wgjwhj.cn

std::vector<int> w = std::move(v);
来源：http://fi.shxzskj.cn

[S54] C++：异常处理
来源：http://cc.huanxung.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://oz.szsharing.cn

[S55] C++：结构化绑定
来源：http://dt.szsharing.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cn.colortex.cn

[S56] C++：optional
来源：http://qs.szxytkj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yq.jianghongdianzi.cn

[S57] C++：编译期常量
来源：http://lj.yuexingan06.cn

constexpr int N = 10;
来源：http://xu.szxytkj.cn

[S58] C++：命名空间
来源：http://wx.huixiangedu.cn

namespace ns { int f() { return 1; } }
来源：http://gx.bookmarksfly.cn

[S59] C++：静态断言
来源：http://bh.newstarts.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ap.hnjuh.cn

[S60] C++：遍历并删除元素
来源：http://df.jctech888.com.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dr.shxzukj.cn

================================================================================
来源：http://jf.huanxung.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ed.asd995.cn

================================================================================
来源：http://dz.wgjwhj.cn

[T01] Kotlin：Hello World
来源：http://kr.chemitech.net.cn

println("Hello")
来源：http://hc.yuntaijiaju.cn

[T02] Kotlin：变量
来源：http://yx.shxzukj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://co.hahajie.cn

[T03] Kotlin：字符串模板
来源：http://jl.shxzukj.cn

"值: $b"
来源：http://eq.shxzskj.cn

[T04] Kotlin：空安全
来源：http://cl.colortex.cn

val n: String? = null;  n?.length
来源：http://ot.521024.cn

[T05] Kotlin：when 表达式
来源：http://ih.szxytkj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jj.9csxet.cn

[T06] Kotlin：集合映射
来源：http://gn.chemitech.net.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://yw.hahajie.cn

[T07] Kotlin：集合过滤
来源：http://pz.bjjhwx.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://uf.nicolike.cn

[T08] Kotlin：数据类
来源：http://ny.nszjky.cn

data class User(val name: String, val age: Int)
来源：http://xn.shtwfgs.cn

[T09] Kotlin：扩展函数
来源：http://ls.shtwfgs.cn

fun String.exclaim() = this + "!"
来源：http://ed.huanxung.cn

[T10] Kotlin：默认参数
来源：http://fq.chemitech.net.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://it.szsharing.cn

[T11] Kotlin：协程
来源：http://si.shxzukj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ab.shxzskj.cn

[T12] Kotlin：解构声明
来源：http://me.9csxet.cn

val (a, b) = Pair(1, 2)
来源：http://bm.huixinmuqiang.cn

[T13] Kotlin：只读 Map
来源：http://ql.9csxet.cn

val m = mapOf("a" to 1)
来源：http://il.huanxung.cn

[T14] Kotlin：循环
来源：http://cj.shxzskj.cn

for (i in 1..10) println(i)
来源：http://dc.newstarts.cn

[T15] Kotlin：接口
来源：http://qz.szsharing.cn

interface Shape { fun area(): Double }
来源：http://aa.nicolike.cn

[T16] Swift：Hello World
来源：http://xp.huixiangedu.cn

print("Hello")
来源：http://zd.jianghongdianzi.cn

[T17] Swift：变量与常量
来源：http://nk.nszjky.cn

var a = 1;  let b = 2
来源：http://nq.shxzskj.cn

[T18] Swift：字符串插值
来源：http://eq.bjjhwx.cn

"值: \(b)"
来源：http://ff.wgjwhj.cn

[T19] Swift：可选绑定
来源：http://ng.shtwfgs.cn

if let n = opt { print(n) }
来源：http://ug.jianghongdianzi.cn

[T20] Swift：数组操作
来源：http://vv.chemitech.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zx.jctech888.com.cn

[T21] Swift：遍历
来源：http://rz.nicolike.cn

for x in a { print(x) }
来源：http://om.lnxyls.cn

[T22] Swift：字典
来源：http://qs.colortex.cn

var d = ["a": 1];  d["b"] = 2
来源：http://rc.muxihuayi.cn

[T23] Swift：函数
来源：http://cj.huixiangedu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gb.shtwfgs.cn

[T24] Swift：闭包
来源：http://gk.shxzskj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ss.bjjhwx.cn

[T25] Swift：结构体
来源：http://cm.9csxet.cn

struct P { var x: Int }
来源：http://ga.huanxung.cn

[T26] Swift：类与重写
来源：http://mg.bjjhwx.cn

class A: Base { override func f() {} }
来源：http://no.huanxung.cn

[T27] Swift：错误处理
来源：http://eq.bookmarksfly.cn

do { try f() } catch { print(error) }
来源：http://kg.szxytkj.cn

[T28] Swift：枚举
来源：http://go.colortex.cn

enum Color { case red, green }
来源：http://om.lnxyls.cn

[T29] Swift：guard 提前返回
来源：http://kw.chemitech.net.cn

guard let x = opt else { return }
来源：http://qz.huixiangedu.cn

[T30] Swift：协议
来源：http://xd.huixinmuqiang.cn

protocol Shape { func area() -> Double }
来源：http://oz.9csxet.cn

[T31] Lua：Hello World
来源：http://sq.huixiangedu.cn

print("Hello")
来源：http://ag.nszjky.cn

[T32] Lua：局部变量
来源：http://aq.huanxung.cn

local a = 1
来源：http://vy.huixinmuqiang.cn

[T33] Lua：表（数组）
来源：http://cz.jctech888.com.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://cp.huixinmuqiang.cn

[T34] Lua：遍历表
来源：http://kx.panjiajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rm.huixinmuqiang.cn

[T35] Lua：字典表
来源：http://uy.shxzukj.cn

local d = { a = 1 };  d.b = 2
来源：http://po.newstarts.cn

[T36] Lua：函数
来源：http://ms.jianghongdianzi.cn

function add(a, b) return a + b end
来源：http://xh.szsharing.cn

[T37] Lua：字符串拼接
来源：http://sg.haigaiapp.cn

"a" .. "b"
来源：http://hq.yuntaijiaju.cn

[T38] Lua：条件
来源：http://il.asd995.cn

if x > 0 then print("正") end
来源：http://yk.jianghongdianzi.cn

[T39] Lua：模式匹配
来源：http://cd.chemitech.net.cn

string.find(s, "%d+")
来源：http://tw.chemitech.net.cn

[T40] Lua：元表
来源：http://vh.yuexingan06.cn

setmetatable({}, { __index = base })
来源：http://cd.huixiangedu.cn

[T41] Perl：Hello World
来源：http://vh.shxzukj.cn

print "Hello\n";
来源：http://zg.asd995.cn

[T42] Perl：变量类型
来源：http://ez.huixinmuqiang.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cc.9csxet.cn

[T43] Perl：字符串插值
来源：http://xq.colortex.cn

"值: $a"
来源：http://kt.gzmigu.cn

[T44] Perl：条件
来源：http://zu.9csxet.cn

if ($a > 0) { print "正"; }
来源：http://pb.lnxyls.cn

[T45] Perl：数组遍历
来源：http://ca.yuntaijiaju.cn

for my $x (@arr) { print $x; }
来源：http://di.bookmarksfly.cn

[T46] Perl：哈希操作
来源：http://qd.panjiajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wn.jianghongdianzi.cn

[T47] Perl：正则捕获
来源：http://hg.colortex.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ug.newstarts.cn

[T48] Perl：正则替换
来源：http://ti.jctech888.com.cn

$s =~ s/old/new/g;
来源：http://hh.521024.cn

[T49] Perl：函数
来源：http://of.gzmigu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tz.panjiajie.cn

[T50] Perl：逐行读文件
来源：http://tk.chemitech.net.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ls.muxihuayi.cn

while (my $line = <$fh>) { print $line; }
来源：http://qq.wgjwhj.cn

[T51] Scala：Hello World
来源：http://ym.hnjuh.cn

println("Hello")
来源：http://gm.hnjuh.cn

[T52] Scala：变量
来源：http://ri.huixiangedu.cn

val a = 1;  var b = 2
来源：http://ek.yuexingan06.cn

[T53] Scala：字符串插值
来源：http://xq.newstarts.cn

s"值: $b"
来源：http://oy.chemitech.net.cn

[T54] Scala：集合映射
来源：http://qo.asd995.cn

List(1, 2, 3).map(_ * 2)
来源：http://iy.lnxyls.cn

[T55] Scala：集合过滤
来源：http://qk.szxytkj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://pt.huixinmuqiang.cn

[T56] Scala：样例类
来源：http://uj.jctech888.com.cn

case class User(name: String, age: Int)
来源：http://ur.yuexingan06.cn

[T57] Scala：模式匹配
来源：http://nw.hahajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://yk.asd995.cn

[T58] Scala：函数定义
来源：http://hl.bjjhwx.cn

def add(a: Int, b: Int): Int = a + b
来源：http://lk.nicolike.cn

[T59] Scala：循环
来源：http://an.szxytkj.cn

for (i <- 1 to 10) println(i)
来源：http://re.huixiangedu.cn

[T60] Scala：折叠
来源：http://np.hahajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://to.lnxyls.cn

================================================================================
来源：http://ld.nszjky.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lr.lnxyls.cn

================================================================================
来源：http://kz.muxihuayi.cn

[U01] Py：创建虚拟环境
来源：http://sa.muxihuayi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nh.asd995.cn

[U02] Py：导出 / 安装依赖
来源：http://vq.haigaiapp.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kt.muxihuayi.cn

[U03] Py：加载 .env 配置
来源：http://gi.lnxyls.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ry.haigaiapp.cn

[U04] Py：变量调试打印
来源：http://ff.bjjhwx.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xa.jianghongdianzi.cn

[U05] Py：列表去重且保序
来源：http://xv.bjjhwx.cn

list(dict.fromkeys(arr))
来源：http://di.colortex.cn

[U06] Py：合并两个字典
来源：http://af.yuexingan06.cn

{**a, **b}
来源：http://oo.shxzukj.cn

[U07] Py：反转字典键值
来源：http://be.jianghongdianzi.cn

{v: k for k, v in d.items()}
来源：http://an.muxihuayi.cn

[U08] Py：展平二维列表
来源：http://op.jctech888.com.cn

[y for x in nested for y in x]
来源：http://dq.521024.cn

[U09] Py：字典取最大值的键
来源：http://ul.shxzskj.cn

max(d, key=d.get)
来源：http://ty.bjjhwx.cn

[U10] Py：按值排序字典
来源：http://bi.gzmigu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://er.521024.cn

[U11] Py：生成器表达式
来源：http://ly.shxzskj.cn

(x * 2 for x in arr)
来源：http://xr.shxzskj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://vq.jianghongdianzi.cn

Counter(arr).most_common(3)
来源：http://dp.yuntaijiaju.cn

[U13] Py：固定长度队列
来源：http://yc.yuexingan06.cn

deque(maxlen=10)
来源：http://ju.bjjhwx.cn

[U14] Py：分组收集到列表
来源：http://ky.haigaiapp.cn

defaultdict(list)
来源：http://tp.jctech888.com.cn

[U15] Py：高精度计时
来源：http://zz.asd995.cn

t = time.perf_counter()
来源：http://qp.asd995.cn

[U16] Py：命令行参数解析
来源：http://fn.nszjky.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hd.lnxyls.cn

[U17] Py：初始化日志
来源：http://rx.bookmarksfly.cn

logging.basicConfig(level=logging.INFO)
来源：http://hu.huanxung.cn

[U18] Py：预编译正则
来源：http://xj.huanxung.cn

pat = re.compile(r"\d+")
来源：http://wr.bookmarksfly.cn

[U19] Py：正则替换带回调
来源：http://un.szsharing.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xl.huanxung.cn

[U20] Py：缓存函数结果
来源：http://qp.szsharing.cn

@functools.lru_cache(maxsize=None)
来源：http://hy.newstarts.cn

[U21] Py：自定义上下文管理器
来源：http://ya.muxihuayi.cn

@contextlib.contextmanager
来源：http://ra.shxzskj.cn

[U22] Py：矩阵转置
来源：http://ig.panjiajie.cn

list(zip(*m))
来源：http://yo.haigaiapp.cn

[U23] Py：分块读取大文件
来源：http://ze.hahajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pa.hnjuh.cn

[U24] Py：路径操作
来源：http://dn.shxzukj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mz.wgjwhj.cn


<!-- 参考信息 -->