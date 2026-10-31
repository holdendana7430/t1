代发 wailian999

[T01] Kotlin：Hello World
来源：http://wf.bjjhwx.cn

println("Hello")
来源：http://xf.szxytkj.cn

[T02] Kotlin：变量
来源：http://hk.jianghongdianzi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nn.huixiangedu.cn

[T03] Kotlin：字符串模板
来源：http://xi.jianghongdianzi.cn

"值: $b"
来源：http://nv.hnjuh.cn

[T04] Kotlin：空安全
来源：http://ii.colortex.cn

val n: String? = null;  n?.length
来源：http://wo.yuntaijiaju.cn

[T05] Kotlin：when 表达式
来源：http://vv.jianghongdianzi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wf.szxytkj.cn

[T06] Kotlin：集合映射
来源：http://ya.muxihuayi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://qb.nszjky.cn

[T07] Kotlin：集合过滤
来源：http://ck.chemitech.net.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://hi.nicolike.cn

[T08] Kotlin：数据类
来源：http://go.wgjwhj.cn

data class User(val name: String, val age: Int)
来源：http://gr.nicolike.cn

[T09] Kotlin：扩展函数
来源：http://wj.shxzskj.cn

fun String.exclaim() = this + "!"
来源：http://cj.yuntaijiaju.cn

[T10] Kotlin：默认参数
来源：http://xc.9csxet.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rq.jianghongdianzi.cn

[T11] Kotlin：协程
来源：http://pb.yuntaijiaju.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://mu.nszjky.cn

[T12] Kotlin：解构声明
来源：http://de.yuexingan06.cn

val (a, b) = Pair(1, 2)
来源：http://ag.nicolike.cn

[T13] Kotlin：只读 Map
来源：http://bp.gzmigu.cn

val m = mapOf("a" to 1)
来源：http://mw.chemitech.net.cn

[T14] Kotlin：循环
来源：http://kt.huixinmuqiang.cn

for (i in 1..10) println(i)
来源：http://mi.newstarts.cn

[T15] Kotlin：接口
来源：http://yh.hnjuh.cn

interface Shape { fun area(): Double }
来源：http://rh.9csxet.cn

[T16] Swift：Hello World
来源：http://vb.bookmarksfly.cn

print("Hello")
来源：http://zj.panjiajie.cn

[T17] Swift：变量与常量
来源：http://be.haigaiapp.cn

var a = 1;  let b = 2
来源：http://us.newstarts.cn

[T18] Swift：字符串插值
来源：http://xi.huixinmuqiang.cn

"值: \(b)"
来源：http://qy.nicolike.cn

[T19] Swift：可选绑定
来源：http://mt.shtwfgs.cn

if let n = opt { print(n) }
来源：http://fb.hnjuh.cn

[T20] Swift：数组操作
来源：http://pp.huanxung.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jn.shxzukj.cn

[T21] Swift：遍历
来源：http://hs.jianghongdianzi.cn

for x in a { print(x) }
来源：http://mh.9csxet.cn

[T22] Swift：字典
来源：http://uy.shxzskj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://hf.nszjky.cn

[T23] Swift：函数
来源：http://ow.yuexingan06.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ix.colortex.cn

[T24] Swift：闭包
来源：http://xc.huanxung.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ht.yuexingan06.cn

[T25] Swift：结构体
来源：http://bx.9csxet.cn

struct P { var x: Int }
来源：http://ba.hahajie.cn

[T26] Swift：类与重写
来源：http://xg.9csxet.cn

class A: Base { override func f() {} }
来源：http://mn.huixiangedu.cn

[T27] Swift：错误处理
来源：http://ib.wgjwhj.cn

do { try f() } catch { print(error) }
来源：http://ot.muxihuayi.cn

[T28] Swift：枚举
来源：http://bg.panjiajie.cn

enum Color { case red, green }
来源：http://ww.gzmigu.cn

[T29] Swift：guard 提前返回
来源：http://jc.hahajie.cn

guard let x = opt else { return }
来源：http://gd.chemitech.net.cn

[T30] Swift：协议
来源：http://ir.yuntaijiaju.cn

