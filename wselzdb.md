代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://wd.chemitech.net.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://lf.bookmarksfly.cn

fclose(f);
来源：http://qk.9csxet.cn

[S12] C：写文件
来源：http://uf.nszjky.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kr.haigaiapp.cn

[S13] C：宏定义
来源：http://jg.bjjhwx.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pt.panjiajie.cn

[S14] C：枚举
来源：http://pu.haigaiapp.cn

enum Color { RED, GREEN, BLUE };
来源：http://cl.jianghongdianzi.cn

[S15] C：类型转换
来源：http://uc.9csxet.cn

(double) a / b
来源：http://zr.hnjuh.cn

[S16] C：位操作置位
来源：http://yf.jctech888.com.cn

x |= (1 << 3);
来源：http://jy.haigaiapp.cn

[S17] C：安全拼接字符串
来源：http://lt.jctech888.com.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ea.szsharing.cn

[S18] C：命令行参数
来源：http://jl.huixiangedu.cn

int main(int argc, char **argv)
来源：http://aw.jianghongdianzi.cn

[S19] C：快速排序
来源：http://jn.yuexingan06.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vo.gzmigu.cn

[S20] C：二分查找
来源：http://kp.bjjhwx.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://af.shxzskj.cn

[S21] C：字符类别判断
来源：http://hw.shxzskj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mf.nszjky.cn

[S22] C：字符串转数字
来源：http://jf.szsharing.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rr.yuexingan06.cn

[S23] C：随机数
来源：http://nu.jianghongdianzi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cy.huanxung.cn

[S24] C：获取本地时间
来源：http://bn.shxzukj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vs.asd995.cn

[S25] C：内存拷贝
来源：http://za.panjiajie.cn

memcpy(dst, src, n);
来源：http://jy.huixinmuqiang.cn

[S26] C：内存清零
来源：http://zv.bookmarksfly.cn

memset(a, 0, sizeof a);
来源：http://me.huanxung.cn

[S27] C：定义常量
来源：http://zf.wgjwhj.cn

const double PI = 3.14159;
来源：http://yp.nszjky.cn

[S28] C：静态变量
来源：http://db.shxzukj.cn

static int counter = 0;
来源：http://ux.chemitech.net.cn

[S29] C：变参函数
来源：http://qf.wgjwhj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fm.shtwfgs.cn

[S30] C：头文件保护
来源：http://ga.shxzukj.cn

#ifndef X_H
来源：http://mb.shxzukj.cn

#define X_H
来源：http://yu.huixiangedu.cn

#endif
来源：http://ih.wgjwhj.cn

[S31] C++：Hello World
来源：http://aa.bjjhwx.cn

#include <iostream>
来源：http://ie.yuexingan06.cn

int main() { std::cout << "Hello\n"; }
来源：http://ck.shtwfgs.cn

[S32] C++：字符串
来源：http://pg.hnjuh.cn

std::string s = "hi";  s += "!";
来源：http://jz.chemitech.net.cn

[S33] C++：vector 增删
来源：http://xh.lnxyls.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ae.colortex.cn

[S34] C++：遍历 vector
来源：http://vk.muxihuayi.cn

for (auto &x : v) { std::cout << x; }
来源：http://mr.shxzskj.cn

[S35] C++：map
来源：http://xs.gzmigu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xa.yuexingan06.cn

[S36] C++：unordered_map
来源：http://rr.haigaiapp.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pa.huanxung.cn

[S37] C++：set
来源：http://ys.szsharing.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lv.shxzskj.cn

[S38] C++：排序
来源：http://zo.hnjuh.cn

std::sort(v.begin(), v.end());
来源：http://jz.yuexingan06.cn

[S39] C++：自定义比较器排序
来源：http://pv.nszjky.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vp.shtwfgs.cn

[S40] C++：查找元素
来源：http://vu.hahajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://og.gzmigu.cn

[S41] C++：类与构造函数
来源：http://ng.asd995.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tg.jianghongdianzi.cn

