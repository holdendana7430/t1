代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pz.panjiajie.cn

[S55] C++：结构化绑定
来源：http://us.jianghongdianzi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qr.shxzskj.cn

[S56] C++：optional
来源：http://ag.hahajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fp.chemitech.net.cn

[S57] C++：编译期常量
来源：http://hm.szsharing.cn

constexpr int N = 10;
来源：http://au.hahajie.cn

[S58] C++：命名空间
来源：http://vl.wgjwhj.cn

namespace ns { int f() { return 1; } }
来源：http://hw.shxzskj.cn

[S59] C++：静态断言
来源：http://ji.bjjhwx.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zi.wgjwhj.cn

[S60] C++：遍历并删除元素
来源：http://vv.huanxung.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://po.panjiajie.cn

================================================================================
来源：http://tc.nszjky.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vu.wgjwhj.cn

================================================================================
来源：http://va.yuexingan06.cn

[T01] Kotlin：Hello World
来源：http://ut.hahajie.cn

println("Hello")
来源：http://td.521024.cn

[T02] Kotlin：变量
来源：http://xk.9csxet.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jh.shxzukj.cn

[T03] Kotlin：字符串模板
来源：http://wt.chemitech.net.cn

"值: $b"
来源：http://gq.chemitech.net.cn

[T04] Kotlin：空安全
来源：http://rc.shxzskj.cn

val n: String? = null;  n?.length
来源：http://wo.wgjwhj.cn

[T05] Kotlin：when 表达式
来源：http://jh.chemitech.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qk.huixinmuqiang.cn

[T06] Kotlin：集合映射
来源：http://rd.shxzskj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://lu.shxzskj.cn

[T07] Kotlin：集合过滤
来源：http://my.wgjwhj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wm.panjiajie.cn

[T08] Kotlin：数据类
来源：http://mv.colortex.cn

data class User(val name: String, val age: Int)
来源：http://gu.shxzukj.cn

[T09] Kotlin：扩展函数
来源：http://vy.bookmarksfly.cn

fun String.exclaim() = this + "!"
来源：http://hb.shxzskj.cn

[T10] Kotlin：默认参数
来源：http://hu.hnjuh.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qm.asd995.cn

[T11] Kotlin：协程
来源：http://qt.szxytkj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://dy.szxytkj.cn

[T12] Kotlin：解构声明
来源：http://lu.asd995.cn

val (a, b) = Pair(1, 2)
来源：http://rp.hahajie.cn

[T13] Kotlin：只读 Map
来源：http://pp.szsharing.cn

val m = mapOf("a" to 1)
来源：http://ko.9csxet.cn

[T14] Kotlin：循环
来源：http://xv.huixiangedu.cn

for (i in 1..10) println(i)
来源：http://qh.nicolike.cn

[T15] Kotlin：接口
来源：http://gp.newstarts.cn

interface Shape { fun area(): Double }
来源：http://ll.yuntaijiaju.cn

[T16] Swift：Hello World
来源：http://zz.jianghongdianzi.cn

print("Hello")
来源：http://ia.muxihuayi.cn

[T17] Swift：变量与常量
来源：http://ad.yuexingan06.cn

var a = 1;  let b = 2
来源：http://iw.huixinmuqiang.cn

[T18] Swift：字符串插值
来源：http://tk.yuexingan06.cn

"值: \(b)"
来源：http://qw.colortex.cn

[T19] Swift：可选绑定
来源：http://yb.lnxyls.cn

if let n = opt { print(n) }
来源：http://zi.hahajie.cn

[T20] Swift：数组操作
来源：http://tr.asd995.cn

var a = [1, 2, 3];  a.append(4)
来源：http://dg.panjiajie.cn

[T21] Swift：遍历
来源：http://dt.9csxet.cn

for x in a { print(x) }
来源：http://ew.huanxung.cn

[T22] Swift：字典
来源：http://km.shxzukj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://yn.muxihuayi.cn

[T23] Swift：函数
来源：http://ia.szxytkj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qj.lnxyls.cn

