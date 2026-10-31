代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://vw.yuexingan06.cn

[S59] C++：静态断言
来源：http://md.yuexingan06.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rf.shxzukj.cn

[S60] C++：遍历并删除元素
来源：http://pb.hahajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bn.bookmarksfly.cn

================================================================================
来源：http://ad.chemitech.net.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://sd.bookmarksfly.cn

================================================================================
来源：http://wn.yuexingan06.cn

[T01] Kotlin：Hello World
来源：http://fr.bookmarksfly.cn

println("Hello")
来源：http://kz.colortex.cn

[T02] Kotlin：变量
来源：http://bw.nicolike.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dj.9csxet.cn

[T03] Kotlin：字符串模板
来源：http://wm.szsharing.cn

"值: $b"
来源：http://mw.szsharing.cn

[T04] Kotlin：空安全
来源：http://xs.huanxung.cn

val n: String? = null;  n?.length
来源：http://uh.nszjky.cn

[T05] Kotlin：when 表达式
来源：http://oa.szxytkj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fh.nszjky.cn

[T06] Kotlin：集合映射
来源：http://my.panjiajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ay.hnjuh.cn

[T07] Kotlin：集合过滤
来源：http://hg.jctech888.com.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fo.szsharing.cn

[T08] Kotlin：数据类
来源：http://lb.9csxet.cn

data class User(val name: String, val age: Int)
来源：http://sz.newstarts.cn

[T09] Kotlin：扩展函数
来源：http://xm.521024.cn

fun String.exclaim() = this + "!"
来源：http://jv.521024.cn

[T10] Kotlin：默认参数
来源：http://mx.bookmarksfly.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ud.yuntaijiaju.cn

[T11] Kotlin：协程
来源：http://ze.huanxung.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ez.lnxyls.cn

[T12] Kotlin：解构声明
来源：http://kw.newstarts.cn

val (a, b) = Pair(1, 2)
来源：http://fv.huixiangedu.cn

[T13] Kotlin：只读 Map
来源：http://at.nszjky.cn

val m = mapOf("a" to 1)
来源：http://ap.hahajie.cn

[T14] Kotlin：循环
来源：http://wb.bjjhwx.cn

for (i in 1..10) println(i)
来源：http://kw.jianghongdianzi.cn

[T15] Kotlin：接口
来源：http://hc.shtwfgs.cn

interface Shape { fun area(): Double }
来源：http://fp.bjjhwx.cn

[T16] Swift：Hello World
来源：http://zz.yuexingan06.cn

print("Hello")
来源：http://uf.gzmigu.cn

[T17] Swift：变量与常量
来源：http://nb.colortex.cn

var a = 1;  let b = 2
来源：http://sm.chemitech.net.cn

[T18] Swift：字符串插值
来源：http://uf.szxytkj.cn

"值: \(b)"
来源：http://ij.panjiajie.cn

[T19] Swift：可选绑定
来源：http://cg.shxzukj.cn

if let n = opt { print(n) }
来源：http://bv.yuexingan06.cn

[T20] Swift：数组操作
来源：http://wl.szsharing.cn

var a = [1, 2, 3];  a.append(4)
来源：http://it.jctech888.com.cn

[T21] Swift：遍历
来源：http://ks.shxzukj.cn

for x in a { print(x) }
来源：http://xv.newstarts.cn

[T22] Swift：字典
来源：http://wc.szxytkj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://dr.colortex.cn

[T23] Swift：函数
来源：http://qn.yuntaijiaju.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wt.huanxung.cn

[T24] Swift：闭包
来源：http://qe.gzmigu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://go.colortex.cn

[T25] Swift：结构体
来源：http://mu.jctech888.com.cn

struct P { var x: Int }
来源：http://iz.hahajie.cn

[T26] Swift：类与重写
来源：http://ql.huanxung.cn

class A: Base { override func f() {} }
来源：http://ku.jctech888.com.cn

[T27] Swift：错误处理
来源：http://jv.huixinmuqiang.cn

