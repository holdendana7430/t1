代发 wailian999

[T17] Swift：变量与常量
来源：http://zg.shtwfgs.cn

var a = 1;  let b = 2
来源：http://fx.hnjuh.cn

[T18] Swift：字符串插值
来源：http://cp.haigaiapp.cn

"值: \(b)"
来源：http://kt.szxytkj.cn

[T19] Swift：可选绑定
来源：http://uv.wgjwhj.cn

if let n = opt { print(n) }
来源：http://el.hnjuh.cn

[T20] Swift：数组操作
来源：http://ez.haigaiapp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://tj.huixiangedu.cn

[T21] Swift：遍历
来源：http://bs.panjiajie.cn

for x in a { print(x) }
来源：http://ia.szsharing.cn

[T22] Swift：字典
来源：http://ya.gzmigu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vv.nicolike.cn

[T23] Swift：函数
来源：http://fy.hahajie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ts.newstarts.cn

[T24] Swift：闭包
来源：http://bx.chemitech.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ss.yuexingan06.cn

[T25] Swift：结构体
来源：http://oc.szsharing.cn

struct P { var x: Int }
来源：http://ta.muxihuayi.cn

[T26] Swift：类与重写
来源：http://um.huixiangedu.cn

class A: Base { override func f() {} }
来源：http://il.wgjwhj.cn

[T27] Swift：错误处理
来源：http://ed.shxzskj.cn

do { try f() } catch { print(error) }
来源：http://jb.huixinmuqiang.cn

[T28] Swift：枚举
来源：http://bg.colortex.cn

enum Color { case red, green }
来源：http://we.huixiangedu.cn

[T29] Swift：guard 提前返回
来源：http://lf.panjiajie.cn

guard let x = opt else { return }
来源：http://xp.jctech888.com.cn

[T30] Swift：协议
来源：http://gf.jianghongdianzi.cn

protocol Shape { func area() -> Double }
来源：http://eg.bjjhwx.cn

[T31] Lua：Hello World
来源：http://oi.hahajie.cn

print("Hello")
来源：http://ji.521024.cn

[T32] Lua：局部变量
来源：http://jj.szsharing.cn

local a = 1
来源：http://ex.asd995.cn

[T33] Lua：表（数组）
来源：http://mn.lnxyls.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fg.szxytkj.cn

[T34] Lua：遍历表
来源：http://bc.muxihuayi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rj.wgjwhj.cn

[T35] Lua：字典表
来源：http://he.hnjuh.cn

local d = { a = 1 };  d.b = 2
来源：http://cl.szsharing.cn

[T36] Lua：函数
来源：http://ez.yuntaijiaju.cn

function add(a, b) return a + b end
来源：http://zq.521024.cn

[T37] Lua：字符串拼接
来源：http://xr.lnxyls.cn

"a" .. "b"
来源：http://dy.jianghongdianzi.cn

[T38] Lua：条件
来源：http://rj.haigaiapp.cn

if x > 0 then print("正") end
来源：http://ed.panjiajie.cn

[T39] Lua：模式匹配
来源：http://yo.muxihuayi.cn

string.find(s, "%d+")
来源：http://st.521024.cn

[T40] Lua：元表
来源：http://hp.jianghongdianzi.cn

setmetatable({}, { __index = base })
来源：http://uy.yuexingan06.cn

[T41] Perl：Hello World
来源：http://tc.szsharing.cn

print "Hello\n";
来源：http://jp.hnjuh.cn

[T42] Perl：变量类型
来源：http://rm.huanxung.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://su.gzmigu.cn

[T43] Perl：字符串插值
来源：http://sa.yuexingan06.cn

"值: $a"
来源：http://pf.huanxung.cn

[T44] Perl：条件
来源：http://pp.szsharing.cn

if ($a > 0) { print "正"; }
来源：http://ag.szsharing.cn

[T45] Perl：数组遍历
来源：http://ze.newstarts.cn

for my $x (@arr) { print $x; }
来源：http://rf.gzmigu.cn

