代发 wailian999

[T03] Kotlin：字符串模板
来源：http://xc.shtwfgs.cn

"值: $b"
来源：http://jr.huanxung.cn

[T04] Kotlin：空安全
来源：http://vc.jctech888.com.cn

val n: String? = null;  n?.length
来源：http://hh.yuexingan06.cn

[T05] Kotlin：when 表达式
来源：http://cj.521024.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vc.shxzskj.cn

[T06] Kotlin：集合映射
来源：http://gk.bjjhwx.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://im.szsharing.cn

[T07] Kotlin：集合过滤
来源：http://ed.nszjky.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ic.panjiajie.cn

[T08] Kotlin：数据类
来源：http://jg.huanxung.cn

data class User(val name: String, val age: Int)
来源：http://qa.szsharing.cn

[T09] Kotlin：扩展函数
来源：http://df.yuexingan06.cn

fun String.exclaim() = this + "!"
来源：http://sm.nszjky.cn

[T10] Kotlin：默认参数
来源：http://nk.hnjuh.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ou.nicolike.cn

[T11] Kotlin：协程
来源：http://wj.521024.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://gn.nicolike.cn

[T12] Kotlin：解构声明
来源：http://st.jctech888.com.cn

val (a, b) = Pair(1, 2)
来源：http://vn.szsharing.cn

[T13] Kotlin：只读 Map
来源：http://zo.nicolike.cn

val m = mapOf("a" to 1)
来源：http://vz.chemitech.net.cn

[T14] Kotlin：循环
来源：http://iq.yuexingan06.cn

for (i in 1..10) println(i)
来源：http://nq.panjiajie.cn

[T15] Kotlin：接口
来源：http://fj.hnjuh.cn

interface Shape { fun area(): Double }
来源：http://ys.bookmarksfly.cn

[T16] Swift：Hello World
来源：http://wd.huanxung.cn

print("Hello")
来源：http://yx.521024.cn

[T17] Swift：变量与常量
来源：http://bl.9csxet.cn

var a = 1;  let b = 2
来源：http://bl.gzmigu.cn

[T18] Swift：字符串插值
来源：http://cx.shtwfgs.cn

"值: \(b)"
来源：http://en.jctech888.com.cn

[T19] Swift：可选绑定
来源：http://oz.9csxet.cn

if let n = opt { print(n) }
来源：http://ui.haigaiapp.cn

[T20] Swift：数组操作
来源：http://lq.shtwfgs.cn

var a = [1, 2, 3];  a.append(4)
来源：http://rc.521024.cn

[T21] Swift：遍历
来源：http://fg.hahajie.cn

for x in a { print(x) }
来源：http://aa.bjjhwx.cn

[T22] Swift：字典
来源：http://pf.nicolike.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ye.haigaiapp.cn

[T23] Swift：函数
来源：http://ht.asd995.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cx.huixinmuqiang.cn

[T24] Swift：闭包
来源：http://jb.chemitech.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vi.yuntaijiaju.cn

[T25] Swift：结构体
来源：http://pf.nszjky.cn

struct P { var x: Int }
来源：http://eb.wgjwhj.cn

[T26] Swift：类与重写
来源：http://hn.huixiangedu.cn

class A: Base { override func f() {} }
来源：http://kz.szsharing.cn

[T27] Swift：错误处理
来源：http://nc.asd995.cn

do { try f() } catch { print(error) }
来源：http://uo.nicolike.cn

[T28] Swift：枚举
来源：http://bx.huanxung.cn

enum Color { case red, green }
来源：http://th.yuexingan06.cn

[T29] Swift：guard 提前返回
来源：http://ub.nszjky.cn

guard let x = opt else { return }
来源：http://iw.huixiangedu.cn

[T30] Swift：协议
来源：http://ge.yuntaijiaju.cn

protocol Shape { func area() -> Double }
来源：http://vm.huixinmuqiang.cn

[T31] Lua：Hello World
来源：http://wn.bookmarksfly.cn

print("Hello")
来源：http://nm.9csxet.cn

[T32] Lua：局部变量
来源：http://xl.shtwfgs.cn

