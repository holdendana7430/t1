代发 wailian999

[T01] Kotlin：Hello World
来源：http://lc.panjiajie.cn

println("Hello")
来源：http://ww.521024.cn

[T02] Kotlin：变量
来源：http://nz.hahajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zt.szxytkj.cn

[T03] Kotlin：字符串模板
来源：http://sv.newstarts.cn

"值: $b"
来源：http://fz.lnxyls.cn

[T04] Kotlin：空安全
来源：http://ju.yuexingan06.cn

val n: String? = null;  n?.length
来源：http://hb.9csxet.cn

[T05] Kotlin：when 表达式
来源：http://mb.jctech888.com.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vm.huixinmuqiang.cn

[T06] Kotlin：集合映射
来源：http://lx.newstarts.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://to.huixiangedu.cn

[T07] Kotlin：集合过滤
来源：http://ua.nszjky.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://nn.haigaiapp.cn

[T08] Kotlin：数据类
来源：http://ns.yuntaijiaju.cn

data class User(val name: String, val age: Int)
来源：http://nx.chemitech.net.cn

[T09] Kotlin：扩展函数
来源：http://ok.9csxet.cn

fun String.exclaim() = this + "!"
来源：http://pg.yuntaijiaju.cn

[T10] Kotlin：默认参数
来源：http://ao.521024.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://kh.shxzukj.cn

[T11] Kotlin：协程
来源：http://yb.yuntaijiaju.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wn.jianghongdianzi.cn

[T12] Kotlin：解构声明
来源：http://je.huixinmuqiang.cn

val (a, b) = Pair(1, 2)
来源：http://iz.chemitech.net.cn

[T13] Kotlin：只读 Map
来源：http://jr.haigaiapp.cn

val m = mapOf("a" to 1)
来源：http://xm.huixinmuqiang.cn

[T14] Kotlin：循环
来源：http://am.huixinmuqiang.cn

for (i in 1..10) println(i)
来源：http://hh.jctech888.com.cn

[T15] Kotlin：接口
来源：http://ah.gzmigu.cn

interface Shape { fun area(): Double }
来源：http://ud.shxzskj.cn

[T16] Swift：Hello World
来源：http://vv.hnjuh.cn

print("Hello")
来源：http://sv.lnxyls.cn

[T17] Swift：变量与常量
来源：http://ue.wgjwhj.cn

var a = 1;  let b = 2
来源：http://km.bjjhwx.cn

[T18] Swift：字符串插值
来源：http://oa.bookmarksfly.cn

"值: \(b)"
来源：http://kj.muxihuayi.cn

[T19] Swift：可选绑定
来源：http://tk.shxzskj.cn

if let n = opt { print(n) }
来源：http://bu.hnjuh.cn

[T20] Swift：数组操作
来源：http://re.szsharing.cn

var a = [1, 2, 3];  a.append(4)
来源：http://vp.muxihuayi.cn

[T21] Swift：遍历
来源：http://mz.hnjuh.cn

for x in a { print(x) }
来源：http://an.jctech888.com.cn

[T22] Swift：字典
来源：http://lu.hnjuh.cn

var d = ["a": 1];  d["b"] = 2
来源：http://rl.bjjhwx.cn

[T23] Swift：函数
来源：http://kc.huixiangedu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ih.huixinmuqiang.cn

[T24] Swift：闭包
来源：http://qm.chemitech.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://cd.shtwfgs.cn

[T25] Swift：结构体
来源：http://ff.huixinmuqiang.cn

struct P { var x: Int }
来源：http://nq.panjiajie.cn

[T26] Swift：类与重写
来源：http://ma.huanxung.cn

class A: Base { override func f() {} }
来源：http://cs.asd995.cn

[T27] Swift：错误处理
来源：http://dx.lnxyls.cn

do { try f() } catch { print(error) }
来源：http://fo.bjjhwx.cn

[T28] Swift：枚举
来源：http://nv.shxzukj.cn

enum Color { case red, green }
来源：http://hd.9csxet.cn

[T29] Swift：guard 提前返回
来源：http://rm.muxihuayi.cn

