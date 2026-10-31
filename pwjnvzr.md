代发 wailian999

[T05] Kotlin：when 表达式
来源：http://tr.shxzukj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://eg.huixinmuqiang.cn

[T06] Kotlin：集合映射
来源：http://pd.bjjhwx.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://wg.szxytkj.cn

[T07] Kotlin：集合过滤
来源：http://my.hahajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://nl.shxzskj.cn

[T08] Kotlin：数据类
来源：http://vi.colortex.cn

data class User(val name: String, val age: Int)
来源：http://bj.shxzskj.cn

[T09] Kotlin：扩展函数
来源：http://uj.szxytkj.cn

fun String.exclaim() = this + "!"
来源：http://gs.9csxet.cn

[T10] Kotlin：默认参数
来源：http://an.huixiangedu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://kj.hnjuh.cn

[T11] Kotlin：协程
来源：http://ox.hahajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://lk.newstarts.cn

[T12] Kotlin：解构声明
来源：http://vb.jctech888.com.cn

val (a, b) = Pair(1, 2)
来源：http://xe.jianghongdianzi.cn

[T13] Kotlin：只读 Map
来源：http://yp.jianghongdianzi.cn

val m = mapOf("a" to 1)
来源：http://uo.yuexingan06.cn

[T14] Kotlin：循环
来源：http://yc.nszjky.cn

for (i in 1..10) println(i)
来源：http://lz.colortex.cn

[T15] Kotlin：接口
来源：http://iz.colortex.cn

interface Shape { fun area(): Double }
来源：http://et.shtwfgs.cn

[T16] Swift：Hello World
来源：http://lj.huixinmuqiang.cn

print("Hello")
来源：http://ao.szsharing.cn

[T17] Swift：变量与常量
来源：http://wa.jctech888.com.cn

var a = 1;  let b = 2
来源：http://vr.shxzukj.cn

[T18] Swift：字符串插值
来源：http://of.huixinmuqiang.cn

"值: \(b)"
来源：http://xf.jianghongdianzi.cn

[T19] Swift：可选绑定
来源：http://kg.huixiangedu.cn

if let n = opt { print(n) }
来源：http://gz.hnjuh.cn

[T20] Swift：数组操作
来源：http://hp.haigaiapp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://pm.shxzukj.cn

[T21] Swift：遍历
来源：http://cp.wgjwhj.cn

for x in a { print(x) }
来源：http://vd.shxzukj.cn

[T22] Swift：字典
来源：http://qr.hahajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ao.colortex.cn

[T23] Swift：函数
来源：http://zc.shxzskj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tl.yuntaijiaju.cn

[T24] Swift：闭包
来源：http://hz.lnxyls.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://lw.muxihuayi.cn

[T25] Swift：结构体
来源：http://tz.haigaiapp.cn

struct P { var x: Int }
来源：http://eo.yuexingan06.cn

[T26] Swift：类与重写
来源：http://ji.bjjhwx.cn

class A: Base { override func f() {} }
来源：http://xf.huanxung.cn

[T27] Swift：错误处理
来源：http://lt.jianghongdianzi.cn

do { try f() } catch { print(error) }
来源：http://qk.nicolike.cn

[T28] Swift：枚举
来源：http://af.521024.cn

enum Color { case red, green }
来源：http://ou.szxytkj.cn

[T29] Swift：guard 提前返回
来源：http://lk.jctech888.com.cn

guard let x = opt else { return }
来源：http://yi.shxzukj.cn

[T30] Swift：协议
来源：http://fu.shxzskj.cn

protocol Shape { func area() -> Double }
来源：http://gp.colortex.cn

[T31] Lua：Hello World
来源：http://uw.huixiangedu.cn

print("Hello")
来源：http://se.521024.cn

[T32] Lua：局部变量
来源：http://sp.huixinmuqiang.cn

local a = 1
来源：http://np.asd995.cn

[T33] Lua：表（数组）
来源：http://zx.haigaiapp.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ky.nszjky.cn

[T34] Lua：遍历表
来源：http://hm.lnxyls.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ad.shxzskj.cn

