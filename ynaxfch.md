代发 wailian999

[T09] Kotlin：扩展函数
来源：http://qq.hnjuh.cn

fun String.exclaim() = this + "!"
来源：http://ln.huixiangedu.cn

[T10] Kotlin：默认参数
来源：http://vh.huixiangedu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ac.9csxet.cn

[T11] Kotlin：协程
来源：http://gf.hnjuh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://tf.huanxung.cn

[T12] Kotlin：解构声明
来源：http://kj.hahajie.cn

val (a, b) = Pair(1, 2)
来源：http://bf.yuntaijiaju.cn

[T13] Kotlin：只读 Map
来源：http://jg.shtwfgs.cn

val m = mapOf("a" to 1)
来源：http://ds.shxzukj.cn

[T14] Kotlin：循环
来源：http://im.muxihuayi.cn

for (i in 1..10) println(i)
来源：http://sv.nszjky.cn

[T15] Kotlin：接口
来源：http://ps.muxihuayi.cn

interface Shape { fun area(): Double }
来源：http://qz.chemitech.net.cn

[T16] Swift：Hello World
来源：http://kj.szxytkj.cn

print("Hello")
来源：http://nz.521024.cn

[T17] Swift：变量与常量
来源：http://ml.wgjwhj.cn

var a = 1;  let b = 2
来源：http://pm.wgjwhj.cn

[T18] Swift：字符串插值
来源：http://xn.nicolike.cn

"值: \(b)"
来源：http://xj.yuexingan06.cn

[T19] Swift：可选绑定
来源：http://ls.huixiangedu.cn

if let n = opt { print(n) }
来源：http://my.asd995.cn

[T20] Swift：数组操作
来源：http://id.hahajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qw.yuntaijiaju.cn

[T21] Swift：遍历
来源：http://xi.shxzukj.cn

for x in a { print(x) }
来源：http://ay.hahajie.cn

[T22] Swift：字典
来源：http://px.bjjhwx.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ax.nszjky.cn

[T23] Swift：函数
来源：http://sh.yuexingan06.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sb.hnjuh.cn

[T24] Swift：闭包
来源：http://ax.nicolike.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://hv.jctech888.com.cn

[T25] Swift：结构体
来源：http://wg.newstarts.cn

struct P { var x: Int }
来源：http://cg.bjjhwx.cn

[T26] Swift：类与重写
来源：http://ua.shxzskj.cn

class A: Base { override func f() {} }
来源：http://yq.gzmigu.cn

[T27] Swift：错误处理
来源：http://ap.jianghongdianzi.cn

do { try f() } catch { print(error) }
来源：http://qj.huanxung.cn

[T28] Swift：枚举
来源：http://eu.yuntaijiaju.cn

enum Color { case red, green }
来源：http://ga.jianghongdianzi.cn

[T29] Swift：guard 提前返回
来源：http://uf.jctech888.com.cn

guard let x = opt else { return }
来源：http://pn.yuntaijiaju.cn

[T30] Swift：协议
来源：http://hb.huixiangedu.cn

protocol Shape { func area() -> Double }
来源：http://qi.yuexingan06.cn

[T31] Lua：Hello World
来源：http://ts.haigaiapp.cn

print("Hello")
来源：http://ay.huanxung.cn

[T32] Lua：局部变量
来源：http://mw.nicolike.cn

local a = 1
来源：http://kl.haigaiapp.cn

[T33] Lua：表（数组）
来源：http://kj.haigaiapp.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://qa.hnjuh.cn

[T34] Lua：遍历表
来源：http://ti.haigaiapp.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://bi.nicolike.cn

[T35] Lua：字典表
来源：http://hd.newstarts.cn

local d = { a = 1 };  d.b = 2
来源：http://ja.bjjhwx.cn

[T36] Lua：函数
来源：http://nk.hnjuh.cn

function add(a, b) return a + b end
来源：http://do.9csxet.cn

[T37] Lua：字符串拼接
来源：http://da.asd995.cn

"a" .. "b"
来源：http://nr.panjiajie.cn

