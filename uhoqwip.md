代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jp.bookmarksfly.cn

[S13] C：宏定义
来源：http://kt.haigaiapp.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sh.gzmigu.cn

[S14] C：枚举
来源：http://my.jctech888.com.cn

enum Color { RED, GREEN, BLUE };
来源：http://gj.szxytkj.cn

[S15] C：类型转换
来源：http://tv.shxzskj.cn

(double) a / b
来源：http://uu.hnjuh.cn

[S16] C：位操作置位
来源：http://nj.shtwfgs.cn

x |= (1 << 3);
来源：http://hc.chemitech.net.cn

[S17] C：安全拼接字符串
来源：http://ba.colortex.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wv.newstarts.cn

[S18] C：命令行参数
来源：http://no.yuntaijiaju.cn

int main(int argc, char **argv)
来源：http://gy.yuntaijiaju.cn

[S19] C：快速排序
来源：http://tc.shxzskj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://pv.gzmigu.cn

[S20] C：二分查找
来源：http://mj.colortex.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vt.huixinmuqiang.cn

[S21] C：字符类别判断
来源：http://gz.huanxung.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wt.szxytkj.cn

[S22] C：字符串转数字
来源：http://pu.shxzskj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vl.shtwfgs.cn

[S23] C：随机数
来源：http://ip.hnjuh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://sh.huanxung.cn

[S24] C：获取本地时间
来源：http://pf.haigaiapp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nk.szxytkj.cn

[S25] C：内存拷贝
来源：http://eo.szxytkj.cn

memcpy(dst, src, n);
来源：http://xj.szsharing.cn

[S26] C：内存清零
来源：http://al.panjiajie.cn

memset(a, 0, sizeof a);
来源：http://jk.szxytkj.cn

[S27] C：定义常量
来源：http://th.yuexingan06.cn

const double PI = 3.14159;
来源：http://rx.hahajie.cn

[S28] C：静态变量
来源：http://bl.wgjwhj.cn

static int counter = 0;
来源：http://su.jctech888.com.cn

[S29] C：变参函数
来源：http://xo.shtwfgs.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cp.yuexingan06.cn

[S30] C：头文件保护
来源：http://rn.hahajie.cn

#ifndef X_H
来源：http://hx.nszjky.cn

#define X_H
来源：http://vg.haigaiapp.cn

#endif
来源：http://co.shxzskj.cn

[S31] C++：Hello World
来源：http://xe.bjjhwx.cn

#include <iostream>
来源：http://hc.wgjwhj.cn

int main() { std::cout << "Hello\n"; }
来源：http://yu.9csxet.cn

[S32] C++：字符串
来源：http://sd.huixinmuqiang.cn

std::string s = "hi";  s += "!";
来源：http://sq.huanxung.cn

[S33] C++：vector 增删
来源：http://in.bookmarksfly.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sr.jctech888.com.cn

[S34] C++：遍历 vector
来源：http://xj.bookmarksfly.cn

for (auto &x : v) { std::cout << x; }
来源：http://rf.nszjky.cn

[S35] C++：map
来源：http://eq.newstarts.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zw.haigaiapp.cn

[S36] C++：unordered_map
来源：http://rm.asd995.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jk.yuntaijiaju.cn

[S37] C++：set
来源：http://ax.lnxyls.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ce.hahajie.cn

[S38] C++：排序
来源：http://gm.chemitech.net.cn

std::sort(v.begin(), v.end());
来源：http://bv.bookmarksfly.cn

[S39] C++：自定义比较器排序
来源：http://vf.szsharing.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jr.muxihuayi.cn

[S40] C++：查找元素
来源：http://kw.wgjwhj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rd.szxytkj.cn

[S41] C++：类与构造函数
来源：http://zd.nszjky.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sw.hnjuh.cn

[S42] C++：继承与虚函数
来源：http://hm.yuntaijiaju.cn

class B : public Base { public: void f() override {} };
来源：http://lb.jctech888.com.cn

