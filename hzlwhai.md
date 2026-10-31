代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ui.jctech888.com.cn

================================================================================
来源：http://sh.szxytkj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ea.yuntaijiaju.cn

================================================================================
来源：http://zs.yuntaijiaju.cn

[T01] Kotlin：Hello World
来源：http://wj.huanxung.cn

println("Hello")
来源：http://lo.bookmarksfly.cn

[T02] Kotlin：变量
来源：http://sy.hahajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gq.hahajie.cn

[T03] Kotlin：字符串模板
来源：http://wx.lnxyls.cn

"值: $b"
来源：http://yo.colortex.cn

[T04] Kotlin：空安全
来源：http://km.bookmarksfly.cn

val n: String? = null;  n?.length
来源：http://ck.shxzskj.cn

[T05] Kotlin：when 表达式
来源：http://qz.yuntaijiaju.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zn.szsharing.cn

[T06] Kotlin：集合映射
来源：http://kh.haigaiapp.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://uz.hahajie.cn

[T07] Kotlin：集合过滤
来源：http://uf.shxzskj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://zt.huixinmuqiang.cn

[T08] Kotlin：数据类
来源：http://ge.gzmigu.cn

data class User(val name: String, val age: Int)
来源：http://pz.nicolike.cn

[T09] Kotlin：扩展函数
来源：http://jb.jianghongdianzi.cn

fun String.exclaim() = this + "!"
来源：http://mg.shxzukj.cn

[T10] Kotlin：默认参数
来源：http://lw.9csxet.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gl.chemitech.net.cn

[T11] Kotlin：协程
来源：http://ef.nicolike.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ve.hahajie.cn

[T12] Kotlin：解构声明
来源：http://pe.hnjuh.cn

val (a, b) = Pair(1, 2)
来源：http://md.newstarts.cn

[T13] Kotlin：只读 Map
来源：http://sl.asd995.cn

val m = mapOf("a" to 1)
来源：http://bm.panjiajie.cn

[T14] Kotlin：循环
来源：http://nr.jianghongdianzi.cn

for (i in 1..10) println(i)
来源：http://am.hnjuh.cn

[T15] Kotlin：接口
来源：http://xe.hahajie.cn

interface Shape { fun area(): Double }
来源：http://rh.haigaiapp.cn

[T16] Swift：Hello World
来源：http://ve.asd995.cn

print("Hello")
来源：http://sf.wgjwhj.cn

[T17] Swift：变量与常量
来源：http://ph.nicolike.cn

var a = 1;  let b = 2
来源：http://if.colortex.cn

[T18] Swift：字符串插值
来源：http://nn.huanxung.cn

"值: \(b)"
来源：http://zn.szxytkj.cn

[T19] Swift：可选绑定
来源：http://ke.muxihuayi.cn

if let n = opt { print(n) }
来源：http://hc.shxzukj.cn

[T20] Swift：数组操作
来源：http://qb.newstarts.cn

var a = [1, 2, 3];  a.append(4)
来源：http://lz.nicolike.cn

[T21] Swift：遍历
来源：http://kn.huanxung.cn

for x in a { print(x) }
来源：http://xv.9csxet.cn

[T22] Swift：字典
来源：http://fg.shxzukj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ww.huixinmuqiang.cn

[T23] Swift：函数
来源：http://wl.panjiajie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ph.jianghongdianzi.cn

[T24] Swift：闭包
来源：http://mm.huixinmuqiang.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://uy.colortex.cn

[T25] Swift：结构体
来源：http://ek.jianghongdianzi.cn

struct P { var x: Int }
来源：http://uh.hahajie.cn

[T26] Swift：类与重写
来源：http://td.bookmarksfly.cn

class A: Base { override func f() {} }
来源：http://fn.9csxet.cn

[T27] Swift：错误处理
来源：http://zp.jianghongdianzi.cn

do { try f() } catch { print(error) }
来源：http://mt.hnjuh.cn

[T28] Swift：枚举
来源：http://zy.asd995.cn

enum Color { case red, green }
来源：http://ih.haigaiapp.cn

