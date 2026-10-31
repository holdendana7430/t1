代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ug.bjjhwx.cn

[S10] C：指针与解引用
来源：http://zl.jianghongdianzi.cn

int *p = &a;  *p = 5;
来源：http://qp.panjiajie.cn

[S11] C：逐行读文件
来源：http://jq.chemitech.net.cn

FILE *f = fopen("a.txt", "r");
来源：http://tt.haigaiapp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://cy.haigaiapp.cn

fclose(f);
来源：http://jq.gzmigu.cn

[S12] C：写文件
来源：http://gs.hnjuh.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hb.asd995.cn

[S13] C：宏定义
来源：http://nx.huixiangedu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vk.shtwfgs.cn

[S14] C：枚举
来源：http://lu.asd995.cn

enum Color { RED, GREEN, BLUE };
来源：http://fe.huixiangedu.cn

[S15] C：类型转换
来源：http://jo.jctech888.com.cn

(double) a / b
来源：http://tf.szsharing.cn

[S16] C：位操作置位
来源：http://vn.panjiajie.cn

x |= (1 << 3);
来源：http://xo.shxzukj.cn

[S17] C：安全拼接字符串
来源：http://fe.panjiajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pg.jctech888.com.cn

[S18] C：命令行参数
来源：http://wy.szsharing.cn

int main(int argc, char **argv)
来源：http://bf.panjiajie.cn

[S19] C：快速排序
来源：http://iy.bookmarksfly.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vn.yuntaijiaju.cn

[S20] C：二分查找
来源：http://hb.jctech888.com.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://aa.shxzskj.cn

[S21] C：字符类别判断
来源：http://xe.nicolike.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tu.huanxung.cn

[S22] C：字符串转数字
来源：http://rv.chemitech.net.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fv.szsharing.cn

[S23] C：随机数
来源：http://zm.colortex.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://sv.shtwfgs.cn

[S24] C：获取本地时间
来源：http://ij.hahajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ub.yuexingan06.cn

[S25] C：内存拷贝
来源：http://bb.hahajie.cn

memcpy(dst, src, n);
来源：http://oa.521024.cn

[S26] C：内存清零
来源：http://rv.nszjky.cn

memset(a, 0, sizeof a);
来源：http://ye.shxzskj.cn

[S27] C：定义常量
来源：http://ek.lnxyls.cn

const double PI = 3.14159;
来源：http://jk.nicolike.cn

[S28] C：静态变量
来源：http://gc.wgjwhj.cn

static int counter = 0;
来源：http://we.shxzukj.cn

[S29] C：变参函数
来源：http://fj.nicolike.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gk.9csxet.cn

[S30] C：头文件保护
来源：http://yt.hahajie.cn

#ifndef X_H
来源：http://sb.shxzskj.cn

#define X_H
来源：http://fj.jianghongdianzi.cn

#endif
来源：http://sl.asd995.cn

[S31] C++：Hello World
来源：http://ub.huixiangedu.cn

#include <iostream>
来源：http://fu.muxihuayi.cn

int main() { std::cout << "Hello\n"; }
来源：http://he.szsharing.cn

[S32] C++：字符串
来源：http://pt.9csxet.cn

std::string s = "hi";  s += "!";
来源：http://rm.newstarts.cn

[S33] C++：vector 增删
来源：http://yf.nicolike.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ix.chemitech.net.cn

[S34] C++：遍历 vector
来源：http://wi.haigaiapp.cn

for (auto &x : v) { std::cout << x; }
来源：http://tv.shtwfgs.cn

[S35] C++：map
来源：http://lv.wgjwhj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://af.nicolike.cn

[S36] C++：unordered_map
来源：http://kw.haigaiapp.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fd.muxihuayi.cn

[S37] C++：set
来源：http://rk.huixiangedu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yq.9csxet.cn

[S38] C++：排序
来源：http://ga.jianghongdianzi.cn

std::sort(v.begin(), v.end());
来源：http://ux.521024.cn

