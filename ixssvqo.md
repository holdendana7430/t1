代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://np.hnjuh.cn

[S57] C++：编译期常量
来源：http://al.colortex.cn

constexpr int N = 10;
来源：http://sh.bjjhwx.cn

[S58] C++：命名空间
来源：http://zn.szsharing.cn

namespace ns { int f() { return 1; } }
来源：http://og.lnxyls.cn

[S59] C++：静态断言
来源：http://je.lnxyls.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lh.jianghongdianzi.cn

[S60] C++：遍历并删除元素
来源：http://ul.gzmigu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ha.panjiajie.cn

================================================================================
来源：http://us.huixinmuqiang.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://do.nszjky.cn

================================================================================
来源：http://dz.huixiangedu.cn

[T01] Kotlin：Hello World
来源：http://ou.colortex.cn

println("Hello")
来源：http://tt.szsharing.cn

[T02] Kotlin：变量
来源：http://vo.panjiajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://iu.jctech888.com.cn

[T03] Kotlin：字符串模板
来源：http://fq.jctech888.com.cn

"值: $b"
来源：http://cs.nicolike.cn

[T04] Kotlin：空安全
来源：http://dj.szxytkj.cn

val n: String? = null;  n?.length
来源：http://pc.shxzukj.cn

[T05] Kotlin：when 表达式
来源：http://er.jctech888.com.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xg.panjiajie.cn

[T06] Kotlin：集合映射
来源：http://oy.gzmigu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://cx.asd995.cn

[T07] Kotlin：集合过滤
来源：http://br.hnjuh.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vk.shxzukj.cn

[T08] Kotlin：数据类
来源：http://yz.szxytkj.cn

data class User(val name: String, val age: Int)
来源：http://mp.chemitech.net.cn

[T09] Kotlin：扩展函数
来源：http://sf.newstarts.cn

fun String.exclaim() = this + "!"
来源：http://xx.bjjhwx.cn

[T10] Kotlin：默认参数
来源：http://mc.huixiangedu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ge.yuexingan06.cn

[T11] Kotlin：协程
来源：http://sy.9csxet.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vj.colortex.cn

[T12] Kotlin：解构声明
来源：http://zf.jianghongdianzi.cn

val (a, b) = Pair(1, 2)
来源：http://ol.gzmigu.cn

[T13] Kotlin：只读 Map
来源：http://ac.gzmigu.cn

val m = mapOf("a" to 1)
来源：http://od.haigaiapp.cn

[T14] Kotlin：循环
来源：http://ou.szxytkj.cn

for (i in 1..10) println(i)
来源：http://kz.panjiajie.cn

[T15] Kotlin：接口
来源：http://od.haigaiapp.cn

interface Shape { fun area(): Double }
来源：http://uh.jianghongdianzi.cn

[T16] Swift：Hello World
来源：http://ha.yuntaijiaju.cn

print("Hello")
来源：http://jr.gzmigu.cn

[T17] Swift：变量与常量
来源：http://ah.muxihuayi.cn

var a = 1;  let b = 2
来源：http://mu.huixiangedu.cn

[T18] Swift：字符串插值
来源：http://fj.nszjky.cn

"值: \(b)"
来源：http://kx.shxzskj.cn

[T19] Swift：可选绑定
来源：http://qg.hahajie.cn

if let n = opt { print(n) }
来源：http://jt.huixiangedu.cn

[T20] Swift：数组操作
来源：http://fa.jctech888.com.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xa.szsharing.cn

[T21] Swift：遍历
来源：http://av.wgjwhj.cn

for x in a { print(x) }
来源：http://vy.newstarts.cn

[T22] Swift：字典
来源：http://cu.hahajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://kg.panjiajie.cn

[T23] Swift：函数
来源：http://eb.colortex.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://md.haigaiapp.cn

[T24] Swift：闭包
来源：http://oj.huanxung.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://bz.gzmigu.cn

[T25] Swift：结构体
来源：http://ai.521024.cn

