代发 wailian999

strlen(s)
来源：http://gz.colortex.cn

[S06] C：字符串比较
来源：http://nu.wgjwhj.cn

strcmp(a, b) == 0
来源：http://dy.haigaiapp.cn

[S07] C：数组遍历求和
来源：http://xp.szsharing.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yl.hahajie.cn

[S08] C：动态内存分配与释放
来源：http://wf.yuexingan06.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://oo.bookmarksfly.cn

[S09] C：结构体定义与初始化
来源：http://sh.muxihuayi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zh.yuexingan06.cn

[S10] C：指针与解引用
来源：http://vy.huixinmuqiang.cn

int *p = &a;  *p = 5;
来源：http://ax.newstarts.cn

[S11] C：逐行读文件
来源：http://xx.bookmarksfly.cn

FILE *f = fopen("a.txt", "r");
来源：http://kr.9csxet.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xa.asd995.cn

fclose(f);
来源：http://ku.muxihuayi.cn

[S12] C：写文件
来源：http://cp.nicolike.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fg.shtwfgs.cn

[S13] C：宏定义
来源：http://lv.shxzskj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hs.bookmarksfly.cn

[S14] C：枚举
来源：http://ts.colortex.cn

enum Color { RED, GREEN, BLUE };
来源：http://sy.jianghongdianzi.cn

[S15] C：类型转换
来源：http://ey.gzmigu.cn

(double) a / b
来源：http://ik.9csxet.cn

[S16] C：位操作置位
来源：http://ie.huanxung.cn

x |= (1 << 3);
来源：http://hn.bjjhwx.cn

[S17] C：安全拼接字符串
来源：http://bp.9csxet.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://am.asd995.cn

[S18] C：命令行参数
来源：http://wv.colortex.cn

int main(int argc, char **argv)
来源：http://ku.bookmarksfly.cn

[S19] C：快速排序
来源：http://ba.huixinmuqiang.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ud.9csxet.cn

[S20] C：二分查找
来源：http://ht.wgjwhj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zk.wgjwhj.cn

[S21] C：字符类别判断
来源：http://wz.muxihuayi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nk.muxihuayi.cn

[S22] C：字符串转数字
来源：http://ck.jianghongdianzi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://hi.bjjhwx.cn

[S23] C：随机数
来源：http://rt.shxzskj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bo.panjiajie.cn

[S24] C：获取本地时间
来源：http://ie.newstarts.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xd.panjiajie.cn

[S25] C：内存拷贝
来源：http://ul.newstarts.cn

memcpy(dst, src, n);
来源：http://st.haigaiapp.cn

[S26] C：内存清零
来源：http://ct.nicolike.cn

memset(a, 0, sizeof a);
来源：http://gu.hahajie.cn

[S27] C：定义常量
来源：http://vb.bookmarksfly.cn

const double PI = 3.14159;
来源：http://es.asd995.cn

[S28] C：静态变量
来源：http://jn.nszjky.cn

static int counter = 0;
来源：http://su.huixinmuqiang.cn

[S29] C：变参函数
来源：http://tz.bjjhwx.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zk.jctech888.com.cn

[S30] C：头文件保护
来源：http://wq.bookmarksfly.cn

#ifndef X_H
来源：http://bl.wgjwhj.cn

#define X_H
来源：http://ny.nicolike.cn

#endif
来源：http://xr.szxytkj.cn

[S31] C++：Hello World
来源：http://ta.jianghongdianzi.cn

#include <iostream>
来源：http://vh.huixinmuqiang.cn

int main() { std::cout << "Hello\n"; }
来源：http://vk.szxytkj.cn

[S32] C++：字符串
来源：http://ew.shxzskj.cn

std::string s = "hi";  s += "!";
来源：http://zu.huixiangedu.cn

[S33] C++：vector 增删
来源：http://yb.szxytkj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jj.9csxet.cn

