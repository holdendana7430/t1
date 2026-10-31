代发 wailian999

[T03] Kotlin：字符串模板
来源：http://ts.gzmigu.cn

"值: $b"
来源：http://xx.huixinmuqiang.cn

[T04] Kotlin：空安全
来源：http://hl.shxzskj.cn

val n: String? = null;  n?.length
来源：http://vh.hnjuh.cn

[T05] Kotlin：when 表达式
来源：http://bw.shxzskj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bk.szsharing.cn

[T06] Kotlin：集合映射
来源：http://zr.gzmigu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ao.shtwfgs.cn

[T07] Kotlin：集合过滤
来源：http://ec.bjjhwx.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ri.9csxet.cn

[T08] Kotlin：数据类
来源：http://jc.colortex.cn

data class User(val name: String, val age: Int)
来源：http://mo.bookmarksfly.cn

[T09] Kotlin：扩展函数
来源：http://is.bjjhwx.cn

fun String.exclaim() = this + "!"
来源：http://qx.lnxyls.cn

[T10] Kotlin：默认参数
来源：http://tl.shxzukj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ah.nicolike.cn

[T11] Kotlin：协程
来源：http://cp.jctech888.com.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nu.yuntaijiaju.cn

[T12] Kotlin：解构声明
来源：http://ud.nszjky.cn

val (a, b) = Pair(1, 2)
来源：http://eu.szxytkj.cn

[T13] Kotlin：只读 Map
来源：http://uv.gzmigu.cn

val m = mapOf("a" to 1)
来源：http://om.panjiajie.cn

[T14] Kotlin：循环
来源：http://ck.szxytkj.cn

for (i in 1..10) println(i)
来源：http://lh.shxzskj.cn

[T15] Kotlin：接口
来源：http://as.huanxung.cn

interface Shape { fun area(): Double }
来源：http://bn.hnjuh.cn

[T16] Swift：Hello World
来源：http://oh.colortex.cn

print("Hello")
来源：http://il.hnjuh.cn

[T17] Swift：变量与常量
来源：http://ck.huanxung.cn

var a = 1;  let b = 2
来源：http://gn.panjiajie.cn

[T18] Swift：字符串插值
来源：http://il.lnxyls.cn

"值: \(b)"
来源：http://dz.colortex.cn

[T19] Swift：可选绑定
来源：http://hd.gzmigu.cn

if let n = opt { print(n) }
来源：http://it.wgjwhj.cn

[T20] Swift：数组操作
来源：http://mw.yuexingan06.cn

var a = [1, 2, 3];  a.append(4)
来源：http://wk.bookmarksfly.cn

[T21] Swift：遍历
来源：http://sl.wgjwhj.cn

for x in a { print(x) }
来源：http://zr.haigaiapp.cn

[T22] Swift：字典
来源：http://me.bjjhwx.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vz.lnxyls.cn

[T23] Swift：函数
来源：http://ta.jianghongdianzi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jm.hnjuh.cn

[T24] Swift：闭包
来源：http://xm.panjiajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vz.shtwfgs.cn

[T25] Swift：结构体
来源：http://mu.colortex.cn

struct P { var x: Int }
来源：http://ne.jianghongdianzi.cn

[T26] Swift：类与重写
来源：http://ze.shxzukj.cn

class A: Base { override func f() {} }
来源：http://vk.bjjhwx.cn

[T27] Swift：错误处理
来源：http://ih.yuntaijiaju.cn

do { try f() } catch { print(error) }
来源：http://hl.9csxet.cn

[T28] Swift：枚举
来源：http://sw.newstarts.cn

enum Color { case red, green }
来源：http://nn.muxihuayi.cn

[T29] Swift：guard 提前返回
来源：http://pe.shxzskj.cn

guard let x = opt else { return }
来源：http://lf.9csxet.cn

[T30] Swift：协议
来源：http://ep.shxzukj.cn

protocol Shape { func area() -> Double }
来源：http://br.bookmarksfly.cn

[T31] Lua：Hello World
来源：http://pb.lnxyls.cn

print("Hello")
来源：http://ct.colortex.cn

