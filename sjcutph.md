代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xo.colortex.cn

================================================================================
来源：http://sb.wgjwhj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ey.panjiajie.cn

================================================================================
来源：http://wp.gzmigu.cn

[T01] Kotlin：Hello World
来源：http://kf.bjjhwx.cn

println("Hello")
来源：http://jp.chemitech.net.cn

[T02] Kotlin：变量
来源：http://lo.bjjhwx.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nf.gzmigu.cn

[T03] Kotlin：字符串模板
来源：http://jv.yuexingan06.cn

"值: $b"
来源：http://dk.panjiajie.cn

[T04] Kotlin：空安全
来源：http://hz.hnjuh.cn

val n: String? = null;  n?.length
来源：http://mi.jianghongdianzi.cn

[T05] Kotlin：when 表达式
来源：http://pg.jctech888.com.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sd.9csxet.cn

[T06] Kotlin：集合映射
来源：http://ex.jctech888.com.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ur.asd995.cn

[T07] Kotlin：集合过滤
来源：http://gh.521024.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://kg.szxytkj.cn

[T08] Kotlin：数据类
来源：http://vz.szxytkj.cn

data class User(val name: String, val age: Int)
来源：http://eu.shxzukj.cn

[T09] Kotlin：扩展函数
来源：http://sc.shtwfgs.cn

fun String.exclaim() = this + "!"
来源：http://xd.shxzskj.cn

[T10] Kotlin：默认参数
来源：http://nl.nszjky.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gd.bookmarksfly.cn

[T11] Kotlin：协程
来源：http://bt.newstarts.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bk.haigaiapp.cn

[T12] Kotlin：解构声明
来源：http://hd.lnxyls.cn

val (a, b) = Pair(1, 2)
来源：http://ai.yuexingan06.cn

[T13] Kotlin：只读 Map
来源：http://lt.szxytkj.cn

val m = mapOf("a" to 1)
来源：http://uq.gzmigu.cn

[T14] Kotlin：循环
来源：http://wj.jianghongdianzi.cn

for (i in 1..10) println(i)
来源：http://gx.colortex.cn

[T15] Kotlin：接口
来源：http://hn.asd995.cn

interface Shape { fun area(): Double }
来源：http://vh.huixinmuqiang.cn

[T16] Swift：Hello World
来源：http://gu.haigaiapp.cn

print("Hello")
来源：http://hu.yuntaijiaju.cn

[T17] Swift：变量与常量
来源：http://st.muxihuayi.cn

var a = 1;  let b = 2
来源：http://tj.521024.cn

[T18] Swift：字符串插值
来源：http://vp.szsharing.cn

"值: \(b)"
来源：http://hq.yuexingan06.cn

[T19] Swift：可选绑定
来源：http://od.bookmarksfly.cn

if let n = opt { print(n) }
来源：http://ae.szxytkj.cn

[T20] Swift：数组操作
来源：http://vi.huanxung.cn

var a = [1, 2, 3];  a.append(4)
来源：http://dr.lnxyls.cn

[T21] Swift：遍历
来源：http://rx.bjjhwx.cn

for x in a { print(x) }
来源：http://hk.huanxung.cn

[T22] Swift：字典
来源：http://iq.huixiangedu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://pw.shxzukj.cn

[T23] Swift：函数
来源：http://ki.szsharing.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hu.colortex.cn

[T24] Swift：闭包
来源：http://wk.521024.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vc.hahajie.cn

[T25] Swift：结构体
来源：http://am.shxzukj.cn

struct P { var x: Int }
来源：http://dm.hnjuh.cn

[T26] Swift：类与重写
来源：http://mj.nicolike.cn

class A: Base { override func f() {} }
来源：http://tl.colortex.cn

[T27] Swift：错误处理
来源：http://qy.bjjhwx.cn

do { try f() } catch { print(error) }
来源：http://zx.huanxung.cn

[T28] Swift：枚举
来源：http://yn.newstarts.cn

enum Color { case red, green }
来源：http://nm.gzmigu.cn

