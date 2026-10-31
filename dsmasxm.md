代发 wailian999

[T05] Kotlin：when 表达式
来源：http://bz.gzmigu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xu.wgjwhj.cn

[T06] Kotlin：集合映射
来源：http://qy.shxzukj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fc.panjiajie.cn

[T07] Kotlin：集合过滤
来源：http://yj.shxzskj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://oi.asd995.cn

[T08] Kotlin：数据类
来源：http://dy.hahajie.cn

data class User(val name: String, val age: Int)
来源：http://qp.wgjwhj.cn

[T09] Kotlin：扩展函数
来源：http://th.shxzskj.cn

fun String.exclaim() = this + "!"
来源：http://ld.panjiajie.cn

[T10] Kotlin：默认参数
来源：http://lq.nicolike.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://lk.colortex.cn

[T11] Kotlin：协程
来源：http://qa.wgjwhj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://al.szsharing.cn

[T12] Kotlin：解构声明
来源：http://js.huixiangedu.cn

val (a, b) = Pair(1, 2)
来源：http://zf.521024.cn

[T13] Kotlin：只读 Map
来源：http://kx.haigaiapp.cn

val m = mapOf("a" to 1)
来源：http://fw.jianghongdianzi.cn

[T14] Kotlin：循环
来源：http://iz.bookmarksfly.cn

for (i in 1..10) println(i)
来源：http://ud.panjiajie.cn

[T15] Kotlin：接口
来源：http://ix.bjjhwx.cn

interface Shape { fun area(): Double }
来源：http://ln.nicolike.cn

[T16] Swift：Hello World
来源：http://ii.chemitech.net.cn

print("Hello")
来源：http://ln.lnxyls.cn

[T17] Swift：变量与常量
来源：http://uy.shxzskj.cn

var a = 1;  let b = 2
来源：http://xu.asd995.cn

[T18] Swift：字符串插值
来源：http://qh.bookmarksfly.cn

"值: \(b)"
来源：http://fj.yuntaijiaju.cn

[T19] Swift：可选绑定
来源：http://bp.gzmigu.cn

if let n = opt { print(n) }
来源：http://uo.yuexingan06.cn

[T20] Swift：数组操作
来源：http://kr.colortex.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hk.shtwfgs.cn

[T21] Swift：遍历
来源：http://ia.wgjwhj.cn

for x in a { print(x) }
来源：http://wp.asd995.cn

[T22] Swift：字典
来源：http://aj.szxytkj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://tr.asd995.cn

[T23] Swift：函数
来源：http://qt.521024.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zr.shxzukj.cn

[T24] Swift：闭包
来源：http://bz.bookmarksfly.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vw.9csxet.cn

[T25] Swift：结构体
来源：http://tr.muxihuayi.cn

struct P { var x: Int }
来源：http://rc.jctech888.com.cn

[T26] Swift：类与重写
来源：http://fh.yuntaijiaju.cn

class A: Base { override func f() {} }
来源：http://jw.colortex.cn

[T27] Swift：错误处理
来源：http://yx.jctech888.com.cn

do { try f() } catch { print(error) }
来源：http://fh.asd995.cn

[T28] Swift：枚举
来源：http://tg.shxzukj.cn

enum Color { case red, green }
来源：http://an.chemitech.net.cn

[T29] Swift：guard 提前返回
来源：http://pu.muxihuayi.cn

guard let x = opt else { return }
来源：http://tx.bjjhwx.cn

[T30] Swift：协议
来源：http://ut.muxihuayi.cn

protocol Shape { func area() -> Double }
来源：http://ze.lnxyls.cn

[T31] Lua：Hello World
来源：http://vd.521024.cn

print("Hello")
来源：http://bk.huixiangedu.cn

[T32] Lua：局部变量
来源：http://tm.hnjuh.cn

local a = 1
来源：http://iu.lnxyls.cn

[T33] Lua：表（数组）
来源：http://mk.szxytkj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ng.bjjhwx.cn

[T34] Lua：遍历表
来源：http://dm.bookmarksfly.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://uk.szsharing.cn

