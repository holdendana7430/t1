代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ll.newstarts.cn

[S10] C：指针与解引用
来源：http://fy.nszjky.cn

int *p = &a;  *p = 5;
来源：http://xw.huanxung.cn

[S11] C：逐行读文件
来源：http://bn.hnjuh.cn

FILE *f = fopen("a.txt", "r");
来源：http://cd.shtwfgs.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nu.hahajie.cn

fclose(f);
来源：http://zd.521024.cn

[S12] C：写文件
来源：http://ff.9csxet.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xd.panjiajie.cn

[S13] C：宏定义
来源：http://kc.asd995.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gq.9csxet.cn

[S14] C：枚举
来源：http://jy.shxzskj.cn

enum Color { RED, GREEN, BLUE };
来源：http://uo.nszjky.cn

[S15] C：类型转换
来源：http://qj.bookmarksfly.cn

(double) a / b
来源：http://ca.nszjky.cn

[S16] C：位操作置位
来源：http://lf.chemitech.net.cn

x |= (1 << 3);
来源：http://nd.muxihuayi.cn

[S17] C：安全拼接字符串
来源：http://nn.yuexingan06.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bg.huixiangedu.cn

[S18] C：命令行参数
来源：http://mg.szsharing.cn

int main(int argc, char **argv)
来源：http://lw.panjiajie.cn

[S19] C：快速排序
来源：http://pd.jctech888.com.cn

qsort(a, n, sizeof(int), cmp);
来源：http://dx.bjjhwx.cn

[S20] C：二分查找
来源：http://xy.yuexingan06.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nf.nszjky.cn

[S21] C：字符类别判断
来源：http://mo.asd995.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ux.jctech888.com.cn

[S22] C：字符串转数字
来源：http://lr.muxihuayi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://it.gzmigu.cn

[S23] C：随机数
来源：http://ox.haigaiapp.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qh.bjjhwx.cn

[S24] C：获取本地时间
来源：http://gx.521024.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ys.szxytkj.cn

[S25] C：内存拷贝
来源：http://jg.jctech888.com.cn

memcpy(dst, src, n);
来源：http://ae.chemitech.net.cn

[S26] C：内存清零
来源：http://zp.shxzukj.cn

memset(a, 0, sizeof a);
来源：http://tt.9csxet.cn

[S27] C：定义常量
来源：http://hi.yuntaijiaju.cn

const double PI = 3.14159;
来源：http://wy.wgjwhj.cn

[S28] C：静态变量
来源：http://ve.shtwfgs.cn

static int counter = 0;
来源：http://bk.nszjky.cn

[S29] C：变参函数
来源：http://qx.521024.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://au.muxihuayi.cn

[S30] C：头文件保护
来源：http://cl.bookmarksfly.cn

#ifndef X_H
来源：http://rl.newstarts.cn

#define X_H
来源：http://kq.szxytkj.cn

#endif
来源：http://ue.shtwfgs.cn

[S31] C++：Hello World
来源：http://nj.shxzukj.cn

#include <iostream>
来源：http://vm.shxzskj.cn

int main() { std::cout << "Hello\n"; }
来源：http://nd.chemitech.net.cn

[S32] C++：字符串
来源：http://wi.9csxet.cn

std::string s = "hi";  s += "!";
来源：http://qy.nicolike.cn

[S33] C++：vector 增删
来源：http://rv.szsharing.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wo.521024.cn

[S34] C++：遍历 vector
来源：http://nv.chemitech.net.cn

for (auto &x : v) { std::cout << x; }
来源：http://kl.gzmigu.cn

[S35] C++：map
来源：http://mq.asd995.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wd.szsharing.cn

[S36] C++：unordered_map
来源：http://mm.jianghongdianzi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bq.newstarts.cn

[S37] C++：set
来源：http://vv.shtwfgs.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kl.jctech888.com.cn

[S38] C++：排序
来源：http://kt.bookmarksfly.cn

