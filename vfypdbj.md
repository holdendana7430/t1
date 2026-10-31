代发 wailian999

[T27] Swift：错误处理
来源：http://bq.muxihuayi.cn

do { try f() } catch { print(error) }
来源：http://wt.haigaiapp.cn

[T28] Swift：枚举
来源：http://pa.asd995.cn

enum Color { case red, green }
来源：http://na.nszjky.cn

[T29] Swift：guard 提前返回
来源：http://rl.haigaiapp.cn

guard let x = opt else { return }
来源：http://wc.wgjwhj.cn

[T30] Swift：协议
来源：http://yd.hnjuh.cn

protocol Shape { func area() -> Double }
来源：http://gg.chemitech.net.cn

[T31] Lua：Hello World
来源：http://tf.asd995.cn

print("Hello")
来源：http://et.wgjwhj.cn

[T32] Lua：局部变量
来源：http://xv.521024.cn

local a = 1
来源：http://qe.haigaiapp.cn

[T33] Lua：表（数组）
来源：http://wj.colortex.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://on.bjjhwx.cn

[T34] Lua：遍历表
来源：http://rw.haigaiapp.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://cw.huixiangedu.cn

[T35] Lua：字典表
来源：http://nx.huanxung.cn

local d = { a = 1 };  d.b = 2
来源：http://lq.9csxet.cn

[T36] Lua：函数
来源：http://sz.shxzskj.cn

function add(a, b) return a + b end
来源：http://de.9csxet.cn

[T37] Lua：字符串拼接
来源：http://dy.szxytkj.cn

"a" .. "b"
来源：http://nt.yuexingan06.cn

[T38] Lua：条件
来源：http://wm.szxytkj.cn

if x > 0 then print("正") end
来源：http://im.chemitech.net.cn

[T39] Lua：模式匹配
来源：http://tz.huanxung.cn

string.find(s, "%d+")
来源：http://rv.huanxung.cn

[T40] Lua：元表
来源：http://ew.huanxung.cn

setmetatable({}, { __index = base })
来源：http://jx.jianghongdianzi.cn

[T41] Perl：Hello World
来源：http://ak.bjjhwx.cn

print "Hello\n";
来源：http://jl.nicolike.cn

[T42] Perl：变量类型
来源：http://er.shtwfgs.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hv.shxzukj.cn

[T43] Perl：字符串插值
来源：http://gf.wgjwhj.cn

"值: $a"
来源：http://cl.chemitech.net.cn

[T44] Perl：条件
来源：http://xw.nicolike.cn

if ($a > 0) { print "正"; }
来源：http://ij.nicolike.cn

[T45] Perl：数组遍历
来源：http://on.hnjuh.cn

for my $x (@arr) { print $x; }
来源：http://ej.huixinmuqiang.cn

[T46] Perl：哈希操作
来源：http://uu.shxzukj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nt.shtwfgs.cn

[T47] Perl：正则捕获
来源：http://ay.chemitech.net.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://os.jianghongdianzi.cn

[T48] Perl：正则替换
来源：http://dy.colortex.cn

$s =~ s/old/new/g;
来源：http://jt.jctech888.com.cn

[T49] Perl：函数
来源：http://qf.szsharing.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lz.yuexingan06.cn

[T50] Perl：逐行读文件
来源：http://pe.jctech888.com.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rq.yuntaijiaju.cn

while (my $line = <$fh>) { print $line; }
来源：http://gs.bjjhwx.cn

[T51] Scala：Hello World
来源：http://al.wgjwhj.cn

println("Hello")
来源：http://up.huanxung.cn

[T52] Scala：变量
来源：http://nm.szxytkj.cn

val a = 1;  var b = 2
来源：http://pm.bjjhwx.cn

[T53] Scala：字符串插值
来源：http://xk.bookmarksfly.cn

s"值: $b"
来源：http://yr.szxytkj.cn

[T54] Scala：集合映射
来源：http://ip.muxihuayi.cn

List(1, 2, 3).map(_ * 2)
来源：http://kg.szsharing.cn

