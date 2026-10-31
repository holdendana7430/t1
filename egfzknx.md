代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://ue.gzmigu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://kq.muxihuayi.cn

fclose(f);
来源：http://ka.wgjwhj.cn

[S12] C：写文件
来源：http://qv.hnjuh.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zs.asd995.cn

[S13] C：宏定义
来源：http://xq.nszjky.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zk.nszjky.cn

[S14] C：枚举
来源：http://vv.huixinmuqiang.cn

enum Color { RED, GREEN, BLUE };
来源：http://jd.gzmigu.cn

[S15] C：类型转换
来源：http://hy.shxzskj.cn

(double) a / b
来源：http://ld.newstarts.cn

[S16] C：位操作置位
来源：http://rn.muxihuayi.cn

x |= (1 << 3);
来源：http://ur.hahajie.cn

[S17] C：安全拼接字符串
来源：http://cj.asd995.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yo.jctech888.com.cn

[S18] C：命令行参数
来源：http://uj.haigaiapp.cn

int main(int argc, char **argv)
来源：http://cr.521024.cn

[S19] C：快速排序
来源：http://eq.yuntaijiaju.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gn.haigaiapp.cn

[S20] C：二分查找
来源：http://su.bjjhwx.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uq.nicolike.cn

[S21] C：字符类别判断
来源：http://dn.bjjhwx.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lx.wgjwhj.cn

[S22] C：字符串转数字
来源：http://gp.wgjwhj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nw.gzmigu.cn

[S23] C：随机数
来源：http://rw.colortex.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ln.chemitech.net.cn

[S24] C：获取本地时间
来源：http://gk.newstarts.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://le.wgjwhj.cn

[S25] C：内存拷贝
来源：http://lk.9csxet.cn

memcpy(dst, src, n);
来源：http://be.shxzskj.cn

[S26] C：内存清零
来源：http://vp.wgjwhj.cn

memset(a, 0, sizeof a);
来源：http://um.yuexingan06.cn

[S27] C：定义常量
来源：http://qh.hahajie.cn

const double PI = 3.14159;
来源：http://ar.shxzskj.cn

[S28] C：静态变量
来源：http://ud.yuexingan06.cn

static int counter = 0;
来源：http://ys.shxzskj.cn

[S29] C：变参函数
来源：http://jp.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rl.asd995.cn

[S30] C：头文件保护
来源：http://gx.colortex.cn

#ifndef X_H
来源：http://xm.hahajie.cn

#define X_H
来源：http://tu.lnxyls.cn

#endif
来源：http://sj.bjjhwx.cn

[S31] C++：Hello World
来源：http://gx.muxihuayi.cn

#include <iostream>
来源：http://oz.yuntaijiaju.cn

int main() { std::cout << "Hello\n"; }
来源：http://jf.hnjuh.cn

[S32] C++：字符串
来源：http://im.jctech888.com.cn

std::string s = "hi";  s += "!";
来源：http://gt.wgjwhj.cn

[S33] C++：vector 增删
来源：http://ae.nszjky.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vx.chemitech.net.cn

[S34] C++：遍历 vector
来源：http://jd.gzmigu.cn

for (auto &x : v) { std::cout << x; }
来源：http://fs.panjiajie.cn

[S35] C++：map
来源：http://yg.shtwfgs.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ng.521024.cn

[S36] C++：unordered_map
来源：http://eg.huanxung.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ws.panjiajie.cn

[S37] C++：set
来源：http://hn.chemitech.net.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sp.lnxyls.cn

[S38] C++：排序
来源：http://xf.nszjky.cn

std::sort(v.begin(), v.end());
来源：http://dx.bjjhwx.cn

[S39] C++：自定义比较器排序
来源：http://ts.panjiajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zk.newstarts.cn

[S40] C++：查找元素
来源：http://qn.muxihuayi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ju.gzmigu.cn

[S41] C++：类与构造函数
来源：http://vw.bjjhwx.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://me.hnjuh.cn

