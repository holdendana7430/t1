代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hg.huixinmuqiang.cn

[S55] C++：结构化绑定
来源：http://yx.yuntaijiaju.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ri.jctech888.com.cn

[S56] C++：optional
来源：http://em.9csxet.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hf.hahajie.cn

[S57] C++：编译期常量
来源：http://sp.colortex.cn

constexpr int N = 10;
来源：http://st.szsharing.cn

[S58] C++：命名空间
来源：http://nv.szxytkj.cn

namespace ns { int f() { return 1; } }
来源：http://jm.nszjky.cn

[S59] C++：静态断言
来源：http://dc.nszjky.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qg.wgjwhj.cn

[S60] C++：遍历并删除元素
来源：http://zz.9csxet.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ua.chemitech.net.cn

================================================================================
来源：http://it.wgjwhj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://su.chemitech.net.cn

================================================================================
来源：http://hb.hnjuh.cn

[T01] Kotlin：Hello World
来源：http://rc.asd995.cn

println("Hello")
来源：http://cy.bjjhwx.cn

[T02] Kotlin：变量
来源：http://dd.shxzukj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fh.shtwfgs.cn

[T03] Kotlin：字符串模板
来源：http://ic.bookmarksfly.cn

"值: $b"
来源：http://wh.bookmarksfly.cn

[T04] Kotlin：空安全
来源：http://hs.szsharing.cn

val n: String? = null;  n?.length
来源：http://of.gzmigu.cn

[T05] Kotlin：when 表达式
来源：http://qt.chemitech.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ak.jianghongdianzi.cn

[T06] Kotlin：集合映射
来源：http://gv.haigaiapp.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://mw.shxzukj.cn

[T07] Kotlin：集合过滤
来源：http://ju.huixinmuqiang.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xu.bjjhwx.cn

[T08] Kotlin：数据类
来源：http://oj.szxytkj.cn

data class User(val name: String, val age: Int)
来源：http://sa.haigaiapp.cn

[T09] Kotlin：扩展函数
来源：http://ey.panjiajie.cn

fun String.exclaim() = this + "!"
来源：http://fj.yuexingan06.cn

[T10] Kotlin：默认参数
来源：http://mq.hnjuh.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hv.yuntaijiaju.cn

[T11] Kotlin：协程
来源：http://hq.huixinmuqiang.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jh.chemitech.net.cn

[T12] Kotlin：解构声明
来源：http://vb.hahajie.cn

val (a, b) = Pair(1, 2)
来源：http://fd.huixiangedu.cn

[T13] Kotlin：只读 Map
来源：http://xq.yuexingan06.cn

val m = mapOf("a" to 1)
来源：http://am.521024.cn

[T14] Kotlin：循环
来源：http://mw.shxzukj.cn

for (i in 1..10) println(i)
来源：http://bn.huanxung.cn

[T15] Kotlin：接口
来源：http://pl.yuntaijiaju.cn

interface Shape { fun area(): Double }
来源：http://xf.shtwfgs.cn

[T16] Swift：Hello World
来源：http://rv.lnxyls.cn

print("Hello")
来源：http://cj.yuntaijiaju.cn

[T17] Swift：变量与常量
来源：http://rh.jianghongdianzi.cn

var a = 1;  let b = 2
来源：http://ks.muxihuayi.cn

[T18] Swift：字符串插值
来源：http://be.szsharing.cn

"值: \(b)"
来源：http://pd.shxzskj.cn

[T19] Swift：可选绑定
来源：http://ph.9csxet.cn

if let n = opt { print(n) }
来源：http://mv.szxytkj.cn

[T20] Swift：数组操作
来源：http://cc.yuexingan06.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gu.newstarts.cn

[T21] Swift：遍历
来源：http://as.gzmigu.cn

for x in a { print(x) }
来源：http://lb.shxzukj.cn

[T22] Swift：字典
来源：http://mx.huanxung.cn

var d = ["a": 1];  d["b"] = 2
来源：http://dr.jianghongdianzi.cn

