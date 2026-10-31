代发 wailian999

[T07] Kotlin：集合过滤
来源：http://qu.521024.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://yx.szsharing.cn

[T08] Kotlin：数据类
来源：http://nx.jianghongdianzi.cn

data class User(val name: String, val age: Int)
来源：http://qf.szxytkj.cn

[T09] Kotlin：扩展函数
来源：http://pl.szsharing.cn

fun String.exclaim() = this + "!"
来源：http://ir.521024.cn

[T10] Kotlin：默认参数
来源：http://mo.hnjuh.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dt.muxihuayi.cn

[T11] Kotlin：协程
来源：http://mi.panjiajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wj.9csxet.cn

[T12] Kotlin：解构声明
来源：http://cr.shxzukj.cn

val (a, b) = Pair(1, 2)
来源：http://cq.yuntaijiaju.cn

[T13] Kotlin：只读 Map
来源：http://og.nicolike.cn

val m = mapOf("a" to 1)
来源：http://dx.chemitech.net.cn

[T14] Kotlin：循环
来源：http://xf.muxihuayi.cn

for (i in 1..10) println(i)
来源：http://uu.shxzukj.cn

[T15] Kotlin：接口
来源：http://ko.shxzskj.cn

interface Shape { fun area(): Double }
来源：http://wo.bookmarksfly.cn

[T16] Swift：Hello World
来源：http://ci.muxihuayi.cn

print("Hello")
来源：http://vq.huanxung.cn

[T17] Swift：变量与常量
来源：http://ny.szxytkj.cn

var a = 1;  let b = 2
来源：http://uw.yuntaijiaju.cn

[T18] Swift：字符串插值
来源：http://um.nszjky.cn

"值: \(b)"
来源：http://en.lnxyls.cn

[T19] Swift：可选绑定
来源：http://jy.shtwfgs.cn

if let n = opt { print(n) }
来源：http://zo.chemitech.net.cn

[T20] Swift：数组操作
来源：http://vg.9csxet.cn

var a = [1, 2, 3];  a.append(4)
来源：http://dt.shxzskj.cn

[T21] Swift：遍历
来源：http://lv.jctech888.com.cn

for x in a { print(x) }
来源：http://mb.szsharing.cn

[T22] Swift：字典
来源：http://va.shxzskj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fr.shxzukj.cn

[T23] Swift：函数
来源：http://yy.szxytkj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ib.huanxung.cn

[T24] Swift：闭包
来源：http://sa.huixiangedu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://fi.colortex.cn

[T25] Swift：结构体
来源：http://qz.szxytkj.cn

struct P { var x: Int }
来源：http://cq.nicolike.cn

[T26] Swift：类与重写
来源：http://jd.szsharing.cn

class A: Base { override func f() {} }
来源：http://ww.asd995.cn

[T27] Swift：错误处理
来源：http://bk.szxytkj.cn

do { try f() } catch { print(error) }
来源：http://be.nszjky.cn

[T28] Swift：枚举
来源：http://mw.yuntaijiaju.cn

enum Color { case red, green }
来源：http://mg.chemitech.net.cn

[T29] Swift：guard 提前返回
来源：http://de.hnjuh.cn

guard let x = opt else { return }
来源：http://ps.yuntaijiaju.cn

[T30] Swift：协议
来源：http://kj.yuntaijiaju.cn

protocol Shape { func area() -> Double }
来源：http://mw.shxzukj.cn

[T31] Lua：Hello World
来源：http://sp.jctech888.com.cn

print("Hello")
来源：http://zc.lnxyls.cn

[T32] Lua：局部变量
来源：http://kw.colortex.cn

local a = 1
来源：http://se.shtwfgs.cn

[T33] Lua：表（数组）
来源：http://pp.wgjwhj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://pj.huanxung.cn

[T34] Lua：遍历表
来源：http://wz.521024.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ng.nicolike.cn

[T35] Lua：字典表
来源：http://us.shxzskj.cn

local d = { a = 1 };  d.b = 2
来源：http://jv.shxzukj.cn