local a = 1
来源：http://wj.chemitech.net.cn

[T33] Lua：表（数组）
来源：http://xz.lnxyls.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://qm.bjjhwx.cn

[T34] Lua：遍历表
来源：http://hn.nszjky.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zz.shxzskj.cn

[T35] Lua：字典表
来源：http://tu.colortex.cn

local d = { a = 1 };  d.b = 2
来源：http://qk.jctech888.com.cn

[T36] Lua：函数
来源：http://oq.jctech888.com.cn

function add(a, b) return a + b end
来源：http://xl.huixinmuqiang.cn

[T37] Lua：字符串拼接
来源：http://ms.huanxung.cn

"a" .. "b"
来源：http://vg.panjiajie.cn

[T38] Lua：条件
来源：http://yr.yuntaijiaju.cn

if x > 0 then print("正") end
来源：http://px.521024.cn

[T39] Lua：模式匹配
来源：http://gm.colortex.cn

string.find(s, "%d+")
来源：http://vr.newstarts.cn

[T40] Lua：元表
来源：http://eb.shxzskj.cn

setmetatable({}, { __index = base })
来源：http://vh.shxzukj.cn

[T41] Perl：Hello World
来源：http://gu.huixinmuqiang.cn

print "Hello\n";
来源：http://ou.nicolike.cn

[T42] Perl：变量类型
来源：http://eq.haigaiapp.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cc.9csxet.cn

[T43] Perl：字符串插值
来源：http://vm.huixiangedu.cn

"值: $a"
来源：http://ti.hnjuh.cn

[T44] Perl：条件
来源：http://ey.nicolike.cn

if ($a > 0) { print "正"; }
来源：http://kt.muxihuayi.cn

[T45] Perl：数组遍历
来源：http://js.hnjuh.cn

for my $x (@arr) { print $x; }
来源：http://rg.asd995.cn

[T46] Perl：哈希操作
来源：http://dv.newstarts.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ti.chemitech.net.cn

[T47] Perl：正则捕获
来源：http://cb.bjjhwx.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://br.huixiangedu.cn

[T48] Perl：正则替换
来源：http://wk.huixinmuqiang.cn

$s =~ s/old/new/g;
来源：http://zc.chemitech.net.cn

[T49] Perl：函数
来源：http://gg.nicolike.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qb.hahajie.cn

[T50] Perl：逐行读文件
来源：http://fh.yuntaijiaju.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://by.asd995.cn

while (my $line = <$fh>) { print $line; }
来源：http://my.yuexingan06.cn

[T51] Scala：Hello World
来源：http://qh.jianghongdianzi.cn

println("Hello")
来源：http://nc.colortex.cn

[T52] Scala：变量
来源：http://io.9csxet.cn

val a = 1;  var b = 2
来源：http://vb.bookmarksfly.cn

[T53] Scala：字符串插值
来源：http://vj.chemitech.net.cn

s"值: $b"
来源：http://jg.nicolike.cn

[T54] Scala：集合映射
来源：http://vc.huixinmuqiang.cn

List(1, 2, 3).map(_ * 2)
来源：http://ru.chemitech.net.cn

[T55] Scala：集合过滤
来源：http://km.bjjhwx.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fd.jctech888.com.cn

[T56] Scala：样例类
来源：http://tk.hahajie.cn

case class User(name: String, age: Int)
来源：http://fc.hahajie.cn

[T57] Scala：模式匹配
来源：http://wb.haigaiapp.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wb.hnjuh.cn

[T58] Scala：函数定义
来源：http://ce.jctech888.com.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ne.chemitech.net.cn

[T59] Scala：循环
来源：http://yt.yuexingan06.cn

for (i <- 1 to 10) println(i)
来源：http://qz.lnxyls.cn

[T60] Scala：折叠
来源：http://qw.szsharing.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qn.gzmigu.cn

================================================================================
来源：http://tq.shxzukj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wf.jctech888.com.cn

================================================================================
来源：http://aq.asd995.cn

[U01] Py：创建虚拟环境
来源：http://ss.nicolike.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vu.wgjwhj.cn

