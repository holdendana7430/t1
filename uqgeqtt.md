代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lc.bookmarksfly.cn

[S08] C：动态内存分配与释放
来源：http://uf.9csxet.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kp.jctech888.com.cn

[S09] C：结构体定义与初始化
来源：http://yp.newstarts.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ne.jctech888.com.cn

[S10] C：指针与解引用
来源：http://hp.asd995.cn

int *p = &a;  *p = 5;
来源：http://kg.szsharing.cn

[S11] C：逐行读文件
来源：http://lu.shxzskj.cn

FILE *f = fopen("a.txt", "r");
来源：http://vp.muxihuayi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://rs.shxzskj.cn

fclose(f);
来源：http://fc.gzmigu.cn

[S12] C：写文件
来源：http://iy.jianghongdianzi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zg.shxzskj.cn

[S13] C：宏定义
来源：http://rd.bjjhwx.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sl.521024.cn

[S14] C：枚举
来源：http://bv.chemitech.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://yo.jianghongdianzi.cn

[S15] C：类型转换
来源：http://cy.lnxyls.cn

(double) a / b
来源：http://jn.bjjhwx.cn

[S16] C：位操作置位
来源：http://mu.newstarts.cn

x |= (1 << 3);
来源：http://hk.asd995.cn

[S17] C：安全拼接字符串
来源：http://bp.hnjuh.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pw.newstarts.cn

[S18] C：命令行参数
来源：http://uk.nicolike.cn

int main(int argc, char **argv)
来源：http://tg.wgjwhj.cn

[S19] C：快速排序
来源：http://bm.bjjhwx.cn

qsort(a, n, sizeof(int), cmp);
来源：http://cu.muxihuayi.cn

[S20] C：二分查找
来源：http://mi.shxzukj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://du.bjjhwx.cn

[S21] C：字符类别判断
来源：http://hh.nicolike.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ab.szsharing.cn

[S22] C：字符串转数字
来源：http://zn.asd995.cn

atoi("42");  strtod("3.14", NULL);
来源：http://lz.wgjwhj.cn

[S23] C：随机数
来源：http://kx.huixiangedu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fv.hnjuh.cn

[S24] C：获取本地时间
来源：http://wv.nicolike.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://oi.szsharing.cn

[S25] C：内存拷贝
来源：http://cj.panjiajie.cn

memcpy(dst, src, n);
来源：http://vw.panjiajie.cn

[S26] C：内存清零
来源：http://tx.szxytkj.cn

memset(a, 0, sizeof a);
来源：http://uh.huixiangedu.cn

[S27] C：定义常量
来源：http://wa.wgjwhj.cn

const double PI = 3.14159;
来源：http://vo.huanxung.cn

[S28] C：静态变量
来源：http://yu.muxihuayi.cn

static int counter = 0;
来源：http://hz.asd995.cn

[S29] C：变参函数
来源：http://lc.chemitech.net.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cp.szxytkj.cn

[S30] C：头文件保护
来源：http://nw.gzmigu.cn

#ifndef X_H
来源：http://nf.szsharing.cn

#define X_H
来源：http://eq.muxihuayi.cn

#endif
来源：http://dg.gzmigu.cn

[S31] C++：Hello World
来源：http://uw.newstarts.cn

#include <iostream>
来源：http://it.asd995.cn

int main() { std::cout << "Hello\n"; }
来源：http://ym.jctech888.com.cn

[S32] C++：字符串
来源：http://qn.newstarts.cn

std::string s = "hi";  s += "!";
来源：http://dc.szsharing.cn

[S33] C++：vector 增删
来源：http://zv.wgjwhj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://la.hahajie.cn

[S34] C++：遍历 vector
来源：http://cz.shtwfgs.cn

for (auto &x : v) { std::cout << x; }
来源：http://tj.colortex.cn

[S35] C++：map
来源：http://qe.szxytkj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gq.gzmigu.cn

[S36] C++：unordered_map
来源：http://gu.jctech888.com.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://aa.521024.cn

