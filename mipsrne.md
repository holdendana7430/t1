代发 wailian999

[T05] Kotlin：when 表达式
来源：http://cx.chemitech.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ir.huixinmuqiang.cn

[T06] Kotlin：集合映射
来源：http://jq.jctech888.com.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fb.nszjky.cn

[T07] Kotlin：集合过滤
来源：http://le.newstarts.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vs.huixinmuqiang.cn

[T08] Kotlin：数据类
来源：http://yr.shxzukj.cn

data class User(val name: String, val age: Int)
来源：http://dj.shxzukj.cn

[T09] Kotlin：扩展函数
来源：http://qk.haigaiapp.cn

fun String.exclaim() = this + "!"
来源：http://ik.9csxet.cn

[T10] Kotlin：默认参数
来源：http://sq.shtwfgs.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://mk.szsharing.cn

[T11] Kotlin：协程
来源：http://nc.shxzukj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bc.wgjwhj.cn

[T12] Kotlin：解构声明
来源：http://ch.newstarts.cn

val (a, b) = Pair(1, 2)
来源：http://rv.lnxyls.cn

[T13] Kotlin：只读 Map
来源：http://nu.shxzskj.cn

val m = mapOf("a" to 1)
来源：http://jq.haigaiapp.cn

[T14] Kotlin：循环
来源：http://yw.shxzskj.cn

for (i in 1..10) println(i)
来源：http://xi.huixiangedu.cn

[T15] Kotlin：接口
来源：http://cn.huixinmuqiang.cn

interface Shape { fun area(): Double }
来源：http://ey.huixinmuqiang.cn

[T16] Swift：Hello World
来源：http://nl.yuexingan06.cn

print("Hello")
来源：http://bj.chemitech.net.cn

[T17] Swift：变量与常量
来源：http://je.shxzukj.cn

var a = 1;  let b = 2
来源：http://ti.lnxyls.cn

[T18] Swift：字符串插值
来源：http://bs.hnjuh.cn

"值: \(b)"
来源：http://qv.jianghongdianzi.cn

[T19] Swift：可选绑定
来源：http://lp.muxihuayi.cn

if let n = opt { print(n) }
来源：http://va.yuntaijiaju.cn

[T20] Swift：数组操作
来源：http://nc.huanxung.cn

var a = [1, 2, 3];  a.append(4)
来源：http://sw.colortex.cn

[T21] Swift：遍历
来源：http://hw.yuexingan06.cn

for x in a { print(x) }
来源：http://pe.haigaiapp.cn

[T22] Swift：字典
来源：http://ro.szsharing.cn

var d = ["a": 1];  d["b"] = 2
来源：http://dl.gzmigu.cn

[T23] Swift：函数
来源：http://zi.nszjky.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ev.shxzukj.cn

[T24] Swift：闭包
来源：http://am.jctech888.com.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://uz.nicolike.cn

[T25] Swift：结构体
来源：http://ha.yuexingan06.cn

struct P { var x: Int }
来源：http://fb.asd995.cn

[T26] Swift：类与重写
来源：http://im.yuntaijiaju.cn

class A: Base { override func f() {} }
来源：http://zx.lnxyls.cn

[T27] Swift：错误处理
来源：http://ie.asd995.cn

do { try f() } catch { print(error) }
来源：http://ty.shxzskj.cn

[T28] Swift：枚举
来源：http://wa.hnjuh.cn

enum Color { case red, green }
来源：http://nb.haigaiapp.cn

[T29] Swift：guard 提前返回
来源：http://ie.asd995.cn

guard let x = opt else { return }
来源：http://mg.shxzskj.cn

[T30] Swift：协议
来源：http://wd.jctech888.com.cn

protocol Shape { func area() -> Double }
来源：http://rv.nszjky.cn

[T31] Lua：Hello World
来源：http://oe.nszjky.cn

print("Hello")
来源：http://vd.nszjky.cn

[T32] Lua：局部变量
来源：http://sh.lnxyls.cn

local a = 1
来源：http://zv.wgjwhj.cn

