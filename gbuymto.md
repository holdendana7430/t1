代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://sn.chemitech.net.cn

[S15] C：类型转换
来源：http://zs.521024.cn

(double) a / b
来源：http://hk.bjjhwx.cn

[S16] C：位操作置位
来源：http://ms.huixinmuqiang.cn

x |= (1 << 3);
来源：http://bg.colortex.cn

[S17] C：安全拼接字符串
来源：http://kn.szsharing.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ci.shxzskj.cn

[S18] C：命令行参数
来源：http://mr.hnjuh.cn

int main(int argc, char **argv)
来源：http://vu.huixiangedu.cn

[S19] C：快速排序
来源：http://xp.hahajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://hv.yuntaijiaju.cn

[S20] C：二分查找
来源：http://ji.huixinmuqiang.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://va.shtwfgs.cn

[S21] C：字符类别判断
来源：http://vg.jctech888.com.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uj.hnjuh.cn

[S22] C：字符串转数字
来源：http://ui.9csxet.cn

atoi("42");  strtod("3.14", NULL);
来源：http://uo.shxzukj.cn

[S23] C：随机数
来源：http://cl.gzmigu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vh.muxihuayi.cn

[S24] C：获取本地时间
来源：http://zd.szsharing.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://au.szxytkj.cn

[S25] C：内存拷贝
来源：http://zo.shxzukj.cn

memcpy(dst, src, n);
来源：http://kx.huixinmuqiang.cn

[S26] C：内存清零
来源：http://ab.jianghongdianzi.cn

memset(a, 0, sizeof a);
来源：http://vx.jianghongdianzi.cn

[S27] C：定义常量
来源：http://om.shtwfgs.cn

const double PI = 3.14159;
来源：http://gk.hnjuh.cn

[S28] C：静态变量
来源：http://kp.hnjuh.cn

static int counter = 0;
来源：http://qv.nszjky.cn

[S29] C：变参函数
来源：http://do.szsharing.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qg.colortex.cn

[S30] C：头文件保护
来源：http://ep.shtwfgs.cn

#ifndef X_H
来源：http://sz.muxihuayi.cn

#define X_H
来源：http://gf.szsharing.cn

#endif
来源：http://wp.wgjwhj.cn

[S31] C++：Hello World
来源：http://ci.haigaiapp.cn

#include <iostream>
来源：http://tb.gzmigu.cn

int main() { std::cout << "Hello\n"; }
来源：http://ft.bookmarksfly.cn

[S32] C++：字符串
来源：http://ip.wgjwhj.cn

std::string s = "hi";  s += "!";
来源：http://sa.hahajie.cn

[S33] C++：vector 增删
来源：http://ik.wgjwhj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tv.newstarts.cn

[S34] C++：遍历 vector
来源：http://oe.shxzukj.cn

for (auto &x : v) { std::cout << x; }
来源：http://cz.huixiangedu.cn

[S35] C++：map
来源：http://yb.szsharing.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ze.9csxet.cn

[S36] C++：unordered_map
来源：http://jp.nicolike.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nk.lnxyls.cn

[S37] C++：set
来源：http://oj.haigaiapp.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zc.chemitech.net.cn

[S38] C++：排序
来源：http://wv.9csxet.cn

std::sort(v.begin(), v.end());
来源：http://lt.shtwfgs.cn

[S39] C++：自定义比较器排序
来源：http://yh.gzmigu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://di.jctech888.com.cn

[S40] C++：查找元素
来源：http://dg.bjjhwx.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rr.haigaiapp.cn

[S41] C++：类与构造函数
来源：http://vy.bjjhwx.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ju.shxzukj.cn

[S42] C++：继承与虚函数
来源：http://jk.9csxet.cn

class B : public Base { public: void f() override {} };
来源：http://tu.szxytkj.cn

[S43] C++：智能指针
来源：http://xd.huanxung.cn

auto p = std::make_unique<int>(5);
来源：http://ey.nicolike.cn

[S44] C++：引用传参
来源：http://kx.521024.cn

