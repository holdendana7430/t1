代发 wailian999

[T07] Kotlin：集合过滤
来源：http://dj.haigaiapp.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ul.colortex.cn

[T08] Kotlin：数据类
来源：http://yk.huixiangedu.cn

data class User(val name: String, val age: Int)
来源：http://di.nszjky.cn

[T09] Kotlin：扩展函数
来源：http://yo.nicolike.cn

fun String.exclaim() = this + "!"
来源：http://qz.szxytkj.cn

[T10] Kotlin：默认参数
来源：http://tl.nszjky.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pm.jianghongdianzi.cn

[T11] Kotlin：协程
来源：http://sl.9csxet.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://lk.chemitech.net.cn

[T12] Kotlin：解构声明
来源：http://fa.shxzukj.cn

val (a, b) = Pair(1, 2)
来源：http://nk.huanxung.cn

[T13] Kotlin：只读 Map
来源：http://kn.szsharing.cn

val m = mapOf("a" to 1)
来源：http://uj.shxzukj.cn

[T14] Kotlin：循环
来源：http://zr.shxzukj.cn

for (i in 1..10) println(i)
来源：http://tn.shxzukj.cn

[T15] Kotlin：接口
来源：http://ni.huanxung.cn

interface Shape { fun area(): Double }
来源：http://aq.lnxyls.cn

[T16] Swift：Hello World
来源：http://vh.jianghongdianzi.cn

print("Hello")
来源：http://ri.bookmarksfly.cn

[T17] Swift：变量与常量
来源：http://pe.colortex.cn

var a = 1;  let b = 2
来源：http://rj.colortex.cn

[T18] Swift：字符串插值
来源：http://lm.chemitech.net.cn

"值: \(b)"
来源：http://xu.shxzskj.cn

[T19] Swift：可选绑定
来源：http://hs.jianghongdianzi.cn

if let n = opt { print(n) }
来源：http://dd.bookmarksfly.cn

[T20] Swift：数组操作
来源：http://nk.huixinmuqiang.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xq.hnjuh.cn

[T21] Swift：遍历
来源：http://bs.nszjky.cn

for x in a { print(x) }
来源：http://kr.asd995.cn

[T22] Swift：字典
来源：http://jj.gzmigu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://gi.muxihuayi.cn

[T23] Swift：函数
来源：http://bu.hnjuh.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ip.newstarts.cn

[T24] Swift：闭包
来源：http://ic.jctech888.com.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://uj.huixiangedu.cn

[T25] Swift：结构体
来源：http://ru.haigaiapp.cn

struct P { var x: Int }
来源：http://rq.yuexingan06.cn

[T26] Swift：类与重写
来源：http://mp.colortex.cn

class A: Base { override func f() {} }
来源：http://bo.shtwfgs.cn

[T27] Swift：错误处理
来源：http://eo.huixinmuqiang.cn

do { try f() } catch { print(error) }
来源：http://kx.chemitech.net.cn

[T28] Swift：枚举
来源：http://ai.9csxet.cn

enum Color { case red, green }
来源：http://kr.chemitech.net.cn

[T29] Swift：guard 提前返回
来源：http://bp.asd995.cn

guard let x = opt else { return }
来源：http://vc.bjjhwx.cn

[T30] Swift：协议
来源：http://eb.szsharing.cn

protocol Shape { func area() -> Double }
来源：http://sx.bjjhwx.cn

[T31] Lua：Hello World
来源：http://fx.colortex.cn

print("Hello")
来源：http://jt.huanxung.cn

[T32] Lua：局部变量
来源：http://xa.nicolike.cn

local a = 1
来源：http://yh.9csxet.cn

[T33] Lua：表（数组）
来源：http://lo.lnxyls.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fx.muxihuayi.cn

[T34] Lua：遍历表
来源：http://kz.huixiangedu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://va.asd995.cn

[T35] Lua：字典表
来源：http://jn.huanxung.cn

local d = { a = 1 };  d.b = 2
来源：http://uj.huixinmuqiang.cn

[T36] Lua：函数
来源：http://ge.shtwfgs.cn

