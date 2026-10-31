代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://bf.521024.cn

[S59] C++：静态断言
来源：http://im.521024.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zt.jianghongdianzi.cn

[S60] C++：遍历并删除元素
来源：http://yh.yuexingan06.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://si.shxzukj.cn

================================================================================
来源：http://bz.hnjuh.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ki.nicolike.cn

================================================================================
来源：http://jv.colortex.cn

[T01] Kotlin：Hello World
来源：http://yb.newstarts.cn

println("Hello")
来源：http://xv.chemitech.net.cn

[T02] Kotlin：变量
来源：http://cr.newstarts.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xa.nszjky.cn

[T03] Kotlin：字符串模板
来源：http://yb.shxzskj.cn

"值: $b"
来源：http://ot.muxihuayi.cn

[T04] Kotlin：空安全
来源：http://tf.hnjuh.cn

val n: String? = null;  n?.length
来源：http://pr.shtwfgs.cn

[T05] Kotlin：when 表达式
来源：http://ut.shxzskj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mc.nicolike.cn

[T06] Kotlin：集合映射
来源：http://aw.lnxyls.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://lw.muxihuayi.cn

[T07] Kotlin：集合过滤
来源：http://yi.huixiangedu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tf.hnjuh.cn

[T08] Kotlin：数据类
来源：http://lu.haigaiapp.cn

data class User(val name: String, val age: Int)
来源：http://ek.huixinmuqiang.cn

[T09] Kotlin：扩展函数
来源：http://av.nszjky.cn

fun String.exclaim() = this + "!"
来源：http://av.shtwfgs.cn

[T10] Kotlin：默认参数
来源：http://be.newstarts.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://kz.yuntaijiaju.cn

[T11] Kotlin：协程
来源：http://uc.yuntaijiaju.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://dh.chemitech.net.cn

[T12] Kotlin：解构声明
来源：http://aa.szxytkj.cn

val (a, b) = Pair(1, 2)
来源：http://ib.shxzskj.cn

[T13] Kotlin：只读 Map
来源：http://jp.lnxyls.cn

val m = mapOf("a" to 1)
来源：http://sn.wgjwhj.cn

[T14] Kotlin：循环
来源：http://zo.haigaiapp.cn

for (i in 1..10) println(i)
来源：http://qa.shxzskj.cn

[T15] Kotlin：接口
来源：http://es.muxihuayi.cn

interface Shape { fun area(): Double }
来源：http://fz.huanxung.cn

[T16] Swift：Hello World
来源：http://wp.huixiangedu.cn

print("Hello")
来源：http://xh.szxytkj.cn

[T17] Swift：变量与常量
来源：http://ni.jctech888.com.cn

var a = 1;  let b = 2
来源：http://bs.newstarts.cn

[T18] Swift：字符串插值
来源：http://wk.nicolike.cn

"值: \(b)"
来源：http://ct.9csxet.cn

[T19] Swift：可选绑定
来源：http://ed.nicolike.cn

if let n = opt { print(n) }
来源：http://mf.colortex.cn

[T20] Swift：数组操作
来源：http://bb.shxzukj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://rn.shxzukj.cn

[T21] Swift：遍历
来源：http://zz.gzmigu.cn

for x in a { print(x) }
来源：http://cs.jianghongdianzi.cn

[T22] Swift：字典
来源：http://dj.shxzukj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fe.hahajie.cn

[T23] Swift：函数
来源：http://xf.lnxyls.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jo.chemitech.net.cn

[T24] Swift：闭包
来源：http://kl.lnxyls.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://pv.colortex.cn

[T25] Swift：结构体
来源：http://tt.gzmigu.cn

struct P { var x: Int }
来源：http://pg.muxihuayi.cn

[T26] Swift：类与重写
来源：http://lb.huixiangedu.cn

class A: Base { override func f() {} }
来源：http://mb.newstarts.cn

[T27] Swift：错误处理
来源：http://ee.colortex.cn

do { try f() } catch { print(error) }
来源：http://av.szsharing.cn

