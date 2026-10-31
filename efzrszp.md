代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cb.gzmigu.cn

[S57] C++：编译期常量
来源：http://uc.colortex.cn

constexpr int N = 10;
来源：http://xz.chemitech.net.cn

[S58] C++：命名空间
来源：http://ba.panjiajie.cn

namespace ns { int f() { return 1; } }
来源：http://up.chemitech.net.cn

[S59] C++：静态断言
来源：http://uh.bjjhwx.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gf.asd995.cn

[S60] C++：遍历并删除元素
来源：http://aa.yuntaijiaju.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rh.hahajie.cn

================================================================================
来源：http://zq.huixiangedu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ji.huanxung.cn

================================================================================
来源：http://ep.szsharing.cn

[T01] Kotlin：Hello World
来源：http://bp.521024.cn

println("Hello")
来源：http://nj.nszjky.cn

[T02] Kotlin：变量
来源：http://fz.9csxet.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jv.huixinmuqiang.cn

[T03] Kotlin：字符串模板
来源：http://iy.521024.cn

"值: $b"
来源：http://pf.panjiajie.cn

[T04] Kotlin：空安全
来源：http://ev.yuexingan06.cn

val n: String? = null;  n?.length
来源：http://ph.huixinmuqiang.cn

[T05] Kotlin：when 表达式
来源：http://mw.huanxung.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jl.gzmigu.cn

[T06] Kotlin：集合映射
来源：http://qf.nicolike.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ch.bjjhwx.cn

[T07] Kotlin：集合过滤
来源：http://ek.yuexingan06.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://eh.jianghongdianzi.cn

[T08] Kotlin：数据类
来源：http://nc.huixiangedu.cn

data class User(val name: String, val age: Int)
来源：http://lu.nicolike.cn

[T09] Kotlin：扩展函数
来源：http://hl.newstarts.cn

fun String.exclaim() = this + "!"
来源：http://hu.yuexingan06.cn

[T10] Kotlin：默认参数
来源：http://bh.asd995.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://la.yuntaijiaju.cn

[T11] Kotlin：协程
来源：http://vv.wgjwhj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xq.shtwfgs.cn

[T12] Kotlin：解构声明
来源：http://jv.bjjhwx.cn

val (a, b) = Pair(1, 2)
来源：http://rp.bjjhwx.cn

[T13] Kotlin：只读 Map
来源：http://eh.shxzskj.cn

val m = mapOf("a" to 1)
来源：http://mg.bjjhwx.cn

[T14] Kotlin：循环
来源：http://od.szxytkj.cn

for (i in 1..10) println(i)
来源：http://lv.colortex.cn

[T15] Kotlin：接口
来源：http://np.yuntaijiaju.cn

interface Shape { fun area(): Double }
来源：http://hk.huixinmuqiang.cn

[T16] Swift：Hello World
来源：http://fb.nicolike.cn

print("Hello")
来源：http://il.szsharing.cn

[T17] Swift：变量与常量
来源：http://mk.yuexingan06.cn

var a = 1;  let b = 2
来源：http://to.nszjky.cn

[T18] Swift：字符串插值
来源：http://jw.jctech888.com.cn

"值: \(b)"
来源：http://vx.yuexingan06.cn

[T19] Swift：可选绑定
来源：http://fm.szxytkj.cn

if let n = opt { print(n) }
来源：http://hr.shxzskj.cn

[T20] Swift：数组操作
来源：http://ck.huixinmuqiang.cn

var a = [1, 2, 3];  a.append(4)
来源：http://dh.bookmarksfly.cn

[T21] Swift：遍历
来源：http://bc.nicolike.cn

for x in a { print(x) }
来源：http://nq.yuntaijiaju.cn

[T22] Swift：字典
来源：http://dj.jianghongdianzi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ha.huanxung.cn

[T23] Swift：函数
来源：http://dd.shxzukj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ym.hnjuh.cn

[T24] Swift：闭包
来源：http://km.colortex.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://lw.521024.cn

[T25] Swift：结构体
来源：http://sn.haigaiapp.cn

