代发 wailian999

[T05] Kotlin：when 表达式
来源：http://te.panjiajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rx.wgjwhj.cn

[T06] Kotlin：集合映射
来源：http://bc.nszjky.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hd.chemitech.net.cn

[T07] Kotlin：集合过滤
来源：http://kp.hahajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://dm.huixiangedu.cn

[T08] Kotlin：数据类
来源：http://sk.nszjky.cn

data class User(val name: String, val age: Int)
来源：http://tv.huanxung.cn

[T09] Kotlin：扩展函数
来源：http://zo.521024.cn

fun String.exclaim() = this + "!"
来源：http://ht.haigaiapp.cn

[T10] Kotlin：默认参数
来源：http://rp.huixiangedu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tm.bookmarksfly.cn

[T11] Kotlin：协程
来源：http://fv.shtwfgs.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://dr.jianghongdianzi.cn

[T12] Kotlin：解构声明
来源：http://rq.huixiangedu.cn

val (a, b) = Pair(1, 2)
来源：http://xi.jctech888.com.cn

[T13] Kotlin：只读 Map
来源：http://jd.bookmarksfly.cn

val m = mapOf("a" to 1)
来源：http://nv.colortex.cn

[T14] Kotlin：循环
来源：http://sx.bjjhwx.cn

for (i in 1..10) println(i)
来源：http://ti.lnxyls.cn

[T15] Kotlin：接口
来源：http://au.panjiajie.cn

interface Shape { fun area(): Double }
来源：http://pk.chemitech.net.cn

[T16] Swift：Hello World
来源：http://zs.muxihuayi.cn

print("Hello")
来源：http://do.bookmarksfly.cn

[T17] Swift：变量与常量
来源：http://pv.hnjuh.cn

var a = 1;  let b = 2
来源：http://lh.jctech888.com.cn

[T18] Swift：字符串插值
来源：http://tz.huixinmuqiang.cn

"值: \(b)"
来源：http://bh.bjjhwx.cn

[T19] Swift：可选绑定
来源：http://wa.shxzskj.cn

if let n = opt { print(n) }
来源：http://bq.yuexingan06.cn

[T20] Swift：数组操作
来源：http://dl.shtwfgs.cn

var a = [1, 2, 3];  a.append(4)
来源：http://pw.colortex.cn

[T21] Swift：遍历
来源：http://eg.colortex.cn

for x in a { print(x) }
来源：http://ru.nszjky.cn

[T22] Swift：字典
来源：http://ry.bjjhwx.cn

var d = ["a": 1];  d["b"] = 2
来源：http://do.shtwfgs.cn

[T23] Swift：函数
来源：http://qv.huanxung.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yp.huanxung.cn

[T24] Swift：闭包
来源：http://nk.shxzukj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://uq.jctech888.com.cn

[T25] Swift：结构体
来源：http://sr.shtwfgs.cn

struct P { var x: Int }
来源：http://jp.newstarts.cn

[T26] Swift：类与重写
来源：http://tg.muxihuayi.cn

class A: Base { override func f() {} }
来源：http://md.yuexingan06.cn

[T27] Swift：错误处理
来源：http://yh.chemitech.net.cn

do { try f() } catch { print(error) }
来源：http://du.szsharing.cn

[T28] Swift：枚举
来源：http://qo.shxzukj.cn

enum Color { case red, green }
来源：http://hk.521024.cn

[T29] Swift：guard 提前返回
来源：http://hj.szsharing.cn

guard let x = opt else { return }
来源：http://nf.wgjwhj.cn

[T30] Swift：协议
来源：http://ac.gzmigu.cn

protocol Shape { func area() -> Double }
来源：http://cd.szxytkj.cn

[T31] Lua：Hello World
来源：http://hh.hahajie.cn

print("Hello")
来源：http://ii.newstarts.cn

[T32] Lua：局部变量
来源：http://du.521024.cn

local a = 1
来源：http://ly.gzmigu.cn

[T33] Lua：表（数组）
来源：http://ll.lnxyls.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://rc.bookmarksfly.cn

