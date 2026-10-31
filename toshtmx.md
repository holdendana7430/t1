代发 wailian999

[T07] Kotlin：集合过滤
来源：http://ye.bookmarksfly.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ag.colortex.cn

[T08] Kotlin：数据类
来源：http://mv.jctech888.com.cn

data class User(val name: String, val age: Int)
来源：http://kf.9csxet.cn

[T09] Kotlin：扩展函数
来源：http://bb.newstarts.cn

fun String.exclaim() = this + "!"
来源：http://he.hnjuh.cn

[T10] Kotlin：默认参数
来源：http://ks.jianghongdianzi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ky.hnjuh.cn

[T11] Kotlin：协程
来源：http://cd.yuntaijiaju.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ee.asd995.cn

[T12] Kotlin：解构声明
来源：http://av.haigaiapp.cn

val (a, b) = Pair(1, 2)
来源：http://eg.szxytkj.cn

[T13] Kotlin：只读 Map
来源：http://tx.asd995.cn

val m = mapOf("a" to 1)
来源：http://wt.lnxyls.cn

[T14] Kotlin：循环
来源：http://gg.nszjky.cn

for (i in 1..10) println(i)
来源：http://xu.huixiangedu.cn

[T15] Kotlin：接口
来源：http://du.yuexingan06.cn

interface Shape { fun area(): Double }
来源：http://pw.wgjwhj.cn

[T16] Swift：Hello World
来源：http://mk.shtwfgs.cn

print("Hello")
来源：http://nl.shxzukj.cn

[T17] Swift：变量与常量
来源：http://zc.colortex.cn

var a = 1;  let b = 2
来源：http://sh.shxzskj.cn

[T18] Swift：字符串插值
来源：http://cw.shxzukj.cn

"值: \(b)"
来源：http://ly.panjiajie.cn

[T19] Swift：可选绑定
来源：http://di.huixiangedu.cn

if let n = opt { print(n) }
来源：http://rh.nicolike.cn

[T20] Swift：数组操作
来源：http://db.lnxyls.cn

var a = [1, 2, 3];  a.append(4)
来源：http://cv.asd995.cn

[T21] Swift：遍历
来源：http://sm.shxzukj.cn

for x in a { print(x) }
来源：http://wn.huixinmuqiang.cn

[T22] Swift：字典
来源：http://em.shtwfgs.cn

var d = ["a": 1];  d["b"] = 2
来源：http://bn.nicolike.cn

[T23] Swift：函数
来源：http://vl.huanxung.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pi.jianghongdianzi.cn

[T24] Swift：闭包
来源：http://ff.asd995.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://dr.shxzukj.cn

[T25] Swift：结构体
来源：http://mn.lnxyls.cn

struct P { var x: Int }
来源：http://dg.newstarts.cn

[T26] Swift：类与重写
来源：http://au.hnjuh.cn

class A: Base { override func f() {} }
来源：http://ep.jctech888.com.cn

[T27] Swift：错误处理
来源：http://mg.hahajie.cn

do { try f() } catch { print(error) }
来源：http://kp.shxzukj.cn

[T28] Swift：枚举
来源：http://qu.nszjky.cn

enum Color { case red, green }
来源：http://xo.huixiangedu.cn

[T29] Swift：guard 提前返回
来源：http://nn.hahajie.cn

guard let x = opt else { return }
来源：http://pg.hnjuh.cn

[T30] Swift：协议
来源：http://tu.bookmarksfly.cn

protocol Shape { func area() -> Double }
来源：http://km.asd995.cn

[T31] Lua：Hello World
来源：http://km.szsharing.cn

print("Hello")
来源：http://qm.asd995.cn

[T32] Lua：局部变量
来源：http://on.yuntaijiaju.cn

local a = 1
来源：http://fz.bjjhwx.cn

[T33] Lua：表（数组）
来源：http://vs.gzmigu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ck.shxzukj.cn

[T34] Lua：遍历表
来源：http://hz.szsharing.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ah.nicolike.cn

[T35] Lua：字典表
来源：http://qa.huixiangedu.cn

local d = { a = 1 };  d.b = 2
来源：http://dv.szsharing.cn

