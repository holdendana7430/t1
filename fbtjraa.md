代发 wailian999

[T03] Kotlin：字符串模板
来源：http://iq.szsharing.cn

"值: $b"
来源：http://nb.hnjuh.cn

[T04] Kotlin：空安全
来源：http://jb.shxzskj.cn

val n: String? = null;  n?.length
来源：http://oj.huixinmuqiang.cn

[T05] Kotlin：when 表达式
来源：http://mv.muxihuayi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://un.newstarts.cn

[T06] Kotlin：集合映射
来源：http://he.yuntaijiaju.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://la.huixiangedu.cn

[T07] Kotlin：集合过滤
来源：http://hz.hahajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://eo.shxzskj.cn

[T08] Kotlin：数据类
来源：http://af.nszjky.cn

data class User(val name: String, val age: Int)
来源：http://gs.huixiangedu.cn

[T09] Kotlin：扩展函数
来源：http://ug.bjjhwx.cn

fun String.exclaim() = this + "!"
来源：http://pr.bjjhwx.cn

[T10] Kotlin：默认参数
来源：http://mp.hahajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ss.bookmarksfly.cn

[T11] Kotlin：协程
来源：http://vd.newstarts.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nl.nszjky.cn

[T12] Kotlin：解构声明
来源：http://ck.bjjhwx.cn

val (a, b) = Pair(1, 2)
来源：http://ew.nszjky.cn

[T13] Kotlin：只读 Map
来源：http://cb.chemitech.net.cn

val m = mapOf("a" to 1)
来源：http://tv.panjiajie.cn

[T14] Kotlin：循环
来源：http://bb.szsharing.cn

for (i in 1..10) println(i)
来源：http://ob.newstarts.cn

[T15] Kotlin：接口
来源：http://se.jianghongdianzi.cn

interface Shape { fun area(): Double }
来源：http://jl.szxytkj.cn

[T16] Swift：Hello World
来源：http://wo.jianghongdianzi.cn

print("Hello")
来源：http://ly.colortex.cn

[T17] Swift：变量与常量
来源：http://oa.asd995.cn

var a = 1;  let b = 2
来源：http://sr.bjjhwx.cn

[T18] Swift：字符串插值
来源：http://rp.huanxung.cn

"值: \(b)"
来源：http://xn.hahajie.cn

[T19] Swift：可选绑定
来源：http://rt.asd995.cn

if let n = opt { print(n) }
来源：http://fe.nszjky.cn

[T20] Swift：数组操作
来源：http://de.szxytkj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://rh.newstarts.cn

[T21] Swift：遍历
来源：http://xh.521024.cn

for x in a { print(x) }
来源：http://pn.nicolike.cn

[T22] Swift：字典
来源：http://iv.muxihuayi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://pc.521024.cn

[T23] Swift：函数
来源：http://ms.nszjky.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zz.jctech888.com.cn

[T24] Swift：闭包
来源：http://he.huixinmuqiang.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ji.521024.cn

[T25] Swift：结构体
来源：http://fd.521024.cn

struct P { var x: Int }
来源：http://gt.huanxung.cn

[T26] Swift：类与重写
来源：http://to.szxytkj.cn

class A: Base { override func f() {} }
来源：http://fc.yuntaijiaju.cn

[T27] Swift：错误处理
来源：http://tb.shtwfgs.cn

do { try f() } catch { print(error) }
来源：http://td.panjiajie.cn

[T28] Swift：枚举
来源：http://sk.bookmarksfly.cn

enum Color { case red, green }
来源：http://ac.chemitech.net.cn

[T29] Swift：guard 提前返回
来源：http://jh.yuexingan06.cn

guard let x = opt else { return }
来源：http://fb.9csxet.cn

[T30] Swift：协议
来源：http://xw.chemitech.net.cn

protocol Shape { func area() -> Double }
来源：http://jt.newstarts.cn

[T31] Lua：Hello World
来源：http://ho.huixiangedu.cn

print("Hello")
来源：http://yp.bjjhwx.cn

