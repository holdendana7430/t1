代发 wailian999

int size() const noexcept { return n_; }
来源：http://mm.haigaiapp.cn

[S53] C++：移动语义
来源：http://xe.gzmigu.cn

std::vector<int> w = std::move(v);
来源：http://hp.huixinmuqiang.cn

[S54] C++：异常处理
来源：http://ec.asd995.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ml.yuntaijiaju.cn

[S55] C++：结构化绑定
来源：http://az.shxzskj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wf.hnjuh.cn

[S56] C++：optional
来源：http://qx.521024.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tk.szsharing.cn

[S57] C++：编译期常量
来源：http://ml.yuexingan06.cn

constexpr int N = 10;
来源：http://qh.wgjwhj.cn

[S58] C++：命名空间
来源：http://xs.wgjwhj.cn

namespace ns { int f() { return 1; } }
来源：http://qf.panjiajie.cn

[S59] C++：静态断言
来源：http://pi.jctech888.com.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xo.9csxet.cn

[S60] C++：遍历并删除元素
来源：http://nb.521024.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ys.lnxyls.cn

================================================================================
来源：http://lu.gzmigu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wa.yuexingan06.cn

================================================================================
来源：http://iy.huixiangedu.cn

[T01] Kotlin：Hello World
来源：http://nf.yuntaijiaju.cn

println("Hello")
来源：http://al.nicolike.cn

[T02] Kotlin：变量
来源：http://ft.colortex.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nj.yuntaijiaju.cn

[T03] Kotlin：字符串模板
来源：http://yd.yuntaijiaju.cn

"值: $b"
来源：http://mh.hahajie.cn

[T04] Kotlin：空安全
来源：http://uu.jianghongdianzi.cn

val n: String? = null;  n?.length
来源：http://fb.panjiajie.cn

[T05] Kotlin：when 表达式
来源：http://ol.yuexingan06.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dc.yuexingan06.cn

[T06] Kotlin：集合映射
来源：http://lw.lnxyls.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://kj.chemitech.net.cn

[T07] Kotlin：集合过滤
来源：http://na.chemitech.net.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://gp.shxzskj.cn

[T08] Kotlin：数据类
来源：http://dl.huixiangedu.cn

data class User(val name: String, val age: Int)
来源：http://xq.asd995.cn

[T09] Kotlin：扩展函数
来源：http://uv.521024.cn

fun String.exclaim() = this + "!"
来源：http://ji.colortex.cn

[T10] Kotlin：默认参数
来源：http://jf.chemitech.net.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://nb.huanxung.cn

[T11] Kotlin：协程
来源：http://iq.haigaiapp.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vt.lnxyls.cn

[T12] Kotlin：解构声明
来源：http://if.hahajie.cn

val (a, b) = Pair(1, 2)
来源：http://eo.shtwfgs.cn

[T13] Kotlin：只读 Map
来源：http://kz.huixiangedu.cn

val m = mapOf("a" to 1)
来源：http://he.shxzskj.cn

[T14] Kotlin：循环
来源：http://cw.bjjhwx.cn

for (i in 1..10) println(i)
来源：http://li.yuexingan06.cn

[T15] Kotlin：接口
来源：http://nl.shtwfgs.cn

interface Shape { fun area(): Double }
来源：http://pi.shtwfgs.cn

[T16] Swift：Hello World
来源：http://qd.bjjhwx.cn

print("Hello")
来源：http://gs.lnxyls.cn

[T17] Swift：变量与常量
来源：http://zb.asd995.cn

var a = 1;  let b = 2
来源：http://ek.szxytkj.cn

[T18] Swift：字符串插值
来源：http://vr.muxihuayi.cn

"值: \(b)"
来源：http://bh.shxzskj.cn

[T19] Swift：可选绑定
来源：http://fz.gzmigu.cn

if let n = opt { print(n) }
来源：http://cj.panjiajie.cn

[T20] Swift：数组操作
来源：http://he.hnjuh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://tj.bookmarksfly.cn

[T21] Swift：遍历
来源：http://dx.jctech888.com.cn

