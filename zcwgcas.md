代发 wailian999

[T01] Kotlin：Hello World
来源：http://nf.shxzukj.cn

println("Hello")
来源：http://yl.haigaiapp.cn

[T02] Kotlin：变量
来源：http://yc.panjiajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://za.jianghongdianzi.cn

[T03] Kotlin：字符串模板
来源：http://nf.chemitech.net.cn

"值: $b"
来源：http://ex.jctech888.com.cn

[T04] Kotlin：空安全
来源：http://hv.szsharing.cn

val n: String? = null;  n?.length
来源：http://pg.huanxung.cn

[T05] Kotlin：when 表达式
来源：http://dy.yuntaijiaju.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ko.9csxet.cn

[T06] Kotlin：集合映射
来源：http://jp.muxihuayi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ic.521024.cn

[T07] Kotlin：集合过滤
来源：http://cd.521024.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://dy.hahajie.cn

[T08] Kotlin：数据类
来源：http://uv.9csxet.cn

data class User(val name: String, val age: Int)
来源：http://rp.nicolike.cn

[T09] Kotlin：扩展函数
来源：http://rr.hnjuh.cn

fun String.exclaim() = this + "!"
来源：http://qg.nszjky.cn

[T10] Kotlin：默认参数
来源：http://wm.shtwfgs.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wo.huanxung.cn

[T11] Kotlin：协程
来源：http://ew.shxzskj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ob.newstarts.cn

[T12] Kotlin：解构声明
来源：http://gv.9csxet.cn

val (a, b) = Pair(1, 2)
来源：http://gm.9csxet.cn

[T13] Kotlin：只读 Map
来源：http://lo.wgjwhj.cn

val m = mapOf("a" to 1)
来源：http://kq.gzmigu.cn

[T14] Kotlin：循环
来源：http://su.gzmigu.cn

for (i in 1..10) println(i)
来源：http://jb.chemitech.net.cn

[T15] Kotlin：接口
来源：http://zs.lnxyls.cn

interface Shape { fun area(): Double }
来源：http://id.bjjhwx.cn

[T16] Swift：Hello World
来源：http://dh.shxzskj.cn

print("Hello")
来源：http://id.hnjuh.cn

[T17] Swift：变量与常量
来源：http://iw.gzmigu.cn

var a = 1;  let b = 2
来源：http://cb.shxzskj.cn

[T18] Swift：字符串插值
来源：http://ja.muxihuayi.cn

"值: \(b)"
来源：http://kt.bookmarksfly.cn

[T19] Swift：可选绑定
来源：http://kt.shxzskj.cn

if let n = opt { print(n) }
来源：http://yy.shxzukj.cn

[T20] Swift：数组操作
来源：http://ev.lnxyls.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qu.yuntaijiaju.cn

[T21] Swift：遍历
来源：http://hw.haigaiapp.cn

for x in a { print(x) }
来源：http://zt.bookmarksfly.cn

[T22] Swift：字典
来源：http://ty.shtwfgs.cn

var d = ["a": 1];  d["b"] = 2
来源：http://yl.huixiangedu.cn

[T23] Swift：函数
来源：http://mo.szxytkj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zt.hnjuh.cn

[T24] Swift：闭包
来源：http://it.hnjuh.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://np.nicolike.cn

[T25] Swift：结构体
来源：http://hr.yuntaijiaju.cn

struct P { var x: Int }
来源：http://rv.asd995.cn

[T26] Swift：类与重写
来源：http://ap.yuntaijiaju.cn

class A: Base { override func f() {} }
来源：http://hf.bjjhwx.cn

[T27] Swift：错误处理
来源：http://aa.9csxet.cn

do { try f() } catch { print(error) }
来源：http://im.hahajie.cn

[T28] Swift：枚举
来源：http://vf.hahajie.cn

enum Color { case red, green }
来源：http://xm.bjjhwx.cn

[T29] Swift：guard 提前返回
来源：http://so.jianghongdianzi.cn

guard let x = opt else { return }
来源：http://ov.huixiangedu.cn

[T30] Swift：协议
来源：http://nf.muxihuayi.cn