protocol Shape { func area() -> Double }
来源：http://lk.muxihuayi.cn

[T31] Lua：Hello World
来源：http://zs.shtwfgs.cn

print("Hello")
来源：http://kb.yuexingan06.cn

[T32] Lua：局部变量
来源：http://wq.yuexingan06.cn

local a = 1
来源：http://bs.yuntaijiaju.cn

[T33] Lua：表（数组）
来源：http://tx.chemitech.net.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xc.shtwfgs.cn

[T34] Lua：遍历表
来源：http://jj.wgjwhj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://hk.szsharing.cn

[T35] Lua：字典表
来源：http://ay.muxihuayi.cn

local d = { a = 1 };  d.b = 2
来源：http://vh.jianghongdianzi.cn

[T36] Lua：函数
来源：http://cj.jctech888.com.cn

function add(a, b) return a + b end
来源：http://ly.haigaiapp.cn

[T37] Lua：字符串拼接
来源：http://lt.521024.cn

"a" .. "b"
来源：http://si.jctech888.com.cn

[T38] Lua：条件
来源：http://cd.lnxyls.cn

if x > 0 then print("正") end
来源：http://wv.jctech888.com.cn

[T39] Lua：模式匹配
来源：http://ps.szsharing.cn

string.find(s, "%d+")
来源：http://bw.nicolike.cn

[T40] Lua：元表
来源：http://tf.newstarts.cn

setmetatable({}, { __index = base })
来源：http://ks.szxytkj.cn

[T41] Perl：Hello World
来源：http://ax.muxihuayi.cn

print "Hello\n";
来源：http://tb.newstarts.cn

[T42] Perl：变量类型
来源：http://ma.colortex.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vr.9csxet.cn

[T43] Perl：字符串插值
来源：http://ht.asd995.cn

"值: $a"
来源：http://yl.panjiajie.cn

[T44] Perl：条件
来源：http://yz.jctech888.com.cn

if ($a > 0) { print "正"; }
来源：http://cn.szsharing.cn

[T45] Perl：数组遍历
来源：http://zp.huixinmuqiang.cn

for my $x (@arr) { print $x; }
来源：http://dd.shxzukj.cn

[T46] Perl：哈希操作
来源：http://ct.jianghongdianzi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nf.shtwfgs.cn

[T47] Perl：正则捕获
来源：http://vr.wgjwhj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ym.9csxet.cn

[T48] Perl：正则替换
来源：http://za.huixinmuqiang.cn

$s =~ s/old/new/g;
来源：http://ca.yuexingan06.cn

[T49] Perl：函数
来源：http://pk.wgjwhj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qi.bjjhwx.cn

[T50] Perl：逐行读文件
来源：http://bo.wgjwhj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xf.newstarts.cn

while (my $line = <$fh>) { print $line; }
来源：http://il.nszjky.cn

[T51] Scala：Hello World
来源：http://yq.nicolike.cn

println("Hello")
来源：http://li.panjiajie.cn

[T52] Scala：变量
来源：http://oy.hahajie.cn

val a = 1;  var b = 2
来源：http://nw.jianghongdianzi.cn

[T53] Scala：字符串插值
来源：http://jr.bookmarksfly.cn

s"值: $b"
来源：http://ss.nszjky.cn

[T54] Scala：集合映射
来源：http://ni.yuexingan06.cn

List(1, 2, 3).map(_ * 2)
来源：http://oq.huanxung.cn

[T55] Scala：集合过滤
来源：http://ko.jctech888.com.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wk.lnxyls.cn

[T56] Scala：样例类
来源：http://aa.shtwfgs.cn

case class User(name: String, age: Int)
来源：http://jo.yuexingan06.cn

[T57] Scala：模式匹配
来源：http://ve.nszjky.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wm.szsharing.cn

[T58] Scala：函数定义
来源：http://fo.521024.cn

def add(a: Int, b: Int): Int = a + b
来源：http://mw.9csxet.cn

[T59] Scala：循环
来源：http://hk.huanxung.cn

