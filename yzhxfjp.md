代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ud.szsharing.cn

================================================================================
来源：http://uq.nszjky.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wc.bjjhwx.cn

================================================================================
来源：http://bo.shxzskj.cn

[T01] Kotlin：Hello World
来源：http://lu.huanxung.cn

println("Hello")
来源：http://bs.huanxung.cn

[T02] Kotlin：变量
来源：http://fw.521024.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://er.jianghongdianzi.cn

[T03] Kotlin：字符串模板
来源：http://ti.panjiajie.cn

"值: $b"
来源：http://gs.newstarts.cn

[T04] Kotlin：空安全
来源：http://xb.jctech888.com.cn

val n: String? = null;  n?.length
来源：http://rn.yuntaijiaju.cn

[T05] Kotlin：when 表达式
来源：http://ec.newstarts.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lt.szxytkj.cn

[T06] Kotlin：集合映射
来源：http://fw.shxzskj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://oz.asd995.cn

[T07] Kotlin：集合过滤
来源：http://by.huixiangedu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://kt.asd995.cn

[T08] Kotlin：数据类
来源：http://ys.szxytkj.cn

data class User(val name: String, val age: Int)
来源：http://yk.jianghongdianzi.cn

[T09] Kotlin：扩展函数
来源：http://ey.521024.cn

fun String.exclaim() = this + "!"
来源：http://sm.nszjky.cn

[T10] Kotlin：默认参数
来源：http://te.yuexingan06.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://nk.chemitech.net.cn

[T11] Kotlin：协程
来源：http://om.nicolike.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jh.lnxyls.cn

[T12] Kotlin：解构声明
来源：http://uw.bookmarksfly.cn

val (a, b) = Pair(1, 2)
来源：http://bu.wgjwhj.cn

[T13] Kotlin：只读 Map
来源：http://sq.hnjuh.cn

val m = mapOf("a" to 1)
来源：http://hn.newstarts.cn

[T14] Kotlin：循环
来源：http://dj.bookmarksfly.cn

for (i in 1..10) println(i)
来源：http://ek.nszjky.cn

[T15] Kotlin：接口
来源：http://zq.newstarts.cn

interface Shape { fun area(): Double }
来源：http://sg.shxzukj.cn

[T16] Swift：Hello World
来源：http://tq.wgjwhj.cn

print("Hello")
来源：http://ga.hnjuh.cn

[T17] Swift：变量与常量
来源：http://lo.bjjhwx.cn

var a = 1;  let b = 2
来源：http://de.shxzukj.cn

[T18] Swift：字符串插值
来源：http://jq.chemitech.net.cn

"值: \(b)"
来源：http://ii.huixiangedu.cn

[T19] Swift：可选绑定
来源：http://we.huixiangedu.cn

if let n = opt { print(n) }
来源：http://dc.bjjhwx.cn

[T20] Swift：数组操作
来源：http://xl.hahajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ue.chemitech.net.cn

[T21] Swift：遍历
来源：http://uh.shtwfgs.cn

for x in a { print(x) }
来源：http://su.shtwfgs.cn

[T22] Swift：字典
来源：http://aj.9csxet.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xi.9csxet.cn

[T23] Swift：函数
来源：http://rn.panjiajie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pv.yuntaijiaju.cn

[T24] Swift：闭包
来源：http://gb.521024.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://bm.jctech888.com.cn

[T25] Swift：结构体
来源：http://wr.asd995.cn

struct P { var x: Int }
来源：http://td.bookmarksfly.cn

[T26] Swift：类与重写
来源：http://zr.yuexingan06.cn

class A: Base { override func f() {} }
来源：http://qh.hnjuh.cn

[T27] Swift：错误处理
来源：http://cb.hahajie.cn

do { try f() } catch { print(error) }
来源：http://cp.nicolike.cn

[T28] Swift：枚举
来源：http://cs.521024.cn

enum Color { case red, green }
来源：http://pi.jianghongdianzi.cn

[T29] Swift：guard 提前返回
来源：http://rh.9csxet.cn

