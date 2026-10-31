代发 wailian999

[T09] Kotlin：扩展函数
来源：http://hh.hnjuh.cn

fun String.exclaim() = this + "!"
来源：http://qm.hahajie.cn

[T10] Kotlin：默认参数
来源：http://yc.szxytkj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jv.shtwfgs.cn

[T11] Kotlin：协程
来源：http://cn.bjjhwx.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://go.colortex.cn

[T12] Kotlin：解构声明
来源：http://yy.jianghongdianzi.cn

val (a, b) = Pair(1, 2)
来源：http://oo.colortex.cn

[T13] Kotlin：只读 Map
来源：http://mj.szsharing.cn

val m = mapOf("a" to 1)
来源：http://km.newstarts.cn

[T14] Kotlin：循环
来源：http://gm.wgjwhj.cn

for (i in 1..10) println(i)
来源：http://ct.bjjhwx.cn

[T15] Kotlin：接口
来源：http://et.haigaiapp.cn

interface Shape { fun area(): Double }
来源：http://wa.lnxyls.cn

[T16] Swift：Hello World
来源：http://ra.asd995.cn

print("Hello")
来源：http://fj.shxzukj.cn

[T17] Swift：变量与常量
来源：http://uw.nicolike.cn

var a = 1;  let b = 2
来源：http://oz.bjjhwx.cn

[T18] Swift：字符串插值
来源：http://nc.nszjky.cn

"值: \(b)"
来源：http://ok.shxzskj.cn

[T19] Swift：可选绑定
来源：http://mn.newstarts.cn

if let n = opt { print(n) }
来源：http://ir.haigaiapp.cn

[T20] Swift：数组操作
来源：http://uv.shtwfgs.cn

var a = [1, 2, 3];  a.append(4)
来源：http://js.jctech888.com.cn

[T21] Swift：遍历
来源：http://ri.bookmarksfly.cn

for x in a { print(x) }
来源：http://rm.haigaiapp.cn

[T22] Swift：字典
来源：http://tg.shtwfgs.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xe.wgjwhj.cn

[T23] Swift：函数
来源：http://ld.yuexingan06.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vq.shxzukj.cn

[T24] Swift：闭包
来源：http://rc.huanxung.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://jq.bookmarksfly.cn

[T25] Swift：结构体
来源：http://wa.bookmarksfly.cn

struct P { var x: Int }
来源：http://zc.asd995.cn

[T26] Swift：类与重写
来源：http://lq.lnxyls.cn

class A: Base { override func f() {} }
来源：http://me.yuntaijiaju.cn

[T27] Swift：错误处理
来源：http://wg.huixiangedu.cn

do { try f() } catch { print(error) }
来源：http://so.hahajie.cn

[T28] Swift：枚举
来源：http://rp.yuexingan06.cn

enum Color { case red, green }
来源：http://ay.yuexingan06.cn

[T29] Swift：guard 提前返回
来源：http://xl.bjjhwx.cn

guard let x = opt else { return }
来源：http://le.jctech888.com.cn

[T30] Swift：协议
来源：http://yf.huixiangedu.cn

protocol Shape { func area() -> Double }
来源：http://jb.huixiangedu.cn

[T31] Lua：Hello World
来源：http://vs.huixinmuqiang.cn

print("Hello")
来源：http://pb.gzmigu.cn

[T32] Lua：局部变量
来源：http://px.newstarts.cn

local a = 1
来源：http://dc.asd995.cn

[T33] Lua：表（数组）
来源：http://qw.shtwfgs.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://pa.9csxet.cn

[T34] Lua：遍历表
来源：http://km.yuexingan06.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://un.yuntaijiaju.cn

[T35] Lua：字典表
来源：http://om.yuntaijiaju.cn

local d = { a = 1 };  d.b = 2
来源：http://uv.chemitech.net.cn

[T36] Lua：函数
来源：http://ta.wgjwhj.cn

function add(a, b) return a + b end
来源：http://bx.nszjky.cn

[T37] Lua：字符串拼接
来源：http://jl.bookmarksfly.cn

"a" .. "b"
来源：http://ps.yuntaijiaju.cn

