代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://ol.szsharing.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bb.yuexingan06.cn

[S48] C++：逐行读文件
来源：http://hc.bjjhwx.cn

std::ifstream in("a.txt");  std::string line;
来源：http://no.lnxyls.cn

while (std::getline(in, line)) { }
来源：http://wx.shxzskj.cn

[S49] C++：写文件
来源：http://kj.9csxet.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zf.bjjhwx.cn

[S50] C++：格式化数字
来源：http://ic.wgjwhj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qw.gzmigu.cn

[S51] C++：显式类型转换
来源：http://mb.panjiajie.cn

static_cast<double>(a) / b
来源：http://le.szsharing.cn

[S52] C++：const 与 noexcept
来源：http://ie.shtwfgs.cn

int size() const noexcept { return n_; }
来源：http://zk.wgjwhj.cn

[S53] C++：移动语义
来源：http://yu.jctech888.com.cn

std::vector<int> w = std::move(v);
来源：http://fq.muxihuayi.cn

[S54] C++：异常处理
来源：http://vf.colortex.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xh.jianghongdianzi.cn

[S55] C++：结构化绑定
来源：http://hb.yuexingan06.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wb.yuexingan06.cn

[S56] C++：optional
来源：http://nn.yuntaijiaju.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://up.nicolike.cn

[S57] C++：编译期常量
来源：http://th.shxzukj.cn

constexpr int N = 10;
来源：http://fy.bjjhwx.cn

[S58] C++：命名空间
来源：http://qq.jctech888.com.cn

namespace ns { int f() { return 1; } }
来源：http://vp.hnjuh.cn

[S59] C++：静态断言
来源：http://ic.colortex.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gl.shxzukj.cn

[S60] C++：遍历并删除元素
来源：http://ur.wgjwhj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tb.newstarts.cn

================================================================================
来源：http://vj.wgjwhj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yh.jianghongdianzi.cn

================================================================================
来源：http://dh.yuexingan06.cn

[T01] Kotlin：Hello World
来源：http://xd.gzmigu.cn

println("Hello")
来源：http://re.shxzukj.cn

[T02] Kotlin：变量
来源：http://uh.shxzskj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ll.chemitech.net.cn

[T03] Kotlin：字符串模板
来源：http://th.muxihuayi.cn

"值: $b"
来源：http://hg.huixinmuqiang.cn

[T04] Kotlin：空安全
来源：http://qs.shtwfgs.cn

val n: String? = null;  n?.length
来源：http://io.szxytkj.cn

[T05] Kotlin：when 表达式
来源：http://wt.bjjhwx.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ka.shxzskj.cn

[T06] Kotlin：集合映射
来源：http://js.yuntaijiaju.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hj.nicolike.cn

[T07] Kotlin：集合过滤
来源：http://ha.huanxung.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://rv.nicolike.cn

[T08] Kotlin：数据类
来源：http://yp.yuntaijiaju.cn

data class User(val name: String, val age: Int)
来源：http://ia.huixinmuqiang.cn

[T09] Kotlin：扩展函数
来源：http://gh.asd995.cn

fun String.exclaim() = this + "!"
来源：http://sn.jianghongdianzi.cn

[T10] Kotlin：默认参数
来源：http://dg.huixiangedu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wh.colortex.cn

[T11] Kotlin：协程
来源：http://po.shxzskj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://rp.muxihuayi.cn

[T12] Kotlin：解构声明
来源：http://ap.colortex.cn

val (a, b) = Pair(1, 2)
来源：http://rq.wgjwhj.cn

[T13] Kotlin：只读 Map
来源：http://pv.shxzukj.cn

val m = mapOf("a" to 1)
来源：http://hg.yuntaijiaju.cn

[T14] Kotlin：循环
来源：http://nm.jctech888.com.cn

for (i in 1..10) println(i)
来源：http://en.haigaiapp.cn

[T15] Kotlin：接口
来源：http://pa.nszjky.cn

interface Shape { fun area(): Double }
来源：http://yi.521024.cn

