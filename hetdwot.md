代发 wailian999

int size() const noexcept { return n_; }
来源：http://ut.wgjwhj.cn

[S53] C++：移动语义
来源：http://tq.gzmigu.cn

std::vector<int> w = std::move(v);
来源：http://gv.asd995.cn

[S54] C++：异常处理
来源：http://nx.muxihuayi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bh.wgjwhj.cn

[S55] C++：结构化绑定
来源：http://wb.szxytkj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://an.bjjhwx.cn

[S56] C++：optional
来源：http://yr.panjiajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lt.gzmigu.cn

[S57] C++：编译期常量
来源：http://mq.huixinmuqiang.cn

constexpr int N = 10;
来源：http://dc.panjiajie.cn

[S58] C++：命名空间
来源：http://zi.szsharing.cn

namespace ns { int f() { return 1; } }
来源：http://rf.yuntaijiaju.cn

[S59] C++：静态断言
来源：http://ek.wgjwhj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ev.newstarts.cn

[S60] C++：遍历并删除元素
来源：http://tj.521024.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tu.bjjhwx.cn

================================================================================
来源：http://ti.shxzskj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xx.yuexingan06.cn

================================================================================
来源：http://gz.521024.cn

[T01] Kotlin：Hello World
来源：http://ks.hahajie.cn

println("Hello")
来源：http://bm.9csxet.cn

[T02] Kotlin：变量
来源：http://xn.lnxyls.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://an.wgjwhj.cn

[T03] Kotlin：字符串模板
来源：http://tv.bookmarksfly.cn

"值: $b"
来源：http://mo.jianghongdianzi.cn

[T04] Kotlin：空安全
来源：http://se.nszjky.cn

val n: String? = null;  n?.length
来源：http://rj.panjiajie.cn

[T05] Kotlin：when 表达式
来源：http://ph.shxzukj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pi.shtwfgs.cn

[T06] Kotlin：集合映射
来源：http://yg.newstarts.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://eh.yuexingan06.cn

[T07] Kotlin：集合过滤
来源：http://ij.shxzukj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ib.hahajie.cn

[T08] Kotlin：数据类
来源：http://ag.panjiajie.cn

data class User(val name: String, val age: Int)
来源：http://jh.bjjhwx.cn

[T09] Kotlin：扩展函数
来源：http://ng.shxzskj.cn

fun String.exclaim() = this + "!"
来源：http://ah.asd995.cn

[T10] Kotlin：默认参数
来源：http://gf.shxzukj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://mq.huanxung.cn

[T11] Kotlin：协程
来源：http://wn.newstarts.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bx.asd995.cn

[T12] Kotlin：解构声明
来源：http://ws.shtwfgs.cn

val (a, b) = Pair(1, 2)
来源：http://hp.shtwfgs.cn

[T13] Kotlin：只读 Map
来源：http://sj.521024.cn

val m = mapOf("a" to 1)
来源：http://eh.shxzukj.cn

[T14] Kotlin：循环
来源：http://ah.chemitech.net.cn

for (i in 1..10) println(i)
来源：http://mf.gzmigu.cn

[T15] Kotlin：接口
来源：http://dz.hahajie.cn

interface Shape { fun area(): Double }
来源：http://hb.bjjhwx.cn

[T16] Swift：Hello World
来源：http://wd.haigaiapp.cn

print("Hello")
来源：http://ao.panjiajie.cn

[T17] Swift：变量与常量
来源：http://bw.shxzskj.cn

var a = 1;  let b = 2
来源：http://mb.jianghongdianzi.cn

[T18] Swift：字符串插值
来源：http://sa.huixinmuqiang.cn

"值: \(b)"
来源：http://ro.shxzukj.cn

[T19] Swift：可选绑定
来源：http://ar.wgjwhj.cn

if let n = opt { print(n) }
来源：http://gp.szxytkj.cn

[T20] Swift：数组操作
来源：http://ef.bookmarksfly.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ot.shxzukj.cn

[T21] Swift：遍历
来源：http://cl.shtwfgs.cn