[S43] C++：智能指针
来源：http://so.haigaiapp.cn

auto p = std::make_unique<int>(5);
来源：http://ul.hnjuh.cn

[S44] C++：引用传参
来源：http://de.panjiajie.cn

void inc(int &x) { ++x; }
来源：http://cq.shtwfgs.cn

[S45] C++：lambda
来源：http://da.jianghongdianzi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ti.panjiajie.cn

[S46] C++：函数模板
来源：http://ch.wgjwhj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://le.wgjwhj.cn

[S47] C++：结构化绑定遍历
来源：http://ec.shtwfgs.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vb.haigaiapp.cn

[S48] C++：逐行读文件
来源：http://hn.lnxyls.cn

std::ifstream in("a.txt");  std::string line;
来源：http://yd.bookmarksfly.cn

while (std::getline(in, line)) { }
来源：http://lg.szxytkj.cn

[S49] C++：写文件
来源：http://tu.bookmarksfly.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jf.9csxet.cn

[S50] C++：格式化数字
来源：http://ed.gzmigu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pq.lnxyls.cn

[S51] C++：显式类型转换
来源：http://ar.szxytkj.cn

static_cast<double>(a) / b
来源：http://vy.shxzskj.cn

[S52] C++：const 与 noexcept
来源：http://cg.yuntaijiaju.cn

int size() const noexcept { return n_; }
来源：http://qt.wgjwhj.cn

[S53] C++：移动语义
来源：http://as.shtwfgs.cn

std::vector<int> w = std::move(v);
来源：http://vj.bookmarksfly.cn

[S54] C++：异常处理
来源：http://of.haigaiapp.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://na.shxzukj.cn

[S55] C++：结构化绑定
来源：http://ek.panjiajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ya.jianghongdianzi.cn

[S56] C++：optional
来源：http://pa.bookmarksfly.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ty.nicolike.cn

[S57] C++：编译期常量
来源：http://un.nicolike.cn

constexpr int N = 10;
来源：http://bn.szsharing.cn

[S58] C++：命名空间
来源：http://wx.shxzukj.cn

namespace ns { int f() { return 1; } }
来源：http://vk.shxzskj.cn

[S59] C++：静态断言
来源：http://zl.szxytkj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zd.huixiangedu.cn

[S60] C++：遍历并删除元素
来源：http://op.shxzukj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fj.jctech888.com.cn

================================================================================
来源：http://ps.szxytkj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bu.hahajie.cn

================================================================================
来源：http://ui.521024.cn

[T01] Kotlin：Hello World
来源：http://ee.9csxet.cn

println("Hello")
来源：http://ho.nszjky.cn

[T02] Kotlin：变量
来源：http://fy.haigaiapp.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://se.huixiangedu.cn

[T03] Kotlin：字符串模板
来源：http://ku.chemitech.net.cn

"值: $b"
来源：http://el.nszjky.cn

[T04] Kotlin：空安全
来源：http://bk.bjjhwx.cn

val n: String? = null;  n?.length
来源：http://ge.panjiajie.cn

[T05] Kotlin：when 表达式
来源：http://vv.huanxung.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yx.wgjwhj.cn

[T06] Kotlin：集合映射
来源：http://ju.szsharing.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://jm.shxzskj.cn

[T07] Kotlin：集合过滤
来源：http://vv.nicolike.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ps.huixinmuqiang.cn

[T08] Kotlin：数据类
来源：http://ad.szsharing.cn

data class User(val name: String, val age: Int)
来源：http://la.jianghongdianzi.cn

[T09] Kotlin：扩展函数
来源：http://jo.bjjhwx.cn

fun String.exclaim() = this + "!"
来源：http://xy.hahajie.cn

[T10] Kotlin：默认参数
来源：http://tx.asd995.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://af.shtwfgs.cn

[T11] Kotlin：协程
来源：http://kx.gzmigu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ar.9csxet.cn

[T12] Kotlin：解构声明
来源：http://zd.szxytkj.cn

