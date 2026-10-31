代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sq.yuexingan06.cn

[S08] C：动态内存分配与释放
来源：http://gq.bjjhwx.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sl.bookmarksfly.cn

[S09] C：结构体定义与初始化
来源：http://vf.jctech888.com.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wz.shxzukj.cn

[S10] C：指针与解引用
来源：http://xt.shtwfgs.cn

int *p = &a;  *p = 5;
来源：http://jq.haigaiapp.cn

[S11] C：逐行读文件
来源：http://yf.521024.cn

FILE *f = fopen("a.txt", "r");
来源：http://bq.9csxet.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fg.huixiangedu.cn

fclose(f);
来源：http://rw.colortex.cn

[S12] C：写文件
来源：http://ip.chemitech.net.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sx.wgjwhj.cn

[S13] C：宏定义
来源：http://ui.huixiangedu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bg.jianghongdianzi.cn

[S14] C：枚举
来源：http://ry.nszjky.cn

enum Color { RED, GREEN, BLUE };
来源：http://oh.wgjwhj.cn

[S15] C：类型转换
来源：http://mw.hnjuh.cn

(double) a / b
来源：http://dh.jianghongdianzi.cn

[S16] C：位操作置位
来源：http://db.nszjky.cn

x |= (1 << 3);
来源：http://fk.bjjhwx.cn

[S17] C：安全拼接字符串
来源：http://zk.nicolike.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://eg.muxihuayi.cn

[S18] C：命令行参数
来源：http://za.newstarts.cn

int main(int argc, char **argv)
来源：http://xi.jianghongdianzi.cn

[S19] C：快速排序
来源：http://zs.huanxung.cn

qsort(a, n, sizeof(int), cmp);
来源：http://bq.bjjhwx.cn

[S20] C：二分查找
来源：http://nt.hnjuh.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fu.asd995.cn

[S21] C：字符类别判断
来源：http://vm.9csxet.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bs.muxihuayi.cn

[S22] C：字符串转数字
来源：http://iy.jctech888.com.cn

atoi("42");  strtod("3.14", NULL);
来源：http://bx.wgjwhj.cn

[S23] C：随机数
来源：http://qa.huixiangedu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://av.nicolike.cn

[S24] C：获取本地时间
来源：http://xi.shxzskj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mn.shxzskj.cn

[S25] C：内存拷贝
来源：http://sl.hahajie.cn

memcpy(dst, src, n);
来源：http://rf.521024.cn

[S26] C：内存清零
来源：http://ae.newstarts.cn

memset(a, 0, sizeof a);
来源：http://tz.shxzukj.cn

[S27] C：定义常量
来源：http://hg.jianghongdianzi.cn

const double PI = 3.14159;
来源：http://ax.shxzukj.cn

[S28] C：静态变量
来源：http://ra.9csxet.cn

static int counter = 0;
来源：http://sh.asd995.cn

[S29] C：变参函数
来源：http://mi.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nd.shxzukj.cn

[S30] C：头文件保护
来源：http://qb.yuntaijiaju.cn

#ifndef X_H
来源：http://lz.huanxung.cn

#define X_H
来源：http://fx.shxzukj.cn

#endif
来源：http://ao.nszjky.cn

[S31] C++：Hello World
来源：http://tz.521024.cn

#include <iostream>
来源：http://pr.colortex.cn

int main() { std::cout << "Hello\n"; }
来源：http://pg.haigaiapp.cn

[S32] C++：字符串
来源：http://xu.huixiangedu.cn

std::string s = "hi";  s += "!";
来源：http://tb.gzmigu.cn

[S33] C++：vector 增删
来源：http://ty.shxzukj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tp.9csxet.cn

[S34] C++：遍历 vector
来源：http://dj.newstarts.cn

for (auto &x : v) { std::cout << x; }
来源：http://re.newstarts.cn

[S35] C++：map
来源：http://jr.bjjhwx.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sx.nszjky.cn

