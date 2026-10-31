代发 wailian999

[T01] Kotlin：Hello World
来源：http://fz.9csxet.cn

println("Hello")
来源：http://qu.shtwfgs.cn

[T02] Kotlin：变量
来源：http://kj.shxzskj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qv.bjjhwx.cn

[T03] Kotlin：字符串模板
来源：http://bj.jianghongdianzi.cn

"值: $b"
来源：http://ch.haigaiapp.cn

[T04] Kotlin：空安全
来源：http://rn.szsharing.cn

val n: String? = null;  n?.length
来源：http://ye.yuexingan06.cn

[T05] Kotlin：when 表达式
来源：http://vw.jianghongdianzi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qn.lnxyls.cn

[T06] Kotlin：集合映射
来源：http://br.hahajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://or.9csxet.cn

[T07] Kotlin：集合过滤
来源：http://rk.huixiangedu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://cj.haigaiapp.cn

[T08] Kotlin：数据类
来源：http://fk.huanxung.cn

data class User(val name: String, val age: Int)
来源：http://cx.shxzukj.cn

[T09] Kotlin：扩展函数
来源：http://hc.shtwfgs.cn

fun String.exclaim() = this + "!"
来源：http://or.nszjky.cn

[T10] Kotlin：默认参数
来源：http://wd.yuntaijiaju.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pe.wgjwhj.cn

[T11] Kotlin：协程
来源：http://of.haigaiapp.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jp.huixiangedu.cn

[T12] Kotlin：解构声明
来源：http://cm.hahajie.cn

val (a, b) = Pair(1, 2)
来源：http://dg.shxzukj.cn

[T13] Kotlin：只读 Map
来源：http://jj.bjjhwx.cn

val m = mapOf("a" to 1)
来源：http://an.nicolike.cn

[T14] Kotlin：循环
来源：http://vz.bjjhwx.cn

for (i in 1..10) println(i)
来源：http://ei.panjiajie.cn

[T15] Kotlin：接口
来源：http://xz.szsharing.cn

interface Shape { fun area(): Double }
来源：http://aw.huixinmuqiang.cn

[T16] Swift：Hello World
来源：http://aq.yuexingan06.cn

print("Hello")
来源：http://sh.nicolike.cn

[T17] Swift：变量与常量
来源：http://lg.huixiangedu.cn

var a = 1;  let b = 2
来源：http://pz.huanxung.cn

[T18] Swift：字符串插值
来源：http://ct.colortex.cn

"值: \(b)"
来源：http://fx.hahajie.cn

[T19] Swift：可选绑定
来源：http://zy.muxihuayi.cn

if let n = opt { print(n) }
来源：http://ey.newstarts.cn

[T20] Swift：数组操作
来源：http://nw.nicolike.cn

var a = [1, 2, 3];  a.append(4)
来源：http://pz.jianghongdianzi.cn

[T21] Swift：遍历
来源：http://nm.huixinmuqiang.cn

for x in a { print(x) }
来源：http://qm.hahajie.cn

[T22] Swift：字典
来源：http://nf.colortex.cn

var d = ["a": 1];  d["b"] = 2
来源：http://sr.chemitech.net.cn

[T23] Swift：函数
来源：http://ez.nszjky.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pk.bjjhwx.cn

[T24] Swift：闭包
来源：http://uz.shxzukj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ii.panjiajie.cn

[T25] Swift：结构体
来源：http://wq.muxihuayi.cn

struct P { var x: Int }
来源：http://dk.bjjhwx.cn

[T26] Swift：类与重写
来源：http://bs.yuexingan06.cn

class A: Base { override func f() {} }
来源：http://ld.haigaiapp.cn

[T27] Swift：错误处理
来源：http://wz.wgjwhj.cn

do { try f() } catch { print(error) }
来源：http://ic.huixiangedu.cn

[T28] Swift：枚举
来源：http://sv.shxzukj.cn

enum Color { case red, green }
来源：http://yy.szxytkj.cn

[T29] Swift：guard 提前返回
来源：http://lg.hnjuh.cn

guard let x = opt else { return }
来源：http://wc.huixiangedu.cn

