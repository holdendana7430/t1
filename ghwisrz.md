代发 wailian999

[T07] Kotlin：集合过滤
来源：http://no.9csxet.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lt.yuntaijiaju.cn

[T08] Kotlin：数据类
来源：http://ex.bjjhwx.cn

data class User(val name: String, val age: Int)
来源：http://ij.hnjuh.cn

[T09] Kotlin：扩展函数
来源：http://mk.haigaiapp.cn

fun String.exclaim() = this + "!"
来源：http://ve.shtwfgs.cn

[T10] Kotlin：默认参数
来源：http://jd.huixinmuqiang.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tk.asd995.cn

[T11] Kotlin：协程
来源：http://qn.huanxung.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qv.jctech888.com.cn

[T12] Kotlin：解构声明
来源：http://wi.gzmigu.cn

val (a, b) = Pair(1, 2)
来源：http://gt.hahajie.cn

[T13] Kotlin：只读 Map
来源：http://gi.nszjky.cn

val m = mapOf("a" to 1)
来源：http://hn.wgjwhj.cn

[T14] Kotlin：循环
来源：http://dd.lnxyls.cn

for (i in 1..10) println(i)
来源：http://wf.nszjky.cn

[T15] Kotlin：接口
来源：http://nh.huixiangedu.cn

interface Shape { fun area(): Double }
来源：http://pr.muxihuayi.cn

[T16] Swift：Hello World
来源：http://zk.szsharing.cn

print("Hello")
来源：http://ac.wgjwhj.cn

[T17] Swift：变量与常量
来源：http://lt.huixinmuqiang.cn

var a = 1;  let b = 2
来源：http://xp.yuntaijiaju.cn

[T18] Swift：字符串插值
来源：http://hu.jctech888.com.cn

"值: \(b)"
来源：http://bt.hahajie.cn

[T19] Swift：可选绑定
来源：http://lf.huanxung.cn

if let n = opt { print(n) }
来源：http://il.muxihuayi.cn

[T20] Swift：数组操作
来源：http://ea.newstarts.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zo.huanxung.cn

[T21] Swift：遍历
来源：http://ra.bookmarksfly.cn

for x in a { print(x) }
来源：http://vr.gzmigu.cn

[T22] Swift：字典
来源：http://lp.bookmarksfly.cn

var d = ["a": 1];  d["b"] = 2
来源：http://su.shxzukj.cn

[T23] Swift：函数
来源：http://nx.chemitech.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ju.huixiangedu.cn

[T24] Swift：闭包
来源：http://lv.yuexingan06.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://oz.asd995.cn

[T25] Swift：结构体
来源：http://ng.muxihuayi.cn

struct P { var x: Int }
来源：http://eg.yuntaijiaju.cn

[T26] Swift：类与重写
来源：http://wu.yuntaijiaju.cn

class A: Base { override func f() {} }
来源：http://mj.szxytkj.cn

[T27] Swift：错误处理
来源：http://sy.hahajie.cn

do { try f() } catch { print(error) }
来源：http://cl.521024.cn

[T28] Swift：枚举
来源：http://wb.521024.cn

enum Color { case red, green }
来源：http://za.lnxyls.cn

[T29] Swift：guard 提前返回
来源：http://mh.szxytkj.cn

guard let x = opt else { return }
来源：http://io.shtwfgs.cn

[T30] Swift：协议
来源：http://cx.newstarts.cn

protocol Shape { func area() -> Double }
来源：http://qb.huanxung.cn

[T31] Lua：Hello World
来源：http://eq.shxzukj.cn

print("Hello")
来源：http://ht.muxihuayi.cn

[T32] Lua：局部变量
来源：http://qz.jianghongdianzi.cn

local a = 1
来源：http://ro.szxytkj.cn

[T33] Lua：表（数组）
来源：http://zk.nszjky.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xi.yuexingan06.cn

[T34] Lua：遍历表
来源：http://zv.yuntaijiaju.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rn.muxihuayi.cn

[T35] Lua：字典表
来源：http://dy.gzmigu.cn

local d = { a = 1 };  d.b = 2
来源：http://gn.jctech888.com.cn

