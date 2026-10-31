代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ag.haigaiapp.cn

[S08] C：动态内存分配与释放
来源：http://qv.hnjuh.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bv.bookmarksfly.cn

[S09] C：结构体定义与初始化
来源：http://oh.newstarts.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uj.lnxyls.cn

[S10] C：指针与解引用
来源：http://na.shtwfgs.cn

int *p = &a;  *p = 5;
来源：http://kc.jianghongdianzi.cn

[S11] C：逐行读文件
来源：http://cm.gzmigu.cn

FILE *f = fopen("a.txt", "r");
来源：http://ep.9csxet.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hs.shxzukj.cn

fclose(f);
来源：http://ds.hnjuh.cn

[S12] C：写文件
来源：http://mm.colortex.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rj.bookmarksfly.cn

[S13] C：宏定义
来源：http://cu.asd995.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://aq.lnxyls.cn

[S14] C：枚举
来源：http://vc.muxihuayi.cn

enum Color { RED, GREEN, BLUE };
来源：http://tg.chemitech.net.cn

[S15] C：类型转换
来源：http://kf.bookmarksfly.cn

(double) a / b
来源：http://dr.szxytkj.cn

[S16] C：位操作置位
来源：http://qo.jianghongdianzi.cn

x |= (1 << 3);
来源：http://vo.huixiangedu.cn

[S17] C：安全拼接字符串
来源：http://ht.shxzukj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mx.lnxyls.cn

[S18] C：命令行参数
来源：http://ms.huixiangedu.cn

int main(int argc, char **argv)
来源：http://wb.shxzukj.cn

[S19] C：快速排序
来源：http://gy.wgjwhj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://pm.9csxet.cn

[S20] C：二分查找
来源：http://lx.szxytkj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://in.huanxung.cn

[S21] C：字符类别判断
来源：http://um.nicolike.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ju.huanxung.cn

[S22] C：字符串转数字
来源：http://vt.hahajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://pb.newstarts.cn

[S23] C：随机数
来源：http://ch.gzmigu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://tt.huixinmuqiang.cn

[S24] C：获取本地时间
来源：http://vk.jctech888.com.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uo.lnxyls.cn

[S25] C：内存拷贝
来源：http://bq.yuntaijiaju.cn

memcpy(dst, src, n);
来源：http://km.yuexingan06.cn

[S26] C：内存清零
来源：http://wz.wgjwhj.cn

memset(a, 0, sizeof a);
来源：http://qc.wgjwhj.cn

[S27] C：定义常量
来源：http://xc.9csxet.cn

const double PI = 3.14159;
来源：http://tl.shtwfgs.cn

[S28] C：静态变量
来源：http://ag.wgjwhj.cn

static int counter = 0;
来源：http://vl.hahajie.cn

[S29] C：变参函数
来源：http://dd.bjjhwx.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ct.chemitech.net.cn

[S30] C：头文件保护
来源：http://vo.huanxung.cn

#ifndef X_H
来源：http://ij.wgjwhj.cn

#define X_H
来源：http://ra.jctech888.com.cn

#endif
来源：http://ys.huixiangedu.cn

[S31] C++：Hello World
来源：http://xe.szxytkj.cn

#include <iostream>
来源：http://xn.hnjuh.cn

int main() { std::cout << "Hello\n"; }
来源：http://ua.panjiajie.cn

[S32] C++：字符串
来源：http://js.chemitech.net.cn

std::string s = "hi";  s += "!";
来源：http://nv.muxihuayi.cn

[S33] C++：vector 增删
来源：http://ip.hnjuh.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wv.shxzukj.cn

[S34] C++：遍历 vector
来源：http://iw.jianghongdianzi.cn

for (auto &x : v) { std::cout << x; }
来源：http://vq.colortex.cn

[S35] C++：map
来源：http://ec.lnxyls.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kx.lnxyls.cn

