代发 wailian999

[T07] Kotlin：集合过滤
来源：http://qk.bjjhwx.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ul.szxytkj.cn

[T08] Kotlin：数据类
来源：http://zl.haigaiapp.cn

data class User(val name: String, val age: Int)
来源：http://av.muxihuayi.cn

[T09] Kotlin：扩展函数
来源：http://ah.hnjuh.cn

fun String.exclaim() = this + "!"
来源：http://va.nszjky.cn

[T10] Kotlin：默认参数
来源：http://df.521024.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ha.yuntaijiaju.cn

[T11] Kotlin：协程
来源：http://dy.jianghongdianzi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://yu.jctech888.com.cn

[T12] Kotlin：解构声明
来源：http://wq.shxzskj.cn

val (a, b) = Pair(1, 2)
来源：http://pq.bjjhwx.cn

[T13] Kotlin：只读 Map
来源：http://sd.haigaiapp.cn

val m = mapOf("a" to 1)
来源：http://yg.gzmigu.cn

[T14] Kotlin：循环
来源：http://re.panjiajie.cn

for (i in 1..10) println(i)
来源：http://lr.jianghongdianzi.cn

[T15] Kotlin：接口
来源：http://fc.hnjuh.cn

interface Shape { fun area(): Double }
来源：http://ae.9csxet.cn

[T16] Swift：Hello World
来源：http://jf.wgjwhj.cn

print("Hello")
来源：http://en.nszjky.cn

[T17] Swift：变量与常量
来源：http://zp.shtwfgs.cn

var a = 1;  let b = 2
来源：http://xz.521024.cn

[T18] Swift：字符串插值
来源：http://qs.jianghongdianzi.cn

"值: \(b)"
来源：http://xk.9csxet.cn

[T19] Swift：可选绑定
来源：http://nm.shxzukj.cn

if let n = opt { print(n) }
来源：http://cw.szxytkj.cn

[T20] Swift：数组操作
来源：http://fa.szsharing.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hc.nicolike.cn

[T21] Swift：遍历
来源：http://ts.szsharing.cn

for x in a { print(x) }
来源：http://oh.szsharing.cn

[T22] Swift：字典
来源：http://bs.hnjuh.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mj.bjjhwx.cn

[T23] Swift：函数
来源：http://jr.wgjwhj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://au.chemitech.net.cn

[T24] Swift：闭包
来源：http://ey.muxihuayi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://sz.haigaiapp.cn

[T25] Swift：结构体
来源：http://kk.szsharing.cn

struct P { var x: Int }
来源：http://yp.shtwfgs.cn

[T26] Swift：类与重写
来源：http://lz.wgjwhj.cn

class A: Base { override func f() {} }
来源：http://sy.shxzskj.cn

[T27] Swift：错误处理
来源：http://ra.nicolike.cn

do { try f() } catch { print(error) }
来源：http://qf.colortex.cn

[T28] Swift：枚举
来源：http://pr.bjjhwx.cn

enum Color { case red, green }
来源：http://ax.lnxyls.cn

[T29] Swift：guard 提前返回
来源：http://sd.yuexingan06.cn

guard let x = opt else { return }
来源：http://bh.bookmarksfly.cn

[T30] Swift：协议
来源：http://cp.colortex.cn

protocol Shape { func area() -> Double }
来源：http://ji.chemitech.net.cn

[T31] Lua：Hello World
来源：http://po.yuexingan06.cn

print("Hello")
来源：http://fe.shtwfgs.cn

[T32] Lua：局部变量
来源：http://zu.huanxung.cn

local a = 1
来源：http://mb.shxzskj.cn

[T33] Lua：表（数组）
来源：http://om.hnjuh.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wu.huixiangedu.cn

[T34] Lua：遍历表
来源：http://sh.521024.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vv.colortex.cn

[T35] Lua：字典表
来源：http://ew.gzmigu.cn

local d = { a = 1 };  d.b = 2
来源：http://ah.szxytkj.cn

[T36] Lua：函数
来源：http://qx.bjjhwx.cn

