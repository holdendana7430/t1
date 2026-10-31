代发 wailian999

[T05] Kotlin：when 表达式
来源：http://ol.wgjwhj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uv.szsharing.cn

[T06] Kotlin：集合映射
来源：http://ia.colortex.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://nl.wgjwhj.cn

[T07] Kotlin：集合过滤
来源：http://zr.colortex.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fe.huixinmuqiang.cn

[T08] Kotlin：数据类
来源：http://cn.9csxet.cn

data class User(val name: String, val age: Int)
来源：http://ft.jianghongdianzi.cn

[T09] Kotlin：扩展函数
来源：http://qb.haigaiapp.cn

fun String.exclaim() = this + "!"
来源：http://xs.jctech888.com.cn

[T10] Kotlin：默认参数
来源：http://ac.9csxet.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rb.gzmigu.cn

[T11] Kotlin：协程
来源：http://yw.colortex.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jz.huixinmuqiang.cn

[T12] Kotlin：解构声明
来源：http://ns.nicolike.cn

val (a, b) = Pair(1, 2)
来源：http://hs.9csxet.cn

[T13] Kotlin：只读 Map
来源：http://jk.colortex.cn

val m = mapOf("a" to 1)
来源：http://ga.hnjuh.cn

[T14] Kotlin：循环
来源：http://ny.nicolike.cn

for (i in 1..10) println(i)
来源：http://ou.shxzskj.cn

[T15] Kotlin：接口
来源：http://wu.shtwfgs.cn

interface Shape { fun area(): Double }
来源：http://hx.asd995.cn

[T16] Swift：Hello World
来源：http://vx.shxzskj.cn

print("Hello")
来源：http://rq.chemitech.net.cn

[T17] Swift：变量与常量
来源：http://bp.nicolike.cn

var a = 1;  let b = 2
来源：http://nu.yuntaijiaju.cn

[T18] Swift：字符串插值
来源：http://cq.wgjwhj.cn

"值: \(b)"
来源：http://vs.colortex.cn

[T19] Swift：可选绑定
来源：http://ie.gzmigu.cn

if let n = opt { print(n) }
来源：http://sa.shxzskj.cn

[T20] Swift：数组操作
来源：http://ne.hnjuh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gf.colortex.cn

[T21] Swift：遍历
来源：http://ir.colortex.cn

for x in a { print(x) }
来源：http://jj.hahajie.cn

[T22] Swift：字典
来源：http://yn.nicolike.cn

var d = ["a": 1];  d["b"] = 2
来源：http://hy.colortex.cn

[T23] Swift：函数
来源：http://em.chemitech.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nd.szxytkj.cn

[T24] Swift：闭包
来源：http://uh.hnjuh.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://az.lnxyls.cn

[T25] Swift：结构体
来源：http://jv.colortex.cn

struct P { var x: Int }
来源：http://gg.haigaiapp.cn

[T26] Swift：类与重写
来源：http://lh.muxihuayi.cn

class A: Base { override func f() {} }
来源：http://qp.panjiajie.cn

[T27] Swift：错误处理
来源：http://nd.hnjuh.cn

do { try f() } catch { print(error) }
来源：http://nq.shxzukj.cn

[T28] Swift：枚举
来源：http://vb.yuntaijiaju.cn

enum Color { case red, green }
来源：http://dk.haigaiapp.cn

[T29] Swift：guard 提前返回
来源：http://ap.huixiangedu.cn

guard let x = opt else { return }
来源：http://hi.wgjwhj.cn

[T30] Swift：协议
来源：http://uq.shtwfgs.cn

protocol Shape { func area() -> Double }
来源：http://wu.521024.cn

[T31] Lua：Hello World
来源：http://cg.jianghongdianzi.cn

print("Hello")
来源：http://qg.bookmarksfly.cn

[T32] Lua：局部变量
来源：http://tp.newstarts.cn

local a = 1
来源：http://ep.newstarts.cn

[T33] Lua：表（数组）
来源：http://tc.szsharing.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://mz.yuntaijiaju.cn

[T34] Lua：遍历表
来源：http://lf.yuexingan06.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://yz.bookmarksfly.cn

