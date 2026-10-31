代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ka.colortex.cn

[S55] C++：结构化绑定
来源：http://yd.521024.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rt.szxytkj.cn

[S56] C++：optional
来源：http://hf.colortex.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dd.521024.cn

[S57] C++：编译期常量
来源：http://zn.huanxung.cn

constexpr int N = 10;
来源：http://fz.haigaiapp.cn

[S58] C++：命名空间
来源：http://tt.hnjuh.cn

namespace ns { int f() { return 1; } }
来源：http://xo.yuntaijiaju.cn

[S59] C++：静态断言
来源：http://ss.lnxyls.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fh.lnxyls.cn

[S60] C++：遍历并删除元素
来源：http://be.asd995.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kk.chemitech.net.cn

================================================================================
来源：http://pi.lnxyls.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hi.bookmarksfly.cn

================================================================================
来源：http://ey.huixinmuqiang.cn

[T01] Kotlin：Hello World
来源：http://vz.9csxet.cn

println("Hello")
来源：http://vn.szsharing.cn

[T02] Kotlin：变量
来源：http://ik.muxihuayi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ts.9csxet.cn

[T03] Kotlin：字符串模板
来源：http://qi.yuntaijiaju.cn

"值: $b"
来源：http://ph.huixinmuqiang.cn

[T04] Kotlin：空安全
来源：http://re.shtwfgs.cn

val n: String? = null;  n?.length
来源：http://qu.szsharing.cn

[T05] Kotlin：when 表达式
来源：http://ha.asd995.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bl.9csxet.cn

[T06] Kotlin：集合映射
来源：http://jj.nszjky.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://qg.shxzskj.cn

[T07] Kotlin：集合过滤
来源：http://km.nszjky.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ae.muxihuayi.cn

[T08] Kotlin：数据类
来源：http://fh.huixinmuqiang.cn

data class User(val name: String, val age: Int)
来源：http://ut.shxzukj.cn

[T09] Kotlin：扩展函数
来源：http://md.lnxyls.cn

fun String.exclaim() = this + "!"
来源：http://zm.chemitech.net.cn

[T10] Kotlin：默认参数
来源：http://xa.szsharing.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://cm.bjjhwx.cn

[T11] Kotlin：协程
来源：http://xs.nicolike.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vf.haigaiapp.cn

[T12] Kotlin：解构声明
来源：http://dz.hahajie.cn

val (a, b) = Pair(1, 2)
来源：http://mc.yuexingan06.cn

[T13] Kotlin：只读 Map
来源：http://zw.szxytkj.cn

val m = mapOf("a" to 1)
来源：http://fq.muxihuayi.cn

[T14] Kotlin：循环
来源：http://rm.gzmigu.cn

for (i in 1..10) println(i)
来源：http://as.huanxung.cn

[T15] Kotlin：接口
来源：http://fk.szxytkj.cn

interface Shape { fun area(): Double }
来源：http://yb.chemitech.net.cn

[T16] Swift：Hello World
来源：http://vh.haigaiapp.cn

print("Hello")
来源：http://qt.bookmarksfly.cn

[T17] Swift：变量与常量
来源：http://sj.panjiajie.cn

var a = 1;  let b = 2
来源：http://oz.muxihuayi.cn

[T18] Swift：字符串插值
来源：http://hs.yuexingan06.cn

"值: \(b)"
来源：http://hl.chemitech.net.cn

[T19] Swift：可选绑定
来源：http://rp.wgjwhj.cn

if let n = opt { print(n) }
来源：http://nc.jctech888.com.cn

[T20] Swift：数组操作
来源：http://zl.nszjky.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qd.shxzskj.cn

[T21] Swift：遍历
来源：http://sf.newstarts.cn

for x in a { print(x) }
来源：http://rc.muxihuayi.cn

[T22] Swift：字典
来源：http://ft.jctech888.com.cn

var d = ["a": 1];  d["b"] = 2
来源：http://rp.huanxung.cn

[T23] Swift：函数
来源：http://qi.huanxung.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ci.szxytkj.cn

