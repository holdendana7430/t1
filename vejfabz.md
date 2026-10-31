代发 wailian999

[T07] Kotlin：集合过滤
来源：http://vr.szxytkj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://rs.wgjwhj.cn

[T08] Kotlin：数据类
来源：http://tt.yuexingan06.cn

data class User(val name: String, val age: Int)
来源：http://yf.newstarts.cn

[T09] Kotlin：扩展函数
来源：http://jd.chemitech.net.cn

fun String.exclaim() = this + "!"
来源：http://dn.bjjhwx.cn

[T10] Kotlin：默认参数
来源：http://js.shxzskj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pq.jctech888.com.cn

[T11] Kotlin：协程
来源：http://wa.szsharing.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://sy.huixinmuqiang.cn

[T12] Kotlin：解构声明
来源：http://rg.shtwfgs.cn

val (a, b) = Pair(1, 2)
来源：http://pe.panjiajie.cn

[T13] Kotlin：只读 Map
来源：http://ai.chemitech.net.cn

val m = mapOf("a" to 1)
来源：http://iw.521024.cn

[T14] Kotlin：循环
来源：http://oh.szsharing.cn

for (i in 1..10) println(i)
来源：http://zq.wgjwhj.cn

[T15] Kotlin：接口
来源：http://zu.asd995.cn

interface Shape { fun area(): Double }
来源：http://fu.jianghongdianzi.cn

[T16] Swift：Hello World
来源：http://ol.bookmarksfly.cn

print("Hello")
来源：http://lh.chemitech.net.cn

[T17] Swift：变量与常量
来源：http://xa.asd995.cn

var a = 1;  let b = 2
来源：http://eg.colortex.cn

[T18] Swift：字符串插值
来源：http://rz.newstarts.cn

"值: \(b)"
来源：http://os.wgjwhj.cn

[T19] Swift：可选绑定
来源：http://sz.hahajie.cn

if let n = opt { print(n) }
来源：http://vp.gzmigu.cn

[T20] Swift：数组操作
来源：http://pb.hnjuh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://al.bookmarksfly.cn

[T21] Swift：遍历
来源：http://zl.hahajie.cn

for x in a { print(x) }
来源：http://qt.haigaiapp.cn

[T22] Swift：字典
来源：http://ta.shtwfgs.cn

var d = ["a": 1];  d["b"] = 2
来源：http://sh.nicolike.cn

[T23] Swift：函数
来源：http://jo.yuexingan06.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uy.huixiangedu.cn

[T24] Swift：闭包
来源：http://tx.hnjuh.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xw.nszjky.cn

[T25] Swift：结构体
来源：http://nc.panjiajie.cn

struct P { var x: Int }
来源：http://ay.521024.cn

[T26] Swift：类与重写
来源：http://pj.shxzukj.cn

class A: Base { override func f() {} }
来源：http://qv.yuexingan06.cn

[T27] Swift：错误处理
来源：http://ma.chemitech.net.cn

do { try f() } catch { print(error) }
来源：http://ot.shtwfgs.cn

[T28] Swift：枚举
来源：http://fp.jianghongdianzi.cn

enum Color { case red, green }
来源：http://td.jianghongdianzi.cn

[T29] Swift：guard 提前返回
来源：http://hf.bjjhwx.cn

guard let x = opt else { return }
来源：http://ev.asd995.cn

[T30] Swift：协议
来源：http://do.bjjhwx.cn

protocol Shape { func area() -> Double }
来源：http://oo.gzmigu.cn

[T31] Lua：Hello World
来源：http://js.huanxung.cn

print("Hello")
来源：http://my.shxzukj.cn

[T32] Lua：局部变量
来源：http://uy.bjjhwx.cn

local a = 1
来源：http://vp.521024.cn

[T33] Lua：表（数组）
来源：http://tf.shtwfgs.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://yu.muxihuayi.cn

[T34] Lua：遍历表
来源：http://dv.szxytkj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ee.szsharing.cn

[T35] Lua：字典表
来源：http://cs.panjiajie.cn

local d = { a = 1 };  d.b = 2
来源：http://wz.jctech888.com.cn

