代发 wailian999

[T09] Kotlin：扩展函数
来源：http://mk.lnxyls.cn

fun String.exclaim() = this + "!"
来源：http://po.szxytkj.cn

[T10] Kotlin：默认参数
来源：http://kh.muxihuayi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jl.huixiangedu.cn

[T11] Kotlin：协程
来源：http://em.hahajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://eq.hahajie.cn

[T12] Kotlin：解构声明
来源：http://sa.bjjhwx.cn

val (a, b) = Pair(1, 2)
来源：http://eo.nszjky.cn

[T13] Kotlin：只读 Map
来源：http://rb.jctech888.com.cn

val m = mapOf("a" to 1)
来源：http://mj.newstarts.cn

[T14] Kotlin：循环
来源：http://aq.muxihuayi.cn

for (i in 1..10) println(i)
来源：http://lj.newstarts.cn

[T15] Kotlin：接口
来源：http://rl.huanxung.cn

interface Shape { fun area(): Double }
来源：http://th.gzmigu.cn

[T16] Swift：Hello World
来源：http://hy.huixiangedu.cn

print("Hello")
来源：http://sx.nicolike.cn

[T17] Swift：变量与常量
来源：http://vv.lnxyls.cn

var a = 1;  let b = 2
来源：http://zo.521024.cn

[T18] Swift：字符串插值
来源：http://lw.gzmigu.cn

"值: \(b)"
来源：http://qu.colortex.cn

[T19] Swift：可选绑定
来源：http://co.521024.cn

if let n = opt { print(n) }
来源：http://hj.bjjhwx.cn

[T20] Swift：数组操作
来源：http://es.shxzskj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ud.yuexingan06.cn

[T21] Swift：遍历
来源：http://bt.chemitech.net.cn

for x in a { print(x) }
来源：http://py.huixinmuqiang.cn

[T22] Swift：字典
来源：http://he.9csxet.cn

var d = ["a": 1];  d["b"] = 2
来源：http://op.yuntaijiaju.cn

[T23] Swift：函数
来源：http://et.jianghongdianzi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cz.shtwfgs.cn

[T24] Swift：闭包
来源：http://py.lnxyls.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://tc.9csxet.cn

[T25] Swift：结构体
来源：http://bf.nszjky.cn

struct P { var x: Int }
来源：http://ba.chemitech.net.cn

[T26] Swift：类与重写
来源：http://lr.hnjuh.cn

class A: Base { override func f() {} }
来源：http://ow.chemitech.net.cn

[T27] Swift：错误处理
来源：http://uc.szsharing.cn

do { try f() } catch { print(error) }
来源：http://ak.jianghongdianzi.cn

[T28] Swift：枚举
来源：http://bk.colortex.cn

enum Color { case red, green }
来源：http://pe.lnxyls.cn

[T29] Swift：guard 提前返回
来源：http://do.hahajie.cn

guard let x = opt else { return }
来源：http://lj.shtwfgs.cn

[T30] Swift：协议
来源：http://fh.yuntaijiaju.cn

protocol Shape { func area() -> Double }
来源：http://rm.nicolike.cn

[T31] Lua：Hello World
来源：http://ye.szxytkj.cn

print("Hello")
来源：http://rn.nszjky.cn

[T32] Lua：局部变量
来源：http://ts.newstarts.cn

local a = 1
来源：http://sr.szsharing.cn

[T33] Lua：表（数组）
来源：http://wc.bjjhwx.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ls.wgjwhj.cn

[T34] Lua：遍历表
来源：http://ny.yuntaijiaju.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://mv.chemitech.net.cn

[T35] Lua：字典表
来源：http://us.muxihuayi.cn

local d = { a = 1 };  d.b = 2
来源：http://bw.yuntaijiaju.cn

[T36] Lua：函数
来源：http://sc.521024.cn

function add(a, b) return a + b end
来源：http://pw.colortex.cn

[T37] Lua：字符串拼接
来源：http://rb.jianghongdianzi.cn

"a" .. "b"
来源：http://eg.lnxyls.cn

[T38] Lua：条件
来源：http://hk.bookmarksfly.cn

