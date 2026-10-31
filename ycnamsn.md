代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sy.panjiajie.cn

[S10] C：指针与解引用
来源：http://dy.newstarts.cn

int *p = &a;  *p = 5;
来源：http://gr.jctech888.com.cn

[S11] C：逐行读文件
来源：http://in.bookmarksfly.cn

FILE *f = fopen("a.txt", "r");
来源：http://hm.szsharing.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wa.jianghongdianzi.cn

fclose(f);
来源：http://yx.521024.cn

[S12] C：写文件
来源：http://xa.huanxung.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ej.huixinmuqiang.cn

[S13] C：宏定义
来源：http://an.shtwfgs.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bk.nszjky.cn

[S14] C：枚举
来源：http://mn.jianghongdianzi.cn

enum Color { RED, GREEN, BLUE };
来源：http://yi.chemitech.net.cn

[S15] C：类型转换
来源：http://xa.shxzukj.cn

(double) a / b
来源：http://gn.lnxyls.cn

[S16] C：位操作置位
来源：http://qr.hahajie.cn

x |= (1 << 3);
来源：http://to.wgjwhj.cn

[S17] C：安全拼接字符串
来源：http://ab.jctech888.com.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bb.bookmarksfly.cn

[S18] C：命令行参数
来源：http://tf.chemitech.net.cn

int main(int argc, char **argv)
来源：http://dw.wgjwhj.cn

[S19] C：快速排序
来源：http://fh.jctech888.com.cn

qsort(a, n, sizeof(int), cmp);
来源：http://eq.shtwfgs.cn

[S20] C：二分查找
来源：http://dz.colortex.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ms.gzmigu.cn

[S21] C：字符类别判断
来源：http://tq.bjjhwx.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ny.shxzskj.cn

[S22] C：字符串转数字
来源：http://iv.lnxyls.cn

atoi("42");  strtod("3.14", NULL);
来源：http://yo.colortex.cn

[S23] C：随机数
来源：http://xn.hahajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://po.huixiangedu.cn

[S24] C：获取本地时间
来源：http://we.asd995.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bv.wgjwhj.cn

[S25] C：内存拷贝
来源：http://wd.colortex.cn

memcpy(dst, src, n);
来源：http://nl.shxzskj.cn

[S26] C：内存清零
来源：http://bd.nicolike.cn

memset(a, 0, sizeof a);
来源：http://jm.hnjuh.cn

[S27] C：定义常量
来源：http://dm.lnxyls.cn

const double PI = 3.14159;
来源：http://qi.wgjwhj.cn

[S28] C：静态变量
来源：http://bb.bjjhwx.cn

static int counter = 0;
来源：http://yn.bookmarksfly.cn

[S29] C：变参函数
来源：http://dv.newstarts.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nn.colortex.cn

[S30] C：头文件保护
来源：http://xq.huanxung.cn

#ifndef X_H
来源：http://ot.jctech888.com.cn

#define X_H
来源：http://fp.bookmarksfly.cn

#endif
来源：http://kn.yuexingan06.cn

[S31] C++：Hello World
来源：http://zt.nszjky.cn

#include <iostream>
来源：http://qc.bjjhwx.cn

int main() { std::cout << "Hello\n"; }
来源：http://wx.shxzukj.cn

[S32] C++：字符串
来源：http://ld.lnxyls.cn

std::string s = "hi";  s += "!";
来源：http://ez.shtwfgs.cn

[S33] C++：vector 增删
来源：http://hz.jianghongdianzi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hf.shxzskj.cn

[S34] C++：遍历 vector
来源：http://gk.bjjhwx.cn

for (auto &x : v) { std::cout << x; }
来源：http://ou.jianghongdianzi.cn

[S35] C++：map
来源：http://ev.colortex.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dl.huixinmuqiang.cn

[S36] C++：unordered_map
来源：http://ud.newstarts.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lf.shxzskj.cn

[S37] C++：set
来源：http://hx.muxihuayi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://az.hahajie.cn