[S42] C++：继承与虚函数
来源：http://dd.bookmarksfly.cn

class B : public Base { public: void f() override {} };
来源：http://as.nicolike.cn

[S43] C++：智能指针
来源：http://xw.huixinmuqiang.cn

auto p = std::make_unique<int>(5);
来源：http://bk.521024.cn

[S44] C++：引用传参
来源：http://vl.muxihuayi.cn

void inc(int &x) { ++x; }
来源：http://ip.newstarts.cn

[S45] C++：lambda
来源：http://wn.9csxet.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zy.yuexingan06.cn

[S46] C++：函数模板
来源：http://nz.huixinmuqiang.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rt.chemitech.net.cn

[S47] C++：结构化绑定遍历
来源：http://mm.hnjuh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rn.szxytkj.cn

[S48] C++：逐行读文件
来源：http://is.muxihuayi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://sl.shxzskj.cn

while (std::getline(in, line)) { }
来源：http://dy.colortex.cn

[S49] C++：写文件
来源：http://ac.wgjwhj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vq.panjiajie.cn

[S50] C++：格式化数字
来源：http://hz.lnxyls.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ir.colortex.cn

[S51] C++：显式类型转换
来源：http://wf.szxytkj.cn

static_cast<double>(a) / b
来源：http://oo.szxytkj.cn

[S52] C++：const 与 noexcept
来源：http://el.huanxung.cn

int size() const noexcept { return n_; }
来源：http://up.newstarts.cn

[S53] C++：移动语义
来源：http://qu.muxihuayi.cn

std::vector<int> w = std::move(v);
来源：http://ys.chemitech.net.cn

[S54] C++：异常处理
来源：http://ob.panjiajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ue.shxzskj.cn

[S55] C++：结构化绑定
来源：http://do.lnxyls.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vs.shxzskj.cn

[S56] C++：optional
来源：http://zs.huixiangedu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vn.hahajie.cn

[S57] C++：编译期常量
来源：http://yh.jctech888.com.cn

constexpr int N = 10;
来源：http://sn.hnjuh.cn

[S58] C++：命名空间
来源：http://xa.hnjuh.cn

namespace ns { int f() { return 1; } }
来源：http://gv.panjiajie.cn

[S59] C++：静态断言
来源：http://ya.gzmigu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dj.muxihuayi.cn

[S60] C++：遍历并删除元素
来源：http://js.gzmigu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kh.bookmarksfly.cn

================================================================================
来源：http://hc.szsharing.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nw.wgjwhj.cn

================================================================================
来源：http://gt.chemitech.net.cn

[T01] Kotlin：Hello World
来源：http://wa.gzmigu.cn

println("Hello")
来源：http://ak.chemitech.net.cn

[T02] Kotlin：变量
来源：http://jy.chemitech.net.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wk.asd995.cn

[T03] Kotlin：字符串模板
来源：http://uh.yuexingan06.cn

"值: $b"
来源：http://ci.yuntaijiaju.cn

[T04] Kotlin：空安全
来源：http://bd.yuexingan06.cn

val n: String? = null;  n?.length
来源：http://kf.chemitech.net.cn

[T05] Kotlin：when 表达式
来源：http://ef.shtwfgs.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bt.haigaiapp.cn

[T06] Kotlin：集合映射
来源：http://rp.panjiajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://wg.szsharing.cn

[T07] Kotlin：集合过滤
来源：http://ly.jctech888.com.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ww.wgjwhj.cn

[T08] Kotlin：数据类
来源：http://es.jianghongdianzi.cn

data class User(val name: String, val age: Int)
来源：http://jk.wgjwhj.cn

[T09] Kotlin：扩展函数
来源：http://ee.jctech888.com.cn

fun String.exclaim() = this + "!"
来源：http://mi.huixinmuqiang.cn

[T10] Kotlin：默认参数
来源：http://uv.huixiangedu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dq.shxzskj.cn

