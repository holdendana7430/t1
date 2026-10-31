代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://te.jianghongdianzi.cn

[S57] C++：编译期常量
来源：http://ei.shxzukj.cn

constexpr int N = 10;
来源：http://on.hnjuh.cn

[S58] C++：命名空间
来源：http://hh.jianghongdianzi.cn

namespace ns { int f() { return 1; } }
来源：http://xe.colortex.cn

[S59] C++：静态断言
来源：http://ph.yuexingan06.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kg.muxihuayi.cn

[S60] C++：遍历并删除元素
来源：http://ds.newstarts.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cz.nicolike.cn

================================================================================
来源：http://ci.gzmigu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rf.hnjuh.cn

================================================================================
来源：http://fe.yuexingan06.cn

[T01] Kotlin：Hello World
来源：http://zl.nicolike.cn

println("Hello")
来源：http://mx.shxzukj.cn

[T02] Kotlin：变量
来源：http://mr.yuntaijiaju.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xs.asd995.cn

[T03] Kotlin：字符串模板
来源：http://sy.haigaiapp.cn

"值: $b"
来源：http://wz.colortex.cn

[T04] Kotlin：空安全
来源：http://lq.haigaiapp.cn

val n: String? = null;  n?.length
来源：http://dw.szsharing.cn

[T05] Kotlin：when 表达式
来源：http://yj.asd995.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://af.lnxyls.cn

[T06] Kotlin：集合映射
来源：http://dh.gzmigu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ox.shtwfgs.cn

[T07] Kotlin：集合过滤
来源：http://th.panjiajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ja.wgjwhj.cn

[T08] Kotlin：数据类
来源：http://dt.asd995.cn

data class User(val name: String, val age: Int)
来源：http://gx.nicolike.cn

[T09] Kotlin：扩展函数
来源：http://eb.nicolike.cn

fun String.exclaim() = this + "!"
来源：http://zx.huanxung.cn

[T10] Kotlin：默认参数
来源：http://bl.hahajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://oa.nszjky.cn

[T11] Kotlin：协程
来源：http://zi.yuexingan06.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ya.huixinmuqiang.cn

[T12] Kotlin：解构声明
来源：http://gn.yuexingan06.cn

val (a, b) = Pair(1, 2)
来源：http://ty.huixinmuqiang.cn

[T13] Kotlin：只读 Map
来源：http://wj.521024.cn

val m = mapOf("a" to 1)
来源：http://qm.haigaiapp.cn

[T14] Kotlin：循环
来源：http://qe.gzmigu.cn

for (i in 1..10) println(i)
来源：http://la.huixiangedu.cn

[T15] Kotlin：接口
来源：http://xl.521024.cn

interface Shape { fun area(): Double }
来源：http://pp.yuntaijiaju.cn

[T16] Swift：Hello World
来源：http://xo.nicolike.cn

print("Hello")
来源：http://lx.lnxyls.cn

[T17] Swift：变量与常量
来源：http://rj.9csxet.cn

var a = 1;  let b = 2
来源：http://wj.hnjuh.cn

[T18] Swift：字符串插值
来源：http://nl.shxzskj.cn

"值: \(b)"
来源：http://cp.521024.cn

[T19] Swift：可选绑定
来源：http://tm.szsharing.cn

if let n = opt { print(n) }
来源：http://sh.hnjuh.cn

[T20] Swift：数组操作
来源：http://qy.bookmarksfly.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ic.jianghongdianzi.cn

[T21] Swift：遍历
来源：http://kv.chemitech.net.cn

for x in a { print(x) }
来源：http://df.hnjuh.cn

[T22] Swift：字典
来源：http://sx.bjjhwx.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ee.szxytkj.cn

[T23] Swift：函数
来源：http://cx.shtwfgs.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bb.shxzskj.cn

[T24] Swift：闭包
来源：http://on.panjiajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gf.haigaiapp.cn

[T25] Swift：结构体
来源：http://hj.bookmarksfly.cn