guard let x = opt else { return }
来源：http://dr.newstarts.cn

[T30] Swift：协议
来源：http://rp.hnjuh.cn

protocol Shape { func area() -> Double }
来源：http://hi.bookmarksfly.cn

[T31] Lua：Hello World
来源：http://yw.muxihuayi.cn

print("Hello")
来源：http://ng.wgjwhj.cn

[T32] Lua：局部变量
来源：http://np.gzmigu.cn

local a = 1
来源：http://fg.hnjuh.cn

[T33] Lua：表（数组）
来源：http://uw.lnxyls.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://bv.newstarts.cn

[T34] Lua：遍历表
来源：http://qz.hnjuh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://fx.newstarts.cn

[T35] Lua：字典表
来源：http://zm.hnjuh.cn

local d = { a = 1 };  d.b = 2
来源：http://oh.bookmarksfly.cn

[T36] Lua：函数
来源：http://cf.521024.cn

function add(a, b) return a + b end
来源：http://dn.colortex.cn

[T37] Lua：字符串拼接
来源：http://hd.asd995.cn

"a" .. "b"
来源：http://qu.yuntaijiaju.cn

[T38] Lua：条件
来源：http://sa.shxzukj.cn

if x > 0 then print("正") end
来源：http://uv.shxzskj.cn

[T39] Lua：模式匹配
来源：http://iq.colortex.cn

string.find(s, "%d+")
来源：http://jl.shxzukj.cn

[T40] Lua：元表
来源：http://ps.shxzukj.cn

setmetatable({}, { __index = base })
来源：http://qq.asd995.cn

[T41] Perl：Hello World
来源：http://wl.huixinmuqiang.cn

print "Hello\n";
来源：http://qo.bookmarksfly.cn

[T42] Perl：变量类型
来源：http://gt.yuntaijiaju.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hd.9csxet.cn

[T43] Perl：字符串插值
来源：http://dz.jianghongdianzi.cn

"值: $a"
来源：http://st.szxytkj.cn

[T44] Perl：条件
来源：http://cp.haigaiapp.cn

if ($a > 0) { print "正"; }
来源：http://zz.haigaiapp.cn

[T45] Perl：数组遍历
来源：http://iu.newstarts.cn

for my $x (@arr) { print $x; }
来源：http://mx.colortex.cn

[T46] Perl：哈希操作
来源：http://xk.521024.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sn.colortex.cn

[T47] Perl：正则捕获
来源：http://oy.huanxung.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vk.yuntaijiaju.cn

[T48] Perl：正则替换
来源：http://gn.chemitech.net.cn

$s =~ s/old/new/g;
来源：http://cg.jctech888.com.cn

[T49] Perl：函数
来源：http://rm.huixinmuqiang.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sr.colortex.cn

[T50] Perl：逐行读文件
来源：http://lm.9csxet.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ff.hahajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://qc.panjiajie.cn

[T51] Scala：Hello World
来源：http://os.huixiangedu.cn

println("Hello")
来源：http://hw.muxihuayi.cn

[T52] Scala：变量
来源：http://qd.colortex.cn

val a = 1;  var b = 2
来源：http://zv.huanxung.cn

[T53] Scala：字符串插值
来源：http://as.hahajie.cn

s"值: $b"
来源：http://ot.hnjuh.cn

[T54] Scala：集合映射
来源：http://lb.newstarts.cn

List(1, 2, 3).map(_ * 2)
来源：http://cx.haigaiapp.cn

[T55] Scala：集合过滤
来源：http://oz.yuexingan06.cn

List(1, 2, 3).filter(_ > 1)
来源：http://pj.muxihuayi.cn

[T56] Scala：样例类
来源：http://by.9csxet.cn

case class User(name: String, age: Int)
来源：http://fx.shtwfgs.cn

[T57] Scala：模式匹配
来源：http://dd.panjiajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vw.wgjwhj.cn

[T58] Scala：函数定义
来源：http://xm.521024.cn

def add(a: Int, b: Int): Int = a + b
来源：http://of.gzmigu.cn