[U02] Py：导出 / 安装依赖
来源：http://bj.wgjwhj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hd.nicolike.cn

[U03] Py：加载 .env 配置
来源：http://ds.panjiajie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://yn.huixiangedu.cn

[U04] Py：变量调试打印
来源：http://uc.9csxet.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zs.nicolike.cn

[U05] Py：列表去重且保序
来源：http://xc.huixinmuqiang.cn

list(dict.fromkeys(arr))
来源：http://yy.521024.cn

[U06] Py：合并两个字典
来源：http://le.shtwfgs.cn

{**a, **b}
来源：http://tr.nszjky.cn

[U07] Py：反转字典键值
来源：http://rf.muxihuayi.cn

{v: k for k, v in d.items()}
来源：http://rf.bjjhwx.cn

[U08] Py：展平二维列表
来源：http://rf.9csxet.cn

[y for x in nested for y in x]
来源：http://ip.nszjky.cn

[U09] Py：字典取最大值的键
来源：http://nc.szxytkj.cn

max(d, key=d.get)
来源：http://gw.9csxet.cn

[U10] Py：按值排序字典
来源：http://gd.asd995.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vg.hahajie.cn

[U11] Py：生成器表达式
来源：http://sw.yuntaijiaju.cn

(x * 2 for x in arr)
来源：http://zk.wgjwhj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://fh.hnjuh.cn

Counter(arr).most_common(3)
来源：http://nk.521024.cn

[U13] Py：固定长度队列
来源：http://oo.wgjwhj.cn

deque(maxlen=10)
来源：http://lh.yuntaijiaju.cn

[U14] Py：分组收集到列表
来源：http://lf.jctech888.com.cn

defaultdict(list)
来源：http://jm.shtwfgs.cn

[U15] Py：高精度计时
来源：http://yi.shxzukj.cn

t = time.perf_counter()
来源：http://jv.shxzskj.cn

[U16] Py：命令行参数解析
来源：http://dt.yuntaijiaju.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lb.asd995.cn

[U17] Py：初始化日志
来源：http://ow.hnjuh.cn

logging.basicConfig(level=logging.INFO)
来源：http://mg.hahajie.cn

[U18] Py：预编译正则
来源：http://nx.bookmarksfly.cn

pat = re.compile(r"\d+")
来源：http://hu.muxihuayi.cn

[U19] Py：正则替换带回调
来源：http://hi.szsharing.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fe.newstarts.cn

[U20] Py：缓存函数结果
来源：http://qe.shtwfgs.cn

@functools.lru_cache(maxsize=None)
来源：http://te.chemitech.net.cn

[U21] Py：自定义上下文管理器
来源：http://ug.jianghongdianzi.cn

@contextlib.contextmanager
来源：http://ii.wgjwhj.cn

[U22] Py：矩阵转置
来源：http://fa.lnxyls.cn

list(zip(*m))
来源：http://dz.wgjwhj.cn

[U23] Py：分块读取大文件
来源：http://jt.szsharing.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://so.huanxung.cn

[U24] Py：路径操作
来源：http://zg.muxihuayi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://js.newstarts.cn

[U25] Py：CSV 按字典读
来源：http://py.szsharing.cn

csv.DictReader(f)
来源：http://oq.yuexingan06.cn

[U26] Py：并发下载
来源：http://xt.bookmarksfly.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yj.9csxet.cn

[U27] Py：异步 HTTP
来源：http://lj.bjjhwx.cn

aiohttp.ClientSession() 配合 async with
来源：http://qw.lnxyls.cn

[U28] Py：类型别名
来源：http://ki.bjjhwx.cn

UserId = int
来源：http://ly.huixinmuqiang.cn

[U29] Py：属性校验
来源：http://tb.9csxet.cn

@property 与 @x.setter 配合
来源：http://xf.jctech888.com.cn

[U30] Py：数据类
来源：http://lk.nszjky.cn

@dataclass(slots=True)
来源：http://lk.panjiajie.cn

[U31] Py：单测
来源：http://mi.gzmigu.cn

