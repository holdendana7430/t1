代发 wailian999

[T03] Kotlin：字符串模板
来源：http://xs.haigaiapp.cn

"值: $b"
来源：http://nv.colortex.cn

[T04] Kotlin：空安全
来源：http://go.nszjky.cn

val n: String? = null;  n?.length
来源：http://vg.huanxung.cn

[T05] Kotlin：when 表达式
来源：http://ei.hnjuh.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cb.jctech888.com.cn

[T06] Kotlin：集合映射
来源：http://cw.asd995.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ab.jianghongdianzi.cn

[T07] Kotlin：集合过滤
来源：http://vx.szxytkj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://hc.asd995.cn

[T08] Kotlin：数据类
来源：http://wx.yuntaijiaju.cn

data class User(val name: String, val age: Int)
来源：http://mo.chemitech.net.cn

[T09] Kotlin：扩展函数
来源：http://fy.yuexingan06.cn

fun String.exclaim() = this + "!"
来源：http://yj.muxihuayi.cn

[T10] Kotlin：默认参数
来源：http://aa.huanxung.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ca.521024.cn

[T11] Kotlin：协程
来源：http://by.jctech888.com.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://yu.hnjuh.cn

[T12] Kotlin：解构声明
来源：http://ed.nszjky.cn

val (a, b) = Pair(1, 2)
来源：http://mb.asd995.cn

[T13] Kotlin：只读 Map
来源：http://ji.shtwfgs.cn

val m = mapOf("a" to 1)
来源：http://vo.shtwfgs.cn

[T14] Kotlin：循环
来源：http://et.nszjky.cn

for (i in 1..10) println(i)
来源：http://ip.asd995.cn

[T15] Kotlin：接口
来源：http://eq.jianghongdianzi.cn

interface Shape { fun area(): Double }
来源：http://wc.szsharing.cn

[T16] Swift：Hello World
来源：http://sj.newstarts.cn

print("Hello")
来源：http://tg.shxzukj.cn

[T17] Swift：变量与常量
来源：http://ms.asd995.cn

var a = 1;  let b = 2
来源：http://qk.shxzukj.cn

[T18] Swift：字符串插值
来源：http://rp.hnjuh.cn

"值: \(b)"
来源：http://jj.jianghongdianzi.cn

[T19] Swift：可选绑定
来源：http://rf.szsharing.cn

if let n = opt { print(n) }
来源：http://rj.gzmigu.cn

[T20] Swift：数组操作
来源：http://sx.521024.cn

var a = [1, 2, 3];  a.append(4)
来源：http://og.nicolike.cn

[T21] Swift：遍历
来源：http://di.shxzskj.cn

for x in a { print(x) }
来源：http://db.9csxet.cn

[T22] Swift：字典
来源：http://tf.wgjwhj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ml.hnjuh.cn

[T23] Swift：函数
来源：http://tw.shxzukj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rl.bookmarksfly.cn

[T24] Swift：闭包
来源：http://jn.lnxyls.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://sy.huixiangedu.cn

[T25] Swift：结构体
来源：http://hz.chemitech.net.cn

struct P { var x: Int }
来源：http://kp.szsharing.cn

[T26] Swift：类与重写
来源：http://qb.colortex.cn

class A: Base { override func f() {} }
来源：http://yc.bjjhwx.cn

[T27] Swift：错误处理
来源：http://dk.shxzskj.cn

do { try f() } catch { print(error) }
来源：http://gt.shxzukj.cn

[T28] Swift：枚举
来源：http://pj.asd995.cn

enum Color { case red, green }
来源：http://gh.9csxet.cn

[T29] Swift：guard 提前返回
来源：http://vh.jianghongdianzi.cn

guard let x = opt else { return }
来源：http://eh.shxzukj.cn

[T30] Swift：协议
来源：http://ui.bookmarksfly.cn

protocol Shape { func area() -> Double }
来源：http://vc.panjiajie.cn

[T31] Lua：Hello World
来源：http://yi.szxytkj.cn

print("Hello")
来源：http://bp.hnjuh.cn

[T32] Lua：局部变量
来源：http://zh.hahajie.cn

