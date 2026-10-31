代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rp.yuexingan06.cn

================================================================================
来源：http://ty.shxzskj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qi.lnxyls.cn

================================================================================
来源：http://vt.chemitech.net.cn

[T01] Kotlin：Hello World
来源：http://an.bjjhwx.cn

println("Hello")
来源：http://zd.haigaiapp.cn

[T02] Kotlin：变量
来源：http://ve.bookmarksfly.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qs.colortex.cn

[T03] Kotlin：字符串模板
来源：http://nz.szxytkj.cn

"值: $b"
来源：http://mx.chemitech.net.cn

[T04] Kotlin：空安全
来源：http://hg.yuntaijiaju.cn

val n: String? = null;  n?.length
来源：http://zs.chemitech.net.cn

[T05] Kotlin：when 表达式
来源：http://sx.huanxung.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kj.huixinmuqiang.cn

[T06] Kotlin：集合映射
来源：http://xv.panjiajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xe.newstarts.cn

[T07] Kotlin：集合过滤
来源：http://vn.huixiangedu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://se.colortex.cn

[T08] Kotlin：数据类
来源：http://ud.nszjky.cn

data class User(val name: String, val age: Int)
来源：http://he.bjjhwx.cn

[T09] Kotlin：扩展函数
来源：http://of.haigaiapp.cn

fun String.exclaim() = this + "!"
来源：http://de.huixinmuqiang.cn

[T10] Kotlin：默认参数
来源：http://hq.gzmigu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://to.huanxung.cn

[T11] Kotlin：协程
来源：http://wp.nszjky.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://tm.lnxyls.cn

[T12] Kotlin：解构声明
来源：http://vx.shtwfgs.cn

val (a, b) = Pair(1, 2)
来源：http://du.shxzukj.cn

[T13] Kotlin：只读 Map
来源：http://gb.shtwfgs.cn

val m = mapOf("a" to 1)
来源：http://ai.chemitech.net.cn

[T14] Kotlin：循环
来源：http://pd.jianghongdianzi.cn

for (i in 1..10) println(i)
来源：http://pl.jianghongdianzi.cn

[T15] Kotlin：接口
来源：http://ri.jctech888.com.cn

interface Shape { fun area(): Double }
来源：http://dp.haigaiapp.cn

[T16] Swift：Hello World
来源：http://rr.lnxyls.cn

print("Hello")
来源：http://oi.521024.cn

[T17] Swift：变量与常量
来源：http://lx.asd995.cn

var a = 1;  let b = 2
来源：http://as.huixinmuqiang.cn

[T18] Swift：字符串插值
来源：http://gx.nszjky.cn

"值: \(b)"
来源：http://zw.hahajie.cn

[T19] Swift：可选绑定
来源：http://tt.shxzskj.cn

if let n = opt { print(n) }
来源：http://ai.panjiajie.cn

[T20] Swift：数组操作
来源：http://su.jctech888.com.cn

var a = [1, 2, 3];  a.append(4)
来源：http://oa.nszjky.cn

[T21] Swift：遍历
来源：http://pb.huixiangedu.cn

for x in a { print(x) }
来源：http://kl.newstarts.cn

[T22] Swift：字典
来源：http://zr.huixiangedu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mr.bookmarksfly.cn

[T23] Swift：函数
来源：http://lb.lnxyls.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nb.nicolike.cn

[T24] Swift：闭包
来源：http://cq.szsharing.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ut.hahajie.cn

[T25] Swift：结构体
来源：http://nt.yuexingan06.cn

struct P { var x: Int }
来源：http://ln.521024.cn

[T26] Swift：类与重写
来源：http://vb.shtwfgs.cn

class A: Base { override func f() {} }
来源：http://lp.szxytkj.cn

[T27] Swift：错误处理
来源：http://tb.jctech888.com.cn

do { try f() } catch { print(error) }
来源：http://hn.lnxyls.cn

[T28] Swift：枚举
来源：http://ts.shxzskj.cn

enum Color { case red, green }
来源：http://vb.shxzskj.cn