struct P { var x: Int }
来源：http://kz.yuexingan06.cn

[T26] Swift：类与重写
来源：http://ur.chemitech.net.cn

class A: Base { override func f() {} }
来源：http://tf.bjjhwx.cn

[T27] Swift：错误处理
来源：http://dv.521024.cn

do { try f() } catch { print(error) }
来源：http://td.521024.cn

[T28] Swift：枚举
来源：http://hh.szsharing.cn

enum Color { case red, green }
来源：http://ta.521024.cn

[T29] Swift：guard 提前返回
来源：http://gp.yuntaijiaju.cn

guard let x = opt else { return }
来源：http://uo.9csxet.cn

[T30] Swift：协议
来源：http://xr.colortex.cn

protocol Shape { func area() -> Double }
来源：http://zo.wgjwhj.cn

[T31] Lua：Hello World
来源：http://zw.szxytkj.cn

print("Hello")
来源：http://en.huixinmuqiang.cn

[T32] Lua：局部变量
来源：http://pn.521024.cn

local a = 1
来源：http://mt.9csxet.cn

[T33] Lua：表（数组）
来源：http://tv.9csxet.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://gq.hnjuh.cn

[T34] Lua：遍历表
来源：http://oo.huanxung.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://nl.haigaiapp.cn

[T35] Lua：字典表
来源：http://zy.bjjhwx.cn

local d = { a = 1 };  d.b = 2
来源：http://uu.jctech888.com.cn

[T36] Lua：函数
来源：http://jp.yuexingan06.cn

function add(a, b) return a + b end
来源：http://fb.chemitech.net.cn

[T37] Lua：字符串拼接
来源：http://ck.jianghongdianzi.cn

"a" .. "b"
来源：http://dd.huanxung.cn

[T38] Lua：条件
来源：http://kl.nicolike.cn

if x > 0 then print("正") end
来源：http://vr.nszjky.cn

[T39] Lua：模式匹配
来源：http://aj.colortex.cn

string.find(s, "%d+")
来源：http://xl.nszjky.cn

[T40] Lua：元表
来源：http://kg.newstarts.cn

setmetatable({}, { __index = base })
来源：http://kw.huixinmuqiang.cn

[T41] Perl：Hello World
来源：http://wy.shxzukj.cn

print "Hello\n";
来源：http://ju.szxytkj.cn

[T42] Perl：变量类型
来源：http://fd.yuntaijiaju.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rl.haigaiapp.cn

[T43] Perl：字符串插值
来源：http://ig.chemitech.net.cn

"值: $a"
来源：http://sa.9csxet.cn

[T44] Perl：条件
来源：http://hk.shxzukj.cn

if ($a > 0) { print "正"; }
来源：http://hg.szxytkj.cn

[T45] Perl：数组遍历
来源：http://ka.nicolike.cn

for my $x (@arr) { print $x; }
来源：http://yo.szxytkj.cn

[T46] Perl：哈希操作
来源：http://uc.huixiangedu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gb.hahajie.cn

[T47] Perl：正则捕获
来源：http://sl.huixiangedu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vl.hnjuh.cn

[T48] Perl：正则替换
来源：http://df.jianghongdianzi.cn

$s =~ s/old/new/g;
来源：http://zq.521024.cn

[T49] Perl：函数
来源：http://er.yuntaijiaju.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ri.yuntaijiaju.cn

[T50] Perl：逐行读文件
来源：http://vr.nicolike.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ol.panjiajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://mk.bjjhwx.cn

[T51] Scala：Hello World
来源：http://su.yuexingan06.cn

println("Hello")
来源：http://up.gzmigu.cn

[T52] Scala：变量
来源：http://gv.shtwfgs.cn

val a = 1;  var b = 2
来源：http://qc.nicolike.cn

[T53] Scala：字符串插值
来源：http://hq.gzmigu.cn

s"值: $b"
来源：http://jm.bookmarksfly.cn

[T54] Scala：集合映射
来源：http://wl.521024.cn

