代发 wailian999

[T01] Kotlin：Hello World
来源：http://xx.szsharing.cn

println("Hello")
来源：http://gv.jctech888.com.cn

[T02] Kotlin：变量
来源：http://iu.lnxyls.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kd.hnjuh.cn

[T03] Kotlin：字符串模板
来源：http://eu.szsharing.cn

"值: $b"
来源：http://to.jctech888.com.cn

[T04] Kotlin：空安全
来源：http://uf.jianghongdianzi.cn

val n: String? = null;  n?.length
来源：http://nf.chemitech.net.cn

[T05] Kotlin：when 表达式
来源：http://xw.hahajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://va.nicolike.cn

[T06] Kotlin：集合映射
来源：http://xc.jctech888.com.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ey.huanxung.cn

[T07] Kotlin：集合过滤
来源：http://ye.jctech888.com.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pa.lnxyls.cn

[T08] Kotlin：数据类
来源：http://lt.yuexingan06.cn

data class User(val name: String, val age: Int)
来源：http://is.huixinmuqiang.cn

[T09] Kotlin：扩展函数
来源：http://lo.huanxung.cn

fun String.exclaim() = this + "!"
来源：http://ti.muxihuayi.cn

[T10] Kotlin：默认参数
来源：http://yx.9csxet.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ra.panjiajie.cn

[T11] Kotlin：协程
来源：http://ep.shtwfgs.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vo.hnjuh.cn

[T12] Kotlin：解构声明
来源：http://ob.wgjwhj.cn

val (a, b) = Pair(1, 2)
来源：http://fn.lnxyls.cn

[T13] Kotlin：只读 Map
来源：http://bb.yuntaijiaju.cn

val m = mapOf("a" to 1)
来源：http://tk.shxzukj.cn

[T14] Kotlin：循环
来源：http://vk.panjiajie.cn

for (i in 1..10) println(i)
来源：http://wa.panjiajie.cn

[T15] Kotlin：接口
来源：http://lh.haigaiapp.cn

interface Shape { fun area(): Double }
来源：http://ia.bookmarksfly.cn

[T16] Swift：Hello World
来源：http://pe.shxzskj.cn

print("Hello")
来源：http://qu.hahajie.cn

[T17] Swift：变量与常量
来源：http://kx.asd995.cn

var a = 1;  let b = 2
来源：http://il.jianghongdianzi.cn

[T18] Swift：字符串插值
来源：http://ur.colortex.cn

"值: \(b)"
来源：http://vl.szxytkj.cn

[T19] Swift：可选绑定
来源：http://mm.newstarts.cn

if let n = opt { print(n) }
来源：http://pp.bjjhwx.cn

[T20] Swift：数组操作
来源：http://dm.yuexingan06.cn

var a = [1, 2, 3];  a.append(4)
来源：http://cx.szsharing.cn

[T21] Swift：遍历
来源：http://au.muxihuayi.cn

for x in a { print(x) }
来源：http://hu.wgjwhj.cn

[T22] Swift：字典
来源：http://oh.jianghongdianzi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://qx.bjjhwx.cn

[T23] Swift：函数
来源：http://va.shtwfgs.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ob.chemitech.net.cn

[T24] Swift：闭包
来源：http://sz.shtwfgs.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://wu.huixiangedu.cn

[T25] Swift：结构体
来源：http://ua.shxzukj.cn

struct P { var x: Int }
来源：http://rv.asd995.cn

[T26] Swift：类与重写
来源：http://fr.chemitech.net.cn

class A: Base { override func f() {} }
来源：http://gh.9csxet.cn

[T27] Swift：错误处理
来源：http://fd.shtwfgs.cn

do { try f() } catch { print(error) }
来源：http://au.asd995.cn

[T28] Swift：枚举
来源：http://rc.shxzukj.cn

enum Color { case red, green }
来源：http://se.bookmarksfly.cn

[T29] Swift：guard 提前返回
来源：http://do.asd995.cn

guard let x = opt else { return }
来源：http://yt.jianghongdianzi.cn

[T30] Swift：协议
来源：http://qt.szxytkj.cn

