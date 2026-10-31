代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://tm.chemitech.net.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://uj.shxzskj.cn

fclose(f);
来源：http://ny.hahajie.cn

[S12] C：写文件
来源：http://yy.muxihuayi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ev.jctech888.com.cn

[S13] C：宏定义
来源：http://zf.hahajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dt.huixinmuqiang.cn

[S14] C：枚举
来源：http://ej.newstarts.cn

enum Color { RED, GREEN, BLUE };
来源：http://jl.nszjky.cn

[S15] C：类型转换
来源：http://ax.colortex.cn

(double) a / b
来源：http://yg.szsharing.cn

[S16] C：位操作置位
来源：http://vx.newstarts.cn

x |= (1 << 3);
来源：http://xn.jianghongdianzi.cn

[S17] C：安全拼接字符串
来源：http://ky.jianghongdianzi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ny.wgjwhj.cn

[S18] C：命令行参数
来源：http://uc.yuntaijiaju.cn

int main(int argc, char **argv)
来源：http://ah.521024.cn

[S19] C：快速排序
来源：http://ox.colortex.cn

qsort(a, n, sizeof(int), cmp);
来源：http://by.shtwfgs.cn

[S20] C：二分查找
来源：http://rp.9csxet.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pf.9csxet.cn

[S21] C：字符类别判断
来源：http://hx.colortex.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kb.nszjky.cn

[S22] C：字符串转数字
来源：http://bh.shxzukj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ep.szxytkj.cn

[S23] C：随机数
来源：http://of.szsharing.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bv.shtwfgs.cn

[S24] C：获取本地时间
来源：http://il.chemitech.net.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tx.bookmarksfly.cn

[S25] C：内存拷贝
来源：http://ep.shxzskj.cn

memcpy(dst, src, n);
来源：http://cq.asd995.cn

[S26] C：内存清零
来源：http://bw.nicolike.cn

memset(a, 0, sizeof a);
来源：http://qw.huixiangedu.cn

[S27] C：定义常量
来源：http://iy.szxytkj.cn

const double PI = 3.14159;
来源：http://ry.shtwfgs.cn

[S28] C：静态变量
来源：http://wp.asd995.cn

static int counter = 0;
来源：http://pd.lnxyls.cn

[S29] C：变参函数
来源：http://fn.szxytkj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qp.nszjky.cn

[S30] C：头文件保护
来源：http://fe.jianghongdianzi.cn

#ifndef X_H
来源：http://qw.szsharing.cn

#define X_H
来源：http://xu.lnxyls.cn

#endif
来源：http://cl.wgjwhj.cn

[S31] C++：Hello World
来源：http://qz.hahajie.cn

#include <iostream>
来源：http://vp.haigaiapp.cn

int main() { std::cout << "Hello\n"; }
来源：http://yp.shxzskj.cn

[S32] C++：字符串
来源：http://ci.jctech888.com.cn

std::string s = "hi";  s += "!";
来源：http://nc.szsharing.cn

[S33] C++：vector 增删
来源：http://am.muxihuayi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qx.asd995.cn

[S34] C++：遍历 vector
来源：http://ki.9csxet.cn

for (auto &x : v) { std::cout << x; }
来源：http://ce.9csxet.cn

[S35] C++：map
来源：http://bs.shxzukj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tw.521024.cn

[S36] C++：unordered_map
来源：http://ou.asd995.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sx.jianghongdianzi.cn

[S37] C++：set
来源：http://st.jianghongdianzi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yk.muxihuayi.cn

[S38] C++：排序
来源：http://pe.shtwfgs.cn

std::sort(v.begin(), v.end());
来源：http://qp.huixinmuqiang.cn

[S39] C++：自定义比较器排序
来源：http://tt.9csxet.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://be.jianghongdianzi.cn

[S40] C++：查找元素
来源：http://ln.hahajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pv.shtwfgs.cn

