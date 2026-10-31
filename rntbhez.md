代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cc.chemitech.net.cn

[S08] C：动态内存分配与释放
来源：http://dp.chemitech.net.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xv.asd995.cn

[S09] C：结构体定义与初始化
来源：http://ow.colortex.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://oj.newstarts.cn

[S10] C：指针与解引用
来源：http://rt.hahajie.cn

int *p = &a;  *p = 5;
来源：http://ki.szsharing.cn

[S11] C：逐行读文件
来源：http://pv.huixinmuqiang.cn

FILE *f = fopen("a.txt", "r");
来源：http://ln.huixiangedu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wt.lnxyls.cn

fclose(f);
来源：http://sb.521024.cn

[S12] C：写文件
来源：http://wn.lnxyls.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cu.9csxet.cn

[S13] C：宏定义
来源：http://yt.huixiangedu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qd.muxihuayi.cn

[S14] C：枚举
来源：http://lp.colortex.cn

enum Color { RED, GREEN, BLUE };
来源：http://xd.huanxung.cn

[S15] C：类型转换
来源：http://pq.shxzukj.cn

(double) a / b
来源：http://sv.hahajie.cn

[S16] C：位操作置位
来源：http://wu.bjjhwx.cn

x |= (1 << 3);
来源：http://br.newstarts.cn

[S17] C：安全拼接字符串
来源：http://is.bjjhwx.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cd.newstarts.cn

[S18] C：命令行参数
来源：http://bi.lnxyls.cn

int main(int argc, char **argv)
来源：http://ql.chemitech.net.cn

[S19] C：快速排序
来源：http://gw.muxihuayi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ft.asd995.cn

[S20] C：二分查找
来源：http://zq.yuntaijiaju.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://aw.huixiangedu.cn

[S21] C：字符类别判断
来源：http://jd.521024.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://iz.gzmigu.cn

[S22] C：字符串转数字
来源：http://if.newstarts.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ir.szxytkj.cn

[S23] C：随机数
来源：http://tc.szxytkj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ne.newstarts.cn

[S24] C：获取本地时间
来源：http://dg.hahajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jl.colortex.cn

[S25] C：内存拷贝
来源：http://cb.huixiangedu.cn

memcpy(dst, src, n);
来源：http://hx.yuntaijiaju.cn

[S26] C：内存清零
来源：http://je.gzmigu.cn

memset(a, 0, sizeof a);
来源：http://qz.colortex.cn

[S27] C：定义常量
来源：http://uc.shtwfgs.cn

const double PI = 3.14159;
来源：http://ui.9csxet.cn

[S28] C：静态变量
来源：http://qe.muxihuayi.cn

static int counter = 0;
来源：http://tb.bjjhwx.cn

[S29] C：变参函数
来源：http://ul.jctech888.com.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yx.haigaiapp.cn

[S30] C：头文件保护
来源：http://ve.hahajie.cn

#ifndef X_H
来源：http://gt.huixinmuqiang.cn

#define X_H
来源：http://am.asd995.cn

#endif
来源：http://kz.yuntaijiaju.cn

[S31] C++：Hello World
来源：http://ze.chemitech.net.cn

#include <iostream>
来源：http://ij.colortex.cn

int main() { std::cout << "Hello\n"; }
来源：http://in.huanxung.cn

[S32] C++：字符串
来源：http://ex.yuexingan06.cn

std::string s = "hi";  s += "!";
来源：http://sb.bookmarksfly.cn

[S33] C++：vector 增删
来源：http://xe.lnxyls.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ef.bjjhwx.cn

[S34] C++：遍历 vector
来源：http://ko.jctech888.com.cn

for (auto &x : v) { std::cout << x; }
来源：http://wa.lnxyls.cn

[S35] C++：map
来源：http://xt.colortex.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://da.nszjky.cn

[S36] C++：unordered_map
来源：http://sq.jianghongdianzi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ia.gzmigu.cn