[T34] Lua：遍历表
来源：http://hx.yuntaijiaju.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vq.shxzukj.cn

[T35] Lua：字典表
来源：http://nh.muxihuayi.cn

local d = { a = 1 };  d.b = 2
来源：http://ne.huixinmuqiang.cn

[T36] Lua：函数
来源：http://my.jianghongdianzi.cn

function add(a, b) return a + b end
来源：http://yz.szxytkj.cn

[T37] Lua：字符串拼接
来源：http://gv.bookmarksfly.cn

"a" .. "b"
来源：http://oj.lnxyls.cn

[T38] Lua：条件
来源：http://bu.gzmigu.cn

if x > 0 then print("正") end
来源：http://vj.chemitech.net.cn

[T39] Lua：模式匹配
来源：http://kk.szxytkj.cn

string.find(s, "%d+")
来源：http://iq.nicolike.cn

[T40] Lua：元表
来源：http://as.huanxung.cn

setmetatable({}, { __index = base })
来源：http://bw.hahajie.cn

[T41] Perl：Hello World
来源：http://ok.shxzskj.cn

print "Hello\n";
来源：http://lr.colortex.cn

[T42] Perl：变量类型
来源：http://il.521024.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ss.shxzukj.cn

[T43] Perl：字符串插值
来源：http://ce.bjjhwx.cn

"值: $a"
来源：http://or.newstarts.cn

[T44] Perl：条件
来源：http://mw.haigaiapp.cn

if ($a > 0) { print "正"; }
来源：http://sa.szxytkj.cn

[T45] Perl：数组遍历
来源：http://xv.bookmarksfly.cn

for my $x (@arr) { print $x; }
来源：http://iz.gzmigu.cn

[T46] Perl：哈希操作
来源：http://ax.bookmarksfly.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://di.bjjhwx.cn

[T47] Perl：正则捕获
来源：http://xz.huixinmuqiang.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://zh.yuexingan06.cn

[T48] Perl：正则替换
来源：http://hl.huixiangedu.cn

$s =~ s/old/new/g;
来源：http://jk.hahajie.cn

[T49] Perl：函数
来源：http://kf.gzmigu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zr.yuexingan06.cn

[T50] Perl：逐行读文件
来源：http://nb.hnjuh.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://mp.yuexingan06.cn

while (my $line = <$fh>) { print $line; }
来源：http://tv.bjjhwx.cn

[T51] Scala：Hello World
来源：http://fn.521024.cn

println("Hello")
来源：http://qq.wgjwhj.cn

[T52] Scala：变量
来源：http://vh.hahajie.cn

val a = 1;  var b = 2
来源：http://la.newstarts.cn

[T53] Scala：字符串插值
来源：http://la.521024.cn

s"值: $b"
来源：http://ai.szxytkj.cn

[T54] Scala：集合映射
来源：http://av.huixiangedu.cn

List(1, 2, 3).map(_ * 2)
来源：http://qq.shxzskj.cn

[T55] Scala：集合过滤
来源：http://sf.newstarts.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xj.nicolike.cn

[T56] Scala：样例类
来源：http://xv.chemitech.net.cn

case class User(name: String, age: Int)
来源：http://sj.asd995.cn

[T57] Scala：模式匹配
来源：http://vz.shxzukj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://lp.szsharing.cn

[T58] Scala：函数定义
来源：http://kp.bookmarksfly.cn

def add(a: Int, b: Int): Int = a + b
来源：http://iy.bjjhwx.cn

[T59] Scala：循环
来源：http://vx.colortex.cn

for (i <- 1 to 10) println(i)
来源：http://tp.yuexingan06.cn

[T60] Scala：折叠
来源：http://yo.asd995.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xw.huanxung.cn

================================================================================
来源：http://yw.bjjhwx.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ll.panjiajie.cn

================================================================================
来源：http://zf.chemitech.net.cn

[U01] Py：创建虚拟环境
来源：http://eb.bjjhwx.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cl.shxzskj.cn

[U02] Py：导出 / 安装依赖
来源：http://ar.jianghongdianzi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gq.colortex.cn