val (a, b) = Pair(1, 2)
来源：http://um.asd995.cn

[T13] Kotlin：只读 Map
来源：http://jz.gzmigu.cn

val m = mapOf("a" to 1)
来源：http://yl.asd995.cn

[T14] Kotlin：循环
来源：http://nf.huixinmuqiang.cn

for (i in 1..10) println(i)
来源：http://fx.yuntaijiaju.cn

[T15] Kotlin：接口
来源：http://za.nszjky.cn

interface Shape { fun area(): Double }
来源：http://up.hahajie.cn

[T16] Swift：Hello World
来源：http://iw.szsharing.cn

print("Hello")
来源：http://pf.hnjuh.cn

[T17] Swift：变量与常量
来源：http://yf.gzmigu.cn

var a = 1;  let b = 2
来源：http://kt.jctech888.com.cn

[T18] Swift：字符串插值
来源：http://vo.hahajie.cn

"值: \(b)"
来源：http://jr.shxzskj.cn

[T19] Swift：可选绑定
来源：http://ed.asd995.cn

if let n = opt { print(n) }
来源：http://kr.gzmigu.cn

[T20] Swift：数组操作
来源：http://ll.hahajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://pb.gzmigu.cn

[T21] Swift：遍历
来源：http://km.hahajie.cn

for x in a { print(x) }
来源：http://jw.shxzukj.cn

[T22] Swift：字典
来源：http://hj.jctech888.com.cn

var d = ["a": 1];  d["b"] = 2
来源：http://yo.bjjhwx.cn

[T23] Swift：函数
来源：http://cy.jctech888.com.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ii.jianghongdianzi.cn

[T24] Swift：闭包
来源：http://tr.shtwfgs.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://km.szxytkj.cn

[T25] Swift：结构体
来源：http://qm.huanxung.cn

struct P { var x: Int }
来源：http://em.colortex.cn

[T26] Swift：类与重写
来源：http://cj.shxzukj.cn

class A: Base { override func f() {} }
来源：http://gb.shtwfgs.cn

[T27] Swift：错误处理
来源：http://ce.nicolike.cn

do { try f() } catch { print(error) }
来源：http://nf.huanxung.cn

[T28] Swift：枚举
来源：http://kp.bookmarksfly.cn

enum Color { case red, green }
来源：http://ed.colortex.cn

[T29] Swift：guard 提前返回
来源：http://zm.szsharing.cn

guard let x = opt else { return }
来源：http://ep.wgjwhj.cn

[T30] Swift：协议
来源：http://us.huixiangedu.cn

protocol Shape { func area() -> Double }
来源：http://xn.hahajie.cn

[T31] Lua：Hello World
来源：http://ku.wgjwhj.cn

print("Hello")
来源：http://by.shxzskj.cn

[T32] Lua：局部变量
来源：http://kz.gzmigu.cn

local a = 1
来源：http://wl.colortex.cn

[T33] Lua：表（数组）
来源：http://ia.szxytkj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://gv.hnjuh.cn

[T34] Lua：遍历表
来源：http://bq.9csxet.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://hv.huanxung.cn

[T35] Lua：字典表
来源：http://bj.hnjuh.cn

local d = { a = 1 };  d.b = 2
来源：http://za.colortex.cn

[T36] Lua：函数
来源：http://rw.yuexingan06.cn

function add(a, b) return a + b end
来源：http://vm.hnjuh.cn

[T37] Lua：字符串拼接
来源：http://ey.yuntaijiaju.cn

"a" .. "b"
来源：http://pw.bjjhwx.cn

[T38] Lua：条件
来源：http://lm.shtwfgs.cn

if x > 0 then print("正") end
来源：http://wg.jctech888.com.cn

[T39] Lua：模式匹配
来源：http://hl.newstarts.cn

string.find(s, "%d+")
来源：http://iw.shxzukj.cn

[T40] Lua：元表
来源：http://vc.lnxyls.cn

setmetatable({}, { __index = base })
来源：http://aq.haigaiapp.cn