[T24] Swift：闭包
来源：http://zx.colortex.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://tp.newstarts.cn

[T25] Swift：结构体
来源：http://xy.szxytkj.cn

struct P { var x: Int }
来源：http://ow.shxzukj.cn

[T26] Swift：类与重写
来源：http://qt.gzmigu.cn

class A: Base { override func f() {} }
来源：http://bm.nszjky.cn

[T27] Swift：错误处理
来源：http://hw.jctech888.com.cn

do { try f() } catch { print(error) }
来源：http://xm.jctech888.com.cn

[T28] Swift：枚举
来源：http://ux.szxytkj.cn

enum Color { case red, green }
来源：http://is.colortex.cn

[T29] Swift：guard 提前返回
来源：http://bn.shtwfgs.cn

guard let x = opt else { return }
来源：http://fs.jctech888.com.cn

[T30] Swift：协议
来源：http://jb.lnxyls.cn

protocol Shape { func area() -> Double }
来源：http://la.hahajie.cn

[T31] Lua：Hello World
来源：http://nq.shxzukj.cn

print("Hello")
来源：http://wy.hnjuh.cn

[T32] Lua：局部变量
来源：http://fm.shtwfgs.cn

local a = 1
来源：http://he.shxzskj.cn

[T33] Lua：表（数组）
来源：http://ao.jctech888.com.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://aq.szsharing.cn

[T34] Lua：遍历表
来源：http://yo.huanxung.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ai.9csxet.cn

[T35] Lua：字典表
来源：http://fu.panjiajie.cn

local d = { a = 1 };  d.b = 2
来源：http://hd.bookmarksfly.cn

[T36] Lua：函数
来源：http://vu.szsharing.cn

function add(a, b) return a + b end
来源：http://yb.nicolike.cn

[T37] Lua：字符串拼接
来源：http://yy.muxihuayi.cn

"a" .. "b"
来源：http://ft.chemitech.net.cn

[T38] Lua：条件
来源：http://zo.yuexingan06.cn

if x > 0 then print("正") end
来源：http://jr.shxzukj.cn

[T39] Lua：模式匹配
来源：http://on.haigaiapp.cn

string.find(s, "%d+")
来源：http://yf.szsharing.cn

[T40] Lua：元表
来源：http://oz.hnjuh.cn

setmetatable({}, { __index = base })
来源：http://yj.9csxet.cn

[T41] Perl：Hello World
来源：http://ua.nicolike.cn

print "Hello\n";
来源：http://pp.szxytkj.cn

[T42] Perl：变量类型
来源：http://nx.shtwfgs.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fu.szxytkj.cn

[T43] Perl：字符串插值
来源：http://zz.jianghongdianzi.cn

"值: $a"
来源：http://zs.colortex.cn

[T44] Perl：条件
来源：http://up.panjiajie.cn

if ($a > 0) { print "正"; }
来源：http://nw.lnxyls.cn

[T45] Perl：数组遍历
来源：http://zs.chemitech.net.cn

for my $x (@arr) { print $x; }
来源：http://st.lnxyls.cn

[T46] Perl：哈希操作
来源：http://rp.jianghongdianzi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mb.shxzukj.cn

[T47] Perl：正则捕获
来源：http://ky.szsharing.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pi.szxytkj.cn

[T48] Perl：正则替换
来源：http://op.9csxet.cn

$s =~ s/old/new/g;
来源：http://wd.hnjuh.cn

[T49] Perl：函数
来源：http://jj.shxzskj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mw.hahajie.cn

[T50] Perl：逐行读文件
来源：http://dg.nicolike.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rh.huixinmuqiang.cn

while (my $line = <$fh>) { print $line; }
来源：http://vj.huixinmuqiang.cn

[T51] Scala：Hello World
来源：http://hx.jianghongdianzi.cn

println("Hello")
来源：http://um.521024.cn

[T52] Scala：变量
来源：http://wr.yuexingan06.cn

val a = 1;  var b = 2
来源：http://vv.nszjky.cn

[T53] Scala：字符串插值
来源：http://fm.jctech888.com.cn