for x in a { print(x) }
来源：http://zq.hnjuh.cn

[T22] Swift：字典
来源：http://je.yuntaijiaju.cn

var d = ["a": 1];  d["b"] = 2
来源：http://jt.hnjuh.cn

[T23] Swift：函数
来源：http://jr.hahajie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jc.panjiajie.cn

[T24] Swift：闭包
来源：http://kr.huanxung.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://lw.colortex.cn

[T25] Swift：结构体
来源：http://zs.newstarts.cn

struct P { var x: Int }
来源：http://be.hnjuh.cn

[T26] Swift：类与重写
来源：http://xl.newstarts.cn

class A: Base { override func f() {} }
来源：http://rd.newstarts.cn

[T27] Swift：错误处理
来源：http://kw.haigaiapp.cn

do { try f() } catch { print(error) }
来源：http://xm.panjiajie.cn

[T28] Swift：枚举
来源：http://vs.huixinmuqiang.cn

enum Color { case red, green }
来源：http://hg.huixinmuqiang.cn

[T29] Swift：guard 提前返回
来源：http://rl.asd995.cn

guard let x = opt else { return }
来源：http://do.wgjwhj.cn

[T30] Swift：协议
来源：http://ku.jctech888.com.cn

protocol Shape { func area() -> Double }
来源：http://hz.huixinmuqiang.cn

[T31] Lua：Hello World
来源：http://uw.521024.cn

print("Hello")
来源：http://hm.521024.cn

[T32] Lua：局部变量
来源：http://ht.huixinmuqiang.cn

local a = 1
来源：http://fh.shxzukj.cn

[T33] Lua：表（数组）
来源：http://yo.szsharing.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://rh.521024.cn

[T34] Lua：遍历表
来源：http://eo.bookmarksfly.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zn.jctech888.com.cn

[T35] Lua：字典表
来源：http://nr.gzmigu.cn

local d = { a = 1 };  d.b = 2
来源：http://ci.huixinmuqiang.cn

[T36] Lua：函数
来源：http://ht.huixiangedu.cn

function add(a, b) return a + b end
来源：http://fi.huixiangedu.cn

[T37] Lua：字符串拼接
来源：http://sv.gzmigu.cn

"a" .. "b"
来源：http://uv.jianghongdianzi.cn

[T38] Lua：条件
来源：http://um.hahajie.cn

if x > 0 then print("正") end
来源：http://rl.chemitech.net.cn

[T39] Lua：模式匹配
来源：http://ix.colortex.cn

string.find(s, "%d+")
来源：http://lt.jctech888.com.cn

[T40] Lua：元表
来源：http://cw.newstarts.cn

setmetatable({}, { __index = base })
来源：http://ch.yuntaijiaju.cn

[T41] Perl：Hello World
来源：http://am.shtwfgs.cn

print "Hello\n";
来源：http://vv.shxzukj.cn

[T42] Perl：变量类型
来源：http://rk.bookmarksfly.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://is.huixiangedu.cn

[T43] Perl：字符串插值
来源：http://qa.hahajie.cn

"值: $a"
来源：http://jw.shtwfgs.cn

[T44] Perl：条件
来源：http://lv.jctech888.com.cn

if ($a > 0) { print "正"; }
来源：http://ne.huanxung.cn

[T45] Perl：数组遍历
来源：http://la.shxzskj.cn

for my $x (@arr) { print $x; }
来源：http://tt.haigaiapp.cn

[T46] Perl：哈希操作
来源：http://hv.yuntaijiaju.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jw.nicolike.cn

[T47] Perl：正则捕获
来源：http://la.huanxung.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://zg.bookmarksfly.cn

[T48] Perl：正则替换
来源：http://ow.yuexingan06.cn

$s =~ s/old/new/g;
来源：http://mt.muxihuayi.cn

[T49] Perl：函数
来源：http://ca.haigaiapp.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://eh.hnjuh.cn

[T50] Perl：逐行读文件
来源：http://zg.gzmigu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://jk.shxzukj.cn

