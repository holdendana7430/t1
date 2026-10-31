代发 wailian999

[S41] C++：类与构造函数
来源：http://ad.muxihuayi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mw.panjiajie.cn

[S42] C++：继承与虚函数
来源：http://ts.nicolike.cn

class B : public Base { public: void f() override {} };
来源：http://jl.hnjuh.cn

[S43] C++：智能指针
来源：http://fx.bookmarksfly.cn

auto p = std::make_unique<int>(5);
来源：http://mz.nicolike.cn

[S44] C++：引用传参
来源：http://lz.hahajie.cn

void inc(int &x) { ++x; }
来源：http://nt.bjjhwx.cn

[S45] C++：lambda
来源：http://et.shxzskj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dm.bjjhwx.cn

[S46] C++：函数模板
来源：http://rg.szsharing.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://us.nszjky.cn

[S47] C++：结构化绑定遍历
来源：http://bp.bjjhwx.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bo.nicolike.cn

[S48] C++：逐行读文件
来源：http://qx.gzmigu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vy.bjjhwx.cn

while (std::getline(in, line)) { }
来源：http://jl.muxihuayi.cn

[S49] C++：写文件
来源：http://yr.haigaiapp.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://br.521024.cn

[S50] C++：格式化数字
来源：http://rn.hahajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jh.hnjuh.cn

[S51] C++：显式类型转换
来源：http://jo.huanxung.cn

static_cast<double>(a) / b
来源：http://ou.haigaiapp.cn

[S52] C++：const 与 noexcept
来源：http://ja.jianghongdianzi.cn

int size() const noexcept { return n_; }
来源：http://un.muxihuayi.cn

[S53] C++：移动语义
来源：http://fb.colortex.cn

std::vector<int> w = std::move(v);
来源：http://yr.szxytkj.cn

[S54] C++：异常处理
来源：http://jr.yuntaijiaju.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://np.yuntaijiaju.cn

[S55] C++：结构化绑定
来源：http://di.asd995.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bt.newstarts.cn

[S56] C++：optional
来源：http://sa.colortex.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kn.yuexingan06.cn

[S57] C++：编译期常量
来源：http://an.huanxung.cn

constexpr int N = 10;
来源：http://ra.szsharing.cn

[S58] C++：命名空间
来源：http://gc.panjiajie.cn

namespace ns { int f() { return 1; } }
来源：http://jc.huanxung.cn

[S59] C++：静态断言
来源：http://ci.colortex.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vq.shxzskj.cn

[S60] C++：遍历并删除元素
来源：http://mo.panjiajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fd.hnjuh.cn

================================================================================
来源：http://ws.panjiajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://is.wgjwhj.cn

================================================================================
来源：http://ys.colortex.cn

[T01] Kotlin：Hello World
来源：http://ew.shxzukj.cn

println("Hello")
来源：http://lr.panjiajie.cn

[T02] Kotlin：变量
来源：http://vu.bjjhwx.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rs.newstarts.cn

[T03] Kotlin：字符串模板
来源：http://yj.asd995.cn

"值: $b"
来源：http://ka.haigaiapp.cn

[T04] Kotlin：空安全
来源：http://ek.nicolike.cn

val n: String? = null;  n?.length
来源：http://ze.asd995.cn

[T05] Kotlin：when 表达式
来源：http://dl.yuexingan06.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://st.chemitech.net.cn

[T06] Kotlin：集合映射
来源：http://gl.huixiangedu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gk.shtwfgs.cn

[T07] Kotlin：集合过滤
来源：http://vu.hahajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vx.gzmigu.cn

[T08] Kotlin：数据类
来源：http://vs.521024.cn

data class User(val name: String, val age: Int)
来源：http://in.shxzskj.cn

[T09] Kotlin：扩展函数
来源：http://vk.gzmigu.cn

fun String.exclaim() = this + "!"
来源：http://ct.asd995.cn

[T10] Kotlin：默认参数
来源：http://ne.jianghongdianzi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hf.9csxet.cn

