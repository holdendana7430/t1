代发 wailian999

[T07] Kotlin：集合过滤
来源：http://vu.9csxet.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://iy.yuexingan06.cn

[T08] Kotlin：数据类
来源：http://rx.yuntaijiaju.cn

data class User(val name: String, val age: Int)
来源：http://tg.chemitech.net.cn

[T09] Kotlin：扩展函数
来源：http://gb.yuntaijiaju.cn

fun String.exclaim() = this + "!"
来源：http://bc.haigaiapp.cn

[T10] Kotlin：默认参数
来源：http://il.bookmarksfly.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gz.shxzukj.cn

[T11] Kotlin：协程
来源：http://ay.szxytkj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://kz.chemitech.net.cn

[T12] Kotlin：解构声明
来源：http://go.huanxung.cn

val (a, b) = Pair(1, 2)
来源：http://so.colortex.cn

[T13] Kotlin：只读 Map
来源：http://lf.hnjuh.cn

val m = mapOf("a" to 1)
来源：http://hv.huanxung.cn

[T14] Kotlin：循环
来源：http://vl.panjiajie.cn

for (i in 1..10) println(i)
来源：http://cz.jianghongdianzi.cn

[T15] Kotlin：接口
来源：http://tt.muxihuayi.cn

interface Shape { fun area(): Double }
来源：http://dr.yuntaijiaju.cn

[T16] Swift：Hello World
来源：http://jx.521024.cn

print("Hello")
来源：http://pf.huixiangedu.cn

[T17] Swift：变量与常量
来源：http://zy.nszjky.cn

var a = 1;  let b = 2
来源：http://yt.yuexingan06.cn

[T18] Swift：字符串插值
来源：http://bp.huixiangedu.cn

"值: \(b)"
来源：http://kt.yuntaijiaju.cn

[T19] Swift：可选绑定
来源：http://su.yuntaijiaju.cn

if let n = opt { print(n) }
来源：http://qy.lnxyls.cn

[T20] Swift：数组操作
来源：http://sv.nicolike.cn

var a = [1, 2, 3];  a.append(4)
来源：http://kr.colortex.cn

[T21] Swift：遍历
来源：http://lo.huixiangedu.cn

for x in a { print(x) }
来源：http://qw.shtwfgs.cn

[T22] Swift：字典
来源：http://xp.yuntaijiaju.cn

var d = ["a": 1];  d["b"] = 2
来源：http://kj.chemitech.net.cn

[T23] Swift：函数
来源：http://gf.shxzskj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rc.szsharing.cn

[T24] Swift：闭包
来源：http://qn.panjiajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://se.bjjhwx.cn

[T25] Swift：结构体
来源：http://zd.asd995.cn

struct P { var x: Int }
来源：http://ux.lnxyls.cn

[T26] Swift：类与重写
来源：http://qn.lnxyls.cn

class A: Base { override func f() {} }
来源：http://nu.huixiangedu.cn

[T27] Swift：错误处理
来源：http://iv.szxytkj.cn

do { try f() } catch { print(error) }
来源：http://ye.bjjhwx.cn

[T28] Swift：枚举
来源：http://aa.jctech888.com.cn

enum Color { case red, green }
来源：http://qb.huanxung.cn

[T29] Swift：guard 提前返回
来源：http://uw.szxytkj.cn

guard let x = opt else { return }
来源：http://vy.muxihuayi.cn

[T30] Swift：协议
来源：http://jr.nicolike.cn

protocol Shape { func area() -> Double }
来源：http://ap.huixinmuqiang.cn

[T31] Lua：Hello World
来源：http://ux.asd995.cn

print("Hello")
来源：http://mv.haigaiapp.cn

[T32] Lua：局部变量
来源：http://jf.yuntaijiaju.cn

local a = 1
来源：http://wl.chemitech.net.cn

[T33] Lua：表（数组）
来源：http://mp.bjjhwx.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ga.hahajie.cn

[T34] Lua：遍历表
来源：http://vy.muxihuayi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://wv.hnjuh.cn

[T35] Lua：字典表
来源：http://xm.shxzukj.cn

