代发 wailian999

[S45] C++：lambda
来源：http://ko.panjiajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://le.shxzukj.cn

[S46] C++：函数模板
来源：http://wh.newstarts.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rb.panjiajie.cn

[S47] C++：结构化绑定遍历
来源：http://jd.huanxung.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://in.yuexingan06.cn

[S48] C++：逐行读文件
来源：http://yo.wgjwhj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pc.yuexingan06.cn

while (std::getline(in, line)) { }
来源：http://mi.shxzskj.cn

[S49] C++：写文件
来源：http://bd.bjjhwx.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ln.huixiangedu.cn

[S50] C++：格式化数字
来源：http://nv.szxytkj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mh.shxzukj.cn

[S51] C++：显式类型转换
来源：http://ew.wgjwhj.cn

static_cast<double>(a) / b
来源：http://et.nicolike.cn

[S52] C++：const 与 noexcept
来源：http://vy.gzmigu.cn

int size() const noexcept { return n_; }
来源：http://lm.hahajie.cn

[S53] C++：移动语义
来源：http://oc.huanxung.cn

std::vector<int> w = std::move(v);
来源：http://gk.asd995.cn

[S54] C++：异常处理
来源：http://wg.hnjuh.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vt.9csxet.cn

[S55] C++：结构化绑定
来源：http://jx.haigaiapp.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://yc.huixiangedu.cn

[S56] C++：optional
来源：http://oj.yuexingan06.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zm.gzmigu.cn

[S57] C++：编译期常量
来源：http://gj.wgjwhj.cn

constexpr int N = 10;
来源：http://ol.hnjuh.cn

[S58] C++：命名空间
来源：http://eo.yuntaijiaju.cn

namespace ns { int f() { return 1; } }
来源：http://aq.shtwfgs.cn

[S59] C++：静态断言
来源：http://dv.bjjhwx.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://un.nicolike.cn

[S60] C++：遍历并删除元素
来源：http://op.lnxyls.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mc.bjjhwx.cn

================================================================================
来源：http://ul.haigaiapp.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ks.jianghongdianzi.cn

================================================================================
来源：http://ar.nszjky.cn

[T01] Kotlin：Hello World
来源：http://wx.newstarts.cn

println("Hello")
来源：http://gg.haigaiapp.cn

[T02] Kotlin：变量
来源：http://dm.asd995.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yr.huanxung.cn

[T03] Kotlin：字符串模板
来源：http://ru.huanxung.cn

"值: $b"
来源：http://vu.hahajie.cn

[T04] Kotlin：空安全
来源：http://td.colortex.cn

val n: String? = null;  n?.length
来源：http://xb.huixiangedu.cn

[T05] Kotlin：when 表达式
来源：http://wm.521024.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bz.huanxung.cn

[T06] Kotlin：集合映射
来源：http://ji.yuexingan06.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fo.hahajie.cn

[T07] Kotlin：集合过滤
来源：http://li.szxytkj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://sn.bookmarksfly.cn

[T08] Kotlin：数据类
来源：http://if.huanxung.cn

data class User(val name: String, val age: Int)
来源：http://jx.szsharing.cn

[T09] Kotlin：扩展函数
来源：http://xn.9csxet.cn

fun String.exclaim() = this + "!"
来源：http://qy.bookmarksfly.cn

[T10] Kotlin：默认参数
来源：http://as.szsharing.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tx.muxihuayi.cn

[T11] Kotlin：协程
来源：http://ce.jctech888.com.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vs.lnxyls.cn

[T12] Kotlin：解构声明
来源：http://ef.huixinmuqiang.cn

val (a, b) = Pair(1, 2)
来源：http://yo.haigaiapp.cn

[T13] Kotlin：只读 Map
来源：http://xp.shtwfgs.cn

val m = mapOf("a" to 1)
来源：http://zm.yuexingan06.cn

[T14] Kotlin：循环
来源：http://mj.yuntaijiaju.cn