std::sort(v.begin(), v.end());
来源：http://ns.jctech888.com.cn

[S39] C++：自定义比较器排序
来源：http://xm.nszjky.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tr.colortex.cn

[S40] C++：查找元素
来源：http://fb.asd995.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://db.9csxet.cn

[S41] C++：类与构造函数
来源：http://ha.newstarts.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wv.newstarts.cn

[S42] C++：继承与虚函数
来源：http://zu.huixiangedu.cn

class B : public Base { public: void f() override {} };
来源：http://ql.newstarts.cn

[S43] C++：智能指针
来源：http://xu.asd995.cn

auto p = std::make_unique<int>(5);
来源：http://ds.bookmarksfly.cn

[S44] C++：引用传参
来源：http://sk.huanxung.cn

void inc(int &x) { ++x; }
来源：http://lg.szxytkj.cn

[S45] C++：lambda
来源：http://ac.hahajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://sp.shxzskj.cn

[S46] C++：函数模板
来源：http://vx.yuexingan06.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nl.huixinmuqiang.cn

[S47] C++：结构化绑定遍历
来源：http://ag.hahajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://df.chemitech.net.cn

[S48] C++：逐行读文件
来源：http://wu.nszjky.cn

std::ifstream in("a.txt");  std::string line;
来源：http://dw.lnxyls.cn

while (std::getline(in, line)) { }
来源：http://ld.asd995.cn

[S49] C++：写文件
来源：http://zh.szxytkj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://km.bjjhwx.cn

[S50] C++：格式化数字
来源：http://ta.shtwfgs.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://id.bjjhwx.cn

[S51] C++：显式类型转换
来源：http://zi.gzmigu.cn

static_cast<double>(a) / b
来源：http://mj.gzmigu.cn

[S52] C++：const 与 noexcept
来源：http://zk.yuntaijiaju.cn

int size() const noexcept { return n_; }
来源：http://se.szxytkj.cn

[S53] C++：移动语义
来源：http://po.szsharing.cn

std::vector<int> w = std::move(v);
来源：http://sa.gzmigu.cn

[S54] C++：异常处理
来源：http://wr.bjjhwx.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dy.colortex.cn

[S55] C++：结构化绑定
来源：http://gp.gzmigu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zx.asd995.cn

[S56] C++：optional
来源：http://wx.newstarts.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jg.bookmarksfly.cn

[S57] C++：编译期常量
来源：http://vc.newstarts.cn

constexpr int N = 10;
来源：http://za.wgjwhj.cn

[S58] C++：命名空间
来源：http://sn.newstarts.cn

namespace ns { int f() { return 1; } }
来源：http://ay.huixiangedu.cn

[S59] C++：静态断言
来源：http://kl.muxihuayi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ei.shtwfgs.cn

[S60] C++：遍历并删除元素
来源：http://nz.jctech888.com.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qp.jianghongdianzi.cn

================================================================================
来源：http://zl.huixinmuqiang.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xz.hahajie.cn

================================================================================
来源：http://wj.bookmarksfly.cn

[T01] Kotlin：Hello World
来源：http://hu.asd995.cn

println("Hello")
来源：http://fe.huixiangedu.cn

[T02] Kotlin：变量
来源：http://jt.panjiajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nj.colortex.cn

[T03] Kotlin：字符串模板
来源：http://hu.asd995.cn

"值: $b"
来源：http://gt.newstarts.cn

[T04] Kotlin：空安全
来源：http://ge.9csxet.cn

val n: String? = null;  n?.length
来源：http://sh.shxzskj.cn

[T05] Kotlin：when 表达式
来源：http://pj.colortex.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://aw.9csxet.cn

[T06] Kotlin：集合映射
来源：http://ag.bjjhwx.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://bk.hahajie.cn

[T07] Kotlin：集合过滤
来源：http://io.jctech888.com.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://zx.9csxet.cn

[T08] Kotlin：数据类
来源：http://qe.shxzukj.cn

