代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gk.hahajie.cn

[S08] C：动态内存分配与释放
来源：http://ca.asd995.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nn.shxzskj.cn

[S09] C：结构体定义与初始化
来源：http://ph.yuntaijiaju.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xi.colortex.cn

[S10] C：指针与解引用
来源：http://ja.jctech888.com.cn

int *p = &a;  *p = 5;
来源：http://bg.jianghongdianzi.cn

[S11] C：逐行读文件
来源：http://ei.9csxet.cn

FILE *f = fopen("a.txt", "r");
来源：http://fg.haigaiapp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gk.huanxung.cn

fclose(f);
来源：http://mc.szsharing.cn

[S12] C：写文件
来源：http://qc.521024.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rl.chemitech.net.cn

[S13] C：宏定义
来源：http://aq.bookmarksfly.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ox.haigaiapp.cn

[S14] C：枚举
来源：http://yt.panjiajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://bb.huixinmuqiang.cn

[S15] C：类型转换
来源：http://rh.521024.cn

(double) a / b
来源：http://ll.nszjky.cn

[S16] C：位操作置位
来源：http://ln.hnjuh.cn

x |= (1 << 3);
来源：http://qq.hahajie.cn

[S17] C：安全拼接字符串
来源：http://ny.huixinmuqiang.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gr.shxzskj.cn

[S18] C：命令行参数
来源：http://ul.nicolike.cn

int main(int argc, char **argv)
来源：http://py.newstarts.cn

[S19] C：快速排序
来源：http://nl.asd995.cn

qsort(a, n, sizeof(int), cmp);
来源：http://co.huixiangedu.cn

[S20] C：二分查找
来源：http://ml.colortex.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nj.nicolike.cn

[S21] C：字符类别判断
来源：http://jc.yuexingan06.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jo.shtwfgs.cn

[S22] C：字符串转数字
来源：http://hc.bookmarksfly.cn

atoi("42");  strtod("3.14", NULL);
来源：http://il.yuntaijiaju.cn

[S23] C：随机数
来源：http://ns.shxzukj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ph.lnxyls.cn

[S24] C：获取本地时间
来源：http://gu.hnjuh.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uq.gzmigu.cn

[S25] C：内存拷贝
来源：http://km.bookmarksfly.cn

memcpy(dst, src, n);
来源：http://tr.wgjwhj.cn

[S26] C：内存清零
来源：http://lj.chemitech.net.cn

memset(a, 0, sizeof a);
来源：http://mp.muxihuayi.cn

[S27] C：定义常量
来源：http://ic.bjjhwx.cn

const double PI = 3.14159;
来源：http://zc.muxihuayi.cn

[S28] C：静态变量
来源：http://gs.wgjwhj.cn

static int counter = 0;
来源：http://je.newstarts.cn

[S29] C：变参函数
来源：http://gn.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://an.9csxet.cn

[S30] C：头文件保护
来源：http://ol.newstarts.cn

#ifndef X_H
来源：http://md.haigaiapp.cn

#define X_H
来源：http://kn.newstarts.cn

#endif
来源：http://zm.yuntaijiaju.cn

[S31] C++：Hello World
来源：http://py.bjjhwx.cn

#include <iostream>
来源：http://yc.huixiangedu.cn

int main() { std::cout << "Hello\n"; }
来源：http://yx.shxzskj.cn

[S32] C++：字符串
来源：http://rb.szsharing.cn

std::string s = "hi";  s += "!";
来源：http://ge.jctech888.com.cn

[S33] C++：vector 增删
来源：http://fd.haigaiapp.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ht.yuexingan06.cn

[S34] C++：遍历 vector
来源：http://ik.huixinmuqiang.cn

for (auto &x : v) { std::cout << x; }
来源：http://ch.colortex.cn

[S35] C++：map
来源：http://ar.szxytkj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nm.muxihuayi.cn

[S36] C++：unordered_map
来源：http://aj.shtwfgs.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xh.asd995.cn

