代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://oq.panjiajie.cn

[S57] C++：编译期常量
来源：http://et.huixiangedu.cn

constexpr int N = 10;
来源：http://ed.lnxyls.cn

[S58] C++：命名空间
来源：http://qq.muxihuayi.cn

namespace ns { int f() { return 1; } }
来源：http://us.newstarts.cn

[S59] C++：静态断言
来源：http://bm.muxihuayi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://sm.szsharing.cn

[S60] C++：遍历并删除元素
来源：http://zz.lnxyls.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cx.colortex.cn

================================================================================
来源：http://zb.yuexingan06.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://oh.gzmigu.cn

================================================================================
来源：http://vc.hnjuh.cn

[T01] Kotlin：Hello World
来源：http://qy.bookmarksfly.cn

println("Hello")
来源：http://sc.huixinmuqiang.cn

[T02] Kotlin：变量
来源：http://ly.newstarts.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mf.huixiangedu.cn

[T03] Kotlin：字符串模板
来源：http://ck.bookmarksfly.cn

"值: $b"
来源：http://eo.chemitech.net.cn

[T04] Kotlin：空安全
来源：http://ma.gzmigu.cn

val n: String? = null;  n?.length
来源：http://gt.huanxung.cn

[T05] Kotlin：when 表达式
来源：http://rw.huanxung.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nl.chemitech.net.cn

[T06] Kotlin：集合映射
来源：http://al.panjiajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://bs.nicolike.cn

[T07] Kotlin：集合过滤
来源：http://qj.521024.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pq.shtwfgs.cn

[T08] Kotlin：数据类
来源：http://gh.shxzskj.cn

data class User(val name: String, val age: Int)
来源：http://hn.bookmarksfly.cn

[T09] Kotlin：扩展函数
来源：http://bi.huanxung.cn

fun String.exclaim() = this + "!"
来源：http://qk.hnjuh.cn

[T10] Kotlin：默认参数
来源：http://lc.bookmarksfly.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ep.panjiajie.cn

[T11] Kotlin：协程
来源：http://em.asd995.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nz.9csxet.cn

[T12] Kotlin：解构声明
来源：http://ym.bookmarksfly.cn

val (a, b) = Pair(1, 2)
来源：http://sr.nszjky.cn

[T13] Kotlin：只读 Map
来源：http://od.asd995.cn

val m = mapOf("a" to 1)
来源：http://cb.jctech888.com.cn

[T14] Kotlin：循环
来源：http://ce.nszjky.cn

for (i in 1..10) println(i)
来源：http://fj.huixinmuqiang.cn

[T15] Kotlin：接口
来源：http://kg.bjjhwx.cn

interface Shape { fun area(): Double }
来源：http://vq.szxytkj.cn

[T16] Swift：Hello World
来源：http://bb.jianghongdianzi.cn

print("Hello")
来源：http://db.yuntaijiaju.cn

[T17] Swift：变量与常量
来源：http://rb.nicolike.cn

var a = 1;  let b = 2
来源：http://oe.jianghongdianzi.cn

[T18] Swift：字符串插值
来源：http://dh.gzmigu.cn

"值: \(b)"
来源：http://cz.huixiangedu.cn

[T19] Swift：可选绑定
来源：http://au.huixinmuqiang.cn

if let n = opt { print(n) }
来源：http://my.hahajie.cn

[T20] Swift：数组操作
来源：http://ue.chemitech.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://bd.gzmigu.cn

[T21] Swift：遍历
来源：http://la.jctech888.com.cn

for x in a { print(x) }
来源：http://jp.jctech888.com.cn

[T22] Swift：字典
来源：http://yy.hahajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://yn.szxytkj.cn

[T23] Swift：函数
来源：http://gq.asd995.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ds.panjiajie.cn

[T24] Swift：闭包
来源：http://iz.huixinmuqiang.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://hd.jctech888.com.cn

[T25] Swift：结构体
来源：http://bu.newstarts.cn

struct P { var x: Int }
来源：http://ad.panjiajie.cn

