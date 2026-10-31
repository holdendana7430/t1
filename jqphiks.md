代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sm.yuntaijiaju.cn

[S10] C：指针与解引用
来源：http://mc.nicolike.cn

int *p = &a;  *p = 5;
来源：http://gc.huixiangedu.cn

[S11] C：逐行读文件
来源：http://gi.newstarts.cn

FILE *f = fopen("a.txt", "r");
来源：http://gb.nicolike.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://da.shxzukj.cn

fclose(f);
来源：http://lb.asd995.cn

[S12] C：写文件
来源：http://th.shtwfgs.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kd.shxzskj.cn

[S13] C：宏定义
来源：http://wo.yuntaijiaju.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sh.521024.cn

[S14] C：枚举
来源：http://np.haigaiapp.cn

enum Color { RED, GREEN, BLUE };
来源：http://tp.panjiajie.cn

[S15] C：类型转换
来源：http://fj.nszjky.cn

(double) a / b
来源：http://ie.szxytkj.cn

[S16] C：位操作置位
来源：http://fe.asd995.cn

x |= (1 << 3);
来源：http://uk.szxytkj.cn

[S17] C：安全拼接字符串
来源：http://tl.yuexingan06.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bz.huixinmuqiang.cn

[S18] C：命令行参数
来源：http://fa.chemitech.net.cn

int main(int argc, char **argv)
来源：http://bo.jianghongdianzi.cn

[S19] C：快速排序
来源：http://fq.szsharing.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fq.szsharing.cn

[S20] C：二分查找
来源：http://uy.shxzukj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bs.yuexingan06.cn

[S21] C：字符类别判断
来源：http://yc.521024.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xo.shxzukj.cn

[S22] C：字符串转数字
来源：http://hf.newstarts.cn

atoi("42");  strtod("3.14", NULL);
来源：http://er.chemitech.net.cn

[S23] C：随机数
来源：http://ve.hahajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fh.huixiangedu.cn

[S24] C：获取本地时间
来源：http://wj.chemitech.net.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mt.haigaiapp.cn

[S25] C：内存拷贝
来源：http://mx.gzmigu.cn

memcpy(dst, src, n);
来源：http://pk.hahajie.cn

[S26] C：内存清零
来源：http://ue.huixinmuqiang.cn

memset(a, 0, sizeof a);
来源：http://oy.lnxyls.cn

[S27] C：定义常量
来源：http://by.nicolike.cn

const double PI = 3.14159;
来源：http://to.yuexingan06.cn

[S28] C：静态变量
来源：http://is.yuexingan06.cn

static int counter = 0;
来源：http://cq.nicolike.cn

[S29] C：变参函数
来源：http://pz.lnxyls.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mm.bookmarksfly.cn

[S30] C：头文件保护
来源：http://lb.hnjuh.cn

#ifndef X_H
来源：http://pe.hahajie.cn

#define X_H
来源：http://mk.jianghongdianzi.cn

#endif
来源：http://vz.asd995.cn

[S31] C++：Hello World
来源：http://fi.huixinmuqiang.cn

#include <iostream>
来源：http://er.gzmigu.cn

int main() { std::cout << "Hello\n"; }
来源：http://dm.521024.cn

[S32] C++：字符串
来源：http://qj.hnjuh.cn

std::string s = "hi";  s += "!";
来源：http://zm.huixiangedu.cn

[S33] C++：vector 增删
来源：http://jy.colortex.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bc.nszjky.cn

[S34] C++：遍历 vector
来源：http://pt.haigaiapp.cn

for (auto &x : v) { std::cout << x; }
来源：http://bh.huixiangedu.cn

[S35] C++：map
来源：http://sd.521024.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zs.9csxet.cn

[S36] C++：unordered_map
来源：http://fe.bookmarksfly.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wn.yuntaijiaju.cn

[S37] C++：set
来源：http://az.szxytkj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fp.wgjwhj.cn

[S38] C++：排序
来源：http://aw.colortex.cn

