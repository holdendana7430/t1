代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://yl.wgjwhj.cn

[S15] C：类型转换
来源：http://kj.wgjwhj.cn

(double) a / b
来源：http://kh.szxytkj.cn

[S16] C：位操作置位
来源：http://ct.huixiangedu.cn

x |= (1 << 3);
来源：http://xh.huixinmuqiang.cn

[S17] C：安全拼接字符串
来源：http://zy.shtwfgs.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://he.szsharing.cn

[S18] C：命令行参数
来源：http://da.521024.cn

int main(int argc, char **argv)
来源：http://xp.bookmarksfly.cn

[S19] C：快速排序
来源：http://uv.panjiajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gi.wgjwhj.cn

[S20] C：二分查找
来源：http://xb.hahajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pc.jianghongdianzi.cn

[S21] C：字符类别判断
来源：http://yd.shxzukj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hq.panjiajie.cn

[S22] C：字符串转数字
来源：http://jk.jianghongdianzi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://dh.jctech888.com.cn

[S23] C：随机数
来源：http://tg.bjjhwx.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://oi.panjiajie.cn

[S24] C：获取本地时间
来源：http://ie.jianghongdianzi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wf.shxzukj.cn

[S25] C：内存拷贝
来源：http://es.lnxyls.cn

memcpy(dst, src, n);
来源：http://kc.wgjwhj.cn

[S26] C：内存清零
来源：http://jh.nicolike.cn

memset(a, 0, sizeof a);
来源：http://on.gzmigu.cn

[S27] C：定义常量
来源：http://af.szsharing.cn

const double PI = 3.14159;
来源：http://xb.panjiajie.cn

[S28] C：静态变量
来源：http://jr.nicolike.cn

static int counter = 0;
来源：http://xf.jianghongdianzi.cn

[S29] C：变参函数
来源：http://mi.lnxyls.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ur.nicolike.cn

[S30] C：头文件保护
来源：http://rx.szxytkj.cn

#ifndef X_H
来源：http://gg.shtwfgs.cn

#define X_H
来源：http://ad.9csxet.cn

#endif
来源：http://ml.jianghongdianzi.cn

[S31] C++：Hello World
来源：http://kk.szxytkj.cn

#include <iostream>
来源：http://cm.colortex.cn

int main() { std::cout << "Hello\n"; }
来源：http://tg.muxihuayi.cn

[S32] C++：字符串
来源：http://dm.shxzskj.cn

std::string s = "hi";  s += "!";
来源：http://tg.newstarts.cn

[S33] C++：vector 增删
来源：http://sl.szsharing.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bv.shtwfgs.cn

[S34] C++：遍历 vector
来源：http://qt.jianghongdianzi.cn

for (auto &x : v) { std::cout << x; }
来源：http://ui.nicolike.cn

[S35] C++：map
来源：http://kg.szsharing.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zb.colortex.cn

[S36] C++：unordered_map
来源：http://ej.huanxung.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://de.chemitech.net.cn

[S37] C++：set
来源：http://xr.colortex.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pn.colortex.cn

[S38] C++：排序
来源：http://ke.panjiajie.cn

std::sort(v.begin(), v.end());
来源：http://sq.newstarts.cn

[S39] C++：自定义比较器排序
来源：http://yy.gzmigu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://iu.yuntaijiaju.cn

[S40] C++：查找元素
来源：http://tn.huixiangedu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ss.huanxung.cn

[S41] C++：类与构造函数
来源：http://zb.muxihuayi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ar.panjiajie.cn

[S42] C++：继承与虚函数
来源：http://zn.huixiangedu.cn

class B : public Base { public: void f() override {} };
来源：http://lx.hahajie.cn

[S43] C++：智能指针
来源：http://me.haigaiapp.cn

auto p = std::make_unique<int>(5);
来源：http://ox.panjiajie.cn

[S44] C++：引用传参
来源：http://hn.nszjky.cn