[T36] Lua：函数
来源：http://co.gzmigu.cn

function add(a, b) return a + b end
来源：http://vb.panjiajie.cn

[T37] Lua：字符串拼接
来源：http://kn.panjiajie.cn

"a" .. "b"
来源：http://as.yuexingan06.cn

[T38] Lua：条件
来源：http://yk.huanxung.cn

if x > 0 then print("正") end
来源：http://bq.colortex.cn

[T39] Lua：模式匹配
来源：http://yn.shtwfgs.cn

string.find(s, "%d+")
来源：http://sq.huixinmuqiang.cn

[T40] Lua：元表
来源：http://jz.hahajie.cn

setmetatable({}, { __index = base })
来源：http://mr.szsharing.cn

[T41] Perl：Hello World
来源：http://gb.nicolike.cn

print "Hello\n";
来源：http://yy.hahajie.cn

[T42] Perl：变量类型
来源：http://qm.newstarts.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sz.panjiajie.cn

[T43] Perl：字符串插值
来源：http://xm.huixinmuqiang.cn

"值: $a"
来源：http://to.jianghongdianzi.cn

[T44] Perl：条件
来源：http://xb.panjiajie.cn

if ($a > 0) { print "正"; }
来源：http://co.huanxung.cn

[T45] Perl：数组遍历
来源：http://xr.hahajie.cn

for my $x (@arr) { print $x; }
来源：http://bi.newstarts.cn

[T46] Perl：哈希操作
来源：http://gy.jctech888.com.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fq.asd995.cn

[T47] Perl：正则捕获
来源：http://ll.haigaiapp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vp.huanxung.cn

[T48] Perl：正则替换
来源：http://pr.gzmigu.cn

$s =~ s/old/new/g;
来源：http://zy.nszjky.cn

[T49] Perl：函数
来源：http://tf.hnjuh.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gq.muxihuayi.cn

[T50] Perl：逐行读文件
来源：http://hd.colortex.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zh.haigaiapp.cn

while (my $line = <$fh>) { print $line; }
来源：http://ik.huanxung.cn

[T51] Scala：Hello World
来源：http://pg.chemitech.net.cn

println("Hello")
来源：http://pn.9csxet.cn

[T52] Scala：变量
来源：http://yw.521024.cn

val a = 1;  var b = 2
来源：http://mc.hnjuh.cn

[T53] Scala：字符串插值
来源：http://ll.bookmarksfly.cn

s"值: $b"
来源：http://xv.jctech888.com.cn

[T54] Scala：集合映射
来源：http://id.szxytkj.cn

List(1, 2, 3).map(_ * 2)
来源：http://be.gzmigu.cn

[T55] Scala：集合过滤
来源：http://wu.jctech888.com.cn

List(1, 2, 3).filter(_ > 1)
来源：http://hw.jctech888.com.cn

[T56] Scala：样例类
来源：http://dc.asd995.cn

case class User(name: String, age: Int)
来源：http://et.nszjky.cn

[T57] Scala：模式匹配
来源：http://el.wgjwhj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://zg.szxytkj.cn

[T58] Scala：函数定义
来源：http://eq.nicolike.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wu.szxytkj.cn

[T59] Scala：循环
来源：http://mt.asd995.cn

for (i <- 1 to 10) println(i)
来源：http://rd.muxihuayi.cn

[T60] Scala：折叠
来源：http://ob.newstarts.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pi.huixinmuqiang.cn

================================================================================
来源：http://lu.szxytkj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pn.huixinmuqiang.cn

================================================================================
来源：http://ja.huanxung.cn

[U01] Py：创建虚拟环境
来源：http://va.jianghongdianzi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://tm.huixiangedu.cn

[U02] Py：导出 / 安装依赖
来源：http://jc.shxzukj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hh.shxzskj.cn

[U03] Py：加载 .env 配置
来源：http://kk.9csxet.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://oh.wgjwhj.cn

[U04] Py：变量调试打印
来源：http://pt.yuntaijiaju.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vi.szsharing.cn