[T16] Swift：Hello World
来源：http://at.panjiajie.cn

print("Hello")
来源：http://mm.huanxung.cn

[T17] Swift：变量与常量
来源：http://wa.chemitech.net.cn

var a = 1;  let b = 2
来源：http://ms.nicolike.cn

[T18] Swift：字符串插值
来源：http://fe.bookmarksfly.cn

"值: \(b)"
来源：http://do.wgjwhj.cn

[T19] Swift：可选绑定
来源：http://kn.521024.cn

if let n = opt { print(n) }
来源：http://ps.shtwfgs.cn

[T20] Swift：数组操作
来源：http://gt.shxzukj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gj.bookmarksfly.cn

[T21] Swift：遍历
来源：http://br.nicolike.cn

for x in a { print(x) }
来源：http://ow.lnxyls.cn

[T22] Swift：字典
来源：http://gv.bjjhwx.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mr.nszjky.cn

[T23] Swift：函数
来源：http://ng.nszjky.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fb.lnxyls.cn

[T24] Swift：闭包
来源：http://js.colortex.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://mv.hnjuh.cn

[T25] Swift：结构体
来源：http://wu.shxzukj.cn

struct P { var x: Int }
来源：http://vg.hnjuh.cn

[T26] Swift：类与重写
来源：http://ti.huanxung.cn

class A: Base { override func f() {} }
来源：http://xp.muxihuayi.cn

[T27] Swift：错误处理
来源：http://ie.huanxung.cn

do { try f() } catch { print(error) }
来源：http://nr.lnxyls.cn

[T28] Swift：枚举
来源：http://cv.haigaiapp.cn

enum Color { case red, green }
来源：http://jx.jianghongdianzi.cn

[T29] Swift：guard 提前返回
来源：http://wz.yuexingan06.cn

guard let x = opt else { return }
来源：http://az.hahajie.cn

[T30] Swift：协议
来源：http://ec.jctech888.com.cn

protocol Shape { func area() -> Double }
来源：http://wz.shxzskj.cn

[T31] Lua：Hello World
来源：http://gq.haigaiapp.cn

print("Hello")
来源：http://rg.shxzukj.cn

[T32] Lua：局部变量
来源：http://dc.huixiangedu.cn

local a = 1
来源：http://ei.asd995.cn

[T33] Lua：表（数组）
来源：http://ps.jianghongdianzi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://nn.9csxet.cn

[T34] Lua：遍历表
来源：http://ml.jianghongdianzi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://nl.9csxet.cn

[T35] Lua：字典表
来源：http://ka.szsharing.cn

local d = { a = 1 };  d.b = 2
来源：http://kk.nszjky.cn

[T36] Lua：函数
来源：http://qg.bjjhwx.cn

function add(a, b) return a + b end
来源：http://cz.hahajie.cn

[T37] Lua：字符串拼接
来源：http://wl.shxzskj.cn

"a" .. "b"
来源：http://vq.colortex.cn

[T38] Lua：条件
来源：http://il.szsharing.cn

if x > 0 then print("正") end
来源：http://cm.hahajie.cn

[T39] Lua：模式匹配
来源：http://kk.muxihuayi.cn

string.find(s, "%d+")
来源：http://cu.bjjhwx.cn

[T40] Lua：元表
来源：http://wz.huixinmuqiang.cn

setmetatable({}, { __index = base })
来源：http://sc.bookmarksfly.cn

[T41] Perl：Hello World
来源：http://ru.huixiangedu.cn

print "Hello\n";
来源：http://sk.9csxet.cn

[T42] Perl：变量类型
来源：http://ot.haigaiapp.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yg.521024.cn

[T43] Perl：字符串插值
来源：http://ol.huixinmuqiang.cn

"值: $a"
来源：http://bu.szxytkj.cn

[T44] Perl：条件
来源：http://ud.szxytkj.cn

if ($a > 0) { print "正"; }
来源：http://wo.9csxet.cn

[T45] Perl：数组遍历
来源：http://xf.shxzskj.cn

