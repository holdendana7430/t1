代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://ni.szxytkj.cn

[S59] C++：静态断言
来源：http://js.gzmigu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wl.lnxyls.cn

[S60] C++：遍历并删除元素
来源：http://ew.lnxyls.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ca.szsharing.cn

================================================================================
来源：http://ei.hahajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pt.szsharing.cn

================================================================================
来源：http://iu.shtwfgs.cn

[T01] Kotlin：Hello World
来源：http://vx.panjiajie.cn

println("Hello")
来源：http://ew.haigaiapp.cn

[T02] Kotlin：变量
来源：http://op.9csxet.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ih.szsharing.cn

[T03] Kotlin：字符串模板
来源：http://cs.hnjuh.cn

"值: $b"
来源：http://qy.wgjwhj.cn

[T04] Kotlin：空安全
来源：http://yp.colortex.cn

val n: String? = null;  n?.length
来源：http://je.asd995.cn

[T05] Kotlin：when 表达式
来源：http://mv.shtwfgs.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xr.huixiangedu.cn

[T06] Kotlin：集合映射
来源：http://ow.nszjky.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://le.colortex.cn

[T07] Kotlin：集合过滤
来源：http://nv.shxzukj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://em.yuexingan06.cn

[T08] Kotlin：数据类
来源：http://mf.huixiangedu.cn

data class User(val name: String, val age: Int)
来源：http://jj.asd995.cn

[T09] Kotlin：扩展函数
来源：http://us.jctech888.com.cn

fun String.exclaim() = this + "!"
来源：http://ad.hahajie.cn

[T10] Kotlin：默认参数
来源：http://ts.521024.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qy.shtwfgs.cn

[T11] Kotlin：协程
来源：http://jj.shxzskj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://eh.panjiajie.cn

[T12] Kotlin：解构声明
来源：http://zo.szsharing.cn

val (a, b) = Pair(1, 2)
来源：http://nr.yuntaijiaju.cn

[T13] Kotlin：只读 Map
来源：http://io.hahajie.cn

val m = mapOf("a" to 1)
来源：http://tf.colortex.cn

[T14] Kotlin：循环
来源：http://iz.bookmarksfly.cn

for (i in 1..10) println(i)
来源：http://br.yuexingan06.cn

[T15] Kotlin：接口
来源：http://to.colortex.cn

interface Shape { fun area(): Double }
来源：http://wz.szsharing.cn

[T16] Swift：Hello World
来源：http://jy.panjiajie.cn

print("Hello")
来源：http://ad.yuntaijiaju.cn

[T17] Swift：变量与常量
来源：http://et.huixiangedu.cn

var a = 1;  let b = 2
来源：http://hr.shtwfgs.cn

[T18] Swift：字符串插值
来源：http://af.shxzskj.cn

"值: \(b)"
来源：http://lx.bookmarksfly.cn

[T19] Swift：可选绑定
来源：http://ge.nszjky.cn

if let n = opt { print(n) }
来源：http://yt.szxytkj.cn

[T20] Swift：数组操作
来源：http://de.521024.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ez.yuntaijiaju.cn

[T21] Swift：遍历
来源：http://rw.hahajie.cn

for x in a { print(x) }
来源：http://my.szxytkj.cn

[T22] Swift：字典
来源：http://zd.szxytkj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://by.huixiangedu.cn

[T23] Swift：函数
来源：http://if.bjjhwx.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ob.chemitech.net.cn

[T24] Swift：闭包
来源：http://tz.nszjky.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xg.colortex.cn

[T25] Swift：结构体
来源：http://lx.nszjky.cn

struct P { var x: Int }
来源：http://ku.9csxet.cn

[T26] Swift：类与重写
来源：http://hg.521024.cn

class A: Base { override func f() {} }
来源：http://uh.bjjhwx.cn

[T27] Swift：错误处理
来源：http://sr.haigaiapp.cn

do { try f() } catch { print(error) }
来源：http://bv.panjiajie.cn

[T28] Swift：枚举
来源：http://xh.9csxet.cn