[T32] Lua：局部变量
来源：http://zw.shxzukj.cn

local a = 1
来源：http://tz.yuexingan06.cn

[T33] Lua：表（数组）
来源：http://rc.lnxyls.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hn.szxytkj.cn

[T34] Lua：遍历表
来源：http://mt.9csxet.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qh.yuexingan06.cn

[T35] Lua：字典表
来源：http://qh.lnxyls.cn

local d = { a = 1 };  d.b = 2
来源：http://ur.bjjhwx.cn

[T36] Lua：函数
来源：http://so.yuexingan06.cn

function add(a, b) return a + b end
来源：http://sl.yuexingan06.cn

[T37] Lua：字符串拼接
来源：http://ur.jctech888.com.cn

"a" .. "b"
来源：http://ew.yuntaijiaju.cn

[T38] Lua：条件
来源：http://gd.muxihuayi.cn

if x > 0 then print("正") end
来源：http://fn.szxytkj.cn

[T39] Lua：模式匹配
来源：http://ru.nicolike.cn

string.find(s, "%d+")
来源：http://jz.huixinmuqiang.cn

[T40] Lua：元表
来源：http://zt.9csxet.cn

setmetatable({}, { __index = base })
来源：http://gk.muxihuayi.cn

[T41] Perl：Hello World
来源：http://vd.bjjhwx.cn

print "Hello\n";
来源：http://ls.asd995.cn

[T42] Perl：变量类型
来源：http://hl.colortex.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sv.gzmigu.cn

[T43] Perl：字符串插值
来源：http://hv.9csxet.cn

"值: $a"
来源：http://xg.hnjuh.cn

[T44] Perl：条件
来源：http://rg.haigaiapp.cn

if ($a > 0) { print "正"; }
来源：http://kf.bookmarksfly.cn

[T45] Perl：数组遍历
来源：http://li.haigaiapp.cn

for my $x (@arr) { print $x; }
来源：http://va.huixinmuqiang.cn

[T46] Perl：哈希操作
来源：http://tp.jianghongdianzi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://yh.jianghongdianzi.cn

[T47] Perl：正则捕获
来源：http://kw.wgjwhj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://kc.szsharing.cn

[T48] Perl：正则替换
来源：http://pu.nszjky.cn

$s =~ s/old/new/g;
来源：http://il.bjjhwx.cn

[T49] Perl：函数
来源：http://rt.521024.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mi.panjiajie.cn

[T50] Perl：逐行读文件
来源：http://nu.nszjky.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://an.szxytkj.cn

while (my $line = <$fh>) { print $line; }
来源：http://vy.szsharing.cn

[T51] Scala：Hello World
来源：http://cj.bjjhwx.cn

println("Hello")
来源：http://df.wgjwhj.cn

[T52] Scala：变量
来源：http://mz.521024.cn

val a = 1;  var b = 2
来源：http://fc.9csxet.cn

[T53] Scala：字符串插值
来源：http://kr.muxihuayi.cn

s"值: $b"
来源：http://sk.panjiajie.cn

[T54] Scala：集合映射
来源：http://gt.bookmarksfly.cn

List(1, 2, 3).map(_ * 2)
来源：http://ws.bjjhwx.cn

[T55] Scala：集合过滤
来源：http://yc.haigaiapp.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ct.asd995.cn

[T56] Scala：样例类
来源：http://ds.yuexingan06.cn

case class User(name: String, age: Int)
来源：http://gz.jianghongdianzi.cn

[T57] Scala：模式匹配
来源：http://vx.muxihuayi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://bd.hahajie.cn

[T58] Scala：函数定义
来源：http://kw.chemitech.net.cn

def add(a: Int, b: Int): Int = a + b
来源：http://st.chemitech.net.cn

[T59] Scala：循环
来源：http://hp.9csxet.cn

for (i <- 1 to 10) println(i)
来源：http://gm.newstarts.cn

[T60] Scala：折叠
来源：http://mc.bjjhwx.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wh.huanxung.cn

================================================================================
来源：http://fs.newstarts.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jl.szsharing.cn

================================================================================
来源：http://ai.bookmarksfly.cn

