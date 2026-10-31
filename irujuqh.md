代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://wx.szxytkj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wt.nszjky.cn

[S48] C++：逐行读文件
来源：http://tw.shtwfgs.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pl.newstarts.cn

while (std::getline(in, line)) { }
来源：http://wz.nszjky.cn

[S49] C++：写文件
来源：http://kv.haigaiapp.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xm.huanxung.cn

[S50] C++：格式化数字
来源：http://xh.panjiajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sc.panjiajie.cn

[S51] C++：显式类型转换
来源：http://zs.lnxyls.cn

static_cast<double>(a) / b
来源：http://rz.newstarts.cn

[S52] C++：const 与 noexcept
来源：http://ui.9csxet.cn

int size() const noexcept { return n_; }
来源：http://ts.haigaiapp.cn

[S53] C++：移动语义
来源：http://fh.hahajie.cn

std::vector<int> w = std::move(v);
来源：http://yz.chemitech.net.cn

[S54] C++：异常处理
来源：http://ri.nicolike.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ne.szsharing.cn

[S55] C++：结构化绑定
来源：http://lu.szsharing.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mf.huanxung.cn

[S56] C++：optional
来源：http://jw.521024.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://un.huanxung.cn

[S57] C++：编译期常量
来源：http://mp.yuexingan06.cn

constexpr int N = 10;
来源：http://zv.panjiajie.cn

[S58] C++：命名空间
来源：http://ce.nszjky.cn

namespace ns { int f() { return 1; } }
来源：http://ee.huixinmuqiang.cn

[S59] C++：静态断言
来源：http://ma.bjjhwx.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xb.newstarts.cn

[S60] C++：遍历并删除元素
来源：http://pj.haigaiapp.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yu.newstarts.cn

================================================================================
来源：http://cw.hahajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uv.szxytkj.cn

================================================================================
来源：http://tc.szxytkj.cn

[T01] Kotlin：Hello World
来源：http://ap.asd995.cn

println("Hello")
来源：http://xf.gzmigu.cn

[T02] Kotlin：变量
来源：http://gz.yuntaijiaju.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://km.szsharing.cn

[T03] Kotlin：字符串模板
来源：http://nx.panjiajie.cn

"值: $b"
来源：http://dk.hahajie.cn

[T04] Kotlin：空安全
来源：http://oo.jianghongdianzi.cn

val n: String? = null;  n?.length
来源：http://gj.gzmigu.cn

[T05] Kotlin：when 表达式
来源：http://dx.jianghongdianzi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zo.newstarts.cn

[T06] Kotlin：集合映射
来源：http://sv.9csxet.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://zp.chemitech.net.cn

[T07] Kotlin：集合过滤
来源：http://yk.jianghongdianzi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://gc.muxihuayi.cn

[T08] Kotlin：数据类
来源：http://xa.jctech888.com.cn

data class User(val name: String, val age: Int)
来源：http://fl.bjjhwx.cn

[T09] Kotlin：扩展函数
来源：http://oy.shtwfgs.cn

fun String.exclaim() = this + "!"
来源：http://ht.bjjhwx.cn

[T10] Kotlin：默认参数
来源：http://lf.hnjuh.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qk.hahajie.cn

[T11] Kotlin：协程
来源：http://ja.colortex.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hg.haigaiapp.cn

[T12] Kotlin：解构声明
来源：http://ra.szsharing.cn

val (a, b) = Pair(1, 2)
来源：http://tl.shxzskj.cn

[T13] Kotlin：只读 Map
来源：http://px.bjjhwx.cn

val m = mapOf("a" to 1)
来源：http://xo.panjiajie.cn

[T14] Kotlin：循环
来源：http://bl.jctech888.com.cn

for (i in 1..10) println(i)
来源：http://nr.shtwfgs.cn

[T15] Kotlin：接口
来源：http://zb.yuexingan06.cn

interface Shape { fun area(): Double }
来源：http://ah.panjiajie.cn

[T16] Swift：Hello World
来源：http://bi.asd995.cn

