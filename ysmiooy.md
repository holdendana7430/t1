代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://qa.jianghongdianzi.cn

[S02] C：变量与格式化输出
来源：http://ck.yuexingan06.cn

int a = 10; printf("%d\n", a);
来源：http://ea.chemitech.net.cn

[S03] C：读入整数
来源：http://yw.lnxyls.cn

int x; scanf("%d", &x);
来源：http://cj.chemitech.net.cn

[S04] C：字符串复制
来源：http://vv.hahajie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://oc.huanxung.cn

[S05] C：字符串长度
来源：http://ev.yuexingan06.cn

strlen(s)
来源：http://xv.huixinmuqiang.cn

[S06] C：字符串比较
来源：http://zk.panjiajie.cn

strcmp(a, b) == 0
来源：http://zo.nicolike.cn

[S07] C：数组遍历求和
来源：http://io.gzmigu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rg.newstarts.cn

[S08] C：动态内存分配与释放
来源：http://jw.panjiajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pp.nicolike.cn

[S09] C：结构体定义与初始化
来源：http://nq.521024.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://td.newstarts.cn

[S10] C：指针与解引用
来源：http://ot.asd995.cn

int *p = &a;  *p = 5;
来源：http://gv.bookmarksfly.cn

[S11] C：逐行读文件
来源：http://kx.hnjuh.cn

FILE *f = fopen("a.txt", "r");
来源：http://lz.nicolike.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ev.szsharing.cn

fclose(f);
来源：http://hl.newstarts.cn

[S12] C：写文件
来源：http://qh.gzmigu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hq.hnjuh.cn

[S13] C：宏定义
来源：http://dn.9csxet.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wx.bjjhwx.cn

[S14] C：枚举
来源：http://ku.yuntaijiaju.cn

enum Color { RED, GREEN, BLUE };
来源：http://he.wgjwhj.cn

[S15] C：类型转换
来源：http://vc.jctech888.com.cn

(double) a / b
来源：http://bq.yuexingan06.cn

[S16] C：位操作置位
来源：http://rg.jctech888.com.cn

x |= (1 << 3);
来源：http://pz.haigaiapp.cn

[S17] C：安全拼接字符串
来源：http://jd.9csxet.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://da.yuntaijiaju.cn

[S18] C：命令行参数
来源：http://yj.jctech888.com.cn

int main(int argc, char **argv)
来源：http://ca.huixinmuqiang.cn

[S19] C：快速排序
来源：http://li.haigaiapp.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zn.muxihuayi.cn

[S20] C：二分查找
来源：http://ih.huanxung.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ea.shxzskj.cn

[S21] C：字符类别判断
来源：http://gx.hahajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lq.asd995.cn

[S22] C：字符串转数字
来源：http://sr.colortex.cn

atoi("42");  strtod("3.14", NULL);
来源：http://td.nszjky.cn

[S23] C：随机数
来源：http://rr.jianghongdianzi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qy.shxzskj.cn

[S24] C：获取本地时间
来源：http://vc.jianghongdianzi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hs.yuntaijiaju.cn

[S25] C：内存拷贝
来源：http://ql.bookmarksfly.cn

memcpy(dst, src, n);
来源：http://ug.hnjuh.cn

[S26] C：内存清零
来源：http://nd.hnjuh.cn

memset(a, 0, sizeof a);
来源：http://aw.huixiangedu.cn

[S27] C：定义常量
来源：http://jy.yuexingan06.cn

const double PI = 3.14159;
来源：http://ny.chemitech.net.cn

[S28] C：静态变量
来源：http://zw.chemitech.net.cn

static int counter = 0;
来源：http://ah.jianghongdianzi.cn

[S29] C：变参函数
来源：http://eg.bjjhwx.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bi.bjjhwx.cn

[S30] C：头文件保护
来源：http://yn.bookmarksfly.cn

#ifndef X_H
来源：http://lc.nszjky.cn