for (i in 1..10) println(i)
来源：http://aq.gzmigu.cn

[T15] Kotlin：接口
来源：http://pk.nicolike.cn

interface Shape { fun area(): Double }
来源：http://ky.bookmarksfly.cn

[T16] Swift：Hello World
来源：http://qs.nicolike.cn

print("Hello")
来源：http://dq.521024.cn

[T17] Swift：变量与常量
来源：http://mw.huanxung.cn

var a = 1;  let b = 2
来源：http://sh.huanxung.cn

[T18] Swift：字符串插值
来源：http://id.gzmigu.cn

"值: \(b)"
来源：http://hs.yuntaijiaju.cn

[T19] Swift：可选绑定
来源：http://hx.huixinmuqiang.cn

if let n = opt { print(n) }
来源：http://oh.wgjwhj.cn

[T20] Swift：数组操作
来源：http://xa.chemitech.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zj.lnxyls.cn

[T21] Swift：遍历
来源：http://ev.hnjuh.cn

for x in a { print(x) }
来源：http://ov.huanxung.cn

[T22] Swift：字典
来源：http://hz.yuntaijiaju.cn

var d = ["a": 1];  d["b"] = 2
来源：http://tm.bjjhwx.cn

[T23] Swift：函数
来源：http://hy.nszjky.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kd.lnxyls.cn

[T24] Swift：闭包
来源：http://tp.huanxung.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qj.panjiajie.cn

[T25] Swift：结构体
来源：http://tx.hnjuh.cn

struct P { var x: Int }
来源：http://qw.hnjuh.cn

[T26] Swift：类与重写
来源：http://cy.wgjwhj.cn

class A: Base { override func f() {} }
来源：http://nz.asd995.cn

[T27] Swift：错误处理
来源：http://fg.newstarts.cn

do { try f() } catch { print(error) }
来源：http://rx.yuexingan06.cn

[T28] Swift：枚举
来源：http://cf.hahajie.cn

enum Color { case red, green }
来源：http://lj.chemitech.net.cn

[T29] Swift：guard 提前返回
来源：http://dr.nszjky.cn

guard let x = opt else { return }
来源：http://my.yuntaijiaju.cn

[T30] Swift：协议
来源：http://ml.nicolike.cn

protocol Shape { func area() -> Double }
来源：http://fa.haigaiapp.cn

[T31] Lua：Hello World
来源：http://ob.huixiangedu.cn

print("Hello")
来源：http://fu.nszjky.cn

[T32] Lua：局部变量
来源：http://wp.hnjuh.cn

local a = 1
来源：http://rx.huixiangedu.cn

[T33] Lua：表（数组）
来源：http://za.gzmigu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://lu.colortex.cn

[T34] Lua：遍历表
来源：http://pd.hnjuh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ma.hahajie.cn

[T35] Lua：字典表
来源：http://op.bjjhwx.cn

local d = { a = 1 };  d.b = 2
来源：http://hc.wgjwhj.cn

[T36] Lua：函数
来源：http://ft.hahajie.cn

function add(a, b) return a + b end
来源：http://qa.jctech888.com.cn

[T37] Lua：字符串拼接
来源：http://vf.huixinmuqiang.cn

"a" .. "b"
来源：http://da.panjiajie.cn

[T38] Lua：条件
来源：http://nl.huixinmuqiang.cn

if x > 0 then print("正") end
来源：http://cw.muxihuayi.cn

[T39] Lua：模式匹配
来源：http://lo.521024.cn

string.find(s, "%d+")
来源：http://zo.521024.cn

[T40] Lua：元表
来源：http://gk.yuntaijiaju.cn

setmetatable({}, { __index = base })
来源：http://tp.hnjuh.cn

[T41] Perl：Hello World
来源：http://in.asd995.cn

print "Hello\n";
来源：http://zi.muxihuayi.cn

[T42] Perl：变量类型
来源：http://hy.lnxyls.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sf.muxihuayi.cn

