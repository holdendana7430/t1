代发 wailian999

S. C / C++ 专题
来源：http://kd.yuntaijiaju.cn

================================================================================
来源：http://cq.szxytkj.cn

[S01] C：Hello World
来源：http://to.shxzskj.cn

#include <stdio.h>
来源：http://jd.hnjuh.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ej.huixiangedu.cn

[S02] C：变量与格式化输出
来源：http://cl.lnxyls.cn

int a = 10; printf("%d\n", a);
来源：http://ml.yuntaijiaju.cn

[S03] C：读入整数
来源：http://ay.hnjuh.cn

int x; scanf("%d", &x);
来源：http://qf.huixinmuqiang.cn

[S04] C：字符串复制
来源：http://te.hnjuh.cn

char dst[32]; strcpy(dst, "hi");
来源：http://cv.panjiajie.cn

[S05] C：字符串长度
来源：http://ul.huixinmuqiang.cn

strlen(s)
来源：http://mt.haigaiapp.cn

[S06] C：字符串比较
来源：http://hh.jianghongdianzi.cn

strcmp(a, b) == 0
来源：http://ty.9csxet.cn

[S07] C：数组遍历求和
来源：http://vj.wgjwhj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ww.shxzukj.cn

[S08] C：动态内存分配与释放
来源：http://zn.nicolike.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ia.panjiajie.cn

[S09] C：结构体定义与初始化
来源：http://uz.wgjwhj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ls.shxzukj.cn

[S10] C：指针与解引用
来源：http://wk.panjiajie.cn

int *p = &a;  *p = 5;
来源：http://er.huixinmuqiang.cn

[S11] C：逐行读文件
来源：http://ff.shxzukj.cn

FILE *f = fopen("a.txt", "r");
来源：http://an.muxihuayi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mf.asd995.cn

fclose(f);
来源：http://bi.wgjwhj.cn

[S12] C：写文件
来源：http://tv.colortex.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rw.shtwfgs.cn

[S13] C：宏定义
来源：http://fw.huixinmuqiang.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dl.newstarts.cn

[S14] C：枚举
来源：http://im.shxzukj.cn

enum Color { RED, GREEN, BLUE };
来源：http://gv.muxihuayi.cn

[S15] C：类型转换
来源：http://jk.wgjwhj.cn

(double) a / b
来源：http://jv.szxytkj.cn

[S16] C：位操作置位
来源：http://lg.haigaiapp.cn

x |= (1 << 3);
来源：http://sv.huixinmuqiang.cn

[S17] C：安全拼接字符串
来源：http://zr.bookmarksfly.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qw.haigaiapp.cn

[S18] C：命令行参数
来源：http://dx.jctech888.com.cn

int main(int argc, char **argv)
来源：http://kd.hnjuh.cn

[S19] C：快速排序
来源：http://yo.521024.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rr.huixiangedu.cn

[S20] C：二分查找
来源：http://jm.shxzskj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gb.shtwfgs.cn

[S21] C：字符类别判断
来源：http://ew.colortex.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dn.chemitech.net.cn

[S22] C：字符串转数字
来源：http://mj.szxytkj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cr.huanxung.cn

[S23] C：随机数
来源：http://bp.yuntaijiaju.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qi.gzmigu.cn

[S24] C：获取本地时间
来源：http://tr.panjiajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hu.yuexingan06.cn

[S25] C：内存拷贝
来源：http://tl.huixiangedu.cn

memcpy(dst, src, n);
来源：http://tc.huixiangedu.cn

[S26] C：内存清零
来源：http://uu.jianghongdianzi.cn

memset(a, 0, sizeof a);
来源：http://yt.huanxung.cn

[S27] C：定义常量
来源：http://bu.huanxung.cn

const double PI = 3.14159;
来源：http://ho.521024.cn

[S28] C：静态变量
来源：http://od.bookmarksfly.cn

static int counter = 0;
来源：http://vc.bjjhwx.cn