[S42] C++：继承与虚函数
来源：http://yp.huixiangedu.cn

class B : public Base { public: void f() override {} };
来源：http://pr.bjjhwx.cn

[S43] C++：智能指针
来源：http://hq.hahajie.cn

auto p = std::make_unique<int>(5);
来源：http://qv.nicolike.cn

[S44] C++：引用传参
来源：http://nh.huixiangedu.cn

void inc(int &x) { ++x; }
来源：http://om.asd995.cn

[S45] C++：lambda
来源：http://bs.jctech888.com.cn

auto add = [](int a, int b) { return a + b; };
来源：http://us.newstarts.cn

[S46] C++：函数模板
来源：http://lw.asd995.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://np.muxihuayi.cn

[S47] C++：结构化绑定遍历
来源：http://zx.hnjuh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://og.hahajie.cn

[S48] C++：逐行读文件
来源：http://vh.wgjwhj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ty.jianghongdianzi.cn

while (std::getline(in, line)) { }
来源：http://ah.muxihuayi.cn

[S49] C++：写文件
来源：http://lb.9csxet.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mr.bjjhwx.cn

[S50] C++：格式化数字
来源：http://ju.panjiajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://de.yuntaijiaju.cn

[S51] C++：显式类型转换
来源：http://vl.huixinmuqiang.cn

static_cast<double>(a) / b
来源：http://xs.jctech888.com.cn

[S52] C++：const 与 noexcept
来源：http://hc.jctech888.com.cn

int size() const noexcept { return n_; }
来源：http://ew.nicolike.cn

[S53] C++：移动语义
来源：http://wl.9csxet.cn

std::vector<int> w = std::move(v);
来源：http://jb.nszjky.cn

[S54] C++：异常处理
来源：http://pw.panjiajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ab.jctech888.com.cn

[S55] C++：结构化绑定
来源：http://tf.wgjwhj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rl.muxihuayi.cn

[S56] C++：optional
来源：http://wa.nicolike.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rk.huanxung.cn

[S57] C++：编译期常量
来源：http://en.chemitech.net.cn

constexpr int N = 10;
来源：http://yb.nicolike.cn

[S58] C++：命名空间
来源：http://og.muxihuayi.cn

namespace ns { int f() { return 1; } }
来源：http://ot.nicolike.cn

[S59] C++：静态断言
来源：http://ek.yuexingan06.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ua.shxzskj.cn

[S60] C++：遍历并删除元素
来源：http://ep.muxihuayi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hs.huixinmuqiang.cn

================================================================================
来源：http://qx.521024.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://un.hnjuh.cn

================================================================================
来源：http://lq.jianghongdianzi.cn

[T01] Kotlin：Hello World
来源：http://uw.shtwfgs.cn

println("Hello")
来源：http://gb.shtwfgs.cn

[T02] Kotlin：变量
来源：http://kn.hnjuh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jl.shxzukj.cn

[T03] Kotlin：字符串模板
来源：http://cz.jctech888.com.cn

"值: $b"
来源：http://pm.szsharing.cn

[T04] Kotlin：空安全
来源：http://of.huanxung.cn

val n: String? = null;  n?.length
来源：http://sr.lnxyls.cn

[T05] Kotlin：when 表达式
来源：http://tk.szxytkj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rf.wgjwhj.cn

[T06] Kotlin：集合映射
来源：http://ek.bjjhwx.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ep.szxytkj.cn

[T07] Kotlin：集合过滤
来源：http://gh.bookmarksfly.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vs.yuexingan06.cn

[T08] Kotlin：数据类
来源：http://rc.colortex.cn

data class User(val name: String, val age: Int)
来源：http://rf.jctech888.com.cn

[T09] Kotlin：扩展函数
来源：http://js.shxzskj.cn

fun String.exclaim() = this + "!"
来源：http://mo.bjjhwx.cn

[T10] Kotlin：默认参数
来源：http://gw.szsharing.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vc.hahajie.cn

