代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://hf.panjiajie.cn

[S15] C：类型转换
来源：http://tg.bjjhwx.cn

(double) a / b
来源：http://on.huanxung.cn

[S16] C：位操作置位
来源：http://kv.szsharing.cn

x |= (1 << 3);
来源：http://kb.panjiajie.cn

[S17] C：安全拼接字符串
来源：http://zl.shxzskj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://oo.bookmarksfly.cn

[S18] C：命令行参数
来源：http://ya.colortex.cn

int main(int argc, char **argv)
来源：http://kl.jctech888.com.cn

[S19] C：快速排序
来源：http://om.gzmigu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ir.lnxyls.cn

[S20] C：二分查找
来源：http://sd.nicolike.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mz.521024.cn

[S21] C：字符类别判断
来源：http://qx.yuntaijiaju.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ef.shxzskj.cn

[S22] C：字符串转数字
来源：http://lo.hnjuh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vt.huixiangedu.cn

[S23] C：随机数
来源：http://fg.huixinmuqiang.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://uc.szsharing.cn

[S24] C：获取本地时间
来源：http://pq.asd995.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://la.shxzukj.cn

[S25] C：内存拷贝
来源：http://ao.yuntaijiaju.cn

memcpy(dst, src, n);
来源：http://pa.wgjwhj.cn

[S26] C：内存清零
来源：http://zx.jianghongdianzi.cn

memset(a, 0, sizeof a);
来源：http://ul.shxzukj.cn

[S27] C：定义常量
来源：http://rl.huanxung.cn

const double PI = 3.14159;
来源：http://nk.shtwfgs.cn

[S28] C：静态变量
来源：http://bk.colortex.cn

static int counter = 0;
来源：http://cb.hnjuh.cn

[S29] C：变参函数
来源：http://im.yuntaijiaju.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cu.9csxet.cn

[S30] C：头文件保护
来源：http://rt.newstarts.cn

#ifndef X_H
来源：http://qj.bookmarksfly.cn

#define X_H
来源：http://dk.panjiajie.cn

#endif
来源：http://hg.huixinmuqiang.cn

[S31] C++：Hello World
来源：http://oi.hnjuh.cn

#include <iostream>
来源：http://zy.shxzskj.cn

int main() { std::cout << "Hello\n"; }
来源：http://lr.muxihuayi.cn

[S32] C++：字符串
来源：http://bu.lnxyls.cn

std::string s = "hi";  s += "!";
来源：http://dy.hnjuh.cn

[S33] C++：vector 增删
来源：http://wf.521024.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sc.jctech888.com.cn

[S34] C++：遍历 vector
来源：http://st.huixiangedu.cn

for (auto &x : v) { std::cout << x; }
来源：http://dv.hnjuh.cn

[S35] C++：map
来源：http://ck.521024.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fc.huixiangedu.cn

[S36] C++：unordered_map
来源：http://rg.hnjuh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jm.szxytkj.cn

[S37] C++：set
来源：http://fm.yuntaijiaju.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zn.colortex.cn

[S38] C++：排序
来源：http://ll.nicolike.cn

std::sort(v.begin(), v.end());
来源：http://mq.chemitech.net.cn

[S39] C++：自定义比较器排序
来源：http://wx.szsharing.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://se.yuntaijiaju.cn

[S40] C++：查找元素
来源：http://gr.szxytkj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sv.szsharing.cn

[S41] C++：类与构造函数
来源：http://vq.9csxet.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ri.521024.cn

[S42] C++：继承与虚函数
来源：http://cx.bookmarksfly.cn

class B : public Base { public: void f() override {} };
来源：http://zw.shxzskj.cn

[S43] C++：智能指针
来源：http://se.huanxung.cn

auto p = std::make_unique<int>(5);
来源：http://oh.hnjuh.cn

[S44] C++：引用传参
来源：http://py.nicolike.cn

void inc(int &x) { ++x; }
来源：http://qd.9csxet.cn