[S36] C++：unordered_map
来源：http://mv.yuexingan06.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ao.hahajie.cn

[S37] C++：set
来源：http://eo.nszjky.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://le.bjjhwx.cn

[S38] C++：排序
来源：http://sn.panjiajie.cn

std::sort(v.begin(), v.end());
来源：http://ay.haigaiapp.cn

[S39] C++：自定义比较器排序
来源：http://tu.521024.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://au.huanxung.cn

[S40] C++：查找元素
来源：http://bj.muxihuayi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dn.jianghongdianzi.cn

[S41] C++：类与构造函数
来源：http://ij.nszjky.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rh.bookmarksfly.cn

[S42] C++：继承与虚函数
来源：http://ck.szxytkj.cn

class B : public Base { public: void f() override {} };
来源：http://io.bjjhwx.cn

[S43] C++：智能指针
来源：http://pn.chemitech.net.cn

auto p = std::make_unique<int>(5);
来源：http://ay.hahajie.cn

[S44] C++：引用传参
来源：http://sf.nszjky.cn

void inc(int &x) { ++x; }
来源：http://vc.jianghongdianzi.cn

[S45] C++：lambda
来源：http://ai.shxzskj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ox.9csxet.cn

[S46] C++：函数模板
来源：http://jw.hahajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zk.colortex.cn

[S47] C++：结构化绑定遍历
来源：http://ae.muxihuayi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ht.nszjky.cn

[S48] C++：逐行读文件
来源：http://nr.521024.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pb.shxzskj.cn

while (std::getline(in, line)) { }
来源：http://ig.nszjky.cn

[S49] C++：写文件
来源：http://so.shxzukj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sp.wgjwhj.cn

[S50] C++：格式化数字
来源：http://fl.wgjwhj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cc.newstarts.cn

[S51] C++：显式类型转换
来源：http://yq.shxzskj.cn

static_cast<double>(a) / b
来源：http://kv.colortex.cn

[S52] C++：const 与 noexcept
来源：http://vq.shxzukj.cn

int size() const noexcept { return n_; }
来源：http://dl.hahajie.cn

[S53] C++：移动语义
来源：http://du.hnjuh.cn

std::vector<int> w = std::move(v);
来源：http://px.hahajie.cn

[S54] C++：异常处理
来源：http://bf.panjiajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lu.jctech888.com.cn

[S55] C++：结构化绑定
来源：http://fy.nszjky.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://de.panjiajie.cn

[S56] C++：optional
来源：http://of.huixiangedu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://oo.huixinmuqiang.cn

[S57] C++：编译期常量
来源：http://wa.bjjhwx.cn

constexpr int N = 10;
来源：http://pa.huixinmuqiang.cn

[S58] C++：命名空间
来源：http://fu.jctech888.com.cn

namespace ns { int f() { return 1; } }
来源：http://go.shxzskj.cn

[S59] C++：静态断言
来源：http://ob.521024.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gf.colortex.cn

[S60] C++：遍历并删除元素
来源：http://ur.newstarts.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nl.huixinmuqiang.cn

================================================================================
来源：http://bm.haigaiapp.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ys.chemitech.net.cn

================================================================================
来源：http://pl.nicolike.cn

[T01] Kotlin：Hello World
来源：http://bm.shtwfgs.cn

println("Hello")
来源：http://xw.muxihuayi.cn

[T02] Kotlin：变量
来源：http://yt.colortex.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wk.huanxung.cn

[T03] Kotlin：字符串模板
来源：http://oy.jianghongdianzi.cn

"值: $b"
来源：http://rz.haigaiapp.cn

[T04] Kotlin：空安全
来源：http://dt.panjiajie.cn

val n: String? = null;  n?.length
来源：http://kd.colortex.cn

[T05] Kotlin：when 表达式
来源：http://im.hnjuh.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://oe.colortex.cn

[T06] Kotlin：集合映射
来源：http://ia.wgjwhj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xc.shxzukj.cn

