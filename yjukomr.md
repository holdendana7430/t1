代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wn.newstarts.cn

[S10] C：指针与解引用
来源：http://db.yuntaijiaju.cn

int *p = &a;  *p = 5;
来源：http://on.huixiangedu.cn

[S11] C：逐行读文件
来源：http://no.szxytkj.cn

FILE *f = fopen("a.txt", "r");
来源：http://gi.haigaiapp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mg.bjjhwx.cn

fclose(f);
来源：http://pj.huanxung.cn

[S12] C：写文件
来源：http://rp.muxihuayi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mi.gzmigu.cn

[S13] C：宏定义
来源：http://sw.gzmigu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jo.wgjwhj.cn

[S14] C：枚举
来源：http://uh.gzmigu.cn

enum Color { RED, GREEN, BLUE };
来源：http://cc.bjjhwx.cn

[S15] C：类型转换
来源：http://zk.huixinmuqiang.cn

(double) a / b
来源：http://gt.jianghongdianzi.cn

[S16] C：位操作置位
来源：http://py.huixiangedu.cn

x |= (1 << 3);
来源：http://eb.muxihuayi.cn

[S17] C：安全拼接字符串
来源：http://wx.hnjuh.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cb.bookmarksfly.cn

[S18] C：命令行参数
来源：http://as.shxzukj.cn

int main(int argc, char **argv)
来源：http://co.huixinmuqiang.cn

[S19] C：快速排序
来源：http://rd.yuexingan06.cn

qsort(a, n, sizeof(int), cmp);
来源：http://at.bjjhwx.cn

[S20] C：二分查找
来源：http://hy.yuexingan06.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ky.huixiangedu.cn

[S21] C：字符类别判断
来源：http://ud.panjiajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cu.wgjwhj.cn

[S22] C：字符串转数字
来源：http://qz.shxzskj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://mx.jctech888.com.cn

[S23] C：随机数
来源：http://xv.panjiajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://yx.gzmigu.cn

[S24] C：获取本地时间
来源：http://jx.bjjhwx.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fk.shtwfgs.cn

[S25] C：内存拷贝
来源：http://xm.newstarts.cn

memcpy(dst, src, n);
来源：http://cf.szxytkj.cn

[S26] C：内存清零
来源：http://va.panjiajie.cn

memset(a, 0, sizeof a);
来源：http://jr.jctech888.com.cn

[S27] C：定义常量
来源：http://ep.9csxet.cn

const double PI = 3.14159;
来源：http://eb.shxzukj.cn

[S28] C：静态变量
来源：http://lp.newstarts.cn

static int counter = 0;
来源：http://cr.hnjuh.cn

[S29] C：变参函数
来源：http://bb.hahajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rq.521024.cn

[S30] C：头文件保护
来源：http://uh.nszjky.cn

#ifndef X_H
来源：http://gi.jctech888.com.cn

#define X_H
来源：http://ws.yuntaijiaju.cn

#endif
来源：http://kx.wgjwhj.cn

[S31] C++：Hello World
来源：http://zc.haigaiapp.cn

#include <iostream>
来源：http://be.yuntaijiaju.cn

int main() { std::cout << "Hello\n"; }
来源：http://yj.colortex.cn

[S32] C++：字符串
来源：http://cy.nicolike.cn

std::string s = "hi";  s += "!";
来源：http://ah.9csxet.cn

[S33] C++：vector 增删
来源：http://vv.lnxyls.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vb.yuexingan06.cn

[S34] C++：遍历 vector
来源：http://ej.panjiajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://hf.shxzskj.cn

[S35] C++：map
来源：http://gd.shxzskj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ju.shtwfgs.cn

[S36] C++：unordered_map
来源：http://hg.colortex.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sk.bjjhwx.cn

[S37] C++：set
来源：http://ag.bjjhwx.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qu.huixinmuqiang.cn

[S38] C++：排序
来源：http://sb.jctech888.com.cn

