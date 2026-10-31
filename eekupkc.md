代发 wailian999

int size() const noexcept { return n_; }
来源：http://uz.9csxet.cn

[S53] C++：移动语义
来源：http://pb.huixinmuqiang.cn

std::vector<int> w = std::move(v);
来源：http://kg.colortex.cn

[S54] C++：异常处理
来源：http://hc.lnxyls.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rn.jianghongdianzi.cn

[S55] C++：结构化绑定
来源：http://wk.hahajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mf.chemitech.net.cn

[S56] C++：optional
来源：http://um.nszjky.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ml.shxzskj.cn

[S57] C++：编译期常量
来源：http://ta.lnxyls.cn

constexpr int N = 10;
来源：http://df.9csxet.cn

[S58] C++：命名空间
来源：http://rb.haigaiapp.cn

namespace ns { int f() { return 1; } }
来源：http://rv.hahajie.cn

[S59] C++：静态断言
来源：http://yn.nicolike.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://oz.yuntaijiaju.cn

[S60] C++：遍历并删除元素
来源：http://gj.asd995.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pe.huixiangedu.cn

================================================================================
来源：http://py.newstarts.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qc.nicolike.cn

================================================================================
来源：http://ka.wgjwhj.cn

[T01] Kotlin：Hello World
来源：http://sn.yuexingan06.cn

println("Hello")
来源：http://dp.jianghongdianzi.cn

[T02] Kotlin：变量
来源：http://yc.bjjhwx.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vr.jianghongdianzi.cn

[T03] Kotlin：字符串模板
来源：http://ig.szsharing.cn

"值: $b"
来源：http://tz.muxihuayi.cn

[T04] Kotlin：空安全
来源：http://jh.wgjwhj.cn

val n: String? = null;  n?.length
来源：http://hd.lnxyls.cn

[T05] Kotlin：when 表达式
来源：http://ns.shxzskj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xs.panjiajie.cn

[T06] Kotlin：集合映射
来源：http://gc.haigaiapp.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xo.shxzskj.cn

[T07] Kotlin：集合过滤
来源：http://og.521024.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lh.haigaiapp.cn

[T08] Kotlin：数据类
来源：http://th.shtwfgs.cn

data class User(val name: String, val age: Int)
来源：http://fr.nszjky.cn

[T09] Kotlin：扩展函数
来源：http://am.jctech888.com.cn

fun String.exclaim() = this + "!"
来源：http://nw.szxytkj.cn

[T10] Kotlin：默认参数
来源：http://uh.9csxet.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://iv.hnjuh.cn

[T11] Kotlin：协程
来源：http://jr.shtwfgs.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://sm.yuexingan06.cn

[T12] Kotlin：解构声明
来源：http://qe.huanxung.cn

val (a, b) = Pair(1, 2)
来源：http://do.shtwfgs.cn

[T13] Kotlin：只读 Map
来源：http://lv.lnxyls.cn

val m = mapOf("a" to 1)
来源：http://bt.haigaiapp.cn

[T14] Kotlin：循环
来源：http://ch.shtwfgs.cn

for (i in 1..10) println(i)
来源：http://kg.chemitech.net.cn

[T15] Kotlin：接口
来源：http://bf.newstarts.cn

interface Shape { fun area(): Double }
来源：http://vo.huixiangedu.cn

[T16] Swift：Hello World
来源：http://mo.9csxet.cn

print("Hello")
来源：http://se.9csxet.cn

[T17] Swift：变量与常量
来源：http://om.shxzskj.cn

var a = 1;  let b = 2
来源：http://bj.colortex.cn

[T18] Swift：字符串插值
来源：http://kh.521024.cn

"值: \(b)"
来源：http://uv.szxytkj.cn

[T19] Swift：可选绑定
来源：http://wo.panjiajie.cn

if let n = opt { print(n) }
来源：http://ve.yuexingan06.cn

[T20] Swift：数组操作
来源：http://zk.bjjhwx.cn