[S36] C++：unordered_map
来源：http://do.bjjhwx.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ym.nicolike.cn

[S37] C++：set
来源：http://da.szsharing.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wt.szsharing.cn

[S38] C++：排序
来源：http://nf.521024.cn

std::sort(v.begin(), v.end());
来源：http://ve.hnjuh.cn

[S39] C++：自定义比较器排序
来源：http://yx.yuntaijiaju.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nk.bjjhwx.cn

[S40] C++：查找元素
来源：http://uy.hahajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hv.shxzukj.cn

[S41] C++：类与构造函数
来源：http://sn.yuexingan06.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jy.szxytkj.cn

[S42] C++：继承与虚函数
来源：http://gt.huanxung.cn

class B : public Base { public: void f() override {} };
来源：http://ln.huanxung.cn

[S43] C++：智能指针
来源：http://jg.hahajie.cn

auto p = std::make_unique<int>(5);
来源：http://ey.panjiajie.cn

[S44] C++：引用传参
来源：http://aq.bookmarksfly.cn

void inc(int &x) { ++x; }
来源：http://aw.panjiajie.cn

[S45] C++：lambda
来源：http://wn.jianghongdianzi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://kr.hnjuh.cn

[S46] C++：函数模板
来源：http://fu.hahajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ej.bjjhwx.cn

[S47] C++：结构化绑定遍历
来源：http://ka.bjjhwx.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ob.bookmarksfly.cn

[S48] C++：逐行读文件
来源：http://pi.muxihuayi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wa.nszjky.cn

while (std::getline(in, line)) { }
来源：http://ha.lnxyls.cn

[S49] C++：写文件
来源：http://wx.nszjky.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tl.shtwfgs.cn

[S50] C++：格式化数字
来源：http://fb.521024.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jg.haigaiapp.cn

[S51] C++：显式类型转换
来源：http://mr.jctech888.com.cn

static_cast<double>(a) / b
来源：http://rv.shxzskj.cn

[S52] C++：const 与 noexcept
来源：http://ly.colortex.cn

int size() const noexcept { return n_; }
来源：http://ij.haigaiapp.cn

[S53] C++：移动语义
来源：http://by.szsharing.cn

std::vector<int> w = std::move(v);
来源：http://za.bookmarksfly.cn

[S54] C++：异常处理
来源：http://bv.hahajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nh.szsharing.cn

[S55] C++：结构化绑定
来源：http://xs.bjjhwx.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xa.chemitech.net.cn

[S56] C++：optional
来源：http://gr.colortex.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gm.hnjuh.cn

[S57] C++：编译期常量
来源：http://js.wgjwhj.cn

constexpr int N = 10;
来源：http://ll.hnjuh.cn

[S58] C++：命名空间
来源：http://fs.wgjwhj.cn

namespace ns { int f() { return 1; } }
来源：http://qk.shxzukj.cn

[S59] C++：静态断言
来源：http://en.hahajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ne.newstarts.cn

[S60] C++：遍历并删除元素
来源：http://qb.szsharing.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hs.521024.cn

================================================================================
来源：http://gp.chemitech.net.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gf.szsharing.cn

================================================================================
来源：http://rq.jianghongdianzi.cn

[T01] Kotlin：Hello World
来源：http://li.muxihuayi.cn

println("Hello")
来源：http://hl.asd995.cn

[T02] Kotlin：变量
来源：http://lm.jctech888.com.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hh.lnxyls.cn

[T03] Kotlin：字符串模板
来源：http://hx.9csxet.cn

"值: $b"
来源：http://kc.nicolike.cn

[T04] Kotlin：空安全
来源：http://an.gzmigu.cn

val n: String? = null;  n?.length
来源：http://xv.hahajie.cn

[T05] Kotlin：when 表达式
来源：http://jo.bjjhwx.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nu.szxytkj.cn

[T06] Kotlin：集合映射
来源：http://cu.jctech888.com.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ka.huanxung.cn

