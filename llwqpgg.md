代发 wailian999

[T09] Kotlin：扩展函数
来源：http://xw.colortex.cn

fun String.exclaim() = this + "!"
来源：http://fl.521024.cn

[T10] Kotlin：默认参数
来源：http://xa.nszjky.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wt.nszjky.cn

[T11] Kotlin：协程
来源：http://un.muxihuayi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nm.colortex.cn

[T12] Kotlin：解构声明
来源：http://ke.bjjhwx.cn

val (a, b) = Pair(1, 2)
来源：http://tc.newstarts.cn

[T13] Kotlin：只读 Map
来源：http://eh.bjjhwx.cn

val m = mapOf("a" to 1)
来源：http://jd.lnxyls.cn

[T14] Kotlin：循环
来源：http://ve.nszjky.cn

for (i in 1..10) println(i)
来源：http://ng.yuexingan06.cn

[T15] Kotlin：接口
来源：http://he.bjjhwx.cn

interface Shape { fun area(): Double }
来源：http://ma.huixiangedu.cn

[T16] Swift：Hello World
来源：http://hp.chemitech.net.cn

print("Hello")
来源：http://my.newstarts.cn

[T17] Swift：变量与常量
来源：http://hr.jianghongdianzi.cn

var a = 1;  let b = 2
来源：http://ha.lnxyls.cn

[T18] Swift：字符串插值
来源：http://fp.jctech888.com.cn

"值: \(b)"
来源：http://zw.haigaiapp.cn

[T19] Swift：可选绑定
来源：http://rn.jctech888.com.cn

if let n = opt { print(n) }
来源：http://ko.gzmigu.cn

[T20] Swift：数组操作
来源：http://dt.asd995.cn

var a = [1, 2, 3];  a.append(4)
来源：http://dq.huanxung.cn

[T21] Swift：遍历
来源：http://hy.jianghongdianzi.cn

for x in a { print(x) }
来源：http://ai.nicolike.cn

[T22] Swift：字典
来源：http://ah.colortex.cn

var d = ["a": 1];  d["b"] = 2
来源：http://eu.gzmigu.cn

[T23] Swift：函数
来源：http://qf.huanxung.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dz.szsharing.cn

[T24] Swift：闭包
来源：http://xz.huanxung.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://fj.jianghongdianzi.cn

[T25] Swift：结构体
来源：http://lp.shtwfgs.cn

struct P { var x: Int }
来源：http://wz.shtwfgs.cn

[T26] Swift：类与重写
来源：http://xm.lnxyls.cn

class A: Base { override func f() {} }
来源：http://kd.panjiajie.cn

[T27] Swift：错误处理
来源：http://py.521024.cn

do { try f() } catch { print(error) }
来源：http://yd.huanxung.cn

[T28] Swift：枚举
来源：http://ch.panjiajie.cn

enum Color { case red, green }
来源：http://hl.huixiangedu.cn

[T29] Swift：guard 提前返回
来源：http://ey.bookmarksfly.cn

guard let x = opt else { return }
来源：http://qv.jianghongdianzi.cn

[T30] Swift：协议
来源：http://el.jctech888.com.cn

protocol Shape { func area() -> Double }
来源：http://ad.shxzskj.cn

[T31] Lua：Hello World
来源：http://ba.hahajie.cn

print("Hello")
来源：http://vi.nszjky.cn

[T32] Lua：局部变量
来源：http://uk.panjiajie.cn

local a = 1
来源：http://pz.szxytkj.cn

[T33] Lua：表（数组）
来源：http://yj.wgjwhj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://pl.bookmarksfly.cn

[T34] Lua：遍历表
来源：http://ls.nicolike.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://lp.haigaiapp.cn

[T35] Lua：字典表
来源：http://gq.szxytkj.cn

local d = { a = 1 };  d.b = 2
来源：http://sc.yuexingan06.cn

[T36] Lua：函数
来源：http://mo.szsharing.cn

function add(a, b) return a + b end
来源：http://wu.wgjwhj.cn

[T37] Lua：字符串拼接
来源：http://mn.haigaiapp.cn

"a" .. "b"
来源：http://eu.asd995.cn

