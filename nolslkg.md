代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://rg.9csxet.cn

[S59] C++：静态断言
来源：http://xt.jctech888.com.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://di.yuexingan06.cn

[S60] C++：遍历并删除元素
来源：http://hx.9csxet.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hn.shxzukj.cn

================================================================================
来源：http://io.hahajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hw.newstarts.cn

================================================================================
来源：http://wm.521024.cn

[T01] Kotlin：Hello World
来源：http://rs.chemitech.net.cn

println("Hello")
来源：http://ls.huixinmuqiang.cn

[T02] Kotlin：变量
来源：http://pc.hnjuh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ly.huixinmuqiang.cn

[T03] Kotlin：字符串模板
来源：http://ub.shtwfgs.cn

"值: $b"
来源：http://gt.shxzukj.cn

[T04] Kotlin：空安全
来源：http://ze.bjjhwx.cn

val n: String? = null;  n?.length
来源：http://eq.hnjuh.cn

[T05] Kotlin：when 表达式
来源：http://zg.hahajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xo.bookmarksfly.cn

[T06] Kotlin：集合映射
来源：http://ej.haigaiapp.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://wp.jianghongdianzi.cn

[T07] Kotlin：集合过滤
来源：http://ki.huixinmuqiang.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wl.shxzskj.cn

[T08] Kotlin：数据类
来源：http://dd.shtwfgs.cn

data class User(val name: String, val age: Int)
来源：http://ya.newstarts.cn

[T09] Kotlin：扩展函数
来源：http://sp.yuntaijiaju.cn

fun String.exclaim() = this + "!"
来源：http://ws.nicolike.cn

[T10] Kotlin：默认参数
来源：http://kq.yuexingan06.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://fq.gzmigu.cn

[T11] Kotlin：协程
来源：http://et.asd995.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://kj.panjiajie.cn

[T12] Kotlin：解构声明
来源：http://ok.hahajie.cn

val (a, b) = Pair(1, 2)
来源：http://ej.asd995.cn

[T13] Kotlin：只读 Map
来源：http://lc.jctech888.com.cn

val m = mapOf("a" to 1)
来源：http://md.bjjhwx.cn

[T14] Kotlin：循环
来源：http://dl.szsharing.cn

for (i in 1..10) println(i)
来源：http://bm.shxzukj.cn

[T15] Kotlin：接口
来源：http://yj.hahajie.cn

interface Shape { fun area(): Double }
来源：http://lb.hahajie.cn

[T16] Swift：Hello World
来源：http://nm.nszjky.cn

print("Hello")
来源：http://eh.nszjky.cn

[T17] Swift：变量与常量
来源：http://py.asd995.cn

var a = 1;  let b = 2
来源：http://ip.haigaiapp.cn

[T18] Swift：字符串插值
来源：http://zc.hnjuh.cn

"值: \(b)"
来源：http://ld.gzmigu.cn

[T19] Swift：可选绑定
来源：http://om.huixinmuqiang.cn

if let n = opt { print(n) }
来源：http://gb.szsharing.cn

[T20] Swift：数组操作
来源：http://jd.bookmarksfly.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ye.huanxung.cn

[T21] Swift：遍历
来源：http://ok.shxzskj.cn

for x in a { print(x) }
来源：http://nd.lnxyls.cn

[T22] Swift：字典
来源：http://ei.nszjky.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vf.muxihuayi.cn

[T23] Swift：函数
来源：http://ff.hnjuh.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://km.panjiajie.cn

[T24] Swift：闭包
来源：http://ng.szxytkj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://kg.huixiangedu.cn

[T25] Swift：结构体
来源：http://jb.yuexingan06.cn

struct P { var x: Int }
来源：http://lc.huixiangedu.cn

[T26] Swift：类与重写
来源：http://sc.colortex.cn

class A: Base { override func f() {} }
来源：http://nw.muxihuayi.cn

[T27] Swift：错误处理
来源：http://gk.chemitech.net.cn

do { try f() } catch { print(error) }
来源：http://ro.chemitech.net.cn

