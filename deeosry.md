代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://yu.nszjky.cn

[S15] C：类型转换
来源：http://qr.nszjky.cn

(double) a / b
来源：http://wd.panjiajie.cn

[S16] C：位操作置位
来源：http://pk.gzmigu.cn

x |= (1 << 3);
来源：http://nk.hnjuh.cn

[S17] C：安全拼接字符串
来源：http://qh.huanxung.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hb.jianghongdianzi.cn

[S18] C：命令行参数
来源：http://ao.nicolike.cn

int main(int argc, char **argv)
来源：http://mt.9csxet.cn

[S19] C：快速排序
来源：http://ej.huixiangedu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://uj.gzmigu.cn

[S20] C：二分查找
来源：http://xh.colortex.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ap.colortex.cn

[S21] C：字符类别判断
来源：http://wo.yuntaijiaju.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ni.colortex.cn

[S22] C：字符串转数字
来源：http://wh.wgjwhj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://uq.jctech888.com.cn

[S23] C：随机数
来源：http://zf.szxytkj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wu.bjjhwx.cn

[S24] C：获取本地时间
来源：http://rx.jianghongdianzi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rq.huixinmuqiang.cn

[S25] C：内存拷贝
来源：http://na.huanxung.cn

memcpy(dst, src, n);
来源：http://ct.shxzskj.cn

[S26] C：内存清零
来源：http://gd.jctech888.com.cn

memset(a, 0, sizeof a);
来源：http://us.muxihuayi.cn

[S27] C：定义常量
来源：http://qg.asd995.cn

const double PI = 3.14159;
来源：http://xv.521024.cn

[S28] C：静态变量
来源：http://hz.lnxyls.cn

static int counter = 0;
来源：http://xh.yuexingan06.cn

[S29] C：变参函数
来源：http://ym.chemitech.net.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ne.nszjky.cn

[S30] C：头文件保护
来源：http://yn.shxzskj.cn

#ifndef X_H
来源：http://au.bjjhwx.cn

#define X_H
来源：http://ti.9csxet.cn

#endif
来源：http://ar.bjjhwx.cn

[S31] C++：Hello World
来源：http://wd.szsharing.cn

#include <iostream>
来源：http://on.nszjky.cn

int main() { std::cout << "Hello\n"; }
来源：http://ok.nicolike.cn

[S32] C++：字符串
来源：http://ft.nszjky.cn

std::string s = "hi";  s += "!";
来源：http://qv.huixiangedu.cn

[S33] C++：vector 增删
来源：http://qm.colortex.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sz.huanxung.cn

[S34] C++：遍历 vector
来源：http://dx.panjiajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://fz.huanxung.cn

[S35] C++：map
来源：http://yi.shxzukj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ym.jianghongdianzi.cn

[S36] C++：unordered_map
来源：http://qu.521024.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mp.9csxet.cn

[S37] C++：set
来源：http://sq.9csxet.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lq.colortex.cn

[S38] C++：排序
来源：http://lr.jctech888.com.cn

std::sort(v.begin(), v.end());
来源：http://yh.yuntaijiaju.cn

[S39] C++：自定义比较器排序
来源：http://kn.wgjwhj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ms.huanxung.cn

[S40] C++：查找元素
来源：http://ug.panjiajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bs.shtwfgs.cn

[S41] C++：类与构造函数
来源：http://kr.huixiangedu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jw.521024.cn

[S42] C++：继承与虚函数
来源：http://yb.huixinmuqiang.cn

class B : public Base { public: void f() override {} };
来源：http://dj.lnxyls.cn

[S43] C++：智能指针
来源：http://op.bookmarksfly.cn

auto p = std::make_unique<int>(5);
来源：http://px.yuexingan06.cn

[S44] C++：引用传参
来源：http://pq.szsharing.cn

void inc(int &x) { ++x; }
来源：http://jv.szxytkj.cn

