代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xi.521024.cn

[S10] C：指针与解引用
来源：http://ut.hahajie.cn

int *p = &a;  *p = 5;
来源：http://re.lnxyls.cn

[S11] C：逐行读文件
来源：http://cv.gzmigu.cn

FILE *f = fopen("a.txt", "r");
来源：http://mw.gzmigu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pg.haigaiapp.cn

fclose(f);
来源：http://zu.chemitech.net.cn

[S12] C：写文件
来源：http://no.nszjky.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kn.panjiajie.cn

[S13] C：宏定义
来源：http://gk.9csxet.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cn.lnxyls.cn

[S14] C：枚举
来源：http://ck.nicolike.cn

enum Color { RED, GREEN, BLUE };
来源：http://qf.9csxet.cn

[S15] C：类型转换
来源：http://ak.newstarts.cn

(double) a / b
来源：http://wn.huixiangedu.cn

[S16] C：位操作置位
来源：http://gm.wgjwhj.cn

x |= (1 << 3);
来源：http://uf.huixinmuqiang.cn

[S17] C：安全拼接字符串
来源：http://re.yuexingan06.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://co.colortex.cn

[S18] C：命令行参数
来源：http://qo.chemitech.net.cn

int main(int argc, char **argv)
来源：http://yf.muxihuayi.cn

[S19] C：快速排序
来源：http://at.bjjhwx.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ci.521024.cn

[S20] C：二分查找
来源：http://bj.bjjhwx.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hi.jctech888.com.cn

[S21] C：字符类别判断
来源：http://dh.bookmarksfly.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://he.szxytkj.cn

[S22] C：字符串转数字
来源：http://wj.szsharing.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xt.shxzukj.cn

[S23] C：随机数
来源：http://yv.jctech888.com.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://lx.huanxung.cn

[S24] C：获取本地时间
来源：http://vs.bookmarksfly.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nw.hnjuh.cn

[S25] C：内存拷贝
来源：http://bz.521024.cn

memcpy(dst, src, n);
来源：http://gu.shxzukj.cn

[S26] C：内存清零
来源：http://sm.gzmigu.cn

memset(a, 0, sizeof a);
来源：http://sv.colortex.cn

[S27] C：定义常量
来源：http://bz.jianghongdianzi.cn

const double PI = 3.14159;
来源：http://ni.jianghongdianzi.cn

[S28] C：静态变量
来源：http://um.newstarts.cn

static int counter = 0;
来源：http://wv.lnxyls.cn

[S29] C：变参函数
来源：http://jd.gzmigu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mm.gzmigu.cn

[S30] C：头文件保护
来源：http://kp.yuexingan06.cn

#ifndef X_H
来源：http://my.gzmigu.cn

#define X_H
来源：http://hp.huanxung.cn

#endif
来源：http://no.9csxet.cn

[S31] C++：Hello World
来源：http://eb.muxihuayi.cn

#include <iostream>
来源：http://xn.chemitech.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://hd.jianghongdianzi.cn

[S32] C++：字符串
来源：http://pi.bjjhwx.cn

std::string s = "hi";  s += "!";
来源：http://rx.yuexingan06.cn

[S33] C++：vector 增删
来源：http://qu.szsharing.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ct.newstarts.cn

[S34] C++：遍历 vector
来源：http://jx.jianghongdianzi.cn

for (auto &x : v) { std::cout << x; }
来源：http://jd.huixinmuqiang.cn

[S35] C++：map
来源：http://kv.9csxet.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://oh.shtwfgs.cn

[S36] C++：unordered_map
来源：http://dp.jianghongdianzi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vv.nicolike.cn

[S37] C++：set
来源：http://yz.szxytkj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tg.chemitech.net.cn

[S38] C++：排序
来源：http://pv.521024.cn

std::sort(v.begin(), v.end());
来源：http://xl.yuexingan06.cn

[S39] C++：自定义比较器排序
来源：http://tc.szsharing.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ok.shxzukj.cn

