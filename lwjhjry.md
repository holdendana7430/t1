代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kc.newstarts.cn

[S51] C++：显式类型转换
来源：http://fi.nicolike.cn

static_cast<double>(a) / b
来源：http://pc.szsharing.cn

[S52] C++：const 与 noexcept
来源：http://tn.gzmigu.cn

int size() const noexcept { return n_; }
来源：http://cl.9csxet.cn

[S53] C++：移动语义
来源：http://ah.newstarts.cn

std::vector<int> w = std::move(v);
来源：http://iz.jianghongdianzi.cn

[S54] C++：异常处理
来源：http://bm.jctech888.com.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gj.szsharing.cn

[S55] C++：结构化绑定
来源：http://dw.shxzukj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cr.jianghongdianzi.cn

[S56] C++：optional
来源：http://vo.szxytkj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lk.shxzskj.cn

[S57] C++：编译期常量
来源：http://lp.colortex.cn

constexpr int N = 10;
来源：http://xm.9csxet.cn

[S58] C++：命名空间
来源：http://ax.shxzskj.cn

namespace ns { int f() { return 1; } }
来源：http://vl.jianghongdianzi.cn

[S59] C++：静态断言
来源：http://ft.lnxyls.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://sb.muxihuayi.cn

[S60] C++：遍历并删除元素
来源：http://af.gzmigu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qr.lnxyls.cn

================================================================================
来源：http://yp.huixiangedu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dh.bjjhwx.cn

================================================================================
来源：http://vv.hnjuh.cn

[T01] Kotlin：Hello World
来源：http://fd.lnxyls.cn

println("Hello")
来源：http://cj.asd995.cn

[T02] Kotlin：变量
来源：http://kq.hahajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xa.chemitech.net.cn

[T03] Kotlin：字符串模板
来源：http://ul.bookmarksfly.cn

"值: $b"
来源：http://bf.colortex.cn

[T04] Kotlin：空安全
来源：http://sq.szsharing.cn

val n: String? = null;  n?.length
来源：http://wu.yuntaijiaju.cn

[T05] Kotlin：when 表达式
来源：http://ci.lnxyls.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://au.chemitech.net.cn

[T06] Kotlin：集合映射
来源：http://rx.hnjuh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ty.chemitech.net.cn

[T07] Kotlin：集合过滤
来源：http://xl.huixiangedu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ax.jctech888.com.cn

[T08] Kotlin：数据类
来源：http://ly.huixinmuqiang.cn

data class User(val name: String, val age: Int)
来源：http://fd.newstarts.cn

[T09] Kotlin：扩展函数
来源：http://pj.newstarts.cn

fun String.exclaim() = this + "!"
来源：http://vb.lnxyls.cn

[T10] Kotlin：默认参数
来源：http://om.shtwfgs.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wi.chemitech.net.cn

[T11] Kotlin：协程
来源：http://fp.colortex.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://he.521024.cn

[T12] Kotlin：解构声明
来源：http://yv.szxytkj.cn

val (a, b) = Pair(1, 2)
来源：http://mw.szsharing.cn

[T13] Kotlin：只读 Map
来源：http://hd.9csxet.cn

val m = mapOf("a" to 1)
来源：http://wj.lnxyls.cn

[T14] Kotlin：循环
来源：http://cn.shtwfgs.cn

for (i in 1..10) println(i)
来源：http://ij.shxzukj.cn

[T15] Kotlin：接口
来源：http://kl.jctech888.com.cn

interface Shape { fun area(): Double }
来源：http://bj.shtwfgs.cn

[T16] Swift：Hello World
来源：http://mx.haigaiapp.cn

print("Hello")
来源：http://bs.wgjwhj.cn

[T17] Swift：变量与常量
来源：http://mj.hahajie.cn

var a = 1;  let b = 2
来源：http://za.huixiangedu.cn

[T18] Swift：字符串插值
来源：http://nv.szsharing.cn

"值: \(b)"
来源：http://vy.yuntaijiaju.cn

[T19] Swift：可选绑定
来源：http://xh.szsharing.cn

