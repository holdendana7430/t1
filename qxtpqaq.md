代发 wailian999

[T03] Kotlin：字符串模板
来源：http://bi.hnjuh.cn

"值: $b"
来源：http://nc.huanxung.cn

[T04] Kotlin：空安全
来源：http://ll.jianghongdianzi.cn

val n: String? = null;  n?.length
来源：http://cr.bjjhwx.cn

[T05] Kotlin：when 表达式
来源：http://gp.521024.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://je.jianghongdianzi.cn

[T06] Kotlin：集合映射
来源：http://hh.muxihuayi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ec.gzmigu.cn

[T07] Kotlin：集合过滤
来源：http://mr.hnjuh.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xy.szxytkj.cn

[T08] Kotlin：数据类
来源：http://yg.yuntaijiaju.cn

data class User(val name: String, val age: Int)
来源：http://jb.hahajie.cn

[T09] Kotlin：扩展函数
来源：http://ym.szsharing.cn

fun String.exclaim() = this + "!"
来源：http://ev.panjiajie.cn

[T10] Kotlin：默认参数
来源：http://zc.huixinmuqiang.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wb.shtwfgs.cn

[T11] Kotlin：协程
来源：http://ii.yuntaijiaju.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ue.shtwfgs.cn

[T12] Kotlin：解构声明
来源：http://cl.colortex.cn

val (a, b) = Pair(1, 2)
来源：http://pq.hnjuh.cn

[T13] Kotlin：只读 Map
来源：http://dl.hnjuh.cn

val m = mapOf("a" to 1)
来源：http://hf.newstarts.cn

[T14] Kotlin：循环
来源：http://va.huixinmuqiang.cn

for (i in 1..10) println(i)
来源：http://zs.asd995.cn

[T15] Kotlin：接口
来源：http://tw.shxzskj.cn

interface Shape { fun area(): Double }
来源：http://yk.haigaiapp.cn

[T16] Swift：Hello World
来源：http://fe.jianghongdianzi.cn

print("Hello")
来源：http://ql.jctech888.com.cn

[T17] Swift：变量与常量
来源：http://am.bjjhwx.cn

var a = 1;  let b = 2
来源：http://di.yuexingan06.cn

[T18] Swift：字符串插值
来源：http://bf.chemitech.net.cn

"值: \(b)"
来源：http://be.newstarts.cn

[T19] Swift：可选绑定
来源：http://vk.shxzukj.cn

if let n = opt { print(n) }
来源：http://hy.newstarts.cn

[T20] Swift：数组操作
来源：http://wd.huanxung.cn

var a = [1, 2, 3];  a.append(4)
来源：http://se.muxihuayi.cn

[T21] Swift：遍历
来源：http://mu.shxzskj.cn

for x in a { print(x) }
来源：http://zf.shxzskj.cn

[T22] Swift：字典
来源：http://pt.lnxyls.cn

var d = ["a": 1];  d["b"] = 2
来源：http://qh.asd995.cn

[T23] Swift：函数
来源：http://ms.yuexingan06.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pa.chemitech.net.cn

[T24] Swift：闭包
来源：http://ol.yuntaijiaju.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vi.yuntaijiaju.cn

[T25] Swift：结构体
来源：http://aq.huixiangedu.cn

struct P { var x: Int }
来源：http://mh.9csxet.cn

[T26] Swift：类与重写
来源：http://lj.haigaiapp.cn

class A: Base { override func f() {} }
来源：http://bt.yuntaijiaju.cn

[T27] Swift：错误处理
来源：http://gh.9csxet.cn

do { try f() } catch { print(error) }
来源：http://kf.shtwfgs.cn

[T28] Swift：枚举
来源：http://oz.panjiajie.cn

enum Color { case red, green }
来源：http://rs.panjiajie.cn

[T29] Swift：guard 提前返回
来源：http://qm.shxzukj.cn

guard let x = opt else { return }
来源：http://fc.huixiangedu.cn

[T30] Swift：协议
来源：http://fg.521024.cn

protocol Shape { func area() -> Double }
来源：http://nh.yuexingan06.cn

