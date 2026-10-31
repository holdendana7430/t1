代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ju.szxytkj.cn

[S55] C++：结构化绑定
来源：http://qw.hahajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cx.9csxet.cn

[S56] C++：optional
来源：http://bd.hahajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cp.wgjwhj.cn

[S57] C++：编译期常量
来源：http://ab.9csxet.cn

constexpr int N = 10;
来源：http://te.gzmigu.cn

[S58] C++：命名空间
来源：http://wu.huanxung.cn

namespace ns { int f() { return 1; } }
来源：http://rs.asd995.cn

[S59] C++：静态断言
来源：http://gd.hnjuh.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ov.shtwfgs.cn

[S60] C++：遍历并删除元素
来源：http://rq.yuexingan06.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kp.shxzskj.cn

================================================================================
来源：http://zx.nicolike.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://re.colortex.cn

================================================================================
来源：http://wf.lnxyls.cn

[T01] Kotlin：Hello World
来源：http://ut.yuexingan06.cn

println("Hello")
来源：http://tu.jctech888.com.cn

[T02] Kotlin：变量
来源：http://hc.colortex.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gx.shxzukj.cn

[T03] Kotlin：字符串模板
来源：http://cs.shxzukj.cn

"值: $b"
来源：http://hc.asd995.cn

[T04] Kotlin：空安全
来源：http://de.jianghongdianzi.cn

val n: String? = null;  n?.length
来源：http://lp.jctech888.com.cn

[T05] Kotlin：when 表达式
来源：http://bi.shtwfgs.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gi.9csxet.cn

[T06] Kotlin：集合映射
来源：http://of.huixinmuqiang.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fs.newstarts.cn

[T07] Kotlin：集合过滤
来源：http://vu.jctech888.com.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://bf.colortex.cn

[T08] Kotlin：数据类
来源：http://am.chemitech.net.cn

data class User(val name: String, val age: Int)
来源：http://by.colortex.cn

[T09] Kotlin：扩展函数
来源：http://sp.chemitech.net.cn

fun String.exclaim() = this + "!"
来源：http://dq.huixinmuqiang.cn

[T10] Kotlin：默认参数
来源：http://jy.521024.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jy.hahajie.cn

[T11] Kotlin：协程
来源：http://cw.nicolike.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qv.muxihuayi.cn

[T12] Kotlin：解构声明
来源：http://gh.jctech888.com.cn

val (a, b) = Pair(1, 2)
来源：http://cn.bjjhwx.cn

[T13] Kotlin：只读 Map
来源：http://fe.shxzskj.cn

val m = mapOf("a" to 1)
来源：http://qs.nszjky.cn

[T14] Kotlin：循环
来源：http://ks.hahajie.cn

for (i in 1..10) println(i)
来源：http://gi.jianghongdianzi.cn

[T15] Kotlin：接口
来源：http://qd.jctech888.com.cn

interface Shape { fun area(): Double }
来源：http://ox.9csxet.cn

[T16] Swift：Hello World
来源：http://ck.shxzukj.cn

print("Hello")
来源：http://zm.szxytkj.cn

[T17] Swift：变量与常量
来源：http://kr.panjiajie.cn

var a = 1;  let b = 2
来源：http://ry.huixinmuqiang.cn

[T18] Swift：字符串插值
来源：http://tl.hnjuh.cn

"值: \(b)"
来源：http://mf.nszjky.cn

[T19] Swift：可选绑定
来源：http://su.bjjhwx.cn

if let n = opt { print(n) }
来源：http://xh.panjiajie.cn

[T20] Swift：数组操作
来源：http://jz.huixiangedu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mk.gzmigu.cn

[T21] Swift：遍历
来源：http://af.jctech888.com.cn

for x in a { print(x) }
来源：http://me.bookmarksfly.cn

[T22] Swift：字典
来源：http://lg.wgjwhj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://em.newstarts.cn

[T23] Swift：函数
来源：http://jb.huanxung.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wl.9csxet.cn