[T36] Lua：函数
来源：http://nc.nicolike.cn

function add(a, b) return a + b end
来源：http://fj.hahajie.cn

[T37] Lua：字符串拼接
来源：http://lh.jctech888.com.cn

"a" .. "b"
来源：http://tq.asd995.cn

[T38] Lua：条件
来源：http://dj.hnjuh.cn

if x > 0 then print("正") end
来源：http://ot.szxytkj.cn

[T39] Lua：模式匹配
来源：http://is.nicolike.cn

string.find(s, "%d+")
来源：http://qg.jianghongdianzi.cn

[T40] Lua：元表
来源：http://tf.hahajie.cn

setmetatable({}, { __index = base })
来源：http://tf.hahajie.cn

[T41] Perl：Hello World
来源：http://io.bookmarksfly.cn

print "Hello\n";
来源：http://xo.yuntaijiaju.cn

[T42] Perl：变量类型
来源：http://mq.huixiangedu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xr.huanxung.cn

[T43] Perl：字符串插值
来源：http://ga.9csxet.cn

"值: $a"
来源：http://uh.chemitech.net.cn

[T44] Perl：条件
来源：http://zs.huanxung.cn

if ($a > 0) { print "正"; }
来源：http://bd.gzmigu.cn

[T45] Perl：数组遍历
来源：http://nw.szsharing.cn

for my $x (@arr) { print $x; }
来源：http://qh.nicolike.cn

[T46] Perl：哈希操作
来源：http://ec.huixiangedu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hv.jianghongdianzi.cn

[T47] Perl：正则捕获
来源：http://mj.asd995.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jt.jctech888.com.cn

[T48] Perl：正则替换
来源：http://yi.haigaiapp.cn

$s =~ s/old/new/g;
来源：http://ij.newstarts.cn

[T49] Perl：函数
来源：http://ux.bjjhwx.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yo.chemitech.net.cn

[T50] Perl：逐行读文件
来源：http://tc.nicolike.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://pn.shtwfgs.cn

while (my $line = <$fh>) { print $line; }
来源：http://if.jianghongdianzi.cn

[T51] Scala：Hello World
来源：http://qa.gzmigu.cn

println("Hello")
来源：http://ti.newstarts.cn

[T52] Scala：变量
来源：http://pc.bookmarksfly.cn

val a = 1;  var b = 2
来源：http://lc.yuntaijiaju.cn

[T53] Scala：字符串插值
来源：http://vi.szxytkj.cn

s"值: $b"
来源：http://tm.nicolike.cn

[T54] Scala：集合映射
来源：http://nw.huixiangedu.cn

List(1, 2, 3).map(_ * 2)
来源：http://ec.huanxung.cn

[T55] Scala：集合过滤
来源：http://ga.panjiajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://zh.bookmarksfly.cn

[T56] Scala：样例类
来源：http://nk.nszjky.cn

case class User(name: String, age: Int)
来源：http://mj.hnjuh.cn

[T57] Scala：模式匹配
来源：http://vg.huixinmuqiang.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://oz.yuntaijiaju.cn

[T58] Scala：函数定义
来源：http://yq.szxytkj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://up.huixinmuqiang.cn

[T59] Scala：循环
来源：http://uu.lnxyls.cn

for (i <- 1 to 10) println(i)
来源：http://ro.9csxet.cn

[T60] Scala：折叠
来源：http://wc.yuexingan06.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sg.bookmarksfly.cn

================================================================================
来源：http://hg.hahajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rj.nszjky.cn

================================================================================
来源：http://nd.chemitech.net.cn

[U01] Py：创建虚拟环境
来源：http://ww.yuexingan06.cn

python -m venv .venv && source .venv/bin/activate
来源：http://hj.muxihuayi.cn

[U02] Py：导出 / 安装依赖
来源：http://zp.yuexingan06.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ja.hahajie.cn

[U03] Py：加载 .env 配置
来源：http://ge.lnxyls.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://sg.asd995.cn

[U04] Py：变量调试打印
来源：http://ww.asd995.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jv.9csxet.cn