function add(a, b) return a + b end
来源：http://ed.huanxung.cn

[T37] Lua：字符串拼接
来源：http://dz.haigaiapp.cn

"a" .. "b"
来源：http://df.bjjhwx.cn

[T38] Lua：条件
来源：http://lf.yuntaijiaju.cn

if x > 0 then print("正") end
来源：http://em.wgjwhj.cn

[T39] Lua：模式匹配
来源：http://qy.lnxyls.cn

string.find(s, "%d+")
来源：http://pw.lnxyls.cn

[T40] Lua：元表
来源：http://gi.szxytkj.cn

setmetatable({}, { __index = base })
来源：http://wj.haigaiapp.cn

[T41] Perl：Hello World
来源：http://mw.nszjky.cn

print "Hello\n";
来源：http://xp.asd995.cn

[T42] Perl：变量类型
来源：http://wm.shtwfgs.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ad.panjiajie.cn

[T43] Perl：字符串插值
来源：http://qo.shxzskj.cn

"值: $a"
来源：http://rg.szsharing.cn

[T44] Perl：条件
来源：http://pq.yuexingan06.cn

if ($a > 0) { print "正"; }
来源：http://hu.hahajie.cn

[T45] Perl：数组遍历
来源：http://hs.szsharing.cn

for my $x (@arr) { print $x; }
来源：http://th.nszjky.cn

[T46] Perl：哈希操作
来源：http://gd.jctech888.com.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ms.bookmarksfly.cn

[T47] Perl：正则捕获
来源：http://vh.nicolike.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pd.chemitech.net.cn

[T48] Perl：正则替换
来源：http://hi.haigaiapp.cn

$s =~ s/old/new/g;
来源：http://io.colortex.cn

[T49] Perl：函数
来源：http://hz.yuntaijiaju.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://im.jctech888.com.cn

[T50] Perl：逐行读文件
来源：http://jm.yuexingan06.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ar.colortex.cn

while (my $line = <$fh>) { print $line; }
来源：http://bd.521024.cn

[T51] Scala：Hello World
来源：http://ob.wgjwhj.cn

println("Hello")
来源：http://bx.haigaiapp.cn

[T52] Scala：变量
来源：http://mp.muxihuayi.cn

val a = 1;  var b = 2
来源：http://aw.nszjky.cn

[T53] Scala：字符串插值
来源：http://na.521024.cn

s"值: $b"
来源：http://jc.yuexingan06.cn

[T54] Scala：集合映射
来源：http://vq.szxytkj.cn

List(1, 2, 3).map(_ * 2)
来源：http://uf.hnjuh.cn

[T55] Scala：集合过滤
来源：http://pu.panjiajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fs.haigaiapp.cn

[T56] Scala：样例类
来源：http://ze.9csxet.cn

case class User(name: String, age: Int)
来源：http://vb.gzmigu.cn

[T57] Scala：模式匹配
来源：http://aw.yuntaijiaju.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://lb.wgjwhj.cn

[T58] Scala：函数定义
来源：http://bx.lnxyls.cn

def add(a: Int, b: Int): Int = a + b
来源：http://kd.9csxet.cn

[T59] Scala：循环
来源：http://nv.shtwfgs.cn

for (i <- 1 to 10) println(i)
来源：http://xl.chemitech.net.cn

[T60] Scala：折叠
来源：http://vm.bookmarksfly.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nf.shxzskj.cn

================================================================================
来源：http://xp.bjjhwx.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dx.jianghongdianzi.cn

================================================================================
来源：http://ta.lnxyls.cn

[U01] Py：创建虚拟环境
来源：http://bf.shxzukj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wm.nszjky.cn

[U02] Py：导出 / 安装依赖
来源：http://cr.bjjhwx.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uz.huanxung.cn

[U03] Py：加载 .env 配置
来源：http://zs.muxihuayi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ew.hnjuh.cn

[U04] Py：变量调试打印
来源：http://el.bookmarksfly.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ol.muxihuayi.cn

