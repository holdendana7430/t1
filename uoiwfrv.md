代发 wailian999

strlen(s)
来源：http://ts.jctech888.com.cn

[S06] C：字符串比较
来源：http://uz.huixinmuqiang.cn

strcmp(a, b) == 0
来源：http://so.hahajie.cn

[S07] C：数组遍历求和
来源：http://bp.hnjuh.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ec.shxzukj.cn

[S08] C：动态内存分配与释放
来源：http://ng.newstarts.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://su.521024.cn

[S09] C：结构体定义与初始化
来源：http://or.wgjwhj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zm.bjjhwx.cn

[S10] C：指针与解引用
来源：http://uo.haigaiapp.cn

int *p = &a;  *p = 5;
来源：http://vj.nszjky.cn

[S11] C：逐行读文件
来源：http://cl.huanxung.cn

FILE *f = fopen("a.txt", "r");
来源：http://rc.haigaiapp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gq.muxihuayi.cn

fclose(f);
来源：http://zl.haigaiapp.cn

[S12] C：写文件
来源：http://xk.wgjwhj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zy.lnxyls.cn

[S13] C：宏定义
来源：http://pk.shtwfgs.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fh.yuntaijiaju.cn

[S14] C：枚举
来源：http://mx.nszjky.cn

enum Color { RED, GREEN, BLUE };
来源：http://pu.jctech888.com.cn

[S15] C：类型转换
来源：http://rr.521024.cn

(double) a / b
来源：http://vt.haigaiapp.cn

[S16] C：位操作置位
来源：http://pu.hnjuh.cn

x |= (1 << 3);
来源：http://bx.nszjky.cn

[S17] C：安全拼接字符串
来源：http://rr.haigaiapp.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://eq.nicolike.cn

[S18] C：命令行参数
来源：http://kf.haigaiapp.cn

int main(int argc, char **argv)
来源：http://sb.shtwfgs.cn

[S19] C：快速排序
来源：http://cx.chemitech.net.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vm.gzmigu.cn

[S20] C：二分查找
来源：http://jw.huixiangedu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pz.szxytkj.cn

[S21] C：字符类别判断
来源：http://ep.9csxet.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ub.gzmigu.cn

[S22] C：字符串转数字
来源：http://ox.nicolike.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fz.muxihuayi.cn

[S23] C：随机数
来源：http://by.shtwfgs.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://tf.haigaiapp.cn

[S24] C：获取本地时间
来源：http://ga.huanxung.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fr.gzmigu.cn

[S25] C：内存拷贝
来源：http://ij.shxzukj.cn

memcpy(dst, src, n);
来源：http://bi.huanxung.cn

[S26] C：内存清零
来源：http://qk.asd995.cn

memset(a, 0, sizeof a);
来源：http://kc.shxzskj.cn

[S27] C：定义常量
来源：http://qe.nicolike.cn

const double PI = 3.14159;
来源：http://do.lnxyls.cn

[S28] C：静态变量
来源：http://zb.nszjky.cn

static int counter = 0;
来源：http://ke.gzmigu.cn

[S29] C：变参函数
来源：http://fe.chemitech.net.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://op.szxytkj.cn

[S30] C：头文件保护
来源：http://ns.chemitech.net.cn

#ifndef X_H
来源：http://dv.9csxet.cn

#define X_H
来源：http://gm.yuntaijiaju.cn

#endif
来源：http://dy.nszjky.cn

[S31] C++：Hello World
来源：http://rt.huixiangedu.cn

#include <iostream>
来源：http://ea.hahajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://cr.shxzskj.cn

[S32] C++：字符串
来源：http://sd.bjjhwx.cn

std::string s = "hi";  s += "!";
来源：http://sq.bjjhwx.cn

[S33] C++：vector 增删
来源：http://sa.wgjwhj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yv.hnjuh.cn

[S34] C++：遍历 vector
来源：http://ug.nicolike.cn

