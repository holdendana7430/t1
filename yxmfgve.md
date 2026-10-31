代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vj.9csxet.cn

[S57] C++：编译期常量
来源：http://vs.gzmigu.cn

constexpr int N = 10;
来源：http://fk.szxytkj.cn

[S58] C++：命名空间
来源：http://ui.nszjky.cn

namespace ns { int f() { return 1; } }
来源：http://ji.huixiangedu.cn

[S59] C++：静态断言
来源：http://xj.asd995.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zn.bookmarksfly.cn

[S60] C++：遍历并删除元素
来源：http://vp.szsharing.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://af.521024.cn

================================================================================
来源：http://bw.chemitech.net.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://as.9csxet.cn

================================================================================
来源：http://qk.yuexingan06.cn

[T01] Kotlin：Hello World
来源：http://ep.szxytkj.cn

println("Hello")
来源：http://ix.chemitech.net.cn

[T02] Kotlin：变量
来源：http://mw.haigaiapp.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ey.hahajie.cn

[T03] Kotlin：字符串模板
来源：http://oo.szsharing.cn

"值: $b"
来源：http://ox.hnjuh.cn

[T04] Kotlin：空安全
来源：http://qm.yuntaijiaju.cn

val n: String? = null;  n?.length
来源：http://yo.huixiangedu.cn

[T05] Kotlin：when 表达式
来源：http://ae.asd995.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bq.gzmigu.cn

[T06] Kotlin：集合映射
来源：http://cd.jctech888.com.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://mx.shxzukj.cn

[T07] Kotlin：集合过滤
来源：http://tp.yuntaijiaju.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://kj.huanxung.cn

[T08] Kotlin：数据类
来源：http://cb.muxihuayi.cn

data class User(val name: String, val age: Int)
来源：http://cu.asd995.cn

[T09] Kotlin：扩展函数
来源：http://al.huanxung.cn

fun String.exclaim() = this + "!"
来源：http://kh.muxihuayi.cn

[T10] Kotlin：默认参数
来源：http://xz.nicolike.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ij.jctech888.com.cn

[T11] Kotlin：协程
来源：http://xx.huanxung.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://rd.521024.cn

[T12] Kotlin：解构声明
来源：http://ss.yuexingan06.cn

val (a, b) = Pair(1, 2)
来源：http://as.shtwfgs.cn

[T13] Kotlin：只读 Map
来源：http://eq.huanxung.cn

val m = mapOf("a" to 1)
来源：http://kd.asd995.cn

[T14] Kotlin：循环
来源：http://oc.panjiajie.cn

for (i in 1..10) println(i)
来源：http://ul.hahajie.cn

[T15] Kotlin：接口
来源：http://bb.hahajie.cn

interface Shape { fun area(): Double }
来源：http://ok.szxytkj.cn

[T16] Swift：Hello World
来源：http://zr.jctech888.com.cn

print("Hello")
来源：http://rt.haigaiapp.cn

[T17] Swift：变量与常量
来源：http://yt.yuntaijiaju.cn

var a = 1;  let b = 2
来源：http://qj.shtwfgs.cn

[T18] Swift：字符串插值
来源：http://fm.chemitech.net.cn

"值: \(b)"
来源：http://ah.bookmarksfly.cn

[T19] Swift：可选绑定
来源：http://zk.shxzskj.cn

if let n = opt { print(n) }
来源：http://fz.bookmarksfly.cn

[T20] Swift：数组操作
来源：http://rp.hahajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://tn.chemitech.net.cn

[T21] Swift：遍历
来源：http://mo.shxzukj.cn

for x in a { print(x) }
来源：http://yy.haigaiapp.cn

[T22] Swift：字典
来源：http://fh.newstarts.cn

var d = ["a": 1];  d["b"] = 2
来源：http://or.muxihuayi.cn

[T23] Swift：函数
来源：http://gl.lnxyls.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hs.panjiajie.cn

[T24] Swift：闭包
来源：http://ey.shxzskj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://sn.nicolike.cn

[T25] Swift：结构体
来源：http://kq.huixinmuqiang.cn

