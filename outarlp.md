代发 wailian999

x |= (1 << 3);
来源：http://du.521024.cn

[S17] C：安全拼接字符串
来源：http://sz.wgjwhj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bs.nicolike.cn

[S18] C：命令行参数
来源：http://my.newstarts.cn

int main(int argc, char **argv)
来源：http://dw.newstarts.cn

[S19] C：快速排序
来源：http://up.asd995.cn

qsort(a, n, sizeof(int), cmp);
来源：http://kn.shxzukj.cn

[S20] C：二分查找
来源：http://gn.nicolike.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ue.chemitech.net.cn

[S21] C：字符类别判断
来源：http://qw.szxytkj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ua.wgjwhj.cn

[S22] C：字符串转数字
来源：http://hy.jianghongdianzi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://aa.9csxet.cn

[S23] C：随机数
来源：http://qy.shtwfgs.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://oj.nszjky.cn

[S24] C：获取本地时间
来源：http://vz.bjjhwx.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fh.newstarts.cn

[S25] C：内存拷贝
来源：http://mc.wgjwhj.cn

memcpy(dst, src, n);
来源：http://vn.huanxung.cn

[S26] C：内存清零
来源：http://wx.521024.cn

memset(a, 0, sizeof a);
来源：http://ym.chemitech.net.cn

[S27] C：定义常量
来源：http://yi.nszjky.cn

const double PI = 3.14159;
来源：http://jp.bookmarksfly.cn

[S28] C：静态变量
来源：http://wi.colortex.cn

static int counter = 0;
来源：http://fo.lnxyls.cn

[S29] C：变参函数
来源：http://el.muxihuayi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ux.gzmigu.cn

[S30] C：头文件保护
来源：http://xk.bookmarksfly.cn

#ifndef X_H
来源：http://aa.haigaiapp.cn

#define X_H
来源：http://xc.huanxung.cn

#endif
来源：http://lo.hnjuh.cn

[S31] C++：Hello World
来源：http://cl.yuntaijiaju.cn

#include <iostream>
来源：http://lv.shxzskj.cn

int main() { std::cout << "Hello\n"; }
来源：http://ih.shtwfgs.cn

[S32] C++：字符串
来源：http://nl.panjiajie.cn

std::string s = "hi";  s += "!";
来源：http://oe.bookmarksfly.cn

[S33] C++：vector 增删
来源：http://wc.haigaiapp.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kc.521024.cn

[S34] C++：遍历 vector
来源：http://tv.huixinmuqiang.cn

for (auto &x : v) { std::cout << x; }
来源：http://oi.bjjhwx.cn

[S35] C++：map
来源：http://fp.bjjhwx.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ry.wgjwhj.cn

[S36] C++：unordered_map
来源：http://jj.yuntaijiaju.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mn.panjiajie.cn

[S37] C++：set
来源：http://ch.jianghongdianzi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hi.hahajie.cn

[S38] C++：排序
来源：http://ir.wgjwhj.cn

std::sort(v.begin(), v.end());
来源：http://qb.nszjky.cn

[S39] C++：自定义比较器排序
来源：http://xu.wgjwhj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ir.hnjuh.cn

[S40] C++：查找元素
来源：http://ub.huixinmuqiang.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vf.shxzukj.cn

[S41] C++：类与构造函数
来源：http://hw.bjjhwx.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ah.haigaiapp.cn

[S42] C++：继承与虚函数
来源：http://vy.jctech888.com.cn

class B : public Base { public: void f() override {} };
来源：http://dt.bookmarksfly.cn

[S43] C++：智能指针
来源：http://gh.colortex.cn

auto p = std::make_unique<int>(5);
来源：http://oc.gzmigu.cn

[S44] C++：引用传参
来源：http://ry.yuexingan06.cn

void inc(int &x) { ++x; }
来源：http://gv.shtwfgs.cn

[S45] C++：lambda
来源：http://de.jctech888.com.cn

auto add = [](int a, int b) { return a + b; };
来源：http://cz.bjjhwx.cn

