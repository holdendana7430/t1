代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dy.shtwfgs.cn

[S08] C：动态内存分配与释放
来源：http://ul.shxzskj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uu.szsharing.cn

[S09] C：结构体定义与初始化
来源：http://jq.9csxet.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bo.lnxyls.cn

[S10] C：指针与解引用
来源：http://wm.muxihuayi.cn

int *p = &a;  *p = 5;
来源：http://we.hnjuh.cn

[S11] C：逐行读文件
来源：http://uw.jctech888.com.cn

FILE *f = fopen("a.txt", "r");
来源：http://rg.asd995.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://no.asd995.cn

fclose(f);
来源：http://qj.asd995.cn

[S12] C：写文件
来源：http://yb.nicolike.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lf.huixinmuqiang.cn

[S13] C：宏定义
来源：http://qd.bookmarksfly.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rf.nszjky.cn

[S14] C：枚举
来源：http://ml.shxzukj.cn

enum Color { RED, GREEN, BLUE };
来源：http://fl.haigaiapp.cn

[S15] C：类型转换
来源：http://nl.asd995.cn

(double) a / b
来源：http://oq.yuexingan06.cn

[S16] C：位操作置位
来源：http://pm.newstarts.cn

x |= (1 << 3);
来源：http://ob.nszjky.cn

[S17] C：安全拼接字符串
来源：http://na.colortex.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://it.huanxung.cn

[S18] C：命令行参数
来源：http://hk.panjiajie.cn

int main(int argc, char **argv)
来源：http://lz.huanxung.cn

[S19] C：快速排序
来源：http://fs.shxzskj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://dz.nszjky.cn

[S20] C：二分查找
来源：http://sg.wgjwhj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ei.huixiangedu.cn

[S21] C：字符类别判断
来源：http://eq.shtwfgs.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sr.jctech888.com.cn

[S22] C：字符串转数字
来源：http://ez.521024.cn

atoi("42");  strtod("3.14", NULL);
来源：http://pv.szxytkj.cn

[S23] C：随机数
来源：http://qr.chemitech.net.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bx.szsharing.cn

[S24] C：获取本地时间
来源：http://sh.haigaiapp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ib.haigaiapp.cn

[S25] C：内存拷贝
来源：http://pf.shxzukj.cn

memcpy(dst, src, n);
来源：http://tn.haigaiapp.cn

[S26] C：内存清零
来源：http://hi.huanxung.cn

memset(a, 0, sizeof a);
来源：http://ts.huixiangedu.cn

[S27] C：定义常量
来源：http://ay.asd995.cn

const double PI = 3.14159;
来源：http://fj.nszjky.cn

[S28] C：静态变量
来源：http://qo.colortex.cn

static int counter = 0;
来源：http://gj.nicolike.cn

[S29] C：变参函数
来源：http://tl.wgjwhj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ie.asd995.cn

[S30] C：头文件保护
来源：http://ne.hnjuh.cn

#ifndef X_H
来源：http://yy.nszjky.cn

#define X_H
来源：http://wn.colortex.cn

#endif
来源：http://gj.huixinmuqiang.cn

[S31] C++：Hello World
来源：http://pg.nszjky.cn

#include <iostream>
来源：http://yu.nicolike.cn

int main() { std::cout << "Hello\n"; }
来源：http://or.9csxet.cn

[S32] C++：字符串
来源：http://oc.szsharing.cn

std::string s = "hi";  s += "!";
来源：http://qn.wgjwhj.cn

[S33] C++：vector 增删
来源：http://dv.hnjuh.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://td.yuexingan06.cn

[S34] C++：遍历 vector
来源：http://aj.asd995.cn

for (auto &x : v) { std::cout << x; }
来源：http://rl.gzmigu.cn

[S35] C++：map
来源：http://jw.hahajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pl.szsharing.cn

[S36] C++：unordered_map
来源：http://wd.bookmarksfly.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uw.asd995.cn

