代发 wailian999

[T05] Kotlin：when 表达式
来源：http://wz.asd995.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ei.shxzskj.cn

[T06] Kotlin：集合映射
来源：http://yy.huixinmuqiang.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hx.jctech888.com.cn

[T07] Kotlin：集合过滤
来源：http://ok.colortex.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://th.gzmigu.cn

[T08] Kotlin：数据类
来源：http://ue.gzmigu.cn

data class User(val name: String, val age: Int)
来源：http://lx.jianghongdianzi.cn

[T09] Kotlin：扩展函数
来源：http://kt.huixiangedu.cn

fun String.exclaim() = this + "!"
来源：http://ig.bookmarksfly.cn

[T10] Kotlin：默认参数
来源：http://vm.szxytkj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://iu.lnxyls.cn

[T11] Kotlin：协程
来源：http://mk.jianghongdianzi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://rj.jctech888.com.cn

[T12] Kotlin：解构声明
来源：http://qd.huixinmuqiang.cn

val (a, b) = Pair(1, 2)
来源：http://sg.szxytkj.cn

[T13] Kotlin：只读 Map
来源：http://jx.huanxung.cn

val m = mapOf("a" to 1)
来源：http://xx.hnjuh.cn

[T14] Kotlin：循环
来源：http://dj.huixiangedu.cn

for (i in 1..10) println(i)
来源：http://it.hnjuh.cn

[T15] Kotlin：接口
来源：http://vx.szsharing.cn

interface Shape { fun area(): Double }
来源：http://ow.bookmarksfly.cn

[T16] Swift：Hello World
来源：http://am.panjiajie.cn

print("Hello")
来源：http://oz.nszjky.cn

[T17] Swift：变量与常量
来源：http://hy.shxzskj.cn

var a = 1;  let b = 2
来源：http://jm.gzmigu.cn

[T18] Swift：字符串插值
来源：http://yq.szxytkj.cn

"值: \(b)"
来源：http://is.nszjky.cn

[T19] Swift：可选绑定
来源：http://gh.9csxet.cn

if let n = opt { print(n) }
来源：http://fq.nszjky.cn

[T20] Swift：数组操作
来源：http://nw.jianghongdianzi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://og.colortex.cn

[T21] Swift：遍历
来源：http://uo.huixinmuqiang.cn

for x in a { print(x) }
来源：http://pz.nicolike.cn

[T22] Swift：字典
来源：http://yw.yuntaijiaju.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ke.hahajie.cn

[T23] Swift：函数
来源：http://yp.521024.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gv.bjjhwx.cn

[T24] Swift：闭包
来源：http://ur.hnjuh.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://nq.521024.cn

[T25] Swift：结构体
来源：http://ev.shxzskj.cn

struct P { var x: Int }
来源：http://ir.jianghongdianzi.cn

[T26] Swift：类与重写
来源：http://kk.huixinmuqiang.cn

class A: Base { override func f() {} }
来源：http://mj.hahajie.cn

[T27] Swift：错误处理
来源：http://qq.hnjuh.cn

do { try f() } catch { print(error) }
来源：http://wl.chemitech.net.cn

[T28] Swift：枚举
来源：http://an.gzmigu.cn

enum Color { case red, green }
来源：http://vx.muxihuayi.cn

[T29] Swift：guard 提前返回
来源：http://ip.asd995.cn

guard let x = opt else { return }
来源：http://kh.asd995.cn

[T30] Swift：协议
来源：http://ev.huixinmuqiang.cn

protocol Shape { func area() -> Double }
来源：http://hs.bookmarksfly.cn

[T31] Lua：Hello World
来源：http://hj.bjjhwx.cn

print("Hello")
来源：http://hd.huixinmuqiang.cn

[T32] Lua：局部变量
来源：http://hx.newstarts.cn

local a = 1
来源：http://cc.hahajie.cn

[T33] Lua：表（数组）
来源：http://az.newstarts.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://yv.huanxung.cn

[T34] Lua：遍历表
来源：http://wx.szxytkj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://jw.szxytkj.cn

