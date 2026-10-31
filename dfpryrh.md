代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nz.gzmigu.cn

[S57] C++：编译期常量
来源：http://wf.hahajie.cn

constexpr int N = 10;
来源：http://qj.lnxyls.cn

[S58] C++：命名空间
来源：http://hs.shxzukj.cn

namespace ns { int f() { return 1; } }
来源：http://kx.nszjky.cn

[S59] C++：静态断言
来源：http://ef.szsharing.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vj.hahajie.cn

[S60] C++：遍历并删除元素
来源：http://cr.huanxung.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ta.jctech888.com.cn

================================================================================
来源：http://bt.szsharing.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vp.huixiangedu.cn

================================================================================
来源：http://jo.nszjky.cn

[T01] Kotlin：Hello World
来源：http://ex.newstarts.cn

println("Hello")
来源：http://am.jianghongdianzi.cn

[T02] Kotlin：变量
来源：http://fg.521024.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hk.521024.cn

[T03] Kotlin：字符串模板
来源：http://nd.newstarts.cn

"值: $b"
来源：http://vn.jianghongdianzi.cn

[T04] Kotlin：空安全
来源：http://bn.muxihuayi.cn

val n: String? = null;  n?.length
来源：http://qk.bjjhwx.cn

[T05] Kotlin：when 表达式
来源：http://dm.9csxet.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ya.haigaiapp.cn

[T06] Kotlin：集合映射
来源：http://xx.bjjhwx.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://zi.asd995.cn

[T07] Kotlin：集合过滤
来源：http://uw.jctech888.com.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://yh.yuntaijiaju.cn

[T08] Kotlin：数据类
来源：http://xa.szxytkj.cn

data class User(val name: String, val age: Int)
来源：http://qa.nszjky.cn

[T09] Kotlin：扩展函数
来源：http://jq.newstarts.cn

fun String.exclaim() = this + "!"
来源：http://wy.colortex.cn

[T10] Kotlin：默认参数
来源：http://jz.gzmigu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qu.lnxyls.cn

[T11] Kotlin：协程
来源：http://xf.jctech888.com.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://gz.hahajie.cn

[T12] Kotlin：解构声明
来源：http://zk.yuntaijiaju.cn

val (a, b) = Pair(1, 2)
来源：http://io.haigaiapp.cn

[T13] Kotlin：只读 Map
来源：http://sf.521024.cn

val m = mapOf("a" to 1)
来源：http://wc.bookmarksfly.cn

[T14] Kotlin：循环
来源：http://rm.muxihuayi.cn

for (i in 1..10) println(i)
来源：http://jr.asd995.cn

[T15] Kotlin：接口
来源：http://yj.muxihuayi.cn

interface Shape { fun area(): Double }
来源：http://ax.yuntaijiaju.cn

[T16] Swift：Hello World
来源：http://fv.colortex.cn

print("Hello")
来源：http://sn.yuexingan06.cn

[T17] Swift：变量与常量
来源：http://xo.wgjwhj.cn

var a = 1;  let b = 2
来源：http://ab.szxytkj.cn

[T18] Swift：字符串插值
来源：http://oq.szsharing.cn

"值: \(b)"
来源：http://rk.huixinmuqiang.cn

[T19] Swift：可选绑定
来源：http://ri.szsharing.cn

if let n = opt { print(n) }
来源：http://mi.bookmarksfly.cn

[T20] Swift：数组操作
来源：http://bs.hahajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://lx.huanxung.cn

[T21] Swift：遍历
来源：http://oh.jctech888.com.cn

for x in a { print(x) }
来源：http://zj.asd995.cn

[T22] Swift：字典
来源：http://lu.huixiangedu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://os.newstarts.cn

[T23] Swift：函数
来源：http://uf.bjjhwx.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://os.haigaiapp.cn

[T24] Swift：闭包
来源：http://lk.panjiajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gr.nszjky.cn

[T25] Swift：结构体
来源：http://dd.szxytkj.cn

struct P { var x: Int }
来源：http://pg.lnxyls.cn