[S34] C++：遍历 vector
来源：http://ih.panjiajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://ta.huixinmuqiang.cn

[S35] C++：map
来源：http://ds.521024.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rh.nicolike.cn

[S36] C++：unordered_map
来源：http://vl.nszjky.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ht.gzmigu.cn

[S37] C++：set
来源：http://sl.huixinmuqiang.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vu.huixiangedu.cn

[S38] C++：排序
来源：http://fi.huanxung.cn

std::sort(v.begin(), v.end());
来源：http://yv.hnjuh.cn

[S39] C++：自定义比较器排序
来源：http://fr.hnjuh.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vg.jctech888.com.cn

[S40] C++：查找元素
来源：http://gm.wgjwhj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vf.huixinmuqiang.cn

[S41] C++：类与构造函数
来源：http://nv.nicolike.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vq.lnxyls.cn

[S42] C++：继承与虚函数
来源：http://mv.bjjhwx.cn

class B : public Base { public: void f() override {} };
来源：http://bn.hahajie.cn

[S43] C++：智能指针
来源：http://kx.huixiangedu.cn

auto p = std::make_unique<int>(5);
来源：http://ns.shxzskj.cn

[S44] C++：引用传参
来源：http://jp.9csxet.cn

void inc(int &x) { ++x; }
来源：http://bc.wgjwhj.cn

[S45] C++：lambda
来源：http://ig.newstarts.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ke.jianghongdianzi.cn

[S46] C++：函数模板
来源：http://ir.hahajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wt.haigaiapp.cn

[S47] C++：结构化绑定遍历
来源：http://im.panjiajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ai.shxzskj.cn

[S48] C++：逐行读文件
来源：http://lq.wgjwhj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ty.panjiajie.cn

while (std::getline(in, line)) { }
来源：http://hp.jctech888.com.cn

[S49] C++：写文件
来源：http://ul.jianghongdianzi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ql.newstarts.cn

[S50] C++：格式化数字
来源：http://yp.hnjuh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rv.9csxet.cn

[S51] C++：显式类型转换
来源：http://xj.nicolike.cn

static_cast<double>(a) / b
来源：http://nm.haigaiapp.cn

[S52] C++：const 与 noexcept
来源：http://vw.shtwfgs.cn

int size() const noexcept { return n_; }
来源：http://cm.jianghongdianzi.cn

[S53] C++：移动语义
来源：http://tm.nszjky.cn

std::vector<int> w = std::move(v);
来源：http://ye.jctech888.com.cn

[S54] C++：异常处理
来源：http://ca.yuntaijiaju.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ry.newstarts.cn

[S55] C++：结构化绑定
来源：http://wf.huanxung.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://lc.shxzskj.cn

[S56] C++：optional
来源：http://zb.newstarts.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kl.wgjwhj.cn

[S57] C++：编译期常量
来源：http://ds.bjjhwx.cn

constexpr int N = 10;
来源：http://ye.yuntaijiaju.cn

[S58] C++：命名空间
来源：http://pa.nicolike.cn

namespace ns { int f() { return 1; } }
来源：http://gp.asd995.cn

[S59] C++：静态断言
来源：http://km.9csxet.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rw.gzmigu.cn

[S60] C++：遍历并删除元素
来源：http://th.huixiangedu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qz.asd995.cn

================================================================================
来源：http://fz.hnjuh.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://um.nicolike.cn

================================================================================
来源：http://ii.muxihuayi.cn

[T01] Kotlin：Hello World
来源：http://fc.huanxung.cn

println("Hello")
来源：http://qq.nicolike.cn

[T02] Kotlin：变量
来源：http://qq.gzmigu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wc.yuexingan06.cn

[T03] Kotlin：字符串模板
来源：http://ri.nszjky.cn

"值: $b"
来源：http://xc.chemitech.net.cn

[T04] Kotlin：空安全
来源：http://sm.521024.cn