std::sort(v.begin(), v.end());
来源：http://bn.nicolike.cn

[S39] C++：自定义比较器排序
来源：http://ku.hnjuh.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://an.szsharing.cn

[S40] C++：查找元素
来源：http://gc.hnjuh.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xf.szxytkj.cn

[S41] C++：类与构造函数
来源：http://jy.jianghongdianzi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sa.nszjky.cn

[S42] C++：继承与虚函数
来源：http://md.szxytkj.cn

class B : public Base { public: void f() override {} };
来源：http://an.bjjhwx.cn

[S43] C++：智能指针
来源：http://wk.521024.cn

auto p = std::make_unique<int>(5);
来源：http://wh.bookmarksfly.cn

[S44] C++：引用传参
来源：http://qo.jctech888.com.cn

void inc(int &x) { ++x; }
来源：http://oz.bookmarksfly.cn

[S45] C++：lambda
来源：http://jw.newstarts.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zw.jianghongdianzi.cn

[S46] C++：函数模板
来源：http://bv.521024.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://va.shxzukj.cn

[S47] C++：结构化绑定遍历
来源：http://pr.hnjuh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cn.yuntaijiaju.cn

[S48] C++：逐行读文件
来源：http://ss.shtwfgs.cn

std::ifstream in("a.txt");  std::string line;
来源：http://yo.huanxung.cn

while (std::getline(in, line)) { }
来源：http://rc.panjiajie.cn

[S49] C++：写文件
来源：http://lt.asd995.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lb.szxytkj.cn

[S50] C++：格式化数字
来源：http://sl.colortex.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bo.nszjky.cn

[S51] C++：显式类型转换
来源：http://fb.haigaiapp.cn

static_cast<double>(a) / b
来源：http://je.newstarts.cn

[S52] C++：const 与 noexcept
来源：http://mz.newstarts.cn

int size() const noexcept { return n_; }
来源：http://vl.hahajie.cn

[S53] C++：移动语义
来源：http://mv.521024.cn

std::vector<int> w = std::move(v);
来源：http://ls.shtwfgs.cn

[S54] C++：异常处理
来源：http://fw.panjiajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mw.gzmigu.cn

[S55] C++：结构化绑定
来源：http://yv.jianghongdianzi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://sg.lnxyls.cn

[S56] C++：optional
来源：http://xf.muxihuayi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tm.shxzskj.cn

[S57] C++：编译期常量
来源：http://ge.panjiajie.cn

constexpr int N = 10;
来源：http://mx.hahajie.cn

[S58] C++：命名空间
来源：http://uo.huixinmuqiang.cn

namespace ns { int f() { return 1; } }
来源：http://ys.521024.cn

[S59] C++：静态断言
来源：http://si.huixinmuqiang.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bu.huixinmuqiang.cn

[S60] C++：遍历并删除元素
来源：http://ak.jctech888.com.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qo.huixinmuqiang.cn

================================================================================
来源：http://tp.yuntaijiaju.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bt.bjjhwx.cn

================================================================================
来源：http://jh.nicolike.cn

[T01] Kotlin：Hello World
来源：http://zn.panjiajie.cn

println("Hello")
来源：http://sj.jianghongdianzi.cn

[T02] Kotlin：变量
来源：http://jd.nszjky.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://re.bjjhwx.cn

[T03] Kotlin：字符串模板
来源：http://hy.wgjwhj.cn

"值: $b"
来源：http://ih.shxzskj.cn

[T04] Kotlin：空安全
来源：http://tn.521024.cn

val n: String? = null;  n?.length
来源：http://gn.yuexingan06.cn

[T05] Kotlin：when 表达式
来源：http://ap.gzmigu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ki.shxzskj.cn

[T06] Kotlin：集合映射
来源：http://fm.muxihuayi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://lk.huanxung.cn

[T07] Kotlin：集合过滤
来源：http://vc.gzmigu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ph.jianghongdianzi.cn

[T08] Kotlin：数据类
来源：http://hw.haigaiapp.cn