[T31] Lua：Hello World
来源：http://ab.bjjhwx.cn

print("Hello")
来源：http://sd.bjjhwx.cn

[T32] Lua：局部变量
来源：http://in.szxytkj.cn

local a = 1
来源：http://ea.szsharing.cn

[T33] Lua：表（数组）
来源：http://zi.lnxyls.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://jb.hnjuh.cn

[T34] Lua：遍历表
来源：http://ly.muxihuayi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vs.colortex.cn

[T35] Lua：字典表
来源：http://pt.hnjuh.cn

local d = { a = 1 };  d.b = 2
来源：http://ah.huixiangedu.cn

[T36] Lua：函数
来源：http://tw.szsharing.cn

function add(a, b) return a + b end
来源：http://js.wgjwhj.cn

[T37] Lua：字符串拼接
来源：http://ba.szxytkj.cn

"a" .. "b"
来源：http://ds.colortex.cn

[T38] Lua：条件
来源：http://zd.yuntaijiaju.cn

if x > 0 then print("正") end
来源：http://an.hnjuh.cn

[T39] Lua：模式匹配
来源：http://ev.jianghongdianzi.cn

string.find(s, "%d+")
来源：http://of.newstarts.cn

[T40] Lua：元表
来源：http://pg.jctech888.com.cn

setmetatable({}, { __index = base })
来源：http://qj.9csxet.cn

[T41] Perl：Hello World
来源：http://zy.chemitech.net.cn

print "Hello\n";
来源：http://pg.hahajie.cn

[T42] Perl：变量类型
来源：http://sa.gzmigu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jx.shxzukj.cn

[T43] Perl：字符串插值
来源：http://nh.bookmarksfly.cn

"值: $a"
来源：http://dq.yuexingan06.cn

[T44] Perl：条件
来源：http://ff.bookmarksfly.cn

if ($a > 0) { print "正"; }
来源：http://mi.asd995.cn

[T45] Perl：数组遍历
来源：http://vy.shxzskj.cn

for my $x (@arr) { print $x; }
来源：http://ot.521024.cn

[T46] Perl：哈希操作
来源：http://fl.jianghongdianzi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://de.haigaiapp.cn

[T47] Perl：正则捕获
来源：http://yv.bjjhwx.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://fd.shxzukj.cn

[T48] Perl：正则替换
来源：http://ph.huixinmuqiang.cn

$s =~ s/old/new/g;
来源：http://rg.muxihuayi.cn

[T49] Perl：函数
来源：http://kv.nszjky.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rx.yuexingan06.cn

[T50] Perl：逐行读文件
来源：http://qg.nicolike.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fg.chemitech.net.cn

while (my $line = <$fh>) { print $line; }
来源：http://vv.shtwfgs.cn

[T51] Scala：Hello World
来源：http://tz.colortex.cn

println("Hello")
来源：http://fj.bookmarksfly.cn

[T52] Scala：变量
来源：http://ae.panjiajie.cn

val a = 1;  var b = 2
来源：http://vf.yuexingan06.cn

[T53] Scala：字符串插值
来源：http://jp.wgjwhj.cn

s"值: $b"
来源：http://ie.panjiajie.cn

[T54] Scala：集合映射
来源：http://qe.9csxet.cn

List(1, 2, 3).map(_ * 2)
来源：http://rl.newstarts.cn

[T55] Scala：集合过滤
来源：http://op.yuexingan06.cn

List(1, 2, 3).filter(_ > 1)
来源：http://kx.haigaiapp.cn

[T56] Scala：样例类
来源：http://oz.nicolike.cn

case class User(name: String, age: Int)
来源：http://lg.lnxyls.cn

[T57] Scala：模式匹配
来源：http://pl.chemitech.net.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://hh.jianghongdianzi.cn

[T58] Scala：函数定义
来源：http://ql.huixinmuqiang.cn

def add(a: Int, b: Int): Int = a + b
来源：http://co.gzmigu.cn

[T59] Scala：循环
来源：http://mh.szsharing.cn

for (i <- 1 to 10) println(i)
来源：http://xy.szxytkj.cn