protocol Shape { func area() -> Double }
来源：http://vc.bookmarksfly.cn

[T31] Lua：Hello World
来源：http://zh.shtwfgs.cn

print("Hello")
来源：http://ax.szxytkj.cn

[T32] Lua：局部变量
来源：http://jl.521024.cn

local a = 1
来源：http://ko.szsharing.cn

[T33] Lua：表（数组）
来源：http://kc.nszjky.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ap.521024.cn

[T34] Lua：遍历表
来源：http://ar.bjjhwx.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qf.newstarts.cn

[T35] Lua：字典表
来源：http://wt.lnxyls.cn

local d = { a = 1 };  d.b = 2
来源：http://dd.jianghongdianzi.cn

[T36] Lua：函数
来源：http://wc.huixinmuqiang.cn

function add(a, b) return a + b end
来源：http://fz.haigaiapp.cn

[T37] Lua：字符串拼接
来源：http://xt.hnjuh.cn

"a" .. "b"
来源：http://zx.haigaiapp.cn

[T38] Lua：条件
来源：http://mo.nszjky.cn

if x > 0 then print("正") end
来源：http://ja.yuntaijiaju.cn

[T39] Lua：模式匹配
来源：http://mn.asd995.cn

string.find(s, "%d+")
来源：http://bo.shxzukj.cn

[T40] Lua：元表
来源：http://vh.shxzskj.cn

setmetatable({}, { __index = base })
来源：http://hu.nszjky.cn

[T41] Perl：Hello World
来源：http://xr.muxihuayi.cn

print "Hello\n";
来源：http://cz.yuntaijiaju.cn

[T42] Perl：变量类型
来源：http://wp.bjjhwx.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ww.yuntaijiaju.cn

[T43] Perl：字符串插值
来源：http://kn.shxzskj.cn

"值: $a"
来源：http://dc.gzmigu.cn

[T44] Perl：条件
来源：http://sb.521024.cn

if ($a > 0) { print "正"; }
来源：http://ek.nicolike.cn

[T45] Perl：数组遍历
来源：http://cj.lnxyls.cn

for my $x (@arr) { print $x; }
来源：http://ds.wgjwhj.cn

[T46] Perl：哈希操作
来源：http://ut.colortex.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nw.shtwfgs.cn

[T47] Perl：正则捕获
来源：http://dq.szsharing.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ul.szsharing.cn

[T48] Perl：正则替换
来源：http://gv.nicolike.cn

$s =~ s/old/new/g;
来源：http://de.yuntaijiaju.cn

[T49] Perl：函数
来源：http://tu.yuexingan06.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://me.asd995.cn

[T50] Perl：逐行读文件
来源：http://lq.muxihuayi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://mr.chemitech.net.cn

while (my $line = <$fh>) { print $line; }
来源：http://qz.bookmarksfly.cn

[T51] Scala：Hello World
来源：http://vc.colortex.cn

println("Hello")
来源：http://or.huixiangedu.cn

[T52] Scala：变量
来源：http://jj.szsharing.cn

val a = 1;  var b = 2
来源：http://rp.521024.cn

[T53] Scala：字符串插值
来源：http://nk.colortex.cn

s"值: $b"
来源：http://uz.newstarts.cn

[T54] Scala：集合映射
来源：http://eu.shxzskj.cn

List(1, 2, 3).map(_ * 2)
来源：http://ac.bjjhwx.cn

[T55] Scala：集合过滤
来源：http://tf.huixinmuqiang.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ar.shtwfgs.cn

[T56] Scala：样例类
来源：http://lm.521024.cn

case class User(name: String, age: Int)
来源：http://uw.newstarts.cn

[T57] Scala：模式匹配
来源：http://mj.shxzukj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fc.521024.cn

[T58] Scala：函数定义
来源：http://nn.gzmigu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://qy.shxzukj.cn

[T59] Scala：循环
来源：http://di.shxzskj.cn

for (i <- 1 to 10) println(i)
来源：http://oy.521024.cn

[T60] Scala：折叠
来源：http://cb.hahajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dy.yuexingan06.cn

