代发 wailian999

[T03] Kotlin：字符串模板
来源：http://hv.szsharing.cn

"值: $b"
来源：http://lv.colortex.cn

[T04] Kotlin：空安全
来源：http://eb.jctech888.com.cn

val n: String? = null;  n?.length
来源：http://xr.shxzskj.cn

[T05] Kotlin：when 表达式
来源：http://yi.muxihuayi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uo.shxzskj.cn

[T06] Kotlin：集合映射
来源：http://fz.huixiangedu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://nc.colortex.cn

[T07] Kotlin：集合过滤
来源：http://tb.521024.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://bv.newstarts.cn

[T08] Kotlin：数据类
来源：http://ps.szxytkj.cn

data class User(val name: String, val age: Int)
来源：http://tf.jctech888.com.cn

[T09] Kotlin：扩展函数
来源：http://iq.szxytkj.cn

fun String.exclaim() = this + "!"
来源：http://jz.bjjhwx.cn

[T10] Kotlin：默认参数
来源：http://zv.shxzskj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wp.szsharing.cn

[T11] Kotlin：协程
来源：http://bm.lnxyls.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bn.chemitech.net.cn

[T12] Kotlin：解构声明
来源：http://xd.bjjhwx.cn

val (a, b) = Pair(1, 2)
来源：http://ty.nicolike.cn

[T13] Kotlin：只读 Map
来源：http://sz.szxytkj.cn

val m = mapOf("a" to 1)
来源：http://as.hahajie.cn

[T14] Kotlin：循环
来源：http://ik.shxzukj.cn

for (i in 1..10) println(i)
来源：http://qi.chemitech.net.cn

[T15] Kotlin：接口
来源：http://rk.szxytkj.cn

interface Shape { fun area(): Double }
来源：http://ux.gzmigu.cn

[T16] Swift：Hello World
来源：http://ka.521024.cn

print("Hello")
来源：http://io.hahajie.cn

[T17] Swift：变量与常量
来源：http://sw.nicolike.cn

var a = 1;  let b = 2
来源：http://gc.521024.cn

[T18] Swift：字符串插值
来源：http://mv.yuntaijiaju.cn

"值: \(b)"
来源：http://pz.shxzukj.cn

[T19] Swift：可选绑定
来源：http://fg.nicolike.cn

if let n = opt { print(n) }
来源：http://iu.panjiajie.cn

[T20] Swift：数组操作
来源：http://qv.jianghongdianzi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://pl.lnxyls.cn

[T21] Swift：遍历
来源：http://oy.muxihuayi.cn

for x in a { print(x) }
来源：http://ic.huixinmuqiang.cn

[T22] Swift：字典
来源：http://yq.bookmarksfly.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ro.asd995.cn

[T23] Swift：函数
来源：http://ij.jctech888.com.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lm.jctech888.com.cn

[T24] Swift：闭包
来源：http://zf.lnxyls.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://yu.huixiangedu.cn

[T25] Swift：结构体
来源：http://hc.jianghongdianzi.cn

struct P { var x: Int }
来源：http://ur.jctech888.com.cn

[T26] Swift：类与重写
来源：http://fj.huanxung.cn

class A: Base { override func f() {} }
来源：http://yl.521024.cn

[T27] Swift：错误处理
来源：http://za.lnxyls.cn

do { try f() } catch { print(error) }
来源：http://jd.colortex.cn

[T28] Swift：枚举
来源：http://zg.newstarts.cn

enum Color { case red, green }
来源：http://ea.szxytkj.cn

[T29] Swift：guard 提前返回
来源：http://pn.chemitech.net.cn

guard let x = opt else { return }
来源：http://mm.szsharing.cn

[T30] Swift：协议
来源：http://kg.panjiajie.cn

protocol Shape { func area() -> Double }
来源：http://wa.shxzukj.cn

[T31] Lua：Hello World
来源：http://vx.muxihuayi.cn

print("Hello")
来源：http://bd.yuntaijiaju.cn

[T32] Lua：局部变量
来源：http://ub.9csxet.cn

