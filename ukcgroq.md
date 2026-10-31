代发 wailian999

[T11] Kotlin：协程
来源：http://zi.gzmigu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ag.yuexingan06.cn

[T12] Kotlin：解构声明
来源：http://dg.yuexingan06.cn

val (a, b) = Pair(1, 2)
来源：http://fk.panjiajie.cn

[T13] Kotlin：只读 Map
来源：http://ec.yuntaijiaju.cn

val m = mapOf("a" to 1)
来源：http://tf.jctech888.com.cn

[T14] Kotlin：循环
来源：http://iq.colortex.cn

for (i in 1..10) println(i)
来源：http://pu.yuexingan06.cn

[T15] Kotlin：接口
来源：http://qg.chemitech.net.cn

interface Shape { fun area(): Double }
来源：http://ny.hnjuh.cn

[T16] Swift：Hello World
来源：http://xi.asd995.cn

print("Hello")
来源：http://uy.colortex.cn

[T17] Swift：变量与常量
来源：http://ba.huixiangedu.cn

var a = 1;  let b = 2
来源：http://km.hahajie.cn

[T18] Swift：字符串插值
来源：http://eh.haigaiapp.cn

"值: \(b)"
来源：http://fh.hnjuh.cn

[T19] Swift：可选绑定
来源：http://lj.shxzukj.cn

if let n = opt { print(n) }
来源：http://wb.lnxyls.cn

[T20] Swift：数组操作
来源：http://ye.szxytkj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://nv.gzmigu.cn

[T21] Swift：遍历
来源：http://me.huixinmuqiang.cn

for x in a { print(x) }
来源：http://ri.bjjhwx.cn

[T22] Swift：字典
来源：http://vf.huanxung.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fu.newstarts.cn

[T23] Swift：函数
来源：http://bt.asd995.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dw.huanxung.cn

[T24] Swift：闭包
来源：http://xz.jianghongdianzi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://oe.nicolike.cn

[T25] Swift：结构体
来源：http://pw.hahajie.cn

struct P { var x: Int }
来源：http://qh.hahajie.cn

[T26] Swift：类与重写
来源：http://pp.jianghongdianzi.cn

class A: Base { override func f() {} }
来源：http://nl.hahajie.cn

[T27] Swift：错误处理
来源：http://hh.newstarts.cn

do { try f() } catch { print(error) }
来源：http://ow.yuntaijiaju.cn

[T28] Swift：枚举
来源：http://cm.haigaiapp.cn

enum Color { case red, green }
来源：http://dt.521024.cn

[T29] Swift：guard 提前返回
来源：http://mt.shxzskj.cn

guard let x = opt else { return }
来源：http://nf.wgjwhj.cn

[T30] Swift：协议
来源：http://gw.nicolike.cn

protocol Shape { func area() -> Double }
来源：http://yu.bookmarksfly.cn

[T31] Lua：Hello World
来源：http://fr.huanxung.cn

print("Hello")
来源：http://zj.colortex.cn

[T32] Lua：局部变量
来源：http://pc.gzmigu.cn

local a = 1
来源：http://ia.panjiajie.cn

[T33] Lua：表（数组）
来源：http://gl.huanxung.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ql.huixiangedu.cn

[T34] Lua：遍历表
来源：http://pb.newstarts.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ik.gzmigu.cn

[T35] Lua：字典表
来源：http://cx.9csxet.cn

local d = { a = 1 };  d.b = 2
来源：http://uc.jianghongdianzi.cn

[T36] Lua：函数
来源：http://qa.szxytkj.cn

function add(a, b) return a + b end
来源：http://ge.huixinmuqiang.cn

[T37] Lua：字符串拼接
来源：http://nb.szsharing.cn

"a" .. "b"
来源：http://xw.hnjuh.cn

[T38] Lua：条件
来源：http://xe.hahajie.cn

if x > 0 then print("正") end
来源：http://bl.shxzskj.cn

[T39] Lua：模式匹配
来源：http://rc.yuexingan06.cn