local d = { a = 1 };  d.b = 2
来源：http://bj.asd995.cn

[T36] Lua：函数
来源：http://sz.huanxung.cn

function add(a, b) return a + b end
来源：http://vz.newstarts.cn

[T37] Lua：字符串拼接
来源：http://rr.szsharing.cn

"a" .. "b"
来源：http://sd.hnjuh.cn

[T38] Lua：条件
来源：http://xp.newstarts.cn

if x > 0 then print("正") end
来源：http://ck.lnxyls.cn

[T39] Lua：模式匹配
来源：http://zp.colortex.cn

string.find(s, "%d+")
来源：http://so.jctech888.com.cn

[T40] Lua：元表
来源：http://hq.bookmarksfly.cn

setmetatable({}, { __index = base })
来源：http://aj.shtwfgs.cn

[T41] Perl：Hello World
来源：http://tz.bookmarksfly.cn

print "Hello\n";
来源：http://by.521024.cn

[T42] Perl：变量类型
来源：http://si.521024.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bg.shxzskj.cn

[T43] Perl：字符串插值
来源：http://ae.newstarts.cn

"值: $a"
来源：http://gp.hnjuh.cn

[T44] Perl：条件
来源：http://uh.bookmarksfly.cn

if ($a > 0) { print "正"; }
来源：http://cp.gzmigu.cn

[T45] Perl：数组遍历
来源：http://sy.bjjhwx.cn

for my $x (@arr) { print $x; }
来源：http://vm.yuntaijiaju.cn

[T46] Perl：哈希操作
来源：http://ni.colortex.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://au.nicolike.cn

[T47] Perl：正则捕获
来源：http://ra.yuexingan06.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://cm.shxzukj.cn

[T48] Perl：正则替换
来源：http://kf.shxzukj.cn

$s =~ s/old/new/g;
来源：http://xf.chemitech.net.cn

[T49] Perl：函数
来源：http://fx.wgjwhj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rv.shxzukj.cn

[T50] Perl：逐行读文件
来源：http://ny.shxzukj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zk.bjjhwx.cn

while (my $line = <$fh>) { print $line; }
来源：http://bq.huanxung.cn

[T51] Scala：Hello World
来源：http://hh.huixinmuqiang.cn

println("Hello")
来源：http://nd.jianghongdianzi.cn

[T52] Scala：变量
来源：http://tq.yuntaijiaju.cn

val a = 1;  var b = 2
来源：http://mm.jianghongdianzi.cn

[T53] Scala：字符串插值
来源：http://og.panjiajie.cn

s"值: $b"
来源：http://da.lnxyls.cn

[T54] Scala：集合映射
来源：http://in.nicolike.cn

List(1, 2, 3).map(_ * 2)
来源：http://am.lnxyls.cn

[T55] Scala：集合过滤
来源：http://gx.hahajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qt.jianghongdianzi.cn

[T56] Scala：样例类
来源：http://ft.yuntaijiaju.cn

case class User(name: String, age: Int)
来源：http://ip.nicolike.cn

[T57] Scala：模式匹配
来源：http://gu.panjiajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://iy.gzmigu.cn

[T58] Scala：函数定义
来源：http://ks.huixiangedu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ni.nicolike.cn

[T59] Scala：循环
来源：http://bl.521024.cn

for (i <- 1 to 10) println(i)
来源：http://qi.nszjky.cn

[T60] Scala：折叠
来源：http://jm.szsharing.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rc.panjiajie.cn

================================================================================
来源：http://uv.9csxet.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://az.huixiangedu.cn

================================================================================
来源：http://qt.lnxyls.cn

[U01] Py：创建虚拟环境
来源：http://ej.hahajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://lu.szxytkj.cn

[U02] Py：导出 / 安装依赖
来源：http://xo.lnxyls.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xr.shxzskj.cn

[U03] Py：加载 .env 配置
来源：http://ku.wgjwhj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://us.muxihuayi.cn

[U04] Py：变量调试打印
来源：http://tv.asd995.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cc.wgjwhj.cn

[U05] Py：列表去重且保序
来源：http://zc.shtwfgs.cn