[T41] Perl：Hello World
来源：http://jr.bjjhwx.cn

print "Hello\n";
来源：http://zm.shxzskj.cn

[T42] Perl：变量类型
来源：http://mj.chemitech.net.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gz.hahajie.cn

[T43] Perl：字符串插值
来源：http://ms.colortex.cn

"值: $a"
来源：http://gv.yuntaijiaju.cn

[T44] Perl：条件
来源：http://lp.newstarts.cn

if ($a > 0) { print "正"; }
来源：http://np.huixiangedu.cn

[T45] Perl：数组遍历
来源：http://cx.jianghongdianzi.cn

for my $x (@arr) { print $x; }
来源：http://mr.yuexingan06.cn

[T46] Perl：哈希操作
来源：http://me.asd995.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uj.huixinmuqiang.cn

[T47] Perl：正则捕获
来源：http://rp.nszjky.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://eo.bjjhwx.cn

[T48] Perl：正则替换
来源：http://zj.jctech888.com.cn

$s =~ s/old/new/g;
来源：http://ce.muxihuayi.cn

[T49] Perl：函数
来源：http://dy.haigaiapp.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bn.huixiangedu.cn

[T50] Perl：逐行读文件
来源：http://lh.jianghongdianzi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://cp.haigaiapp.cn

while (my $line = <$fh>) { print $line; }
来源：http://gl.haigaiapp.cn

[T51] Scala：Hello World
来源：http://dq.lnxyls.cn

println("Hello")
来源：http://td.9csxet.cn

[T52] Scala：变量
来源：http://bf.szxytkj.cn

val a = 1;  var b = 2
来源：http://ys.nszjky.cn

[T53] Scala：字符串插值
来源：http://xo.hahajie.cn

s"值: $b"
来源：http://wk.szxytkj.cn

[T54] Scala：集合映射
来源：http://gf.newstarts.cn

List(1, 2, 3).map(_ * 2)
来源：http://yh.huanxung.cn

[T55] Scala：集合过滤
来源：http://tt.nszjky.cn

List(1, 2, 3).filter(_ > 1)
来源：http://th.szsharing.cn

[T56] Scala：样例类
来源：http://fj.bookmarksfly.cn

case class User(name: String, age: Int)
来源：http://du.nszjky.cn

[T57] Scala：模式匹配
来源：http://ui.szsharing.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://en.hnjuh.cn

[T58] Scala：函数定义
来源：http://jq.asd995.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ub.bjjhwx.cn

[T59] Scala：循环
来源：http://uk.9csxet.cn

for (i <- 1 to 10) println(i)
来源：http://wr.muxihuayi.cn

[T60] Scala：折叠
来源：http://nf.hnjuh.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xv.lnxyls.cn

================================================================================
来源：http://xm.asd995.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://px.chemitech.net.cn

================================================================================
来源：http://jp.gzmigu.cn

[U01] Py：创建虚拟环境
来源：http://rr.haigaiapp.cn

python -m venv .venv && source .venv/bin/activate
来源：http://xa.jctech888.com.cn

[U02] Py：导出 / 安装依赖
来源：http://xj.shtwfgs.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zu.yuexingan06.cn

[U03] Py：加载 .env 配置
来源：http://xa.nicolike.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://oa.yuexingan06.cn

[U04] Py：变量调试打印
来源：http://lj.shxzskj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ww.nicolike.cn

[U05] Py：列表去重且保序
来源：http://zq.jctech888.com.cn

list(dict.fromkeys(arr))
来源：http://aa.nicolike.cn

[U06] Py：合并两个字典
来源：http://id.huixiangedu.cn

{**a, **b}
来源：http://hm.muxihuayi.cn

[U07] Py：反转字典键值
来源：http://wz.9csxet.cn

{v: k for k, v in d.items()}
来源：http://yw.huixiangedu.cn

[U08] Py：展平二维列表
来源：http://ns.nicolike.cn

[y for x in nested for y in x]
来源：http://ko.shxzukj.cn