struct P { var x: Int }
来源：http://ik.nicolike.cn

[T26] Swift：类与重写
来源：http://zz.shxzukj.cn

class A: Base { override func f() {} }
来源：http://kq.jianghongdianzi.cn

[T27] Swift：错误处理
来源：http://qn.shxzukj.cn

do { try f() } catch { print(error) }
来源：http://wh.colortex.cn

[T28] Swift：枚举
来源：http://or.yuntaijiaju.cn

enum Color { case red, green }
来源：http://ky.nszjky.cn

[T29] Swift：guard 提前返回
来源：http://ma.muxihuayi.cn

guard let x = opt else { return }
来源：http://sz.9csxet.cn

[T30] Swift：协议
来源：http://my.shtwfgs.cn

protocol Shape { func area() -> Double }
来源：http://ee.szxytkj.cn

[T31] Lua：Hello World
来源：http://xq.gzmigu.cn

print("Hello")
来源：http://pe.colortex.cn

[T32] Lua：局部变量
来源：http://cr.9csxet.cn

local a = 1
来源：http://ec.jctech888.com.cn

[T33] Lua：表（数组）
来源：http://me.shxzskj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://cp.yuexingan06.cn

[T34] Lua：遍历表
来源：http://qs.muxihuayi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://jw.bjjhwx.cn

[T35] Lua：字典表
来源：http://gl.521024.cn

local d = { a = 1 };  d.b = 2
来源：http://ly.muxihuayi.cn

[T36] Lua：函数
来源：http://vo.521024.cn

function add(a, b) return a + b end
来源：http://ff.shtwfgs.cn

[T37] Lua：字符串拼接
来源：http://ns.bookmarksfly.cn

"a" .. "b"
来源：http://se.521024.cn

[T38] Lua：条件
来源：http://zc.newstarts.cn

if x > 0 then print("正") end
来源：http://kf.521024.cn

[T39] Lua：模式匹配
来源：http://qj.9csxet.cn

string.find(s, "%d+")
来源：http://jh.gzmigu.cn

[T40] Lua：元表
来源：http://et.jctech888.com.cn

setmetatable({}, { __index = base })
来源：http://dj.nicolike.cn

[T41] Perl：Hello World
来源：http://ei.jctech888.com.cn

print "Hello\n";
来源：http://uf.szxytkj.cn

[T42] Perl：变量类型
来源：http://ds.haigaiapp.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cl.huixinmuqiang.cn

[T43] Perl：字符串插值
来源：http://xg.szxytkj.cn

"值: $a"
来源：http://ws.chemitech.net.cn

[T44] Perl：条件
来源：http://ak.nszjky.cn

if ($a > 0) { print "正"; }
来源：http://gn.jianghongdianzi.cn

[T45] Perl：数组遍历
来源：http://uw.asd995.cn

for my $x (@arr) { print $x; }
来源：http://jw.hnjuh.cn

[T46] Perl：哈希操作
来源：http://it.yuntaijiaju.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mi.jctech888.com.cn

[T47] Perl：正则捕获
来源：http://xy.huixinmuqiang.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://hc.colortex.cn

[T48] Perl：正则替换
来源：http://vi.bookmarksfly.cn

$s =~ s/old/new/g;
来源：http://al.huanxung.cn

[T49] Perl：函数
来源：http://qj.gzmigu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cn.colortex.cn

[T50] Perl：逐行读文件
来源：http://uu.shxzskj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://oj.muxihuayi.cn

while (my $line = <$fh>) { print $line; }
来源：http://mv.lnxyls.cn

[T51] Scala：Hello World
来源：http://cx.szsharing.cn

println("Hello")
来源：http://wf.shxzukj.cn

[T52] Scala：变量
来源：http://ua.huixiangedu.cn

val a = 1;  var b = 2
来源：http://sj.hnjuh.cn

[T53] Scala：字符串插值
来源：http://jq.panjiajie.cn

s"值: $b"
来源：http://xr.nszjky.cn

[T54] Scala：集合映射
来源：http://sq.hahajie.cn

