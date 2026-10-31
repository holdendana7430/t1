代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ss.colortex.cn

[S57] C++：编译期常量
来源：http://sd.gzmigu.cn

constexpr int N = 10;
来源：http://rs.huixiangedu.cn

[S58] C++：命名空间
来源：http://kg.9csxet.cn

namespace ns { int f() { return 1; } }
来源：http://wi.bookmarksfly.cn

[S59] C++：静态断言
来源：http://ie.9csxet.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qf.yuexingan06.cn

[S60] C++：遍历并删除元素
来源：http://xz.chemitech.net.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zp.gzmigu.cn

================================================================================
来源：http://lg.panjiajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://oq.hnjuh.cn

================================================================================
来源：http://zf.muxihuayi.cn

[T01] Kotlin：Hello World
来源：http://jq.shtwfgs.cn

println("Hello")
来源：http://lr.haigaiapp.cn

[T02] Kotlin：变量
来源：http://sf.szxytkj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yr.yuexingan06.cn

[T03] Kotlin：字符串模板
来源：http://xt.yuexingan06.cn

"值: $b"
来源：http://jo.huanxung.cn

[T04] Kotlin：空安全
来源：http://bm.shtwfgs.cn

val n: String? = null;  n?.length
来源：http://sv.chemitech.net.cn

[T05] Kotlin：when 表达式
来源：http://eb.yuexingan06.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bv.jianghongdianzi.cn

[T06] Kotlin：集合映射
来源：http://sb.nicolike.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://eh.hahajie.cn

[T07] Kotlin：集合过滤
来源：http://gi.shxzukj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xq.panjiajie.cn

[T08] Kotlin：数据类
来源：http://sa.huanxung.cn

data class User(val name: String, val age: Int)
来源：http://we.hnjuh.cn

[T09] Kotlin：扩展函数
来源：http://ym.colortex.cn

fun String.exclaim() = this + "!"
来源：http://hg.szsharing.cn

[T10] Kotlin：默认参数
来源：http://yg.muxihuayi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ao.szxytkj.cn

[T11] Kotlin：协程
来源：http://fk.huixiangedu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ba.yuntaijiaju.cn

[T12] Kotlin：解构声明
来源：http://lr.huanxung.cn

val (a, b) = Pair(1, 2)
来源：http://yp.9csxet.cn

[T13] Kotlin：只读 Map
来源：http://ay.bjjhwx.cn

val m = mapOf("a" to 1)
来源：http://bh.9csxet.cn

[T14] Kotlin：循环
来源：http://ri.hahajie.cn

for (i in 1..10) println(i)
来源：http://um.nicolike.cn

[T15] Kotlin：接口
来源：http://qo.colortex.cn

interface Shape { fun area(): Double }
来源：http://rz.panjiajie.cn

[T16] Swift：Hello World
来源：http://xd.panjiajie.cn

print("Hello")
来源：http://ku.bookmarksfly.cn

[T17] Swift：变量与常量
来源：http://sw.bookmarksfly.cn

var a = 1;  let b = 2
来源：http://sn.szsharing.cn

[T18] Swift：字符串插值
来源：http://qq.nszjky.cn

"值: \(b)"
来源：http://pi.colortex.cn

[T19] Swift：可选绑定
来源：http://yg.nszjky.cn

if let n = opt { print(n) }
来源：http://hf.colortex.cn

[T20] Swift：数组操作
来源：http://gb.muxihuayi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zr.wgjwhj.cn

[T21] Swift：遍历
来源：http://zh.bjjhwx.cn

for x in a { print(x) }
来源：http://dv.bookmarksfly.cn

[T22] Swift：字典
来源：http://ff.shxzskj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://tp.colortex.cn

[T23] Swift：函数
来源：http://bp.shxzukj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vx.521024.cn

[T24] Swift：闭包
来源：http://ml.huanxung.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://pd.huanxung.cn

[T25] Swift：结构体
来源：http://kv.szxytkj.cn

struct P { var x: Int }
来源：http://gd.colortex.cn

