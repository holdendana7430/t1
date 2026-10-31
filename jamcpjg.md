代发 wailian999

[T03] Kotlin：字符串模板
来源：http://xb.9csxet.cn

"值: $b"
来源：http://xx.shxzukj.cn

[T04] Kotlin：空安全
来源：http://tq.nszjky.cn

val n: String? = null;  n?.length
来源：http://vv.huanxung.cn

[T05] Kotlin：when 表达式
来源：http://jf.chemitech.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rh.yuntaijiaju.cn

[T06] Kotlin：集合映射
来源：http://xc.9csxet.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://mq.shxzskj.cn

[T07] Kotlin：集合过滤
来源：http://ex.shxzukj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://nw.9csxet.cn

[T08] Kotlin：数据类
来源：http://oy.yuntaijiaju.cn

data class User(val name: String, val age: Int)
来源：http://pf.nicolike.cn

[T09] Kotlin：扩展函数
来源：http://qk.9csxet.cn

fun String.exclaim() = this + "!"
来源：http://on.nicolike.cn

[T10] Kotlin：默认参数
来源：http://qu.szxytkj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://uu.jctech888.com.cn

[T11] Kotlin：协程
来源：http://tg.haigaiapp.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bj.521024.cn

[T12] Kotlin：解构声明
来源：http://wt.huixiangedu.cn

val (a, b) = Pair(1, 2)
来源：http://dn.jctech888.com.cn

[T13] Kotlin：只读 Map
来源：http://kc.panjiajie.cn

val m = mapOf("a" to 1)
来源：http://nq.yuntaijiaju.cn

[T14] Kotlin：循环
来源：http://sg.bookmarksfly.cn

for (i in 1..10) println(i)
来源：http://vy.nicolike.cn

[T15] Kotlin：接口
来源：http://bj.lnxyls.cn

interface Shape { fun area(): Double }
来源：http://tg.hahajie.cn

[T16] Swift：Hello World
来源：http://vk.huixiangedu.cn

print("Hello")
来源：http://su.colortex.cn

[T17] Swift：变量与常量
来源：http://dj.huanxung.cn

var a = 1;  let b = 2
来源：http://jb.huixiangedu.cn

[T18] Swift：字符串插值
来源：http://vq.chemitech.net.cn

"值: \(b)"
来源：http://ji.nszjky.cn

[T19] Swift：可选绑定
来源：http://ak.bookmarksfly.cn

if let n = opt { print(n) }
来源：http://az.huixinmuqiang.cn

[T20] Swift：数组操作
来源：http://hg.wgjwhj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://py.nicolike.cn

[T21] Swift：遍历
来源：http://th.hnjuh.cn

for x in a { print(x) }
来源：http://mi.shxzukj.cn

[T22] Swift：字典
来源：http://ss.huanxung.cn

var d = ["a": 1];  d["b"] = 2
来源：http://re.huixiangedu.cn

[T23] Swift：函数
来源：http://ll.gzmigu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gl.521024.cn

[T24] Swift：闭包
来源：http://jj.hnjuh.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ha.haigaiapp.cn

[T25] Swift：结构体
来源：http://gn.huixinmuqiang.cn

struct P { var x: Int }
来源：http://hl.nszjky.cn

[T26] Swift：类与重写
来源：http://ib.huanxung.cn

class A: Base { override func f() {} }
来源：http://yp.asd995.cn

[T27] Swift：错误处理
来源：http://gj.szsharing.cn

do { try f() } catch { print(error) }
来源：http://ng.nszjky.cn

[T28] Swift：枚举
来源：http://tn.asd995.cn

enum Color { case red, green }
来源：http://vs.bjjhwx.cn

[T29] Swift：guard 提前返回
来源：http://ij.nszjky.cn

guard let x = opt else { return }
来源：http://ji.hahajie.cn

[T30] Swift：协议
来源：http://hu.chemitech.net.cn

protocol Shape { func area() -> Double }
来源：http://ac.shxzskj.cn

[T31] Lua：Hello World
来源：http://hv.colortex.cn

