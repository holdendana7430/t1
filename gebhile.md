代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://el.yuexingan06.cn

================================================================================
来源：http://il.panjiajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fv.muxihuayi.cn

================================================================================
来源：http://ur.huixinmuqiang.cn

[T01] Kotlin：Hello World
来源：http://vn.newstarts.cn

println("Hello")
来源：http://rz.shtwfgs.cn

[T02] Kotlin：变量
来源：http://bb.shxzukj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qt.haigaiapp.cn

[T03] Kotlin：字符串模板
来源：http://pw.hahajie.cn

"值: $b"
来源：http://jc.hahajie.cn

[T04] Kotlin：空安全
来源：http://pl.huanxung.cn

val n: String? = null;  n?.length
来源：http://cy.yuntaijiaju.cn

[T05] Kotlin：when 表达式
来源：http://wf.jctech888.com.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pv.bookmarksfly.cn

[T06] Kotlin：集合映射
来源：http://zo.muxihuayi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://sl.bookmarksfly.cn

[T07] Kotlin：集合过滤
来源：http://ck.bookmarksfly.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://df.szsharing.cn

[T08] Kotlin：数据类
来源：http://oq.lnxyls.cn

data class User(val name: String, val age: Int)
来源：http://vd.szsharing.cn

[T09] Kotlin：扩展函数
来源：http://cx.szsharing.cn

fun String.exclaim() = this + "!"
来源：http://us.huixinmuqiang.cn

[T10] Kotlin：默认参数
来源：http://yn.huixiangedu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://br.bookmarksfly.cn

[T11] Kotlin：协程
来源：http://ec.bookmarksfly.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://cn.chemitech.net.cn

[T12] Kotlin：解构声明
来源：http://fd.shxzukj.cn

val (a, b) = Pair(1, 2)
来源：http://jp.muxihuayi.cn

[T13] Kotlin：只读 Map
来源：http://tq.huanxung.cn

val m = mapOf("a" to 1)
来源：http://lm.jctech888.com.cn

[T14] Kotlin：循环
来源：http://sv.nicolike.cn

for (i in 1..10) println(i)
来源：http://xj.wgjwhj.cn

[T15] Kotlin：接口
来源：http://ol.muxihuayi.cn

interface Shape { fun area(): Double }
来源：http://kw.asd995.cn

[T16] Swift：Hello World
来源：http://ih.huixinmuqiang.cn

print("Hello")
来源：http://sh.gzmigu.cn

[T17] Swift：变量与常量
来源：http://lh.szxytkj.cn

var a = 1;  let b = 2
来源：http://es.shxzskj.cn

[T18] Swift：字符串插值
来源：http://vr.gzmigu.cn

"值: \(b)"
来源：http://nm.hnjuh.cn

[T19] Swift：可选绑定
来源：http://uy.szxytkj.cn

if let n = opt { print(n) }
来源：http://do.jianghongdianzi.cn

[T20] Swift：数组操作
来源：http://wr.chemitech.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://rg.chemitech.net.cn

[T21] Swift：遍历
来源：http://yz.9csxet.cn

for x in a { print(x) }
来源：http://bk.shtwfgs.cn

[T22] Swift：字典
来源：http://eh.lnxyls.cn

var d = ["a": 1];  d["b"] = 2
来源：http://qo.chemitech.net.cn

[T23] Swift：函数
来源：http://wj.nszjky.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kh.lnxyls.cn

[T24] Swift：闭包
来源：http://ys.bookmarksfly.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ae.bookmarksfly.cn

[T25] Swift：结构体
来源：http://fp.chemitech.net.cn

struct P { var x: Int }
来源：http://bo.huanxung.cn

[T26] Swift：类与重写
来源：http://jv.hahajie.cn

class A: Base { override func f() {} }
来源：http://sz.haigaiapp.cn

[T27] Swift：错误处理
来源：http://kf.huixiangedu.cn

do { try f() } catch { print(error) }
来源：http://el.szxytkj.cn

[T28] Swift：枚举
来源：http://fg.szsharing.cn

