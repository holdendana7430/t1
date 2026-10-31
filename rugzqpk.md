代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://io.nicolike.cn

[S08] C：动态内存分配与释放
来源：http://jj.shxzukj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ho.colortex.cn

[S09] C：结构体定义与初始化
来源：http://xa.hahajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xz.huixinmuqiang.cn

[S10] C：指针与解引用
来源：http://hz.huixinmuqiang.cn

int *p = &a;  *p = 5;
来源：http://gr.newstarts.cn

[S11] C：逐行读文件
来源：http://hx.521024.cn

FILE *f = fopen("a.txt", "r");
来源：http://pu.jctech888.com.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://uj.muxihuayi.cn

fclose(f);
来源：http://ej.muxihuayi.cn

[S12] C：写文件
来源：http://tz.hahajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://va.szxytkj.cn

[S13] C：宏定义
来源：http://jt.yuntaijiaju.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jl.huanxung.cn

[S14] C：枚举
来源：http://ke.yuexingan06.cn

enum Color { RED, GREEN, BLUE };
来源：http://vc.521024.cn

[S15] C：类型转换
来源：http://um.huanxung.cn

(double) a / b
来源：http://hr.lnxyls.cn

[S16] C：位操作置位
来源：http://dp.huixinmuqiang.cn

x |= (1 << 3);
来源：http://gb.nszjky.cn

[S17] C：安全拼接字符串
来源：http://vt.nszjky.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ub.hahajie.cn

[S18] C：命令行参数
来源：http://kj.wgjwhj.cn

int main(int argc, char **argv)
来源：http://wh.lnxyls.cn

[S19] C：快速排序
来源：http://bw.chemitech.net.cn

qsort(a, n, sizeof(int), cmp);
来源：http://cg.yuexingan06.cn

[S20] C：二分查找
来源：http://kt.huixiangedu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cl.nszjky.cn

[S21] C：字符类别判断
来源：http://dz.nszjky.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bp.nszjky.cn

[S22] C：字符串转数字
来源：http://sl.shxzskj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://zl.colortex.cn

[S23] C：随机数
来源：http://vc.gzmigu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://dn.9csxet.cn

[S24] C：获取本地时间
来源：http://ra.jianghongdianzi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mp.wgjwhj.cn

[S25] C：内存拷贝
来源：http://bz.shxzskj.cn

memcpy(dst, src, n);
来源：http://xh.bookmarksfly.cn

[S26] C：内存清零
来源：http://zo.lnxyls.cn

memset(a, 0, sizeof a);
来源：http://cx.panjiajie.cn

[S27] C：定义常量
来源：http://qk.shxzukj.cn

const double PI = 3.14159;
来源：http://it.shtwfgs.cn

[S28] C：静态变量
来源：http://po.huixiangedu.cn

static int counter = 0;
来源：http://tp.newstarts.cn

[S29] C：变参函数
来源：http://cs.hnjuh.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ae.yuntaijiaju.cn

[S30] C：头文件保护
来源：http://ap.panjiajie.cn

#ifndef X_H
来源：http://zh.yuexingan06.cn

#define X_H
来源：http://fz.jianghongdianzi.cn

#endif
来源：http://bs.huixiangedu.cn

[S31] C++：Hello World
来源：http://rw.9csxet.cn

#include <iostream>
来源：http://si.9csxet.cn

int main() { std::cout << "Hello\n"; }
来源：http://hu.yuntaijiaju.cn

[S32] C++：字符串
来源：http://je.hahajie.cn

std::string s = "hi";  s += "!";
来源：http://xe.hnjuh.cn

[S33] C++：vector 增删
来源：http://lq.shxzskj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fm.jianghongdianzi.cn

[S34] C++：遍历 vector
来源：http://hj.wgjwhj.cn

for (auto &x : v) { std::cout << x; }
来源：http://rv.shtwfgs.cn