list(dict.fromkeys(arr))
来源：http://lq.panjiajie.cn

[U06] Py：合并两个字典
来源：http://wn.jianghongdianzi.cn

{**a, **b}
来源：http://ms.hahajie.cn

[U07] Py：反转字典键值
来源：http://xn.jianghongdianzi.cn

{v: k for k, v in d.items()}
来源：http://jh.huixiangedu.cn

[U08] Py：展平二维列表
来源：http://bx.wgjwhj.cn

[y for x in nested for y in x]
来源：http://al.shxzukj.cn

[U09] Py：字典取最大值的键
来源：http://li.lnxyls.cn

max(d, key=d.get)
来源：http://oe.gzmigu.cn

[U10] Py：按值排序字典
来源：http://sc.shtwfgs.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://us.bjjhwx.cn

[U11] Py：生成器表达式
来源：http://ca.nicolike.cn

(x * 2 for x in arr)
来源：http://mo.huixinmuqiang.cn

[U12] Py：取出现最多的 3 个元素
来源：http://as.shxzskj.cn

Counter(arr).most_common(3)
来源：http://sa.muxihuayi.cn

[U13] Py：固定长度队列
来源：http://wt.muxihuayi.cn

deque(maxlen=10)
来源：http://au.muxihuayi.cn

[U14] Py：分组收集到列表
来源：http://jc.bjjhwx.cn

defaultdict(list)
来源：http://ie.colortex.cn

[U15] Py：高精度计时
来源：http://sn.521024.cn

t = time.perf_counter()
来源：http://ig.asd995.cn

[U16] Py：命令行参数解析
来源：http://gn.bookmarksfly.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ia.haigaiapp.cn

[U17] Py：初始化日志
来源：http://wa.lnxyls.cn

logging.basicConfig(level=logging.INFO)
来源：http://yt.szsharing.cn

[U18] Py：预编译正则
来源：http://mh.bjjhwx.cn

pat = re.compile(r"\d+")
来源：http://cu.lnxyls.cn

[U19] Py：正则替换带回调
来源：http://ov.lnxyls.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://da.colortex.cn

[U20] Py：缓存函数结果
来源：http://zu.muxihuayi.cn

@functools.lru_cache(maxsize=None)
来源：http://cf.hnjuh.cn

[U21] Py：自定义上下文管理器
来源：http://bc.huixiangedu.cn

@contextlib.contextmanager
来源：http://im.nicolike.cn

[U22] Py：矩阵转置
来源：http://iv.521024.cn

list(zip(*m))
来源：http://nl.newstarts.cn

[U23] Py：分块读取大文件
来源：http://lq.shxzskj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xq.gzmigu.cn

[U24] Py：路径操作
来源：http://bu.wgjwhj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ug.wgjwhj.cn

[U25] Py：CSV 按字典读
来源：http://qw.jctech888.com.cn

csv.DictReader(f)
来源：http://fo.muxihuayi.cn

[U26] Py：并发下载
来源：http://zi.hnjuh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gh.newstarts.cn

[U27] Py：异步 HTTP
来源：http://bd.gzmigu.cn

aiohttp.ClientSession() 配合 async with
来源：http://my.9csxet.cn

[U28] Py：类型别名
来源：http://pt.chemitech.net.cn

UserId = int
来源：http://xa.jianghongdianzi.cn

[U29] Py：属性校验
来源：http://pb.nszjky.cn

@property 与 @x.setter 配合
来源：http://me.shxzukj.cn

[U30] Py：数据类
来源：http://cl.shxzskj.cn

@dataclass(slots=True)
来源：http://xx.jctech888.com.cn

[U31] Py：单测
来源：http://mc.huixinmuqiang.cn

python -m pytest -q
来源：http://qf.huanxung.cn

[U32] Py：代码格式化
来源：http://aj.yuntaijiaju.cn

ruff format . && ruff check --fix .
来源：http://lg.shtwfgs.cn

[U33] Py：打包发布
来源：http://bm.huixiangedu.cn

python -m build  （依赖 pyproject.toml）
来源：http://xp.huixinmuqiang.cn