void inc(int &x) { ++x; }
来源：http://wx.huixiangedu.cn

[S45] C++：lambda
来源：http://av.huanxung.cn

auto add = [](int a, int b) { return a + b; };
来源：http://di.bookmarksfly.cn

[S46] C++：函数模板
来源：http://gp.jianghongdianzi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xb.huanxung.cn

[S47] C++：结构化绑定遍历
来源：http://lu.wgjwhj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://an.gzmigu.cn

[S48] C++：逐行读文件
来源：http://wc.huixiangedu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zw.szsharing.cn

while (std::getline(in, line)) { }
来源：http://ut.lnxyls.cn

[S49] C++：写文件
来源：http://bq.9csxet.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uo.chemitech.net.cn

[S50] C++：格式化数字
来源：http://rd.asd995.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pc.newstarts.cn

[S51] C++：显式类型转换
来源：http://eh.asd995.cn

static_cast<double>(a) / b
来源：http://kb.bookmarksfly.cn

[S52] C++：const 与 noexcept
来源：http://ut.huixiangedu.cn

int size() const noexcept { return n_; }
来源：http://av.panjiajie.cn

[S53] C++：移动语义
来源：http://ly.521024.cn

std::vector<int> w = std::move(v);
来源：http://jw.wgjwhj.cn

[S54] C++：异常处理
来源：http://qo.yuexingan06.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lg.bjjhwx.cn

[S55] C++：结构化绑定
来源：http://hm.9csxet.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://sw.wgjwhj.cn

[S56] C++：optional
来源：http://zk.huixinmuqiang.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dl.hnjuh.cn

[S57] C++：编译期常量
来源：http://dk.huixiangedu.cn

constexpr int N = 10;
来源：http://ru.hahajie.cn

[S58] C++：命名空间
来源：http://ow.panjiajie.cn

namespace ns { int f() { return 1; } }
来源：http://rm.nicolike.cn

[S59] C++：静态断言
来源：http://uc.huixinmuqiang.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ss.szsharing.cn

[S60] C++：遍历并删除元素
来源：http://xp.521024.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sr.hnjuh.cn

================================================================================
来源：http://fg.newstarts.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yv.shxzskj.cn

================================================================================
来源：http://ku.colortex.cn

[T01] Kotlin：Hello World
来源：http://km.huanxung.cn

println("Hello")
来源：http://cw.jctech888.com.cn

[T02] Kotlin：变量
来源：http://er.szxytkj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cs.szsharing.cn

[T03] Kotlin：字符串模板
来源：http://ik.nicolike.cn

"值: $b"
来源：http://my.bjjhwx.cn

[T04] Kotlin：空安全
来源：http://kv.9csxet.cn

val n: String? = null;  n?.length
来源：http://ie.jianghongdianzi.cn

[T05] Kotlin：when 表达式
来源：http://bo.gzmigu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ew.muxihuayi.cn

[T06] Kotlin：集合映射
来源：http://fm.shxzskj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://mg.panjiajie.cn

[T07] Kotlin：集合过滤
来源：http://rk.bjjhwx.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://jv.shtwfgs.cn

[T08] Kotlin：数据类
来源：http://ow.nszjky.cn

data class User(val name: String, val age: Int)
来源：http://mu.szxytkj.cn

[T09] Kotlin：扩展函数
来源：http://dh.jctech888.com.cn

fun String.exclaim() = this + "!"
来源：http://qt.9csxet.cn

[T10] Kotlin：默认参数
来源：http://lk.huanxung.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rc.szsharing.cn

[T11] Kotlin：协程
来源：http://sq.chemitech.net.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vx.yuntaijiaju.cn

[T12] Kotlin：解构声明
来源：http://qg.panjiajie.cn

val (a, b) = Pair(1, 2)
来源：http://se.huanxung.cn

[T13] Kotlin：只读 Map
来源：http://ud.nicolike.cn

val m = mapOf("a" to 1)
来源：http://vg.panjiajie.cn

