代发 wailian999

[T11] Kotlin：协程
来源：http://fj.asd995.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jr.asd995.cn

[T12] Kotlin：解构声明
来源：http://ls.nicolike.cn

val (a, b) = Pair(1, 2)
来源：http://pu.9csxet.cn

[T13] Kotlin：只读 Map
来源：http://co.huanxung.cn

val m = mapOf("a" to 1)
来源：http://wv.huixiangedu.cn

[T14] Kotlin：循环
来源：http://cq.bjjhwx.cn

for (i in 1..10) println(i)
来源：http://al.521024.cn

[T15] Kotlin：接口
来源：http://hx.nszjky.cn

interface Shape { fun area(): Double }
来源：http://cu.szxytkj.cn

[T16] Swift：Hello World
来源：http://zr.szxytkj.cn

print("Hello")
来源：http://ud.jctech888.com.cn

[T17] Swift：变量与常量
来源：http://pm.nszjky.cn

var a = 1;  let b = 2
来源：http://kx.colortex.cn

[T18] Swift：字符串插值
来源：http://oe.huixiangedu.cn

"值: \(b)"
来源：http://kx.panjiajie.cn

[T19] Swift：可选绑定
来源：http://kj.hnjuh.cn

if let n = opt { print(n) }
来源：http://ri.asd995.cn

[T20] Swift：数组操作
来源：http://in.yuexingan06.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qd.huixiangedu.cn

[T21] Swift：遍历
来源：http://fv.shxzukj.cn

for x in a { print(x) }
来源：http://ho.asd995.cn

[T22] Swift：字典
来源：http://fk.yuexingan06.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mj.jctech888.com.cn

[T23] Swift：函数
来源：http://ac.bjjhwx.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bp.9csxet.cn

[T24] Swift：闭包
来源：http://ob.haigaiapp.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://jk.jctech888.com.cn

[T25] Swift：结构体
来源：http://jw.bookmarksfly.cn

struct P { var x: Int }
来源：http://om.bjjhwx.cn

[T26] Swift：类与重写
来源：http://qn.9csxet.cn

class A: Base { override func f() {} }
来源：http://jh.shxzskj.cn

[T27] Swift：错误处理
来源：http://fk.9csxet.cn

do { try f() } catch { print(error) }
来源：http://yv.yuexingan06.cn

[T28] Swift：枚举
来源：http://cf.nszjky.cn

enum Color { case red, green }
来源：http://lk.bookmarksfly.cn

[T29] Swift：guard 提前返回
来源：http://kl.hahajie.cn

guard let x = opt else { return }
来源：http://uo.szxytkj.cn

[T30] Swift：协议
来源：http://hn.muxihuayi.cn

protocol Shape { func area() -> Double }
来源：http://jr.huixinmuqiang.cn

[T31] Lua：Hello World
来源：http://sw.bjjhwx.cn

print("Hello")
来源：http://ik.shxzskj.cn

[T32] Lua：局部变量
来源：http://tx.huixiangedu.cn

local a = 1
来源：http://zr.lnxyls.cn

[T33] Lua：表（数组）
来源：http://tq.521024.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ep.asd995.cn

[T34] Lua：遍历表
来源：http://hm.huanxung.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://fb.shtwfgs.cn

[T35] Lua：字典表
来源：http://lv.shxzskj.cn

local d = { a = 1 };  d.b = 2
来源：http://og.521024.cn

[T36] Lua：函数
来源：http://bh.gzmigu.cn

function add(a, b) return a + b end
来源：http://us.huixinmuqiang.cn

[T37] Lua：字符串拼接
来源：http://ki.chemitech.net.cn

"a" .. "b"
来源：http://sz.bjjhwx.cn

[T38] Lua：条件
来源：http://mi.yuexingan06.cn

if x > 0 then print("正") end
来源：http://ld.bookmarksfly.cn

[T39] Lua：模式匹配
来源：http://iq.panjiajie.cn

string.find(s, "%d+")
来源：http://an.muxihuayi.cn

[T40] Lua：元表
来源：http://hc.gzmigu.cn