[T24] Swift：闭包
来源：http://xo.newstarts.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://cs.haigaiapp.cn

[T25] Swift：结构体
来源：http://gw.nicolike.cn

struct P { var x: Int }
来源：http://do.nicolike.cn

[T26] Swift：类与重写
来源：http://hf.nszjky.cn

class A: Base { override func f() {} }
来源：http://tn.bjjhwx.cn

[T27] Swift：错误处理
来源：http://yh.9csxet.cn

do { try f() } catch { print(error) }
来源：http://iw.bjjhwx.cn

[T28] Swift：枚举
来源：http://ak.shtwfgs.cn

enum Color { case red, green }
来源：http://gh.asd995.cn

[T29] Swift：guard 提前返回
来源：http://aw.bookmarksfly.cn

guard let x = opt else { return }
来源：http://zo.jctech888.com.cn

[T30] Swift：协议
来源：http://aw.nszjky.cn

protocol Shape { func area() -> Double }
来源：http://ym.chemitech.net.cn

[T31] Lua：Hello World
来源：http://lp.huixiangedu.cn

print("Hello")
来源：http://jq.colortex.cn

[T32] Lua：局部变量
来源：http://zw.huixinmuqiang.cn

local a = 1
来源：http://lj.szsharing.cn

[T33] Lua：表（数组）
来源：http://nc.panjiajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://jj.panjiajie.cn

[T34] Lua：遍历表
来源：http://ih.colortex.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ea.colortex.cn

[T35] Lua：字典表
来源：http://wg.jianghongdianzi.cn

local d = { a = 1 };  d.b = 2
来源：http://yy.nicolike.cn

[T36] Lua：函数
来源：http://dj.muxihuayi.cn

function add(a, b) return a + b end
来源：http://xi.shtwfgs.cn

[T37] Lua：字符串拼接
来源：http://yc.9csxet.cn

"a" .. "b"
来源：http://ce.shxzukj.cn

[T38] Lua：条件
来源：http://ks.huixinmuqiang.cn

if x > 0 then print("正") end
来源：http://vg.haigaiapp.cn

[T39] Lua：模式匹配
来源：http://xp.yuexingan06.cn

string.find(s, "%d+")
来源：http://yi.huixiangedu.cn

[T40] Lua：元表
来源：http://zc.bjjhwx.cn

setmetatable({}, { __index = base })
来源：http://hg.szxytkj.cn

[T41] Perl：Hello World
来源：http://pm.muxihuayi.cn

print "Hello\n";
来源：http://zl.9csxet.cn

[T42] Perl：变量类型
来源：http://nc.shxzukj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yb.nicolike.cn

[T43] Perl：字符串插值
来源：http://fd.gzmigu.cn

"值: $a"
来源：http://bw.yuntaijiaju.cn

[T44] Perl：条件
来源：http://fz.colortex.cn

if ($a > 0) { print "正"; }
来源：http://ej.colortex.cn

[T45] Perl：数组遍历
来源：http://yk.bjjhwx.cn

for my $x (@arr) { print $x; }
来源：http://he.hahajie.cn

[T46] Perl：哈希操作
来源：http://ar.521024.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jh.shtwfgs.cn

[T47] Perl：正则捕获
来源：http://vh.bookmarksfly.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://sp.yuntaijiaju.cn

[T48] Perl：正则替换
来源：http://kq.colortex.cn

$s =~ s/old/new/g;
来源：http://ix.bjjhwx.cn

[T49] Perl：函数
来源：http://ew.nszjky.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ut.nszjky.cn

[T50] Perl：逐行读文件
来源：http://kd.szsharing.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://mv.szxytkj.cn

while (my $line = <$fh>) { print $line; }
来源：http://km.bookmarksfly.cn

[T51] Scala：Hello World
来源：http://qm.wgjwhj.cn

println("Hello")
来源：http://ow.yuexingan06.cn

[T52] Scala：变量
来源：http://lk.huanxung.cn

val a = 1;  var b = 2
来源：http://gb.panjiajie.cn

