代发 wailian999

[S41] C++：类与构造函数
来源：http://jv.lnxyls.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ea.yuntaijiaju.cn

[S42] C++：继承与虚函数
来源：http://lw.jianghongdianzi.cn

class B : public Base { public: void f() override {} };
来源：http://ao.bjjhwx.cn

[S43] C++：智能指针
来源：http://gm.hahajie.cn

auto p = std::make_unique<int>(5);
来源：http://wm.shxzskj.cn

[S44] C++：引用传参
来源：http://oc.hnjuh.cn

void inc(int &x) { ++x; }
来源：http://jh.huanxung.cn

[S45] C++：lambda
来源：http://ty.nicolike.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bb.newstarts.cn

[S46] C++：函数模板
来源：http://kb.bjjhwx.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nq.nszjky.cn

[S47] C++：结构化绑定遍历
来源：http://ku.shtwfgs.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nw.huixiangedu.cn

[S48] C++：逐行读文件
来源：http://ee.szsharing.cn

std::ifstream in("a.txt");  std::string line;
来源：http://bd.hnjuh.cn

while (std::getline(in, line)) { }
来源：http://qr.huixinmuqiang.cn

[S49] C++：写文件
来源：http://ik.haigaiapp.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ft.muxihuayi.cn

[S50] C++：格式化数字
来源：http://xc.hnjuh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gw.hnjuh.cn

[S51] C++：显式类型转换
来源：http://be.lnxyls.cn

static_cast<double>(a) / b
来源：http://ib.panjiajie.cn

[S52] C++：const 与 noexcept
来源：http://vq.huixinmuqiang.cn

int size() const noexcept { return n_; }
来源：http://uo.yuntaijiaju.cn

[S53] C++：移动语义
来源：http://kk.9csxet.cn

std::vector<int> w = std::move(v);
来源：http://xq.huixinmuqiang.cn

[S54] C++：异常处理
来源：http://wa.panjiajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kg.huixinmuqiang.cn

[S55] C++：结构化绑定
来源：http://ib.bjjhwx.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://nx.jctech888.com.cn

[S56] C++：optional
来源：http://sp.shxzskj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dc.nicolike.cn

[S57] C++：编译期常量
来源：http://xv.asd995.cn

constexpr int N = 10;
来源：http://dk.hahajie.cn

[S58] C++：命名空间
来源：http://ti.521024.cn

namespace ns { int f() { return 1; } }
来源：http://ih.colortex.cn

[S59] C++：静态断言
来源：http://zz.lnxyls.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yk.nszjky.cn

[S60] C++：遍历并删除元素
来源：http://rw.jctech888.com.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rn.szxytkj.cn

================================================================================
来源：http://gt.muxihuayi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rh.yuntaijiaju.cn

================================================================================
来源：http://xq.wgjwhj.cn

[T01] Kotlin：Hello World
来源：http://lp.nszjky.cn

println("Hello")
来源：http://kl.gzmigu.cn

[T02] Kotlin：变量
来源：http://uw.huanxung.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://la.hahajie.cn

[T03] Kotlin：字符串模板
来源：http://yb.yuntaijiaju.cn

"值: $b"
来源：http://uu.hnjuh.cn

[T04] Kotlin：空安全
来源：http://mf.shxzukj.cn

val n: String? = null;  n?.length
来源：http://gx.muxihuayi.cn

[T05] Kotlin：when 表达式
来源：http://sv.yuntaijiaju.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vv.asd995.cn

[T06] Kotlin：集合映射
来源：http://xr.huanxung.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://qk.hahajie.cn

[T07] Kotlin：集合过滤
来源：http://yp.yuexingan06.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://nm.jianghongdianzi.cn

[T08] Kotlin：数据类
来源：http://qs.shtwfgs.cn

data class User(val name: String, val age: Int)
来源：http://hu.szsharing.cn

[T09] Kotlin：扩展函数
来源：http://mx.wgjwhj.cn

fun String.exclaim() = this + "!"
来源：http://wn.huixiangedu.cn