[T14] Kotlin：循环
来源：http://el.asd995.cn

for (i in 1..10) println(i)
来源：http://nh.haigaiapp.cn

[T15] Kotlin：接口
来源：http://xf.huixiangedu.cn

interface Shape { fun area(): Double }
来源：http://yc.asd995.cn

[T16] Swift：Hello World
来源：http://tn.haigaiapp.cn

print("Hello")
来源：http://ik.colortex.cn

[T17] Swift：变量与常量
来源：http://js.jianghongdianzi.cn

var a = 1;  let b = 2
来源：http://ka.huixiangedu.cn

[T18] Swift：字符串插值
来源：http://lf.hahajie.cn

"值: \(b)"
来源：http://vp.bookmarksfly.cn

[T19] Swift：可选绑定
来源：http://xh.szsharing.cn

if let n = opt { print(n) }
来源：http://tn.szxytkj.cn

[T20] Swift：数组操作
来源：http://mt.szxytkj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qd.colortex.cn

[T21] Swift：遍历
来源：http://ar.yuntaijiaju.cn

for x in a { print(x) }
来源：http://lt.nicolike.cn

[T22] Swift：字典
来源：http://xu.szxytkj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://wc.szsharing.cn

[T23] Swift：函数
来源：http://vf.hnjuh.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ou.haigaiapp.cn

[T24] Swift：闭包
来源：http://nu.wgjwhj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://lz.lnxyls.cn

[T25] Swift：结构体
来源：http://xe.bookmarksfly.cn

struct P { var x: Int }
来源：http://lr.haigaiapp.cn

[T26] Swift：类与重写
来源：http://ez.gzmigu.cn

class A: Base { override func f() {} }
来源：http://tl.huanxung.cn

[T27] Swift：错误处理
来源：http://md.muxihuayi.cn

do { try f() } catch { print(error) }
来源：http://ab.chemitech.net.cn

[T28] Swift：枚举
来源：http://om.szxytkj.cn

enum Color { case red, green }
来源：http://cz.521024.cn

[T29] Swift：guard 提前返回
来源：http://sg.panjiajie.cn

guard let x = opt else { return }
来源：http://au.bookmarksfly.cn

[T30] Swift：协议
来源：http://sf.asd995.cn

protocol Shape { func area() -> Double }
来源：http://zz.shxzukj.cn

[T31] Lua：Hello World
来源：http://ge.huanxung.cn

print("Hello")
来源：http://vs.haigaiapp.cn

[T32] Lua：局部变量
来源：http://xu.yuntaijiaju.cn

local a = 1
来源：http://bk.nicolike.cn

[T33] Lua：表（数组）
来源：http://rz.shxzskj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ce.huanxung.cn

[T34] Lua：遍历表
来源：http://cv.nszjky.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://oh.shtwfgs.cn

[T35] Lua：字典表
来源：http://mi.hnjuh.cn

local d = { a = 1 };  d.b = 2
来源：http://dm.shtwfgs.cn

[T36] Lua：函数
来源：http://ou.huixiangedu.cn

function add(a, b) return a + b end
来源：http://af.szxytkj.cn

[T37] Lua：字符串拼接
来源：http://df.nicolike.cn

"a" .. "b"
来源：http://zu.9csxet.cn

[T38] Lua：条件
来源：http://vl.lnxyls.cn

if x > 0 then print("正") end
来源：http://yw.yuntaijiaju.cn

[T39] Lua：模式匹配
来源：http://dh.nszjky.cn

string.find(s, "%d+")
来源：http://ss.gzmigu.cn

[T40] Lua：元表
来源：http://pn.gzmigu.cn

setmetatable({}, { __index = base })
来源：http://pq.nszjky.cn

[T41] Perl：Hello World
来源：http://xv.bjjhwx.cn

print "Hello\n";
来源：http://db.nszjky.cn

[T42] Perl：变量类型
来源：http://bi.szxytkj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pv.521024.cn

