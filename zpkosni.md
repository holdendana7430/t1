代发 wailian999

[T05] Kotlin：when 表达式
来源：http://kj.huixiangedu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yt.szxytkj.cn

[T06] Kotlin：集合映射
来源：http://ql.huixiangedu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ts.521024.cn

[T07] Kotlin：集合过滤
来源：http://gu.szsharing.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://bq.colortex.cn

[T08] Kotlin：数据类
来源：http://jb.huanxung.cn

data class User(val name: String, val age: Int)
来源：http://tb.hahajie.cn

[T09] Kotlin：扩展函数
来源：http://zu.chemitech.net.cn

fun String.exclaim() = this + "!"
来源：http://wl.chemitech.net.cn

[T10] Kotlin：默认参数
来源：http://td.jianghongdianzi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://uu.szsharing.cn

[T11] Kotlin：协程
来源：http://zw.hnjuh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ko.jctech888.com.cn

[T12] Kotlin：解构声明
来源：http://js.panjiajie.cn

val (a, b) = Pair(1, 2)
来源：http://ig.yuntaijiaju.cn

[T13] Kotlin：只读 Map
来源：http://xa.lnxyls.cn

val m = mapOf("a" to 1)
来源：http://vv.bjjhwx.cn

[T14] Kotlin：循环
来源：http://qt.asd995.cn

for (i in 1..10) println(i)
来源：http://of.haigaiapp.cn

[T15] Kotlin：接口
来源：http://sd.lnxyls.cn

interface Shape { fun area(): Double }
来源：http://rk.szsharing.cn

[T16] Swift：Hello World
来源：http://rz.jctech888.com.cn

print("Hello")
来源：http://rj.jianghongdianzi.cn

[T17] Swift：变量与常量
来源：http://iw.wgjwhj.cn

var a = 1;  let b = 2
来源：http://xj.9csxet.cn

[T18] Swift：字符串插值
来源：http://yr.521024.cn

"值: \(b)"
来源：http://im.szxytkj.cn

[T19] Swift：可选绑定
来源：http://hw.huixiangedu.cn

if let n = opt { print(n) }
来源：http://fg.shtwfgs.cn

[T20] Swift：数组操作
来源：http://al.521024.cn

var a = [1, 2, 3];  a.append(4)
来源：http://cn.521024.cn

[T21] Swift：遍历
来源：http://ae.hahajie.cn

for x in a { print(x) }
来源：http://ty.haigaiapp.cn

[T22] Swift：字典
来源：http://mh.colortex.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ma.gzmigu.cn

[T23] Swift：函数
来源：http://mv.szxytkj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hi.521024.cn

[T24] Swift：闭包
来源：http://lw.bjjhwx.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ry.colortex.cn

[T25] Swift：结构体
来源：http://pm.haigaiapp.cn

struct P { var x: Int }
来源：http://lc.hnjuh.cn

[T26] Swift：类与重写
来源：http://qt.huixinmuqiang.cn

class A: Base { override func f() {} }
来源：http://go.jctech888.com.cn

[T27] Swift：错误处理
来源：http://qq.jctech888.com.cn

do { try f() } catch { print(error) }
来源：http://sj.gzmigu.cn

[T28] Swift：枚举
来源：http://qh.bookmarksfly.cn

enum Color { case red, green }
来源：http://hz.lnxyls.cn

[T29] Swift：guard 提前返回
来源：http://nw.wgjwhj.cn

guard let x = opt else { return }
来源：http://da.521024.cn

[T30] Swift：协议
来源：http://zn.haigaiapp.cn

protocol Shape { func area() -> Double }
来源：http://wm.lnxyls.cn

[T31] Lua：Hello World
来源：http://ty.huanxung.cn

print("Hello")
来源：http://fm.muxihuayi.cn

[T32] Lua：局部变量
来源：http://ey.szxytkj.cn

local a = 1
来源：http://wn.521024.cn

[T33] Lua：表（数组）
来源：http://uk.muxihuayi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://la.jctech888.com.cn

[T34] Lua：遍历表
来源：http://pf.lnxyls.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://am.huixiangedu.cn

