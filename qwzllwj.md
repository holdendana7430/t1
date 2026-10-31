代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://rq.bookmarksfly.cn

[S59] C++：静态断言
来源：http://ye.gzmigu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://iv.chemitech.net.cn

[S60] C++：遍历并删除元素
来源：http://ou.muxihuayi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vr.shxzukj.cn

================================================================================
来源：http://sb.chemitech.net.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://aq.nszjky.cn

================================================================================
来源：http://fg.jctech888.com.cn

[T01] Kotlin：Hello World
来源：http://lo.szsharing.cn

println("Hello")
来源：http://mv.szsharing.cn

[T02] Kotlin：变量
来源：http://ze.jianghongdianzi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fn.szsharing.cn

[T03] Kotlin：字符串模板
来源：http://js.szsharing.cn

"值: $b"
来源：http://jz.bookmarksfly.cn

[T04] Kotlin：空安全
来源：http://we.huixinmuqiang.cn

val n: String? = null;  n?.length
来源：http://fi.wgjwhj.cn

[T05] Kotlin：when 表达式
来源：http://fy.shxzskj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tp.jianghongdianzi.cn

[T06] Kotlin：集合映射
来源：http://to.bjjhwx.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://va.huixiangedu.cn

[T07] Kotlin：集合过滤
来源：http://pt.jianghongdianzi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tm.yuntaijiaju.cn

[T08] Kotlin：数据类
来源：http://lj.panjiajie.cn

data class User(val name: String, val age: Int)
来源：http://dt.asd995.cn

[T09] Kotlin：扩展函数
来源：http://nc.hnjuh.cn

fun String.exclaim() = this + "!"
来源：http://qa.yuexingan06.cn

[T10] Kotlin：默认参数
来源：http://zm.shxzukj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tr.huixiangedu.cn

[T11] Kotlin：协程
来源：http://el.chemitech.net.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://cf.colortex.cn

[T12] Kotlin：解构声明
来源：http://um.yuexingan06.cn

val (a, b) = Pair(1, 2)
来源：http://dc.szxytkj.cn

[T13] Kotlin：只读 Map
来源：http://vf.yuntaijiaju.cn

val m = mapOf("a" to 1)
来源：http://mf.9csxet.cn

[T14] Kotlin：循环
来源：http://df.jianghongdianzi.cn

for (i in 1..10) println(i)
来源：http://oa.hahajie.cn

[T15] Kotlin：接口
来源：http://kz.gzmigu.cn

interface Shape { fun area(): Double }
来源：http://bh.huixiangedu.cn

[T16] Swift：Hello World
来源：http://pn.wgjwhj.cn

print("Hello")
来源：http://qn.szxytkj.cn

[T17] Swift：变量与常量
来源：http://ue.panjiajie.cn

var a = 1;  let b = 2
来源：http://kn.muxihuayi.cn

[T18] Swift：字符串插值
来源：http://mb.huixiangedu.cn

"值: \(b)"
来源：http://sd.wgjwhj.cn

[T19] Swift：可选绑定
来源：http://en.shxzskj.cn

if let n = opt { print(n) }
来源：http://yz.nicolike.cn

[T20] Swift：数组操作
来源：http://yi.newstarts.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hf.nicolike.cn

[T21] Swift：遍历
来源：http://ff.szsharing.cn

for x in a { print(x) }
来源：http://oh.huixinmuqiang.cn

[T22] Swift：字典
来源：http://qr.hahajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://lz.huixiangedu.cn

[T23] Swift：函数
来源：http://bw.shxzukj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dj.szsharing.cn

[T24] Swift：闭包
来源：http://wh.yuntaijiaju.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://op.shxzukj.cn

[T25] Swift：结构体
来源：http://vd.shxzskj.cn

struct P { var x: Int }
来源：http://hz.nszjky.cn

[T26] Swift：类与重写
来源：http://ez.jctech888.com.cn

class A: Base { override func f() {} }
来源：http://fi.muxihuayi.cn

[T27] Swift：错误处理
来源：http://gj.jianghongdianzi.cn