enum Color { case red, green }
来源：http://bd.szsharing.cn

[T29] Swift：guard 提前返回
来源：http://pa.newstarts.cn

guard let x = opt else { return }
来源：http://mc.szxytkj.cn

[T30] Swift：协议
来源：http://wm.chemitech.net.cn

protocol Shape { func area() -> Double }
来源：http://mp.wgjwhj.cn

[T31] Lua：Hello World
来源：http://yr.nicolike.cn

print("Hello")
来源：http://mv.shxzukj.cn

[T32] Lua：局部变量
来源：http://fy.panjiajie.cn

local a = 1
来源：http://bj.nicolike.cn

[T33] Lua：表（数组）
来源：http://ss.muxihuayi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ec.hnjuh.cn

[T34] Lua：遍历表
来源：http://dr.panjiajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://jb.szxytkj.cn

[T35] Lua：字典表
来源：http://tp.haigaiapp.cn

local d = { a = 1 };  d.b = 2
来源：http://km.yuntaijiaju.cn

[T36] Lua：函数
来源：http://wo.shxzukj.cn

function add(a, b) return a + b end
来源：http://qy.huixiangedu.cn

[T37] Lua：字符串拼接
来源：http://kb.newstarts.cn

"a" .. "b"
来源：http://ay.521024.cn

[T38] Lua：条件
来源：http://eb.huixiangedu.cn

if x > 0 then print("正") end
来源：http://pb.huixiangedu.cn

[T39] Lua：模式匹配
来源：http://vr.bjjhwx.cn

string.find(s, "%d+")
来源：http://ye.jianghongdianzi.cn

[T40] Lua：元表
来源：http://bw.haigaiapp.cn

setmetatable({}, { __index = base })
来源：http://cf.shtwfgs.cn

[T41] Perl：Hello World
来源：http://nj.jctech888.com.cn

print "Hello\n";
来源：http://pm.chemitech.net.cn

[T42] Perl：变量类型
来源：http://if.muxihuayi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qu.yuntaijiaju.cn

[T43] Perl：字符串插值
来源：http://ev.huixinmuqiang.cn

"值: $a"
来源：http://cf.bookmarksfly.cn

[T44] Perl：条件
来源：http://uj.bjjhwx.cn

if ($a > 0) { print "正"; }
来源：http://uf.huanxung.cn

[T45] Perl：数组遍历
来源：http://mq.szsharing.cn

for my $x (@arr) { print $x; }
来源：http://gw.chemitech.net.cn

[T46] Perl：哈希操作
来源：http://nw.521024.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sz.bookmarksfly.cn

[T47] Perl：正则捕获
来源：http://ht.huanxung.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pz.huanxung.cn

[T48] Perl：正则替换
来源：http://xj.bjjhwx.cn

$s =~ s/old/new/g;
来源：http://ib.muxihuayi.cn

[T49] Perl：函数
来源：http://ar.yuntaijiaju.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qd.521024.cn

[T50] Perl：逐行读文件
来源：http://zv.jctech888.com.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://jc.jctech888.com.cn

while (my $line = <$fh>) { print $line; }
来源：http://uw.szxytkj.cn

[T51] Scala：Hello World
来源：http://af.jctech888.com.cn

println("Hello")
来源：http://nq.colortex.cn

[T52] Scala：变量
来源：http://qh.chemitech.net.cn

val a = 1;  var b = 2
来源：http://rq.shxzskj.cn

[T53] Scala：字符串插值
来源：http://fn.hnjuh.cn

s"值: $b"
来源：http://kh.yuexingan06.cn

[T54] Scala：集合映射
来源：http://gu.nicolike.cn

List(1, 2, 3).map(_ * 2)
来源：http://gu.huixinmuqiang.cn

[T55] Scala：集合过滤
来源：http://es.lnxyls.cn

List(1, 2, 3).filter(_ > 1)
来源：http://pt.huanxung.cn

[T56] Scala：样例类
来源：http://ug.shxzskj.cn

