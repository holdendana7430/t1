代发 wailian999

[T01] Kotlin：Hello World
来源：http://gs.huixinmuqiang.cn

println("Hello")
来源：http://zk.bookmarksfly.cn

[T02] Kotlin：变量
来源：http://lv.huixiangedu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dy.yuntaijiaju.cn

[T03] Kotlin：字符串模板
来源：http://pm.nicolike.cn

"值: $b"
来源：http://kg.jctech888.com.cn

[T04] Kotlin：空安全
来源：http://eq.shxzukj.cn

val n: String? = null;  n?.length
来源：http://ri.521024.cn

[T05] Kotlin：when 表达式
来源：http://sf.panjiajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kf.gzmigu.cn

[T06] Kotlin：集合映射
来源：http://ea.nicolike.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://us.lnxyls.cn

[T07] Kotlin：集合过滤
来源：http://mf.bookmarksfly.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://si.huixinmuqiang.cn

[T08] Kotlin：数据类
来源：http://pk.521024.cn

data class User(val name: String, val age: Int)
来源：http://ds.jctech888.com.cn

[T09] Kotlin：扩展函数
来源：http://ee.bjjhwx.cn

fun String.exclaim() = this + "!"
来源：http://ti.bookmarksfly.cn

[T10] Kotlin：默认参数
来源：http://ev.chemitech.net.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://bp.jianghongdianzi.cn

[T11] Kotlin：协程
来源：http://fg.9csxet.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://tm.nszjky.cn

[T12] Kotlin：解构声明
来源：http://di.newstarts.cn

val (a, b) = Pair(1, 2)
来源：http://bv.huixiangedu.cn

[T13] Kotlin：只读 Map
来源：http://mm.wgjwhj.cn

val m = mapOf("a" to 1)
来源：http://yh.chemitech.net.cn

[T14] Kotlin：循环
来源：http://md.bjjhwx.cn

for (i in 1..10) println(i)
来源：http://xj.hnjuh.cn

[T15] Kotlin：接口
来源：http://px.wgjwhj.cn

interface Shape { fun area(): Double }
来源：http://ee.szxytkj.cn

[T16] Swift：Hello World
来源：http://ni.bjjhwx.cn

print("Hello")
来源：http://rq.nszjky.cn

[T17] Swift：变量与常量
来源：http://jb.haigaiapp.cn

var a = 1;  let b = 2
来源：http://eo.asd995.cn

[T18] Swift：字符串插值
来源：http://ss.lnxyls.cn

"值: \(b)"
来源：http://sr.shxzukj.cn

[T19] Swift：可选绑定
来源：http://qn.521024.cn

if let n = opt { print(n) }
来源：http://pv.newstarts.cn

[T20] Swift：数组操作
来源：http://xw.panjiajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fn.huixinmuqiang.cn

[T21] Swift：遍历
来源：http://gy.nicolike.cn

for x in a { print(x) }
来源：http://ut.jianghongdianzi.cn

[T22] Swift：字典
来源：http://sb.bookmarksfly.cn

var d = ["a": 1];  d["b"] = 2
来源：http://sa.jianghongdianzi.cn

[T23] Swift：函数
来源：http://zj.panjiajie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ql.szxytkj.cn

[T24] Swift：闭包
来源：http://kp.chemitech.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://rd.521024.cn

[T25] Swift：结构体
来源：http://rw.huanxung.cn

struct P { var x: Int }
来源：http://jk.newstarts.cn

[T26] Swift：类与重写
来源：http://tp.shxzukj.cn

class A: Base { override func f() {} }
来源：http://hn.9csxet.cn

[T27] Swift：错误处理
来源：http://bp.hahajie.cn

do { try f() } catch { print(error) }
来源：http://fv.haigaiapp.cn

[T28] Swift：枚举
来源：http://xr.hnjuh.cn

enum Color { case red, green }
来源：http://gw.yuexingan06.cn

[T29] Swift：guard 提前返回
来源：http://mo.yuntaijiaju.cn

guard let x = opt else { return }
来源：http://go.hahajie.cn

