代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://au.haigaiapp.cn

[S55] C++：结构化绑定
来源：http://zj.chemitech.net.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://no.lnxyls.cn

[S56] C++：optional
来源：http://eo.521024.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qf.huixiangedu.cn

[S57] C++：编译期常量
来源：http://ry.lnxyls.cn

constexpr int N = 10;
来源：http://mo.nicolike.cn

[S58] C++：命名空间
来源：http://wh.jctech888.com.cn

namespace ns { int f() { return 1; } }
来源：http://ju.szxytkj.cn

[S59] C++：静态断言
来源：http://qq.gzmigu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hu.9csxet.cn

[S60] C++：遍历并删除元素
来源：http://of.chemitech.net.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sv.yuexingan06.cn

================================================================================
来源：http://gc.huixinmuqiang.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tr.chemitech.net.cn

================================================================================
来源：http://pr.muxihuayi.cn

[T01] Kotlin：Hello World
来源：http://ny.wgjwhj.cn

println("Hello")
来源：http://hz.muxihuayi.cn

[T02] Kotlin：变量
来源：http://rr.wgjwhj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fk.chemitech.net.cn

[T03] Kotlin：字符串模板
来源：http://te.lnxyls.cn

"值: $b"
来源：http://yk.chemitech.net.cn

[T04] Kotlin：空安全
来源：http://ti.panjiajie.cn

val n: String? = null;  n?.length
来源：http://uz.hnjuh.cn

[T05] Kotlin：when 表达式
来源：http://mx.panjiajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ul.panjiajie.cn

[T06] Kotlin：集合映射
来源：http://ec.lnxyls.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://vd.huixiangedu.cn

[T07] Kotlin：集合过滤
来源：http://wh.bookmarksfly.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://km.shxzskj.cn

[T08] Kotlin：数据类
来源：http://dl.bookmarksfly.cn

data class User(val name: String, val age: Int)
来源：http://ou.jianghongdianzi.cn

[T09] Kotlin：扩展函数
来源：http://aq.huanxung.cn

fun String.exclaim() = this + "!"
来源：http://bu.shxzukj.cn

[T10] Kotlin：默认参数
来源：http://ps.bjjhwx.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ia.asd995.cn

[T11] Kotlin：协程
来源：http://px.jctech888.com.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://on.gzmigu.cn

[T12] Kotlin：解构声明
来源：http://zr.nszjky.cn

val (a, b) = Pair(1, 2)
来源：http://yz.chemitech.net.cn

[T13] Kotlin：只读 Map
来源：http://qb.shxzukj.cn

val m = mapOf("a" to 1)
来源：http://up.9csxet.cn

[T14] Kotlin：循环
来源：http://gt.huixinmuqiang.cn

for (i in 1..10) println(i)
来源：http://mr.muxihuayi.cn

[T15] Kotlin：接口
来源：http://cr.szxytkj.cn

interface Shape { fun area(): Double }
来源：http://zo.huixiangedu.cn

[T16] Swift：Hello World
来源：http://or.huixiangedu.cn

print("Hello")
来源：http://ug.bjjhwx.cn

[T17] Swift：变量与常量
来源：http://ve.panjiajie.cn

var a = 1;  let b = 2
来源：http://kc.asd995.cn

[T18] Swift：字符串插值
来源：http://bw.hahajie.cn

"值: \(b)"
来源：http://oe.lnxyls.cn

[T19] Swift：可选绑定
来源：http://mn.521024.cn

if let n = opt { print(n) }
来源：http://mn.szsharing.cn

[T20] Swift：数组操作
来源：http://hp.chemitech.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://yr.yuntaijiaju.cn

[T21] Swift：遍历
来源：http://tg.jctech888.com.cn

for x in a { print(x) }
来源：http://sj.jianghongdianzi.cn

[T22] Swift：字典
来源：http://qa.chemitech.net.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mg.hahajie.cn

[T23] Swift：函数
来源：http://ra.asd995.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lg.huixiangedu.cn

