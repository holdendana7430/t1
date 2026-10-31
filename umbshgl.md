代发 wailian999

[T05] Kotlin：when 表达式
来源：http://zx.szxytkj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zc.muxihuayi.cn

[T06] Kotlin：集合映射
来源：http://zo.szsharing.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://cw.huixiangedu.cn

[T07] Kotlin：集合过滤
来源：http://qe.521024.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lr.chemitech.net.cn

[T08] Kotlin：数据类
来源：http://yh.colortex.cn

data class User(val name: String, val age: Int)
来源：http://nx.jctech888.com.cn

[T09] Kotlin：扩展函数
来源：http://km.muxihuayi.cn

fun String.exclaim() = this + "!"
来源：http://ao.gzmigu.cn

[T10] Kotlin：默认参数
来源：http://cc.panjiajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pd.huixinmuqiang.cn

[T11] Kotlin：协程
来源：http://iu.shxzukj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://zf.szxytkj.cn

[T12] Kotlin：解构声明
来源：http://vg.jianghongdianzi.cn

val (a, b) = Pair(1, 2)
来源：http://ex.hahajie.cn

[T13] Kotlin：只读 Map
来源：http://ke.colortex.cn

val m = mapOf("a" to 1)
来源：http://as.colortex.cn

[T14] Kotlin：循环
来源：http://dr.jctech888.com.cn

for (i in 1..10) println(i)
来源：http://kx.nszjky.cn

[T15] Kotlin：接口
来源：http://he.9csxet.cn

interface Shape { fun area(): Double }
来源：http://kw.colortex.cn

[T16] Swift：Hello World
来源：http://fp.wgjwhj.cn

print("Hello")
来源：http://ol.asd995.cn

[T17] Swift：变量与常量
来源：http://cs.hahajie.cn

var a = 1;  let b = 2
来源：http://zz.szsharing.cn

[T18] Swift：字符串插值
来源：http://dq.nszjky.cn

"值: \(b)"
来源：http://sn.haigaiapp.cn

[T19] Swift：可选绑定
来源：http://ay.shxzukj.cn

if let n = opt { print(n) }
来源：http://ww.jctech888.com.cn

[T20] Swift：数组操作
来源：http://gl.nszjky.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ro.nszjky.cn

[T21] Swift：遍历
来源：http://tb.panjiajie.cn

for x in a { print(x) }
来源：http://dh.jctech888.com.cn

[T22] Swift：字典
来源：http://mq.huixiangedu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zn.panjiajie.cn

[T23] Swift：函数
来源：http://hh.yuexingan06.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://af.shxzskj.cn

[T24] Swift：闭包
来源：http://kg.hnjuh.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://pg.521024.cn

[T25] Swift：结构体
来源：http://bv.521024.cn

struct P { var x: Int }
来源：http://rs.hnjuh.cn

[T26] Swift：类与重写
来源：http://wa.yuntaijiaju.cn

class A: Base { override func f() {} }
来源：http://bk.chemitech.net.cn

[T27] Swift：错误处理
来源：http://rv.yuntaijiaju.cn

do { try f() } catch { print(error) }
来源：http://mn.huixinmuqiang.cn

[T28] Swift：枚举
来源：http://rs.nicolike.cn

enum Color { case red, green }
来源：http://zt.nszjky.cn

[T29] Swift：guard 提前返回
来源：http://sg.panjiajie.cn

guard let x = opt else { return }
来源：http://xs.muxihuayi.cn

[T30] Swift：协议
来源：http://gb.colortex.cn

protocol Shape { func area() -> Double }
来源：http://wd.muxihuayi.cn

[T31] Lua：Hello World
来源：http://wq.asd995.cn

print("Hello")
来源：http://iy.yuexingan06.cn

[T32] Lua：局部变量
来源：http://pq.nszjky.cn

local a = 1
来源：http://rf.nszjky.cn

[T33] Lua：表（数组）
来源：http://xx.huixinmuqiang.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://yw.szsharing.cn

[T34] Lua：遍历表
来源：http://rj.bookmarksfly.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://fi.nszjky.cn

