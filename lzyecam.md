代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rm.shxzskj.cn

[S55] C++：结构化绑定
来源：http://ww.shxzukj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vj.jianghongdianzi.cn

[S56] C++：optional
来源：http://cg.yuexingan06.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fi.huixinmuqiang.cn

[S57] C++：编译期常量
来源：http://ft.shxzukj.cn

constexpr int N = 10;
来源：http://ts.shxzukj.cn

[S58] C++：命名空间
来源：http://bo.chemitech.net.cn

namespace ns { int f() { return 1; } }
来源：http://cl.huixinmuqiang.cn

[S59] C++：静态断言
来源：http://pa.szsharing.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ke.bjjhwx.cn

[S60] C++：遍历并删除元素
来源：http://yw.szsharing.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dh.szsharing.cn

================================================================================
来源：http://mx.szxytkj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qc.shxzskj.cn

================================================================================
来源：http://so.huanxung.cn

[T01] Kotlin：Hello World
来源：http://zh.jctech888.com.cn

println("Hello")
来源：http://id.shxzskj.cn

[T02] Kotlin：变量
来源：http://hy.huanxung.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fe.lnxyls.cn

[T03] Kotlin：字符串模板
来源：http://sy.hnjuh.cn

"值: $b"
来源：http://ti.bjjhwx.cn

[T04] Kotlin：空安全
来源：http://nz.bookmarksfly.cn

val n: String? = null;  n?.length
来源：http://yf.newstarts.cn

[T05] Kotlin：when 表达式
来源：http://hb.hnjuh.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ss.jianghongdianzi.cn

[T06] Kotlin：集合映射
来源：http://nb.521024.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://aj.colortex.cn

[T07] Kotlin：集合过滤
来源：http://rf.szsharing.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://an.shxzukj.cn

[T08] Kotlin：数据类
来源：http://uo.newstarts.cn

data class User(val name: String, val age: Int)
来源：http://nr.szsharing.cn

[T09] Kotlin：扩展函数
来源：http://jd.521024.cn

fun String.exclaim() = this + "!"
来源：http://ga.huixinmuqiang.cn

[T10] Kotlin：默认参数
来源：http://yl.jctech888.com.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://to.muxihuayi.cn

[T11] Kotlin：协程
来源：http://ui.9csxet.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://aq.nicolike.cn

[T12] Kotlin：解构声明
来源：http://uq.wgjwhj.cn

val (a, b) = Pair(1, 2)
来源：http://rb.lnxyls.cn

[T13] Kotlin：只读 Map
来源：http://pl.shtwfgs.cn

val m = mapOf("a" to 1)
来源：http://lp.huixinmuqiang.cn

[T14] Kotlin：循环
来源：http://dd.gzmigu.cn

for (i in 1..10) println(i)
来源：http://mx.huixinmuqiang.cn

[T15] Kotlin：接口
来源：http://rl.nicolike.cn

interface Shape { fun area(): Double }
来源：http://ib.yuexingan06.cn

[T16] Swift：Hello World
来源：http://hx.haigaiapp.cn

print("Hello")
来源：http://xb.lnxyls.cn

[T17] Swift：变量与常量
来源：http://ig.huixiangedu.cn

var a = 1;  let b = 2
来源：http://ph.bookmarksfly.cn

[T18] Swift：字符串插值
来源：http://re.panjiajie.cn

"值: \(b)"
来源：http://xo.huanxung.cn

[T19] Swift：可选绑定
来源：http://ig.shxzukj.cn

if let n = opt { print(n) }
来源：http://ei.newstarts.cn

[T20] Swift：数组操作
来源：http://oh.shxzskj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fj.bjjhwx.cn

[T21] Swift：遍历
来源：http://dl.yuntaijiaju.cn

for x in a { print(x) }
来源：http://qw.wgjwhj.cn

[T22] Swift：字典
来源：http://de.panjiajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mn.wgjwhj.cn

[T23] Swift：函数
来源：http://zz.yuntaijiaju.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ja.asd995.cn