[T07] Kotlin：集合过滤
来源：http://qt.newstarts.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xf.jctech888.com.cn

[T08] Kotlin：数据类
来源：http://ro.shxzskj.cn

data class User(val name: String, val age: Int)
来源：http://dq.newstarts.cn

[T09] Kotlin：扩展函数
来源：http://hs.wgjwhj.cn

fun String.exclaim() = this + "!"
来源：http://ww.hnjuh.cn

[T10] Kotlin：默认参数
来源：http://kw.muxihuayi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rm.shxzukj.cn

[T11] Kotlin：协程
来源：http://cq.asd995.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xu.haigaiapp.cn

[T12] Kotlin：解构声明
来源：http://vq.9csxet.cn

val (a, b) = Pair(1, 2)
来源：http://dy.wgjwhj.cn

[T13] Kotlin：只读 Map
来源：http://qo.jianghongdianzi.cn

val m = mapOf("a" to 1)
来源：http://pv.hahajie.cn

[T14] Kotlin：循环
来源：http://vx.asd995.cn

for (i in 1..10) println(i)
来源：http://ka.nszjky.cn

[T15] Kotlin：接口
来源：http://sy.nicolike.cn

interface Shape { fun area(): Double }
来源：http://cu.szsharing.cn

[T16] Swift：Hello World
来源：http://uf.szsharing.cn

print("Hello")
来源：http://ta.bjjhwx.cn

[T17] Swift：变量与常量
来源：http://hp.hnjuh.cn

var a = 1;  let b = 2
来源：http://bv.9csxet.cn

[T18] Swift：字符串插值
来源：http://nk.hnjuh.cn

"值: \(b)"
来源：http://bs.huixiangedu.cn

[T19] Swift：可选绑定
来源：http://uj.lnxyls.cn

if let n = opt { print(n) }
来源：http://th.jianghongdianzi.cn

[T20] Swift：数组操作
来源：http://su.yuexingan06.cn

var a = [1, 2, 3];  a.append(4)
来源：http://kz.bookmarksfly.cn

[T21] Swift：遍历
来源：http://jp.shxzskj.cn

for x in a { print(x) }
来源：http://um.lnxyls.cn

[T22] Swift：字典
来源：http://wy.shxzukj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://he.521024.cn

[T23] Swift：函数
来源：http://sl.lnxyls.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yw.9csxet.cn

[T24] Swift：闭包
来源：http://gk.hnjuh.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://dx.lnxyls.cn

[T25] Swift：结构体
来源：http://fb.hahajie.cn

struct P { var x: Int }
来源：http://kc.9csxet.cn

[T26] Swift：类与重写
来源：http://wd.wgjwhj.cn

class A: Base { override func f() {} }
来源：http://jy.gzmigu.cn

[T27] Swift：错误处理
来源：http://hc.yuntaijiaju.cn

do { try f() } catch { print(error) }
来源：http://jb.huixiangedu.cn

[T28] Swift：枚举
来源：http://pe.muxihuayi.cn

enum Color { case red, green }
来源：http://wk.9csxet.cn

[T29] Swift：guard 提前返回
来源：http://py.nicolike.cn

guard let x = opt else { return }
来源：http://tt.colortex.cn

[T30] Swift：协议
来源：http://ew.jianghongdianzi.cn

protocol Shape { func area() -> Double }
来源：http://td.shxzukj.cn

[T31] Lua：Hello World
来源：http://fm.9csxet.cn

print("Hello")
来源：http://pn.huanxung.cn

[T32] Lua：局部变量
来源：http://uw.9csxet.cn

local a = 1
来源：http://di.chemitech.net.cn

[T33] Lua：表（数组）
来源：http://hy.hnjuh.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ty.bjjhwx.cn

[T34] Lua：遍历表
来源：http://jp.lnxyls.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://tl.shxzskj.cn

[T35] Lua：字典表
来源：http://jn.chemitech.net.cn

