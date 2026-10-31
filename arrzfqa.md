代发 wailian999

int x; scanf("%d", &x);
来源：http://dt.huanxung.cn

[S04] C：字符串复制
来源：http://gu.jctech888.com.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fg.hahajie.cn

[S05] C：字符串长度
来源：http://fm.gzmigu.cn

strlen(s)
来源：http://yx.szxytkj.cn

[S06] C：字符串比较
来源：http://br.gzmigu.cn

strcmp(a, b) == 0
来源：http://fu.521024.cn

[S07] C：数组遍历求和
来源：http://gp.9csxet.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cc.chemitech.net.cn

[S08] C：动态内存分配与释放
来源：http://th.shxzskj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://os.yuexingan06.cn

[S09] C：结构体定义与初始化
来源：http://kq.yuntaijiaju.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ji.hnjuh.cn

[S10] C：指针与解引用
来源：http://mt.huixinmuqiang.cn

int *p = &a;  *p = 5;
来源：http://hl.panjiajie.cn

[S11] C：逐行读文件
来源：http://vc.nszjky.cn

FILE *f = fopen("a.txt", "r");
来源：http://ly.yuntaijiaju.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mu.nicolike.cn

fclose(f);
来源：http://xp.shxzskj.cn

[S12] C：写文件
来源：http://ll.bjjhwx.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dl.chemitech.net.cn

[S13] C：宏定义
来源：http://kx.colortex.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jp.chemitech.net.cn

[S14] C：枚举
来源：http://ty.asd995.cn

enum Color { RED, GREEN, BLUE };
来源：http://pp.wgjwhj.cn

[S15] C：类型转换
来源：http://vx.newstarts.cn

(double) a / b
来源：http://bf.bookmarksfly.cn

[S16] C：位操作置位
来源：http://dq.jianghongdianzi.cn

x |= (1 << 3);
来源：http://us.521024.cn

[S17] C：安全拼接字符串
来源：http://lf.bookmarksfly.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wd.521024.cn

[S18] C：命令行参数
来源：http://pa.lnxyls.cn

int main(int argc, char **argv)
来源：http://ct.huixinmuqiang.cn

[S19] C：快速排序
来源：http://aq.yuntaijiaju.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fx.bjjhwx.cn

[S20] C：二分查找
来源：http://cb.yuntaijiaju.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://or.gzmigu.cn

[S21] C：字符类别判断
来源：http://tz.huixiangedu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kq.hnjuh.cn

[S22] C：字符串转数字
来源：http://lp.shtwfgs.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xa.yuntaijiaju.cn

[S23] C：随机数
来源：http://qm.jctech888.com.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qr.nszjky.cn

[S24] C：获取本地时间
来源：http://mc.shxzukj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qk.yuexingan06.cn

[S25] C：内存拷贝
来源：http://vu.shxzskj.cn

memcpy(dst, src, n);
来源：http://bp.huixiangedu.cn

[S26] C：内存清零
来源：http://rm.521024.cn

memset(a, 0, sizeof a);
来源：http://uw.jctech888.com.cn

[S27] C：定义常量
来源：http://rt.yuexingan06.cn

const double PI = 3.14159;
来源：http://es.chemitech.net.cn

[S28] C：静态变量
来源：http://ro.yuexingan06.cn

static int counter = 0;
来源：http://sw.hahajie.cn

[S29] C：变参函数
来源：http://za.lnxyls.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yo.huixiangedu.cn

[S30] C：头文件保护
来源：http://ng.shxzskj.cn

#ifndef X_H
来源：http://zi.yuntaijiaju.cn

#define X_H
来源：http://ck.shxzukj.cn

#endif
来源：http://xr.wgjwhj.cn

[S31] C++：Hello World
来源：http://ug.bjjhwx.cn

#include <iostream>
来源：http://hd.shxzskj.cn

int main() { std::cout << "Hello\n"; }
来源：http://uf.yuntaijiaju.cn