[T38] Lua：条件
来源：http://ds.asd995.cn

if x > 0 then print("正") end
来源：http://oa.wgjwhj.cn

[T39] Lua：模式匹配
来源：http://th.huixinmuqiang.cn

string.find(s, "%d+")
来源：http://lg.521024.cn

[T40] Lua：元表
来源：http://na.asd995.cn

setmetatable({}, { __index = base })
来源：http://hk.muxihuayi.cn

[T41] Perl：Hello World
来源：http://vg.szsharing.cn

print "Hello\n";
来源：http://mt.haigaiapp.cn

[T42] Perl：变量类型
来源：http://zz.chemitech.net.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ce.nszjky.cn

[T43] Perl：字符串插值
来源：http://el.szsharing.cn

"值: $a"
来源：http://xc.haigaiapp.cn

[T44] Perl：条件
来源：http://du.huixinmuqiang.cn

if ($a > 0) { print "正"; }
来源：http://wv.nicolike.cn

[T45] Perl：数组遍历
来源：http://xa.szxytkj.cn

for my $x (@arr) { print $x; }
来源：http://eb.haigaiapp.cn

[T46] Perl：哈希操作
来源：http://bn.panjiajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xt.szsharing.cn

[T47] Perl：正则捕获
来源：http://sk.9csxet.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://iu.jianghongdianzi.cn

[T48] Perl：正则替换
来源：http://zu.colortex.cn

$s =~ s/old/new/g;
来源：http://af.huanxung.cn

[T49] Perl：函数
来源：http://wy.yuexingan06.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://io.yuexingan06.cn

[T50] Perl：逐行读文件
来源：http://ye.shxzukj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://li.shtwfgs.cn

while (my $line = <$fh>) { print $line; }
来源：http://vp.colortex.cn

[T51] Scala：Hello World
来源：http://je.jctech888.com.cn

println("Hello")
来源：http://be.shxzskj.cn

[T52] Scala：变量
来源：http://kn.shxzskj.cn

val a = 1;  var b = 2
来源：http://hp.bookmarksfly.cn

[T53] Scala：字符串插值
来源：http://no.shtwfgs.cn

s"值: $b"
来源：http://uk.yuexingan06.cn

[T54] Scala：集合映射
来源：http://sl.asd995.cn

List(1, 2, 3).map(_ * 2)
来源：http://cz.hahajie.cn

[T55] Scala：集合过滤
来源：http://vu.szxytkj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ly.yuexingan06.cn

[T56] Scala：样例类
来源：http://fk.colortex.cn

case class User(name: String, age: Int)
来源：http://aj.hahajie.cn

[T57] Scala：模式匹配
来源：http://kz.wgjwhj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://uq.szsharing.cn

[T58] Scala：函数定义
来源：http://lo.colortex.cn

def add(a: Int, b: Int): Int = a + b
来源：http://io.shtwfgs.cn

[T59] Scala：循环
来源：http://oi.hnjuh.cn

for (i <- 1 to 10) println(i)
来源：http://wt.nicolike.cn

[T60] Scala：折叠
来源：http://ai.bookmarksfly.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://je.bookmarksfly.cn

================================================================================
来源：http://mb.bookmarksfly.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ow.jctech888.com.cn

================================================================================
来源：http://pw.hnjuh.cn

[U01] Py：创建虚拟环境
来源：http://ox.lnxyls.cn

python -m venv .venv && source .venv/bin/activate
来源：http://lh.hahajie.cn

[U02] Py：导出 / 安装依赖
来源：http://sx.gzmigu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://aq.hahajie.cn

[U03] Py：加载 .env 配置
来源：http://tw.asd995.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://hw.hahajie.cn

[U04] Py：变量调试打印
来源：http://sl.huixiangedu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://md.chemitech.net.cn

[U05] Py：列表去重且保序
来源：http://dc.chemitech.net.cn

list(dict.fromkeys(arr))
来源：http://yi.hahajie.cn

[U06] Py：合并两个字典
来源：http://eb.muxihuayi.cn

{**a, **b}
来源：http://uw.huixiangedu.cn