[T35] Lua：字典表
来源：http://th.huanxung.cn

local d = { a = 1 };  d.b = 2
来源：http://cn.shxzukj.cn

[T36] Lua：函数
来源：http://ku.asd995.cn

function add(a, b) return a + b end
来源：http://km.shtwfgs.cn

[T37] Lua：字符串拼接
来源：http://sm.chemitech.net.cn

"a" .. "b"
来源：http://vr.yuntaijiaju.cn

[T38] Lua：条件
来源：http://pp.panjiajie.cn

if x > 0 then print("正") end
来源：http://ez.jctech888.com.cn

[T39] Lua：模式匹配
来源：http://pi.521024.cn

string.find(s, "%d+")
来源：http://zw.nszjky.cn

[T40] Lua：元表
来源：http://xw.huixiangedu.cn

setmetatable({}, { __index = base })
来源：http://ge.bjjhwx.cn

[T41] Perl：Hello World
来源：http://ts.bookmarksfly.cn

print "Hello\n";
来源：http://te.gzmigu.cn

[T42] Perl：变量类型
来源：http://lv.shtwfgs.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ml.asd995.cn

[T43] Perl：字符串插值
来源：http://gr.shtwfgs.cn

"值: $a"
来源：http://wj.szxytkj.cn

[T44] Perl：条件
来源：http://pc.yuntaijiaju.cn

if ($a > 0) { print "正"; }
来源：http://uk.gzmigu.cn

[T45] Perl：数组遍历
来源：http://kd.panjiajie.cn

for my $x (@arr) { print $x; }
来源：http://jl.jianghongdianzi.cn

[T46] Perl：哈希操作
来源：http://ce.9csxet.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sh.yuexingan06.cn

[T47] Perl：正则捕获
来源：http://vq.9csxet.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://tr.panjiajie.cn

[T48] Perl：正则替换
来源：http://hr.wgjwhj.cn

$s =~ s/old/new/g;
来源：http://jv.newstarts.cn

[T49] Perl：函数
来源：http://fb.shxzukj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qe.huanxung.cn

[T50] Perl：逐行读文件
来源：http://vu.yuntaijiaju.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://uf.lnxyls.cn

while (my $line = <$fh>) { print $line; }
来源：http://ow.bookmarksfly.cn

[T51] Scala：Hello World
来源：http://dc.bookmarksfly.cn

println("Hello")
来源：http://av.huanxung.cn

[T52] Scala：变量
来源：http://ag.hnjuh.cn

val a = 1;  var b = 2
来源：http://dy.bjjhwx.cn

[T53] Scala：字符串插值
来源：http://jy.521024.cn

s"值: $b"
来源：http://gz.panjiajie.cn

[T54] Scala：集合映射
来源：http://ac.wgjwhj.cn

List(1, 2, 3).map(_ * 2)
来源：http://ir.9csxet.cn

[T55] Scala：集合过滤
来源：http://rx.lnxyls.cn

List(1, 2, 3).filter(_ > 1)
来源：http://cj.yuexingan06.cn

[T56] Scala：样例类
来源：http://mq.panjiajie.cn

case class User(name: String, age: Int)
来源：http://cp.haigaiapp.cn

[T57] Scala：模式匹配
来源：http://hf.lnxyls.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vy.newstarts.cn

[T58] Scala：函数定义
来源：http://sn.wgjwhj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://nl.huixiangedu.cn

[T59] Scala：循环
来源：http://ag.shxzukj.cn

for (i <- 1 to 10) println(i)
来源：http://sy.shxzukj.cn

[T60] Scala：折叠
来源：http://cv.gzmigu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mr.521024.cn

================================================================================
来源：http://yg.yuntaijiaju.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cd.jianghongdianzi.cn

================================================================================
来源：http://sb.huanxung.cn

[U01] Py：创建虚拟环境
来源：http://ti.shtwfgs.cn

python -m venv .venv && source .venv/bin/activate
来源：http://sn.shtwfgs.cn

[U02] Py：导出 / 安装依赖
来源：http://ki.yuntaijiaju.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ed.shtwfgs.cn

