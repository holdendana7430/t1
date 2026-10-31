代发 wailian999

S. C / C++ 专题
来源：http://bm.hahajie.cn

================================================================================
来源：http://by.hnjuh.cn

[S01] C：Hello World
来源：http://je.hnjuh.cn

#include <stdio.h>
来源：http://cz.521024.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wu.nicolike.cn

[S02] C：变量与格式化输出
来源：http://vy.bookmarksfly.cn

int a = 10; printf("%d\n", a);
来源：http://tt.colortex.cn

[S03] C：读入整数
来源：http://fa.huixinmuqiang.cn

int x; scanf("%d", &x);
来源：http://id.huixinmuqiang.cn

[S04] C：字符串复制
来源：http://fu.huanxung.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fk.gzmigu.cn

[S05] C：字符串长度
来源：http://ql.szsharing.cn

strlen(s)
来源：http://cb.panjiajie.cn

[S06] C：字符串比较
来源：http://au.huixiangedu.cn

strcmp(a, b) == 0
来源：http://uj.szxytkj.cn

[S07] C：数组遍历求和
来源：http://wc.hnjuh.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ad.chemitech.net.cn

[S08] C：动态内存分配与释放
来源：http://xd.yuntaijiaju.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zs.9csxet.cn

[S09] C：结构体定义与初始化
来源：http://zt.huixinmuqiang.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wu.hahajie.cn

[S10] C：指针与解引用
来源：http://gp.lnxyls.cn

int *p = &a;  *p = 5;
来源：http://ty.muxihuayi.cn

[S11] C：逐行读文件
来源：http://yn.yuexingan06.cn

FILE *f = fopen("a.txt", "r");
来源：http://mo.wgjwhj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://iq.shxzskj.cn

fclose(f);
来源：http://ht.huanxung.cn

[S12] C：写文件
来源：http://ns.gzmigu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wx.jctech888.com.cn

[S13] C：宏定义
来源：http://du.shxzukj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rm.yuntaijiaju.cn

[S14] C：枚举
来源：http://wz.colortex.cn

enum Color { RED, GREEN, BLUE };
来源：http://em.wgjwhj.cn

[S15] C：类型转换
来源：http://pl.jctech888.com.cn

(double) a / b
来源：http://pd.huixiangedu.cn

[S16] C：位操作置位
来源：http://mn.colortex.cn

x |= (1 << 3);
来源：http://em.nszjky.cn

[S17] C：安全拼接字符串
来源：http://zy.chemitech.net.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jq.yuntaijiaju.cn

[S18] C：命令行参数
来源：http://fu.jctech888.com.cn

int main(int argc, char **argv)
来源：http://fl.nszjky.cn

[S19] C：快速排序
来源：http://xi.lnxyls.cn

qsort(a, n, sizeof(int), cmp);
来源：http://mr.szxytkj.cn

[S20] C：二分查找
来源：http://du.asd995.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://am.gzmigu.cn

[S21] C：字符类别判断
来源：http://dz.haigaiapp.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mg.shxzskj.cn

[S22] C：字符串转数字
来源：http://wc.bookmarksfly.cn

atoi("42");  strtod("3.14", NULL);
来源：http://za.chemitech.net.cn

[S23] C：随机数
来源：http://qu.nszjky.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xc.nicolike.cn

[S24] C：获取本地时间
来源：http://tq.jctech888.com.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gh.asd995.cn

[S25] C：内存拷贝
来源：http://ro.lnxyls.cn

memcpy(dst, src, n);
来源：http://bd.9csxet.cn

[S26] C：内存清零
来源：http://jw.newstarts.cn

memset(a, 0, sizeof a);
来源：http://hw.huixinmuqiang.cn

[S27] C：定义常量
来源：http://oc.newstarts.cn

const double PI = 3.14159;
来源：http://sg.shxzukj.cn

[S28] C：静态变量
来源：http://aq.lnxyls.cn