[T07] Kotlin：集合过滤
来源：http://gk.jctech888.com.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xv.newstarts.cn

[T08] Kotlin：数据类
来源：http://lz.colortex.cn

data class User(val name: String, val age: Int)
来源：http://eu.yuntaijiaju.cn

[T09] Kotlin：扩展函数
来源：http://ty.muxihuayi.cn

fun String.exclaim() = this + "!"
来源：http://mp.jctech888.com.cn

[T10] Kotlin：默认参数
来源：http://ud.panjiajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://cf.yuexingan06.cn

[T11] Kotlin：协程
来源：http://gh.nszjky.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qj.521024.cn

[T12] Kotlin：解构声明
来源：http://lf.panjiajie.cn

val (a, b) = Pair(1, 2)
来源：http://qf.huanxung.cn

[T13] Kotlin：只读 Map
来源：http://yl.huixiangedu.cn

val m = mapOf("a" to 1)
来源：http://rh.hnjuh.cn

[T14] Kotlin：循环
来源：http://dh.shtwfgs.cn

for (i in 1..10) println(i)
来源：http://vp.huanxung.cn

[T15] Kotlin：接口
来源：http://ip.shxzukj.cn

interface Shape { fun area(): Double }
来源：http://zv.lnxyls.cn

[T16] Swift：Hello World
来源：http://tk.chemitech.net.cn

print("Hello")
来源：http://dz.wgjwhj.cn

[T17] Swift：变量与常量
来源：http://om.nicolike.cn

var a = 1;  let b = 2
来源：http://qp.521024.cn

[T18] Swift：字符串插值
来源：http://um.521024.cn

"值: \(b)"
来源：http://zd.hnjuh.cn

[T19] Swift：可选绑定
来源：http://fa.haigaiapp.cn

if let n = opt { print(n) }
来源：http://zh.huixinmuqiang.cn

[T20] Swift：数组操作
来源：http://zq.shtwfgs.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hu.nicolike.cn

[T21] Swift：遍历
来源：http://gq.9csxet.cn

for x in a { print(x) }
来源：http://tt.newstarts.cn

[T22] Swift：字典
来源：http://sg.huixiangedu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fg.panjiajie.cn

[T23] Swift：函数
来源：http://or.9csxet.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yx.yuntaijiaju.cn

[T24] Swift：闭包
来源：http://tj.huanxung.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://fg.huixinmuqiang.cn

[T25] Swift：结构体
来源：http://mc.nicolike.cn

struct P { var x: Int }
来源：http://zm.nicolike.cn

[T26] Swift：类与重写
来源：http://ke.bjjhwx.cn

class A: Base { override func f() {} }
来源：http://hq.shtwfgs.cn

[T27] Swift：错误处理
来源：http://vl.nszjky.cn

do { try f() } catch { print(error) }
来源：http://io.521024.cn

[T28] Swift：枚举
来源：http://ks.haigaiapp.cn

enum Color { case red, green }
来源：http://ah.bookmarksfly.cn

[T29] Swift：guard 提前返回
来源：http://oe.newstarts.cn

guard let x = opt else { return }
来源：http://mg.9csxet.cn

[T30] Swift：协议
来源：http://ey.huanxung.cn

protocol Shape { func area() -> Double }
来源：http://bu.9csxet.cn

[T31] Lua：Hello World
来源：http://eo.asd995.cn

print("Hello")
来源：http://vr.haigaiapp.cn

[T32] Lua：局部变量
来源：http://pc.nicolike.cn

local a = 1
来源：http://ow.huixinmuqiang.cn

[T33] Lua：表（数组）
来源：http://ts.hnjuh.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ae.huanxung.cn

[T34] Lua：遍历表
来源：http://jm.gzmigu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rl.muxihuayi.cn

[T35] Lua：字典表
来源：http://ho.lnxyls.cn

local d = { a = 1 };  d.b = 2
来源：http://gw.yuexingan06.cn