[T10] Kotlin：默认参数
来源：http://ht.shtwfgs.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://so.jianghongdianzi.cn

[T11] Kotlin：协程
来源：http://vk.shxzskj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ou.szsharing.cn

[T12] Kotlin：解构声明
来源：http://dj.colortex.cn

val (a, b) = Pair(1, 2)
来源：http://vs.colortex.cn

[T13] Kotlin：只读 Map
来源：http://xf.hahajie.cn

val m = mapOf("a" to 1)
来源：http://ou.jctech888.com.cn

[T14] Kotlin：循环
来源：http://ey.colortex.cn

for (i in 1..10) println(i)
来源：http://vw.jianghongdianzi.cn

[T15] Kotlin：接口
来源：http://kn.colortex.cn

interface Shape { fun area(): Double }
来源：http://pk.szsharing.cn

[T16] Swift：Hello World
来源：http://re.chemitech.net.cn

print("Hello")
来源：http://lx.hnjuh.cn

[T17] Swift：变量与常量
来源：http://qm.szsharing.cn

var a = 1;  let b = 2
来源：http://qy.nszjky.cn

[T18] Swift：字符串插值
来源：http://sf.shtwfgs.cn

"值: \(b)"
来源：http://ck.521024.cn

[T19] Swift：可选绑定
来源：http://na.muxihuayi.cn

if let n = opt { print(n) }
来源：http://sl.colortex.cn

[T20] Swift：数组操作
来源：http://fv.521024.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ee.newstarts.cn

[T21] Swift：遍历
来源：http://la.huixiangedu.cn

for x in a { print(x) }
来源：http://jd.hnjuh.cn

[T22] Swift：字典
来源：http://zt.bookmarksfly.cn

var d = ["a": 1];  d["b"] = 2
来源：http://gd.jianghongdianzi.cn

[T23] Swift：函数
来源：http://hm.gzmigu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uy.muxihuayi.cn

[T24] Swift：闭包
来源：http://cp.nicolike.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://fe.colortex.cn

[T25] Swift：结构体
来源：http://mi.hnjuh.cn

struct P { var x: Int }
来源：http://uj.gzmigu.cn

[T26] Swift：类与重写
来源：http://zd.hnjuh.cn

class A: Base { override func f() {} }
来源：http://kz.szxytkj.cn

[T27] Swift：错误处理
来源：http://bo.hnjuh.cn

do { try f() } catch { print(error) }
来源：http://pi.nszjky.cn

[T28] Swift：枚举
来源：http://hk.shxzukj.cn

enum Color { case red, green }
来源：http://mu.bjjhwx.cn

[T29] Swift：guard 提前返回
来源：http://hn.bookmarksfly.cn

guard let x = opt else { return }
来源：http://iw.huixiangedu.cn

[T30] Swift：协议
来源：http://su.gzmigu.cn

protocol Shape { func area() -> Double }
来源：http://gq.newstarts.cn

[T31] Lua：Hello World
来源：http://wv.lnxyls.cn

print("Hello")
来源：http://sy.yuntaijiaju.cn

[T32] Lua：局部变量
来源：http://sw.huixinmuqiang.cn

local a = 1
来源：http://sa.521024.cn

[T33] Lua：表（数组）
来源：http://lr.asd995.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://it.lnxyls.cn

[T34] Lua：遍历表
来源：http://ah.shxzskj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://sz.szxytkj.cn

[T35] Lua：字典表
来源：http://of.wgjwhj.cn

local d = { a = 1 };  d.b = 2
来源：http://rm.huanxung.cn

[T36] Lua：函数
来源：http://iz.asd995.cn

function add(a, b) return a + b end
来源：http://bm.shxzskj.cn

[T37] Lua：字符串拼接
来源：http://wt.hahajie.cn

"a" .. "b"
来源：http://vr.wgjwhj.cn

[T38] Lua：条件
来源：http://gw.huixiangedu.cn

if x > 0 then print("正") end
来源：http://lr.wgjwhj.cn

[T39] Lua：模式匹配
来源：http://xj.jctech888.com.cn

