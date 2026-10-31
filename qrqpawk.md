代发 wailian999

int x; scanf("%d", &x);
来源：http://xl.muxihuayi.cn

[S04] C：字符串复制
来源：http://lr.bookmarksfly.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rg.hahajie.cn

[S05] C：字符串长度
来源：http://uo.panjiajie.cn

strlen(s)
来源：http://cv.jianghongdianzi.cn

[S06] C：字符串比较
来源：http://wg.muxihuayi.cn

strcmp(a, b) == 0
来源：http://wa.hahajie.cn

[S07] C：数组遍历求和
来源：http://ux.521024.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yd.jianghongdianzi.cn

[S08] C：动态内存分配与释放
来源：http://na.hnjuh.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sw.nicolike.cn

[S09] C：结构体定义与初始化
来源：http://xz.9csxet.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gy.hnjuh.cn

[S10] C：指针与解引用
来源：http://xj.hahajie.cn

int *p = &a;  *p = 5;
来源：http://mh.shtwfgs.cn

[S11] C：逐行读文件
来源：http://vt.521024.cn

FILE *f = fopen("a.txt", "r");
来源：http://dg.9csxet.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zu.asd995.cn

fclose(f);
来源：http://bo.nicolike.cn

[S12] C：写文件
来源：http://mc.huanxung.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://um.wgjwhj.cn

[S13] C：宏定义
来源：http://fz.bookmarksfly.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tj.yuntaijiaju.cn

[S14] C：枚举
来源：http://bc.huixiangedu.cn

enum Color { RED, GREEN, BLUE };
来源：http://sg.bjjhwx.cn

[S15] C：类型转换
来源：http://ta.yuexingan06.cn

(double) a / b
来源：http://od.9csxet.cn

[S16] C：位操作置位
来源：http://ss.haigaiapp.cn

x |= (1 << 3);
来源：http://rg.haigaiapp.cn

[S17] C：安全拼接字符串
来源：http://kg.colortex.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ap.jctech888.com.cn

[S18] C：命令行参数
来源：http://ke.muxihuayi.cn

int main(int argc, char **argv)
来源：http://oc.chemitech.net.cn

[S19] C：快速排序
来源：http://ff.yuntaijiaju.cn

qsort(a, n, sizeof(int), cmp);
来源：http://su.nszjky.cn

[S20] C：二分查找
来源：http://wr.newstarts.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zn.shxzskj.cn

[S21] C：字符类别判断
来源：http://nj.haigaiapp.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ej.shxzukj.cn

[S22] C：字符串转数字
来源：http://tr.9csxet.cn

atoi("42");  strtod("3.14", NULL);
来源：http://lf.bookmarksfly.cn

[S23] C：随机数
来源：http://dy.wgjwhj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rb.nszjky.cn

[S24] C：获取本地时间
来源：http://mu.szxytkj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gt.yuntaijiaju.cn

[S25] C：内存拷贝
来源：http://dz.asd995.cn

memcpy(dst, src, n);
来源：http://ow.hnjuh.cn

[S26] C：内存清零
来源：http://nn.wgjwhj.cn

memset(a, 0, sizeof a);
来源：http://hu.hnjuh.cn

[S27] C：定义常量
来源：http://ep.huixinmuqiang.cn

const double PI = 3.14159;
来源：http://jp.shtwfgs.cn

[S28] C：静态变量
来源：http://ac.jctech888.com.cn

static int counter = 0;
来源：http://xy.chemitech.net.cn

[S29] C：变参函数
来源：http://sn.wgjwhj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pd.colortex.cn

[S30] C：头文件保护
来源：http://bp.huanxung.cn

#ifndef X_H
来源：http://qk.huixinmuqiang.cn

#define X_H
来源：http://zv.gzmigu.cn

#endif
来源：http://hp.521024.cn

[S31] C++：Hello World
来源：http://vw.9csxet.cn

#include <iostream>
来源：http://lj.huixiangedu.cn

int main() { std::cout << "Hello\n"; }
来源：http://jk.panjiajie.cn

