代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://if.huixinmuqiang.cn

[S59] C++：静态断言
来源：http://uu.shxzskj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://md.panjiajie.cn

[S60] C++：遍历并删除元素
来源：http://tr.gzmigu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qe.huixiangedu.cn

================================================================================
来源：http://ju.chemitech.net.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gs.shxzskj.cn

================================================================================
来源：http://hb.yuexingan06.cn

[T01] Kotlin：Hello World
来源：http://ps.9csxet.cn

println("Hello")
来源：http://kf.shxzukj.cn

[T02] Kotlin：变量
来源：http://bw.yuexingan06.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zv.9csxet.cn

[T03] Kotlin：字符串模板
来源：http://ph.hnjuh.cn

"值: $b"
来源：http://yq.muxihuayi.cn

[T04] Kotlin：空安全
来源：http://tk.yuntaijiaju.cn

val n: String? = null;  n?.length
来源：http://js.yuntaijiaju.cn

[T05] Kotlin：when 表达式
来源：http://no.wgjwhj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xn.wgjwhj.cn

[T06] Kotlin：集合映射
来源：http://xk.huixiangedu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://kv.yuexingan06.cn

[T07] Kotlin：集合过滤
来源：http://rh.lnxyls.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ll.szxytkj.cn

[T08] Kotlin：数据类
来源：http://js.chemitech.net.cn

data class User(val name: String, val age: Int)
来源：http://on.gzmigu.cn

[T09] Kotlin：扩展函数
来源：http://or.newstarts.cn

fun String.exclaim() = this + "!"
来源：http://ww.9csxet.cn

[T10] Kotlin：默认参数
来源：http://ly.huixinmuqiang.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://sz.shtwfgs.cn

[T11] Kotlin：协程
来源：http://mw.521024.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ia.9csxet.cn

[T12] Kotlin：解构声明
来源：http://lt.bookmarksfly.cn

val (a, b) = Pair(1, 2)
来源：http://re.521024.cn

[T13] Kotlin：只读 Map
来源：http://cr.shxzukj.cn

val m = mapOf("a" to 1)
来源：http://wf.lnxyls.cn

[T14] Kotlin：循环
来源：http://sr.szxytkj.cn

for (i in 1..10) println(i)
来源：http://hm.hnjuh.cn

[T15] Kotlin：接口
来源：http://eq.521024.cn

interface Shape { fun area(): Double }
来源：http://sb.shtwfgs.cn

[T16] Swift：Hello World
来源：http://ml.szsharing.cn

print("Hello")
来源：http://aw.bookmarksfly.cn

[T17] Swift：变量与常量
来源：http://xl.bookmarksfly.cn

var a = 1;  let b = 2
来源：http://vt.jianghongdianzi.cn

[T18] Swift：字符串插值
来源：http://tb.shxzskj.cn

"值: \(b)"
来源：http://vu.newstarts.cn

[T19] Swift：可选绑定
来源：http://pf.yuntaijiaju.cn

if let n = opt { print(n) }
来源：http://gl.521024.cn

[T20] Swift：数组操作
来源：http://cs.shxzukj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://id.lnxyls.cn

[T21] Swift：遍历
来源：http://cj.szxytkj.cn

for x in a { print(x) }
来源：http://bo.shxzukj.cn

[T22] Swift：字典
来源：http://hb.haigaiapp.cn

var d = ["a": 1];  d["b"] = 2
来源：http://rd.shxzukj.cn

[T23] Swift：函数
来源：http://mk.huixiangedu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qt.newstarts.cn

[T24] Swift：闭包
来源：http://gj.shxzskj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://kn.yuntaijiaju.cn

[T25] Swift：结构体
来源：http://ys.szxytkj.cn

struct P { var x: Int }
来源：http://wk.521024.cn

[T26] Swift：类与重写
来源：http://pl.asd995.cn

class A: Base { override func f() {} }
来源：http://jz.wgjwhj.cn

[T27] Swift：错误处理
来源：http://gf.colortex.cn

