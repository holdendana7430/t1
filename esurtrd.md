代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://hj.hnjuh.cn

[S15] C：类型转换
来源：http://bs.jctech888.com.cn

(double) a / b
来源：http://kt.huanxung.cn

[S16] C：位操作置位
来源：http://xp.szxytkj.cn

x |= (1 << 3);
来源：http://ok.huixiangedu.cn

[S17] C：安全拼接字符串
来源：http://ff.haigaiapp.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qp.newstarts.cn

[S18] C：命令行参数
来源：http://pa.shxzskj.cn

int main(int argc, char **argv)
来源：http://nx.huixinmuqiang.cn

[S19] C：快速排序
来源：http://hu.szxytkj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xw.lnxyls.cn

[S20] C：二分查找
来源：http://sp.chemitech.net.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ni.jctech888.com.cn

[S21] C：字符类别判断
来源：http://xg.huixiangedu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ua.huixiangedu.cn

[S22] C：字符串转数字
来源：http://gs.asd995.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wy.wgjwhj.cn

[S23] C：随机数
来源：http://ig.nszjky.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://yh.shxzukj.cn

[S24] C：获取本地时间
来源：http://gs.gzmigu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mt.521024.cn

[S25] C：内存拷贝
来源：http://dq.chemitech.net.cn

memcpy(dst, src, n);
来源：http://en.newstarts.cn

[S26] C：内存清零
来源：http://yx.colortex.cn

memset(a, 0, sizeof a);
来源：http://jf.521024.cn

[S27] C：定义常量
来源：http://eb.huixinmuqiang.cn

const double PI = 3.14159;
来源：http://km.nicolike.cn

[S28] C：静态变量
来源：http://yq.gzmigu.cn

static int counter = 0;
来源：http://op.asd995.cn

[S29] C：变参函数
来源：http://xk.asd995.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kl.yuntaijiaju.cn

[S30] C：头文件保护
来源：http://gp.shtwfgs.cn

#ifndef X_H
来源：http://mt.newstarts.cn

#define X_H
来源：http://bp.yuntaijiaju.cn

#endif
来源：http://ra.muxihuayi.cn

[S31] C++：Hello World
来源：http://of.panjiajie.cn

#include <iostream>
来源：http://dd.521024.cn

int main() { std::cout << "Hello\n"; }
来源：http://ct.bookmarksfly.cn

[S32] C++：字符串
来源：http://gb.huixiangedu.cn

std::string s = "hi";  s += "!";
来源：http://eg.huanxung.cn

[S33] C++：vector 增删
来源：http://zk.yuntaijiaju.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ka.hnjuh.cn

[S34] C++：遍历 vector
来源：http://xv.muxihuayi.cn

for (auto &x : v) { std::cout << x; }
来源：http://zp.yuexingan06.cn

[S35] C++：map
来源：http://ml.chemitech.net.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bw.asd995.cn

[S36] C++：unordered_map
来源：http://ns.bookmarksfly.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nf.yuexingan06.cn

[S37] C++：set
来源：http://go.lnxyls.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yq.shxzukj.cn

[S38] C++：排序
来源：http://xs.colortex.cn

std::sort(v.begin(), v.end());
来源：http://ei.huixiangedu.cn

[S39] C++：自定义比较器排序
来源：http://uo.panjiajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zz.huixiangedu.cn

[S40] C++：查找元素
来源：http://gc.newstarts.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ej.panjiajie.cn

[S41] C++：类与构造函数
来源：http://ph.jianghongdianzi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mp.huixinmuqiang.cn

[S42] C++：继承与虚函数
来源：http://oy.chemitech.net.cn

class B : public Base { public: void f() override {} };
来源：http://yw.huanxung.cn

[S43] C++：智能指针
来源：http://lm.nicolike.cn

auto p = std::make_unique<int>(5);
来源：http://cv.hnjuh.cn

[S44] C++：引用传参
来源：http://vl.muxihuayi.cn

