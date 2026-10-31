代发 wailian999

[T13] Kotlin：只读 Map
来源：http://zh.asd995.cn

val m = mapOf("a" to 1)
来源：http://pm.haigaiapp.cn

[T14] Kotlin：循环
来源：http://ea.hahajie.cn

for (i in 1..10) println(i)
来源：http://sw.nszjky.cn

[T15] Kotlin：接口
来源：http://qw.jctech888.com.cn

interface Shape { fun area(): Double }
来源：http://qu.wgjwhj.cn

[T16] Swift：Hello World
来源：http://uz.panjiajie.cn

print("Hello")
来源：http://ge.huixiangedu.cn

[T17] Swift：变量与常量
来源：http://ug.bjjhwx.cn

var a = 1;  let b = 2
来源：http://de.szsharing.cn

[T18] Swift：字符串插值
来源：http://of.huixiangedu.cn

"值: \(b)"
来源：http://kp.szxytkj.cn

[T19] Swift：可选绑定
来源：http://ou.wgjwhj.cn

if let n = opt { print(n) }
来源：http://qu.hnjuh.cn

[T20] Swift：数组操作
来源：http://nt.newstarts.cn

var a = [1, 2, 3];  a.append(4)
来源：http://yt.panjiajie.cn

[T21] Swift：遍历
来源：http://uc.huanxung.cn

for x in a { print(x) }
来源：http://ms.chemitech.net.cn

[T22] Swift：字典
来源：http://jy.chemitech.net.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mz.nszjky.cn

[T23] Swift：函数
来源：http://pa.jianghongdianzi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dy.shtwfgs.cn

[T24] Swift：闭包
来源：http://nn.shxzskj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://hi.chemitech.net.cn

[T25] Swift：结构体
来源：http://kb.szsharing.cn

struct P { var x: Int }
来源：http://sw.yuexingan06.cn

[T26] Swift：类与重写
来源：http://ei.shtwfgs.cn

class A: Base { override func f() {} }
来源：http://bw.shxzukj.cn

[T27] Swift：错误处理
来源：http://bp.nszjky.cn

do { try f() } catch { print(error) }
来源：http://lo.szsharing.cn

[T28] Swift：枚举
来源：http://ot.asd995.cn

enum Color { case red, green }
来源：http://xx.newstarts.cn

[T29] Swift：guard 提前返回
来源：http://it.huixinmuqiang.cn

guard let x = opt else { return }
来源：http://tt.newstarts.cn

[T30] Swift：协议
来源：http://pr.nszjky.cn

protocol Shape { func area() -> Double }
来源：http://an.panjiajie.cn

[T31] Lua：Hello World
来源：http://ry.yuntaijiaju.cn

print("Hello")
来源：http://pu.panjiajie.cn

[T32] Lua：局部变量
来源：http://am.huanxung.cn

local a = 1
来源：http://is.jctech888.com.cn

[T33] Lua：表（数组）
来源：http://gf.521024.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://jt.wgjwhj.cn

[T34] Lua：遍历表
来源：http://so.szsharing.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://wk.szsharing.cn

[T35] Lua：字典表
来源：http://zy.chemitech.net.cn

local d = { a = 1 };  d.b = 2
来源：http://lj.chemitech.net.cn

[T36] Lua：函数
来源：http://mo.nszjky.cn

function add(a, b) return a + b end
来源：http://yb.9csxet.cn

[T37] Lua：字符串拼接
来源：http://ch.shtwfgs.cn

"a" .. "b"
来源：http://ft.jctech888.com.cn

[T38] Lua：条件
来源：http://lz.haigaiapp.cn

if x > 0 then print("正") end
来源：http://ke.gzmigu.cn

[T39] Lua：模式匹配
来源：http://jt.hnjuh.cn

string.find(s, "%d+")
来源：http://kz.jctech888.com.cn

[T40] Lua：元表
来源：http://kl.9csxet.cn

setmetatable({}, { __index = base })
来源：http://oj.asd995.cn

[T41] Perl：Hello World
来源：http://en.jctech888.com.cn

print "Hello\n";
来源：http://ab.lnxyls.cn