[T35] Lua：字典表
来源：http://qf.yuntaijiaju.cn

local d = { a = 1 };  d.b = 2
来源：http://qf.newstarts.cn

[T36] Lua：函数
来源：http://cv.bjjhwx.cn

function add(a, b) return a + b end
来源：http://ll.gzmigu.cn

[T37] Lua：字符串拼接
来源：http://wl.521024.cn

"a" .. "b"
来源：http://nh.colortex.cn

[T38] Lua：条件
来源：http://rk.newstarts.cn

if x > 0 then print("正") end
来源：http://fo.szxytkj.cn

[T39] Lua：模式匹配
来源：http://dv.jctech888.com.cn

string.find(s, "%d+")
来源：http://xp.hnjuh.cn

[T40] Lua：元表
来源：http://qc.szsharing.cn

setmetatable({}, { __index = base })
来源：http://vm.shxzskj.cn

[T41] Perl：Hello World
来源：http://uu.panjiajie.cn

print "Hello\n";
来源：http://gm.jctech888.com.cn

[T42] Perl：变量类型
来源：http://qe.yuntaijiaju.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gy.jianghongdianzi.cn

[T43] Perl：字符串插值
来源：http://dn.haigaiapp.cn

"值: $a"
来源：http://je.newstarts.cn

[T44] Perl：条件
来源：http://hn.jctech888.com.cn

if ($a > 0) { print "正"; }
来源：http://ne.wgjwhj.cn

[T45] Perl：数组遍历
来源：http://tt.nicolike.cn

for my $x (@arr) { print $x; }
来源：http://gp.hahajie.cn

[T46] Perl：哈希操作
来源：http://vz.asd995.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pk.huixiangedu.cn

[T47] Perl：正则捕获
来源：http://gs.yuexingan06.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://tc.bjjhwx.cn

[T48] Perl：正则替换
来源：http://sj.newstarts.cn

$s =~ s/old/new/g;
来源：http://ge.panjiajie.cn

[T49] Perl：函数
来源：http://tt.hnjuh.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mb.lnxyls.cn

[T50] Perl：逐行读文件
来源：http://ij.lnxyls.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zt.shxzukj.cn

while (my $line = <$fh>) { print $line; }
来源：http://lm.521024.cn

[T51] Scala：Hello World
来源：http://yf.521024.cn

println("Hello")
来源：http://au.panjiajie.cn

[T52] Scala：变量
来源：http://em.huixiangedu.cn

val a = 1;  var b = 2
来源：http://py.521024.cn

[T53] Scala：字符串插值
来源：http://nf.szsharing.cn

s"值: $b"
来源：http://es.szsharing.cn

[T54] Scala：集合映射
来源：http://bq.9csxet.cn

List(1, 2, 3).map(_ * 2)
来源：http://xi.lnxyls.cn

[T55] Scala：集合过滤
来源：http://ox.shxzukj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://mm.shxzskj.cn

[T56] Scala：样例类
来源：http://ms.521024.cn

case class User(name: String, age: Int)
来源：http://il.huixinmuqiang.cn

[T57] Scala：模式匹配
来源：http://ae.9csxet.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://qg.shtwfgs.cn

[T58] Scala：函数定义
来源：http://zu.colortex.cn

def add(a: Int, b: Int): Int = a + b
来源：http://os.haigaiapp.cn

[T59] Scala：循环
来源：http://po.lnxyls.cn

for (i <- 1 to 10) println(i)
来源：http://fq.jctech888.com.cn

[T60] Scala：折叠
来源：http://na.gzmigu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://do.shxzukj.cn

================================================================================
来源：http://li.bookmarksfly.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kb.szsharing.cn

================================================================================
来源：http://vv.nicolike.cn

[U01] Py：创建虚拟环境
来源：http://ea.bookmarksfly.cn

python -m venv .venv && source .venv/bin/activate
来源：http://yc.shxzskj.cn

[U02] Py：导出 / 安装依赖
来源：http://wm.szxytkj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cp.wgjwhj.cn