[T26] Swift：类与重写
来源：http://tn.hahajie.cn

class A: Base { override func f() {} }
来源：http://dn.gzmigu.cn

[T27] Swift：错误处理
来源：http://vq.muxihuayi.cn

do { try f() } catch { print(error) }
来源：http://sb.szsharing.cn

[T28] Swift：枚举
来源：http://eh.gzmigu.cn

enum Color { case red, green }
来源：http://hh.chemitech.net.cn

[T29] Swift：guard 提前返回
来源：http://rp.szxytkj.cn

guard let x = opt else { return }
来源：http://ym.shtwfgs.cn

[T30] Swift：协议
来源：http://bz.hnjuh.cn

protocol Shape { func area() -> Double }
来源：http://sa.huixiangedu.cn

[T31] Lua：Hello World
来源：http://hx.wgjwhj.cn

print("Hello")
来源：http://fd.huixiangedu.cn

[T32] Lua：局部变量
来源：http://uz.huixiangedu.cn

local a = 1
来源：http://ww.jctech888.com.cn

[T33] Lua：表（数组）
来源：http://iy.jctech888.com.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://po.haigaiapp.cn

[T34] Lua：遍历表
来源：http://jt.chemitech.net.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://sn.yuexingan06.cn

[T35] Lua：字典表
来源：http://id.shxzskj.cn

local d = { a = 1 };  d.b = 2
来源：http://yr.haigaiapp.cn

[T36] Lua：函数
来源：http://em.nicolike.cn

function add(a, b) return a + b end
来源：http://gj.szsharing.cn

[T37] Lua：字符串拼接
来源：http://dr.nszjky.cn

"a" .. "b"
来源：http://gu.shxzskj.cn

[T38] Lua：条件
来源：http://da.szxytkj.cn

if x > 0 then print("正") end
来源：http://le.9csxet.cn

[T39] Lua：模式匹配
来源：http://zd.chemitech.net.cn

string.find(s, "%d+")
来源：http://fc.9csxet.cn

[T40] Lua：元表
来源：http://io.bookmarksfly.cn

setmetatable({}, { __index = base })
来源：http://pr.yuntaijiaju.cn

[T41] Perl：Hello World
来源：http://ps.huanxung.cn

print "Hello\n";
来源：http://my.nicolike.cn

[T42] Perl：变量类型
来源：http://db.nszjky.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gi.gzmigu.cn

[T43] Perl：字符串插值
来源：http://ni.lnxyls.cn

"值: $a"
来源：http://pk.bjjhwx.cn

[T44] Perl：条件
来源：http://ak.huixinmuqiang.cn

if ($a > 0) { print "正"; }
来源：http://ny.521024.cn

[T45] Perl：数组遍历
来源：http://lo.chemitech.net.cn

for my $x (@arr) { print $x; }
来源：http://kv.shtwfgs.cn

[T46] Perl：哈希操作
来源：http://kn.huixiangedu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://or.yuntaijiaju.cn

[T47] Perl：正则捕获
来源：http://in.wgjwhj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ps.newstarts.cn

[T48] Perl：正则替换
来源：http://jm.panjiajie.cn

$s =~ s/old/new/g;
来源：http://cx.hahajie.cn

[T49] Perl：函数
来源：http://am.hnjuh.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bo.huixinmuqiang.cn

[T50] Perl：逐行读文件
来源：http://ur.gzmigu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://yb.lnxyls.cn

while (my $line = <$fh>) { print $line; }
来源：http://wl.wgjwhj.cn

[T51] Scala：Hello World
来源：http://wr.9csxet.cn

println("Hello")
来源：http://hy.shxzskj.cn

[T52] Scala：变量
来源：http://xh.chemitech.net.cn

val a = 1;  var b = 2
来源：http://wh.shxzskj.cn

[T53] Scala：字符串插值
来源：http://tb.hahajie.cn

s"值: $b"
来源：http://le.shtwfgs.cn

[T54] Scala：集合映射
来源：http://fy.colortex.cn

List(1, 2, 3).map(_ * 2)
来源：http://nw.nicolike.cn