[S45] C++：lambda
来源：http://ij.9csxet.cn

auto add = [](int a, int b) { return a + b; };
来源：http://cy.yuntaijiaju.cn

[S46] C++：函数模板
来源：http://tf.nszjky.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ql.hahajie.cn

[S47] C++：结构化绑定遍历
来源：http://rg.hahajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ga.muxihuayi.cn

[S48] C++：逐行读文件
来源：http://on.shxzskj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wo.jctech888.com.cn

while (std::getline(in, line)) { }
来源：http://og.shxzukj.cn

[S49] C++：写文件
来源：http://wl.asd995.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pd.shtwfgs.cn

[S50] C++：格式化数字
来源：http://ki.haigaiapp.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ai.nicolike.cn

[S51] C++：显式类型转换
来源：http://zk.hnjuh.cn

static_cast<double>(a) / b
来源：http://th.wgjwhj.cn

[S52] C++：const 与 noexcept
来源：http://if.hnjuh.cn

int size() const noexcept { return n_; }
来源：http://wf.lnxyls.cn

[S53] C++：移动语义
来源：http://hz.yuntaijiaju.cn

std::vector<int> w = std::move(v);
来源：http://ch.chemitech.net.cn

[S54] C++：异常处理
来源：http://mk.nicolike.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kw.shtwfgs.cn

[S55] C++：结构化绑定
来源：http://qj.521024.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kb.nicolike.cn

[S56] C++：optional
来源：http://di.panjiajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ri.huixiangedu.cn

[S57] C++：编译期常量
来源：http://eq.jctech888.com.cn

constexpr int N = 10;
来源：http://bx.jctech888.com.cn

[S58] C++：命名空间
来源：http://wm.panjiajie.cn

namespace ns { int f() { return 1; } }
来源：http://tn.jctech888.com.cn

[S59] C++：静态断言
来源：http://ed.bjjhwx.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gz.hahajie.cn

[S60] C++：遍历并删除元素
来源：http://dm.haigaiapp.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lp.yuntaijiaju.cn

================================================================================
来源：http://bb.yuexingan06.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xr.bookmarksfly.cn

================================================================================
来源：http://fq.yuntaijiaju.cn

[T01] Kotlin：Hello World
来源：http://px.asd995.cn

println("Hello")
来源：http://dd.hahajie.cn

[T02] Kotlin：变量
来源：http://fu.jianghongdianzi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vr.muxihuayi.cn

[T03] Kotlin：字符串模板
来源：http://kx.asd995.cn

"值: $b"
来源：http://wl.colortex.cn

[T04] Kotlin：空安全
来源：http://px.yuexingan06.cn

val n: String? = null;  n?.length
来源：http://qm.haigaiapp.cn

[T05] Kotlin：when 表达式
来源：http://oi.panjiajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bz.szsharing.cn

[T06] Kotlin：集合映射
来源：http://rs.panjiajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://nc.hahajie.cn

[T07] Kotlin：集合过滤
来源：http://bs.chemitech.net.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://jx.bookmarksfly.cn

[T08] Kotlin：数据类
来源：http://kt.521024.cn

data class User(val name: String, val age: Int)
来源：http://su.newstarts.cn

[T09] Kotlin：扩展函数
来源：http://fg.yuntaijiaju.cn

fun String.exclaim() = this + "!"
来源：http://be.newstarts.cn

[T10] Kotlin：默认参数
来源：http://bd.wgjwhj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://zk.huixinmuqiang.cn

[T11] Kotlin：协程
来源：http://gm.bookmarksfly.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://va.szsharing.cn

[T12] Kotlin：解构声明
来源：http://qy.huanxung.cn

val (a, b) = Pair(1, 2)
来源：http://vt.szsharing.cn

[T13] Kotlin：只读 Map
来源：http://af.muxihuayi.cn

val m = mapOf("a" to 1)
来源：http://fg.lnxyls.cn

[T14] Kotlin：循环
来源：http://nt.521024.cn

