代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://aq.yuexingan06.cn

================================================================================
来源：http://jr.huanxung.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fv.nszjky.cn

================================================================================
来源：http://zb.asd995.cn

[T01] Kotlin：Hello World
来源：http://ci.bookmarksfly.cn

println("Hello")
来源：http://gg.jianghongdianzi.cn

[T02] Kotlin：变量
来源：http://ev.9csxet.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hk.nszjky.cn

[T03] Kotlin：字符串模板
来源：http://nd.jianghongdianzi.cn

"值: $b"
来源：http://ta.hnjuh.cn

[T04] Kotlin：空安全
来源：http://sa.panjiajie.cn

val n: String? = null;  n?.length
来源：http://vz.szxytkj.cn

[T05] Kotlin：when 表达式
来源：http://jl.bjjhwx.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hi.jctech888.com.cn

[T06] Kotlin：集合映射
来源：http://jw.9csxet.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ti.yuntaijiaju.cn

[T07] Kotlin：集合过滤
来源：http://so.huixiangedu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xn.nszjky.cn

[T08] Kotlin：数据类
来源：http://pc.wgjwhj.cn

data class User(val name: String, val age: Int)
来源：http://hw.szxytkj.cn

[T09] Kotlin：扩展函数
来源：http://ot.hnjuh.cn

fun String.exclaim() = this + "!"
来源：http://mx.huixinmuqiang.cn

[T10] Kotlin：默认参数
来源：http://bj.bookmarksfly.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ot.gzmigu.cn

[T11] Kotlin：协程
来源：http://wi.huixiangedu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nl.haigaiapp.cn

[T12] Kotlin：解构声明
来源：http://bh.szxytkj.cn

val (a, b) = Pair(1, 2)
来源：http://gd.chemitech.net.cn

[T13] Kotlin：只读 Map
来源：http://cv.chemitech.net.cn

val m = mapOf("a" to 1)
来源：http://aa.szsharing.cn

[T14] Kotlin：循环
来源：http://yr.szsharing.cn

for (i in 1..10) println(i)
来源：http://kd.yuntaijiaju.cn

[T15] Kotlin：接口
来源：http://na.newstarts.cn

interface Shape { fun area(): Double }
来源：http://uf.shtwfgs.cn

[T16] Swift：Hello World
来源：http://ux.gzmigu.cn

print("Hello")
来源：http://ws.lnxyls.cn

[T17] Swift：变量与常量
来源：http://ze.bookmarksfly.cn

var a = 1;  let b = 2
来源：http://yn.chemitech.net.cn

[T18] Swift：字符串插值
来源：http://qv.shxzskj.cn

"值: \(b)"
来源：http://nd.nicolike.cn

[T19] Swift：可选绑定
来源：http://uh.jctech888.com.cn

if let n = opt { print(n) }
来源：http://qn.521024.cn

[T20] Swift：数组操作
来源：http://xp.jianghongdianzi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fe.nicolike.cn

[T21] Swift：遍历
来源：http://fm.bookmarksfly.cn

for x in a { print(x) }
来源：http://ac.jctech888.com.cn

[T22] Swift：字典
来源：http://hm.bjjhwx.cn

var d = ["a": 1];  d["b"] = 2
来源：http://dr.huixiangedu.cn

[T23] Swift：函数
来源：http://qr.hnjuh.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zi.hnjuh.cn

[T24] Swift：闭包
来源：http://dy.jctech888.com.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://hy.shxzskj.cn

[T25] Swift：结构体
来源：http://ed.huanxung.cn

struct P { var x: Int }
来源：http://pm.huixinmuqiang.cn

[T26] Swift：类与重写
来源：http://lw.9csxet.cn

class A: Base { override func f() {} }
来源：http://py.haigaiapp.cn

[T27] Swift：错误处理
来源：http://uc.nszjky.cn

do { try f() } catch { print(error) }
来源：http://yp.haigaiapp.cn

[T28] Swift：枚举
来源：http://cl.521024.cn

enum Color { case red, green }
来源：http://wh.nicolike.cn

