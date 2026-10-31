代发 wailian999

strlen(s)
来源：http://ue.shtwfgs.cn

[S06] C：字符串比较
来源：http://xv.lnxyls.cn

strcmp(a, b) == 0
来源：http://tp.hnjuh.cn

[S07] C：数组遍历求和
来源：http://nc.jianghongdianzi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mv.jctech888.com.cn

[S08] C：动态内存分配与释放
来源：http://qp.colortex.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://oe.shxzskj.cn

[S09] C：结构体定义与初始化
来源：http://ph.lnxyls.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zw.shxzukj.cn

[S10] C：指针与解引用
来源：http://gv.muxihuayi.cn

int *p = &a;  *p = 5;
来源：http://ll.newstarts.cn

[S11] C：逐行读文件
来源：http://cr.gzmigu.cn

FILE *f = fopen("a.txt", "r");
来源：http://ka.muxihuayi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://cd.huanxung.cn

fclose(f);
来源：http://gt.huanxung.cn

[S12] C：写文件
来源：http://kw.huanxung.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zw.colortex.cn

[S13] C：宏定义
来源：http://no.521024.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://oq.panjiajie.cn

[S14] C：枚举
来源：http://sj.muxihuayi.cn

enum Color { RED, GREEN, BLUE };
来源：http://ru.lnxyls.cn

[S15] C：类型转换
来源：http://qi.bjjhwx.cn

(double) a / b
来源：http://dj.yuexingan06.cn

[S16] C：位操作置位
来源：http://sg.hnjuh.cn

x |= (1 << 3);
来源：http://tr.wgjwhj.cn

[S17] C：安全拼接字符串
来源：http://eg.panjiajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jy.521024.cn

[S18] C：命令行参数
来源：http://fe.bjjhwx.cn

int main(int argc, char **argv)
来源：http://wy.huixinmuqiang.cn

[S19] C：快速排序
来源：http://ip.huixiangedu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gc.hahajie.cn

[S20] C：二分查找
来源：http://ov.nszjky.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bf.shxzukj.cn

[S21] C：字符类别判断
来源：http://bl.gzmigu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ap.panjiajie.cn

[S22] C：字符串转数字
来源：http://ta.wgjwhj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://bk.colortex.cn

[S23] C：随机数
来源：http://lw.jianghongdianzi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zk.chemitech.net.cn

[S24] C：获取本地时间
来源：http://ay.colortex.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pc.gzmigu.cn

[S25] C：内存拷贝
来源：http://gx.hnjuh.cn

memcpy(dst, src, n);
来源：http://tm.bjjhwx.cn

[S26] C：内存清零
来源：http://wr.521024.cn

memset(a, 0, sizeof a);
来源：http://hl.haigaiapp.cn

[S27] C：定义常量
来源：http://lq.hnjuh.cn

const double PI = 3.14159;
来源：http://te.shxzukj.cn

[S28] C：静态变量
来源：http://fg.bookmarksfly.cn

static int counter = 0;
来源：http://dt.9csxet.cn

[S29] C：变参函数
来源：http://zt.shxzskj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://my.9csxet.cn

[S30] C：头文件保护
来源：http://an.szsharing.cn

#ifndef X_H
来源：http://it.bjjhwx.cn

#define X_H
来源：http://wv.chemitech.net.cn

#endif
来源：http://gb.hahajie.cn

[S31] C++：Hello World
来源：http://pp.hahajie.cn

#include <iostream>
来源：http://lr.wgjwhj.cn

int main() { std::cout << "Hello\n"; }
来源：http://ch.9csxet.cn

[S32] C++：字符串
来源：http://ij.lnxyls.cn

std::string s = "hi";  s += "!";
来源：http://jx.chemitech.net.cn

[S33] C++：vector 增删
来源：http://qd.szsharing.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dt.haigaiapp.cn

[S34] C++：遍历 vector
来源：http://qc.521024.cn