for (i <- 1 to 10) println(i)
来源：http://sa.huixiangedu.cn

[T60] Scala：折叠
来源：http://qn.shtwfgs.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ci.asd995.cn

================================================================================
来源：http://qn.bjjhwx.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yv.521024.cn

================================================================================
来源：http://rc.newstarts.cn

[U01] Py：创建虚拟环境
来源：http://kh.hnjuh.cn

python -m venv .venv && source .venv/bin/activate
来源：http://pq.jctech888.com.cn

[U02] Py：导出 / 安装依赖
来源：http://dm.asd995.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fp.bjjhwx.cn

[U03] Py：加载 .env 配置
来源：http://sp.colortex.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://hb.bjjhwx.cn

[U04] Py：变量调试打印
来源：http://ir.huanxung.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hm.gzmigu.cn

[U05] Py：列表去重且保序
来源：http://mp.jianghongdianzi.cn

list(dict.fromkeys(arr))
来源：http://dj.shxzukj.cn

[U06] Py：合并两个字典
来源：http://tt.asd995.cn

{**a, **b}
来源：http://fd.9csxet.cn

[U07] Py：反转字典键值
来源：http://az.huanxung.cn

{v: k for k, v in d.items()}
来源：http://qu.asd995.cn

[U08] Py：展平二维列表
来源：http://rk.yuexingan06.cn

[y for x in nested for y in x]
来源：http://gy.asd995.cn

[U09] Py：字典取最大值的键
来源：http://jm.asd995.cn

max(d, key=d.get)
来源：http://ey.huixiangedu.cn

[U10] Py：按值排序字典
来源：http://km.lnxyls.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ui.huanxung.cn

[U11] Py：生成器表达式
来源：http://pt.nicolike.cn

(x * 2 for x in arr)
来源：http://up.huixinmuqiang.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xy.yuntaijiaju.cn

Counter(arr).most_common(3)
来源：http://is.huixinmuqiang.cn

[U13] Py：固定长度队列
来源：http://id.haigaiapp.cn

deque(maxlen=10)
来源：http://za.szsharing.cn

[U14] Py：分组收集到列表
来源：http://qv.yuexingan06.cn

defaultdict(list)
来源：http://yg.nicolike.cn

[U15] Py：高精度计时
来源：http://mx.nszjky.cn

t = time.perf_counter()
来源：http://sw.nszjky.cn

[U16] Py：命令行参数解析
来源：http://kp.huanxung.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mj.jctech888.com.cn

[U17] Py：初始化日志
来源：http://lf.hahajie.cn

logging.basicConfig(level=logging.INFO)
来源：http://nq.huixiangedu.cn

[U18] Py：预编译正则
来源：http://vx.lnxyls.cn

pat = re.compile(r"\d+")
来源：http://bf.wgjwhj.cn

[U19] Py：正则替换带回调
来源：http://yk.yuexingan06.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kg.szxytkj.cn

[U20] Py：缓存函数结果
来源：http://fj.hahajie.cn

@functools.lru_cache(maxsize=None)
来源：http://yy.huixiangedu.cn

[U21] Py：自定义上下文管理器
来源：http://na.panjiajie.cn

@contextlib.contextmanager
来源：http://yq.yuexingan06.cn

[U22] Py：矩阵转置
来源：http://cs.szsharing.cn

list(zip(*m))
来源：http://eo.jianghongdianzi.cn

[U23] Py：分块读取大文件
来源：http://xz.nszjky.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bq.hnjuh.cn

[U24] Py：路径操作
来源：http://de.jctech888.com.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gd.huixiangedu.cn

[U25] Py：CSV 按字典读
来源：http://yz.huixinmuqiang.cn

csv.DictReader(f)
来源：http://rm.wgjwhj.cn

[U26] Py：并发下载
来源：http://no.huixiangedu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nk.huixiangedu.cn

[U27] Py：异步 HTTP
来源：http://yf.yuntaijiaju.cn

aiohttp.ClientSession() 配合 async with
来源：http://ub.shtwfgs.cn

[U28] Py：类型别名
来源：http://qg.gzmigu.cn

