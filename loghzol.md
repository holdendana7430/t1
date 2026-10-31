代发 wailian999

[T21] Swift：遍历
来源：http://kt.huixiangedu.cn

for x in a { print(x) }
来源：http://pt.panjiajie.cn

[T22] Swift：字典
来源：http://qd.521024.cn

var d = ["a": 1];  d["b"] = 2
来源：http://bi.wgjwhj.cn

[T23] Swift：函数
来源：http://xo.panjiajie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cf.yuntaijiaju.cn

[T24] Swift：闭包
来源：http://ch.yuntaijiaju.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://am.shxzskj.cn

[T25] Swift：结构体
来源：http://uz.huanxung.cn

struct P { var x: Int }
来源：http://yc.panjiajie.cn

[T26] Swift：类与重写
来源：http://ux.yuntaijiaju.cn

class A: Base { override func f() {} }
来源：http://ps.szsharing.cn

[T27] Swift：错误处理
来源：http://ky.bjjhwx.cn

do { try f() } catch { print(error) }
来源：http://uv.521024.cn

[T28] Swift：枚举
来源：http://nw.yuexingan06.cn

enum Color { case red, green }
来源：http://zx.shtwfgs.cn

[T29] Swift：guard 提前返回
来源：http://xn.huixiangedu.cn

guard let x = opt else { return }
来源：http://ch.yuntaijiaju.cn

[T30] Swift：协议
来源：http://yn.huixiangedu.cn

protocol Shape { func area() -> Double }
来源：http://qb.haigaiapp.cn

[T31] Lua：Hello World
来源：http://hm.yuexingan06.cn

print("Hello")
来源：http://jl.9csxet.cn

[T32] Lua：局部变量
来源：http://df.shxzskj.cn

local a = 1
来源：http://lk.hahajie.cn

[T33] Lua：表（数组）
来源：http://wo.nicolike.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://gh.yuntaijiaju.cn

[T34] Lua：遍历表
来源：http://pk.nszjky.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zi.9csxet.cn

[T35] Lua：字典表
来源：http://vi.huixiangedu.cn

local d = { a = 1 };  d.b = 2
来源：http://uv.wgjwhj.cn

[T36] Lua：函数
来源：http://kq.jctech888.com.cn

function add(a, b) return a + b end
来源：http://bx.gzmigu.cn

[T37] Lua：字符串拼接
来源：http://ig.521024.cn

"a" .. "b"
来源：http://lv.shxzskj.cn

[T38] Lua：条件
来源：http://fi.newstarts.cn

if x > 0 then print("正") end
来源：http://rh.9csxet.cn

[T39] Lua：模式匹配
来源：http://rf.hnjuh.cn

string.find(s, "%d+")
来源：http://fd.newstarts.cn

[T40] Lua：元表
来源：http://pf.shtwfgs.cn

setmetatable({}, { __index = base })
来源：http://zd.hahajie.cn

[T41] Perl：Hello World
来源：http://oe.nszjky.cn

print "Hello\n";
来源：http://jt.shxzskj.cn

[T42] Perl：变量类型
来源：http://jw.jctech888.com.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://by.nszjky.cn

[T43] Perl：字符串插值
来源：http://mc.huixinmuqiang.cn

"值: $a"
来源：http://oe.asd995.cn

[T44] Perl：条件
来源：http://mk.szxytkj.cn

if ($a > 0) { print "正"; }
来源：http://ts.huixiangedu.cn

[T45] Perl：数组遍历
来源：http://hd.521024.cn

for my $x (@arr) { print $x; }
来源：http://gl.lnxyls.cn

[T46] Perl：哈希操作
来源：http://ie.bookmarksfly.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tb.nicolike.cn

[T47] Perl：正则捕获
来源：http://fc.hnjuh.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://yn.huixiangedu.cn

[T48] Perl：正则替换
来源：http://px.bjjhwx.cn

$s =~ s/old/new/g;
来源：http://ln.bookmarksfly.cn

[T49] Perl：函数
来源：http://fq.szsharing.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cr.chemitech.net.cn