[T26] Swift：类与重写
来源：http://qm.haigaiapp.cn

class A: Base { override func f() {} }
来源：http://kp.szxytkj.cn

[T27] Swift：错误处理
来源：http://gy.gzmigu.cn

do { try f() } catch { print(error) }
来源：http://wf.huixinmuqiang.cn

[T28] Swift：枚举
来源：http://bi.chemitech.net.cn

enum Color { case red, green }
来源：http://wv.gzmigu.cn

[T29] Swift：guard 提前返回
来源：http://lp.bookmarksfly.cn

guard let x = opt else { return }
来源：http://sr.gzmigu.cn

[T30] Swift：协议
来源：http://oz.hnjuh.cn

protocol Shape { func area() -> Double }
来源：http://rk.lnxyls.cn

[T31] Lua：Hello World
来源：http://mj.bjjhwx.cn

print("Hello")
来源：http://nk.chemitech.net.cn

[T32] Lua：局部变量
来源：http://tw.yuntaijiaju.cn

local a = 1
来源：http://qv.bjjhwx.cn

[T33] Lua：表（数组）
来源：http://pi.nicolike.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wd.nszjky.cn

[T34] Lua：遍历表
来源：http://bt.huixinmuqiang.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gv.nicolike.cn

[T35] Lua：字典表
来源：http://xj.shtwfgs.cn

local d = { a = 1 };  d.b = 2
来源：http://gw.muxihuayi.cn

[T36] Lua：函数
来源：http://zb.huixinmuqiang.cn

function add(a, b) return a + b end
来源：http://pj.huixiangedu.cn

[T37] Lua：字符串拼接
来源：http://qo.shxzukj.cn

"a" .. "b"
来源：http://pj.shtwfgs.cn

[T38] Lua：条件
来源：http://wo.bjjhwx.cn

if x > 0 then print("正") end
来源：http://vb.szxytkj.cn

[T39] Lua：模式匹配
来源：http://jb.hahajie.cn

string.find(s, "%d+")
来源：http://zu.521024.cn

[T40] Lua：元表
来源：http://fe.521024.cn

setmetatable({}, { __index = base })
来源：http://gw.lnxyls.cn

[T41] Perl：Hello World
来源：http://pe.hnjuh.cn

print "Hello\n";
来源：http://wn.shtwfgs.cn

[T42] Perl：变量类型
来源：http://hr.haigaiapp.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xm.shxzskj.cn

[T43] Perl：字符串插值
来源：http://aj.jctech888.com.cn

"值: $a"
来源：http://lj.jctech888.com.cn

[T44] Perl：条件
来源：http://lv.shxzskj.cn

if ($a > 0) { print "正"; }
来源：http://jf.nszjky.cn

[T45] Perl：数组遍历
来源：http://hk.szsharing.cn

for my $x (@arr) { print $x; }
来源：http://bl.hnjuh.cn

[T46] Perl：哈希操作
来源：http://pi.bjjhwx.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tq.chemitech.net.cn

[T47] Perl：正则捕获
来源：http://mm.nicolike.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://bv.yuexingan06.cn

[T48] Perl：正则替换
来源：http://dz.gzmigu.cn

$s =~ s/old/new/g;
来源：http://fv.newstarts.cn

[T49] Perl：函数
来源：http://nw.gzmigu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://um.haigaiapp.cn

[T50] Perl：逐行读文件
来源：http://rg.newstarts.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fc.9csxet.cn

while (my $line = <$fh>) { print $line; }
来源：http://sj.gzmigu.cn

[T51] Scala：Hello World
来源：http://gh.colortex.cn

println("Hello")
来源：http://au.muxihuayi.cn

[T52] Scala：变量
来源：http://fx.521024.cn

val a = 1;  var b = 2
来源：http://ur.colortex.cn

[T53] Scala：字符串插值
来源：http://bp.nszjky.cn

s"值: $b"
来源：http://mw.shxzukj.cn

[T54] Scala：集合映射
来源：http://dq.gzmigu.cn

