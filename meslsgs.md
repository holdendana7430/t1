代发 wailian999

[T11] Kotlin：协程
来源：http://dx.haigaiapp.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hw.hahajie.cn

[T12] Kotlin：解构声明
来源：http://mi.newstarts.cn

val (a, b) = Pair(1, 2)
来源：http://xv.wgjwhj.cn

[T13] Kotlin：只读 Map
来源：http://eq.521024.cn

val m = mapOf("a" to 1)
来源：http://rl.hnjuh.cn

[T14] Kotlin：循环
来源：http://zz.521024.cn

for (i in 1..10) println(i)
来源：http://ib.shxzskj.cn

[T15] Kotlin：接口
来源：http://ff.haigaiapp.cn

interface Shape { fun area(): Double }
来源：http://yt.bjjhwx.cn

[T16] Swift：Hello World
来源：http://ap.szsharing.cn

print("Hello")
来源：http://ai.newstarts.cn

[T17] Swift：变量与常量
来源：http://yr.jianghongdianzi.cn

var a = 1;  let b = 2
来源：http://sa.szsharing.cn

[T18] Swift：字符串插值
来源：http://jl.jctech888.com.cn

"值: \(b)"
来源：http://sr.521024.cn

[T19] Swift：可选绑定
来源：http://ca.haigaiapp.cn

if let n = opt { print(n) }
来源：http://rd.lnxyls.cn

[T20] Swift：数组操作
来源：http://uh.huixinmuqiang.cn

var a = [1, 2, 3];  a.append(4)
来源：http://rq.521024.cn

[T21] Swift：遍历
来源：http://et.9csxet.cn

for x in a { print(x) }
来源：http://np.hnjuh.cn

[T22] Swift：字典
来源：http://is.asd995.cn

var d = ["a": 1];  d["b"] = 2
来源：http://hl.wgjwhj.cn

[T23] Swift：函数
来源：http://ai.huixiangedu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gz.gzmigu.cn

[T24] Swift：闭包
来源：http://xp.shtwfgs.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://oe.yuexingan06.cn

[T25] Swift：结构体
来源：http://oc.bjjhwx.cn

struct P { var x: Int }
来源：http://mj.huixiangedu.cn

[T26] Swift：类与重写
来源：http://vr.shxzukj.cn

class A: Base { override func f() {} }
来源：http://zm.muxihuayi.cn

[T27] Swift：错误处理
来源：http://rh.panjiajie.cn

do { try f() } catch { print(error) }
来源：http://sf.haigaiapp.cn

[T28] Swift：枚举
来源：http://zq.nszjky.cn

enum Color { case red, green }
来源：http://rm.9csxet.cn

[T29] Swift：guard 提前返回
来源：http://cy.huixiangedu.cn

guard let x = opt else { return }
来源：http://xq.hahajie.cn

[T30] Swift：协议
来源：http://hz.colortex.cn

protocol Shape { func area() -> Double }
来源：http://fo.gzmigu.cn

[T31] Lua：Hello World
来源：http://ui.szsharing.cn

print("Hello")
来源：http://ul.shtwfgs.cn

[T32] Lua：局部变量
来源：http://en.newstarts.cn

local a = 1
来源：http://bl.jianghongdianzi.cn

[T33] Lua：表（数组）
来源：http://vb.wgjwhj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://by.colortex.cn

[T34] Lua：遍历表
来源：http://yx.nicolike.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://kf.yuntaijiaju.cn

[T35] Lua：字典表
来源：http://ff.huixiangedu.cn

local d = { a = 1 };  d.b = 2
来源：http://gk.huixiangedu.cn

[T36] Lua：函数
来源：http://rl.jianghongdianzi.cn

function add(a, b) return a + b end
来源：http://jp.colortex.cn

[T37] Lua：字符串拼接
来源：http://sz.wgjwhj.cn

"a" .. "b"
来源：http://ai.huixiangedu.cn

[T38] Lua：条件
来源：http://mh.szsharing.cn

if x > 0 then print("正") end
来源：http://xo.shxzukj.cn