#define X_H
来源：http://zf.chemitech.net.cn

#endif
来源：http://rq.panjiajie.cn

[S31] C++：Hello World
来源：http://ns.jianghongdianzi.cn

#include <iostream>
来源：http://ii.gzmigu.cn

int main() { std::cout << "Hello\n"; }
来源：http://bb.jctech888.com.cn

[S32] C++：字符串
来源：http://hq.nszjky.cn

std::string s = "hi";  s += "!";
来源：http://tr.huixinmuqiang.cn

[S33] C++：vector 增删
来源：http://eu.shxzskj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kp.huixiangedu.cn

[S34] C++：遍历 vector
来源：http://cb.521024.cn

for (auto &x : v) { std::cout << x; }
来源：http://pq.shxzskj.cn

[S35] C++：map
来源：http://sj.hnjuh.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jl.huanxung.cn

[S36] C++：unordered_map
来源：http://jm.asd995.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dk.chemitech.net.cn

[S37] C++：set
来源：http://zy.asd995.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vr.shxzskj.cn

[S38] C++：排序
来源：http://kg.wgjwhj.cn

std::sort(v.begin(), v.end());
来源：http://xo.chemitech.net.cn

[S39] C++：自定义比较器排序
来源：http://ws.colortex.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cy.shtwfgs.cn

[S40] C++：查找元素
来源：http://io.jctech888.com.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xn.muxihuayi.cn

[S41] C++：类与构造函数
来源：http://yg.panjiajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://eg.bjjhwx.cn

[S42] C++：继承与虚函数
来源：http://nc.521024.cn

class B : public Base { public: void f() override {} };
来源：http://sn.gzmigu.cn

[S43] C++：智能指针
来源：http://wa.szsharing.cn

auto p = std::make_unique<int>(5);
来源：http://en.haigaiapp.cn

[S44] C++：引用传参
来源：http://yk.hahajie.cn

void inc(int &x) { ++x; }
来源：http://wq.huixiangedu.cn

[S45] C++：lambda
来源：http://yk.haigaiapp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fj.lnxyls.cn

[S46] C++：函数模板
来源：http://nx.nicolike.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ca.jctech888.com.cn

[S47] C++：结构化绑定遍历
来源：http://wg.huixinmuqiang.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hd.bjjhwx.cn

[S48] C++：逐行读文件
来源：http://zb.shxzskj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ol.huanxung.cn

while (std::getline(in, line)) { }
来源：http://xf.jianghongdianzi.cn

[S49] C++：写文件
来源：http://fk.gzmigu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xp.newstarts.cn

[S50] C++：格式化数字
来源：http://uo.haigaiapp.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nf.hahajie.cn

[S51] C++：显式类型转换
来源：http://lc.jctech888.com.cn

static_cast<double>(a) / b
来源：http://lu.shxzskj.cn

[S52] C++：const 与 noexcept
来源：http://qf.nicolike.cn

int size() const noexcept { return n_; }
来源：http://xt.muxihuayi.cn

[S53] C++：移动语义
来源：http://cz.nicolike.cn

std::vector<int> w = std::move(v);
来源：http://ma.yuntaijiaju.cn

[S54] C++：异常处理
来源：http://rj.huixinmuqiang.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gk.panjiajie.cn

[S55] C++：结构化绑定
来源：http://uj.bookmarksfly.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://de.shxzskj.cn

[S56] C++：optional
来源：http://xi.jctech888.com.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://om.muxihuayi.cn

[S57] C++：编译期常量
来源：http://ar.yuexingan06.cn

constexpr int N = 10;
来源：http://np.huixiangedu.cn

[S58] C++：命名空间
来源：http://pc.huixiangedu.cn

namespace ns { int f() { return 1; } }
来源：http://dt.hahajie.cn

[S59] C++：静态断言
来源：http://ma.nicolike.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lb.huixiangedu.cn