[T43] Perl：字符串插值
来源：http://xx.muxihuayi.cn

"值: $a"
来源：http://gj.shtwfgs.cn

[T44] Perl：条件
来源：http://xz.hahajie.cn

if ($a > 0) { print "正"; }
来源：http://by.jianghongdianzi.cn

[T45] Perl：数组遍历
来源：http://js.shxzskj.cn

for my $x (@arr) { print $x; }
来源：http://yn.gzmigu.cn

[T46] Perl：哈希操作
来源：http://df.hahajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cm.gzmigu.cn

[T47] Perl：正则捕获
来源：http://ps.szsharing.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ys.haigaiapp.cn

[T48] Perl：正则替换
来源：http://ww.huixiangedu.cn

$s =~ s/old/new/g;
来源：http://hi.hahajie.cn

[T49] Perl：函数
来源：http://ju.huixiangedu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gp.muxihuayi.cn

[T50] Perl：逐行读文件
来源：http://xn.colortex.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wl.yuexingan06.cn

while (my $line = <$fh>) { print $line; }
来源：http://mz.huanxung.cn

[T51] Scala：Hello World
来源：http://bz.chemitech.net.cn

println("Hello")
来源：http://oh.nicolike.cn

[T52] Scala：变量
来源：http://kq.huixiangedu.cn

val a = 1;  var b = 2
来源：http://yh.bjjhwx.cn

[T53] Scala：字符串插值
来源：http://zv.yuntaijiaju.cn

s"值: $b"
来源：http://ss.asd995.cn

[T54] Scala：集合映射
来源：http://rz.hnjuh.cn

List(1, 2, 3).map(_ * 2)
来源：http://ex.chemitech.net.cn

[T55] Scala：集合过滤
来源：http://gy.szxytkj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://td.chemitech.net.cn

[T56] Scala：样例类
来源：http://qh.jctech888.com.cn

case class User(name: String, age: Int)
来源：http://ke.521024.cn

[T57] Scala：模式匹配
来源：http://xo.huixinmuqiang.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ez.yuntaijiaju.cn

[T58] Scala：函数定义
来源：http://ie.shxzukj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://qf.muxihuayi.cn

[T59] Scala：循环
来源：http://ys.9csxet.cn

for (i <- 1 to 10) println(i)
来源：http://tp.asd995.cn

[T60] Scala：折叠
来源：http://cd.nicolike.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://js.9csxet.cn

================================================================================
来源：http://hf.huixinmuqiang.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fj.chemitech.net.cn

================================================================================
来源：http://sv.hahajie.cn

[U01] Py：创建虚拟环境
来源：http://jq.asd995.cn

python -m venv .venv && source .venv/bin/activate
来源：http://to.yuntaijiaju.cn

[U02] Py：导出 / 安装依赖
来源：http://yu.nszjky.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://la.huanxung.cn

[U03] Py：加载 .env 配置
来源：http://mu.jctech888.com.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xw.shxzskj.cn

[U04] Py：变量调试打印
来源：http://sv.nicolike.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mp.9csxet.cn

[U05] Py：列表去重且保序
来源：http://qs.chemitech.net.cn

list(dict.fromkeys(arr))
来源：http://ti.shtwfgs.cn

[U06] Py：合并两个字典
来源：http://vy.yuntaijiaju.cn

{**a, **b}
来源：http://vm.shtwfgs.cn

[U07] Py：反转字典键值
来源：http://sp.huixinmuqiang.cn

{v: k for k, v in d.items()}
来源：http://sy.nicolike.cn

[U08] Py：展平二维列表
来源：http://rj.lnxyls.cn

[y for x in nested for y in x]
来源：http://tu.huixiangedu.cn

[U09] Py：字典取最大值的键
来源：http://sl.521024.cn

max(d, key=d.get)
来源：http://qf.hahajie.cn

[U10] Py：按值排序字典
来源：http://ic.szxytkj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kt.szxytkj.cn

