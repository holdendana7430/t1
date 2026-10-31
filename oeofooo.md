代发 wailian999

[T09] Kotlin：扩展函数
来源：http://gl.szsharing.cn

fun String.exclaim() = this + "!"
来源：http://lx.haigaiapp.cn

[T10] Kotlin：默认参数
来源：http://ej.shxzskj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://lb.hahajie.cn

[T11] Kotlin：协程
来源：http://xa.muxihuayi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vi.lnxyls.cn

[T12] Kotlin：解构声明
来源：http://qj.muxihuayi.cn

val (a, b) = Pair(1, 2)
来源：http://cj.shtwfgs.cn

[T13] Kotlin：只读 Map
来源：http://pj.huixiangedu.cn

val m = mapOf("a" to 1)
来源：http://du.wgjwhj.cn

[T14] Kotlin：循环
来源：http://zv.shtwfgs.cn

for (i in 1..10) println(i)
来源：http://ry.huixinmuqiang.cn

[T15] Kotlin：接口
来源：http://zb.shtwfgs.cn

interface Shape { fun area(): Double }
来源：http://aj.asd995.cn

[T16] Swift：Hello World
来源：http://mx.jctech888.com.cn

print("Hello")
来源：http://gx.panjiajie.cn

[T17] Swift：变量与常量
来源：http://ln.shxzskj.cn

var a = 1;  let b = 2
来源：http://yh.gzmigu.cn

[T18] Swift：字符串插值
来源：http://eo.wgjwhj.cn

"值: \(b)"
来源：http://fx.huixinmuqiang.cn

[T19] Swift：可选绑定
来源：http://wy.newstarts.cn

if let n = opt { print(n) }
来源：http://bl.521024.cn

[T20] Swift：数组操作
来源：http://ml.521024.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ve.yuexingan06.cn

[T21] Swift：遍历
来源：http://sr.shxzukj.cn

for x in a { print(x) }
来源：http://cb.huixiangedu.cn

[T22] Swift：字典
来源：http://wj.szsharing.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xd.muxihuayi.cn

[T23] Swift：函数
来源：http://mp.asd995.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cz.yuexingan06.cn

[T24] Swift：闭包
来源：http://ip.jianghongdianzi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://us.shtwfgs.cn

[T25] Swift：结构体
来源：http://mg.szsharing.cn

struct P { var x: Int }
来源：http://vg.huanxung.cn

[T26] Swift：类与重写
来源：http://ha.yuntaijiaju.cn

class A: Base { override func f() {} }
来源：http://sr.hahajie.cn

[T27] Swift：错误处理
来源：http://gv.szxytkj.cn

do { try f() } catch { print(error) }
来源：http://ol.colortex.cn

[T28] Swift：枚举
来源：http://pn.huixiangedu.cn

enum Color { case red, green }
来源：http://hr.shxzskj.cn

[T29] Swift：guard 提前返回
来源：http://sk.shxzukj.cn

guard let x = opt else { return }
来源：http://gu.huanxung.cn

[T30] Swift：协议
来源：http://hp.wgjwhj.cn

protocol Shape { func area() -> Double }
来源：http://wy.hahajie.cn

[T31] Lua：Hello World
来源：http://vv.huixiangedu.cn

print("Hello")
来源：http://ej.hahajie.cn

[T32] Lua：局部变量
来源：http://pj.huixiangedu.cn

local a = 1
来源：http://mp.wgjwhj.cn

[T33] Lua：表（数组）
来源：http://qq.bjjhwx.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ao.shxzskj.cn

[T34] Lua：遍历表
来源：http://xy.jctech888.com.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ec.szxytkj.cn

[T35] Lua：字典表
来源：http://ja.jianghongdianzi.cn

local d = { a = 1 };  d.b = 2
来源：http://gj.bjjhwx.cn

[T36] Lua：函数
来源：http://cj.hnjuh.cn

function add(a, b) return a + b end
来源：http://ui.haigaiapp.cn

[T37] Lua：字符串拼接
来源：http://ar.gzmigu.cn