[S29] C：变参函数
来源：http://ar.muxihuayi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gn.asd995.cn

[S30] C：头文件保护
来源：http://pi.haigaiapp.cn

#ifndef X_H
来源：http://jv.jctech888.com.cn

#define X_H
来源：http://xp.shxzukj.cn

#endif
来源：http://wn.9csxet.cn

[S31] C++：Hello World
来源：http://on.jianghongdianzi.cn

#include <iostream>
来源：http://pb.yuexingan06.cn

int main() { std::cout << "Hello\n"; }
来源：http://io.yuexingan06.cn

[S32] C++：字符串
来源：http://oe.chemitech.net.cn

std::string s = "hi";  s += "!";
来源：http://zm.asd995.cn

[S33] C++：vector 增删
来源：http://ew.nicolike.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://da.wgjwhj.cn

[S34] C++：遍历 vector
来源：http://gc.hnjuh.cn

for (auto &x : v) { std::cout << x; }
来源：http://nt.muxihuayi.cn

[S35] C++：map
来源：http://nu.521024.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ht.shxzskj.cn

[S36] C++：unordered_map
来源：http://nu.shxzukj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ws.hnjuh.cn

[S37] C++：set
来源：http://mb.haigaiapp.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://av.nicolike.cn

[S38] C++：排序
来源：http://gl.bjjhwx.cn

std::sort(v.begin(), v.end());
来源：http://ls.9csxet.cn

[S39] C++：自定义比较器排序
来源：http://ld.nicolike.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://th.huixinmuqiang.cn

[S40] C++：查找元素
来源：http://ce.newstarts.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nv.jianghongdianzi.cn

[S41] C++：类与构造函数
来源：http://fd.colortex.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://op.bjjhwx.cn

[S42] C++：继承与虚函数
来源：http://ik.9csxet.cn

class B : public Base { public: void f() override {} };
来源：http://dv.wgjwhj.cn

[S43] C++：智能指针
来源：http://zc.shxzskj.cn

auto p = std::make_unique<int>(5);
来源：http://hh.szxytkj.cn

[S44] C++：引用传参
来源：http://xt.yuexingan06.cn

void inc(int &x) { ++x; }
来源：http://wr.chemitech.net.cn

[S45] C++：lambda
来源：http://sx.9csxet.cn

auto add = [](int a, int b) { return a + b; };
来源：http://rh.jctech888.com.cn

[S46] C++：函数模板
来源：http://fz.shxzukj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zw.colortex.cn

[S47] C++：结构化绑定遍历
来源：http://dq.shtwfgs.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zp.hahajie.cn

[S48] C++：逐行读文件
来源：http://vr.newstarts.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wh.521024.cn

while (std::getline(in, line)) { }
来源：http://wd.521024.cn

[S49] C++：写文件
来源：http://hq.shtwfgs.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lz.nicolike.cn

[S50] C++：格式化数字
来源：http://si.bjjhwx.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ll.gzmigu.cn

[S51] C++：显式类型转换
来源：http://pa.shxzukj.cn

static_cast<double>(a) / b
来源：http://gl.wgjwhj.cn

[S52] C++：const 与 noexcept
来源：http://gh.nszjky.cn

int size() const noexcept { return n_; }
来源：http://hv.yuntaijiaju.cn

[S53] C++：移动语义
来源：http://we.9csxet.cn

std::vector<int> w = std::move(v);
来源：http://en.lnxyls.cn

[S54] C++：异常处理
来源：http://yy.bookmarksfly.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ji.huanxung.cn

[S55] C++：结构化绑定
来源：http://lc.hahajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://nq.lnxyls.cn

[S56] C++：optional
来源：http://nn.yuntaijiaju.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://li.shtwfgs.cn

[S57] C++：编译期常量
来源：http://wu.yuexingan06.cn

constexpr int N = 10;
来源：http://fc.szxytkj.cn

[S58] C++：命名空间
来源：http://no.jctech888.com.cn