[T30] Swift：协议
来源：http://je.panjiajie.cn

protocol Shape { func area() -> Double }
来源：http://ah.wgjwhj.cn

[T31] Lua：Hello World
来源：http://wc.colortex.cn

print("Hello")
来源：http://bt.hahajie.cn

[T32] Lua：局部变量
来源：http://tv.shxzukj.cn

local a = 1
来源：http://pi.muxihuayi.cn

[T33] Lua：表（数组）
来源：http://yk.jianghongdianzi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ix.muxihuayi.cn

[T34] Lua：遍历表
来源：http://ze.nicolike.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rq.shxzskj.cn

[T35] Lua：字典表
来源：http://ye.newstarts.cn

local d = { a = 1 };  d.b = 2
来源：http://gj.shxzukj.cn

[T36] Lua：函数
来源：http://vn.nszjky.cn

function add(a, b) return a + b end
来源：http://wh.9csxet.cn

[T37] Lua：字符串拼接
来源：http://wb.521024.cn

"a" .. "b"
来源：http://ec.shtwfgs.cn

[T38] Lua：条件
来源：http://ww.hnjuh.cn

if x > 0 then print("正") end
来源：http://jr.bjjhwx.cn

[T39] Lua：模式匹配
来源：http://yr.szsharing.cn

string.find(s, "%d+")
来源：http://ag.yuexingan06.cn

[T40] Lua：元表
来源：http://ql.shtwfgs.cn

setmetatable({}, { __index = base })
来源：http://zm.muxihuayi.cn

[T41] Perl：Hello World
来源：http://yf.nszjky.cn

print "Hello\n";
来源：http://jz.huixiangedu.cn

[T42] Perl：变量类型
来源：http://sg.huixiangedu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yp.jctech888.com.cn

[T43] Perl：字符串插值
来源：http://th.lnxyls.cn

"值: $a"
来源：http://cm.huanxung.cn

[T44] Perl：条件
来源：http://lp.muxihuayi.cn

if ($a > 0) { print "正"; }
来源：http://qj.bookmarksfly.cn

[T45] Perl：数组遍历
来源：http://wk.yuntaijiaju.cn

for my $x (@arr) { print $x; }
来源：http://ae.jctech888.com.cn

[T46] Perl：哈希操作
来源：http://wt.yuexingan06.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fj.yuntaijiaju.cn

[T47] Perl：正则捕获
来源：http://gh.newstarts.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pf.yuexingan06.cn

[T48] Perl：正则替换
来源：http://ap.haigaiapp.cn

$s =~ s/old/new/g;
来源：http://np.szsharing.cn

[T49] Perl：函数
来源：http://mm.9csxet.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yy.yuexingan06.cn

[T50] Perl：逐行读文件
来源：http://fe.huixinmuqiang.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://nv.shtwfgs.cn

while (my $line = <$fh>) { print $line; }
来源：http://xj.jctech888.com.cn

[T51] Scala：Hello World
来源：http://ul.gzmigu.cn

println("Hello")
来源：http://mo.chemitech.net.cn

[T52] Scala：变量
来源：http://yi.shtwfgs.cn

val a = 1;  var b = 2
来源：http://cd.colortex.cn

[T53] Scala：字符串插值
来源：http://by.gzmigu.cn

s"值: $b"
来源：http://at.huanxung.cn

[T54] Scala：集合映射
来源：http://co.gzmigu.cn

List(1, 2, 3).map(_ * 2)
来源：http://zm.shxzskj.cn

[T55] Scala：集合过滤
来源：http://od.yuntaijiaju.cn

List(1, 2, 3).filter(_ > 1)
来源：http://pq.gzmigu.cn

[T56] Scala：样例类
来源：http://tf.bjjhwx.cn

case class User(name: String, age: Int)
来源：http://fr.bookmarksfly.cn

[T57] Scala：模式匹配
来源：http://bn.huixinmuqiang.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://cx.newstarts.cn

[T58] Scala：函数定义
来源：http://te.shxzukj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://sz.asd995.cn

[T59] Scala：循环
来源：http://fd.huanxung.cn