[T33] Lua：表（数组）
来源：http://sq.shtwfgs.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ok.panjiajie.cn

[T34] Lua：遍历表
来源：http://kb.jctech888.com.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ne.colortex.cn

[T35] Lua：字典表
来源：http://zn.gzmigu.cn

local d = { a = 1 };  d.b = 2
来源：http://bd.lnxyls.cn

[T36] Lua：函数
来源：http://jv.shxzukj.cn

function add(a, b) return a + b end
来源：http://ha.szxytkj.cn

[T37] Lua：字符串拼接
来源：http://ch.panjiajie.cn

"a" .. "b"
来源：http://ue.nszjky.cn

[T38] Lua：条件
来源：http://ok.9csxet.cn

if x > 0 then print("正") end
来源：http://yj.jianghongdianzi.cn

[T39] Lua：模式匹配
来源：http://ho.huanxung.cn

string.find(s, "%d+")
来源：http://fc.bjjhwx.cn

[T40] Lua：元表
来源：http://yi.wgjwhj.cn

setmetatable({}, { __index = base })
来源：http://el.asd995.cn

[T41] Perl：Hello World
来源：http://xd.hnjuh.cn

print "Hello\n";
来源：http://jh.jctech888.com.cn

[T42] Perl：变量类型
来源：http://or.szsharing.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hd.yuntaijiaju.cn

[T43] Perl：字符串插值
来源：http://gu.521024.cn

"值: $a"
来源：http://eg.asd995.cn

[T44] Perl：条件
来源：http://wj.haigaiapp.cn

if ($a > 0) { print "正"; }
来源：http://as.nszjky.cn

[T45] Perl：数组遍历
来源：http://qh.9csxet.cn

for my $x (@arr) { print $x; }
来源：http://sp.asd995.cn

[T46] Perl：哈希操作
来源：http://lq.wgjwhj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dk.shtwfgs.cn

[T47] Perl：正则捕获
来源：http://sb.hnjuh.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wa.yuntaijiaju.cn

[T48] Perl：正则替换
来源：http://io.gzmigu.cn

$s =~ s/old/new/g;
来源：http://xk.huixinmuqiang.cn

[T49] Perl：函数
来源：http://fk.bookmarksfly.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ug.huixiangedu.cn

[T50] Perl：逐行读文件
来源：http://hn.nszjky.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xl.nszjky.cn

while (my $line = <$fh>) { print $line; }
来源：http://tg.bookmarksfly.cn

[T51] Scala：Hello World
来源：http://kf.9csxet.cn

println("Hello")
来源：http://uk.szxytkj.cn

[T52] Scala：变量
来源：http://wv.lnxyls.cn

val a = 1;  var b = 2
来源：http://ok.colortex.cn

[T53] Scala：字符串插值
来源：http://gn.yuexingan06.cn

s"值: $b"
来源：http://ai.shtwfgs.cn

[T54] Scala：集合映射
来源：http://qr.jctech888.com.cn

List(1, 2, 3).map(_ * 2)
来源：http://td.newstarts.cn

[T55] Scala：集合过滤
来源：http://li.shxzukj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://nq.nszjky.cn

[T56] Scala：样例类
来源：http://wx.nszjky.cn

case class User(name: String, age: Int)
来源：http://fd.newstarts.cn

[T57] Scala：模式匹配
来源：http://wl.newstarts.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://pd.jianghongdianzi.cn

[T58] Scala：函数定义
来源：http://si.huixinmuqiang.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ir.shtwfgs.cn

[T59] Scala：循环
来源：http://wy.gzmigu.cn

for (i <- 1 to 10) println(i)
来源：http://dm.hahajie.cn

[T60] Scala：折叠
来源：http://sk.panjiajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bc.9csxet.cn

================================================================================
来源：http://ag.huixiangedu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zs.panjiajie.cn

================================================================================
来源：http://ab.nszjky.cn

[U01] Py：创建虚拟环境
来源：http://as.bjjhwx.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ys.panjiajie.cn

[U02] Py：导出 / 安装依赖
来源：http://so.hahajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vl.hahajie.cn