static int counter = 0;
来源：http://sv.muxihuayi.cn

[S29] C：变参函数
来源：http://vy.wgjwhj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://md.hahajie.cn

[S30] C：头文件保护
来源：http://wn.panjiajie.cn

#ifndef X_H
来源：http://fn.huanxung.cn

#define X_H
来源：http://gt.hnjuh.cn

#endif
来源：http://xa.haigaiapp.cn

[S31] C++：Hello World
来源：http://py.nszjky.cn

#include <iostream>
来源：http://yj.9csxet.cn

int main() { std::cout << "Hello\n"; }
来源：http://vs.huixiangedu.cn

[S32] C++：字符串
来源：http://kt.bjjhwx.cn

std::string s = "hi";  s += "!";
来源：http://wa.yuexingan06.cn

[S33] C++：vector 增删
来源：http://gr.szxytkj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ol.huixiangedu.cn

[S34] C++：遍历 vector
来源：http://yf.wgjwhj.cn

for (auto &x : v) { std::cout << x; }
来源：http://yj.asd995.cn

[S35] C++：map
来源：http://ny.asd995.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ug.huixinmuqiang.cn

[S36] C++：unordered_map
来源：http://kl.shxzskj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mi.szsharing.cn

[S37] C++：set
来源：http://xo.521024.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rb.9csxet.cn

[S38] C++：排序
来源：http://gv.huixinmuqiang.cn

std::sort(v.begin(), v.end());
来源：http://uh.szxytkj.cn

[S39] C++：自定义比较器排序
来源：http://vv.asd995.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tf.shxzukj.cn

[S40] C++：查找元素
来源：http://lh.yuntaijiaju.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tm.gzmigu.cn

[S41] C++：类与构造函数
来源：http://ly.panjiajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://re.bookmarksfly.cn

[S42] C++：继承与虚函数
来源：http://hs.nicolike.cn

class B : public Base { public: void f() override {} };
来源：http://jj.colortex.cn

[S43] C++：智能指针
来源：http://ru.hnjuh.cn

auto p = std::make_unique<int>(5);
来源：http://ug.nicolike.cn

[S44] C++：引用传参
来源：http://qg.wgjwhj.cn

void inc(int &x) { ++x; }
来源：http://ee.szsharing.cn

[S45] C++：lambda
来源：http://ui.shtwfgs.cn

auto add = [](int a, int b) { return a + b; };
来源：http://la.huanxung.cn

[S46] C++：函数模板
来源：http://jl.bookmarksfly.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bj.colortex.cn

[S47] C++：结构化绑定遍历
来源：http://ks.huanxung.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hp.haigaiapp.cn

[S48] C++：逐行读文件
来源：http://hz.jianghongdianzi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ia.szxytkj.cn

while (std::getline(in, line)) { }
来源：http://bj.hnjuh.cn

[S49] C++：写文件
来源：http://yi.jianghongdianzi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fm.521024.cn

[S50] C++：格式化数字
来源：http://xg.nicolike.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uk.huixiangedu.cn

[S51] C++：显式类型转换
来源：http://zr.nicolike.cn

static_cast<double>(a) / b
来源：http://gv.jctech888.com.cn

[S52] C++：const 与 noexcept
来源：http://lt.lnxyls.cn

int size() const noexcept { return n_; }
来源：http://oh.muxihuayi.cn

[S53] C++：移动语义
来源：http://ij.bjjhwx.cn

std::vector<int> w = std::move(v);
来源：http://ui.huixiangedu.cn

[S54] C++：异常处理
来源：http://al.521024.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xj.panjiajie.cn

[S55] C++：结构化绑定
来源：http://mm.haigaiapp.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xl.jianghongdianzi.cn

[S56] C++：optional
来源：http://lt.newstarts.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://aj.jctech888.com.cn

[S57] C++：编译期常量
来源：http://pw.nicolike.cn

constexpr int N = 10;
来源：http://uz.muxihuayi.cn

