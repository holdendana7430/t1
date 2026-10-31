代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://oh.shtwfgs.cn

[S55] C++：结构化绑定
来源：http://qm.hahajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ei.muxihuayi.cn

[S56] C++：optional
来源：http://fi.hnjuh.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ex.szsharing.cn

[S57] C++：编译期常量
来源：http://if.yuntaijiaju.cn

constexpr int N = 10;
来源：http://mm.521024.cn

[S58] C++：命名空间
来源：http://yb.chemitech.net.cn

namespace ns { int f() { return 1; } }
来源：http://jo.szxytkj.cn

[S59] C++：静态断言
来源：http://oo.hnjuh.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yg.huixiangedu.cn

[S60] C++：遍历并删除元素
来源：http://ls.shxzukj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://be.9csxet.cn

================================================================================
来源：http://vy.521024.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cu.shtwfgs.cn

================================================================================
来源：http://jn.shtwfgs.cn

[T01] Kotlin：Hello World
来源：http://cw.gzmigu.cn

println("Hello")
来源：http://wx.hahajie.cn

[T02] Kotlin：变量
来源：http://tf.bookmarksfly.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jq.nicolike.cn

[T03] Kotlin：字符串模板
来源：http://xj.huixinmuqiang.cn

"值: $b"
来源：http://ay.huixinmuqiang.cn

[T04] Kotlin：空安全
来源：http://bn.bjjhwx.cn

val n: String? = null;  n?.length
来源：http://wy.huixiangedu.cn

[T05] Kotlin：when 表达式
来源：http://wh.panjiajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jd.gzmigu.cn

[T06] Kotlin：集合映射
来源：http://pj.huixiangedu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ne.huanxung.cn

[T07] Kotlin：集合过滤
来源：http://nn.shxzukj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wd.shtwfgs.cn

[T08] Kotlin：数据类
来源：http://vv.hnjuh.cn

data class User(val name: String, val age: Int)
来源：http://ti.szxytkj.cn

[T09] Kotlin：扩展函数
来源：http://ta.haigaiapp.cn

fun String.exclaim() = this + "!"
来源：http://ig.yuexingan06.cn

[T10] Kotlin：默认参数
来源：http://vo.shtwfgs.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ra.shxzskj.cn

[T11] Kotlin：协程
来源：http://zl.jianghongdianzi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://kx.huixinmuqiang.cn

[T12] Kotlin：解构声明
来源：http://bv.lnxyls.cn

val (a, b) = Pair(1, 2)
来源：http://xc.lnxyls.cn

[T13] Kotlin：只读 Map
来源：http://lr.panjiajie.cn

val m = mapOf("a" to 1)
来源：http://fd.muxihuayi.cn

[T14] Kotlin：循环
来源：http://nr.shxzskj.cn

for (i in 1..10) println(i)
来源：http://gq.jctech888.com.cn

[T15] Kotlin：接口
来源：http://qx.nicolike.cn

interface Shape { fun area(): Double }
来源：http://bj.nszjky.cn

[T16] Swift：Hello World
来源：http://gt.panjiajie.cn

print("Hello")
来源：http://nd.shxzskj.cn

[T17] Swift：变量与常量
来源：http://ow.huanxung.cn

var a = 1;  let b = 2
来源：http://lc.lnxyls.cn

[T18] Swift：字符串插值
来源：http://rj.asd995.cn

"值: \(b)"
来源：http://mf.lnxyls.cn

[T19] Swift：可选绑定
来源：http://ki.shxzskj.cn

if let n = opt { print(n) }
来源：http://ix.bjjhwx.cn

[T20] Swift：数组操作
来源：http://kr.huixinmuqiang.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ep.jianghongdianzi.cn

[T21] Swift：遍历
来源：http://xd.muxihuayi.cn

for x in a { print(x) }
来源：http://rv.hahajie.cn

[T22] Swift：字典
来源：http://gr.jianghongdianzi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zj.haigaiapp.cn

[T23] Swift：函数
来源：http://hr.shxzukj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qh.jianghongdianzi.cn