protocol Shape { func area() -> Double }
来源：http://vp.huixinmuqiang.cn

[T31] Lua：Hello World
来源：http://vx.shxzukj.cn

print("Hello")
来源：http://sb.yuntaijiaju.cn

[T32] Lua：局部变量
来源：http://yw.gzmigu.cn

local a = 1
来源：http://nf.huixiangedu.cn

[T33] Lua：表（数组）
来源：http://rl.nicolike.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ki.hnjuh.cn

[T34] Lua：遍历表
来源：http://id.newstarts.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://yj.wgjwhj.cn

[T35] Lua：字典表
来源：http://kv.muxihuayi.cn

local d = { a = 1 };  d.b = 2
来源：http://ia.yuntaijiaju.cn

[T36] Lua：函数
来源：http://fg.huanxung.cn

function add(a, b) return a + b end
来源：http://nd.panjiajie.cn

[T37] Lua：字符串拼接
来源：http://gm.yuntaijiaju.cn

"a" .. "b"
来源：http://ve.yuntaijiaju.cn

[T38] Lua：条件
来源：http://zm.muxihuayi.cn

if x > 0 then print("正") end
来源：http://fu.hnjuh.cn

[T39] Lua：模式匹配
来源：http://hs.wgjwhj.cn

string.find(s, "%d+")
来源：http://qf.panjiajie.cn

[T40] Lua：元表
来源：http://rq.asd995.cn

setmetatable({}, { __index = base })
来源：http://ff.nicolike.cn

[T41] Perl：Hello World
来源：http://wg.chemitech.net.cn

print "Hello\n";
来源：http://hq.lnxyls.cn

[T42] Perl：变量类型
来源：http://xg.newstarts.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hi.hnjuh.cn

[T43] Perl：字符串插值
来源：http://gx.gzmigu.cn

"值: $a"
来源：http://ps.szxytkj.cn

[T44] Perl：条件
来源：http://wq.shtwfgs.cn

if ($a > 0) { print "正"; }
来源：http://md.wgjwhj.cn

[T45] Perl：数组遍历
来源：http://yq.wgjwhj.cn

for my $x (@arr) { print $x; }
来源：http://wn.colortex.cn

[T46] Perl：哈希操作
来源：http://vo.asd995.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hj.newstarts.cn

[T47] Perl：正则捕获
来源：http://pc.lnxyls.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xj.newstarts.cn

[T48] Perl：正则替换
来源：http://rw.muxihuayi.cn

$s =~ s/old/new/g;
来源：http://gk.yuntaijiaju.cn

[T49] Perl：函数
来源：http://qi.szxytkj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ms.szsharing.cn

[T50] Perl：逐行读文件
来源：http://ow.shxzukj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://tx.haigaiapp.cn

while (my $line = <$fh>) { print $line; }
来源：http://tn.shxzskj.cn

[T51] Scala：Hello World
来源：http://em.nicolike.cn

println("Hello")
来源：http://ri.chemitech.net.cn

[T52] Scala：变量
来源：http://rf.huixinmuqiang.cn

val a = 1;  var b = 2
来源：http://re.newstarts.cn

[T53] Scala：字符串插值
来源：http://st.hahajie.cn

s"值: $b"
来源：http://bf.szxytkj.cn

[T54] Scala：集合映射
来源：http://nk.szsharing.cn

List(1, 2, 3).map(_ * 2)
来源：http://ty.nicolike.cn

[T55] Scala：集合过滤
来源：http://dg.nszjky.cn

List(1, 2, 3).filter(_ > 1)
来源：http://uv.bjjhwx.cn

[T56] Scala：样例类
来源：http://mk.haigaiapp.cn

case class User(name: String, age: Int)
来源：http://yd.szsharing.cn

[T57] Scala：模式匹配
来源：http://nb.shtwfgs.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://dh.gzmigu.cn

[T58] Scala：函数定义
来源：http://tq.haigaiapp.cn

def add(a: Int, b: Int): Int = a + b
来源：http://jv.nszjky.cn

[T59] Scala：循环
来源：http://hn.huixiangedu.cn