[U03] Py：加载 .env 配置
来源：http://nn.huixiangedu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://bk.shtwfgs.cn

[U04] Py：变量调试打印
来源：http://mi.521024.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bd.lnxyls.cn

[U05] Py：列表去重且保序
来源：http://hy.chemitech.net.cn

list(dict.fromkeys(arr))
来源：http://hy.hahajie.cn

[U06] Py：合并两个字典
来源：http://aw.shtwfgs.cn

{**a, **b}
来源：http://dk.panjiajie.cn

[U07] Py：反转字典键值
来源：http://ig.yuexingan06.cn

{v: k for k, v in d.items()}
来源：http://gk.muxihuayi.cn

[U08] Py：展平二维列表
来源：http://ys.nszjky.cn

[y for x in nested for y in x]
来源：http://zl.hahajie.cn

[U09] Py：字典取最大值的键
来源：http://hy.nszjky.cn

max(d, key=d.get)
来源：http://nm.shxzukj.cn

[U10] Py：按值排序字典
来源：http://hc.huixinmuqiang.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vb.yuntaijiaju.cn

[U11] Py：生成器表达式
来源：http://tf.haigaiapp.cn

(x * 2 for x in arr)
来源：http://mu.wgjwhj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://jz.muxihuayi.cn

Counter(arr).most_common(3)
来源：http://wp.panjiajie.cn

[U13] Py：固定长度队列
来源：http://kn.shtwfgs.cn

deque(maxlen=10)
来源：http://oa.shxzukj.cn

[U14] Py：分组收集到列表
来源：http://ou.shxzukj.cn

defaultdict(list)
来源：http://xk.colortex.cn

[U15] Py：高精度计时
来源：http://to.newstarts.cn

t = time.perf_counter()
来源：http://ge.shxzukj.cn

[U16] Py：命令行参数解析
来源：http://ix.huanxung.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ma.newstarts.cn

[U17] Py：初始化日志
来源：http://yq.yuexingan06.cn

logging.basicConfig(level=logging.INFO)
来源：http://og.muxihuayi.cn

[U18] Py：预编译正则
来源：http://qt.nszjky.cn

pat = re.compile(r"\d+")
来源：http://cr.haigaiapp.cn

[U19] Py：正则替换带回调
来源：http://rb.szsharing.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sy.huixinmuqiang.cn

[U20] Py：缓存函数结果
来源：http://tb.szxytkj.cn

@functools.lru_cache(maxsize=None)
来源：http://of.muxihuayi.cn

[U21] Py：自定义上下文管理器
来源：http://ax.bjjhwx.cn

@contextlib.contextmanager
来源：http://pt.huanxung.cn

[U22] Py：矩阵转置
来源：http://to.huanxung.cn

list(zip(*m))
来源：http://dr.szxytkj.cn

[U23] Py：分块读取大文件
来源：http://to.yuntaijiaju.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://em.521024.cn

[U24] Py：路径操作
来源：http://uo.muxihuayi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fk.shtwfgs.cn

[U25] Py：CSV 按字典读
来源：http://of.jianghongdianzi.cn

csv.DictReader(f)
来源：http://bk.9csxet.cn

[U26] Py：并发下载
来源：http://bt.hnjuh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cy.szxytkj.cn

[U27] Py：异步 HTTP
来源：http://tu.bookmarksfly.cn

aiohttp.ClientSession() 配合 async with
来源：http://ic.shxzskj.cn

[U28] Py：类型别名
来源：http://sy.huanxung.cn

UserId = int
来源：http://zw.521024.cn

[U29] Py：属性校验
来源：http://kt.nicolike.cn

@property 与 @x.setter 配合
来源：http://aw.gzmigu.cn

[U30] Py：数据类
来源：http://sz.colortex.cn

@dataclass(slots=True)
来源：http://no.szsharing.cn

[U31] Py：单测
来源：http://hn.wgjwhj.cn

python -m pytest -q
来源：http://fu.nszjky.cn

[U32] Py：代码格式化
来源：http://hc.bookmarksfly.cn