[T35] Lua：字典表
来源：http://ay.gzmigu.cn

local d = { a = 1 };  d.b = 2
来源：http://ja.nszjky.cn

[T36] Lua：函数
来源：http://fx.lnxyls.cn

function add(a, b) return a + b end
来源：http://nu.shtwfgs.cn

[T37] Lua：字符串拼接
来源：http://mc.panjiajie.cn

"a" .. "b"
来源：http://gs.nszjky.cn

[T38] Lua：条件
来源：http://wz.nicolike.cn

if x > 0 then print("正") end
来源：http://yy.muxihuayi.cn

[T39] Lua：模式匹配
来源：http://uw.shxzukj.cn

string.find(s, "%d+")
来源：http://bs.hnjuh.cn

[T40] Lua：元表
来源：http://wq.wgjwhj.cn

setmetatable({}, { __index = base })
来源：http://wq.shtwfgs.cn

[T41] Perl：Hello World
来源：http://ht.jianghongdianzi.cn

print "Hello\n";
来源：http://kb.nicolike.cn

[T42] Perl：变量类型
来源：http://vp.colortex.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hl.nicolike.cn

[T43] Perl：字符串插值
来源：http://hr.hnjuh.cn

"值: $a"
来源：http://kd.huixinmuqiang.cn

[T44] Perl：条件
来源：http://oz.panjiajie.cn

if ($a > 0) { print "正"; }
来源：http://dx.9csxet.cn

[T45] Perl：数组遍历
来源：http://jv.huanxung.cn

for my $x (@arr) { print $x; }
来源：http://mx.yuexingan06.cn

[T46] Perl：哈希操作
来源：http://fe.jctech888.com.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lo.panjiajie.cn

[T47] Perl：正则捕获
来源：http://rn.shtwfgs.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dc.nicolike.cn

[T48] Perl：正则替换
来源：http://ox.muxihuayi.cn

$s =~ s/old/new/g;
来源：http://gu.huixiangedu.cn

[T49] Perl：函数
来源：http://ie.lnxyls.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lv.muxihuayi.cn

[T50] Perl：逐行读文件
来源：http://cr.lnxyls.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://dq.newstarts.cn

while (my $line = <$fh>) { print $line; }
来源：http://ch.bookmarksfly.cn

[T51] Scala：Hello World
来源：http://ho.chemitech.net.cn

println("Hello")
来源：http://dr.chemitech.net.cn

[T52] Scala：变量
来源：http://xg.huixinmuqiang.cn

val a = 1;  var b = 2
来源：http://pq.jianghongdianzi.cn

[T53] Scala：字符串插值
来源：http://mn.bookmarksfly.cn

s"值: $b"
来源：http://nw.szsharing.cn

[T54] Scala：集合映射
来源：http://on.colortex.cn

List(1, 2, 3).map(_ * 2)
来源：http://gu.bookmarksfly.cn

[T55] Scala：集合过滤
来源：http://pp.newstarts.cn

List(1, 2, 3).filter(_ > 1)
来源：http://oj.jctech888.com.cn

[T56] Scala：样例类
来源：http://zi.jianghongdianzi.cn

case class User(name: String, age: Int)
来源：http://pf.lnxyls.cn

[T57] Scala：模式匹配
来源：http://ql.newstarts.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://bl.shxzukj.cn

[T58] Scala：函数定义
来源：http://dv.shtwfgs.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zm.9csxet.cn

[T59] Scala：循环
来源：http://fi.hnjuh.cn

for (i <- 1 to 10) println(i)
来源：http://yx.chemitech.net.cn

[T60] Scala：折叠
来源：http://xh.bookmarksfly.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gc.nicolike.cn

================================================================================
来源：http://rk.shxzskj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gn.haigaiapp.cn

================================================================================
来源：http://fu.huanxung.cn

[U01] Py：创建虚拟环境
来源：http://te.muxihuayi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://yk.shxzukj.cn

[U02] Py：导出 / 安装依赖
来源：http://dc.jianghongdianzi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://us.colortex.cn