[S40] C++：查找元素
来源：http://zr.gzmigu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pj.panjiajie.cn

[S41] C++：类与构造函数
来源：http://rc.nszjky.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vt.shxzskj.cn

[S42] C++：继承与虚函数
来源：http://si.yuexingan06.cn

class B : public Base { public: void f() override {} };
来源：http://si.shtwfgs.cn

[S43] C++：智能指针
来源：http://dw.colortex.cn

auto p = std::make_unique<int>(5);
来源：http://vn.yuntaijiaju.cn

[S44] C++：引用传参
来源：http://zi.shxzskj.cn

void inc(int &x) { ++x; }
来源：http://dr.shxzskj.cn

[S45] C++：lambda
来源：http://io.gzmigu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://mp.wgjwhj.cn

[S46] C++：函数模板
来源：http://nt.nicolike.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kg.yuexingan06.cn

[S47] C++：结构化绑定遍历
来源：http://md.asd995.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hy.muxihuayi.cn

[S48] C++：逐行读文件
来源：http://mf.bjjhwx.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wx.colortex.cn

while (std::getline(in, line)) { }
来源：http://bc.haigaiapp.cn

[S49] C++：写文件
来源：http://cf.asd995.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kf.huixinmuqiang.cn

[S50] C++：格式化数字
来源：http://ls.szxytkj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mg.lnxyls.cn

[S51] C++：显式类型转换
来源：http://bu.hahajie.cn

static_cast<double>(a) / b
来源：http://qw.bjjhwx.cn

[S52] C++：const 与 noexcept
来源：http://vb.haigaiapp.cn

int size() const noexcept { return n_; }
来源：http://wg.bookmarksfly.cn

[S53] C++：移动语义
来源：http://jv.hnjuh.cn

std::vector<int> w = std::move(v);
来源：http://az.wgjwhj.cn

[S54] C++：异常处理
来源：http://ir.szxytkj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rx.szsharing.cn

[S55] C++：结构化绑定
来源：http://qs.bookmarksfly.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bo.huixinmuqiang.cn

[S56] C++：optional
来源：http://pu.szsharing.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sy.shxzukj.cn

[S57] C++：编译期常量
来源：http://fs.jianghongdianzi.cn

constexpr int N = 10;
来源：http://sx.colortex.cn

[S58] C++：命名空间
来源：http://uz.521024.cn

namespace ns { int f() { return 1; } }
来源：http://sm.nszjky.cn

[S59] C++：静态断言
来源：http://vn.asd995.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kg.asd995.cn

[S60] C++：遍历并删除元素
来源：http://ct.newstarts.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ft.asd995.cn

================================================================================
来源：http://ne.shxzskj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jr.chemitech.net.cn

================================================================================
来源：http://ob.huixinmuqiang.cn

[T01] Kotlin：Hello World
来源：http://mb.yuexingan06.cn

println("Hello")
来源：http://ef.asd995.cn

[T02] Kotlin：变量
来源：http://xw.shxzskj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vl.yuexingan06.cn

[T03] Kotlin：字符串模板
来源：http://nl.nicolike.cn

"值: $b"
来源：http://jn.hahajie.cn

[T04] Kotlin：空安全
来源：http://cl.muxihuayi.cn

val n: String? = null;  n?.length
来源：http://ol.nicolike.cn

[T05] Kotlin：when 表达式
来源：http://ow.hnjuh.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ck.szxytkj.cn

[T06] Kotlin：集合映射
来源：http://za.shxzukj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://yu.hahajie.cn

[T07] Kotlin：集合过滤
来源：http://ts.wgjwhj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vj.szxytkj.cn

[T08] Kotlin：数据类
来源：http://nv.lnxyls.cn

data class User(val name: String, val age: Int)
来源：http://we.jctech888.com.cn

[T09] Kotlin：扩展函数
来源：http://dy.hahajie.cn

