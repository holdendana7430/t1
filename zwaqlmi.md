代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://xt.huanxung.cn

[S02] C：变量与格式化输出
来源：http://mf.9csxet.cn

int a = 10; printf("%d\n", a);
来源：http://gc.yuntaijiaju.cn

[S03] C：读入整数
来源：http://lc.shxzskj.cn

int x; scanf("%d", &x);
来源：http://ac.huixiangedu.cn

[S04] C：字符串复制
来源：http://xv.szsharing.cn

char dst[32]; strcpy(dst, "hi");
来源：http://bp.nicolike.cn

[S05] C：字符串长度
来源：http://xu.jctech888.com.cn

strlen(s)
来源：http://yb.hnjuh.cn

[S06] C：字符串比较
来源：http://ee.huixinmuqiang.cn

strcmp(a, b) == 0
来源：http://xc.shxzukj.cn

[S07] C：数组遍历求和
来源：http://np.jctech888.com.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sp.hnjuh.cn

[S08] C：动态内存分配与释放
来源：http://wz.bjjhwx.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://oy.shxzukj.cn

[S09] C：结构体定义与初始化
来源：http://ss.jctech888.com.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jl.shxzukj.cn

[S10] C：指针与解引用
来源：http://pt.521024.cn

int *p = &a;  *p = 5;
来源：http://tu.panjiajie.cn

[S11] C：逐行读文件
来源：http://hc.chemitech.net.cn

FILE *f = fopen("a.txt", "r");
来源：http://fr.yuexingan06.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://de.yuntaijiaju.cn

fclose(f);
来源：http://jh.gzmigu.cn

[S12] C：写文件
来源：http://ik.huanxung.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bt.hahajie.cn

[S13] C：宏定义
来源：http://hp.yuntaijiaju.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dz.jianghongdianzi.cn

[S14] C：枚举
来源：http://ht.bjjhwx.cn

enum Color { RED, GREEN, BLUE };
来源：http://fv.szsharing.cn

[S15] C：类型转换
来源：http://lo.gzmigu.cn

(double) a / b
来源：http://og.9csxet.cn

[S16] C：位操作置位
来源：http://pa.newstarts.cn

x |= (1 << 3);
来源：http://qu.gzmigu.cn

[S17] C：安全拼接字符串
来源：http://xg.panjiajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zq.shxzskj.cn

[S18] C：命令行参数
来源：http://ml.huanxung.cn

int main(int argc, char **argv)
来源：http://vz.wgjwhj.cn

[S19] C：快速排序
来源：http://kp.shxzskj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://or.bookmarksfly.cn

[S20] C：二分查找
来源：http://jz.shtwfgs.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xi.chemitech.net.cn

[S21] C：字符类别判断
来源：http://bj.shxzukj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cj.panjiajie.cn

[S22] C：字符串转数字
来源：http://wk.nicolike.cn

atoi("42");  strtod("3.14", NULL);
来源：http://hx.muxihuayi.cn

[S23] C：随机数
来源：http://xw.shtwfgs.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://yc.huixinmuqiang.cn

[S24] C：获取本地时间
来源：http://ua.jianghongdianzi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dc.jianghongdianzi.cn

[S25] C：内存拷贝
来源：http://qo.521024.cn

memcpy(dst, src, n);
来源：http://bq.huixiangedu.cn

[S26] C：内存清零
来源：http://hk.shxzukj.cn

memset(a, 0, sizeof a);
来源：http://wr.asd995.cn

[S27] C：定义常量
来源：http://bp.9csxet.cn

const double PI = 3.14159;
来源：http://tv.bjjhwx.cn

[S28] C：静态变量
来源：http://hw.huixinmuqiang.cn

static int counter = 0;
来源：http://tu.lnxyls.cn

[S29] C：变参函数
来源：http://jw.jctech888.com.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ki.yuexingan06.cn

[S30] C：头文件保护
来源：http://mf.nszjky.cn

