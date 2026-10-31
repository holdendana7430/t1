代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kb.szxytkj.cn

[S57] C++：编译期常量
来源：http://wk.newstarts.cn

constexpr int N = 10;
来源：http://rl.chemitech.net.cn

[S58] C++：命名空间
来源：http://ml.bjjhwx.cn

namespace ns { int f() { return 1; } }
来源：http://er.szsharing.cn

[S59] C++：静态断言
来源：http://rj.gzmigu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zt.521024.cn

[S60] C++：遍历并删除元素
来源：http://yg.panjiajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sv.hnjuh.cn

================================================================================
来源：http://wc.shtwfgs.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mi.huanxung.cn

================================================================================
来源：http://di.muxihuayi.cn

[T01] Kotlin：Hello World
来源：http://vv.jianghongdianzi.cn

println("Hello")
来源：http://ch.haigaiapp.cn

[T02] Kotlin：变量
来源：http://xe.chemitech.net.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pn.521024.cn

[T03] Kotlin：字符串模板
来源：http://wi.huixiangedu.cn

"值: $b"
来源：http://uk.haigaiapp.cn

[T04] Kotlin：空安全
来源：http://rx.chemitech.net.cn

val n: String? = null;  n?.length
来源：http://na.hahajie.cn

[T05] Kotlin：when 表达式
来源：http://mn.huanxung.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://eb.colortex.cn

[T06] Kotlin：集合映射
来源：http://ej.9csxet.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://lj.haigaiapp.cn

[T07] Kotlin：集合过滤
来源：http://eu.haigaiapp.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://th.huanxung.cn

[T08] Kotlin：数据类
来源：http://tb.nszjky.cn

data class User(val name: String, val age: Int)
来源：http://nb.gzmigu.cn

[T09] Kotlin：扩展函数
来源：http://cp.shxzskj.cn

fun String.exclaim() = this + "!"
来源：http://xl.szxytkj.cn

[T10] Kotlin：默认参数
来源：http://mt.huixiangedu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://oi.nszjky.cn

[T11] Kotlin：协程
来源：http://xb.521024.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://sa.yuexingan06.cn

[T12] Kotlin：解构声明
来源：http://vx.szsharing.cn

val (a, b) = Pair(1, 2)
来源：http://rc.bjjhwx.cn

[T13] Kotlin：只读 Map
来源：http://ll.muxihuayi.cn

val m = mapOf("a" to 1)
来源：http://su.hnjuh.cn

[T14] Kotlin：循环
来源：http://wi.huixinmuqiang.cn

for (i in 1..10) println(i)
来源：http://li.colortex.cn

[T15] Kotlin：接口
来源：http://hk.szsharing.cn

interface Shape { fun area(): Double }
来源：http://it.huixiangedu.cn

[T16] Swift：Hello World
来源：http://mx.shtwfgs.cn

print("Hello")
来源：http://kb.bjjhwx.cn

[T17] Swift：变量与常量
来源：http://dh.colortex.cn

var a = 1;  let b = 2
来源：http://bz.hnjuh.cn

[T18] Swift：字符串插值
来源：http://qv.hahajie.cn

"值: \(b)"
来源：http://va.huixinmuqiang.cn

[T19] Swift：可选绑定
来源：http://au.huixiangedu.cn

if let n = opt { print(n) }
来源：http://db.wgjwhj.cn

[T20] Swift：数组操作
来源：http://fv.yuntaijiaju.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fp.jianghongdianzi.cn

[T21] Swift：遍历
来源：http://ya.wgjwhj.cn

for x in a { print(x) }
来源：http://tm.huixiangedu.cn

[T22] Swift：字典
来源：http://is.hahajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://tq.huanxung.cn

[T23] Swift：函数
来源：http://pp.chemitech.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fn.muxihuayi.cn

[T24] Swift：闭包
来源：http://lh.9csxet.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://wa.lnxyls.cn

[T25] Swift：结构体
来源：http://ii.yuntaijiaju.cn

struct P { var x: Int }
来源：http://ho.jctech888.com.cn