[T26] Swift：类与重写
来源：http://hp.colortex.cn

class A: Base { override func f() {} }
来源：http://md.szsharing.cn

[T27] Swift：错误处理
来源：http://tm.hahajie.cn

do { try f() } catch { print(error) }
来源：http://na.shxzukj.cn

[T28] Swift：枚举
来源：http://de.bjjhwx.cn

enum Color { case red, green }
来源：http://lw.lnxyls.cn

[T29] Swift：guard 提前返回
来源：http://ta.nicolike.cn

guard let x = opt else { return }
来源：http://ls.asd995.cn

[T30] Swift：协议
来源：http://pl.panjiajie.cn

protocol Shape { func area() -> Double }
来源：http://cr.huanxung.cn

[T31] Lua：Hello World
来源：http://ou.shtwfgs.cn

print("Hello")
来源：http://vz.huixiangedu.cn

[T32] Lua：局部变量
来源：http://ks.bjjhwx.cn

local a = 1
来源：http://vh.muxihuayi.cn

[T33] Lua：表（数组）
来源：http://qz.gzmigu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://le.hahajie.cn

[T34] Lua：遍历表
来源：http://ce.nszjky.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://yv.bookmarksfly.cn

[T35] Lua：字典表
来源：http://xx.asd995.cn

local d = { a = 1 };  d.b = 2
来源：http://xu.asd995.cn

[T36] Lua：函数
来源：http://rl.panjiajie.cn

function add(a, b) return a + b end
来源：http://tw.shxzskj.cn

[T37] Lua：字符串拼接
来源：http://mh.huixinmuqiang.cn

"a" .. "b"
来源：http://ab.yuexingan06.cn

[T38] Lua：条件
来源：http://ny.muxihuayi.cn

if x > 0 then print("正") end
来源：http://fy.asd995.cn

[T39] Lua：模式匹配
来源：http://fg.shxzukj.cn

string.find(s, "%d+")
来源：http://xc.jctech888.com.cn

[T40] Lua：元表
来源：http://rk.huixiangedu.cn

setmetatable({}, { __index = base })
来源：http://qc.shtwfgs.cn

[T41] Perl：Hello World
来源：http://sj.hnjuh.cn

print "Hello\n";
来源：http://wm.wgjwhj.cn

[T42] Perl：变量类型
来源：http://oj.szsharing.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://or.colortex.cn

[T43] Perl：字符串插值
来源：http://ff.huixinmuqiang.cn

"值: $a"
来源：http://yn.szsharing.cn

[T44] Perl：条件
来源：http://wp.haigaiapp.cn

if ($a > 0) { print "正"; }
来源：http://kl.wgjwhj.cn

[T45] Perl：数组遍历
来源：http://hl.wgjwhj.cn

for my $x (@arr) { print $x; }
来源：http://oo.521024.cn

[T46] Perl：哈希操作
来源：http://ol.chemitech.net.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://aq.shtwfgs.cn

[T47] Perl：正则捕获
来源：http://ls.colortex.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rh.colortex.cn

[T48] Perl：正则替换
来源：http://jh.wgjwhj.cn

$s =~ s/old/new/g;
来源：http://kb.shxzukj.cn

[T49] Perl：函数
来源：http://dq.chemitech.net.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ov.hahajie.cn

[T50] Perl：逐行读文件
来源：http://rr.hnjuh.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xs.bookmarksfly.cn

while (my $line = <$fh>) { print $line; }
来源：http://pt.asd995.cn

[T51] Scala：Hello World
来源：http://su.yuntaijiaju.cn

println("Hello")
来源：http://oy.huanxung.cn

[T52] Scala：变量
来源：http://dg.hnjuh.cn

val a = 1;  var b = 2
来源：http://oc.muxihuayi.cn

[T53] Scala：字符串插值
来源：http://zm.szxytkj.cn

s"值: $b"
来源：http://cu.hahajie.cn

[T54] Scala：集合映射
来源：http://nw.chemitech.net.cn