#ifndef X_H
来源：http://wa.lnxyls.cn

#define X_H
来源：http://sx.shtwfgs.cn

#endif
来源：http://qc.nszjky.cn

[S31] C++：Hello World
来源：http://ik.wgjwhj.cn

#include <iostream>
来源：http://kc.521024.cn

int main() { std::cout << "Hello\n"; }
来源：http://pv.nszjky.cn

[S32] C++：字符串
来源：http://eh.wgjwhj.cn

std::string s = "hi";  s += "!";
来源：http://jb.jianghongdianzi.cn

[S33] C++：vector 增删
来源：http://xp.muxihuayi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ty.nicolike.cn

[S34] C++：遍历 vector
来源：http://jr.nicolike.cn

for (auto &x : v) { std::cout << x; }
来源：http://ao.shxzskj.cn

[S35] C++：map
来源：http://sm.szxytkj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ki.huixinmuqiang.cn

[S36] C++：unordered_map
来源：http://sz.jctech888.com.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cj.colortex.cn

[S37] C++：set
来源：http://vx.shxzukj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ty.nicolike.cn

[S38] C++：排序
来源：http://yc.shtwfgs.cn

std::sort(v.begin(), v.end());
来源：http://qe.hnjuh.cn

[S39] C++：自定义比较器排序
来源：http://ch.szsharing.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rx.szxytkj.cn

[S40] C++：查找元素
来源：http://ed.huixiangedu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fq.hnjuh.cn

[S41] C++：类与构造函数
来源：http://eb.huanxung.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yu.bookmarksfly.cn

[S42] C++：继承与虚函数
来源：http://ss.panjiajie.cn

class B : public Base { public: void f() override {} };
来源：http://te.haigaiapp.cn

[S43] C++：智能指针
来源：http://ek.chemitech.net.cn

auto p = std::make_unique<int>(5);
来源：http://gn.huixiangedu.cn

[S44] C++：引用传参
来源：http://br.9csxet.cn

void inc(int &x) { ++x; }
来源：http://ev.hahajie.cn

[S45] C++：lambda
来源：http://pn.521024.cn

auto add = [](int a, int b) { return a + b; };
来源：http://er.newstarts.cn

[S46] C++：函数模板
来源：http://hx.wgjwhj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ka.huixinmuqiang.cn

[S47] C++：结构化绑定遍历
来源：http://yi.shxzskj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ed.hnjuh.cn

[S48] C++：逐行读文件
来源：http://or.huanxung.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xy.newstarts.cn

while (std::getline(in, line)) { }
来源：http://mo.9csxet.cn

[S49] C++：写文件
来源：http://nx.bookmarksfly.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ay.nszjky.cn

[S50] C++：格式化数字
来源：http://ew.gzmigu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://au.wgjwhj.cn

[S51] C++：显式类型转换
来源：http://cq.huanxung.cn

static_cast<double>(a) / b
来源：http://uz.nszjky.cn

[S52] C++：const 与 noexcept
来源：http://hv.huixiangedu.cn

int size() const noexcept { return n_; }
来源：http://oo.huixiangedu.cn

[S53] C++：移动语义
来源：http://pc.jctech888.com.cn

std::vector<int> w = std::move(v);
来源：http://jg.jctech888.com.cn

[S54] C++：异常处理
来源：http://nh.9csxet.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gc.yuexingan06.cn

[S55] C++：结构化绑定
来源：http://ct.chemitech.net.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zs.yuntaijiaju.cn

[S56] C++：optional
来源：http://vw.9csxet.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://py.shtwfgs.cn

[S57] C++：编译期常量
来源：http://tp.bookmarksfly.cn

constexpr int N = 10;
来源：http://si.nszjky.cn

[S58] C++：命名空间
来源：http://pa.jctech888.com.cn

namespace ns { int f() { return 1; } }
来源：http://uv.newstarts.cn

[S59] C++：静态断言
来源：http://is.521024.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://af.nicolike.cn

