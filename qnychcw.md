代发 wailian999

#include <iostream>
来源：http://mc.nicolike.cn

int main() { std::cout << "Hello\n"; }
来源：http://hh.9csxet.cn

[S32] C++：字符串
来源：http://af.shxzskj.cn

std::string s = "hi";  s += "!";
来源：http://cx.szxytkj.cn

[S33] C++：vector 增删
来源：http://li.newstarts.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rb.jianghongdianzi.cn

[S34] C++：遍历 vector
来源：http://ps.hnjuh.cn

for (auto &x : v) { std::cout << x; }
来源：http://ar.shtwfgs.cn

[S35] C++：map
来源：http://lp.yuntaijiaju.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zi.szxytkj.cn

[S36] C++：unordered_map
来源：http://fv.lnxyls.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yp.wgjwhj.cn

[S37] C++：set
来源：http://lk.jctech888.com.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ap.nszjky.cn

[S38] C++：排序
来源：http://ju.bookmarksfly.cn

std::sort(v.begin(), v.end());
来源：http://la.hahajie.cn

[S39] C++：自定义比较器排序
来源：http://pg.yuexingan06.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nd.newstarts.cn

[S40] C++：查找元素
来源：http://qa.shtwfgs.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bx.huixiangedu.cn

[S41] C++：类与构造函数
来源：http://vi.521024.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xv.chemitech.net.cn

[S42] C++：继承与虚函数
来源：http://rm.haigaiapp.cn

class B : public Base { public: void f() override {} };
来源：http://xu.yuntaijiaju.cn

[S43] C++：智能指针
来源：http://oz.muxihuayi.cn

auto p = std::make_unique<int>(5);
来源：http://oq.newstarts.cn

[S44] C++：引用传参
来源：http://ed.shxzskj.cn

void inc(int &x) { ++x; }
来源：http://kf.muxihuayi.cn

[S45] C++：lambda
来源：http://co.szsharing.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vp.muxihuayi.cn

[S46] C++：函数模板
来源：http://cf.szxytkj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jj.muxihuayi.cn

[S47] C++：结构化绑定遍历
来源：http://yv.jianghongdianzi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tf.newstarts.cn

[S48] C++：逐行读文件
来源：http://vd.huixinmuqiang.cn

std::ifstream in("a.txt");  std::string line;
来源：http://nx.yuntaijiaju.cn

while (std::getline(in, line)) { }
来源：http://dh.huixinmuqiang.cn

[S49] C++：写文件
来源：http://xc.hahajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qy.colortex.cn

[S50] C++：格式化数字
来源：http://wa.lnxyls.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://oi.nszjky.cn

[S51] C++：显式类型转换
来源：http://gz.haigaiapp.cn

static_cast<double>(a) / b
来源：http://lh.panjiajie.cn

[S52] C++：const 与 noexcept
来源：http://gs.yuexingan06.cn

int size() const noexcept { return n_; }
来源：http://kd.haigaiapp.cn

[S53] C++：移动语义
来源：http://hu.shxzukj.cn

std::vector<int> w = std::move(v);
来源：http://gn.bookmarksfly.cn

[S54] C++：异常处理
来源：http://jz.wgjwhj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ti.shxzukj.cn

[S55] C++：结构化绑定
来源：http://wx.hnjuh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ek.huixinmuqiang.cn

[S56] C++：optional
来源：http://ys.shxzukj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ct.huanxung.cn

[S57] C++：编译期常量
来源：http://yp.asd995.cn

constexpr int N = 10;
来源：http://et.hahajie.cn

[S58] C++：命名空间
来源：http://mz.lnxyls.cn

namespace ns { int f() { return 1; } }
来源：http://hl.huixinmuqiang.cn

[S59] C++：静态断言
来源：http://fp.chemitech.net.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fz.yuntaijiaju.cn

[S60] C++：遍历并删除元素
来源：http://uo.panjiajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zw.huanxung.cn

================================================================================
来源：http://mh.yuntaijiaju.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ms.bjjhwx.cn

================================================================================
来源：http://ju.newstarts.cn