while (my $line = <$fh>) { print $line; }
来源：http://ih.bjjhwx.cn

[T51] Scala：Hello World
来源：http://da.muxihuayi.cn

println("Hello")
来源：http://bs.shtwfgs.cn

[T52] Scala：变量
来源：http://ds.muxihuayi.cn

val a = 1;  var b = 2
来源：http://nz.jianghongdianzi.cn

[T53] Scala：字符串插值
来源：http://md.colortex.cn

s"值: $b"
来源：http://ng.nszjky.cn

[T54] Scala：集合映射
来源：http://px.9csxet.cn

List(1, 2, 3).map(_ * 2)
来源：http://bu.muxihuayi.cn

[T55] Scala：集合过滤
来源：http://dg.szsharing.cn

List(1, 2, 3).filter(_ > 1)
来源：http://nm.huanxung.cn

[T56] Scala：样例类
来源：http://wi.bookmarksfly.cn

case class User(name: String, age: Int)
来源：http://rw.huixiangedu.cn

[T57] Scala：模式匹配
来源：http://qg.yuexingan06.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://bk.jctech888.com.cn

[T58] Scala：函数定义
来源：http://hs.haigaiapp.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ay.asd995.cn

[T59] Scala：循环
来源：http://si.newstarts.cn

for (i <- 1 to 10) println(i)
来源：http://yr.lnxyls.cn

[T60] Scala：折叠
来源：http://ls.bjjhwx.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bc.lnxyls.cn

================================================================================
来源：http://zy.shxzukj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://el.hahajie.cn

================================================================================
来源：http://kj.wgjwhj.cn

[U01] Py：创建虚拟环境
来源：http://kw.huanxung.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ua.muxihuayi.cn

[U02] Py：导出 / 安装依赖
来源：http://rp.muxihuayi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://au.bjjhwx.cn

[U03] Py：加载 .env 配置
来源：http://pf.jctech888.com.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wo.gzmigu.cn

[U04] Py：变量调试打印
来源：http://cx.yuexingan06.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wl.bjjhwx.cn

[U05] Py：列表去重且保序
来源：http://jb.wgjwhj.cn

list(dict.fromkeys(arr))
来源：http://ep.chemitech.net.cn

[U06] Py：合并两个字典
来源：http://wx.yuexingan06.cn

{**a, **b}
来源：http://ac.nicolike.cn

[U07] Py：反转字典键值
来源：http://ve.hahajie.cn

{v: k for k, v in d.items()}
来源：http://jc.yuexingan06.cn

[U08] Py：展平二维列表
来源：http://mn.newstarts.cn

[y for x in nested for y in x]
来源：http://mf.shtwfgs.cn

[U09] Py：字典取最大值的键
来源：http://yj.521024.cn

max(d, key=d.get)
来源：http://uk.huixiangedu.cn

[U10] Py：按值排序字典
来源：http://xi.bjjhwx.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ot.szsharing.cn

[U11] Py：生成器表达式
来源：http://hn.nszjky.cn

(x * 2 for x in arr)
来源：http://aj.newstarts.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zi.shxzskj.cn

Counter(arr).most_common(3)
来源：http://rf.huixinmuqiang.cn

[U13] Py：固定长度队列
来源：http://oa.newstarts.cn

deque(maxlen=10)
来源：http://ho.chemitech.net.cn

[U14] Py：分组收集到列表
来源：http://nl.yuexingan06.cn

defaultdict(list)
来源：http://si.lnxyls.cn

[U15] Py：高精度计时
来源：http://ol.nicolike.cn

t = time.perf_counter()
来源：http://ht.panjiajie.cn

[U16] Py：命令行参数解析
来源：http://sd.gzmigu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zj.muxihuayi.cn

[U17] Py：初始化日志
来源：http://bg.shxzskj.cn

logging.basicConfig(level=logging.INFO)
来源：http://ar.panjiajie.cn

[U18] Py：预编译正则
来源：http://oc.nszjky.cn

pat = re.compile(r"\d+")
来源：http://zg.huixiangedu.cn