for (i in 1..10) println(i)
来源：http://sm.521024.cn

[T15] Kotlin：接口
来源：http://mt.shxzukj.cn

interface Shape { fun area(): Double }
来源：http://rm.shxzukj.cn

[T16] Swift：Hello World
来源：http://zm.yuntaijiaju.cn

print("Hello")
来源：http://ia.shxzukj.cn

[T17] Swift：变量与常量
来源：http://zz.szxytkj.cn

var a = 1;  let b = 2
来源：http://sl.haigaiapp.cn

[T18] Swift：字符串插值
来源：http://tc.chemitech.net.cn

"值: \(b)"
来源：http://zx.huixinmuqiang.cn

[T19] Swift：可选绑定
来源：http://bg.huanxung.cn

if let n = opt { print(n) }
来源：http://il.hnjuh.cn

[T20] Swift：数组操作
来源：http://kc.haigaiapp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://nv.521024.cn

[T21] Swift：遍历
来源：http://ui.asd995.cn

for x in a { print(x) }
来源：http://vt.hnjuh.cn

[T22] Swift：字典
来源：http://rt.9csxet.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fn.hnjuh.cn

[T23] Swift：函数
来源：http://gd.9csxet.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ox.shxzukj.cn

[T24] Swift：闭包
来源：http://xh.yuntaijiaju.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://of.jianghongdianzi.cn

[T25] Swift：结构体
来源：http://ic.muxihuayi.cn

struct P { var x: Int }
来源：http://uh.yuexingan06.cn

[T26] Swift：类与重写
来源：http://tl.bjjhwx.cn

class A: Base { override func f() {} }
来源：http://fe.huixiangedu.cn

[T27] Swift：错误处理
来源：http://of.panjiajie.cn

do { try f() } catch { print(error) }
来源：http://vo.colortex.cn

[T28] Swift：枚举
来源：http://pt.newstarts.cn

enum Color { case red, green }
来源：http://yf.521024.cn

[T29] Swift：guard 提前返回
来源：http://ex.muxihuayi.cn

guard let x = opt else { return }
来源：http://um.muxihuayi.cn

[T30] Swift：协议
来源：http://cp.huanxung.cn

protocol Shape { func area() -> Double }
来源：http://sg.shxzskj.cn

[T31] Lua：Hello World
来源：http://sm.yuexingan06.cn

print("Hello")
来源：http://ob.hnjuh.cn

[T32] Lua：局部变量
来源：http://as.muxihuayi.cn

local a = 1
来源：http://eg.nicolike.cn

[T33] Lua：表（数组）
来源：http://mq.colortex.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://lx.hnjuh.cn

[T34] Lua：遍历表
来源：http://ez.chemitech.net.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qe.521024.cn

[T35] Lua：字典表
来源：http://mr.hahajie.cn

local d = { a = 1 };  d.b = 2
来源：http://hx.gzmigu.cn

[T36] Lua：函数
来源：http://tn.nicolike.cn

function add(a, b) return a + b end
来源：http://xf.huanxung.cn

[T37] Lua：字符串拼接
来源：http://ol.shxzukj.cn

"a" .. "b"
来源：http://ki.hnjuh.cn

[T38] Lua：条件
来源：http://dg.nszjky.cn

if x > 0 then print("正") end
来源：http://xp.yuntaijiaju.cn

[T39] Lua：模式匹配
来源：http://hk.bookmarksfly.cn

string.find(s, "%d+")
来源：http://hb.nszjky.cn

[T40] Lua：元表
来源：http://hs.haigaiapp.cn

setmetatable({}, { __index = base })
来源：http://al.shxzukj.cn

[T41] Perl：Hello World
来源：http://km.haigaiapp.cn

print "Hello\n";
来源：http://xa.521024.cn

[T42] Perl：变量类型
来源：http://un.chemitech.net.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://re.9csxet.cn

[T43] Perl：字符串插值
来源：http://qg.szsharing.cn

"值: $a"
来源：http://tn.hahajie.cn