enum Color { case red, green }
来源：http://bu.hnjuh.cn

[T29] Swift：guard 提前返回
来源：http://aj.colortex.cn

guard let x = opt else { return }
来源：http://sx.haigaiapp.cn

[T30] Swift：协议
来源：http://bl.huixiangedu.cn

protocol Shape { func area() -> Double }
来源：http://ao.521024.cn

[T31] Lua：Hello World
来源：http://qo.huixiangedu.cn

print("Hello")
来源：http://et.haigaiapp.cn

[T32] Lua：局部变量
来源：http://mj.huanxung.cn

local a = 1
来源：http://ei.haigaiapp.cn

[T33] Lua：表（数组）
来源：http://gn.muxihuayi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ke.hahajie.cn

[T34] Lua：遍历表
来源：http://dl.asd995.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ik.nszjky.cn

[T35] Lua：字典表
来源：http://kb.hnjuh.cn

local d = { a = 1 };  d.b = 2
来源：http://hk.521024.cn

[T36] Lua：函数
来源：http://qu.shxzskj.cn

function add(a, b) return a + b end
来源：http://fp.nicolike.cn

[T37] Lua：字符串拼接
来源：http://ow.bjjhwx.cn

"a" .. "b"
来源：http://uo.chemitech.net.cn

[T38] Lua：条件
来源：http://wi.shxzukj.cn

if x > 0 then print("正") end
来源：http://ch.hahajie.cn

[T39] Lua：模式匹配
来源：http://rd.9csxet.cn

string.find(s, "%d+")
来源：http://qc.bjjhwx.cn

[T40] Lua：元表
来源：http://vn.jianghongdianzi.cn

setmetatable({}, { __index = base })
来源：http://cp.shxzukj.cn

[T41] Perl：Hello World
来源：http://ea.9csxet.cn

print "Hello\n";
来源：http://ze.chemitech.net.cn

[T42] Perl：变量类型
来源：http://rd.newstarts.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pn.bjjhwx.cn

[T43] Perl：字符串插值
来源：http://pv.newstarts.cn

"值: $a"
来源：http://kd.wgjwhj.cn

[T44] Perl：条件
来源：http://jq.nicolike.cn

if ($a > 0) { print "正"; }
来源：http://rw.haigaiapp.cn

[T45] Perl：数组遍历
来源：http://ue.wgjwhj.cn

for my $x (@arr) { print $x; }
来源：http://fx.huixiangedu.cn

[T46] Perl：哈希操作
来源：http://mq.gzmigu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qf.wgjwhj.cn

[T47] Perl：正则捕获
来源：http://dg.jctech888.com.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wy.asd995.cn

[T48] Perl：正则替换
来源：http://mz.bookmarksfly.cn

$s =~ s/old/new/g;
来源：http://da.shtwfgs.cn

[T49] Perl：函数
来源：http://gx.colortex.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ts.wgjwhj.cn

[T50] Perl：逐行读文件
来源：http://ww.huixiangedu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://me.huanxung.cn

while (my $line = <$fh>) { print $line; }
来源：http://cm.panjiajie.cn

[T51] Scala：Hello World
来源：http://ft.bjjhwx.cn

println("Hello")
来源：http://su.huanxung.cn

[T52] Scala：变量
来源：http://kb.lnxyls.cn

val a = 1;  var b = 2
来源：http://ns.bjjhwx.cn

[T53] Scala：字符串插值
来源：http://wp.jianghongdianzi.cn

s"值: $b"
来源：http://nq.yuntaijiaju.cn

[T54] Scala：集合映射
来源：http://wa.newstarts.cn

List(1, 2, 3).map(_ * 2)
来源：http://vw.yuntaijiaju.cn

[T55] Scala：集合过滤
来源：http://hb.asd995.cn

List(1, 2, 3).filter(_ > 1)
来源：http://px.shtwfgs.cn

[T56] Scala：样例类
来源：http://hy.wgjwhj.cn

case class User(name: String, age: Int)
来源：http://ly.hahajie.cn