struct P { var x: Int }
来源：http://ia.nszjky.cn

[T26] Swift：类与重写
来源：http://cx.chemitech.net.cn

class A: Base { override func f() {} }
来源：http://pm.lnxyls.cn

[T27] Swift：错误处理
来源：http://px.chemitech.net.cn

do { try f() } catch { print(error) }
来源：http://vf.colortex.cn

[T28] Swift：枚举
来源：http://vv.hahajie.cn

enum Color { case red, green }
来源：http://hs.9csxet.cn

[T29] Swift：guard 提前返回
来源：http://da.panjiajie.cn

guard let x = opt else { return }
来源：http://zk.bookmarksfly.cn

[T30] Swift：协议
来源：http://nt.bjjhwx.cn

protocol Shape { func area() -> Double }
来源：http://id.hahajie.cn

[T31] Lua：Hello World
来源：http://mj.wgjwhj.cn

print("Hello")
来源：http://dk.colortex.cn

[T32] Lua：局部变量
来源：http://jh.shxzukj.cn

local a = 1
来源：http://ga.jctech888.com.cn

[T33] Lua：表（数组）
来源：http://va.szsharing.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://bw.jctech888.com.cn

[T34] Lua：遍历表
来源：http://la.wgjwhj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://fj.muxihuayi.cn

[T35] Lua：字典表
来源：http://hu.huixinmuqiang.cn

local d = { a = 1 };  d.b = 2
来源：http://ab.yuntaijiaju.cn

[T36] Lua：函数
来源：http://rs.panjiajie.cn

function add(a, b) return a + b end
来源：http://qt.wgjwhj.cn

[T37] Lua：字符串拼接
来源：http://mv.asd995.cn

"a" .. "b"
来源：http://ue.haigaiapp.cn

[T38] Lua：条件
来源：http://ur.asd995.cn

if x > 0 then print("正") end
来源：http://hn.huixiangedu.cn

[T39] Lua：模式匹配
来源：http://dr.jctech888.com.cn

string.find(s, "%d+")
来源：http://va.jctech888.com.cn

[T40] Lua：元表
来源：http://tj.haigaiapp.cn

setmetatable({}, { __index = base })
来源：http://rd.asd995.cn

[T41] Perl：Hello World
来源：http://pv.yuexingan06.cn

print "Hello\n";
来源：http://cr.jianghongdianzi.cn

[T42] Perl：变量类型
来源：http://js.jianghongdianzi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lk.nicolike.cn

[T43] Perl：字符串插值
来源：http://tm.yuexingan06.cn

"值: $a"
来源：http://ct.jctech888.com.cn

[T44] Perl：条件
来源：http://nq.hahajie.cn

if ($a > 0) { print "正"; }
来源：http://tr.huixiangedu.cn

[T45] Perl：数组遍历
来源：http://mm.nszjky.cn

for my $x (@arr) { print $x; }
来源：http://un.hahajie.cn

[T46] Perl：哈希操作
来源：http://rx.shxzskj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kq.lnxyls.cn

[T47] Perl：正则捕获
来源：http://xw.asd995.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rf.panjiajie.cn

[T48] Perl：正则替换
来源：http://am.shxzukj.cn

$s =~ s/old/new/g;
来源：http://or.shxzskj.cn

[T49] Perl：函数
来源：http://cc.shxzukj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://av.shtwfgs.cn

[T50] Perl：逐行读文件
来源：http://ms.muxihuayi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ci.panjiajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://xx.chemitech.net.cn

[T51] Scala：Hello World
来源：http://bt.gzmigu.cn

println("Hello")
来源：http://mn.huixiangedu.cn

[T52] Scala：变量
来源：http://kz.szxytkj.cn

val a = 1;  var b = 2
来源：http://yh.521024.cn

[T53] Scala：字符串插值
来源：http://cy.jctech888.com.cn

s"值: $b"
来源：http://zf.jianghongdianzi.cn

[T54] Scala：集合映射
来源：http://sj.yuexingan06.cn