[T11] Kotlin：协程
来源：http://mx.bookmarksfly.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ho.huixiangedu.cn

[T12] Kotlin：解构声明
来源：http://ye.huixiangedu.cn

val (a, b) = Pair(1, 2)
来源：http://ss.9csxet.cn

[T13] Kotlin：只读 Map
来源：http://tg.colortex.cn

val m = mapOf("a" to 1)
来源：http://dp.yuntaijiaju.cn

[T14] Kotlin：循环
来源：http://sw.9csxet.cn

for (i in 1..10) println(i)
来源：http://wv.9csxet.cn

[T15] Kotlin：接口
来源：http://wg.wgjwhj.cn

interface Shape { fun area(): Double }
来源：http://sc.wgjwhj.cn

[T16] Swift：Hello World
来源：http://hq.hnjuh.cn

print("Hello")
来源：http://ps.bjjhwx.cn

[T17] Swift：变量与常量
来源：http://vt.jianghongdianzi.cn

var a = 1;  let b = 2
来源：http://xf.521024.cn

[T18] Swift：字符串插值
来源：http://ie.chemitech.net.cn

"值: \(b)"
来源：http://rh.gzmigu.cn

[T19] Swift：可选绑定
来源：http://hy.haigaiapp.cn

if let n = opt { print(n) }
来源：http://zl.panjiajie.cn

[T20] Swift：数组操作
来源：http://lg.muxihuayi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://th.haigaiapp.cn

[T21] Swift：遍历
来源：http://uj.shxzskj.cn

for x in a { print(x) }
来源：http://xv.9csxet.cn

[T22] Swift：字典
来源：http://tf.nszjky.cn

var d = ["a": 1];  d["b"] = 2
来源：http://yr.newstarts.cn

[T23] Swift：函数
来源：http://lv.wgjwhj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xt.hahajie.cn

[T24] Swift：闭包
来源：http://kj.jianghongdianzi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://od.yuexingan06.cn

[T25] Swift：结构体
来源：http://ks.shxzukj.cn

struct P { var x: Int }
来源：http://gg.yuexingan06.cn

[T26] Swift：类与重写
来源：http://hk.jctech888.com.cn

class A: Base { override func f() {} }
来源：http://ym.jctech888.com.cn

[T27] Swift：错误处理
来源：http://fn.panjiajie.cn

do { try f() } catch { print(error) }
来源：http://wr.haigaiapp.cn

[T28] Swift：枚举
来源：http://ix.newstarts.cn

enum Color { case red, green }
来源：http://st.jctech888.com.cn

[T29] Swift：guard 提前返回
来源：http://bl.chemitech.net.cn

guard let x = opt else { return }
来源：http://up.nicolike.cn

[T30] Swift：协议
来源：http://as.szsharing.cn

protocol Shape { func area() -> Double }
来源：http://bo.nicolike.cn

[T31] Lua：Hello World
来源：http://uk.colortex.cn

print("Hello")
来源：http://ts.jianghongdianzi.cn

[T32] Lua：局部变量
来源：http://td.shxzskj.cn

local a = 1
来源：http://rp.colortex.cn

[T33] Lua：表（数组）
来源：http://xh.muxihuayi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://dw.wgjwhj.cn

[T34] Lua：遍历表
来源：http://yi.panjiajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://oo.haigaiapp.cn

[T35] Lua：字典表
来源：http://cl.huixinmuqiang.cn

local d = { a = 1 };  d.b = 2
来源：http://xs.wgjwhj.cn

[T36] Lua：函数
来源：http://bx.asd995.cn

function add(a, b) return a + b end
来源：http://tb.szxytkj.cn

[T37] Lua：字符串拼接
来源：http://yv.521024.cn

"a" .. "b"
来源：http://yk.szsharing.cn

[T38] Lua：条件
来源：http://zv.nszjky.cn

if x > 0 then print("正") end
来源：http://fy.yuntaijiaju.cn

