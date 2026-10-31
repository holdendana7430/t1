代发 wailian999

[T11] Kotlin：协程
来源：http://ws.jianghongdianzi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bh.yuexingan06.cn

[T12] Kotlin：解构声明
来源：http://es.huanxung.cn

val (a, b) = Pair(1, 2)
来源：http://xu.huixinmuqiang.cn

[T13] Kotlin：只读 Map
来源：http://cu.chemitech.net.cn

val m = mapOf("a" to 1)
来源：http://rd.shtwfgs.cn

[T14] Kotlin：循环
来源：http://ti.shxzukj.cn

for (i in 1..10) println(i)
来源：http://zw.9csxet.cn

[T15] Kotlin：接口
来源：http://qn.bookmarksfly.cn

interface Shape { fun area(): Double }
来源：http://mh.shxzskj.cn

[T16] Swift：Hello World
来源：http://ie.haigaiapp.cn

print("Hello")
来源：http://cs.szsharing.cn

[T17] Swift：变量与常量
来源：http://kn.nicolike.cn

var a = 1;  let b = 2
来源：http://fx.szsharing.cn

[T18] Swift：字符串插值
来源：http://br.wgjwhj.cn

"值: \(b)"
来源：http://kd.nszjky.cn

[T19] Swift：可选绑定
来源：http://oj.bjjhwx.cn

if let n = opt { print(n) }
来源：http://gf.nszjky.cn

[T20] Swift：数组操作
来源：http://sf.bookmarksfly.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ek.jianghongdianzi.cn

[T21] Swift：遍历
来源：http://ni.gzmigu.cn

for x in a { print(x) }
来源：http://aq.hahajie.cn

[T22] Swift：字典
来源：http://iz.hahajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zu.jctech888.com.cn

[T23] Swift：函数
来源：http://ph.521024.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://oq.asd995.cn

[T24] Swift：闭包
来源：http://od.szxytkj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gq.huanxung.cn

[T25] Swift：结构体
来源：http://gf.yuntaijiaju.cn

struct P { var x: Int }
来源：http://ep.lnxyls.cn

[T26] Swift：类与重写
来源：http://ar.panjiajie.cn

class A: Base { override func f() {} }
来源：http://kh.nszjky.cn

[T27] Swift：错误处理
来源：http://hs.muxihuayi.cn

do { try f() } catch { print(error) }
来源：http://kq.hnjuh.cn

[T28] Swift：枚举
来源：http://ew.yuntaijiaju.cn

enum Color { case red, green }
来源：http://xr.9csxet.cn

[T29] Swift：guard 提前返回
来源：http://bx.gzmigu.cn

guard let x = opt else { return }
来源：http://jr.bjjhwx.cn

[T30] Swift：协议
来源：http://dt.huixiangedu.cn

protocol Shape { func area() -> Double }
来源：http://ng.shtwfgs.cn

[T31] Lua：Hello World
来源：http://qu.szsharing.cn

print("Hello")
来源：http://kt.shtwfgs.cn

[T32] Lua：局部变量
来源：http://ic.szsharing.cn

local a = 1
来源：http://ox.haigaiapp.cn

[T33] Lua：表（数组）
来源：http://um.shxzukj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://bv.newstarts.cn

[T34] Lua：遍历表
来源：http://xi.chemitech.net.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qu.shxzskj.cn

[T35] Lua：字典表
来源：http://hw.shtwfgs.cn

local d = { a = 1 };  d.b = 2
来源：http://zu.huixiangedu.cn

[T36] Lua：函数
来源：http://sc.muxihuayi.cn

function add(a, b) return a + b end
来源：http://qh.jctech888.com.cn

[T37] Lua：字符串拼接
来源：http://xd.hnjuh.cn

"a" .. "b"
来源：http://uj.shxzskj.cn

[T38] Lua：条件
来源：http://ct.szxytkj.cn

if x > 0 then print("正") end
来源：http://pa.newstarts.cn

[T39] Lua：模式匹配
来源：http://zx.szsharing.cn

