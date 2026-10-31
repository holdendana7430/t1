代发 wailian999

[S43] C++：智能指针
来源：http://am.shtwfgs.cn

auto p = std::make_unique<int>(5);
来源：http://mu.szxytkj.cn

[S44] C++：引用传参
来源：http://lr.asd995.cn

void inc(int &x) { ++x; }
来源：http://rr.9csxet.cn

[S45] C++：lambda
来源：http://ns.panjiajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bq.huixinmuqiang.cn

[S46] C++：函数模板
来源：http://kz.jianghongdianzi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hn.huixiangedu.cn

[S47] C++：结构化绑定遍历
来源：http://ox.jctech888.com.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ks.bjjhwx.cn

[S48] C++：逐行读文件
来源：http://cl.huanxung.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fc.szsharing.cn

while (std::getline(in, line)) { }
来源：http://je.asd995.cn

[S49] C++：写文件
来源：http://bk.9csxet.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kj.yuexingan06.cn

[S50] C++：格式化数字
来源：http://ha.szsharing.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pg.wgjwhj.cn

[S51] C++：显式类型转换
来源：http://ae.yuexingan06.cn

static_cast<double>(a) / b
来源：http://az.wgjwhj.cn

[S52] C++：const 与 noexcept
来源：http://pc.panjiajie.cn

int size() const noexcept { return n_; }
来源：http://sn.shxzskj.cn

[S53] C++：移动语义
来源：http://ci.yuntaijiaju.cn

std::vector<int> w = std::move(v);
来源：http://dq.shxzukj.cn

[S54] C++：异常处理
来源：http://lb.huanxung.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zx.bjjhwx.cn

[S55] C++：结构化绑定
来源：http://tr.muxihuayi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jh.huixiangedu.cn

[S56] C++：optional
来源：http://om.nszjky.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yn.huanxung.cn

[S57] C++：编译期常量
来源：http://wt.szxytkj.cn

constexpr int N = 10;
来源：http://xr.huanxung.cn

[S58] C++：命名空间
来源：http://xv.521024.cn

namespace ns { int f() { return 1; } }
来源：http://zz.lnxyls.cn

[S59] C++：静态断言
来源：http://cm.hahajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hl.hnjuh.cn

[S60] C++：遍历并删除元素
来源：http://uu.chemitech.net.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wn.bookmarksfly.cn

================================================================================
来源：http://un.muxihuayi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gd.huixinmuqiang.cn

================================================================================
来源：http://en.shxzskj.cn

[T01] Kotlin：Hello World
来源：http://np.nicolike.cn

println("Hello")
来源：http://vs.jctech888.com.cn

[T02] Kotlin：变量
来源：http://ky.yuexingan06.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kd.nicolike.cn

[T03] Kotlin：字符串模板
来源：http://xp.asd995.cn

"值: $b"
来源：http://cf.bjjhwx.cn

[T04] Kotlin：空安全
来源：http://eq.shxzskj.cn

val n: String? = null;  n?.length
来源：http://on.muxihuayi.cn

[T05] Kotlin：when 表达式
来源：http://za.nicolike.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lh.yuntaijiaju.cn

[T06] Kotlin：集合映射
来源：http://qs.shxzskj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://if.chemitech.net.cn

[T07] Kotlin：集合过滤
来源：http://hc.bjjhwx.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wh.huixinmuqiang.cn

[T08] Kotlin：数据类
来源：http://ja.hahajie.cn

data class User(val name: String, val age: Int)
来源：http://jp.yuexingan06.cn

[T09] Kotlin：扩展函数
来源：http://up.gzmigu.cn

fun String.exclaim() = this + "!"
来源：http://ud.yuexingan06.cn

[T10] Kotlin：默认参数
来源：http://zp.yuntaijiaju.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://yz.gzmigu.cn

[T11] Kotlin：协程
来源：http://dr.szsharing.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hg.bjjhwx.cn

[T12] Kotlin：解构声明
来源：http://ei.hnjuh.cn