void inc(int &x) { ++x; }
来源：http://rn.9csxet.cn

[S45] C++：lambda
来源：http://ao.shxzskj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://le.huixiangedu.cn

[S46] C++：函数模板
来源：http://ex.huanxung.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nk.newstarts.cn

[S47] C++：结构化绑定遍历
来源：http://gv.szxytkj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fv.yuntaijiaju.cn

[S48] C++：逐行读文件
来源：http://vp.gzmigu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ps.huanxung.cn

while (std::getline(in, line)) { }
来源：http://bf.asd995.cn

[S49] C++：写文件
来源：http://fd.jctech888.com.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://oy.hnjuh.cn

[S50] C++：格式化数字
来源：http://zx.lnxyls.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fe.jctech888.com.cn

[S51] C++：显式类型转换
来源：http://rb.huixinmuqiang.cn

static_cast<double>(a) / b
来源：http://xu.jianghongdianzi.cn

[S52] C++：const 与 noexcept
来源：http://sz.shtwfgs.cn

int size() const noexcept { return n_; }
来源：http://tv.newstarts.cn

[S53] C++：移动语义
来源：http://ut.shxzskj.cn

std::vector<int> w = std::move(v);
来源：http://eo.shxzskj.cn

[S54] C++：异常处理
来源：http://na.newstarts.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ed.huixinmuqiang.cn

[S55] C++：结构化绑定
来源：http://dg.szsharing.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vw.haigaiapp.cn

[S56] C++：optional
来源：http://ig.bjjhwx.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pq.muxihuayi.cn

[S57] C++：编译期常量
来源：http://qq.panjiajie.cn

constexpr int N = 10;
来源：http://ho.shxzskj.cn

[S58] C++：命名空间
来源：http://cj.yuexingan06.cn

namespace ns { int f() { return 1; } }
来源：http://la.wgjwhj.cn

[S59] C++：静态断言
来源：http://ec.bjjhwx.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yw.yuntaijiaju.cn

[S60] C++：遍历并删除元素
来源：http://nf.hahajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vs.hahajie.cn

================================================================================
来源：http://eg.521024.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://er.haigaiapp.cn

================================================================================
来源：http://dl.shtwfgs.cn

[T01] Kotlin：Hello World
来源：http://xj.newstarts.cn

println("Hello")
来源：http://lh.lnxyls.cn

[T02] Kotlin：变量
来源：http://hh.muxihuayi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ar.colortex.cn

[T03] Kotlin：字符串模板
来源：http://pn.521024.cn

"值: $b"
来源：http://vu.shxzukj.cn

[T04] Kotlin：空安全
来源：http://vw.bookmarksfly.cn

val n: String? = null;  n?.length
来源：http://px.chemitech.net.cn

[T05] Kotlin：when 表达式
来源：http://fs.szsharing.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bq.szsharing.cn

[T06] Kotlin：集合映射
来源：http://hc.nszjky.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://up.shxzskj.cn

[T07] Kotlin：集合过滤
来源：http://th.hahajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qj.panjiajie.cn

[T08] Kotlin：数据类
来源：http://sa.asd995.cn

data class User(val name: String, val age: Int)
来源：http://pm.bjjhwx.cn

[T09] Kotlin：扩展函数
来源：http://is.bookmarksfly.cn

fun String.exclaim() = this + "!"
来源：http://ly.yuexingan06.cn

[T10] Kotlin：默认参数
来源：http://zc.521024.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qz.muxihuayi.cn

[T11] Kotlin：协程
来源：http://ps.jianghongdianzi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://uz.huixinmuqiang.cn

[T12] Kotlin：解构声明
来源：http://dw.chemitech.net.cn

val (a, b) = Pair(1, 2)
来源：http://io.asd995.cn

[T13] Kotlin：只读 Map
来源：http://xt.szxytkj.cn

val m = mapOf("a" to 1)
来源：http://no.newstarts.cn