struct P { var x: Int }
来源：http://el.szsharing.cn

[T26] Swift：类与重写
来源：http://jh.jctech888.com.cn

class A: Base { override func f() {} }
来源：http://de.huanxung.cn

[T27] Swift：错误处理
来源：http://zv.jianghongdianzi.cn

do { try f() } catch { print(error) }
来源：http://sl.nicolike.cn

[T28] Swift：枚举
来源：http://qi.yuexingan06.cn

enum Color { case red, green }
来源：http://un.521024.cn

[T29] Swift：guard 提前返回
来源：http://kx.wgjwhj.cn

guard let x = opt else { return }
来源：http://jx.shtwfgs.cn

[T30] Swift：协议
来源：http://dt.bjjhwx.cn

protocol Shape { func area() -> Double }
来源：http://yy.newstarts.cn

[T31] Lua：Hello World
来源：http://iy.bjjhwx.cn

print("Hello")
来源：http://gy.huixinmuqiang.cn

[T32] Lua：局部变量
来源：http://gm.9csxet.cn

local a = 1
来源：http://dl.muxihuayi.cn

[T33] Lua：表（数组）
来源：http://gr.shxzukj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vx.9csxet.cn

[T34] Lua：遍历表
来源：http://op.yuntaijiaju.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rd.521024.cn

[T35] Lua：字典表
来源：http://vd.shxzskj.cn

local d = { a = 1 };  d.b = 2
来源：http://pc.huixinmuqiang.cn

[T36] Lua：函数
来源：http://xe.nszjky.cn

function add(a, b) return a + b end
来源：http://xs.yuntaijiaju.cn

[T37] Lua：字符串拼接
来源：http://fe.wgjwhj.cn

"a" .. "b"
来源：http://ml.muxihuayi.cn

[T38] Lua：条件
来源：http://cx.yuntaijiaju.cn

if x > 0 then print("正") end
来源：http://td.panjiajie.cn

[T39] Lua：模式匹配
来源：http://pg.huanxung.cn

string.find(s, "%d+")
来源：http://zz.yuexingan06.cn

[T40] Lua：元表
来源：http://au.shtwfgs.cn

setmetatable({}, { __index = base })
来源：http://yi.huanxung.cn

[T41] Perl：Hello World
来源：http://oj.shtwfgs.cn

print "Hello\n";
来源：http://ba.gzmigu.cn

[T42] Perl：变量类型
来源：http://vb.szsharing.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mb.szxytkj.cn

[T43] Perl：字符串插值
来源：http://fp.hnjuh.cn

"值: $a"
来源：http://tr.szxytkj.cn

[T44] Perl：条件
来源：http://la.huixiangedu.cn

if ($a > 0) { print "正"; }
来源：http://qt.lnxyls.cn

[T45] Perl：数组遍历
来源：http://ta.colortex.cn

for my $x (@arr) { print $x; }
来源：http://al.gzmigu.cn

[T46] Perl：哈希操作
来源：http://if.huixinmuqiang.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uh.yuexingan06.cn

[T47] Perl：正则捕获
来源：http://dc.shxzskj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://fv.wgjwhj.cn

[T48] Perl：正则替换
来源：http://us.colortex.cn

$s =~ s/old/new/g;
来源：http://vp.jianghongdianzi.cn

[T49] Perl：函数
来源：http://se.huanxung.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://eh.shtwfgs.cn

[T50] Perl：逐行读文件
来源：http://vd.bjjhwx.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rd.colortex.cn

while (my $line = <$fh>) { print $line; }
来源：http://ab.lnxyls.cn

[T51] Scala：Hello World
来源：http://sg.wgjwhj.cn

println("Hello")
来源：http://se.shtwfgs.cn

[T52] Scala：变量
来源：http://wn.huixinmuqiang.cn

val a = 1;  var b = 2
来源：http://mn.szxytkj.cn

[T53] Scala：字符串插值
来源：http://sn.jctech888.com.cn

s"值: $b"
来源：http://uy.bjjhwx.cn