[T36] Lua：函数
来源：http://yo.hnjuh.cn

function add(a, b) return a + b end
来源：http://kb.huanxung.cn

[T37] Lua：字符串拼接
来源：http://bv.jctech888.com.cn

"a" .. "b"
来源：http://xv.shxzskj.cn

[T38] Lua：条件
来源：http://ij.shxzskj.cn

if x > 0 then print("正") end
来源：http://tj.panjiajie.cn

[T39] Lua：模式匹配
来源：http://jj.hnjuh.cn

string.find(s, "%d+")
来源：http://bw.hnjuh.cn

[T40] Lua：元表
来源：http://zy.muxihuayi.cn

setmetatable({}, { __index = base })
来源：http://ni.panjiajie.cn

[T41] Perl：Hello World
来源：http://nq.yuntaijiaju.cn

print "Hello\n";
来源：http://yp.yuexingan06.cn

[T42] Perl：变量类型
来源：http://oj.bjjhwx.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rv.haigaiapp.cn

[T43] Perl：字符串插值
来源：http://ub.panjiajie.cn

"值: $a"
来源：http://pz.bookmarksfly.cn

[T44] Perl：条件
来源：http://at.bjjhwx.cn

if ($a > 0) { print "正"; }
来源：http://la.szsharing.cn

[T45] Perl：数组遍历
来源：http://sq.nicolike.cn

for my $x (@arr) { print $x; }
来源：http://cp.shxzukj.cn

[T46] Perl：哈希操作
来源：http://pe.9csxet.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kp.hnjuh.cn

[T47] Perl：正则捕获
来源：http://xz.bjjhwx.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://zt.yuexingan06.cn

[T48] Perl：正则替换
来源：http://rq.bjjhwx.cn

$s =~ s/old/new/g;
来源：http://pc.colortex.cn

[T49] Perl：函数
来源：http://ye.bookmarksfly.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lc.nicolike.cn

[T50] Perl：逐行读文件
来源：http://fy.yuntaijiaju.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://mh.jianghongdianzi.cn

while (my $line = <$fh>) { print $line; }
来源：http://in.wgjwhj.cn

[T51] Scala：Hello World
来源：http://le.jianghongdianzi.cn

println("Hello")
来源：http://is.bjjhwx.cn

[T52] Scala：变量
来源：http://vu.szsharing.cn

val a = 1;  var b = 2
来源：http://ik.szsharing.cn

[T53] Scala：字符串插值
来源：http://sb.newstarts.cn

s"值: $b"
来源：http://rp.jianghongdianzi.cn

[T54] Scala：集合映射
来源：http://xw.muxihuayi.cn

List(1, 2, 3).map(_ * 2)
来源：http://vk.yuexingan06.cn

[T55] Scala：集合过滤
来源：http://ui.shtwfgs.cn

List(1, 2, 3).filter(_ > 1)
来源：http://lf.muxihuayi.cn

[T56] Scala：样例类
来源：http://ri.yuntaijiaju.cn

case class User(name: String, age: Int)
来源：http://zp.asd995.cn

[T57] Scala：模式匹配
来源：http://tf.jianghongdianzi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://mp.wgjwhj.cn

[T58] Scala：函数定义
来源：http://gn.huixinmuqiang.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bm.haigaiapp.cn

[T59] Scala：循环
来源：http://mw.nszjky.cn

for (i <- 1 to 10) println(i)
来源：http://hj.newstarts.cn

[T60] Scala：折叠
来源：http://ow.colortex.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://uq.muxihuayi.cn

================================================================================
来源：http://go.hahajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pa.panjiajie.cn

================================================================================
来源：http://nv.521024.cn

[U01] Py：创建虚拟环境
来源：http://lo.nicolike.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jq.shxzskj.cn

[U02] Py：导出 / 安装依赖
来源：http://wt.nicolike.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://sf.jctech888.com.cn

