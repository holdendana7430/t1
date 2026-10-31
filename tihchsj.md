代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://ju.521024.cn

[S59] C++：静态断言
来源：http://zo.panjiajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vt.asd995.cn

[S60] C++：遍历并删除元素
来源：http://yn.shxzskj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qd.szxytkj.cn

================================================================================
来源：http://ur.521024.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://au.newstarts.cn

================================================================================
来源：http://ag.hahajie.cn

[T01] Kotlin：Hello World
来源：http://ya.yuntaijiaju.cn

println("Hello")
来源：http://dl.jianghongdianzi.cn

[T02] Kotlin：变量
来源：http://eb.9csxet.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sx.szxytkj.cn

[T03] Kotlin：字符串模板
来源：http://to.muxihuayi.cn

"值: $b"
来源：http://yu.huixiangedu.cn

[T04] Kotlin：空安全
来源：http://pu.yuntaijiaju.cn

val n: String? = null;  n?.length
来源：http://ri.gzmigu.cn

[T05] Kotlin：when 表达式
来源：http://pk.jctech888.com.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kw.huanxung.cn

[T06] Kotlin：集合映射
来源：http://xq.yuexingan06.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hf.lnxyls.cn

[T07] Kotlin：集合过滤
来源：http://nw.gzmigu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pu.asd995.cn

[T08] Kotlin：数据类
来源：http://lr.jianghongdianzi.cn

data class User(val name: String, val age: Int)
来源：http://ie.wgjwhj.cn

[T09] Kotlin：扩展函数
来源：http://qe.huanxung.cn

fun String.exclaim() = this + "!"
来源：http://vb.bjjhwx.cn

[T10] Kotlin：默认参数
来源：http://pb.bjjhwx.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://mq.hahajie.cn

[T11] Kotlin：协程
来源：http://bu.newstarts.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xh.huixiangedu.cn

[T12] Kotlin：解构声明
来源：http://ck.muxihuayi.cn

val (a, b) = Pair(1, 2)
来源：http://tj.521024.cn

[T13] Kotlin：只读 Map
来源：http://mi.szsharing.cn

val m = mapOf("a" to 1)
来源：http://lc.9csxet.cn

[T14] Kotlin：循环
来源：http://ny.huixiangedu.cn

for (i in 1..10) println(i)
来源：http://jv.huixinmuqiang.cn

[T15] Kotlin：接口
来源：http://al.hahajie.cn

interface Shape { fun area(): Double }
来源：http://vw.bookmarksfly.cn

[T16] Swift：Hello World
来源：http://ti.hnjuh.cn

print("Hello")
来源：http://ix.jianghongdianzi.cn

[T17] Swift：变量与常量
来源：http://jp.yuexingan06.cn

var a = 1;  let b = 2
来源：http://pb.shxzukj.cn

[T18] Swift：字符串插值
来源：http://vt.9csxet.cn

"值: \(b)"
来源：http://ot.9csxet.cn

[T19] Swift：可选绑定
来源：http://si.521024.cn

if let n = opt { print(n) }
来源：http://lg.panjiajie.cn

[T20] Swift：数组操作
来源：http://wg.521024.cn

var a = [1, 2, 3];  a.append(4)
来源：http://bm.bookmarksfly.cn

[T21] Swift：遍历
来源：http://fo.nicolike.cn

for x in a { print(x) }
来源：http://os.hnjuh.cn

[T22] Swift：字典
来源：http://rv.yuexingan06.cn

var d = ["a": 1];  d["b"] = 2
来源：http://nj.hnjuh.cn

[T23] Swift：函数
来源：http://qb.huanxung.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jw.9csxet.cn

[T24] Swift：闭包
来源：http://xd.yuexingan06.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vh.nicolike.cn

[T25] Swift：结构体
来源：http://op.huixiangedu.cn

struct P { var x: Int }
来源：http://ia.bookmarksfly.cn

[T26] Swift：类与重写
来源：http://fp.gzmigu.cn

class A: Base { override func f() {} }
来源：http://mu.jianghongdianzi.cn