data class User(val name: String, val age: Int)
来源：http://tt.szxytkj.cn

[T09] Kotlin：扩展函数
来源：http://af.huixinmuqiang.cn

fun String.exclaim() = this + "!"
来源：http://bj.panjiajie.cn

[T10] Kotlin：默认参数
来源：http://ti.9csxet.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://um.newstarts.cn

[T11] Kotlin：协程
来源：http://jk.wgjwhj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://lv.hnjuh.cn

[T12] Kotlin：解构声明
来源：http://mf.shxzskj.cn

val (a, b) = Pair(1, 2)
来源：http://kx.panjiajie.cn

[T13] Kotlin：只读 Map
来源：http://ks.nszjky.cn

val m = mapOf("a" to 1)
来源：http://fk.huixinmuqiang.cn

[T14] Kotlin：循环
来源：http://vk.colortex.cn

for (i in 1..10) println(i)
来源：http://ey.shxzukj.cn

[T15] Kotlin：接口
来源：http://gn.yuntaijiaju.cn

interface Shape { fun area(): Double }
来源：http://ux.gzmigu.cn

[T16] Swift：Hello World
来源：http://my.newstarts.cn

print("Hello")
来源：http://cy.bjjhwx.cn

[T17] Swift：变量与常量
来源：http://vs.asd995.cn

var a = 1;  let b = 2
来源：http://fc.shxzukj.cn

[T18] Swift：字符串插值
来源：http://sz.bjjhwx.cn

"值: \(b)"
来源：http://bv.szxytkj.cn

[T19] Swift：可选绑定
来源：http://xy.huanxung.cn

if let n = opt { print(n) }
来源：http://xu.9csxet.cn

[T20] Swift：数组操作
来源：http://ig.9csxet.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zn.lnxyls.cn

[T21] Swift：遍历
来源：http://gw.lnxyls.cn

for x in a { print(x) }
来源：http://qb.jianghongdianzi.cn

[T22] Swift：字典
来源：http://er.shxzskj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vj.lnxyls.cn

[T23] Swift：函数
来源：http://jd.asd995.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ig.panjiajie.cn

[T24] Swift：闭包
来源：http://gv.muxihuayi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ye.shxzskj.cn

[T25] Swift：结构体
来源：http://zl.9csxet.cn

struct P { var x: Int }
来源：http://qw.jctech888.com.cn

[T26] Swift：类与重写
来源：http://gs.huixinmuqiang.cn

class A: Base { override func f() {} }
来源：http://bc.muxihuayi.cn

[T27] Swift：错误处理
来源：http://fe.gzmigu.cn

do { try f() } catch { print(error) }
来源：http://yr.newstarts.cn

[T28] Swift：枚举
来源：http://cn.huixiangedu.cn

enum Color { case red, green }
来源：http://vk.521024.cn

[T29] Swift：guard 提前返回
来源：http://rq.bjjhwx.cn

guard let x = opt else { return }
来源：http://uw.bookmarksfly.cn

[T30] Swift：协议
来源：http://zh.bookmarksfly.cn

protocol Shape { func area() -> Double }
来源：http://pw.bjjhwx.cn

[T31] Lua：Hello World
来源：http://ll.bookmarksfly.cn

print("Hello")
来源：http://tu.hnjuh.cn

[T32] Lua：局部变量
来源：http://uw.jctech888.com.cn

local a = 1
来源：http://hu.bookmarksfly.cn

[T33] Lua：表（数组）
来源：http://zw.huanxung.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://mw.jctech888.com.cn

[T34] Lua：遍历表
来源：http://ck.hahajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ca.yuntaijiaju.cn

[T35] Lua：字典表
来源：http://xs.muxihuayi.cn

local d = { a = 1 };  d.b = 2
来源：http://ou.hahajie.cn

[T36] Lua：函数
来源：http://fz.nicolike.cn

function add(a, b) return a + b end
来源：http://fg.521024.cn

