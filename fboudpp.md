代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ia.shxzskj.cn

[S10] C：指针与解引用
来源：http://yn.hahajie.cn

int *p = &a;  *p = 5;
来源：http://oc.lnxyls.cn

[S11] C：逐行读文件
来源：http://cu.jctech888.com.cn

FILE *f = fopen("a.txt", "r");
来源：http://jj.shxzskj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hx.bjjhwx.cn

fclose(f);
来源：http://jx.haigaiapp.cn

[S12] C：写文件
来源：http://nx.lnxyls.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cm.chemitech.net.cn

[S13] C：宏定义
来源：http://xo.newstarts.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pl.bookmarksfly.cn

[S14] C：枚举
来源：http://sj.hahajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://wm.huixiangedu.cn

[S15] C：类型转换
来源：http://sw.lnxyls.cn

(double) a / b
来源：http://mi.yuexingan06.cn

[S16] C：位操作置位
来源：http://hs.wgjwhj.cn

x |= (1 << 3);
来源：http://gk.muxihuayi.cn

[S17] C：安全拼接字符串
来源：http://qd.bjjhwx.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tg.521024.cn

[S18] C：命令行参数
来源：http://hk.jianghongdianzi.cn

int main(int argc, char **argv)
来源：http://aw.shxzukj.cn

[S19] C：快速排序
来源：http://mo.hahajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://oj.shxzskj.cn

[S20] C：二分查找
来源：http://zh.huanxung.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xo.shtwfgs.cn

[S21] C：字符类别判断
来源：http://cl.huanxung.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pf.huixiangedu.cn

[S22] C：字符串转数字
来源：http://bi.lnxyls.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cu.panjiajie.cn

[S23] C：随机数
来源：http://xk.lnxyls.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kg.newstarts.cn

[S24] C：获取本地时间
来源：http://if.szxytkj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zq.shxzukj.cn

[S25] C：内存拷贝
来源：http://dt.nszjky.cn

memcpy(dst, src, n);
来源：http://dx.hnjuh.cn

[S26] C：内存清零
来源：http://te.asd995.cn

memset(a, 0, sizeof a);
来源：http://dc.shxzukj.cn

[S27] C：定义常量
来源：http://ly.chemitech.net.cn

const double PI = 3.14159;
来源：http://wx.wgjwhj.cn

[S28] C：静态变量
来源：http://ho.huixiangedu.cn

static int counter = 0;
来源：http://kb.haigaiapp.cn

[S29] C：变参函数
来源：http://dm.nicolike.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ph.bjjhwx.cn

[S30] C：头文件保护
来源：http://bt.wgjwhj.cn

#ifndef X_H
来源：http://zk.colortex.cn

#define X_H
来源：http://jq.huixiangedu.cn

#endif
来源：http://bv.huixiangedu.cn

[S31] C++：Hello World
来源：http://xl.huanxung.cn

#include <iostream>
来源：http://az.lnxyls.cn

int main() { std::cout << "Hello\n"; }
来源：http://qk.jctech888.com.cn

[S32] C++：字符串
来源：http://at.asd995.cn

std::string s = "hi";  s += "!";
来源：http://pf.shxzukj.cn

[S33] C++：vector 增删
来源：http://xn.asd995.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jw.521024.cn

[S34] C++：遍历 vector
来源：http://ip.lnxyls.cn

for (auto &x : v) { std::cout << x; }
来源：http://lk.chemitech.net.cn

[S35] C++：map
来源：http://nh.asd995.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lw.521024.cn

[S36] C++：unordered_map
来源：http://ts.huixiangedu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://eq.muxihuayi.cn

[S37] C++：set
来源：http://wk.szsharing.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xb.chemitech.net.cn

[S38] C++：排序
来源：http://wp.newstarts.cn

std::sort(v.begin(), v.end());
来源：http://vs.hahajie.cn