setmetatable({}, { __index = base })
来源：http://qr.jctech888.com.cn

[T41] Perl：Hello World
来源：http://ky.hahajie.cn

print "Hello\n";
来源：http://ww.nszjky.cn

[T42] Perl：变量类型
来源：http://br.bjjhwx.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lt.huixiangedu.cn

[T43] Perl：字符串插值
来源：http://ik.muxihuayi.cn

"值: $a"
来源：http://cm.wgjwhj.cn

[T44] Perl：条件
来源：http://je.shtwfgs.cn

if ($a > 0) { print "正"; }
来源：http://pv.huanxung.cn

[T45] Perl：数组遍历
来源：http://mk.jctech888.com.cn

for my $x (@arr) { print $x; }
来源：http://yh.shxzskj.cn

[T46] Perl：哈希操作
来源：http://iv.huanxung.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fn.jianghongdianzi.cn

[T47] Perl：正则捕获
来源：http://sw.9csxet.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://tl.szxytkj.cn

[T48] Perl：正则替换
来源：http://sd.newstarts.cn

$s =~ s/old/new/g;
来源：http://vu.nszjky.cn

[T49] Perl：函数
来源：http://yl.shxzskj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dg.szsharing.cn

[T50] Perl：逐行读文件
来源：http://pm.hnjuh.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://jk.bjjhwx.cn

while (my $line = <$fh>) { print $line; }
来源：http://ia.hahajie.cn

[T51] Scala：Hello World
来源：http://vq.521024.cn

println("Hello")
来源：http://lu.colortex.cn

[T52] Scala：变量
来源：http://yw.wgjwhj.cn

val a = 1;  var b = 2
来源：http://xy.lnxyls.cn

[T53] Scala：字符串插值
来源：http://ed.jianghongdianzi.cn

s"值: $b"
来源：http://ke.asd995.cn

[T54] Scala：集合映射
来源：http://vb.szxytkj.cn

List(1, 2, 3).map(_ * 2)
来源：http://mr.9csxet.cn

[T55] Scala：集合过滤
来源：http://ud.nicolike.cn

List(1, 2, 3).filter(_ > 1)
来源：http://lz.chemitech.net.cn

[T56] Scala：样例类
来源：http://zw.szsharing.cn

case class User(name: String, age: Int)
来源：http://gz.bookmarksfly.cn

[T57] Scala：模式匹配
来源：http://ey.asd995.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://la.yuexingan06.cn

[T58] Scala：函数定义
来源：http://xd.nicolike.cn

def add(a: Int, b: Int): Int = a + b
来源：http://jc.bjjhwx.cn

[T59] Scala：循环
来源：http://dh.shtwfgs.cn

for (i <- 1 to 10) println(i)
来源：http://xc.huanxung.cn

[T60] Scala：折叠
来源：http://ix.nicolike.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qa.huixiangedu.cn

================================================================================
来源：http://cv.gzmigu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cf.bookmarksfly.cn

================================================================================
来源：http://jv.szxytkj.cn

[U01] Py：创建虚拟环境
来源：http://ye.wgjwhj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://uq.lnxyls.cn

[U02] Py：导出 / 安装依赖
来源：http://pm.huixiangedu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gb.hahajie.cn

[U03] Py：加载 .env 配置
来源：http://se.9csxet.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xg.9csxet.cn

[U04] Py：变量调试打印
来源：http://kr.nicolike.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lc.bjjhwx.cn

[U05] Py：列表去重且保序
来源：http://wu.chemitech.net.cn

list(dict.fromkeys(arr))
来源：http://ya.huixinmuqiang.cn

[U06] Py：合并两个字典
来源：http://jk.huixiangedu.cn

{**a, **b}
来源：http://mu.shtwfgs.cn

[U07] Py：反转字典键值
来源：http://pd.asd995.cn

{v: k for k, v in d.items()}
来源：http://mk.panjiajie.cn

[U08] Py：展平二维列表
来源：http://fw.yuntaijiaju.cn

[y for x in nested for y in x]
来源：http://hb.szxytkj.cn