[T24] Swift：闭包
来源：http://tf.huixiangedu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qj.shxzukj.cn

[T25] Swift：结构体
来源：http://ct.huixinmuqiang.cn

struct P { var x: Int }
来源：http://xf.bjjhwx.cn

[T26] Swift：类与重写
来源：http://ig.jianghongdianzi.cn

class A: Base { override func f() {} }
来源：http://fe.bjjhwx.cn

[T27] Swift：错误处理
来源：http://ai.nicolike.cn

do { try f() } catch { print(error) }
来源：http://fi.panjiajie.cn

[T28] Swift：枚举
来源：http://vz.haigaiapp.cn

enum Color { case red, green }
来源：http://ra.newstarts.cn

[T29] Swift：guard 提前返回
来源：http://yr.shxzukj.cn

guard let x = opt else { return }
来源：http://uq.hnjuh.cn

[T30] Swift：协议
来源：http://ox.lnxyls.cn

protocol Shape { func area() -> Double }
来源：http://si.bookmarksfly.cn

[T31] Lua：Hello World
来源：http://nu.yuntaijiaju.cn

print("Hello")
来源：http://gp.hnjuh.cn

[T32] Lua：局部变量
来源：http://qo.shxzukj.cn

local a = 1
来源：http://wt.lnxyls.cn

[T33] Lua：表（数组）
来源：http://lc.wgjwhj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vv.nicolike.cn

[T34] Lua：遍历表
来源：http://nd.jianghongdianzi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qr.yuntaijiaju.cn

[T35] Lua：字典表
来源：http://xt.nicolike.cn

local d = { a = 1 };  d.b = 2
来源：http://og.shxzukj.cn

[T36] Lua：函数
来源：http://qs.colortex.cn

function add(a, b) return a + b end
来源：http://gk.szsharing.cn

[T37] Lua：字符串拼接
来源：http://ew.asd995.cn

"a" .. "b"
来源：http://gy.nszjky.cn

[T38] Lua：条件
来源：http://wz.muxihuayi.cn

if x > 0 then print("正") end
来源：http://gl.huixinmuqiang.cn

[T39] Lua：模式匹配
来源：http://jw.shxzukj.cn

string.find(s, "%d+")
来源：http://uf.gzmigu.cn

[T40] Lua：元表
来源：http://tj.newstarts.cn

setmetatable({}, { __index = base })
来源：http://hv.haigaiapp.cn

[T41] Perl：Hello World
来源：http://hr.shxzukj.cn

print "Hello\n";
来源：http://db.shxzskj.cn

[T42] Perl：变量类型
来源：http://mw.haigaiapp.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lw.hahajie.cn

[T43] Perl：字符串插值
来源：http://ht.yuntaijiaju.cn

"值: $a"
来源：http://ty.nicolike.cn

[T44] Perl：条件
来源：http://hg.muxihuayi.cn

if ($a > 0) { print "正"; }
来源：http://qc.szxytkj.cn

[T45] Perl：数组遍历
来源：http://nx.lnxyls.cn

for my $x (@arr) { print $x; }
来源：http://yk.lnxyls.cn

[T46] Perl：哈希操作
来源：http://hh.szxytkj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ex.shtwfgs.cn

[T47] Perl：正则捕获
来源：http://kq.huixiangedu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://gl.bookmarksfly.cn

[T48] Perl：正则替换
来源：http://mc.jctech888.com.cn

$s =~ s/old/new/g;
来源：http://ah.wgjwhj.cn

[T49] Perl：函数
来源：http://zc.9csxet.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yn.newstarts.cn

[T50] Perl：逐行读文件
来源：http://sz.nszjky.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xa.shxzskj.cn

while (my $line = <$fh>) { print $line; }
来源：http://cr.jctech888.com.cn

[T51] Scala：Hello World
来源：http://xc.haigaiapp.cn

println("Hello")
来源：http://hm.panjiajie.cn

[T52] Scala：变量
来源：http://vv.bookmarksfly.cn

val a = 1;  var b = 2
来源：http://ac.wgjwhj.cn