do { try f() } catch { print(error) }
来源：http://bu.haigaiapp.cn

[T28] Swift：枚举
来源：http://nn.gzmigu.cn

enum Color { case red, green }
来源：http://hj.huanxung.cn

[T29] Swift：guard 提前返回
来源：http://ur.521024.cn

guard let x = opt else { return }
来源：http://kv.bookmarksfly.cn

[T30] Swift：协议
来源：http://xk.shtwfgs.cn

protocol Shape { func area() -> Double }
来源：http://zp.yuexingan06.cn

[T31] Lua：Hello World
来源：http://ve.shxzskj.cn

print("Hello")
来源：http://bk.bookmarksfly.cn

[T32] Lua：局部变量
来源：http://qx.jianghongdianzi.cn

local a = 1
来源：http://wq.shxzskj.cn

[T33] Lua：表（数组）
来源：http://nh.nszjky.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://oc.lnxyls.cn

[T34] Lua：遍历表
来源：http://ig.wgjwhj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://le.bookmarksfly.cn

[T35] Lua：字典表
来源：http://kg.haigaiapp.cn

local d = { a = 1 };  d.b = 2
来源：http://ph.szsharing.cn

[T36] Lua：函数
来源：http://fr.muxihuayi.cn

function add(a, b) return a + b end
来源：http://hb.szsharing.cn

[T37] Lua：字符串拼接
来源：http://bb.jianghongdianzi.cn

"a" .. "b"
来源：http://xc.hnjuh.cn

[T38] Lua：条件
来源：http://mp.muxihuayi.cn

if x > 0 then print("正") end
来源：http://cs.shxzskj.cn

[T39] Lua：模式匹配
来源：http://hz.hnjuh.cn

string.find(s, "%d+")
来源：http://qp.newstarts.cn

[T40] Lua：元表
来源：http://bz.hahajie.cn

setmetatable({}, { __index = base })
来源：http://gw.jctech888.com.cn

[T41] Perl：Hello World
来源：http://kn.bookmarksfly.cn

print "Hello\n";
来源：http://hj.huixiangedu.cn

[T42] Perl：变量类型
来源：http://yt.hahajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://su.yuexingan06.cn

[T43] Perl：字符串插值
来源：http://lu.shxzukj.cn

"值: $a"
来源：http://tw.panjiajie.cn

[T44] Perl：条件
来源：http://zf.jctech888.com.cn

if ($a > 0) { print "正"; }
来源：http://qi.newstarts.cn

[T45] Perl：数组遍历
来源：http://fg.shxzukj.cn

for my $x (@arr) { print $x; }
来源：http://hn.chemitech.net.cn

[T46] Perl：哈希操作
来源：http://vx.colortex.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cv.nicolike.cn

[T47] Perl：正则捕获
来源：http://ac.szsharing.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dr.521024.cn

[T48] Perl：正则替换
来源：http://pq.szsharing.cn

$s =~ s/old/new/g;
来源：http://gd.shxzskj.cn

[T49] Perl：函数
来源：http://mq.huixiangedu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qd.huixinmuqiang.cn

[T50] Perl：逐行读文件
来源：http://bi.hnjuh.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://cd.521024.cn

while (my $line = <$fh>) { print $line; }
来源：http://mo.muxihuayi.cn

[T51] Scala：Hello World
来源：http://nv.szsharing.cn

println("Hello")
来源：http://bs.yuexingan06.cn

[T52] Scala：变量
来源：http://yt.yuntaijiaju.cn

val a = 1;  var b = 2
来源：http://ju.nszjky.cn

[T53] Scala：字符串插值
来源：http://wu.wgjwhj.cn

s"值: $b"
来源：http://nf.colortex.cn

[T54] Scala：集合映射
来源：http://mo.nicolike.cn

List(1, 2, 3).map(_ * 2)
来源：http://bk.9csxet.cn

[T55] Scala：集合过滤
来源：http://eq.bjjhwx.cn

List(1, 2, 3).filter(_ > 1)
来源：http://kl.shtwfgs.cn