[T35] Lua：字典表
来源：http://ul.muxihuayi.cn

local d = { a = 1 };  d.b = 2
来源：http://uo.nicolike.cn

[T36] Lua：函数
来源：http://he.hnjuh.cn

function add(a, b) return a + b end
来源：http://oe.muxihuayi.cn

[T37] Lua：字符串拼接
来源：http://ym.huanxung.cn

"a" .. "b"
来源：http://da.521024.cn

[T38] Lua：条件
来源：http://gr.colortex.cn

if x > 0 then print("正") end
来源：http://kf.jianghongdianzi.cn

[T39] Lua：模式匹配
来源：http://jn.huanxung.cn

string.find(s, "%d+")
来源：http://my.chemitech.net.cn

[T40] Lua：元表
来源：http://gh.jctech888.com.cn

setmetatable({}, { __index = base })
来源：http://bo.szsharing.cn

[T41] Perl：Hello World
来源：http://ym.521024.cn

print "Hello\n";
来源：http://ya.chemitech.net.cn

[T42] Perl：变量类型
来源：http://cw.asd995.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://oi.bookmarksfly.cn

[T43] Perl：字符串插值
来源：http://kz.shtwfgs.cn

"值: $a"
来源：http://me.jctech888.com.cn

[T44] Perl：条件
来源：http://bw.9csxet.cn

if ($a > 0) { print "正"; }
来源：http://yr.muxihuayi.cn

[T45] Perl：数组遍历
来源：http://rf.chemitech.net.cn

for my $x (@arr) { print $x; }
来源：http://wp.521024.cn

[T46] Perl：哈希操作
来源：http://zj.asd995.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gs.haigaiapp.cn

[T47] Perl：正则捕获
来源：http://vo.panjiajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://nl.nszjky.cn

[T48] Perl：正则替换
来源：http://vw.panjiajie.cn

$s =~ s/old/new/g;
来源：http://tq.chemitech.net.cn

[T49] Perl：函数
来源：http://ce.nicolike.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sd.jctech888.com.cn

[T50] Perl：逐行读文件
来源：http://er.hnjuh.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zo.haigaiapp.cn

while (my $line = <$fh>) { print $line; }
来源：http://xo.yuntaijiaju.cn

[T51] Scala：Hello World
来源：http://ak.muxihuayi.cn

println("Hello")
来源：http://cu.newstarts.cn

[T52] Scala：变量
来源：http://pp.chemitech.net.cn

val a = 1;  var b = 2
来源：http://ka.szxytkj.cn

[T53] Scala：字符串插值
来源：http://wq.9csxet.cn

s"值: $b"
来源：http://nx.shtwfgs.cn

[T54] Scala：集合映射
来源：http://vp.szxytkj.cn

List(1, 2, 3).map(_ * 2)
来源：http://ns.nicolike.cn

[T55] Scala：集合过滤
来源：http://cs.lnxyls.cn

List(1, 2, 3).filter(_ > 1)
来源：http://yk.shxzukj.cn

[T56] Scala：样例类
来源：http://ft.wgjwhj.cn

case class User(name: String, age: Int)
来源：http://um.shxzskj.cn

[T57] Scala：模式匹配
来源：http://gh.wgjwhj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://nv.shtwfgs.cn

[T58] Scala：函数定义
来源：http://rk.hnjuh.cn

def add(a: Int, b: Int): Int = a + b
来源：http://el.muxihuayi.cn

[T59] Scala：循环
来源：http://ss.wgjwhj.cn

for (i <- 1 to 10) println(i)
来源：http://ha.lnxyls.cn

[T60] Scala：折叠
来源：http://vm.haigaiapp.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xh.colortex.cn

================================================================================
来源：http://is.bjjhwx.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lx.nszjky.cn

================================================================================
来源：http://qm.9csxet.cn

[U01] Py：创建虚拟环境
来源：http://cg.colortex.cn

python -m venv .venv && source .venv/bin/activate
来源：http://sv.hnjuh.cn

[U02] Py：导出 / 安装依赖
来源：http://jd.panjiajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://na.yuexingan06.cn