for x in a { print(x) }
来源：http://vz.jianghongdianzi.cn

[T22] Swift：字典
来源：http://nr.hnjuh.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ka.szsharing.cn

[T23] Swift：函数
来源：http://qo.muxihuayi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zl.yuexingan06.cn

[T24] Swift：闭包
来源：http://cx.shtwfgs.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://dl.huanxung.cn

[T25] Swift：结构体
来源：http://pu.hnjuh.cn

struct P { var x: Int }
来源：http://yw.huixiangedu.cn

[T26] Swift：类与重写
来源：http://uo.chemitech.net.cn

class A: Base { override func f() {} }
来源：http://rz.shxzskj.cn

[T27] Swift：错误处理
来源：http://zq.jianghongdianzi.cn

do { try f() } catch { print(error) }
来源：http://mx.haigaiapp.cn

[T28] Swift：枚举
来源：http://tl.gzmigu.cn

enum Color { case red, green }
来源：http://ie.huixinmuqiang.cn

[T29] Swift：guard 提前返回
来源：http://lt.521024.cn

guard let x = opt else { return }
来源：http://oa.haigaiapp.cn

[T30] Swift：协议
来源：http://ww.gzmigu.cn

protocol Shape { func area() -> Double }
来源：http://yn.9csxet.cn

[T31] Lua：Hello World
来源：http://dg.panjiajie.cn

print("Hello")
来源：http://dk.hahajie.cn

[T32] Lua：局部变量
来源：http://ma.szsharing.cn

local a = 1
来源：http://ch.shxzukj.cn

[T33] Lua：表（数组）
来源：http://yv.colortex.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://jq.yuntaijiaju.cn

[T34] Lua：遍历表
来源：http://te.huixiangedu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://os.bjjhwx.cn

[T35] Lua：字典表
来源：http://im.asd995.cn

local d = { a = 1 };  d.b = 2
来源：http://hl.colortex.cn

[T36] Lua：函数
来源：http://hc.shxzukj.cn

function add(a, b) return a + b end
来源：http://qt.jianghongdianzi.cn

[T37] Lua：字符串拼接
来源：http://bo.chemitech.net.cn

"a" .. "b"
来源：http://vd.yuexingan06.cn

[T38] Lua：条件
来源：http://cs.colortex.cn

if x > 0 then print("正") end
来源：http://mn.colortex.cn

[T39] Lua：模式匹配
来源：http://fk.haigaiapp.cn

string.find(s, "%d+")
来源：http://om.yuexingan06.cn

[T40] Lua：元表
来源：http://mi.9csxet.cn

setmetatable({}, { __index = base })
来源：http://hc.wgjwhj.cn

[T41] Perl：Hello World
来源：http://ie.nszjky.cn

print "Hello\n";
来源：http://xt.bookmarksfly.cn

[T42] Perl：变量类型
来源：http://dr.huixiangedu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jv.huixinmuqiang.cn

[T43] Perl：字符串插值
来源：http://tt.chemitech.net.cn

"值: $a"
来源：http://zt.colortex.cn

[T44] Perl：条件
来源：http://wl.panjiajie.cn

if ($a > 0) { print "正"; }
来源：http://pp.huixinmuqiang.cn

[T45] Perl：数组遍历
来源：http://nz.wgjwhj.cn

for my $x (@arr) { print $x; }
来源：http://am.shtwfgs.cn

[T46] Perl：哈希操作
来源：http://eq.szsharing.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xb.gzmigu.cn

[T47] Perl：正则捕获
来源：http://de.hnjuh.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://fi.bookmarksfly.cn

[T48] Perl：正则替换
来源：http://ig.huixiangedu.cn

$s =~ s/old/new/g;
来源：http://mv.yuexingan06.cn

[T49] Perl：函数
来源：http://zz.wgjwhj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vv.nicolike.cn

[T50] Perl：逐行读文件
来源：http://pe.szxytkj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://hl.yuntaijiaju.cn

while (my $line = <$fh>) { print $line; }
来源：http://ri.bookmarksfly.cn

