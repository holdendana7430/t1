代发 wailian999

[T03] Kotlin：字符串模板
来源：http://jh.bjjhwx.cn

"值: $b"
来源：http://zq.hahajie.cn

[T04] Kotlin：空安全
来源：http://ye.szsharing.cn

val n: String? = null;  n?.length
来源：http://pq.szxytkj.cn

[T05] Kotlin：when 表达式
来源：http://qu.huixiangedu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nc.hnjuh.cn

[T06] Kotlin：集合映射
来源：http://mj.shtwfgs.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://mw.jctech888.com.cn

[T07] Kotlin：集合过滤
来源：http://hr.nicolike.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wn.521024.cn

[T08] Kotlin：数据类
来源：http://eu.panjiajie.cn

data class User(val name: String, val age: Int)
来源：http://ic.chemitech.net.cn

[T09] Kotlin：扩展函数
来源：http://zf.nszjky.cn

fun String.exclaim() = this + "!"
来源：http://ui.nicolike.cn

[T10] Kotlin：默认参数
来源：http://ys.lnxyls.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://cw.gzmigu.cn

[T11] Kotlin：协程
来源：http://gu.gzmigu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://cr.9csxet.cn

[T12] Kotlin：解构声明
来源：http://sm.nicolike.cn

val (a, b) = Pair(1, 2)
来源：http://ie.lnxyls.cn

[T13] Kotlin：只读 Map
来源：http://kq.nszjky.cn

val m = mapOf("a" to 1)
来源：http://hd.bookmarksfly.cn

[T14] Kotlin：循环
来源：http://up.nszjky.cn

for (i in 1..10) println(i)
来源：http://qz.hahajie.cn

[T15] Kotlin：接口
来源：http://ml.colortex.cn

interface Shape { fun area(): Double }
来源：http://yv.chemitech.net.cn

[T16] Swift：Hello World
来源：http://uo.colortex.cn

print("Hello")
来源：http://ae.bookmarksfly.cn

[T17] Swift：变量与常量
来源：http://bv.colortex.cn

var a = 1;  let b = 2
来源：http://vv.shxzskj.cn

[T18] Swift：字符串插值
来源：http://mw.shxzukj.cn

"值: \(b)"
来源：http://aw.shxzskj.cn

[T19] Swift：可选绑定
来源：http://ri.huanxung.cn

if let n = opt { print(n) }
来源：http://ds.panjiajie.cn

[T20] Swift：数组操作
来源：http://ji.yuntaijiaju.cn

var a = [1, 2, 3];  a.append(4)
来源：http://bp.shxzskj.cn

[T21] Swift：遍历
来源：http://yt.huixiangedu.cn

for x in a { print(x) }
来源：http://oa.huixinmuqiang.cn

[T22] Swift：字典
来源：http://qu.huanxung.cn

var d = ["a": 1];  d["b"] = 2
来源：http://gh.chemitech.net.cn

[T23] Swift：函数
来源：http://bc.chemitech.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qi.nicolike.cn

[T24] Swift：闭包
来源：http://ht.9csxet.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://fg.nszjky.cn

[T25] Swift：结构体
来源：http://of.shtwfgs.cn

struct P { var x: Int }
来源：http://ig.szxytkj.cn

[T26] Swift：类与重写
来源：http://uh.bookmarksfly.cn

class A: Base { override func f() {} }
来源：http://wj.szsharing.cn

[T27] Swift：错误处理
来源：http://ih.huanxung.cn

do { try f() } catch { print(error) }
来源：http://lk.jianghongdianzi.cn

[T28] Swift：枚举
来源：http://px.szsharing.cn

enum Color { case red, green }
来源：http://yp.yuntaijiaju.cn

[T29] Swift：guard 提前返回
来源：http://jj.huixinmuqiang.cn

guard let x = opt else { return }
来源：http://vs.shxzskj.cn

[T30] Swift：协议
来源：http://kz.nicolike.cn

protocol Shape { func area() -> Double }
来源：http://rg.shtwfgs.cn

[T31] Lua：Hello World
来源：http://yv.jianghongdianzi.cn

print("Hello")
来源：http://sz.521024.cn

