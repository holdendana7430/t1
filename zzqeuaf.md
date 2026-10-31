代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sn.521024.cn

[S10] C：指针与解引用
来源：http://uf.jianghongdianzi.cn

int *p = &a;  *p = 5;
来源：http://ka.huixiangedu.cn

[S11] C：逐行读文件
来源：http://cz.shxzukj.cn

FILE *f = fopen("a.txt", "r");
来源：http://cu.bookmarksfly.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://td.muxihuayi.cn

fclose(f);
来源：http://dm.521024.cn

[S12] C：写文件
来源：http://dg.yuntaijiaju.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yn.bookmarksfly.cn

[S13] C：宏定义
来源：http://fk.huixiangedu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cr.colortex.cn

[S14] C：枚举
来源：http://iq.jctech888.com.cn

enum Color { RED, GREEN, BLUE };
来源：http://ko.521024.cn

[S15] C：类型转换
来源：http://sp.gzmigu.cn

(double) a / b
来源：http://pw.jctech888.com.cn

[S16] C：位操作置位
来源：http://nt.nszjky.cn

x |= (1 << 3);
来源：http://qg.chemitech.net.cn

[S17] C：安全拼接字符串
来源：http://zm.9csxet.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wc.hahajie.cn

[S18] C：命令行参数
来源：http://mw.yuexingan06.cn

int main(int argc, char **argv)
来源：http://ov.huixiangedu.cn

[S19] C：快速排序
来源：http://yz.9csxet.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gr.bookmarksfly.cn

[S20] C：二分查找
来源：http://sw.nicolike.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sm.nszjky.cn

[S21] C：字符类别判断
来源：http://cg.haigaiapp.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ou.nicolike.cn

[S22] C：字符串转数字
来源：http://wn.panjiajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://dt.muxihuayi.cn

[S23] C：随机数
来源：http://pg.nicolike.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ki.panjiajie.cn

[S24] C：获取本地时间
来源：http://fe.hahajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://oz.yuntaijiaju.cn

[S25] C：内存拷贝
来源：http://ue.hahajie.cn

memcpy(dst, src, n);
来源：http://xf.huanxung.cn

[S26] C：内存清零
来源：http://di.haigaiapp.cn

memset(a, 0, sizeof a);
来源：http://pe.haigaiapp.cn

[S27] C：定义常量
来源：http://yk.lnxyls.cn

const double PI = 3.14159;
来源：http://ey.nszjky.cn

[S28] C：静态变量
来源：http://su.bjjhwx.cn

static int counter = 0;
来源：http://yw.szsharing.cn

[S29] C：变参函数
来源：http://dl.shxzskj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gy.bjjhwx.cn

[S30] C：头文件保护
来源：http://yj.panjiajie.cn

#ifndef X_H
来源：http://pn.muxihuayi.cn

#define X_H
来源：http://qy.jctech888.com.cn

#endif
来源：http://kw.muxihuayi.cn

[S31] C++：Hello World
来源：http://gl.521024.cn

#include <iostream>
来源：http://gb.haigaiapp.cn

int main() { std::cout << "Hello\n"; }
来源：http://gb.yuexingan06.cn

[S32] C++：字符串
来源：http://ui.hahajie.cn

std::string s = "hi";  s += "!";
来源：http://sz.shxzukj.cn

[S33] C++：vector 增删
来源：http://ur.hahajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ig.muxihuayi.cn

[S34] C++：遍历 vector
来源：http://de.wgjwhj.cn

for (auto &x : v) { std::cout << x; }
来源：http://zc.hnjuh.cn

[S35] C++：map
来源：http://ot.muxihuayi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qb.colortex.cn

[S36] C++：unordered_map
来源：http://gf.szsharing.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qi.bjjhwx.cn

[S37] C++：set
来源：http://in.lnxyls.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yu.shxzukj.cn

[S38] C++：排序
来源：http://rg.jctech888.com.cn

std::sort(v.begin(), v.end());
来源：http://vp.chemitech.net.cn

