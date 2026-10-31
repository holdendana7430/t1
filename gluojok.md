代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uf.huixinmuqiang.cn

[S57] C++：编译期常量
来源：http://pa.szsharing.cn

constexpr int N = 10;
来源：http://lh.hahajie.cn

[S58] C++：命名空间
来源：http://up.521024.cn

namespace ns { int f() { return 1; } }
来源：http://te.szxytkj.cn

[S59] C++：静态断言
来源：http://ch.haigaiapp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://sw.yuexingan06.cn

[S60] C++：遍历并删除元素
来源：http://ic.muxihuayi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ae.bjjhwx.cn

================================================================================
来源：http://id.nicolike.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fk.lnxyls.cn

================================================================================
来源：http://tu.hnjuh.cn

[T01] Kotlin：Hello World
来源：http://cg.hahajie.cn

println("Hello")
来源：http://ok.shxzskj.cn

[T02] Kotlin：变量
来源：http://ik.haigaiapp.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kf.chemitech.net.cn

[T03] Kotlin：字符串模板
来源：http://rq.521024.cn

"值: $b"
来源：http://lp.shxzskj.cn

[T04] Kotlin：空安全
来源：http://dt.huixiangedu.cn

val n: String? = null;  n?.length
来源：http://ca.shxzukj.cn

[T05] Kotlin：when 表达式
来源：http://nd.bookmarksfly.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ib.wgjwhj.cn

[T06] Kotlin：集合映射
来源：http://gp.shtwfgs.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://vc.asd995.cn

[T07] Kotlin：集合过滤
来源：http://xe.521024.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wn.shtwfgs.cn

[T08] Kotlin：数据类
来源：http://ui.shtwfgs.cn

data class User(val name: String, val age: Int)
来源：http://nb.jianghongdianzi.cn

[T09] Kotlin：扩展函数
来源：http://xu.wgjwhj.cn

fun String.exclaim() = this + "!"
来源：http://dj.9csxet.cn

[T10] Kotlin：默认参数
来源：http://ma.shxzukj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://oy.yuexingan06.cn

[T11] Kotlin：协程
来源：http://bv.chemitech.net.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qx.haigaiapp.cn

[T12] Kotlin：解构声明
来源：http://ep.chemitech.net.cn

val (a, b) = Pair(1, 2)
来源：http://xh.9csxet.cn

[T13] Kotlin：只读 Map
来源：http://wa.newstarts.cn

val m = mapOf("a" to 1)
来源：http://dp.jianghongdianzi.cn

[T14] Kotlin：循环
来源：http://kx.szsharing.cn

for (i in 1..10) println(i)
来源：http://bw.bookmarksfly.cn

[T15] Kotlin：接口
来源：http://pf.jianghongdianzi.cn

interface Shape { fun area(): Double }
来源：http://xp.bookmarksfly.cn

[T16] Swift：Hello World
来源：http://ue.newstarts.cn

print("Hello")
来源：http://fk.9csxet.cn

[T17] Swift：变量与常量
来源：http://ch.shxzskj.cn

var a = 1;  let b = 2
来源：http://ri.huanxung.cn

[T18] Swift：字符串插值
来源：http://ho.9csxet.cn

"值: \(b)"
来源：http://ab.bookmarksfly.cn

[T19] Swift：可选绑定
来源：http://cw.bjjhwx.cn

if let n = opt { print(n) }
来源：http://uo.bjjhwx.cn

[T20] Swift：数组操作
来源：http://mr.asd995.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ca.9csxet.cn

[T21] Swift：遍历
来源：http://uf.huixiangedu.cn

for x in a { print(x) }
来源：http://ww.asd995.cn

[T22] Swift：字典
来源：http://dj.521024.cn

var d = ["a": 1];  d["b"] = 2
来源：http://oq.haigaiapp.cn

[T23] Swift：函数
来源：http://cy.yuntaijiaju.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uy.shxzskj.cn

[T24] Swift：闭包
来源：http://hl.nszjky.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ut.huanxung.cn