[U05] Py：列表去重且保序
来源：http://fw.szsharing.cn

list(dict.fromkeys(arr))
来源：http://xc.jianghongdianzi.cn

[U06] Py：合并两个字典
来源：http://cv.bjjhwx.cn

{**a, **b}
来源：http://ig.haigaiapp.cn

[U07] Py：反转字典键值
来源：http://cr.newstarts.cn

{v: k for k, v in d.items()}
来源：http://az.asd995.cn

[U08] Py：展平二维列表
来源：http://ug.colortex.cn

[y for x in nested for y in x]
来源：http://sc.nszjky.cn

[U09] Py：字典取最大值的键
来源：http://ki.asd995.cn

max(d, key=d.get)
来源：http://pc.9csxet.cn

[U10] Py：按值排序字典
来源：http://vs.newstarts.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ok.shxzskj.cn

[U11] Py：生成器表达式
来源：http://fu.yuntaijiaju.cn

(x * 2 for x in arr)
来源：http://oa.lnxyls.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mj.yuntaijiaju.cn

Counter(arr).most_common(3)
来源：http://jp.chemitech.net.cn

[U13] Py：固定长度队列
来源：http://sx.szxytkj.cn

deque(maxlen=10)
来源：http://fr.colortex.cn

[U14] Py：分组收集到列表
来源：http://bi.yuexingan06.cn

defaultdict(list)
来源：http://gi.newstarts.cn

[U15] Py：高精度计时
来源：http://st.nszjky.cn

t = time.perf_counter()
来源：http://bm.chemitech.net.cn

[U16] Py：命令行参数解析
来源：http://ua.yuntaijiaju.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ba.yuntaijiaju.cn

[U17] Py：初始化日志
来源：http://ry.521024.cn

logging.basicConfig(level=logging.INFO)
来源：http://zq.yuexingan06.cn

[U18] Py：预编译正则
来源：http://gz.jianghongdianzi.cn

pat = re.compile(r"\d+")
来源：http://iz.haigaiapp.cn

[U19] Py：正则替换带回调
来源：http://kj.shxzskj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lc.panjiajie.cn

[U20] Py：缓存函数结果
来源：http://af.jianghongdianzi.cn

@functools.lru_cache(maxsize=None)
来源：http://bd.asd995.cn

[U21] Py：自定义上下文管理器
来源：http://ik.lnxyls.cn

@contextlib.contextmanager
来源：http://oz.newstarts.cn

[U22] Py：矩阵转置
来源：http://za.colortex.cn

list(zip(*m))
来源：http://dx.shtwfgs.cn

[U23] Py：分块读取大文件
来源：http://vm.huanxung.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ex.newstarts.cn

[U24] Py：路径操作
来源：http://rc.muxihuayi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://da.huanxung.cn

[U25] Py：CSV 按字典读
来源：http://ge.yuntaijiaju.cn

csv.DictReader(f)
来源：http://nz.jianghongdianzi.cn

[U26] Py：并发下载
来源：http://gb.wgjwhj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://se.jctech888.com.cn

[U27] Py：异步 HTTP
来源：http://wr.huixiangedu.cn

aiohttp.ClientSession() 配合 async with
来源：http://tp.hahajie.cn

[U28] Py：类型别名
来源：http://qz.huixinmuqiang.cn

UserId = int
来源：http://qr.shxzskj.cn

[U29] Py：属性校验
来源：http://eq.jianghongdianzi.cn

@property 与 @x.setter 配合
来源：http://tn.huanxung.cn

[U30] Py：数据类
来源：http://ef.yuexingan06.cn

@dataclass(slots=True)
来源：http://qm.muxihuayi.cn

[U31] Py：单测
来源：http://re.szxytkj.cn

python -m pytest -q
来源：http://az.yuexingan06.cn

[U32] Py：代码格式化
来源：http://vw.jianghongdianzi.cn

ruff format . && ruff check --fix .
来源：http://yt.gzmigu.cn

[U33] Py：打包发布
来源：http://jx.shxzskj.cn

python -m build  （依赖 pyproject.toml）
来源：http://yt.shxzukj.cn