[T53] Scala：字符串插值
来源：http://uy.521024.cn

s"值: $b"
来源：http://wc.asd995.cn

[T54] Scala：集合映射
来源：http://ue.newstarts.cn

List(1, 2, 3).map(_ * 2)
来源：http://vm.newstarts.cn

[T55] Scala：集合过滤
来源：http://dx.panjiajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://cr.panjiajie.cn

[T56] Scala：样例类
来源：http://ye.gzmigu.cn

case class User(name: String, age: Int)
来源：http://lu.bjjhwx.cn

[T57] Scala：模式匹配
来源：http://lb.bookmarksfly.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://dj.yuntaijiaju.cn

[T58] Scala：函数定义
来源：http://kr.asd995.cn

def add(a: Int, b: Int): Int = a + b
来源：http://kg.jianghongdianzi.cn

[T59] Scala：循环
来源：http://sl.shxzskj.cn

for (i <- 1 to 10) println(i)
来源：http://py.huanxung.cn

[T60] Scala：折叠
来源：http://hl.nicolike.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vb.nszjky.cn

================================================================================
来源：http://ms.newstarts.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ya.9csxet.cn

================================================================================
来源：http://da.shtwfgs.cn

[U01] Py：创建虚拟环境
来源：http://am.haigaiapp.cn

python -m venv .venv && source .venv/bin/activate
来源：http://iq.huixinmuqiang.cn

[U02] Py：导出 / 安装依赖
来源：http://we.yuntaijiaju.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dn.panjiajie.cn

[U03] Py：加载 .env 配置
来源：http://wy.huanxung.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://cl.hahajie.cn

[U04] Py：变量调试打印
来源：http://rr.asd995.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xj.bookmarksfly.cn

[U05] Py：列表去重且保序
来源：http://lj.wgjwhj.cn

list(dict.fromkeys(arr))
来源：http://ap.chemitech.net.cn

[U06] Py：合并两个字典
来源：http://xo.shxzskj.cn

{**a, **b}
来源：http://al.9csxet.cn

[U07] Py：反转字典键值
来源：http://ob.jctech888.com.cn

{v: k for k, v in d.items()}
来源：http://rw.nicolike.cn

[U08] Py：展平二维列表
来源：http://ac.shxzukj.cn

[y for x in nested for y in x]
来源：http://yn.gzmigu.cn

[U09] Py：字典取最大值的键
来源：http://lw.shtwfgs.cn

max(d, key=d.get)
来源：http://jb.haigaiapp.cn

[U10] Py：按值排序字典
来源：http://yv.yuexingan06.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rf.shxzskj.cn

[U11] Py：生成器表达式
来源：http://gt.nicolike.cn

(x * 2 for x in arr)
来源：http://uj.haigaiapp.cn

[U12] Py：取出现最多的 3 个元素
来源：http://bv.521024.cn

Counter(arr).most_common(3)
来源：http://ia.hahajie.cn

[U13] Py：固定长度队列
来源：http://ph.wgjwhj.cn

deque(maxlen=10)
来源：http://ky.lnxyls.cn

[U14] Py：分组收集到列表
来源：http://ht.9csxet.cn

defaultdict(list)
来源：http://xb.9csxet.cn

[U15] Py：高精度计时
来源：http://gq.huixiangedu.cn

t = time.perf_counter()
来源：http://xp.9csxet.cn

[U16] Py：命令行参数解析
来源：http://vg.shxzskj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ud.jctech888.com.cn

[U17] Py：初始化日志
来源：http://jj.lnxyls.cn

logging.basicConfig(level=logging.INFO)
来源：http://nf.newstarts.cn

[U18] Py：预编译正则
来源：http://ma.hnjuh.cn

pat = re.compile(r"\d+")
来源：http://qt.9csxet.cn

[U19] Py：正则替换带回调
来源：http://sk.shxzukj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yx.nszjky.cn

[U20] Py：缓存函数结果
来源：http://qk.shtwfgs.cn

@functools.lru_cache(maxsize=None)
来源：http://qd.panjiajie.cn