[T50] Perl：逐行读文件
来源：http://gb.szsharing.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ky.shtwfgs.cn

while (my $line = <$fh>) { print $line; }
来源：http://tk.szxytkj.cn

[T51] Scala：Hello World
来源：http://xv.huanxung.cn

println("Hello")
来源：http://if.haigaiapp.cn

[T52] Scala：变量
来源：http://fz.shtwfgs.cn

val a = 1;  var b = 2
来源：http://vx.shxzukj.cn

[T53] Scala：字符串插值
来源：http://ex.haigaiapp.cn

s"值: $b"
来源：http://ya.colortex.cn

[T54] Scala：集合映射
来源：http://vm.bookmarksfly.cn

List(1, 2, 3).map(_ * 2)
来源：http://ce.nicolike.cn

[T55] Scala：集合过滤
来源：http://bc.shxzskj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://zv.lnxyls.cn

[T56] Scala：样例类
来源：http://no.nicolike.cn

case class User(name: String, age: Int)
来源：http://vc.nszjky.cn

[T57] Scala：模式匹配
来源：http://fn.chemitech.net.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://in.asd995.cn

[T58] Scala：函数定义
来源：http://ql.shtwfgs.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bt.nicolike.cn

[T59] Scala：循环
来源：http://ho.lnxyls.cn

for (i <- 1 to 10) println(i)
来源：http://mw.newstarts.cn

[T60] Scala：折叠
来源：http://qj.hnjuh.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yl.yuexingan06.cn

================================================================================
来源：http://pe.yuntaijiaju.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vm.hahajie.cn

================================================================================
来源：http://um.shxzskj.cn

[U01] Py：创建虚拟环境
来源：http://le.szsharing.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jv.panjiajie.cn

[U02] Py：导出 / 安装依赖
来源：http://ho.asd995.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wr.nszjky.cn

[U03] Py：加载 .env 配置
来源：http://wa.muxihuayi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://er.bjjhwx.cn

[U04] Py：变量调试打印
来源：http://of.chemitech.net.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tg.yuexingan06.cn

[U05] Py：列表去重且保序
来源：http://eg.huixinmuqiang.cn

list(dict.fromkeys(arr))
来源：http://rx.haigaiapp.cn

[U06] Py：合并两个字典
来源：http://ej.huixinmuqiang.cn

{**a, **b}
来源：http://sf.hahajie.cn

[U07] Py：反转字典键值
来源：http://tf.wgjwhj.cn

{v: k for k, v in d.items()}
来源：http://ux.nszjky.cn

[U08] Py：展平二维列表
来源：http://zm.hnjuh.cn

[y for x in nested for y in x]
来源：http://rs.hahajie.cn

[U09] Py：字典取最大值的键
来源：http://qd.shxzskj.cn

max(d, key=d.get)
来源：http://fq.hahajie.cn

[U10] Py：按值排序字典
来源：http://cd.shxzukj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qy.szsharing.cn

[U11] Py：生成器表达式
来源：http://za.newstarts.cn

(x * 2 for x in arr)
来源：http://kh.jctech888.com.cn

[U12] Py：取出现最多的 3 个元素
来源：http://sj.szxytkj.cn

Counter(arr).most_common(3)
来源：http://ht.haigaiapp.cn

[U13] Py：固定长度队列
来源：http://hm.huixiangedu.cn

deque(maxlen=10)
来源：http://hw.panjiajie.cn

[U14] Py：分组收集到列表
来源：http://zb.jctech888.com.cn

defaultdict(list)
来源：http://jt.521024.cn

[U15] Py：高精度计时
来源：http://br.huanxung.cn

t = time.perf_counter()
来源：http://fr.chemitech.net.cn

[U16] Py：命令行参数解析
来源：http://wf.newstarts.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hw.shtwfgs.cn

[U17] Py：初始化日志
来源：http://ch.huixiangedu.cn

logging.basicConfig(level=logging.INFO)
来源：http://es.huixiangedu.cn

[U18] Py：预编译正则
来源：http://zn.jianghongdianzi.cn