[S35] C++：map
来源：http://hm.jianghongdianzi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qv.gzmigu.cn

[S36] C++：unordered_map
来源：http://en.shtwfgs.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yd.hahajie.cn

[S37] C++：set
来源：http://ko.szsharing.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ui.szsharing.cn

[S38] C++：排序
来源：http://en.asd995.cn

std::sort(v.begin(), v.end());
来源：http://wu.shxzskj.cn

[S39] C++：自定义比较器排序
来源：http://te.shxzskj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dq.jctech888.com.cn

[S40] C++：查找元素
来源：http://ag.bjjhwx.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ih.9csxet.cn

[S41] C++：类与构造函数
来源：http://dj.huanxung.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xj.shxzukj.cn

[S42] C++：继承与虚函数
来源：http://fl.huanxung.cn

class B : public Base { public: void f() override {} };
来源：http://ih.chemitech.net.cn

[S43] C++：智能指针
来源：http://gm.shxzskj.cn

auto p = std::make_unique<int>(5);
来源：http://ov.asd995.cn

[S44] C++：引用传参
来源：http://qh.yuexingan06.cn

void inc(int &x) { ++x; }
来源：http://ip.shtwfgs.cn

[S45] C++：lambda
来源：http://tj.asd995.cn

auto add = [](int a, int b) { return a + b; };
来源：http://yl.shxzskj.cn

[S46] C++：函数模板
来源：http://lu.huanxung.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://or.shxzskj.cn

[S47] C++：结构化绑定遍历
来源：http://kl.lnxyls.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mr.lnxyls.cn

[S48] C++：逐行读文件
来源：http://yu.szsharing.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vw.muxihuayi.cn

while (std::getline(in, line)) { }
来源：http://mf.nszjky.cn

[S49] C++：写文件
来源：http://tj.muxihuayi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fb.huixiangedu.cn

[S50] C++：格式化数字
来源：http://td.chemitech.net.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uc.9csxet.cn

[S51] C++：显式类型转换
来源：http://zr.hahajie.cn

static_cast<double>(a) / b
来源：http://hy.yuntaijiaju.cn

[S52] C++：const 与 noexcept
来源：http://po.colortex.cn

int size() const noexcept { return n_; }
来源：http://ne.521024.cn

[S53] C++：移动语义
来源：http://wx.chemitech.net.cn

std::vector<int> w = std::move(v);
来源：http://if.bjjhwx.cn

[S54] C++：异常处理
来源：http://jc.jctech888.com.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vr.wgjwhj.cn

[S55] C++：结构化绑定
来源：http://jb.yuntaijiaju.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://dl.shtwfgs.cn

[S56] C++：optional
来源：http://sy.gzmigu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ip.shxzukj.cn

[S57] C++：编译期常量
来源：http://mq.hnjuh.cn

constexpr int N = 10;
来源：http://md.9csxet.cn

[S58] C++：命名空间
来源：http://at.yuexingan06.cn

namespace ns { int f() { return 1; } }
来源：http://zc.9csxet.cn

[S59] C++：静态断言
来源：http://tp.shxzukj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fx.szxytkj.cn

[S60] C++：遍历并删除元素
来源：http://ja.yuexingan06.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xd.shxzskj.cn

================================================================================
来源：http://gx.shtwfgs.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ux.bjjhwx.cn

================================================================================
来源：http://kt.gzmigu.cn

[T01] Kotlin：Hello World
来源：http://lq.haigaiapp.cn

println("Hello")
来源：http://hd.newstarts.cn

[T02] Kotlin：变量
来源：http://hk.wgjwhj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xy.nicolike.cn

[T03] Kotlin：字符串模板
来源：http://en.nszjky.cn

"值: $b"
来源：http://xx.9csxet.cn

[T04] Kotlin：空安全
来源：http://qj.521024.cn

val n: String? = null;  n?.length
来源：http://zr.hahajie.cn