[U34] Py：判断编码
来源：http://ky.chemitech.net.cn

chardet.detect(raw)
来源：http://mh.521024.cn

[U35] Py：发送邮件
来源：http://wd.colortex.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://av.bjjhwx.cn

[U36] Py：定时任务
来源：http://kt.haigaiapp.cn

schedule.every(10).minutes.do(job)
来源：http://iv.colortex.cn

[U37] Py：读写 Excel
来源：http://wi.szsharing.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qx.jianghongdianzi.cn

[U38] Py：获取脚本所在目录
来源：http://dh.lnxyls.cn

Path(__file__).resolve().parent
来源：http://ib.huanxung.cn

[U39] Py：判断是否在交互环境
来源：http://un.chemitech.net.cn

sys.stdout.isatty()
来源：http://qv.hahajie.cn

[U40] Py：打印到标准错误
来源：http://vx.newstarts.cn

print("err", file=sys.stderr)
来源：http://wc.gzmigu.cn

[U41] PHP：初始化 Composer 项目
来源：http://uk.huixiangedu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://cf.shxzskj.cn

[U42] PHP：PSR-4 自动加载
来源：http://jb.haigaiapp.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tc.szsharing.cn

[U43] PHP：声明命名空间
来源：http://xp.colortex.cn

namespace App\Http;
来源：http://ft.jctech888.com.cn

[U44] PHP：开启严格类型
来源：http://dp.hahajie.cn

declare(strict_types=1);
来源：http://zm.huanxung.cn

[U45] PHP：类型声明与返回类型
来源：http://gm.yuntaijiaju.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://rn.shtwfgs.cn

[U46] PHP：可空类型
来源：http://hz.jianghongdianzi.cn

?string $name = null
来源：http://rn.hahajie.cn

[U47] PHP：联合类型
来源：http://nl.9csxet.cn

int|string $id
来源：http://xx.yuntaijiaju.cn

[U48] PHP：纯枚举
来源：http://gl.shxzskj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sg.haigaiapp.cn

[U49] PHP：只读属性
来源：http://lb.nicolike.cn

public readonly string $name
来源：http://ll.yuexingan06.cn

[U50] PHP：构造器属性提升
来源：http://rs.huixiangedu.cn

public function __construct(private int $id) {}
来源：http://fe.muxihuayi.cn

[U51] PHP：数组解构
来源：http://yl.wgjwhj.cn

[$a, $b] = $arr;
来源：http://gu.colortex.cn

[U52] PHP：箭头函数
来源：http://go.shxzukj.cn

$double = fn($x) => $x * 2;
来源：http://hh.szsharing.cn

[U53] PHP：空合并运算符
来源：http://ez.nicolike.cn

$v = $a ?? $b ?? "default";
来源：http://wk.nicolike.cn

[U54] PHP：空安全调用
来源：http://ah.haigaiapp.cn

$obj?->method()
来源：http://hc.hahajie.cn

[U55] PHP：match 表达式
来源：http://kn.colortex.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://st.gzmigu.cn

[U56] PHP：命名参数
来源：http://yr.521024.cn

f(a: 1, b: 2)
来源：http://re.shtwfgs.cn

[U57] PHP：字符串插值
来源：http://ht.bookmarksfly.cn

"值: {$a}"
来源：http://nh.bookmarksfly.cn

[U58] PHP：数组三件套
来源：http://ba.bookmarksfly.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://oo.yuntaijiaju.cn

[U59] PHP：自定义排序
来源：http://hs.yuexingan06.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mi.huixiangedu.cn

[U60] PHP：JSON 编解码
来源：http://dr.panjiajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://il.hnjuh.cn

[U61] PHP：正则
来源：http://ei.huanxung.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jj.asd995.cn

[U62] PHP：日期对象
来源：http://xk.shxzukj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gv.szxytkj.cn

[U63] PHP：文件读写
来源：http://tx.hnjuh.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qc.bjjhwx.cn

[U64] PHP：目录遍历
来源：http://pg.hnjuh.cn

glob("dir/*.php");  scandir("dir");
来源：http://cq.huanxung.cn

[U65] PHP：会话
来源：http://pt.521024.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://gn.9csxet.cn