[S39] C++：自定义比较器排序
来源：http://ve.jctech888.com.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ab.szxytkj.cn

[S40] C++：查找元素
来源：http://hc.hahajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gi.shxzukj.cn

[S41] C++：类与构造函数
来源：http://ei.jctech888.com.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fz.yuntaijiaju.cn

[S42] C++：继承与虚函数
来源：http://aq.nszjky.cn

class B : public Base { public: void f() override {} };
来源：http://id.wgjwhj.cn

[S43] C++：智能指针
来源：http://hd.muxihuayi.cn

auto p = std::make_unique<int>(5);
来源：http://pu.newstarts.cn

[S44] C++：引用传参
来源：http://dq.hahajie.cn

void inc(int &x) { ++x; }
来源：http://dy.bjjhwx.cn

[S45] C++：lambda
来源：http://pa.jctech888.com.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gh.huixiangedu.cn

[S46] C++：函数模板
来源：http://tk.shxzskj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fk.yuexingan06.cn

[S47] C++：结构化绑定遍历
来源：http://mf.gzmigu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ig.shtwfgs.cn

[S48] C++：逐行读文件
来源：http://ti.huixiangedu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ul.huixiangedu.cn

while (std::getline(in, line)) { }
来源：http://qa.jianghongdianzi.cn

[S49] C++：写文件
来源：http://og.huanxung.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ho.muxihuayi.cn

[S50] C++：格式化数字
来源：http://fo.yuexingan06.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ln.hahajie.cn

[S51] C++：显式类型转换
来源：http://tf.chemitech.net.cn

static_cast<double>(a) / b
来源：http://dp.szxytkj.cn

[S52] C++：const 与 noexcept
来源：http://yo.muxihuayi.cn

int size() const noexcept { return n_; }
来源：http://cz.bjjhwx.cn

[S53] C++：移动语义
来源：http://db.lnxyls.cn

std::vector<int> w = std::move(v);
来源：http://cv.nicolike.cn

[S54] C++：异常处理
来源：http://lr.shtwfgs.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zl.jianghongdianzi.cn

[S55] C++：结构化绑定
来源：http://me.shxzukj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gh.jianghongdianzi.cn

[S56] C++：optional
来源：http://hb.jianghongdianzi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qa.jianghongdianzi.cn

[S57] C++：编译期常量
来源：http://in.shxzukj.cn

constexpr int N = 10;
来源：http://of.521024.cn

[S58] C++：命名空间
来源：http://fr.szsharing.cn

namespace ns { int f() { return 1; } }
来源：http://qd.huixiangedu.cn

[S59] C++：静态断言
来源：http://uq.hnjuh.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hx.muxihuayi.cn

[S60] C++：遍历并删除元素
来源：http://xt.lnxyls.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bz.szxytkj.cn

================================================================================
来源：http://op.521024.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://aw.bjjhwx.cn

================================================================================
来源：http://wd.huixinmuqiang.cn

[T01] Kotlin：Hello World
来源：http://wu.yuntaijiaju.cn

println("Hello")
来源：http://sr.gzmigu.cn

[T02] Kotlin：变量
来源：http://wo.asd995.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gh.jianghongdianzi.cn

[T03] Kotlin：字符串模板
来源：http://ti.haigaiapp.cn

"值: $b"
来源：http://pe.hahajie.cn

[T04] Kotlin：空安全
来源：http://lx.wgjwhj.cn

val n: String? = null;  n?.length
来源：http://mo.hahajie.cn

[T05] Kotlin：when 表达式
来源：http://gt.huixinmuqiang.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rg.huanxung.cn

[T06] Kotlin：集合映射
来源：http://tf.lnxyls.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://pp.yuntaijiaju.cn

[T07] Kotlin：集合过滤
来源：http://qq.asd995.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lt.szsharing.cn

[T08] Kotlin：数据类
来源：http://po.newstarts.cn

