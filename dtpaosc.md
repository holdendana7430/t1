代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mb.jianghongdianzi.cn

[S57] C++：编译期常量
来源：http://cq.huixinmuqiang.cn

constexpr int N = 10;
来源：http://wg.jctech888.com.cn

[S58] C++：命名空间
来源：http://xn.shxzskj.cn

namespace ns { int f() { return 1; } }
来源：http://ec.bjjhwx.cn

[S59] C++：静态断言
来源：http://yq.521024.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nj.yuexingan06.cn

[S60] C++：遍历并删除元素
来源：http://qq.panjiajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wl.colortex.cn

================================================================================
来源：http://iy.bookmarksfly.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gi.huixiangedu.cn

================================================================================
来源：http://ya.lnxyls.cn

[T01] Kotlin：Hello World
来源：http://or.newstarts.cn

println("Hello")
来源：http://ue.521024.cn

[T02] Kotlin：变量
来源：http://ae.bjjhwx.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wm.jianghongdianzi.cn

[T03] Kotlin：字符串模板
来源：http://vh.bjjhwx.cn

"值: $b"
来源：http://bv.lnxyls.cn

[T04] Kotlin：空安全
来源：http://yb.gzmigu.cn

val n: String? = null;  n?.length
来源：http://cx.chemitech.net.cn

[T05] Kotlin：when 表达式
来源：http://tw.muxihuayi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mh.muxihuayi.cn

[T06] Kotlin：集合映射
来源：http://jj.yuntaijiaju.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ii.9csxet.cn

[T07] Kotlin：集合过滤
来源：http://nx.shtwfgs.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://li.lnxyls.cn

[T08] Kotlin：数据类
来源：http://zh.huixinmuqiang.cn

data class User(val name: String, val age: Int)
来源：http://tb.huanxung.cn

[T09] Kotlin：扩展函数
来源：http://ig.szxytkj.cn

fun String.exclaim() = this + "!"
来源：http://dy.haigaiapp.cn

[T10] Kotlin：默认参数
来源：http://wt.yuntaijiaju.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xw.wgjwhj.cn

[T11] Kotlin：协程
来源：http://wo.jctech888.com.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vh.colortex.cn

[T12] Kotlin：解构声明
来源：http://cy.hahajie.cn

val (a, b) = Pair(1, 2)
来源：http://kw.shtwfgs.cn

[T13] Kotlin：只读 Map
来源：http://dt.jianghongdianzi.cn

val m = mapOf("a" to 1)
来源：http://yw.hahajie.cn

[T14] Kotlin：循环
来源：http://wt.huixiangedu.cn

for (i in 1..10) println(i)
来源：http://ol.panjiajie.cn

[T15] Kotlin：接口
来源：http://ab.muxihuayi.cn

interface Shape { fun area(): Double }
来源：http://tz.hnjuh.cn

[T16] Swift：Hello World
来源：http://af.asd995.cn

print("Hello")
来源：http://io.huixiangedu.cn

[T17] Swift：变量与常量
来源：http://jn.chemitech.net.cn

var a = 1;  let b = 2
来源：http://se.huanxung.cn

[T18] Swift：字符串插值
来源：http://lk.lnxyls.cn

"值: \(b)"
来源：http://bw.lnxyls.cn

[T19] Swift：可选绑定
来源：http://kz.bjjhwx.cn

if let n = opt { print(n) }
来源：http://qp.hahajie.cn

[T20] Swift：数组操作
来源：http://rz.hnjuh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://oo.lnxyls.cn

[T21] Swift：遍历
来源：http://ik.bookmarksfly.cn

for x in a { print(x) }
来源：http://ai.bookmarksfly.cn

[T22] Swift：字典
来源：http://vy.colortex.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vw.huixinmuqiang.cn

[T23] Swift：函数
来源：http://pn.yuntaijiaju.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ft.nicolike.cn

[T24] Swift：闭包
来源：http://hz.bjjhwx.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://pj.jianghongdianzi.cn

[T25] Swift：结构体
来源：http://at.shtwfgs.cn

