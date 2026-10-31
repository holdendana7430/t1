代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://sq.jctech888.com.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wi.chemitech.net.cn

[S48] C++：逐行读文件
来源：http://ii.newstarts.cn

std::ifstream in("a.txt");  std::string line;
来源：http://cs.wgjwhj.cn

while (std::getline(in, line)) { }
来源：http://bo.szsharing.cn

[S49] C++：写文件
来源：http://cy.chemitech.net.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ta.nszjky.cn

[S50] C++：格式化数字
来源：http://xt.newstarts.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xd.9csxet.cn

[S51] C++：显式类型转换
来源：http://fd.hahajie.cn

static_cast<double>(a) / b
来源：http://mb.lnxyls.cn

[S52] C++：const 与 noexcept
来源：http://kd.hnjuh.cn

int size() const noexcept { return n_; }
来源：http://qj.haigaiapp.cn

[S53] C++：移动语义
来源：http://ss.yuntaijiaju.cn

std::vector<int> w = std::move(v);
来源：http://ta.nszjky.cn

[S54] C++：异常处理
来源：http://pp.wgjwhj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tm.huanxung.cn

[S55] C++：结构化绑定
来源：http://pm.wgjwhj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gl.bookmarksfly.cn

[S56] C++：optional
来源：http://pu.huixiangedu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bv.huanxung.cn

[S57] C++：编译期常量
来源：http://rf.muxihuayi.cn

constexpr int N = 10;
来源：http://no.bookmarksfly.cn

[S58] C++：命名空间
来源：http://cq.szxytkj.cn

namespace ns { int f() { return 1; } }
来源：http://jl.bookmarksfly.cn

[S59] C++：静态断言
来源：http://as.panjiajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dt.szxytkj.cn

[S60] C++：遍历并删除元素
来源：http://qt.newstarts.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jc.hahajie.cn

================================================================================
来源：http://zh.huanxung.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://sp.huixiangedu.cn

================================================================================
来源：http://xl.huixinmuqiang.cn

[T01] Kotlin：Hello World
来源：http://gr.chemitech.net.cn

println("Hello")
来源：http://ej.asd995.cn

[T02] Kotlin：变量
来源：http://zr.521024.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ee.chemitech.net.cn

[T03] Kotlin：字符串模板
来源：http://xm.shxzukj.cn

"值: $b"
来源：http://xl.gzmigu.cn

[T04] Kotlin：空安全
来源：http://oz.panjiajie.cn

val n: String? = null;  n?.length
来源：http://wk.panjiajie.cn

[T05] Kotlin：when 表达式
来源：http://rr.panjiajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fw.bjjhwx.cn

[T06] Kotlin：集合映射
来源：http://vp.shxzukj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://lo.szsharing.cn

[T07] Kotlin：集合过滤
来源：http://wx.nszjky.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wq.colortex.cn

[T08] Kotlin：数据类
来源：http://jl.panjiajie.cn

data class User(val name: String, val age: Int)
来源：http://wt.haigaiapp.cn

[T09] Kotlin：扩展函数
来源：http://hk.shxzukj.cn

fun String.exclaim() = this + "!"
来源：http://hn.shtwfgs.cn

[T10] Kotlin：默认参数
来源：http://nd.szsharing.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://nl.jctech888.com.cn

[T11] Kotlin：协程
来源：http://xc.lnxyls.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://iy.9csxet.cn

[T12] Kotlin：解构声明
来源：http://wc.chemitech.net.cn

val (a, b) = Pair(1, 2)
来源：http://gj.bjjhwx.cn

[T13] Kotlin：只读 Map
来源：http://eo.asd995.cn

val m = mapOf("a" to 1)
来源：http://ts.hnjuh.cn

[T14] Kotlin：循环
来源：http://ie.panjiajie.cn

for (i in 1..10) println(i)
来源：http://dv.nicolike.cn

[T15] Kotlin：接口
来源：http://aa.szsharing.cn

interface Shape { fun area(): Double }
来源：http://ym.hnjuh.cn