[T23] Swift：函数
来源：http://nq.panjiajie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://oh.lnxyls.cn

[T24] Swift：闭包
来源：http://kz.shtwfgs.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://wd.521024.cn

[T25] Swift：结构体
来源：http://hx.hahajie.cn

struct P { var x: Int }
来源：http://bh.nszjky.cn

[T26] Swift：类与重写
来源：http://ek.huixinmuqiang.cn

class A: Base { override func f() {} }
来源：http://oi.szxytkj.cn

[T27] Swift：错误处理
来源：http://zp.huanxung.cn

do { try f() } catch { print(error) }
来源：http://zc.shtwfgs.cn

[T28] Swift：枚举
来源：http://io.shtwfgs.cn

enum Color { case red, green }
来源：http://cz.wgjwhj.cn

[T29] Swift：guard 提前返回
来源：http://xi.yuntaijiaju.cn

guard let x = opt else { return }
来源：http://qd.szsharing.cn

[T30] Swift：协议
来源：http://qk.hnjuh.cn

protocol Shape { func area() -> Double }
来源：http://it.gzmigu.cn

[T31] Lua：Hello World
来源：http://or.hnjuh.cn

print("Hello")
来源：http://os.haigaiapp.cn

[T32] Lua：局部变量
来源：http://qf.chemitech.net.cn

local a = 1
来源：http://mn.nicolike.cn

[T33] Lua：表（数组）
来源：http://hz.nszjky.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hw.yuexingan06.cn

[T34] Lua：遍历表
来源：http://sd.shxzskj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://lx.shtwfgs.cn

[T35] Lua：字典表
来源：http://nb.hnjuh.cn

local d = { a = 1 };  d.b = 2
来源：http://wo.szsharing.cn

[T36] Lua：函数
来源：http://xk.haigaiapp.cn

function add(a, b) return a + b end
来源：http://eb.huixinmuqiang.cn

[T37] Lua：字符串拼接
来源：http://za.yuexingan06.cn

"a" .. "b"
来源：http://ax.huixinmuqiang.cn

[T38] Lua：条件
来源：http://fu.huixiangedu.cn

if x > 0 then print("正") end
来源：http://vz.muxihuayi.cn

[T39] Lua：模式匹配
来源：http://jt.hahajie.cn

string.find(s, "%d+")
来源：http://gu.muxihuayi.cn

[T40] Lua：元表
来源：http://lv.hahajie.cn

setmetatable({}, { __index = base })
来源：http://vd.colortex.cn

[T41] Perl：Hello World
来源：http://jo.9csxet.cn

print "Hello\n";
来源：http://cu.huixinmuqiang.cn

[T42] Perl：变量类型
来源：http://gs.hahajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fa.muxihuayi.cn

[T43] Perl：字符串插值
来源：http://ea.9csxet.cn

"值: $a"
来源：http://jf.lnxyls.cn

[T44] Perl：条件
来源：http://eq.9csxet.cn

if ($a > 0) { print "正"; }
来源：http://zc.9csxet.cn

[T45] Perl：数组遍历
来源：http://tr.hnjuh.cn

for my $x (@arr) { print $x; }
来源：http://ck.yuntaijiaju.cn

[T46] Perl：哈希操作
来源：http://vt.bookmarksfly.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rb.asd995.cn

[T47] Perl：正则捕获
来源：http://vi.yuntaijiaju.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://et.bjjhwx.cn

[T48] Perl：正则替换
来源：http://bq.shtwfgs.cn

$s =~ s/old/new/g;
来源：http://nj.nicolike.cn

[T49] Perl：函数
来源：http://gz.521024.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zc.jctech888.com.cn

[T50] Perl：逐行读文件
来源：http://fb.lnxyls.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ak.asd995.cn

while (my $line = <$fh>) { print $line; }
来源：http://qa.muxihuayi.cn

[T51] Scala：Hello World
来源：http://fl.szxytkj.cn

println("Hello")
来源：http://yi.huanxung.cn

[T52] Scala：变量
来源：http://uv.chemitech.net.cn

val a = 1;  var b = 2
来源：http://de.huixinmuqiang.cn