data class User(val name: String, val age: Int)
来源：http://gf.hnjuh.cn

[T09] Kotlin：扩展函数
来源：http://km.shtwfgs.cn

fun String.exclaim() = this + "!"
来源：http://pp.haigaiapp.cn

[T10] Kotlin：默认参数
来源：http://lr.huixiangedu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://sb.newstarts.cn

[T11] Kotlin：协程
来源：http://qq.521024.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ae.huanxung.cn

[T12] Kotlin：解构声明
来源：http://uz.jianghongdianzi.cn

val (a, b) = Pair(1, 2)
来源：http://ca.jianghongdianzi.cn

[T13] Kotlin：只读 Map
来源：http://ia.asd995.cn

val m = mapOf("a" to 1)
来源：http://we.yuntaijiaju.cn

[T14] Kotlin：循环
来源：http://dq.szsharing.cn

for (i in 1..10) println(i)
来源：http://fy.521024.cn

[T15] Kotlin：接口
来源：http://zt.colortex.cn

interface Shape { fun area(): Double }
来源：http://xy.huixiangedu.cn

[T16] Swift：Hello World
来源：http://oi.lnxyls.cn

print("Hello")
来源：http://ol.bjjhwx.cn

[T17] Swift：变量与常量
来源：http://tw.gzmigu.cn

var a = 1;  let b = 2
来源：http://gp.shxzskj.cn

[T18] Swift：字符串插值
来源：http://bi.szxytkj.cn

"值: \(b)"
来源：http://ss.hnjuh.cn

[T19] Swift：可选绑定
来源：http://zi.haigaiapp.cn

if let n = opt { print(n) }
来源：http://qa.huixiangedu.cn

[T20] Swift：数组操作
来源：http://gq.szsharing.cn

var a = [1, 2, 3];  a.append(4)
来源：http://yv.szsharing.cn

[T21] Swift：遍历
来源：http://ce.szxytkj.cn

for x in a { print(x) }
来源：http://og.gzmigu.cn

[T22] Swift：字典
来源：http://od.huixinmuqiang.cn

var d = ["a": 1];  d["b"] = 2
来源：http://lq.shxzskj.cn

[T23] Swift：函数
来源：http://ee.nszjky.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://md.haigaiapp.cn

[T24] Swift：闭包
来源：http://oi.huanxung.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://im.nszjky.cn

[T25] Swift：结构体
来源：http://ak.bookmarksfly.cn

struct P { var x: Int }
来源：http://ml.huixiangedu.cn

[T26] Swift：类与重写
来源：http://uc.bjjhwx.cn

class A: Base { override func f() {} }
来源：http://hh.huixiangedu.cn

[T27] Swift：错误处理
来源：http://pk.shtwfgs.cn

do { try f() } catch { print(error) }
来源：http://tv.szxytkj.cn

[T28] Swift：枚举
来源：http://qv.hnjuh.cn

enum Color { case red, green }
来源：http://kq.9csxet.cn

[T29] Swift：guard 提前返回
来源：http://oq.szsharing.cn

guard let x = opt else { return }
来源：http://tu.gzmigu.cn

[T30] Swift：协议
来源：http://dq.asd995.cn

protocol Shape { func area() -> Double }
来源：http://xz.yuntaijiaju.cn

[T31] Lua：Hello World
来源：http://ai.gzmigu.cn

print("Hello")
来源：http://op.9csxet.cn

[T32] Lua：局部变量
来源：http://dy.haigaiapp.cn

local a = 1
来源：http://hl.bookmarksfly.cn

[T33] Lua：表（数组）
来源：http://px.colortex.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fa.yuexingan06.cn

[T34] Lua：遍历表
来源：http://hd.yuexingan06.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://nj.szxytkj.cn

[T35] Lua：字典表
来源：http://oq.szxytkj.cn

local d = { a = 1 };  d.b = 2
来源：http://qd.colortex.cn

[T36] Lua：函数
来源：http://jb.asd995.cn