local d = { a = 1 };  d.b = 2
来源：http://we.lnxyls.cn

[T36] Lua：函数
来源：http://oz.nicolike.cn

function add(a, b) return a + b end
来源：http://ab.szxytkj.cn

[T37] Lua：字符串拼接
来源：http://xl.yuexingan06.cn

"a" .. "b"
来源：http://jc.wgjwhj.cn

[T38] Lua：条件
来源：http://oq.shxzskj.cn

if x > 0 then print("正") end
来源：http://vc.chemitech.net.cn

[T39] Lua：模式匹配
来源：http://jl.panjiajie.cn

string.find(s, "%d+")
来源：http://ht.huixinmuqiang.cn

[T40] Lua：元表
来源：http://jv.huixinmuqiang.cn

setmetatable({}, { __index = base })
来源：http://zn.lnxyls.cn

[T41] Perl：Hello World
来源：http://bh.shxzskj.cn

print "Hello\n";
来源：http://bn.521024.cn

[T42] Perl：变量类型
来源：http://wy.bjjhwx.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hf.bookmarksfly.cn

[T43] Perl：字符串插值
来源：http://dx.bookmarksfly.cn

"值: $a"
来源：http://md.nszjky.cn

[T44] Perl：条件
来源：http://yv.asd995.cn

if ($a > 0) { print "正"; }
来源：http://ce.shtwfgs.cn

[T45] Perl：数组遍历
来源：http://fl.shtwfgs.cn

for my $x (@arr) { print $x; }
来源：http://ki.nicolike.cn

[T46] Perl：哈希操作
来源：http://xr.newstarts.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://de.newstarts.cn

[T47] Perl：正则捕获
来源：http://nf.hnjuh.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wq.bookmarksfly.cn

[T48] Perl：正则替换
来源：http://to.colortex.cn

$s =~ s/old/new/g;
来源：http://da.asd995.cn

[T49] Perl：函数
来源：http://du.yuexingan06.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ld.bookmarksfly.cn

[T50] Perl：逐行读文件
来源：http://dq.bjjhwx.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://jo.huanxung.cn

while (my $line = <$fh>) { print $line; }
来源：http://ig.521024.cn

[T51] Scala：Hello World
来源：http://fh.hahajie.cn

println("Hello")
来源：http://px.panjiajie.cn

[T52] Scala：变量
来源：http://vq.shtwfgs.cn

val a = 1;  var b = 2
来源：http://wx.shxzskj.cn

[T53] Scala：字符串插值
来源：http://fd.nicolike.cn

s"值: $b"
来源：http://vm.nicolike.cn

[T54] Scala：集合映射
来源：http://jv.asd995.cn

List(1, 2, 3).map(_ * 2)
来源：http://ha.shtwfgs.cn

[T55] Scala：集合过滤
来源：http://sc.newstarts.cn

List(1, 2, 3).filter(_ > 1)
来源：http://md.jctech888.com.cn

[T56] Scala：样例类
来源：http://af.bjjhwx.cn

case class User(name: String, age: Int)
来源：http://xm.newstarts.cn

[T57] Scala：模式匹配
来源：http://cn.shxzukj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://av.shxzukj.cn

[T58] Scala：函数定义
来源：http://xk.bjjhwx.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gv.shxzskj.cn

[T59] Scala：循环
来源：http://ws.shxzukj.cn

for (i <- 1 to 10) println(i)
来源：http://nd.bookmarksfly.cn

[T60] Scala：折叠
来源：http://no.lnxyls.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yn.wgjwhj.cn

================================================================================
来源：http://ys.gzmigu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rg.bjjhwx.cn

================================================================================
来源：http://lw.521024.cn

[U01] Py：创建虚拟环境
来源：http://ml.jctech888.com.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nw.gzmigu.cn

[U02] Py：导出 / 安装依赖
来源：http://bq.huixiangedu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ks.jctech888.com.cn