List(1, 2, 3).map(_ * 2)
来源：http://vf.jctech888.com.cn

[T55] Scala：集合过滤
来源：http://tb.muxihuayi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wc.521024.cn

[T56] Scala：样例类
来源：http://qu.yuexingan06.cn

case class User(name: String, age: Int)
来源：http://vj.lnxyls.cn

[T57] Scala：模式匹配
来源：http://am.colortex.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://lb.shxzukj.cn

[T58] Scala：函数定义
来源：http://ij.haigaiapp.cn

def add(a: Int, b: Int): Int = a + b
来源：http://oj.9csxet.cn

[T59] Scala：循环
来源：http://xn.newstarts.cn

for (i <- 1 to 10) println(i)
来源：http://io.jianghongdianzi.cn

[T60] Scala：折叠
来源：http://xo.wgjwhj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qx.newstarts.cn

================================================================================
来源：http://ko.yuntaijiaju.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kf.panjiajie.cn

================================================================================
来源：http://eg.521024.cn

[U01] Py：创建虚拟环境
来源：http://jh.huixiangedu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://tv.szsharing.cn

[U02] Py：导出 / 安装依赖
来源：http://nr.lnxyls.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gn.yuexingan06.cn

[U03] Py：加载 .env 配置
来源：http://nn.huanxung.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fw.wgjwhj.cn

[U04] Py：变量调试打印
来源：http://dp.521024.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mi.hahajie.cn

[U05] Py：列表去重且保序
来源：http://cp.muxihuayi.cn

list(dict.fromkeys(arr))
来源：http://wu.521024.cn

[U06] Py：合并两个字典
来源：http://wo.shxzskj.cn

{**a, **b}
来源：http://md.yuntaijiaju.cn

[U07] Py：反转字典键值
来源：http://ou.nicolike.cn

{v: k for k, v in d.items()}
来源：http://xe.bookmarksfly.cn

[U08] Py：展平二维列表
来源：http://wc.huixinmuqiang.cn

[y for x in nested for y in x]
来源：http://ej.chemitech.net.cn

[U09] Py：字典取最大值的键
来源：http://tu.muxihuayi.cn

max(d, key=d.get)
来源：http://zl.szxytkj.cn

[U10] Py：按值排序字典
来源：http://ih.hahajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tt.huanxung.cn

[U11] Py：生成器表达式
来源：http://hd.colortex.cn

(x * 2 for x in arr)
来源：http://tf.huixiangedu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mu.wgjwhj.cn

Counter(arr).most_common(3)
来源：http://ox.asd995.cn

[U13] Py：固定长度队列
来源：http://ce.nicolike.cn

deque(maxlen=10)
来源：http://ms.bookmarksfly.cn

[U14] Py：分组收集到列表
来源：http://eb.chemitech.net.cn

defaultdict(list)
来源：http://sj.colortex.cn

[U15] Py：高精度计时
来源：http://hu.colortex.cn

t = time.perf_counter()
来源：http://cv.newstarts.cn

[U16] Py：命令行参数解析
来源：http://gq.hnjuh.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rm.huixinmuqiang.cn

[U17] Py：初始化日志
来源：http://bo.wgjwhj.cn

logging.basicConfig(level=logging.INFO)
来源：http://ep.huixinmuqiang.cn

[U18] Py：预编译正则
来源：http://mx.bookmarksfly.cn

pat = re.compile(r"\d+")
来源：http://rj.nszjky.cn

[U19] Py：正则替换带回调
来源：http://nd.muxihuayi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nh.shxzukj.cn

[U20] Py：缓存函数结果
来源：http://hj.chemitech.net.cn

@functools.lru_cache(maxsize=None)
来源：http://oj.nszjky.cn

[U21] Py：自定义上下文管理器
来源：http://je.9csxet.cn

@contextlib.contextmanager
来源：http://wy.hnjuh.cn

[U22] Py：矩阵转置
来源：http://jy.panjiajie.cn

list(zip(*m))
来源：http://nk.yuntaijiaju.cn

