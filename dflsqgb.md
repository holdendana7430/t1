代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cp.newstarts.cn

[S08] C：动态内存分配与释放
来源：http://tp.bookmarksfly.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ug.shxzukj.cn

[S09] C：结构体定义与初始化
来源：http://rk.yuntaijiaju.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ub.gzmigu.cn

[S10] C：指针与解引用
来源：http://ro.hahajie.cn

int *p = &a;  *p = 5;
来源：http://xw.huixinmuqiang.cn

[S11] C：逐行读文件
来源：http://fg.huixinmuqiang.cn

FILE *f = fopen("a.txt", "r");
来源：http://np.shtwfgs.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://rv.jianghongdianzi.cn

fclose(f);
来源：http://sr.lnxyls.cn

[S12] C：写文件
来源：http://pg.asd995.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ia.wgjwhj.cn

[S13] C：宏定义
来源：http://hv.9csxet.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://si.521024.cn

[S14] C：枚举
来源：http://uq.muxihuayi.cn

enum Color { RED, GREEN, BLUE };
来源：http://ck.szsharing.cn

[S15] C：类型转换
来源：http://ys.nszjky.cn

(double) a / b
来源：http://wo.huixiangedu.cn

[S16] C：位操作置位
来源：http://np.jianghongdianzi.cn

x |= (1 << 3);
来源：http://lz.nszjky.cn

[S17] C：安全拼接字符串
来源：http://rg.panjiajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ld.jianghongdianzi.cn

[S18] C：命令行参数
来源：http://jg.huixiangedu.cn

int main(int argc, char **argv)
来源：http://oz.shtwfgs.cn

[S19] C：快速排序
来源：http://ad.bookmarksfly.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fb.huanxung.cn

[S20] C：二分查找
来源：http://om.jianghongdianzi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ne.shxzskj.cn

[S21] C：字符类别判断
来源：http://er.shxzukj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gl.9csxet.cn

[S22] C：字符串转数字
来源：http://mp.bjjhwx.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xo.nicolike.cn

[S23] C：随机数
来源：http://me.shtwfgs.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://nt.huanxung.cn

[S24] C：获取本地时间
来源：http://vh.asd995.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vq.newstarts.cn

[S25] C：内存拷贝
来源：http://dd.shtwfgs.cn

memcpy(dst, src, n);
来源：http://rf.jctech888.com.cn

[S26] C：内存清零
来源：http://vt.yuntaijiaju.cn

memset(a, 0, sizeof a);
来源：http://fa.huixiangedu.cn

[S27] C：定义常量
来源：http://ae.bjjhwx.cn

const double PI = 3.14159;
来源：http://rr.chemitech.net.cn

[S28] C：静态变量
来源：http://vn.nszjky.cn

static int counter = 0;
来源：http://ta.shxzukj.cn

[S29] C：变参函数
来源：http://zl.yuntaijiaju.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lg.szsharing.cn

[S30] C：头文件保护
来源：http://kx.huanxung.cn

#ifndef X_H
来源：http://jr.muxihuayi.cn

#define X_H
来源：http://po.asd995.cn

#endif
来源：http://nt.wgjwhj.cn

[S31] C++：Hello World
来源：http://op.9csxet.cn

#include <iostream>
来源：http://jq.panjiajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://lu.newstarts.cn

[S32] C++：字符串
来源：http://gr.jctech888.com.cn

std::string s = "hi";  s += "!";
来源：http://qz.shxzskj.cn

[S33] C++：vector 增删
来源：http://yp.hnjuh.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dh.yuntaijiaju.cn

[S34] C++：遍历 vector
来源：http://fe.colortex.cn

for (auto &x : v) { std::cout << x; }
来源：http://eo.bjjhwx.cn

[S35] C++：map
来源：http://jk.newstarts.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wt.jctech888.com.cn

[S36] C++：unordered_map
来源：http://ba.chemitech.net.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ya.asd995.cn