List(1, 2, 3).map(_ * 2)
来源：http://bx.gzmigu.cn

[T55] Scala：集合过滤
来源：http://xm.panjiajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wq.haigaiapp.cn

[T56] Scala：样例类
来源：http://mc.shtwfgs.cn

case class User(name: String, age: Int)
来源：http://gt.colortex.cn

[T57] Scala：模式匹配
来源：http://fq.szsharing.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://of.yuntaijiaju.cn

[T58] Scala：函数定义
来源：http://db.9csxet.cn

def add(a: Int, b: Int): Int = a + b
来源：http://vz.jianghongdianzi.cn

[T59] Scala：循环
来源：http://ae.9csxet.cn

for (i <- 1 to 10) println(i)
来源：http://pq.shxzukj.cn

[T60] Scala：折叠
来源：http://oh.nicolike.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zv.lnxyls.cn

================================================================================
来源：http://pk.huanxung.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fp.huixinmuqiang.cn

================================================================================
来源：http://pq.yuexingan06.cn

[U01] Py：创建虚拟环境
来源：http://gy.gzmigu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bw.gzmigu.cn

[U02] Py：导出 / 安装依赖
来源：http://az.panjiajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://oz.huanxung.cn

[U03] Py：加载 .env 配置
来源：http://oa.asd995.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rb.521024.cn

[U04] Py：变量调试打印
来源：http://gp.hahajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vb.lnxyls.cn

[U05] Py：列表去重且保序
来源：http://gt.chemitech.net.cn

list(dict.fromkeys(arr))
来源：http://zk.nszjky.cn

[U06] Py：合并两个字典
来源：http://pq.bjjhwx.cn

{**a, **b}
来源：http://do.yuntaijiaju.cn

[U07] Py：反转字典键值
来源：http://za.colortex.cn

{v: k for k, v in d.items()}
来源：http://cs.chemitech.net.cn

[U08] Py：展平二维列表
来源：http://jq.9csxet.cn

[y for x in nested for y in x]
来源：http://ne.bookmarksfly.cn

[U09] Py：字典取最大值的键
来源：http://oo.jctech888.com.cn

max(d, key=d.get)
来源：http://pj.wgjwhj.cn

[U10] Py：按值排序字典
来源：http://ww.hnjuh.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cu.bjjhwx.cn

[U11] Py：生成器表达式
来源：http://io.szsharing.cn

(x * 2 for x in arr)
来源：http://qg.huixiangedu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rw.hahajie.cn

Counter(arr).most_common(3)
来源：http://ym.nszjky.cn

[U13] Py：固定长度队列
来源：http://bn.521024.cn

deque(maxlen=10)
来源：http://qo.panjiajie.cn

[U14] Py：分组收集到列表
来源：http://kp.nszjky.cn

defaultdict(list)
来源：http://oq.hnjuh.cn

[U15] Py：高精度计时
来源：http://om.hahajie.cn

t = time.perf_counter()
来源：http://yx.gzmigu.cn

[U16] Py：命令行参数解析
来源：http://jj.huixiangedu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zc.jctech888.com.cn

[U17] Py：初始化日志
来源：http://nv.hahajie.cn

logging.basicConfig(level=logging.INFO)
来源：http://pi.colortex.cn

[U18] Py：预编译正则
来源：http://qh.hnjuh.cn

pat = re.compile(r"\d+")
来源：http://gf.nicolike.cn

[U19] Py：正则替换带回调
来源：http://dm.bjjhwx.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gb.haigaiapp.cn

[U20] Py：缓存函数结果
来源：http://ki.huixinmuqiang.cn

@functools.lru_cache(maxsize=None)
来源：http://yw.hahajie.cn

[U21] Py：自定义上下文管理器
来源：http://gd.521024.cn

@contextlib.contextmanager
来源：http://ug.huixiangedu.cn

[U22] Py：矩阵转置
来源：http://zd.chemitech.net.cn

list(zip(*m))
来源：http://hg.bjjhwx.cn