[T29] Swift：guard 提前返回
来源：http://gy.shtwfgs.cn

guard let x = opt else { return }
来源：http://zj.szxytkj.cn

[T30] Swift：协议
来源：http://ic.huanxung.cn

protocol Shape { func area() -> Double }
来源：http://mj.gzmigu.cn

[T31] Lua：Hello World
来源：http://tl.asd995.cn

print("Hello")
来源：http://sx.wgjwhj.cn

[T32] Lua：局部变量
来源：http://ft.szxytkj.cn

local a = 1
来源：http://px.bjjhwx.cn

[T33] Lua：表（数组）
来源：http://kr.haigaiapp.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://nj.shxzukj.cn

[T34] Lua：遍历表
来源：http://oo.yuexingan06.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://yg.newstarts.cn

[T35] Lua：字典表
来源：http://jj.huixinmuqiang.cn

local d = { a = 1 };  d.b = 2
来源：http://gj.gzmigu.cn

[T36] Lua：函数
来源：http://zr.haigaiapp.cn

function add(a, b) return a + b end
来源：http://ib.huanxung.cn

[T37] Lua：字符串拼接
来源：http://tk.nicolike.cn

"a" .. "b"
来源：http://fx.newstarts.cn

[T38] Lua：条件
来源：http://fq.jianghongdianzi.cn

if x > 0 then print("正") end
来源：http://bi.jianghongdianzi.cn

[T39] Lua：模式匹配
来源：http://ax.panjiajie.cn

string.find(s, "%d+")
来源：http://as.muxihuayi.cn

[T40] Lua：元表
来源：http://bi.521024.cn

setmetatable({}, { __index = base })
来源：http://yo.newstarts.cn

[T41] Perl：Hello World
来源：http://rk.yuntaijiaju.cn

print "Hello\n";
来源：http://rf.wgjwhj.cn

[T42] Perl：变量类型
来源：http://pw.shxzukj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ys.panjiajie.cn

[T43] Perl：字符串插值
来源：http://gs.gzmigu.cn

"值: $a"
来源：http://lx.hahajie.cn

[T44] Perl：条件
来源：http://tv.newstarts.cn

if ($a > 0) { print "正"; }
来源：http://et.nszjky.cn

[T45] Perl：数组遍历
来源：http://al.jctech888.com.cn

for my $x (@arr) { print $x; }
来源：http://pk.9csxet.cn

[T46] Perl：哈希操作
来源：http://sk.newstarts.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ms.lnxyls.cn

[T47] Perl：正则捕获
来源：http://hj.jctech888.com.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://bh.huanxung.cn

[T48] Perl：正则替换
来源：http://ta.szxytkj.cn

$s =~ s/old/new/g;
来源：http://um.shxzukj.cn

[T49] Perl：函数
来源：http://zh.newstarts.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://id.muxihuayi.cn

[T50] Perl：逐行读文件
来源：http://yx.huanxung.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://pd.shtwfgs.cn

while (my $line = <$fh>) { print $line; }
来源：http://uu.nicolike.cn

[T51] Scala：Hello World
来源：http://fq.hahajie.cn

println("Hello")
来源：http://qq.muxihuayi.cn

[T52] Scala：变量
来源：http://jk.huixinmuqiang.cn

val a = 1;  var b = 2
来源：http://us.hahajie.cn

[T53] Scala：字符串插值
来源：http://rb.colortex.cn

s"值: $b"
来源：http://ws.yuexingan06.cn

[T54] Scala：集合映射
来源：http://qx.colortex.cn

List(1, 2, 3).map(_ * 2)
来源：http://rl.yuntaijiaju.cn

[T55] Scala：集合过滤
来源：http://lf.colortex.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ue.yuexingan06.cn

[T56] Scala：样例类
来源：http://eg.huixiangedu.cn

case class User(name: String, age: Int)
来源：http://pk.bjjhwx.cn

[T57] Scala：模式匹配
来源：http://nm.shtwfgs.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ay.nicolike.cn

[T58] Scala：函数定义
来源：http://if.chemitech.net.cn