[T28] Swift：枚举
来源：http://bt.yuntaijiaju.cn

enum Color { case red, green }
来源：http://bj.lnxyls.cn

[T29] Swift：guard 提前返回
来源：http://ps.newstarts.cn

guard let x = opt else { return }
来源：http://yb.nszjky.cn

[T30] Swift：协议
来源：http://yn.jctech888.com.cn

protocol Shape { func area() -> Double }
来源：http://gu.muxihuayi.cn

[T31] Lua：Hello World
来源：http://qe.huanxung.cn

print("Hello")
来源：http://rh.colortex.cn

[T32] Lua：局部变量
来源：http://is.chemitech.net.cn

local a = 1
来源：http://aq.szxytkj.cn

[T33] Lua：表（数组）
来源：http://yh.jctech888.com.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wt.huixinmuqiang.cn

[T34] Lua：遍历表
来源：http://tm.shxzskj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://lb.shxzukj.cn

[T35] Lua：字典表
来源：http://lz.yuntaijiaju.cn

local d = { a = 1 };  d.b = 2
来源：http://cg.newstarts.cn

[T36] Lua：函数
来源：http://hf.chemitech.net.cn

function add(a, b) return a + b end
来源：http://xy.shxzskj.cn

[T37] Lua：字符串拼接
来源：http://lh.chemitech.net.cn

"a" .. "b"
来源：http://hg.chemitech.net.cn

[T38] Lua：条件
来源：http://sd.hahajie.cn

if x > 0 then print("正") end
来源：http://uf.gzmigu.cn

[T39] Lua：模式匹配
来源：http://lm.colortex.cn

string.find(s, "%d+")
来源：http://rc.lnxyls.cn

[T40] Lua：元表
来源：http://tf.hahajie.cn

setmetatable({}, { __index = base })
来源：http://ib.chemitech.net.cn

[T41] Perl：Hello World
来源：http://og.szxytkj.cn

print "Hello\n";
来源：http://la.chemitech.net.cn

[T42] Perl：变量类型
来源：http://ct.9csxet.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://eo.lnxyls.cn

[T43] Perl：字符串插值
来源：http://qe.shxzskj.cn

"值: $a"
来源：http://bk.newstarts.cn

[T44] Perl：条件
来源：http://qz.huixinmuqiang.cn

if ($a > 0) { print "正"; }
来源：http://jx.521024.cn

[T45] Perl：数组遍历
来源：http://vf.lnxyls.cn

for my $x (@arr) { print $x; }
来源：http://vx.shxzukj.cn

[T46] Perl：哈希操作
来源：http://pt.chemitech.net.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wk.shtwfgs.cn

[T47] Perl：正则捕获
来源：http://ij.wgjwhj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://zl.shxzskj.cn

[T48] Perl：正则替换
来源：http://fl.shxzskj.cn

$s =~ s/old/new/g;
来源：http://xi.szxytkj.cn

[T49] Perl：函数
来源：http://yr.521024.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vv.colortex.cn

[T50] Perl：逐行读文件
来源：http://ac.9csxet.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://hv.shtwfgs.cn

while (my $line = <$fh>) { print $line; }
来源：http://il.9csxet.cn

[T51] Scala：Hello World
来源：http://dv.panjiajie.cn

println("Hello")
来源：http://er.shxzskj.cn

[T52] Scala：变量
来源：http://hg.szsharing.cn

val a = 1;  var b = 2
来源：http://pt.hnjuh.cn

[T53] Scala：字符串插值
来源：http://lt.shtwfgs.cn

s"值: $b"
来源：http://zf.huixiangedu.cn

[T54] Scala：集合映射
来源：http://bj.shxzukj.cn

List(1, 2, 3).map(_ * 2)
来源：http://vh.521024.cn

[T55] Scala：集合过滤
来源：http://ea.szsharing.cn

List(1, 2, 3).filter(_ > 1)
来源：http://jm.newstarts.cn

[T56] Scala：样例类
来源：http://an.muxihuayi.cn

case class User(name: String, age: Int)
来源：http://me.haigaiapp.cn

