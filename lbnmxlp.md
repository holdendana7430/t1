代发 wailian999

strlen(s)
来源：http://go.bjjhwx.cn

[S06] C：字符串比较
来源：http://lr.yuntaijiaju.cn

strcmp(a, b) == 0
来源：http://fp.yuexingan06.cn

[S07] C：数组遍历求和
来源：http://gi.muxihuayi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ms.muxihuayi.cn

[S08] C：动态内存分配与释放
来源：http://yp.huixinmuqiang.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ae.muxihuayi.cn

[S09] C：结构体定义与初始化
来源：http://wz.huixiangedu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xz.lnxyls.cn

[S10] C：指针与解引用
来源：http://hr.muxihuayi.cn

int *p = &a;  *p = 5;
来源：http://ev.nszjky.cn

[S11] C：逐行读文件
来源：http://wj.nszjky.cn

FILE *f = fopen("a.txt", "r");
来源：http://ry.yuexingan06.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xm.huixinmuqiang.cn

fclose(f);
来源：http://cl.gzmigu.cn

[S12] C：写文件
来源：http://tj.panjiajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hw.huixinmuqiang.cn

[S13] C：宏定义
来源：http://dx.shxzskj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qr.chemitech.net.cn

[S14] C：枚举
来源：http://wu.wgjwhj.cn

enum Color { RED, GREEN, BLUE };
来源：http://jr.jianghongdianzi.cn

[S15] C：类型转换
来源：http://kk.huanxung.cn

(double) a / b
来源：http://ue.jctech888.com.cn

[S16] C：位操作置位
来源：http://yd.nszjky.cn

x |= (1 << 3);
来源：http://ax.bookmarksfly.cn

[S17] C：安全拼接字符串
来源：http://gb.hahajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zj.muxihuayi.cn

[S18] C：命令行参数
来源：http://ce.nszjky.cn

int main(int argc, char **argv)
来源：http://vi.huixiangedu.cn

[S19] C：快速排序
来源：http://sm.bjjhwx.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rg.huixiangedu.cn

[S20] C：二分查找
来源：http://ek.bookmarksfly.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rc.shxzskj.cn

[S21] C：字符类别判断
来源：http://en.hnjuh.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sd.huixiangedu.cn

[S22] C：字符串转数字
来源：http://bc.muxihuayi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vu.huanxung.cn

[S23] C：随机数
来源：http://zc.hahajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://gp.szxytkj.cn

[S24] C：获取本地时间
来源：http://va.panjiajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xn.yuexingan06.cn

[S25] C：内存拷贝
来源：http://ac.newstarts.cn

memcpy(dst, src, n);
来源：http://oy.shtwfgs.cn

[S26] C：内存清零
来源：http://tk.jctech888.com.cn

memset(a, 0, sizeof a);
来源：http://hh.newstarts.cn

[S27] C：定义常量
来源：http://zg.nszjky.cn

const double PI = 3.14159;
来源：http://jl.nicolike.cn

[S28] C：静态变量
来源：http://lh.hahajie.cn

static int counter = 0;
来源：http://vx.szsharing.cn

[S29] C：变参函数
来源：http://ky.szxytkj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yf.hnjuh.cn

[S30] C：头文件保护
来源：http://uu.hnjuh.cn

#ifndef X_H
来源：http://xg.wgjwhj.cn

#define X_H
来源：http://ir.szsharing.cn

#endif
来源：http://md.shxzukj.cn

[S31] C++：Hello World
来源：http://tn.asd995.cn

#include <iostream>
来源：http://zb.9csxet.cn

int main() { std::cout << "Hello\n"; }
来源：http://fa.9csxet.cn

[S32] C++：字符串
来源：http://ci.szsharing.cn

std::string s = "hi";  s += "!";
来源：http://da.jianghongdianzi.cn

[S33] C++：vector 增删
来源：http://ng.huixiangedu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qk.muxihuayi.cn