[U23] Py：分块读取大文件
来源：http://tk.nicolike.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yuexingan06.cn

[U24] Py：路径操作
来源：http://gp.szxytkj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://do.szxytkj.cn

[U25] Py：CSV 按字典读
来源：http://jb.haigaiapp.cn

csv.DictReader(f)
来源：http://iv.panjiajie.cn

[U26] Py：并发下载
来源：http://pf.huixiangedu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ow.9csxet.cn

[U27] Py：异步 HTTP
来源：http://on.haigaiapp.cn

aiohttp.ClientSession() 配合 async with
来源：http://nd.huixiangedu.cn

[U28] Py：类型别名
来源：http://ua.panjiajie.cn

UserId = int
来源：http://wb.yuntaijiaju.cn

[U29] Py：属性校验
来源：http://ul.jctech888.com.cn

@property 与 @x.setter 配合
来源：http://sx.asd995.cn

[U30] Py：数据类
来源：http://ir.szxytkj.cn

@dataclass(slots=True)
来源：http://or.jctech888.com.cn

[U31] Py：单测
来源：http://jc.szsharing.cn

python -m pytest -q
来源：http://mf.newstarts.cn

[U32] Py：代码格式化
来源：http://af.huixiangedu.cn

ruff format . && ruff check --fix .
来源：http://ue.jctech888.com.cn

[U33] Py：打包发布
来源：http://fg.shtwfgs.cn

python -m build  （依赖 pyproject.toml）
来源：http://hh.colortex.cn

[U34] Py：判断编码
来源：http://qi.muxihuayi.cn

chardet.detect(raw)
来源：http://li.newstarts.cn

[U35] Py：发送邮件
来源：http://gu.gzmigu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://op.bjjhwx.cn

[U36] Py：定时任务
来源：http://uo.9csxet.cn

schedule.every(10).minutes.do(job)
来源：http://mo.jctech888.com.cn

[U37] Py：读写 Excel
来源：http://fa.asd995.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qx.jctech888.com.cn

[U38] Py：获取脚本所在目录
来源：http://ws.9csxet.cn

Path(__file__).resolve().parent
来源：http://np.yuexingan06.cn

[U39] Py：判断是否在交互环境
来源：http://ag.hahajie.cn

sys.stdout.isatty()
来源：http://rd.hnjuh.cn

[U40] Py：打印到标准错误
来源：http://rb.yuntaijiaju.cn

print("err", file=sys.stderr)
来源：http://es.newstarts.cn

[U41] PHP：初始化 Composer 项目
来源：http://dh.yuntaijiaju.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://to.bjjhwx.cn

[U42] PHP：PSR-4 自动加载
来源：http://ue.chemitech.net.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wl.haigaiapp.cn

[U43] PHP：声明命名空间
来源：http://so.asd995.cn

namespace App\Http;
来源：http://ec.haigaiapp.cn

[U44] PHP：开启严格类型
来源：http://ae.shxzskj.cn

declare(strict_types=1);
来源：http://oi.panjiajie.cn

[U45] PHP：类型声明与返回类型
来源：http://rs.haigaiapp.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://te.chemitech.net.cn

[U46] PHP：可空类型
来源：http://pz.yuntaijiaju.cn

?string $name = null
来源：http://hu.shxzskj.cn

[U47] PHP：联合类型
来源：http://vg.bjjhwx.cn

int|string $id
来源：http://mh.wgjwhj.cn

[U48] PHP：纯枚举
来源：http://cv.panjiajie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cn.nszjky.cn

[U49] PHP：只读属性
来源：http://kh.yuntaijiaju.cn

public readonly string $name
来源：http://lh.lnxyls.cn

[U50] PHP：构造器属性提升
来源：http://zm.colortex.cn

public function __construct(private int $id) {}
来源：http://av.gzmigu.cn

[U51] PHP：数组解构
来源：http://nh.lnxyls.cn

[$a, $b] = $arr;
来源：http://hg.shxzukj.cn

[U52] PHP：箭头函数
来源：http://nz.9csxet.cn