val (a, b) = Pair(1, 2)
来源：http://iu.colortex.cn

[T13] Kotlin：只读 Map
来源：http://mh.bjjhwx.cn

val m = mapOf("a" to 1)
来源：http://cf.shxzskj.cn

[T14] Kotlin：循环
来源：http://on.gzmigu.cn

for (i in 1..10) println(i)
来源：http://av.jianghongdianzi.cn

[T15] Kotlin：接口
来源：http://bl.nszjky.cn

interface Shape { fun area(): Double }
来源：http://cd.szsharing.cn

[T16] Swift：Hello World
来源：http://zd.521024.cn

print("Hello")
来源：http://kt.shtwfgs.cn

[T17] Swift：变量与常量
来源：http://dp.shxzukj.cn

var a = 1;  let b = 2
来源：http://pj.asd995.cn

[T18] Swift：字符串插值
来源：http://fd.shxzskj.cn

"值: \(b)"
来源：http://is.521024.cn

[T19] Swift：可选绑定
来源：http://da.yuexingan06.cn

if let n = opt { print(n) }
来源：http://vx.lnxyls.cn

[T20] Swift：数组操作
来源：http://ud.521024.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fa.lnxyls.cn

[T21] Swift：遍历
来源：http://cm.bookmarksfly.cn

for x in a { print(x) }
来源：http://on.muxihuayi.cn

[T22] Swift：字典
来源：http://hx.yuexingan06.cn

var d = ["a": 1];  d["b"] = 2
来源：http://yw.chemitech.net.cn

[T23] Swift：函数
来源：http://vf.haigaiapp.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wx.shxzukj.cn

[T24] Swift：闭包
来源：http://ve.muxihuayi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://bq.asd995.cn

[T25] Swift：结构体
来源：http://nu.panjiajie.cn

struct P { var x: Int }
来源：http://wq.jctech888.com.cn

[T26] Swift：类与重写
来源：http://ry.hahajie.cn

class A: Base { override func f() {} }
来源：http://np.szsharing.cn

[T27] Swift：错误处理
来源：http://ue.bookmarksfly.cn

do { try f() } catch { print(error) }
来源：http://xh.gzmigu.cn

[T28] Swift：枚举
来源：http://or.9csxet.cn

enum Color { case red, green }
来源：http://cz.chemitech.net.cn

[T29] Swift：guard 提前返回
来源：http://nr.nicolike.cn

guard let x = opt else { return }
来源：http://xs.yuexingan06.cn

[T30] Swift：协议
来源：http://ir.lnxyls.cn

protocol Shape { func area() -> Double }
来源：http://lc.shxzskj.cn

[T31] Lua：Hello World
来源：http://ki.521024.cn

print("Hello")
来源：http://hp.9csxet.cn

[T32] Lua：局部变量
来源：http://yu.9csxet.cn

local a = 1
来源：http://yn.colortex.cn

[T33] Lua：表（数组）
来源：http://yc.panjiajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xb.bjjhwx.cn

[T34] Lua：遍历表
来源：http://lb.huixinmuqiang.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://eg.jianghongdianzi.cn

[T35] Lua：字典表
来源：http://ou.521024.cn

local d = { a = 1 };  d.b = 2
来源：http://nx.shxzskj.cn

[T36] Lua：函数
来源：http://hj.huanxung.cn

function add(a, b) return a + b end
来源：http://ru.521024.cn

[T37] Lua：字符串拼接
来源：http://ce.jianghongdianzi.cn

"a" .. "b"
来源：http://ea.newstarts.cn

[T38] Lua：条件
来源：http://ta.jianghongdianzi.cn

if x > 0 then print("正") end
来源：http://hn.shxzskj.cn

[T39] Lua：模式匹配
来源：http://ng.panjiajie.cn

string.find(s, "%d+")
来源：http://mb.nszjky.cn

[T40] Lua：元表
来源：http://yh.bookmarksfly.cn

setmetatable({}, { __index = base })
来源：http://sy.asd995.cn

[T41] Perl：Hello World
来源：http://ez.nszjky.cn