[T16] Swift：Hello World
来源：http://pu.9csxet.cn

print("Hello")
来源：http://os.huixiangedu.cn

[T17] Swift：变量与常量
来源：http://ya.jianghongdianzi.cn

var a = 1;  let b = 2
来源：http://vi.panjiajie.cn

[T18] Swift：字符串插值
来源：http://be.muxihuayi.cn

"值: \(b)"
来源：http://he.muxihuayi.cn

[T19] Swift：可选绑定
来源：http://bn.yuntaijiaju.cn

if let n = opt { print(n) }
来源：http://zn.szsharing.cn

[T20] Swift：数组操作
来源：http://cy.hahajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ls.huanxung.cn

[T21] Swift：遍历
来源：http://bc.huixinmuqiang.cn

for x in a { print(x) }
来源：http://ul.bookmarksfly.cn

[T22] Swift：字典
来源：http://vp.asd995.cn

var d = ["a": 1];  d["b"] = 2
来源：http://uu.huixiangedu.cn

[T23] Swift：函数
来源：http://um.haigaiapp.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ql.szsharing.cn

[T24] Swift：闭包
来源：http://zs.yuntaijiaju.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://td.szsharing.cn

[T25] Swift：结构体
来源：http://iu.colortex.cn

struct P { var x: Int }
来源：http://gp.hnjuh.cn

[T26] Swift：类与重写
来源：http://jf.panjiajie.cn

class A: Base { override func f() {} }
来源：http://lq.panjiajie.cn

[T27] Swift：错误处理
来源：http://my.jianghongdianzi.cn

do { try f() } catch { print(error) }
来源：http://kj.szxytkj.cn

[T28] Swift：枚举
来源：http://hs.shxzukj.cn

enum Color { case red, green }
来源：http://jo.hnjuh.cn

[T29] Swift：guard 提前返回
来源：http://mu.gzmigu.cn

guard let x = opt else { return }
来源：http://tp.chemitech.net.cn

[T30] Swift：协议
来源：http://at.shxzukj.cn

protocol Shape { func area() -> Double }
来源：http://so.wgjwhj.cn

[T31] Lua：Hello World
来源：http://mj.newstarts.cn

print("Hello")
来源：http://bz.9csxet.cn

[T32] Lua：局部变量
来源：http://wg.szsharing.cn

local a = 1
来源：http://hv.9csxet.cn

[T33] Lua：表（数组）
来源：http://cp.521024.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://es.nszjky.cn

[T34] Lua：遍历表
来源：http://iq.shxzukj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://yp.9csxet.cn

[T35] Lua：字典表
来源：http://nc.shxzukj.cn

local d = { a = 1 };  d.b = 2
来源：http://mr.bookmarksfly.cn

[T36] Lua：函数
来源：http://fh.bookmarksfly.cn

function add(a, b) return a + b end
来源：http://gg.colortex.cn

[T37] Lua：字符串拼接
来源：http://dt.szsharing.cn

"a" .. "b"
来源：http://zy.gzmigu.cn

[T38] Lua：条件
来源：http://cv.shtwfgs.cn

if x > 0 then print("正") end
来源：http://yh.gzmigu.cn

[T39] Lua：模式匹配
来源：http://go.huixiangedu.cn

string.find(s, "%d+")
来源：http://jr.colortex.cn

[T40] Lua：元表
来源：http://bj.szxytkj.cn

setmetatable({}, { __index = base })
来源：http://zv.jianghongdianzi.cn

[T41] Perl：Hello World
来源：http://ec.hnjuh.cn

print "Hello\n";
来源：http://ih.panjiajie.cn

[T42] Perl：变量类型
来源：http://ee.haigaiapp.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rh.panjiajie.cn

[T43] Perl：字符串插值
来源：http://yi.jianghongdianzi.cn

"值: $a"
来源：http://ma.hahajie.cn

[T44] Perl：条件
来源：http://hj.hnjuh.cn

if ($a > 0) { print "正"; }
来源：http://zz.gzmigu.cn