List(1, 2, 3).map(_ * 2)
来源：http://yw.haigaiapp.cn

[T55] Scala：集合过滤
来源：http://jv.yuexingan06.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ts.nszjky.cn

[T56] Scala：样例类
来源：http://ze.haigaiapp.cn

case class User(name: String, age: Int)
来源：http://oc.huixinmuqiang.cn

[T57] Scala：模式匹配
来源：http://dh.wgjwhj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vf.wgjwhj.cn

[T58] Scala：函数定义
来源：http://ss.bookmarksfly.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gc.chemitech.net.cn

[T59] Scala：循环
来源：http://rs.gzmigu.cn

for (i <- 1 to 10) println(i)
来源：http://uu.huixinmuqiang.cn

[T60] Scala：折叠
来源：http://lm.jctech888.com.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://md.9csxet.cn

================================================================================
来源：http://mh.hahajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mr.bjjhwx.cn

================================================================================
来源：http://kc.jianghongdianzi.cn

[U01] Py：创建虚拟环境
来源：http://ry.shtwfgs.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ko.haigaiapp.cn

[U02] Py：导出 / 安装依赖
来源：http://js.hnjuh.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://su.hahajie.cn

[U03] Py：加载 .env 配置
来源：http://hx.szsharing.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://bo.muxihuayi.cn

[U04] Py：变量调试打印
来源：http://hj.huixiangedu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sl.newstarts.cn

[U05] Py：列表去重且保序
来源：http://oq.bjjhwx.cn

list(dict.fromkeys(arr))
来源：http://uj.hahajie.cn

[U06] Py：合并两个字典
来源：http://wd.shtwfgs.cn

{**a, **b}
来源：http://rb.nicolike.cn

[U07] Py：反转字典键值
来源：http://vp.huixiangedu.cn

{v: k for k, v in d.items()}
来源：http://ee.9csxet.cn

[U08] Py：展平二维列表
来源：http://kj.szsharing.cn

[y for x in nested for y in x]
来源：http://xv.yuexingan06.cn

[U09] Py：字典取最大值的键
来源：http://uu.hnjuh.cn

max(d, key=d.get)
来源：http://kc.jianghongdianzi.cn

[U10] Py：按值排序字典
来源：http://tn.yuexingan06.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hr.huixinmuqiang.cn

[U11] Py：生成器表达式
来源：http://nb.szxytkj.cn

(x * 2 for x in arr)
来源：http://lk.nszjky.cn

[U12] Py：取出现最多的 3 个元素
来源：http://bo.hnjuh.cn

Counter(arr).most_common(3)
来源：http://my.colortex.cn

[U13] Py：固定长度队列
来源：http://wq.shxzukj.cn

deque(maxlen=10)
来源：http://ru.haigaiapp.cn

[U14] Py：分组收集到列表
来源：http://wz.wgjwhj.cn

defaultdict(list)
来源：http://ds.bookmarksfly.cn

[U15] Py：高精度计时
来源：http://vd.huanxung.cn

t = time.perf_counter()
来源：http://ti.bjjhwx.cn

[U16] Py：命令行参数解析
来源：http://sd.bookmarksfly.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qw.521024.cn

[U17] Py：初始化日志
来源：http://ad.haigaiapp.cn

logging.basicConfig(level=logging.INFO)
来源：http://vn.colortex.cn

[U18] Py：预编译正则
来源：http://dh.yuexingan06.cn

pat = re.compile(r"\d+")
来源：http://xs.jctech888.com.cn

[U19] Py：正则替换带回调
来源：http://jr.bookmarksfly.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jf.hnjuh.cn

[U20] Py：缓存函数结果
来源：http://ni.hahajie.cn

@functools.lru_cache(maxsize=None)
来源：http://mg.521024.cn

[U21] Py：自定义上下文管理器
来源：http://lf.asd995.cn

@contextlib.contextmanager
来源：http://xr.521024.cn

[U22] Py：矩阵转置
来源：http://ri.lnxyls.cn

list(zip(*m))
来源：http://fw.szsharing.cn

