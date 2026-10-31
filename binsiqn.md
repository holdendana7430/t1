代发 wailian999

[T19] Swift：可选绑定
来源：http://rm.haigaiapp.cn

if let n = opt { print(n) }
来源：http://fi.yuntaijiaju.cn

[T20] Swift：数组操作
来源：http://ht.9csxet.cn

var a = [1, 2, 3];  a.append(4)
来源：http://bq.nicolike.cn

[T21] Swift：遍历
来源：http://ix.bjjhwx.cn

for x in a { print(x) }
来源：http://hj.hahajie.cn

[T22] Swift：字典
来源：http://is.hnjuh.cn

var d = ["a": 1];  d["b"] = 2
来源：http://hi.jianghongdianzi.cn

[T23] Swift：函数
来源：http://ui.hahajie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yf.panjiajie.cn

[T24] Swift：闭包
来源：http://hc.521024.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://iz.colortex.cn

[T25] Swift：结构体
来源：http://uf.shxzukj.cn

struct P { var x: Int }
来源：http://mh.szxytkj.cn

[T26] Swift：类与重写
来源：http://kj.asd995.cn

class A: Base { override func f() {} }
来源：http://zw.szsharing.cn

[T27] Swift：错误处理
来源：http://pu.chemitech.net.cn

do { try f() } catch { print(error) }
来源：http://wy.colortex.cn

[T28] Swift：枚举
来源：http://cz.yuntaijiaju.cn

enum Color { case red, green }
来源：http://xd.hnjuh.cn

[T29] Swift：guard 提前返回
来源：http://ex.jianghongdianzi.cn

guard let x = opt else { return }
来源：http://hi.bjjhwx.cn

[T30] Swift：协议
来源：http://lb.gzmigu.cn

protocol Shape { func area() -> Double }
来源：http://ew.shxzskj.cn

[T31] Lua：Hello World
来源：http://kh.shxzskj.cn

print("Hello")
来源：http://pp.jianghongdianzi.cn

[T32] Lua：局部变量
来源：http://wi.nszjky.cn

local a = 1
来源：http://qr.bookmarksfly.cn

[T33] Lua：表（数组）
来源：http://do.hnjuh.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vk.shxzukj.cn

[T34] Lua：遍历表
来源：http://ux.521024.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://oa.szsharing.cn

[T35] Lua：字典表
来源：http://gc.colortex.cn

local d = { a = 1 };  d.b = 2
来源：http://qj.521024.cn

[T36] Lua：函数
来源：http://zd.szxytkj.cn

function add(a, b) return a + b end
来源：http://ik.huixiangedu.cn

[T37] Lua：字符串拼接
来源：http://xw.nicolike.cn

"a" .. "b"
来源：http://fp.521024.cn

[T38] Lua：条件
来源：http://gx.yuexingan06.cn

if x > 0 then print("正") end
来源：http://qt.asd995.cn

[T39] Lua：模式匹配
来源：http://jb.9csxet.cn

string.find(s, "%d+")
来源：http://zn.huixiangedu.cn

[T40] Lua：元表
来源：http://fy.jianghongdianzi.cn

setmetatable({}, { __index = base })
来源：http://un.yuntaijiaju.cn

[T41] Perl：Hello World
来源：http://kv.huixiangedu.cn

print "Hello\n";
来源：http://jf.bookmarksfly.cn

[T42] Perl：变量类型
来源：http://qu.hnjuh.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://uh.szsharing.cn

[T43] Perl：字符串插值
来源：http://bu.nszjky.cn

"值: $a"
来源：http://qp.yuexingan06.cn

[T44] Perl：条件
来源：http://kt.chemitech.net.cn

if ($a > 0) { print "正"; }
来源：http://lf.521024.cn

[T45] Perl：数组遍历
来源：http://hf.panjiajie.cn

for my $x (@arr) { print $x; }
来源：http://bl.gzmigu.cn

[T46] Perl：哈希操作
来源：http://fb.yuexingan06.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bo.jianghongdianzi.cn