[S60] C++：遍历并删除元素
来源：http://iq.jctech888.com.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ab.chemitech.net.cn

================================================================================
来源：http://bx.huanxung.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wq.shxzskj.cn

================================================================================
来源：http://wj.gzmigu.cn

[T01] Kotlin：Hello World
来源：http://qm.nszjky.cn

println("Hello")
来源：http://ts.panjiajie.cn

[T02] Kotlin：变量
来源：http://vd.hahajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uj.nicolike.cn

[T03] Kotlin：字符串模板
来源：http://la.lnxyls.cn

"值: $b"
来源：http://fg.shtwfgs.cn

[T04] Kotlin：空安全
来源：http://nb.chemitech.net.cn

val n: String? = null;  n?.length
来源：http://wy.bookmarksfly.cn

[T05] Kotlin：when 表达式
来源：http://qs.huixinmuqiang.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hu.jctech888.com.cn

[T06] Kotlin：集合映射
来源：http://bu.shxzukj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xo.jianghongdianzi.cn

[T07] Kotlin：集合过滤
来源：http://jn.9csxet.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://rh.newstarts.cn

[T08] Kotlin：数据类
来源：http://vf.bjjhwx.cn

data class User(val name: String, val age: Int)
来源：http://in.yuexingan06.cn

[T09] Kotlin：扩展函数
来源：http://iu.huixinmuqiang.cn

fun String.exclaim() = this + "!"
来源：http://vl.colortex.cn

[T10] Kotlin：默认参数
来源：http://if.lnxyls.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ns.jctech888.com.cn

[T11] Kotlin：协程
来源：http://np.shxzskj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://lo.szxytkj.cn

[T12] Kotlin：解构声明
来源：http://wo.nszjky.cn

val (a, b) = Pair(1, 2)
来源：http://ba.colortex.cn

[T13] Kotlin：只读 Map
来源：http://ba.asd995.cn

val m = mapOf("a" to 1)
来源：http://co.szsharing.cn

[T14] Kotlin：循环
来源：http://oe.haigaiapp.cn

for (i in 1..10) println(i)
来源：http://oz.haigaiapp.cn

[T15] Kotlin：接口
来源：http://kv.hahajie.cn

interface Shape { fun area(): Double }
来源：http://xn.muxihuayi.cn

[T16] Swift：Hello World
来源：http://lr.yuntaijiaju.cn

print("Hello")
来源：http://vr.huanxung.cn

[T17] Swift：变量与常量
来源：http://gx.muxihuayi.cn

var a = 1;  let b = 2
来源：http://kf.gzmigu.cn

[T18] Swift：字符串插值
来源：http://uv.szsharing.cn

"值: \(b)"
来源：http://js.panjiajie.cn

[T19] Swift：可选绑定
来源：http://uj.szxytkj.cn

if let n = opt { print(n) }
来源：http://nk.asd995.cn

[T20] Swift：数组操作
来源：http://xp.szxytkj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://dy.wgjwhj.cn

[T21] Swift：遍历
来源：http://zv.hnjuh.cn

for x in a { print(x) }
来源：http://az.lnxyls.cn

[T22] Swift：字典
来源：http://zx.haigaiapp.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ta.asd995.cn

[T23] Swift：函数
来源：http://to.colortex.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://od.asd995.cn

[T24] Swift：闭包
来源：http://iu.szxytkj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://bg.huixiangedu.cn

[T25] Swift：结构体
来源：http://kk.shxzukj.cn

struct P { var x: Int }
来源：http://xm.shxzukj.cn

[T26] Swift：类与重写
来源：http://jn.szsharing.cn

class A: Base { override func f() {} }
来源：http://gy.bjjhwx.cn

[T27] Swift：错误处理
来源：http://au.shxzukj.cn

do { try f() } catch { print(error) }
来源：http://vl.hahajie.cn

[T28] Swift：枚举
来源：http://vs.wgjwhj.cn

enum Color { case red, green }
来源：http://vc.chemitech.net.cn