[T44] Perl：条件
来源：http://fk.bjjhwx.cn

if ($a > 0) { print "正"; }
来源：http://ob.panjiajie.cn

[T45] Perl：数组遍历
来源：http://yy.jctech888.com.cn

for my $x (@arr) { print $x; }
来源：http://rv.szxytkj.cn

[T46] Perl：哈希操作
来源：http://ec.newstarts.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nw.521024.cn

[T47] Perl：正则捕获
来源：http://ag.szsharing.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ny.jctech888.com.cn

[T48] Perl：正则替换
来源：http://wo.bjjhwx.cn

$s =~ s/old/new/g;
来源：http://fp.shxzukj.cn

[T49] Perl：函数
来源：http://fy.yuexingan06.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yf.huixiangedu.cn

[T50] Perl：逐行读文件
来源：http://kn.9csxet.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://lm.shtwfgs.cn

while (my $line = <$fh>) { print $line; }
来源：http://so.panjiajie.cn

[T51] Scala：Hello World
来源：http://yf.huixinmuqiang.cn

println("Hello")
来源：http://ru.haigaiapp.cn

[T52] Scala：变量
来源：http://bh.gzmigu.cn

val a = 1;  var b = 2
来源：http://oa.huanxung.cn

[T53] Scala：字符串插值
来源：http://kg.panjiajie.cn

s"值: $b"
来源：http://cx.huixiangedu.cn

[T54] Scala：集合映射
来源：http://jv.521024.cn

List(1, 2, 3).map(_ * 2)
来源：http://bm.huixinmuqiang.cn

[T55] Scala：集合过滤
来源：http://vn.yuntaijiaju.cn

List(1, 2, 3).filter(_ > 1)
来源：http://mv.shtwfgs.cn

[T56] Scala：样例类
来源：http://zq.haigaiapp.cn

case class User(name: String, age: Int)
来源：http://ww.jctech888.com.cn

[T57] Scala：模式匹配
来源：http://mg.yuntaijiaju.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://jm.colortex.cn

[T58] Scala：函数定义
来源：http://fu.hnjuh.cn

def add(a: Int, b: Int): Int = a + b
来源：http://rk.hnjuh.cn

[T59] Scala：循环
来源：http://gc.shxzukj.cn

for (i <- 1 to 10) println(i)
来源：http://ia.521024.cn

[T60] Scala：折叠
来源：http://bv.yuntaijiaju.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dv.asd995.cn

================================================================================
来源：http://xp.jctech888.com.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ze.bookmarksfly.cn

================================================================================
来源：http://hk.hahajie.cn

[U01] Py：创建虚拟环境
来源：http://wk.yuntaijiaju.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nd.jianghongdianzi.cn

[U02] Py：导出 / 安装依赖
来源：http://oo.chemitech.net.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lp.9csxet.cn

[U03] Py：加载 .env 配置
来源：http://iq.chemitech.net.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://tb.jctech888.com.cn

[U04] Py：变量调试打印
来源：http://fb.huixinmuqiang.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://li.yuntaijiaju.cn

[U05] Py：列表去重且保序
来源：http://bh.521024.cn

list(dict.fromkeys(arr))
来源：http://hh.wgjwhj.cn

[U06] Py：合并两个字典
来源：http://uc.shxzukj.cn

{**a, **b}
来源：http://ty.huanxung.cn

[U07] Py：反转字典键值
来源：http://tw.hahajie.cn

{v: k for k, v in d.items()}
来源：http://rn.9csxet.cn

[U08] Py：展平二维列表
来源：http://ls.shxzskj.cn

[y for x in nested for y in x]
来源：http://hn.jctech888.com.cn

[U09] Py：字典取最大值的键
来源：http://cw.hnjuh.cn

max(d, key=d.get)
来源：http://kh.huixiangedu.cn

[U10] Py：按值排序字典
来源：http://mb.hahajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ra.colortex.cn

