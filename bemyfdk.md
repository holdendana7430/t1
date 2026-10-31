代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yh.shxzukj.cn

[S55] C++：结构化绑定
来源：http://ip.yuexingan06.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qu.huanxung.cn

[S56] C++：optional
来源：http://sc.muxihuayi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wu.shxzukj.cn

[S57] C++：编译期常量
来源：http://pi.jianghongdianzi.cn

constexpr int N = 10;
来源：http://bh.newstarts.cn

[S58] C++：命名空间
来源：http://mx.newstarts.cn

namespace ns { int f() { return 1; } }
来源：http://gx.panjiajie.cn

[S59] C++：静态断言
来源：http://an.hahajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cg.hnjuh.cn

[S60] C++：遍历并删除元素
来源：http://pv.wgjwhj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bh.bookmarksfly.cn

================================================================================
来源：http://fe.9csxet.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vt.chemitech.net.cn

================================================================================
来源：http://yx.szxytkj.cn

[T01] Kotlin：Hello World
来源：http://wi.bjjhwx.cn

println("Hello")
来源：http://he.yuexingan06.cn

[T02] Kotlin：变量
来源：http://oh.yuntaijiaju.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://oc.szxytkj.cn

[T03] Kotlin：字符串模板
来源：http://ff.nicolike.cn

"值: $b"
来源：http://je.huixiangedu.cn

[T04] Kotlin：空安全
来源：http://gm.shtwfgs.cn

val n: String? = null;  n?.length
来源：http://co.huixinmuqiang.cn

[T05] Kotlin：when 表达式
来源：http://sa.hahajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uq.hahajie.cn

[T06] Kotlin：集合映射
来源：http://fw.nszjky.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://qn.bjjhwx.cn

[T07] Kotlin：集合过滤
来源：http://ca.huanxung.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tb.hnjuh.cn

[T08] Kotlin：数据类
来源：http://pz.szsharing.cn

data class User(val name: String, val age: Int)
来源：http://uy.lnxyls.cn

[T09] Kotlin：扩展函数
来源：http://xu.shtwfgs.cn

fun String.exclaim() = this + "!"
来源：http://bl.colortex.cn

[T10] Kotlin：默认参数
来源：http://rv.muxihuayi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://cc.521024.cn

[T11] Kotlin：协程
来源：http://rf.bjjhwx.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wj.huixiangedu.cn

[T12] Kotlin：解构声明
来源：http://ng.huanxung.cn

val (a, b) = Pair(1, 2)
来源：http://dm.gzmigu.cn

[T13] Kotlin：只读 Map
来源：http://vt.colortex.cn

val m = mapOf("a" to 1)
来源：http://re.asd995.cn

[T14] Kotlin：循环
来源：http://jp.shtwfgs.cn

for (i in 1..10) println(i)
来源：http://ck.521024.cn

[T15] Kotlin：接口
来源：http://ah.shxzskj.cn

interface Shape { fun area(): Double }
来源：http://ad.jctech888.com.cn

[T16] Swift：Hello World
来源：http://mf.nszjky.cn

print("Hello")
来源：http://rt.haigaiapp.cn

[T17] Swift：变量与常量
来源：http://bi.chemitech.net.cn

var a = 1;  let b = 2
来源：http://za.haigaiapp.cn

[T18] Swift：字符串插值
来源：http://xg.hahajie.cn

"值: \(b)"
来源：http://ja.hahajie.cn

[T19] Swift：可选绑定
来源：http://pq.521024.cn

if let n = opt { print(n) }
来源：http://yr.bookmarksfly.cn

[T20] Swift：数组操作
来源：http://ka.asd995.cn

var a = [1, 2, 3];  a.append(4)
来源：http://yc.haigaiapp.cn

[T21] Swift：遍历
来源：http://rl.9csxet.cn

for x in a { print(x) }
来源：http://iw.panjiajie.cn

[T22] Swift：字典
来源：http://fe.szsharing.cn

var d = ["a": 1];  d["b"] = 2
来源：http://bs.szsharing.cn