================================================================================
来源：http://oq.asd995.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ek.szxytkj.cn

================================================================================
来源：http://kq.9csxet.cn

[U01] Py：创建虚拟环境
来源：http://et.hahajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://lq.gzmigu.cn

[U02] Py：导出 / 安装依赖
来源：http://wb.huixiangedu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zj.yuntaijiaju.cn

[U03] Py：加载 .env 配置
来源：http://uo.shxzukj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://sz.521024.cn

[U04] Py：变量调试打印
来源：http://gm.szxytkj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qr.colortex.cn

[U05] Py：列表去重且保序
来源：http://dp.521024.cn

list(dict.fromkeys(arr))
来源：http://nf.haigaiapp.cn

[U06] Py：合并两个字典
来源：http://iw.chemitech.net.cn

{**a, **b}
来源：http://sj.jianghongdianzi.cn

[U07] Py：反转字典键值
来源：http://du.newstarts.cn

{v: k for k, v in d.items()}
来源：http://rw.shxzskj.cn

[U08] Py：展平二维列表
来源：http://jp.shxzskj.cn

[y for x in nested for y in x]
来源：http://ju.huanxung.cn

[U09] Py：字典取最大值的键
来源：http://sg.gzmigu.cn

max(d, key=d.get)
来源：http://ni.panjiajie.cn

[U10] Py：按值排序字典
来源：http://sh.521024.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nj.wgjwhj.cn

[U11] Py：生成器表达式
来源：http://dp.bookmarksfly.cn

(x * 2 for x in arr)
来源：http://oy.521024.cn

[U12] Py：取出现最多的 3 个元素
来源：http://eq.shxzukj.cn

Counter(arr).most_common(3)
来源：http://nn.shtwfgs.cn

[U13] Py：固定长度队列
来源：http://cj.wgjwhj.cn

deque(maxlen=10)
来源：http://zi.haigaiapp.cn

[U14] Py：分组收集到列表
来源：http://sw.hnjuh.cn

defaultdict(list)
来源：http://kg.asd995.cn

[U15] Py：高精度计时
来源：http://jj.yuexingan06.cn

t = time.perf_counter()
来源：http://ok.bookmarksfly.cn

[U16] Py：命令行参数解析
来源：http://rg.muxihuayi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ff.muxihuayi.cn

[U17] Py：初始化日志
来源：http://vo.gzmigu.cn

logging.basicConfig(level=logging.INFO)
来源：http://eh.chemitech.net.cn

[U18] Py：预编译正则
来源：http://og.huanxung.cn

pat = re.compile(r"\d+")
来源：http://ny.huixinmuqiang.cn

[U19] Py：正则替换带回调
来源：http://tt.asd995.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vh.huanxung.cn

[U20] Py：缓存函数结果
来源：http://vo.jianghongdianzi.cn

@functools.lru_cache(maxsize=None)
来源：http://lx.nszjky.cn

[U21] Py：自定义上下文管理器
来源：http://ji.chemitech.net.cn

@contextlib.contextmanager
来源：http://km.huixiangedu.cn

[U22] Py：矩阵转置
来源：http://di.huixinmuqiang.cn

list(zip(*m))
来源：http://hp.huixinmuqiang.cn

[U23] Py：分块读取大文件
来源：http://jd.9csxet.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dl.hnjuh.cn

[U24] Py：路径操作
来源：http://yk.nicolike.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xx.panjiajie.cn

[U25] Py：CSV 按字典读
来源：http://iy.muxihuayi.cn

csv.DictReader(f)
来源：http://ij.szsharing.cn

[U26] Py：并发下载
来源：http://wx.hahajie.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zi.szxytkj.cn

[U27] Py：异步 HTTP
来源：http://dr.szxytkj.cn

aiohttp.ClientSession() 配合 async with
来源：http://dc.asd995.cn

[U28] Py：类型别名
来源：http://ld.gzmigu.cn

UserId = int
来源：http://ve.bjjhwx.cn

[U29] Py：属性校验
来源：http://pk.lnxyls.cn

@property 与 @x.setter 配合
来源：http://eo.shxzskj.cn