[S45] C++：lambda
来源：http://da.hnjuh.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xz.huixinmuqiang.cn

[S46] C++：函数模板
来源：http://pc.bjjhwx.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vd.yuexingan06.cn

[S47] C++：结构化绑定遍历
来源：http://tr.hnjuh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gz.shxzukj.cn

[S48] C++：逐行读文件
来源：http://ya.haigaiapp.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ws.shxzskj.cn

while (std::getline(in, line)) { }
来源：http://es.shtwfgs.cn

[S49] C++：写文件
来源：http://vf.szxytkj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gn.bjjhwx.cn

[S50] C++：格式化数字
来源：http://fc.nicolike.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sg.nicolike.cn

[S51] C++：显式类型转换
来源：http://un.bjjhwx.cn

static_cast<double>(a) / b
来源：http://xn.huanxung.cn

[S52] C++：const 与 noexcept
来源：http://pk.hnjuh.cn

int size() const noexcept { return n_; }
来源：http://nz.gzmigu.cn

[S53] C++：移动语义
来源：http://gi.9csxet.cn

std::vector<int> w = std::move(v);
来源：http://ea.szsharing.cn

[S54] C++：异常处理
来源：http://lh.yuexingan06.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hw.colortex.cn

[S55] C++：结构化绑定
来源：http://oo.colortex.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://nv.huixiangedu.cn

[S56] C++：optional
来源：http://sh.huixiangedu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qp.szsharing.cn

[S57] C++：编译期常量
来源：http://ap.hnjuh.cn

constexpr int N = 10;
来源：http://dr.panjiajie.cn

[S58] C++：命名空间
来源：http://qt.9csxet.cn

namespace ns { int f() { return 1; } }
来源：http://th.yuexingan06.cn

[S59] C++：静态断言
来源：http://sf.szsharing.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tb.huanxung.cn

[S60] C++：遍历并删除元素
来源：http://tv.9csxet.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uq.chemitech.net.cn

================================================================================
来源：http://lw.shxzskj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uk.hahajie.cn

================================================================================
来源：http://vl.szxytkj.cn

[T01] Kotlin：Hello World
来源：http://zw.9csxet.cn

println("Hello")
来源：http://go.shxzukj.cn

[T02] Kotlin：变量
来源：http://hp.shxzukj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://it.asd995.cn

[T03] Kotlin：字符串模板
来源：http://bd.colortex.cn

"值: $b"
来源：http://ga.bookmarksfly.cn

[T04] Kotlin：空安全
来源：http://qd.bookmarksfly.cn

val n: String? = null;  n?.length
来源：http://kj.huixiangedu.cn

[T05] Kotlin：when 表达式
来源：http://yj.haigaiapp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jr.9csxet.cn

[T06] Kotlin：集合映射
来源：http://zp.chemitech.net.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ai.nszjky.cn

[T07] Kotlin：集合过滤
来源：http://th.asd995.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xg.szsharing.cn

[T08] Kotlin：数据类
来源：http://xu.shxzskj.cn

data class User(val name: String, val age: Int)
来源：http://gw.szxytkj.cn

[T09] Kotlin：扩展函数
来源：http://ok.jianghongdianzi.cn

fun String.exclaim() = this + "!"
来源：http://rj.wgjwhj.cn

[T10] Kotlin：默认参数
来源：http://fv.hnjuh.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://nt.huanxung.cn

[T11] Kotlin：协程
来源：http://tw.9csxet.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jp.gzmigu.cn

[T12] Kotlin：解构声明
来源：http://ny.hnjuh.cn

val (a, b) = Pair(1, 2)
来源：http://py.szxytkj.cn

[T13] Kotlin：只读 Map
来源：http://sn.hahajie.cn

val m = mapOf("a" to 1)
来源：http://gx.panjiajie.cn

[T14] Kotlin：循环
来源：http://wi.huanxung.cn

for (i in 1..10) println(i)
来源：http://mj.huixiangedu.cn