var a = [1, 2, 3];  a.append(4)
来源：http://di.colortex.cn

[T21] Swift：遍历
来源：http://ti.panjiajie.cn

for x in a { print(x) }
来源：http://nv.chemitech.net.cn

[T22] Swift：字典
来源：http://kv.lnxyls.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zh.szxytkj.cn

[T23] Swift：函数
来源：http://bq.szsharing.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fn.szxytkj.cn

[T24] Swift：闭包
来源：http://gj.newstarts.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://oe.shtwfgs.cn

[T25] Swift：结构体
来源：http://ey.wgjwhj.cn

struct P { var x: Int }
来源：http://kk.shxzskj.cn

[T26] Swift：类与重写
来源：http://vn.jianghongdianzi.cn

class A: Base { override func f() {} }
来源：http://xj.521024.cn

[T27] Swift：错误处理
来源：http://zw.yuntaijiaju.cn

do { try f() } catch { print(error) }
来源：http://ne.hahajie.cn

[T28] Swift：枚举
来源：http://qz.hnjuh.cn

enum Color { case red, green }
来源：http://pn.colortex.cn

[T29] Swift：guard 提前返回
来源：http://ge.szsharing.cn

guard let x = opt else { return }
来源：http://me.nicolike.cn

[T30] Swift：协议
来源：http://fx.colortex.cn

protocol Shape { func area() -> Double }
来源：http://ei.panjiajie.cn

[T31] Lua：Hello World
来源：http://fz.muxihuayi.cn

print("Hello")
来源：http://ek.huanxung.cn

[T32] Lua：局部变量
来源：http://mv.nszjky.cn

local a = 1
来源：http://nn.newstarts.cn

[T33] Lua：表（数组）
来源：http://up.jianghongdianzi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://rq.haigaiapp.cn

[T34] Lua：遍历表
来源：http://ew.jianghongdianzi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://mb.shxzskj.cn

[T35] Lua：字典表
来源：http://kp.asd995.cn

local d = { a = 1 };  d.b = 2
来源：http://qb.shxzukj.cn

[T36] Lua：函数
来源：http://am.szxytkj.cn

function add(a, b) return a + b end
来源：http://pp.haigaiapp.cn

[T37] Lua：字符串拼接
来源：http://om.panjiajie.cn

"a" .. "b"
来源：http://sw.yuntaijiaju.cn

[T38] Lua：条件
来源：http://wf.hnjuh.cn

if x > 0 then print("正") end
来源：http://gm.chemitech.net.cn

[T39] Lua：模式匹配
来源：http://ex.hahajie.cn

string.find(s, "%d+")
来源：http://iu.huanxung.cn

[T40] Lua：元表
来源：http://kz.colortex.cn

setmetatable({}, { __index = base })
来源：http://et.huanxung.cn

[T41] Perl：Hello World
来源：http://ar.chemitech.net.cn

print "Hello\n";
来源：http://ze.bookmarksfly.cn

[T42] Perl：变量类型
来源：http://hs.521024.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ux.colortex.cn

[T43] Perl：字符串插值
来源：http://db.shtwfgs.cn

"值: $a"
来源：http://fo.lnxyls.cn

[T44] Perl：条件
来源：http://ml.yuntaijiaju.cn

if ($a > 0) { print "正"; }
来源：http://ox.hahajie.cn

[T45] Perl：数组遍历
来源：http://ql.szxytkj.cn

for my $x (@arr) { print $x; }
来源：http://mh.szxytkj.cn

[T46] Perl：哈希操作
来源：http://tm.wgjwhj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sd.hnjuh.cn

[T47] Perl：正则捕获
来源：http://li.shtwfgs.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://fk.szxytkj.cn

[T48] Perl：正则替换
来源：http://wt.panjiajie.cn

$s =~ s/old/new/g;
来源：http://ci.huanxung.cn

[T49] Perl：函数
来源：http://fj.nszjky.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://df.asd995.cn

[T50] Perl：逐行读文件
来源：http://ie.huanxung.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://hi.huixiangedu.cn