[S37] C++：set
来源：http://wy.szxytkj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yx.huanxung.cn

[S38] C++：排序
来源：http://nc.yuexingan06.cn

std::sort(v.begin(), v.end());
来源：http://th.chemitech.net.cn

[S39] C++：自定义比较器排序
来源：http://gv.nszjky.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sd.huixinmuqiang.cn

[S40] C++：查找元素
来源：http://up.nszjky.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nv.lnxyls.cn

[S41] C++：类与构造函数
来源：http://hp.521024.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zu.jianghongdianzi.cn

[S42] C++：继承与虚函数
来源：http://nr.bookmarksfly.cn

class B : public Base { public: void f() override {} };
来源：http://ae.szxytkj.cn

[S43] C++：智能指针
来源：http://nf.hnjuh.cn

auto p = std::make_unique<int>(5);
来源：http://ft.shxzukj.cn

[S44] C++：引用传参
来源：http://aa.nicolike.cn

void inc(int &x) { ++x; }
来源：http://zi.shxzskj.cn

[S45] C++：lambda
来源：http://mn.nicolike.cn

auto add = [](int a, int b) { return a + b; };
来源：http://oe.9csxet.cn

[S46] C++：函数模板
来源：http://hd.asd995.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jq.wgjwhj.cn

[S47] C++：结构化绑定遍历
来源：http://gy.szxytkj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ug.haigaiapp.cn

[S48] C++：逐行读文件
来源：http://zt.lnxyls.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zm.lnxyls.cn

while (std::getline(in, line)) { }
来源：http://hy.shtwfgs.cn

[S49] C++：写文件
来源：http://xo.panjiajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ec.yuntaijiaju.cn

[S50] C++：格式化数字
来源：http://qb.bookmarksfly.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ib.nicolike.cn

[S51] C++：显式类型转换
来源：http://gq.hnjuh.cn

static_cast<double>(a) / b
来源：http://fs.gzmigu.cn

[S52] C++：const 与 noexcept
来源：http://zo.hahajie.cn

int size() const noexcept { return n_; }
来源：http://wy.yuexingan06.cn

[S53] C++：移动语义
来源：http://vz.gzmigu.cn

std::vector<int> w = std::move(v);
来源：http://fw.muxihuayi.cn

[S54] C++：异常处理
来源：http://vo.bookmarksfly.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sb.szxytkj.cn

[S55] C++：结构化绑定
来源：http://iy.jianghongdianzi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ln.nicolike.cn

[S56] C++：optional
来源：http://vj.bjjhwx.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://te.newstarts.cn

[S57] C++：编译期常量
来源：http://xo.jianghongdianzi.cn

constexpr int N = 10;
来源：http://ex.nszjky.cn

[S58] C++：命名空间
来源：http://qr.szxytkj.cn

namespace ns { int f() { return 1; } }
来源：http://gp.szxytkj.cn

[S59] C++：静态断言
来源：http://fs.huixinmuqiang.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uy.yuntaijiaju.cn

[S60] C++：遍历并删除元素
来源：http://on.muxihuayi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qz.yuexingan06.cn

================================================================================
来源：http://zy.szxytkj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ao.huixiangedu.cn

================================================================================
来源：http://qx.yuntaijiaju.cn

[T01] Kotlin：Hello World
来源：http://hh.gzmigu.cn

println("Hello")
来源：http://we.yuntaijiaju.cn

[T02] Kotlin：变量
来源：http://jq.yuntaijiaju.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gp.huanxung.cn

[T03] Kotlin：字符串模板
来源：http://wm.haigaiapp.cn

"值: $b"
来源：http://ou.lnxyls.cn

[T04] Kotlin：空安全
来源：http://ec.panjiajie.cn

val n: String? = null;  n?.length
来源：http://hv.521024.cn

[T05] Kotlin：when 表达式
来源：http://kr.huixinmuqiang.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zn.bookmarksfly.cn

