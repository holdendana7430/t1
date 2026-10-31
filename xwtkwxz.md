代发 wailian999

int x; scanf("%d", &x);
来源：http://rh.szsharing.cn

[S04] C：字符串复制
来源：http://ns.gzmigu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gh.szsharing.cn

[S05] C：字符串长度
来源：http://cp.huixinmuqiang.cn

strlen(s)
来源：http://gj.huanxung.cn

[S06] C：字符串比较
来源：http://mj.bjjhwx.cn

strcmp(a, b) == 0
来源：http://uu.yuexingan06.cn

[S07] C：数组遍历求和
来源：http://kc.huixinmuqiang.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ej.gzmigu.cn

[S08] C：动态内存分配与释放
来源：http://ao.hnjuh.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xr.gzmigu.cn

[S09] C：结构体定义与初始化
来源：http://aj.colortex.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ny.szxytkj.cn

[S10] C：指针与解引用
来源：http://cm.hnjuh.cn

int *p = &a;  *p = 5;
来源：http://rn.shxzukj.cn

[S11] C：逐行读文件
来源：http://zr.wgjwhj.cn

FILE *f = fopen("a.txt", "r");
来源：http://tq.9csxet.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gg.chemitech.net.cn

fclose(f);
来源：http://zy.shtwfgs.cn

[S12] C：写文件
来源：http://vs.jianghongdianzi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wg.lnxyls.cn

[S13] C：宏定义
来源：http://ls.hahajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qd.shtwfgs.cn

[S14] C：枚举
来源：http://pt.szxytkj.cn

enum Color { RED, GREEN, BLUE };
来源：http://ls.huanxung.cn

[S15] C：类型转换
来源：http://sb.yuexingan06.cn

(double) a / b
来源：http://hr.szsharing.cn

[S16] C：位操作置位
来源：http://tp.huixiangedu.cn

x |= (1 << 3);
来源：http://us.jianghongdianzi.cn

[S17] C：安全拼接字符串
来源：http://tg.jctech888.com.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bg.muxihuayi.cn

[S18] C：命令行参数
来源：http://wc.panjiajie.cn

int main(int argc, char **argv)
来源：http://dh.shtwfgs.cn

[S19] C：快速排序
来源：http://pi.521024.cn

qsort(a, n, sizeof(int), cmp);
来源：http://yi.huixinmuqiang.cn

[S20] C：二分查找
来源：http://ln.lnxyls.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gm.nicolike.cn

[S21] C：字符类别判断
来源：http://jm.hnjuh.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rf.bookmarksfly.cn

[S22] C：字符串转数字
来源：http://ym.asd995.cn

atoi("42");  strtod("3.14", NULL);
来源：http://du.huixinmuqiang.cn

[S23] C：随机数
来源：http://cm.shtwfgs.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://nj.gzmigu.cn

[S24] C：获取本地时间
来源：http://qa.gzmigu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://st.huixinmuqiang.cn

[S25] C：内存拷贝
来源：http://mn.yuexingan06.cn

memcpy(dst, src, n);
来源：http://qo.shxzskj.cn

[S26] C：内存清零
来源：http://ud.shxzukj.cn

memset(a, 0, sizeof a);
来源：http://po.shxzskj.cn

[S27] C：定义常量
来源：http://vd.chemitech.net.cn

const double PI = 3.14159;
来源：http://ba.shtwfgs.cn

[S28] C：静态变量
来源：http://jm.muxihuayi.cn

static int counter = 0;
来源：http://bn.haigaiapp.cn

[S29] C：变参函数
来源：http://aw.nicolike.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vy.panjiajie.cn

[S30] C：头文件保护
来源：http://es.shxzukj.cn

#ifndef X_H
来源：http://qc.bookmarksfly.cn

#define X_H
来源：http://as.asd995.cn

#endif
来源：http://bm.jctech888.com.cn

[S31] C++：Hello World
来源：http://kg.bjjhwx.cn