[T32] Lua：局部变量
来源：http://rf.muxihuayi.cn

local a = 1
来源：http://wl.hnjuh.cn

[T33] Lua：表（数组）
来源：http://iw.muxihuayi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://au.jianghongdianzi.cn

[T34] Lua：遍历表
来源：http://da.asd995.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zk.huixiangedu.cn

[T35] Lua：字典表
来源：http://pi.gzmigu.cn

local d = { a = 1 };  d.b = 2
来源：http://zf.bookmarksfly.cn

[T36] Lua：函数
来源：http://nd.huixiangedu.cn

function add(a, b) return a + b end
来源：http://lg.shxzskj.cn

[T37] Lua：字符串拼接
来源：http://wz.bjjhwx.cn

"a" .. "b"
来源：http://vl.szxytkj.cn

[T38] Lua：条件
来源：http://rw.bookmarksfly.cn

if x > 0 then print("正") end
来源：http://md.hnjuh.cn

[T39] Lua：模式匹配
来源：http://nq.szsharing.cn

string.find(s, "%d+")
来源：http://gd.nszjky.cn

[T40] Lua：元表
来源：http://qy.shxzskj.cn

setmetatable({}, { __index = base })
来源：http://sm.newstarts.cn

[T41] Perl：Hello World
来源：http://rc.hahajie.cn

print "Hello\n";
来源：http://bk.jctech888.com.cn

[T42] Perl：变量类型
来源：http://tk.szsharing.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yr.chemitech.net.cn

[T43] Perl：字符串插值
来源：http://ay.shtwfgs.cn

"值: $a"
来源：http://ds.nszjky.cn

[T44] Perl：条件
来源：http://ee.asd995.cn

if ($a > 0) { print "正"; }
来源：http://sm.haigaiapp.cn

[T45] Perl：数组遍历
来源：http://dv.newstarts.cn

for my $x (@arr) { print $x; }
来源：http://uw.bookmarksfly.cn

[T46] Perl：哈希操作
来源：http://cl.colortex.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xz.szsharing.cn

[T47] Perl：正则捕获
来源：http://rm.bjjhwx.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vu.bjjhwx.cn

[T48] Perl：正则替换
来源：http://ez.bjjhwx.cn

$s =~ s/old/new/g;
来源：http://ds.521024.cn

[T49] Perl：函数
来源：http://dx.9csxet.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qv.hahajie.cn

[T50] Perl：逐行读文件
来源：http://ad.gzmigu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://uy.nszjky.cn

while (my $line = <$fh>) { print $line; }
来源：http://xn.colortex.cn

[T51] Scala：Hello World
来源：http://jn.521024.cn

println("Hello")
来源：http://kh.bookmarksfly.cn

[T52] Scala：变量
来源：http://fv.colortex.cn

val a = 1;  var b = 2
来源：http://jb.nszjky.cn

[T53] Scala：字符串插值
来源：http://ii.szsharing.cn

s"值: $b"
来源：http://ji.newstarts.cn

[T54] Scala：集合映射
来源：http://hs.521024.cn

List(1, 2, 3).map(_ * 2)
来源：http://cf.huixiangedu.cn

[T55] Scala：集合过滤
来源：http://dk.hnjuh.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wn.colortex.cn

[T56] Scala：样例类
来源：http://gq.jianghongdianzi.cn

case class User(name: String, age: Int)
来源：http://yj.bjjhwx.cn

[T57] Scala：模式匹配
来源：http://fy.gzmigu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wb.lnxyls.cn

[T58] Scala：函数定义
来源：http://sb.nicolike.cn

def add(a: Int, b: Int): Int = a + b
来源：http://mf.hnjuh.cn

[T59] Scala：循环
来源：http://vq.chemitech.net.cn

for (i <- 1 to 10) println(i)
来源：http://pj.nszjky.cn

[T60] Scala：折叠
来源：http://cm.521024.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ut.bookmarksfly.cn

================================================================================
来源：http://kw.szxytkj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jj.chemitech.net.cn

================================================================================
来源：http://tw.gzmigu.cn

