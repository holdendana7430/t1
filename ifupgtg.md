代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://pz.chemitech.net.cn

[S15] C：类型转换
来源：http://xx.colortex.cn

(double) a / b
来源：http://kw.huixiangedu.cn

[S16] C：位操作置位
来源：http://wq.chemitech.net.cn

x |= (1 << 3);
来源：http://tj.huanxung.cn

[S17] C：安全拼接字符串
来源：http://rq.wgjwhj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://de.lnxyls.cn

[S18] C：命令行参数
来源：http://yi.nicolike.cn

int main(int argc, char **argv)
来源：http://lw.shtwfgs.cn

[S19] C：快速排序
来源：http://uf.chemitech.net.cn

qsort(a, n, sizeof(int), cmp);
来源：http://bo.haigaiapp.cn

[S20] C：二分查找
来源：http://bn.shtwfgs.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cf.jctech888.com.cn

[S21] C：字符类别判断
来源：http://db.9csxet.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hd.jctech888.com.cn

[S22] C：字符串转数字
来源：http://xe.shxzskj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://zf.shxzskj.cn

[S23] C：随机数
来源：http://vx.shxzukj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zk.asd995.cn

[S24] C：获取本地时间
来源：http://wx.lnxyls.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dv.asd995.cn

[S25] C：内存拷贝
来源：http://fn.shxzskj.cn

memcpy(dst, src, n);
来源：http://nv.chemitech.net.cn

[S26] C：内存清零
来源：http://rw.chemitech.net.cn

memset(a, 0, sizeof a);
来源：http://zs.haigaiapp.cn

[S27] C：定义常量
来源：http://um.gzmigu.cn

const double PI = 3.14159;
来源：http://ln.9csxet.cn

[S28] C：静态变量
来源：http://vl.bookmarksfly.cn

static int counter = 0;
来源：http://qk.chemitech.net.cn

[S29] C：变参函数
来源：http://qs.huixinmuqiang.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://eg.jctech888.com.cn

[S30] C：头文件保护
来源：http://kg.panjiajie.cn

#ifndef X_H
来源：http://zr.colortex.cn

#define X_H
来源：http://pm.yuexingan06.cn

#endif
来源：http://mb.nszjky.cn

[S31] C++：Hello World
来源：http://qo.shxzukj.cn

#include <iostream>
来源：http://mc.nszjky.cn

int main() { std::cout << "Hello\n"; }
来源：http://ue.shxzukj.cn

[S32] C++：字符串
来源：http://cv.nszjky.cn

std::string s = "hi";  s += "!";
来源：http://oz.asd995.cn

[S33] C++：vector 增删
来源：http://bo.huixinmuqiang.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jd.panjiajie.cn

[S34] C++：遍历 vector
来源：http://tx.9csxet.cn

for (auto &x : v) { std::cout << x; }
来源：http://ny.hahajie.cn

[S35] C++：map
来源：http://wc.huixinmuqiang.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tv.asd995.cn

[S36] C++：unordered_map
来源：http://nk.muxihuayi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://oo.nicolike.cn

[S37] C++：set
来源：http://jp.gzmigu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qa.shtwfgs.cn

[S38] C++：排序
来源：http://bt.bookmarksfly.cn

std::sort(v.begin(), v.end());
来源：http://qy.muxihuayi.cn

[S39] C++：自定义比较器排序
来源：http://qp.jctech888.com.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dh.yuexingan06.cn

[S40] C++：查找元素
来源：http://rx.newstarts.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uo.9csxet.cn

[S41] C++：类与构造函数
来源：http://dq.shxzukj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://co.colortex.cn

[S42] C++：继承与虚函数
来源：http://kq.newstarts.cn

class B : public Base { public: void f() override {} };
来源：http://cv.jctech888.com.cn

[S43] C++：智能指针
来源：http://xq.lnxyls.cn

auto p = std::make_unique<int>(5);
来源：http://pe.huixiangedu.cn

[S44] C++：引用传参
来源：http://ju.nicolike.cn