[T11] Kotlin：协程
来源：http://bx.newstarts.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://og.bjjhwx.cn

[T12] Kotlin：解构声明
来源：http://pl.shtwfgs.cn

val (a, b) = Pair(1, 2)
来源：http://qt.szxytkj.cn

[T13] Kotlin：只读 Map
来源：http://yo.muxihuayi.cn

val m = mapOf("a" to 1)
来源：http://bu.9csxet.cn

[T14] Kotlin：循环
来源：http://mw.nicolike.cn

for (i in 1..10) println(i)
来源：http://hq.bookmarksfly.cn

[T15] Kotlin：接口
来源：http://iw.shxzskj.cn

interface Shape { fun area(): Double }
来源：http://ua.szxytkj.cn

[T16] Swift：Hello World
来源：http://uv.shxzskj.cn

print("Hello")
来源：http://ev.shxzukj.cn

[T17] Swift：变量与常量
来源：http://fq.panjiajie.cn

var a = 1;  let b = 2
来源：http://tv.hnjuh.cn

[T18] Swift：字符串插值
来源：http://wr.9csxet.cn

"值: \(b)"
来源：http://my.asd995.cn

[T19] Swift：可选绑定
来源：http://io.szxytkj.cn

if let n = opt { print(n) }
来源：http://vv.shtwfgs.cn

[T20] Swift：数组操作
来源：http://pr.shxzukj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://on.gzmigu.cn

[T21] Swift：遍历
来源：http://zc.huixiangedu.cn

for x in a { print(x) }
来源：http://mx.newstarts.cn

[T22] Swift：字典
来源：http://rp.szxytkj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://im.nszjky.cn

[T23] Swift：函数
来源：http://ru.haigaiapp.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kc.521024.cn

[T24] Swift：闭包
来源：http://vi.szxytkj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://rt.wgjwhj.cn

[T25] Swift：结构体
来源：http://gn.huixiangedu.cn

struct P { var x: Int }
来源：http://rs.521024.cn

[T26] Swift：类与重写
来源：http://uy.huixinmuqiang.cn

class A: Base { override func f() {} }
来源：http://jh.jianghongdianzi.cn

[T27] Swift：错误处理
来源：http://nm.bookmarksfly.cn

do { try f() } catch { print(error) }
来源：http://jp.bookmarksfly.cn

[T28] Swift：枚举
来源：http://pm.panjiajie.cn

enum Color { case red, green }
来源：http://gn.huanxung.cn

[T29] Swift：guard 提前返回
来源：http://ay.asd995.cn

guard let x = opt else { return }
来源：http://hv.shtwfgs.cn

[T30] Swift：协议
来源：http://ul.lnxyls.cn

protocol Shape { func area() -> Double }
来源：http://dx.colortex.cn

[T31] Lua：Hello World
来源：http://jl.wgjwhj.cn

print("Hello")
来源：http://zt.huixiangedu.cn

[T32] Lua：局部变量
来源：http://gl.haigaiapp.cn

local a = 1
来源：http://xv.colortex.cn

[T33] Lua：表（数组）
来源：http://bi.asd995.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://uy.huixiangedu.cn

[T34] Lua：遍历表
来源：http://da.newstarts.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://aj.yuexingan06.cn

[T35] Lua：字典表
来源：http://bo.bjjhwx.cn

local d = { a = 1 };  d.b = 2
来源：http://is.chemitech.net.cn

[T36] Lua：函数
来源：http://gn.chemitech.net.cn

function add(a, b) return a + b end
来源：http://vy.huixiangedu.cn

[T37] Lua：字符串拼接
来源：http://wl.nszjky.cn

"a" .. "b"
来源：http://le.bookmarksfly.cn

[T38] Lua：条件
来源：http://cz.nicolike.cn

if x > 0 then print("正") end
来源：http://fv.bookmarksfly.cn