[S37] C++：set
来源：http://sr.huixiangedu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ir.hahajie.cn

[S38] C++：排序
来源：http://nq.nicolike.cn

std::sort(v.begin(), v.end());
来源：http://iq.huanxung.cn

[S39] C++：自定义比较器排序
来源：http://mn.jctech888.com.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://no.hahajie.cn

[S40] C++：查找元素
来源：http://ey.shxzukj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vq.bjjhwx.cn

[S41] C++：类与构造函数
来源：http://hf.nszjky.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vi.colortex.cn

[S42] C++：继承与虚函数
来源：http://qg.521024.cn

class B : public Base { public: void f() override {} };
来源：http://zh.huanxung.cn

[S43] C++：智能指针
来源：http://ic.shxzukj.cn

auto p = std::make_unique<int>(5);
来源：http://vy.nicolike.cn

[S44] C++：引用传参
来源：http://ov.hnjuh.cn

void inc(int &x) { ++x; }
来源：http://sn.huixinmuqiang.cn

[S45] C++：lambda
来源：http://ln.huixinmuqiang.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gs.nszjky.cn

[S46] C++：函数模板
来源：http://og.bookmarksfly.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://is.wgjwhj.cn

[S47] C++：结构化绑定遍历
来源：http://fg.jianghongdianzi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hj.huanxung.cn

[S48] C++：逐行读文件
来源：http://vs.bookmarksfly.cn

std::ifstream in("a.txt");  std::string line;
来源：http://sg.huixiangedu.cn

while (std::getline(in, line)) { }
来源：http://yu.panjiajie.cn

[S49] C++：写文件
来源：http://jk.shxzukj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ek.gzmigu.cn

[S50] C++：格式化数字
来源：http://la.asd995.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nc.9csxet.cn

[S51] C++：显式类型转换
来源：http://vy.lnxyls.cn

static_cast<double>(a) / b
来源：http://zl.huixinmuqiang.cn

[S52] C++：const 与 noexcept
来源：http://tj.hahajie.cn

int size() const noexcept { return n_; }
来源：http://jx.nszjky.cn

[S53] C++：移动语义
来源：http://bt.bjjhwx.cn

std::vector<int> w = std::move(v);
来源：http://ql.szxytkj.cn

[S54] C++：异常处理
来源：http://lh.colortex.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jw.nicolike.cn

[S55] C++：结构化绑定
来源：http://hw.nicolike.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bm.huanxung.cn

[S56] C++：optional
来源：http://qj.szxytkj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zn.nszjky.cn

[S57] C++：编译期常量
来源：http://rr.asd995.cn

constexpr int N = 10;
来源：http://iw.lnxyls.cn

[S58] C++：命名空间
来源：http://oi.huixinmuqiang.cn

namespace ns { int f() { return 1; } }
来源：http://rw.shtwfgs.cn

[S59] C++：静态断言
来源：http://yk.newstarts.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lg.shtwfgs.cn

[S60] C++：遍历并删除元素
来源：http://ny.bjjhwx.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qh.bjjhwx.cn

================================================================================
来源：http://tp.jianghongdianzi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ju.nicolike.cn

================================================================================
来源：http://uc.shtwfgs.cn

[T01] Kotlin：Hello World
来源：http://ou.9csxet.cn

println("Hello")
来源：http://la.asd995.cn

[T02] Kotlin：变量
来源：http://wt.haigaiapp.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ud.hnjuh.cn

[T03] Kotlin：字符串模板
来源：http://ej.jianghongdianzi.cn

"值: $b"
来源：http://zr.nicolike.cn

[T04] Kotlin：空安全
来源：http://dy.521024.cn

val n: String? = null;  n?.length
来源：http://cb.jctech888.com.cn

[T05] Kotlin：when 表达式
来源：http://tl.jctech888.com.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pc.jianghongdianzi.cn