case class User(name: String, age: Int)
来源：http://dl.hnjuh.cn

[T57] Scala：模式匹配
来源：http://fx.panjiajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://lr.hnjuh.cn

[T58] Scala：函数定义
来源：http://no.chemitech.net.cn

def add(a: Int, b: Int): Int = a + b
来源：http://an.wgjwhj.cn

[T59] Scala：循环
来源：http://aw.lnxyls.cn

for (i <- 1 to 10) println(i)
来源：http://hq.gzmigu.cn

[T60] Scala：折叠
来源：http://dw.gzmigu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jo.huixinmuqiang.cn

================================================================================
来源：http://tj.haigaiapp.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://oq.lnxyls.cn

================================================================================
来源：http://rh.hahajie.cn

[U01] Py：创建虚拟环境
来源：http://hv.yuntaijiaju.cn

python -m venv .venv && source .venv/bin/activate
来源：http://va.nicolike.cn

[U02] Py：导出 / 安装依赖
来源：http://nu.huixiangedu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xt.shtwfgs.cn

[U03] Py：加载 .env 配置
来源：http://ef.gzmigu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://bw.yuexingan06.cn

[U04] Py：变量调试打印
来源：http://sd.hahajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ea.gzmigu.cn

[U05] Py：列表去重且保序
来源：http://xp.nszjky.cn

list(dict.fromkeys(arr))
来源：http://di.muxihuayi.cn

[U06] Py：合并两个字典
来源：http://bx.huixinmuqiang.cn

{**a, **b}
来源：http://ge.hnjuh.cn

[U07] Py：反转字典键值
来源：http://qj.shxzskj.cn

{v: k for k, v in d.items()}
来源：http://mt.newstarts.cn

[U08] Py：展平二维列表
来源：http://zd.huanxung.cn

[y for x in nested for y in x]
来源：http://vb.521024.cn

[U09] Py：字典取最大值的键
来源：http://kj.shtwfgs.cn

max(d, key=d.get)
来源：http://lu.wgjwhj.cn

[U10] Py：按值排序字典
来源：http://pg.jctech888.com.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cu.newstarts.cn

[U11] Py：生成器表达式
来源：http://aq.hnjuh.cn

(x * 2 for x in arr)
来源：http://wc.nszjky.cn

[U12] Py：取出现最多的 3 个元素
来源：http://gc.yuexingan06.cn

Counter(arr).most_common(3)
来源：http://dz.yuntaijiaju.cn

[U13] Py：固定长度队列
来源：http://jy.shtwfgs.cn

deque(maxlen=10)
来源：http://af.huixiangedu.cn

[U14] Py：分组收集到列表
来源：http://iq.asd995.cn

defaultdict(list)
来源：http://kp.asd995.cn

[U15] Py：高精度计时
来源：http://ew.9csxet.cn

t = time.perf_counter()
来源：http://el.521024.cn

[U16] Py：命令行参数解析
来源：http://fn.lnxyls.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cg.huixinmuqiang.cn

[U17] Py：初始化日志
来源：http://bl.nszjky.cn

logging.basicConfig(level=logging.INFO)
来源：http://yu.nszjky.cn

[U18] Py：预编译正则
来源：http://da.yuntaijiaju.cn

pat = re.compile(r"\d+")
来源：http://yk.wgjwhj.cn

[U19] Py：正则替换带回调
来源：http://lt.colortex.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hw.chemitech.net.cn

[U20] Py：缓存函数结果
来源：http://za.521024.cn

@functools.lru_cache(maxsize=None)
来源：http://be.jctech888.com.cn

[U21] Py：自定义上下文管理器
来源：http://ll.haigaiapp.cn

@contextlib.contextmanager
来源：http://pe.panjiajie.cn

[U22] Py：矩阵转置
来源：http://je.yuntaijiaju.cn

list(zip(*m))
来源：http://oj.shxzukj.cn

[U23] Py：分块读取大文件
来源：http://us.huixinmuqiang.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ly.9csxet.cn

[U24] Py：路径操作
来源：http://ht.shxzukj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ai.panjiajie.cn