local a = 1
来源：http://et.panjiajie.cn

[T33] Lua：表（数组）
来源：http://yd.nszjky.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://nu.panjiajie.cn

[T34] Lua：遍历表
来源：http://zc.szxytkj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://kw.nicolike.cn

[T35] Lua：字典表
来源：http://cm.szxytkj.cn

local d = { a = 1 };  d.b = 2
来源：http://tv.huanxung.cn

[T36] Lua：函数
来源：http://zz.shtwfgs.cn

function add(a, b) return a + b end
来源：http://up.jianghongdianzi.cn

[T37] Lua：字符串拼接
来源：http://yq.jianghongdianzi.cn

"a" .. "b"
来源：http://kv.huixinmuqiang.cn

[T38] Lua：条件
来源：http://kb.hnjuh.cn

if x > 0 then print("正") end
来源：http://ob.shtwfgs.cn

[T39] Lua：模式匹配
来源：http://xl.lnxyls.cn

string.find(s, "%d+")
来源：http://kf.shtwfgs.cn

[T40] Lua：元表
来源：http://ar.yuntaijiaju.cn

setmetatable({}, { __index = base })
来源：http://dl.bjjhwx.cn

[T41] Perl：Hello World
来源：http://cw.huixinmuqiang.cn

print "Hello\n";
来源：http://yg.wgjwhj.cn

[T42] Perl：变量类型
来源：http://qc.nicolike.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wh.jianghongdianzi.cn

[T43] Perl：字符串插值
来源：http://kk.haigaiapp.cn

"值: $a"
来源：http://ls.hahajie.cn

[T44] Perl：条件
来源：http://qv.colortex.cn

if ($a > 0) { print "正"; }
来源：http://im.gzmigu.cn

[T45] Perl：数组遍历
来源：http://cd.shtwfgs.cn

for my $x (@arr) { print $x; }
来源：http://rm.huixinmuqiang.cn

[T46] Perl：哈希操作
来源：http://eq.nicolike.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://at.muxihuayi.cn

[T47] Perl：正则捕获
来源：http://og.shxzskj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rw.panjiajie.cn

[T48] Perl：正则替换
来源：http://hq.jctech888.com.cn

$s =~ s/old/new/g;
来源：http://at.9csxet.cn

[T49] Perl：函数
来源：http://fp.hnjuh.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sh.nszjky.cn

[T50] Perl：逐行读文件
来源：http://gl.newstarts.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://dz.colortex.cn

while (my $line = <$fh>) { print $line; }
来源：http://rr.9csxet.cn

[T51] Scala：Hello World
来源：http://he.panjiajie.cn

println("Hello")
来源：http://hq.yuntaijiaju.cn

[T52] Scala：变量
来源：http://zh.szsharing.cn

val a = 1;  var b = 2
来源：http://dc.nicolike.cn

[T53] Scala：字符串插值
来源：http://qd.yuntaijiaju.cn

s"值: $b"
来源：http://ny.gzmigu.cn

[T54] Scala：集合映射
来源：http://dl.chemitech.net.cn

List(1, 2, 3).map(_ * 2)
来源：http://ud.haigaiapp.cn

[T55] Scala：集合过滤
来源：http://jn.newstarts.cn

List(1, 2, 3).filter(_ > 1)
来源：http://mu.bjjhwx.cn

[T56] Scala：样例类
来源：http://wn.szsharing.cn

case class User(name: String, age: Int)
来源：http://xq.huixiangedu.cn

[T57] Scala：模式匹配
来源：http://wo.asd995.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://hx.shtwfgs.cn

[T58] Scala：函数定义
来源：http://mw.nszjky.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zx.newstarts.cn

[T59] Scala：循环
来源：http://fr.wgjwhj.cn

for (i <- 1 to 10) println(i)
来源：http://kr.huixinmuqiang.cn

[T60] Scala：折叠
来源：http://mg.szxytkj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rt.szsharing.cn

================================================================================
来源：http://rk.panjiajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://si.nicolike.cn

================================================================================
来源：http://ss.shtwfgs.cn

