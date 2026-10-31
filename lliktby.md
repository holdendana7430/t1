代发 wailian999

[T05] Kotlin：when 表达式
来源：http://sl.huixinmuqiang.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://is.szsharing.cn

[T06] Kotlin：集合映射
来源：http://xb.yuntaijiaju.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hs.huixiangedu.cn

[T07] Kotlin：集合过滤
来源：http://oq.lnxyls.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ed.yuntaijiaju.cn

[T08] Kotlin：数据类
来源：http://cp.yuexingan06.cn

data class User(val name: String, val age: Int)
来源：http://bk.521024.cn

[T09] Kotlin：扩展函数
来源：http://ux.gzmigu.cn

fun String.exclaim() = this + "!"
来源：http://lw.bjjhwx.cn

[T10] Kotlin：默认参数
来源：http://lt.gzmigu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://uq.wgjwhj.cn

[T11] Kotlin：协程
来源：http://mb.yuntaijiaju.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bj.huixiangedu.cn

[T12] Kotlin：解构声明
来源：http://og.9csxet.cn

val (a, b) = Pair(1, 2)
来源：http://om.chemitech.net.cn

[T13] Kotlin：只读 Map
来源：http://lx.lnxyls.cn

val m = mapOf("a" to 1)
来源：http://qb.bjjhwx.cn

[T14] Kotlin：循环
来源：http://hb.muxihuayi.cn

for (i in 1..10) println(i)
来源：http://pe.jctech888.com.cn

[T15] Kotlin：接口
来源：http://ix.jctech888.com.cn

interface Shape { fun area(): Double }
来源：http://kc.huixinmuqiang.cn

[T16] Swift：Hello World
来源：http://gf.jctech888.com.cn

print("Hello")
来源：http://mu.9csxet.cn

[T17] Swift：变量与常量
来源：http://ji.shxzskj.cn

var a = 1;  let b = 2
来源：http://yn.hnjuh.cn

[T18] Swift：字符串插值
来源：http://ay.gzmigu.cn

"值: \(b)"
来源：http://ai.newstarts.cn

[T19] Swift：可选绑定
来源：http://hj.9csxet.cn

if let n = opt { print(n) }
来源：http://wc.huixiangedu.cn

[T20] Swift：数组操作
来源：http://kk.colortex.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mw.yuntaijiaju.cn

[T21] Swift：遍历
来源：http://kb.shtwfgs.cn

for x in a { print(x) }
来源：http://og.nicolike.cn

[T22] Swift：字典
来源：http://jt.panjiajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://sw.nicolike.cn

[T23] Swift：函数
来源：http://ej.yuntaijiaju.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zk.nszjky.cn

[T24] Swift：闭包
来源：http://cf.gzmigu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ye.wgjwhj.cn

[T25] Swift：结构体
来源：http://ky.jctech888.com.cn

struct P { var x: Int }
来源：http://pn.szxytkj.cn

[T26] Swift：类与重写
来源：http://cd.panjiajie.cn

class A: Base { override func f() {} }
来源：http://mm.haigaiapp.cn

[T27] Swift：错误处理
来源：http://gv.hnjuh.cn

do { try f() } catch { print(error) }
来源：http://jr.nszjky.cn

[T28] Swift：枚举
来源：http://dh.bookmarksfly.cn

enum Color { case red, green }
来源：http://gl.9csxet.cn

[T29] Swift：guard 提前返回
来源：http://ju.shxzukj.cn

guard let x = opt else { return }
来源：http://qs.szsharing.cn

[T30] Swift：协议
来源：http://my.asd995.cn

protocol Shape { func area() -> Double }
来源：http://kd.haigaiapp.cn

[T31] Lua：Hello World
来源：http://me.szxytkj.cn

print("Hello")
来源：http://gs.lnxyls.cn

[T32] Lua：局部变量
来源：http://ff.asd995.cn

local a = 1
来源：http://xo.huixiangedu.cn

[T33] Lua：表（数组）
来源：http://ra.shtwfgs.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://cy.newstarts.cn

[T34] Lua：遍历表
来源：http://af.hahajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://wo.gzmigu.cn

