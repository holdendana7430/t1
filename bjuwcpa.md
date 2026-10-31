代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://hq.9csxet.cn

[S15] C：类型转换
来源：http://de.nicolike.cn

(double) a / b
来源：http://hd.gzmigu.cn

[S16] C：位操作置位
来源：http://hc.szsharing.cn

x |= (1 << 3);
来源：http://jl.muxihuayi.cn

[S17] C：安全拼接字符串
来源：http://nt.szxytkj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dq.jianghongdianzi.cn

[S18] C：命令行参数
来源：http://lg.asd995.cn

int main(int argc, char **argv)
来源：http://bl.yuntaijiaju.cn

[S19] C：快速排序
来源：http://ia.haigaiapp.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xv.huixinmuqiang.cn

[S20] C：二分查找
来源：http://wo.huixiangedu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xf.shxzskj.cn

[S21] C：字符类别判断
来源：http://rm.huixiangedu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kl.yuntaijiaju.cn

[S22] C：字符串转数字
来源：http://mg.colortex.cn

atoi("42");  strtod("3.14", NULL);
来源：http://do.gzmigu.cn

[S23] C：随机数
来源：http://io.colortex.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wz.lnxyls.cn

[S24] C：获取本地时间
来源：http://jo.nicolike.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sf.huixinmuqiang.cn

[S25] C：内存拷贝
来源：http://co.yuntaijiaju.cn

memcpy(dst, src, n);
来源：http://vc.521024.cn

[S26] C：内存清零
来源：http://jr.szsharing.cn

memset(a, 0, sizeof a);
来源：http://bn.hnjuh.cn

[S27] C：定义常量
来源：http://xm.yuntaijiaju.cn

const double PI = 3.14159;
来源：http://tv.yuntaijiaju.cn

[S28] C：静态变量
来源：http://sq.yuexingan06.cn

static int counter = 0;
来源：http://hn.521024.cn

[S29] C：变参函数
来源：http://mq.hahajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ou.9csxet.cn

[S30] C：头文件保护
来源：http://ha.colortex.cn

#ifndef X_H
来源：http://kq.panjiajie.cn

#define X_H
来源：http://ky.huixiangedu.cn

#endif
来源：http://jc.hnjuh.cn

[S31] C++：Hello World
来源：http://st.panjiajie.cn

#include <iostream>
来源：http://zf.szsharing.cn

int main() { std::cout << "Hello\n"; }
来源：http://rz.muxihuayi.cn

[S32] C++：字符串
来源：http://um.nicolike.cn

std::string s = "hi";  s += "!";
来源：http://gi.521024.cn

[S33] C++：vector 增删
来源：http://mv.521024.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pj.szsharing.cn

[S34] C++：遍历 vector
来源：http://ge.yuexingan06.cn

for (auto &x : v) { std::cout << x; }
来源：http://wz.newstarts.cn

[S35] C++：map
来源：http://ps.huixinmuqiang.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ce.nicolike.cn

[S36] C++：unordered_map
来源：http://fe.asd995.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zn.muxihuayi.cn

[S37] C++：set
来源：http://xh.muxihuayi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fs.panjiajie.cn

[S38] C++：排序
来源：http://ey.huixiangedu.cn

std::sort(v.begin(), v.end());
来源：http://bg.huixiangedu.cn

[S39] C++：自定义比较器排序
来源：http://zu.hnjuh.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kd.haigaiapp.cn

[S40] C++：查找元素
来源：http://ex.yuexingan06.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mc.muxihuayi.cn

[S41] C++：类与构造函数
来源：http://zp.shxzskj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ml.9csxet.cn

[S42] C++：继承与虚函数
来源：http://fe.hahajie.cn

class B : public Base { public: void f() override {} };
来源：http://ax.huanxung.cn

[S43] C++：智能指针
来源：http://ew.yuexingan06.cn

auto p = std::make_unique<int>(5);
来源：http://kv.gzmigu.cn

[S44] C++：引用传参
来源：http://zw.bookmarksfly.cn