[T29] Swift：guard 提前返回
来源：http://rd.jctech888.com.cn

guard let x = opt else { return }
来源：http://vh.nszjky.cn

[T30] Swift：协议
来源：http://jl.jctech888.com.cn

protocol Shape { func area() -> Double }
来源：http://dq.huixiangedu.cn

[T31] Lua：Hello World
来源：http://ry.yuntaijiaju.cn

print("Hello")
来源：http://jl.nicolike.cn

[T32] Lua：局部变量
来源：http://cl.huixiangedu.cn

local a = 1
来源：http://ym.nicolike.cn

[T33] Lua：表（数组）
来源：http://vp.shtwfgs.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zw.szsharing.cn

[T34] Lua：遍历表
来源：http://hh.huixiangedu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ka.shxzskj.cn

[T35] Lua：字典表
来源：http://wc.chemitech.net.cn

local d = { a = 1 };  d.b = 2
来源：http://ow.wgjwhj.cn

[T36] Lua：函数
来源：http://vk.nszjky.cn

function add(a, b) return a + b end
来源：http://xv.haigaiapp.cn

[T37] Lua：字符串拼接
来源：http://bv.muxihuayi.cn

"a" .. "b"
来源：http://xc.521024.cn

[T38] Lua：条件
来源：http://bc.huanxung.cn

if x > 0 then print("正") end
来源：http://oi.panjiajie.cn

[T39] Lua：模式匹配
来源：http://ij.bjjhwx.cn

string.find(s, "%d+")
来源：http://ow.yuntaijiaju.cn

[T40] Lua：元表
来源：http://jc.gzmigu.cn

setmetatable({}, { __index = base })
来源：http://ve.szxytkj.cn

[T41] Perl：Hello World
来源：http://aq.colortex.cn

print "Hello\n";
来源：http://dq.panjiajie.cn

[T42] Perl：变量类型
来源：http://va.lnxyls.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cq.shxzskj.cn

[T43] Perl：字符串插值
来源：http://vl.bookmarksfly.cn

"值: $a"
来源：http://sv.hnjuh.cn

[T44] Perl：条件
来源：http://nn.nicolike.cn

if ($a > 0) { print "正"; }
来源：http://ik.huixiangedu.cn

[T45] Perl：数组遍历
来源：http://bx.colortex.cn

for my $x (@arr) { print $x; }
来源：http://jq.nszjky.cn

[T46] Perl：哈希操作
来源：http://nk.nszjky.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://aa.yuntaijiaju.cn

[T47] Perl：正则捕获
来源：http://hb.gzmigu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://yc.haigaiapp.cn

[T48] Perl：正则替换
来源：http://ht.bookmarksfly.cn

$s =~ s/old/new/g;
来源：http://ef.nszjky.cn

[T49] Perl：函数
来源：http://vb.nicolike.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ew.nicolike.cn

[T50] Perl：逐行读文件
来源：http://eq.shxzskj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zn.colortex.cn

while (my $line = <$fh>) { print $line; }
来源：http://ws.huixinmuqiang.cn

[T51] Scala：Hello World
来源：http://if.9csxet.cn

println("Hello")
来源：http://me.nicolike.cn

[T52] Scala：变量
来源：http://vz.yuexingan06.cn

val a = 1;  var b = 2
来源：http://bx.wgjwhj.cn

[T53] Scala：字符串插值
来源：http://sa.hahajie.cn

s"值: $b"
来源：http://io.huixinmuqiang.cn

[T54] Scala：集合映射
来源：http://ut.gzmigu.cn

List(1, 2, 3).map(_ * 2)
来源：http://qh.szxytkj.cn

[T55] Scala：集合过滤
来源：http://hn.nszjky.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xw.jianghongdianzi.cn

[T56] Scala：样例类
来源：http://px.jctech888.com.cn

case class User(name: String, age: Int)
来源：http://sr.521024.cn

[T57] Scala：模式匹配
来源：http://gn.panjiajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://yj.gzmigu.cn

[T58] Scala：函数定义
来源：http://je.yuntaijiaju.cn