for (auto &x : v) { std::cout << x; }
来源：http://lg.szxytkj.cn

[S35] C++：map
来源：http://hh.yuexingan06.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yy.szsharing.cn

[S36] C++：unordered_map
来源：http://pk.colortex.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jg.szxytkj.cn

[S37] C++：set
来源：http://yx.bjjhwx.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ta.hahajie.cn

[S38] C++：排序
来源：http://qu.yuntaijiaju.cn

std::sort(v.begin(), v.end());
来源：http://in.asd995.cn

[S39] C++：自定义比较器排序
来源：http://rk.hnjuh.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ue.asd995.cn

[S40] C++：查找元素
来源：http://se.9csxet.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://af.huanxung.cn

[S41] C++：类与构造函数
来源：http://kq.muxihuayi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://if.nszjky.cn

[S42] C++：继承与虚函数
来源：http://dx.wgjwhj.cn

class B : public Base { public: void f() override {} };
来源：http://fv.shxzskj.cn

[S43] C++：智能指针
来源：http://ms.jctech888.com.cn

auto p = std::make_unique<int>(5);
来源：http://la.huixiangedu.cn

[S44] C++：引用传参
来源：http://bh.huanxung.cn

void inc(int &x) { ++x; }
来源：http://uy.yuexingan06.cn

[S45] C++：lambda
来源：http://gi.szsharing.cn

auto add = [](int a, int b) { return a + b; };
来源：http://sc.shxzskj.cn

[S46] C++：函数模板
来源：http://aw.shtwfgs.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://st.yuntaijiaju.cn

[S47] C++：结构化绑定遍历
来源：http://tk.szsharing.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bx.nicolike.cn

[S48] C++：逐行读文件
来源：http://ke.521024.cn

std::ifstream in("a.txt");  std::string line;
来源：http://tt.nicolike.cn

while (std::getline(in, line)) { }
来源：http://by.9csxet.cn

[S49] C++：写文件
来源：http://rb.bookmarksfly.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ix.521024.cn

[S50] C++：格式化数字
来源：http://gx.521024.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kc.shxzskj.cn

[S51] C++：显式类型转换
来源：http://ck.huanxung.cn

static_cast<double>(a) / b
来源：http://nc.9csxet.cn

[S52] C++：const 与 noexcept
来源：http://nd.muxihuayi.cn

int size() const noexcept { return n_; }
来源：http://mf.yuexingan06.cn

[S53] C++：移动语义
来源：http://lo.bookmarksfly.cn

std::vector<int> w = std::move(v);
来源：http://qh.bookmarksfly.cn

[S54] C++：异常处理
来源：http://kb.panjiajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dv.asd995.cn

[S55] C++：结构化绑定
来源：http://ll.huixinmuqiang.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fl.szxytkj.cn

[S56] C++：optional
来源：http://lw.huixiangedu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ik.colortex.cn

[S57] C++：编译期常量
来源：http://xa.huixiangedu.cn

constexpr int N = 10;
来源：http://yf.bookmarksfly.cn

[S58] C++：命名空间
来源：http://nj.panjiajie.cn

namespace ns { int f() { return 1; } }
来源：http://wp.shxzukj.cn

[S59] C++：静态断言
来源：http://aj.bookmarksfly.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jv.haigaiapp.cn

[S60] C++：遍历并删除元素
来源：http://ul.gzmigu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kl.shxzskj.cn

================================================================================
来源：http://de.huixiangedu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dc.yuntaijiaju.cn

================================================================================
来源：http://zd.colortex.cn

[T01] Kotlin：Hello World
来源：http://id.huanxung.cn

println("Hello")
来源：http://lu.9csxet.cn

[T02] Kotlin：变量
来源：http://fm.panjiajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jl.shtwfgs.cn

[T03] Kotlin：字符串模板
来源：http://ug.gzmigu.cn

"值: $b"
来源：http://sj.szxytkj.cn

