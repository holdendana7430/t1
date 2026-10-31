代发 wailian999

strlen(s)
来源：http://sd.9csxet.cn

[S06] C：字符串比较
来源：http://rk.wgjwhj.cn

strcmp(a, b) == 0
来源：http://eu.nszjky.cn

[S07] C：数组遍历求和
来源：http://bw.yuntaijiaju.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ka.huixiangedu.cn

[S08] C：动态内存分配与释放
来源：http://xm.huixiangedu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vj.wgjwhj.cn

[S09] C：结构体定义与初始化
来源：http://hq.nszjky.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gk.shxzukj.cn

[S10] C：指针与解引用
来源：http://ra.huixinmuqiang.cn

int *p = &a;  *p = 5;
来源：http://wn.huixiangedu.cn

[S11] C：逐行读文件
来源：http://pw.bjjhwx.cn

FILE *f = fopen("a.txt", "r");
来源：http://as.huixiangedu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wo.szsharing.cn

fclose(f);
来源：http://lh.muxihuayi.cn

[S12] C：写文件
来源：http://er.lnxyls.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zw.521024.cn

[S13] C：宏定义
来源：http://vs.asd995.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ku.lnxyls.cn

[S14] C：枚举
来源：http://yu.haigaiapp.cn

enum Color { RED, GREEN, BLUE };
来源：http://dp.lnxyls.cn

[S15] C：类型转换
来源：http://ub.jctech888.com.cn

(double) a / b
来源：http://td.huixiangedu.cn

[S16] C：位操作置位
来源：http://em.wgjwhj.cn

x |= (1 << 3);
来源：http://sz.hahajie.cn

[S17] C：安全拼接字符串
来源：http://pn.bookmarksfly.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ze.bookmarksfly.cn

[S18] C：命令行参数
来源：http://gl.haigaiapp.cn

int main(int argc, char **argv)
来源：http://cp.huixiangedu.cn

[S19] C：快速排序
来源：http://bu.bookmarksfly.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zz.bookmarksfly.cn

[S20] C：二分查找
来源：http://th.hnjuh.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ks.newstarts.cn

[S21] C：字符类别判断
来源：http://sx.huixinmuqiang.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vn.bookmarksfly.cn

[S22] C：字符串转数字
来源：http://cp.jctech888.com.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ho.newstarts.cn

[S23] C：随机数
来源：http://ee.colortex.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://lj.shtwfgs.cn

[S24] C：获取本地时间
来源：http://wj.bjjhwx.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hb.chemitech.net.cn

[S25] C：内存拷贝
来源：http://kp.521024.cn

memcpy(dst, src, n);
来源：http://ch.gzmigu.cn

[S26] C：内存清零
来源：http://pr.lnxyls.cn

memset(a, 0, sizeof a);
来源：http://ww.jctech888.com.cn

[S27] C：定义常量
来源：http://rc.szxytkj.cn

const double PI = 3.14159;
来源：http://no.521024.cn

[S28] C：静态变量
来源：http://mn.haigaiapp.cn

static int counter = 0;
来源：http://ys.szxytkj.cn

[S29] C：变参函数
来源：http://ut.jctech888.com.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sc.bookmarksfly.cn

[S30] C：头文件保护
来源：http://ko.huanxung.cn

#ifndef X_H
来源：http://se.asd995.cn

#define X_H
来源：http://yv.lnxyls.cn

#endif
来源：http://kp.huanxung.cn

[S31] C++：Hello World
来源：http://qj.szsharing.cn

#include <iostream>
来源：http://fd.nicolike.cn

int main() { std::cout << "Hello\n"; }
来源：http://cf.lnxyls.cn

[S32] C++：字符串
来源：http://qo.gzmigu.cn

std::string s = "hi";  s += "!";
来源：http://th.lnxyls.cn

[S33] C++：vector 增删
来源：http://ik.bjjhwx.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wp.9csxet.cn