[U03] Py：加载 .env 配置
来源：http://kx.9csxet.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qk.colortex.cn

[U04] Py：变量调试打印
来源：http://lp.colortex.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hc.hahajie.cn

[U05] Py：列表去重且保序
来源：http://fv.asd995.cn

list(dict.fromkeys(arr))
来源：http://fn.jianghongdianzi.cn

[U06] Py：合并两个字典
来源：http://rg.szxytkj.cn

{**a, **b}
来源：http://dw.lnxyls.cn

[U07] Py：反转字典键值
来源：http://qc.szsharing.cn

{v: k for k, v in d.items()}
来源：http://qq.bjjhwx.cn

[U08] Py：展平二维列表
来源：http://jp.shtwfgs.cn

[y for x in nested for y in x]
来源：http://tx.521024.cn

[U09] Py：字典取最大值的键
来源：http://cz.521024.cn

max(d, key=d.get)
来源：http://mn.wgjwhj.cn

[U10] Py：按值排序字典
来源：http://jp.wgjwhj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rh.yuntaijiaju.cn

[U11] Py：生成器表达式
来源：http://to.bookmarksfly.cn

(x * 2 for x in arr)
来源：http://mt.yuntaijiaju.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ao.bookmarksfly.cn

Counter(arr).most_common(3)
来源：http://lb.bjjhwx.cn

[U13] Py：固定长度队列
来源：http://mc.shxzukj.cn

deque(maxlen=10)
来源：http://ph.haigaiapp.cn

[U14] Py：分组收集到列表
来源：http://kc.szxytkj.cn

defaultdict(list)
来源：http://aa.shtwfgs.cn

[U15] Py：高精度计时
来源：http://vp.haigaiapp.cn

t = time.perf_counter()
来源：http://vx.nszjky.cn

[U16] Py：命令行参数解析
来源：http://sk.chemitech.net.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lt.nicolike.cn

[U17] Py：初始化日志
来源：http://tl.newstarts.cn

logging.basicConfig(level=logging.INFO)
来源：http://gj.nicolike.cn

[U18] Py：预编译正则
来源：http://ff.huanxung.cn

pat = re.compile(r"\d+")
来源：http://ar.yuexingan06.cn

[U19] Py：正则替换带回调
来源：http://kr.lnxyls.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kg.jctech888.com.cn

[U20] Py：缓存函数结果
来源：http://es.lnxyls.cn

@functools.lru_cache(maxsize=None)
来源：http://kt.chemitech.net.cn

[U21] Py：自定义上下文管理器
来源：http://fi.hnjuh.cn

@contextlib.contextmanager
来源：http://do.nszjky.cn

[U22] Py：矩阵转置
来源：http://oa.shtwfgs.cn

list(zip(*m))
来源：http://xs.colortex.cn

[U23] Py：分块读取大文件
来源：http://ky.wgjwhj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qt.9csxet.cn

[U24] Py：路径操作
来源：http://nk.jctech888.com.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ah.9csxet.cn

[U25] Py：CSV 按字典读
来源：http://bk.szsharing.cn

csv.DictReader(f)
来源：http://di.colortex.cn

[U26] Py：并发下载
来源：http://xt.huixinmuqiang.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qf.hnjuh.cn

[U27] Py：异步 HTTP
来源：http://tn.bjjhwx.cn

aiohttp.ClientSession() 配合 async with
来源：http://ps.colortex.cn

[U28] Py：类型别名
来源：http://ar.panjiajie.cn

UserId = int
来源：http://ys.521024.cn

[U29] Py：属性校验
来源：http://np.szsharing.cn

@property 与 @x.setter 配合
来源：http://hn.bookmarksfly.cn

[U30] Py：数据类
来源：http://gv.szsharing.cn

@dataclass(slots=True)
来源：http://if.szxytkj.cn

[U31] Py：单测
来源：http://bj.newstarts.cn

python -m pytest -q
来源：http://cu.huanxung.cn

[U32] Py：代码格式化
来源：http://gd.muxihuayi.cn

