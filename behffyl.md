代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://hg.nicolike.cn

[S59] C++：静态断言
来源：http://kj.nicolike.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pi.nszjky.cn

[S60] C++：遍历并删除元素
来源：http://au.521024.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ys.szxytkj.cn

================================================================================
来源：http://uk.huixinmuqiang.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://it.nicolike.cn

================================================================================
来源：http://bb.shxzukj.cn

[T01] Kotlin：Hello World
来源：http://vr.hahajie.cn

println("Hello")
来源：http://fd.nicolike.cn

[T02] Kotlin：变量
来源：http://hq.gzmigu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://oq.muxihuayi.cn

[T03] Kotlin：字符串模板
来源：http://ym.colortex.cn

"值: $b"
来源：http://cu.shxzukj.cn

[T04] Kotlin：空安全
来源：http://pq.lnxyls.cn

val n: String? = null;  n?.length
来源：http://ur.bookmarksfly.cn

[T05] Kotlin：when 表达式
来源：http://xl.szsharing.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gi.chemitech.net.cn

[T06] Kotlin：集合映射
来源：http://il.shxzukj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://bj.bookmarksfly.cn

[T07] Kotlin：集合过滤
来源：http://fi.lnxyls.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://nm.jianghongdianzi.cn

[T08] Kotlin：数据类
来源：http://nx.newstarts.cn

data class User(val name: String, val age: Int)
来源：http://si.9csxet.cn

[T09] Kotlin：扩展函数
来源：http://wf.yuntaijiaju.cn

fun String.exclaim() = this + "!"
来源：http://vl.yuntaijiaju.cn

[T10] Kotlin：默认参数
来源：http://zh.panjiajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://yk.huixiangedu.cn

[T11] Kotlin：协程
来源：http://pt.nszjky.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jx.huixiangedu.cn

[T12] Kotlin：解构声明
来源：http://hp.gzmigu.cn

val (a, b) = Pair(1, 2)
来源：http://hj.szsharing.cn

[T13] Kotlin：只读 Map
来源：http://fr.9csxet.cn

val m = mapOf("a" to 1)
来源：http://ue.bookmarksfly.cn

[T14] Kotlin：循环
来源：http://kn.bjjhwx.cn

for (i in 1..10) println(i)
来源：http://gb.nicolike.cn

[T15] Kotlin：接口
来源：http://ou.chemitech.net.cn

interface Shape { fun area(): Double }
来源：http://dc.yuexingan06.cn

[T16] Swift：Hello World
来源：http://gt.muxihuayi.cn

print("Hello")
来源：http://jy.panjiajie.cn

[T17] Swift：变量与常量
来源：http://mh.chemitech.net.cn

var a = 1;  let b = 2
来源：http://gn.huixinmuqiang.cn

[T18] Swift：字符串插值
来源：http://oh.hnjuh.cn

"值: \(b)"
来源：http://xz.shtwfgs.cn

[T19] Swift：可选绑定
来源：http://dg.shtwfgs.cn

if let n = opt { print(n) }
来源：http://ha.colortex.cn

[T20] Swift：数组操作
来源：http://uc.hnjuh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://bs.gzmigu.cn

[T21] Swift：遍历
来源：http://ue.9csxet.cn

for x in a { print(x) }
来源：http://pi.muxihuayi.cn

[T22] Swift：字典
来源：http://yg.shxzukj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://hr.jianghongdianzi.cn

[T23] Swift：函数
来源：http://ek.huixiangedu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kx.jctech888.com.cn

[T24] Swift：闭包
来源：http://bj.9csxet.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zn.shtwfgs.cn

[T25] Swift：结构体
来源：http://yc.hahajie.cn

struct P { var x: Int }
来源：http://vz.521024.cn

[T26] Swift：类与重写
来源：http://yi.huixiangedu.cn

class A: Base { override func f() {} }
来源：http://vf.szxytkj.cn

[T27] Swift：错误处理
来源：http://pr.nszjky.cn

do { try f() } catch { print(error) }
来源：http://pv.yuntaijiaju.cn