[S58] C++：命名空间
来源：http://yb.haigaiapp.cn

namespace ns { int f() { return 1; } }
来源：http://cu.chemitech.net.cn

[S59] C++：静态断言
来源：http://nh.yuntaijiaju.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kc.jianghongdianzi.cn

[S60] C++：遍历并删除元素
来源：http://et.panjiajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://aj.shxzukj.cn

================================================================================
来源：http://bj.shtwfgs.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zb.hnjuh.cn

================================================================================
来源：http://yb.colortex.cn

[T01] Kotlin：Hello World
来源：http://da.muxihuayi.cn

println("Hello")
来源：http://md.shxzukj.cn

[T02] Kotlin：变量
来源：http://ml.chemitech.net.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gy.521024.cn

[T03] Kotlin：字符串模板
来源：http://sc.hnjuh.cn

"值: $b"
来源：http://im.yuntaijiaju.cn

[T04] Kotlin：空安全
来源：http://er.hnjuh.cn

val n: String? = null;  n?.length
来源：http://dy.colortex.cn

[T05] Kotlin：when 表达式
来源：http://zg.haigaiapp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zq.jianghongdianzi.cn

[T06] Kotlin：集合映射
来源：http://hp.yuexingan06.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rv.hahajie.cn

[T07] Kotlin：集合过滤
来源：http://sy.gzmigu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wj.521024.cn

[T08] Kotlin：数据类
来源：http://yi.huanxung.cn

data class User(val name: String, val age: Int)
来源：http://sh.yuexingan06.cn

[T09] Kotlin：扩展函数
来源：http://lv.nszjky.cn

fun String.exclaim() = this + "!"
来源：http://kf.asd995.cn

[T10] Kotlin：默认参数
来源：http://vb.jctech888.com.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://nj.huixinmuqiang.cn

[T11] Kotlin：协程
来源：http://qa.shxzskj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://cg.bookmarksfly.cn

[T12] Kotlin：解构声明
来源：http://qb.newstarts.cn

val (a, b) = Pair(1, 2)
来源：http://uy.nszjky.cn

[T13] Kotlin：只读 Map
来源：http://mu.shxzskj.cn

val m = mapOf("a" to 1)
来源：http://xr.shxzukj.cn

[T14] Kotlin：循环
来源：http://za.yuexingan06.cn

for (i in 1..10) println(i)
来源：http://jz.lnxyls.cn

[T15] Kotlin：接口
来源：http://ro.bookmarksfly.cn

interface Shape { fun area(): Double }
来源：http://em.521024.cn

[T16] Swift：Hello World
来源：http://ro.yuexingan06.cn

print("Hello")
来源：http://wz.shtwfgs.cn

[T17] Swift：变量与常量
来源：http://km.asd995.cn

var a = 1;  let b = 2
来源：http://kj.szsharing.cn

[T18] Swift：字符串插值
来源：http://ro.colortex.cn

"值: \(b)"
来源：http://xw.bjjhwx.cn

[T19] Swift：可选绑定
来源：http://kx.bjjhwx.cn

if let n = opt { print(n) }
来源：http://yf.shxzskj.cn

[T20] Swift：数组操作
来源：http://co.hahajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://af.huixiangedu.cn

[T21] Swift：遍历
来源：http://zx.chemitech.net.cn

for x in a { print(x) }
来源：http://ug.huixiangedu.cn

[T22] Swift：字典
来源：http://kn.muxihuayi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://wb.9csxet.cn

[T23] Swift：函数
来源：http://yj.jianghongdianzi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qr.521024.cn

[T24] Swift：闭包
来源：http://dt.shxzskj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://hd.hahajie.cn

[T25] Swift：结构体
来源：http://pa.huixinmuqiang.cn

struct P { var x: Int }
来源：http://pi.shtwfgs.cn

[T26] Swift：类与重写
来源：http://rv.nicolike.cn

class A: Base { override func f() {} }
来源：http://ys.jianghongdianzi.cn