[T06] Kotlin：集合映射
来源：http://vk.asd995.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gh.chemitech.net.cn

[T07] Kotlin：集合过滤
来源：http://nk.bjjhwx.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ll.hnjuh.cn

[T08] Kotlin：数据类
来源：http://xk.asd995.cn

data class User(val name: String, val age: Int)
来源：http://be.521024.cn

[T09] Kotlin：扩展函数
来源：http://en.521024.cn

fun String.exclaim() = this + "!"
来源：http://kd.huixiangedu.cn

[T10] Kotlin：默认参数
来源：http://mi.muxihuayi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://mh.asd995.cn

[T11] Kotlin：协程
来源：http://sx.huanxung.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nv.bjjhwx.cn

[T12] Kotlin：解构声明
来源：http://ve.muxihuayi.cn

val (a, b) = Pair(1, 2)
来源：http://co.muxihuayi.cn

[T13] Kotlin：只读 Map
来源：http://pu.huanxung.cn

val m = mapOf("a" to 1)
来源：http://ae.yuntaijiaju.cn

[T14] Kotlin：循环
来源：http://vb.nszjky.cn

for (i in 1..10) println(i)
来源：http://pf.jianghongdianzi.cn

[T15] Kotlin：接口
来源：http://fz.jctech888.com.cn

interface Shape { fun area(): Double }
来源：http://qw.hnjuh.cn

[T16] Swift：Hello World
来源：http://cu.521024.cn

print("Hello")
来源：http://kg.szsharing.cn

[T17] Swift：变量与常量
来源：http://yq.521024.cn

var a = 1;  let b = 2
来源：http://zy.shxzskj.cn

[T18] Swift：字符串插值
来源：http://cd.lnxyls.cn

"值: \(b)"
来源：http://jg.asd995.cn

[T19] Swift：可选绑定
来源：http://mh.wgjwhj.cn

if let n = opt { print(n) }
来源：http://ot.huixiangedu.cn

[T20] Swift：数组操作
来源：http://gu.hnjuh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://rl.hnjuh.cn

[T21] Swift：遍历
来源：http://lc.521024.cn

for x in a { print(x) }
来源：http://ho.nicolike.cn

[T22] Swift：字典
来源：http://mc.huixinmuqiang.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ij.521024.cn

[T23] Swift：函数
来源：http://uc.chemitech.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ks.jianghongdianzi.cn

[T24] Swift：闭包
来源：http://rl.bookmarksfly.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://bt.chemitech.net.cn

[T25] Swift：结构体
来源：http://ag.gzmigu.cn

struct P { var x: Int }
来源：http://bp.shxzukj.cn

[T26] Swift：类与重写
来源：http://me.9csxet.cn

class A: Base { override func f() {} }
来源：http://je.colortex.cn

[T27] Swift：错误处理
来源：http://hr.nszjky.cn

do { try f() } catch { print(error) }
来源：http://pv.jctech888.com.cn

[T28] Swift：枚举
来源：http://ce.jianghongdianzi.cn

enum Color { case red, green }
来源：http://mw.nicolike.cn

[T29] Swift：guard 提前返回
来源：http://ez.bookmarksfly.cn

guard let x = opt else { return }
来源：http://ua.521024.cn

[T30] Swift：协议
来源：http://jl.huanxung.cn

protocol Shape { func area() -> Double }
来源：http://dg.panjiajie.cn

[T31] Lua：Hello World
来源：http://dd.521024.cn

print("Hello")
来源：http://vz.szxytkj.cn

[T32] Lua：局部变量
来源：http://dz.huanxung.cn

local a = 1
来源：http://gt.wgjwhj.cn

[T33] Lua：表（数组）
来源：http://og.muxihuayi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://tv.huanxung.cn

[T34] Lua：遍历表
来源：http://fh.panjiajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://av.huanxung.cn

[T35] Lua：字典表
来源：http://eu.wgjwhj.cn