[T57] Scala：模式匹配
来源：http://pa.nszjky.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ph.nszjky.cn

[T58] Scala：函数定义
来源：http://pe.yuexingan06.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fr.shtwfgs.cn

[T59] Scala：循环
来源：http://xg.szxytkj.cn

for (i <- 1 to 10) println(i)
来源：http://lj.lnxyls.cn

[T60] Scala：折叠
来源：http://et.newstarts.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://go.shxzskj.cn

================================================================================
来源：http://fo.szxytkj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rm.hnjuh.cn

================================================================================
来源：http://eu.shxzskj.cn

[U01] Py：创建虚拟环境
来源：http://bq.yuntaijiaju.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ai.jianghongdianzi.cn

[U02] Py：导出 / 安装依赖
来源：http://ne.yuntaijiaju.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mc.shxzukj.cn

[U03] Py：加载 .env 配置
来源：http://fb.huanxung.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://je.hnjuh.cn

[U04] Py：变量调试打印
来源：http://oq.huixiangedu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lv.panjiajie.cn

[U05] Py：列表去重且保序
来源：http://xf.huanxung.cn

list(dict.fromkeys(arr))
来源：http://ha.panjiajie.cn

[U06] Py：合并两个字典
来源：http://mv.huanxung.cn

{**a, **b}
来源：http://ky.shxzukj.cn

[U07] Py：反转字典键值
来源：http://gq.nicolike.cn

{v: k for k, v in d.items()}
来源：http://rv.muxihuayi.cn

[U08] Py：展平二维列表
来源：http://xu.newstarts.cn

[y for x in nested for y in x]
来源：http://if.szxytkj.cn

[U09] Py：字典取最大值的键
来源：http://fe.colortex.cn

max(d, key=d.get)
来源：http://rq.521024.cn

[U10] Py：按值排序字典
来源：http://hh.521024.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://od.jianghongdianzi.cn

[U11] Py：生成器表达式
来源：http://zd.bookmarksfly.cn

(x * 2 for x in arr)
来源：http://pk.huixinmuqiang.cn

[U12] Py：取出现最多的 3 个元素
来源：http://sc.szxytkj.cn

Counter(arr).most_common(3)
来源：http://lg.colortex.cn

[U13] Py：固定长度队列
来源：http://lo.chemitech.net.cn

deque(maxlen=10)
来源：http://kd.bjjhwx.cn

[U14] Py：分组收集到列表
来源：http://zz.panjiajie.cn

defaultdict(list)
来源：http://dg.521024.cn

[U15] Py：高精度计时
来源：http://qf.szsharing.cn

t = time.perf_counter()
来源：http://mo.nszjky.cn

[U16] Py：命令行参数解析
来源：http://or.huanxung.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nz.shxzukj.cn

[U17] Py：初始化日志
来源：http://at.shxzukj.cn

logging.basicConfig(level=logging.INFO)
来源：http://kb.huanxung.cn

[U18] Py：预编译正则
来源：http://se.muxihuayi.cn

pat = re.compile(r"\d+")
来源：http://ll.huixinmuqiang.cn

[U19] Py：正则替换带回调
来源：http://qx.huixiangedu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://iy.colortex.cn

[U20] Py：缓存函数结果
来源：http://cb.nicolike.cn

@functools.lru_cache(maxsize=None)
来源：http://mq.newstarts.cn

[U21] Py：自定义上下文管理器
来源：http://wu.bookmarksfly.cn

@contextlib.contextmanager
来源：http://nz.shxzskj.cn

[U22] Py：矩阵转置
来源：http://dj.nicolike.cn

list(zip(*m))
来源：http://au.lnxyls.cn

[U23] Py：分块读取大文件
来源：http://wp.yuntaijiaju.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tp.gzmigu.cn

[U24] Py：路径操作
来源：http://yr.huanxung.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://aa.yuexingan06.cn

[U25] Py：CSV 按字典读
来源：http://ja.shxzukj.cn

csv.DictReader(f)
来源：http://gb.nszjky.cn