[U03] Py：加载 .env 配置
来源：http://hy.colortex.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://dr.panjiajie.cn

[U04] Py：变量调试打印
来源：http://tw.huixiangedu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cb.jianghongdianzi.cn

[U05] Py：列表去重且保序
来源：http://rp.shxzukj.cn

list(dict.fromkeys(arr))
来源：http://xi.hnjuh.cn

[U06] Py：合并两个字典
来源：http://oh.hnjuh.cn

{**a, **b}
来源：http://gz.nicolike.cn

[U07] Py：反转字典键值
来源：http://bw.hahajie.cn

{v: k for k, v in d.items()}
来源：http://sk.jianghongdianzi.cn

[U08] Py：展平二维列表
来源：http://dy.9csxet.cn

[y for x in nested for y in x]
来源：http://di.shtwfgs.cn

[U09] Py：字典取最大值的键
来源：http://ay.chemitech.net.cn

max(d, key=d.get)
来源：http://xl.panjiajie.cn

[U10] Py：按值排序字典
来源：http://dl.shxzukj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jh.szsharing.cn

[U11] Py：生成器表达式
来源：http://op.colortex.cn

(x * 2 for x in arr)
来源：http://pa.nszjky.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ud.shxzukj.cn

Counter(arr).most_common(3)
来源：http://kg.panjiajie.cn

[U13] Py：固定长度队列
来源：http://cx.nszjky.cn

deque(maxlen=10)
来源：http://lv.bjjhwx.cn

[U14] Py：分组收集到列表
来源：http://oy.panjiajie.cn

defaultdict(list)
来源：http://ea.jianghongdianzi.cn

[U15] Py：高精度计时
来源：http://rc.bjjhwx.cn

t = time.perf_counter()
来源：http://fq.haigaiapp.cn

[U16] Py：命令行参数解析
来源：http://wh.jctech888.com.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fk.jctech888.com.cn

[U17] Py：初始化日志
来源：http://of.panjiajie.cn

logging.basicConfig(level=logging.INFO)
来源：http://vd.panjiajie.cn

[U18] Py：预编译正则
来源：http://ro.jianghongdianzi.cn

pat = re.compile(r"\d+")
来源：http://zm.jianghongdianzi.cn

[U19] Py：正则替换带回调
来源：http://vq.newstarts.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jk.nszjky.cn

[U20] Py：缓存函数结果
来源：http://lw.haigaiapp.cn

@functools.lru_cache(maxsize=None)
来源：http://bv.huanxung.cn

[U21] Py：自定义上下文管理器
来源：http://ch.nicolike.cn

@contextlib.contextmanager
来源：http://ju.huixinmuqiang.cn

[U22] Py：矩阵转置
来源：http://bf.hnjuh.cn

list(zip(*m))
来源：http://ez.bjjhwx.cn

[U23] Py：分块读取大文件
来源：http://tb.gzmigu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bn.hahajie.cn

[U24] Py：路径操作
来源：http://vo.szxytkj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nm.gzmigu.cn

[U25] Py：CSV 按字典读
来源：http://uh.szsharing.cn

csv.DictReader(f)
来源：http://aa.wgjwhj.cn

[U26] Py：并发下载
来源：http://zb.huixinmuqiang.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bh.jianghongdianzi.cn

[U27] Py：异步 HTTP
来源：http://rj.yuntaijiaju.cn

aiohttp.ClientSession() 配合 async with
来源：http://uq.yuntaijiaju.cn

[U28] Py：类型别名
来源：http://tl.shxzukj.cn

UserId = int
来源：http://xg.colortex.cn

[U29] Py：属性校验
来源：http://wk.jianghongdianzi.cn

@property 与 @x.setter 配合
来源：http://tk.nicolike.cn

[U30] Py：数据类
来源：http://sc.szsharing.cn

@dataclass(slots=True)
来源：http://kz.chemitech.net.cn

[U31] Py：单测
来源：http://ek.asd995.cn

python -m pytest -q
来源：http://kf.jctech888.com.cn

[U32] Py：代码格式化
来源：http://va.colortex.cn