[T43] Perl：字符串插值
来源：http://wn.szxytkj.cn

"值: $a"
来源：http://mz.9csxet.cn

[T44] Perl：条件
来源：http://uu.huixiangedu.cn

if ($a > 0) { print "正"; }
来源：http://rr.bookmarksfly.cn

[T45] Perl：数组遍历
来源：http://eo.newstarts.cn

for my $x (@arr) { print $x; }
来源：http://ca.jctech888.com.cn

[T46] Perl：哈希操作
来源：http://tz.asd995.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ty.hnjuh.cn

[T47] Perl：正则捕获
来源：http://ft.huixiangedu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ci.panjiajie.cn

[T48] Perl：正则替换
来源：http://rp.bookmarksfly.cn

$s =~ s/old/new/g;
来源：http://em.muxihuayi.cn

[T49] Perl：函数
来源：http://fm.jianghongdianzi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zu.szxytkj.cn

[T50] Perl：逐行读文件
来源：http://lr.haigaiapp.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://kw.nicolike.cn

while (my $line = <$fh>) { print $line; }
来源：http://jq.szsharing.cn

[T51] Scala：Hello World
来源：http://za.shxzskj.cn

println("Hello")
来源：http://ai.nicolike.cn

[T52] Scala：变量
来源：http://aw.gzmigu.cn

val a = 1;  var b = 2
来源：http://mj.hnjuh.cn

[T53] Scala：字符串插值
来源：http://dp.gzmigu.cn

s"值: $b"
来源：http://td.yuntaijiaju.cn

[T54] Scala：集合映射
来源：http://hv.chemitech.net.cn

List(1, 2, 3).map(_ * 2)
来源：http://bs.colortex.cn

[T55] Scala：集合过滤
来源：http://bv.szxytkj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xw.huixinmuqiang.cn

[T56] Scala：样例类
来源：http://yl.haigaiapp.cn

case class User(name: String, age: Int)
来源：http://ai.haigaiapp.cn

[T57] Scala：模式匹配
来源：http://yd.lnxyls.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://hr.yuntaijiaju.cn

[T58] Scala：函数定义
来源：http://am.521024.cn

def add(a: Int, b: Int): Int = a + b
来源：http://eo.wgjwhj.cn

[T59] Scala：循环
来源：http://th.haigaiapp.cn

for (i <- 1 to 10) println(i)
来源：http://wy.shxzukj.cn

[T60] Scala：折叠
来源：http://hu.szsharing.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ms.gzmigu.cn

================================================================================
来源：http://ju.yuexingan06.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xv.szxytkj.cn

================================================================================
来源：http://xj.shxzskj.cn

[U01] Py：创建虚拟环境
来源：http://bt.hahajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://oq.521024.cn

[U02] Py：导出 / 安装依赖
来源：http://da.shxzskj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://db.521024.cn

[U03] Py：加载 .env 配置
来源：http://vn.jctech888.com.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qv.shxzukj.cn

[U04] Py：变量调试打印
来源：http://jt.yuntaijiaju.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://oj.wgjwhj.cn

[U05] Py：列表去重且保序
来源：http://ej.huixinmuqiang.cn

list(dict.fromkeys(arr))
来源：http://vu.muxihuayi.cn

[U06] Py：合并两个字典
来源：http://xc.gzmigu.cn

{**a, **b}
来源：http://av.jctech888.com.cn

[U07] Py：反转字典键值
来源：http://fx.newstarts.cn

{v: k for k, v in d.items()}
来源：http://jv.gzmigu.cn

[U08] Py：展平二维列表
来源：http://wh.yuexingan06.cn

[y for x in nested for y in x]
来源：http://by.9csxet.cn

[U09] Py：字典取最大值的键
来源：http://xi.haigaiapp.cn

max(d, key=d.get)
来源：http://ij.wgjwhj.cn

[U10] Py：按值排序字典
来源：http://qr.bjjhwx.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lo.9csxet.cn