[S60] C++：遍历并删除元素
来源：http://uv.shtwfgs.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bp.szsharing.cn

================================================================================
来源：http://xp.huanxung.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://li.haigaiapp.cn

================================================================================
来源：http://gp.gzmigu.cn

[T01] Kotlin：Hello World
来源：http://ju.nicolike.cn

println("Hello")
来源：http://ih.huanxung.cn

[T02] Kotlin：变量
来源：http://kw.asd995.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xs.chemitech.net.cn

[T03] Kotlin：字符串模板
来源：http://as.muxihuayi.cn

"值: $b"
来源：http://by.shxzskj.cn

[T04] Kotlin：空安全
来源：http://eu.nszjky.cn

val n: String? = null;  n?.length
来源：http://wx.nicolike.cn

[T05] Kotlin：when 表达式
来源：http://kt.shtwfgs.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dd.yuntaijiaju.cn

[T06] Kotlin：集合映射
来源：http://sv.asd995.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://sv.9csxet.cn

[T07] Kotlin：集合过滤
来源：http://wi.muxihuayi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tp.hahajie.cn

[T08] Kotlin：数据类
来源：http://fy.hnjuh.cn

data class User(val name: String, val age: Int)
来源：http://nu.521024.cn

[T09] Kotlin：扩展函数
来源：http://fk.yuntaijiaju.cn

fun String.exclaim() = this + "!"
来源：http://pl.yuexingan06.cn

[T10] Kotlin：默认参数
来源：http://kw.yuntaijiaju.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://yp.shtwfgs.cn

[T11] Kotlin：协程
来源：http://ck.wgjwhj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://kw.jctech888.com.cn

[T12] Kotlin：解构声明
来源：http://et.asd995.cn

val (a, b) = Pair(1, 2)
来源：http://uo.521024.cn

[T13] Kotlin：只读 Map
来源：http://an.szxytkj.cn

val m = mapOf("a" to 1)
来源：http://jf.gzmigu.cn

[T14] Kotlin：循环
来源：http://nf.yuntaijiaju.cn

for (i in 1..10) println(i)
来源：http://ap.hnjuh.cn

[T15] Kotlin：接口
来源：http://qt.jianghongdianzi.cn

interface Shape { fun area(): Double }
来源：http://ul.nicolike.cn

[T16] Swift：Hello World
来源：http://vp.bjjhwx.cn

print("Hello")
来源：http://mn.haigaiapp.cn

[T17] Swift：变量与常量
来源：http://gj.hnjuh.cn

var a = 1;  let b = 2
来源：http://if.haigaiapp.cn

[T18] Swift：字符串插值
来源：http://ql.yuexingan06.cn

"值: \(b)"
来源：http://pt.wgjwhj.cn

[T19] Swift：可选绑定
来源：http://ws.chemitech.net.cn

if let n = opt { print(n) }
来源：http://om.nszjky.cn

[T20] Swift：数组操作
来源：http://yd.bjjhwx.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fn.panjiajie.cn

[T21] Swift：遍历
来源：http://yx.colortex.cn

for x in a { print(x) }
来源：http://bj.szxytkj.cn

[T22] Swift：字典
来源：http://zb.szsharing.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xl.9csxet.cn

[T23] Swift：函数
来源：http://fh.colortex.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cl.asd995.cn

[T24] Swift：闭包
来源：http://ac.haigaiapp.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://tl.shtwfgs.cn

[T25] Swift：结构体
来源：http://vx.hahajie.cn

struct P { var x: Int }
来源：http://mt.nicolike.cn

[T26] Swift：类与重写
来源：http://rs.wgjwhj.cn

class A: Base { override func f() {} }
来源：http://fc.shtwfgs.cn

[T27] Swift：错误处理
来源：http://tn.9csxet.cn

do { try f() } catch { print(error) }
来源：http://ck.bjjhwx.cn

[T28] Swift：枚举
来源：http://rj.bjjhwx.cn