print("Hello")
来源：http://xc.bookmarksfly.cn

[T32] Lua：局部变量
来源：http://ze.521024.cn

local a = 1
来源：http://nh.newstarts.cn

[T33] Lua：表（数组）
来源：http://mk.nicolike.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zi.bjjhwx.cn

[T34] Lua：遍历表
来源：http://ij.521024.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://yh.szxytkj.cn

[T35] Lua：字典表
来源：http://lw.chemitech.net.cn

local d = { a = 1 };  d.b = 2
来源：http://kn.yuexingan06.cn

[T36] Lua：函数
来源：http://nm.521024.cn

function add(a, b) return a + b end
来源：http://kq.jianghongdianzi.cn

[T37] Lua：字符串拼接
来源：http://lt.wgjwhj.cn

"a" .. "b"
来源：http://hx.asd995.cn

[T38] Lua：条件
来源：http://zz.shxzskj.cn

if x > 0 then print("正") end
来源：http://al.hahajie.cn

[T39] Lua：模式匹配
来源：http://ux.haigaiapp.cn

string.find(s, "%d+")
来源：http://my.szsharing.cn

[T40] Lua：元表
来源：http://cn.shtwfgs.cn

setmetatable({}, { __index = base })
来源：http://zk.bookmarksfly.cn

[T41] Perl：Hello World
来源：http://az.szxytkj.cn

print "Hello\n";
来源：http://dh.yuntaijiaju.cn

[T42] Perl：变量类型
来源：http://rx.jctech888.com.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dy.nszjky.cn

[T43] Perl：字符串插值
来源：http://rs.asd995.cn

"值: $a"
来源：http://oj.huixinmuqiang.cn

[T44] Perl：条件
来源：http://ws.wgjwhj.cn

if ($a > 0) { print "正"; }
来源：http://zg.panjiajie.cn

[T45] Perl：数组遍历
来源：http://de.yuexingan06.cn

for my $x (@arr) { print $x; }
来源：http://ds.huanxung.cn

[T46] Perl：哈希操作
来源：http://ky.huixiangedu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wo.asd995.cn

[T47] Perl：正则捕获
来源：http://ig.colortex.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ul.shtwfgs.cn

[T48] Perl：正则替换
来源：http://wi.newstarts.cn

$s =~ s/old/new/g;
来源：http://dr.huixiangedu.cn

[T49] Perl：函数
来源：http://bu.panjiajie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kh.9csxet.cn

[T50] Perl：逐行读文件
来源：http://zm.hahajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xn.yuexingan06.cn

while (my $line = <$fh>) { print $line; }
来源：http://mi.shxzskj.cn

[T51] Scala：Hello World
来源：http://ph.521024.cn

println("Hello")
来源：http://el.huixinmuqiang.cn

[T52] Scala：变量
来源：http://ph.huixinmuqiang.cn

val a = 1;  var b = 2
来源：http://vm.huixinmuqiang.cn

[T53] Scala：字符串插值
来源：http://pr.jianghongdianzi.cn

s"值: $b"
来源：http://ic.szxytkj.cn

[T54] Scala：集合映射
来源：http://xi.shxzukj.cn

List(1, 2, 3).map(_ * 2)
来源：http://yj.lnxyls.cn

[T55] Scala：集合过滤
来源：http://hu.szxytkj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gi.shtwfgs.cn

[T56] Scala：样例类
来源：http://hk.haigaiapp.cn

case class User(name: String, age: Int)
来源：http://ng.yuntaijiaju.cn

[T57] Scala：模式匹配
来源：http://ss.lnxyls.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://sl.9csxet.cn

[T58] Scala：函数定义
来源：http://ch.bjjhwx.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bi.colortex.cn

[T59] Scala：循环
来源：http://uj.szsharing.cn

for (i <- 1 to 10) println(i)
来源：http://ot.hnjuh.cn

[T60] Scala：折叠
来源：http://vg.newstarts.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vs.bookmarksfly.cn

================================================================================
来源：http://bk.lnxyls.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zn.lnxyls.cn

================================================================================
来源：http://in.9csxet.cn