[T27] Swift：错误处理
来源：http://xs.gzmigu.cn

do { try f() } catch { print(error) }
来源：http://yi.shxzskj.cn

[T28] Swift：枚举
来源：http://ci.yuexingan06.cn

enum Color { case red, green }
来源：http://sy.asd995.cn

[T29] Swift：guard 提前返回
来源：http://gq.jctech888.com.cn

guard let x = opt else { return }
来源：http://gy.panjiajie.cn

[T30] Swift：协议
来源：http://in.bookmarksfly.cn

protocol Shape { func area() -> Double }
来源：http://oy.newstarts.cn

[T31] Lua：Hello World
来源：http://wl.shxzukj.cn

print("Hello")
来源：http://fx.shxzukj.cn

[T32] Lua：局部变量
来源：http://el.9csxet.cn

local a = 1
来源：http://wy.gzmigu.cn

[T33] Lua：表（数组）
来源：http://dp.huanxung.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ex.9csxet.cn

[T34] Lua：遍历表
来源：http://tl.szsharing.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://sv.jctech888.com.cn

[T35] Lua：字典表
来源：http://gn.bookmarksfly.cn

local d = { a = 1 };  d.b = 2
来源：http://mg.szxytkj.cn

[T36] Lua：函数
来源：http://xs.newstarts.cn

function add(a, b) return a + b end
来源：http://fs.nicolike.cn

[T37] Lua：字符串拼接
来源：http://wh.yuntaijiaju.cn

"a" .. "b"
来源：http://tt.panjiajie.cn

[T38] Lua：条件
来源：http://pl.hahajie.cn

if x > 0 then print("正") end
来源：http://wb.9csxet.cn

[T39] Lua：模式匹配
来源：http://va.521024.cn

string.find(s, "%d+")
来源：http://wx.asd995.cn

[T40] Lua：元表
来源：http://ek.chemitech.net.cn

setmetatable({}, { __index = base })
来源：http://ly.asd995.cn

[T41] Perl：Hello World
来源：http://hq.hnjuh.cn

print "Hello\n";
来源：http://gj.chemitech.net.cn

[T42] Perl：变量类型
来源：http://ml.szsharing.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yo.wgjwhj.cn

[T43] Perl：字符串插值
来源：http://gr.yuntaijiaju.cn

"值: $a"
来源：http://rh.newstarts.cn

[T44] Perl：条件
来源：http://cc.yuntaijiaju.cn

if ($a > 0) { print "正"; }
来源：http://dm.nszjky.cn

[T45] Perl：数组遍历
来源：http://oq.shxzukj.cn

for my $x (@arr) { print $x; }
来源：http://ua.huanxung.cn

[T46] Perl：哈希操作
来源：http://gs.huixinmuqiang.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uh.bookmarksfly.cn

[T47] Perl：正则捕获
来源：http://ve.gzmigu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://eb.newstarts.cn

[T48] Perl：正则替换
来源：http://dh.panjiajie.cn

$s =~ s/old/new/g;
来源：http://fw.huanxung.cn

[T49] Perl：函数
来源：http://om.newstarts.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wk.panjiajie.cn

[T50] Perl：逐行读文件
来源：http://yr.panjiajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://yl.9csxet.cn

while (my $line = <$fh>) { print $line; }
来源：http://zg.szxytkj.cn

[T51] Scala：Hello World
来源：http://jh.panjiajie.cn

println("Hello")
来源：http://td.gzmigu.cn

[T52] Scala：变量
来源：http://vm.nszjky.cn

val a = 1;  var b = 2
来源：http://oy.haigaiapp.cn

[T53] Scala：字符串插值
来源：http://zk.521024.cn

s"值: $b"
来源：http://kc.yuntaijiaju.cn

[T54] Scala：集合映射
来源：http://ja.colortex.cn

List(1, 2, 3).map(_ * 2)
来源：http://dm.szxytkj.cn

[T55] Scala：集合过滤
来源：http://rb.hahajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://nn.jctech888.com.cn