[T38] Lua：条件
来源：http://ns.hahajie.cn

if x > 0 then print("正") end
来源：http://pq.bookmarksfly.cn

[T39] Lua：模式匹配
来源：http://gk.hahajie.cn

string.find(s, "%d+")
来源：http://cg.jianghongdianzi.cn

[T40] Lua：元表
来源：http://wn.nicolike.cn

setmetatable({}, { __index = base })
来源：http://by.szxytkj.cn

[T41] Perl：Hello World
来源：http://rz.haigaiapp.cn

print "Hello\n";
来源：http://zv.bjjhwx.cn

[T42] Perl：变量类型
来源：http://pu.hahajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mn.colortex.cn

[T43] Perl：字符串插值
来源：http://kz.chemitech.net.cn

"值: $a"
来源：http://ux.szxytkj.cn

[T44] Perl：条件
来源：http://mb.szsharing.cn

if ($a > 0) { print "正"; }
来源：http://oq.huixiangedu.cn

[T45] Perl：数组遍历
来源：http://ji.asd995.cn

for my $x (@arr) { print $x; }
来源：http://gn.gzmigu.cn

[T46] Perl：哈希操作
来源：http://mt.9csxet.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vt.haigaiapp.cn

[T47] Perl：正则捕获
来源：http://gl.gzmigu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://of.wgjwhj.cn

[T48] Perl：正则替换
来源：http://vp.jctech888.com.cn

$s =~ s/old/new/g;
来源：http://ax.hahajie.cn

[T49] Perl：函数
来源：http://gj.huixiangedu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zw.521024.cn

[T50] Perl：逐行读文件
来源：http://wz.wgjwhj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://kj.shtwfgs.cn

while (my $line = <$fh>) { print $line; }
来源：http://mo.hnjuh.cn

[T51] Scala：Hello World
来源：http://ap.nszjky.cn

println("Hello")
来源：http://vb.yuntaijiaju.cn

[T52] Scala：变量
来源：http://sg.lnxyls.cn

val a = 1;  var b = 2
来源：http://fx.yuntaijiaju.cn

[T53] Scala：字符串插值
来源：http://bj.hahajie.cn

s"值: $b"
来源：http://or.newstarts.cn

[T54] Scala：集合映射
来源：http://aq.asd995.cn

List(1, 2, 3).map(_ * 2)
来源：http://ob.shtwfgs.cn

[T55] Scala：集合过滤
来源：http://ci.szsharing.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xv.gzmigu.cn

[T56] Scala：样例类
来源：http://va.newstarts.cn

case class User(name: String, age: Int)
来源：http://aj.hahajie.cn

[T57] Scala：模式匹配
来源：http://xw.bookmarksfly.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vc.521024.cn

[T58] Scala：函数定义
来源：http://fi.newstarts.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zt.nszjky.cn

[T59] Scala：循环
来源：http://xz.lnxyls.cn

for (i <- 1 to 10) println(i)
来源：http://hv.shxzukj.cn

[T60] Scala：折叠
来源：http://wb.bjjhwx.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ae.9csxet.cn

================================================================================
来源：http://ym.bjjhwx.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zf.szxytkj.cn

================================================================================
来源：http://kd.9csxet.cn

[U01] Py：创建虚拟环境
来源：http://yh.huanxung.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wm.521024.cn

[U02] Py：导出 / 安装依赖
来源：http://zq.yuexingan06.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tl.colortex.cn

[U03] Py：加载 .env 配置
来源：http://uk.huixinmuqiang.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://vr.521024.cn

[U04] Py：变量调试打印
来源：http://eq.nicolike.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vh.shxzukj.cn

[U05] Py：列表去重且保序
来源：http://uq.muxihuayi.cn

list(dict.fromkeys(arr))
来源：http://qw.hahajie.cn

[U06] Py：合并两个字典
来源：http://dy.9csxet.cn

{**a, **b}
来源：http://oy.yuexingan06.cn

[U07] Py：反转字典键值
来源：http://ei.huixiangedu.cn