[T42] Perl：变量类型
来源：http://cw.szsharing.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yc.haigaiapp.cn

[T43] Perl：字符串插值
来源：http://iz.colortex.cn

"值: $a"
来源：http://lo.shxzukj.cn

[T44] Perl：条件
来源：http://ts.panjiajie.cn

if ($a > 0) { print "正"; }
来源：http://ku.nszjky.cn

[T45] Perl：数组遍历
来源：http://dx.colortex.cn

for my $x (@arr) { print $x; }
来源：http://xl.asd995.cn

[T46] Perl：哈希操作
来源：http://ze.nicolike.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://di.panjiajie.cn

[T47] Perl：正则捕获
来源：http://tq.9csxet.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ab.shtwfgs.cn

[T48] Perl：正则替换
来源：http://qj.yuexingan06.cn

$s =~ s/old/new/g;
来源：http://jh.nszjky.cn

[T49] Perl：函数
来源：http://gw.521024.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://un.bjjhwx.cn

[T50] Perl：逐行读文件
来源：http://iv.shxzskj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qd.shxzukj.cn

while (my $line = <$fh>) { print $line; }
来源：http://tl.shtwfgs.cn

[T51] Scala：Hello World
来源：http://bi.colortex.cn

println("Hello")
来源：http://hc.huanxung.cn

[T52] Scala：变量
来源：http://wq.newstarts.cn

val a = 1;  var b = 2
来源：http://pb.shxzskj.cn

[T53] Scala：字符串插值
来源：http://by.jctech888.com.cn

s"值: $b"
来源：http://eq.chemitech.net.cn

[T54] Scala：集合映射
来源：http://bh.shtwfgs.cn

List(1, 2, 3).map(_ * 2)
来源：http://xo.gzmigu.cn

[T55] Scala：集合过滤
来源：http://dg.yuexingan06.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qe.muxihuayi.cn

[T56] Scala：样例类
来源：http://nn.hahajie.cn

case class User(name: String, age: Int)
来源：http://wy.chemitech.net.cn

[T57] Scala：模式匹配
来源：http://yl.yuexingan06.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://cg.jianghongdianzi.cn

[T58] Scala：函数定义
来源：http://ky.yuexingan06.cn

def add(a: Int, b: Int): Int = a + b
来源：http://rr.hahajie.cn

[T59] Scala：循环
来源：http://mg.nicolike.cn

for (i <- 1 to 10) println(i)
来源：http://gp.wgjwhj.cn

[T60] Scala：折叠
来源：http://ln.nszjky.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://za.521024.cn

================================================================================
来源：http://ff.colortex.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yk.shxzukj.cn

================================================================================
来源：http://zq.nszjky.cn

[U01] Py：创建虚拟环境
来源：http://dn.nicolike.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cm.hahajie.cn

[U02] Py：导出 / 安装依赖
来源：http://ua.newstarts.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gn.chemitech.net.cn

[U03] Py：加载 .env 配置
来源：http://ph.gzmigu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://on.hahajie.cn

[U04] Py：变量调试打印
来源：http://jo.muxihuayi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xe.shtwfgs.cn

[U05] Py：列表去重且保序
来源：http://rd.huixiangedu.cn

list(dict.fromkeys(arr))
来源：http://fu.gzmigu.cn

[U06] Py：合并两个字典
来源：http://go.521024.cn

{**a, **b}
来源：http://an.huixiangedu.cn

[U07] Py：反转字典键值
来源：http://vl.shtwfgs.cn

{v: k for k, v in d.items()}
来源：http://xl.panjiajie.cn

[U08] Py：展平二维列表
来源：http://mi.newstarts.cn

[y for x in nested for y in x]
来源：http://dl.yuexingan06.cn

[U09] Py：字典取最大值的键
来源：http://ig.huanxung.cn

max(d, key=d.get)
来源：http://ky.haigaiapp.cn

[U10] Py：按值排序字典
来源：http://ma.bjjhwx.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kh.9csxet.cn

[U11] Py：生成器表达式
来源：http://hm.panjiajie.cn