[U09] Py：字典取最大值的键
来源：http://pg.huixinmuqiang.cn

max(d, key=d.get)
来源：http://cb.huixinmuqiang.cn

[U10] Py：按值排序字典
来源：http://ci.colortex.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qw.9csxet.cn

[U11] Py：生成器表达式
来源：http://tw.bjjhwx.cn

(x * 2 for x in arr)
来源：http://qk.jctech888.com.cn

[U12] Py：取出现最多的 3 个元素
来源：http://fa.huanxung.cn

Counter(arr).most_common(3)
来源：http://ka.muxihuayi.cn

[U13] Py：固定长度队列
来源：http://ha.asd995.cn

deque(maxlen=10)
来源：http://xb.nszjky.cn

[U14] Py：分组收集到列表
来源：http://zv.bookmarksfly.cn

defaultdict(list)
来源：http://ht.panjiajie.cn

[U15] Py：高精度计时
来源：http://yu.colortex.cn

t = time.perf_counter()
来源：http://px.9csxet.cn

[U16] Py：命令行参数解析
来源：http://iu.nszjky.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://oj.huanxung.cn

[U17] Py：初始化日志
来源：http://bt.asd995.cn

logging.basicConfig(level=logging.INFO)
来源：http://vk.haigaiapp.cn

[U18] Py：预编译正则
来源：http://uf.panjiajie.cn

pat = re.compile(r"\d+")
来源：http://xx.szsharing.cn

[U19] Py：正则替换带回调
来源：http://mv.szxytkj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ho.hnjuh.cn

[U20] Py：缓存函数结果
来源：http://il.szxytkj.cn

@functools.lru_cache(maxsize=None)
来源：http://pb.huixinmuqiang.cn

[U21] Py：自定义上下文管理器
来源：http://by.gzmigu.cn

@contextlib.contextmanager
来源：http://cs.wgjwhj.cn

[U22] Py：矩阵转置
来源：http://fm.shtwfgs.cn

list(zip(*m))
来源：http://ig.9csxet.cn

[U23] Py：分块读取大文件
来源：http://lh.szsharing.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ec.huixinmuqiang.cn

[U24] Py：路径操作
来源：http://ji.huixiangedu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ru.yuexingan06.cn

[U25] Py：CSV 按字典读
来源：http://xf.nszjky.cn

csv.DictReader(f)
来源：http://mk.nszjky.cn

[U26] Py：并发下载
来源：http://mh.newstarts.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://al.shtwfgs.cn

[U27] Py：异步 HTTP
来源：http://wp.huixiangedu.cn

aiohttp.ClientSession() 配合 async with
来源：http://lp.shxzukj.cn

[U28] Py：类型别名
来源：http://mn.asd995.cn

UserId = int
来源：http://xj.wgjwhj.cn

[U29] Py：属性校验
来源：http://ws.asd995.cn

@property 与 @x.setter 配合
来源：http://dq.huixiangedu.cn

[U30] Py：数据类
来源：http://og.chemitech.net.cn

@dataclass(slots=True)
来源：http://gk.yuntaijiaju.cn

[U31] Py：单测
来源：http://vp.yuntaijiaju.cn

python -m pytest -q
来源：http://tr.newstarts.cn

[U32] Py：代码格式化
来源：http://hd.bookmarksfly.cn

ruff format . && ruff check --fix .
来源：http://mn.huixiangedu.cn

[U33] Py：打包发布
来源：http://ct.asd995.cn

python -m build  （依赖 pyproject.toml）
来源：http://rc.haigaiapp.cn

[U34] Py：判断编码
来源：http://on.nicolike.cn

chardet.detect(raw)
来源：http://ak.lnxyls.cn

[U35] Py：发送邮件
来源：http://nv.521024.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://is.9csxet.cn

[U36] Py：定时任务
来源：http://nt.jianghongdianzi.cn

schedule.every(10).minutes.do(job)
来源：http://at.wgjwhj.cn

[U37] Py：读写 Excel
来源：http://rb.521024.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ch.nicolike.cn