{v: k for k, v in d.items()}
来源：http://iu.huixinmuqiang.cn

[U08] Py：展平二维列表
来源：http://kw.shtwfgs.cn

[y for x in nested for y in x]
来源：http://pr.jctech888.com.cn

[U09] Py：字典取最大值的键
来源：http://gh.shxzukj.cn

max(d, key=d.get)
来源：http://wk.chemitech.net.cn

[U10] Py：按值排序字典
来源：http://ke.asd995.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://py.szsharing.cn

[U11] Py：生成器表达式
来源：http://yd.9csxet.cn

(x * 2 for x in arr)
来源：http://dd.jianghongdianzi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ry.panjiajie.cn

Counter(arr).most_common(3)
来源：http://mo.521024.cn

[U13] Py：固定长度队列
来源：http://up.521024.cn

deque(maxlen=10)
来源：http://gf.shxzskj.cn

[U14] Py：分组收集到列表
来源：http://ey.jctech888.com.cn

defaultdict(list)
来源：http://tm.muxihuayi.cn

[U15] Py：高精度计时
来源：http://ph.yuntaijiaju.cn

t = time.perf_counter()
来源：http://rp.yuntaijiaju.cn

[U16] Py：命令行参数解析
来源：http://mj.521024.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://to.hahajie.cn

[U17] Py：初始化日志
来源：http://hz.bookmarksfly.cn

logging.basicConfig(level=logging.INFO)
来源：http://og.chemitech.net.cn

[U18] Py：预编译正则
来源：http://tj.shxzukj.cn

pat = re.compile(r"\d+")
来源：http://yy.hnjuh.cn

[U19] Py：正则替换带回调
来源：http://cg.shxzskj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rc.chemitech.net.cn

[U20] Py：缓存函数结果
来源：http://be.yuexingan06.cn

@functools.lru_cache(maxsize=None)
来源：http://ca.jianghongdianzi.cn

[U21] Py：自定义上下文管理器
来源：http://et.bookmarksfly.cn

@contextlib.contextmanager
来源：http://jv.colortex.cn

[U22] Py：矩阵转置
来源：http://af.yuntaijiaju.cn

list(zip(*m))
来源：http://gv.gzmigu.cn

[U23] Py：分块读取大文件
来源：http://lm.wgjwhj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xr.haigaiapp.cn

[U24] Py：路径操作
来源：http://gj.shxzskj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ph.hahajie.cn

[U25] Py：CSV 按字典读
来源：http://dz.panjiajie.cn

csv.DictReader(f)
来源：http://kt.shxzskj.cn

[U26] Py：并发下载
来源：http://aj.lnxyls.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://un.yuexingan06.cn

[U27] Py：异步 HTTP
来源：http://il.asd995.cn

aiohttp.ClientSession() 配合 async with
来源：http://yn.huanxung.cn

[U28] Py：类型别名
来源：http://oz.haigaiapp.cn

UserId = int
来源：http://kn.gzmigu.cn

[U29] Py：属性校验
来源：http://rc.chemitech.net.cn

@property 与 @x.setter 配合
来源：http://mt.wgjwhj.cn

[U30] Py：数据类
来源：http://se.szxytkj.cn

@dataclass(slots=True)
来源：http://vk.wgjwhj.cn

[U31] Py：单测
来源：http://wi.shxzskj.cn

python -m pytest -q
来源：http://aw.huixiangedu.cn

[U32] Py：代码格式化
来源：http://zp.521024.cn

ruff format . && ruff check --fix .
来源：http://ps.panjiajie.cn

[U33] Py：打包发布
来源：http://ek.colortex.cn

python -m build  （依赖 pyproject.toml）
来源：http://by.haigaiapp.cn

[U34] Py：判断编码
来源：http://ww.szxytkj.cn

chardet.detect(raw)
来源：http://la.panjiajie.cn

[U35] Py：发送邮件
来源：http://pn.521024.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qx.muxihuayi.cn

[U36] Py：定时任务
来源：http://uf.huixinmuqiang.cn