[T55] Scala：集合过滤
来源：http://xh.jctech888.com.cn

List(1, 2, 3).filter(_ > 1)
来源：http://lc.hahajie.cn

[T56] Scala：样例类
来源：http://ih.newstarts.cn

case class User(name: String, age: Int)
来源：http://xe.jianghongdianzi.cn

[T57] Scala：模式匹配
来源：http://fd.huixiangedu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://pw.chemitech.net.cn

[T58] Scala：函数定义
来源：http://zp.nicolike.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bj.yuntaijiaju.cn

[T59] Scala：循环
来源：http://bh.huixiangedu.cn

for (i <- 1 to 10) println(i)
来源：http://hf.lnxyls.cn

[T60] Scala：折叠
来源：http://do.yuntaijiaju.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ce.hnjuh.cn

================================================================================
来源：http://um.9csxet.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tz.chemitech.net.cn

================================================================================
来源：http://ot.colortex.cn

[U01] Py：创建虚拟环境
来源：http://jl.panjiajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nb.chemitech.net.cn

[U02] Py：导出 / 安装依赖
来源：http://oa.9csxet.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ee.asd995.cn

[U03] Py：加载 .env 配置
来源：http://xx.hnjuh.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://cc.huanxung.cn

[U04] Py：变量调试打印
来源：http://sj.shxzskj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://am.haigaiapp.cn

[U05] Py：列表去重且保序
来源：http://wh.nszjky.cn

list(dict.fromkeys(arr))
来源：http://rj.shxzukj.cn

[U06] Py：合并两个字典
来源：http://rx.panjiajie.cn

{**a, **b}
来源：http://sz.huixiangedu.cn

[U07] Py：反转字典键值
来源：http://yb.bookmarksfly.cn

{v: k for k, v in d.items()}
来源：http://xz.szsharing.cn

[U08] Py：展平二维列表
来源：http://lw.newstarts.cn

[y for x in nested for y in x]
来源：http://bs.lnxyls.cn

[U09] Py：字典取最大值的键
来源：http://gx.yuexingan06.cn

max(d, key=d.get)
来源：http://pc.521024.cn

[U10] Py：按值排序字典
来源：http://lz.9csxet.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://he.haigaiapp.cn

[U11] Py：生成器表达式
来源：http://bz.haigaiapp.cn

(x * 2 for x in arr)
来源：http://ab.muxihuayi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://oc.shxzskj.cn

Counter(arr).most_common(3)
来源：http://we.shxzskj.cn

[U13] Py：固定长度队列
来源：http://lb.huixiangedu.cn

deque(maxlen=10)
来源：http://zp.muxihuayi.cn

[U14] Py：分组收集到列表
来源：http://mz.szxytkj.cn

defaultdict(list)
来源：http://sf.shxzukj.cn

[U15] Py：高精度计时
来源：http://gg.hnjuh.cn

t = time.perf_counter()
来源：http://iz.lnxyls.cn

[U16] Py：命令行参数解析
来源：http://al.haigaiapp.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://od.colortex.cn

[U17] Py：初始化日志
来源：http://qr.wgjwhj.cn

logging.basicConfig(level=logging.INFO)
来源：http://lt.huixinmuqiang.cn

[U18] Py：预编译正则
来源：http://hj.chemitech.net.cn

pat = re.compile(r"\d+")
来源：http://kq.gzmigu.cn

[U19] Py：正则替换带回调
来源：http://gf.colortex.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gp.colortex.cn

[U20] Py：缓存函数结果
来源：http://vg.bookmarksfly.cn

@functools.lru_cache(maxsize=None)
来源：http://np.panjiajie.cn

[U21] Py：自定义上下文管理器
来源：http://nc.nicolike.cn

@contextlib.contextmanager
来源：http://cb.bookmarksfly.cn

[U22] Py：矩阵转置
来源：http://yn.huixinmuqiang.cn

list(zip(*m))
来源：http://vx.huixiangedu.cn

[U23] Py：分块读取大文件
来源：http://cm.bjjhwx.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://kd.huixiangedu.cn