[S38] C++：排序
来源：http://cf.lnxyls.cn

std::sort(v.begin(), v.end());
来源：http://gr.jctech888.com.cn

[S39] C++：自定义比较器排序
来源：http://or.huixiangedu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fq.hnjuh.cn

[S40] C++：查找元素
来源：http://am.shxzukj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wl.521024.cn

[S41] C++：类与构造函数
来源：http://kk.lnxyls.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sa.nicolike.cn

[S42] C++：继承与虚函数
来源：http://bh.yuntaijiaju.cn

class B : public Base { public: void f() override {} };
来源：http://bg.jctech888.com.cn

[S43] C++：智能指针
来源：http://wm.szsharing.cn

auto p = std::make_unique<int>(5);
来源：http://nv.yuntaijiaju.cn

[S44] C++：引用传参
来源：http://tw.chemitech.net.cn

void inc(int &x) { ++x; }
来源：http://rq.newstarts.cn

[S45] C++：lambda
来源：http://dy.jianghongdianzi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://tw.huixinmuqiang.cn

[S46] C++：函数模板
来源：http://rm.yuexingan06.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qt.panjiajie.cn

[S47] C++：结构化绑定遍历
来源：http://so.9csxet.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yw.9csxet.cn

[S48] C++：逐行读文件
来源：http://gh.newstarts.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wz.521024.cn

while (std::getline(in, line)) { }
来源：http://kg.wgjwhj.cn

[S49] C++：写文件
来源：http://ml.shxzskj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://at.colortex.cn

[S50] C++：格式化数字
来源：http://fq.bjjhwx.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uy.szxytkj.cn

[S51] C++：显式类型转换
来源：http://nn.hahajie.cn

static_cast<double>(a) / b
来源：http://ja.shxzukj.cn

[S52] C++：const 与 noexcept
来源：http://os.521024.cn

int size() const noexcept { return n_; }
来源：http://lm.521024.cn

[S53] C++：移动语义
来源：http://gi.shxzskj.cn

std::vector<int> w = std::move(v);
来源：http://fh.bjjhwx.cn

[S54] C++：异常处理
来源：http://qx.gzmigu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ml.shtwfgs.cn

[S55] C++：结构化绑定
来源：http://cc.newstarts.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jf.nicolike.cn

[S56] C++：optional
来源：http://cm.haigaiapp.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hn.haigaiapp.cn

[S57] C++：编译期常量
来源：http://vh.bjjhwx.cn

constexpr int N = 10;
来源：http://si.jianghongdianzi.cn

[S58] C++：命名空间
来源：http://hp.bookmarksfly.cn

namespace ns { int f() { return 1; } }
来源：http://xs.hahajie.cn

[S59] C++：静态断言
来源：http://tl.lnxyls.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://we.shtwfgs.cn

[S60] C++：遍历并删除元素
来源：http://wr.shtwfgs.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gj.wgjwhj.cn

================================================================================
来源：http://kw.bookmarksfly.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fc.muxihuayi.cn

================================================================================
来源：http://cu.shxzukj.cn

[T01] Kotlin：Hello World
来源：http://uy.szsharing.cn

println("Hello")
来源：http://sz.lnxyls.cn

[T02] Kotlin：变量
来源：http://rv.szxytkj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ke.shtwfgs.cn

[T03] Kotlin：字符串模板
来源：http://sa.panjiajie.cn

"值: $b"
来源：http://at.hnjuh.cn

[T04] Kotlin：空安全
来源：http://lb.shxzukj.cn

val n: String? = null;  n?.length
来源：http://lr.yuntaijiaju.cn

[T05] Kotlin：when 表达式
来源：http://xg.muxihuayi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yp.yuntaijiaju.cn

[T06] Kotlin：集合映射
来源：http://ph.nszjky.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://oy.hnjuh.cn

[T07] Kotlin：集合过滤
来源：http://om.jianghongdianzi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tx.bjjhwx.cn