[S32] C++：字符串
来源：http://wf.bjjhwx.cn

std::string s = "hi";  s += "!";
来源：http://vc.bjjhwx.cn

[S33] C++：vector 增删
来源：http://js.yuexingan06.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gg.jctech888.com.cn

[S34] C++：遍历 vector
来源：http://lk.szxytkj.cn

for (auto &x : v) { std::cout << x; }
来源：http://ae.haigaiapp.cn

[S35] C++：map
来源：http://ve.521024.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://og.jianghongdianzi.cn

[S36] C++：unordered_map
来源：http://tg.gzmigu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tg.szxytkj.cn

[S37] C++：set
来源：http://ro.nicolike.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hi.shxzukj.cn

[S38] C++：排序
来源：http://zc.yuntaijiaju.cn

std::sort(v.begin(), v.end());
来源：http://td.newstarts.cn

[S39] C++：自定义比较器排序
来源：http://iy.huanxung.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tp.hnjuh.cn

[S40] C++：查找元素
来源：http://ko.shtwfgs.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qd.jianghongdianzi.cn

[S41] C++：类与构造函数
来源：http://ys.jianghongdianzi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ap.bookmarksfly.cn

[S42] C++：继承与虚函数
来源：http://wt.muxihuayi.cn

class B : public Base { public: void f() override {} };
来源：http://wv.bookmarksfly.cn

[S43] C++：智能指针
来源：http://mg.newstarts.cn

auto p = std::make_unique<int>(5);
来源：http://da.gzmigu.cn

[S44] C++：引用传参
来源：http://ou.jianghongdianzi.cn

void inc(int &x) { ++x; }
来源：http://fi.huanxung.cn

[S45] C++：lambda
来源：http://iz.shxzskj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://oh.521024.cn

[S46] C++：函数模板
来源：http://bj.huixinmuqiang.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tp.yuntaijiaju.cn

[S47] C++：结构化绑定遍历
来源：http://tu.panjiajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qy.shxzskj.cn

[S48] C++：逐行读文件
来源：http://he.muxihuayi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ci.hnjuh.cn

while (std::getline(in, line)) { }
来源：http://dn.panjiajie.cn

[S49] C++：写文件
来源：http://dg.colortex.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xe.huixinmuqiang.cn

[S50] C++：格式化数字
来源：http://ue.nszjky.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ga.huanxung.cn

[S51] C++：显式类型转换
来源：http://cp.huixiangedu.cn

static_cast<double>(a) / b
来源：http://ud.jianghongdianzi.cn

[S52] C++：const 与 noexcept
来源：http://aj.szsharing.cn

int size() const noexcept { return n_; }
来源：http://bp.521024.cn

[S53] C++：移动语义
来源：http://xb.bookmarksfly.cn

std::vector<int> w = std::move(v);
来源：http://yx.jctech888.com.cn

[S54] C++：异常处理
来源：http://oq.shxzskj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fv.szxytkj.cn

[S55] C++：结构化绑定
来源：http://fx.haigaiapp.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://oc.shtwfgs.cn

[S56] C++：optional
来源：http://jl.szxytkj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ee.colortex.cn

[S57] C++：编译期常量
来源：http://et.yuntaijiaju.cn

constexpr int N = 10;
来源：http://mt.panjiajie.cn

[S58] C++：命名空间
来源：http://bn.huixiangedu.cn

namespace ns { int f() { return 1; } }
来源：http://nv.521024.cn

[S59] C++：静态断言
来源：http://lc.wgjwhj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://oc.huixinmuqiang.cn

[S60] C++：遍历并删除元素
来源：http://bk.gzmigu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kc.szxytkj.cn

================================================================================
来源：http://qm.newstarts.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xd.hnjuh.cn

================================================================================
来源：http://vh.gzmigu.cn

[T01] Kotlin：Hello World
来源：http://zn.panjiajie.cn

println("Hello")
来源：http://rd.shxzukj.cn