[T04] Kotlin：空安全
来源：http://mv.huixiangedu.cn

val n: String? = null;  n?.length
来源：http://mt.nicolike.cn

[T05] Kotlin：when 表达式
来源：http://zj.hahajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vn.huanxung.cn

[T06] Kotlin：集合映射
来源：http://cz.colortex.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ro.muxihuayi.cn

[T07] Kotlin：集合过滤
来源：http://lt.9csxet.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://of.shxzskj.cn

[T08] Kotlin：数据类
来源：http://sy.huanxung.cn

data class User(val name: String, val age: Int)
来源：http://ov.huanxung.cn

[T09] Kotlin：扩展函数
来源：http://qe.huixinmuqiang.cn

fun String.exclaim() = this + "!"
来源：http://yw.colortex.cn

[T10] Kotlin：默认参数
来源：http://ll.shxzukj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pk.panjiajie.cn

[T11] Kotlin：协程
来源：http://ko.szsharing.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://cx.yuexingan06.cn

[T12] Kotlin：解构声明
来源：http://ur.yuntaijiaju.cn

val (a, b) = Pair(1, 2)
来源：http://ob.yuexingan06.cn

[T13] Kotlin：只读 Map
来源：http://fq.colortex.cn

val m = mapOf("a" to 1)
来源：http://kb.haigaiapp.cn

[T14] Kotlin：循环
来源：http://yu.9csxet.cn

for (i in 1..10) println(i)
来源：http://ck.nicolike.cn

[T15] Kotlin：接口
来源：http://cl.shxzukj.cn

interface Shape { fun area(): Double }
来源：http://lc.nicolike.cn

[T16] Swift：Hello World
来源：http://jx.shtwfgs.cn

print("Hello")
来源：http://dk.huixiangedu.cn

[T17] Swift：变量与常量
来源：http://pc.colortex.cn

var a = 1;  let b = 2
来源：http://ka.bjjhwx.cn

[T18] Swift：字符串插值
来源：http://sx.wgjwhj.cn

"值: \(b)"
来源：http://zt.jianghongdianzi.cn

[T19] Swift：可选绑定
来源：http://jm.szsharing.cn

if let n = opt { print(n) }
来源：http://le.nszjky.cn

[T20] Swift：数组操作
来源：http://ff.huanxung.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ro.nicolike.cn

[T21] Swift：遍历
来源：http://rg.szxytkj.cn

for x in a { print(x) }
来源：http://pk.521024.cn

[T22] Swift：字典
来源：http://er.lnxyls.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ec.shtwfgs.cn

[T23] Swift：函数
来源：http://vx.szxytkj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bi.yuntaijiaju.cn

[T24] Swift：闭包
来源：http://iv.szsharing.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://wa.panjiajie.cn

[T25] Swift：结构体
来源：http://vs.chemitech.net.cn

struct P { var x: Int }
来源：http://sl.chemitech.net.cn

[T26] Swift：类与重写
来源：http://ff.bookmarksfly.cn

class A: Base { override func f() {} }
来源：http://np.jctech888.com.cn

[T27] Swift：错误处理
来源：http://cd.szsharing.cn

do { try f() } catch { print(error) }
来源：http://ep.yuexingan06.cn

[T28] Swift：枚举
来源：http://bn.colortex.cn

enum Color { case red, green }
来源：http://ds.nszjky.cn

[T29] Swift：guard 提前返回
来源：http://ny.yuntaijiaju.cn

guard let x = opt else { return }
来源：http://cb.9csxet.cn

[T30] Swift：协议
来源：http://ix.shxzukj.cn

protocol Shape { func area() -> Double }
来源：http://yt.yuexingan06.cn

[T31] Lua：Hello World
来源：http://wk.panjiajie.cn

print("Hello")
来源：http://pn.bookmarksfly.cn

[T32] Lua：局部变量
来源：http://yv.nszjky.cn