[T28] Swift：枚举
来源：http://tx.9csxet.cn

enum Color { case red, green }
来源：http://ff.yuntaijiaju.cn

[T29] Swift：guard 提前返回
来源：http://yi.muxihuayi.cn

guard let x = opt else { return }
来源：http://wy.hahajie.cn

[T30] Swift：协议
来源：http://fi.wgjwhj.cn

protocol Shape { func area() -> Double }
来源：http://hs.asd995.cn

[T31] Lua：Hello World
来源：http://va.chemitech.net.cn

print("Hello")
来源：http://sl.yuntaijiaju.cn

[T32] Lua：局部变量
来源：http://ev.szsharing.cn

local a = 1
来源：http://ev.521024.cn

[T33] Lua：表（数组）
来源：http://ud.lnxyls.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ve.nszjky.cn

[T34] Lua：遍历表
来源：http://mg.521024.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://td.bjjhwx.cn

[T35] Lua：字典表
来源：http://ji.szxytkj.cn

local d = { a = 1 };  d.b = 2
来源：http://gb.gzmigu.cn

[T36] Lua：函数
来源：http://qd.huixiangedu.cn

function add(a, b) return a + b end
来源：http://ui.huixiangedu.cn

[T37] Lua：字符串拼接
来源：http://ec.wgjwhj.cn

"a" .. "b"
来源：http://pm.newstarts.cn

[T38] Lua：条件
来源：http://xy.hnjuh.cn

if x > 0 then print("正") end
来源：http://kt.hahajie.cn

[T39] Lua：模式匹配
来源：http://xx.haigaiapp.cn

string.find(s, "%d+")
来源：http://fr.chemitech.net.cn

[T40] Lua：元表
来源：http://vz.szsharing.cn

setmetatable({}, { __index = base })
来源：http://nw.wgjwhj.cn

[T41] Perl：Hello World
来源：http://qq.szxytkj.cn

print "Hello\n";
来源：http://df.bookmarksfly.cn

[T42] Perl：变量类型
来源：http://my.chemitech.net.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ic.521024.cn

[T43] Perl：字符串插值
来源：http://ve.newstarts.cn

"值: $a"
来源：http://hg.muxihuayi.cn

[T44] Perl：条件
来源：http://md.yuntaijiaju.cn

if ($a > 0) { print "正"; }
来源：http://wp.chemitech.net.cn

[T45] Perl：数组遍历
来源：http://fx.hnjuh.cn

for my $x (@arr) { print $x; }
来源：http://ns.colortex.cn

[T46] Perl：哈希操作
来源：http://km.wgjwhj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tb.shxzukj.cn

[T47] Perl：正则捕获
来源：http://aj.chemitech.net.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://of.lnxyls.cn

[T48] Perl：正则替换
来源：http://sn.haigaiapp.cn

$s =~ s/old/new/g;
来源：http://yd.nszjky.cn

[T49] Perl：函数
来源：http://ad.nicolike.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zh.jctech888.com.cn

[T50] Perl：逐行读文件
来源：http://uh.hnjuh.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fp.hahajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://ep.bookmarksfly.cn

[T51] Scala：Hello World
来源：http://qk.huixiangedu.cn

println("Hello")
来源：http://wt.521024.cn

[T52] Scala：变量
来源：http://wx.bjjhwx.cn

val a = 1;  var b = 2
来源：http://vm.haigaiapp.cn

[T53] Scala：字符串插值
来源：http://lf.jianghongdianzi.cn

s"值: $b"
来源：http://kq.szxytkj.cn

[T54] Scala：集合映射
来源：http://uf.gzmigu.cn

List(1, 2, 3).map(_ * 2)
来源：http://rz.nszjky.cn

[T55] Scala：集合过滤
来源：http://bk.hahajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fr.521024.cn

[T56] Scala：样例类
来源：http://nk.hnjuh.cn

case class User(name: String, age: Int)
来源：http://ps.panjiajie.cn