[T47] Perl：正则捕获
来源：http://cv.panjiajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://fp.shxzukj.cn

[T48] Perl：正则替换
来源：http://rs.521024.cn

$s =~ s/old/new/g;
来源：http://xl.hnjuh.cn

[T49] Perl：函数
来源：http://yh.jctech888.com.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rw.panjiajie.cn

[T50] Perl：逐行读文件
来源：http://lt.colortex.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://uj.huixinmuqiang.cn

while (my $line = <$fh>) { print $line; }
来源：http://iq.huixinmuqiang.cn

[T51] Scala：Hello World
来源：http://ib.yuexingan06.cn

println("Hello")
来源：http://xj.shtwfgs.cn

[T52] Scala：变量
来源：http://vm.haigaiapp.cn

val a = 1;  var b = 2
来源：http://hx.szsharing.cn

[T53] Scala：字符串插值
来源：http://xa.hahajie.cn

s"值: $b"
来源：http://xm.yuexingan06.cn

[T54] Scala：集合映射
来源：http://vs.lnxyls.cn

List(1, 2, 3).map(_ * 2)
来源：http://vk.haigaiapp.cn

[T55] Scala：集合过滤
来源：http://xn.haigaiapp.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qa.bjjhwx.cn

[T56] Scala：样例类
来源：http://un.panjiajie.cn

case class User(name: String, age: Int)
来源：http://yp.yuntaijiaju.cn

[T57] Scala：模式匹配
来源：http://mk.muxihuayi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://qw.asd995.cn

[T58] Scala：函数定义
来源：http://tx.shxzskj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://vd.szxytkj.cn

[T59] Scala：循环
来源：http://br.asd995.cn

for (i <- 1 to 10) println(i)
来源：http://au.hnjuh.cn

[T60] Scala：折叠
来源：http://or.huixiangedu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pd.muxihuayi.cn

================================================================================
来源：http://ey.nszjky.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sq.huanxung.cn

================================================================================
来源：http://ip.szxytkj.cn

[U01] Py：创建虚拟环境
来源：http://tq.colortex.cn

python -m venv .venv && source .venv/bin/activate
来源：http://do.nszjky.cn

[U02] Py：导出 / 安装依赖
来源：http://ib.gzmigu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ds.haigaiapp.cn

[U03] Py：加载 .env 配置
来源：http://yy.huanxung.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://sz.huanxung.cn

[U04] Py：变量调试打印
来源：http://rg.newstarts.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kb.chemitech.net.cn

[U05] Py：列表去重且保序
来源：http://pr.haigaiapp.cn

list(dict.fromkeys(arr))
来源：http://vr.521024.cn

[U06] Py：合并两个字典
来源：http://lf.gzmigu.cn

{**a, **b}
来源：http://ee.shxzskj.cn

[U07] Py：反转字典键值
来源：http://kv.bookmarksfly.cn

{v: k for k, v in d.items()}
来源：http://td.shxzskj.cn

[U08] Py：展平二维列表
来源：http://uk.jianghongdianzi.cn

[y for x in nested for y in x]
来源：http://zy.hahajie.cn

[U09] Py：字典取最大值的键
来源：http://ha.haigaiapp.cn

max(d, key=d.get)
来源：http://zq.lnxyls.cn

[U10] Py：按值排序字典
来源：http://yf.yuntaijiaju.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gd.shtwfgs.cn

[U11] Py：生成器表达式
来源：http://ma.asd995.cn

(x * 2 for x in arr)
来源：http://vb.wgjwhj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rr.asd995.cn

Counter(arr).most_common(3)
来源：http://lf.shtwfgs.cn

[U13] Py：固定长度队列
来源：http://gl.yuntaijiaju.cn

deque(maxlen=10)
来源：http://sq.jctech888.com.cn

[U14] Py：分组收集到列表
来源：http://xo.gzmigu.cn

defaultdict(list)
来源：http://wh.colortex.cn

[U15] Py：高精度计时
来源：http://ga.newstarts.cn

t = time.perf_counter()
来源：http://ej.chemitech.net.cn