ruff format . && ruff check --fix .
来源：http://ym.bjjhwx.cn

[U33] Py：打包发布
来源：http://vq.hahajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://qp.bjjhwx.cn

[U34] Py：判断编码
来源：http://hx.shtwfgs.cn

chardet.detect(raw)
来源：http://gd.huixinmuqiang.cn

[U35] Py：发送邮件
来源：http://ta.nszjky.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vv.jianghongdianzi.cn

[U36] Py：定时任务
来源：http://yt.yuntaijiaju.cn

schedule.every(10).minutes.do(job)
来源：http://yc.521024.cn

[U37] Py：读写 Excel
来源：http://nq.chemitech.net.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ms.yuexingan06.cn

[U38] Py：获取脚本所在目录
来源：http://ol.yuntaijiaju.cn

Path(__file__).resolve().parent
来源：http://ui.muxihuayi.cn

[U39] Py：判断是否在交互环境
来源：http://hn.yuntaijiaju.cn

sys.stdout.isatty()
来源：http://kr.9csxet.cn

[U40] Py：打印到标准错误
来源：http://je.yuexingan06.cn

print("err", file=sys.stderr)
来源：http://bn.hnjuh.cn

[U41] PHP：初始化 Composer 项目
来源：http://xd.wgjwhj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://rd.9csxet.cn

[U42] PHP：PSR-4 自动加载
来源：http://mr.9csxet.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ky.asd995.cn

[U43] PHP：声明命名空间
来源：http://ik.gzmigu.cn

namespace App\Http;
来源：http://xe.9csxet.cn

[U44] PHP：开启严格类型
来源：http://wz.panjiajie.cn

declare(strict_types=1);
来源：http://py.szsharing.cn

[U45] PHP：类型声明与返回类型
来源：http://qg.shtwfgs.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://cs.asd995.cn

[U46] PHP：可空类型
来源：http://we.bookmarksfly.cn

?string $name = null
来源：http://px.shxzskj.cn

[U47] PHP：联合类型
来源：http://ea.jctech888.com.cn

int|string $id
来源：http://ch.yuntaijiaju.cn

[U48] PHP：纯枚举
来源：http://xs.asd995.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cc.asd995.cn

[U49] PHP：只读属性
来源：http://yh.hahajie.cn

public readonly string $name
来源：http://pu.chemitech.net.cn

[U50] PHP：构造器属性提升
来源：http://wc.asd995.cn

public function __construct(private int $id) {}
来源：http://fi.chemitech.net.cn

[U51] PHP：数组解构
来源：http://bf.shtwfgs.cn

[$a, $b] = $arr;
来源：http://qh.lnxyls.cn

[U52] PHP：箭头函数
来源：http://dd.jianghongdianzi.cn

$double = fn($x) => $x * 2;
来源：http://sj.haigaiapp.cn

[U53] PHP：空合并运算符
来源：http://mm.9csxet.cn

$v = $a ?? $b ?? "default";
来源：http://mx.asd995.cn

[U54] PHP：空安全调用
来源：http://wi.huanxung.cn

$obj?->method()
来源：http://zs.colortex.cn

[U55] PHP：match 表达式
来源：http://sw.shtwfgs.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zm.nicolike.cn

[U56] PHP：命名参数
来源：http://ft.yuntaijiaju.cn

f(a: 1, b: 2)
来源：http://he.bjjhwx.cn

[U57] PHP：字符串插值
来源：http://qc.jianghongdianzi.cn

"值: {$a}"
来源：http://wq.huixinmuqiang.cn

[U58] PHP：数组三件套
来源：http://lp.wgjwhj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gy.hnjuh.cn

[U59] PHP：自定义排序
来源：http://gb.chemitech.net.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hj.jianghongdianzi.cn

[U60] PHP：JSON 编解码
来源：http://oq.wgjwhj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ww.haigaiapp.cn

[U61] PHP：正则
来源：http://ch.yuntaijiaju.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ef.bjjhwx.cn

[U62] PHP：日期对象
来源：http://iu.szsharing.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://or.shtwfgs.cn

