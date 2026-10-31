代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yn.bookmarksfly.cn

[S08] C：动态内存分配与释放
来源：http://aq.yuexingan06.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ze.muxihuayi.cn

[S09] C：结构体定义与初始化
来源：http://lx.lnxyls.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ko.yuntaijiaju.cn

[S10] C：指针与解引用
来源：http://nv.huanxung.cn

int *p = &a;  *p = 5;
来源：http://gx.yuexingan06.cn

[S11] C：逐行读文件
来源：http://nl.colortex.cn

FILE *f = fopen("a.txt", "r");
来源：http://kh.huixinmuqiang.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ln.colortex.cn

fclose(f);
来源：http://fm.szxytkj.cn

[S12] C：写文件
来源：http://lm.chemitech.net.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rc.newstarts.cn

[S13] C：宏定义
来源：http://nz.chemitech.net.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cn.haigaiapp.cn

[S14] C：枚举
来源：http://sd.bjjhwx.cn

enum Color { RED, GREEN, BLUE };
来源：http://id.shxzukj.cn

[S15] C：类型转换
来源：http://nl.szxytkj.cn

(double) a / b
来源：http://pw.huixiangedu.cn

[S16] C：位操作置位
来源：http://rd.muxihuayi.cn

x |= (1 << 3);
来源：http://mh.szxytkj.cn

[S17] C：安全拼接字符串
来源：http://pv.huixiangedu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cq.asd995.cn

[S18] C：命令行参数
来源：http://om.asd995.cn

int main(int argc, char **argv)
来源：http://jj.asd995.cn

[S19] C：快速排序
来源：http://vb.jctech888.com.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vt.huixiangedu.cn

[S20] C：二分查找
来源：http://rt.newstarts.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pe.huixinmuqiang.cn

[S21] C：字符类别判断
来源：http://tl.panjiajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ug.colortex.cn

[S22] C：字符串转数字
来源：http://fl.hahajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jr.asd995.cn

[S23] C：随机数
来源：http://qu.chemitech.net.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://mx.panjiajie.cn

[S24] C：获取本地时间
来源：http://uk.nicolike.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ii.hahajie.cn

[S25] C：内存拷贝
来源：http://be.szsharing.cn

memcpy(dst, src, n);
来源：http://gt.jctech888.com.cn

[S26] C：内存清零
来源：http://od.521024.cn

memset(a, 0, sizeof a);
来源：http://hc.shxzskj.cn

[S27] C：定义常量
来源：http://yh.panjiajie.cn

const double PI = 3.14159;
来源：http://un.yuntaijiaju.cn

[S28] C：静态变量
来源：http://ur.bookmarksfly.cn

static int counter = 0;
来源：http://gv.shxzskj.cn

[S29] C：变参函数
来源：http://rx.jctech888.com.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sx.szxytkj.cn

[S30] C：头文件保护
来源：http://rz.hnjuh.cn

#ifndef X_H
来源：http://eq.muxihuayi.cn

#define X_H
来源：http://ha.haigaiapp.cn

#endif
来源：http://ls.asd995.cn

[S31] C++：Hello World
来源：http://pj.gzmigu.cn

#include <iostream>
来源：http://ri.lnxyls.cn

int main() { std::cout << "Hello\n"; }
来源：http://il.9csxet.cn

[S32] C++：字符串
来源：http://zw.huanxung.cn

std::string s = "hi";  s += "!";
来源：http://dy.newstarts.cn

[S33] C++：vector 增删
来源：http://um.wgjwhj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ke.colortex.cn

[S34] C++：遍历 vector
来源：http://qy.yuntaijiaju.cn

for (auto &x : v) { std::cout << x; }
来源：http://ae.shtwfgs.cn

[S35] C++：map
来源：http://vm.huixiangedu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ag.bjjhwx.cn

[S36] C++：unordered_map
来源：http://ps.szsharing.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cy.nszjky.cn