[T01] Kotlin：Hello World
来源：http://vs.haigaiapp.cn

println("Hello")
来源：http://ro.jctech888.com.cn

[T02] Kotlin：变量
来源：http://nr.nicolike.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xt.shtwfgs.cn

[T03] Kotlin：字符串模板
来源：http://wj.shtwfgs.cn

"值: $b"
来源：http://uu.shxzskj.cn

[T04] Kotlin：空安全
来源：http://ng.nszjky.cn

val n: String? = null;  n?.length
来源：http://ov.haigaiapp.cn

[T05] Kotlin：when 表达式
来源：http://sk.shxzskj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bf.haigaiapp.cn

[T06] Kotlin：集合映射
来源：http://ws.huixiangedu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gn.haigaiapp.cn

[T07] Kotlin：集合过滤
来源：http://oh.nicolike.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fu.huixinmuqiang.cn

[T08] Kotlin：数据类
来源：http://xh.chemitech.net.cn

data class User(val name: String, val age: Int)
来源：http://gv.newstarts.cn

[T09] Kotlin：扩展函数
来源：http://kh.chemitech.net.cn

fun String.exclaim() = this + "!"
来源：http://dd.chemitech.net.cn

[T10] Kotlin：默认参数
来源：http://jb.panjiajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qf.chemitech.net.cn

[T11] Kotlin：协程
来源：http://rv.hahajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ah.jctech888.com.cn

[T12] Kotlin：解构声明
来源：http://ba.jianghongdianzi.cn

val (a, b) = Pair(1, 2)
来源：http://ea.szsharing.cn

[T13] Kotlin：只读 Map
来源：http://ph.colortex.cn

val m = mapOf("a" to 1)
来源：http://gu.9csxet.cn

[T14] Kotlin：循环
来源：http://ht.bookmarksfly.cn

for (i in 1..10) println(i)
来源：http://he.asd995.cn

[T15] Kotlin：接口
来源：http://ns.szsharing.cn

interface Shape { fun area(): Double }
来源：http://zh.haigaiapp.cn

[T16] Swift：Hello World
来源：http://il.szsharing.cn

print("Hello")
来源：http://vf.muxihuayi.cn

[T17] Swift：变量与常量
来源：http://ia.bookmarksfly.cn

var a = 1;  let b = 2
来源：http://jb.521024.cn

[T18] Swift：字符串插值
来源：http://rf.nszjky.cn

"值: \(b)"
来源：http://xw.shtwfgs.cn

[T19] Swift：可选绑定
来源：http://fd.colortex.cn

if let n = opt { print(n) }
来源：http://ta.nszjky.cn

[T20] Swift：数组操作
来源：http://co.chemitech.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ek.9csxet.cn

[T21] Swift：遍历
来源：http://vg.gzmigu.cn

for x in a { print(x) }
来源：http://oy.newstarts.cn

[T22] Swift：字典
来源：http://pk.wgjwhj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ky.panjiajie.cn

[T23] Swift：函数
来源：http://pl.chemitech.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://km.huanxung.cn

[T24] Swift：闭包
来源：http://gp.wgjwhj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://bt.hnjuh.cn

[T25] Swift：结构体
来源：http://rp.shxzskj.cn

struct P { var x: Int }
来源：http://mn.szxytkj.cn

[T26] Swift：类与重写
来源：http://hd.huanxung.cn

class A: Base { override func f() {} }
来源：http://bw.shtwfgs.cn

[T27] Swift：错误处理
来源：http://ij.huixinmuqiang.cn

do { try f() } catch { print(error) }
来源：http://wm.bookmarksfly.cn

[T28] Swift：枚举
来源：http://nh.newstarts.cn

enum Color { case red, green }
来源：http://oq.yuntaijiaju.cn

[T29] Swift：guard 提前返回
来源：http://tz.hahajie.cn

guard let x = opt else { return }
来源：http://mb.jianghongdianzi.cn

[T30] Swift：协议
来源：http://mt.wgjwhj.cn