while (my $line = <$fh>) { print $line; }
来源：http://cs.huixinmuqiang.cn

[T51] Scala：Hello World
来源：http://hq.huanxung.cn

println("Hello")
来源：http://nl.521024.cn

[T52] Scala：变量
来源：http://rs.9csxet.cn

val a = 1;  var b = 2
来源：http://qk.shxzskj.cn

[T53] Scala：字符串插值
来源：http://tl.nszjky.cn

s"值: $b"
来源：http://gl.panjiajie.cn

[T54] Scala：集合映射
来源：http://jc.9csxet.cn

List(1, 2, 3).map(_ * 2)
来源：http://yb.nicolike.cn

[T55] Scala：集合过滤
来源：http://up.huixinmuqiang.cn

List(1, 2, 3).filter(_ > 1)
来源：http://sl.asd995.cn

[T56] Scala：样例类
来源：http://yd.bjjhwx.cn

case class User(name: String, age: Int)
来源：http://am.9csxet.cn

[T57] Scala：模式匹配
来源：http://pg.colortex.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://px.shxzukj.cn

[T58] Scala：函数定义
来源：http://xi.newstarts.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ul.shtwfgs.cn

[T59] Scala：循环
来源：http://nn.huixiangedu.cn

for (i <- 1 to 10) println(i)
来源：http://bv.szxytkj.cn

[T60] Scala：折叠
来源：http://kn.hnjuh.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ot.lnxyls.cn

================================================================================
来源：http://oh.jianghongdianzi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wo.hnjuh.cn

================================================================================
来源：http://gk.huixiangedu.cn

[U01] Py：创建虚拟环境
来源：http://ag.521024.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ba.hahajie.cn

[U02] Py：导出 / 安装依赖
来源：http://qj.wgjwhj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ke.asd995.cn

[U03] Py：加载 .env 配置
来源：http://cs.hahajie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://bh.bjjhwx.cn

[U04] Py：变量调试打印
来源：http://zp.bookmarksfly.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dm.huixiangedu.cn

[U05] Py：列表去重且保序
来源：http://sz.newstarts.cn

list(dict.fromkeys(arr))
来源：http://pl.yuexingan06.cn

[U06] Py：合并两个字典
来源：http://gq.521024.cn

{**a, **b}
来源：http://cj.panjiajie.cn

[U07] Py：反转字典键值
来源：http://ew.bookmarksfly.cn

{v: k for k, v in d.items()}
来源：http://wh.nicolike.cn

[U08] Py：展平二维列表
来源：http://sj.huanxung.cn

[y for x in nested for y in x]
来源：http://is.hahajie.cn

[U09] Py：字典取最大值的键
来源：http://qi.lnxyls.cn

max(d, key=d.get)
来源：http://pq.newstarts.cn

[U10] Py：按值排序字典
来源：http://sf.lnxyls.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mu.wgjwhj.cn

[U11] Py：生成器表达式
来源：http://tl.hahajie.cn

(x * 2 for x in arr)
来源：http://se.gzmigu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xi.chemitech.net.cn

Counter(arr).most_common(3)
来源：http://gt.yuntaijiaju.cn

[U13] Py：固定长度队列
来源：http://na.yuntaijiaju.cn

deque(maxlen=10)
来源：http://hf.panjiajie.cn

[U14] Py：分组收集到列表
来源：http://zj.chemitech.net.cn

defaultdict(list)
来源：http://rl.bookmarksfly.cn

[U15] Py：高精度计时
来源：http://jz.521024.cn

t = time.perf_counter()
来源：http://ab.jctech888.com.cn

[U16] Py：命令行参数解析
来源：http://uc.521024.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mb.haigaiapp.cn

[U17] Py：初始化日志
来源：http://lc.asd995.cn

logging.basicConfig(level=logging.INFO)
来源：http://uy.huixiangedu.cn

[U18] Py：预编译正则
来源：http://eg.huanxung.cn

pat = re.compile(r"\d+")
来源：http://ck.lnxyls.cn