[U05] Py：列表去重且保序
来源：http://zf.jianghongdianzi.cn

list(dict.fromkeys(arr))
来源：http://fo.521024.cn

[U06] Py：合并两个字典
来源：http://xl.haigaiapp.cn

{**a, **b}
来源：http://nf.chemitech.net.cn

[U07] Py：反转字典键值
来源：http://cg.huanxung.cn

{v: k for k, v in d.items()}
来源：http://ge.shxzukj.cn

[U08] Py：展平二维列表
来源：http://pc.yuexingan06.cn

[y for x in nested for y in x]
来源：http://bk.gzmigu.cn

[U09] Py：字典取最大值的键
来源：http://io.nicolike.cn

max(d, key=d.get)
来源：http://fo.jctech888.com.cn

[U10] Py：按值排序字典
来源：http://yg.nicolike.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://st.chemitech.net.cn

[U11] Py：生成器表达式
来源：http://lc.shxzskj.cn

(x * 2 for x in arr)
来源：http://oj.muxihuayi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://hj.hnjuh.cn

Counter(arr).most_common(3)
来源：http://pu.shxzskj.cn

[U13] Py：固定长度队列
来源：http://gu.szxytkj.cn

deque(maxlen=10)
来源：http://gp.hahajie.cn

[U14] Py：分组收集到列表
来源：http://eb.szxytkj.cn

defaultdict(list)
来源：http://sf.haigaiapp.cn

[U15] Py：高精度计时
来源：http://az.colortex.cn

t = time.perf_counter()
来源：http://aw.colortex.cn

[U16] Py：命令行参数解析
来源：http://tn.hnjuh.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ru.9csxet.cn

[U17] Py：初始化日志
来源：http://ra.521024.cn

logging.basicConfig(level=logging.INFO)
来源：http://hk.521024.cn

[U18] Py：预编译正则
来源：http://eg.shxzukj.cn

pat = re.compile(r"\d+")
来源：http://vt.huanxung.cn

[U19] Py：正则替换带回调
来源：http://qs.yuntaijiaju.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zf.haigaiapp.cn

[U20] Py：缓存函数结果
来源：http://bo.huanxung.cn

@functools.lru_cache(maxsize=None)
来源：http://er.newstarts.cn

[U21] Py：自定义上下文管理器
来源：http://bn.9csxet.cn

@contextlib.contextmanager
来源：http://ah.nicolike.cn

[U22] Py：矩阵转置
来源：http://hn.muxihuayi.cn

list(zip(*m))
来源：http://zv.yuexingan06.cn

[U23] Py：分块读取大文件
来源：http://az.nicolike.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xm.yuntaijiaju.cn

[U24] Py：路径操作
来源：http://fu.wgjwhj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wg.chemitech.net.cn

[U25] Py：CSV 按字典读
来源：http://jl.newstarts.cn

csv.DictReader(f)
来源：http://af.bookmarksfly.cn

[U26] Py：并发下载
来源：http://rd.huixiangedu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://td.lnxyls.cn

[U27] Py：异步 HTTP
来源：http://vm.newstarts.cn

aiohttp.ClientSession() 配合 async with
来源：http://nr.lnxyls.cn

[U28] Py：类型别名
来源：http://mg.muxihuayi.cn

UserId = int
来源：http://sd.shxzskj.cn

[U29] Py：属性校验
来源：http://of.wgjwhj.cn

@property 与 @x.setter 配合
来源：http://lb.panjiajie.cn

[U30] Py：数据类
来源：http://ss.haigaiapp.cn

@dataclass(slots=True)
来源：http://yk.szxytkj.cn

[U31] Py：单测
来源：http://oh.jctech888.com.cn

python -m pytest -q
来源：http://jr.colortex.cn

[U32] Py：代码格式化
来源：http://kr.bjjhwx.cn

ruff format . && ruff check --fix .
来源：http://qt.haigaiapp.cn

[U33] Py：打包发布
来源：http://rm.muxihuayi.cn

python -m build  （依赖 pyproject.toml）
来源：http://rs.bjjhwx.cn