fun String.exclaim() = this + "!"
来源：http://uu.521024.cn

[T10] Kotlin：默认参数
来源：http://ww.szxytkj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hp.newstarts.cn

[T11] Kotlin：协程
来源：http://ma.colortex.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ka.asd995.cn

[T12] Kotlin：解构声明
来源：http://yw.haigaiapp.cn

val (a, b) = Pair(1, 2)
来源：http://wj.colortex.cn

[T13] Kotlin：只读 Map
来源：http://dv.jianghongdianzi.cn

val m = mapOf("a" to 1)
来源：http://ep.huixiangedu.cn

[T14] Kotlin：循环
来源：http://dy.bookmarksfly.cn

for (i in 1..10) println(i)
来源：http://go.chemitech.net.cn

[T15] Kotlin：接口
来源：http://cj.newstarts.cn

interface Shape { fun area(): Double }
来源：http://no.jctech888.com.cn

[T16] Swift：Hello World
来源：http://pl.yuntaijiaju.cn

print("Hello")
来源：http://ea.huixiangedu.cn

[T17] Swift：变量与常量
来源：http://ws.haigaiapp.cn

var a = 1;  let b = 2
来源：http://lm.panjiajie.cn

[T18] Swift：字符串插值
来源：http://jm.nicolike.cn

"值: \(b)"
来源：http://pp.gzmigu.cn

[T19] Swift：可选绑定
来源：http://fl.yuexingan06.cn

if let n = opt { print(n) }
来源：http://eq.9csxet.cn

[T20] Swift：数组操作
来源：http://pk.lnxyls.cn

var a = [1, 2, 3];  a.append(4)
来源：http://kx.bjjhwx.cn

[T21] Swift：遍历
来源：http://nt.huanxung.cn

for x in a { print(x) }
来源：http://wc.huixiangedu.cn

[T22] Swift：字典
来源：http://jy.nicolike.cn

var d = ["a": 1];  d["b"] = 2
来源：http://qq.521024.cn

[T23] Swift：函数
来源：http://dt.muxihuayi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://os.9csxet.cn

[T24] Swift：闭包
来源：http://pa.szsharing.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://bc.hahajie.cn

[T25] Swift：结构体
来源：http://ht.muxihuayi.cn

struct P { var x: Int }
来源：http://ao.hnjuh.cn

[T26] Swift：类与重写
来源：http://jx.yuntaijiaju.cn

class A: Base { override func f() {} }
来源：http://pe.yuntaijiaju.cn

[T27] Swift：错误处理
来源：http://jb.shxzukj.cn

do { try f() } catch { print(error) }
来源：http://gk.shtwfgs.cn

[T28] Swift：枚举
来源：http://pe.panjiajie.cn

enum Color { case red, green }
来源：http://wx.colortex.cn

[T29] Swift：guard 提前返回
来源：http://ta.lnxyls.cn

guard let x = opt else { return }
来源：http://oe.jianghongdianzi.cn

[T30] Swift：协议
来源：http://fh.huixiangedu.cn

protocol Shape { func area() -> Double }
来源：http://pq.shxzukj.cn

[T31] Lua：Hello World
来源：http://vx.asd995.cn

print("Hello")
来源：http://ff.huixiangedu.cn

[T32] Lua：局部变量
来源：http://rx.wgjwhj.cn

local a = 1
来源：http://mu.newstarts.cn

[T33] Lua：表（数组）
来源：http://ff.huixiangedu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wx.lnxyls.cn

[T34] Lua：遍历表
来源：http://lc.lnxyls.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://es.9csxet.cn

[T35] Lua：字典表
来源：http://ls.asd995.cn

local d = { a = 1 };  d.b = 2
来源：http://cz.panjiajie.cn

[T36] Lua：函数
来源：http://wy.shxzskj.cn

function add(a, b) return a + b end
来源：http://ft.newstarts.cn

[T37] Lua：字符串拼接
来源：http://hs.chemitech.net.cn