data class User(val name: String, val age: Int)
来源：http://ud.chemitech.net.cn

[T09] Kotlin：扩展函数
来源：http://vx.jianghongdianzi.cn

fun String.exclaim() = this + "!"
来源：http://gb.hahajie.cn

[T10] Kotlin：默认参数
来源：http://xi.jctech888.com.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://nf.colortex.cn

[T11] Kotlin：协程
来源：http://pp.panjiajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ey.gzmigu.cn

[T12] Kotlin：解构声明
来源：http://up.szsharing.cn

val (a, b) = Pair(1, 2)
来源：http://oi.haigaiapp.cn

[T13] Kotlin：只读 Map
来源：http://bv.nszjky.cn

val m = mapOf("a" to 1)
来源：http://ve.yuexingan06.cn

[T14] Kotlin：循环
来源：http://lb.szsharing.cn

for (i in 1..10) println(i)
来源：http://bs.hahajie.cn

[T15] Kotlin：接口
来源：http://bx.haigaiapp.cn

interface Shape { fun area(): Double }
来源：http://hz.shxzskj.cn

[T16] Swift：Hello World
来源：http://jo.chemitech.net.cn

print("Hello")
来源：http://kn.bjjhwx.cn

[T17] Swift：变量与常量
来源：http://bw.nszjky.cn

var a = 1;  let b = 2
来源：http://zi.hnjuh.cn

[T18] Swift：字符串插值
来源：http://id.muxihuayi.cn

"值: \(b)"
来源：http://oy.huanxung.cn

[T19] Swift：可选绑定
来源：http://kj.nicolike.cn

if let n = opt { print(n) }
来源：http://ov.shtwfgs.cn

[T20] Swift：数组操作
来源：http://we.huanxung.cn

var a = [1, 2, 3];  a.append(4)
来源：http://dt.lnxyls.cn

[T21] Swift：遍历
来源：http://sb.yuntaijiaju.cn

for x in a { print(x) }
来源：http://sa.shxzskj.cn

[T22] Swift：字典
来源：http://uh.bookmarksfly.cn

var d = ["a": 1];  d["b"] = 2
来源：http://go.yuntaijiaju.cn

[T23] Swift：函数
来源：http://pj.gzmigu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ji.szxytkj.cn

[T24] Swift：闭包
来源：http://av.muxihuayi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://sj.colortex.cn

[T25] Swift：结构体
来源：http://as.colortex.cn

struct P { var x: Int }
来源：http://fl.huixinmuqiang.cn

[T26] Swift：类与重写
来源：http://lp.jctech888.com.cn

class A: Base { override func f() {} }
来源：http://bi.chemitech.net.cn

[T27] Swift：错误处理
来源：http://rd.chemitech.net.cn

do { try f() } catch { print(error) }
来源：http://kx.shxzskj.cn

[T28] Swift：枚举
来源：http://ua.bookmarksfly.cn

enum Color { case red, green }
来源：http://br.shxzskj.cn

[T29] Swift：guard 提前返回
来源：http://kr.haigaiapp.cn

guard let x = opt else { return }
来源：http://kc.newstarts.cn

[T30] Swift：协议
来源：http://kg.huixiangedu.cn

protocol Shape { func area() -> Double }
来源：http://bw.chemitech.net.cn

[T31] Lua：Hello World
来源：http://bs.jctech888.com.cn

print("Hello")
来源：http://rp.huanxung.cn

[T32] Lua：局部变量
来源：http://ib.haigaiapp.cn

local a = 1
来源：http://ea.shtwfgs.cn

[T33] Lua：表（数组）
来源：http://wd.muxihuayi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ax.9csxet.cn

[T34] Lua：遍历表
来源：http://up.szxytkj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://dr.newstarts.cn

[T35] Lua：字典表
来源：http://in.bookmarksfly.cn

local d = { a = 1 };  d.b = 2
来源：http://vb.shxzukj.cn