[T24] Swift：闭包
来源：http://tt.huixinmuqiang.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://nt.9csxet.cn

[T25] Swift：结构体
来源：http://kc.bookmarksfly.cn

struct P { var x: Int }
来源：http://tl.hahajie.cn

[T26] Swift：类与重写
来源：http://bv.shxzskj.cn

class A: Base { override func f() {} }
来源：http://or.yuexingan06.cn

[T27] Swift：错误处理
来源：http://ow.lnxyls.cn

do { try f() } catch { print(error) }
来源：http://mr.nszjky.cn

[T28] Swift：枚举
来源：http://zm.yuntaijiaju.cn

enum Color { case red, green }
来源：http://ya.wgjwhj.cn

[T29] Swift：guard 提前返回
来源：http://wr.hahajie.cn

guard let x = opt else { return }
来源：http://io.521024.cn

[T30] Swift：协议
来源：http://ud.jctech888.com.cn

protocol Shape { func area() -> Double }
来源：http://cr.lnxyls.cn

[T31] Lua：Hello World
来源：http://om.jianghongdianzi.cn

print("Hello")
来源：http://lf.521024.cn

[T32] Lua：局部变量
来源：http://by.bookmarksfly.cn

local a = 1
来源：http://hy.bookmarksfly.cn

[T33] Lua：表（数组）
来源：http://uo.gzmigu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ey.szsharing.cn

[T34] Lua：遍历表
来源：http://ge.shxzskj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ct.521024.cn

[T35] Lua：字典表
来源：http://li.jctech888.com.cn

local d = { a = 1 };  d.b = 2
来源：http://gp.hahajie.cn

[T36] Lua：函数
来源：http://jz.nszjky.cn

function add(a, b) return a + b end
来源：http://rf.huixiangedu.cn

[T37] Lua：字符串拼接
来源：http://xl.haigaiapp.cn

"a" .. "b"
来源：http://bw.lnxyls.cn

[T38] Lua：条件
来源：http://eg.hahajie.cn

if x > 0 then print("正") end
来源：http://iz.bjjhwx.cn

[T39] Lua：模式匹配
来源：http://ys.shtwfgs.cn

string.find(s, "%d+")
来源：http://ap.yuexingan06.cn

[T40] Lua：元表
来源：http://rn.yuntaijiaju.cn

setmetatable({}, { __index = base })
来源：http://dk.muxihuayi.cn

[T41] Perl：Hello World
来源：http://kg.newstarts.cn

print "Hello\n";
来源：http://bk.haigaiapp.cn

[T42] Perl：变量类型
来源：http://oo.yuntaijiaju.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sn.nicolike.cn

[T43] Perl：字符串插值
来源：http://ov.yuexingan06.cn

"值: $a"
来源：http://eh.nicolike.cn

[T44] Perl：条件
来源：http://tq.jctech888.com.cn

if ($a > 0) { print "正"; }
来源：http://of.panjiajie.cn

[T45] Perl：数组遍历
来源：http://rf.nszjky.cn

for my $x (@arr) { print $x; }
来源：http://vl.chemitech.net.cn

[T46] Perl：哈希操作
来源：http://ma.asd995.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://va.huanxung.cn

[T47] Perl：正则捕获
来源：http://wx.huanxung.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://iu.nicolike.cn

[T48] Perl：正则替换
来源：http://az.yuntaijiaju.cn

$s =~ s/old/new/g;
来源：http://kc.9csxet.cn

[T49] Perl：函数
来源：http://pe.shtwfgs.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ds.hahajie.cn

[T50] Perl：逐行读文件
来源：http://ku.bookmarksfly.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://mi.521024.cn

while (my $line = <$fh>) { print $line; }
来源：http://ib.chemitech.net.cn

[T51] Scala：Hello World
来源：http://dr.newstarts.cn

println("Hello")
来源：http://dn.newstarts.cn

[T52] Scala：变量
来源：http://ka.bookmarksfly.cn