if let n = opt { print(n) }
来源：http://zo.panjiajie.cn

[T20] Swift：数组操作
来源：http://mc.nszjky.cn

var a = [1, 2, 3];  a.append(4)
来源：http://dd.panjiajie.cn

[T21] Swift：遍历
来源：http://yv.gzmigu.cn

for x in a { print(x) }
来源：http://ns.huixiangedu.cn

[T22] Swift：字典
来源：http://kz.huanxung.cn

var d = ["a": 1];  d["b"] = 2
来源：http://uj.bjjhwx.cn

[T23] Swift：函数
来源：http://xw.shtwfgs.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cw.lnxyls.cn

[T24] Swift：闭包
来源：http://zo.shtwfgs.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://bf.szsharing.cn

[T25] Swift：结构体
来源：http://dz.szxytkj.cn

struct P { var x: Int }
来源：http://nf.lnxyls.cn

[T26] Swift：类与重写
来源：http://rs.nszjky.cn

class A: Base { override func f() {} }
来源：http://zp.hahajie.cn

[T27] Swift：错误处理
来源：http://cq.jianghongdianzi.cn

do { try f() } catch { print(error) }
来源：http://ua.gzmigu.cn

[T28] Swift：枚举
来源：http://ol.yuexingan06.cn

enum Color { case red, green }
来源：http://uu.shtwfgs.cn

[T29] Swift：guard 提前返回
来源：http://mj.bjjhwx.cn

guard let x = opt else { return }
来源：http://mw.muxihuayi.cn

[T30] Swift：协议
来源：http://pf.bookmarksfly.cn

protocol Shape { func area() -> Double }
来源：http://nv.muxihuayi.cn

[T31] Lua：Hello World
来源：http://io.shtwfgs.cn

print("Hello")
来源：http://te.panjiajie.cn

[T32] Lua：局部变量
来源：http://oq.9csxet.cn

local a = 1
来源：http://we.bjjhwx.cn

[T33] Lua：表（数组）
来源：http://vx.nicolike.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vi.bookmarksfly.cn

[T34] Lua：遍历表
来源：http://xm.wgjwhj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ky.bjjhwx.cn

[T35] Lua：字典表
来源：http://dr.lnxyls.cn

local d = { a = 1 };  d.b = 2
来源：http://hw.521024.cn

[T36] Lua：函数
来源：http://qx.huixiangedu.cn

function add(a, b) return a + b end
来源：http://kv.gzmigu.cn

[T37] Lua：字符串拼接
来源：http://dt.panjiajie.cn

"a" .. "b"
来源：http://mm.hahajie.cn

[T38] Lua：条件
来源：http://qw.hnjuh.cn

if x > 0 then print("正") end
来源：http://rx.huanxung.cn

[T39] Lua：模式匹配
来源：http://da.bookmarksfly.cn

string.find(s, "%d+")
来源：http://fp.shxzukj.cn

[T40] Lua：元表
来源：http://mc.shtwfgs.cn

setmetatable({}, { __index = base })
来源：http://nd.chemitech.net.cn

[T41] Perl：Hello World
来源：http://lx.shtwfgs.cn

print "Hello\n";
来源：http://dc.jianghongdianzi.cn

[T42] Perl：变量类型
来源：http://qk.shxzskj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mx.9csxet.cn

[T43] Perl：字符串插值
来源：http://ly.nszjky.cn

"值: $a"
来源：http://eq.szsharing.cn

[T44] Perl：条件
来源：http://ta.hnjuh.cn

if ($a > 0) { print "正"; }
来源：http://oj.bjjhwx.cn

[T45] Perl：数组遍历
来源：http://su.szsharing.cn

for my $x (@arr) { print $x; }
来源：http://ne.shtwfgs.cn

[T46] Perl：哈希操作
来源：http://sv.huixinmuqiang.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jj.muxihuayi.cn

[T47] Perl：正则捕获
来源：http://ij.panjiajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://bc.shtwfgs.cn

