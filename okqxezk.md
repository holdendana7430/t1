代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sz.huixiangedu.cn

[S13] C：宏定义
来源：http://mg.newstarts.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rp.szxytkj.cn

[S14] C：枚举
来源：http://ir.asd995.cn

enum Color { RED, GREEN, BLUE };
来源：http://tl.shxzukj.cn

[S15] C：类型转换
来源：http://xr.nicolike.cn

(double) a / b
来源：http://ms.yuexingan06.cn

[S16] C：位操作置位
来源：http://sh.szsharing.cn

x |= (1 << 3);
来源：http://di.bjjhwx.cn

[S17] C：安全拼接字符串
来源：http://du.colortex.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wl.shtwfgs.cn

[S18] C：命令行参数
来源：http://ai.newstarts.cn

int main(int argc, char **argv)
来源：http://ku.shtwfgs.cn

[S19] C：快速排序
来源：http://kr.bookmarksfly.cn

qsort(a, n, sizeof(int), cmp);
来源：http://go.huixiangedu.cn

[S20] C：二分查找
来源：http://al.haigaiapp.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://de.panjiajie.cn

[S21] C：字符类别判断
来源：http://xt.wgjwhj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://du.jianghongdianzi.cn

[S22] C：字符串转数字
来源：http://uj.9csxet.cn

atoi("42");  strtod("3.14", NULL);
来源：http://yn.gzmigu.cn

[S23] C：随机数
来源：http://cb.szsharing.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://lg.nicolike.cn

[S24] C：获取本地时间
来源：http://qj.lnxyls.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wx.szxytkj.cn

[S25] C：内存拷贝
来源：http://pk.bjjhwx.cn

memcpy(dst, src, n);
来源：http://gr.colortex.cn

[S26] C：内存清零
来源：http://oz.szxytkj.cn

memset(a, 0, sizeof a);
来源：http://wv.jctech888.com.cn

[S27] C：定义常量
来源：http://xi.muxihuayi.cn

const double PI = 3.14159;
来源：http://ax.asd995.cn

[S28] C：静态变量
来源：http://ud.szsharing.cn

static int counter = 0;
来源：http://ou.huixiangedu.cn

[S29] C：变参函数
来源：http://ni.huixiangedu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jj.lnxyls.cn

[S30] C：头文件保护
来源：http://pi.huixiangedu.cn

#ifndef X_H
来源：http://eq.521024.cn

#define X_H
来源：http://ow.huixinmuqiang.cn

#endif
来源：http://do.lnxyls.cn

[S31] C++：Hello World
来源：http://qs.yuexingan06.cn

#include <iostream>
来源：http://oc.hahajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://tq.yuntaijiaju.cn

[S32] C++：字符串
来源：http://um.szsharing.cn

std::string s = "hi";  s += "!";
来源：http://cz.wgjwhj.cn

[S33] C++：vector 增删
来源：http://zc.chemitech.net.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mv.panjiajie.cn

[S34] C++：遍历 vector
来源：http://ue.nicolike.cn

for (auto &x : v) { std::cout << x; }
来源：http://yf.huanxung.cn

[S35] C++：map
来源：http://vk.jianghongdianzi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tm.shxzukj.cn

[S36] C++：unordered_map
来源：http://rq.yuexingan06.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qt.panjiajie.cn

[S37] C++：set
来源：http://bn.gzmigu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sk.bookmarksfly.cn

[S38] C++：排序
来源：http://jt.szsharing.cn

std::sort(v.begin(), v.end());
来源：http://tt.jianghongdianzi.cn

[S39] C++：自定义比较器排序
来源：http://tb.shxzukj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qp.jctech888.com.cn

[S40] C++：查找元素
来源：http://bf.asd995.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://as.9csxet.cn

[S41] C++：类与构造函数
来源：http://vt.shxzukj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ba.panjiajie.cn

[S42] C++：继承与虚函数
来源：http://zc.jianghongdianzi.cn

