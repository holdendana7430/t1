代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bh.colortex.cn

[S10] C：指针与解引用
来源：http://iu.wgjwhj.cn

int *p = &a;  *p = 5;
来源：http://rx.colortex.cn

[S11] C：逐行读文件
来源：http://pt.szxytkj.cn

FILE *f = fopen("a.txt", "r");
来源：http://ey.lnxyls.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qg.huixiangedu.cn

fclose(f);
来源：http://ic.colortex.cn

[S12] C：写文件
来源：http://gw.shtwfgs.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ss.shtwfgs.cn

[S13] C：宏定义
来源：http://qu.yuexingan06.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ru.hnjuh.cn

[S14] C：枚举
来源：http://qe.shxzskj.cn

enum Color { RED, GREEN, BLUE };
来源：http://af.nicolike.cn

[S15] C：类型转换
来源：http://xd.shtwfgs.cn

(double) a / b
来源：http://zr.yuexingan06.cn

[S16] C：位操作置位
来源：http://lc.muxihuayi.cn

x |= (1 << 3);
来源：http://cg.szxytkj.cn

[S17] C：安全拼接字符串
来源：http://vl.asd995.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zk.muxihuayi.cn

[S18] C：命令行参数
来源：http://az.panjiajie.cn

int main(int argc, char **argv)
来源：http://be.muxihuayi.cn

[S19] C：快速排序
来源：http://rd.9csxet.cn

qsort(a, n, sizeof(int), cmp);
来源：http://uq.colortex.cn

[S20] C：二分查找
来源：http://kc.wgjwhj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rz.panjiajie.cn

[S21] C：字符类别判断
来源：http://yr.muxihuayi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zf.yuntaijiaju.cn

[S22] C：字符串转数字
来源：http://ys.9csxet.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wg.yuexingan06.cn

[S23] C：随机数
来源：http://sq.jctech888.com.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wa.521024.cn

[S24] C：获取本地时间
来源：http://dx.colortex.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pz.nicolike.cn

[S25] C：内存拷贝
来源：http://pt.shxzskj.cn

memcpy(dst, src, n);
来源：http://hq.panjiajie.cn

[S26] C：内存清零
来源：http://sm.haigaiapp.cn

memset(a, 0, sizeof a);
来源：http://rn.huixinmuqiang.cn

[S27] C：定义常量
来源：http://tk.szxytkj.cn

const double PI = 3.14159;
来源：http://xv.szxytkj.cn

[S28] C：静态变量
来源：http://da.9csxet.cn

static int counter = 0;
来源：http://mr.huixinmuqiang.cn

[S29] C：变参函数
来源：http://qg.yuntaijiaju.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dy.haigaiapp.cn

[S30] C：头文件保护
来源：http://xv.huixinmuqiang.cn

#ifndef X_H
来源：http://zy.panjiajie.cn

#define X_H
来源：http://zi.shxzukj.cn

#endif
来源：http://rg.bjjhwx.cn

[S31] C++：Hello World
来源：http://gq.lnxyls.cn

#include <iostream>
来源：http://cg.newstarts.cn

int main() { std::cout << "Hello\n"; }
来源：http://en.hnjuh.cn

[S32] C++：字符串
来源：http://vw.asd995.cn

std::string s = "hi";  s += "!";
来源：http://un.yuexingan06.cn

[S33] C++：vector 增删
来源：http://ab.bookmarksfly.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zu.shxzskj.cn

[S34] C++：遍历 vector
来源：http://xe.shxzukj.cn

for (auto &x : v) { std::cout << x; }
来源：http://au.panjiajie.cn

[S35] C++：map
来源：http://bk.bjjhwx.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jd.hahajie.cn

[S36] C++：unordered_map
来源：http://gq.haigaiapp.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cx.lnxyls.cn

[S37] C++：set
来源：http://ae.huixinmuqiang.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hw.shxzskj.cn

[S38] C++：排序
来源：http://lj.huixiangedu.cn