[U11] Py：生成器表达式
来源：http://yo.yuexingan06.cn

(x * 2 for x in arr)
来源：http://sw.huixiangedu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://fh.hahajie.cn

Counter(arr).most_common(3)
来源：http://ny.nszjky.cn

[U13] Py：固定长度队列
来源：http://df.szxytkj.cn

deque(maxlen=10)
来源：http://hr.panjiajie.cn

[U14] Py：分组收集到列表
来源：http://tp.shxzukj.cn

defaultdict(list)
来源：http://wy.9csxet.cn

[U15] Py：高精度计时
来源：http://kg.muxihuayi.cn

t = time.perf_counter()
来源：http://ye.shtwfgs.cn

[U16] Py：命令行参数解析
来源：http://jy.shxzskj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yh.lnxyls.cn

[U17] Py：初始化日志
来源：http://jt.shxzskj.cn

logging.basicConfig(level=logging.INFO)
来源：http://sq.yuexingan06.cn

[U18] Py：预编译正则
来源：http://ty.hnjuh.cn

pat = re.compile(r"\d+")
来源：http://tc.huixiangedu.cn

[U19] Py：正则替换带回调
来源：http://yk.hahajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zr.asd995.cn

[U20] Py：缓存函数结果
来源：http://fn.bjjhwx.cn

@functools.lru_cache(maxsize=None)
来源：http://in.gzmigu.cn

[U21] Py：自定义上下文管理器
来源：http://ch.jctech888.com.cn

@contextlib.contextmanager
来源：http://ny.gzmigu.cn

[U22] Py：矩阵转置
来源：http://jw.huixinmuqiang.cn

list(zip(*m))
来源：http://zu.panjiajie.cn

[U23] Py：分块读取大文件
来源：http://pr.yuexingan06.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yh.newstarts.cn

[U24] Py：路径操作
来源：http://pn.yuexingan06.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ep.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://mz.szsharing.cn

csv.DictReader(f)
来源：http://be.huixiangedu.cn

[U26] Py：并发下载
来源：http://ci.jctech888.com.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://da.panjiajie.cn

[U27] Py：异步 HTTP
来源：http://ln.muxihuayi.cn

aiohttp.ClientSession() 配合 async with
来源：http://zo.yuntaijiaju.cn

[U28] Py：类型别名
来源：http://fw.szxytkj.cn

UserId = int
来源：http://ci.shxzskj.cn

[U29] Py：属性校验
来源：http://bi.hahajie.cn

@property 与 @x.setter 配合
来源：http://bx.gzmigu.cn

[U30] Py：数据类
来源：http://qn.jianghongdianzi.cn

@dataclass(slots=True)
来源：http://fv.521024.cn

[U31] Py：单测
来源：http://fj.hahajie.cn

python -m pytest -q
来源：http://ub.hahajie.cn

[U32] Py：代码格式化
来源：http://oe.521024.cn

ruff format . && ruff check --fix .
来源：http://um.nicolike.cn

[U33] Py：打包发布
来源：http://lk.9csxet.cn

python -m build  （依赖 pyproject.toml）
来源：http://br.muxihuayi.cn

[U34] Py：判断编码
来源：http://su.bjjhwx.cn

chardet.detect(raw)
来源：http://vz.9csxet.cn

[U35] Py：发送邮件
来源：http://we.bjjhwx.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://uk.hahajie.cn

[U36] Py：定时任务
来源：http://mh.gzmigu.cn

schedule.every(10).minutes.do(job)
来源：http://cw.wgjwhj.cn

[U37] Py：读写 Excel
来源：http://rr.newstarts.cn

pandas.read_excel / DataFrame.to_excel
来源：http://gv.wgjwhj.cn

[U38] Py：获取脚本所在目录
来源：http://wb.huixiangedu.cn

Path(__file__).resolve().parent
来源：http://qz.jianghongdianzi.cn

[U39] Py：判断是否在交互环境
来源：http://om.yuexingan06.cn

