代发 wailian999

[T01] Kotlin：Hello World
来源：http://zt.shxzskj.cn

println("Hello")
来源：http://xz.yuntaijiaju.cn

[T02] Kotlin：变量
来源：http://gf.shtwfgs.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gm.panjiajie.cn

[T03] Kotlin：字符串模板
来源：http://ii.huixiangedu.cn

"值: $b"
来源：http://em.shxzskj.cn

[T04] Kotlin：空安全
来源：http://fb.shtwfgs.cn

val n: String? = null;  n?.length
来源：http://dm.newstarts.cn

[T05] Kotlin：when 表达式
来源：http://aq.szsharing.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vx.gzmigu.cn

[T06] Kotlin：集合映射
来源：http://kf.colortex.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ff.wgjwhj.cn

[T07] Kotlin：集合过滤
来源：http://zs.haigaiapp.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ip.huanxung.cn

[T08] Kotlin：数据类
来源：http://ii.jianghongdianzi.cn

data class User(val name: String, val age: Int)
来源：http://ux.szxytkj.cn

[T09] Kotlin：扩展函数
来源：http://as.haigaiapp.cn

fun String.exclaim() = this + "!"
来源：http://rh.chemitech.net.cn

[T10] Kotlin：默认参数
来源：http://tb.huixinmuqiang.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://fn.colortex.cn

[T11] Kotlin：协程
来源：http://ej.asd995.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://db.yuexingan06.cn

[T12] Kotlin：解构声明
来源：http://mp.shxzukj.cn

val (a, b) = Pair(1, 2)
来源：http://kx.bookmarksfly.cn

[T13] Kotlin：只读 Map
来源：http://jz.huixinmuqiang.cn

val m = mapOf("a" to 1)
来源：http://mu.chemitech.net.cn

[T14] Kotlin：循环
来源：http://kl.9csxet.cn

for (i in 1..10) println(i)
来源：http://me.shxzukj.cn

[T15] Kotlin：接口
来源：http://jx.9csxet.cn

interface Shape { fun area(): Double }
来源：http://hl.bjjhwx.cn

[T16] Swift：Hello World
来源：http://ql.haigaiapp.cn

print("Hello")
来源：http://eq.muxihuayi.cn

[T17] Swift：变量与常量
来源：http://hi.nicolike.cn

var a = 1;  let b = 2
来源：http://kb.lnxyls.cn

[T18] Swift：字符串插值
来源：http://bj.huanxung.cn

"值: \(b)"
来源：http://pn.nicolike.cn

[T19] Swift：可选绑定
来源：http://ma.9csxet.cn

if let n = opt { print(n) }
来源：http://ob.bookmarksfly.cn

[T20] Swift：数组操作
来源：http://ji.nszjky.cn

var a = [1, 2, 3];  a.append(4)
来源：http://wz.huixinmuqiang.cn

[T21] Swift：遍历
来源：http://rl.szxytkj.cn

for x in a { print(x) }
来源：http://wc.chemitech.net.cn

[T22] Swift：字典
来源：http://ws.hahajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://el.jctech888.com.cn

[T23] Swift：函数
来源：http://bt.bjjhwx.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qz.muxihuayi.cn

[T24] Swift：闭包
来源：http://gu.colortex.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ds.shxzskj.cn

[T25] Swift：结构体
来源：http://qf.lnxyls.cn

struct P { var x: Int }
来源：http://kx.jianghongdianzi.cn

[T26] Swift：类与重写
来源：http://om.jianghongdianzi.cn

class A: Base { override func f() {} }
来源：http://fh.shxzskj.cn

[T27] Swift：错误处理
来源：http://oa.panjiajie.cn

do { try f() } catch { print(error) }
来源：http://am.szsharing.cn

[T28] Swift：枚举
来源：http://ps.newstarts.cn

enum Color { case red, green }
来源：http://rw.szsharing.cn

[T29] Swift：guard 提前返回
来源：http://oz.szxytkj.cn

guard let x = opt else { return }
来源：http://lq.haigaiapp.cn

[T30] Swift：协议
来源：http://zm.jianghongdianzi.cn