print("Hello")
来源：http://cs.shxzukj.cn

[T17] Swift：变量与常量
来源：http://oi.szsharing.cn

var a = 1;  let b = 2
来源：http://ft.jctech888.com.cn

[T18] Swift：字符串插值
来源：http://gg.huixiangedu.cn

"值: \(b)"
来源：http://uh.wgjwhj.cn

[T19] Swift：可选绑定
来源：http://tr.yuexingan06.cn

if let n = opt { print(n) }
来源：http://xl.panjiajie.cn

[T20] Swift：数组操作
来源：http://cv.9csxet.cn

var a = [1, 2, 3];  a.append(4)
来源：http://cl.panjiajie.cn

[T21] Swift：遍历
来源：http://gy.haigaiapp.cn

for x in a { print(x) }
来源：http://mv.hahajie.cn

[T22] Swift：字典
来源：http://el.yuntaijiaju.cn

var d = ["a": 1];  d["b"] = 2
来源：http://uy.hnjuh.cn

[T23] Swift：函数
来源：http://hc.jctech888.com.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ca.szxytkj.cn

[T24] Swift：闭包
来源：http://db.nicolike.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://pv.shxzukj.cn

[T25] Swift：结构体
来源：http://kg.hnjuh.cn

struct P { var x: Int }
来源：http://uc.yuexingan06.cn

[T26] Swift：类与重写
来源：http://qw.521024.cn

class A: Base { override func f() {} }
来源：http://ws.shxzukj.cn

[T27] Swift：错误处理
来源：http://mc.huixinmuqiang.cn

do { try f() } catch { print(error) }
来源：http://xa.newstarts.cn

[T28] Swift：枚举
来源：http://hw.nszjky.cn

enum Color { case red, green }
来源：http://dr.huixiangedu.cn

[T29] Swift：guard 提前返回
来源：http://hr.jianghongdianzi.cn

guard let x = opt else { return }
来源：http://cp.yuexingan06.cn

[T30] Swift：协议
来源：http://im.nicolike.cn

protocol Shape { func area() -> Double }
来源：http://vl.nicolike.cn

[T31] Lua：Hello World
来源：http://gp.jctech888.com.cn

print("Hello")
来源：http://gj.wgjwhj.cn

[T32] Lua：局部变量
来源：http://ey.newstarts.cn

local a = 1
来源：http://nm.szsharing.cn

[T33] Lua：表（数组）
来源：http://bn.chemitech.net.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wf.newstarts.cn

[T34] Lua：遍历表
来源：http://sj.huanxung.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://wd.shtwfgs.cn

[T35] Lua：字典表
来源：http://ek.gzmigu.cn

local d = { a = 1 };  d.b = 2
来源：http://hk.szsharing.cn

[T36] Lua：函数
来源：http://da.szsharing.cn

function add(a, b) return a + b end
来源：http://kv.jianghongdianzi.cn

[T37] Lua：字符串拼接
来源：http://xj.jctech888.com.cn

"a" .. "b"
来源：http://yl.huixinmuqiang.cn

[T38] Lua：条件
来源：http://bs.shxzskj.cn

if x > 0 then print("正") end
来源：http://lq.nicolike.cn

[T39] Lua：模式匹配
来源：http://nj.nszjky.cn

string.find(s, "%d+")
来源：http://pm.hnjuh.cn

[T40] Lua：元表
来源：http://yq.bookmarksfly.cn

setmetatable({}, { __index = base })
来源：http://ci.szxytkj.cn

[T41] Perl：Hello World
来源：http://fo.wgjwhj.cn

print "Hello\n";
来源：http://fb.newstarts.cn

[T42] Perl：变量类型
来源：http://pj.shxzskj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zx.jianghongdianzi.cn

[T43] Perl：字符串插值
来源：http://fk.bookmarksfly.cn

"值: $a"
来源：http://cf.haigaiapp.cn

[T44] Perl：条件
来源：http://fh.hnjuh.cn

if ($a > 0) { print "正"; }
来源：http://cb.shxzskj.cn

