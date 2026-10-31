代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gy.hahajie.cn

[S10] C：指针与解引用
来源：http://px.asd995.cn

int *p = &a;  *p = 5;
来源：http://eb.chemitech.net.cn

[S11] C：逐行读文件
来源：http://wq.shtwfgs.cn

FILE *f = fopen("a.txt", "r");
来源：http://lx.muxihuayi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qn.huanxung.cn

fclose(f);
来源：http://os.9csxet.cn

[S12] C：写文件
来源：http://gc.shxzskj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ec.jianghongdianzi.cn

[S13] C：宏定义
来源：http://xx.szxytkj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jm.521024.cn

[S14] C：枚举
来源：http://sq.haigaiapp.cn

enum Color { RED, GREEN, BLUE };
来源：http://ds.yuexingan06.cn

[S15] C：类型转换
来源：http://oe.haigaiapp.cn

(double) a / b
来源：http://re.muxihuayi.cn

[S16] C：位操作置位
来源：http://fe.bookmarksfly.cn

x |= (1 << 3);
来源：http://qk.hahajie.cn

[S17] C：安全拼接字符串
来源：http://ou.haigaiapp.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://am.shtwfgs.cn

[S18] C：命令行参数
来源：http://jf.haigaiapp.cn

int main(int argc, char **argv)
来源：http://kh.hahajie.cn

[S19] C：快速排序
来源：http://rh.shxzskj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ti.hnjuh.cn

[S20] C：二分查找
来源：http://kt.shxzskj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dq.huixiangedu.cn

[S21] C：字符类别判断
来源：http://xr.chemitech.net.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lx.bjjhwx.cn

[S22] C：字符串转数字
来源：http://op.shtwfgs.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rk.huanxung.cn

[S23] C：随机数
来源：http://sh.hahajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ib.lnxyls.cn

[S24] C：获取本地时间
来源：http://bk.shxzskj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dc.colortex.cn

[S25] C：内存拷贝
来源：http://mt.yuexingan06.cn

memcpy(dst, src, n);
来源：http://ri.panjiajie.cn

[S26] C：内存清零
来源：http://bl.9csxet.cn

memset(a, 0, sizeof a);
来源：http://cu.hahajie.cn

[S27] C：定义常量
来源：http://jk.nszjky.cn

const double PI = 3.14159;
来源：http://ik.colortex.cn

[S28] C：静态变量
来源：http://fw.haigaiapp.cn

static int counter = 0;
来源：http://hp.shxzskj.cn

[S29] C：变参函数
来源：http://oh.colortex.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://js.panjiajie.cn

[S30] C：头文件保护
来源：http://yd.jianghongdianzi.cn

#ifndef X_H
来源：http://nc.huixinmuqiang.cn

#define X_H
来源：http://ky.huixiangedu.cn

#endif
来源：http://mb.szsharing.cn

[S31] C++：Hello World
来源：http://fo.shxzukj.cn

#include <iostream>
来源：http://no.muxihuayi.cn

int main() { std::cout << "Hello\n"; }
来源：http://ds.nicolike.cn

[S32] C++：字符串
来源：http://qd.bjjhwx.cn

std::string s = "hi";  s += "!";
来源：http://wj.jctech888.com.cn

[S33] C++：vector 增删
来源：http://uf.nicolike.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gw.haigaiapp.cn

[S34] C++：遍历 vector
来源：http://rf.lnxyls.cn

for (auto &x : v) { std::cout << x; }
来源：http://pi.shtwfgs.cn

[S35] C++：map
来源：http://su.yuntaijiaju.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tb.panjiajie.cn

[S36] C++：unordered_map
来源：http://vn.jianghongdianzi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mr.jctech888.com.cn

[S37] C++：set
来源：http://xv.colortex.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rq.yuexingan06.cn

[S38] C++：排序
来源：http://no.bjjhwx.cn

std::sort(v.begin(), v.end());
来源：http://cs.9csxet.cn