string.find(s, "%d+")
来源：http://cp.hnjuh.cn

[T40] Lua：元表
来源：http://mw.shxzskj.cn

setmetatable({}, { __index = base })
来源：http://ar.hnjuh.cn

[T41] Perl：Hello World
来源：http://dk.huixinmuqiang.cn

print "Hello\n";
来源：http://dm.jctech888.com.cn

[T42] Perl：变量类型
来源：http://jn.panjiajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://am.jianghongdianzi.cn

[T43] Perl：字符串插值
来源：http://bz.nszjky.cn

"值: $a"
来源：http://hv.muxihuayi.cn

[T44] Perl：条件
来源：http://tz.nicolike.cn

if ($a > 0) { print "正"; }
来源：http://cr.chemitech.net.cn

[T45] Perl：数组遍历
来源：http://nb.haigaiapp.cn

for my $x (@arr) { print $x; }
来源：http://sa.szsharing.cn

[T46] Perl：哈希操作
来源：http://gx.panjiajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tv.hnjuh.cn

[T47] Perl：正则捕获
来源：http://ej.shxzukj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://id.shxzukj.cn

[T48] Perl：正则替换
来源：http://fv.szxytkj.cn

$s =~ s/old/new/g;
来源：http://wa.shxzskj.cn

[T49] Perl：函数
来源：http://nf.panjiajie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bn.nicolike.cn

[T50] Perl：逐行读文件
来源：http://ox.asd995.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qj.lnxyls.cn

while (my $line = <$fh>) { print $line; }
来源：http://el.jctech888.com.cn

[T51] Scala：Hello World
来源：http://nf.jianghongdianzi.cn

println("Hello")
来源：http://cw.asd995.cn

[T52] Scala：变量
来源：http://op.shxzukj.cn

val a = 1;  var b = 2
来源：http://ic.jianghongdianzi.cn

[T53] Scala：字符串插值
来源：http://hf.jctech888.com.cn

s"值: $b"
来源：http://vp.chemitech.net.cn

[T54] Scala：集合映射
来源：http://le.huanxung.cn

List(1, 2, 3).map(_ * 2)
来源：http://xq.nszjky.cn

[T55] Scala：集合过滤
来源：http://xg.bjjhwx.cn

List(1, 2, 3).filter(_ > 1)
来源：http://jb.hahajie.cn

[T56] Scala：样例类
来源：http://vo.muxihuayi.cn

case class User(name: String, age: Int)
来源：http://eq.yuexingan06.cn

[T57] Scala：模式匹配
来源：http://ju.muxihuayi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gb.bookmarksfly.cn

[T58] Scala：函数定义
来源：http://sy.newstarts.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ky.shxzskj.cn

[T59] Scala：循环
来源：http://om.shxzukj.cn

for (i <- 1 to 10) println(i)
来源：http://zv.huixiangedu.cn

[T60] Scala：折叠
来源：http://qg.szsharing.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yn.nicolike.cn

================================================================================
来源：http://as.shxzukj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wr.bjjhwx.cn

================================================================================
来源：http://xr.lnxyls.cn

[U01] Py：创建虚拟环境
来源：http://iy.szsharing.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ck.nszjky.cn

[U02] Py：导出 / 安装依赖
来源：http://jf.shxzskj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qv.nszjky.cn

[U03] Py：加载 .env 配置
来源：http://qc.lnxyls.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://hj.huixiangedu.cn

[U04] Py：变量调试打印
来源：http://ch.521024.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fn.szxytkj.cn

[U05] Py：列表去重且保序
来源：http://iz.shtwfgs.cn

list(dict.fromkeys(arr))
来源：http://zc.jctech888.com.cn

[U06] Py：合并两个字典
来源：http://qq.asd995.cn

{**a, **b}
来源：http://ry.nicolike.cn

[U07] Py：反转字典键值
来源：http://xu.yuexingan06.cn

{v: k for k, v in d.items()}
来源：http://ho.hahajie.cn

[U08] Py：展平二维列表
来源：http://xb.colortex.cn