[S37] C++：set
来源：http://yx.shtwfgs.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ms.newstarts.cn

[S38] C++：排序
来源：http://tu.shtwfgs.cn

std::sort(v.begin(), v.end());
来源：http://fl.hahajie.cn

[S39] C++：自定义比较器排序
来源：http://ss.bjjhwx.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sv.yuexingan06.cn

[S40] C++：查找元素
来源：http://rb.szxytkj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://au.jianghongdianzi.cn

[S41] C++：类与构造函数
来源：http://cr.szsharing.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zk.panjiajie.cn

[S42] C++：继承与虚函数
来源：http://cj.jianghongdianzi.cn

class B : public Base { public: void f() override {} };
来源：http://su.hnjuh.cn

[S43] C++：智能指针
来源：http://mn.colortex.cn

auto p = std::make_unique<int>(5);
来源：http://ta.huanxung.cn

[S44] C++：引用传参
来源：http://yi.jianghongdianzi.cn

void inc(int &x) { ++x; }
来源：http://yu.huanxung.cn

[S45] C++：lambda
来源：http://ge.huixiangedu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xe.nicolike.cn

[S46] C++：函数模板
来源：http://az.szsharing.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://iu.newstarts.cn

[S47] C++：结构化绑定遍历
来源：http://gl.szsharing.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://he.nicolike.cn

[S48] C++：逐行读文件
来源：http://ie.lnxyls.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fw.haigaiapp.cn

while (std::getline(in, line)) { }
来源：http://qi.wgjwhj.cn

[S49] C++：写文件
来源：http://yv.shtwfgs.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://we.bookmarksfly.cn

[S50] C++：格式化数字
来源：http://re.colortex.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qk.gzmigu.cn

[S51] C++：显式类型转换
来源：http://sm.9csxet.cn

static_cast<double>(a) / b
来源：http://ve.lnxyls.cn

[S52] C++：const 与 noexcept
来源：http://xw.lnxyls.cn

int size() const noexcept { return n_; }
来源：http://wl.chemitech.net.cn

[S53] C++：移动语义
来源：http://hq.muxihuayi.cn

std::vector<int> w = std::move(v);
来源：http://yp.wgjwhj.cn

[S54] C++：异常处理
来源：http://ba.jctech888.com.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pu.jctech888.com.cn

[S55] C++：结构化绑定
来源：http://vy.nszjky.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gi.shxzskj.cn

[S56] C++：optional
来源：http://ix.huixinmuqiang.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tk.szxytkj.cn

[S57] C++：编译期常量
来源：http://ue.newstarts.cn

constexpr int N = 10;
来源：http://dd.bjjhwx.cn

[S58] C++：命名空间
来源：http://xm.shtwfgs.cn

namespace ns { int f() { return 1; } }
来源：http://jr.huanxung.cn

[S59] C++：静态断言
来源：http://ln.gzmigu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qn.muxihuayi.cn

[S60] C++：遍历并删除元素
来源：http://xx.wgjwhj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bs.hnjuh.cn

================================================================================
来源：http://nk.521024.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qm.yuntaijiaju.cn

================================================================================
来源：http://yk.yuntaijiaju.cn

[T01] Kotlin：Hello World
来源：http://qx.huanxung.cn

println("Hello")
来源：http://fo.haigaiapp.cn

[T02] Kotlin：变量
来源：http://ay.nicolike.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mu.newstarts.cn

[T03] Kotlin：字符串模板
来源：http://lc.yuntaijiaju.cn

"值: $b"
来源：http://ne.jianghongdianzi.cn

[T04] Kotlin：空安全
来源：http://dd.jctech888.com.cn

val n: String? = null;  n?.length
来源：http://pm.shxzskj.cn

[T05] Kotlin：when 表达式
来源：http://lx.hahajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://co.huanxung.cn

[T06] Kotlin：集合映射
来源：http://vz.yuexingan06.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://dl.haigaiapp.cn