[T56] Scala：样例类
来源：http://qg.szxytkj.cn

case class User(name: String, age: Int)
来源：http://ik.szxytkj.cn

[T57] Scala：模式匹配
来源：http://av.colortex.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vg.jianghongdianzi.cn

[T58] Scala：函数定义
来源：http://tc.jctech888.com.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ey.nszjky.cn

[T59] Scala：循环
来源：http://xr.lnxyls.cn

for (i <- 1 to 10) println(i)
来源：http://fz.lnxyls.cn

[T60] Scala：折叠
来源：http://lg.yuntaijiaju.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://go.jctech888.com.cn

================================================================================
来源：http://my.muxihuayi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pd.panjiajie.cn

================================================================================
来源：http://pa.yuexingan06.cn

[U01] Py：创建虚拟环境
来源：http://dt.yuntaijiaju.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bl.shxzukj.cn

[U02] Py：导出 / 安装依赖
来源：http://yk.panjiajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ql.newstarts.cn

[U03] Py：加载 .env 配置
来源：http://vb.jianghongdianzi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://dv.wgjwhj.cn

[U04] Py：变量调试打印
来源：http://dy.jctech888.com.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wi.muxihuayi.cn

[U05] Py：列表去重且保序
来源：http://pj.yuexingan06.cn

list(dict.fromkeys(arr))
来源：http://rd.muxihuayi.cn

[U06] Py：合并两个字典
来源：http://qu.colortex.cn

{**a, **b}
来源：http://ex.hnjuh.cn

[U07] Py：反转字典键值
来源：http://ds.nicolike.cn

{v: k for k, v in d.items()}
来源：http://zb.shxzukj.cn

[U08] Py：展平二维列表
来源：http://en.szxytkj.cn

[y for x in nested for y in x]
来源：http://nx.huanxung.cn

[U09] Py：字典取最大值的键
来源：http://fp.chemitech.net.cn

max(d, key=d.get)
来源：http://as.lnxyls.cn

[U10] Py：按值排序字典
来源：http://zq.nszjky.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lp.huanxung.cn

[U11] Py：生成器表达式
来源：http://nh.bjjhwx.cn

(x * 2 for x in arr)
来源：http://pq.shxzukj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://sd.9csxet.cn

Counter(arr).most_common(3)
来源：http://oa.haigaiapp.cn

[U13] Py：固定长度队列
来源：http://gi.szxytkj.cn

deque(maxlen=10)
来源：http://bc.521024.cn

[U14] Py：分组收集到列表
来源：http://ka.gzmigu.cn

defaultdict(list)
来源：http://nj.newstarts.cn

[U15] Py：高精度计时
来源：http://mb.asd995.cn

t = time.perf_counter()
来源：http://dt.wgjwhj.cn

[U16] Py：命令行参数解析
来源：http://sm.muxihuayi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://om.gzmigu.cn

[U17] Py：初始化日志
来源：http://qf.huixiangedu.cn

logging.basicConfig(level=logging.INFO)
来源：http://wz.panjiajie.cn

[U18] Py：预编译正则
来源：http://jx.huixinmuqiang.cn

pat = re.compile(r"\d+")
来源：http://pt.wgjwhj.cn

[U19] Py：正则替换带回调
来源：http://xv.nicolike.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://iu.lnxyls.cn

[U20] Py：缓存函数结果
来源：http://qj.panjiajie.cn

@functools.lru_cache(maxsize=None)
来源：http://dl.lnxyls.cn

[U21] Py：自定义上下文管理器
来源：http://su.jianghongdianzi.cn

@contextlib.contextmanager
来源：http://qe.nszjky.cn

[U22] Py：矩阵转置
来源：http://fc.szxytkj.cn

list(zip(*m))
来源：http://rv.shxzukj.cn

[U23] Py：分块读取大文件
来源：http://xj.jctech888.com.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qe.muxihuayi.cn

[U24] Py：路径操作
来源：http://pm.nicolike.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://be.panjiajie.cn