function add(a, b) return a + b end
来源：http://wc.gzmigu.cn

[T37] Lua：字符串拼接
来源：http://xt.asd995.cn

"a" .. "b"
来源：http://vx.szxytkj.cn

[T38] Lua：条件
来源：http://pd.panjiajie.cn

if x > 0 then print("正") end
来源：http://rj.gzmigu.cn

[T39] Lua：模式匹配
来源：http://qv.nicolike.cn

string.find(s, "%d+")
来源：http://ut.chemitech.net.cn

[T40] Lua：元表
来源：http://vb.yuexingan06.cn

setmetatable({}, { __index = base })
来源：http://gc.huixiangedu.cn

[T41] Perl：Hello World
来源：http://qs.shtwfgs.cn

print "Hello\n";
来源：http://ea.huanxung.cn

[T42] Perl：变量类型
来源：http://at.nicolike.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tl.chemitech.net.cn

[T43] Perl：字符串插值
来源：http://id.asd995.cn

"值: $a"
来源：http://mb.yuntaijiaju.cn

[T44] Perl：条件
来源：http://na.jianghongdianzi.cn

if ($a > 0) { print "正"; }
来源：http://gm.colortex.cn

[T45] Perl：数组遍历
来源：http://bm.yuntaijiaju.cn

for my $x (@arr) { print $x; }
来源：http://xc.haigaiapp.cn

[T46] Perl：哈希操作
来源：http://cp.chemitech.net.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://es.muxihuayi.cn

[T47] Perl：正则捕获
来源：http://gf.hnjuh.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://uz.hnjuh.cn

[T48] Perl：正则替换
来源：http://os.hnjuh.cn

$s =~ s/old/new/g;
来源：http://sp.huanxung.cn

[T49] Perl：函数
来源：http://gq.huanxung.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qh.jianghongdianzi.cn

[T50] Perl：逐行读文件
来源：http://jq.panjiajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zy.wgjwhj.cn

while (my $line = <$fh>) { print $line; }
来源：http://kn.hnjuh.cn

[T51] Scala：Hello World
来源：http://ai.wgjwhj.cn

println("Hello")
来源：http://kd.521024.cn

[T52] Scala：变量
来源：http://pa.gzmigu.cn

val a = 1;  var b = 2
来源：http://ah.shtwfgs.cn

[T53] Scala：字符串插值
来源：http://gx.bjjhwx.cn

s"值: $b"
来源：http://fv.szxytkj.cn

[T54] Scala：集合映射
来源：http://gw.nicolike.cn

List(1, 2, 3).map(_ * 2)
来源：http://he.muxihuayi.cn

[T55] Scala：集合过滤
来源：http://xk.yuexingan06.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gk.nszjky.cn

[T56] Scala：样例类
来源：http://kv.shxzukj.cn

case class User(name: String, age: Int)
来源：http://tp.newstarts.cn

[T57] Scala：模式匹配
来源：http://cy.bjjhwx.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://mw.chemitech.net.cn

[T58] Scala：函数定义
来源：http://gl.yuntaijiaju.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fh.asd995.cn

[T59] Scala：循环
来源：http://td.nicolike.cn

for (i <- 1 to 10) println(i)
来源：http://dh.nicolike.cn

[T60] Scala：折叠
来源：http://di.jianghongdianzi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ms.chemitech.net.cn

================================================================================
来源：http://hn.bookmarksfly.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kv.wgjwhj.cn

================================================================================
来源：http://bw.asd995.cn

[U01] Py：创建虚拟环境
来源：http://rf.yuntaijiaju.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jn.shtwfgs.cn

[U02] Py：导出 / 安装依赖
来源：http://wq.bookmarksfly.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ch.shxzukj.cn

[U03] Py：加载 .env 配置
来源：http://yh.yuexingan06.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gq.shxzskj.cn

[U04] Py：变量调试打印
来源：http://ll.colortex.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qu.hnjuh.cn

[U05] Py：列表去重且保序
来源：http://vw.wgjwhj.cn