[U16] Py：命令行参数解析
来源：http://id.szxytkj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://la.wgjwhj.cn

[U17] Py：初始化日志
来源：http://nm.yuntaijiaju.cn

logging.basicConfig(level=logging.INFO)
来源：http://oz.huanxung.cn

[U18] Py：预编译正则
来源：http://fa.muxihuayi.cn

pat = re.compile(r"\d+")
来源：http://qv.huixiangedu.cn

[U19] Py：正则替换带回调
来源：http://pg.bookmarksfly.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xa.shxzskj.cn

[U20] Py：缓存函数结果
来源：http://pd.gzmigu.cn

@functools.lru_cache(maxsize=None)
来源：http://ma.9csxet.cn

[U21] Py：自定义上下文管理器
来源：http://lb.yuntaijiaju.cn

@contextlib.contextmanager
来源：http://gb.jianghongdianzi.cn

[U22] Py：矩阵转置
来源：http://va.muxihuayi.cn

list(zip(*m))
来源：http://jm.colortex.cn

[U23] Py：分块读取大文件
来源：http://oz.nszjky.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://iq.gzmigu.cn

[U24] Py：路径操作
来源：http://ja.huixinmuqiang.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bf.szsharing.cn

[U25] Py：CSV 按字典读
来源：http://pe.nszjky.cn

csv.DictReader(f)
来源：http://cu.shtwfgs.cn

[U26] Py：并发下载
来源：http://sj.yuntaijiaju.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zo.newstarts.cn

[U27] Py：异步 HTTP
来源：http://df.bjjhwx.cn

aiohttp.ClientSession() 配合 async with
来源：http://sp.colortex.cn

[U28] Py：类型别名
来源：http://kk.shtwfgs.cn

UserId = int
来源：http://oj.bjjhwx.cn

[U29] Py：属性校验
来源：http://kx.huanxung.cn

@property 与 @x.setter 配合
来源：http://sc.haigaiapp.cn

[U30] Py：数据类
来源：http://gq.lnxyls.cn

@dataclass(slots=True)
来源：http://zk.nicolike.cn

[U31] Py：单测
来源：http://ch.shxzukj.cn

python -m pytest -q
来源：http://tk.panjiajie.cn

[U32] Py：代码格式化
来源：http://nd.panjiajie.cn

ruff format . && ruff check --fix .
来源：http://qm.bookmarksfly.cn

[U33] Py：打包发布
来源：http://tt.bookmarksfly.cn

python -m build  （依赖 pyproject.toml）
来源：http://kb.wgjwhj.cn

[U34] Py：判断编码
来源：http://fd.newstarts.cn

chardet.detect(raw)
来源：http://ql.colortex.cn

[U35] Py：发送邮件
来源：http://rn.yuntaijiaju.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yo.jianghongdianzi.cn

[U36] Py：定时任务
来源：http://en.asd995.cn

schedule.every(10).minutes.do(job)
来源：http://ua.nszjky.cn

[U37] Py：读写 Excel
来源：http://mf.lnxyls.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ca.9csxet.cn

[U38] Py：获取脚本所在目录
来源：http://qw.wgjwhj.cn

Path(__file__).resolve().parent
来源：http://du.bookmarksfly.cn

[U39] Py：判断是否在交互环境
来源：http://sw.szsharing.cn

sys.stdout.isatty()
来源：http://lk.gzmigu.cn

[U40] Py：打印到标准错误
来源：http://kq.wgjwhj.cn

print("err", file=sys.stderr)
来源：http://oj.haigaiapp.cn

[U41] PHP：初始化 Composer 项目
来源：http://rv.panjiajie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://mf.hahajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://tz.huanxung.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pe.shxzskj.cn

[U43] PHP：声明命名空间
来源：http://fk.yuntaijiaju.cn

namespace App\Http;
来源：http://rt.yuntaijiaju.cn

[U44] PHP：开启严格类型
来源：http://na.jctech888.com.cn

declare(strict_types=1);
来源：http://po.bookmarksfly.cn