[T53] Scala：字符串插值
来源：http://gn.gzmigu.cn

s"值: $b"
来源：http://do.muxihuayi.cn

[T54] Scala：集合映射
来源：http://wl.wgjwhj.cn

List(1, 2, 3).map(_ * 2)
来源：http://vv.jctech888.com.cn

[T55] Scala：集合过滤
来源：http://kv.nicolike.cn

List(1, 2, 3).filter(_ > 1)
来源：http://yy.newstarts.cn

[T56] Scala：样例类
来源：http://ln.lnxyls.cn

case class User(name: String, age: Int)
来源：http://xm.gzmigu.cn

[T57] Scala：模式匹配
来源：http://fs.huanxung.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fo.gzmigu.cn

[T58] Scala：函数定义
来源：http://fl.nicolike.cn

def add(a: Int, b: Int): Int = a + b
来源：http://tp.haigaiapp.cn

[T59] Scala：循环
来源：http://cw.panjiajie.cn

for (i <- 1 to 10) println(i)
来源：http://xv.jctech888.com.cn

[T60] Scala：折叠
来源：http://ad.wgjwhj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jl.huanxung.cn

================================================================================
来源：http://qo.shtwfgs.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fo.newstarts.cn

================================================================================
来源：http://iw.jctech888.com.cn

[U01] Py：创建虚拟环境
来源：http://px.wgjwhj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://tk.bjjhwx.cn

[U02] Py：导出 / 安装依赖
来源：http://qm.jctech888.com.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cg.wgjwhj.cn

[U03] Py：加载 .env 配置
来源：http://hf.huanxung.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wo.wgjwhj.cn

[U04] Py：变量调试打印
来源：http://ib.hahajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gw.muxihuayi.cn

[U05] Py：列表去重且保序
来源：http://hs.shtwfgs.cn

list(dict.fromkeys(arr))
来源：http://ev.chemitech.net.cn

[U06] Py：合并两个字典
来源：http://dl.wgjwhj.cn

{**a, **b}
来源：http://xq.yuntaijiaju.cn

[U07] Py：反转字典键值
来源：http://mr.muxihuayi.cn

{v: k for k, v in d.items()}
来源：http://zk.nszjky.cn

[U08] Py：展平二维列表
来源：http://vx.nicolike.cn

[y for x in nested for y in x]
来源：http://zr.yuntaijiaju.cn

[U09] Py：字典取最大值的键
来源：http://xx.hahajie.cn

max(d, key=d.get)
来源：http://kc.shxzukj.cn

[U10] Py：按值排序字典
来源：http://uu.huixiangedu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xb.asd995.cn

[U11] Py：生成器表达式
来源：http://al.chemitech.net.cn

(x * 2 for x in arr)
来源：http://pd.gzmigu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lu.muxihuayi.cn

Counter(arr).most_common(3)
来源：http://ss.szxytkj.cn

[U13] Py：固定长度队列
来源：http://xt.wgjwhj.cn

deque(maxlen=10)
来源：http://rl.huanxung.cn

[U14] Py：分组收集到列表
来源：http://cl.haigaiapp.cn

defaultdict(list)
来源：http://mo.yuexingan06.cn

[U15] Py：高精度计时
来源：http://il.nicolike.cn

t = time.perf_counter()
来源：http://fu.wgjwhj.cn

[U16] Py：命令行参数解析
来源：http://od.huixinmuqiang.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zm.gzmigu.cn

[U17] Py：初始化日志
来源：http://lx.hnjuh.cn

logging.basicConfig(level=logging.INFO)
来源：http://zr.lnxyls.cn

[U18] Py：预编译正则
来源：http://jb.jianghongdianzi.cn

pat = re.compile(r"\d+")
来源：http://kn.szxytkj.cn

[U19] Py：正则替换带回调
来源：http://sr.huanxung.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://do.shtwfgs.cn

[U20] Py：缓存函数结果
来源：http://jd.shtwfgs.cn

@functools.lru_cache(maxsize=None)
来源：http://mf.chemitech.net.cn

