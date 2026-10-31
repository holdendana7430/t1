代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dt.szsharing.cn

[S10] C：指针与解引用
来源：http://wh.szsharing.cn

int *p = &a;  *p = 5;
来源：http://qz.521024.cn

[S11] C：逐行读文件
来源：http://ev.gzmigu.cn

FILE *f = fopen("a.txt", "r");
来源：http://mv.shtwfgs.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://lg.yuexingan06.cn

fclose(f);
来源：http://zs.chemitech.net.cn

[S12] C：写文件
来源：http://ck.huixiangedu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hs.huixiangedu.cn

[S13] C：宏定义
来源：http://id.szsharing.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dd.yuexingan06.cn

[S14] C：枚举
来源：http://qf.bookmarksfly.cn

enum Color { RED, GREEN, BLUE };
来源：http://zw.newstarts.cn

[S15] C：类型转换
来源：http://tc.szsharing.cn

(double) a / b
来源：http://uq.wgjwhj.cn

[S16] C：位操作置位
来源：http://pt.hnjuh.cn

x |= (1 << 3);
来源：http://tu.huixiangedu.cn

[S17] C：安全拼接字符串
来源：http://pr.panjiajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gz.yuntaijiaju.cn

[S18] C：命令行参数
来源：http://xa.huanxung.cn

int main(int argc, char **argv)
来源：http://jt.chemitech.net.cn

[S19] C：快速排序
来源：http://vc.szsharing.cn

qsort(a, n, sizeof(int), cmp);
来源：http://cm.lnxyls.cn

[S20] C：二分查找
来源：http://eo.muxihuayi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ha.521024.cn

[S21] C：字符类别判断
来源：http://am.shxzskj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qd.nszjky.cn

[S22] C：字符串转数字
来源：http://ko.shxzukj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xf.haigaiapp.cn

[S23] C：随机数
来源：http://zp.hnjuh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wc.521024.cn

[S24] C：获取本地时间
来源：http://ib.shxzukj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hs.shxzskj.cn

[S25] C：内存拷贝
来源：http://ro.jianghongdianzi.cn

memcpy(dst, src, n);
来源：http://lo.bookmarksfly.cn

[S26] C：内存清零
来源：http://pe.bjjhwx.cn

memset(a, 0, sizeof a);
来源：http://bj.huanxung.cn

[S27] C：定义常量
来源：http://wu.shxzukj.cn

const double PI = 3.14159;
来源：http://di.newstarts.cn

[S28] C：静态变量
来源：http://ee.9csxet.cn

static int counter = 0;
来源：http://oz.haigaiapp.cn

[S29] C：变参函数
来源：http://co.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zu.bookmarksfly.cn

[S30] C：头文件保护
来源：http://dj.hnjuh.cn

#ifndef X_H
来源：http://tv.bjjhwx.cn

#define X_H
来源：http://rr.huanxung.cn

#endif
来源：http://ey.asd995.cn

[S31] C++：Hello World
来源：http://gf.asd995.cn

#include <iostream>
来源：http://kq.hnjuh.cn

int main() { std::cout << "Hello\n"; }
来源：http://rj.lnxyls.cn

[S32] C++：字符串
来源：http://zh.colortex.cn

std::string s = "hi";  s += "!";
来源：http://fg.yuexingan06.cn

[S33] C++：vector 增删
来源：http://hu.huanxung.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gk.shxzukj.cn

[S34] C++：遍历 vector
来源：http://si.bookmarksfly.cn

for (auto &x : v) { std::cout << x; }
来源：http://cw.nszjky.cn

[S35] C++：map
来源：http://am.521024.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yi.jctech888.com.cn

[S36] C++：unordered_map
来源：http://hf.szxytkj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ef.panjiajie.cn

[S37] C++：set
来源：http://hu.newstarts.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wz.szsharing.cn

[S38] C++：排序
来源：http://vg.chemitech.net.cn

std::sort(v.begin(), v.end());
来源：http://bd.nicolike.cn