[T29] Swift：guard 提前返回
来源：http://ui.gzmigu.cn

guard let x = opt else { return }
来源：http://mn.haigaiapp.cn

[T30] Swift：协议
来源：http://mw.9csxet.cn

protocol Shape { func area() -> Double }
来源：http://vh.lnxyls.cn

[T31] Lua：Hello World
来源：http://lb.lnxyls.cn

print("Hello")
来源：http://hd.newstarts.cn

[T32] Lua：局部变量
来源：http://px.colortex.cn

local a = 1
来源：http://sq.newstarts.cn

[T33] Lua：表（数组）
来源：http://xk.panjiajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://gm.hahajie.cn

[T34] Lua：遍历表
来源：http://ao.shtwfgs.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://pt.shxzukj.cn

[T35] Lua：字典表
来源：http://qe.hahajie.cn

local d = { a = 1 };  d.b = 2
来源：http://go.bjjhwx.cn

[T36] Lua：函数
来源：http://rv.muxihuayi.cn

function add(a, b) return a + b end
来源：http://wt.asd995.cn

[T37] Lua：字符串拼接
来源：http://yw.bjjhwx.cn

"a" .. "b"
来源：http://hx.colortex.cn

[T38] Lua：条件
来源：http://uw.lnxyls.cn

if x > 0 then print("正") end
来源：http://yn.hahajie.cn

[T39] Lua：模式匹配
来源：http://jd.shxzskj.cn

string.find(s, "%d+")
来源：http://ys.panjiajie.cn

[T40] Lua：元表
来源：http://ub.szsharing.cn

setmetatable({}, { __index = base })
来源：http://vd.lnxyls.cn

[T41] Perl：Hello World
来源：http://wd.jctech888.com.cn

print "Hello\n";
来源：http://rs.yuexingan06.cn

[T42] Perl：变量类型
来源：http://bs.lnxyls.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dd.muxihuayi.cn

[T43] Perl：字符串插值
来源：http://te.asd995.cn

"值: $a"
来源：http://hb.chemitech.net.cn

[T44] Perl：条件
来源：http://aw.bjjhwx.cn

if ($a > 0) { print "正"; }
来源：http://na.yuntaijiaju.cn

[T45] Perl：数组遍历
来源：http://gx.huanxung.cn

for my $x (@arr) { print $x; }
来源：http://ev.szsharing.cn

[T46] Perl：哈希操作
来源：http://of.hnjuh.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jk.muxihuayi.cn

[T47] Perl：正则捕获
来源：http://fu.szsharing.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://tm.huixiangedu.cn

[T48] Perl：正则替换
来源：http://xv.shtwfgs.cn

$s =~ s/old/new/g;
来源：http://bz.asd995.cn

[T49] Perl：函数
来源：http://bm.jctech888.com.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nu.huanxung.cn

[T50] Perl：逐行读文件
来源：http://pg.jianghongdianzi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ka.huixiangedu.cn

while (my $line = <$fh>) { print $line; }
来源：http://ja.9csxet.cn

[T51] Scala：Hello World
来源：http://ne.muxihuayi.cn

println("Hello")
来源：http://qv.bookmarksfly.cn

[T52] Scala：变量
来源：http://ns.asd995.cn

val a = 1;  var b = 2
来源：http://af.lnxyls.cn

[T53] Scala：字符串插值
来源：http://xg.bookmarksfly.cn

s"值: $b"
来源：http://kr.asd995.cn

[T54] Scala：集合映射
来源：http://yk.yuexingan06.cn

List(1, 2, 3).map(_ * 2)
来源：http://ug.shtwfgs.cn

[T55] Scala：集合过滤
来源：http://pu.hnjuh.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fx.shxzskj.cn

[T56] Scala：样例类
来源：http://ra.9csxet.cn

case class User(name: String, age: Int)
来源：http://kr.shtwfgs.cn

[T57] Scala：模式匹配
来源：http://al.jianghongdianzi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ui.panjiajie.cn