[T29] Swift：guard 提前返回
来源：http://fo.huixiangedu.cn

guard let x = opt else { return }
来源：http://sx.9csxet.cn

[T30] Swift：协议
来源：http://pk.bookmarksfly.cn

protocol Shape { func area() -> Double }
来源：http://bh.jctech888.com.cn

[T31] Lua：Hello World
来源：http://ex.jctech888.com.cn

print("Hello")
来源：http://bh.wgjwhj.cn

[T32] Lua：局部变量
来源：http://me.panjiajie.cn

local a = 1
来源：http://kc.huixinmuqiang.cn

[T33] Lua：表（数组）
来源：http://pc.shxzukj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ut.jianghongdianzi.cn

[T34] Lua：遍历表
来源：http://fr.521024.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zp.szxytkj.cn

[T35] Lua：字典表
来源：http://vx.yuexingan06.cn

local d = { a = 1 };  d.b = 2
来源：http://kw.bjjhwx.cn

[T36] Lua：函数
来源：http://ux.chemitech.net.cn

function add(a, b) return a + b end
来源：http://fp.asd995.cn

[T37] Lua：字符串拼接
来源：http://xq.wgjwhj.cn

"a" .. "b"
来源：http://dl.szsharing.cn

[T38] Lua：条件
来源：http://oh.newstarts.cn

if x > 0 then print("正") end
来源：http://gb.jianghongdianzi.cn

[T39] Lua：模式匹配
来源：http://ic.szsharing.cn

string.find(s, "%d+")
来源：http://px.szsharing.cn

[T40] Lua：元表
来源：http://ou.bookmarksfly.cn

setmetatable({}, { __index = base })
来源：http://zv.colortex.cn

[T41] Perl：Hello World
来源：http://rq.nszjky.cn

print "Hello\n";
来源：http://ye.muxihuayi.cn

[T42] Perl：变量类型
来源：http://lk.newstarts.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yn.hahajie.cn

[T43] Perl：字符串插值
来源：http://ix.huixiangedu.cn

"值: $a"
来源：http://uh.shxzskj.cn

[T44] Perl：条件
来源：http://uc.wgjwhj.cn

if ($a > 0) { print "正"; }
来源：http://zx.jctech888.com.cn

[T45] Perl：数组遍历
来源：http://zw.panjiajie.cn

for my $x (@arr) { print $x; }
来源：http://on.jianghongdianzi.cn

[T46] Perl：哈希操作
来源：http://fo.haigaiapp.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jx.haigaiapp.cn

[T47] Perl：正则捕获
来源：http://xh.haigaiapp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ia.shxzskj.cn

[T48] Perl：正则替换
来源：http://zu.shxzskj.cn

$s =~ s/old/new/g;
来源：http://rw.chemitech.net.cn

[T49] Perl：函数
来源：http://ay.haigaiapp.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lo.9csxet.cn

[T50] Perl：逐行读文件
来源：http://pj.nszjky.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://iw.shxzskj.cn

while (my $line = <$fh>) { print $line; }
来源：http://pg.bjjhwx.cn

[T51] Scala：Hello World
来源：http://hk.wgjwhj.cn

println("Hello")
来源：http://ys.panjiajie.cn

[T52] Scala：变量
来源：http://bs.chemitech.net.cn

val a = 1;  var b = 2
来源：http://vg.nicolike.cn

[T53] Scala：字符串插值
来源：http://vi.muxihuayi.cn

s"值: $b"
来源：http://re.shxzukj.cn

[T54] Scala：集合映射
来源：http://ta.hnjuh.cn

List(1, 2, 3).map(_ * 2)
来源：http://px.bjjhwx.cn

[T55] Scala：集合过滤
来源：http://sn.hnjuh.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qi.szsharing.cn

[T56] Scala：样例类
来源：http://hh.huanxung.cn

case class User(name: String, age: Int)
来源：http://lg.yuntaijiaju.cn

[T57] Scala：模式匹配
来源：http://ji.9csxet.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://cb.nszjky.cn