[S34] C++：遍历 vector
来源：http://fa.huanxung.cn

for (auto &x : v) { std::cout << x; }
来源：http://dr.gzmigu.cn

[S35] C++：map
来源：http://ke.nicolike.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://oz.panjiajie.cn

[S36] C++：unordered_map
来源：http://vj.shxzukj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ys.hahajie.cn

[S37] C++：set
来源：http://zh.9csxet.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hw.asd995.cn

[S38] C++：排序
来源：http://fm.hahajie.cn

std::sort(v.begin(), v.end());
来源：http://tk.521024.cn

[S39] C++：自定义比较器排序
来源：http://jf.lnxyls.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pr.nszjky.cn

[S40] C++：查找元素
来源：http://vz.haigaiapp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://oo.szxytkj.cn

[S41] C++：类与构造函数
来源：http://kc.521024.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wp.huixiangedu.cn

[S42] C++：继承与虚函数
来源：http://rp.chemitech.net.cn

class B : public Base { public: void f() override {} };
来源：http://ig.huanxung.cn

[S43] C++：智能指针
来源：http://qn.521024.cn

auto p = std::make_unique<int>(5);
来源：http://ic.nszjky.cn

[S44] C++：引用传参
来源：http://rm.panjiajie.cn

void inc(int &x) { ++x; }
来源：http://go.wgjwhj.cn

[S45] C++：lambda
来源：http://gm.bjjhwx.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jp.shtwfgs.cn

[S46] C++：函数模板
来源：http://zx.muxihuayi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qz.wgjwhj.cn

[S47] C++：结构化绑定遍历
来源：http://py.shxzskj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ur.newstarts.cn

[S48] C++：逐行读文件
来源：http://oo.nszjky.cn

std::ifstream in("a.txt");  std::string line;
来源：http://va.yuexingan06.cn

while (std::getline(in, line)) { }
来源：http://pu.haigaiapp.cn

[S49] C++：写文件
来源：http://zx.521024.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://de.bjjhwx.cn

[S50] C++：格式化数字
来源：http://vc.lnxyls.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cv.nicolike.cn

[S51] C++：显式类型转换
来源：http://oh.huixinmuqiang.cn

static_cast<double>(a) / b
来源：http://yg.shxzskj.cn

[S52] C++：const 与 noexcept
来源：http://ba.newstarts.cn

int size() const noexcept { return n_; }
来源：http://mv.nicolike.cn

[S53] C++：移动语义
来源：http://nr.hahajie.cn

std::vector<int> w = std::move(v);
来源：http://yd.newstarts.cn

[S54] C++：异常处理
来源：http://kl.9csxet.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pk.521024.cn

[S55] C++：结构化绑定
来源：http://cr.shtwfgs.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jn.muxihuayi.cn

[S56] C++：optional
来源：http://an.huixinmuqiang.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mv.shxzskj.cn

[S57] C++：编译期常量
来源：http://as.shtwfgs.cn

constexpr int N = 10;
来源：http://ig.521024.cn

[S58] C++：命名空间
来源：http://cb.shxzskj.cn

namespace ns { int f() { return 1; } }
来源：http://tc.jctech888.com.cn

[S59] C++：静态断言
来源：http://av.bjjhwx.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lx.hnjuh.cn

[S60] C++：遍历并删除元素
来源：http://dg.panjiajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ie.huanxung.cn

================================================================================
来源：http://hx.colortex.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://de.chemitech.net.cn

================================================================================
来源：http://lt.newstarts.cn

[T01] Kotlin：Hello World
来源：http://ah.huixiangedu.cn

println("Hello")
来源：http://sz.chemitech.net.cn

[T02] Kotlin：变量
来源：http://wi.lnxyls.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jh.haigaiapp.cn

[T03] Kotlin：字符串模板
来源：http://ec.shxzukj.cn

"值: $b"
来源：http://lx.bookmarksfly.cn

[T04] Kotlin：空安全
来源：http://fi.huixinmuqiang.cn