[T15] Kotlin：接口
来源：http://pg.shxzukj.cn

interface Shape { fun area(): Double }
来源：http://sj.panjiajie.cn

[T16] Swift：Hello World
来源：http://tz.521024.cn

print("Hello")
来源：http://uh.colortex.cn

[T17] Swift：变量与常量
来源：http://ky.colortex.cn

var a = 1;  let b = 2
来源：http://mf.muxihuayi.cn

[T18] Swift：字符串插值
来源：http://fh.bjjhwx.cn

"值: \(b)"
来源：http://px.lnxyls.cn

[T19] Swift：可选绑定
来源：http://vg.huixiangedu.cn

if let n = opt { print(n) }
来源：http://pj.huixinmuqiang.cn

[T20] Swift：数组操作
来源：http://pn.muxihuayi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ew.wgjwhj.cn

[T21] Swift：遍历
来源：http://zj.jianghongdianzi.cn

for x in a { print(x) }
来源：http://sq.yuntaijiaju.cn

[T22] Swift：字典
来源：http://ru.hahajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ep.haigaiapp.cn

[T23] Swift：函数
来源：http://wh.szxytkj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mx.hnjuh.cn

[T24] Swift：闭包
来源：http://in.nszjky.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://bp.bookmarksfly.cn

[T25] Swift：结构体
来源：http://ro.bjjhwx.cn

struct P { var x: Int }
来源：http://ti.colortex.cn

[T26] Swift：类与重写
来源：http://io.szxytkj.cn

class A: Base { override func f() {} }
来源：http://oa.nszjky.cn

[T27] Swift：错误处理
来源：http://up.yuexingan06.cn

do { try f() } catch { print(error) }
来源：http://pf.nicolike.cn

[T28] Swift：枚举
来源：http://qm.jctech888.com.cn

enum Color { case red, green }
来源：http://oe.huixinmuqiang.cn

[T29] Swift：guard 提前返回
来源：http://hn.gzmigu.cn

guard let x = opt else { return }
来源：http://wd.gzmigu.cn

[T30] Swift：协议
来源：http://ws.shxzukj.cn

protocol Shape { func area() -> Double }
来源：http://dc.asd995.cn

[T31] Lua：Hello World
来源：http://mt.nicolike.cn

print("Hello")
来源：http://pc.nszjky.cn

[T32] Lua：局部变量
来源：http://rz.gzmigu.cn

local a = 1
来源：http://er.jianghongdianzi.cn

[T33] Lua：表（数组）
来源：http://zn.nicolike.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://oo.huanxung.cn

[T34] Lua：遍历表
来源：http://ep.jianghongdianzi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://hv.colortex.cn

[T35] Lua：字典表
来源：http://re.nicolike.cn

local d = { a = 1 };  d.b = 2
来源：http://xu.lnxyls.cn

[T36] Lua：函数
来源：http://xk.shtwfgs.cn

function add(a, b) return a + b end
来源：http://ug.jctech888.com.cn

[T37] Lua：字符串拼接
来源：http://gx.panjiajie.cn

"a" .. "b"
来源：http://zk.shxzskj.cn

[T38] Lua：条件
来源：http://qj.panjiajie.cn

if x > 0 then print("正") end
来源：http://rr.yuntaijiaju.cn

[T39] Lua：模式匹配
来源：http://rs.colortex.cn

string.find(s, "%d+")
来源：http://rf.9csxet.cn

[T40] Lua：元表
来源：http://oj.nszjky.cn

setmetatable({}, { __index = base })
来源：http://sm.shtwfgs.cn

[T41] Perl：Hello World
来源：http://nb.haigaiapp.cn

print "Hello\n";
来源：http://vq.asd995.cn

[T42] Perl：变量类型
来源：http://qc.521024.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://li.shxzskj.cn

[T43] Perl：字符串插值
来源：http://kj.521024.cn

"值: $a"
来源：http://st.hnjuh.cn