(x * 2 for x in arr)
来源：http://cu.szxytkj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://bt.gzmigu.cn

Counter(arr).most_common(3)
来源：http://au.yuntaijiaju.cn

[U13] Py：固定长度队列
来源：http://zs.hnjuh.cn

deque(maxlen=10)
来源：http://qv.muxihuayi.cn

[U14] Py：分组收集到列表
来源：http://uj.asd995.cn

defaultdict(list)
来源：http://dg.yuntaijiaju.cn

[U15] Py：高精度计时
来源：http://at.9csxet.cn

t = time.perf_counter()
来源：http://qe.yuexingan06.cn

[U16] Py：命令行参数解析
来源：http://iw.bjjhwx.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://au.muxihuayi.cn

[U17] Py：初始化日志
来源：http://hr.nicolike.cn

logging.basicConfig(level=logging.INFO)
来源：http://gp.yuexingan06.cn

[U18] Py：预编译正则
来源：http://nt.panjiajie.cn

pat = re.compile(r"\d+")
来源：http://wc.huixinmuqiang.cn

[U19] Py：正则替换带回调
来源：http://ft.hahajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hc.haigaiapp.cn

[U20] Py：缓存函数结果
来源：http://fb.chemitech.net.cn

@functools.lru_cache(maxsize=None)
来源：http://qw.shxzukj.cn

[U21] Py：自定义上下文管理器
来源：http://tl.shxzukj.cn

@contextlib.contextmanager
来源：http://po.muxihuayi.cn

[U22] Py：矩阵转置
来源：http://kz.gzmigu.cn

list(zip(*m))
来源：http://hh.jianghongdianzi.cn

[U23] Py：分块读取大文件
来源：http://dv.huanxung.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mn.hahajie.cn

[U24] Py：路径操作
来源：http://il.nszjky.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wv.yuntaijiaju.cn

[U25] Py：CSV 按字典读
来源：http://ch.hahajie.cn

csv.DictReader(f)
来源：http://ny.lnxyls.cn

[U26] Py：并发下载
来源：http://dy.szxytkj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bz.gzmigu.cn

[U27] Py：异步 HTTP
来源：http://zf.szsharing.cn

aiohttp.ClientSession() 配合 async with
来源：http://jn.jctech888.com.cn

[U28] Py：类型别名
来源：http://ua.shtwfgs.cn

UserId = int
来源：http://ye.shxzukj.cn

[U29] Py：属性校验
来源：http://se.shtwfgs.cn

@property 与 @x.setter 配合
来源：http://zc.szsharing.cn

[U30] Py：数据类
来源：http://gw.jctech888.com.cn

@dataclass(slots=True)
来源：http://va.9csxet.cn

[U31] Py：单测
来源：http://ay.szsharing.cn

python -m pytest -q
来源：http://ns.szxytkj.cn

[U32] Py：代码格式化
来源：http://hs.muxihuayi.cn

ruff format . && ruff check --fix .
来源：http://kw.521024.cn

[U33] Py：打包发布
来源：http://bt.huixiangedu.cn

python -m build  （依赖 pyproject.toml）
来源：http://yy.yuntaijiaju.cn

[U34] Py：判断编码
来源：http://lr.9csxet.cn

chardet.detect(raw)
来源：http://iu.yuexingan06.cn

[U35] Py：发送邮件
来源：http://ln.haigaiapp.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xv.panjiajie.cn

[U36] Py：定时任务
来源：http://ec.yuntaijiaju.cn

schedule.every(10).minutes.do(job)
来源：http://tj.hnjuh.cn

[U37] Py：读写 Excel
来源：http://iq.hnjuh.cn

pandas.read_excel / DataFrame.to_excel
来源：http://of.muxihuayi.cn

[U38] Py：获取脚本所在目录
来源：http://ig.bookmarksfly.cn

Path(__file__).resolve().parent
来源：http://kv.panjiajie.cn

[U39] Py：判断是否在交互环境
来源：http://gz.colortex.cn

sys.stdout.isatty()
来源：http://de.nszjky.cn

[U40] Py：打印到标准错误
来源：http://pa.asd995.cn