void inc(int &x) { ++x; }
来源：http://fl.hahajie.cn

[S45] C++：lambda
来源：http://ri.shtwfgs.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ea.lnxyls.cn

[S46] C++：函数模板
来源：http://nx.huanxung.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ac.9csxet.cn

[S47] C++：结构化绑定遍历
来源：http://ak.huixiangedu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://po.521024.cn

[S48] C++：逐行读文件
来源：http://kp.9csxet.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wq.szsharing.cn

while (std::getline(in, line)) { }
来源：http://qs.huixinmuqiang.cn

[S49] C++：写文件
来源：http://ua.wgjwhj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qj.jctech888.com.cn

[S50] C++：格式化数字
来源：http://af.jianghongdianzi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jm.haigaiapp.cn

[S51] C++：显式类型转换
来源：http://qd.jianghongdianzi.cn

static_cast<double>(a) / b
来源：http://dv.jctech888.com.cn

[S52] C++：const 与 noexcept
来源：http://cc.yuexingan06.cn

int size() const noexcept { return n_; }
来源：http://la.gzmigu.cn

[S53] C++：移动语义
来源：http://rg.yuntaijiaju.cn

std::vector<int> w = std::move(v);
来源：http://jh.huixinmuqiang.cn

[S54] C++：异常处理
来源：http://bd.bjjhwx.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fm.jianghongdianzi.cn

[S55] C++：结构化绑定
来源：http://ex.gzmigu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://im.lnxyls.cn

[S56] C++：optional
来源：http://mn.yuexingan06.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kj.jianghongdianzi.cn

[S57] C++：编译期常量
来源：http://oh.hnjuh.cn

constexpr int N = 10;
来源：http://cf.colortex.cn

[S58] C++：命名空间
来源：http://ow.bjjhwx.cn

namespace ns { int f() { return 1; } }
来源：http://mo.nicolike.cn

[S59] C++：静态断言
来源：http://ix.shxzskj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rv.shtwfgs.cn

[S60] C++：遍历并删除元素
来源：http://ct.panjiajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tj.panjiajie.cn

================================================================================
来源：http://xk.muxihuayi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kj.panjiajie.cn

================================================================================
来源：http://ff.yuntaijiaju.cn

[T01] Kotlin：Hello World
来源：http://ze.shxzskj.cn

println("Hello")
来源：http://ga.521024.cn

[T02] Kotlin：变量
来源：http://yn.nicolike.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://io.huanxung.cn

[T03] Kotlin：字符串模板
来源：http://kt.asd995.cn

"值: $b"
来源：http://ic.lnxyls.cn

[T04] Kotlin：空安全
来源：http://xj.jianghongdianzi.cn

val n: String? = null;  n?.length
来源：http://ln.jctech888.com.cn

[T05] Kotlin：when 表达式
来源：http://et.yuntaijiaju.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zr.nszjky.cn

[T06] Kotlin：集合映射
来源：http://go.wgjwhj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://wg.hnjuh.cn

[T07] Kotlin：集合过滤
来源：http://cz.hahajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://rc.chemitech.net.cn

[T08] Kotlin：数据类
来源：http://ep.jctech888.com.cn

data class User(val name: String, val age: Int)
来源：http://pb.jctech888.com.cn

[T09] Kotlin：扩展函数
来源：http://vc.jianghongdianzi.cn

fun String.exclaim() = this + "!"
来源：http://gp.gzmigu.cn

[T10] Kotlin：默认参数
来源：http://ju.newstarts.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://uk.huanxung.cn

[T11] Kotlin：协程
来源：http://fu.shxzukj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vc.jctech888.com.cn

[T12] Kotlin：解构声明
来源：http://ty.shxzskj.cn

val (a, b) = Pair(1, 2)
来源：http://of.chemitech.net.cn

[T13] Kotlin：只读 Map
来源：http://uf.szxytkj.cn

val m = mapOf("a" to 1)
来源：http://lt.huanxung.cn