[T24] Swift：闭包
来源：http://jk.lnxyls.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vb.asd995.cn

[T25] Swift：结构体
来源：http://gz.9csxet.cn

struct P { var x: Int }
来源：http://mh.shxzukj.cn

[T26] Swift：类与重写
来源：http://bg.hnjuh.cn

class A: Base { override func f() {} }
来源：http://ar.jctech888.com.cn

[T27] Swift：错误处理
来源：http://ub.panjiajie.cn

do { try f() } catch { print(error) }
来源：http://cr.yuexingan06.cn

[T28] Swift：枚举
来源：http://ux.muxihuayi.cn

enum Color { case red, green }
来源：http://us.hnjuh.cn

[T29] Swift：guard 提前返回
来源：http://oz.huanxung.cn

guard let x = opt else { return }
来源：http://ea.panjiajie.cn

[T30] Swift：协议
来源：http://gm.panjiajie.cn

protocol Shape { func area() -> Double }
来源：http://po.lnxyls.cn

[T31] Lua：Hello World
来源：http://vf.chemitech.net.cn

print("Hello")
来源：http://ls.colortex.cn

[T32] Lua：局部变量
来源：http://ua.nicolike.cn

local a = 1
来源：http://zs.9csxet.cn

[T33] Lua：表（数组）
来源：http://gq.shxzskj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://tp.nszjky.cn

[T34] Lua：遍历表
来源：http://ye.nicolike.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://mc.shxzskj.cn

[T35] Lua：字典表
来源：http://ga.bookmarksfly.cn

local d = { a = 1 };  d.b = 2
来源：http://gd.shxzukj.cn

[T36] Lua：函数
来源：http://ll.jianghongdianzi.cn

function add(a, b) return a + b end
来源：http://hr.newstarts.cn

[T37] Lua：字符串拼接
来源：http://pm.chemitech.net.cn

"a" .. "b"
来源：http://zp.yuexingan06.cn

[T38] Lua：条件
来源：http://jj.szsharing.cn

if x > 0 then print("正") end
来源：http://bi.shxzskj.cn

[T39] Lua：模式匹配
来源：http://aj.hahajie.cn

string.find(s, "%d+")
来源：http://qm.huanxung.cn

[T40] Lua：元表
来源：http://mo.wgjwhj.cn

setmetatable({}, { __index = base })
来源：http://bf.jctech888.com.cn

[T41] Perl：Hello World
来源：http://bi.asd995.cn

print "Hello\n";
来源：http://xc.chemitech.net.cn

[T42] Perl：变量类型
来源：http://xv.nszjky.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hf.newstarts.cn

[T43] Perl：字符串插值
来源：http://cd.jctech888.com.cn

"值: $a"
来源：http://ox.nszjky.cn

[T44] Perl：条件
来源：http://sh.yuntaijiaju.cn

if ($a > 0) { print "正"; }
来源：http://oi.jctech888.com.cn

[T45] Perl：数组遍历
来源：http://hk.huixinmuqiang.cn

for my $x (@arr) { print $x; }
来源：http://wn.hahajie.cn

[T46] Perl：哈希操作
来源：http://nk.szsharing.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qj.nszjky.cn

[T47] Perl：正则捕获
来源：http://ju.bjjhwx.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ju.shxzukj.cn

[T48] Perl：正则替换
来源：http://mb.yuexingan06.cn

$s =~ s/old/new/g;
来源：http://hm.wgjwhj.cn

[T49] Perl：函数
来源：http://yn.chemitech.net.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mw.wgjwhj.cn

[T50] Perl：逐行读文件
来源：http://yf.haigaiapp.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zd.9csxet.cn

while (my $line = <$fh>) { print $line; }
来源：http://rl.hahajie.cn

[T51] Scala：Hello World
来源：http://tg.shtwfgs.cn

println("Hello")
来源：http://ab.521024.cn

[T52] Scala：变量
来源：http://yl.jctech888.com.cn

val a = 1;  var b = 2
来源：http://om.newstarts.cn