for my $x (@arr) { print $x; }
来源：http://ke.chemitech.net.cn

[T46] Perl：哈希操作
来源：http://jy.shxzukj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rr.bjjhwx.cn

[T47] Perl：正则捕获
来源：http://yq.gzmigu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rb.hnjuh.cn

[T48] Perl：正则替换
来源：http://sv.hahajie.cn

$s =~ s/old/new/g;
来源：http://ur.9csxet.cn

[T49] Perl：函数
来源：http://fd.yuntaijiaju.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nc.hnjuh.cn

[T50] Perl：逐行读文件
来源：http://da.szsharing.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://cm.nszjky.cn

while (my $line = <$fh>) { print $line; }
来源：http://kw.haigaiapp.cn

[T51] Scala：Hello World
来源：http://em.jctech888.com.cn

println("Hello")
来源：http://su.shxzukj.cn

[T52] Scala：变量
来源：http://hm.newstarts.cn

val a = 1;  var b = 2
来源：http://qk.bjjhwx.cn

[T53] Scala：字符串插值
来源：http://yo.wgjwhj.cn

s"值: $b"
来源：http://bl.szxytkj.cn

[T54] Scala：集合映射
来源：http://re.szsharing.cn

List(1, 2, 3).map(_ * 2)
来源：http://hc.szsharing.cn

[T55] Scala：集合过滤
来源：http://zn.szxytkj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fr.asd995.cn

[T56] Scala：样例类
来源：http://hg.jctech888.com.cn

case class User(name: String, age: Int)
来源：http://ni.huanxung.cn

[T57] Scala：模式匹配
来源：http://tm.huanxung.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://pz.jianghongdianzi.cn

[T58] Scala：函数定义
来源：http://lh.yuntaijiaju.cn

def add(a: Int, b: Int): Int = a + b
来源：http://at.asd995.cn

[T59] Scala：循环
来源：http://iv.bookmarksfly.cn

for (i <- 1 to 10) println(i)
来源：http://kv.haigaiapp.cn

[T60] Scala：折叠
来源：http://kb.hahajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://br.hnjuh.cn

================================================================================
来源：http://vl.panjiajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kt.gzmigu.cn

================================================================================
来源：http://xq.lnxyls.cn

[U01] Py：创建虚拟环境
来源：http://fy.9csxet.cn

python -m venv .venv && source .venv/bin/activate
来源：http://dl.muxihuayi.cn

[U02] Py：导出 / 安装依赖
来源：http://el.jianghongdianzi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mx.9csxet.cn

[U03] Py：加载 .env 配置
来源：http://qq.yuexingan06.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://lc.521024.cn

[U04] Py：变量调试打印
来源：http://ke.yuexingan06.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bp.huixiangedu.cn

[U05] Py：列表去重且保序
来源：http://ax.chemitech.net.cn

list(dict.fromkeys(arr))
来源：http://mv.jctech888.com.cn

[U06] Py：合并两个字典
来源：http://ac.nicolike.cn

{**a, **b}
来源：http://px.newstarts.cn

[U07] Py：反转字典键值
来源：http://to.haigaiapp.cn

{v: k for k, v in d.items()}
来源：http://zt.yuexingan06.cn

[U08] Py：展平二维列表
来源：http://ba.huixinmuqiang.cn

[y for x in nested for y in x]
来源：http://tl.hahajie.cn

[U09] Py：字典取最大值的键
来源：http://jy.asd995.cn

max(d, key=d.get)
来源：http://ig.shxzukj.cn

[U10] Py：按值排序字典
来源：http://yo.9csxet.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://iy.panjiajie.cn

[U11] Py：生成器表达式
来源：http://tc.nszjky.cn

(x * 2 for x in arr)
来源：http://mw.huanxung.cn

[U12] Py：取出现最多的 3 个元素
来源：http://gd.jctech888.com.cn

Counter(arr).most_common(3)
来源：http://ky.bookmarksfly.cn