val a = 1;  var b = 2
来源：http://px.jianghongdianzi.cn

[T53] Scala：字符串插值
来源：http://dq.hahajie.cn

s"值: $b"
来源：http://rm.gzmigu.cn

[T54] Scala：集合映射
来源：http://sg.huanxung.cn

List(1, 2, 3).map(_ * 2)
来源：http://uv.chemitech.net.cn

[T55] Scala：集合过滤
来源：http://ry.nszjky.cn

List(1, 2, 3).filter(_ > 1)
来源：http://oq.yuexingan06.cn

[T56] Scala：样例类
来源：http://gv.asd995.cn

case class User(name: String, age: Int)
来源：http://xp.521024.cn

[T57] Scala：模式匹配
来源：http://ar.shtwfgs.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://cs.szxytkj.cn

[T58] Scala：函数定义
来源：http://xm.jianghongdianzi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://sf.shxzskj.cn

[T59] Scala：循环
来源：http://cu.wgjwhj.cn

for (i <- 1 to 10) println(i)
来源：http://bm.yuexingan06.cn

[T60] Scala：折叠
来源：http://bm.huixiangedu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://af.colortex.cn

================================================================================
来源：http://zf.haigaiapp.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ps.haigaiapp.cn

================================================================================
来源：http://qw.huixinmuqiang.cn

[U01] Py：创建虚拟环境
来源：http://kg.huixinmuqiang.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cp.jctech888.com.cn

[U02] Py：导出 / 安装依赖
来源：http://lu.hahajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ti.szxytkj.cn

[U03] Py：加载 .env 配置
来源：http://iv.asd995.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ni.shtwfgs.cn

[U04] Py：变量调试打印
来源：http://ir.haigaiapp.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sb.szsharing.cn

[U05] Py：列表去重且保序
来源：http://yn.shxzskj.cn

list(dict.fromkeys(arr))
来源：http://ey.bookmarksfly.cn

[U06] Py：合并两个字典
来源：http://zk.jctech888.com.cn

{**a, **b}
来源：http://hn.nszjky.cn

[U07] Py：反转字典键值
来源：http://qg.521024.cn

{v: k for k, v in d.items()}
来源：http://kq.chemitech.net.cn

[U08] Py：展平二维列表
来源：http://uj.shxzukj.cn

[y for x in nested for y in x]
来源：http://yf.newstarts.cn

[U09] Py：字典取最大值的键
来源：http://ch.huixiangedu.cn

max(d, key=d.get)
来源：http://sn.muxihuayi.cn

[U10] Py：按值排序字典
来源：http://em.shtwfgs.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://by.huixiangedu.cn

[U11] Py：生成器表达式
来源：http://fr.szsharing.cn

(x * 2 for x in arr)
来源：http://fm.shxzskj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://go.asd995.cn

Counter(arr).most_common(3)
来源：http://wp.haigaiapp.cn

[U13] Py：固定长度队列
来源：http://yq.szxytkj.cn

deque(maxlen=10)
来源：http://yj.nicolike.cn

[U14] Py：分组收集到列表
来源：http://kg.yuntaijiaju.cn

defaultdict(list)
来源：http://tg.gzmigu.cn

[U15] Py：高精度计时
来源：http://oo.wgjwhj.cn

t = time.perf_counter()
来源：http://xf.haigaiapp.cn

[U16] Py：命令行参数解析
来源：http://ag.wgjwhj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bg.newstarts.cn

[U17] Py：初始化日志
来源：http://wg.szsharing.cn

logging.basicConfig(level=logging.INFO)
来源：http://kt.gzmigu.cn

[U18] Py：预编译正则
来源：http://nc.gzmigu.cn

pat = re.compile(r"\d+")
来源：http://lw.szxytkj.cn

[U19] Py：正则替换带回调
来源：http://zk.yuexingan06.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mq.newstarts.cn

[U20] Py：缓存函数结果
来源：http://zk.chemitech.net.cn

@functools.lru_cache(maxsize=None)
来源：http://ho.huanxung.cn