protocol Shape { func area() -> Double }
来源：http://xg.hnjuh.cn

[T31] Lua：Hello World
来源：http://wi.newstarts.cn

print("Hello")
来源：http://wj.nszjky.cn

[T32] Lua：局部变量
来源：http://ed.panjiajie.cn

local a = 1
来源：http://zv.bookmarksfly.cn

[T33] Lua：表（数组）
来源：http://xy.newstarts.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://tz.huixinmuqiang.cn

[T34] Lua：遍历表
来源：http://bw.521024.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://hs.huixinmuqiang.cn

[T35] Lua：字典表
来源：http://zm.shxzskj.cn

local d = { a = 1 };  d.b = 2
来源：http://ae.521024.cn

[T36] Lua：函数
来源：http://ma.shxzukj.cn

function add(a, b) return a + b end
来源：http://ng.521024.cn

[T37] Lua：字符串拼接
来源：http://td.szxytkj.cn

"a" .. "b"
来源：http://ig.gzmigu.cn

[T38] Lua：条件
来源：http://mt.wgjwhj.cn

if x > 0 then print("正") end
来源：http://qv.colortex.cn

[T39] Lua：模式匹配
来源：http://gi.lnxyls.cn

string.find(s, "%d+")
来源：http://ep.wgjwhj.cn

[T40] Lua：元表
来源：http://wt.nicolike.cn

setmetatable({}, { __index = base })
来源：http://qe.huanxung.cn

[T41] Perl：Hello World
来源：http://cg.szsharing.cn

print "Hello\n";
来源：http://xn.jianghongdianzi.cn

[T42] Perl：变量类型
来源：http://bi.nszjky.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ik.9csxet.cn

[T43] Perl：字符串插值
来源：http://zi.huanxung.cn

"值: $a"
来源：http://at.wgjwhj.cn

[T44] Perl：条件
来源：http://ww.shxzukj.cn

if ($a > 0) { print "正"; }
来源：http://ut.bjjhwx.cn

[T45] Perl：数组遍历
来源：http://hu.521024.cn

for my $x (@arr) { print $x; }
来源：http://vj.newstarts.cn

[T46] Perl：哈希操作
来源：http://rh.bjjhwx.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nz.shxzskj.cn

[T47] Perl：正则捕获
来源：http://il.haigaiapp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://hx.nicolike.cn

[T48] Perl：正则替换
来源：http://wf.jctech888.com.cn

$s =~ s/old/new/g;
来源：http://pa.jctech888.com.cn

[T49] Perl：函数
来源：http://ka.jianghongdianzi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gn.szsharing.cn

[T50] Perl：逐行读文件
来源：http://xv.asd995.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ek.lnxyls.cn

while (my $line = <$fh>) { print $line; }
来源：http://yf.gzmigu.cn

[T51] Scala：Hello World
来源：http://dk.haigaiapp.cn

println("Hello")
来源：http://uq.panjiajie.cn

[T52] Scala：变量
来源：http://gg.panjiajie.cn

val a = 1;  var b = 2
来源：http://wd.yuntaijiaju.cn

[T53] Scala：字符串插值
来源：http://ak.chemitech.net.cn

s"值: $b"
来源：http://ot.huixiangedu.cn

[T54] Scala：集合映射
来源：http://tq.shxzukj.cn

List(1, 2, 3).map(_ * 2)
来源：http://li.nicolike.cn

[T55] Scala：集合过滤
来源：http://sr.shxzukj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://cr.shxzskj.cn

[T56] Scala：样例类
来源：http://by.yuntaijiaju.cn

case class User(name: String, age: Int)
来源：http://iu.colortex.cn

[T57] Scala：模式匹配
来源：http://bf.panjiajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://bw.huanxung.cn

[T58] Scala：函数定义
来源：http://ni.yuntaijiaju.cn

def add(a: Int, b: Int): Int = a + b
来源：http://uh.szxytkj.cn

[T59] Scala：循环
来源：http://gc.szxytkj.cn

for (i <- 1 to 10) println(i)
来源：http://se.shxzukj.cn