protocol Shape { func area() -> Double }
来源：http://xi.huanxung.cn

[T31] Lua：Hello World
来源：http://dq.newstarts.cn

print("Hello")
来源：http://wv.bjjhwx.cn

[T32] Lua：局部变量
来源：http://ah.asd995.cn

local a = 1
来源：http://uu.muxihuayi.cn

[T33] Lua：表（数组）
来源：http://df.9csxet.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://or.szsharing.cn

[T34] Lua：遍历表
来源：http://cb.asd995.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ro.9csxet.cn

[T35] Lua：字典表
来源：http://aa.hnjuh.cn

local d = { a = 1 };  d.b = 2
来源：http://nt.chemitech.net.cn

[T36] Lua：函数
来源：http://tm.szsharing.cn

function add(a, b) return a + b end
来源：http://de.shxzskj.cn

[T37] Lua：字符串拼接
来源：http://ft.chemitech.net.cn

"a" .. "b"
来源：http://wh.szsharing.cn

[T38] Lua：条件
来源：http://qc.nszjky.cn

if x > 0 then print("正") end
来源：http://bl.hahajie.cn

[T39] Lua：模式匹配
来源：http://gs.jctech888.com.cn

string.find(s, "%d+")
来源：http://fh.huixiangedu.cn

[T40] Lua：元表
来源：http://ab.yuexingan06.cn

setmetatable({}, { __index = base })
来源：http://fs.huanxung.cn

[T41] Perl：Hello World
来源：http://xa.bookmarksfly.cn

print "Hello\n";
来源：http://cs.asd995.cn

[T42] Perl：变量类型
来源：http://mu.jianghongdianzi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hd.lnxyls.cn

[T43] Perl：字符串插值
来源：http://gh.yuntaijiaju.cn

"值: $a"
来源：http://xa.panjiajie.cn

[T44] Perl：条件
来源：http://hf.bookmarksfly.cn

if ($a > 0) { print "正"; }
来源：http://fj.huixinmuqiang.cn

[T45] Perl：数组遍历
来源：http://vr.asd995.cn

for my $x (@arr) { print $x; }
来源：http://lg.huanxung.cn

[T46] Perl：哈希操作
来源：http://az.bjjhwx.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://li.bjjhwx.cn

[T47] Perl：正则捕获
来源：http://pi.haigaiapp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://tl.haigaiapp.cn

[T48] Perl：正则替换
来源：http://uq.hahajie.cn

$s =~ s/old/new/g;
来源：http://oo.hahajie.cn

[T49] Perl：函数
来源：http://pw.huanxung.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ao.lnxyls.cn

[T50] Perl：逐行读文件
来源：http://uf.colortex.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ai.wgjwhj.cn

while (my $line = <$fh>) { print $line; }
来源：http://ph.newstarts.cn

[T51] Scala：Hello World
来源：http://rw.jianghongdianzi.cn

println("Hello")
来源：http://rl.shxzskj.cn

[T52] Scala：变量
来源：http://yz.hahajie.cn

val a = 1;  var b = 2
来源：http://fw.yuntaijiaju.cn

[T53] Scala：字符串插值
来源：http://vt.521024.cn

s"值: $b"
来源：http://ql.nicolike.cn

[T54] Scala：集合映射
来源：http://vk.yuexingan06.cn

List(1, 2, 3).map(_ * 2)
来源：http://ku.jctech888.com.cn

[T55] Scala：集合过滤
来源：http://xm.521024.cn

List(1, 2, 3).filter(_ > 1)
来源：http://bd.szxytkj.cn

[T56] Scala：样例类
来源：http://ij.jctech888.com.cn

case class User(name: String, age: Int)
来源：http://oq.bookmarksfly.cn

[T57] Scala：模式匹配
来源：http://bz.haigaiapp.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gh.521024.cn

[T58] Scala：函数定义
来源：http://nn.9csxet.cn

def add(a: Int, b: Int): Int = a + b
来源：http://nz.yuexingan06.cn

[T59] Scala：循环
来源：http://lf.nszjky.cn

