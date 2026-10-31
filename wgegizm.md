代发 wailian999

strlen(s)
来源：http://ux.gzmigu.cn

[S06] C：字符串比较
来源：http://hu.huixinmuqiang.cn

strcmp(a, b) == 0
来源：http://pn.colortex.cn

[S07] C：数组遍历求和
来源：http://sm.nicolike.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zy.jctech888.com.cn

[S08] C：动态内存分配与释放
来源：http://ha.nszjky.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jm.lnxyls.cn

[S09] C：结构体定义与初始化
来源：http://rm.hahajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gn.bookmarksfly.cn

[S10] C：指针与解引用
来源：http://io.gzmigu.cn

int *p = &a;  *p = 5;
来源：http://ng.chemitech.net.cn

[S11] C：逐行读文件
来源：http://db.yuntaijiaju.cn

FILE *f = fopen("a.txt", "r");
来源：http://xi.colortex.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ms.nicolike.cn

fclose(f);
来源：http://sl.shxzskj.cn

[S12] C：写文件
来源：http://si.huanxung.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gy.hahajie.cn

[S13] C：宏定义
来源：http://rh.chemitech.net.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dn.bookmarksfly.cn

[S14] C：枚举
来源：http://lr.szsharing.cn

enum Color { RED, GREEN, BLUE };
来源：http://cm.huanxung.cn

[S15] C：类型转换
来源：http://td.gzmigu.cn

(double) a / b
来源：http://dv.huixinmuqiang.cn

[S16] C：位操作置位
来源：http://ea.yuexingan06.cn

x |= (1 << 3);
来源：http://kg.haigaiapp.cn

[S17] C：安全拼接字符串
来源：http://mk.muxihuayi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://at.asd995.cn

[S18] C：命令行参数
来源：http://ez.yuexingan06.cn

int main(int argc, char **argv)
来源：http://ht.shtwfgs.cn

[S19] C：快速排序
来源：http://ha.huanxung.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jg.asd995.cn

[S20] C：二分查找
来源：http://dz.gzmigu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xe.szxytkj.cn

[S21] C：字符类别判断
来源：http://gj.huanxung.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bm.yuexingan06.cn

[S22] C：字符串转数字
来源：http://qa.bookmarksfly.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vm.nszjky.cn

[S23] C：随机数
来源：http://xv.muxihuayi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pu.lnxyls.cn

[S24] C：获取本地时间
来源：http://ni.chemitech.net.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zt.colortex.cn

[S25] C：内存拷贝
来源：http://rt.hahajie.cn

memcpy(dst, src, n);
来源：http://ue.haigaiapp.cn

[S26] C：内存清零
来源：http://be.muxihuayi.cn

memset(a, 0, sizeof a);
来源：http://no.szsharing.cn

[S27] C：定义常量
来源：http://yk.haigaiapp.cn

const double PI = 3.14159;
来源：http://ur.bjjhwx.cn

[S28] C：静态变量
来源：http://ye.chemitech.net.cn

static int counter = 0;
来源：http://dc.shxzukj.cn

[S29] C：变参函数
来源：http://se.muxihuayi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ou.szsharing.cn

[S30] C：头文件保护
来源：http://ov.wgjwhj.cn

#ifndef X_H
来源：http://eb.newstarts.cn

#define X_H
来源：http://qr.hnjuh.cn

#endif
来源：http://nc.lnxyls.cn

[S31] C++：Hello World
来源：http://mf.haigaiapp.cn

#include <iostream>
来源：http://ug.lnxyls.cn

int main() { std::cout << "Hello\n"; }
来源：http://bd.yuexingan06.cn

[S32] C++：字符串
来源：http://fd.jctech888.com.cn

std::string s = "hi";  s += "!";
来源：http://oo.521024.cn

[S33] C++：vector 增删
来源：http://mv.shtwfgs.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qt.gzmigu.cn

[S34] C++：遍历 vector
来源：http://ds.huixiangedu.cn