[T35] Lua：字典表
来源：http://yx.yuntaijiaju.cn

local d = { a = 1 };  d.b = 2
来源：http://jh.szsharing.cn

[T36] Lua：函数
来源：http://mw.chemitech.net.cn

function add(a, b) return a + b end
来源：http://op.gzmigu.cn

[T37] Lua：字符串拼接
来源：http://xm.panjiajie.cn

"a" .. "b"
来源：http://vr.huanxung.cn

[T38] Lua：条件
来源：http://dp.panjiajie.cn

if x > 0 then print("正") end
来源：http://nu.szxytkj.cn

[T39] Lua：模式匹配
来源：http://cu.nszjky.cn

string.find(s, "%d+")
来源：http://kx.shxzskj.cn

[T40] Lua：元表
来源：http://ys.jianghongdianzi.cn

setmetatable({}, { __index = base })
来源：http://aa.wgjwhj.cn

[T41] Perl：Hello World
来源：http://ou.gzmigu.cn

print "Hello\n";
来源：http://bc.yuntaijiaju.cn

[T42] Perl：变量类型
来源：http://ue.chemitech.net.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ji.huixinmuqiang.cn

[T43] Perl：字符串插值
来源：http://cb.9csxet.cn

"值: $a"
来源：http://em.szxytkj.cn

[T44] Perl：条件
来源：http://uq.chemitech.net.cn

if ($a > 0) { print "正"; }
来源：http://ms.9csxet.cn

[T45] Perl：数组遍历
来源：http://bw.gzmigu.cn

for my $x (@arr) { print $x; }
来源：http://vb.shxzskj.cn

[T46] Perl：哈希操作
来源：http://ei.jianghongdianzi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qr.huixinmuqiang.cn

[T47] Perl：正则捕获
来源：http://nf.huixiangedu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ry.nszjky.cn

[T48] Perl：正则替换
来源：http://ge.chemitech.net.cn

$s =~ s/old/new/g;
来源：http://lj.colortex.cn

[T49] Perl：函数
来源：http://lt.wgjwhj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mr.bjjhwx.cn

[T50] Perl：逐行读文件
来源：http://ta.muxihuayi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wo.gzmigu.cn

while (my $line = <$fh>) { print $line; }
来源：http://xx.hahajie.cn

[T51] Scala：Hello World
来源：http://uw.nicolike.cn

println("Hello")
来源：http://pp.jianghongdianzi.cn

[T52] Scala：变量
来源：http://it.nszjky.cn

val a = 1;  var b = 2
来源：http://fh.shxzukj.cn

[T53] Scala：字符串插值
来源：http://pt.shxzskj.cn

s"值: $b"
来源：http://ti.colortex.cn

[T54] Scala：集合映射
来源：http://uf.haigaiapp.cn

List(1, 2, 3).map(_ * 2)
来源：http://yr.nicolike.cn

[T55] Scala：集合过滤
来源：http://gl.szxytkj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://pn.shxzukj.cn

[T56] Scala：样例类
来源：http://td.shxzukj.cn

case class User(name: String, age: Int)
来源：http://bc.9csxet.cn

[T57] Scala：模式匹配
来源：http://ly.colortex.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://lm.yuntaijiaju.cn

[T58] Scala：函数定义
来源：http://oh.hnjuh.cn

def add(a: Int, b: Int): Int = a + b
来源：http://so.muxihuayi.cn

[T59] Scala：循环
来源：http://lq.muxihuayi.cn

for (i <- 1 to 10) println(i)
来源：http://fh.huixiangedu.cn

[T60] Scala：折叠
来源：http://gn.nicolike.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mn.muxihuayi.cn

================================================================================
来源：http://np.jctech888.com.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wu.asd995.cn

================================================================================
来源：http://ig.huanxung.cn

[U01] Py：创建虚拟环境
来源：http://om.nszjky.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cg.chemitech.net.cn

[U02] Py：导出 / 安装依赖
来源：http://zy.muxihuayi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ns.panjiajie.cn