[T05] Kotlin：when 表达式
来源：http://xq.szsharing.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tl.jctech888.com.cn

[T06] Kotlin：集合映射
来源：http://tv.bookmarksfly.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://zp.jctech888.com.cn

[T07] Kotlin：集合过滤
来源：http://im.lnxyls.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://bs.bookmarksfly.cn

[T08] Kotlin：数据类
来源：http://bk.bjjhwx.cn

data class User(val name: String, val age: Int)
来源：http://du.jianghongdianzi.cn

[T09] Kotlin：扩展函数
来源：http://xn.shxzskj.cn

fun String.exclaim() = this + "!"
来源：http://ua.panjiajie.cn

[T10] Kotlin：默认参数
来源：http://bt.9csxet.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vk.wgjwhj.cn

[T11] Kotlin：协程
来源：http://lb.jianghongdianzi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://yx.jianghongdianzi.cn

[T12] Kotlin：解构声明
来源：http://ka.colortex.cn

val (a, b) = Pair(1, 2)
来源：http://el.muxihuayi.cn

[T13] Kotlin：只读 Map
来源：http://nw.hnjuh.cn

val m = mapOf("a" to 1)
来源：http://oj.colortex.cn

[T14] Kotlin：循环
来源：http://nh.9csxet.cn

for (i in 1..10) println(i)
来源：http://wa.gzmigu.cn

[T15] Kotlin：接口
来源：http://uv.521024.cn

interface Shape { fun area(): Double }
来源：http://ab.muxihuayi.cn

[T16] Swift：Hello World
来源：http://cr.nicolike.cn

print("Hello")
来源：http://mg.shxzukj.cn

[T17] Swift：变量与常量
来源：http://nq.szsharing.cn

var a = 1;  let b = 2
来源：http://wj.9csxet.cn

[T18] Swift：字符串插值
来源：http://rs.jctech888.com.cn

"值: \(b)"
来源：http://xz.panjiajie.cn

[T19] Swift：可选绑定
来源：http://ya.chemitech.net.cn

if let n = opt { print(n) }
来源：http://hh.9csxet.cn

[T20] Swift：数组操作
来源：http://hb.lnxyls.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hy.jctech888.com.cn

[T21] Swift：遍历
来源：http://wd.9csxet.cn

for x in a { print(x) }
来源：http://ik.wgjwhj.cn

[T22] Swift：字典
来源：http://re.jianghongdianzi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ly.newstarts.cn

[T23] Swift：函数
来源：http://rr.yuexingan06.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nv.nicolike.cn

[T24] Swift：闭包
来源：http://kh.huixiangedu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gh.panjiajie.cn

[T25] Swift：结构体
来源：http://bf.newstarts.cn

struct P { var x: Int }
来源：http://he.jctech888.com.cn

[T26] Swift：类与重写
来源：http://dl.nszjky.cn

class A: Base { override func f() {} }
来源：http://mq.muxihuayi.cn

[T27] Swift：错误处理
来源：http://dt.shxzukj.cn

do { try f() } catch { print(error) }
来源：http://wd.shxzskj.cn

[T28] Swift：枚举
来源：http://kj.521024.cn

enum Color { case red, green }
来源：http://mw.yuexingan06.cn

[T29] Swift：guard 提前返回
来源：http://vh.shtwfgs.cn

guard let x = opt else { return }
来源：http://zw.huanxung.cn

[T30] Swift：协议
来源：http://uu.9csxet.cn

protocol Shape { func area() -> Double }
来源：http://ab.521024.cn

[T31] Lua：Hello World
来源：http://ls.bjjhwx.cn

print("Hello")
来源：http://bi.jctech888.com.cn

[T32] Lua：局部变量
来源：http://if.colortex.cn

local a = 1
来源：http://wk.hnjuh.cn

[T33] Lua：表（数组）
来源：http://db.szsharing.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hc.huixinmuqiang.cn