[U03] Py：加载 .env 配置
来源：http://fn.lnxyls.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xf.nszjky.cn

[U04] Py：变量调试打印
来源：http://zf.szxytkj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vq.521024.cn

[U05] Py：列表去重且保序
来源：http://uw.bookmarksfly.cn

list(dict.fromkeys(arr))
来源：http://wp.jianghongdianzi.cn

[U06] Py：合并两个字典
来源：http://cf.szsharing.cn

{**a, **b}
来源：http://ha.nszjky.cn

[U07] Py：反转字典键值
来源：http://el.jianghongdianzi.cn

{v: k for k, v in d.items()}
来源：http://ee.muxihuayi.cn

[U08] Py：展平二维列表
来源：http://sx.asd995.cn

[y for x in nested for y in x]
来源：http://cz.shtwfgs.cn

[U09] Py：字典取最大值的键
来源：http://wn.nszjky.cn

max(d, key=d.get)
来源：http://dh.bookmarksfly.cn

[U10] Py：按值排序字典
来源：http://xx.bookmarksfly.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://to.jctech888.com.cn

[U11] Py：生成器表达式
来源：http://dc.panjiajie.cn

(x * 2 for x in arr)
来源：http://ev.bjjhwx.cn

[U12] Py：取出现最多的 3 个元素
来源：http://vd.asd995.cn

Counter(arr).most_common(3)
来源：http://zb.huixiangedu.cn

[U13] Py：固定长度队列
来源：http://vm.lnxyls.cn

deque(maxlen=10)
来源：http://ie.gzmigu.cn

[U14] Py：分组收集到列表
来源：http://zj.huixiangedu.cn

defaultdict(list)
来源：http://yt.yuexingan06.cn

[U15] Py：高精度计时
来源：http://fo.panjiajie.cn

t = time.perf_counter()
来源：http://su.shxzskj.cn

[U16] Py：命令行参数解析
来源：http://be.bookmarksfly.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kn.muxihuayi.cn

[U17] Py：初始化日志
来源：http://xj.nszjky.cn

logging.basicConfig(level=logging.INFO)
来源：http://na.szxytkj.cn

[U18] Py：预编译正则
来源：http://dz.nicolike.cn

pat = re.compile(r"\d+")
来源：http://hs.jctech888.com.cn

[U19] Py：正则替换带回调
来源：http://ua.haigaiapp.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cm.newstarts.cn

[U20] Py：缓存函数结果
来源：http://hk.szsharing.cn

@functools.lru_cache(maxsize=None)
来源：http://he.nicolike.cn

[U21] Py：自定义上下文管理器
来源：http://fv.gzmigu.cn

@contextlib.contextmanager
来源：http://jj.newstarts.cn

[U22] Py：矩阵转置
来源：http://gm.jctech888.com.cn

list(zip(*m))
来源：http://qg.huixiangedu.cn

[U23] Py：分块读取大文件
来源：http://ei.521024.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ou.chemitech.net.cn

[U24] Py：路径操作
来源：http://nn.hnjuh.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ut.jianghongdianzi.cn

[U25] Py：CSV 按字典读
来源：http://bz.muxihuayi.cn

csv.DictReader(f)
来源：http://wz.shxzskj.cn

[U26] Py：并发下载
来源：http://zt.yuexingan06.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jp.yuexingan06.cn

[U27] Py：异步 HTTP
来源：http://av.shtwfgs.cn

aiohttp.ClientSession() 配合 async with
来源：http://ax.hahajie.cn

[U28] Py：类型别名
来源：http://ja.huixinmuqiang.cn

UserId = int
来源：http://mm.newstarts.cn

[U29] Py：属性校验
来源：http://ws.nszjky.cn

@property 与 @x.setter 配合
来源：http://ol.huixinmuqiang.cn

[U30] Py：数据类
来源：http://qh.colortex.cn

@dataclass(slots=True)
来源：http://ug.shxzskj.cn

[U31] Py：单测
来源：http://bs.jianghongdianzi.cn

python -m pytest -q
来源：http://kh.bookmarksfly.cn

[U32] Py：代码格式化
来源：http://ba.asd995.cn