[U24] Py：路径操作
来源：http://af.huixiangedu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://sr.shtwfgs.cn

[U25] Py：CSV 按字典读
来源：http://cu.hnjuh.cn

csv.DictReader(f)
来源：http://ji.wgjwhj.cn

[U26] Py：并发下载
来源：http://gc.wgjwhj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ym.huanxung.cn

[U27] Py：异步 HTTP
来源：http://dc.shxzskj.cn

aiohttp.ClientSession() 配合 async with
来源：http://mb.huanxung.cn

[U28] Py：类型别名
来源：http://qp.panjiajie.cn

UserId = int
来源：http://ut.panjiajie.cn

[U29] Py：属性校验
来源：http://is.jctech888.com.cn

@property 与 @x.setter 配合
来源：http://zt.521024.cn

[U30] Py：数据类
来源：http://wr.huixinmuqiang.cn

@dataclass(slots=True)
来源：http://bk.muxihuayi.cn

[U31] Py：单测
来源：http://ur.asd995.cn

python -m pytest -q
来源：http://yk.bjjhwx.cn

[U32] Py：代码格式化
来源：http://wn.huixiangedu.cn

ruff format . && ruff check --fix .
来源：http://pi.bjjhwx.cn

[U33] Py：打包发布
来源：http://ys.jctech888.com.cn

python -m build  （依赖 pyproject.toml）
来源：http://sz.szsharing.cn

[U34] Py：判断编码
来源：http://wa.wgjwhj.cn

chardet.detect(raw)
来源：http://ne.9csxet.cn

[U35] Py：发送邮件
来源：http://tw.bjjhwx.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fj.9csxet.cn

[U36] Py：定时任务
来源：http://df.muxihuayi.cn

schedule.every(10).minutes.do(job)
来源：http://yq.bookmarksfly.cn

[U37] Py：读写 Excel
来源：http://qr.jctech888.com.cn

pandas.read_excel / DataFrame.to_excel
来源：http://fe.huixiangedu.cn

[U38] Py：获取脚本所在目录
来源：http://yg.szsharing.cn

Path(__file__).resolve().parent
来源：http://mw.nszjky.cn

[U39] Py：判断是否在交互环境
来源：http://lh.gzmigu.cn

sys.stdout.isatty()
来源：http://qq.colortex.cn

[U40] Py：打印到标准错误
来源：http://xv.hnjuh.cn

print("err", file=sys.stderr)
来源：http://xg.haigaiapp.cn

[U41] PHP：初始化 Composer 项目
来源：http://ni.panjiajie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://mr.yuexingan06.cn

[U42] PHP：PSR-4 自动加载
来源：http://yv.hnjuh.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://md.9csxet.cn

[U43] PHP：声明命名空间
来源：http://rk.jctech888.com.cn

namespace App\Http;
来源：http://en.521024.cn

[U44] PHP：开启严格类型
来源：http://mx.haigaiapp.cn

declare(strict_types=1);
来源：http://cb.shxzskj.cn

[U45] PHP：类型声明与返回类型
来源：http://ei.panjiajie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://iv.jctech888.com.cn

[U46] PHP：可空类型
来源：http://xj.bjjhwx.cn

?string $name = null
来源：http://dz.huixiangedu.cn

[U47] PHP：联合类型
来源：http://qj.lnxyls.cn

int|string $id
来源：http://lt.wgjwhj.cn

[U48] PHP：纯枚举
来源：http://ur.nicolike.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://md.shtwfgs.cn

[U49] PHP：只读属性
来源：http://dv.szxytkj.cn

public readonly string $name
来源：http://mf.jianghongdianzi.cn

[U50] PHP：构造器属性提升
来源：http://tw.gzmigu.cn

public function __construct(private int $id) {}
来源：http://ri.panjiajie.cn

[U51] PHP：数组解构
来源：http://aj.haigaiapp.cn

[$a, $b] = $arr;
来源：http://tb.wgjwhj.cn

[U52] PHP：箭头函数
来源：http://si.shxzskj.cn