[U01] Py：创建虚拟环境
来源：http://kl.9csxet.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mp.gzmigu.cn

[U02] Py：导出 / 安装依赖
来源：http://nc.shxzskj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://sf.szxytkj.cn

[U03] Py：加载 .env 配置
来源：http://st.newstarts.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://di.nszjky.cn

[U04] Py：变量调试打印
来源：http://oa.bjjhwx.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xm.lnxyls.cn

[U05] Py：列表去重且保序
来源：http://xj.newstarts.cn

list(dict.fromkeys(arr))
来源：http://ey.jctech888.com.cn

[U06] Py：合并两个字典
来源：http://as.lnxyls.cn

{**a, **b}
来源：http://qd.yuntaijiaju.cn

[U07] Py：反转字典键值
来源：http://bu.bookmarksfly.cn

{v: k for k, v in d.items()}
来源：http://ft.shtwfgs.cn

[U08] Py：展平二维列表
来源：http://bu.nicolike.cn

[y for x in nested for y in x]
来源：http://dr.newstarts.cn

[U09] Py：字典取最大值的键
来源：http://so.wgjwhj.cn

max(d, key=d.get)
来源：http://sp.huixinmuqiang.cn

[U10] Py：按值排序字典
来源：http://na.hnjuh.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vs.haigaiapp.cn

[U11] Py：生成器表达式
来源：http://jr.wgjwhj.cn

(x * 2 for x in arr)
来源：http://uj.muxihuayi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://oh.panjiajie.cn

Counter(arr).most_common(3)
来源：http://ne.huixinmuqiang.cn

[U13] Py：固定长度队列
来源：http://wu.huixinmuqiang.cn

deque(maxlen=10)
来源：http://ix.shtwfgs.cn

[U14] Py：分组收集到列表
来源：http://ky.chemitech.net.cn

defaultdict(list)
来源：http://jx.asd995.cn

[U15] Py：高精度计时
来源：http://ws.panjiajie.cn

t = time.perf_counter()
来源：http://ir.newstarts.cn

[U16] Py：命令行参数解析
来源：http://vx.hahajie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rx.bookmarksfly.cn

[U17] Py：初始化日志
来源：http://qk.szxytkj.cn

logging.basicConfig(level=logging.INFO)
来源：http://ct.wgjwhj.cn

[U18] Py：预编译正则
来源：http://ty.jianghongdianzi.cn

pat = re.compile(r"\d+")
来源：http://sx.jianghongdianzi.cn

[U19] Py：正则替换带回调
来源：http://yv.asd995.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xv.muxihuayi.cn

[U20] Py：缓存函数结果
来源：http://nf.huanxung.cn

@functools.lru_cache(maxsize=None)
来源：http://gn.nicolike.cn

[U21] Py：自定义上下文管理器
来源：http://wi.nszjky.cn

@contextlib.contextmanager
来源：http://bi.bjjhwx.cn

[U22] Py：矩阵转置
来源：http://ct.bjjhwx.cn

list(zip(*m))
来源：http://wo.bookmarksfly.cn

[U23] Py：分块读取大文件
来源：http://ap.bookmarksfly.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mt.521024.cn

[U24] Py：路径操作
来源：http://nb.colortex.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wg.haigaiapp.cn

[U25] Py：CSV 按字典读
来源：http://wv.newstarts.cn

csv.DictReader(f)
来源：http://lw.wgjwhj.cn

[U26] Py：并发下载
来源：http://vv.hnjuh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ld.9csxet.cn

[U27] Py：异步 HTTP
来源：http://wd.huanxung.cn

aiohttp.ClientSession() 配合 async with
来源：http://ms.huixinmuqiang.cn

[U28] Py：类型别名
来源：http://ra.szsharing.cn

UserId = int
来源：http://vb.yuexingan06.cn

[U29] Py：属性校验
来源：http://am.szxytkj.cn

@property 与 @x.setter 配合
来源：http://qy.asd995.cn

[U30] Py：数据类
来源：http://ds.huanxung.cn

@dataclass(slots=True)
来源：http://fj.muxihuayi.cn