list(dict.fromkeys(arr))
来源：http://xj.wgjwhj.cn

[U06] Py：合并两个字典
来源：http://jg.nicolike.cn

{**a, **b}
来源：http://ud.szxytkj.cn

[U07] Py：反转字典键值
来源：http://cu.521024.cn

{v: k for k, v in d.items()}
来源：http://wa.chemitech.net.cn

[U08] Py：展平二维列表
来源：http://od.jianghongdianzi.cn

[y for x in nested for y in x]
来源：http://wi.nszjky.cn

[U09] Py：字典取最大值的键
来源：http://uv.shxzukj.cn

max(d, key=d.get)
来源：http://mx.szsharing.cn

[U10] Py：按值排序字典
来源：http://fz.asd995.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rw.521024.cn

[U11] Py：生成器表达式
来源：http://iv.521024.cn

(x * 2 for x in arr)
来源：http://wf.bookmarksfly.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xs.jianghongdianzi.cn

Counter(arr).most_common(3)
来源：http://mk.nszjky.cn

[U13] Py：固定长度队列
来源：http://gs.huixinmuqiang.cn

deque(maxlen=10)
来源：http://cu.nicolike.cn

[U14] Py：分组收集到列表
来源：http://cx.hahajie.cn

defaultdict(list)
来源：http://iv.bjjhwx.cn

[U15] Py：高精度计时
来源：http://ww.newstarts.cn

t = time.perf_counter()
来源：http://gb.shxzukj.cn

[U16] Py：命令行参数解析
来源：http://jw.jianghongdianzi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kc.asd995.cn

[U17] Py：初始化日志
来源：http://hf.chemitech.net.cn

logging.basicConfig(level=logging.INFO)
来源：http://ho.shxzukj.cn

[U18] Py：预编译正则
来源：http://cq.szxytkj.cn

pat = re.compile(r"\d+")
来源：http://eg.gzmigu.cn

[U19] Py：正则替换带回调
来源：http://lj.bookmarksfly.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cy.nicolike.cn

[U20] Py：缓存函数结果
来源：http://nh.hnjuh.cn

@functools.lru_cache(maxsize=None)
来源：http://xs.hnjuh.cn

[U21] Py：自定义上下文管理器
来源：http://iz.yuexingan06.cn

@contextlib.contextmanager
来源：http://ta.yuntaijiaju.cn

[U22] Py：矩阵转置
来源：http://pt.hahajie.cn

list(zip(*m))
来源：http://bi.asd995.cn

[U23] Py：分块读取大文件
来源：http://rk.newstarts.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nj.nicolike.cn

[U24] Py：路径操作
来源：http://gl.jianghongdianzi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ya.yuexingan06.cn

[U25] Py：CSV 按字典读
来源：http://zf.asd995.cn

csv.DictReader(f)
来源：http://jm.colortex.cn

[U26] Py：并发下载
来源：http://lj.wgjwhj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lh.szsharing.cn

[U27] Py：异步 HTTP
来源：http://wo.asd995.cn

aiohttp.ClientSession() 配合 async with
来源：http://sn.hnjuh.cn

[U28] Py：类型别名
来源：http://fi.521024.cn

UserId = int
来源：http://ns.shtwfgs.cn

[U29] Py：属性校验
来源：http://qq.muxihuayi.cn

@property 与 @x.setter 配合
来源：http://rk.jctech888.com.cn

[U30] Py：数据类
来源：http://at.shxzukj.cn

@dataclass(slots=True)
来源：http://qy.haigaiapp.cn

[U31] Py：单测
来源：http://te.newstarts.cn

python -m pytest -q
来源：http://cj.521024.cn

[U32] Py：代码格式化
来源：http://yj.shtwfgs.cn

ruff format . && ruff check --fix .
来源：http://so.muxihuayi.cn

[U33] Py：打包发布
来源：http://dm.muxihuayi.cn

python -m build  （依赖 pyproject.toml）
来源：http://ie.bookmarksfly.cn

[U34] Py：判断编码
来源：http://kt.shxzukj.cn