[S37] C++：set
来源：http://rx.newstarts.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ww.asd995.cn

[S38] C++：排序
来源：http://ta.lnxyls.cn

std::sort(v.begin(), v.end());
来源：http://nc.wgjwhj.cn

[S39] C++：自定义比较器排序
来源：http://gt.szsharing.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oy.huixinmuqiang.cn

[S40] C++：查找元素
来源：http://oa.521024.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://om.haigaiapp.cn

[S41] C++：类与构造函数
来源：http://xu.chemitech.net.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xi.bjjhwx.cn

[S42] C++：继承与虚函数
来源：http://sw.asd995.cn

class B : public Base { public: void f() override {} };
来源：http://ki.lnxyls.cn

[S43] C++：智能指针
来源：http://ry.bookmarksfly.cn

auto p = std::make_unique<int>(5);
来源：http://jz.bookmarksfly.cn

[S44] C++：引用传参
来源：http://mi.huixiangedu.cn

void inc(int &x) { ++x; }
来源：http://hm.haigaiapp.cn

[S45] C++：lambda
来源：http://sj.haigaiapp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://uf.gzmigu.cn

[S46] C++：函数模板
来源：http://yd.szxytkj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ui.huixiangedu.cn

[S47] C++：结构化绑定遍历
来源：http://tk.newstarts.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kb.asd995.cn

[S48] C++：逐行读文件
来源：http://ag.huixinmuqiang.cn

std::ifstream in("a.txt");  std::string line;
来源：http://lj.gzmigu.cn

while (std::getline(in, line)) { }
来源：http://lu.yuntaijiaju.cn

[S49] C++：写文件
来源：http://dn.nszjky.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ad.yuexingan06.cn

[S50] C++：格式化数字
来源：http://cc.wgjwhj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zx.wgjwhj.cn

[S51] C++：显式类型转换
来源：http://pq.huanxung.cn

static_cast<double>(a) / b
来源：http://sk.bjjhwx.cn

[S52] C++：const 与 noexcept
来源：http://qt.9csxet.cn

int size() const noexcept { return n_; }
来源：http://it.jianghongdianzi.cn

[S53] C++：移动语义
来源：http://mj.nicolike.cn

std::vector<int> w = std::move(v);
来源：http://yq.lnxyls.cn

[S54] C++：异常处理
来源：http://wc.szxytkj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cl.huixinmuqiang.cn

[S55] C++：结构化绑定
来源：http://pk.panjiajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://od.wgjwhj.cn

[S56] C++：optional
来源：http://mi.bookmarksfly.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gp.nicolike.cn

[S57] C++：编译期常量
来源：http://ce.huanxung.cn

constexpr int N = 10;
来源：http://rr.colortex.cn

[S58] C++：命名空间
来源：http://jp.haigaiapp.cn

namespace ns { int f() { return 1; } }
来源：http://nm.shtwfgs.cn

[S59] C++：静态断言
来源：http://bs.nszjky.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://td.newstarts.cn

[S60] C++：遍历并删除元素
来源：http://as.9csxet.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yz.szsharing.cn

================================================================================
来源：http://sj.huanxung.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qv.nicolike.cn

================================================================================
来源：http://xn.bookmarksfly.cn

[T01] Kotlin：Hello World
来源：http://zp.muxihuayi.cn

println("Hello")
来源：http://ij.shxzukj.cn

[T02] Kotlin：变量
来源：http://lc.huanxung.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ad.bjjhwx.cn

[T03] Kotlin：字符串模板
来源：http://pp.colortex.cn

"值: $b"
来源：http://hu.shxzskj.cn

[T04] Kotlin：空安全
来源：http://np.asd995.cn

val n: String? = null;  n?.length
来源：http://qu.szxytkj.cn

[T05] Kotlin：when 表达式
来源：http://vz.asd995.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pn.haigaiapp.cn

[T06] Kotlin：集合映射
来源：http://ve.nicolike.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://lh.shxzukj.cn

