代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://kp.wgjwhj.cn

[S15] C：类型转换
来源：http://au.9csxet.cn

(double) a / b
来源：http://ry.521024.cn

[S16] C：位操作置位
来源：http://nf.wgjwhj.cn

x |= (1 << 3);
来源：http://xm.hnjuh.cn

[S17] C：安全拼接字符串
来源：http://td.muxihuayi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ry.gzmigu.cn

[S18] C：命令行参数
来源：http://yd.jianghongdianzi.cn

int main(int argc, char **argv)
来源：http://ne.9csxet.cn

[S19] C：快速排序
来源：http://vi.yuntaijiaju.cn

qsort(a, n, sizeof(int), cmp);
来源：http://bi.panjiajie.cn

[S20] C：二分查找
来源：http://hi.haigaiapp.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xj.bookmarksfly.cn

[S21] C：字符类别判断
来源：http://id.hnjuh.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ej.jianghongdianzi.cn

[S22] C：字符串转数字
来源：http://ug.nszjky.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wy.521024.cn

[S23] C：随机数
来源：http://cr.9csxet.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://te.shxzskj.cn

[S24] C：获取本地时间
来源：http://ds.colortex.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jz.huixinmuqiang.cn

[S25] C：内存拷贝
来源：http://nw.521024.cn

memcpy(dst, src, n);
来源：http://pp.shxzskj.cn

[S26] C：内存清零
来源：http://cw.colortex.cn

memset(a, 0, sizeof a);
来源：http://fx.panjiajie.cn

[S27] C：定义常量
来源：http://ov.nicolike.cn

const double PI = 3.14159;
来源：http://sr.szxytkj.cn

[S28] C：静态变量
来源：http://bv.bjjhwx.cn

static int counter = 0;
来源：http://pq.jctech888.com.cn

[S29] C：变参函数
来源：http://vm.colortex.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lq.szxytkj.cn

[S30] C：头文件保护
来源：http://dt.shxzukj.cn

#ifndef X_H
来源：http://fr.521024.cn

#define X_H
来源：http://si.haigaiapp.cn

#endif
来源：http://tn.jianghongdianzi.cn

[S31] C++：Hello World
来源：http://nk.haigaiapp.cn

#include <iostream>
来源：http://gm.shxzukj.cn

int main() { std::cout << "Hello\n"; }
来源：http://su.nszjky.cn

[S32] C++：字符串
来源：http://jp.gzmigu.cn

std::string s = "hi";  s += "!";
来源：http://pa.szxytkj.cn

[S33] C++：vector 增删
来源：http://oa.szxytkj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ee.szxytkj.cn

[S34] C++：遍历 vector
来源：http://fd.panjiajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://ud.521024.cn

[S35] C++：map
来源：http://nr.newstarts.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wm.colortex.cn

[S36] C++：unordered_map
来源：http://ft.newstarts.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ua.panjiajie.cn

[S37] C++：set
来源：http://vl.shxzskj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ub.lnxyls.cn

[S38] C++：排序
来源：http://kk.szsharing.cn

std::sort(v.begin(), v.end());
来源：http://fi.chemitech.net.cn

[S39] C++：自定义比较器排序
来源：http://ml.szxytkj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mm.huanxung.cn

[S40] C++：查找元素
来源：http://ng.9csxet.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fq.lnxyls.cn

[S41] C++：类与构造函数
来源：http://id.hnjuh.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://av.newstarts.cn

[S42] C++：继承与虚函数
来源：http://qs.haigaiapp.cn

class B : public Base { public: void f() override {} };
来源：http://hq.haigaiapp.cn

[S43] C++：智能指针
来源：http://eh.521024.cn

auto p = std::make_unique<int>(5);
来源：http://wp.muxihuayi.cn

[S44] C++：引用传参
来源：http://ta.shxzukj.cn

void inc(int &x) { ++x; }
来源：http://ea.shxzskj.cn