val n: String? = null;  n?.length
来源：http://ji.szsharing.cn

[T05] Kotlin：when 表达式
来源：http://cw.shxzukj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gz.bjjhwx.cn

[T06] Kotlin：集合映射
来源：http://hs.newstarts.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rp.shxzukj.cn

[T07] Kotlin：集合过滤
来源：http://oa.colortex.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pn.bjjhwx.cn

[T08] Kotlin：数据类
来源：http://fk.shxzukj.cn

data class User(val name: String, val age: Int)
来源：http://le.jctech888.com.cn

[T09] Kotlin：扩展函数
来源：http://xg.chemitech.net.cn

fun String.exclaim() = this + "!"
来源：http://ta.jctech888.com.cn

[T10] Kotlin：默认参数
来源：http://ao.9csxet.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pp.521024.cn

[T11] Kotlin：协程
来源：http://ij.wgjwhj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jc.szxytkj.cn

[T12] Kotlin：解构声明
来源：http://ki.asd995.cn

val (a, b) = Pair(1, 2)
来源：http://rm.shxzukj.cn

[T13] Kotlin：只读 Map
来源：http://eg.szxytkj.cn

val m = mapOf("a" to 1)
来源：http://ji.chemitech.net.cn

[T14] Kotlin：循环
来源：http://tl.nszjky.cn

for (i in 1..10) println(i)
来源：http://ju.asd995.cn

[T15] Kotlin：接口
来源：http://qe.yuntaijiaju.cn

interface Shape { fun area(): Double }
来源：http://kz.gzmigu.cn

[T16] Swift：Hello World
来源：http://kn.shtwfgs.cn

print("Hello")
来源：http://jd.huanxung.cn

[T17] Swift：变量与常量
来源：http://xv.nicolike.cn

var a = 1;  let b = 2
来源：http://lz.jctech888.com.cn

[T18] Swift：字符串插值
来源：http://te.nicolike.cn

"值: \(b)"
来源：http://dz.bjjhwx.cn

[T19] Swift：可选绑定
来源：http://ky.bjjhwx.cn

if let n = opt { print(n) }
来源：http://as.newstarts.cn

[T20] Swift：数组操作
来源：http://ro.muxihuayi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://cy.9csxet.cn

[T21] Swift：遍历
来源：http://ya.shxzskj.cn

for x in a { print(x) }
来源：http://hn.nicolike.cn

[T22] Swift：字典
来源：http://qf.wgjwhj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zv.gzmigu.cn

[T23] Swift：函数
来源：http://ri.jianghongdianzi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://go.nszjky.cn

[T24] Swift：闭包
来源：http://yc.yuntaijiaju.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ui.newstarts.cn

[T25] Swift：结构体
来源：http://fr.muxihuayi.cn

struct P { var x: Int }
来源：http://ca.jianghongdianzi.cn

[T26] Swift：类与重写
来源：http://xg.muxihuayi.cn

class A: Base { override func f() {} }
来源：http://et.szxytkj.cn

[T27] Swift：错误处理
来源：http://ez.huixinmuqiang.cn

do { try f() } catch { print(error) }
来源：http://yu.bookmarksfly.cn

[T28] Swift：枚举
来源：http://ok.yuntaijiaju.cn

enum Color { case red, green }
来源：http://ap.colortex.cn

[T29] Swift：guard 提前返回
来源：http://gl.huixinmuqiang.cn

guard let x = opt else { return }
来源：http://gs.wgjwhj.cn

[T30] Swift：协议
来源：http://ii.haigaiapp.cn

protocol Shape { func area() -> Double }
来源：http://ts.chemitech.net.cn

[T31] Lua：Hello World
来源：http://wz.9csxet.cn

print("Hello")
来源：http://ks.jianghongdianzi.cn

[T32] Lua：局部变量
来源：http://gi.muxihuayi.cn