std::sort(v.begin(), v.end());
来源：http://hr.9csxet.cn

[S39] C++：自定义比较器排序
来源：http://lg.bookmarksfly.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://aq.shxzukj.cn

[S40] C++：查找元素
来源：http://fb.hahajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://um.jianghongdianzi.cn

[S41] C++：类与构造函数
来源：http://vy.shxzukj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dc.muxihuayi.cn

[S42] C++：继承与虚函数
来源：http://kk.haigaiapp.cn

class B : public Base { public: void f() override {} };
来源：http://lj.shxzskj.cn

[S43] C++：智能指针
来源：http://rn.wgjwhj.cn

auto p = std::make_unique<int>(5);
来源：http://uw.chemitech.net.cn

[S44] C++：引用传参
来源：http://ol.jctech888.com.cn

void inc(int &x) { ++x; }
来源：http://sp.shtwfgs.cn

[S45] C++：lambda
来源：http://ws.hnjuh.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wv.9csxet.cn

[S46] C++：函数模板
来源：http://rn.haigaiapp.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ty.jianghongdianzi.cn

[S47] C++：结构化绑定遍历
来源：http://ii.shtwfgs.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wn.jianghongdianzi.cn

[S48] C++：逐行读文件
来源：http://aw.shxzskj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://uz.yuntaijiaju.cn

while (std::getline(in, line)) { }
来源：http://im.bjjhwx.cn

[S49] C++：写文件
来源：http://uq.asd995.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dr.yuexingan06.cn

[S50] C++：格式化数字
来源：http://lk.shxzskj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fc.huixinmuqiang.cn

[S51] C++：显式类型转换
来源：http://lw.wgjwhj.cn

static_cast<double>(a) / b
来源：http://pr.9csxet.cn

[S52] C++：const 与 noexcept
来源：http://za.yuntaijiaju.cn

int size() const noexcept { return n_; }
来源：http://uo.9csxet.cn

[S53] C++：移动语义
来源：http://ot.jianghongdianzi.cn

std::vector<int> w = std::move(v);
来源：http://jy.chemitech.net.cn

[S54] C++：异常处理
来源：http://hd.hahajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://az.shxzskj.cn

[S55] C++：结构化绑定
来源：http://ei.yuntaijiaju.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ln.colortex.cn

[S56] C++：optional
来源：http://pd.shxzskj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qn.chemitech.net.cn

[S57] C++：编译期常量
来源：http://vg.gzmigu.cn

constexpr int N = 10;
来源：http://rg.muxihuayi.cn

[S58] C++：命名空间
来源：http://xg.hnjuh.cn

namespace ns { int f() { return 1; } }
来源：http://ne.szxytkj.cn

[S59] C++：静态断言
来源：http://wi.chemitech.net.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zp.nszjky.cn

[S60] C++：遍历并删除元素
来源：http://gu.newstarts.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://it.huanxung.cn

================================================================================
来源：http://tm.521024.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://je.muxihuayi.cn

================================================================================
来源：http://jg.haigaiapp.cn

[T01] Kotlin：Hello World
来源：http://kk.hahajie.cn

println("Hello")
来源：http://hj.yuntaijiaju.cn

[T02] Kotlin：变量
来源：http://aw.521024.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cm.colortex.cn

[T03] Kotlin：字符串模板
来源：http://lc.colortex.cn

"值: $b"
来源：http://cc.haigaiapp.cn

[T04] Kotlin：空安全
来源：http://ed.nszjky.cn

val n: String? = null;  n?.length
来源：http://xj.huixinmuqiang.cn

[T05] Kotlin：when 表达式
来源：http://ob.szxytkj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dl.szsharing.cn

[T06] Kotlin：集合映射
来源：http://bj.asd995.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rx.hahajie.cn

[T07] Kotlin：集合过滤
来源：http://hc.yuexingan06.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://mi.shxzskj.cn