python -m pytest -q
来源：http://um.hahajie.cn

[U32] Py：代码格式化
来源：http://vu.lnxyls.cn

ruff format . && ruff check --fix .
来源：http://pk.hahajie.cn

[U33] Py：打包发布
来源：http://xt.shxzukj.cn

python -m build  （依赖 pyproject.toml）
来源：http://py.hahajie.cn

[U34] Py：判断编码
来源：http://br.szxytkj.cn

chardet.detect(raw)
来源：http://ue.asd995.cn

[U35] Py：发送邮件
来源：http://yk.huixiangedu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jd.hnjuh.cn

[U36] Py：定时任务
来源：http://xn.huixinmuqiang.cn

schedule.every(10).minutes.do(job)
来源：http://zo.muxihuayi.cn

[U37] Py：读写 Excel
来源：http://tq.yuexingan06.cn

pandas.read_excel / DataFrame.to_excel
来源：http://fa.muxihuayi.cn

[U38] Py：获取脚本所在目录
来源：http://lo.chemitech.net.cn

Path(__file__).resolve().parent
来源：http://xu.shtwfgs.cn

[U39] Py：判断是否在交互环境
来源：http://pc.hnjuh.cn

sys.stdout.isatty()
来源：http://cw.bookmarksfly.cn

[U40] Py：打印到标准错误
来源：http://qh.hnjuh.cn

print("err", file=sys.stderr)
来源：http://fr.colortex.cn

[U41] PHP：初始化 Composer 项目
来源：http://ge.gzmigu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://pv.bjjhwx.cn

[U42] PHP：PSR-4 自动加载
来源：http://so.asd995.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://iz.bjjhwx.cn

[U43] PHP：声明命名空间
来源：http://mk.colortex.cn

namespace App\Http;
来源：http://qg.bookmarksfly.cn

[U44] PHP：开启严格类型
来源：http://cz.wgjwhj.cn

declare(strict_types=1);
来源：http://ir.shxzukj.cn

[U45] PHP：类型声明与返回类型
来源：http://ze.nicolike.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://up.muxihuayi.cn

[U46] PHP：可空类型
来源：http://xs.jianghongdianzi.cn

?string $name = null
来源：http://lp.nszjky.cn

[U47] PHP：联合类型
来源：http://hp.yuexingan06.cn

int|string $id
来源：http://fd.jctech888.com.cn

[U48] PHP：纯枚举
来源：http://fx.shtwfgs.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ti.hahajie.cn

[U49] PHP：只读属性
来源：http://dz.hahajie.cn

public readonly string $name
来源：http://ja.lnxyls.cn

[U50] PHP：构造器属性提升
来源：http://ii.yuexingan06.cn

public function __construct(private int $id) {}
来源：http://vj.haigaiapp.cn

[U51] PHP：数组解构
来源：http://oc.nicolike.cn

[$a, $b] = $arr;
来源：http://sj.szsharing.cn

[U52] PHP：箭头函数
来源：http://li.hahajie.cn

$double = fn($x) => $x * 2;
来源：http://id.wgjwhj.cn

[U53] PHP：空合并运算符
来源：http://za.szsharing.cn

$v = $a ?? $b ?? "default";
来源：http://qz.bookmarksfly.cn

[U54] PHP：空安全调用
来源：http://zk.szsharing.cn

$obj?->method()
来源：http://le.hnjuh.cn

[U55] PHP：match 表达式
来源：http://xe.gzmigu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ou.haigaiapp.cn

[U56] PHP：命名参数
来源：http://oe.szsharing.cn

f(a: 1, b: 2)
来源：http://ix.shxzskj.cn

[U57] PHP：字符串插值
来源：http://ks.panjiajie.cn

"值: {$a}"
来源：http://kp.huixiangedu.cn

[U58] PHP：数组三件套
来源：http://ci.bookmarksfly.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vn.hahajie.cn

[U59] PHP：自定义排序
来源：http://ob.hnjuh.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pt.jctech888.com.cn

[U60] PHP：JSON 编解码
来源：http://dm.hnjuh.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bq.bookmarksfly.cn