[U26] Py：并发下载
来源：http://ig.chemitech.net.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vu.jianghongdianzi.cn

[U27] Py：异步 HTTP
来源：http://eg.shxzskj.cn

aiohttp.ClientSession() 配合 async with
来源：http://gw.shxzukj.cn

[U28] Py：类型别名
来源：http://zs.hnjuh.cn

UserId = int
来源：http://cf.shtwfgs.cn

[U29] Py：属性校验
来源：http://bn.szsharing.cn

@property 与 @x.setter 配合
来源：http://gq.shxzskj.cn

[U30] Py：数据类
来源：http://ld.yuexingan06.cn

@dataclass(slots=True)
来源：http://uo.haigaiapp.cn

[U31] Py：单测
来源：http://yy.colortex.cn

python -m pytest -q
来源：http://gu.szxytkj.cn

[U32] Py：代码格式化
来源：http://ki.yuntaijiaju.cn

ruff format . && ruff check --fix .
来源：http://xj.shtwfgs.cn

[U33] Py：打包发布
来源：http://wv.huixinmuqiang.cn

python -m build  （依赖 pyproject.toml）
来源：http://cn.bookmarksfly.cn

[U34] Py：判断编码
来源：http://tf.asd995.cn

chardet.detect(raw)
来源：http://ul.huanxung.cn

[U35] Py：发送邮件
来源：http://st.jctech888.com.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yk.yuntaijiaju.cn

[U36] Py：定时任务
来源：http://fi.gzmigu.cn

schedule.every(10).minutes.do(job)
来源：http://dp.chemitech.net.cn

[U37] Py：读写 Excel
来源：http://kw.521024.cn

pandas.read_excel / DataFrame.to_excel
来源：http://zy.huixiangedu.cn

[U38] Py：获取脚本所在目录
来源：http://qe.9csxet.cn

Path(__file__).resolve().parent
来源：http://lf.521024.cn

[U39] Py：判断是否在交互环境
来源：http://vj.bookmarksfly.cn

sys.stdout.isatty()
来源：http://tn.muxihuayi.cn

[U40] Py：打印到标准错误
来源：http://ai.yuntaijiaju.cn

print("err", file=sys.stderr)
来源：http://ik.hahajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://is.shxzskj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ug.hahajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://pc.szsharing.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ra.asd995.cn

[U43] PHP：声明命名空间
来源：http://lw.wgjwhj.cn

namespace App\Http;
来源：http://jr.colortex.cn

[U44] PHP：开启严格类型
来源：http://qy.hnjuh.cn

declare(strict_types=1);
来源：http://ks.shxzskj.cn

[U45] PHP：类型声明与返回类型
来源：http://py.shxzskj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://xr.shtwfgs.cn

[U46] PHP：可空类型
来源：http://zn.wgjwhj.cn

?string $name = null
来源：http://du.yuntaijiaju.cn

[U47] PHP：联合类型
来源：http://cm.bjjhwx.cn

int|string $id
来源：http://eg.colortex.cn

[U48] PHP：纯枚举
来源：http://uo.jctech888.com.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://df.bookmarksfly.cn

[U49] PHP：只读属性
来源：http://zj.yuexingan06.cn

public readonly string $name
来源：http://km.szsharing.cn

[U50] PHP：构造器属性提升
来源：http://zl.wgjwhj.cn

public function __construct(private int $id) {}
来源：http://vl.9csxet.cn

[U51] PHP：数组解构
来源：http://rh.chemitech.net.cn

[$a, $b] = $arr;
来源：http://sh.nicolike.cn

[U52] PHP：箭头函数
来源：http://qe.yuexingan06.cn

$double = fn($x) => $x * 2;
来源：http://vp.szxytkj.cn

[U53] PHP：空合并运算符
来源：http://nq.jctech888.com.cn

$v = $a ?? $b ?? "default";
来源：http://fp.shxzskj.cn

[U54] PHP：空安全调用
来源：http://mx.jctech888.com.cn

$obj?->method()
来源：http://sg.huixinmuqiang.cn