[T36] Lua：函数
来源：http://fs.chemitech.net.cn

function add(a, b) return a + b end
来源：http://rw.yuexingan06.cn

[T37] Lua：字符串拼接
来源：http://oh.lnxyls.cn

"a" .. "b"
来源：http://qq.wgjwhj.cn

[T38] Lua：条件
来源：http://ps.jctech888.com.cn

if x > 0 then print("正") end
来源：http://ce.yuntaijiaju.cn

[T39] Lua：模式匹配
来源：http://qa.lnxyls.cn

string.find(s, "%d+")
来源：http://gv.9csxet.cn

[T40] Lua：元表
来源：http://gr.jctech888.com.cn

setmetatable({}, { __index = base })
来源：http://sy.jianghongdianzi.cn

[T41] Perl：Hello World
来源：http://rj.muxihuayi.cn

print "Hello\n";
来源：http://lu.colortex.cn

[T42] Perl：变量类型
来源：http://pi.newstarts.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gd.panjiajie.cn

[T43] Perl：字符串插值
来源：http://xa.gzmigu.cn

"值: $a"
来源：http://qg.colortex.cn

[T44] Perl：条件
来源：http://lj.wgjwhj.cn

if ($a > 0) { print "正"; }
来源：http://az.colortex.cn

[T45] Perl：数组遍历
来源：http://sq.asd995.cn

for my $x (@arr) { print $x; }
来源：http://pt.521024.cn

[T46] Perl：哈希操作
来源：http://bq.yuexingan06.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pi.shxzskj.cn

[T47] Perl：正则捕获
来源：http://gy.huixiangedu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://zy.lnxyls.cn

[T48] Perl：正则替换
来源：http://oy.yuntaijiaju.cn

$s =~ s/old/new/g;
来源：http://kv.colortex.cn

[T49] Perl：函数
来源：http://ey.shxzskj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xd.lnxyls.cn

[T50] Perl：逐行读文件
来源：http://ks.bjjhwx.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fw.bookmarksfly.cn

while (my $line = <$fh>) { print $line; }
来源：http://gz.shxzskj.cn

[T51] Scala：Hello World
来源：http://ys.lnxyls.cn

println("Hello")
来源：http://hl.521024.cn

[T52] Scala：变量
来源：http://gh.wgjwhj.cn

val a = 1;  var b = 2
来源：http://nr.jctech888.com.cn

[T53] Scala：字符串插值
来源：http://ft.nszjky.cn

s"值: $b"
来源：http://ar.chemitech.net.cn

[T54] Scala：集合映射
来源：http://cd.gzmigu.cn

List(1, 2, 3).map(_ * 2)
来源：http://qe.haigaiapp.cn

[T55] Scala：集合过滤
来源：http://cm.szsharing.cn

List(1, 2, 3).filter(_ > 1)
来源：http://iv.newstarts.cn

[T56] Scala：样例类
来源：http://bx.muxihuayi.cn

case class User(name: String, age: Int)
来源：http://mg.gzmigu.cn

[T57] Scala：模式匹配
来源：http://zn.szsharing.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://su.szxytkj.cn

[T58] Scala：函数定义
来源：http://tt.huixinmuqiang.cn

def add(a: Int, b: Int): Int = a + b
来源：http://mr.shxzukj.cn

[T59] Scala：循环
来源：http://tw.asd995.cn

for (i <- 1 to 10) println(i)
来源：http://kf.haigaiapp.cn

[T60] Scala：折叠
来源：http://py.521024.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pd.colortex.cn

================================================================================
来源：http://ev.gzmigu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dp.jctech888.com.cn

================================================================================
来源：http://el.bjjhwx.cn

[U01] Py：创建虚拟环境
来源：http://kh.newstarts.cn

python -m venv .venv && source .venv/bin/activate
来源：http://rk.nicolike.cn

[U02] Py：导出 / 安装依赖
来源：http://gw.bjjhwx.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://td.haigaiapp.cn

[U03] Py：加载 .env 配置
来源：http://bo.jianghongdianzi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ns.huixinmuqiang.cn

[U04] Py：变量调试打印
来源：http://hz.shxzskj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yuexingan06.cn

