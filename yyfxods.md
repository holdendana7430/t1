代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://ox.nicolike.cn

[S02] C：变量与格式化输出
来源：http://bh.9csxet.cn

int a = 10; printf("%d\n", a);
来源：http://iw.panjiajie.cn

[S03] C：读入整数
来源：http://ga.haigaiapp.cn

int x; scanf("%d", &x);
来源：http://jd.yuexingan06.cn

[S04] C：字符串复制
来源：http://ko.yuntaijiaju.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ag.haigaiapp.cn

[S05] C：字符串长度
来源：http://vm.jctech888.com.cn

strlen(s)
来源：http://gm.lnxyls.cn

[S06] C：字符串比较
来源：http://nb.shxzskj.cn

strcmp(a, b) == 0
来源：http://ca.yuntaijiaju.cn

[S07] C：数组遍历求和
来源：http://ra.haigaiapp.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sl.panjiajie.cn

[S08] C：动态内存分配与释放
来源：http://sm.521024.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gw.bookmarksfly.cn

[S09] C：结构体定义与初始化
来源：http://gs.wgjwhj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fr.lnxyls.cn

[S10] C：指针与解引用
来源：http://rn.colortex.cn

int *p = &a;  *p = 5;
来源：http://mt.asd995.cn

[S11] C：逐行读文件
来源：http://sa.nszjky.cn

FILE *f = fopen("a.txt", "r");
来源：http://dd.jctech888.com.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ql.nszjky.cn

fclose(f);
来源：http://hw.wgjwhj.cn

[S12] C：写文件
来源：http://ez.haigaiapp.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gw.gzmigu.cn

[S13] C：宏定义
来源：http://xd.hahajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jp.huixiangedu.cn

[S14] C：枚举
来源：http://bw.haigaiapp.cn

enum Color { RED, GREEN, BLUE };
来源：http://ie.lnxyls.cn

[S15] C：类型转换
来源：http://nt.hnjuh.cn

(double) a / b
来源：http://fh.yuntaijiaju.cn

[S16] C：位操作置位
来源：http://hu.shtwfgs.cn

x |= (1 << 3);
来源：http://jt.chemitech.net.cn

[S17] C：安全拼接字符串
来源：http://en.shxzskj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nz.jctech888.com.cn

[S18] C：命令行参数
来源：http://cc.szsharing.cn

int main(int argc, char **argv)
来源：http://fn.hnjuh.cn

[S19] C：快速排序
来源：http://pu.chemitech.net.cn

qsort(a, n, sizeof(int), cmp);
来源：http://sd.wgjwhj.cn

[S20] C：二分查找
来源：http://pq.huixiangedu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jd.jianghongdianzi.cn

[S21] C：字符类别判断
来源：http://aw.asd995.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jk.muxihuayi.cn

[S22] C：字符串转数字
来源：http://gm.colortex.cn

atoi("42");  strtod("3.14", NULL);
来源：http://zt.chemitech.net.cn

[S23] C：随机数
来源：http://pb.yuexingan06.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vs.gzmigu.cn

[S24] C：获取本地时间
来源：http://nb.jctech888.com.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cc.szxytkj.cn

[S25] C：内存拷贝
来源：http://pc.bjjhwx.cn

memcpy(dst, src, n);
来源：http://lq.colortex.cn

[S26] C：内存清零
来源：http://sf.colortex.cn

memset(a, 0, sizeof a);
来源：http://dr.huixiangedu.cn

[S27] C：定义常量
来源：http://ux.chemitech.net.cn

const double PI = 3.14159;
来源：http://bb.wgjwhj.cn

[S28] C：静态变量
来源：http://ey.muxihuayi.cn

static int counter = 0;
来源：http://zu.wgjwhj.cn

[S29] C：变参函数
来源：http://qi.nicolike.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bk.panjiajie.cn

[S30] C：头文件保护
来源：http://kf.nicolike.cn

#ifndef X_H
来源：http://nr.jianghongdianzi.cn