[T32] Lua：局部变量
来源：http://yk.huixinmuqiang.cn

local a = 1
来源：http://nd.lnxyls.cn

[T33] Lua：表（数组）
来源：http://nd.yuexingan06.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://dt.9csxet.cn

[T34] Lua：遍历表
来源：http://ht.nicolike.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ts.huixinmuqiang.cn

[T35] Lua：字典表
来源：http://hk.yuntaijiaju.cn

local d = { a = 1 };  d.b = 2
来源：http://fz.nszjky.cn

[T36] Lua：函数
来源：http://mz.newstarts.cn

function add(a, b) return a + b end
来源：http://cp.panjiajie.cn

[T37] Lua：字符串拼接
来源：http://gg.shxzskj.cn

"a" .. "b"
来源：http://vf.newstarts.cn

[T38] Lua：条件
来源：http://yy.panjiajie.cn

if x > 0 then print("正") end
来源：http://iz.haigaiapp.cn

[T39] Lua：模式匹配
来源：http://bz.yuexingan06.cn

string.find(s, "%d+")
来源：http://ue.huixiangedu.cn

[T40] Lua：元表
来源：http://te.huanxung.cn

setmetatable({}, { __index = base })
来源：http://bz.gzmigu.cn

[T41] Perl：Hello World
来源：http://ep.bjjhwx.cn

print "Hello\n";
来源：http://pa.bookmarksfly.cn

[T42] Perl：变量类型
来源：http://zp.yuntaijiaju.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bi.yuexingan06.cn

[T43] Perl：字符串插值
来源：http://wh.bjjhwx.cn

"值: $a"
来源：http://le.nicolike.cn

[T44] Perl：条件
来源：http://nx.wgjwhj.cn

if ($a > 0) { print "正"; }
来源：http://ie.bookmarksfly.cn

[T45] Perl：数组遍历
来源：http://bz.shxzskj.cn

for my $x (@arr) { print $x; }
来源：http://sn.szxytkj.cn

[T46] Perl：哈希操作
来源：http://zt.haigaiapp.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pw.hnjuh.cn

[T47] Perl：正则捕获
来源：http://aq.newstarts.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xq.yuexingan06.cn

[T48] Perl：正则替换
来源：http://ne.jianghongdianzi.cn

$s =~ s/old/new/g;
来源：http://hx.nicolike.cn

[T49] Perl：函数
来源：http://eq.bookmarksfly.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sp.jianghongdianzi.cn

[T50] Perl：逐行读文件
来源：http://yj.nszjky.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ab.521024.cn

while (my $line = <$fh>) { print $line; }
来源：http://rp.shxzukj.cn

[T51] Scala：Hello World
来源：http://wy.haigaiapp.cn

println("Hello")
来源：http://yp.bjjhwx.cn

[T52] Scala：变量
来源：http://ik.newstarts.cn

val a = 1;  var b = 2
来源：http://sc.gzmigu.cn

[T53] Scala：字符串插值
来源：http://yh.asd995.cn

s"值: $b"
来源：http://tw.szsharing.cn

[T54] Scala：集合映射
来源：http://am.huanxung.cn

List(1, 2, 3).map(_ * 2)
来源：http://hs.shtwfgs.cn

[T55] Scala：集合过滤
来源：http://yd.nszjky.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ta.shtwfgs.cn

[T56] Scala：样例类
来源：http://it.chemitech.net.cn

case class User(name: String, age: Int)
来源：http://uz.yuexingan06.cn

[T57] Scala：模式匹配
来源：http://jx.huixinmuqiang.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://zu.wgjwhj.cn

[T58] Scala：函数定义
来源：http://tz.gzmigu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://dn.colortex.cn

[T59] Scala：循环
来源：http://ak.yuntaijiaju.cn

for (i <- 1 to 10) println(i)
来源：http://uy.yuntaijiaju.cn

[T60] Scala：折叠
来源：http://qe.panjiajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qy.shtwfgs.cn

================================================================================
来源：http://zt.newstarts.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bd.lnxyls.cn

================================================================================
来源：http://uw.lnxyls.cn