print "Hello\n";
来源：http://qd.huixiangedu.cn

[T42] Perl：变量类型
来源：http://qp.bjjhwx.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bj.bjjhwx.cn

[T43] Perl：字符串插值
来源：http://yl.huixinmuqiang.cn

"值: $a"
来源：http://lt.yuexingan06.cn

[T44] Perl：条件
来源：http://wt.colortex.cn

if ($a > 0) { print "正"; }
来源：http://fo.chemitech.net.cn

[T45] Perl：数组遍历
来源：http://wc.huixiangedu.cn

for my $x (@arr) { print $x; }
来源：http://bk.huixiangedu.cn

[T46] Perl：哈希操作
来源：http://uw.gzmigu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ry.jctech888.com.cn

[T47] Perl：正则捕获
来源：http://zj.shxzskj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jp.jctech888.com.cn

[T48] Perl：正则替换
来源：http://oz.colortex.cn

$s =~ s/old/new/g;
来源：http://or.jianghongdianzi.cn

[T49] Perl：函数
来源：http://ur.shxzskj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vg.muxihuayi.cn

[T50] Perl：逐行读文件
来源：http://xc.muxihuayi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://cz.shxzskj.cn

while (my $line = <$fh>) { print $line; }
来源：http://xc.521024.cn

[T51] Scala：Hello World
来源：http://sj.chemitech.net.cn

println("Hello")
来源：http://uk.haigaiapp.cn

[T52] Scala：变量
来源：http://ro.newstarts.cn

val a = 1;  var b = 2
来源：http://ob.nszjky.cn

[T53] Scala：字符串插值
来源：http://oo.nicolike.cn

s"值: $b"
来源：http://zw.muxihuayi.cn

[T54] Scala：集合映射
来源：http://cy.9csxet.cn

List(1, 2, 3).map(_ * 2)
来源：http://hv.bookmarksfly.cn

[T55] Scala：集合过滤
来源：http://ex.panjiajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://oi.jianghongdianzi.cn

[T56] Scala：样例类
来源：http://ar.nicolike.cn

case class User(name: String, age: Int)
来源：http://pj.521024.cn

[T57] Scala：模式匹配
来源：http://kl.jianghongdianzi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gq.nicolike.cn

[T58] Scala：函数定义
来源：http://fo.nszjky.cn

def add(a: Int, b: Int): Int = a + b
来源：http://dk.shxzukj.cn

[T59] Scala：循环
来源：http://wn.shxzukj.cn

for (i <- 1 to 10) println(i)
来源：http://zp.yuntaijiaju.cn

[T60] Scala：折叠
来源：http://bl.bookmarksfly.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yx.shtwfgs.cn

================================================================================
来源：http://vt.nszjky.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tm.szxytkj.cn

================================================================================
来源：http://mp.shtwfgs.cn

[U01] Py：创建虚拟环境
来源：http://qn.newstarts.cn

python -m venv .venv && source .venv/bin/activate
来源：http://fk.9csxet.cn

[U02] Py：导出 / 安装依赖
来源：http://id.newstarts.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fi.huanxung.cn

[U03] Py：加载 .env 配置
来源：http://on.jctech888.com.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rr.nszjky.cn

[U04] Py：变量调试打印
来源：http://yf.huixiangedu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ig.nicolike.cn

[U05] Py：列表去重且保序
来源：http://xs.yuexingan06.cn

list(dict.fromkeys(arr))
来源：http://qo.haigaiapp.cn

[U06] Py：合并两个字典
来源：http://rn.nszjky.cn

{**a, **b}
来源：http://zx.wgjwhj.cn

[U07] Py：反转字典键值
来源：http://ql.gzmigu.cn

{v: k for k, v in d.items()}
来源：http://fy.bjjhwx.cn

[U08] Py：展平二维列表
来源：http://ny.hnjuh.cn

[y for x in nested for y in x]
来源：http://ev.hnjuh.cn

[U09] Py：字典取最大值的键
来源：http://yv.huixiangedu.cn