[U34] Py：判断编码
来源：http://dw.wgjwhj.cn

chardet.detect(raw)
来源：http://te.nicolike.cn

[U35] Py：发送邮件
来源：http://di.shtwfgs.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xn.gzmigu.cn

[U36] Py：定时任务
来源：http://pd.bjjhwx.cn

schedule.every(10).minutes.do(job)
来源：http://jo.hahajie.cn

[U37] Py：读写 Excel
来源：http://pj.huixiangedu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://zo.szxytkj.cn

[U38] Py：获取脚本所在目录
来源：http://lb.shxzskj.cn

Path(__file__).resolve().parent
来源：http://tt.wgjwhj.cn

[U39] Py：判断是否在交互环境
来源：http://ar.huixinmuqiang.cn

sys.stdout.isatty()
来源：http://zh.gzmigu.cn

[U40] Py：打印到标准错误
来源：http://uk.hahajie.cn

print("err", file=sys.stderr)
来源：http://pc.nszjky.cn

[U41] PHP：初始化 Composer 项目
来源：http://hq.colortex.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://du.jianghongdianzi.cn

[U42] PHP：PSR-4 自动加载
来源：http://rv.haigaiapp.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gk.hahajie.cn

[U43] PHP：声明命名空间
来源：http://ol.wgjwhj.cn

namespace App\Http;
来源：http://ko.muxihuayi.cn

[U44] PHP：开启严格类型
来源：http://wz.lnxyls.cn

declare(strict_types=1);
来源：http://qu.haigaiapp.cn

[U45] PHP：类型声明与返回类型
来源：http://cz.szsharing.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ag.wgjwhj.cn

[U46] PHP：可空类型
来源：http://dl.newstarts.cn

?string $name = null
来源：http://cc.yuexingan06.cn

[U47] PHP：联合类型
来源：http://zh.bookmarksfly.cn

int|string $id
来源：http://if.colortex.cn

[U48] PHP：纯枚举
来源：http://te.newstarts.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rp.haigaiapp.cn

[U49] PHP：只读属性
来源：http://tm.yuntaijiaju.cn

public readonly string $name
来源：http://it.jianghongdianzi.cn

[U50] PHP：构造器属性提升
来源：http://cs.muxihuayi.cn

public function __construct(private int $id) {}
来源：http://dv.jianghongdianzi.cn

[U51] PHP：数组解构
来源：http://tt.nszjky.cn

[$a, $b] = $arr;
来源：http://lr.nszjky.cn

[U52] PHP：箭头函数
来源：http://zy.huixiangedu.cn

$double = fn($x) => $x * 2;
来源：http://ek.lnxyls.cn

[U53] PHP：空合并运算符
来源：http://xz.gzmigu.cn

$v = $a ?? $b ?? "default";
来源：http://yk.hahajie.cn

[U54] PHP：空安全调用
来源：http://nm.jctech888.com.cn

$obj?->method()
来源：http://mp.yuexingan06.cn

[U55] PHP：match 表达式
来源：http://tn.hnjuh.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ni.szxytkj.cn

[U56] PHP：命名参数
来源：http://cb.hnjuh.cn

f(a: 1, b: 2)
来源：http://wa.huixinmuqiang.cn

[U57] PHP：字符串插值
来源：http://oi.szsharing.cn

"值: {$a}"
来源：http://ar.9csxet.cn

[U58] PHP：数组三件套
来源：http://ca.521024.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jt.wgjwhj.cn

[U59] PHP：自定义排序
来源：http://ep.asd995.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://en.szxytkj.cn

[U60] PHP：JSON 编解码
来源：http://ne.muxihuayi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pp.yuexingan06.cn

[U61] PHP：正则
来源：http://tk.wgjwhj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wr.huixinmuqiang.cn

[U62] PHP：日期对象
来源：http://su.haigaiapp.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vv.huanxung.cn

[U63] PHP：文件读写
来源：http://vq.haigaiapp.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fj.gzmigu.cn

[U64] PHP：目录遍历
来源：http://mt.shxzukj.cn