#include <iostream>
来源：http://yl.bjjhwx.cn

int main() { std::cout << "Hello\n"; }
来源：http://ih.newstarts.cn

[S32] C++：字符串
来源：http://uk.szsharing.cn

std::string s = "hi";  s += "!";
来源：http://kd.huanxung.cn

[S33] C++：vector 增删
来源：http://mg.newstarts.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ox.haigaiapp.cn

[S34] C++：遍历 vector
来源：http://gw.colortex.cn

for (auto &x : v) { std::cout << x; }
来源：http://qp.huixinmuqiang.cn

[S35] C++：map
来源：http://nu.wgjwhj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://du.9csxet.cn

[S36] C++：unordered_map
来源：http://ep.yuexingan06.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nq.hnjuh.cn

[S37] C++：set
来源：http://rg.yuntaijiaju.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mz.szsharing.cn

[S38] C++：排序
来源：http://en.yuexingan06.cn

std::sort(v.begin(), v.end());
来源：http://ov.asd995.cn

[S39] C++：自定义比较器排序
来源：http://xf.shxzukj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xj.newstarts.cn

[S40] C++：查找元素
来源：http://vw.nszjky.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://om.asd995.cn

[S41] C++：类与构造函数
来源：http://zu.gzmigu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fc.521024.cn

[S42] C++：继承与虚函数
来源：http://ks.chemitech.net.cn

class B : public Base { public: void f() override {} };
来源：http://kj.shxzukj.cn

[S43] C++：智能指针
来源：http://it.asd995.cn

auto p = std::make_unique<int>(5);
来源：http://bt.newstarts.cn

[S44] C++：引用传参
来源：http://tm.jianghongdianzi.cn

void inc(int &x) { ++x; }
来源：http://hb.9csxet.cn

[S45] C++：lambda
来源：http://yx.newstarts.cn

auto add = [](int a, int b) { return a + b; };
来源：http://yn.newstarts.cn

[S46] C++：函数模板
来源：http://gw.gzmigu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://us.shxzukj.cn

[S47] C++：结构化绑定遍历
来源：http://za.colortex.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jw.muxihuayi.cn

[S48] C++：逐行读文件
来源：http://oq.9csxet.cn

std::ifstream in("a.txt");  std::string line;
来源：http://iv.jctech888.com.cn

while (std::getline(in, line)) { }
来源：http://wx.hahajie.cn

[S49] C++：写文件
来源：http://ro.hahajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hg.hahajie.cn

[S50] C++：格式化数字
来源：http://vx.hahajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qy.panjiajie.cn

[S51] C++：显式类型转换
来源：http://oi.yuexingan06.cn

static_cast<double>(a) / b
来源：http://lu.hahajie.cn

[S52] C++：const 与 noexcept
来源：http://yi.szsharing.cn

int size() const noexcept { return n_; }
来源：http://zd.huixiangedu.cn

[S53] C++：移动语义
来源：http://gg.9csxet.cn

std::vector<int> w = std::move(v);
来源：http://gw.asd995.cn

[S54] C++：异常处理
来源：http://sd.gzmigu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xp.newstarts.cn

[S55] C++：结构化绑定
来源：http://ps.lnxyls.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xh.panjiajie.cn

[S56] C++：optional
来源：http://se.bookmarksfly.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hd.nicolike.cn

[S57] C++：编译期常量
来源：http://sw.szxytkj.cn

constexpr int N = 10;
来源：http://ya.asd995.cn

[S58] C++：命名空间
来源：http://ux.szsharing.cn

namespace ns { int f() { return 1; } }
来源：http://yq.bjjhwx.cn

[S59] C++：静态断言
来源：http://em.nicolike.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tm.colortex.cn

[S60] C++：遍历并删除元素
来源：http://mx.hahajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://op.wgjwhj.cn

================================================================================
来源：http://gn.panjiajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://we.newstarts.cn

================================================================================
来源：http://ey.nszjky.cn