List(1, 2, 3).map(_ * 2)
来源：http://um.nszjky.cn

[T55] Scala：集合过滤
来源：http://ji.huixiangedu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xs.colortex.cn

[T56] Scala：样例类
来源：http://vd.yuexingan06.cn

case class User(name: String, age: Int)
来源：http://da.shtwfgs.cn

[T57] Scala：模式匹配
来源：http://fr.asd995.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://pj.hnjuh.cn

[T58] Scala：函数定义
来源：http://jg.wgjwhj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ng.wgjwhj.cn

[T59] Scala：循环
来源：http://tl.haigaiapp.cn

for (i <- 1 to 10) println(i)
来源：http://xx.huixiangedu.cn

[T60] Scala：折叠
来源：http://ul.521024.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rv.szxytkj.cn

================================================================================
来源：http://eq.bookmarksfly.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lm.jianghongdianzi.cn

================================================================================
来源：http://kt.huanxung.cn

[U01] Py：创建虚拟环境
来源：http://rp.hahajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://gd.huixiangedu.cn

[U02] Py：导出 / 安装依赖
来源：http://ow.nszjky.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fc.huanxung.cn

[U03] Py：加载 .env 配置
来源：http://lm.newstarts.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ug.wgjwhj.cn

[U04] Py：变量调试打印
来源：http://qj.colortex.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ds.newstarts.cn

[U05] Py：列表去重且保序
来源：http://hi.huixiangedu.cn

list(dict.fromkeys(arr))
来源：http://yd.hahajie.cn

[U06] Py：合并两个字典
来源：http://wc.wgjwhj.cn

{**a, **b}
来源：http://kk.asd995.cn

[U07] Py：反转字典键值
来源：http://vz.hahajie.cn

{v: k for k, v in d.items()}
来源：http://kz.hnjuh.cn

[U08] Py：展平二维列表
来源：http://br.yuntaijiaju.cn

[y for x in nested for y in x]
来源：http://tn.haigaiapp.cn

[U09] Py：字典取最大值的键
来源：http://hk.huanxung.cn

max(d, key=d.get)
来源：http://xa.yuntaijiaju.cn

[U10] Py：按值排序字典
来源：http://vi.nszjky.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://df.szsharing.cn

[U11] Py：生成器表达式
来源：http://rp.panjiajie.cn

(x * 2 for x in arr)
来源：http://wt.szxytkj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rj.huanxung.cn

Counter(arr).most_common(3)
来源：http://ii.bjjhwx.cn

[U13] Py：固定长度队列
来源：http://ir.asd995.cn

deque(maxlen=10)
来源：http://vm.hnjuh.cn

[U14] Py：分组收集到列表
来源：http://tl.lnxyls.cn

defaultdict(list)
来源：http://ye.lnxyls.cn

[U15] Py：高精度计时
来源：http://vx.shtwfgs.cn

t = time.perf_counter()
来源：http://oz.hahajie.cn

[U16] Py：命令行参数解析
来源：http://ev.shxzukj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://js.bjjhwx.cn

[U17] Py：初始化日志
来源：http://me.bjjhwx.cn

logging.basicConfig(level=logging.INFO)
来源：http://hf.yuntaijiaju.cn

[U18] Py：预编译正则
来源：http://fq.jianghongdianzi.cn

pat = re.compile(r"\d+")
来源：http://xl.newstarts.cn

[U19] Py：正则替换带回调
来源：http://fq.jctech888.com.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ym.521024.cn

[U20] Py：缓存函数结果
来源：http://ea.haigaiapp.cn

@functools.lru_cache(maxsize=None)
来源：http://iz.gzmigu.cn

[U21] Py：自定义上下文管理器
来源：http://yi.wgjwhj.cn

@contextlib.contextmanager
来源：http://it.panjiajie.cn

[U22] Py：矩阵转置
来源：http://zc.shxzskj.cn

list(zip(*m))
来源：http://gm.9csxet.cn

[U23] Py：分块读取大文件
来源：http://mg.chemitech.net.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dw.521024.cn

