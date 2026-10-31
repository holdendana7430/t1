代发 wailian999

[T27] Swift：错误处理
来源：http://cq.lnxyls.cn

do { try f() } catch { print(error) }
来源：http://qv.nicolike.cn

[T28] Swift：枚举
来源：http://md.gzmigu.cn

enum Color { case red, green }
来源：http://iy.yuexingan06.cn

[T29] Swift：guard 提前返回
来源：http://wf.shtwfgs.cn

guard let x = opt else { return }
来源：http://in.huanxung.cn

[T30] Swift：协议
来源：http://hp.jianghongdianzi.cn

protocol Shape { func area() -> Double }
来源：http://mo.chemitech.net.cn

[T31] Lua：Hello World
来源：http://bk.huixiangedu.cn

print("Hello")
来源：http://uk.yuntaijiaju.cn

[T32] Lua：局部变量
来源：http://sb.nszjky.cn

local a = 1
来源：http://fl.lnxyls.cn

[T33] Lua：表（数组）
来源：http://gz.haigaiapp.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://oh.szsharing.cn

[T34] Lua：遍历表
来源：http://ju.wgjwhj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vw.hnjuh.cn

[T35] Lua：字典表
来源：http://fa.huixiangedu.cn

local d = { a = 1 };  d.b = 2
来源：http://el.yuexingan06.cn

[T36] Lua：函数
来源：http://wy.nicolike.cn

function add(a, b) return a + b end
来源：http://cp.hnjuh.cn

[T37] Lua：字符串拼接
来源：http://xq.lnxyls.cn

"a" .. "b"
来源：http://zn.bookmarksfly.cn

[T38] Lua：条件
来源：http://fw.huanxung.cn

if x > 0 then print("正") end
来源：http://yc.huixiangedu.cn

[T39] Lua：模式匹配
来源：http://xn.asd995.cn

string.find(s, "%d+")
来源：http://kb.wgjwhj.cn

[T40] Lua：元表
来源：http://ub.haigaiapp.cn

setmetatable({}, { __index = base })
来源：http://rr.shtwfgs.cn

[T41] Perl：Hello World
来源：http://pk.gzmigu.cn

print "Hello\n";
来源：http://jw.bookmarksfly.cn

[T42] Perl：变量类型
来源：http://wj.panjiajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://iu.muxihuayi.cn

[T43] Perl：字符串插值
来源：http://pu.lnxyls.cn

"值: $a"
来源：http://qb.szsharing.cn

[T44] Perl：条件
来源：http://zy.jctech888.com.cn

if ($a > 0) { print "正"; }
来源：http://mc.hahajie.cn

[T45] Perl：数组遍历
来源：http://gs.haigaiapp.cn

for my $x (@arr) { print $x; }
来源：http://st.haigaiapp.cn

[T46] Perl：哈希操作
来源：http://ot.huixinmuqiang.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ni.nszjky.cn

[T47] Perl：正则捕获
来源：http://qu.nicolike.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pa.panjiajie.cn

[T48] Perl：正则替换
来源：http://bs.yuntaijiaju.cn

$s =~ s/old/new/g;
来源：http://ra.lnxyls.cn

[T49] Perl：函数
来源：http://iz.muxihuayi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tr.wgjwhj.cn

[T50] Perl：逐行读文件
来源：http://bc.wgjwhj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://yn.haigaiapp.cn

while (my $line = <$fh>) { print $line; }
来源：http://yo.yuntaijiaju.cn

[T51] Scala：Hello World
来源：http://fk.shxzskj.cn

println("Hello")
来源：http://aa.yuexingan06.cn

[T52] Scala：变量
来源：http://jp.wgjwhj.cn

val a = 1;  var b = 2
来源：http://po.szsharing.cn

[T53] Scala：字符串插值
来源：http://aq.jctech888.com.cn

s"值: $b"
来源：http://vt.muxihuayi.cn

[T54] Scala：集合映射
来源：http://ct.huanxung.cn

List(1, 2, 3).map(_ * 2)
来源：http://mw.9csxet.cn