[U31] Py：单测
来源：http://lf.521024.cn

python -m pytest -q
来源：http://jd.bookmarksfly.cn

[U32] Py：代码格式化
来源：http://wt.szxytkj.cn

ruff format . && ruff check --fix .
来源：http://vm.huanxung.cn

[U33] Py：打包发布
来源：http://mf.chemitech.net.cn

python -m build  （依赖 pyproject.toml）
来源：http://pd.asd995.cn

[U34] Py：判断编码
来源：http://us.huixinmuqiang.cn

chardet.detect(raw)
来源：http://dj.muxihuayi.cn

[U35] Py：发送邮件
来源：http://oi.shxzukj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dt.chemitech.net.cn

[U36] Py：定时任务
来源：http://bi.asd995.cn

schedule.every(10).minutes.do(job)
来源：http://ud.bookmarksfly.cn

[U37] Py：读写 Excel
来源：http://lz.huixinmuqiang.cn

pandas.read_excel / DataFrame.to_excel
来源：http://at.huixinmuqiang.cn

[U38] Py：获取脚本所在目录
来源：http://yk.szsharing.cn

Path(__file__).resolve().parent
来源：http://zz.newstarts.cn

[U39] Py：判断是否在交互环境
来源：http://tu.chemitech.net.cn

sys.stdout.isatty()
来源：http://kf.shtwfgs.cn

[U40] Py：打印到标准错误
来源：http://rw.huixinmuqiang.cn

print("err", file=sys.stderr)
来源：http://zw.521024.cn

[U41] PHP：初始化 Composer 项目
来源：http://hk.huixiangedu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://bo.lnxyls.cn

[U42] PHP：PSR-4 自动加载
来源：http://ps.asd995.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vr.haigaiapp.cn

[U43] PHP：声明命名空间
来源：http://sm.9csxet.cn

namespace App\Http;
来源：http://vy.nszjky.cn

[U44] PHP：开启严格类型
来源：http://qa.nicolike.cn

declare(strict_types=1);
来源：http://wj.szsharing.cn

[U45] PHP：类型声明与返回类型
来源：http://yi.shtwfgs.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://vx.szxytkj.cn

[U46] PHP：可空类型
来源：http://hn.jianghongdianzi.cn

?string $name = null
来源：http://nz.gzmigu.cn

[U47] PHP：联合类型
来源：http://ch.gzmigu.cn

int|string $id
来源：http://mj.hnjuh.cn

[U48] PHP：纯枚举
来源：http://ay.huixiangedu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ss.lnxyls.cn

[U49] PHP：只读属性
来源：http://xw.colortex.cn

public readonly string $name
来源：http://tx.haigaiapp.cn

[U50] PHP：构造器属性提升
来源：http://ja.9csxet.cn

public function __construct(private int $id) {}
来源：http://lw.521024.cn

[U51] PHP：数组解构
来源：http://fd.huixiangedu.cn

[$a, $b] = $arr;
来源：http://wf.jctech888.com.cn

[U52] PHP：箭头函数
来源：http://tb.newstarts.cn

$double = fn($x) => $x * 2;
来源：http://fy.jianghongdianzi.cn

[U53] PHP：空合并运算符
来源：http://av.shtwfgs.cn

$v = $a ?? $b ?? "default";
来源：http://on.hnjuh.cn

[U54] PHP：空安全调用
来源：http://kt.shxzukj.cn

$obj?->method()
来源：http://qy.bookmarksfly.cn

[U55] PHP：match 表达式
来源：http://em.huixinmuqiang.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uo.hahajie.cn

[U56] PHP：命名参数
来源：http://ka.haigaiapp.cn

f(a: 1, b: 2)
来源：http://pp.hahajie.cn

[U57] PHP：字符串插值
来源：http://bs.nicolike.cn

"值: {$a}"
来源：http://vv.jctech888.com.cn

[U58] PHP：数组三件套
来源：http://vf.jctech888.com.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xk.nicolike.cn

[U59] PHP：自定义排序
来源：http://vt.9csxet.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nj.9csxet.cn