[U07] Py：反转字典键值
来源：http://fp.huixiangedu.cn

{v: k for k, v in d.items()}
来源：http://yl.huanxung.cn

[U08] Py：展平二维列表
来源：http://nu.wgjwhj.cn

[y for x in nested for y in x]
来源：http://bz.muxihuayi.cn

[U09] Py：字典取最大值的键
来源：http://sb.shxzukj.cn

max(d, key=d.get)
来源：http://jd.szxytkj.cn

[U10] Py：按值排序字典
来源：http://hp.szsharing.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://iz.yuexingan06.cn

[U11] Py：生成器表达式
来源：http://og.chemitech.net.cn

(x * 2 for x in arr)
来源：http://tm.shxzskj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zy.huixiangedu.cn

Counter(arr).most_common(3)
来源：http://yn.bjjhwx.cn

[U13] Py：固定长度队列
来源：http://sy.asd995.cn

deque(maxlen=10)
来源：http://uu.bookmarksfly.cn

[U14] Py：分组收集到列表
来源：http://rs.bjjhwx.cn

defaultdict(list)
来源：http://qw.colortex.cn

[U15] Py：高精度计时
来源：http://wz.521024.cn

t = time.perf_counter()
来源：http://oz.shxzukj.cn

[U16] Py：命令行参数解析
来源：http://es.chemitech.net.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qn.shxzskj.cn

[U17] Py：初始化日志
来源：http://vc.jctech888.com.cn

logging.basicConfig(level=logging.INFO)
来源：http://oq.wgjwhj.cn

[U18] Py：预编译正则
来源：http://rk.nszjky.cn

pat = re.compile(r"\d+")
来源：http://lz.lnxyls.cn

[U19] Py：正则替换带回调
来源：http://sq.nicolike.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ik.wgjwhj.cn

[U20] Py：缓存函数结果
来源：http://vt.newstarts.cn

@functools.lru_cache(maxsize=None)
来源：http://xw.521024.cn

[U21] Py：自定义上下文管理器
来源：http://ng.jianghongdianzi.cn

@contextlib.contextmanager
来源：http://zv.newstarts.cn

[U22] Py：矩阵转置
来源：http://zq.521024.cn

list(zip(*m))
来源：http://lw.nszjky.cn

[U23] Py：分块读取大文件
来源：http://bf.huixinmuqiang.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rr.9csxet.cn

[U24] Py：路径操作
来源：http://xa.yuexingan06.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xe.muxihuayi.cn

[U25] Py：CSV 按字典读
来源：http://zx.hnjuh.cn

csv.DictReader(f)
来源：http://ug.colortex.cn

[U26] Py：并发下载
来源：http://ex.yuexingan06.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://oy.gzmigu.cn

[U27] Py：异步 HTTP
来源：http://al.huixinmuqiang.cn

aiohttp.ClientSession() 配合 async with
来源：http://ju.yuntaijiaju.cn

[U28] Py：类型别名
来源：http://rv.shxzukj.cn

UserId = int
来源：http://vg.colortex.cn

[U29] Py：属性校验
来源：http://on.wgjwhj.cn

@property 与 @x.setter 配合
来源：http://tb.colortex.cn

[U30] Py：数据类
来源：http://hd.haigaiapp.cn

@dataclass(slots=True)
来源：http://lt.nszjky.cn

[U31] Py：单测
来源：http://ll.hnjuh.cn

python -m pytest -q
来源：http://or.nszjky.cn

[U32] Py：代码格式化
来源：http://xf.huanxung.cn

ruff format . && ruff check --fix .
来源：http://oh.lnxyls.cn

[U33] Py：打包发布
来源：http://od.szsharing.cn

python -m build  （依赖 pyproject.toml）
来源：http://qd.colortex.cn

[U34] Py：判断编码
来源：http://we.jianghongdianzi.cn

chardet.detect(raw)
来源：http://jw.shxzskj.cn

[U35] Py：发送邮件
来源：http://zy.szxytkj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ly.bjjhwx.cn

[U36] Py：定时任务
来源：http://iw.jianghongdianzi.cn