[T11] Kotlin：协程
来源：http://ql.muxihuayi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://cf.hnjuh.cn

[T12] Kotlin：解构声明
来源：http://ru.huanxung.cn

val (a, b) = Pair(1, 2)
来源：http://sd.huixinmuqiang.cn

[T13] Kotlin：只读 Map
来源：http://ez.yuntaijiaju.cn

val m = mapOf("a" to 1)
来源：http://ha.muxihuayi.cn

[T14] Kotlin：循环
来源：http://bs.wgjwhj.cn

for (i in 1..10) println(i)
来源：http://tq.haigaiapp.cn

[T15] Kotlin：接口
来源：http://er.szsharing.cn

interface Shape { fun area(): Double }
来源：http://mf.hnjuh.cn

[T16] Swift：Hello World
来源：http://zu.newstarts.cn

print("Hello")
来源：http://iw.haigaiapp.cn

[T17] Swift：变量与常量
来源：http://rs.colortex.cn

var a = 1;  let b = 2
来源：http://ed.muxihuayi.cn

[T18] Swift：字符串插值
来源：http://wv.huixinmuqiang.cn

"值: \(b)"
来源：http://aw.hnjuh.cn

[T19] Swift：可选绑定
来源：http://js.gzmigu.cn

if let n = opt { print(n) }
来源：http://qe.lnxyls.cn

[T20] Swift：数组操作
来源：http://is.bjjhwx.cn

var a = [1, 2, 3];  a.append(4)
来源：http://sl.huixinmuqiang.cn

[T21] Swift：遍历
来源：http://op.9csxet.cn

for x in a { print(x) }
来源：http://ni.newstarts.cn

[T22] Swift：字典
来源：http://ht.lnxyls.cn

var d = ["a": 1];  d["b"] = 2
来源：http://sg.bookmarksfly.cn

[T23] Swift：函数
来源：http://zf.szsharing.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dv.muxihuayi.cn

[T24] Swift：闭包
来源：http://ly.jctech888.com.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://hl.szxytkj.cn

[T25] Swift：结构体
来源：http://ed.colortex.cn

struct P { var x: Int }
来源：http://rq.huanxung.cn

[T26] Swift：类与重写
来源：http://nh.muxihuayi.cn

class A: Base { override func f() {} }
来源：http://oy.yuntaijiaju.cn

[T27] Swift：错误处理
来源：http://tr.nszjky.cn

do { try f() } catch { print(error) }
来源：http://gg.shtwfgs.cn

[T28] Swift：枚举
来源：http://kv.jctech888.com.cn

enum Color { case red, green }
来源：http://kr.haigaiapp.cn

[T29] Swift：guard 提前返回
来源：http://ye.gzmigu.cn

guard let x = opt else { return }
来源：http://qy.jianghongdianzi.cn

[T30] Swift：协议
来源：http://et.chemitech.net.cn

protocol Shape { func area() -> Double }
来源：http://po.gzmigu.cn

[T31] Lua：Hello World
来源：http://iy.asd995.cn

print("Hello")
来源：http://ql.bjjhwx.cn

[T32] Lua：局部变量
来源：http://pd.yuntaijiaju.cn

local a = 1
来源：http://ze.newstarts.cn

[T33] Lua：表（数组）
来源：http://sy.haigaiapp.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://lj.panjiajie.cn

[T34] Lua：遍历表
来源：http://jr.yuntaijiaju.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://xk.szxytkj.cn

[T35] Lua：字典表
来源：http://gh.shtwfgs.cn

local d = { a = 1 };  d.b = 2
来源：http://yo.nszjky.cn

[T36] Lua：函数
来源：http://pi.hahajie.cn

function add(a, b) return a + b end
来源：http://ne.huixiangedu.cn

[T37] Lua：字符串拼接
来源：http://lx.huixinmuqiang.cn

"a" .. "b"
来源：http://ul.asd995.cn