[S46] C++：函数模板
来源：http://vt.hnjuh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nc.haigaiapp.cn

[S47] C++：结构化绑定遍历
来源：http://pe.hnjuh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ds.shxzukj.cn

[S48] C++：逐行读文件
来源：http://ob.shxzskj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jx.shxzskj.cn

while (std::getline(in, line)) { }
来源：http://fb.szxytkj.cn

[S49] C++：写文件
来源：http://rh.521024.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fj.newstarts.cn

[S50] C++：格式化数字
来源：http://jd.hahajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wq.asd995.cn

[S51] C++：显式类型转换
来源：http://ok.lnxyls.cn

static_cast<double>(a) / b
来源：http://lu.colortex.cn

[S52] C++：const 与 noexcept
来源：http://sh.huanxung.cn

int size() const noexcept { return n_; }
来源：http://ke.bookmarksfly.cn

[S53] C++：移动语义
来源：http://gr.huixiangedu.cn

std::vector<int> w = std::move(v);
来源：http://lw.bookmarksfly.cn

[S54] C++：异常处理
来源：http://ru.huixiangedu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://re.hahajie.cn

[S55] C++：结构化绑定
来源：http://sj.szxytkj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ea.asd995.cn

[S56] C++：optional
来源：http://sz.asd995.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wc.wgjwhj.cn

[S57] C++：编译期常量
来源：http://ar.nszjky.cn

constexpr int N = 10;
来源：http://tr.asd995.cn

[S58] C++：命名空间
来源：http://cs.chemitech.net.cn

namespace ns { int f() { return 1; } }
来源：http://pl.hahajie.cn

[S59] C++：静态断言
来源：http://xl.panjiajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qx.newstarts.cn

[S60] C++：遍历并删除元素
来源：http://ew.nicolike.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fw.szsharing.cn

================================================================================
来源：http://zz.newstarts.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jk.szxytkj.cn

================================================================================
来源：http://rq.521024.cn

[T01] Kotlin：Hello World
来源：http://sp.nicolike.cn

println("Hello")
来源：http://aq.szxytkj.cn

[T02] Kotlin：变量
来源：http://de.wgjwhj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sc.jctech888.com.cn

[T03] Kotlin：字符串模板
来源：http://rk.jianghongdianzi.cn

"值: $b"
来源：http://hb.szxytkj.cn

[T04] Kotlin：空安全
来源：http://or.gzmigu.cn

val n: String? = null;  n?.length
来源：http://gi.huixiangedu.cn

[T05] Kotlin：when 表达式
来源：http://du.shxzukj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tx.huanxung.cn

[T06] Kotlin：集合映射
来源：http://dj.hahajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://dp.jctech888.com.cn

[T07] Kotlin：集合过滤
来源：http://zj.jianghongdianzi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://kk.colortex.cn

[T08] Kotlin：数据类
来源：http://we.yuexingan06.cn

data class User(val name: String, val age: Int)
来源：http://af.colortex.cn

[T09] Kotlin：扩展函数
来源：http://wn.hahajie.cn

fun String.exclaim() = this + "!"
来源：http://ke.asd995.cn

[T10] Kotlin：默认参数
来源：http://ap.bjjhwx.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ta.newstarts.cn

[T11] Kotlin：协程
来源：http://ee.asd995.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qa.jctech888.com.cn

[T12] Kotlin：解构声明
来源：http://cl.hnjuh.cn

val (a, b) = Pair(1, 2)
来源：http://rb.szsharing.cn

[T13] Kotlin：只读 Map
来源：http://ff.newstarts.cn

val m = mapOf("a" to 1)
来源：http://rw.shtwfgs.cn

[T14] Kotlin：循环
来源：http://is.shtwfgs.cn

for (i in 1..10) println(i)
来源：http://oj.yuntaijiaju.cn

[T15] Kotlin：接口
来源：http://fp.nszjky.cn

interface Shape { fun area(): Double }
来源：http://pe.hnjuh.cn