[T28] Swift：枚举
来源：http://ou.huanxung.cn

enum Color { case red, green }
来源：http://yo.szxytkj.cn

[T29] Swift：guard 提前返回
来源：http://ig.chemitech.net.cn

guard let x = opt else { return }
来源：http://ie.newstarts.cn

[T30] Swift：协议
来源：http://sl.lnxyls.cn

protocol Shape { func area() -> Double }
来源：http://gg.newstarts.cn

[T31] Lua：Hello World
来源：http://oi.shxzskj.cn

print("Hello")
来源：http://mc.lnxyls.cn

[T32] Lua：局部变量
来源：http://cg.521024.cn

local a = 1
来源：http://wc.hahajie.cn

[T33] Lua：表（数组）
来源：http://tw.shxzskj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://qq.jianghongdianzi.cn

[T34] Lua：遍历表
来源：http://xc.yuexingan06.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://li.chemitech.net.cn

[T35] Lua：字典表
来源：http://jl.szsharing.cn

local d = { a = 1 };  d.b = 2
来源：http://op.nszjky.cn

[T36] Lua：函数
来源：http://gh.huixiangedu.cn

function add(a, b) return a + b end
来源：http://ui.szxytkj.cn

[T37] Lua：字符串拼接
来源：http://vg.newstarts.cn

"a" .. "b"
来源：http://rt.wgjwhj.cn

[T38] Lua：条件
来源：http://qh.panjiajie.cn

if x > 0 then print("正") end
来源：http://me.9csxet.cn

[T39] Lua：模式匹配
来源：http://gm.huixinmuqiang.cn

string.find(s, "%d+")
来源：http://zg.bookmarksfly.cn

[T40] Lua：元表
来源：http://ft.asd995.cn

setmetatable({}, { __index = base })
来源：http://nx.szsharing.cn

[T41] Perl：Hello World
来源：http://nb.muxihuayi.cn

print "Hello\n";
来源：http://hn.yuexingan06.cn

[T42] Perl：变量类型
来源：http://bk.gzmigu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nl.hnjuh.cn

[T43] Perl：字符串插值
来源：http://eb.bjjhwx.cn

"值: $a"
来源：http://uw.chemitech.net.cn

[T44] Perl：条件
来源：http://pb.shxzskj.cn

if ($a > 0) { print "正"; }
来源：http://jx.haigaiapp.cn

[T45] Perl：数组遍历
来源：http://pi.muxihuayi.cn

for my $x (@arr) { print $x; }
来源：http://ec.huanxung.cn

[T46] Perl：哈希操作
来源：http://um.lnxyls.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vu.huixiangedu.cn

[T47] Perl：正则捕获
来源：http://uh.9csxet.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dj.yuexingan06.cn

[T48] Perl：正则替换
来源：http://vx.huixiangedu.cn

$s =~ s/old/new/g;
来源：http://nc.521024.cn

[T49] Perl：函数
来源：http://ud.muxihuayi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fq.shtwfgs.cn

[T50] Perl：逐行读文件
来源：http://fu.nszjky.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ju.nszjky.cn

while (my $line = <$fh>) { print $line; }
来源：http://ok.lnxyls.cn

[T51] Scala：Hello World
来源：http://dn.521024.cn

println("Hello")
来源：http://wx.shxzukj.cn

[T52] Scala：变量
来源：http://zg.9csxet.cn

val a = 1;  var b = 2
来源：http://ff.hnjuh.cn

[T53] Scala：字符串插值
来源：http://iy.hahajie.cn

s"值: $b"
来源：http://jq.huixiangedu.cn

[T54] Scala：集合映射
来源：http://yf.nicolike.cn

List(1, 2, 3).map(_ * 2)
来源：http://gs.nicolike.cn

[T55] Scala：集合过滤
来源：http://jk.szsharing.cn

List(1, 2, 3).filter(_ > 1)
来源：http://zn.chemitech.net.cn

[T56] Scala：样例类
来源：http://rn.colortex.cn

case class User(name: String, age: Int)
来源：http://tz.hahajie.cn