[T25] Swift：结构体
来源：http://od.nicolike.cn

struct P { var x: Int }
来源：http://tr.colortex.cn

[T26] Swift：类与重写
来源：http://jd.lnxyls.cn

class A: Base { override func f() {} }
来源：http://hk.chemitech.net.cn

[T27] Swift：错误处理
来源：http://sx.yuntaijiaju.cn

do { try f() } catch { print(error) }
来源：http://wq.9csxet.cn

[T28] Swift：枚举
来源：http://gg.colortex.cn

enum Color { case red, green }
来源：http://ne.asd995.cn

[T29] Swift：guard 提前返回
来源：http://fz.nszjky.cn

guard let x = opt else { return }
来源：http://jf.bjjhwx.cn

[T30] Swift：协议
来源：http://vp.nicolike.cn

protocol Shape { func area() -> Double }
来源：http://mz.shtwfgs.cn

[T31] Lua：Hello World
来源：http://xk.szsharing.cn

print("Hello")
来源：http://gc.huanxung.cn

[T32] Lua：局部变量
来源：http://qa.lnxyls.cn

local a = 1
来源：http://kh.muxihuayi.cn

[T33] Lua：表（数组）
来源：http://hn.panjiajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://qi.bookmarksfly.cn

[T34] Lua：遍历表
来源：http://dg.nszjky.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qf.hnjuh.cn

[T35] Lua：字典表
来源：http://hm.muxihuayi.cn

local d = { a = 1 };  d.b = 2
来源：http://kt.521024.cn

[T36] Lua：函数
来源：http://al.521024.cn

function add(a, b) return a + b end
来源：http://vx.jianghongdianzi.cn

[T37] Lua：字符串拼接
来源：http://ae.jctech888.com.cn

"a" .. "b"
来源：http://nn.asd995.cn

[T38] Lua：条件
来源：http://kj.nicolike.cn

if x > 0 then print("正") end
来源：http://yy.panjiajie.cn

[T39] Lua：模式匹配
来源：http://no.nszjky.cn

string.find(s, "%d+")
来源：http://ga.haigaiapp.cn

[T40] Lua：元表
来源：http://do.shxzukj.cn

setmetatable({}, { __index = base })
来源：http://cy.hahajie.cn

[T41] Perl：Hello World
来源：http://fq.asd995.cn

print "Hello\n";
来源：http://vq.panjiajie.cn

[T42] Perl：变量类型
来源：http://bp.muxihuayi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qp.9csxet.cn

[T43] Perl：字符串插值
来源：http://sq.gzmigu.cn

"值: $a"
来源：http://za.huixinmuqiang.cn

[T44] Perl：条件
来源：http://fn.muxihuayi.cn

if ($a > 0) { print "正"; }
来源：http://ze.yuexingan06.cn

[T45] Perl：数组遍历
来源：http://mr.chemitech.net.cn

for my $x (@arr) { print $x; }
来源：http://kc.chemitech.net.cn

[T46] Perl：哈希操作
来源：http://ki.szsharing.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cf.yuexingan06.cn

[T47] Perl：正则捕获
来源：http://du.hahajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://se.shxzskj.cn

[T48] Perl：正则替换
来源：http://xo.shxzukj.cn

$s =~ s/old/new/g;
来源：http://lo.nicolike.cn

[T49] Perl：函数
来源：http://sc.jianghongdianzi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dt.muxihuayi.cn

[T50] Perl：逐行读文件
来源：http://py.shxzukj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://mo.muxihuayi.cn

while (my $line = <$fh>) { print $line; }
来源：http://tl.newstarts.cn

[T51] Scala：Hello World
来源：http://ga.bjjhwx.cn

println("Hello")
来源：http://ef.shxzukj.cn

[T52] Scala：变量
来源：http://aa.muxihuayi.cn

val a = 1;  var b = 2
来源：http://tm.lnxyls.cn

[T53] Scala：字符串插值
来源：http://xd.muxihuayi.cn

s"值: $b"
来源：http://xw.huixinmuqiang.cn

