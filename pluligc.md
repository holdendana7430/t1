代发 wailian999

[T01] Kotlin：Hello World
来源：http://uw.9csxet.cn

println("Hello")
来源：http://tq.haigaiapp.cn

[T02] Kotlin：变量
来源：http://hn.shtwfgs.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://iv.szsharing.cn

[T03] Kotlin：字符串模板
来源：http://vw.asd995.cn

"值: $b"
来源：http://wn.szsharing.cn

[T04] Kotlin：空安全
来源：http://nr.wgjwhj.cn

val n: String? = null;  n?.length
来源：http://zm.colortex.cn

[T05] Kotlin：when 表达式
来源：http://bl.haigaiapp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jb.jctech888.com.cn

[T06] Kotlin：集合映射
来源：http://mi.yuntaijiaju.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gb.newstarts.cn

[T07] Kotlin：集合过滤
来源：http://bd.huixiangedu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xi.muxihuayi.cn

[T08] Kotlin：数据类
来源：http://gw.lnxyls.cn

data class User(val name: String, val age: Int)
来源：http://xu.szxytkj.cn

[T09] Kotlin：扩展函数
来源：http://jp.lnxyls.cn

fun String.exclaim() = this + "!"
来源：http://ea.bookmarksfly.cn

[T10] Kotlin：默认参数
来源：http://fc.yuexingan06.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rm.huanxung.cn

[T11] Kotlin：协程
来源：http://np.colortex.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://uj.shxzskj.cn

[T12] Kotlin：解构声明
来源：http://px.huanxung.cn

val (a, b) = Pair(1, 2)
来源：http://im.asd995.cn

[T13] Kotlin：只读 Map
来源：http://zt.hnjuh.cn

val m = mapOf("a" to 1)
来源：http://lz.jctech888.com.cn

[T14] Kotlin：循环
来源：http://pp.nszjky.cn

for (i in 1..10) println(i)
来源：http://ua.jctech888.com.cn

[T15] Kotlin：接口
来源：http://rk.gzmigu.cn

interface Shape { fun area(): Double }
来源：http://nd.newstarts.cn

[T16] Swift：Hello World
来源：http://ym.jianghongdianzi.cn

print("Hello")
来源：http://st.haigaiapp.cn

[T17] Swift：变量与常量
来源：http://lt.yuntaijiaju.cn

var a = 1;  let b = 2
来源：http://yd.colortex.cn

[T18] Swift：字符串插值
来源：http://hp.yuexingan06.cn

"值: \(b)"
来源：http://ck.muxihuayi.cn

[T19] Swift：可选绑定
来源：http://xj.colortex.cn

if let n = opt { print(n) }
来源：http://ea.newstarts.cn

[T20] Swift：数组操作
来源：http://ad.chemitech.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qy.huixiangedu.cn

[T21] Swift：遍历
来源：http://of.hahajie.cn

for x in a { print(x) }
来源：http://ud.yuexingan06.cn

[T22] Swift：字典
来源：http://sb.shxzskj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://cq.wgjwhj.cn

[T23] Swift：函数
来源：http://eo.9csxet.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ik.yuexingan06.cn

[T24] Swift：闭包
来源：http://di.szxytkj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://fg.asd995.cn

[T25] Swift：结构体
来源：http://px.huixiangedu.cn

struct P { var x: Int }
来源：http://vp.nicolike.cn

[T26] Swift：类与重写
来源：http://ac.chemitech.net.cn

class A: Base { override func f() {} }
来源：http://cg.shtwfgs.cn

[T27] Swift：错误处理
来源：http://te.gzmigu.cn

do { try f() } catch { print(error) }
来源：http://nl.yuntaijiaju.cn

[T28] Swift：枚举
来源：http://ec.jctech888.com.cn

enum Color { case red, green }
来源：http://qm.yuntaijiaju.cn

[T29] Swift：guard 提前返回
来源：http://fg.huanxung.cn

guard let x = opt else { return }
来源：http://th.shxzukj.cn

[T30] Swift：协议
来源：http://un.nszjky.cn