[T14] Kotlin：循环
来源：http://bk.yuntaijiaju.cn

for (i in 1..10) println(i)
来源：http://od.asd995.cn

[T15] Kotlin：接口
来源：http://jp.nicolike.cn

interface Shape { fun area(): Double }
来源：http://br.gzmigu.cn

[T16] Swift：Hello World
来源：http://cx.huixinmuqiang.cn

print("Hello")
来源：http://rn.shxzukj.cn

[T17] Swift：变量与常量
来源：http://dv.yuntaijiaju.cn

var a = 1;  let b = 2
来源：http://az.chemitech.net.cn

[T18] Swift：字符串插值
来源：http://hr.colortex.cn

"值: \(b)"
来源：http://sn.shtwfgs.cn

[T19] Swift：可选绑定
来源：http://tx.yuntaijiaju.cn

if let n = opt { print(n) }
来源：http://zj.bjjhwx.cn

[T20] Swift：数组操作
来源：http://fl.szxytkj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://cs.yuexingan06.cn

[T21] Swift：遍历
来源：http://ps.bjjhwx.cn

for x in a { print(x) }
来源：http://nq.huanxung.cn

[T22] Swift：字典
来源：http://mp.newstarts.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ah.yuexingan06.cn

[T23] Swift：函数
来源：http://rs.shtwfgs.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://so.jianghongdianzi.cn

[T24] Swift：闭包
来源：http://do.chemitech.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://db.yuntaijiaju.cn

[T25] Swift：结构体
来源：http://cb.lnxyls.cn

struct P { var x: Int }
来源：http://az.nszjky.cn

[T26] Swift：类与重写
来源：http://qj.huixinmuqiang.cn

class A: Base { override func f() {} }
来源：http://ih.szsharing.cn

[T27] Swift：错误处理
来源：http://cs.hahajie.cn

do { try f() } catch { print(error) }
来源：http://oh.bjjhwx.cn

[T28] Swift：枚举
来源：http://sx.jctech888.com.cn

enum Color { case red, green }
来源：http://tb.szxytkj.cn

[T29] Swift：guard 提前返回
来源：http://zj.bjjhwx.cn

guard let x = opt else { return }
来源：http://ar.jctech888.com.cn

[T30] Swift：协议
来源：http://gl.huixiangedu.cn

protocol Shape { func area() -> Double }
来源：http://xf.huanxung.cn

[T31] Lua：Hello World
来源：http://hf.hnjuh.cn

print("Hello")
来源：http://ny.yuntaijiaju.cn

[T32] Lua：局部变量
来源：http://iv.jctech888.com.cn

local a = 1
来源：http://un.bjjhwx.cn

[T33] Lua：表（数组）
来源：http://zc.chemitech.net.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://og.szxytkj.cn

[T34] Lua：遍历表
来源：http://va.haigaiapp.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://cm.521024.cn

[T35] Lua：字典表
来源：http://yg.chemitech.net.cn

local d = { a = 1 };  d.b = 2
来源：http://xa.hnjuh.cn

[T36] Lua：函数
来源：http://km.muxihuayi.cn

function add(a, b) return a + b end
来源：http://go.szxytkj.cn

[T37] Lua：字符串拼接
来源：http://yz.colortex.cn

"a" .. "b"
来源：http://er.muxihuayi.cn

[T38] Lua：条件
来源：http://ho.hnjuh.cn

if x > 0 then print("正") end
来源：http://qp.9csxet.cn

[T39] Lua：模式匹配
来源：http://br.newstarts.cn

string.find(s, "%d+")
来源：http://sx.chemitech.net.cn

[T40] Lua：元表
来源：http://ue.szsharing.cn

setmetatable({}, { __index = base })
来源：http://qk.shxzskj.cn

[T41] Perl：Hello World
来源：http://bz.nicolike.cn

print "Hello\n";
来源：http://ir.colortex.cn