[U03] Py：加载 .env 配置
来源：http://fx.hnjuh.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rm.wgjwhj.cn

[U04] Py：变量调试打印
来源：http://ij.lnxyls.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cb.haigaiapp.cn

[U05] Py：列表去重且保序
来源：http://nn.szsharing.cn

list(dict.fromkeys(arr))
来源：http://gc.huixiangedu.cn

[U06] Py：合并两个字典
来源：http://et.chemitech.net.cn

{**a, **b}
来源：http://ds.jianghongdianzi.cn

[U07] Py：反转字典键值
来源：http://tz.nszjky.cn

{v: k for k, v in d.items()}
来源：http://iz.nicolike.cn

[U08] Py：展平二维列表
来源：http://uc.muxihuayi.cn

[y for x in nested for y in x]
来源：http://aa.shxzskj.cn

[U09] Py：字典取最大值的键
来源：http://kp.yuntaijiaju.cn

max(d, key=d.get)
来源：http://wl.hnjuh.cn

[U10] Py：按值排序字典
来源：http://wl.shxzukj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fw.shxzskj.cn

[U11] Py：生成器表达式
来源：http://rf.521024.cn

(x * 2 for x in arr)
来源：http://ey.wgjwhj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://oc.lnxyls.cn

Counter(arr).most_common(3)
来源：http://rb.huanxung.cn

[U13] Py：固定长度队列
来源：http://zr.panjiajie.cn

deque(maxlen=10)
来源：http://vx.bjjhwx.cn

[U14] Py：分组收集到列表
来源：http://rq.jctech888.com.cn

defaultdict(list)
来源：http://uh.panjiajie.cn

[U15] Py：高精度计时
来源：http://fy.szsharing.cn

t = time.perf_counter()
来源：http://fn.gzmigu.cn

[U16] Py：命令行参数解析
来源：http://ta.jianghongdianzi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vg.hahajie.cn

[U17] Py：初始化日志
来源：http://pp.yuntaijiaju.cn

logging.basicConfig(level=logging.INFO)
来源：http://vc.shxzskj.cn

[U18] Py：预编译正则
来源：http://ii.hahajie.cn

pat = re.compile(r"\d+")
来源：http://vp.gzmigu.cn

[U19] Py：正则替换带回调
来源：http://ww.haigaiapp.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://oc.szxytkj.cn

[U20] Py：缓存函数结果
来源：http://on.shxzukj.cn

@functools.lru_cache(maxsize=None)
来源：http://od.gzmigu.cn

[U21] Py：自定义上下文管理器
来源：http://nr.gzmigu.cn

@contextlib.contextmanager
来源：http://fv.lnxyls.cn

[U22] Py：矩阵转置
来源：http://un.wgjwhj.cn

list(zip(*m))
来源：http://es.szsharing.cn

[U23] Py：分块读取大文件
来源：http://ol.shtwfgs.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gs.newstarts.cn

[U24] Py：路径操作
来源：http://pv.nszjky.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ch.muxihuayi.cn

[U25] Py：CSV 按字典读
来源：http://ei.9csxet.cn

csv.DictReader(f)
来源：http://hv.gzmigu.cn

[U26] Py：并发下载
来源：http://pm.asd995.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://co.szxytkj.cn

[U27] Py：异步 HTTP
来源：http://fa.yuexingan06.cn

aiohttp.ClientSession() 配合 async with
来源：http://dj.szsharing.cn

[U28] Py：类型别名
来源：http://aw.521024.cn

UserId = int
来源：http://dw.szxytkj.cn

[U29] Py：属性校验
来源：http://xm.hahajie.cn

@property 与 @x.setter 配合
来源：http://kt.szsharing.cn

[U30] Py：数据类
来源：http://af.chemitech.net.cn

@dataclass(slots=True)
来源：http://eh.haigaiapp.cn

[U31] Py：单测
来源：http://xr.jctech888.com.cn

python -m pytest -q
来源：http://rr.wgjwhj.cn