[T55] Scala：集合过滤
来源：http://ws.huanxung.cn

List(1, 2, 3).filter(_ > 1)
来源：http://rt.panjiajie.cn

[T56] Scala：样例类
来源：http://zu.newstarts.cn

case class User(name: String, age: Int)
来源：http://wq.lnxyls.cn

[T57] Scala：模式匹配
来源：http://sy.nicolike.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://nr.muxihuayi.cn

[T58] Scala：函数定义
来源：http://ur.jianghongdianzi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://az.yuexingan06.cn

[T59] Scala：循环
来源：http://hi.wgjwhj.cn

for (i <- 1 to 10) println(i)
来源：http://ia.bjjhwx.cn

[T60] Scala：折叠
来源：http://hj.colortex.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bj.muxihuayi.cn

================================================================================
来源：http://ag.huixiangedu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dl.hahajie.cn

================================================================================
来源：http://lx.nicolike.cn

[U01] Py：创建虚拟环境
来源：http://de.jianghongdianzi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zv.szxytkj.cn

[U02] Py：导出 / 安装依赖
来源：http://cu.wgjwhj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zj.colortex.cn

[U03] Py：加载 .env 配置
来源：http://of.asd995.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://lc.haigaiapp.cn

[U04] Py：变量调试打印
来源：http://vi.shxzukj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cm.szxytkj.cn

[U05] Py：列表去重且保序
来源：http://cb.chemitech.net.cn

list(dict.fromkeys(arr))
来源：http://gt.hahajie.cn

[U06] Py：合并两个字典
来源：http://ur.asd995.cn

{**a, **b}
来源：http://zb.asd995.cn

[U07] Py：反转字典键值
来源：http://wc.bjjhwx.cn

{v: k for k, v in d.items()}
来源：http://rr.hahajie.cn

[U08] Py：展平二维列表
来源：http://tm.newstarts.cn

[y for x in nested for y in x]
来源：http://qb.asd995.cn

[U09] Py：字典取最大值的键
来源：http://eo.shxzskj.cn

max(d, key=d.get)
来源：http://ki.huixinmuqiang.cn

[U10] Py：按值排序字典
来源：http://jp.szsharing.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://az.yuntaijiaju.cn

[U11] Py：生成器表达式
来源：http://ii.shtwfgs.cn

(x * 2 for x in arr)
来源：http://ok.gzmigu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qn.jctech888.com.cn

Counter(arr).most_common(3)
来源：http://jc.colortex.cn

[U13] Py：固定长度队列
来源：http://we.huanxung.cn

deque(maxlen=10)
来源：http://ix.asd995.cn

[U14] Py：分组收集到列表
来源：http://np.panjiajie.cn

defaultdict(list)
来源：http://xj.jianghongdianzi.cn

[U15] Py：高精度计时
来源：http://ki.9csxet.cn

t = time.perf_counter()
来源：http://vw.szxytkj.cn

[U16] Py：命令行参数解析
来源：http://xv.9csxet.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lb.haigaiapp.cn

[U17] Py：初始化日志
来源：http://wa.9csxet.cn

logging.basicConfig(level=logging.INFO)
来源：http://vn.9csxet.cn

[U18] Py：预编译正则
来源：http://pq.hnjuh.cn

pat = re.compile(r"\d+")
来源：http://bk.huanxung.cn

[U19] Py：正则替换带回调
来源：http://sk.nicolike.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ry.shtwfgs.cn

[U20] Py：缓存函数结果
来源：http://af.bookmarksfly.cn

@functools.lru_cache(maxsize=None)
来源：http://lp.colortex.cn

[U21] Py：自定义上下文管理器
来源：http://nd.huixiangedu.cn

@contextlib.contextmanager
来源：http://ul.chemitech.net.cn

[U22] Py：矩阵转置
来源：http://ze.newstarts.cn

list(zip(*m))
来源：http://ly.521024.cn

[U23] Py：分块读取大文件
来源：http://pj.shxzukj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://my.huixiangedu.cn