[U21] Py：自定义上下文管理器
来源：http://pp.hnjuh.cn

@contextlib.contextmanager
来源：http://xc.jianghongdianzi.cn

[U22] Py：矩阵转置
来源：http://jk.hahajie.cn

list(zip(*m))
来源：http://fk.nicolike.cn

[U23] Py：分块读取大文件
来源：http://zu.jctech888.com.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fn.gzmigu.cn

[U24] Py：路径操作
来源：http://mt.chemitech.net.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lx.chemitech.net.cn

[U25] Py：CSV 按字典读
来源：http://uc.shxzskj.cn

csv.DictReader(f)
来源：http://sq.9csxet.cn

[U26] Py：并发下载
来源：http://vw.hnjuh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ko.nicolike.cn

[U27] Py：异步 HTTP
来源：http://nu.gzmigu.cn

aiohttp.ClientSession() 配合 async with
来源：http://uv.shtwfgs.cn

[U28] Py：类型别名
来源：http://tj.jianghongdianzi.cn

UserId = int
来源：http://yt.gzmigu.cn

[U29] Py：属性校验
来源：http://ez.bjjhwx.cn

@property 与 @x.setter 配合
来源：http://sj.huixinmuqiang.cn

[U30] Py：数据类
来源：http://ml.huixiangedu.cn

@dataclass(slots=True)
来源：http://ji.szxytkj.cn

[U31] Py：单测
来源：http://xt.colortex.cn

python -m pytest -q
来源：http://jo.hahajie.cn

[U32] Py：代码格式化
来源：http://us.yuntaijiaju.cn

ruff format . && ruff check --fix .
来源：http://ow.shtwfgs.cn

[U33] Py：打包发布
来源：http://kz.hahajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://le.hahajie.cn

[U34] Py：判断编码
来源：http://rl.haigaiapp.cn

chardet.detect(raw)
来源：http://ru.jctech888.com.cn

[U35] Py：发送邮件
来源：http://ke.huanxung.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ff.chemitech.net.cn

[U36] Py：定时任务
来源：http://rb.wgjwhj.cn

schedule.every(10).minutes.do(job)
来源：http://mz.nicolike.cn

[U37] Py：读写 Excel
来源：http://vv.colortex.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ek.bjjhwx.cn

[U38] Py：获取脚本所在目录
来源：http://en.lnxyls.cn

Path(__file__).resolve().parent
来源：http://ne.panjiajie.cn

[U39] Py：判断是否在交互环境
来源：http://eg.chemitech.net.cn

sys.stdout.isatty()
来源：http://ec.panjiajie.cn

[U40] Py：打印到标准错误
来源：http://dr.jianghongdianzi.cn

print("err", file=sys.stderr)
来源：http://xz.newstarts.cn

[U41] PHP：初始化 Composer 项目
来源：http://je.nszjky.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://kn.hnjuh.cn

[U42] PHP：PSR-4 自动加载
来源：http://cc.wgjwhj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://iv.bookmarksfly.cn

[U43] PHP：声明命名空间
来源：http://sl.wgjwhj.cn

namespace App\Http;
来源：http://ne.panjiajie.cn

[U44] PHP：开启严格类型
来源：http://te.shxzukj.cn

declare(strict_types=1);
来源：http://lw.asd995.cn

[U45] PHP：类型声明与返回类型
来源：http://st.bjjhwx.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://pa.hnjuh.cn

[U46] PHP：可空类型
来源：http://am.colortex.cn

?string $name = null
来源：http://zw.bookmarksfly.cn

[U47] PHP：联合类型
来源：http://ol.jctech888.com.cn

int|string $id
来源：http://iv.jctech888.com.cn

[U48] PHP：纯枚举
来源：http://ty.chemitech.net.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ti.gzmigu.cn

[U49] PHP：只读属性
来源：http://wj.nszjky.cn

public readonly string $name
来源：http://dt.jctech888.com.cn

[U50] PHP：构造器属性提升
来源：http://cx.jianghongdianzi.cn