[U09] Py：字典取最大值的键
来源：http://gb.chemitech.net.cn

max(d, key=d.get)
来源：http://kl.jctech888.com.cn

[U10] Py：按值排序字典
来源：http://ym.yuexingan06.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uu.wgjwhj.cn

[U11] Py：生成器表达式
来源：http://xf.haigaiapp.cn

(x * 2 for x in arr)
来源：http://dk.colortex.cn

[U12] Py：取出现最多的 3 个元素
来源：http://dn.colortex.cn

Counter(arr).most_common(3)
来源：http://di.yuntaijiaju.cn

[U13] Py：固定长度队列
来源：http://ha.hahajie.cn

deque(maxlen=10)
来源：http://eo.szxytkj.cn

[U14] Py：分组收集到列表
来源：http://ym.colortex.cn

defaultdict(list)
来源：http://ax.shtwfgs.cn

[U15] Py：高精度计时
来源：http://tm.yuexingan06.cn

t = time.perf_counter()
来源：http://nj.nicolike.cn

[U16] Py：命令行参数解析
来源：http://cj.szsharing.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qh.521024.cn

[U17] Py：初始化日志
来源：http://az.haigaiapp.cn

logging.basicConfig(level=logging.INFO)
来源：http://np.asd995.cn

[U18] Py：预编译正则
来源：http://he.jianghongdianzi.cn

pat = re.compile(r"\d+")
来源：http://kp.shxzskj.cn

[U19] Py：正则替换带回调
来源：http://ct.shxzskj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://im.hnjuh.cn

[U20] Py：缓存函数结果
来源：http://np.shtwfgs.cn

@functools.lru_cache(maxsize=None)
来源：http://pe.nszjky.cn

[U21] Py：自定义上下文管理器
来源：http://md.szsharing.cn

@contextlib.contextmanager
来源：http://zc.colortex.cn

[U22] Py：矩阵转置
来源：http://pa.shtwfgs.cn

list(zip(*m))
来源：http://ap.colortex.cn

[U23] Py：分块读取大文件
来源：http://ht.yuntaijiaju.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://aj.nszjky.cn

[U24] Py：路径操作
来源：http://hy.yuexingan06.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ws.newstarts.cn

[U25] Py：CSV 按字典读
来源：http://qi.hahajie.cn

csv.DictReader(f)
来源：http://eg.hnjuh.cn

[U26] Py：并发下载
来源：http://ud.szxytkj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gq.haigaiapp.cn

[U27] Py：异步 HTTP
来源：http://gx.shtwfgs.cn

aiohttp.ClientSession() 配合 async with
来源：http://lk.newstarts.cn

[U28] Py：类型别名
来源：http://hl.bookmarksfly.cn

UserId = int
来源：http://zc.newstarts.cn

[U29] Py：属性校验
来源：http://pw.muxihuayi.cn

@property 与 @x.setter 配合
来源：http://dn.huanxung.cn

[U30] Py：数据类
来源：http://ux.muxihuayi.cn

@dataclass(slots=True)
来源：http://gn.bookmarksfly.cn

[U31] Py：单测
来源：http://jo.szsharing.cn

python -m pytest -q
来源：http://zt.jianghongdianzi.cn

[U32] Py：代码格式化
来源：http://oe.jianghongdianzi.cn

ruff format . && ruff check --fix .
来源：http://tg.asd995.cn

[U33] Py：打包发布
来源：http://zv.nicolike.cn

python -m build  （依赖 pyproject.toml）
来源：http://op.huixiangedu.cn

[U34] Py：判断编码
来源：http://dl.hnjuh.cn

chardet.detect(raw)
来源：http://hu.yuntaijiaju.cn

[U35] Py：发送邮件
来源：http://tv.shtwfgs.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://aj.haigaiapp.cn

[U36] Py：定时任务
来源：http://rg.shxzukj.cn

schedule.every(10).minutes.do(job)
来源：http://lf.hahajie.cn


<!-- 参考信息 -->