[T60] Scala：折叠
来源：http://og.jianghongdianzi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://oo.bjjhwx.cn

================================================================================
来源：http://pu.nicolike.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hu.chemitech.net.cn

================================================================================
来源：http://mq.nicolike.cn

[U01] Py：创建虚拟环境
来源：http://nv.nicolike.cn

python -m venv .venv && source .venv/bin/activate
来源：http://fg.jianghongdianzi.cn

[U02] Py：导出 / 安装依赖
来源：http://sq.huixiangedu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ir.shtwfgs.cn

[U03] Py：加载 .env 配置
来源：http://so.chemitech.net.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://nx.jianghongdianzi.cn

[U04] Py：变量调试打印
来源：http://kv.bjjhwx.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pn.bjjhwx.cn

[U05] Py：列表去重且保序
来源：http://nr.asd995.cn

list(dict.fromkeys(arr))
来源：http://nn.huanxung.cn

[U06] Py：合并两个字典
来源：http://yi.shxzukj.cn

{**a, **b}
来源：http://mt.haigaiapp.cn

[U07] Py：反转字典键值
来源：http://sp.9csxet.cn

{v: k for k, v in d.items()}
来源：http://xq.chemitech.net.cn

[U08] Py：展平二维列表
来源：http://yn.chemitech.net.cn

[y for x in nested for y in x]
来源：http://du.colortex.cn

[U09] Py：字典取最大值的键
来源：http://zo.bookmarksfly.cn

max(d, key=d.get)
来源：http://cn.gzmigu.cn

[U10] Py：按值排序字典
来源：http://fg.newstarts.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ta.nicolike.cn

[U11] Py：生成器表达式
来源：http://fy.jianghongdianzi.cn

(x * 2 for x in arr)
来源：http://jj.bjjhwx.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ey.huixiangedu.cn

Counter(arr).most_common(3)
来源：http://lr.yuntaijiaju.cn

[U13] Py：固定长度队列
来源：http://hn.shxzskj.cn

deque(maxlen=10)
来源：http://wh.lnxyls.cn

[U14] Py：分组收集到列表
来源：http://az.nicolike.cn

defaultdict(list)
来源：http://fc.wgjwhj.cn

[U15] Py：高精度计时
来源：http://wy.hahajie.cn

t = time.perf_counter()
来源：http://mu.wgjwhj.cn

[U16] Py：命令行参数解析
来源：http://kq.yuntaijiaju.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sk.bookmarksfly.cn

[U17] Py：初始化日志
来源：http://tl.szsharing.cn

logging.basicConfig(level=logging.INFO)
来源：http://dv.newstarts.cn

[U18] Py：预编译正则
来源：http://cm.chemitech.net.cn

pat = re.compile(r"\d+")
来源：http://ks.shxzukj.cn

[U19] Py：正则替换带回调
来源：http://iw.lnxyls.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ts.nicolike.cn

[U20] Py：缓存函数结果
来源：http://tp.lnxyls.cn

@functools.lru_cache(maxsize=None)
来源：http://ur.hnjuh.cn

[U21] Py：自定义上下文管理器
来源：http://qr.jctech888.com.cn

@contextlib.contextmanager
来源：http://te.szsharing.cn

[U22] Py：矩阵转置
来源：http://dd.hahajie.cn

list(zip(*m))
来源：http://ap.newstarts.cn

[U23] Py：分块读取大文件
来源：http://wc.huixinmuqiang.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mn.chemitech.net.cn

[U24] Py：路径操作
来源：http://xk.szxytkj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nv.yuntaijiaju.cn

[U25] Py：CSV 按字典读
来源：http://vd.bookmarksfly.cn

csv.DictReader(f)
来源：http://fi.521024.cn

[U26] Py：并发下载
来源：http://ru.yuexingan06.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qn.jianghongdianzi.cn

[U27] Py：异步 HTTP
来源：http://cz.shtwfgs.cn

aiohttp.ClientSession() 配合 async with
来源：http://qt.nszjky.cn

[U28] Py：类型别名
来源：http://yb.nszjky.cn