[T48] Perl：正则替换
来源：http://fw.wgjwhj.cn

$s =~ s/old/new/g;
来源：http://ke.muxihuayi.cn

[T49] Perl：函数
来源：http://qh.newstarts.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qd.bookmarksfly.cn

[T50] Perl：逐行读文件
来源：http://jk.muxihuayi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qm.huixiangedu.cn

while (my $line = <$fh>) { print $line; }
来源：http://ka.huixiangedu.cn

[T51] Scala：Hello World
来源：http://jn.haigaiapp.cn

println("Hello")
来源：http://um.huixiangedu.cn

[T52] Scala：变量
来源：http://kk.newstarts.cn

val a = 1;  var b = 2
来源：http://eg.newstarts.cn

[T53] Scala：字符串插值
来源：http://gz.yuexingan06.cn

s"值: $b"
来源：http://tq.huixinmuqiang.cn

[T54] Scala：集合映射
来源：http://ex.huixiangedu.cn

List(1, 2, 3).map(_ * 2)
来源：http://hy.muxihuayi.cn

[T55] Scala：集合过滤
来源：http://vy.yuexingan06.cn

List(1, 2, 3).filter(_ > 1)
来源：http://jq.gzmigu.cn

[T56] Scala：样例类
来源：http://vz.gzmigu.cn

case class User(name: String, age: Int)
来源：http://as.haigaiapp.cn

[T57] Scala：模式匹配
来源：http://ro.shxzukj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://zb.bookmarksfly.cn

[T58] Scala：函数定义
来源：http://ty.chemitech.net.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ts.wgjwhj.cn

[T59] Scala：循环
来源：http://jx.521024.cn

for (i <- 1 to 10) println(i)
来源：http://rd.hahajie.cn

[T60] Scala：折叠
来源：http://vo.nicolike.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pl.bookmarksfly.cn

================================================================================
来源：http://hz.panjiajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zk.gzmigu.cn

================================================================================
来源：http://cx.nszjky.cn

[U01] Py：创建虚拟环境
来源：http://ox.chemitech.net.cn

python -m venv .venv && source .venv/bin/activate
来源：http://xs.hahajie.cn

[U02] Py：导出 / 安装依赖
来源：http://lh.hahajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://je.huanxung.cn

[U03] Py：加载 .env 配置
来源：http://ki.gzmigu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ua.lnxyls.cn

[U04] Py：变量调试打印
来源：http://yc.yuntaijiaju.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jt.muxihuayi.cn

[U05] Py：列表去重且保序
来源：http://ay.chemitech.net.cn

list(dict.fromkeys(arr))
来源：http://ph.nicolike.cn

[U06] Py：合并两个字典
来源：http://yz.yuntaijiaju.cn

{**a, **b}
来源：http://ar.chemitech.net.cn

[U07] Py：反转字典键值
来源：http://lq.chemitech.net.cn

{v: k for k, v in d.items()}
来源：http://au.jctech888.com.cn

[U08] Py：展平二维列表
来源：http://qi.lnxyls.cn

[y for x in nested for y in x]
来源：http://sz.szsharing.cn

[U09] Py：字典取最大值的键
来源：http://ak.521024.cn

max(d, key=d.get)
来源：http://jo.wgjwhj.cn

[U10] Py：按值排序字典
来源：http://ii.hnjuh.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pn.gzmigu.cn

[U11] Py：生成器表达式
来源：http://vq.huanxung.cn

(x * 2 for x in arr)
来源：http://zt.yuntaijiaju.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rc.hahajie.cn

Counter(arr).most_common(3)
来源：http://gj.nicolike.cn

[U13] Py：固定长度队列
来源：http://kn.huanxung.cn

deque(maxlen=10)
来源：http://rj.muxihuayi.cn

[U14] Py：分组收集到列表
来源：http://mt.szxytkj.cn

defaultdict(list)
来源：http://zv.chemitech.net.cn

[U15] Py：高精度计时
来源：http://zu.panjiajie.cn

t = time.perf_counter()
来源：http://sc.huixiangedu.cn