[T27] Swift：错误处理
来源：http://mc.bookmarksfly.cn

do { try f() } catch { print(error) }
来源：http://ji.9csxet.cn

[T28] Swift：枚举
来源：http://qp.hnjuh.cn

enum Color { case red, green }
来源：http://vo.shxzskj.cn

[T29] Swift：guard 提前返回
来源：http://rk.shtwfgs.cn

guard let x = opt else { return }
来源：http://rq.gzmigu.cn

[T30] Swift：协议
来源：http://vk.hahajie.cn

protocol Shape { func area() -> Double }
来源：http://nj.bookmarksfly.cn

[T31] Lua：Hello World
来源：http://kn.chemitech.net.cn

print("Hello")
来源：http://sa.gzmigu.cn

[T32] Lua：局部变量
来源：http://sn.hnjuh.cn

local a = 1
来源：http://me.szxytkj.cn

[T33] Lua：表（数组）
来源：http://dg.521024.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vs.chemitech.net.cn

[T34] Lua：遍历表
来源：http://fu.nszjky.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://uz.yuntaijiaju.cn

[T35] Lua：字典表
来源：http://ib.szxytkj.cn

local d = { a = 1 };  d.b = 2
来源：http://tw.521024.cn

[T36] Lua：函数
来源：http://xo.huixiangedu.cn

function add(a, b) return a + b end
来源：http://oa.newstarts.cn

[T37] Lua：字符串拼接
来源：http://pf.shtwfgs.cn

"a" .. "b"
来源：http://qn.yuexingan06.cn

[T38] Lua：条件
来源：http://dc.wgjwhj.cn

if x > 0 then print("正") end
来源：http://sm.wgjwhj.cn

[T39] Lua：模式匹配
来源：http://hu.hnjuh.cn

string.find(s, "%d+")
来源：http://nv.huixiangedu.cn

[T40] Lua：元表
来源：http://hz.gzmigu.cn

setmetatable({}, { __index = base })
来源：http://ht.shxzskj.cn

[T41] Perl：Hello World
来源：http://hu.jianghongdianzi.cn

print "Hello\n";
来源：http://eg.panjiajie.cn

[T42] Perl：变量类型
来源：http://bb.colortex.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kg.wgjwhj.cn

[T43] Perl：字符串插值
来源：http://ho.bookmarksfly.cn

"值: $a"
来源：http://ni.szsharing.cn

[T44] Perl：条件
来源：http://zu.jctech888.com.cn

if ($a > 0) { print "正"; }
来源：http://cb.hnjuh.cn

[T45] Perl：数组遍历
来源：http://uc.shxzskj.cn

for my $x (@arr) { print $x; }
来源：http://vq.yuntaijiaju.cn

[T46] Perl：哈希操作
来源：http://rc.bookmarksfly.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lh.shxzskj.cn

[T47] Perl：正则捕获
来源：http://jr.shtwfgs.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vc.huanxung.cn

[T48] Perl：正则替换
来源：http://si.bjjhwx.cn

$s =~ s/old/new/g;
来源：http://ki.jctech888.com.cn

[T49] Perl：函数
来源：http://ca.huanxung.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lo.nicolike.cn

[T50] Perl：逐行读文件
来源：http://hs.szsharing.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rz.panjiajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://ax.szxytkj.cn

[T51] Scala：Hello World
来源：http://uf.shxzukj.cn

println("Hello")
来源：http://jj.shxzskj.cn

[T52] Scala：变量
来源：http://hl.asd995.cn

val a = 1;  var b = 2
来源：http://to.521024.cn

[T53] Scala：字符串插值
来源：http://mh.bjjhwx.cn

s"值: $b"
来源：http://fu.muxihuayi.cn

[T54] Scala：集合映射
来源：http://qw.yuntaijiaju.cn

List(1, 2, 3).map(_ * 2)
来源：http://va.521024.cn