[T16] Swift：Hello World
来源：http://gp.hnjuh.cn

print("Hello")
来源：http://sl.nicolike.cn

[T17] Swift：变量与常量
来源：http://nd.hahajie.cn

var a = 1;  let b = 2
来源：http://nb.521024.cn

[T18] Swift：字符串插值
来源：http://hv.huixinmuqiang.cn

"值: \(b)"
来源：http://vk.hnjuh.cn

[T19] Swift：可选绑定
来源：http://dd.muxihuayi.cn

if let n = opt { print(n) }
来源：http://fg.colortex.cn

[T20] Swift：数组操作
来源：http://nt.szxytkj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://uw.bjjhwx.cn

[T21] Swift：遍历
来源：http://kk.bjjhwx.cn

for x in a { print(x) }
来源：http://nd.szxytkj.cn

[T22] Swift：字典
来源：http://ke.yuexingan06.cn

var d = ["a": 1];  d["b"] = 2
来源：http://du.shxzukj.cn

[T23] Swift：函数
来源：http://fk.bjjhwx.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ha.jctech888.com.cn

[T24] Swift：闭包
来源：http://rt.shxzukj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://oa.nszjky.cn

[T25] Swift：结构体
来源：http://si.bookmarksfly.cn

struct P { var x: Int }
来源：http://wz.9csxet.cn

[T26] Swift：类与重写
来源：http://vy.huanxung.cn

class A: Base { override func f() {} }
来源：http://kn.bookmarksfly.cn

[T27] Swift：错误处理
来源：http://ri.yuntaijiaju.cn

do { try f() } catch { print(error) }
来源：http://sx.nicolike.cn

[T28] Swift：枚举
来源：http://mv.chemitech.net.cn

enum Color { case red, green }
来源：http://rq.asd995.cn

[T29] Swift：guard 提前返回
来源：http://bh.jianghongdianzi.cn

guard let x = opt else { return }
来源：http://ik.jianghongdianzi.cn

[T30] Swift：协议
来源：http://ri.shxzskj.cn

protocol Shape { func area() -> Double }
来源：http://mn.wgjwhj.cn

[T31] Lua：Hello World
来源：http://re.yuntaijiaju.cn

print("Hello")
来源：http://kw.gzmigu.cn

[T32] Lua：局部变量
来源：http://nd.muxihuayi.cn

local a = 1
来源：http://pb.panjiajie.cn

[T33] Lua：表（数组）
来源：http://nh.asd995.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xa.colortex.cn

[T34] Lua：遍历表
来源：http://pr.yuntaijiaju.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://yy.muxihuayi.cn

[T35] Lua：字典表
来源：http://wl.chemitech.net.cn

local d = { a = 1 };  d.b = 2
来源：http://dn.huanxung.cn

[T36] Lua：函数
来源：http://mz.hnjuh.cn

function add(a, b) return a + b end
来源：http://xp.shtwfgs.cn

[T37] Lua：字符串拼接
来源：http://ud.shtwfgs.cn

"a" .. "b"
来源：http://hy.huanxung.cn

[T38] Lua：条件
来源：http://nt.yuexingan06.cn

if x > 0 then print("正") end
来源：http://lm.521024.cn

[T39] Lua：模式匹配
来源：http://mu.szxytkj.cn

string.find(s, "%d+")
来源：http://tz.chemitech.net.cn

[T40] Lua：元表
来源：http://uy.shxzukj.cn

setmetatable({}, { __index = base })
来源：http://ac.521024.cn

[T41] Perl：Hello World
来源：http://vv.huixinmuqiang.cn

print "Hello\n";
来源：http://yv.newstarts.cn

[T42] Perl：变量类型
来源：http://yx.muxihuayi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nt.huixiangedu.cn

[T43] Perl：字符串插值
来源：http://td.newstarts.cn

"值: $a"
来源：http://jg.gzmigu.cn

[T44] Perl：条件
来源：http://pv.jctech888.com.cn

if ($a > 0) { print "正"; }
来源：http://fk.bjjhwx.cn