def add(a: Int, b: Int): Int = a + b
来源：http://sj.muxihuayi.cn

[T59] Scala：循环
来源：http://mc.bookmarksfly.cn

for (i <- 1 to 10) println(i)
来源：http://gr.huixinmuqiang.cn

[T60] Scala：折叠
来源：http://kx.szxytkj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lp.521024.cn

================================================================================
来源：http://rz.colortex.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lk.bjjhwx.cn

================================================================================
来源：http://ev.jianghongdianzi.cn

[U01] Py：创建虚拟环境
来源：http://xr.szsharing.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ws.nicolike.cn

[U02] Py：导出 / 安装依赖
来源：http://zw.muxihuayi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ub.shxzukj.cn

[U03] Py：加载 .env 配置
来源：http://rv.yuntaijiaju.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fg.shxzskj.cn

[U04] Py：变量调试打印
来源：http://yj.jianghongdianzi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ha.szxytkj.cn

[U05] Py：列表去重且保序
来源：http://fs.jianghongdianzi.cn

list(dict.fromkeys(arr))
来源：http://jj.colortex.cn

[U06] Py：合并两个字典
来源：http://fq.hahajie.cn

{**a, **b}
来源：http://sz.szxytkj.cn

[U07] Py：反转字典键值
来源：http://bx.shtwfgs.cn

{v: k for k, v in d.items()}
来源：http://hm.shtwfgs.cn

[U08] Py：展平二维列表
来源：http://gs.shxzskj.cn

[y for x in nested for y in x]
来源：http://cr.shxzukj.cn

[U09] Py：字典取最大值的键
来源：http://gr.yuntaijiaju.cn

max(d, key=d.get)
来源：http://zo.shxzukj.cn

[U10] Py：按值排序字典
来源：http://bp.lnxyls.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xi.bjjhwx.cn

[U11] Py：生成器表达式
来源：http://pj.nicolike.cn

(x * 2 for x in arr)
来源：http://sa.nszjky.cn

[U12] Py：取出现最多的 3 个元素
来源：http://za.haigaiapp.cn

Counter(arr).most_common(3)
来源：http://al.jianghongdianzi.cn

[U13] Py：固定长度队列
来源：http://lg.newstarts.cn

deque(maxlen=10)
来源：http://yf.nicolike.cn

[U14] Py：分组收集到列表
来源：http://vq.jianghongdianzi.cn

defaultdict(list)
来源：http://pn.bjjhwx.cn

[U15] Py：高精度计时
来源：http://fw.9csxet.cn

t = time.perf_counter()
来源：http://sp.hnjuh.cn

[U16] Py：命令行参数解析
来源：http://ak.bjjhwx.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ol.panjiajie.cn

[U17] Py：初始化日志
来源：http://ki.szsharing.cn

logging.basicConfig(level=logging.INFO)
来源：http://lp.yuntaijiaju.cn

[U18] Py：预编译正则
来源：http://ah.huixiangedu.cn

pat = re.compile(r"\d+")
来源：http://kb.szxytkj.cn

[U19] Py：正则替换带回调
来源：http://ui.9csxet.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pv.szsharing.cn

[U20] Py：缓存函数结果
来源：http://lv.521024.cn

@functools.lru_cache(maxsize=None)
来源：http://og.asd995.cn

[U21] Py：自定义上下文管理器
来源：http://qy.nszjky.cn

@contextlib.contextmanager
来源：http://kh.chemitech.net.cn

[U22] Py：矩阵转置
来源：http://vd.shxzukj.cn

list(zip(*m))
来源：http://xo.lnxyls.cn

[U23] Py：分块读取大文件
来源：http://en.asd995.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xb.huanxung.cn

[U24] Py：路径操作
来源：http://ze.9csxet.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zr.yuntaijiaju.cn

[U25] Py：CSV 按字典读
来源：http://zj.bjjhwx.cn

csv.DictReader(f)
来源：http://fr.haigaiapp.cn

[U26] Py：并发下载
来源：http://jg.521024.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lu.szsharing.cn