val n: String? = null;  n?.length
来源：http://pz.huixiangedu.cn

[T05] Kotlin：when 表达式
来源：http://ge.shxzskj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kv.huixinmuqiang.cn

[T06] Kotlin：集合映射
来源：http://yi.chemitech.net.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://de.nicolike.cn

[T07] Kotlin：集合过滤
来源：http://at.bjjhwx.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://sq.haigaiapp.cn

[T08] Kotlin：数据类
来源：http://kj.newstarts.cn

data class User(val name: String, val age: Int)
来源：http://mk.huanxung.cn

[T09] Kotlin：扩展函数
来源：http://mt.szsharing.cn

fun String.exclaim() = this + "!"
来源：http://qh.szsharing.cn

[T10] Kotlin：默认参数
来源：http://ry.lnxyls.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ak.wgjwhj.cn

[T11] Kotlin：协程
来源：http://cx.wgjwhj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xx.huixinmuqiang.cn

[T12] Kotlin：解构声明
来源：http://xb.jianghongdianzi.cn

val (a, b) = Pair(1, 2)
来源：http://bc.nicolike.cn

[T13] Kotlin：只读 Map
来源：http://sh.newstarts.cn

val m = mapOf("a" to 1)
来源：http://rc.521024.cn

[T14] Kotlin：循环
来源：http://an.yuexingan06.cn

for (i in 1..10) println(i)
来源：http://hp.shtwfgs.cn

[T15] Kotlin：接口
来源：http://hr.wgjwhj.cn

interface Shape { fun area(): Double }
来源：http://nx.colortex.cn

[T16] Swift：Hello World
来源：http://bq.panjiajie.cn

print("Hello")
来源：http://ut.huixiangedu.cn

[T17] Swift：变量与常量
来源：http://vm.lnxyls.cn

var a = 1;  let b = 2
来源：http://xq.panjiajie.cn

[T18] Swift：字符串插值
来源：http://qh.521024.cn

"值: \(b)"
来源：http://vr.huixinmuqiang.cn

[T19] Swift：可选绑定
来源：http://km.wgjwhj.cn

if let n = opt { print(n) }
来源：http://jd.huixiangedu.cn

[T20] Swift：数组操作
来源：http://ev.szxytkj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://og.szxytkj.cn

[T21] Swift：遍历
来源：http://sq.huanxung.cn

for x in a { print(x) }
来源：http://nn.9csxet.cn

[T22] Swift：字典
来源：http://gu.wgjwhj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://jb.asd995.cn

[T23] Swift：函数
来源：http://xu.shxzskj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vp.shxzskj.cn

[T24] Swift：闭包
来源：http://py.jianghongdianzi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://hg.huixinmuqiang.cn

[T25] Swift：结构体
来源：http://bh.hahajie.cn

struct P { var x: Int }
来源：http://ni.asd995.cn

[T26] Swift：类与重写
来源：http://fy.huanxung.cn

class A: Base { override func f() {} }
来源：http://yh.szsharing.cn

[T27] Swift：错误处理
来源：http://gf.chemitech.net.cn

do { try f() } catch { print(error) }
来源：http://jz.yuntaijiaju.cn

[T28] Swift：枚举
来源：http://el.szxytkj.cn

enum Color { case red, green }
来源：http://up.colortex.cn

[T29] Swift：guard 提前返回
来源：http://ax.lnxyls.cn

guard let x = opt else { return }
来源：http://xs.yuexingan06.cn

[T30] Swift：协议
来源：http://iq.huanxung.cn

protocol Shape { func area() -> Double }
来源：http://vd.jctech888.com.cn

[T31] Lua：Hello World
来源：http://zy.shxzskj.cn

print("Hello")
来源：http://ea.shxzukj.cn

[T32] Lua：局部变量
来源：http://zk.nszjky.cn

local a = 1
来源：http://ek.gzmigu.cn

[T33] Lua：表（数组）
来源：http://kx.nicolike.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://nz.shxzukj.cn