[U01] Py：创建虚拟环境
来源：http://kw.colortex.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bs.9csxet.cn

[U02] Py：导出 / 安装依赖
来源：http://zl.huanxung.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://aa.9csxet.cn

[U03] Py：加载 .env 配置
来源：http://le.szsharing.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://bk.asd995.cn

[U04] Py：变量调试打印
来源：http://as.hnjuh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mb.shxzskj.cn

[U05] Py：列表去重且保序
来源：http://zw.panjiajie.cn

list(dict.fromkeys(arr))
来源：http://eg.9csxet.cn

[U06] Py：合并两个字典
来源：http://af.shxzskj.cn

{**a, **b}
来源：http://hg.yuexingan06.cn

[U07] Py：反转字典键值
来源：http://vo.jianghongdianzi.cn

{v: k for k, v in d.items()}
来源：http://cy.hahajie.cn

[U08] Py：展平二维列表
来源：http://bc.wgjwhj.cn

[y for x in nested for y in x]
来源：http://by.huixiangedu.cn

[U09] Py：字典取最大值的键
来源：http://ct.jctech888.com.cn

max(d, key=d.get)
来源：http://nr.jianghongdianzi.cn

[U10] Py：按值排序字典
来源：http://vl.szxytkj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dh.yuexingan06.cn

[U11] Py：生成器表达式
来源：http://ei.hnjuh.cn

(x * 2 for x in arr)
来源：http://pk.haigaiapp.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ym.521024.cn

Counter(arr).most_common(3)
来源：http://db.bjjhwx.cn

[U13] Py：固定长度队列
来源：http://ru.newstarts.cn

deque(maxlen=10)
来源：http://yp.huanxung.cn

[U14] Py：分组收集到列表
来源：http://jh.asd995.cn

defaultdict(list)
来源：http://eo.huixinmuqiang.cn

[U15] Py：高精度计时
来源：http://ej.9csxet.cn

t = time.perf_counter()
来源：http://du.lnxyls.cn

[U16] Py：命令行参数解析
来源：http://ph.huixiangedu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cu.bookmarksfly.cn

[U17] Py：初始化日志
来源：http://cn.asd995.cn

logging.basicConfig(level=logging.INFO)
来源：http://id.huanxung.cn

[U18] Py：预编译正则
来源：http://mg.nszjky.cn

pat = re.compile(r"\d+")
来源：http://wo.jianghongdianzi.cn

[U19] Py：正则替换带回调
来源：http://vq.huixinmuqiang.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yw.nicolike.cn

[U20] Py：缓存函数结果
来源：http://co.huanxung.cn

@functools.lru_cache(maxsize=None)
来源：http://wm.hnjuh.cn

[U21] Py：自定义上下文管理器
来源：http://rr.yuexingan06.cn

@contextlib.contextmanager
来源：http://zj.asd995.cn

[U22] Py：矩阵转置
来源：http://hg.yuntaijiaju.cn

list(zip(*m))
来源：http://xi.jianghongdianzi.cn

[U23] Py：分块读取大文件
来源：http://lu.haigaiapp.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bd.haigaiapp.cn

[U24] Py：路径操作
来源：http://hc.bookmarksfly.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://an.jctech888.com.cn

[U25] Py：CSV 按字典读
来源：http://ek.9csxet.cn

csv.DictReader(f)
来源：http://tx.jctech888.com.cn

[U26] Py：并发下载
来源：http://mj.panjiajie.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ww.colortex.cn

[U27] Py：异步 HTTP
来源：http://ej.shxzukj.cn

aiohttp.ClientSession() 配合 async with
来源：http://xh.panjiajie.cn

[U28] Py：类型别名
来源：http://yf.szsharing.cn

UserId = int
来源：http://vo.szsharing.cn

[U29] Py：属性校验
来源：http://am.newstarts.cn

@property 与 @x.setter 配合
来源：http://nm.nicolike.cn

[U30] Py：数据类
来源：http://xf.huixinmuqiang.cn

@dataclass(slots=True)
来源：http://ok.jctech888.com.cn