do { try f() } catch { print(error) }
来源：http://kv.bookmarksfly.cn

[T28] Swift：枚举
来源：http://fl.newstarts.cn

enum Color { case red, green }
来源：http://pq.shxzukj.cn

[T29] Swift：guard 提前返回
来源：http://ff.jianghongdianzi.cn

guard let x = opt else { return }
来源：http://ib.muxihuayi.cn

[T30] Swift：协议
来源：http://co.bookmarksfly.cn

protocol Shape { func area() -> Double }
来源：http://ft.huixiangedu.cn

[T31] Lua：Hello World
来源：http://rc.chemitech.net.cn

print("Hello")
来源：http://fi.shxzskj.cn

[T32] Lua：局部变量
来源：http://me.jctech888.com.cn

local a = 1
来源：http://he.hahajie.cn

[T33] Lua：表（数组）
来源：http://in.lnxyls.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://mg.521024.cn

[T34] Lua：遍历表
来源：http://kb.hnjuh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://oc.huixinmuqiang.cn

[T35] Lua：字典表
来源：http://xc.lnxyls.cn

local d = { a = 1 };  d.b = 2
来源：http://vi.hahajie.cn

[T36] Lua：函数
来源：http://wr.muxihuayi.cn

function add(a, b) return a + b end
来源：http://dq.9csxet.cn

[T37] Lua：字符串拼接
来源：http://oo.nicolike.cn

"a" .. "b"
来源：http://ya.szsharing.cn

[T38] Lua：条件
来源：http://pa.shtwfgs.cn

if x > 0 then print("正") end
来源：http://ln.nszjky.cn

[T39] Lua：模式匹配
来源：http://jf.bjjhwx.cn

string.find(s, "%d+")
来源：http://bz.szsharing.cn

[T40] Lua：元表
来源：http://ub.chemitech.net.cn

setmetatable({}, { __index = base })
来源：http://ms.nszjky.cn

[T41] Perl：Hello World
来源：http://gf.521024.cn

print "Hello\n";
来源：http://yf.nicolike.cn

[T42] Perl：变量类型
来源：http://ud.yuexingan06.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ma.hahajie.cn

[T43] Perl：字符串插值
来源：http://vk.nicolike.cn

"值: $a"
来源：http://lz.bjjhwx.cn

[T44] Perl：条件
来源：http://ra.yuexingan06.cn

if ($a > 0) { print "正"; }
来源：http://bg.chemitech.net.cn

[T45] Perl：数组遍历
来源：http://ea.nszjky.cn

for my $x (@arr) { print $x; }
来源：http://eg.shtwfgs.cn

[T46] Perl：哈希操作
来源：http://eq.asd995.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mr.lnxyls.cn

[T47] Perl：正则捕获
来源：http://hz.hahajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://bf.lnxyls.cn

[T48] Perl：正则替换
来源：http://db.haigaiapp.cn

$s =~ s/old/new/g;
来源：http://po.gzmigu.cn

[T49] Perl：函数
来源：http://mj.huixiangedu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pg.szsharing.cn

[T50] Perl：逐行读文件
来源：http://sn.panjiajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://lk.bookmarksfly.cn

while (my $line = <$fh>) { print $line; }
来源：http://wd.yuexingan06.cn

[T51] Scala：Hello World
来源：http://cw.chemitech.net.cn

println("Hello")
来源：http://qp.bjjhwx.cn

[T52] Scala：变量
来源：http://bu.yuntaijiaju.cn

val a = 1;  var b = 2
来源：http://dq.colortex.cn

[T53] Scala：字符串插值
来源：http://qf.521024.cn

s"值: $b"
来源：http://kq.huixiangedu.cn

[T54] Scala：集合映射
来源：http://iq.jianghongdianzi.cn

List(1, 2, 3).map(_ * 2)
来源：http://as.bjjhwx.cn

[T55] Scala：集合过滤
来源：http://qo.muxihuayi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xo.huixiangedu.cn

[T56] Scala：样例类
来源：http://gq.szxytkj.cn