[S39] C++：自定义比较器排序
来源：http://no.9csxet.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sw.panjiajie.cn

[S40] C++：查找元素
来源：http://ba.9csxet.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mt.panjiajie.cn

[S41] C++：类与构造函数
来源：http://yl.lnxyls.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rr.colortex.cn

[S42] C++：继承与虚函数
来源：http://we.shxzukj.cn

class B : public Base { public: void f() override {} };
来源：http://nt.chemitech.net.cn

[S43] C++：智能指针
来源：http://bo.nszjky.cn

auto p = std::make_unique<int>(5);
来源：http://ay.chemitech.net.cn

[S44] C++：引用传参
来源：http://tp.chemitech.net.cn

void inc(int &x) { ++x; }
来源：http://ix.jianghongdianzi.cn

[S45] C++：lambda
来源：http://fv.wgjwhj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ug.asd995.cn

[S46] C++：函数模板
来源：http://tu.szxytkj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ue.colortex.cn

[S47] C++：结构化绑定遍历
来源：http://yp.hnjuh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rr.shxzukj.cn

[S48] C++：逐行读文件
来源：http://kh.nicolike.cn

std::ifstream in("a.txt");  std::string line;
来源：http://cw.bookmarksfly.cn

while (std::getline(in, line)) { }
来源：http://cg.chemitech.net.cn

[S49] C++：写文件
来源：http://bv.shxzskj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hw.lnxyls.cn

[S50] C++：格式化数字
来源：http://cz.hnjuh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vu.hnjuh.cn

[S51] C++：显式类型转换
来源：http://ky.nszjky.cn

static_cast<double>(a) / b
来源：http://gd.haigaiapp.cn

[S52] C++：const 与 noexcept
来源：http://vx.panjiajie.cn

int size() const noexcept { return n_; }
来源：http://jw.nszjky.cn

[S53] C++：移动语义
来源：http://ac.newstarts.cn

std::vector<int> w = std::move(v);
来源：http://dq.muxihuayi.cn

[S54] C++：异常处理
来源：http://nk.bookmarksfly.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cc.yuntaijiaju.cn

[S55] C++：结构化绑定
来源：http://kj.bookmarksfly.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jn.shtwfgs.cn

[S56] C++：optional
来源：http://sj.asd995.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zk.bookmarksfly.cn

[S57] C++：编译期常量
来源：http://mv.szxytkj.cn

constexpr int N = 10;
来源：http://nq.shxzskj.cn

[S58] C++：命名空间
来源：http://xs.panjiajie.cn

namespace ns { int f() { return 1; } }
来源：http://tw.haigaiapp.cn

[S59] C++：静态断言
来源：http://if.lnxyls.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://px.colortex.cn

[S60] C++：遍历并删除元素
来源：http://ig.bjjhwx.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kw.haigaiapp.cn

================================================================================
来源：http://yw.9csxet.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mw.szxytkj.cn

================================================================================
来源：http://ts.haigaiapp.cn

[T01] Kotlin：Hello World
来源：http://mh.asd995.cn

println("Hello")
来源：http://hx.huixiangedu.cn

[T02] Kotlin：变量
来源：http://mc.shxzskj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sy.hnjuh.cn

[T03] Kotlin：字符串模板
来源：http://qz.szxytkj.cn

"值: $b"
来源：http://bs.colortex.cn

[T04] Kotlin：空安全
来源：http://ng.yuexingan06.cn

val n: String? = null;  n?.length
来源：http://tx.shxzukj.cn

[T05] Kotlin：when 表达式
来源：http://uu.chemitech.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dg.bjjhwx.cn

[T06] Kotlin：集合映射
来源：http://pu.9csxet.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://sy.colortex.cn

[T07] Kotlin：集合过滤
来源：http://rh.chemitech.net.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fy.jctech888.com.cn

[T08] Kotlin：数据类
来源：http://ea.haigaiapp.cn