[T14] Kotlin：循环
来源：http://rt.chemitech.net.cn

for (i in 1..10) println(i)
来源：http://zj.yuexingan06.cn

[T15] Kotlin：接口
来源：http://ld.lnxyls.cn

interface Shape { fun area(): Double }
来源：http://zh.chemitech.net.cn

[T16] Swift：Hello World
来源：http://vg.nszjky.cn

print("Hello")
来源：http://yd.jctech888.com.cn

[T17] Swift：变量与常量
来源：http://pj.muxihuayi.cn

var a = 1;  let b = 2
来源：http://gn.muxihuayi.cn

[T18] Swift：字符串插值
来源：http://qq.nszjky.cn

"值: \(b)"
来源：http://qn.hnjuh.cn

[T19] Swift：可选绑定
来源：http://tx.szxytkj.cn

if let n = opt { print(n) }
来源：http://tn.huixinmuqiang.cn

[T20] Swift：数组操作
来源：http://lp.huixiangedu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gx.nszjky.cn

[T21] Swift：遍历
来源：http://ci.asd995.cn

for x in a { print(x) }
来源：http://gs.yuexingan06.cn

[T22] Swift：字典
来源：http://gl.yuexingan06.cn

var d = ["a": 1];  d["b"] = 2
来源：http://rw.521024.cn

[T23] Swift：函数
来源：http://yt.521024.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://of.hahajie.cn

[T24] Swift：闭包
来源：http://id.szsharing.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zz.wgjwhj.cn

[T25] Swift：结构体
来源：http://ac.nszjky.cn

struct P { var x: Int }
来源：http://zv.haigaiapp.cn

[T26] Swift：类与重写
来源：http://jj.haigaiapp.cn

class A: Base { override func f() {} }
来源：http://ue.yuntaijiaju.cn

[T27] Swift：错误处理
来源：http://sc.chemitech.net.cn

do { try f() } catch { print(error) }
来源：http://wq.huixiangedu.cn

[T28] Swift：枚举
来源：http://lt.haigaiapp.cn

enum Color { case red, green }
来源：http://vj.asd995.cn

[T29] Swift：guard 提前返回
来源：http://ja.nszjky.cn

guard let x = opt else { return }
来源：http://vj.colortex.cn

[T30] Swift：协议
来源：http://eh.bjjhwx.cn

protocol Shape { func area() -> Double }
来源：http://it.muxihuayi.cn

[T31] Lua：Hello World
来源：http://va.lnxyls.cn

print("Hello")
来源：http://ua.bookmarksfly.cn

[T32] Lua：局部变量
来源：http://ls.gzmigu.cn

local a = 1
来源：http://og.szxytkj.cn

[T33] Lua：表（数组）
来源：http://st.521024.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://db.yuexingan06.cn

[T34] Lua：遍历表
来源：http://no.jianghongdianzi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ky.huixiangedu.cn

[T35] Lua：字典表
来源：http://tw.newstarts.cn

local d = { a = 1 };  d.b = 2
来源：http://uw.newstarts.cn

[T36] Lua：函数
来源：http://gp.szxytkj.cn

function add(a, b) return a + b end
来源：http://vj.bjjhwx.cn

[T37] Lua：字符串拼接
来源：http://ti.shxzskj.cn

"a" .. "b"
来源：http://bp.bjjhwx.cn

[T38] Lua：条件
来源：http://xe.chemitech.net.cn

if x > 0 then print("正") end
来源：http://ro.yuexingan06.cn

[T39] Lua：模式匹配
来源：http://md.szsharing.cn

string.find(s, "%d+")
来源：http://gb.bookmarksfly.cn

[T40] Lua：元表
来源：http://au.521024.cn

setmetatable({}, { __index = base })
来源：http://bo.bookmarksfly.cn

[T41] Perl：Hello World
来源：http://qv.newstarts.cn

print "Hello\n";
来源：http://wp.chemitech.net.cn

[T42] Perl：变量类型
来源：http://pb.521024.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yz.huanxung.cn