string.find(s, "%d+")
来源：http://hm.lnxyls.cn

[T40] Lua：元表
来源：http://ii.wgjwhj.cn

setmetatable({}, { __index = base })
来源：http://ye.huixinmuqiang.cn

[T41] Perl：Hello World
来源：http://jf.bjjhwx.cn

print "Hello\n";
来源：http://ou.szxytkj.cn

[T42] Perl：变量类型
来源：http://qc.shtwfgs.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ie.shxzukj.cn

[T43] Perl：字符串插值
来源：http://dy.huixinmuqiang.cn

"值: $a"
来源：http://fv.hahajie.cn

[T44] Perl：条件
来源：http://dk.hnjuh.cn

if ($a > 0) { print "正"; }
来源：http://ak.asd995.cn

[T45] Perl：数组遍历
来源：http://wm.yuexingan06.cn

for my $x (@arr) { print $x; }
来源：http://ci.nicolike.cn

[T46] Perl：哈希操作
来源：http://gy.huixinmuqiang.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ly.lnxyls.cn

[T47] Perl：正则捕获
来源：http://ee.huixiangedu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rv.szsharing.cn

[T48] Perl：正则替换
来源：http://oz.huixiangedu.cn

$s =~ s/old/new/g;
来源：http://pg.shtwfgs.cn

[T49] Perl：函数
来源：http://wp.jctech888.com.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://od.colortex.cn

[T50] Perl：逐行读文件
来源：http://qo.panjiajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://yr.hahajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://us.newstarts.cn

[T51] Scala：Hello World
来源：http://ei.chemitech.net.cn

println("Hello")
来源：http://kh.521024.cn

[T52] Scala：变量
来源：http://rs.bjjhwx.cn

val a = 1;  var b = 2
来源：http://my.szsharing.cn

[T53] Scala：字符串插值
来源：http://pm.shxzukj.cn

s"值: $b"
来源：http://od.hahajie.cn

[T54] Scala：集合映射
来源：http://rx.hahajie.cn

List(1, 2, 3).map(_ * 2)
来源：http://pr.jctech888.com.cn

[T55] Scala：集合过滤
来源：http://lh.hnjuh.cn

List(1, 2, 3).filter(_ > 1)
来源：http://du.huixiangedu.cn

[T56] Scala：样例类
来源：http://ox.bjjhwx.cn

case class User(name: String, age: Int)
来源：http://ar.asd995.cn

[T57] Scala：模式匹配
来源：http://xv.hahajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://oi.nszjky.cn

[T58] Scala：函数定义
来源：http://lo.yuexingan06.cn

def add(a: Int, b: Int): Int = a + b
来源：http://yt.nszjky.cn

[T59] Scala：循环
来源：http://ba.asd995.cn

for (i <- 1 to 10) println(i)
来源：http://ne.yuexingan06.cn

[T60] Scala：折叠
来源：http://ks.nszjky.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ru.bjjhwx.cn

================================================================================
来源：http://ms.nszjky.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://td.szsharing.cn

================================================================================
来源：http://eg.hahajie.cn

[U01] Py：创建虚拟环境
来源：http://xo.colortex.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nl.huixiangedu.cn

[U02] Py：导出 / 安装依赖
来源：http://zv.nszjky.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tx.hnjuh.cn

[U03] Py：加载 .env 配置
来源：http://tc.shtwfgs.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://jo.lnxyls.cn

[U04] Py：变量调试打印
来源：http://fs.shxzukj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gt.huixiangedu.cn

[U05] Py：列表去重且保序
来源：http://nh.haigaiapp.cn

list(dict.fromkeys(arr))
来源：http://xx.shxzskj.cn

[U06] Py：合并两个字典
来源：http://wf.shtwfgs.cn

{**a, **b}
来源：http://ef.yuntaijiaju.cn

[U07] Py：反转字典键值
来源：http://te.huanxung.cn

{v: k for k, v in d.items()}
来源：http://nq.chemitech.net.cn

[U08] Py：展平二维列表
来源：http://qo.yuntaijiaju.cn