for (auto &x : v) { std::cout << x; }
来源：http://ak.jctech888.com.cn

[S35] C++：map
来源：http://fa.hahajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fd.521024.cn

[S36] C++：unordered_map
来源：http://cv.huanxung.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xg.muxihuayi.cn

[S37] C++：set
来源：http://vs.muxihuayi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://so.huixiangedu.cn

[S38] C++：排序
来源：http://dl.szxytkj.cn

std::sort(v.begin(), v.end());
来源：http://ai.shxzskj.cn

[S39] C++：自定义比较器排序
来源：http://wl.lnxyls.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://iq.yuexingan06.cn

[S40] C++：查找元素
来源：http://am.chemitech.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://it.chemitech.net.cn

[S41] C++：类与构造函数
来源：http://vt.bookmarksfly.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wc.haigaiapp.cn

[S42] C++：继承与虚函数
来源：http://nv.colortex.cn

class B : public Base { public: void f() override {} };
来源：http://da.huixiangedu.cn

[S43] C++：智能指针
来源：http://rl.shxzukj.cn

auto p = std::make_unique<int>(5);
来源：http://zm.huanxung.cn

[S44] C++：引用传参
来源：http://mp.huixiangedu.cn

void inc(int &x) { ++x; }
来源：http://pl.nszjky.cn

[S45] C++：lambda
来源：http://pd.hnjuh.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ag.wgjwhj.cn

[S46] C++：函数模板
来源：http://iw.hahajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yn.jianghongdianzi.cn

[S47] C++：结构化绑定遍历
来源：http://wj.jctech888.com.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gq.nicolike.cn

[S48] C++：逐行读文件
来源：http://uu.yuntaijiaju.cn

std::ifstream in("a.txt");  std::string line;
来源：http://yi.hahajie.cn

while (std::getline(in, line)) { }
来源：http://wx.521024.cn

[S49] C++：写文件
来源：http://yj.bjjhwx.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://za.jctech888.com.cn

[S50] C++：格式化数字
来源：http://ci.newstarts.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qr.nicolike.cn

[S51] C++：显式类型转换
来源：http://qd.szxytkj.cn

static_cast<double>(a) / b
来源：http://zw.shxzukj.cn

[S52] C++：const 与 noexcept
来源：http://rz.gzmigu.cn

int size() const noexcept { return n_; }
来源：http://ug.jianghongdianzi.cn

[S53] C++：移动语义
来源：http://cq.yuexingan06.cn

std::vector<int> w = std::move(v);
来源：http://bs.szsharing.cn

[S54] C++：异常处理
来源：http://cg.lnxyls.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xs.521024.cn

[S55] C++：结构化绑定
来源：http://ub.lnxyls.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ro.chemitech.net.cn

[S56] C++：optional
来源：http://ng.asd995.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ee.shtwfgs.cn

[S57] C++：编译期常量
来源：http://of.muxihuayi.cn

constexpr int N = 10;
来源：http://bo.huixiangedu.cn

[S58] C++：命名空间
来源：http://nq.muxihuayi.cn

namespace ns { int f() { return 1; } }
来源：http://yx.szxytkj.cn

[S59] C++：静态断言
来源：http://sw.chemitech.net.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qp.haigaiapp.cn

[S60] C++：遍历并删除元素
来源：http://nk.shxzskj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fl.gzmigu.cn

================================================================================
来源：http://rd.muxihuayi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hv.jctech888.com.cn

================================================================================
来源：http://sn.panjiajie.cn

[T01] Kotlin：Hello World
来源：http://xx.huanxung.cn

println("Hello")
来源：http://ue.nicolike.cn

[T02] Kotlin：变量
来源：http://jx.jianghongdianzi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hx.shxzskj.cn

[T03] Kotlin：字符串模板
来源：http://wd.szxytkj.cn

"值: $b"
来源：http://oo.521024.cn