#define X_H
来源：http://nv.szxytkj.cn

#endif
来源：http://pm.chemitech.net.cn

[S31] C++：Hello World
来源：http://bj.lnxyls.cn

#include <iostream>
来源：http://el.yuexingan06.cn

int main() { std::cout << "Hello\n"; }
来源：http://na.newstarts.cn

[S32] C++：字符串
来源：http://ps.szsharing.cn

std::string s = "hi";  s += "!";
来源：http://du.huixinmuqiang.cn

[S33] C++：vector 增删
来源：http://zz.shtwfgs.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qi.bookmarksfly.cn

[S34] C++：遍历 vector
来源：http://ae.chemitech.net.cn

for (auto &x : v) { std::cout << x; }
来源：http://jm.panjiajie.cn

[S35] C++：map
来源：http://lv.yuntaijiaju.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wa.huanxung.cn

[S36] C++：unordered_map
来源：http://kf.muxihuayi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bg.shxzukj.cn

[S37] C++：set
来源：http://go.szsharing.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ci.nszjky.cn

[S38] C++：排序
来源：http://lc.huixiangedu.cn

std::sort(v.begin(), v.end());
来源：http://jf.nicolike.cn

[S39] C++：自定义比较器排序
来源：http://ar.yuntaijiaju.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sn.shtwfgs.cn

[S40] C++：查找元素
来源：http://fm.huixinmuqiang.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lj.huixiangedu.cn

[S41] C++：类与构造函数
来源：http://qt.yuntaijiaju.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ej.gzmigu.cn

[S42] C++：继承与虚函数
来源：http://eg.colortex.cn

class B : public Base { public: void f() override {} };
来源：http://ld.huixinmuqiang.cn

[S43] C++：智能指针
来源：http://rl.asd995.cn

auto p = std::make_unique<int>(5);
来源：http://vr.9csxet.cn

[S44] C++：引用传参
来源：http://nc.jianghongdianzi.cn

void inc(int &x) { ++x; }
来源：http://je.huixinmuqiang.cn

[S45] C++：lambda
来源：http://lb.asd995.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zy.yuntaijiaju.cn

[S46] C++：函数模板
来源：http://cz.bookmarksfly.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lj.nszjky.cn

[S47] C++：结构化绑定遍历
来源：http://cj.yuexingan06.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ly.shxzukj.cn

[S48] C++：逐行读文件
来源：http://nv.jianghongdianzi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ct.panjiajie.cn

while (std::getline(in, line)) { }
来源：http://dl.asd995.cn

[S49] C++：写文件
来源：http://ql.nicolike.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yz.colortex.cn

[S50] C++：格式化数字
来源：http://vk.chemitech.net.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hk.yuexingan06.cn

[S51] C++：显式类型转换
来源：http://ob.muxihuayi.cn

static_cast<double>(a) / b
来源：http://os.huixinmuqiang.cn

[S52] C++：const 与 noexcept
来源：http://oj.haigaiapp.cn

int size() const noexcept { return n_; }
来源：http://zc.gzmigu.cn

[S53] C++：移动语义
来源：http://sp.asd995.cn

std::vector<int> w = std::move(v);
来源：http://dg.jianghongdianzi.cn

[S54] C++：异常处理
来源：http://pj.nszjky.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yf.panjiajie.cn

[S55] C++：结构化绑定
来源：http://wh.bookmarksfly.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://aa.yuexingan06.cn

[S56] C++：optional
来源：http://fs.chemitech.net.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qt.wgjwhj.cn

[S57] C++：编译期常量
来源：http://qm.huixinmuqiang.cn

constexpr int N = 10;
来源：http://oe.521024.cn

[S58] C++：命名空间
来源：http://uh.nicolike.cn

namespace ns { int f() { return 1; } }
来源：http://vd.huanxung.cn

[S59] C++：静态断言
来源：http://lp.yuntaijiaju.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ga.chemitech.net.cn