data class User(val name: String, val age: Int)
来源：http://lk.newstarts.cn

[T09] Kotlin：扩展函数
来源：http://zb.gzmigu.cn

fun String.exclaim() = this + "!"
来源：http://vr.huixiangedu.cn

[T10] Kotlin：默认参数
来源：http://cc.huixiangedu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gb.shxzskj.cn

[T11] Kotlin：协程
来源：http://xw.jctech888.com.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bd.newstarts.cn

[T12] Kotlin：解构声明
来源：http://hp.szsharing.cn

val (a, b) = Pair(1, 2)
来源：http://pa.hnjuh.cn

[T13] Kotlin：只读 Map
来源：http://hp.shxzskj.cn

val m = mapOf("a" to 1)
来源：http://rq.newstarts.cn

[T14] Kotlin：循环
来源：http://px.muxihuayi.cn

for (i in 1..10) println(i)
来源：http://ts.panjiajie.cn

[T15] Kotlin：接口
来源：http://nd.szsharing.cn

interface Shape { fun area(): Double }
来源：http://ck.jianghongdianzi.cn

[T16] Swift：Hello World
来源：http://ha.lnxyls.cn

print("Hello")
来源：http://dk.szxytkj.cn

[T17] Swift：变量与常量
来源：http://ap.shxzskj.cn

var a = 1;  let b = 2
来源：http://ue.jctech888.com.cn

[T18] Swift：字符串插值
来源：http://zo.muxihuayi.cn

"值: \(b)"
来源：http://pl.szsharing.cn

[T19] Swift：可选绑定
来源：http://bj.shxzukj.cn

if let n = opt { print(n) }
来源：http://qs.nszjky.cn

[T20] Swift：数组操作
来源：http://fq.bjjhwx.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fk.chemitech.net.cn

[T21] Swift：遍历
来源：http://rt.chemitech.net.cn

for x in a { print(x) }
来源：http://th.szsharing.cn

[T22] Swift：字典
来源：http://jg.panjiajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://kt.newstarts.cn

[T23] Swift：函数
来源：http://si.shtwfgs.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lh.yuntaijiaju.cn

[T24] Swift：闭包
来源：http://jt.huixiangedu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://me.asd995.cn

[T25] Swift：结构体
来源：http://xd.shxzskj.cn

struct P { var x: Int }
来源：http://ys.jianghongdianzi.cn

[T26] Swift：类与重写
来源：http://ax.chemitech.net.cn

class A: Base { override func f() {} }
来源：http://hr.bookmarksfly.cn

[T27] Swift：错误处理
来源：http://jb.shxzskj.cn

do { try f() } catch { print(error) }
来源：http://yl.muxihuayi.cn

[T28] Swift：枚举
来源：http://zf.shxzukj.cn

enum Color { case red, green }
来源：http://gt.huixinmuqiang.cn

[T29] Swift：guard 提前返回
来源：http://nw.shxzukj.cn

guard let x = opt else { return }
来源：http://le.shxzskj.cn

[T30] Swift：协议
来源：http://cl.shxzukj.cn

protocol Shape { func area() -> Double }
来源：http://il.shxzskj.cn

[T31] Lua：Hello World
来源：http://le.szxytkj.cn

print("Hello")
来源：http://nw.shxzukj.cn

[T32] Lua：局部变量
来源：http://gg.szxytkj.cn

local a = 1
来源：http://bz.szxytkj.cn

[T33] Lua：表（数组）
来源：http://pp.szxytkj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://rf.muxihuayi.cn

[T34] Lua：遍历表
来源：http://om.szxytkj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ik.nszjky.cn

[T35] Lua：字典表
来源：http://nh.shxzskj.cn

local d = { a = 1 };  d.b = 2
来源：http://cx.szsharing.cn

[T36] Lua：函数
来源：http://al.huixinmuqiang.cn

function add(a, b) return a + b end
来源：http://bb.nicolike.cn