[T39] Lua：模式匹配
来源：http://cj.newstarts.cn

string.find(s, "%d+")
来源：http://kt.jctech888.com.cn

[T40] Lua：元表
来源：http://io.szsharing.cn

setmetatable({}, { __index = base })
来源：http://iz.521024.cn

[T41] Perl：Hello World
来源：http://vu.huanxung.cn

print "Hello\n";
来源：http://aw.nszjky.cn

[T42] Perl：变量类型
来源：http://xm.huanxung.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://aa.chemitech.net.cn

[T43] Perl：字符串插值
来源：http://lp.szsharing.cn

"值: $a"
来源：http://li.bjjhwx.cn

[T44] Perl：条件
来源：http://pg.hahajie.cn

if ($a > 0) { print "正"; }
来源：http://ll.nicolike.cn

[T45] Perl：数组遍历
来源：http://qf.lnxyls.cn

for my $x (@arr) { print $x; }
来源：http://sb.shtwfgs.cn

[T46] Perl：哈希操作
来源：http://nw.9csxet.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vd.muxihuayi.cn

[T47] Perl：正则捕获
来源：http://dk.nicolike.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://bz.shxzskj.cn

[T48] Perl：正则替换
来源：http://nz.huanxung.cn

$s =~ s/old/new/g;
来源：http://rh.gzmigu.cn

[T49] Perl：函数
来源：http://dn.gzmigu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fb.colortex.cn

[T50] Perl：逐行读文件
来源：http://qq.jctech888.com.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rt.colortex.cn

while (my $line = <$fh>) { print $line; }
来源：http://fp.huixiangedu.cn

[T51] Scala：Hello World
来源：http://jw.hahajie.cn

println("Hello")
来源：http://er.muxihuayi.cn

[T52] Scala：变量
来源：http://ks.szsharing.cn

val a = 1;  var b = 2
来源：http://dq.huixinmuqiang.cn

[T53] Scala：字符串插值
来源：http://tc.jctech888.com.cn

s"值: $b"
来源：http://am.hahajie.cn

[T54] Scala：集合映射
来源：http://se.muxihuayi.cn

List(1, 2, 3).map(_ * 2)
来源：http://fq.szsharing.cn

[T55] Scala：集合过滤
来源：http://ns.shtwfgs.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ph.newstarts.cn

[T56] Scala：样例类
来源：http://gq.bookmarksfly.cn

case class User(name: String, age: Int)
来源：http://wh.szxytkj.cn

[T57] Scala：模式匹配
来源：http://ry.9csxet.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://kk.lnxyls.cn

[T58] Scala：函数定义
来源：http://xa.yuntaijiaju.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fb.haigaiapp.cn

[T59] Scala：循环
来源：http://hv.haigaiapp.cn

for (i <- 1 to 10) println(i)
来源：http://cs.shxzskj.cn

[T60] Scala：折叠
来源：http://ne.nszjky.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ma.9csxet.cn

================================================================================
来源：http://ib.wgjwhj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vc.chemitech.net.cn

================================================================================
来源：http://fb.szxytkj.cn

[U01] Py：创建虚拟环境
来源：http://lv.lnxyls.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bd.huixiangedu.cn

[U02] Py：导出 / 安装依赖
来源：http://yg.yuntaijiaju.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cp.shxzukj.cn

[U03] Py：加载 .env 配置
来源：http://ot.9csxet.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://cf.szxytkj.cn

[U04] Py：变量调试打印
来源：http://cf.yuexingan06.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pt.panjiajie.cn

[U05] Py：列表去重且保序
来源：http://qy.shtwfgs.cn

list(dict.fromkeys(arr))
来源：http://jx.nszjky.cn

[U06] Py：合并两个字典
来源：http://zg.haigaiapp.cn

{**a, **b}
来源：http://gp.bjjhwx.cn

[U07] Py：反转字典键值
来源：http://sh.yuntaijiaju.cn

{v: k for k, v in d.items()}
来源：http://bl.asd995.cn

[U08] Py：展平二维列表
来源：http://da.asd995.cn

[y for x in nested for y in x]
来源：http://qb.haigaiapp.cn