[U03] Py：加载 .env 配置
来源：http://wh.bookmarksfly.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://nk.shxzskj.cn

[U04] Py：变量调试打印
来源：http://lp.colortex.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ld.gzmigu.cn

[U05] Py：列表去重且保序
来源：http://pd.hahajie.cn

list(dict.fromkeys(arr))
来源：http://wz.lnxyls.cn

[U06] Py：合并两个字典
来源：http://lh.szsharing.cn

{**a, **b}
来源：http://dd.521024.cn

[U07] Py：反转字典键值
来源：http://wx.asd995.cn

{v: k for k, v in d.items()}
来源：http://zk.521024.cn

[U08] Py：展平二维列表
来源：http://sk.shxzukj.cn

[y for x in nested for y in x]
来源：http://mq.nszjky.cn

[U09] Py：字典取最大值的键
来源：http://wu.nszjky.cn

max(d, key=d.get)
来源：http://ei.hnjuh.cn

[U10] Py：按值排序字典
来源：http://mv.shxzskj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zt.shxzskj.cn

[U11] Py：生成器表达式
来源：http://in.haigaiapp.cn

(x * 2 for x in arr)
来源：http://vu.521024.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zd.shxzukj.cn

Counter(arr).most_common(3)
来源：http://ql.jctech888.com.cn

[U13] Py：固定长度队列
来源：http://vw.huixiangedu.cn

deque(maxlen=10)
来源：http://ui.bjjhwx.cn

[U14] Py：分组收集到列表
来源：http://iy.9csxet.cn

defaultdict(list)
来源：http://py.shtwfgs.cn

[U15] Py：高精度计时
来源：http://sf.asd995.cn

t = time.perf_counter()
来源：http://dh.huanxung.cn

[U16] Py：命令行参数解析
来源：http://xp.huanxung.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ld.9csxet.cn

[U17] Py：初始化日志
来源：http://au.huanxung.cn

logging.basicConfig(level=logging.INFO)
来源：http://ko.yuntaijiaju.cn

[U18] Py：预编译正则
来源：http://ml.bookmarksfly.cn

pat = re.compile(r"\d+")
来源：http://le.nszjky.cn

[U19] Py：正则替换带回调
来源：http://va.haigaiapp.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ah.newstarts.cn

[U20] Py：缓存函数结果
来源：http://vs.jianghongdianzi.cn

@functools.lru_cache(maxsize=None)
来源：http://eo.chemitech.net.cn

[U21] Py：自定义上下文管理器
来源：http://pi.newstarts.cn

@contextlib.contextmanager
来源：http://tj.shtwfgs.cn

[U22] Py：矩阵转置
来源：http://yq.wgjwhj.cn

list(zip(*m))
来源：http://qb.yuexingan06.cn

[U23] Py：分块读取大文件
来源：http://hg.muxihuayi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fw.yuntaijiaju.cn

[U24] Py：路径操作
来源：http://eh.shxzukj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ar.huixinmuqiang.cn

[U25] Py：CSV 按字典读
来源：http://by.huixiangedu.cn

csv.DictReader(f)
来源：http://bz.panjiajie.cn

[U26] Py：并发下载
来源：http://oz.shxzskj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://en.9csxet.cn

[U27] Py：异步 HTTP
来源：http://xk.bookmarksfly.cn

aiohttp.ClientSession() 配合 async with
来源：http://tx.jianghongdianzi.cn

[U28] Py：类型别名
来源：http://mp.9csxet.cn

UserId = int
来源：http://jn.nicolike.cn

[U29] Py：属性校验
来源：http://pz.muxihuayi.cn

@property 与 @x.setter 配合
来源：http://pg.yuexingan06.cn

[U30] Py：数据类
来源：http://pz.newstarts.cn

@dataclass(slots=True)
来源：http://dr.bookmarksfly.cn

[U31] Py：单测
来源：http://yd.nicolike.cn

python -m pytest -q
来源：http://ct.muxihuayi.cn

[U32] Py：代码格式化
来源：http://zy.shtwfgs.cn

ruff format . && ruff check --fix .
来源：http://nk.muxihuayi.cn