[T37] Lua：字符串拼接
来源：http://qq.lnxyls.cn

"a" .. "b"
来源：http://gu.gzmigu.cn

[T38] Lua：条件
来源：http://ti.9csxet.cn

if x > 0 then print("正") end
来源：http://wo.asd995.cn

[T39] Lua：模式匹配
来源：http://ej.shxzukj.cn

string.find(s, "%d+")
来源：http://uh.colortex.cn

[T40] Lua：元表
来源：http://tg.asd995.cn

setmetatable({}, { __index = base })
来源：http://sd.huixinmuqiang.cn

[T41] Perl：Hello World
来源：http://tp.chemitech.net.cn

print "Hello\n";
来源：http://mz.haigaiapp.cn

[T42] Perl：变量类型
来源：http://ob.lnxyls.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fi.hnjuh.cn

[T43] Perl：字符串插值
来源：http://zf.nszjky.cn

"值: $a"
来源：http://jd.nszjky.cn

[T44] Perl：条件
来源：http://bb.jctech888.com.cn

if ($a > 0) { print "正"; }
来源：http://mx.yuexingan06.cn

[T45] Perl：数组遍历
来源：http://lp.gzmigu.cn

for my $x (@arr) { print $x; }
来源：http://yb.gzmigu.cn

[T46] Perl：哈希操作
来源：http://mh.shxzskj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://di.jianghongdianzi.cn

[T47] Perl：正则捕获
来源：http://fv.szxytkj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ut.hahajie.cn

[T48] Perl：正则替换
来源：http://on.huixiangedu.cn

$s =~ s/old/new/g;
来源：http://ll.huixinmuqiang.cn

[T49] Perl：函数
来源：http://nw.asd995.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zy.shxzskj.cn

[T50] Perl：逐行读文件
来源：http://ey.newstarts.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://pg.shxzskj.cn

while (my $line = <$fh>) { print $line; }
来源：http://dn.muxihuayi.cn

[T51] Scala：Hello World
来源：http://tm.colortex.cn

println("Hello")
来源：http://tx.huanxung.cn

[T52] Scala：变量
来源：http://te.huixinmuqiang.cn

val a = 1;  var b = 2
来源：http://la.panjiajie.cn

[T53] Scala：字符串插值
来源：http://dl.panjiajie.cn

s"值: $b"
来源：http://ll.lnxyls.cn

[T54] Scala：集合映射
来源：http://bo.huixinmuqiang.cn

List(1, 2, 3).map(_ * 2)
来源：http://ua.haigaiapp.cn

[T55] Scala：集合过滤
来源：http://wo.huanxung.cn

List(1, 2, 3).filter(_ > 1)
来源：http://jn.newstarts.cn

[T56] Scala：样例类
来源：http://eo.nicolike.cn

case class User(name: String, age: Int)
来源：http://no.muxihuayi.cn

[T57] Scala：模式匹配
来源：http://dd.huixiangedu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ed.bookmarksfly.cn

[T58] Scala：函数定义
来源：http://oh.lnxyls.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zf.nicolike.cn

[T59] Scala：循环
来源：http://pf.yuntaijiaju.cn

for (i <- 1 to 10) println(i)
来源：http://bu.szsharing.cn

[T60] Scala：折叠
来源：http://va.szxytkj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nt.yuntaijiaju.cn

================================================================================
来源：http://my.huixiangedu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vm.huanxung.cn

================================================================================
来源：http://ns.521024.cn

[U01] Py：创建虚拟环境
来源：http://pa.huixinmuqiang.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nh.yuexingan06.cn

[U02] Py：导出 / 安装依赖
来源：http://bq.huanxung.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nh.nicolike.cn

[U03] Py：加载 .env 配置
来源：http://gg.nszjky.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://od.shxzskj.cn

[U04] Py：变量调试打印
来源：http://ks.panjiajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xu.huixinmuqiang.cn