[T24] Swift：闭包
来源：http://bz.haigaiapp.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://na.521024.cn

[T25] Swift：结构体
来源：http://os.szsharing.cn

struct P { var x: Int }
来源：http://dw.szsharing.cn

[T26] Swift：类与重写
来源：http://hj.521024.cn

class A: Base { override func f() {} }
来源：http://rs.szxytkj.cn

[T27] Swift：错误处理
来源：http://uz.colortex.cn

do { try f() } catch { print(error) }
来源：http://fe.hnjuh.cn

[T28] Swift：枚举
来源：http://ml.521024.cn

enum Color { case red, green }
来源：http://hu.shxzskj.cn

[T29] Swift：guard 提前返回
来源：http://mz.yuexingan06.cn

guard let x = opt else { return }
来源：http://fo.nszjky.cn

[T30] Swift：协议
来源：http://db.haigaiapp.cn

protocol Shape { func area() -> Double }
来源：http://qo.wgjwhj.cn

[T31] Lua：Hello World
来源：http://dt.haigaiapp.cn

print("Hello")
来源：http://nt.hahajie.cn

[T32] Lua：局部变量
来源：http://ec.jctech888.com.cn

local a = 1
来源：http://mq.szsharing.cn

[T33] Lua：表（数组）
来源：http://ly.9csxet.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ot.huanxung.cn

[T34] Lua：遍历表
来源：http://ss.gzmigu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://cc.huanxung.cn

[T35] Lua：字典表
来源：http://wj.hahajie.cn

local d = { a = 1 };  d.b = 2
来源：http://ua.nszjky.cn

[T36] Lua：函数
来源：http://jy.newstarts.cn

function add(a, b) return a + b end
来源：http://dh.yuexingan06.cn

[T37] Lua：字符串拼接
来源：http://qc.9csxet.cn

"a" .. "b"
来源：http://gs.huixiangedu.cn

[T38] Lua：条件
来源：http://rw.shxzskj.cn

if x > 0 then print("正") end
来源：http://gd.nicolike.cn

[T39] Lua：模式匹配
来源：http://nr.colortex.cn

string.find(s, "%d+")
来源：http://wm.gzmigu.cn

[T40] Lua：元表
来源：http://ua.shxzskj.cn

setmetatable({}, { __index = base })
来源：http://iv.asd995.cn

[T41] Perl：Hello World
来源：http://ns.jianghongdianzi.cn

print "Hello\n";
来源：http://lx.shxzukj.cn

[T42] Perl：变量类型
来源：http://nv.521024.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dm.gzmigu.cn

[T43] Perl：字符串插值
来源：http://qg.jianghongdianzi.cn

"值: $a"
来源：http://ui.bookmarksfly.cn

[T44] Perl：条件
来源：http://hq.hahajie.cn

if ($a > 0) { print "正"; }
来源：http://rl.gzmigu.cn

[T45] Perl：数组遍历
来源：http://mk.jctech888.com.cn

for my $x (@arr) { print $x; }
来源：http://ej.521024.cn

[T46] Perl：哈希操作
来源：http://st.huixiangedu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://le.colortex.cn

[T47] Perl：正则捕获
来源：http://pg.chemitech.net.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ve.szxytkj.cn

[T48] Perl：正则替换
来源：http://eg.szxytkj.cn

$s =~ s/old/new/g;
来源：http://xf.muxihuayi.cn

[T49] Perl：函数
来源：http://gy.asd995.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://au.jianghongdianzi.cn

[T50] Perl：逐行读文件
来源：http://ja.huixiangedu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ze.haigaiapp.cn

while (my $line = <$fh>) { print $line; }
来源：http://di.szsharing.cn

[T51] Scala：Hello World
来源：http://yi.colortex.cn

println("Hello")
来源：http://jj.shxzskj.cn

[T52] Scala：变量
来源：http://dr.huixinmuqiang.cn

val a = 1;  var b = 2
来源：http://ot.gzmigu.cn