max(d, key=d.get)
来源：http://dl.shxzukj.cn

[U10] Py：按值排序字典
来源：http://ky.huixinmuqiang.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ui.chemitech.net.cn

[U11] Py：生成器表达式
来源：http://zm.jianghongdianzi.cn

(x * 2 for x in arr)
来源：http://om.huixinmuqiang.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rt.huanxung.cn

Counter(arr).most_common(3)
来源：http://rh.huixiangedu.cn

[U13] Py：固定长度队列
来源：http://jq.hahajie.cn

deque(maxlen=10)
来源：http://dw.szxytkj.cn

[U14] Py：分组收集到列表
来源：http://ul.asd995.cn

defaultdict(list)
来源：http://zk.muxihuayi.cn

[U15] Py：高精度计时
来源：http://kw.jianghongdianzi.cn

t = time.perf_counter()
来源：http://sa.huixinmuqiang.cn

[U16] Py：命令行参数解析
来源：http://tu.shxzskj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lf.huanxung.cn

[U17] Py：初始化日志
来源：http://ch.nszjky.cn

logging.basicConfig(level=logging.INFO)
来源：http://fb.521024.cn

[U18] Py：预编译正则
来源：http://es.yuexingan06.cn

pat = re.compile(r"\d+")
来源：http://br.9csxet.cn

[U19] Py：正则替换带回调
来源：http://ng.shxzskj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://as.asd995.cn

[U20] Py：缓存函数结果
来源：http://ak.huixiangedu.cn

@functools.lru_cache(maxsize=None)
来源：http://hb.jctech888.com.cn

[U21] Py：自定义上下文管理器
来源：http://tv.colortex.cn

@contextlib.contextmanager
来源：http://ai.huanxung.cn

[U22] Py：矩阵转置
来源：http://ra.bjjhwx.cn

list(zip(*m))
来源：http://xj.nszjky.cn

[U23] Py：分块读取大文件
来源：http://jz.haigaiapp.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zg.huanxung.cn

[U24] Py：路径操作
来源：http://ck.jctech888.com.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qa.huixiangedu.cn

[U25] Py：CSV 按字典读
来源：http://xv.nicolike.cn

csv.DictReader(f)
来源：http://ma.yuntaijiaju.cn

[U26] Py：并发下载
来源：http://aa.shxzukj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vx.huixinmuqiang.cn

[U27] Py：异步 HTTP
来源：http://bn.newstarts.cn

aiohttp.ClientSession() 配合 async with
来源：http://mm.hahajie.cn

[U28] Py：类型别名
来源：http://zr.hnjuh.cn

UserId = int
来源：http://dk.colortex.cn

[U29] Py：属性校验
来源：http://gc.9csxet.cn

@property 与 @x.setter 配合
来源：http://dc.hahajie.cn

[U30] Py：数据类
来源：http://by.shtwfgs.cn

@dataclass(slots=True)
来源：http://rv.nszjky.cn

[U31] Py：单测
来源：http://px.521024.cn

python -m pytest -q
来源：http://kl.bjjhwx.cn

[U32] Py：代码格式化
来源：http://bs.panjiajie.cn

ruff format . && ruff check --fix .
来源：http://id.gzmigu.cn

[U33] Py：打包发布
来源：http://ni.hnjuh.cn

python -m build  （依赖 pyproject.toml）
来源：http://mv.huixinmuqiang.cn

[U34] Py：判断编码
来源：http://hu.huixiangedu.cn

chardet.detect(raw)
来源：http://hs.szxytkj.cn

[U35] Py：发送邮件
来源：http://rt.jctech888.com.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://uc.huanxung.cn

[U36] Py：定时任务
来源：http://wx.9csxet.cn

schedule.every(10).minutes.do(job)
来源：http://wc.bjjhwx.cn

[U37] Py：读写 Excel
来源：http://br.bjjhwx.cn

pandas.read_excel / DataFrame.to_excel
来源：http://hw.shxzukj.cn