[S32] C++：字符串
来源：http://ar.hnjuh.cn

std::string s = "hi";  s += "!";
来源：http://sb.521024.cn

[S33] C++：vector 增删
来源：http://du.newstarts.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bn.muxihuayi.cn

[S34] C++：遍历 vector
来源：http://ym.shxzukj.cn

for (auto &x : v) { std::cout << x; }
来源：http://fi.shxzskj.cn

[S35] C++：map
来源：http://ja.hahajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nx.jctech888.com.cn

[S36] C++：unordered_map
来源：http://rv.yuntaijiaju.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ge.bjjhwx.cn

[S37] C++：set
来源：http://at.huixiangedu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://du.szsharing.cn

[S38] C++：排序
来源：http://xj.newstarts.cn

std::sort(v.begin(), v.end());
来源：http://kc.shtwfgs.cn

[S39] C++：自定义比较器排序
来源：http://ze.jctech888.com.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mw.shxzskj.cn

[S40] C++：查找元素
来源：http://gq.huanxung.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rr.muxihuayi.cn

[S41] C++：类与构造函数
来源：http://uq.gzmigu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vc.nszjky.cn

[S42] C++：继承与虚函数
来源：http://xv.9csxet.cn

class B : public Base { public: void f() override {} };
来源：http://zt.huanxung.cn

[S43] C++：智能指针
来源：http://eb.shxzskj.cn

auto p = std::make_unique<int>(5);
来源：http://bi.jianghongdianzi.cn

[S44] C++：引用传参
来源：http://ee.jianghongdianzi.cn

void inc(int &x) { ++x; }
来源：http://zy.muxihuayi.cn

[S45] C++：lambda
来源：http://co.hahajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fm.521024.cn

[S46] C++：函数模板
来源：http://cw.gzmigu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gz.lnxyls.cn

[S47] C++：结构化绑定遍历
来源：http://fi.nicolike.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ld.521024.cn

[S48] C++：逐行读文件
来源：http://tb.muxihuayi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://cn.gzmigu.cn

while (std::getline(in, line)) { }
来源：http://ub.9csxet.cn

[S49] C++：写文件
来源：http://kv.hahajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jf.wgjwhj.cn

[S50] C++：格式化数字
来源：http://al.bjjhwx.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zv.9csxet.cn

[S51] C++：显式类型转换
来源：http://je.panjiajie.cn

static_cast<double>(a) / b
来源：http://at.muxihuayi.cn

[S52] C++：const 与 noexcept
来源：http://om.huixiangedu.cn

int size() const noexcept { return n_; }
来源：http://di.shtwfgs.cn

[S53] C++：移动语义
来源：http://bv.lnxyls.cn

std::vector<int> w = std::move(v);
来源：http://oy.huanxung.cn

[S54] C++：异常处理
来源：http://gv.yuexingan06.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tu.colortex.cn

[S55] C++：结构化绑定
来源：http://km.huixinmuqiang.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://sj.huanxung.cn

[S56] C++：optional
来源：http://uq.hahajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bl.shxzskj.cn

[S57] C++：编译期常量
来源：http://pi.szsharing.cn

constexpr int N = 10;
来源：http://jk.chemitech.net.cn

[S58] C++：命名空间
来源：http://ta.bookmarksfly.cn

namespace ns { int f() { return 1; } }
来源：http://of.chemitech.net.cn

[S59] C++：静态断言
来源：http://pv.colortex.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://oc.9csxet.cn

[S60] C++：遍历并删除元素
来源：http://fh.chemitech.net.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://le.haigaiapp.cn

================================================================================
来源：http://mw.bookmarksfly.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ug.muxihuayi.cn

================================================================================
来源：http://gn.lnxyls.cn

[T01] Kotlin：Hello World
来源：http://so.szsharing.cn

println("Hello")
来源：http://hu.huanxung.cn