"a" .. "b"
来源：http://xl.muxihuayi.cn

[T38] Lua：条件
来源：http://xy.shxzskj.cn

if x > 0 then print("正") end
来源：http://xw.asd995.cn

[T39] Lua：模式匹配
来源：http://gk.wgjwhj.cn

string.find(s, "%d+")
来源：http://pc.szsharing.cn

[T40] Lua：元表
来源：http://qe.yuntaijiaju.cn

setmetatable({}, { __index = base })
来源：http://ot.bookmarksfly.cn

[T41] Perl：Hello World
来源：http://qt.chemitech.net.cn

print "Hello\n";
来源：http://vu.asd995.cn

[T42] Perl：变量类型
来源：http://fw.gzmigu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sw.yuexingan06.cn

[T43] Perl：字符串插值
来源：http://cl.bjjhwx.cn

"值: $a"
来源：http://ys.hnjuh.cn

[T44] Perl：条件
来源：http://zb.muxihuayi.cn

if ($a > 0) { print "正"; }
来源：http://wc.hnjuh.cn

[T45] Perl：数组遍历
来源：http://qe.jianghongdianzi.cn

for my $x (@arr) { print $x; }
来源：http://gp.yuntaijiaju.cn

[T46] Perl：哈希操作
来源：http://te.panjiajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cy.haigaiapp.cn

[T47] Perl：正则捕获
来源：http://ks.nicolike.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://in.hahajie.cn

[T48] Perl：正则替换
来源：http://bz.nicolike.cn

$s =~ s/old/new/g;
来源：http://ty.hnjuh.cn

[T49] Perl：函数
来源：http://bl.hahajie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ga.haigaiapp.cn

[T50] Perl：逐行读文件
来源：http://kn.shxzukj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://su.asd995.cn

while (my $line = <$fh>) { print $line; }
来源：http://ze.colortex.cn

[T51] Scala：Hello World
来源：http://wx.chemitech.net.cn

println("Hello")
来源：http://eh.lnxyls.cn

[T52] Scala：变量
来源：http://kl.nszjky.cn

val a = 1;  var b = 2
来源：http://dt.chemitech.net.cn

[T53] Scala：字符串插值
来源：http://cq.jctech888.com.cn

s"值: $b"
来源：http://jy.shxzukj.cn

[T54] Scala：集合映射
来源：http://jb.shtwfgs.cn

List(1, 2, 3).map(_ * 2)
来源：http://rn.szsharing.cn

[T55] Scala：集合过滤
来源：http://vg.hahajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ht.szxytkj.cn

[T56] Scala：样例类
来源：http://ty.nicolike.cn

case class User(name: String, age: Int)
来源：http://xv.jianghongdianzi.cn

[T57] Scala：模式匹配
来源：http://ef.huixinmuqiang.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ex.huixiangedu.cn

[T58] Scala：函数定义
来源：http://mi.yuntaijiaju.cn

def add(a: Int, b: Int): Int = a + b
来源：http://rm.huixiangedu.cn

[T59] Scala：循环
来源：http://bk.nszjky.cn

for (i <- 1 to 10) println(i)
来源：http://yq.shxzukj.cn

[T60] Scala：折叠
来源：http://zn.nszjky.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qq.huanxung.cn

================================================================================
来源：http://xb.asd995.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yy.yuntaijiaju.cn

================================================================================
来源：http://bf.jctech888.com.cn

[U01] Py：创建虚拟环境
来源：http://zd.bookmarksfly.cn

python -m venv .venv && source .venv/bin/activate
来源：http://hm.bjjhwx.cn

[U02] Py：导出 / 安装依赖
来源：http://dc.bjjhwx.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ui.jianghongdianzi.cn

[U03] Py：加载 .env 配置
来源：http://bp.hahajie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://dg.yuexingan06.cn

[U04] Py：变量调试打印
来源：http://om.hnjuh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://df.bjjhwx.cn