void inc(int &x) { ++x; }
来源：http://bc.gzmigu.cn

[S45] C++：lambda
来源：http://vr.chemitech.net.cn

auto add = [](int a, int b) { return a + b; };
来源：http://la.hahajie.cn

[S46] C++：函数模板
来源：http://pw.haigaiapp.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sh.newstarts.cn

[S47] C++：结构化绑定遍历
来源：http://sh.shtwfgs.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ar.shtwfgs.cn

[S48] C++：逐行读文件
来源：http://gz.huanxung.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ba.shtwfgs.cn

while (std::getline(in, line)) { }
来源：http://js.jctech888.com.cn

[S49] C++：写文件
来源：http://pg.panjiajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ce.colortex.cn

[S50] C++：格式化数字
来源：http://kb.colortex.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cj.gzmigu.cn

[S51] C++：显式类型转换
来源：http://ec.nszjky.cn

static_cast<double>(a) / b
来源：http://yt.9csxet.cn

[S52] C++：const 与 noexcept
来源：http://kv.nszjky.cn

int size() const noexcept { return n_; }
来源：http://qd.huixinmuqiang.cn

[S53] C++：移动语义
来源：http://kj.jianghongdianzi.cn

std::vector<int> w = std::move(v);
来源：http://bt.jianghongdianzi.cn

[S54] C++：异常处理
来源：http://nr.colortex.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vu.huixinmuqiang.cn

[S55] C++：结构化绑定
来源：http://lu.chemitech.net.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://to.521024.cn

[S56] C++：optional
来源：http://pg.jianghongdianzi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://de.9csxet.cn

[S57] C++：编译期常量
来源：http://uf.panjiajie.cn

constexpr int N = 10;
来源：http://og.jianghongdianzi.cn

[S58] C++：命名空间
来源：http://uy.lnxyls.cn

namespace ns { int f() { return 1; } }
来源：http://zk.521024.cn

[S59] C++：静态断言
来源：http://cl.jctech888.com.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qj.yuexingan06.cn

[S60] C++：遍历并删除元素
来源：http://te.colortex.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tr.huixinmuqiang.cn

================================================================================
来源：http://hh.yuntaijiaju.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hm.chemitech.net.cn

================================================================================
来源：http://yu.huanxung.cn

[T01] Kotlin：Hello World
来源：http://he.huixinmuqiang.cn

println("Hello")
来源：http://kj.colortex.cn

[T02] Kotlin：变量
来源：http://ko.lnxyls.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sj.colortex.cn

[T03] Kotlin：字符串模板
来源：http://gb.gzmigu.cn

"值: $b"
来源：http://nc.lnxyls.cn

[T04] Kotlin：空安全
来源：http://wd.yuntaijiaju.cn

val n: String? = null;  n?.length
来源：http://lb.huanxung.cn

[T05] Kotlin：when 表达式
来源：http://ql.shxzskj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ed.nszjky.cn

[T06] Kotlin：集合映射
来源：http://ck.9csxet.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://kw.jctech888.com.cn

[T07] Kotlin：集合过滤
来源：http://gc.szsharing.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lb.yuntaijiaju.cn

[T08] Kotlin：数据类
来源：http://gg.lnxyls.cn

data class User(val name: String, val age: Int)
来源：http://rb.colortex.cn

[T09] Kotlin：扩展函数
来源：http://mi.panjiajie.cn

fun String.exclaim() = this + "!"
来源：http://li.shtwfgs.cn

[T10] Kotlin：默认参数
来源：http://yb.gzmigu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://fx.newstarts.cn

[T11] Kotlin：协程
来源：http://ak.shxzukj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://og.nicolike.cn

[T12] Kotlin：解构声明
来源：http://co.shtwfgs.cn

val (a, b) = Pair(1, 2)
来源：http://nw.shtwfgs.cn

[T13] Kotlin：只读 Map
来源：http://vq.yuntaijiaju.cn

val m = mapOf("a" to 1)
来源：http://rq.lnxyls.cn