s"值: $b"
来源：http://yc.hnjuh.cn

[T54] Scala：集合映射
来源：http://md.yuexingan06.cn

List(1, 2, 3).map(_ * 2)
来源：http://su.9csxet.cn

[T55] Scala：集合过滤
来源：http://dq.haigaiapp.cn

List(1, 2, 3).filter(_ > 1)
来源：http://me.shxzukj.cn

[T56] Scala：样例类
来源：http://fe.shtwfgs.cn

case class User(name: String, age: Int)
来源：http://zf.hnjuh.cn

[T57] Scala：模式匹配
来源：http://pm.colortex.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://uu.9csxet.cn

[T58] Scala：函数定义
来源：http://wu.haigaiapp.cn

def add(a: Int, b: Int): Int = a + b
来源：http://eb.haigaiapp.cn

[T59] Scala：循环
来源：http://qm.panjiajie.cn

for (i <- 1 to 10) println(i)
来源：http://lf.jctech888.com.cn

[T60] Scala：折叠
来源：http://qh.asd995.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vc.szsharing.cn

================================================================================
来源：http://mm.yuexingan06.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kh.panjiajie.cn

================================================================================
来源：http://ap.521024.cn

[U01] Py：创建虚拟环境
来源：http://qs.yuntaijiaju.cn

python -m venv .venv && source .venv/bin/activate
来源：http://np.bookmarksfly.cn

[U02] Py：导出 / 安装依赖
来源：http://ae.haigaiapp.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zk.hnjuh.cn

[U03] Py：加载 .env 配置
来源：http://nm.szsharing.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ky.wgjwhj.cn

[U04] Py：变量调试打印
来源：http://sy.jctech888.com.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ai.yuntaijiaju.cn

[U05] Py：列表去重且保序
来源：http://mb.huixiangedu.cn

list(dict.fromkeys(arr))
来源：http://ti.szxytkj.cn

[U06] Py：合并两个字典
来源：http://zr.newstarts.cn

{**a, **b}
来源：http://xm.jianghongdianzi.cn

[U07] Py：反转字典键值
来源：http://vz.szxytkj.cn

{v: k for k, v in d.items()}
来源：http://gv.hahajie.cn

[U08] Py：展平二维列表
来源：http://iu.asd995.cn

[y for x in nested for y in x]
来源：http://kk.gzmigu.cn

[U09] Py：字典取最大值的键
来源：http://ui.bjjhwx.cn

max(d, key=d.get)
来源：http://hd.shxzukj.cn

[U10] Py：按值排序字典
来源：http://aa.nszjky.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://js.haigaiapp.cn

[U11] Py：生成器表达式
来源：http://cw.hahajie.cn

(x * 2 for x in arr)
来源：http://se.haigaiapp.cn

[U12] Py：取出现最多的 3 个元素
来源：http://nt.asd995.cn

Counter(arr).most_common(3)
来源：http://zf.yuntaijiaju.cn

[U13] Py：固定长度队列
来源：http://yw.asd995.cn

deque(maxlen=10)
来源：http://gm.bookmarksfly.cn

[U14] Py：分组收集到列表
来源：http://fk.huixinmuqiang.cn

defaultdict(list)
来源：http://cw.nicolike.cn

[U15] Py：高精度计时
来源：http://tp.yuexingan06.cn

t = time.perf_counter()
来源：http://yr.shxzskj.cn

[U16] Py：命令行参数解析
来源：http://el.panjiajie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zv.bookmarksfly.cn

[U17] Py：初始化日志
来源：http://hn.wgjwhj.cn

logging.basicConfig(level=logging.INFO)
来源：http://xs.wgjwhj.cn

[U18] Py：预编译正则
来源：http://bf.9csxet.cn

pat = re.compile(r"\d+")
来源：http://sv.shxzukj.cn

[U19] Py：正则替换带回调
来源：http://av.bookmarksfly.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lz.bjjhwx.cn

[U20] Py：缓存函数结果
来源：http://sw.panjiajie.cn

@functools.lru_cache(maxsize=None)
来源：http://xq.jctech888.com.cn

