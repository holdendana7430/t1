代发 wailian999

[S45] C++：lambda
来源：http://tn.9csxet.cn

auto add = [](int a, int b) { return a + b; };
来源：http://eb.bookmarksfly.cn

[S46] C++：函数模板
来源：http://ps.nicolike.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ro.wgjwhj.cn

[S47] C++：结构化绑定遍历
来源：http://xt.521024.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jp.nszjky.cn

[S48] C++：逐行读文件
来源：http://vr.shxzukj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://tf.yuexingan06.cn

while (std::getline(in, line)) { }
来源：http://rh.haigaiapp.cn

[S49] C++：写文件
来源：http://ht.jctech888.com.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pg.shtwfgs.cn

[S50] C++：格式化数字
来源：http://fc.nszjky.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rp.szxytkj.cn

[S51] C++：显式类型转换
来源：http://fn.muxihuayi.cn

static_cast<double>(a) / b
来源：http://ie.colortex.cn

[S52] C++：const 与 noexcept
来源：http://am.shxzskj.cn

int size() const noexcept { return n_; }
来源：http://bk.newstarts.cn

[S53] C++：移动语义
来源：http://cf.muxihuayi.cn

std::vector<int> w = std::move(v);
来源：http://zj.chemitech.net.cn

[S54] C++：异常处理
来源：http://jj.huixinmuqiang.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://io.shxzukj.cn

[S55] C++：结构化绑定
来源：http://yx.nicolike.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ly.lnxyls.cn

[S56] C++：optional
来源：http://dz.asd995.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pl.yuntaijiaju.cn

[S57] C++：编译期常量
来源：http://to.haigaiapp.cn

constexpr int N = 10;
来源：http://on.shxzukj.cn

[S58] C++：命名空间
来源：http://we.asd995.cn

namespace ns { int f() { return 1; } }
来源：http://pl.hnjuh.cn

[S59] C++：静态断言
来源：http://yx.szsharing.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tl.asd995.cn

[S60] C++：遍历并删除元素
来源：http://yo.newstarts.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://st.asd995.cn

================================================================================
来源：http://vg.hahajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://iz.yuexingan06.cn

================================================================================
来源：http://hs.521024.cn

[T01] Kotlin：Hello World
来源：http://wd.muxihuayi.cn

println("Hello")
来源：http://rt.yuexingan06.cn

[T02] Kotlin：变量
来源：http://id.lnxyls.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rx.huanxung.cn

[T03] Kotlin：字符串模板
来源：http://am.521024.cn

"值: $b"
来源：http://vi.521024.cn

[T04] Kotlin：空安全
来源：http://pk.gzmigu.cn

val n: String? = null;  n?.length
来源：http://jh.nicolike.cn

[T05] Kotlin：when 表达式
来源：http://oe.gzmigu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://li.chemitech.net.cn

[T06] Kotlin：集合映射
来源：http://ni.lnxyls.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://mo.chemitech.net.cn

[T07] Kotlin：集合过滤
来源：http://vi.chemitech.net.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://nc.9csxet.cn

[T08] Kotlin：数据类
来源：http://dx.shxzskj.cn

data class User(val name: String, val age: Int)
来源：http://vk.521024.cn

[T09] Kotlin：扩展函数
来源：http://bd.asd995.cn

fun String.exclaim() = this + "!"
来源：http://fv.asd995.cn

[T10] Kotlin：默认参数
来源：http://zn.szsharing.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pz.huixiangedu.cn

[T11] Kotlin：协程
来源：http://se.huixiangedu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://pa.huanxung.cn

[T12] Kotlin：解构声明
来源：http://wh.huanxung.cn

val (a, b) = Pair(1, 2)
来源：http://bc.bjjhwx.cn

[T13] Kotlin：只读 Map
来源：http://rk.nszjky.cn

val m = mapOf("a" to 1)
来源：http://ou.muxihuayi.cn

[T14] Kotlin：循环
来源：http://uo.haigaiapp.cn