[S39] C++：自定义比较器排序
来源：http://gn.haigaiapp.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sy.asd995.cn

[S40] C++：查找元素
来源：http://ry.shxzskj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ns.nicolike.cn

[S41] C++：类与构造函数
来源：http://mf.hahajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xp.lnxyls.cn

[S42] C++：继承与虚函数
来源：http://tc.wgjwhj.cn

class B : public Base { public: void f() override {} };
来源：http://ss.newstarts.cn

[S43] C++：智能指针
来源：http://yc.9csxet.cn

auto p = std::make_unique<int>(5);
来源：http://yw.9csxet.cn

[S44] C++：引用传参
来源：http://wn.521024.cn

void inc(int &x) { ++x; }
来源：http://ul.gzmigu.cn

[S45] C++：lambda
来源：http://pl.hnjuh.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ia.muxihuayi.cn

[S46] C++：函数模板
来源：http://ca.hnjuh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://op.521024.cn

[S47] C++：结构化绑定遍历
来源：http://qk.jianghongdianzi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gf.bjjhwx.cn

[S48] C++：逐行读文件
来源：http://nw.huixiangedu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://mt.yuexingan06.cn

while (std::getline(in, line)) { }
来源：http://qe.shtwfgs.cn

[S49] C++：写文件
来源：http://mc.asd995.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kw.panjiajie.cn

[S50] C++：格式化数字
来源：http://dv.nicolike.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ob.asd995.cn

[S51] C++：显式类型转换
来源：http://va.shtwfgs.cn

static_cast<double>(a) / b
来源：http://dd.huanxung.cn

[S52] C++：const 与 noexcept
来源：http://zh.szsharing.cn

int size() const noexcept { return n_; }
来源：http://fy.newstarts.cn

[S53] C++：移动语义
来源：http://lz.huanxung.cn

std::vector<int> w = std::move(v);
来源：http://rq.hnjuh.cn

[S54] C++：异常处理
来源：http://wi.521024.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://od.bookmarksfly.cn

[S55] C++：结构化绑定
来源：http://jt.nszjky.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gi.szsharing.cn

[S56] C++：optional
来源：http://cq.szsharing.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://im.jctech888.com.cn

[S57] C++：编译期常量
来源：http://eq.jianghongdianzi.cn

constexpr int N = 10;
来源：http://eo.haigaiapp.cn

[S58] C++：命名空间
来源：http://px.shxzukj.cn

namespace ns { int f() { return 1; } }
来源：http://wg.yuexingan06.cn

[S59] C++：静态断言
来源：http://lk.wgjwhj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://im.jctech888.com.cn

[S60] C++：遍历并删除元素
来源：http://cu.asd995.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kw.haigaiapp.cn

================================================================================
来源：http://aa.szsharing.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rx.muxihuayi.cn

================================================================================
来源：http://ad.bjjhwx.cn

[T01] Kotlin：Hello World
来源：http://fb.huixiangedu.cn

println("Hello")
来源：http://em.yuexingan06.cn

[T02] Kotlin：变量
来源：http://ex.hahajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://at.muxihuayi.cn

[T03] Kotlin：字符串模板
来源：http://ne.9csxet.cn

"值: $b"
来源：http://lj.lnxyls.cn

[T04] Kotlin：空安全
来源：http://vg.jianghongdianzi.cn

val n: String? = null;  n?.length
来源：http://yc.szsharing.cn

[T05] Kotlin：when 表达式
来源：http://fe.hnjuh.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sk.lnxyls.cn

[T06] Kotlin：集合映射
来源：http://am.shxzskj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://eg.muxihuayi.cn

[T07] Kotlin：集合过滤
来源：http://bt.yuntaijiaju.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://zi.521024.cn

[T08] Kotlin：数据类
来源：http://ka.shtwfgs.cn

data class User(val name: String, val age: Int)
来源：http://iw.huixiangedu.cn

