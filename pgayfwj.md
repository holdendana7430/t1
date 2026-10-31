代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yb.huanxung.cn

[S57] C++：编译期常量
来源：http://lx.bjjhwx.cn

constexpr int N = 10;
来源：http://fi.jianghongdianzi.cn

[S58] C++：命名空间
来源：http://nf.muxihuayi.cn

namespace ns { int f() { return 1; } }
来源：http://ux.chemitech.net.cn

[S59] C++：静态断言
来源：http://vm.9csxet.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ml.szxytkj.cn

[S60] C++：遍历并删除元素
来源：http://ak.huixinmuqiang.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ow.huanxung.cn

================================================================================
来源：http://id.shtwfgs.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ej.jianghongdianzi.cn

================================================================================
来源：http://tz.shxzskj.cn

[T01] Kotlin：Hello World
来源：http://op.shtwfgs.cn

println("Hello")
来源：http://lq.panjiajie.cn

[T02] Kotlin：变量
来源：http://pt.szsharing.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ao.huanxung.cn

[T03] Kotlin：字符串模板
来源：http://ju.szxytkj.cn

"值: $b"
来源：http://do.haigaiapp.cn

[T04] Kotlin：空安全
来源：http://xv.szsharing.cn

val n: String? = null;  n?.length
来源：http://zz.nicolike.cn

[T05] Kotlin：when 表达式
来源：http://kv.szsharing.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xb.huixinmuqiang.cn

[T06] Kotlin：集合映射
来源：http://po.nicolike.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ib.nicolike.cn

[T07] Kotlin：集合过滤
来源：http://qz.bjjhwx.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://uk.gzmigu.cn

[T08] Kotlin：数据类
来源：http://dj.colortex.cn

data class User(val name: String, val age: Int)
来源：http://au.gzmigu.cn

[T09] Kotlin：扩展函数
来源：http://gu.shtwfgs.cn

fun String.exclaim() = this + "!"
来源：http://ct.hnjuh.cn

[T10] Kotlin：默认参数
来源：http://wg.shtwfgs.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ew.wgjwhj.cn

[T11] Kotlin：协程
来源：http://ls.yuntaijiaju.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://pe.shxzukj.cn

[T12] Kotlin：解构声明
来源：http://tf.yuexingan06.cn

val (a, b) = Pair(1, 2)
来源：http://mf.nszjky.cn

[T13] Kotlin：只读 Map
来源：http://gg.asd995.cn

val m = mapOf("a" to 1)
来源：http://xe.muxihuayi.cn

[T14] Kotlin：循环
来源：http://gn.huanxung.cn

for (i in 1..10) println(i)
来源：http://zl.jctech888.com.cn

[T15] Kotlin：接口
来源：http://ao.haigaiapp.cn

interface Shape { fun area(): Double }
来源：http://tv.haigaiapp.cn

[T16] Swift：Hello World
来源：http://no.yuntaijiaju.cn

print("Hello")
来源：http://cn.colortex.cn

[T17] Swift：变量与常量
来源：http://qj.szxytkj.cn

var a = 1;  let b = 2
来源：http://jd.hahajie.cn

[T18] Swift：字符串插值
来源：http://is.gzmigu.cn

"值: \(b)"
来源：http://vu.hahajie.cn

[T19] Swift：可选绑定
来源：http://jl.521024.cn

if let n = opt { print(n) }
来源：http://xu.nicolike.cn

[T20] Swift：数组操作
来源：http://wq.szsharing.cn

var a = [1, 2, 3];  a.append(4)
来源：http://oj.shxzukj.cn

[T21] Swift：遍历
来源：http://rl.chemitech.net.cn

for x in a { print(x) }
来源：http://gy.panjiajie.cn

[T22] Swift：字典
来源：http://xt.jctech888.com.cn

var d = ["a": 1];  d["b"] = 2
来源：http://yl.bookmarksfly.cn

[T23] Swift：函数
来源：http://hl.huixinmuqiang.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://js.colortex.cn

[T24] Swift：闭包
来源：http://zw.jianghongdianzi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://bm.shtwfgs.cn