[U11] Py：生成器表达式
来源：http://xh.yuntaijiaju.cn

(x * 2 for x in arr)
来源：http://zq.bookmarksfly.cn

[U12] Py：取出现最多的 3 个元素
来源：http://vx.hahajie.cn

Counter(arr).most_common(3)
来源：http://lx.nicolike.cn

[U13] Py：固定长度队列
来源：http://db.lnxyls.cn

deque(maxlen=10)
来源：http://nt.wgjwhj.cn

[U14] Py：分组收集到列表
来源：http://jb.haigaiapp.cn

defaultdict(list)
来源：http://ua.shxzukj.cn

[U15] Py：高精度计时
来源：http://pl.yuntaijiaju.cn

t = time.perf_counter()
来源：http://ea.gzmigu.cn

[U16] Py：命令行参数解析
来源：http://tn.szxytkj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cl.huixinmuqiang.cn

[U17] Py：初始化日志
来源：http://qj.hahajie.cn

logging.basicConfig(level=logging.INFO)
来源：http://wj.wgjwhj.cn

[U18] Py：预编译正则
来源：http://pn.huanxung.cn

pat = re.compile(r"\d+")
来源：http://qu.wgjwhj.cn

[U19] Py：正则替换带回调
来源：http://kv.hahajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://im.szsharing.cn

[U20] Py：缓存函数结果
来源：http://ll.colortex.cn

@functools.lru_cache(maxsize=None)
来源：http://oe.chemitech.net.cn

[U21] Py：自定义上下文管理器
来源：http://ed.9csxet.cn

@contextlib.contextmanager
来源：http://bt.shtwfgs.cn

[U22] Py：矩阵转置
来源：http://kk.nicolike.cn

list(zip(*m))
来源：http://oi.yuntaijiaju.cn

[U23] Py：分块读取大文件
来源：http://xh.9csxet.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mt.huixinmuqiang.cn

[U24] Py：路径操作
来源：http://pz.huixinmuqiang.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://it.chemitech.net.cn

[U25] Py：CSV 按字典读
来源：http://it.lnxyls.cn

csv.DictReader(f)
来源：http://yh.nszjky.cn

[U26] Py：并发下载
来源：http://mw.bjjhwx.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://de.shtwfgs.cn

[U27] Py：异步 HTTP
来源：http://hn.bookmarksfly.cn

aiohttp.ClientSession() 配合 async with
来源：http://cg.wgjwhj.cn

[U28] Py：类型别名
来源：http://gr.asd995.cn

UserId = int
来源：http://qe.shtwfgs.cn

[U29] Py：属性校验
来源：http://it.nicolike.cn

@property 与 @x.setter 配合
来源：http://xk.wgjwhj.cn

[U30] Py：数据类
来源：http://fo.521024.cn

@dataclass(slots=True)
来源：http://xt.nicolike.cn

[U31] Py：单测
来源：http://mg.yuexingan06.cn

python -m pytest -q
来源：http://vw.nszjky.cn

[U32] Py：代码格式化
来源：http://fe.chemitech.net.cn

ruff format . && ruff check --fix .
来源：http://zo.asd995.cn

[U33] Py：打包发布
来源：http://hl.yuexingan06.cn

python -m build  （依赖 pyproject.toml）
来源：http://fp.shtwfgs.cn

[U34] Py：判断编码
来源：http://mr.huanxung.cn

chardet.detect(raw)
来源：http://vl.hnjuh.cn

[U35] Py：发送邮件
来源：http://vp.bjjhwx.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://em.chemitech.net.cn

[U36] Py：定时任务
来源：http://cs.panjiajie.cn

schedule.every(10).minutes.do(job)
来源：http://zb.shxzskj.cn

[U37] Py：读写 Excel
来源：http://bv.huanxung.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ax.szxytkj.cn

[U38] Py：获取脚本所在目录
来源：http://xo.panjiajie.cn

Path(__file__).resolve().parent
来源：http://la.hahajie.cn


<!-- 参考信息 -->