[T39] Lua：模式匹配
来源：http://bc.shtwfgs.cn

string.find(s, "%d+")
来源：http://aw.gzmigu.cn

[T40] Lua：元表
来源：http://fd.bookmarksfly.cn

setmetatable({}, { __index = base })
来源：http://jd.shtwfgs.cn

[T41] Perl：Hello World
来源：http://ce.hnjuh.cn

print "Hello\n";
来源：http://eo.9csxet.cn

[T42] Perl：变量类型
来源：http://fn.hahajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ot.jctech888.com.cn

[T43] Perl：字符串插值
来源：http://lu.szxytkj.cn

"值: $a"
来源：http://tf.chemitech.net.cn

[T44] Perl：条件
来源：http://rr.huanxung.cn

if ($a > 0) { print "正"; }
来源：http://ei.szxytkj.cn

[T45] Perl：数组遍历
来源：http://ue.9csxet.cn

for my $x (@arr) { print $x; }
来源：http://mt.newstarts.cn

[T46] Perl：哈希操作
来源：http://fd.hnjuh.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jt.szsharing.cn

[T47] Perl：正则捕获
来源：http://vt.jctech888.com.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ob.nicolike.cn

[T48] Perl：正则替换
来源：http://sl.wgjwhj.cn

$s =~ s/old/new/g;
来源：http://mc.yuntaijiaju.cn

[T49] Perl：函数
来源：http://mr.bookmarksfly.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xu.yuntaijiaju.cn

[T50] Perl：逐行读文件
来源：http://yi.shxzskj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://px.shxzskj.cn

while (my $line = <$fh>) { print $line; }
来源：http://yo.bjjhwx.cn

[T51] Scala：Hello World
来源：http://ng.szxytkj.cn

println("Hello")
来源：http://ut.panjiajie.cn

[T52] Scala：变量
来源：http://rl.szxytkj.cn

val a = 1;  var b = 2
来源：http://ms.yuntaijiaju.cn

[T53] Scala：字符串插值
来源：http://qi.muxihuayi.cn

s"值: $b"
来源：http://yf.hahajie.cn

[T54] Scala：集合映射
来源：http://ij.muxihuayi.cn

List(1, 2, 3).map(_ * 2)
来源：http://gp.szxytkj.cn

[T55] Scala：集合过滤
来源：http://mc.muxihuayi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qt.lnxyls.cn

[T56] Scala：样例类
来源：http://sz.wgjwhj.cn

case class User(name: String, age: Int)
来源：http://vt.newstarts.cn

[T57] Scala：模式匹配
来源：http://ph.szxytkj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gw.szxytkj.cn

[T58] Scala：函数定义
来源：http://xb.szxytkj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zr.yuexingan06.cn

[T59] Scala：循环
来源：http://pc.bjjhwx.cn

for (i <- 1 to 10) println(i)
来源：http://ge.jctech888.com.cn

[T60] Scala：折叠
来源：http://en.521024.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nw.lnxyls.cn

================================================================================
来源：http://ul.huanxung.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ul.szsharing.cn

================================================================================
来源：http://nd.hahajie.cn

[U01] Py：创建虚拟环境
来源：http://oi.yuexingan06.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qp.hnjuh.cn

[U02] Py：导出 / 安装依赖
来源：http://vl.hnjuh.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hg.gzmigu.cn

[U03] Py：加载 .env 配置
来源：http://jw.huixinmuqiang.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fm.yuexingan06.cn

[U04] Py：变量调试打印
来源：http://pz.jctech888.com.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bs.huanxung.cn

[U05] Py：列表去重且保序
来源：http://an.bjjhwx.cn

list(dict.fromkeys(arr))
来源：http://dk.chemitech.net.cn

[U06] Py：合并两个字典
来源：http://cd.shtwfgs.cn

{**a, **b}
来源：http://ml.yuexingan06.cn

[U07] Py：反转字典键值
来源：http://po.shxzskj.cn

{v: k for k, v in d.items()}
来源：http://eu.nicolike.cn