for (i <- 1 to 10) println(i)
来源：http://gt.haigaiapp.cn

[T60] Scala：折叠
来源：http://aa.shxzskj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ys.huanxung.cn

================================================================================
来源：http://cj.chemitech.net.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jv.szxytkj.cn

================================================================================
来源：http://qp.9csxet.cn

[U01] Py：创建虚拟环境
来源：http://ge.yuexingan06.cn

python -m venv .venv && source .venv/bin/activate
来源：http://uf.szxytkj.cn

[U02] Py：导出 / 安装依赖
来源：http://go.hnjuh.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nb.wgjwhj.cn

[U03] Py：加载 .env 配置
来源：http://vd.huanxung.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ye.hnjuh.cn

[U04] Py：变量调试打印
来源：http://ki.szxytkj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fq.hnjuh.cn

[U05] Py：列表去重且保序
来源：http://bj.shtwfgs.cn

list(dict.fromkeys(arr))
来源：http://qf.nszjky.cn

[U06] Py：合并两个字典
来源：http://nh.nicolike.cn

{**a, **b}
来源：http://sj.asd995.cn

[U07] Py：反转字典键值
来源：http://nn.shxzukj.cn

{v: k for k, v in d.items()}
来源：http://cg.newstarts.cn

[U08] Py：展平二维列表
来源：http://sl.huixinmuqiang.cn

[y for x in nested for y in x]
来源：http://jx.huanxung.cn

[U09] Py：字典取最大值的键
来源：http://ik.hnjuh.cn

max(d, key=d.get)
来源：http://xl.hnjuh.cn

[U10] Py：按值排序字典
来源：http://uv.9csxet.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://go.muxihuayi.cn

[U11] Py：生成器表达式
来源：http://og.bjjhwx.cn

(x * 2 for x in arr)
来源：http://mv.nszjky.cn

[U12] Py：取出现最多的 3 个元素
来源：http://gl.szsharing.cn

Counter(arr).most_common(3)
来源：http://ni.yuntaijiaju.cn

[U13] Py：固定长度队列
来源：http://wu.nicolike.cn

deque(maxlen=10)
来源：http://so.nszjky.cn

[U14] Py：分组收集到列表
来源：http://le.9csxet.cn

defaultdict(list)
来源：http://jk.asd995.cn

[U15] Py：高精度计时
来源：http://ec.lnxyls.cn

t = time.perf_counter()
来源：http://lb.shtwfgs.cn

[U16] Py：命令行参数解析
来源：http://im.chemitech.net.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ot.huanxung.cn

[U17] Py：初始化日志
来源：http://ln.9csxet.cn

logging.basicConfig(level=logging.INFO)
来源：http://al.lnxyls.cn

[U18] Py：预编译正则
来源：http://gj.huanxung.cn

pat = re.compile(r"\d+")
来源：http://aa.colortex.cn

[U19] Py：正则替换带回调
来源：http://lm.huanxung.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wk.asd995.cn

[U20] Py：缓存函数结果
来源：http://xl.shxzukj.cn

@functools.lru_cache(maxsize=None)
来源：http://ur.huixinmuqiang.cn

[U21] Py：自定义上下文管理器
来源：http://ba.jianghongdianzi.cn

@contextlib.contextmanager
来源：http://rb.yuexingan06.cn

[U22] Py：矩阵转置
来源：http://nd.huanxung.cn

list(zip(*m))
来源：http://cj.asd995.cn

[U23] Py：分块读取大文件
来源：http://wt.shxzskj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mv.hnjuh.cn

[U24] Py：路径操作
来源：http://pq.shtwfgs.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://uk.hnjuh.cn

[U25] Py：CSV 按字典读
来源：http://gu.9csxet.cn

csv.DictReader(f)
来源：http://xa.szxytkj.cn

[U26] Py：并发下载
来源：http://vu.huixiangedu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jo.9csxet.cn

[U27] Py：异步 HTTP
来源：http://yw.yuntaijiaju.cn

aiohttp.ClientSession() 配合 async with
来源：http://qv.521024.cn

[U28] Py：类型别名
来源：http://oz.521024.cn