enum Color { case red, green }
来源：http://ny.panjiajie.cn

[T29] Swift：guard 提前返回
来源：http://sf.huixinmuqiang.cn

guard let x = opt else { return }
来源：http://gd.nicolike.cn

[T30] Swift：协议
来源：http://eg.nszjky.cn

protocol Shape { func area() -> Double }
来源：http://hh.nicolike.cn

[T31] Lua：Hello World
来源：http://jj.hahajie.cn

print("Hello")
来源：http://cq.asd995.cn

[T32] Lua：局部变量
来源：http://zq.hahajie.cn

local a = 1
来源：http://ef.jianghongdianzi.cn

[T33] Lua：表（数组）
来源：http://cv.huixiangedu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vz.huixinmuqiang.cn

[T34] Lua：遍历表
来源：http://ou.muxihuayi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://on.panjiajie.cn

[T35] Lua：字典表
来源：http://vj.lnxyls.cn

local d = { a = 1 };  d.b = 2
来源：http://gr.gzmigu.cn

[T36] Lua：函数
来源：http://uw.hahajie.cn

function add(a, b) return a + b end
来源：http://qx.asd995.cn

[T37] Lua：字符串拼接
来源：http://ih.hnjuh.cn

"a" .. "b"
来源：http://zo.newstarts.cn

[T38] Lua：条件
来源：http://yx.nszjky.cn

if x > 0 then print("正") end
来源：http://qp.chemitech.net.cn

[T39] Lua：模式匹配
来源：http://gu.521024.cn

string.find(s, "%d+")
来源：http://uj.chemitech.net.cn

[T40] Lua：元表
来源：http://kx.shxzskj.cn

setmetatable({}, { __index = base })
来源：http://re.huixinmuqiang.cn

[T41] Perl：Hello World
来源：http://is.szsharing.cn

print "Hello\n";
来源：http://gp.hnjuh.cn

[T42] Perl：变量类型
来源：http://fg.muxihuayi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yu.jianghongdianzi.cn

[T43] Perl：字符串插值
来源：http://hc.wgjwhj.cn

"值: $a"
来源：http://az.jctech888.com.cn

[T44] Perl：条件
来源：http://gg.jctech888.com.cn

if ($a > 0) { print "正"; }
来源：http://zi.gzmigu.cn

[T45] Perl：数组遍历
来源：http://ng.jctech888.com.cn

for my $x (@arr) { print $x; }
来源：http://hb.huixiangedu.cn

[T46] Perl：哈希操作
来源：http://xl.wgjwhj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vp.huanxung.cn

[T47] Perl：正则捕获
来源：http://ch.colortex.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vg.gzmigu.cn

[T48] Perl：正则替换
来源：http://jy.bookmarksfly.cn

$s =~ s/old/new/g;
来源：http://fh.szxytkj.cn

[T49] Perl：函数
来源：http://va.shtwfgs.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cr.jctech888.com.cn

[T50] Perl：逐行读文件
来源：http://tp.shxzukj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://at.yuexingan06.cn

while (my $line = <$fh>) { print $line; }
来源：http://jk.shxzskj.cn

[T51] Scala：Hello World
来源：http://ld.gzmigu.cn

println("Hello")
来源：http://vr.shxzukj.cn

[T52] Scala：变量
来源：http://nn.bookmarksfly.cn

val a = 1;  var b = 2
来源：http://bu.yuntaijiaju.cn

[T53] Scala：字符串插值
来源：http://an.szxytkj.cn

s"值: $b"
来源：http://aa.yuexingan06.cn

[T54] Scala：集合映射
来源：http://by.shxzskj.cn

List(1, 2, 3).map(_ * 2)
来源：http://sk.huanxung.cn

[T55] Scala：集合过滤
来源：http://px.521024.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fw.9csxet.cn

[T56] Scala：样例类
来源：http://zp.shxzskj.cn

case class User(name: String, age: Int)
来源：http://rz.nszjky.cn