[U09] Py：字典取最大值的键
来源：http://vw.nicolike.cn

max(d, key=d.get)
来源：http://dc.shxzukj.cn

[U10] Py：按值排序字典
来源：http://pm.newstarts.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://oj.yuntaijiaju.cn

[U11] Py：生成器表达式
来源：http://xd.lnxyls.cn

(x * 2 for x in arr)
来源：http://qt.jianghongdianzi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://np.jianghongdianzi.cn

Counter(arr).most_common(3)
来源：http://nn.shxzukj.cn

[U13] Py：固定长度队列
来源：http://qn.chemitech.net.cn

deque(maxlen=10)
来源：http://nu.wgjwhj.cn

[U14] Py：分组收集到列表
来源：http://md.shxzskj.cn

defaultdict(list)
来源：http://fq.jctech888.com.cn

[U15] Py：高精度计时
来源：http://ek.muxihuayi.cn

t = time.perf_counter()
来源：http://uu.muxihuayi.cn

[U16] Py：命令行参数解析
来源：http://oi.gzmigu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://el.huanxung.cn

[U17] Py：初始化日志
来源：http://xj.chemitech.net.cn

logging.basicConfig(level=logging.INFO)
来源：http://gq.yuexingan06.cn

[U18] Py：预编译正则
来源：http://vq.bjjhwx.cn

pat = re.compile(r"\d+")
来源：http://vg.nszjky.cn

[U19] Py：正则替换带回调
来源：http://lo.jianghongdianzi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ay.asd995.cn

[U20] Py：缓存函数结果
来源：http://zh.yuntaijiaju.cn

@functools.lru_cache(maxsize=None)
来源：http://qx.szsharing.cn

[U21] Py：自定义上下文管理器
来源：http://hi.colortex.cn

@contextlib.contextmanager
来源：http://bg.lnxyls.cn

[U22] Py：矩阵转置
来源：http://og.9csxet.cn

list(zip(*m))
来源：http://ff.nicolike.cn

[U23] Py：分块读取大文件
来源：http://qz.huixinmuqiang.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mg.lnxyls.cn

[U24] Py：路径操作
来源：http://gt.muxihuayi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kh.huixiangedu.cn

[U25] Py：CSV 按字典读
来源：http://vm.chemitech.net.cn

csv.DictReader(f)
来源：http://ut.shxzskj.cn

[U26] Py：并发下载
来源：http://mz.newstarts.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bh.hahajie.cn

[U27] Py：异步 HTTP
来源：http://ia.chemitech.net.cn

aiohttp.ClientSession() 配合 async with
来源：http://zx.yuexingan06.cn

[U28] Py：类型别名
来源：http://th.nicolike.cn

UserId = int
来源：http://ki.bjjhwx.cn

[U29] Py：属性校验
来源：http://hl.wgjwhj.cn

@property 与 @x.setter 配合
来源：http://mp.haigaiapp.cn

[U30] Py：数据类
来源：http://yu.yuexingan06.cn

@dataclass(slots=True)
来源：http://nv.yuexingan06.cn

[U31] Py：单测
来源：http://jz.9csxet.cn

python -m pytest -q
来源：http://gi.bookmarksfly.cn

[U32] Py：代码格式化
来源：http://pa.muxihuayi.cn

ruff format . && ruff check --fix .
来源：http://cs.521024.cn

[U33] Py：打包发布
来源：http://mx.hnjuh.cn

python -m build  （依赖 pyproject.toml）
来源：http://xa.shxzskj.cn

[U34] Py：判断编码
来源：http://gf.9csxet.cn

chardet.detect(raw)
来源：http://ac.shxzukj.cn

[U35] Py：发送邮件
来源：http://qa.szxytkj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kd.huixiangedu.cn

[U36] Py：定时任务
来源：http://xy.colortex.cn

schedule.every(10).minutes.do(job)
来源：http://gb.shxzskj.cn

[U37] Py：读写 Excel
来源：http://xs.szsharing.cn

pandas.read_excel / DataFrame.to_excel
来源：http://xw.huanxung.cn