def add(a: Int, b: Int): Int = a + b
来源：http://lt.yuntaijiaju.cn

[T59] Scala：循环
来源：http://bi.shtwfgs.cn

for (i <- 1 to 10) println(i)
来源：http://hw.jianghongdianzi.cn

[T60] Scala：折叠
来源：http://tv.jianghongdianzi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ar.colortex.cn

================================================================================
来源：http://bt.gzmigu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lt.haigaiapp.cn

================================================================================
来源：http://yb.wgjwhj.cn

[U01] Py：创建虚拟环境
来源：http://nc.colortex.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ls.wgjwhj.cn

[U02] Py：导出 / 安装依赖
来源：http://pv.haigaiapp.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zx.gzmigu.cn

[U03] Py：加载 .env 配置
来源：http://kx.yuntaijiaju.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://pd.bjjhwx.cn

[U04] Py：变量调试打印
来源：http://pd.hnjuh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ce.shxzukj.cn

[U05] Py：列表去重且保序
来源：http://qz.szsharing.cn

list(dict.fromkeys(arr))
来源：http://di.521024.cn

[U06] Py：合并两个字典
来源：http://ec.szxytkj.cn

{**a, **b}
来源：http://gl.shxzskj.cn

[U07] Py：反转字典键值
来源：http://jf.huanxung.cn

{v: k for k, v in d.items()}
来源：http://kk.szxytkj.cn

[U08] Py：展平二维列表
来源：http://yl.nszjky.cn

[y for x in nested for y in x]
来源：http://hg.colortex.cn

[U09] Py：字典取最大值的键
来源：http://zk.newstarts.cn

max(d, key=d.get)
来源：http://ie.newstarts.cn

[U10] Py：按值排序字典
来源：http://wt.huixinmuqiang.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wf.huanxung.cn

[U11] Py：生成器表达式
来源：http://lf.huixinmuqiang.cn

(x * 2 for x in arr)
来源：http://cy.szxytkj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://hy.nszjky.cn

Counter(arr).most_common(3)
来源：http://bn.lnxyls.cn

[U13] Py：固定长度队列
来源：http://gz.szsharing.cn

deque(maxlen=10)
来源：http://hq.lnxyls.cn

[U14] Py：分组收集到列表
来源：http://ld.panjiajie.cn

defaultdict(list)
来源：http://lt.nicolike.cn

[U15] Py：高精度计时
来源：http://wf.hahajie.cn

t = time.perf_counter()
来源：http://pm.bjjhwx.cn

[U16] Py：命令行参数解析
来源：http://es.panjiajie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sx.huixiangedu.cn

[U17] Py：初始化日志
来源：http://rc.chemitech.net.cn

logging.basicConfig(level=logging.INFO)
来源：http://oa.nicolike.cn

[U18] Py：预编译正则
来源：http://bm.yuexingan06.cn

pat = re.compile(r"\d+")
来源：http://fw.bjjhwx.cn

[U19] Py：正则替换带回调
来源：http://uq.jctech888.com.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tj.jctech888.com.cn

[U20] Py：缓存函数结果
来源：http://sv.bjjhwx.cn

@functools.lru_cache(maxsize=None)
来源：http://ye.nszjky.cn

[U21] Py：自定义上下文管理器
来源：http://ah.gzmigu.cn

@contextlib.contextmanager
来源：http://jo.yuntaijiaju.cn

[U22] Py：矩阵转置
来源：http://cl.521024.cn

list(zip(*m))
来源：http://pi.szsharing.cn

[U23] Py：分块读取大文件
来源：http://ez.521024.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ah.asd995.cn

[U24] Py：路径操作
来源：http://bf.wgjwhj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wf.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://dp.huixiangedu.cn

csv.DictReader(f)
来源：http://gi.gzmigu.cn

[U26] Py：并发下载
来源：http://wc.jctech888.com.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ir.colortex.cn

[U27] Py：异步 HTTP
来源：http://hw.huixiangedu.cn

aiohttp.ClientSession() 配合 async with
来源：http://tp.gzmigu.cn