ruff format . && ruff check --fix .
来源：http://si.muxihuayi.cn

[U33] Py：打包发布
来源：http://vi.wgjwhj.cn

python -m build  （依赖 pyproject.toml）
来源：http://nv.jianghongdianzi.cn

[U34] Py：判断编码
来源：http://bx.jianghongdianzi.cn

chardet.detect(raw)
来源：http://ot.yuexingan06.cn

[U35] Py：发送邮件
来源：http://tq.bjjhwx.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fv.jctech888.com.cn

[U36] Py：定时任务
来源：http://ab.chemitech.net.cn

schedule.every(10).minutes.do(job)
来源：http://px.colortex.cn

[U37] Py：读写 Excel
来源：http://dc.szsharing.cn

pandas.read_excel / DataFrame.to_excel
来源：http://px.yuntaijiaju.cn

[U38] Py：获取脚本所在目录
来源：http://eq.newstarts.cn

Path(__file__).resolve().parent
来源：http://nr.nicolike.cn

[U39] Py：判断是否在交互环境
来源：http://fr.gzmigu.cn

sys.stdout.isatty()
来源：http://ne.colortex.cn

[U40] Py：打印到标准错误
来源：http://nn.yuntaijiaju.cn

print("err", file=sys.stderr)
来源：http://aq.shtwfgs.cn

[U41] PHP：初始化 Composer 项目
来源：http://hr.yuexingan06.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xk.huanxung.cn

[U42] PHP：PSR-4 自动加载
来源：http://yh.jctech888.com.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zu.chemitech.net.cn

[U43] PHP：声明命名空间
来源：http://te.jianghongdianzi.cn

namespace App\Http;
来源：http://tn.newstarts.cn

[U44] PHP：开启严格类型
来源：http://dt.hahajie.cn

declare(strict_types=1);
来源：http://un.huixiangedu.cn

[U45] PHP：类型声明与返回类型
来源：http://jk.chemitech.net.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://se.bjjhwx.cn

[U46] PHP：可空类型
来源：http://hb.yuexingan06.cn

?string $name = null
来源：http://xc.521024.cn

[U47] PHP：联合类型
来源：http://jo.521024.cn

int|string $id
来源：http://eo.muxihuayi.cn

[U48] PHP：纯枚举
来源：http://en.newstarts.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ek.bookmarksfly.cn

[U49] PHP：只读属性
来源：http://ok.asd995.cn

public readonly string $name
来源：http://lt.haigaiapp.cn

[U50] PHP：构造器属性提升
来源：http://cp.haigaiapp.cn

public function __construct(private int $id) {}
来源：http://ke.nicolike.cn

[U51] PHP：数组解构
来源：http://ix.haigaiapp.cn

[$a, $b] = $arr;
来源：http://lr.shxzskj.cn

[U52] PHP：箭头函数
来源：http://jv.huixiangedu.cn

$double = fn($x) => $x * 2;
来源：http://kz.hnjuh.cn

[U53] PHP：空合并运算符
来源：http://sr.shxzskj.cn

$v = $a ?? $b ?? "default";
来源：http://ud.haigaiapp.cn

[U54] PHP：空安全调用
来源：http://ib.huixiangedu.cn

$obj?->method()
来源：http://sc.lnxyls.cn

[U55] PHP：match 表达式
来源：http://oy.yuntaijiaju.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ig.lnxyls.cn

[U56] PHP：命名参数
来源：http://pg.hnjuh.cn

f(a: 1, b: 2)
来源：http://mu.hnjuh.cn

[U57] PHP：字符串插值
来源：http://ny.muxihuayi.cn

"值: {$a}"
来源：http://vn.gzmigu.cn

[U58] PHP：数组三件套
来源：http://qf.nszjky.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qi.9csxet.cn

[U59] PHP：自定义排序
来源：http://hu.colortex.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://go.nszjky.cn

[U60] PHP：JSON 编解码
来源：http://jr.panjiajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jk.muxihuayi.cn

[U61] PHP：正则
来源：http://qo.gzmigu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pg.chemitech.net.cn