[U27] Py：异步 HTTP
来源：http://dt.521024.cn

aiohttp.ClientSession() 配合 async with
来源：http://cm.chemitech.net.cn

[U28] Py：类型别名
来源：http://zw.huixiangedu.cn

UserId = int
来源：http://zq.shtwfgs.cn

[U29] Py：属性校验
来源：http://mh.shxzukj.cn

@property 与 @x.setter 配合
来源：http://pr.jianghongdianzi.cn

[U30] Py：数据类
来源：http://yr.chemitech.net.cn

@dataclass(slots=True)
来源：http://fn.newstarts.cn

[U31] Py：单测
来源：http://ll.9csxet.cn

python -m pytest -q
来源：http://zk.9csxet.cn

[U32] Py：代码格式化
来源：http://jd.huixiangedu.cn

ruff format . && ruff check --fix .
来源：http://yp.chemitech.net.cn

[U33] Py：打包发布
来源：http://et.hahajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://qv.bookmarksfly.cn

[U34] Py：判断编码
来源：http://pz.yuntaijiaju.cn

chardet.detect(raw)
来源：http://ig.colortex.cn

[U35] Py：发送邮件
来源：http://th.huixinmuqiang.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ix.521024.cn

[U36] Py：定时任务
来源：http://gc.yuntaijiaju.cn

schedule.every(10).minutes.do(job)
来源：http://df.huixinmuqiang.cn

[U37] Py：读写 Excel
来源：http://ly.shxzukj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://dw.shxzskj.cn

[U38] Py：获取脚本所在目录
来源：http://bk.huixinmuqiang.cn

Path(__file__).resolve().parent
来源：http://ap.szxytkj.cn

[U39] Py：判断是否在交互环境
来源：http://rm.shtwfgs.cn

sys.stdout.isatty()
来源：http://cq.huixinmuqiang.cn

[U40] Py：打印到标准错误
来源：http://ur.huanxung.cn

print("err", file=sys.stderr)
来源：http://qo.haigaiapp.cn

[U41] PHP：初始化 Composer 项目
来源：http://ix.chemitech.net.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://bp.jianghongdianzi.cn

[U42] PHP：PSR-4 自动加载
来源：http://wp.chemitech.net.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://av.nicolike.cn

[U43] PHP：声明命名空间
来源：http://mm.szxytkj.cn

namespace App\Http;
来源：http://ip.muxihuayi.cn

[U44] PHP：开启严格类型
来源：http://nj.9csxet.cn

declare(strict_types=1);
来源：http://jj.muxihuayi.cn

[U45] PHP：类型声明与返回类型
来源：http://cr.panjiajie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://lv.lnxyls.cn

[U46] PHP：可空类型
来源：http://pj.bjjhwx.cn

?string $name = null
来源：http://zx.lnxyls.cn

[U47] PHP：联合类型
来源：http://zp.bjjhwx.cn

int|string $id
来源：http://qi.huixiangedu.cn

[U48] PHP：纯枚举
来源：http://sg.newstarts.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jt.huixinmuqiang.cn

[U49] PHP：只读属性
来源：http://ye.newstarts.cn

public readonly string $name
来源：http://ro.newstarts.cn

[U50] PHP：构造器属性提升
来源：http://gg.gzmigu.cn

public function __construct(private int $id) {}
来源：http://kd.nszjky.cn

[U51] PHP：数组解构
来源：http://hy.huixinmuqiang.cn

[$a, $b] = $arr;
来源：http://ie.muxihuayi.cn

[U52] PHP：箭头函数
来源：http://kw.szxytkj.cn

$double = fn($x) => $x * 2;
来源：http://he.colortex.cn

[U53] PHP：空合并运算符
来源：http://kq.asd995.cn

$v = $a ?? $b ?? "default";
来源：http://br.szsharing.cn

[U54] PHP：空安全调用
来源：http://je.nicolike.cn

$obj?->method()
来源：http://hn.huixinmuqiang.cn

[U55] PHP：match 表达式
来源：http://rz.9csxet.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tm.521024.cn

[U56] PHP：命名参数
来源：http://yf.wgjwhj.cn