void inc(int &x) { ++x; }
来源：http://fo.huanxung.cn

[S45] C++：lambda
来源：http://vi.huixinmuqiang.cn

auto add = [](int a, int b) { return a + b; };
来源：http://kn.panjiajie.cn

[S46] C++：函数模板
来源：http://pd.panjiajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bv.huixinmuqiang.cn

[S47] C++：结构化绑定遍历
来源：http://hh.lnxyls.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ma.shtwfgs.cn

[S48] C++：逐行读文件
来源：http://uj.bjjhwx.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jc.wgjwhj.cn

while (std::getline(in, line)) { }
来源：http://or.shxzukj.cn

[S49] C++：写文件
来源：http://ng.shxzukj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kx.newstarts.cn

[S50] C++：格式化数字
来源：http://ql.muxihuayi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ms.shxzskj.cn

[S51] C++：显式类型转换
来源：http://pq.jianghongdianzi.cn

static_cast<double>(a) / b
来源：http://cl.newstarts.cn

[S52] C++：const 与 noexcept
来源：http://eg.wgjwhj.cn

int size() const noexcept { return n_; }
来源：http://vt.haigaiapp.cn

[S53] C++：移动语义
来源：http://ro.nicolike.cn

std::vector<int> w = std::move(v);
来源：http://gk.asd995.cn

[S54] C++：异常处理
来源：http://yj.521024.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hl.shxzukj.cn

[S55] C++：结构化绑定
来源：http://xu.szsharing.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vn.asd995.cn

[S56] C++：optional
来源：http://nf.asd995.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wd.jianghongdianzi.cn

[S57] C++：编译期常量
来源：http://of.9csxet.cn

constexpr int N = 10;
来源：http://jx.muxihuayi.cn

[S58] C++：命名空间
来源：http://uc.gzmigu.cn

namespace ns { int f() { return 1; } }
来源：http://bm.asd995.cn

[S59] C++：静态断言
来源：http://oh.newstarts.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hb.szxytkj.cn

[S60] C++：遍历并删除元素
来源：http://la.yuexingan06.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ba.gzmigu.cn

================================================================================
来源：http://lg.yuntaijiaju.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://df.yuntaijiaju.cn

================================================================================
来源：http://hf.bookmarksfly.cn

[T01] Kotlin：Hello World
来源：http://el.newstarts.cn

println("Hello")
来源：http://gn.chemitech.net.cn

[T02] Kotlin：变量
来源：http://bl.huanxung.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qi.newstarts.cn

[T03] Kotlin：字符串模板
来源：http://mo.gzmigu.cn

"值: $b"
来源：http://mu.nicolike.cn

[T04] Kotlin：空安全
来源：http://dg.yuntaijiaju.cn

val n: String? = null;  n?.length
来源：http://nk.hahajie.cn

[T05] Kotlin：when 表达式
来源：http://co.asd995.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zo.shxzskj.cn

[T06] Kotlin：集合映射
来源：http://in.nicolike.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gb.szsharing.cn

[T07] Kotlin：集合过滤
来源：http://ds.bookmarksfly.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://oa.panjiajie.cn

[T08] Kotlin：数据类
来源：http://kp.asd995.cn

data class User(val name: String, val age: Int)
来源：http://gl.huixinmuqiang.cn

[T09] Kotlin：扩展函数
来源：http://ai.panjiajie.cn

fun String.exclaim() = this + "!"
来源：http://uu.hahajie.cn

[T10] Kotlin：默认参数
来源：http://is.9csxet.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ik.chemitech.net.cn

[T11] Kotlin：协程
来源：http://xc.panjiajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://rt.hnjuh.cn

[T12] Kotlin：解构声明
来源：http://ey.asd995.cn

val (a, b) = Pair(1, 2)
来源：http://wf.asd995.cn

[T13] Kotlin：只读 Map
来源：http://ft.newstarts.cn

val m = mapOf("a" to 1)
来源：http://zz.shxzukj.cn