pat = re.compile(r"\d+")
来源：http://xn.muxihuayi.cn

[U19] Py：正则替换带回调
来源：http://hd.hnjuh.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ye.nicolike.cn

[U20] Py：缓存函数结果
来源：http://sn.wgjwhj.cn

@functools.lru_cache(maxsize=None)
来源：http://as.bookmarksfly.cn

[U21] Py：自定义上下文管理器
来源：http://gz.nicolike.cn

@contextlib.contextmanager
来源：http://jm.szsharing.cn

[U22] Py：矩阵转置
来源：http://ol.chemitech.net.cn

list(zip(*m))
来源：http://yt.hnjuh.cn

[U23] Py：分块读取大文件
来源：http://wn.bookmarksfly.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ey.bjjhwx.cn

[U24] Py：路径操作
来源：http://sy.colortex.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mm.521024.cn

[U25] Py：CSV 按字典读
来源：http://qt.panjiajie.cn

csv.DictReader(f)
来源：http://qx.jctech888.com.cn

[U26] Py：并发下载
来源：http://gr.lnxyls.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ov.haigaiapp.cn

[U27] Py：异步 HTTP
来源：http://wl.9csxet.cn

aiohttp.ClientSession() 配合 async with
来源：http://je.bookmarksfly.cn

[U28] Py：类型别名
来源：http://qj.muxihuayi.cn

UserId = int
来源：http://pf.gzmigu.cn

[U29] Py：属性校验
来源：http://vg.szsharing.cn

@property 与 @x.setter 配合
来源：http://fa.szxytkj.cn

[U30] Py：数据类
来源：http://zp.bookmarksfly.cn

@dataclass(slots=True)
来源：http://yd.nszjky.cn

[U31] Py：单测
来源：http://im.yuexingan06.cn

python -m pytest -q
来源：http://zp.szsharing.cn

[U32] Py：代码格式化
来源：http://ei.nicolike.cn

ruff format . && ruff check --fix .
来源：http://hm.nicolike.cn

[U33] Py：打包发布
来源：http://wf.lnxyls.cn

python -m build  （依赖 pyproject.toml）
来源：http://ta.bookmarksfly.cn

[U34] Py：判断编码
来源：http://ds.jctech888.com.cn

chardet.detect(raw)
来源：http://hv.nicolike.cn

[U35] Py：发送邮件
来源：http://vz.huixinmuqiang.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://be.yuntaijiaju.cn

[U36] Py：定时任务
来源：http://vj.9csxet.cn

schedule.every(10).minutes.do(job)
来源：http://su.gzmigu.cn

[U37] Py：读写 Excel
来源：http://cr.chemitech.net.cn

pandas.read_excel / DataFrame.to_excel
来源：http://pu.muxihuayi.cn

[U38] Py：获取脚本所在目录
来源：http://to.newstarts.cn

Path(__file__).resolve().parent
来源：http://ya.lnxyls.cn

[U39] Py：判断是否在交互环境
来源：http://wi.asd995.cn

sys.stdout.isatty()
来源：http://md.lnxyls.cn

[U40] Py：打印到标准错误
来源：http://oc.huanxung.cn

print("err", file=sys.stderr)
来源：http://ee.colortex.cn

[U41] PHP：初始化 Composer 项目
来源：http://gl.bjjhwx.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ud.shxzukj.cn

[U42] PHP：PSR-4 自动加载
来源：http://re.bookmarksfly.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xo.huixiangedu.cn

[U43] PHP：声明命名空间
来源：http://by.hnjuh.cn

namespace App\Http;
来源：http://kd.szxytkj.cn

[U44] PHP：开启严格类型
来源：http://ii.panjiajie.cn

declare(strict_types=1);
来源：http://sm.chemitech.net.cn

[U45] PHP：类型声明与返回类型
来源：http://br.hnjuh.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://cm.gzmigu.cn

[U46] PHP：可空类型
来源：http://nv.wgjwhj.cn

?string $name = null
来源：http://ua.bjjhwx.cn