[T38] Lua：条件
来源：http://mi.huixinmuqiang.cn

if x > 0 then print("正") end
来源：http://ew.jctech888.com.cn

[T39] Lua：模式匹配
来源：http://xg.chemitech.net.cn

string.find(s, "%d+")
来源：http://zc.gzmigu.cn

[T40] Lua：元表
来源：http://iu.jianghongdianzi.cn

setmetatable({}, { __index = base })
来源：http://ft.huixinmuqiang.cn

[T41] Perl：Hello World
来源：http://uu.haigaiapp.cn

print "Hello\n";
来源：http://ch.yuntaijiaju.cn

[T42] Perl：变量类型
来源：http://hu.9csxet.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ln.jianghongdianzi.cn

[T43] Perl：字符串插值
来源：http://zl.muxihuayi.cn

"值: $a"
来源：http://rr.9csxet.cn

[T44] Perl：条件
来源：http://hb.panjiajie.cn

if ($a > 0) { print "正"; }
来源：http://br.huanxung.cn

[T45] Perl：数组遍历
来源：http://wd.521024.cn

for my $x (@arr) { print $x; }
来源：http://ia.huixiangedu.cn

[T46] Perl：哈希操作
来源：http://os.huixinmuqiang.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qj.gzmigu.cn

[T47] Perl：正则捕获
来源：http://nj.jianghongdianzi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ws.bookmarksfly.cn

[T48] Perl：正则替换
来源：http://bi.hahajie.cn

$s =~ s/old/new/g;
来源：http://sw.szsharing.cn

[T49] Perl：函数
来源：http://gr.wgjwhj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sp.haigaiapp.cn

[T50] Perl：逐行读文件
来源：http://jp.colortex.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ss.bjjhwx.cn

while (my $line = <$fh>) { print $line; }
来源：http://ys.huixinmuqiang.cn

[T51] Scala：Hello World
来源：http://rn.huixiangedu.cn

println("Hello")
来源：http://nm.hahajie.cn

[T52] Scala：变量
来源：http://hv.yuntaijiaju.cn

val a = 1;  var b = 2
来源：http://fr.nszjky.cn

[T53] Scala：字符串插值
来源：http://vv.yuexingan06.cn

s"值: $b"
来源：http://md.hnjuh.cn

[T54] Scala：集合映射
来源：http://ys.haigaiapp.cn

List(1, 2, 3).map(_ * 2)
来源：http://bo.nicolike.cn

[T55] Scala：集合过滤
来源：http://jj.newstarts.cn

List(1, 2, 3).filter(_ > 1)
来源：http://uz.colortex.cn

[T56] Scala：样例类
来源：http://jl.bookmarksfly.cn

case class User(name: String, age: Int)
来源：http://uf.huanxung.cn

[T57] Scala：模式匹配
来源：http://sm.huixiangedu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ij.colortex.cn

[T58] Scala：函数定义
来源：http://qu.521024.cn

def add(a: Int, b: Int): Int = a + b
来源：http://qn.haigaiapp.cn

[T59] Scala：循环
来源：http://np.gzmigu.cn

for (i <- 1 to 10) println(i)
来源：http://ju.jianghongdianzi.cn

[T60] Scala：折叠
来源：http://tv.shxzukj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gv.shxzukj.cn

================================================================================
来源：http://cj.gzmigu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hw.nszjky.cn

================================================================================
来源：http://pt.colortex.cn

[U01] Py：创建虚拟环境
来源：http://sd.nicolike.cn

python -m venv .venv && source .venv/bin/activate
来源：http://uk.shtwfgs.cn

[U02] Py：导出 / 安装依赖
来源：http://lu.hnjuh.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zd.chemitech.net.cn

[U03] Py：加载 .env 配置
来源：http://hj.chemitech.net.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zy.colortex.cn

[U04] Py：变量调试打印
来源：http://yh.panjiajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jk.yuntaijiaju.cn

[U05] Py：列表去重且保序
来源：http://qc.asd995.cn

list(dict.fromkeys(arr))
来源：http://pe.panjiajie.cn