protocol Shape { func area() -> Double }
来源：http://jp.shxzskj.cn

[T31] Lua：Hello World
来源：http://zs.jianghongdianzi.cn

print("Hello")
来源：http://xs.chemitech.net.cn

[T32] Lua：局部变量
来源：http://ap.colortex.cn

local a = 1
来源：http://rj.shtwfgs.cn

[T33] Lua：表（数组）
来源：http://sh.muxihuayi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vi.hahajie.cn

[T34] Lua：遍历表
来源：http://ji.nicolike.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://kj.huixinmuqiang.cn

[T35] Lua：字典表
来源：http://hy.bookmarksfly.cn

local d = { a = 1 };  d.b = 2
来源：http://hi.yuntaijiaju.cn

[T36] Lua：函数
来源：http://vi.9csxet.cn

function add(a, b) return a + b end
来源：http://qz.chemitech.net.cn

[T37] Lua：字符串拼接
来源：http://bd.shxzukj.cn

"a" .. "b"
来源：http://qo.muxihuayi.cn

[T38] Lua：条件
来源：http://os.haigaiapp.cn

if x > 0 then print("正") end
来源：http://yf.bookmarksfly.cn

[T39] Lua：模式匹配
来源：http://lu.szxytkj.cn

string.find(s, "%d+")
来源：http://dj.huixiangedu.cn

[T40] Lua：元表
来源：http://om.shtwfgs.cn

setmetatable({}, { __index = base })
来源：http://nw.haigaiapp.cn

[T41] Perl：Hello World
来源：http://ix.muxihuayi.cn

print "Hello\n";
来源：http://nl.bjjhwx.cn

[T42] Perl：变量类型
来源：http://ti.panjiajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jx.szsharing.cn

[T43] Perl：字符串插值
来源：http://wb.hnjuh.cn

"值: $a"
来源：http://sm.shxzukj.cn

[T44] Perl：条件
来源：http://dx.newstarts.cn

if ($a > 0) { print "正"; }
来源：http://ht.panjiajie.cn

[T45] Perl：数组遍历
来源：http://zb.bjjhwx.cn

for my $x (@arr) { print $x; }
来源：http://rr.colortex.cn

[T46] Perl：哈希操作
来源：http://ys.jianghongdianzi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hd.wgjwhj.cn

[T47] Perl：正则捕获
来源：http://oq.huixinmuqiang.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ha.huixinmuqiang.cn

[T48] Perl：正则替换
来源：http://gw.hahajie.cn

$s =~ s/old/new/g;
来源：http://ha.shxzukj.cn

[T49] Perl：函数
来源：http://fq.bjjhwx.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://id.yuexingan06.cn

[T50] Perl：逐行读文件
来源：http://xw.gzmigu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://hi.huanxung.cn

while (my $line = <$fh>) { print $line; }
来源：http://ur.yuntaijiaju.cn

[T51] Scala：Hello World
来源：http://ja.shtwfgs.cn

println("Hello")
来源：http://hb.huanxung.cn

[T52] Scala：变量
来源：http://jo.jianghongdianzi.cn

val a = 1;  var b = 2
来源：http://hi.jianghongdianzi.cn

[T53] Scala：字符串插值
来源：http://ou.huixiangedu.cn

s"值: $b"
来源：http://nv.colortex.cn

[T54] Scala：集合映射
来源：http://zh.colortex.cn

List(1, 2, 3).map(_ * 2)
来源：http://rj.shxzskj.cn

[T55] Scala：集合过滤
来源：http://jo.bjjhwx.cn

List(1, 2, 3).filter(_ > 1)
来源：http://dq.nszjky.cn

[T56] Scala：样例类
来源：http://ar.9csxet.cn

case class User(name: String, age: Int)
来源：http://cp.nszjky.cn

[T57] Scala：模式匹配
来源：http://bo.haigaiapp.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://xi.chemitech.net.cn

[T58] Scala：函数定义
来源：http://bi.shxzukj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ng.colortex.cn

[T59] Scala：循环
来源：http://um.muxihuayi.cn