[U05] Py：列表去重且保序
来源：http://tt.newstarts.cn

list(dict.fromkeys(arr))
来源：http://ma.muxihuayi.cn

[U06] Py：合并两个字典
来源：http://zb.bookmarksfly.cn

{**a, **b}
来源：http://rn.panjiajie.cn

[U07] Py：反转字典键值
来源：http://jw.muxihuayi.cn

{v: k for k, v in d.items()}
来源：http://jl.hnjuh.cn

[U08] Py：展平二维列表
来源：http://gc.muxihuayi.cn

[y for x in nested for y in x]
来源：http://bx.muxihuayi.cn

[U09] Py：字典取最大值的键
来源：http://mo.wgjwhj.cn

max(d, key=d.get)
来源：http://cn.bjjhwx.cn

[U10] Py：按值排序字典
来源：http://sg.lnxyls.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ms.nicolike.cn

[U11] Py：生成器表达式
来源：http://cl.colortex.cn

(x * 2 for x in arr)
来源：http://ic.nicolike.cn

[U12] Py：取出现最多的 3 个元素
来源：http://pq.colortex.cn

Counter(arr).most_common(3)
来源：http://xv.9csxet.cn

[U13] Py：固定长度队列
来源：http://go.shxzukj.cn

deque(maxlen=10)
来源：http://ww.panjiajie.cn

[U14] Py：分组收集到列表
来源：http://nr.hnjuh.cn

defaultdict(list)
来源：http://zs.9csxet.cn

[U15] Py：高精度计时
来源：http://aj.huixiangedu.cn

t = time.perf_counter()
来源：http://gz.nszjky.cn

[U16] Py：命令行参数解析
来源：http://rx.jianghongdianzi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pf.jctech888.com.cn

[U17] Py：初始化日志
来源：http://sl.shtwfgs.cn

logging.basicConfig(level=logging.INFO)
来源：http://we.9csxet.cn

[U18] Py：预编译正则
来源：http://dd.521024.cn

pat = re.compile(r"\d+")
来源：http://lx.bookmarksfly.cn

[U19] Py：正则替换带回调
来源：http://hg.huixinmuqiang.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xz.hahajie.cn

[U20] Py：缓存函数结果
来源：http://eu.muxihuayi.cn

@functools.lru_cache(maxsize=None)
来源：http://db.shxzskj.cn

[U21] Py：自定义上下文管理器
来源：http://sz.hahajie.cn

@contextlib.contextmanager
来源：http://mz.gzmigu.cn

[U22] Py：矩阵转置
来源：http://xf.huixiangedu.cn

list(zip(*m))
来源：http://jw.bookmarksfly.cn

[U23] Py：分块读取大文件
来源：http://gt.521024.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vi.colortex.cn

[U24] Py：路径操作
来源：http://ds.colortex.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rg.panjiajie.cn

[U25] Py：CSV 按字典读
来源：http://qj.521024.cn

csv.DictReader(f)
来源：http://kr.521024.cn

[U26] Py：并发下载
来源：http://rj.shtwfgs.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kk.hahajie.cn

[U27] Py：异步 HTTP
来源：http://vf.szsharing.cn

aiohttp.ClientSession() 配合 async with
来源：http://th.shtwfgs.cn

[U28] Py：类型别名
来源：http://ei.szxytkj.cn

UserId = int
来源：http://we.asd995.cn

[U29] Py：属性校验
来源：http://ey.szsharing.cn

@property 与 @x.setter 配合
来源：http://ek.nicolike.cn

[U30] Py：数据类
来源：http://gc.521024.cn

@dataclass(slots=True)
来源：http://gs.bjjhwx.cn

[U31] Py：单测
来源：http://sa.colortex.cn

python -m pytest -q
来源：http://tu.huixinmuqiang.cn

[U32] Py：代码格式化
来源：http://xb.shxzskj.cn

ruff format . && ruff check --fix .
来源：http://fq.szsharing.cn


<!-- 参考信息 -->