[T51] Scala：Hello World
来源：http://kk.newstarts.cn

println("Hello")
来源：http://em.newstarts.cn

[T52] Scala：变量
来源：http://vo.shtwfgs.cn

val a = 1;  var b = 2
来源：http://jk.muxihuayi.cn

[T53] Scala：字符串插值
来源：http://bc.szxytkj.cn

s"值: $b"
来源：http://xo.9csxet.cn

[T54] Scala：集合映射
来源：http://sw.szsharing.cn

List(1, 2, 3).map(_ * 2)
来源：http://ux.chemitech.net.cn

[T55] Scala：集合过滤
来源：http://gj.panjiajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://hy.bjjhwx.cn

[T56] Scala：样例类
来源：http://xo.jctech888.com.cn

case class User(name: String, age: Int)
来源：http://ed.9csxet.cn

[T57] Scala：模式匹配
来源：http://rq.newstarts.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ru.shxzskj.cn

[T58] Scala：函数定义
来源：http://ur.nicolike.cn

def add(a: Int, b: Int): Int = a + b
来源：http://xc.szsharing.cn

[T59] Scala：循环
来源：http://to.521024.cn

for (i <- 1 to 10) println(i)
来源：http://mn.hahajie.cn

[T60] Scala：折叠
来源：http://ib.wgjwhj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wg.asd995.cn

================================================================================
来源：http://lh.bookmarksfly.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bv.yuexingan06.cn

================================================================================
来源：http://tq.huanxung.cn

[U01] Py：创建虚拟环境
来源：http://tj.9csxet.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mc.bjjhwx.cn

[U02] Py：导出 / 安装依赖
来源：http://te.jctech888.com.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lc.chemitech.net.cn

[U03] Py：加载 .env 配置
来源：http://ni.colortex.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://uf.huixiangedu.cn

[U04] Py：变量调试打印
来源：http://bi.jctech888.com.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jp.muxihuayi.cn

[U05] Py：列表去重且保序
来源：http://gg.jctech888.com.cn

list(dict.fromkeys(arr))
来源：http://yo.wgjwhj.cn

[U06] Py：合并两个字典
来源：http://cs.bjjhwx.cn

{**a, **b}
来源：http://ye.shtwfgs.cn

[U07] Py：反转字典键值
来源：http://qr.lnxyls.cn

{v: k for k, v in d.items()}
来源：http://vy.nicolike.cn

[U08] Py：展平二维列表
来源：http://pa.shxzukj.cn

[y for x in nested for y in x]
来源：http://ew.gzmigu.cn

[U09] Py：字典取最大值的键
来源：http://cp.shtwfgs.cn

max(d, key=d.get)
来源：http://ak.colortex.cn

[U10] Py：按值排序字典
来源：http://qq.chemitech.net.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://do.jianghongdianzi.cn

[U11] Py：生成器表达式
来源：http://cz.huixinmuqiang.cn

(x * 2 for x in arr)
来源：http://hj.muxihuayi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lg.jianghongdianzi.cn

Counter(arr).most_common(3)
来源：http://vi.panjiajie.cn

[U13] Py：固定长度队列
来源：http://vg.nszjky.cn

deque(maxlen=10)
来源：http://tb.szsharing.cn

[U14] Py：分组收集到列表
来源：http://tt.szsharing.cn

defaultdict(list)
来源：http://hs.jianghongdianzi.cn

[U15] Py：高精度计时
来源：http://ky.asd995.cn

t = time.perf_counter()
来源：http://rv.jctech888.com.cn

[U16] Py：命令行参数解析
来源：http://wo.hnjuh.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xc.colortex.cn

[U17] Py：初始化日志
来源：http://xg.hnjuh.cn

logging.basicConfig(level=logging.INFO)
来源：http://do.lnxyls.cn

[U18] Py：预编译正则
来源：http://zq.bookmarksfly.cn

pat = re.compile(r"\d+")
来源：http://iy.jctech888.com.cn

[U19] Py：正则替换带回调
来源：http://zy.jctech888.com.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://al.huixinmuqiang.cn