[T45] Perl：数组遍历
来源：http://yb.haigaiapp.cn

for my $x (@arr) { print $x; }
来源：http://oy.muxihuayi.cn

[T46] Perl：哈希操作
来源：http://wp.wgjwhj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lo.jianghongdianzi.cn

[T47] Perl：正则捕获
来源：http://zl.shxzskj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://nq.9csxet.cn

[T48] Perl：正则替换
来源：http://em.wgjwhj.cn

$s =~ s/old/new/g;
来源：http://to.jianghongdianzi.cn

[T49] Perl：函数
来源：http://ni.jctech888.com.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ck.panjiajie.cn

[T50] Perl：逐行读文件
来源：http://ix.chemitech.net.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ta.shtwfgs.cn

while (my $line = <$fh>) { print $line; }
来源：http://we.szsharing.cn

[T51] Scala：Hello World
来源：http://yc.jianghongdianzi.cn

println("Hello")
来源：http://ht.hahajie.cn

[T52] Scala：变量
来源：http://pk.jianghongdianzi.cn

val a = 1;  var b = 2
来源：http://gh.hnjuh.cn

[T53] Scala：字符串插值
来源：http://uy.szsharing.cn

s"值: $b"
来源：http://df.muxihuayi.cn

[T54] Scala：集合映射
来源：http://ze.shxzskj.cn

List(1, 2, 3).map(_ * 2)
来源：http://vr.shxzukj.cn

[T55] Scala：集合过滤
来源：http://uy.chemitech.net.cn

List(1, 2, 3).filter(_ > 1)
来源：http://kq.nszjky.cn

[T56] Scala：样例类
来源：http://zd.nicolike.cn

case class User(name: String, age: Int)
来源：http://xr.newstarts.cn

[T57] Scala：模式匹配
来源：http://dz.szxytkj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://do.yuntaijiaju.cn

[T58] Scala：函数定义
来源：http://kz.shxzukj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ve.newstarts.cn

[T59] Scala：循环
来源：http://ef.szsharing.cn

for (i <- 1 to 10) println(i)
来源：http://fw.gzmigu.cn

[T60] Scala：折叠
来源：http://yx.nicolike.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fz.huixiangedu.cn

================================================================================
来源：http://ag.yuexingan06.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fs.shtwfgs.cn

================================================================================
来源：http://kj.shxzskj.cn

[U01] Py：创建虚拟环境
来源：http://kp.9csxet.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nx.521024.cn

[U02] Py：导出 / 安装依赖
来源：http://lr.9csxet.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mw.hnjuh.cn

[U03] Py：加载 .env 配置
来源：http://bx.shtwfgs.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://io.huanxung.cn

[U04] Py：变量调试打印
来源：http://fu.wgjwhj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://oi.gzmigu.cn

[U05] Py：列表去重且保序
来源：http://ic.huixinmuqiang.cn

list(dict.fromkeys(arr))
来源：http://zn.yuntaijiaju.cn

[U06] Py：合并两个字典
来源：http://zy.bjjhwx.cn

{**a, **b}
来源：http://cu.yuexingan06.cn

[U07] Py：反转字典键值
来源：http://th.bjjhwx.cn

{v: k for k, v in d.items()}
来源：http://gy.shxzukj.cn

[U08] Py：展平二维列表
来源：http://tf.newstarts.cn

[y for x in nested for y in x]
来源：http://by.wgjwhj.cn

[U09] Py：字典取最大值的键
来源：http://hc.gzmigu.cn

max(d, key=d.get)
来源：http://ap.chemitech.net.cn

[U10] Py：按值排序字典
来源：http://bu.newstarts.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bq.haigaiapp.cn

[U11] Py：生成器表达式
来源：http://hw.yuntaijiaju.cn

(x * 2 for x in arr)
来源：http://nx.bjjhwx.cn

[U12] Py：取出现最多的 3 个元素
来源：http://si.huixinmuqiang.cn

Counter(arr).most_common(3)
来源：http://xq.huanxung.cn