[S41] C++：类与构造函数
来源：http://gp.newstarts.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ch.huixiangedu.cn

[S42] C++：继承与虚函数
来源：http://kq.szsharing.cn

class B : public Base { public: void f() override {} };
来源：http://jk.shxzskj.cn

[S43] C++：智能指针
来源：http://kb.huixiangedu.cn

auto p = std::make_unique<int>(5);
来源：http://iz.nszjky.cn

[S44] C++：引用传参
来源：http://kh.panjiajie.cn

void inc(int &x) { ++x; }
来源：http://be.szxytkj.cn

[S45] C++：lambda
来源：http://ti.shxzskj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jg.wgjwhj.cn

[S46] C++：函数模板
来源：http://gl.huanxung.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cr.shtwfgs.cn

[S47] C++：结构化绑定遍历
来源：http://pd.shxzskj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ob.yuntaijiaju.cn

[S48] C++：逐行读文件
来源：http://ye.panjiajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://sq.gzmigu.cn

while (std::getline(in, line)) { }
来源：http://ai.shtwfgs.cn

[S49] C++：写文件
来源：http://pq.9csxet.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wm.newstarts.cn

[S50] C++：格式化数字
来源：http://bh.huixinmuqiang.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wn.asd995.cn

[S51] C++：显式类型转换
来源：http://sv.huixinmuqiang.cn

static_cast<double>(a) / b
来源：http://dj.yuexingan06.cn

[S52] C++：const 与 noexcept
来源：http://yk.yuntaijiaju.cn

int size() const noexcept { return n_; }
来源：http://hx.lnxyls.cn

[S53] C++：移动语义
来源：http://do.colortex.cn

std::vector<int> w = std::move(v);
来源：http://yi.huixinmuqiang.cn

[S54] C++：异常处理
来源：http://cb.szxytkj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nx.jctech888.com.cn

[S55] C++：结构化绑定
来源：http://ah.jianghongdianzi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://da.jianghongdianzi.cn

[S56] C++：optional
来源：http://pi.lnxyls.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hl.lnxyls.cn

[S57] C++：编译期常量
来源：http://we.nszjky.cn

constexpr int N = 10;
来源：http://pn.shxzskj.cn

[S58] C++：命名空间
来源：http://al.szxytkj.cn

namespace ns { int f() { return 1; } }
来源：http://cy.szxytkj.cn

[S59] C++：静态断言
来源：http://ot.shxzskj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vi.shtwfgs.cn

[S60] C++：遍历并删除元素
来源：http://xx.bookmarksfly.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jy.jianghongdianzi.cn

================================================================================
来源：http://fc.521024.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zt.jctech888.com.cn

================================================================================
来源：http://el.bookmarksfly.cn

[T01] Kotlin：Hello World
来源：http://vv.jianghongdianzi.cn

println("Hello")
来源：http://sr.chemitech.net.cn

[T02] Kotlin：变量
来源：http://vb.jctech888.com.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rn.lnxyls.cn

[T03] Kotlin：字符串模板
来源：http://qn.shtwfgs.cn

"值: $b"
来源：http://zi.panjiajie.cn

[T04] Kotlin：空安全
来源：http://bw.gzmigu.cn

val n: String? = null;  n?.length
来源：http://xq.colortex.cn

[T05] Kotlin：when 表达式
来源：http://cv.muxihuayi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vw.nicolike.cn

[T06] Kotlin：集合映射
来源：http://sg.panjiajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ph.9csxet.cn

[T07] Kotlin：集合过滤
来源：http://uy.szsharing.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ut.huixinmuqiang.cn

[T08] Kotlin：数据类
来源：http://ie.huixiangedu.cn

data class User(val name: String, val age: Int)
来源：http://vb.colortex.cn

[T09] Kotlin：扩展函数
来源：http://eo.9csxet.cn

fun String.exclaim() = this + "!"
来源：http://vh.szsharing.cn