[U31] Py：单测
来源：http://vz.nicolike.cn

python -m pytest -q
来源：http://lw.nszjky.cn

[U32] Py：代码格式化
来源：http://aw.wgjwhj.cn

ruff format . && ruff check --fix .
来源：http://ic.huanxung.cn

[U33] Py：打包发布
来源：http://ui.lnxyls.cn

python -m build  （依赖 pyproject.toml）
来源：http://ci.521024.cn

[U34] Py：判断编码
来源：http://rl.wgjwhj.cn

chardet.detect(raw)
来源：http://oe.hnjuh.cn

[U35] Py：发送邮件
来源：http://ax.chemitech.net.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gz.gzmigu.cn

[U36] Py：定时任务
来源：http://sz.nszjky.cn

schedule.every(10).minutes.do(job)
来源：http://vr.hnjuh.cn

[U37] Py：读写 Excel
来源：http://zk.shxzskj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://hm.shtwfgs.cn

[U38] Py：获取脚本所在目录
来源：http://fx.lnxyls.cn

Path(__file__).resolve().parent
来源：http://zn.bjjhwx.cn

[U39] Py：判断是否在交互环境
来源：http://zt.huanxung.cn

sys.stdout.isatty()
来源：http://wa.szxytkj.cn

[U40] Py：打印到标准错误
来源：http://fh.szxytkj.cn

print("err", file=sys.stderr)
来源：http://ec.huixinmuqiang.cn

[U41] PHP：初始化 Composer 项目
来源：http://gc.shtwfgs.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://tc.nszjky.cn

[U42] PHP：PSR-4 自动加载
来源：http://go.huixiangedu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fb.shxzukj.cn

[U43] PHP：声明命名空间
来源：http://aj.hnjuh.cn

namespace App\Http;
来源：http://ca.huixinmuqiang.cn

[U44] PHP：开启严格类型
来源：http://dv.yuexingan06.cn

declare(strict_types=1);
来源：http://sj.hnjuh.cn

[U45] PHP：类型声明与返回类型
来源：http://ey.szxytkj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bh.yuntaijiaju.cn

[U46] PHP：可空类型
来源：http://au.lnxyls.cn

?string $name = null
来源：http://fm.huixiangedu.cn

[U47] PHP：联合类型
来源：http://jf.colortex.cn

int|string $id
来源：http://nm.hnjuh.cn

[U48] PHP：纯枚举
来源：http://cd.chemitech.net.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ua.521024.cn

[U49] PHP：只读属性
来源：http://jl.newstarts.cn

public readonly string $name
来源：http://bf.wgjwhj.cn

[U50] PHP：构造器属性提升
来源：http://ev.szsharing.cn

public function __construct(private int $id) {}
来源：http://sg.huixiangedu.cn

[U51] PHP：数组解构
来源：http://fi.jctech888.com.cn

[$a, $b] = $arr;
来源：http://vd.muxihuayi.cn

[U52] PHP：箭头函数
来源：http://vp.9csxet.cn

$double = fn($x) => $x * 2;
来源：http://es.wgjwhj.cn

[U53] PHP：空合并运算符
来源：http://rb.yuntaijiaju.cn

$v = $a ?? $b ?? "default";
来源：http://id.nicolike.cn

[U54] PHP：空安全调用
来源：http://gv.jianghongdianzi.cn

$obj?->method()
来源：http://yd.hnjuh.cn

[U55] PHP：match 表达式
来源：http://fu.jctech888.com.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://sq.colortex.cn

[U56] PHP：命名参数
来源：http://kd.muxihuayi.cn

f(a: 1, b: 2)
来源：http://ut.shxzukj.cn

[U57] PHP：字符串插值
来源：http://po.9csxet.cn

"值: {$a}"
来源：http://rs.bookmarksfly.cn

[U58] PHP：数组三件套
来源：http://yv.huixiangedu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bc.colortex.cn

[U59] PHP：自定义排序
来源：http://wc.newstarts.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cx.haigaiapp.cn