[y for x in nested for y in x]
来源：http://le.haigaiapp.cn

[U09] Py：字典取最大值的键
来源：http://wx.chemitech.net.cn

max(d, key=d.get)
来源：http://lo.haigaiapp.cn

[U10] Py：按值排序字典
来源：http://tg.521024.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yc.521024.cn

[U11] Py：生成器表达式
来源：http://wk.newstarts.cn

(x * 2 for x in arr)
来源：http://se.9csxet.cn

[U12] Py：取出现最多的 3 个元素
来源：http://hp.jianghongdianzi.cn

Counter(arr).most_common(3)
来源：http://ra.chemitech.net.cn

[U13] Py：固定长度队列
来源：http://qn.shxzskj.cn

deque(maxlen=10)
来源：http://cr.lnxyls.cn

[U14] Py：分组收集到列表
来源：http://ty.panjiajie.cn

defaultdict(list)
来源：http://ad.szsharing.cn

[U15] Py：高精度计时
来源：http://pm.newstarts.cn

t = time.perf_counter()
来源：http://qg.haigaiapp.cn

[U16] Py：命令行参数解析
来源：http://nl.lnxyls.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ai.shxzskj.cn

[U17] Py：初始化日志
来源：http://aq.nszjky.cn

logging.basicConfig(level=logging.INFO)
来源：http://eq.bookmarksfly.cn

[U18] Py：预编译正则
来源：http://rx.panjiajie.cn

pat = re.compile(r"\d+")
来源：http://la.huixinmuqiang.cn

[U19] Py：正则替换带回调
来源：http://sm.shxzukj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pk.colortex.cn

[U20] Py：缓存函数结果
来源：http://sm.huixinmuqiang.cn

@functools.lru_cache(maxsize=None)
来源：http://il.szsharing.cn

[U21] Py：自定义上下文管理器
来源：http://gi.bjjhwx.cn

@contextlib.contextmanager
来源：http://du.yuntaijiaju.cn

[U22] Py：矩阵转置
来源：http://eb.huanxung.cn

list(zip(*m))
来源：http://ck.gzmigu.cn

[U23] Py：分块读取大文件
来源：http://pk.colortex.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ya.szsharing.cn

[U24] Py：路径操作
来源：http://ly.chemitech.net.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lu.huanxung.cn

[U25] Py：CSV 按字典读
来源：http://bq.hahajie.cn

csv.DictReader(f)
来源：http://qb.521024.cn

[U26] Py：并发下载
来源：http://xu.chemitech.net.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mz.shxzukj.cn

[U27] Py：异步 HTTP
来源：http://se.lnxyls.cn

aiohttp.ClientSession() 配合 async with
来源：http://xx.shxzskj.cn

[U28] Py：类型别名
来源：http://rb.gzmigu.cn

UserId = int
来源：http://qj.jctech888.com.cn

[U29] Py：属性校验
来源：http://es.huixiangedu.cn

@property 与 @x.setter 配合
来源：http://hs.yuntaijiaju.cn

[U30] Py：数据类
来源：http://pg.haigaiapp.cn

@dataclass(slots=True)
来源：http://fg.newstarts.cn

[U31] Py：单测
来源：http://zi.huanxung.cn

python -m pytest -q
来源：http://dg.shxzukj.cn

[U32] Py：代码格式化
来源：http://dx.asd995.cn

ruff format . && ruff check --fix .
来源：http://of.shxzskj.cn

[U33] Py：打包发布
来源：http://oi.hahajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://qg.szsharing.cn

[U34] Py：判断编码
来源：http://nz.lnxyls.cn

chardet.detect(raw)
来源：http://or.haigaiapp.cn

[U35] Py：发送邮件
来源：http://ie.wgjwhj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mi.asd995.cn

[U36] Py：定时任务
来源：http://tl.asd995.cn

schedule.every(10).minutes.do(job)
来源：http://qg.yuexingan06.cn

[U37] Py：读写 Excel
来源：http://kh.asd995.cn

pandas.read_excel / DataFrame.to_excel
来源：http://uj.hnjuh.cn