namespace ns { int f() { return 1; } }
来源：http://rc.szxytkj.cn

[S59] C++：静态断言
来源：http://bq.panjiajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bk.521024.cn

[S60] C++：遍历并删除元素
来源：http://cg.chemitech.net.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://oe.gzmigu.cn

================================================================================
来源：http://kz.jctech888.com.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://da.colortex.cn

================================================================================
来源：http://mq.szsharing.cn

[T01] Kotlin：Hello World
来源：http://dj.shxzskj.cn

println("Hello")
来源：http://tq.panjiajie.cn

[T02] Kotlin：变量
来源：http://uw.lnxyls.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ao.asd995.cn

[T03] Kotlin：字符串模板
来源：http://xo.shxzskj.cn

"值: $b"
来源：http://zk.yuexingan06.cn

[T04] Kotlin：空安全
来源：http://qb.huixiangedu.cn

val n: String? = null;  n?.length
来源：http://hf.hnjuh.cn

[T05] Kotlin：when 表达式
来源：http://yg.szxytkj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pl.huanxung.cn

[T06] Kotlin：集合映射
来源：http://cp.chemitech.net.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ou.nszjky.cn

[T07] Kotlin：集合过滤
来源：http://xo.yuntaijiaju.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ac.huixiangedu.cn

[T08] Kotlin：数据类
来源：http://cn.jianghongdianzi.cn

data class User(val name: String, val age: Int)
来源：http://pr.huanxung.cn

[T09] Kotlin：扩展函数
来源：http://ci.gzmigu.cn

fun String.exclaim() = this + "!"
来源：http://fv.yuexingan06.cn

[T10] Kotlin：默认参数
来源：http://tv.panjiajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rq.szxytkj.cn

[T11] Kotlin：协程
来源：http://nv.yuexingan06.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://zz.haigaiapp.cn

[T12] Kotlin：解构声明
来源：http://aa.chemitech.net.cn

val (a, b) = Pair(1, 2)
来源：http://jq.gzmigu.cn

[T13] Kotlin：只读 Map
来源：http://yy.colortex.cn

val m = mapOf("a" to 1)
来源：http://hv.bookmarksfly.cn

[T14] Kotlin：循环
来源：http://sc.9csxet.cn

for (i in 1..10) println(i)
来源：http://rd.huanxung.cn

[T15] Kotlin：接口
来源：http://xv.szsharing.cn

interface Shape { fun area(): Double }
来源：http://ek.bookmarksfly.cn

[T16] Swift：Hello World
来源：http://yu.nicolike.cn

print("Hello")
来源：http://sp.nicolike.cn

[T17] Swift：变量与常量
来源：http://tq.nszjky.cn

var a = 1;  let b = 2
来源：http://nu.huixiangedu.cn

[T18] Swift：字符串插值
来源：http://qh.newstarts.cn

"值: \(b)"
来源：http://qf.huanxung.cn

[T19] Swift：可选绑定
来源：http://mj.521024.cn

if let n = opt { print(n) }
来源：http://vc.9csxet.cn

[T20] Swift：数组操作
来源：http://vr.chemitech.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://yk.wgjwhj.cn

[T21] Swift：遍历
来源：http://yi.nicolike.cn

for x in a { print(x) }
来源：http://nn.huixinmuqiang.cn

[T22] Swift：字典
来源：http://yn.bookmarksfly.cn

var d = ["a": 1];  d["b"] = 2
来源：http://qb.lnxyls.cn

[T23] Swift：函数
来源：http://sv.newstarts.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pa.shxzukj.cn

[T24] Swift：闭包
来源：http://fv.bookmarksfly.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gs.9csxet.cn

[T25] Swift：结构体
来源：http://pd.szsharing.cn

struct P { var x: Int }
来源：http://sm.521024.cn

[T26] Swift：类与重写
来源：http://ph.521024.cn

class A: Base { override func f() {} }
来源：http://qm.huixinmuqiang.cn