struct P { var x: Int }
来源：http://dw.bjjhwx.cn

[T26] Swift：类与重写
来源：http://bb.hnjuh.cn

class A: Base { override func f() {} }
来源：http://lx.szsharing.cn

[T27] Swift：错误处理
来源：http://hb.huixinmuqiang.cn

do { try f() } catch { print(error) }
来源：http://mj.newstarts.cn

[T28] Swift：枚举
来源：http://cs.szsharing.cn

enum Color { case red, green }
来源：http://mq.shtwfgs.cn

[T29] Swift：guard 提前返回
来源：http://bd.bookmarksfly.cn

guard let x = opt else { return }
来源：http://sf.huixinmuqiang.cn

[T30] Swift：协议
来源：http://cf.nicolike.cn

protocol Shape { func area() -> Double }
来源：http://nj.wgjwhj.cn

[T31] Lua：Hello World
来源：http://tj.bookmarksfly.cn

print("Hello")
来源：http://rd.shxzukj.cn

[T32] Lua：局部变量
来源：http://iv.hnjuh.cn

local a = 1
来源：http://on.newstarts.cn

[T33] Lua：表（数组）
来源：http://za.huixinmuqiang.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ph.jctech888.com.cn

[T34] Lua：遍历表
来源：http://yi.colortex.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://jg.jianghongdianzi.cn

[T35] Lua：字典表
来源：http://no.yuntaijiaju.cn

local d = { a = 1 };  d.b = 2
来源：http://hz.521024.cn

[T36] Lua：函数
来源：http://mq.panjiajie.cn

function add(a, b) return a + b end
来源：http://tw.shtwfgs.cn

[T37] Lua：字符串拼接
来源：http://fz.yuntaijiaju.cn

"a" .. "b"
来源：http://wx.nszjky.cn

[T38] Lua：条件
来源：http://yc.hnjuh.cn

if x > 0 then print("正") end
来源：http://rq.shxzskj.cn

[T39] Lua：模式匹配
来源：http://vf.gzmigu.cn

string.find(s, "%d+")
来源：http://gk.muxihuayi.cn

[T40] Lua：元表
来源：http://bj.bookmarksfly.cn

setmetatable({}, { __index = base })
来源：http://lh.asd995.cn

[T41] Perl：Hello World
来源：http://gp.lnxyls.cn

print "Hello\n";
来源：http://xy.nszjky.cn

[T42] Perl：变量类型
来源：http://kz.szsharing.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://oz.521024.cn

[T43] Perl：字符串插值
来源：http://an.nicolike.cn

"值: $a"
来源：http://mp.muxihuayi.cn

[T44] Perl：条件
来源：http://dp.jctech888.com.cn

if ($a > 0) { print "正"; }
来源：http://fz.huanxung.cn

[T45] Perl：数组遍历
来源：http://eb.colortex.cn

for my $x (@arr) { print $x; }
来源：http://ir.521024.cn

[T46] Perl：哈希操作
来源：http://yo.muxihuayi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qf.asd995.cn

[T47] Perl：正则捕获
来源：http://rd.9csxet.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://sj.asd995.cn

[T48] Perl：正则替换
来源：http://zb.asd995.cn

$s =~ s/old/new/g;
来源：http://xz.jianghongdianzi.cn

[T49] Perl：函数
来源：http://us.bjjhwx.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pq.huixinmuqiang.cn

[T50] Perl：逐行读文件
来源：http://nt.szsharing.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://aq.szsharing.cn

while (my $line = <$fh>) { print $line; }
来源：http://ps.hahajie.cn

[T51] Scala：Hello World
来源：http://zq.nszjky.cn

println("Hello")
来源：http://vr.bjjhwx.cn

[T52] Scala：变量
来源：http://cn.yuexingan06.cn

val a = 1;  var b = 2
来源：http://yb.yuntaijiaju.cn

[T53] Scala：字符串插值
来源：http://ig.9csxet.cn

s"值: $b"
来源：http://xe.szsharing.cn