[U13] Py：固定长度队列
来源：http://cq.haigaiapp.cn

deque(maxlen=10)
来源：http://wk.haigaiapp.cn

[U14] Py：分组收集到列表
来源：http://tw.haigaiapp.cn

defaultdict(list)
来源：http://nv.huixinmuqiang.cn

[U15] Py：高精度计时
来源：http://lj.jctech888.com.cn

t = time.perf_counter()
来源：http://rd.chemitech.net.cn

[U16] Py：命令行参数解析
来源：http://cd.hnjuh.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kv.newstarts.cn

[U17] Py：初始化日志
来源：http://eg.haigaiapp.cn

logging.basicConfig(level=logging.INFO)
来源：http://hf.bookmarksfly.cn

[U18] Py：预编译正则
来源：http://ow.asd995.cn

pat = re.compile(r"\d+")
来源：http://na.jianghongdianzi.cn

[U19] Py：正则替换带回调
来源：http://tp.9csxet.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kl.szxytkj.cn

[U20] Py：缓存函数结果
来源：http://zr.lnxyls.cn

@functools.lru_cache(maxsize=None)
来源：http://uq.shxzukj.cn

[U21] Py：自定义上下文管理器
来源：http://mw.521024.cn

@contextlib.contextmanager
来源：http://zx.wgjwhj.cn

[U22] Py：矩阵转置
来源：http://ek.bookmarksfly.cn

list(zip(*m))
来源：http://jq.colortex.cn

[U23] Py：分块读取大文件
来源：http://fk.muxihuayi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zg.hnjuh.cn

[U24] Py：路径操作
来源：http://nq.shxzskj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ih.panjiajie.cn

[U25] Py：CSV 按字典读
来源：http://ee.asd995.cn

csv.DictReader(f)
来源：http://vr.9csxet.cn

[U26] Py：并发下载
来源：http://be.yuntaijiaju.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://un.bookmarksfly.cn

[U27] Py：异步 HTTP
来源：http://qg.yuexingan06.cn

aiohttp.ClientSession() 配合 async with
来源：http://bu.yuexingan06.cn

[U28] Py：类型别名
来源：http://hn.lnxyls.cn

UserId = int
来源：http://wm.bookmarksfly.cn

[U29] Py：属性校验
来源：http://kr.newstarts.cn

@property 与 @x.setter 配合
来源：http://am.yuexingan06.cn

[U30] Py：数据类
来源：http://rh.chemitech.net.cn

@dataclass(slots=True)
来源：http://rh.chemitech.net.cn

[U31] Py：单测
来源：http://on.521024.cn

python -m pytest -q
来源：http://ur.shxzskj.cn

[U32] Py：代码格式化
来源：http://vx.yuexingan06.cn

ruff format . && ruff check --fix .
来源：http://xx.haigaiapp.cn

[U33] Py：打包发布
来源：http://sl.huanxung.cn

python -m build  （依赖 pyproject.toml）
来源：http://sx.bookmarksfly.cn

[U34] Py：判断编码
来源：http://pg.panjiajie.cn

chardet.detect(raw)
来源：http://eq.chemitech.net.cn

[U35] Py：发送邮件
来源：http://sd.szxytkj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mq.szxytkj.cn

[U36] Py：定时任务
来源：http://gz.lnxyls.cn

schedule.every(10).minutes.do(job)
来源：http://mm.wgjwhj.cn

[U37] Py：读写 Excel
来源：http://iw.huixiangedu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://hz.wgjwhj.cn

[U38] Py：获取脚本所在目录
来源：http://ek.hahajie.cn

Path(__file__).resolve().parent
来源：http://zj.nszjky.cn

[U39] Py：判断是否在交互环境
来源：http://jk.panjiajie.cn

sys.stdout.isatty()
来源：http://xg.huixinmuqiang.cn

[U40] Py：打印到标准错误
来源：http://eg.colortex.cn

print("err", file=sys.stderr)
来源：http://tz.szsharing.cn