[T45] Perl：数组遍历
来源：http://ym.haigaiapp.cn

for my $x (@arr) { print $x; }
来源：http://rr.haigaiapp.cn

[T46] Perl：哈希操作
来源：http://lw.szxytkj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ze.gzmigu.cn

[T47] Perl：正则捕获
来源：http://cz.nszjky.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://cq.hnjuh.cn

[T48] Perl：正则替换
来源：http://kn.szsharing.cn

$s =~ s/old/new/g;
来源：http://sh.newstarts.cn

[T49] Perl：函数
来源：http://nj.yuexingan06.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jx.szsharing.cn

[T50] Perl：逐行读文件
来源：http://xx.haigaiapp.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://js.muxihuayi.cn

while (my $line = <$fh>) { print $line; }
来源：http://kn.newstarts.cn

[T51] Scala：Hello World
来源：http://qp.huanxung.cn

println("Hello")
来源：http://kh.huanxung.cn

[T52] Scala：变量
来源：http://hs.shxzskj.cn

val a = 1;  var b = 2
来源：http://bs.bjjhwx.cn

[T53] Scala：字符串插值
来源：http://bx.9csxet.cn

s"值: $b"
来源：http://fp.bookmarksfly.cn

[T54] Scala：集合映射
来源：http://ja.hnjuh.cn

List(1, 2, 3).map(_ * 2)
来源：http://np.huanxung.cn

[T55] Scala：集合过滤
来源：http://qe.szsharing.cn

List(1, 2, 3).filter(_ > 1)
来源：http://hz.hahajie.cn

[T56] Scala：样例类
来源：http://pk.szsharing.cn

case class User(name: String, age: Int)
来源：http://oe.9csxet.cn

[T57] Scala：模式匹配
来源：http://wa.szsharing.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://sc.panjiajie.cn

[T58] Scala：函数定义
来源：http://cn.shxzukj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gl.hahajie.cn

[T59] Scala：循环
来源：http://ar.shxzskj.cn

for (i <- 1 to 10) println(i)
来源：http://sl.huixinmuqiang.cn

[T60] Scala：折叠
来源：http://km.shtwfgs.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://em.szxytkj.cn

================================================================================
来源：http://ec.panjiajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rq.newstarts.cn

================================================================================
来源：http://td.muxihuayi.cn

[U01] Py：创建虚拟环境
来源：http://je.asd995.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ol.hnjuh.cn

[U02] Py：导出 / 安装依赖
来源：http://la.jianghongdianzi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cb.huixinmuqiang.cn

[U03] Py：加载 .env 配置
来源：http://ka.szsharing.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://jr.yuntaijiaju.cn

[U04] Py：变量调试打印
来源：http://lw.nicolike.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wk.haigaiapp.cn

[U05] Py：列表去重且保序
来源：http://gg.lnxyls.cn

list(dict.fromkeys(arr))
来源：http://xs.huixiangedu.cn

[U06] Py：合并两个字典
来源：http://yj.shxzukj.cn

{**a, **b}
来源：http://de.hahajie.cn

[U07] Py：反转字典键值
来源：http://qr.hahajie.cn

{v: k for k, v in d.items()}
来源：http://mn.huixiangedu.cn

[U08] Py：展平二维列表
来源：http://wq.nicolike.cn

[y for x in nested for y in x]
来源：http://hc.huixinmuqiang.cn

[U09] Py：字典取最大值的键
来源：http://nj.newstarts.cn

max(d, key=d.get)
来源：http://lc.yuntaijiaju.cn

[U10] Py：按值排序字典
来源：http://yv.muxihuayi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://px.shxzskj.cn

[U11] Py：生成器表达式
来源：http://dz.jianghongdianzi.cn

(x * 2 for x in arr)
来源：http://uu.bjjhwx.cn

[U12] Py：取出现最多的 3 个元素
来源：http://yx.haigaiapp.cn

Counter(arr).most_common(3)
来源：http://th.nszjky.cn

[U13] Py：固定长度队列
来源：http://vj.colortex.cn