guard let x = opt else { return }
来源：http://oe.muxihuayi.cn

[T30] Swift：协议
来源：http://te.shtwfgs.cn

protocol Shape { func area() -> Double }
来源：http://uc.asd995.cn

[T31] Lua：Hello World
来源：http://gd.nszjky.cn

print("Hello")
来源：http://gb.yuntaijiaju.cn

[T32] Lua：局部变量
来源：http://mk.521024.cn

local a = 1
来源：http://tm.newstarts.cn

[T33] Lua：表（数组）
来源：http://rx.shxzskj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://bd.muxihuayi.cn

[T34] Lua：遍历表
来源：http://rt.jianghongdianzi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vm.9csxet.cn

[T35] Lua：字典表
来源：http://ho.9csxet.cn

local d = { a = 1 };  d.b = 2
来源：http://nh.wgjwhj.cn

[T36] Lua：函数
来源：http://bl.shtwfgs.cn

function add(a, b) return a + b end
来源：http://bl.9csxet.cn

[T37] Lua：字符串拼接
来源：http://pr.shxzukj.cn

"a" .. "b"
来源：http://at.gzmigu.cn

[T38] Lua：条件
来源：http://pu.huixiangedu.cn

if x > 0 then print("正") end
来源：http://tb.newstarts.cn

[T39] Lua：模式匹配
来源：http://fq.nicolike.cn

string.find(s, "%d+")
来源：http://oe.jctech888.com.cn

[T40] Lua：元表
来源：http://mo.jianghongdianzi.cn

setmetatable({}, { __index = base })
来源：http://gl.chemitech.net.cn

[T41] Perl：Hello World
来源：http://pz.bjjhwx.cn

print "Hello\n";
来源：http://rh.521024.cn

[T42] Perl：变量类型
来源：http://zz.huanxung.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lf.newstarts.cn

[T43] Perl：字符串插值
来源：http://pm.bookmarksfly.cn

"值: $a"
来源：http://kq.szsharing.cn

[T44] Perl：条件
来源：http://ld.szsharing.cn

if ($a > 0) { print "正"; }
来源：http://jk.gzmigu.cn

[T45] Perl：数组遍历
来源：http://qa.hahajie.cn

for my $x (@arr) { print $x; }
来源：http://mw.wgjwhj.cn

[T46] Perl：哈希操作
来源：http://pv.szsharing.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pw.asd995.cn

[T47] Perl：正则捕获
来源：http://ce.wgjwhj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://nj.jctech888.com.cn

[T48] Perl：正则替换
来源：http://lv.chemitech.net.cn

$s =~ s/old/new/g;
来源：http://db.asd995.cn

[T49] Perl：函数
来源：http://wy.asd995.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jf.jianghongdianzi.cn

[T50] Perl：逐行读文件
来源：http://kt.jianghongdianzi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://bh.hahajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://ew.jctech888.com.cn

[T51] Scala：Hello World
来源：http://fa.huanxung.cn

println("Hello")
来源：http://bh.huanxung.cn

[T52] Scala：变量
来源：http://vu.shtwfgs.cn

val a = 1;  var b = 2
来源：http://fn.bjjhwx.cn

[T53] Scala：字符串插值
来源：http://wi.jctech888.com.cn

s"值: $b"
来源：http://iy.newstarts.cn

[T54] Scala：集合映射
来源：http://fp.hnjuh.cn

List(1, 2, 3).map(_ * 2)
来源：http://mf.panjiajie.cn

[T55] Scala：集合过滤
来源：http://es.shxzskj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://zr.shxzskj.cn

[T56] Scala：样例类
来源：http://fw.muxihuayi.cn

case class User(name: String, age: Int)
来源：http://pn.chemitech.net.cn

[T57] Scala：模式匹配
来源：http://ul.yuntaijiaju.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ac.lnxyls.cn

[T58] Scala：函数定义
来源：http://sb.yuexingan06.cn

def add(a: Int, b: Int): Int = a + b
来源：http://xe.jianghongdianzi.cn