case class User(name: String, age: Int)
来源：http://ni.gzmigu.cn

[T57] Scala：模式匹配
来源：http://sz.muxihuayi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fy.haigaiapp.cn

[T58] Scala：函数定义
来源：http://fs.jianghongdianzi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://pd.yuexingan06.cn

[T59] Scala：循环
来源：http://pu.huixinmuqiang.cn

for (i <- 1 to 10) println(i)
来源：http://jj.chemitech.net.cn

[T60] Scala：折叠
来源：http://wg.huixinmuqiang.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ub.huixinmuqiang.cn

================================================================================
来源：http://qm.colortex.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://py.chemitech.net.cn

================================================================================
来源：http://as.szsharing.cn

[U01] Py：创建虚拟环境
来源：http://wr.bookmarksfly.cn

python -m venv .venv && source .venv/bin/activate
来源：http://rx.bjjhwx.cn

[U02] Py：导出 / 安装依赖
来源：http://am.panjiajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fh.yuntaijiaju.cn

[U03] Py：加载 .env 配置
来源：http://if.haigaiapp.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://va.9csxet.cn

[U04] Py：变量调试打印
来源：http://zb.521024.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bf.huixiangedu.cn

[U05] Py：列表去重且保序
来源：http://ir.wgjwhj.cn

list(dict.fromkeys(arr))
来源：http://xn.haigaiapp.cn

[U06] Py：合并两个字典
来源：http://tu.chemitech.net.cn

{**a, **b}
来源：http://xr.newstarts.cn

[U07] Py：反转字典键值
来源：http://uv.shxzukj.cn

{v: k for k, v in d.items()}
来源：http://ob.9csxet.cn

[U08] Py：展平二维列表
来源：http://jh.521024.cn

[y for x in nested for y in x]
来源：http://kj.shxzskj.cn

[U09] Py：字典取最大值的键
来源：http://da.lnxyls.cn

max(d, key=d.get)
来源：http://ri.jctech888.com.cn

[U10] Py：按值排序字典
来源：http://wq.hahajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kz.chemitech.net.cn

[U11] Py：生成器表达式
来源：http://wx.asd995.cn

(x * 2 for x in arr)
来源：http://so.huanxung.cn

[U12] Py：取出现最多的 3 个元素
来源：http://yq.shxzskj.cn

Counter(arr).most_common(3)
来源：http://wc.muxihuayi.cn

[U13] Py：固定长度队列
来源：http://eu.szxytkj.cn

deque(maxlen=10)
来源：http://in.shxzskj.cn

[U14] Py：分组收集到列表
来源：http://gl.nicolike.cn

defaultdict(list)
来源：http://ji.nszjky.cn

[U15] Py：高精度计时
来源：http://ym.shxzukj.cn

t = time.perf_counter()
来源：http://ju.panjiajie.cn

[U16] Py：命令行参数解析
来源：http://yx.huanxung.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xp.chemitech.net.cn

[U17] Py：初始化日志
来源：http://ti.bjjhwx.cn

logging.basicConfig(level=logging.INFO)
来源：http://ct.9csxet.cn

[U18] Py：预编译正则
来源：http://jr.szsharing.cn

pat = re.compile(r"\d+")
来源：http://et.bjjhwx.cn

[U19] Py：正则替换带回调
来源：http://xe.haigaiapp.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ea.panjiajie.cn

[U20] Py：缓存函数结果
来源：http://ey.jctech888.com.cn

@functools.lru_cache(maxsize=None)
来源：http://zw.nicolike.cn

[U21] Py：自定义上下文管理器
来源：http://ob.yuexingan06.cn

@contextlib.contextmanager
来源：http://ye.yuexingan06.cn

[U22] Py：矩阵转置
来源：http://fi.newstarts.cn

list(zip(*m))
来源：http://jk.huixinmuqiang.cn

[U23] Py：分块读取大文件
来源：http://kh.newstarts.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ei.jianghongdianzi.cn

[U24] Py：路径操作
来源：http://gz.colortex.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://eg.huixiangedu.cn