[T57] Scala：模式匹配
来源：http://yi.szxytkj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://eu.shtwfgs.cn

[T58] Scala：函数定义
来源：http://jp.huixinmuqiang.cn

def add(a: Int, b: Int): Int = a + b
来源：http://to.wgjwhj.cn

[T59] Scala：循环
来源：http://il.panjiajie.cn

for (i <- 1 to 10) println(i)
来源：http://mk.newstarts.cn

[T60] Scala：折叠
来源：http://pl.bookmarksfly.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wb.9csxet.cn

================================================================================
来源：http://pq.shxzukj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mm.lnxyls.cn

================================================================================
来源：http://gz.asd995.cn

[U01] Py：创建虚拟环境
来源：http://yw.jianghongdianzi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cd.jianghongdianzi.cn

[U02] Py：导出 / 安装依赖
来源：http://fp.bjjhwx.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dw.9csxet.cn

[U03] Py：加载 .env 配置
来源：http://xg.huanxung.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://df.huixinmuqiang.cn

[U04] Py：变量调试打印
来源：http://og.szsharing.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rp.colortex.cn

[U05] Py：列表去重且保序
来源：http://ex.bjjhwx.cn

list(dict.fromkeys(arr))
来源：http://by.haigaiapp.cn

[U06] Py：合并两个字典
来源：http://ha.shxzukj.cn

{**a, **b}
来源：http://bq.jianghongdianzi.cn

[U07] Py：反转字典键值
来源：http://pe.haigaiapp.cn

{v: k for k, v in d.items()}
来源：http://rr.yuntaijiaju.cn

[U08] Py：展平二维列表
来源：http://uk.muxihuayi.cn

[y for x in nested for y in x]
来源：http://ei.521024.cn

[U09] Py：字典取最大值的键
来源：http://cj.lnxyls.cn

max(d, key=d.get)
来源：http://cu.bookmarksfly.cn

[U10] Py：按值排序字典
来源：http://fx.9csxet.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://oq.hnjuh.cn

[U11] Py：生成器表达式
来源：http://hq.jctech888.com.cn

(x * 2 for x in arr)
来源：http://jh.colortex.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mi.huixiangedu.cn

Counter(arr).most_common(3)
来源：http://xs.shtwfgs.cn

[U13] Py：固定长度队列
来源：http://ck.huanxung.cn

deque(maxlen=10)
来源：http://wa.hahajie.cn

[U14] Py：分组收集到列表
来源：http://jl.szxytkj.cn

defaultdict(list)
来源：http://zl.yuntaijiaju.cn

[U15] Py：高精度计时
来源：http://yl.nszjky.cn

t = time.perf_counter()
来源：http://mp.shtwfgs.cn

[U16] Py：命令行参数解析
来源：http://hs.huanxung.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://so.newstarts.cn

[U17] Py：初始化日志
来源：http://lv.9csxet.cn

logging.basicConfig(level=logging.INFO)
来源：http://rr.huixiangedu.cn

[U18] Py：预编译正则
来源：http://nc.jianghongdianzi.cn

pat = re.compile(r"\d+")
来源：http://kj.colortex.cn

[U19] Py：正则替换带回调
来源：http://uj.9csxet.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lp.jianghongdianzi.cn

[U20] Py：缓存函数结果
来源：http://bu.huanxung.cn

@functools.lru_cache(maxsize=None)
来源：http://ca.szxytkj.cn

[U21] Py：自定义上下文管理器
来源：http://yw.huanxung.cn

@contextlib.contextmanager
来源：http://qc.wgjwhj.cn

[U22] Py：矩阵转置
来源：http://ul.bookmarksfly.cn

list(zip(*m))
来源：http://co.yuexingan06.cn

[U23] Py：分块读取大文件
来源：http://mm.panjiajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bc.hnjuh.cn

[U24] Py：路径操作
来源：http://to.colortex.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ov.panjiajie.cn

[U25] Py：CSV 按字典读
来源：http://zn.jctech888.com.cn

csv.DictReader(f)
来源：http://in.9csxet.cn