ruff format . && ruff check --fix .
来源：http://rr.hahajie.cn

[U33] Py：打包发布
来源：http://ph.hnjuh.cn

python -m build  （依赖 pyproject.toml）
来源：http://be.haigaiapp.cn

[U34] Py：判断编码
来源：http://bi.szxytkj.cn

chardet.detect(raw)
来源：http://jf.wgjwhj.cn

[U35] Py：发送邮件
来源：http://iu.muxihuayi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://al.chemitech.net.cn

[U36] Py：定时任务
来源：http://qg.nszjky.cn

schedule.every(10).minutes.do(job)
来源：http://ln.chemitech.net.cn

[U37] Py：读写 Excel
来源：http://za.bjjhwx.cn

pandas.read_excel / DataFrame.to_excel
来源：http://cb.huanxung.cn

[U38] Py：获取脚本所在目录
来源：http://co.asd995.cn

Path(__file__).resolve().parent
来源：http://ya.hnjuh.cn

[U39] Py：判断是否在交互环境
来源：http://gw.gzmigu.cn

sys.stdout.isatty()
来源：http://db.shxzukj.cn

[U40] Py：打印到标准错误
来源：http://zu.szsharing.cn

print("err", file=sys.stderr)
来源：http://fe.shxzukj.cn

[U41] PHP：初始化 Composer 项目
来源：http://al.yuntaijiaju.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://tl.521024.cn

[U42] PHP：PSR-4 自动加载
来源：http://qt.huanxung.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pf.asd995.cn

[U43] PHP：声明命名空间
来源：http://pa.nszjky.cn

namespace App\Http;
来源：http://nb.huanxung.cn

[U44] PHP：开启严格类型
来源：http://eb.bookmarksfly.cn

declare(strict_types=1);
来源：http://fx.szxytkj.cn

[U45] PHP：类型声明与返回类型
来源：http://sv.lnxyls.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://nh.asd995.cn

[U46] PHP：可空类型
来源：http://yi.bjjhwx.cn

?string $name = null
来源：http://lc.9csxet.cn

[U47] PHP：联合类型
来源：http://ve.newstarts.cn

int|string $id
来源：http://qk.panjiajie.cn

[U48] PHP：纯枚举
来源：http://kb.huixinmuqiang.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xm.panjiajie.cn

[U49] PHP：只读属性
来源：http://nt.yuexingan06.cn

public readonly string $name
来源：http://qe.wgjwhj.cn

[U50] PHP：构造器属性提升
来源：http://zg.9csxet.cn

public function __construct(private int $id) {}
来源：http://hd.chemitech.net.cn

[U51] PHP：数组解构
来源：http://oj.szsharing.cn

[$a, $b] = $arr;
来源：http://da.szsharing.cn

[U52] PHP：箭头函数
来源：http://xa.521024.cn

$double = fn($x) => $x * 2;
来源：http://jk.521024.cn

[U53] PHP：空合并运算符
来源：http://vj.panjiajie.cn

$v = $a ?? $b ?? "default";
来源：http://ri.bookmarksfly.cn

[U54] PHP：空安全调用
来源：http://tm.shxzukj.cn

$obj?->method()
来源：http://iy.shxzskj.cn

[U55] PHP：match 表达式
来源：http://tz.asd995.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uf.shxzukj.cn

[U56] PHP：命名参数
来源：http://yj.colortex.cn

f(a: 1, b: 2)
来源：http://ab.newstarts.cn

[U57] PHP：字符串插值
来源：http://dn.newstarts.cn

"值: {$a}"
来源：http://ig.yuexingan06.cn

[U58] PHP：数组三件套
来源：http://jn.shxzukj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ey.newstarts.cn

[U59] PHP：自定义排序
来源：http://jg.yuexingan06.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mt.colortex.cn

[U60] PHP：JSON 编解码
来源：http://oy.panjiajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ul.chemitech.net.cn

[U61] PHP：正则
来源：http://tu.hahajie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pa.jianghongdianzi.cn

[U62] PHP：日期对象
来源：http://hb.bjjhwx.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ng.521024.cn