[S39] C++：自定义比较器排序
来源：http://lu.jianghongdianzi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mz.chemitech.net.cn

[S40] C++：查找元素
来源：http://ay.hnjuh.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cu.bjjhwx.cn

[S41] C++：类与构造函数
来源：http://mp.nicolike.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nh.521024.cn

[S42] C++：继承与虚函数
来源：http://ac.szsharing.cn

class B : public Base { public: void f() override {} };
来源：http://ec.huixinmuqiang.cn

[S43] C++：智能指针
来源：http://mi.9csxet.cn

auto p = std::make_unique<int>(5);
来源：http://og.szsharing.cn

[S44] C++：引用传参
来源：http://on.huixiangedu.cn

void inc(int &x) { ++x; }
来源：http://ai.yuntaijiaju.cn

[S45] C++：lambda
来源：http://ih.colortex.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hm.asd995.cn

[S46] C++：函数模板
来源：http://og.nszjky.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xy.lnxyls.cn

[S47] C++：结构化绑定遍历
来源：http://ku.haigaiapp.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pa.haigaiapp.cn

[S48] C++：逐行读文件
来源：http://vd.shxzskj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://iv.huixinmuqiang.cn

while (std::getline(in, line)) { }
来源：http://nv.muxihuayi.cn

[S49] C++：写文件
来源：http://gh.asd995.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yc.nicolike.cn

[S50] C++：格式化数字
来源：http://sm.hahajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ki.shtwfgs.cn

[S51] C++：显式类型转换
来源：http://ma.chemitech.net.cn

static_cast<double>(a) / b
来源：http://hu.hahajie.cn

[S52] C++：const 与 noexcept
来源：http://ls.jctech888.com.cn

int size() const noexcept { return n_; }
来源：http://gh.bjjhwx.cn

[S53] C++：移动语义
来源：http://ti.haigaiapp.cn

std::vector<int> w = std::move(v);
来源：http://fs.9csxet.cn

[S54] C++：异常处理
来源：http://tp.yuntaijiaju.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hb.jianghongdianzi.cn

[S55] C++：结构化绑定
来源：http://ti.wgjwhj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://hk.nszjky.cn

[S56] C++：optional
来源：http://wy.9csxet.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jr.szsharing.cn

[S57] C++：编译期常量
来源：http://qb.gzmigu.cn

constexpr int N = 10;
来源：http://hy.bookmarksfly.cn

[S58] C++：命名空间
来源：http://zs.chemitech.net.cn

namespace ns { int f() { return 1; } }
来源：http://cb.muxihuayi.cn

[S59] C++：静态断言
来源：http://us.szxytkj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://st.panjiajie.cn

[S60] C++：遍历并删除元素
来源：http://ra.muxihuayi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gv.colortex.cn

================================================================================
来源：http://va.jianghongdianzi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://la.wgjwhj.cn

================================================================================
来源：http://ap.haigaiapp.cn

[T01] Kotlin：Hello World
来源：http://pq.muxihuayi.cn

println("Hello")
来源：http://hy.newstarts.cn

[T02] Kotlin：变量
来源：http://ox.haigaiapp.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sp.chemitech.net.cn

[T03] Kotlin：字符串模板
来源：http://ip.shxzskj.cn

"值: $b"
来源：http://wl.yuntaijiaju.cn

[T04] Kotlin：空安全
来源：http://hb.chemitech.net.cn

val n: String? = null;  n?.length
来源：http://ok.panjiajie.cn

[T05] Kotlin：when 表达式
来源：http://vp.gzmigu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ab.szsharing.cn

[T06] Kotlin：集合映射
来源：http://ci.hnjuh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://nv.jctech888.com.cn

[T07] Kotlin：集合过滤
来源：http://it.huixinmuqiang.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vm.9csxet.cn

[T08] Kotlin：数据类
来源：http://vo.shxzukj.cn

data class User(val name: String, val age: Int)
来源：http://ih.521024.cn