do { try f() } catch { print(error) }
来源：http://ij.huixiangedu.cn

[T28] Swift：枚举
来源：http://tj.521024.cn

enum Color { case red, green }
来源：http://wt.panjiajie.cn

[T29] Swift：guard 提前返回
来源：http://on.huixiangedu.cn

guard let x = opt else { return }
来源：http://sr.yuexingan06.cn

[T30] Swift：协议
来源：http://ev.yuntaijiaju.cn

protocol Shape { func area() -> Double }
来源：http://bt.haigaiapp.cn

[T31] Lua：Hello World
来源：http://oc.bjjhwx.cn

print("Hello")
来源：http://qz.yuntaijiaju.cn

[T32] Lua：局部变量
来源：http://er.muxihuayi.cn

local a = 1
来源：http://vl.colortex.cn

[T33] Lua：表（数组）
来源：http://ts.haigaiapp.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://uh.bookmarksfly.cn

[T34] Lua：遍历表
来源：http://gf.gzmigu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://sa.szsharing.cn

[T35] Lua：字典表
来源：http://od.hahajie.cn

local d = { a = 1 };  d.b = 2
来源：http://lk.huixinmuqiang.cn

[T36] Lua：函数
来源：http://fm.bookmarksfly.cn

function add(a, b) return a + b end
来源：http://wh.shtwfgs.cn

[T37] Lua：字符串拼接
来源：http://hx.gzmigu.cn

"a" .. "b"
来源：http://tj.shxzukj.cn

[T38] Lua：条件
来源：http://uj.wgjwhj.cn

if x > 0 then print("正") end
来源：http://zy.szsharing.cn

[T39] Lua：模式匹配
来源：http://yj.gzmigu.cn

string.find(s, "%d+")
来源：http://ew.chemitech.net.cn

[T40] Lua：元表
来源：http://ih.nicolike.cn

setmetatable({}, { __index = base })
来源：http://ja.bjjhwx.cn

[T41] Perl：Hello World
来源：http://xh.521024.cn

print "Hello\n";
来源：http://it.shtwfgs.cn

[T42] Perl：变量类型
来源：http://te.lnxyls.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zf.hahajie.cn

[T43] Perl：字符串插值
来源：http://kn.bjjhwx.cn

"值: $a"
来源：http://ya.shxzukj.cn

[T44] Perl：条件
来源：http://jg.shxzukj.cn

if ($a > 0) { print "正"; }
来源：http://ra.huixiangedu.cn

[T45] Perl：数组遍历
来源：http://is.9csxet.cn

for my $x (@arr) { print $x; }
来源：http://xy.jctech888.com.cn

[T46] Perl：哈希操作
来源：http://cp.newstarts.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://un.szsharing.cn

[T47] Perl：正则捕获
来源：http://ns.hahajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://mw.newstarts.cn

[T48] Perl：正则替换
来源：http://ww.szsharing.cn

$s =~ s/old/new/g;
来源：http://vb.521024.cn

[T49] Perl：函数
来源：http://ab.asd995.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vv.nicolike.cn

[T50] Perl：逐行读文件
来源：http://qz.chemitech.net.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://lj.hnjuh.cn

while (my $line = <$fh>) { print $line; }
来源：http://ih.521024.cn

[T51] Scala：Hello World
来源：http://wi.nicolike.cn

println("Hello")
来源：http://fl.gzmigu.cn

[T52] Scala：变量
来源：http://ex.huanxung.cn

val a = 1;  var b = 2
来源：http://rc.newstarts.cn

[T53] Scala：字符串插值
来源：http://ug.asd995.cn

s"值: $b"
来源：http://tt.szxytkj.cn

[T54] Scala：集合映射
来源：http://ra.jctech888.com.cn

List(1, 2, 3).map(_ * 2)
来源：http://me.panjiajie.cn

[T55] Scala：集合过滤
来源：http://nh.asd995.cn

List(1, 2, 3).filter(_ > 1)
来源：http://kj.shtwfgs.cn

[T56] Scala：样例类
来源：http://jg.yuntaijiaju.cn