[T54] Scala：集合映射
来源：http://nl.hnjuh.cn

List(1, 2, 3).map(_ * 2)
来源：http://zc.shxzskj.cn

[T55] Scala：集合过滤
来源：http://vn.shxzskj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://yk.szsharing.cn

[T56] Scala：样例类
来源：http://tw.bjjhwx.cn

case class User(name: String, age: Int)
来源：http://nb.huixiangedu.cn

[T57] Scala：模式匹配
来源：http://fk.hahajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://eq.huixiangedu.cn

[T58] Scala：函数定义
来源：http://ys.hahajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://vu.9csxet.cn

[T59] Scala：循环
来源：http://ky.bookmarksfly.cn

for (i <- 1 to 10) println(i)
来源：http://ve.bjjhwx.cn

[T60] Scala：折叠
来源：http://bo.shxzskj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nj.szxytkj.cn

================================================================================
来源：http://dg.huixiangedu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ig.shxzukj.cn

================================================================================
来源：http://di.hahajie.cn

[U01] Py：创建虚拟环境
来源：http://zm.huanxung.cn

python -m venv .venv && source .venv/bin/activate
来源：http://yw.huixinmuqiang.cn

[U02] Py：导出 / 安装依赖
来源：http://gd.huanxung.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pa.bjjhwx.cn

[U03] Py：加载 .env 配置
来源：http://cq.haigaiapp.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://tk.huixiangedu.cn

[U04] Py：变量调试打印
来源：http://eh.asd995.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ha.521024.cn

[U05] Py：列表去重且保序
来源：http://ed.bjjhwx.cn

list(dict.fromkeys(arr))
来源：http://mu.huixinmuqiang.cn

[U06] Py：合并两个字典
来源：http://vl.newstarts.cn

{**a, **b}
来源：http://vn.panjiajie.cn

[U07] Py：反转字典键值
来源：http://mf.huixiangedu.cn

{v: k for k, v in d.items()}
来源：http://nv.panjiajie.cn

[U08] Py：展平二维列表
来源：http://yx.colortex.cn

[y for x in nested for y in x]
来源：http://kt.bjjhwx.cn

[U09] Py：字典取最大值的键
来源：http://iw.lnxyls.cn

max(d, key=d.get)
来源：http://yf.huixiangedu.cn

[U10] Py：按值排序字典
来源：http://ge.asd995.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qv.newstarts.cn

[U11] Py：生成器表达式
来源：http://tu.lnxyls.cn

(x * 2 for x in arr)
来源：http://hy.lnxyls.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ty.jctech888.com.cn

Counter(arr).most_common(3)
来源：http://mo.haigaiapp.cn

[U13] Py：固定长度队列
来源：http://gy.newstarts.cn

deque(maxlen=10)
来源：http://mm.lnxyls.cn

[U14] Py：分组收集到列表
来源：http://yt.yuntaijiaju.cn

defaultdict(list)
来源：http://kf.huixiangedu.cn

[U15] Py：高精度计时
来源：http://ah.huanxung.cn

t = time.perf_counter()
来源：http://tx.huixiangedu.cn

[U16] Py：命令行参数解析
来源：http://jx.huanxung.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ph.muxihuayi.cn

[U17] Py：初始化日志
来源：http://eg.huixinmuqiang.cn

logging.basicConfig(level=logging.INFO)
来源：http://uh.nszjky.cn

[U18] Py：预编译正则
来源：http://aq.szsharing.cn

pat = re.compile(r"\d+")
来源：http://vt.lnxyls.cn

[U19] Py：正则替换带回调
来源：http://iy.shxzskj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kr.jianghongdianzi.cn

[U20] Py：缓存函数结果
来源：http://hd.shxzukj.cn

@functools.lru_cache(maxsize=None)
来源：http://lb.newstarts.cn

[U21] Py：自定义上下文管理器
来源：http://uh.szsharing.cn

@contextlib.contextmanager
来源：http://yc.shtwfgs.cn

[U22] Py：矩阵转置
来源：http://ri.gzmigu.cn