for (i <- 1 to 10) println(i)
来源：http://ui.wgjwhj.cn

[T60] Scala：折叠
来源：http://js.jianghongdianzi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hm.yuexingan06.cn

================================================================================
来源：http://kh.huixinmuqiang.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qe.colortex.cn

================================================================================
来源：http://wq.chemitech.net.cn

[U01] Py：创建虚拟环境
来源：http://gi.yuntaijiaju.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mi.jianghongdianzi.cn

[U02] Py：导出 / 安装依赖
来源：http://kh.yuntaijiaju.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://aq.huixinmuqiang.cn

[U03] Py：加载 .env 配置
来源：http://jl.bookmarksfly.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://os.huanxung.cn

[U04] Py：变量调试打印
来源：http://ld.muxihuayi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cu.jianghongdianzi.cn

[U05] Py：列表去重且保序
来源：http://ii.hnjuh.cn

list(dict.fromkeys(arr))
来源：http://hb.huanxung.cn

[U06] Py：合并两个字典
来源：http://kp.huixinmuqiang.cn

{**a, **b}
来源：http://uv.9csxet.cn

[U07] Py：反转字典键值
来源：http://zo.jianghongdianzi.cn

{v: k for k, v in d.items()}
来源：http://jz.huixinmuqiang.cn

[U08] Py：展平二维列表
来源：http://nw.shtwfgs.cn

[y for x in nested for y in x]
来源：http://pk.lnxyls.cn

[U09] Py：字典取最大值的键
来源：http://sx.shtwfgs.cn

max(d, key=d.get)
来源：http://bm.chemitech.net.cn

[U10] Py：按值排序字典
来源：http://mq.wgjwhj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://it.lnxyls.cn

[U11] Py：生成器表达式
来源：http://gd.bjjhwx.cn

(x * 2 for x in arr)
来源：http://dp.huixinmuqiang.cn

[U12] Py：取出现最多的 3 个元素
来源：http://za.lnxyls.cn

Counter(arr).most_common(3)
来源：http://eb.nszjky.cn

[U13] Py：固定长度队列
来源：http://zc.shxzskj.cn

deque(maxlen=10)
来源：http://fu.hahajie.cn

[U14] Py：分组收集到列表
来源：http://ny.shxzukj.cn

defaultdict(list)
来源：http://cg.szsharing.cn

[U15] Py：高精度计时
来源：http://cq.huanxung.cn

t = time.perf_counter()
来源：http://se.9csxet.cn

[U16] Py：命令行参数解析
来源：http://ku.bjjhwx.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://af.shtwfgs.cn

[U17] Py：初始化日志
来源：http://bs.jianghongdianzi.cn

logging.basicConfig(level=logging.INFO)
来源：http://fd.huixinmuqiang.cn

[U18] Py：预编译正则
来源：http://qt.huixiangedu.cn

pat = re.compile(r"\d+")
来源：http://do.jianghongdianzi.cn

[U19] Py：正则替换带回调
来源：http://zs.gzmigu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fq.szsharing.cn

[U20] Py：缓存函数结果
来源：http://mn.bookmarksfly.cn

@functools.lru_cache(maxsize=None)
来源：http://gq.hahajie.cn

[U21] Py：自定义上下文管理器
来源：http://ko.asd995.cn

@contextlib.contextmanager
来源：http://zu.bjjhwx.cn

[U22] Py：矩阵转置
来源：http://ld.hahajie.cn

list(zip(*m))
来源：http://ag.shxzukj.cn

[U23] Py：分块读取大文件
来源：http://pg.nicolike.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vx.hnjuh.cn

[U24] Py：路径操作
来源：http://ps.bookmarksfly.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ij.9csxet.cn

[U25] Py：CSV 按字典读
来源：http://dd.shxzukj.cn

csv.DictReader(f)
来源：http://az.nszjky.cn

[U26] Py：并发下载
来源：http://ot.huixiangedu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tp.panjiajie.cn

[U27] Py：异步 HTTP
来源：http://gv.shxzskj.cn

aiohttp.ClientSession() 配合 async with
来源：http://qt.szsharing.cn