UserId = int
来源：http://nt.lnxyls.cn

[U29] Py：属性校验
来源：http://tp.shtwfgs.cn

@property 与 @x.setter 配合
来源：http://tb.jianghongdianzi.cn

[U30] Py：数据类
来源：http://mo.521024.cn

@dataclass(slots=True)
来源：http://di.newstarts.cn

[U31] Py：单测
来源：http://uh.newstarts.cn

python -m pytest -q
来源：http://xg.huixiangedu.cn

[U32] Py：代码格式化
来源：http://zx.huixiangedu.cn

ruff format . && ruff check --fix .
来源：http://sd.9csxet.cn

[U33] Py：打包发布
来源：http://ot.newstarts.cn

python -m build  （依赖 pyproject.toml）
来源：http://in.9csxet.cn

[U34] Py：判断编码
来源：http://il.huixiangedu.cn

chardet.detect(raw)
来源：http://yz.szsharing.cn

[U35] Py：发送邮件
来源：http://cn.nicolike.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vp.haigaiapp.cn

[U36] Py：定时任务
来源：http://ue.nicolike.cn

schedule.every(10).minutes.do(job)
来源：http://vv.shtwfgs.cn

[U37] Py：读写 Excel
来源：http://it.huanxung.cn

pandas.read_excel / DataFrame.to_excel
来源：http://gt.yuntaijiaju.cn

[U38] Py：获取脚本所在目录
来源：http://gh.hnjuh.cn

Path(__file__).resolve().parent
来源：http://hn.shtwfgs.cn

[U39] Py：判断是否在交互环境
来源：http://az.hnjuh.cn

sys.stdout.isatty()
来源：http://iq.jctech888.com.cn

[U40] Py：打印到标准错误
来源：http://mt.nszjky.cn

print("err", file=sys.stderr)
来源：http://rr.shxzukj.cn

[U41] PHP：初始化 Composer 项目
来源：http://lb.asd995.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://hu.yuntaijiaju.cn

[U42] PHP：PSR-4 自动加载
来源：http://nb.shxzskj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ky.521024.cn

[U43] PHP：声明命名空间
来源：http://oq.9csxet.cn

namespace App\Http;
来源：http://mm.huixinmuqiang.cn

[U44] PHP：开启严格类型
来源：http://cf.gzmigu.cn

declare(strict_types=1);
来源：http://jd.wgjwhj.cn

[U45] PHP：类型声明与返回类型
来源：http://rw.panjiajie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://yk.shxzukj.cn

[U46] PHP：可空类型
来源：http://vo.szsharing.cn

?string $name = null
来源：http://yf.newstarts.cn

[U47] PHP：联合类型
来源：http://xc.gzmigu.cn

int|string $id
来源：http://hx.521024.cn

[U48] PHP：纯枚举
来源：http://wc.newstarts.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://df.muxihuayi.cn

[U49] PHP：只读属性
来源：http://iw.jianghongdianzi.cn

public readonly string $name
来源：http://rv.nszjky.cn

[U50] PHP：构造器属性提升
来源：http://ja.yuntaijiaju.cn

public function __construct(private int $id) {}
来源：http://id.jianghongdianzi.cn

[U51] PHP：数组解构
来源：http://uf.bookmarksfly.cn

[$a, $b] = $arr;
来源：http://dh.yuexingan06.cn

[U52] PHP：箭头函数
来源：http://ul.hnjuh.cn

$double = fn($x) => $x * 2;
来源：http://sd.muxihuayi.cn

[U53] PHP：空合并运算符
来源：http://en.bookmarksfly.cn

$v = $a ?? $b ?? "default";
来源：http://qm.nicolike.cn

[U54] PHP：空安全调用
来源：http://ae.yuntaijiaju.cn

$obj?->method()
来源：http://qv.nicolike.cn

[U55] PHP：match 表达式
来源：http://rf.asd995.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cn.yuntaijiaju.cn

[U56] PHP：命名参数
来源：http://by.muxihuayi.cn

f(a: 1, b: 2)
来源：http://wf.huanxung.cn

[U57] PHP：字符串插值
来源：http://ln.haigaiapp.cn