[T57] Scala：模式匹配
来源：http://ji.muxihuayi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://uf.hnjuh.cn

[T58] Scala：函数定义
来源：http://ut.wgjwhj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://qa.chemitech.net.cn

[T59] Scala：循环
来源：http://xo.gzmigu.cn

for (i <- 1 to 10) println(i)
来源：http://dv.jianghongdianzi.cn

[T60] Scala：折叠
来源：http://sa.nicolike.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lj.haigaiapp.cn

================================================================================
来源：http://uu.chemitech.net.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fh.colortex.cn

================================================================================
来源：http://aj.shxzskj.cn

[U01] Py：创建虚拟环境
来源：http://kp.huixiangedu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zf.521024.cn

[U02] Py：导出 / 安装依赖
来源：http://fh.yuexingan06.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lh.szxytkj.cn

[U03] Py：加载 .env 配置
来源：http://gz.huixinmuqiang.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rk.jianghongdianzi.cn

[U04] Py：变量调试打印
来源：http://dv.yuntaijiaju.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nq.hahajie.cn

[U05] Py：列表去重且保序
来源：http://qy.hnjuh.cn

list(dict.fromkeys(arr))
来源：http://yl.shtwfgs.cn

[U06] Py：合并两个字典
来源：http://hd.shtwfgs.cn

{**a, **b}
来源：http://zh.521024.cn

[U07] Py：反转字典键值
来源：http://fq.nicolike.cn

{v: k for k, v in d.items()}
来源：http://qb.newstarts.cn

[U08] Py：展平二维列表
来源：http://ha.jctech888.com.cn

[y for x in nested for y in x]
来源：http://wx.nszjky.cn

[U09] Py：字典取最大值的键
来源：http://uu.huixinmuqiang.cn

max(d, key=d.get)
来源：http://ew.huixinmuqiang.cn

[U10] Py：按值排序字典
来源：http://hh.colortex.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pr.hnjuh.cn

[U11] Py：生成器表达式
来源：http://rx.hnjuh.cn

(x * 2 for x in arr)
来源：http://pq.huixiangedu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://jh.panjiajie.cn

Counter(arr).most_common(3)
来源：http://xo.shtwfgs.cn

[U13] Py：固定长度队列
来源：http://ce.nicolike.cn

deque(maxlen=10)
来源：http://gs.szxytkj.cn

[U14] Py：分组收集到列表
来源：http://te.bookmarksfly.cn

defaultdict(list)
来源：http://jr.yuntaijiaju.cn

[U15] Py：高精度计时
来源：http://ec.lnxyls.cn

t = time.perf_counter()
来源：http://tx.hahajie.cn

[U16] Py：命令行参数解析
来源：http://rz.szsharing.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://we.yuntaijiaju.cn

[U17] Py：初始化日志
来源：http://vz.szsharing.cn

logging.basicConfig(level=logging.INFO)
来源：http://or.hnjuh.cn

[U18] Py：预编译正则
来源：http://mz.9csxet.cn

pat = re.compile(r"\d+")
来源：http://ud.521024.cn

[U19] Py：正则替换带回调
来源：http://oa.bjjhwx.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ul.muxihuayi.cn

[U20] Py：缓存函数结果
来源：http://wp.huixinmuqiang.cn

@functools.lru_cache(maxsize=None)
来源：http://yg.jianghongdianzi.cn

[U21] Py：自定义上下文管理器
来源：http://md.hahajie.cn

@contextlib.contextmanager
来源：http://kx.jianghongdianzi.cn

[U22] Py：矩阵转置
来源：http://pd.newstarts.cn

list(zip(*m))
来源：http://ph.colortex.cn

[U23] Py：分块读取大文件
来源：http://wp.bjjhwx.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hr.huixiangedu.cn

[U24] Py：路径操作
来源：http://iz.shxzukj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mw.yuexingan06.cn

[U25] Py：CSV 按字典读
来源：http://mh.yuntaijiaju.cn

csv.DictReader(f)
来源：http://sf.huanxung.cn