[T07] Kotlin：集合过滤
来源：http://hn.shxzskj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tv.shxzskj.cn

[T08] Kotlin：数据类
来源：http://ft.panjiajie.cn

data class User(val name: String, val age: Int)
来源：http://ri.gzmigu.cn

[T09] Kotlin：扩展函数
来源：http://wc.wgjwhj.cn

fun String.exclaim() = this + "!"
来源：http://vu.lnxyls.cn

[T10] Kotlin：默认参数
来源：http://jx.lnxyls.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://bs.chemitech.net.cn

[T11] Kotlin：协程
来源：http://pb.hahajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vr.bjjhwx.cn

[T12] Kotlin：解构声明
来源：http://hv.521024.cn

val (a, b) = Pair(1, 2)
来源：http://gq.gzmigu.cn

[T13] Kotlin：只读 Map
来源：http://gp.panjiajie.cn

val m = mapOf("a" to 1)
来源：http://ee.haigaiapp.cn

[T14] Kotlin：循环
来源：http://vr.chemitech.net.cn

for (i in 1..10) println(i)
来源：http://zi.muxihuayi.cn

[T15] Kotlin：接口
来源：http://lr.jianghongdianzi.cn

interface Shape { fun area(): Double }
来源：http://lk.lnxyls.cn

[T16] Swift：Hello World
来源：http://uw.huixiangedu.cn

print("Hello")
来源：http://ku.shtwfgs.cn

[T17] Swift：变量与常量
来源：http://vc.szxytkj.cn

var a = 1;  let b = 2
来源：http://uf.huixiangedu.cn

[T18] Swift：字符串插值
来源：http://az.asd995.cn

"值: \(b)"
来源：http://gb.haigaiapp.cn

[T19] Swift：可选绑定
来源：http://zf.muxihuayi.cn

if let n = opt { print(n) }
来源：http://kr.jianghongdianzi.cn

[T20] Swift：数组操作
来源：http://rc.hnjuh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ua.muxihuayi.cn

[T21] Swift：遍历
来源：http://jl.haigaiapp.cn

for x in a { print(x) }
来源：http://kf.shxzukj.cn

[T22] Swift：字典
来源：http://yq.nicolike.cn

var d = ["a": 1];  d["b"] = 2
来源：http://jd.lnxyls.cn

[T23] Swift：函数
来源：http://hy.yuntaijiaju.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://co.lnxyls.cn

[T24] Swift：闭包
来源：http://th.shxzukj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://dr.huixinmuqiang.cn

[T25] Swift：结构体
来源：http://ck.jianghongdianzi.cn

struct P { var x: Int }
来源：http://il.huixinmuqiang.cn

[T26] Swift：类与重写
来源：http://ye.wgjwhj.cn

class A: Base { override func f() {} }
来源：http://cd.bjjhwx.cn

[T27] Swift：错误处理
来源：http://rn.szxytkj.cn

do { try f() } catch { print(error) }
来源：http://vu.nszjky.cn

[T28] Swift：枚举
来源：http://bb.shxzskj.cn

enum Color { case red, green }
来源：http://td.521024.cn

[T29] Swift：guard 提前返回
来源：http://ql.yuexingan06.cn

guard let x = opt else { return }
来源：http://pu.wgjwhj.cn

[T30] Swift：协议
来源：http://wt.jianghongdianzi.cn

protocol Shape { func area() -> Double }
来源：http://mk.newstarts.cn

[T31] Lua：Hello World
来源：http://hc.haigaiapp.cn

print("Hello")
来源：http://ww.huixiangedu.cn

[T32] Lua：局部变量
来源：http://hu.szsharing.cn

local a = 1
来源：http://of.yuntaijiaju.cn

[T33] Lua：表（数组）
来源：http://md.9csxet.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vq.bjjhwx.cn

[T34] Lua：遍历表
来源：http://xa.jctech888.com.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qs.hnjuh.cn