[T26] Swift：类与重写
来源：http://lp.asd995.cn

class A: Base { override func f() {} }
来源：http://vs.newstarts.cn

[T27] Swift：错误处理
来源：http://ev.bookmarksfly.cn

do { try f() } catch { print(error) }
来源：http://gq.shxzskj.cn

[T28] Swift：枚举
来源：http://zb.asd995.cn

enum Color { case red, green }
来源：http://qz.yuexingan06.cn

[T29] Swift：guard 提前返回
来源：http://ti.jctech888.com.cn

guard let x = opt else { return }
来源：http://at.huixiangedu.cn

[T30] Swift：协议
来源：http://lw.colortex.cn

protocol Shape { func area() -> Double }
来源：http://nl.asd995.cn

[T31] Lua：Hello World
来源：http://lg.asd995.cn

print("Hello")
来源：http://cz.9csxet.cn

[T32] Lua：局部变量
来源：http://nr.gzmigu.cn

local a = 1
来源：http://uh.panjiajie.cn

[T33] Lua：表（数组）
来源：http://ko.asd995.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://rx.wgjwhj.cn

[T34] Lua：遍历表
来源：http://ld.jctech888.com.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://hx.gzmigu.cn

[T35] Lua：字典表
来源：http://mx.huixiangedu.cn

local d = { a = 1 };  d.b = 2
来源：http://wk.nszjky.cn

[T36] Lua：函数
来源：http://zw.nszjky.cn

function add(a, b) return a + b end
来源：http://fy.nicolike.cn

[T37] Lua：字符串拼接
来源：http://wf.bookmarksfly.cn

"a" .. "b"
来源：http://up.haigaiapp.cn

[T38] Lua：条件
来源：http://jw.shxzskj.cn

if x > 0 then print("正") end
来源：http://ov.nicolike.cn

[T39] Lua：模式匹配
来源：http://cs.bjjhwx.cn

string.find(s, "%d+")
来源：http://xw.shxzskj.cn

[T40] Lua：元表
来源：http://uj.bookmarksfly.cn

setmetatable({}, { __index = base })
来源：http://xp.muxihuayi.cn

[T41] Perl：Hello World
来源：http://ik.chemitech.net.cn

print "Hello\n";
来源：http://jz.lnxyls.cn

[T42] Perl：变量类型
来源：http://jb.shxzukj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ma.jianghongdianzi.cn

[T43] Perl：字符串插值
来源：http://xs.colortex.cn

"值: $a"
来源：http://ig.asd995.cn

[T44] Perl：条件
来源：http://wk.huanxung.cn

if ($a > 0) { print "正"; }
来源：http://gq.nicolike.cn

[T45] Perl：数组遍历
来源：http://xt.shxzukj.cn

for my $x (@arr) { print $x; }
来源：http://xl.shtwfgs.cn

[T46] Perl：哈希操作
来源：http://kx.muxihuayi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rv.yuntaijiaju.cn

[T47] Perl：正则捕获
来源：http://os.yuntaijiaju.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://uy.szxytkj.cn

[T48] Perl：正则替换
来源：http://xx.colortex.cn

$s =~ s/old/new/g;
来源：http://ld.nszjky.cn

[T49] Perl：函数
来源：http://kn.shxzskj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cx.bookmarksfly.cn

[T50] Perl：逐行读文件
来源：http://sm.wgjwhj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://sv.panjiajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://px.chemitech.net.cn

[T51] Scala：Hello World
来源：http://nn.muxihuayi.cn

println("Hello")
来源：http://yl.chemitech.net.cn

[T52] Scala：变量
来源：http://sh.hahajie.cn

val a = 1;  var b = 2
来源：http://or.huanxung.cn

[T53] Scala：字符串插值
来源：http://ta.huixiangedu.cn

s"值: $b"
来源：http://ao.521024.cn

[T54] Scala：集合映射
来源：http://vb.asd995.cn

List(1, 2, 3).map(_ * 2)
来源：http://an.jctech888.com.cn