std::sort(v.begin(), v.end());
来源：http://mo.szxytkj.cn

[S39] C++：自定义比较器排序
来源：http://wz.yuexingan06.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rq.nszjky.cn

[S40] C++：查找元素
来源：http://og.hahajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ky.asd995.cn

[S41] C++：类与构造函数
来源：http://dc.huixiangedu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lv.haigaiapp.cn

[S42] C++：继承与虚函数
来源：http://tc.muxihuayi.cn

class B : public Base { public: void f() override {} };
来源：http://dj.huanxung.cn

[S43] C++：智能指针
来源：http://ec.szsharing.cn

auto p = std::make_unique<int>(5);
来源：http://nf.521024.cn

[S44] C++：引用传参
来源：http://cq.yuntaijiaju.cn

void inc(int &x) { ++x; }
来源：http://si.jctech888.com.cn

[S45] C++：lambda
来源：http://ma.newstarts.cn

auto add = [](int a, int b) { return a + b; };
来源：http://je.jctech888.com.cn

[S46] C++：函数模板
来源：http://oy.jctech888.com.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ey.hnjuh.cn

[S47] C++：结构化绑定遍历
来源：http://qf.bookmarksfly.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://al.lnxyls.cn

[S48] C++：逐行读文件
来源：http://aj.jctech888.com.cn

std::ifstream in("a.txt");  std::string line;
来源：http://dg.haigaiapp.cn

while (std::getline(in, line)) { }
来源：http://oa.haigaiapp.cn

[S49] C++：写文件
来源：http://gm.haigaiapp.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://je.szsharing.cn

[S50] C++：格式化数字
来源：http://ck.nicolike.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pm.gzmigu.cn

[S51] C++：显式类型转换
来源：http://oy.gzmigu.cn

static_cast<double>(a) / b
来源：http://kf.bookmarksfly.cn

[S52] C++：const 与 noexcept
来源：http://sk.shtwfgs.cn

int size() const noexcept { return n_; }
来源：http://sb.colortex.cn

[S53] C++：移动语义
来源：http://ux.asd995.cn

std::vector<int> w = std::move(v);
来源：http://li.hahajie.cn

[S54] C++：异常处理
来源：http://ww.chemitech.net.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ss.huixinmuqiang.cn

[S55] C++：结构化绑定
来源：http://if.shxzukj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://oy.newstarts.cn

[S56] C++：optional
来源：http://dg.szsharing.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pa.panjiajie.cn

[S57] C++：编译期常量
来源：http://zp.jctech888.com.cn

constexpr int N = 10;
来源：http://fh.colortex.cn

[S58] C++：命名空间
来源：http://gq.yuexingan06.cn

namespace ns { int f() { return 1; } }
来源：http://fp.shxzukj.cn

[S59] C++：静态断言
来源：http://gv.huixiangedu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nc.huixiangedu.cn

[S60] C++：遍历并删除元素
来源：http://wv.bjjhwx.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dl.9csxet.cn

================================================================================
来源：http://oq.huixiangedu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fs.jianghongdianzi.cn

================================================================================
来源：http://tc.wgjwhj.cn

[T01] Kotlin：Hello World
来源：http://sk.yuexingan06.cn

println("Hello")
来源：http://ly.hnjuh.cn

[T02] Kotlin：变量
来源：http://mo.panjiajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nl.wgjwhj.cn

[T03] Kotlin：字符串模板
来源：http://hk.shtwfgs.cn

"值: $b"
来源：http://np.panjiajie.cn

[T04] Kotlin：空安全
来源：http://lw.yuntaijiaju.cn

val n: String? = null;  n?.length
来源：http://nv.521024.cn

[T05] Kotlin：when 表达式
来源：http://kz.9csxet.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ir.jianghongdianzi.cn

[T06] Kotlin：集合映射
来源：http://ol.shxzskj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://qc.jianghongdianzi.cn

[T07] Kotlin：集合过滤
来源：http://zu.yuntaijiaju.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vr.szsharing.cn