[U61] PHP：正则
来源：http://lv.yuexingan06.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://co.nszjky.cn

[U62] PHP：日期对象
来源：http://at.hahajie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bz.yuntaijiaju.cn

[U63] PHP：文件读写
来源：http://on.yuexingan06.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bi.bookmarksfly.cn

[U64] PHP：目录遍历
来源：http://nl.9csxet.cn

glob("dir/*.php");  scandir("dir");
来源：http://br.hahajie.cn

[U65] PHP：会话
来源：http://hn.shxzukj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ji.huanxung.cn

[U66] PHP：设置 Cookie
来源：http://bu.jctech888.com.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wf.haigaiapp.cn

[U67] PHP：处理文件上传
来源：http://mz.szxytkj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ax.muxihuayi.cn

[U68] PHP：PDO 连接
来源：http://fx.jctech888.com.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ri.huixinmuqiang.cn

[U69] PHP：PDO 预处理
来源：http://ki.gzmigu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rz.szsharing.cn

[U70] PHP：PDO 事务
来源：http://mf.bookmarksfly.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vn.bjjhwx.cn

[U71] PHP：抛出异常
来源：http://ze.shxzukj.cn

throw new RuntimeException("失败", 500);
来源：http://fa.szsharing.cn

[U72] PHP：写错误日志
来源：http://sz.shtwfgs.cn

error_log("失败: " . $e->getMessage());
来源：http://ze.asd995.cn

[U73] PHP：读取 ini 配置
来源：http://fj.muxihuayi.cn

parse_ini_file("config.ini", true)
来源：http://jm.bookmarksfly.cn

[U74] PHP：读取环境变量
来源：http://mu.9csxet.cn

getenv("APP_ENV") ?: "production"
来源：http://ce.jianghongdianzi.cn

[U75] PHP：依赖注入
来源：http://ab.huixinmuqiang.cn

composer require psr/container
来源：http://xn.haigaiapp.cn

[U76] PHP：简单路由
来源：http://ht.shtwfgs.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pb.shxzskj.cn

[U77] PHP：模板渲染
来源：http://xn.szxytkj.cn

composer require twig/twig
来源：http://zp.shxzukj.cn

[U78] PHP：单元测试
来源：http://pb.yuntaijiaju.cn

composer require --dev phpunit/phpunit
来源：http://ci.bookmarksfly.cn

[U79] PHP：静态分析
来源：http://mr.nszjky.cn

composer require --dev phpstan/phpstan
来源：http://ue.bookmarksfly.cn

[U80] PHP：代码规范修复
来源：http://bn.colortex.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://zl.lnxyls.cn

[U81] JS：初始化项目
来源：http://hu.panjiajie.cn

npm init -y;  npm i express
来源：http://sg.huixinmuqiang.cn

[U82] JS：package.json 脚本
来源：http://og.szsharing.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wg.huixinmuqiang.cn

[U83] JS：ES Module 导入导出
来源：http://zh.szsharing.cn

export const a = 1;  import { a } from "./m.js";
来源：http://kp.jianghongdianzi.cn

[U84] JS：CommonJS 写法
来源：http://zk.wgjwhj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wc.yuntaijiaju.cn

[U85] JS：可选链
来源：http://bq.shtwfgs.cn

a?.b?.c
来源：http://la.gzmigu.cn

[U86] JS：空值合并
来源：http://gd.jctech888.com.cn

a ?? b
来源：http://fu.shtwfgs.cn

[U87] JS：解构默认值
来源：http://mp.jianghongdianzi.cn

const { a = 1, b = 2 } = obj;
来源：http://lu.bookmarksfly.cn

[U88] JS：对象展开合并
来源：http://av.wgjwhj.cn

{ ...a, ...b }
来源：http://pp.panjiajie.cn

[U89] JS：数组去重
来源：http://xf.huanxung.cn

[...new Set(arr)]
来源：http://pq.lnxyls.cn

[U90] JS：数字数组排序
来源：http://ga.jctech888.com.cn

[...arr].sort((a, b) => a - b)
来源：http://za.szsharing.cn


<!-- 参考信息 -->