[T14] Kotlin：循环
来源：http://ur.yuexingan06.cn

for (i in 1..10) println(i)
来源：http://uq.szsharing.cn

[T15] Kotlin：接口
来源：http://tu.jianghongdianzi.cn

interface Shape { fun area(): Double }
来源：http://ov.huanxung.cn

[T16] Swift：Hello World
来源：http://gz.huixiangedu.cn

print("Hello")
来源：http://gl.hahajie.cn

[T17] Swift：变量与常量
来源：http://zg.shtwfgs.cn

var a = 1;  let b = 2
来源：http://zz.jianghongdianzi.cn

[T18] Swift：字符串插值
来源：http://cq.huanxung.cn

"值: \(b)"
来源：http://xp.9csxet.cn

[T19] Swift：可选绑定
来源：http://pj.szxytkj.cn

if let n = opt { print(n) }
来源：http://ny.jctech888.com.cn

[T20] Swift：数组操作
来源：http://mj.huanxung.cn

var a = [1, 2, 3];  a.append(4)
来源：http://dt.shtwfgs.cn

[T21] Swift：遍历
来源：http://vw.lnxyls.cn

for x in a { print(x) }
来源：http://au.jctech888.com.cn

[T22] Swift：字典
来源：http://dw.521024.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ne.yuntaijiaju.cn

[T23] Swift：函数
来源：http://io.szsharing.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jf.huixinmuqiang.cn

[T24] Swift：闭包
来源：http://bw.bjjhwx.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://wf.shxzukj.cn

[T25] Swift：结构体
来源：http://jt.muxihuayi.cn

struct P { var x: Int }
来源：http://cj.yuntaijiaju.cn

[T26] Swift：类与重写
来源：http://hw.9csxet.cn

class A: Base { override func f() {} }
来源：http://ja.shxzskj.cn

[T27] Swift：错误处理
来源：http://zz.521024.cn

do { try f() } catch { print(error) }
来源：http://gl.jctech888.com.cn

[T28] Swift：枚举
来源：http://nu.lnxyls.cn

enum Color { case red, green }
来源：http://jd.hahajie.cn

[T29] Swift：guard 提前返回
来源：http://el.lnxyls.cn

guard let x = opt else { return }
来源：http://ry.asd995.cn

[T30] Swift：协议
来源：http://bq.huixinmuqiang.cn

protocol Shape { func area() -> Double }
来源：http://dq.colortex.cn

[T31] Lua：Hello World
来源：http://xf.nszjky.cn

print("Hello")
来源：http://tm.huanxung.cn

[T32] Lua：局部变量
来源：http://ej.hnjuh.cn

local a = 1
来源：http://ga.panjiajie.cn

[T33] Lua：表（数组）
来源：http://ka.szsharing.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ka.9csxet.cn

[T34] Lua：遍历表
来源：http://wn.hahajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ut.shxzskj.cn

[T35] Lua：字典表
来源：http://lh.muxihuayi.cn

local d = { a = 1 };  d.b = 2
来源：http://sy.huanxung.cn

[T36] Lua：函数
来源：http://lr.colortex.cn

function add(a, b) return a + b end
来源：http://hq.shxzskj.cn

[T37] Lua：字符串拼接
来源：http://up.shxzukj.cn

"a" .. "b"
来源：http://vn.huixiangedu.cn

[T38] Lua：条件
来源：http://ws.lnxyls.cn

if x > 0 then print("正") end
来源：http://gt.chemitech.net.cn

[T39] Lua：模式匹配
来源：http://qf.hahajie.cn

string.find(s, "%d+")
来源：http://wp.hnjuh.cn

[T40] Lua：元表
来源：http://tv.9csxet.cn

setmetatable({}, { __index = base })
来源：http://wz.jianghongdianzi.cn

[T41] Perl：Hello World
来源：http://xb.newstarts.cn

print "Hello\n";
来源：http://ev.newstarts.cn

[T42] Perl：变量类型
来源：http://hk.szxytkj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gt.jianghongdianzi.cn