[T08] Kotlin：数据类
来源：http://by.huixiangedu.cn

data class User(val name: String, val age: Int)
来源：http://jx.521024.cn

[T09] Kotlin：扩展函数
来源：http://ui.hnjuh.cn

fun String.exclaim() = this + "!"
来源：http://zj.wgjwhj.cn

[T10] Kotlin：默认参数
来源：http://dj.jianghongdianzi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ab.chemitech.net.cn

[T11] Kotlin：协程
来源：http://ie.521024.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://kp.szsharing.cn

[T12] Kotlin：解构声明
来源：http://qp.jianghongdianzi.cn

val (a, b) = Pair(1, 2)
来源：http://oj.haigaiapp.cn

[T13] Kotlin：只读 Map
来源：http://bj.huixinmuqiang.cn

val m = mapOf("a" to 1)
来源：http://zw.haigaiapp.cn

[T14] Kotlin：循环
来源：http://ua.chemitech.net.cn

for (i in 1..10) println(i)
来源：http://rq.huanxung.cn

[T15] Kotlin：接口
来源：http://ge.haigaiapp.cn

interface Shape { fun area(): Double }
来源：http://tp.haigaiapp.cn

[T16] Swift：Hello World
来源：http://vi.huixiangedu.cn

print("Hello")
来源：http://qf.yuexingan06.cn

[T17] Swift：变量与常量
来源：http://ls.szsharing.cn

var a = 1;  let b = 2
来源：http://dc.panjiajie.cn

[T18] Swift：字符串插值
来源：http://yv.huixiangedu.cn

"值: \(b)"
来源：http://cs.szsharing.cn

[T19] Swift：可选绑定
来源：http://pv.huanxung.cn

if let n = opt { print(n) }
来源：http://tg.huixinmuqiang.cn

[T20] Swift：数组操作
来源：http://jo.bjjhwx.cn

var a = [1, 2, 3];  a.append(4)
来源：http://aa.shtwfgs.cn

[T21] Swift：遍历
来源：http://ad.wgjwhj.cn

for x in a { print(x) }
来源：http://tw.huanxung.cn

[T22] Swift：字典
来源：http://xj.huixiangedu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://rr.shxzukj.cn

[T23] Swift：函数
来源：http://sg.huixiangedu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ke.lnxyls.cn

[T24] Swift：闭包
来源：http://by.asd995.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://nk.huanxung.cn

[T25] Swift：结构体
来源：http://et.panjiajie.cn

struct P { var x: Int }
来源：http://en.nszjky.cn

[T26] Swift：类与重写
来源：http://oh.chemitech.net.cn

class A: Base { override func f() {} }
来源：http://rs.panjiajie.cn

[T27] Swift：错误处理
来源：http://il.wgjwhj.cn

do { try f() } catch { print(error) }
来源：http://rp.newstarts.cn

[T28] Swift：枚举
来源：http://zh.bookmarksfly.cn

enum Color { case red, green }
来源：http://im.nszjky.cn

[T29] Swift：guard 提前返回
来源：http://gs.wgjwhj.cn

guard let x = opt else { return }
来源：http://dp.wgjwhj.cn

[T30] Swift：协议
来源：http://vt.bookmarksfly.cn

protocol Shape { func area() -> Double }
来源：http://nl.shtwfgs.cn

[T31] Lua：Hello World
来源：http://mf.szsharing.cn

print("Hello")
来源：http://kc.yuntaijiaju.cn

[T32] Lua：局部变量
来源：http://sv.lnxyls.cn

local a = 1
来源：http://zb.haigaiapp.cn

[T33] Lua：表（数组）
来源：http://ek.bookmarksfly.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fh.nicolike.cn

[T34] Lua：遍历表
来源：http://cc.szxytkj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qy.jianghongdianzi.cn

[T35] Lua：字典表
来源：http://tw.muxihuayi.cn

local d = { a = 1 };  d.b = 2
来源：http://ll.huixinmuqiang.cn

[T36] Lua：函数
来源：http://qh.shxzskj.cn

