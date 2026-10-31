代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://da.nicolike.cn

[S55] C++：结构化绑定
来源：http://en.jctech888.com.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://un.newstarts.cn

[S56] C++：optional
来源：http://at.szsharing.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://et.bookmarksfly.cn

[S57] C++：编译期常量
来源：http://th.shxzskj.cn

constexpr int N = 10;
来源：http://hw.chemitech.net.cn

[S58] C++：命名空间
来源：http://sn.huixiangedu.cn

namespace ns { int f() { return 1; } }
来源：http://mm.bjjhwx.cn

[S59] C++：静态断言
来源：http://va.jianghongdianzi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qn.wgjwhj.cn

[S60] C++：遍历并删除元素
来源：http://jd.jctech888.com.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://io.szxytkj.cn

================================================================================
来源：http://vf.nszjky.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gf.wgjwhj.cn

================================================================================
来源：http://ho.shxzukj.cn

[T01] Kotlin：Hello World
来源：http://lc.gzmigu.cn

println("Hello")
来源：http://mg.yuexingan06.cn

[T02] Kotlin：变量
来源：http://lk.shxzukj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pc.szxytkj.cn

[T03] Kotlin：字符串模板
来源：http://zc.shtwfgs.cn

"值: $b"
来源：http://pg.muxihuayi.cn

[T04] Kotlin：空安全
来源：http://dg.szxytkj.cn

val n: String? = null;  n?.length
来源：http://og.shxzskj.cn

[T05] Kotlin：when 表达式
来源：http://yf.huanxung.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ii.huanxung.cn

[T06] Kotlin：集合映射
来源：http://ee.muxihuayi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rj.lnxyls.cn

[T07] Kotlin：集合过滤
来源：http://uh.nicolike.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ez.chemitech.net.cn

[T08] Kotlin：数据类
来源：http://uj.haigaiapp.cn

data class User(val name: String, val age: Int)
来源：http://oq.nicolike.cn

[T09] Kotlin：扩展函数
来源：http://zi.jctech888.com.cn

fun String.exclaim() = this + "!"
来源：http://gw.yuntaijiaju.cn

[T10] Kotlin：默认参数
来源：http://jh.jctech888.com.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://bv.lnxyls.cn

[T11] Kotlin：协程
来源：http://va.hnjuh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ns.9csxet.cn

[T12] Kotlin：解构声明
来源：http://xd.jianghongdianzi.cn

val (a, b) = Pair(1, 2)
来源：http://en.lnxyls.cn

[T13] Kotlin：只读 Map
来源：http://ju.chemitech.net.cn

val m = mapOf("a" to 1)
来源：http://nm.huixiangedu.cn

[T14] Kotlin：循环
来源：http://ol.hnjuh.cn

for (i in 1..10) println(i)
来源：http://ne.szxytkj.cn

[T15] Kotlin：接口
来源：http://be.wgjwhj.cn

interface Shape { fun area(): Double }
来源：http://wr.bjjhwx.cn

[T16] Swift：Hello World
来源：http://wt.huanxung.cn

print("Hello")
来源：http://gd.yuexingan06.cn

[T17] Swift：变量与常量
来源：http://zx.huanxung.cn

var a = 1;  let b = 2
来源：http://dd.chemitech.net.cn

[T18] Swift：字符串插值
来源：http://gj.panjiajie.cn

"值: \(b)"
来源：http://il.shtwfgs.cn

[T19] Swift：可选绑定
来源：http://mg.nszjky.cn

if let n = opt { print(n) }
来源：http://go.muxihuayi.cn

[T20] Swift：数组操作
来源：http://wy.chemitech.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://dz.hnjuh.cn

[T21] Swift：遍历
来源：http://te.jianghongdianzi.cn

for x in a { print(x) }
来源：http://uw.muxihuayi.cn

[T22] Swift：字典
来源：http://ho.nicolike.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zz.colortex.cn

[T23] Swift：函数
来源：http://du.hahajie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mq.yuntaijiaju.cn

[T24] Swift：闭包
来源：http://tb.shxzskj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://uw.huixinmuqiang.cn