for (i <- 1 to 10) println(i)
来源：http://om.nicolike.cn

[T60] Scala：折叠
来源：http://qj.bookmarksfly.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ns.shxzskj.cn

================================================================================
来源：http://ud.chemitech.net.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ex.hnjuh.cn

================================================================================
来源：http://pz.hahajie.cn

[U01] Py：创建虚拟环境
来源：http://bt.muxihuayi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://hu.colortex.cn

[U02] Py：导出 / 安装依赖
来源：http://yk.shtwfgs.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bv.lnxyls.cn

[U03] Py：加载 .env 配置
来源：http://tc.jctech888.com.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zn.nszjky.cn

[U04] Py：变量调试打印
来源：http://uc.wgjwhj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gp.bjjhwx.cn

[U05] Py：列表去重且保序
来源：http://rb.shxzskj.cn

list(dict.fromkeys(arr))
来源：http://jk.lnxyls.cn

[U06] Py：合并两个字典
来源：http://vk.asd995.cn

{**a, **b}
来源：http://wx.szsharing.cn

[U07] Py：反转字典键值
来源：http://tw.hahajie.cn

{v: k for k, v in d.items()}
来源：http://ti.huixiangedu.cn

[U08] Py：展平二维列表
来源：http://lc.szsharing.cn

[y for x in nested for y in x]
来源：http://dv.chemitech.net.cn

[U09] Py：字典取最大值的键
来源：http://mu.shxzskj.cn

max(d, key=d.get)
来源：http://uz.lnxyls.cn

[U10] Py：按值排序字典
来源：http://wo.jctech888.com.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vq.newstarts.cn

[U11] Py：生成器表达式
来源：http://vu.szsharing.cn

(x * 2 for x in arr)
来源：http://sm.chemitech.net.cn

[U12] Py：取出现最多的 3 个元素
来源：http://oj.nicolike.cn

Counter(arr).most_common(3)
来源：http://ch.huixiangedu.cn

[U13] Py：固定长度队列
来源：http://pr.wgjwhj.cn

deque(maxlen=10)
来源：http://zx.colortex.cn

[U14] Py：分组收集到列表
来源：http://bv.panjiajie.cn

defaultdict(list)
来源：http://iu.521024.cn

[U15] Py：高精度计时
来源：http://ks.521024.cn

t = time.perf_counter()
来源：http://pc.shtwfgs.cn

[U16] Py：命令行参数解析
来源：http://xm.shtwfgs.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ml.huanxung.cn

[U17] Py：初始化日志
来源：http://bl.lnxyls.cn

logging.basicConfig(level=logging.INFO)
来源：http://om.chemitech.net.cn

[U18] Py：预编译正则
来源：http://an.yuexingan06.cn

pat = re.compile(r"\d+")
来源：http://sh.wgjwhj.cn

[U19] Py：正则替换带回调
来源：http://lw.haigaiapp.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tq.jianghongdianzi.cn

[U20] Py：缓存函数结果
来源：http://ix.gzmigu.cn

@functools.lru_cache(maxsize=None)
来源：http://hu.jctech888.com.cn

[U21] Py：自定义上下文管理器
来源：http://pl.huanxung.cn

@contextlib.contextmanager
来源：http://vd.haigaiapp.cn

[U22] Py：矩阵转置
来源：http://za.huixinmuqiang.cn

list(zip(*m))
来源：http://cg.chemitech.net.cn

[U23] Py：分块读取大文件
来源：http://ut.jctech888.com.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wr.haigaiapp.cn

[U24] Py：路径操作
来源：http://fg.newstarts.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gb.jctech888.com.cn

[U25] Py：CSV 按字典读
来源：http://ty.shxzskj.cn

csv.DictReader(f)
来源：http://md.chemitech.net.cn

[U26] Py：并发下载
来源：http://qr.nszjky.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pb.jianghongdianzi.cn

[U27] Py：异步 HTTP
来源：http://tw.asd995.cn

aiohttp.ClientSession() 配合 async with
来源：http://tb.szxytkj.cn

[U28] Py：类型别名
来源：http://qj.nicolike.cn