[U60] PHP：JSON 编解码
来源：http://ik.yuexingan06.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kc.shtwfgs.cn

[U61] PHP：正则
来源：http://ng.bookmarksfly.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sz.lnxyls.cn

[U62] PHP：日期对象
来源：http://wz.asd995.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dx.colortex.cn

[U63] PHP：文件读写
来源：http://ye.gzmigu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kx.jianghongdianzi.cn

[U64] PHP：目录遍历
来源：http://uh.panjiajie.cn

glob("dir/*.php");  scandir("dir");
来源：http://kg.nszjky.cn

[U65] PHP：会话
来源：http://sz.asd995.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://el.newstarts.cn

[U66] PHP：设置 Cookie
来源：http://ff.newstarts.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mp.shxzskj.cn

[U67] PHP：处理文件上传
来源：http://hv.521024.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ao.shxzskj.cn

[U68] PHP：PDO 连接
来源：http://mo.huanxung.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://el.yuntaijiaju.cn

[U69] PHP：PDO 预处理
来源：http://wk.wgjwhj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://az.wgjwhj.cn

[U70] PHP：PDO 事务
来源：http://vs.521024.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pa.hahajie.cn

[U71] PHP：抛出异常
来源：http://sm.colortex.cn

throw new RuntimeException("失败", 500);
来源：http://nf.huanxung.cn

[U72] PHP：写错误日志
来源：http://kw.szxytkj.cn

error_log("失败: " . $e->getMessage());
来源：http://aq.521024.cn

[U73] PHP：读取 ini 配置
来源：http://ae.colortex.cn

parse_ini_file("config.ini", true)
来源：http://fi.newstarts.cn

[U74] PHP：读取环境变量
来源：http://lo.szsharing.cn

getenv("APP_ENV") ?: "production"
来源：http://lt.bookmarksfly.cn

[U75] PHP：依赖注入
来源：http://xi.9csxet.cn

composer require psr/container
来源：http://qv.jianghongdianzi.cn

[U76] PHP：简单路由
来源：http://dq.nszjky.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ck.nszjky.cn

[U77] PHP：模板渲染
来源：http://qh.nicolike.cn

composer require twig/twig
来源：http://fh.jianghongdianzi.cn

[U78] PHP：单元测试
来源：http://gy.nszjky.cn

composer require --dev phpunit/phpunit
来源：http://jb.asd995.cn

[U79] PHP：静态分析
来源：http://rl.wgjwhj.cn

composer require --dev phpstan/phpstan
来源：http://mv.shxzukj.cn

[U80] PHP：代码规范修复
来源：http://dq.hnjuh.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://gw.gzmigu.cn

[U81] JS：初始化项目
来源：http://wl.shxzskj.cn

npm init -y;  npm i express
来源：http://zy.yuntaijiaju.cn

[U82] JS：package.json 脚本
来源：http://dk.huanxung.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://od.yuexingan06.cn

[U83] JS：ES Module 导入导出
来源：http://am.panjiajie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://nk.hnjuh.cn

[U84] JS：CommonJS 写法
来源：http://ny.newstarts.cn

module.exports = { a };  const { a } = require("./m");
来源：http://sj.nicolike.cn

[U85] JS：可选链
来源：http://dp.shxzskj.cn

a?.b?.c
来源：http://sg.nszjky.cn

[U86] JS：空值合并
来源：http://ss.colortex.cn

a ?? b
来源：http://jp.newstarts.cn

[U87] JS：解构默认值
来源：http://cx.newstarts.cn

const { a = 1, b = 2 } = obj;
来源：http://zf.lnxyls.cn

[U88] JS：对象展开合并
来源：http://jn.jctech888.com.cn

{ ...a, ...b }
来源：http://ea.nszjky.cn

[U89] JS：数组去重
来源：http://tg.lnxyls.cn

[...new Set(arr)]
来源：http://ff.bookmarksfly.cn

[U90] JS：数字数组排序
来源：http://jj.huanxung.cn

[...arr].sort((a, b) => a - b)
来源：http://go.521024.cn


<!-- 参考信息 -->