[T45] Perl：数组遍历
来源：http://pe.jctech888.com.cn

for my $x (@arr) { print $x; }
来源：http://tq.chemitech.net.cn

[T46] Perl：哈希操作
来源：http://av.jianghongdianzi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://we.szsharing.cn

[T47] Perl：正则捕获
来源：http://ss.bookmarksfly.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wy.bookmarksfly.cn

[T48] Perl：正则替换
来源：http://uc.huixinmuqiang.cn

$s =~ s/old/new/g;
来源：http://pi.jctech888.com.cn

[T49] Perl：函数
来源：http://mr.shtwfgs.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vp.colortex.cn

[T50] Perl：逐行读文件
来源：http://xx.jianghongdianzi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://uk.nszjky.cn

while (my $line = <$fh>) { print $line; }
来源：http://zy.nicolike.cn

[T51] Scala：Hello World
来源：http://lh.shxzskj.cn

println("Hello")
来源：http://lv.jianghongdianzi.cn

[T52] Scala：变量
来源：http://nz.jianghongdianzi.cn

val a = 1;  var b = 2
来源：http://xf.9csxet.cn

[T53] Scala：字符串插值
来源：http://hg.newstarts.cn

s"值: $b"
来源：http://wi.muxihuayi.cn

[T54] Scala：集合映射
来源：http://ox.hahajie.cn

List(1, 2, 3).map(_ * 2)
来源：http://wq.colortex.cn

[T55] Scala：集合过滤
来源：http://vg.panjiajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xl.huixinmuqiang.cn

[T56] Scala：样例类
来源：http://kx.nicolike.cn

case class User(name: String, age: Int)
来源：http://py.colortex.cn

[T57] Scala：模式匹配
来源：http://zd.hnjuh.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vq.huixiangedu.cn

[T58] Scala：函数定义
来源：http://ez.asd995.cn

def add(a: Int, b: Int): Int = a + b
来源：http://sr.wgjwhj.cn

[T59] Scala：循环
来源：http://rf.bjjhwx.cn

for (i <- 1 to 10) println(i)
来源：http://lv.huixiangedu.cn

[T60] Scala：折叠
来源：http://lc.shxzukj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ql.lnxyls.cn

================================================================================
来源：http://vt.bookmarksfly.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ye.nszjky.cn

================================================================================
来源：http://jh.chemitech.net.cn

[U01] Py：创建虚拟环境
来源：http://yp.shxzskj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://pq.yuntaijiaju.cn

[U02] Py：导出 / 安装依赖
来源：http://no.asd995.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ik.muxihuayi.cn

[U03] Py：加载 .env 配置
来源：http://ns.shtwfgs.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gu.wgjwhj.cn

[U04] Py：变量调试打印
来源：http://ap.szsharing.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://st.shxzskj.cn

[U05] Py：列表去重且保序
来源：http://sm.yuexingan06.cn

list(dict.fromkeys(arr))
来源：http://ol.huixinmuqiang.cn

[U06] Py：合并两个字典
来源：http://bn.shxzskj.cn

{**a, **b}
来源：http://iu.shtwfgs.cn

[U07] Py：反转字典键值
来源：http://jy.yuntaijiaju.cn

{v: k for k, v in d.items()}
来源：http://sg.9csxet.cn

[U08] Py：展平二维列表
来源：http://lz.gzmigu.cn

[y for x in nested for y in x]
来源：http://sh.yuntaijiaju.cn

[U09] Py：字典取最大值的键
来源：http://oq.newstarts.cn

max(d, key=d.get)
来源：http://pf.521024.cn

[U10] Py：按值排序字典
来源：http://rt.gzmigu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sl.huixiangedu.cn

[U11] Py：生成器表达式
来源：http://sj.jianghongdianzi.cn

(x * 2 for x in arr)
来源：http://af.shxzukj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://fn.jctech888.com.cn

Counter(arr).most_common(3)
来源：http://iz.hnjuh.cn

[U13] Py：固定长度队列
来源：http://wo.jctech888.com.cn