[T38] Lua：条件
来源：http://qu.hnjuh.cn

if x > 0 then print("正") end
来源：http://ns.shxzskj.cn

[T39] Lua：模式匹配
来源：http://ad.szxytkj.cn

string.find(s, "%d+")
来源：http://iq.9csxet.cn

[T40] Lua：元表
来源：http://gb.haigaiapp.cn

setmetatable({}, { __index = base })
来源：http://zu.huixinmuqiang.cn

[T41] Perl：Hello World
来源：http://bj.bookmarksfly.cn

print "Hello\n";
来源：http://nt.muxihuayi.cn

[T42] Perl：变量类型
来源：http://qd.newstarts.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kh.muxihuayi.cn

[T43] Perl：字符串插值
来源：http://vw.szsharing.cn

"值: $a"
来源：http://xo.yuexingan06.cn

[T44] Perl：条件
来源：http://qd.asd995.cn

if ($a > 0) { print "正"; }
来源：http://ta.bookmarksfly.cn

[T45] Perl：数组遍历
来源：http://to.szxytkj.cn

for my $x (@arr) { print $x; }
来源：http://gl.hahajie.cn

[T46] Perl：哈希操作
来源：http://br.shtwfgs.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xa.nicolike.cn

[T47] Perl：正则捕获
来源：http://ip.yuexingan06.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://yn.szsharing.cn

[T48] Perl：正则替换
来源：http://kc.szxytkj.cn

$s =~ s/old/new/g;
来源：http://zj.chemitech.net.cn

[T49] Perl：函数
来源：http://is.521024.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mk.colortex.cn

[T50] Perl：逐行读文件
来源：http://ka.jianghongdianzi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://bv.bjjhwx.cn

while (my $line = <$fh>) { print $line; }
来源：http://ms.huixiangedu.cn

[T51] Scala：Hello World
来源：http://yt.yuntaijiaju.cn

println("Hello")
来源：http://it.muxihuayi.cn

[T52] Scala：变量
来源：http://mj.521024.cn

val a = 1;  var b = 2
来源：http://sn.nicolike.cn

[T53] Scala：字符串插值
来源：http://ql.bookmarksfly.cn

s"值: $b"
来源：http://md.panjiajie.cn

[T54] Scala：集合映射
来源：http://th.huixinmuqiang.cn

List(1, 2, 3).map(_ * 2)
来源：http://ae.yuexingan06.cn

[T55] Scala：集合过滤
来源：http://jr.521024.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fb.yuexingan06.cn

[T56] Scala：样例类
来源：http://tk.huixinmuqiang.cn

case class User(name: String, age: Int)
来源：http://kj.hahajie.cn

[T57] Scala：模式匹配
来源：http://wz.bookmarksfly.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://xr.bjjhwx.cn

[T58] Scala：函数定义
来源：http://pc.colortex.cn

def add(a: Int, b: Int): Int = a + b
来源：http://st.shxzukj.cn

[T59] Scala：循环
来源：http://fp.szsharing.cn

for (i <- 1 to 10) println(i)
来源：http://go.shxzskj.cn

[T60] Scala：折叠
来源：http://ga.shxzukj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ob.521024.cn

================================================================================
来源：http://wi.wgjwhj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://so.huanxung.cn

================================================================================
来源：http://ac.bookmarksfly.cn

[U01] Py：创建虚拟环境
来源：http://kb.nicolike.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mt.newstarts.cn

[U02] Py：导出 / 安装依赖
来源：http://zd.huanxung.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ux.huixinmuqiang.cn

[U03] Py：加载 .env 配置
来源：http://sj.huanxung.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wa.szsharing.cn

[U04] Py：变量调试打印
来源：http://ug.szsharing.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://su.asd995.cn

[U05] Py：列表去重且保序
来源：http://ui.bjjhwx.cn

list(dict.fromkeys(arr))
来源：http://xq.panjiajie.cn

[U06] Py：合并两个字典
来源：http://bn.gzmigu.cn