ruff format . && ruff check --fix .
来源：http://na.huanxung.cn

[U33] Py：打包发布
来源：http://cw.yuexingan06.cn

python -m build  （依赖 pyproject.toml）
来源：http://dd.9csxet.cn

[U34] Py：判断编码
来源：http://lk.shtwfgs.cn

chardet.detect(raw)
来源：http://ai.chemitech.net.cn

[U35] Py：发送邮件
来源：http://pn.hahajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tc.bjjhwx.cn

[U36] Py：定时任务
来源：http://az.jianghongdianzi.cn

schedule.every(10).minutes.do(job)
来源：http://ke.wgjwhj.cn

[U37] Py：读写 Excel
来源：http://vr.yuntaijiaju.cn

pandas.read_excel / DataFrame.to_excel
来源：http://sf.jctech888.com.cn

[U38] Py：获取脚本所在目录
来源：http://sd.gzmigu.cn

Path(__file__).resolve().parent
来源：http://qo.hahajie.cn

[U39] Py：判断是否在交互环境
来源：http://qr.muxihuayi.cn

sys.stdout.isatty()
来源：http://ie.9csxet.cn

[U40] Py：打印到标准错误
来源：http://oa.wgjwhj.cn

print("err", file=sys.stderr)
来源：http://ua.gzmigu.cn

[U41] PHP：初始化 Composer 项目
来源：http://sy.yuntaijiaju.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://wr.yuexingan06.cn

[U42] PHP：PSR-4 自动加载
来源：http://os.yuexingan06.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vy.huixinmuqiang.cn

[U43] PHP：声明命名空间
来源：http://ov.521024.cn

namespace App\Http;
来源：http://ov.bjjhwx.cn

[U44] PHP：开启严格类型
来源：http://nh.huixinmuqiang.cn

declare(strict_types=1);
来源：http://wm.hahajie.cn

[U45] PHP：类型声明与返回类型
来源：http://wm.huanxung.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://vt.huixinmuqiang.cn

[U46] PHP：可空类型
来源：http://mh.huixinmuqiang.cn

?string $name = null
来源：http://mi.jctech888.com.cn

[U47] PHP：联合类型
来源：http://rl.huixiangedu.cn

int|string $id
来源：http://go.hnjuh.cn

[U48] PHP：纯枚举
来源：http://jh.wgjwhj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qc.jctech888.com.cn

[U49] PHP：只读属性
来源：http://fx.lnxyls.cn

public readonly string $name
来源：http://ck.colortex.cn

[U50] PHP：构造器属性提升
来源：http://bk.521024.cn

public function __construct(private int $id) {}
来源：http://aa.bookmarksfly.cn

[U51] PHP：数组解构
来源：http://xc.shtwfgs.cn

[$a, $b] = $arr;
来源：http://jv.521024.cn

[U52] PHP：箭头函数
来源：http://hl.newstarts.cn

$double = fn($x) => $x * 2;
来源：http://ah.szxytkj.cn

[U53] PHP：空合并运算符
来源：http://wf.haigaiapp.cn

$v = $a ?? $b ?? "default";
来源：http://vg.panjiajie.cn

[U54] PHP：空安全调用
来源：http://ts.chemitech.net.cn

$obj?->method()
来源：http://yg.muxihuayi.cn

[U55] PHP：match 表达式
来源：http://gk.szsharing.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ub.shtwfgs.cn

[U56] PHP：命名参数
来源：http://po.asd995.cn

f(a: 1, b: 2)
来源：http://lj.bjjhwx.cn

[U57] PHP：字符串插值
来源：http://rv.chemitech.net.cn

"值: {$a}"
来源：http://xm.yuntaijiaju.cn

[U58] PHP：数组三件套
来源：http://jk.asd995.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ol.newstarts.cn

[U59] PHP：自定义排序
来源：http://kq.newstarts.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ys.lnxyls.cn

[U60] PHP：JSON 编解码
来源：http://of.bjjhwx.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://uz.newstarts.cn

[U61] PHP：正则
来源：http://mn.yuexingan06.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bn.bookmarksfly.cn

