代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://au.yuntaijiaju.cn

================================================================================
来源：http://so.shtwfgs.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ct.shxzukj.cn

================================================================================
来源：http://lf.gzmigu.cn

[T01] Kotlin：Hello World
来源：http://lu.szsharing.cn

println("Hello")
来源：http://et.hahajie.cn

[T02] Kotlin：变量
来源：http://ca.9csxet.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gn.huixinmuqiang.cn

[T03] Kotlin：字符串模板
来源：http://yd.huixinmuqiang.cn

"值: $b"
来源：http://yv.huixinmuqiang.cn

[T04] Kotlin：空安全
来源：http://fg.wgjwhj.cn

val n: String? = null;  n?.length
来源：http://zy.panjiajie.cn

[T05] Kotlin：when 表达式
来源：http://gd.521024.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bw.wgjwhj.cn

[T06] Kotlin：集合映射
来源：http://ja.asd995.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://vq.szsharing.cn

[T07] Kotlin：集合过滤
来源：http://hh.hahajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://jg.huixiangedu.cn

[T08] Kotlin：数据类
来源：http://hj.nszjky.cn

data class User(val name: String, val age: Int)
来源：http://ml.szxytkj.cn

[T09] Kotlin：扩展函数
来源：http://vr.muxihuayi.cn

fun String.exclaim() = this + "!"
来源：http://am.newstarts.cn

[T10] Kotlin：默认参数
来源：http://og.hnjuh.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rm.newstarts.cn

[T11] Kotlin：协程
来源：http://pn.panjiajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nj.huixiangedu.cn

[T12] Kotlin：解构声明
来源：http://pk.gzmigu.cn

val (a, b) = Pair(1, 2)
来源：http://jb.muxihuayi.cn

[T13] Kotlin：只读 Map
来源：http://wa.jctech888.com.cn

val m = mapOf("a" to 1)
来源：http://pr.szsharing.cn

[T14] Kotlin：循环
来源：http://pt.chemitech.net.cn

for (i in 1..10) println(i)
来源：http://jn.jianghongdianzi.cn

[T15] Kotlin：接口
来源：http://wi.jctech888.com.cn

interface Shape { fun area(): Double }
来源：http://ku.shxzukj.cn

[T16] Swift：Hello World
来源：http://dy.chemitech.net.cn

print("Hello")
来源：http://ug.wgjwhj.cn

[T17] Swift：变量与常量
来源：http://qt.hahajie.cn

var a = 1;  let b = 2
来源：http://ls.panjiajie.cn

[T18] Swift：字符串插值
来源：http://pf.nszjky.cn

"值: \(b)"
来源：http://ax.asd995.cn

[T19] Swift：可选绑定
来源：http://or.newstarts.cn

if let n = opt { print(n) }
来源：http://jn.szxytkj.cn

[T20] Swift：数组操作
来源：http://ty.jctech888.com.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ih.szsharing.cn

[T21] Swift：遍历
来源：http://bv.chemitech.net.cn

for x in a { print(x) }
来源：http://cm.huixiangedu.cn

[T22] Swift：字典
来源：http://ra.panjiajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://jw.gzmigu.cn

[T23] Swift：函数
来源：http://gg.gzmigu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ws.huixiangedu.cn

[T24] Swift：闭包
来源：http://rl.yuexingan06.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gc.nicolike.cn

[T25] Swift：结构体
来源：http://ve.asd995.cn

struct P { var x: Int }
来源：http://wp.haigaiapp.cn

[T26] Swift：类与重写
来源：http://ae.shtwfgs.cn

class A: Base { override func f() {} }
来源：http://mo.yuntaijiaju.cn

[T27] Swift：错误处理
来源：http://pv.yuexingan06.cn

do { try f() } catch { print(error) }
来源：http://hj.haigaiapp.cn

[T28] Swift：枚举
来源：http://fu.shxzskj.cn

enum Color { case red, green }
来源：http://yr.wgjwhj.cn