[T44] Perl：条件
来源：http://rc.wgjwhj.cn

if ($a > 0) { print "正"; }
来源：http://me.huanxung.cn

[T45] Perl：数组遍历
来源：http://dm.newstarts.cn

for my $x (@arr) { print $x; }
来源：http://ys.bookmarksfly.cn

[T46] Perl：哈希操作
来源：http://fb.newstarts.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xj.jianghongdianzi.cn

[T47] Perl：正则捕获
来源：http://jf.huanxung.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://fm.shxzskj.cn

[T48] Perl：正则替换
来源：http://zk.muxihuayi.cn

$s =~ s/old/new/g;
来源：http://fe.huixiangedu.cn

[T49] Perl：函数
来源：http://wd.shxzskj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gl.szxytkj.cn

[T50] Perl：逐行读文件
来源：http://wu.wgjwhj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ri.huanxung.cn

while (my $line = <$fh>) { print $line; }
来源：http://dk.bjjhwx.cn

[T51] Scala：Hello World
来源：http://jw.chemitech.net.cn

println("Hello")
来源：http://rg.jianghongdianzi.cn

[T52] Scala：变量
来源：http://ny.panjiajie.cn

val a = 1;  var b = 2
来源：http://br.jctech888.com.cn

[T53] Scala：字符串插值
来源：http://su.huixinmuqiang.cn

s"值: $b"
来源：http://cj.szxytkj.cn

[T54] Scala：集合映射
来源：http://il.muxihuayi.cn

List(1, 2, 3).map(_ * 2)
来源：http://tg.9csxet.cn

[T55] Scala：集合过滤
来源：http://rn.9csxet.cn

List(1, 2, 3).filter(_ > 1)
来源：http://zv.nicolike.cn

[T56] Scala：样例类
来源：http://lt.521024.cn

case class User(name: String, age: Int)
来源：http://uw.shxzukj.cn

[T57] Scala：模式匹配
来源：http://mh.yuexingan06.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://zb.9csxet.cn

[T58] Scala：函数定义
来源：http://re.nicolike.cn

def add(a: Int, b: Int): Int = a + b
来源：http://uj.yuexingan06.cn

[T59] Scala：循环
来源：http://zj.hnjuh.cn

for (i <- 1 to 10) println(i)
来源：http://si.szxytkj.cn

[T60] Scala：折叠
来源：http://xv.bookmarksfly.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ga.huixiangedu.cn

================================================================================
来源：http://vb.jctech888.com.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fm.szxytkj.cn

================================================================================
来源：http://si.szxytkj.cn

[U01] Py：创建虚拟环境
来源：http://bl.gzmigu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zn.hahajie.cn

[U02] Py：导出 / 安装依赖
来源：http://of.wgjwhj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ba.asd995.cn

[U03] Py：加载 .env 配置
来源：http://wk.nicolike.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://mj.huanxung.cn

[U04] Py：变量调试打印
来源：http://lz.wgjwhj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pt.9csxet.cn

[U05] Py：列表去重且保序
来源：http://au.nicolike.cn

list(dict.fromkeys(arr))
来源：http://cs.shtwfgs.cn

[U06] Py：合并两个字典
来源：http://zl.521024.cn

{**a, **b}
来源：http://ag.colortex.cn

[U07] Py：反转字典键值
来源：http://vy.huixiangedu.cn

{v: k for k, v in d.items()}
来源：http://pi.huanxung.cn

[U08] Py：展平二维列表
来源：http://vh.asd995.cn

[y for x in nested for y in x]
来源：http://sr.szxytkj.cn

[U09] Py：字典取最大值的键
来源：http://ng.shxzskj.cn

max(d, key=d.get)
来源：http://sc.jianghongdianzi.cn

[U10] Py：按值排序字典
来源：http://gq.panjiajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://at.huixinmuqiang.cn

[U11] Py：生成器表达式
来源：http://oy.yuexingan06.cn