string.find(s, "%d+")
来源：http://uz.hahajie.cn

[T40] Lua：元表
来源：http://gg.bjjhwx.cn

setmetatable({}, { __index = base })
来源：http://ld.yuexingan06.cn

[T41] Perl：Hello World
来源：http://gv.hnjuh.cn

print "Hello\n";
来源：http://rn.hahajie.cn

[T42] Perl：变量类型
来源：http://ic.huanxung.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jm.bookmarksfly.cn

[T43] Perl：字符串插值
来源：http://dq.gzmigu.cn

"值: $a"
来源：http://hm.shtwfgs.cn

[T44] Perl：条件
来源：http://xk.szsharing.cn

if ($a > 0) { print "正"; }
来源：http://fh.bjjhwx.cn

[T45] Perl：数组遍历
来源：http://px.bookmarksfly.cn

for my $x (@arr) { print $x; }
来源：http://uu.gzmigu.cn

[T46] Perl：哈希操作
来源：http://zk.yuntaijiaju.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ch.panjiajie.cn

[T47] Perl：正则捕获
来源：http://hk.yuntaijiaju.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://be.lnxyls.cn

[T48] Perl：正则替换
来源：http://lo.hnjuh.cn

$s =~ s/old/new/g;
来源：http://ui.nicolike.cn

[T49] Perl：函数
来源：http://bh.yuntaijiaju.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ik.nicolike.cn

[T50] Perl：逐行读文件
来源：http://mw.yuntaijiaju.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://bb.huanxung.cn

while (my $line = <$fh>) { print $line; }
来源：http://nk.szxytkj.cn

[T51] Scala：Hello World
来源：http://jb.szsharing.cn

println("Hello")
来源：http://ap.shxzskj.cn

[T52] Scala：变量
来源：http://ov.wgjwhj.cn

val a = 1;  var b = 2
来源：http://yk.jianghongdianzi.cn

[T53] Scala：字符串插值
来源：http://mz.shtwfgs.cn

s"值: $b"
来源：http://mh.wgjwhj.cn

[T54] Scala：集合映射
来源：http://ys.szsharing.cn

List(1, 2, 3).map(_ * 2)
来源：http://cg.szxytkj.cn

[T55] Scala：集合过滤
来源：http://mp.bookmarksfly.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gm.asd995.cn

[T56] Scala：样例类
来源：http://br.huixinmuqiang.cn

case class User(name: String, age: Int)
来源：http://wt.gzmigu.cn

[T57] Scala：模式匹配
来源：http://uv.huanxung.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://xk.panjiajie.cn

[T58] Scala：函数定义
来源：http://yk.hnjuh.cn

def add(a: Int, b: Int): Int = a + b
来源：http://rb.hahajie.cn

[T59] Scala：循环
来源：http://xh.huixiangedu.cn

for (i <- 1 to 10) println(i)
来源：http://kq.hahajie.cn

[T60] Scala：折叠
来源：http://we.wgjwhj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wv.bjjhwx.cn

================================================================================
来源：http://wo.jctech888.com.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qm.haigaiapp.cn

================================================================================
来源：http://pr.szsharing.cn

[U01] Py：创建虚拟环境
来源：http://dq.haigaiapp.cn

python -m venv .venv && source .venv/bin/activate
来源：http://xw.jianghongdianzi.cn

[U02] Py：导出 / 安装依赖
来源：http://ts.colortex.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vy.asd995.cn

[U03] Py：加载 .env 配置
来源：http://hg.yuexingan06.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://hs.lnxyls.cn

[U04] Py：变量调试打印
来源：http://lr.bjjhwx.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ty.shxzukj.cn

[U05] Py：列表去重且保序
来源：http://uj.yuexingan06.cn

list(dict.fromkeys(arr))
来源：http://rt.jianghongdianzi.cn

[U06] Py：合并两个字典
来源：http://de.szxytkj.cn

{**a, **b}
来源：http://de.yuexingan06.cn

[U07] Py：反转字典键值
来源：http://ef.hahajie.cn