[T30] Swift：协议
来源：http://nm.szxytkj.cn

protocol Shape { func area() -> Double }
来源：http://xs.szsharing.cn

[T31] Lua：Hello World
来源：http://ik.jianghongdianzi.cn

print("Hello")
来源：http://jd.huanxung.cn

[T32] Lua：局部变量
来源：http://ax.szsharing.cn

local a = 1
来源：http://ph.hahajie.cn

[T33] Lua：表（数组）
来源：http://hb.yuntaijiaju.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ju.lnxyls.cn

[T34] Lua：遍历表
来源：http://cz.wgjwhj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gr.gzmigu.cn

[T35] Lua：字典表
来源：http://os.jctech888.com.cn

local d = { a = 1 };  d.b = 2
来源：http://eg.9csxet.cn

[T36] Lua：函数
来源：http://fx.jctech888.com.cn

function add(a, b) return a + b end
来源：http://qx.huixiangedu.cn

[T37] Lua：字符串拼接
来源：http://kv.yuntaijiaju.cn

"a" .. "b"
来源：http://le.shxzskj.cn

[T38] Lua：条件
来源：http://xb.szsharing.cn

if x > 0 then print("正") end
来源：http://ke.shtwfgs.cn

[T39] Lua：模式匹配
来源：http://ai.lnxyls.cn

string.find(s, "%d+")
来源：http://aw.hahajie.cn

[T40] Lua：元表
来源：http://jb.bjjhwx.cn

setmetatable({}, { __index = base })
来源：http://gz.bjjhwx.cn

[T41] Perl：Hello World
来源：http://hb.shxzskj.cn

print "Hello\n";
来源：http://uw.colortex.cn

[T42] Perl：变量类型
来源：http://fg.chemitech.net.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tq.muxihuayi.cn

[T43] Perl：字符串插值
来源：http://ua.hnjuh.cn

"值: $a"
来源：http://ut.hahajie.cn

[T44] Perl：条件
来源：http://vo.shtwfgs.cn

if ($a > 0) { print "正"; }
来源：http://yl.nicolike.cn

[T45] Perl：数组遍历
来源：http://pk.huixiangedu.cn

for my $x (@arr) { print $x; }
来源：http://jh.nicolike.cn

[T46] Perl：哈希操作
来源：http://rw.jianghongdianzi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://eu.9csxet.cn

[T47] Perl：正则捕获
来源：http://zt.hnjuh.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://tr.jianghongdianzi.cn

[T48] Perl：正则替换
来源：http://ap.szxytkj.cn

$s =~ s/old/new/g;
来源：http://rs.gzmigu.cn

[T49] Perl：函数
来源：http://ke.jctech888.com.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sr.huixinmuqiang.cn

[T50] Perl：逐行读文件
来源：http://gi.haigaiapp.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ii.szsharing.cn

while (my $line = <$fh>) { print $line; }
来源：http://eq.gzmigu.cn

[T51] Scala：Hello World
来源：http://to.9csxet.cn

println("Hello")
来源：http://ck.huixinmuqiang.cn

[T52] Scala：变量
来源：http://fq.asd995.cn

val a = 1;  var b = 2
来源：http://wr.huixinmuqiang.cn

[T53] Scala：字符串插值
来源：http://us.huixinmuqiang.cn

s"值: $b"
来源：http://nv.jctech888.com.cn

[T54] Scala：集合映射
来源：http://wg.panjiajie.cn

List(1, 2, 3).map(_ * 2)
来源：http://ni.huixinmuqiang.cn

[T55] Scala：集合过滤
来源：http://hh.newstarts.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ma.huixiangedu.cn

[T56] Scala：样例类
来源：http://rv.colortex.cn

case class User(name: String, age: Int)
来源：http://lt.yuexingan06.cn

[T57] Scala：模式匹配
来源：http://gw.muxihuayi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://bt.chemitech.net.cn

[T58] Scala：函数定义
来源：http://gc.shxzskj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://qe.huixinmuqiang.cn

[T59] Scala：循环
来源：http://eb.jctech888.com.cn