[T02] Kotlin：变量
来源：http://yb.newstarts.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ri.muxihuayi.cn

[T03] Kotlin：字符串模板
来源：http://fx.jianghongdianzi.cn

"值: $b"
来源：http://pv.colortex.cn

[T04] Kotlin：空安全
来源：http://wz.newstarts.cn

val n: String? = null;  n?.length
来源：http://sb.521024.cn

[T05] Kotlin：when 表达式
来源：http://rh.hahajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uk.hahajie.cn

[T06] Kotlin：集合映射
来源：http://dz.hahajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://cd.jctech888.com.cn

[T07] Kotlin：集合过滤
来源：http://xj.haigaiapp.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wz.haigaiapp.cn

[T08] Kotlin：数据类
来源：http://xz.9csxet.cn

data class User(val name: String, val age: Int)
来源：http://li.521024.cn

[T09] Kotlin：扩展函数
来源：http://op.colortex.cn

fun String.exclaim() = this + "!"
来源：http://ud.bookmarksfly.cn

[T10] Kotlin：默认参数
来源：http://aj.wgjwhj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://eh.hnjuh.cn

[T11] Kotlin：协程
来源：http://rk.jianghongdianzi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wm.shxzskj.cn

[T12] Kotlin：解构声明
来源：http://gc.szsharing.cn

val (a, b) = Pair(1, 2)
来源：http://pf.hahajie.cn

[T13] Kotlin：只读 Map
来源：http://vt.huixiangedu.cn

val m = mapOf("a" to 1)
来源：http://bi.shxzukj.cn

[T14] Kotlin：循环
来源：http://if.521024.cn

for (i in 1..10) println(i)
来源：http://pu.nszjky.cn

[T15] Kotlin：接口
来源：http://gp.hahajie.cn

interface Shape { fun area(): Double }
来源：http://uz.hnjuh.cn

[T16] Swift：Hello World
来源：http://ai.huixiangedu.cn

print("Hello")
来源：http://ny.szxytkj.cn

[T17] Swift：变量与常量
来源：http://kx.huixiangedu.cn

var a = 1;  let b = 2
来源：http://mt.szsharing.cn

[T18] Swift：字符串插值
来源：http://su.shtwfgs.cn

"值: \(b)"
来源：http://by.wgjwhj.cn

[T19] Swift：可选绑定
来源：http://jy.jctech888.com.cn

if let n = opt { print(n) }
来源：http://fn.hnjuh.cn

[T20] Swift：数组操作
来源：http://nv.wgjwhj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://kd.yuntaijiaju.cn

[T21] Swift：遍历
来源：http://cb.szxytkj.cn

for x in a { print(x) }
来源：http://dz.chemitech.net.cn

[T22] Swift：字典
来源：http://la.newstarts.cn

var d = ["a": 1];  d["b"] = 2
来源：http://lk.muxihuayi.cn

[T23] Swift：函数
来源：http://hw.newstarts.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vy.szxytkj.cn

[T24] Swift：闭包
来源：http://vc.hnjuh.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ov.hahajie.cn

[T25] Swift：结构体
来源：http://ry.nszjky.cn

struct P { var x: Int }
来源：http://hk.hahajie.cn

[T26] Swift：类与重写
来源：http://vf.lnxyls.cn

class A: Base { override func f() {} }
来源：http://yx.shxzskj.cn

[T27] Swift：错误处理
来源：http://av.huanxung.cn

do { try f() } catch { print(error) }
来源：http://ru.newstarts.cn

[T28] Swift：枚举
来源：http://qb.huixiangedu.cn

enum Color { case red, green }
来源：http://gn.huixiangedu.cn

[T29] Swift：guard 提前返回
来源：http://ex.huixiangedu.cn

guard let x = opt else { return }
来源：http://be.yuntaijiaju.cn

[T30] Swift：协议
来源：http://xy.wgjwhj.cn