[U26] Py：并发下载
来源：http://na.yuexingan06.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://og.jianghongdianzi.cn

[U27] Py：异步 HTTP
来源：http://ye.yuexingan06.cn

aiohttp.ClientSession() 配合 async with
来源：http://gc.lnxyls.cn

[U28] Py：类型别名
来源：http://ij.hnjuh.cn

UserId = int
来源：http://cc.huanxung.cn

[U29] Py：属性校验
来源：http://mf.wgjwhj.cn

@property 与 @x.setter 配合
来源：http://qn.bjjhwx.cn

[U30] Py：数据类
来源：http://ya.yuntaijiaju.cn

@dataclass(slots=True)
来源：http://jx.huixinmuqiang.cn

[U31] Py：单测
来源：http://sr.jctech888.com.cn

python -m pytest -q
来源：http://pb.szxytkj.cn

[U32] Py：代码格式化
来源：http://in.huixinmuqiang.cn

ruff format . && ruff check --fix .
来源：http://nr.shxzukj.cn

[U33] Py：打包发布
来源：http://ro.bjjhwx.cn

python -m build  （依赖 pyproject.toml）
来源：http://el.huixinmuqiang.cn

[U34] Py：判断编码
来源：http://ls.haigaiapp.cn

chardet.detect(raw)
来源：http://se.panjiajie.cn

[U35] Py：发送邮件
来源：http://kr.shxzskj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zd.newstarts.cn

[U36] Py：定时任务
来源：http://fg.hahajie.cn

schedule.every(10).minutes.do(job)
来源：http://fh.haigaiapp.cn

[U37] Py：读写 Excel
来源：http://rg.chemitech.net.cn

pandas.read_excel / DataFrame.to_excel
来源：http://yh.bjjhwx.cn

[U38] Py：获取脚本所在目录
来源：http://fg.nicolike.cn

Path(__file__).resolve().parent
来源：http://mo.hahajie.cn

[U39] Py：判断是否在交互环境
来源：http://da.huixinmuqiang.cn

sys.stdout.isatty()
来源：http://uh.yuntaijiaju.cn

[U40] Py：打印到标准错误
来源：http://os.szxytkj.cn

print("err", file=sys.stderr)
来源：http://hq.huanxung.cn

[U41] PHP：初始化 Composer 项目
来源：http://np.muxihuayi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ff.szsharing.cn

[U42] PHP：PSR-4 自动加载
来源：http://oe.huanxung.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ri.nicolike.cn

[U43] PHP：声明命名空间
来源：http://aw.huixiangedu.cn

namespace App\Http;
来源：http://tu.colortex.cn

[U44] PHP：开启严格类型
来源：http://nz.huixinmuqiang.cn

declare(strict_types=1);
来源：http://fe.521024.cn

[U45] PHP：类型声明与返回类型
来源：http://ks.szsharing.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://gj.huixiangedu.cn

[U46] PHP：可空类型
来源：http://vn.panjiajie.cn

?string $name = null
来源：http://vi.haigaiapp.cn

[U47] PHP：联合类型
来源：http://qt.nszjky.cn

int|string $id
来源：http://gi.gzmigu.cn

[U48] PHP：纯枚举
来源：http://jv.haigaiapp.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vo.9csxet.cn

[U49] PHP：只读属性
来源：http://tl.haigaiapp.cn

public readonly string $name
来源：http://tf.shxzskj.cn

[U50] PHP：构造器属性提升
来源：http://pd.szsharing.cn

public function __construct(private int $id) {}
来源：http://nf.haigaiapp.cn

[U51] PHP：数组解构
来源：http://nc.nicolike.cn

[$a, $b] = $arr;
来源：http://nx.hnjuh.cn

[U52] PHP：箭头函数
来源：http://yr.asd995.cn

$double = fn($x) => $x * 2;
来源：http://gr.nicolike.cn

[U53] PHP：空合并运算符
来源：http://oy.shxzskj.cn

$v = $a ?? $b ?? "default";
来源：http://rd.jctech888.com.cn