[U25] Py：CSV 按字典读
来源：http://on.bookmarksfly.cn

csv.DictReader(f)
来源：http://og.shxzskj.cn

[U26] Py：并发下载
来源：http://ea.nicolike.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yy.shtwfgs.cn

[U27] Py：异步 HTTP
来源：http://gv.szxytkj.cn

aiohttp.ClientSession() 配合 async with
来源：http://es.hnjuh.cn

[U28] Py：类型别名
来源：http://fu.panjiajie.cn

UserId = int
来源：http://jd.newstarts.cn

[U29] Py：属性校验
来源：http://qj.jianghongdianzi.cn

@property 与 @x.setter 配合
来源：http://yk.newstarts.cn

[U30] Py：数据类
来源：http://hc.jctech888.com.cn

@dataclass(slots=True)
来源：http://xg.haigaiapp.cn

[U31] Py：单测
来源：http://ks.jctech888.com.cn

python -m pytest -q
来源：http://bh.bjjhwx.cn

[U32] Py：代码格式化
来源：http://gn.9csxet.cn

ruff format . && ruff check --fix .
来源：http://bo.szsharing.cn

[U33] Py：打包发布
来源：http://ib.lnxyls.cn

python -m build  （依赖 pyproject.toml）
来源：http://je.szxytkj.cn

[U34] Py：判断编码
来源：http://rd.wgjwhj.cn

chardet.detect(raw)
来源：http://ua.jianghongdianzi.cn

[U35] Py：发送邮件
来源：http://ea.nszjky.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mz.521024.cn

[U36] Py：定时任务
来源：http://vj.yuexingan06.cn

schedule.every(10).minutes.do(job)
来源：http://ir.521024.cn

[U37] Py：读写 Excel
来源：http://tq.szsharing.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ge.wgjwhj.cn

[U38] Py：获取脚本所在目录
来源：http://uo.hnjuh.cn

Path(__file__).resolve().parent
来源：http://tc.shxzskj.cn

[U39] Py：判断是否在交互环境
来源：http://yb.szsharing.cn

sys.stdout.isatty()
来源：http://pw.bookmarksfly.cn

[U40] Py：打印到标准错误
来源：http://ju.9csxet.cn

print("err", file=sys.stderr)
来源：http://zb.szsharing.cn

[U41] PHP：初始化 Composer 项目
来源：http://se.bjjhwx.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xz.huixiangedu.cn

[U42] PHP：PSR-4 自动加载
来源：http://lq.huixinmuqiang.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wl.hahajie.cn

[U43] PHP：声明命名空间
来源：http://ja.szsharing.cn

namespace App\Http;
来源：http://ks.huanxung.cn

[U44] PHP：开启严格类型
来源：http://un.jianghongdianzi.cn

declare(strict_types=1);
来源：http://kc.wgjwhj.cn

[U45] PHP：类型声明与返回类型
来源：http://wx.newstarts.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://pr.wgjwhj.cn

[U46] PHP：可空类型
来源：http://xy.huixiangedu.cn

?string $name = null
来源：http://qb.szxytkj.cn

[U47] PHP：联合类型
来源：http://vn.9csxet.cn

int|string $id
来源：http://lh.colortex.cn

[U48] PHP：纯枚举
来源：http://cv.shxzukj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nc.9csxet.cn

[U49] PHP：只读属性
来源：http://db.bookmarksfly.cn

public readonly string $name
来源：http://nh.yuntaijiaju.cn

[U50] PHP：构造器属性提升
来源：http://fg.shxzukj.cn

public function __construct(private int $id) {}
来源：http://ii.521024.cn

[U51] PHP：数组解构
来源：http://mq.lnxyls.cn

[$a, $b] = $arr;
来源：http://ut.yuexingan06.cn

[U52] PHP：箭头函数
来源：http://rh.huanxung.cn

$double = fn($x) => $x * 2;
来源：http://ao.huixinmuqiang.cn

[U53] PHP：空合并运算符
来源：http://lp.szsharing.cn