[U38] Py：获取脚本所在目录
来源：http://rn.huixinmuqiang.cn

Path(__file__).resolve().parent
来源：http://of.nicolike.cn

[U39] Py：判断是否在交互环境
来源：http://ge.hahajie.cn

sys.stdout.isatty()
来源：http://az.bjjhwx.cn

[U40] Py：打印到标准错误
来源：http://lb.panjiajie.cn

print("err", file=sys.stderr)
来源：http://hl.9csxet.cn

[U41] PHP：初始化 Composer 项目
来源：http://hl.haigaiapp.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ba.jianghongdianzi.cn

[U42] PHP：PSR-4 自动加载
来源：http://pu.muxihuayi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pq.muxihuayi.cn

[U43] PHP：声明命名空间
来源：http://yb.panjiajie.cn

namespace App\Http;
来源：http://iz.521024.cn

[U44] PHP：开启严格类型
来源：http://tb.9csxet.cn

declare(strict_types=1);
来源：http://mp.lnxyls.cn

[U45] PHP：类型声明与返回类型
来源：http://ja.newstarts.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://vz.panjiajie.cn

[U46] PHP：可空类型
来源：http://su.jctech888.com.cn

?string $name = null
来源：http://bh.panjiajie.cn

[U47] PHP：联合类型
来源：http://ls.szxytkj.cn

int|string $id
来源：http://np.colortex.cn

[U48] PHP：纯枚举
来源：http://oc.haigaiapp.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://em.lnxyls.cn

[U49] PHP：只读属性
来源：http://sr.shtwfgs.cn

public readonly string $name
来源：http://zl.jianghongdianzi.cn

[U50] PHP：构造器属性提升
来源：http://qt.gzmigu.cn

public function __construct(private int $id) {}
来源：http://kk.yuntaijiaju.cn

[U51] PHP：数组解构
来源：http://sg.newstarts.cn

[$a, $b] = $arr;
来源：http://pj.muxihuayi.cn

[U52] PHP：箭头函数
来源：http://qe.wgjwhj.cn

$double = fn($x) => $x * 2;
来源：http://la.haigaiapp.cn

[U53] PHP：空合并运算符
来源：http://fm.jianghongdianzi.cn

$v = $a ?? $b ?? "default";
来源：http://qb.gzmigu.cn

[U54] PHP：空安全调用
来源：http://yv.shtwfgs.cn

$obj?->method()
来源：http://dj.haigaiapp.cn

[U55] PHP：match 表达式
来源：http://ap.9csxet.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yi.shxzskj.cn

[U56] PHP：命名参数
来源：http://ox.szsharing.cn

f(a: 1, b: 2)
来源：http://er.jctech888.com.cn

[U57] PHP：字符串插值
来源：http://om.panjiajie.cn

"值: {$a}"
来源：http://oo.hahajie.cn

[U58] PHP：数组三件套
来源：http://cf.huixinmuqiang.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lb.nicolike.cn

[U59] PHP：自定义排序
来源：http://zn.wgjwhj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vz.hnjuh.cn

[U60] PHP：JSON 编解码
来源：http://hr.muxihuayi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gl.yuntaijiaju.cn

[U61] PHP：正则
来源：http://ha.shxzukj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://je.bookmarksfly.cn

[U62] PHP：日期对象
来源：http://um.colortex.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bd.nicolike.cn

[U63] PHP：文件读写
来源：http://cb.wgjwhj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dy.hahajie.cn

[U64] PHP：目录遍历
来源：http://wf.shtwfgs.cn

glob("dir/*.php");  scandir("dir");
来源：http://dv.szxytkj.cn

[U65] PHP：会话
来源：http://es.huanxung.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ja.szsharing.cn

[U66] PHP：设置 Cookie
来源：http://pf.9csxet.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://eh.shxzukj.cn

[U67] PHP：处理文件上传
来源：http://cv.wgjwhj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pq.chemitech.net.cn

[U68] PHP：PDO 连接
来源：http://cx.chemitech.net.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://be.gzmigu.cn


<!-- 参考信息 -->