glob("dir/*.php");  scandir("dir");
来源：http://nc.hnjuh.cn

[U65] PHP：会话
来源：http://qt.nicolike.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://bg.521024.cn

[U66] PHP：设置 Cookie
来源：http://el.shtwfgs.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://uh.wgjwhj.cn

[U67] PHP：处理文件上传
来源：http://vj.szsharing.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fr.bjjhwx.cn

[U68] PHP：PDO 连接
来源：http://uq.colortex.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lw.gzmigu.cn

[U69] PHP：PDO 预处理
来源：http://nd.panjiajie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hf.panjiajie.cn

[U70] PHP：PDO 事务
来源：http://oi.muxihuayi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gr.huixinmuqiang.cn

[U71] PHP：抛出异常
来源：http://tg.yuexingan06.cn

throw new RuntimeException("失败", 500);
来源：http://xe.colortex.cn

[U72] PHP：写错误日志
来源：http://it.shtwfgs.cn

error_log("失败: " . $e->getMessage());
来源：http://rg.colortex.cn

[U73] PHP：读取 ini 配置
来源：http://hq.nicolike.cn

parse_ini_file("config.ini", true)
来源：http://bt.shtwfgs.cn

[U74] PHP：读取环境变量
来源：http://js.shxzskj.cn

getenv("APP_ENV") ?: "production"
来源：http://ft.gzmigu.cn

[U75] PHP：依赖注入
来源：http://is.huixinmuqiang.cn

composer require psr/container
来源：http://ak.lnxyls.cn

[U76] PHP：简单路由
来源：http://zm.jianghongdianzi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tm.nicolike.cn

[U77] PHP：模板渲染
来源：http://qr.huixiangedu.cn

composer require twig/twig
来源：http://we.huixiangedu.cn

[U78] PHP：单元测试
来源：http://ym.haigaiapp.cn

composer require --dev phpunit/phpunit
来源：http://oq.wgjwhj.cn

[U79] PHP：静态分析
来源：http://pf.huixiangedu.cn

composer require --dev phpstan/phpstan
来源：http://il.bjjhwx.cn

[U80] PHP：代码规范修复
来源：http://vi.szxytkj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://au.asd995.cn

[U81] JS：初始化项目
来源：http://zz.gzmigu.cn

npm init -y;  npm i express
来源：http://io.shxzukj.cn

[U82] JS：package.json 脚本
来源：http://wv.shxzukj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vw.panjiajie.cn

[U83] JS：ES Module 导入导出
来源：http://ge.colortex.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zq.nszjky.cn

[U84] JS：CommonJS 写法
来源：http://ed.colortex.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wb.yuntaijiaju.cn

[U85] JS：可选链
来源：http://ja.bjjhwx.cn

a?.b?.c
来源：http://ot.asd995.cn

[U86] JS：空值合并
来源：http://bl.nicolike.cn

a ?? b
来源：http://oj.nszjky.cn

[U87] JS：解构默认值
来源：http://hz.panjiajie.cn

const { a = 1, b = 2 } = obj;
来源：http://vu.szsharing.cn

[U88] JS：对象展开合并
来源：http://sv.gzmigu.cn

{ ...a, ...b }
来源：http://jy.asd995.cn

[U89] JS：数组去重
来源：http://ig.jianghongdianzi.cn

[...new Set(arr)]
来源：http://ew.newstarts.cn

[U90] JS：数字数组排序
来源：http://cj.panjiajie.cn

[...arr].sort((a, b) => a - b)
来源：http://tg.hahajie.cn

[U91] JS：对象键值遍历
来源：http://ns.nicolike.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://an.asd995.cn

[U92] JS：深拷贝
来源：http://fo.521024.cn

structuredClone(obj)
来源：http://lb.chemitech.net.cn

[U93] JS：模板字符串
来源：http://df.nicolike.cn

`共 ${n} 条`
来源：http://gf.521024.cn

[U94] JS：箭头函数
来源：http://ef.yuntaijiaju.cn

const double = x => x * 2;
来源：http://dw.nszjky.cn


<!-- 参考信息 -->