[T36] Lua：函数
来源：http://to.nszjky.cn

function add(a, b) return a + b end
来源：http://xj.haigaiapp.cn

[T37] Lua：字符串拼接
来源：http://rr.9csxet.cn

"a" .. "b"
来源：http://sm.jctech888.com.cn

[T38] Lua：条件
来源：http://sp.gzmigu.cn

if x > 0 then print("正") end
来源：http://eq.shxzskj.cn

[T39] Lua：模式匹配
来源：http://ci.muxihuayi.cn

string.find(s, "%d+")
来源：http://bq.wgjwhj.cn

[T40] Lua：元表
来源：http://hc.jianghongdianzi.cn

setmetatable({}, { __index = base })
来源：http://mc.huanxung.cn

[T41] Perl：Hello World
来源：http://md.jianghongdianzi.cn

print "Hello\n";
来源：http://hf.bookmarksfly.cn

[T42] Perl：变量类型
来源：http://jb.521024.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://so.yuexingan06.cn

[T43] Perl：字符串插值
来源：http://ge.haigaiapp.cn

"值: $a"
来源：http://md.szxytkj.cn

[T44] Perl：条件
来源：http://tu.shtwfgs.cn

if ($a > 0) { print "正"; }
来源：http://ao.colortex.cn

[T45] Perl：数组遍历
来源：http://ox.huixiangedu.cn

for my $x (@arr) { print $x; }
来源：http://ui.bjjhwx.cn

[T46] Perl：哈希操作
来源：http://gj.panjiajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dx.nszjky.cn

[T47] Perl：正则捕获
来源：http://jc.nszjky.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wg.wgjwhj.cn

[T48] Perl：正则替换
来源：http://ny.colortex.cn

$s =~ s/old/new/g;
来源：http://xf.9csxet.cn

[T49] Perl：函数
来源：http://ze.jctech888.com.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lz.huixinmuqiang.cn

[T50] Perl：逐行读文件
来源：http://jy.bjjhwx.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://nm.jianghongdianzi.cn

while (my $line = <$fh>) { print $line; }
来源：http://iw.521024.cn

[T51] Scala：Hello World
来源：http://nr.9csxet.cn

println("Hello")
来源：http://qf.asd995.cn

[T52] Scala：变量
来源：http://xf.yuexingan06.cn

val a = 1;  var b = 2
来源：http://av.shtwfgs.cn

[T53] Scala：字符串插值
来源：http://bv.panjiajie.cn

s"值: $b"
来源：http://at.gzmigu.cn

[T54] Scala：集合映射
来源：http://hz.bookmarksfly.cn

List(1, 2, 3).map(_ * 2)
来源：http://mr.huixinmuqiang.cn

[T55] Scala：集合过滤
来源：http://rp.hahajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fx.chemitech.net.cn

[T56] Scala：样例类
来源：http://ms.yuexingan06.cn

case class User(name: String, age: Int)
来源：http://vf.gzmigu.cn

[T57] Scala：模式匹配
来源：http://jg.yuexingan06.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://qg.szxytkj.cn

[T58] Scala：函数定义
来源：http://gx.colortex.cn

def add(a: Int, b: Int): Int = a + b
来源：http://km.hnjuh.cn

[T59] Scala：循环
来源：http://ch.jianghongdianzi.cn

for (i <- 1 to 10) println(i)
来源：http://tt.yuexingan06.cn

[T60] Scala：折叠
来源：http://ud.bookmarksfly.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://de.haigaiapp.cn

================================================================================
来源：http://fq.9csxet.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qn.huixinmuqiang.cn

================================================================================
来源：http://zg.muxihuayi.cn

[U01] Py：创建虚拟环境
来源：http://ay.panjiajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://si.bjjhwx.cn

[U02] Py：导出 / 安装依赖
来源：http://iy.hnjuh.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jb.szsharing.cn

[U03] Py：加载 .env 配置
来源：http://ht.jianghongdianzi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qt.shxzskj.cn

[U04] Py：变量调试打印
来源：http://js.hnjuh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rt.panjiajie.cn