[U38] Py：获取脚本所在目录
来源：http://xj.asd995.cn

Path(__file__).resolve().parent
来源：http://xf.nicolike.cn

[U39] Py：判断是否在交互环境
来源：http://hm.jctech888.com.cn

sys.stdout.isatty()
来源：http://qk.szxytkj.cn

[U40] Py：打印到标准错误
来源：http://lq.szxytkj.cn

print("err", file=sys.stderr)
来源：http://ok.jianghongdianzi.cn

[U41] PHP：初始化 Composer 项目
来源：http://ae.chemitech.net.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://da.shxzskj.cn

[U42] PHP：PSR-4 自动加载
来源：http://au.szxytkj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cv.hahajie.cn

[U43] PHP：声明命名空间
来源：http://jw.jianghongdianzi.cn

namespace App\Http;
来源：http://hj.bjjhwx.cn

[U44] PHP：开启严格类型
来源：http://yr.lnxyls.cn

declare(strict_types=1);
来源：http://fz.hahajie.cn

[U45] PHP：类型声明与返回类型
来源：http://hx.jctech888.com.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qc.haigaiapp.cn

[U46] PHP：可空类型
来源：http://ai.9csxet.cn

?string $name = null
来源：http://jt.hahajie.cn

[U47] PHP：联合类型
来源：http://gr.lnxyls.cn

int|string $id
来源：http://gb.szxytkj.cn

[U48] PHP：纯枚举
来源：http://ij.szxytkj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://he.lnxyls.cn

[U49] PHP：只读属性
来源：http://nv.huixinmuqiang.cn

public readonly string $name
来源：http://kb.haigaiapp.cn

[U50] PHP：构造器属性提升
来源：http://dy.szsharing.cn

public function __construct(private int $id) {}
来源：http://kt.gzmigu.cn

[U51] PHP：数组解构
来源：http://lh.chemitech.net.cn

[$a, $b] = $arr;
来源：http://dq.yuexingan06.cn

[U52] PHP：箭头函数
来源：http://cw.jianghongdianzi.cn

$double = fn($x) => $x * 2;
来源：http://zv.shtwfgs.cn

[U53] PHP：空合并运算符
来源：http://mw.yuexingan06.cn

$v = $a ?? $b ?? "default";
来源：http://nq.bjjhwx.cn

[U54] PHP：空安全调用
来源：http://re.chemitech.net.cn

$obj?->method()
来源：http://ws.bookmarksfly.cn

[U55] PHP：match 表达式
来源：http://ym.yuntaijiaju.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ro.shxzukj.cn

[U56] PHP：命名参数
来源：http://kl.huixiangedu.cn

f(a: 1, b: 2)
来源：http://tj.newstarts.cn

[U57] PHP：字符串插值
来源：http://dk.szsharing.cn

"值: {$a}"
来源：http://cl.521024.cn

[U58] PHP：数组三件套
来源：http://zo.gzmigu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tz.521024.cn

[U59] PHP：自定义排序
来源：http://wj.asd995.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://is.9csxet.cn

[U60] PHP：JSON 编解码
来源：http://cq.chemitech.net.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bg.huixinmuqiang.cn

[U61] PHP：正则
来源：http://by.jctech888.com.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qi.521024.cn

[U62] PHP：日期对象
来源：http://ug.yuexingan06.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ma.bookmarksfly.cn

[U63] PHP：文件读写
来源：http://kd.nicolike.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vs.bjjhwx.cn

[U64] PHP：目录遍历
来源：http://wc.shxzukj.cn

glob("dir/*.php");  scandir("dir");
来源：http://of.chemitech.net.cn

[U65] PHP：会话
来源：http://ex.shtwfgs.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ye.hahajie.cn

[U66] PHP：设置 Cookie
来源：http://rk.chemitech.net.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://es.huixinmuqiang.cn

[U67] PHP：处理文件上传
来源：http://ec.szxytkj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dg.jianghongdianzi.cn

[U68] PHP：PDO 连接
来源：http://tj.hnjuh.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ny.nicolike.cn