print("err", file=sys.stderr)
来源：http://bi.wgjwhj.cn

[U41] PHP：初始化 Composer 项目
来源：http://ro.colortex.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xr.gzmigu.cn

[U42] PHP：PSR-4 自动加载
来源：http://kj.shxzukj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://la.huixinmuqiang.cn

[U43] PHP：声明命名空间
来源：http://cw.wgjwhj.cn

namespace App\Http;
来源：http://xb.szsharing.cn

[U44] PHP：开启严格类型
来源：http://mj.shtwfgs.cn

declare(strict_types=1);
来源：http://mx.shxzukj.cn

[U45] PHP：类型声明与返回类型
来源：http://ws.chemitech.net.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://wu.shxzskj.cn

[U46] PHP：可空类型
来源：http://pe.shxzskj.cn

?string $name = null
来源：http://ug.huanxung.cn

[U47] PHP：联合类型
来源：http://ec.shtwfgs.cn

int|string $id
来源：http://ot.newstarts.cn

[U48] PHP：纯枚举
来源：http://kx.szxytkj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nw.yuexingan06.cn

[U49] PHP：只读属性
来源：http://ja.shxzskj.cn

public readonly string $name
来源：http://nc.shxzukj.cn

[U50] PHP：构造器属性提升
来源：http://ku.hnjuh.cn

public function __construct(private int $id) {}
来源：http://xw.nicolike.cn

[U51] PHP：数组解构
来源：http://ht.newstarts.cn

[$a, $b] = $arr;
来源：http://bd.bookmarksfly.cn

[U52] PHP：箭头函数
来源：http://nb.shxzukj.cn

$double = fn($x) => $x * 2;
来源：http://ac.panjiajie.cn

[U53] PHP：空合并运算符
来源：http://uo.hnjuh.cn

$v = $a ?? $b ?? "default";
来源：http://vc.jianghongdianzi.cn

[U54] PHP：空安全调用
来源：http://gc.muxihuayi.cn

$obj?->method()
来源：http://dy.bjjhwx.cn

[U55] PHP：match 表达式
来源：http://te.chemitech.net.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zv.shxzukj.cn

[U56] PHP：命名参数
来源：http://wg.wgjwhj.cn

f(a: 1, b: 2)
来源：http://eo.nicolike.cn

[U57] PHP：字符串插值
来源：http://em.lnxyls.cn

"值: {$a}"
来源：http://sw.szsharing.cn

[U58] PHP：数组三件套
来源：http://tu.yuntaijiaju.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://eb.9csxet.cn

[U59] PHP：自定义排序
来源：http://ab.bookmarksfly.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ei.yuntaijiaju.cn

[U60] PHP：JSON 编解码
来源：http://wh.huanxung.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jy.asd995.cn

[U61] PHP：正则
来源：http://uy.muxihuayi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jf.yuexingan06.cn

[U62] PHP：日期对象
来源：http://km.lnxyls.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xe.asd995.cn

[U63] PHP：文件读写
来源：http://ny.hahajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mq.bookmarksfly.cn

[U64] PHP：目录遍历
来源：http://db.bjjhwx.cn

glob("dir/*.php");  scandir("dir");
来源：http://se.szxytkj.cn

[U65] PHP：会话
来源：http://xv.lnxyls.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://lz.huixinmuqiang.cn

[U66] PHP：设置 Cookie
来源：http://pi.shtwfgs.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ps.shxzukj.cn

[U67] PHP：处理文件上传
来源：http://af.yuexingan06.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mz.newstarts.cn

[U68] PHP：PDO 连接
来源：http://it.shtwfgs.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://je.panjiajie.cn

[U69] PHP：PDO 预处理
来源：http://ma.jctech888.com.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qi.shxzskj.cn

[U70] PHP：PDO 事务
来源：http://lo.colortex.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://up.colortex.cn

[U71] PHP：抛出异常
来源：http://uj.yuexingan06.cn

throw new RuntimeException("失败", 500);
来源：http://yb.muxihuayi.cn

[U72] PHP：写错误日志
来源：http://kg.shxzukj.cn