[T59] Scala：循环
来源：http://pg.panjiajie.cn

for (i <- 1 to 10) println(i)
来源：http://nx.chemitech.net.cn

[T60] Scala：折叠
来源：http://fu.shtwfgs.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fg.521024.cn

================================================================================
来源：http://ik.newstarts.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yh.hahajie.cn

================================================================================
来源：http://dd.shtwfgs.cn

[U01] Py：创建虚拟环境
来源：http://cs.colortex.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zf.nszjky.cn

[U02] Py：导出 / 安装依赖
来源：http://zy.shxzukj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rr.panjiajie.cn

[U03] Py：加载 .env 配置
来源：http://gj.bjjhwx.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ua.9csxet.cn

[U04] Py：变量调试打印
来源：http://zf.521024.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://na.hnjuh.cn

[U05] Py：列表去重且保序
来源：http://ei.521024.cn

list(dict.fromkeys(arr))
来源：http://pe.muxihuayi.cn

[U06] Py：合并两个字典
来源：http://og.bjjhwx.cn

{**a, **b}
来源：http://eq.szxytkj.cn

[U07] Py：反转字典键值
来源：http://cq.colortex.cn

{v: k for k, v in d.items()}
来源：http://xp.huixinmuqiang.cn

[U08] Py：展平二维列表
来源：http://vy.szxytkj.cn

[y for x in nested for y in x]
来源：http://pi.haigaiapp.cn

[U09] Py：字典取最大值的键
来源：http://no.gzmigu.cn

max(d, key=d.get)
来源：http://xt.newstarts.cn

[U10] Py：按值排序字典
来源：http://ho.yuexingan06.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xm.szsharing.cn

[U11] Py：生成器表达式
来源：http://zi.jctech888.com.cn

(x * 2 for x in arr)
来源：http://wv.yuexingan06.cn

[U12] Py：取出现最多的 3 个元素
来源：http://hs.nicolike.cn

Counter(arr).most_common(3)
来源：http://ie.asd995.cn

[U13] Py：固定长度队列
来源：http://qj.huixinmuqiang.cn

deque(maxlen=10)
来源：http://kb.huanxung.cn

[U14] Py：分组收集到列表
来源：http://aw.panjiajie.cn

defaultdict(list)
来源：http://ee.huixinmuqiang.cn

[U15] Py：高精度计时
来源：http://df.lnxyls.cn

t = time.perf_counter()
来源：http://dn.bookmarksfly.cn

[U16] Py：命令行参数解析
来源：http://ip.chemitech.net.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vt.szxytkj.cn

[U17] Py：初始化日志
来源：http://pg.shxzukj.cn

logging.basicConfig(level=logging.INFO)
来源：http://at.521024.cn

[U18] Py：预编译正则
来源：http://ep.szxytkj.cn

pat = re.compile(r"\d+")
来源：http://lh.jctech888.com.cn

[U19] Py：正则替换带回调
来源：http://pg.colortex.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ot.yuexingan06.cn

[U20] Py：缓存函数结果
来源：http://qs.newstarts.cn

@functools.lru_cache(maxsize=None)
来源：http://zb.shtwfgs.cn

[U21] Py：自定义上下文管理器
来源：http://cc.colortex.cn

@contextlib.contextmanager
来源：http://sg.shtwfgs.cn

[U22] Py：矩阵转置
来源：http://eh.jctech888.com.cn

list(zip(*m))
来源：http://wv.shxzukj.cn

[U23] Py：分块读取大文件
来源：http://ad.yuntaijiaju.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xs.shxzukj.cn

[U24] Py：路径操作
来源：http://zm.huixiangedu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qx.muxihuayi.cn

[U25] Py：CSV 按字典读
来源：http://qj.szsharing.cn

csv.DictReader(f)
来源：http://aq.jctech888.com.cn

[U26] Py：并发下载
来源：http://nr.szxytkj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ac.chemitech.net.cn

[U27] Py：异步 HTTP
来源：http://eu.hnjuh.cn