[T46] Perl：哈希操作
来源：http://ll.521024.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ra.haigaiapp.cn

[T47] Perl：正则捕获
来源：http://ru.yuexingan06.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://le.nszjky.cn

[T48] Perl：正则替换
来源：http://cr.huixinmuqiang.cn

$s =~ s/old/new/g;
来源：http://cd.haigaiapp.cn

[T49] Perl：函数
来源：http://wf.gzmigu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qf.jctech888.com.cn

[T50] Perl：逐行读文件
来源：http://si.haigaiapp.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://yf.newstarts.cn

while (my $line = <$fh>) { print $line; }
来源：http://ih.wgjwhj.cn

[T51] Scala：Hello World
来源：http://wh.gzmigu.cn

println("Hello")
来源：http://hq.szxytkj.cn

[T52] Scala：变量
来源：http://xt.hahajie.cn

val a = 1;  var b = 2
来源：http://na.nicolike.cn

[T53] Scala：字符串插值
来源：http://jl.shxzukj.cn

s"值: $b"
来源：http://uz.hnjuh.cn

[T54] Scala：集合映射
来源：http://qi.panjiajie.cn

List(1, 2, 3).map(_ * 2)
来源：http://gj.bookmarksfly.cn

[T55] Scala：集合过滤
来源：http://zg.shxzukj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://df.bookmarksfly.cn

[T56] Scala：样例类
来源：http://ee.shxzukj.cn

case class User(name: String, age: Int)
来源：http://bu.hahajie.cn

[T57] Scala：模式匹配
来源：http://fi.huixiangedu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fi.nicolike.cn

[T58] Scala：函数定义
来源：http://br.shxzskj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://dr.muxihuayi.cn

[T59] Scala：循环
来源：http://np.haigaiapp.cn

for (i <- 1 to 10) println(i)
来源：http://vm.jctech888.com.cn

[T60] Scala：折叠
来源：http://ni.huixiangedu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ar.newstarts.cn

================================================================================
来源：http://sj.hnjuh.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tq.shxzskj.cn

================================================================================
来源：http://ww.huanxung.cn

[U01] Py：创建虚拟环境
来源：http://td.bookmarksfly.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mw.nszjky.cn

[U02] Py：导出 / 安装依赖
来源：http://nf.huixiangedu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rj.hahajie.cn

[U03] Py：加载 .env 配置
来源：http://fn.bookmarksfly.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qd.9csxet.cn

[U04] Py：变量调试打印
来源：http://ty.9csxet.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ew.wgjwhj.cn

[U05] Py：列表去重且保序
来源：http://oo.wgjwhj.cn

list(dict.fromkeys(arr))
来源：http://ya.hahajie.cn

[U06] Py：合并两个字典
来源：http://fb.szxytkj.cn

{**a, **b}
来源：http://sd.9csxet.cn

[U07] Py：反转字典键值
来源：http://pq.hahajie.cn

{v: k for k, v in d.items()}
来源：http://ov.panjiajie.cn

[U08] Py：展平二维列表
来源：http://yo.jctech888.com.cn

[y for x in nested for y in x]
来源：http://pt.panjiajie.cn

[U09] Py：字典取最大值的键
来源：http://bg.9csxet.cn

max(d, key=d.get)
来源：http://vd.bookmarksfly.cn

[U10] Py：按值排序字典
来源：http://bg.asd995.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tx.szsharing.cn

[U11] Py：生成器表达式
来源：http://rr.lnxyls.cn

(x * 2 for x in arr)
来源：http://ar.shxzskj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://it.shxzukj.cn

Counter(arr).most_common(3)
来源：http://ig.bookmarksfly.cn

[U13] Py：固定长度队列
来源：http://am.huixiangedu.cn

deque(maxlen=10)
来源：http://wb.asd995.cn

[U14] Py：分组收集到列表
来源：http://ro.yuexingan06.cn

defaultdict(list)
来源：http://xb.jianghongdianzi.cn

[U15] Py：高精度计时
来源：http://ll.521024.cn