[T56] Scala：样例类
来源：http://rd.shxzukj.cn

case class User(name: String, age: Int)
来源：http://ct.yuexingan06.cn

[T57] Scala：模式匹配
来源：http://lc.lnxyls.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wt.521024.cn

[T58] Scala：函数定义
来源：http://md.yuntaijiaju.cn

def add(a: Int, b: Int): Int = a + b
来源：http://jv.szsharing.cn

[T59] Scala：循环
来源：http://wq.nszjky.cn

for (i <- 1 to 10) println(i)
来源：http://vx.colortex.cn

[T60] Scala：折叠
来源：http://yv.huixiangedu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ul.huixinmuqiang.cn

================================================================================
来源：http://bq.lnxyls.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://od.huanxung.cn

================================================================================
来源：http://wl.muxihuayi.cn

[U01] Py：创建虚拟环境
来源：http://hj.huixinmuqiang.cn

python -m venv .venv && source .venv/bin/activate
来源：http://gn.shxzukj.cn

[U02] Py：导出 / 安装依赖
来源：http://yh.haigaiapp.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yp.jianghongdianzi.cn

[U03] Py：加载 .env 配置
来源：http://wk.nszjky.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zm.lnxyls.cn

[U04] Py：变量调试打印
来源：http://db.panjiajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fo.szxytkj.cn

[U05] Py：列表去重且保序
来源：http://sx.yuntaijiaju.cn

list(dict.fromkeys(arr))
来源：http://ky.bjjhwx.cn

[U06] Py：合并两个字典
来源：http://xh.szxytkj.cn

{**a, **b}
来源：http://dh.szxytkj.cn

[U07] Py：反转字典键值
来源：http://od.chemitech.net.cn

{v: k for k, v in d.items()}
来源：http://xf.9csxet.cn

[U08] Py：展平二维列表
来源：http://wh.bjjhwx.cn

[y for x in nested for y in x]
来源：http://bi.muxihuayi.cn

[U09] Py：字典取最大值的键
来源：http://is.lnxyls.cn

max(d, key=d.get)
来源：http://hd.szxytkj.cn

[U10] Py：按值排序字典
来源：http://hc.9csxet.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wb.gzmigu.cn

[U11] Py：生成器表达式
来源：http://cs.lnxyls.cn

(x * 2 for x in arr)
来源：http://qn.shxzukj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://hz.lnxyls.cn

Counter(arr).most_common(3)
来源：http://kt.nicolike.cn

[U13] Py：固定长度队列
来源：http://uo.shxzskj.cn

deque(maxlen=10)
来源：http://bn.bjjhwx.cn

[U14] Py：分组收集到列表
来源：http://ig.lnxyls.cn

defaultdict(list)
来源：http://ft.yuntaijiaju.cn

[U15] Py：高精度计时
来源：http://ub.colortex.cn

t = time.perf_counter()
来源：http://fs.huixiangedu.cn

[U16] Py：命令行参数解析
来源：http://lr.panjiajie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://no.wgjwhj.cn

[U17] Py：初始化日志
来源：http://bg.hnjuh.cn

logging.basicConfig(level=logging.INFO)
来源：http://km.yuexingan06.cn

[U18] Py：预编译正则
来源：http://ls.9csxet.cn

pat = re.compile(r"\d+")
来源：http://ic.huixiangedu.cn

[U19] Py：正则替换带回调
来源：http://nx.yuexingan06.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gk.lnxyls.cn

[U20] Py：缓存函数结果
来源：http://et.newstarts.cn

@functools.lru_cache(maxsize=None)
来源：http://xt.nszjky.cn

[U21] Py：自定义上下文管理器
来源：http://hf.chemitech.net.cn

@contextlib.contextmanager
来源：http://sp.yuexingan06.cn

[U22] Py：矩阵转置
来源：http://db.nszjky.cn

list(zip(*m))
来源：http://we.yuexingan06.cn

[U23] Py：分块读取大文件
来源：http://se.newstarts.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ir.chemitech.net.cn

[U24] Py：路径操作
来源：http://zg.asd995.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pt.shtwfgs.cn

