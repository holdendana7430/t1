代发 wailian999

[T27] Swift：错误处理
来源：http://yu.newstarts.cn

do { try f() } catch { print(error) }
来源：http://vu.nicolike.cn

[T28] Swift：枚举
来源：http://yh.shtwfgs.cn

enum Color { case red, green }
来源：http://nk.haigaiapp.cn

[T29] Swift：guard 提前返回
来源：http://cl.yuexingan06.cn

guard let x = opt else { return }
来源：http://ch.jianghongdianzi.cn

[T30] Swift：协议
来源：http://cd.wgjwhj.cn

protocol Shape { func area() -> Double }
来源：http://ss.panjiajie.cn

[T31] Lua：Hello World
来源：http://cz.shtwfgs.cn

print("Hello")
来源：http://ox.yuexingan06.cn

[T32] Lua：局部变量
来源：http://nb.shxzukj.cn

local a = 1
来源：http://ue.yuntaijiaju.cn

[T33] Lua：表（数组）
来源：http://bk.haigaiapp.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ee.yuntaijiaju.cn

[T34] Lua：遍历表
来源：http://gt.huixiangedu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://or.huixiangedu.cn

[T35] Lua：字典表
来源：http://jk.huixinmuqiang.cn

local d = { a = 1 };  d.b = 2
来源：http://my.lnxyls.cn

[T36] Lua：函数
来源：http://kn.nszjky.cn

function add(a, b) return a + b end
来源：http://mp.521024.cn

[T37] Lua：字符串拼接
来源：http://qx.newstarts.cn

"a" .. "b"
来源：http://fj.colortex.cn

[T38] Lua：条件
来源：http://td.haigaiapp.cn

if x > 0 then print("正") end
来源：http://yv.huanxung.cn

[T39] Lua：模式匹配
来源：http://qy.yuexingan06.cn

string.find(s, "%d+")
来源：http://re.huixiangedu.cn

[T40] Lua：元表
来源：http://hl.hnjuh.cn

setmetatable({}, { __index = base })
来源：http://tk.huixinmuqiang.cn

[T41] Perl：Hello World
来源：http://wa.jctech888.com.cn

print "Hello\n";
来源：http://jk.colortex.cn

[T42] Perl：变量类型
来源：http://we.bookmarksfly.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ww.hnjuh.cn

[T43] Perl：字符串插值
来源：http://jo.yuexingan06.cn

"值: $a"
来源：http://gb.asd995.cn

[T44] Perl：条件
来源：http://zn.jianghongdianzi.cn

if ($a > 0) { print "正"; }
来源：http://kg.muxihuayi.cn

[T45] Perl：数组遍历
来源：http://ub.szsharing.cn

for my $x (@arr) { print $x; }
来源：http://rh.wgjwhj.cn

[T46] Perl：哈希操作
来源：http://gm.hahajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://an.yuntaijiaju.cn

[T47] Perl：正则捕获
来源：http://ez.nszjky.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://un.nicolike.cn

[T48] Perl：正则替换
来源：http://pw.huanxung.cn

$s =~ s/old/new/g;
来源：http://jr.jianghongdianzi.cn

[T49] Perl：函数
来源：http://dy.yuntaijiaju.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pf.huixinmuqiang.cn

[T50] Perl：逐行读文件
来源：http://fa.nicolike.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ia.shtwfgs.cn

while (my $line = <$fh>) { print $line; }
来源：http://ci.gzmigu.cn

[T51] Scala：Hello World
来源：http://kj.9csxet.cn

println("Hello")
来源：http://mx.nszjky.cn

[T52] Scala：变量
来源：http://vk.bookmarksfly.cn

val a = 1;  var b = 2
来源：http://dd.huanxung.cn

[T53] Scala：字符串插值
来源：http://fi.wgjwhj.cn

s"值: $b"
来源：http://nb.colortex.cn

[T54] Scala：集合映射
来源：http://qw.bookmarksfly.cn

List(1, 2, 3).map(_ * 2)
来源：http://cd.newstarts.cn