aiohttp.ClientSession() 配合 async with
来源：http://qg.hahajie.cn

[U28] Py：类型别名
来源：http://dn.asd995.cn

UserId = int
来源：http://aj.gzmigu.cn

[U29] Py：属性校验
来源：http://yu.nszjky.cn

@property 与 @x.setter 配合
来源：http://rb.huixinmuqiang.cn

[U30] Py：数据类
来源：http://ce.shxzskj.cn

@dataclass(slots=True)
来源：http://jt.asd995.cn

[U31] Py：单测
来源：http://nr.nicolike.cn

python -m pytest -q
来源：http://ht.shxzskj.cn

[U32] Py：代码格式化
来源：http://ty.yuntaijiaju.cn

ruff format . && ruff check --fix .
来源：http://fv.gzmigu.cn

[U33] Py：打包发布
来源：http://wt.huixinmuqiang.cn

python -m build  （依赖 pyproject.toml）
来源：http://mo.huanxung.cn

[U34] Py：判断编码
来源：http://qo.lnxyls.cn

chardet.detect(raw)
来源：http://vp.huanxung.cn

[U35] Py：发送邮件
来源：http://tp.chemitech.net.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ro.asd995.cn

[U36] Py：定时任务
来源：http://ig.szsharing.cn

schedule.every(10).minutes.do(job)
来源：http://fw.muxihuayi.cn

[U37] Py：读写 Excel
来源：http://up.shxzukj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ma.huixinmuqiang.cn

[U38] Py：获取脚本所在目录
来源：http://rn.jianghongdianzi.cn

Path(__file__).resolve().parent
来源：http://uo.bookmarksfly.cn

[U39] Py：判断是否在交互环境
来源：http://pw.jianghongdianzi.cn

sys.stdout.isatty()
来源：http://jy.nszjky.cn

[U40] Py：打印到标准错误
来源：http://ae.huanxung.cn

print("err", file=sys.stderr)
来源：http://pt.panjiajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://ya.shxzskj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://cs.szxytkj.cn

[U42] PHP：PSR-4 自动加载
来源：http://de.newstarts.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://an.jctech888.com.cn

[U43] PHP：声明命名空间
来源：http://sn.chemitech.net.cn

namespace App\Http;
来源：http://qn.chemitech.net.cn

[U44] PHP：开启严格类型
来源：http://pg.lnxyls.cn

declare(strict_types=1);
来源：http://dk.hahajie.cn

[U45] PHP：类型声明与返回类型
来源：http://uw.newstarts.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://oe.9csxet.cn

[U46] PHP：可空类型
来源：http://og.lnxyls.cn

?string $name = null
来源：http://rp.bjjhwx.cn

[U47] PHP：联合类型
来源：http://jh.jctech888.com.cn

int|string $id
来源：http://et.muxihuayi.cn

[U48] PHP：纯枚举
来源：http://qg.jianghongdianzi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ed.huanxung.cn

[U49] PHP：只读属性
来源：http://yt.huixiangedu.cn

public readonly string $name
来源：http://fn.shxzukj.cn

[U50] PHP：构造器属性提升
来源：http://jc.huixiangedu.cn

public function __construct(private int $id) {}
来源：http://xu.hahajie.cn

[U51] PHP：数组解构
来源：http://wl.yuexingan06.cn

[$a, $b] = $arr;
来源：http://ht.yuntaijiaju.cn

[U52] PHP：箭头函数
来源：http://mp.bookmarksfly.cn

$double = fn($x) => $x * 2;
来源：http://mg.hahajie.cn

[U53] PHP：空合并运算符
来源：http://la.szxytkj.cn

$v = $a ?? $b ?? "default";
来源：http://gs.szxytkj.cn

[U54] PHP：空安全调用
来源：http://py.panjiajie.cn

$obj?->method()
来源：http://im.lnxyls.cn

[U55] PHP：match 表达式
来源：http://vp.haigaiapp.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fz.gzmigu.cn

[U56] PHP：命名参数
来源：http://ct.asd995.cn