[U24] Py：路径操作
来源：http://oi.yuntaijiaju.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://in.nszjky.cn

[U25] Py：CSV 按字典读
来源：http://ms.9csxet.cn

csv.DictReader(f)
来源：http://cv.huixinmuqiang.cn

[U26] Py：并发下载
来源：http://yl.shtwfgs.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jg.lnxyls.cn

[U27] Py：异步 HTTP
来源：http://zo.hnjuh.cn

aiohttp.ClientSession() 配合 async with
来源：http://in.shtwfgs.cn

[U28] Py：类型别名
来源：http://eq.haigaiapp.cn

UserId = int
来源：http://xu.nicolike.cn

[U29] Py：属性校验
来源：http://rr.hnjuh.cn

@property 与 @x.setter 配合
来源：http://wx.szsharing.cn

[U30] Py：数据类
来源：http://ur.asd995.cn

@dataclass(slots=True)
来源：http://wv.shxzskj.cn

[U31] Py：单测
来源：http://nu.hahajie.cn

python -m pytest -q
来源：http://bh.lnxyls.cn

[U32] Py：代码格式化
来源：http://hz.shtwfgs.cn

ruff format . && ruff check --fix .
来源：http://rr.hnjuh.cn

[U33] Py：打包发布
来源：http://uz.huanxung.cn

python -m build  （依赖 pyproject.toml）
来源：http://il.shxzskj.cn

[U34] Py：判断编码
来源：http://pm.newstarts.cn

chardet.detect(raw)
来源：http://zy.newstarts.cn

[U35] Py：发送邮件
来源：http://ll.lnxyls.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mr.asd995.cn

[U36] Py：定时任务
来源：http://yv.jctech888.com.cn

schedule.every(10).minutes.do(job)
来源：http://ke.wgjwhj.cn

[U37] Py：读写 Excel
来源：http://te.colortex.cn

pandas.read_excel / DataFrame.to_excel
来源：http://nl.huixinmuqiang.cn

[U38] Py：获取脚本所在目录
来源：http://fy.wgjwhj.cn

Path(__file__).resolve().parent
来源：http://jh.huanxung.cn

[U39] Py：判断是否在交互环境
来源：http://jj.jianghongdianzi.cn

sys.stdout.isatty()
来源：http://tb.9csxet.cn

[U40] Py：打印到标准错误
来源：http://rz.9csxet.cn

print("err", file=sys.stderr)
来源：http://cy.wgjwhj.cn

[U41] PHP：初始化 Composer 项目
来源：http://uy.wgjwhj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://wb.haigaiapp.cn

[U42] PHP：PSR-4 自动加载
来源：http://ai.gzmigu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pw.newstarts.cn

[U43] PHP：声明命名空间
来源：http://sj.lnxyls.cn

namespace App\Http;
来源：http://ud.wgjwhj.cn

[U44] PHP：开启严格类型
来源：http://wb.shtwfgs.cn

declare(strict_types=1);
来源：http://jw.gzmigu.cn

[U45] PHP：类型声明与返回类型
来源：http://ey.hahajie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://zd.521024.cn

[U46] PHP：可空类型
来源：http://ry.521024.cn

?string $name = null
来源：http://um.panjiajie.cn

[U47] PHP：联合类型
来源：http://eo.colortex.cn

int|string $id
来源：http://zf.bjjhwx.cn

[U48] PHP：纯枚举
来源：http://fs.huanxung.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pg.nicolike.cn

[U49] PHP：只读属性
来源：http://kh.nicolike.cn

public readonly string $name
来源：http://em.yuntaijiaju.cn

[U50] PHP：构造器属性提升
来源：http://we.yuexingan06.cn

public function __construct(private int $id) {}
来源：http://uj.521024.cn

[U51] PHP：数组解构
来源：http://ul.panjiajie.cn

[$a, $b] = $arr;
来源：http://kn.szsharing.cn

[U52] PHP：箭头函数
来源：http://ew.huixiangedu.cn