[U05] Py：列表去重且保序
来源：http://zr.jctech888.com.cn

list(dict.fromkeys(arr))
来源：http://ni.nicolike.cn

[U06] Py：合并两个字典
来源：http://gq.shtwfgs.cn

{**a, **b}
来源：http://lq.szsharing.cn

[U07] Py：反转字典键值
来源：http://yw.chemitech.net.cn

{v: k for k, v in d.items()}
来源：http://iy.yuexingan06.cn

[U08] Py：展平二维列表
来源：http://hh.nszjky.cn

[y for x in nested for y in x]
来源：http://pe.wgjwhj.cn

[U09] Py：字典取最大值的键
来源：http://kt.hnjuh.cn

max(d, key=d.get)
来源：http://wf.szsharing.cn

[U10] Py：按值排序字典
来源：http://ag.9csxet.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pc.jianghongdianzi.cn

[U11] Py：生成器表达式
来源：http://le.panjiajie.cn

(x * 2 for x in arr)
来源：http://im.newstarts.cn

[U12] Py：取出现最多的 3 个元素
来源：http://is.bookmarksfly.cn

Counter(arr).most_common(3)
来源：http://qz.hnjuh.cn

[U13] Py：固定长度队列
来源：http://kt.nicolike.cn

deque(maxlen=10)
来源：http://ho.asd995.cn

[U14] Py：分组收集到列表
来源：http://ro.521024.cn

defaultdict(list)
来源：http://gc.gzmigu.cn

[U15] Py：高精度计时
来源：http://as.bjjhwx.cn

t = time.perf_counter()
来源：http://ph.huanxung.cn

[U16] Py：命令行参数解析
来源：http://dl.wgjwhj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wq.nszjky.cn

[U17] Py：初始化日志
来源：http://dm.shtwfgs.cn

logging.basicConfig(level=logging.INFO)
来源：http://em.bookmarksfly.cn

[U18] Py：预编译正则
来源：http://vi.haigaiapp.cn

pat = re.compile(r"\d+")
来源：http://jn.lnxyls.cn

[U19] Py：正则替换带回调
来源：http://qd.521024.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://iq.huanxung.cn

[U20] Py：缓存函数结果
来源：http://xm.nicolike.cn

@functools.lru_cache(maxsize=None)
来源：http://tq.521024.cn

[U21] Py：自定义上下文管理器
来源：http://ec.shtwfgs.cn

@contextlib.contextmanager
来源：http://nr.asd995.cn

[U22] Py：矩阵转置
来源：http://om.yuexingan06.cn

list(zip(*m))
来源：http://up.chemitech.net.cn

[U23] Py：分块读取大文件
来源：http://qo.yuexingan06.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ek.jctech888.com.cn

[U24] Py：路径操作
来源：http://ya.huixiangedu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fz.panjiajie.cn

[U25] Py：CSV 按字典读
来源：http://nz.9csxet.cn

csv.DictReader(f)
来源：http://um.nicolike.cn

[U26] Py：并发下载
来源：http://ig.lnxyls.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jm.yuexingan06.cn

[U27] Py：异步 HTTP
来源：http://mr.shxzukj.cn

aiohttp.ClientSession() 配合 async with
来源：http://gj.muxihuayi.cn

[U28] Py：类型别名
来源：http://rj.chemitech.net.cn

UserId = int
来源：http://qm.hnjuh.cn

[U29] Py：属性校验
来源：http://ng.szxytkj.cn

@property 与 @x.setter 配合
来源：http://ud.szxytkj.cn

[U30] Py：数据类
来源：http://la.muxihuayi.cn

@dataclass(slots=True)
来源：http://mr.gzmigu.cn

[U31] Py：单测
来源：http://qi.muxihuayi.cn

python -m pytest -q
来源：http://gt.huixinmuqiang.cn

[U32] Py：代码格式化
来源：http://xq.szxytkj.cn

ruff format . && ruff check --fix .
来源：http://dq.muxihuayi.cn

[U33] Py：打包发布
来源：http://ss.lnxyls.cn

python -m build  （依赖 pyproject.toml）
来源：http://kw.shxzskj.cn