[T35] Lua：字典表
来源：http://ba.yuexingan06.cn

local d = { a = 1 };  d.b = 2
来源：http://lg.panjiajie.cn

[T36] Lua：函数
来源：http://kt.521024.cn

function add(a, b) return a + b end
来源：http://ub.bookmarksfly.cn

[T37] Lua：字符串拼接
来源：http://gk.panjiajie.cn

"a" .. "b"
来源：http://os.asd995.cn

[T38] Lua：条件
来源：http://ac.shxzukj.cn

if x > 0 then print("正") end
来源：http://hl.nszjky.cn

[T39] Lua：模式匹配
来源：http://cs.yuexingan06.cn

string.find(s, "%d+")
来源：http://hy.newstarts.cn

[T40] Lua：元表
来源：http://pi.yuexingan06.cn

setmetatable({}, { __index = base })
来源：http://zo.haigaiapp.cn

[T41] Perl：Hello World
来源：http://vy.panjiajie.cn

print "Hello\n";
来源：http://ho.9csxet.cn

[T42] Perl：变量类型
来源：http://dy.newstarts.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xe.jctech888.com.cn

[T43] Perl：字符串插值
来源：http://oi.szsharing.cn

"值: $a"
来源：http://ln.huixiangedu.cn

[T44] Perl：条件
来源：http://nc.hnjuh.cn

if ($a > 0) { print "正"; }
来源：http://rl.bookmarksfly.cn

[T45] Perl：数组遍历
来源：http://do.muxihuayi.cn

for my $x (@arr) { print $x; }
来源：http://ne.lnxyls.cn

[T46] Perl：哈希操作
来源：http://mn.asd995.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ix.newstarts.cn

[T47] Perl：正则捕获
来源：http://mf.gzmigu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://kr.hahajie.cn

[T48] Perl：正则替换
来源：http://kg.yuntaijiaju.cn

$s =~ s/old/new/g;
来源：http://rb.shtwfgs.cn

[T49] Perl：函数
来源：http://nb.asd995.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://um.huanxung.cn

[T50] Perl：逐行读文件
来源：http://gd.wgjwhj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://up.szsharing.cn

while (my $line = <$fh>) { print $line; }
来源：http://oi.nicolike.cn

[T51] Scala：Hello World
来源：http://pz.shxzukj.cn

println("Hello")
来源：http://ra.asd995.cn

[T52] Scala：变量
来源：http://nu.bookmarksfly.cn

val a = 1;  var b = 2
来源：http://cq.hnjuh.cn

[T53] Scala：字符串插值
来源：http://cs.chemitech.net.cn

s"值: $b"
来源：http://fq.lnxyls.cn

[T54] Scala：集合映射
来源：http://ht.szxytkj.cn

List(1, 2, 3).map(_ * 2)
来源：http://aq.shxzskj.cn

[T55] Scala：集合过滤
来源：http://tf.jianghongdianzi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://lj.9csxet.cn

[T56] Scala：样例类
来源：http://xe.9csxet.cn

case class User(name: String, age: Int)
来源：http://cq.gzmigu.cn

[T57] Scala：模式匹配
来源：http://kk.9csxet.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://sa.yuexingan06.cn

[T58] Scala：函数定义
来源：http://kf.huanxung.cn

def add(a: Int, b: Int): Int = a + b
来源：http://np.bjjhwx.cn

[T59] Scala：循环
来源：http://dh.szxytkj.cn

for (i <- 1 to 10) println(i)
来源：http://uh.newstarts.cn

[T60] Scala：折叠
来源：http://vv.newstarts.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ut.hnjuh.cn

================================================================================
来源：http://ag.jctech888.com.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://je.muxihuayi.cn

================================================================================
来源：http://iw.521024.cn

[U01] Py：创建虚拟环境
来源：http://da.lnxyls.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bc.chemitech.net.cn

[U02] Py：导出 / 安装依赖
来源：http://ni.szxytkj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.szsharing.cn