for (i in 1..10) println(i)
来源：http://xa.nicolike.cn

[T15] Kotlin：接口
来源：http://hm.colortex.cn

interface Shape { fun area(): Double }
来源：http://sh.haigaiapp.cn

[T16] Swift：Hello World
来源：http://ll.newstarts.cn

print("Hello")
来源：http://ek.colortex.cn

[T17] Swift：变量与常量
来源：http://ju.521024.cn

var a = 1;  let b = 2
来源：http://yr.huanxung.cn

[T18] Swift：字符串插值
来源：http://nu.9csxet.cn

"值: \(b)"
来源：http://ou.bookmarksfly.cn

[T19] Swift：可选绑定
来源：http://ba.shxzukj.cn

if let n = opt { print(n) }
来源：http://gq.newstarts.cn

[T20] Swift：数组操作
来源：http://qw.huanxung.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mm.521024.cn

[T21] Swift：遍历
来源：http://sg.jianghongdianzi.cn

for x in a { print(x) }
来源：http://ft.lnxyls.cn

[T22] Swift：字典
来源：http://us.panjiajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://bx.lnxyls.cn

[T23] Swift：函数
来源：http://fj.bjjhwx.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dd.huixiangedu.cn

[T24] Swift：闭包
来源：http://yx.jianghongdianzi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://pq.lnxyls.cn

[T25] Swift：结构体
来源：http://ad.gzmigu.cn

struct P { var x: Int }
来源：http://rw.panjiajie.cn

[T26] Swift：类与重写
来源：http://sy.521024.cn

class A: Base { override func f() {} }
来源：http://mt.asd995.cn

[T27] Swift：错误处理
来源：http://qv.shxzukj.cn

do { try f() } catch { print(error) }
来源：http://us.asd995.cn

[T28] Swift：枚举
来源：http://rg.521024.cn

enum Color { case red, green }
来源：http://dc.9csxet.cn

[T29] Swift：guard 提前返回
来源：http://gm.hahajie.cn

guard let x = opt else { return }
来源：http://do.asd995.cn

[T30] Swift：协议
来源：http://po.521024.cn

protocol Shape { func area() -> Double }
来源：http://jc.chemitech.net.cn

[T31] Lua：Hello World
来源：http://uk.lnxyls.cn

print("Hello")
来源：http://bc.chemitech.net.cn

[T32] Lua：局部变量
来源：http://mm.huixinmuqiang.cn

local a = 1
来源：http://lf.521024.cn

[T33] Lua：表（数组）
来源：http://fo.muxihuayi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xp.huanxung.cn

[T34] Lua：遍历表
来源：http://ny.huixinmuqiang.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://me.szxytkj.cn

[T35] Lua：字典表
来源：http://kt.lnxyls.cn

local d = { a = 1 };  d.b = 2
来源：http://zp.szxytkj.cn

[T36] Lua：函数
来源：http://ga.muxihuayi.cn

function add(a, b) return a + b end
来源：http://ft.huixiangedu.cn

[T37] Lua：字符串拼接
来源：http://df.szxytkj.cn

"a" .. "b"
来源：http://ou.hahajie.cn

[T38] Lua：条件
来源：http://iy.jianghongdianzi.cn

if x > 0 then print("正") end
来源：http://pu.wgjwhj.cn

[T39] Lua：模式匹配
来源：http://au.huixiangedu.cn

string.find(s, "%d+")
来源：http://ga.shtwfgs.cn

[T40] Lua：元表
来源：http://hx.colortex.cn

setmetatable({}, { __index = base })
来源：http://ag.lnxyls.cn

[T41] Perl：Hello World
来源：http://lx.9csxet.cn

print "Hello\n";
来源：http://tu.lnxyls.cn

[T42] Perl：变量类型
来源：http://jl.newstarts.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sq.shtwfgs.cn

[T43] Perl：字符串插值
来源：http://cj.haigaiapp.cn

"值: $a"
来源：http://je.asd995.cn

[T44] Perl：条件
来源：http://sf.hnjuh.cn