[T29] Swift：guard 提前返回
来源：http://ny.bookmarksfly.cn

guard let x = opt else { return }
来源：http://hh.shtwfgs.cn

[T30] Swift：协议
来源：http://rd.hnjuh.cn

protocol Shape { func area() -> Double }
来源：http://ab.huanxung.cn

[T31] Lua：Hello World
来源：http://ph.huanxung.cn

print("Hello")
来源：http://md.szsharing.cn

[T32] Lua：局部变量
来源：http://ls.huixiangedu.cn

local a = 1
来源：http://kr.newstarts.cn

[T33] Lua：表（数组）
来源：http://bv.szsharing.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://bp.nszjky.cn

[T34] Lua：遍历表
来源：http://zl.hahajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ux.521024.cn

[T35] Lua：字典表
来源：http://sb.hahajie.cn

local d = { a = 1 };  d.b = 2
来源：http://lg.nszjky.cn

[T36] Lua：函数
来源：http://km.shxzukj.cn

function add(a, b) return a + b end
来源：http://je.newstarts.cn

[T37] Lua：字符串拼接
来源：http://ra.huixinmuqiang.cn

"a" .. "b"
来源：http://gf.nszjky.cn

[T38] Lua：条件
来源：http://xu.szxytkj.cn

if x > 0 then print("正") end
来源：http://dq.huanxung.cn

[T39] Lua：模式匹配
来源：http://jg.newstarts.cn

string.find(s, "%d+")
来源：http://bm.huanxung.cn

[T40] Lua：元表
来源：http://cf.shxzskj.cn

setmetatable({}, { __index = base })
来源：http://kn.panjiajie.cn

[T41] Perl：Hello World
来源：http://jq.haigaiapp.cn

print "Hello\n";
来源：http://rc.hnjuh.cn

[T42] Perl：变量类型
来源：http://jj.huixinmuqiang.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qn.shxzukj.cn

[T43] Perl：字符串插值
来源：http://cd.huanxung.cn

"值: $a"
来源：http://kb.wgjwhj.cn

[T44] Perl：条件
来源：http://mr.nicolike.cn

if ($a > 0) { print "正"; }
来源：http://je.shxzukj.cn

[T45] Perl：数组遍历
来源：http://cz.hnjuh.cn

for my $x (@arr) { print $x; }
来源：http://qu.colortex.cn

[T46] Perl：哈希操作
来源：http://cj.newstarts.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fo.bookmarksfly.cn

[T47] Perl：正则捕获
来源：http://he.muxihuayi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xv.muxihuayi.cn

[T48] Perl：正则替换
来源：http://ch.wgjwhj.cn

$s =~ s/old/new/g;
来源：http://vs.wgjwhj.cn

[T49] Perl：函数
来源：http://pq.jianghongdianzi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ne.hahajie.cn

[T50] Perl：逐行读文件
来源：http://oi.colortex.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zd.shxzukj.cn

while (my $line = <$fh>) { print $line; }
来源：http://lz.bookmarksfly.cn

[T51] Scala：Hello World
来源：http://kl.shtwfgs.cn

println("Hello")
来源：http://ua.muxihuayi.cn

[T52] Scala：变量
来源：http://lu.colortex.cn

val a = 1;  var b = 2
来源：http://qb.wgjwhj.cn

[T53] Scala：字符串插值
来源：http://ai.hnjuh.cn

s"值: $b"
来源：http://jl.huanxung.cn

[T54] Scala：集合映射
来源：http://zo.haigaiapp.cn

List(1, 2, 3).map(_ * 2)
来源：http://qe.lnxyls.cn

[T55] Scala：集合过滤
来源：http://sc.nszjky.cn

List(1, 2, 3).filter(_ > 1)
来源：http://bh.9csxet.cn

[T56] Scala：样例类
来源：http://ou.szxytkj.cn

case class User(name: String, age: Int)
来源：http://ep.bjjhwx.cn

[T57] Scala：模式匹配
来源：http://ii.szsharing.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ko.szxytkj.cn