[U66] PHP：设置 Cookie
来源：http://ps.gzmigu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://oc.huanxung.cn

[U67] PHP：处理文件上传
来源：http://qy.jianghongdianzi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tn.szxytkj.cn

[U68] PHP：PDO 连接
来源：http://kq.jctech888.com.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ye.bjjhwx.cn

[U69] PHP：PDO 预处理
来源：http://ld.hahajie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jb.bookmarksfly.cn

[U70] PHP：PDO 事务
来源：http://wl.shxzukj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mj.bjjhwx.cn

[U71] PHP：抛出异常
来源：http://df.nszjky.cn

throw new RuntimeException("失败", 500);
来源：http://kw.huixiangedu.cn

[U72] PHP：写错误日志
来源：http://iq.521024.cn

error_log("失败: " . $e->getMessage());
来源：http://dm.szxytkj.cn

[U73] PHP：读取 ini 配置
来源：http://yi.panjiajie.cn

parse_ini_file("config.ini", true)
来源：http://qv.521024.cn

[U74] PHP：读取环境变量
来源：http://rb.shxzukj.cn

getenv("APP_ENV") ?: "production"
来源：http://gv.szxytkj.cn

[U75] PHP：依赖注入
来源：http://ed.muxihuayi.cn

composer require psr/container
来源：http://hx.szxytkj.cn

[U76] PHP：简单路由
来源：http://bz.yuexingan06.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ew.bookmarksfly.cn

[U77] PHP：模板渲染
来源：http://yw.huanxung.cn

composer require twig/twig
来源：http://bj.huixiangedu.cn

[U78] PHP：单元测试
来源：http://et.gzmigu.cn

composer require --dev phpunit/phpunit
来源：http://zw.521024.cn

[U79] PHP：静态分析
来源：http://mx.521024.cn

composer require --dev phpstan/phpstan
来源：http://bs.szxytkj.cn

[U80] PHP：代码规范修复
来源：http://fa.huanxung.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ka.hnjuh.cn

[U81] JS：初始化项目
来源：http://cx.huixiangedu.cn

npm init -y;  npm i express
来源：http://zh.hahajie.cn

[U82] JS：package.json 脚本
来源：http://cy.wgjwhj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ni.haigaiapp.cn

[U83] JS：ES Module 导入导出
来源：http://dp.nicolike.cn

export const a = 1;  import { a } from "./m.js";
来源：http://np.hahajie.cn

[U84] JS：CommonJS 写法
来源：http://bm.huixinmuqiang.cn

module.exports = { a };  const { a } = require("./m");
来源：http://az.shtwfgs.cn

[U85] JS：可选链
来源：http://yd.bookmarksfly.cn

a?.b?.c
来源：http://aa.jianghongdianzi.cn

[U86] JS：空值合并
来源：http://rr.muxihuayi.cn

a ?? b
来源：http://nx.nicolike.cn

[U87] JS：解构默认值
来源：http://cf.yuexingan06.cn

const { a = 1, b = 2 } = obj;
来源：http://sd.9csxet.cn

[U88] JS：对象展开合并
来源：http://rz.colortex.cn

{ ...a, ...b }
来源：http://eo.asd995.cn

[U89] JS：数组去重
来源：http://dd.chemitech.net.cn

[...new Set(arr)]
来源：http://no.wgjwhj.cn

[U90] JS：数字数组排序
来源：http://qa.szxytkj.cn

[...arr].sort((a, b) => a - b)
来源：http://bj.panjiajie.cn

[U91] JS：对象键值遍历
来源：http://ya.yuntaijiaju.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vz.lnxyls.cn

[U92] JS：深拷贝
来源：http://zd.muxihuayi.cn

structuredClone(obj)
来源：http://db.bookmarksfly.cn

[U93] JS：模板字符串
来源：http://jv.gzmigu.cn

`共 ${n} 条`
来源：http://ms.521024.cn

[U94] JS：箭头函数
来源：http://ux.bjjhwx.cn

const double = x => x * 2;
来源：http://rz.9csxet.cn


<!-- 参考信息 -->