[T29] Swift：guard 提前返回
来源：http://fp.huanxung.cn

guard let x = opt else { return }
来源：http://ks.jctech888.com.cn

[T30] Swift：协议
来源：http://ua.szsharing.cn

protocol Shape { func area() -> Double }
来源：http://da.9csxet.cn

[T31] Lua：Hello World
来源：http://wt.bjjhwx.cn

print("Hello")
来源：http://od.nicolike.cn

[T32] Lua：局部变量
来源：http://sz.asd995.cn

local a = 1
来源：http://ty.shxzukj.cn

[T33] Lua：表（数组）
来源：http://uy.shxzskj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://gy.szxytkj.cn

[T34] Lua：遍历表
来源：http://do.huanxung.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gh.shxzukj.cn

[T35] Lua：字典表
来源：http://jx.shtwfgs.cn

local d = { a = 1 };  d.b = 2
来源：http://ef.panjiajie.cn

[T36] Lua：函数
来源：http://tn.muxihuayi.cn

function add(a, b) return a + b end
来源：http://vy.szsharing.cn

[T37] Lua：字符串拼接
来源：http://uf.asd995.cn

"a" .. "b"
来源：http://lj.hnjuh.cn

[T38] Lua：条件
来源：http://gd.lnxyls.cn

if x > 0 then print("正") end
来源：http://cy.shtwfgs.cn

[T39] Lua：模式匹配
来源：http://rb.bookmarksfly.cn

string.find(s, "%d+")
来源：http://sk.panjiajie.cn

[T40] Lua：元表
来源：http://qq.panjiajie.cn

setmetatable({}, { __index = base })
来源：http://co.bookmarksfly.cn

[T41] Perl：Hello World
来源：http://uh.wgjwhj.cn

print "Hello\n";
来源：http://cn.haigaiapp.cn

[T42] Perl：变量类型
来源：http://tp.521024.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fq.521024.cn

[T43] Perl：字符串插值
来源：http://dd.huixiangedu.cn

"值: $a"
来源：http://cu.huanxung.cn

[T44] Perl：条件
来源：http://ha.gzmigu.cn

if ($a > 0) { print "正"; }
来源：http://mr.muxihuayi.cn

[T45] Perl：数组遍历
来源：http://vf.lnxyls.cn

for my $x (@arr) { print $x; }
来源：http://jd.wgjwhj.cn

[T46] Perl：哈希操作
来源：http://vn.9csxet.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vq.huixiangedu.cn

[T47] Perl：正则捕获
来源：http://ic.muxihuayi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://mu.yuntaijiaju.cn

[T48] Perl：正则替换
来源：http://eo.yuexingan06.cn

$s =~ s/old/new/g;
来源：http://jk.9csxet.cn

[T49] Perl：函数
来源：http://on.gzmigu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pv.huixiangedu.cn

[T50] Perl：逐行读文件
来源：http://lu.haigaiapp.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fr.huixiangedu.cn

while (my $line = <$fh>) { print $line; }
来源：http://ci.newstarts.cn

[T51] Scala：Hello World
来源：http://qs.szxytkj.cn

println("Hello")
来源：http://dw.521024.cn

[T52] Scala：变量
来源：http://nf.bjjhwx.cn

val a = 1;  var b = 2
来源：http://aj.szxytkj.cn

[T53] Scala：字符串插值
来源：http://iz.szxytkj.cn

s"值: $b"
来源：http://yt.shxzukj.cn

[T54] Scala：集合映射
来源：http://sv.bjjhwx.cn

List(1, 2, 3).map(_ * 2)
来源：http://vz.521024.cn

[T55] Scala：集合过滤
来源：http://kz.gzmigu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://cw.jctech888.com.cn

[T56] Scala：样例类
来源：http://ww.huanxung.cn

case class User(name: String, age: Int)
来源：http://et.521024.cn