[U30] Py：数据类
来源：http://od.chemitech.net.cn

@dataclass(slots=True)
来源：http://bn.chemitech.net.cn

[U31] Py：单测
来源：http://ih.9csxet.cn

python -m pytest -q
来源：http://ao.huixinmuqiang.cn

[U32] Py：代码格式化
来源：http://pg.shxzukj.cn

ruff format . && ruff check --fix .
来源：http://rj.colortex.cn

[U33] Py：打包发布
来源：http://te.huixinmuqiang.cn

python -m build  （依赖 pyproject.toml）
来源：http://pe.muxihuayi.cn

[U34] Py：判断编码
来源：http://fh.hnjuh.cn

chardet.detect(raw)
来源：http://qd.hnjuh.cn

[U35] Py：发送邮件
来源：http://bg.huanxung.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fb.asd995.cn

[U36] Py：定时任务
来源：http://ki.gzmigu.cn

schedule.every(10).minutes.do(job)
来源：http://nb.bookmarksfly.cn

[U37] Py：读写 Excel
来源：http://kg.521024.cn

pandas.read_excel / DataFrame.to_excel
来源：http://eh.nszjky.cn

[U38] Py：获取脚本所在目录
来源：http://sx.hahajie.cn

Path(__file__).resolve().parent
来源：http://cs.9csxet.cn

[U39] Py：判断是否在交互环境
来源：http://rp.szsharing.cn

sys.stdout.isatty()
来源：http://ke.nszjky.cn

[U40] Py：打印到标准错误
来源：http://qh.huixinmuqiang.cn

print("err", file=sys.stderr)
来源：http://kl.chemitech.net.cn

[U41] PHP：初始化 Composer 项目
来源：http://bb.nszjky.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://hf.yuntaijiaju.cn

[U42] PHP：PSR-4 自动加载
来源：http://nd.hnjuh.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rs.wgjwhj.cn

[U43] PHP：声明命名空间
来源：http://mc.hahajie.cn

namespace App\Http;
来源：http://ap.nszjky.cn

[U44] PHP：开启严格类型
来源：http://cc.nszjky.cn

declare(strict_types=1);
来源：http://yw.gzmigu.cn

[U45] PHP：类型声明与返回类型
来源：http://yg.wgjwhj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://sx.nicolike.cn

[U46] PHP：可空类型
来源：http://qb.huixinmuqiang.cn

?string $name = null
来源：http://uc.yuexingan06.cn

[U47] PHP：联合类型
来源：http://yf.panjiajie.cn

int|string $id
来源：http://gc.huixinmuqiang.cn

[U48] PHP：纯枚举
来源：http://ne.newstarts.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ty.shxzskj.cn

[U49] PHP：只读属性
来源：http://ds.nszjky.cn

public readonly string $name
来源：http://zb.bjjhwx.cn

[U50] PHP：构造器属性提升
来源：http://rs.shtwfgs.cn

public function __construct(private int $id) {}
来源：http://je.szsharing.cn

[U51] PHP：数组解构
来源：http://ro.yuntaijiaju.cn

[$a, $b] = $arr;
来源：http://pz.gzmigu.cn

[U52] PHP：箭头函数
来源：http://ql.huixinmuqiang.cn

$double = fn($x) => $x * 2;
来源：http://nw.szsharing.cn

[U53] PHP：空合并运算符
来源：http://gi.haigaiapp.cn

$v = $a ?? $b ?? "default";
来源：http://un.jianghongdianzi.cn

[U54] PHP：空安全调用
来源：http://pk.huanxung.cn

$obj?->method()
来源：http://pt.jctech888.com.cn

[U55] PHP：match 表达式
来源：http://by.nszjky.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xe.szxytkj.cn

[U56] PHP：命名参数
来源：http://aj.gzmigu.cn

f(a: 1, b: 2)
来源：http://ye.shxzukj.cn

[U57] PHP：字符串插值
来源：http://ou.huixinmuqiang.cn

"值: {$a}"
来源：http://jf.szxytkj.cn