"值: {$a}"
来源：http://xm.jianghongdianzi.cn

[U58] PHP：数组三件套
来源：http://uw.hnjuh.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xu.shtwfgs.cn

[U59] PHP：自定义排序
来源：http://vo.huixiangedu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hl.muxihuayi.cn

[U60] PHP：JSON 编解码
来源：http://gf.muxihuayi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xl.huixinmuqiang.cn

[U61] PHP：正则
来源：http://ws.panjiajie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gb.shtwfgs.cn

[U62] PHP：日期对象
来源：http://zr.shxzskj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mp.nicolike.cn

[U63] PHP：文件读写
来源：http://xq.bjjhwx.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zr.lnxyls.cn

[U64] PHP：目录遍历
来源：http://vn.521024.cn

glob("dir/*.php");  scandir("dir");
来源：http://gl.chemitech.net.cn

[U65] PHP：会话
来源：http://mx.hnjuh.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://bw.hnjuh.cn

[U66] PHP：设置 Cookie
来源：http://kn.lnxyls.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://uq.hnjuh.cn

[U67] PHP：处理文件上传
来源：http://oh.szsharing.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xk.bjjhwx.cn

[U68] PHP：PDO 连接
来源：http://pb.yuexingan06.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://na.jianghongdianzi.cn

[U69] PHP：PDO 预处理
来源：http://vn.nicolike.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xz.newstarts.cn

[U70] PHP：PDO 事务
来源：http://bx.szxytkj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dc.yuntaijiaju.cn

[U71] PHP：抛出异常
来源：http://sx.bookmarksfly.cn

throw new RuntimeException("失败", 500);
来源：http://qr.colortex.cn

[U72] PHP：写错误日志
来源：http://qr.nszjky.cn

error_log("失败: " . $e->getMessage());
来源：http://od.hnjuh.cn

[U73] PHP：读取 ini 配置
来源：http://yf.bookmarksfly.cn

parse_ini_file("config.ini", true)
来源：http://cx.yuexingan06.cn

[U74] PHP：读取环境变量
来源：http://ca.bjjhwx.cn

getenv("APP_ENV") ?: "production"
来源：http://em.szsharing.cn

[U75] PHP：依赖注入
来源：http://vt.newstarts.cn

composer require psr/container
来源：http://yi.nszjky.cn

[U76] PHP：简单路由
来源：http://yu.yuexingan06.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bn.shxzukj.cn

[U77] PHP：模板渲染
来源：http://rg.gzmigu.cn

composer require twig/twig
来源：http://mw.szxytkj.cn

[U78] PHP：单元测试
来源：http://la.chemitech.net.cn

composer require --dev phpunit/phpunit
来源：http://kw.gzmigu.cn

[U79] PHP：静态分析
来源：http://ue.huanxung.cn

composer require --dev phpstan/phpstan
来源：http://az.hnjuh.cn

[U80] PHP：代码规范修复
来源：http://th.yuexingan06.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jq.shtwfgs.cn

[U81] JS：初始化项目
来源：http://io.lnxyls.cn

npm init -y;  npm i express
来源：http://li.huixinmuqiang.cn

[U82] JS：package.json 脚本
来源：http://xq.chemitech.net.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zn.shtwfgs.cn

[U83] JS：ES Module 导入导出
来源：http://bi.muxihuayi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qo.jctech888.com.cn

[U84] JS：CommonJS 写法
来源：http://ik.bookmarksfly.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ca.szxytkj.cn

[U85] JS：可选链
来源：http://ew.shxzukj.cn

a?.b?.c
来源：http://nl.huixiangedu.cn

[U86] JS：空值合并
来源：http://dd.haigaiapp.cn

a ?? b
来源：http://an.jianghongdianzi.cn

[U87] JS：解构默认值
来源：http://xp.shxzukj.cn

const { a = 1, b = 2 } = obj;
来源：http://et.yuntaijiaju.cn

[U88] JS：对象展开合并
来源：http://rg.colortex.cn

{ ...a, ...b }
来源：http://vl.huanxung.cn


<!-- 参考信息 -->