[U34] Py：判断编码
来源：http://ow.chemitech.net.cn

chardet.detect(raw)
来源：http://za.muxihuayi.cn

[U35] Py：发送邮件
来源：http://xv.szsharing.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dn.yuntaijiaju.cn

[U36] Py：定时任务
来源：http://ky.haigaiapp.cn

schedule.every(10).minutes.do(job)
来源：http://hg.bookmarksfly.cn

[U37] Py：读写 Excel
来源：http://oq.bookmarksfly.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jf.bjjhwx.cn

[U38] Py：获取脚本所在目录
来源：http://ah.yuexingan06.cn

Path(__file__).resolve().parent
来源：http://pv.hnjuh.cn

[U39] Py：判断是否在交互环境
来源：http://ht.szsharing.cn

sys.stdout.isatty()
来源：http://nz.nszjky.cn

[U40] Py：打印到标准错误
来源：http://jg.muxihuayi.cn

print("err", file=sys.stderr)
来源：http://ad.newstarts.cn

[U41] PHP：初始化 Composer 项目
来源：http://mf.shxzukj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ks.hnjuh.cn

[U42] PHP：PSR-4 自动加载
来源：http://ni.haigaiapp.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vm.wgjwhj.cn

[U43] PHP：声明命名空间
来源：http://mo.panjiajie.cn

namespace App\Http;
来源：http://sl.jctech888.com.cn

[U44] PHP：开启严格类型
来源：http://ok.jctech888.com.cn

declare(strict_types=1);
来源：http://yl.521024.cn

[U45] PHP：类型声明与返回类型
来源：http://gl.jctech888.com.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://vj.newstarts.cn

[U46] PHP：可空类型
来源：http://tc.szsharing.cn

?string $name = null
来源：http://lx.huixinmuqiang.cn

[U47] PHP：联合类型
来源：http://fa.bjjhwx.cn

int|string $id
来源：http://tr.yuexingan06.cn

[U48] PHP：纯枚举
来源：http://gr.shxzskj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hp.9csxet.cn

[U49] PHP：只读属性
来源：http://or.bjjhwx.cn

public readonly string $name
来源：http://sy.szxytkj.cn

[U50] PHP：构造器属性提升
来源：http://ue.shxzukj.cn

public function __construct(private int $id) {}
来源：http://if.521024.cn

[U51] PHP：数组解构
来源：http://vz.yuexingan06.cn

[$a, $b] = $arr;
来源：http://yq.haigaiapp.cn

[U52] PHP：箭头函数
来源：http://yb.newstarts.cn

$double = fn($x) => $x * 2;
来源：http://rj.hnjuh.cn

[U53] PHP：空合并运算符
来源：http://be.panjiajie.cn

$v = $a ?? $b ?? "default";
来源：http://hq.hnjuh.cn

[U54] PHP：空安全调用
来源：http://ey.asd995.cn

$obj?->method()
来源：http://ab.haigaiapp.cn

[U55] PHP：match 表达式
来源：http://kn.9csxet.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hs.newstarts.cn

[U56] PHP：命名参数
来源：http://el.nszjky.cn

f(a: 1, b: 2)
来源：http://pu.newstarts.cn

[U57] PHP：字符串插值
来源：http://cs.szsharing.cn

"值: {$a}"
来源：http://vw.wgjwhj.cn

[U58] PHP：数组三件套
来源：http://ug.shxzukj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lo.bookmarksfly.cn

[U59] PHP：自定义排序
来源：http://cr.szsharing.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://re.panjiajie.cn

[U60] PHP：JSON 编解码
来源：http://ly.shxzskj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ow.huixinmuqiang.cn

[U61] PHP：正则
来源：http://wc.newstarts.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vh.huixinmuqiang.cn

[U62] PHP：日期对象
来源：http://qi.bookmarksfly.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ut.muxihuayi.cn

[U63] PHP：文件读写
来源：http://ls.nszjky.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://eq.shxzskj.cn

[U64] PHP：目录遍历
来源：http://fd.yuntaijiaju.cn