class B : public Base { public: void f() override {} };
来源：http://hs.shxzskj.cn

[S43] C++：智能指针
来源：http://hu.szsharing.cn

auto p = std::make_unique<int>(5);
来源：http://wl.muxihuayi.cn

[S44] C++：引用传参
来源：http://jq.bookmarksfly.cn

void inc(int &x) { ++x; }
来源：http://ag.wgjwhj.cn

[S45] C++：lambda
来源：http://ew.bjjhwx.cn

auto add = [](int a, int b) { return a + b; };
来源：http://yp.wgjwhj.cn

[S46] C++：函数模板
来源：http://ra.lnxyls.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hn.lnxyls.cn

[S47] C++：结构化绑定遍历
来源：http://uh.shxzskj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wf.jianghongdianzi.cn

[S48] C++：逐行读文件
来源：http://mx.panjiajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xb.nszjky.cn

while (std::getline(in, line)) { }
来源：http://eh.wgjwhj.cn

[S49] C++：写文件
来源：http://ll.shxzukj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://eo.lnxyls.cn

[S50] C++：格式化数字
来源：http://yu.asd995.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://co.chemitech.net.cn

[S51] C++：显式类型转换
来源：http://ic.9csxet.cn

static_cast<double>(a) / b
来源：http://jw.huanxung.cn

[S52] C++：const 与 noexcept
来源：http://lv.asd995.cn

int size() const noexcept { return n_; }
来源：http://gi.haigaiapp.cn

[S53] C++：移动语义
来源：http://vs.hahajie.cn

std::vector<int> w = std::move(v);
来源：http://qy.yuntaijiaju.cn

[S54] C++：异常处理
来源：http://xq.shxzukj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://it.huixinmuqiang.cn

[S55] C++：结构化绑定
来源：http://dp.huixinmuqiang.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pr.chemitech.net.cn

[S56] C++：optional
来源：http://ud.panjiajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fz.asd995.cn

[S57] C++：编译期常量
来源：http://bc.jianghongdianzi.cn

constexpr int N = 10;
来源：http://vn.lnxyls.cn

[S58] C++：命名空间
来源：http://hl.gzmigu.cn

namespace ns { int f() { return 1; } }
来源：http://bu.521024.cn

[S59] C++：静态断言
来源：http://ln.huixiangedu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kf.panjiajie.cn

[S60] C++：遍历并删除元素
来源：http://lz.haigaiapp.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sv.newstarts.cn

================================================================================
来源：http://hd.bjjhwx.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uz.jctech888.com.cn

================================================================================
来源：http://vo.jctech888.com.cn

[T01] Kotlin：Hello World
来源：http://lv.lnxyls.cn

println("Hello")
来源：http://oe.shtwfgs.cn

[T02] Kotlin：变量
来源：http://df.colortex.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qc.huixiangedu.cn

[T03] Kotlin：字符串模板
来源：http://me.muxihuayi.cn

"值: $b"
来源：http://nc.huixiangedu.cn

[T04] Kotlin：空安全
来源：http://tv.chemitech.net.cn

val n: String? = null;  n?.length
来源：http://qt.asd995.cn

[T05] Kotlin：when 表达式
来源：http://fy.szsharing.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cb.yuntaijiaju.cn

[T06] Kotlin：集合映射
来源：http://ou.huixiangedu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://je.521024.cn

[T07] Kotlin：集合过滤
来源：http://ks.muxihuayi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fh.jianghongdianzi.cn

[T08] Kotlin：数据类
来源：http://rr.szsharing.cn

data class User(val name: String, val age: Int)
来源：http://cq.szxytkj.cn

[T09] Kotlin：扩展函数
来源：http://bp.wgjwhj.cn

fun String.exclaim() = this + "!"
来源：http://fe.hahajie.cn

[T10] Kotlin：默认参数
来源：http://rb.hahajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ur.yuntaijiaju.cn

[T11] Kotlin：协程
来源：http://ro.panjiajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://yk.chemitech.net.cn