[T10] Kotlin：默认参数
来源：http://ij.szxytkj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rt.gzmigu.cn

[T11] Kotlin：协程
来源：http://kv.bjjhwx.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://kl.hahajie.cn

[T12] Kotlin：解构声明
来源：http://xh.muxihuayi.cn

val (a, b) = Pair(1, 2)
来源：http://si.gzmigu.cn

[T13] Kotlin：只读 Map
来源：http://qr.asd995.cn

val m = mapOf("a" to 1)
来源：http://gs.asd995.cn

[T14] Kotlin：循环
来源：http://ld.yuntaijiaju.cn

for (i in 1..10) println(i)
来源：http://ck.asd995.cn

[T15] Kotlin：接口
来源：http://dk.asd995.cn

interface Shape { fun area(): Double }
来源：http://jl.wgjwhj.cn

[T16] Swift：Hello World
来源：http://dh.bjjhwx.cn

print("Hello")
来源：http://ok.nszjky.cn

[T17] Swift：变量与常量
来源：http://cc.huixiangedu.cn

var a = 1;  let b = 2
来源：http://sp.wgjwhj.cn

[T18] Swift：字符串插值
来源：http://hu.shxzskj.cn

"值: \(b)"
来源：http://zv.hnjuh.cn

[T19] Swift：可选绑定
来源：http://go.nszjky.cn

if let n = opt { print(n) }
来源：http://ry.huixiangedu.cn

[T20] Swift：数组操作
来源：http://ct.huixiangedu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ou.yuexingan06.cn

[T21] Swift：遍历
来源：http://hn.huixinmuqiang.cn

for x in a { print(x) }
来源：http://nv.chemitech.net.cn

[T22] Swift：字典
来源：http://cy.nszjky.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ak.nszjky.cn

[T23] Swift：函数
来源：http://da.huanxung.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rq.shxzskj.cn

[T24] Swift：闭包
来源：http://jk.szsharing.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qe.yuntaijiaju.cn

[T25] Swift：结构体
来源：http://tr.colortex.cn

struct P { var x: Int }
来源：http://vd.chemitech.net.cn

[T26] Swift：类与重写
来源：http://yb.yuntaijiaju.cn

class A: Base { override func f() {} }
来源：http://fp.jianghongdianzi.cn

[T27] Swift：错误处理
来源：http://fz.hahajie.cn

do { try f() } catch { print(error) }
来源：http://mv.colortex.cn

[T28] Swift：枚举
来源：http://bk.huixinmuqiang.cn

enum Color { case red, green }
来源：http://pq.huanxung.cn

[T29] Swift：guard 提前返回
来源：http://pl.bjjhwx.cn

guard let x = opt else { return }
来源：http://zh.shtwfgs.cn

[T30] Swift：协议
来源：http://ei.wgjwhj.cn

protocol Shape { func area() -> Double }
来源：http://hm.huixinmuqiang.cn

[T31] Lua：Hello World
来源：http://km.nszjky.cn

print("Hello")
来源：http://yq.shxzskj.cn

[T32] Lua：局部变量
来源：http://xm.szsharing.cn

local a = 1
来源：http://vh.shxzukj.cn

[T33] Lua：表（数组）
来源：http://zm.shxzukj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://kx.shxzukj.cn

[T34] Lua：遍历表
来源：http://yq.hahajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ny.panjiajie.cn

[T35] Lua：字典表
来源：http://hr.jctech888.com.cn

local d = { a = 1 };  d.b = 2
来源：http://ip.yuntaijiaju.cn

[T36] Lua：函数
来源：http://mg.panjiajie.cn

function add(a, b) return a + b end
来源：http://xb.newstarts.cn

[T37] Lua：字符串拼接
来源：http://dp.jianghongdianzi.cn

"a" .. "b"
来源：http://hh.colortex.cn

[T38] Lua：条件
来源：http://bk.asd995.cn

if x > 0 then print("正") end
来源：http://xd.bjjhwx.cn

