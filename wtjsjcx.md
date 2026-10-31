代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yn.bjjhwx.cn

================================================================================
来源：http://qa.yuexingan06.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://se.shxzukj.cn

================================================================================
来源：http://ox.chemitech.net.cn

[T01] Kotlin：Hello World
来源：http://mp.shtwfgs.cn

println("Hello")
来源：http://nu.wgjwhj.cn

[T02] Kotlin：变量
来源：http://or.yuntaijiaju.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jr.wgjwhj.cn

[T03] Kotlin：字符串模板
来源：http://cw.muxihuayi.cn

"值: $b"
来源：http://kf.chemitech.net.cn

[T04] Kotlin：空安全
来源：http://km.huixinmuqiang.cn

val n: String? = null;  n?.length
来源：http://he.yuntaijiaju.cn

[T05] Kotlin：when 表达式
来源：http://oi.jctech888.com.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://du.jctech888.com.cn

[T06] Kotlin：集合映射
来源：http://ug.muxihuayi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fw.newstarts.cn

[T07] Kotlin：集合过滤
来源：http://ol.bookmarksfly.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fu.haigaiapp.cn

[T08] Kotlin：数据类
来源：http://iw.lnxyls.cn

data class User(val name: String, val age: Int)
来源：http://xy.huixinmuqiang.cn

[T09] Kotlin：扩展函数
来源：http://zc.yuntaijiaju.cn

fun String.exclaim() = this + "!"
来源：http://tm.wgjwhj.cn

[T10] Kotlin：默认参数
来源：http://tt.hahajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://np.haigaiapp.cn

[T11] Kotlin：协程
来源：http://yq.wgjwhj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://rl.521024.cn

[T12] Kotlin：解构声明
来源：http://px.wgjwhj.cn

val (a, b) = Pair(1, 2)
来源：http://hd.yuexingan06.cn

[T13] Kotlin：只读 Map
来源：http://ft.panjiajie.cn

val m = mapOf("a" to 1)
来源：http://qt.newstarts.cn

[T14] Kotlin：循环
来源：http://jt.gzmigu.cn

for (i in 1..10) println(i)
来源：http://wh.9csxet.cn

[T15] Kotlin：接口
来源：http://hg.haigaiapp.cn

interface Shape { fun area(): Double }
来源：http://lt.gzmigu.cn

[T16] Swift：Hello World
来源：http://qm.huixiangedu.cn

print("Hello")
来源：http://kb.shxzukj.cn

[T17] Swift：变量与常量
来源：http://rf.chemitech.net.cn

var a = 1;  let b = 2
来源：http://nj.bookmarksfly.cn

[T18] Swift：字符串插值
来源：http://de.szxytkj.cn

"值: \(b)"
来源：http://xa.bjjhwx.cn

[T19] Swift：可选绑定
来源：http://iw.newstarts.cn

if let n = opt { print(n) }
来源：http://qp.shxzukj.cn

[T20] Swift：数组操作
来源：http://cm.nszjky.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ul.panjiajie.cn

[T21] Swift：遍历
来源：http://dh.huanxung.cn

for x in a { print(x) }
来源：http://sh.newstarts.cn

[T22] Swift：字典
来源：http://wf.wgjwhj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://en.shxzukj.cn

[T23] Swift：函数
来源：http://rn.szxytkj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cu.haigaiapp.cn

[T24] Swift：闭包
来源：http://xz.huanxung.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://kz.9csxet.cn

[T25] Swift：结构体
来源：http://kj.wgjwhj.cn

struct P { var x: Int }
来源：http://nz.huanxung.cn

[T26] Swift：类与重写
来源：http://zb.muxihuayi.cn

class A: Base { override func f() {} }
来源：http://wm.asd995.cn

[T27] Swift：错误处理
来源：http://wy.9csxet.cn

do { try f() } catch { print(error) }
来源：http://uw.nicolike.cn

[T28] Swift：枚举
来源：http://uq.jianghongdianzi.cn

enum Color { case red, green }
来源：http://cb.asd995.cn