[T59] Scala：循环
来源：http://mk.bjjhwx.cn

for (i <- 1 to 10) println(i)
来源：http://eh.gzmigu.cn

[T60] Scala：折叠
来源：http://em.hnjuh.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://iw.panjiajie.cn

================================================================================
来源：http://cc.lnxyls.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zj.nicolike.cn

================================================================================
来源：http://wm.lnxyls.cn

[U01] Py：创建虚拟环境
来源：http://lo.bjjhwx.cn

python -m venv .venv && source .venv/bin/activate
来源：http://lp.nicolike.cn

[U02] Py：导出 / 安装依赖
来源：http://lz.asd995.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ab.shtwfgs.cn

[U03] Py：加载 .env 配置
来源：http://ye.chemitech.net.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qw.nszjky.cn

[U04] Py：变量调试打印
来源：http://fd.colortex.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xv.521024.cn

[U05] Py：列表去重且保序
来源：http://me.nszjky.cn

list(dict.fromkeys(arr))
来源：http://fp.shtwfgs.cn

[U06] Py：合并两个字典
来源：http://il.huixinmuqiang.cn

{**a, **b}
来源：http://ye.9csxet.cn

[U07] Py：反转字典键值
来源：http://mr.nszjky.cn

{v: k for k, v in d.items()}
来源：http://cv.szsharing.cn

[U08] Py：展平二维列表
来源：http://xf.lnxyls.cn

[y for x in nested for y in x]
来源：http://oa.bookmarksfly.cn

[U09] Py：字典取最大值的键
来源：http://be.yuntaijiaju.cn

max(d, key=d.get)
来源：http://jo.huixinmuqiang.cn

[U10] Py：按值排序字典
来源：http://xc.jianghongdianzi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://un.hnjuh.cn

[U11] Py：生成器表达式
来源：http://eg.jctech888.com.cn

(x * 2 for x in arr)
来源：http://oy.shxzukj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://kx.shxzukj.cn

Counter(arr).most_common(3)
来源：http://ck.newstarts.cn

[U13] Py：固定长度队列
来源：http://ia.panjiajie.cn

deque(maxlen=10)
来源：http://jp.szsharing.cn

[U14] Py：分组收集到列表
来源：http://vc.asd995.cn

defaultdict(list)
来源：http://rz.lnxyls.cn

[U15] Py：高精度计时
来源：http://am.asd995.cn

t = time.perf_counter()
来源：http://kb.huixinmuqiang.cn

[U16] Py：命令行参数解析
来源：http://ql.yuntaijiaju.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gi.muxihuayi.cn

[U17] Py：初始化日志
来源：http://fg.chemitech.net.cn

logging.basicConfig(level=logging.INFO)
来源：http://ar.szxytkj.cn

[U18] Py：预编译正则
来源：http://lv.szxytkj.cn

pat = re.compile(r"\d+")
来源：http://em.haigaiapp.cn

[U19] Py：正则替换带回调
来源：http://ee.nszjky.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lq.szxytkj.cn

[U20] Py：缓存函数结果
来源：http://be.shtwfgs.cn

@functools.lru_cache(maxsize=None)
来源：http://dj.szxytkj.cn

[U21] Py：自定义上下文管理器
来源：http://qc.szxytkj.cn

@contextlib.contextmanager
来源：http://ls.nicolike.cn

[U22] Py：矩阵转置
来源：http://nq.shxzskj.cn

list(zip(*m))
来源：http://eh.9csxet.cn

[U23] Py：分块读取大文件
来源：http://wq.nszjky.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pt.huixinmuqiang.cn

[U24] Py：路径操作
来源：http://dv.521024.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pd.521024.cn

[U25] Py：CSV 按字典读
来源：http://tw.huixiangedu.cn

csv.DictReader(f)
来源：http://eb.nszjky.cn

[U26] Py：并发下载
来源：http://tc.yuexingan06.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bd.shxzukj.cn

[U27] Py：异步 HTTP
来源：http://fc.jctech888.com.cn

aiohttp.ClientSession() 配合 async with
来源：http://nv.asd995.cn