[T35] Lua：字典表
来源：http://os.colortex.cn

local d = { a = 1 };  d.b = 2
来源：http://yo.szsharing.cn

[T36] Lua：函数
来源：http://yi.yuexingan06.cn

function add(a, b) return a + b end
来源：http://bu.bjjhwx.cn

[T37] Lua：字符串拼接
来源：http://ed.yuexingan06.cn

"a" .. "b"
来源：http://rb.hahajie.cn

[T38] Lua：条件
来源：http://mv.shxzukj.cn

if x > 0 then print("正") end
来源：http://kx.shxzskj.cn

[T39] Lua：模式匹配
来源：http://uy.bjjhwx.cn

string.find(s, "%d+")
来源：http://ac.jctech888.com.cn

[T40] Lua：元表
来源：http://tg.huanxung.cn

setmetatable({}, { __index = base })
来源：http://ex.huixiangedu.cn

[T41] Perl：Hello World
来源：http://gi.nicolike.cn

print "Hello\n";
来源：http://is.newstarts.cn

[T42] Perl：变量类型
来源：http://js.muxihuayi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://eb.chemitech.net.cn

[T43] Perl：字符串插值
来源：http://mq.jctech888.com.cn

"值: $a"
来源：http://va.hahajie.cn

[T44] Perl：条件
来源：http://dh.colortex.cn

if ($a > 0) { print "正"; }
来源：http://do.colortex.cn

[T45] Perl：数组遍历
来源：http://ld.shxzukj.cn

for my $x (@arr) { print $x; }
来源：http://us.huixinmuqiang.cn

[T46] Perl：哈希操作
来源：http://xz.panjiajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hf.jctech888.com.cn

[T47] Perl：正则捕获
来源：http://wd.hahajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://sc.chemitech.net.cn

[T48] Perl：正则替换
来源：http://el.huixinmuqiang.cn

$s =~ s/old/new/g;
来源：http://mn.hnjuh.cn

[T49] Perl：函数
来源：http://px.huanxung.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://it.huixinmuqiang.cn

[T50] Perl：逐行读文件
来源：http://lg.szxytkj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://vm.muxihuayi.cn

while (my $line = <$fh>) { print $line; }
来源：http://pq.yuntaijiaju.cn

[T51] Scala：Hello World
来源：http://ro.huixiangedu.cn

println("Hello")
来源：http://wx.nicolike.cn

[T52] Scala：变量
来源：http://tb.shxzskj.cn

val a = 1;  var b = 2
来源：http://tm.bjjhwx.cn

[T53] Scala：字符串插值
来源：http://cw.panjiajie.cn

s"值: $b"
来源：http://zq.yuntaijiaju.cn

[T54] Scala：集合映射
来源：http://hg.newstarts.cn

List(1, 2, 3).map(_ * 2)
来源：http://bg.yuntaijiaju.cn

[T55] Scala：集合过滤
来源：http://dv.shxzskj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xg.bookmarksfly.cn

[T56] Scala：样例类
来源：http://qf.panjiajie.cn

case class User(name: String, age: Int)
来源：http://hi.lnxyls.cn

[T57] Scala：模式匹配
来源：http://fl.newstarts.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://no.muxihuayi.cn

[T58] Scala：函数定义
来源：http://uq.newstarts.cn

def add(a: Int, b: Int): Int = a + b
来源：http://lt.jctech888.com.cn

[T59] Scala：循环
来源：http://iv.muxihuayi.cn

for (i <- 1 to 10) println(i)
来源：http://vo.newstarts.cn

[T60] Scala：折叠
来源：http://ds.hnjuh.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qa.muxihuayi.cn

================================================================================
来源：http://ub.bookmarksfly.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pc.shxzukj.cn

================================================================================
来源：http://rf.newstarts.cn

[U01] Py：创建虚拟环境
来源：http://ya.szsharing.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cj.szxytkj.cn

[U02] Py：导出 / 安装依赖
来源：http://gd.haigaiapp.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wj.shtwfgs.cn

[U03] Py：加载 .env 配置
来源：http://uu.huixinmuqiang.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://hh.wgjwhj.cn