[U01] Py：创建虚拟环境
来源：http://fh.gzmigu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vr.huixiangedu.cn

[U02] Py：导出 / 安装依赖
来源：http://cm.szsharing.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wq.bookmarksfly.cn

[U03] Py：加载 .env 配置
来源：http://an.yuexingan06.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://lt.szsharing.cn

[U04] Py：变量调试打印
来源：http://iy.asd995.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nk.huixiangedu.cn

[U05] Py：列表去重且保序
来源：http://jn.huixinmuqiang.cn

list(dict.fromkeys(arr))
来源：http://ut.haigaiapp.cn

[U06] Py：合并两个字典
来源：http://bv.szxytkj.cn

{**a, **b}
来源：http://yw.521024.cn

[U07] Py：反转字典键值
来源：http://je.9csxet.cn

{v: k for k, v in d.items()}
来源：http://kb.panjiajie.cn

[U08] Py：展平二维列表
来源：http://kp.newstarts.cn

[y for x in nested for y in x]
来源：http://al.9csxet.cn

[U09] Py：字典取最大值的键
来源：http://qt.huixiangedu.cn

max(d, key=d.get)
来源：http://fl.521024.cn

[U10] Py：按值排序字典
来源：http://lp.szxytkj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bs.panjiajie.cn

[U11] Py：生成器表达式
来源：http://ts.nicolike.cn

(x * 2 for x in arr)
来源：http://vj.9csxet.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rf.jctech888.com.cn

Counter(arr).most_common(3)
来源：http://qd.colortex.cn

[U13] Py：固定长度队列
来源：http://ho.nicolike.cn

deque(maxlen=10)
来源：http://hj.szxytkj.cn

[U14] Py：分组收集到列表
来源：http://xi.hahajie.cn

defaultdict(list)
来源：http://qb.jianghongdianzi.cn

[U15] Py：高精度计时
来源：http://ts.asd995.cn

t = time.perf_counter()
来源：http://fc.szxytkj.cn

[U16] Py：命令行参数解析
来源：http://ee.bjjhwx.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://aw.szsharing.cn

[U17] Py：初始化日志
来源：http://gu.yuexingan06.cn

logging.basicConfig(level=logging.INFO)
来源：http://pm.szxytkj.cn

[U18] Py：预编译正则
来源：http://ic.colortex.cn

pat = re.compile(r"\d+")
来源：http://vd.asd995.cn

[U19] Py：正则替换带回调
来源：http://nn.bjjhwx.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jj.hahajie.cn

[U20] Py：缓存函数结果
来源：http://li.bjjhwx.cn

@functools.lru_cache(maxsize=None)
来源：http://dp.huixiangedu.cn

[U21] Py：自定义上下文管理器
来源：http://fz.gzmigu.cn

@contextlib.contextmanager
来源：http://ie.shxzukj.cn

[U22] Py：矩阵转置
来源：http://lh.521024.cn

list(zip(*m))
来源：http://ha.asd995.cn

[U23] Py：分块读取大文件
来源：http://rf.colortex.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://oi.yuntaijiaju.cn

[U24] Py：路径操作
来源：http://zu.chemitech.net.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wq.huixinmuqiang.cn

[U25] Py：CSV 按字典读
来源：http://qd.wgjwhj.cn

csv.DictReader(f)
来源：http://bl.hahajie.cn

[U26] Py：并发下载
来源：http://hm.lnxyls.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tu.hnjuh.cn

[U27] Py：异步 HTTP
来源：http://zy.521024.cn

aiohttp.ClientSession() 配合 async with
来源：http://un.szsharing.cn

[U28] Py：类型别名
来源：http://qp.shxzskj.cn

UserId = int
来源：http://sb.chemitech.net.cn

[U29] Py：属性校验
来源：http://zz.yuexingan06.cn

@property 与 @x.setter 配合
来源：http://zy.chemitech.net.cn

[U30] Py：数据类
来源：http://qq.muxihuayi.cn

@dataclass(slots=True)
来源：http://xc.bookmarksfly.cn

[U31] Py：单测
来源：http://cl.gzmigu.cn