[T23] Swift：函数
来源：http://we.9csxet.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rq.huanxung.cn

[T24] Swift：闭包
来源：http://we.asd995.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gx.huixiangedu.cn

[T25] Swift：结构体
来源：http://ch.gzmigu.cn

struct P { var x: Int }
来源：http://fh.521024.cn

[T26] Swift：类与重写
来源：http://lr.shxzskj.cn

class A: Base { override func f() {} }
来源：http://hp.muxihuayi.cn

[T27] Swift：错误处理
来源：http://iz.nszjky.cn

do { try f() } catch { print(error) }
来源：http://vb.bookmarksfly.cn

[T28] Swift：枚举
来源：http://mp.nicolike.cn

enum Color { case red, green }
来源：http://cr.haigaiapp.cn

[T29] Swift：guard 提前返回
来源：http://mq.hnjuh.cn

guard let x = opt else { return }
来源：http://oj.huanxung.cn

[T30] Swift：协议
来源：http://uq.nicolike.cn

protocol Shape { func area() -> Double }
来源：http://xh.shxzukj.cn

[T31] Lua：Hello World
来源：http://qo.yuexingan06.cn

print("Hello")
来源：http://uv.szxytkj.cn

[T32] Lua：局部变量
来源：http://mj.gzmigu.cn

local a = 1
来源：http://vc.wgjwhj.cn

[T33] Lua：表（数组）
来源：http://zu.gzmigu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://qq.chemitech.net.cn

[T34] Lua：遍历表
来源：http://dp.shxzskj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://no.hnjuh.cn

[T35] Lua：字典表
来源：http://gx.chemitech.net.cn

local d = { a = 1 };  d.b = 2
来源：http://xq.muxihuayi.cn

[T36] Lua：函数
来源：http://pd.panjiajie.cn

function add(a, b) return a + b end
来源：http://bg.bookmarksfly.cn

[T37] Lua：字符串拼接
来源：http://kc.bjjhwx.cn

"a" .. "b"
来源：http://mv.hahajie.cn

[T38] Lua：条件
来源：http://ud.521024.cn

if x > 0 then print("正") end
来源：http://ok.bookmarksfly.cn

[T39] Lua：模式匹配
来源：http://hr.newstarts.cn

string.find(s, "%d+")
来源：http://fn.bjjhwx.cn

[T40] Lua：元表
来源：http://ch.hnjuh.cn

setmetatable({}, { __index = base })
来源：http://jj.jianghongdianzi.cn

[T41] Perl：Hello World
来源：http://at.bookmarksfly.cn

print "Hello\n";
来源：http://pw.chemitech.net.cn

[T42] Perl：变量类型
来源：http://pa.shxzukj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wm.shtwfgs.cn

[T43] Perl：字符串插值
来源：http://lr.nicolike.cn

"值: $a"
来源：http://zu.muxihuayi.cn

[T44] Perl：条件
来源：http://es.nicolike.cn

if ($a > 0) { print "正"; }
来源：http://fm.jctech888.com.cn

[T45] Perl：数组遍历
来源：http://ry.lnxyls.cn

for my $x (@arr) { print $x; }
来源：http://dk.gzmigu.cn

[T46] Perl：哈希操作
来源：http://pm.yuntaijiaju.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ml.szxytkj.cn

[T47] Perl：正则捕获
来源：http://eq.nszjky.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jh.hnjuh.cn

[T48] Perl：正则替换
来源：http://bq.shxzukj.cn

$s =~ s/old/new/g;
来源：http://xr.chemitech.net.cn

[T49] Perl：函数
来源：http://kn.nszjky.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ik.jctech888.com.cn

[T50] Perl：逐行读文件
来源：http://wi.shxzskj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://vm.nszjky.cn

while (my $line = <$fh>) { print $line; }
来源：http://yv.chemitech.net.cn

[T51] Scala：Hello World
来源：http://uo.chemitech.net.cn

println("Hello")
来源：http://ss.szxytkj.cn

[T52] Scala：变量
来源：http://ew.bookmarksfly.cn