[S37] C++：set
来源：http://dt.huanxung.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mu.asd995.cn

[S38] C++：排序
来源：http://cn.shtwfgs.cn

std::sort(v.begin(), v.end());
来源：http://la.shtwfgs.cn

[S39] C++：自定义比较器排序
来源：http://nw.bjjhwx.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mu.bookmarksfly.cn

[S40] C++：查找元素
来源：http://yc.bjjhwx.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sx.huixinmuqiang.cn

[S41] C++：类与构造函数
来源：http://cr.colortex.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cm.521024.cn

[S42] C++：继承与虚函数
来源：http://dv.nicolike.cn

class B : public Base { public: void f() override {} };
来源：http://jo.huixiangedu.cn

[S43] C++：智能指针
来源：http://sp.lnxyls.cn

auto p = std::make_unique<int>(5);
来源：http://ue.9csxet.cn

[S44] C++：引用传参
来源：http://do.huixinmuqiang.cn

void inc(int &x) { ++x; }
来源：http://ql.lnxyls.cn

[S45] C++：lambda
来源：http://gc.bookmarksfly.cn

auto add = [](int a, int b) { return a + b; };
来源：http://aq.9csxet.cn

[S46] C++：函数模板
来源：http://zi.asd995.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fr.lnxyls.cn

[S47] C++：结构化绑定遍历
来源：http://jf.huixinmuqiang.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ju.shtwfgs.cn

[S48] C++：逐行读文件
来源：http://we.huixiangedu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vy.szsharing.cn

while (std::getline(in, line)) { }
来源：http://mk.nszjky.cn

[S49] C++：写文件
来源：http://rs.panjiajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sk.bookmarksfly.cn

[S50] C++：格式化数字
来源：http://oo.hnjuh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pd.shtwfgs.cn

[S51] C++：显式类型转换
来源：http://fc.gzmigu.cn

static_cast<double>(a) / b
来源：http://lp.gzmigu.cn

[S52] C++：const 与 noexcept
来源：http://tn.gzmigu.cn

int size() const noexcept { return n_; }
来源：http://nk.colortex.cn

[S53] C++：移动语义
来源：http://pj.asd995.cn

std::vector<int> w = std::move(v);
来源：http://cz.szsharing.cn

[S54] C++：异常处理
来源：http://zr.huixinmuqiang.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lp.yuntaijiaju.cn

[S55] C++：结构化绑定
来源：http://aa.nicolike.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ia.huixiangedu.cn

[S56] C++：optional
来源：http://rq.colortex.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gb.9csxet.cn

[S57] C++：编译期常量
来源：http://ld.huixiangedu.cn

constexpr int N = 10;
来源：http://ir.muxihuayi.cn

[S58] C++：命名空间
来源：http://ah.nszjky.cn

namespace ns { int f() { return 1; } }
来源：http://ko.lnxyls.cn

[S59] C++：静态断言
来源：http://zx.hnjuh.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xl.gzmigu.cn

[S60] C++：遍历并删除元素
来源：http://df.9csxet.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://iu.lnxyls.cn

================================================================================
来源：http://md.shxzukj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kw.9csxet.cn

================================================================================
来源：http://pd.muxihuayi.cn

[T01] Kotlin：Hello World
来源：http://rx.hnjuh.cn

println("Hello")
来源：http://ns.chemitech.net.cn

[T02] Kotlin：变量
来源：http://yp.shxzskj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sb.colortex.cn

[T03] Kotlin：字符串模板
来源：http://vv.newstarts.cn

"值: $b"
来源：http://iq.szxytkj.cn

[T04] Kotlin：空安全
来源：http://rv.gzmigu.cn

val n: String? = null;  n?.length
来源：http://em.colortex.cn

[T05] Kotlin：when 表达式
来源：http://sn.muxihuayi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tn.shtwfgs.cn

[T06] Kotlin：集合映射
来源：http://am.asd995.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://vl.jctech888.com.cn