[U62] PHP：日期对象
来源：http://ew.hnjuh.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yo.asd995.cn

[U63] PHP：文件读写
来源：http://ox.9csxet.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vq.jctech888.com.cn

[U64] PHP：目录遍历
来源：http://ur.shxzukj.cn

glob("dir/*.php");  scandir("dir");
来源：http://sf.shxzukj.cn

[U65] PHP：会话
来源：http://or.yuexingan06.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://cq.shxzukj.cn

[U66] PHP：设置 Cookie
来源：http://ca.colortex.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vd.shtwfgs.cn

[U67] PHP：处理文件上传
来源：http://qx.panjiajie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hd.wgjwhj.cn

[U68] PHP：PDO 连接
来源：http://ca.colortex.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ao.newstarts.cn

[U69] PHP：PDO 预处理
来源：http://dd.nicolike.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dt.9csxet.cn

[U70] PHP：PDO 事务
来源：http://uy.yuntaijiaju.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bv.colortex.cn

[U71] PHP：抛出异常
来源：http://iq.wgjwhj.cn

throw new RuntimeException("失败", 500);
来源：http://ah.9csxet.cn

[U72] PHP：写错误日志
来源：http://bl.nszjky.cn

error_log("失败: " . $e->getMessage());
来源：http://cc.huanxung.cn

[U73] PHP：读取 ini 配置
来源：http://ph.shtwfgs.cn

parse_ini_file("config.ini", true)
来源：http://ld.szxytkj.cn

[U74] PHP：读取环境变量
来源：http://jo.gzmigu.cn

getenv("APP_ENV") ?: "production"
来源：http://dz.nszjky.cn

[U75] PHP：依赖注入
来源：http://eg.gzmigu.cn

composer require psr/container
来源：http://lt.nicolike.cn

[U76] PHP：简单路由
来源：http://no.hahajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lc.huanxung.cn

[U77] PHP：模板渲染
来源：http://md.521024.cn

composer require twig/twig
来源：http://gp.hnjuh.cn

[U78] PHP：单元测试
来源：http://qz.hahajie.cn

composer require --dev phpunit/phpunit
来源：http://nf.nicolike.cn

[U79] PHP：静态分析
来源：http://xk.hnjuh.cn

composer require --dev phpstan/phpstan
来源：http://gx.yuntaijiaju.cn

[U80] PHP：代码规范修复
来源：http://fc.newstarts.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://op.colortex.cn

[U81] JS：初始化项目
来源：http://ln.muxihuayi.cn

npm init -y;  npm i express
来源：http://on.nicolike.cn

[U82] JS：package.json 脚本
来源：http://um.9csxet.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ng.wgjwhj.cn

[U83] JS：ES Module 导入导出
来源：http://xa.gzmigu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://sx.huixinmuqiang.cn

[U84] JS：CommonJS 写法
来源：http://nt.bookmarksfly.cn

module.exports = { a };  const { a } = require("./m");
来源：http://kf.huanxung.cn

[U85] JS：可选链
来源：http://tg.asd995.cn

a?.b?.c
来源：http://db.colortex.cn

[U86] JS：空值合并
来源：http://qd.gzmigu.cn

a ?? b
来源：http://ws.nszjky.cn

[U87] JS：解构默认值
来源：http://oq.hahajie.cn

const { a = 1, b = 2 } = obj;
来源：http://fr.jctech888.com.cn

[U88] JS：对象展开合并
来源：http://cs.huixinmuqiang.cn

{ ...a, ...b }
来源：http://gs.521024.cn

[U89] JS：数组去重
来源：http://dj.yuntaijiaju.cn

[...new Set(arr)]
来源：http://jw.yuexingan06.cn

[U90] JS：数字数组排序
来源：http://kn.szsharing.cn

[...arr].sort((a, b) => a - b)
来源：http://wl.huanxung.cn

[U91] JS：对象键值遍历
来源：http://af.yuexingan06.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vt.shxzukj.cn

[U92] JS：深拷贝
来源：http://rw.yuexingan06.cn

structuredClone(obj)
来源：http://ru.nszjky.cn


<!-- 参考信息 -->