deque(maxlen=10)
来源：http://mm.asd995.cn

[U14] Py：分组收集到列表
来源：http://zv.huixiangedu.cn

defaultdict(list)
来源：http://nc.hahajie.cn

[U15] Py：高精度计时
来源：http://gx.jctech888.com.cn

t = time.perf_counter()
来源：http://gl.haigaiapp.cn

[U16] Py：命令行参数解析
来源：http://mv.colortex.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://oh.hnjuh.cn

[U17] Py：初始化日志
来源：http://nz.shtwfgs.cn

logging.basicConfig(level=logging.INFO)
来源：http://tc.bjjhwx.cn

[U18] Py：预编译正则
来源：http://bm.yuexingan06.cn

pat = re.compile(r"\d+")
来源：http://bz.yuntaijiaju.cn

[U19] Py：正则替换带回调
来源：http://jh.lnxyls.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jo.newstarts.cn

[U20] Py：缓存函数结果
来源：http://zj.jianghongdianzi.cn

@functools.lru_cache(maxsize=None)
来源：http://ka.hahajie.cn

[U21] Py：自定义上下文管理器
来源：http://fq.jctech888.com.cn

@contextlib.contextmanager
来源：http://my.panjiajie.cn

[U22] Py：矩阵转置
来源：http://vw.panjiajie.cn

list(zip(*m))
来源：http://el.chemitech.net.cn

[U23] Py：分块读取大文件
来源：http://mh.shtwfgs.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mn.yuntaijiaju.cn

[U24] Py：路径操作
来源：http://rn.haigaiapp.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ww.szsharing.cn

[U25] Py：CSV 按字典读
来源：http://yq.hnjuh.cn

csv.DictReader(f)
来源：http://el.shxzukj.cn

[U26] Py：并发下载
来源：http://ge.521024.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wk.asd995.cn

[U27] Py：异步 HTTP
来源：http://px.newstarts.cn

aiohttp.ClientSession() 配合 async with
来源：http://ts.bookmarksfly.cn

[U28] Py：类型别名
来源：http://oa.newstarts.cn

UserId = int
来源：http://mc.huanxung.cn

[U29] Py：属性校验
来源：http://yy.szsharing.cn

@property 与 @x.setter 配合
来源：http://wg.haigaiapp.cn

[U30] Py：数据类
来源：http://ww.9csxet.cn

@dataclass(slots=True)
来源：http://ro.nicolike.cn

[U31] Py：单测
来源：http://la.hahajie.cn

python -m pytest -q
来源：http://fg.muxihuayi.cn

[U32] Py：代码格式化
来源：http://rs.jctech888.com.cn

ruff format . && ruff check --fix .
来源：http://hh.shxzskj.cn

[U33] Py：打包发布
来源：http://mi.wgjwhj.cn

python -m build  （依赖 pyproject.toml）
来源：http://jj.colortex.cn

[U34] Py：判断编码
来源：http://on.newstarts.cn

chardet.detect(raw)
来源：http://oz.shxzskj.cn

[U35] Py：发送邮件
来源：http://ne.jianghongdianzi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yo.jianghongdianzi.cn

[U36] Py：定时任务
来源：http://dr.nszjky.cn

schedule.every(10).minutes.do(job)
来源：http://jj.wgjwhj.cn

[U37] Py：读写 Excel
来源：http://ir.huixiangedu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://sw.lnxyls.cn

[U38] Py：获取脚本所在目录
来源：http://ul.bjjhwx.cn

Path(__file__).resolve().parent
来源：http://ou.shxzukj.cn

[U39] Py：判断是否在交互环境
来源：http://mo.huixinmuqiang.cn

sys.stdout.isatty()
来源：http://ny.hahajie.cn

[U40] Py：打印到标准错误
来源：http://ni.muxihuayi.cn

print("err", file=sys.stderr)
来源：http://qb.lnxyls.cn

[U41] PHP：初始化 Composer 项目
来源：http://al.shxzukj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xi.lnxyls.cn