[T55] Scala：集合过滤
来源：http://ud.asd995.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ze.hnjuh.cn

[T56] Scala：样例类
来源：http://iz.shxzukj.cn

case class User(name: String, age: Int)
来源：http://rc.haigaiapp.cn

[T57] Scala：模式匹配
来源：http://vt.shxzskj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vr.panjiajie.cn

[T58] Scala：函数定义
来源：http://gz.panjiajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zp.yuntaijiaju.cn

[T59] Scala：循环
来源：http://vd.bjjhwx.cn

for (i <- 1 to 10) println(i)
来源：http://kv.nicolike.cn

[T60] Scala：折叠
来源：http://bx.shxzukj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://aa.hahajie.cn

================================================================================
来源：http://su.huixiangedu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ih.haigaiapp.cn

================================================================================
来源：http://nx.lnxyls.cn

[U01] Py：创建虚拟环境
来源：http://xa.shtwfgs.cn

python -m venv .venv && source .venv/bin/activate
来源：http://fu.szxytkj.cn

[U02] Py：导出 / 安装依赖
来源：http://ru.jianghongdianzi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zm.asd995.cn

[U03] Py：加载 .env 配置
来源：http://en.huixiangedu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://og.nicolike.cn

[U04] Py：变量调试打印
来源：http://yw.asd995.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ey.yuntaijiaju.cn

[U05] Py：列表去重且保序
来源：http://ar.jctech888.com.cn

list(dict.fromkeys(arr))
来源：http://ui.colortex.cn

[U06] Py：合并两个字典
来源：http://kq.nszjky.cn

{**a, **b}
来源：http://xo.shxzskj.cn

[U07] Py：反转字典键值
来源：http://uf.huanxung.cn

{v: k for k, v in d.items()}
来源：http://mn.huixiangedu.cn

[U08] Py：展平二维列表
来源：http://io.chemitech.net.cn

[y for x in nested for y in x]
来源：http://cd.huixiangedu.cn

[U09] Py：字典取最大值的键
来源：http://ao.hnjuh.cn

max(d, key=d.get)
来源：http://kt.muxihuayi.cn

[U10] Py：按值排序字典
来源：http://et.haigaiapp.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pc.huixiangedu.cn

[U11] Py：生成器表达式
来源：http://en.chemitech.net.cn

(x * 2 for x in arr)
来源：http://rs.jianghongdianzi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xk.lnxyls.cn

Counter(arr).most_common(3)
来源：http://wh.lnxyls.cn

[U13] Py：固定长度队列
来源：http://gz.muxihuayi.cn

deque(maxlen=10)
来源：http://mx.521024.cn

[U14] Py：分组收集到列表
来源：http://bs.nszjky.cn

defaultdict(list)
来源：http://ry.szxytkj.cn

[U15] Py：高精度计时
来源：http://do.wgjwhj.cn

t = time.perf_counter()
来源：http://ct.nicolike.cn

[U16] Py：命令行参数解析
来源：http://ki.wgjwhj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nx.muxihuayi.cn

[U17] Py：初始化日志
来源：http://ag.szsharing.cn

logging.basicConfig(level=logging.INFO)
来源：http://de.nicolike.cn

[U18] Py：预编译正则
来源：http://ec.lnxyls.cn

pat = re.compile(r"\d+")
来源：http://qi.jctech888.com.cn

[U19] Py：正则替换带回调
来源：http://gi.hahajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cd.nszjky.cn

[U20] Py：缓存函数结果
来源：http://of.huanxung.cn

@functools.lru_cache(maxsize=None)
来源：http://ix.muxihuayi.cn

[U21] Py：自定义上下文管理器
来源：http://fz.bookmarksfly.cn

@contextlib.contextmanager
来源：http://gl.gzmigu.cn

[U22] Py：矩阵转置
来源：http://jn.asd995.cn

list(zip(*m))
来源：http://qz.panjiajie.cn

[U23] Py：分块读取大文件
来源：http://lv.jianghongdianzi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pf.shxzukj.cn