if x > 0 then print("正") end
来源：http://uz.wgjwhj.cn

[T39] Lua：模式匹配
来源：http://mt.yuexingan06.cn

string.find(s, "%d+")
来源：http://qj.huixinmuqiang.cn

[T40] Lua：元表
来源：http://vj.gzmigu.cn

setmetatable({}, { __index = base })
来源：http://nf.newstarts.cn

[T41] Perl：Hello World
来源：http://uj.chemitech.net.cn

print "Hello\n";
来源：http://hc.nszjky.cn

[T42] Perl：变量类型
来源：http://jx.newstarts.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ua.szsharing.cn

[T43] Perl：字符串插值
来源：http://bh.jctech888.com.cn

"值: $a"
来源：http://gw.wgjwhj.cn

[T44] Perl：条件
来源：http://bt.asd995.cn

if ($a > 0) { print "正"; }
来源：http://ql.wgjwhj.cn

[T45] Perl：数组遍历
来源：http://hi.newstarts.cn

for my $x (@arr) { print $x; }
来源：http://pu.huixiangedu.cn

[T46] Perl：哈希操作
来源：http://cp.jianghongdianzi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qy.shxzukj.cn

[T47] Perl：正则捕获
来源：http://dx.yuexingan06.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ik.chemitech.net.cn

[T48] Perl：正则替换
来源：http://nf.jctech888.com.cn

$s =~ s/old/new/g;
来源：http://gr.colortex.cn

[T49] Perl：函数
来源：http://kl.chemitech.net.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jt.yuexingan06.cn

[T50] Perl：逐行读文件
来源：http://ub.nicolike.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ok.9csxet.cn

while (my $line = <$fh>) { print $line; }
来源：http://oo.chemitech.net.cn

[T51] Scala：Hello World
来源：http://lm.wgjwhj.cn

println("Hello")
来源：http://zx.yuntaijiaju.cn

[T52] Scala：变量
来源：http://hj.shxzskj.cn

val a = 1;  var b = 2
来源：http://at.chemitech.net.cn

[T53] Scala：字符串插值
来源：http://ow.huixiangedu.cn

s"值: $b"
来源：http://ng.jctech888.com.cn

[T54] Scala：集合映射
来源：http://gz.szxytkj.cn

List(1, 2, 3).map(_ * 2)
来源：http://ux.jctech888.com.cn

[T55] Scala：集合过滤
来源：http://zm.yuntaijiaju.cn

List(1, 2, 3).filter(_ > 1)
来源：http://sr.huixiangedu.cn

[T56] Scala：样例类
来源：http://te.huanxung.cn

case class User(name: String, age: Int)
来源：http://xx.jctech888.com.cn

[T57] Scala：模式匹配
来源：http://ii.bjjhwx.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ut.521024.cn

[T58] Scala：函数定义
来源：http://to.huanxung.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zi.hahajie.cn

[T59] Scala：循环
来源：http://jv.nszjky.cn

for (i <- 1 to 10) println(i)
来源：http://qo.chemitech.net.cn

[T60] Scala：折叠
来源：http://jl.shxzukj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yh.jianghongdianzi.cn

================================================================================
来源：http://ry.hnjuh.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xd.9csxet.cn

================================================================================
来源：http://qx.lnxyls.cn

[U01] Py：创建虚拟环境
来源：http://yv.lnxyls.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mp.lnxyls.cn

[U02] Py：导出 / 安装依赖
来源：http://pj.panjiajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://el.szxytkj.cn

[U03] Py：加载 .env 配置
来源：http://jl.szxytkj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ht.szxytkj.cn

[U04] Py：变量调试打印
来源：http://cr.521024.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://at.jctech888.com.cn

[U05] Py：列表去重且保序
来源：http://um.jctech888.com.cn

list(dict.fromkeys(arr))
来源：http://fn.gzmigu.cn

[U06] Py：合并两个字典
来源：http://mv.gzmigu.cn

{**a, **b}
来源：http://xe.lnxyls.cn

[U07] Py：反转字典键值
来源：http://qe.nszjky.cn