[U21] Py：自定义上下文管理器
来源：http://vj.yuexingan06.cn

@contextlib.contextmanager
来源：http://av.haigaiapp.cn

[U22] Py：矩阵转置
来源：http://gl.haigaiapp.cn

list(zip(*m))
来源：http://lx.huanxung.cn

[U23] Py：分块读取大文件
来源：http://kw.wgjwhj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ts.jctech888.com.cn

[U24] Py：路径操作
来源：http://ul.haigaiapp.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mv.shtwfgs.cn

[U25] Py：CSV 按字典读
来源：http://kh.lnxyls.cn

csv.DictReader(f)
来源：http://dh.jctech888.com.cn

[U26] Py：并发下载
来源：http://cp.huixiangedu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mf.huanxung.cn

[U27] Py：异步 HTTP
来源：http://wo.huixiangedu.cn

aiohttp.ClientSession() 配合 async with
来源：http://kv.gzmigu.cn

[U28] Py：类型别名
来源：http://kh.colortex.cn

UserId = int
来源：http://ek.huixinmuqiang.cn

[U29] Py：属性校验
来源：http://nv.huixiangedu.cn

@property 与 @x.setter 配合
来源：http://wm.gzmigu.cn

[U30] Py：数据类
来源：http://mv.szxytkj.cn

@dataclass(slots=True)
来源：http://kp.muxihuayi.cn

[U31] Py：单测
来源：http://lo.panjiajie.cn

python -m pytest -q
来源：http://sv.haigaiapp.cn

[U32] Py：代码格式化
来源：http://hx.521024.cn

ruff format . && ruff check --fix .
来源：http://mc.521024.cn

[U33] Py：打包发布
来源：http://no.bjjhwx.cn

python -m build  （依赖 pyproject.toml）
来源：http://lc.shtwfgs.cn

[U34] Py：判断编码
来源：http://dn.jianghongdianzi.cn

chardet.detect(raw)
来源：http://kr.panjiajie.cn

[U35] Py：发送邮件
来源：http://lt.szxytkj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://et.nicolike.cn

[U36] Py：定时任务
来源：http://qb.yuexingan06.cn

schedule.every(10).minutes.do(job)
来源：http://pv.yuexingan06.cn

[U37] Py：读写 Excel
来源：http://hy.wgjwhj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://yy.nszjky.cn

[U38] Py：获取脚本所在目录
来源：http://ut.yuexingan06.cn

Path(__file__).resolve().parent
来源：http://si.lnxyls.cn

[U39] Py：判断是否在交互环境
来源：http://yp.hahajie.cn

sys.stdout.isatty()
来源：http://ky.huixinmuqiang.cn

[U40] Py：打印到标准错误
来源：http://yu.asd995.cn

print("err", file=sys.stderr)
来源：http://hj.szxytkj.cn

[U41] PHP：初始化 Composer 项目
来源：http://xj.yuntaijiaju.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://da.newstarts.cn

[U42] PHP：PSR-4 自动加载
来源：http://ew.shxzskj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yg.shxzukj.cn

[U43] PHP：声明命名空间
来源：http://ob.hnjuh.cn

namespace App\Http;
来源：http://sh.wgjwhj.cn

[U44] PHP：开启严格类型
来源：http://dj.newstarts.cn

declare(strict_types=1);
来源：http://sq.lnxyls.cn

[U45] PHP：类型声明与返回类型
来源：http://sh.gzmigu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://fz.bjjhwx.cn

[U46] PHP：可空类型
来源：http://nu.jianghongdianzi.cn

?string $name = null
来源：http://ge.hnjuh.cn

[U47] PHP：联合类型
来源：http://ss.huixiangedu.cn

int|string $id
来源：http://fz.newstarts.cn

[U48] PHP：纯枚举
来源：http://ex.nicolike.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xz.huanxung.cn

[U49] PHP：只读属性
来源：http://jd.shtwfgs.cn

public readonly string $name
来源：http://hg.muxihuayi.cn

[U50] PHP：构造器属性提升
来源：http://uo.chemitech.net.cn