[U16] Py：命令行参数解析
来源：http://hc.bjjhwx.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://up.521024.cn

[U17] Py：初始化日志
来源：http://me.9csxet.cn

logging.basicConfig(level=logging.INFO)
来源：http://zn.shxzskj.cn

[U18] Py：预编译正则
来源：http://mr.lnxyls.cn

pat = re.compile(r"\d+")
来源：http://pe.chemitech.net.cn

[U19] Py：正则替换带回调
来源：http://uq.haigaiapp.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qx.9csxet.cn

[U20] Py：缓存函数结果
来源：http://dt.newstarts.cn

@functools.lru_cache(maxsize=None)
来源：http://xo.colortex.cn

[U21] Py：自定义上下文管理器
来源：http://xu.yuexingan06.cn

@contextlib.contextmanager
来源：http://mg.nszjky.cn

[U22] Py：矩阵转置
来源：http://ku.chemitech.net.cn

list(zip(*m))
来源：http://fa.shtwfgs.cn

[U23] Py：分块读取大文件
来源：http://wg.asd995.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rm.gzmigu.cn

[U24] Py：路径操作
来源：http://ak.colortex.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dq.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://kl.lnxyls.cn

csv.DictReader(f)
来源：http://ye.shxzukj.cn

[U26] Py：并发下载
来源：http://gi.jctech888.com.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zs.shtwfgs.cn

[U27] Py：异步 HTTP
来源：http://ct.huixiangedu.cn

aiohttp.ClientSession() 配合 async with
来源：http://xs.szxytkj.cn

[U28] Py：类型别名
来源：http://zr.jianghongdianzi.cn

UserId = int
来源：http://ty.gzmigu.cn

[U29] Py：属性校验
来源：http://us.jctech888.com.cn

@property 与 @x.setter 配合
来源：http://vi.newstarts.cn

[U30] Py：数据类
来源：http://qy.yuntaijiaju.cn

@dataclass(slots=True)
来源：http://gy.huanxung.cn

[U31] Py：单测
来源：http://cu.hnjuh.cn

python -m pytest -q
来源：http://by.nicolike.cn

[U32] Py：代码格式化
来源：http://ys.nicolike.cn

ruff format . && ruff check --fix .
来源：http://nn.newstarts.cn

[U33] Py：打包发布
来源：http://fp.yuexingan06.cn

python -m build  （依赖 pyproject.toml）
来源：http://mh.wgjwhj.cn

[U34] Py：判断编码
来源：http://du.colortex.cn

chardet.detect(raw)
来源：http://da.nszjky.cn

[U35] Py：发送邮件
来源：http://ys.gzmigu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jq.lnxyls.cn

[U36] Py：定时任务
来源：http://og.jctech888.com.cn

schedule.every(10).minutes.do(job)
来源：http://vt.bjjhwx.cn

[U37] Py：读写 Excel
来源：http://mn.hahajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qh.huanxung.cn

[U38] Py：获取脚本所在目录
来源：http://xj.jianghongdianzi.cn

Path(__file__).resolve().parent
来源：http://sh.wgjwhj.cn

[U39] Py：判断是否在交互环境
来源：http://xl.szsharing.cn

sys.stdout.isatty()
来源：http://st.hahajie.cn

[U40] Py：打印到标准错误
来源：http://fz.521024.cn

print("err", file=sys.stderr)
来源：http://rk.wgjwhj.cn

[U41] PHP：初始化 Composer 项目
来源：http://fq.gzmigu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jl.huixiangedu.cn

[U42] PHP：PSR-4 自动加载
来源：http://qs.newstarts.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zs.huanxung.cn

[U43] PHP：声明命名空间
来源：http://by.9csxet.cn

namespace App\Http;
来源：http://mt.huanxung.cn

[U44] PHP：开启严格类型
来源：http://km.jianghongdianzi.cn

declare(strict_types=1);
来源：http://fo.hnjuh.cn

[U45] PHP：类型声明与返回类型
来源：http://vh.nszjky.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://dw.newstarts.cn