[U19] Py：正则替换带回调
来源：http://ln.panjiajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wc.nszjky.cn

[U20] Py：缓存函数结果
来源：http://jo.haigaiapp.cn

@functools.lru_cache(maxsize=None)
来源：http://gz.huixinmuqiang.cn

[U21] Py：自定义上下文管理器
来源：http://nh.huixinmuqiang.cn

@contextlib.contextmanager
来源：http://dx.huanxung.cn

[U22] Py：矩阵转置
来源：http://ms.wgjwhj.cn

list(zip(*m))
来源：http://nc.szxytkj.cn

[U23] Py：分块读取大文件
来源：http://mi.shxzskj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ww.bjjhwx.cn

[U24] Py：路径操作
来源：http://ik.huixiangedu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wv.colortex.cn

[U25] Py：CSV 按字典读
来源：http://xj.jctech888.com.cn

csv.DictReader(f)
来源：http://ic.nicolike.cn

[U26] Py：并发下载
来源：http://ns.yuexingan06.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://my.hnjuh.cn

[U27] Py：异步 HTTP
来源：http://zk.haigaiapp.cn

aiohttp.ClientSession() 配合 async with
来源：http://vx.haigaiapp.cn

[U28] Py：类型别名
来源：http://gy.szxytkj.cn

UserId = int
来源：http://bp.huanxung.cn

[U29] Py：属性校验
来源：http://ki.hahajie.cn

@property 与 @x.setter 配合
来源：http://fn.shxzskj.cn

[U30] Py：数据类
来源：http://mc.colortex.cn

@dataclass(slots=True)
来源：http://iw.bjjhwx.cn

[U31] Py：单测
来源：http://jw.szxytkj.cn

python -m pytest -q
来源：http://hj.huanxung.cn

[U32] Py：代码格式化
来源：http://qj.hnjuh.cn

ruff format . && ruff check --fix .
来源：http://ln.newstarts.cn

[U33] Py：打包发布
来源：http://no.szxytkj.cn

python -m build  （依赖 pyproject.toml）
来源：http://vv.newstarts.cn

[U34] Py：判断编码
来源：http://ct.hahajie.cn

chardet.detect(raw)
来源：http://hs.bookmarksfly.cn

[U35] Py：发送邮件
来源：http://fc.yuexingan06.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wn.shtwfgs.cn

[U36] Py：定时任务
来源：http://ae.newstarts.cn

schedule.every(10).minutes.do(job)
来源：http://wm.hnjuh.cn

[U37] Py：读写 Excel
来源：http://mj.521024.cn

pandas.read_excel / DataFrame.to_excel
来源：http://rk.huixiangedu.cn

[U38] Py：获取脚本所在目录
来源：http://lj.jctech888.com.cn

Path(__file__).resolve().parent
来源：http://dz.nicolike.cn

[U39] Py：判断是否在交互环境
来源：http://gt.panjiajie.cn

sys.stdout.isatty()
来源：http://be.wgjwhj.cn

[U40] Py：打印到标准错误
来源：http://gg.colortex.cn

print("err", file=sys.stderr)
来源：http://zf.yuntaijiaju.cn

[U41] PHP：初始化 Composer 项目
来源：http://sq.haigaiapp.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ts.hnjuh.cn

[U42] PHP：PSR-4 自动加载
来源：http://sx.haigaiapp.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kq.colortex.cn

[U43] PHP：声明命名空间
来源：http://hv.bookmarksfly.cn

namespace App\Http;
来源：http://cn.hahajie.cn

[U44] PHP：开启严格类型
来源：http://mh.panjiajie.cn

declare(strict_types=1);
来源：http://vp.szxytkj.cn

[U45] PHP：类型声明与返回类型
来源：http://mw.shxzukj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ih.wgjwhj.cn

[U46] PHP：可空类型
来源：http://te.muxihuayi.cn

?string $name = null
来源：http://qw.lnxyls.cn

[U47] PHP：联合类型
来源：http://lo.huixiangedu.cn

int|string $id
来源：http://bu.asd995.cn