[T02] Kotlin：变量
来源：http://ix.shxzukj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pf.shxzskj.cn

[T03] Kotlin：字符串模板
来源：http://jd.newstarts.cn

"值: $b"
来源：http://au.haigaiapp.cn

[T04] Kotlin：空安全
来源：http://ng.colortex.cn

val n: String? = null;  n?.length
来源：http://uk.muxihuayi.cn

[T05] Kotlin：when 表达式
来源：http://bv.lnxyls.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://aq.szsharing.cn

[T06] Kotlin：集合映射
来源：http://gp.chemitech.net.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ar.huanxung.cn

[T07] Kotlin：集合过滤
来源：http://fq.haigaiapp.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://cc.panjiajie.cn

[T08] Kotlin：数据类
来源：http://tp.521024.cn

data class User(val name: String, val age: Int)
来源：http://lz.panjiajie.cn

[T09] Kotlin：扩展函数
来源：http://gf.yuexingan06.cn

fun String.exclaim() = this + "!"
来源：http://ik.muxihuayi.cn

[T10] Kotlin：默认参数
来源：http://nx.huanxung.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gf.jctech888.com.cn

[T11] Kotlin：协程
来源：http://hv.nicolike.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://uw.bookmarksfly.cn

[T12] Kotlin：解构声明
来源：http://ey.shxzukj.cn

val (a, b) = Pair(1, 2)
来源：http://xl.szsharing.cn

[T13] Kotlin：只读 Map
来源：http://hi.yuntaijiaju.cn

val m = mapOf("a" to 1)
来源：http://tm.bjjhwx.cn

[T14] Kotlin：循环
来源：http://zj.newstarts.cn

for (i in 1..10) println(i)
来源：http://zy.haigaiapp.cn

[T15] Kotlin：接口
来源：http://bk.shxzukj.cn

interface Shape { fun area(): Double }
来源：http://qa.jctech888.com.cn

[T16] Swift：Hello World
来源：http://go.szxytkj.cn

print("Hello")
来源：http://sz.bookmarksfly.cn

[T17] Swift：变量与常量
来源：http://fb.yuntaijiaju.cn

var a = 1;  let b = 2
来源：http://ch.nszjky.cn

[T18] Swift：字符串插值
来源：http://sx.jianghongdianzi.cn

"值: \(b)"
来源：http://lw.521024.cn

[T19] Swift：可选绑定
来源：http://yd.shxzukj.cn

if let n = opt { print(n) }
来源：http://id.jianghongdianzi.cn

[T20] Swift：数组操作
来源：http://rg.9csxet.cn

var a = [1, 2, 3];  a.append(4)
来源：http://pr.wgjwhj.cn

[T21] Swift：遍历
来源：http://zd.shxzskj.cn

for x in a { print(x) }
来源：http://ra.shtwfgs.cn

[T22] Swift：字典
来源：http://ww.jctech888.com.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ru.jctech888.com.cn

[T23] Swift：函数
来源：http://tv.shtwfgs.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jz.bookmarksfly.cn

[T24] Swift：闭包
来源：http://mg.9csxet.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://so.huixiangedu.cn

[T25] Swift：结构体
来源：http://wt.asd995.cn

struct P { var x: Int }
来源：http://oh.asd995.cn

[T26] Swift：类与重写
来源：http://qk.huixinmuqiang.cn

class A: Base { override func f() {} }
来源：http://nu.haigaiapp.cn

[T27] Swift：错误处理
来源：http://be.asd995.cn

do { try f() } catch { print(error) }
来源：http://yw.panjiajie.cn

[T28] Swift：枚举
来源：http://mj.huixinmuqiang.cn

enum Color { case red, green }
来源：http://nz.szxytkj.cn

[T29] Swift：guard 提前返回
来源：http://oe.huixinmuqiang.cn

guard let x = opt else { return }
来源：http://gj.muxihuayi.cn

[T30] Swift：协议
来源：http://pb.shxzskj.cn

protocol Shape { func area() -> Double }
来源：http://kt.nszjky.cn