for (auto &x : v) { std::cout << x; }
来源：http://jy.colortex.cn

[S35] C++：map
来源：http://za.shxzukj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://te.haigaiapp.cn

[S36] C++：unordered_map
来源：http://wg.muxihuayi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xf.asd995.cn

[S37] C++：set
来源：http://yp.asd995.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fu.jianghongdianzi.cn

[S38] C++：排序
来源：http://tj.jctech888.com.cn

std::sort(v.begin(), v.end());
来源：http://ce.yuexingan06.cn

[S39] C++：自定义比较器排序
来源：http://vw.muxihuayi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://eo.jctech888.com.cn

[S40] C++：查找元素
来源：http://qk.hahajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xy.nicolike.cn

[S41] C++：类与构造函数
来源：http://av.bjjhwx.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yf.asd995.cn

[S42] C++：继承与虚函数
来源：http://lc.muxihuayi.cn

class B : public Base { public: void f() override {} };
来源：http://vy.shxzukj.cn

[S43] C++：智能指针
来源：http://el.yuntaijiaju.cn

auto p = std::make_unique<int>(5);
来源：http://um.huixiangedu.cn

[S44] C++：引用传参
来源：http://zp.haigaiapp.cn

void inc(int &x) { ++x; }
来源：http://ah.shtwfgs.cn

[S45] C++：lambda
来源：http://ap.bookmarksfly.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ar.yuntaijiaju.cn

[S46] C++：函数模板
来源：http://qm.lnxyls.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ug.jctech888.com.cn

[S47] C++：结构化绑定遍历
来源：http://dy.hahajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bi.521024.cn

[S48] C++：逐行读文件
来源：http://uw.panjiajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ln.9csxet.cn

while (std::getline(in, line)) { }
来源：http://rh.haigaiapp.cn

[S49] C++：写文件
来源：http://fl.521024.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jp.shtwfgs.cn

[S50] C++：格式化数字
来源：http://gb.huixinmuqiang.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ab.shxzukj.cn

[S51] C++：显式类型转换
来源：http://li.newstarts.cn

static_cast<double>(a) / b
来源：http://af.yuexingan06.cn

[S52] C++：const 与 noexcept
来源：http://uq.nicolike.cn

int size() const noexcept { return n_; }
来源：http://ud.panjiajie.cn

[S53] C++：移动语义
来源：http://oe.huixiangedu.cn

std::vector<int> w = std::move(v);
来源：http://go.yuexingan06.cn

[S54] C++：异常处理
来源：http://nt.shxzukj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ym.wgjwhj.cn

[S55] C++：结构化绑定
来源：http://tp.hahajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://um.newstarts.cn

[S56] C++：optional
来源：http://hr.huixinmuqiang.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kd.shxzukj.cn

[S57] C++：编译期常量
来源：http://of.yuntaijiaju.cn

constexpr int N = 10;
来源：http://dj.asd995.cn

[S58] C++：命名空间
来源：http://ec.jctech888.com.cn

namespace ns { int f() { return 1; } }
来源：http://wf.colortex.cn

[S59] C++：静态断言
来源：http://eq.jctech888.com.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zb.bookmarksfly.cn

[S60] C++：遍历并删除元素
来源：http://yp.nszjky.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://si.bookmarksfly.cn

================================================================================
来源：http://xn.jctech888.com.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://iu.shtwfgs.cn

================================================================================
来源：http://im.jctech888.com.cn

[T01] Kotlin：Hello World
来源：http://al.huixiangedu.cn

println("Hello")
来源：http://tf.panjiajie.cn

[T02] Kotlin：变量
来源：http://kj.newstarts.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yz.nicolike.cn

[T03] Kotlin：字符串模板
来源：http://uz.jctech888.com.cn

"值: $b"
来源：http://hc.newstarts.cn

[T04] Kotlin：空安全
来源：http://ch.newstarts.cn

val n: String? = null;  n?.length
来源：http://bf.jctech888.com.cn