[y for x in nested for y in x]
来源：http://zq.szsharing.cn

[U09] Py：字典取最大值的键
来源：http://lm.9csxet.cn

max(d, key=d.get)
来源：http://tx.521024.cn

[U10] Py：按值排序字典
来源：http://lu.bjjhwx.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lh.newstarts.cn

[U11] Py：生成器表达式
来源：http://hd.huixiangedu.cn

(x * 2 for x in arr)
来源：http://sz.yuntaijiaju.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ao.gzmigu.cn

Counter(arr).most_common(3)
来源：http://uc.colortex.cn

[U13] Py：固定长度队列
来源：http://us.huixinmuqiang.cn

deque(maxlen=10)
来源：http://rl.jianghongdianzi.cn

[U14] Py：分组收集到列表
来源：http://zg.colortex.cn

defaultdict(list)
来源：http://pz.muxihuayi.cn

[U15] Py：高精度计时
来源：http://ck.haigaiapp.cn

t = time.perf_counter()
来源：http://xd.newstarts.cn

[U16] Py：命令行参数解析
来源：http://qk.jianghongdianzi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jc.lnxyls.cn

[U17] Py：初始化日志
来源：http://jh.wgjwhj.cn

logging.basicConfig(level=logging.INFO)
来源：http://so.haigaiapp.cn

[U18] Py：预编译正则
来源：http://gp.huixiangedu.cn

pat = re.compile(r"\d+")
来源：http://jl.szsharing.cn

[U19] Py：正则替换带回调
来源：http://lv.bookmarksfly.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zy.muxihuayi.cn

[U20] Py：缓存函数结果
来源：http://om.lnxyls.cn

@functools.lru_cache(maxsize=None)
来源：http://fl.lnxyls.cn

[U21] Py：自定义上下文管理器
来源：http://ic.lnxyls.cn

@contextlib.contextmanager
来源：http://vd.muxihuayi.cn

[U22] Py：矩阵转置
来源：http://aa.bjjhwx.cn

list(zip(*m))
来源：http://us.9csxet.cn

[U23] Py：分块读取大文件
来源：http://oa.haigaiapp.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cg.panjiajie.cn

[U24] Py：路径操作
来源：http://gi.szsharing.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bj.nszjky.cn

[U25] Py：CSV 按字典读
来源：http://lt.chemitech.net.cn

csv.DictReader(f)
来源：http://mc.9csxet.cn

[U26] Py：并发下载
来源：http://qr.haigaiapp.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xr.shxzukj.cn

[U27] Py：异步 HTTP
来源：http://lv.hahajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://or.hahajie.cn

[U28] Py：类型别名
来源：http://pf.bookmarksfly.cn

UserId = int
来源：http://tr.bjjhwx.cn

[U29] Py：属性校验
来源：http://kw.jctech888.com.cn

@property 与 @x.setter 配合
来源：http://sd.szxytkj.cn

[U30] Py：数据类
来源：http://pv.yuntaijiaju.cn

@dataclass(slots=True)
来源：http://df.panjiajie.cn

[U31] Py：单测
来源：http://og.newstarts.cn

python -m pytest -q
来源：http://df.nszjky.cn

[U32] Py：代码格式化
来源：http://fr.muxihuayi.cn

ruff format . && ruff check --fix .
来源：http://va.yuexingan06.cn

[U33] Py：打包发布
来源：http://lr.panjiajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://gh.wgjwhj.cn

[U34] Py：判断编码
来源：http://ci.lnxyls.cn

chardet.detect(raw)
来源：http://sa.nszjky.cn

[U35] Py：发送邮件
来源：http://ei.shxzskj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gl.szxytkj.cn

[U36] Py：定时任务
来源：http://cw.lnxyls.cn

schedule.every(10).minutes.do(job)
来源：http://lu.hahajie.cn

[U37] Py：读写 Excel
来源：http://yx.colortex.cn

pandas.read_excel / DataFrame.to_excel
来源：http://zo.haigaiapp.cn