"a" .. "b"
来源：http://ts.yuexingan06.cn

[T38] Lua：条件
来源：http://vd.gzmigu.cn

if x > 0 then print("正") end
来源：http://ik.haigaiapp.cn

[T39] Lua：模式匹配
来源：http://nf.haigaiapp.cn

string.find(s, "%d+")
来源：http://cs.huixiangedu.cn

[T40] Lua：元表
来源：http://ei.huixinmuqiang.cn

setmetatable({}, { __index = base })
来源：http://lj.yuntaijiaju.cn

[T41] Perl：Hello World
来源：http://tf.asd995.cn

print "Hello\n";
来源：http://rr.huixinmuqiang.cn

[T42] Perl：变量类型
来源：http://hg.wgjwhj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jf.hahajie.cn

[T43] Perl：字符串插值
来源：http://cl.nszjky.cn

"值: $a"
来源：http://we.chemitech.net.cn

[T44] Perl：条件
来源：http://en.newstarts.cn

if ($a > 0) { print "正"; }
来源：http://rh.shxzskj.cn

[T45] Perl：数组遍历
来源：http://bo.asd995.cn

for my $x (@arr) { print $x; }
来源：http://uw.newstarts.cn

[T46] Perl：哈希操作
来源：http://kp.panjiajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zw.colortex.cn

[T47] Perl：正则捕获
来源：http://zy.521024.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pt.panjiajie.cn

[T48] Perl：正则替换
来源：http://kl.yuexingan06.cn

$s =~ s/old/new/g;
来源：http://ss.hahajie.cn

[T49] Perl：函数
来源：http://xj.bookmarksfly.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ft.gzmigu.cn

[T50] Perl：逐行读文件
来源：http://oy.huanxung.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://lp.gzmigu.cn

while (my $line = <$fh>) { print $line; }
来源：http://qo.newstarts.cn

[T51] Scala：Hello World
来源：http://ge.huanxung.cn

println("Hello")
来源：http://fo.haigaiapp.cn

[T52] Scala：变量
来源：http://ij.haigaiapp.cn

val a = 1;  var b = 2
来源：http://io.szsharing.cn

[T53] Scala：字符串插值
来源：http://sh.hnjuh.cn

s"值: $b"
来源：http://ua.shxzukj.cn

[T54] Scala：集合映射
来源：http://an.9csxet.cn

List(1, 2, 3).map(_ * 2)
来源：http://mr.nszjky.cn

[T55] Scala：集合过滤
来源：http://rl.bjjhwx.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ge.haigaiapp.cn

[T56] Scala：样例类
来源：http://hc.panjiajie.cn

case class User(name: String, age: Int)
来源：http://cx.lnxyls.cn

[T57] Scala：模式匹配
来源：http://rn.shxzukj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://rt.colortex.cn

[T58] Scala：函数定义
来源：http://yr.szsharing.cn

def add(a: Int, b: Int): Int = a + b
来源：http://oo.9csxet.cn

[T59] Scala：循环
来源：http://nr.bookmarksfly.cn

for (i <- 1 to 10) println(i)
来源：http://ie.yuntaijiaju.cn

[T60] Scala：折叠
来源：http://vb.panjiajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nv.shxzukj.cn

================================================================================
来源：http://yv.lnxyls.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ch.lnxyls.cn

================================================================================
来源：http://ta.nicolike.cn

[U01] Py：创建虚拟环境
来源：http://dp.gzmigu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mx.jctech888.com.cn

[U02] Py：导出 / 安装依赖
来源：http://og.9csxet.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lb.shtwfgs.cn

[U03] Py：加载 .env 配置
来源：http://dd.yuexingan06.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://za.jianghongdianzi.cn

[U04] Py：变量调试打印
来源：http://tu.yuntaijiaju.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://da.jctech888.com.cn

[U05] Py：列表去重且保序
来源：http://do.huixiangedu.cn

list(dict.fromkeys(arr))
来源：http://aw.9csxet.cn

[U06] Py：合并两个字典
来源：http://bd.hahajie.cn

{**a, **b}
来源：http://fn.huixinmuqiang.cn