[T25] Swift：结构体
来源：http://ib.chemitech.net.cn

struct P { var x: Int }
来源：http://xa.yuexingan06.cn

[T26] Swift：类与重写
来源：http://xr.newstarts.cn

class A: Base { override func f() {} }
来源：http://ga.yuexingan06.cn

[T27] Swift：错误处理
来源：http://wn.jianghongdianzi.cn

do { try f() } catch { print(error) }
来源：http://lm.yuexingan06.cn

[T28] Swift：枚举
来源：http://bx.gzmigu.cn

enum Color { case red, green }
来源：http://am.bookmarksfly.cn

[T29] Swift：guard 提前返回
来源：http://ri.shtwfgs.cn

guard let x = opt else { return }
来源：http://jp.huixinmuqiang.cn

[T30] Swift：协议
来源：http://yw.nszjky.cn

protocol Shape { func area() -> Double }
来源：http://ld.shxzukj.cn

[T31] Lua：Hello World
来源：http://ga.bjjhwx.cn

print("Hello")
来源：http://yx.nszjky.cn

[T32] Lua：局部变量
来源：http://uc.szsharing.cn

local a = 1
来源：http://pp.shxzskj.cn

[T33] Lua：表（数组）
来源：http://nz.jianghongdianzi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ec.521024.cn

[T34] Lua：遍历表
来源：http://jc.bjjhwx.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://pe.asd995.cn

[T35] Lua：字典表
来源：http://wf.haigaiapp.cn

local d = { a = 1 };  d.b = 2
来源：http://he.newstarts.cn

[T36] Lua：函数
来源：http://bf.jctech888.com.cn

function add(a, b) return a + b end
来源：http://ki.lnxyls.cn

[T37] Lua：字符串拼接
来源：http://zx.jctech888.com.cn

"a" .. "b"
来源：http://ay.haigaiapp.cn

[T38] Lua：条件
来源：http://rg.jctech888.com.cn

if x > 0 then print("正") end
来源：http://mx.9csxet.cn

[T39] Lua：模式匹配
来源：http://zv.muxihuayi.cn

string.find(s, "%d+")
来源：http://uz.haigaiapp.cn

[T40] Lua：元表
来源：http://ak.newstarts.cn

setmetatable({}, { __index = base })
来源：http://us.szsharing.cn

[T41] Perl：Hello World
来源：http://om.haigaiapp.cn

print "Hello\n";
来源：http://xd.lnxyls.cn

[T42] Perl：变量类型
来源：http://mt.bjjhwx.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tz.yuntaijiaju.cn

[T43] Perl：字符串插值
来源：http://cy.nszjky.cn

"值: $a"
来源：http://ls.bookmarksfly.cn

[T44] Perl：条件
来源：http://dl.jctech888.com.cn

if ($a > 0) { print "正"; }
来源：http://hw.jctech888.com.cn

[T45] Perl：数组遍历
来源：http://en.shxzukj.cn

for my $x (@arr) { print $x; }
来源：http://sn.nszjky.cn

[T46] Perl：哈希操作
来源：http://na.nicolike.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zo.bookmarksfly.cn

[T47] Perl：正则捕获
来源：http://bm.nicolike.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://kg.jianghongdianzi.cn

[T48] Perl：正则替换
来源：http://uo.panjiajie.cn

$s =~ s/old/new/g;
来源：http://pz.wgjwhj.cn

[T49] Perl：函数
来源：http://ab.bjjhwx.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ir.wgjwhj.cn

[T50] Perl：逐行读文件
来源：http://aq.9csxet.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wu.lnxyls.cn

while (my $line = <$fh>) { print $line; }
来源：http://hs.yuntaijiaju.cn

[T51] Scala：Hello World
来源：http://ak.yuexingan06.cn

println("Hello")
来源：http://tn.panjiajie.cn

[T52] Scala：变量
来源：http://gc.panjiajie.cn

val a = 1;  var b = 2
来源：http://sd.nicolike.cn