[T29] Swift：guard 提前返回
来源：http://qy.haigaiapp.cn

guard let x = opt else { return }
来源：http://gy.asd995.cn

[T30] Swift：协议
来源：http://nw.asd995.cn

protocol Shape { func area() -> Double }
来源：http://we.yuexingan06.cn

[T31] Lua：Hello World
来源：http://he.szsharing.cn

print("Hello")
来源：http://dv.yuntaijiaju.cn

[T32] Lua：局部变量
来源：http://ag.asd995.cn

local a = 1
来源：http://yc.9csxet.cn

[T33] Lua：表（数组）
来源：http://ra.huixinmuqiang.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://lp.huixiangedu.cn

[T34] Lua：遍历表
来源：http://xi.shxzukj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gd.hnjuh.cn

[T35] Lua：字典表
来源：http://ds.shxzukj.cn

local d = { a = 1 };  d.b = 2
来源：http://xy.jianghongdianzi.cn

[T36] Lua：函数
来源：http://fl.bookmarksfly.cn

function add(a, b) return a + b end
来源：http://zm.colortex.cn

[T37] Lua：字符串拼接
来源：http://ek.nicolike.cn

"a" .. "b"
来源：http://tk.colortex.cn

[T38] Lua：条件
来源：http://pf.nicolike.cn

if x > 0 then print("正") end
来源：http://xy.asd995.cn

[T39] Lua：模式匹配
来源：http://pj.yuntaijiaju.cn

string.find(s, "%d+")
来源：http://fw.szsharing.cn

[T40] Lua：元表
来源：http://at.szsharing.cn

setmetatable({}, { __index = base })
来源：http://cr.haigaiapp.cn

[T41] Perl：Hello World
来源：http://ef.haigaiapp.cn

print "Hello\n";
来源：http://fb.521024.cn

[T42] Perl：变量类型
来源：http://cr.jctech888.com.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kj.huixinmuqiang.cn

[T43] Perl：字符串插值
来源：http://qq.szxytkj.cn

"值: $a"
来源：http://qw.asd995.cn

[T44] Perl：条件
来源：http://rx.shtwfgs.cn

if ($a > 0) { print "正"; }
来源：http://is.nszjky.cn

[T45] Perl：数组遍历
来源：http://kq.jctech888.com.cn

for my $x (@arr) { print $x; }
来源：http://kg.gzmigu.cn

[T46] Perl：哈希操作
来源：http://qd.nicolike.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dy.jctech888.com.cn

[T47] Perl：正则捕获
来源：http://cv.521024.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qr.9csxet.cn

[T48] Perl：正则替换
来源：http://yg.9csxet.cn

$s =~ s/old/new/g;
来源：http://yn.yuexingan06.cn

[T49] Perl：函数
来源：http://jn.hahajie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zf.chemitech.net.cn

[T50] Perl：逐行读文件
来源：http://qa.yuexingan06.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fi.shtwfgs.cn

while (my $line = <$fh>) { print $line; }
来源：http://xr.colortex.cn

[T51] Scala：Hello World
来源：http://vi.huanxung.cn

println("Hello")
来源：http://om.yuntaijiaju.cn

[T52] Scala：变量
来源：http://sk.hnjuh.cn

val a = 1;  var b = 2
来源：http://wh.szxytkj.cn

[T53] Scala：字符串插值
来源：http://rs.shtwfgs.cn

s"值: $b"
来源：http://ac.panjiajie.cn

[T54] Scala：集合映射
来源：http://vk.bookmarksfly.cn

List(1, 2, 3).map(_ * 2)
来源：http://on.shxzukj.cn

[T55] Scala：集合过滤
来源：http://ec.muxihuayi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fb.chemitech.net.cn

[T56] Scala：样例类
来源：http://co.nszjky.cn

case class User(name: String, age: Int)
来源：http://aq.panjiajie.cn

[T57] Scala：模式匹配
来源：http://by.colortex.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://to.newstarts.cn

[T58] Scala：函数定义
来源：http://rt.hnjuh.cn

def add(a: Int, b: Int): Int = a + b
来源：http://cs.szxytkj.cn