case class User(name: String, age: Int)
来源：http://zb.asd995.cn

[T57] Scala：模式匹配
来源：http://tx.szxytkj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ye.yuntaijiaju.cn

[T58] Scala：函数定义
来源：http://bh.bookmarksfly.cn

def add(a: Int, b: Int): Int = a + b
来源：http://iw.nszjky.cn

[T59] Scala：循环
来源：http://ym.shtwfgs.cn

for (i <- 1 to 10) println(i)
来源：http://zz.wgjwhj.cn

[T60] Scala：折叠
来源：http://gj.newstarts.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dc.huixinmuqiang.cn

================================================================================
来源：http://ri.shtwfgs.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kr.jianghongdianzi.cn

================================================================================
来源：http://ss.lnxyls.cn

[U01] Py：创建虚拟环境
来源：http://oq.nicolike.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ca.szxytkj.cn

[U02] Py：导出 / 安装依赖
来源：http://ka.9csxet.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yo.panjiajie.cn

[U03] Py：加载 .env 配置
来源：http://dz.szxytkj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://in.huixiangedu.cn

[U04] Py：变量调试打印
来源：http://ts.huixinmuqiang.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rw.panjiajie.cn

[U05] Py：列表去重且保序
来源：http://yc.521024.cn

list(dict.fromkeys(arr))
来源：http://ep.jianghongdianzi.cn

[U06] Py：合并两个字典
来源：http://hk.szsharing.cn

{**a, **b}
来源：http://li.hahajie.cn

[U07] Py：反转字典键值
来源：http://fe.shxzskj.cn

{v: k for k, v in d.items()}
来源：http://mc.jctech888.com.cn

[U08] Py：展平二维列表
来源：http://qa.9csxet.cn

[y for x in nested for y in x]
来源：http://bc.gzmigu.cn

[U09] Py：字典取最大值的键
来源：http://mk.yuexingan06.cn

max(d, key=d.get)
来源：http://xx.huanxung.cn

[U10] Py：按值排序字典
来源：http://vt.shxzukj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hk.hahajie.cn

[U11] Py：生成器表达式
来源：http://fd.shxzskj.cn

(x * 2 for x in arr)
来源：http://kf.hahajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://fs.shxzskj.cn

Counter(arr).most_common(3)
来源：http://nc.hnjuh.cn

[U13] Py：固定长度队列
来源：http://it.yuntaijiaju.cn

deque(maxlen=10)
来源：http://dn.huixinmuqiang.cn

[U14] Py：分组收集到列表
来源：http://or.gzmigu.cn

defaultdict(list)
来源：http://lq.gzmigu.cn

[U15] Py：高精度计时
来源：http://go.shxzukj.cn

t = time.perf_counter()
来源：http://iz.muxihuayi.cn

[U16] Py：命令行参数解析
来源：http://eo.lnxyls.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tq.shxzskj.cn

[U17] Py：初始化日志
来源：http://yx.jianghongdianzi.cn

logging.basicConfig(level=logging.INFO)
来源：http://em.huixiangedu.cn

[U18] Py：预编译正则
来源：http://na.huanxung.cn

pat = re.compile(r"\d+")
来源：http://rm.huanxung.cn

[U19] Py：正则替换带回调
来源：http://dt.lnxyls.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://aw.huixiangedu.cn

[U20] Py：缓存函数结果
来源：http://jb.shxzukj.cn

@functools.lru_cache(maxsize=None)
来源：http://cn.jianghongdianzi.cn

[U21] Py：自定义上下文管理器
来源：http://wb.hnjuh.cn

@contextlib.contextmanager
来源：http://rq.shxzukj.cn

[U22] Py：矩阵转置
来源：http://nu.panjiajie.cn

list(zip(*m))
来源：http://pc.shxzskj.cn

[U23] Py：分块读取大文件
来源：http://aq.colortex.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cw.gzmigu.cn

[U24] Py：路径操作
来源：http://or.muxihuayi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fq.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://xr.newstarts.cn