[T55] Scala：集合过滤
来源：http://yr.jianghongdianzi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ce.shxzukj.cn

[T56] Scala：样例类
来源：http://au.muxihuayi.cn

case class User(name: String, age: Int)
来源：http://dd.shtwfgs.cn

[T57] Scala：模式匹配
来源：http://uh.haigaiapp.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://qn.chemitech.net.cn

[T58] Scala：函数定义
来源：http://gd.yuntaijiaju.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zu.szxytkj.cn

[T59] Scala：循环
来源：http://uj.nicolike.cn

for (i <- 1 to 10) println(i)
来源：http://bi.shtwfgs.cn

[T60] Scala：折叠
来源：http://hl.panjiajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fv.9csxet.cn

================================================================================
来源：http://ln.chemitech.net.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mg.shxzskj.cn

================================================================================
来源：http://hm.haigaiapp.cn

[U01] Py：创建虚拟环境
来源：http://hi.jianghongdianzi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jq.colortex.cn

[U02] Py：导出 / 安装依赖
来源：http://kg.9csxet.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yu.yuntaijiaju.cn

[U03] Py：加载 .env 配置
来源：http://gz.shxzskj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://oz.shxzukj.cn

[U04] Py：变量调试打印
来源：http://jf.szxytkj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wp.hahajie.cn

[U05] Py：列表去重且保序
来源：http://gc.colortex.cn

list(dict.fromkeys(arr))
来源：http://bn.nicolike.cn

[U06] Py：合并两个字典
来源：http://cz.szsharing.cn

{**a, **b}
来源：http://kf.shtwfgs.cn

[U07] Py：反转字典键值
来源：http://kn.yuntaijiaju.cn

{v: k for k, v in d.items()}
来源：http://zd.wgjwhj.cn

[U08] Py：展平二维列表
来源：http://yt.nicolike.cn

[y for x in nested for y in x]
来源：http://pe.gzmigu.cn

[U09] Py：字典取最大值的键
来源：http://nc.szsharing.cn

max(d, key=d.get)
来源：http://sp.wgjwhj.cn

[U10] Py：按值排序字典
来源：http://ig.bookmarksfly.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://da.szxytkj.cn

[U11] Py：生成器表达式
来源：http://me.shtwfgs.cn

(x * 2 for x in arr)
来源：http://au.jianghongdianzi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ds.shxzukj.cn

Counter(arr).most_common(3)
来源：http://oe.haigaiapp.cn

[U13] Py：固定长度队列
来源：http://ma.shtwfgs.cn

deque(maxlen=10)
来源：http://lc.szxytkj.cn

[U14] Py：分组收集到列表
来源：http://fq.huanxung.cn

defaultdict(list)
来源：http://ay.wgjwhj.cn

[U15] Py：高精度计时
来源：http://cj.lnxyls.cn

t = time.perf_counter()
来源：http://ae.huixinmuqiang.cn

[U16] Py：命令行参数解析
来源：http://ck.wgjwhj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gi.muxihuayi.cn

[U17] Py：初始化日志
来源：http://py.newstarts.cn

logging.basicConfig(level=logging.INFO)
来源：http://ch.panjiajie.cn

[U18] Py：预编译正则
来源：http://ct.gzmigu.cn

pat = re.compile(r"\d+")
来源：http://wl.shtwfgs.cn

[U19] Py：正则替换带回调
来源：http://ub.521024.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mc.colortex.cn

[U20] Py：缓存函数结果
来源：http://un.panjiajie.cn

@functools.lru_cache(maxsize=None)
来源：http://sd.yuexingan06.cn

[U21] Py：自定义上下文管理器
来源：http://jt.newstarts.cn

@contextlib.contextmanager
来源：http://fo.wgjwhj.cn

[U22] Py：矩阵转置
来源：http://oc.jctech888.com.cn

list(zip(*m))
来源：http://lr.9csxet.cn

[U23] Py：分块读取大文件
来源：http://xs.huixiangedu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dl.chemitech.net.cn