[U45] PHP：类型声明与返回类型
来源：http://lh.colortex.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://sj.huixiangedu.cn

[U46] PHP：可空类型
来源：http://it.gzmigu.cn

?string $name = null
来源：http://rt.gzmigu.cn

[U47] PHP：联合类型
来源：http://pp.muxihuayi.cn

int|string $id
来源：http://yo.jctech888.com.cn

[U48] PHP：纯枚举
来源：http://hv.lnxyls.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xl.shxzskj.cn

[U49] PHP：只读属性
来源：http://hw.gzmigu.cn

public readonly string $name
来源：http://bt.lnxyls.cn

[U50] PHP：构造器属性提升
来源：http://xg.colortex.cn

public function __construct(private int $id) {}
来源：http://ro.bookmarksfly.cn

[U51] PHP：数组解构
来源：http://jy.wgjwhj.cn

[$a, $b] = $arr;
来源：http://qa.szsharing.cn

[U52] PHP：箭头函数
来源：http://ow.lnxyls.cn

$double = fn($x) => $x * 2;
来源：http://ht.jianghongdianzi.cn

[U53] PHP：空合并运算符
来源：http://aj.shxzskj.cn

$v = $a ?? $b ?? "default";
来源：http://uq.haigaiapp.cn

[U54] PHP：空安全调用
来源：http://xi.huanxung.cn

$obj?->method()
来源：http://qv.jctech888.com.cn

[U55] PHP：match 表达式
来源：http://sz.chemitech.net.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tm.newstarts.cn

[U56] PHP：命名参数
来源：http://et.yuexingan06.cn

f(a: 1, b: 2)
来源：http://sd.bjjhwx.cn

[U57] PHP：字符串插值
来源：http://pe.huixinmuqiang.cn

"值: {$a}"
来源：http://ej.jctech888.com.cn

[U58] PHP：数组三件套
来源：http://ih.szsharing.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pk.hnjuh.cn

[U59] PHP：自定义排序
来源：http://bk.shxzskj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ed.yuntaijiaju.cn

[U60] PHP：JSON 编解码
来源：http://eb.bjjhwx.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zl.huixinmuqiang.cn

[U61] PHP：正则
来源：http://ji.bjjhwx.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jj.bjjhwx.cn

[U62] PHP：日期对象
来源：http://cw.521024.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sa.colortex.cn

[U63] PHP：文件读写
来源：http://zv.huanxung.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vy.szsharing.cn

[U64] PHP：目录遍历
来源：http://fb.muxihuayi.cn

glob("dir/*.php");  scandir("dir");
来源：http://ut.yuexingan06.cn

[U65] PHP：会话
来源：http://oh.yuntaijiaju.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vw.yuexingan06.cn

[U66] PHP：设置 Cookie
来源：http://pz.newstarts.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hb.521024.cn

[U67] PHP：处理文件上传
来源：http://hv.yuexingan06.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kz.9csxet.cn

[U68] PHP：PDO 连接
来源：http://mj.szxytkj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wj.bjjhwx.cn

[U69] PHP：PDO 预处理
来源：http://xr.huixinmuqiang.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rw.szsharing.cn

[U70] PHP：PDO 事务
来源：http://qg.jctech888.com.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xn.szxytkj.cn

[U71] PHP：抛出异常
来源：http://zr.asd995.cn

throw new RuntimeException("失败", 500);
来源：http://hq.nicolike.cn

[U72] PHP：写错误日志
来源：http://hs.shxzukj.cn

error_log("失败: " . $e->getMessage());
来源：http://hq.nszjky.cn

[U73] PHP：读取 ini 配置
来源：http://dz.huixinmuqiang.cn

parse_ini_file("config.ini", true)
来源：http://hn.huixinmuqiang.cn

[U74] PHP：读取环境变量
来源：http://ul.huanxung.cn

getenv("APP_ENV") ?: "production"
来源：http://lj.panjiajie.cn

[U75] PHP：依赖注入
来源：http://mu.shtwfgs.cn

composer require psr/container
来源：http://tj.asd995.cn