[U55] PHP：match 表达式
来源：http://rv.lnxyls.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bv.huixinmuqiang.cn

[U56] PHP：命名参数
来源：http://an.yuntaijiaju.cn

f(a: 1, b: 2)
来源：http://vx.hnjuh.cn

[U57] PHP：字符串插值
来源：http://ce.wgjwhj.cn

"值: {$a}"
来源：http://pk.bookmarksfly.cn

[U58] PHP：数组三件套
来源：http://lh.szsharing.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://iy.haigaiapp.cn

[U59] PHP：自定义排序
来源：http://mr.yuntaijiaju.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bs.521024.cn

[U60] PHP：JSON 编解码
来源：http://lc.gzmigu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jh.shxzukj.cn

[U61] PHP：正则
来源：http://pe.hahajie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rd.yuntaijiaju.cn

[U62] PHP：日期对象
来源：http://bp.huixiangedu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ms.szsharing.cn

[U63] PHP：文件读写
来源：http://bh.521024.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xi.521024.cn

[U64] PHP：目录遍历
来源：http://cl.9csxet.cn

glob("dir/*.php");  scandir("dir");
来源：http://tw.wgjwhj.cn

[U65] PHP：会话
来源：http://ik.haigaiapp.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://lj.jctech888.com.cn

[U66] PHP：设置 Cookie
来源：http://uj.shxzskj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mn.shtwfgs.cn

[U67] PHP：处理文件上传
来源：http://hg.newstarts.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kx.lnxyls.cn

[U68] PHP：PDO 连接
来源：http://ba.colortex.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tr.nszjky.cn

[U69] PHP：PDO 预处理
来源：http://fj.newstarts.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tq.huixiangedu.cn

[U70] PHP：PDO 事务
来源：http://sm.huixiangedu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jv.chemitech.net.cn

[U71] PHP：抛出异常
来源：http://qa.huanxung.cn

throw new RuntimeException("失败", 500);
来源：http://aw.colortex.cn

[U72] PHP：写错误日志
来源：http://gi.9csxet.cn

error_log("失败: " . $e->getMessage());
来源：http://vv.huixinmuqiang.cn

[U73] PHP：读取 ini 配置
来源：http://ml.chemitech.net.cn

parse_ini_file("config.ini", true)
来源：http://xz.jctech888.com.cn

[U74] PHP：读取环境变量
来源：http://wf.shtwfgs.cn

getenv("APP_ENV") ?: "production"
来源：http://fd.haigaiapp.cn

[U75] PHP：依赖注入
来源：http://ss.wgjwhj.cn

composer require psr/container
来源：http://mj.gzmigu.cn

[U76] PHP：简单路由
来源：http://kh.huanxung.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gx.panjiajie.cn

[U77] PHP：模板渲染
来源：http://mb.muxihuayi.cn

composer require twig/twig
来源：http://ow.shxzukj.cn

[U78] PHP：单元测试
来源：http://po.newstarts.cn

composer require --dev phpunit/phpunit
来源：http://gc.9csxet.cn

[U79] PHP：静态分析
来源：http://df.shtwfgs.cn

composer require --dev phpstan/phpstan
来源：http://jg.lnxyls.cn

[U80] PHP：代码规范修复
来源：http://bv.521024.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ae.newstarts.cn

[U81] JS：初始化项目
来源：http://ce.colortex.cn

npm init -y;  npm i express
来源：http://oo.bjjhwx.cn

[U82] JS：package.json 脚本
来源：http://jh.bookmarksfly.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wv.yuexingan06.cn

[U83] JS：ES Module 导入导出
来源：http://nd.szxytkj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://om.szsharing.cn

[U84] JS：CommonJS 写法
来源：http://vo.521024.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ny.haigaiapp.cn

[U85] JS：可选链
来源：http://ll.jctech888.com.cn

a?.b?.c
来源：http://qe.asd995.cn

[U86] JS：空值合并
来源：http://ei.huanxung.cn

a ?? b
来源：http://aw.colortex.cn


<!-- 参考信息 -->