csv.DictReader(f)
来源：http://pp.shtwfgs.cn

[U26] Py：并发下载
来源：http://fp.jianghongdianzi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jp.chemitech.net.cn

[U27] Py：异步 HTTP
来源：http://fv.shxzukj.cn

aiohttp.ClientSession() 配合 async with
来源：http://rr.nszjky.cn

[U28] Py：类型别名
来源：http://xk.huanxung.cn

UserId = int
来源：http://eb.shxzskj.cn

[U29] Py：属性校验
来源：http://zw.521024.cn

@property 与 @x.setter 配合
来源：http://dj.hahajie.cn

[U30] Py：数据类
来源：http://sh.521024.cn

@dataclass(slots=True)
来源：http://ww.shtwfgs.cn

[U31] Py：单测
来源：http://ri.gzmigu.cn

python -m pytest -q
来源：http://ot.huanxung.cn

[U32] Py：代码格式化
来源：http://hh.jianghongdianzi.cn

ruff format . && ruff check --fix .
来源：http://tf.szsharing.cn

[U33] Py：打包发布
来源：http://ti.newstarts.cn

python -m build  （依赖 pyproject.toml）
来源：http://py.huanxung.cn

[U34] Py：判断编码
来源：http://tr.muxihuayi.cn

chardet.detect(raw)
来源：http://dh.nicolike.cn

[U35] Py：发送邮件
来源：http://hp.bjjhwx.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yb.haigaiapp.cn

[U36] Py：定时任务
来源：http://ke.521024.cn

schedule.every(10).minutes.do(job)
来源：http://qj.huanxung.cn

[U37] Py：读写 Excel
来源：http://kz.huanxung.cn

pandas.read_excel / DataFrame.to_excel
来源：http://bg.newstarts.cn

[U38] Py：获取脚本所在目录
来源：http://yf.bookmarksfly.cn

Path(__file__).resolve().parent
来源：http://ne.huixiangedu.cn

[U39] Py：判断是否在交互环境
来源：http://pm.jctech888.com.cn

sys.stdout.isatty()
来源：http://mq.chemitech.net.cn

[U40] Py：打印到标准错误
来源：http://vx.jianghongdianzi.cn

print("err", file=sys.stderr)
来源：http://ae.9csxet.cn

[U41] PHP：初始化 Composer 项目
来源：http://lw.colortex.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://uu.szsharing.cn

[U42] PHP：PSR-4 自动加载
来源：http://pl.hahajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cy.szsharing.cn

[U43] PHP：声明命名空间
来源：http://xl.huixinmuqiang.cn

namespace App\Http;
来源：http://yn.haigaiapp.cn

[U44] PHP：开启严格类型
来源：http://ly.huixiangedu.cn

declare(strict_types=1);
来源：http://dg.yuntaijiaju.cn

[U45] PHP：类型声明与返回类型
来源：http://lh.hahajie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://gr.newstarts.cn

[U46] PHP：可空类型
来源：http://ds.huixiangedu.cn

?string $name = null
来源：http://zh.shxzskj.cn

[U47] PHP：联合类型
来源：http://cv.huixinmuqiang.cn

int|string $id
来源：http://tg.521024.cn

[U48] PHP：纯枚举
来源：http://mt.szxytkj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fo.colortex.cn

[U49] PHP：只读属性
来源：http://go.9csxet.cn

public readonly string $name
来源：http://tv.huixiangedu.cn

[U50] PHP：构造器属性提升
来源：http://ui.bjjhwx.cn

public function __construct(private int $id) {}
来源：http://xj.huanxung.cn

[U51] PHP：数组解构
来源：http://wh.hnjuh.cn

[$a, $b] = $arr;
来源：http://uz.asd995.cn

[U52] PHP：箭头函数
来源：http://tk.chemitech.net.cn

$double = fn($x) => $x * 2;
来源：http://yh.wgjwhj.cn

[U53] PHP：空合并运算符
来源：http://ky.yuexingan06.cn

$v = $a ?? $b ?? "default";
来源：http://wp.shtwfgs.cn