[T09] Kotlin：扩展函数
来源：http://bq.chemitech.net.cn

fun String.exclaim() = this + "!"
来源：http://ie.huixinmuqiang.cn

[T10] Kotlin：默认参数
来源：http://ml.nszjky.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tx.yuntaijiaju.cn

[T11] Kotlin：协程
来源：http://mn.yuexingan06.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xu.asd995.cn

[T12] Kotlin：解构声明
来源：http://mp.jctech888.com.cn

val (a, b) = Pair(1, 2)
来源：http://fr.hahajie.cn

[T13] Kotlin：只读 Map
来源：http://yj.asd995.cn

val m = mapOf("a" to 1)
来源：http://rw.haigaiapp.cn

[T14] Kotlin：循环
来源：http://pv.nicolike.cn

for (i in 1..10) println(i)
来源：http://yd.shtwfgs.cn

[T15] Kotlin：接口
来源：http://oe.yuntaijiaju.cn

interface Shape { fun area(): Double }
来源：http://dg.hnjuh.cn

[T16] Swift：Hello World
来源：http://ig.chemitech.net.cn

print("Hello")
来源：http://py.huixinmuqiang.cn

[T17] Swift：变量与常量
来源：http://sq.muxihuayi.cn

var a = 1;  let b = 2
来源：http://kd.haigaiapp.cn

[T18] Swift：字符串插值
来源：http://wr.szsharing.cn

"值: \(b)"
来源：http://zk.yuntaijiaju.cn

[T19] Swift：可选绑定
来源：http://vj.huixinmuqiang.cn

if let n = opt { print(n) }
来源：http://wx.huixinmuqiang.cn

[T20] Swift：数组操作
来源：http://ms.huixiangedu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://dq.newstarts.cn

[T21] Swift：遍历
来源：http://wo.muxihuayi.cn

for x in a { print(x) }
来源：http://ph.yuexingan06.cn

[T22] Swift：字典
来源：http://oq.bjjhwx.cn

var d = ["a": 1];  d["b"] = 2
来源：http://jf.szxytkj.cn

[T23] Swift：函数
来源：http://de.gzmigu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rh.panjiajie.cn

[T24] Swift：闭包
来源：http://cm.shxzukj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://pb.nicolike.cn

[T25] Swift：结构体
来源：http://se.hnjuh.cn

struct P { var x: Int }
来源：http://zy.bjjhwx.cn

[T26] Swift：类与重写
来源：http://xo.wgjwhj.cn

class A: Base { override func f() {} }
来源：http://fz.huixinmuqiang.cn

[T27] Swift：错误处理
来源：http://bw.hnjuh.cn

do { try f() } catch { print(error) }
来源：http://qs.lnxyls.cn

[T28] Swift：枚举
来源：http://dq.nicolike.cn

enum Color { case red, green }
来源：http://ir.shtwfgs.cn

[T29] Swift：guard 提前返回
来源：http://qc.newstarts.cn

guard let x = opt else { return }
来源：http://ed.haigaiapp.cn

[T30] Swift：协议
来源：http://mq.hahajie.cn

protocol Shape { func area() -> Double }
来源：http://xp.wgjwhj.cn

[T31] Lua：Hello World
来源：http://js.yuexingan06.cn

print("Hello")
来源：http://ae.wgjwhj.cn

[T32] Lua：局部变量
来源：http://bx.huixinmuqiang.cn

local a = 1
来源：http://cy.shxzskj.cn

[T33] Lua：表（数组）
来源：http://mr.szxytkj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://gi.lnxyls.cn

[T34] Lua：遍历表
来源：http://ya.colortex.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gv.hnjuh.cn

[T35] Lua：字典表
来源：http://wk.muxihuayi.cn

local d = { a = 1 };  d.b = 2
来源：http://kf.bookmarksfly.cn

[T36] Lua：函数
来源：http://rz.yuexingan06.cn

function add(a, b) return a + b end
来源：http://ix.newstarts.cn