[U63] PHP：文件读写
来源：http://sy.jctech888.com.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ze.newstarts.cn

[U64] PHP：目录遍历
来源：http://ry.521024.cn

glob("dir/*.php");  scandir("dir");
来源：http://oq.jctech888.com.cn

[U65] PHP：会话
来源：http://il.bookmarksfly.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://mo.chemitech.net.cn

[U66] PHP：设置 Cookie
来源：http://at.shtwfgs.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://om.huixinmuqiang.cn

[U67] PHP：处理文件上传
来源：http://pl.asd995.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gv.jianghongdianzi.cn

[U68] PHP：PDO 连接
来源：http://rm.muxihuayi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ww.muxihuayi.cn

[U69] PHP：PDO 预处理
来源：http://ml.shxzskj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://su.shxzukj.cn

[U70] PHP：PDO 事务
来源：http://cg.huanxung.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gv.bjjhwx.cn

[U71] PHP：抛出异常
来源：http://yu.newstarts.cn

throw new RuntimeException("失败", 500);
来源：http://ev.shxzskj.cn

[U72] PHP：写错误日志
来源：http://kh.9csxet.cn

error_log("失败: " . $e->getMessage());
来源：http://pf.bjjhwx.cn

[U73] PHP：读取 ini 配置
来源：http://bn.jctech888.com.cn

parse_ini_file("config.ini", true)
来源：http://en.huixinmuqiang.cn

[U74] PHP：读取环境变量
来源：http://wd.yuntaijiaju.cn

getenv("APP_ENV") ?: "production"
来源：http://wa.haigaiapp.cn

[U75] PHP：依赖注入
来源：http://os.newstarts.cn

composer require psr/container
来源：http://ch.yuexingan06.cn

[U76] PHP：简单路由
来源：http://pt.shtwfgs.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fa.jctech888.com.cn

[U77] PHP：模板渲染
来源：http://xx.lnxyls.cn

composer require twig/twig
来源：http://nt.szsharing.cn

[U78] PHP：单元测试
来源：http://li.haigaiapp.cn

composer require --dev phpunit/phpunit
来源：http://xw.gzmigu.cn

[U79] PHP：静态分析
来源：http://ks.nszjky.cn

composer require --dev phpstan/phpstan
来源：http://pq.shtwfgs.cn

[U80] PHP：代码规范修复
来源：http://ba.huixinmuqiang.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://rf.nszjky.cn

[U81] JS：初始化项目
来源：http://va.lnxyls.cn

npm init -y;  npm i express
来源：http://en.nicolike.cn

[U82] JS：package.json 脚本
来源：http://fc.jianghongdianzi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gv.panjiajie.cn

[U83] JS：ES Module 导入导出
来源：http://st.nszjky.cn

export const a = 1;  import { a } from "./m.js";
来源：http://rx.newstarts.cn

[U84] JS：CommonJS 写法
来源：http://fh.asd995.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ek.colortex.cn

[U85] JS：可选链
来源：http://tk.newstarts.cn

a?.b?.c
来源：http://td.lnxyls.cn

[U86] JS：空值合并
来源：http://zm.9csxet.cn

a ?? b
来源：http://ez.yuexingan06.cn

[U87] JS：解构默认值
来源：http://vm.szsharing.cn

const { a = 1, b = 2 } = obj;
来源：http://my.bjjhwx.cn

[U88] JS：对象展开合并
来源：http://rt.nszjky.cn

{ ...a, ...b }
来源：http://pa.asd995.cn

[U89] JS：数组去重
来源：http://fd.szsharing.cn

[...new Set(arr)]
来源：http://dz.bjjhwx.cn

[U90] JS：数字数组排序
来源：http://oo.jianghongdianzi.cn

[...arr].sort((a, b) => a - b)
来源：http://fo.yuntaijiaju.cn

[U91] JS：对象键值遍历
来源：http://fo.panjiajie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://db.shxzukj.cn

[U92] JS：深拷贝
来源：http://pa.asd995.cn

structuredClone(obj)
来源：http://od.hnjuh.cn


<!-- 参考信息 -->