for (i <- 1 to 10) println(i)
来源：http://gx.jianghongdianzi.cn

[T60] Scala：折叠
来源：http://tv.muxihuayi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bq.gzmigu.cn

================================================================================
来源：http://ap.muxihuayi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cz.hahajie.cn

================================================================================
来源：http://sv.huixiangedu.cn

[U01] Py：创建虚拟环境
来源：http://kb.9csxet.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wl.wgjwhj.cn

[U02] Py：导出 / 安装依赖
来源：http://ug.jianghongdianzi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xm.shxzukj.cn

[U03] Py：加载 .env 配置
来源：http://de.hahajie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://bz.yuntaijiaju.cn

[U04] Py：变量调试打印
来源：http://fu.jctech888.com.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xc.shxzukj.cn

[U05] Py：列表去重且保序
来源：http://cz.gzmigu.cn

list(dict.fromkeys(arr))
来源：http://ru.huixinmuqiang.cn

[U06] Py：合并两个字典
来源：http://hv.jianghongdianzi.cn

{**a, **b}
来源：http://xa.hahajie.cn

[U07] Py：反转字典键值
来源：http://qa.huanxung.cn

{v: k for k, v in d.items()}
来源：http://ag.newstarts.cn

[U08] Py：展平二维列表
来源：http://ia.gzmigu.cn

[y for x in nested for y in x]
来源：http://ok.hahajie.cn

[U09] Py：字典取最大值的键
来源：http://hr.szsharing.cn

max(d, key=d.get)
来源：http://ea.bjjhwx.cn

[U10] Py：按值排序字典
来源：http://em.huanxung.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://li.szsharing.cn

[U11] Py：生成器表达式
来源：http://mz.shtwfgs.cn

(x * 2 for x in arr)
来源：http://uw.haigaiapp.cn

[U12] Py：取出现最多的 3 个元素
来源：http://wb.panjiajie.cn

Counter(arr).most_common(3)
来源：http://ir.asd995.cn

[U13] Py：固定长度队列
来源：http://ok.chemitech.net.cn

deque(maxlen=10)
来源：http://aq.521024.cn

[U14] Py：分组收集到列表
来源：http://nl.szsharing.cn

defaultdict(list)
来源：http://au.jianghongdianzi.cn

[U15] Py：高精度计时
来源：http://nl.jianghongdianzi.cn

t = time.perf_counter()
来源：http://uv.wgjwhj.cn

[U16] Py：命令行参数解析
来源：http://ks.huixinmuqiang.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nb.asd995.cn

[U17] Py：初始化日志
来源：http://gl.panjiajie.cn

logging.basicConfig(level=logging.INFO)
来源：http://wz.nicolike.cn

[U18] Py：预编译正则
来源：http://zy.asd995.cn

pat = re.compile(r"\d+")
来源：http://gt.hahajie.cn

[U19] Py：正则替换带回调
来源：http://wt.szxytkj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cd.newstarts.cn

[U20] Py：缓存函数结果
来源：http://gf.huixinmuqiang.cn

@functools.lru_cache(maxsize=None)
来源：http://mf.panjiajie.cn

[U21] Py：自定义上下文管理器
来源：http://sb.shxzskj.cn

@contextlib.contextmanager
来源：http://mb.hahajie.cn

[U22] Py：矩阵转置
来源：http://kt.hnjuh.cn

list(zip(*m))
来源：http://bp.nicolike.cn

[U23] Py：分块读取大文件
来源：http://ju.9csxet.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fd.szxytkj.cn

[U24] Py：路径操作
来源：http://sl.nicolike.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zs.szxytkj.cn

[U25] Py：CSV 按字典读
来源：http://ny.nicolike.cn

csv.DictReader(f)
来源：http://se.yuexingan06.cn

[U26] Py：并发下载
来源：http://tp.panjiajie.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wa.521024.cn

[U27] Py：异步 HTTP
来源：http://kg.huixinmuqiang.cn

aiohttp.ClientSession() 配合 async with
来源：http://tc.nicolike.cn

[U28] Py：类型别名
来源：http://nm.bookmarksfly.cn