[T35] Lua：字典表
来源：http://gc.bjjhwx.cn

local d = { a = 1 };  d.b = 2
来源：http://wt.haigaiapp.cn

[T36] Lua：函数
来源：http://ln.muxihuayi.cn

function add(a, b) return a + b end
来源：http://wf.shxzukj.cn

[T37] Lua：字符串拼接
来源：http://oo.bookmarksfly.cn

"a" .. "b"
来源：http://aq.asd995.cn

[T38] Lua：条件
来源：http://oy.yuexingan06.cn

if x > 0 then print("正") end
来源：http://gv.521024.cn

[T39] Lua：模式匹配
来源：http://ng.nicolike.cn

string.find(s, "%d+")
来源：http://ho.jctech888.com.cn

[T40] Lua：元表
来源：http://iq.muxihuayi.cn

setmetatable({}, { __index = base })
来源：http://pb.huixinmuqiang.cn

[T41] Perl：Hello World
来源：http://az.huixiangedu.cn

print "Hello\n";
来源：http://zn.nicolike.cn

[T42] Perl：变量类型
来源：http://uw.chemitech.net.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zt.shtwfgs.cn

[T43] Perl：字符串插值
来源：http://rc.panjiajie.cn

"值: $a"
来源：http://sy.huixiangedu.cn

[T44] Perl：条件
来源：http://gd.wgjwhj.cn

if ($a > 0) { print "正"; }
来源：http://tt.huanxung.cn

[T45] Perl：数组遍历
来源：http://we.wgjwhj.cn

for my $x (@arr) { print $x; }
来源：http://no.newstarts.cn

[T46] Perl：哈希操作
来源：http://sd.bookmarksfly.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gi.nszjky.cn

[T47] Perl：正则捕获
来源：http://ty.shtwfgs.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ls.nicolike.cn

[T48] Perl：正则替换
来源：http://pt.jianghongdianzi.cn

$s =~ s/old/new/g;
来源：http://wk.9csxet.cn

[T49] Perl：函数
来源：http://cs.chemitech.net.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nf.lnxyls.cn

[T50] Perl：逐行读文件
来源：http://cu.szxytkj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://md.jctech888.com.cn

while (my $line = <$fh>) { print $line; }
来源：http://li.521024.cn

[T51] Scala：Hello World
来源：http://oj.haigaiapp.cn

println("Hello")
来源：http://ul.haigaiapp.cn

[T52] Scala：变量
来源：http://qc.bjjhwx.cn

val a = 1;  var b = 2
来源：http://fm.chemitech.net.cn

[T53] Scala：字符串插值
来源：http://wq.9csxet.cn

s"值: $b"
来源：http://kf.szxytkj.cn

[T54] Scala：集合映射
来源：http://tw.nszjky.cn

List(1, 2, 3).map(_ * 2)
来源：http://xn.nicolike.cn

[T55] Scala：集合过滤
来源：http://vn.yuntaijiaju.cn

List(1, 2, 3).filter(_ > 1)
来源：http://up.shtwfgs.cn

[T56] Scala：样例类
来源：http://yz.jianghongdianzi.cn

case class User(name: String, age: Int)
来源：http://jh.wgjwhj.cn

[T57] Scala：模式匹配
来源：http://oc.shxzukj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://nw.nicolike.cn

[T58] Scala：函数定义
来源：http://tu.9csxet.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ct.huixiangedu.cn

[T59] Scala：循环
来源：http://nk.nicolike.cn

for (i <- 1 to 10) println(i)
来源：http://nt.lnxyls.cn

[T60] Scala：折叠
来源：http://uo.jctech888.com.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wa.nszjky.cn

================================================================================
来源：http://qc.521024.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dv.panjiajie.cn

================================================================================
来源：http://qz.newstarts.cn

[U01] Py：创建虚拟环境
来源：http://rr.wgjwhj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://my.szsharing.cn

[U02] Py：导出 / 安装依赖
来源：http://qk.bookmarksfly.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://id.jianghongdianzi.cn