[T57] Scala：模式匹配
来源：http://ms.9csxet.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://px.shtwfgs.cn

[T58] Scala：函数定义
来源：http://zp.nszjky.cn

def add(a: Int, b: Int): Int = a + b
来源：http://nh.nicolike.cn

[T59] Scala：循环
来源：http://al.shxzukj.cn

for (i <- 1 to 10) println(i)
来源：http://nq.colortex.cn

[T60] Scala：折叠
来源：http://xf.521024.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://le.huanxung.cn

================================================================================
来源：http://ow.hahajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pn.haigaiapp.cn

================================================================================
来源：http://uo.wgjwhj.cn

[U01] Py：创建虚拟环境
来源：http://se.shxzukj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://as.szxytkj.cn

[U02] Py：导出 / 安装依赖
来源：http://pe.huanxung.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fb.9csxet.cn

[U03] Py：加载 .env 配置
来源：http://dg.lnxyls.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zj.wgjwhj.cn

[U04] Py：变量调试打印
来源：http://su.panjiajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jh.huanxung.cn

[U05] Py：列表去重且保序
来源：http://ca.shxzukj.cn

list(dict.fromkeys(arr))
来源：http://rf.haigaiapp.cn

[U06] Py：合并两个字典
来源：http://dc.shxzukj.cn

{**a, **b}
来源：http://db.newstarts.cn

[U07] Py：反转字典键值
来源：http://bb.huixinmuqiang.cn

{v: k for k, v in d.items()}
来源：http://il.bjjhwx.cn

[U08] Py：展平二维列表
来源：http://tc.bjjhwx.cn

[y for x in nested for y in x]
来源：http://hf.chemitech.net.cn

[U09] Py：字典取最大值的键
来源：http://mj.bjjhwx.cn

max(d, key=d.get)
来源：http://us.muxihuayi.cn

[U10] Py：按值排序字典
来源：http://cx.nszjky.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gg.shxzskj.cn

[U11] Py：生成器表达式
来源：http://il.bookmarksfly.cn

(x * 2 for x in arr)
来源：http://cv.colortex.cn

[U12] Py：取出现最多的 3 个元素
来源：http://bp.muxihuayi.cn

Counter(arr).most_common(3)
来源：http://bj.9csxet.cn

[U13] Py：固定长度队列
来源：http://ht.huixiangedu.cn

deque(maxlen=10)
来源：http://xv.521024.cn

[U14] Py：分组收集到列表
来源：http://lt.szsharing.cn

defaultdict(list)
来源：http://dv.szsharing.cn

[U15] Py：高精度计时
来源：http://fx.lnxyls.cn

t = time.perf_counter()
来源：http://ap.hnjuh.cn

[U16] Py：命令行参数解析
来源：http://jj.szsharing.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ac.yuexingan06.cn

[U17] Py：初始化日志
来源：http://kv.muxihuayi.cn

logging.basicConfig(level=logging.INFO)
来源：http://ql.panjiajie.cn

[U18] Py：预编译正则
来源：http://va.haigaiapp.cn

pat = re.compile(r"\d+")
来源：http://oa.jctech888.com.cn

[U19] Py：正则替换带回调
来源：http://ct.huanxung.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yj.shxzskj.cn

[U20] Py：缓存函数结果
来源：http://kb.chemitech.net.cn

@functools.lru_cache(maxsize=None)
来源：http://mp.nicolike.cn

[U21] Py：自定义上下文管理器
来源：http://ic.chemitech.net.cn

@contextlib.contextmanager
来源：http://bl.colortex.cn

[U22] Py：矩阵转置
来源：http://si.jianghongdianzi.cn

list(zip(*m))
来源：http://ku.shxzukj.cn

[U23] Py：分块读取大文件
来源：http://tx.szsharing.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xv.newstarts.cn

[U24] Py：路径操作
来源：http://lf.bookmarksfly.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qw.haigaiapp.cn


<!-- 参考信息 -->