local d = { a = 1 };  d.b = 2
来源：http://wm.bjjhwx.cn

[T36] Lua：函数
来源：http://aq.hahajie.cn

function add(a, b) return a + b end
来源：http://jm.panjiajie.cn

[T37] Lua：字符串拼接
来源：http://bu.shxzukj.cn

"a" .. "b"
来源：http://gr.bookmarksfly.cn

[T38] Lua：条件
来源：http://md.huixinmuqiang.cn

if x > 0 then print("正") end
来源：http://ug.hnjuh.cn

[T39] Lua：模式匹配
来源：http://mf.bookmarksfly.cn

string.find(s, "%d+")
来源：http://ke.muxihuayi.cn

[T40] Lua：元表
来源：http://jt.newstarts.cn

setmetatable({}, { __index = base })
来源：http://da.chemitech.net.cn

[T41] Perl：Hello World
来源：http://ut.huanxung.cn

print "Hello\n";
来源：http://pu.gzmigu.cn

[T42] Perl：变量类型
来源：http://xs.shxzukj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pc.wgjwhj.cn

[T43] Perl：字符串插值
来源：http://hs.jctech888.com.cn

"值: $a"
来源：http://up.shxzukj.cn

[T44] Perl：条件
来源：http://bd.hahajie.cn

if ($a > 0) { print "正"; }
来源：http://yo.521024.cn

[T45] Perl：数组遍历
来源：http://ie.panjiajie.cn

for my $x (@arr) { print $x; }
来源：http://hl.panjiajie.cn

[T46] Perl：哈希操作
来源：http://aj.jianghongdianzi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nn.shxzskj.cn

[T47] Perl：正则捕获
来源：http://rg.wgjwhj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.panjiajie.cn

[T48] Perl：正则替换
来源：http://vi.chemitech.net.cn

$s =~ s/old/new/g;
来源：http://dg.lnxyls.cn

[T49] Perl：函数
来源：http://fb.hnjuh.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jc.yuexingan06.cn

[T50] Perl：逐行读文件
来源：http://pn.huixiangedu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://iw.hnjuh.cn

while (my $line = <$fh>) { print $line; }
来源：http://od.haigaiapp.cn

[T51] Scala：Hello World
来源：http://uw.jianghongdianzi.cn

println("Hello")
来源：http://jv.szsharing.cn

[T52] Scala：变量
来源：http://gm.hahajie.cn

val a = 1;  var b = 2
来源：http://ib.panjiajie.cn

[T53] Scala：字符串插值
来源：http://jo.newstarts.cn

s"值: $b"
来源：http://yb.bjjhwx.cn

[T54] Scala：集合映射
来源：http://es.bookmarksfly.cn

List(1, 2, 3).map(_ * 2)
来源：http://em.lnxyls.cn

[T55] Scala：集合过滤
来源：http://mz.chemitech.net.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gu.bookmarksfly.cn

[T56] Scala：样例类
来源：http://oy.shxzskj.cn

case class User(name: String, age: Int)
来源：http://th.521024.cn

[T57] Scala：模式匹配
来源：http://fx.lnxyls.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wu.colortex.cn

[T58] Scala：函数定义
来源：http://me.shxzukj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://va.newstarts.cn

[T59] Scala：循环
来源：http://rh.haigaiapp.cn

for (i <- 1 to 10) println(i)
来源：http://vl.hahajie.cn

[T60] Scala：折叠
来源：http://cj.szxytkj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://to.shxzukj.cn

================================================================================
来源：http://hn.nszjky.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jg.newstarts.cn

================================================================================
来源：http://ki.jianghongdianzi.cn

[U01] Py：创建虚拟环境
来源：http://vh.9csxet.cn

python -m venv .venv && source .venv/bin/activate
来源：http://gx.huixinmuqiang.cn

[U02] Py：导出 / 安装依赖
来源：http://oz.huixinmuqiang.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://te.9csxet.cn