[S60] C++：遍历并删除元素
来源：http://sz.colortex.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pt.colortex.cn

================================================================================
来源：http://zh.nicolike.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kg.shxzskj.cn

================================================================================
来源：http://bl.bookmarksfly.cn

[T01] Kotlin：Hello World
来源：http://ck.shtwfgs.cn

println("Hello")
来源：http://hd.chemitech.net.cn

[T02] Kotlin：变量
来源：http://op.newstarts.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://oa.hnjuh.cn

[T03] Kotlin：字符串模板
来源：http://go.jctech888.com.cn

"值: $b"
来源：http://rl.hnjuh.cn

[T04] Kotlin：空安全
来源：http://xa.colortex.cn

val n: String? = null;  n?.length
来源：http://yg.szxytkj.cn

[T05] Kotlin：when 表达式
来源：http://wi.szsharing.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mt.nicolike.cn

[T06] Kotlin：集合映射
来源：http://oz.shxzskj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://sg.9csxet.cn

[T07] Kotlin：集合过滤
来源：http://ij.nszjky.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pa.huixiangedu.cn

[T08] Kotlin：数据类
来源：http://ix.chemitech.net.cn

data class User(val name: String, val age: Int)
来源：http://ou.jianghongdianzi.cn

[T09] Kotlin：扩展函数
来源：http://uk.yuexingan06.cn

fun String.exclaim() = this + "!"
来源：http://cy.chemitech.net.cn

[T10] Kotlin：默认参数
来源：http://ja.panjiajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://uu.9csxet.cn

[T11] Kotlin：协程
来源：http://ff.szxytkj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://og.521024.cn

[T12] Kotlin：解构声明
来源：http://mx.gzmigu.cn

val (a, b) = Pair(1, 2)
来源：http://pu.521024.cn

[T13] Kotlin：只读 Map
来源：http://za.gzmigu.cn

val m = mapOf("a" to 1)
来源：http://pa.szxytkj.cn

[T14] Kotlin：循环
来源：http://yu.huixinmuqiang.cn

for (i in 1..10) println(i)
来源：http://xx.yuexingan06.cn

[T15] Kotlin：接口
来源：http://lw.muxihuayi.cn

interface Shape { fun area(): Double }
来源：http://jl.shxzukj.cn

[T16] Swift：Hello World
来源：http://gx.huixiangedu.cn

print("Hello")
来源：http://mf.jianghongdianzi.cn

[T17] Swift：变量与常量
来源：http://at.jctech888.com.cn

var a = 1;  let b = 2
来源：http://xa.nicolike.cn

[T18] Swift：字符串插值
来源：http://sx.jianghongdianzi.cn

"值: \(b)"
来源：http://xg.521024.cn

[T19] Swift：可选绑定
来源：http://cu.9csxet.cn

if let n = opt { print(n) }
来源：http://ri.shtwfgs.cn

[T20] Swift：数组操作
来源：http://al.panjiajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ig.yuntaijiaju.cn

[T21] Swift：遍历
来源：http://qb.nicolike.cn

for x in a { print(x) }
来源：http://zl.yuexingan06.cn

[T22] Swift：字典
来源：http://ii.jianghongdianzi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://if.colortex.cn

[T23] Swift：函数
来源：http://sa.hnjuh.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hh.lnxyls.cn

[T24] Swift：闭包
来源：http://mo.newstarts.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://pz.gzmigu.cn

[T25] Swift：结构体
来源：http://xw.jctech888.com.cn

struct P { var x: Int }
来源：http://fl.szxytkj.cn

[T26] Swift：类与重写
来源：http://eo.szxytkj.cn

class A: Base { override func f() {} }
来源：http://vx.asd995.cn

[T27] Swift：错误处理
来源：http://tv.shxzukj.cn

do { try f() } catch { print(error) }
来源：http://ih.huixinmuqiang.cn

[T28] Swift：枚举
来源：http://dp.muxihuayi.cn