[T55] Scala：集合过滤
来源：http://dt.521024.cn

List(1, 2, 3).filter(_ > 1)
来源：http://cc.nszjky.cn

[T56] Scala：样例类
来源：http://kt.colortex.cn

case class User(name: String, age: Int)
来源：http://sv.shxzukj.cn

[T57] Scala：模式匹配
来源：http://hz.shxzukj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://at.wgjwhj.cn

[T58] Scala：函数定义
来源：http://dt.newstarts.cn

def add(a: Int, b: Int): Int = a + b
来源：http://so.hahajie.cn

[T59] Scala：循环
来源：http://vf.bookmarksfly.cn

for (i <- 1 to 10) println(i)
来源：http://su.panjiajie.cn

[T60] Scala：折叠
来源：http://tt.9csxet.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sz.szsharing.cn

================================================================================
来源：http://bg.szsharing.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zk.jianghongdianzi.cn

================================================================================
来源：http://tw.bookmarksfly.cn

[U01] Py：创建虚拟环境
来源：http://bu.lnxyls.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nk.newstarts.cn

[U02] Py：导出 / 安装依赖
来源：http://eg.yuexingan06.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://iv.hahajie.cn

[U03] Py：加载 .env 配置
来源：http://dw.hnjuh.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://pv.bookmarksfly.cn

[U04] Py：变量调试打印
来源：http://lg.jctech888.com.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ft.9csxet.cn

[U05] Py：列表去重且保序
来源：http://km.panjiajie.cn

list(dict.fromkeys(arr))
来源：http://bb.nicolike.cn

[U06] Py：合并两个字典
来源：http://ob.shtwfgs.cn

{**a, **b}
来源：http://xm.szsharing.cn

[U07] Py：反转字典键值
来源：http://hv.shxzukj.cn

{v: k for k, v in d.items()}
来源：http://xf.bjjhwx.cn

[U08] Py：展平二维列表
来源：http://od.haigaiapp.cn

[y for x in nested for y in x]
来源：http://ll.gzmigu.cn

[U09] Py：字典取最大值的键
来源：http://ju.panjiajie.cn

max(d, key=d.get)
来源：http://jq.muxihuayi.cn

[U10] Py：按值排序字典
来源：http://if.hnjuh.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yv.shxzskj.cn

[U11] Py：生成器表达式
来源：http://rw.nicolike.cn

(x * 2 for x in arr)
来源：http://gf.hnjuh.cn

[U12] Py：取出现最多的 3 个元素
来源：http://io.panjiajie.cn

Counter(arr).most_common(3)
来源：http://tt.colortex.cn

[U13] Py：固定长度队列
来源：http://xi.bjjhwx.cn

deque(maxlen=10)
来源：http://be.szxytkj.cn

[U14] Py：分组收集到列表
来源：http://lt.yuexingan06.cn

defaultdict(list)
来源：http://zs.yuexingan06.cn

[U15] Py：高精度计时
来源：http://gw.bjjhwx.cn

t = time.perf_counter()
来源：http://lf.gzmigu.cn

[U16] Py：命令行参数解析
来源：http://zv.yuntaijiaju.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ao.szsharing.cn

[U17] Py：初始化日志
来源：http://qu.panjiajie.cn

logging.basicConfig(level=logging.INFO)
来源：http://dp.nszjky.cn

[U18] Py：预编译正则
来源：http://mt.gzmigu.cn

pat = re.compile(r"\d+")
来源：http://fs.hahajie.cn

[U19] Py：正则替换带回调
来源：http://az.szsharing.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fo.shxzskj.cn

[U20] Py：缓存函数结果
来源：http://qj.newstarts.cn

@functools.lru_cache(maxsize=None)
来源：http://rt.huanxung.cn

[U21] Py：自定义上下文管理器
来源：http://dt.jctech888.com.cn

@contextlib.contextmanager
来源：http://oz.muxihuayi.cn

[U22] Py：矩阵转置
来源：http://eg.gzmigu.cn

list(zip(*m))
来源：http://ij.lnxyls.cn