if ($a > 0) { print "正"; }
来源：http://qh.jianghongdianzi.cn

[T45] Perl：数组遍历
来源：http://sp.shtwfgs.cn

for my $x (@arr) { print $x; }
来源：http://tw.521024.cn

[T46] Perl：哈希操作
来源：http://yi.jianghongdianzi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pf.hahajie.cn

[T47] Perl：正则捕获
来源：http://qf.lnxyls.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://tb.newstarts.cn

[T48] Perl：正则替换
来源：http://jl.shxzukj.cn

$s =~ s/old/new/g;
来源：http://ex.bookmarksfly.cn

[T49] Perl：函数
来源：http://hl.lnxyls.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sa.yuexingan06.cn

[T50] Perl：逐行读文件
来源：http://fv.jctech888.com.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://gl.nszjky.cn

while (my $line = <$fh>) { print $line; }
来源：http://aq.bookmarksfly.cn

[T51] Scala：Hello World
来源：http://rt.521024.cn

println("Hello")
来源：http://nd.jctech888.com.cn

[T52] Scala：变量
来源：http://cp.bjjhwx.cn

val a = 1;  var b = 2
来源：http://tg.jctech888.com.cn

[T53] Scala：字符串插值
来源：http://jm.jctech888.com.cn

s"值: $b"
来源：http://wy.nicolike.cn

[T54] Scala：集合映射
来源：http://nr.gzmigu.cn

List(1, 2, 3).map(_ * 2)
来源：http://vf.shxzukj.cn

[T55] Scala：集合过滤
来源：http://iv.muxihuayi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://sc.yuntaijiaju.cn

[T56] Scala：样例类
来源：http://gp.lnxyls.cn

case class User(name: String, age: Int)
来源：http://fx.521024.cn

[T57] Scala：模式匹配
来源：http://rk.nszjky.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://rb.haigaiapp.cn

[T58] Scala：函数定义
来源：http://nj.bjjhwx.cn

def add(a: Int, b: Int): Int = a + b
来源：http://nc.newstarts.cn

[T59] Scala：循环
来源：http://fe.hnjuh.cn

for (i <- 1 to 10) println(i)
来源：http://gl.hnjuh.cn

[T60] Scala：折叠
来源：http://jw.gzmigu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mi.yuntaijiaju.cn

================================================================================
来源：http://je.jctech888.com.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mf.wgjwhj.cn

================================================================================
来源：http://pt.haigaiapp.cn

[U01] Py：创建虚拟环境
来源：http://lc.yuntaijiaju.cn

python -m venv .venv && source .venv/bin/activate
来源：http://pm.huixiangedu.cn

[U02] Py：导出 / 安装依赖
来源：http://mk.lnxyls.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qt.newstarts.cn

[U03] Py：加载 .env 配置
来源：http://qp.muxihuayi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wc.newstarts.cn

[U04] Py：变量调试打印
来源：http://pp.bjjhwx.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ce.asd995.cn

[U05] Py：列表去重且保序
来源：http://ny.nszjky.cn

list(dict.fromkeys(arr))
来源：http://lo.yuexingan06.cn

[U06] Py：合并两个字典
来源：http://jb.jianghongdianzi.cn

{**a, **b}
来源：http://mu.yuexingan06.cn

[U07] Py：反转字典键值
来源：http://nf.hnjuh.cn

{v: k for k, v in d.items()}
来源：http://qb.nszjky.cn

[U08] Py：展平二维列表
来源：http://ij.shtwfgs.cn

[y for x in nested for y in x]
来源：http://xk.szsharing.cn

[U09] Py：字典取最大值的键
来源：http://qu.shtwfgs.cn

max(d, key=d.get)
来源：http://ea.shtwfgs.cn

[U10] Py：按值排序字典
来源：http://js.gzmigu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lr.bjjhwx.cn

[U11] Py：生成器表达式
来源：http://mq.yuntaijiaju.cn