[T08] Kotlin：数据类
来源：http://on.521024.cn

data class User(val name: String, val age: Int)
来源：http://nj.yuexingan06.cn

[T09] Kotlin：扩展函数
来源：http://sz.asd995.cn

fun String.exclaim() = this + "!"
来源：http://oy.hahajie.cn

[T10] Kotlin：默认参数
来源：http://tw.hahajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ow.bookmarksfly.cn

[T11] Kotlin：协程
来源：http://ya.shtwfgs.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://pk.jianghongdianzi.cn

[T12] Kotlin：解构声明
来源：http://qw.wgjwhj.cn

val (a, b) = Pair(1, 2)
来源：http://sv.muxihuayi.cn

[T13] Kotlin：只读 Map
来源：http://vz.nicolike.cn

val m = mapOf("a" to 1)
来源：http://oe.huixinmuqiang.cn

[T14] Kotlin：循环
来源：http://sy.shxzukj.cn

for (i in 1..10) println(i)
来源：http://yq.lnxyls.cn

[T15] Kotlin：接口
来源：http://dp.colortex.cn

interface Shape { fun area(): Double }
来源：http://kk.yuexingan06.cn

[T16] Swift：Hello World
来源：http://fb.bookmarksfly.cn

print("Hello")
来源：http://wn.szsharing.cn

[T17] Swift：变量与常量
来源：http://oq.szxytkj.cn

var a = 1;  let b = 2
来源：http://nz.jctech888.com.cn

[T18] Swift：字符串插值
来源：http://ky.shtwfgs.cn

"值: \(b)"
来源：http://cb.lnxyls.cn

[T19] Swift：可选绑定
来源：http://ah.hahajie.cn

if let n = opt { print(n) }
来源：http://xg.szxytkj.cn

[T20] Swift：数组操作
来源：http://jx.huixiangedu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://de.bookmarksfly.cn

[T21] Swift：遍历
来源：http://iw.szsharing.cn

for x in a { print(x) }
来源：http://bs.shxzskj.cn

[T22] Swift：字典
来源：http://cz.huixiangedu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://hb.haigaiapp.cn

[T23] Swift：函数
来源：http://ky.szsharing.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fy.lnxyls.cn

[T24] Swift：闭包
来源：http://cg.panjiajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://kt.shxzukj.cn

[T25] Swift：结构体
来源：http://pe.bjjhwx.cn

struct P { var x: Int }
来源：http://cv.nszjky.cn

[T26] Swift：类与重写
来源：http://yl.bjjhwx.cn

class A: Base { override func f() {} }
来源：http://vl.521024.cn

[T27] Swift：错误处理
来源：http://fi.huixinmuqiang.cn

do { try f() } catch { print(error) }
来源：http://ep.9csxet.cn

[T28] Swift：枚举
来源：http://rt.hahajie.cn

enum Color { case red, green }
来源：http://ve.bookmarksfly.cn

[T29] Swift：guard 提前返回
来源：http://al.chemitech.net.cn

guard let x = opt else { return }
来源：http://lk.hnjuh.cn

[T30] Swift：协议
来源：http://ha.panjiajie.cn

protocol Shape { func area() -> Double }
来源：http://tx.asd995.cn

[T31] Lua：Hello World
来源：http://sz.shtwfgs.cn

print("Hello")
来源：http://cp.gzmigu.cn

[T32] Lua：局部变量
来源：http://yw.gzmigu.cn

local a = 1
来源：http://pc.hnjuh.cn

[T33] Lua：表（数组）
来源：http://ij.hahajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://sk.gzmigu.cn

[T34] Lua：遍历表
来源：http://ht.huanxung.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://or.521024.cn

[T35] Lua：字典表
来源：http://vw.newstarts.cn

local d = { a = 1 };  d.b = 2
来源：http://rw.lnxyls.cn

[T36] Lua：函数
来源：http://pg.hnjuh.cn