UserId = int
来源：http://hy.nszjky.cn

[U29] Py：属性校验
来源：http://uy.nicolike.cn

@property 与 @x.setter 配合
来源：http://gw.szsharing.cn

[U30] Py：数据类
来源：http://tl.panjiajie.cn

@dataclass(slots=True)
来源：http://om.yuntaijiaju.cn

[U31] Py：单测
来源：http://bz.9csxet.cn

python -m pytest -q
来源：http://yp.newstarts.cn

[U32] Py：代码格式化
来源：http://yv.521024.cn

ruff format . && ruff check --fix .
来源：http://sy.wgjwhj.cn

[U33] Py：打包发布
来源：http://wn.jianghongdianzi.cn

python -m build  （依赖 pyproject.toml）
来源：http://td.newstarts.cn

[U34] Py：判断编码
来源：http://uy.szxytkj.cn

chardet.detect(raw)
来源：http://yj.hnjuh.cn

[U35] Py：发送邮件
来源：http://ip.huixiangedu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bx.shtwfgs.cn

[U36] Py：定时任务
来源：http://bx.nicolike.cn

schedule.every(10).minutes.do(job)
来源：http://qm.huixiangedu.cn

[U37] Py：读写 Excel
来源：http://oz.huixiangedu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://gr.panjiajie.cn

[U38] Py：获取脚本所在目录
来源：http://ey.hnjuh.cn

Path(__file__).resolve().parent
来源：http://da.yuexingan06.cn

[U39] Py：判断是否在交互环境
来源：http://vm.shxzukj.cn

sys.stdout.isatty()
来源：http://cl.haigaiapp.cn

[U40] Py：打印到标准错误
来源：http://ow.colortex.cn

print("err", file=sys.stderr)
来源：http://ue.nszjky.cn

[U41] PHP：初始化 Composer 项目
来源：http://vd.nicolike.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ht.bookmarksfly.cn

[U42] PHP：PSR-4 自动加载
来源：http://lv.nicolike.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zu.bookmarksfly.cn

[U43] PHP：声明命名空间
来源：http://xf.bjjhwx.cn

namespace App\Http;
来源：http://gd.szsharing.cn

[U44] PHP：开启严格类型
来源：http://fq.szxytkj.cn

declare(strict_types=1);
来源：http://wb.shxzukj.cn

[U45] PHP：类型声明与返回类型
来源：http://gk.szxytkj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bk.lnxyls.cn

[U46] PHP：可空类型
来源：http://bx.hnjuh.cn

?string $name = null
来源：http://ex.shtwfgs.cn

[U47] PHP：联合类型
来源：http://tt.hahajie.cn

int|string $id
来源：http://gp.szxytkj.cn

[U48] PHP：纯枚举
来源：http://rv.asd995.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lc.szsharing.cn

[U49] PHP：只读属性
来源：http://nr.panjiajie.cn

public readonly string $name
来源：http://af.shxzskj.cn

[U50] PHP：构造器属性提升
来源：http://bz.shtwfgs.cn

public function __construct(private int $id) {}
来源：http://tk.muxihuayi.cn

[U51] PHP：数组解构
来源：http://hr.huanxung.cn

[$a, $b] = $arr;
来源：http://ta.lnxyls.cn

[U52] PHP：箭头函数
来源：http://sg.shtwfgs.cn

$double = fn($x) => $x * 2;
来源：http://oc.9csxet.cn

[U53] PHP：空合并运算符
来源：http://mw.nicolike.cn

$v = $a ?? $b ?? "default";
来源：http://yb.yuexingan06.cn

[U54] PHP：空安全调用
来源：http://zv.nicolike.cn

$obj?->method()
来源：http://ey.shxzukj.cn

[U55] PHP：match 表达式
来源：http://bf.bookmarksfly.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jq.wgjwhj.cn

[U56] PHP：命名参数
来源：http://cb.bookmarksfly.cn

f(a: 1, b: 2)
来源：http://sz.wgjwhj.cn

[U57] PHP：字符串插值
来源：http://xl.bookmarksfly.cn

"值: {$a}"
来源：http://wb.asd995.cn