local a = 1
来源：http://ro.bookmarksfly.cn

[T33] Lua：表（数组）
来源：http://lf.shxzukj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://sw.shxzukj.cn

[T34] Lua：遍历表
来源：http://su.panjiajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://pq.chemitech.net.cn

[T35] Lua：字典表
来源：http://uf.chemitech.net.cn

local d = { a = 1 };  d.b = 2
来源：http://of.shxzukj.cn

[T36] Lua：函数
来源：http://xk.gzmigu.cn

function add(a, b) return a + b end
来源：http://cr.huixinmuqiang.cn

[T37] Lua：字符串拼接
来源：http://fi.hnjuh.cn

"a" .. "b"
来源：http://pf.shxzukj.cn

[T38] Lua：条件
来源：http://iz.wgjwhj.cn

if x > 0 then print("正") end
来源：http://ce.huanxung.cn

[T39] Lua：模式匹配
来源：http://dq.bjjhwx.cn

string.find(s, "%d+")
来源：http://vv.chemitech.net.cn

[T40] Lua：元表
来源：http://si.muxihuayi.cn

setmetatable({}, { __index = base })
来源：http://bm.huanxung.cn

[T41] Perl：Hello World
来源：http://my.huixinmuqiang.cn

print "Hello\n";
来源：http://mz.jianghongdianzi.cn

[T42] Perl：变量类型
来源：http://gi.panjiajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pb.jctech888.com.cn

[T43] Perl：字符串插值
来源：http://tq.colortex.cn

"值: $a"
来源：http://ky.jianghongdianzi.cn

[T44] Perl：条件
来源：http://mw.newstarts.cn

if ($a > 0) { print "正"; }
来源：http://yl.szsharing.cn

[T45] Perl：数组遍历
来源：http://bm.chemitech.net.cn

for my $x (@arr) { print $x; }
来源：http://va.chemitech.net.cn

[T46] Perl：哈希操作
来源：http://of.nszjky.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ur.yuntaijiaju.cn

[T47] Perl：正则捕获
来源：http://zf.jctech888.com.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vk.521024.cn

[T48] Perl：正则替换
来源：http://vv.bjjhwx.cn

$s =~ s/old/new/g;
来源：http://zt.shxzukj.cn

[T49] Perl：函数
来源：http://cq.huanxung.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kf.jianghongdianzi.cn

[T50] Perl：逐行读文件
来源：http://wi.bookmarksfly.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://lz.521024.cn

while (my $line = <$fh>) { print $line; }
来源：http://xf.huanxung.cn

[T51] Scala：Hello World
来源：http://oa.shxzukj.cn

println("Hello")
来源：http://wt.shtwfgs.cn

[T52] Scala：变量
来源：http://ad.wgjwhj.cn

val a = 1;  var b = 2
来源：http://zf.muxihuayi.cn

[T53] Scala：字符串插值
来源：http://xk.jctech888.com.cn

s"值: $b"
来源：http://ff.nicolike.cn

[T54] Scala：集合映射
来源：http://bc.haigaiapp.cn

List(1, 2, 3).map(_ * 2)
来源：http://qw.huixiangedu.cn

[T55] Scala：集合过滤
来源：http://wf.jianghongdianzi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://mc.bookmarksfly.cn

[T56] Scala：样例类
来源：http://ao.szsharing.cn

case class User(name: String, age: Int)
来源：http://mz.521024.cn

[T57] Scala：模式匹配
来源：http://pu.huixiangedu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tq.muxihuayi.cn

[T58] Scala：函数定义
来源：http://cq.chemitech.net.cn

def add(a: Int, b: Int): Int = a + b
来源：http://tf.9csxet.cn

[T59] Scala：循环
来源：http://sp.shxzukj.cn

for (i <- 1 to 10) println(i)
来源：http://pw.huanxung.cn

[T60] Scala：折叠
来源：http://oh.hahajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ef.521024.cn

================================================================================
来源：http://bx.haigaiapp.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pv.jctech888.com.cn

================================================================================
来源：http://cd.wgjwhj.cn