[T58] Scala：函数定义
来源：http://hz.muxihuayi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://qe.bjjhwx.cn

[T59] Scala：循环
来源：http://ik.bjjhwx.cn

for (i <- 1 to 10) println(i)
来源：http://zt.shtwfgs.cn

[T60] Scala：折叠
来源：http://uk.szsharing.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://oc.szxytkj.cn

================================================================================
来源：http://fa.gzmigu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yi.szsharing.cn

================================================================================
来源：http://cf.huixinmuqiang.cn

[U01] Py：创建虚拟环境
来源：http://zq.bookmarksfly.cn

python -m venv .venv && source .venv/bin/activate
来源：http://or.asd995.cn

[U02] Py：导出 / 安装依赖
来源：http://hz.gzmigu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hs.yuexingan06.cn

[U03] Py：加载 .env 配置
来源：http://zj.bookmarksfly.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qx.nszjky.cn

[U04] Py：变量调试打印
来源：http://ds.szsharing.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wv.asd995.cn

[U05] Py：列表去重且保序
来源：http://ba.colortex.cn

list(dict.fromkeys(arr))
来源：http://ba.newstarts.cn

[U06] Py：合并两个字典
来源：http://np.gzmigu.cn

{**a, **b}
来源：http://ou.huixiangedu.cn

[U07] Py：反转字典键值
来源：http://vl.wgjwhj.cn

{v: k for k, v in d.items()}
来源：http://oe.nicolike.cn

[U08] Py：展平二维列表
来源：http://rs.nicolike.cn

[y for x in nested for y in x]
来源：http://sg.huanxung.cn

[U09] Py：字典取最大值的键
来源：http://ic.huixinmuqiang.cn

max(d, key=d.get)
来源：http://oi.yuexingan06.cn

[U10] Py：按值排序字典
来源：http://ey.muxihuayi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lg.lnxyls.cn

[U11] Py：生成器表达式
来源：http://qu.shxzukj.cn

(x * 2 for x in arr)
来源：http://fa.nicolike.cn

[U12] Py：取出现最多的 3 个元素
来源：http://hb.bjjhwx.cn

Counter(arr).most_common(3)
来源：http://xn.colortex.cn

[U13] Py：固定长度队列
来源：http://as.chemitech.net.cn

deque(maxlen=10)
来源：http://dp.yuntaijiaju.cn

[U14] Py：分组收集到列表
来源：http://ji.huixinmuqiang.cn

defaultdict(list)
来源：http://st.huixiangedu.cn

[U15] Py：高精度计时
来源：http://hb.colortex.cn

t = time.perf_counter()
来源：http://ya.hnjuh.cn

[U16] Py：命令行参数解析
来源：http://qa.yuexingan06.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ku.hnjuh.cn

[U17] Py：初始化日志
来源：http://jn.bookmarksfly.cn

logging.basicConfig(level=logging.INFO)
来源：http://mq.521024.cn

[U18] Py：预编译正则
来源：http://fw.nszjky.cn

pat = re.compile(r"\d+")
来源：http://az.jctech888.com.cn

[U19] Py：正则替换带回调
来源：http://mv.muxihuayi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fk.bookmarksfly.cn

[U20] Py：缓存函数结果
来源：http://ao.huixiangedu.cn

@functools.lru_cache(maxsize=None)
来源：http://iy.yuntaijiaju.cn

[U21] Py：自定义上下文管理器
来源：http://ub.bookmarksfly.cn

@contextlib.contextmanager
来源：http://os.521024.cn

[U22] Py：矩阵转置
来源：http://nz.jctech888.com.cn

list(zip(*m))
来源：http://mg.wgjwhj.cn

[U23] Py：分块读取大文件
来源：http://pu.nicolike.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lq.huanxung.cn

[U24] Py：路径操作
来源：http://fs.shxzskj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kd.szsharing.cn

[U25] Py：CSV 按字典读
来源：http://rd.szxytkj.cn

csv.DictReader(f)
来源：http://dc.521024.cn

[U26] Py：并发下载
来源：http://ex.jctech888.com.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bg.huanxung.cn