[T34] Lua：遍历表
来源：http://qg.muxihuayi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://pu.lnxyls.cn

[T35] Lua：字典表
来源：http://vu.gzmigu.cn

local d = { a = 1 };  d.b = 2
来源：http://wa.nicolike.cn

[T36] Lua：函数
来源：http://yf.newstarts.cn

function add(a, b) return a + b end
来源：http://wo.haigaiapp.cn

[T37] Lua：字符串拼接
来源：http://hb.shxzskj.cn

"a" .. "b"
来源：http://dm.hnjuh.cn

[T38] Lua：条件
来源：http://aj.huixiangedu.cn

if x > 0 then print("正") end
来源：http://tn.newstarts.cn

[T39] Lua：模式匹配
来源：http://kp.hnjuh.cn

string.find(s, "%d+")
来源：http://en.huixinmuqiang.cn

[T40] Lua：元表
来源：http://le.huixiangedu.cn

setmetatable({}, { __index = base })
来源：http://fc.szxytkj.cn

[T41] Perl：Hello World
来源：http://ib.shxzukj.cn

print "Hello\n";
来源：http://uq.jianghongdianzi.cn

[T42] Perl：变量类型
来源：http://dx.colortex.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://og.huanxung.cn

[T43] Perl：字符串插值
来源：http://pd.colortex.cn

"值: $a"
来源：http://gt.hnjuh.cn

[T44] Perl：条件
来源：http://jj.shxzukj.cn

if ($a > 0) { print "正"; }
来源：http://zi.wgjwhj.cn

[T45] Perl：数组遍历
来源：http://qb.521024.cn

for my $x (@arr) { print $x; }
来源：http://ce.huixiangedu.cn

[T46] Perl：哈希操作
来源：http://ks.colortex.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://me.szxytkj.cn

[T47] Perl：正则捕获
来源：http://ic.muxihuayi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://fu.yuexingan06.cn

[T48] Perl：正则替换
来源：http://nl.haigaiapp.cn

$s =~ s/old/new/g;
来源：http://xx.huixinmuqiang.cn

[T49] Perl：函数
来源：http://vf.wgjwhj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zc.jianghongdianzi.cn

[T50] Perl：逐行读文件
来源：http://dr.jianghongdianzi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://id.bjjhwx.cn

while (my $line = <$fh>) { print $line; }
来源：http://vi.muxihuayi.cn

[T51] Scala：Hello World
来源：http://rz.nszjky.cn

println("Hello")
来源：http://ag.hnjuh.cn

[T52] Scala：变量
来源：http://cp.asd995.cn

val a = 1;  var b = 2
来源：http://wj.gzmigu.cn

[T53] Scala：字符串插值
来源：http://pf.huanxung.cn

s"值: $b"
来源：http://mz.panjiajie.cn

[T54] Scala：集合映射
来源：http://er.huanxung.cn

List(1, 2, 3).map(_ * 2)
来源：http://bb.shtwfgs.cn

[T55] Scala：集合过滤
来源：http://du.nicolike.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ls.hnjuh.cn

[T56] Scala：样例类
来源：http://uz.shxzukj.cn

case class User(name: String, age: Int)
来源：http://gt.newstarts.cn

[T57] Scala：模式匹配
来源：http://dj.asd995.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://yo.panjiajie.cn

[T58] Scala：函数定义
来源：http://sq.nszjky.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zj.9csxet.cn

[T59] Scala：循环
来源：http://iy.chemitech.net.cn

for (i <- 1 to 10) println(i)
来源：http://xb.huanxung.cn

[T60] Scala：折叠
来源：http://wb.lnxyls.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://eu.yuntaijiaju.cn

================================================================================
来源：http://dp.shxzskj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tl.shxzskj.cn

================================================================================
来源：http://pp.hahajie.cn

[U01] Py：创建虚拟环境
来源：http://oa.yuntaijiaju.cn