[T25] Swift：结构体
来源：http://xa.nszjky.cn

struct P { var x: Int }
来源：http://ko.jctech888.com.cn

[T26] Swift：类与重写
来源：http://lt.9csxet.cn

class A: Base { override func f() {} }
来源：http://zr.shxzskj.cn

[T27] Swift：错误处理
来源：http://gq.521024.cn

do { try f() } catch { print(error) }
来源：http://he.yuexingan06.cn

[T28] Swift：枚举
来源：http://kh.gzmigu.cn

enum Color { case red, green }
来源：http://zi.lnxyls.cn

[T29] Swift：guard 提前返回
来源：http://xy.hahajie.cn

guard let x = opt else { return }
来源：http://mo.muxihuayi.cn

[T30] Swift：协议
来源：http://kn.shxzskj.cn

protocol Shape { func area() -> Double }
来源：http://lm.huanxung.cn

[T31] Lua：Hello World
来源：http://kk.szxytkj.cn

print("Hello")
来源：http://wx.shtwfgs.cn

[T32] Lua：局部变量
来源：http://eo.szxytkj.cn

local a = 1
来源：http://qh.hnjuh.cn

[T33] Lua：表（数组）
来源：http://rz.panjiajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://jg.haigaiapp.cn

[T34] Lua：遍历表
来源：http://en.shxzskj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ao.wgjwhj.cn

[T35] Lua：字典表
来源：http://tn.521024.cn

local d = { a = 1 };  d.b = 2
来源：http://fu.colortex.cn

[T36] Lua：函数
来源：http://bz.bjjhwx.cn

function add(a, b) return a + b end
来源：http://rw.nicolike.cn

[T37] Lua：字符串拼接
来源：http://el.521024.cn

"a" .. "b"
来源：http://nr.hnjuh.cn

[T38] Lua：条件
来源：http://tx.panjiajie.cn

if x > 0 then print("正") end
来源：http://bj.huixinmuqiang.cn

[T39] Lua：模式匹配
来源：http://jk.asd995.cn

string.find(s, "%d+")
来源：http://au.nszjky.cn

[T40] Lua：元表
来源：http://kb.yuexingan06.cn

setmetatable({}, { __index = base })
来源：http://xr.asd995.cn

[T41] Perl：Hello World
来源：http://ey.nicolike.cn

print "Hello\n";
来源：http://ej.asd995.cn

[T42] Perl：变量类型
来源：http://nh.huanxung.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fk.jianghongdianzi.cn

[T43] Perl：字符串插值
来源：http://je.wgjwhj.cn

"值: $a"
来源：http://mk.hnjuh.cn

[T44] Perl：条件
来源：http://ki.hnjuh.cn

if ($a > 0) { print "正"; }
来源：http://pz.chemitech.net.cn

[T45] Perl：数组遍历
来源：http://hs.bjjhwx.cn

for my $x (@arr) { print $x; }
来源：http://ay.shtwfgs.cn

[T46] Perl：哈希操作
来源：http://xk.lnxyls.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gc.wgjwhj.cn

[T47] Perl：正则捕获
来源：http://eu.huixiangedu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://gg.szsharing.cn

[T48] Perl：正则替换
来源：http://tp.lnxyls.cn

$s =~ s/old/new/g;
来源：http://xa.shtwfgs.cn

[T49] Perl：函数
来源：http://os.yuexingan06.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jf.shxzskj.cn

[T50] Perl：逐行读文件
来源：http://bo.521024.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://cc.gzmigu.cn

while (my $line = <$fh>) { print $line; }
来源：http://sl.colortex.cn

[T51] Scala：Hello World
来源：http://vt.lnxyls.cn

println("Hello")
来源：http://xi.jianghongdianzi.cn

[T52] Scala：变量
来源：http://mf.nszjky.cn

val a = 1;  var b = 2
来源：http://jk.huixiangedu.cn

[T53] Scala：字符串插值
来源：http://fy.bjjhwx.cn

s"值: $b"
来源：http://bq.huixiangedu.cn