List(1, 2, 3).map(_ * 2)
来源：http://eg.colortex.cn

[T55] Scala：集合过滤
来源：http://xl.szxytkj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ab.gzmigu.cn

[T56] Scala：样例类
来源：http://vk.nszjky.cn

case class User(name: String, age: Int)
来源：http://ah.asd995.cn

[T57] Scala：模式匹配
来源：http://yo.wgjwhj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gi.asd995.cn

[T58] Scala：函数定义
来源：http://ua.colortex.cn

def add(a: Int, b: Int): Int = a + b
来源：http://tr.szsharing.cn

[T59] Scala：循环
来源：http://zr.yuntaijiaju.cn

for (i <- 1 to 10) println(i)
来源：http://cm.huixiangedu.cn

[T60] Scala：折叠
来源：http://qe.nicolike.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xv.shxzskj.cn

================================================================================
来源：http://ad.yuexingan06.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sq.521024.cn

================================================================================
来源：http://up.gzmigu.cn

[U01] Py：创建虚拟环境
来源：http://wx.bjjhwx.cn

python -m venv .venv && source .venv/bin/activate
来源：http://sk.hahajie.cn

[U02] Py：导出 / 安装依赖
来源：http://gq.shtwfgs.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://df.bjjhwx.cn

[U03] Py：加载 .env 配置
来源：http://ac.jianghongdianzi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rf.colortex.cn

[U04] Py：变量调试打印
来源：http://oc.lnxyls.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pj.szxytkj.cn

[U05] Py：列表去重且保序
来源：http://px.colortex.cn

list(dict.fromkeys(arr))
来源：http://hr.huanxung.cn

[U06] Py：合并两个字典
来源：http://do.szxytkj.cn

{**a, **b}
来源：http://nj.lnxyls.cn

[U07] Py：反转字典键值
来源：http://ko.nszjky.cn

{v: k for k, v in d.items()}
来源：http://mo.nicolike.cn

[U08] Py：展平二维列表
来源：http://pg.yuntaijiaju.cn

[y for x in nested for y in x]
来源：http://id.shtwfgs.cn

[U09] Py：字典取最大值的键
来源：http://hg.gzmigu.cn

max(d, key=d.get)
来源：http://cf.jctech888.com.cn

[U10] Py：按值排序字典
来源：http://co.wgjwhj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bm.chemitech.net.cn

[U11] Py：生成器表达式
来源：http://uu.huixinmuqiang.cn

(x * 2 for x in arr)
来源：http://qx.shxzskj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lm.wgjwhj.cn

Counter(arr).most_common(3)
来源：http://pi.nszjky.cn

[U13] Py：固定长度队列
来源：http://xk.yuntaijiaju.cn

deque(maxlen=10)
来源：http://ta.lnxyls.cn

[U14] Py：分组收集到列表
来源：http://af.yuexingan06.cn

defaultdict(list)
来源：http://pv.nicolike.cn

[U15] Py：高精度计时
来源：http://bl.bookmarksfly.cn

t = time.perf_counter()
来源：http://hc.bookmarksfly.cn

[U16] Py：命令行参数解析
来源：http://ts.jctech888.com.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nv.huixiangedu.cn

[U17] Py：初始化日志
来源：http://zu.jctech888.com.cn

logging.basicConfig(level=logging.INFO)
来源：http://ql.lnxyls.cn

[U18] Py：预编译正则
来源：http://ny.chemitech.net.cn

pat = re.compile(r"\d+")
来源：http://ok.szsharing.cn

[U19] Py：正则替换带回调
来源：http://ho.521024.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://oj.jianghongdianzi.cn

[U20] Py：缓存函数结果
来源：http://gt.bjjhwx.cn

@functools.lru_cache(maxsize=None)
来源：http://ve.jianghongdianzi.cn

[U21] Py：自定义上下文管理器
来源：http://fn.wgjwhj.cn

@contextlib.contextmanager
来源：http://tf.colortex.cn

[U22] Py：矩阵转置
来源：http://wg.chemitech.net.cn