[T09] Kotlin：扩展函数
来源：http://ue.nicolike.cn

fun String.exclaim() = this + "!"
来源：http://rz.shxzukj.cn

[T10] Kotlin：默认参数
来源：http://nj.shxzskj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ms.bookmarksfly.cn

[T11] Kotlin：协程
来源：http://gi.asd995.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://th.shxzukj.cn

[T12] Kotlin：解构声明
来源：http://bz.newstarts.cn

val (a, b) = Pair(1, 2)
来源：http://cu.9csxet.cn

[T13] Kotlin：只读 Map
来源：http://xm.wgjwhj.cn

val m = mapOf("a" to 1)
来源：http://be.hnjuh.cn

[T14] Kotlin：循环
来源：http://ib.muxihuayi.cn

for (i in 1..10) println(i)
来源：http://pi.521024.cn

[T15] Kotlin：接口
来源：http://qb.nicolike.cn

interface Shape { fun area(): Double }
来源：http://xx.hnjuh.cn

[T16] Swift：Hello World
来源：http://cm.yuntaijiaju.cn

print("Hello")
来源：http://ei.hnjuh.cn

[T17] Swift：变量与常量
来源：http://ss.nszjky.cn

var a = 1;  let b = 2
来源：http://iz.nszjky.cn

[T18] Swift：字符串插值
来源：http://ha.yuntaijiaju.cn

"值: \(b)"
来源：http://ip.szsharing.cn

[T19] Swift：可选绑定
来源：http://io.jctech888.com.cn

if let n = opt { print(n) }
来源：http://qv.yuexingan06.cn

[T20] Swift：数组操作
来源：http://jc.wgjwhj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xd.nicolike.cn

[T21] Swift：遍历
来源：http://le.jctech888.com.cn

for x in a { print(x) }
来源：http://cj.yuexingan06.cn

[T22] Swift：字典
来源：http://io.hnjuh.cn

var d = ["a": 1];  d["b"] = 2
来源：http://wt.szsharing.cn

[T23] Swift：函数
来源：http://xl.shxzukj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ut.yuntaijiaju.cn

[T24] Swift：闭包
来源：http://yi.asd995.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ku.yuexingan06.cn

[T25] Swift：结构体
来源：http://yv.shxzukj.cn

struct P { var x: Int }
来源：http://xz.haigaiapp.cn

[T26] Swift：类与重写
来源：http://cm.huixinmuqiang.cn

class A: Base { override func f() {} }
来源：http://ok.huixiangedu.cn

[T27] Swift：错误处理
来源：http://yc.wgjwhj.cn

do { try f() } catch { print(error) }
来源：http://sy.shtwfgs.cn

[T28] Swift：枚举
来源：http://rx.hahajie.cn

enum Color { case red, green }
来源：http://ga.huixinmuqiang.cn

[T29] Swift：guard 提前返回
来源：http://sb.bookmarksfly.cn

guard let x = opt else { return }
来源：http://rt.521024.cn

[T30] Swift：协议
来源：http://xq.szxytkj.cn

protocol Shape { func area() -> Double }
来源：http://ic.lnxyls.cn

[T31] Lua：Hello World
来源：http://tn.jctech888.com.cn

print("Hello")
来源：http://iu.jctech888.com.cn

[T32] Lua：局部变量
来源：http://yu.huanxung.cn

local a = 1
来源：http://pl.nszjky.cn

[T33] Lua：表（数组）
来源：http://jq.9csxet.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://nw.chemitech.net.cn

[T34] Lua：遍历表
来源：http://tx.huanxung.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://lt.newstarts.cn

[T35] Lua：字典表
来源：http://wl.nicolike.cn

local d = { a = 1 };  d.b = 2
来源：http://mg.asd995.cn

[T36] Lua：函数
来源：http://yy.colortex.cn

function add(a, b) return a + b end
来源：http://ei.muxihuayi.cn