public function __construct(private int $id) {}
来源：http://lh.huixiangedu.cn

[U51] PHP：数组解构
来源：http://xw.hnjuh.cn

[$a, $b] = $arr;
来源：http://gy.haigaiapp.cn

[U52] PHP：箭头函数
来源：http://xx.bjjhwx.cn

$double = fn($x) => $x * 2;
来源：http://vs.bookmarksfly.cn

[U53] PHP：空合并运算符
来源：http://dq.nszjky.cn

$v = $a ?? $b ?? "default";
来源：http://tr.wgjwhj.cn

[U54] PHP：空安全调用
来源：http://wm.asd995.cn

$obj?->method()
来源：http://si.wgjwhj.cn

[U55] PHP：match 表达式
来源：http://gd.haigaiapp.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fh.newstarts.cn

[U56] PHP：命名参数
来源：http://ie.wgjwhj.cn

f(a: 1, b: 2)
来源：http://id.9csxet.cn

[U57] PHP：字符串插值
来源：http://to.huixiangedu.cn

"值: {$a}"
来源：http://gu.shxzskj.cn

[U58] PHP：数组三件套
来源：http://ua.nicolike.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pu.521024.cn

[U59] PHP：自定义排序
来源：http://pl.9csxet.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pu.yuntaijiaju.cn

[U60] PHP：JSON 编解码
来源：http://sr.bjjhwx.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ab.jianghongdianzi.cn

[U61] PHP：正则
来源：http://ch.panjiajie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pv.hahajie.cn

[U62] PHP：日期对象
来源：http://xc.huanxung.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xm.yuntaijiaju.cn

[U63] PHP：文件读写
来源：http://zi.yuexingan06.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://me.szxytkj.cn

[U64] PHP：目录遍历
来源：http://ex.szxytkj.cn

glob("dir/*.php");  scandir("dir");
来源：http://hw.lnxyls.cn

[U65] PHP：会话
来源：http://fb.hnjuh.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://lc.bjjhwx.cn

[U66] PHP：设置 Cookie
来源：http://oh.szxytkj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sc.yuntaijiaju.cn

[U67] PHP：处理文件上传
来源：http://ix.jctech888.com.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dl.jianghongdianzi.cn

[U68] PHP：PDO 连接
来源：http://ya.jctech888.com.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yz.chemitech.net.cn

[U69] PHP：PDO 预处理
来源：http://gg.newstarts.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ke.nszjky.cn

[U70] PHP：PDO 事务
来源：http://bj.huixinmuqiang.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yd.yuntaijiaju.cn

[U71] PHP：抛出异常
来源：http://rs.colortex.cn

throw new RuntimeException("失败", 500);
来源：http://ij.huanxung.cn

[U72] PHP：写错误日志
来源：http://ub.newstarts.cn

error_log("失败: " . $e->getMessage());
来源：http://ak.wgjwhj.cn

[U73] PHP：读取 ini 配置
来源：http://od.lnxyls.cn

parse_ini_file("config.ini", true)
来源：http://ix.521024.cn

[U74] PHP：读取环境变量
来源：http://bh.yuntaijiaju.cn

getenv("APP_ENV") ?: "production"
来源：http://na.9csxet.cn

[U75] PHP：依赖注入
来源：http://kz.asd995.cn

composer require psr/container
来源：http://cn.huanxung.cn

[U76] PHP：简单路由
来源：http://bz.newstarts.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ir.bjjhwx.cn

[U77] PHP：模板渲染
来源：http://za.shtwfgs.cn

composer require twig/twig
来源：http://qo.shxzukj.cn

[U78] PHP：单元测试
来源：http://ew.asd995.cn

composer require --dev phpunit/phpunit
来源：http://vk.bookmarksfly.cn

[U79] PHP：静态分析
来源：http://et.yuexingan06.cn

composer require --dev phpstan/phpstan
来源：http://to.nicolike.cn

[U80] PHP：代码规范修复
来源：http://uw.szsharing.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://tv.9csxet.cn


<!-- 参考信息 -->