[T04] Kotlin：空安全
来源：http://ye.huixinmuqiang.cn

val n: String? = null;  n?.length
来源：http://ck.yuntaijiaju.cn

[T05] Kotlin：when 表达式
来源：http://bb.huanxung.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fx.wgjwhj.cn

[T06] Kotlin：集合映射
来源：http://dv.yuntaijiaju.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xg.newstarts.cn

[T07] Kotlin：集合过滤
来源：http://ww.huanxung.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pg.wgjwhj.cn

[T08] Kotlin：数据类
来源：http://ur.nszjky.cn

data class User(val name: String, val age: Int)
来源：http://aw.nicolike.cn

[T09] Kotlin：扩展函数
来源：http://gq.hnjuh.cn

fun String.exclaim() = this + "!"
来源：http://qu.yuexingan06.cn

[T10] Kotlin：默认参数
来源：http://eb.jianghongdianzi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://sq.9csxet.cn

[T11] Kotlin：协程
来源：http://vd.jctech888.com.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ah.jianghongdianzi.cn

[T12] Kotlin：解构声明
来源：http://qg.huanxung.cn

val (a, b) = Pair(1, 2)
来源：http://la.shtwfgs.cn

[T13] Kotlin：只读 Map
来源：http://dz.muxihuayi.cn

val m = mapOf("a" to 1)
来源：http://xr.9csxet.cn

[T14] Kotlin：循环
来源：http://ey.huixinmuqiang.cn

for (i in 1..10) println(i)
来源：http://jt.nszjky.cn

[T15] Kotlin：接口
来源：http://fy.jctech888.com.cn

interface Shape { fun area(): Double }
来源：http://px.shxzukj.cn

[T16] Swift：Hello World
来源：http://ht.wgjwhj.cn

print("Hello")
来源：http://mc.521024.cn

[T17] Swift：变量与常量
来源：http://dv.yuntaijiaju.cn

var a = 1;  let b = 2
来源：http://fm.nszjky.cn

[T18] Swift：字符串插值
来源：http://bt.szxytkj.cn

"值: \(b)"
来源：http://ah.wgjwhj.cn

[T19] Swift：可选绑定
来源：http://zy.szxytkj.cn

if let n = opt { print(n) }
来源：http://zz.huanxung.cn

[T20] Swift：数组操作
来源：http://az.bjjhwx.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hg.bjjhwx.cn

[T21] Swift：遍历
来源：http://vn.haigaiapp.cn

for x in a { print(x) }
来源：http://od.szxytkj.cn

[T22] Swift：字典
来源：http://ap.yuntaijiaju.cn

var d = ["a": 1];  d["b"] = 2
来源：http://hj.gzmigu.cn

[T23] Swift：函数
来源：http://vc.shxzskj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mh.wgjwhj.cn

[T24] Swift：闭包
来源：http://fr.bookmarksfly.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xp.huixiangedu.cn

[T25] Swift：结构体
来源：http://to.szsharing.cn

struct P { var x: Int }
来源：http://cb.colortex.cn

[T26] Swift：类与重写
来源：http://tf.521024.cn

class A: Base { override func f() {} }
来源：http://xt.wgjwhj.cn

[T27] Swift：错误处理
来源：http://je.lnxyls.cn

do { try f() } catch { print(error) }
来源：http://gk.szxytkj.cn

[T28] Swift：枚举
来源：http://st.shxzukj.cn

enum Color { case red, green }
来源：http://ar.wgjwhj.cn

[T29] Swift：guard 提前返回
来源：http://pi.yuexingan06.cn

guard let x = opt else { return }
来源：http://wx.szsharing.cn

[T30] Swift：协议
来源：http://ni.hnjuh.cn

protocol Shape { func area() -> Double }
来源：http://ox.panjiajie.cn

[T31] Lua：Hello World
来源：http://tp.chemitech.net.cn

print("Hello")
来源：http://tx.szsharing.cn

[T32] Lua：局部变量
来源：http://xt.huanxung.cn