[T05] Kotlin：when 表达式
来源：http://rs.nszjky.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mx.colortex.cn

[T06] Kotlin：集合映射
来源：http://pf.yuntaijiaju.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://bt.shxzskj.cn

[T07] Kotlin：集合过滤
来源：http://yg.szxytkj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tv.bjjhwx.cn

[T08] Kotlin：数据类
来源：http://gl.colortex.cn

data class User(val name: String, val age: Int)
来源：http://uz.wgjwhj.cn

[T09] Kotlin：扩展函数
来源：http://uf.nszjky.cn

fun String.exclaim() = this + "!"
来源：http://en.szxytkj.cn

[T10] Kotlin：默认参数
来源：http://pr.huixiangedu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://us.hahajie.cn

[T11] Kotlin：协程
来源：http://bk.bjjhwx.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ot.nicolike.cn

[T12] Kotlin：解构声明
来源：http://wh.shxzskj.cn

val (a, b) = Pair(1, 2)
来源：http://pm.haigaiapp.cn

[T13] Kotlin：只读 Map
来源：http://oe.jianghongdianzi.cn

val m = mapOf("a" to 1)
来源：http://lc.shtwfgs.cn

[T14] Kotlin：循环
来源：http://lo.szsharing.cn

for (i in 1..10) println(i)
来源：http://xx.nszjky.cn

[T15] Kotlin：接口
来源：http://au.szsharing.cn

interface Shape { fun area(): Double }
来源：http://wd.nszjky.cn

[T16] Swift：Hello World
来源：http://wp.haigaiapp.cn

print("Hello")
来源：http://kr.szsharing.cn

[T17] Swift：变量与常量
来源：http://dp.chemitech.net.cn

var a = 1;  let b = 2
来源：http://rz.nicolike.cn

[T18] Swift：字符串插值
来源：http://oi.huixinmuqiang.cn

"值: \(b)"
来源：http://rr.jctech888.com.cn

[T19] Swift：可选绑定
来源：http://er.colortex.cn

if let n = opt { print(n) }
来源：http://iy.lnxyls.cn

[T20] Swift：数组操作
来源：http://sn.521024.cn

var a = [1, 2, 3];  a.append(4)
来源：http://dq.hahajie.cn

[T21] Swift：遍历
来源：http://gb.panjiajie.cn

for x in a { print(x) }
来源：http://xo.gzmigu.cn

[T22] Swift：字典
来源：http://gi.bookmarksfly.cn

var d = ["a": 1];  d["b"] = 2
来源：http://kz.newstarts.cn

[T23] Swift：函数
来源：http://xl.jianghongdianzi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ve.huixiangedu.cn

[T24] Swift：闭包
来源：http://gx.haigaiapp.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://st.jianghongdianzi.cn

[T25] Swift：结构体
来源：http://wt.szsharing.cn

struct P { var x: Int }
来源：http://bk.521024.cn

[T26] Swift：类与重写
来源：http://jk.gzmigu.cn

class A: Base { override func f() {} }
来源：http://wk.gzmigu.cn

[T27] Swift：错误处理
来源：http://tx.yuntaijiaju.cn

do { try f() } catch { print(error) }
来源：http://xr.hnjuh.cn

[T28] Swift：枚举
来源：http://sw.shtwfgs.cn

enum Color { case red, green }
来源：http://sw.szsharing.cn

[T29] Swift：guard 提前返回
来源：http://oi.jctech888.com.cn

guard let x = opt else { return }
来源：http://cv.nicolike.cn

[T30] Swift：协议
来源：http://tq.gzmigu.cn

protocol Shape { func area() -> Double }
来源：http://nl.9csxet.cn

[T31] Lua：Hello World
来源：http://fg.jctech888.com.cn

print("Hello")
来源：http://dz.lnxyls.cn

[T32] Lua：局部变量
来源：http://lo.yuntaijiaju.cn

local a = 1
来源：http://dg.shxzskj.cn