[T58] Scala：函数定义
来源：http://ly.szxytkj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://kt.nszjky.cn

[T59] Scala：循环
来源：http://id.newstarts.cn

for (i <- 1 to 10) println(i)
来源：http://ce.szxytkj.cn

[T60] Scala：折叠
来源：http://uo.jianghongdianzi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xp.hahajie.cn

================================================================================
来源：http://re.521024.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ud.yuexingan06.cn

================================================================================
来源：http://md.521024.cn

[U01] Py：创建虚拟环境
来源：http://zu.jianghongdianzi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://xq.shtwfgs.cn

[U02] Py：导出 / 安装依赖
来源：http://eg.newstarts.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uj.asd995.cn

[U03] Py：加载 .env 配置
来源：http://qa.521024.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gc.chemitech.net.cn

[U04] Py：变量调试打印
来源：http://hr.shtwfgs.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fa.521024.cn

[U05] Py：列表去重且保序
来源：http://kr.szsharing.cn

list(dict.fromkeys(arr))
来源：http://nw.huanxung.cn

[U06] Py：合并两个字典
来源：http://sj.hahajie.cn

{**a, **b}
来源：http://cl.bookmarksfly.cn

[U07] Py：反转字典键值
来源：http://rd.shxzskj.cn

{v: k for k, v in d.items()}
来源：http://bv.wgjwhj.cn

[U08] Py：展平二维列表
来源：http://fd.lnxyls.cn

[y for x in nested for y in x]
来源：http://ph.hnjuh.cn

[U09] Py：字典取最大值的键
来源：http://ke.nszjky.cn

max(d, key=d.get)
来源：http://vr.shxzukj.cn

[U10] Py：按值排序字典
来源：http://te.panjiajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bb.muxihuayi.cn

[U11] Py：生成器表达式
来源：http://xc.asd995.cn

(x * 2 for x in arr)
来源：http://or.shxzukj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://cz.nszjky.cn

Counter(arr).most_common(3)
来源：http://gi.nszjky.cn

[U13] Py：固定长度队列
来源：http://nt.chemitech.net.cn

deque(maxlen=10)
来源：http://nt.huanxung.cn

[U14] Py：分组收集到列表
来源：http://zp.colortex.cn

defaultdict(list)
来源：http://kw.huanxung.cn

[U15] Py：高精度计时
来源：http://la.shxzukj.cn

t = time.perf_counter()
来源：http://se.shtwfgs.cn

[U16] Py：命令行参数解析
来源：http://bp.hnjuh.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://su.colortex.cn

[U17] Py：初始化日志
来源：http://vb.shxzskj.cn

logging.basicConfig(level=logging.INFO)
来源：http://ad.haigaiapp.cn

[U18] Py：预编译正则
来源：http://qb.9csxet.cn

pat = re.compile(r"\d+")
来源：http://zp.9csxet.cn

[U19] Py：正则替换带回调
来源：http://rt.bookmarksfly.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rr.521024.cn

[U20] Py：缓存函数结果
来源：http://kr.szxytkj.cn

@functools.lru_cache(maxsize=None)
来源：http://ln.bookmarksfly.cn

[U21] Py：自定义上下文管理器
来源：http://xt.gzmigu.cn

@contextlib.contextmanager
来源：http://sg.9csxet.cn

[U22] Py：矩阵转置
来源：http://lp.shxzukj.cn

list(zip(*m))
来源：http://zf.shtwfgs.cn

[U23] Py：分块读取大文件
来源：http://yr.colortex.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tp.szxytkj.cn

[U24] Py：路径操作
来源：http://da.chemitech.net.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://oq.shxzukj.cn

[U25] Py：CSV 按字典读
来源：http://dd.huixiangedu.cn

csv.DictReader(f)
来源：http://rx.szsharing.cn

[U26] Py：并发下载
来源：http://ih.nszjky.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ng.bjjhwx.cn

[U27] Py：异步 HTTP
来源：http://ok.newstarts.cn