[T12] Kotlin：解构声明
来源：http://ul.panjiajie.cn

val (a, b) = Pair(1, 2)
来源：http://kp.huanxung.cn

[T13] Kotlin：只读 Map
来源：http://bk.szxytkj.cn

val m = mapOf("a" to 1)
来源：http://cg.hnjuh.cn

[T14] Kotlin：循环
来源：http://sz.szxytkj.cn

for (i in 1..10) println(i)
来源：http://ox.bookmarksfly.cn

[T15] Kotlin：接口
来源：http://ut.huanxung.cn

interface Shape { fun area(): Double }
来源：http://gr.yuexingan06.cn

[T16] Swift：Hello World
来源：http://ew.newstarts.cn

print("Hello")
来源：http://yb.yuexingan06.cn

[T17] Swift：变量与常量
来源：http://by.szxytkj.cn

var a = 1;  let b = 2
来源：http://sr.jianghongdianzi.cn

[T18] Swift：字符串插值
来源：http://ga.shtwfgs.cn

"值: \(b)"
来源：http://qw.jianghongdianzi.cn

[T19] Swift：可选绑定
来源：http://cx.9csxet.cn

if let n = opt { print(n) }
来源：http://tl.shxzukj.cn

[T20] Swift：数组操作
来源：http://sb.wgjwhj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://tx.shxzskj.cn

[T21] Swift：遍历
来源：http://tj.shxzukj.cn

for x in a { print(x) }
来源：http://am.huixinmuqiang.cn

[T22] Swift：字典
来源：http://wo.huanxung.cn

var d = ["a": 1];  d["b"] = 2
来源：http://uw.hahajie.cn

[T23] Swift：函数
来源：http://up.yuexingan06.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://na.asd995.cn

[T24] Swift：闭包
来源：http://qy.yuntaijiaju.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://pq.yuexingan06.cn

[T25] Swift：结构体
来源：http://ei.huanxung.cn

struct P { var x: Int }
来源：http://mx.szsharing.cn

[T26] Swift：类与重写
来源：http://zy.lnxyls.cn

class A: Base { override func f() {} }
来源：http://vm.asd995.cn

[T27] Swift：错误处理
来源：http://tb.asd995.cn

do { try f() } catch { print(error) }
来源：http://qw.gzmigu.cn

[T28] Swift：枚举
来源：http://qz.colortex.cn

enum Color { case red, green }
来源：http://yl.asd995.cn

[T29] Swift：guard 提前返回
来源：http://pk.9csxet.cn

guard let x = opt else { return }
来源：http://im.huixiangedu.cn

[T30] Swift：协议
来源：http://fy.521024.cn

protocol Shape { func area() -> Double }
来源：http://qm.colortex.cn

[T31] Lua：Hello World
来源：http://nr.bjjhwx.cn

print("Hello")
来源：http://xx.wgjwhj.cn

[T32] Lua：局部变量
来源：http://ed.wgjwhj.cn

local a = 1
来源：http://tz.asd995.cn

[T33] Lua：表（数组）
来源：http://ov.hnjuh.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://cm.nszjky.cn

[T34] Lua：遍历表
来源：http://zx.lnxyls.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rw.haigaiapp.cn

[T35] Lua：字典表
来源：http://jn.muxihuayi.cn

local d = { a = 1 };  d.b = 2
来源：http://dz.huixiangedu.cn

[T36] Lua：函数
来源：http://qd.yuntaijiaju.cn

function add(a, b) return a + b end
来源：http://zi.szsharing.cn

[T37] Lua：字符串拼接
来源：http://xn.nszjky.cn

"a" .. "b"
来源：http://qr.jianghongdianzi.cn

[T38] Lua：条件
来源：http://su.jctech888.com.cn

if x > 0 then print("正") end
来源：http://xb.gzmigu.cn

[T39] Lua：模式匹配
来源：http://fq.newstarts.cn

string.find(s, "%d+")
来源：http://qm.yuexingan06.cn