[T33] Lua：表（数组）
来源：http://yq.521024.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ua.nszjky.cn

[T34] Lua：遍历表
来源：http://jr.wgjwhj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ln.szxytkj.cn

[T35] Lua：字典表
来源：http://lr.bjjhwx.cn

local d = { a = 1 };  d.b = 2
来源：http://xs.huixiangedu.cn

[T36] Lua：函数
来源：http://cl.huixinmuqiang.cn

function add(a, b) return a + b end
来源：http://nv.huixiangedu.cn

[T37] Lua：字符串拼接
来源：http://ri.yuexingan06.cn

"a" .. "b"
来源：http://al.521024.cn

[T38] Lua：条件
来源：http://gy.szsharing.cn

if x > 0 then print("正") end
来源：http://ky.huixiangedu.cn

[T39] Lua：模式匹配
来源：http://bw.asd995.cn

string.find(s, "%d+")
来源：http://my.asd995.cn

[T40] Lua：元表
来源：http://gn.huanxung.cn

setmetatable({}, { __index = base })
来源：http://oa.jianghongdianzi.cn

[T41] Perl：Hello World
来源：http://yw.haigaiapp.cn

print "Hello\n";
来源：http://os.huixiangedu.cn

[T42] Perl：变量类型
来源：http://hm.shxzskj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qh.haigaiapp.cn

[T43] Perl：字符串插值
来源：http://yj.jctech888.com.cn

"值: $a"
来源：http://qx.shtwfgs.cn

[T44] Perl：条件
来源：http://mq.yuntaijiaju.cn

if ($a > 0) { print "正"; }
来源：http://we.yuexingan06.cn

[T45] Perl：数组遍历
来源：http://zx.shxzskj.cn

for my $x (@arr) { print $x; }
来源：http://ww.gzmigu.cn

[T46] Perl：哈希操作
来源：http://fr.asd995.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hl.nszjky.cn

[T47] Perl：正则捕获
来源：http://ft.shxzskj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wv.huanxung.cn

[T48] Perl：正则替换
来源：http://pd.chemitech.net.cn

$s =~ s/old/new/g;
来源：http://pn.colortex.cn

[T49] Perl：函数
来源：http://on.shtwfgs.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lc.jctech888.com.cn

[T50] Perl：逐行读文件
来源：http://kk.hnjuh.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://kw.bookmarksfly.cn

while (my $line = <$fh>) { print $line; }
来源：http://nl.shtwfgs.cn

[T51] Scala：Hello World
来源：http://bf.jctech888.com.cn

println("Hello")
来源：http://tu.huixiangedu.cn

[T52] Scala：变量
来源：http://bm.shxzukj.cn

val a = 1;  var b = 2
来源：http://li.colortex.cn

[T53] Scala：字符串插值
来源：http://zn.shxzukj.cn

s"值: $b"
来源：http://bd.hahajie.cn

[T54] Scala：集合映射
来源：http://fr.szsharing.cn

List(1, 2, 3).map(_ * 2)
来源：http://qp.huanxung.cn

[T55] Scala：集合过滤
来源：http://fp.lnxyls.cn

List(1, 2, 3).filter(_ > 1)
来源：http://cy.jctech888.com.cn

[T56] Scala：样例类
来源：http://mp.9csxet.cn

case class User(name: String, age: Int)
来源：http://xz.lnxyls.cn

[T57] Scala：模式匹配
来源：http://pg.asd995.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://uy.huixiangedu.cn

[T58] Scala：函数定义
来源：http://mz.gzmigu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zu.nicolike.cn

[T59] Scala：循环
来源：http://dj.nicolike.cn

for (i <- 1 to 10) println(i)
来源：http://cf.muxihuayi.cn

[T60] Scala：折叠
来源：http://hg.asd995.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ri.chemitech.net.cn

================================================================================
来源：http://aq.shtwfgs.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nf.nicolike.cn