[U05] Py：列表去重且保序
来源：http://zw.szxytkj.cn

list(dict.fromkeys(arr))
来源：http://st.shxzskj.cn

[U06] Py：合并两个字典
来源：http://vn.jianghongdianzi.cn

{**a, **b}
来源：http://or.bookmarksfly.cn

[U07] Py：反转字典键值
来源：http://qn.huixinmuqiang.cn

{v: k for k, v in d.items()}
来源：http://am.gzmigu.cn

[U08] Py：展平二维列表
来源：http://ij.gzmigu.cn

[y for x in nested for y in x]
来源：http://pu.lnxyls.cn

[U09] Py：字典取最大值的键
来源：http://cu.panjiajie.cn

max(d, key=d.get)
来源：http://fr.hahajie.cn

[U10] Py：按值排序字典
来源：http://qk.szxytkj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fv.muxihuayi.cn

[U11] Py：生成器表达式
来源：http://in.colortex.cn

(x * 2 for x in arr)
来源：http://pl.yuntaijiaju.cn

[U12] Py：取出现最多的 3 个元素
来源：http://bh.asd995.cn

Counter(arr).most_common(3)
来源：http://ov.newstarts.cn

[U13] Py：固定长度队列
来源：http://yq.newstarts.cn

deque(maxlen=10)
来源：http://to.521024.cn

[U14] Py：分组收集到列表
来源：http://do.szsharing.cn

defaultdict(list)
来源：http://jz.9csxet.cn

[U15] Py：高精度计时
来源：http://tu.yuntaijiaju.cn

t = time.perf_counter()
来源：http://bd.colortex.cn

[U16] Py：命令行参数解析
来源：http://oc.panjiajie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vl.jctech888.com.cn

[U17] Py：初始化日志
来源：http://pc.nszjky.cn

logging.basicConfig(level=logging.INFO)
来源：http://kq.lnxyls.cn

[U18] Py：预编译正则
来源：http://lm.shtwfgs.cn

pat = re.compile(r"\d+")
来源：http://qp.hnjuh.cn

[U19] Py：正则替换带回调
来源：http://ru.jianghongdianzi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rn.lnxyls.cn

[U20] Py：缓存函数结果
来源：http://yi.panjiajie.cn

@functools.lru_cache(maxsize=None)
来源：http://sc.muxihuayi.cn

[U21] Py：自定义上下文管理器
来源：http://ge.wgjwhj.cn

@contextlib.contextmanager
来源：http://be.wgjwhj.cn

[U22] Py：矩阵转置
来源：http://xz.shxzukj.cn

list(zip(*m))
来源：http://hl.haigaiapp.cn

[U23] Py：分块读取大文件
来源：http://on.huixinmuqiang.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jm.lnxyls.cn

[U24] Py：路径操作
来源：http://bd.yuexingan06.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wo.9csxet.cn

[U25] Py：CSV 按字典读
来源：http://oo.shxzskj.cn

csv.DictReader(f)
来源：http://xc.hahajie.cn

[U26] Py：并发下载
来源：http://al.521024.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ls.asd995.cn

[U27] Py：异步 HTTP
来源：http://xn.bookmarksfly.cn

aiohttp.ClientSession() 配合 async with
来源：http://go.shtwfgs.cn

[U28] Py：类型别名
来源：http://cb.bjjhwx.cn

UserId = int
来源：http://qc.shtwfgs.cn

[U29] Py：属性校验
来源：http://iw.nszjky.cn

@property 与 @x.setter 配合
来源：http://yu.shxzukj.cn

[U30] Py：数据类
来源：http://rd.szxytkj.cn

@dataclass(slots=True)
来源：http://ou.hnjuh.cn

[U31] Py：单测
来源：http://rr.szsharing.cn

python -m pytest -q
来源：http://fc.jianghongdianzi.cn

[U32] Py：代码格式化
来源：http://om.nicolike.cn

ruff format . && ruff check --fix .
来源：http://gn.colortex.cn

[U33] Py：打包发布
来源：http://fx.huanxung.cn

python -m build  （依赖 pyproject.toml）
来源：http://pp.jctech888.com.cn