[T37] Lua：字符串拼接
来源：http://ej.haigaiapp.cn

"a" .. "b"
来源：http://aq.huanxung.cn

[T38] Lua：条件
来源：http://um.newstarts.cn

if x > 0 then print("正") end
来源：http://ul.wgjwhj.cn

[T39] Lua：模式匹配
来源：http://ie.szsharing.cn

string.find(s, "%d+")
来源：http://fp.jctech888.com.cn

[T40] Lua：元表
来源：http://nq.chemitech.net.cn

setmetatable({}, { __index = base })
来源：http://dq.yuntaijiaju.cn

[T41] Perl：Hello World
来源：http://as.chemitech.net.cn

print "Hello\n";
来源：http://ri.shxzukj.cn

[T42] Perl：变量类型
来源：http://iz.asd995.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jl.hahajie.cn

[T43] Perl：字符串插值
来源：http://da.asd995.cn

"值: $a"
来源：http://xt.chemitech.net.cn

[T44] Perl：条件
来源：http://gd.yuexingan06.cn

if ($a > 0) { print "正"; }
来源：http://il.bookmarksfly.cn

[T45] Perl：数组遍历
来源：http://qo.yuntaijiaju.cn

for my $x (@arr) { print $x; }
来源：http://ry.9csxet.cn

[T46] Perl：哈希操作
来源：http://uv.jianghongdianzi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mx.muxihuayi.cn

[T47] Perl：正则捕获
来源：http://yc.nicolike.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ll.nszjky.cn

[T48] Perl：正则替换
来源：http://ry.shxzskj.cn

$s =~ s/old/new/g;
来源：http://ft.shxzukj.cn

[T49] Perl：函数
来源：http://ez.newstarts.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://no.9csxet.cn

[T50] Perl：逐行读文件
来源：http://ft.gzmigu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ix.newstarts.cn

while (my $line = <$fh>) { print $line; }
来源：http://nn.huanxung.cn

[T51] Scala：Hello World
来源：http://yu.yuexingan06.cn

println("Hello")
来源：http://gt.panjiajie.cn

[T52] Scala：变量
来源：http://ti.colortex.cn

val a = 1;  var b = 2
来源：http://an.newstarts.cn

[T53] Scala：字符串插值
来源：http://jd.nicolike.cn

s"值: $b"
来源：http://ss.huanxung.cn

[T54] Scala：集合映射
来源：http://rn.bjjhwx.cn

List(1, 2, 3).map(_ * 2)
来源：http://fj.shxzukj.cn

[T55] Scala：集合过滤
来源：http://ap.asd995.cn

List(1, 2, 3).filter(_ > 1)
来源：http://jn.jianghongdianzi.cn

[T56] Scala：样例类
来源：http://uw.shxzskj.cn

case class User(name: String, age: Int)
来源：http://ig.muxihuayi.cn

[T57] Scala：模式匹配
来源：http://cp.gzmigu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://bx.muxihuayi.cn

[T58] Scala：函数定义
来源：http://pd.yuexingan06.cn

def add(a: Int, b: Int): Int = a + b
来源：http://nc.521024.cn

[T59] Scala：循环
来源：http://iw.wgjwhj.cn

for (i <- 1 to 10) println(i)
来源：http://ig.bjjhwx.cn

[T60] Scala：折叠
来源：http://mb.bjjhwx.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fw.gzmigu.cn

================================================================================
来源：http://qa.asd995.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wt.shxzskj.cn

================================================================================
来源：http://iq.bookmarksfly.cn

[U01] Py：创建虚拟环境
来源：http://zc.shxzukj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wi.panjiajie.cn

[U02] Py：导出 / 安装依赖
来源：http://tj.bjjhwx.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qe.shxzukj.cn

[U03] Py：加载 .env 配置
来源：http://oa.muxihuayi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ft.gzmigu.cn

[U04] Py：变量调试打印
来源：http://pm.bookmarksfly.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fr.newstarts.cn