schedule.every(10).minutes.do(job)
来源：http://nc.nszjky.cn

[U37] Py：读写 Excel
来源：http://qo.lnxyls.cn

pandas.read_excel / DataFrame.to_excel
来源：http://iz.bjjhwx.cn

[U38] Py：获取脚本所在目录
来源：http://vf.9csxet.cn

Path(__file__).resolve().parent
来源：http://rn.muxihuayi.cn

[U39] Py：判断是否在交互环境
来源：http://uk.521024.cn

sys.stdout.isatty()
来源：http://sm.bjjhwx.cn

[U40] Py：打印到标准错误
来源：http://sr.wgjwhj.cn

print("err", file=sys.stderr)
来源：http://cv.shtwfgs.cn

[U41] PHP：初始化 Composer 项目
来源：http://nl.9csxet.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ng.nszjky.cn

[U42] PHP：PSR-4 自动加载
来源：http://ve.yuexingan06.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yj.shxzukj.cn

[U43] PHP：声明命名空间
来源：http://ba.panjiajie.cn

namespace App\Http;
来源：http://sl.szxytkj.cn

[U44] PHP：开启严格类型
来源：http://di.hnjuh.cn

declare(strict_types=1);
来源：http://yz.chemitech.net.cn

[U45] PHP：类型声明与返回类型
来源：http://ti.shxzskj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://dp.muxihuayi.cn

[U46] PHP：可空类型
来源：http://zm.hahajie.cn

?string $name = null
来源：http://ng.szsharing.cn

[U47] PHP：联合类型
来源：http://ha.huixinmuqiang.cn

int|string $id
来源：http://ak.521024.cn

[U48] PHP：纯枚举
来源：http://lh.shxzukj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ce.lnxyls.cn

[U49] PHP：只读属性
来源：http://qv.huanxung.cn

public readonly string $name
来源：http://bk.yuntaijiaju.cn

[U50] PHP：构造器属性提升
来源：http://au.newstarts.cn

public function __construct(private int $id) {}
来源：http://tw.jianghongdianzi.cn

[U51] PHP：数组解构
来源：http://xd.521024.cn

[$a, $b] = $arr;
来源：http://rx.chemitech.net.cn

[U52] PHP：箭头函数
来源：http://vs.newstarts.cn

$double = fn($x) => $x * 2;
来源：http://xu.yuntaijiaju.cn

[U53] PHP：空合并运算符
来源：http://hj.chemitech.net.cn

$v = $a ?? $b ?? "default";
来源：http://du.huixinmuqiang.cn

[U54] PHP：空安全调用
来源：http://lm.newstarts.cn

$obj?->method()
来源：http://dd.yuntaijiaju.cn

[U55] PHP：match 表达式
来源：http://gz.bookmarksfly.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vm.yuexingan06.cn

[U56] PHP：命名参数
来源：http://ob.hnjuh.cn

f(a: 1, b: 2)
来源：http://up.nicolike.cn

[U57] PHP：字符串插值
来源：http://uz.asd995.cn

"值: {$a}"
来源：http://ig.szxytkj.cn

[U58] PHP：数组三件套
来源：http://pk.colortex.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ih.huanxung.cn

[U59] PHP：自定义排序
来源：http://be.chemitech.net.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dv.gzmigu.cn

[U60] PHP：JSON 编解码
来源：http://xw.panjiajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ao.nicolike.cn

[U61] PHP：正则
来源：http://cu.szsharing.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wj.szsharing.cn

[U62] PHP：日期对象
来源：http://ii.szxytkj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hj.shxzukj.cn

[U63] PHP：文件读写
来源：http://ji.muxihuayi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://oy.jianghongdianzi.cn

[U64] PHP：目录遍历
来源：http://aa.yuexingan06.cn

glob("dir/*.php");  scandir("dir");
来源：http://ff.yuntaijiaju.cn

[U65] PHP：会话
来源：http://yi.nszjky.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://cx.jianghongdianzi.cn

[U66] PHP：设置 Cookie
来源：http://hl.yuntaijiaju.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hd.newstarts.cn

[U67] PHP：处理文件上传
来源：http://rn.panjiajie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pz.muxihuayi.cn