protocol Shape { func area() -> Double }
来源：http://mg.nszjky.cn

[T31] Lua：Hello World
来源：http://oa.nicolike.cn

print("Hello")
来源：http://bl.jianghongdianzi.cn

[T32] Lua：局部变量
来源：http://gj.jianghongdianzi.cn

local a = 1
来源：http://ho.huixinmuqiang.cn

[T33] Lua：表（数组）
来源：http://ei.gzmigu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://qp.bjjhwx.cn

[T34] Lua：遍历表
来源：http://ti.yuexingan06.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://wv.lnxyls.cn

[T35] Lua：字典表
来源：http://kt.wgjwhj.cn

local d = { a = 1 };  d.b = 2
来源：http://js.nicolike.cn

[T36] Lua：函数
来源：http://eu.newstarts.cn

function add(a, b) return a + b end
来源：http://fa.chemitech.net.cn

[T37] Lua：字符串拼接
来源：http://ph.shtwfgs.cn

"a" .. "b"
来源：http://zm.lnxyls.cn

[T38] Lua：条件
来源：http://bu.521024.cn

if x > 0 then print("正") end
来源：http://rv.521024.cn

[T39] Lua：模式匹配
来源：http://uo.bjjhwx.cn

string.find(s, "%d+")
来源：http://pg.yuntaijiaju.cn

[T40] Lua：元表
来源：http://di.asd995.cn

setmetatable({}, { __index = base })
来源：http://jy.shtwfgs.cn

[T41] Perl：Hello World
来源：http://os.wgjwhj.cn

print "Hello\n";
来源：http://zo.shtwfgs.cn

[T42] Perl：变量类型
来源：http://mw.huixinmuqiang.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kv.muxihuayi.cn

[T43] Perl：字符串插值
来源：http://oz.yuexingan06.cn

"值: $a"
来源：http://oh.panjiajie.cn

[T44] Perl：条件
来源：http://oy.yuntaijiaju.cn

if ($a > 0) { print "正"; }
来源：http://nu.hahajie.cn

[T45] Perl：数组遍历
来源：http://ta.colortex.cn

for my $x (@arr) { print $x; }
来源：http://jd.huixiangedu.cn

[T46] Perl：哈希操作
来源：http://da.hahajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wm.gzmigu.cn

[T47] Perl：正则捕获
来源：http://uz.bookmarksfly.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ej.panjiajie.cn

[T48] Perl：正则替换
来源：http://aw.lnxyls.cn

$s =~ s/old/new/g;
来源：http://hm.bjjhwx.cn

[T49] Perl：函数
来源：http://vs.panjiajie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cc.szxytkj.cn

[T50] Perl：逐行读文件
来源：http://fc.shxzukj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://go.jctech888.com.cn

while (my $line = <$fh>) { print $line; }
来源：http://ar.yuntaijiaju.cn

[T51] Scala：Hello World
来源：http://nf.9csxet.cn

println("Hello")
来源：http://is.colortex.cn

[T52] Scala：变量
来源：http://pc.jianghongdianzi.cn

val a = 1;  var b = 2
来源：http://ms.yuntaijiaju.cn

[T53] Scala：字符串插值
来源：http://ln.jianghongdianzi.cn

s"值: $b"
来源：http://ku.jctech888.com.cn

[T54] Scala：集合映射
来源：http://oz.hahajie.cn

List(1, 2, 3).map(_ * 2)
来源：http://cl.521024.cn

[T55] Scala：集合过滤
来源：http://bq.hahajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://vu.nicolike.cn

[T56] Scala：样例类
来源：http://sp.lnxyls.cn

case class User(name: String, age: Int)
来源：http://vu.shxzskj.cn

[T57] Scala：模式匹配
来源：http://yy.hnjuh.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://qk.huixiangedu.cn

[T58] Scala：函数定义
来源：http://ou.panjiajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wt.colortex.cn