[U03] Py：加载 .env 配置
来源：http://ok.bjjhwx.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ot.hahajie.cn

[U04] Py：变量调试打印
来源：http://fm.haigaiapp.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ry.lnxyls.cn

[U05] Py：列表去重且保序
来源：http://el.yuntaijiaju.cn

list(dict.fromkeys(arr))
来源：http://df.szsharing.cn

[U06] Py：合并两个字典
来源：http://il.yuntaijiaju.cn

{**a, **b}
来源：http://sg.colortex.cn

[U07] Py：反转字典键值
来源：http://fc.521024.cn

{v: k for k, v in d.items()}
来源：http://dt.9csxet.cn

[U08] Py：展平二维列表
来源：http://dp.yuntaijiaju.cn

[y for x in nested for y in x]
来源：http://yq.gzmigu.cn

[U09] Py：字典取最大值的键
来源：http://bw.lnxyls.cn

max(d, key=d.get)
来源：http://bq.haigaiapp.cn

[U10] Py：按值排序字典
来源：http://zj.gzmigu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wm.hnjuh.cn

[U11] Py：生成器表达式
来源：http://si.9csxet.cn

(x * 2 for x in arr)
来源：http://to.shxzskj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://pc.yuexingan06.cn

Counter(arr).most_common(3)
来源：http://di.9csxet.cn

[U13] Py：固定长度队列
来源：http://gd.haigaiapp.cn

deque(maxlen=10)
来源：http://fs.huixiangedu.cn

[U14] Py：分组收集到列表
来源：http://go.nicolike.cn

defaultdict(list)
来源：http://gi.bjjhwx.cn

[U15] Py：高精度计时
来源：http://ct.nicolike.cn

t = time.perf_counter()
来源：http://mb.shtwfgs.cn

[U16] Py：命令行参数解析
来源：http://gd.huanxung.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gl.jianghongdianzi.cn

[U17] Py：初始化日志
来源：http://so.szsharing.cn

logging.basicConfig(level=logging.INFO)
来源：http://sg.yuntaijiaju.cn

[U18] Py：预编译正则
来源：http://ab.colortex.cn

pat = re.compile(r"\d+")
来源：http://jp.521024.cn

[U19] Py：正则替换带回调
来源：http://pp.huixiangedu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://eb.shxzukj.cn

[U20] Py：缓存函数结果
来源：http://yq.jctech888.com.cn

@functools.lru_cache(maxsize=None)
来源：http://cl.nszjky.cn

[U21] Py：自定义上下文管理器
来源：http://ar.huanxung.cn

@contextlib.contextmanager
来源：http://eq.huixiangedu.cn

[U22] Py：矩阵转置
来源：http://ic.521024.cn

list(zip(*m))
来源：http://gd.szxytkj.cn

[U23] Py：分块读取大文件
来源：http://gq.9csxet.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ua.huixiangedu.cn

[U24] Py：路径操作
来源：http://ky.gzmigu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xy.newstarts.cn

[U25] Py：CSV 按字典读
来源：http://vb.lnxyls.cn

csv.DictReader(f)
来源：http://cg.szxytkj.cn

[U26] Py：并发下载
来源：http://bg.szxytkj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lg.panjiajie.cn

[U27] Py：异步 HTTP
来源：http://rk.yuexingan06.cn

aiohttp.ClientSession() 配合 async with
来源：http://us.nszjky.cn

[U28] Py：类型别名
来源：http://tr.jianghongdianzi.cn

UserId = int
来源：http://ty.hnjuh.cn

[U29] Py：属性校验
来源：http://nw.huixiangedu.cn

@property 与 @x.setter 配合
来源：http://ju.colortex.cn

[U30] Py：数据类
来源：http://gc.lnxyls.cn

@dataclass(slots=True)
来源：http://sx.yuexingan06.cn

[U31] Py：单测
来源：http://lv.jctech888.com.cn

python -m pytest -q
来源：http://yl.huixiangedu.cn

[U32] Py：代码格式化
来源：http://ht.nszjky.cn

ruff format . && ruff check --fix .
来源：http://ok.yuntaijiaju.cn