[T58] Scala：函数定义
来源：http://ov.szxytkj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fs.jctech888.com.cn

[T59] Scala：循环
来源：http://pt.bjjhwx.cn

for (i <- 1 to 10) println(i)
来源：http://xc.muxihuayi.cn

[T60] Scala：折叠
来源：http://rq.9csxet.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fv.gzmigu.cn

================================================================================
来源：http://zw.shtwfgs.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ds.nszjky.cn

================================================================================
来源：http://nq.asd995.cn

[U01] Py：创建虚拟环境
来源：http://of.huixiangedu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://xk.chemitech.net.cn

[U02] Py：导出 / 安装依赖
来源：http://qm.muxihuayi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wo.lnxyls.cn

[U03] Py：加载 .env 配置
来源：http://qz.huixinmuqiang.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ez.hahajie.cn

[U04] Py：变量调试打印
来源：http://id.asd995.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jf.nszjky.cn

[U05] Py：列表去重且保序
来源：http://rr.panjiajie.cn

list(dict.fromkeys(arr))
来源：http://dl.nicolike.cn

[U06] Py：合并两个字典
来源：http://mm.haigaiapp.cn

{**a, **b}
来源：http://dx.bookmarksfly.cn

[U07] Py：反转字典键值
来源：http://pi.hahajie.cn

{v: k for k, v in d.items()}
来源：http://ri.bookmarksfly.cn

[U08] Py：展平二维列表
来源：http://zm.9csxet.cn

[y for x in nested for y in x]
来源：http://ab.panjiajie.cn

[U09] Py：字典取最大值的键
来源：http://oz.panjiajie.cn

max(d, key=d.get)
来源：http://ms.panjiajie.cn

[U10] Py：按值排序字典
来源：http://oa.huanxung.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://io.hahajie.cn

[U11] Py：生成器表达式
来源：http://uz.szxytkj.cn

(x * 2 for x in arr)
来源：http://op.9csxet.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lr.hahajie.cn

Counter(arr).most_common(3)
来源：http://cu.huanxung.cn

[U13] Py：固定长度队列
来源：http://no.huixiangedu.cn

deque(maxlen=10)
来源：http://sp.haigaiapp.cn

[U14] Py：分组收集到列表
来源：http://oc.newstarts.cn

defaultdict(list)
来源：http://yv.chemitech.net.cn

[U15] Py：高精度计时
来源：http://ai.colortex.cn

t = time.perf_counter()
来源：http://ni.huixinmuqiang.cn

[U16] Py：命令行参数解析
来源：http://wt.huixinmuqiang.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jb.gzmigu.cn

[U17] Py：初始化日志
来源：http://ux.colortex.cn

logging.basicConfig(level=logging.INFO)
来源：http://qe.haigaiapp.cn

[U18] Py：预编译正则
来源：http://uq.nicolike.cn

pat = re.compile(r"\d+")
来源：http://bv.huixiangedu.cn

[U19] Py：正则替换带回调
来源：http://oq.bookmarksfly.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://on.chemitech.net.cn

[U20] Py：缓存函数结果
来源：http://yz.szxytkj.cn

@functools.lru_cache(maxsize=None)
来源：http://gc.yuexingan06.cn

[U21] Py：自定义上下文管理器
来源：http://td.jctech888.com.cn

@contextlib.contextmanager
来源：http://wy.colortex.cn

[U22] Py：矩阵转置
来源：http://rj.lnxyls.cn

list(zip(*m))
来源：http://yi.szxytkj.cn

[U23] Py：分块读取大文件
来源：http://oq.9csxet.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xv.yuexingan06.cn

[U24] Py：路径操作
来源：http://hq.lnxyls.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ro.yuntaijiaju.cn

[U25] Py：CSV 按字典读
来源：http://ob.9csxet.cn

csv.DictReader(f)
来源：http://hx.newstarts.cn

[U26] Py：并发下载
来源：http://rm.521024.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tr.shtwfgs.cn

[U27] Py：异步 HTTP
来源：http://qd.chemitech.net.cn