[T54] Scala：集合映射
来源：http://ml.shtwfgs.cn

List(1, 2, 3).map(_ * 2)
来源：http://vr.jctech888.com.cn

[T55] Scala：集合过滤
来源：http://ky.chemitech.net.cn

List(1, 2, 3).filter(_ > 1)
来源：http://bu.muxihuayi.cn

[T56] Scala：样例类
来源：http://pn.huixiangedu.cn

case class User(name: String, age: Int)
来源：http://oo.huixiangedu.cn

[T57] Scala：模式匹配
来源：http://ri.panjiajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://pb.nszjky.cn

[T58] Scala：函数定义
来源：http://se.huanxung.cn

def add(a: Int, b: Int): Int = a + b
来源：http://xt.yuntaijiaju.cn

[T59] Scala：循环
来源：http://hg.9csxet.cn

for (i <- 1 to 10) println(i)
来源：http://me.colortex.cn

[T60] Scala：折叠
来源：http://je.lnxyls.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pq.jctech888.com.cn

================================================================================
来源：http://cq.hahajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zb.lnxyls.cn

================================================================================
来源：http://ng.asd995.cn

[U01] Py：创建虚拟环境
来源：http://mn.haigaiapp.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vs.yuntaijiaju.cn

[U02] Py：导出 / 安装依赖
来源：http://aq.yuntaijiaju.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ob.9csxet.cn

[U03] Py：加载 .env 配置
来源：http://rj.muxihuayi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://iy.newstarts.cn

[U04] Py：变量调试打印
来源：http://ax.huixiangedu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bq.nszjky.cn

[U05] Py：列表去重且保序
来源：http://ym.hahajie.cn

list(dict.fromkeys(arr))
来源：http://mt.lnxyls.cn

[U06] Py：合并两个字典
来源：http://go.szxytkj.cn

{**a, **b}
来源：http://ww.wgjwhj.cn

[U07] Py：反转字典键值
来源：http://rf.bjjhwx.cn

{v: k for k, v in d.items()}
来源：http://rs.colortex.cn

[U08] Py：展平二维列表
来源：http://do.hnjuh.cn

[y for x in nested for y in x]
来源：http://oy.huanxung.cn

[U09] Py：字典取最大值的键
来源：http://wc.panjiajie.cn

max(d, key=d.get)
来源：http://iw.huanxung.cn

[U10] Py：按值排序字典
来源：http://dn.huanxung.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mb.szsharing.cn

[U11] Py：生成器表达式
来源：http://yh.hahajie.cn

(x * 2 for x in arr)
来源：http://ml.hahajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://dd.muxihuayi.cn

Counter(arr).most_common(3)
来源：http://rj.chemitech.net.cn

[U13] Py：固定长度队列
来源：http://ow.gzmigu.cn

deque(maxlen=10)
来源：http://rt.newstarts.cn

[U14] Py：分组收集到列表
来源：http://jg.shxzskj.cn

defaultdict(list)
来源：http://es.521024.cn

[U15] Py：高精度计时
来源：http://yk.bjjhwx.cn

t = time.perf_counter()
来源：http://ry.9csxet.cn

[U16] Py：命令行参数解析
来源：http://nu.jctech888.com.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bs.muxihuayi.cn

[U17] Py：初始化日志
来源：http://hr.521024.cn

logging.basicConfig(level=logging.INFO)
来源：http://bg.jctech888.com.cn

[U18] Py：预编译正则
来源：http://vg.lnxyls.cn

pat = re.compile(r"\d+")
来源：http://lu.shtwfgs.cn

[U19] Py：正则替换带回调
来源：http://xp.hahajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pu.shxzskj.cn

[U20] Py：缓存函数结果
来源：http://ht.muxihuayi.cn

@functools.lru_cache(maxsize=None)
来源：http://px.521024.cn

[U21] Py：自定义上下文管理器
来源：http://zs.muxihuayi.cn

@contextlib.contextmanager
来源：http://fb.szsharing.cn