python -m pytest -q
来源：http://ie.wgjwhj.cn

[U32] Py：代码格式化
来源：http://fw.szxytkj.cn

ruff format . && ruff check --fix .
来源：http://hr.yuntaijiaju.cn

[U33] Py：打包发布
来源：http://uq.asd995.cn

python -m build  （依赖 pyproject.toml）
来源：http://lt.nszjky.cn

[U34] Py：判断编码
来源：http://rn.szxytkj.cn

chardet.detect(raw)
来源：http://gf.asd995.cn

[U35] Py：发送邮件
来源：http://kz.huixinmuqiang.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pm.huixiangedu.cn

[U36] Py：定时任务
来源：http://cs.szxytkj.cn

schedule.every(10).minutes.do(job)
来源：http://wx.panjiajie.cn

[U37] Py：读写 Excel
来源：http://qw.szxytkj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ej.nicolike.cn

[U38] Py：获取脚本所在目录
来源：http://tk.huixiangedu.cn

Path(__file__).resolve().parent
来源：http://jg.wgjwhj.cn

[U39] Py：判断是否在交互环境
来源：http://to.colortex.cn

sys.stdout.isatty()
来源：http://pe.asd995.cn

[U40] Py：打印到标准错误
来源：http://rq.newstarts.cn

print("err", file=sys.stderr)
来源：http://dv.haigaiapp.cn

[U41] PHP：初始化 Composer 项目
来源：http://lq.muxihuayi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://lr.wgjwhj.cn

[U42] PHP：PSR-4 自动加载
来源：http://tf.jctech888.com.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wr.shxzskj.cn

[U43] PHP：声明命名空间
来源：http://zn.gzmigu.cn

namespace App\Http;
来源：http://jy.asd995.cn

[U44] PHP：开启严格类型
来源：http://kc.shxzukj.cn

declare(strict_types=1);
来源：http://bv.nicolike.cn

[U45] PHP：类型声明与返回类型
来源：http://bv.bookmarksfly.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://mc.panjiajie.cn

[U46] PHP：可空类型
来源：http://wt.jctech888.com.cn

?string $name = null
来源：http://vv.521024.cn

[U47] PHP：联合类型
来源：http://hl.chemitech.net.cn

int|string $id
来源：http://nb.hahajie.cn

[U48] PHP：纯枚举
来源：http://qc.haigaiapp.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://uc.9csxet.cn

[U49] PHP：只读属性
来源：http://yz.bjjhwx.cn

public readonly string $name
来源：http://mz.yuexingan06.cn

[U50] PHP：构造器属性提升
来源：http://hi.szxytkj.cn

public function __construct(private int $id) {}
来源：http://rx.asd995.cn

[U51] PHP：数组解构
来源：http://df.521024.cn

[$a, $b] = $arr;
来源：http://sl.gzmigu.cn

[U52] PHP：箭头函数
来源：http://pu.nicolike.cn

$double = fn($x) => $x * 2;
来源：http://sn.huixiangedu.cn

[U53] PHP：空合并运算符
来源：http://lj.hnjuh.cn

$v = $a ?? $b ?? "default";
来源：http://fe.szsharing.cn

[U54] PHP：空安全调用
来源：http://tw.newstarts.cn

$obj?->method()
来源：http://ua.bjjhwx.cn

[U55] PHP：match 表达式
来源：http://bn.yuntaijiaju.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uy.nicolike.cn

[U56] PHP：命名参数
来源：http://vs.huixiangedu.cn

f(a: 1, b: 2)
来源：http://az.shtwfgs.cn

[U57] PHP：字符串插值
来源：http://uo.lnxyls.cn

"值: {$a}"
来源：http://jj.jctech888.com.cn

[U58] PHP：数组三件套
来源：http://me.huixiangedu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yi.colortex.cn

[U59] PHP：自定义排序
来源：http://tk.9csxet.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ay.huanxung.cn

[U60] PHP：JSON 编解码
来源：http://yg.jianghongdianzi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fz.panjiajie.cn