[T53] Scala：字符串插值
来源：http://fc.shxzukj.cn

s"值: $b"
来源：http://iz.jctech888.com.cn

[T54] Scala：集合映射
来源：http://sm.shxzskj.cn

List(1, 2, 3).map(_ * 2)
来源：http://jy.muxihuayi.cn

[T55] Scala：集合过滤
来源：http://an.lnxyls.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ev.szxytkj.cn

[T56] Scala：样例类
来源：http://oj.nszjky.cn

case class User(name: String, age: Int)
来源：http://rz.szxytkj.cn

[T57] Scala：模式匹配
来源：http://kx.hnjuh.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://hi.521024.cn

[T58] Scala：函数定义
来源：http://vw.shtwfgs.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wp.nszjky.cn

[T59] Scala：循环
来源：http://yr.huixinmuqiang.cn

for (i <- 1 to 10) println(i)
来源：http://qo.bookmarksfly.cn

[T60] Scala：折叠
来源：http://dv.haigaiapp.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sa.bookmarksfly.cn

================================================================================
来源：http://gv.jctech888.com.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://re.hnjuh.cn

================================================================================
来源：http://iw.szxytkj.cn

[U01] Py：创建虚拟环境
来源：http://oe.asd995.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nh.szsharing.cn

[U02] Py：导出 / 安装依赖
来源：http://bt.huanxung.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ex.nszjky.cn

[U03] Py：加载 .env 配置
来源：http://jo.shtwfgs.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://bk.bjjhwx.cn

[U04] Py：变量调试打印
来源：http://ch.nicolike.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gx.wgjwhj.cn

[U05] Py：列表去重且保序
来源：http://wy.jianghongdianzi.cn

list(dict.fromkeys(arr))
来源：http://ke.9csxet.cn

[U06] Py：合并两个字典
来源：http://st.huixinmuqiang.cn

{**a, **b}
来源：http://ea.9csxet.cn

[U07] Py：反转字典键值
来源：http://rl.asd995.cn

{v: k for k, v in d.items()}
来源：http://bx.9csxet.cn

[U08] Py：展平二维列表
来源：http://lb.nicolike.cn

[y for x in nested for y in x]
来源：http://jg.szxytkj.cn

[U09] Py：字典取最大值的键
来源：http://hp.yuntaijiaju.cn

max(d, key=d.get)
来源：http://zf.newstarts.cn

[U10] Py：按值排序字典
来源：http://pg.shtwfgs.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wh.yuntaijiaju.cn

[U11] Py：生成器表达式
来源：http://ca.panjiajie.cn

(x * 2 for x in arr)
来源：http://yr.nszjky.cn

[U12] Py：取出现最多的 3 个元素
来源：http://iq.haigaiapp.cn

Counter(arr).most_common(3)
来源：http://ry.colortex.cn

[U13] Py：固定长度队列
来源：http://cz.jctech888.com.cn

deque(maxlen=10)
来源：http://sm.lnxyls.cn

[U14] Py：分组收集到列表
来源：http://ip.9csxet.cn

defaultdict(list)
来源：http://ge.panjiajie.cn

[U15] Py：高精度计时
来源：http://iy.muxihuayi.cn

t = time.perf_counter()
来源：http://hb.huixiangedu.cn

[U16] Py：命令行参数解析
来源：http://zi.shxzskj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ek.yuexingan06.cn

[U17] Py：初始化日志
来源：http://pw.hahajie.cn

logging.basicConfig(level=logging.INFO)
来源：http://kn.bookmarksfly.cn

[U18] Py：预编译正则
来源：http://xe.szsharing.cn

pat = re.compile(r"\d+")
来源：http://jz.colortex.cn

[U19] Py：正则替换带回调
来源：http://be.muxihuayi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zn.521024.cn

[U20] Py：缓存函数结果
来源：http://yn.jianghongdianzi.cn

@functools.lru_cache(maxsize=None)
来源：http://uk.shxzskj.cn