UserId = int
来源：http://ro.bookmarksfly.cn

[U29] Py：属性校验
来源：http://bq.muxihuayi.cn

@property 与 @x.setter 配合
来源：http://my.colortex.cn

[U30] Py：数据类
来源：http://uk.bookmarksfly.cn

@dataclass(slots=True)
来源：http://pg.szsharing.cn

[U31] Py：单测
来源：http://cm.shxzukj.cn

python -m pytest -q
来源：http://km.shxzskj.cn

[U32] Py：代码格式化
来源：http://gf.chemitech.net.cn

ruff format . && ruff check --fix .
来源：http://ss.jianghongdianzi.cn

[U33] Py：打包发布
来源：http://la.bookmarksfly.cn

python -m build  （依赖 pyproject.toml）
来源：http://vi.hnjuh.cn

[U34] Py：判断编码
来源：http://hr.newstarts.cn

chardet.detect(raw)
来源：http://bt.panjiajie.cn

[U35] Py：发送邮件
来源：http://uv.shtwfgs.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ra.shtwfgs.cn

[U36] Py：定时任务
来源：http://gm.9csxet.cn

schedule.every(10).minutes.do(job)
来源：http://qd.wgjwhj.cn

[U37] Py：读写 Excel
来源：http://zr.wgjwhj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://pg.panjiajie.cn

[U38] Py：获取脚本所在目录
来源：http://pv.szxytkj.cn

Path(__file__).resolve().parent
来源：http://cg.hahajie.cn

[U39] Py：判断是否在交互环境
来源：http://xa.521024.cn

sys.stdout.isatty()
来源：http://vq.shxzukj.cn

[U40] Py：打印到标准错误
来源：http://yc.huixinmuqiang.cn

print("err", file=sys.stderr)
来源：http://yz.muxihuayi.cn

[U41] PHP：初始化 Composer 项目
来源：http://ir.asd995.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://cg.huanxung.cn

[U42] PHP：PSR-4 自动加载
来源：http://av.521024.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://on.yuntaijiaju.cn

[U43] PHP：声明命名空间
来源：http://pw.shtwfgs.cn

namespace App\Http;
来源：http://uu.shxzskj.cn

[U44] PHP：开启严格类型
来源：http://uw.521024.cn

declare(strict_types=1);
来源：http://ff.521024.cn

[U45] PHP：类型声明与返回类型
来源：http://cq.muxihuayi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://xp.lnxyls.cn

[U46] PHP：可空类型
来源：http://mk.newstarts.cn

?string $name = null
来源：http://xf.lnxyls.cn

[U47] PHP：联合类型
来源：http://nr.shxzskj.cn

int|string $id
来源：http://tx.lnxyls.cn

[U48] PHP：纯枚举
来源：http://xe.bookmarksfly.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ls.yuntaijiaju.cn

[U49] PHP：只读属性
来源：http://ib.9csxet.cn

public readonly string $name
来源：http://nb.jctech888.com.cn

[U50] PHP：构造器属性提升
来源：http://gw.yuexingan06.cn

public function __construct(private int $id) {}
来源：http://qr.lnxyls.cn

[U51] PHP：数组解构
来源：http://gc.muxihuayi.cn

[$a, $b] = $arr;
来源：http://ok.nszjky.cn

[U52] PHP：箭头函数
来源：http://qn.panjiajie.cn

$double = fn($x) => $x * 2;
来源：http://qt.haigaiapp.cn

[U53] PHP：空合并运算符
来源：http://hv.haigaiapp.cn

$v = $a ?? $b ?? "default";
来源：http://ft.bjjhwx.cn

[U54] PHP：空安全调用
来源：http://jb.asd995.cn

$obj?->method()
来源：http://hv.bjjhwx.cn

[U55] PHP：match 表达式
来源：http://cb.colortex.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ak.nicolike.cn

[U56] PHP：命名参数
来源：http://tz.haigaiapp.cn

f(a: 1, b: 2)
来源：http://wi.shxzskj.cn

[U57] PHP：字符串插值
来源：http://ef.asd995.cn