list(zip(*m))
来源：http://sw.haigaiapp.cn

[U23] Py：分块读取大文件
来源：http://ci.bjjhwx.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gc.newstarts.cn

[U24] Py：路径操作
来源：http://uf.jctech888.com.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ol.newstarts.cn

[U25] Py：CSV 按字典读
来源：http://cn.haigaiapp.cn

csv.DictReader(f)
来源：http://vw.shtwfgs.cn

[U26] Py：并发下载
来源：http://nj.jianghongdianzi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://it.shxzukj.cn

[U27] Py：异步 HTTP
来源：http://uk.panjiajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://us.gzmigu.cn

[U28] Py：类型别名
来源：http://mn.haigaiapp.cn

UserId = int
来源：http://mf.haigaiapp.cn

[U29] Py：属性校验
来源：http://nx.yuexingan06.cn

@property 与 @x.setter 配合
来源：http://gb.shxzskj.cn

[U30] Py：数据类
来源：http://gz.bookmarksfly.cn

@dataclass(slots=True)
来源：http://hl.9csxet.cn

[U31] Py：单测
来源：http://vb.shtwfgs.cn

python -m pytest -q
来源：http://yi.asd995.cn

[U32] Py：代码格式化
来源：http://xr.panjiajie.cn

ruff format . && ruff check --fix .
来源：http://nt.chemitech.net.cn

[U33] Py：打包发布
来源：http://nf.muxihuayi.cn

python -m build  （依赖 pyproject.toml）
来源：http://zq.huixinmuqiang.cn

[U34] Py：判断编码
来源：http://bl.yuntaijiaju.cn

chardet.detect(raw)
来源：http://ok.szsharing.cn

[U35] Py：发送邮件
来源：http://xe.nszjky.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mj.szxytkj.cn

[U36] Py：定时任务
来源：http://ag.521024.cn

schedule.every(10).minutes.do(job)
来源：http://pk.haigaiapp.cn

[U37] Py：读写 Excel
来源：http://ap.newstarts.cn

pandas.read_excel / DataFrame.to_excel
来源：http://cy.shxzukj.cn

[U38] Py：获取脚本所在目录
来源：http://tf.yuexingan06.cn

Path(__file__).resolve().parent
来源：http://gb.szsharing.cn

[U39] Py：判断是否在交互环境
来源：http://nk.huanxung.cn

sys.stdout.isatty()
来源：http://yq.shtwfgs.cn

[U40] Py：打印到标准错误
来源：http://nm.bookmarksfly.cn

print("err", file=sys.stderr)
来源：http://uo.panjiajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://xg.asd995.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gn.jctech888.com.cn

[U42] PHP：PSR-4 自动加载
来源：http://bk.huixinmuqiang.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cn.newstarts.cn

[U43] PHP：声明命名空间
来源：http://gk.jctech888.com.cn

namespace App\Http;
来源：http://ij.bookmarksfly.cn

[U44] PHP：开启严格类型
来源：http://cu.chemitech.net.cn

declare(strict_types=1);
来源：http://sl.bookmarksfly.cn

[U45] PHP：类型声明与返回类型
来源：http://fs.muxihuayi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://lx.yuexingan06.cn

[U46] PHP：可空类型
来源：http://nf.shxzskj.cn

?string $name = null
来源：http://gu.panjiajie.cn

[U47] PHP：联合类型
来源：http://qa.szxytkj.cn

int|string $id
来源：http://pj.bookmarksfly.cn

[U48] PHP：纯枚举
来源：http://nu.lnxyls.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nw.szxytkj.cn

[U49] PHP：只读属性
来源：http://iv.asd995.cn

public readonly string $name
来源：http://st.shxzskj.cn

[U50] PHP：构造器属性提升
来源：http://pc.szsharing.cn

public function __construct(private int $id) {}
来源：http://mu.hahajie.cn

[U51] PHP：数组解构
来源：http://ux.szxytkj.cn

[$a, $b] = $arr;
来源：http://zv.nszjky.cn