[S45] C++：lambda
来源：http://wd.jctech888.com.cn

auto add = [](int a, int b) { return a + b; };
来源：http://uh.muxihuayi.cn

[S46] C++：函数模板
来源：http://rj.szxytkj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fk.nszjky.cn

[S47] C++：结构化绑定遍历
来源：http://fu.asd995.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bb.bjjhwx.cn

[S48] C++：逐行读文件
来源：http://ow.bjjhwx.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ku.panjiajie.cn

while (std::getline(in, line)) { }
来源：http://hm.hnjuh.cn

[S49] C++：写文件
来源：http://yq.panjiajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vn.nszjky.cn

[S50] C++：格式化数字
来源：http://je.panjiajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ji.asd995.cn

[S51] C++：显式类型转换
来源：http://qg.9csxet.cn

static_cast<double>(a) / b
来源：http://ko.colortex.cn

[S52] C++：const 与 noexcept
来源：http://jc.newstarts.cn

int size() const noexcept { return n_; }
来源：http://jt.huanxung.cn

[S53] C++：移动语义
来源：http://ap.gzmigu.cn

std::vector<int> w = std::move(v);
来源：http://yn.bjjhwx.cn

[S54] C++：异常处理
来源：http://wx.szsharing.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://am.muxihuayi.cn

[S55] C++：结构化绑定
来源：http://xq.nszjky.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://yy.asd995.cn

[S56] C++：optional
来源：http://kw.muxihuayi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cf.muxihuayi.cn

[S57] C++：编译期常量
来源：http://fc.muxihuayi.cn

constexpr int N = 10;
来源：http://ic.yuexingan06.cn

[S58] C++：命名空间
来源：http://qw.hahajie.cn

namespace ns { int f() { return 1; } }
来源：http://zv.haigaiapp.cn

[S59] C++：静态断言
来源：http://fy.haigaiapp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://td.yuexingan06.cn

[S60] C++：遍历并删除元素
来源：http://qt.nszjky.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cf.wgjwhj.cn

================================================================================
来源：http://as.shxzukj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ng.shtwfgs.cn

================================================================================
来源：http://qi.gzmigu.cn

[T01] Kotlin：Hello World
来源：http://gp.nicolike.cn

println("Hello")
来源：http://bc.newstarts.cn

[T02] Kotlin：变量
来源：http://kf.bjjhwx.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://aw.9csxet.cn

[T03] Kotlin：字符串模板
来源：http://ow.bjjhwx.cn

"值: $b"
来源：http://at.szsharing.cn

[T04] Kotlin：空安全
来源：http://ss.lnxyls.cn

val n: String? = null;  n?.length
来源：http://ck.huixinmuqiang.cn

[T05] Kotlin：when 表达式
来源：http://mo.wgjwhj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hx.colortex.cn

[T06] Kotlin：集合映射
来源：http://ct.huanxung.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://du.yuntaijiaju.cn

[T07] Kotlin：集合过滤
来源：http://pi.nicolike.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ax.shxzukj.cn

[T08] Kotlin：数据类
来源：http://pj.hnjuh.cn

data class User(val name: String, val age: Int)
来源：http://lt.bookmarksfly.cn

[T09] Kotlin：扩展函数
来源：http://hj.huixiangedu.cn

fun String.exclaim() = this + "!"
来源：http://ms.jctech888.com.cn

[T10] Kotlin：默认参数
来源：http://xd.panjiajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://fk.hnjuh.cn

[T11] Kotlin：协程
来源：http://ha.yuexingan06.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://zt.hahajie.cn

[T12] Kotlin：解构声明
来源：http://xt.nszjky.cn

val (a, b) = Pair(1, 2)
来源：http://hk.nszjky.cn

[T13] Kotlin：只读 Map
来源：http://sy.panjiajie.cn

val m = mapOf("a" to 1)
来源：http://zl.szsharing.cn

[T14] Kotlin：循环
来源：http://wf.jianghongdianzi.cn