[U33] Py：打包发布
来源：http://pj.colortex.cn

python -m build  （依赖 pyproject.toml）
来源：http://xm.chemitech.net.cn

[U34] Py：判断编码
来源：http://jk.newstarts.cn

chardet.detect(raw)
来源：http://wq.shxzskj.cn

[U35] Py：发送邮件
来源：http://ec.chemitech.net.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tq.hahajie.cn

[U36] Py：定时任务
来源：http://xo.szsharing.cn

schedule.every(10).minutes.do(job)
来源：http://xe.hnjuh.cn

[U37] Py：读写 Excel
来源：http://ue.hnjuh.cn

pandas.read_excel / DataFrame.to_excel
来源：http://em.szsharing.cn

[U38] Py：获取脚本所在目录
来源：http://ie.chemitech.net.cn

Path(__file__).resolve().parent
来源：http://no.muxihuayi.cn

[U39] Py：判断是否在交互环境
来源：http://hq.szsharing.cn

sys.stdout.isatty()
来源：http://io.9csxet.cn

[U40] Py：打印到标准错误
来源：http://ue.shxzukj.cn

print("err", file=sys.stderr)
来源：http://sn.colortex.cn

[U41] PHP：初始化 Composer 项目
来源：http://rx.asd995.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ze.muxihuayi.cn

[U42] PHP：PSR-4 自动加载
来源：http://cp.muxihuayi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://uf.bjjhwx.cn

[U43] PHP：声明命名空间
来源：http://ps.newstarts.cn

namespace App\Http;
来源：http://bb.9csxet.cn

[U44] PHP：开启严格类型
来源：http://tl.wgjwhj.cn

declare(strict_types=1);
来源：http://ey.gzmigu.cn

[U45] PHP：类型声明与返回类型
来源：http://lq.yuntaijiaju.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://tg.colortex.cn

[U46] PHP：可空类型
来源：http://xz.jctech888.com.cn

?string $name = null
来源：http://hk.shxzskj.cn

[U47] PHP：联合类型
来源：http://hi.chemitech.net.cn

int|string $id
来源：http://lw.shtwfgs.cn

[U48] PHP：纯枚举
来源：http://nt.hahajie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ft.huanxung.cn

[U49] PHP：只读属性
来源：http://by.asd995.cn

public readonly string $name
来源：http://oq.jctech888.com.cn

[U50] PHP：构造器属性提升
来源：http://se.lnxyls.cn

public function __construct(private int $id) {}
来源：http://cq.szsharing.cn

[U51] PHP：数组解构
来源：http://go.gzmigu.cn

[$a, $b] = $arr;
来源：http://cn.panjiajie.cn

[U52] PHP：箭头函数
来源：http://az.asd995.cn

$double = fn($x) => $x * 2;
来源：http://py.gzmigu.cn

[U53] PHP：空合并运算符
来源：http://mh.chemitech.net.cn

$v = $a ?? $b ?? "default";
来源：http://gn.jctech888.com.cn

[U54] PHP：空安全调用
来源：http://mg.lnxyls.cn

$obj?->method()
来源：http://rf.chemitech.net.cn

[U55] PHP：match 表达式
来源：http://fy.szxytkj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hj.panjiajie.cn

[U56] PHP：命名参数
来源：http://kd.asd995.cn

f(a: 1, b: 2)
来源：http://ky.asd995.cn

[U57] PHP：字符串插值
来源：http://lw.jctech888.com.cn

"值: {$a}"
来源：http://ai.panjiajie.cn

[U58] PHP：数组三件套
来源：http://cz.jctech888.com.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://aq.yuexingan06.cn

[U59] PHP：自定义排序
来源：http://yw.jctech888.com.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://en.9csxet.cn

[U60] PHP：JSON 编解码
来源：http://kp.hahajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fy.huixinmuqiang.cn

[U61] PHP：正则
来源：http://bz.szxytkj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yc.hahajie.cn

[U62] PHP：日期对象
来源：http://wj.huixinmuqiang.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vb.haigaiapp.cn