function add(a, b) return a + b end
来源：http://ap.bjjhwx.cn

[T37] Lua：字符串拼接
来源：http://rd.9csxet.cn

"a" .. "b"
来源：http://mw.yuexingan06.cn

[T38] Lua：条件
来源：http://nd.bjjhwx.cn

if x > 0 then print("正") end
来源：http://oa.chemitech.net.cn

[T39] Lua：模式匹配
来源：http://mz.newstarts.cn

string.find(s, "%d+")
来源：http://fj.shxzskj.cn

[T40] Lua：元表
来源：http://vm.wgjwhj.cn

setmetatable({}, { __index = base })
来源：http://pk.shxzskj.cn

[T41] Perl：Hello World
来源：http://rg.asd995.cn

print "Hello\n";
来源：http://xj.lnxyls.cn

[T42] Perl：变量类型
来源：http://pt.haigaiapp.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://li.shtwfgs.cn

[T43] Perl：字符串插值
来源：http://jj.jctech888.com.cn

"值: $a"
来源：http://og.colortex.cn

[T44] Perl：条件
来源：http://bf.gzmigu.cn

if ($a > 0) { print "正"; }
来源：http://cc.haigaiapp.cn

[T45] Perl：数组遍历
来源：http://uu.nszjky.cn

for my $x (@arr) { print $x; }
来源：http://ex.hnjuh.cn

[T46] Perl：哈希操作
来源：http://bh.521024.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gz.huanxung.cn

[T47] Perl：正则捕获
来源：http://oi.nicolike.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://se.hahajie.cn

[T48] Perl：正则替换
来源：http://uo.shxzskj.cn

$s =~ s/old/new/g;
来源：http://gs.shtwfgs.cn

[T49] Perl：函数
来源：http://vp.shxzukj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tl.huanxung.cn

[T50] Perl：逐行读文件
来源：http://xh.asd995.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://vq.wgjwhj.cn

while (my $line = <$fh>) { print $line; }
来源：http://xd.colortex.cn

[T51] Scala：Hello World
来源：http://ui.nszjky.cn

println("Hello")
来源：http://ha.huanxung.cn

[T52] Scala：变量
来源：http://jl.yuexingan06.cn

val a = 1;  var b = 2
来源：http://xq.521024.cn

[T53] Scala：字符串插值
来源：http://nn.hnjuh.cn

s"值: $b"
来源：http://uk.hahajie.cn

[T54] Scala：集合映射
来源：http://ht.shtwfgs.cn

List(1, 2, 3).map(_ * 2)
来源：http://wg.huixinmuqiang.cn

[T55] Scala：集合过滤
来源：http://au.bjjhwx.cn

List(1, 2, 3).filter(_ > 1)
来源：http://bw.muxihuayi.cn

[T56] Scala：样例类
来源：http://jn.shtwfgs.cn

case class User(name: String, age: Int)
来源：http://yb.newstarts.cn

[T57] Scala：模式匹配
来源：http://gh.jianghongdianzi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://mm.panjiajie.cn

[T58] Scala：函数定义
来源：http://bf.bjjhwx.cn

def add(a: Int, b: Int): Int = a + b
来源：http://rt.shxzskj.cn

[T59] Scala：循环
来源：http://gh.huanxung.cn

for (i <- 1 to 10) println(i)
来源：http://ul.shxzskj.cn

[T60] Scala：折叠
来源：http://mm.bookmarksfly.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jy.lnxyls.cn

================================================================================
来源：http://my.9csxet.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dp.huixinmuqiang.cn

================================================================================
来源：http://qr.nicolike.cn

[U01] Py：创建虚拟环境
来源：http://hp.shxzskj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://dk.haigaiapp.cn

[U02] Py：导出 / 安装依赖
来源：http://af.colortex.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uj.newstarts.cn

[U03] Py：加载 .env 配置
来源：http://fg.chemitech.net.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ng.shxzukj.cn

[U04] Py：变量调试打印
来源：http://ew.lnxyls.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gp.521024.cn