local a = 1
来源：http://cq.nicolike.cn

[T33] Lua：表（数组）
来源：http://gc.haigaiapp.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://sf.huixinmuqiang.cn

[T34] Lua：遍历表
来源：http://py.bjjhwx.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://sy.hahajie.cn

[T35] Lua：字典表
来源：http://pi.yuexingan06.cn

local d = { a = 1 };  d.b = 2
来源：http://lq.gzmigu.cn

[T36] Lua：函数
来源：http://ef.shtwfgs.cn

function add(a, b) return a + b end
来源：http://ey.jctech888.com.cn

[T37] Lua：字符串拼接
来源：http://vz.huixinmuqiang.cn

"a" .. "b"
来源：http://du.shxzukj.cn

[T38] Lua：条件
来源：http://cb.bjjhwx.cn

if x > 0 then print("正") end
来源：http://lk.muxihuayi.cn

[T39] Lua：模式匹配
来源：http://ie.lnxyls.cn

string.find(s, "%d+")
来源：http://yx.nszjky.cn

[T40] Lua：元表
来源：http://hf.newstarts.cn

setmetatable({}, { __index = base })
来源：http://nl.hahajie.cn

[T41] Perl：Hello World
来源：http://wd.hahajie.cn

print "Hello\n";
来源：http://bk.asd995.cn

[T42] Perl：变量类型
来源：http://rz.521024.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pj.szsharing.cn

[T43] Perl：字符串插值
来源：http://wi.panjiajie.cn

"值: $a"
来源：http://gs.huixinmuqiang.cn

[T44] Perl：条件
来源：http://ih.nicolike.cn

if ($a > 0) { print "正"; }
来源：http://gd.bookmarksfly.cn

[T45] Perl：数组遍历
来源：http://vd.jctech888.com.cn

for my $x (@arr) { print $x; }
来源：http://iw.hnjuh.cn

[T46] Perl：哈希操作
来源：http://qc.hahajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gv.shxzskj.cn

[T47] Perl：正则捕获
来源：http://ua.hahajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://za.wgjwhj.cn

[T48] Perl：正则替换
来源：http://bz.nszjky.cn

$s =~ s/old/new/g;
来源：http://hm.huixiangedu.cn

[T49] Perl：函数
来源：http://ty.hnjuh.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tj.bjjhwx.cn

[T50] Perl：逐行读文件
来源：http://ek.521024.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rk.shxzskj.cn

while (my $line = <$fh>) { print $line; }
来源：http://ty.szsharing.cn

[T51] Scala：Hello World
来源：http://wn.jianghongdianzi.cn

println("Hello")
来源：http://np.521024.cn

[T52] Scala：变量
来源：http://bj.newstarts.cn

val a = 1;  var b = 2
来源：http://xr.panjiajie.cn

[T53] Scala：字符串插值
来源：http://bl.jctech888.com.cn

s"值: $b"
来源：http://ce.yuexingan06.cn

[T54] Scala：集合映射
来源：http://zv.chemitech.net.cn

List(1, 2, 3).map(_ * 2)
来源：http://ni.haigaiapp.cn

[T55] Scala：集合过滤
来源：http://dv.lnxyls.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wz.jctech888.com.cn

[T56] Scala：样例类
来源：http://wk.chemitech.net.cn

case class User(name: String, age: Int)
来源：http://to.hnjuh.cn

[T57] Scala：模式匹配
来源：http://vq.hahajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://sk.yuntaijiaju.cn

[T58] Scala：函数定义
来源：http://fi.gzmigu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://te.yuntaijiaju.cn

[T59] Scala：循环
来源：http://gy.bjjhwx.cn

for (i <- 1 to 10) println(i)
来源：http://ps.wgjwhj.cn

[T60] Scala：折叠
来源：http://iw.chemitech.net.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ba.newstarts.cn

================================================================================
来源：http://om.shxzskj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://of.jctech888.com.cn