[T06] Kotlin：集合映射
来源：http://de.jianghongdianzi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://pp.jctech888.com.cn

[T07] Kotlin：集合过滤
来源：http://kh.yuexingan06.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ce.haigaiapp.cn

[T08] Kotlin：数据类
来源：http://re.nicolike.cn

data class User(val name: String, val age: Int)
来源：http://oj.shxzukj.cn

[T09] Kotlin：扩展函数
来源：http://sq.jctech888.com.cn

fun String.exclaim() = this + "!"
来源：http://mu.jctech888.com.cn

[T10] Kotlin：默认参数
来源：http://lv.nszjky.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wn.shxzskj.cn

[T11] Kotlin：协程
来源：http://ag.bjjhwx.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xw.huixiangedu.cn

[T12] Kotlin：解构声明
来源：http://pt.hnjuh.cn

val (a, b) = Pair(1, 2)
来源：http://zo.chemitech.net.cn

[T13] Kotlin：只读 Map
来源：http://vs.521024.cn

val m = mapOf("a" to 1)
来源：http://pe.gzmigu.cn

[T14] Kotlin：循环
来源：http://za.szsharing.cn

for (i in 1..10) println(i)
来源：http://en.huixiangedu.cn

[T15] Kotlin：接口
来源：http://wm.newstarts.cn

interface Shape { fun area(): Double }
来源：http://vr.521024.cn

[T16] Swift：Hello World
来源：http://pg.hahajie.cn

print("Hello")
来源：http://ej.huixiangedu.cn

[T17] Swift：变量与常量
来源：http://sm.szsharing.cn

var a = 1;  let b = 2
来源：http://it.panjiajie.cn

[T18] Swift：字符串插值
来源：http://ko.hnjuh.cn

"值: \(b)"
来源：http://rm.jianghongdianzi.cn

[T19] Swift：可选绑定
来源：http://rk.bookmarksfly.cn

if let n = opt { print(n) }
来源：http://qx.shxzukj.cn

[T20] Swift：数组操作
来源：http://rc.huanxung.cn

var a = [1, 2, 3];  a.append(4)
来源：http://rk.shxzukj.cn

[T21] Swift：遍历
来源：http://wx.shtwfgs.cn

for x in a { print(x) }
来源：http://hl.szsharing.cn

[T22] Swift：字典
来源：http://qv.nicolike.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ic.huixinmuqiang.cn

[T23] Swift：函数
来源：http://ze.jctech888.com.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hf.bookmarksfly.cn

[T24] Swift：闭包
来源：http://av.lnxyls.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://cp.jctech888.com.cn

[T25] Swift：结构体
来源：http://rw.colortex.cn

struct P { var x: Int }
来源：http://lj.521024.cn

[T26] Swift：类与重写
来源：http://jf.jianghongdianzi.cn

class A: Base { override func f() {} }
来源：http://yj.asd995.cn

[T27] Swift：错误处理
来源：http://vv.bookmarksfly.cn

do { try f() } catch { print(error) }
来源：http://yx.shtwfgs.cn

[T28] Swift：枚举
来源：http://td.shxzskj.cn

enum Color { case red, green }
来源：http://yr.haigaiapp.cn

[T29] Swift：guard 提前返回
来源：http://en.newstarts.cn

guard let x = opt else { return }
来源：http://jd.asd995.cn

[T30] Swift：协议
来源：http://cc.hahajie.cn

protocol Shape { func area() -> Double }
来源：http://xi.muxihuayi.cn

[T31] Lua：Hello World
来源：http://wu.jctech888.com.cn

print("Hello")
来源：http://kk.nicolike.cn

[T32] Lua：局部变量
来源：http://gp.9csxet.cn

local a = 1
来源：http://jw.huixinmuqiang.cn

[T33] Lua：表（数组）
来源：http://ex.gzmigu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://uq.lnxyls.cn