[U21] Py：自定义上下文管理器
来源：http://tr.yuntaijiaju.cn

@contextlib.contextmanager
来源：http://sa.hahajie.cn

[U22] Py：矩阵转置
来源：http://le.newstarts.cn

list(zip(*m))
来源：http://ti.asd995.cn

[U23] Py：分块读取大文件
来源：http://mn.hnjuh.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pm.gzmigu.cn

[U24] Py：路径操作
来源：http://zx.yuntaijiaju.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hq.huixinmuqiang.cn

[U25] Py：CSV 按字典读
来源：http://vh.colortex.cn

csv.DictReader(f)
来源：http://ao.shxzukj.cn

[U26] Py：并发下载
来源：http://iu.huixiangedu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wq.nicolike.cn

[U27] Py：异步 HTTP
来源：http://fp.szsharing.cn

aiohttp.ClientSession() 配合 async with
来源：http://zf.shxzskj.cn

[U28] Py：类型别名
来源：http://fb.jianghongdianzi.cn

UserId = int
来源：http://hs.huixiangedu.cn

[U29] Py：属性校验
来源：http://ob.shxzskj.cn

@property 与 @x.setter 配合
来源：http://tz.asd995.cn

[U30] Py：数据类
来源：http://sc.gzmigu.cn

@dataclass(slots=True)
来源：http://vw.bjjhwx.cn

[U31] Py：单测
来源：http://gx.yuntaijiaju.cn

python -m pytest -q
来源：http://gz.huixinmuqiang.cn

[U32] Py：代码格式化
来源：http://wx.hahajie.cn

ruff format . && ruff check --fix .
来源：http://ng.haigaiapp.cn

[U33] Py：打包发布
来源：http://rw.nicolike.cn

python -m build  （依赖 pyproject.toml）
来源：http://za.521024.cn

[U34] Py：判断编码
来源：http://ap.huixiangedu.cn

chardet.detect(raw)
来源：http://we.asd995.cn

[U35] Py：发送邮件
来源：http://zh.lnxyls.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://py.szsharing.cn

[U36] Py：定时任务
来源：http://ks.shxzskj.cn

schedule.every(10).minutes.do(job)
来源：http://dt.521024.cn

[U37] Py：读写 Excel
来源：http://xx.bjjhwx.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jw.521024.cn

[U38] Py：获取脚本所在目录
来源：http://vw.huixiangedu.cn

Path(__file__).resolve().parent
来源：http://sf.lnxyls.cn

[U39] Py：判断是否在交互环境
来源：http://ny.hnjuh.cn

sys.stdout.isatty()
来源：http://ol.gzmigu.cn

[U40] Py：打印到标准错误
来源：http://gd.hahajie.cn

print("err", file=sys.stderr)
来源：http://eq.521024.cn

[U41] PHP：初始化 Composer 项目
来源：http://rn.szxytkj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://cr.jianghongdianzi.cn

[U42] PHP：PSR-4 自动加载
来源：http://rl.9csxet.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yy.szxytkj.cn

[U43] PHP：声明命名空间
来源：http://ni.nszjky.cn

namespace App\Http;
来源：http://et.bjjhwx.cn

[U44] PHP：开启严格类型
来源：http://rj.bjjhwx.cn

declare(strict_types=1);
来源：http://ad.lnxyls.cn

[U45] PHP：类型声明与返回类型
来源：http://db.bookmarksfly.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ss.shtwfgs.cn

[U46] PHP：可空类型
来源：http://ve.yuntaijiaju.cn

?string $name = null
来源：http://oa.huanxung.cn

[U47] PHP：联合类型
来源：http://no.gzmigu.cn

int|string $id
来源：http://dg.newstarts.cn

[U48] PHP：纯枚举
来源：http://id.huixiangedu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dd.huixiangedu.cn

[U49] PHP：只读属性
来源：http://pl.newstarts.cn

public readonly string $name
来源：http://ww.shtwfgs.cn

[U50] PHP：构造器属性提升
来源：http://je.yuntaijiaju.cn