[U21] Py：自定义上下文管理器
来源：http://ic.shtwfgs.cn

@contextlib.contextmanager
来源：http://qs.muxihuayi.cn

[U22] Py：矩阵转置
来源：http://xd.huanxung.cn

list(zip(*m))
来源：http://or.huanxung.cn

[U23] Py：分块读取大文件
来源：http://gh.lnxyls.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rx.hahajie.cn

[U24] Py：路径操作
来源：http://te.muxihuayi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fk.shxzukj.cn

[U25] Py：CSV 按字典读
来源：http://to.szsharing.cn

csv.DictReader(f)
来源：http://al.shtwfgs.cn

[U26] Py：并发下载
来源：http://fm.shtwfgs.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://sr.asd995.cn

[U27] Py：异步 HTTP
来源：http://id.521024.cn

aiohttp.ClientSession() 配合 async with
来源：http://js.newstarts.cn

[U28] Py：类型别名
来源：http://pv.shxzskj.cn

UserId = int
来源：http://if.huixiangedu.cn

[U29] Py：属性校验
来源：http://cf.asd995.cn

@property 与 @x.setter 配合
来源：http://fe.wgjwhj.cn

[U30] Py：数据类
来源：http://qk.yuntaijiaju.cn

@dataclass(slots=True)
来源：http://os.lnxyls.cn

[U31] Py：单测
来源：http://pz.asd995.cn

python -m pytest -q
来源：http://lj.chemitech.net.cn

[U32] Py：代码格式化
来源：http://ok.jctech888.com.cn

ruff format . && ruff check --fix .
来源：http://sz.nicolike.cn

[U33] Py：打包发布
来源：http://ju.lnxyls.cn

python -m build  （依赖 pyproject.toml）
来源：http://ct.jctech888.com.cn

[U34] Py：判断编码
来源：http://er.huixiangedu.cn

chardet.detect(raw)
来源：http://oo.haigaiapp.cn

[U35] Py：发送邮件
来源：http://nd.szxytkj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yk.lnxyls.cn

[U36] Py：定时任务
来源：http://fs.hahajie.cn

schedule.every(10).minutes.do(job)
来源：http://sy.colortex.cn

[U37] Py：读写 Excel
来源：http://nu.huanxung.cn

pandas.read_excel / DataFrame.to_excel
来源：http://uz.shxzskj.cn

[U38] Py：获取脚本所在目录
来源：http://eq.huixiangedu.cn

Path(__file__).resolve().parent
来源：http://yr.chemitech.net.cn

[U39] Py：判断是否在交互环境
来源：http://gk.nicolike.cn

sys.stdout.isatty()
来源：http://nw.chemitech.net.cn

[U40] Py：打印到标准错误
来源：http://lk.huanxung.cn

print("err", file=sys.stderr)
来源：http://mp.panjiajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://tj.yuexingan06.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://cy.shxzskj.cn

[U42] PHP：PSR-4 自动加载
来源：http://gx.jctech888.com.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://li.muxihuayi.cn

[U43] PHP：声明命名空间
来源：http://fz.wgjwhj.cn

namespace App\Http;
来源：http://sc.colortex.cn

[U44] PHP：开启严格类型
来源：http://en.haigaiapp.cn

declare(strict_types=1);
来源：http://qc.szxytkj.cn

[U45] PHP：类型声明与返回类型
来源：http://nn.jianghongdianzi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://dr.yuexingan06.cn

[U46] PHP：可空类型
来源：http://hv.bookmarksfly.cn

?string $name = null
来源：http://wd.gzmigu.cn

[U47] PHP：联合类型
来源：http://rx.bjjhwx.cn

int|string $id
来源：http://yb.asd995.cn

[U48] PHP：纯枚举
来源：http://zx.lnxyls.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qc.nicolike.cn

[U49] PHP：只读属性
来源：http://xp.huixinmuqiang.cn

public readonly string $name
来源：http://xs.huixiangedu.cn

[U50] PHP：构造器属性提升
来源：http://jc.yuexingan06.cn