[U21] Py：自定义上下文管理器
来源：http://oq.panjiajie.cn

@contextlib.contextmanager
来源：http://rm.newstarts.cn

[U22] Py：矩阵转置
来源：http://xc.szxytkj.cn

list(zip(*m))
来源：http://ya.haigaiapp.cn

[U23] Py：分块读取大文件
来源：http://vd.gzmigu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jn.hahajie.cn

[U24] Py：路径操作
来源：http://qn.asd995.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dd.nszjky.cn

[U25] Py：CSV 按字典读
来源：http://ct.szxytkj.cn

csv.DictReader(f)
来源：http://cc.lnxyls.cn

[U26] Py：并发下载
来源：http://jk.szxytkj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://uj.gzmigu.cn

[U27] Py：异步 HTTP
来源：http://uk.haigaiapp.cn

aiohttp.ClientSession() 配合 async with
来源：http://oh.panjiajie.cn

[U28] Py：类型别名
来源：http://nv.hahajie.cn

UserId = int
来源：http://ug.yuntaijiaju.cn

[U29] Py：属性校验
来源：http://th.asd995.cn

@property 与 @x.setter 配合
来源：http://ug.gzmigu.cn

[U30] Py：数据类
来源：http://jn.haigaiapp.cn

@dataclass(slots=True)
来源：http://sw.jctech888.com.cn

[U31] Py：单测
来源：http://rv.wgjwhj.cn

python -m pytest -q
来源：http://qj.haigaiapp.cn

[U32] Py：代码格式化
来源：http://qa.haigaiapp.cn

ruff format . && ruff check --fix .
来源：http://aq.bookmarksfly.cn

[U33] Py：打包发布
来源：http://gn.muxihuayi.cn

python -m build  （依赖 pyproject.toml）
来源：http://gz.panjiajie.cn

[U34] Py：判断编码
来源：http://gh.asd995.cn

chardet.detect(raw)
来源：http://un.jianghongdianzi.cn

[U35] Py：发送邮件
来源：http://bk.nicolike.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fz.9csxet.cn

[U36] Py：定时任务
来源：http://ow.bjjhwx.cn

schedule.every(10).minutes.do(job)
来源：http://ty.newstarts.cn

[U37] Py：读写 Excel
来源：http://gd.hahajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://li.szsharing.cn

[U38] Py：获取脚本所在目录
来源：http://gc.haigaiapp.cn

Path(__file__).resolve().parent
来源：http://nr.gzmigu.cn

[U39] Py：判断是否在交互环境
来源：http://cz.hnjuh.cn

sys.stdout.isatty()
来源：http://af.szsharing.cn

[U40] Py：打印到标准错误
来源：http://jc.muxihuayi.cn

print("err", file=sys.stderr)
来源：http://vz.shtwfgs.cn

[U41] PHP：初始化 Composer 项目
来源：http://lg.gzmigu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xn.shxzskj.cn

[U42] PHP：PSR-4 自动加载
来源：http://hq.shtwfgs.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qs.muxihuayi.cn

[U43] PHP：声明命名空间
来源：http://le.panjiajie.cn

namespace App\Http;
来源：http://es.bookmarksfly.cn

[U44] PHP：开启严格类型
来源：http://cp.newstarts.cn

declare(strict_types=1);
来源：http://au.9csxet.cn

[U45] PHP：类型声明与返回类型
来源：http://rd.shxzukj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://yy.szsharing.cn

[U46] PHP：可空类型
来源：http://ew.bjjhwx.cn

?string $name = null
来源：http://mz.szsharing.cn

[U47] PHP：联合类型
来源：http://nj.huixiangedu.cn

int|string $id
来源：http://mj.haigaiapp.cn

[U48] PHP：纯枚举
来源：http://mp.shxzskj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sz.shxzukj.cn

[U49] PHP：只读属性
来源：http://ym.yuexingan06.cn

public readonly string $name
来源：http://xv.huixinmuqiang.cn