[U06] Py：合并两个字典
来源：http://cj.colortex.cn

{**a, **b}
来源：http://tf.bjjhwx.cn

[U07] Py：反转字典键值
来源：http://ai.yuntaijiaju.cn

{v: k for k, v in d.items()}
来源：http://rp.wgjwhj.cn

[U08] Py：展平二维列表
来源：http://qo.huixinmuqiang.cn

[y for x in nested for y in x]
来源：http://vc.bjjhwx.cn

[U09] Py：字典取最大值的键
来源：http://yx.huixiangedu.cn

max(d, key=d.get)
来源：http://vb.nszjky.cn

[U10] Py：按值排序字典
来源：http://nl.shxzskj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jk.haigaiapp.cn

[U11] Py：生成器表达式
来源：http://kl.lnxyls.cn

(x * 2 for x in arr)
来源：http://ok.huixiangedu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ro.colortex.cn

Counter(arr).most_common(3)
来源：http://pn.shxzskj.cn

[U13] Py：固定长度队列
来源：http://ax.lnxyls.cn

deque(maxlen=10)
来源：http://to.shtwfgs.cn

[U14] Py：分组收集到列表
来源：http://mh.huixinmuqiang.cn

defaultdict(list)
来源：http://lt.muxihuayi.cn

[U15] Py：高精度计时
来源：http://sk.asd995.cn

t = time.perf_counter()
来源：http://lb.gzmigu.cn

[U16] Py：命令行参数解析
来源：http://zj.asd995.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lm.lnxyls.cn

[U17] Py：初始化日志
来源：http://oi.lnxyls.cn

logging.basicConfig(level=logging.INFO)
来源：http://va.9csxet.cn

[U18] Py：预编译正则
来源：http://fj.haigaiapp.cn

pat = re.compile(r"\d+")
来源：http://vw.huixiangedu.cn

[U19] Py：正则替换带回调
来源：http://ln.521024.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ti.jctech888.com.cn

[U20] Py：缓存函数结果
来源：http://yv.bookmarksfly.cn

@functools.lru_cache(maxsize=None)
来源：http://xr.muxihuayi.cn

[U21] Py：自定义上下文管理器
来源：http://td.bjjhwx.cn

@contextlib.contextmanager
来源：http://lg.jianghongdianzi.cn

[U22] Py：矩阵转置
来源：http://yt.asd995.cn

list(zip(*m))
来源：http://jp.yuexingan06.cn

[U23] Py：分块读取大文件
来源：http://rc.shtwfgs.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wq.shxzskj.cn

[U24] Py：路径操作
来源：http://rs.chemitech.net.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kk.huixiangedu.cn

[U25] Py：CSV 按字典读
来源：http://jg.gzmigu.cn

csv.DictReader(f)
来源：http://zf.asd995.cn

[U26] Py：并发下载
来源：http://pw.hnjuh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xa.nszjky.cn

[U27] Py：异步 HTTP
来源：http://ap.huixiangedu.cn

aiohttp.ClientSession() 配合 async with
来源：http://lx.muxihuayi.cn

[U28] Py：类型别名
来源：http://ud.wgjwhj.cn

UserId = int
来源：http://iq.nicolike.cn

[U29] Py：属性校验
来源：http://pv.asd995.cn

@property 与 @x.setter 配合
来源：http://gx.haigaiapp.cn

[U30] Py：数据类
来源：http://mb.szsharing.cn

@dataclass(slots=True)
来源：http://bd.haigaiapp.cn

[U31] Py：单测
来源：http://rt.yuntaijiaju.cn

python -m pytest -q
来源：http://vl.jianghongdianzi.cn

[U32] Py：代码格式化
来源：http://eq.shtwfgs.cn

ruff format . && ruff check --fix .
来源：http://ck.hahajie.cn

[U33] Py：打包发布
来源：http://gq.hahajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://pv.yuexingan06.cn

[U34] Py：判断编码
来源：http://aq.hnjuh.cn

chardet.detect(raw)
来源：http://ms.yuntaijiaju.cn

[U35] Py：发送邮件
来源：http://yu.jianghongdianzi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zx.asd995.cn