[T37] Lua：字符串拼接
来源：http://uz.shtwfgs.cn

"a" .. "b"
来源：http://zw.shtwfgs.cn

[T38] Lua：条件
来源：http://pi.wgjwhj.cn

if x > 0 then print("正") end
来源：http://lj.muxihuayi.cn

[T39] Lua：模式匹配
来源：http://ys.hnjuh.cn

string.find(s, "%d+")
来源：http://ha.bjjhwx.cn

[T40] Lua：元表
来源：http://ph.haigaiapp.cn

setmetatable({}, { __index = base })
来源：http://cu.yuntaijiaju.cn

[T41] Perl：Hello World
来源：http://zj.9csxet.cn

print "Hello\n";
来源：http://ij.lnxyls.cn

[T42] Perl：变量类型
来源：http://fn.bjjhwx.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xt.huixinmuqiang.cn

[T43] Perl：字符串插值
来源：http://gd.jianghongdianzi.cn

"值: $a"
来源：http://tp.wgjwhj.cn

[T44] Perl：条件
来源：http://nq.yuntaijiaju.cn

if ($a > 0) { print "正"; }
来源：http://dl.huanxung.cn

[T45] Perl：数组遍历
来源：http://bo.newstarts.cn

for my $x (@arr) { print $x; }
来源：http://sr.521024.cn

[T46] Perl：哈希操作
来源：http://ua.gzmigu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ac.shxzukj.cn

[T47] Perl：正则捕获
来源：http://dz.jctech888.com.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://om.szxytkj.cn

[T48] Perl：正则替换
来源：http://mn.jianghongdianzi.cn

$s =~ s/old/new/g;
来源：http://dr.muxihuayi.cn

[T49] Perl：函数
来源：http://yb.huixinmuqiang.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qg.bjjhwx.cn

[T50] Perl：逐行读文件
来源：http://fw.shxzskj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://jy.colortex.cn

while (my $line = <$fh>) { print $line; }
来源：http://wb.jianghongdianzi.cn

[T51] Scala：Hello World
来源：http://ew.huixiangedu.cn

println("Hello")
来源：http://ha.wgjwhj.cn

[T52] Scala：变量
来源：http://wu.newstarts.cn

val a = 1;  var b = 2
来源：http://cd.hahajie.cn

[T53] Scala：字符串插值
来源：http://aq.521024.cn

s"值: $b"
来源：http://ro.shxzukj.cn

[T54] Scala：集合映射
来源：http://re.muxihuayi.cn

List(1, 2, 3).map(_ * 2)
来源：http://ma.huanxung.cn

[T55] Scala：集合过滤
来源：http://yb.huixinmuqiang.cn

List(1, 2, 3).filter(_ > 1)
来源：http://jh.bookmarksfly.cn

[T56] Scala：样例类
来源：http://cy.jianghongdianzi.cn

case class User(name: String, age: Int)
来源：http://sv.hahajie.cn

[T57] Scala：模式匹配
来源：http://bw.shxzskj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://rb.shtwfgs.cn

[T58] Scala：函数定义
来源：http://js.asd995.cn

def add(a: Int, b: Int): Int = a + b
来源：http://uy.shxzskj.cn

[T59] Scala：循环
来源：http://ko.huanxung.cn

for (i <- 1 to 10) println(i)
来源：http://xu.szsharing.cn

[T60] Scala：折叠
来源：http://ny.shxzskj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qu.shxzskj.cn

================================================================================
来源：http://bs.jianghongdianzi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://st.gzmigu.cn

================================================================================
来源：http://hb.newstarts.cn

[U01] Py：创建虚拟环境
来源：http://aq.gzmigu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://yz.521024.cn

[U02] Py：导出 / 安装依赖
来源：http://wy.muxihuayi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ar.gzmigu.cn

[U03] Py：加载 .env 配置
来源：http://nq.colortex.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ug.lnxyls.cn