[U32] Py：代码格式化
来源：http://qg.nicolike.cn

ruff format . && ruff check --fix .
来源：http://ph.nszjky.cn

[U33] Py：打包发布
来源：http://gv.wgjwhj.cn

python -m build  （依赖 pyproject.toml）
来源：http://dw.wgjwhj.cn

[U34] Py：判断编码
来源：http://ve.muxihuayi.cn

chardet.detect(raw)
来源：http://zl.huixiangedu.cn

[U35] Py：发送邮件
来源：http://ku.panjiajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hx.bookmarksfly.cn

[U36] Py：定时任务
来源：http://qs.shtwfgs.cn

schedule.every(10).minutes.do(job)
来源：http://xz.nszjky.cn

[U37] Py：读写 Excel
来源：http://hl.szxytkj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://oo.nszjky.cn

[U38] Py：获取脚本所在目录
来源：http://kc.wgjwhj.cn

Path(__file__).resolve().parent
来源：http://lz.nicolike.cn

[U39] Py：判断是否在交互环境
来源：http://mi.hnjuh.cn

sys.stdout.isatty()
来源：http://qj.lnxyls.cn

[U40] Py：打印到标准错误
来源：http://fi.asd995.cn

print("err", file=sys.stderr)
来源：http://mu.hahajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://ri.asd995.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://fi.gzmigu.cn

[U42] PHP：PSR-4 自动加载
来源：http://dd.panjiajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mz.colortex.cn

[U43] PHP：声明命名空间
来源：http://fl.jianghongdianzi.cn

namespace App\Http;
来源：http://ux.szxytkj.cn

[U44] PHP：开启严格类型
来源：http://im.shtwfgs.cn

declare(strict_types=1);
来源：http://sw.colortex.cn

[U45] PHP：类型声明与返回类型
来源：http://sy.521024.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://mb.panjiajie.cn

[U46] PHP：可空类型
来源：http://ia.panjiajie.cn

?string $name = null
来源：http://jk.szxytkj.cn

[U47] PHP：联合类型
来源：http://zd.newstarts.cn

int|string $id
来源：http://qz.colortex.cn

[U48] PHP：纯枚举
来源：http://uc.bookmarksfly.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bc.szxytkj.cn

[U49] PHP：只读属性
来源：http://fy.bookmarksfly.cn

public readonly string $name
来源：http://nx.huixiangedu.cn

[U50] PHP：构造器属性提升
来源：http://ua.shxzskj.cn

public function __construct(private int $id) {}
来源：http://pl.panjiajie.cn

[U51] PHP：数组解构
来源：http://rq.9csxet.cn

[$a, $b] = $arr;
来源：http://se.colortex.cn

[U52] PHP：箭头函数
来源：http://tb.huixinmuqiang.cn

$double = fn($x) => $x * 2;
来源：http://ki.9csxet.cn

[U53] PHP：空合并运算符
来源：http://zp.shxzukj.cn

$v = $a ?? $b ?? "default";
来源：http://hu.asd995.cn

[U54] PHP：空安全调用
来源：http://uw.newstarts.cn

$obj?->method()
来源：http://ch.haigaiapp.cn

[U55] PHP：match 表达式
来源：http://cs.shxzskj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kq.asd995.cn

[U56] PHP：命名参数
来源：http://xs.shxzskj.cn

f(a: 1, b: 2)
来源：http://ec.shxzukj.cn

[U57] PHP：字符串插值
来源：http://du.bookmarksfly.cn

"值: {$a}"
来源：http://dp.shxzskj.cn

[U58] PHP：数组三件套
来源：http://wi.yuntaijiaju.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jx.nicolike.cn

[U59] PHP：自定义排序
来源：http://me.lnxyls.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pw.szxytkj.cn

[U60] PHP：JSON 编解码
来源：http://zs.colortex.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jy.haigaiapp.cn

[U61] PHP：正则
来源：http://nc.yuexingan06.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zi.newstarts.cn

[U62] PHP：日期对象
来源：http://ut.9csxet.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ab.huanxung.cn