[T07] Kotlin：集合过滤
来源：http://wg.yuntaijiaju.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://rs.haigaiapp.cn

[T08] Kotlin：数据类
来源：http://dm.gzmigu.cn

data class User(val name: String, val age: Int)
来源：http://pw.asd995.cn

[T09] Kotlin：扩展函数
来源：http://rg.huixiangedu.cn

fun String.exclaim() = this + "!"
来源：http://vt.gzmigu.cn

[T10] Kotlin：默认参数
来源：http://ns.panjiajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jp.haigaiapp.cn

[T11] Kotlin：协程
来源：http://xy.shxzukj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nr.chemitech.net.cn

[T12] Kotlin：解构声明
来源：http://jb.nicolike.cn

val (a, b) = Pair(1, 2)
来源：http://nh.bookmarksfly.cn

[T13] Kotlin：只读 Map
来源：http://wk.yuntaijiaju.cn

val m = mapOf("a" to 1)
来源：http://jl.lnxyls.cn

[T14] Kotlin：循环
来源：http://ou.newstarts.cn

for (i in 1..10) println(i)
来源：http://hk.colortex.cn

[T15] Kotlin：接口
来源：http://ib.521024.cn

interface Shape { fun area(): Double }
来源：http://pf.lnxyls.cn

[T16] Swift：Hello World
来源：http://qu.521024.cn

print("Hello")
来源：http://hn.newstarts.cn

[T17] Swift：变量与常量
来源：http://ht.jianghongdianzi.cn

var a = 1;  let b = 2
来源：http://ww.nicolike.cn

[T18] Swift：字符串插值
来源：http://lh.9csxet.cn

"值: \(b)"
来源：http://oq.hahajie.cn

[T19] Swift：可选绑定
来源：http://wq.panjiajie.cn

if let n = opt { print(n) }
来源：http://ig.huanxung.cn

[T20] Swift：数组操作
来源：http://yh.szsharing.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gs.nszjky.cn

[T21] Swift：遍历
来源：http://tn.yuntaijiaju.cn

for x in a { print(x) }
来源：http://zs.9csxet.cn

[T22] Swift：字典
来源：http://vu.gzmigu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://tv.newstarts.cn

[T23] Swift：函数
来源：http://re.colortex.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yq.wgjwhj.cn

[T24] Swift：闭包
来源：http://le.bookmarksfly.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://rs.newstarts.cn

[T25] Swift：结构体
来源：http://am.szsharing.cn

struct P { var x: Int }
来源：http://ij.yuntaijiaju.cn

[T26] Swift：类与重写
来源：http://rp.szsharing.cn

class A: Base { override func f() {} }
来源：http://rn.panjiajie.cn

[T27] Swift：错误处理
来源：http://cz.bjjhwx.cn

do { try f() } catch { print(error) }
来源：http://zy.nszjky.cn

[T28] Swift：枚举
来源：http://sy.yuntaijiaju.cn

enum Color { case red, green }
来源：http://iy.yuexingan06.cn

[T29] Swift：guard 提前返回
来源：http://ru.huixiangedu.cn

guard let x = opt else { return }
来源：http://cp.chemitech.net.cn

[T30] Swift：协议
来源：http://gg.newstarts.cn

protocol Shape { func area() -> Double }
来源：http://qz.lnxyls.cn

[T31] Lua：Hello World
来源：http://zd.shtwfgs.cn

print("Hello")
来源：http://qg.haigaiapp.cn

[T32] Lua：局部变量
来源：http://ab.szxytkj.cn

local a = 1
来源：http://qc.huanxung.cn

[T33] Lua：表（数组）
来源：http://dv.colortex.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://od.nszjky.cn

[T34] Lua：遍历表
来源：http://ii.colortex.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ea.panjiajie.cn

[T35] Lua：字典表
来源：http://gd.nszjky.cn