[U46] PHP：可空类型
来源：http://oz.521024.cn

?string $name = null
来源：http://ph.yuexingan06.cn

[U47] PHP：联合类型
来源：http://eg.haigaiapp.cn

int|string $id
来源：http://mo.jianghongdianzi.cn

[U48] PHP：纯枚举
来源：http://lo.521024.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.asd995.cn

[U49] PHP：只读属性
来源：http://so.bjjhwx.cn

public readonly string $name
来源：http://en.wgjwhj.cn

[U50] PHP：构造器属性提升
来源：http://ee.9csxet.cn

public function __construct(private int $id) {}
来源：http://xi.gzmigu.cn

[U51] PHP：数组解构
来源：http://gr.huixiangedu.cn

[$a, $b] = $arr;
来源：http://ch.nszjky.cn

[U52] PHP：箭头函数
来源：http://cp.panjiajie.cn

$double = fn($x) => $x * 2;
来源：http://wk.bookmarksfly.cn

[U53] PHP：空合并运算符
来源：http://by.huixiangedu.cn

$v = $a ?? $b ?? "default";
来源：http://rr.wgjwhj.cn

[U54] PHP：空安全调用
来源：http://gb.gzmigu.cn

$obj?->method()
来源：http://mp.gzmigu.cn

[U55] PHP：match 表达式
来源：http://js.huanxung.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fk.jianghongdianzi.cn

[U56] PHP：命名参数
来源：http://qo.huanxung.cn

f(a: 1, b: 2)
来源：http://gf.9csxet.cn

[U57] PHP：字符串插值
来源：http://ip.9csxet.cn

"值: {$a}"
来源：http://nx.hahajie.cn

[U58] PHP：数组三件套
来源：http://xr.hnjuh.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ct.yuntaijiaju.cn

[U59] PHP：自定义排序
来源：http://gf.yuntaijiaju.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iq.nszjky.cn

[U60] PHP：JSON 编解码
来源：http://fy.huanxung.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://sk.9csxet.cn

[U61] PHP：正则
来源：http://cw.nszjky.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jr.szsharing.cn

[U62] PHP：日期对象
来源：http://dt.nicolike.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lz.szsharing.cn

[U63] PHP：文件读写
来源：http://jl.szxytkj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sy.newstarts.cn

[U64] PHP：目录遍历
来源：http://qx.521024.cn

glob("dir/*.php");  scandir("dir");
来源：http://ul.wgjwhj.cn

[U65] PHP：会话
来源：http://ul.wgjwhj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ui.bjjhwx.cn

[U66] PHP：设置 Cookie
来源：http://nk.yuntaijiaju.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qw.newstarts.cn

[U67] PHP：处理文件上传
来源：http://rg.panjiajie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ut.szxytkj.cn

[U68] PHP：PDO 连接
来源：http://qz.muxihuayi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lm.szsharing.cn

[U69] PHP：PDO 预处理
来源：http://dz.muxihuayi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ei.szsharing.cn

[U70] PHP：PDO 事务
来源：http://gj.shtwfgs.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://el.chemitech.net.cn

[U71] PHP：抛出异常
来源：http://az.yuntaijiaju.cn

throw new RuntimeException("失败", 500);
来源：http://sk.wgjwhj.cn

[U72] PHP：写错误日志
来源：http://tf.colortex.cn

error_log("失败: " . $e->getMessage());
来源：http://rt.muxihuayi.cn

[U73] PHP：读取 ini 配置
来源：http://cb.haigaiapp.cn

parse_ini_file("config.ini", true)
来源：http://dd.lnxyls.cn

[U74] PHP：读取环境变量
来源：http://ff.nszjky.cn

getenv("APP_ENV") ?: "production"
来源：http://bp.yuexingan06.cn

[U75] PHP：依赖注入
来源：http://by.bookmarksfly.cn

composer require psr/container
来源：http://so.jctech888.com.cn

[U76] PHP：简单路由
来源：http://qc.huixiangedu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kt.muxihuayi.cn


<!-- 参考信息 -->