[U20] Py：缓存函数结果
来源：http://qt.jctech888.com.cn

@functools.lru_cache(maxsize=None)
来源：http://em.hahajie.cn

[U21] Py：自定义上下文管理器
来源：http://tn.haigaiapp.cn

@contextlib.contextmanager
来源：http://fi.huixinmuqiang.cn

[U22] Py：矩阵转置
来源：http://ad.asd995.cn

list(zip(*m))
来源：http://ls.bjjhwx.cn

[U23] Py：分块读取大文件
来源：http://pu.shxzukj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fz.hnjuh.cn

[U24] Py：路径操作
来源：http://ic.nszjky.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ju.colortex.cn

[U25] Py：CSV 按字典读
来源：http://nz.lnxyls.cn

csv.DictReader(f)
来源：http://dm.panjiajie.cn

[U26] Py：并发下载
来源：http://hf.shxzskj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ow.szxytkj.cn

[U27] Py：异步 HTTP
来源：http://tr.yuntaijiaju.cn

aiohttp.ClientSession() 配合 async with
来源：http://eb.yuntaijiaju.cn

[U28] Py：类型别名
来源：http://ya.shxzskj.cn

UserId = int
来源：http://ys.521024.cn

[U29] Py：属性校验
来源：http://mw.huixiangedu.cn

@property 与 @x.setter 配合
来源：http://ss.hahajie.cn

[U30] Py：数据类
来源：http://jv.haigaiapp.cn

@dataclass(slots=True)
来源：http://xr.shxzskj.cn

[U31] Py：单测
来源：http://xp.jianghongdianzi.cn

python -m pytest -q
来源：http://ue.gzmigu.cn

[U32] Py：代码格式化
来源：http://ki.jianghongdianzi.cn

ruff format . && ruff check --fix .
来源：http://jx.521024.cn

[U33] Py：打包发布
来源：http://zv.9csxet.cn

python -m build  （依赖 pyproject.toml）
来源：http://fm.newstarts.cn

[U34] Py：判断编码
来源：http://mo.huanxung.cn

chardet.detect(raw)
来源：http://kn.shtwfgs.cn

[U35] Py：发送邮件
来源：http://iy.shxzskj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://uc.huixinmuqiang.cn

[U36] Py：定时任务
来源：http://kh.asd995.cn

schedule.every(10).minutes.do(job)
来源：http://kp.bookmarksfly.cn

[U37] Py：读写 Excel
来源：http://vo.yuexingan06.cn

pandas.read_excel / DataFrame.to_excel
来源：http://bs.jianghongdianzi.cn

[U38] Py：获取脚本所在目录
来源：http://ml.shxzukj.cn

Path(__file__).resolve().parent
来源：http://na.szsharing.cn

[U39] Py：判断是否在交互环境
来源：http://vt.bookmarksfly.cn

sys.stdout.isatty()
来源：http://oh.jctech888.com.cn

[U40] Py：打印到标准错误
来源：http://ow.huixinmuqiang.cn

print("err", file=sys.stderr)
来源：http://sx.shxzukj.cn

[U41] PHP：初始化 Composer 项目
来源：http://fa.hnjuh.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zk.muxihuayi.cn

[U42] PHP：PSR-4 自动加载
来源：http://cr.hahajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gd.shtwfgs.cn

[U43] PHP：声明命名空间
来源：http://re.szxytkj.cn

namespace App\Http;
来源：http://mi.haigaiapp.cn

[U44] PHP：开启严格类型
来源：http://ke.muxihuayi.cn

declare(strict_types=1);
来源：http://hx.huixinmuqiang.cn

[U45] PHP：类型声明与返回类型
来源：http://om.huixiangedu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://gg.nszjky.cn

[U46] PHP：可空类型
来源：http://ig.jctech888.com.cn

?string $name = null
来源：http://th.yuntaijiaju.cn

[U47] PHP：联合类型
来源：http://pa.huixinmuqiang.cn

int|string $id
来源：http://gb.huixiangedu.cn