$v = $a ?? $b ?? "default";
来源：http://pe.bjjhwx.cn

[U54] PHP：空安全调用
来源：http://io.lnxyls.cn

$obj?->method()
来源：http://zs.bookmarksfly.cn

[U55] PHP：match 表达式
来源：http://bj.yuexingan06.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qb.newstarts.cn

[U56] PHP：命名参数
来源：http://wl.huanxung.cn

f(a: 1, b: 2)
来源：http://ph.hnjuh.cn

[U57] PHP：字符串插值
来源：http://ed.shxzukj.cn

"值: {$a}"
来源：http://qj.9csxet.cn

[U58] PHP：数组三件套
来源：http://zw.nicolike.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xg.jctech888.com.cn

[U59] PHP：自定义排序
来源：http://gb.hahajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qc.haigaiapp.cn

[U60] PHP：JSON 编解码
来源：http://yv.9csxet.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tk.shtwfgs.cn

[U61] PHP：正则
来源：http://fn.shtwfgs.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hn.shxzukj.cn

[U62] PHP：日期对象
来源：http://mk.jctech888.com.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zh.huixiangedu.cn

[U63] PHP：文件读写
来源：http://qg.panjiajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pn.haigaiapp.cn

[U64] PHP：目录遍历
来源：http://by.hnjuh.cn

glob("dir/*.php");  scandir("dir");
来源：http://sn.huixinmuqiang.cn

[U65] PHP：会话
来源：http://od.chemitech.net.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://oj.gzmigu.cn

[U66] PHP：设置 Cookie
来源：http://hq.panjiajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zf.nicolike.cn

[U67] PHP：处理文件上传
来源：http://xf.yuexingan06.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yk.chemitech.net.cn

[U68] PHP：PDO 连接
来源：http://ns.hnjuh.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dj.szxytkj.cn

[U69] PHP：PDO 预处理
来源：http://mw.hahajie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gj.yuexingan06.cn

[U70] PHP：PDO 事务
来源：http://ur.bookmarksfly.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gy.szsharing.cn

[U71] PHP：抛出异常
来源：http://on.colortex.cn

throw new RuntimeException("失败", 500);
来源：http://pq.newstarts.cn

[U72] PHP：写错误日志
来源：http://yc.521024.cn

error_log("失败: " . $e->getMessage());
来源：http://sk.bookmarksfly.cn

[U73] PHP：读取 ini 配置
来源：http://kr.asd995.cn

parse_ini_file("config.ini", true)
来源：http://jq.haigaiapp.cn

[U74] PHP：读取环境变量
来源：http://oy.wgjwhj.cn

getenv("APP_ENV") ?: "production"
来源：http://kk.lnxyls.cn

[U75] PHP：依赖注入
来源：http://kx.muxihuayi.cn

composer require psr/container
来源：http://xp.hnjuh.cn

[U76] PHP：简单路由
来源：http://qm.chemitech.net.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bs.huixinmuqiang.cn

[U77] PHP：模板渲染
来源：http://os.9csxet.cn

composer require twig/twig
来源：http://hh.muxihuayi.cn

[U78] PHP：单元测试
来源：http://fk.colortex.cn

composer require --dev phpunit/phpunit
来源：http://ld.muxihuayi.cn

[U79] PHP：静态分析
来源：http://ob.asd995.cn

composer require --dev phpstan/phpstan
来源：http://xt.muxihuayi.cn

[U80] PHP：代码规范修复
来源：http://hv.shxzukj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://nj.huanxung.cn

[U81] JS：初始化项目
来源：http://kx.yuntaijiaju.cn

npm init -y;  npm i express
来源：http://dc.9csxet.cn

[U82] JS：package.json 脚本
来源：http://lx.lnxyls.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mp.colortex.cn

[U83] JS：ES Module 导入导出
来源：http://lf.huanxung.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ml.huixinmuqiang.cn

[U84] JS：CommonJS 写法
来源：http://bk.muxihuayi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://nq.nicolike.cn


<!-- 参考信息 -->