[U07] Py：反转字典键值
来源：http://mk.gzmigu.cn

{v: k for k, v in d.items()}
来源：http://zm.yuntaijiaju.cn

[U08] Py：展平二维列表
来源：http://ln.jctech888.com.cn

[y for x in nested for y in x]
来源：http://vg.bookmarksfly.cn

[U09] Py：字典取最大值的键
来源：http://bt.bookmarksfly.cn

max(d, key=d.get)
来源：http://at.521024.cn

[U10] Py：按值排序字典
来源：http://ms.huanxung.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sy.gzmigu.cn

[U11] Py：生成器表达式
来源：http://rc.asd995.cn

(x * 2 for x in arr)
来源：http://yd.shtwfgs.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ur.shxzskj.cn

Counter(arr).most_common(3)
来源：http://nc.szxytkj.cn

[U13] Py：固定长度队列
来源：http://vm.bookmarksfly.cn

deque(maxlen=10)
来源：http://bl.hahajie.cn

[U14] Py：分组收集到列表
来源：http://zj.9csxet.cn

defaultdict(list)
来源：http://zv.lnxyls.cn

[U15] Py：高精度计时
来源：http://gj.shtwfgs.cn

t = time.perf_counter()
来源：http://qg.521024.cn

[U16] Py：命令行参数解析
来源：http://eb.lnxyls.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fn.newstarts.cn

[U17] Py：初始化日志
来源：http://ns.shxzukj.cn

logging.basicConfig(level=logging.INFO)
来源：http://qh.nszjky.cn

[U18] Py：预编译正则
来源：http://mu.bjjhwx.cn

pat = re.compile(r"\d+")
来源：http://fy.asd995.cn

[U19] Py：正则替换带回调
来源：http://ru.muxihuayi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tz.nicolike.cn

[U20] Py：缓存函数结果
来源：http://ky.szxytkj.cn

@functools.lru_cache(maxsize=None)
来源：http://au.shtwfgs.cn

[U21] Py：自定义上下文管理器
来源：http://uf.newstarts.cn

@contextlib.contextmanager
来源：http://nk.bjjhwx.cn

[U22] Py：矩阵转置
来源：http://uf.hnjuh.cn

list(zip(*m))
来源：http://lf.haigaiapp.cn

[U23] Py：分块读取大文件
来源：http://ac.lnxyls.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mq.shtwfgs.cn

[U24] Py：路径操作
来源：http://ee.szxytkj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zv.huixinmuqiang.cn

[U25] Py：CSV 按字典读
来源：http://cx.newstarts.cn

csv.DictReader(f)
来源：http://ls.hahajie.cn

[U26] Py：并发下载
来源：http://qe.yuntaijiaju.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xn.521024.cn

[U27] Py：异步 HTTP
来源：http://jw.jctech888.com.cn

aiohttp.ClientSession() 配合 async with
来源：http://zs.jianghongdianzi.cn

[U28] Py：类型别名
来源：http://tj.9csxet.cn

UserId = int
来源：http://dv.jctech888.com.cn

[U29] Py：属性校验
来源：http://im.nicolike.cn

@property 与 @x.setter 配合
来源：http://bx.shtwfgs.cn

[U30] Py：数据类
来源：http://qu.hnjuh.cn

@dataclass(slots=True)
来源：http://su.shxzukj.cn

[U31] Py：单测
来源：http://kj.shxzukj.cn

python -m pytest -q
来源：http://ll.panjiajie.cn

[U32] Py：代码格式化
来源：http://qr.521024.cn

ruff format . && ruff check --fix .
来源：http://yf.huixiangedu.cn

[U33] Py：打包发布
来源：http://yb.yuntaijiaju.cn

python -m build  （依赖 pyproject.toml）
来源：http://ty.panjiajie.cn

[U34] Py：判断编码
来源：http://la.hnjuh.cn

chardet.detect(raw)
来源：http://qj.hnjuh.cn

[U35] Py：发送邮件
来源：http://oi.wgjwhj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://em.lnxyls.cn