[T54] Scala：集合映射
来源：http://kd.lnxyls.cn

List(1, 2, 3).map(_ * 2)
来源：http://yd.szxytkj.cn

[T55] Scala：集合过滤
来源：http://no.521024.cn

List(1, 2, 3).filter(_ > 1)
来源：http://vu.hnjuh.cn

[T56] Scala：样例类
来源：http://jq.lnxyls.cn

case class User(name: String, age: Int)
来源：http://ce.wgjwhj.cn

[T57] Scala：模式匹配
来源：http://jt.hahajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://la.lnxyls.cn

[T58] Scala：函数定义
来源：http://pw.wgjwhj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://sv.bjjhwx.cn

[T59] Scala：循环
来源：http://qx.szxytkj.cn

for (i <- 1 to 10) println(i)
来源：http://yd.nszjky.cn

[T60] Scala：折叠
来源：http://za.shxzskj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://oc.asd995.cn

================================================================================
来源：http://tw.shxzskj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fa.jctech888.com.cn

================================================================================
来源：http://wu.szsharing.cn

[U01] Py：创建虚拟环境
来源：http://pw.nszjky.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qh.newstarts.cn

[U02] Py：导出 / 安装依赖
来源：http://zq.panjiajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://up.9csxet.cn

[U03] Py：加载 .env 配置
来源：http://zs.szxytkj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://vm.jianghongdianzi.cn

[U04] Py：变量调试打印
来源：http://mb.szsharing.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dm.hnjuh.cn

[U05] Py：列表去重且保序
来源：http://yz.haigaiapp.cn

list(dict.fromkeys(arr))
来源：http://sz.asd995.cn

[U06] Py：合并两个字典
来源：http://zj.9csxet.cn

{**a, **b}
来源：http://dz.hnjuh.cn

[U07] Py：反转字典键值
来源：http://ab.bjjhwx.cn

{v: k for k, v in d.items()}
来源：http://su.hnjuh.cn

[U08] Py：展平二维列表
来源：http://bl.nicolike.cn

[y for x in nested for y in x]
来源：http://pr.hahajie.cn

[U09] Py：字典取最大值的键
来源：http://tm.9csxet.cn

max(d, key=d.get)
来源：http://ri.9csxet.cn

[U10] Py：按值排序字典
来源：http://mf.9csxet.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rr.jctech888.com.cn

[U11] Py：生成器表达式
来源：http://yp.9csxet.cn

(x * 2 for x in arr)
来源：http://nx.shxzskj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ab.9csxet.cn

Counter(arr).most_common(3)
来源：http://pr.szxytkj.cn

[U13] Py：固定长度队列
来源：http://yr.nicolike.cn

deque(maxlen=10)
来源：http://ci.newstarts.cn

[U14] Py：分组收集到列表
来源：http://fm.bookmarksfly.cn

defaultdict(list)
来源：http://ip.shxzukj.cn

[U15] Py：高精度计时
来源：http://tu.hnjuh.cn

t = time.perf_counter()
来源：http://dl.shxzukj.cn

[U16] Py：命令行参数解析
来源：http://ma.huanxung.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rt.chemitech.net.cn

[U17] Py：初始化日志
来源：http://br.jianghongdianzi.cn

logging.basicConfig(level=logging.INFO)
来源：http://xj.szsharing.cn

[U18] Py：预编译正则
来源：http://iy.shxzskj.cn

pat = re.compile(r"\d+")
来源：http://qi.colortex.cn

[U19] Py：正则替换带回调
来源：http://tm.yuntaijiaju.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://td.gzmigu.cn

[U20] Py：缓存函数结果
来源：http://im.szsharing.cn

@functools.lru_cache(maxsize=None)
来源：http://ej.huanxung.cn

[U21] Py：自定义上下文管理器
来源：http://zv.szxytkj.cn

@contextlib.contextmanager
来源：http://xk.jctech888.com.cn

[U22] Py：矩阵转置
来源：http://yv.huixinmuqiang.cn