[U01] Py：创建虚拟环境
来源：http://km.szxytkj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ig.yuexingan06.cn

[U02] Py：导出 / 安装依赖
来源：http://yz.gzmigu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bh.hahajie.cn

[U03] Py：加载 .env 配置
来源：http://xy.haigaiapp.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://me.nicolike.cn

[U04] Py：变量调试打印
来源：http://az.shxzskj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://yr.panjiajie.cn

[U05] Py：列表去重且保序
来源：http://jc.bookmarksfly.cn

list(dict.fromkeys(arr))
来源：http://ab.gzmigu.cn

[U06] Py：合并两个字典
来源：http://yf.bookmarksfly.cn

{**a, **b}
来源：http://ca.szxytkj.cn

[U07] Py：反转字典键值
来源：http://qz.huixiangedu.cn

{v: k for k, v in d.items()}
来源：http://wk.yuexingan06.cn

[U08] Py：展平二维列表
来源：http://lh.yuexingan06.cn

[y for x in nested for y in x]
来源：http://mt.szsharing.cn

[U09] Py：字典取最大值的键
来源：http://jp.lnxyls.cn

max(d, key=d.get)
来源：http://jq.chemitech.net.cn

[U10] Py：按值排序字典
来源：http://zz.colortex.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bf.huanxung.cn

[U11] Py：生成器表达式
来源：http://xv.521024.cn

(x * 2 for x in arr)
来源：http://cs.nszjky.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zg.bjjhwx.cn

Counter(arr).most_common(3)
来源：http://ct.szsharing.cn

[U13] Py：固定长度队列
来源：http://ql.shxzukj.cn

deque(maxlen=10)
来源：http://jr.9csxet.cn

[U14] Py：分组收集到列表
来源：http://lt.shxzskj.cn

defaultdict(list)
来源：http://jp.nszjky.cn

[U15] Py：高精度计时
来源：http://rl.panjiajie.cn

t = time.perf_counter()
来源：http://tu.newstarts.cn

[U16] Py：命令行参数解析
来源：http://ow.jianghongdianzi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://to.wgjwhj.cn

[U17] Py：初始化日志
来源：http://qh.shxzukj.cn

logging.basicConfig(level=logging.INFO)
来源：http://wb.jianghongdianzi.cn

[U18] Py：预编译正则
来源：http://ix.muxihuayi.cn

pat = re.compile(r"\d+")
来源：http://gb.shxzukj.cn

[U19] Py：正则替换带回调
来源：http://ud.wgjwhj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kr.panjiajie.cn

[U20] Py：缓存函数结果
来源：http://er.chemitech.net.cn

@functools.lru_cache(maxsize=None)
来源：http://gd.hahajie.cn

[U21] Py：自定义上下文管理器
来源：http://id.nszjky.cn

@contextlib.contextmanager
来源：http://mj.chemitech.net.cn

[U22] Py：矩阵转置
来源：http://wa.shxzskj.cn

list(zip(*m))
来源：http://kg.szsharing.cn

[U23] Py：分块读取大文件
来源：http://ym.shxzukj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lp.szsharing.cn

[U24] Py：路径操作
来源：http://tj.huixinmuqiang.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gj.panjiajie.cn

[U25] Py：CSV 按字典读
来源：http://oc.muxihuayi.cn

csv.DictReader(f)
来源：http://pw.yuntaijiaju.cn

[U26] Py：并发下载
来源：http://si.wgjwhj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://oy.shtwfgs.cn

[U27] Py：异步 HTTP
来源：http://xv.haigaiapp.cn

aiohttp.ClientSession() 配合 async with
来源：http://pl.haigaiapp.cn

[U28] Py：类型别名
来源：http://iv.bjjhwx.cn

UserId = int
来源：http://ku.shtwfgs.cn

[U29] Py：属性校验
来源：http://xd.yuexingan06.cn

@property 与 @x.setter 配合
来源：http://zk.jctech888.com.cn

[U30] Py：数据类
来源：http://op.9csxet.cn