for (i <- 1 to 10) println(i)
来源：http://wt.colortex.cn

[T60] Scala：折叠
来源：http://ht.yuntaijiaju.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sx.9csxet.cn

================================================================================
来源：http://iv.huanxung.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zw.asd995.cn

================================================================================
来源：http://bu.huixinmuqiang.cn

[U01] Py：创建虚拟环境
来源：http://mn.asd995.cn

python -m venv .venv && source .venv/bin/activate
来源：http://yi.521024.cn

[U02] Py：导出 / 安装依赖
来源：http://mw.huixinmuqiang.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pc.asd995.cn

[U03] Py：加载 .env 配置
来源：http://vs.521024.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://iw.szxytkj.cn

[U04] Py：变量调试打印
来源：http://jc.hahajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gn.huixiangedu.cn

[U05] Py：列表去重且保序
来源：http://ux.huanxung.cn

list(dict.fromkeys(arr))
来源：http://vj.huanxung.cn

[U06] Py：合并两个字典
来源：http://ee.nszjky.cn

{**a, **b}
来源：http://in.panjiajie.cn

[U07] Py：反转字典键值
来源：http://ur.panjiajie.cn

{v: k for k, v in d.items()}
来源：http://tz.bookmarksfly.cn

[U08] Py：展平二维列表
来源：http://cx.nszjky.cn

[y for x in nested for y in x]
来源：http://jw.jctech888.com.cn

[U09] Py：字典取最大值的键
来源：http://hn.newstarts.cn

max(d, key=d.get)
来源：http://pi.panjiajie.cn

[U10] Py：按值排序字典
来源：http://je.nszjky.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zn.521024.cn

[U11] Py：生成器表达式
来源：http://tf.huixiangedu.cn

(x * 2 for x in arr)
来源：http://bk.huixinmuqiang.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ve.9csxet.cn

Counter(arr).most_common(3)
来源：http://ff.szxytkj.cn

[U13] Py：固定长度队列
来源：http://vp.bjjhwx.cn

deque(maxlen=10)
来源：http://zp.haigaiapp.cn

[U14] Py：分组收集到列表
来源：http://gg.yuntaijiaju.cn

defaultdict(list)
来源：http://ui.wgjwhj.cn

[U15] Py：高精度计时
来源：http://lq.muxihuayi.cn

t = time.perf_counter()
来源：http://ai.521024.cn

[U16] Py：命令行参数解析
来源：http://xt.huanxung.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pt.9csxet.cn

[U17] Py：初始化日志
来源：http://zc.muxihuayi.cn

logging.basicConfig(level=logging.INFO)
来源：http://ir.bjjhwx.cn

[U18] Py：预编译正则
来源：http://rk.bjjhwx.cn

pat = re.compile(r"\d+")
来源：http://ow.szsharing.cn

[U19] Py：正则替换带回调
来源：http://zu.521024.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ii.chemitech.net.cn

[U20] Py：缓存函数结果
来源：http://iv.muxihuayi.cn

@functools.lru_cache(maxsize=None)
来源：http://it.lnxyls.cn

[U21] Py：自定义上下文管理器
来源：http://jb.yuntaijiaju.cn

@contextlib.contextmanager
来源：http://qa.jianghongdianzi.cn

[U22] Py：矩阵转置
来源：http://ts.shxzskj.cn

list(zip(*m))
来源：http://yi.9csxet.cn

[U23] Py：分块读取大文件
来源：http://xu.bjjhwx.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cx.bookmarksfly.cn

[U24] Py：路径操作
来源：http://ze.shtwfgs.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yf.jianghongdianzi.cn

[U25] Py：CSV 按字典读
来源：http://jf.yuntaijiaju.cn

csv.DictReader(f)
来源：http://wz.521024.cn

[U26] Py：并发下载
来源：http://ie.nszjky.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hb.521024.cn

[U27] Py：异步 HTTP
来源：http://lb.shxzukj.cn

aiohttp.ClientSession() 配合 async with
来源：http://jk.newstarts.cn

[U28] Py：类型别名
来源：http://gq.panjiajie.cn