[U24] Py：路径操作
来源：http://iz.bookmarksfly.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ew.wgjwhj.cn

[U25] Py：CSV 按字典读
来源：http://ut.bjjhwx.cn

csv.DictReader(f)
来源：http://yq.gzmigu.cn

[U26] Py：并发下载
来源：http://wm.yuntaijiaju.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hq.panjiajie.cn

[U27] Py：异步 HTTP
来源：http://rm.asd995.cn

aiohttp.ClientSession() 配合 async with
来源：http://el.hnjuh.cn

[U28] Py：类型别名
来源：http://iz.yuntaijiaju.cn

UserId = int
来源：http://hc.asd995.cn

[U29] Py：属性校验
来源：http://ml.huixiangedu.cn

@property 与 @x.setter 配合
来源：http://dr.nszjky.cn

[U30] Py：数据类
来源：http://ab.wgjwhj.cn

@dataclass(slots=True)
来源：http://kr.hahajie.cn

[U31] Py：单测
来源：http://ls.chemitech.net.cn

python -m pytest -q
来源：http://zd.wgjwhj.cn

[U32] Py：代码格式化
来源：http://oc.asd995.cn

ruff format . && ruff check --fix .
来源：http://lw.nicolike.cn

[U33] Py：打包发布
来源：http://sq.521024.cn

python -m build  （依赖 pyproject.toml）
来源：http://kz.asd995.cn

[U34] Py：判断编码
来源：http://le.shxzukj.cn

chardet.detect(raw)
来源：http://nb.szxytkj.cn

[U35] Py：发送邮件
来源：http://jf.szsharing.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yd.shxzukj.cn

[U36] Py：定时任务
来源：http://zt.huixinmuqiang.cn

schedule.every(10).minutes.do(job)
来源：http://np.huanxung.cn

[U37] Py：读写 Excel
来源：http://um.nszjky.cn

pandas.read_excel / DataFrame.to_excel
来源：http://th.newstarts.cn

[U38] Py：获取脚本所在目录
来源：http://rc.huixinmuqiang.cn

Path(__file__).resolve().parent
来源：http://bv.szxytkj.cn

[U39] Py：判断是否在交互环境
来源：http://cd.huixinmuqiang.cn

sys.stdout.isatty()
来源：http://sh.hahajie.cn

[U40] Py：打印到标准错误
来源：http://wx.shxzukj.cn

print("err", file=sys.stderr)
来源：http://fy.szsharing.cn

[U41] PHP：初始化 Composer 项目
来源：http://nm.shxzskj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://pl.jianghongdianzi.cn

[U42] PHP：PSR-4 自动加载
来源：http://kf.hnjuh.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pk.haigaiapp.cn

[U43] PHP：声明命名空间
来源：http://yd.panjiajie.cn

namespace App\Http;
来源：http://gi.shtwfgs.cn

[U44] PHP：开启严格类型
来源：http://ti.yuexingan06.cn

declare(strict_types=1);
来源：http://mh.asd995.cn

[U45] PHP：类型声明与返回类型
来源：http://el.huixiangedu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://tp.muxihuayi.cn

[U46] PHP：可空类型
来源：http://yz.nszjky.cn

?string $name = null
来源：http://ry.newstarts.cn

[U47] PHP：联合类型
来源：http://ii.9csxet.cn

int|string $id
来源：http://xb.gzmigu.cn

[U48] PHP：纯枚举
来源：http://ig.shtwfgs.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hl.nszjky.cn

[U49] PHP：只读属性
来源：http://dm.chemitech.net.cn

public readonly string $name
来源：http://vh.shxzukj.cn

[U50] PHP：构造器属性提升
来源：http://zh.shxzukj.cn

public function __construct(private int $id) {}
来源：http://ys.hahajie.cn

[U51] PHP：数组解构
来源：http://pv.jianghongdianzi.cn

[$a, $b] = $arr;
来源：http://sz.bookmarksfly.cn

[U52] PHP：箭头函数
来源：http://sm.9csxet.cn

$double = fn($x) => $x * 2;
来源：http://kw.yuexingan06.cn