[U28] Py：类型别名
来源：http://xp.colortex.cn

UserId = int
来源：http://qd.jianghongdianzi.cn

[U29] Py：属性校验
来源：http://sm.jianghongdianzi.cn

@property 与 @x.setter 配合
来源：http://te.hahajie.cn

[U30] Py：数据类
来源：http://gn.nicolike.cn

@dataclass(slots=True)
来源：http://ex.hnjuh.cn

[U31] Py：单测
来源：http://ga.szsharing.cn

python -m pytest -q
来源：http://ij.chemitech.net.cn

[U32] Py：代码格式化
来源：http://zu.huanxung.cn

ruff format . && ruff check --fix .
来源：http://sc.yuexingan06.cn

[U33] Py：打包发布
来源：http://cv.szsharing.cn

python -m build  （依赖 pyproject.toml）
来源：http://eu.hahajie.cn

[U34] Py：判断编码
来源：http://bf.szxytkj.cn

chardet.detect(raw)
来源：http://id.szxytkj.cn

[U35] Py：发送邮件
来源：http://rg.huanxung.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vu.shxzskj.cn

[U36] Py：定时任务
来源：http://iz.gzmigu.cn

schedule.every(10).minutes.do(job)
来源：http://wl.jianghongdianzi.cn

[U37] Py：读写 Excel
来源：http://gm.panjiajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://gw.shxzskj.cn

[U38] Py：获取脚本所在目录
来源：http://tt.wgjwhj.cn

Path(__file__).resolve().parent
来源：http://xm.huanxung.cn

[U39] Py：判断是否在交互环境
来源：http://jo.nicolike.cn

sys.stdout.isatty()
来源：http://dk.huixiangedu.cn

[U40] Py：打印到标准错误
来源：http://tu.521024.cn

print("err", file=sys.stderr)
来源：http://cl.shtwfgs.cn

[U41] PHP：初始化 Composer 项目
来源：http://ji.shxzskj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://od.huixiangedu.cn

[U42] PHP：PSR-4 自动加载
来源：http://km.chemitech.net.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hc.521024.cn

[U43] PHP：声明命名空间
来源：http://no.huixinmuqiang.cn

namespace App\Http;
来源：http://fa.huixinmuqiang.cn

[U44] PHP：开启严格类型
来源：http://hu.shxzskj.cn

declare(strict_types=1);
来源：http://qf.huixiangedu.cn

[U45] PHP：类型声明与返回类型
来源：http://js.gzmigu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ni.haigaiapp.cn

[U46] PHP：可空类型
来源：http://km.muxihuayi.cn

?string $name = null
来源：http://ja.jctech888.com.cn

[U47] PHP：联合类型
来源：http://vc.jctech888.com.cn

int|string $id
来源：http://gk.colortex.cn

[U48] PHP：纯枚举
来源：http://po.bookmarksfly.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://to.lnxyls.cn

[U49] PHP：只读属性
来源：http://gy.lnxyls.cn

public readonly string $name
来源：http://bl.9csxet.cn

[U50] PHP：构造器属性提升
来源：http://ob.yuntaijiaju.cn

public function __construct(private int $id) {}
来源：http://il.521024.cn

[U51] PHP：数组解构
来源：http://hx.bjjhwx.cn

[$a, $b] = $arr;
来源：http://va.newstarts.cn

[U52] PHP：箭头函数
来源：http://fm.hahajie.cn

$double = fn($x) => $x * 2;
来源：http://ec.muxihuayi.cn

[U53] PHP：空合并运算符
来源：http://pt.colortex.cn

$v = $a ?? $b ?? "default";
来源：http://ef.521024.cn

[U54] PHP：空安全调用
来源：http://vi.huixinmuqiang.cn

$obj?->method()
来源：http://xq.newstarts.cn

[U55] PHP：match 表达式
来源：http://la.wgjwhj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dk.wgjwhj.cn

[U56] PHP：命名参数
来源：http://ek.shtwfgs.cn

f(a: 1, b: 2)
来源：http://in.hnjuh.cn

[U57] PHP：字符串插值
来源：http://lq.521024.cn