[T53] Scala：字符串插值
来源：http://ew.nicolike.cn

s"值: $b"
来源：http://el.hnjuh.cn

[T54] Scala：集合映射
来源：http://jr.yuexingan06.cn

List(1, 2, 3).map(_ * 2)
来源：http://gq.nszjky.cn

[T55] Scala：集合过滤
来源：http://zs.bookmarksfly.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xo.hnjuh.cn

[T56] Scala：样例类
来源：http://nr.yuntaijiaju.cn

case class User(name: String, age: Int)
来源：http://si.jctech888.com.cn

[T57] Scala：模式匹配
来源：http://pf.nszjky.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ie.szsharing.cn

[T58] Scala：函数定义
来源：http://rt.muxihuayi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wc.jianghongdianzi.cn

[T59] Scala：循环
来源：http://lp.panjiajie.cn

for (i <- 1 to 10) println(i)
来源：http://ne.shxzskj.cn

[T60] Scala：折叠
来源：http://iw.9csxet.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ed.hnjuh.cn

================================================================================
来源：http://ha.nicolike.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://en.521024.cn

================================================================================
来源：http://ws.yuntaijiaju.cn

[U01] Py：创建虚拟环境
来源：http://zw.shtwfgs.cn

python -m venv .venv && source .venv/bin/activate
来源：http://og.newstarts.cn

[U02] Py：导出 / 安装依赖
来源：http://kx.521024.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ul.hahajie.cn

[U03] Py：加载 .env 配置
来源：http://iz.nszjky.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://cm.asd995.cn

[U04] Py：变量调试打印
来源：http://rs.chemitech.net.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vc.newstarts.cn

[U05] Py：列表去重且保序
来源：http://en.shtwfgs.cn

list(dict.fromkeys(arr))
来源：http://ll.gzmigu.cn

[U06] Py：合并两个字典
来源：http://ep.9csxet.cn

{**a, **b}
来源：http://vz.colortex.cn

[U07] Py：反转字典键值
来源：http://ri.szsharing.cn

{v: k for k, v in d.items()}
来源：http://nd.colortex.cn

[U08] Py：展平二维列表
来源：http://ws.huanxung.cn

[y for x in nested for y in x]
来源：http://qz.jianghongdianzi.cn

[U09] Py：字典取最大值的键
来源：http://yp.szsharing.cn

max(d, key=d.get)
来源：http://lp.nicolike.cn

[U10] Py：按值排序字典
来源：http://vi.szxytkj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ts.colortex.cn

[U11] Py：生成器表达式
来源：http://qu.nicolike.cn

(x * 2 for x in arr)
来源：http://mi.shxzskj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ad.newstarts.cn

Counter(arr).most_common(3)
来源：http://gg.9csxet.cn

[U13] Py：固定长度队列
来源：http://ae.lnxyls.cn

deque(maxlen=10)
来源：http://jl.jianghongdianzi.cn

[U14] Py：分组收集到列表
来源：http://qp.szsharing.cn

defaultdict(list)
来源：http://my.shxzukj.cn

[U15] Py：高精度计时
来源：http://pp.nszjky.cn

t = time.perf_counter()
来源：http://hk.newstarts.cn

[U16] Py：命令行参数解析
来源：http://fu.shxzukj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xz.colortex.cn

[U17] Py：初始化日志
来源：http://yx.huixinmuqiang.cn

logging.basicConfig(level=logging.INFO)
来源：http://ke.panjiajie.cn

[U18] Py：预编译正则
来源：http://na.bjjhwx.cn

pat = re.compile(r"\d+")
来源：http://jf.nszjky.cn

[U19] Py：正则替换带回调
来源：http://vx.jianghongdianzi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yx.wgjwhj.cn

[U20] Py：缓存函数结果
来源：http://zt.lnxyls.cn

@functools.lru_cache(maxsize=None)
来源：http://wq.bjjhwx.cn

[U21] Py：自定义上下文管理器
来源：http://lx.huanxung.cn