[U53] PHP：空合并运算符
来源：http://tn.muxihuayi.cn

$v = $a ?? $b ?? "default";
来源：http://vm.chemitech.net.cn

[U54] PHP：空安全调用
来源：http://fh.hnjuh.cn

$obj?->method()
来源：http://ju.hahajie.cn

[U55] PHP：match 表达式
来源：http://ex.yuexingan06.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mx.szsharing.cn

[U56] PHP：命名参数
来源：http://yf.colortex.cn

f(a: 1, b: 2)
来源：http://lv.jianghongdianzi.cn

[U57] PHP：字符串插值
来源：http://tq.shxzukj.cn

"值: {$a}"
来源：http://ko.asd995.cn

[U58] PHP：数组三件套
来源：http://qd.huixiangedu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://sx.shtwfgs.cn

[U59] PHP：自定义排序
来源：http://hr.lnxyls.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bp.asd995.cn

[U60] PHP：JSON 编解码
来源：http://lm.asd995.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pi.bookmarksfly.cn

[U61] PHP：正则
来源：http://bk.colortex.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://eq.521024.cn

[U62] PHP：日期对象
来源：http://mb.shtwfgs.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wn.hahajie.cn

[U63] PHP：文件读写
来源：http://zv.szsharing.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pr.hahajie.cn

[U64] PHP：目录遍历
来源：http://rk.bookmarksfly.cn

glob("dir/*.php");  scandir("dir");
来源：http://cs.bookmarksfly.cn

[U65] PHP：会话
来源：http://ic.shtwfgs.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://wn.nszjky.cn

[U66] PHP：设置 Cookie
来源：http://lh.shxzskj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://iv.jianghongdianzi.cn

[U67] PHP：处理文件上传
来源：http://pw.hnjuh.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nq.shxzskj.cn

[U68] PHP：PDO 连接
来源：http://qy.shxzskj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vw.521024.cn

[U69] PHP：PDO 预处理
来源：http://yl.jctech888.com.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jk.bjjhwx.cn

[U70] PHP：PDO 事务
来源：http://vy.huanxung.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pc.bjjhwx.cn

[U71] PHP：抛出异常
来源：http://aq.shtwfgs.cn

throw new RuntimeException("失败", 500);
来源：http://xb.gzmigu.cn

[U72] PHP：写错误日志
来源：http://ib.wgjwhj.cn

error_log("失败: " . $e->getMessage());
来源：http://xv.jianghongdianzi.cn

[U73] PHP：读取 ini 配置
来源：http://rc.nszjky.cn

parse_ini_file("config.ini", true)
来源：http://iw.521024.cn

[U74] PHP：读取环境变量
来源：http://ba.jianghongdianzi.cn

getenv("APP_ENV") ?: "production"
来源：http://kh.hahajie.cn

[U75] PHP：依赖注入
来源：http://mp.muxihuayi.cn

composer require psr/container
来源：http://pv.yuntaijiaju.cn

[U76] PHP：简单路由
来源：http://bz.huixinmuqiang.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nw.wgjwhj.cn

[U77] PHP：模板渲染
来源：http://hp.huixiangedu.cn

composer require twig/twig
来源：http://eq.chemitech.net.cn

[U78] PHP：单元测试
来源：http://rc.nszjky.cn

composer require --dev phpunit/phpunit
来源：http://cs.nszjky.cn

[U79] PHP：静态分析
来源：http://sw.shtwfgs.cn

composer require --dev phpstan/phpstan
来源：http://ds.nszjky.cn

[U80] PHP：代码规范修复
来源：http://qh.chemitech.net.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://lq.shxzukj.cn

[U81] JS：初始化项目
来源：http://fp.521024.cn

npm init -y;  npm i express
来源：http://yb.colortex.cn

[U82] JS：package.json 脚本
来源：http://kq.huanxung.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ky.bookmarksfly.cn

[U83] JS：ES Module 导入导出
来源：http://ck.lnxyls.cn

export const a = 1;  import { a } from "./m.js";
来源：http://rg.colortex.cn