[U23] Py：分块读取大文件
来源：http://ub.haigaiapp.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bf.szxytkj.cn

[U24] Py：路径操作
来源：http://is.nszjky.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kj.521024.cn

[U25] Py：CSV 按字典读
来源：http://yh.szxytkj.cn

csv.DictReader(f)
来源：http://ha.haigaiapp.cn

[U26] Py：并发下载
来源：http://jf.shxzukj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jr.gzmigu.cn

[U27] Py：异步 HTTP
来源：http://mg.huixinmuqiang.cn

aiohttp.ClientSession() 配合 async with
来源：http://wi.huanxung.cn

[U28] Py：类型别名
来源：http://ft.chemitech.net.cn

UserId = int
来源：http://mi.lnxyls.cn

[U29] Py：属性校验
来源：http://ut.hahajie.cn

@property 与 @x.setter 配合
来源：http://qu.yuntaijiaju.cn

[U30] Py：数据类
来源：http://wl.nszjky.cn

@dataclass(slots=True)
来源：http://mv.shtwfgs.cn

[U31] Py：单测
来源：http://rp.hnjuh.cn

python -m pytest -q
来源：http://go.bookmarksfly.cn

[U32] Py：代码格式化
来源：http://oi.bookmarksfly.cn

ruff format . && ruff check --fix .
来源：http://rq.colortex.cn

[U33] Py：打包发布
来源：http://hr.wgjwhj.cn

python -m build  （依赖 pyproject.toml）
来源：http://fq.szxytkj.cn

[U34] Py：判断编码
来源：http://wq.wgjwhj.cn

chardet.detect(raw)
来源：http://ih.panjiajie.cn

[U35] Py：发送邮件
来源：http://gu.huixinmuqiang.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://md.jctech888.com.cn

[U36] Py：定时任务
来源：http://vk.chemitech.net.cn

schedule.every(10).minutes.do(job)
来源：http://ko.haigaiapp.cn

[U37] Py：读写 Excel
来源：http://pt.521024.cn

pandas.read_excel / DataFrame.to_excel
来源：http://xh.jianghongdianzi.cn

[U38] Py：获取脚本所在目录
来源：http://so.jianghongdianzi.cn

Path(__file__).resolve().parent
来源：http://bf.szxytkj.cn

[U39] Py：判断是否在交互环境
来源：http://oe.hnjuh.cn

sys.stdout.isatty()
来源：http://bb.asd995.cn

[U40] Py：打印到标准错误
来源：http://dd.wgjwhj.cn

print("err", file=sys.stderr)
来源：http://es.shtwfgs.cn

[U41] PHP：初始化 Composer 项目
来源：http://mj.wgjwhj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zf.asd995.cn

[U42] PHP：PSR-4 自动加载
来源：http://hu.haigaiapp.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lc.gzmigu.cn

[U43] PHP：声明命名空间
来源：http://aj.wgjwhj.cn

namespace App\Http;
来源：http://kl.muxihuayi.cn

[U44] PHP：开启严格类型
来源：http://sl.yuntaijiaju.cn

declare(strict_types=1);
来源：http://kk.nicolike.cn

[U45] PHP：类型声明与返回类型
来源：http://zu.wgjwhj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://uj.panjiajie.cn

[U46] PHP：可空类型
来源：http://tu.jctech888.com.cn

?string $name = null
来源：http://lh.colortex.cn

[U47] PHP：联合类型
来源：http://vg.haigaiapp.cn

int|string $id
来源：http://wi.chemitech.net.cn

[U48] PHP：纯枚举
来源：http://zh.panjiajie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ny.521024.cn

[U49] PHP：只读属性
来源：http://ii.9csxet.cn

public readonly string $name
来源：http://fk.yuexingan06.cn

[U50] PHP：构造器属性提升
来源：http://qo.colortex.cn

public function __construct(private int $id) {}
来源：http://ig.haigaiapp.cn

[U51] PHP：数组解构
来源：http://iu.nszjky.cn

[$a, $b] = $arr;
来源：http://jh.nicolike.cn