function add(a, b) return a + b end
来源：http://yn.szsharing.cn

[T37] Lua：字符串拼接
来源：http://bt.colortex.cn

"a" .. "b"
来源：http://is.panjiajie.cn

[T38] Lua：条件
来源：http://ii.9csxet.cn

if x > 0 then print("正") end
来源：http://qt.hahajie.cn

[T39] Lua：模式匹配
来源：http://qs.haigaiapp.cn

string.find(s, "%d+")
来源：http://rg.asd995.cn

[T40] Lua：元表
来源：http://mp.hnjuh.cn

setmetatable({}, { __index = base })
来源：http://vd.yuntaijiaju.cn

[T41] Perl：Hello World
来源：http://fe.wgjwhj.cn

print "Hello\n";
来源：http://nb.szxytkj.cn

[T42] Perl：变量类型
来源：http://qz.szsharing.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wu.gzmigu.cn

[T43] Perl：字符串插值
来源：http://eq.yuntaijiaju.cn

"值: $a"
来源：http://ls.521024.cn

[T44] Perl：条件
来源：http://eo.hnjuh.cn

if ($a > 0) { print "正"; }
来源：http://lb.szsharing.cn

[T45] Perl：数组遍历
来源：http://qw.hahajie.cn

for my $x (@arr) { print $x; }
来源：http://al.nicolike.cn

[T46] Perl：哈希操作
来源：http://rw.nicolike.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://aq.haigaiapp.cn

[T47] Perl：正则捕获
来源：http://zs.huanxung.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ml.gzmigu.cn

[T48] Perl：正则替换
来源：http://dz.yuntaijiaju.cn

$s =~ s/old/new/g;
来源：http://ck.shxzukj.cn

[T49] Perl：函数
来源：http://qz.jctech888.com.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ay.chemitech.net.cn

[T50] Perl：逐行读文件
来源：http://ph.yuexingan06.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://px.shxzukj.cn

while (my $line = <$fh>) { print $line; }
来源：http://cl.huanxung.cn

[T51] Scala：Hello World
来源：http://hn.jctech888.com.cn

println("Hello")
来源：http://le.jctech888.com.cn

[T52] Scala：变量
来源：http://ch.yuntaijiaju.cn

val a = 1;  var b = 2
来源：http://rp.gzmigu.cn

[T53] Scala：字符串插值
来源：http://ef.521024.cn

s"值: $b"
来源：http://vd.huanxung.cn

[T54] Scala：集合映射
来源：http://tt.huixiangedu.cn

List(1, 2, 3).map(_ * 2)
来源：http://ic.yuntaijiaju.cn

[T55] Scala：集合过滤
来源：http://jm.huixinmuqiang.cn

List(1, 2, 3).filter(_ > 1)
来源：http://kz.hahajie.cn

[T56] Scala：样例类
来源：http://xh.hahajie.cn

case class User(name: String, age: Int)
来源：http://sq.chemitech.net.cn

[T57] Scala：模式匹配
来源：http://ve.nicolike.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ux.haigaiapp.cn

[T58] Scala：函数定义
来源：http://ui.panjiajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ne.chemitech.net.cn

[T59] Scala：循环
来源：http://xn.szxytkj.cn

for (i <- 1 to 10) println(i)
来源：http://sk.521024.cn

[T60] Scala：折叠
来源：http://yl.huanxung.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://io.nicolike.cn

================================================================================
来源：http://ej.9csxet.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lf.muxihuayi.cn

================================================================================
来源：http://zp.jianghongdianzi.cn

[U01] Py：创建虚拟环境
来源：http://kn.huanxung.cn

python -m venv .venv && source .venv/bin/activate
来源：http://rf.521024.cn

[U02] Py：导出 / 安装依赖
来源：http://qr.wgjwhj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yj.haigaiapp.cn

[U03] Py：加载 .env 配置
来源：http://pm.jianghongdianzi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gv.yuntaijiaju.cn

[U04] Py：变量调试打印
来源：http://ie.9csxet.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ij.wgjwhj.cn