deque(maxlen=10)
来源：http://pp.bookmarksfly.cn

[U14] Py：分组收集到列表
来源：http://mg.shxzskj.cn

defaultdict(list)
来源：http://fy.nicolike.cn

[U15] Py：高精度计时
来源：http://bj.hahajie.cn

t = time.perf_counter()
来源：http://ew.asd995.cn

[U16] Py：命令行参数解析
来源：http://gl.wgjwhj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gb.521024.cn

[U17] Py：初始化日志
来源：http://ct.yuntaijiaju.cn

logging.basicConfig(level=logging.INFO)
来源：http://vx.nicolike.cn

[U18] Py：预编译正则
来源：http://tr.huixinmuqiang.cn

pat = re.compile(r"\d+")
来源：http://hu.nicolike.cn

[U19] Py：正则替换带回调
来源：http://of.lnxyls.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lt.nicolike.cn

[U20] Py：缓存函数结果
来源：http://td.521024.cn

@functools.lru_cache(maxsize=None)
来源：http://qb.huanxung.cn

[U21] Py：自定义上下文管理器
来源：http://dz.jianghongdianzi.cn

@contextlib.contextmanager
来源：http://qy.hnjuh.cn

[U22] Py：矩阵转置
来源：http://eh.huixiangedu.cn

list(zip(*m))
来源：http://lg.9csxet.cn

[U23] Py：分块读取大文件
来源：http://pc.bookmarksfly.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wh.521024.cn

[U24] Py：路径操作
来源：http://vv.huixiangedu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bc.521024.cn

[U25] Py：CSV 按字典读
来源：http://am.jianghongdianzi.cn

csv.DictReader(f)
来源：http://ad.panjiajie.cn

[U26] Py：并发下载
来源：http://dv.shtwfgs.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wk.jianghongdianzi.cn

[U27] Py：异步 HTTP
来源：http://lf.jctech888.com.cn

aiohttp.ClientSession() 配合 async with
来源：http://ps.szxytkj.cn

[U28] Py：类型别名
来源：http://fk.bookmarksfly.cn

UserId = int
来源：http://zl.nszjky.cn

[U29] Py：属性校验
来源：http://pa.asd995.cn

@property 与 @x.setter 配合
来源：http://sg.yuntaijiaju.cn

[U30] Py：数据类
来源：http://bp.hnjuh.cn

@dataclass(slots=True)
来源：http://rq.wgjwhj.cn

[U31] Py：单测
来源：http://tu.521024.cn

python -m pytest -q
来源：http://jb.bjjhwx.cn

[U32] Py：代码格式化
来源：http://lb.szxytkj.cn

ruff format . && ruff check --fix .
来源：http://zn.gzmigu.cn

[U33] Py：打包发布
来源：http://bk.huanxung.cn

python -m build  （依赖 pyproject.toml）
来源：http://ca.gzmigu.cn

[U34] Py：判断编码
来源：http://uf.huanxung.cn

chardet.detect(raw)
来源：http://gn.shtwfgs.cn

[U35] Py：发送邮件
来源：http://uw.szxytkj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://id.shxzukj.cn

[U36] Py：定时任务
来源：http://ga.huixinmuqiang.cn

schedule.every(10).minutes.do(job)
来源：http://dn.huanxung.cn

[U37] Py：读写 Excel
来源：http://xh.jianghongdianzi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wj.gzmigu.cn

[U38] Py：获取脚本所在目录
来源：http://gk.muxihuayi.cn

Path(__file__).resolve().parent
来源：http://tw.9csxet.cn

[U39] Py：判断是否在交互环境
来源：http://ye.szsharing.cn

sys.stdout.isatty()
来源：http://ou.shxzskj.cn

[U40] Py：打印到标准错误
来源：http://ph.hahajie.cn

print("err", file=sys.stderr)
来源：http://di.yuntaijiaju.cn

[U41] PHP：初始化 Composer 项目
来源：http://fh.wgjwhj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xk.haigaiapp.cn