list(zip(*m))
来源：http://wo.szsharing.cn

[U23] Py：分块读取大文件
来源：http://to.jctech888.com.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ns.huixinmuqiang.cn

[U24] Py：路径操作
来源：http://wr.huanxung.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ud.nicolike.cn

[U25] Py：CSV 按字典读
来源：http://wk.huanxung.cn

csv.DictReader(f)
来源：http://he.asd995.cn

[U26] Py：并发下载
来源：http://sp.bookmarksfly.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xr.shxzskj.cn

[U27] Py：异步 HTTP
来源：http://vy.nszjky.cn

aiohttp.ClientSession() 配合 async with
来源：http://kj.hahajie.cn

[U28] Py：类型别名
来源：http://mo.bookmarksfly.cn

UserId = int
来源：http://bg.nicolike.cn

[U29] Py：属性校验
来源：http://zf.nicolike.cn

@property 与 @x.setter 配合
来源：http://ch.lnxyls.cn

[U30] Py：数据类
来源：http://ze.nicolike.cn

@dataclass(slots=True)
来源：http://af.chemitech.net.cn

[U31] Py：单测
来源：http://xk.9csxet.cn

python -m pytest -q
来源：http://ov.nszjky.cn

[U32] Py：代码格式化
来源：http://tr.gzmigu.cn

ruff format . && ruff check --fix .
来源：http://in.shxzskj.cn

[U33] Py：打包发布
来源：http://fm.hnjuh.cn

python -m build  （依赖 pyproject.toml）
来源：http://bu.muxihuayi.cn

[U34] Py：判断编码
来源：http://ty.colortex.cn

chardet.detect(raw)
来源：http://wa.lnxyls.cn

[U35] Py：发送邮件
来源：http://ou.shxzskj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ey.gzmigu.cn

[U36] Py：定时任务
来源：http://aq.huanxung.cn

schedule.every(10).minutes.do(job)
来源：http://kt.bjjhwx.cn

[U37] Py：读写 Excel
来源：http://ts.yuntaijiaju.cn

pandas.read_excel / DataFrame.to_excel
来源：http://kt.newstarts.cn

[U38] Py：获取脚本所在目录
来源：http://ms.lnxyls.cn

Path(__file__).resolve().parent
来源：http://xr.9csxet.cn

[U39] Py：判断是否在交互环境
来源：http://mq.huanxung.cn

sys.stdout.isatty()
来源：http://me.huixinmuqiang.cn

[U40] Py：打印到标准错误
来源：http://gx.shtwfgs.cn

print("err", file=sys.stderr)
来源：http://hk.521024.cn

[U41] PHP：初始化 Composer 项目
来源：http://kf.newstarts.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qw.jianghongdianzi.cn

[U42] PHP：PSR-4 自动加载
来源：http://km.yuntaijiaju.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rw.gzmigu.cn

[U43] PHP：声明命名空间
来源：http://au.shxzskj.cn

namespace App\Http;
来源：http://fd.huixiangedu.cn

[U44] PHP：开启严格类型
来源：http://ag.hahajie.cn

declare(strict_types=1);
来源：http://ky.wgjwhj.cn

[U45] PHP：类型声明与返回类型
来源：http://ga.jianghongdianzi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://eb.panjiajie.cn

[U46] PHP：可空类型
来源：http://ip.szsharing.cn

?string $name = null
来源：http://qn.wgjwhj.cn

[U47] PHP：联合类型
来源：http://kg.shxzskj.cn

int|string $id
来源：http://bd.szxytkj.cn

[U48] PHP：纯枚举
来源：http://nq.newstarts.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bj.bookmarksfly.cn

[U49] PHP：只读属性
来源：http://qu.newstarts.cn

public readonly string $name
来源：http://vp.yuntaijiaju.cn

[U50] PHP：构造器属性提升
来源：http://fe.yuntaijiaju.cn

public function __construct(private int $id) {}
来源：http://bg.jctech888.com.cn

[U51] PHP：数组解构
来源：http://bh.newstarts.cn

[$a, $b] = $arr;
来源：http://bo.shxzukj.cn