list(zip(*m))
来源：http://yj.nszjky.cn

[U23] Py：分块读取大文件
来源：http://gj.nszjky.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hr.shtwfgs.cn

[U24] Py：路径操作
来源：http://mc.bookmarksfly.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mh.szsharing.cn

[U25] Py：CSV 按字典读
来源：http://dd.huixinmuqiang.cn

csv.DictReader(f)
来源：http://qr.asd995.cn

[U26] Py：并发下载
来源：http://xp.bjjhwx.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nt.huixiangedu.cn

[U27] Py：异步 HTTP
来源：http://mr.chemitech.net.cn

aiohttp.ClientSession() 配合 async with
来源：http://ks.huixiangedu.cn

[U28] Py：类型别名
来源：http://ey.haigaiapp.cn

UserId = int
来源：http://ok.yuntaijiaju.cn

[U29] Py：属性校验
来源：http://hy.chemitech.net.cn

@property 与 @x.setter 配合
来源：http://de.newstarts.cn

[U30] Py：数据类
来源：http://tx.lnxyls.cn

@dataclass(slots=True)
来源：http://tf.yuexingan06.cn

[U31] Py：单测
来源：http://oc.yuntaijiaju.cn

python -m pytest -q
来源：http://sh.newstarts.cn

[U32] Py：代码格式化
来源：http://dv.gzmigu.cn

ruff format . && ruff check --fix .
来源：http://cg.huixinmuqiang.cn

[U33] Py：打包发布
来源：http://sf.shxzukj.cn

python -m build  （依赖 pyproject.toml）
来源：http://ba.yuexingan06.cn

[U34] Py：判断编码
来源：http://ub.yuexingan06.cn

chardet.detect(raw)
来源：http://uh.shxzukj.cn

[U35] Py：发送邮件
来源：http://bq.panjiajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://sn.nszjky.cn

[U36] Py：定时任务
来源：http://kk.shtwfgs.cn

schedule.every(10).minutes.do(job)
来源：http://nm.hnjuh.cn

[U37] Py：读写 Excel
来源：http://mm.panjiajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://kq.bjjhwx.cn

[U38] Py：获取脚本所在目录
来源：http://zn.jianghongdianzi.cn

Path(__file__).resolve().parent
来源：http://ba.bookmarksfly.cn

[U39] Py：判断是否在交互环境
来源：http://xt.jianghongdianzi.cn

sys.stdout.isatty()
来源：http://iq.shxzukj.cn

[U40] Py：打印到标准错误
来源：http://lk.wgjwhj.cn

print("err", file=sys.stderr)
来源：http://yx.panjiajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://gp.nicolike.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://tj.shxzukj.cn

[U42] PHP：PSR-4 自动加载
来源：http://wl.newstarts.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://oz.hnjuh.cn

[U43] PHP：声明命名空间
来源：http://bg.newstarts.cn

namespace App\Http;
来源：http://zt.9csxet.cn

[U44] PHP：开启严格类型
来源：http://ml.chemitech.net.cn

declare(strict_types=1);
来源：http://oo.lnxyls.cn

[U45] PHP：类型声明与返回类型
来源：http://tf.shxzukj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bt.521024.cn

[U46] PHP：可空类型
来源：http://ap.muxihuayi.cn

?string $name = null
来源：http://og.shtwfgs.cn

[U47] PHP：联合类型
来源：http://ih.nszjky.cn

int|string $id
来源：http://fe.huixinmuqiang.cn

[U48] PHP：纯枚举
来源：http://zb.newstarts.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://db.hahajie.cn

[U49] PHP：只读属性
来源：http://kq.nszjky.cn

public readonly string $name
来源：http://un.shxzukj.cn

[U50] PHP：构造器属性提升
来源：http://my.gzmigu.cn

public function __construct(private int $id) {}
来源：http://cv.bookmarksfly.cn

[U51] PHP：数组解构
来源：http://gd.wgjwhj.cn

[$a, $b] = $arr;
来源：http://cg.jctech888.com.cn