[U84] JS：CommonJS 写法
来源：http://la.muxihuayi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://jp.bookmarksfly.cn

[U85] JS：可选链
来源：http://sf.bookmarksfly.cn

a?.b?.c
来源：http://lm.bjjhwx.cn

[U86] JS：空值合并
来源：http://am.521024.cn

a ?? b
来源：http://zs.jianghongdianzi.cn

[U87] JS：解构默认值
来源：http://ju.muxihuayi.cn

const { a = 1, b = 2 } = obj;
来源：http://jw.muxihuayi.cn

[U88] JS：对象展开合并
来源：http://di.huixinmuqiang.cn

{ ...a, ...b }
来源：http://wb.shxzukj.cn

[U89] JS：数组去重
来源：http://ey.lnxyls.cn

[...new Set(arr)]
来源：http://sc.shxzskj.cn

[U90] JS：数字数组排序
来源：http://ld.gzmigu.cn

[...arr].sort((a, b) => a - b)
来源：http://jl.szxytkj.cn

[U91] JS：对象键值遍历
来源：http://tz.szxytkj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xi.asd995.cn

[U92] JS：深拷贝
来源：http://dn.yuexingan06.cn

structuredClone(obj)
来源：http://pj.shtwfgs.cn

[U93] JS：模板字符串
来源：http://df.nszjky.cn

`共 ${n} 条`
来源：http://iv.muxihuayi.cn

[U94] JS：箭头函数
来源：http://ej.wgjwhj.cn

const double = x => x * 2;
来源：http://dm.nicolike.cn

[U95] JS：Promise 包装
来源：http://fd.jianghongdianzi.cn

new Promise((resolve, reject) => {})
来源：http://bj.huixiangedu.cn

[U96] JS：async/await 与异常
来源：http://ve.9csxet.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wa.jctech888.com.cn

[U97] JS：并发请求
来源：http://jf.newstarts.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://yu.shxzskj.cn

[U98] JS：fetch 带 JSON
来源：http://ih.jianghongdianzi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gs.shxzukj.cn

[U99] JS：事件监听
来源：http://cl.shxzskj.cn

el.addEventListener("click", e => {})
来源：http://ud.chemitech.net.cn

[U100] JS：DOM 查询
来源：http://em.jctech888.com.cn

document.querySelector(".item")
来源：http://mp.hnjuh.cn

[U101] JS：classList 操作
来源：http://bk.gzmigu.cn

el.classList.toggle("active")
来源：http://wg.yuexingan06.cn

[U102] JS：本地存储
来源：http://ls.huixiangedu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://cz.wgjwhj.cn

[U103] JS：定时器
来源：http://gz.wgjwhj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yv.shtwfgs.cn

[U104] JS：防抖
来源：http://qn.szxytkj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lk.panjiajie.cn

[U105] JS：节流
来源：http://cn.muxihuayi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sm.lnxyls.cn

[U106] JS：日期格式化
来源：http://gn.bookmarksfly.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hn.hahajie.cn

[U107] JS：数字千分位
来源：http://mo.panjiajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://un.haigaiapp.cn

[U108] JS：随机整数
来源：http://vk.chemitech.net.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nd.asd995.cn

[U109] JS：数组分组
来源：http://nk.jctech888.com.cn

Object.groupBy(arr, x => x.type)
来源：http://zs.panjiajie.cn

[U110] JS：数组分块
来源：http://iu.bjjhwx.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bb.szsharing.cn

[U111] JS：对象转 Map
来源：http://ur.jctech888.com.cn

new Map(Object.entries(obj))
来源：http://mo.asd995.cn

[U112] JS：字符串补位
来源：http://lj.wgjwhj.cn

"7".padStart(3, "0")
来源：http://wb.haigaiapp.cn

[U113] JS：正则替换全部
来源：http://qg.lnxyls.cn

s.replaceAll("a", "b")
来源：http://bc.muxihuayi.cn

[U114] JS：JSON 深比较
来源：http://xv.hnjuh.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://kx.huixinmuqiang.cn


<!-- 参考信息 -->