[U22] Py：矩阵转置
来源：http://jr.colortex.cn

list(zip(*m))
来源：http://vz.bjjhwx.cn

[U23] Py：分块读取大文件
来源：http://cm.haigaiapp.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ya.chemitech.net.cn

[U24] Py：路径操作
来源：http://sa.bookmarksfly.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ni.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://cm.shxzskj.cn

csv.DictReader(f)
来源：http://hn.bjjhwx.cn

[U26] Py：并发下载
来源：http://sm.shxzukj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ad.nszjky.cn

[U27] Py：异步 HTTP
来源：http://xc.jctech888.com.cn

aiohttp.ClientSession() 配合 async with
来源：http://fp.bjjhwx.cn

[U28] Py：类型别名
来源：http://ey.chemitech.net.cn

UserId = int
来源：http://hm.asd995.cn

[U29] Py：属性校验
来源：http://nm.shxzukj.cn

@property 与 @x.setter 配合
来源：http://yf.huixinmuqiang.cn

[U30] Py：数据类
来源：http://uo.shxzskj.cn

@dataclass(slots=True)
来源：http://yh.nszjky.cn

[U31] Py：单测
来源：http://ys.yuexingan06.cn

python -m pytest -q
来源：http://rs.huixiangedu.cn

[U32] Py：代码格式化
来源：http://pz.newstarts.cn

ruff format . && ruff check --fix .
来源：http://ij.huixiangedu.cn

[U33] Py：打包发布
来源：http://pi.chemitech.net.cn

python -m build  （依赖 pyproject.toml）
来源：http://qx.szsharing.cn

[U34] Py：判断编码
来源：http://ut.huixinmuqiang.cn

chardet.detect(raw)
来源：http://dv.hahajie.cn

[U35] Py：发送邮件
来源：http://cw.shxzskj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tz.jctech888.com.cn

[U36] Py：定时任务
来源：http://qm.521024.cn

schedule.every(10).minutes.do(job)
来源：http://qt.huixinmuqiang.cn

[U37] Py：读写 Excel
来源：http://pc.hahajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://nt.shxzukj.cn

[U38] Py：获取脚本所在目录
来源：http://ze.szsharing.cn

Path(__file__).resolve().parent
来源：http://ae.wgjwhj.cn

[U39] Py：判断是否在交互环境
来源：http://yu.yuntaijiaju.cn

sys.stdout.isatty()
来源：http://tk.jctech888.com.cn

[U40] Py：打印到标准错误
来源：http://gd.asd995.cn

print("err", file=sys.stderr)
来源：http://ba.hahajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://dj.nicolike.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://wb.panjiajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://zv.shtwfgs.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yg.lnxyls.cn

[U43] PHP：声明命名空间
来源：http://bm.bookmarksfly.cn

namespace App\Http;
来源：http://uh.haigaiapp.cn

[U44] PHP：开启严格类型
来源：http://lx.yuntaijiaju.cn

declare(strict_types=1);
来源：http://td.yuexingan06.cn

[U45] PHP：类型声明与返回类型
来源：http://fd.nszjky.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://it.muxihuayi.cn

[U46] PHP：可空类型
来源：http://hr.bookmarksfly.cn

?string $name = null
来源：http://yt.asd995.cn

[U47] PHP：联合类型
来源：http://lo.hnjuh.cn

int|string $id
来源：http://ve.shxzskj.cn

[U48] PHP：纯枚举
来源：http://jq.chemitech.net.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ac.asd995.cn

[U49] PHP：只读属性
来源：http://km.lnxyls.cn

public readonly string $name
来源：http://po.newstarts.cn

[U50] PHP：构造器属性提升
来源：http://gq.huixinmuqiang.cn

public function __construct(private int $id) {}
来源：http://ds.wgjwhj.cn

[U51] PHP：数组解构
来源：http://rt.jianghongdianzi.cn

[$a, $b] = $arr;
来源：http://cx.huanxung.cn

[U52] PHP：箭头函数
来源：http://bf.huanxung.cn