[U69] PHP：PDO 预处理
来源：http://hi.yuntaijiaju.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tl.szsharing.cn

[U70] PHP：PDO 事务
来源：http://xc.colortex.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bb.hnjuh.cn

[U71] PHP：抛出异常
来源：http://fp.huixiangedu.cn

throw new RuntimeException("失败", 500);
来源：http://vy.newstarts.cn

[U72] PHP：写错误日志
来源：http://yc.szsharing.cn

error_log("失败: " . $e->getMessage());
来源：http://kp.gzmigu.cn

[U73] PHP：读取 ini 配置
来源：http://ki.bjjhwx.cn

parse_ini_file("config.ini", true)
来源：http://kj.huixinmuqiang.cn

[U74] PHP：读取环境变量
来源：http://gk.huixinmuqiang.cn

getenv("APP_ENV") ?: "production"
来源：http://sm.wgjwhj.cn

[U75] PHP：依赖注入
来源：http://co.jctech888.com.cn

composer require psr/container
来源：http://wh.panjiajie.cn

[U76] PHP：简单路由
来源：http://lb.gzmigu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dg.yuntaijiaju.cn

[U77] PHP：模板渲染
来源：http://ro.panjiajie.cn

composer require twig/twig
来源：http://sc.521024.cn

[U78] PHP：单元测试
来源：http://ld.jianghongdianzi.cn

composer require --dev phpunit/phpunit
来源：http://ph.huixiangedu.cn

[U79] PHP：静态分析
来源：http://my.hnjuh.cn

composer require --dev phpstan/phpstan
来源：http://co.nicolike.cn

[U80] PHP：代码规范修复
来源：http://hl.hnjuh.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://pd.shtwfgs.cn

[U81] JS：初始化项目
来源：http://ib.chemitech.net.cn

npm init -y;  npm i express
来源：http://iw.newstarts.cn

[U82] JS：package.json 脚本
来源：http://gl.bjjhwx.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cv.9csxet.cn

[U83] JS：ES Module 导入导出
来源：http://mw.wgjwhj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://wx.lnxyls.cn

[U84] JS：CommonJS 写法
来源：http://ny.hahajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ud.panjiajie.cn

[U85] JS：可选链
来源：http://jg.gzmigu.cn

a?.b?.c
来源：http://di.asd995.cn

[U86] JS：空值合并
来源：http://ug.newstarts.cn

a ?? b
来源：http://bl.muxihuayi.cn

[U87] JS：解构默认值
来源：http://uu.bjjhwx.cn

const { a = 1, b = 2 } = obj;
来源：http://wr.newstarts.cn

[U88] JS：对象展开合并
来源：http://eh.shtwfgs.cn

{ ...a, ...b }
来源：http://cs.huixiangedu.cn

[U89] JS：数组去重
来源：http://yx.yuexingan06.cn

[...new Set(arr)]
来源：http://hr.521024.cn

[U90] JS：数字数组排序
来源：http://xo.bjjhwx.cn

[...arr].sort((a, b) => a - b)
来源：http://wa.huixiangedu.cn

[U91] JS：对象键值遍历
来源：http://zf.yuntaijiaju.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kl.wgjwhj.cn

[U92] JS：深拷贝
来源：http://sn.bjjhwx.cn

structuredClone(obj)
来源：http://ei.nszjky.cn

[U93] JS：模板字符串
来源：http://kh.panjiajie.cn

`共 ${n} 条`
来源：http://ig.9csxet.cn

[U94] JS：箭头函数
来源：http://im.jctech888.com.cn

const double = x => x * 2;
来源：http://ej.lnxyls.cn

[U95] JS：Promise 包装
来源：http://jh.chemitech.net.cn

new Promise((resolve, reject) => {})
来源：http://ej.wgjwhj.cn

[U96] JS：async/await 与异常
来源：http://bm.jianghongdianzi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://de.wgjwhj.cn

[U97] JS：并发请求
来源：http://nr.szsharing.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://sk.jianghongdianzi.cn

[U98] JS：fetch 带 JSON
来源：http://fl.bjjhwx.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://je.lnxyls.cn


<!-- 参考信息 -->