[T34] Lua：遍历表
来源：http://jp.9csxet.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ca.panjiajie.cn

[T35] Lua：字典表
来源：http://kn.huixinmuqiang.cn

local d = { a = 1 };  d.b = 2
来源：http://vb.nicolike.cn

[T36] Lua：函数
来源：http://ub.bjjhwx.cn

function add(a, b) return a + b end
来源：http://sb.szxytkj.cn

[T37] Lua：字符串拼接
来源：http://wb.jianghongdianzi.cn

"a" .. "b"
来源：http://my.lnxyls.cn

[T38] Lua：条件
来源：http://qj.hnjuh.cn

if x > 0 then print("正") end
来源：http://gr.yuntaijiaju.cn

[T39] Lua：模式匹配
来源：http://nf.szxytkj.cn

string.find(s, "%d+")
来源：http://by.yuntaijiaju.cn

[T40] Lua：元表
来源：http://cg.huanxung.cn

setmetatable({}, { __index = base })
来源：http://sl.huixiangedu.cn

[T41] Perl：Hello World
来源：http://dn.huixiangedu.cn

print "Hello\n";
来源：http://nm.nicolike.cn

[T42] Perl：变量类型
来源：http://gf.nicolike.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://el.9csxet.cn

[T43] Perl：字符串插值
来源：http://aa.asd995.cn

"值: $a"
来源：http://un.hahajie.cn

[T44] Perl：条件
来源：http://gf.hnjuh.cn

if ($a > 0) { print "正"; }
来源：http://vc.shtwfgs.cn

[T45] Perl：数组遍历
来源：http://gr.9csxet.cn

for my $x (@arr) { print $x; }
来源：http://co.nszjky.cn

[T46] Perl：哈希操作
来源：http://li.szsharing.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pr.haigaiapp.cn

[T47] Perl：正则捕获
来源：http://xf.jctech888.com.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://nb.yuexingan06.cn

[T48] Perl：正则替换
来源：http://sr.huanxung.cn

$s =~ s/old/new/g;
来源：http://jd.szsharing.cn

[T49] Perl：函数
来源：http://lr.9csxet.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yy.yuntaijiaju.cn

[T50] Perl：逐行读文件
来源：http://lt.shxzskj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zt.shtwfgs.cn

while (my $line = <$fh>) { print $line; }
来源：http://zu.haigaiapp.cn

[T51] Scala：Hello World
来源：http://aw.bookmarksfly.cn

println("Hello")
来源：http://kz.szxytkj.cn

[T52] Scala：变量
来源：http://xl.szsharing.cn

val a = 1;  var b = 2
来源：http://vq.shxzukj.cn

[T53] Scala：字符串插值
来源：http://re.bookmarksfly.cn

s"值: $b"
来源：http://rg.nicolike.cn

[T54] Scala：集合映射
来源：http://wt.muxihuayi.cn

List(1, 2, 3).map(_ * 2)
来源：http://qz.asd995.cn

[T55] Scala：集合过滤
来源：http://ad.colortex.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xf.jctech888.com.cn

[T56] Scala：样例类
来源：http://cw.muxihuayi.cn

case class User(name: String, age: Int)
来源：http://gv.yuntaijiaju.cn

[T57] Scala：模式匹配
来源：http://gf.bjjhwx.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://yw.nicolike.cn

[T58] Scala：函数定义
来源：http://yd.bjjhwx.cn

def add(a: Int, b: Int): Int = a + b
来源：http://uf.wgjwhj.cn

[T59] Scala：循环
来源：http://en.shxzukj.cn

for (i <- 1 to 10) println(i)
来源：http://fz.panjiajie.cn

[T60] Scala：折叠
来源：http://co.521024.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tm.gzmigu.cn

================================================================================
来源：http://rc.shtwfgs.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yv.gzmigu.cn

================================================================================
来源：http://ks.wgjwhj.cn