[U52] PHP：箭头函数
来源：http://ns.bookmarksfly.cn

$double = fn($x) => $x * 2;
来源：http://iz.shxzukj.cn

[U53] PHP：空合并运算符
来源：http://lo.nicolike.cn

$v = $a ?? $b ?? "default";
来源：http://rq.asd995.cn

[U54] PHP：空安全调用
来源：http://lg.szsharing.cn

$obj?->method()
来源：http://lc.shtwfgs.cn

[U55] PHP：match 表达式
来源：http://hp.huanxung.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lv.nicolike.cn

[U56] PHP：命名参数
来源：http://sz.asd995.cn

f(a: 1, b: 2)
来源：http://kx.521024.cn

[U57] PHP：字符串插值
来源：http://dr.shxzskj.cn

"值: {$a}"
来源：http://zz.jctech888.com.cn

[U58] PHP：数组三件套
来源：http://au.gzmigu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ox.nicolike.cn

[U59] PHP：自定义排序
来源：http://ng.chemitech.net.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://it.521024.cn

[U60] PHP：JSON 编解码
来源：http://vd.nicolike.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ea.yuntaijiaju.cn

[U61] PHP：正则
来源：http://qc.panjiajie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qw.hnjuh.cn

[U62] PHP：日期对象
来源：http://jx.muxihuayi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nz.bookmarksfly.cn

[U63] PHP：文件读写
来源：http://wv.huixinmuqiang.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://of.lnxyls.cn

[U64] PHP：目录遍历
来源：http://lz.shxzskj.cn

glob("dir/*.php");  scandir("dir");
来源：http://pf.521024.cn

[U65] PHP：会话
来源：http://uj.wgjwhj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://uo.hahajie.cn

[U66] PHP：设置 Cookie
来源：http://vr.nicolike.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wn.521024.cn

[U67] PHP：处理文件上传
来源：http://fz.huixiangedu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://iw.gzmigu.cn

[U68] PHP：PDO 连接
来源：http://um.gzmigu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://oi.colortex.cn

[U69] PHP：PDO 预处理
来源：http://zt.muxihuayi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://li.shtwfgs.cn

[U70] PHP：PDO 事务
来源：http://kg.panjiajie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ro.jctech888.com.cn

[U71] PHP：抛出异常
来源：http://pv.wgjwhj.cn

throw new RuntimeException("失败", 500);
来源：http://iu.panjiajie.cn

[U72] PHP：写错误日志
来源：http://pg.muxihuayi.cn

error_log("失败: " . $e->getMessage());
来源：http://yr.shxzskj.cn

[U73] PHP：读取 ini 配置
来源：http://cy.yuexingan06.cn

parse_ini_file("config.ini", true)
来源：http://ri.szxytkj.cn

[U74] PHP：读取环境变量
来源：http://ia.9csxet.cn

getenv("APP_ENV") ?: "production"
来源：http://yr.bjjhwx.cn

[U75] PHP：依赖注入
来源：http://cn.shxzskj.cn

composer require psr/container
来源：http://sb.gzmigu.cn

[U76] PHP：简单路由
来源：http://eq.newstarts.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jz.colortex.cn

[U77] PHP：模板渲染
来源：http://sb.9csxet.cn

composer require twig/twig
来源：http://pa.jianghongdianzi.cn

[U78] PHP：单元测试
来源：http://gp.huanxung.cn

composer require --dev phpunit/phpunit
来源：http://gb.hahajie.cn

[U79] PHP：静态分析
来源：http://cs.shtwfgs.cn

composer require --dev phpstan/phpstan
来源：http://hj.hahajie.cn

[U80] PHP：代码规范修复
来源：http://tn.colortex.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ki.hahajie.cn

[U81] JS：初始化项目
来源：http://qg.9csxet.cn

npm init -y;  npm i express
来源：http://yl.nszjky.cn

[U82] JS：package.json 脚本
来源：http://ey.asd995.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ol.yuntaijiaju.cn


<!-- 参考信息 -->