[U36] Py：定时任务
来源：http://pk.nicolike.cn

schedule.every(10).minutes.do(job)
来源：http://gp.bjjhwx.cn

[U37] Py：读写 Excel
来源：http://ig.shxzukj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://do.panjiajie.cn

[U38] Py：获取脚本所在目录
来源：http://tv.9csxet.cn

Path(__file__).resolve().parent
来源：http://rz.9csxet.cn

[U39] Py：判断是否在交互环境
来源：http://uw.jctech888.com.cn

sys.stdout.isatty()
来源：http://kh.szsharing.cn

[U40] Py：打印到标准错误
来源：http://xp.yuexingan06.cn

print("err", file=sys.stderr)
来源：http://tl.colortex.cn

[U41] PHP：初始化 Composer 项目
来源：http://eg.gzmigu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jn.chemitech.net.cn

[U42] PHP：PSR-4 自动加载
来源：http://lw.gzmigu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vc.newstarts.cn

[U43] PHP：声明命名空间
来源：http://yl.shxzukj.cn

namespace App\Http;
来源：http://cb.shtwfgs.cn

[U44] PHP：开启严格类型
来源：http://pc.jianghongdianzi.cn

declare(strict_types=1);
来源：http://bp.huixinmuqiang.cn

[U45] PHP：类型声明与返回类型
来源：http://ui.chemitech.net.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://yv.hnjuh.cn

[U46] PHP：可空类型
来源：http://oy.haigaiapp.cn

?string $name = null
来源：http://nr.bookmarksfly.cn

[U47] PHP：联合类型
来源：http://jq.9csxet.cn

int|string $id
来源：http://wu.wgjwhj.cn

[U48] PHP：纯枚举
来源：http://jo.szsharing.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ls.lnxyls.cn

[U49] PHP：只读属性
来源：http://om.gzmigu.cn

public readonly string $name
来源：http://km.asd995.cn

[U50] PHP：构造器属性提升
来源：http://wl.9csxet.cn

public function __construct(private int $id) {}
来源：http://ig.521024.cn

[U51] PHP：数组解构
来源：http://cm.521024.cn

[$a, $b] = $arr;
来源：http://fi.gzmigu.cn

[U52] PHP：箭头函数
来源：http://ty.chemitech.net.cn

$double = fn($x) => $x * 2;
来源：http://lp.shxzskj.cn

[U53] PHP：空合并运算符
来源：http://fi.asd995.cn

$v = $a ?? $b ?? "default";
来源：http://de.huanxung.cn

[U54] PHP：空安全调用
来源：http://nu.bjjhwx.cn

$obj?->method()
来源：http://gm.bjjhwx.cn

[U55] PHP：match 表达式
来源：http://le.jctech888.com.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ez.521024.cn

[U56] PHP：命名参数
来源：http://wo.521024.cn

f(a: 1, b: 2)
来源：http://ro.gzmigu.cn

[U57] PHP：字符串插值
来源：http://ir.jctech888.com.cn

"值: {$a}"
来源：http://gg.asd995.cn

[U58] PHP：数组三件套
来源：http://st.yuntaijiaju.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rn.szsharing.cn

[U59] PHP：自定义排序
来源：http://cn.panjiajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ol.haigaiapp.cn

[U60] PHP：JSON 编解码
来源：http://bi.muxihuayi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://we.bjjhwx.cn

[U61] PHP：正则
来源：http://xg.jctech888.com.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jp.wgjwhj.cn

[U62] PHP：日期对象
来源：http://ls.muxihuayi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qz.shtwfgs.cn

[U63] PHP：文件读写
来源：http://rq.hahajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ec.hahajie.cn

[U64] PHP：目录遍历
来源：http://zb.colortex.cn

glob("dir/*.php");  scandir("dir");
来源：http://st.jianghongdianzi.cn

[U65] PHP：会话
来源：http://en.huixiangedu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://zs.jianghongdianzi.cn

[U66] PHP：设置 Cookie
来源：http://uz.hahajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pf.jianghongdianzi.cn

[U67] PHP：处理文件上传
来源：http://kr.chemitech.net.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wp.muxihuayi.cn