val a = 1;  var b = 2
来源：http://pf.muxihuayi.cn

[T53] Scala：字符串插值
来源：http://kj.shxzskj.cn

s"值: $b"
来源：http://gn.yuntaijiaju.cn

[T54] Scala：集合映射
来源：http://kx.asd995.cn

List(1, 2, 3).map(_ * 2)
来源：http://mz.szsharing.cn

[T55] Scala：集合过滤
来源：http://mx.colortex.cn

List(1, 2, 3).filter(_ > 1)
来源：http://bq.shtwfgs.cn

[T56] Scala：样例类
来源：http://as.bookmarksfly.cn

case class User(name: String, age: Int)
来源：http://ig.nicolike.cn

[T57] Scala：模式匹配
来源：http://rq.shxzukj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ze.yuntaijiaju.cn

[T58] Scala：函数定义
来源：http://je.huixinmuqiang.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fq.szxytkj.cn

[T59] Scala：循环
来源：http://fg.hahajie.cn

for (i <- 1 to 10) println(i)
来源：http://fl.9csxet.cn

[T60] Scala：折叠
来源：http://sd.9csxet.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://op.9csxet.cn

================================================================================
来源：http://cr.shxzukj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gh.jianghongdianzi.cn

================================================================================
来源：http://uu.chemitech.net.cn

[U01] Py：创建虚拟环境
来源：http://tv.shxzskj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://fs.521024.cn

[U02] Py：导出 / 安装依赖
来源：http://gt.shtwfgs.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lc.colortex.cn

[U03] Py：加载 .env 配置
来源：http://tj.lnxyls.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://jo.huixiangedu.cn

[U04] Py：变量调试打印
来源：http://bb.haigaiapp.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qn.jctech888.com.cn

[U05] Py：列表去重且保序
来源：http://sh.newstarts.cn

list(dict.fromkeys(arr))
来源：http://me.huanxung.cn

[U06] Py：合并两个字典
来源：http://qf.huixiangedu.cn

{**a, **b}
来源：http://cu.panjiajie.cn

[U07] Py：反转字典键值
来源：http://vz.newstarts.cn

{v: k for k, v in d.items()}
来源：http://sn.nszjky.cn

[U08] Py：展平二维列表
来源：http://nr.yuntaijiaju.cn

[y for x in nested for y in x]
来源：http://xs.huanxung.cn

[U09] Py：字典取最大值的键
来源：http://od.hnjuh.cn

max(d, key=d.get)
来源：http://tn.yuntaijiaju.cn

[U10] Py：按值排序字典
来源：http://yr.9csxet.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dq.colortex.cn

[U11] Py：生成器表达式
来源：http://jz.wgjwhj.cn

(x * 2 for x in arr)
来源：http://qm.panjiajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://yb.wgjwhj.cn

Counter(arr).most_common(3)
来源：http://oh.521024.cn

[U13] Py：固定长度队列
来源：http://zx.shxzukj.cn

deque(maxlen=10)
来源：http://er.muxihuayi.cn

[U14] Py：分组收集到列表
来源：http://vk.panjiajie.cn

defaultdict(list)
来源：http://cc.haigaiapp.cn

[U15] Py：高精度计时
来源：http://do.szsharing.cn

t = time.perf_counter()
来源：http://se.huanxung.cn

[U16] Py：命令行参数解析
来源：http://jl.jctech888.com.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yu.huixinmuqiang.cn

[U17] Py：初始化日志
来源：http://ck.bookmarksfly.cn

logging.basicConfig(level=logging.INFO)
来源：http://nn.colortex.cn

[U18] Py：预编译正则
来源：http://ze.asd995.cn

pat = re.compile(r"\d+")
来源：http://bj.hahajie.cn

[U19] Py：正则替换带回调
来源：http://da.hahajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://en.colortex.cn

[U20] Py：缓存函数结果
来源：http://au.nszjky.cn

@functools.lru_cache(maxsize=None)
来源：http://zd.huanxung.cn