[U01] Py：创建虚拟环境
来源：http://dh.yuexingan06.cn

python -m venv .venv && source .venv/bin/activate
来源：http://st.shxzukj.cn

[U02] Py：导出 / 安装依赖
来源：http://tx.shtwfgs.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zj.wgjwhj.cn

[U03] Py：加载 .env 配置
来源：http://qn.shtwfgs.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://nq.panjiajie.cn

[U04] Py：变量调试打印
来源：http://sk.gzmigu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hu.9csxet.cn

[U05] Py：列表去重且保序
来源：http://fm.shxzukj.cn

list(dict.fromkeys(arr))
来源：http://sp.asd995.cn

[U06] Py：合并两个字典
来源：http://cm.szxytkj.cn

{**a, **b}
来源：http://uv.panjiajie.cn

[U07] Py：反转字典键值
来源：http://ew.lnxyls.cn

{v: k for k, v in d.items()}
来源：http://ys.gzmigu.cn

[U08] Py：展平二维列表
来源：http://mj.newstarts.cn

[y for x in nested for y in x]
来源：http://hk.huanxung.cn

[U09] Py：字典取最大值的键
来源：http://kn.chemitech.net.cn

max(d, key=d.get)
来源：http://mg.wgjwhj.cn

[U10] Py：按值排序字典
来源：http://md.shtwfgs.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qn.huixiangedu.cn

[U11] Py：生成器表达式
来源：http://tv.nicolike.cn

(x * 2 for x in arr)
来源：http://uo.huixinmuqiang.cn

[U12] Py：取出现最多的 3 个元素
来源：http://eu.wgjwhj.cn

Counter(arr).most_common(3)
来源：http://xl.yuntaijiaju.cn

[U13] Py：固定长度队列
来源：http://hz.bookmarksfly.cn

deque(maxlen=10)
来源：http://gz.bjjhwx.cn

[U14] Py：分组收集到列表
来源：http://vr.hahajie.cn

defaultdict(list)
来源：http://ji.asd995.cn

[U15] Py：高精度计时
来源：http://ny.bookmarksfly.cn

t = time.perf_counter()
来源：http://pf.nicolike.cn

[U16] Py：命令行参数解析
来源：http://br.hnjuh.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cy.9csxet.cn

[U17] Py：初始化日志
来源：http://kj.szxytkj.cn

logging.basicConfig(level=logging.INFO)
来源：http://gg.shtwfgs.cn

[U18] Py：预编译正则
来源：http://he.gzmigu.cn

pat = re.compile(r"\d+")
来源：http://lw.hahajie.cn

[U19] Py：正则替换带回调
来源：http://ad.nicolike.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zk.shtwfgs.cn

[U20] Py：缓存函数结果
来源：http://bf.jctech888.com.cn

@functools.lru_cache(maxsize=None)
来源：http://hj.szsharing.cn

[U21] Py：自定义上下文管理器
来源：http://xe.huanxung.cn

@contextlib.contextmanager
来源：http://wo.lnxyls.cn

[U22] Py：矩阵转置
来源：http://ki.colortex.cn

list(zip(*m))
来源：http://bt.muxihuayi.cn

[U23] Py：分块读取大文件
来源：http://jr.hnjuh.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ha.bookmarksfly.cn

[U24] Py：路径操作
来源：http://xn.asd995.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://to.yuexingan06.cn

[U25] Py：CSV 按字典读
来源：http://jb.jctech888.com.cn

csv.DictReader(f)
来源：http://bf.hnjuh.cn

[U26] Py：并发下载
来源：http://uw.bjjhwx.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zn.shtwfgs.cn

[U27] Py：异步 HTTP
来源：http://wh.huanxung.cn

aiohttp.ClientSession() 配合 async with
来源：http://sc.shtwfgs.cn

[U28] Py：类型别名
来源：http://id.yuntaijiaju.cn

UserId = int
来源：http://nu.shxzukj.cn


<!-- 参考信息 -->