[U68] PHP：PDO 连接
来源：http://jp.shtwfgs.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gi.panjiajie.cn

[U69] PHP：PDO 预处理
来源：http://uu.szsharing.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ug.wgjwhj.cn

[U70] PHP：PDO 事务
来源：http://ek.shxzukj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pw.bookmarksfly.cn

[U71] PHP：抛出异常
来源：http://gd.gzmigu.cn

throw new RuntimeException("失败", 500);
来源：http://an.newstarts.cn

[U72] PHP：写错误日志
来源：http://sd.shtwfgs.cn

error_log("失败: " . $e->getMessage());
来源：http://ie.szxytkj.cn

[U73] PHP：读取 ini 配置
来源：http://sb.muxihuayi.cn

parse_ini_file("config.ini", true)
来源：http://cf.jctech888.com.cn

[U74] PHP：读取环境变量
来源：http://nv.9csxet.cn

getenv("APP_ENV") ?: "production"
来源：http://qg.nicolike.cn

[U75] PHP：依赖注入
来源：http://jm.hahajie.cn

composer require psr/container
来源：http://mu.hahajie.cn

[U76] PHP：简单路由
来源：http://ig.chemitech.net.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zn.hnjuh.cn

[U77] PHP：模板渲染
来源：http://ls.szxytkj.cn

composer require twig/twig
来源：http://tu.wgjwhj.cn

[U78] PHP：单元测试
来源：http://uu.chemitech.net.cn

composer require --dev phpunit/phpunit
来源：http://sf.hnjuh.cn

[U79] PHP：静态分析
来源：http://mu.9csxet.cn

composer require --dev phpstan/phpstan
来源：http://ju.hahajie.cn

[U80] PHP：代码规范修复
来源：http://fc.yuntaijiaju.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ir.muxihuayi.cn

[U81] JS：初始化项目
来源：http://rp.szxytkj.cn

npm init -y;  npm i express
来源：http://pr.yuexingan06.cn

[U82] JS：package.json 脚本
来源：http://sd.hahajie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gw.hahajie.cn

[U83] JS：ES Module 导入导出
来源：http://qs.gzmigu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://oc.newstarts.cn

[U84] JS：CommonJS 写法
来源：http://ek.szsharing.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ri.panjiajie.cn

[U85] JS：可选链
来源：http://lx.521024.cn

a?.b?.c
来源：http://vx.chemitech.net.cn

[U86] JS：空值合并
来源：http://op.bookmarksfly.cn

a ?? b
来源：http://yp.gzmigu.cn

[U87] JS：解构默认值
来源：http://yg.haigaiapp.cn

const { a = 1, b = 2 } = obj;
来源：http://cz.haigaiapp.cn

[U88] JS：对象展开合并
来源：http://by.gzmigu.cn

{ ...a, ...b }
来源：http://wa.haigaiapp.cn

[U89] JS：数组去重
来源：http://bs.colortex.cn

[...new Set(arr)]
来源：http://rt.huixiangedu.cn

[U90] JS：数字数组排序
来源：http://ax.bookmarksfly.cn

[...arr].sort((a, b) => a - b)
来源：http://mi.panjiajie.cn

[U91] JS：对象键值遍历
来源：http://lr.muxihuayi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ob.huixinmuqiang.cn

[U92] JS：深拷贝
来源：http://qw.szxytkj.cn

structuredClone(obj)
来源：http://ca.panjiajie.cn

[U93] JS：模板字符串
来源：http://wq.haigaiapp.cn

`共 ${n} 条`
来源：http://ce.chemitech.net.cn

[U94] JS：箭头函数
来源：http://od.chemitech.net.cn

const double = x => x * 2;
来源：http://hg.521024.cn

[U95] JS：Promise 包装
来源：http://ie.yuntaijiaju.cn

new Promise((resolve, reject) => {})
来源：http://cu.huixiangedu.cn

[U96] JS：async/await 与异常
来源：http://wi.huixinmuqiang.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ex.wgjwhj.cn


<!-- 参考信息 -->