[T59] Scala：循环
来源：http://eg.chemitech.net.cn

for (i <- 1 to 10) println(i)
来源：http://ve.shtwfgs.cn

[T60] Scala：折叠
来源：http://uq.muxihuayi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ct.nicolike.cn

================================================================================
来源：http://ao.bookmarksfly.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://aq.lnxyls.cn

================================================================================
来源：http://wz.lnxyls.cn

[U01] Py：创建虚拟环境
来源：http://hy.newstarts.cn

python -m venv .venv && source .venv/bin/activate
来源：http://tj.chemitech.net.cn

[U02] Py：导出 / 安装依赖
来源：http://bm.colortex.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://aw.hahajie.cn

[U03] Py：加载 .env 配置
来源：http://xt.9csxet.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://sq.hnjuh.cn

[U04] Py：变量调试打印
来源：http://yo.muxihuayi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ag.szsharing.cn

[U05] Py：列表去重且保序
来源：http://du.panjiajie.cn

list(dict.fromkeys(arr))
来源：http://ze.szxytkj.cn

[U06] Py：合并两个字典
来源：http://kt.nszjky.cn

{**a, **b}
来源：http://ey.jctech888.com.cn

[U07] Py：反转字典键值
来源：http://jt.521024.cn

{v: k for k, v in d.items()}
来源：http://zq.nszjky.cn

[U08] Py：展平二维列表
来源：http://kt.yuexingan06.cn

[y for x in nested for y in x]
来源：http://jm.shxzukj.cn

[U09] Py：字典取最大值的键
来源：http://ss.wgjwhj.cn

max(d, key=d.get)
来源：http://gh.shxzskj.cn

[U10] Py：按值排序字典
来源：http://wi.huanxung.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://es.jianghongdianzi.cn

[U11] Py：生成器表达式
来源：http://kd.haigaiapp.cn

(x * 2 for x in arr)
来源：http://ls.huanxung.cn

[U12] Py：取出现最多的 3 个元素
来源：http://oo.haigaiapp.cn

Counter(arr).most_common(3)
来源：http://vj.bookmarksfly.cn

[U13] Py：固定长度队列
来源：http://ex.asd995.cn

deque(maxlen=10)
来源：http://ew.nicolike.cn

[U14] Py：分组收集到列表
来源：http://gq.hnjuh.cn

defaultdict(list)
来源：http://gu.huixinmuqiang.cn

[U15] Py：高精度计时
来源：http://rj.9csxet.cn

t = time.perf_counter()
来源：http://ql.nszjky.cn

[U16] Py：命令行参数解析
来源：http://hh.nicolike.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dg.panjiajie.cn

[U17] Py：初始化日志
来源：http://bx.521024.cn

logging.basicConfig(level=logging.INFO)
来源：http://uu.wgjwhj.cn

[U18] Py：预编译正则
来源：http://go.huixinmuqiang.cn

pat = re.compile(r"\d+")
来源：http://fo.asd995.cn

[U19] Py：正则替换带回调
来源：http://oz.nszjky.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gw.huanxung.cn

[U20] Py：缓存函数结果
来源：http://ij.huanxung.cn

@functools.lru_cache(maxsize=None)
来源：http://kp.bjjhwx.cn

[U21] Py：自定义上下文管理器
来源：http://bq.wgjwhj.cn

@contextlib.contextmanager
来源：http://yc.wgjwhj.cn

[U22] Py：矩阵转置
来源：http://ri.hnjuh.cn

list(zip(*m))
来源：http://pp.shxzskj.cn

[U23] Py：分块读取大文件
来源：http://jq.bookmarksfly.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dc.wgjwhj.cn

[U24] Py：路径操作
来源：http://qu.panjiajie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dj.muxihuayi.cn

[U25] Py：CSV 按字典读
来源：http://db.bookmarksfly.cn

csv.DictReader(f)
来源：http://pk.hahajie.cn

[U26] Py：并发下载
来源：http://xt.newstarts.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vk.521024.cn

[U27] Py：异步 HTTP
来源：http://ke.szxytkj.cn