[T42] Perl：变量类型
来源：http://nv.newstarts.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fy.huixinmuqiang.cn

[T43] Perl：字符串插值
来源：http://ux.huixinmuqiang.cn

"值: $a"
来源：http://ou.shtwfgs.cn

[T44] Perl：条件
来源：http://yy.huanxung.cn

if ($a > 0) { print "正"; }
来源：http://hl.hnjuh.cn

[T45] Perl：数组遍历
来源：http://mv.szsharing.cn

for my $x (@arr) { print $x; }
来源：http://go.yuexingan06.cn

[T46] Perl：哈希操作
来源：http://ug.szsharing.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nm.shxzukj.cn

[T47] Perl：正则捕获
来源：http://su.huixinmuqiang.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://hn.hnjuh.cn

[T48] Perl：正则替换
来源：http://bl.nicolike.cn

$s =~ s/old/new/g;
来源：http://cs.shtwfgs.cn

[T49] Perl：函数
来源：http://ar.huanxung.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ln.hnjuh.cn

[T50] Perl：逐行读文件
来源：http://tt.colortex.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wr.9csxet.cn

while (my $line = <$fh>) { print $line; }
来源：http://ak.shtwfgs.cn

[T51] Scala：Hello World
来源：http://zy.bookmarksfly.cn

println("Hello")
来源：http://ry.muxihuayi.cn

[T52] Scala：变量
来源：http://sw.newstarts.cn

val a = 1;  var b = 2
来源：http://ko.huixiangedu.cn

[T53] Scala：字符串插值
来源：http://ed.asd995.cn

s"值: $b"
来源：http://na.asd995.cn

[T54] Scala：集合映射
来源：http://wf.hahajie.cn

List(1, 2, 3).map(_ * 2)
来源：http://rx.asd995.cn

[T55] Scala：集合过滤
来源：http://xy.gzmigu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ij.shtwfgs.cn

[T56] Scala：样例类
来源：http://of.muxihuayi.cn

case class User(name: String, age: Int)
来源：http://ld.szsharing.cn

[T57] Scala：模式匹配
来源：http://jd.hahajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://rk.jianghongdianzi.cn

[T58] Scala：函数定义
来源：http://xw.hahajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ry.nicolike.cn

[T59] Scala：循环
来源：http://dx.nicolike.cn

for (i <- 1 to 10) println(i)
来源：http://qy.yuexingan06.cn

[T60] Scala：折叠
来源：http://hi.jctech888.com.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bw.newstarts.cn

================================================================================
来源：http://cz.521024.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yc.521024.cn

================================================================================
来源：http://jq.hahajie.cn

[U01] Py：创建虚拟环境
来源：http://sf.lnxyls.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vq.huixinmuqiang.cn

[U02] Py：导出 / 安装依赖
来源：http://xb.panjiajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nb.nszjky.cn

[U03] Py：加载 .env 配置
来源：http://sa.chemitech.net.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wj.nszjky.cn

[U04] Py：变量调试打印
来源：http://ss.colortex.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fv.nszjky.cn

[U05] Py：列表去重且保序
来源：http://hj.chemitech.net.cn

list(dict.fromkeys(arr))
来源：http://ls.szxytkj.cn

[U06] Py：合并两个字典
来源：http://mw.jianghongdianzi.cn

{**a, **b}
来源：http://ar.muxihuayi.cn

[U07] Py：反转字典键值
来源：http://mz.lnxyls.cn

{v: k for k, v in d.items()}
来源：http://av.newstarts.cn

[U08] Py：展平二维列表
来源：http://jn.huixiangedu.cn

[y for x in nested for y in x]
来源：http://ep.colortex.cn

[U09] Py：字典取最大值的键
来源：http://lc.panjiajie.cn

max(d, key=d.get)
来源：http://jx.haigaiapp.cn

[U10] Py：按值排序字典
来源：http://pg.lnxyls.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ja.nszjky.cn

[U11] Py：生成器表达式
来源：http://mp.bookmarksfly.cn