[U36] Py：定时任务
来源：http://qz.gzmigu.cn

schedule.every(10).minutes.do(job)
来源：http://ha.yuntaijiaju.cn

[U37] Py：读写 Excel
来源：http://on.shxzukj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://up.chemitech.net.cn

[U38] Py：获取脚本所在目录
来源：http://ia.9csxet.cn

Path(__file__).resolve().parent
来源：http://bv.asd995.cn

[U39] Py：判断是否在交互环境
来源：http://ui.jianghongdianzi.cn

sys.stdout.isatty()
来源：http://og.huixiangedu.cn

[U40] Py：打印到标准错误
来源：http://go.colortex.cn

print("err", file=sys.stderr)
来源：http://sq.yuntaijiaju.cn

[U41] PHP：初始化 Composer 项目
来源：http://ov.jianghongdianzi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://mi.shxzskj.cn

[U42] PHP：PSR-4 自动加载
来源：http://wv.lnxyls.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hb.jianghongdianzi.cn

[U43] PHP：声明命名空间
来源：http://rv.bjjhwx.cn

namespace App\Http;
来源：http://qu.huixinmuqiang.cn

[U44] PHP：开启严格类型
来源：http://rl.9csxet.cn

declare(strict_types=1);
来源：http://so.chemitech.net.cn

[U45] PHP：类型声明与返回类型
来源：http://bh.jianghongdianzi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://et.jianghongdianzi.cn

[U46] PHP：可空类型
来源：http://fi.chemitech.net.cn

?string $name = null
来源：http://ag.szxytkj.cn

[U47] PHP：联合类型
来源：http://dz.yuexingan06.cn

int|string $id
来源：http://zs.muxihuayi.cn

[U48] PHP：纯枚举
来源：http://un.9csxet.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://io.bookmarksfly.cn

[U49] PHP：只读属性
来源：http://ef.yuexingan06.cn

public readonly string $name
来源：http://em.huixiangedu.cn

[U50] PHP：构造器属性提升
来源：http://pj.lnxyls.cn

public function __construct(private int $id) {}
来源：http://sn.shxzukj.cn

[U51] PHP：数组解构
来源：http://wj.panjiajie.cn

[$a, $b] = $arr;
来源：http://fi.jianghongdianzi.cn

[U52] PHP：箭头函数
来源：http://bq.nszjky.cn

$double = fn($x) => $x * 2;
来源：http://ie.hahajie.cn

[U53] PHP：空合并运算符
来源：http://iu.bjjhwx.cn

$v = $a ?? $b ?? "default";
来源：http://iw.szxytkj.cn

[U54] PHP：空安全调用
来源：http://ss.szsharing.cn

$obj?->method()
来源：http://aj.lnxyls.cn

[U55] PHP：match 表达式
来源：http://ri.shxzukj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gd.jctech888.com.cn

[U56] PHP：命名参数
来源：http://jz.newstarts.cn

f(a: 1, b: 2)
来源：http://dk.bjjhwx.cn

[U57] PHP：字符串插值
来源：http://sp.muxihuayi.cn

"值: {$a}"
来源：http://cr.shtwfgs.cn

[U58] PHP：数组三件套
来源：http://cv.jctech888.com.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gj.nicolike.cn

[U59] PHP：自定义排序
来源：http://sv.jianghongdianzi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cl.nszjky.cn

[U60] PHP：JSON 编解码
来源：http://bp.newstarts.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lb.colortex.cn

[U61] PHP：正则
来源：http://ts.newstarts.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qw.panjiajie.cn

[U62] PHP：日期对象
来源：http://ml.jctech888.com.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ro.yuexingan06.cn

[U63] PHP：文件读写
来源：http://ak.9csxet.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dh.colortex.cn

[U64] PHP：目录遍历
来源：http://ek.muxihuayi.cn

glob("dir/*.php");  scandir("dir");
来源：http://sk.shtwfgs.cn

[U65] PHP：会话
来源：http://ym.lnxyls.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ng.szxytkj.cn

[U66] PHP：设置 Cookie
来源：http://dq.yuexingan06.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zg.gzmigu.cn