[T14] Kotlin：循环
来源：http://xg.bjjhwx.cn

for (i in 1..10) println(i)
来源：http://qb.szxytkj.cn

[T15] Kotlin：接口
来源：http://wo.jctech888.com.cn

interface Shape { fun area(): Double }
来源：http://rt.wgjwhj.cn

[T16] Swift：Hello World
来源：http://fe.asd995.cn

print("Hello")
来源：http://qv.szsharing.cn

[T17] Swift：变量与常量
来源：http://tm.newstarts.cn

var a = 1;  let b = 2
来源：http://il.shxzskj.cn

[T18] Swift：字符串插值
来源：http://qu.newstarts.cn

"值: \(b)"
来源：http://jm.huixiangedu.cn

[T19] Swift：可选绑定
来源：http://aj.chemitech.net.cn

if let n = opt { print(n) }
来源：http://yw.521024.cn

[T20] Swift：数组操作
来源：http://yz.bjjhwx.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jm.bjjhwx.cn

[T21] Swift：遍历
来源：http://gn.lnxyls.cn

for x in a { print(x) }
来源：http://ov.9csxet.cn

[T22] Swift：字典
来源：http://zg.huixiangedu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zp.yuntaijiaju.cn

[T23] Swift：函数
来源：http://al.yuntaijiaju.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zt.yuntaijiaju.cn

[T24] Swift：闭包
来源：http://dk.jianghongdianzi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://lp.szsharing.cn

[T25] Swift：结构体
来源：http://gk.jctech888.com.cn

struct P { var x: Int }
来源：http://ei.newstarts.cn

[T26] Swift：类与重写
来源：http://jr.nicolike.cn

class A: Base { override func f() {} }
来源：http://av.521024.cn

[T27] Swift：错误处理
来源：http://ek.haigaiapp.cn

do { try f() } catch { print(error) }
来源：http://ki.9csxet.cn

[T28] Swift：枚举
来源：http://eb.szsharing.cn

enum Color { case red, green }
来源：http://wr.shxzskj.cn

[T29] Swift：guard 提前返回
来源：http://vf.521024.cn

guard let x = opt else { return }
来源：http://jy.nszjky.cn

[T30] Swift：协议
来源：http://pr.asd995.cn

protocol Shape { func area() -> Double }
来源：http://wa.huixinmuqiang.cn

[T31] Lua：Hello World
来源：http://dd.9csxet.cn

print("Hello")
来源：http://im.chemitech.net.cn

[T32] Lua：局部变量
来源：http://pj.huixiangedu.cn

local a = 1
来源：http://zg.huixiangedu.cn

[T33] Lua：表（数组）
来源：http://iw.nszjky.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://mj.9csxet.cn

[T34] Lua：遍历表
来源：http://cp.asd995.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://mo.wgjwhj.cn

[T35] Lua：字典表
来源：http://ol.gzmigu.cn

local d = { a = 1 };  d.b = 2
来源：http://nr.szsharing.cn

[T36] Lua：函数
来源：http://dp.huixiangedu.cn

function add(a, b) return a + b end
来源：http://oy.jctech888.com.cn

[T37] Lua：字符串拼接
来源：http://fr.521024.cn

"a" .. "b"
来源：http://pm.bookmarksfly.cn

[T38] Lua：条件
来源：http://zc.shxzskj.cn

if x > 0 then print("正") end
来源：http://mg.chemitech.net.cn

[T39] Lua：模式匹配
来源：http://fk.huixiangedu.cn

string.find(s, "%d+")
来源：http://il.muxihuayi.cn

[T40] Lua：元表
来源：http://rx.hahajie.cn

setmetatable({}, { __index = base })
来源：http://ti.asd995.cn

[T41] Perl：Hello World
来源：http://lh.shtwfgs.cn

print "Hello\n";
来源：http://ab.jctech888.com.cn

[T42] Perl：变量类型
来源：http://dq.colortex.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gt.newstarts.cn

[T43] Perl：字符串插值
来源：http://xf.hahajie.cn