{**a, **b}
来源：http://mk.521024.cn

[U07] Py：反转字典键值
来源：http://ky.huanxung.cn

{v: k for k, v in d.items()}
来源：http://cs.newstarts.cn

[U08] Py：展平二维列表
来源：http://gb.nszjky.cn

[y for x in nested for y in x]
来源：http://gt.gzmigu.cn

[U09] Py：字典取最大值的键
来源：http://jt.bookmarksfly.cn

max(d, key=d.get)
来源：http://ir.shtwfgs.cn

[U10] Py：按值排序字典
来源：http://dl.haigaiapp.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bl.muxihuayi.cn

[U11] Py：生成器表达式
来源：http://yr.lnxyls.cn

(x * 2 for x in arr)
来源：http://gm.shxzukj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://se.lnxyls.cn

Counter(arr).most_common(3)
来源：http://xr.lnxyls.cn

[U13] Py：固定长度队列
来源：http://kn.haigaiapp.cn

deque(maxlen=10)
来源：http://pb.panjiajie.cn

[U14] Py：分组收集到列表
来源：http://gs.huixiangedu.cn

defaultdict(list)
来源：http://oe.nszjky.cn

[U15] Py：高精度计时
来源：http://wg.asd995.cn

t = time.perf_counter()
来源：http://uu.bjjhwx.cn

[U16] Py：命令行参数解析
来源：http://tk.haigaiapp.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ry.gzmigu.cn

[U17] Py：初始化日志
来源：http://nl.wgjwhj.cn

logging.basicConfig(level=logging.INFO)
来源：http://cv.gzmigu.cn

[U18] Py：预编译正则
来源：http://xt.huixiangedu.cn

pat = re.compile(r"\d+")
来源：http://rr.jianghongdianzi.cn

[U19] Py：正则替换带回调
来源：http://bp.lnxyls.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://id.muxihuayi.cn

[U20] Py：缓存函数结果
来源：http://pn.yuntaijiaju.cn

@functools.lru_cache(maxsize=None)
来源：http://io.bookmarksfly.cn

[U21] Py：自定义上下文管理器
来源：http://tm.haigaiapp.cn

@contextlib.contextmanager
来源：http://co.jianghongdianzi.cn

[U22] Py：矩阵转置
来源：http://rc.shxzukj.cn

list(zip(*m))
来源：http://jb.shtwfgs.cn

[U23] Py：分块读取大文件
来源：http://in.huanxung.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jz.haigaiapp.cn

[U24] Py：路径操作
来源：http://yy.hahajie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nz.wgjwhj.cn

[U25] Py：CSV 按字典读
来源：http://el.shxzskj.cn

csv.DictReader(f)
来源：http://gq.shxzukj.cn

[U26] Py：并发下载
来源：http://gm.shxzukj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rc.shxzukj.cn

[U27] Py：异步 HTTP
来源：http://ml.szxytkj.cn

aiohttp.ClientSession() 配合 async with
来源：http://sk.lnxyls.cn

[U28] Py：类型别名
来源：http://dy.huanxung.cn

UserId = int
来源：http://so.nszjky.cn

[U29] Py：属性校验
来源：http://yd.haigaiapp.cn

@property 与 @x.setter 配合
来源：http://dh.521024.cn

[U30] Py：数据类
来源：http://kv.shxzukj.cn

@dataclass(slots=True)
来源：http://sa.asd995.cn

[U31] Py：单测
来源：http://uy.jianghongdianzi.cn

python -m pytest -q
来源：http://eu.colortex.cn

[U32] Py：代码格式化
来源：http://lk.lnxyls.cn

ruff format . && ruff check --fix .
来源：http://pp.chemitech.net.cn

[U33] Py：打包发布
来源：http://tc.panjiajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://so.huanxung.cn

[U34] Py：判断编码
来源：http://wc.lnxyls.cn

chardet.detect(raw)
来源：http://uf.chemitech.net.cn


<!-- 参考信息 -->