[U28] Py：类型别名
来源：http://ca.9csxet.cn

UserId = int
来源：http://ps.hahajie.cn

[U29] Py：属性校验
来源：http://fe.jctech888.com.cn

@property 与 @x.setter 配合
来源：http://ue.bjjhwx.cn

[U30] Py：数据类
来源：http://dq.bjjhwx.cn

@dataclass(slots=True)
来源：http://na.shtwfgs.cn

[U31] Py：单测
来源：http://hq.yuntaijiaju.cn

python -m pytest -q
来源：http://ia.panjiajie.cn

[U32] Py：代码格式化
来源：http://ws.bookmarksfly.cn

ruff format . && ruff check --fix .
来源：http://ph.bjjhwx.cn

[U33] Py：打包发布
来源：http://iq.jianghongdianzi.cn

python -m build  （依赖 pyproject.toml）
来源：http://vq.521024.cn

[U34] Py：判断编码
来源：http://fu.hnjuh.cn

chardet.detect(raw)
来源：http://yz.muxihuayi.cn

[U35] Py：发送邮件
来源：http://pw.haigaiapp.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vd.chemitech.net.cn

[U36] Py：定时任务
来源：http://ni.bjjhwx.cn

schedule.every(10).minutes.do(job)
来源：http://bx.hnjuh.cn

[U37] Py：读写 Excel
来源：http://yn.jctech888.com.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ch.yuntaijiaju.cn

[U38] Py：获取脚本所在目录
来源：http://to.huixiangedu.cn

Path(__file__).resolve().parent
来源：http://im.hnjuh.cn

[U39] Py：判断是否在交互环境
来源：http://db.panjiajie.cn

sys.stdout.isatty()
来源：http://ec.shxzskj.cn

[U40] Py：打印到标准错误
来源：http://cq.colortex.cn

print("err", file=sys.stderr)
来源：http://wn.huixinmuqiang.cn

[U41] PHP：初始化 Composer 项目
来源：http://ow.bookmarksfly.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://rc.521024.cn

[U42] PHP：PSR-4 自动加载
来源：http://yd.szxytkj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zs.hahajie.cn

[U43] PHP：声明命名空间
来源：http://oi.521024.cn

namespace App\Http;
来源：http://qe.huixiangedu.cn

[U44] PHP：开启严格类型
来源：http://ox.bjjhwx.cn

declare(strict_types=1);
来源：http://ds.szsharing.cn

[U45] PHP：类型声明与返回类型
来源：http://dx.shxzukj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://mb.yuexingan06.cn

[U46] PHP：可空类型
来源：http://xf.bookmarksfly.cn

?string $name = null
来源：http://tf.yuexingan06.cn

[U47] PHP：联合类型
来源：http://ge.gzmigu.cn

int|string $id
来源：http://cu.shxzukj.cn

[U48] PHP：纯枚举
来源：http://vz.shxzskj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nr.haigaiapp.cn

[U49] PHP：只读属性
来源：http://aj.chemitech.net.cn

public readonly string $name
来源：http://dr.colortex.cn

[U50] PHP：构造器属性提升
来源：http://fv.asd995.cn

public function __construct(private int $id) {}
来源：http://jp.jianghongdianzi.cn

[U51] PHP：数组解构
来源：http://zq.shxzskj.cn

[$a, $b] = $arr;
来源：http://gs.yuexingan06.cn

[U52] PHP：箭头函数
来源：http://nh.jctech888.com.cn

$double = fn($x) => $x * 2;
来源：http://zy.chemitech.net.cn

[U53] PHP：空合并运算符
来源：http://rd.hnjuh.cn

$v = $a ?? $b ?? "default";
来源：http://cd.szxytkj.cn

[U54] PHP：空安全调用
来源：http://oj.huixiangedu.cn

$obj?->method()
来源：http://al.shxzukj.cn

[U55] PHP：match 表达式
来源：http://nc.hahajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xg.haigaiapp.cn

[U56] PHP：命名参数
来源：http://hc.asd995.cn

f(a: 1, b: 2)
来源：http://nu.hnjuh.cn