$double = fn($x) => $x * 2;
来源：http://vb.colortex.cn

[U53] PHP：空合并运算符
来源：http://ia.bjjhwx.cn

$v = $a ?? $b ?? "default";
来源：http://oi.huanxung.cn

[U54] PHP：空安全调用
来源：http://jj.jianghongdianzi.cn

$obj?->method()
来源：http://sv.asd995.cn

[U55] PHP：match 表达式
来源：http://hg.huixinmuqiang.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uh.nszjky.cn

[U56] PHP：命名参数
来源：http://zo.szsharing.cn

f(a: 1, b: 2)
来源：http://ed.hahajie.cn

[U57] PHP：字符串插值
来源：http://nx.hnjuh.cn

"值: {$a}"
来源：http://rh.szsharing.cn

[U58] PHP：数组三件套
来源：http://ki.muxihuayi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ot.huixiangedu.cn

[U59] PHP：自定义排序
来源：http://am.hahajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://no.asd995.cn

[U60] PHP：JSON 编解码
来源：http://nn.chemitech.net.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ye.szsharing.cn

[U61] PHP：正则
来源：http://yz.yuntaijiaju.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zs.szxytkj.cn

[U62] PHP：日期对象
来源：http://ve.colortex.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://oh.newstarts.cn

[U63] PHP：文件读写
来源：http://dr.yuexingan06.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vg.huixiangedu.cn

[U64] PHP：目录遍历
来源：http://tm.panjiajie.cn

glob("dir/*.php");  scandir("dir");
来源：http://vf.shxzukj.cn

[U65] PHP：会话
来源：http://om.shtwfgs.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://uk.szsharing.cn

[U66] PHP：设置 Cookie
来源：http://sb.shxzskj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rl.wgjwhj.cn

[U67] PHP：处理文件上传
来源：http://us.shtwfgs.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kh.colortex.cn

[U68] PHP：PDO 连接
来源：http://yz.szsharing.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ir.szxytkj.cn

[U69] PHP：PDO 预处理
来源：http://rx.asd995.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tz.muxihuayi.cn

[U70] PHP：PDO 事务
来源：http://sl.jctech888.com.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qj.gzmigu.cn

[U71] PHP：抛出异常
来源：http://sd.bjjhwx.cn

throw new RuntimeException("失败", 500);
来源：http://jo.muxihuayi.cn

[U72] PHP：写错误日志
来源：http://uz.shtwfgs.cn

error_log("失败: " . $e->getMessage());
来源：http://br.asd995.cn

[U73] PHP：读取 ini 配置
来源：http://yr.asd995.cn

parse_ini_file("config.ini", true)
来源：http://oe.shtwfgs.cn

[U74] PHP：读取环境变量
来源：http://jo.hnjuh.cn

getenv("APP_ENV") ?: "production"
来源：http://zs.jianghongdianzi.cn

[U75] PHP：依赖注入
来源：http://ps.asd995.cn

composer require psr/container
来源：http://xt.panjiajie.cn

[U76] PHP：简单路由
来源：http://gt.yuexingan06.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tj.huanxung.cn

[U77] PHP：模板渲染
来源：http://bc.asd995.cn

composer require twig/twig
来源：http://fl.bjjhwx.cn

[U78] PHP：单元测试
来源：http://iu.colortex.cn

composer require --dev phpunit/phpunit
来源：http://ah.huanxung.cn

[U79] PHP：静态分析
来源：http://lv.wgjwhj.cn

composer require --dev phpstan/phpstan
来源：http://nk.hahajie.cn

[U80] PHP：代码规范修复
来源：http://vm.muxihuayi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://lo.yuntaijiaju.cn

[U81] JS：初始化项目
来源：http://kw.wgjwhj.cn

npm init -y;  npm i express
来源：http://wj.shtwfgs.cn

[U82] JS：package.json 脚本
来源：http://jx.shxzukj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ew.shxzukj.cn


<!-- 参考信息 -->