[T34] Lua：遍历表
来源：http://nh.hahajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://it.yuexingan06.cn

[T35] Lua：字典表
来源：http://xe.panjiajie.cn

local d = { a = 1 };  d.b = 2
来源：http://bm.huixinmuqiang.cn

[T36] Lua：函数
来源：http://go.lnxyls.cn

function add(a, b) return a + b end
来源：http://md.muxihuayi.cn

[T37] Lua：字符串拼接
来源：http://pp.521024.cn

"a" .. "b"
来源：http://st.wgjwhj.cn

[T38] Lua：条件
来源：http://rb.asd995.cn

if x > 0 then print("正") end
来源：http://dy.chemitech.net.cn

[T39] Lua：模式匹配
来源：http://ov.szxytkj.cn

string.find(s, "%d+")
来源：http://ft.szsharing.cn

[T40] Lua：元表
来源：http://wl.wgjwhj.cn

setmetatable({}, { __index = base })
来源：http://tq.gzmigu.cn

[T41] Perl：Hello World
来源：http://bx.huixinmuqiang.cn

print "Hello\n";
来源：http://il.huixinmuqiang.cn

[T42] Perl：变量类型
来源：http://yp.szsharing.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vb.9csxet.cn

[T43] Perl：字符串插值
来源：http://oo.newstarts.cn

"值: $a"
来源：http://qk.shxzskj.cn

[T44] Perl：条件
来源：http://xr.bjjhwx.cn

if ($a > 0) { print "正"; }
来源：http://oh.chemitech.net.cn

[T45] Perl：数组遍历
来源：http://lq.chemitech.net.cn

for my $x (@arr) { print $x; }
来源：http://mu.panjiajie.cn

[T46] Perl：哈希操作
来源：http://uc.panjiajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zf.jianghongdianzi.cn

[T47] Perl：正则捕获
来源：http://ed.lnxyls.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pd.jianghongdianzi.cn

[T48] Perl：正则替换
来源：http://zv.colortex.cn

$s =~ s/old/new/g;
来源：http://dk.jctech888.com.cn

[T49] Perl：函数
来源：http://ht.lnxyls.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yr.jctech888.com.cn

[T50] Perl：逐行读文件
来源：http://as.shtwfgs.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://sj.wgjwhj.cn

while (my $line = <$fh>) { print $line; }
来源：http://ae.hahajie.cn

[T51] Scala：Hello World
来源：http://je.yuexingan06.cn

println("Hello")
来源：http://zc.hahajie.cn

[T52] Scala：变量
来源：http://nf.shxzukj.cn

val a = 1;  var b = 2
来源：http://xa.521024.cn

[T53] Scala：字符串插值
来源：http://zu.hahajie.cn

s"值: $b"
来源：http://ei.yuexingan06.cn

[T54] Scala：集合映射
来源：http://iw.jctech888.com.cn

List(1, 2, 3).map(_ * 2)
来源：http://dw.shxzukj.cn

[T55] Scala：集合过滤
来源：http://qn.wgjwhj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://uy.szsharing.cn

[T56] Scala：样例类
来源：http://hk.colortex.cn

case class User(name: String, age: Int)
来源：http://nk.huanxung.cn

[T57] Scala：模式匹配
来源：http://pn.gzmigu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ww.jctech888.com.cn

[T58] Scala：函数定义
来源：http://fi.shxzskj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://pb.szxytkj.cn

[T59] Scala：循环
来源：http://yd.521024.cn

for (i <- 1 to 10) println(i)
来源：http://gx.gzmigu.cn

[T60] Scala：折叠
来源：http://cj.newstarts.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nq.shtwfgs.cn

================================================================================
来源：http://fd.wgjwhj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sb.521024.cn

================================================================================
来源：http://aj.muxihuayi.cn

[U01] Py：创建虚拟环境
来源：http://gw.huixiangedu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qb.shtwfgs.cn