t = time.perf_counter()
来源：http://oy.newstarts.cn

[U16] Py：命令行参数解析
来源：http://zl.jianghongdianzi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hd.shxzukj.cn

[U17] Py：初始化日志
来源：http://ry.jctech888.com.cn

logging.basicConfig(level=logging.INFO)
来源：http://cs.colortex.cn

[U18] Py：预编译正则
来源：http://cl.shtwfgs.cn

pat = re.compile(r"\d+")
来源：http://zs.wgjwhj.cn

[U19] Py：正则替换带回调
来源：http://ac.chemitech.net.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wa.bookmarksfly.cn

[U20] Py：缓存函数结果
来源：http://lw.nicolike.cn

@functools.lru_cache(maxsize=None)
来源：http://ff.asd995.cn

[U21] Py：自定义上下文管理器
来源：http://vo.muxihuayi.cn

@contextlib.contextmanager
来源：http://ok.nicolike.cn

[U22] Py：矩阵转置
来源：http://sb.jianghongdianzi.cn

list(zip(*m))
来源：http://qq.huanxung.cn

[U23] Py：分块读取大文件
来源：http://gj.bjjhwx.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zr.wgjwhj.cn

[U24] Py：路径操作
来源：http://yk.lnxyls.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hx.huanxung.cn

[U25] Py：CSV 按字典读
来源：http://nt.nszjky.cn

csv.DictReader(f)
来源：http://yi.chemitech.net.cn

[U26] Py：并发下载
来源：http://yd.colortex.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wh.yuexingan06.cn

[U27] Py：异步 HTTP
来源：http://el.szsharing.cn

aiohttp.ClientSession() 配合 async with
来源：http://nn.chemitech.net.cn

[U28] Py：类型别名
来源：http://jy.9csxet.cn

UserId = int
来源：http://qk.newstarts.cn

[U29] Py：属性校验
来源：http://bl.yuntaijiaju.cn

@property 与 @x.setter 配合
来源：http://ku.asd995.cn

[U30] Py：数据类
来源：http://ar.yuntaijiaju.cn

@dataclass(slots=True)
来源：http://bn.panjiajie.cn

[U31] Py：单测
来源：http://af.haigaiapp.cn

python -m pytest -q
来源：http://hy.szxytkj.cn

[U32] Py：代码格式化
来源：http://ep.panjiajie.cn

ruff format . && ruff check --fix .
来源：http://fh.wgjwhj.cn

[U33] Py：打包发布
来源：http://gd.hahajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://hh.shxzukj.cn

[U34] Py：判断编码
来源：http://yc.9csxet.cn

chardet.detect(raw)
来源：http://cj.newstarts.cn

[U35] Py：发送邮件
来源：http://rb.szsharing.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fh.shtwfgs.cn

[U36] Py：定时任务
来源：http://vh.yuexingan06.cn

schedule.every(10).minutes.do(job)
来源：http://or.huixinmuqiang.cn

[U37] Py：读写 Excel
来源：http://os.huixiangedu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ov.gzmigu.cn

[U38] Py：获取脚本所在目录
来源：http://xk.newstarts.cn

Path(__file__).resolve().parent
来源：http://mb.szsharing.cn

[U39] Py：判断是否在交互环境
来源：http://ff.wgjwhj.cn

sys.stdout.isatty()
来源：http://gj.wgjwhj.cn

[U40] Py：打印到标准错误
来源：http://yq.hnjuh.cn

print("err", file=sys.stderr)
来源：http://xw.szxytkj.cn

[U41] PHP：初始化 Composer 项目
来源：http://zs.huixinmuqiang.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ag.bookmarksfly.cn

[U42] PHP：PSR-4 自动加载
来源：http://tz.colortex.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ye.shxzukj.cn

[U43] PHP：声明命名空间
来源：http://zj.haigaiapp.cn

namespace App\Http;
来源：http://xo.huixiangedu.cn

[U44] PHP：开启严格类型
来源：http://xu.jctech888.com.cn