[U47] PHP：联合类型
来源：http://ty.yuexingan06.cn

int|string $id
来源：http://pe.shtwfgs.cn

[U48] PHP：纯枚举
来源：http://hi.521024.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kr.chemitech.net.cn

[U49] PHP：只读属性
来源：http://qq.hnjuh.cn

public readonly string $name
来源：http://un.jctech888.com.cn

[U50] PHP：构造器属性提升
来源：http://rg.szxytkj.cn

public function __construct(private int $id) {}
来源：http://dt.asd995.cn

[U51] PHP：数组解构
来源：http://kc.wgjwhj.cn

[$a, $b] = $arr;
来源：http://fc.newstarts.cn

[U52] PHP：箭头函数
来源：http://rl.colortex.cn

$double = fn($x) => $x * 2;
来源：http://fm.haigaiapp.cn

[U53] PHP：空合并运算符
来源：http://ou.yuexingan06.cn

$v = $a ?? $b ?? "default";
来源：http://ux.shxzskj.cn

[U54] PHP：空安全调用
来源：http://hu.newstarts.cn

$obj?->method()
来源：http://cy.jianghongdianzi.cn

[U55] PHP：match 表达式
来源：http://um.shxzukj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lt.lnxyls.cn

[U56] PHP：命名参数
来源：http://fu.chemitech.net.cn

f(a: 1, b: 2)
来源：http://yf.szxytkj.cn

[U57] PHP：字符串插值
来源：http://vr.newstarts.cn

"值: {$a}"
来源：http://vs.lnxyls.cn

[U58] PHP：数组三件套
来源：http://bu.muxihuayi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://na.haigaiapp.cn

[U59] PHP：自定义排序
来源：http://ao.jctech888.com.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ru.yuexingan06.cn

[U60] PHP：JSON 编解码
来源：http://ku.bjjhwx.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://op.chemitech.net.cn

[U61] PHP：正则
来源：http://jy.huixinmuqiang.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lg.haigaiapp.cn

[U62] PHP：日期对象
来源：http://vr.521024.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bj.521024.cn

[U63] PHP：文件读写
来源：http://rc.shtwfgs.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tf.asd995.cn

[U64] PHP：目录遍历
来源：http://nt.huanxung.cn

glob("dir/*.php");  scandir("dir");
来源：http://be.hahajie.cn

[U65] PHP：会话
来源：http://xt.huixiangedu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://wp.hnjuh.cn

[U66] PHP：设置 Cookie
来源：http://co.muxihuayi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xv.gzmigu.cn

[U67] PHP：处理文件上传
来源：http://dn.bookmarksfly.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xc.szsharing.cn

[U68] PHP：PDO 连接
来源：http://hp.huixinmuqiang.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lv.shxzskj.cn

[U69] PHP：PDO 预处理
来源：http://nv.huixiangedu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vu.wgjwhj.cn

[U70] PHP：PDO 事务
来源：http://dv.shtwfgs.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ku.bjjhwx.cn

[U71] PHP：抛出异常
来源：http://ni.9csxet.cn

throw new RuntimeException("失败", 500);
来源：http://sw.haigaiapp.cn

[U72] PHP：写错误日志
来源：http://aj.lnxyls.cn

error_log("失败: " . $e->getMessage());
来源：http://si.lnxyls.cn

[U73] PHP：读取 ini 配置
来源：http://bw.gzmigu.cn

parse_ini_file("config.ini", true)
来源：http://xi.colortex.cn

[U74] PHP：读取环境变量
来源：http://yz.lnxyls.cn

getenv("APP_ENV") ?: "production"
来源：http://bh.haigaiapp.cn

[U75] PHP：依赖注入
来源：http://ml.huanxung.cn

composer require psr/container
来源：http://ss.hnjuh.cn

[U76] PHP：简单路由
来源：http://ak.wgjwhj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gw.gzmigu.cn

[U77] PHP：模板渲染
来源：http://kr.szsharing.cn

composer require twig/twig
来源：http://tc.shtwfgs.cn