[U23] Py：分块读取大文件
来源：http://ie.521024.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cn.shxzskj.cn

[U24] Py：路径操作
来源：http://wd.huixinmuqiang.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rk.hnjuh.cn

[U25] Py：CSV 按字典读
来源：http://iz.lnxyls.cn

csv.DictReader(f)
来源：http://ko.9csxet.cn

[U26] Py：并发下载
来源：http://vg.bookmarksfly.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ck.yuexingan06.cn

[U27] Py：异步 HTTP
来源：http://hv.szxytkj.cn

aiohttp.ClientSession() 配合 async with
来源：http://sh.jctech888.com.cn

[U28] Py：类型别名
来源：http://sv.jctech888.com.cn

UserId = int
来源：http://ev.521024.cn

[U29] Py：属性校验
来源：http://tm.hnjuh.cn

@property 与 @x.setter 配合
来源：http://mt.panjiajie.cn

[U30] Py：数据类
来源：http://ov.szxytkj.cn

@dataclass(slots=True)
来源：http://lv.szsharing.cn

[U31] Py：单测
来源：http://vv.nicolike.cn

python -m pytest -q
来源：http://uo.jianghongdianzi.cn

[U32] Py：代码格式化
来源：http://vz.nicolike.cn

ruff format . && ruff check --fix .
来源：http://wj.nszjky.cn

[U33] Py：打包发布
来源：http://sm.szsharing.cn

python -m build  （依赖 pyproject.toml）
来源：http://bz.shxzukj.cn

[U34] Py：判断编码
来源：http://nx.jianghongdianzi.cn

chardet.detect(raw)
来源：http://hy.shxzskj.cn

[U35] Py：发送邮件
来源：http://tk.9csxet.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wr.muxihuayi.cn

[U36] Py：定时任务
来源：http://ee.hahajie.cn

schedule.every(10).minutes.do(job)
来源：http://kt.nszjky.cn

[U37] Py：读写 Excel
来源：http://co.panjiajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qg.newstarts.cn

[U38] Py：获取脚本所在目录
来源：http://vx.shxzskj.cn

Path(__file__).resolve().parent
来源：http://wp.shxzskj.cn

[U39] Py：判断是否在交互环境
来源：http://xc.shxzukj.cn

sys.stdout.isatty()
来源：http://yr.bjjhwx.cn

[U40] Py：打印到标准错误
来源：http://qi.jctech888.com.cn

print("err", file=sys.stderr)
来源：http://zs.jianghongdianzi.cn

[U41] PHP：初始化 Composer 项目
来源：http://wd.szsharing.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://cf.huanxung.cn

[U42] PHP：PSR-4 自动加载
来源：http://vz.nszjky.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zb.jianghongdianzi.cn

[U43] PHP：声明命名空间
来源：http://me.9csxet.cn

namespace App\Http;
来源：http://fg.521024.cn

[U44] PHP：开启严格类型
来源：http://rs.asd995.cn

declare(strict_types=1);
来源：http://ar.panjiajie.cn

[U45] PHP：类型声明与返回类型
来源：http://sl.huanxung.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://kj.nszjky.cn

[U46] PHP：可空类型
来源：http://br.panjiajie.cn

?string $name = null
来源：http://kd.yuexingan06.cn

[U47] PHP：联合类型
来源：http://nx.shtwfgs.cn

int|string $id
来源：http://dr.gzmigu.cn

[U48] PHP：纯枚举
来源：http://pm.yuntaijiaju.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jr.521024.cn

[U49] PHP：只读属性
来源：http://ed.szsharing.cn

public readonly string $name
来源：http://zl.bookmarksfly.cn

[U50] PHP：构造器属性提升
来源：http://qq.yuexingan06.cn

public function __construct(private int $id) {}
来源：http://mz.gzmigu.cn

[U51] PHP：数组解构
来源：http://bj.muxihuayi.cn

[$a, $b] = $arr;
来源：http://fc.haigaiapp.cn

[U52] PHP：箭头函数
来源：http://ui.muxihuayi.cn