[T39] Lua：模式匹配
来源：http://cx.muxihuayi.cn

string.find(s, "%d+")
来源：http://ju.wgjwhj.cn

[T40] Lua：元表
来源：http://am.shxzskj.cn

setmetatable({}, { __index = base })
来源：http://hi.shxzukj.cn

[T41] Perl：Hello World
来源：http://ro.yuexingan06.cn

print "Hello\n";
来源：http://ry.yuexingan06.cn

[T42] Perl：变量类型
来源：http://of.jianghongdianzi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vm.huixiangedu.cn

[T43] Perl：字符串插值
来源：http://dy.huanxung.cn

"值: $a"
来源：http://mu.newstarts.cn

[T44] Perl：条件
来源：http://cl.nicolike.cn

if ($a > 0) { print "正"; }
来源：http://wr.shtwfgs.cn

[T45] Perl：数组遍历
来源：http://gt.lnxyls.cn

for my $x (@arr) { print $x; }
来源：http://aw.shtwfgs.cn

[T46] Perl：哈希操作
来源：http://qg.jctech888.com.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ba.szsharing.cn

[T47] Perl：正则捕获
来源：http://an.haigaiapp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ze.jctech888.com.cn

[T48] Perl：正则替换
来源：http://na.shxzukj.cn

$s =~ s/old/new/g;
来源：http://pw.lnxyls.cn

[T49] Perl：函数
来源：http://sk.haigaiapp.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ce.yuexingan06.cn

[T50] Perl：逐行读文件
来源：http://id.bookmarksfly.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://lb.huixinmuqiang.cn

while (my $line = <$fh>) { print $line; }
来源：http://tj.9csxet.cn

[T51] Scala：Hello World
来源：http://ei.huixiangedu.cn

println("Hello")
来源：http://gd.jctech888.com.cn

[T52] Scala：变量
来源：http://yi.jianghongdianzi.cn

val a = 1;  var b = 2
来源：http://pn.nszjky.cn

[T53] Scala：字符串插值
来源：http://ar.jianghongdianzi.cn

s"值: $b"
来源：http://wd.szsharing.cn

[T54] Scala：集合映射
来源：http://ra.huixinmuqiang.cn

List(1, 2, 3).map(_ * 2)
来源：http://bb.chemitech.net.cn

[T55] Scala：集合过滤
来源：http://wr.szxytkj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://hf.yuexingan06.cn

[T56] Scala：样例类
来源：http://jd.shxzukj.cn

case class User(name: String, age: Int)
来源：http://mi.jctech888.com.cn

[T57] Scala：模式匹配
来源：http://kr.yuntaijiaju.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ek.shxzskj.cn

[T58] Scala：函数定义
来源：http://rk.bjjhwx.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ix.jctech888.com.cn

[T59] Scala：循环
来源：http://wr.haigaiapp.cn

for (i <- 1 to 10) println(i)
来源：http://sw.hahajie.cn

[T60] Scala：折叠
来源：http://yy.chemitech.net.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://io.gzmigu.cn

================================================================================
来源：http://eo.shxzskj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fu.hahajie.cn

================================================================================
来源：http://xt.colortex.cn

[U01] Py：创建虚拟环境
来源：http://fg.panjiajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mb.panjiajie.cn

[U02] Py：导出 / 安装依赖
来源：http://ka.chemitech.net.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dt.shxzskj.cn

[U03] Py：加载 .env 配置
来源：http://oi.wgjwhj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://we.huixiangedu.cn

[U04] Py：变量调试打印
来源：http://ce.bjjhwx.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://eq.huixinmuqiang.cn

[U05] Py：列表去重且保序
来源：http://xt.shxzukj.cn

list(dict.fromkeys(arr))
来源：http://bn.huanxung.cn

[U06] Py：合并两个字典
来源：http://mt.newstarts.cn

{**a, **b}
来源：http://yn.szxytkj.cn

[U07] Py：反转字典键值
来源：http://wq.huixinmuqiang.cn