[T43] Perl：字符串插值
来源：http://ve.hahajie.cn

"值: $a"
来源：http://ea.jctech888.com.cn

[T44] Perl：条件
来源：http://qv.lnxyls.cn

if ($a > 0) { print "正"; }
来源：http://gz.huixinmuqiang.cn

[T45] Perl：数组遍历
来源：http://xm.wgjwhj.cn

for my $x (@arr) { print $x; }
来源：http://gc.nszjky.cn

[T46] Perl：哈希操作
来源：http://gp.hnjuh.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zw.jctech888.com.cn

[T47] Perl：正则捕获
来源：http://us.bookmarksfly.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://zn.huixinmuqiang.cn

[T48] Perl：正则替换
来源：http://sm.wgjwhj.cn

$s =~ s/old/new/g;
来源：http://ci.muxihuayi.cn

[T49] Perl：函数
来源：http://tg.chemitech.net.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lk.szxytkj.cn

[T50] Perl：逐行读文件
来源：http://fo.wgjwhj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://hc.chemitech.net.cn

while (my $line = <$fh>) { print $line; }
来源：http://al.shxzukj.cn

[T51] Scala：Hello World
来源：http://aq.nszjky.cn

println("Hello")
来源：http://yo.huanxung.cn

[T52] Scala：变量
来源：http://wx.yuexingan06.cn

val a = 1;  var b = 2
来源：http://ed.9csxet.cn

[T53] Scala：字符串插值
来源：http://co.huixiangedu.cn

s"值: $b"
来源：http://fo.shxzskj.cn

[T54] Scala：集合映射
来源：http://he.yuexingan06.cn

List(1, 2, 3).map(_ * 2)
来源：http://ir.shtwfgs.cn

[T55] Scala：集合过滤
来源：http://qf.szxytkj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://py.huanxung.cn

[T56] Scala：样例类
来源：http://ik.bookmarksfly.cn

case class User(name: String, age: Int)
来源：http://ch.muxihuayi.cn

[T57] Scala：模式匹配
来源：http://em.huixiangedu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vx.asd995.cn

[T58] Scala：函数定义
来源：http://fr.newstarts.cn

def add(a: Int, b: Int): Int = a + b
来源：http://tg.hahajie.cn

[T59] Scala：循环
来源：http://rb.wgjwhj.cn

for (i <- 1 to 10) println(i)
来源：http://rj.nicolike.cn

[T60] Scala：折叠
来源：http://ku.szxytkj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ki.bookmarksfly.cn

================================================================================
来源：http://ps.bjjhwx.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rj.panjiajie.cn

================================================================================
来源：http://dt.shtwfgs.cn

[U01] Py：创建虚拟环境
来源：http://fk.gzmigu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vl.newstarts.cn

[U02] Py：导出 / 安装依赖
来源：http://ss.lnxyls.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uj.newstarts.cn

[U03] Py：加载 .env 配置
来源：http://rw.lnxyls.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://td.bjjhwx.cn

[U04] Py：变量调试打印
来源：http://cq.bookmarksfly.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://in.hahajie.cn

[U05] Py：列表去重且保序
来源：http://dp.shxzukj.cn

list(dict.fromkeys(arr))
来源：http://hn.chemitech.net.cn

[U06] Py：合并两个字典
来源：http://ho.szsharing.cn

{**a, **b}
来源：http://gx.shxzskj.cn

[U07] Py：反转字典键值
来源：http://iw.9csxet.cn

{v: k for k, v in d.items()}
来源：http://km.9csxet.cn

[U08] Py：展平二维列表
来源：http://vs.bookmarksfly.cn

[y for x in nested for y in x]
来源：http://xi.jianghongdianzi.cn

[U09] Py：字典取最大值的键
来源：http://wk.szxytkj.cn

max(d, key=d.get)
来源：http://zj.szxytkj.cn

[U10] Py：按值排序字典
来源：http://rn.huixinmuqiang.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ub.szsharing.cn

[U11] Py：生成器表达式
来源：http://wt.gzmigu.cn