[U03] Py：加载 .env 配置
来源：http://ac.huanxung.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ud.shtwfgs.cn

[U04] Py：变量调试打印
来源：http://fx.muxihuayi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mc.bookmarksfly.cn

[U05] Py：列表去重且保序
来源：http://qe.szsharing.cn

list(dict.fromkeys(arr))
来源：http://ed.haigaiapp.cn

[U06] Py：合并两个字典
来源：http://hq.chemitech.net.cn

{**a, **b}
来源：http://ry.szxytkj.cn

[U07] Py：反转字典键值
来源：http://yn.yuntaijiaju.cn

{v: k for k, v in d.items()}
来源：http://ns.muxihuayi.cn

[U08] Py：展平二维列表
来源：http://jm.shtwfgs.cn

[y for x in nested for y in x]
来源：http://uu.shxzskj.cn

[U09] Py：字典取最大值的键
来源：http://cb.lnxyls.cn

max(d, key=d.get)
来源：http://lh.shtwfgs.cn

[U10] Py：按值排序字典
来源：http://wl.szxytkj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wf.jctech888.com.cn

[U11] Py：生成器表达式
来源：http://da.szsharing.cn

(x * 2 for x in arr)
来源：http://ni.shtwfgs.cn

[U12] Py：取出现最多的 3 个元素
来源：http://iz.huanxung.cn

Counter(arr).most_common(3)
来源：http://eb.bjjhwx.cn

[U13] Py：固定长度队列
来源：http://tu.haigaiapp.cn

deque(maxlen=10)
来源：http://yy.muxihuayi.cn

[U14] Py：分组收集到列表
来源：http://bt.yuntaijiaju.cn

defaultdict(list)
来源：http://bp.9csxet.cn

[U15] Py：高精度计时
来源：http://wb.jctech888.com.cn

t = time.perf_counter()
来源：http://td.bookmarksfly.cn

[U16] Py：命令行参数解析
来源：http://de.huixinmuqiang.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nz.yuntaijiaju.cn

[U17] Py：初始化日志
来源：http://pn.yuntaijiaju.cn

logging.basicConfig(level=logging.INFO)
来源：http://ck.jianghongdianzi.cn

[U18] Py：预编译正则
来源：http://gg.nicolike.cn

pat = re.compile(r"\d+")
来源：http://gs.nicolike.cn

[U19] Py：正则替换带回调
来源：http://xd.jctech888.com.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://um.shxzukj.cn

[U20] Py：缓存函数结果
来源：http://fw.newstarts.cn

@functools.lru_cache(maxsize=None)
来源：http://sk.lnxyls.cn

[U21] Py：自定义上下文管理器
来源：http://cv.muxihuayi.cn

@contextlib.contextmanager
来源：http://se.yuntaijiaju.cn

[U22] Py：矩阵转置
来源：http://cz.szsharing.cn

list(zip(*m))
来源：http://tv.huanxung.cn

[U23] Py：分块读取大文件
来源：http://la.lnxyls.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ot.gzmigu.cn

[U24] Py：路径操作
来源：http://ew.9csxet.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://js.huixinmuqiang.cn

[U25] Py：CSV 按字典读
来源：http://la.shtwfgs.cn

csv.DictReader(f)
来源：http://zj.lnxyls.cn

[U26] Py：并发下载
来源：http://py.shxzukj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mb.colortex.cn

[U27] Py：异步 HTTP
来源：http://zv.hahajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://tb.shtwfgs.cn

[U28] Py：类型别名
来源：http://si.huixinmuqiang.cn

UserId = int
来源：http://jt.huanxung.cn

[U29] Py：属性校验
来源：http://ch.jianghongdianzi.cn

@property 与 @x.setter 配合
来源：http://qt.9csxet.cn

[U30] Py：数据类
来源：http://ri.huixiangedu.cn

@dataclass(slots=True)
来源：http://ok.nszjky.cn


<!-- 参考信息 -->