[T53] Scala：字符串插值
来源：http://au.yuntaijiaju.cn

s"值: $b"
来源：http://oq.huixiangedu.cn

[T54] Scala：集合映射
来源：http://oy.szxytkj.cn

List(1, 2, 3).map(_ * 2)
来源：http://ye.newstarts.cn

[T55] Scala：集合过滤
来源：http://jj.colortex.cn

List(1, 2, 3).filter(_ > 1)
来源：http://og.yuexingan06.cn

[T56] Scala：样例类
来源：http://vt.muxihuayi.cn

case class User(name: String, age: Int)
来源：http://vn.jctech888.com.cn

[T57] Scala：模式匹配
来源：http://yu.panjiajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fy.szxytkj.cn

[T58] Scala：函数定义
来源：http://qs.wgjwhj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gg.yuexingan06.cn

[T59] Scala：循环
来源：http://uz.hahajie.cn

for (i <- 1 to 10) println(i)
来源：http://pl.9csxet.cn

[T60] Scala：折叠
来源：http://vf.shxzskj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cu.lnxyls.cn

================================================================================
来源：http://wk.muxihuayi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lp.gzmigu.cn

================================================================================
来源：http://yz.chemitech.net.cn

[U01] Py：创建虚拟环境
来源：http://kk.asd995.cn

python -m venv .venv && source .venv/bin/activate
来源：http://uk.yuntaijiaju.cn

[U02] Py：导出 / 安装依赖
来源：http://mk.hnjuh.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ug.muxihuayi.cn

[U03] Py：加载 .env 配置
来源：http://nn.nszjky.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rl.szxytkj.cn

[U04] Py：变量调试打印
来源：http://oo.bjjhwx.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ot.gzmigu.cn

[U05] Py：列表去重且保序
来源：http://yz.lnxyls.cn

list(dict.fromkeys(arr))
来源：http://hu.colortex.cn

[U06] Py：合并两个字典
来源：http://zz.huixinmuqiang.cn

{**a, **b}
来源：http://ij.szxytkj.cn

[U07] Py：反转字典键值
来源：http://tb.haigaiapp.cn

{v: k for k, v in d.items()}
来源：http://qt.yuntaijiaju.cn

[U08] Py：展平二维列表
来源：http://tl.yuntaijiaju.cn

[y for x in nested for y in x]
来源：http://nw.9csxet.cn

[U09] Py：字典取最大值的键
来源：http://lj.shxzukj.cn

max(d, key=d.get)
来源：http://jr.hahajie.cn

[U10] Py：按值排序字典
来源：http://tb.nszjky.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zq.szsharing.cn

[U11] Py：生成器表达式
来源：http://yh.colortex.cn

(x * 2 for x in arr)
来源：http://qu.huixinmuqiang.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lz.chemitech.net.cn

Counter(arr).most_common(3)
来源：http://es.huixinmuqiang.cn

[U13] Py：固定长度队列
来源：http://tq.gzmigu.cn

deque(maxlen=10)
来源：http://fh.colortex.cn

[U14] Py：分组收集到列表
来源：http://wg.chemitech.net.cn

defaultdict(list)
来源：http://vp.gzmigu.cn

[U15] Py：高精度计时
来源：http://qq.9csxet.cn

t = time.perf_counter()
来源：http://qz.colortex.cn

[U16] Py：命令行参数解析
来源：http://iv.haigaiapp.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://iq.chemitech.net.cn

[U17] Py：初始化日志
来源：http://ui.huixiangedu.cn

logging.basicConfig(level=logging.INFO)
来源：http://be.hahajie.cn

[U18] Py：预编译正则
来源：http://bw.521024.cn

pat = re.compile(r"\d+")
来源：http://dn.521024.cn

[U19] Py：正则替换带回调
来源：http://iy.521024.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qk.bjjhwx.cn

[U20] Py：缓存函数结果
来源：http://ig.huanxung.cn

@functools.lru_cache(maxsize=None)
来源：http://zy.jctech888.com.cn

[U21] Py：自定义上下文管理器
来源：http://ua.lnxyls.cn