[T55] Scala：集合过滤
来源：http://xl.muxihuayi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://vm.yuexingan06.cn

[T56] Scala：样例类
来源：http://qf.shxzskj.cn

case class User(name: String, age: Int)
来源：http://tm.newstarts.cn

[T57] Scala：模式匹配
来源：http://rw.shxzukj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ch.yuntaijiaju.cn

[T58] Scala：函数定义
来源：http://xp.wgjwhj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://lx.colortex.cn

[T59] Scala：循环
来源：http://dd.newstarts.cn

for (i <- 1 to 10) println(i)
来源：http://jo.haigaiapp.cn

[T60] Scala：折叠
来源：http://jl.gzmigu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ur.yuntaijiaju.cn

================================================================================
来源：http://ib.yuexingan06.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wr.huanxung.cn

================================================================================
来源：http://wv.lnxyls.cn

[U01] Py：创建虚拟环境
来源：http://qw.wgjwhj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://rh.jianghongdianzi.cn

[U02] Py：导出 / 安装依赖
来源：http://cz.bookmarksfly.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rb.hahajie.cn

[U03] Py：加载 .env 配置
来源：http://yo.muxihuayi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ko.asd995.cn

[U04] Py：变量调试打印
来源：http://eo.yuexingan06.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://uu.muxihuayi.cn

[U05] Py：列表去重且保序
来源：http://xz.9csxet.cn

list(dict.fromkeys(arr))
来源：http://ys.huixiangedu.cn

[U06] Py：合并两个字典
来源：http://hj.521024.cn

{**a, **b}
来源：http://kj.szxytkj.cn

[U07] Py：反转字典键值
来源：http://dx.521024.cn

{v: k for k, v in d.items()}
来源：http://gk.jctech888.com.cn

[U08] Py：展平二维列表
来源：http://zi.asd995.cn

[y for x in nested for y in x]
来源：http://jg.bookmarksfly.cn

[U09] Py：字典取最大值的键
来源：http://dn.chemitech.net.cn

max(d, key=d.get)
来源：http://ou.newstarts.cn

[U10] Py：按值排序字典
来源：http://eo.colortex.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kd.huixinmuqiang.cn

[U11] Py：生成器表达式
来源：http://xc.newstarts.cn

(x * 2 for x in arr)
来源：http://ix.szsharing.cn

[U12] Py：取出现最多的 3 个元素
来源：http://cm.huanxung.cn

Counter(arr).most_common(3)
来源：http://pt.lnxyls.cn

[U13] Py：固定长度队列
来源：http://rv.lnxyls.cn

deque(maxlen=10)
来源：http://ov.jianghongdianzi.cn

[U14] Py：分组收集到列表
来源：http://fi.bjjhwx.cn

defaultdict(list)
来源：http://ar.lnxyls.cn

[U15] Py：高精度计时
来源：http://bn.shxzukj.cn

t = time.perf_counter()
来源：http://qf.lnxyls.cn

[U16] Py：命令行参数解析
来源：http://qc.asd995.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pf.gzmigu.cn

[U17] Py：初始化日志
来源：http://kf.521024.cn

logging.basicConfig(level=logging.INFO)
来源：http://ug.newstarts.cn

[U18] Py：预编译正则
来源：http://ld.chemitech.net.cn

pat = re.compile(r"\d+")
来源：http://ue.jianghongdianzi.cn

[U19] Py：正则替换带回调
来源：http://nm.huixiangedu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sa.gzmigu.cn

[U20] Py：缓存函数结果
来源：http://ss.jctech888.com.cn

@functools.lru_cache(maxsize=None)
来源：http://rp.521024.cn

[U21] Py：自定义上下文管理器
来源：http://on.jianghongdianzi.cn

@contextlib.contextmanager
来源：http://jn.shxzskj.cn

[U22] Py：矩阵转置
来源：http://cg.jianghongdianzi.cn

list(zip(*m))
来源：http://cx.muxihuayi.cn


<!-- 参考信息 -->