[U03] Py：加载 .env 配置
来源：http://ui.nicolike.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ni.huixinmuqiang.cn

[U04] Py：变量调试打印
来源：http://cg.nszjky.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nw.haigaiapp.cn

[U05] Py：列表去重且保序
来源：http://nk.shxzukj.cn

list(dict.fromkeys(arr))
来源：http://wq.bjjhwx.cn

[U06] Py：合并两个字典
来源：http://ku.asd995.cn

{**a, **b}
来源：http://cy.muxihuayi.cn

[U07] Py：反转字典键值
来源：http://bx.szxytkj.cn

{v: k for k, v in d.items()}
来源：http://er.hahajie.cn

[U08] Py：展平二维列表
来源：http://js.bjjhwx.cn

[y for x in nested for y in x]
来源：http://mr.521024.cn

[U09] Py：字典取最大值的键
来源：http://ez.hahajie.cn

max(d, key=d.get)
来源：http://dg.yuexingan06.cn

[U10] Py：按值排序字典
来源：http://ia.nszjky.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jm.asd995.cn

[U11] Py：生成器表达式
来源：http://nj.nicolike.cn

(x * 2 for x in arr)
来源：http://pu.shtwfgs.cn

[U12] Py：取出现最多的 3 个元素
来源：http://fp.jctech888.com.cn

Counter(arr).most_common(3)
来源：http://gh.szsharing.cn

[U13] Py：固定长度队列
来源：http://ca.asd995.cn

deque(maxlen=10)
来源：http://ih.bookmarksfly.cn

[U14] Py：分组收集到列表
来源：http://cr.yuntaijiaju.cn

defaultdict(list)
来源：http://vm.huanxung.cn

[U15] Py：高精度计时
来源：http://zx.chemitech.net.cn

t = time.perf_counter()
来源：http://cx.panjiajie.cn

[U16] Py：命令行参数解析
来源：http://tm.gzmigu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wt.haigaiapp.cn

[U17] Py：初始化日志
来源：http://au.huixinmuqiang.cn

logging.basicConfig(level=logging.INFO)
来源：http://dq.lnxyls.cn

[U18] Py：预编译正则
来源：http://pk.huixinmuqiang.cn

pat = re.compile(r"\d+")
来源：http://xp.shxzskj.cn

[U19] Py：正则替换带回调
来源：http://zs.szxytkj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://if.bjjhwx.cn

[U20] Py：缓存函数结果
来源：http://dp.huixiangedu.cn

@functools.lru_cache(maxsize=None)
来源：http://hu.yuexingan06.cn

[U21] Py：自定义上下文管理器
来源：http://fj.newstarts.cn

@contextlib.contextmanager
来源：http://nz.haigaiapp.cn

[U22] Py：矩阵转置
来源：http://ob.yuexingan06.cn

list(zip(*m))
来源：http://tn.yuntaijiaju.cn

[U23] Py：分块读取大文件
来源：http://un.nszjky.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tn.shxzukj.cn

[U24] Py：路径操作
来源：http://kq.bookmarksfly.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wm.szsharing.cn

[U25] Py：CSV 按字典读
来源：http://eo.wgjwhj.cn

csv.DictReader(f)
来源：http://ah.haigaiapp.cn

[U26] Py：并发下载
来源：http://sl.asd995.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xl.gzmigu.cn

[U27] Py：异步 HTTP
来源：http://bk.huixiangedu.cn

aiohttp.ClientSession() 配合 async with
来源：http://fl.panjiajie.cn

[U28] Py：类型别名
来源：http://pp.gzmigu.cn

UserId = int
来源：http://mk.shxzskj.cn

[U29] Py：属性校验
来源：http://xn.hnjuh.cn

@property 与 @x.setter 配合
来源：http://ta.hnjuh.cn

[U30] Py：数据类
来源：http://nq.shxzukj.cn

@dataclass(slots=True)
来源：http://ft.huixinmuqiang.cn


<!-- 参考信息 -->