[S34] C++：遍历 vector
来源：http://pj.shxzukj.cn

for (auto &x : v) { std::cout << x; }
来源：http://zz.huixinmuqiang.cn

[S35] C++：map
来源：http://rj.panjiajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ts.shxzukj.cn

[S36] C++：unordered_map
来源：http://lu.huixiangedu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wh.9csxet.cn

[S37] C++：set
来源：http://bp.szxytkj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vx.muxihuayi.cn

[S38] C++：排序
来源：http://kg.muxihuayi.cn

std::sort(v.begin(), v.end());
来源：http://zv.panjiajie.cn

[S39] C++：自定义比较器排序
来源：http://ae.nszjky.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bp.wgjwhj.cn

[S40] C++：查找元素
来源：http://gt.shxzukj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xb.jctech888.com.cn

[S41] C++：类与构造函数
来源：http://ot.newstarts.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sb.newstarts.cn

[S42] C++：继承与虚函数
来源：http://xk.asd995.cn

class B : public Base { public: void f() override {} };
来源：http://lw.panjiajie.cn

[S43] C++：智能指针
来源：http://ak.bookmarksfly.cn

auto p = std::make_unique<int>(5);
来源：http://ee.szxytkj.cn

[S44] C++：引用传参
来源：http://me.haigaiapp.cn

void inc(int &x) { ++x; }
来源：http://dw.shtwfgs.cn

[S45] C++：lambda
来源：http://kv.huixinmuqiang.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vg.muxihuayi.cn

[S46] C++：函数模板
来源：http://rp.lnxyls.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://er.haigaiapp.cn

[S47] C++：结构化绑定遍历
来源：http://hk.yuntaijiaju.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lq.szxytkj.cn

[S48] C++：逐行读文件
来源：http://sv.chemitech.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jx.shtwfgs.cn

while (std::getline(in, line)) { }
来源：http://kd.521024.cn

[S49] C++：写文件
来源：http://se.9csxet.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://io.haigaiapp.cn

[S50] C++：格式化数字
来源：http://kh.szsharing.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lx.muxihuayi.cn

[S51] C++：显式类型转换
来源：http://op.colortex.cn

static_cast<double>(a) / b
来源：http://wf.hnjuh.cn

[S52] C++：const 与 noexcept
来源：http://ha.huixiangedu.cn

int size() const noexcept { return n_; }
来源：http://jc.bookmarksfly.cn

[S53] C++：移动语义
来源：http://ll.muxihuayi.cn

std::vector<int> w = std::move(v);
来源：http://tj.muxihuayi.cn

[S54] C++：异常处理
来源：http://jt.shxzukj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cm.haigaiapp.cn

[S55] C++：结构化绑定
来源：http://dn.shxzskj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gj.yuexingan06.cn

[S56] C++：optional
来源：http://zf.yuntaijiaju.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vs.newstarts.cn

[S57] C++：编译期常量
来源：http://jx.shxzskj.cn

constexpr int N = 10;
来源：http://wx.nszjky.cn

[S58] C++：命名空间
来源：http://sd.colortex.cn

namespace ns { int f() { return 1; } }
来源：http://uk.haigaiapp.cn

[S59] C++：静态断言
来源：http://jw.521024.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ak.szsharing.cn

[S60] C++：遍历并删除元素
来源：http://pt.haigaiapp.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dl.bjjhwx.cn

================================================================================
来源：http://yf.huanxung.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fl.asd995.cn

================================================================================
来源：http://dz.jctech888.com.cn

[T01] Kotlin：Hello World
来源：http://xo.yuexingan06.cn

println("Hello")
来源：http://qo.bjjhwx.cn

[T02] Kotlin：变量
来源：http://lh.szsharing.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mw.lnxyls.cn

[T03] Kotlin：字符串模板
来源：http://vy.nicolike.cn

"值: $b"
来源：http://xy.bookmarksfly.cn