[U04] Py：变量调试打印
来源：http://ea.yuexingan06.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rw.hahajie.cn

[U05] Py：列表去重且保序
来源：http://ov.colortex.cn

list(dict.fromkeys(arr))
来源：http://yl.jctech888.com.cn

[U06] Py：合并两个字典
来源：http://ff.nicolike.cn

{**a, **b}
来源：http://il.wgjwhj.cn

[U07] Py：反转字典键值
来源：http://zm.nszjky.cn

{v: k for k, v in d.items()}
来源：http://fu.colortex.cn

[U08] Py：展平二维列表
来源：http://rm.yuntaijiaju.cn

[y for x in nested for y in x]
来源：http://zr.bookmarksfly.cn

[U09] Py：字典取最大值的键
来源：http://xn.gzmigu.cn

max(d, key=d.get)
来源：http://jy.asd995.cn

[U10] Py：按值排序字典
来源：http://ne.wgjwhj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://iy.bookmarksfly.cn

[U11] Py：生成器表达式
来源：http://km.bjjhwx.cn

(x * 2 for x in arr)
来源：http://ao.chemitech.net.cn

[U12] Py：取出现最多的 3 个元素
来源：http://nb.nszjky.cn

Counter(arr).most_common(3)
来源：http://kf.gzmigu.cn

[U13] Py：固定长度队列
来源：http://ok.huixinmuqiang.cn

deque(maxlen=10)
来源：http://sn.colortex.cn

[U14] Py：分组收集到列表
来源：http://ip.nicolike.cn

defaultdict(list)
来源：http://ch.szxytkj.cn

[U15] Py：高精度计时
来源：http://rq.shtwfgs.cn

t = time.perf_counter()
来源：http://ag.jianghongdianzi.cn

[U16] Py：命令行参数解析
来源：http://de.szsharing.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vt.huixinmuqiang.cn

[U17] Py：初始化日志
来源：http://gf.huixinmuqiang.cn

logging.basicConfig(level=logging.INFO)
来源：http://ly.hahajie.cn

[U18] Py：预编译正则
来源：http://so.wgjwhj.cn

pat = re.compile(r"\d+")
来源：http://qd.yuexingan06.cn

[U19] Py：正则替换带回调
来源：http://xh.9csxet.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sk.shtwfgs.cn

[U20] Py：缓存函数结果
来源：http://ns.panjiajie.cn

@functools.lru_cache(maxsize=None)
来源：http://vl.huanxung.cn

[U21] Py：自定义上下文管理器
来源：http://kx.szsharing.cn

@contextlib.contextmanager
来源：http://re.shxzukj.cn

[U22] Py：矩阵转置
来源：http://wd.yuexingan06.cn

list(zip(*m))
来源：http://zb.hahajie.cn

[U23] Py：分块读取大文件
来源：http://vj.hahajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rp.jctech888.com.cn

[U24] Py：路径操作
来源：http://ro.huixiangedu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xs.asd995.cn

[U25] Py：CSV 按字典读
来源：http://cp.jctech888.com.cn

csv.DictReader(f)
来源：http://lh.gzmigu.cn

[U26] Py：并发下载
来源：http://vr.shxzskj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wc.yuntaijiaju.cn

[U27] Py：异步 HTTP
来源：http://if.huixiangedu.cn

aiohttp.ClientSession() 配合 async with
来源：http://dr.nszjky.cn

[U28] Py：类型别名
来源：http://tc.wgjwhj.cn

UserId = int
来源：http://lq.jianghongdianzi.cn

[U29] Py：属性校验
来源：http://ed.jctech888.com.cn

@property 与 @x.setter 配合
来源：http://wz.huixinmuqiang.cn

[U30] Py：数据类
来源：http://fr.chemitech.net.cn

@dataclass(slots=True)
来源：http://kp.huixinmuqiang.cn

[U31] Py：单测
来源：http://bx.jctech888.com.cn

python -m pytest -q
来源：http://rj.jctech888.com.cn

[U32] Py：代码格式化
来源：http://tp.bookmarksfly.cn