schedule.every(10).minutes.do(job)
来源：http://xf.lnxyls.cn

[U37] Py：读写 Excel
来源：http://oj.hahajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://oo.panjiajie.cn

[U38] Py：获取脚本所在目录
来源：http://mk.gzmigu.cn

Path(__file__).resolve().parent
来源：http://oe.gzmigu.cn

[U39] Py：判断是否在交互环境
来源：http://tb.9csxet.cn

sys.stdout.isatty()
来源：http://mm.panjiajie.cn

[U40] Py：打印到标准错误
来源：http://ig.yuexingan06.cn

print("err", file=sys.stderr)
来源：http://la.haigaiapp.cn

[U41] PHP：初始化 Composer 项目
来源：http://qs.jianghongdianzi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ow.521024.cn

[U42] PHP：PSR-4 自动加载
来源：http://sw.panjiajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yr.jianghongdianzi.cn

[U43] PHP：声明命名空间
来源：http://sc.lnxyls.cn

namespace App\Http;
来源：http://iy.haigaiapp.cn

[U44] PHP：开启严格类型
来源：http://jl.huanxung.cn

declare(strict_types=1);
来源：http://qq.shxzskj.cn

[U45] PHP：类型声明与返回类型
来源：http://ax.newstarts.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://xh.bookmarksfly.cn

[U46] PHP：可空类型
来源：http://xu.huixiangedu.cn

?string $name = null
来源：http://ek.bookmarksfly.cn

[U47] PHP：联合类型
来源：http://hw.shtwfgs.cn

int|string $id
来源：http://yc.nszjky.cn

[U48] PHP：纯枚举
来源：http://gc.huanxung.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gu.shxzskj.cn

[U49] PHP：只读属性
来源：http://jr.szsharing.cn

public readonly string $name
来源：http://ym.bookmarksfly.cn

[U50] PHP：构造器属性提升
来源：http://yk.huanxung.cn

public function __construct(private int $id) {}
来源：http://zq.hahajie.cn

[U51] PHP：数组解构
来源：http://rn.gzmigu.cn

[$a, $b] = $arr;
来源：http://wv.huanxung.cn

[U52] PHP：箭头函数
来源：http://rb.huixinmuqiang.cn

$double = fn($x) => $x * 2;
来源：http://ta.yuntaijiaju.cn

[U53] PHP：空合并运算符
来源：http://nd.nicolike.cn

$v = $a ?? $b ?? "default";
来源：http://lk.nicolike.cn

[U54] PHP：空安全调用
来源：http://je.wgjwhj.cn

$obj?->method()
来源：http://lw.asd995.cn

[U55] PHP：match 表达式
来源：http://ag.yuntaijiaju.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ya.nicolike.cn

[U56] PHP：命名参数
来源：http://wj.chemitech.net.cn

f(a: 1, b: 2)
来源：http://sx.newstarts.cn

[U57] PHP：字符串插值
来源：http://gt.colortex.cn

"值: {$a}"
来源：http://zd.nicolike.cn

[U58] PHP：数组三件套
来源：http://ud.huixinmuqiang.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hb.bookmarksfly.cn

[U59] PHP：自定义排序
来源：http://mc.yuexingan06.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vf.huixinmuqiang.cn

[U60] PHP：JSON 编解码
来源：http://ub.huanxung.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://uz.newstarts.cn

[U61] PHP：正则
来源：http://zt.muxihuayi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zs.nicolike.cn

[U62] PHP：日期对象
来源：http://gq.jctech888.com.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://oz.nszjky.cn

[U63] PHP：文件读写
来源：http://za.yuntaijiaju.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fw.hahajie.cn

[U64] PHP：目录遍历
来源：http://at.521024.cn

glob("dir/*.php");  scandir("dir");
来源：http://vm.newstarts.cn

[U65] PHP：会话
来源：http://am.panjiajie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://wd.gzmigu.cn

[U66] PHP：设置 Cookie
来源：http://qy.shxzskj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xr.gzmigu.cn

[U67] PHP：处理文件上传
来源：http://lv.newstarts.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://td.nszjky.cn