[T36] Lua：函数
来源：http://wr.hahajie.cn

function add(a, b) return a + b end
来源：http://zq.nicolike.cn

[T37] Lua：字符串拼接
来源：http://ql.bookmarksfly.cn

"a" .. "b"
来源：http://oi.chemitech.net.cn

[T38] Lua：条件
来源：http://jk.panjiajie.cn

if x > 0 then print("正") end
来源：http://ji.huixiangedu.cn

[T39] Lua：模式匹配
来源：http://hr.chemitech.net.cn

string.find(s, "%d+")
来源：http://rw.szsharing.cn

[T40] Lua：元表
来源：http://lg.521024.cn

setmetatable({}, { __index = base })
来源：http://aj.shtwfgs.cn

[T41] Perl：Hello World
来源：http://vc.szsharing.cn

print "Hello\n";
来源：http://nt.521024.cn

[T42] Perl：变量类型
来源：http://ih.newstarts.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sp.shxzukj.cn

[T43] Perl：字符串插值
来源：http://ss.bookmarksfly.cn

"值: $a"
来源：http://yz.szsharing.cn

[T44] Perl：条件
来源：http://fq.bookmarksfly.cn

if ($a > 0) { print "正"; }
来源：http://wd.gzmigu.cn

[T45] Perl：数组遍历
来源：http://hp.huixinmuqiang.cn

for my $x (@arr) { print $x; }
来源：http://ji.bjjhwx.cn

[T46] Perl：哈希操作
来源：http://cf.muxihuayi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fg.colortex.cn

[T47] Perl：正则捕获
来源：http://lt.haigaiapp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ji.huanxung.cn

[T48] Perl：正则替换
来源：http://gp.muxihuayi.cn

$s =~ s/old/new/g;
来源：http://km.hnjuh.cn

[T49] Perl：函数
来源：http://md.huixinmuqiang.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wy.wgjwhj.cn

[T50] Perl：逐行读文件
来源：http://mq.nszjky.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://sa.hnjuh.cn

while (my $line = <$fh>) { print $line; }
来源：http://kn.521024.cn

[T51] Scala：Hello World
来源：http://qy.gzmigu.cn

println("Hello")
来源：http://ea.colortex.cn

[T52] Scala：变量
来源：http://jl.szsharing.cn

val a = 1;  var b = 2
来源：http://pp.521024.cn

[T53] Scala：字符串插值
来源：http://lx.huanxung.cn

s"值: $b"
来源：http://pc.jctech888.com.cn

[T54] Scala：集合映射
来源：http://in.colortex.cn

List(1, 2, 3).map(_ * 2)
来源：http://pi.521024.cn

[T55] Scala：集合过滤
来源：http://rx.muxihuayi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ys.yuexingan06.cn

[T56] Scala：样例类
来源：http://te.bjjhwx.cn

case class User(name: String, age: Int)
来源：http://al.yuntaijiaju.cn

[T57] Scala：模式匹配
来源：http://yy.asd995.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://cw.colortex.cn

[T58] Scala：函数定义
来源：http://oz.9csxet.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ep.asd995.cn

[T59] Scala：循环
来源：http://go.yuexingan06.cn

for (i <- 1 to 10) println(i)
来源：http://sg.huanxung.cn

[T60] Scala：折叠
来源：http://cj.muxihuayi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yd.hahajie.cn

================================================================================
来源：http://iu.9csxet.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ai.jianghongdianzi.cn

================================================================================
来源：http://gm.nicolike.cn

[U01] Py：创建虚拟环境
来源：http://gb.yuntaijiaju.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ca.huanxung.cn

[U02] Py：导出 / 安装依赖
来源：http://lw.panjiajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lw.shxzskj.cn

[U03] Py：加载 .env 配置
来源：http://qr.hahajie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fj.wgjwhj.cn

[U04] Py：变量调试打印
来源：http://ub.yuntaijiaju.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ki.gzmigu.cn

[U05] Py：列表去重且保序
来源：http://yj.521024.cn