chardet.detect(raw)
来源：http://cw.yuexingan06.cn

[U35] Py：发送邮件
来源：http://qi.newstarts.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lj.szxytkj.cn

[U36] Py：定时任务
来源：http://da.yuntaijiaju.cn

schedule.every(10).minutes.do(job)
来源：http://pr.huanxung.cn

[U37] Py：读写 Excel
来源：http://hb.hnjuh.cn

pandas.read_excel / DataFrame.to_excel
来源：http://xy.asd995.cn

[U38] Py：获取脚本所在目录
来源：http://fc.hahajie.cn

Path(__file__).resolve().parent
来源：http://jd.huanxung.cn

[U39] Py：判断是否在交互环境
来源：http://pr.huixinmuqiang.cn

sys.stdout.isatty()
来源：http://sj.shtwfgs.cn

[U40] Py：打印到标准错误
来源：http://hb.lnxyls.cn

print("err", file=sys.stderr)
来源：http://dx.hnjuh.cn

[U41] PHP：初始化 Composer 项目
来源：http://bi.bookmarksfly.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://tl.bookmarksfly.cn

[U42] PHP：PSR-4 自动加载
来源：http://qw.muxihuayi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rk.shxzskj.cn

[U43] PHP：声明命名空间
来源：http://at.panjiajie.cn

namespace App\Http;
来源：http://pw.asd995.cn

[U44] PHP：开启严格类型
来源：http://jy.szsharing.cn

declare(strict_types=1);
来源：http://mn.bjjhwx.cn

[U45] PHP：类型声明与返回类型
来源：http://fy.yuexingan06.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://uh.chemitech.net.cn

[U46] PHP：可空类型
来源：http://fg.bookmarksfly.cn

?string $name = null
来源：http://jz.9csxet.cn

[U47] PHP：联合类型
来源：http://yb.asd995.cn

int|string $id
来源：http://ij.521024.cn

[U48] PHP：纯枚举
来源：http://wq.jctech888.com.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dk.chemitech.net.cn

[U49] PHP：只读属性
来源：http://hj.jianghongdianzi.cn

public readonly string $name
来源：http://wb.panjiajie.cn

[U50] PHP：构造器属性提升
来源：http://kd.panjiajie.cn

public function __construct(private int $id) {}
来源：http://nn.gzmigu.cn

[U51] PHP：数组解构
来源：http://xr.nszjky.cn

[$a, $b] = $arr;
来源：http://pk.shtwfgs.cn

[U52] PHP：箭头函数
来源：http://cr.huanxung.cn

$double = fn($x) => $x * 2;
来源：http://cd.huixinmuqiang.cn

[U53] PHP：空合并运算符
来源：http://ry.lnxyls.cn

$v = $a ?? $b ?? "default";
来源：http://gv.gzmigu.cn

[U54] PHP：空安全调用
来源：http://ol.chemitech.net.cn

$obj?->method()
来源：http://ek.bjjhwx.cn

[U55] PHP：match 表达式
来源：http://so.bookmarksfly.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zw.bookmarksfly.cn

[U56] PHP：命名参数
来源：http://vm.huixinmuqiang.cn

f(a: 1, b: 2)
来源：http://ah.huixiangedu.cn

[U57] PHP：字符串插值
来源：http://hs.haigaiapp.cn

"值: {$a}"
来源：http://va.lnxyls.cn

[U58] PHP：数组三件套
来源：http://dd.haigaiapp.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kh.newstarts.cn

[U59] PHP：自定义排序
来源：http://zh.chemitech.net.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pe.newstarts.cn

[U60] PHP：JSON 编解码
来源：http://mu.huixinmuqiang.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zi.szsharing.cn

[U61] PHP：正则
来源：http://pe.huanxung.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cz.chemitech.net.cn

[U62] PHP：日期对象
来源：http://dd.bookmarksfly.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mh.yuexingan06.cn

[U63] PHP：文件读写
来源：http://ve.colortex.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hy.yuexingan06.cn

[U64] PHP：目录遍历
来源：http://sj.wgjwhj.cn