sys.stdout.isatty()
来源：http://nq.shtwfgs.cn

[U40] Py：打印到标准错误
来源：http://kj.huixinmuqiang.cn

print("err", file=sys.stderr)
来源：http://xr.shxzskj.cn

[U41] PHP：初始化 Composer 项目
来源：http://ok.521024.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xc.panjiajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://ld.shxzukj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://oo.shxzskj.cn

[U43] PHP：声明命名空间
来源：http://kc.hahajie.cn

namespace App\Http;
来源：http://nz.newstarts.cn

[U44] PHP：开启严格类型
来源：http://in.panjiajie.cn

declare(strict_types=1);
来源：http://rt.gzmigu.cn

[U45] PHP：类型声明与返回类型
来源：http://xt.newstarts.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ny.hnjuh.cn

[U46] PHP：可空类型
来源：http://qx.yuexingan06.cn

?string $name = null
来源：http://gx.bjjhwx.cn

[U47] PHP：联合类型
来源：http://gc.huixinmuqiang.cn

int|string $id
来源：http://gg.muxihuayi.cn

[U48] PHP：纯枚举
来源：http://qf.gzmigu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mo.huanxung.cn

[U49] PHP：只读属性
来源：http://xy.lnxyls.cn

public readonly string $name
来源：http://io.jianghongdianzi.cn

[U50] PHP：构造器属性提升
来源：http://qw.szsharing.cn

public function __construct(private int $id) {}
来源：http://nq.nicolike.cn

[U51] PHP：数组解构
来源：http://xj.bookmarksfly.cn

[$a, $b] = $arr;
来源：http://nd.lnxyls.cn

[U52] PHP：箭头函数
来源：http://vm.colortex.cn

$double = fn($x) => $x * 2;
来源：http://cn.hahajie.cn

[U53] PHP：空合并运算符
来源：http://uj.huanxung.cn

$v = $a ?? $b ?? "default";
来源：http://ji.jctech888.com.cn

[U54] PHP：空安全调用
来源：http://ba.asd995.cn

$obj?->method()
来源：http://wx.newstarts.cn

[U55] PHP：match 表达式
来源：http://hz.asd995.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vb.huixinmuqiang.cn

[U56] PHP：命名参数
来源：http://pq.muxihuayi.cn

f(a: 1, b: 2)
来源：http://af.colortex.cn

[U57] PHP：字符串插值
来源：http://hq.shxzskj.cn

"值: {$a}"
来源：http://pu.gzmigu.cn

[U58] PHP：数组三件套
来源：http://mw.9csxet.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vn.nszjky.cn

[U59] PHP：自定义排序
来源：http://xk.521024.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mv.huixinmuqiang.cn

[U60] PHP：JSON 编解码
来源：http://oz.szsharing.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lv.szsharing.cn

[U61] PHP：正则
来源：http://yr.huixiangedu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lr.shxzukj.cn

[U62] PHP：日期对象
来源：http://si.bjjhwx.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dw.lnxyls.cn

[U63] PHP：文件读写
来源：http://cd.colortex.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gs.asd995.cn

[U64] PHP：目录遍历
来源：http://rk.gzmigu.cn

glob("dir/*.php");  scandir("dir");
来源：http://fs.521024.cn

[U65] PHP：会话
来源：http://uo.gzmigu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://sv.shxzskj.cn

[U66] PHP：设置 Cookie
来源：http://jd.yuntaijiaju.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jk.szxytkj.cn

[U67] PHP：处理文件上传
来源：http://nl.bjjhwx.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://it.huixinmuqiang.cn

[U68] PHP：PDO 连接
来源：http://fs.bjjhwx.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qs.gzmigu.cn

[U69] PHP：PDO 预处理
来源：http://px.szxytkj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ox.szsharing.cn

[U70] PHP：PDO 事务
来源：http://pc.chemitech.net.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cl.gzmigu.cn


<!-- 参考信息 -->