local a = 1
来源：http://re.9csxet.cn

[T33] Lua：表（数组）
来源：http://xp.newstarts.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ts.hahajie.cn

[T34] Lua：遍历表
来源：http://hd.nszjky.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ra.hahajie.cn

[T35] Lua：字典表
来源：http://rz.chemitech.net.cn

local d = { a = 1 };  d.b = 2
来源：http://rq.jianghongdianzi.cn

[T36] Lua：函数
来源：http://qb.colortex.cn

function add(a, b) return a + b end
来源：http://ds.jctech888.com.cn

[T37] Lua：字符串拼接
来源：http://yp.chemitech.net.cn

"a" .. "b"
来源：http://xe.huixinmuqiang.cn

[T38] Lua：条件
来源：http://hr.shxzukj.cn

if x > 0 then print("正") end
来源：http://be.muxihuayi.cn

[T39] Lua：模式匹配
来源：http://wn.muxihuayi.cn

string.find(s, "%d+")
来源：http://ve.jctech888.com.cn

[T40] Lua：元表
来源：http://gt.shxzskj.cn

setmetatable({}, { __index = base })
来源：http://sc.colortex.cn

[T41] Perl：Hello World
来源：http://fm.wgjwhj.cn

print "Hello\n";
来源：http://tz.shtwfgs.cn

[T42] Perl：变量类型
来源：http://cg.huixiangedu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://os.hahajie.cn

[T43] Perl：字符串插值
来源：http://la.muxihuayi.cn

"值: $a"
来源：http://fn.9csxet.cn

[T44] Perl：条件
来源：http://tk.chemitech.net.cn

if ($a > 0) { print "正"; }
来源：http://kg.colortex.cn

[T45] Perl：数组遍历
来源：http://qj.szxytkj.cn

for my $x (@arr) { print $x; }
来源：http://cn.bookmarksfly.cn

[T46] Perl：哈希操作
来源：http://cq.panjiajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nb.nicolike.cn

[T47] Perl：正则捕获
来源：http://jx.bookmarksfly.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://lt.huixiangedu.cn

[T48] Perl：正则替换
来源：http://ze.jianghongdianzi.cn

$s =~ s/old/new/g;
来源：http://km.huixiangedu.cn

[T49] Perl：函数
来源：http://ra.gzmigu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lk.jianghongdianzi.cn

[T50] Perl：逐行读文件
来源：http://la.yuntaijiaju.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://yp.panjiajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://ux.nicolike.cn

[T51] Scala：Hello World
来源：http://zg.lnxyls.cn

println("Hello")
来源：http://fg.lnxyls.cn

[T52] Scala：变量
来源：http://yg.panjiajie.cn

val a = 1;  var b = 2
来源：http://en.bjjhwx.cn

[T53] Scala：字符串插值
来源：http://sv.lnxyls.cn

s"值: $b"
来源：http://zo.nszjky.cn

[T54] Scala：集合映射
来源：http://tw.muxihuayi.cn

List(1, 2, 3).map(_ * 2)
来源：http://kn.newstarts.cn

[T55] Scala：集合过滤
来源：http://om.newstarts.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wa.asd995.cn

[T56] Scala：样例类
来源：http://zq.bookmarksfly.cn

case class User(name: String, age: Int)
来源：http://ex.nicolike.cn

[T57] Scala：模式匹配
来源：http://dn.huixinmuqiang.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ai.gzmigu.cn

[T58] Scala：函数定义
来源：http://ja.shtwfgs.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gv.haigaiapp.cn

[T59] Scala：循环
来源：http://zy.jctech888.com.cn

for (i <- 1 to 10) println(i)
来源：http://jf.panjiajie.cn

[T60] Scala：折叠
来源：http://nc.bjjhwx.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ub.jctech888.com.cn

================================================================================
来源：http://zi.asd995.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ed.nicolike.cn