[U19] Py：正则替换带回调
来源：http://uk.nicolike.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sp.huixiangedu.cn

[U20] Py：缓存函数结果
来源：http://cm.lnxyls.cn

@functools.lru_cache(maxsize=None)
来源：http://ag.bjjhwx.cn

[U21] Py：自定义上下文管理器
来源：http://ok.panjiajie.cn

@contextlib.contextmanager
来源：http://ey.haigaiapp.cn

[U22] Py：矩阵转置
来源：http://kv.shxzskj.cn

list(zip(*m))
来源：http://ld.nicolike.cn

[U23] Py：分块读取大文件
来源：http://ii.huixiangedu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sq.haigaiapp.cn

[U24] Py：路径操作
来源：http://mv.szxytkj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://aw.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://dd.bookmarksfly.cn

csv.DictReader(f)
来源：http://ba.hnjuh.cn

[U26] Py：并发下载
来源：http://od.nszjky.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://uw.szsharing.cn

[U27] Py：异步 HTTP
来源：http://pg.lnxyls.cn

aiohttp.ClientSession() 配合 async with
来源：http://nf.shxzskj.cn

[U28] Py：类型别名
来源：http://ok.shxzskj.cn

UserId = int
来源：http://ik.jctech888.com.cn

[U29] Py：属性校验
来源：http://vy.521024.cn

@property 与 @x.setter 配合
来源：http://sr.wgjwhj.cn

[U30] Py：数据类
来源：http://sj.hnjuh.cn

@dataclass(slots=True)
来源：http://in.521024.cn

[U31] Py：单测
来源：http://dm.521024.cn

python -m pytest -q
来源：http://en.huixiangedu.cn

[U32] Py：代码格式化
来源：http://cx.wgjwhj.cn

ruff format . && ruff check --fix .
来源：http://rw.shxzskj.cn

[U33] Py：打包发布
来源：http://ao.asd995.cn

python -m build  （依赖 pyproject.toml）
来源：http://zm.wgjwhj.cn

[U34] Py：判断编码
来源：http://uu.newstarts.cn

chardet.detect(raw)
来源：http://ys.colortex.cn

[U35] Py：发送邮件
来源：http://qb.wgjwhj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cv.521024.cn

[U36] Py：定时任务
来源：http://er.shxzskj.cn

schedule.every(10).minutes.do(job)
来源：http://jv.huixinmuqiang.cn

[U37] Py：读写 Excel
来源：http://yq.muxihuayi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wf.yuexingan06.cn

[U38] Py：获取脚本所在目录
来源：http://cc.shxzukj.cn

Path(__file__).resolve().parent
来源：http://ym.shxzskj.cn

[U39] Py：判断是否在交互环境
来源：http://oy.huixinmuqiang.cn

sys.stdout.isatty()
来源：http://es.wgjwhj.cn

[U40] Py：打印到标准错误
来源：http://hw.huanxung.cn

print("err", file=sys.stderr)
来源：http://cw.gzmigu.cn

[U41] PHP：初始化 Composer 项目
来源：http://mh.muxihuayi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://dr.bookmarksfly.cn

[U42] PHP：PSR-4 自动加载
来源：http://jn.bjjhwx.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hw.lnxyls.cn

[U43] PHP：声明命名空间
来源：http://tt.newstarts.cn

namespace App\Http;
来源：http://cs.hahajie.cn

[U44] PHP：开启严格类型
来源：http://rl.chemitech.net.cn

declare(strict_types=1);
来源：http://ac.hahajie.cn

[U45] PHP：类型声明与返回类型
来源：http://kn.shtwfgs.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://gn.9csxet.cn

[U46] PHP：可空类型
来源：http://bn.szsharing.cn

?string $name = null
来源：http://ct.szsharing.cn

[U47] PHP：联合类型
来源：http://lz.shtwfgs.cn

int|string $id
来源：http://oj.yuexingan06.cn

[U48] PHP：纯枚举
来源：http://ki.hnjuh.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kx.chemitech.net.cn