$double = fn($x) => $x * 2;
来源：http://zo.shtwfgs.cn

[U53] PHP：空合并运算符
来源：http://bd.nszjky.cn

$v = $a ?? $b ?? "default";
来源：http://ec.muxihuayi.cn

[U54] PHP：空安全调用
来源：http://zb.chemitech.net.cn

$obj?->method()
来源：http://kf.muxihuayi.cn

[U55] PHP：match 表达式
来源：http://vb.huanxung.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qu.shxzskj.cn

[U56] PHP：命名参数
来源：http://qg.shxzskj.cn

f(a: 1, b: 2)
来源：http://qu.9csxet.cn

[U57] PHP：字符串插值
来源：http://ez.asd995.cn

"值: {$a}"
来源：http://ey.panjiajie.cn

[U58] PHP：数组三件套
来源：http://ys.yuntaijiaju.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cz.huanxung.cn

[U59] PHP：自定义排序
来源：http://ku.hahajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pd.521024.cn

[U60] PHP：JSON 编解码
来源：http://hj.jctech888.com.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://uo.huanxung.cn

[U61] PHP：正则
来源：http://xg.szsharing.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kj.jianghongdianzi.cn

[U62] PHP：日期对象
来源：http://dy.jianghongdianzi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pz.9csxet.cn

[U63] PHP：文件读写
来源：http://bd.521024.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tf.muxihuayi.cn

[U64] PHP：目录遍历
来源：http://rm.szxytkj.cn

glob("dir/*.php");  scandir("dir");
来源：http://vk.nicolike.cn

[U65] PHP：会话
来源：http://pf.hnjuh.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://nc.huixinmuqiang.cn

[U66] PHP：设置 Cookie
来源：http://pw.huixinmuqiang.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hn.shtwfgs.cn

[U67] PHP：处理文件上传
来源：http://ce.jianghongdianzi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ij.yuexingan06.cn

[U68] PHP：PDO 连接
来源：http://vv.yuntaijiaju.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cx.gzmigu.cn

[U69] PHP：PDO 预处理
来源：http://zc.jianghongdianzi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ct.wgjwhj.cn

[U70] PHP：PDO 事务
来源：http://ll.lnxyls.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://di.haigaiapp.cn

[U71] PHP：抛出异常
来源：http://nb.newstarts.cn

throw new RuntimeException("失败", 500);
来源：http://bi.colortex.cn

[U72] PHP：写错误日志
来源：http://yb.bookmarksfly.cn

error_log("失败: " . $e->getMessage());
来源：http://vh.shxzukj.cn

[U73] PHP：读取 ini 配置
来源：http://vf.gzmigu.cn

parse_ini_file("config.ini", true)
来源：http://hp.jianghongdianzi.cn

[U74] PHP：读取环境变量
来源：http://kr.yuntaijiaju.cn

getenv("APP_ENV") ?: "production"
来源：http://yd.nszjky.cn

[U75] PHP：依赖注入
来源：http://iq.shxzukj.cn

composer require psr/container
来源：http://bq.newstarts.cn

[U76] PHP：简单路由
来源：http://sx.chemitech.net.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yb.chemitech.net.cn

[U77] PHP：模板渲染
来源：http://ag.huanxung.cn

composer require twig/twig
来源：http://di.jianghongdianzi.cn

[U78] PHP：单元测试
来源：http://jh.jctech888.com.cn

composer require --dev phpunit/phpunit
来源：http://xv.asd995.cn

[U79] PHP：静态分析
来源：http://dk.9csxet.cn

composer require --dev phpstan/phpstan
来源：http://qj.shtwfgs.cn

[U80] PHP：代码规范修复
来源：http://sh.hahajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://zo.szxytkj.cn

[U81] JS：初始化项目
来源：http://ge.huixinmuqiang.cn

npm init -y;  npm i express
来源：http://fz.yuexingan06.cn

[U82] JS：package.json 脚本
来源：http://li.haigaiapp.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jx.muxihuayi.cn


<!-- 参考信息 -->