[U03] Py：加载 .env 配置
来源：http://rv.hnjuh.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ez.newstarts.cn

[U04] Py：变量调试打印
来源：http://dy.asd995.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ky.jctech888.com.cn

[U05] Py：列表去重且保序
来源：http://ja.bjjhwx.cn

list(dict.fromkeys(arr))
来源：http://lg.huixiangedu.cn

[U06] Py：合并两个字典
来源：http://oa.haigaiapp.cn

{**a, **b}
来源：http://ts.huanxung.cn

[U07] Py：反转字典键值
来源：http://dr.hnjuh.cn

{v: k for k, v in d.items()}
来源：http://nf.wgjwhj.cn

[U08] Py：展平二维列表
来源：http://wd.yuexingan06.cn

[y for x in nested for y in x]
来源：http://yg.jctech888.com.cn

[U09] Py：字典取最大值的键
来源：http://tn.huixiangedu.cn

max(d, key=d.get)
来源：http://zm.bookmarksfly.cn

[U10] Py：按值排序字典
来源：http://jd.wgjwhj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ni.huixiangedu.cn

[U11] Py：生成器表达式
来源：http://xt.9csxet.cn

(x * 2 for x in arr)
来源：http://un.hnjuh.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mv.gzmigu.cn

Counter(arr).most_common(3)
来源：http://zd.jctech888.com.cn

[U13] Py：固定长度队列
来源：http://lu.wgjwhj.cn

deque(maxlen=10)
来源：http://kl.nszjky.cn

[U14] Py：分组收集到列表
来源：http://fn.shxzskj.cn

defaultdict(list)
来源：http://od.haigaiapp.cn

[U15] Py：高精度计时
来源：http://fg.huixiangedu.cn

t = time.perf_counter()
来源：http://aa.nszjky.cn

[U16] Py：命令行参数解析
来源：http://st.bookmarksfly.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tx.chemitech.net.cn

[U17] Py：初始化日志
来源：http://ad.newstarts.cn

logging.basicConfig(level=logging.INFO)
来源：http://dm.9csxet.cn

[U18] Py：预编译正则
来源：http://ks.521024.cn

pat = re.compile(r"\d+")
来源：http://xq.szxytkj.cn

[U19] Py：正则替换带回调
来源：http://js.nicolike.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cp.newstarts.cn

[U20] Py：缓存函数结果
来源：http://az.hnjuh.cn

@functools.lru_cache(maxsize=None)
来源：http://jo.haigaiapp.cn

[U21] Py：自定义上下文管理器
来源：http://md.9csxet.cn

@contextlib.contextmanager
来源：http://am.shxzukj.cn

[U22] Py：矩阵转置
来源：http://pb.bjjhwx.cn

list(zip(*m))
来源：http://du.szsharing.cn

[U23] Py：分块读取大文件
来源：http://ry.nszjky.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ni.shxzukj.cn

[U24] Py：路径操作
来源：http://fx.chemitech.net.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nn.nszjky.cn

[U25] Py：CSV 按字典读
来源：http://du.shxzukj.cn

csv.DictReader(f)
来源：http://mc.bjjhwx.cn

[U26] Py：并发下载
来源：http://mu.521024.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://sr.panjiajie.cn

[U27] Py：异步 HTTP
来源：http://mz.newstarts.cn

aiohttp.ClientSession() 配合 async with
来源：http://ww.521024.cn

[U28] Py：类型别名
来源：http://ia.newstarts.cn

UserId = int
来源：http://os.jianghongdianzi.cn

[U29] Py：属性校验
来源：http://jj.gzmigu.cn

@property 与 @x.setter 配合
来源：http://fo.521024.cn

[U30] Py：数据类
来源：http://ny.bookmarksfly.cn

@dataclass(slots=True)
来源：http://fu.shxzukj.cn

[U31] Py：单测
来源：http://cf.huixinmuqiang.cn

python -m pytest -q
来源：http://em.asd995.cn

[U32] Py：代码格式化
来源：http://jo.szsharing.cn

ruff format . && ruff check --fix .
来源：http://vt.colortex.cn