[U26] Py：并发下载
来源：http://mr.muxihuayi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zl.jctech888.com.cn

[U27] Py：异步 HTTP
来源：http://po.muxihuayi.cn

aiohttp.ClientSession() 配合 async with
来源：http://bh.lnxyls.cn

[U28] Py：类型别名
来源：http://qo.asd995.cn

UserId = int
来源：http://ag.huixinmuqiang.cn

[U29] Py：属性校验
来源：http://bo.521024.cn

@property 与 @x.setter 配合
来源：http://xv.9csxet.cn

[U30] Py：数据类
来源：http://ml.yuntaijiaju.cn

@dataclass(slots=True)
来源：http://jr.chemitech.net.cn

[U31] Py：单测
来源：http://yj.muxihuayi.cn

python -m pytest -q
来源：http://mv.asd995.cn

[U32] Py：代码格式化
来源：http://uv.muxihuayi.cn

ruff format . && ruff check --fix .
来源：http://hp.asd995.cn

[U33] Py：打包发布
来源：http://es.colortex.cn

python -m build  （依赖 pyproject.toml）
来源：http://vh.shxzukj.cn

[U34] Py：判断编码
来源：http://gh.huixiangedu.cn

chardet.detect(raw)
来源：http://wq.bjjhwx.cn

[U35] Py：发送邮件
来源：http://qe.hnjuh.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gg.chemitech.net.cn

[U36] Py：定时任务
来源：http://ci.yuexingan06.cn

schedule.every(10).minutes.do(job)
来源：http://ok.lnxyls.cn

[U37] Py：读写 Excel
来源：http://or.haigaiapp.cn

pandas.read_excel / DataFrame.to_excel
来源：http://yj.jianghongdianzi.cn

[U38] Py：获取脚本所在目录
来源：http://oh.hnjuh.cn

Path(__file__).resolve().parent
来源：http://oa.bjjhwx.cn

[U39] Py：判断是否在交互环境
来源：http://gz.panjiajie.cn

sys.stdout.isatty()
来源：http://mi.nicolike.cn

[U40] Py：打印到标准错误
来源：http://kf.huixinmuqiang.cn

print("err", file=sys.stderr)
来源：http://bk.huixiangedu.cn

[U41] PHP：初始化 Composer 项目
来源：http://lj.asd995.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://rd.shxzukj.cn

[U42] PHP：PSR-4 自动加载
来源：http://nk.chemitech.net.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zx.bookmarksfly.cn

[U43] PHP：声明命名空间
来源：http://an.jianghongdianzi.cn

namespace App\Http;
来源：http://ub.gzmigu.cn

[U44] PHP：开启严格类型
来源：http://oa.9csxet.cn

declare(strict_types=1);
来源：http://zd.9csxet.cn

[U45] PHP：类型声明与返回类型
来源：http://wo.wgjwhj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ch.yuntaijiaju.cn

[U46] PHP：可空类型
来源：http://dq.jianghongdianzi.cn

?string $name = null
来源：http://po.shxzukj.cn

[U47] PHP：联合类型
来源：http://yg.muxihuayi.cn

int|string $id
来源：http://ss.hahajie.cn

[U48] PHP：纯枚举
来源：http://gu.huixiangedu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qk.hahajie.cn

[U49] PHP：只读属性
来源：http://po.haigaiapp.cn

public readonly string $name
来源：http://fh.yuntaijiaju.cn

[U50] PHP：构造器属性提升
来源：http://pr.hnjuh.cn

public function __construct(private int $id) {}
来源：http://qx.nszjky.cn

[U51] PHP：数组解构
来源：http://zd.yuntaijiaju.cn

[$a, $b] = $arr;
来源：http://zp.bjjhwx.cn

[U52] PHP：箭头函数
来源：http://dg.nszjky.cn

$double = fn($x) => $x * 2;
来源：http://ng.asd995.cn

[U53] PHP：空合并运算符
来源：http://yl.9csxet.cn

$v = $a ?? $b ?? "default";
来源：http://xi.jctech888.com.cn