[T39] Lua：模式匹配
来源：http://lw.huanxung.cn

string.find(s, "%d+")
来源：http://yx.jianghongdianzi.cn

[T40] Lua：元表
来源：http://oc.shtwfgs.cn

setmetatable({}, { __index = base })
来源：http://ze.chemitech.net.cn

[T41] Perl：Hello World
来源：http://mu.muxihuayi.cn

print "Hello\n";
来源：http://ub.asd995.cn

[T42] Perl：变量类型
来源：http://eo.huixiangedu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ck.bjjhwx.cn

[T43] Perl：字符串插值
来源：http://xw.shxzukj.cn

"值: $a"
来源：http://ez.shtwfgs.cn

[T44] Perl：条件
来源：http://ng.shtwfgs.cn

if ($a > 0) { print "正"; }
来源：http://li.shxzukj.cn

[T45] Perl：数组遍历
来源：http://iq.chemitech.net.cn

for my $x (@arr) { print $x; }
来源：http://tl.muxihuayi.cn

[T46] Perl：哈希操作
来源：http://bz.shxzukj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ep.gzmigu.cn

[T47] Perl：正则捕获
来源：http://dl.nszjky.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://sl.szxytkj.cn

[T48] Perl：正则替换
来源：http://mh.huixinmuqiang.cn

$s =~ s/old/new/g;
来源：http://lx.9csxet.cn

[T49] Perl：函数
来源：http://mn.huixiangedu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tu.muxihuayi.cn

[T50] Perl：逐行读文件
来源：http://fi.shtwfgs.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wz.shtwfgs.cn

while (my $line = <$fh>) { print $line; }
来源：http://wg.shxzukj.cn

[T51] Scala：Hello World
来源：http://ab.hahajie.cn

println("Hello")
来源：http://od.shxzukj.cn

[T52] Scala：变量
来源：http://ib.szsharing.cn

val a = 1;  var b = 2
来源：http://md.asd995.cn

[T53] Scala：字符串插值
来源：http://os.yuexingan06.cn

s"值: $b"
来源：http://zo.panjiajie.cn

[T54] Scala：集合映射
来源：http://nd.521024.cn

List(1, 2, 3).map(_ * 2)
来源：http://ho.521024.cn

[T55] Scala：集合过滤
来源：http://db.lnxyls.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gb.yuntaijiaju.cn

[T56] Scala：样例类
来源：http://ok.bjjhwx.cn

case class User(name: String, age: Int)
来源：http://kj.hahajie.cn

[T57] Scala：模式匹配
来源：http://wa.huixiangedu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://dl.hahajie.cn

[T58] Scala：函数定义
来源：http://gu.shxzukj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://as.huixiangedu.cn

[T59] Scala：循环
来源：http://ne.yuntaijiaju.cn

for (i <- 1 to 10) println(i)
来源：http://xj.yuntaijiaju.cn

[T60] Scala：折叠
来源：http://bo.hahajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gj.szxytkj.cn

================================================================================
来源：http://rn.521024.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vj.shxzukj.cn

================================================================================
来源：http://di.521024.cn

[U01] Py：创建虚拟环境
来源：http://cj.szsharing.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ar.bookmarksfly.cn

[U02] Py：导出 / 安装依赖
来源：http://oi.yuntaijiaju.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cl.huixiangedu.cn

[U03] Py：加载 .env 配置
来源：http://wq.asd995.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://sk.huixinmuqiang.cn

[U04] Py：变量调试打印
来源：http://hn.muxihuayi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fq.shxzukj.cn

[U05] Py：列表去重且保序
来源：http://tb.newstarts.cn

list(dict.fromkeys(arr))
来源：http://yw.asd995.cn

[U06] Py：合并两个字典
来源：http://hl.newstarts.cn

{**a, **b}
来源：http://so.szsharing.cn

[U07] Py：反转字典键值
来源：http://eh.newstarts.cn