[U68] PHP：PDO 连接
来源：http://yb.shxzukj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ru.nszjky.cn

[U69] PHP：PDO 预处理
来源：http://vo.muxihuayi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://es.shxzukj.cn

[U70] PHP：PDO 事务
来源：http://xg.szxytkj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ly.huanxung.cn

[U71] PHP：抛出异常
来源：http://hz.huixiangedu.cn

throw new RuntimeException("失败", 500);
来源：http://sv.yuexingan06.cn

[U72] PHP：写错误日志
来源：http://as.shtwfgs.cn

error_log("失败: " . $e->getMessage());
来源：http://ec.shxzskj.cn

[U73] PHP：读取 ini 配置
来源：http://lb.newstarts.cn

parse_ini_file("config.ini", true)
来源：http://sc.shxzskj.cn

[U74] PHP：读取环境变量
来源：http://fm.lnxyls.cn

getenv("APP_ENV") ?: "production"
来源：http://ho.nicolike.cn

[U75] PHP：依赖注入
来源：http://vz.521024.cn

composer require psr/container
来源：http://ux.haigaiapp.cn

[U76] PHP：简单路由
来源：http://aj.nszjky.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vw.chemitech.net.cn

[U77] PHP：模板渲染
来源：http://iy.huanxung.cn

composer require twig/twig
来源：http://zn.nicolike.cn

[U78] PHP：单元测试
来源：http://cp.521024.cn

composer require --dev phpunit/phpunit
来源：http://no.gzmigu.cn

[U79] PHP：静态分析
来源：http://sc.gzmigu.cn

composer require --dev phpstan/phpstan
来源：http://qq.szxytkj.cn

[U80] PHP：代码规范修复
来源：http://fr.jianghongdianzi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xi.huixinmuqiang.cn

[U81] JS：初始化项目
来源：http://vl.muxihuayi.cn

npm init -y;  npm i express
来源：http://ul.szxytkj.cn

[U82] JS：package.json 脚本
来源：http://sy.huixiangedu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gc.shxzukj.cn

[U83] JS：ES Module 导入导出
来源：http://lr.szsharing.cn

export const a = 1;  import { a } from "./m.js";
来源：http://bw.huixiangedu.cn

[U84] JS：CommonJS 写法
来源：http://rr.nicolike.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ov.shtwfgs.cn

[U85] JS：可选链
来源：http://wn.asd995.cn

a?.b?.c
来源：http://dh.hahajie.cn

[U86] JS：空值合并
来源：http://of.bookmarksfly.cn

a ?? b
来源：http://eo.yuntaijiaju.cn

[U87] JS：解构默认值
来源：http://ju.muxihuayi.cn

const { a = 1, b = 2 } = obj;
来源：http://ln.huixiangedu.cn

[U88] JS：对象展开合并
来源：http://jl.huixinmuqiang.cn

{ ...a, ...b }
来源：http://sc.yuexingan06.cn

[U89] JS：数组去重
来源：http://ez.jianghongdianzi.cn

[...new Set(arr)]
来源：http://gx.521024.cn

[U90] JS：数字数组排序
来源：http://vg.szsharing.cn

[...arr].sort((a, b) => a - b)
来源：http://xk.hnjuh.cn

[U91] JS：对象键值遍历
来源：http://xc.muxihuayi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jf.panjiajie.cn

[U92] JS：深拷贝
来源：http://wd.shxzukj.cn

structuredClone(obj)
来源：http://ho.nicolike.cn

[U93] JS：模板字符串
来源：http://aj.haigaiapp.cn

`共 ${n} 条`
来源：http://nx.szxytkj.cn

[U94] JS：箭头函数
来源：http://jg.yuntaijiaju.cn

const double = x => x * 2;
来源：http://fs.newstarts.cn

[U95] JS：Promise 包装
来源：http://is.gzmigu.cn

new Promise((resolve, reject) => {})
来源：http://lt.yuntaijiaju.cn

[U96] JS：async/await 与异常
来源：http://ee.shxzukj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://te.shxzukj.cn


<!-- 参考信息 -->