[U25] Py：CSV 按字典读
来源：http://vo.muxihuayi.cn

csv.DictReader(f)
来源：http://jy.521024.cn

[U26] Py：并发下载
来源：http://zz.huixinmuqiang.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://if.shxzukj.cn

[U27] Py：异步 HTTP
来源：http://iy.shxzskj.cn

aiohttp.ClientSession() 配合 async with
来源：http://rf.huixinmuqiang.cn

[U28] Py：类型别名
来源：http://dv.wgjwhj.cn

UserId = int
来源：http://cm.shtwfgs.cn

[U29] Py：属性校验
来源：http://fw.bjjhwx.cn

@property 与 @x.setter 配合
来源：http://nk.9csxet.cn

[U30] Py：数据类
来源：http://ql.panjiajie.cn

@dataclass(slots=True)
来源：http://nf.yuexingan06.cn

[U31] Py：单测
来源：http://pk.panjiajie.cn

python -m pytest -q
来源：http://na.wgjwhj.cn

[U32] Py：代码格式化
来源：http://tc.colortex.cn

ruff format . && ruff check --fix .
来源：http://dp.muxihuayi.cn

[U33] Py：打包发布
来源：http://ie.muxihuayi.cn

python -m build  （依赖 pyproject.toml）
来源：http://mp.wgjwhj.cn

[U34] Py：判断编码
来源：http://il.bjjhwx.cn

chardet.detect(raw)
来源：http://zw.wgjwhj.cn

[U35] Py：发送邮件
来源：http://ex.shtwfgs.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qr.panjiajie.cn

[U36] Py：定时任务
来源：http://vb.hnjuh.cn

schedule.every(10).minutes.do(job)
来源：http://ry.hahajie.cn

[U37] Py：读写 Excel
来源：http://mz.wgjwhj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://en.nicolike.cn

[U38] Py：获取脚本所在目录
来源：http://af.muxihuayi.cn

Path(__file__).resolve().parent
来源：http://zo.shtwfgs.cn

[U39] Py：判断是否在交互环境
来源：http://qz.newstarts.cn

sys.stdout.isatty()
来源：http://kj.hnjuh.cn

[U40] Py：打印到标准错误
来源：http://vh.shtwfgs.cn

print("err", file=sys.stderr)
来源：http://th.lnxyls.cn

[U41] PHP：初始化 Composer 项目
来源：http://eb.yuexingan06.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://kx.huixinmuqiang.cn

[U42] PHP：PSR-4 自动加载
来源：http://gj.521024.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sr.yuntaijiaju.cn

[U43] PHP：声明命名空间
来源：http://kn.muxihuayi.cn

namespace App\Http;
来源：http://zs.bjjhwx.cn

[U44] PHP：开启严格类型
来源：http://zw.huixiangedu.cn

declare(strict_types=1);
来源：http://fk.hnjuh.cn

[U45] PHP：类型声明与返回类型
来源：http://qv.yuntaijiaju.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://xn.jctech888.com.cn

[U46] PHP：可空类型
来源：http://jc.9csxet.cn

?string $name = null
来源：http://zk.jianghongdianzi.cn

[U47] PHP：联合类型
来源：http://sn.haigaiapp.cn

int|string $id
来源：http://im.shxzskj.cn

[U48] PHP：纯枚举
来源：http://ol.shxzskj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ln.521024.cn

[U49] PHP：只读属性
来源：http://iy.bjjhwx.cn

public readonly string $name
来源：http://jv.9csxet.cn

[U50] PHP：构造器属性提升
来源：http://jd.szsharing.cn

public function __construct(private int $id) {}
来源：http://lc.521024.cn

[U51] PHP：数组解构
来源：http://jc.haigaiapp.cn

[$a, $b] = $arr;
来源：http://pa.hahajie.cn

[U52] PHP：箭头函数
来源：http://hn.yuntaijiaju.cn

$double = fn($x) => $x * 2;
来源：http://uj.bookmarksfly.cn

[U53] PHP：空合并运算符
来源：http://xw.szxytkj.cn