[U57] PHP：字符串插值
来源：http://pq.huanxung.cn

"值: {$a}"
来源：http://dr.asd995.cn

[U58] PHP：数组三件套
来源：http://us.hahajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hh.shxzukj.cn

[U59] PHP：自定义排序
来源：http://la.huixiangedu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gm.bjjhwx.cn

[U60] PHP：JSON 编解码
来源：http://ij.huixinmuqiang.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://sk.haigaiapp.cn

[U61] PHP：正则
来源：http://mc.yuexingan06.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gk.hahajie.cn

[U62] PHP：日期对象
来源：http://ot.521024.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ec.huixinmuqiang.cn

[U63] PHP：文件读写
来源：http://ph.huixiangedu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gc.nicolike.cn

[U64] PHP：目录遍历
来源：http://yt.lnxyls.cn

glob("dir/*.php");  scandir("dir");
来源：http://uv.shxzskj.cn

[U65] PHP：会话
来源：http://br.colortex.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://dn.panjiajie.cn

[U66] PHP：设置 Cookie
来源：http://uk.nicolike.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fw.haigaiapp.cn

[U67] PHP：处理文件上传
来源：http://vw.panjiajie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ck.colortex.cn

[U68] PHP：PDO 连接
来源：http://qi.shxzskj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ff.haigaiapp.cn

[U69] PHP：PDO 预处理
来源：http://yk.wgjwhj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qc.colortex.cn

[U70] PHP：PDO 事务
来源：http://kr.nszjky.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tu.szsharing.cn

[U71] PHP：抛出异常
来源：http://yb.hahajie.cn

throw new RuntimeException("失败", 500);
来源：http://pj.jianghongdianzi.cn

[U72] PHP：写错误日志
来源：http://mb.yuntaijiaju.cn

error_log("失败: " . $e->getMessage());
来源：http://uy.haigaiapp.cn

[U73] PHP：读取 ini 配置
来源：http://iy.nicolike.cn

parse_ini_file("config.ini", true)
来源：http://ea.chemitech.net.cn

[U74] PHP：读取环境变量
来源：http://ae.hnjuh.cn

getenv("APP_ENV") ?: "production"
来源：http://qx.bjjhwx.cn

[U75] PHP：依赖注入
来源：http://fz.shxzukj.cn

composer require psr/container
来源：http://dj.shxzskj.cn

[U76] PHP：简单路由
来源：http://pr.huixiangedu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qc.nszjky.cn

[U77] PHP：模板渲染
来源：http://ph.bookmarksfly.cn

composer require twig/twig
来源：http://zl.jianghongdianzi.cn

[U78] PHP：单元测试
来源：http://xo.lnxyls.cn

composer require --dev phpunit/phpunit
来源：http://tz.chemitech.net.cn

[U79] PHP：静态分析
来源：http://gz.colortex.cn

composer require --dev phpstan/phpstan
来源：http://fi.yuexingan06.cn

[U80] PHP：代码规范修复
来源：http://qx.colortex.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://vj.wgjwhj.cn

[U81] JS：初始化项目
来源：http://pg.9csxet.cn

npm init -y;  npm i express
来源：http://iz.bookmarksfly.cn

[U82] JS：package.json 脚本
来源：http://po.bookmarksfly.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kt.lnxyls.cn

[U83] JS：ES Module 导入导出
来源：http://mn.nszjky.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zp.wgjwhj.cn

[U84] JS：CommonJS 写法
来源：http://uu.panjiajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wv.szsharing.cn

[U85] JS：可选链
来源：http://mp.jianghongdianzi.cn

a?.b?.c
来源：http://bi.shxzukj.cn

[U86] JS：空值合并
来源：http://xr.szsharing.cn

a ?? b
来源：http://po.newstarts.cn

[U87] JS：解构默认值
来源：http://km.nicolike.cn

const { a = 1, b = 2 } = obj;
来源：http://zw.bjjhwx.cn

[U88] JS：对象展开合并
来源：http://xt.shtwfgs.cn

{ ...a, ...b }
来源：http://no.yuntaijiaju.cn


<!-- 参考信息 -->