[T54] Scala：集合映射
来源：http://ye.shtwfgs.cn

List(1, 2, 3).map(_ * 2)
来源：http://da.jianghongdianzi.cn

[T55] Scala：集合过滤
来源：http://ho.panjiajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://bn.yuntaijiaju.cn

[T56] Scala：样例类
来源：http://iq.szsharing.cn

case class User(name: String, age: Int)
来源：http://db.shxzskj.cn

[T57] Scala：模式匹配
来源：http://en.hahajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fe.jianghongdianzi.cn

[T58] Scala：函数定义
来源：http://hf.hahajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://pi.hahajie.cn

[T59] Scala：循环
来源：http://eq.yuntaijiaju.cn

for (i <- 1 to 10) println(i)
来源：http://ph.wgjwhj.cn

[T60] Scala：折叠
来源：http://ad.bookmarksfly.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wi.jctech888.com.cn

================================================================================
来源：http://gb.shtwfgs.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nx.panjiajie.cn

================================================================================
来源：http://xd.muxihuayi.cn

[U01] Py：创建虚拟环境
来源：http://ko.shxzukj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://uw.bookmarksfly.cn

[U02] Py：导出 / 安装依赖
来源：http://by.asd995.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nt.shxzukj.cn

[U03] Py：加载 .env 配置
来源：http://rj.huanxung.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rk.yuntaijiaju.cn

[U04] Py：变量调试打印
来源：http://lh.bjjhwx.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://si.szsharing.cn

[U05] Py：列表去重且保序
来源：http://aj.9csxet.cn

list(dict.fromkeys(arr))
来源：http://fa.newstarts.cn

[U06] Py：合并两个字典
来源：http://ye.nicolike.cn

{**a, **b}
来源：http://nv.jianghongdianzi.cn

[U07] Py：反转字典键值
来源：http://zc.shtwfgs.cn

{v: k for k, v in d.items()}
来源：http://kt.bookmarksfly.cn

[U08] Py：展平二维列表
来源：http://rg.lnxyls.cn

[y for x in nested for y in x]
来源：http://uy.huanxung.cn

[U09] Py：字典取最大值的键
来源：http://cl.szxytkj.cn

max(d, key=d.get)
来源：http://cl.nicolike.cn

[U10] Py：按值排序字典
来源：http://vu.shtwfgs.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qd.bookmarksfly.cn

[U11] Py：生成器表达式
来源：http://qv.huanxung.cn

(x * 2 for x in arr)
来源：http://kq.panjiajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zx.haigaiapp.cn

Counter(arr).most_common(3)
来源：http://vo.haigaiapp.cn

[U13] Py：固定长度队列
来源：http://cn.huanxung.cn

deque(maxlen=10)
来源：http://oe.9csxet.cn

[U14] Py：分组收集到列表
来源：http://mc.hnjuh.cn

defaultdict(list)
来源：http://ln.asd995.cn

[U15] Py：高精度计时
来源：http://on.chemitech.net.cn

t = time.perf_counter()
来源：http://xh.hahajie.cn

[U16] Py：命令行参数解析
来源：http://yt.9csxet.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kb.9csxet.cn

[U17] Py：初始化日志
来源：http://xx.jianghongdianzi.cn

logging.basicConfig(level=logging.INFO)
来源：http://gh.haigaiapp.cn

[U18] Py：预编译正则
来源：http://hi.hnjuh.cn

pat = re.compile(r"\d+")
来源：http://bv.huixinmuqiang.cn

[U19] Py：正则替换带回调
来源：http://fy.haigaiapp.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ur.shxzskj.cn

[U20] Py：缓存函数结果
来源：http://qa.wgjwhj.cn

@functools.lru_cache(maxsize=None)
来源：http://ym.panjiajie.cn

[U21] Py：自定义上下文管理器
来源：http://kk.wgjwhj.cn

@contextlib.contextmanager
来源：http://zl.panjiajie.cn

[U22] Py：矩阵转置
来源：http://cf.yuexingan06.cn

list(zip(*m))
来源：http://db.nszjky.cn