[T43] Perl：字符串插值
来源：http://tr.huixiangedu.cn

"值: $a"
来源：http://np.colortex.cn

[T44] Perl：条件
来源：http://eo.nicolike.cn

if ($a > 0) { print "正"; }
来源：http://nb.wgjwhj.cn

[T45] Perl：数组遍历
来源：http://ks.colortex.cn

for my $x (@arr) { print $x; }
来源：http://gk.szxytkj.cn

[T46] Perl：哈希操作
来源：http://xr.yuexingan06.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lb.521024.cn

[T47] Perl：正则捕获
来源：http://th.shxzskj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xm.huixiangedu.cn

[T48] Perl：正则替换
来源：http://aa.jctech888.com.cn

$s =~ s/old/new/g;
来源：http://jh.haigaiapp.cn

[T49] Perl：函数
来源：http://vl.panjiajie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cs.shxzskj.cn

[T50] Perl：逐行读文件
来源：http://vv.chemitech.net.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rd.huixiangedu.cn

while (my $line = <$fh>) { print $line; }
来源：http://wh.nszjky.cn

[T51] Scala：Hello World
来源：http://qi.muxihuayi.cn

println("Hello")
来源：http://an.gzmigu.cn

[T52] Scala：变量
来源：http://cp.wgjwhj.cn

val a = 1;  var b = 2
来源：http://ac.nszjky.cn

[T53] Scala：字符串插值
来源：http://xx.hahajie.cn

s"值: $b"
来源：http://qs.shtwfgs.cn

[T54] Scala：集合映射
来源：http://am.nszjky.cn

List(1, 2, 3).map(_ * 2)
来源：http://fu.yuntaijiaju.cn

[T55] Scala：集合过滤
来源：http://cw.jianghongdianzi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://lc.szxytkj.cn

[T56] Scala：样例类
来源：http://ls.yuexingan06.cn

case class User(name: String, age: Int)
来源：http://yb.panjiajie.cn

[T57] Scala：模式匹配
来源：http://fd.yuexingan06.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://te.newstarts.cn

[T58] Scala：函数定义
来源：http://qu.colortex.cn

def add(a: Int, b: Int): Int = a + b
来源：http://xh.szxytkj.cn

[T59] Scala：循环
来源：http://ml.gzmigu.cn

for (i <- 1 to 10) println(i)
来源：http://pt.asd995.cn

[T60] Scala：折叠
来源：http://zx.shxzskj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qr.521024.cn

================================================================================
来源：http://qz.gzmigu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://er.colortex.cn

================================================================================
来源：http://sf.nszjky.cn

[U01] Py：创建虚拟环境
来源：http://an.521024.cn

python -m venv .venv && source .venv/bin/activate
来源：http://tb.yuntaijiaju.cn

[U02] Py：导出 / 安装依赖
来源：http://fx.bookmarksfly.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cv.huixinmuqiang.cn

[U03] Py：加载 .env 配置
来源：http://fz.jctech888.com.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://sx.yuntaijiaju.cn

[U04] Py：变量调试打印
来源：http://lr.yuntaijiaju.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://um.nszjky.cn

[U05] Py：列表去重且保序
来源：http://vq.shxzukj.cn

list(dict.fromkeys(arr))
来源：http://ss.chemitech.net.cn

[U06] Py：合并两个字典
来源：http://yr.hnjuh.cn

{**a, **b}
来源：http://fv.huixinmuqiang.cn

[U07] Py：反转字典键值
来源：http://hh.bookmarksfly.cn

{v: k for k, v in d.items()}
来源：http://xl.newstarts.cn

[U08] Py：展平二维列表
来源：http://yt.jianghongdianzi.cn

[y for x in nested for y in x]
来源：http://yq.muxihuayi.cn

[U09] Py：字典取最大值的键
来源：http://ys.nicolike.cn

max(d, key=d.get)
来源：http://bs.huanxung.cn