[S39] C++：自定义比较器排序
来源：http://un.colortex.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tk.szxytkj.cn

[S40] C++：查找元素
来源：http://me.muxihuayi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://es.bjjhwx.cn

[S41] C++：类与构造函数
来源：http://ri.yuexingan06.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ze.lnxyls.cn

[S42] C++：继承与虚函数
来源：http://pd.muxihuayi.cn

class B : public Base { public: void f() override {} };
来源：http://ip.lnxyls.cn

[S43] C++：智能指针
来源：http://ie.bookmarksfly.cn

auto p = std::make_unique<int>(5);
来源：http://gm.szsharing.cn

[S44] C++：引用传参
来源：http://tz.lnxyls.cn

void inc(int &x) { ++x; }
来源：http://pl.panjiajie.cn

[S45] C++：lambda
来源：http://gf.jianghongdianzi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wh.jctech888.com.cn

[S46] C++：函数模板
来源：http://fu.huixinmuqiang.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gj.hahajie.cn

[S47] C++：结构化绑定遍历
来源：http://va.haigaiapp.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fd.hnjuh.cn

[S48] C++：逐行读文件
来源：http://rt.szxytkj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://bs.shxzukj.cn

while (std::getline(in, line)) { }
来源：http://jw.hnjuh.cn

[S49] C++：写文件
来源：http://nf.nszjky.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cd.nszjky.cn

[S50] C++：格式化数字
来源：http://zc.jctech888.com.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ru.muxihuayi.cn

[S51] C++：显式类型转换
来源：http://ld.newstarts.cn

static_cast<double>(a) / b
来源：http://ft.szxytkj.cn

[S52] C++：const 与 noexcept
来源：http://mm.yuntaijiaju.cn

int size() const noexcept { return n_; }
来源：http://qa.muxihuayi.cn

[S53] C++：移动语义
来源：http://fz.jianghongdianzi.cn

std::vector<int> w = std::move(v);
来源：http://fi.huixinmuqiang.cn

[S54] C++：异常处理
来源：http://vg.bjjhwx.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pd.nicolike.cn

[S55] C++：结构化绑定
来源：http://tn.asd995.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mk.jianghongdianzi.cn

[S56] C++：optional
来源：http://nh.muxihuayi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uq.bookmarksfly.cn

[S57] C++：编译期常量
来源：http://da.bookmarksfly.cn

constexpr int N = 10;
来源：http://cd.asd995.cn

[S58] C++：命名空间
来源：http://em.nicolike.cn

namespace ns { int f() { return 1; } }
来源：http://to.hahajie.cn

[S59] C++：静态断言
来源：http://lq.bjjhwx.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cr.huanxung.cn

[S60] C++：遍历并删除元素
来源：http://zm.huanxung.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://an.yuexingan06.cn

================================================================================
来源：http://km.szsharing.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wz.bookmarksfly.cn

================================================================================
来源：http://np.gzmigu.cn

[T01] Kotlin：Hello World
来源：http://ng.nszjky.cn

println("Hello")
来源：http://sj.yuexingan06.cn

[T02] Kotlin：变量
来源：http://is.panjiajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bx.wgjwhj.cn

[T03] Kotlin：字符串模板
来源：http://qv.521024.cn

"值: $b"
来源：http://jh.szxytkj.cn

[T04] Kotlin：空安全
来源：http://tg.yuexingan06.cn

val n: String? = null;  n?.length
来源：http://di.nicolike.cn

[T05] Kotlin：when 表达式
来源：http://es.jianghongdianzi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fq.jianghongdianzi.cn

[T06] Kotlin：集合映射
来源：http://uk.chemitech.net.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fs.yuntaijiaju.cn

[T07] Kotlin：集合过滤
来源：http://gd.bjjhwx.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ev.jianghongdianzi.cn

[T08] Kotlin：数据类
来源：http://ap.wgjwhj.cn

data class User(val name: String, val age: Int)
来源：http://lf.szsharing.cn