[U08] Py：展平二维列表
来源：http://dm.huanxung.cn

[y for x in nested for y in x]
来源：http://gh.szsharing.cn

[U09] Py：字典取最大值的键
来源：http://dl.shtwfgs.cn

max(d, key=d.get)
来源：http://ai.asd995.cn

[U10] Py：按值排序字典
来源：http://zb.nicolike.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ys.shtwfgs.cn

[U11] Py：生成器表达式
来源：http://cn.hahajie.cn

(x * 2 for x in arr)
来源：http://jt.huixinmuqiang.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ar.jianghongdianzi.cn

Counter(arr).most_common(3)
来源：http://gu.yuexingan06.cn

[U13] Py：固定长度队列
来源：http://ul.asd995.cn

deque(maxlen=10)
来源：http://xl.newstarts.cn

[U14] Py：分组收集到列表
来源：http://bo.521024.cn

defaultdict(list)
来源：http://yh.panjiajie.cn

[U15] Py：高精度计时
来源：http://jg.newstarts.cn

t = time.perf_counter()
来源：http://ed.asd995.cn

[U16] Py：命令行参数解析
来源：http://hm.shxzukj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ua.panjiajie.cn

[U17] Py：初始化日志
来源：http://gg.wgjwhj.cn

logging.basicConfig(level=logging.INFO)
来源：http://of.panjiajie.cn

[U18] Py：预编译正则
来源：http://od.szsharing.cn

pat = re.compile(r"\d+")
来源：http://eu.wgjwhj.cn

[U19] Py：正则替换带回调
来源：http://yx.wgjwhj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ma.lnxyls.cn

[U20] Py：缓存函数结果
来源：http://ho.asd995.cn

@functools.lru_cache(maxsize=None)
来源：http://we.hnjuh.cn

[U21] Py：自定义上下文管理器
来源：http://jx.lnxyls.cn

@contextlib.contextmanager
来源：http://xa.shxzukj.cn

[U22] Py：矩阵转置
来源：http://pp.colortex.cn

list(zip(*m))
来源：http://ox.bookmarksfly.cn

[U23] Py：分块读取大文件
来源：http://jd.chemitech.net.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bx.wgjwhj.cn

[U24] Py：路径操作
来源：http://nq.jctech888.com.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jo.lnxyls.cn

[U25] Py：CSV 按字典读
来源：http://nz.huanxung.cn

csv.DictReader(f)
来源：http://ef.muxihuayi.cn

[U26] Py：并发下载
来源：http://sk.shxzukj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cr.colortex.cn

[U27] Py：异步 HTTP
来源：http://ou.yuexingan06.cn

aiohttp.ClientSession() 配合 async with
来源：http://yb.bookmarksfly.cn

[U28] Py：类型别名
来源：http://wm.newstarts.cn

UserId = int
来源：http://fh.bookmarksfly.cn

[U29] Py：属性校验
来源：http://wa.nicolike.cn

@property 与 @x.setter 配合
来源：http://fn.newstarts.cn

[U30] Py：数据类
来源：http://or.shxzukj.cn

@dataclass(slots=True)
来源：http://eb.muxihuayi.cn

[U31] Py：单测
来源：http://lj.huixinmuqiang.cn

python -m pytest -q
来源：http://hs.asd995.cn

[U32] Py：代码格式化
来源：http://cv.gzmigu.cn

ruff format . && ruff check --fix .
来源：http://hh.newstarts.cn

[U33] Py：打包发布
来源：http://xb.huanxung.cn

python -m build  （依赖 pyproject.toml）
来源：http://km.huixinmuqiang.cn

[U34] Py：判断编码
来源：http://su.muxihuayi.cn

chardet.detect(raw)
来源：http://lu.shtwfgs.cn

[U35] Py：发送邮件
来源：http://sw.jianghongdianzi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zx.hnjuh.cn

[U36] Py：定时任务
来源：http://wk.huanxung.cn

schedule.every(10).minutes.do(job)
来源：http://zm.bjjhwx.cn