list(dict.fromkeys(arr))
来源：http://yi.bookmarksfly.cn

[U06] Py：合并两个字典
来源：http://zy.huixinmuqiang.cn

{**a, **b}
来源：http://jp.huanxung.cn

[U07] Py：反转字典键值
来源：http://cf.szsharing.cn

{v: k for k, v in d.items()}
来源：http://ho.jianghongdianzi.cn

[U08] Py：展平二维列表
来源：http://sq.shxzskj.cn

[y for x in nested for y in x]
来源：http://yb.muxihuayi.cn

[U09] Py：字典取最大值的键
来源：http://xd.hahajie.cn

max(d, key=d.get)
来源：http://zw.huixinmuqiang.cn

[U10] Py：按值排序字典
来源：http://fm.hahajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ch.huanxung.cn

[U11] Py：生成器表达式
来源：http://we.newstarts.cn

(x * 2 for x in arr)
来源：http://sw.lnxyls.cn

[U12] Py：取出现最多的 3 个元素
来源：http://hj.nszjky.cn

Counter(arr).most_common(3)
来源：http://db.hnjuh.cn

[U13] Py：固定长度队列
来源：http://as.hnjuh.cn

deque(maxlen=10)
来源：http://ek.bookmarksfly.cn

[U14] Py：分组收集到列表
来源：http://wa.wgjwhj.cn

defaultdict(list)
来源：http://vb.jianghongdianzi.cn

[U15] Py：高精度计时
来源：http://td.bjjhwx.cn

t = time.perf_counter()
来源：http://gc.shxzskj.cn

[U16] Py：命令行参数解析
来源：http://sf.huixinmuqiang.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xf.panjiajie.cn

[U17] Py：初始化日志
来源：http://no.colortex.cn

logging.basicConfig(level=logging.INFO)
来源：http://kz.chemitech.net.cn

[U18] Py：预编译正则
来源：http://qf.colortex.cn

pat = re.compile(r"\d+")
来源：http://zm.jianghongdianzi.cn

[U19] Py：正则替换带回调
来源：http://ny.newstarts.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rh.asd995.cn

[U20] Py：缓存函数结果
来源：http://wf.szxytkj.cn

@functools.lru_cache(maxsize=None)
来源：http://bs.yuntaijiaju.cn

[U21] Py：自定义上下文管理器
来源：http://sw.gzmigu.cn

@contextlib.contextmanager
来源：http://vo.haigaiapp.cn

[U22] Py：矩阵转置
来源：http://td.shtwfgs.cn

list(zip(*m))
来源：http://kx.chemitech.net.cn

[U23] Py：分块读取大文件
来源：http://vo.newstarts.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xa.chemitech.net.cn

[U24] Py：路径操作
来源：http://sq.chemitech.net.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bk.shxzskj.cn

[U25] Py：CSV 按字典读
来源：http://ql.nicolike.cn

csv.DictReader(f)
来源：http://pp.hnjuh.cn

[U26] Py：并发下载
来源：http://pe.nszjky.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rt.hnjuh.cn

[U27] Py：异步 HTTP
来源：http://mk.newstarts.cn

aiohttp.ClientSession() 配合 async with
来源：http://or.jianghongdianzi.cn

[U28] Py：类型别名
来源：http://wn.muxihuayi.cn

UserId = int
来源：http://ya.asd995.cn

[U29] Py：属性校验
来源：http://vc.hahajie.cn

@property 与 @x.setter 配合
来源：http://fs.newstarts.cn

[U30] Py：数据类
来源：http://ca.hnjuh.cn

@dataclass(slots=True)
来源：http://ny.9csxet.cn

[U31] Py：单测
来源：http://ur.huanxung.cn

python -m pytest -q
来源：http://jv.shtwfgs.cn

[U32] Py：代码格式化
来源：http://xe.yuexingan06.cn

ruff format . && ruff check --fix .
来源：http://xe.muxihuayi.cn


<!-- 参考信息 -->