[S37] C++：set
来源：http://bu.szxytkj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://iu.shxzukj.cn

[S38] C++：排序
来源：http://ko.asd995.cn

std::sort(v.begin(), v.end());
来源：http://vp.gzmigu.cn

[S39] C++：自定义比较器排序
来源：http://it.szxytkj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fc.gzmigu.cn

[S40] C++：查找元素
来源：http://zc.szsharing.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sz.chemitech.net.cn

[S41] C++：类与构造函数
来源：http://rd.yuntaijiaju.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dn.chemitech.net.cn

[S42] C++：继承与虚函数
来源：http://bz.haigaiapp.cn

class B : public Base { public: void f() override {} };
来源：http://cp.haigaiapp.cn

[S43] C++：智能指针
来源：http://zx.nszjky.cn

auto p = std::make_unique<int>(5);
来源：http://mm.bjjhwx.cn

[S44] C++：引用传参
来源：http://lj.nszjky.cn

void inc(int &x) { ++x; }
来源：http://iv.haigaiapp.cn

[S45] C++：lambda
来源：http://je.lnxyls.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dw.haigaiapp.cn

[S46] C++：函数模板
来源：http://et.lnxyls.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wk.huanxung.cn

[S47] C++：结构化绑定遍历
来源：http://qa.jianghongdianzi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kq.nszjky.cn

[S48] C++：逐行读文件
来源：http://na.wgjwhj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jd.wgjwhj.cn

while (std::getline(in, line)) { }
来源：http://vd.newstarts.cn

[S49] C++：写文件
来源：http://av.lnxyls.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sk.wgjwhj.cn

[S50] C++：格式化数字
来源：http://zk.asd995.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uf.colortex.cn

[S51] C++：显式类型转换
来源：http://wd.huixiangedu.cn

static_cast<double>(a) / b
来源：http://gz.hahajie.cn

[S52] C++：const 与 noexcept
来源：http://wd.wgjwhj.cn

int size() const noexcept { return n_; }
来源：http://go.bookmarksfly.cn

[S53] C++：移动语义
来源：http://ms.hnjuh.cn

std::vector<int> w = std::move(v);
来源：http://xx.huixinmuqiang.cn

[S54] C++：异常处理
来源：http://lx.9csxet.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zu.szsharing.cn

[S55] C++：结构化绑定
来源：http://qc.chemitech.net.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://lu.muxihuayi.cn

[S56] C++：optional
来源：http://im.wgjwhj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://to.yuexingan06.cn

[S57] C++：编译期常量
来源：http://yl.szxytkj.cn

constexpr int N = 10;
来源：http://dr.huanxung.cn

[S58] C++：命名空间
来源：http://bp.lnxyls.cn

namespace ns { int f() { return 1; } }
来源：http://fc.haigaiapp.cn

[S59] C++：静态断言
来源：http://td.hnjuh.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ew.wgjwhj.cn

[S60] C++：遍历并删除元素
来源：http://nt.huanxung.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ma.nszjky.cn

================================================================================
来源：http://pd.huanxung.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ma.szsharing.cn

================================================================================
来源：http://ha.shxzukj.cn

[T01] Kotlin：Hello World
来源：http://nl.szsharing.cn

println("Hello")
来源：http://sc.colortex.cn

[T02] Kotlin：变量
来源：http://ih.haigaiapp.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wh.muxihuayi.cn

[T03] Kotlin：字符串模板
来源：http://gl.yuntaijiaju.cn

"值: $b"
来源：http://op.muxihuayi.cn

[T04] Kotlin：空安全
来源：http://hu.bjjhwx.cn

val n: String? = null;  n?.length
来源：http://oy.bookmarksfly.cn

[T05] Kotlin：when 表达式
来源：http://ys.bookmarksfly.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xe.hnjuh.cn

[T06] Kotlin：集合映射
来源：http://pt.shtwfgs.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://vp.jianghongdianzi.cn