[U11] Py：生成器表达式
来源：http://cv.asd995.cn

(x * 2 for x in arr)
来源：http://fh.huixinmuqiang.cn

[U12] Py：取出现最多的 3 个元素
来源：http://oy.jianghongdianzi.cn

Counter(arr).most_common(3)
来源：http://rm.colortex.cn

[U13] Py：固定长度队列
来源：http://xp.jctech888.com.cn

deque(maxlen=10)
来源：http://jl.hahajie.cn

[U14] Py：分组收集到列表
来源：http://jv.colortex.cn

defaultdict(list)
来源：http://ma.haigaiapp.cn

[U15] Py：高精度计时
来源：http://tq.muxihuayi.cn

t = time.perf_counter()
来源：http://gz.wgjwhj.cn

[U16] Py：命令行参数解析
来源：http://hk.gzmigu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zy.huixiangedu.cn

[U17] Py：初始化日志
来源：http://tz.szsharing.cn

logging.basicConfig(level=logging.INFO)
来源：http://iu.panjiajie.cn

[U18] Py：预编译正则
来源：http://ic.hahajie.cn

pat = re.compile(r"\d+")
来源：http://xt.muxihuayi.cn

[U19] Py：正则替换带回调
来源：http://kb.9csxet.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nj.lnxyls.cn

[U20] Py：缓存函数结果
来源：http://gw.szsharing.cn

@functools.lru_cache(maxsize=None)
来源：http://uz.yuexingan06.cn

[U21] Py：自定义上下文管理器
来源：http://it.bookmarksfly.cn

@contextlib.contextmanager
来源：http://ea.huanxung.cn

[U22] Py：矩阵转置
来源：http://ww.muxihuayi.cn

list(zip(*m))
来源：http://st.asd995.cn

[U23] Py：分块读取大文件
来源：http://gq.jianghongdianzi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ni.hahajie.cn

[U24] Py：路径操作
来源：http://ug.yuexingan06.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tn.shtwfgs.cn

[U25] Py：CSV 按字典读
来源：http://bf.colortex.cn

csv.DictReader(f)
来源：http://tc.nszjky.cn

[U26] Py：并发下载
来源：http://qe.hnjuh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://if.hnjuh.cn

[U27] Py：异步 HTTP
来源：http://hm.huixinmuqiang.cn

aiohttp.ClientSession() 配合 async with
来源：http://aq.shxzukj.cn

[U28] Py：类型别名
来源：http://lx.bjjhwx.cn

UserId = int
来源：http://ma.521024.cn

[U29] Py：属性校验
来源：http://to.nszjky.cn

@property 与 @x.setter 配合
来源：http://uj.szxytkj.cn

[U30] Py：数据类
来源：http://ys.521024.cn

@dataclass(slots=True)
来源：http://ka.huanxung.cn

[U31] Py：单测
来源：http://em.bookmarksfly.cn

python -m pytest -q
来源：http://ph.nicolike.cn

[U32] Py：代码格式化
来源：http://pk.asd995.cn

ruff format . && ruff check --fix .
来源：http://pz.huixiangedu.cn

[U33] Py：打包发布
来源：http://nw.shxzskj.cn

python -m build  （依赖 pyproject.toml）
来源：http://ow.huixinmuqiang.cn

[U34] Py：判断编码
来源：http://wy.huixinmuqiang.cn

chardet.detect(raw)
来源：http://iy.huixinmuqiang.cn

[U35] Py：发送邮件
来源：http://jx.nicolike.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zm.muxihuayi.cn

[U36] Py：定时任务
来源：http://ou.szxytkj.cn

schedule.every(10).minutes.do(job)
来源：http://ny.jianghongdianzi.cn

[U37] Py：读写 Excel
来源：http://ts.gzmigu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ou.hahajie.cn

[U38] Py：获取脚本所在目录
来源：http://fz.hnjuh.cn

Path(__file__).resolve().parent
来源：http://si.chemitech.net.cn


<!-- 参考信息 -->