[T31] Lua：Hello World
来源：http://mj.muxihuayi.cn

print("Hello")
来源：http://iq.colortex.cn

[T32] Lua：局部变量
来源：http://rc.haigaiapp.cn

local a = 1
来源：http://ix.shtwfgs.cn

[T33] Lua：表（数组）
来源：http://km.hahajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ti.yuntaijiaju.cn

[T34] Lua：遍历表
来源：http://va.muxihuayi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://wy.lnxyls.cn

[T35] Lua：字典表
来源：http://pj.jianghongdianzi.cn

local d = { a = 1 };  d.b = 2
来源：http://pk.newstarts.cn

[T36] Lua：函数
来源：http://iq.shxzukj.cn

function add(a, b) return a + b end
来源：http://jh.asd995.cn

[T37] Lua：字符串拼接
来源：http://qu.bookmarksfly.cn

"a" .. "b"
来源：http://cx.yuexingan06.cn

[T38] Lua：条件
来源：http://vv.huixinmuqiang.cn

if x > 0 then print("正") end
来源：http://ik.lnxyls.cn

[T39] Lua：模式匹配
来源：http://fh.huixiangedu.cn

string.find(s, "%d+")
来源：http://xk.gzmigu.cn

[T40] Lua：元表
来源：http://gl.9csxet.cn

setmetatable({}, { __index = base })
来源：http://wr.colortex.cn

[T41] Perl：Hello World
来源：http://dh.shxzskj.cn

print "Hello\n";
来源：http://pp.yuntaijiaju.cn

[T42] Perl：变量类型
来源：http://ah.shtwfgs.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tt.huixiangedu.cn

[T43] Perl：字符串插值
来源：http://jj.shxzukj.cn

"值: $a"
来源：http://fk.shxzukj.cn

[T44] Perl：条件
来源：http://ml.muxihuayi.cn

if ($a > 0) { print "正"; }
来源：http://fm.nszjky.cn

[T45] Perl：数组遍历
来源：http://ek.huixinmuqiang.cn

for my $x (@arr) { print $x; }
来源：http://wt.huixiangedu.cn

[T46] Perl：哈希操作
来源：http://zd.wgjwhj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pt.panjiajie.cn

[T47] Perl：正则捕获
来源：http://nw.huixinmuqiang.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://cm.muxihuayi.cn

[T48] Perl：正则替换
来源：http://me.bookmarksfly.cn

$s =~ s/old/new/g;
来源：http://hx.huixinmuqiang.cn

[T49] Perl：函数
来源：http://mx.szxytkj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jn.shxzskj.cn

[T50] Perl：逐行读文件
来源：http://yv.9csxet.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://kl.yuexingan06.cn

while (my $line = <$fh>) { print $line; }
来源：http://tt.nszjky.cn

[T51] Scala：Hello World
来源：http://qz.huixiangedu.cn

println("Hello")
来源：http://sb.huixinmuqiang.cn

[T52] Scala：变量
来源：http://xr.lnxyls.cn

val a = 1;  var b = 2
来源：http://hf.wgjwhj.cn

[T53] Scala：字符串插值
来源：http://lc.wgjwhj.cn

s"值: $b"
来源：http://ti.muxihuayi.cn

[T54] Scala：集合映射
来源：http://oi.muxihuayi.cn

List(1, 2, 3).map(_ * 2)
来源：http://fb.shtwfgs.cn

[T55] Scala：集合过滤
来源：http://as.bjjhwx.cn

List(1, 2, 3).filter(_ > 1)
来源：http://me.yuntaijiaju.cn

[T56] Scala：样例类
来源：http://yo.panjiajie.cn

case class User(name: String, age: Int)
来源：http://bo.hahajie.cn

[T57] Scala：模式匹配
来源：http://ub.jctech888.com.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ix.muxihuayi.cn

[T58] Scala：函数定义
来源：http://pj.nszjky.cn

def add(a: Int, b: Int): Int = a + b
来源：http://mv.panjiajie.cn