[U25] Py：CSV 按字典读
来源：http://jg.bookmarksfly.cn

csv.DictReader(f)
来源：http://pz.panjiajie.cn

[U26] Py：并发下载
来源：http://ri.colortex.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fz.9csxet.cn

[U27] Py：异步 HTTP
来源：http://df.gzmigu.cn

aiohttp.ClientSession() 配合 async with
来源：http://ja.hahajie.cn

[U28] Py：类型别名
来源：http://fx.huixiangedu.cn

UserId = int
来源：http://oc.shxzukj.cn

[U29] Py：属性校验
来源：http://az.hahajie.cn

@property 与 @x.setter 配合
来源：http://ns.chemitech.net.cn

[U30] Py：数据类
来源：http://ie.hahajie.cn

@dataclass(slots=True)
来源：http://ar.jianghongdianzi.cn

[U31] Py：单测
来源：http://ig.9csxet.cn

python -m pytest -q
来源：http://is.gzmigu.cn

[U32] Py：代码格式化
来源：http://xe.szsharing.cn

ruff format . && ruff check --fix .
来源：http://av.yuntaijiaju.cn

[U33] Py：打包发布
来源：http://vx.gzmigu.cn

python -m build  （依赖 pyproject.toml）
来源：http://ym.hahajie.cn

[U34] Py：判断编码
来源：http://ju.szxytkj.cn

chardet.detect(raw)
来源：http://px.haigaiapp.cn

[U35] Py：发送邮件
来源：http://rq.nicolike.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jv.szsharing.cn

[U36] Py：定时任务
来源：http://ds.huanxung.cn

schedule.every(10).minutes.do(job)
来源：http://td.yuexingan06.cn

[U37] Py：读写 Excel
来源：http://rg.lnxyls.cn

pandas.read_excel / DataFrame.to_excel
来源：http://bz.gzmigu.cn

[U38] Py：获取脚本所在目录
来源：http://cw.shxzskj.cn

Path(__file__).resolve().parent
来源：http://ke.shxzukj.cn

[U39] Py：判断是否在交互环境
来源：http://hv.asd995.cn

sys.stdout.isatty()
来源：http://sq.newstarts.cn

[U40] Py：打印到标准错误
来源：http://bn.yuexingan06.cn

print("err", file=sys.stderr)
来源：http://oa.hahajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://cb.lnxyls.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ur.newstarts.cn

[U42] PHP：PSR-4 自动加载
来源：http://qy.huixinmuqiang.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yr.yuntaijiaju.cn

[U43] PHP：声明命名空间
来源：http://ox.lnxyls.cn

namespace App\Http;
来源：http://ii.szxytkj.cn

[U44] PHP：开启严格类型
来源：http://pu.jianghongdianzi.cn

declare(strict_types=1);
来源：http://nu.shtwfgs.cn

[U45] PHP：类型声明与返回类型
来源：http://tu.szsharing.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://lg.hahajie.cn

[U46] PHP：可空类型
来源：http://gl.asd995.cn

?string $name = null
来源：http://fw.bjjhwx.cn

[U47] PHP：联合类型
来源：http://uc.521024.cn

int|string $id
来源：http://qr.chemitech.net.cn

[U48] PHP：纯枚举
来源：http://kn.chemitech.net.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jm.muxihuayi.cn

[U49] PHP：只读属性
来源：http://wy.asd995.cn

public readonly string $name
来源：http://ue.jianghongdianzi.cn

[U50] PHP：构造器属性提升
来源：http://ha.huanxung.cn

public function __construct(private int $id) {}
来源：http://va.lnxyls.cn

[U51] PHP：数组解构
来源：http://fz.lnxyls.cn

[$a, $b] = $arr;
来源：http://if.chemitech.net.cn

[U52] PHP：箭头函数
来源：http://es.521024.cn

$double = fn($x) => $x * 2;
来源：http://sq.panjiajie.cn

[U53] PHP：空合并运算符
来源：http://tc.shxzskj.cn

$v = $a ?? $b ?? "default";
来源：http://qm.szsharing.cn