{v: k for k, v in d.items()}
来源：http://on.panjiajie.cn

[U08] Py：展平二维列表
来源：http://yw.nszjky.cn

[y for x in nested for y in x]
来源：http://hp.jctech888.com.cn

[U09] Py：字典取最大值的键
来源：http://va.huixiangedu.cn

max(d, key=d.get)
来源：http://lj.lnxyls.cn

[U10] Py：按值排序字典
来源：http://rk.colortex.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kb.yuexingan06.cn

[U11] Py：生成器表达式
来源：http://bs.gzmigu.cn

(x * 2 for x in arr)
来源：http://vl.newstarts.cn

[U12] Py：取出现最多的 3 个元素
来源：http://js.newstarts.cn

Counter(arr).most_common(3)
来源：http://us.521024.cn

[U13] Py：固定长度队列
来源：http://uw.newstarts.cn

deque(maxlen=10)
来源：http://hy.nszjky.cn

[U14] Py：分组收集到列表
来源：http://ov.yuntaijiaju.cn

defaultdict(list)
来源：http://ww.chemitech.net.cn

[U15] Py：高精度计时
来源：http://zk.huixiangedu.cn

t = time.perf_counter()
来源：http://zl.yuntaijiaju.cn

[U16] Py：命令行参数解析
来源：http://bv.panjiajie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lk.newstarts.cn

[U17] Py：初始化日志
来源：http://iy.hnjuh.cn

logging.basicConfig(level=logging.INFO)
来源：http://dc.asd995.cn

[U18] Py：预编译正则
来源：http://en.muxihuayi.cn

pat = re.compile(r"\d+")
来源：http://sg.colortex.cn

[U19] Py：正则替换带回调
来源：http://bu.hnjuh.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qx.szxytkj.cn

[U20] Py：缓存函数结果
来源：http://cz.521024.cn

@functools.lru_cache(maxsize=None)
来源：http://aj.muxihuayi.cn

[U21] Py：自定义上下文管理器
来源：http://jz.nicolike.cn

@contextlib.contextmanager
来源：http://tp.jianghongdianzi.cn

[U22] Py：矩阵转置
来源：http://gw.szsharing.cn

list(zip(*m))
来源：http://iu.huixiangedu.cn

[U23] Py：分块读取大文件
来源：http://nt.huixinmuqiang.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lf.hnjuh.cn

[U24] Py：路径操作
来源：http://xd.nicolike.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://my.gzmigu.cn

[U25] Py：CSV 按字典读
来源：http://wc.huixiangedu.cn

csv.DictReader(f)
来源：http://gi.bookmarksfly.cn

[U26] Py：并发下载
来源：http://sn.colortex.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fb.haigaiapp.cn

[U27] Py：异步 HTTP
来源：http://xb.bjjhwx.cn

aiohttp.ClientSession() 配合 async with
来源：http://av.huanxung.cn

[U28] Py：类型别名
来源：http://oq.hnjuh.cn

UserId = int
来源：http://lp.panjiajie.cn

[U29] Py：属性校验
来源：http://om.jctech888.com.cn

@property 与 @x.setter 配合
来源：http://gn.jianghongdianzi.cn

[U30] Py：数据类
来源：http://wo.shxzukj.cn

@dataclass(slots=True)
来源：http://ad.szsharing.cn

[U31] Py：单测
来源：http://jq.shtwfgs.cn

python -m pytest -q
来源：http://cf.bookmarksfly.cn

[U32] Py：代码格式化
来源：http://rf.nszjky.cn

ruff format . && ruff check --fix .
来源：http://tu.hahajie.cn

[U33] Py：打包发布
来源：http://ef.shxzukj.cn

python -m build  （依赖 pyproject.toml）
来源：http://ih.hnjuh.cn

[U34] Py：判断编码
来源：http://jg.bookmarksfly.cn

chardet.detect(raw)
来源：http://ey.szxytkj.cn

[U35] Py：发送邮件
来源：http://yu.jianghongdianzi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mx.yuntaijiaju.cn

[U36] Py：定时任务
来源：http://xm.muxihuayi.cn