[U41] PHP：初始化 Composer 项目
来源：http://jl.yuntaijiaju.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://oj.hahajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://rk.newstarts.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ud.jianghongdianzi.cn

[U43] PHP：声明命名空间
来源：http://qn.asd995.cn

namespace App\Http;
来源：http://ag.nszjky.cn

[U44] PHP：开启严格类型
来源：http://xy.szsharing.cn

declare(strict_types=1);
来源：http://bx.nszjky.cn

[U45] PHP：类型声明与返回类型
来源：http://qu.jianghongdianzi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://il.shtwfgs.cn

[U46] PHP：可空类型
来源：http://uc.bookmarksfly.cn

?string $name = null
来源：http://io.huixinmuqiang.cn

[U47] PHP：联合类型
来源：http://hj.szsharing.cn

int|string $id
来源：http://mo.shxzskj.cn

[U48] PHP：纯枚举
来源：http://wz.9csxet.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ov.asd995.cn

[U49] PHP：只读属性
来源：http://tm.muxihuayi.cn

public readonly string $name
来源：http://ja.huixiangedu.cn

[U50] PHP：构造器属性提升
来源：http://nk.521024.cn

public function __construct(private int $id) {}
来源：http://pa.asd995.cn

[U51] PHP：数组解构
来源：http://op.bjjhwx.cn

[$a, $b] = $arr;
来源：http://gl.yuntaijiaju.cn

[U52] PHP：箭头函数
来源：http://ua.shxzskj.cn

$double = fn($x) => $x * 2;
来源：http://je.nicolike.cn

[U53] PHP：空合并运算符
来源：http://ne.bookmarksfly.cn

$v = $a ?? $b ?? "default";
来源：http://ks.szsharing.cn

[U54] PHP：空安全调用
来源：http://kz.bookmarksfly.cn

$obj?->method()
来源：http://td.asd995.cn

[U55] PHP：match 表达式
来源：http://dj.shxzskj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fm.colortex.cn

[U56] PHP：命名参数
来源：http://jv.huanxung.cn

f(a: 1, b: 2)
来源：http://es.shxzukj.cn

[U57] PHP：字符串插值
来源：http://hq.jctech888.com.cn

"值: {$a}"
来源：http://zn.huixiangedu.cn

[U58] PHP：数组三件套
来源：http://lu.shtwfgs.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ck.muxihuayi.cn

[U59] PHP：自定义排序
来源：http://tc.haigaiapp.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bk.shxzskj.cn

[U60] PHP：JSON 编解码
来源：http://ks.chemitech.net.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qt.szxytkj.cn

[U61] PHP：正则
来源：http://xv.huixinmuqiang.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://uw.szsharing.cn

[U62] PHP：日期对象
来源：http://vo.asd995.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ed.muxihuayi.cn

[U63] PHP：文件读写
来源：http://sx.gzmigu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ck.muxihuayi.cn

[U64] PHP：目录遍历
来源：http://wl.lnxyls.cn

glob("dir/*.php");  scandir("dir");
来源：http://ni.jctech888.com.cn

[U65] PHP：会话
来源：http://kt.nicolike.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://jv.newstarts.cn

[U66] PHP：设置 Cookie
来源：http://ky.chemitech.net.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mj.huixinmuqiang.cn

[U67] PHP：处理文件上传
来源：http://ne.szsharing.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qk.huixiangedu.cn

[U68] PHP：PDO 连接
来源：http://hj.bookmarksfly.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xm.nicolike.cn

[U69] PHP：PDO 预处理
来源：http://ls.chemitech.net.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fg.jctech888.com.cn

[U70] PHP：PDO 事务
来源：http://gc.hnjuh.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wi.panjiajie.cn

[U71] PHP：抛出异常
来源：http://fm.gzmigu.cn

throw new RuntimeException("失败", 500);
来源：http://he.gzmigu.cn

[U72] PHP：写错误日志
来源：http://mx.shxzskj.cn

error_log("失败: " . $e->getMessage());
来源：http://ir.shxzskj.cn


<!-- 参考信息 -->