function add(a, b) return a + b end
来源：http://qb.nicolike.cn

[T37] Lua：字符串拼接
来源：http://cf.nszjky.cn

"a" .. "b"
来源：http://ls.haigaiapp.cn

[T38] Lua：条件
来源：http://de.nicolike.cn

if x > 0 then print("正") end
来源：http://la.szxytkj.cn

[T39] Lua：模式匹配
来源：http://hc.bjjhwx.cn

string.find(s, "%d+")
来源：http://oa.shxzukj.cn

[T40] Lua：元表
来源：http://cq.jctech888.com.cn

setmetatable({}, { __index = base })
来源：http://hs.lnxyls.cn

[T41] Perl：Hello World
来源：http://ru.nicolike.cn

print "Hello\n";
来源：http://dj.chemitech.net.cn

[T42] Perl：变量类型
来源：http://ih.bookmarksfly.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ci.muxihuayi.cn

[T43] Perl：字符串插值
来源：http://eh.yuexingan06.cn

"值: $a"
来源：http://zs.jianghongdianzi.cn

[T44] Perl：条件
来源：http://sy.szxytkj.cn

if ($a > 0) { print "正"; }
来源：http://nd.shxzukj.cn

[T45] Perl：数组遍历
来源：http://hx.panjiajie.cn

for my $x (@arr) { print $x; }
来源：http://qq.shxzukj.cn

[T46] Perl：哈希操作
来源：http://rq.yuexingan06.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vi.wgjwhj.cn

[T47] Perl：正则捕获
来源：http://kt.nicolike.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://mx.jianghongdianzi.cn

[T48] Perl：正则替换
来源：http://ho.nicolike.cn

$s =~ s/old/new/g;
来源：http://sf.muxihuayi.cn

[T49] Perl：函数
来源：http://if.jianghongdianzi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ld.colortex.cn

[T50] Perl：逐行读文件
来源：http://ah.nszjky.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://kx.shxzskj.cn

while (my $line = <$fh>) { print $line; }
来源：http://hp.wgjwhj.cn

[T51] Scala：Hello World
来源：http://up.nicolike.cn

println("Hello")
来源：http://ik.521024.cn

[T52] Scala：变量
来源：http://fy.gzmigu.cn

val a = 1;  var b = 2
来源：http://ao.haigaiapp.cn

[T53] Scala：字符串插值
来源：http://wj.hahajie.cn

s"值: $b"
来源：http://fn.newstarts.cn

[T54] Scala：集合映射
来源：http://cm.panjiajie.cn

List(1, 2, 3).map(_ * 2)
来源：http://vf.521024.cn

[T55] Scala：集合过滤
来源：http://oe.nicolike.cn

List(1, 2, 3).filter(_ > 1)
来源：http://um.bjjhwx.cn

[T56] Scala：样例类
来源：http://dm.huixinmuqiang.cn

case class User(name: String, age: Int)
来源：http://np.wgjwhj.cn

[T57] Scala：模式匹配
来源：http://df.hnjuh.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://qk.newstarts.cn

[T58] Scala：函数定义
来源：http://kt.shxzukj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wn.521024.cn

[T59] Scala：循环
来源：http://tc.hnjuh.cn

for (i <- 1 to 10) println(i)
来源：http://fd.jianghongdianzi.cn

[T60] Scala：折叠
来源：http://xb.hnjuh.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gh.hnjuh.cn

================================================================================
来源：http://ec.nszjky.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rd.shxzukj.cn

================================================================================
来源：http://ps.szsharing.cn

[U01] Py：创建虚拟环境
来源：http://xf.jctech888.com.cn

python -m venv .venv && source .venv/bin/activate
来源：http://xh.szxytkj.cn

[U02] Py：导出 / 安装依赖
来源：http://qj.lnxyls.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lp.hahajie.cn

[U03] Py：加载 .env 配置
来源：http://om.yuexingan06.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rg.521024.cn