[T07] Kotlin：集合过滤
来源：http://yp.panjiajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tk.panjiajie.cn

[T08] Kotlin：数据类
来源：http://ds.jctech888.com.cn

data class User(val name: String, val age: Int)
来源：http://wo.nszjky.cn

[T09] Kotlin：扩展函数
来源：http://vf.haigaiapp.cn

fun String.exclaim() = this + "!"
来源：http://nb.huixiangedu.cn

[T10] Kotlin：默认参数
来源：http://ym.shxzskj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xc.shtwfgs.cn

[T11] Kotlin：协程
来源：http://tf.chemitech.net.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://eu.9csxet.cn

[T12] Kotlin：解构声明
来源：http://fk.huanxung.cn

val (a, b) = Pair(1, 2)
来源：http://ip.bjjhwx.cn

[T13] Kotlin：只读 Map
来源：http://ge.wgjwhj.cn

val m = mapOf("a" to 1)
来源：http://pi.shtwfgs.cn

[T14] Kotlin：循环
来源：http://ev.jctech888.com.cn

for (i in 1..10) println(i)
来源：http://ey.nicolike.cn

[T15] Kotlin：接口
来源：http://kl.shtwfgs.cn

interface Shape { fun area(): Double }
来源：http://zv.521024.cn

[T16] Swift：Hello World
来源：http://am.jctech888.com.cn

print("Hello")
来源：http://qn.szsharing.cn

[T17] Swift：变量与常量
来源：http://or.huixiangedu.cn

var a = 1;  let b = 2
来源：http://vv.asd995.cn

[T18] Swift：字符串插值
来源：http://ln.bjjhwx.cn

"值: \(b)"
来源：http://jh.muxihuayi.cn

[T19] Swift：可选绑定
来源：http://bw.shxzukj.cn

if let n = opt { print(n) }
来源：http://vs.shtwfgs.cn

[T20] Swift：数组操作
来源：http://hb.lnxyls.cn

var a = [1, 2, 3];  a.append(4)
来源：http://lj.newstarts.cn

[T21] Swift：遍历
来源：http://sh.hnjuh.cn

for x in a { print(x) }
来源：http://ce.szxytkj.cn

[T22] Swift：字典
来源：http://cu.yuexingan06.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fp.newstarts.cn

[T23] Swift：函数
来源：http://ek.jctech888.com.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bw.huixinmuqiang.cn

[T24] Swift：闭包
来源：http://tc.nicolike.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://mq.bookmarksfly.cn

[T25] Swift：结构体
来源：http://cx.chemitech.net.cn

struct P { var x: Int }
来源：http://da.szxytkj.cn

[T26] Swift：类与重写
来源：http://nv.lnxyls.cn

class A: Base { override func f() {} }
来源：http://qw.521024.cn

[T27] Swift：错误处理
来源：http://td.bjjhwx.cn

do { try f() } catch { print(error) }
来源：http://nu.jianghongdianzi.cn

[T28] Swift：枚举
来源：http://gu.9csxet.cn

enum Color { case red, green }
来源：http://xz.bookmarksfly.cn

[T29] Swift：guard 提前返回
来源：http://jy.haigaiapp.cn

guard let x = opt else { return }
来源：http://oj.asd995.cn

[T30] Swift：协议
来源：http://ls.newstarts.cn

protocol Shape { func area() -> Double }
来源：http://rb.muxihuayi.cn

[T31] Lua：Hello World
来源：http://sq.gzmigu.cn

print("Hello")
来源：http://qv.panjiajie.cn

[T32] Lua：局部变量
来源：http://ik.haigaiapp.cn

local a = 1
来源：http://dh.jianghongdianzi.cn

[T33] Lua：表（数组）
来源：http://yv.huixiangedu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://yy.huixiangedu.cn

[T34] Lua：遍历表
来源：http://zb.bookmarksfly.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qn.huixiangedu.cn

[T35] Lua：字典表
来源：http://yg.gzmigu.cn