[T01] Kotlin：Hello World
来源：http://dk.wgjwhj.cn

println("Hello")
来源：http://xi.szsharing.cn

[T02] Kotlin：变量
来源：http://zh.szsharing.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ss.gzmigu.cn

[T03] Kotlin：字符串模板
来源：http://at.chemitech.net.cn

"值: $b"
来源：http://tf.521024.cn

[T04] Kotlin：空安全
来源：http://tm.bookmarksfly.cn

val n: String? = null;  n?.length
来源：http://om.asd995.cn

[T05] Kotlin：when 表达式
来源：http://ln.huixiangedu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ub.haigaiapp.cn

[T06] Kotlin：集合映射
来源：http://hc.nszjky.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://cv.szsharing.cn

[T07] Kotlin：集合过滤
来源：http://nv.shxzukj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://mt.asd995.cn

[T08] Kotlin：数据类
来源：http://ut.shxzskj.cn

data class User(val name: String, val age: Int)
来源：http://cv.colortex.cn

[T09] Kotlin：扩展函数
来源：http://dh.jianghongdianzi.cn

fun String.exclaim() = this + "!"
来源：http://ie.asd995.cn

[T10] Kotlin：默认参数
来源：http://jb.yuexingan06.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ot.szxytkj.cn

[T11] Kotlin：协程
来源：http://gv.szxytkj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://dc.huanxung.cn

[T12] Kotlin：解构声明
来源：http://zm.shxzukj.cn

val (a, b) = Pair(1, 2)
来源：http://em.bjjhwx.cn

[T13] Kotlin：只读 Map
来源：http://dl.9csxet.cn

val m = mapOf("a" to 1)
来源：http://wt.hahajie.cn

[T14] Kotlin：循环
来源：http://yy.huixinmuqiang.cn

for (i in 1..10) println(i)
来源：http://yo.yuexingan06.cn

[T15] Kotlin：接口
来源：http://us.nszjky.cn

interface Shape { fun area(): Double }
来源：http://pz.9csxet.cn

[T16] Swift：Hello World
来源：http://ks.nicolike.cn

print("Hello")
来源：http://lh.muxihuayi.cn

[T17] Swift：变量与常量
来源：http://cu.bjjhwx.cn

var a = 1;  let b = 2
来源：http://rw.hnjuh.cn

[T18] Swift：字符串插值
来源：http://ye.wgjwhj.cn

"值: \(b)"
来源：http://gx.yuntaijiaju.cn

[T19] Swift：可选绑定
来源：http://jg.szsharing.cn

if let n = opt { print(n) }
来源：http://ys.hnjuh.cn

[T20] Swift：数组操作
来源：http://ke.gzmigu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ap.shtwfgs.cn

[T21] Swift：遍历
来源：http://he.jianghongdianzi.cn

for x in a { print(x) }
来源：http://aq.nszjky.cn

[T22] Swift：字典
来源：http://dv.shtwfgs.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mm.huanxung.cn

[T23] Swift：函数
来源：http://zg.hahajie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uq.shxzskj.cn

[T24] Swift：闭包
来源：http://zb.shxzskj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://dq.huixiangedu.cn

[T25] Swift：结构体
来源：http://yt.hnjuh.cn

struct P { var x: Int }
来源：http://ew.521024.cn

[T26] Swift：类与重写
来源：http://sd.chemitech.net.cn

class A: Base { override func f() {} }
来源：http://nd.yuexingan06.cn

[T27] Swift：错误处理
来源：http://og.shtwfgs.cn

do { try f() } catch { print(error) }
来源：http://aj.chemitech.net.cn

[T28] Swift：枚举
来源：http://xd.chemitech.net.cn

enum Color { case red, green }
来源：http://nn.wgjwhj.cn

[T29] Swift：guard 提前返回
来源：http://uk.szsharing.cn

guard let x = opt else { return }
来源：http://ob.jianghongdianzi.cn

[T30] Swift：协议
来源：http://dv.nicolike.cn