[U24] Py：路径操作
来源：http://vs.asd995.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hv.muxihuayi.cn

[U25] Py：CSV 按字典读
来源：http://ns.muxihuayi.cn

csv.DictReader(f)
来源：http://eb.shxzskj.cn

[U26] Py：并发下载
来源：http://vu.colortex.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gi.hahajie.cn

[U27] Py：异步 HTTP
来源：http://vn.yuntaijiaju.cn

aiohttp.ClientSession() 配合 async with
来源：http://sy.521024.cn

[U28] Py：类型别名
来源：http://wl.szxytkj.cn

UserId = int
来源：http://oc.gzmigu.cn

[U29] Py：属性校验
来源：http://ii.wgjwhj.cn

@property 与 @x.setter 配合
来源：http://fi.szxytkj.cn

[U30] Py：数据类
来源：http://bg.haigaiapp.cn

@dataclass(slots=True)
来源：http://wf.jctech888.com.cn

[U31] Py：单测
来源：http://jf.yuexingan06.cn

python -m pytest -q
来源：http://bp.asd995.cn

[U32] Py：代码格式化
来源：http://gf.shtwfgs.cn

ruff format . && ruff check --fix .
来源：http://wt.hnjuh.cn

[U33] Py：打包发布
来源：http://zx.lnxyls.cn

python -m build  （依赖 pyproject.toml）
来源：http://ol.hnjuh.cn

[U34] Py：判断编码
来源：http://bt.nicolike.cn

chardet.detect(raw)
来源：http://bv.jianghongdianzi.cn

[U35] Py：发送邮件
来源：http://yk.colortex.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://oo.bjjhwx.cn

[U36] Py：定时任务
来源：http://pi.bjjhwx.cn

schedule.every(10).minutes.do(job)
来源：http://jc.nszjky.cn

[U37] Py：读写 Excel
来源：http://fm.shxzskj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ox.nicolike.cn

[U38] Py：获取脚本所在目录
来源：http://kl.asd995.cn

Path(__file__).resolve().parent
来源：http://nq.huixiangedu.cn

[U39] Py：判断是否在交互环境
来源：http://zw.szsharing.cn

sys.stdout.isatty()
来源：http://et.hahajie.cn

[U40] Py：打印到标准错误
来源：http://ac.yuntaijiaju.cn

print("err", file=sys.stderr)
来源：http://gn.wgjwhj.cn

[U41] PHP：初始化 Composer 项目
来源：http://gk.hahajie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://vw.colortex.cn

[U42] PHP：PSR-4 自动加载
来源：http://tl.colortex.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ff.521024.cn

[U43] PHP：声明命名空间
来源：http://ps.szsharing.cn

namespace App\Http;
来源：http://gb.shxzukj.cn

[U44] PHP：开启严格类型
来源：http://yj.haigaiapp.cn

declare(strict_types=1);
来源：http://td.wgjwhj.cn

[U45] PHP：类型声明与返回类型
来源：http://rr.colortex.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://of.jctech888.com.cn

[U46] PHP：可空类型
来源：http://ip.bjjhwx.cn

?string $name = null
来源：http://yl.bjjhwx.cn

[U47] PHP：联合类型
来源：http://ek.huixinmuqiang.cn

int|string $id
来源：http://jt.chemitech.net.cn

[U48] PHP：纯枚举
来源：http://ix.hnjuh.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xd.hahajie.cn

[U49] PHP：只读属性
来源：http://rx.wgjwhj.cn

public readonly string $name
来源：http://gj.9csxet.cn

[U50] PHP：构造器属性提升
来源：http://wr.szsharing.cn

public function __construct(private int $id) {}
来源：http://et.newstarts.cn

[U51] PHP：数组解构
来源：http://kb.yuexingan06.cn

[$a, $b] = $arr;
来源：http://xi.huixinmuqiang.cn

[U52] PHP：箭头函数
来源：http://wj.wgjwhj.cn

$double = fn($x) => $x * 2;
来源：http://ja.haigaiapp.cn