[U33] Py：打包发布
来源：http://ni.huanxung.cn

python -m build  （依赖 pyproject.toml）
来源：http://ub.hnjuh.cn

[U34] Py：判断编码
来源：http://ka.colortex.cn

chardet.detect(raw)
来源：http://wl.huixinmuqiang.cn

[U35] Py：发送邮件
来源：http://ij.muxihuayi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bi.hahajie.cn

[U36] Py：定时任务
来源：http://pl.nicolike.cn

schedule.every(10).minutes.do(job)
来源：http://mw.521024.cn

[U37] Py：读写 Excel
来源：http://de.shxzskj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://py.wgjwhj.cn

[U38] Py：获取脚本所在目录
来源：http://be.521024.cn

Path(__file__).resolve().parent
来源：http://ym.wgjwhj.cn

[U39] Py：判断是否在交互环境
来源：http://gw.9csxet.cn

sys.stdout.isatty()
来源：http://rj.muxihuayi.cn

[U40] Py：打印到标准错误
来源：http://fn.muxihuayi.cn

print("err", file=sys.stderr)
来源：http://wm.shxzskj.cn

[U41] PHP：初始化 Composer 项目
来源：http://xl.muxihuayi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://hx.nicolike.cn

[U42] PHP：PSR-4 自动加载
来源：http://ov.jianghongdianzi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xj.chemitech.net.cn

[U43] PHP：声明命名空间
来源：http://ic.huanxung.cn

namespace App\Http;
来源：http://jr.colortex.cn

[U44] PHP：开启严格类型
来源：http://nu.muxihuayi.cn

declare(strict_types=1);
来源：http://kq.nszjky.cn

[U45] PHP：类型声明与返回类型
来源：http://mp.huanxung.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ud.bookmarksfly.cn

[U46] PHP：可空类型
来源：http://la.huixinmuqiang.cn

?string $name = null
来源：http://tc.hahajie.cn

[U47] PHP：联合类型
来源：http://cx.nszjky.cn

int|string $id
来源：http://oe.muxihuayi.cn

[U48] PHP：纯枚举
来源：http://vh.yuexingan06.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zo.bjjhwx.cn

[U49] PHP：只读属性
来源：http://na.wgjwhj.cn

public readonly string $name
来源：http://dv.hnjuh.cn

[U50] PHP：构造器属性提升
来源：http://tm.hahajie.cn

public function __construct(private int $id) {}
来源：http://iv.wgjwhj.cn

[U51] PHP：数组解构
来源：http://wq.nszjky.cn

[$a, $b] = $arr;
来源：http://hs.nicolike.cn

[U52] PHP：箭头函数
来源：http://vw.huixinmuqiang.cn

$double = fn($x) => $x * 2;
来源：http://ci.9csxet.cn

[U53] PHP：空合并运算符
来源：http://ga.panjiajie.cn

$v = $a ?? $b ?? "default";
来源：http://es.bjjhwx.cn

[U54] PHP：空安全调用
来源：http://pl.huixiangedu.cn

$obj?->method()
来源：http://ty.bookmarksfly.cn

[U55] PHP：match 表达式
来源：http://qr.haigaiapp.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://py.panjiajie.cn

[U56] PHP：命名参数
来源：http://yn.muxihuayi.cn

f(a: 1, b: 2)
来源：http://px.huanxung.cn

[U57] PHP：字符串插值
来源：http://wc.szsharing.cn

"值: {$a}"
来源：http://ri.bookmarksfly.cn

[U58] PHP：数组三件套
来源：http://ku.bookmarksfly.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cv.yuexingan06.cn

[U59] PHP：自定义排序
来源：http://ug.szsharing.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://km.bjjhwx.cn

[U60] PHP：JSON 编解码
来源：http://yc.szsharing.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pr.521024.cn

[U61] PHP：正则
来源：http://gs.shxzskj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qi.yuntaijiaju.cn

[U62] PHP：日期对象
来源：http://mu.521024.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bg.bookmarksfly.cn

[U63] PHP：文件读写
来源：http://cj.hahajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rv.jctech888.com.cn