[U02] Py：导出 / 安装依赖
来源：http://oa.shxzukj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cr.yuexingan06.cn

[U03] Py：加载 .env 配置
来源：http://rx.bjjhwx.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zz.yuntaijiaju.cn

[U04] Py：变量调试打印
来源：http://dz.bookmarksfly.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ee.hnjuh.cn

[U05] Py：列表去重且保序
来源：http://kz.bookmarksfly.cn

list(dict.fromkeys(arr))
来源：http://vs.haigaiapp.cn

[U06] Py：合并两个字典
来源：http://nl.panjiajie.cn

{**a, **b}
来源：http://ua.szsharing.cn

[U07] Py：反转字典键值
来源：http://fk.hnjuh.cn

{v: k for k, v in d.items()}
来源：http://an.hnjuh.cn

[U08] Py：展平二维列表
来源：http://un.nicolike.cn

[y for x in nested for y in x]
来源：http://ua.colortex.cn

[U09] Py：字典取最大值的键
来源：http://cp.shxzskj.cn

max(d, key=d.get)
来源：http://fw.newstarts.cn

[U10] Py：按值排序字典
来源：http://gc.hahajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qx.colortex.cn

[U11] Py：生成器表达式
来源：http://se.panjiajie.cn

(x * 2 for x in arr)
来源：http://es.lnxyls.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ms.asd995.cn

Counter(arr).most_common(3)
来源：http://ha.szxytkj.cn

[U13] Py：固定长度队列
来源：http://uc.newstarts.cn

deque(maxlen=10)
来源：http://bq.haigaiapp.cn

[U14] Py：分组收集到列表
来源：http://os.asd995.cn

defaultdict(list)
来源：http://ni.hnjuh.cn

[U15] Py：高精度计时
来源：http://os.yuntaijiaju.cn

t = time.perf_counter()
来源：http://yo.huixiangedu.cn

[U16] Py：命令行参数解析
来源：http://mn.szsharing.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jt.shtwfgs.cn

[U17] Py：初始化日志
来源：http://cc.szsharing.cn

logging.basicConfig(level=logging.INFO)
来源：http://ep.szxytkj.cn

[U18] Py：预编译正则
来源：http://es.wgjwhj.cn

pat = re.compile(r"\d+")
来源：http://iw.521024.cn

[U19] Py：正则替换带回调
来源：http://ab.huanxung.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wb.jianghongdianzi.cn

[U20] Py：缓存函数结果
来源：http://vy.muxihuayi.cn

@functools.lru_cache(maxsize=None)
来源：http://rv.nszjky.cn

[U21] Py：自定义上下文管理器
来源：http://fb.lnxyls.cn

@contextlib.contextmanager
来源：http://ox.gzmigu.cn

[U22] Py：矩阵转置
来源：http://yz.huanxung.cn

list(zip(*m))
来源：http://ez.hnjuh.cn

[U23] Py：分块读取大文件
来源：http://pd.gzmigu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://oe.chemitech.net.cn

[U24] Py：路径操作
来源：http://ah.huixinmuqiang.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ya.jianghongdianzi.cn

[U25] Py：CSV 按字典读
来源：http://cv.9csxet.cn

csv.DictReader(f)
来源：http://lz.gzmigu.cn

[U26] Py：并发下载
来源：http://ny.huixiangedu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gs.521024.cn

[U27] Py：异步 HTTP
来源：http://dd.hahajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://cw.jianghongdianzi.cn

[U28] Py：类型别名
来源：http://ha.shxzskj.cn

UserId = int
来源：http://cu.nicolike.cn

[U29] Py：属性校验
来源：http://nl.nszjky.cn

@property 与 @x.setter 配合
来源：http://cc.yuntaijiaju.cn

[U30] Py：数据类
来源：http://fi.521024.cn

@dataclass(slots=True)
来源：http://ua.panjiajie.cn


<!-- 参考信息 -->