[U01] Py：创建虚拟环境
来源：http://oy.huixiangedu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ai.shxzukj.cn

[U02] Py：导出 / 安装依赖
来源：http://ar.nicolike.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://re.szxytkj.cn

[U03] Py：加载 .env 配置
来源：http://wr.gzmigu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ir.shtwfgs.cn

[U04] Py：变量调试打印
来源：http://pg.521024.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vd.yuexingan06.cn

[U05] Py：列表去重且保序
来源：http://ul.nszjky.cn

list(dict.fromkeys(arr))
来源：http://yu.haigaiapp.cn

[U06] Py：合并两个字典
来源：http://vp.colortex.cn

{**a, **b}
来源：http://wo.nszjky.cn

[U07] Py：反转字典键值
来源：http://dz.huixiangedu.cn

{v: k for k, v in d.items()}
来源：http://qc.newstarts.cn

[U08] Py：展平二维列表
来源：http://sw.jctech888.com.cn

[y for x in nested for y in x]
来源：http://vi.yuexingan06.cn

[U09] Py：字典取最大值的键
来源：http://bv.jctech888.com.cn

max(d, key=d.get)
来源：http://bu.lnxyls.cn

[U10] Py：按值排序字典
来源：http://dw.shxzskj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xu.shxzskj.cn

[U11] Py：生成器表达式
来源：http://ep.yuntaijiaju.cn

(x * 2 for x in arr)
来源：http://nl.hnjuh.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zp.haigaiapp.cn

Counter(arr).most_common(3)
来源：http://hn.lnxyls.cn

[U13] Py：固定长度队列
来源：http://fm.yuexingan06.cn

deque(maxlen=10)
来源：http://yc.bjjhwx.cn

[U14] Py：分组收集到列表
来源：http://fb.yuexingan06.cn

defaultdict(list)
来源：http://sx.yuntaijiaju.cn

[U15] Py：高精度计时
来源：http://bu.chemitech.net.cn

t = time.perf_counter()
来源：http://ne.huanxung.cn

[U16] Py：命令行参数解析
来源：http://ph.521024.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fg.521024.cn

[U17] Py：初始化日志
来源：http://oo.newstarts.cn

logging.basicConfig(level=logging.INFO)
来源：http://bd.chemitech.net.cn

[U18] Py：预编译正则
来源：http://fd.colortex.cn

pat = re.compile(r"\d+")
来源：http://kb.yuntaijiaju.cn

[U19] Py：正则替换带回调
来源：http://gx.yuntaijiaju.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ix.shxzskj.cn

[U20] Py：缓存函数结果
来源：http://wm.huanxung.cn

@functools.lru_cache(maxsize=None)
来源：http://dg.hnjuh.cn

[U21] Py：自定义上下文管理器
来源：http://ne.newstarts.cn

@contextlib.contextmanager
来源：http://gc.hahajie.cn

[U22] Py：矩阵转置
来源：http://tk.jianghongdianzi.cn

list(zip(*m))
来源：http://fj.jctech888.com.cn

[U23] Py：分块读取大文件
来源：http://fl.huanxung.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mv.hahajie.cn

[U24] Py：路径操作
来源：http://pi.huixinmuqiang.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xz.yuexingan06.cn

[U25] Py：CSV 按字典读
来源：http://wc.shtwfgs.cn

csv.DictReader(f)
来源：http://pk.chemitech.net.cn

[U26] Py：并发下载
来源：http://zd.huixinmuqiang.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://to.haigaiapp.cn

[U27] Py：异步 HTTP
来源：http://xe.bjjhwx.cn

aiohttp.ClientSession() 配合 async with
来源：http://xl.colortex.cn

[U28] Py：类型别名
来源：http://jq.nszjky.cn

UserId = int
来源：http://di.gzmigu.cn

[U29] Py：属性校验
来源：http://iu.jctech888.com.cn

@property 与 @x.setter 配合
来源：http://dz.newstarts.cn

[U30] Py：数据类
来源：http://lr.jianghongdianzi.cn

@dataclass(slots=True)
来源：http://xn.nicolike.cn

[U31] Py：单测
来源：http://qf.asd995.cn