[U38] Py：获取脚本所在目录
来源：http://zi.shxzskj.cn

Path(__file__).resolve().parent
来源：http://oz.huixinmuqiang.cn

[U39] Py：判断是否在交互环境
来源：http://un.yuexingan06.cn

sys.stdout.isatty()
来源：http://xm.panjiajie.cn

[U40] Py：打印到标准错误
来源：http://ew.asd995.cn

print("err", file=sys.stderr)
来源：http://dp.shxzukj.cn

[U41] PHP：初始化 Composer 项目
来源：http://pi.9csxet.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ap.shxzukj.cn

[U42] PHP：PSR-4 自动加载
来源：http://wg.521024.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ag.shtwfgs.cn

[U43] PHP：声明命名空间
来源：http://yn.chemitech.net.cn

namespace App\Http;
来源：http://ju.nszjky.cn

[U44] PHP：开启严格类型
来源：http://wg.9csxet.cn

declare(strict_types=1);
来源：http://yv.hahajie.cn

[U45] PHP：类型声明与返回类型
来源：http://nw.colortex.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://oy.shxzukj.cn

[U46] PHP：可空类型
来源：http://sk.yuntaijiaju.cn

?string $name = null
来源：http://is.huixinmuqiang.cn

[U47] PHP：联合类型
来源：http://mk.huanxung.cn

int|string $id
来源：http://zp.szsharing.cn

[U48] PHP：纯枚举
来源：http://yz.huixinmuqiang.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wb.szxytkj.cn

[U49] PHP：只读属性
来源：http://wg.shxzukj.cn

public readonly string $name
来源：http://ms.lnxyls.cn

[U50] PHP：构造器属性提升
来源：http://bz.lnxyls.cn

public function __construct(private int $id) {}
来源：http://rp.huixiangedu.cn

[U51] PHP：数组解构
来源：http://yu.asd995.cn

[$a, $b] = $arr;
来源：http://yo.shtwfgs.cn

[U52] PHP：箭头函数
来源：http://tc.yuexingan06.cn

$double = fn($x) => $x * 2;
来源：http://go.huixiangedu.cn

[U53] PHP：空合并运算符
来源：http://dz.huanxung.cn

$v = $a ?? $b ?? "default";
来源：http://ac.521024.cn

[U54] PHP：空安全调用
来源：http://nx.9csxet.cn

$obj?->method()
来源：http://ox.hahajie.cn

[U55] PHP：match 表达式
来源：http://ys.szsharing.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hy.newstarts.cn

[U56] PHP：命名参数
来源：http://nq.gzmigu.cn

f(a: 1, b: 2)
来源：http://jh.yuexingan06.cn

[U57] PHP：字符串插值
来源：http://bw.nicolike.cn

"值: {$a}"
来源：http://ly.lnxyls.cn

[U58] PHP：数组三件套
来源：http://he.hahajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://od.gzmigu.cn

[U59] PHP：自定义排序
来源：http://vf.shtwfgs.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ny.huixiangedu.cn

[U60] PHP：JSON 编解码
来源：http://qz.bjjhwx.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fp.hnjuh.cn

[U61] PHP：正则
来源：http://no.szxytkj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vm.yuexingan06.cn

[U62] PHP：日期对象
来源：http://rv.bookmarksfly.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fn.lnxyls.cn

[U63] PHP：文件读写
来源：http://ky.9csxet.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gw.bjjhwx.cn

[U64] PHP：目录遍历
来源：http://je.asd995.cn

glob("dir/*.php");  scandir("dir");
来源：http://tv.shtwfgs.cn

[U65] PHP：会话
来源：http://pc.asd995.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://fy.panjiajie.cn

[U66] PHP：设置 Cookie
来源：http://fi.bjjhwx.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nn.shxzskj.cn

[U67] PHP：处理文件上传
来源：http://xx.shxzukj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yn.muxihuayi.cn

[U68] PHP：PDO 连接
来源：http://ot.lnxyls.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jz.szxytkj.cn

[U69] PHP：PDO 预处理
来源：http://dp.chemitech.net.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pr.521024.cn