[U42] PHP：PSR-4 自动加载
来源：http://qv.yuntaijiaju.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zj.jianghongdianzi.cn

[U43] PHP：声明命名空间
来源：http://ej.gzmigu.cn

namespace App\Http;
来源：http://ul.asd995.cn

[U44] PHP：开启严格类型
来源：http://xw.hahajie.cn

declare(strict_types=1);
来源：http://bq.muxihuayi.cn

[U45] PHP：类型声明与返回类型
来源：http://hu.panjiajie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://dd.huixinmuqiang.cn

[U46] PHP：可空类型
来源：http://ah.hnjuh.cn

?string $name = null
来源：http://nz.gzmigu.cn

[U47] PHP：联合类型
来源：http://lz.jianghongdianzi.cn

int|string $id
来源：http://je.9csxet.cn

[U48] PHP：纯枚举
来源：http://hh.lnxyls.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://so.szsharing.cn

[U49] PHP：只读属性
来源：http://nw.yuexingan06.cn

public readonly string $name
来源：http://jz.szsharing.cn

[U50] PHP：构造器属性提升
来源：http://hl.521024.cn

public function __construct(private int $id) {}
来源：http://yn.hnjuh.cn

[U51] PHP：数组解构
来源：http://hj.huanxung.cn

[$a, $b] = $arr;
来源：http://ey.bookmarksfly.cn

[U52] PHP：箭头函数
来源：http://ab.shtwfgs.cn

$double = fn($x) => $x * 2;
来源：http://hl.hnjuh.cn

[U53] PHP：空合并运算符
来源：http://kt.shxzukj.cn

$v = $a ?? $b ?? "default";
来源：http://lm.muxihuayi.cn

[U54] PHP：空安全调用
来源：http://ke.yuntaijiaju.cn

$obj?->method()
来源：http://jr.jianghongdianzi.cn

[U55] PHP：match 表达式
来源：http://uo.nszjky.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jg.haigaiapp.cn

[U56] PHP：命名参数
来源：http://qm.shxzskj.cn

f(a: 1, b: 2)
来源：http://ju.shxzskj.cn

[U57] PHP：字符串插值
来源：http://nd.nszjky.cn

"值: {$a}"
来源：http://om.haigaiapp.cn

[U58] PHP：数组三件套
来源：http://ui.jctech888.com.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pr.hahajie.cn

[U59] PHP：自定义排序
来源：http://wd.shxzukj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wg.haigaiapp.cn

[U60] PHP：JSON 编解码
来源：http://is.bjjhwx.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bg.huanxung.cn

[U61] PHP：正则
来源：http://js.newstarts.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gx.huixiangedu.cn

[U62] PHP：日期对象
来源：http://cr.nicolike.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://aw.shxzskj.cn

[U63] PHP：文件读写
来源：http://yu.hahajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://va.jianghongdianzi.cn

[U64] PHP：目录遍历
来源：http://qk.szsharing.cn

glob("dir/*.php");  scandir("dir");
来源：http://vi.nszjky.cn

[U65] PHP：会话
来源：http://fi.chemitech.net.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://hu.szxytkj.cn

[U66] PHP：设置 Cookie
来源：http://xz.hnjuh.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gu.gzmigu.cn

[U67] PHP：处理文件上传
来源：http://jl.wgjwhj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gq.hahajie.cn

[U68] PHP：PDO 连接
来源：http://zr.9csxet.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ut.yuntaijiaju.cn

[U69] PHP：PDO 预处理
来源：http://lx.shxzskj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wr.panjiajie.cn

[U70] PHP：PDO 事务
来源：http://px.chemitech.net.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lq.yuexingan06.cn

[U71] PHP：抛出异常
来源：http://eu.jianghongdianzi.cn

throw new RuntimeException("失败", 500);
来源：http://co.yuntaijiaju.cn

[U72] PHP：写错误日志
来源：http://am.chemitech.net.cn

error_log("失败: " . $e->getMessage());
来源：http://av.colortex.cn


<!-- 参考信息 -->