[U52] PHP：箭头函数
来源：http://iy.colortex.cn

$double = fn($x) => $x * 2;
来源：http://af.asd995.cn

[U53] PHP：空合并运算符
来源：http://vo.gzmigu.cn

$v = $a ?? $b ?? "default";
来源：http://jz.huixiangedu.cn

[U54] PHP：空安全调用
来源：http://ez.yuexingan06.cn

$obj?->method()
来源：http://ml.huixinmuqiang.cn

[U55] PHP：match 表达式
来源：http://ft.wgjwhj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ws.panjiajie.cn

[U56] PHP：命名参数
来源：http://bu.huanxung.cn

f(a: 1, b: 2)
来源：http://cb.shxzskj.cn

[U57] PHP：字符串插值
来源：http://bc.panjiajie.cn

"值: {$a}"
来源：http://tz.9csxet.cn

[U58] PHP：数组三件套
来源：http://xi.asd995.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qx.bookmarksfly.cn

[U59] PHP：自定义排序
来源：http://yv.bjjhwx.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sj.yuexingan06.cn

[U60] PHP：JSON 编解码
来源：http://nc.wgjwhj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jf.chemitech.net.cn

[U61] PHP：正则
来源：http://cz.panjiajie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vn.wgjwhj.cn

[U62] PHP：日期对象
来源：http://dc.newstarts.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sw.muxihuayi.cn

[U63] PHP：文件读写
来源：http://eb.shxzskj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qw.bookmarksfly.cn

[U64] PHP：目录遍历
来源：http://tu.nicolike.cn

glob("dir/*.php");  scandir("dir");
来源：http://jn.lnxyls.cn

[U65] PHP：会话
来源：http://qp.chemitech.net.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://po.szxytkj.cn

[U66] PHP：设置 Cookie
来源：http://rf.chemitech.net.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vl.newstarts.cn

[U67] PHP：处理文件上传
来源：http://lq.gzmigu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://av.jianghongdianzi.cn

[U68] PHP：PDO 连接
来源：http://ju.nszjky.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bz.muxihuayi.cn

[U69] PHP：PDO 预处理
来源：http://mo.9csxet.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xk.hnjuh.cn

[U70] PHP：PDO 事务
来源：http://nh.chemitech.net.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kg.nszjky.cn

[U71] PHP：抛出异常
来源：http://km.nszjky.cn

throw new RuntimeException("失败", 500);
来源：http://ez.9csxet.cn

[U72] PHP：写错误日志
来源：http://do.huanxung.cn

error_log("失败: " . $e->getMessage());
来源：http://he.hnjuh.cn

[U73] PHP：读取 ini 配置
来源：http://ec.gzmigu.cn

parse_ini_file("config.ini", true)
来源：http://lg.nszjky.cn

[U74] PHP：读取环境变量
来源：http://kb.lnxyls.cn

getenv("APP_ENV") ?: "production"
来源：http://ze.shxzukj.cn

[U75] PHP：依赖注入
来源：http://tx.haigaiapp.cn

composer require psr/container
来源：http://ca.szxytkj.cn

[U76] PHP：简单路由
来源：http://tw.shxzukj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://id.nicolike.cn

[U77] PHP：模板渲染
来源：http://zv.colortex.cn

composer require twig/twig
来源：http://zl.yuexingan06.cn

[U78] PHP：单元测试
来源：http://uf.shxzskj.cn

composer require --dev phpunit/phpunit
来源：http://be.hahajie.cn

[U79] PHP：静态分析
来源：http://rg.szsharing.cn

composer require --dev phpstan/phpstan
来源：http://sg.9csxet.cn

[U80] PHP：代码规范修复
来源：http://qg.shtwfgs.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qv.shtwfgs.cn

[U81] JS：初始化项目
来源：http://jd.szxytkj.cn

npm init -y;  npm i express
来源：http://uh.bookmarksfly.cn

[U82] JS：package.json 脚本
来源：http://ld.bjjhwx.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kp.yuexingan06.cn


<!-- 参考信息 -->