{v: k for k, v in d.items()}
来源：http://uy.hahajie.cn

[U08] Py：展平二维列表
来源：http://ed.colortex.cn

[y for x in nested for y in x]
来源：http://sx.yuexingan06.cn

[U09] Py：字典取最大值的键
来源：http://mb.hahajie.cn

max(d, key=d.get)
来源：http://ns.nszjky.cn

[U10] Py：按值排序字典
来源：http://rb.shxzskj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bz.lnxyls.cn

[U11] Py：生成器表达式
来源：http://aa.huanxung.cn

(x * 2 for x in arr)
来源：http://cs.huanxung.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rk.huixinmuqiang.cn

Counter(arr).most_common(3)
来源：http://ks.bookmarksfly.cn

[U13] Py：固定长度队列
来源：http://sc.shxzukj.cn

deque(maxlen=10)
来源：http://jr.colortex.cn

[U14] Py：分组收集到列表
来源：http://yq.gzmigu.cn

defaultdict(list)
来源：http://xp.yuntaijiaju.cn

[U15] Py：高精度计时
来源：http://xq.bookmarksfly.cn

t = time.perf_counter()
来源：http://ti.shtwfgs.cn

[U16] Py：命令行参数解析
来源：http://hp.huixiangedu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ha.shxzskj.cn

[U17] Py：初始化日志
来源：http://oz.bookmarksfly.cn

logging.basicConfig(level=logging.INFO)
来源：http://uz.jctech888.com.cn

[U18] Py：预编译正则
来源：http://jk.wgjwhj.cn

pat = re.compile(r"\d+")
来源：http://ae.9csxet.cn

[U19] Py：正则替换带回调
来源：http://og.jianghongdianzi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pi.szsharing.cn

[U20] Py：缓存函数结果
来源：http://gw.nicolike.cn

@functools.lru_cache(maxsize=None)
来源：http://tx.yuexingan06.cn

[U21] Py：自定义上下文管理器
来源：http://ah.chemitech.net.cn

@contextlib.contextmanager
来源：http://kj.shxzskj.cn

[U22] Py：矩阵转置
来源：http://jn.szsharing.cn

list(zip(*m))
来源：http://xg.nszjky.cn

[U23] Py：分块读取大文件
来源：http://jt.wgjwhj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xx.newstarts.cn

[U24] Py：路径操作
来源：http://sy.jianghongdianzi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qu.panjiajie.cn

[U25] Py：CSV 按字典读
来源：http://pl.9csxet.cn

csv.DictReader(f)
来源：http://as.newstarts.cn

[U26] Py：并发下载
来源：http://ps.hahajie.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://he.muxihuayi.cn

[U27] Py：异步 HTTP
来源：http://ts.shxzukj.cn

aiohttp.ClientSession() 配合 async with
来源：http://la.panjiajie.cn

[U28] Py：类型别名
来源：http://hp.yuexingan06.cn

UserId = int
来源：http://tt.yuntaijiaju.cn

[U29] Py：属性校验
来源：http://wf.gzmigu.cn

@property 与 @x.setter 配合
来源：http://el.huixiangedu.cn

[U30] Py：数据类
来源：http://nv.szxytkj.cn

@dataclass(slots=True)
来源：http://ke.hnjuh.cn

[U31] Py：单测
来源：http://fw.hnjuh.cn

python -m pytest -q
来源：http://ri.jctech888.com.cn

[U32] Py：代码格式化
来源：http://op.szxytkj.cn

ruff format . && ruff check --fix .
来源：http://in.huixinmuqiang.cn

[U33] Py：打包发布
来源：http://xj.shxzukj.cn

python -m build  （依赖 pyproject.toml）
来源：http://hd.hnjuh.cn

[U34] Py：判断编码
来源：http://bn.haigaiapp.cn

chardet.detect(raw)
来源：http://bz.jianghongdianzi.cn


<!-- 参考信息 -->