[U60] PHP：JSON 编解码
来源：http://iz.bookmarksfly.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gf.9csxet.cn

[U61] PHP：正则
来源：http://jf.panjiajie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bq.szsharing.cn

[U62] PHP：日期对象
来源：http://qu.shtwfgs.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ra.yuntaijiaju.cn

[U63] PHP：文件读写
来源：http://rf.chemitech.net.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tc.huixinmuqiang.cn

[U64] PHP：目录遍历
来源：http://qo.bjjhwx.cn

glob("dir/*.php");  scandir("dir");
来源：http://uy.bookmarksfly.cn

[U65] PHP：会话
来源：http://rm.bookmarksfly.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://zh.huixinmuqiang.cn

[U66] PHP：设置 Cookie
来源：http://nq.jianghongdianzi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jv.hahajie.cn

[U67] PHP：处理文件上传
来源：http://wk.gzmigu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rd.newstarts.cn

[U68] PHP：PDO 连接
来源：http://zt.hnjuh.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lg.bjjhwx.cn

[U69] PHP：PDO 预处理
来源：http://jg.shxzskj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://it.huixiangedu.cn

[U70] PHP：PDO 事务
来源：http://nh.haigaiapp.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vp.muxihuayi.cn

[U71] PHP：抛出异常
来源：http://dk.gzmigu.cn

throw new RuntimeException("失败", 500);
来源：http://gj.colortex.cn

[U72] PHP：写错误日志
来源：http://ar.yuexingan06.cn

error_log("失败: " . $e->getMessage());
来源：http://ib.szxytkj.cn

[U73] PHP：读取 ini 配置
来源：http://tb.9csxet.cn

parse_ini_file("config.ini", true)
来源：http://ow.huanxung.cn

[U74] PHP：读取环境变量
来源：http://yh.shxzukj.cn

getenv("APP_ENV") ?: "production"
来源：http://vs.bjjhwx.cn

[U75] PHP：依赖注入
来源：http://vt.colortex.cn

composer require psr/container
来源：http://rd.huanxung.cn

[U76] PHP：简单路由
来源：http://xu.shxzskj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jf.huixiangedu.cn

[U77] PHP：模板渲染
来源：http://eh.muxihuayi.cn

composer require twig/twig
来源：http://jv.yuexingan06.cn

[U78] PHP：单元测试
来源：http://ah.521024.cn

composer require --dev phpunit/phpunit
来源：http://qh.szxytkj.cn

[U79] PHP：静态分析
来源：http://rf.hnjuh.cn

composer require --dev phpstan/phpstan
来源：http://jf.nicolike.cn

[U80] PHP：代码规范修复
来源：http://es.shtwfgs.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ls.hahajie.cn

[U81] JS：初始化项目
来源：http://gc.colortex.cn

npm init -y;  npm i express
来源：http://ns.asd995.cn

[U82] JS：package.json 脚本
来源：http://ff.colortex.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mj.huanxung.cn

[U83] JS：ES Module 导入导出
来源：http://bf.szsharing.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qc.shxzskj.cn

[U84] JS：CommonJS 写法
来源：http://nu.haigaiapp.cn

module.exports = { a };  const { a } = require("./m");
来源：http://qh.newstarts.cn

[U85] JS：可选链
来源：http://ad.wgjwhj.cn

a?.b?.c
来源：http://hy.panjiajie.cn

[U86] JS：空值合并
来源：http://zp.szsharing.cn

a ?? b
来源：http://ll.panjiajie.cn

[U87] JS：解构默认值
来源：http://ui.hahajie.cn

const { a = 1, b = 2 } = obj;
来源：http://qn.gzmigu.cn

[U88] JS：对象展开合并
来源：http://bo.gzmigu.cn

{ ...a, ...b }
来源：http://po.hahajie.cn

[U89] JS：数组去重
来源：http://mh.shxzukj.cn

[...new Set(arr)]
来源：http://ly.huixinmuqiang.cn

[U90] JS：数字数组排序
来源：http://rs.gzmigu.cn

[...arr].sort((a, b) => a - b)
来源：http://ib.hnjuh.cn


<!-- 参考信息 -->