[T60] Scala：折叠
来源：http://fe.lnxyls.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xr.9csxet.cn

================================================================================
来源：http://em.szsharing.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ox.huixiangedu.cn

================================================================================
来源：http://di.521024.cn

[U01] Py：创建虚拟环境
来源：http://om.521024.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cg.panjiajie.cn

[U02] Py：导出 / 安装依赖
来源：http://fp.9csxet.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vn.521024.cn

[U03] Py：加载 .env 配置
来源：http://fg.jctech888.com.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ri.wgjwhj.cn

[U04] Py：变量调试打印
来源：http://pp.nszjky.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xb.shxzukj.cn

[U05] Py：列表去重且保序
来源：http://aq.hnjuh.cn

list(dict.fromkeys(arr))
来源：http://vg.huanxung.cn

[U06] Py：合并两个字典
来源：http://um.shtwfgs.cn

{**a, **b}
来源：http://dt.521024.cn

[U07] Py：反转字典键值
来源：http://ca.muxihuayi.cn

{v: k for k, v in d.items()}
来源：http://il.newstarts.cn

[U08] Py：展平二维列表
来源：http://hb.szsharing.cn

[y for x in nested for y in x]
来源：http://xg.521024.cn

[U09] Py：字典取最大值的键
来源：http://tf.chemitech.net.cn

max(d, key=d.get)
来源：http://lc.shtwfgs.cn

[U10] Py：按值排序字典
来源：http://nj.bookmarksfly.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://do.huanxung.cn

[U11] Py：生成器表达式
来源：http://ut.szxytkj.cn

(x * 2 for x in arr)
来源：http://ae.panjiajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ro.haigaiapp.cn

Counter(arr).most_common(3)
来源：http://wl.shtwfgs.cn

[U13] Py：固定长度队列
来源：http://hf.huixiangedu.cn

deque(maxlen=10)
来源：http://sg.huanxung.cn

[U14] Py：分组收集到列表
来源：http://vx.hahajie.cn

defaultdict(list)
来源：http://oz.panjiajie.cn

[U15] Py：高精度计时
来源：http://sv.shtwfgs.cn

t = time.perf_counter()
来源：http://lb.yuntaijiaju.cn

[U16] Py：命令行参数解析
来源：http://jd.newstarts.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mz.huixinmuqiang.cn

[U17] Py：初始化日志
来源：http://sl.jctech888.com.cn

logging.basicConfig(level=logging.INFO)
来源：http://ei.hnjuh.cn

[U18] Py：预编译正则
来源：http://rg.colortex.cn

pat = re.compile(r"\d+")
来源：http://di.nszjky.cn

[U19] Py：正则替换带回调
来源：http://ii.haigaiapp.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cf.colortex.cn

[U20] Py：缓存函数结果
来源：http://xr.lnxyls.cn

@functools.lru_cache(maxsize=None)
来源：http://wh.shxzukj.cn

[U21] Py：自定义上下文管理器
来源：http://tt.huanxung.cn

@contextlib.contextmanager
来源：http://er.hnjuh.cn

[U22] Py：矩阵转置
来源：http://dm.bjjhwx.cn

list(zip(*m))
来源：http://gs.panjiajie.cn

[U23] Py：分块读取大文件
来源：http://bn.wgjwhj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ma.yuntaijiaju.cn

[U24] Py：路径操作
来源：http://ud.nszjky.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ye.hahajie.cn

[U25] Py：CSV 按字典读
来源：http://zr.huixinmuqiang.cn

csv.DictReader(f)
来源：http://ws.shtwfgs.cn

[U26] Py：并发下载
来源：http://op.huanxung.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wk.yuexingan06.cn

[U27] Py：异步 HTTP
来源：http://at.panjiajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://mr.nszjky.cn

[U28] Py：类型别名
来源：http://be.shxzskj.cn

UserId = int
来源：http://lw.lnxyls.cn

[U29] Py：属性校验
来源：http://hv.colortex.cn

@property 与 @x.setter 配合
来源：http://fu.panjiajie.cn

[U30] Py：数据类
来源：http://rd.shxzukj.cn