[U76] PHP：简单路由
来源：http://qg.huanxung.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ye.muxihuayi.cn

[U77] PHP：模板渲染
来源：http://jq.szxytkj.cn

composer require twig/twig
来源：http://yo.muxihuayi.cn

[U78] PHP：单元测试
来源：http://fw.hnjuh.cn

composer require --dev phpunit/phpunit
来源：http://bj.colortex.cn

[U79] PHP：静态分析
来源：http://jr.huanxung.cn

composer require --dev phpstan/phpstan
来源：http://es.bookmarksfly.cn

[U80] PHP：代码规范修复
来源：http://tn.nicolike.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ld.chemitech.net.cn

[U81] JS：初始化项目
来源：http://wj.hahajie.cn

npm init -y;  npm i express
来源：http://by.nszjky.cn

[U82] JS：package.json 脚本
来源：http://jj.szsharing.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://la.shtwfgs.cn

[U83] JS：ES Module 导入导出
来源：http://wt.huixiangedu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zj.shxzskj.cn

[U84] JS：CommonJS 写法
来源：http://hx.hnjuh.cn

module.exports = { a };  const { a } = require("./m");
来源：http://vo.bjjhwx.cn

[U85] JS：可选链
来源：http://wp.huixinmuqiang.cn

a?.b?.c
来源：http://wo.bjjhwx.cn

[U86] JS：空值合并
来源：http://wg.huanxung.cn

a ?? b
来源：http://bn.9csxet.cn

[U87] JS：解构默认值
来源：http://jk.yuexingan06.cn

const { a = 1, b = 2 } = obj;
来源：http://dd.shtwfgs.cn

[U88] JS：对象展开合并
来源：http://dv.huanxung.cn

{ ...a, ...b }
来源：http://em.huixiangedu.cn

[U89] JS：数组去重
来源：http://cs.huixiangedu.cn

[...new Set(arr)]
来源：http://gk.muxihuayi.cn

[U90] JS：数字数组排序
来源：http://ej.shxzukj.cn

[...arr].sort((a, b) => a - b)
来源：http://ah.panjiajie.cn

[U91] JS：对象键值遍历
来源：http://kj.shxzukj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://an.shxzukj.cn

[U92] JS：深拷贝
来源：http://ur.haigaiapp.cn

structuredClone(obj)
来源：http://qt.9csxet.cn

[U93] JS：模板字符串
来源：http://yh.huixiangedu.cn

`共 ${n} 条`
来源：http://at.521024.cn

[U94] JS：箭头函数
来源：http://zm.haigaiapp.cn

const double = x => x * 2;
来源：http://vy.newstarts.cn

[U95] JS：Promise 包装
来源：http://cr.nicolike.cn

new Promise((resolve, reject) => {})
来源：http://qh.521024.cn

[U96] JS：async/await 与异常
来源：http://zk.huixiangedu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vz.9csxet.cn

[U97] JS：并发请求
来源：http://ex.lnxyls.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zu.panjiajie.cn

[U98] JS：fetch 带 JSON
来源：http://sv.asd995.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ph.muxihuayi.cn

[U99] JS：事件监听
来源：http://ob.huixinmuqiang.cn

el.addEventListener("click", e => {})
来源：http://bw.wgjwhj.cn

[U100] JS：DOM 查询
来源：http://fq.521024.cn

document.querySelector(".item")
来源：http://lk.yuntaijiaju.cn

[U101] JS：classList 操作
来源：http://ui.muxihuayi.cn

el.classList.toggle("active")
来源：http://iu.jctech888.com.cn

[U102] JS：本地存储
来源：http://gs.hahajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://vk.chemitech.net.cn

[U103] JS：定时器
来源：http://pt.jianghongdianzi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lx.panjiajie.cn

[U104] JS：防抖
来源：http://zw.jianghongdianzi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jc.szxytkj.cn

[U105] JS：节流
来源：http://pv.panjiajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://at.huixinmuqiang.cn

[U106] JS：日期格式化
来源：http://rz.gzmigu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yz.shxzskj.cn


<!-- 参考信息 -->