local d = { a = 1 };  d.b = 2
来源：http://bh.bookmarksfly.cn

[T36] Lua：函数
来源：http://lw.hnjuh.cn

function add(a, b) return a + b end
来源：http://jv.huixinmuqiang.cn

[T37] Lua：字符串拼接
来源：http://rl.muxihuayi.cn

"a" .. "b"
来源：http://yu.shxzukj.cn

[T38] Lua：条件
来源：http://sj.chemitech.net.cn

if x > 0 then print("正") end
来源：http://hv.lnxyls.cn

[T39] Lua：模式匹配
来源：http://vd.panjiajie.cn

string.find(s, "%d+")
来源：http://hb.szsharing.cn

[T40] Lua：元表
来源：http://fm.jianghongdianzi.cn

setmetatable({}, { __index = base })
来源：http://vo.yuexingan06.cn

[T41] Perl：Hello World
来源：http://ev.wgjwhj.cn

print "Hello\n";
来源：http://kv.shtwfgs.cn

[T42] Perl：变量类型
来源：http://ub.panjiajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fr.9csxet.cn

[T43] Perl：字符串插值
来源：http://gg.jianghongdianzi.cn

"值: $a"
来源：http://td.lnxyls.cn

[T44] Perl：条件
来源：http://ow.haigaiapp.cn

if ($a > 0) { print "正"; }
来源：http://up.bookmarksfly.cn

[T45] Perl：数组遍历
来源：http://ic.nicolike.cn

for my $x (@arr) { print $x; }
来源：http://rb.asd995.cn

[T46] Perl：哈希操作
来源：http://lf.wgjwhj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ww.shtwfgs.cn

[T47] Perl：正则捕获
来源：http://ng.521024.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://do.asd995.cn

[T48] Perl：正则替换
来源：http://ls.panjiajie.cn

$s =~ s/old/new/g;
来源：http://vy.lnxyls.cn

[T49] Perl：函数
来源：http://hr.panjiajie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bg.haigaiapp.cn

[T50] Perl：逐行读文件
来源：http://jd.bjjhwx.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zw.asd995.cn

while (my $line = <$fh>) { print $line; }
来源：http://mn.shxzskj.cn

[T51] Scala：Hello World
来源：http://wk.bookmarksfly.cn

println("Hello")
来源：http://tw.hnjuh.cn

[T52] Scala：变量
来源：http://yl.shtwfgs.cn

val a = 1;  var b = 2
来源：http://gk.gzmigu.cn

[T53] Scala：字符串插值
来源：http://wf.huixinmuqiang.cn

s"值: $b"
来源：http://eg.huixiangedu.cn

[T54] Scala：集合映射
来源：http://dt.9csxet.cn

List(1, 2, 3).map(_ * 2)
来源：http://gp.9csxet.cn

[T55] Scala：集合过滤
来源：http://ia.haigaiapp.cn

List(1, 2, 3).filter(_ > 1)
来源：http://md.shxzskj.cn

[T56] Scala：样例类
来源：http://qk.jctech888.com.cn

case class User(name: String, age: Int)
来源：http://cc.szsharing.cn

[T57] Scala：模式匹配
来源：http://ba.colortex.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://xq.bjjhwx.cn

[T58] Scala：函数定义
来源：http://ly.muxihuayi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ga.asd995.cn

[T59] Scala：循环
来源：http://ve.gzmigu.cn

for (i <- 1 to 10) println(i)
来源：http://me.huixinmuqiang.cn

[T60] Scala：折叠
来源：http://gm.szsharing.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dv.bjjhwx.cn

================================================================================
来源：http://ye.gzmigu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ob.colortex.cn

================================================================================
来源：http://qu.haigaiapp.cn

[U01] Py：创建虚拟环境
来源：http://pf.asd995.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ny.asd995.cn

[U02] Py：导出 / 安装依赖
来源：http://ff.yuntaijiaju.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ng.shxzskj.cn