protocol Shape { func area() -> Double }
来源：http://lk.bookmarksfly.cn

[T31] Lua：Hello World
来源：http://kq.huixinmuqiang.cn

print("Hello")
来源：http://py.wgjwhj.cn

[T32] Lua：局部变量
来源：http://rx.shtwfgs.cn

local a = 1
来源：http://rv.muxihuayi.cn

[T33] Lua：表（数组）
来源：http://ow.szsharing.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://qy.nszjky.cn

[T34] Lua：遍历表
来源：http://uo.szxytkj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gv.yuexingan06.cn

[T35] Lua：字典表
来源：http://dt.jianghongdianzi.cn

local d = { a = 1 };  d.b = 2
来源：http://ug.hahajie.cn

[T36] Lua：函数
来源：http://do.huanxung.cn

function add(a, b) return a + b end
来源：http://xo.bjjhwx.cn

[T37] Lua：字符串拼接
来源：http://bx.shxzukj.cn

"a" .. "b"
来源：http://bm.chemitech.net.cn

[T38] Lua：条件
来源：http://yu.panjiajie.cn

if x > 0 then print("正") end
来源：http://gd.panjiajie.cn

[T39] Lua：模式匹配
来源：http://gq.huixiangedu.cn

string.find(s, "%d+")
来源：http://xc.hnjuh.cn

[T40] Lua：元表
来源：http://pt.wgjwhj.cn

setmetatable({}, { __index = base })
来源：http://ti.wgjwhj.cn

[T41] Perl：Hello World
来源：http://je.panjiajie.cn

print "Hello\n";
来源：http://be.521024.cn

[T42] Perl：变量类型
来源：http://ij.nicolike.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ih.asd995.cn

[T43] Perl：字符串插值
来源：http://oj.panjiajie.cn

"值: $a"
来源：http://zg.bookmarksfly.cn

[T44] Perl：条件
来源：http://cl.yuexingan06.cn

if ($a > 0) { print "正"; }
来源：http://pl.chemitech.net.cn

[T45] Perl：数组遍历
来源：http://ve.nicolike.cn

for my $x (@arr) { print $x; }
来源：http://sz.lnxyls.cn

[T46] Perl：哈希操作
来源：http://hy.gzmigu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ph.521024.cn

[T47] Perl：正则捕获
来源：http://am.shtwfgs.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ku.yuexingan06.cn

[T48] Perl：正则替换
来源：http://ky.9csxet.cn

$s =~ s/old/new/g;
来源：http://qd.newstarts.cn

[T49] Perl：函数
来源：http://dy.yuntaijiaju.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://om.9csxet.cn

[T50] Perl：逐行读文件
来源：http://dv.chemitech.net.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://gv.lnxyls.cn

while (my $line = <$fh>) { print $line; }
来源：http://sy.9csxet.cn

[T51] Scala：Hello World
来源：http://ig.chemitech.net.cn

println("Hello")
来源：http://mr.shxzskj.cn

[T52] Scala：变量
来源：http://tl.shxzukj.cn

val a = 1;  var b = 2
来源：http://aj.hahajie.cn

[T53] Scala：字符串插值
来源：http://gu.huixiangedu.cn

s"值: $b"
来源：http://zk.panjiajie.cn

[T54] Scala：集合映射
来源：http://ob.szxytkj.cn

List(1, 2, 3).map(_ * 2)
来源：http://cm.panjiajie.cn

[T55] Scala：集合过滤
来源：http://ld.muxihuayi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://oj.jianghongdianzi.cn

[T56] Scala：样例类
来源：http://sn.nszjky.cn

case class User(name: String, age: Int)
来源：http://zn.521024.cn

[T57] Scala：模式匹配
来源：http://sd.bookmarksfly.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wk.hahajie.cn

[T58] Scala：函数定义
来源：http://uk.jctech888.com.cn

def add(a: Int, b: Int): Int = a + b
来源：http://vz.shxzskj.cn