python -m pytest -q
来源：http://uo.huixiangedu.cn

[U32] Py：代码格式化
来源：http://ch.szsharing.cn

ruff format . && ruff check --fix .
来源：http://tm.yuexingan06.cn

[U33] Py：打包发布
来源：http://sa.yuntaijiaju.cn

python -m build  （依赖 pyproject.toml）
来源：http://ui.hahajie.cn

[U34] Py：判断编码
来源：http://cz.huanxung.cn

chardet.detect(raw)
来源：http://tb.9csxet.cn

[U35] Py：发送邮件
来源：http://es.yuntaijiaju.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zj.gzmigu.cn

[U36] Py：定时任务
来源：http://gj.asd995.cn

schedule.every(10).minutes.do(job)
来源：http://jf.huixinmuqiang.cn

[U37] Py：读写 Excel
来源：http://ah.huixinmuqiang.cn

pandas.read_excel / DataFrame.to_excel
来源：http://px.shtwfgs.cn

[U38] Py：获取脚本所在目录
来源：http://js.chemitech.net.cn

Path(__file__).resolve().parent
来源：http://yg.9csxet.cn

[U39] Py：判断是否在交互环境
来源：http://qu.shtwfgs.cn

sys.stdout.isatty()
来源：http://lt.jianghongdianzi.cn

[U40] Py：打印到标准错误
来源：http://mu.9csxet.cn

print("err", file=sys.stderr)
来源：http://zc.yuntaijiaju.cn

[U41] PHP：初始化 Composer 项目
来源：http://br.bjjhwx.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://tj.bjjhwx.cn

[U42] PHP：PSR-4 自动加载
来源：http://ay.szsharing.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://so.hnjuh.cn

[U43] PHP：声明命名空间
来源：http://xq.bjjhwx.cn

namespace App\Http;
来源：http://xs.huixinmuqiang.cn

[U44] PHP：开启严格类型
来源：http://wb.huixiangedu.cn

declare(strict_types=1);
来源：http://qn.haigaiapp.cn

[U45] PHP：类型声明与返回类型
来源：http://ms.szsharing.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://xw.shtwfgs.cn

[U46] PHP：可空类型
来源：http://eg.lnxyls.cn

?string $name = null
来源：http://jx.newstarts.cn

[U47] PHP：联合类型
来源：http://lh.9csxet.cn

int|string $id
来源：http://yb.yuntaijiaju.cn

[U48] PHP：纯枚举
来源：http://sq.colortex.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ph.shtwfgs.cn

[U49] PHP：只读属性
来源：http://nf.nszjky.cn

public readonly string $name
来源：http://wb.hnjuh.cn

[U50] PHP：构造器属性提升
来源：http://zu.panjiajie.cn

public function __construct(private int $id) {}
来源：http://zd.szxytkj.cn

[U51] PHP：数组解构
来源：http://yi.wgjwhj.cn

[$a, $b] = $arr;
来源：http://xx.wgjwhj.cn

[U52] PHP：箭头函数
来源：http://nw.bookmarksfly.cn

$double = fn($x) => $x * 2;
来源：http://cz.huixinmuqiang.cn

[U53] PHP：空合并运算符
来源：http://de.szsharing.cn

$v = $a ?? $b ?? "default";
来源：http://ug.chemitech.net.cn

[U54] PHP：空安全调用
来源：http://vo.huixinmuqiang.cn

$obj?->method()
来源：http://ip.yuntaijiaju.cn

[U55] PHP：match 表达式
来源：http://ir.lnxyls.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lm.muxihuayi.cn

[U56] PHP：命名参数
来源：http://ag.chemitech.net.cn

f(a: 1, b: 2)
来源：http://hz.shxzskj.cn

[U57] PHP：字符串插值
来源：http://jj.newstarts.cn

"值: {$a}"
来源：http://jm.yuntaijiaju.cn

[U58] PHP：数组三件套
来源：http://di.hahajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ej.szxytkj.cn

[U59] PHP：自定义排序
来源：http://td.shtwfgs.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sj.huanxung.cn

[U60] PHP：JSON 编解码
来源：http://ki.hnjuh.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ju.jctech888.com.cn