================================================================================
来源：http://nd.hahajie.cn

[U01] Py：创建虚拟环境
来源：http://dq.shxzskj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://hr.chemitech.net.cn

[U02] Py：导出 / 安装依赖
来源：http://sj.nicolike.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ro.521024.cn

[U03] Py：加载 .env 配置
来源：http://wr.521024.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://tt.hahajie.cn

[U04] Py：变量调试打印
来源：http://xe.hnjuh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ow.colortex.cn

[U05] Py：列表去重且保序
来源：http://uo.huanxung.cn

list(dict.fromkeys(arr))
来源：http://za.shtwfgs.cn

[U06] Py：合并两个字典
来源：http://ot.newstarts.cn

{**a, **b}
来源：http://xr.newstarts.cn

[U07] Py：反转字典键值
来源：http://hr.huanxung.cn

{v: k for k, v in d.items()}
来源：http://oh.hnjuh.cn

[U08] Py：展平二维列表
来源：http://vi.wgjwhj.cn

[y for x in nested for y in x]
来源：http://ox.bookmarksfly.cn

[U09] Py：字典取最大值的键
来源：http://rq.lnxyls.cn

max(d, key=d.get)
来源：http://yc.newstarts.cn

[U10] Py：按值排序字典
来源：http://mz.szxytkj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://eu.nszjky.cn

[U11] Py：生成器表达式
来源：http://or.haigaiapp.cn

(x * 2 for x in arr)
来源：http://gs.bjjhwx.cn

[U12] Py：取出现最多的 3 个元素
来源：http://bt.yuexingan06.cn

Counter(arr).most_common(3)
来源：http://lk.nicolike.cn

[U13] Py：固定长度队列
来源：http://lt.szxytkj.cn

deque(maxlen=10)
来源：http://eq.huixiangedu.cn

[U14] Py：分组收集到列表
来源：http://jk.huixinmuqiang.cn

defaultdict(list)
来源：http://yy.asd995.cn

[U15] Py：高精度计时
来源：http://yi.wgjwhj.cn

t = time.perf_counter()
来源：http://jt.huixiangedu.cn

[U16] Py：命令行参数解析
来源：http://pm.yuntaijiaju.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bv.yuexingan06.cn

[U17] Py：初始化日志
来源：http://eg.huixinmuqiang.cn

logging.basicConfig(level=logging.INFO)
来源：http://gb.asd995.cn

[U18] Py：预编译正则
来源：http://rb.wgjwhj.cn

pat = re.compile(r"\d+")
来源：http://jl.shtwfgs.cn

[U19] Py：正则替换带回调
来源：http://nw.huixinmuqiang.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nm.colortex.cn

[U20] Py：缓存函数结果
来源：http://ua.nszjky.cn

@functools.lru_cache(maxsize=None)
来源：http://wh.bookmarksfly.cn

[U21] Py：自定义上下文管理器
来源：http://ai.jctech888.com.cn

@contextlib.contextmanager
来源：http://vd.panjiajie.cn

[U22] Py：矩阵转置
来源：http://eg.panjiajie.cn

list(zip(*m))
来源：http://fe.huixiangedu.cn

[U23] Py：分块读取大文件
来源：http://mi.bjjhwx.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zk.yuexingan06.cn

[U24] Py：路径操作
来源：http://nw.bjjhwx.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zx.asd995.cn

[U25] Py：CSV 按字典读
来源：http://ov.yuexingan06.cn

csv.DictReader(f)
来源：http://uy.bjjhwx.cn

[U26] Py：并发下载
来源：http://ui.shxzskj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jb.jctech888.com.cn

[U27] Py：异步 HTTP
来源：http://dz.chemitech.net.cn

aiohttp.ClientSession() 配合 async with
来源：http://nm.newstarts.cn

[U28] Py：类型别名
来源：http://ch.colortex.cn

UserId = int
来源：http://ax.jianghongdianzi.cn


<!-- 参考信息 -->