local a = 1
来源：http://yf.shtwfgs.cn

[T33] Lua：表（数组）
来源：http://bk.colortex.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://at.huanxung.cn

[T34] Lua：遍历表
来源：http://dj.bjjhwx.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zb.gzmigu.cn

[T35] Lua：字典表
来源：http://nk.hahajie.cn

local d = { a = 1 };  d.b = 2
来源：http://cg.521024.cn

[T36] Lua：函数
来源：http://gx.haigaiapp.cn

function add(a, b) return a + b end
来源：http://hm.hahajie.cn

[T37] Lua：字符串拼接
来源：http://tc.521024.cn

"a" .. "b"
来源：http://us.haigaiapp.cn

[T38] Lua：条件
来源：http://lv.colortex.cn

if x > 0 then print("正") end
来源：http://de.szsharing.cn

[T39] Lua：模式匹配
来源：http://kg.shtwfgs.cn

string.find(s, "%d+")
来源：http://vs.colortex.cn

[T40] Lua：元表
来源：http://vo.yuntaijiaju.cn

setmetatable({}, { __index = base })
来源：http://ze.haigaiapp.cn

[T41] Perl：Hello World
来源：http://gv.huixiangedu.cn

print "Hello\n";
来源：http://am.shxzskj.cn

[T42] Perl：变量类型
来源：http://ah.asd995.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://id.nszjky.cn

[T43] Perl：字符串插值
来源：http://go.huanxung.cn

"值: $a"
来源：http://gw.huanxung.cn

[T44] Perl：条件
来源：http://xa.nicolike.cn

if ($a > 0) { print "正"; }
来源：http://ih.muxihuayi.cn

[T45] Perl：数组遍历
来源：http://cy.shxzskj.cn

for my $x (@arr) { print $x; }
来源：http://mv.colortex.cn

[T46] Perl：哈希操作
来源：http://xj.huixinmuqiang.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ik.huixinmuqiang.cn

[T47] Perl：正则捕获
来源：http://fg.hahajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ip.hahajie.cn

[T48] Perl：正则替换
来源：http://lu.jianghongdianzi.cn

$s =~ s/old/new/g;
来源：http://rt.haigaiapp.cn

[T49] Perl：函数
来源：http://cj.bookmarksfly.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://at.jctech888.com.cn

[T50] Perl：逐行读文件
来源：http://jp.panjiajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qs.jctech888.com.cn

while (my $line = <$fh>) { print $line; }
来源：http://lr.jianghongdianzi.cn

[T51] Scala：Hello World
来源：http://jm.newstarts.cn

println("Hello")
来源：http://az.nszjky.cn

[T52] Scala：变量
来源：http://uw.nicolike.cn

val a = 1;  var b = 2
来源：http://dg.nicolike.cn

[T53] Scala：字符串插值
来源：http://pe.jctech888.com.cn

s"值: $b"
来源：http://ez.shtwfgs.cn

[T54] Scala：集合映射
来源：http://wh.gzmigu.cn

List(1, 2, 3).map(_ * 2)
来源：http://vt.bookmarksfly.cn

[T55] Scala：集合过滤
来源：http://kv.hahajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://aq.bookmarksfly.cn

[T56] Scala：样例类
来源：http://xc.szsharing.cn

case class User(name: String, age: Int)
来源：http://gy.jianghongdianzi.cn

[T57] Scala：模式匹配
来源：http://ji.muxihuayi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://yk.chemitech.net.cn

[T58] Scala：函数定义
来源：http://uq.bjjhwx.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fi.szxytkj.cn

[T59] Scala：循环
来源：http://vp.muxihuayi.cn

for (i <- 1 to 10) println(i)
来源：http://pk.hnjuh.cn

[T60] Scala：折叠
来源：http://xx.shtwfgs.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://es.szxytkj.cn

================================================================================
来源：http://uo.nszjky.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ou.bjjhwx.cn