[U23] Py：分块读取大文件
来源：http://mh.newstarts.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hy.asd995.cn

[U24] Py：路径操作
来源：http://bk.yuexingan06.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://oc.jctech888.com.cn

[U25] Py：CSV 按字典读
来源：http://uc.chemitech.net.cn

csv.DictReader(f)
来源：http://zt.szsharing.cn

[U26] Py：并发下载
来源：http://pa.huixiangedu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vp.colortex.cn

[U27] Py：异步 HTTP
来源：http://ae.haigaiapp.cn

aiohttp.ClientSession() 配合 async with
来源：http://vm.asd995.cn

[U28] Py：类型别名
来源：http://oy.haigaiapp.cn

UserId = int
来源：http://xo.lnxyls.cn

[U29] Py：属性校验
来源：http://lu.hnjuh.cn

@property 与 @x.setter 配合
来源：http://dg.jianghongdianzi.cn

[U30] Py：数据类
来源：http://sq.muxihuayi.cn

@dataclass(slots=True)
来源：http://ph.szxytkj.cn

[U31] Py：单测
来源：http://ku.yuexingan06.cn

python -m pytest -q
来源：http://uj.wgjwhj.cn

[U32] Py：代码格式化
来源：http://nz.asd995.cn

ruff format . && ruff check --fix .
来源：http://ps.bjjhwx.cn

[U33] Py：打包发布
来源：http://pw.nszjky.cn

python -m build  （依赖 pyproject.toml）
来源：http://cs.9csxet.cn

[U34] Py：判断编码
来源：http://ou.9csxet.cn

chardet.detect(raw)
来源：http://kl.bookmarksfly.cn

[U35] Py：发送邮件
来源：http://gr.jctech888.com.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wx.shxzskj.cn

[U36] Py：定时任务
来源：http://ai.nicolike.cn

schedule.every(10).minutes.do(job)
来源：http://vq.chemitech.net.cn

[U37] Py：读写 Excel
来源：http://ni.huanxung.cn

pandas.read_excel / DataFrame.to_excel
来源：http://mp.nicolike.cn

[U38] Py：获取脚本所在目录
来源：http://pp.huanxung.cn

Path(__file__).resolve().parent
来源：http://gz.chemitech.net.cn

[U39] Py：判断是否在交互环境
来源：http://sw.panjiajie.cn

sys.stdout.isatty()
来源：http://ki.wgjwhj.cn

[U40] Py：打印到标准错误
来源：http://no.newstarts.cn

print("err", file=sys.stderr)
来源：http://hp.muxihuayi.cn

[U41] PHP：初始化 Composer 项目
来源：http://lt.hahajie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://bt.newstarts.cn

[U42] PHP：PSR-4 自动加载
来源：http://ut.huixiangedu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bi.huixinmuqiang.cn

[U43] PHP：声明命名空间
来源：http://ev.huixinmuqiang.cn

namespace App\Http;
来源：http://wy.huixinmuqiang.cn

[U44] PHP：开启严格类型
来源：http://qg.haigaiapp.cn

declare(strict_types=1);
来源：http://re.colortex.cn

[U45] PHP：类型声明与返回类型
来源：http://jq.huixiangedu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://rs.521024.cn

[U46] PHP：可空类型
来源：http://wu.huanxung.cn

?string $name = null
来源：http://xu.nicolike.cn

[U47] PHP：联合类型
来源：http://bg.colortex.cn

int|string $id
来源：http://ff.gzmigu.cn

[U48] PHP：纯枚举
来源：http://wj.huanxung.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gw.9csxet.cn

[U49] PHP：只读属性
来源：http://hj.muxihuayi.cn

public readonly string $name
来源：http://vt.nicolike.cn

[U50] PHP：构造器属性提升
来源：http://rl.huixiangedu.cn

public function __construct(private int $id) {}
来源：http://ql.hahajie.cn

[U51] PHP：数组解构
来源：http://fz.nszjky.cn

[$a, $b] = $arr;
来源：http://wl.wgjwhj.cn