for (i in 1..10) println(i)
来源：http://jg.chemitech.net.cn

[T15] Kotlin：接口
来源：http://qi.nszjky.cn

interface Shape { fun area(): Double }
来源：http://mf.szxytkj.cn

[T16] Swift：Hello World
来源：http://ei.chemitech.net.cn

print("Hello")
来源：http://bg.bjjhwx.cn

[T17] Swift：变量与常量
来源：http://bc.szxytkj.cn

var a = 1;  let b = 2
来源：http://qn.hahajie.cn

[T18] Swift：字符串插值
来源：http://jp.huixiangedu.cn

"值: \(b)"
来源：http://mh.szsharing.cn

[T19] Swift：可选绑定
来源：http://ix.shxzukj.cn

if let n = opt { print(n) }
来源：http://at.huixiangedu.cn

[T20] Swift：数组操作
来源：http://sm.shxzukj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qm.lnxyls.cn

[T21] Swift：遍历
来源：http://od.9csxet.cn

for x in a { print(x) }
来源：http://oh.9csxet.cn

[T22] Swift：字典
来源：http://oy.haigaiapp.cn

var d = ["a": 1];  d["b"] = 2
来源：http://yp.chemitech.net.cn

[T23] Swift：函数
来源：http://gm.panjiajie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hf.chemitech.net.cn

[T24] Swift：闭包
来源：http://nx.chemitech.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://tx.gzmigu.cn

[T25] Swift：结构体
来源：http://cq.yuexingan06.cn

struct P { var x: Int }
来源：http://kj.panjiajie.cn

[T26] Swift：类与重写
来源：http://bf.yuexingan06.cn

class A: Base { override func f() {} }
来源：http://vp.szsharing.cn

[T27] Swift：错误处理
来源：http://to.haigaiapp.cn

do { try f() } catch { print(error) }
来源：http://vq.huixinmuqiang.cn

[T28] Swift：枚举
来源：http://xg.panjiajie.cn

enum Color { case red, green }
来源：http://ya.hnjuh.cn

[T29] Swift：guard 提前返回
来源：http://ew.yuntaijiaju.cn

guard let x = opt else { return }
来源：http://fj.shxzskj.cn

[T30] Swift：协议
来源：http://ei.lnxyls.cn

protocol Shape { func area() -> Double }
来源：http://qc.hahajie.cn

[T31] Lua：Hello World
来源：http://fq.huixinmuqiang.cn

print("Hello")
来源：http://kw.shxzskj.cn

[T32] Lua：局部变量
来源：http://sy.shtwfgs.cn

local a = 1
来源：http://pp.newstarts.cn

[T33] Lua：表（数组）
来源：http://ti.panjiajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://yf.shxzukj.cn

[T34] Lua：遍历表
来源：http://vb.521024.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://iq.521024.cn

[T35] Lua：字典表
来源：http://ld.9csxet.cn

local d = { a = 1 };  d.b = 2
来源：http://cb.jctech888.com.cn

[T36] Lua：函数
来源：http://zq.shxzukj.cn

function add(a, b) return a + b end
来源：http://jb.hnjuh.cn

[T37] Lua：字符串拼接
来源：http://ue.bookmarksfly.cn

"a" .. "b"
来源：http://gc.huanxung.cn

[T38] Lua：条件
来源：http://xx.shtwfgs.cn

if x > 0 then print("正") end
来源：http://vf.9csxet.cn

[T39] Lua：模式匹配
来源：http://iz.gzmigu.cn

string.find(s, "%d+")
来源：http://ia.yuntaijiaju.cn

[T40] Lua：元表
来源：http://gi.521024.cn

setmetatable({}, { __index = base })
来源：http://lr.shxzskj.cn

[T41] Perl：Hello World
来源：http://ij.shtwfgs.cn

print "Hello\n";
来源：http://pv.huixiangedu.cn