[U21] Py：自定义上下文管理器
来源：http://bq.yuntaijiaju.cn

@contextlib.contextmanager
来源：http://dl.yuntaijiaju.cn

[U22] Py：矩阵转置
来源：http://yf.9csxet.cn

list(zip(*m))
来源：http://oe.nicolike.cn

[U23] Py：分块读取大文件
来源：http://wi.asd995.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://uk.wgjwhj.cn

[U24] Py：路径操作
来源：http://ap.muxihuayi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ch.colortex.cn

[U25] Py：CSV 按字典读
来源：http://zp.colortex.cn

csv.DictReader(f)
来源：http://eu.shxzukj.cn

[U26] Py：并发下载
来源：http://bm.szxytkj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ro.haigaiapp.cn

[U27] Py：异步 HTTP
来源：http://th.asd995.cn

aiohttp.ClientSession() 配合 async with
来源：http://ei.haigaiapp.cn

[U28] Py：类型别名
来源：http://tf.huixiangedu.cn

UserId = int
来源：http://hj.521024.cn

[U29] Py：属性校验
来源：http://le.huixiangedu.cn

@property 与 @x.setter 配合
来源：http://em.nicolike.cn

[U30] Py：数据类
来源：http://du.nicolike.cn

@dataclass(slots=True)
来源：http://iv.yuntaijiaju.cn

[U31] Py：单测
来源：http://wl.shxzukj.cn

python -m pytest -q
来源：http://us.nicolike.cn

[U32] Py：代码格式化
来源：http://tf.haigaiapp.cn

ruff format . && ruff check --fix .
来源：http://iz.muxihuayi.cn

[U33] Py：打包发布
来源：http://ws.huanxung.cn

python -m build  （依赖 pyproject.toml）
来源：http://du.panjiajie.cn

[U34] Py：判断编码
来源：http://pe.panjiajie.cn

chardet.detect(raw)
来源：http://zi.nszjky.cn

[U35] Py：发送邮件
来源：http://cf.shxzukj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wu.huixiangedu.cn

[U36] Py：定时任务
来源：http://oi.szxytkj.cn

schedule.every(10).minutes.do(job)
来源：http://rn.nszjky.cn

[U37] Py：读写 Excel
来源：http://rm.nszjky.cn

pandas.read_excel / DataFrame.to_excel
来源：http://yy.jctech888.com.cn

[U38] Py：获取脚本所在目录
来源：http://gs.colortex.cn

Path(__file__).resolve().parent
来源：http://er.nicolike.cn

[U39] Py：判断是否在交互环境
来源：http://qx.haigaiapp.cn

sys.stdout.isatty()
来源：http://cm.jctech888.com.cn

[U40] Py：打印到标准错误
来源：http://wh.nicolike.cn

print("err", file=sys.stderr)
来源：http://rn.shxzskj.cn

[U41] PHP：初始化 Composer 项目
来源：http://ax.yuntaijiaju.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://cj.jctech888.com.cn

[U42] PHP：PSR-4 自动加载
来源：http://go.shxzskj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pe.colortex.cn

[U43] PHP：声明命名空间
来源：http://cw.huixiangedu.cn

namespace App\Http;
来源：http://bf.shxzskj.cn

[U44] PHP：开启严格类型
来源：http://ik.colortex.cn

declare(strict_types=1);
来源：http://he.nszjky.cn

[U45] PHP：类型声明与返回类型
来源：http://ix.hahajie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://sm.wgjwhj.cn

[U46] PHP：可空类型
来源：http://hz.nicolike.cn

?string $name = null
来源：http://tw.chemitech.net.cn

[U47] PHP：联合类型
来源：http://uz.newstarts.cn

int|string $id
来源：http://eg.chemitech.net.cn

[U48] PHP：纯枚举
来源：http://tq.shxzskj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zy.nszjky.cn

[U49] PHP：只读属性
来源：http://ja.huixiangedu.cn

public readonly string $name
来源：http://zd.nszjky.cn

[U50] PHP：构造器属性提升
来源：http://hd.huixinmuqiang.cn