[U33] Py：打包发布
来源：http://wa.wgjwhj.cn

python -m build  （依赖 pyproject.toml）
来源：http://hn.gzmigu.cn

[U34] Py：判断编码
来源：http://ks.wgjwhj.cn

chardet.detect(raw)
来源：http://ry.wgjwhj.cn

[U35] Py：发送邮件
来源：http://qh.colortex.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mg.szxytkj.cn

[U36] Py：定时任务
来源：http://br.panjiajie.cn

schedule.every(10).minutes.do(job)
来源：http://wk.shtwfgs.cn

[U37] Py：读写 Excel
来源：http://yk.lnxyls.cn

pandas.read_excel / DataFrame.to_excel
来源：http://op.gzmigu.cn

[U38] Py：获取脚本所在目录
来源：http://jc.hahajie.cn

Path(__file__).resolve().parent
来源：http://qh.szsharing.cn

[U39] Py：判断是否在交互环境
来源：http://ff.asd995.cn

sys.stdout.isatty()
来源：http://tx.shxzskj.cn

[U40] Py：打印到标准错误
来源：http://hr.521024.cn

print("err", file=sys.stderr)
来源：http://oc.panjiajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://wa.hnjuh.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://kl.szxytkj.cn

[U42] PHP：PSR-4 自动加载
来源：http://lw.hnjuh.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://za.panjiajie.cn

[U43] PHP：声明命名空间
来源：http://lk.nicolike.cn

namespace App\Http;
来源：http://cf.wgjwhj.cn

[U44] PHP：开启严格类型
来源：http://ri.shxzskj.cn

declare(strict_types=1);
来源：http://ts.gzmigu.cn

[U45] PHP：类型声明与返回类型
来源：http://xd.nicolike.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gzmigu.cn

[U46] PHP：可空类型
来源：http://mf.huixinmuqiang.cn

?string $name = null
来源：http://uv.szsharing.cn

[U47] PHP：联合类型
来源：http://ag.yuexingan06.cn

int|string $id
来源：http://uw.huixinmuqiang.cn

[U48] PHP：纯枚举
来源：http://ic.huixinmuqiang.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://uc.521024.cn

[U49] PHP：只读属性
来源：http://dl.huanxung.cn

public readonly string $name
来源：http://jc.521024.cn

[U50] PHP：构造器属性提升
来源：http://ee.jianghongdianzi.cn

public function __construct(private int $id) {}
来源：http://zj.hnjuh.cn

[U51] PHP：数组解构
来源：http://xx.9csxet.cn

[$a, $b] = $arr;
来源：http://dg.colortex.cn

[U52] PHP：箭头函数
来源：http://ka.jctech888.com.cn

$double = fn($x) => $x * 2;
来源：http://tq.wgjwhj.cn

[U53] PHP：空合并运算符
来源：http://bn.shxzskj.cn

$v = $a ?? $b ?? "default";
来源：http://yz.huanxung.cn

[U54] PHP：空安全调用
来源：http://oi.muxihuayi.cn

$obj?->method()
来源：http://cf.9csxet.cn

[U55] PHP：match 表达式
来源：http://dy.hnjuh.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ve.chemitech.net.cn

[U56] PHP：命名参数
来源：http://zu.shxzukj.cn

f(a: 1, b: 2)
来源：http://ex.huixiangedu.cn

[U57] PHP：字符串插值
来源：http://cb.yuexingan06.cn

"值: {$a}"
来源：http://eb.muxihuayi.cn

[U58] PHP：数组三件套
来源：http://ug.bookmarksfly.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kp.nszjky.cn

[U59] PHP：自定义排序
来源：http://ag.chemitech.net.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rl.hnjuh.cn

[U60] PHP：JSON 编解码
来源：http://dc.shxzukj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xq.521024.cn

[U61] PHP：正则
来源：http://gq.wgjwhj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://uv.huanxung.cn

[U62] PHP：日期对象
来源：http://lc.huixiangedu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jb.shxzukj.cn

[U63] PHP：文件读写
来源：http://uo.shtwfgs.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bf.521024.cn