[U58] PHP：数组三件套
来源：http://dw.huanxung.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://io.haigaiapp.cn

[U59] PHP：自定义排序
来源：http://fg.muxihuayi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bu.huixiangedu.cn

[U60] PHP：JSON 编解码
来源：http://kf.shxzskj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rw.panjiajie.cn

[U61] PHP：正则
来源：http://nc.bookmarksfly.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zg.bjjhwx.cn

[U62] PHP：日期对象
来源：http://nh.huixinmuqiang.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ce.asd995.cn

[U63] PHP：文件读写
来源：http://nm.huixinmuqiang.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kz.jctech888.com.cn

[U64] PHP：目录遍历
来源：http://sm.jctech888.com.cn

glob("dir/*.php");  scandir("dir");
来源：http://rs.huixinmuqiang.cn

[U65] PHP：会话
来源：http://en.hahajie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://eq.chemitech.net.cn

[U66] PHP：设置 Cookie
来源：http://bk.yuntaijiaju.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://uk.hnjuh.cn

[U67] PHP：处理文件上传
来源：http://fc.521024.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vw.haigaiapp.cn

[U68] PHP：PDO 连接
来源：http://he.huanxung.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zg.shtwfgs.cn

[U69] PHP：PDO 预处理
来源：http://eu.newstarts.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bi.9csxet.cn

[U70] PHP：PDO 事务
来源：http://uy.nicolike.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gx.nszjky.cn

[U71] PHP：抛出异常
来源：http://rt.szxytkj.cn

throw new RuntimeException("失败", 500);
来源：http://st.nszjky.cn

[U72] PHP：写错误日志
来源：http://nf.panjiajie.cn

error_log("失败: " . $e->getMessage());
来源：http://cv.shxzukj.cn

[U73] PHP：读取 ini 配置
来源：http://og.newstarts.cn

parse_ini_file("config.ini", true)
来源：http://oy.9csxet.cn

[U74] PHP：读取环境变量
来源：http://gx.hahajie.cn

getenv("APP_ENV") ?: "production"
来源：http://yq.shxzukj.cn

[U75] PHP：依赖注入
来源：http://fr.yuntaijiaju.cn

composer require psr/container
来源：http://iv.wgjwhj.cn

[U76] PHP：简单路由
来源：http://ck.huixiangedu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nx.lnxyls.cn

[U77] PHP：模板渲染
来源：http://yh.lnxyls.cn

composer require twig/twig
来源：http://xn.bjjhwx.cn

[U78] PHP：单元测试
来源：http://xk.asd995.cn

composer require --dev phpunit/phpunit
来源：http://qy.muxihuayi.cn

[U79] PHP：静态分析
来源：http://zk.huixinmuqiang.cn

composer require --dev phpstan/phpstan
来源：http://um.muxihuayi.cn

[U80] PHP：代码规范修复
来源：http://xa.jianghongdianzi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://br.nszjky.cn

[U81] JS：初始化项目
来源：http://zc.shxzskj.cn

npm init -y;  npm i express
来源：http://yr.bookmarksfly.cn

[U82] JS：package.json 脚本
来源：http://wi.shxzukj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bk.haigaiapp.cn

[U83] JS：ES Module 导入导出
来源：http://qk.muxihuayi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://oo.wgjwhj.cn

[U84] JS：CommonJS 写法
来源：http://ul.bjjhwx.cn

module.exports = { a };  const { a } = require("./m");
来源：http://go.huixinmuqiang.cn

[U85] JS：可选链
来源：http://lx.nszjky.cn

a?.b?.c
来源：http://nh.shxzukj.cn

[U86] JS：空值合并
来源：http://dl.lnxyls.cn

a ?? b
来源：http://ym.bookmarksfly.cn

[U87] JS：解构默认值
来源：http://za.hahajie.cn

const { a = 1, b = 2 } = obj;
来源：http://tv.shxzskj.cn

[U88] JS：对象展开合并
来源：http://mq.yuntaijiaju.cn

{ ...a, ...b }
来源：http://ag.bjjhwx.cn


<!-- 参考信息 -->