[T08] Kotlin：数据类
来源：http://uz.yuntaijiaju.cn

data class User(val name: String, val age: Int)
来源：http://ez.shxzukj.cn

[T09] Kotlin：扩展函数
来源：http://fg.yuexingan06.cn

fun String.exclaim() = this + "!"
来源：http://ue.szsharing.cn

[T10] Kotlin：默认参数
来源：http://jj.lnxyls.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ic.bookmarksfly.cn

[T11] Kotlin：协程
来源：http://yf.newstarts.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://lm.bjjhwx.cn

[T12] Kotlin：解构声明
来源：http://st.shxzskj.cn

val (a, b) = Pair(1, 2)
来源：http://nh.shxzukj.cn

[T13] Kotlin：只读 Map
来源：http://sz.shxzukj.cn

val m = mapOf("a" to 1)
来源：http://ar.9csxet.cn

[T14] Kotlin：循环
来源：http://ul.shxzskj.cn

for (i in 1..10) println(i)
来源：http://no.panjiajie.cn

[T15] Kotlin：接口
来源：http://mc.szsharing.cn

interface Shape { fun area(): Double }
来源：http://zg.wgjwhj.cn

[T16] Swift：Hello World
来源：http://mt.nicolike.cn

print("Hello")
来源：http://kt.huixinmuqiang.cn

[T17] Swift：变量与常量
来源：http://ic.shtwfgs.cn

var a = 1;  let b = 2
来源：http://vo.bjjhwx.cn

[T18] Swift：字符串插值
来源：http://ga.nicolike.cn

"值: \(b)"
来源：http://vo.9csxet.cn

[T19] Swift：可选绑定
来源：http://tz.haigaiapp.cn

if let n = opt { print(n) }
来源：http://ps.shxzukj.cn

[T20] Swift：数组操作
来源：http://pb.colortex.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gn.9csxet.cn

[T21] Swift：遍历
来源：http://zf.gzmigu.cn

for x in a { print(x) }
来源：http://xl.bjjhwx.cn

[T22] Swift：字典
来源：http://kx.newstarts.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ef.huixiangedu.cn

[T23] Swift：函数
来源：http://xw.wgjwhj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://su.bookmarksfly.cn

[T24] Swift：闭包
来源：http://fj.shxzskj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ic.hnjuh.cn

[T25] Swift：结构体
来源：http://rc.bookmarksfly.cn

struct P { var x: Int }
来源：http://tf.panjiajie.cn

[T26] Swift：类与重写
来源：http://hp.muxihuayi.cn

class A: Base { override func f() {} }
来源：http://sa.chemitech.net.cn

[T27] Swift：错误处理
来源：http://vt.bjjhwx.cn

do { try f() } catch { print(error) }
来源：http://jh.panjiajie.cn

[T28] Swift：枚举
来源：http://dw.newstarts.cn

enum Color { case red, green }
来源：http://nr.yuntaijiaju.cn

[T29] Swift：guard 提前返回
来源：http://th.bjjhwx.cn

guard let x = opt else { return }
来源：http://um.yuexingan06.cn

[T30] Swift：协议
来源：http://tt.521024.cn

protocol Shape { func area() -> Double }
来源：http://vi.bookmarksfly.cn

[T31] Lua：Hello World
来源：http://to.521024.cn

print("Hello")
来源：http://sd.gzmigu.cn

[T32] Lua：局部变量
来源：http://ah.gzmigu.cn

local a = 1
来源：http://eq.yuexingan06.cn

[T33] Lua：表（数组）
来源：http://wi.shxzskj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xc.shxzukj.cn

[T34] Lua：遍历表
来源：http://va.shxzukj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ri.hahajie.cn

[T35] Lua：字典表
来源：http://xw.nicolike.cn

local d = { a = 1 };  d.b = 2
来源：http://oa.haigaiapp.cn

[T36] Lua：函数
来源：http://hf.newstarts.cn