[U05] Py：列表去重且保序
来源：http://kb.hahajie.cn

list(dict.fromkeys(arr))
来源：http://tk.gzmigu.cn

[U06] Py：合并两个字典
来源：http://zw.huixiangedu.cn

{**a, **b}
来源：http://bm.panjiajie.cn

[U07] Py：反转字典键值
来源：http://zk.lnxyls.cn

{v: k for k, v in d.items()}
来源：http://ci.nicolike.cn

[U08] Py：展平二维列表
来源：http://ru.gzmigu.cn

[y for x in nested for y in x]
来源：http://ft.hahajie.cn

[U09] Py：字典取最大值的键
来源：http://cv.nicolike.cn

max(d, key=d.get)
来源：http://nf.wgjwhj.cn

[U10] Py：按值排序字典
来源：http://th.nicolike.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qo.huixinmuqiang.cn

[U11] Py：生成器表达式
来源：http://ms.muxihuayi.cn

(x * 2 for x in arr)
来源：http://dg.521024.cn

[U12] Py：取出现最多的 3 个元素
来源：http://px.muxihuayi.cn

Counter(arr).most_common(3)
来源：http://ex.521024.cn

[U13] Py：固定长度队列
来源：http://rw.bjjhwx.cn

deque(maxlen=10)
来源：http://rb.shtwfgs.cn

[U14] Py：分组收集到列表
来源：http://uc.nszjky.cn

defaultdict(list)
来源：http://rl.shtwfgs.cn

[U15] Py：高精度计时
来源：http://vb.asd995.cn

t = time.perf_counter()
来源：http://ib.nicolike.cn

[U16] Py：命令行参数解析
来源：http://bx.jctech888.com.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fq.521024.cn

[U17] Py：初始化日志
来源：http://xn.nszjky.cn

logging.basicConfig(level=logging.INFO)
来源：http://kg.nszjky.cn

[U18] Py：预编译正则
来源：http://ne.jianghongdianzi.cn

pat = re.compile(r"\d+")
来源：http://uq.bookmarksfly.cn

[U19] Py：正则替换带回调
来源：http://xw.newstarts.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://uu.gzmigu.cn

[U20] Py：缓存函数结果
来源：http://vu.haigaiapp.cn

@functools.lru_cache(maxsize=None)
来源：http://rw.shtwfgs.cn

[U21] Py：自定义上下文管理器
来源：http://fs.shtwfgs.cn

@contextlib.contextmanager
来源：http://sk.huixinmuqiang.cn

[U22] Py：矩阵转置
来源：http://np.huixiangedu.cn

list(zip(*m))
来源：http://jh.lnxyls.cn

[U23] Py：分块读取大文件
来源：http://qr.9csxet.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ty.gzmigu.cn

[U24] Py：路径操作
来源：http://ss.nszjky.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fg.hnjuh.cn

[U25] Py：CSV 按字典读
来源：http://ms.bjjhwx.cn

csv.DictReader(f)
来源：http://ei.gzmigu.cn

[U26] Py：并发下载
来源：http://ts.muxihuayi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://po.gzmigu.cn

[U27] Py：异步 HTTP
来源：http://gi.colortex.cn

aiohttp.ClientSession() 配合 async with
来源：http://kt.panjiajie.cn

[U28] Py：类型别名
来源：http://nc.nszjky.cn

UserId = int
来源：http://pw.szsharing.cn

[U29] Py：属性校验
来源：http://vs.521024.cn

@property 与 @x.setter 配合
来源：http://bc.chemitech.net.cn

[U30] Py：数据类
来源：http://nc.huanxung.cn

@dataclass(slots=True)
来源：http://sn.nicolike.cn

[U31] Py：单测
来源：http://hy.shxzukj.cn

python -m pytest -q
来源：http://ya.shxzskj.cn

[U32] Py：代码格式化
来源：http://aq.lnxyls.cn

ruff format . && ruff check --fix .
来源：http://cw.colortex.cn

[U33] Py：打包发布
来源：http://op.huanxung.cn

python -m build  （依赖 pyproject.toml）
来源：http://sc.yuexingan06.cn