UserId = int
来源：http://ii.szsharing.cn

[U29] Py：属性校验
来源：http://rl.lnxyls.cn

@property 与 @x.setter 配合
来源：http://xr.newstarts.cn

[U30] Py：数据类
来源：http://rt.nicolike.cn

@dataclass(slots=True)
来源：http://ho.colortex.cn

[U31] Py：单测
来源：http://la.jianghongdianzi.cn

python -m pytest -q
来源：http://xx.colortex.cn

[U32] Py：代码格式化
来源：http://qg.shxzskj.cn

ruff format . && ruff check --fix .
来源：http://ft.chemitech.net.cn

[U33] Py：打包发布
来源：http://jh.yuntaijiaju.cn

python -m build  （依赖 pyproject.toml）
来源：http://rv.nicolike.cn

[U34] Py：判断编码
来源：http://bh.panjiajie.cn

chardet.detect(raw)
来源：http://db.muxihuayi.cn

[U35] Py：发送邮件
来源：http://dl.bookmarksfly.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://re.newstarts.cn

[U36] Py：定时任务
来源：http://sq.9csxet.cn

schedule.every(10).minutes.do(job)
来源：http://pr.hahajie.cn

[U37] Py：读写 Excel
来源：http://bc.huanxung.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ph.huixiangedu.cn

[U38] Py：获取脚本所在目录
来源：http://gy.hahajie.cn

Path(__file__).resolve().parent
来源：http://em.nicolike.cn

[U39] Py：判断是否在交互环境
来源：http://yt.bookmarksfly.cn

sys.stdout.isatty()
来源：http://ce.jianghongdianzi.cn

[U40] Py：打印到标准错误
来源：http://bt.lnxyls.cn

print("err", file=sys.stderr)
来源：http://vl.yuexingan06.cn

[U41] PHP：初始化 Composer 项目
来源：http://gt.bookmarksfly.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ey.nszjky.cn

[U42] PHP：PSR-4 自动加载
来源：http://bu.bjjhwx.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://in.jctech888.com.cn

[U43] PHP：声明命名空间
来源：http://et.nicolike.cn

namespace App\Http;
来源：http://py.yuntaijiaju.cn

[U44] PHP：开启严格类型
来源：http://dq.chemitech.net.cn

declare(strict_types=1);
来源：http://bn.9csxet.cn

[U45] PHP：类型声明与返回类型
来源：http://vv.asd995.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://gb.asd995.cn

[U46] PHP：可空类型
来源：http://ka.shtwfgs.cn

?string $name = null
来源：http://ei.yuexingan06.cn

[U47] PHP：联合类型
来源：http://oh.gzmigu.cn

int|string $id
来源：http://ne.nszjky.cn

[U48] PHP：纯枚举
来源：http://or.shxzukj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sl.shxzskj.cn

[U49] PHP：只读属性
来源：http://zz.haigaiapp.cn

public readonly string $name
来源：http://dt.bookmarksfly.cn

[U50] PHP：构造器属性提升
来源：http://hj.asd995.cn

public function __construct(private int $id) {}
来源：http://vj.panjiajie.cn

[U51] PHP：数组解构
来源：http://vm.nicolike.cn

[$a, $b] = $arr;
来源：http://vf.yuntaijiaju.cn

[U52] PHP：箭头函数
来源：http://om.jianghongdianzi.cn

$double = fn($x) => $x * 2;
来源：http://hx.newstarts.cn

[U53] PHP：空合并运算符
来源：http://px.hahajie.cn

$v = $a ?? $b ?? "default";
来源：http://dz.muxihuayi.cn

[U54] PHP：空安全调用
来源：http://eu.huanxung.cn

$obj?->method()
来源：http://zc.jianghongdianzi.cn

[U55] PHP：match 表达式
来源：http://rv.lnxyls.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lx.hahajie.cn

[U56] PHP：命名参数
来源：http://ag.bjjhwx.cn

f(a: 1, b: 2)
来源：http://xx.bjjhwx.cn

[U57] PHP：字符串插值
来源：http://ps.huixiangedu.cn