================================================================================
来源：http://ik.asd995.cn

[U01] Py：创建虚拟环境
来源：http://vp.huanxung.cn

python -m venv .venv && source .venv/bin/activate
来源：http://pj.panjiajie.cn

[U02] Py：导出 / 安装依赖
来源：http://kv.muxihuayi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bk.9csxet.cn

[U03] Py：加载 .env 配置
来源：http://ow.huixinmuqiang.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wi.nicolike.cn

[U04] Py：变量调试打印
来源：http://uu.shxzukj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ze.chemitech.net.cn

[U05] Py：列表去重且保序
来源：http://po.szxytkj.cn

list(dict.fromkeys(arr))
来源：http://pp.nicolike.cn

[U06] Py：合并两个字典
来源：http://ft.bookmarksfly.cn

{**a, **b}
来源：http://oh.huixiangedu.cn

[U07] Py：反转字典键值
来源：http://bv.521024.cn

{v: k for k, v in d.items()}
来源：http://wn.wgjwhj.cn

[U08] Py：展平二维列表
来源：http://fk.521024.cn

[y for x in nested for y in x]
来源：http://wk.chemitech.net.cn

[U09] Py：字典取最大值的键
来源：http://ks.yuexingan06.cn

max(d, key=d.get)
来源：http://cz.wgjwhj.cn

[U10] Py：按值排序字典
来源：http://mv.muxihuayi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zp.szsharing.cn

[U11] Py：生成器表达式
来源：http://ln.huanxung.cn

(x * 2 for x in arr)
来源：http://ga.lnxyls.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lt.asd995.cn

Counter(arr).most_common(3)
来源：http://zi.szsharing.cn

[U13] Py：固定长度队列
来源：http://if.wgjwhj.cn

deque(maxlen=10)
来源：http://db.hnjuh.cn

[U14] Py：分组收集到列表
来源：http://hy.szsharing.cn

defaultdict(list)
来源：http://ue.haigaiapp.cn

[U15] Py：高精度计时
来源：http://jf.haigaiapp.cn

t = time.perf_counter()
来源：http://uy.huixinmuqiang.cn

[U16] Py：命令行参数解析
来源：http://fk.hahajie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pc.gzmigu.cn

[U17] Py：初始化日志
来源：http://is.muxihuayi.cn

logging.basicConfig(level=logging.INFO)
来源：http://fk.gzmigu.cn

[U18] Py：预编译正则
来源：http://tp.yuntaijiaju.cn

pat = re.compile(r"\d+")
来源：http://ol.asd995.cn

[U19] Py：正则替换带回调
来源：http://yl.haigaiapp.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jk.shtwfgs.cn

[U20] Py：缓存函数结果
来源：http://du.szxytkj.cn

@functools.lru_cache(maxsize=None)
来源：http://nc.jianghongdianzi.cn

[U21] Py：自定义上下文管理器
来源：http://if.haigaiapp.cn

@contextlib.contextmanager
来源：http://mg.shtwfgs.cn

[U22] Py：矩阵转置
来源：http://vi.bookmarksfly.cn

list(zip(*m))
来源：http://eo.huanxung.cn

[U23] Py：分块读取大文件
来源：http://zl.lnxyls.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fh.9csxet.cn

[U24] Py：路径操作
来源：http://rr.jianghongdianzi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rm.asd995.cn

[U25] Py：CSV 按字典读
来源：http://xy.huixinmuqiang.cn

csv.DictReader(f)
来源：http://dw.newstarts.cn

[U26] Py：并发下载
来源：http://us.colortex.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wn.gzmigu.cn

[U27] Py：异步 HTTP
来源：http://ep.asd995.cn

aiohttp.ClientSession() 配合 async with
来源：http://vi.colortex.cn

[U28] Py：类型别名
来源：http://gi.nszjky.cn

UserId = int
来源：http://hi.nszjky.cn


<!-- 参考信息 -->