@contextlib.contextmanager
来源：http://cv.szsharing.cn

[U22] Py：矩阵转置
来源：http://ux.shxzukj.cn

list(zip(*m))
来源：http://bf.asd995.cn

[U23] Py：分块读取大文件
来源：http://hr.shxzskj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cy.chemitech.net.cn

[U24] Py：路径操作
来源：http://st.shxzskj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yc.nszjky.cn

[U25] Py：CSV 按字典读
来源：http://tk.asd995.cn

csv.DictReader(f)
来源：http://ro.haigaiapp.cn

[U26] Py：并发下载
来源：http://ri.bjjhwx.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ap.nicolike.cn

[U27] Py：异步 HTTP
来源：http://pd.lnxyls.cn

aiohttp.ClientSession() 配合 async with
来源：http://vc.huixinmuqiang.cn

[U28] Py：类型别名
来源：http://rf.lnxyls.cn

UserId = int
来源：http://da.huixiangedu.cn

[U29] Py：属性校验
来源：http://wk.shxzskj.cn

@property 与 @x.setter 配合
来源：http://oa.wgjwhj.cn

[U30] Py：数据类
来源：http://jb.shxzskj.cn

@dataclass(slots=True)
来源：http://yl.gzmigu.cn

[U31] Py：单测
来源：http://dc.jctech888.com.cn

python -m pytest -q
来源：http://sk.szsharing.cn

[U32] Py：代码格式化
来源：http://eo.hnjuh.cn

ruff format . && ruff check --fix .
来源：http://tp.huanxung.cn

[U33] Py：打包发布
来源：http://qh.colortex.cn

python -m build  （依赖 pyproject.toml）
来源：http://oa.panjiajie.cn

[U34] Py：判断编码
来源：http://nw.hahajie.cn

chardet.detect(raw)
来源：http://fl.shtwfgs.cn

[U35] Py：发送邮件
来源：http://qg.hnjuh.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://no.jianghongdianzi.cn

[U36] Py：定时任务
来源：http://ts.haigaiapp.cn

schedule.every(10).minutes.do(job)
来源：http://gb.haigaiapp.cn

[U37] Py：读写 Excel
来源：http://kn.muxihuayi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://pc.lnxyls.cn

[U38] Py：获取脚本所在目录
来源：http://qw.9csxet.cn

Path(__file__).resolve().parent
来源：http://ln.bjjhwx.cn

[U39] Py：判断是否在交互环境
来源：http://be.hahajie.cn

sys.stdout.isatty()
来源：http://jb.bookmarksfly.cn

[U40] Py：打印到标准错误
来源：http://zj.bjjhwx.cn

print("err", file=sys.stderr)
来源：http://lt.shxzskj.cn

[U41] PHP：初始化 Composer 项目
来源：http://dj.hnjuh.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://km.hnjuh.cn

[U42] PHP：PSR-4 自动加载
来源：http://sa.szsharing.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vm.hahajie.cn

[U43] PHP：声明命名空间
来源：http://lr.lnxyls.cn

namespace App\Http;
来源：http://tq.hnjuh.cn

[U44] PHP：开启严格类型
来源：http://zj.hahajie.cn

declare(strict_types=1);
来源：http://gz.shtwfgs.cn

[U45] PHP：类型声明与返回类型
来源：http://sr.hnjuh.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://pi.yuexingan06.cn

[U46] PHP：可空类型
来源：http://rp.gzmigu.cn

?string $name = null
来源：http://uw.hnjuh.cn

[U47] PHP：联合类型
来源：http://ek.nicolike.cn

int|string $id
来源：http://vn.wgjwhj.cn

[U48] PHP：纯枚举
来源：http://py.shxzukj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sm.hahajie.cn

[U49] PHP：只读属性
来源：http://ku.bookmarksfly.cn

public readonly string $name
来源：http://uc.huanxung.cn

[U50] PHP：构造器属性提升
来源：http://ng.yuexingan06.cn