[T40] Lua：元表
来源：http://mx.asd995.cn

setmetatable({}, { __index = base })
来源：http://nf.bjjhwx.cn

[T41] Perl：Hello World
来源：http://nd.jianghongdianzi.cn

print "Hello\n";
来源：http://bf.9csxet.cn

[T42] Perl：变量类型
来源：http://td.huixinmuqiang.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pv.wgjwhj.cn

[T43] Perl：字符串插值
来源：http://nd.bjjhwx.cn

"值: $a"
来源：http://fe.haigaiapp.cn

[T44] Perl：条件
来源：http://ub.nicolike.cn

if ($a > 0) { print "正"; }
来源：http://at.nicolike.cn

[T45] Perl：数组遍历
来源：http://kr.szxytkj.cn

for my $x (@arr) { print $x; }
来源：http://ba.bjjhwx.cn

[T46] Perl：哈希操作
来源：http://th.lnxyls.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bq.hahajie.cn

[T47] Perl：正则捕获
来源：http://gp.nszjky.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jd.521024.cn

[T48] Perl：正则替换
来源：http://ib.asd995.cn

$s =~ s/old/new/g;
来源：http://ye.521024.cn

[T49] Perl：函数
来源：http://lj.hahajie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ml.gzmigu.cn

[T50] Perl：逐行读文件
来源：http://cw.huanxung.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://lh.yuexingan06.cn

while (my $line = <$fh>) { print $line; }
来源：http://sr.shtwfgs.cn

[T51] Scala：Hello World
来源：http://bh.huixiangedu.cn

println("Hello")
来源：http://hy.shxzukj.cn

[T52] Scala：变量
来源：http://zf.gzmigu.cn

val a = 1;  var b = 2
来源：http://qm.huixiangedu.cn

[T53] Scala：字符串插值
来源：http://by.nicolike.cn

s"值: $b"
来源：http://wa.yuntaijiaju.cn

[T54] Scala：集合映射
来源：http://gf.jctech888.com.cn

List(1, 2, 3).map(_ * 2)
来源：http://sn.lnxyls.cn

[T55] Scala：集合过滤
来源：http://rh.gzmigu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://df.haigaiapp.cn

[T56] Scala：样例类
来源：http://ux.bjjhwx.cn

case class User(name: String, age: Int)
来源：http://qg.jianghongdianzi.cn

[T57] Scala：模式匹配
来源：http://mc.yuexingan06.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://jw.panjiajie.cn

[T58] Scala：函数定义
来源：http://kx.shxzskj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ac.9csxet.cn

[T59] Scala：循环
来源：http://yx.shxzskj.cn

for (i <- 1 to 10) println(i)
来源：http://fi.huixinmuqiang.cn

[T60] Scala：折叠
来源：http://io.panjiajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yk.bjjhwx.cn

================================================================================
来源：http://hq.huixiangedu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://it.shtwfgs.cn

================================================================================
来源：http://sx.lnxyls.cn

[U01] Py：创建虚拟环境
来源：http://sv.lnxyls.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mj.huixinmuqiang.cn

[U02] Py：导出 / 安装依赖
来源：http://qp.muxihuayi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ry.muxihuayi.cn

[U03] Py：加载 .env 配置
来源：http://ee.wgjwhj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xt.shxzukj.cn

[U04] Py：变量调试打印
来源：http://hv.haigaiapp.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ce.panjiajie.cn

[U05] Py：列表去重且保序
来源：http://mr.szsharing.cn

list(dict.fromkeys(arr))
来源：http://pg.lnxyls.cn

[U06] Py：合并两个字典
来源：http://vc.shxzukj.cn

{**a, **b}
来源：http://zp.521024.cn

[U07] Py：反转字典键值
来源：http://ba.jianghongdianzi.cn

{v: k for k, v in d.items()}
来源：http://ed.bookmarksfly.cn

[U08] Py：展平二维列表
来源：http://wm.shxzukj.cn