[U38] Py：获取脚本所在目录
来源：http://we.colortex.cn

Path(__file__).resolve().parent
来源：http://zs.shxzukj.cn

[U39] Py：判断是否在交互环境
来源：http://wd.hnjuh.cn

sys.stdout.isatty()
来源：http://ta.521024.cn

[U40] Py：打印到标准错误
来源：http://wb.jctech888.com.cn

print("err", file=sys.stderr)
来源：http://uv.yuexingan06.cn

[U41] PHP：初始化 Composer 项目
来源：http://ia.bookmarksfly.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xa.bookmarksfly.cn

[U42] PHP：PSR-4 自动加载
来源：http://ju.nszjky.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lm.shxzskj.cn

[U43] PHP：声明命名空间
来源：http://eq.yuntaijiaju.cn

namespace App\Http;
来源：http://db.shxzskj.cn

[U44] PHP：开启严格类型
来源：http://ci.huixinmuqiang.cn

declare(strict_types=1);
来源：http://ju.nicolike.cn

[U45] PHP：类型声明与返回类型
来源：http://uu.asd995.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bd.huixiangedu.cn

[U46] PHP：可空类型
来源：http://vc.haigaiapp.cn

?string $name = null
来源：http://lk.hahajie.cn

[U47] PHP：联合类型
来源：http://uf.colortex.cn

int|string $id
来源：http://ze.colortex.cn

[U48] PHP：纯枚举
来源：http://dd.jctech888.com.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tw.newstarts.cn

[U49] PHP：只读属性
来源：http://rs.gzmigu.cn

public readonly string $name
来源：http://bg.asd995.cn

[U50] PHP：构造器属性提升
来源：http://zp.huixiangedu.cn

public function __construct(private int $id) {}
来源：http://bn.hahajie.cn

[U51] PHP：数组解构
来源：http://ag.muxihuayi.cn

[$a, $b] = $arr;
来源：http://jv.asd995.cn

[U52] PHP：箭头函数
来源：http://du.shxzukj.cn

$double = fn($x) => $x * 2;
来源：http://xg.chemitech.net.cn

[U53] PHP：空合并运算符
来源：http://np.muxihuayi.cn

$v = $a ?? $b ?? "default";
来源：http://ct.szxytkj.cn

[U54] PHP：空安全调用
来源：http://ft.hnjuh.cn

$obj?->method()
来源：http://ei.lnxyls.cn

[U55] PHP：match 表达式
来源：http://bs.huixinmuqiang.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ry.muxihuayi.cn

[U56] PHP：命名参数
来源：http://cm.szsharing.cn

f(a: 1, b: 2)
来源：http://ns.nicolike.cn

[U57] PHP：字符串插值
来源：http://pe.shxzskj.cn

"值: {$a}"
来源：http://zo.yuntaijiaju.cn

[U58] PHP：数组三件套
来源：http://sp.nszjky.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bx.yuexingan06.cn

[U59] PHP：自定义排序
来源：http://co.chemitech.net.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uz.nszjky.cn

[U60] PHP：JSON 编解码
来源：http://ak.szsharing.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ei.bookmarksfly.cn

[U61] PHP：正则
来源：http://di.jianghongdianzi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pb.panjiajie.cn

[U62] PHP：日期对象
来源：http://kk.szsharing.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ht.9csxet.cn

[U63] PHP：文件读写
来源：http://li.yuntaijiaju.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bv.szxytkj.cn

[U64] PHP：目录遍历
来源：http://bt.newstarts.cn

glob("dir/*.php");  scandir("dir");
来源：http://mv.shxzukj.cn

[U65] PHP：会话
来源：http://ij.huixinmuqiang.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://be.huixiangedu.cn

[U66] PHP：设置 Cookie
来源：http://jg.muxihuayi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xq.colortex.cn

[U67] PHP：处理文件上传
来源：http://kg.szxytkj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fv.huanxung.cn

[U68] PHP：PDO 连接
来源：http://ty.haigaiapp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ky.haigaiapp.cn

[U69] PHP：PDO 预处理
来源：http://cz.wgjwhj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rp.hnjuh.cn