[U54] PHP：空安全调用
来源：http://kr.gzmigu.cn

$obj?->method()
来源：http://to.chemitech.net.cn

[U55] PHP：match 表达式
来源：http://vo.gzmigu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kr.shxzskj.cn

[U56] PHP：命名参数
来源：http://nm.hahajie.cn

f(a: 1, b: 2)
来源：http://jq.hnjuh.cn

[U57] PHP：字符串插值
来源：http://av.muxihuayi.cn

"值: {$a}"
来源：http://sn.hnjuh.cn

[U58] PHP：数组三件套
来源：http://hu.panjiajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jv.muxihuayi.cn

[U59] PHP：自定义排序
来源：http://sr.huixiangedu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://za.szxytkj.cn

[U60] PHP：JSON 编解码
来源：http://xj.huixiangedu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wr.bookmarksfly.cn

[U61] PHP：正则
来源：http://eh.asd995.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ei.huanxung.cn

[U62] PHP：日期对象
来源：http://da.bookmarksfly.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bc.szxytkj.cn

[U63] PHP：文件读写
来源：http://mh.colortex.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fx.hnjuh.cn

[U64] PHP：目录遍历
来源：http://yp.gzmigu.cn

glob("dir/*.php");  scandir("dir");
来源：http://kl.szxytkj.cn

[U65] PHP：会话
来源：http://rg.shxzskj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://py.nszjky.cn

[U66] PHP：设置 Cookie
来源：http://ce.9csxet.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bo.bookmarksfly.cn

[U67] PHP：处理文件上传
来源：http://vi.chemitech.net.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jo.szsharing.cn

[U68] PHP：PDO 连接
来源：http://gf.jctech888.com.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cf.wgjwhj.cn

[U69] PHP：PDO 预处理
来源：http://gl.lnxyls.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bx.hahajie.cn

[U70] PHP：PDO 事务
来源：http://hd.nszjky.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ty.hahajie.cn

[U71] PHP：抛出异常
来源：http://bi.shxzskj.cn

throw new RuntimeException("失败", 500);
来源：http://ww.hahajie.cn

[U72] PHP：写错误日志
来源：http://pm.jianghongdianzi.cn

error_log("失败: " . $e->getMessage());
来源：http://he.szxytkj.cn

[U73] PHP：读取 ini 配置
来源：http://th.hahajie.cn

parse_ini_file("config.ini", true)
来源：http://ps.newstarts.cn

[U74] PHP：读取环境变量
来源：http://ib.jctech888.com.cn

getenv("APP_ENV") ?: "production"
来源：http://px.bjjhwx.cn

[U75] PHP：依赖注入
来源：http://ui.asd995.cn

composer require psr/container
来源：http://lb.bookmarksfly.cn

[U76] PHP：简单路由
来源：http://qd.chemitech.net.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cn.shxzskj.cn

[U77] PHP：模板渲染
来源：http://mb.yuexingan06.cn

composer require twig/twig
来源：http://hu.huanxung.cn

[U78] PHP：单元测试
来源：http://it.wgjwhj.cn

composer require --dev phpunit/phpunit
来源：http://lv.hnjuh.cn

[U79] PHP：静态分析
来源：http://br.muxihuayi.cn

composer require --dev phpstan/phpstan
来源：http://jx.521024.cn

[U80] PHP：代码规范修复
来源：http://zf.bookmarksfly.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://rm.chemitech.net.cn

[U81] JS：初始化项目
来源：http://fw.shtwfgs.cn

npm init -y;  npm i express
来源：http://kc.newstarts.cn

[U82] JS：package.json 脚本
来源：http://ir.newstarts.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yw.huixiangedu.cn

[U83] JS：ES Module 导入导出
来源：http://gl.yuntaijiaju.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zt.shxzukj.cn

[U84] JS：CommonJS 写法
来源：http://ml.bjjhwx.cn

module.exports = { a };  const { a } = require("./m");
来源：http://fr.muxihuayi.cn


<!-- 参考信息 -->