[U24] Py：路径操作
来源：http://uj.jianghongdianzi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ot.shtwfgs.cn

[U25] Py：CSV 按字典读
来源：http://al.wgjwhj.cn

csv.DictReader(f)
来源：http://jt.shtwfgs.cn

[U26] Py：并发下载
来源：http://lx.shxzukj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tv.lnxyls.cn

[U27] Py：异步 HTTP
来源：http://bq.szxytkj.cn

aiohttp.ClientSession() 配合 async with
来源：http://jr.chemitech.net.cn

[U28] Py：类型别名
来源：http://ig.asd995.cn

UserId = int
来源：http://lq.szxytkj.cn

[U29] Py：属性校验
来源：http://vh.nszjky.cn

@property 与 @x.setter 配合
来源：http://ac.wgjwhj.cn

[U30] Py：数据类
来源：http://cx.gzmigu.cn

@dataclass(slots=True)
来源：http://jb.huixiangedu.cn

[U31] Py：单测
来源：http://tx.colortex.cn

python -m pytest -q
来源：http://me.haigaiapp.cn

[U32] Py：代码格式化
来源：http://la.nicolike.cn

ruff format . && ruff check --fix .
来源：http://pv.yuntaijiaju.cn

[U33] Py：打包发布
来源：http://pw.huixiangedu.cn

python -m build  （依赖 pyproject.toml）
来源：http://jz.colortex.cn

[U34] Py：判断编码
来源：http://sb.hahajie.cn

chardet.detect(raw)
来源：http://gx.szxytkj.cn

[U35] Py：发送邮件
来源：http://fq.chemitech.net.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ix.hahajie.cn

[U36] Py：定时任务
来源：http://fo.lnxyls.cn

schedule.every(10).minutes.do(job)
来源：http://tu.shxzukj.cn

[U37] Py：读写 Excel
来源：http://er.9csxet.cn

pandas.read_excel / DataFrame.to_excel
来源：http://kz.gzmigu.cn

[U38] Py：获取脚本所在目录
来源：http://km.shtwfgs.cn

Path(__file__).resolve().parent
来源：http://rk.jianghongdianzi.cn

[U39] Py：判断是否在交互环境
来源：http://gi.bookmarksfly.cn

sys.stdout.isatty()
来源：http://ko.colortex.cn

[U40] Py：打印到标准错误
来源：http://gy.colortex.cn

print("err", file=sys.stderr)
来源：http://rr.szxytkj.cn

[U41] PHP：初始化 Composer 项目
来源：http://jy.muxihuayi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zx.yuntaijiaju.cn

[U42] PHP：PSR-4 自动加载
来源：http://ur.nszjky.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yk.wgjwhj.cn

[U43] PHP：声明命名空间
来源：http://jv.huixinmuqiang.cn

namespace App\Http;
来源：http://sv.gzmigu.cn

[U44] PHP：开启严格类型
来源：http://cr.huanxung.cn

declare(strict_types=1);
来源：http://cv.jianghongdianzi.cn

[U45] PHP：类型声明与返回类型
来源：http://qc.newstarts.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://an.bjjhwx.cn

[U46] PHP：可空类型
来源：http://th.newstarts.cn

?string $name = null
来源：http://iu.szxytkj.cn

[U47] PHP：联合类型
来源：http://va.asd995.cn

int|string $id
来源：http://xq.shtwfgs.cn

[U48] PHP：纯枚举
来源：http://xo.lnxyls.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wa.bjjhwx.cn

[U49] PHP：只读属性
来源：http://cn.gzmigu.cn

public readonly string $name
来源：http://wb.haigaiapp.cn

[U50] PHP：构造器属性提升
来源：http://gl.yuexingan06.cn

public function __construct(private int $id) {}
来源：http://hm.huixinmuqiang.cn

[U51] PHP：数组解构
来源：http://ed.jianghongdianzi.cn

[$a, $b] = $arr;
来源：http://nl.nszjky.cn

[U52] PHP：箭头函数
来源：http://nq.hahajie.cn

$double = fn($x) => $x * 2;
来源：http://dg.shxzskj.cn