declare(strict_types=1);
来源：http://wc.hnjuh.cn

[U45] PHP：类型声明与返回类型
来源：http://zk.hnjuh.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://oi.nszjky.cn

[U46] PHP：可空类型
来源：http://fh.bookmarksfly.cn

?string $name = null
来源：http://qk.shxzskj.cn

[U47] PHP：联合类型
来源：http://lg.gzmigu.cn

int|string $id
来源：http://fo.hahajie.cn

[U48] PHP：纯枚举
来源：http://sg.yuexingan06.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hr.huixiangedu.cn

[U49] PHP：只读属性
来源：http://ia.521024.cn

public readonly string $name
来源：http://th.9csxet.cn

[U50] PHP：构造器属性提升
来源：http://ez.yuexingan06.cn

public function __construct(private int $id) {}
来源：http://ba.panjiajie.cn

[U51] PHP：数组解构
来源：http://zy.yuexingan06.cn

[$a, $b] = $arr;
来源：http://lk.szsharing.cn

[U52] PHP：箭头函数
来源：http://ac.panjiajie.cn

$double = fn($x) => $x * 2;
来源：http://am.colortex.cn

[U53] PHP：空合并运算符
来源：http://ul.colortex.cn

$v = $a ?? $b ?? "default";
来源：http://pf.jctech888.com.cn

[U54] PHP：空安全调用
来源：http://tn.jctech888.com.cn

$obj?->method()
来源：http://ud.szxytkj.cn

[U55] PHP：match 表达式
来源：http://fb.wgjwhj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jr.hnjuh.cn

[U56] PHP：命名参数
来源：http://lk.chemitech.net.cn

f(a: 1, b: 2)
来源：http://kj.shxzukj.cn

[U57] PHP：字符串插值
来源：http://gm.gzmigu.cn

"值: {$a}"
来源：http://lv.gzmigu.cn

[U58] PHP：数组三件套
来源：http://ks.9csxet.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yk.jianghongdianzi.cn

[U59] PHP：自定义排序
来源：http://wo.nszjky.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sm.521024.cn

[U60] PHP：JSON 编解码
来源：http://mz.yuexingan06.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xh.haigaiapp.cn

[U61] PHP：正则
来源：http://fa.wgjwhj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qe.szsharing.cn

[U62] PHP：日期对象
来源：http://ne.newstarts.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cs.bookmarksfly.cn

[U63] PHP：文件读写
来源：http://fo.muxihuayi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vx.yuntaijiaju.cn

[U64] PHP：目录遍历
来源：http://ii.chemitech.net.cn

glob("dir/*.php");  scandir("dir");
来源：http://vp.bookmarksfly.cn

[U65] PHP：会话
来源：http://mg.shtwfgs.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kg.shtwfgs.cn

[U66] PHP：设置 Cookie
来源：http://gi.yuntaijiaju.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jk.haigaiapp.cn

[U67] PHP：处理文件上传
来源：http://bg.yuexingan06.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yo.wgjwhj.cn

[U68] PHP：PDO 连接
来源：http://ev.bookmarksfly.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pt.521024.cn

[U69] PHP：PDO 预处理
来源：http://cb.521024.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jm.muxihuayi.cn

[U70] PHP：PDO 事务
来源：http://ya.muxihuayi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cy.szxytkj.cn

[U71] PHP：抛出异常
来源：http://lh.hahajie.cn

throw new RuntimeException("失败", 500);
来源：http://al.nszjky.cn

[U72] PHP：写错误日志
来源：http://hc.yuntaijiaju.cn

error_log("失败: " . $e->getMessage());
来源：http://th.bookmarksfly.cn

[U73] PHP：读取 ini 配置
来源：http://zp.wgjwhj.cn

parse_ini_file("config.ini", true)
来源：http://ul.asd995.cn

[U74] PHP：读取环境变量
来源：http://mp.asd995.cn

getenv("APP_ENV") ?: "production"
来源：http://pk.hnjuh.cn

[U75] PHP：依赖注入
来源：http://jv.chemitech.net.cn