local d = { a = 1 };  d.b = 2
来源：http://ib.jctech888.com.cn

[T36] Lua：函数
来源：http://nm.9csxet.cn

function add(a, b) return a + b end
来源：http://hf.newstarts.cn

[T37] Lua：字符串拼接
来源：http://lo.jctech888.com.cn

"a" .. "b"
来源：http://fh.hahajie.cn

[T38] Lua：条件
来源：http://ah.9csxet.cn

if x > 0 then print("正") end
来源：http://mi.huixinmuqiang.cn

[T39] Lua：模式匹配
来源：http://sp.bjjhwx.cn

string.find(s, "%d+")
来源：http://ln.huanxung.cn

[T40] Lua：元表
来源：http://fy.szsharing.cn

setmetatable({}, { __index = base })
来源：http://yg.9csxet.cn

[T41] Perl：Hello World
来源：http://wi.521024.cn

print "Hello\n";
来源：http://vs.huixiangedu.cn

[T42] Perl：变量类型
来源：http://uk.shxzskj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dd.muxihuayi.cn

[T43] Perl：字符串插值
来源：http://mh.panjiajie.cn

"值: $a"
来源：http://bi.chemitech.net.cn

[T44] Perl：条件
来源：http://cf.muxihuayi.cn

if ($a > 0) { print "正"; }
来源：http://le.szsharing.cn

[T45] Perl：数组遍历
来源：http://nq.hahajie.cn

for my $x (@arr) { print $x; }
来源：http://dv.bjjhwx.cn

[T46] Perl：哈希操作
来源：http://ue.newstarts.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fm.yuntaijiaju.cn

[T47] Perl：正则捕获
来源：http://dm.huixinmuqiang.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://kj.jctech888.com.cn

[T48] Perl：正则替换
来源：http://yb.shtwfgs.cn

$s =~ s/old/new/g;
来源：http://ab.szxytkj.cn

[T49] Perl：函数
来源：http://xe.gzmigu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kc.jctech888.com.cn

[T50] Perl：逐行读文件
来源：http://pu.jctech888.com.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fu.521024.cn

while (my $line = <$fh>) { print $line; }
来源：http://ov.shxzskj.cn

[T51] Scala：Hello World
来源：http://zv.gzmigu.cn

println("Hello")
来源：http://vf.szsharing.cn

[T52] Scala：变量
来源：http://lb.huanxung.cn

val a = 1;  var b = 2
来源：http://wf.newstarts.cn

[T53] Scala：字符串插值
来源：http://bp.hahajie.cn

s"值: $b"
来源：http://xq.gzmigu.cn

[T54] Scala：集合映射
来源：http://qn.shtwfgs.cn

List(1, 2, 3).map(_ * 2)
来源：http://pb.wgjwhj.cn

[T55] Scala：集合过滤
来源：http://al.chemitech.net.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fy.lnxyls.cn

[T56] Scala：样例类
来源：http://vw.wgjwhj.cn

case class User(name: String, age: Int)
来源：http://sh.huixiangedu.cn

[T57] Scala：模式匹配
来源：http://lv.shxzukj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ti.asd995.cn

[T58] Scala：函数定义
来源：http://aa.nicolike.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ly.wgjwhj.cn

[T59] Scala：循环
来源：http://zf.wgjwhj.cn

for (i <- 1 to 10) println(i)
来源：http://op.yuntaijiaju.cn

[T60] Scala：折叠
来源：http://za.yuexingan06.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hj.9csxet.cn

================================================================================
来源：http://kl.jianghongdianzi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://de.newstarts.cn

================================================================================
来源：http://ml.shxzskj.cn

[U01] Py：创建虚拟环境
来源：http://uk.muxihuayi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nl.chemitech.net.cn

[U02] Py：导出 / 安装依赖
来源：http://tf.jianghongdianzi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ht.newstarts.cn

[U03] Py：加载 .env 配置
来源：http://lt.newstarts.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://uy.shtwfgs.cn