[T57] Scala：模式匹配
来源：http://hh.lnxyls.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://bf.jctech888.com.cn

[T58] Scala：函数定义
来源：http://jv.jianghongdianzi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fa.lnxyls.cn

[T59] Scala：循环
来源：http://pu.huixinmuqiang.cn

for (i <- 1 to 10) println(i)
来源：http://ia.szxytkj.cn

[T60] Scala：折叠
来源：http://uw.haigaiapp.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pf.colortex.cn

================================================================================
来源：http://eb.shxzukj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://oi.huixiangedu.cn

================================================================================
来源：http://sn.szsharing.cn

[U01] Py：创建虚拟环境
来源：http://dl.9csxet.cn

python -m venv .venv && source .venv/bin/activate
来源：http://pa.szsharing.cn

[U02] Py：导出 / 安装依赖
来源：http://ly.nicolike.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fb.shtwfgs.cn

[U03] Py：加载 .env 配置
来源：http://ac.shtwfgs.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://pz.nszjky.cn

[U04] Py：变量调试打印
来源：http://hs.bjjhwx.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jr.shxzukj.cn

[U05] Py：列表去重且保序
来源：http://mi.huixiangedu.cn

list(dict.fromkeys(arr))
来源：http://fq.gzmigu.cn

[U06] Py：合并两个字典
来源：http://bx.jctech888.com.cn

{**a, **b}
来源：http://ov.szsharing.cn

[U07] Py：反转字典键值
来源：http://jv.huanxung.cn

{v: k for k, v in d.items()}
来源：http://us.yuexingan06.cn

[U08] Py：展平二维列表
来源：http://bj.hnjuh.cn

[y for x in nested for y in x]
来源：http://ct.nicolike.cn

[U09] Py：字典取最大值的键
来源：http://cw.jctech888.com.cn

max(d, key=d.get)
来源：http://kf.wgjwhj.cn

[U10] Py：按值排序字典
来源：http://xq.521024.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ln.yuntaijiaju.cn

[U11] Py：生成器表达式
来源：http://wi.huixinmuqiang.cn

(x * 2 for x in arr)
来源：http://dm.wgjwhj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://eu.nicolike.cn

Counter(arr).most_common(3)
来源：http://pa.lnxyls.cn

[U13] Py：固定长度队列
来源：http://qy.hahajie.cn

deque(maxlen=10)
来源：http://ga.muxihuayi.cn

[U14] Py：分组收集到列表
来源：http://vm.haigaiapp.cn

defaultdict(list)
来源：http://lt.huixinmuqiang.cn

[U15] Py：高精度计时
来源：http://lk.haigaiapp.cn

t = time.perf_counter()
来源：http://to.shtwfgs.cn

[U16] Py：命令行参数解析
来源：http://nn.haigaiapp.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gg.jianghongdianzi.cn

[U17] Py：初始化日志
来源：http://bx.bjjhwx.cn

logging.basicConfig(level=logging.INFO)
来源：http://kg.gzmigu.cn

[U18] Py：预编译正则
来源：http://qn.hahajie.cn

pat = re.compile(r"\d+")
来源：http://je.newstarts.cn

[U19] Py：正则替换带回调
来源：http://iu.muxihuayi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yk.hnjuh.cn

[U20] Py：缓存函数结果
来源：http://kz.huixiangedu.cn

@functools.lru_cache(maxsize=None)
来源：http://gg.chemitech.net.cn

[U21] Py：自定义上下文管理器
来源：http://ku.szsharing.cn

@contextlib.contextmanager
来源：http://yz.jianghongdianzi.cn

[U22] Py：矩阵转置
来源：http://ss.asd995.cn

list(zip(*m))
来源：http://ny.huixiangedu.cn

[U23] Py：分块读取大文件
来源：http://ih.bookmarksfly.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://em.gzmigu.cn

[U24] Py：路径操作
来源：http://kf.shtwfgs.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://aw.panjiajie.cn


<!-- 参考信息 -->