glob("dir/*.php");  scandir("dir");
来源：http://md.szsharing.cn

[U65] PHP：会话
来源：http://vn.shtwfgs.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vw.hnjuh.cn

[U66] PHP：设置 Cookie
来源：http://ft.nicolike.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gb.asd995.cn

[U67] PHP：处理文件上传
来源：http://yn.bookmarksfly.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qm.hnjuh.cn

[U68] PHP：PDO 连接
来源：http://tt.haigaiapp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vd.muxihuayi.cn

[U69] PHP：PDO 预处理
来源：http://fo.panjiajie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bx.newstarts.cn

[U70] PHP：PDO 事务
来源：http://xj.yuntaijiaju.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bl.nicolike.cn

[U71] PHP：抛出异常
来源：http://cv.wgjwhj.cn

throw new RuntimeException("失败", 500);
来源：http://id.jctech888.com.cn

[U72] PHP：写错误日志
来源：http://pm.colortex.cn

error_log("失败: " . $e->getMessage());
来源：http://fw.huixinmuqiang.cn

[U73] PHP：读取 ini 配置
来源：http://td.szxytkj.cn

parse_ini_file("config.ini", true)
来源：http://mn.colortex.cn

[U74] PHP：读取环境变量
来源：http://gp.nicolike.cn

getenv("APP_ENV") ?: "production"
来源：http://cw.yuexingan06.cn

[U75] PHP：依赖注入
来源：http://si.wgjwhj.cn

composer require psr/container
来源：http://hx.nszjky.cn

[U76] PHP：简单路由
来源：http://dj.nszjky.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rp.huixiangedu.cn

[U77] PHP：模板渲染
来源：http://ee.9csxet.cn

composer require twig/twig
来源：http://ey.nszjky.cn

[U78] PHP：单元测试
来源：http://lu.colortex.cn

composer require --dev phpunit/phpunit
来源：http://wu.lnxyls.cn

[U79] PHP：静态分析
来源：http://cb.521024.cn

composer require --dev phpstan/phpstan
来源：http://fr.521024.cn

[U80] PHP：代码规范修复
来源：http://qx.yuexingan06.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jt.huixinmuqiang.cn

[U81] JS：初始化项目
来源：http://vk.shxzukj.cn

npm init -y;  npm i express
来源：http://ct.521024.cn

[U82] JS：package.json 脚本
来源：http://pb.nszjky.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lg.shxzukj.cn

[U83] JS：ES Module 导入导出
来源：http://ia.gzmigu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://in.521024.cn

[U84] JS：CommonJS 写法
来源：http://mo.9csxet.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ek.colortex.cn

[U85] JS：可选链
来源：http://bt.haigaiapp.cn

a?.b?.c
来源：http://di.gzmigu.cn

[U86] JS：空值合并
来源：http://sa.shtwfgs.cn

a ?? b
来源：http://fs.huanxung.cn

[U87] JS：解构默认值
来源：http://do.panjiajie.cn

const { a = 1, b = 2 } = obj;
来源：http://rq.521024.cn

[U88] JS：对象展开合并
来源：http://zw.wgjwhj.cn

{ ...a, ...b }
来源：http://la.hnjuh.cn

[U89] JS：数组去重
来源：http://st.shxzukj.cn

[...new Set(arr)]
来源：http://se.shxzukj.cn

[U90] JS：数字数组排序
来源：http://os.hahajie.cn

[...arr].sort((a, b) => a - b)
来源：http://wu.9csxet.cn

[U91] JS：对象键值遍历
来源：http://vm.shtwfgs.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://uc.colortex.cn

[U92] JS：深拷贝
来源：http://qz.haigaiapp.cn

structuredClone(obj)
来源：http://yu.newstarts.cn

[U93] JS：模板字符串
来源：http://he.shxzukj.cn

`共 ${n} 条`
来源：http://mx.szsharing.cn

[U94] JS：箭头函数
来源：http://rk.hahajie.cn

const double = x => x * 2;
来源：http://hh.huixinmuqiang.cn


<!-- 参考信息 -->