[U50] PHP：构造器属性提升
来源：http://xp.panjiajie.cn

public function __construct(private int $id) {}
来源：http://yx.colortex.cn

[U51] PHP：数组解构
来源：http://eh.lnxyls.cn

[$a, $b] = $arr;
来源：http://ex.asd995.cn

[U52] PHP：箭头函数
来源：http://pm.colortex.cn

$double = fn($x) => $x * 2;
来源：http://nt.gzmigu.cn

[U53] PHP：空合并运算符
来源：http://aa.shtwfgs.cn

$v = $a ?? $b ?? "default";
来源：http://jr.shxzukj.cn

[U54] PHP：空安全调用
来源：http://sf.hahajie.cn

$obj?->method()
来源：http://px.szxytkj.cn

[U55] PHP：match 表达式
来源：http://hp.nszjky.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cn.gzmigu.cn

[U56] PHP：命名参数
来源：http://js.lnxyls.cn

f(a: 1, b: 2)
来源：http://fp.szsharing.cn

[U57] PHP：字符串插值
来源：http://na.chemitech.net.cn

"值: {$a}"
来源：http://yn.jctech888.com.cn

[U58] PHP：数组三件套
来源：http://sb.huanxung.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://km.muxihuayi.cn

[U59] PHP：自定义排序
来源：http://vy.colortex.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lf.nicolike.cn

[U60] PHP：JSON 编解码
来源：http://ia.wgjwhj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ge.9csxet.cn

[U61] PHP：正则
来源：http://xy.nicolike.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gs.chemitech.net.cn

[U62] PHP：日期对象
来源：http://az.chemitech.net.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sx.yuntaijiaju.cn

[U63] PHP：文件读写
来源：http://tx.shxzskj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://et.shtwfgs.cn

[U64] PHP：目录遍历
来源：http://ei.huanxung.cn

glob("dir/*.php");  scandir("dir");
来源：http://su.szsharing.cn

[U65] PHP：会话
来源：http://ph.colortex.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://in.shxzukj.cn

[U66] PHP：设置 Cookie
来源：http://zu.huanxung.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qy.nicolike.cn

[U67] PHP：处理文件上传
来源：http://wt.wgjwhj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nu.hahajie.cn

[U68] PHP：PDO 连接
来源：http://pd.nszjky.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yc.asd995.cn

[U69] PHP：PDO 预处理
来源：http://mg.shxzskj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ws.asd995.cn

[U70] PHP：PDO 事务
来源：http://ib.lnxyls.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ge.shxzskj.cn

[U71] PHP：抛出异常
来源：http://qj.521024.cn

throw new RuntimeException("失败", 500);
来源：http://wu.szsharing.cn

[U72] PHP：写错误日志
来源：http://so.wgjwhj.cn

error_log("失败: " . $e->getMessage());
来源：http://vg.9csxet.cn

[U73] PHP：读取 ini 配置
来源：http://rw.521024.cn

parse_ini_file("config.ini", true)
来源：http://fs.shxzskj.cn

[U74] PHP：读取环境变量
来源：http://zm.huanxung.cn

getenv("APP_ENV") ?: "production"
来源：http://rv.gzmigu.cn

[U75] PHP：依赖注入
来源：http://lp.haigaiapp.cn

composer require psr/container
来源：http://se.asd995.cn

[U76] PHP：简单路由
来源：http://lk.muxihuayi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yk.shtwfgs.cn

[U77] PHP：模板渲染
来源：http://aa.nszjky.cn

composer require twig/twig
来源：http://ld.nszjky.cn

[U78] PHP：单元测试
来源：http://ow.hahajie.cn

composer require --dev phpunit/phpunit
来源：http://gf.9csxet.cn

[U79] PHP：静态分析
来源：http://ia.panjiajie.cn

composer require --dev phpstan/phpstan
来源：http://wx.bjjhwx.cn

[U80] PHP：代码规范修复
来源：http://db.muxihuayi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://bb.yuexingan06.cn


<!-- 参考信息 -->