[U01] Py：创建虚拟环境
来源：http://gk.gzmigu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://rq.asd995.cn

[U02] Py：导出 / 安装依赖
来源：http://to.hnjuh.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mm.bjjhwx.cn

[U03] Py：加载 .env 配置
来源：http://hl.muxihuayi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://oi.521024.cn

[U04] Py：变量调试打印
来源：http://zz.yuexingan06.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ss.nszjky.cn

[U05] Py：列表去重且保序
来源：http://ug.jianghongdianzi.cn

list(dict.fromkeys(arr))
来源：http://mp.gzmigu.cn

[U06] Py：合并两个字典
来源：http://qi.9csxet.cn

{**a, **b}
来源：http://dk.huixiangedu.cn

[U07] Py：反转字典键值
来源：http://rv.muxihuayi.cn

{v: k for k, v in d.items()}
来源：http://lc.szsharing.cn

[U08] Py：展平二维列表
来源：http://lm.jianghongdianzi.cn

[y for x in nested for y in x]
来源：http://ne.colortex.cn

[U09] Py：字典取最大值的键
来源：http://kx.jianghongdianzi.cn

max(d, key=d.get)
来源：http://gf.szsharing.cn

[U10] Py：按值排序字典
来源：http://xb.asd995.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mv.shxzukj.cn

[U11] Py：生成器表达式
来源：http://tf.huixiangedu.cn

(x * 2 for x in arr)
来源：http://iv.gzmigu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://iz.szxytkj.cn

Counter(arr).most_common(3)
来源：http://ur.nicolike.cn

[U13] Py：固定长度队列
来源：http://lt.muxihuayi.cn

deque(maxlen=10)
来源：http://bi.jianghongdianzi.cn

[U14] Py：分组收集到列表
来源：http://qr.lnxyls.cn

defaultdict(list)
来源：http://qd.shxzskj.cn

[U15] Py：高精度计时
来源：http://yd.yuntaijiaju.cn

t = time.perf_counter()
来源：http://zz.newstarts.cn

[U16] Py：命令行参数解析
来源：http://wg.huixiangedu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ct.haigaiapp.cn

[U17] Py：初始化日志
来源：http://rg.panjiajie.cn

logging.basicConfig(level=logging.INFO)
来源：http://qu.huixinmuqiang.cn

[U18] Py：预编译正则
来源：http://bi.szxytkj.cn

pat = re.compile(r"\d+")
来源：http://ag.huanxung.cn

[U19] Py：正则替换带回调
来源：http://fh.szxytkj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://up.chemitech.net.cn

[U20] Py：缓存函数结果
来源：http://lz.newstarts.cn

@functools.lru_cache(maxsize=None)
来源：http://lv.9csxet.cn

[U21] Py：自定义上下文管理器
来源：http://cb.gzmigu.cn

@contextlib.contextmanager
来源：http://bv.521024.cn

[U22] Py：矩阵转置
来源：http://ya.nszjky.cn

list(zip(*m))
来源：http://xk.bjjhwx.cn

[U23] Py：分块读取大文件
来源：http://ju.bookmarksfly.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jp.hnjuh.cn

[U24] Py：路径操作
来源：http://mx.szsharing.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hj.jctech888.com.cn

[U25] Py：CSV 按字典读
来源：http://rw.huixinmuqiang.cn

csv.DictReader(f)
来源：http://dk.521024.cn

[U26] Py：并发下载
来源：http://ux.haigaiapp.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ea.asd995.cn

[U27] Py：异步 HTTP
来源：http://gv.newstarts.cn

aiohttp.ClientSession() 配合 async with
来源：http://jw.huixinmuqiang.cn

[U28] Py：类型别名
来源：http://td.9csxet.cn

UserId = int
来源：http://nk.yuexingan06.cn

[U29] Py：属性校验
来源：http://qi.gzmigu.cn

@property 与 @x.setter 配合
来源：http://km.9csxet.cn

[U30] Py：数据类
来源：http://ni.wgjwhj.cn

@dataclass(slots=True)
来源：http://xw.gzmigu.cn

[U31] Py：单测
来源：http://mh.9csxet.cn