schedule.every(10).minutes.do(job)
来源：http://oh.szxytkj.cn

[U37] Py：读写 Excel
来源：http://wj.lnxyls.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qd.huixiangedu.cn

[U38] Py：获取脚本所在目录
来源：http://go.huanxung.cn

Path(__file__).resolve().parent
来源：http://fh.shxzukj.cn

[U39] Py：判断是否在交互环境
来源：http://od.huixiangedu.cn

sys.stdout.isatty()
来源：http://kl.jctech888.com.cn

[U40] Py：打印到标准错误
来源：http://qk.bookmarksfly.cn

print("err", file=sys.stderr)
来源：http://jy.huixinmuqiang.cn

[U41] PHP：初始化 Composer 项目
来源：http://zf.panjiajie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://tw.haigaiapp.cn

[U42] PHP：PSR-4 自动加载
来源：http://ry.asd995.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cg.muxihuayi.cn

[U43] PHP：声明命名空间
来源：http://he.hahajie.cn

namespace App\Http;
来源：http://oe.yuexingan06.cn

[U44] PHP：开启严格类型
来源：http://di.gzmigu.cn

declare(strict_types=1);
来源：http://qc.bookmarksfly.cn

[U45] PHP：类型声明与返回类型
来源：http://qd.shxzukj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ts.lnxyls.cn

[U46] PHP：可空类型
来源：http://wd.jctech888.com.cn

?string $name = null
来源：http://cp.newstarts.cn

[U47] PHP：联合类型
来源：http://aa.shxzukj.cn

int|string $id
来源：http://ab.yuexingan06.cn

[U48] PHP：纯枚举
来源：http://ct.lnxyls.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://iu.hahajie.cn

[U49] PHP：只读属性
来源：http://eu.colortex.cn

public readonly string $name
来源：http://is.shxzskj.cn

[U50] PHP：构造器属性提升
来源：http://wx.jianghongdianzi.cn

public function __construct(private int $id) {}
来源：http://ao.muxihuayi.cn

[U51] PHP：数组解构
来源：http://kb.jianghongdianzi.cn

[$a, $b] = $arr;
来源：http://rd.shxzukj.cn

[U52] PHP：箭头函数
来源：http://xh.huanxung.cn

$double = fn($x) => $x * 2;
来源：http://ih.muxihuayi.cn

[U53] PHP：空合并运算符
来源：http://oz.huixiangedu.cn

$v = $a ?? $b ?? "default";
来源：http://sm.bjjhwx.cn

[U54] PHP：空安全调用
来源：http://gf.haigaiapp.cn

$obj?->method()
来源：http://af.shtwfgs.cn

[U55] PHP：match 表达式
来源：http://mw.shxzukj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fg.521024.cn

[U56] PHP：命名参数
来源：http://zr.nszjky.cn

f(a: 1, b: 2)
来源：http://oi.huanxung.cn

[U57] PHP：字符串插值
来源：http://uv.yuntaijiaju.cn

"值: {$a}"
来源：http://sq.hahajie.cn

[U58] PHP：数组三件套
来源：http://ii.huanxung.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jo.colortex.cn

[U59] PHP：自定义排序
来源：http://wu.hnjuh.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wx.colortex.cn

[U60] PHP：JSON 编解码
来源：http://bg.haigaiapp.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ef.lnxyls.cn

[U61] PHP：正则
来源：http://re.hnjuh.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://km.bjjhwx.cn

[U62] PHP：日期对象
来源：http://wg.panjiajie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://if.bjjhwx.cn

[U63] PHP：文件读写
来源：http://yj.jctech888.com.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vz.chemitech.net.cn

[U64] PHP：目录遍历
来源：http://hl.lnxyls.cn

glob("dir/*.php");  scandir("dir");
来源：http://kj.shtwfgs.cn

[U65] PHP：会话
来源：http://pq.hnjuh.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://qz.shxzskj.cn

[U66] PHP：设置 Cookie
来源：http://ky.jctech888.com.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hc.yuexingan06.cn

[U67] PHP：处理文件上传
来源：http://aw.shxzskj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qi.yuexingan06.cn