$double = fn($x) => $x * 2;
来源：http://vn.9csxet.cn

[U53] PHP：空合并运算符
来源：http://sn.9csxet.cn

$v = $a ?? $b ?? "default";
来源：http://eh.nicolike.cn

[U54] PHP：空安全调用
来源：http://so.bjjhwx.cn

$obj?->method()
来源：http://db.hahajie.cn

[U55] PHP：match 表达式
来源：http://ro.huixiangedu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://am.9csxet.cn

[U56] PHP：命名参数
来源：http://pf.9csxet.cn

f(a: 1, b: 2)
来源：http://vd.newstarts.cn

[U57] PHP：字符串插值
来源：http://zj.wgjwhj.cn

"值: {$a}"
来源：http://vp.huanxung.cn

[U58] PHP：数组三件套
来源：http://dm.yuntaijiaju.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ni.asd995.cn

[U59] PHP：自定义排序
来源：http://si.bjjhwx.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://av.chemitech.net.cn

[U60] PHP：JSON 编解码
来源：http://mj.shxzukj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kr.colortex.cn

[U61] PHP：正则
来源：http://pj.jianghongdianzi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jh.9csxet.cn

[U62] PHP：日期对象
来源：http://nv.huixinmuqiang.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://to.nicolike.cn

[U63] PHP：文件读写
来源：http://fp.haigaiapp.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lt.nicolike.cn

[U64] PHP：目录遍历
来源：http://bq.nszjky.cn

glob("dir/*.php");  scandir("dir");
来源：http://jm.shtwfgs.cn

[U65] PHP：会话
来源：http://dx.muxihuayi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://mi.hnjuh.cn

[U66] PHP：设置 Cookie
来源：http://ys.shtwfgs.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://as.nicolike.cn

[U67] PHP：处理文件上传
来源：http://nj.shtwfgs.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nx.yuexingan06.cn

[U68] PHP：PDO 连接
来源：http://lw.shxzskj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kr.huixiangedu.cn

[U69] PHP：PDO 预处理
来源：http://gc.huanxung.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://li.chemitech.net.cn

[U70] PHP：PDO 事务
来源：http://js.gzmigu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mv.9csxet.cn

[U71] PHP：抛出异常
来源：http://js.yuntaijiaju.cn

throw new RuntimeException("失败", 500);
来源：http://hv.lnxyls.cn

[U72] PHP：写错误日志
来源：http://fz.jctech888.com.cn

error_log("失败: " . $e->getMessage());
来源：http://pq.gzmigu.cn

[U73] PHP：读取 ini 配置
来源：http://fj.yuntaijiaju.cn

parse_ini_file("config.ini", true)
来源：http://jc.bookmarksfly.cn

[U74] PHP：读取环境变量
来源：http://up.huanxung.cn

getenv("APP_ENV") ?: "production"
来源：http://bg.jctech888.com.cn

[U75] PHP：依赖注入
来源：http://sy.bookmarksfly.cn

composer require psr/container
来源：http://cp.huanxung.cn

[U76] PHP：简单路由
来源：http://mn.haigaiapp.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gp.gzmigu.cn

[U77] PHP：模板渲染
来源：http://fb.9csxet.cn

composer require twig/twig
来源：http://kd.bookmarksfly.cn

[U78] PHP：单元测试
来源：http://gh.bookmarksfly.cn

composer require --dev phpunit/phpunit
来源：http://sc.bjjhwx.cn

[U79] PHP：静态分析
来源：http://eo.hnjuh.cn

composer require --dev phpstan/phpstan
来源：http://to.asd995.cn

[U80] PHP：代码规范修复
来源：http://rj.szsharing.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://bd.jctech888.com.cn

[U81] JS：初始化项目
来源：http://sr.jianghongdianzi.cn

npm init -y;  npm i express
来源：http://ty.shtwfgs.cn

[U82] JS：package.json 脚本
来源：http://ub.huanxung.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wk.lnxyls.cn


<!-- 参考信息 -->