error_log("失败: " . $e->getMessage());
来源：http://hj.bjjhwx.cn

[U73] PHP：读取 ini 配置
来源：http://qq.jctech888.com.cn

parse_ini_file("config.ini", true)
来源：http://jl.szsharing.cn

[U74] PHP：读取环境变量
来源：http://va.bjjhwx.cn

getenv("APP_ENV") ?: "production"
来源：http://hu.huixiangedu.cn

[U75] PHP：依赖注入
来源：http://yi.9csxet.cn

composer require psr/container
来源：http://ag.nszjky.cn

[U76] PHP：简单路由
来源：http://sm.yuntaijiaju.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pp.shtwfgs.cn

[U77] PHP：模板渲染
来源：http://eo.panjiajie.cn

composer require twig/twig
来源：http://da.wgjwhj.cn

[U78] PHP：单元测试
来源：http://td.yuexingan06.cn

composer require --dev phpunit/phpunit
来源：http://sp.shxzskj.cn

[U79] PHP：静态分析
来源：http://mp.colortex.cn

composer require --dev phpstan/phpstan
来源：http://pd.yuexingan06.cn

[U80] PHP：代码规范修复
来源：http://hc.yuexingan06.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://gl.hnjuh.cn

[U81] JS：初始化项目
来源：http://bo.shxzskj.cn

npm init -y;  npm i express
来源：http://ps.jctech888.com.cn

[U82] JS：package.json 脚本
来源：http://rj.shtwfgs.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://on.shxzukj.cn

[U83] JS：ES Module 导入导出
来源：http://ce.newstarts.cn

export const a = 1;  import { a } from "./m.js";
来源：http://on.panjiajie.cn

[U84] JS：CommonJS 写法
来源：http://qm.521024.cn

module.exports = { a };  const { a } = require("./m");
来源：http://dl.yuexingan06.cn

[U85] JS：可选链
来源：http://po.haigaiapp.cn

a?.b?.c
来源：http://fi.huixiangedu.cn

[U86] JS：空值合并
来源：http://tb.chemitech.net.cn

a ?? b
来源：http://ew.newstarts.cn

[U87] JS：解构默认值
来源：http://ho.hnjuh.cn

const { a = 1, b = 2 } = obj;
来源：http://ek.wgjwhj.cn

[U88] JS：对象展开合并
来源：http://lo.haigaiapp.cn

{ ...a, ...b }
来源：http://ns.szxytkj.cn

[U89] JS：数组去重
来源：http://vi.huixinmuqiang.cn

[...new Set(arr)]
来源：http://ss.shxzskj.cn

[U90] JS：数字数组排序
来源：http://xb.muxihuayi.cn

[...arr].sort((a, b) => a - b)
来源：http://de.nszjky.cn

[U91] JS：对象键值遍历
来源：http://rr.nicolike.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jm.newstarts.cn

[U92] JS：深拷贝
来源：http://ax.gzmigu.cn

structuredClone(obj)
来源：http://dp.shxzukj.cn

[U93] JS：模板字符串
来源：http://zg.muxihuayi.cn

`共 ${n} 条`
来源：http://na.huixinmuqiang.cn

[U94] JS：箭头函数
来源：http://as.huanxung.cn

const double = x => x * 2;
来源：http://bk.chemitech.net.cn

[U95] JS：Promise 包装
来源：http://fw.panjiajie.cn

new Promise((resolve, reject) => {})
来源：http://om.521024.cn

[U96] JS：async/await 与异常
来源：http://fw.muxihuayi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zw.jctech888.com.cn

[U97] JS：并发请求
来源：http://ny.wgjwhj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://pc.nicolike.cn

[U98] JS：fetch 带 JSON
来源：http://wr.muxihuayi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ts.yuntaijiaju.cn

[U99] JS：事件监听
来源：http://xo.shxzskj.cn

el.addEventListener("click", e => {})
来源：http://ar.asd995.cn

[U100] JS：DOM 查询
来源：http://kx.szsharing.cn

document.querySelector(".item")
来源：http://wj.jianghongdianzi.cn


<!-- 参考信息 -->