[U38] Py：获取脚本所在目录
来源：http://mn.szsharing.cn

Path(__file__).resolve().parent
来源：http://xv.nszjky.cn

[U39] Py：判断是否在交互环境
来源：http://go.huixiangedu.cn

sys.stdout.isatty()
来源：http://jj.haigaiapp.cn

[U40] Py：打印到标准错误
来源：http://ww.muxihuayi.cn

print("err", file=sys.stderr)
来源：http://ka.bookmarksfly.cn

[U41] PHP：初始化 Composer 项目
来源：http://rd.muxihuayi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://af.521024.cn

[U42] PHP：PSR-4 自动加载
来源：http://en.szxytkj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://up.nszjky.cn

[U43] PHP：声明命名空间
来源：http://zh.hahajie.cn

namespace App\Http;
来源：http://rd.szxytkj.cn

[U44] PHP：开启严格类型
来源：http://cc.huanxung.cn

declare(strict_types=1);
来源：http://yv.colortex.cn

[U45] PHP：类型声明与返回类型
来源：http://qp.wgjwhj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jd.szxytkj.cn

[U46] PHP：可空类型
来源：http://me.szsharing.cn

?string $name = null
来源：http://es.shxzskj.cn

[U47] PHP：联合类型
来源：http://yp.jctech888.com.cn

int|string $id
来源：http://jd.521024.cn

[U48] PHP：纯枚举
来源：http://tl.shtwfgs.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ra.shxzskj.cn

[U49] PHP：只读属性
来源：http://rg.bookmarksfly.cn

public readonly string $name
来源：http://mt.jianghongdianzi.cn

[U50] PHP：构造器属性提升
来源：http://kw.jianghongdianzi.cn

public function __construct(private int $id) {}
来源：http://zj.yuexingan06.cn

[U51] PHP：数组解构
来源：http://vs.chemitech.net.cn

[$a, $b] = $arr;
来源：http://zk.lnxyls.cn

[U52] PHP：箭头函数
来源：http://ik.jctech888.com.cn

$double = fn($x) => $x * 2;
来源：http://sd.szxytkj.cn

[U53] PHP：空合并运算符
来源：http://jo.szsharing.cn

$v = $a ?? $b ?? "default";
来源：http://tt.lnxyls.cn

[U54] PHP：空安全调用
来源：http://qe.jctech888.com.cn

$obj?->method()
来源：http://lu.gzmigu.cn

[U55] PHP：match 表达式
来源：http://lh.bookmarksfly.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://aq.colortex.cn

[U56] PHP：命名参数
来源：http://yz.9csxet.cn

f(a: 1, b: 2)
来源：http://lq.newstarts.cn

[U57] PHP：字符串插值
来源：http://ge.huixiangedu.cn

"值: {$a}"
来源：http://zw.huanxung.cn

[U58] PHP：数组三件套
来源：http://rp.lnxyls.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://di.asd995.cn

[U59] PHP：自定义排序
来源：http://ju.shxzskj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mx.nicolike.cn

[U60] PHP：JSON 编解码
来源：http://xy.yuexingan06.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vr.9csxet.cn

[U61] PHP：正则
来源：http://fq.huanxung.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mp.huanxung.cn

[U62] PHP：日期对象
来源：http://xc.asd995.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bu.9csxet.cn

[U63] PHP：文件读写
来源：http://cu.bjjhwx.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kf.lnxyls.cn

[U64] PHP：目录遍历
来源：http://ln.huanxung.cn

glob("dir/*.php");  scandir("dir");
来源：http://qm.muxihuayi.cn

[U65] PHP：会话
来源：http://mg.521024.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ul.nszjky.cn

[U66] PHP：设置 Cookie
来源：http://st.muxihuayi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ma.shxzukj.cn

[U67] PHP：处理文件上传
来源：http://fv.huixiangedu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yc.gzmigu.cn

[U68] PHP：PDO 连接
来源：http://xx.colortex.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://eb.szxytkj.cn