[U28] Py：类型别名
来源：http://aj.huixinmuqiang.cn

UserId = int
来源：http://db.colortex.cn

[U29] Py：属性校验
来源：http://wp.huixinmuqiang.cn

@property 与 @x.setter 配合
来源：http://ks.huixiangedu.cn

[U30] Py：数据类
来源：http://ke.muxihuayi.cn

@dataclass(slots=True)
来源：http://vy.9csxet.cn

[U31] Py：单测
来源：http://gm.9csxet.cn

python -m pytest -q
来源：http://dj.haigaiapp.cn

[U32] Py：代码格式化
来源：http://dx.bjjhwx.cn

ruff format . && ruff check --fix .
来源：http://ja.szsharing.cn

[U33] Py：打包发布
来源：http://lq.hnjuh.cn

python -m build  （依赖 pyproject.toml）
来源：http://va.yuexingan06.cn

[U34] Py：判断编码
来源：http://sq.yuexingan06.cn

chardet.detect(raw)
来源：http://iw.muxihuayi.cn

[U35] Py：发送邮件
来源：http://ru.yuexingan06.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yu.yuntaijiaju.cn

[U36] Py：定时任务
来源：http://ns.jianghongdianzi.cn

schedule.every(10).minutes.do(job)
来源：http://ow.panjiajie.cn

[U37] Py：读写 Excel
来源：http://id.hnjuh.cn

pandas.read_excel / DataFrame.to_excel
来源：http://kv.yuntaijiaju.cn

[U38] Py：获取脚本所在目录
来源：http://gv.521024.cn

Path(__file__).resolve().parent
来源：http://zl.muxihuayi.cn

[U39] Py：判断是否在交互环境
来源：http://tc.chemitech.net.cn

sys.stdout.isatty()
来源：http://fq.lnxyls.cn

[U40] Py：打印到标准错误
来源：http://hc.huixinmuqiang.cn

print("err", file=sys.stderr)
来源：http://wx.521024.cn

[U41] PHP：初始化 Composer 项目
来源：http://cd.panjiajie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://fz.521024.cn

[U42] PHP：PSR-4 自动加载
来源：http://hu.nszjky.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hh.nszjky.cn

[U43] PHP：声明命名空间
来源：http://oh.newstarts.cn

namespace App\Http;
来源：http://sc.huanxung.cn

[U44] PHP：开启严格类型
来源：http://wi.colortex.cn

declare(strict_types=1);
来源：http://kx.shtwfgs.cn

[U45] PHP：类型声明与返回类型
来源：http://kd.panjiajie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://uh.yuntaijiaju.cn

[U46] PHP：可空类型
来源：http://lm.szxytkj.cn

?string $name = null
来源：http://bw.bjjhwx.cn

[U47] PHP：联合类型
来源：http://tk.jianghongdianzi.cn

int|string $id
来源：http://ph.shxzukj.cn

[U48] PHP：纯枚举
来源：http://tj.huixinmuqiang.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://as.bjjhwx.cn

[U49] PHP：只读属性
来源：http://ig.asd995.cn

public readonly string $name
来源：http://la.szsharing.cn

[U50] PHP：构造器属性提升
来源：http://ej.521024.cn

public function __construct(private int $id) {}
来源：http://tf.yuexingan06.cn

[U51] PHP：数组解构
来源：http://el.yuexingan06.cn

[$a, $b] = $arr;
来源：http://lg.panjiajie.cn

[U52] PHP：箭头函数
来源：http://on.huixiangedu.cn

$double = fn($x) => $x * 2;
来源：http://xe.wgjwhj.cn

[U53] PHP：空合并运算符
来源：http://wa.hahajie.cn

$v = $a ?? $b ?? "default";
来源：http://px.szsharing.cn

[U54] PHP：空安全调用
来源：http://ci.9csxet.cn

$obj?->method()
来源：http://cx.jianghongdianzi.cn

[U55] PHP：match 表达式
来源：http://mq.yuexingan06.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rq.hnjuh.cn