enum Color { case red, green }
来源：http://op.asd995.cn

[T29] Swift：guard 提前返回
来源：http://uh.shxzukj.cn

guard let x = opt else { return }
来源：http://dz.haigaiapp.cn

[T30] Swift：协议
来源：http://uo.chemitech.net.cn

protocol Shape { func area() -> Double }
来源：http://rc.wgjwhj.cn

[T31] Lua：Hello World
来源：http://ho.jianghongdianzi.cn

print("Hello")
来源：http://jh.shxzskj.cn

[T32] Lua：局部变量
来源：http://uy.muxihuayi.cn

local a = 1
来源：http://yr.jianghongdianzi.cn

[T33] Lua：表（数组）
来源：http://ie.shxzskj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://qw.shtwfgs.cn

[T34] Lua：遍历表
来源：http://zb.hnjuh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://kl.521024.cn

[T35] Lua：字典表
来源：http://gk.gzmigu.cn

local d = { a = 1 };  d.b = 2
来源：http://pg.shxzskj.cn

[T36] Lua：函数
来源：http://yg.shxzukj.cn

function add(a, b) return a + b end
来源：http://fd.panjiajie.cn

[T37] Lua：字符串拼接
来源：http://dj.521024.cn

"a" .. "b"
来源：http://am.hahajie.cn

[T38] Lua：条件
来源：http://fa.huanxung.cn

if x > 0 then print("正") end
来源：http://cs.bjjhwx.cn

[T39] Lua：模式匹配
来源：http://et.shxzskj.cn

string.find(s, "%d+")
来源：http://ma.shtwfgs.cn

[T40] Lua：元表
来源：http://dg.9csxet.cn

setmetatable({}, { __index = base })
来源：http://ve.yuntaijiaju.cn

[T41] Perl：Hello World
来源：http://iu.hnjuh.cn

print "Hello\n";
来源：http://pc.huixiangedu.cn

[T42] Perl：变量类型
来源：http://sj.hnjuh.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zg.szxytkj.cn

[T43] Perl：字符串插值
来源：http://db.asd995.cn

"值: $a"
来源：http://tm.jctech888.com.cn

[T44] Perl：条件
来源：http://xy.nicolike.cn

if ($a > 0) { print "正"; }
来源：http://xh.nicolike.cn

[T45] Perl：数组遍历
来源：http://pp.huixinmuqiang.cn

for my $x (@arr) { print $x; }
来源：http://pd.jianghongdianzi.cn

[T46] Perl：哈希操作
来源：http://gz.9csxet.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vb.colortex.cn

[T47] Perl：正则捕获
来源：http://lt.yuexingan06.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wt.yuntaijiaju.cn

[T48] Perl：正则替换
来源：http://ey.nicolike.cn

$s =~ s/old/new/g;
来源：http://of.chemitech.net.cn

[T49] Perl：函数
来源：http://rw.wgjwhj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ap.colortex.cn

[T50] Perl：逐行读文件
来源：http://wh.chemitech.net.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://vd.nicolike.cn

while (my $line = <$fh>) { print $line; }
来源：http://ig.bookmarksfly.cn

[T51] Scala：Hello World
来源：http://no.bjjhwx.cn

println("Hello")
来源：http://qj.szxytkj.cn

[T52] Scala：变量
来源：http://kr.hnjuh.cn

val a = 1;  var b = 2
来源：http://lz.asd995.cn

[T53] Scala：字符串插值
来源：http://vg.chemitech.net.cn

s"值: $b"
来源：http://tw.nszjky.cn

[T54] Scala：集合映射
来源：http://kg.huanxung.cn

List(1, 2, 3).map(_ * 2)
来源：http://pc.asd995.cn

[T55] Scala：集合过滤
来源：http://kf.shxzukj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://el.chemitech.net.cn

[T56] Scala：样例类
来源：http://tb.haigaiapp.cn

case class User(name: String, age: Int)
来源：http://vu.nszjky.cn