python -m pytest -q
来源：http://ss.shtwfgs.cn

[U32] Py：代码格式化
来源：http://ct.huanxung.cn

ruff format . && ruff check --fix .
来源：http://fg.nicolike.cn

[U33] Py：打包发布
来源：http://qy.bjjhwx.cn

python -m build  （依赖 pyproject.toml）
来源：http://zd.szxytkj.cn

[U34] Py：判断编码
来源：http://ci.panjiajie.cn

chardet.detect(raw)
来源：http://rv.jianghongdianzi.cn

[U35] Py：发送邮件
来源：http://ly.bjjhwx.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pl.haigaiapp.cn

[U36] Py：定时任务
来源：http://vu.bjjhwx.cn

schedule.every(10).minutes.do(job)
来源：http://to.panjiajie.cn

[U37] Py：读写 Excel
来源：http://oc.szsharing.cn

pandas.read_excel / DataFrame.to_excel
来源：http://iv.haigaiapp.cn

[U38] Py：获取脚本所在目录
来源：http://gl.colortex.cn

Path(__file__).resolve().parent
来源：http://ra.gzmigu.cn

[U39] Py：判断是否在交互环境
来源：http://be.nszjky.cn

sys.stdout.isatty()
来源：http://oe.bjjhwx.cn

[U40] Py：打印到标准错误
来源：http://px.huixiangedu.cn

print("err", file=sys.stderr)
来源：http://qq.lnxyls.cn

[U41] PHP：初始化 Composer 项目
来源：http://hq.lnxyls.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xk.hahajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://rm.colortex.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vl.szsharing.cn

[U43] PHP：声明命名空间
来源：http://tz.muxihuayi.cn

namespace App\Http;
来源：http://vk.newstarts.cn

[U44] PHP：开启严格类型
来源：http://hu.huixiangedu.cn

declare(strict_types=1);
来源：http://pt.muxihuayi.cn

[U45] PHP：类型声明与返回类型
来源：http://bi.chemitech.net.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://vg.newstarts.cn

[U46] PHP：可空类型
来源：http://id.jianghongdianzi.cn

?string $name = null
来源：http://fy.huixinmuqiang.cn

[U47] PHP：联合类型
来源：http://bf.szsharing.cn

int|string $id
来源：http://vq.wgjwhj.cn

[U48] PHP：纯枚举
来源：http://xo.panjiajie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ji.muxihuayi.cn

[U49] PHP：只读属性
来源：http://js.jianghongdianzi.cn

public readonly string $name
来源：http://wq.szsharing.cn

[U50] PHP：构造器属性提升
来源：http://zb.newstarts.cn

public function __construct(private int $id) {}
来源：http://qx.nicolike.cn

[U51] PHP：数组解构
来源：http://vn.shtwfgs.cn

[$a, $b] = $arr;
来源：http://iz.jianghongdianzi.cn

[U52] PHP：箭头函数
来源：http://sk.9csxet.cn

$double = fn($x) => $x * 2;
来源：http://fw.bjjhwx.cn

[U53] PHP：空合并运算符
来源：http://rh.wgjwhj.cn

$v = $a ?? $b ?? "default";
来源：http://qx.lnxyls.cn

[U54] PHP：空安全调用
来源：http://ni.hnjuh.cn

$obj?->method()
来源：http://ip.shxzukj.cn

[U55] PHP：match 表达式
来源：http://qw.chemitech.net.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://be.gzmigu.cn

[U56] PHP：命名参数
来源：http://ph.nicolike.cn

f(a: 1, b: 2)
来源：http://rw.chemitech.net.cn

[U57] PHP：字符串插值
来源：http://mq.bjjhwx.cn

"值: {$a}"
来源：http://wg.jianghongdianzi.cn

[U58] PHP：数组三件套
来源：http://hd.szxytkj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ik.haigaiapp.cn

[U59] PHP：自定义排序
来源：http://aw.panjiajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dl.shxzskj.cn

[U60] PHP：JSON 编解码
来源：http://ep.shxzskj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kr.yuntaijiaju.cn