[T09] Kotlin：扩展函数
来源：http://xl.yuntaijiaju.cn

fun String.exclaim() = this + "!"
来源：http://iz.shtwfgs.cn

[T10] Kotlin：默认参数
来源：http://rw.jianghongdianzi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jl.newstarts.cn

[T11] Kotlin：协程
来源：http://kg.yuexingan06.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ev.bjjhwx.cn

[T12] Kotlin：解构声明
来源：http://mc.yuntaijiaju.cn

val (a, b) = Pair(1, 2)
来源：http://fx.szsharing.cn

[T13] Kotlin：只读 Map
来源：http://yl.nszjky.cn

val m = mapOf("a" to 1)
来源：http://po.wgjwhj.cn

[T14] Kotlin：循环
来源：http://vw.haigaiapp.cn

for (i in 1..10) println(i)
来源：http://hm.panjiajie.cn

[T15] Kotlin：接口
来源：http://fy.lnxyls.cn

interface Shape { fun area(): Double }
来源：http://qm.muxihuayi.cn

[T16] Swift：Hello World
来源：http://ld.gzmigu.cn

print("Hello")
来源：http://kg.huanxung.cn

[T17] Swift：变量与常量
来源：http://yg.hnjuh.cn

var a = 1;  let b = 2
来源：http://fk.nicolike.cn

[T18] Swift：字符串插值
来源：http://ip.bjjhwx.cn

"值: \(b)"
来源：http://nu.chemitech.net.cn

[T19] Swift：可选绑定
来源：http://mn.hnjuh.cn

if let n = opt { print(n) }
来源：http://zi.shxzskj.cn

[T20] Swift：数组操作
来源：http://yd.asd995.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ag.muxihuayi.cn

[T21] Swift：遍历
来源：http://gy.yuntaijiaju.cn

for x in a { print(x) }
来源：http://lf.9csxet.cn

[T22] Swift：字典
来源：http://qx.bjjhwx.cn

var d = ["a": 1];  d["b"] = 2
来源：http://im.shtwfgs.cn

[T23] Swift：函数
来源：http://bp.shxzukj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mm.huixiangedu.cn

[T24] Swift：闭包
来源：http://cq.yuexingan06.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zf.colortex.cn

[T25] Swift：结构体
来源：http://st.hnjuh.cn

struct P { var x: Int }
来源：http://io.szxytkj.cn

[T26] Swift：类与重写
来源：http://hi.shtwfgs.cn

class A: Base { override func f() {} }
来源：http://ra.szsharing.cn

[T27] Swift：错误处理
来源：http://tq.bookmarksfly.cn

do { try f() } catch { print(error) }
来源：http://et.muxihuayi.cn

[T28] Swift：枚举
来源：http://cf.newstarts.cn

enum Color { case red, green }
来源：http://zd.lnxyls.cn

[T29] Swift：guard 提前返回
来源：http://gs.nicolike.cn

guard let x = opt else { return }
来源：http://uc.huixiangedu.cn

[T30] Swift：协议
来源：http://rz.muxihuayi.cn

protocol Shape { func area() -> Double }
来源：http://xw.chemitech.net.cn

[T31] Lua：Hello World
来源：http://sb.huanxung.cn

print("Hello")
来源：http://br.shxzukj.cn

[T32] Lua：局部变量
来源：http://lm.szsharing.cn

local a = 1
来源：http://tg.szsharing.cn

[T33] Lua：表（数组）
来源：http://oa.521024.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wy.yuexingan06.cn

[T34] Lua：遍历表
来源：http://bh.szsharing.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zs.bookmarksfly.cn

[T35] Lua：字典表
来源：http://hy.huixiangedu.cn

local d = { a = 1 };  d.b = 2
来源：http://ay.haigaiapp.cn

[T36] Lua：函数
来源：http://bb.shxzukj.cn

function add(a, b) return a + b end
来源：http://gr.panjiajie.cn

[T37] Lua：字符串拼接
来源：http://oq.huixinmuqiang.cn