[U03] Py：加载 .env 配置
来源：http://lf.huixiangedu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ar.huanxung.cn

[U04] Py：变量调试打印
来源：http://yl.lnxyls.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tt.gzmigu.cn

[U05] Py：列表去重且保序
来源：http://tc.newstarts.cn

list(dict.fromkeys(arr))
来源：http://pg.muxihuayi.cn

[U06] Py：合并两个字典
来源：http://dr.bookmarksfly.cn

{**a, **b}
来源：http://md.asd995.cn

[U07] Py：反转字典键值
来源：http://ni.bjjhwx.cn

{v: k for k, v in d.items()}
来源：http://fw.muxihuayi.cn

[U08] Py：展平二维列表
来源：http://fq.chemitech.net.cn

[y for x in nested for y in x]
来源：http://pf.yuexingan06.cn

[U09] Py：字典取最大值的键
来源：http://pl.lnxyls.cn

max(d, key=d.get)
来源：http://rh.yuexingan06.cn

[U10] Py：按值排序字典
来源：http://ca.asd995.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ti.hahajie.cn

[U11] Py：生成器表达式
来源：http://bw.bookmarksfly.cn

(x * 2 for x in arr)
来源：http://qo.521024.cn

[U12] Py：取出现最多的 3 个元素
来源：http://yp.wgjwhj.cn

Counter(arr).most_common(3)
来源：http://sv.panjiajie.cn

[U13] Py：固定长度队列
来源：http://tb.nszjky.cn

deque(maxlen=10)
来源：http://ch.chemitech.net.cn

[U14] Py：分组收集到列表
来源：http://fo.chemitech.net.cn

defaultdict(list)
来源：http://ie.panjiajie.cn

[U15] Py：高精度计时
来源：http://xy.huanxung.cn

t = time.perf_counter()
来源：http://hq.bookmarksfly.cn

[U16] Py：命令行参数解析
来源：http://jl.shxzskj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dx.haigaiapp.cn

[U17] Py：初始化日志
来源：http://yz.huixinmuqiang.cn

logging.basicConfig(level=logging.INFO)
来源：http://xi.hnjuh.cn

[U18] Py：预编译正则
来源：http://ds.shtwfgs.cn

pat = re.compile(r"\d+")
来源：http://kb.nszjky.cn

[U19] Py：正则替换带回调
来源：http://up.huixiangedu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nv.gzmigu.cn

[U20] Py：缓存函数结果
来源：http://cy.szxytkj.cn

@functools.lru_cache(maxsize=None)
来源：http://ad.newstarts.cn

[U21] Py：自定义上下文管理器
来源：http://ji.yuexingan06.cn

@contextlib.contextmanager
来源：http://vh.wgjwhj.cn

[U22] Py：矩阵转置
来源：http://qy.huixiangedu.cn

list(zip(*m))
来源：http://km.chemitech.net.cn

[U23] Py：分块读取大文件
来源：http://xf.bjjhwx.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qk.nszjky.cn

[U24] Py：路径操作
来源：http://jr.shtwfgs.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zj.bookmarksfly.cn

[U25] Py：CSV 按字典读
来源：http://ha.newstarts.cn

csv.DictReader(f)
来源：http://hl.colortex.cn

[U26] Py：并发下载
来源：http://lg.huixinmuqiang.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cd.huixiangedu.cn

[U27] Py：异步 HTTP
来源：http://fr.hahajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://sv.szxytkj.cn

[U28] Py：类型别名
来源：http://wv.bjjhwx.cn

UserId = int
来源：http://je.lnxyls.cn

[U29] Py：属性校验
来源：http://cl.shxzukj.cn

@property 与 @x.setter 配合
来源：http://qc.haigaiapp.cn

[U30] Py：数据类
来源：http://ij.wgjwhj.cn

@dataclass(slots=True)
来源：http://km.huixinmuqiang.cn


<!-- 参考信息 -->