[U34] Py：判断编码
来源：http://hw.521024.cn

chardet.detect(raw)
来源：http://nq.chemitech.net.cn

[U35] Py：发送邮件
来源：http://ws.nicolike.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ql.jianghongdianzi.cn

[U36] Py：定时任务
来源：http://uq.newstarts.cn

schedule.every(10).minutes.do(job)
来源：http://gg.yuntaijiaju.cn

[U37] Py：读写 Excel
来源：http://oz.chemitech.net.cn

pandas.read_excel / DataFrame.to_excel
来源：http://bx.panjiajie.cn

[U38] Py：获取脚本所在目录
来源：http://yp.yuexingan06.cn

Path(__file__).resolve().parent
来源：http://uw.huixinmuqiang.cn

[U39] Py：判断是否在交互环境
来源：http://zd.nicolike.cn

sys.stdout.isatty()
来源：http://ul.9csxet.cn

[U40] Py：打印到标准错误
来源：http://yx.haigaiapp.cn

print("err", file=sys.stderr)
来源：http://yr.bookmarksfly.cn

[U41] PHP：初始化 Composer 项目
来源：http://nl.jctech888.com.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qd.hnjuh.cn

[U42] PHP：PSR-4 自动加载
来源：http://rk.asd995.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ht.huanxung.cn

[U43] PHP：声明命名空间
来源：http://de.huixiangedu.cn

namespace App\Http;
来源：http://xa.szsharing.cn

[U44] PHP：开启严格类型
来源：http://py.asd995.cn

declare(strict_types=1);
来源：http://uj.wgjwhj.cn

[U45] PHP：类型声明与返回类型
来源：http://nx.nszjky.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ws.jianghongdianzi.cn

[U46] PHP：可空类型
来源：http://jb.bookmarksfly.cn

?string $name = null
来源：http://ud.yuntaijiaju.cn

[U47] PHP：联合类型
来源：http://se.nicolike.cn

int|string $id
来源：http://jf.haigaiapp.cn

[U48] PHP：纯枚举
来源：http://ms.nszjky.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://la.nszjky.cn

[U49] PHP：只读属性
来源：http://rm.shxzskj.cn

public readonly string $name
来源：http://xt.9csxet.cn

[U50] PHP：构造器属性提升
来源：http://ud.chemitech.net.cn

public function __construct(private int $id) {}
来源：http://gx.shxzukj.cn

[U51] PHP：数组解构
来源：http://zz.gzmigu.cn

[$a, $b] = $arr;
来源：http://fp.nszjky.cn

[U52] PHP：箭头函数
来源：http://xx.panjiajie.cn

$double = fn($x) => $x * 2;
来源：http://mh.521024.cn

[U53] PHP：空合并运算符
来源：http://hm.9csxet.cn

$v = $a ?? $b ?? "default";
来源：http://jh.bjjhwx.cn

[U54] PHP：空安全调用
来源：http://ch.jctech888.com.cn

$obj?->method()
来源：http://dk.muxihuayi.cn

[U55] PHP：match 表达式
来源：http://fy.hahajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://er.shxzskj.cn

[U56] PHP：命名参数
来源：http://cw.nszjky.cn

f(a: 1, b: 2)
来源：http://de.wgjwhj.cn

[U57] PHP：字符串插值
来源：http://jg.chemitech.net.cn

"值: {$a}"
来源：http://hn.huixinmuqiang.cn

[U58] PHP：数组三件套
来源：http://bi.hahajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cz.yuexingan06.cn

[U59] PHP：自定义排序
来源：http://xf.shxzukj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nv.shxzukj.cn

[U60] PHP：JSON 编解码
来源：http://wx.chemitech.net.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wv.colortex.cn

[U61] PHP：正则
来源：http://na.gzmigu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://va.muxihuayi.cn

[U62] PHP：日期对象
来源：http://yy.lnxyls.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ia.szxytkj.cn

[U63] PHP：文件读写
来源：http://gv.szxytkj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bu.bookmarksfly.cn

[U64] PHP：目录遍历
来源：http://cd.nicolike.cn

glob("dir/*.php");  scandir("dir");
来源：http://kf.shxzskj.cn