"a" .. "b"
来源：http://sl.asd995.cn

[T38] Lua：条件
来源：http://yx.wgjwhj.cn

if x > 0 then print("正") end
来源：http://on.colortex.cn

[T39] Lua：模式匹配
来源：http://id.9csxet.cn

string.find(s, "%d+")
来源：http://km.wgjwhj.cn

[T40] Lua：元表
来源：http://ss.haigaiapp.cn

setmetatable({}, { __index = base })
来源：http://dr.haigaiapp.cn

[T41] Perl：Hello World
来源：http://bq.szsharing.cn

print "Hello\n";
来源：http://mo.szxytkj.cn

[T42] Perl：变量类型
来源：http://pn.shxzukj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rz.lnxyls.cn

[T43] Perl：字符串插值
来源：http://um.shxzskj.cn

"值: $a"
来源：http://wy.yuexingan06.cn

[T44] Perl：条件
来源：http://gp.yuexingan06.cn

if ($a > 0) { print "正"; }
来源：http://vr.shtwfgs.cn

[T45] Perl：数组遍历
来源：http://bf.panjiajie.cn

for my $x (@arr) { print $x; }
来源：http://mt.szxytkj.cn

[T46] Perl：哈希操作
来源：http://vm.huixinmuqiang.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fr.nicolike.cn

[T47] Perl：正则捕获
来源：http://gi.gzmigu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://io.jianghongdianzi.cn

[T48] Perl：正则替换
来源：http://gw.muxihuayi.cn

$s =~ s/old/new/g;
来源：http://zy.yuntaijiaju.cn

[T49] Perl：函数
来源：http://gh.bjjhwx.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zw.huanxung.cn

[T50] Perl：逐行读文件
来源：http://nw.bjjhwx.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zp.newstarts.cn

while (my $line = <$fh>) { print $line; }
来源：http://or.521024.cn

[T51] Scala：Hello World
来源：http://wv.wgjwhj.cn

println("Hello")
来源：http://in.szxytkj.cn

[T52] Scala：变量
来源：http://fz.shxzukj.cn

val a = 1;  var b = 2
来源：http://qd.jianghongdianzi.cn

[T53] Scala：字符串插值
来源：http://hy.bjjhwx.cn

s"值: $b"
来源：http://vr.lnxyls.cn

[T54] Scala：集合映射
来源：http://af.asd995.cn

List(1, 2, 3).map(_ * 2)
来源：http://ll.bookmarksfly.cn

[T55] Scala：集合过滤
来源：http://lm.shtwfgs.cn

List(1, 2, 3).filter(_ > 1)
来源：http://dm.panjiajie.cn

[T56] Scala：样例类
来源：http://sv.yuntaijiaju.cn

case class User(name: String, age: Int)
来源：http://ep.colortex.cn

[T57] Scala：模式匹配
来源：http://me.shxzskj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ol.szsharing.cn

[T58] Scala：函数定义
来源：http://gk.bjjhwx.cn

def add(a: Int, b: Int): Int = a + b
来源：http://aa.haigaiapp.cn

[T59] Scala：循环
来源：http://fy.huixiangedu.cn

for (i <- 1 to 10) println(i)
来源：http://zg.9csxet.cn

[T60] Scala：折叠
来源：http://rt.bookmarksfly.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ju.shxzskj.cn

================================================================================
来源：http://lo.hnjuh.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zu.szxytkj.cn

================================================================================
来源：http://kr.bookmarksfly.cn

[U01] Py：创建虚拟环境
来源：http://zk.szxytkj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://na.haigaiapp.cn

[U02] Py：导出 / 安装依赖
来源：http://oi.nicolike.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lt.gzmigu.cn

[U03] Py：加载 .env 配置
来源：http://at.9csxet.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://nf.newstarts.cn

[U04] Py：变量调试打印
来源：http://ub.hahajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://oc.szsharing.cn

[U05] Py：列表去重且保序
来源：http://jp.chemitech.net.cn