[U04] Py：变量调试打印
来源：http://ip.gzmigu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ep.9csxet.cn

[U05] Py：列表去重且保序
来源：http://gu.szxytkj.cn

list(dict.fromkeys(arr))
来源：http://jz.521024.cn

[U06] Py：合并两个字典
来源：http://zi.huixiangedu.cn

{**a, **b}
来源：http://pl.shtwfgs.cn

[U07] Py：反转字典键值
来源：http://wu.hnjuh.cn

{v: k for k, v in d.items()}
来源：http://mn.huixinmuqiang.cn

[U08] Py：展平二维列表
来源：http://hj.asd995.cn

[y for x in nested for y in x]
来源：http://wr.newstarts.cn

[U09] Py：字典取最大值的键
来源：http://ui.szxytkj.cn

max(d, key=d.get)
来源：http://tz.hahajie.cn

[U10] Py：按值排序字典
来源：http://tj.huixiangedu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qo.shxzskj.cn

[U11] Py：生成器表达式
来源：http://rd.521024.cn

(x * 2 for x in arr)
来源：http://dl.wgjwhj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://df.panjiajie.cn

Counter(arr).most_common(3)
来源：http://ha.newstarts.cn

[U13] Py：固定长度队列
来源：http://nk.521024.cn

deque(maxlen=10)
来源：http://cy.huanxung.cn

[U14] Py：分组收集到列表
来源：http://vo.jianghongdianzi.cn

defaultdict(list)
来源：http://be.yuexingan06.cn

[U15] Py：高精度计时
来源：http://xe.nszjky.cn

t = time.perf_counter()
来源：http://uw.lnxyls.cn

[U16] Py：命令行参数解析
来源：http://gu.yuexingan06.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vw.jianghongdianzi.cn

[U17] Py：初始化日志
来源：http://fx.gzmigu.cn

logging.basicConfig(level=logging.INFO)
来源：http://fe.szxytkj.cn

[U18] Py：预编译正则
来源：http://hy.haigaiapp.cn

pat = re.compile(r"\d+")
来源：http://ud.jianghongdianzi.cn

[U19] Py：正则替换带回调
来源：http://kf.huixinmuqiang.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dj.bookmarksfly.cn

[U20] Py：缓存函数结果
来源：http://mv.asd995.cn

@functools.lru_cache(maxsize=None)
来源：http://je.wgjwhj.cn

[U21] Py：自定义上下文管理器
来源：http://kv.jctech888.com.cn

@contextlib.contextmanager
来源：http://lp.hahajie.cn

[U22] Py：矩阵转置
来源：http://oa.panjiajie.cn

list(zip(*m))
来源：http://nk.hnjuh.cn

[U23] Py：分块读取大文件
来源：http://gm.gzmigu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pi.szxytkj.cn

[U24] Py：路径操作
来源：http://uu.nicolike.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ia.panjiajie.cn

[U25] Py：CSV 按字典读
来源：http://ew.huanxung.cn

csv.DictReader(f)
来源：http://dm.muxihuayi.cn

[U26] Py：并发下载
来源：http://av.muxihuayi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wl.shtwfgs.cn

[U27] Py：异步 HTTP
来源：http://dl.hahajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://zq.szxytkj.cn

[U28] Py：类型别名
来源：http://vq.nszjky.cn

UserId = int
来源：http://eb.bookmarksfly.cn

[U29] Py：属性校验
来源：http://xb.hnjuh.cn

@property 与 @x.setter 配合
来源：http://kb.nszjky.cn

[U30] Py：数据类
来源：http://mt.shtwfgs.cn

@dataclass(slots=True)
来源：http://om.gzmigu.cn

[U31] Py：单测
来源：http://qp.hahajie.cn

python -m pytest -q
来源：http://jy.wgjwhj.cn

[U32] Py：代码格式化
来源：http://qi.gzmigu.cn

ruff format . && ruff check --fix .
来源：http://dj.colortex.cn


<!-- 参考信息 -->