[T04] Kotlin：空安全
来源：http://fw.yuntaijiaju.cn

val n: String? = null;  n?.length
来源：http://ew.huixiangedu.cn

[T05] Kotlin：when 表达式
来源：http://vs.colortex.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jl.yuexingan06.cn

[T06] Kotlin：集合映射
来源：http://kd.chemitech.net.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ma.9csxet.cn

[T07] Kotlin：集合过滤
来源：http://wg.huixiangedu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://go.bookmarksfly.cn

[T08] Kotlin：数据类
来源：http://ua.nicolike.cn

data class User(val name: String, val age: Int)
来源：http://xc.szxytkj.cn

[T09] Kotlin：扩展函数
来源：http://yq.jctech888.com.cn

fun String.exclaim() = this + "!"
来源：http://sw.haigaiapp.cn

[T10] Kotlin：默认参数
来源：http://mm.huanxung.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://bo.521024.cn

[T11] Kotlin：协程
来源：http://bn.gzmigu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vi.hahajie.cn

[T12] Kotlin：解构声明
来源：http://wf.jctech888.com.cn

val (a, b) = Pair(1, 2)
来源：http://kl.jctech888.com.cn

[T13] Kotlin：只读 Map
来源：http://pz.hnjuh.cn

val m = mapOf("a" to 1)
来源：http://fe.newstarts.cn

[T14] Kotlin：循环
来源：http://jm.wgjwhj.cn

for (i in 1..10) println(i)
来源：http://hh.hnjuh.cn

[T15] Kotlin：接口
来源：http://dr.colortex.cn

interface Shape { fun area(): Double }
来源：http://be.hahajie.cn

[T16] Swift：Hello World
来源：http://dq.colortex.cn

print("Hello")
来源：http://ad.muxihuayi.cn

[T17] Swift：变量与常量
来源：http://uk.huanxung.cn

var a = 1;  let b = 2
来源：http://lj.newstarts.cn

[T18] Swift：字符串插值
来源：http://ss.shxzskj.cn

"值: \(b)"
来源：http://ir.colortex.cn

[T19] Swift：可选绑定
来源：http://ph.nszjky.cn

if let n = opt { print(n) }
来源：http://qm.nszjky.cn

[T20] Swift：数组操作
来源：http://wq.hahajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://tp.bookmarksfly.cn

[T21] Swift：遍历
来源：http://ew.szsharing.cn

for x in a { print(x) }
来源：http://jd.gzmigu.cn

[T22] Swift：字典
来源：http://km.hnjuh.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xy.huixinmuqiang.cn

[T23] Swift：函数
来源：http://dm.asd995.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hw.panjiajie.cn

[T24] Swift：闭包
来源：http://ha.shtwfgs.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qe.asd995.cn

[T25] Swift：结构体
来源：http://cw.nicolike.cn

struct P { var x: Int }
来源：http://nc.asd995.cn

[T26] Swift：类与重写
来源：http://ee.shxzukj.cn

class A: Base { override func f() {} }
来源：http://hc.panjiajie.cn

[T27] Swift：错误处理
来源：http://vc.szsharing.cn

do { try f() } catch { print(error) }
来源：http://ge.szsharing.cn

[T28] Swift：枚举
来源：http://yu.gzmigu.cn

enum Color { case red, green }
来源：http://fr.haigaiapp.cn

[T29] Swift：guard 提前返回
来源：http://fn.chemitech.net.cn

guard let x = opt else { return }
来源：http://pg.nicolike.cn

[T30] Swift：协议
来源：http://gl.nicolike.cn

protocol Shape { func area() -> Double }
来源：http://fa.szxytkj.cn

[T31] Lua：Hello World
来源：http://ea.haigaiapp.cn

print("Hello")
来源：http://sj.huixiangedu.cn

[T32] Lua：局部变量
来源：http://lp.9csxet.cn

local a = 1
来源：http://ku.shtwfgs.cn