================================================================================
来源：http://vh.huixinmuqiang.cn

[U01] Py：创建虚拟环境
来源：http://fe.huanxung.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wt.haigaiapp.cn

[U02] Py：导出 / 安装依赖
来源：http://jz.shxzukj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qr.shxzukj.cn

[U03] Py：加载 .env 配置
来源：http://od.nicolike.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gu.chemitech.net.cn

[U04] Py：变量调试打印
来源：http://hh.hnjuh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nr.lnxyls.cn

[U05] Py：列表去重且保序
来源：http://ca.jianghongdianzi.cn

list(dict.fromkeys(arr))
来源：http://od.colortex.cn

[U06] Py：合并两个字典
来源：http://mi.muxihuayi.cn

{**a, **b}
来源：http://ju.huanxung.cn

[U07] Py：反转字典键值
来源：http://qt.yuexingan06.cn

{v: k for k, v in d.items()}
来源：http://eb.shxzukj.cn

[U08] Py：展平二维列表
来源：http://wd.colortex.cn

[y for x in nested for y in x]
来源：http://xc.jctech888.com.cn

[U09] Py：字典取最大值的键
来源：http://cd.huixiangedu.cn

max(d, key=d.get)
来源：http://fd.chemitech.net.cn

[U10] Py：按值排序字典
来源：http://im.bjjhwx.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vj.shxzskj.cn

[U11] Py：生成器表达式
来源：http://mr.yuexingan06.cn

(x * 2 for x in arr)
来源：http://sc.bookmarksfly.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ui.shxzukj.cn

Counter(arr).most_common(3)
来源：http://zf.chemitech.net.cn

[U13] Py：固定长度队列
来源：http://ug.wgjwhj.cn

deque(maxlen=10)
来源：http://ek.huixiangedu.cn

[U14] Py：分组收集到列表
来源：http://bu.shxzukj.cn

defaultdict(list)
来源：http://ol.huixiangedu.cn

[U15] Py：高精度计时
来源：http://ln.bookmarksfly.cn

t = time.perf_counter()
来源：http://xt.521024.cn

[U16] Py：命令行参数解析
来源：http://yb.asd995.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qo.9csxet.cn

[U17] Py：初始化日志
来源：http://jr.9csxet.cn

logging.basicConfig(level=logging.INFO)
来源：http://dr.jctech888.com.cn

[U18] Py：预编译正则
来源：http://pz.nszjky.cn

pat = re.compile(r"\d+")
来源：http://wq.asd995.cn

[U19] Py：正则替换带回调
来源：http://gf.521024.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qn.newstarts.cn

[U20] Py：缓存函数结果
来源：http://rh.huixinmuqiang.cn

@functools.lru_cache(maxsize=None)
来源：http://my.szsharing.cn

[U21] Py：自定义上下文管理器
来源：http://hj.lnxyls.cn

@contextlib.contextmanager
来源：http://ls.szsharing.cn

[U22] Py：矩阵转置
来源：http://qd.9csxet.cn

list(zip(*m))
来源：http://up.bjjhwx.cn

[U23] Py：分块读取大文件
来源：http://ap.huixiangedu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://px.wgjwhj.cn

[U24] Py：路径操作
来源：http://qg.bjjhwx.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rr.lnxyls.cn

[U25] Py：CSV 按字典读
来源：http://cx.9csxet.cn

csv.DictReader(f)
来源：http://mb.521024.cn

[U26] Py：并发下载
来源：http://rq.bookmarksfly.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://an.szxytkj.cn

[U27] Py：异步 HTTP
来源：http://vf.jctech888.com.cn

aiohttp.ClientSession() 配合 async with
来源：http://ry.shxzskj.cn

[U28] Py：类型别名
来源：http://xu.wgjwhj.cn

UserId = int
来源：http://om.szsharing.cn


<!-- 参考信息 -->