[U10] Py：按值排序字典
来源：http://er.colortex.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jc.gzmigu.cn

[U11] Py：生成器表达式
来源：http://re.hahajie.cn

(x * 2 for x in arr)
来源：http://mz.hnjuh.cn

[U12] Py：取出现最多的 3 个元素
来源：http://aj.521024.cn

Counter(arr).most_common(3)
来源：http://aq.szxytkj.cn

[U13] Py：固定长度队列
来源：http://mh.newstarts.cn

deque(maxlen=10)
来源：http://lz.nicolike.cn

[U14] Py：分组收集到列表
来源：http://go.newstarts.cn

defaultdict(list)
来源：http://jb.bookmarksfly.cn

[U15] Py：高精度计时
来源：http://vx.9csxet.cn

t = time.perf_counter()
来源：http://jp.bjjhwx.cn

[U16] Py：命令行参数解析
来源：http://qj.shxzskj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://st.colortex.cn

[U17] Py：初始化日志
来源：http://lf.jianghongdianzi.cn

logging.basicConfig(level=logging.INFO)
来源：http://lp.newstarts.cn

[U18] Py：预编译正则
来源：http://ge.colortex.cn

pat = re.compile(r"\d+")
来源：http://md.shxzukj.cn

[U19] Py：正则替换带回调
来源：http://il.shxzukj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ha.jctech888.com.cn

[U20] Py：缓存函数结果
来源：http://hb.521024.cn

@functools.lru_cache(maxsize=None)
来源：http://vg.huixiangedu.cn

[U21] Py：自定义上下文管理器
来源：http://wi.newstarts.cn

@contextlib.contextmanager
来源：http://mq.chemitech.net.cn

[U22] Py：矩阵转置
来源：http://rg.521024.cn

list(zip(*m))
来源：http://da.colortex.cn

[U23] Py：分块读取大文件
来源：http://sd.huanxung.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zz.szxytkj.cn

[U24] Py：路径操作
来源：http://fh.muxihuayi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mo.nszjky.cn

[U25] Py：CSV 按字典读
来源：http://sv.huixinmuqiang.cn

csv.DictReader(f)
来源：http://qi.yuntaijiaju.cn

[U26] Py：并发下载
来源：http://lc.colortex.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ra.shxzskj.cn

[U27] Py：异步 HTTP
来源：http://ex.hnjuh.cn

aiohttp.ClientSession() 配合 async with
来源：http://wp.521024.cn

[U28] Py：类型别名
来源：http://mi.shxzskj.cn

UserId = int
来源：http://kf.nicolike.cn

[U29] Py：属性校验
来源：http://al.huanxung.cn

@property 与 @x.setter 配合
来源：http://ev.gzmigu.cn

[U30] Py：数据类
来源：http://ez.bookmarksfly.cn

@dataclass(slots=True)
来源：http://hz.shxzskj.cn

[U31] Py：单测
来源：http://vz.shtwfgs.cn

python -m pytest -q
来源：http://iu.shtwfgs.cn

[U32] Py：代码格式化
来源：http://xy.yuntaijiaju.cn

ruff format . && ruff check --fix .
来源：http://ur.hnjuh.cn

[U33] Py：打包发布
来源：http://vx.jctech888.com.cn

python -m build  （依赖 pyproject.toml）
来源：http://kk.gzmigu.cn

[U34] Py：判断编码
来源：http://bj.shxzukj.cn

chardet.detect(raw)
来源：http://ut.shxzukj.cn

[U35] Py：发送邮件
来源：http://fz.shtwfgs.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gr.yuexingan06.cn

[U36] Py：定时任务
来源：http://pc.newstarts.cn

schedule.every(10).minutes.do(job)
来源：http://nx.shtwfgs.cn

[U37] Py：读写 Excel
来源：http://fz.wgjwhj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ha.colortex.cn

[U38] Py：获取脚本所在目录
来源：http://uj.szsharing.cn

Path(__file__).resolve().parent
来源：http://ig.hnjuh.cn


<!-- 参考信息 -->