public function __construct(private int $id) {}
来源：http://ut.chemitech.net.cn

[U51] PHP：数组解构
来源：http://iz.jianghongdianzi.cn

[$a, $b] = $arr;
来源：http://xr.nicolike.cn

[U52] PHP：箭头函数
来源：http://jf.jctech888.com.cn

$double = fn($x) => $x * 2;
来源：http://az.9csxet.cn

[U53] PHP：空合并运算符
来源：http://xk.lnxyls.cn

$v = $a ?? $b ?? "default";
来源：http://sn.nicolike.cn

[U54] PHP：空安全调用
来源：http://wg.szsharing.cn

$obj?->method()
来源：http://wk.shxzukj.cn

[U55] PHP：match 表达式
来源：http://lz.szsharing.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.nicolike.cn

[U56] PHP：命名参数
来源：http://ud.shxzukj.cn

f(a: 1, b: 2)
来源：http://uq.hnjuh.cn

[U57] PHP：字符串插值
来源：http://zb.bookmarksfly.cn

"值: {$a}"
来源：http://dn.shxzukj.cn

[U58] PHP：数组三件套
来源：http://rp.muxihuayi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://uh.bjjhwx.cn

[U59] PHP：自定义排序
来源：http://gt.lnxyls.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jp.nicolike.cn

[U60] PHP：JSON 编解码
来源：http://yz.lnxyls.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gx.521024.cn

[U61] PHP：正则
来源：http://jp.lnxyls.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pb.szxytkj.cn

[U62] PHP：日期对象
来源：http://rn.yuntaijiaju.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://op.nicolike.cn

[U63] PHP：文件读写
来源：http://at.wgjwhj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ao.szsharing.cn

[U64] PHP：目录遍历
来源：http://zz.bookmarksfly.cn

glob("dir/*.php");  scandir("dir");
来源：http://np.haigaiapp.cn

[U65] PHP：会话
来源：http://pt.colortex.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://sp.asd995.cn

[U66] PHP：设置 Cookie
来源：http://gm.huixiangedu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ia.yuexingan06.cn

[U67] PHP：处理文件上传
来源：http://ep.shxzskj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yi.gzmigu.cn

[U68] PHP：PDO 连接
来源：http://li.lnxyls.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pt.wgjwhj.cn

[U69] PHP：PDO 预处理
来源：http://oe.huixiangedu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yi.panjiajie.cn

[U70] PHP：PDO 事务
来源：http://uu.huanxung.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yn.jianghongdianzi.cn

[U71] PHP：抛出异常
来源：http://kb.lnxyls.cn

throw new RuntimeException("失败", 500);
来源：http://bf.521024.cn

[U72] PHP：写错误日志
来源：http://ll.huanxung.cn

error_log("失败: " . $e->getMessage());
来源：http://aw.nicolike.cn

[U73] PHP：读取 ini 配置
来源：http://en.shxzskj.cn

parse_ini_file("config.ini", true)
来源：http://pe.haigaiapp.cn

[U74] PHP：读取环境变量
来源：http://do.hnjuh.cn

getenv("APP_ENV") ?: "production"
来源：http://kq.yuexingan06.cn

[U75] PHP：依赖注入
来源：http://nj.hahajie.cn

composer require psr/container
来源：http://yw.wgjwhj.cn

[U76] PHP：简单路由
来源：http://ud.hahajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yw.jianghongdianzi.cn

[U77] PHP：模板渲染
来源：http://zl.shxzukj.cn

composer require twig/twig
来源：http://py.szsharing.cn

[U78] PHP：单元测试
来源：http://ph.521024.cn

composer require --dev phpunit/phpunit
来源：http://db.hahajie.cn

[U79] PHP：静态分析
来源：http://dp.bookmarksfly.cn

composer require --dev phpstan/phpstan
来源：http://rn.hahajie.cn

[U80] PHP：代码规范修复
来源：http://em.muxihuayi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://sq.nicolike.cn


<!-- 参考信息 -->