[U64] PHP：目录遍历
来源：http://wp.gzmigu.cn

glob("dir/*.php");  scandir("dir");
来源：http://le.colortex.cn

[U65] PHP：会话
来源：http://bp.asd995.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ro.panjiajie.cn

[U66] PHP：设置 Cookie
来源：http://kx.gzmigu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kp.asd995.cn

[U67] PHP：处理文件上传
来源：http://rt.panjiajie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ey.chemitech.net.cn

[U68] PHP：PDO 连接
来源：http://sj.bookmarksfly.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nu.huixiangedu.cn

[U69] PHP：PDO 预处理
来源：http://me.muxihuayi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fm.gzmigu.cn

[U70] PHP：PDO 事务
来源：http://zf.newstarts.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tv.jctech888.com.cn

[U71] PHP：抛出异常
来源：http://vu.muxihuayi.cn

throw new RuntimeException("失败", 500);
来源：http://fl.huixinmuqiang.cn

[U72] PHP：写错误日志
来源：http://fq.jianghongdianzi.cn

error_log("失败: " . $e->getMessage());
来源：http://fc.szxytkj.cn

[U73] PHP：读取 ini 配置
来源：http://ka.haigaiapp.cn

parse_ini_file("config.ini", true)
来源：http://rp.yuntaijiaju.cn

[U74] PHP：读取环境变量
来源：http://rl.jianghongdianzi.cn

getenv("APP_ENV") ?: "production"
来源：http://ma.jianghongdianzi.cn

[U75] PHP：依赖注入
来源：http://zz.huixiangedu.cn

composer require psr/container
来源：http://rf.colortex.cn

[U76] PHP：简单路由
来源：http://ua.muxihuayi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ys.haigaiapp.cn

[U77] PHP：模板渲染
来源：http://ea.huanxung.cn

composer require twig/twig
来源：http://xl.szxytkj.cn

[U78] PHP：单元测试
来源：http://nn.lnxyls.cn

composer require --dev phpunit/phpunit
来源：http://sm.gzmigu.cn

[U79] PHP：静态分析
来源：http://rk.9csxet.cn

composer require --dev phpstan/phpstan
来源：http://kc.nicolike.cn

[U80] PHP：代码规范修复
来源：http://hg.bjjhwx.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://mv.huixiangedu.cn

[U81] JS：初始化项目
来源：http://cf.9csxet.cn

npm init -y;  npm i express
来源：http://or.shtwfgs.cn

[U82] JS：package.json 脚本
来源：http://yl.9csxet.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dc.hnjuh.cn

[U83] JS：ES Module 导入导出
来源：http://dd.nicolike.cn

export const a = 1;  import { a } from "./m.js";
来源：http://us.yuntaijiaju.cn

[U84] JS：CommonJS 写法
来源：http://qm.hnjuh.cn

module.exports = { a };  const { a } = require("./m");
来源：http://vt.gzmigu.cn

[U85] JS：可选链
来源：http://my.hahajie.cn

a?.b?.c
来源：http://xj.hnjuh.cn

[U86] JS：空值合并
来源：http://io.yuexingan06.cn

a ?? b
来源：http://yx.hahajie.cn

[U87] JS：解构默认值
来源：http://wq.lnxyls.cn

const { a = 1, b = 2 } = obj;
来源：http://sj.szsharing.cn

[U88] JS：对象展开合并
来源：http://je.shxzukj.cn

{ ...a, ...b }
来源：http://gm.colortex.cn

[U89] JS：数组去重
来源：http://dk.haigaiapp.cn

[...new Set(arr)]
来源：http://yj.haigaiapp.cn

[U90] JS：数字数组排序
来源：http://tz.jctech888.com.cn

[...arr].sort((a, b) => a - b)
来源：http://br.jianghongdianzi.cn

[U91] JS：对象键值遍历
来源：http://ib.huanxung.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ur.nicolike.cn

[U92] JS：深拷贝
来源：http://za.szsharing.cn

structuredClone(obj)
来源：http://gq.521024.cn


<!-- 参考信息 -->