[U70] PHP：PDO 事务
来源：http://fw.huixiangedu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wb.muxihuayi.cn

[U71] PHP：抛出异常
来源：http://ac.panjiajie.cn

throw new RuntimeException("失败", 500);
来源：http://wq.colortex.cn

[U72] PHP：写错误日志
来源：http://rp.nicolike.cn

error_log("失败: " . $e->getMessage());
来源：http://ua.521024.cn

[U73] PHP：读取 ini 配置
来源：http://zp.muxihuayi.cn

parse_ini_file("config.ini", true)
来源：http://ih.muxihuayi.cn

[U74] PHP：读取环境变量
来源：http://tv.bjjhwx.cn

getenv("APP_ENV") ?: "production"
来源：http://ar.huanxung.cn

[U75] PHP：依赖注入
来源：http://fj.521024.cn

composer require psr/container
来源：http://ss.colortex.cn

[U76] PHP：简单路由
来源：http://qy.chemitech.net.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pr.colortex.cn

[U77] PHP：模板渲染
来源：http://nx.bjjhwx.cn

composer require twig/twig
来源：http://sf.hnjuh.cn

[U78] PHP：单元测试
来源：http://wc.huixiangedu.cn

composer require --dev phpunit/phpunit
来源：http://nq.gzmigu.cn

[U79] PHP：静态分析
来源：http://xw.panjiajie.cn

composer require --dev phpstan/phpstan
来源：http://cq.hahajie.cn

[U80] PHP：代码规范修复
来源：http://rp.shxzukj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://zf.bjjhwx.cn

[U81] JS：初始化项目
来源：http://ij.wgjwhj.cn

npm init -y;  npm i express
来源：http://rc.lnxyls.cn

[U82] JS：package.json 脚本
来源：http://rw.bjjhwx.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zy.yuexingan06.cn

[U83] JS：ES Module 导入导出
来源：http://ov.muxihuayi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ao.huanxung.cn

[U84] JS：CommonJS 写法
来源：http://lw.szxytkj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://tx.521024.cn

[U85] JS：可选链
来源：http://an.521024.cn

a?.b?.c
来源：http://iu.jctech888.com.cn

[U86] JS：空值合并
来源：http://vr.bjjhwx.cn

a ?? b
来源：http://xd.hnjuh.cn

[U87] JS：解构默认值
来源：http://sc.shtwfgs.cn

const { a = 1, b = 2 } = obj;
来源：http://qf.bookmarksfly.cn

[U88] JS：对象展开合并
来源：http://xu.haigaiapp.cn

{ ...a, ...b }
来源：http://cq.hnjuh.cn

[U89] JS：数组去重
来源：http://pb.szsharing.cn

[...new Set(arr)]
来源：http://jr.panjiajie.cn

[U90] JS：数字数组排序
来源：http://fe.wgjwhj.cn

[...arr].sort((a, b) => a - b)
来源：http://ur.jctech888.com.cn

[U91] JS：对象键值遍历
来源：http://wv.jianghongdianzi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://la.wgjwhj.cn

[U92] JS：深拷贝
来源：http://hg.chemitech.net.cn

structuredClone(obj)
来源：http://px.jianghongdianzi.cn

[U93] JS：模板字符串
来源：http://bk.huixinmuqiang.cn

`共 ${n} 条`
来源：http://ue.jianghongdianzi.cn

[U94] JS：箭头函数
来源：http://ct.wgjwhj.cn

const double = x => x * 2;
来源：http://cq.hnjuh.cn

[U95] JS：Promise 包装
来源：http://ye.haigaiapp.cn

new Promise((resolve, reject) => {})
来源：http://us.shtwfgs.cn

[U96] JS：async/await 与异常
来源：http://ga.nszjky.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xr.szxytkj.cn

[U97] JS：并发请求
来源：http://wm.shxzukj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ao.shxzskj.cn

[U98] JS：fetch 带 JSON
来源：http://bh.shxzskj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bk.muxihuayi.cn


<!-- 参考信息 -->