[T42] Perl：变量类型
来源：http://ly.muxihuayi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mt.huixinmuqiang.cn

[T43] Perl：字符串插值
来源：http://zt.hnjuh.cn

"值: $a"
来源：http://yx.521024.cn

[T44] Perl：条件
来源：http://et.shxzskj.cn

if ($a > 0) { print "正"; }
来源：http://ul.jctech888.com.cn

[T45] Perl：数组遍历
来源：http://yw.huixiangedu.cn

for my $x (@arr) { print $x; }
来源：http://ml.bookmarksfly.cn

[T46] Perl：哈希操作
来源：http://mt.huixiangedu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wj.shtwfgs.cn

[T47] Perl：正则捕获
来源：http://px.yuntaijiaju.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://hp.hnjuh.cn

[T48] Perl：正则替换
来源：http://cw.huanxung.cn

$s =~ s/old/new/g;
来源：http://us.jianghongdianzi.cn

[T49] Perl：函数
来源：http://hd.wgjwhj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dc.nicolike.cn

[T50] Perl：逐行读文件
来源：http://nu.panjiajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ky.asd995.cn

while (my $line = <$fh>) { print $line; }
来源：http://vy.newstarts.cn

[T51] Scala：Hello World
来源：http://sk.huixinmuqiang.cn

println("Hello")
来源：http://xb.huixinmuqiang.cn

[T52] Scala：变量
来源：http://ti.jianghongdianzi.cn

val a = 1;  var b = 2
来源：http://ae.shxzukj.cn

[T53] Scala：字符串插值
来源：http://aw.panjiajie.cn

s"值: $b"
来源：http://yd.bookmarksfly.cn

[T54] Scala：集合映射
来源：http://iw.szsharing.cn

List(1, 2, 3).map(_ * 2)
来源：http://xx.muxihuayi.cn

[T55] Scala：集合过滤
来源：http://ij.shxzskj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://va.bjjhwx.cn

[T56] Scala：样例类
来源：http://my.shxzskj.cn

case class User(name: String, age: Int)
来源：http://jj.panjiajie.cn

[T57] Scala：模式匹配
来源：http://eb.szxytkj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ep.huanxung.cn

[T58] Scala：函数定义
来源：http://vx.huixiangedu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://cn.huanxung.cn

[T59] Scala：循环
来源：http://bo.bookmarksfly.cn

for (i <- 1 to 10) println(i)
来源：http://at.jianghongdianzi.cn

[T60] Scala：折叠
来源：http://qk.yuntaijiaju.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qm.newstarts.cn

================================================================================
来源：http://di.huanxung.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bs.asd995.cn

================================================================================
来源：http://uw.521024.cn

[U01] Py：创建虚拟环境
来源：http://tk.shxzukj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://pe.nicolike.cn

[U02] Py：导出 / 安装依赖
来源：http://cd.wgjwhj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dz.shxzskj.cn

[U03] Py：加载 .env 配置
来源：http://po.panjiajie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://hy.asd995.cn

[U04] Py：变量调试打印
来源：http://yn.wgjwhj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cy.521024.cn

[U05] Py：列表去重且保序
来源：http://nq.bjjhwx.cn

list(dict.fromkeys(arr))
来源：http://qw.jianghongdianzi.cn

[U06] Py：合并两个字典
来源：http://ym.colortex.cn

{**a, **b}
来源：http://iq.lnxyls.cn

[U07] Py：反转字典键值
来源：http://hf.szxytkj.cn

{v: k for k, v in d.items()}
来源：http://vb.wgjwhj.cn

[U08] Py：展平二维列表
来源：http://gy.colortex.cn

[y for x in nested for y in x]
来源：http://ku.lnxyls.cn

[U09] Py：字典取最大值的键
来源：http://pl.huanxung.cn

max(d, key=d.get)
来源：http://st.huixiangedu.cn

[U10] Py：按值排序字典
来源：http://cu.huanxung.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wt.bookmarksfly.cn