python -m venv .venv && source .venv/bin/activate
来源：http://pl.newstarts.cn

[U02] Py：导出 / 安装依赖
来源：http://kd.shxzskj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fr.wgjwhj.cn

[U03] Py：加载 .env 配置
来源：http://uc.hahajie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://em.huixiangedu.cn

[U04] Py：变量调试打印
来源：http://ge.huixiangedu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hr.yuntaijiaju.cn

[U05] Py：列表去重且保序
来源：http://qz.shxzskj.cn

list(dict.fromkeys(arr))
来源：http://aw.asd995.cn

[U06] Py：合并两个字典
来源：http://kx.haigaiapp.cn

{**a, **b}
来源：http://bn.nszjky.cn

[U07] Py：反转字典键值
来源：http://av.panjiajie.cn

{v: k for k, v in d.items()}
来源：http://on.newstarts.cn

[U08] Py：展平二维列表
来源：http://nb.muxihuayi.cn

[y for x in nested for y in x]
来源：http://tn.521024.cn

[U09] Py：字典取最大值的键
来源：http://us.newstarts.cn

max(d, key=d.get)
来源：http://gw.muxihuayi.cn

[U10] Py：按值排序字典
来源：http://kh.huanxung.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://aw.huanxung.cn

[U11] Py：生成器表达式
来源：http://jv.shxzukj.cn

(x * 2 for x in arr)
来源：http://bw.wgjwhj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zl.szxytkj.cn

Counter(arr).most_common(3)
来源：http://ar.gzmigu.cn

[U13] Py：固定长度队列
来源：http://ik.nicolike.cn

deque(maxlen=10)
来源：http://gq.nicolike.cn

[U14] Py：分组收集到列表
来源：http://ci.huixiangedu.cn

defaultdict(list)
来源：http://wh.huixinmuqiang.cn

[U15] Py：高精度计时
来源：http://dh.jianghongdianzi.cn

t = time.perf_counter()
来源：http://dd.chemitech.net.cn

[U16] Py：命令行参数解析
来源：http://lf.jctech888.com.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lc.jctech888.com.cn

[U17] Py：初始化日志
来源：http://rc.shxzukj.cn

logging.basicConfig(level=logging.INFO)
来源：http://cq.shtwfgs.cn

[U18] Py：预编译正则
来源：http://na.chemitech.net.cn

pat = re.compile(r"\d+")
来源：http://hi.shtwfgs.cn

[U19] Py：正则替换带回调
来源：http://qi.wgjwhj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jb.szsharing.cn

[U20] Py：缓存函数结果
来源：http://jc.nicolike.cn

@functools.lru_cache(maxsize=None)
来源：http://je.jianghongdianzi.cn

[U21] Py：自定义上下文管理器
来源：http://qu.huixiangedu.cn

@contextlib.contextmanager
来源：http://vs.chemitech.net.cn

[U22] Py：矩阵转置
来源：http://cl.asd995.cn

list(zip(*m))
来源：http://dn.asd995.cn

[U23] Py：分块读取大文件
来源：http://jq.huixiangedu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hb.wgjwhj.cn

[U24] Py：路径操作
来源：http://sl.nszjky.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nz.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://af.szxytkj.cn

csv.DictReader(f)
来源：http://fb.wgjwhj.cn

[U26] Py：并发下载
来源：http://it.huanxung.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yy.haigaiapp.cn

[U27] Py：异步 HTTP
来源：http://ib.panjiajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://gg.asd995.cn

[U28] Py：类型别名
来源：http://om.newstarts.cn

UserId = int
来源：http://xt.panjiajie.cn

[U29] Py：属性校验
来源：http://ja.shtwfgs.cn

@property 与 @x.setter 配合
来源：http://lb.shxzukj.cn

[U30] Py：数据类
来源：http://vx.nicolike.cn

@dataclass(slots=True)
来源：http://tv.nicolike.cn


<!-- 参考信息 -->