[U54] PHP：空安全调用
来源：http://mr.nszjky.cn

$obj?->method()
来源：http://ly.nszjky.cn

[U55] PHP：match 表达式
来源：http://hg.szsharing.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vy.bookmarksfly.cn

[U56] PHP：命名参数
来源：http://qf.newstarts.cn

f(a: 1, b: 2)
来源：http://qd.jianghongdianzi.cn

[U57] PHP：字符串插值
来源：http://ki.nicolike.cn

"值: {$a}"
来源：http://lm.chemitech.net.cn

[U58] PHP：数组三件套
来源：http://od.chemitech.net.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://aj.asd995.cn

[U59] PHP：自定义排序
来源：http://wc.shxzukj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bj.hahajie.cn

[U60] PHP：JSON 编解码
来源：http://bi.yuexingan06.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qz.huixiangedu.cn

[U61] PHP：正则
来源：http://cl.9csxet.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://we.shxzukj.cn

[U62] PHP：日期对象
来源：http://ig.yuexingan06.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://li.haigaiapp.cn

[U63] PHP：文件读写
来源：http://eg.shxzukj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hd.wgjwhj.cn

[U64] PHP：目录遍历
来源：http://hi.haigaiapp.cn

glob("dir/*.php");  scandir("dir");
来源：http://ut.shxzskj.cn

[U65] PHP：会话
来源：http://hg.asd995.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://qf.yuntaijiaju.cn

[U66] PHP：设置 Cookie
来源：http://qx.colortex.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fg.panjiajie.cn

[U67] PHP：处理文件上传
来源：http://ya.jianghongdianzi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://th.hahajie.cn

[U68] PHP：PDO 连接
来源：http://yr.521024.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://iv.newstarts.cn

[U69] PHP：PDO 预处理
来源：http://kv.szxytkj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://at.bjjhwx.cn

[U70] PHP：PDO 事务
来源：http://sh.gzmigu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qu.bookmarksfly.cn

[U71] PHP：抛出异常
来源：http://ff.gzmigu.cn

throw new RuntimeException("失败", 500);
来源：http://ek.szxytkj.cn

[U72] PHP：写错误日志
来源：http://le.szxytkj.cn

error_log("失败: " . $e->getMessage());
来源：http://it.521024.cn

[U73] PHP：读取 ini 配置
来源：http://fg.huanxung.cn

parse_ini_file("config.ini", true)
来源：http://oy.szxytkj.cn

[U74] PHP：读取环境变量
来源：http://rq.hahajie.cn

getenv("APP_ENV") ?: "production"
来源：http://fn.colortex.cn

[U75] PHP：依赖注入
来源：http://ws.hahajie.cn

composer require psr/container
来源：http://ft.haigaiapp.cn

[U76] PHP：简单路由
来源：http://xi.newstarts.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kk.9csxet.cn

[U77] PHP：模板渲染
来源：http://nq.shxzukj.cn

composer require twig/twig
来源：http://yb.bjjhwx.cn

[U78] PHP：单元测试
来源：http://an.huixiangedu.cn

composer require --dev phpunit/phpunit
来源：http://xo.yuexingan06.cn

[U79] PHP：静态分析
来源：http://vf.nszjky.cn

composer require --dev phpstan/phpstan
来源：http://ob.521024.cn

[U80] PHP：代码规范修复
来源：http://aa.bjjhwx.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qb.colortex.cn

[U81] JS：初始化项目
来源：http://zx.yuntaijiaju.cn

npm init -y;  npm i express
来源：http://od.521024.cn

[U82] JS：package.json 脚本
来源：http://zq.haigaiapp.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xq.bjjhwx.cn

[U83] JS：ES Module 导入导出
来源：http://ek.hnjuh.cn

export const a = 1;  import { a } from "./m.js";
来源：http://aq.bjjhwx.cn

[U84] JS：CommonJS 写法
来源：http://op.bjjhwx.cn

module.exports = { a };  const { a } = require("./m");
来源：http://pr.asd995.cn


<!-- 参考信息 -->