$double = fn($x) => $x * 2;
来源：http://wm.huixinmuqiang.cn

[U53] PHP：空合并运算符
来源：http://ws.bjjhwx.cn

$v = $a ?? $b ?? "default";
来源：http://cl.huixinmuqiang.cn

[U54] PHP：空安全调用
来源：http://vs.hnjuh.cn

$obj?->method()
来源：http://ne.lnxyls.cn

[U55] PHP：match 表达式
来源：http://vl.yuntaijiaju.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://py.panjiajie.cn

[U56] PHP：命名参数
来源：http://dm.asd995.cn

f(a: 1, b: 2)
来源：http://ek.huixinmuqiang.cn

[U57] PHP：字符串插值
来源：http://ns.nicolike.cn

"值: {$a}"
来源：http://ga.szxytkj.cn

[U58] PHP：数组三件套
来源：http://pe.haigaiapp.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zb.shxzskj.cn

[U59] PHP：自定义排序
来源：http://fp.szxytkj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kb.wgjwhj.cn

[U60] PHP：JSON 编解码
来源：http://jr.shxzskj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rb.9csxet.cn

[U61] PHP：正则
来源：http://us.bookmarksfly.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hv.nicolike.cn

[U62] PHP：日期对象
来源：http://yx.shxzukj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mq.nszjky.cn

[U63] PHP：文件读写
来源：http://di.shxzskj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zg.shxzukj.cn

[U64] PHP：目录遍历
来源：http://dv.hnjuh.cn

glob("dir/*.php");  scandir("dir");
来源：http://ln.huixinmuqiang.cn

[U65] PHP：会话
来源：http://ea.nszjky.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://mn.shtwfgs.cn

[U66] PHP：设置 Cookie
来源：http://fi.muxihuayi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rq.chemitech.net.cn

[U67] PHP：处理文件上传
来源：http://vr.huixinmuqiang.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ku.521024.cn

[U68] PHP：PDO 连接
来源：http://cm.shxzskj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bu.yuntaijiaju.cn

[U69] PHP：PDO 预处理
来源：http://la.bookmarksfly.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xk.9csxet.cn

[U70] PHP：PDO 事务
来源：http://zq.haigaiapp.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sh.szxytkj.cn

[U71] PHP：抛出异常
来源：http://zg.shxzukj.cn

throw new RuntimeException("失败", 500);
来源：http://wi.hnjuh.cn

[U72] PHP：写错误日志
来源：http://ah.chemitech.net.cn

error_log("失败: " . $e->getMessage());
来源：http://bl.panjiajie.cn

[U73] PHP：读取 ini 配置
来源：http://tz.bjjhwx.cn

parse_ini_file("config.ini", true)
来源：http://uc.colortex.cn

[U74] PHP：读取环境变量
来源：http://my.521024.cn

getenv("APP_ENV") ?: "production"
来源：http://jw.yuntaijiaju.cn

[U75] PHP：依赖注入
来源：http://uv.shxzukj.cn

composer require psr/container
来源：http://lk.huixiangedu.cn

[U76] PHP：简单路由
来源：http://zl.chemitech.net.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qn.shtwfgs.cn

[U77] PHP：模板渲染
来源：http://ld.gzmigu.cn

composer require twig/twig
来源：http://jy.bookmarksfly.cn

[U78] PHP：单元测试
来源：http://kw.szsharing.cn

composer require --dev phpunit/phpunit
来源：http://oi.colortex.cn

[U79] PHP：静态分析
来源：http://xy.wgjwhj.cn

composer require --dev phpstan/phpstan
来源：http://nc.bjjhwx.cn

[U80] PHP：代码规范修复
来源：http://nt.hnjuh.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ko.yuexingan06.cn

[U81] JS：初始化项目
来源：http://yp.shxzskj.cn

npm init -y;  npm i express
来源：http://cq.lnxyls.cn

[U82] JS：package.json 脚本
来源：http://mv.szsharing.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rh.newstarts.cn


<!-- 参考信息 -->