[U03] Py：加载 .env 配置
来源：http://mr.szsharing.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://io.hnjuh.cn

[U04] Py：变量调试打印
来源：http://jr.haigaiapp.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://yl.shtwfgs.cn

[U05] Py：列表去重且保序
来源：http://jl.szsharing.cn

list(dict.fromkeys(arr))
来源：http://xp.521024.cn

[U06] Py：合并两个字典
来源：http://la.bjjhwx.cn

{**a, **b}
来源：http://jd.hnjuh.cn

[U07] Py：反转字典键值
来源：http://lo.nszjky.cn

{v: k for k, v in d.items()}
来源：http://jk.asd995.cn

[U08] Py：展平二维列表
来源：http://yu.jianghongdianzi.cn

[y for x in nested for y in x]
来源：http://ig.szsharing.cn

[U09] Py：字典取最大值的键
来源：http://bw.chemitech.net.cn

max(d, key=d.get)
来源：http://bo.lnxyls.cn

[U10] Py：按值排序字典
来源：http://we.newstarts.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kj.huixiangedu.cn

[U11] Py：生成器表达式
来源：http://mf.yuexingan06.cn

(x * 2 for x in arr)
来源：http://sn.newstarts.cn

[U12] Py：取出现最多的 3 个元素
来源：http://fn.szsharing.cn

Counter(arr).most_common(3)
来源：http://qo.wgjwhj.cn

[U13] Py：固定长度队列
来源：http://cs.jianghongdianzi.cn

deque(maxlen=10)
来源：http://xo.panjiajie.cn

[U14] Py：分组收集到列表
来源：http://jx.panjiajie.cn

defaultdict(list)
来源：http://ai.chemitech.net.cn

[U15] Py：高精度计时
来源：http://er.yuntaijiaju.cn

t = time.perf_counter()
来源：http://cm.shxzskj.cn

[U16] Py：命令行参数解析
来源：http://uq.huixinmuqiang.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yy.colortex.cn

[U17] Py：初始化日志
来源：http://ae.bjjhwx.cn

logging.basicConfig(level=logging.INFO)
来源：http://on.muxihuayi.cn

[U18] Py：预编译正则
来源：http://ka.newstarts.cn

pat = re.compile(r"\d+")
来源：http://rk.nszjky.cn

[U19] Py：正则替换带回调
来源：http://cq.jctech888.com.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rm.shxzskj.cn

[U20] Py：缓存函数结果
来源：http://ai.panjiajie.cn

@functools.lru_cache(maxsize=None)
来源：http://hi.hahajie.cn

[U21] Py：自定义上下文管理器
来源：http://ch.wgjwhj.cn

@contextlib.contextmanager
来源：http://jq.shtwfgs.cn

[U22] Py：矩阵转置
来源：http://it.haigaiapp.cn

list(zip(*m))
来源：http://fd.huanxung.cn

[U23] Py：分块读取大文件
来源：http://tl.hahajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bt.9csxet.cn

[U24] Py：路径操作
来源：http://vz.shtwfgs.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wj.chemitech.net.cn

[U25] Py：CSV 按字典读
来源：http://tv.nszjky.cn

csv.DictReader(f)
来源：http://xj.521024.cn

[U26] Py：并发下载
来源：http://xx.hahajie.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yc.huanxung.cn

[U27] Py：异步 HTTP
来源：http://si.shxzukj.cn

aiohttp.ClientSession() 配合 async with
来源：http://eo.9csxet.cn

[U28] Py：类型别名
来源：http://vj.nszjky.cn

UserId = int
来源：http://ro.bjjhwx.cn

[U29] Py：属性校验
来源：http://pd.szsharing.cn

@property 与 @x.setter 配合
来源：http://nv.panjiajie.cn

[U30] Py：数据类
来源：http://lj.newstarts.cn

@dataclass(slots=True)
来源：http://qe.huixinmuqiang.cn


<!-- 参考信息 -->