[U78] PHP：单元测试
来源：http://lj.521024.cn

composer require --dev phpunit/phpunit
来源：http://se.lnxyls.cn

[U79] PHP：静态分析
来源：http://al.shtwfgs.cn

composer require --dev phpstan/phpstan
来源：http://wu.huixinmuqiang.cn

[U80] PHP：代码规范修复
来源：http://ek.bookmarksfly.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ki.9csxet.cn

[U81] JS：初始化项目
来源：http://gn.huixinmuqiang.cn

npm init -y;  npm i express
来源：http://zy.huixiangedu.cn

[U82] JS：package.json 脚本
来源：http://nu.hahajie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ul.hahajie.cn

[U83] JS：ES Module 导入导出
来源：http://fx.yuntaijiaju.cn

export const a = 1;  import { a } from "./m.js";
来源：http://bw.hnjuh.cn

[U84] JS：CommonJS 写法
来源：http://ye.bjjhwx.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ht.colortex.cn

[U85] JS：可选链
来源：http://tf.huanxung.cn

a?.b?.c
来源：http://qm.bjjhwx.cn

[U86] JS：空值合并
来源：http://dg.jianghongdianzi.cn

a ?? b
来源：http://ks.521024.cn

[U87] JS：解构默认值
来源：http://ct.panjiajie.cn

const { a = 1, b = 2 } = obj;
来源：http://tm.bookmarksfly.cn

[U88] JS：对象展开合并
来源：http://hj.yuntaijiaju.cn

{ ...a, ...b }
来源：http://cq.haigaiapp.cn

[U89] JS：数组去重
来源：http://jo.panjiajie.cn

[...new Set(arr)]
来源：http://ba.bjjhwx.cn

[U90] JS：数字数组排序
来源：http://lc.asd995.cn

[...arr].sort((a, b) => a - b)
来源：http://nd.bjjhwx.cn

[U91] JS：对象键值遍历
来源：http://xd.panjiajie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jg.huixiangedu.cn

[U92] JS：深拷贝
来源：http://dc.bjjhwx.cn

structuredClone(obj)
来源：http://ou.newstarts.cn

[U93] JS：模板字符串
来源：http://zi.szsharing.cn

`共 ${n} 条`
来源：http://lw.bjjhwx.cn

[U94] JS：箭头函数
来源：http://xd.colortex.cn

const double = x => x * 2;
来源：http://ql.gzmigu.cn

[U95] JS：Promise 包装
来源：http://ah.hahajie.cn

new Promise((resolve, reject) => {})
来源：http://be.huanxung.cn

[U96] JS：async/await 与异常
来源：http://mk.szsharing.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nd.huixinmuqiang.cn

[U97] JS：并发请求
来源：http://bz.hnjuh.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://tr.wgjwhj.cn

[U98] JS：fetch 带 JSON
来源：http://xp.wgjwhj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vn.szsharing.cn

[U99] JS：事件监听
来源：http://jd.lnxyls.cn

el.addEventListener("click", e => {})
来源：http://el.newstarts.cn

[U100] JS：DOM 查询
来源：http://bl.9csxet.cn

document.querySelector(".item")
来源：http://oa.newstarts.cn

[U101] JS：classList 操作
来源：http://dc.haigaiapp.cn

el.classList.toggle("active")
来源：http://tu.hahajie.cn

[U102] JS：本地存储
来源：http://no.asd995.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://sp.szsharing.cn

[U103] JS：定时器
来源：http://ho.shxzskj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fu.huanxung.cn

[U104] JS：防抖
来源：http://nq.wgjwhj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vh.muxihuayi.cn

[U105] JS：节流
来源：http://oh.haigaiapp.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qa.yuntaijiaju.cn

[U106] JS：日期格式化
来源：http://ur.huixinmuqiang.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pz.szxytkj.cn

[U107] JS：数字千分位
来源：http://re.lnxyls.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sd.huixinmuqiang.cn

[U108] JS：随机整数
来源：http://vb.521024.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jr.yuntaijiaju.cn


<!-- 参考信息 -->