[T57] Scala：模式匹配
来源：http://hx.szxytkj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://we.yuntaijiaju.cn

[T58] Scala：函数定义
来源：http://qt.asd995.cn

def add(a: Int, b: Int): Int = a + b
来源：http://uh.bjjhwx.cn

[T59] Scala：循环
来源：http://nn.panjiajie.cn

for (i <- 1 to 10) println(i)
来源：http://jz.haigaiapp.cn

[T60] Scala：折叠
来源：http://my.jctech888.com.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://il.panjiajie.cn

================================================================================
来源：http://nw.bookmarksfly.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bh.9csxet.cn

================================================================================
来源：http://ze.521024.cn

[U01] Py：创建虚拟环境
来源：http://ve.bookmarksfly.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ez.huixiangedu.cn

[U02] Py：导出 / 安装依赖
来源：http://ah.jianghongdianzi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://me.chemitech.net.cn

[U03] Py：加载 .env 配置
来源：http://jn.bookmarksfly.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gh.szsharing.cn

[U04] Py：变量调试打印
来源：http://si.9csxet.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ak.shtwfgs.cn

[U05] Py：列表去重且保序
来源：http://gf.newstarts.cn

list(dict.fromkeys(arr))
来源：http://zy.nicolike.cn

[U06] Py：合并两个字典
来源：http://ta.asd995.cn

{**a, **b}
来源：http://mb.huixiangedu.cn

[U07] Py：反转字典键值
来源：http://as.huanxung.cn

{v: k for k, v in d.items()}
来源：http://ka.jctech888.com.cn

[U08] Py：展平二维列表
来源：http://cb.bookmarksfly.cn

[y for x in nested for y in x]
来源：http://pk.chemitech.net.cn

[U09] Py：字典取最大值的键
来源：http://cj.shtwfgs.cn

max(d, key=d.get)
来源：http://ib.521024.cn

[U10] Py：按值排序字典
来源：http://vl.chemitech.net.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wh.jctech888.com.cn

[U11] Py：生成器表达式
来源：http://iw.asd995.cn

(x * 2 for x in arr)
来源：http://pz.bookmarksfly.cn

[U12] Py：取出现最多的 3 个元素
来源：http://bp.shxzskj.cn

Counter(arr).most_common(3)
来源：http://yg.szsharing.cn

[U13] Py：固定长度队列
来源：http://ng.huanxung.cn

deque(maxlen=10)
来源：http://ye.bookmarksfly.cn

[U14] Py：分组收集到列表
来源：http://xh.shtwfgs.cn

defaultdict(list)
来源：http://ys.wgjwhj.cn

[U15] Py：高精度计时
来源：http://nz.huixiangedu.cn

t = time.perf_counter()
来源：http://wq.hahajie.cn

[U16] Py：命令行参数解析
来源：http://wo.colortex.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ck.yuexingan06.cn

[U17] Py：初始化日志
来源：http://nx.lnxyls.cn

logging.basicConfig(level=logging.INFO)
来源：http://hx.huanxung.cn

[U18] Py：预编译正则
来源：http://cn.jctech888.com.cn

pat = re.compile(r"\d+")
来源：http://dz.nicolike.cn

[U19] Py：正则替换带回调
来源：http://pe.colortex.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://if.bjjhwx.cn

[U20] Py：缓存函数结果
来源：http://pc.nszjky.cn

@functools.lru_cache(maxsize=None)
来源：http://yp.chemitech.net.cn

[U21] Py：自定义上下文管理器
来源：http://eh.huanxung.cn

@contextlib.contextmanager
来源：http://ly.hahajie.cn

[U22] Py：矩阵转置
来源：http://dy.huixiangedu.cn

list(zip(*m))
来源：http://ku.yuexingan06.cn

[U23] Py：分块读取大文件
来源：http://fc.huanxung.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://so.jctech888.com.cn

[U24] Py：路径操作
来源：http://sl.muxihuayi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ba.asd995.cn


<!-- 参考信息 -->