[U48] PHP：纯枚举
来源：http://uf.szsharing.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xo.muxihuayi.cn

[U49] PHP：只读属性
来源：http://wj.colortex.cn

public readonly string $name
来源：http://xw.shxzskj.cn

[U50] PHP：构造器属性提升
来源：http://eh.shtwfgs.cn

public function __construct(private int $id) {}
来源：http://es.wgjwhj.cn

[U51] PHP：数组解构
来源：http://wa.lnxyls.cn

[$a, $b] = $arr;
来源：http://va.szsharing.cn

[U52] PHP：箭头函数
来源：http://ov.chemitech.net.cn

$double = fn($x) => $x * 2;
来源：http://xd.jctech888.com.cn

[U53] PHP：空合并运算符
来源：http://ng.chemitech.net.cn

$v = $a ?? $b ?? "default";
来源：http://xm.chemitech.net.cn

[U54] PHP：空安全调用
来源：http://id.hahajie.cn

$obj?->method()
来源：http://ce.wgjwhj.cn

[U55] PHP：match 表达式
来源：http://lm.gzmigu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://al.haigaiapp.cn

[U56] PHP：命名参数
来源：http://ev.yuntaijiaju.cn

f(a: 1, b: 2)
来源：http://bh.nszjky.cn

[U57] PHP：字符串插值
来源：http://hu.jctech888.com.cn

"值: {$a}"
来源：http://dq.szxytkj.cn

[U58] PHP：数组三件套
来源：http://cf.bookmarksfly.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ia.jianghongdianzi.cn

[U59] PHP：自定义排序
来源：http://cc.yuexingan06.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hy.hnjuh.cn

[U60] PHP：JSON 编解码
来源：http://nt.yuntaijiaju.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gr.lnxyls.cn

[U61] PHP：正则
来源：http://by.haigaiapp.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dp.shtwfgs.cn

[U62] PHP：日期对象
来源：http://ro.lnxyls.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://me.shtwfgs.cn

[U63] PHP：文件读写
来源：http://iw.jctech888.com.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yu.szxytkj.cn

[U64] PHP：目录遍历
来源：http://cs.huixinmuqiang.cn

glob("dir/*.php");  scandir("dir");
来源：http://dw.huanxung.cn

[U65] PHP：会话
来源：http://nq.lnxyls.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://db.nicolike.cn

[U66] PHP：设置 Cookie
来源：http://qu.szxytkj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yd.nszjky.cn

[U67] PHP：处理文件上传
来源：http://ph.haigaiapp.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wl.shtwfgs.cn

[U68] PHP：PDO 连接
来源：http://aw.szxytkj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kk.szxytkj.cn

[U69] PHP：PDO 预处理
来源：http://go.colortex.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gk.521024.cn

[U70] PHP：PDO 事务
来源：http://ci.hahajie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gf.nszjky.cn

[U71] PHP：抛出异常
来源：http://vg.gzmigu.cn

throw new RuntimeException("失败", 500);
来源：http://vl.huixinmuqiang.cn

[U72] PHP：写错误日志
来源：http://tf.shxzukj.cn

error_log("失败: " . $e->getMessage());
来源：http://ni.yuexingan06.cn

[U73] PHP：读取 ini 配置
来源：http://dx.9csxet.cn

parse_ini_file("config.ini", true)
来源：http://jk.hnjuh.cn

[U74] PHP：读取环境变量
来源：http://ux.huixiangedu.cn

getenv("APP_ENV") ?: "production"
来源：http://xw.szxytkj.cn

[U75] PHP：依赖注入
来源：http://ev.asd995.cn

composer require psr/container
来源：http://jl.huixiangedu.cn

[U76] PHP：简单路由
来源：http://go.shxzukj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fk.chemitech.net.cn

[U77] PHP：模板渲染
来源：http://mf.haigaiapp.cn

composer require twig/twig
来源：http://um.nicolike.cn

[U78] PHP：单元测试
来源：http://gy.9csxet.cn

composer require --dev phpunit/phpunit
来源：http://et.521024.cn


<!-- 参考信息 -->