[U67] PHP：处理文件上传
来源：http://lo.haigaiapp.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dg.szxytkj.cn

[U68] PHP：PDO 连接
来源：http://xu.muxihuayi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://st.gzmigu.cn

[U69] PHP：PDO 预处理
来源：http://sg.wgjwhj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ku.yuexingan06.cn

[U70] PHP：PDO 事务
来源：http://rn.jctech888.com.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sx.bookmarksfly.cn

[U71] PHP：抛出异常
来源：http://px.lnxyls.cn

throw new RuntimeException("失败", 500);
来源：http://wr.huixiangedu.cn

[U72] PHP：写错误日志
来源：http://hh.hnjuh.cn

error_log("失败: " . $e->getMessage());
来源：http://rb.chemitech.net.cn

[U73] PHP：读取 ini 配置
来源：http://cz.panjiajie.cn

parse_ini_file("config.ini", true)
来源：http://hi.wgjwhj.cn

[U74] PHP：读取环境变量
来源：http://ca.gzmigu.cn

getenv("APP_ENV") ?: "production"
来源：http://zx.colortex.cn

[U75] PHP：依赖注入
来源：http://vk.bjjhwx.cn

composer require psr/container
来源：http://rx.chemitech.net.cn

[U76] PHP：简单路由
来源：http://pv.bjjhwx.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zq.haigaiapp.cn

[U77] PHP：模板渲染
来源：http://is.yuexingan06.cn

composer require twig/twig
来源：http://tg.szxytkj.cn

[U78] PHP：单元测试
来源：http://tl.bookmarksfly.cn

composer require --dev phpunit/phpunit
来源：http://cm.haigaiapp.cn

[U79] PHP：静态分析
来源：http://su.9csxet.cn

composer require --dev phpstan/phpstan
来源：http://gt.bjjhwx.cn

[U80] PHP：代码规范修复
来源：http://od.asd995.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://rb.yuntaijiaju.cn

[U81] JS：初始化项目
来源：http://tb.lnxyls.cn

npm init -y;  npm i express
来源：http://dx.huanxung.cn

[U82] JS：package.json 脚本
来源：http://xw.hnjuh.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vf.gzmigu.cn

[U83] JS：ES Module 导入导出
来源：http://qr.huanxung.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ej.haigaiapp.cn

[U84] JS：CommonJS 写法
来源：http://al.521024.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ew.szxytkj.cn

[U85] JS：可选链
来源：http://ab.jianghongdianzi.cn

a?.b?.c
来源：http://qj.bjjhwx.cn

[U86] JS：空值合并
来源：http://vw.chemitech.net.cn

a ?? b
来源：http://ld.yuntaijiaju.cn

[U87] JS：解构默认值
来源：http://og.9csxet.cn

const { a = 1, b = 2 } = obj;
来源：http://uo.wgjwhj.cn

[U88] JS：对象展开合并
来源：http://nk.jianghongdianzi.cn

{ ...a, ...b }
来源：http://yz.muxihuayi.cn

[U89] JS：数组去重
来源：http://wu.hnjuh.cn

[...new Set(arr)]
来源：http://bb.shtwfgs.cn

[U90] JS：数字数组排序
来源：http://pv.jianghongdianzi.cn

[...arr].sort((a, b) => a - b)
来源：http://po.hahajie.cn

[U91] JS：对象键值遍历
来源：http://zs.colortex.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://di.jianghongdianzi.cn

[U92] JS：深拷贝
来源：http://cc.gzmigu.cn

structuredClone(obj)
来源：http://he.szxytkj.cn

[U93] JS：模板字符串
来源：http://fc.shtwfgs.cn

`共 ${n} 条`
来源：http://mh.nicolike.cn

[U94] JS：箭头函数
来源：http://dp.szsharing.cn

const double = x => x * 2;
来源：http://rd.yuexingan06.cn

[U95] JS：Promise 包装
来源：http://ih.jctech888.com.cn

new Promise((resolve, reject) => {})
来源：http://bw.huanxung.cn

[U96] JS：async/await 与异常
来源：http://nu.chemitech.net.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vf.muxihuayi.cn


<!-- 参考信息 -->