f(a: 1, b: 2)
来源：http://uk.asd995.cn

[U57] PHP：字符串插值
来源：http://lg.huanxung.cn

"值: {$a}"
来源：http://dg.hnjuh.cn

[U58] PHP：数组三件套
来源：http://ij.521024.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pe.yuexingan06.cn

[U59] PHP：自定义排序
来源：http://vk.wgjwhj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xd.szsharing.cn

[U60] PHP：JSON 编解码
来源：http://bi.haigaiapp.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kn.shtwfgs.cn

[U61] PHP：正则
来源：http://el.asd995.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kc.szsharing.cn

[U62] PHP：日期对象
来源：http://us.bjjhwx.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ok.panjiajie.cn

[U63] PHP：文件读写
来源：http://wp.shtwfgs.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yr.muxihuayi.cn

[U64] PHP：目录遍历
来源：http://kz.nszjky.cn

glob("dir/*.php");  scandir("dir");
来源：http://ak.yuexingan06.cn

[U65] PHP：会话
来源：http://zf.panjiajie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://cd.szsharing.cn

[U66] PHP：设置 Cookie
来源：http://hy.haigaiapp.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pp.haigaiapp.cn

[U67] PHP：处理文件上传
来源：http://vi.bjjhwx.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xd.shtwfgs.cn

[U68] PHP：PDO 连接
来源：http://yd.huixiangedu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wt.jianghongdianzi.cn

[U69] PHP：PDO 预处理
来源：http://rd.hahajie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wd.shxzukj.cn

[U70] PHP：PDO 事务
来源：http://ct.asd995.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dg.yuntaijiaju.cn

[U71] PHP：抛出异常
来源：http://cv.gzmigu.cn

throw new RuntimeException("失败", 500);
来源：http://ok.yuntaijiaju.cn

[U72] PHP：写错误日志
来源：http://ix.521024.cn

error_log("失败: " . $e->getMessage());
来源：http://at.huixiangedu.cn

[U73] PHP：读取 ini 配置
来源：http://nb.lnxyls.cn

parse_ini_file("config.ini", true)
来源：http://fp.shxzskj.cn

[U74] PHP：读取环境变量
来源：http://ko.muxihuayi.cn

getenv("APP_ENV") ?: "production"
来源：http://pm.panjiajie.cn

[U75] PHP：依赖注入
来源：http://ku.szsharing.cn

composer require psr/container
来源：http://lz.bookmarksfly.cn

[U76] PHP：简单路由
来源：http://mg.bjjhwx.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://np.chemitech.net.cn

[U77] PHP：模板渲染
来源：http://tq.bookmarksfly.cn

composer require twig/twig
来源：http://kb.jctech888.com.cn

[U78] PHP：单元测试
来源：http://sx.haigaiapp.cn

composer require --dev phpunit/phpunit
来源：http://rg.newstarts.cn

[U79] PHP：静态分析
来源：http://gc.jctech888.com.cn

composer require --dev phpstan/phpstan
来源：http://sv.hnjuh.cn

[U80] PHP：代码规范修复
来源：http://pc.shtwfgs.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://pr.huixinmuqiang.cn

[U81] JS：初始化项目
来源：http://wd.yuntaijiaju.cn

npm init -y;  npm i express
来源：http://uj.panjiajie.cn

[U82] JS：package.json 脚本
来源：http://dm.muxihuayi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ap.muxihuayi.cn

[U83] JS：ES Module 导入导出
来源：http://cc.muxihuayi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://tn.szxytkj.cn

[U84] JS：CommonJS 写法
来源：http://fq.yuexingan06.cn

module.exports = { a };  const { a } = require("./m");
来源：http://yr.muxihuayi.cn

[U85] JS：可选链
来源：http://gb.bjjhwx.cn

a?.b?.c
来源：http://sv.jianghongdianzi.cn

[U86] JS：空值合并
来源：http://jq.jianghongdianzi.cn

a ?? b
来源：http://xy.szsharing.cn


<!-- 参考信息 -->