[U25] Py：CSV 按字典读
来源：http://sb.shxzukj.cn

csv.DictReader(f)
来源：http://kn.shxzukj.cn

[U26] Py：并发下载
来源：http://nm.nicolike.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://el.lnxyls.cn

[U27] Py：异步 HTTP
来源：http://oy.muxihuayi.cn

aiohttp.ClientSession() 配合 async with
来源：http://as.yuexingan06.cn

[U28] Py：类型别名
来源：http://kg.huixinmuqiang.cn

UserId = int
来源：http://ny.521024.cn

[U29] Py：属性校验
来源：http://ti.wgjwhj.cn

@property 与 @x.setter 配合
来源：http://tk.shxzukj.cn

[U30] Py：数据类
来源：http://ln.gzmigu.cn

@dataclass(slots=True)
来源：http://zv.jctech888.com.cn

[U31] Py：单测
来源：http://pg.haigaiapp.cn

python -m pytest -q
来源：http://sv.huixiangedu.cn

[U32] Py：代码格式化
来源：http://pm.9csxet.cn

ruff format . && ruff check --fix .
来源：http://kr.panjiajie.cn

[U33] Py：打包发布
来源：http://cz.bjjhwx.cn

python -m build  （依赖 pyproject.toml）
来源：http://pj.szsharing.cn

[U34] Py：判断编码
来源：http://db.wgjwhj.cn

chardet.detect(raw)
来源：http://hw.yuntaijiaju.cn

[U35] Py：发送邮件
来源：http://xp.chemitech.net.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://af.yuntaijiaju.cn

[U36] Py：定时任务
来源：http://ph.gzmigu.cn

schedule.every(10).minutes.do(job)
来源：http://um.hahajie.cn

[U37] Py：读写 Excel
来源：http://ep.wgjwhj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wk.yuntaijiaju.cn

[U38] Py：获取脚本所在目录
来源：http://la.colortex.cn

Path(__file__).resolve().parent
来源：http://ws.chemitech.net.cn

[U39] Py：判断是否在交互环境
来源：http://lv.bjjhwx.cn

sys.stdout.isatty()
来源：http://dv.wgjwhj.cn

[U40] Py：打印到标准错误
来源：http://gx.panjiajie.cn

print("err", file=sys.stderr)
来源：http://yw.bookmarksfly.cn

[U41] PHP：初始化 Composer 项目
来源：http://rg.shxzskj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://vl.hahajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://ta.lnxyls.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qv.hnjuh.cn

[U43] PHP：声明命名空间
来源：http://eq.newstarts.cn

namespace App\Http;
来源：http://rx.huanxung.cn

[U44] PHP：开启严格类型
来源：http://ee.wgjwhj.cn

declare(strict_types=1);
来源：http://ii.shxzukj.cn

[U45] PHP：类型声明与返回类型
来源：http://bg.lnxyls.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://pi.wgjwhj.cn

[U46] PHP：可空类型
来源：http://gg.shtwfgs.cn

?string $name = null
来源：http://by.hahajie.cn

[U47] PHP：联合类型
来源：http://jw.yuntaijiaju.cn

int|string $id
来源：http://ym.jctech888.com.cn

[U48] PHP：纯枚举
来源：http://ea.shtwfgs.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cq.jctech888.com.cn

[U49] PHP：只读属性
来源：http://cx.huixiangedu.cn

public readonly string $name
来源：http://ci.9csxet.cn

[U50] PHP：构造器属性提升
来源：http://bk.huixinmuqiang.cn

public function __construct(private int $id) {}
来源：http://sd.wgjwhj.cn

[U51] PHP：数组解构
来源：http://ad.asd995.cn

[$a, $b] = $arr;
来源：http://ej.shxzukj.cn

[U52] PHP：箭头函数
来源：http://iz.muxihuayi.cn

$double = fn($x) => $x * 2;
来源：http://ky.jianghongdianzi.cn

[U53] PHP：空合并运算符
来源：http://vj.panjiajie.cn

$v = $a ?? $b ?? "default";
来源：http://ko.shxzukj.cn