{v: k for k, v in d.items()}
来源：http://ky.newstarts.cn

[U08] Py：展平二维列表
来源：http://wy.haigaiapp.cn

[y for x in nested for y in x]
来源：http://ar.asd995.cn

[U09] Py：字典取最大值的键
来源：http://hz.jianghongdianzi.cn

max(d, key=d.get)
来源：http://et.hahajie.cn

[U10] Py：按值排序字典
来源：http://xo.panjiajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bx.521024.cn

[U11] Py：生成器表达式
来源：http://ze.9csxet.cn

(x * 2 for x in arr)
来源：http://un.gzmigu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ih.hnjuh.cn

Counter(arr).most_common(3)
来源：http://kw.huixiangedu.cn

[U13] Py：固定长度队列
来源：http://ae.haigaiapp.cn

deque(maxlen=10)
来源：http://ah.gzmigu.cn

[U14] Py：分组收集到列表
来源：http://dz.shxzskj.cn

defaultdict(list)
来源：http://eu.muxihuayi.cn

[U15] Py：高精度计时
来源：http://fg.bjjhwx.cn

t = time.perf_counter()
来源：http://za.nszjky.cn

[U16] Py：命令行参数解析
来源：http://qr.9csxet.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kx.bookmarksfly.cn

[U17] Py：初始化日志
来源：http://sm.haigaiapp.cn

logging.basicConfig(level=logging.INFO)
来源：http://hr.lnxyls.cn

[U18] Py：预编译正则
来源：http://sm.yuexingan06.cn

pat = re.compile(r"\d+")
来源：http://dk.hahajie.cn

[U19] Py：正则替换带回调
来源：http://qe.gzmigu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nc.szxytkj.cn

[U20] Py：缓存函数结果
来源：http://si.nszjky.cn

@functools.lru_cache(maxsize=None)
来源：http://am.yuexingan06.cn

[U21] Py：自定义上下文管理器
来源：http://pq.521024.cn

@contextlib.contextmanager
来源：http://kn.9csxet.cn

[U22] Py：矩阵转置
来源：http://eg.colortex.cn

list(zip(*m))
来源：http://wv.yuexingan06.cn

[U23] Py：分块读取大文件
来源：http://bw.muxihuayi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://st.521024.cn

[U24] Py：路径操作
来源：http://tj.chemitech.net.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jn.shxzskj.cn

[U25] Py：CSV 按字典读
来源：http://fp.9csxet.cn

csv.DictReader(f)
来源：http://rv.newstarts.cn

[U26] Py：并发下载
来源：http://lw.hnjuh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yt.chemitech.net.cn

[U27] Py：异步 HTTP
来源：http://hn.shtwfgs.cn

aiohttp.ClientSession() 配合 async with
来源：http://gj.shxzskj.cn

[U28] Py：类型别名
来源：http://jl.nszjky.cn

UserId = int
来源：http://wk.9csxet.cn

[U29] Py：属性校验
来源：http://wv.bjjhwx.cn

@property 与 @x.setter 配合
来源：http://oj.jianghongdianzi.cn

[U30] Py：数据类
来源：http://dt.muxihuayi.cn

@dataclass(slots=True)
来源：http://uf.panjiajie.cn

[U31] Py：单测
来源：http://aj.chemitech.net.cn

python -m pytest -q
来源：http://gq.shxzukj.cn

[U32] Py：代码格式化
来源：http://ta.asd995.cn

ruff format . && ruff check --fix .
来源：http://sk.szxytkj.cn

[U33] Py：打包发布
来源：http://nf.hnjuh.cn

python -m build  （依赖 pyproject.toml）
来源：http://ct.muxihuayi.cn

[U34] Py：判断编码
来源：http://wo.shtwfgs.cn

chardet.detect(raw)
来源：http://ac.gzmigu.cn

[U35] Py：发送邮件
来源：http://gx.asd995.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://oc.nszjky.cn

[U36] Py：定时任务
来源：http://ff.szsharing.cn

schedule.every(10).minutes.do(job)
来源：http://uu.muxihuayi.cn