[U56] PHP：命名参数
来源：http://pc.shxzskj.cn

f(a: 1, b: 2)
来源：http://ch.jctech888.com.cn

[U57] PHP：字符串插值
来源：http://nb.shxzskj.cn

"值: {$a}"
来源：http://er.huixiangedu.cn

[U58] PHP：数组三件套
来源：http://vk.huixinmuqiang.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://us.nicolike.cn

[U59] PHP：自定义排序
来源：http://dc.yuexingan06.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mm.szxytkj.cn

[U60] PHP：JSON 编解码
来源：http://ss.nszjky.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://op.newstarts.cn

[U61] PHP：正则
来源：http://ph.shxzskj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hr.nicolike.cn

[U62] PHP：日期对象
来源：http://dg.wgjwhj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jn.hnjuh.cn

[U63] PHP：文件读写
来源：http://hm.nszjky.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vt.shxzskj.cn

[U64] PHP：目录遍历
来源：http://ti.jianghongdianzi.cn

glob("dir/*.php");  scandir("dir");
来源：http://ek.szsharing.cn

[U65] PHP：会话
来源：http://fq.colortex.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ma.huanxung.cn

[U66] PHP：设置 Cookie
来源：http://zz.colortex.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dv.lnxyls.cn

[U67] PHP：处理文件上传
来源：http://zl.shxzukj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lh.hahajie.cn

[U68] PHP：PDO 连接
来源：http://xk.hnjuh.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://oh.bookmarksfly.cn

[U69] PHP：PDO 预处理
来源：http://pk.colortex.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jf.gzmigu.cn

[U70] PHP：PDO 事务
来源：http://zw.szxytkj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fb.wgjwhj.cn

[U71] PHP：抛出异常
来源：http://ro.huixiangedu.cn

throw new RuntimeException("失败", 500);
来源：http://yu.shtwfgs.cn

[U72] PHP：写错误日志
来源：http://ro.lnxyls.cn

error_log("失败: " . $e->getMessage());
来源：http://sy.shxzukj.cn

[U73] PHP：读取 ini 配置
来源：http://kf.jianghongdianzi.cn

parse_ini_file("config.ini", true)
来源：http://xx.bjjhwx.cn

[U74] PHP：读取环境变量
来源：http://wf.asd995.cn

getenv("APP_ENV") ?: "production"
来源：http://lg.9csxet.cn

[U75] PHP：依赖注入
来源：http://kf.huixiangedu.cn

composer require psr/container
来源：http://pv.9csxet.cn

[U76] PHP：简单路由
来源：http://qv.szsharing.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ho.yuntaijiaju.cn

[U77] PHP：模板渲染
来源：http://gm.muxihuayi.cn

composer require twig/twig
来源：http://tc.9csxet.cn

[U78] PHP：单元测试
来源：http://pb.huixinmuqiang.cn

composer require --dev phpunit/phpunit
来源：http://bp.bjjhwx.cn

[U79] PHP：静态分析
来源：http://ln.yuexingan06.cn

composer require --dev phpstan/phpstan
来源：http://by.panjiajie.cn

[U80] PHP：代码规范修复
来源：http://oq.nszjky.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qj.shxzukj.cn

[U81] JS：初始化项目
来源：http://la.hahajie.cn

npm init -y;  npm i express
来源：http://qm.shxzskj.cn

[U82] JS：package.json 脚本
来源：http://dd.gzmigu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ud.shxzskj.cn

[U83] JS：ES Module 导入导出
来源：http://uj.huanxung.cn

export const a = 1;  import { a } from "./m.js";
来源：http://iy.szsharing.cn

[U84] JS：CommonJS 写法
来源：http://px.hnjuh.cn

module.exports = { a };  const { a } = require("./m");
来源：http://xb.huixinmuqiang.cn

[U85] JS：可选链
来源：http://kp.haigaiapp.cn

a?.b?.c
来源：http://de.nszjky.cn

[U86] JS：空值合并
来源：http://zv.szxytkj.cn

a ?? b
来源：http://of.szsharing.cn


<!-- 参考信息 -->