[U04] Py：变量调试打印
来源：http://ra.9csxet.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://od.bjjhwx.cn

[U05] Py：列表去重且保序
来源：http://yk.wgjwhj.cn

list(dict.fromkeys(arr))
来源：http://tq.huanxung.cn

[U06] Py：合并两个字典
来源：http://kt.szxytkj.cn

{**a, **b}
来源：http://ff.huixinmuqiang.cn

[U07] Py：反转字典键值
来源：http://xb.jianghongdianzi.cn

{v: k for k, v in d.items()}
来源：http://fj.szsharing.cn

[U08] Py：展平二维列表
来源：http://ds.9csxet.cn

[y for x in nested for y in x]
来源：http://wy.shtwfgs.cn

[U09] Py：字典取最大值的键
来源：http://qh.lnxyls.cn

max(d, key=d.get)
来源：http://zz.9csxet.cn

[U10] Py：按值排序字典
来源：http://bk.szsharing.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pn.jianghongdianzi.cn

[U11] Py：生成器表达式
来源：http://ro.shxzskj.cn

(x * 2 for x in arr)
来源：http://aa.hnjuh.cn

[U12] Py：取出现最多的 3 个元素
来源：http://op.asd995.cn

Counter(arr).most_common(3)
来源：http://oj.haigaiapp.cn

[U13] Py：固定长度队列
来源：http://kt.bookmarksfly.cn

deque(maxlen=10)
来源：http://tz.nicolike.cn

[U14] Py：分组收集到列表
来源：http://sr.yuntaijiaju.cn

defaultdict(list)
来源：http://ug.huixinmuqiang.cn

[U15] Py：高精度计时
来源：http://pq.521024.cn

t = time.perf_counter()
来源：http://pf.szsharing.cn

[U16] Py：命令行参数解析
来源：http://zr.huixinmuqiang.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nq.bookmarksfly.cn

[U17] Py：初始化日志
来源：http://xn.colortex.cn

logging.basicConfig(level=logging.INFO)
来源：http://ru.haigaiapp.cn

[U18] Py：预编译正则
来源：http://lq.huixinmuqiang.cn

pat = re.compile(r"\d+")
来源：http://zh.huanxung.cn

[U19] Py：正则替换带回调
来源：http://hq.panjiajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qc.nicolike.cn

[U20] Py：缓存函数结果
来源：http://zn.nszjky.cn

@functools.lru_cache(maxsize=None)
来源：http://te.shtwfgs.cn

[U21] Py：自定义上下文管理器
来源：http://xy.huixinmuqiang.cn

@contextlib.contextmanager
来源：http://ak.jianghongdianzi.cn

[U22] Py：矩阵转置
来源：http://kb.wgjwhj.cn

list(zip(*m))
来源：http://vp.bookmarksfly.cn

[U23] Py：分块读取大文件
来源：http://dg.huixinmuqiang.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fv.huanxung.cn

[U24] Py：路径操作
来源：http://mq.521024.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kw.nszjky.cn

[U25] Py：CSV 按字典读
来源：http://td.colortex.cn

csv.DictReader(f)
来源：http://sq.shtwfgs.cn

[U26] Py：并发下载
来源：http://hl.panjiajie.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://aw.jctech888.com.cn

[U27] Py：异步 HTTP
来源：http://hj.szxytkj.cn

aiohttp.ClientSession() 配合 async with
来源：http://jo.shxzukj.cn

[U28] Py：类型别名
来源：http://of.muxihuayi.cn

UserId = int
来源：http://yy.newstarts.cn

[U29] Py：属性校验
来源：http://xo.szxytkj.cn

@property 与 @x.setter 配合
来源：http://ff.bookmarksfly.cn

[U30] Py：数据类
来源：http://xj.bookmarksfly.cn

@dataclass(slots=True)
来源：http://ir.shxzskj.cn


<!-- 参考信息 -->