[T07] Kotlin：集合过滤
来源：http://sp.huanxung.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://cb.wgjwhj.cn

[T08] Kotlin：数据类
来源：http://gy.jianghongdianzi.cn

data class User(val name: String, val age: Int)
来源：http://vx.shtwfgs.cn

[T09] Kotlin：扩展函数
来源：http://ls.jianghongdianzi.cn

fun String.exclaim() = this + "!"
来源：http://ok.yuexingan06.cn

[T10] Kotlin：默认参数
来源：http://bp.jianghongdianzi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ph.bjjhwx.cn

[T11] Kotlin：协程
来源：http://ot.huixinmuqiang.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://md.haigaiapp.cn

[T12] Kotlin：解构声明
来源：http://mx.yuntaijiaju.cn

val (a, b) = Pair(1, 2)
来源：http://nn.jianghongdianzi.cn

[T13] Kotlin：只读 Map
来源：http://aq.lnxyls.cn

val m = mapOf("a" to 1)
来源：http://zz.shtwfgs.cn

[T14] Kotlin：循环
来源：http://ax.shxzskj.cn

for (i in 1..10) println(i)
来源：http://wd.shxzskj.cn

[T15] Kotlin：接口
来源：http://jx.huanxung.cn

interface Shape { fun area(): Double }
来源：http://gq.hahajie.cn

[T16] Swift：Hello World
来源：http://pj.bookmarksfly.cn

print("Hello")
来源：http://df.huixinmuqiang.cn

[T17] Swift：变量与常量
来源：http://fd.colortex.cn

var a = 1;  let b = 2
来源：http://tl.szsharing.cn

[T18] Swift：字符串插值
来源：http://sg.shtwfgs.cn

"值: \(b)"
来源：http://ru.asd995.cn

[T19] Swift：可选绑定
来源：http://go.szsharing.cn

if let n = opt { print(n) }
来源：http://va.asd995.cn

[T20] Swift：数组操作
来源：http://ij.muxihuayi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mp.shxzukj.cn

[T21] Swift：遍历
来源：http://ho.jianghongdianzi.cn

for x in a { print(x) }
来源：http://ov.jianghongdianzi.cn

[T22] Swift：字典
来源：http://rd.nicolike.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mm.newstarts.cn

[T23] Swift：函数
来源：http://pm.bookmarksfly.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vv.panjiajie.cn

[T24] Swift：闭包
来源：http://ox.panjiajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://mp.hahajie.cn

[T25] Swift：结构体
来源：http://ag.panjiajie.cn

struct P { var x: Int }
来源：http://ob.jianghongdianzi.cn

[T26] Swift：类与重写
来源：http://lr.yuntaijiaju.cn

class A: Base { override func f() {} }
来源：http://jq.newstarts.cn

[T27] Swift：错误处理
来源：http://zx.colortex.cn

do { try f() } catch { print(error) }
来源：http://xk.asd995.cn

[T28] Swift：枚举
来源：http://hc.nszjky.cn

enum Color { case red, green }
来源：http://ff.hnjuh.cn

[T29] Swift：guard 提前返回
来源：http://kl.yuntaijiaju.cn

guard let x = opt else { return }
来源：http://cu.wgjwhj.cn

[T30] Swift：协议
来源：http://wt.lnxyls.cn

protocol Shape { func area() -> Double }
来源：http://ui.shxzukj.cn

[T31] Lua：Hello World
来源：http://po.huanxung.cn

print("Hello")
来源：http://um.chemitech.net.cn

[T32] Lua：局部变量
来源：http://wt.huixiangedu.cn

local a = 1
来源：http://hg.9csxet.cn

[T33] Lua：表（数组）
来源：http://ql.jctech888.com.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://pl.huixinmuqiang.cn

[T34] Lua：遍历表
来源：http://da.shtwfgs.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://sj.hnjuh.cn

[T35] Lua：字典表
来源：http://qp.wgjwhj.cn