[U61] PHP：正则
来源：http://wa.newstarts.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://by.shxzskj.cn

[U62] PHP：日期对象
来源：http://rh.nszjky.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qa.shxzskj.cn

[U63] PHP：文件读写
来源：http://tv.huixiangedu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://is.colortex.cn

[U64] PHP：目录遍历
来源：http://fd.asd995.cn

glob("dir/*.php");  scandir("dir");
来源：http://in.shxzskj.cn

[U65] PHP：会话
来源：http://ua.nicolike.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://el.muxihuayi.cn

[U66] PHP：设置 Cookie
来源：http://rr.jctech888.com.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ad.colortex.cn

[U67] PHP：处理文件上传
来源：http://nz.yuntaijiaju.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://iz.hahajie.cn

[U68] PHP：PDO 连接
来源：http://uj.wgjwhj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fp.9csxet.cn

[U69] PHP：PDO 预处理
来源：http://as.huixiangedu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tw.wgjwhj.cn

[U70] PHP：PDO 事务
来源：http://xs.newstarts.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xv.yuntaijiaju.cn

[U71] PHP：抛出异常
来源：http://ev.shxzukj.cn

throw new RuntimeException("失败", 500);
来源：http://mj.jianghongdianzi.cn

[U72] PHP：写错误日志
来源：http://wt.hnjuh.cn

error_log("失败: " . $e->getMessage());
来源：http://fk.lnxyls.cn

[U73] PHP：读取 ini 配置
来源：http://ky.wgjwhj.cn

parse_ini_file("config.ini", true)
来源：http://ng.szxytkj.cn

[U74] PHP：读取环境变量
来源：http://dx.colortex.cn

getenv("APP_ENV") ?: "production"
来源：http://sw.haigaiapp.cn

[U75] PHP：依赖注入
来源：http://cq.huixinmuqiang.cn

composer require psr/container
来源：http://mb.panjiajie.cn

[U76] PHP：简单路由
来源：http://lh.panjiajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pw.9csxet.cn

[U77] PHP：模板渲染
来源：http://ow.haigaiapp.cn

composer require twig/twig
来源：http://ud.521024.cn

[U78] PHP：单元测试
来源：http://cs.colortex.cn

composer require --dev phpunit/phpunit
来源：http://fh.hnjuh.cn

[U79] PHP：静态分析
来源：http://fi.colortex.cn

composer require --dev phpstan/phpstan
来源：http://vg.jctech888.com.cn

[U80] PHP：代码规范修复
来源：http://ut.shtwfgs.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://bq.hnjuh.cn

[U81] JS：初始化项目
来源：http://zr.huixinmuqiang.cn

npm init -y;  npm i express
来源：http://ng.hahajie.cn

[U82] JS：package.json 脚本
来源：http://wy.szxytkj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pj.hahajie.cn

[U83] JS：ES Module 导入导出
来源：http://tm.asd995.cn

export const a = 1;  import { a } from "./m.js";
来源：http://im.9csxet.cn

[U84] JS：CommonJS 写法
来源：http://aq.haigaiapp.cn

module.exports = { a };  const { a } = require("./m");
来源：http://js.haigaiapp.cn

[U85] JS：可选链
来源：http://fw.chemitech.net.cn

a?.b?.c
来源：http://vl.shxzskj.cn

[U86] JS：空值合并
来源：http://mg.shxzskj.cn

a ?? b
来源：http://xh.shxzukj.cn

[U87] JS：解构默认值
来源：http://tn.yuexingan06.cn

const { a = 1, b = 2 } = obj;
来源：http://vc.yuntaijiaju.cn

[U88] JS：对象展开合并
来源：http://cv.hnjuh.cn

{ ...a, ...b }
来源：http://sz.jctech888.com.cn

[U89] JS：数组去重
来源：http://mp.bjjhwx.cn

[...new Set(arr)]
来源：http://nd.yuntaijiaju.cn

[U90] JS：数字数组排序
来源：http://gx.bjjhwx.cn

[...arr].sort((a, b) => a - b)
来源：http://hz.huanxung.cn


<!-- 参考信息 -->