[T57] Scala：模式匹配
来源：http://kl.jctech888.com.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://sc.521024.cn

[T58] Scala：函数定义
来源：http://gl.9csxet.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fp.shxzukj.cn

[T59] Scala：循环
来源：http://vp.newstarts.cn

for (i <- 1 to 10) println(i)
来源：http://oc.hahajie.cn

[T60] Scala：折叠
来源：http://js.nicolike.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://br.shxzskj.cn

================================================================================
来源：http://ut.panjiajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dh.hnjuh.cn

================================================================================
来源：http://ye.yuexingan06.cn

[U01] Py：创建虚拟环境
来源：http://hi.colortex.cn

python -m venv .venv && source .venv/bin/activate
来源：http://fn.huanxung.cn

[U02] Py：导出 / 安装依赖
来源：http://vb.szxytkj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dx.shxzukj.cn

[U03] Py：加载 .env 配置
来源：http://ck.huixinmuqiang.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://dr.yuexingan06.cn

[U04] Py：变量调试打印
来源：http://lu.bookmarksfly.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jb.nszjky.cn

[U05] Py：列表去重且保序
来源：http://es.chemitech.net.cn

list(dict.fromkeys(arr))
来源：http://ur.yuexingan06.cn

[U06] Py：合并两个字典
来源：http://gu.haigaiapp.cn

{**a, **b}
来源：http://cj.yuexingan06.cn

[U07] Py：反转字典键值
来源：http://ep.9csxet.cn

{v: k for k, v in d.items()}
来源：http://az.huanxung.cn

[U08] Py：展平二维列表
来源：http://tr.521024.cn

[y for x in nested for y in x]
来源：http://cu.shtwfgs.cn

[U09] Py：字典取最大值的键
来源：http://lj.colortex.cn

max(d, key=d.get)
来源：http://sk.hahajie.cn

[U10] Py：按值排序字典
来源：http://mk.shxzukj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://eq.521024.cn

[U11] Py：生成器表达式
来源：http://cs.haigaiapp.cn

(x * 2 for x in arr)
来源：http://ke.bjjhwx.cn

[U12] Py：取出现最多的 3 个元素
来源：http://bm.shxzukj.cn

Counter(arr).most_common(3)
来源：http://ht.yuntaijiaju.cn

[U13] Py：固定长度队列
来源：http://sf.521024.cn

deque(maxlen=10)
来源：http://oy.hahajie.cn

[U14] Py：分组收集到列表
来源：http://qr.panjiajie.cn

defaultdict(list)
来源：http://tb.jianghongdianzi.cn

[U15] Py：高精度计时
来源：http://cc.szxytkj.cn

t = time.perf_counter()
来源：http://gf.nszjky.cn

[U16] Py：命令行参数解析
来源：http://cc.chemitech.net.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hw.wgjwhj.cn

[U17] Py：初始化日志
来源：http://ht.gzmigu.cn

logging.basicConfig(level=logging.INFO)
来源：http://eo.chemitech.net.cn

[U18] Py：预编译正则
来源：http://kh.bookmarksfly.cn

pat = re.compile(r"\d+")
来源：http://oh.shxzukj.cn

[U19] Py：正则替换带回调
来源：http://il.lnxyls.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dt.bjjhwx.cn

[U20] Py：缓存函数结果
来源：http://xj.huanxung.cn

@functools.lru_cache(maxsize=None)
来源：http://bs.9csxet.cn

[U21] Py：自定义上下文管理器
来源：http://gk.shtwfgs.cn

@contextlib.contextmanager
来源：http://wu.lnxyls.cn

[U22] Py：矩阵转置
来源：http://kj.shtwfgs.cn

list(zip(*m))
来源：http://tx.panjiajie.cn

[U23] Py：分块读取大文件
来源：http://ox.hnjuh.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gx.lnxyls.cn

[U24] Py：路径操作
来源：http://rx.lnxyls.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bc.szsharing.cn

[U25] Py：CSV 按字典读
来源：http://gq.panjiajie.cn