[U34] Py：判断编码
来源：http://pa.huixinmuqiang.cn

chardet.detect(raw)
来源：http://pi.gzmigu.cn

[U35] Py：发送邮件
来源：http://he.shtwfgs.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pf.nszjky.cn

[U36] Py：定时任务
来源：http://kd.szsharing.cn

schedule.every(10).minutes.do(job)
来源：http://fi.haigaiapp.cn

[U37] Py：读写 Excel
来源：http://da.yuexingan06.cn

pandas.read_excel / DataFrame.to_excel
来源：http://it.gzmigu.cn

[U38] Py：获取脚本所在目录
来源：http://ki.521024.cn

Path(__file__).resolve().parent
来源：http://rv.newstarts.cn

[U39] Py：判断是否在交互环境
来源：http://pn.muxihuayi.cn

sys.stdout.isatty()
来源：http://yt.chemitech.net.cn

[U40] Py：打印到标准错误
来源：http://oi.haigaiapp.cn

print("err", file=sys.stderr)
来源：http://vu.hahajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://wa.szxytkj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://tn.hahajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://bg.colortex.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ps.szsharing.cn

[U43] PHP：声明命名空间
来源：http://cr.bookmarksfly.cn

namespace App\Http;
来源：http://vt.jctech888.com.cn

[U44] PHP：开启严格类型
来源：http://vm.9csxet.cn

declare(strict_types=1);
来源：http://qw.huanxung.cn

[U45] PHP：类型声明与返回类型
来源：http://ou.huixiangedu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://yw.huixiangedu.cn

[U46] PHP：可空类型
来源：http://fq.jctech888.com.cn

?string $name = null
来源：http://cr.521024.cn

[U47] PHP：联合类型
来源：http://ss.wgjwhj.cn

int|string $id
来源：http://fy.newstarts.cn

[U48] PHP：纯枚举
来源：http://mx.shtwfgs.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mx.jctech888.com.cn

[U49] PHP：只读属性
来源：http://ak.shxzskj.cn

public readonly string $name
来源：http://rp.panjiajie.cn

[U50] PHP：构造器属性提升
来源：http://sv.gzmigu.cn

public function __construct(private int $id) {}
来源：http://pl.lnxyls.cn

[U51] PHP：数组解构
来源：http://xz.huixiangedu.cn

[$a, $b] = $arr;
来源：http://pe.yuexingan06.cn

[U52] PHP：箭头函数
来源：http://kp.bjjhwx.cn

$double = fn($x) => $x * 2;
来源：http://ge.szsharing.cn

[U53] PHP：空合并运算符
来源：http://ou.asd995.cn

$v = $a ?? $b ?? "default";
来源：http://cx.huixiangedu.cn

[U54] PHP：空安全调用
来源：http://gj.shxzukj.cn

$obj?->method()
来源：http://jp.shxzukj.cn

[U55] PHP：match 表达式
来源：http://ej.muxihuayi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ym.521024.cn

[U56] PHP：命名参数
来源：http://ji.jianghongdianzi.cn

f(a: 1, b: 2)
来源：http://oj.521024.cn

[U57] PHP：字符串插值
来源：http://bv.hnjuh.cn

"值: {$a}"
来源：http://wz.muxihuayi.cn

[U58] PHP：数组三件套
来源：http://xd.panjiajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kc.nszjky.cn

[U59] PHP：自定义排序
来源：http://fk.jianghongdianzi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pt.521024.cn

[U60] PHP：JSON 编解码
来源：http://oq.521024.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bg.jianghongdianzi.cn

[U61] PHP：正则
来源：http://ma.jctech888.com.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pi.lnxyls.cn

[U62] PHP：日期对象
来源：http://wd.yuexingan06.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ic.shxzukj.cn

[U63] PHP：文件读写
来源：http://nk.jctech888.com.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://us.hahajie.cn

[U64] PHP：目录遍历
来源：http://xj.newstarts.cn

glob("dir/*.php");  scandir("dir");
来源：http://yp.bookmarksfly.cn