[T33] Lua：表（数组）
来源：http://vb.huanxung.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zw.9csxet.cn

[T34] Lua：遍历表
来源：http://to.bjjhwx.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ro.yuexingan06.cn

[T35] Lua：字典表
来源：http://ff.shtwfgs.cn

local d = { a = 1 };  d.b = 2
来源：http://oq.yuntaijiaju.cn

[T36] Lua：函数
来源：http://jf.521024.cn

function add(a, b) return a + b end
来源：http://vb.shtwfgs.cn

[T37] Lua：字符串拼接
来源：http://mw.lnxyls.cn

"a" .. "b"
来源：http://ht.newstarts.cn

[T38] Lua：条件
来源：http://ry.wgjwhj.cn

if x > 0 then print("正") end
来源：http://kg.bjjhwx.cn

[T39] Lua：模式匹配
来源：http://qc.huanxung.cn

string.find(s, "%d+")
来源：http://px.gzmigu.cn

[T40] Lua：元表
来源：http://av.szxytkj.cn

setmetatable({}, { __index = base })
来源：http://ke.hahajie.cn

[T41] Perl：Hello World
来源：http://im.szsharing.cn

print "Hello\n";
来源：http://np.bookmarksfly.cn

[T42] Perl：变量类型
来源：http://lv.9csxet.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fo.szsharing.cn

[T43] Perl：字符串插值
来源：http://ze.huixinmuqiang.cn

"值: $a"
来源：http://xp.huixiangedu.cn

[T44] Perl：条件
来源：http://tm.yuexingan06.cn

if ($a > 0) { print "正"; }
来源：http://fx.bookmarksfly.cn

[T45] Perl：数组遍历
来源：http://ou.hnjuh.cn

for my $x (@arr) { print $x; }
来源：http://ym.huixinmuqiang.cn

[T46] Perl：哈希操作
来源：http://uh.huixiangedu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://be.hnjuh.cn

[T47] Perl：正则捕获
来源：http://tl.yuexingan06.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://us.wgjwhj.cn

[T48] Perl：正则替换
来源：http://pr.huixiangedu.cn

$s =~ s/old/new/g;
来源：http://dg.yuntaijiaju.cn

[T49] Perl：函数
来源：http://ds.huixiangedu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gm.nszjky.cn

[T50] Perl：逐行读文件
来源：http://in.huixiangedu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://hu.nszjky.cn

while (my $line = <$fh>) { print $line; }
来源：http://rp.shtwfgs.cn

[T51] Scala：Hello World
来源：http://wg.huanxung.cn

println("Hello")
来源：http://qu.nszjky.cn

[T52] Scala：变量
来源：http://uk.huanxung.cn

val a = 1;  var b = 2
来源：http://rk.huanxung.cn

[T53] Scala：字符串插值
来源：http://hq.szsharing.cn

s"值: $b"
来源：http://rp.hahajie.cn

[T54] Scala：集合映射
来源：http://ty.hnjuh.cn

List(1, 2, 3).map(_ * 2)
来源：http://il.yuexingan06.cn

[T55] Scala：集合过滤
来源：http://xc.lnxyls.cn

List(1, 2, 3).filter(_ > 1)
来源：http://yp.muxihuayi.cn

[T56] Scala：样例类
来源：http://na.gzmigu.cn

case class User(name: String, age: Int)
来源：http://ve.yuntaijiaju.cn

[T57] Scala：模式匹配
来源：http://wk.hnjuh.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tm.asd995.cn

[T58] Scala：函数定义
来源：http://mr.bookmarksfly.cn

def add(a: Int, b: Int): Int = a + b
来源：http://cd.haigaiapp.cn

[T59] Scala：循环
来源：http://xa.chemitech.net.cn

for (i <- 1 to 10) println(i)
来源：http://iu.nicolike.cn

[T60] Scala：折叠
来源：http://tc.asd995.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gt.haigaiapp.cn