csv.DictReader(f)
来源：http://zw.gzmigu.cn

[U26] Py：并发下载
来源：http://cr.huanxung.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://df.521024.cn

[U27] Py：异步 HTTP
来源：http://mg.nicolike.cn

aiohttp.ClientSession() 配合 async with
来源：http://kx.lnxyls.cn

[U28] Py：类型别名
来源：http://hx.asd995.cn

UserId = int
来源：http://zs.muxihuayi.cn

[U29] Py：属性校验
来源：http://wg.shxzukj.cn

@property 与 @x.setter 配合
来源：http://ui.muxihuayi.cn

[U30] Py：数据类
来源：http://px.panjiajie.cn

@dataclass(slots=True)
来源：http://kv.huanxung.cn

[U31] Py：单测
来源：http://va.521024.cn

python -m pytest -q
来源：http://fu.huixinmuqiang.cn

[U32] Py：代码格式化
来源：http://gf.lnxyls.cn

ruff format . && ruff check --fix .
来源：http://je.bjjhwx.cn

[U33] Py：打包发布
来源：http://jz.nicolike.cn

python -m build  （依赖 pyproject.toml）
来源：http://xx.nszjky.cn

[U34] Py：判断编码
来源：http://ue.hnjuh.cn

chardet.detect(raw)
来源：http://zd.huixinmuqiang.cn

[U35] Py：发送邮件
来源：http://rz.wgjwhj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nk.huanxung.cn

[U36] Py：定时任务
来源：http://kt.newstarts.cn

schedule.every(10).minutes.do(job)
来源：http://ou.yuntaijiaju.cn

[U37] Py：读写 Excel
来源：http://qy.lnxyls.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ie.yuntaijiaju.cn

[U38] Py：获取脚本所在目录
来源：http://vp.huixinmuqiang.cn

Path(__file__).resolve().parent
来源：http://jm.asd995.cn

[U39] Py：判断是否在交互环境
来源：http://vq.bjjhwx.cn

sys.stdout.isatty()
来源：http://me.jctech888.com.cn

[U40] Py：打印到标准错误
来源：http://tc.wgjwhj.cn

print("err", file=sys.stderr)
来源：http://mn.szxytkj.cn

[U41] PHP：初始化 Composer 项目
来源：http://wk.jianghongdianzi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://vq.haigaiapp.cn

[U42] PHP：PSR-4 自动加载
来源：http://cx.hnjuh.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zy.gzmigu.cn

[U43] PHP：声明命名空间
来源：http://oe.huixinmuqiang.cn

namespace App\Http;
来源：http://jo.yuexingan06.cn

[U44] PHP：开启严格类型
来源：http://dt.huanxung.cn

declare(strict_types=1);
来源：http://wa.nszjky.cn

[U45] PHP：类型声明与返回类型
来源：http://vm.yuexingan06.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://wa.huixinmuqiang.cn

[U46] PHP：可空类型
来源：http://hd.9csxet.cn

?string $name = null
来源：http://ph.szxytkj.cn

[U47] PHP：联合类型
来源：http://nk.nicolike.cn

int|string $id
来源：http://cm.asd995.cn

[U48] PHP：纯枚举
来源：http://bn.yuexingan06.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bo.hahajie.cn

[U49] PHP：只读属性
来源：http://mc.nicolike.cn

public readonly string $name
来源：http://nz.huanxung.cn

[U50] PHP：构造器属性提升
来源：http://ci.szsharing.cn

public function __construct(private int $id) {}
来源：http://ci.panjiajie.cn

[U51] PHP：数组解构
来源：http://hk.nicolike.cn

[$a, $b] = $arr;
来源：http://cj.jianghongdianzi.cn

[U52] PHP：箭头函数
来源：http://kw.wgjwhj.cn

$double = fn($x) => $x * 2;
来源：http://th.yuntaijiaju.cn

[U53] PHP：空合并运算符
来源：http://ps.shxzskj.cn

$v = $a ?? $b ?? "default";
来源：http://pg.asd995.cn