aiohttp.ClientSession() 配合 async with
来源：http://yi.newstarts.cn

[U28] Py：类型别名
来源：http://wc.haigaiapp.cn

UserId = int
来源：http://xn.hahajie.cn

[U29] Py：属性校验
来源：http://ep.huixiangedu.cn

@property 与 @x.setter 配合
来源：http://cn.lnxyls.cn

[U30] Py：数据类
来源：http://vf.huanxung.cn

@dataclass(slots=True)
来源：http://gw.colortex.cn

[U31] Py：单测
来源：http://bo.bookmarksfly.cn

python -m pytest -q
来源：http://ny.hnjuh.cn

[U32] Py：代码格式化
来源：http://qx.panjiajie.cn

ruff format . && ruff check --fix .
来源：http://cn.colortex.cn

[U33] Py：打包发布
来源：http://eq.nszjky.cn

python -m build  （依赖 pyproject.toml）
来源：http://dm.jianghongdianzi.cn

[U34] Py：判断编码
来源：http://yt.bjjhwx.cn

chardet.detect(raw)
来源：http://mc.hahajie.cn

[U35] Py：发送邮件
来源：http://iz.yuexingan06.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pf.521024.cn

[U36] Py：定时任务
来源：http://dx.colortex.cn

schedule.every(10).minutes.do(job)
来源：http://ux.szsharing.cn

[U37] Py：读写 Excel
来源：http://qa.9csxet.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wi.9csxet.cn

[U38] Py：获取脚本所在目录
来源：http://an.jianghongdianzi.cn

Path(__file__).resolve().parent
来源：http://zw.muxihuayi.cn

[U39] Py：判断是否在交互环境
来源：http://ue.9csxet.cn

sys.stdout.isatty()
来源：http://mq.colortex.cn

[U40] Py：打印到标准错误
来源：http://ad.chemitech.net.cn

print("err", file=sys.stderr)
来源：http://ov.haigaiapp.cn

[U41] PHP：初始化 Composer 项目
来源：http://br.jianghongdianzi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zi.shxzukj.cn

[U42] PHP：PSR-4 自动加载
来源：http://fl.szxytkj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rs.huixiangedu.cn

[U43] PHP：声明命名空间
来源：http://ed.newstarts.cn

namespace App\Http;
来源：http://su.nszjky.cn

[U44] PHP：开启严格类型
来源：http://ul.huanxung.cn

declare(strict_types=1);
来源：http://zy.muxihuayi.cn

[U45] PHP：类型声明与返回类型
来源：http://io.bjjhwx.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://lw.haigaiapp.cn

[U46] PHP：可空类型
来源：http://un.9csxet.cn

?string $name = null
来源：http://ha.muxihuayi.cn

[U47] PHP：联合类型
来源：http://tj.colortex.cn

int|string $id
来源：http://yj.hnjuh.cn

[U48] PHP：纯枚举
来源：http://xw.bjjhwx.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mv.shxzukj.cn

[U49] PHP：只读属性
来源：http://zb.huanxung.cn

public readonly string $name
来源：http://xq.gzmigu.cn

[U50] PHP：构造器属性提升
来源：http://ta.asd995.cn

public function __construct(private int $id) {}
来源：http://nb.shxzukj.cn

[U51] PHP：数组解构
来源：http://gk.szsharing.cn

[$a, $b] = $arr;
来源：http://hx.nicolike.cn

[U52] PHP：箭头函数
来源：http://ni.chemitech.net.cn

$double = fn($x) => $x * 2;
来源：http://kd.gzmigu.cn

[U53] PHP：空合并运算符
来源：http://ya.bjjhwx.cn

$v = $a ?? $b ?? "default";
来源：http://dx.muxihuayi.cn

[U54] PHP：空安全调用
来源：http://am.jianghongdianzi.cn

$obj?->method()
来源：http://wy.bookmarksfly.cn

[U55] PHP：match 表达式
来源：http://nl.huixinmuqiang.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zs.shxzskj.cn