[T27] Swift：错误处理
来源：http://cp.huixiangedu.cn

do { try f() } catch { print(error) }
来源：http://al.newstarts.cn

[T28] Swift：枚举
来源：http://hl.bjjhwx.cn

enum Color { case red, green }
来源：http://uu.shtwfgs.cn

[T29] Swift：guard 提前返回
来源：http://bl.huixiangedu.cn

guard let x = opt else { return }
来源：http://pe.szsharing.cn

[T30] Swift：协议
来源：http://ew.huixiangedu.cn

protocol Shape { func area() -> Double }
来源：http://qu.nszjky.cn

[T31] Lua：Hello World
来源：http://xb.newstarts.cn

print("Hello")
来源：http://iq.huixinmuqiang.cn

[T32] Lua：局部变量
来源：http://al.9csxet.cn

local a = 1
来源：http://iw.huanxung.cn

[T33] Lua：表（数组）
来源：http://vn.szsharing.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hf.9csxet.cn

[T34] Lua：遍历表
来源：http://sx.hahajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://er.521024.cn

[T35] Lua：字典表
来源：http://fs.hnjuh.cn

local d = { a = 1 };  d.b = 2
来源：http://tl.asd995.cn

[T36] Lua：函数
来源：http://zs.haigaiapp.cn

function add(a, b) return a + b end
来源：http://mz.bookmarksfly.cn

[T37] Lua：字符串拼接
来源：http://rf.shxzskj.cn

"a" .. "b"
来源：http://pf.nicolike.cn

[T38] Lua：条件
来源：http://dw.jianghongdianzi.cn

if x > 0 then print("正") end
来源：http://ek.asd995.cn

[T39] Lua：模式匹配
来源：http://ru.panjiajie.cn

string.find(s, "%d+")
来源：http://vo.yuntaijiaju.cn

[T40] Lua：元表
来源：http://rr.szsharing.cn

setmetatable({}, { __index = base })
来源：http://yk.colortex.cn

[T41] Perl：Hello World
来源：http://pk.szsharing.cn

print "Hello\n";
来源：http://ec.muxihuayi.cn

[T42] Perl：变量类型
来源：http://hy.hahajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ro.nicolike.cn

[T43] Perl：字符串插值
来源：http://rl.haigaiapp.cn

"值: $a"
来源：http://ln.asd995.cn

[T44] Perl：条件
来源：http://he.asd995.cn

if ($a > 0) { print "正"; }
来源：http://lw.colortex.cn

[T45] Perl：数组遍历
来源：http://ko.panjiajie.cn

for my $x (@arr) { print $x; }
来源：http://de.hahajie.cn

[T46] Perl：哈希操作
来源：http://pb.muxihuayi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bj.hahajie.cn

[T47] Perl：正则捕获
来源：http://su.muxihuayi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://sd.shxzskj.cn

[T48] Perl：正则替换
来源：http://id.jianghongdianzi.cn

$s =~ s/old/new/g;
来源：http://lc.9csxet.cn

[T49] Perl：函数
来源：http://nc.nicolike.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://du.bookmarksfly.cn

[T50] Perl：逐行读文件
来源：http://nv.huixinmuqiang.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://pl.hnjuh.cn

while (my $line = <$fh>) { print $line; }
来源：http://nn.colortex.cn

[T51] Scala：Hello World
来源：http://cv.huixinmuqiang.cn

println("Hello")
来源：http://lx.szxytkj.cn

[T52] Scala：变量
来源：http://np.huixiangedu.cn

val a = 1;  var b = 2
来源：http://nm.gzmigu.cn

[T53] Scala：字符串插值
来源：http://fy.shtwfgs.cn

s"值: $b"
来源：http://xy.nszjky.cn

[T54] Scala：集合映射
来源：http://ej.nszjky.cn

List(1, 2, 3).map(_ * 2)
来源：http://im.jctech888.com.cn