[U54] PHP：空安全调用
来源：http://uu.nszjky.cn

$obj?->method()
来源：http://az.nszjky.cn

[U55] PHP：match 表达式
来源：http://np.huixinmuqiang.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yi.panjiajie.cn

[U56] PHP：命名参数
来源：http://hh.jianghongdianzi.cn

f(a: 1, b: 2)
来源：http://zc.9csxet.cn

[U57] PHP：字符串插值
来源：http://sl.huixiangedu.cn

"值: {$a}"
来源：http://jn.9csxet.cn

[U58] PHP：数组三件套
来源：http://ng.shxzukj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://td.huanxung.cn

[U59] PHP：自定义排序
来源：http://bi.hahajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yy.bookmarksfly.cn

[U60] PHP：JSON 编解码
来源：http://cq.9csxet.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://us.huixiangedu.cn

[U61] PHP：正则
来源：http://sh.szsharing.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jh.chemitech.net.cn

[U62] PHP：日期对象
来源：http://kh.lnxyls.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://im.gzmigu.cn

[U63] PHP：文件读写
来源：http://tm.wgjwhj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gr.yuntaijiaju.cn

[U64] PHP：目录遍历
来源：http://xh.jctech888.com.cn

glob("dir/*.php");  scandir("dir");
来源：http://rt.gzmigu.cn

[U65] PHP：会话
来源：http://mg.huixiangedu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://xy.bjjhwx.cn

[U66] PHP：设置 Cookie
来源：http://fe.huixiangedu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pp.jianghongdianzi.cn

[U67] PHP：处理文件上传
来源：http://kb.nicolike.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jf.lnxyls.cn

[U68] PHP：PDO 连接
来源：http://es.wgjwhj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kz.shtwfgs.cn

[U69] PHP：PDO 预处理
来源：http://jf.hnjuh.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://uj.colortex.cn

[U70] PHP：PDO 事务
来源：http://ez.9csxet.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hp.gzmigu.cn

[U71] PHP：抛出异常
来源：http://bj.jctech888.com.cn

throw new RuntimeException("失败", 500);
来源：http://ye.huixiangedu.cn

[U72] PHP：写错误日志
来源：http://sb.muxihuayi.cn

error_log("失败: " . $e->getMessage());
来源：http://qs.huixiangedu.cn

[U73] PHP：读取 ini 配置
来源：http://xd.bjjhwx.cn

parse_ini_file("config.ini", true)
来源：http://hh.gzmigu.cn

[U74] PHP：读取环境变量
来源：http://hp.9csxet.cn

getenv("APP_ENV") ?: "production"
来源：http://fb.asd995.cn

[U75] PHP：依赖注入
来源：http://ky.jianghongdianzi.cn

composer require psr/container
来源：http://nv.yuexingan06.cn

[U76] PHP：简单路由
来源：http://ti.gzmigu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xk.szsharing.cn

[U77] PHP：模板渲染
来源：http://jp.nicolike.cn

composer require twig/twig
来源：http://wq.wgjwhj.cn

[U78] PHP：单元测试
来源：http://pt.huanxung.cn

composer require --dev phpunit/phpunit
来源：http://ll.wgjwhj.cn

[U79] PHP：静态分析
来源：http://rm.yuexingan06.cn

composer require --dev phpstan/phpstan
来源：http://dz.huixiangedu.cn

[U80] PHP：代码规范修复
来源：http://gb.jctech888.com.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ws.jctech888.com.cn

[U81] JS：初始化项目
来源：http://qv.szxytkj.cn

npm init -y;  npm i express
来源：http://zd.asd995.cn

[U82] JS：package.json 脚本
来源：http://ge.nszjky.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ql.huixinmuqiang.cn

[U83] JS：ES Module 导入导出
来源：http://dd.szsharing.cn

export const a = 1;  import { a } from "./m.js";
来源：http://bs.521024.cn

[U84] JS：CommonJS 写法
来源：http://hw.shxzskj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://sh.yuexingan06.cn


<!-- 参考信息 -->