"值: $a"
来源：http://dz.szsharing.cn

[T44] Perl：条件
来源：http://tp.muxihuayi.cn

if ($a > 0) { print "正"; }
来源：http://rd.huanxung.cn

[T45] Perl：数组遍历
来源：http://gq.chemitech.net.cn

for my $x (@arr) { print $x; }
来源：http://xw.asd995.cn

[T46] Perl：哈希操作
来源：http://sf.bookmarksfly.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://oi.hnjuh.cn

[T47] Perl：正则捕获
来源：http://ns.huixiangedu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://yg.nicolike.cn

[T48] Perl：正则替换
来源：http://cg.newstarts.cn

$s =~ s/old/new/g;
来源：http://fy.lnxyls.cn

[T49] Perl：函数
来源：http://dq.huanxung.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tc.huanxung.cn

[T50] Perl：逐行读文件
来源：http://ai.bjjhwx.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://jg.shxzukj.cn

while (my $line = <$fh>) { print $line; }
来源：http://el.nszjky.cn

[T51] Scala：Hello World
来源：http://ht.huixiangedu.cn

println("Hello")
来源：http://jw.haigaiapp.cn

[T52] Scala：变量
来源：http://rs.yuexingan06.cn

val a = 1;  var b = 2
来源：http://sx.chemitech.net.cn

[T53] Scala：字符串插值
来源：http://ub.hnjuh.cn

s"值: $b"
来源：http://je.bjjhwx.cn

[T54] Scala：集合映射
来源：http://qg.huixinmuqiang.cn

List(1, 2, 3).map(_ * 2)
来源：http://wv.colortex.cn

[T55] Scala：集合过滤
来源：http://pq.szsharing.cn

List(1, 2, 3).filter(_ > 1)
来源：http://yp.asd995.cn

[T56] Scala：样例类
来源：http://at.panjiajie.cn

case class User(name: String, age: Int)
来源：http://en.colortex.cn

[T57] Scala：模式匹配
来源：http://nw.yuntaijiaju.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://zj.huixinmuqiang.cn

[T58] Scala：函数定义
来源：http://rv.muxihuayi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://qa.bookmarksfly.cn

[T59] Scala：循环
来源：http://vl.newstarts.cn

for (i <- 1 to 10) println(i)
来源：http://mw.panjiajie.cn

[T60] Scala：折叠
来源：http://ie.panjiajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ur.nicolike.cn

================================================================================
来源：http://vi.chemitech.net.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dg.jctech888.com.cn

================================================================================
来源：http://lm.huixinmuqiang.cn

[U01] Py：创建虚拟环境
来源：http://sq.lnxyls.cn

python -m venv .venv && source .venv/bin/activate
来源：http://dl.lnxyls.cn

[U02] Py：导出 / 安装依赖
来源：http://gs.yuntaijiaju.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kj.bookmarksfly.cn

[U03] Py：加载 .env 配置
来源：http://zw.shtwfgs.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://he.huixiangedu.cn

[U04] Py：变量调试打印
来源：http://ps.wgjwhj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lm.muxihuayi.cn

[U05] Py：列表去重且保序
来源：http://ng.chemitech.net.cn

list(dict.fromkeys(arr))
来源：http://rm.newstarts.cn

[U06] Py：合并两个字典
来源：http://pt.bjjhwx.cn

{**a, **b}
来源：http://tc.yuexingan06.cn

[U07] Py：反转字典键值
来源：http://ho.haigaiapp.cn

{v: k for k, v in d.items()}
来源：http://gj.colortex.cn

[U08] Py：展平二维列表
来源：http://rw.haigaiapp.cn

[y for x in nested for y in x]
来源：http://pm.jctech888.com.cn

[U09] Py：字典取最大值的键
来源：http://uy.jianghongdianzi.cn

max(d, key=d.get)
来源：http://lz.newstarts.cn

[U10] Py：按值排序字典
来源：http://xu.yuexingan06.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gf.wgjwhj.cn

[U11] Py：生成器表达式
来源：http://it.jctech888.com.cn