[U48] PHP：纯枚举
来源：http://wn.shxzskj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zm.shxzukj.cn

[U49] PHP：只读属性
来源：http://bz.521024.cn

public readonly string $name
来源：http://ex.hnjuh.cn

[U50] PHP：构造器属性提升
来源：http://sx.newstarts.cn

public function __construct(private int $id) {}
来源：http://mx.jianghongdianzi.cn

[U51] PHP：数组解构
来源：http://dt.huixinmuqiang.cn

[$a, $b] = $arr;
来源：http://sz.yuntaijiaju.cn

[U52] PHP：箭头函数
来源：http://me.521024.cn

$double = fn($x) => $x * 2;
来源：http://zl.hnjuh.cn

[U53] PHP：空合并运算符
来源：http://tw.newstarts.cn

$v = $a ?? $b ?? "default";
来源：http://zr.yuexingan06.cn

[U54] PHP：空安全调用
来源：http://su.colortex.cn

$obj?->method()
来源：http://yr.lnxyls.cn

[U55] PHP：match 表达式
来源：http://nt.szxytkj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cx.nicolike.cn

[U56] PHP：命名参数
来源：http://rq.yuexingan06.cn

f(a: 1, b: 2)
来源：http://oe.9csxet.cn

[U57] PHP：字符串插值
来源：http://gc.lnxyls.cn

"值: {$a}"
来源：http://om.colortex.cn

[U58] PHP：数组三件套
来源：http://bh.9csxet.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://aq.shxzskj.cn

[U59] PHP：自定义排序
来源：http://nf.huixinmuqiang.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://in.521024.cn

[U60] PHP：JSON 编解码
来源：http://pp.521024.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://uk.muxihuayi.cn

[U61] PHP：正则
来源：http://uu.nszjky.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://di.muxihuayi.cn

[U62] PHP：日期对象
来源：http://xs.chemitech.net.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gm.gzmigu.cn

[U63] PHP：文件读写
来源：http://nv.shtwfgs.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gj.szxytkj.cn

[U64] PHP：目录遍历
来源：http://wn.jctech888.com.cn

glob("dir/*.php");  scandir("dir");
来源：http://ls.hahajie.cn

[U65] PHP：会话
来源：http://tn.chemitech.net.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://zw.gzmigu.cn

[U66] PHP：设置 Cookie
来源：http://rr.521024.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vu.shtwfgs.cn

[U67] PHP：处理文件上传
来源：http://qk.shxzukj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://uv.newstarts.cn

[U68] PHP：PDO 连接
来源：http://ic.nicolike.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://we.bjjhwx.cn

[U69] PHP：PDO 预处理
来源：http://vv.gzmigu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ly.bjjhwx.cn

[U70] PHP：PDO 事务
来源：http://xc.newstarts.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cl.nszjky.cn

[U71] PHP：抛出异常
来源：http://wr.lnxyls.cn

throw new RuntimeException("失败", 500);
来源：http://yp.gzmigu.cn

[U72] PHP：写错误日志
来源：http://nh.jctech888.com.cn

error_log("失败: " . $e->getMessage());
来源：http://ac.muxihuayi.cn

[U73] PHP：读取 ini 配置
来源：http://bh.huanxung.cn

parse_ini_file("config.ini", true)
来源：http://ip.jctech888.com.cn

[U74] PHP：读取环境变量
来源：http://cr.chemitech.net.cn

getenv("APP_ENV") ?: "production"
来源：http://qm.yuexingan06.cn

[U75] PHP：依赖注入
来源：http://xc.szsharing.cn

composer require psr/container
来源：http://sw.jctech888.com.cn

[U76] PHP：简单路由
来源：http://rg.colortex.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wa.haigaiapp.cn

[U77] PHP：模板渲染
来源：http://fh.haigaiapp.cn

composer require twig/twig
来源：http://ou.huixinmuqiang.cn

[U78] PHP：单元测试
来源：http://pg.gzmigu.cn

composer require --dev phpunit/phpunit
来源：http://zv.colortex.cn


<!-- 参考信息 -->