[U61] PHP：正则
来源：http://ee.jianghongdianzi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ru.nszjky.cn

[U62] PHP：日期对象
来源：http://pf.chemitech.net.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://oe.yuntaijiaju.cn

[U63] PHP：文件读写
来源：http://mm.colortex.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ap.szxytkj.cn

[U64] PHP：目录遍历
来源：http://yf.bookmarksfly.cn

glob("dir/*.php");  scandir("dir");
来源：http://lu.newstarts.cn

[U65] PHP：会话
来源：http://fv.huixiangedu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vm.muxihuayi.cn

[U66] PHP：设置 Cookie
来源：http://ut.jctech888.com.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yn.jctech888.com.cn

[U67] PHP：处理文件上传
来源：http://qq.panjiajie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tp.gzmigu.cn

[U68] PHP：PDO 连接
来源：http://lc.nszjky.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yy.jctech888.com.cn

[U69] PHP：PDO 预处理
来源：http://th.bjjhwx.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mv.bjjhwx.cn

[U70] PHP：PDO 事务
来源：http://nj.bookmarksfly.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cx.asd995.cn

[U71] PHP：抛出异常
来源：http://gw.shxzskj.cn

throw new RuntimeException("失败", 500);
来源：http://th.hahajie.cn

[U72] PHP：写错误日志
来源：http://af.chemitech.net.cn

error_log("失败: " . $e->getMessage());
来源：http://uq.yuexingan06.cn

[U73] PHP：读取 ini 配置
来源：http://qe.huixiangedu.cn

parse_ini_file("config.ini", true)
来源：http://gu.haigaiapp.cn

[U74] PHP：读取环境变量
来源：http://mb.huixiangedu.cn

getenv("APP_ENV") ?: "production"
来源：http://lx.nszjky.cn

[U75] PHP：依赖注入
来源：http://tk.szxytkj.cn

composer require psr/container
来源：http://zl.yuexingan06.cn

[U76] PHP：简单路由
来源：http://hc.9csxet.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://us.yuntaijiaju.cn

[U77] PHP：模板渲染
来源：http://uv.521024.cn

composer require twig/twig
来源：http://hm.bjjhwx.cn

[U78] PHP：单元测试
来源：http://kl.szsharing.cn

composer require --dev phpunit/phpunit
来源：http://zo.hahajie.cn

[U79] PHP：静态分析
来源：http://bv.nicolike.cn

composer require --dev phpstan/phpstan
来源：http://el.szxytkj.cn

[U80] PHP：代码规范修复
来源：http://kx.jianghongdianzi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://bz.yuntaijiaju.cn

[U81] JS：初始化项目
来源：http://gf.jctech888.com.cn

npm init -y;  npm i express
来源：http://pd.9csxet.cn

[U82] JS：package.json 脚本
来源：http://ds.shtwfgs.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ut.yuntaijiaju.cn

[U83] JS：ES Module 导入导出
来源：http://oy.shxzukj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://hy.bookmarksfly.cn

[U84] JS：CommonJS 写法
来源：http://dy.bookmarksfly.cn

module.exports = { a };  const { a } = require("./m");
来源：http://qo.hnjuh.cn

[U85] JS：可选链
来源：http://ay.jianghongdianzi.cn

a?.b?.c
来源：http://co.gzmigu.cn

[U86] JS：空值合并
来源：http://nm.panjiajie.cn

a ?? b
来源：http://qm.gzmigu.cn

[U87] JS：解构默认值
来源：http://az.panjiajie.cn

const { a = 1, b = 2 } = obj;
来源：http://yf.yuntaijiaju.cn

[U88] JS：对象展开合并
来源：http://xt.shtwfgs.cn

{ ...a, ...b }
来源：http://wf.yuntaijiaju.cn

[U89] JS：数组去重
来源：http://mr.9csxet.cn

[...new Set(arr)]
来源：http://rj.asd995.cn

[U90] JS：数字数组排序
来源：http://dx.hahajie.cn

[...arr].sort((a, b) => a - b)
来源：http://xl.huixinmuqiang.cn


<!-- 参考信息 -->