(x * 2 for x in arr)
来源：http://cc.shxzukj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://dp.colortex.cn

Counter(arr).most_common(3)
来源：http://qy.yuexingan06.cn

[U13] Py：固定长度队列
来源：http://wg.huixiangedu.cn

deque(maxlen=10)
来源：http://cn.szsharing.cn

[U14] Py：分组收集到列表
来源：http://ey.szxytkj.cn

defaultdict(list)
来源：http://sa.lnxyls.cn

[U15] Py：高精度计时
来源：http://jk.lnxyls.cn

t = time.perf_counter()
来源：http://cd.jianghongdianzi.cn

[U16] Py：命令行参数解析
来源：http://kg.muxihuayi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sv.newstarts.cn

[U17] Py：初始化日志
来源：http://ib.nszjky.cn

logging.basicConfig(level=logging.INFO)
来源：http://nz.szxytkj.cn

[U18] Py：预编译正则
来源：http://rx.szsharing.cn

pat = re.compile(r"\d+")
来源：http://qd.521024.cn

[U19] Py：正则替换带回调
来源：http://uq.newstarts.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://co.hnjuh.cn

[U20] Py：缓存函数结果
来源：http://kw.shxzskj.cn

@functools.lru_cache(maxsize=None)
来源：http://jz.szxytkj.cn

[U21] Py：自定义上下文管理器
来源：http://nl.panjiajie.cn

@contextlib.contextmanager
来源：http://vm.chemitech.net.cn

[U22] Py：矩阵转置
来源：http://pk.jctech888.com.cn

list(zip(*m))
来源：http://ax.yuexingan06.cn

[U23] Py：分块读取大文件
来源：http://kj.nicolike.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cw.shxzukj.cn

[U24] Py：路径操作
来源：http://cb.lnxyls.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cf.nszjky.cn

[U25] Py：CSV 按字典读
来源：http://wx.asd995.cn

csv.DictReader(f)
来源：http://fa.haigaiapp.cn

[U26] Py：并发下载
来源：http://fl.9csxet.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wd.jctech888.com.cn

[U27] Py：异步 HTTP
来源：http://hh.bjjhwx.cn

aiohttp.ClientSession() 配合 async with
来源：http://pa.panjiajie.cn

[U28] Py：类型别名
来源：http://ko.newstarts.cn

UserId = int
来源：http://np.yuexingan06.cn

[U29] Py：属性校验
来源：http://bu.colortex.cn

@property 与 @x.setter 配合
来源：http://yk.jianghongdianzi.cn

[U30] Py：数据类
来源：http://nh.shxzskj.cn

@dataclass(slots=True)
来源：http://bt.hahajie.cn

[U31] Py：单测
来源：http://qw.huixinmuqiang.cn

python -m pytest -q
来源：http://ug.bjjhwx.cn

[U32] Py：代码格式化
来源：http://iu.huanxung.cn

ruff format . && ruff check --fix .
来源：http://hn.wgjwhj.cn

[U33] Py：打包发布
来源：http://sc.huixinmuqiang.cn

python -m build  （依赖 pyproject.toml）
来源：http://co.wgjwhj.cn

[U34] Py：判断编码
来源：http://im.hahajie.cn

chardet.detect(raw)
来源：http://bx.nszjky.cn

[U35] Py：发送邮件
来源：http://yd.jianghongdianzi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ds.szxytkj.cn

[U36] Py：定时任务
来源：http://ji.szsharing.cn

schedule.every(10).minutes.do(job)
来源：http://pe.newstarts.cn

[U37] Py：读写 Excel
来源：http://kk.shtwfgs.cn

pandas.read_excel / DataFrame.to_excel
来源：http://si.jianghongdianzi.cn

[U38] Py：获取脚本所在目录
来源：http://cx.bjjhwx.cn

Path(__file__).resolve().parent
来源：http://lv.jctech888.com.cn


<!-- 参考信息 -->