[U05] Py：列表去重且保序
来源：http://nn.hnjuh.cn

list(dict.fromkeys(arr))
来源：http://oq.bjjhwx.cn

[U06] Py：合并两个字典
来源：http://ec.shtwfgs.cn

{**a, **b}
来源：http://ce.nszjky.cn

[U07] Py：反转字典键值
来源：http://po.newstarts.cn

{v: k for k, v in d.items()}
来源：http://ft.szsharing.cn

[U08] Py：展平二维列表
来源：http://wp.yuntaijiaju.cn

[y for x in nested for y in x]
来源：http://ua.hnjuh.cn

[U09] Py：字典取最大值的键
来源：http://zu.shtwfgs.cn

max(d, key=d.get)
来源：http://sd.shxzskj.cn

[U10] Py：按值排序字典
来源：http://cg.haigaiapp.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wp.yuntaijiaju.cn

[U11] Py：生成器表达式
来源：http://wd.hahajie.cn

(x * 2 for x in arr)
来源：http://ps.bookmarksfly.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xf.yuntaijiaju.cn

Counter(arr).most_common(3)
来源：http://ha.huanxung.cn

[U13] Py：固定长度队列
来源：http://qd.shxzukj.cn

deque(maxlen=10)
来源：http://wm.newstarts.cn

[U14] Py：分组收集到列表
来源：http://cd.nszjky.cn

defaultdict(list)
来源：http://mo.asd995.cn

[U15] Py：高精度计时
来源：http://cm.newstarts.cn

t = time.perf_counter()
来源：http://rh.hahajie.cn

[U16] Py：命令行参数解析
来源：http://ey.jctech888.com.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qn.szxytkj.cn

[U17] Py：初始化日志
来源：http://cl.szxytkj.cn

logging.basicConfig(level=logging.INFO)
来源：http://bm.521024.cn

[U18] Py：预编译正则
来源：http://uh.yuntaijiaju.cn

pat = re.compile(r"\d+")
来源：http://kb.jianghongdianzi.cn

[U19] Py：正则替换带回调
来源：http://nq.huanxung.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ws.wgjwhj.cn

[U20] Py：缓存函数结果
来源：http://ez.yuntaijiaju.cn

@functools.lru_cache(maxsize=None)
来源：http://mr.hnjuh.cn

[U21] Py：自定义上下文管理器
来源：http://zs.asd995.cn

@contextlib.contextmanager
来源：http://bl.shxzukj.cn

[U22] Py：矩阵转置
来源：http://wq.9csxet.cn

list(zip(*m))
来源：http://nz.bookmarksfly.cn

[U23] Py：分块读取大文件
来源：http://gc.nicolike.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tt.jianghongdianzi.cn

[U24] Py：路径操作
来源：http://yl.szsharing.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rc.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://lw.huanxung.cn

csv.DictReader(f)
来源：http://nn.newstarts.cn

[U26] Py：并发下载
来源：http://aw.hnjuh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xg.wgjwhj.cn

[U27] Py：异步 HTTP
来源：http://gi.colortex.cn

aiohttp.ClientSession() 配合 async with
来源：http://vs.haigaiapp.cn

[U28] Py：类型别名
来源：http://jb.shtwfgs.cn

UserId = int
来源：http://rg.szxytkj.cn

[U29] Py：属性校验
来源：http://wh.521024.cn

@property 与 @x.setter 配合
来源：http://hs.shtwfgs.cn

[U30] Py：数据类
来源：http://qr.lnxyls.cn

@dataclass(slots=True)
来源：http://ef.bookmarksfly.cn

[U31] Py：单测
来源：http://jt.haigaiapp.cn

python -m pytest -q
来源：http://xe.nicolike.cn

[U32] Py：代码格式化
来源：http://sc.jianghongdianzi.cn

ruff format . && ruff check --fix .
来源：http://ed.jianghongdianzi.cn


<!-- 参考信息 -->