$double = fn($x) => $x * 2;
来源：http://mh.wgjwhj.cn

[U53] PHP：空合并运算符
来源：http://ik.huixinmuqiang.cn

$v = $a ?? $b ?? "default";
来源：http://gf.panjiajie.cn

[U54] PHP：空安全调用
来源：http://yk.shxzskj.cn

$obj?->method()
来源：http://ve.shxzukj.cn

[U55] PHP：match 表达式
来源：http://vo.shtwfgs.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ba.jianghongdianzi.cn

[U56] PHP：命名参数
来源：http://ac.9csxet.cn

f(a: 1, b: 2)
来源：http://wb.huixinmuqiang.cn

[U57] PHP：字符串插值
来源：http://rn.nszjky.cn

"值: {$a}"
来源：http://fw.yuntaijiaju.cn

[U58] PHP：数组三件套
来源：http://me.shtwfgs.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ne.jianghongdianzi.cn

[U59] PHP：自定义排序
来源：http://oq.szxytkj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kc.lnxyls.cn

[U60] PHP：JSON 编解码
来源：http://uq.muxihuayi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vr.huixinmuqiang.cn

[U61] PHP：正则
来源：http://so.shxzukj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ln.nicolike.cn

[U62] PHP：日期对象
来源：http://gd.bookmarksfly.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://oy.shxzskj.cn

[U63] PHP：文件读写
来源：http://uz.9csxet.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wt.szxytkj.cn

[U64] PHP：目录遍历
来源：http://yj.wgjwhj.cn

glob("dir/*.php");  scandir("dir");
来源：http://nn.huanxung.cn

[U65] PHP：会话
来源：http://xd.nicolike.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://qt.wgjwhj.cn

[U66] PHP：设置 Cookie
来源：http://tw.panjiajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lu.yuntaijiaju.cn

[U67] PHP：处理文件上传
来源：http://if.szsharing.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ke.yuntaijiaju.cn

[U68] PHP：PDO 连接
来源：http://ow.hahajie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bb.bookmarksfly.cn

[U69] PHP：PDO 预处理
来源：http://cc.asd995.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pp.521024.cn

[U70] PHP：PDO 事务
来源：http://du.chemitech.net.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ik.gzmigu.cn

[U71] PHP：抛出异常
来源：http://ia.shxzukj.cn

throw new RuntimeException("失败", 500);
来源：http://lq.shxzukj.cn

[U72] PHP：写错误日志
来源：http://ih.huixiangedu.cn

error_log("失败: " . $e->getMessage());
来源：http://si.yuntaijiaju.cn

[U73] PHP：读取 ini 配置
来源：http://gk.yuexingan06.cn

parse_ini_file("config.ini", true)
来源：http://jo.szsharing.cn

[U74] PHP：读取环境变量
来源：http://rp.jianghongdianzi.cn

getenv("APP_ENV") ?: "production"
来源：http://fg.nicolike.cn

[U75] PHP：依赖注入
来源：http://un.bookmarksfly.cn

composer require psr/container
来源：http://fk.nszjky.cn

[U76] PHP：简单路由
来源：http://ry.yuexingan06.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rg.huixinmuqiang.cn

[U77] PHP：模板渲染
来源：http://xz.nicolike.cn

composer require twig/twig
来源：http://fs.gzmigu.cn

[U78] PHP：单元测试
来源：http://fp.chemitech.net.cn

composer require --dev phpunit/phpunit
来源：http://dr.asd995.cn

[U79] PHP：静态分析
来源：http://uu.wgjwhj.cn

composer require --dev phpstan/phpstan
来源：http://cs.yuntaijiaju.cn

[U80] PHP：代码规范修复
来源：http://ex.wgjwhj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xw.panjiajie.cn

[U81] JS：初始化项目
来源：http://sx.hnjuh.cn

npm init -y;  npm i express
来源：http://fq.newstarts.cn

[U82] JS：package.json 脚本
来源：http://sj.huixiangedu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nq.bookmarksfly.cn


<!-- 参考信息 -->