[U03] Py：加载 .env 配置
来源：http://ni.9csxet.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://lh.panjiajie.cn

[U04] Py：变量调试打印
来源：http://hb.gzmigu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sr.hahajie.cn

[U05] Py：列表去重且保序
来源：http://oq.huixinmuqiang.cn

list(dict.fromkeys(arr))
来源：http://sq.shtwfgs.cn

[U06] Py：合并两个字典
来源：http://jk.haigaiapp.cn

{**a, **b}
来源：http://uy.shtwfgs.cn

[U07] Py：反转字典键值
来源：http://zh.bookmarksfly.cn

{v: k for k, v in d.items()}
来源：http://dj.huixinmuqiang.cn

[U08] Py：展平二维列表
来源：http://ox.shtwfgs.cn

[y for x in nested for y in x]
来源：http://uu.521024.cn

[U09] Py：字典取最大值的键
来源：http://cv.yuexingan06.cn

max(d, key=d.get)
来源：http://fq.wgjwhj.cn

[U10] Py：按值排序字典
来源：http://nz.muxihuayi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ju.haigaiapp.cn

[U11] Py：生成器表达式
来源：http://ro.yuntaijiaju.cn

(x * 2 for x in arr)
来源：http://tx.haigaiapp.cn

[U12] Py：取出现最多的 3 个元素
来源：http://oz.haigaiapp.cn

Counter(arr).most_common(3)
来源：http://ss.chemitech.net.cn

[U13] Py：固定长度队列
来源：http://xg.szsharing.cn

deque(maxlen=10)
来源：http://xs.colortex.cn

[U14] Py：分组收集到列表
来源：http://so.wgjwhj.cn

defaultdict(list)
来源：http://jl.lnxyls.cn

[U15] Py：高精度计时
来源：http://cr.panjiajie.cn

t = time.perf_counter()
来源：http://mg.lnxyls.cn

[U16] Py：命令行参数解析
来源：http://xb.bookmarksfly.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mr.asd995.cn

[U17] Py：初始化日志
来源：http://zp.haigaiapp.cn

logging.basicConfig(level=logging.INFO)
来源：http://qc.chemitech.net.cn

[U18] Py：预编译正则
来源：http://xf.huixiangedu.cn

pat = re.compile(r"\d+")
来源：http://dq.shxzukj.cn

[U19] Py：正则替换带回调
来源：http://vu.jctech888.com.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zn.haigaiapp.cn

[U20] Py：缓存函数结果
来源：http://ji.hnjuh.cn

@functools.lru_cache(maxsize=None)
来源：http://eb.9csxet.cn

[U21] Py：自定义上下文管理器
来源：http://qc.huanxung.cn

@contextlib.contextmanager
来源：http://ya.jianghongdianzi.cn

[U22] Py：矩阵转置
来源：http://gy.muxihuayi.cn

list(zip(*m))
来源：http://by.shxzukj.cn

[U23] Py：分块读取大文件
来源：http://mn.panjiajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://us.nszjky.cn

[U24] Py：路径操作
来源：http://du.asd995.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fx.nszjky.cn

[U25] Py：CSV 按字典读
来源：http://xk.lnxyls.cn

csv.DictReader(f)
来源：http://wi.hnjuh.cn

[U26] Py：并发下载
来源：http://rm.huanxung.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mv.muxihuayi.cn

[U27] Py：异步 HTTP
来源：http://yy.yuntaijiaju.cn

aiohttp.ClientSession() 配合 async with
来源：http://jm.wgjwhj.cn

[U28] Py：类型别名
来源：http://gw.521024.cn

UserId = int
来源：http://qu.9csxet.cn

[U29] Py：属性校验
来源：http://is.huixiangedu.cn

@property 与 @x.setter 配合
来源：http://td.shtwfgs.cn

[U30] Py：数据类
来源：http://fc.hnjuh.cn

@dataclass(slots=True)
来源：http://sw.yuntaijiaju.cn


<!-- 参考信息 -->