(x * 2 for x in arr)
来源：http://ea.shtwfgs.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ac.hahajie.cn

Counter(arr).most_common(3)
来源：http://ex.huanxung.cn

[U13] Py：固定长度队列
来源：http://sk.szsharing.cn

deque(maxlen=10)
来源：http://sd.wgjwhj.cn

[U14] Py：分组收集到列表
来源：http://wm.9csxet.cn

defaultdict(list)
来源：http://al.jianghongdianzi.cn

[U15] Py：高精度计时
来源：http://qf.haigaiapp.cn

t = time.perf_counter()
来源：http://wh.asd995.cn

[U16] Py：命令行参数解析
来源：http://oi.shtwfgs.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lm.haigaiapp.cn

[U17] Py：初始化日志
来源：http://fj.jctech888.com.cn

logging.basicConfig(level=logging.INFO)
来源：http://kr.panjiajie.cn

[U18] Py：预编译正则
来源：http://za.hahajie.cn

pat = re.compile(r"\d+")
来源：http://of.haigaiapp.cn

[U19] Py：正则替换带回调
来源：http://yo.huixiangedu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://eb.szxytkj.cn

[U20] Py：缓存函数结果
来源：http://ty.newstarts.cn

@functools.lru_cache(maxsize=None)
来源：http://ao.gzmigu.cn

[U21] Py：自定义上下文管理器
来源：http://if.shtwfgs.cn

@contextlib.contextmanager
来源：http://vh.wgjwhj.cn

[U22] Py：矩阵转置
来源：http://bb.lnxyls.cn

list(zip(*m))
来源：http://pi.asd995.cn

[U23] Py：分块读取大文件
来源：http://ek.huixiangedu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mg.chemitech.net.cn

[U24] Py：路径操作
来源：http://ta.jianghongdianzi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gn.asd995.cn

[U25] Py：CSV 按字典读
来源：http://dc.muxihuayi.cn

csv.DictReader(f)
来源：http://qz.9csxet.cn

[U26] Py：并发下载
来源：http://ol.nszjky.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://sp.huixiangedu.cn

[U27] Py：异步 HTTP
来源：http://gm.lnxyls.cn

aiohttp.ClientSession() 配合 async with
来源：http://xv.gzmigu.cn

[U28] Py：类型别名
来源：http://hw.shxzukj.cn

UserId = int
来源：http://rx.yuexingan06.cn

[U29] Py：属性校验
来源：http://kd.yuntaijiaju.cn

@property 与 @x.setter 配合
来源：http://oc.huixinmuqiang.cn

[U30] Py：数据类
来源：http://wr.szxytkj.cn

@dataclass(slots=True)
来源：http://fg.shxzukj.cn

[U31] Py：单测
来源：http://so.hahajie.cn

python -m pytest -q
来源：http://om.nszjky.cn

[U32] Py：代码格式化
来源：http://yz.huanxung.cn

ruff format . && ruff check --fix .
来源：http://qr.lnxyls.cn

[U33] Py：打包发布
来源：http://zy.haigaiapp.cn

python -m build  （依赖 pyproject.toml）
来源：http://pd.hahajie.cn

[U34] Py：判断编码
来源：http://rj.shtwfgs.cn

chardet.detect(raw)
来源：http://ca.huixiangedu.cn

[U35] Py：发送邮件
来源：http://br.gzmigu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://le.jctech888.com.cn

[U36] Py：定时任务
来源：http://ij.hnjuh.cn

schedule.every(10).minutes.do(job)
来源：http://xl.colortex.cn

[U37] Py：读写 Excel
来源：http://ov.521024.cn

pandas.read_excel / DataFrame.to_excel
来源：http://gw.chemitech.net.cn

[U38] Py：获取脚本所在目录
来源：http://wv.wgjwhj.cn

Path(__file__).resolve().parent
来源：http://hz.szsharing.cn


<!-- 参考信息 -->