[T37] Lua：字符串拼接
来源：http://gz.wgjwhj.cn

"a" .. "b"
来源：http://nw.asd995.cn

[T38] Lua：条件
来源：http://ka.shtwfgs.cn

if x > 0 then print("正") end
来源：http://yh.521024.cn

[T39] Lua：模式匹配
来源：http://wv.gzmigu.cn

string.find(s, "%d+")
来源：http://zt.chemitech.net.cn

[T40] Lua：元表
来源：http://bb.yuntaijiaju.cn

setmetatable({}, { __index = base })
来源：http://vv.panjiajie.cn

[T41] Perl：Hello World
来源：http://tl.jianghongdianzi.cn

print "Hello\n";
来源：http://ee.bookmarksfly.cn

[T42] Perl：变量类型
来源：http://kp.hahajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tj.nicolike.cn

[T43] Perl：字符串插值
来源：http://gq.huixiangedu.cn

"值: $a"
来源：http://zm.bjjhwx.cn

[T44] Perl：条件
来源：http://pd.chemitech.net.cn

if ($a > 0) { print "正"; }
来源：http://zj.bookmarksfly.cn

[T45] Perl：数组遍历
来源：http://gh.muxihuayi.cn

for my $x (@arr) { print $x; }
来源：http://gm.huixinmuqiang.cn

[T46] Perl：哈希操作
来源：http://yn.bookmarksfly.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vm.hnjuh.cn

[T47] Perl：正则捕获
来源：http://gn.shxzukj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wq.panjiajie.cn

[T48] Perl：正则替换
来源：http://ex.bookmarksfly.cn

$s =~ s/old/new/g;
来源：http://zr.9csxet.cn

[T49] Perl：函数
来源：http://sv.nszjky.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qq.nicolike.cn

[T50] Perl：逐行读文件
来源：http://ej.shtwfgs.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fn.wgjwhj.cn

while (my $line = <$fh>) { print $line; }
来源：http://bd.huixiangedu.cn

[T51] Scala：Hello World
来源：http://lo.hnjuh.cn

println("Hello")
来源：http://nv.huanxung.cn

[T52] Scala：变量
来源：http://iu.huixinmuqiang.cn

val a = 1;  var b = 2
来源：http://ct.shxzskj.cn

[T53] Scala：字符串插值
来源：http://dz.bjjhwx.cn

s"值: $b"
来源：http://os.bjjhwx.cn

[T54] Scala：集合映射
来源：http://af.huixiangedu.cn

List(1, 2, 3).map(_ * 2)
来源：http://cj.lnxyls.cn

[T55] Scala：集合过滤
来源：http://jp.9csxet.cn

List(1, 2, 3).filter(_ > 1)
来源：http://vw.chemitech.net.cn

[T56] Scala：样例类
来源：http://km.chemitech.net.cn

case class User(name: String, age: Int)
来源：http://ce.yuntaijiaju.cn

[T57] Scala：模式匹配
来源：http://cd.szsharing.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fc.9csxet.cn

[T58] Scala：函数定义
来源：http://rn.hahajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ug.9csxet.cn

[T59] Scala：循环
来源：http://gv.newstarts.cn

for (i <- 1 to 10) println(i)
来源：http://am.nicolike.cn

[T60] Scala：折叠
来源：http://qe.panjiajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pq.asd995.cn

================================================================================
来源：http://nc.asd995.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qg.lnxyls.cn

================================================================================
来源：http://jh.shxzukj.cn

[U01] Py：创建虚拟环境
来源：http://fn.huixiangedu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ma.yuexingan06.cn

[U02] Py：导出 / 安装依赖
来源：http://xv.lnxyls.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qc.hnjuh.cn

[U03] Py：加载 .env 配置
来源：http://lm.colortex.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://od.yuexingan06.cn

[U04] Py：变量调试打印
来源：http://vl.huixinmuqiang.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ky.asd995.cn