public function __construct(private int $id) {}
来源：http://sk.huixinmuqiang.cn

[U51] PHP：数组解构
来源：http://rp.szsharing.cn

[$a, $b] = $arr;
来源：http://wq.chemitech.net.cn

[U52] PHP：箭头函数
来源：http://ab.nicolike.cn

$double = fn($x) => $x * 2;
来源：http://sa.szxytkj.cn

[U53] PHP：空合并运算符
来源：http://kq.yuntaijiaju.cn

$v = $a ?? $b ?? "default";
来源：http://mi.nicolike.cn

[U54] PHP：空安全调用
来源：http://nz.chemitech.net.cn

$obj?->method()
来源：http://kp.huanxung.cn

[U55] PHP：match 表达式
来源：http://rb.shxzukj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://sp.lnxyls.cn

[U56] PHP：命名参数
来源：http://fx.yuexingan06.cn

f(a: 1, b: 2)
来源：http://qu.chemitech.net.cn

[U57] PHP：字符串插值
来源：http://nw.jianghongdianzi.cn

"值: {$a}"
来源：http://tz.asd995.cn

[U58] PHP：数组三件套
来源：http://rf.9csxet.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nc.hnjuh.cn

[U59] PHP：自定义排序
来源：http://xk.huixiangedu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mh.bjjhwx.cn

[U60] PHP：JSON 编解码
来源：http://lh.huixinmuqiang.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dc.shtwfgs.cn

[U61] PHP：正则
来源：http://bd.huixiangedu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ot.szxytkj.cn

[U62] PHP：日期对象
来源：http://yl.haigaiapp.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://es.bjjhwx.cn

[U63] PHP：文件读写
来源：http://kn.chemitech.net.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fk.wgjwhj.cn

[U64] PHP：目录遍历
来源：http://xq.bookmarksfly.cn

glob("dir/*.php");  scandir("dir");
来源：http://bw.szsharing.cn

[U65] PHP：会话
来源：http://ji.shtwfgs.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://pp.huixiangedu.cn

[U66] PHP：设置 Cookie
来源：http://dj.9csxet.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sw.shtwfgs.cn

[U67] PHP：处理文件上传
来源：http://ec.huanxung.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yq.chemitech.net.cn

[U68] PHP：PDO 连接
来源：http://fj.colortex.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://aw.huixiangedu.cn

[U69] PHP：PDO 预处理
来源：http://jz.bookmarksfly.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://aa.wgjwhj.cn

[U70] PHP：PDO 事务
来源：http://uk.colortex.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sm.huixinmuqiang.cn

[U71] PHP：抛出异常
来源：http://rz.colortex.cn

throw new RuntimeException("失败", 500);
来源：http://ju.hnjuh.cn

[U72] PHP：写错误日志
来源：http://cp.9csxet.cn

error_log("失败: " . $e->getMessage());
来源：http://vt.jianghongdianzi.cn

[U73] PHP：读取 ini 配置
来源：http://qs.yuexingan06.cn

parse_ini_file("config.ini", true)
来源：http://gn.shxzukj.cn

[U74] PHP：读取环境变量
来源：http://po.chemitech.net.cn

getenv("APP_ENV") ?: "production"
来源：http://yo.huanxung.cn

[U75] PHP：依赖注入
来源：http://em.jianghongdianzi.cn

composer require psr/container
来源：http://tl.newstarts.cn

[U76] PHP：简单路由
来源：http://dz.huixiangedu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jd.newstarts.cn

[U77] PHP：模板渲染
来源：http://qy.huixinmuqiang.cn

composer require twig/twig
来源：http://it.huixinmuqiang.cn

[U78] PHP：单元测试
来源：http://nd.nszjky.cn

composer require --dev phpunit/phpunit
来源：http://wh.bjjhwx.cn

[U79] PHP：静态分析
来源：http://ew.newstarts.cn

composer require --dev phpstan/phpstan
来源：http://br.panjiajie.cn

[U80] PHP：代码规范修复
来源：http://si.nszjky.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://iz.lnxyls.cn


<!-- 参考信息 -->