public function __construct(private int $id) {}
来源：http://hb.chemitech.net.cn

[U51] PHP：数组解构
来源：http://bx.shtwfgs.cn

[$a, $b] = $arr;
来源：http://xn.bookmarksfly.cn

[U52] PHP：箭头函数
来源：http://ew.newstarts.cn

$double = fn($x) => $x * 2;
来源：http://fr.lnxyls.cn

[U53] PHP：空合并运算符
来源：http://gh.yuntaijiaju.cn

$v = $a ?? $b ?? "default";
来源：http://pe.panjiajie.cn

[U54] PHP：空安全调用
来源：http://tx.newstarts.cn

$obj?->method()
来源：http://cf.newstarts.cn

[U55] PHP：match 表达式
来源：http://zp.bjjhwx.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yb.bookmarksfly.cn

[U56] PHP：命名参数
来源：http://no.huanxung.cn

f(a: 1, b: 2)
来源：http://ub.shtwfgs.cn

[U57] PHP：字符串插值
来源：http://da.shtwfgs.cn

"值: {$a}"
来源：http://wc.lnxyls.cn

[U58] PHP：数组三件套
来源：http://qn.shxzskj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ew.wgjwhj.cn

[U59] PHP：自定义排序
来源：http://rp.shxzskj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vy.chemitech.net.cn

[U60] PHP：JSON 编解码
来源：http://it.huixiangedu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://el.jctech888.com.cn

[U61] PHP：正则
来源：http://rq.jctech888.com.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fs.newstarts.cn

[U62] PHP：日期对象
来源：http://if.szsharing.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mw.yuexingan06.cn

[U63] PHP：文件读写
来源：http://lm.yuntaijiaju.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://if.wgjwhj.cn

[U64] PHP：目录遍历
来源：http://fo.shxzskj.cn

glob("dir/*.php");  scandir("dir");
来源：http://vj.gzmigu.cn

[U65] PHP：会话
来源：http://dr.newstarts.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://eu.colortex.cn

[U66] PHP：设置 Cookie
来源：http://wo.chemitech.net.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rl.jctech888.com.cn

[U67] PHP：处理文件上传
来源：http://ww.hahajie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://aj.jctech888.com.cn

[U68] PHP：PDO 连接
来源：http://fg.521024.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qy.huixinmuqiang.cn

[U69] PHP：PDO 预处理
来源：http://ki.yuexingan06.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ri.yuntaijiaju.cn

[U70] PHP：PDO 事务
来源：http://mg.szxytkj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jh.nicolike.cn

[U71] PHP：抛出异常
来源：http://lh.nszjky.cn

throw new RuntimeException("失败", 500);
来源：http://pu.gzmigu.cn

[U72] PHP：写错误日志
来源：http://ax.chemitech.net.cn

error_log("失败: " . $e->getMessage());
来源：http://at.shxzskj.cn

[U73] PHP：读取 ini 配置
来源：http://bt.huixiangedu.cn

parse_ini_file("config.ini", true)
来源：http://tk.muxihuayi.cn

[U74] PHP：读取环境变量
来源：http://rw.huanxung.cn

getenv("APP_ENV") ?: "production"
来源：http://in.huixinmuqiang.cn

[U75] PHP：依赖注入
来源：http://vn.szsharing.cn

composer require psr/container
来源：http://ym.huixinmuqiang.cn

[U76] PHP：简单路由
来源：http://cv.jctech888.com.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qu.nicolike.cn

[U77] PHP：模板渲染
来源：http://vw.asd995.cn

composer require twig/twig
来源：http://ed.haigaiapp.cn

[U78] PHP：单元测试
来源：http://zv.lnxyls.cn

composer require --dev phpunit/phpunit
来源：http://ds.nszjky.cn

[U79] PHP：静态分析
来源：http://zb.panjiajie.cn

composer require --dev phpstan/phpstan
来源：http://hf.shxzskj.cn

[U80] PHP：代码规范修复
来源：http://at.newstarts.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://zk.muxihuayi.cn


<!-- 参考信息 -->