[U05] Py：列表去重且保序
来源：http://un.521024.cn

list(dict.fromkeys(arr))
来源：http://sy.huixiangedu.cn

[U06] Py：合并两个字典
来源：http://jm.hnjuh.cn

{**a, **b}
来源：http://qw.hahajie.cn

[U07] Py：反转字典键值
来源：http://ed.huanxung.cn

{v: k for k, v in d.items()}
来源：http://es.huixinmuqiang.cn

[U08] Py：展平二维列表
来源：http://ed.wgjwhj.cn

[y for x in nested for y in x]
来源：http://wm.szsharing.cn

[U09] Py：字典取最大值的键
来源：http://uz.huanxung.cn

max(d, key=d.get)
来源：http://cy.shtwfgs.cn

[U10] Py：按值排序字典
来源：http://gd.huixiangedu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vd.shxzukj.cn

[U11] Py：生成器表达式
来源：http://ut.bookmarksfly.cn

(x * 2 for x in arr)
来源：http://og.shxzukj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://gy.szxytkj.cn

Counter(arr).most_common(3)
来源：http://bg.shxzskj.cn

[U13] Py：固定长度队列
来源：http://kb.9csxet.cn

deque(maxlen=10)
来源：http://gi.huixiangedu.cn

[U14] Py：分组收集到列表
来源：http://nz.asd995.cn

defaultdict(list)
来源：http://ob.asd995.cn

[U15] Py：高精度计时
来源：http://ou.asd995.cn

t = time.perf_counter()
来源：http://mb.jianghongdianzi.cn

[U16] Py：命令行参数解析
来源：http://tx.shxzskj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://uh.521024.cn

[U17] Py：初始化日志
来源：http://fi.nszjky.cn

logging.basicConfig(level=logging.INFO)
来源：http://oj.gzmigu.cn

[U18] Py：预编译正则
来源：http://yh.shxzskj.cn

pat = re.compile(r"\d+")
来源：http://fj.haigaiapp.cn

[U19] Py：正则替换带回调
来源：http://qr.yuntaijiaju.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zh.yuntaijiaju.cn

[U20] Py：缓存函数结果
来源：http://fn.huixinmuqiang.cn

@functools.lru_cache(maxsize=None)
来源：http://kf.bjjhwx.cn

[U21] Py：自定义上下文管理器
来源：http://wx.shxzskj.cn

@contextlib.contextmanager
来源：http://eu.nicolike.cn

[U22] Py：矩阵转置
来源：http://lk.huixiangedu.cn

list(zip(*m))
来源：http://nu.shxzukj.cn

[U23] Py：分块读取大文件
来源：http://ij.hnjuh.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dh.asd995.cn

[U24] Py：路径操作
来源：http://sk.panjiajie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xt.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://rd.9csxet.cn

csv.DictReader(f)
来源：http://vu.yuntaijiaju.cn

[U26] Py：并发下载
来源：http://kk.colortex.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hp.shxzskj.cn

[U27] Py：异步 HTTP
来源：http://oi.shxzukj.cn

aiohttp.ClientSession() 配合 async with
来源：http://us.colortex.cn

[U28] Py：类型别名
来源：http://tk.hahajie.cn

UserId = int
来源：http://iz.panjiajie.cn

[U29] Py：属性校验
来源：http://bk.szxytkj.cn

@property 与 @x.setter 配合
来源：http://ci.nicolike.cn

[U30] Py：数据类
来源：http://wv.huixiangedu.cn

@dataclass(slots=True)
来源：http://gy.gzmigu.cn

[U31] Py：单测
来源：http://xv.colortex.cn

python -m pytest -q
来源：http://cg.szxytkj.cn

[U32] Py：代码格式化
来源：http://ys.hnjuh.cn

ruff format . && ruff check --fix .
来源：http://hv.huanxung.cn


<!-- 参考信息 -->