[U11] Py：生成器表达式
来源：http://ts.bookmarksfly.cn

(x * 2 for x in arr)
来源：http://qc.shxzukj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://pn.shxzskj.cn

Counter(arr).most_common(3)
来源：http://eb.szxytkj.cn

[U13] Py：固定长度队列
来源：http://ho.colortex.cn

deque(maxlen=10)
来源：http://kn.bookmarksfly.cn

[U14] Py：分组收集到列表
来源：http://jx.hnjuh.cn

defaultdict(list)
来源：http://kk.huanxung.cn

[U15] Py：高精度计时
来源：http://yj.wgjwhj.cn

t = time.perf_counter()
来源：http://nd.gzmigu.cn

[U16] Py：命令行参数解析
来源：http://xc.hnjuh.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ew.shxzskj.cn

[U17] Py：初始化日志
来源：http://av.chemitech.net.cn

logging.basicConfig(level=logging.INFO)
来源：http://pr.newstarts.cn

[U18] Py：预编译正则
来源：http://mb.szxytkj.cn

pat = re.compile(r"\d+")
来源：http://ev.nicolike.cn

[U19] Py：正则替换带回调
来源：http://ua.shxzskj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zm.wgjwhj.cn

[U20] Py：缓存函数结果
来源：http://em.bjjhwx.cn

@functools.lru_cache(maxsize=None)
来源：http://nt.shxzskj.cn

[U21] Py：自定义上下文管理器
来源：http://we.chemitech.net.cn

@contextlib.contextmanager
来源：http://wk.nszjky.cn

[U22] Py：矩阵转置
来源：http://rs.wgjwhj.cn

list(zip(*m))
来源：http://mg.jianghongdianzi.cn

[U23] Py：分块读取大文件
来源：http://zo.chemitech.net.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rs.bjjhwx.cn

[U24] Py：路径操作
来源：http://zr.wgjwhj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.lnxyls.cn

[U25] Py：CSV 按字典读
来源：http://nm.haigaiapp.cn

csv.DictReader(f)
来源：http://hj.hnjuh.cn

[U26] Py：并发下载
来源：http://pb.chemitech.net.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vs.nicolike.cn

[U27] Py：异步 HTTP
来源：http://mr.jianghongdianzi.cn

aiohttp.ClientSession() 配合 async with
来源：http://pw.yuexingan06.cn

[U28] Py：类型别名
来源：http://mm.jctech888.com.cn

UserId = int
来源：http://oy.9csxet.cn

[U29] Py：属性校验
来源：http://cb.panjiajie.cn

@property 与 @x.setter 配合
来源：http://qx.nicolike.cn

[U30] Py：数据类
来源：http://dy.bookmarksfly.cn

@dataclass(slots=True)
来源：http://tl.bjjhwx.cn

[U31] Py：单测
来源：http://xf.jctech888.com.cn

python -m pytest -q
来源：http://nh.lnxyls.cn

[U32] Py：代码格式化
来源：http://vt.shxzskj.cn

ruff format . && ruff check --fix .
来源：http://zh.huanxung.cn

[U33] Py：打包发布
来源：http://pn.9csxet.cn

python -m build  （依赖 pyproject.toml）
来源：http://dt.nicolike.cn

[U34] Py：判断编码
来源：http://wh.szsharing.cn

chardet.detect(raw)
来源：http://vp.hnjuh.cn

[U35] Py：发送邮件
来源：http://kg.bookmarksfly.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lk.shxzskj.cn

[U36] Py：定时任务
来源：http://sf.hahajie.cn

schedule.every(10).minutes.do(job)
来源：http://es.521024.cn

[U37] Py：读写 Excel
来源：http://yh.yuntaijiaju.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ci.shxzskj.cn

[U38] Py：获取脚本所在目录
来源：http://fz.yuexingan06.cn

Path(__file__).resolve().parent
来源：http://vw.521024.cn


<!-- 参考信息 -->