@dataclass(slots=True)
来源：http://ir.asd995.cn

[U31] Py：单测
来源：http://ag.bookmarksfly.cn

python -m pytest -q
来源：http://jn.panjiajie.cn

[U32] Py：代码格式化
来源：http://fq.chemitech.net.cn

ruff format . && ruff check --fix .
来源：http://ys.shxzukj.cn

[U33] Py：打包发布
来源：http://rv.lnxyls.cn

python -m build  （依赖 pyproject.toml）
来源：http://gn.newstarts.cn

[U34] Py：判断编码
来源：http://np.huixiangedu.cn

chardet.detect(raw)
来源：http://so.jianghongdianzi.cn

[U35] Py：发送邮件
来源：http://ys.colortex.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yp.9csxet.cn

[U36] Py：定时任务
来源：http://gj.hahajie.cn

schedule.every(10).minutes.do(job)
来源：http://by.newstarts.cn

[U37] Py：读写 Excel
来源：http://yi.asd995.cn

pandas.read_excel / DataFrame.to_excel
来源：http://yj.gzmigu.cn

[U38] Py：获取脚本所在目录
来源：http://rh.nicolike.cn

Path(__file__).resolve().parent
来源：http://vw.newstarts.cn

[U39] Py：判断是否在交互环境
来源：http://zz.newstarts.cn

sys.stdout.isatty()
来源：http://pe.shtwfgs.cn

[U40] Py：打印到标准错误
来源：http://wj.yuexingan06.cn

print("err", file=sys.stderr)
来源：http://it.wgjwhj.cn

[U41] PHP：初始化 Composer 项目
来源：http://ym.gzmigu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ff.521024.cn

[U42] PHP：PSR-4 自动加载
来源：http://sa.jctech888.com.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sl.bookmarksfly.cn

[U43] PHP：声明命名空间
来源：http://wl.szxytkj.cn

namespace App\Http;
来源：http://ib.hnjuh.cn

[U44] PHP：开启严格类型
来源：http://ag.hnjuh.cn

declare(strict_types=1);
来源：http://ho.asd995.cn

[U45] PHP：类型声明与返回类型
来源：http://wb.shxzukj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://gv.szsharing.cn

[U46] PHP：可空类型
来源：http://at.9csxet.cn

?string $name = null
来源：http://ef.szsharing.cn

[U47] PHP：联合类型
来源：http://mq.shtwfgs.cn

int|string $id
来源：http://zg.colortex.cn

[U48] PHP：纯枚举
来源：http://ga.521024.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zo.jianghongdianzi.cn

[U49] PHP：只读属性
来源：http://za.521024.cn

public readonly string $name
来源：http://vt.yuntaijiaju.cn

[U50] PHP：构造器属性提升
来源：http://vc.newstarts.cn

public function __construct(private int $id) {}
来源：http://iq.bookmarksfly.cn

[U51] PHP：数组解构
来源：http://ld.shtwfgs.cn

[$a, $b] = $arr;
来源：http://vr.521024.cn

[U52] PHP：箭头函数
来源：http://cg.huanxung.cn

$double = fn($x) => $x * 2;
来源：http://ke.panjiajie.cn

[U53] PHP：空合并运算符
来源：http://kd.asd995.cn

$v = $a ?? $b ?? "default";
来源：http://wa.521024.cn

[U54] PHP：空安全调用
来源：http://hh.haigaiapp.cn

$obj?->method()
来源：http://su.nszjky.cn

[U55] PHP：match 表达式
来源：http://of.chemitech.net.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://do.colortex.cn

[U56] PHP：命名参数
来源：http://la.huanxung.cn

f(a: 1, b: 2)
来源：http://gd.hahajie.cn

[U57] PHP：字符串插值
来源：http://zz.muxihuayi.cn

"值: {$a}"
来源：http://bp.nszjky.cn

[U58] PHP：数组三件套
来源：http://dx.jctech888.com.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://an.panjiajie.cn

[U59] PHP：自定义排序
来源：http://to.yuntaijiaju.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uz.newstarts.cn

[U60] PHP：JSON 编解码
来源：http://fl.bjjhwx.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yj.colortex.cn