[U58] PHP：数组三件套
来源：http://sn.nszjky.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jm.szxytkj.cn

[U59] PHP：自定义排序
来源：http://cg.9csxet.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zu.shxzskj.cn

[U60] PHP：JSON 编解码
来源：http://sf.szxytkj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rp.nszjky.cn

[U61] PHP：正则
来源：http://ze.yuexingan06.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gm.shtwfgs.cn

[U62] PHP：日期对象
来源：http://ub.wgjwhj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cu.jctech888.com.cn

[U63] PHP：文件读写
来源：http://bh.huanxung.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bj.chemitech.net.cn

[U64] PHP：目录遍历
来源：http://uf.newstarts.cn

glob("dir/*.php");  scandir("dir");
来源：http://nr.gzmigu.cn

[U65] PHP：会话
来源：http://fd.wgjwhj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ke.bjjhwx.cn

[U66] PHP：设置 Cookie
来源：http://ex.nicolike.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mn.nicolike.cn

[U67] PHP：处理文件上传
来源：http://hl.szxytkj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bx.bjjhwx.cn

[U68] PHP：PDO 连接
来源：http://lz.wgjwhj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gf.jctech888.com.cn

[U69] PHP：PDO 预处理
来源：http://vg.chemitech.net.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ka.huanxung.cn

[U70] PHP：PDO 事务
来源：http://ai.nicolike.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wx.bookmarksfly.cn

[U71] PHP：抛出异常
来源：http://lh.haigaiapp.cn

throw new RuntimeException("失败", 500);
来源：http://eh.asd995.cn

[U72] PHP：写错误日志
来源：http://bh.yuntaijiaju.cn

error_log("失败: " . $e->getMessage());
来源：http://rm.chemitech.net.cn

[U73] PHP：读取 ini 配置
来源：http://va.nicolike.cn

parse_ini_file("config.ini", true)
来源：http://qu.yuexingan06.cn

[U74] PHP：读取环境变量
来源：http://vw.huixiangedu.cn

getenv("APP_ENV") ?: "production"
来源：http://tk.lnxyls.cn

[U75] PHP：依赖注入
来源：http://yc.521024.cn

composer require psr/container
来源：http://nv.yuntaijiaju.cn

[U76] PHP：简单路由
来源：http://tn.szxytkj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ef.jctech888.com.cn

[U77] PHP：模板渲染
来源：http://tm.yuntaijiaju.cn

composer require twig/twig
来源：http://zr.shxzskj.cn

[U78] PHP：单元测试
来源：http://to.jctech888.com.cn

composer require --dev phpunit/phpunit
来源：http://vj.gzmigu.cn

[U79] PHP：静态分析
来源：http://ck.bjjhwx.cn

composer require --dev phpstan/phpstan
来源：http://iy.wgjwhj.cn

[U80] PHP：代码规范修复
来源：http://tj.yuntaijiaju.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://hu.521024.cn

[U81] JS：初始化项目
来源：http://lc.shtwfgs.cn

npm init -y;  npm i express
来源：http://rz.newstarts.cn

[U82] JS：package.json 脚本
来源：http://ew.nszjky.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bh.szsharing.cn

[U83] JS：ES Module 导入导出
来源：http://qk.yuntaijiaju.cn

export const a = 1;  import { a } from "./m.js";
来源：http://il.huixiangedu.cn

[U84] JS：CommonJS 写法
来源：http://uc.asd995.cn

module.exports = { a };  const { a } = require("./m");
来源：http://fg.szsharing.cn

[U85] JS：可选链
来源：http://py.yuexingan06.cn

a?.b?.c
来源：http://vq.szxytkj.cn

[U86] JS：空值合并
来源：http://br.huanxung.cn

a ?? b
来源：http://tx.huixinmuqiang.cn

[U87] JS：解构默认值
来源：http://ec.huanxung.cn

const { a = 1, b = 2 } = obj;
来源：http://dh.jianghongdianzi.cn

[U88] JS：对象展开合并
来源：http://zy.newstarts.cn

{ ...a, ...b }
来源：http://kt.bjjhwx.cn


<!-- 参考信息 -->