UserId = int
来源：http://yc.szsharing.cn

[U29] Py：属性校验
来源：http://sj.muxihuayi.cn

@property 与 @x.setter 配合
来源：http://ck.yuntaijiaju.cn

[U30] Py：数据类
来源：http://ij.jctech888.com.cn

@dataclass(slots=True)
来源：http://bw.shxzukj.cn

[U31] Py：单测
来源：http://qv.nszjky.cn

python -m pytest -q
来源：http://mx.shxzukj.cn

[U32] Py：代码格式化
来源：http://nu.shxzukj.cn

ruff format . && ruff check --fix .
来源：http://ps.asd995.cn

[U33] Py：打包发布
来源：http://kj.huanxung.cn

python -m build  （依赖 pyproject.toml）
来源：http://zm.asd995.cn

[U34] Py：判断编码
来源：http://ar.gzmigu.cn

chardet.detect(raw)
来源：http://hc.chemitech.net.cn

[U35] Py：发送邮件
来源：http://qj.szsharing.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fb.szxytkj.cn

[U36] Py：定时任务
来源：http://gg.shxzskj.cn

schedule.every(10).minutes.do(job)
来源：http://qw.bjjhwx.cn

[U37] Py：读写 Excel
来源：http://nc.newstarts.cn

pandas.read_excel / DataFrame.to_excel
来源：http://tz.hnjuh.cn

[U38] Py：获取脚本所在目录
来源：http://lv.haigaiapp.cn

Path(__file__).resolve().parent
来源：http://yi.colortex.cn

[U39] Py：判断是否在交互环境
来源：http://pp.shtwfgs.cn

sys.stdout.isatty()
来源：http://cw.hahajie.cn

[U40] Py：打印到标准错误
来源：http://rs.nicolike.cn

print("err", file=sys.stderr)
来源：http://ml.szxytkj.cn

[U41] PHP：初始化 Composer 项目
来源：http://xa.bookmarksfly.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://in.wgjwhj.cn

[U42] PHP：PSR-4 自动加载
来源：http://gv.gzmigu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://la.shtwfgs.cn

[U43] PHP：声明命名空间
来源：http://cr.wgjwhj.cn

namespace App\Http;
来源：http://kv.newstarts.cn

[U44] PHP：开启严格类型
来源：http://ak.haigaiapp.cn

declare(strict_types=1);
来源：http://sw.9csxet.cn

[U45] PHP：类型声明与返回类型
来源：http://au.szxytkj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://mr.nicolike.cn

[U46] PHP：可空类型
来源：http://zp.shtwfgs.cn

?string $name = null
来源：http://ih.gzmigu.cn

[U47] PHP：联合类型
来源：http://pd.hahajie.cn

int|string $id
来源：http://ky.panjiajie.cn

[U48] PHP：纯枚举
来源：http://hs.asd995.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lf.jctech888.com.cn

[U49] PHP：只读属性
来源：http://wx.haigaiapp.cn

public readonly string $name
来源：http://gz.szxytkj.cn

[U50] PHP：构造器属性提升
来源：http://ms.huanxung.cn

public function __construct(private int $id) {}
来源：http://cu.panjiajie.cn

[U51] PHP：数组解构
来源：http://am.521024.cn

[$a, $b] = $arr;
来源：http://ht.szxytkj.cn

[U52] PHP：箭头函数
来源：http://ln.bookmarksfly.cn

$double = fn($x) => $x * 2;
来源：http://se.nicolike.cn

[U53] PHP：空合并运算符
来源：http://ja.nszjky.cn

$v = $a ?? $b ?? "default";
来源：http://jz.panjiajie.cn

[U54] PHP：空安全调用
来源：http://ht.521024.cn

$obj?->method()
来源：http://qx.szsharing.cn

[U55] PHP：match 表达式
来源：http://sx.521024.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tb.yuexingan06.cn

[U56] PHP：命名参数
来源：http://sz.szxytkj.cn

f(a: 1, b: 2)
来源：http://ds.bjjhwx.cn


<!-- 参考信息 -->