[U52] PHP：箭头函数
来源：http://yl.jianghongdianzi.cn

$double = fn($x) => $x * 2;
来源：http://je.hahajie.cn

[U53] PHP：空合并运算符
来源：http://rd.huixinmuqiang.cn

$v = $a ?? $b ?? "default";
来源：http://xz.hahajie.cn

[U54] PHP：空安全调用
来源：http://pp.lnxyls.cn

$obj?->method()
来源：http://kt.shtwfgs.cn

[U55] PHP：match 表达式
来源：http://za.9csxet.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qc.szsharing.cn

[U56] PHP：命名参数
来源：http://co.huanxung.cn

f(a: 1, b: 2)
来源：http://hy.panjiajie.cn

[U57] PHP：字符串插值
来源：http://av.hnjuh.cn

"值: {$a}"
来源：http://bz.yuntaijiaju.cn

[U58] PHP：数组三件套
来源：http://dh.newstarts.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pj.szxytkj.cn

[U59] PHP：自定义排序
来源：http://zg.nszjky.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dd.huanxung.cn

[U60] PHP：JSON 编解码
来源：http://ts.colortex.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qq.huixinmuqiang.cn

[U61] PHP：正则
来源：http://wj.szxytkj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://py.521024.cn

[U62] PHP：日期对象
来源：http://cr.bjjhwx.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wh.bookmarksfly.cn

[U63] PHP：文件读写
来源：http://ko.jianghongdianzi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://uh.nicolike.cn

[U64] PHP：目录遍历
来源：http://gx.9csxet.cn

glob("dir/*.php");  scandir("dir");
来源：http://qk.9csxet.cn

[U65] PHP：会话
来源：http://ae.9csxet.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://lj.panjiajie.cn

[U66] PHP：设置 Cookie
来源：http://iy.shtwfgs.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vn.nszjky.cn

[U67] PHP：处理文件上传
来源：http://rp.bookmarksfly.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://oy.bjjhwx.cn

[U68] PHP：PDO 连接
来源：http://km.asd995.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://na.521024.cn

[U69] PHP：PDO 预处理
来源：http://vu.shxzskj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yg.newstarts.cn

[U70] PHP：PDO 事务
来源：http://bc.newstarts.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.hnjuh.cn

[U71] PHP：抛出异常
来源：http://lt.yuexingan06.cn

throw new RuntimeException("失败", 500);
来源：http://se.hahajie.cn

[U72] PHP：写错误日志
来源：http://xe.yuntaijiaju.cn

error_log("失败: " . $e->getMessage());
来源：http://kr.hnjuh.cn

[U73] PHP：读取 ini 配置
来源：http://gj.gzmigu.cn

parse_ini_file("config.ini", true)
来源：http://sn.9csxet.cn

[U74] PHP：读取环境变量
来源：http://ef.wgjwhj.cn

getenv("APP_ENV") ?: "production"
来源：http://ai.chemitech.net.cn

[U75] PHP：依赖注入
来源：http://fp.newstarts.cn

composer require psr/container
来源：http://jn.hnjuh.cn

[U76] PHP：简单路由
来源：http://vt.jctech888.com.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dm.chemitech.net.cn

[U77] PHP：模板渲染
来源：http://sv.szsharing.cn

composer require twig/twig
来源：http://bc.haigaiapp.cn

[U78] PHP：单元测试
来源：http://sm.asd995.cn

composer require --dev phpunit/phpunit
来源：http://fv.hahajie.cn

[U79] PHP：静态分析
来源：http://va.yuexingan06.cn

composer require --dev phpstan/phpstan
来源：http://iy.nszjky.cn

[U80] PHP：代码规范修复
来源：http://er.bookmarksfly.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://bk.haigaiapp.cn

[U81] JS：初始化项目
来源：http://lu.yuntaijiaju.cn

npm init -y;  npm i express
来源：http://mg.newstarts.cn

[U82] JS：package.json 脚本
来源：http://ep.shxzskj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nx.9csxet.cn


<!-- 参考信息 -->