$v = $a ?? $b ?? "default";
来源：http://sa.shxzskj.cn

[U54] PHP：空安全调用
来源：http://mu.huixinmuqiang.cn

$obj?->method()
来源：http://jm.asd995.cn

[U55] PHP：match 表达式
来源：http://ta.jctech888.com.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://de.yuntaijiaju.cn

[U56] PHP：命名参数
来源：http://jv.asd995.cn

f(a: 1, b: 2)
来源：http://sz.yuexingan06.cn

[U57] PHP：字符串插值
来源：http://js.hnjuh.cn

"值: {$a}"
来源：http://ny.gzmigu.cn

[U58] PHP：数组三件套
来源：http://gf.nszjky.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nd.colortex.cn

[U59] PHP：自定义排序
来源：http://zc.chemitech.net.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vc.chemitech.net.cn

[U60] PHP：JSON 编解码
来源：http://dx.jctech888.com.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://is.newstarts.cn

[U61] PHP：正则
来源：http://sq.huanxung.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pa.panjiajie.cn

[U62] PHP：日期对象
来源：http://rn.huixinmuqiang.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fb.hnjuh.cn

[U63] PHP：文件读写
来源：http://ds.asd995.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wm.szsharing.cn

[U64] PHP：目录遍历
来源：http://kr.chemitech.net.cn

glob("dir/*.php");  scandir("dir");
来源：http://gm.shxzukj.cn

[U65] PHP：会话
来源：http://cg.bjjhwx.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://yo.hahajie.cn

[U66] PHP：设置 Cookie
来源：http://he.hnjuh.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://up.huanxung.cn

[U67] PHP：处理文件上传
来源：http://zo.jianghongdianzi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kq.yuntaijiaju.cn

[U68] PHP：PDO 连接
来源：http://ve.haigaiapp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ym.shtwfgs.cn

[U69] PHP：PDO 预处理
来源：http://li.asd995.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ib.shtwfgs.cn

[U70] PHP：PDO 事务
来源：http://co.yuexingan06.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rg.yuntaijiaju.cn

[U71] PHP：抛出异常
来源：http://we.nszjky.cn

throw new RuntimeException("失败", 500);
来源：http://oj.shxzukj.cn

[U72] PHP：写错误日志
来源：http://wk.jctech888.com.cn

error_log("失败: " . $e->getMessage());
来源：http://vs.bookmarksfly.cn

[U73] PHP：读取 ini 配置
来源：http://fw.hahajie.cn

parse_ini_file("config.ini", true)
来源：http://el.bjjhwx.cn

[U74] PHP：读取环境变量
来源：http://ek.panjiajie.cn

getenv("APP_ENV") ?: "production"
来源：http://sa.521024.cn

[U75] PHP：依赖注入
来源：http://vd.bjjhwx.cn

composer require psr/container
来源：http://sv.shxzukj.cn

[U76] PHP：简单路由
来源：http://xu.521024.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fd.nicolike.cn

[U77] PHP：模板渲染
来源：http://zn.haigaiapp.cn

composer require twig/twig
来源：http://az.yuntaijiaju.cn

[U78] PHP：单元测试
来源：http://bd.colortex.cn

composer require --dev phpunit/phpunit
来源：http://gt.huixiangedu.cn

[U79] PHP：静态分析
来源：http://af.shtwfgs.cn

composer require --dev phpstan/phpstan
来源：http://ih.jctech888.com.cn

[U80] PHP：代码规范修复
来源：http://ta.521024.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://vd.szxytkj.cn

[U81] JS：初始化项目
来源：http://fr.asd995.cn

npm init -y;  npm i express
来源：http://wh.jctech888.com.cn

[U82] JS：package.json 脚本
来源：http://er.muxihuayi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ns.yuexingan06.cn

[U83] JS：ES Module 导入导出
来源：http://qs.hahajie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://kb.jctech888.com.cn

[U84] JS：CommonJS 写法
来源：http://gl.shxzukj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://og.huixiangedu.cn


<!-- 参考信息 -->