[U63] PHP：文件读写
来源：http://mv.huanxung.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rt.huixiangedu.cn

[U64] PHP：目录遍历
来源：http://to.shxzukj.cn

glob("dir/*.php");  scandir("dir");
来源：http://kx.muxihuayi.cn

[U65] PHP：会话
来源：http://lw.wgjwhj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://fw.huixinmuqiang.cn

[U66] PHP：设置 Cookie
来源：http://ul.nszjky.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pn.huixiangedu.cn

[U67] PHP：处理文件上传
来源：http://bc.hnjuh.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nw.huixinmuqiang.cn

[U68] PHP：PDO 连接
来源：http://hc.shxzukj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hn.shxzskj.cn

[U69] PHP：PDO 预处理
来源：http://tb.nszjky.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ga.asd995.cn

[U70] PHP：PDO 事务
来源：http://nd.shxzskj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rs.521024.cn

[U71] PHP：抛出异常
来源：http://kg.panjiajie.cn

throw new RuntimeException("失败", 500);
来源：http://dc.shxzskj.cn

[U72] PHP：写错误日志
来源：http://ud.nszjky.cn

error_log("失败: " . $e->getMessage());
来源：http://tb.yuexingan06.cn

[U73] PHP：读取 ini 配置
来源：http://dp.panjiajie.cn

parse_ini_file("config.ini", true)
来源：http://nt.nicolike.cn

[U74] PHP：读取环境变量
来源：http://bg.haigaiapp.cn

getenv("APP_ENV") ?: "production"
来源：http://tp.newstarts.cn

[U75] PHP：依赖注入
来源：http://dy.chemitech.net.cn

composer require psr/container
来源：http://yf.szsharing.cn

[U76] PHP：简单路由
来源：http://av.szsharing.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cj.huixiangedu.cn

[U77] PHP：模板渲染
来源：http://sf.shxzukj.cn

composer require twig/twig
来源：http://de.9csxet.cn

[U78] PHP：单元测试
来源：http://kw.521024.cn

composer require --dev phpunit/phpunit
来源：http://od.panjiajie.cn

[U79] PHP：静态分析
来源：http://hk.yuexingan06.cn

composer require --dev phpstan/phpstan
来源：http://ms.hnjuh.cn

[U80] PHP：代码规范修复
来源：http://tf.bookmarksfly.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://wq.yuexingan06.cn

[U81] JS：初始化项目
来源：http://uq.newstarts.cn

npm init -y;  npm i express
来源：http://lf.nszjky.cn

[U82] JS：package.json 脚本
来源：http://el.hahajie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wp.newstarts.cn

[U83] JS：ES Module 导入导出
来源：http://pr.yuntaijiaju.cn

export const a = 1;  import { a } from "./m.js";
来源：http://lm.huixinmuqiang.cn

[U84] JS：CommonJS 写法
来源：http://dt.nicolike.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wp.hnjuh.cn

[U85] JS：可选链
来源：http://zd.chemitech.net.cn

a?.b?.c
来源：http://mw.szsharing.cn

[U86] JS：空值合并
来源：http://tc.huanxung.cn

a ?? b
来源：http://tp.gzmigu.cn

[U87] JS：解构默认值
来源：http://se.panjiajie.cn

const { a = 1, b = 2 } = obj;
来源：http://vf.bjjhwx.cn

[U88] JS：对象展开合并
来源：http://dc.jctech888.com.cn

{ ...a, ...b }
来源：http://ds.bookmarksfly.cn

[U89] JS：数组去重
来源：http://lk.jctech888.com.cn

[...new Set(arr)]
来源：http://ec.newstarts.cn

[U90] JS：数字数组排序
来源：http://wn.colortex.cn

[...arr].sort((a, b) => a - b)
来源：http://nu.szxytkj.cn

[U91] JS：对象键值遍历
来源：http://zk.newstarts.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pa.hahajie.cn

[U92] JS：深拷贝
来源：http://pf.9csxet.cn

structuredClone(obj)
来源：http://jt.yuntaijiaju.cn


<!-- 参考信息 -->