[U68] PHP：PDO 连接
来源：http://kx.hnjuh.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ao.hahajie.cn

[U69] PHP：PDO 预处理
来源：http://jo.nszjky.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ct.szsharing.cn

[U70] PHP：PDO 事务
来源：http://id.haigaiapp.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xe.shtwfgs.cn

[U71] PHP：抛出异常
来源：http://mj.jctech888.com.cn

throw new RuntimeException("失败", 500);
来源：http://ru.bookmarksfly.cn

[U72] PHP：写错误日志
来源：http://kh.huanxung.cn

error_log("失败: " . $e->getMessage());
来源：http://rc.huixiangedu.cn

[U73] PHP：读取 ini 配置
来源：http://gm.nicolike.cn

parse_ini_file("config.ini", true)
来源：http://go.colortex.cn

[U74] PHP：读取环境变量
来源：http://hv.huanxung.cn

getenv("APP_ENV") ?: "production"
来源：http://dj.bjjhwx.cn

[U75] PHP：依赖注入
来源：http://rm.szxytkj.cn

composer require psr/container
来源：http://qo.muxihuayi.cn

[U76] PHP：简单路由
来源：http://pd.wgjwhj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vo.lnxyls.cn

[U77] PHP：模板渲染
来源：http://rg.hahajie.cn

composer require twig/twig
来源：http://pg.bjjhwx.cn

[U78] PHP：单元测试
来源：http://uo.shxzskj.cn

composer require --dev phpunit/phpunit
来源：http://xf.colortex.cn

[U79] PHP：静态分析
来源：http://tr.jianghongdianzi.cn

composer require --dev phpstan/phpstan
来源：http://lj.nszjky.cn

[U80] PHP：代码规范修复
来源：http://fi.szxytkj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://gg.haigaiapp.cn

[U81] JS：初始化项目
来源：http://qq.hahajie.cn

npm init -y;  npm i express
来源：http://up.jianghongdianzi.cn

[U82] JS：package.json 脚本
来源：http://wt.colortex.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ol.szsharing.cn

[U83] JS：ES Module 导入导出
来源：http://jf.muxihuayi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://kh.hahajie.cn

[U84] JS：CommonJS 写法
来源：http://oi.huixinmuqiang.cn

module.exports = { a };  const { a } = require("./m");
来源：http://td.shxzskj.cn

[U85] JS：可选链
来源：http://gw.huixinmuqiang.cn

a?.b?.c
来源：http://rc.wgjwhj.cn

[U86] JS：空值合并
来源：http://yh.muxihuayi.cn

a ?? b
来源：http://wi.yuexingan06.cn

[U87] JS：解构默认值
来源：http://pp.newstarts.cn

const { a = 1, b = 2 } = obj;
来源：http://ek.yuntaijiaju.cn

[U88] JS：对象展开合并
来源：http://pr.muxihuayi.cn

{ ...a, ...b }
来源：http://xu.hahajie.cn

[U89] JS：数组去重
来源：http://dd.bookmarksfly.cn

[...new Set(arr)]
来源：http://fc.bjjhwx.cn

[U90] JS：数字数组排序
来源：http://am.shxzukj.cn

[...arr].sort((a, b) => a - b)
来源：http://sg.jctech888.com.cn

[U91] JS：对象键值遍历
来源：http://bj.shtwfgs.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pi.yuntaijiaju.cn

[U92] JS：深拷贝
来源：http://tv.newstarts.cn

structuredClone(obj)
来源：http://fx.lnxyls.cn

[U93] JS：模板字符串
来源：http://ud.gzmigu.cn

`共 ${n} 条`
来源：http://zt.yuexingan06.cn

[U94] JS：箭头函数
来源：http://tm.wgjwhj.cn

const double = x => x * 2;
来源：http://vr.shxzukj.cn

[U95] JS：Promise 包装
来源：http://fx.bjjhwx.cn

new Promise((resolve, reject) => {})
来源：http://qw.panjiajie.cn

[U96] JS：async/await 与异常
来源：http://vg.9csxet.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ih.9csxet.cn


<!-- 参考信息 -->