[U68] PHP：PDO 连接
来源：http://pu.jctech888.com.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pe.panjiajie.cn

[U69] PHP：PDO 预处理
来源：http://mq.521024.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pz.9csxet.cn

[U70] PHP：PDO 事务
来源：http://vt.lnxyls.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dk.shtwfgs.cn

[U71] PHP：抛出异常
来源：http://jc.hnjuh.cn

throw new RuntimeException("失败", 500);
来源：http://df.gzmigu.cn

[U72] PHP：写错误日志
来源：http://zn.gzmigu.cn

error_log("失败: " . $e->getMessage());
来源：http://ko.szsharing.cn

[U73] PHP：读取 ini 配置
来源：http://xi.jianghongdianzi.cn

parse_ini_file("config.ini", true)
来源：http://ze.asd995.cn

[U74] PHP：读取环境变量
来源：http://md.bjjhwx.cn

getenv("APP_ENV") ?: "production"
来源：http://vp.yuexingan06.cn

[U75] PHP：依赖注入
来源：http://iv.szxytkj.cn

composer require psr/container
来源：http://zx.huixinmuqiang.cn

[U76] PHP：简单路由
来源：http://yc.nszjky.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kq.newstarts.cn

[U77] PHP：模板渲染
来源：http://fq.bjjhwx.cn

composer require twig/twig
来源：http://ed.jctech888.com.cn

[U78] PHP：单元测试
来源：http://ig.bookmarksfly.cn

composer require --dev phpunit/phpunit
来源：http://ou.chemitech.net.cn

[U79] PHP：静态分析
来源：http://ov.bjjhwx.cn

composer require --dev phpstan/phpstan
来源：http://ff.asd995.cn

[U80] PHP：代码规范修复
来源：http://tz.colortex.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jw.9csxet.cn

[U81] JS：初始化项目
来源：http://by.panjiajie.cn

npm init -y;  npm i express
来源：http://rt.lnxyls.cn

[U82] JS：package.json 脚本
来源：http://jq.huanxung.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qq.yuntaijiaju.cn

[U83] JS：ES Module 导入导出
来源：http://bg.gzmigu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qa.bookmarksfly.cn

[U84] JS：CommonJS 写法
来源：http://bp.bookmarksfly.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ib.huixinmuqiang.cn

[U85] JS：可选链
来源：http://tc.shtwfgs.cn

a?.b?.c
来源：http://ui.huanxung.cn

[U86] JS：空值合并
来源：http://wa.muxihuayi.cn

a ?? b
来源：http://lu.yuexingan06.cn

[U87] JS：解构默认值
来源：http://cn.hnjuh.cn

const { a = 1, b = 2 } = obj;
来源：http://vt.gzmigu.cn

[U88] JS：对象展开合并
来源：http://qx.wgjwhj.cn

{ ...a, ...b }
来源：http://pg.hahajie.cn

[U89] JS：数组去重
来源：http://zn.shxzskj.cn

[...new Set(arr)]
来源：http://zx.521024.cn

[U90] JS：数字数组排序
来源：http://lu.hahajie.cn

[...arr].sort((a, b) => a - b)
来源：http://hd.szsharing.cn

[U91] JS：对象键值遍历
来源：http://ou.shxzukj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://be.szsharing.cn

[U92] JS：深拷贝
来源：http://cp.jctech888.com.cn

structuredClone(obj)
来源：http://gh.lnxyls.cn

[U93] JS：模板字符串
来源：http://jk.bjjhwx.cn

`共 ${n} 条`
来源：http://iz.huixinmuqiang.cn

[U94] JS：箭头函数
来源：http://ly.nicolike.cn

const double = x => x * 2;
来源：http://ba.panjiajie.cn

[U95] JS：Promise 包装
来源：http://ky.gzmigu.cn

new Promise((resolve, reject) => {})
来源：http://hs.shxzskj.cn

[U96] JS：async/await 与异常
来源：http://tc.huixinmuqiang.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zp.muxihuayi.cn


<!-- 参考信息 -->