[T59] Scala：循环
来源：http://jw.bjjhwx.cn

for (i <- 1 to 10) println(i)
来源：http://br.yuexingan06.cn

[T60] Scala：折叠
来源：http://fc.bjjhwx.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://di.nszjky.cn

================================================================================
来源：http://pq.hnjuh.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mj.gzmigu.cn

================================================================================
来源：http://jd.jianghongdianzi.cn

[U01] Py：创建虚拟环境
来源：http://an.panjiajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mt.newstarts.cn

[U02] Py：导出 / 安装依赖
来源：http://jn.haigaiapp.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kc.nszjky.cn

[U03] Py：加载 .env 配置
来源：http://wh.haigaiapp.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://po.gzmigu.cn

[U04] Py：变量调试打印
来源：http://dv.huixinmuqiang.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ob.shxzukj.cn

[U05] Py：列表去重且保序
来源：http://rx.shxzskj.cn

list(dict.fromkeys(arr))
来源：http://yh.nicolike.cn

[U06] Py：合并两个字典
来源：http://hh.muxihuayi.cn

{**a, **b}
来源：http://hc.szxytkj.cn

[U07] Py：反转字典键值
来源：http://gn.huixinmuqiang.cn

{v: k for k, v in d.items()}
来源：http://ct.yuexingan06.cn

[U08] Py：展平二维列表
来源：http://zf.huanxung.cn

[y for x in nested for y in x]
来源：http://ny.shxzukj.cn

[U09] Py：字典取最大值的键
来源：http://uo.huanxung.cn

max(d, key=d.get)
来源：http://iw.shxzskj.cn

[U10] Py：按值排序字典
来源：http://xs.shxzskj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xz.wgjwhj.cn

[U11] Py：生成器表达式
来源：http://yv.hahajie.cn

(x * 2 for x in arr)
来源：http://ul.nszjky.cn

[U12] Py：取出现最多的 3 个元素
来源：http://nk.panjiajie.cn

Counter(arr).most_common(3)
来源：http://aa.asd995.cn

[U13] Py：固定长度队列
来源：http://tz.hnjuh.cn

deque(maxlen=10)
来源：http://pq.gzmigu.cn

[U14] Py：分组收集到列表
来源：http://av.newstarts.cn

defaultdict(list)
来源：http://wk.szsharing.cn

[U15] Py：高精度计时
来源：http://hj.newstarts.cn

t = time.perf_counter()
来源：http://ft.newstarts.cn

[U16] Py：命令行参数解析
来源：http://de.huixiangedu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fm.hahajie.cn

[U17] Py：初始化日志
来源：http://mq.asd995.cn

logging.basicConfig(level=logging.INFO)
来源：http://jp.szsharing.cn

[U18] Py：预编译正则
来源：http://qs.huixinmuqiang.cn

pat = re.compile(r"\d+")
来源：http://hn.9csxet.cn

[U19] Py：正则替换带回调
来源：http://lq.hnjuh.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ac.hnjuh.cn

[U20] Py：缓存函数结果
来源：http://jv.newstarts.cn

@functools.lru_cache(maxsize=None)
来源：http://ng.asd995.cn

[U21] Py：自定义上下文管理器
来源：http://tn.9csxet.cn

@contextlib.contextmanager
来源：http://ve.colortex.cn

[U22] Py：矩阵转置
来源：http://lh.asd995.cn

list(zip(*m))
来源：http://hs.shxzukj.cn

[U23] Py：分块读取大文件
来源：http://ft.szxytkj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sx.panjiajie.cn

[U24] Py：路径操作
来源：http://ox.shtwfgs.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vf.hnjuh.cn

[U25] Py：CSV 按字典读
来源：http://hz.muxihuayi.cn

csv.DictReader(f)
来源：http://dg.shxzukj.cn

[U26] Py：并发下载
来源：http://rh.chemitech.net.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wn.9csxet.cn


<!-- 参考信息 -->