local d = { a = 1 };  d.b = 2
来源：http://kq.jianghongdianzi.cn

[T36] Lua：函数
来源：http://mp.chemitech.net.cn

function add(a, b) return a + b end
来源：http://bv.jianghongdianzi.cn

[T37] Lua：字符串拼接
来源：http://dj.shxzukj.cn

"a" .. "b"
来源：http://gd.panjiajie.cn

[T38] Lua：条件
来源：http://oo.9csxet.cn

if x > 0 then print("正") end
来源：http://yw.shxzskj.cn

[T39] Lua：模式匹配
来源：http://rw.9csxet.cn

string.find(s, "%d+")
来源：http://oi.szxytkj.cn

[T40] Lua：元表
来源：http://iw.yuexingan06.cn

setmetatable({}, { __index = base })
来源：http://xq.huixiangedu.cn

[T41] Perl：Hello World
来源：http://jo.hnjuh.cn

print "Hello\n";
来源：http://fc.hnjuh.cn

[T42] Perl：变量类型
来源：http://cy.haigaiapp.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zi.huixinmuqiang.cn

[T43] Perl：字符串插值
来源：http://yp.521024.cn

"值: $a"
来源：http://qd.521024.cn

[T44] Perl：条件
来源：http://vx.chemitech.net.cn

if ($a > 0) { print "正"; }
来源：http://ui.shxzukj.cn

[T45] Perl：数组遍历
来源：http://ra.jianghongdianzi.cn

for my $x (@arr) { print $x; }
来源：http://wv.huixinmuqiang.cn

[T46] Perl：哈希操作
来源：http://cn.9csxet.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rp.yuntaijiaju.cn

[T47] Perl：正则捕获
来源：http://pj.panjiajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wt.shxzskj.cn

[T48] Perl：正则替换
来源：http://gv.gzmigu.cn

$s =~ s/old/new/g;
来源：http://xz.hnjuh.cn

[T49] Perl：函数
来源：http://ee.jctech888.com.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://by.hahajie.cn

[T50] Perl：逐行读文件
来源：http://pm.9csxet.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://af.nszjky.cn

while (my $line = <$fh>) { print $line; }
来源：http://dp.nicolike.cn

[T51] Scala：Hello World
来源：http://ik.szxytkj.cn

println("Hello")
来源：http://cp.lnxyls.cn

[T52] Scala：变量
来源：http://pj.chemitech.net.cn

val a = 1;  var b = 2
来源：http://eu.szxytkj.cn

[T53] Scala：字符串插值
来源：http://bf.shxzukj.cn

s"值: $b"
来源：http://ul.colortex.cn

[T54] Scala：集合映射
来源：http://ja.lnxyls.cn

List(1, 2, 3).map(_ * 2)
来源：http://kg.nicolike.cn

[T55] Scala：集合过滤
来源：http://dh.huanxung.cn

List(1, 2, 3).filter(_ > 1)
来源：http://hc.asd995.cn

[T56] Scala：样例类
来源：http://if.muxihuayi.cn

case class User(name: String, age: Int)
来源：http://yj.szxytkj.cn

[T57] Scala：模式匹配
来源：http://bv.gzmigu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://zf.shxzukj.cn

[T58] Scala：函数定义
来源：http://qr.shxzskj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://kj.shtwfgs.cn

[T59] Scala：循环
来源：http://st.jianghongdianzi.cn

for (i <- 1 to 10) println(i)
来源：http://ad.bookmarksfly.cn

[T60] Scala：折叠
来源：http://xj.nszjky.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://px.yuntaijiaju.cn

================================================================================
来源：http://se.shxzukj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://am.panjiajie.cn

================================================================================
来源：http://gz.huixinmuqiang.cn

[U01] Py：创建虚拟环境
来源：http://qu.521024.cn

python -m venv .venv && source .venv/bin/activate
来源：http://xn.hahajie.cn

[U02] Py：导出 / 安装依赖
来源：http://dc.shxzskj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kj.hnjuh.cn