@dataclass(slots=True)
来源：http://da.hnjuh.cn

[U31] Py：单测
来源：http://gc.yuntaijiaju.cn

python -m pytest -q
来源：http://ut.colortex.cn

[U32] Py：代码格式化
来源：http://gn.huixiangedu.cn

ruff format . && ruff check --fix .
来源：http://kd.muxihuayi.cn

[U33] Py：打包发布
来源：http://fw.shtwfgs.cn

python -m build  （依赖 pyproject.toml）
来源：http://xl.newstarts.cn

[U34] Py：判断编码
来源：http://cp.haigaiapp.cn

chardet.detect(raw)
来源：http://ha.9csxet.cn

[U35] Py：发送邮件
来源：http://ic.chemitech.net.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xj.muxihuayi.cn

[U36] Py：定时任务
来源：http://kt.shxzskj.cn

schedule.every(10).minutes.do(job)
来源：http://ew.jianghongdianzi.cn

[U37] Py：读写 Excel
来源：http://dq.panjiajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://hm.521024.cn

[U38] Py：获取脚本所在目录
来源：http://gw.521024.cn

Path(__file__).resolve().parent
来源：http://tp.hahajie.cn

[U39] Py：判断是否在交互环境
来源：http://ym.gzmigu.cn

sys.stdout.isatty()
来源：http://ck.szsharing.cn

[U40] Py：打印到标准错误
来源：http://lf.huixinmuqiang.cn

print("err", file=sys.stderr)
来源：http://un.huixinmuqiang.cn

[U41] PHP：初始化 Composer 项目
来源：http://zd.shxzukj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ip.szxytkj.cn

[U42] PHP：PSR-4 自动加载
来源：http://nm.hahajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zd.szsharing.cn

[U43] PHP：声明命名空间
来源：http://qy.gzmigu.cn

namespace App\Http;
来源：http://qf.huixiangedu.cn

[U44] PHP：开启严格类型
来源：http://rt.521024.cn

declare(strict_types=1);
来源：http://qg.yuntaijiaju.cn

[U45] PHP：类型声明与返回类型
来源：http://tt.yuntaijiaju.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://mq.huixiangedu.cn

[U46] PHP：可空类型
来源：http://xd.jianghongdianzi.cn

?string $name = null
来源：http://hg.hahajie.cn

[U47] PHP：联合类型
来源：http://rr.colortex.cn

int|string $id
来源：http://wl.shtwfgs.cn

[U48] PHP：纯枚举
来源：http://at.nszjky.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jm.nszjky.cn

[U49] PHP：只读属性
来源：http://op.chemitech.net.cn

public readonly string $name
来源：http://ju.panjiajie.cn

[U50] PHP：构造器属性提升
来源：http://jt.jianghongdianzi.cn

public function __construct(private int $id) {}
来源：http://sb.haigaiapp.cn

[U51] PHP：数组解构
来源：http://ti.9csxet.cn

[$a, $b] = $arr;
来源：http://qx.bjjhwx.cn

[U52] PHP：箭头函数
来源：http://mk.haigaiapp.cn

$double = fn($x) => $x * 2;
来源：http://zg.panjiajie.cn

[U53] PHP：空合并运算符
来源：http://ir.hahajie.cn

$v = $a ?? $b ?? "default";
来源：http://zj.hnjuh.cn

[U54] PHP：空安全调用
来源：http://cs.shxzukj.cn

$obj?->method()
来源：http://np.nszjky.cn

[U55] PHP：match 表达式
来源：http://zz.newstarts.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cx.gzmigu.cn

[U56] PHP：命名参数
来源：http://ic.9csxet.cn

f(a: 1, b: 2)
来源：http://ca.jctech888.com.cn

[U57] PHP：字符串插值
来源：http://lq.muxihuayi.cn

"值: {$a}"
来源：http://gg.nszjky.cn

[U58] PHP：数组三件套
来源：http://xl.wgjwhj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jl.szsharing.cn

[U59] PHP：自定义排序
来源：http://he.huixiangedu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ei.shxzskj.cn