[U53] PHP：空合并运算符
来源：http://fk.huixinmuqiang.cn

$v = $a ?? $b ?? "default";
来源：http://ue.huanxung.cn

[U54] PHP：空安全调用
来源：http://ht.gzmigu.cn

$obj?->method()
来源：http://mo.asd995.cn

[U55] PHP：match 表达式
来源：http://he.panjiajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mw.shxzukj.cn

[U56] PHP：命名参数
来源：http://oh.huixinmuqiang.cn

f(a: 1, b: 2)
来源：http://ia.hahajie.cn

[U57] PHP：字符串插值
来源：http://ci.huixiangedu.cn

"值: {$a}"
来源：http://co.nicolike.cn

[U58] PHP：数组三件套
来源：http://lc.wgjwhj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nh.colortex.cn

[U59] PHP：自定义排序
来源：http://af.hnjuh.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mr.jianghongdianzi.cn

[U60] PHP：JSON 编解码
来源：http://xk.wgjwhj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bj.gzmigu.cn

[U61] PHP：正则
来源：http://vt.huixiangedu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rm.lnxyls.cn

[U62] PHP：日期对象
来源：http://qp.9csxet.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jp.lnxyls.cn

[U63] PHP：文件读写
来源：http://ny.bookmarksfly.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tv.9csxet.cn

[U64] PHP：目录遍历
来源：http://sj.chemitech.net.cn

glob("dir/*.php");  scandir("dir");
来源：http://ry.szsharing.cn

[U65] PHP：会话
来源：http://hb.szsharing.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rg.muxihuayi.cn

[U66] PHP：设置 Cookie
来源：http://fj.shxzskj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ia.asd995.cn

[U67] PHP：处理文件上传
来源：http://jb.muxihuayi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fk.shxzukj.cn

[U68] PHP：PDO 连接
来源：http://hw.haigaiapp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ns.nicolike.cn

[U69] PHP：PDO 预处理
来源：http://bo.huixiangedu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tz.szsharing.cn

[U70] PHP：PDO 事务
来源：http://iv.panjiajie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rm.bookmarksfly.cn

[U71] PHP：抛出异常
来源：http://sk.haigaiapp.cn

throw new RuntimeException("失败", 500);
来源：http://wn.muxihuayi.cn

[U72] PHP：写错误日志
来源：http://ya.nicolike.cn

error_log("失败: " . $e->getMessage());
来源：http://mr.hahajie.cn

[U73] PHP：读取 ini 配置
来源：http://rj.shtwfgs.cn

parse_ini_file("config.ini", true)
来源：http://nz.panjiajie.cn

[U74] PHP：读取环境变量
来源：http://tm.lnxyls.cn

getenv("APP_ENV") ?: "production"
来源：http://dm.asd995.cn

[U75] PHP：依赖注入
来源：http://jz.jctech888.com.cn

composer require psr/container
来源：http://ng.huixinmuqiang.cn

[U76] PHP：简单路由
来源：http://ze.szxytkj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yj.jctech888.com.cn

[U77] PHP：模板渲染
来源：http://cf.nicolike.cn

composer require twig/twig
来源：http://sd.yuntaijiaju.cn

[U78] PHP：单元测试
来源：http://qi.wgjwhj.cn

composer require --dev phpunit/phpunit
来源：http://ze.haigaiapp.cn

[U79] PHP：静态分析
来源：http://wo.szxytkj.cn

composer require --dev phpstan/phpstan
来源：http://sc.nszjky.cn

[U80] PHP：代码规范修复
来源：http://eu.huanxung.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://un.yuntaijiaju.cn

[U81] JS：初始化项目
来源：http://ax.huanxung.cn

npm init -y;  npm i express
来源：http://kh.wgjwhj.cn

[U82] JS：package.json 脚本
来源：http://gc.lnxyls.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xd.panjiajie.cn

[U83] JS：ES Module 导入导出
来源：http://es.shxzukj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ed.panjiajie.cn