@contextlib.contextmanager
来源：http://ok.shtwfgs.cn

[U22] Py：矩阵转置
来源：http://st.chemitech.net.cn

list(zip(*m))
来源：http://by.9csxet.cn

[U23] Py：分块读取大文件
来源：http://yw.szsharing.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://od.panjiajie.cn

[U24] Py：路径操作
来源：http://ny.bjjhwx.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ki.yuexingan06.cn

[U25] Py：CSV 按字典读
来源：http://aa.panjiajie.cn

csv.DictReader(f)
来源：http://jh.yuexingan06.cn

[U26] Py：并发下载
来源：http://wn.colortex.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ho.nszjky.cn

[U27] Py：异步 HTTP
来源：http://mt.jianghongdianzi.cn

aiohttp.ClientSession() 配合 async with
来源：http://bn.haigaiapp.cn

[U28] Py：类型别名
来源：http://xg.yuntaijiaju.cn

UserId = int
来源：http://gy.huixinmuqiang.cn

[U29] Py：属性校验
来源：http://ja.yuntaijiaju.cn

@property 与 @x.setter 配合
来源：http://oi.muxihuayi.cn

[U30] Py：数据类
来源：http://wx.chemitech.net.cn

@dataclass(slots=True)
来源：http://vi.asd995.cn

[U31] Py：单测
来源：http://lg.shxzskj.cn

python -m pytest -q
来源：http://tp.shtwfgs.cn

[U32] Py：代码格式化
来源：http://hx.lnxyls.cn

ruff format . && ruff check --fix .
来源：http://mm.huixiangedu.cn

[U33] Py：打包发布
来源：http://zm.chemitech.net.cn

python -m build  （依赖 pyproject.toml）
来源：http://fq.bjjhwx.cn

[U34] Py：判断编码
来源：http://lm.szxytkj.cn

chardet.detect(raw)
来源：http://ec.shxzskj.cn

[U35] Py：发送邮件
来源：http://mv.muxihuayi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bk.jctech888.com.cn

[U36] Py：定时任务
来源：http://xy.hahajie.cn

schedule.every(10).minutes.do(job)
来源：http://cn.gzmigu.cn

[U37] Py：读写 Excel
来源：http://mo.colortex.cn

pandas.read_excel / DataFrame.to_excel
来源：http://vy.yuntaijiaju.cn

[U38] Py：获取脚本所在目录
来源：http://wk.gzmigu.cn

Path(__file__).resolve().parent
来源：http://mq.hnjuh.cn

[U39] Py：判断是否在交互环境
来源：http://oy.nszjky.cn

sys.stdout.isatty()
来源：http://uo.shxzskj.cn

[U40] Py：打印到标准错误
来源：http://rk.yuntaijiaju.cn

print("err", file=sys.stderr)
来源：http://tz.yuntaijiaju.cn

[U41] PHP：初始化 Composer 项目
来源：http://mx.colortex.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://iz.nicolike.cn

[U42] PHP：PSR-4 自动加载
来源：http://in.yuntaijiaju.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kg.wgjwhj.cn

[U43] PHP：声明命名空间
来源：http://qg.hahajie.cn

namespace App\Http;
来源：http://rd.jianghongdianzi.cn

[U44] PHP：开启严格类型
来源：http://qf.nszjky.cn

declare(strict_types=1);
来源：http://ok.colortex.cn

[U45] PHP：类型声明与返回类型
来源：http://qe.szsharing.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://zc.nicolike.cn

[U46] PHP：可空类型
来源：http://xh.shtwfgs.cn

?string $name = null
来源：http://ek.muxihuayi.cn

[U47] PHP：联合类型
来源：http://rf.lnxyls.cn

int|string $id
来源：http://oi.shtwfgs.cn

[U48] PHP：纯枚举
来源：http://cs.huixiangedu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zw.haigaiapp.cn

[U49] PHP：只读属性
来源：http://fz.huixinmuqiang.cn

public readonly string $name
来源：http://ly.panjiajie.cn