[U69] PHP：PDO 预处理
来源：http://dt.szsharing.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://oj.wgjwhj.cn

[U70] PHP：PDO 事务
来源：http://mw.huanxung.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gt.szxytkj.cn

[U71] PHP：抛出异常
来源：http://dc.nicolike.cn

throw new RuntimeException("失败", 500);
来源：http://xt.hahajie.cn

[U72] PHP：写错误日志
来源：http://ba.huanxung.cn

error_log("失败: " . $e->getMessage());
来源：http://jo.szxytkj.cn

[U73] PHP：读取 ini 配置
来源：http://yl.yuexingan06.cn

parse_ini_file("config.ini", true)
来源：http://gh.nicolike.cn

[U74] PHP：读取环境变量
来源：http://uc.bjjhwx.cn

getenv("APP_ENV") ?: "production"
来源：http://ei.szsharing.cn

[U75] PHP：依赖注入
来源：http://dr.yuntaijiaju.cn

composer require psr/container
来源：http://mr.huanxung.cn

[U76] PHP：简单路由
来源：http://uo.newstarts.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ju.nicolike.cn

[U77] PHP：模板渲染
来源：http://jv.newstarts.cn

composer require twig/twig
来源：http://ho.huixiangedu.cn

[U78] PHP：单元测试
来源：http://of.hnjuh.cn

composer require --dev phpunit/phpunit
来源：http://di.hahajie.cn

[U79] PHP：静态分析
来源：http://zr.lnxyls.cn

composer require --dev phpstan/phpstan
来源：http://tu.jctech888.com.cn

[U80] PHP：代码规范修复
来源：http://hb.bjjhwx.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://er.gzmigu.cn

[U81] JS：初始化项目
来源：http://rg.jctech888.com.cn

npm init -y;  npm i express
来源：http://ls.huixinmuqiang.cn

[U82] JS：package.json 脚本
来源：http://yo.yuexingan06.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cb.newstarts.cn

[U83] JS：ES Module 导入导出
来源：http://lu.hahajie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zu.colortex.cn

[U84] JS：CommonJS 写法
来源：http://fs.hahajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ty.gzmigu.cn

[U85] JS：可选链
来源：http://ld.gzmigu.cn

a?.b?.c
来源：http://af.gzmigu.cn

[U86] JS：空值合并
来源：http://hd.521024.cn

a ?? b
来源：http://pa.haigaiapp.cn

[U87] JS：解构默认值
来源：http://ha.chemitech.net.cn

const { a = 1, b = 2 } = obj;
来源：http://av.newstarts.cn

[U88] JS：对象展开合并
来源：http://pz.asd995.cn

{ ...a, ...b }
来源：http://dc.lnxyls.cn

[U89] JS：数组去重
来源：http://ev.shxzskj.cn

[...new Set(arr)]
来源：http://ul.nszjky.cn

[U90] JS：数字数组排序
来源：http://yh.colortex.cn

[...arr].sort((a, b) => a - b)
来源：http://hp.szxytkj.cn

[U91] JS：对象键值遍历
来源：http://va.yuexingan06.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hy.bjjhwx.cn

[U92] JS：深拷贝
来源：http://yo.huixiangedu.cn

structuredClone(obj)
来源：http://dn.shxzukj.cn

[U93] JS：模板字符串
来源：http://dq.jctech888.com.cn

`共 ${n} 条`
来源：http://ii.shxzukj.cn

[U94] JS：箭头函数
来源：http://jk.shtwfgs.cn

const double = x => x * 2;
来源：http://wp.nszjky.cn

[U95] JS：Promise 包装
来源：http://cn.huanxung.cn

new Promise((resolve, reject) => {})
来源：http://pm.nicolike.cn

[U96] JS：async/await 与异常
来源：http://si.9csxet.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dz.newstarts.cn

[U97] JS：并发请求
来源：http://um.shxzukj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ip.hnjuh.cn

[U98] JS：fetch 带 JSON
来源：http://sn.colortex.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vw.huixinmuqiang.cn


<!-- 参考信息 -->