{v: k for k, v in d.items()}
来源：http://gt.muxihuayi.cn

[U08] Py：展平二维列表
来源：http://iu.szsharing.cn

[y for x in nested for y in x]
来源：http://de.muxihuayi.cn

[U09] Py：字典取最大值的键
来源：http://du.huixinmuqiang.cn

max(d, key=d.get)
来源：http://va.shxzskj.cn

[U10] Py：按值排序字典
来源：http://ia.hnjuh.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ql.asd995.cn

[U11] Py：生成器表达式
来源：http://hz.bjjhwx.cn

(x * 2 for x in arr)
来源：http://tc.szsharing.cn

[U12] Py：取出现最多的 3 个元素
来源：http://dl.huixiangedu.cn

Counter(arr).most_common(3)
来源：http://ox.nicolike.cn

[U13] Py：固定长度队列
来源：http://tb.szxytkj.cn

deque(maxlen=10)
来源：http://na.huixiangedu.cn

[U14] Py：分组收集到列表
来源：http://up.newstarts.cn

defaultdict(list)
来源：http://cq.huixinmuqiang.cn

[U15] Py：高精度计时
来源：http://nc.jctech888.com.cn

t = time.perf_counter()
来源：http://ny.521024.cn

[U16] Py：命令行参数解析
来源：http://sw.hahajie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ik.jctech888.com.cn

[U17] Py：初始化日志
来源：http://hw.huanxung.cn

logging.basicConfig(level=logging.INFO)
来源：http://oe.shxzskj.cn

[U18] Py：预编译正则
来源：http://xt.shtwfgs.cn

pat = re.compile(r"\d+")
来源：http://ug.muxihuayi.cn

[U19] Py：正则替换带回调
来源：http://fd.jctech888.com.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zv.shxzskj.cn

[U20] Py：缓存函数结果
来源：http://in.newstarts.cn

@functools.lru_cache(maxsize=None)
来源：http://go.szsharing.cn

[U21] Py：自定义上下文管理器
来源：http://oy.huixinmuqiang.cn

@contextlib.contextmanager
来源：http://uh.huixinmuqiang.cn

[U22] Py：矩阵转置
来源：http://nh.bookmarksfly.cn

list(zip(*m))
来源：http://ty.bookmarksfly.cn

[U23] Py：分块读取大文件
来源：http://cq.lnxyls.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gz.gzmigu.cn

[U24] Py：路径操作
来源：http://vq.muxihuayi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ik.muxihuayi.cn

[U25] Py：CSV 按字典读
来源：http://fp.bookmarksfly.cn

csv.DictReader(f)
来源：http://ak.asd995.cn

[U26] Py：并发下载
来源：http://vk.szsharing.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vx.newstarts.cn

[U27] Py：异步 HTTP
来源：http://gp.panjiajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://pa.haigaiapp.cn

[U28] Py：类型别名
来源：http://ej.newstarts.cn

UserId = int
来源：http://uv.lnxyls.cn

[U29] Py：属性校验
来源：http://lb.chemitech.net.cn

@property 与 @x.setter 配合
来源：http://gi.huixiangedu.cn

[U30] Py：数据类
来源：http://pv.hahajie.cn

@dataclass(slots=True)
来源：http://un.panjiajie.cn

[U31] Py：单测
来源：http://bd.nszjky.cn

python -m pytest -q
来源：http://hn.chemitech.net.cn

[U32] Py：代码格式化
来源：http://tj.huixiangedu.cn

ruff format . && ruff check --fix .
来源：http://ib.jianghongdianzi.cn

[U33] Py：打包发布
来源：http://ws.9csxet.cn

python -m build  （依赖 pyproject.toml）
来源：http://xw.nicolike.cn

[U34] Py：判断编码
来源：http://ee.wgjwhj.cn

chardet.detect(raw)
来源：http://zo.shxzukj.cn


<!-- 参考信息 -->