(x * 2 for x in arr)
来源：http://xl.haigaiapp.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rr.huixiangedu.cn

Counter(arr).most_common(3)
来源：http://ba.szxytkj.cn

[U13] Py：固定长度队列
来源：http://ur.szxytkj.cn

deque(maxlen=10)
来源：http://oo.huixiangedu.cn

[U14] Py：分组收集到列表
来源：http://cv.huixinmuqiang.cn

defaultdict(list)
来源：http://kd.bjjhwx.cn

[U15] Py：高精度计时
来源：http://nw.huanxung.cn

t = time.perf_counter()
来源：http://rj.asd995.cn

[U16] Py：命令行参数解析
来源：http://eb.521024.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qs.asd995.cn

[U17] Py：初始化日志
来源：http://xq.chemitech.net.cn

logging.basicConfig(level=logging.INFO)
来源：http://di.huixinmuqiang.cn

[U18] Py：预编译正则
来源：http://dk.huanxung.cn

pat = re.compile(r"\d+")
来源：http://sy.9csxet.cn

[U19] Py：正则替换带回调
来源：http://yg.shtwfgs.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ij.gzmigu.cn

[U20] Py：缓存函数结果
来源：http://jy.szxytkj.cn

@functools.lru_cache(maxsize=None)
来源：http://wt.nicolike.cn

[U21] Py：自定义上下文管理器
来源：http://nl.huanxung.cn

@contextlib.contextmanager
来源：http://au.colortex.cn

[U22] Py：矩阵转置
来源：http://js.newstarts.cn

list(zip(*m))
来源：http://ne.haigaiapp.cn

[U23] Py：分块读取大文件
来源：http://py.chemitech.net.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wy.wgjwhj.cn

[U24] Py：路径操作
来源：http://eh.jianghongdianzi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yh.asd995.cn

[U25] Py：CSV 按字典读
来源：http://jr.muxihuayi.cn

csv.DictReader(f)
来源：http://tg.jctech888.com.cn

[U26] Py：并发下载
来源：http://hc.hnjuh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pc.szsharing.cn

[U27] Py：异步 HTTP
来源：http://oc.bookmarksfly.cn

aiohttp.ClientSession() 配合 async with
来源：http://jf.bookmarksfly.cn

[U28] Py：类型别名
来源：http://yv.jctech888.com.cn

UserId = int
来源：http://sv.gzmigu.cn

[U29] Py：属性校验
来源：http://qr.nszjky.cn

@property 与 @x.setter 配合
来源：http://zh.hahajie.cn

[U30] Py：数据类
来源：http://rv.wgjwhj.cn

@dataclass(slots=True)
来源：http://cl.shtwfgs.cn

[U31] Py：单测
来源：http://zu.shxzukj.cn

python -m pytest -q
来源：http://hg.szsharing.cn

[U32] Py：代码格式化
来源：http://vr.panjiajie.cn

ruff format . && ruff check --fix .
来源：http://wq.huixiangedu.cn

[U33] Py：打包发布
来源：http://zg.newstarts.cn

python -m build  （依赖 pyproject.toml）
来源：http://gh.asd995.cn

[U34] Py：判断编码
来源：http://aw.asd995.cn

chardet.detect(raw)
来源：http://zk.bjjhwx.cn

[U35] Py：发送邮件
来源：http://tw.newstarts.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ws.jianghongdianzi.cn

[U36] Py：定时任务
来源：http://ks.wgjwhj.cn

schedule.every(10).minutes.do(job)
来源：http://eq.hnjuh.cn

[U37] Py：读写 Excel
来源：http://ui.lnxyls.cn

pandas.read_excel / DataFrame.to_excel
来源：http://yj.chemitech.net.cn

[U38] Py：获取脚本所在目录
来源：http://ug.shtwfgs.cn

Path(__file__).resolve().parent
来源：http://ry.szxytkj.cn

[U39] Py：判断是否在交互环境
来源：http://wx.yuntaijiaju.cn

sys.stdout.isatty()
来源：http://qz.521024.cn