[U65] PHP：会话
来源：http://cu.nicolike.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://zc.shxzskj.cn

[U66] PHP：设置 Cookie
来源：http://ay.jctech888.com.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sy.colortex.cn

[U67] PHP：处理文件上传
来源：http://ed.asd995.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ux.bjjhwx.cn

[U68] PHP：PDO 连接
来源：http://yq.chemitech.net.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lh.szsharing.cn

[U69] PHP：PDO 预处理
来源：http://md.yuntaijiaju.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zr.bookmarksfly.cn

[U70] PHP：PDO 事务
来源：http://fx.521024.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xp.szsharing.cn

[U71] PHP：抛出异常
来源：http://nn.chemitech.net.cn

throw new RuntimeException("失败", 500);
来源：http://jh.haigaiapp.cn

[U72] PHP：写错误日志
来源：http://hp.nszjky.cn

error_log("失败: " . $e->getMessage());
来源：http://io.9csxet.cn

[U73] PHP：读取 ini 配置
来源：http://zj.shxzskj.cn

parse_ini_file("config.ini", true)
来源：http://tk.asd995.cn

[U74] PHP：读取环境变量
来源：http://cc.shxzskj.cn

getenv("APP_ENV") ?: "production"
来源：http://ot.9csxet.cn

[U75] PHP：依赖注入
来源：http://tf.yuexingan06.cn

composer require psr/container
来源：http://qx.shtwfgs.cn

[U76] PHP：简单路由
来源：http://wo.lnxyls.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fc.szsharing.cn

[U77] PHP：模板渲染
来源：http://qo.9csxet.cn

composer require twig/twig
来源：http://sx.asd995.cn

[U78] PHP：单元测试
来源：http://fd.huixiangedu.cn

composer require --dev phpunit/phpunit
来源：http://rp.szxytkj.cn

[U79] PHP：静态分析
来源：http://yp.huixiangedu.cn

composer require --dev phpstan/phpstan
来源：http://ei.nszjky.cn

[U80] PHP：代码规范修复
来源：http://vn.huanxung.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://wl.bjjhwx.cn

[U81] JS：初始化项目
来源：http://xd.jctech888.com.cn

npm init -y;  npm i express
来源：http://re.521024.cn

[U82] JS：package.json 脚本
来源：http://wv.asd995.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://eu.gzmigu.cn

[U83] JS：ES Module 导入导出
来源：http://ub.gzmigu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://sf.yuexingan06.cn

[U84] JS：CommonJS 写法
来源：http://uc.jianghongdianzi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://nh.haigaiapp.cn

[U85] JS：可选链
来源：http://rh.shxzskj.cn

a?.b?.c
来源：http://ih.hnjuh.cn

[U86] JS：空值合并
来源：http://nv.lnxyls.cn

a ?? b
来源：http://zo.nszjky.cn

[U87] JS：解构默认值
来源：http://qk.chemitech.net.cn

const { a = 1, b = 2 } = obj;
来源：http://tc.nicolike.cn

[U88] JS：对象展开合并
来源：http://bg.panjiajie.cn

{ ...a, ...b }
来源：http://zb.panjiajie.cn

[U89] JS：数组去重
来源：http://ml.haigaiapp.cn

[...new Set(arr)]
来源：http://ui.szsharing.cn

[U90] JS：数字数组排序
来源：http://uf.wgjwhj.cn

[...arr].sort((a, b) => a - b)
来源：http://tj.muxihuayi.cn

[U91] JS：对象键值遍历
来源：http://zu.huixinmuqiang.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://uu.hahajie.cn

[U92] JS：深拷贝
来源：http://nn.wgjwhj.cn

structuredClone(obj)
来源：http://bw.gzmigu.cn

[U93] JS：模板字符串
来源：http://pq.panjiajie.cn

`共 ${n} 条`
来源：http://ua.521024.cn

[U94] JS：箭头函数
来源：http://bh.hnjuh.cn

const double = x => x * 2;
来源：http://gl.lnxyls.cn


<!-- 参考信息 -->