[U52] PHP：箭头函数
来源：http://po.wgjwhj.cn

$double = fn($x) => $x * 2;
来源：http://tg.nszjky.cn

[U53] PHP：空合并运算符
来源：http://et.hnjuh.cn

$v = $a ?? $b ?? "default";
来源：http://lk.shxzukj.cn

[U54] PHP：空安全调用
来源：http://xc.colortex.cn

$obj?->method()
来源：http://wr.jianghongdianzi.cn

[U55] PHP：match 表达式
来源：http://ob.huanxung.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ku.9csxet.cn

[U56] PHP：命名参数
来源：http://nv.bookmarksfly.cn

f(a: 1, b: 2)
来源：http://mr.lnxyls.cn

[U57] PHP：字符串插值
来源：http://lq.nszjky.cn

"值: {$a}"
来源：http://un.hahajie.cn

[U58] PHP：数组三件套
来源：http://kj.lnxyls.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://di.shxzskj.cn

[U59] PHP：自定义排序
来源：http://xv.panjiajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ew.yuexingan06.cn

[U60] PHP：JSON 编解码
来源：http://rq.shtwfgs.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ur.nszjky.cn

[U61] PHP：正则
来源：http://sm.lnxyls.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://so.huixiangedu.cn

[U62] PHP：日期对象
来源：http://zy.huixiangedu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://aq.newstarts.cn

[U63] PHP：文件读写
来源：http://oo.gzmigu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zq.hahajie.cn

[U64] PHP：目录遍历
来源：http://qo.jctech888.com.cn

glob("dir/*.php");  scandir("dir");
来源：http://on.9csxet.cn

[U65] PHP：会话
来源：http://mx.521024.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://fm.bookmarksfly.cn

[U66] PHP：设置 Cookie
来源：http://ht.shxzukj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pe.shxzskj.cn

[U67] PHP：处理文件上传
来源：http://rd.lnxyls.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://in.jctech888.com.cn

[U68] PHP：PDO 连接
来源：http://as.haigaiapp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ud.nszjky.cn

[U69] PHP：PDO 预处理
来源：http://gu.shxzukj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jx.lnxyls.cn

[U70] PHP：PDO 事务
来源：http://sp.nszjky.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gg.huixinmuqiang.cn

[U71] PHP：抛出异常
来源：http://gt.nicolike.cn

throw new RuntimeException("失败", 500);
来源：http://bk.shxzukj.cn

[U72] PHP：写错误日志
来源：http://ea.yuexingan06.cn

error_log("失败: " . $e->getMessage());
来源：http://td.yuexingan06.cn

[U73] PHP：读取 ini 配置
来源：http://yf.huanxung.cn

parse_ini_file("config.ini", true)
来源：http://et.521024.cn

[U74] PHP：读取环境变量
来源：http://wp.colortex.cn

getenv("APP_ENV") ?: "production"
来源：http://al.yuntaijiaju.cn

[U75] PHP：依赖注入
来源：http://wk.shxzskj.cn

composer require psr/container
来源：http://sc.huixinmuqiang.cn

[U76] PHP：简单路由
来源：http://xf.521024.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ct.bookmarksfly.cn

[U77] PHP：模板渲染
来源：http://pa.panjiajie.cn

composer require twig/twig
来源：http://zp.jianghongdianzi.cn

[U78] PHP：单元测试
来源：http://gb.521024.cn

composer require --dev phpunit/phpunit
来源：http://wt.huanxung.cn

[U79] PHP：静态分析
来源：http://mr.colortex.cn

composer require --dev phpstan/phpstan
来源：http://jp.lnxyls.cn

[U80] PHP：代码规范修复
来源：http://vh.bookmarksfly.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://km.hnjuh.cn

[U81] JS：初始化项目
来源：http://qu.asd995.cn

npm init -y;  npm i express
来源：http://qk.newstarts.cn

[U82] JS：package.json 脚本
来源：http://og.szsharing.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pn.lnxyls.cn


<!-- 参考信息 -->