[U52] PHP：箭头函数
来源：http://qq.shtwfgs.cn

$double = fn($x) => $x * 2;
来源：http://wq.haigaiapp.cn

[U53] PHP：空合并运算符
来源：http://ch.jianghongdianzi.cn

$v = $a ?? $b ?? "default";
来源：http://ef.hnjuh.cn

[U54] PHP：空安全调用
来源：http://jf.bjjhwx.cn

$obj?->method()
来源：http://zv.jianghongdianzi.cn

[U55] PHP：match 表达式
来源：http://wy.521024.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://sk.shtwfgs.cn

[U56] PHP：命名参数
来源：http://ol.jctech888.com.cn

f(a: 1, b: 2)
来源：http://ho.huanxung.cn

[U57] PHP：字符串插值
来源：http://qt.nszjky.cn

"值: {$a}"
来源：http://ht.panjiajie.cn

[U58] PHP：数组三件套
来源：http://wa.hahajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fi.newstarts.cn

[U59] PHP：自定义排序
来源：http://iv.bjjhwx.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://du.wgjwhj.cn

[U60] PHP：JSON 编解码
来源：http://ro.colortex.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://al.bjjhwx.cn

[U61] PHP：正则
来源：http://az.huanxung.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://at.shxzskj.cn

[U62] PHP：日期对象
来源：http://ws.muxihuayi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pk.yuexingan06.cn

[U63] PHP：文件读写
来源：http://ja.haigaiapp.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://il.muxihuayi.cn

[U64] PHP：目录遍历
来源：http://wz.huixiangedu.cn

glob("dir/*.php");  scandir("dir");
来源：http://gi.shxzskj.cn

[U65] PHP：会话
来源：http://vf.jianghongdianzi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://yg.szsharing.cn

[U66] PHP：设置 Cookie
来源：http://ve.colortex.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jq.muxihuayi.cn

[U67] PHP：处理文件上传
来源：http://rk.szsharing.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fe.shxzskj.cn

[U68] PHP：PDO 连接
来源：http://se.szxytkj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yn.9csxet.cn

[U69] PHP：PDO 预处理
来源：http://vu.hnjuh.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dq.haigaiapp.cn

[U70] PHP：PDO 事务
来源：http://ne.yuntaijiaju.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kr.muxihuayi.cn

[U71] PHP：抛出异常
来源：http://nx.shtwfgs.cn

throw new RuntimeException("失败", 500);
来源：http://bt.muxihuayi.cn

[U72] PHP：写错误日志
来源：http://aj.bookmarksfly.cn

error_log("失败: " . $e->getMessage());
来源：http://ci.haigaiapp.cn

[U73] PHP：读取 ini 配置
来源：http://wk.szxytkj.cn

parse_ini_file("config.ini", true)
来源：http://xa.chemitech.net.cn

[U74] PHP：读取环境变量
来源：http://qn.lnxyls.cn

getenv("APP_ENV") ?: "production"
来源：http://ox.huixiangedu.cn

[U75] PHP：依赖注入
来源：http://dn.jctech888.com.cn

composer require psr/container
来源：http://mg.asd995.cn

[U76] PHP：简单路由
来源：http://qs.szsharing.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kp.asd995.cn

[U77] PHP：模板渲染
来源：http://sj.muxihuayi.cn

composer require twig/twig
来源：http://bi.hahajie.cn

[U78] PHP：单元测试
来源：http://nk.bjjhwx.cn

composer require --dev phpunit/phpunit
来源：http://ef.huixiangedu.cn

[U79] PHP：静态分析
来源：http://mr.gzmigu.cn

composer require --dev phpstan/phpstan
来源：http://cj.szsharing.cn

[U80] PHP：代码规范修复
来源：http://kw.haigaiapp.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qp.wgjwhj.cn

[U81] JS：初始化项目
来源：http://rb.shxzukj.cn

npm init -y;  npm i express
来源：http://ul.9csxet.cn

[U82] JS：package.json 脚本
来源：http://js.yuexingan06.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ot.bookmarksfly.cn


<!-- 参考信息 -->