[U37] Py：读写 Excel
来源：http://rf.chemitech.net.cn

pandas.read_excel / DataFrame.to_excel
来源：http://hi.521024.cn

[U38] Py：获取脚本所在目录
来源：http://zw.521024.cn

Path(__file__).resolve().parent
来源：http://fx.gzmigu.cn

[U39] Py：判断是否在交互环境
来源：http://so.shxzskj.cn

sys.stdout.isatty()
来源：http://ui.yuexingan06.cn

[U40] Py：打印到标准错误
来源：http://zn.shtwfgs.cn

print("err", file=sys.stderr)
来源：http://wh.shxzskj.cn

[U41] PHP：初始化 Composer 项目
来源：http://kh.nszjky.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://yk.yuntaijiaju.cn

[U42] PHP：PSR-4 自动加载
来源：http://nx.yuntaijiaju.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fi.muxihuayi.cn

[U43] PHP：声明命名空间
来源：http://nk.huixinmuqiang.cn

namespace App\Http;
来源：http://ul.bookmarksfly.cn

[U44] PHP：开启严格类型
来源：http://lu.muxihuayi.cn

declare(strict_types=1);
来源：http://lq.shxzukj.cn

[U45] PHP：类型声明与返回类型
来源：http://iz.szsharing.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ub.chemitech.net.cn

[U46] PHP：可空类型
来源：http://pr.yuexingan06.cn

?string $name = null
来源：http://fr.haigaiapp.cn

[U47] PHP：联合类型
来源：http://lc.gzmigu.cn

int|string $id
来源：http://qj.huanxung.cn

[U48] PHP：纯枚举
来源：http://gb.colortex.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gk.colortex.cn

[U49] PHP：只读属性
来源：http://jd.panjiajie.cn

public readonly string $name
来源：http://xv.gzmigu.cn

[U50] PHP：构造器属性提升
来源：http://nc.huixinmuqiang.cn

public function __construct(private int $id) {}
来源：http://at.yuntaijiaju.cn

[U51] PHP：数组解构
来源：http://gq.jctech888.com.cn

[$a, $b] = $arr;
来源：http://zb.gzmigu.cn

[U52] PHP：箭头函数
来源：http://cy.colortex.cn

$double = fn($x) => $x * 2;
来源：http://ez.bjjhwx.cn

[U53] PHP：空合并运算符
来源：http://vw.newstarts.cn

$v = $a ?? $b ?? "default";
来源：http://ay.huanxung.cn

[U54] PHP：空安全调用
来源：http://qi.szxytkj.cn

$obj?->method()
来源：http://ij.nszjky.cn

[U55] PHP：match 表达式
来源：http://ae.jctech888.com.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wn.gzmigu.cn

[U56] PHP：命名参数
来源：http://ui.shxzukj.cn

f(a: 1, b: 2)
来源：http://lj.huixiangedu.cn

[U57] PHP：字符串插值
来源：http://ba.panjiajie.cn

"值: {$a}"
来源：http://mb.jianghongdianzi.cn

[U58] PHP：数组三件套
来源：http://pq.asd995.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ek.wgjwhj.cn

[U59] PHP：自定义排序
来源：http://lz.huixinmuqiang.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ea.lnxyls.cn

[U60] PHP：JSON 编解码
来源：http://aj.wgjwhj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://de.jctech888.com.cn

[U61] PHP：正则
来源：http://vb.colortex.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yw.521024.cn

[U62] PHP：日期对象
来源：http://kw.huixiangedu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jf.shxzskj.cn

[U63] PHP：文件读写
来源：http://vk.muxihuayi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ay.gzmigu.cn

[U64] PHP：目录遍历
来源：http://ak.shtwfgs.cn

glob("dir/*.php");  scandir("dir");
来源：http://sc.gzmigu.cn

[U65] PHP：会话
来源：http://so.szxytkj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ue.yuntaijiaju.cn

[U66] PHP：设置 Cookie
来源：http://so.jianghongdianzi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nt.huixiangedu.cn


<!-- 参考信息 -->