list(dict.fromkeys(arr))
来源：http://pg.yuexingan06.cn

[U06] Py：合并两个字典
来源：http://oc.chemitech.net.cn

{**a, **b}
来源：http://jw.huixinmuqiang.cn

[U07] Py：反转字典键值
来源：http://pd.wgjwhj.cn

{v: k for k, v in d.items()}
来源：http://te.szsharing.cn

[U08] Py：展平二维列表
来源：http://jz.huixiangedu.cn

[y for x in nested for y in x]
来源：http://ac.shxzskj.cn

[U09] Py：字典取最大值的键
来源：http://sl.gzmigu.cn

max(d, key=d.get)
来源：http://vf.nicolike.cn

[U10] Py：按值排序字典
来源：http://tg.chemitech.net.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ru.muxihuayi.cn

[U11] Py：生成器表达式
来源：http://jj.lnxyls.cn

(x * 2 for x in arr)
来源：http://qm.szsharing.cn

[U12] Py：取出现最多的 3 个元素
来源：http://wz.haigaiapp.cn

Counter(arr).most_common(3)
来源：http://ro.521024.cn

[U13] Py：固定长度队列
来源：http://uv.jctech888.com.cn

deque(maxlen=10)
来源：http://ic.nszjky.cn

[U14] Py：分组收集到列表
来源：http://mt.yuntaijiaju.cn

defaultdict(list)
来源：http://uq.huixinmuqiang.cn

[U15] Py：高精度计时
来源：http://jm.chemitech.net.cn

t = time.perf_counter()
来源：http://lo.szsharing.cn

[U16] Py：命令行参数解析
来源：http://ij.wgjwhj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ab.asd995.cn

[U17] Py：初始化日志
来源：http://pf.huixinmuqiang.cn

logging.basicConfig(level=logging.INFO)
来源：http://xf.gzmigu.cn

[U18] Py：预编译正则
来源：http://ji.haigaiapp.cn

pat = re.compile(r"\d+")
来源：http://gr.nicolike.cn

[U19] Py：正则替换带回调
来源：http://uh.bjjhwx.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rd.nicolike.cn

[U20] Py：缓存函数结果
来源：http://pc.yuexingan06.cn

@functools.lru_cache(maxsize=None)
来源：http://ce.9csxet.cn

[U21] Py：自定义上下文管理器
来源：http://kc.gzmigu.cn

@contextlib.contextmanager
来源：http://ny.yuexingan06.cn

[U22] Py：矩阵转置
来源：http://cu.huixiangedu.cn

list(zip(*m))
来源：http://tj.521024.cn

[U23] Py：分块读取大文件
来源：http://ne.shxzskj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fr.panjiajie.cn

[U24] Py：路径操作
来源：http://ki.chemitech.net.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://oz.lnxyls.cn

[U25] Py：CSV 按字典读
来源：http://tj.szsharing.cn

csv.DictReader(f)
来源：http://od.hahajie.cn

[U26] Py：并发下载
来源：http://qr.shxzukj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dr.shxzukj.cn

[U27] Py：异步 HTTP
来源：http://ps.521024.cn

aiohttp.ClientSession() 配合 async with
来源：http://sr.haigaiapp.cn

[U28] Py：类型别名
来源：http://jo.szxytkj.cn

UserId = int
来源：http://gu.huixinmuqiang.cn

[U29] Py：属性校验
来源：http://nu.nszjky.cn

@property 与 @x.setter 配合
来源：http://zg.jianghongdianzi.cn

[U30] Py：数据类
来源：http://dk.wgjwhj.cn

@dataclass(slots=True)
来源：http://xz.colortex.cn

[U31] Py：单测
来源：http://ls.wgjwhj.cn

python -m pytest -q
来源：http://tz.panjiajie.cn

[U32] Py：代码格式化
来源：http://wp.9csxet.cn

ruff format . && ruff check --fix .
来源：http://tf.huixiangedu.cn


<!-- 参考信息 -->