[T59] Scala：循环
来源：http://mt.szsharing.cn

for (i <- 1 to 10) println(i)
来源：http://lz.newstarts.cn

[T60] Scala：折叠
来源：http://zc.jctech888.com.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zi.bookmarksfly.cn

================================================================================
来源：http://ww.shxzskj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dx.muxihuayi.cn

================================================================================
来源：http://ka.panjiajie.cn

[U01] Py：创建虚拟环境
来源：http://rf.shxzukj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://uh.yuntaijiaju.cn

[U02] Py：导出 / 安装依赖
来源：http://uk.521024.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zn.chemitech.net.cn

[U03] Py：加载 .env 配置
来源：http://xa.9csxet.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://mg.lnxyls.cn

[U04] Py：变量调试打印
来源：http://cw.521024.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fw.szxytkj.cn

[U05] Py：列表去重且保序
来源：http://cd.huanxung.cn

list(dict.fromkeys(arr))
来源：http://vi.chemitech.net.cn

[U06] Py：合并两个字典
来源：http://vg.nicolike.cn

{**a, **b}
来源：http://fc.nszjky.cn

[U07] Py：反转字典键值
来源：http://jq.9csxet.cn

{v: k for k, v in d.items()}
来源：http://lp.bjjhwx.cn

[U08] Py：展平二维列表
来源：http://rc.colortex.cn

[y for x in nested for y in x]
来源：http://zb.newstarts.cn

[U09] Py：字典取最大值的键
来源：http://yd.huanxung.cn

max(d, key=d.get)
来源：http://yz.szxytkj.cn

[U10] Py：按值排序字典
来源：http://ji.hahajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dv.chemitech.net.cn

[U11] Py：生成器表达式
来源：http://bc.shxzukj.cn

(x * 2 for x in arr)
来源：http://tp.shtwfgs.cn

[U12] Py：取出现最多的 3 个元素
来源：http://oe.panjiajie.cn

Counter(arr).most_common(3)
来源：http://nl.nszjky.cn

[U13] Py：固定长度队列
来源：http://re.nszjky.cn

deque(maxlen=10)
来源：http://au.521024.cn

[U14] Py：分组收集到列表
来源：http://uh.haigaiapp.cn

defaultdict(list)
来源：http://zp.huixiangedu.cn

[U15] Py：高精度计时
来源：http://ll.hnjuh.cn

t = time.perf_counter()
来源：http://om.muxihuayi.cn

[U16] Py：命令行参数解析
来源：http://nx.hnjuh.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jq.bjjhwx.cn

[U17] Py：初始化日志
来源：http://vx.shtwfgs.cn

logging.basicConfig(level=logging.INFO)
来源：http://ht.bookmarksfly.cn

[U18] Py：预编译正则
来源：http://tj.jianghongdianzi.cn

pat = re.compile(r"\d+")
来源：http://om.muxihuayi.cn

[U19] Py：正则替换带回调
来源：http://fz.hnjuh.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ec.newstarts.cn

[U20] Py：缓存函数结果
来源：http://th.521024.cn

@functools.lru_cache(maxsize=None)
来源：http://xf.panjiajie.cn

[U21] Py：自定义上下文管理器
来源：http://zd.asd995.cn

@contextlib.contextmanager
来源：http://tv.haigaiapp.cn

[U22] Py：矩阵转置
来源：http://kq.jctech888.com.cn

list(zip(*m))
来源：http://ag.szxytkj.cn

[U23] Py：分块读取大文件
来源：http://bd.gzmigu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pi.nicolike.cn

[U24] Py：路径操作
来源：http://dt.nicolike.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zx.szsharing.cn

[U25] Py：CSV 按字典读
来源：http://sg.jctech888.com.cn

csv.DictReader(f)
来源：http://fo.hnjuh.cn

[U26] Py：并发下载
来源：http://he.newstarts.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dz.szsharing.cn


<!-- 参考信息 -->