glob("dir/*.php");  scandir("dir");
来源：http://oq.shxzskj.cn

[U65] PHP：会话
来源：http://aa.szxytkj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ia.jctech888.com.cn

[U66] PHP：设置 Cookie
来源：http://ij.shtwfgs.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lr.shxzskj.cn

[U67] PHP：处理文件上传
来源：http://vx.gzmigu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hq.nszjky.cn

[U68] PHP：PDO 连接
来源：http://to.panjiajie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qa.hnjuh.cn

[U69] PHP：PDO 预处理
来源：http://ff.haigaiapp.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dn.muxihuayi.cn

[U70] PHP：PDO 事务
来源：http://eh.jctech888.com.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hy.gzmigu.cn

[U71] PHP：抛出异常
来源：http://tf.hahajie.cn

throw new RuntimeException("失败", 500);
来源：http://aq.hnjuh.cn

[U72] PHP：写错误日志
来源：http://jr.haigaiapp.cn

error_log("失败: " . $e->getMessage());
来源：http://kc.521024.cn

[U73] PHP：读取 ini 配置
来源：http://ue.yuntaijiaju.cn

parse_ini_file("config.ini", true)
来源：http://gm.huanxung.cn

[U74] PHP：读取环境变量
来源：http://nd.wgjwhj.cn

getenv("APP_ENV") ?: "production"
来源：http://ef.panjiajie.cn

[U75] PHP：依赖注入
来源：http://ef.shtwfgs.cn

composer require psr/container
来源：http://vk.shtwfgs.cn

[U76] PHP：简单路由
来源：http://tb.huanxung.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vs.shxzskj.cn

[U77] PHP：模板渲染
来源：http://rq.yuexingan06.cn

composer require twig/twig
来源：http://wu.shxzskj.cn

[U78] PHP：单元测试
来源：http://zh.gzmigu.cn

composer require --dev phpunit/phpunit
来源：http://uf.huixinmuqiang.cn

[U79] PHP：静态分析
来源：http://pm.huixiangedu.cn

composer require --dev phpstan/phpstan
来源：http://fy.huixinmuqiang.cn

[U80] PHP：代码规范修复
来源：http://bd.bjjhwx.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://kj.shtwfgs.cn

[U81] JS：初始化项目
来源：http://bw.shtwfgs.cn

npm init -y;  npm i express
来源：http://sa.haigaiapp.cn

[U82] JS：package.json 脚本
来源：http://fv.chemitech.net.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lo.shxzukj.cn

[U83] JS：ES Module 导入导出
来源：http://fb.wgjwhj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ih.muxihuayi.cn

[U84] JS：CommonJS 写法
来源：http://ij.muxihuayi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://pv.asd995.cn

[U85] JS：可选链
来源：http://xj.hahajie.cn

a?.b?.c
来源：http://rd.lnxyls.cn

[U86] JS：空值合并
来源：http://cb.nszjky.cn

a ?? b
来源：http://gr.nicolike.cn

[U87] JS：解构默认值
来源：http://mi.shxzskj.cn

const { a = 1, b = 2 } = obj;
来源：http://oc.shtwfgs.cn

[U88] JS：对象展开合并
来源：http://we.bookmarksfly.cn

{ ...a, ...b }
来源：http://lc.nszjky.cn

[U89] JS：数组去重
来源：http://re.nszjky.cn

[...new Set(arr)]
来源：http://wo.9csxet.cn

[U90] JS：数字数组排序
来源：http://gd.haigaiapp.cn

[...arr].sort((a, b) => a - b)
来源：http://yc.colortex.cn

[U91] JS：对象键值遍历
来源：http://iy.haigaiapp.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ht.newstarts.cn

[U92] JS：深拷贝
来源：http://dp.hahajie.cn

structuredClone(obj)
来源：http://at.colortex.cn

[U93] JS：模板字符串
来源：http://kd.yuexingan06.cn

`共 ${n} 条`
来源：http://tc.huixiangedu.cn

[U94] JS：箭头函数
来源：http://nu.haigaiapp.cn

const double = x => x * 2;
来源：http://ys.jctech888.com.cn


<!-- 参考信息 -->