[U49] PHP：只读属性
来源：http://xf.jianghongdianzi.cn

public readonly string $name
来源：http://ga.wgjwhj.cn

[U50] PHP：构造器属性提升
来源：http://yi.9csxet.cn

public function __construct(private int $id) {}
来源：http://do.shxzukj.cn

[U51] PHP：数组解构
来源：http://fl.yuexingan06.cn

[$a, $b] = $arr;
来源：http://cv.panjiajie.cn

[U52] PHP：箭头函数
来源：http://ty.chemitech.net.cn

$double = fn($x) => $x * 2;
来源：http://ce.haigaiapp.cn

[U53] PHP：空合并运算符
来源：http://mw.huixiangedu.cn

$v = $a ?? $b ?? "default";
来源：http://im.nszjky.cn

[U54] PHP：空安全调用
来源：http://xe.yuntaijiaju.cn

$obj?->method()
来源：http://uv.521024.cn

[U55] PHP：match 表达式
来源：http://jw.muxihuayi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ki.colortex.cn

[U56] PHP：命名参数
来源：http://ue.521024.cn

f(a: 1, b: 2)
来源：http://gp.yuexingan06.cn

[U57] PHP：字符串插值
来源：http://pl.bjjhwx.cn

"值: {$a}"
来源：http://ku.9csxet.cn

[U58] PHP：数组三件套
来源：http://gs.huanxung.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ss.huanxung.cn

[U59] PHP：自定义排序
来源：http://or.haigaiapp.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jm.colortex.cn

[U60] PHP：JSON 编解码
来源：http://rs.haigaiapp.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gm.521024.cn

[U61] PHP：正则
来源：http://at.szsharing.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hi.shxzukj.cn

[U62] PHP：日期对象
来源：http://dy.gzmigu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ua.colortex.cn

[U63] PHP：文件读写
来源：http://br.newstarts.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fb.yuntaijiaju.cn

[U64] PHP：目录遍历
来源：http://ri.szxytkj.cn

glob("dir/*.php");  scandir("dir");
来源：http://gc.wgjwhj.cn

[U65] PHP：会话
来源：http://ev.shtwfgs.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://la.hnjuh.cn

[U66] PHP：设置 Cookie
来源：http://zk.huixiangedu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ck.hahajie.cn

[U67] PHP：处理文件上传
来源：http://fz.521024.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xk.gzmigu.cn

[U68] PHP：PDO 连接
来源：http://ic.chemitech.net.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://je.asd995.cn

[U69] PHP：PDO 预处理
来源：http://mk.hahajie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://de.huanxung.cn

[U70] PHP：PDO 事务
来源：http://ic.asd995.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://es.yuntaijiaju.cn

[U71] PHP：抛出异常
来源：http://xq.haigaiapp.cn

throw new RuntimeException("失败", 500);
来源：http://lz.bookmarksfly.cn

[U72] PHP：写错误日志
来源：http://wv.huixiangedu.cn

error_log("失败: " . $e->getMessage());
来源：http://gg.haigaiapp.cn

[U73] PHP：读取 ini 配置
来源：http://it.shxzukj.cn

parse_ini_file("config.ini", true)
来源：http://kc.bookmarksfly.cn

[U74] PHP：读取环境变量
来源：http://qt.huanxung.cn

getenv("APP_ENV") ?: "production"
来源：http://xq.shxzskj.cn

[U75] PHP：依赖注入
来源：http://ep.bookmarksfly.cn

composer require psr/container
来源：http://gs.yuntaijiaju.cn

[U76] PHP：简单路由
来源：http://ey.colortex.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gu.colortex.cn

[U77] PHP：模板渲染
来源：http://ik.jctech888.com.cn

composer require twig/twig
来源：http://sg.asd995.cn

[U78] PHP：单元测试
来源：http://xa.hahajie.cn

composer require --dev phpunit/phpunit
来源：http://qa.chemitech.net.cn


<!-- 参考信息 -->