[U37] Py：读写 Excel
来源：http://pz.shxzukj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://vs.newstarts.cn

[U38] Py：获取脚本所在目录
来源：http://ss.9csxet.cn

Path(__file__).resolve().parent
来源：http://de.newstarts.cn

[U39] Py：判断是否在交互环境
来源：http://js.newstarts.cn

sys.stdout.isatty()
来源：http://eq.hnjuh.cn

[U40] Py：打印到标准错误
来源：http://lv.521024.cn

print("err", file=sys.stderr)
来源：http://eq.muxihuayi.cn

[U41] PHP：初始化 Composer 项目
来源：http://ta.bjjhwx.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://pw.chemitech.net.cn

[U42] PHP：PSR-4 自动加载
来源：http://cx.jctech888.com.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fp.szsharing.cn

[U43] PHP：声明命名空间
来源：http://ah.hnjuh.cn

namespace App\Http;
来源：http://xh.521024.cn

[U44] PHP：开启严格类型
来源：http://ku.bjjhwx.cn

declare(strict_types=1);
来源：http://ea.shxzukj.cn

[U45] PHP：类型声明与返回类型
来源：http://vn.huixinmuqiang.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://mb.bjjhwx.cn

[U46] PHP：可空类型
来源：http://zj.shxzskj.cn

?string $name = null
来源：http://se.521024.cn

[U47] PHP：联合类型
来源：http://cw.shxzskj.cn

int|string $id
来源：http://aa.asd995.cn

[U48] PHP：纯枚举
来源：http://kk.szxytkj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xi.shxzskj.cn

[U49] PHP：只读属性
来源：http://fu.szxytkj.cn

public readonly string $name
来源：http://za.yuntaijiaju.cn

[U50] PHP：构造器属性提升
来源：http://ld.haigaiapp.cn

public function __construct(private int $id) {}
来源：http://vb.nicolike.cn

[U51] PHP：数组解构
来源：http://xe.shxzukj.cn

[$a, $b] = $arr;
来源：http://jy.shxzukj.cn

[U52] PHP：箭头函数
来源：http://vi.hnjuh.cn

$double = fn($x) => $x * 2;
来源：http://ah.panjiajie.cn

[U53] PHP：空合并运算符
来源：http://br.521024.cn

$v = $a ?? $b ?? "default";
来源：http://wh.jianghongdianzi.cn

[U54] PHP：空安全调用
来源：http://mv.shxzukj.cn

$obj?->method()
来源：http://lx.nszjky.cn

[U55] PHP：match 表达式
来源：http://ox.lnxyls.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://oh.bookmarksfly.cn

[U56] PHP：命名参数
来源：http://dq.colortex.cn

f(a: 1, b: 2)
来源：http://et.9csxet.cn

[U57] PHP：字符串插值
来源：http://pe.jctech888.com.cn

"值: {$a}"
来源：http://mn.lnxyls.cn

[U58] PHP：数组三件套
来源：http://dn.yuntaijiaju.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qf.jianghongdianzi.cn

[U59] PHP：自定义排序
来源：http://fo.bookmarksfly.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rz.haigaiapp.cn

[U60] PHP：JSON 编解码
来源：http://hy.jctech888.com.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pl.9csxet.cn

[U61] PHP：正则
来源：http://ge.chemitech.net.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cj.shxzukj.cn

[U62] PHP：日期对象
来源：http://qp.yuntaijiaju.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://we.szxytkj.cn

[U63] PHP：文件读写
来源：http://qd.nicolike.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lb.nszjky.cn

[U64] PHP：目录遍历
来源：http://nb.nicolike.cn

glob("dir/*.php");  scandir("dir");
来源：http://xk.nicolike.cn

[U65] PHP：会话
来源：http://nn.bjjhwx.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vb.wgjwhj.cn

[U66] PHP：设置 Cookie
来源：http://zq.panjiajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nj.yuexingan06.cn


<!-- 参考信息 -->