[U40] Py：打印到标准错误
来源：http://ae.szxytkj.cn

print("err", file=sys.stderr)
来源：http://hm.newstarts.cn

[U41] PHP：初始化 Composer 项目
来源：http://eu.shxzskj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://at.bookmarksfly.cn

[U42] PHP：PSR-4 自动加载
来源：http://ce.huanxung.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tk.shxzukj.cn

[U43] PHP：声明命名空间
来源：http://fz.jctech888.com.cn

namespace App\Http;
来源：http://lv.jianghongdianzi.cn

[U44] PHP：开启严格类型
来源：http://yq.hnjuh.cn

declare(strict_types=1);
来源：http://km.shxzukj.cn

[U45] PHP：类型声明与返回类型
来源：http://hw.nicolike.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://wn.nicolike.cn

[U46] PHP：可空类型
来源：http://ew.huixinmuqiang.cn

?string $name = null
来源：http://wa.wgjwhj.cn

[U47] PHP：联合类型
来源：http://ho.jianghongdianzi.cn

int|string $id
来源：http://iy.9csxet.cn

[U48] PHP：纯枚举
来源：http://oz.shxzskj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ep.huixiangedu.cn

[U49] PHP：只读属性
来源：http://bj.yuexingan06.cn

public readonly string $name
来源：http://jx.lnxyls.cn

[U50] PHP：构造器属性提升
来源：http://mp.bjjhwx.cn

public function __construct(private int $id) {}
来源：http://ir.muxihuayi.cn

[U51] PHP：数组解构
来源：http://qs.yuexingan06.cn

[$a, $b] = $arr;
来源：http://fy.asd995.cn

[U52] PHP：箭头函数
来源：http://vf.shxzukj.cn

$double = fn($x) => $x * 2;
来源：http://ox.bookmarksfly.cn

[U53] PHP：空合并运算符
来源：http://za.muxihuayi.cn

$v = $a ?? $b ?? "default";
来源：http://wl.muxihuayi.cn

[U54] PHP：空安全调用
来源：http://iy.jctech888.com.cn

$obj?->method()
来源：http://yj.shxzukj.cn

[U55] PHP：match 表达式
来源：http://hl.panjiajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ym.huixiangedu.cn

[U56] PHP：命名参数
来源：http://ou.panjiajie.cn

f(a: 1, b: 2)
来源：http://km.huixiangedu.cn

[U57] PHP：字符串插值
来源：http://py.hnjuh.cn

"值: {$a}"
来源：http://qi.szxytkj.cn

[U58] PHP：数组三件套
来源：http://bq.bjjhwx.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://sd.asd995.cn

[U59] PHP：自定义排序
来源：http://zi.newstarts.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fq.szxytkj.cn

[U60] PHP：JSON 编解码
来源：http://xh.shtwfgs.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://an.shxzskj.cn

[U61] PHP：正则
来源：http://kk.panjiajie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bg.yuntaijiaju.cn

[U62] PHP：日期对象
来源：http://es.jianghongdianzi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ec.haigaiapp.cn

[U63] PHP：文件读写
来源：http://hb.szsharing.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zr.hahajie.cn

[U64] PHP：目录遍历
来源：http://kh.shxzukj.cn

glob("dir/*.php");  scandir("dir");
来源：http://fv.lnxyls.cn

[U65] PHP：会话
来源：http://dl.shxzskj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rh.huixinmuqiang.cn

[U66] PHP：设置 Cookie
来源：http://in.chemitech.net.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cl.shxzukj.cn

[U67] PHP：处理文件上传
来源：http://rl.hnjuh.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://np.jianghongdianzi.cn

[U68] PHP：PDO 连接
来源：http://va.gzmigu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://in.hahajie.cn

[U69] PHP：PDO 预处理
来源：http://nm.muxihuayi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://uw.newstarts.cn

[U70] PHP：PDO 事务
来源：http://za.hnjuh.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bl.bookmarksfly.cn


<!-- 参考信息 -->