================================================================================
来源：http://xy.huixiangedu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zz.asd995.cn

================================================================================
来源：http://kc.szsharing.cn

[U01] Py：创建虚拟环境
来源：http://nv.huixiangedu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://uq.asd995.cn

[U02] Py：导出 / 安装依赖
来源：http://mv.9csxet.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nb.nicolike.cn

[U03] Py：加载 .env 配置
来源：http://vy.bookmarksfly.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://il.jianghongdianzi.cn

[U04] Py：变量调试打印
来源：http://zf.hahajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rv.wgjwhj.cn

[U05] Py：列表去重且保序
来源：http://op.shxzskj.cn

list(dict.fromkeys(arr))
来源：http://du.chemitech.net.cn

[U06] Py：合并两个字典
来源：http://yn.shxzukj.cn

{**a, **b}
来源：http://aj.shxzskj.cn

[U07] Py：反转字典键值
来源：http://tc.nicolike.cn

{v: k for k, v in d.items()}
来源：http://qj.lnxyls.cn

[U08] Py：展平二维列表
来源：http://kh.huanxung.cn

[y for x in nested for y in x]
来源：http://fe.shxzskj.cn

[U09] Py：字典取最大值的键
来源：http://mn.nszjky.cn

max(d, key=d.get)
来源：http://ub.haigaiapp.cn

[U10] Py：按值排序字典
来源：http://va.hahajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rc.bjjhwx.cn

[U11] Py：生成器表达式
来源：http://tu.hnjuh.cn

(x * 2 for x in arr)
来源：http://gy.newstarts.cn

[U12] Py：取出现最多的 3 个元素
来源：http://uv.shxzukj.cn

Counter(arr).most_common(3)
来源：http://ul.nicolike.cn

[U13] Py：固定长度队列
来源：http://nf.gzmigu.cn

deque(maxlen=10)
来源：http://nc.gzmigu.cn

[U14] Py：分组收集到列表
来源：http://yq.bjjhwx.cn

defaultdict(list)
来源：http://py.panjiajie.cn

[U15] Py：高精度计时
来源：http://cq.panjiajie.cn

t = time.perf_counter()
来源：http://mv.521024.cn

[U16] Py：命令行参数解析
来源：http://hm.muxihuayi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ac.gzmigu.cn

[U17] Py：初始化日志
来源：http://qd.nicolike.cn

logging.basicConfig(level=logging.INFO)
来源：http://vh.huanxung.cn

[U18] Py：预编译正则
来源：http://vx.huanxung.cn

pat = re.compile(r"\d+")
来源：http://jp.nszjky.cn

[U19] Py：正则替换带回调
来源：http://bh.hnjuh.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yk.jctech888.com.cn

[U20] Py：缓存函数结果
来源：http://rj.jctech888.com.cn

@functools.lru_cache(maxsize=None)
来源：http://pv.szxytkj.cn

[U21] Py：自定义上下文管理器
来源：http://td.yuexingan06.cn

@contextlib.contextmanager
来源：http://oi.newstarts.cn

[U22] Py：矩阵转置
来源：http://jk.gzmigu.cn

list(zip(*m))
来源：http://gg.521024.cn

[U23] Py：分块读取大文件
来源：http://oj.chemitech.net.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://um.hahajie.cn

[U24] Py：路径操作
来源：http://nj.shxzukj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://uk.shxzskj.cn

[U25] Py：CSV 按字典读
来源：http://la.wgjwhj.cn

csv.DictReader(f)
来源：http://re.asd995.cn

[U26] Py：并发下载
来源：http://hp.hnjuh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ne.hnjuh.cn

[U27] Py：异步 HTTP
来源：http://fh.lnxyls.cn

aiohttp.ClientSession() 配合 async with
来源：http://sm.lnxyls.cn

[U28] Py：类型别名
来源：http://ch.yuntaijiaju.cn

UserId = int
来源：http://de.szsharing.cn


<!-- 参考信息 -->