[U60] PHP：JSON 编解码
来源：http://tj.9csxet.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://md.hnjuh.cn

[U61] PHP：正则
来源：http://wg.nicolike.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bw.nszjky.cn

[U62] PHP：日期对象
来源：http://vb.muxihuayi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mz.9csxet.cn

[U63] PHP：文件读写
来源：http://ev.haigaiapp.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zn.huixiangedu.cn

[U64] PHP：目录遍历
来源：http://qx.nszjky.cn

glob("dir/*.php");  scandir("dir");
来源：http://lk.szsharing.cn

[U65] PHP：会话
来源：http://re.nicolike.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://bx.shxzukj.cn

[U66] PHP：设置 Cookie
来源：http://kq.nicolike.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sq.nszjky.cn

[U67] PHP：处理文件上传
来源：http://nu.hahajie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fp.shxzukj.cn

[U68] PHP：PDO 连接
来源：http://vi.huixinmuqiang.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jx.panjiajie.cn

[U69] PHP：PDO 预处理
来源：http://yj.huixiangedu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dw.bookmarksfly.cn

[U70] PHP：PDO 事务
来源：http://dv.nicolike.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zx.521024.cn

[U71] PHP：抛出异常
来源：http://mz.nszjky.cn

throw new RuntimeException("失败", 500);
来源：http://em.jctech888.com.cn

[U72] PHP：写错误日志
来源：http://nt.nszjky.cn

error_log("失败: " . $e->getMessage());
来源：http://ip.colortex.cn

[U73] PHP：读取 ini 配置
来源：http://gw.huixinmuqiang.cn

parse_ini_file("config.ini", true)
来源：http://un.521024.cn

[U74] PHP：读取环境变量
来源：http://od.yuntaijiaju.cn

getenv("APP_ENV") ?: "production"
来源：http://mg.huixiangedu.cn

[U75] PHP：依赖注入
来源：http://wd.lnxyls.cn

composer require psr/container
来源：http://jd.9csxet.cn

[U76] PHP：简单路由
来源：http://cy.wgjwhj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://im.asd995.cn

[U77] PHP：模板渲染
来源：http://ux.huixinmuqiang.cn

composer require twig/twig
来源：http://fr.huixinmuqiang.cn

[U78] PHP：单元测试
来源：http://er.huanxung.cn

composer require --dev phpunit/phpunit
来源：http://dr.colortex.cn

[U79] PHP：静态分析
来源：http://yu.yuexingan06.cn

composer require --dev phpstan/phpstan
来源：http://vq.chemitech.net.cn

[U80] PHP：代码规范修复
来源：http://mm.yuexingan06.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jg.9csxet.cn

[U81] JS：初始化项目
来源：http://rz.lnxyls.cn

npm init -y;  npm i express
来源：http://os.bookmarksfly.cn

[U82] JS：package.json 脚本
来源：http://bd.hnjuh.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fj.chemitech.net.cn

[U83] JS：ES Module 导入导出
来源：http://ur.gzmigu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://du.wgjwhj.cn

[U84] JS：CommonJS 写法
来源：http://fg.muxihuayi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://cy.asd995.cn

[U85] JS：可选链
来源：http://iz.shxzukj.cn

a?.b?.c
来源：http://qq.nszjky.cn

[U86] JS：空值合并
来源：http://ic.hahajie.cn

a ?? b
来源：http://da.haigaiapp.cn

[U87] JS：解构默认值
来源：http://na.hnjuh.cn

const { a = 1, b = 2 } = obj;
来源：http://qf.wgjwhj.cn

[U88] JS：对象展开合并
来源：http://pk.521024.cn

{ ...a, ...b }
来源：http://xo.panjiajie.cn

[U89] JS：数组去重
来源：http://bq.huixiangedu.cn

[...new Set(arr)]
来源：http://es.chemitech.net.cn

[U90] JS：数字数组排序
来源：http://bq.lnxyls.cn

[...arr].sort((a, b) => a - b)
来源：http://mp.muxihuayi.cn


<!-- 参考信息 -->