[y for x in nested for y in x]
来源：http://tl.jctech888.com.cn

[U09] Py：字典取最大值的键
来源：http://jr.nicolike.cn

max(d, key=d.get)
来源：http://ga.bookmarksfly.cn

[U10] Py：按值排序字典
来源：http://pv.jianghongdianzi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ua.nicolike.cn

[U11] Py：生成器表达式
来源：http://xj.bookmarksfly.cn

(x * 2 for x in arr)
来源：http://as.jianghongdianzi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://fa.jianghongdianzi.cn

Counter(arr).most_common(3)
来源：http://in.newstarts.cn

[U13] Py：固定长度队列
来源：http://yw.shtwfgs.cn

deque(maxlen=10)
来源：http://yt.panjiajie.cn

[U14] Py：分组收集到列表
来源：http://gg.newstarts.cn

defaultdict(list)
来源：http://zx.szxytkj.cn

[U15] Py：高精度计时
来源：http://cx.chemitech.net.cn

t = time.perf_counter()
来源：http://si.nicolike.cn

[U16] Py：命令行参数解析
来源：http://bm.9csxet.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fi.haigaiapp.cn

[U17] Py：初始化日志
来源：http://bt.shxzskj.cn

logging.basicConfig(level=logging.INFO)
来源：http://tk.jianghongdianzi.cn

[U18] Py：预编译正则
来源：http://jr.9csxet.cn

pat = re.compile(r"\d+")
来源：http://uu.hahajie.cn

[U19] Py：正则替换带回调
来源：http://cm.521024.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xa.newstarts.cn

[U20] Py：缓存函数结果
来源：http://zf.hahajie.cn

@functools.lru_cache(maxsize=None)
来源：http://oc.yuexingan06.cn

[U21] Py：自定义上下文管理器
来源：http://fr.szsharing.cn

@contextlib.contextmanager
来源：http://oc.huixinmuqiang.cn

[U22] Py：矩阵转置
来源：http://dh.shtwfgs.cn

list(zip(*m))
来源：http://mv.asd995.cn

[U23] Py：分块读取大文件
来源：http://gp.szxytkj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lx.yuntaijiaju.cn

[U24] Py：路径操作
来源：http://kh.yuntaijiaju.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qs.hnjuh.cn

[U25] Py：CSV 按字典读
来源：http://uo.panjiajie.cn

csv.DictReader(f)
来源：http://hi.shxzskj.cn

[U26] Py：并发下载
来源：http://yo.muxihuayi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://eb.newstarts.cn

[U27] Py：异步 HTTP
来源：http://db.jianghongdianzi.cn

aiohttp.ClientSession() 配合 async with
来源：http://io.huixinmuqiang.cn

[U28] Py：类型别名
来源：http://to.hahajie.cn

UserId = int
来源：http://ry.newstarts.cn

[U29] Py：属性校验
来源：http://jw.newstarts.cn

@property 与 @x.setter 配合
来源：http://ik.panjiajie.cn

[U30] Py：数据类
来源：http://at.yuntaijiaju.cn

@dataclass(slots=True)
来源：http://my.shxzukj.cn

[U31] Py：单测
来源：http://gq.bookmarksfly.cn

python -m pytest -q
来源：http://at.szsharing.cn

[U32] Py：代码格式化
来源：http://jo.yuntaijiaju.cn

ruff format . && ruff check --fix .
来源：http://gd.szsharing.cn

[U33] Py：打包发布
来源：http://vk.shxzskj.cn

python -m build  （依赖 pyproject.toml）
来源：http://zw.newstarts.cn

[U34] Py：判断编码
来源：http://fo.nicolike.cn

chardet.detect(raw)
来源：http://ym.yuexingan06.cn

[U35] Py：发送邮件
来源：http://kp.hahajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tr.hnjuh.cn

[U36] Py：定时任务
来源：http://tt.asd995.cn

schedule.every(10).minutes.do(job)
来源：http://el.szsharing.cn


<!-- 参考信息 -->