aiohttp.ClientSession() 配合 async with
来源：http://dv.shxzskj.cn

[U28] Py：类型别名
来源：http://qb.lnxyls.cn

UserId = int
来源：http://qa.haigaiapp.cn

[U29] Py：属性校验
来源：http://np.9csxet.cn

@property 与 @x.setter 配合
来源：http://qk.shtwfgs.cn

[U30] Py：数据类
来源：http://vw.bjjhwx.cn

@dataclass(slots=True)
来源：http://uj.colortex.cn

[U31] Py：单测
来源：http://wd.szsharing.cn

python -m pytest -q
来源：http://gp.hahajie.cn

[U32] Py：代码格式化
来源：http://bf.muxihuayi.cn

ruff format . && ruff check --fix .
来源：http://vf.hahajie.cn

[U33] Py：打包发布
来源：http://tu.muxihuayi.cn

python -m build  （依赖 pyproject.toml）
来源：http://mf.jctech888.com.cn

[U34] Py：判断编码
来源：http://mq.panjiajie.cn

chardet.detect(raw)
来源：http://jk.haigaiapp.cn

[U35] Py：发送邮件
来源：http://dk.huanxung.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://np.huanxung.cn

[U36] Py：定时任务
来源：http://ph.newstarts.cn

schedule.every(10).minutes.do(job)
来源：http://ja.szsharing.cn

[U37] Py：读写 Excel
来源：http://po.muxihuayi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://zl.muxihuayi.cn

[U38] Py：获取脚本所在目录
来源：http://db.bjjhwx.cn

Path(__file__).resolve().parent
来源：http://aw.hnjuh.cn

[U39] Py：判断是否在交互环境
来源：http://rw.lnxyls.cn

sys.stdout.isatty()
来源：http://bg.muxihuayi.cn

[U40] Py：打印到标准错误
来源：http://mg.nszjky.cn

print("err", file=sys.stderr)
来源：http://fz.gzmigu.cn

[U41] PHP：初始化 Composer 项目
来源：http://wz.wgjwhj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://dt.shtwfgs.cn

[U42] PHP：PSR-4 自动加载
来源：http://ss.9csxet.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zl.nicolike.cn

[U43] PHP：声明命名空间
来源：http://lq.szxytkj.cn

namespace App\Http;
来源：http://tv.nszjky.cn

[U44] PHP：开启严格类型
来源：http://ge.nicolike.cn

declare(strict_types=1);
来源：http://pc.huixiangedu.cn

[U45] PHP：类型声明与返回类型
来源：http://wi.muxihuayi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ff.jctech888.com.cn

[U46] PHP：可空类型
来源：http://ep.colortex.cn

?string $name = null
来源：http://bl.shtwfgs.cn

[U47] PHP：联合类型
来源：http://sb.newstarts.cn

int|string $id
来源：http://nu.hahajie.cn

[U48] PHP：纯枚举
来源：http://ja.9csxet.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bt.chemitech.net.cn

[U49] PHP：只读属性
来源：http://vz.huanxung.cn

public readonly string $name
来源：http://nj.hahajie.cn

[U50] PHP：构造器属性提升
来源：http://fo.521024.cn

public function __construct(private int $id) {}
来源：http://tg.haigaiapp.cn

[U51] PHP：数组解构
来源：http://nt.huixiangedu.cn

[$a, $b] = $arr;
来源：http://jh.bjjhwx.cn

[U52] PHP：箭头函数
来源：http://lu.shxzskj.cn

$double = fn($x) => $x * 2;
来源：http://ou.521024.cn

[U53] PHP：空合并运算符
来源：http://co.bookmarksfly.cn

$v = $a ?? $b ?? "default";
来源：http://sm.521024.cn

[U54] PHP：空安全调用
来源：http://mt.szxytkj.cn

$obj?->method()
来源：http://tc.jianghongdianzi.cn

[U55] PHP：match 表达式
来源：http://fb.asd995.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gw.jctech888.com.cn

[U56] PHP：命名参数
来源：http://mn.yuntaijiaju.cn