[U34] Py：判断编码
来源：http://gs.hnjuh.cn

chardet.detect(raw)
来源：http://gz.haigaiapp.cn

[U35] Py：发送邮件
来源：http://gp.jctech888.com.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ql.panjiajie.cn

[U36] Py：定时任务
来源：http://za.asd995.cn

schedule.every(10).minutes.do(job)
来源：http://zi.yuntaijiaju.cn

[U37] Py：读写 Excel
来源：http://br.shxzukj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://pn.chemitech.net.cn

[U38] Py：获取脚本所在目录
来源：http://am.asd995.cn

Path(__file__).resolve().parent
来源：http://lp.muxihuayi.cn

[U39] Py：判断是否在交互环境
来源：http://xz.wgjwhj.cn

sys.stdout.isatty()
来源：http://ad.panjiajie.cn

[U40] Py：打印到标准错误
来源：http://pd.muxihuayi.cn

print("err", file=sys.stderr)
来源：http://oi.muxihuayi.cn

[U41] PHP：初始化 Composer 项目
来源：http://ng.bjjhwx.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.colortex.cn

[U42] PHP：PSR-4 自动加载
来源：http://aw.gzmigu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ax.yuexingan06.cn

[U43] PHP：声明命名空间
来源：http://gs.yuntaijiaju.cn

namespace App\Http;
来源：http://ya.hnjuh.cn

[U44] PHP：开启严格类型
来源：http://ul.9csxet.cn

declare(strict_types=1);
来源：http://bv.yuexingan06.cn

[U45] PHP：类型声明与返回类型
来源：http://fj.shxzukj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://tq.hnjuh.cn

[U46] PHP：可空类型
来源：http://ov.521024.cn

?string $name = null
来源：http://jg.huanxung.cn

[U47] PHP：联合类型
来源：http://sm.panjiajie.cn

int|string $id
来源：http://jd.9csxet.cn

[U48] PHP：纯枚举
来源：http://zs.muxihuayi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pm.asd995.cn

[U49] PHP：只读属性
来源：http://os.szxytkj.cn

public readonly string $name
来源：http://vj.asd995.cn

[U50] PHP：构造器属性提升
来源：http://ug.shtwfgs.cn

public function __construct(private int $id) {}
来源：http://do.szsharing.cn

[U51] PHP：数组解构
来源：http://dl.shxzukj.cn

[$a, $b] = $arr;
来源：http://bk.gzmigu.cn

[U52] PHP：箭头函数
来源：http://pq.jianghongdianzi.cn

$double = fn($x) => $x * 2;
来源：http://ii.szxytkj.cn

[U53] PHP：空合并运算符
来源：http://vx.yuntaijiaju.cn

$v = $a ?? $b ?? "default";
来源：http://bk.yuexingan06.cn

[U54] PHP：空安全调用
来源：http://uw.nszjky.cn

$obj?->method()
来源：http://se.shtwfgs.cn

[U55] PHP：match 表达式
来源：http://rp.9csxet.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xt.wgjwhj.cn

[U56] PHP：命名参数
来源：http://hk.szxytkj.cn

f(a: 1, b: 2)
来源：http://eo.yuntaijiaju.cn

[U57] PHP：字符串插值
来源：http://oc.shtwfgs.cn

"值: {$a}"
来源：http://xq.colortex.cn

[U58] PHP：数组三件套
来源：http://ck.lnxyls.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ip.gzmigu.cn

[U59] PHP：自定义排序
来源：http://xw.panjiajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://on.muxihuayi.cn

[U60] PHP：JSON 编解码
来源：http://kj.chemitech.net.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fg.muxihuayi.cn

[U61] PHP：正则
来源：http://cu.newstarts.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ns.shxzskj.cn

[U62] PHP：日期对象
来源：http://tv.521024.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zz.gzmigu.cn

[U63] PHP：文件读写
来源：http://fs.wgjwhj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rq.yuexingan06.cn

[U64] PHP：目录遍历
来源：http://ee.gzmigu.cn

glob("dir/*.php");  scandir("dir");
来源：http://rd.nicolike.cn