================================================================================
来源：http://ml.nicolike.cn

[U01] Py：创建虚拟环境
来源：http://ka.panjiajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qn.yuexingan06.cn

[U02] Py：导出 / 安装依赖
来源：http://sp.huixinmuqiang.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wx.muxihuayi.cn

[U03] Py：加载 .env 配置
来源：http://ze.huixinmuqiang.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://dl.newstarts.cn

[U04] Py：变量调试打印
来源：http://ep.lnxyls.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wm.szxytkj.cn

[U05] Py：列表去重且保序
来源：http://ax.huixinmuqiang.cn

list(dict.fromkeys(arr))
来源：http://od.asd995.cn

[U06] Py：合并两个字典
来源：http://yr.yuntaijiaju.cn

{**a, **b}
来源：http://wm.hnjuh.cn

[U07] Py：反转字典键值
来源：http://rb.wgjwhj.cn

{v: k for k, v in d.items()}
来源：http://ob.huixiangedu.cn

[U08] Py：展平二维列表
来源：http://jt.nszjky.cn

[y for x in nested for y in x]
来源：http://hs.gzmigu.cn

[U09] Py：字典取最大值的键
来源：http://id.haigaiapp.cn

max(d, key=d.get)
来源：http://lm.szxytkj.cn

[U10] Py：按值排序字典
来源：http://ug.newstarts.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sj.chemitech.net.cn

[U11] Py：生成器表达式
来源：http://oq.bookmarksfly.cn

(x * 2 for x in arr)
来源：http://zy.jctech888.com.cn

[U12] Py：取出现最多的 3 个元素
来源：http://bu.panjiajie.cn

Counter(arr).most_common(3)
来源：http://yk.huanxung.cn

[U13] Py：固定长度队列
来源：http://nc.nszjky.cn

deque(maxlen=10)
来源：http://fe.nicolike.cn

[U14] Py：分组收集到列表
来源：http://pw.nicolike.cn

defaultdict(list)
来源：http://mx.panjiajie.cn

[U15] Py：高精度计时
来源：http://dv.panjiajie.cn

t = time.perf_counter()
来源：http://hf.9csxet.cn

[U16] Py：命令行参数解析
来源：http://cb.huixiangedu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://no.gzmigu.cn

[U17] Py：初始化日志
来源：http://pp.nicolike.cn

logging.basicConfig(level=logging.INFO)
来源：http://fl.szxytkj.cn

[U18] Py：预编译正则
来源：http://fr.muxihuayi.cn

pat = re.compile(r"\d+")
来源：http://ls.yuexingan06.cn

[U19] Py：正则替换带回调
来源：http://ru.huixiangedu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://un.wgjwhj.cn

[U20] Py：缓存函数结果
来源：http://ta.shxzukj.cn

@functools.lru_cache(maxsize=None)
来源：http://jg.lnxyls.cn

[U21] Py：自定义上下文管理器
来源：http://uo.newstarts.cn

@contextlib.contextmanager
来源：http://fq.panjiajie.cn

[U22] Py：矩阵转置
来源：http://km.hnjuh.cn

list(zip(*m))
来源：http://sl.newstarts.cn

[U23] Py：分块读取大文件
来源：http://eo.haigaiapp.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://an.yuexingan06.cn

[U24] Py：路径操作
来源：http://gt.huixinmuqiang.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rv.hahajie.cn

[U25] Py：CSV 按字典读
来源：http://jz.bjjhwx.cn

csv.DictReader(f)
来源：http://dx.szsharing.cn

[U26] Py：并发下载
来源：http://lu.9csxet.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rv.szsharing.cn

[U27] Py：异步 HTTP
来源：http://kl.szsharing.cn

aiohttp.ClientSession() 配合 async with
来源：http://wh.huanxung.cn

[U28] Py：类型别名
来源：http://wz.521024.cn

UserId = int
来源：http://sk.521024.cn


<!-- 参考信息 -->