[T59] Scala：循环
来源：http://gw.muxihuayi.cn

for (i <- 1 to 10) println(i)
来源：http://tv.huixinmuqiang.cn

[T60] Scala：折叠
来源：http://vs.haigaiapp.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://em.shtwfgs.cn

================================================================================
来源：http://yz.chemitech.net.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pq.nszjky.cn

================================================================================
来源：http://mv.wgjwhj.cn

[U01] Py：创建虚拟环境
来源：http://ue.szxytkj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mw.szxytkj.cn

[U02] Py：导出 / 安装依赖
来源：http://ka.huixiangedu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://az.muxihuayi.cn

[U03] Py：加载 .env 配置
来源：http://yk.huixiangedu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://uk.colortex.cn

[U04] Py：变量调试打印
来源：http://kr.newstarts.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ys.yuexingan06.cn

[U05] Py：列表去重且保序
来源：http://mu.shtwfgs.cn

list(dict.fromkeys(arr))
来源：http://dg.huixinmuqiang.cn

[U06] Py：合并两个字典
来源：http://ng.panjiajie.cn

{**a, **b}
来源：http://zo.nicolike.cn

[U07] Py：反转字典键值
来源：http://xt.lnxyls.cn

{v: k for k, v in d.items()}
来源：http://lz.hahajie.cn

[U08] Py：展平二维列表
来源：http://uv.hnjuh.cn

[y for x in nested for y in x]
来源：http://or.jctech888.com.cn

[U09] Py：字典取最大值的键
来源：http://ko.asd995.cn

max(d, key=d.get)
来源：http://zx.nszjky.cn

[U10] Py：按值排序字典
来源：http://ci.panjiajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sd.asd995.cn

[U11] Py：生成器表达式
来源：http://hb.chemitech.net.cn

(x * 2 for x in arr)
来源：http://rg.huanxung.cn

[U12] Py：取出现最多的 3 个元素
来源：http://by.yuntaijiaju.cn

Counter(arr).most_common(3)
来源：http://lz.521024.cn

[U13] Py：固定长度队列
来源：http://tb.nszjky.cn

deque(maxlen=10)
来源：http://md.colortex.cn

[U14] Py：分组收集到列表
来源：http://js.shxzskj.cn

defaultdict(list)
来源：http://ak.521024.cn

[U15] Py：高精度计时
来源：http://br.lnxyls.cn

t = time.perf_counter()
来源：http://jv.hnjuh.cn

[U16] Py：命令行参数解析
来源：http://oa.jianghongdianzi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jx.jianghongdianzi.cn

[U17] Py：初始化日志
来源：http://xb.yuexingan06.cn

logging.basicConfig(level=logging.INFO)
来源：http://zx.shxzukj.cn

[U18] Py：预编译正则
来源：http://cw.shxzukj.cn

pat = re.compile(r"\d+")
来源：http://op.bjjhwx.cn

[U19] Py：正则替换带回调
来源：http://yb.panjiajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zk.szsharing.cn

[U20] Py：缓存函数结果
来源：http://wq.bookmarksfly.cn

@functools.lru_cache(maxsize=None)
来源：http://jo.jctech888.com.cn

[U21] Py：自定义上下文管理器
来源：http://lb.haigaiapp.cn

@contextlib.contextmanager
来源：http://cj.wgjwhj.cn

[U22] Py：矩阵转置
来源：http://jt.lnxyls.cn

list(zip(*m))
来源：http://lw.bookmarksfly.cn

[U23] Py：分块读取大文件
来源：http://ed.nicolike.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ye.nszjky.cn

[U24] Py：路径操作
来源：http://fg.shxzukj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lu.9csxet.cn

[U25] Py：CSV 按字典读
来源：http://iu.bjjhwx.cn

csv.DictReader(f)
来源：http://dk.jctech888.com.cn

[U26] Py：并发下载
来源：http://ks.newstarts.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bo.newstarts.cn


<!-- 参考信息 -->