[T55] Scala：集合过滤
来源：http://zi.yuntaijiaju.cn

List(1, 2, 3).filter(_ > 1)
来源：http://pl.hahajie.cn

[T56] Scala：样例类
来源：http://re.bjjhwx.cn

case class User(name: String, age: Int)
来源：http://ie.yuexingan06.cn

[T57] Scala：模式匹配
来源：http://wu.muxihuayi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tr.huixiangedu.cn

[T58] Scala：函数定义
来源：http://jv.muxihuayi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://lm.9csxet.cn

[T59] Scala：循环
来源：http://gn.521024.cn

for (i <- 1 to 10) println(i)
来源：http://pn.bjjhwx.cn

[T60] Scala：折叠
来源：http://js.wgjwhj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pt.panjiajie.cn

================================================================================
来源：http://lh.yuntaijiaju.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tk.shxzskj.cn

================================================================================
来源：http://wt.muxihuayi.cn

[U01] Py：创建虚拟环境
来源：http://oq.haigaiapp.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mn.panjiajie.cn

[U02] Py：导出 / 安装依赖
来源：http://wb.shtwfgs.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qo.jctech888.com.cn

[U03] Py：加载 .env 配置
来源：http://xy.wgjwhj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://dp.jctech888.com.cn

[U04] Py：变量调试打印
来源：http://st.colortex.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ce.521024.cn

[U05] Py：列表去重且保序
来源：http://hy.chemitech.net.cn

list(dict.fromkeys(arr))
来源：http://wi.521024.cn

[U06] Py：合并两个字典
来源：http://wt.jctech888.com.cn

{**a, **b}
来源：http://zz.colortex.cn

[U07] Py：反转字典键值
来源：http://ya.huixiangedu.cn

{v: k for k, v in d.items()}
来源：http://no.szxytkj.cn

[U08] Py：展平二维列表
来源：http://tf.9csxet.cn

[y for x in nested for y in x]
来源：http://eo.nszjky.cn

[U09] Py：字典取最大值的键
来源：http://qy.jianghongdianzi.cn

max(d, key=d.get)
来源：http://df.szxytkj.cn

[U10] Py：按值排序字典
来源：http://lp.lnxyls.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ic.yuexingan06.cn

[U11] Py：生成器表达式
来源：http://jm.huanxung.cn

(x * 2 for x in arr)
来源：http://bf.9csxet.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mc.shtwfgs.cn

Counter(arr).most_common(3)
来源：http://ws.bjjhwx.cn

[U13] Py：固定长度队列
来源：http://vk.szsharing.cn

deque(maxlen=10)
来源：http://ro.muxihuayi.cn

[U14] Py：分组收集到列表
来源：http://my.jctech888.com.cn

defaultdict(list)
来源：http://qw.shxzukj.cn

[U15] Py：高精度计时
来源：http://fh.panjiajie.cn

t = time.perf_counter()
来源：http://rf.haigaiapp.cn

[U16] Py：命令行参数解析
来源：http://je.bookmarksfly.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vt.huanxung.cn

[U17] Py：初始化日志
来源：http://ss.bookmarksfly.cn

logging.basicConfig(level=logging.INFO)
来源：http://mh.huixiangedu.cn

[U18] Py：预编译正则
来源：http://rq.szsharing.cn

pat = re.compile(r"\d+")
来源：http://td.9csxet.cn

[U19] Py：正则替换带回调
来源：http://jk.colortex.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sm.haigaiapp.cn

[U20] Py：缓存函数结果
来源：http://nz.wgjwhj.cn

@functools.lru_cache(maxsize=None)
来源：http://nj.wgjwhj.cn

[U21] Py：自定义上下文管理器
来源：http://ai.hnjuh.cn

@contextlib.contextmanager
来源：http://yj.hahajie.cn

[U22] Py：矩阵转置
来源：http://ng.shxzukj.cn

list(zip(*m))
来源：http://ql.muxihuayi.cn


<!-- 参考信息 -->