[U54] PHP：空安全调用
来源：http://kx.newstarts.cn

$obj?->method()
来源：http://zq.haigaiapp.cn

[U55] PHP：match 表达式
来源：http://bj.bookmarksfly.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uc.chemitech.net.cn

[U56] PHP：命名参数
来源：http://cw.szxytkj.cn

f(a: 1, b: 2)
来源：http://cw.newstarts.cn

[U57] PHP：字符串插值
来源：http://hh.hahajie.cn

"值: {$a}"
来源：http://ob.hnjuh.cn

[U58] PHP：数组三件套
来源：http://jl.bookmarksfly.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ba.shtwfgs.cn

[U59] PHP：自定义排序
来源：http://fi.shtwfgs.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xn.jianghongdianzi.cn

[U60] PHP：JSON 编解码
来源：http://dp.muxihuayi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://je.hnjuh.cn

[U61] PHP：正则
来源：http://dq.szsharing.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ep.gzmigu.cn

[U62] PHP：日期对象
来源：http://rk.colortex.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ji.521024.cn

[U63] PHP：文件读写
来源：http://gs.panjiajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pe.hahajie.cn

[U64] PHP：目录遍历
来源：http://gf.nszjky.cn

glob("dir/*.php");  scandir("dir");
来源：http://ay.521024.cn

[U65] PHP：会话
来源：http://pk.yuntaijiaju.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rm.huanxung.cn

[U66] PHP：设置 Cookie
来源：http://bs.shxzukj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://eq.shxzskj.cn

[U67] PHP：处理文件上传
来源：http://rm.colortex.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://iv.haigaiapp.cn

[U68] PHP：PDO 连接
来源：http://uw.shxzukj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cv.shxzukj.cn

[U69] PHP：PDO 预处理
来源：http://hb.colortex.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ja.haigaiapp.cn

[U70] PHP：PDO 事务
来源：http://vg.shxzskj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yv.bjjhwx.cn

[U71] PHP：抛出异常
来源：http://jr.asd995.cn

throw new RuntimeException("失败", 500);
来源：http://sl.shxzskj.cn

[U72] PHP：写错误日志
来源：http://oi.shxzukj.cn

error_log("失败: " . $e->getMessage());
来源：http://mp.szxytkj.cn

[U73] PHP：读取 ini 配置
来源：http://ps.szsharing.cn

parse_ini_file("config.ini", true)
来源：http://vr.huixinmuqiang.cn

[U74] PHP：读取环境变量
来源：http://ne.hnjuh.cn

getenv("APP_ENV") ?: "production"
来源：http://bd.huanxung.cn

[U75] PHP：依赖注入
来源：http://qu.huixinmuqiang.cn

composer require psr/container
来源：http://iu.bookmarksfly.cn

[U76] PHP：简单路由
来源：http://gc.yuntaijiaju.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bq.shxzskj.cn

[U77] PHP：模板渲染
来源：http://is.nszjky.cn

composer require twig/twig
来源：http://cd.bjjhwx.cn

[U78] PHP：单元测试
来源：http://nt.chemitech.net.cn

composer require --dev phpunit/phpunit
来源：http://ns.szsharing.cn

[U79] PHP：静态分析
来源：http://ab.521024.cn

composer require --dev phpstan/phpstan
来源：http://uz.chemitech.net.cn

[U80] PHP：代码规范修复
来源：http://ut.bookmarksfly.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://th.haigaiapp.cn

[U81] JS：初始化项目
来源：http://me.huixinmuqiang.cn

npm init -y;  npm i express
来源：http://jz.bookmarksfly.cn

[U82] JS：package.json 脚本
来源：http://sb.haigaiapp.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jk.nszjky.cn

[U83] JS：ES Module 导入导出
来源：http://fb.panjiajie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qd.shxzskj.cn

[U84] JS：CommonJS 写法
来源：http://si.9csxet.cn

module.exports = { a };  const { a } = require("./m");
来源：http://uh.colortex.cn


<!-- 参考信息 -->