[U62] PHP：日期对象
来源：http://sq.huixinmuqiang.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bt.huixiangedu.cn

[U63] PHP：文件读写
来源：http://ki.chemitech.net.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lp.shxzskj.cn

[U64] PHP：目录遍历
来源：http://kp.bjjhwx.cn

glob("dir/*.php");  scandir("dir");
来源：http://ik.hahajie.cn

[U65] PHP：会话
来源：http://ys.shxzskj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://fe.newstarts.cn

[U66] PHP：设置 Cookie
来源：http://qu.wgjwhj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mi.jianghongdianzi.cn

[U67] PHP：处理文件上传
来源：http://ms.jianghongdianzi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cs.bjjhwx.cn

[U68] PHP：PDO 连接
来源：http://qg.huixinmuqiang.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kc.yuexingan06.cn

[U69] PHP：PDO 预处理
来源：http://xc.hahajie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rl.9csxet.cn

[U70] PHP：PDO 事务
来源：http://ez.521024.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hb.hahajie.cn

[U71] PHP：抛出异常
来源：http://jv.521024.cn

throw new RuntimeException("失败", 500);
来源：http://kg.huanxung.cn

[U72] PHP：写错误日志
来源：http://md.newstarts.cn

error_log("失败: " . $e->getMessage());
来源：http://ks.huixinmuqiang.cn

[U73] PHP：读取 ini 配置
来源：http://db.bookmarksfly.cn

parse_ini_file("config.ini", true)
来源：http://vz.9csxet.cn

[U74] PHP：读取环境变量
来源：http://qn.shxzukj.cn

getenv("APP_ENV") ?: "production"
来源：http://ao.yuntaijiaju.cn

[U75] PHP：依赖注入
来源：http://db.yuexingan06.cn

composer require psr/container
来源：http://vr.nicolike.cn

[U76] PHP：简单路由
来源：http://mk.colortex.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xc.bjjhwx.cn

[U77] PHP：模板渲染
来源：http://ij.gzmigu.cn

composer require twig/twig
来源：http://kj.jctech888.com.cn

[U78] PHP：单元测试
来源：http://dt.szsharing.cn

composer require --dev phpunit/phpunit
来源：http://ke.hahajie.cn

[U79] PHP：静态分析
来源：http://fc.muxihuayi.cn

composer require --dev phpstan/phpstan
来源：http://wd.bjjhwx.cn

[U80] PHP：代码规范修复
来源：http://rz.chemitech.net.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ny.huanxung.cn

[U81] JS：初始化项目
来源：http://wl.lnxyls.cn

npm init -y;  npm i express
来源：http://db.9csxet.cn

[U82] JS：package.json 脚本
来源：http://ob.huanxung.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sz.panjiajie.cn

[U83] JS：ES Module 导入导出
来源：http://xp.gzmigu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://dc.asd995.cn

[U84] JS：CommonJS 写法
来源：http://pa.hahajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://bn.szsharing.cn

[U85] JS：可选链
来源：http://gq.hnjuh.cn

a?.b?.c
来源：http://eb.shtwfgs.cn

[U86] JS：空值合并
来源：http://ze.szxytkj.cn

a ?? b
来源：http://vc.szsharing.cn

[U87] JS：解构默认值
来源：http://su.9csxet.cn

const { a = 1, b = 2 } = obj;
来源：http://gq.yuntaijiaju.cn

[U88] JS：对象展开合并
来源：http://wq.chemitech.net.cn

{ ...a, ...b }
来源：http://zm.9csxet.cn

[U89] JS：数组去重
来源：http://lh.asd995.cn

[...new Set(arr)]
来源：http://xp.chemitech.net.cn

[U90] JS：数字数组排序
来源：http://hi.521024.cn

[...arr].sort((a, b) => a - b)
来源：http://ak.shtwfgs.cn

[U91] JS：对象键值遍历
来源：http://wu.muxihuayi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vg.nicolike.cn

[U92] JS：深拷贝
来源：http://lo.jctech888.com.cn

structuredClone(obj)
来源：http://pc.jianghongdianzi.cn


<!-- 参考信息 -->