"值: {$a}"
来源：http://je.jctech888.com.cn

[U58] PHP：数组三件套
来源：http://cf.9csxet.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vt.shxzskj.cn

[U59] PHP：自定义排序
来源：http://un.huixiangedu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mw.521024.cn

[U60] PHP：JSON 编解码
来源：http://wi.jianghongdianzi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ey.haigaiapp.cn

[U61] PHP：正则
来源：http://zx.nicolike.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ge.muxihuayi.cn

[U62] PHP：日期对象
来源：http://ga.huixinmuqiang.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://im.panjiajie.cn

[U63] PHP：文件读写
来源：http://hs.nicolike.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sz.521024.cn

[U64] PHP：目录遍历
来源：http://yb.yuexingan06.cn

glob("dir/*.php");  scandir("dir");
来源：http://wg.asd995.cn

[U65] PHP：会话
来源：http://qo.bjjhwx.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ot.nicolike.cn

[U66] PHP：设置 Cookie
来源：http://bb.huixinmuqiang.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ju.colortex.cn

[U67] PHP：处理文件上传
来源：http://jo.muxihuayi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bg.huixinmuqiang.cn

[U68] PHP：PDO 连接
来源：http://lf.shxzukj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://oq.shxzskj.cn

[U69] PHP：PDO 预处理
来源：http://av.lnxyls.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xv.jctech888.com.cn

[U70] PHP：PDO 事务
来源：http://qh.jctech888.com.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mp.newstarts.cn

[U71] PHP：抛出异常
来源：http://pl.haigaiapp.cn

throw new RuntimeException("失败", 500);
来源：http://am.shtwfgs.cn

[U72] PHP：写错误日志
来源：http://on.huanxung.cn

error_log("失败: " . $e->getMessage());
来源：http://nh.huixinmuqiang.cn

[U73] PHP：读取 ini 配置
来源：http://xs.yuntaijiaju.cn

parse_ini_file("config.ini", true)
来源：http://lg.hahajie.cn

[U74] PHP：读取环境变量
来源：http://mq.521024.cn

getenv("APP_ENV") ?: "production"
来源：http://cj.jianghongdianzi.cn

[U75] PHP：依赖注入
来源：http://px.jianghongdianzi.cn

composer require psr/container
来源：http://ez.shxzskj.cn

[U76] PHP：简单路由
来源：http://em.huixinmuqiang.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xl.nszjky.cn

[U77] PHP：模板渲染
来源：http://mi.newstarts.cn

composer require twig/twig
来源：http://uh.bookmarksfly.cn

[U78] PHP：单元测试
来源：http://ri.jianghongdianzi.cn

composer require --dev phpunit/phpunit
来源：http://mu.lnxyls.cn

[U79] PHP：静态分析
来源：http://rj.bookmarksfly.cn

composer require --dev phpstan/phpstan
来源：http://gg.nicolike.cn

[U80] PHP：代码规范修复
来源：http://ud.shxzskj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://iy.hahajie.cn

[U81] JS：初始化项目
来源：http://nn.521024.cn

npm init -y;  npm i express
来源：http://xk.muxihuayi.cn

[U82] JS：package.json 脚本
来源：http://lh.shxzskj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gv.lnxyls.cn

[U83] JS：ES Module 导入导出
来源：http://qx.shtwfgs.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vl.lnxyls.cn

[U84] JS：CommonJS 写法
来源：http://sl.panjiajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ak.gzmigu.cn

[U85] JS：可选链
来源：http://rv.nszjky.cn

a?.b?.c
来源：http://ts.yuexingan06.cn

[U86] JS：空值合并
来源：http://hp.hnjuh.cn

a ?? b
来源：http://lz.muxihuayi.cn

[U87] JS：解构默认值
来源：http://pg.wgjwhj.cn

const { a = 1, b = 2 } = obj;
来源：http://oe.chemitech.net.cn

[U88] JS：对象展开合并
来源：http://pg.shxzskj.cn

{ ...a, ...b }
来源：http://vg.bookmarksfly.cn


<!-- 参考信息 -->