[U54] PHP：空安全调用
来源：http://wq.bjjhwx.cn

$obj?->method()
来源：http://fi.9csxet.cn

[U55] PHP：match 表达式
来源：http://ef.panjiajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qd.shxzukj.cn

[U56] PHP：命名参数
来源：http://jl.nszjky.cn

f(a: 1, b: 2)
来源：http://xg.lnxyls.cn

[U57] PHP：字符串插值
来源：http://zr.gzmigu.cn

"值: {$a}"
来源：http://gq.szxytkj.cn

[U58] PHP：数组三件套
来源：http://md.yuexingan06.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bt.jctech888.com.cn

[U59] PHP：自定义排序
来源：http://xs.chemitech.net.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gx.shtwfgs.cn

[U60] PHP：JSON 编解码
来源：http://yg.szsharing.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ne.haigaiapp.cn

[U61] PHP：正则
来源：http://dk.wgjwhj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xn.asd995.cn

[U62] PHP：日期对象
来源：http://wb.bjjhwx.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pv.szsharing.cn

[U63] PHP：文件读写
来源：http://xp.panjiajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pn.szsharing.cn

[U64] PHP：目录遍历
来源：http://ze.shxzukj.cn

glob("dir/*.php");  scandir("dir");
来源：http://rz.bjjhwx.cn

[U65] PHP：会话
来源：http://kq.haigaiapp.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://fi.nicolike.cn

[U66] PHP：设置 Cookie
来源：http://au.wgjwhj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yf.haigaiapp.cn

[U67] PHP：处理文件上传
来源：http://vk.shxzukj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cj.jianghongdianzi.cn

[U68] PHP：PDO 连接
来源：http://ds.huixiangedu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yz.muxihuayi.cn

[U69] PHP：PDO 预处理
来源：http://bc.nszjky.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vw.newstarts.cn

[U70] PHP：PDO 事务
来源：http://iz.9csxet.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ht.gzmigu.cn

[U71] PHP：抛出异常
来源：http://by.bookmarksfly.cn

throw new RuntimeException("失败", 500);
来源：http://ol.szsharing.cn

[U72] PHP：写错误日志
来源：http://pa.hnjuh.cn

error_log("失败: " . $e->getMessage());
来源：http://ry.yuexingan06.cn

[U73] PHP：读取 ini 配置
来源：http://qf.newstarts.cn

parse_ini_file("config.ini", true)
来源：http://al.jctech888.com.cn

[U74] PHP：读取环境变量
来源：http://hk.haigaiapp.cn

getenv("APP_ENV") ?: "production"
来源：http://qq.newstarts.cn

[U75] PHP：依赖注入
来源：http://yf.jianghongdianzi.cn

composer require psr/container
来源：http://ng.szsharing.cn

[U76] PHP：简单路由
来源：http://vn.bjjhwx.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cg.521024.cn

[U77] PHP：模板渲染
来源：http://wb.shxzskj.cn

composer require twig/twig
来源：http://ah.hahajie.cn

[U78] PHP：单元测试
来源：http://qc.521024.cn

composer require --dev phpunit/phpunit
来源：http://xw.521024.cn

[U79] PHP：静态分析
来源：http://ve.muxihuayi.cn

composer require --dev phpstan/phpstan
来源：http://lr.521024.cn

[U80] PHP：代码规范修复
来源：http://wo.shtwfgs.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ct.hahajie.cn

[U81] JS：初始化项目
来源：http://kx.szxytkj.cn

npm init -y;  npm i express
来源：http://kq.bjjhwx.cn

[U82] JS：package.json 脚本
来源：http://yc.shxzskj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://oy.jctech888.com.cn

[U83] JS：ES Module 导入导出
来源：http://qy.bookmarksfly.cn

export const a = 1;  import { a } from "./m.js";
来源：http://pw.huixiangedu.cn

[U84] JS：CommonJS 写法
来源：http://vt.nszjky.cn

module.exports = { a };  const { a } = require("./m");
来源：http://kv.huixinmuqiang.cn


<!-- 参考信息 -->