[U63] PHP：文件读写
来源：http://vm.muxihuayi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://to.chemitech.net.cn

[U64] PHP：目录遍历
来源：http://ag.huixiangedu.cn

glob("dir/*.php");  scandir("dir");
来源：http://yt.521024.cn

[U65] PHP：会话
来源：http://bt.szxytkj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ub.shtwfgs.cn

[U66] PHP：设置 Cookie
来源：http://sz.szsharing.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kf.yuexingan06.cn

[U67] PHP：处理文件上传
来源：http://ma.colortex.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bf.jctech888.com.cn

[U68] PHP：PDO 连接
来源：http://oe.jctech888.com.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hs.shxzskj.cn

[U69] PHP：PDO 预处理
来源：http://vl.szsharing.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://iu.nicolike.cn

[U70] PHP：PDO 事务
来源：http://fe.yuntaijiaju.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://oa.lnxyls.cn

[U71] PHP：抛出异常
来源：http://mb.jianghongdianzi.cn

throw new RuntimeException("失败", 500);
来源：http://lx.shxzukj.cn

[U72] PHP：写错误日志
来源：http://io.szxytkj.cn

error_log("失败: " . $e->getMessage());
来源：http://zo.shtwfgs.cn

[U73] PHP：读取 ini 配置
来源：http://wf.panjiajie.cn

parse_ini_file("config.ini", true)
来源：http://nh.asd995.cn

[U74] PHP：读取环境变量
来源：http://ov.muxihuayi.cn

getenv("APP_ENV") ?: "production"
来源：http://tn.nicolike.cn

[U75] PHP：依赖注入
来源：http://mv.hnjuh.cn

composer require psr/container
来源：http://sn.9csxet.cn

[U76] PHP：简单路由
来源：http://gr.wgjwhj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jz.hahajie.cn

[U77] PHP：模板渲染
来源：http://lz.chemitech.net.cn

composer require twig/twig
来源：http://ee.panjiajie.cn

[U78] PHP：单元测试
来源：http://et.muxihuayi.cn

composer require --dev phpunit/phpunit
来源：http://ek.yuntaijiaju.cn

[U79] PHP：静态分析
来源：http://bz.huixinmuqiang.cn

composer require --dev phpstan/phpstan
来源：http://kh.bookmarksfly.cn

[U80] PHP：代码规范修复
来源：http://mj.jctech888.com.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://rr.asd995.cn

[U81] JS：初始化项目
来源：http://ac.szxytkj.cn

npm init -y;  npm i express
来源：http://en.muxihuayi.cn

[U82] JS：package.json 脚本
来源：http://fd.hnjuh.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wa.huixiangedu.cn

[U83] JS：ES Module 导入导出
来源：http://yu.colortex.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ww.hnjuh.cn

[U84] JS：CommonJS 写法
来源：http://wt.huanxung.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ue.chemitech.net.cn

[U85] JS：可选链
来源：http://xa.newstarts.cn

a?.b?.c
来源：http://hn.jctech888.com.cn

[U86] JS：空值合并
来源：http://qg.shxzskj.cn

a ?? b
来源：http://sw.hnjuh.cn

[U87] JS：解构默认值
来源：http://gb.bjjhwx.cn

const { a = 1, b = 2 } = obj;
来源：http://cm.shtwfgs.cn

[U88] JS：对象展开合并
来源：http://hz.yuntaijiaju.cn

{ ...a, ...b }
来源：http://qp.newstarts.cn

[U89] JS：数组去重
来源：http://bl.nszjky.cn

[...new Set(arr)]
来源：http://ju.szsharing.cn

[U90] JS：数字数组排序
来源：http://yw.asd995.cn

[...arr].sort((a, b) => a - b)
来源：http://mn.hahajie.cn

[U91] JS：对象键值遍历
来源：http://ov.nicolike.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mf.nszjky.cn

[U92] JS：深拷贝
来源：http://ik.bjjhwx.cn

structuredClone(obj)
来源：http://es.haigaiapp.cn


<!-- 参考信息 -->