(x * 2 for x in arr)
来源：http://sl.colortex.cn

[U12] Py：取出现最多的 3 个元素
来源：http://il.newstarts.cn

Counter(arr).most_common(3)
来源：http://ll.haigaiapp.cn

[U13] Py：固定长度队列
来源：http://cq.jianghongdianzi.cn

deque(maxlen=10)
来源：http://va.huixinmuqiang.cn

[U14] Py：分组收集到列表
来源：http://pq.bjjhwx.cn

defaultdict(list)
来源：http://ha.newstarts.cn

[U15] Py：高精度计时
来源：http://vt.yuntaijiaju.cn

t = time.perf_counter()
来源：http://kl.yuexingan06.cn

[U16] Py：命令行参数解析
来源：http://ky.muxihuayi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xt.bookmarksfly.cn

[U17] Py：初始化日志
来源：http://bz.chemitech.net.cn

logging.basicConfig(level=logging.INFO)
来源：http://ao.521024.cn

[U18] Py：预编译正则
来源：http://nu.bjjhwx.cn

pat = re.compile(r"\d+")
来源：http://it.szsharing.cn

[U19] Py：正则替换带回调
来源：http://qe.9csxet.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zk.chemitech.net.cn

[U20] Py：缓存函数结果
来源：http://ko.chemitech.net.cn

@functools.lru_cache(maxsize=None)
来源：http://en.nicolike.cn

[U21] Py：自定义上下文管理器
来源：http://lw.hahajie.cn

@contextlib.contextmanager
来源：http://zg.lnxyls.cn

[U22] Py：矩阵转置
来源：http://gz.shxzskj.cn

list(zip(*m))
来源：http://vq.hnjuh.cn

[U23] Py：分块读取大文件
来源：http://hg.shtwfgs.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://uy.shxzukj.cn

[U24] Py：路径操作
来源：http://kx.yuntaijiaju.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yn.panjiajie.cn

[U25] Py：CSV 按字典读
来源：http://fp.szsharing.cn

csv.DictReader(f)
来源：http://bk.lnxyls.cn

[U26] Py：并发下载
来源：http://uz.szxytkj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mq.bjjhwx.cn

[U27] Py：异步 HTTP
来源：http://nl.hnjuh.cn

aiohttp.ClientSession() 配合 async with
来源：http://mz.yuntaijiaju.cn

[U28] Py：类型别名
来源：http://ng.hahajie.cn

UserId = int
来源：http://ok.shxzskj.cn

[U29] Py：属性校验
来源：http://hx.jianghongdianzi.cn

@property 与 @x.setter 配合
来源：http://um.huixiangedu.cn

[U30] Py：数据类
来源：http://yo.jianghongdianzi.cn

@dataclass(slots=True)
来源：http://ge.shxzskj.cn

[U31] Py：单测
来源：http://bo.9csxet.cn

python -m pytest -q
来源：http://vo.newstarts.cn

[U32] Py：代码格式化
来源：http://vp.huixiangedu.cn

ruff format . && ruff check --fix .
来源：http://mu.asd995.cn

[U33] Py：打包发布
来源：http://om.newstarts.cn

python -m build  （依赖 pyproject.toml）
来源：http://tb.colortex.cn

[U34] Py：判断编码
来源：http://rb.huanxung.cn

chardet.detect(raw)
来源：http://jv.shtwfgs.cn

[U35] Py：发送邮件
来源：http://pb.huixiangedu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rj.wgjwhj.cn

[U36] Py：定时任务
来源：http://kg.bjjhwx.cn

schedule.every(10).minutes.do(job)
来源：http://ey.colortex.cn

[U37] Py：读写 Excel
来源：http://pc.haigaiapp.cn

pandas.read_excel / DataFrame.to_excel
来源：http://iw.szxytkj.cn

[U38] Py：获取脚本所在目录
来源：http://to.haigaiapp.cn

Path(__file__).resolve().parent
来源：http://sr.hnjuh.cn


<!-- 参考信息 -->