f(a: 1, b: 2)
来源：http://nf.szxytkj.cn

[U57] PHP：字符串插值
来源：http://gp.huixiangedu.cn

"值: {$a}"
来源：http://ry.gzmigu.cn

[U58] PHP：数组三件套
来源：http://mr.521024.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gy.huixinmuqiang.cn

[U59] PHP：自定义排序
来源：http://dr.yuexingan06.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ah.shxzukj.cn

[U60] PHP：JSON 编解码
来源：http://vw.huanxung.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jc.muxihuayi.cn

[U61] PHP：正则
来源：http://ag.bjjhwx.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tg.nszjky.cn

[U62] PHP：日期对象
来源：http://th.9csxet.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lk.gzmigu.cn

[U63] PHP：文件读写
来源：http://eg.chemitech.net.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sw.asd995.cn

[U64] PHP：目录遍历
来源：http://oe.yuntaijiaju.cn

glob("dir/*.php");  scandir("dir");
来源：http://um.shtwfgs.cn

[U65] PHP：会话
来源：http://xq.bjjhwx.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kq.hahajie.cn

[U66] PHP：设置 Cookie
来源：http://gl.huixiangedu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sa.asd995.cn

[U67] PHP：处理文件上传
来源：http://tk.yuntaijiaju.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ab.bjjhwx.cn

[U68] PHP：PDO 连接
来源：http://hu.muxihuayi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yd.shtwfgs.cn

[U69] PHP：PDO 预处理
来源：http://dg.jianghongdianzi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wi.jianghongdianzi.cn

[U70] PHP：PDO 事务
来源：http://mb.shxzukj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wm.gzmigu.cn

[U71] PHP：抛出异常
来源：http://tz.asd995.cn

throw new RuntimeException("失败", 500);
来源：http://zf.asd995.cn

[U72] PHP：写错误日志
来源：http://sy.muxihuayi.cn

error_log("失败: " . $e->getMessage());
来源：http://oi.panjiajie.cn

[U73] PHP：读取 ini 配置
来源：http://tn.521024.cn

parse_ini_file("config.ini", true)
来源：http://yp.jianghongdianzi.cn

[U74] PHP：读取环境变量
来源：http://ek.shxzskj.cn

getenv("APP_ENV") ?: "production"
来源：http://xg.asd995.cn

[U75] PHP：依赖注入
来源：http://ky.haigaiapp.cn

composer require psr/container
来源：http://sv.yuexingan06.cn

[U76] PHP：简单路由
来源：http://am.hahajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ya.nicolike.cn

[U77] PHP：模板渲染
来源：http://us.asd995.cn

composer require twig/twig
来源：http://hb.hahajie.cn

[U78] PHP：单元测试
来源：http://cc.haigaiapp.cn

composer require --dev phpunit/phpunit
来源：http://vh.bjjhwx.cn

[U79] PHP：静态分析
来源：http://gi.huixiangedu.cn

composer require --dev phpstan/phpstan
来源：http://qd.yuntaijiaju.cn

[U80] PHP：代码规范修复
来源：http://mc.hnjuh.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://te.lnxyls.cn

[U81] JS：初始化项目
来源：http://ko.hnjuh.cn

npm init -y;  npm i express
来源：http://yk.huixiangedu.cn

[U82] JS：package.json 脚本
来源：http://oq.shxzukj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mo.bookmarksfly.cn

[U83] JS：ES Module 导入导出
来源：http://id.haigaiapp.cn

export const a = 1;  import { a } from "./m.js";
来源：http://tk.yuntaijiaju.cn

[U84] JS：CommonJS 写法
来源：http://bn.bookmarksfly.cn

module.exports = { a };  const { a } = require("./m");
来源：http://gz.nszjky.cn

[U85] JS：可选链
来源：http://yh.shtwfgs.cn

a?.b?.c
来源：http://mt.hnjuh.cn

[U86] JS：空值合并
来源：http://hy.hahajie.cn

a ?? b
来源：http://gr.chemitech.net.cn


<!-- 参考信息 -->