[U53] PHP：空合并运算符
来源：http://cu.hahajie.cn

$v = $a ?? $b ?? "default";
来源：http://fb.huanxung.cn

[U54] PHP：空安全调用
来源：http://ym.gzmigu.cn

$obj?->method()
来源：http://bx.shxzskj.cn

[U55] PHP：match 表达式
来源：http://jb.shxzukj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fa.muxihuayi.cn

[U56] PHP：命名参数
来源：http://se.szxytkj.cn

f(a: 1, b: 2)
来源：http://ew.nicolike.cn

[U57] PHP：字符串插值
来源：http://wh.huixinmuqiang.cn

"值: {$a}"
来源：http://tb.muxihuayi.cn

[U58] PHP：数组三件套
来源：http://qu.yuntaijiaju.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vv.shxzskj.cn

[U59] PHP：自定义排序
来源：http://ro.hnjuh.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sl.bookmarksfly.cn

[U60] PHP：JSON 编解码
来源：http://sk.chemitech.net.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fl.jctech888.com.cn

[U61] PHP：正则
来源：http://fl.huanxung.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wp.huixiangedu.cn

[U62] PHP：日期对象
来源：http://kb.szsharing.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qi.asd995.cn

[U63] PHP：文件读写
来源：http://vo.9csxet.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nt.jctech888.com.cn

[U64] PHP：目录遍历
来源：http://nd.szxytkj.cn

glob("dir/*.php");  scandir("dir");
来源：http://wq.newstarts.cn

[U65] PHP：会话
来源：http://yr.huanxung.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://jw.nszjky.cn

[U66] PHP：设置 Cookie
来源：http://jf.panjiajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fx.bookmarksfly.cn

[U67] PHP：处理文件上传
来源：http://zb.jctech888.com.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ks.shxzukj.cn

[U68] PHP：PDO 连接
来源：http://sb.521024.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tl.yuntaijiaju.cn

[U69] PHP：PDO 预处理
来源：http://zm.huixinmuqiang.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bk.lnxyls.cn

[U70] PHP：PDO 事务
来源：http://rn.szsharing.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ew.9csxet.cn

[U71] PHP：抛出异常
来源：http://fu.bookmarksfly.cn

throw new RuntimeException("失败", 500);
来源：http://ip.huixinmuqiang.cn

[U72] PHP：写错误日志
来源：http://lr.newstarts.cn

error_log("失败: " . $e->getMessage());
来源：http://fz.shxzskj.cn

[U73] PHP：读取 ini 配置
来源：http://fe.nszjky.cn

parse_ini_file("config.ini", true)
来源：http://ut.wgjwhj.cn

[U74] PHP：读取环境变量
来源：http://ju.shxzukj.cn

getenv("APP_ENV") ?: "production"
来源：http://fy.yuntaijiaju.cn

[U75] PHP：依赖注入
来源：http://jo.shxzskj.cn

composer require psr/container
来源：http://ng.colortex.cn

[U76] PHP：简单路由
来源：http://iw.nicolike.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qn.huixiangedu.cn

[U77] PHP：模板渲染
来源：http://eu.nszjky.cn

composer require twig/twig
来源：http://ve.hnjuh.cn

[U78] PHP：单元测试
来源：http://bf.wgjwhj.cn

composer require --dev phpunit/phpunit
来源：http://yr.shxzukj.cn

[U79] PHP：静态分析
来源：http://re.gzmigu.cn

composer require --dev phpstan/phpstan
来源：http://wb.szsharing.cn

[U80] PHP：代码规范修复
来源：http://vt.huanxung.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://yh.newstarts.cn

[U81] JS：初始化项目
来源：http://gy.wgjwhj.cn

npm init -y;  npm i express
来源：http://gd.huixiangedu.cn

[U82] JS：package.json 脚本
来源：http://of.colortex.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://po.huixiangedu.cn

[U83] JS：ES Module 导入导出
来源：http://kr.yuexingan06.cn

export const a = 1;  import { a } from "./m.js";
来源：http://at.yuntaijiaju.cn