[T53] Scala：字符串插值
来源：http://gw.haigaiapp.cn

s"值: $b"
来源：http://qh.szsharing.cn

[T54] Scala：集合映射
来源：http://vo.haigaiapp.cn

List(1, 2, 3).map(_ * 2)
来源：http://mc.panjiajie.cn

[T55] Scala：集合过滤
来源：http://cm.yuntaijiaju.cn

List(1, 2, 3).filter(_ > 1)
来源：http://rq.shtwfgs.cn

[T56] Scala：样例类
来源：http://yf.521024.cn

case class User(name: String, age: Int)
来源：http://gd.asd995.cn

[T57] Scala：模式匹配
来源：http://xg.asd995.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://xf.jianghongdianzi.cn

[T58] Scala：函数定义
来源：http://ph.nicolike.cn

def add(a: Int, b: Int): Int = a + b
来源：http://kk.nicolike.cn

[T59] Scala：循环
来源：http://fp.szxytkj.cn

for (i <- 1 to 10) println(i)
来源：http://rv.huanxung.cn

[T60] Scala：折叠
来源：http://nk.lnxyls.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ko.lnxyls.cn

================================================================================
来源：http://xy.chemitech.net.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zg.szxytkj.cn

================================================================================
来源：http://np.chemitech.net.cn

[U01] Py：创建虚拟环境
来源：http://kr.hahajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://do.jianghongdianzi.cn

[U02] Py：导出 / 安装依赖
来源：http://ls.bjjhwx.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rk.521024.cn

[U03] Py：加载 .env 配置
来源：http://gx.haigaiapp.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ng.9csxet.cn

[U04] Py：变量调试打印
来源：http://vq.bookmarksfly.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xk.muxihuayi.cn

[U05] Py：列表去重且保序
来源：http://dg.yuexingan06.cn

list(dict.fromkeys(arr))
来源：http://pw.huixinmuqiang.cn

[U06] Py：合并两个字典
来源：http://cn.chemitech.net.cn

{**a, **b}
来源：http://gb.panjiajie.cn

[U07] Py：反转字典键值
来源：http://gr.shxzukj.cn

{v: k for k, v in d.items()}
来源：http://sr.jctech888.com.cn

[U08] Py：展平二维列表
来源：http://fd.haigaiapp.cn

[y for x in nested for y in x]
来源：http://vr.521024.cn

[U09] Py：字典取最大值的键
来源：http://lq.newstarts.cn

max(d, key=d.get)
来源：http://hp.chemitech.net.cn

[U10] Py：按值排序字典
来源：http://vo.yuntaijiaju.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://um.yuntaijiaju.cn

[U11] Py：生成器表达式
来源：http://py.haigaiapp.cn

(x * 2 for x in arr)
来源：http://uz.hnjuh.cn

[U12] Py：取出现最多的 3 个元素
来源：http://vm.huixiangedu.cn

Counter(arr).most_common(3)
来源：http://af.bjjhwx.cn

[U13] Py：固定长度队列
来源：http://hj.lnxyls.cn

deque(maxlen=10)
来源：http://og.huixiangedu.cn

[U14] Py：分组收集到列表
来源：http://ym.chemitech.net.cn

defaultdict(list)
来源：http://lo.wgjwhj.cn

[U15] Py：高精度计时
来源：http://ar.panjiajie.cn

t = time.perf_counter()
来源：http://su.huixiangedu.cn

[U16] Py：命令行参数解析
来源：http://xn.chemitech.net.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ya.jctech888.com.cn

[U17] Py：初始化日志
来源：http://qo.chemitech.net.cn

logging.basicConfig(level=logging.INFO)
来源：http://zo.chemitech.net.cn

[U18] Py：预编译正则
来源：http://yi.nszjky.cn

pat = re.compile(r"\d+")
来源：http://dy.yuntaijiaju.cn

[U19] Py：正则替换带回调
来源：http://bb.wgjwhj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://aw.shxzskj.cn

[U20] Py：缓存函数结果
来源：http://vj.panjiajie.cn

@functools.lru_cache(maxsize=None)
来源：http://im.bjjhwx.cn