[U50] PHP：构造器属性提升
来源：http://zc.yuexingan06.cn

public function __construct(private int $id) {}
来源：http://hn.gzmigu.cn

[U51] PHP：数组解构
来源：http://pv.panjiajie.cn

[$a, $b] = $arr;
来源：http://cl.nszjky.cn

[U52] PHP：箭头函数
来源：http://bv.shtwfgs.cn

$double = fn($x) => $x * 2;
来源：http://bl.yuntaijiaju.cn

[U53] PHP：空合并运算符
来源：http://wt.szsharing.cn

$v = $a ?? $b ?? "default";
来源：http://kp.wgjwhj.cn

[U54] PHP：空安全调用
来源：http://rb.newstarts.cn

$obj?->method()
来源：http://ad.shxzskj.cn

[U55] PHP：match 表达式
来源：http://pj.szsharing.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uf.wgjwhj.cn

[U56] PHP：命名参数
来源：http://gr.bjjhwx.cn

f(a: 1, b: 2)
来源：http://wf.muxihuayi.cn

[U57] PHP：字符串插值
来源：http://em.newstarts.cn

"值: {$a}"
来源：http://zc.panjiajie.cn

[U58] PHP：数组三件套
来源：http://yk.shxzukj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ij.huixinmuqiang.cn

[U59] PHP：自定义排序
来源：http://ik.jctech888.com.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zp.panjiajie.cn

[U60] PHP：JSON 编解码
来源：http://za.chemitech.net.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ta.colortex.cn

[U61] PHP：正则
来源：http://jw.hnjuh.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gi.huixiangedu.cn

[U62] PHP：日期对象
来源：http://vp.panjiajie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ii.jctech888.com.cn

[U63] PHP：文件读写
来源：http://ck.hnjuh.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ly.colortex.cn

[U64] PHP：目录遍历
来源：http://nv.jianghongdianzi.cn

glob("dir/*.php");  scandir("dir");
来源：http://sx.9csxet.cn

[U65] PHP：会话
来源：http://af.jianghongdianzi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ni.muxihuayi.cn

[U66] PHP：设置 Cookie
来源：http://sb.yuexingan06.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://un.haigaiapp.cn

[U67] PHP：处理文件上传
来源：http://pj.newstarts.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qe.9csxet.cn

[U68] PHP：PDO 连接
来源：http://dz.haigaiapp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uv.nszjky.cn

[U69] PHP：PDO 预处理
来源：http://ew.huixinmuqiang.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ya.gzmigu.cn

[U70] PHP：PDO 事务
来源：http://qn.muxihuayi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ou.521024.cn

[U71] PHP：抛出异常
来源：http://it.9csxet.cn

throw new RuntimeException("失败", 500);
来源：http://rp.gzmigu.cn

[U72] PHP：写错误日志
来源：http://ue.panjiajie.cn

error_log("失败: " . $e->getMessage());
来源：http://eo.szxytkj.cn

[U73] PHP：读取 ini 配置
来源：http://dt.hahajie.cn

parse_ini_file("config.ini", true)
来源：http://sc.hnjuh.cn

[U74] PHP：读取环境变量
来源：http://xh.nszjky.cn

getenv("APP_ENV") ?: "production"
来源：http://pp.hnjuh.cn

[U75] PHP：依赖注入
来源：http://ge.nszjky.cn

composer require psr/container
来源：http://zc.colortex.cn

[U76] PHP：简单路由
来源：http://mr.hahajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cn.jctech888.com.cn

[U77] PHP：模板渲染
来源：http://vu.shxzskj.cn

composer require twig/twig
来源：http://mh.gzmigu.cn

[U78] PHP：单元测试
来源：http://qy.hahajie.cn

composer require --dev phpunit/phpunit
来源：http://aw.szsharing.cn

[U79] PHP：静态分析
来源：http://vl.wgjwhj.cn

composer require --dev phpstan/phpstan
来源：http://lg.shtwfgs.cn

[U80] PHP：代码规范修复
来源：http://jz.huixiangedu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://rh.colortex.cn


<!-- 参考信息 -->