[U70] PHP：PDO 事务
来源：http://ax.bjjhwx.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mw.haigaiapp.cn

[U71] PHP：抛出异常
来源：http://np.asd995.cn

throw new RuntimeException("失败", 500);
来源：http://ks.szsharing.cn

[U72] PHP：写错误日志
来源：http://fn.panjiajie.cn

error_log("失败: " . $e->getMessage());
来源：http://ji.yuexingan06.cn

[U73] PHP：读取 ini 配置
来源：http://pc.nicolike.cn

parse_ini_file("config.ini", true)
来源：http://lo.wgjwhj.cn

[U74] PHP：读取环境变量
来源：http://uk.chemitech.net.cn

getenv("APP_ENV") ?: "production"
来源：http://yf.newstarts.cn

[U75] PHP：依赖注入
来源：http://vj.bjjhwx.cn

composer require psr/container
来源：http://kd.hnjuh.cn

[U76] PHP：简单路由
来源：http://ct.szsharing.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fd.gzmigu.cn

[U77] PHP：模板渲染
来源：http://fn.shtwfgs.cn

composer require twig/twig
来源：http://tm.bookmarksfly.cn

[U78] PHP：单元测试
来源：http://fr.szxytkj.cn

composer require --dev phpunit/phpunit
来源：http://ia.wgjwhj.cn

[U79] PHP：静态分析
来源：http://fv.bookmarksfly.cn

composer require --dev phpstan/phpstan
来源：http://rx.yuexingan06.cn

[U80] PHP：代码规范修复
来源：http://ps.huixiangedu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ji.nszjky.cn

[U81] JS：初始化项目
来源：http://rn.521024.cn

npm init -y;  npm i express
来源：http://bs.muxihuayi.cn

[U82] JS：package.json 脚本
来源：http://eg.asd995.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zj.shtwfgs.cn

[U83] JS：ES Module 导入导出
来源：http://xb.szxytkj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ac.huanxung.cn

[U84] JS：CommonJS 写法
来源：http://gf.521024.cn

module.exports = { a };  const { a } = require("./m");
来源：http://br.colortex.cn

[U85] JS：可选链
来源：http://ce.newstarts.cn

a?.b?.c
来源：http://rz.yuntaijiaju.cn

[U86] JS：空值合并
来源：http://bt.jctech888.com.cn

a ?? b
来源：http://bi.521024.cn

[U87] JS：解构默认值
来源：http://wz.muxihuayi.cn

const { a = 1, b = 2 } = obj;
来源：http://as.hnjuh.cn

[U88] JS：对象展开合并
来源：http://bk.shxzukj.cn

{ ...a, ...b }
来源：http://to.shxzskj.cn

[U89] JS：数组去重
来源：http://hb.nicolike.cn

[...new Set(arr)]
来源：http://hi.huixinmuqiang.cn

[U90] JS：数字数组排序
来源：http://vc.szsharing.cn

[...arr].sort((a, b) => a - b)
来源：http://xt.hahajie.cn

[U91] JS：对象键值遍历
来源：http://jx.9csxet.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ok.szxytkj.cn

[U92] JS：深拷贝
来源：http://yx.521024.cn

structuredClone(obj)
来源：http://ih.yuexingan06.cn

[U93] JS：模板字符串
来源：http://xk.shtwfgs.cn

`共 ${n} 条`
来源：http://ux.huanxung.cn

[U94] JS：箭头函数
来源：http://uz.muxihuayi.cn

const double = x => x * 2;
来源：http://zb.9csxet.cn

[U95] JS：Promise 包装
来源：http://pf.colortex.cn

new Promise((resolve, reject) => {})
来源：http://we.huanxung.cn

[U96] JS：async/await 与异常
来源：http://mb.nicolike.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cr.huanxung.cn

[U97] JS：并发请求
来源：http://zf.szxytkj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qh.colortex.cn

[U98] JS：fetch 带 JSON
来源：http://rs.szxytkj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://iy.chemitech.net.cn


<!-- 参考信息 -->