"值: {$a}"
来源：http://gq.shxzukj.cn

[U58] PHP：数组三件套
来源：http://dz.hnjuh.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ov.bjjhwx.cn

[U59] PHP：自定义排序
来源：http://wl.shxzskj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iz.muxihuayi.cn

[U60] PHP：JSON 编解码
来源：http://zp.haigaiapp.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wz.shtwfgs.cn

[U61] PHP：正则
来源：http://iz.nicolike.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ds.bjjhwx.cn

[U62] PHP：日期对象
来源：http://tj.huixiangedu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vh.gzmigu.cn

[U63] PHP：文件读写
来源：http://vq.huanxung.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pu.gzmigu.cn

[U64] PHP：目录遍历
来源：http://qc.panjiajie.cn

glob("dir/*.php");  scandir("dir");
来源：http://hj.jctech888.com.cn

[U65] PHP：会话
来源：http://xh.huanxung.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://zy.muxihuayi.cn

[U66] PHP：设置 Cookie
来源：http://qe.nicolike.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kr.jctech888.com.cn

[U67] PHP：处理文件上传
来源：http://rh.bookmarksfly.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jv.9csxet.cn

[U68] PHP：PDO 连接
来源：http://yv.9csxet.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://se.haigaiapp.cn

[U69] PHP：PDO 预处理
来源：http://ht.bookmarksfly.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ut.huixinmuqiang.cn

[U70] PHP：PDO 事务
来源：http://jo.huixinmuqiang.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wl.chemitech.net.cn

[U71] PHP：抛出异常
来源：http://ct.haigaiapp.cn

throw new RuntimeException("失败", 500);
来源：http://kb.huixinmuqiang.cn

[U72] PHP：写错误日志
来源：http://ih.szxytkj.cn

error_log("失败: " . $e->getMessage());
来源：http://zz.shtwfgs.cn

[U73] PHP：读取 ini 配置
来源：http://im.lnxyls.cn

parse_ini_file("config.ini", true)
来源：http://ie.nszjky.cn

[U74] PHP：读取环境变量
来源：http://xr.newstarts.cn

getenv("APP_ENV") ?: "production"
来源：http://ev.shtwfgs.cn

[U75] PHP：依赖注入
来源：http://nb.lnxyls.cn

composer require psr/container
来源：http://wo.asd995.cn

[U76] PHP：简单路由
来源：http://hq.521024.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wy.hahajie.cn

[U77] PHP：模板渲染
来源：http://bd.9csxet.cn

composer require twig/twig
来源：http://eo.bookmarksfly.cn

[U78] PHP：单元测试
来源：http://ek.bjjhwx.cn

composer require --dev phpunit/phpunit
来源：http://rr.panjiajie.cn

[U79] PHP：静态分析
来源：http://bo.wgjwhj.cn

composer require --dev phpstan/phpstan
来源：http://yn.shtwfgs.cn

[U80] PHP：代码规范修复
来源：http://dl.nszjky.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ae.yuntaijiaju.cn

[U81] JS：初始化项目
来源：http://km.asd995.cn

npm init -y;  npm i express
来源：http://gh.shxzskj.cn

[U82] JS：package.json 脚本
来源：http://mb.huanxung.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zf.colortex.cn

[U83] JS：ES Module 导入导出
来源：http://fl.bjjhwx.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ro.szsharing.cn

[U84] JS：CommonJS 写法
来源：http://la.jianghongdianzi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://zo.huixiangedu.cn

[U85] JS：可选链
来源：http://vw.huixiangedu.cn

a?.b?.c
来源：http://wc.chemitech.net.cn

[U86] JS：空值合并
来源：http://mp.nicolike.cn

a ?? b
来源：http://op.jianghongdianzi.cn

[U87] JS：解构默认值
来源：http://tn.shtwfgs.cn

const { a = 1, b = 2 } = obj;
来源：http://ti.jctech888.com.cn

[U88] JS：对象展开合并
来源：http://mq.bookmarksfly.cn

{ ...a, ...b }
来源：http://do.bookmarksfly.cn


<!-- 参考信息 -->