(x * 2 for x in arr)
来源：http://ea.yuntaijiaju.cn

[U12] Py：取出现最多的 3 个元素
来源：http://jb.yuexingan06.cn

Counter(arr).most_common(3)
来源：http://fa.szsharing.cn

[U13] Py：固定长度队列
来源：http://ot.9csxet.cn

deque(maxlen=10)
来源：http://ly.huanxung.cn

[U14] Py：分组收集到列表
来源：http://oe.nszjky.cn

defaultdict(list)
来源：http://vu.9csxet.cn

[U15] Py：高精度计时
来源：http://wo.hahajie.cn

t = time.perf_counter()
来源：http://nu.gzmigu.cn

[U16] Py：命令行参数解析
来源：http://po.hnjuh.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ml.muxihuayi.cn

[U17] Py：初始化日志
来源：http://ee.hnjuh.cn

logging.basicConfig(level=logging.INFO)
来源：http://pw.nszjky.cn

[U18] Py：预编译正则
来源：http://pa.huanxung.cn

pat = re.compile(r"\d+")
来源：http://gb.yuexingan06.cn

[U19] Py：正则替换带回调
来源：http://az.bjjhwx.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ad.lnxyls.cn

[U20] Py：缓存函数结果
来源：http://gt.huixiangedu.cn

@functools.lru_cache(maxsize=None)
来源：http://pv.yuntaijiaju.cn

[U21] Py：自定义上下文管理器
来源：http://gg.hnjuh.cn

@contextlib.contextmanager
来源：http://ye.yuexingan06.cn

[U22] Py：矩阵转置
来源：http://ji.huixinmuqiang.cn

list(zip(*m))
来源：http://ty.huixiangedu.cn

[U23] Py：分块读取大文件
来源：http://rm.huanxung.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ny.bjjhwx.cn

[U24] Py：路径操作
来源：http://zm.chemitech.net.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qh.muxihuayi.cn

[U25] Py：CSV 按字典读
来源：http://ya.yuexingan06.cn

csv.DictReader(f)
来源：http://ia.521024.cn

[U26] Py：并发下载
来源：http://sl.huixinmuqiang.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://uk.chemitech.net.cn

[U27] Py：异步 HTTP
来源：http://hz.asd995.cn

aiohttp.ClientSession() 配合 async with
来源：http://hr.asd995.cn

[U28] Py：类型别名
来源：http://sk.huixinmuqiang.cn

UserId = int
来源：http://bd.huanxung.cn

[U29] Py：属性校验
来源：http://nd.hnjuh.cn

@property 与 @x.setter 配合
来源：http://nb.haigaiapp.cn

[U30] Py：数据类
来源：http://ju.yuexingan06.cn

@dataclass(slots=True)
来源：http://ot.panjiajie.cn

[U31] Py：单测
来源：http://xr.szsharing.cn

python -m pytest -q
来源：http://db.haigaiapp.cn

[U32] Py：代码格式化
来源：http://jg.jctech888.com.cn

ruff format . && ruff check --fix .
来源：http://ro.bjjhwx.cn

[U33] Py：打包发布
来源：http://vf.shxzukj.cn

python -m build  （依赖 pyproject.toml）
来源：http://ni.colortex.cn

[U34] Py：判断编码
来源：http://nv.yuntaijiaju.cn

chardet.detect(raw)
来源：http://fz.shtwfgs.cn

[U35] Py：发送邮件
来源：http://mj.shxzukj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ju.hnjuh.cn

[U36] Py：定时任务
来源：http://js.9csxet.cn

schedule.every(10).minutes.do(job)
来源：http://yr.521024.cn

[U37] Py：读写 Excel
来源：http://ca.shtwfgs.cn

pandas.read_excel / DataFrame.to_excel
来源：http://uz.yuexingan06.cn

[U38] Py：获取脚本所在目录
来源：http://df.asd995.cn

Path(__file__).resolve().parent
来源：http://ej.chemitech.net.cn


<!-- 参考信息 -->