[U61] PHP：正则
来源：http://xw.chemitech.net.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ik.yuntaijiaju.cn

[U62] PHP：日期对象
来源：http://hn.hnjuh.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ie.hnjuh.cn

[U63] PHP：文件读写
来源：http://cf.huanxung.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qu.huixiangedu.cn

[U64] PHP：目录遍历
来源：http://ul.newstarts.cn

glob("dir/*.php");  scandir("dir");
来源：http://di.chemitech.net.cn

[U65] PHP：会话
来源：http://qs.muxihuayi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://cz.nicolike.cn

[U66] PHP：设置 Cookie
来源：http://el.nicolike.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://db.huixinmuqiang.cn

[U67] PHP：处理文件上传
来源：http://fe.yuexingan06.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mk.wgjwhj.cn

[U68] PHP：PDO 连接
来源：http://et.huixinmuqiang.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bx.shxzukj.cn

[U69] PHP：PDO 预处理
来源：http://ch.panjiajie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lm.newstarts.cn

[U70] PHP：PDO 事务
来源：http://mq.huixiangedu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://he.colortex.cn

[U71] PHP：抛出异常
来源：http://wz.jianghongdianzi.cn

throw new RuntimeException("失败", 500);
来源：http://vh.9csxet.cn

[U72] PHP：写错误日志
来源：http://vd.bookmarksfly.cn

error_log("失败: " . $e->getMessage());
来源：http://pz.colortex.cn

[U73] PHP：读取 ini 配置
来源：http://mm.jctech888.com.cn

parse_ini_file("config.ini", true)
来源：http://kc.lnxyls.cn

[U74] PHP：读取环境变量
来源：http://hb.colortex.cn

getenv("APP_ENV") ?: "production"
来源：http://gn.shxzskj.cn

[U75] PHP：依赖注入
来源：http://zl.newstarts.cn

composer require psr/container
来源：http://zw.bjjhwx.cn

[U76] PHP：简单路由
来源：http://gv.wgjwhj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zd.bookmarksfly.cn

[U77] PHP：模板渲染
来源：http://ws.shtwfgs.cn

composer require twig/twig
来源：http://yk.hahajie.cn

[U78] PHP：单元测试
来源：http://dr.jianghongdianzi.cn

composer require --dev phpunit/phpunit
来源：http://fx.yuexingan06.cn

[U79] PHP：静态分析
来源：http://rm.chemitech.net.cn

composer require --dev phpstan/phpstan
来源：http://vs.yuntaijiaju.cn

[U80] PHP：代码规范修复
来源：http://py.jctech888.com.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://tl.jianghongdianzi.cn

[U81] JS：初始化项目
来源：http://ly.yuexingan06.cn

npm init -y;  npm i express
来源：http://bt.shtwfgs.cn

[U82] JS：package.json 脚本
来源：http://uo.jctech888.com.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://th.colortex.cn

[U83] JS：ES Module 导入导出
来源：http://qy.haigaiapp.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vl.asd995.cn

[U84] JS：CommonJS 写法
来源：http://ow.jctech888.com.cn

module.exports = { a };  const { a } = require("./m");
来源：http://px.bjjhwx.cn

[U85] JS：可选链
来源：http://tb.shxzukj.cn

a?.b?.c
来源：http://wy.nicolike.cn

[U86] JS：空值合并
来源：http://wp.nicolike.cn

a ?? b
来源：http://xk.bjjhwx.cn

[U87] JS：解构默认值
来源：http://vs.hahajie.cn

const { a = 1, b = 2 } = obj;
来源：http://bm.szxytkj.cn

[U88] JS：对象展开合并
来源：http://ru.newstarts.cn

{ ...a, ...b }
来源：http://ul.yuntaijiaju.cn

[U89] JS：数组去重
来源：http://pd.gzmigu.cn

[...new Set(arr)]
来源：http://oy.haigaiapp.cn

[U90] JS：数字数组排序
来源：http://ff.wgjwhj.cn

[...arr].sort((a, b) => a - b)
来源：http://zg.9csxet.cn


<!-- 参考信息 -->