[U03] Py：加载 .env 配置
来源：http://xq.shxzukj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://kc.bjjhwx.cn

[U04] Py：变量调试打印
来源：http://yl.shxzskj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://te.yuexingan06.cn

[U05] Py：列表去重且保序
来源：http://om.shxzskj.cn

list(dict.fromkeys(arr))
来源：http://bz.huixinmuqiang.cn

[U06] Py：合并两个字典
来源：http://pp.yuexingan06.cn

{**a, **b}
来源：http://ae.huixiangedu.cn

[U07] Py：反转字典键值
来源：http://ho.gzmigu.cn

{v: k for k, v in d.items()}
来源：http://pt.gzmigu.cn

[U08] Py：展平二维列表
来源：http://zd.gzmigu.cn

[y for x in nested for y in x]
来源：http://no.9csxet.cn

[U09] Py：字典取最大值的键
来源：http://pe.szsharing.cn

max(d, key=d.get)
来源：http://ws.gzmigu.cn

[U10] Py：按值排序字典
来源：http://pv.shtwfgs.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ix.yuexingan06.cn

[U11] Py：生成器表达式
来源：http://wm.yuexingan06.cn

(x * 2 for x in arr)
来源：http://ca.panjiajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://oj.jctech888.com.cn

Counter(arr).most_common(3)
来源：http://lh.huixinmuqiang.cn

[U13] Py：固定长度队列
来源：http://qe.newstarts.cn

deque(maxlen=10)
来源：http://ak.hahajie.cn

[U14] Py：分组收集到列表
来源：http://kj.521024.cn

defaultdict(list)
来源：http://qx.huixinmuqiang.cn

[U15] Py：高精度计时
来源：http://mx.lnxyls.cn

t = time.perf_counter()
来源：http://re.newstarts.cn

[U16] Py：命令行参数解析
来源：http://ri.yuntaijiaju.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jv.szxytkj.cn

[U17] Py：初始化日志
来源：http://cp.lnxyls.cn

logging.basicConfig(level=logging.INFO)
来源：http://cx.huanxung.cn

[U18] Py：预编译正则
来源：http://sx.wgjwhj.cn

pat = re.compile(r"\d+")
来源：http://ss.lnxyls.cn

[U19] Py：正则替换带回调
来源：http://lf.gzmigu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://el.gzmigu.cn

[U20] Py：缓存函数结果
来源：http://ua.jctech888.com.cn

@functools.lru_cache(maxsize=None)
来源：http://pg.huanxung.cn

[U21] Py：自定义上下文管理器
来源：http://ka.yuntaijiaju.cn

@contextlib.contextmanager
来源：http://bs.yuntaijiaju.cn

[U22] Py：矩阵转置
来源：http://bs.nicolike.cn

list(zip(*m))
来源：http://vj.jianghongdianzi.cn

[U23] Py：分块读取大文件
来源：http://oh.szxytkj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jv.haigaiapp.cn

[U24] Py：路径操作
来源：http://pb.shxzskj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ki.huixinmuqiang.cn

[U25] Py：CSV 按字典读
来源：http://um.lnxyls.cn

csv.DictReader(f)
来源：http://zj.9csxet.cn

[U26] Py：并发下载
来源：http://ix.lnxyls.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qv.gzmigu.cn

[U27] Py：异步 HTTP
来源：http://wt.shxzukj.cn

aiohttp.ClientSession() 配合 async with
来源：http://uj.szxytkj.cn

[U28] Py：类型别名
来源：http://nt.panjiajie.cn

UserId = int
来源：http://lx.szsharing.cn

[U29] Py：属性校验
来源：http://iw.shtwfgs.cn

@property 与 @x.setter 配合
来源：http://vz.hnjuh.cn

[U30] Py：数据类
来源：http://zf.panjiajie.cn

@dataclass(slots=True)
来源：http://gz.lnxyls.cn


<!-- 参考信息 -->