[U05] Py：列表去重且保序
来源：http://ev.bookmarksfly.cn

list(dict.fromkeys(arr))
来源：http://mg.huixinmuqiang.cn

[U06] Py：合并两个字典
来源：http://yv.newstarts.cn

{**a, **b}
来源：http://wo.huixinmuqiang.cn

[U07] Py：反转字典键值
来源：http://id.yuntaijiaju.cn

{v: k for k, v in d.items()}
来源：http://zb.yuntaijiaju.cn

[U08] Py：展平二维列表
来源：http://fa.nicolike.cn

[y for x in nested for y in x]
来源：http://jt.panjiajie.cn

[U09] Py：字典取最大值的键
来源：http://wq.huanxung.cn

max(d, key=d.get)
来源：http://lw.huixinmuqiang.cn

[U10] Py：按值排序字典
来源：http://jj.hnjuh.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cf.bjjhwx.cn

[U11] Py：生成器表达式
来源：http://zz.haigaiapp.cn

(x * 2 for x in arr)
来源：http://ih.yuexingan06.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rv.wgjwhj.cn

Counter(arr).most_common(3)
来源：http://os.hnjuh.cn

[U13] Py：固定长度队列
来源：http://ar.nszjky.cn

deque(maxlen=10)
来源：http://rb.huixinmuqiang.cn

[U14] Py：分组收集到列表
来源：http://gl.shxzukj.cn

defaultdict(list)
来源：http://lm.huixiangedu.cn

[U15] Py：高精度计时
来源：http://ne.bookmarksfly.cn

t = time.perf_counter()
来源：http://hh.chemitech.net.cn

[U16] Py：命令行参数解析
来源：http://sh.521024.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vi.521024.cn

[U17] Py：初始化日志
来源：http://yo.huanxung.cn

logging.basicConfig(level=logging.INFO)
来源：http://xj.yuntaijiaju.cn

[U18] Py：预编译正则
来源：http://rs.shtwfgs.cn

pat = re.compile(r"\d+")
来源：http://gf.9csxet.cn

[U19] Py：正则替换带回调
来源：http://tg.jctech888.com.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rp.chemitech.net.cn

[U20] Py：缓存函数结果
来源：http://ya.haigaiapp.cn

@functools.lru_cache(maxsize=None)
来源：http://kk.chemitech.net.cn

[U21] Py：自定义上下文管理器
来源：http://it.huanxung.cn

@contextlib.contextmanager
来源：http://zd.huanxung.cn

[U22] Py：矩阵转置
来源：http://zy.gzmigu.cn

list(zip(*m))
来源：http://xk.9csxet.cn

[U23] Py：分块读取大文件
来源：http://gb.bjjhwx.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pk.huixinmuqiang.cn

[U24] Py：路径操作
来源：http://bf.yuexingan06.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://sy.asd995.cn

[U25] Py：CSV 按字典读
来源：http://xj.gzmigu.cn

csv.DictReader(f)
来源：http://xu.jctech888.com.cn

[U26] Py：并发下载
来源：http://li.nszjky.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gv.newstarts.cn

[U27] Py：异步 HTTP
来源：http://kf.9csxet.cn

aiohttp.ClientSession() 配合 async with
来源：http://zw.shtwfgs.cn

[U28] Py：类型别名
来源：http://rd.gzmigu.cn

UserId = int
来源：http://mk.gzmigu.cn

[U29] Py：属性校验
来源：http://wc.9csxet.cn

@property 与 @x.setter 配合
来源：http://vu.huanxung.cn

[U30] Py：数据类
来源：http://is.hnjuh.cn

@dataclass(slots=True)
来源：http://zf.huixiangedu.cn

[U31] Py：单测
来源：http://he.521024.cn

python -m pytest -q
来源：http://de.shxzskj.cn

[U32] Py：代码格式化
来源：http://em.yuntaijiaju.cn

ruff format . && ruff check --fix .
来源：http://jn.huixiangedu.cn


<!-- 参考信息 -->