aiohttp.ClientSession() 配合 async with
来源：http://ub.bookmarksfly.cn

[U28] Py：类型别名
来源：http://hn.huixiangedu.cn

UserId = int
来源：http://wl.szxytkj.cn

[U29] Py：属性校验
来源：http://fd.9csxet.cn

@property 与 @x.setter 配合
来源：http://zf.panjiajie.cn

[U30] Py：数据类
来源：http://bd.szxytkj.cn

@dataclass(slots=True)
来源：http://vo.521024.cn

[U31] Py：单测
来源：http://nf.asd995.cn

python -m pytest -q
来源：http://zt.huixiangedu.cn

[U32] Py：代码格式化
来源：http://ds.yuntaijiaju.cn

ruff format . && ruff check --fix .
来源：http://lj.shxzskj.cn

[U33] Py：打包发布
来源：http://dx.yuntaijiaju.cn

python -m build  （依赖 pyproject.toml）
来源：http://wb.lnxyls.cn

[U34] Py：判断编码
来源：http://pv.panjiajie.cn

chardet.detect(raw)
来源：http://to.jianghongdianzi.cn

[U35] Py：发送邮件
来源：http://ay.shxzskj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ym.szsharing.cn

[U36] Py：定时任务
来源：http://wb.wgjwhj.cn

schedule.every(10).minutes.do(job)
来源：http://xf.chemitech.net.cn

[U37] Py：读写 Excel
来源：http://an.nszjky.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ss.huixinmuqiang.cn

[U38] Py：获取脚本所在目录
来源：http://fu.hnjuh.cn

Path(__file__).resolve().parent
来源：http://fo.szsharing.cn

[U39] Py：判断是否在交互环境
来源：http://cu.bookmarksfly.cn

sys.stdout.isatty()
来源：http://fg.wgjwhj.cn

[U40] Py：打印到标准错误
来源：http://ph.asd995.cn

print("err", file=sys.stderr)
来源：http://yf.colortex.cn

[U41] PHP：初始化 Composer 项目
来源：http://pj.nszjky.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qz.bjjhwx.cn

[U42] PHP：PSR-4 自动加载
来源：http://hj.521024.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ck.nicolike.cn

[U43] PHP：声明命名空间
来源：http://vc.nszjky.cn

namespace App\Http;
来源：http://zk.jianghongdianzi.cn

[U44] PHP：开启严格类型
来源：http://op.shxzukj.cn

declare(strict_types=1);
来源：http://ut.huixiangedu.cn

[U45] PHP：类型声明与返回类型
来源：http://vs.huanxung.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ln.huixiangedu.cn

[U46] PHP：可空类型
来源：http://zr.bookmarksfly.cn

?string $name = null
来源：http://sh.szsharing.cn

[U47] PHP：联合类型
来源：http://st.szxytkj.cn

int|string $id
来源：http://zn.huanxung.cn

[U48] PHP：纯枚举
来源：http://qd.9csxet.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ss.colortex.cn

[U49] PHP：只读属性
来源：http://up.muxihuayi.cn

public readonly string $name
来源：http://yu.szsharing.cn

[U50] PHP：构造器属性提升
来源：http://te.jctech888.com.cn

public function __construct(private int $id) {}
来源：http://af.nszjky.cn

[U51] PHP：数组解构
来源：http://ua.huixinmuqiang.cn

[$a, $b] = $arr;
来源：http://qk.shxzskj.cn

[U52] PHP：箭头函数
来源：http://ig.gzmigu.cn

$double = fn($x) => $x * 2;
来源：http://be.jianghongdianzi.cn

[U53] PHP：空合并运算符
来源：http://lr.huixinmuqiang.cn

$v = $a ?? $b ?? "default";
来源：http://ly.yuexingan06.cn

[U54] PHP：空安全调用
来源：http://fw.gzmigu.cn

$obj?->method()
来源：http://ll.shxzskj.cn

[U55] PHP：match 表达式
来源：http://be.jctech888.com.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://sv.521024.cn