[U84] JS：CommonJS 写法
来源：http://vc.panjiajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://vi.szxytkj.cn

[U85] JS：可选链
来源：http://va.haigaiapp.cn

a?.b?.c
来源：http://tn.jctech888.com.cn

[U86] JS：空值合并
来源：http://zw.huixinmuqiang.cn

a ?? b
来源：http://tv.szxytkj.cn

[U87] JS：解构默认值
来源：http://iv.szxytkj.cn

const { a = 1, b = 2 } = obj;
来源：http://ew.shtwfgs.cn

[U88] JS：对象展开合并
来源：http://hp.haigaiapp.cn

{ ...a, ...b }
来源：http://ys.asd995.cn

[U89] JS：数组去重
来源：http://sy.chemitech.net.cn

[...new Set(arr)]
来源：http://ez.bookmarksfly.cn

[U90] JS：数字数组排序
来源：http://dq.panjiajie.cn

[...arr].sort((a, b) => a - b)
来源：http://iz.shxzskj.cn

[U91] JS：对象键值遍历
来源：http://bu.shxzskj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ot.hahajie.cn

[U92] JS：深拷贝
来源：http://gf.szxytkj.cn

structuredClone(obj)
来源：http://zi.asd995.cn

[U93] JS：模板字符串
来源：http://ex.yuntaijiaju.cn

`共 ${n} 条`
来源：http://ys.shxzskj.cn

[U94] JS：箭头函数
来源：http://ue.chemitech.net.cn

const double = x => x * 2;
来源：http://iv.muxihuayi.cn

[U95] JS：Promise 包装
来源：http://jo.huixiangedu.cn

new Promise((resolve, reject) => {})
来源：http://gl.huixiangedu.cn

[U96] JS：async/await 与异常
来源：http://lt.huanxung.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sm.panjiajie.cn

[U97] JS：并发请求
来源：http://mj.lnxyls.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://uy.bjjhwx.cn

[U98] JS：fetch 带 JSON
来源：http://gp.wgjwhj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qi.521024.cn

[U99] JS：事件监听
来源：http://ip.asd995.cn

el.addEventListener("click", e => {})
来源：http://ty.jianghongdianzi.cn

[U100] JS：DOM 查询
来源：http://kf.wgjwhj.cn

document.querySelector(".item")
来源：http://rg.colortex.cn

[U101] JS：classList 操作
来源：http://ut.wgjwhj.cn

el.classList.toggle("active")
来源：http://ai.9csxet.cn

[U102] JS：本地存储
来源：http://he.yuntaijiaju.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://fa.huanxung.cn

[U103] JS：定时器
来源：http://jq.jianghongdianzi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hk.bookmarksfly.cn

[U104] JS：防抖
来源：http://ey.szsharing.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wi.521024.cn

[U105] JS：节流
来源：http://qo.huixiangedu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zx.shxzukj.cn

[U106] JS：日期格式化
来源：http://st.yuntaijiaju.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jy.asd995.cn

[U107] JS：数字千分位
来源：http://nl.huanxung.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fl.szxytkj.cn

[U108] JS：随机整数
来源：http://vk.lnxyls.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gj.bjjhwx.cn

[U109] JS：数组分组
来源：http://dv.nicolike.cn

Object.groupBy(arr, x => x.type)
来源：http://iy.shxzukj.cn

[U110] JS：数组分块
来源：http://xy.nszjky.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rs.lnxyls.cn

[U111] JS：对象转 Map
来源：http://fy.jianghongdianzi.cn

new Map(Object.entries(obj))
来源：http://lc.521024.cn

[U112] JS：字符串补位
来源：http://fx.panjiajie.cn

"7".padStart(3, "0")
来源：http://bu.wgjwhj.cn

[U113] JS：正则替换全部
来源：http://hc.gzmigu.cn

s.replaceAll("a", "b")
来源：http://jm.huanxung.cn

[U114] JS：JSON 深比较
来源：http://xu.haigaiapp.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ls.nicolike.cn


<!-- 参考信息 -->