[U56] PHP：命名参数
来源：http://ps.bjjhwx.cn

f(a: 1, b: 2)
来源：http://xq.nszjky.cn

[U57] PHP：字符串插值
来源：http://kd.gzmigu.cn

"值: {$a}"
来源：http://cm.szxytkj.cn

[U58] PHP：数组三件套
来源：http://cp.huanxung.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ug.9csxet.cn

[U59] PHP：自定义排序
来源：http://wt.shxzskj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xt.hahajie.cn

[U60] PHP：JSON 编解码
来源：http://tj.gzmigu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xx.yuntaijiaju.cn

[U61] PHP：正则
来源：http://ut.shtwfgs.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sx.hahajie.cn

[U62] PHP：日期对象
来源：http://ok.bookmarksfly.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ts.hnjuh.cn

[U63] PHP：文件读写
来源：http://nz.lnxyls.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bk.chemitech.net.cn

[U64] PHP：目录遍历
来源：http://xp.yuexingan06.cn

glob("dir/*.php");  scandir("dir");
来源：http://gh.colortex.cn

[U65] PHP：会话
来源：http://vp.shtwfgs.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://su.nicolike.cn

[U66] PHP：设置 Cookie
来源：http://lg.szsharing.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://oe.yuexingan06.cn

[U67] PHP：处理文件上传
来源：http://yq.jctech888.com.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rn.bookmarksfly.cn

[U68] PHP：PDO 连接
来源：http://qz.jctech888.com.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zm.hnjuh.cn

[U69] PHP：PDO 预处理
来源：http://en.wgjwhj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://io.shxzukj.cn

[U70] PHP：PDO 事务
来源：http://ak.huixiangedu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ic.gzmigu.cn

[U71] PHP：抛出异常
来源：http://ub.huanxung.cn

throw new RuntimeException("失败", 500);
来源：http://hl.wgjwhj.cn

[U72] PHP：写错误日志
来源：http://tr.wgjwhj.cn

error_log("失败: " . $e->getMessage());
来源：http://yf.lnxyls.cn

[U73] PHP：读取 ini 配置
来源：http://ws.521024.cn

parse_ini_file("config.ini", true)
来源：http://vr.jianghongdianzi.cn

[U74] PHP：读取环境变量
来源：http://du.hnjuh.cn

getenv("APP_ENV") ?: "production"
来源：http://gj.szxytkj.cn

[U75] PHP：依赖注入
来源：http://ki.chemitech.net.cn

composer require psr/container
来源：http://pm.shxzskj.cn

[U76] PHP：简单路由
来源：http://vj.yuexingan06.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ir.panjiajie.cn

[U77] PHP：模板渲染
来源：http://fh.521024.cn

composer require twig/twig
来源：http://mz.szsharing.cn

[U78] PHP：单元测试
来源：http://py.nszjky.cn

composer require --dev phpunit/phpunit
来源：http://eh.asd995.cn

[U79] PHP：静态分析
来源：http://gn.haigaiapp.cn

composer require --dev phpstan/phpstan
来源：http://rv.huanxung.cn

[U80] PHP：代码规范修复
来源：http://yv.bookmarksfly.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://hm.nszjky.cn

[U81] JS：初始化项目
来源：http://hh.haigaiapp.cn

npm init -y;  npm i express
来源：http://gw.huixinmuqiang.cn

[U82] JS：package.json 脚本
来源：http://nv.nicolike.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lv.szsharing.cn

[U83] JS：ES Module 导入导出
来源：http://zg.huixiangedu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ho.newstarts.cn

[U84] JS：CommonJS 写法
来源：http://qm.jctech888.com.cn

module.exports = { a };  const { a } = require("./m");
来源：http://lc.gzmigu.cn

[U85] JS：可选链
来源：http://oh.shxzskj.cn

a?.b?.c
来源：http://bn.bjjhwx.cn

[U86] JS：空值合并
来源：http://zx.haigaiapp.cn

a ?? b
来源：http://qn.hnjuh.cn


<!-- 参考信息 -->