[U23] Py：分块读取大文件
来源：http://uz.haigaiapp.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://kl.bjjhwx.cn

[U24] Py：路径操作
来源：http://qx.hahajie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hy.gzmigu.cn

[U25] Py：CSV 按字典读
来源：http://af.chemitech.net.cn

csv.DictReader(f)
来源：http://gp.chemitech.net.cn

[U26] Py：并发下载
来源：http://vt.jianghongdianzi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://we.shxzukj.cn

[U27] Py：异步 HTTP
来源：http://ww.bjjhwx.cn

aiohttp.ClientSession() 配合 async with
来源：http://vc.shxzskj.cn

[U28] Py：类型别名
来源：http://dw.yuexingan06.cn

UserId = int
来源：http://te.bjjhwx.cn

[U29] Py：属性校验
来源：http://sj.panjiajie.cn

@property 与 @x.setter 配合
来源：http://dv.shxzskj.cn

[U30] Py：数据类
来源：http://ed.521024.cn

@dataclass(slots=True)
来源：http://nl.asd995.cn

[U31] Py：单测
来源：http://he.bookmarksfly.cn

python -m pytest -q
来源：http://zw.bookmarksfly.cn

[U32] Py：代码格式化
来源：http://ob.newstarts.cn

ruff format . && ruff check --fix .
来源：http://zt.haigaiapp.cn

[U33] Py：打包发布
来源：http://ar.gzmigu.cn

python -m build  （依赖 pyproject.toml）
来源：http://il.gzmigu.cn

[U34] Py：判断编码
来源：http://gb.wgjwhj.cn

chardet.detect(raw)
来源：http://ca.shxzukj.cn

[U35] Py：发送邮件
来源：http://if.shxzukj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nx.521024.cn

[U36] Py：定时任务
来源：http://wb.chemitech.net.cn

schedule.every(10).minutes.do(job)
来源：http://in.jctech888.com.cn

[U37] Py：读写 Excel
来源：http://um.newstarts.cn

pandas.read_excel / DataFrame.to_excel
来源：http://iy.bookmarksfly.cn

[U38] Py：获取脚本所在目录
来源：http://ya.huixinmuqiang.cn

Path(__file__).resolve().parent
来源：http://oq.9csxet.cn

[U39] Py：判断是否在交互环境
来源：http://ic.yuexingan06.cn

sys.stdout.isatty()
来源：http://oo.bookmarksfly.cn

[U40] Py：打印到标准错误
来源：http://yx.szsharing.cn

print("err", file=sys.stderr)
来源：http://af.chemitech.net.cn

[U41] PHP：初始化 Composer 项目
来源：http://pu.asd995.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jp.huixiangedu.cn

[U42] PHP：PSR-4 自动加载
来源：http://nm.wgjwhj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ts.bookmarksfly.cn

[U43] PHP：声明命名空间
来源：http://au.jianghongdianzi.cn

namespace App\Http;
来源：http://bg.nicolike.cn

[U44] PHP：开启严格类型
来源：http://sh.newstarts.cn

declare(strict_types=1);
来源：http://fs.bjjhwx.cn

[U45] PHP：类型声明与返回类型
来源：http://mz.haigaiapp.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://dh.yuexingan06.cn

[U46] PHP：可空类型
来源：http://vi.newstarts.cn

?string $name = null
来源：http://eq.wgjwhj.cn

[U47] PHP：联合类型
来源：http://ls.colortex.cn

int|string $id
来源：http://jo.bookmarksfly.cn

[U48] PHP：纯枚举
来源：http://gp.hahajie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xe.9csxet.cn

[U49] PHP：只读属性
来源：http://fx.huanxung.cn

public readonly string $name
来源：http://jj.yuntaijiaju.cn

[U50] PHP：构造器属性提升
来源：http://og.wgjwhj.cn

public function __construct(private int $id) {}
来源：http://yc.jctech888.com.cn

[U51] PHP：数组解构
来源：http://kb.chemitech.net.cn

[$a, $b] = $arr;
来源：http://ej.huixiangedu.cn