public function __construct(private int $id) {}
来源：http://fi.szsharing.cn

[U51] PHP：数组解构
来源：http://do.bookmarksfly.cn

[$a, $b] = $arr;
来源：http://gc.nszjky.cn

[U52] PHP：箭头函数
来源：http://xj.nszjky.cn

$double = fn($x) => $x * 2;
来源：http://zy.hnjuh.cn

[U53] PHP：空合并运算符
来源：http://le.lnxyls.cn

$v = $a ?? $b ?? "default";
来源：http://uh.jctech888.com.cn

[U54] PHP：空安全调用
来源：http://fq.shtwfgs.cn

$obj?->method()
来源：http://mx.chemitech.net.cn

[U55] PHP：match 表达式
来源：http://ow.hahajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bx.huixiangedu.cn

[U56] PHP：命名参数
来源：http://ml.jctech888.com.cn

f(a: 1, b: 2)
来源：http://tr.hnjuh.cn

[U57] PHP：字符串插值
来源：http://xx.asd995.cn

"值: {$a}"
来源：http://cp.wgjwhj.cn

[U58] PHP：数组三件套
来源：http://jw.szxytkj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qa.nszjky.cn

[U59] PHP：自定义排序
来源：http://or.shxzukj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ra.colortex.cn

[U60] PHP：JSON 编解码
来源：http://re.9csxet.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kv.nszjky.cn

[U61] PHP：正则
来源：http://sp.yuntaijiaju.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bz.chemitech.net.cn

[U62] PHP：日期对象
来源：http://ct.shxzukj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kz.yuexingan06.cn

[U63] PHP：文件读写
来源：http://dz.gzmigu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sj.colortex.cn

[U64] PHP：目录遍历
来源：http://yo.bookmarksfly.cn

glob("dir/*.php");  scandir("dir");
来源：http://nr.colortex.cn

[U65] PHP：会话
来源：http://tv.newstarts.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://uw.bookmarksfly.cn

[U66] PHP：设置 Cookie
来源：http://jx.jctech888.com.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rz.bookmarksfly.cn

[U67] PHP：处理文件上传
来源：http://if.shtwfgs.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wx.nszjky.cn

[U68] PHP：PDO 连接
来源：http://nb.gzmigu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gb.nicolike.cn

[U69] PHP：PDO 预处理
来源：http://hq.szxytkj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jy.bookmarksfly.cn

[U70] PHP：PDO 事务
来源：http://xc.jianghongdianzi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rn.gzmigu.cn

[U71] PHP：抛出异常
来源：http://xf.newstarts.cn

throw new RuntimeException("失败", 500);
来源：http://at.szsharing.cn

[U72] PHP：写错误日志
来源：http://ut.shtwfgs.cn

error_log("失败: " . $e->getMessage());
来源：http://li.jianghongdianzi.cn

[U73] PHP：读取 ini 配置
来源：http://te.wgjwhj.cn

parse_ini_file("config.ini", true)
来源：http://gh.shxzskj.cn

[U74] PHP：读取环境变量
来源：http://kp.szxytkj.cn

getenv("APP_ENV") ?: "production"
来源：http://fg.shtwfgs.cn

[U75] PHP：依赖注入
来源：http://fk.hnjuh.cn

composer require psr/container
来源：http://fo.lnxyls.cn

[U76] PHP：简单路由
来源：http://bi.shxzukj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kz.szxytkj.cn

[U77] PHP：模板渲染
来源：http://vc.asd995.cn

composer require twig/twig
来源：http://bp.newstarts.cn

[U78] PHP：单元测试
来源：http://fm.nicolike.cn

composer require --dev phpunit/phpunit
来源：http://dc.shxzukj.cn

[U79] PHP：静态分析
来源：http://gt.huanxung.cn

composer require --dev phpstan/phpstan
来源：http://pg.gzmigu.cn

[U80] PHP：代码规范修复
来源：http://hl.bjjhwx.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ie.shxzukj.cn


<!-- 参考信息 -->