public function __construct(private int $id) {}
来源：http://yv.yuexingan06.cn

[U51] PHP：数组解构
来源：http://mh.nicolike.cn

[$a, $b] = $arr;
来源：http://dy.521024.cn

[U52] PHP：箭头函数
来源：http://lb.wgjwhj.cn

$double = fn($x) => $x * 2;
来源：http://tc.yuntaijiaju.cn

[U53] PHP：空合并运算符
来源：http://gn.521024.cn

$v = $a ?? $b ?? "default";
来源：http://db.panjiajie.cn

[U54] PHP：空安全调用
来源：http://ui.521024.cn

$obj?->method()
来源：http://hp.9csxet.cn

[U55] PHP：match 表达式
来源：http://zi.9csxet.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hh.jianghongdianzi.cn

[U56] PHP：命名参数
来源：http://pf.jianghongdianzi.cn

f(a: 1, b: 2)
来源：http://gp.colortex.cn

[U57] PHP：字符串插值
来源：http://bd.colortex.cn

"值: {$a}"
来源：http://df.huixiangedu.cn

[U58] PHP：数组三件套
来源：http://wq.shxzskj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fb.muxihuayi.cn

[U59] PHP：自定义排序
来源：http://qc.hnjuh.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rp.hahajie.cn

[U60] PHP：JSON 编解码
来源：http://fs.huixinmuqiang.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://se.yuntaijiaju.cn

[U61] PHP：正则
来源：http://do.hahajie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lt.wgjwhj.cn

[U62] PHP：日期对象
来源：http://nl.jctech888.com.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rv.lnxyls.cn

[U63] PHP：文件读写
来源：http://nq.nicolike.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kj.521024.cn

[U64] PHP：目录遍历
来源：http://yg.jianghongdianzi.cn

glob("dir/*.php");  scandir("dir");
来源：http://vs.panjiajie.cn

[U65] PHP：会话
来源：http://vo.huixinmuqiang.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://sl.asd995.cn

[U66] PHP：设置 Cookie
来源：http://zm.colortex.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qd.chemitech.net.cn

[U67] PHP：处理文件上传
来源：http://ez.bjjhwx.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hl.yuexingan06.cn

[U68] PHP：PDO 连接
来源：http://lx.nicolike.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dp.huanxung.cn

[U69] PHP：PDO 预处理
来源：http://rz.huanxung.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xe.gzmigu.cn

[U70] PHP：PDO 事务
来源：http://uc.521024.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hx.hnjuh.cn

[U71] PHP：抛出异常
来源：http://ju.jianghongdianzi.cn

throw new RuntimeException("失败", 500);
来源：http://vv.newstarts.cn

[U72] PHP：写错误日志
来源：http://es.jctech888.com.cn

error_log("失败: " . $e->getMessage());
来源：http://bm.nszjky.cn

[U73] PHP：读取 ini 配置
来源：http://cg.haigaiapp.cn

parse_ini_file("config.ini", true)
来源：http://oy.bookmarksfly.cn

[U74] PHP：读取环境变量
来源：http://ye.nicolike.cn

getenv("APP_ENV") ?: "production"
来源：http://uk.shxzskj.cn

[U75] PHP：依赖注入
来源：http://ww.huixiangedu.cn

composer require psr/container
来源：http://ao.bjjhwx.cn

[U76] PHP：简单路由
来源：http://le.jianghongdianzi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ey.chemitech.net.cn

[U77] PHP：模板渲染
来源：http://dy.jianghongdianzi.cn

composer require twig/twig
来源：http://pz.muxihuayi.cn

[U78] PHP：单元测试
来源：http://ky.hnjuh.cn

composer require --dev phpunit/phpunit
来源：http://pt.muxihuayi.cn

[U79] PHP：静态分析
来源：http://lm.shxzskj.cn

composer require --dev phpstan/phpstan
来源：http://ne.wgjwhj.cn

[U80] PHP：代码规范修复
来源：http://sc.bjjhwx.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://hi.newstarts.cn


<!-- 参考信息 -->