[U21] Py：自定义上下文管理器
来源：http://kp.huixinmuqiang.cn

@contextlib.contextmanager
来源：http://lh.yuntaijiaju.cn

[U22] Py：矩阵转置
来源：http://en.muxihuayi.cn

list(zip(*m))
来源：http://ce.shxzukj.cn

[U23] Py：分块读取大文件
来源：http://ae.hnjuh.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://es.jianghongdianzi.cn

[U24] Py：路径操作
来源：http://lg.newstarts.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ed.bookmarksfly.cn

[U25] Py：CSV 按字典读
来源：http://rr.nicolike.cn

csv.DictReader(f)
来源：http://eg.asd995.cn

[U26] Py：并发下载
来源：http://sg.shxzukj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ir.szsharing.cn

[U27] Py：异步 HTTP
来源：http://ks.jianghongdianzi.cn

aiohttp.ClientSession() 配合 async with
来源：http://cf.shxzukj.cn

[U28] Py：类型别名
来源：http://ah.wgjwhj.cn

UserId = int
来源：http://yr.nszjky.cn

[U29] Py：属性校验
来源：http://zx.huixiangedu.cn

@property 与 @x.setter 配合
来源：http://em.yuntaijiaju.cn

[U30] Py：数据类
来源：http://zf.shxzukj.cn

@dataclass(slots=True)
来源：http://jf.nszjky.cn

[U31] Py：单测
来源：http://bj.nszjky.cn

python -m pytest -q
来源：http://yq.shxzskj.cn

[U32] Py：代码格式化
来源：http://re.muxihuayi.cn

ruff format . && ruff check --fix .
来源：http://rj.gzmigu.cn

[U33] Py：打包发布
来源：http://xh.huanxung.cn

python -m build  （依赖 pyproject.toml）
来源：http://ep.nszjky.cn

[U34] Py：判断编码
来源：http://pt.muxihuayi.cn

chardet.detect(raw)
来源：http://bh.huanxung.cn

[U35] Py：发送邮件
来源：http://ea.shxzskj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xr.colortex.cn

[U36] Py：定时任务
来源：http://of.shxzukj.cn

schedule.every(10).minutes.do(job)
来源：http://et.asd995.cn

[U37] Py：读写 Excel
来源：http://fd.szxytkj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://yb.szsharing.cn

[U38] Py：获取脚本所在目录
来源：http://qh.9csxet.cn

Path(__file__).resolve().parent
来源：http://ip.9csxet.cn

[U39] Py：判断是否在交互环境
来源：http://rd.panjiajie.cn

sys.stdout.isatty()
来源：http://hi.szsharing.cn

[U40] Py：打印到标准错误
来源：http://ky.wgjwhj.cn

print("err", file=sys.stderr)
来源：http://gn.shxzukj.cn

[U41] PHP：初始化 Composer 项目
来源：http://tu.bookmarksfly.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ib.shxzskj.cn

[U42] PHP：PSR-4 自动加载
来源：http://ts.colortex.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://aj.yuntaijiaju.cn

[U43] PHP：声明命名空间
来源：http://it.huixinmuqiang.cn

namespace App\Http;
来源：http://do.bjjhwx.cn

[U44] PHP：开启严格类型
来源：http://sh.szxytkj.cn

declare(strict_types=1);
来源：http://yg.huixinmuqiang.cn

[U45] PHP：类型声明与返回类型
来源：http://qx.gzmigu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://hm.newstarts.cn

[U46] PHP：可空类型
来源：http://zt.shtwfgs.cn

?string $name = null
来源：http://wm.huanxung.cn

[U47] PHP：联合类型
来源：http://tf.gzmigu.cn

int|string $id
来源：http://ky.shxzskj.cn

[U48] PHP：纯枚举
来源：http://jy.yuexingan06.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fb.chemitech.net.cn

[U49] PHP：只读属性
来源：http://gt.gzmigu.cn

public readonly string $name
来源：http://th.wgjwhj.cn

[U50] PHP：构造器属性提升
来源：http://ml.nicolike.cn