[U05] Py：列表去重且保序
来源：http://qw.bjjhwx.cn

list(dict.fromkeys(arr))
来源：http://tl.huanxung.cn

[U06] Py：合并两个字典
来源：http://fk.9csxet.cn

{**a, **b}
来源：http://hb.nicolike.cn

[U07] Py：反转字典键值
来源：http://wc.nicolike.cn

{v: k for k, v in d.items()}
来源：http://av.asd995.cn

[U08] Py：展平二维列表
来源：http://wt.chemitech.net.cn

[y for x in nested for y in x]
来源：http://ga.haigaiapp.cn

[U09] Py：字典取最大值的键
来源：http://og.huixinmuqiang.cn

max(d, key=d.get)
来源：http://cf.szsharing.cn

[U10] Py：按值排序字典
来源：http://xg.yuexingan06.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://us.nicolike.cn

[U11] Py：生成器表达式
来源：http://yz.newstarts.cn

(x * 2 for x in arr)
来源：http://xs.colortex.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ym.521024.cn

Counter(arr).most_common(3)
来源：http://or.nszjky.cn

[U13] Py：固定长度队列
来源：http://ek.panjiajie.cn

deque(maxlen=10)
来源：http://vv.szxytkj.cn

[U14] Py：分组收集到列表
来源：http://oz.521024.cn

defaultdict(list)
来源：http://nh.shxzukj.cn

[U15] Py：高精度计时
来源：http://po.shxzskj.cn

t = time.perf_counter()
来源：http://tk.chemitech.net.cn

[U16] Py：命令行参数解析
来源：http://ig.newstarts.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jg.gzmigu.cn

[U17] Py：初始化日志
来源：http://fz.newstarts.cn

logging.basicConfig(level=logging.INFO)
来源：http://gx.huanxung.cn

[U18] Py：预编译正则
来源：http://lf.colortex.cn

pat = re.compile(r"\d+")
来源：http://zr.szsharing.cn

[U19] Py：正则替换带回调
来源：http://yf.wgjwhj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://or.lnxyls.cn

[U20] Py：缓存函数结果
来源：http://ab.lnxyls.cn

@functools.lru_cache(maxsize=None)
来源：http://dg.newstarts.cn

[U21] Py：自定义上下文管理器
来源：http://mg.shxzukj.cn

@contextlib.contextmanager
来源：http://tt.shxzukj.cn

[U22] Py：矩阵转置
来源：http://lw.521024.cn

list(zip(*m))
来源：http://ut.521024.cn

[U23] Py：分块读取大文件
来源：http://mu.huanxung.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ym.huixinmuqiang.cn

[U24] Py：路径操作
来源：http://cr.colortex.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nc.jctech888.com.cn

[U25] Py：CSV 按字典读
来源：http://mi.yuntaijiaju.cn

csv.DictReader(f)
来源：http://xf.muxihuayi.cn

[U26] Py：并发下载
来源：http://uj.chemitech.net.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ld.jctech888.com.cn

[U27] Py：异步 HTTP
来源：http://mt.shxzukj.cn

aiohttp.ClientSession() 配合 async with
来源：http://sr.panjiajie.cn

[U28] Py：类型别名
来源：http://il.wgjwhj.cn

UserId = int
来源：http://yp.jctech888.com.cn

[U29] Py：属性校验
来源：http://kk.yuntaijiaju.cn

@property 与 @x.setter 配合
来源：http://jf.lnxyls.cn

[U30] Py：数据类
来源：http://fi.shxzskj.cn

@dataclass(slots=True)
来源：http://un.lnxyls.cn

[U31] Py：单测
来源：http://bt.bookmarksfly.cn

python -m pytest -q
来源：http://xh.huanxung.cn

[U32] Py：代码格式化
来源：http://kv.asd995.cn

ruff format . && ruff check --fix .
来源：http://nr.gzmigu.cn


<!-- 参考信息 -->