ruff format . && ruff check --fix .
来源：http://uw.shxzukj.cn

[U33] Py：打包发布
来源：http://vc.lnxyls.cn

python -m build  （依赖 pyproject.toml）
来源：http://zk.shxzukj.cn

[U34] Py：判断编码
来源：http://an.bjjhwx.cn

chardet.detect(raw)
来源：http://kc.hnjuh.cn

[U35] Py：发送邮件
来源：http://nu.hahajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mw.jianghongdianzi.cn

[U36] Py：定时任务
来源：http://ou.hahajie.cn

schedule.every(10).minutes.do(job)
来源：http://qj.yuntaijiaju.cn

[U37] Py：读写 Excel
来源：http://ql.huixiangedu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://iy.gzmigu.cn

[U38] Py：获取脚本所在目录
来源：http://ti.bookmarksfly.cn

Path(__file__).resolve().parent
来源：http://gr.9csxet.cn

[U39] Py：判断是否在交互环境
来源：http://yy.szxytkj.cn

sys.stdout.isatty()
来源：http://pf.haigaiapp.cn

[U40] Py：打印到标准错误
来源：http://rb.szsharing.cn

print("err", file=sys.stderr)
来源：http://lz.bjjhwx.cn

[U41] PHP：初始化 Composer 项目
来源：http://lc.colortex.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xm.haigaiapp.cn

[U42] PHP：PSR-4 自动加载
来源：http://jw.9csxet.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ui.bookmarksfly.cn

[U43] PHP：声明命名空间
来源：http://vc.jctech888.com.cn

namespace App\Http;
来源：http://tu.hahajie.cn

[U44] PHP：开启严格类型
来源：http://jh.huixinmuqiang.cn

declare(strict_types=1);
来源：http://ax.shxzukj.cn

[U45] PHP：类型声明与返回类型
来源：http://ks.jianghongdianzi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ru.jianghongdianzi.cn

[U46] PHP：可空类型
来源：http://vk.huixiangedu.cn

?string $name = null
来源：http://un.shtwfgs.cn

[U47] PHP：联合类型
来源：http://wc.yuntaijiaju.cn

int|string $id
来源：http://mn.huixiangedu.cn

[U48] PHP：纯枚举
来源：http://nr.hnjuh.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ap.521024.cn

[U49] PHP：只读属性
来源：http://eg.yuexingan06.cn

public readonly string $name
来源：http://hz.bjjhwx.cn

[U50] PHP：构造器属性提升
来源：http://ic.newstarts.cn

public function __construct(private int $id) {}
来源：http://vm.chemitech.net.cn

[U51] PHP：数组解构
来源：http://te.muxihuayi.cn

[$a, $b] = $arr;
来源：http://ne.haigaiapp.cn

[U52] PHP：箭头函数
来源：http://ys.nszjky.cn

$double = fn($x) => $x * 2;
来源：http://pl.shtwfgs.cn

[U53] PHP：空合并运算符
来源：http://xz.muxihuayi.cn

$v = $a ?? $b ?? "default";
来源：http://mo.hnjuh.cn

[U54] PHP：空安全调用
来源：http://zn.nszjky.cn

$obj?->method()
来源：http://ip.yuexingan06.cn

[U55] PHP：match 表达式
来源：http://fk.wgjwhj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zf.jctech888.com.cn

[U56] PHP：命名参数
来源：http://do.chemitech.net.cn

f(a: 1, b: 2)
来源：http://mh.nszjky.cn

[U57] PHP：字符串插值
来源：http://vn.shxzukj.cn

"值: {$a}"
来源：http://nj.yuexingan06.cn

[U58] PHP：数组三件套
来源：http://oq.hnjuh.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://io.szsharing.cn

[U59] PHP：自定义排序
来源：http://aq.newstarts.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ra.jctech888.com.cn

[U60] PHP：JSON 编解码
来源：http://sv.huixiangedu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ot.jctech888.com.cn

[U61] PHP：正则
来源：http://ln.9csxet.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wi.nszjky.cn

[U62] PHP：日期对象
来源：http://zb.huixinmuqiang.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lw.muxihuayi.cn