[U65] PHP：会话
来源：http://xg.yuexingan06.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://zw.521024.cn

[U66] PHP：设置 Cookie
来源：http://ww.huixinmuqiang.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cl.shxzukj.cn

[U67] PHP：处理文件上传
来源：http://zd.huixinmuqiang.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ct.chemitech.net.cn

[U68] PHP：PDO 连接
来源：http://vu.huanxung.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yy.hahajie.cn

[U69] PHP：PDO 预处理
来源：http://qt.bookmarksfly.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://op.hnjuh.cn

[U70] PHP：PDO 事务
来源：http://xv.muxihuayi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://eh.hnjuh.cn

[U71] PHP：抛出异常
来源：http://yi.wgjwhj.cn

throw new RuntimeException("失败", 500);
来源：http://dk.shxzukj.cn

[U72] PHP：写错误日志
来源：http://vg.shtwfgs.cn

error_log("失败: " . $e->getMessage());
来源：http://rp.shxzskj.cn

[U73] PHP：读取 ini 配置
来源：http://jn.nszjky.cn

parse_ini_file("config.ini", true)
来源：http://jc.lnxyls.cn

[U74] PHP：读取环境变量
来源：http://xs.asd995.cn

getenv("APP_ENV") ?: "production"
来源：http://oq.haigaiapp.cn

[U75] PHP：依赖注入
来源：http://xa.bjjhwx.cn

composer require psr/container
来源：http://tl.lnxyls.cn

[U76] PHP：简单路由
来源：http://ia.nszjky.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bf.bjjhwx.cn

[U77] PHP：模板渲染
来源：http://cp.huanxung.cn

composer require twig/twig
来源：http://eu.shxzskj.cn

[U78] PHP：单元测试
来源：http://sw.shxzukj.cn

composer require --dev phpunit/phpunit
来源：http://bn.colortex.cn

[U79] PHP：静态分析
来源：http://hf.szsharing.cn

composer require --dev phpstan/phpstan
来源：http://bv.huanxung.cn

[U80] PHP：代码规范修复
来源：http://vh.asd995.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://il.bookmarksfly.cn

[U81] JS：初始化项目
来源：http://vj.gzmigu.cn

npm init -y;  npm i express
来源：http://ii.huanxung.cn

[U82] JS：package.json 脚本
来源：http://pp.muxihuayi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tn.panjiajie.cn

[U83] JS：ES Module 导入导出
来源：http://da.shxzukj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://nx.panjiajie.cn

[U84] JS：CommonJS 写法
来源：http://yf.colortex.cn

module.exports = { a };  const { a } = require("./m");
来源：http://hw.lnxyls.cn

[U85] JS：可选链
来源：http://ey.bjjhwx.cn

a?.b?.c
来源：http://yq.asd995.cn

[U86] JS：空值合并
来源：http://tb.chemitech.net.cn

a ?? b
来源：http://qt.nicolike.cn

[U87] JS：解构默认值
来源：http://ny.shxzukj.cn

const { a = 1, b = 2 } = obj;
来源：http://cs.shtwfgs.cn

[U88] JS：对象展开合并
来源：http://eg.521024.cn

{ ...a, ...b }
来源：http://vm.gzmigu.cn

[U89] JS：数组去重
来源：http://aa.shtwfgs.cn

[...new Set(arr)]
来源：http://wx.wgjwhj.cn

[U90] JS：数字数组排序
来源：http://ct.bookmarksfly.cn

[...arr].sort((a, b) => a - b)
来源：http://fo.shtwfgs.cn

[U91] JS：对象键值遍历
来源：http://qh.jianghongdianzi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hg.huixiangedu.cn

[U92] JS：深拷贝
来源：http://cn.shxzukj.cn

structuredClone(obj)
来源：http://pi.shxzukj.cn

[U93] JS：模板字符串
来源：http://da.newstarts.cn

`共 ${n} 条`
来源：http://fu.colortex.cn

[U94] JS：箭头函数
来源：http://it.haigaiapp.cn

const double = x => x * 2;
来源：http://ra.asd995.cn


<!-- 参考信息 -->