function add(a, b) return a + b end
来源：http://vv.jctech888.com.cn

[T37] Lua：字符串拼接
来源：http://rk.wgjwhj.cn

"a" .. "b"
来源：http://vr.huanxung.cn

[T38] Lua：条件
来源：http://av.huixinmuqiang.cn

if x > 0 then print("正") end
来源：http://ih.9csxet.cn

[T39] Lua：模式匹配
来源：http://wl.hahajie.cn

string.find(s, "%d+")
来源：http://yk.shtwfgs.cn

[T40] Lua：元表
来源：http://vb.jianghongdianzi.cn

setmetatable({}, { __index = base })
来源：http://zc.haigaiapp.cn

[T41] Perl：Hello World
来源：http://ec.jctech888.com.cn

print "Hello\n";
来源：http://ph.asd995.cn

[T42] Perl：变量类型
来源：http://bm.huanxung.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fj.wgjwhj.cn

[T43] Perl：字符串插值
来源：http://pm.521024.cn

"值: $a"
来源：http://fb.huixinmuqiang.cn

[T44] Perl：条件
来源：http://cl.nicolike.cn

if ($a > 0) { print "正"; }
来源：http://ku.jianghongdianzi.cn

[T45] Perl：数组遍历
来源：http://ah.nszjky.cn

for my $x (@arr) { print $x; }
来源：http://uu.gzmigu.cn

[T46] Perl：哈希操作
来源：http://fk.huanxung.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rq.bookmarksfly.cn

[T47] Perl：正则捕获
来源：http://oj.huanxung.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://we.nicolike.cn

[T48] Perl：正则替换
来源：http://og.muxihuayi.cn

$s =~ s/old/new/g;
来源：http://mb.huanxung.cn

[T49] Perl：函数
来源：http://uc.yuntaijiaju.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://oe.chemitech.net.cn

[T50] Perl：逐行读文件
来源：http://sj.chemitech.net.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qi.chemitech.net.cn

while (my $line = <$fh>) { print $line; }
来源：http://lm.bjjhwx.cn

[T51] Scala：Hello World
来源：http://ql.huanxung.cn

println("Hello")
来源：http://op.521024.cn

[T52] Scala：变量
来源：http://cx.wgjwhj.cn

val a = 1;  var b = 2
来源：http://bk.colortex.cn

[T53] Scala：字符串插值
来源：http://qx.jianghongdianzi.cn

s"值: $b"
来源：http://zz.newstarts.cn

[T54] Scala：集合映射
来源：http://oo.szsharing.cn

List(1, 2, 3).map(_ * 2)
来源：http://xl.huanxung.cn

[T55] Scala：集合过滤
来源：http://ao.9csxet.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ck.9csxet.cn

[T56] Scala：样例类
来源：http://xo.yuntaijiaju.cn

case class User(name: String, age: Int)
来源：http://cy.szsharing.cn

[T57] Scala：模式匹配
来源：http://pm.gzmigu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://aa.bjjhwx.cn

[T58] Scala：函数定义
来源：http://hh.shxzskj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gl.gzmigu.cn

[T59] Scala：循环
来源：http://og.newstarts.cn

for (i <- 1 to 10) println(i)
来源：http://ev.szxytkj.cn

[T60] Scala：折叠
来源：http://xe.wgjwhj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qv.huixinmuqiang.cn

================================================================================
来源：http://dh.shtwfgs.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bq.521024.cn

================================================================================
来源：http://ka.lnxyls.cn

[U01] Py：创建虚拟环境
来源：http://td.jctech888.com.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mw.colortex.cn

[U02] Py：导出 / 安装依赖
来源：http://ui.shxzukj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://iz.yuntaijiaju.cn

[U03] Py：加载 .env 配置
来源：http://kx.szsharing.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://hb.szxytkj.cn

[U04] Py：变量调试打印
来源：http://ie.chemitech.net.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jo.huixiangedu.cn

[U05] Py：列表去重且保序
来源：http://oz.huixiangedu.cn