[U27] Py：异步 HTTP
来源：http://qh.9csxet.cn

aiohttp.ClientSession() 配合 async with
来源：http://ee.yuexingan06.cn

[U28] Py：类型别名
来源：http://qh.panjiajie.cn

UserId = int
来源：http://zy.nicolike.cn

[U29] Py：属性校验
来源：http://dg.szxytkj.cn

@property 与 @x.setter 配合
来源：http://bm.lnxyls.cn

[U30] Py：数据类
来源：http://os.521024.cn

@dataclass(slots=True)
来源：http://zd.jctech888.com.cn

[U31] Py：单测
来源：http://qa.haigaiapp.cn

python -m pytest -q
来源：http://ug.huixiangedu.cn

[U32] Py：代码格式化
来源：http://nk.bjjhwx.cn

ruff format . && ruff check --fix .
来源：http://xq.panjiajie.cn

[U33] Py：打包发布
来源：http://ko.newstarts.cn

python -m build  （依赖 pyproject.toml）
来源：http://bz.hnjuh.cn

[U34] Py：判断编码
来源：http://vi.haigaiapp.cn

chardet.detect(raw)
来源：http://et.szsharing.cn

[U35] Py：发送邮件
来源：http://yz.lnxyls.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rl.haigaiapp.cn

[U36] Py：定时任务
来源：http://ni.haigaiapp.cn

schedule.every(10).minutes.do(job)
来源：http://fp.9csxet.cn

[U37] Py：读写 Excel
来源：http://wi.haigaiapp.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ss.haigaiapp.cn

[U38] Py：获取脚本所在目录
来源：http://hs.nszjky.cn

Path(__file__).resolve().parent
来源：http://ak.huixiangedu.cn

[U39] Py：判断是否在交互环境
来源：http://vx.asd995.cn

sys.stdout.isatty()
来源：http://vz.newstarts.cn

[U40] Py：打印到标准错误
来源：http://jp.huanxung.cn

print("err", file=sys.stderr)
来源：http://bu.szsharing.cn

[U41] PHP：初始化 Composer 项目
来源：http://iw.jctech888.com.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zu.panjiajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://qg.wgjwhj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://uv.nicolike.cn

[U43] PHP：声明命名空间
来源：http://zo.hnjuh.cn

namespace App\Http;
来源：http://hh.nszjky.cn

[U44] PHP：开启严格类型
来源：http://yn.huixinmuqiang.cn

declare(strict_types=1);
来源：http://au.huanxung.cn

[U45] PHP：类型声明与返回类型
来源：http://gx.asd995.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://zb.gzmigu.cn

[U46] PHP：可空类型
来源：http://ob.szxytkj.cn

?string $name = null
来源：http://pw.muxihuayi.cn

[U47] PHP：联合类型
来源：http://do.hnjuh.cn

int|string $id
来源：http://ih.asd995.cn

[U48] PHP：纯枚举
来源：http://xz.jctech888.com.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ft.hahajie.cn

[U49] PHP：只读属性
来源：http://ki.nicolike.cn

public readonly string $name
来源：http://gz.nicolike.cn

[U50] PHP：构造器属性提升
来源：http://ru.colortex.cn

public function __construct(private int $id) {}
来源：http://le.jctech888.com.cn

[U51] PHP：数组解构
来源：http://rg.muxihuayi.cn

[$a, $b] = $arr;
来源：http://jm.chemitech.net.cn

[U52] PHP：箭头函数
来源：http://sk.bookmarksfly.cn

$double = fn($x) => $x * 2;
来源：http://qj.521024.cn

[U53] PHP：空合并运算符
来源：http://vd.lnxyls.cn

$v = $a ?? $b ?? "default";
来源：http://ye.huanxung.cn

[U54] PHP：空安全调用
来源：http://mh.hahajie.cn

$obj?->method()
来源：http://rr.szsharing.cn

[U55] PHP：match 表达式
来源：http://iu.9csxet.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vo.hnjuh.cn