UserId = int
来源：http://iw.haigaiapp.cn

[U29] Py：属性校验
来源：http://dt.panjiajie.cn

@property 与 @x.setter 配合
来源：http://za.lnxyls.cn

[U30] Py：数据类
来源：http://rh.521024.cn

@dataclass(slots=True)
来源：http://le.panjiajie.cn

[U31] Py：单测
来源：http://de.nicolike.cn

python -m pytest -q
来源：http://te.jctech888.com.cn

[U32] Py：代码格式化
来源：http://ms.huixiangedu.cn

ruff format . && ruff check --fix .
来源：http://nz.huixinmuqiang.cn

[U33] Py：打包发布
来源：http://wr.9csxet.cn

python -m build  （依赖 pyproject.toml）
来源：http://ec.yuexingan06.cn

[U34] Py：判断编码
来源：http://ca.jctech888.com.cn

chardet.detect(raw)
来源：http://fv.gzmigu.cn

[U35] Py：发送邮件
来源：http://sg.szxytkj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fz.yuexingan06.cn

[U36] Py：定时任务
来源：http://hr.bookmarksfly.cn

schedule.every(10).minutes.do(job)
来源：http://qs.nszjky.cn

[U37] Py：读写 Excel
来源：http://jg.jianghongdianzi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://kx.jctech888.com.cn

[U38] Py：获取脚本所在目录
来源：http://lx.newstarts.cn

Path(__file__).resolve().parent
来源：http://ul.yuexingan06.cn

[U39] Py：判断是否在交互环境
来源：http://qh.shxzukj.cn

sys.stdout.isatty()
来源：http://oy.bjjhwx.cn

[U40] Py：打印到标准错误
来源：http://ss.yuexingan06.cn

print("err", file=sys.stderr)
来源：http://xw.yuexingan06.cn

[U41] PHP：初始化 Composer 项目
来源：http://ly.colortex.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ql.wgjwhj.cn

[U42] PHP：PSR-4 自动加载
来源：http://vy.haigaiapp.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://du.bookmarksfly.cn

[U43] PHP：声明命名空间
来源：http://ie.hahajie.cn

namespace App\Http;
来源：http://qi.asd995.cn

[U44] PHP：开启严格类型
来源：http://zd.wgjwhj.cn

declare(strict_types=1);
来源：http://ik.huixiangedu.cn

[U45] PHP：类型声明与返回类型
来源：http://sd.shxzskj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ow.chemitech.net.cn

[U46] PHP：可空类型
来源：http://dx.huixinmuqiang.cn

?string $name = null
来源：http://ul.szsharing.cn

[U47] PHP：联合类型
来源：http://he.gzmigu.cn

int|string $id
来源：http://jv.shxzskj.cn

[U48] PHP：纯枚举
来源：http://nb.nszjky.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wf.hnjuh.cn

[U49] PHP：只读属性
来源：http://lm.huanxung.cn

public readonly string $name
来源：http://ja.muxihuayi.cn

[U50] PHP：构造器属性提升
来源：http://nn.szsharing.cn

public function __construct(private int $id) {}
来源：http://sl.asd995.cn

[U51] PHP：数组解构
来源：http://qf.lnxyls.cn

[$a, $b] = $arr;
来源：http://jz.panjiajie.cn

[U52] PHP：箭头函数
来源：http://ga.huixinmuqiang.cn

$double = fn($x) => $x * 2;
来源：http://mi.bjjhwx.cn

[U53] PHP：空合并运算符
来源：http://wv.colortex.cn

$v = $a ?? $b ?? "default";
来源：http://ti.shxzskj.cn

[U54] PHP：空安全调用
来源：http://uy.szsharing.cn

$obj?->method()
来源：http://wm.shxzukj.cn

[U55] PHP：match 表达式
来源：http://ar.yuntaijiaju.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rk.bjjhwx.cn

[U56] PHP：命名参数
来源：http://cd.nszjky.cn

f(a: 1, b: 2)
来源：http://cy.huixiangedu.cn

[U57] PHP：字符串插值
来源：http://ky.haigaiapp.cn