[U64] PHP：目录遍历
来源：http://mh.shtwfgs.cn

glob("dir/*.php");  scandir("dir");
来源：http://yb.shtwfgs.cn

[U65] PHP：会话
来源：http://an.gzmigu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://my.bookmarksfly.cn

[U66] PHP：设置 Cookie
来源：http://zs.bjjhwx.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fa.yuexingan06.cn

[U67] PHP：处理文件上传
来源：http://zn.gzmigu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pm.newstarts.cn

[U68] PHP：PDO 连接
来源：http://rr.hahajie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nv.muxihuayi.cn

[U69] PHP：PDO 预处理
来源：http://ai.bjjhwx.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vc.wgjwhj.cn

[U70] PHP：PDO 事务
来源：http://ba.yuntaijiaju.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bg.wgjwhj.cn

[U71] PHP：抛出异常
来源：http://vj.szsharing.cn

throw new RuntimeException("失败", 500);
来源：http://wa.521024.cn

[U72] PHP：写错误日志
来源：http://bg.nicolike.cn

error_log("失败: " . $e->getMessage());
来源：http://bt.newstarts.cn

[U73] PHP：读取 ini 配置
来源：http://qo.hnjuh.cn

parse_ini_file("config.ini", true)
来源：http://bl.yuntaijiaju.cn

[U74] PHP：读取环境变量
来源：http://so.jctech888.com.cn

getenv("APP_ENV") ?: "production"
来源：http://yg.lnxyls.cn

[U75] PHP：依赖注入
来源：http://vd.bjjhwx.cn

composer require psr/container
来源：http://mi.bookmarksfly.cn

[U76] PHP：简单路由
来源：http://ea.hnjuh.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yp.jctech888.com.cn

[U77] PHP：模板渲染
来源：http://sr.szsharing.cn

composer require twig/twig
来源：http://ox.haigaiapp.cn

[U78] PHP：单元测试
来源：http://vw.huixinmuqiang.cn

composer require --dev phpunit/phpunit
来源：http://vl.nicolike.cn

[U79] PHP：静态分析
来源：http://ll.shtwfgs.cn

composer require --dev phpstan/phpstan
来源：http://gc.panjiajie.cn

[U80] PHP：代码规范修复
来源：http://qq.colortex.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://cx.nszjky.cn

[U81] JS：初始化项目
来源：http://ac.9csxet.cn

npm init -y;  npm i express
来源：http://is.huixiangedu.cn

[U82] JS：package.json 脚本
来源：http://ka.hahajie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xk.szxytkj.cn

[U83] JS：ES Module 导入导出
来源：http://pe.szsharing.cn

export const a = 1;  import { a } from "./m.js";
来源：http://tx.lnxyls.cn

[U84] JS：CommonJS 写法
来源：http://uk.yuntaijiaju.cn

module.exports = { a };  const { a } = require("./m");
来源：http://qt.yuexingan06.cn

[U85] JS：可选链
来源：http://pz.shtwfgs.cn

a?.b?.c
来源：http://dz.panjiajie.cn

[U86] JS：空值合并
来源：http://oy.huanxung.cn

a ?? b
来源：http://ra.gzmigu.cn

[U87] JS：解构默认值
来源：http://bx.9csxet.cn

const { a = 1, b = 2 } = obj;
来源：http://et.jianghongdianzi.cn

[U88] JS：对象展开合并
来源：http://ua.hahajie.cn

{ ...a, ...b }
来源：http://yy.jctech888.com.cn

[U89] JS：数组去重
来源：http://ga.lnxyls.cn

[...new Set(arr)]
来源：http://yp.shtwfgs.cn

[U90] JS：数字数组排序
来源：http://jt.szsharing.cn

[...arr].sort((a, b) => a - b)
来源：http://mn.huixinmuqiang.cn

[U91] JS：对象键值遍历
来源：http://kd.yuntaijiaju.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nh.asd995.cn

[U92] JS：深拷贝
来源：http://vg.szxytkj.cn

structuredClone(obj)
来源：http://jb.colortex.cn


<!-- 参考信息 -->