[U52] PHP：箭头函数
来源：http://hd.lnxyls.cn

$double = fn($x) => $x * 2;
来源：http://ov.gzmigu.cn

[U53] PHP：空合并运算符
来源：http://oi.shxzskj.cn

$v = $a ?? $b ?? "default";
来源：http://ja.panjiajie.cn

[U54] PHP：空安全调用
来源：http://rz.yuexingan06.cn

$obj?->method()
来源：http://sr.9csxet.cn

[U55] PHP：match 表达式
来源：http://mo.9csxet.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yi.panjiajie.cn

[U56] PHP：命名参数
来源：http://mo.jianghongdianzi.cn

f(a: 1, b: 2)
来源：http://ye.muxihuayi.cn

[U57] PHP：字符串插值
来源：http://if.huanxung.cn

"值: {$a}"
来源：http://xu.muxihuayi.cn

[U58] PHP：数组三件套
来源：http://bh.muxihuayi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qh.jianghongdianzi.cn

[U59] PHP：自定义排序
来源：http://so.lnxyls.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xn.bookmarksfly.cn

[U60] PHP：JSON 编解码
来源：http://pn.nszjky.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jg.bjjhwx.cn

[U61] PHP：正则
来源：http://mj.muxihuayi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ms.nicolike.cn

[U62] PHP：日期对象
来源：http://aa.huixinmuqiang.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://aa.hahajie.cn

[U63] PHP：文件读写
来源：http://li.szsharing.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mv.hnjuh.cn

[U64] PHP：目录遍历
来源：http://ah.colortex.cn

glob("dir/*.php");  scandir("dir");
来源：http://zt.jianghongdianzi.cn

[U65] PHP：会话
来源：http://lr.huixinmuqiang.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://tk.yuntaijiaju.cn

[U66] PHP：设置 Cookie
来源：http://rz.521024.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ur.shxzukj.cn

[U67] PHP：处理文件上传
来源：http://dt.hnjuh.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fx.hnjuh.cn

[U68] PHP：PDO 连接
来源：http://db.asd995.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gl.szsharing.cn

[U69] PHP：PDO 预处理
来源：http://ok.muxihuayi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ke.jianghongdianzi.cn

[U70] PHP：PDO 事务
来源：http://sd.newstarts.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zo.yuntaijiaju.cn

[U71] PHP：抛出异常
来源：http://my.521024.cn

throw new RuntimeException("失败", 500);
来源：http://az.shxzukj.cn

[U72] PHP：写错误日志
来源：http://sp.bjjhwx.cn

error_log("失败: " . $e->getMessage());
来源：http://iv.9csxet.cn

[U73] PHP：读取 ini 配置
来源：http://jk.huixinmuqiang.cn

parse_ini_file("config.ini", true)
来源：http://nq.521024.cn

[U74] PHP：读取环境变量
来源：http://tw.yuexingan06.cn

getenv("APP_ENV") ?: "production"
来源：http://am.521024.cn

[U75] PHP：依赖注入
来源：http://ke.jianghongdianzi.cn

composer require psr/container
来源：http://ng.chemitech.net.cn

[U76] PHP：简单路由
来源：http://rk.shxzskj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://oe.yuexingan06.cn

[U77] PHP：模板渲染
来源：http://gl.521024.cn

composer require twig/twig
来源：http://mb.jctech888.com.cn

[U78] PHP：单元测试
来源：http://qk.asd995.cn

composer require --dev phpunit/phpunit
来源：http://mq.huixiangedu.cn

[U79] PHP：静态分析
来源：http://zd.shxzskj.cn

composer require --dev phpstan/phpstan
来源：http://zc.shtwfgs.cn

[U80] PHP：代码规范修复
来源：http://op.lnxyls.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://dw.muxihuayi.cn

[U81] JS：初始化项目
来源：http://os.huixiangedu.cn

npm init -y;  npm i express
来源：http://ha.wgjwhj.cn

[U82] JS：package.json 脚本
来源：http://qv.panjiajie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yz.gzmigu.cn


<!-- 参考信息 -->