"值: {$a}"
来源：http://ua.bjjhwx.cn

[U58] PHP：数组三件套
来源：http://ct.chemitech.net.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mq.9csxet.cn

[U59] PHP：自定义排序
来源：http://gh.newstarts.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tr.hnjuh.cn

[U60] PHP：JSON 编解码
来源：http://ia.muxihuayi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yp.bookmarksfly.cn

[U61] PHP：正则
来源：http://ai.huixiangedu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tg.jctech888.com.cn

[U62] PHP：日期对象
来源：http://bd.yuntaijiaju.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://we.shxzukj.cn

[U63] PHP：文件读写
来源：http://po.szxytkj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nv.asd995.cn

[U64] PHP：目录遍历
来源：http://mb.szsharing.cn

glob("dir/*.php");  scandir("dir");
来源：http://ym.szxytkj.cn

[U65] PHP：会话
来源：http://rx.colortex.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ru.yuexingan06.cn

[U66] PHP：设置 Cookie
来源：http://yd.9csxet.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dd.panjiajie.cn

[U67] PHP：处理文件上传
来源：http://oq.chemitech.net.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dz.szsharing.cn

[U68] PHP：PDO 连接
来源：http://ad.jianghongdianzi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ua.yuexingan06.cn

[U69] PHP：PDO 预处理
来源：http://gg.bjjhwx.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kh.szxytkj.cn

[U70] PHP：PDO 事务
来源：http://tt.9csxet.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://eg.shxzskj.cn

[U71] PHP：抛出异常
来源：http://il.newstarts.cn

throw new RuntimeException("失败", 500);
来源：http://sy.huanxung.cn

[U72] PHP：写错误日志
来源：http://go.lnxyls.cn

error_log("失败: " . $e->getMessage());
来源：http://im.asd995.cn

[U73] PHP：读取 ini 配置
来源：http://ra.muxihuayi.cn

parse_ini_file("config.ini", true)
来源：http://et.bjjhwx.cn

[U74] PHP：读取环境变量
来源：http://gr.hahajie.cn

getenv("APP_ENV") ?: "production"
来源：http://kx.hahajie.cn

[U75] PHP：依赖注入
来源：http://kp.yuexingan06.cn

composer require psr/container
来源：http://aw.huanxung.cn

[U76] PHP：简单路由
来源：http://or.lnxyls.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bc.huanxung.cn

[U77] PHP：模板渲染
来源：http://dx.huanxung.cn

composer require twig/twig
来源：http://bs.nicolike.cn

[U78] PHP：单元测试
来源：http://uq.haigaiapp.cn

composer require --dev phpunit/phpunit
来源：http://gq.asd995.cn

[U79] PHP：静态分析
来源：http://mj.hnjuh.cn

composer require --dev phpstan/phpstan
来源：http://ab.newstarts.cn

[U80] PHP：代码规范修复
来源：http://pe.huixiangedu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://aj.huixinmuqiang.cn

[U81] JS：初始化项目
来源：http://eu.muxihuayi.cn

npm init -y;  npm i express
来源：http://ih.asd995.cn

[U82] JS：package.json 脚本
来源：http://oy.bookmarksfly.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://is.bookmarksfly.cn

[U83] JS：ES Module 导入导出
来源：http://wp.jctech888.com.cn

export const a = 1;  import { a } from "./m.js";
来源：http://yb.9csxet.cn

[U84] JS：CommonJS 写法
来源：http://qy.hnjuh.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ef.panjiajie.cn

[U85] JS：可选链
来源：http://xl.nicolike.cn

a?.b?.c
来源：http://td.muxihuayi.cn

[U86] JS：空值合并
来源：http://iq.huixiangedu.cn

a ?? b
来源：http://sl.huixiangedu.cn

[U87] JS：解构默认值
来源：http://lb.chemitech.net.cn

const { a = 1, b = 2 } = obj;
来源：http://it.521024.cn

[U88] JS：对象展开合并
来源：http://tt.shxzukj.cn

{ ...a, ...b }
来源：http://bo.shxzukj.cn


<!-- 参考信息 -->