f(a: 1, b: 2)
来源：http://fd.lnxyls.cn

[U57] PHP：字符串插值
来源：http://ap.huixiangedu.cn

"值: {$a}"
来源：http://uh.huanxung.cn

[U58] PHP：数组三件套
来源：http://qo.szsharing.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xv.huixinmuqiang.cn

[U59] PHP：自定义排序
来源：http://lp.panjiajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eu.nszjky.cn

[U60] PHP：JSON 编解码
来源：http://ko.panjiajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://va.nszjky.cn

[U61] PHP：正则
来源：http://cc.521024.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zi.521024.cn

[U62] PHP：日期对象
来源：http://yj.bookmarksfly.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://it.panjiajie.cn

[U63] PHP：文件读写
来源：http://sa.jianghongdianzi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ad.shxzukj.cn

[U64] PHP：目录遍历
来源：http://rs.9csxet.cn

glob("dir/*.php");  scandir("dir");
来源：http://su.haigaiapp.cn

[U65] PHP：会话
来源：http://vr.jctech888.com.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://zr.shxzskj.cn

[U66] PHP：设置 Cookie
来源：http://oa.yuntaijiaju.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ry.nszjky.cn

[U67] PHP：处理文件上传
来源：http://wq.asd995.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://in.bjjhwx.cn

[U68] PHP：PDO 连接
来源：http://ti.haigaiapp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nl.huanxung.cn

[U69] PHP：PDO 预处理
来源：http://ji.521024.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fm.newstarts.cn

[U70] PHP：PDO 事务
来源：http://os.huixinmuqiang.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wc.shtwfgs.cn

[U71] PHP：抛出异常
来源：http://rc.haigaiapp.cn

throw new RuntimeException("失败", 500);
来源：http://kk.gzmigu.cn

[U72] PHP：写错误日志
来源：http://kj.bookmarksfly.cn

error_log("失败: " . $e->getMessage());
来源：http://kk.yuexingan06.cn

[U73] PHP：读取 ini 配置
来源：http://nv.asd995.cn

parse_ini_file("config.ini", true)
来源：http://iw.panjiajie.cn

[U74] PHP：读取环境变量
来源：http://xt.shtwfgs.cn

getenv("APP_ENV") ?: "production"
来源：http://xm.nszjky.cn

[U75] PHP：依赖注入
来源：http://ws.shxzskj.cn

composer require psr/container
来源：http://bl.haigaiapp.cn

[U76] PHP：简单路由
来源：http://rt.huixinmuqiang.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gn.gzmigu.cn

[U77] PHP：模板渲染
来源：http://jk.huixinmuqiang.cn

composer require twig/twig
来源：http://mo.haigaiapp.cn

[U78] PHP：单元测试
来源：http://mj.yuntaijiaju.cn

composer require --dev phpunit/phpunit
来源：http://cx.521024.cn

[U79] PHP：静态分析
来源：http://ya.wgjwhj.cn

composer require --dev phpstan/phpstan
来源：http://tb.shtwfgs.cn

[U80] PHP：代码规范修复
来源：http://so.szsharing.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://hr.nicolike.cn

[U81] JS：初始化项目
来源：http://hk.huanxung.cn

npm init -y;  npm i express
来源：http://se.yuntaijiaju.cn

[U82] JS：package.json 脚本
来源：http://pq.yuntaijiaju.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ng.muxihuayi.cn

[U83] JS：ES Module 导入导出
来源：http://oq.hnjuh.cn

export const a = 1;  import { a } from "./m.js";
来源：http://gd.9csxet.cn

[U84] JS：CommonJS 写法
来源：http://sg.haigaiapp.cn

module.exports = { a };  const { a } = require("./m");
来源：http://fp.asd995.cn

[U85] JS：可选链
来源：http://su.nicolike.cn

a?.b?.c
来源：http://rd.bookmarksfly.cn

[U86] JS：空值合并
来源：http://mt.jctech888.com.cn

a ?? b
来源：http://ak.muxihuayi.cn


<!-- 参考信息 -->