[U63] PHP：文件读写
来源：http://br.huanxung.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nn.panjiajie.cn

[U64] PHP：目录遍历
来源：http://xp.yuexingan06.cn

glob("dir/*.php");  scandir("dir");
来源：http://nu.asd995.cn

[U65] PHP：会话
来源：http://is.jctech888.com.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://tl.9csxet.cn

[U66] PHP：设置 Cookie
来源：http://gh.521024.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ij.shxzukj.cn

[U67] PHP：处理文件上传
来源：http://kr.yuntaijiaju.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://es.yuntaijiaju.cn

[U68] PHP：PDO 连接
来源：http://vh.newstarts.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ad.wgjwhj.cn

[U69] PHP：PDO 预处理
来源：http://yn.shtwfgs.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bm.huixinmuqiang.cn

[U70] PHP：PDO 事务
来源：http://tz.bookmarksfly.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sf.shtwfgs.cn

[U71] PHP：抛出异常
来源：http://ta.muxihuayi.cn

throw new RuntimeException("失败", 500);
来源：http://ys.nszjky.cn

[U72] PHP：写错误日志
来源：http://iv.chemitech.net.cn

error_log("失败: " . $e->getMessage());
来源：http://gh.bjjhwx.cn

[U73] PHP：读取 ini 配置
来源：http://tn.nszjky.cn

parse_ini_file("config.ini", true)
来源：http://fn.hahajie.cn

[U74] PHP：读取环境变量
来源：http://td.panjiajie.cn

getenv("APP_ENV") ?: "production"
来源：http://nq.asd995.cn

[U75] PHP：依赖注入
来源：http://bl.gzmigu.cn

composer require psr/container
来源：http://nb.shxzukj.cn

[U76] PHP：简单路由
来源：http://dn.shxzskj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rn.nicolike.cn

[U77] PHP：模板渲染
来源：http://ks.yuntaijiaju.cn

composer require twig/twig
来源：http://tg.szxytkj.cn

[U78] PHP：单元测试
来源：http://rt.nicolike.cn

composer require --dev phpunit/phpunit
来源：http://oj.szxytkj.cn

[U79] PHP：静态分析
来源：http://ee.huanxung.cn

composer require --dev phpstan/phpstan
来源：http://qt.haigaiapp.cn

[U80] PHP：代码规范修复
来源：http://nj.asd995.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://mb.shxzukj.cn

[U81] JS：初始化项目
来源：http://wg.521024.cn

npm init -y;  npm i express
来源：http://eu.nicolike.cn

[U82] JS：package.json 脚本
来源：http://ok.lnxyls.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rq.huixiangedu.cn

[U83] JS：ES Module 导入导出
来源：http://jp.szsharing.cn

export const a = 1;  import { a } from "./m.js";
来源：http://dn.yuexingan06.cn

[U84] JS：CommonJS 写法
来源：http://gt.yuexingan06.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ux.nicolike.cn

[U85] JS：可选链
来源：http://ep.bjjhwx.cn

a?.b?.c
来源：http://cb.newstarts.cn

[U86] JS：空值合并
来源：http://hi.asd995.cn

a ?? b
来源：http://lo.gzmigu.cn

[U87] JS：解构默认值
来源：http://an.hnjuh.cn

const { a = 1, b = 2 } = obj;
来源：http://eb.huixiangedu.cn

[U88] JS：对象展开合并
来源：http://be.hahajie.cn

{ ...a, ...b }
来源：http://ix.lnxyls.cn

[U89] JS：数组去重
来源：http://da.521024.cn

[...new Set(arr)]
来源：http://ek.jianghongdianzi.cn

[U90] JS：数字数组排序
来源：http://ex.nszjky.cn

[...arr].sort((a, b) => a - b)
来源：http://ey.nszjky.cn

[U91] JS：对象键值遍历
来源：http://sb.asd995.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://eu.hnjuh.cn

[U92] JS：深拷贝
来源：http://hm.shtwfgs.cn

structuredClone(obj)
来源：http://wx.huixiangedu.cn


<!-- 参考信息 -->