[U42] PHP：PSR-4 自动加载
来源：http://ht.szxytkj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://uy.hnjuh.cn

[U43] PHP：声明命名空间
来源：http://al.nszjky.cn

namespace App\Http;
来源：http://bx.muxihuayi.cn

[U44] PHP：开启严格类型
来源：http://mw.yuexingan06.cn

declare(strict_types=1);
来源：http://ia.newstarts.cn

[U45] PHP：类型声明与返回类型
来源：http://vd.huanxung.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://un.colortex.cn

[U46] PHP：可空类型
来源：http://cv.yuntaijiaju.cn

?string $name = null
来源：http://yz.shxzskj.cn

[U47] PHP：联合类型
来源：http://nh.huanxung.cn

int|string $id
来源：http://km.wgjwhj.cn

[U48] PHP：纯枚举
来源：http://ln.hahajie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ld.nszjky.cn

[U49] PHP：只读属性
来源：http://ba.yuntaijiaju.cn

public readonly string $name
来源：http://cn.huixinmuqiang.cn

[U50] PHP：构造器属性提升
来源：http://ko.bjjhwx.cn

public function __construct(private int $id) {}
来源：http://oq.chemitech.net.cn

[U51] PHP：数组解构
来源：http://yz.hnjuh.cn

[$a, $b] = $arr;
来源：http://yy.newstarts.cn

[U52] PHP：箭头函数
来源：http://ll.szsharing.cn

$double = fn($x) => $x * 2;
来源：http://tr.yuexingan06.cn

[U53] PHP：空合并运算符
来源：http://zy.bookmarksfly.cn

$v = $a ?? $b ?? "default";
来源：http://ij.huixiangedu.cn

[U54] PHP：空安全调用
来源：http://vo.9csxet.cn

$obj?->method()
来源：http://jw.gzmigu.cn

[U55] PHP：match 表达式
来源：http://da.yuntaijiaju.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zj.huixiangedu.cn

[U56] PHP：命名参数
来源：http://jn.gzmigu.cn

f(a: 1, b: 2)
来源：http://nu.shtwfgs.cn

[U57] PHP：字符串插值
来源：http://vu.huixinmuqiang.cn

"值: {$a}"
来源：http://ut.9csxet.cn

[U58] PHP：数组三件套
来源：http://am.shxzskj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fz.shxzskj.cn

[U59] PHP：自定义排序
来源：http://ds.jianghongdianzi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wp.yuntaijiaju.cn

[U60] PHP：JSON 编解码
来源：http://wq.chemitech.net.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vv.haigaiapp.cn

[U61] PHP：正则
来源：http://us.lnxyls.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mx.shxzskj.cn

[U62] PHP：日期对象
来源：http://vk.bjjhwx.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gn.szxytkj.cn

[U63] PHP：文件读写
来源：http://rh.shtwfgs.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ga.szxytkj.cn

[U64] PHP：目录遍历
来源：http://si.asd995.cn

glob("dir/*.php");  scandir("dir");
来源：http://zv.panjiajie.cn

[U65] PHP：会话
来源：http://di.asd995.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ji.nszjky.cn

[U66] PHP：设置 Cookie
来源：http://jo.huanxung.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cf.shtwfgs.cn

[U67] PHP：处理文件上传
来源：http://lp.szxytkj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://oy.colortex.cn

[U68] PHP：PDO 连接
来源：http://ox.haigaiapp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://si.hnjuh.cn

[U69] PHP：PDO 预处理
来源：http://qe.szxytkj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rp.9csxet.cn

[U70] PHP：PDO 事务
来源：http://tu.haigaiapp.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://oe.huixiangedu.cn

[U71] PHP：抛出异常
来源：http://md.bookmarksfly.cn

throw new RuntimeException("失败", 500);
来源：http://sq.huanxung.cn

[U72] PHP：写错误日志
来源：http://vc.shtwfgs.cn

error_log("失败: " . $e->getMessage());
来源：http://hf.muxihuayi.cn


<!-- 参考信息 -->