[U56] PHP：命名参数
来源：http://xl.huixiangedu.cn

f(a: 1, b: 2)
来源：http://vn.szsharing.cn

[U57] PHP：字符串插值
来源：http://qy.gzmigu.cn

"值: {$a}"
来源：http://oj.521024.cn

[U58] PHP：数组三件套
来源：http://yu.shxzskj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nq.muxihuayi.cn

[U59] PHP：自定义排序
来源：http://ga.panjiajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ok.huixiangedu.cn

[U60] PHP：JSON 编解码
来源：http://gm.shxzskj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xp.asd995.cn

[U61] PHP：正则
来源：http://nu.newstarts.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://us.shxzukj.cn

[U62] PHP：日期对象
来源：http://no.szsharing.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ce.szxytkj.cn

[U63] PHP：文件读写
来源：http://yp.szxytkj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ko.nicolike.cn

[U64] PHP：目录遍历
来源：http://xa.jctech888.com.cn

glob("dir/*.php");  scandir("dir");
来源：http://pk.hnjuh.cn

[U65] PHP：会话
来源：http://lo.asd995.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://uw.gzmigu.cn

[U66] PHP：设置 Cookie
来源：http://pm.wgjwhj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ly.huanxung.cn

[U67] PHP：处理文件上传
来源：http://lw.wgjwhj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tu.haigaiapp.cn

[U68] PHP：PDO 连接
来源：http://ar.panjiajie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mq.huixiangedu.cn

[U69] PHP：PDO 预处理
来源：http://tw.yuntaijiaju.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ud.lnxyls.cn

[U70] PHP：PDO 事务
来源：http://jh.huixinmuqiang.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lg.haigaiapp.cn

[U71] PHP：抛出异常
来源：http://og.colortex.cn

throw new RuntimeException("失败", 500);
来源：http://sz.yuexingan06.cn

[U72] PHP：写错误日志
来源：http://uk.nszjky.cn

error_log("失败: " . $e->getMessage());
来源：http://ii.yuntaijiaju.cn

[U73] PHP：读取 ini 配置
来源：http://ra.521024.cn

parse_ini_file("config.ini", true)
来源：http://it.shxzskj.cn

[U74] PHP：读取环境变量
来源：http://zq.yuntaijiaju.cn

getenv("APP_ENV") ?: "production"
来源：http://wu.shxzukj.cn

[U75] PHP：依赖注入
来源：http://jb.asd995.cn

composer require psr/container
来源：http://fo.newstarts.cn

[U76] PHP：简单路由
来源：http://qm.muxihuayi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yy.shtwfgs.cn

[U77] PHP：模板渲染
来源：http://fc.9csxet.cn

composer require twig/twig
来源：http://lq.bookmarksfly.cn

[U78] PHP：单元测试
来源：http://bi.wgjwhj.cn

composer require --dev phpunit/phpunit
来源：http://aq.hnjuh.cn

[U79] PHP：静态分析
来源：http://mm.lnxyls.cn

composer require --dev phpstan/phpstan
来源：http://yv.panjiajie.cn

[U80] PHP：代码规范修复
来源：http://zp.shxzskj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://gj.szsharing.cn

[U81] JS：初始化项目
来源：http://ah.bjjhwx.cn

npm init -y;  npm i express
来源：http://id.bookmarksfly.cn

[U82] JS：package.json 脚本
来源：http://xb.jctech888.com.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ep.huanxung.cn

[U83] JS：ES Module 导入导出
来源：http://pc.wgjwhj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://un.chemitech.net.cn

[U84] JS：CommonJS 写法
来源：http://rz.bjjhwx.cn

module.exports = { a };  const { a } = require("./m");
来源：http://pr.hnjuh.cn

[U85] JS：可选链
来源：http://dm.panjiajie.cn

a?.b?.c
来源：http://iu.yuntaijiaju.cn

[U86] JS：空值合并
来源：http://wu.wgjwhj.cn

a ?? b
来源：http://ek.haigaiapp.cn


<!-- 参考信息 -->