[U61] PHP：正则
来源：http://iq.muxihuayi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kx.huanxung.cn

[U62] PHP：日期对象
来源：http://iz.bjjhwx.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://um.chemitech.net.cn

[U63] PHP：文件读写
来源：http://xh.haigaiapp.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ki.hnjuh.cn

[U64] PHP：目录遍历
来源：http://tq.colortex.cn

glob("dir/*.php");  scandir("dir");
来源：http://az.lnxyls.cn

[U65] PHP：会话
来源：http://bb.9csxet.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://je.shxzskj.cn

[U66] PHP：设置 Cookie
来源：http://rp.shxzskj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cu.huixinmuqiang.cn

[U67] PHP：处理文件上传
来源：http://ka.szsharing.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hy.gzmigu.cn

[U68] PHP：PDO 连接
来源：http://ut.bjjhwx.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mj.colortex.cn

[U69] PHP：PDO 预处理
来源：http://tk.szxytkj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ik.huixinmuqiang.cn

[U70] PHP：PDO 事务
来源：http://wx.chemitech.net.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bb.asd995.cn

[U71] PHP：抛出异常
来源：http://hy.521024.cn

throw new RuntimeException("失败", 500);
来源：http://de.nszjky.cn

[U72] PHP：写错误日志
来源：http://xj.nszjky.cn

error_log("失败: " . $e->getMessage());
来源：http://oa.yuntaijiaju.cn

[U73] PHP：读取 ini 配置
来源：http://az.colortex.cn

parse_ini_file("config.ini", true)
来源：http://ae.bookmarksfly.cn

[U74] PHP：读取环境变量
来源：http://xu.bookmarksfly.cn

getenv("APP_ENV") ?: "production"
来源：http://aa.hahajie.cn

[U75] PHP：依赖注入
来源：http://tx.nicolike.cn

composer require psr/container
来源：http://vh.yuntaijiaju.cn

[U76] PHP：简单路由
来源：http://ej.521024.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bi.newstarts.cn

[U77] PHP：模板渲染
来源：http://bo.chemitech.net.cn

composer require twig/twig
来源：http://sx.haigaiapp.cn

[U78] PHP：单元测试
来源：http://dz.bookmarksfly.cn

composer require --dev phpunit/phpunit
来源：http://ju.yuexingan06.cn

[U79] PHP：静态分析
来源：http://wz.bookmarksfly.cn

composer require --dev phpstan/phpstan
来源：http://fb.nszjky.cn

[U80] PHP：代码规范修复
来源：http://zw.shxzskj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://uv.asd995.cn

[U81] JS：初始化项目
来源：http://ug.newstarts.cn

npm init -y;  npm i express
来源：http://hb.yuntaijiaju.cn

[U82] JS：package.json 脚本
来源：http://js.jctech888.com.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rd.huixiangedu.cn

[U83] JS：ES Module 导入导出
来源：http://ev.nicolike.cn

export const a = 1;  import { a } from "./m.js";
来源：http://eq.shtwfgs.cn

[U84] JS：CommonJS 写法
来源：http://lx.lnxyls.cn

module.exports = { a };  const { a } = require("./m");
来源：http://eu.hnjuh.cn

[U85] JS：可选链
来源：http://qg.hahajie.cn

a?.b?.c
来源：http://gw.muxihuayi.cn

[U86] JS：空值合并
来源：http://no.muxihuayi.cn

a ?? b
来源：http://qu.bjjhwx.cn

[U87] JS：解构默认值
来源：http://bo.yuexingan06.cn

const { a = 1, b = 2 } = obj;
来源：http://ii.9csxet.cn

[U88] JS：对象展开合并
来源：http://nd.shxzskj.cn

{ ...a, ...b }
来源：http://vs.colortex.cn

[U89] JS：数组去重
来源：http://wn.jctech888.com.cn

[...new Set(arr)]
来源：http://zd.panjiajie.cn

[U90] JS：数字数组排序
来源：http://aq.jianghongdianzi.cn

[...arr].sort((a, b) => a - b)
来源：http://na.yuexingan06.cn


<!-- 参考信息 -->