[U56] PHP：命名参数
来源：http://ha.yuntaijiaju.cn

f(a: 1, b: 2)
来源：http://ul.bookmarksfly.cn

[U57] PHP：字符串插值
来源：http://ba.bjjhwx.cn

"值: {$a}"
来源：http://ug.huixinmuqiang.cn

[U58] PHP：数组三件套
来源：http://pl.chemitech.net.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vh.haigaiapp.cn

[U59] PHP：自定义排序
来源：http://du.9csxet.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xv.shxzukj.cn

[U60] PHP：JSON 编解码
来源：http://xa.haigaiapp.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fi.haigaiapp.cn

[U61] PHP：正则
来源：http://vk.521024.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ku.huixiangedu.cn

[U62] PHP：日期对象
来源：http://gv.szsharing.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xf.hnjuh.cn

[U63] PHP：文件读写
来源：http://lt.shxzukj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://np.nicolike.cn

[U64] PHP：目录遍历
来源：http://vb.bjjhwx.cn

glob("dir/*.php");  scandir("dir");
来源：http://jl.asd995.cn

[U65] PHP：会话
来源：http://ao.nszjky.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://zr.newstarts.cn

[U66] PHP：设置 Cookie
来源：http://xv.huanxung.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xq.bookmarksfly.cn

[U67] PHP：处理文件上传
来源：http://bd.asd995.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fu.hahajie.cn

[U68] PHP：PDO 连接
来源：http://dh.newstarts.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pi.bookmarksfly.cn

[U69] PHP：PDO 预处理
来源：http://na.panjiajie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wr.shtwfgs.cn

[U70] PHP：PDO 事务
来源：http://nj.hahajie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://el.wgjwhj.cn

[U71] PHP：抛出异常
来源：http://tu.asd995.cn

throw new RuntimeException("失败", 500);
来源：http://nu.shxzskj.cn

[U72] PHP：写错误日志
来源：http://id.shxzukj.cn

error_log("失败: " . $e->getMessage());
来源：http://bt.huanxung.cn

[U73] PHP：读取 ini 配置
来源：http://jv.hnjuh.cn

parse_ini_file("config.ini", true)
来源：http://ib.nszjky.cn

[U74] PHP：读取环境变量
来源：http://pq.gzmigu.cn

getenv("APP_ENV") ?: "production"
来源：http://fr.shxzukj.cn

[U75] PHP：依赖注入
来源：http://ob.huixiangedu.cn

composer require psr/container
来源：http://ca.gzmigu.cn

[U76] PHP：简单路由
来源：http://zl.haigaiapp.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sw.jctech888.com.cn

[U77] PHP：模板渲染
来源：http://cb.muxihuayi.cn

composer require twig/twig
来源：http://kc.newstarts.cn

[U78] PHP：单元测试
来源：http://rn.hahajie.cn

composer require --dev phpunit/phpunit
来源：http://np.lnxyls.cn

[U79] PHP：静态分析
来源：http://lw.huixinmuqiang.cn

composer require --dev phpstan/phpstan
来源：http://rc.lnxyls.cn

[U80] PHP：代码规范修复
来源：http://qu.bookmarksfly.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://hq.yuntaijiaju.cn

[U81] JS：初始化项目
来源：http://xh.newstarts.cn

npm init -y;  npm i express
来源：http://id.panjiajie.cn

[U82] JS：package.json 脚本
来源：http://bi.asd995.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jm.bjjhwx.cn

[U83] JS：ES Module 导入导出
来源：http://qt.yuexingan06.cn

export const a = 1;  import { a } from "./m.js";
来源：http://af.shxzskj.cn

[U84] JS：CommonJS 写法
来源：http://wy.hnjuh.cn

module.exports = { a };  const { a } = require("./m");
来源：http://di.huanxung.cn

[U85] JS：可选链
来源：http://zn.szsharing.cn

a?.b?.c
来源：http://ht.huanxung.cn

[U86] JS：空值合并
来源：http://pa.colortex.cn

a ?? b
来源：http://ix.jianghongdianzi.cn


<!-- 参考信息 -->