[U05] Py：列表去重且保序
来源：http://mt.jctech888.com.cn

list(dict.fromkeys(arr))
来源：http://pi.jianghongdianzi.cn

[U06] Py：合并两个字典
来源：http://rl.colortex.cn

{**a, **b}
来源：http://cl.colortex.cn

[U07] Py：反转字典键值
来源：http://hj.huixiangedu.cn

{v: k for k, v in d.items()}
来源：http://si.yuntaijiaju.cn

[U08] Py：展平二维列表
来源：http://ra.nicolike.cn

[y for x in nested for y in x]
来源：http://ur.asd995.cn

[U09] Py：字典取最大值的键
来源：http://ff.huixinmuqiang.cn

max(d, key=d.get)
来源：http://zt.haigaiapp.cn

[U10] Py：按值排序字典
来源：http://sx.szxytkj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sk.yuntaijiaju.cn

[U11] Py：生成器表达式
来源：http://fs.nicolike.cn

(x * 2 for x in arr)
来源：http://ol.chemitech.net.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xj.yuexingan06.cn

Counter(arr).most_common(3)
来源：http://do.shxzskj.cn

[U13] Py：固定长度队列
来源：http://vp.huixinmuqiang.cn

deque(maxlen=10)
来源：http://uf.szxytkj.cn

[U14] Py：分组收集到列表
来源：http://ft.colortex.cn

defaultdict(list)
来源：http://wu.shxzukj.cn

[U15] Py：高精度计时
来源：http://ik.colortex.cn

t = time.perf_counter()
来源：http://sk.panjiajie.cn

[U16] Py：命令行参数解析
来源：http://fz.haigaiapp.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://br.panjiajie.cn

[U17] Py：初始化日志
来源：http://nl.huanxung.cn

logging.basicConfig(level=logging.INFO)
来源：http://zz.shtwfgs.cn

[U18] Py：预编译正则
来源：http://ze.lnxyls.cn

pat = re.compile(r"\d+")
来源：http://jn.shtwfgs.cn

[U19] Py：正则替换带回调
来源：http://su.huixinmuqiang.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tb.jctech888.com.cn

[U20] Py：缓存函数结果
来源：http://wk.hahajie.cn

@functools.lru_cache(maxsize=None)
来源：http://mh.yuntaijiaju.cn

[U21] Py：自定义上下文管理器
来源：http://tc.szxytkj.cn

@contextlib.contextmanager
来源：http://kb.bookmarksfly.cn

[U22] Py：矩阵转置
来源：http://rg.shxzukj.cn

list(zip(*m))
来源：http://ts.nicolike.cn

[U23] Py：分块读取大文件
来源：http://qd.yuntaijiaju.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fb.haigaiapp.cn

[U24] Py：路径操作
来源：http://jw.521024.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kf.nicolike.cn

[U25] Py：CSV 按字典读
来源：http://br.hnjuh.cn

csv.DictReader(f)
来源：http://mj.gzmigu.cn

[U26] Py：并发下载
来源：http://ee.lnxyls.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nr.521024.cn

[U27] Py：异步 HTTP
来源：http://pg.huixinmuqiang.cn

aiohttp.ClientSession() 配合 async with
来源：http://jp.huixinmuqiang.cn

[U28] Py：类型别名
来源：http://rx.nszjky.cn

UserId = int
来源：http://rn.gzmigu.cn

[U29] Py：属性校验
来源：http://ct.hnjuh.cn

@property 与 @x.setter 配合
来源：http://qf.yuexingan06.cn

[U30] Py：数据类
来源：http://cd.panjiajie.cn

@dataclass(slots=True)
来源：http://nw.9csxet.cn

[U31] Py：单测
来源：http://qe.hahajie.cn

python -m pytest -q
来源：http://sx.9csxet.cn

[U32] Py：代码格式化
来源：http://ej.colortex.cn

ruff format . && ruff check --fix .
来源：http://av.yuntaijiaju.cn


<!-- 参考信息 -->