[U65] PHP：会话
来源：http://nu.bookmarksfly.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://aq.nicolike.cn

[U66] PHP：设置 Cookie
来源：http://la.yuexingan06.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qv.shxzskj.cn

[U67] PHP：处理文件上传
来源：http://eq.muxihuayi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tu.chemitech.net.cn

[U68] PHP：PDO 连接
来源：http://bc.shxzskj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hl.newstarts.cn

[U69] PHP：PDO 预处理
来源：http://qh.shxzskj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tw.lnxyls.cn

[U70] PHP：PDO 事务
来源：http://ra.colortex.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mn.huixinmuqiang.cn

[U71] PHP：抛出异常
来源：http://rs.9csxet.cn

throw new RuntimeException("失败", 500);
来源：http://jz.bjjhwx.cn

[U72] PHP：写错误日志
来源：http://zp.9csxet.cn

error_log("失败: " . $e->getMessage());
来源：http://tz.yuntaijiaju.cn

[U73] PHP：读取 ini 配置
来源：http://ny.jianghongdianzi.cn

parse_ini_file("config.ini", true)
来源：http://ao.asd995.cn

[U74] PHP：读取环境变量
来源：http://hd.521024.cn

getenv("APP_ENV") ?: "production"
来源：http://ga.newstarts.cn

[U75] PHP：依赖注入
来源：http://jh.nicolike.cn

composer require psr/container
来源：http://sg.panjiajie.cn

[U76] PHP：简单路由
来源：http://im.huixiangedu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jt.asd995.cn

[U77] PHP：模板渲染
来源：http://hl.gzmigu.cn

composer require twig/twig
来源：http://lt.jianghongdianzi.cn

[U78] PHP：单元测试
来源：http://ds.gzmigu.cn

composer require --dev phpunit/phpunit
来源：http://uq.shtwfgs.cn

[U79] PHP：静态分析
来源：http://ih.shxzskj.cn

composer require --dev phpstan/phpstan
来源：http://jt.jianghongdianzi.cn

[U80] PHP：代码规范修复
来源：http://qg.bjjhwx.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://hy.yuntaijiaju.cn

[U81] JS：初始化项目
来源：http://xh.newstarts.cn

npm init -y;  npm i express
来源：http://wo.huixinmuqiang.cn

[U82] JS：package.json 脚本
来源：http://nc.szxytkj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ci.huanxung.cn

[U83] JS：ES Module 导入导出
来源：http://ol.shxzukj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ya.yuexingan06.cn

[U84] JS：CommonJS 写法
来源：http://go.huixinmuqiang.cn

module.exports = { a };  const { a } = require("./m");
来源：http://dp.shtwfgs.cn

[U85] JS：可选链
来源：http://lc.haigaiapp.cn

a?.b?.c
来源：http://lf.hnjuh.cn

[U86] JS：空值合并
来源：http://mb.huixiangedu.cn

a ?? b
来源：http://wj.jianghongdianzi.cn

[U87] JS：解构默认值
来源：http://yx.gzmigu.cn

const { a = 1, b = 2 } = obj;
来源：http://tj.szxytkj.cn

[U88] JS：对象展开合并
来源：http://ep.bookmarksfly.cn

{ ...a, ...b }
来源：http://dh.muxihuayi.cn

[U89] JS：数组去重
来源：http://ha.jctech888.com.cn

[...new Set(arr)]
来源：http://be.yuexingan06.cn

[U90] JS：数字数组排序
来源：http://wy.huanxung.cn

[...arr].sort((a, b) => a - b)
来源：http://vv.colortex.cn

[U91] JS：对象键值遍历
来源：http://xu.wgjwhj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ra.nszjky.cn

[U92] JS：深拷贝
来源：http://pb.chemitech.net.cn

structuredClone(obj)
来源：http://ne.muxihuayi.cn

[U93] JS：模板字符串
来源：http://kg.jianghongdianzi.cn

`共 ${n} 条`
来源：http://qj.lnxyls.cn

[U94] JS：箭头函数
来源：http://yn.huixiangedu.cn

const double = x => x * 2;
来源：http://bh.jianghongdianzi.cn


<!-- 参考信息 -->