[U13] Py：固定长度队列
来源：http://qn.huixiangedu.cn

deque(maxlen=10)
来源：http://ca.521024.cn

[U14] Py：分组收集到列表
来源：http://kd.chemitech.net.cn

defaultdict(list)
来源：http://ru.nszjky.cn

[U15] Py：高精度计时
来源：http://rt.colortex.cn

t = time.perf_counter()
来源：http://tw.521024.cn

[U16] Py：命令行参数解析
来源：http://ue.asd995.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://um.newstarts.cn

[U17] Py：初始化日志
来源：http://le.yuexingan06.cn

logging.basicConfig(level=logging.INFO)
来源：http://ft.huixiangedu.cn

[U18] Py：预编译正则
来源：http://nc.shxzskj.cn

pat = re.compile(r"\d+")
来源：http://dg.nszjky.cn

[U19] Py：正则替换带回调
来源：http://ht.hnjuh.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vn.hnjuh.cn

[U20] Py：缓存函数结果
来源：http://ew.shtwfgs.cn

@functools.lru_cache(maxsize=None)
来源：http://js.huixinmuqiang.cn

[U21] Py：自定义上下文管理器
来源：http://lg.huixiangedu.cn

@contextlib.contextmanager
来源：http://uy.jianghongdianzi.cn

[U22] Py：矩阵转置
来源：http://od.szsharing.cn

list(zip(*m))
来源：http://kf.bookmarksfly.cn

[U23] Py：分块读取大文件
来源：http://gj.wgjwhj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://oy.jianghongdianzi.cn

[U24] Py：路径操作
来源：http://fl.hahajie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://oc.panjiajie.cn

[U25] Py：CSV 按字典读
来源：http://iy.newstarts.cn

csv.DictReader(f)
来源：http://oh.chemitech.net.cn

[U26] Py：并发下载
来源：http://hh.hnjuh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hc.newstarts.cn

[U27] Py：异步 HTTP
来源：http://mz.shtwfgs.cn

aiohttp.ClientSession() 配合 async with
来源：http://rv.hnjuh.cn

[U28] Py：类型别名
来源：http://mz.yuntaijiaju.cn

UserId = int
来源：http://bu.bookmarksfly.cn

[U29] Py：属性校验
来源：http://wa.shxzukj.cn

@property 与 @x.setter 配合
来源：http://ds.lnxyls.cn

[U30] Py：数据类
来源：http://ir.nszjky.cn

@dataclass(slots=True)
来源：http://fi.panjiajie.cn

[U31] Py：单测
来源：http://mk.panjiajie.cn

python -m pytest -q
来源：http://iv.huixiangedu.cn

[U32] Py：代码格式化
来源：http://uf.muxihuayi.cn

ruff format . && ruff check --fix .
来源：http://ax.panjiajie.cn

[U33] Py：打包发布
来源：http://gc.colortex.cn

python -m build  （依赖 pyproject.toml）
来源：http://ba.haigaiapp.cn

[U34] Py：判断编码
来源：http://gt.szxytkj.cn

chardet.detect(raw)
来源：http://vi.szsharing.cn

[U35] Py：发送邮件
来源：http://xq.hahajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yf.bookmarksfly.cn

[U36] Py：定时任务
来源：http://it.haigaiapp.cn

schedule.every(10).minutes.do(job)
来源：http://nh.shxzskj.cn

[U37] Py：读写 Excel
来源：http://he.521024.cn

pandas.read_excel / DataFrame.to_excel
来源：http://xs.9csxet.cn

[U38] Py：获取脚本所在目录
来源：http://ws.huixinmuqiang.cn

Path(__file__).resolve().parent
来源：http://oj.shtwfgs.cn

[U39] Py：判断是否在交互环境
来源：http://od.hahajie.cn

sys.stdout.isatty()
来源：http://gs.wgjwhj.cn

[U40] Py：打印到标准错误
来源：http://dj.shxzskj.cn

print("err", file=sys.stderr)
来源：http://rq.shxzukj.cn


<!-- 参考信息 -->