[U63] PHP：文件读写
来源：http://do.nszjky.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ub.shxzskj.cn

[U64] PHP：目录遍历
来源：http://zi.bookmarksfly.cn

glob("dir/*.php");  scandir("dir");
来源：http://tp.yuntaijiaju.cn

[U65] PHP：会话
来源：http://at.huixiangedu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://sy.nszjky.cn

[U66] PHP：设置 Cookie
来源：http://dm.shxzukj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tq.haigaiapp.cn

[U67] PHP：处理文件上传
来源：http://up.szsharing.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dw.bookmarksfly.cn

[U68] PHP：PDO 连接
来源：http://xy.bookmarksfly.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://td.colortex.cn

[U69] PHP：PDO 预处理
来源：http://wa.bookmarksfly.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://so.nicolike.cn

[U70] PHP：PDO 事务
来源：http://ra.lnxyls.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nk.lnxyls.cn

[U71] PHP：抛出异常
来源：http://yn.nicolike.cn

throw new RuntimeException("失败", 500);
来源：http://xu.yuexingan06.cn

[U72] PHP：写错误日志
来源：http://ag.bjjhwx.cn

error_log("失败: " . $e->getMessage());
来源：http://wq.wgjwhj.cn

[U73] PHP：读取 ini 配置
来源：http://lb.huanxung.cn

parse_ini_file("config.ini", true)
来源：http://nz.hnjuh.cn

[U74] PHP：读取环境变量
来源：http://vx.9csxet.cn

getenv("APP_ENV") ?: "production"
来源：http://wh.hnjuh.cn

[U75] PHP：依赖注入
来源：http://yh.wgjwhj.cn

composer require psr/container
来源：http://yq.huixiangedu.cn

[U76] PHP：简单路由
来源：http://bq.nszjky.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ie.chemitech.net.cn

[U77] PHP：模板渲染
来源：http://ir.wgjwhj.cn

composer require twig/twig
来源：http://jo.521024.cn

[U78] PHP：单元测试
来源：http://en.szsharing.cn

composer require --dev phpunit/phpunit
来源：http://zs.szxytkj.cn

[U79] PHP：静态分析
来源：http://hs.hnjuh.cn

composer require --dev phpstan/phpstan
来源：http://uk.hahajie.cn

[U80] PHP：代码规范修复
来源：http://ey.chemitech.net.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://zg.hahajie.cn

[U81] JS：初始化项目
来源：http://ic.shxzskj.cn

npm init -y;  npm i express
来源：http://zj.yuntaijiaju.cn

[U82] JS：package.json 脚本
来源：http://iv.9csxet.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wn.shtwfgs.cn

[U83] JS：ES Module 导入导出
来源：http://fw.haigaiapp.cn

export const a = 1;  import { a } from "./m.js";
来源：http://lh.wgjwhj.cn

[U84] JS：CommonJS 写法
来源：http://bc.shxzskj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://am.jctech888.com.cn

[U85] JS：可选链
来源：http://eq.nicolike.cn

a?.b?.c
来源：http://xa.521024.cn

[U86] JS：空值合并
来源：http://kt.huanxung.cn

a ?? b
来源：http://ww.gzmigu.cn

[U87] JS：解构默认值
来源：http://ha.jianghongdianzi.cn

const { a = 1, b = 2 } = obj;
来源：http://vz.nicolike.cn

[U88] JS：对象展开合并
来源：http://dh.szsharing.cn

{ ...a, ...b }
来源：http://vj.szxytkj.cn

[U89] JS：数组去重
来源：http://yr.panjiajie.cn

[...new Set(arr)]
来源：http://cy.colortex.cn

[U90] JS：数字数组排序
来源：http://ho.panjiajie.cn

[...arr].sort((a, b) => a - b)
来源：http://xy.shxzukj.cn

[U91] JS：对象键值遍历
来源：http://wz.huixinmuqiang.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hu.hahajie.cn

[U92] JS：深拷贝
来源：http://xx.nicolike.cn

structuredClone(obj)
来源：http://qp.muxihuayi.cn


<!-- 参考信息 -->