"值: {$a}"
来源：http://zd.asd995.cn

[U58] PHP：数组三件套
来源：http://st.haigaiapp.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ws.bjjhwx.cn

[U59] PHP：自定义排序
来源：http://yw.asd995.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ox.huixiangedu.cn

[U60] PHP：JSON 编解码
来源：http://cv.hnjuh.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://za.szxytkj.cn

[U61] PHP：正则
来源：http://dg.haigaiapp.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://us.chemitech.net.cn

[U62] PHP：日期对象
来源：http://sc.chemitech.net.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ae.muxihuayi.cn

[U63] PHP：文件读写
来源：http://ub.hnjuh.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://td.bookmarksfly.cn

[U64] PHP：目录遍历
来源：http://gu.asd995.cn

glob("dir/*.php");  scandir("dir");
来源：http://wq.shxzskj.cn

[U65] PHP：会话
来源：http://cz.hahajie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://hw.bjjhwx.cn

[U66] PHP：设置 Cookie
来源：http://aw.hahajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lf.shxzukj.cn

[U67] PHP：处理文件上传
来源：http://dj.shxzskj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pd.yuntaijiaju.cn

[U68] PHP：PDO 连接
来源：http://jh.chemitech.net.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://el.szxytkj.cn

[U69] PHP：PDO 预处理
来源：http://tt.lnxyls.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fn.panjiajie.cn

[U70] PHP：PDO 事务
来源：http://yk.hnjuh.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gq.shxzskj.cn

[U71] PHP：抛出异常
来源：http://lo.haigaiapp.cn

throw new RuntimeException("失败", 500);
来源：http://yd.szxytkj.cn

[U72] PHP：写错误日志
来源：http://xq.shtwfgs.cn

error_log("失败: " . $e->getMessage());
来源：http://bx.521024.cn

[U73] PHP：读取 ini 配置
来源：http://ca.wgjwhj.cn

parse_ini_file("config.ini", true)
来源：http://ob.hahajie.cn

[U74] PHP：读取环境变量
来源：http://ju.hnjuh.cn

getenv("APP_ENV") ?: "production"
来源：http://ga.shtwfgs.cn

[U75] PHP：依赖注入
来源：http://su.shtwfgs.cn

composer require psr/container
来源：http://zm.bookmarksfly.cn

[U76] PHP：简单路由
来源：http://nt.huixiangedu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hj.panjiajie.cn

[U77] PHP：模板渲染
来源：http://td.bjjhwx.cn

composer require twig/twig
来源：http://wl.huixiangedu.cn

[U78] PHP：单元测试
来源：http://in.panjiajie.cn

composer require --dev phpunit/phpunit
来源：http://hs.yuntaijiaju.cn

[U79] PHP：静态分析
来源：http://qa.9csxet.cn

composer require --dev phpstan/phpstan
来源：http://un.shxzskj.cn

[U80] PHP：代码规范修复
来源：http://qb.nicolike.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://mk.gzmigu.cn

[U81] JS：初始化项目
来源：http://ij.huixiangedu.cn

npm init -y;  npm i express
来源：http://bo.yuexingan06.cn

[U82] JS：package.json 脚本
来源：http://fs.muxihuayi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://af.hnjuh.cn

[U83] JS：ES Module 导入导出
来源：http://rg.haigaiapp.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qj.jianghongdianzi.cn

[U84] JS：CommonJS 写法
来源：http://yh.chemitech.net.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ov.nicolike.cn

[U85] JS：可选链
来源：http://mg.bookmarksfly.cn

a?.b?.c
来源：http://lx.shxzukj.cn

[U86] JS：空值合并
来源：http://bk.shtwfgs.cn

a ?? b
来源：http://em.nszjky.cn

[U87] JS：解构默认值
来源：http://kd.jctech888.com.cn

const { a = 1, b = 2 } = obj;
来源：http://wt.nszjky.cn

[U88] JS：对象展开合并
来源：http://oc.shxzukj.cn

{ ...a, ...b }
来源：http://ye.hnjuh.cn


<!-- 参考信息 -->