list(dict.fromkeys(arr))
来源：http://ae.bookmarksfly.cn

[U06] Py：合并两个字典
来源：http://ci.huanxung.cn

{**a, **b}
来源：http://xw.yuntaijiaju.cn

[U07] Py：反转字典键值
来源：http://nj.jctech888.com.cn

{v: k for k, v in d.items()}
来源：http://gs.bjjhwx.cn

[U08] Py：展平二维列表
来源：http://ok.9csxet.cn

[y for x in nested for y in x]
来源：http://kf.haigaiapp.cn

[U09] Py：字典取最大值的键
来源：http://sk.shxzukj.cn

max(d, key=d.get)
来源：http://np.colortex.cn

[U10] Py：按值排序字典
来源：http://wh.asd995.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ao.hnjuh.cn

[U11] Py：生成器表达式
来源：http://rb.hnjuh.cn

(x * 2 for x in arr)
来源：http://zh.chemitech.net.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rs.bookmarksfly.cn

Counter(arr).most_common(3)
来源：http://pw.bookmarksfly.cn

[U13] Py：固定长度队列
来源：http://zs.shxzukj.cn

deque(maxlen=10)
来源：http://mg.shtwfgs.cn

[U14] Py：分组收集到列表
来源：http://hx.asd995.cn

defaultdict(list)
来源：http://ku.521024.cn

[U15] Py：高精度计时
来源：http://jc.huanxung.cn

t = time.perf_counter()
来源：http://gx.shxzukj.cn

[U16] Py：命令行参数解析
来源：http://yr.jianghongdianzi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zz.colortex.cn

[U17] Py：初始化日志
来源：http://mu.yuexingan06.cn

logging.basicConfig(level=logging.INFO)
来源：http://fv.muxihuayi.cn

[U18] Py：预编译正则
来源：http://jx.hnjuh.cn

pat = re.compile(r"\d+")
来源：http://dr.bjjhwx.cn

[U19] Py：正则替换带回调
来源：http://tb.asd995.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yr.yuntaijiaju.cn

[U20] Py：缓存函数结果
来源：http://vo.bookmarksfly.cn

@functools.lru_cache(maxsize=None)
来源：http://rv.nszjky.cn

[U21] Py：自定义上下文管理器
来源：http://rv.shxzukj.cn

@contextlib.contextmanager
来源：http://ds.newstarts.cn

[U22] Py：矩阵转置
来源：http://vb.huanxung.cn

list(zip(*m))
来源：http://iz.wgjwhj.cn

[U23] Py：分块读取大文件
来源：http://ug.nicolike.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bz.nszjky.cn

[U24] Py：路径操作
来源：http://mr.yuntaijiaju.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://od.szsharing.cn

[U25] Py：CSV 按字典读
来源：http://qz.wgjwhj.cn

csv.DictReader(f)
来源：http://um.bookmarksfly.cn

[U26] Py：并发下载
来源：http://ue.haigaiapp.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://si.lnxyls.cn

[U27] Py：异步 HTTP
来源：http://oi.nicolike.cn

aiohttp.ClientSession() 配合 async with
来源：http://qj.gzmigu.cn

[U28] Py：类型别名
来源：http://fr.9csxet.cn

UserId = int
来源：http://tl.huixinmuqiang.cn

[U29] Py：属性校验
来源：http://xr.jctech888.com.cn

@property 与 @x.setter 配合
来源：http://vu.huixiangedu.cn

[U30] Py：数据类
来源：http://uj.hahajie.cn

@dataclass(slots=True)
来源：http://lr.muxihuayi.cn

[U31] Py：单测
来源：http://si.shxzukj.cn

python -m pytest -q
来源：http://lf.nicolike.cn

[U32] Py：代码格式化
来源：http://ve.hahajie.cn

ruff format . && ruff check --fix .
来源：http://qv.wgjwhj.cn


<!-- 参考信息 -->