[U04] Py：变量调试打印
来源：http://tu.wgjwhj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://av.szsharing.cn

[U05] Py：列表去重且保序
来源：http://ty.jianghongdianzi.cn

list(dict.fromkeys(arr))
来源：http://ys.9csxet.cn

[U06] Py：合并两个字典
来源：http://is.asd995.cn

{**a, **b}
来源：http://bt.nszjky.cn

[U07] Py：反转字典键值
来源：http://aw.gzmigu.cn

{v: k for k, v in d.items()}
来源：http://ur.9csxet.cn

[U08] Py：展平二维列表
来源：http://ya.9csxet.cn

[y for x in nested for y in x]
来源：http://kb.bookmarksfly.cn

[U09] Py：字典取最大值的键
来源：http://kp.colortex.cn

max(d, key=d.get)
来源：http://dz.jctech888.com.cn

[U10] Py：按值排序字典
来源：http://ih.panjiajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bt.gzmigu.cn

[U11] Py：生成器表达式
来源：http://so.gzmigu.cn

(x * 2 for x in arr)
来源：http://go.huixiangedu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://nf.asd995.cn

Counter(arr).most_common(3)
来源：http://zt.gzmigu.cn

[U13] Py：固定长度队列
来源：http://xq.nszjky.cn

deque(maxlen=10)
来源：http://fu.colortex.cn

[U14] Py：分组收集到列表
来源：http://kg.chemitech.net.cn

defaultdict(list)
来源：http://zb.huixinmuqiang.cn

[U15] Py：高精度计时
来源：http://nj.gzmigu.cn

t = time.perf_counter()
来源：http://hu.newstarts.cn

[U16] Py：命令行参数解析
来源：http://ai.szsharing.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ed.huixiangedu.cn

[U17] Py：初始化日志
来源：http://vs.bookmarksfly.cn

logging.basicConfig(level=logging.INFO)
来源：http://cj.asd995.cn

[U18] Py：预编译正则
来源：http://ss.asd995.cn

pat = re.compile(r"\d+")
来源：http://dk.bjjhwx.cn

[U19] Py：正则替换带回调
来源：http://tk.haigaiapp.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gz.lnxyls.cn

[U20] Py：缓存函数结果
来源：http://pl.521024.cn

@functools.lru_cache(maxsize=None)
来源：http://zl.huixiangedu.cn

[U21] Py：自定义上下文管理器
来源：http://yf.colortex.cn

@contextlib.contextmanager
来源：http://qy.shxzskj.cn

[U22] Py：矩阵转置
来源：http://si.yuntaijiaju.cn

list(zip(*m))
来源：http://eu.yuntaijiaju.cn

[U23] Py：分块读取大文件
来源：http://fs.colortex.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lv.gzmigu.cn

[U24] Py：路径操作
来源：http://ah.panjiajie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://on.shtwfgs.cn

[U25] Py：CSV 按字典读
来源：http://hs.bjjhwx.cn

csv.DictReader(f)
来源：http://ky.szxytkj.cn

[U26] Py：并发下载
来源：http://lm.hahajie.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://sp.yuntaijiaju.cn

[U27] Py：异步 HTTP
来源：http://yx.hahajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://yh.chemitech.net.cn

[U28] Py：类型别名
来源：http://wm.gzmigu.cn

UserId = int
来源：http://un.huanxung.cn

[U29] Py：属性校验
来源：http://sv.huixiangedu.cn

@property 与 @x.setter 配合
来源：http://zo.bookmarksfly.cn

[U30] Py：数据类
来源：http://qj.colortex.cn

@dataclass(slots=True)
来源：http://sm.jianghongdianzi.cn

[U31] Py：单测
来源：http://jz.bjjhwx.cn

python -m pytest -q
来源：http://ks.newstarts.cn

[U32] Py：代码格式化
来源：http://cw.huixinmuqiang.cn

ruff format . && ruff check --fix .
来源：http://xg.newstarts.cn


<!-- 参考信息 -->