composer require psr/container
来源：http://jr.colortex.cn

[U76] PHP：简单路由
来源：http://op.wgjwhj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pg.colortex.cn

[U77] PHP：模板渲染
来源：http://lh.chemitech.net.cn

composer require twig/twig
来源：http://tj.9csxet.cn

[U78] PHP：单元测试
来源：http://gq.shxzukj.cn

composer require --dev phpunit/phpunit
来源：http://ya.shxzukj.cn

[U79] PHP：静态分析
来源：http://jv.bjjhwx.cn

composer require --dev phpstan/phpstan
来源：http://pt.shtwfgs.cn

[U80] PHP：代码规范修复
来源：http://yf.9csxet.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://mc.shxzskj.cn

[U81] JS：初始化项目
来源：http://gs.muxihuayi.cn

npm init -y;  npm i express
来源：http://ut.szxytkj.cn

[U82] JS：package.json 脚本
来源：http://io.shxzukj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ik.shxzskj.cn

[U83] JS：ES Module 导入导出
来源：http://ip.szsharing.cn

export const a = 1;  import { a } from "./m.js";
来源：http://gt.szxytkj.cn

[U84] JS：CommonJS 写法
来源：http://sv.yuexingan06.cn

module.exports = { a };  const { a } = require("./m");
来源：http://eu.panjiajie.cn

[U85] JS：可选链
来源：http://yu.jianghongdianzi.cn

a?.b?.c
来源：http://hw.9csxet.cn

[U86] JS：空值合并
来源：http://tl.szxytkj.cn

a ?? b
来源：http://tu.szsharing.cn

[U87] JS：解构默认值
来源：http://ny.nszjky.cn

const { a = 1, b = 2 } = obj;
来源：http://pf.huixiangedu.cn

[U88] JS：对象展开合并
来源：http://hi.lnxyls.cn

{ ...a, ...b }
来源：http://zz.nszjky.cn

[U89] JS：数组去重
来源：http://tc.huanxung.cn

[...new Set(arr)]
来源：http://nu.nicolike.cn

[U90] JS：数字数组排序
来源：http://ms.jctech888.com.cn

[...arr].sort((a, b) => a - b)
来源：http://ig.hahajie.cn

[U91] JS：对象键值遍历
来源：http://le.haigaiapp.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dh.hnjuh.cn

[U92] JS：深拷贝
来源：http://qg.bjjhwx.cn

structuredClone(obj)
来源：http://id.521024.cn

[U93] JS：模板字符串
来源：http://nt.lnxyls.cn

`共 ${n} 条`
来源：http://jk.jctech888.com.cn

[U94] JS：箭头函数
来源：http://jv.szsharing.cn

const double = x => x * 2;
来源：http://di.colortex.cn

[U95] JS：Promise 包装
来源：http://rc.bookmarksfly.cn

new Promise((resolve, reject) => {})
来源：http://ui.chemitech.net.cn

[U96] JS：async/await 与异常
来源：http://la.wgjwhj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vx.jianghongdianzi.cn

[U97] JS：并发请求
来源：http://ng.panjiajie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://au.bjjhwx.cn

[U98] JS：fetch 带 JSON
来源：http://rz.panjiajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ql.huixinmuqiang.cn

[U99] JS：事件监听
来源：http://ok.jianghongdianzi.cn

el.addEventListener("click", e => {})
来源：http://ao.huixinmuqiang.cn

[U100] JS：DOM 查询
来源：http://al.colortex.cn

document.querySelector(".item")
来源：http://tw.nicolike.cn

[U101] JS：classList 操作
来源：http://xw.jctech888.com.cn

el.classList.toggle("active")
来源：http://ka.wgjwhj.cn

[U102] JS：本地存储
来源：http://is.wgjwhj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://sx.jianghongdianzi.cn

[U103] JS：定时器
来源：http://wi.newstarts.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fu.muxihuayi.cn

[U104] JS：防抖
来源：http://qx.yuexingan06.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sb.nicolike.cn


<!-- 参考信息 -->