public function __construct(private int $id) {}
来源：http://ol.szsharing.cn

[U51] PHP：数组解构
来源：http://ho.yuexingan06.cn

[$a, $b] = $arr;
来源：http://in.shxzukj.cn

[U52] PHP：箭头函数
来源：http://na.jctech888.com.cn

$double = fn($x) => $x * 2;
来源：http://nq.bookmarksfly.cn

[U53] PHP：空合并运算符
来源：http://vy.9csxet.cn

$v = $a ?? $b ?? "default";
来源：http://mw.wgjwhj.cn

[U54] PHP：空安全调用
来源：http://jj.jianghongdianzi.cn

$obj?->method()
来源：http://gw.colortex.cn

[U55] PHP：match 表达式
来源：http://ti.yuexingan06.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qy.gzmigu.cn

[U56] PHP：命名参数
来源：http://vt.panjiajie.cn

f(a: 1, b: 2)
来源：http://jh.asd995.cn

[U57] PHP：字符串插值
来源：http://gy.panjiajie.cn

"值: {$a}"
来源：http://uh.shxzukj.cn

[U58] PHP：数组三件套
来源：http://ii.asd995.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zc.panjiajie.cn

[U59] PHP：自定义排序
来源：http://ir.shtwfgs.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://br.gzmigu.cn

[U60] PHP：JSON 编解码
来源：http://sh.huixiangedu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://do.9csxet.cn

[U61] PHP：正则
来源：http://ew.huixiangedu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mk.jianghongdianzi.cn

[U62] PHP：日期对象
来源：http://ps.yuexingan06.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://aj.huixiangedu.cn

[U63] PHP：文件读写
来源：http://bu.huixiangedu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qz.shxzukj.cn

[U64] PHP：目录遍历
来源：http://lp.haigaiapp.cn

glob("dir/*.php");  scandir("dir");
来源：http://ou.szxytkj.cn

[U65] PHP：会话
来源：http://ng.nicolike.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rg.gzmigu.cn

[U66] PHP：设置 Cookie
来源：http://ds.wgjwhj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dp.chemitech.net.cn

[U67] PHP：处理文件上传
来源：http://yy.yuntaijiaju.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yl.shxzskj.cn

[U68] PHP：PDO 连接
来源：http://zo.newstarts.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://iv.yuntaijiaju.cn

[U69] PHP：PDO 预处理
来源：http://oh.chemitech.net.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xs.gzmigu.cn

[U70] PHP：PDO 事务
来源：http://tn.szxytkj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ry.panjiajie.cn

[U71] PHP：抛出异常
来源：http://xp.521024.cn

throw new RuntimeException("失败", 500);
来源：http://bc.hnjuh.cn

[U72] PHP：写错误日志
来源：http://gi.hahajie.cn

error_log("失败: " . $e->getMessage());
来源：http://ps.shtwfgs.cn

[U73] PHP：读取 ini 配置
来源：http://ht.hnjuh.cn

parse_ini_file("config.ini", true)
来源：http://sf.shxzukj.cn

[U74] PHP：读取环境变量
来源：http://wx.hahajie.cn

getenv("APP_ENV") ?: "production"
来源：http://bn.jctech888.com.cn

[U75] PHP：依赖注入
来源：http://bp.huanxung.cn

composer require psr/container
来源：http://rv.lnxyls.cn

[U76] PHP：简单路由
来源：http://qo.hnjuh.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tw.haigaiapp.cn

[U77] PHP：模板渲染
来源：http://kt.colortex.cn

composer require twig/twig
来源：http://so.521024.cn

[U78] PHP：单元测试
来源：http://ko.huixiangedu.cn

composer require --dev phpunit/phpunit
来源：http://wd.panjiajie.cn

[U79] PHP：静态分析
来源：http://nm.nszjky.cn

composer require --dev phpstan/phpstan
来源：http://gc.shxzukj.cn

[U80] PHP：代码规范修复
来源：http://zs.wgjwhj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://yo.521024.cn


<!-- 参考信息 -->