[U54] PHP：空安全调用
来源：http://dx.szxytkj.cn

$obj?->method()
来源：http://kj.asd995.cn

[U55] PHP：match 表达式
来源：http://fj.huanxung.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zc.muxihuayi.cn

[U56] PHP：命名参数
来源：http://qx.szxytkj.cn

f(a: 1, b: 2)
来源：http://ic.szxytkj.cn

[U57] PHP：字符串插值
来源：http://rl.chemitech.net.cn

"值: {$a}"
来源：http://ey.yuexingan06.cn

[U58] PHP：数组三件套
来源：http://ge.muxihuayi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jy.colortex.cn

[U59] PHP：自定义排序
来源：http://we.hnjuh.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ki.jianghongdianzi.cn

[U60] PHP：JSON 编解码
来源：http://gu.hnjuh.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://sg.wgjwhj.cn

[U61] PHP：正则
来源：http://hd.haigaiapp.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ja.colortex.cn

[U62] PHP：日期对象
来源：http://kj.muxihuayi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pa.huixinmuqiang.cn

[U63] PHP：文件读写
来源：http://pt.shxzskj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lb.shxzukj.cn

[U64] PHP：目录遍历
来源：http://vm.shtwfgs.cn

glob("dir/*.php");  scandir("dir");
来源：http://ql.chemitech.net.cn

[U65] PHP：会话
来源：http://pi.szxytkj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://oj.hnjuh.cn

[U66] PHP：设置 Cookie
来源：http://no.newstarts.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rt.shxzukj.cn

[U67] PHP：处理文件上传
来源：http://vd.bookmarksfly.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kx.hahajie.cn

[U68] PHP：PDO 连接
来源：http://ry.haigaiapp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tv.jianghongdianzi.cn

[U69] PHP：PDO 预处理
来源：http://bo.9csxet.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rz.nicolike.cn

[U70] PHP：PDO 事务
来源：http://vt.lnxyls.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qk.wgjwhj.cn

[U71] PHP：抛出异常
来源：http://ys.szsharing.cn

throw new RuntimeException("失败", 500);
来源：http://pm.9csxet.cn

[U72] PHP：写错误日志
来源：http://he.szsharing.cn

error_log("失败: " . $e->getMessage());
来源：http://nz.colortex.cn

[U73] PHP：读取 ini 配置
来源：http://oj.yuntaijiaju.cn

parse_ini_file("config.ini", true)
来源：http://pr.szxytkj.cn

[U74] PHP：读取环境变量
来源：http://ab.jctech888.com.cn

getenv("APP_ENV") ?: "production"
来源：http://pz.bookmarksfly.cn

[U75] PHP：依赖注入
来源：http://or.asd995.cn

composer require psr/container
来源：http://sf.bjjhwx.cn

[U76] PHP：简单路由
来源：http://vd.szxytkj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mm.yuexingan06.cn

[U77] PHP：模板渲染
来源：http://aj.shtwfgs.cn

composer require twig/twig
来源：http://cp.szsharing.cn

[U78] PHP：单元测试
来源：http://se.muxihuayi.cn

composer require --dev phpunit/phpunit
来源：http://ii.shxzskj.cn

[U79] PHP：静态分析
来源：http://ny.szxytkj.cn

composer require --dev phpstan/phpstan
来源：http://vj.wgjwhj.cn

[U80] PHP：代码规范修复
来源：http://dn.colortex.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ah.bookmarksfly.cn

[U81] JS：初始化项目
来源：http://dq.huanxung.cn

npm init -y;  npm i express
来源：http://sk.bjjhwx.cn

[U82] JS：package.json 脚本
来源：http://xe.lnxyls.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pd.lnxyls.cn

[U83] JS：ES Module 导入导出
来源：http://ek.gzmigu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qp.bjjhwx.cn

[U84] JS：CommonJS 写法
来源：http://nd.colortex.cn

module.exports = { a };  const { a } = require("./m");
来源：http://fn.shxzukj.cn


<!-- 参考信息 -->