[U84] JS：CommonJS 写法
来源：http://yz.newstarts.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ac.huixiangedu.cn

[U85] JS：可选链
来源：http://qp.bookmarksfly.cn

a?.b?.c
来源：http://em.huixinmuqiang.cn

[U86] JS：空值合并
来源：http://fm.muxihuayi.cn

a ?? b
来源：http://ea.9csxet.cn

[U87] JS：解构默认值
来源：http://ot.hnjuh.cn

const { a = 1, b = 2 } = obj;
来源：http://sa.szsharing.cn

[U88] JS：对象展开合并
来源：http://hc.nicolike.cn

{ ...a, ...b }
来源：http://ye.panjiajie.cn

[U89] JS：数组去重
来源：http://ph.szsharing.cn

[...new Set(arr)]
来源：http://sh.yuntaijiaju.cn

[U90] JS：数字数组排序
来源：http://ee.wgjwhj.cn

[...arr].sort((a, b) => a - b)
来源：http://vg.jianghongdianzi.cn

[U91] JS：对象键值遍历
来源：http://mu.huanxung.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gh.nicolike.cn

[U92] JS：深拷贝
来源：http://lp.bookmarksfly.cn

structuredClone(obj)
来源：http://jk.nszjky.cn

[U93] JS：模板字符串
来源：http://hn.yuntaijiaju.cn

`共 ${n} 条`
来源：http://cm.wgjwhj.cn

[U94] JS：箭头函数
来源：http://tv.bjjhwx.cn

const double = x => x * 2;
来源：http://oc.colortex.cn

[U95] JS：Promise 包装
来源：http://tw.asd995.cn

new Promise((resolve, reject) => {})
来源：http://nz.shxzskj.cn

[U96] JS：async/await 与异常
来源：http://bt.shtwfgs.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lq.shtwfgs.cn

[U97] JS：并发请求
来源：http://lo.szsharing.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://td.szsharing.cn

[U98] JS：fetch 带 JSON
来源：http://qc.hnjuh.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wr.bookmarksfly.cn

[U99] JS：事件监听
来源：http://mu.lnxyls.cn

el.addEventListener("click", e => {})
来源：http://yu.szxytkj.cn

[U100] JS：DOM 查询
来源：http://lp.szxytkj.cn

document.querySelector(".item")
来源：http://ke.bjjhwx.cn

[U101] JS：classList 操作
来源：http://nc.jctech888.com.cn

el.classList.toggle("active")
来源：http://os.huixiangedu.cn

[U102] JS：本地存储
来源：http://ql.yuexingan06.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jw.shxzskj.cn

[U103] JS：定时器
来源：http://fh.colortex.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xw.nszjky.cn

[U104] JS：防抖
来源：http://ga.shtwfgs.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mv.shxzskj.cn

[U105] JS：节流
来源：http://jc.nszjky.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gv.colortex.cn

[U106] JS：日期格式化
来源：http://wg.huanxung.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qm.nicolike.cn

[U107] JS：数字千分位
来源：http://ky.huanxung.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rs.gzmigu.cn

[U108] JS：随机整数
来源：http://tm.shxzskj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yj.shtwfgs.cn

[U109] JS：数组分组
来源：http://qe.shxzukj.cn

Object.groupBy(arr, x => x.type)
来源：http://rx.lnxyls.cn

[U110] JS：数组分块
来源：http://bf.yuntaijiaju.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://di.nszjky.cn

[U111] JS：对象转 Map
来源：http://co.panjiajie.cn

new Map(Object.entries(obj))
来源：http://wu.jctech888.com.cn

[U112] JS：字符串补位
来源：http://by.hahajie.cn

"7".padStart(3, "0")
来源：http://ec.shxzskj.cn

[U113] JS：正则替换全部
来源：http://ke.bjjhwx.cn

s.replaceAll("a", "b")
来源：http://pu.lnxyls.cn

[U114] JS：JSON 深比较
来源：http://nd.panjiajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ud.huixinmuqiang.cn


<!-- 参考信息 -->