代发 wailian999

[T25] Swift：结构体
来源：http://vb.newstarts.cn

struct P { var x: Int }
来源：http://jc.huixiangedu.cn

[T26] Swift：类与重写
来源：http://vy.bjjhwx.cn

class A: Base { override func f() {} }
来源：http://eu.haigaiapp.cn

[T27] Swift：错误处理
来源：http://an.huixiangedu.cn

do { try f() } catch { print(error) }
来源：http://mx.9csxet.cn

[T28] Swift：枚举
来源：http://os.jctech888.com.cn

enum Color { case red, green }
来源：http://wx.bookmarksfly.cn

[T29] Swift：guard 提前返回
来源：http://fu.yuntaijiaju.cn

guard let x = opt else { return }
来源：http://ld.hahajie.cn

[T30] Swift：协议
来源：http://em.szsharing.cn

protocol Shape { func area() -> Double }
来源：http://xp.szxytkj.cn

[T31] Lua：Hello World
来源：http://ch.colortex.cn

print("Hello")
来源：http://sb.szxytkj.cn

[T32] Lua：局部变量
来源：http://fo.hnjuh.cn

local a = 1
来源：http://zy.jianghongdianzi.cn

[T33] Lua：表（数组）
来源：http://xw.shxzukj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://lm.huixinmuqiang.cn

[T34] Lua：遍历表
来源：http://pd.lnxyls.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://nu.yuexingan06.cn

[T35] Lua：字典表
来源：http://ul.colortex.cn

local d = { a = 1 };  d.b = 2
来源：http://do.hnjuh.cn

[T36] Lua：函数
来源：http://of.521024.cn

function add(a, b) return a + b end
来源：http://bf.yuexingan06.cn

[T37] Lua：字符串拼接
来源：http://hu.gzmigu.cn

"a" .. "b"
来源：http://au.9csxet.cn

[T38] Lua：条件
来源：http://mx.521024.cn

if x > 0 then print("正") end
来源：http://jd.haigaiapp.cn

[T39] Lua：模式匹配
来源：http://yu.haigaiapp.cn

string.find(s, "%d+")
来源：http://xf.521024.cn

[T40] Lua：元表
来源：http://vp.gzmigu.cn

setmetatable({}, { __index = base })
来源：http://hs.muxihuayi.cn

[T41] Perl：Hello World
来源：http://qs.jctech888.com.cn

print "Hello\n";
来源：http://gz.huixiangedu.cn

[T42] Perl：变量类型
来源：http://fw.huixinmuqiang.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tm.hahajie.cn

[T43] Perl：字符串插值
来源：http://tc.colortex.cn

"值: $a"
来源：http://sd.yuexingan06.cn

[T44] Perl：条件
来源：http://mp.chemitech.net.cn

if ($a > 0) { print "正"; }
来源：http://ug.9csxet.cn

[T45] Perl：数组遍历
来源：http://bm.lnxyls.cn

for my $x (@arr) { print $x; }
来源：http://um.yuexingan06.cn

[T46] Perl：哈希操作
来源：http://aj.gzmigu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zn.wgjwhj.cn

[T47] Perl：正则捕获
来源：http://jr.nicolike.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://cq.asd995.cn

[T48] Perl：正则替换
来源：http://hb.szsharing.cn

$s =~ s/old/new/g;
来源：http://bo.szsharing.cn

[T49] Perl：函数
来源：http://zo.huixiangedu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tb.gzmigu.cn

[T50] Perl：逐行读文件
来源：http://ku.huixiangedu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ht.shxzskj.cn

while (my $line = <$fh>) { print $line; }
来源：http://vc.yuntaijiaju.cn

[T51] Scala：Hello World
来源：http://ls.huixiangedu.cn

println("Hello")
来源：http://nb.nszjky.cn

[T52] Scala：变量
来源：http://sb.jctech888.com.cn

val a = 1;  var b = 2
来源：http://hw.nszjky.cn

[T53] Scala：字符串插值
来源：http://hw.newstarts.cn

s"值: $b"
来源：http://yp.hahajie.cn

[T54] Scala：集合映射
来源：http://pj.haigaiapp.cn

List(1, 2, 3).map(_ * 2)
来源：http://ia.bjjhwx.cn

[T55] Scala：集合过滤
来源：http://tg.shtwfgs.cn

List(1, 2, 3).filter(_ > 1)
来源：http://bl.hnjuh.cn

[T56] Scala：样例类
来源：http://kb.521024.cn

case class User(name: String, age: Int)
来源：http://wf.muxihuayi.cn

[T57] Scala：模式匹配
来源：http://dv.yuntaijiaju.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://hl.szxytkj.cn

[T58] Scala：函数定义
来源：http://ux.huixinmuqiang.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ll.hnjuh.cn

[T59] Scala：循环
来源：http://id.lnxyls.cn

for (i <- 1 to 10) println(i)
来源：http://ge.nszjky.cn

[T60] Scala：折叠
来源：http://ty.huanxung.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nq.newstarts.cn

================================================================================
来源：http://go.nszjky.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rd.jianghongdianzi.cn

================================================================================
来源：http://sq.colortex.cn

[U01] Py：创建虚拟环境
来源：http://ar.huanxung.cn

python -m venv .venv && source .venv/bin/activate
来源：http://fn.nicolike.cn

[U02] Py：导出 / 安装依赖
来源：http://nb.haigaiapp.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gx.yuntaijiaju.cn

[U03] Py：加载 .env 配置
来源：http://ko.gzmigu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://vq.jianghongdianzi.cn

[U04] Py：变量调试打印
来源：http://mk.shtwfgs.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ve.haigaiapp.cn

[U05] Py：列表去重且保序
来源：http://jn.asd995.cn

list(dict.fromkeys(arr))
来源：http://of.jctech888.com.cn

[U06] Py：合并两个字典
来源：http://jr.bjjhwx.cn

{**a, **b}
来源：http://jc.hnjuh.cn

[U07] Py：反转字典键值
来源：http://yr.jianghongdianzi.cn

{v: k for k, v in d.items()}
来源：http://nf.newstarts.cn

[U08] Py：展平二维列表
来源：http://ho.bjjhwx.cn

[y for x in nested for y in x]
来源：http://gu.panjiajie.cn

[U09] Py：字典取最大值的键
来源：http://ou.wgjwhj.cn

max(d, key=d.get)
来源：http://ge.hahajie.cn

[U10] Py：按值排序字典
来源：http://oa.jianghongdianzi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cs.huixiangedu.cn

[U11] Py：生成器表达式
来源：http://wc.shxzukj.cn

(x * 2 for x in arr)
来源：http://kx.hnjuh.cn

[U12] Py：取出现最多的 3 个元素
来源：http://od.jianghongdianzi.cn

Counter(arr).most_common(3)
来源：http://ma.asd995.cn

[U13] Py：固定长度队列
来源：http://ge.jianghongdianzi.cn

deque(maxlen=10)
来源：http://mg.colortex.cn

[U14] Py：分组收集到列表
来源：http://su.huanxung.cn

defaultdict(list)
来源：http://mq.bjjhwx.cn

[U15] Py：高精度计时
来源：http://ud.hahajie.cn

t = time.perf_counter()
来源：http://co.jianghongdianzi.cn

[U16] Py：命令行参数解析
来源：http://cp.huixinmuqiang.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sz.hnjuh.cn

[U17] Py：初始化日志
来源：http://vb.gzmigu.cn

logging.basicConfig(level=logging.INFO)
来源：http://he.szxytkj.cn

[U18] Py：预编译正则
来源：http://wt.huixinmuqiang.cn

pat = re.compile(r"\d+")
来源：http://xc.muxihuayi.cn

[U19] Py：正则替换带回调
来源：http://mn.shxzskj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lt.newstarts.cn

[U20] Py：缓存函数结果
来源：http://zv.szxytkj.cn

@functools.lru_cache(maxsize=None)
来源：http://zi.wgjwhj.cn

[U21] Py：自定义上下文管理器
来源：http://da.lnxyls.cn

@contextlib.contextmanager
来源：http://qo.szsharing.cn

[U22] Py：矩阵转置
来源：http://hn.colortex.cn

list(zip(*m))
来源：http://me.haigaiapp.cn

[U23] Py：分块读取大文件
来源：http://aa.haigaiapp.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ho.szsharing.cn

[U24] Py：路径操作
来源：http://il.gzmigu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ln.9csxet.cn

[U25] Py：CSV 按字典读
来源：http://lz.huixiangedu.cn

csv.DictReader(f)
来源：http://ss.szxytkj.cn

[U26] Py：并发下载
来源：http://vv.521024.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://sy.huixiangedu.cn

[U27] Py：异步 HTTP
来源：http://sb.lnxyls.cn

aiohttp.ClientSession() 配合 async with
来源：http://ps.gzmigu.cn

[U28] Py：类型别名
来源：http://gr.muxihuayi.cn

UserId = int
来源：http://sf.521024.cn

[U29] Py：属性校验
来源：http://qb.shxzukj.cn

@property 与 @x.setter 配合
来源：http://wh.hnjuh.cn

[U30] Py：数据类
来源：http://ey.nicolike.cn

@dataclass(slots=True)
来源：http://tk.chemitech.net.cn

[U31] Py：单测
来源：http://py.9csxet.cn

python -m pytest -q
来源：http://xc.521024.cn

[U32] Py：代码格式化
来源：http://wx.shxzukj.cn

ruff format . && ruff check --fix .
来源：http://le.bjjhwx.cn

[U33] Py：打包发布
来源：http://ak.chemitech.net.cn

python -m build  （依赖 pyproject.toml）
来源：http://vr.521024.cn

[U34] Py：判断编码
来源：http://eo.bookmarksfly.cn

chardet.detect(raw)
来源：http://go.nicolike.cn

[U35] Py：发送邮件
来源：http://et.huanxung.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nw.hnjuh.cn

[U36] Py：定时任务
来源：http://ow.muxihuayi.cn

schedule.every(10).minutes.do(job)
来源：http://qh.szsharing.cn

[U37] Py：读写 Excel
来源：http://et.newstarts.cn

pandas.read_excel / DataFrame.to_excel
来源：http://tm.huanxung.cn

[U38] Py：获取脚本所在目录
来源：http://bd.nszjky.cn

Path(__file__).resolve().parent
来源：http://bm.huixiangedu.cn

[U39] Py：判断是否在交互环境
来源：http://fr.panjiajie.cn

sys.stdout.isatty()
来源：http://vq.haigaiapp.cn

[U40] Py：打印到标准错误
来源：http://zj.jctech888.com.cn

print("err", file=sys.stderr)
来源：http://uc.jianghongdianzi.cn

[U41] PHP：初始化 Composer 项目
来源：http://ig.9csxet.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://pc.yuexingan06.cn

[U42] PHP：PSR-4 自动加载
来源：http://nt.lnxyls.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nv.521024.cn

[U43] PHP：声明命名空间
来源：http://ah.yuntaijiaju.cn

namespace App\Http;
来源：http://bs.huanxung.cn

[U44] PHP：开启严格类型
来源：http://hu.muxihuayi.cn

declare(strict_types=1);
来源：http://gg.shxzskj.cn

[U45] PHP：类型声明与返回类型
来源：http://ga.nszjky.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ax.huixiangedu.cn

[U46] PHP：可空类型
来源：http://ok.9csxet.cn

?string $name = null
来源：http://ju.yuntaijiaju.cn

[U47] PHP：联合类型
来源：http://xk.jianghongdianzi.cn

int|string $id
来源：http://lz.huanxung.cn

[U48] PHP：纯枚举
来源：http://zj.gzmigu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://et.panjiajie.cn

[U49] PHP：只读属性
来源：http://uc.lnxyls.cn

public readonly string $name
来源：http://rt.huixiangedu.cn

[U50] PHP：构造器属性提升
来源：http://jm.lnxyls.cn

public function __construct(private int $id) {}
来源：http://wi.haigaiapp.cn

[U51] PHP：数组解构
来源：http://me.muxihuayi.cn

[$a, $b] = $arr;
来源：http://hj.chemitech.net.cn

[U52] PHP：箭头函数
来源：http://ek.yuntaijiaju.cn

$double = fn($x) => $x * 2;
来源：http://ra.huixiangedu.cn

[U53] PHP：空合并运算符
来源：http://qa.jctech888.com.cn

$v = $a ?? $b ?? "default";
来源：http://jh.szxytkj.cn

[U54] PHP：空安全调用
来源：http://cy.bjjhwx.cn

$obj?->method()
来源：http://vv.hnjuh.cn

[U55] PHP：match 表达式
来源：http://hu.shxzskj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qe.shxzskj.cn

[U56] PHP：命名参数
来源：http://wi.asd995.cn

f(a: 1, b: 2)
来源：http://tx.shxzskj.cn

[U57] PHP：字符串插值
来源：http://ag.nicolike.cn

"值: {$a}"
来源：http://gz.muxihuayi.cn

[U58] PHP：数组三件套
来源：http://ak.nicolike.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wu.jianghongdianzi.cn

[U59] PHP：自定义排序
来源：http://qr.gzmigu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yg.jctech888.com.cn

[U60] PHP：JSON 编解码
来源：http://ca.shtwfgs.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qj.521024.cn

[U61] PHP：正则
来源：http://ko.asd995.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fz.yuntaijiaju.cn

[U62] PHP：日期对象
来源：http://lp.shxzskj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dz.yuexingan06.cn

[U63] PHP：文件读写
来源：http://nh.muxihuayi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pj.yuntaijiaju.cn

[U64] PHP：目录遍历
来源：http://ub.521024.cn

glob("dir/*.php");  scandir("dir");
来源：http://et.huanxung.cn

[U65] PHP：会话
来源：http://xn.nicolike.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://sx.hnjuh.cn

[U66] PHP：设置 Cookie
来源：http://cq.yuexingan06.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ts.lnxyls.cn

[U67] PHP：处理文件上传
来源：http://no.521024.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rh.lnxyls.cn

[U68] PHP：PDO 连接
来源：http://ja.hnjuh.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ra.huanxung.cn

[U69] PHP：PDO 预处理
来源：http://mo.shxzskj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rr.asd995.cn

[U70] PHP：PDO 事务
来源：http://mx.jctech888.com.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ge.panjiajie.cn

[U71] PHP：抛出异常
来源：http://qy.shtwfgs.cn

throw new RuntimeException("失败", 500);
来源：http://md.szxytkj.cn

[U72] PHP：写错误日志
来源：http://hw.szxytkj.cn

error_log("失败: " . $e->getMessage());
来源：http://ki.huanxung.cn

[U73] PHP：读取 ini 配置
来源：http://he.bookmarksfly.cn

parse_ini_file("config.ini", true)
来源：http://kh.jctech888.com.cn

[U74] PHP：读取环境变量
来源：http://ju.huixinmuqiang.cn

getenv("APP_ENV") ?: "production"
来源：http://hg.hnjuh.cn

[U75] PHP：依赖注入
来源：http://zs.lnxyls.cn

composer require psr/container
来源：http://me.jctech888.com.cn

[U76] PHP：简单路由
来源：http://zy.huixiangedu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wq.jctech888.com.cn

[U77] PHP：模板渲染
来源：http://gs.haigaiapp.cn

composer require twig/twig
来源：http://na.hahajie.cn

[U78] PHP：单元测试
来源：http://xt.huixiangedu.cn

composer require --dev phpunit/phpunit
来源：http://xo.yuexingan06.cn

[U79] PHP：静态分析
来源：http://hr.yuntaijiaju.cn

composer require --dev phpstan/phpstan
来源：http://vs.yuexingan06.cn

[U80] PHP：代码规范修复
来源：http://mb.hahajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://sa.bjjhwx.cn

[U81] JS：初始化项目
来源：http://ks.hahajie.cn

npm init -y;  npm i express
来源：http://ac.yuexingan06.cn

[U82] JS：package.json 脚本
来源：http://zc.bjjhwx.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://of.wgjwhj.cn

[U83] JS：ES Module 导入导出
来源：http://zq.huixinmuqiang.cn

export const a = 1;  import { a } from "./m.js";
来源：http://sb.bookmarksfly.cn

[U84] JS：CommonJS 写法
来源：http://jz.yuexingan06.cn

module.exports = { a };  const { a } = require("./m");
来源：http://nw.szsharing.cn

[U85] JS：可选链
来源：http://qp.haigaiapp.cn

a?.b?.c
来源：http://cn.yuntaijiaju.cn

[U86] JS：空值合并
来源：http://xm.nicolike.cn

a ?? b
来源：http://on.shtwfgs.cn

[U87] JS：解构默认值
来源：http://xw.panjiajie.cn

const { a = 1, b = 2 } = obj;
来源：http://sx.huixiangedu.cn

[U88] JS：对象展开合并
来源：http://sm.bjjhwx.cn

{ ...a, ...b }
来源：http://hm.yuntaijiaju.cn

[U89] JS：数组去重
来源：http://dk.shxzskj.cn

[...new Set(arr)]
来源：http://fp.yuntaijiaju.cn

[U90] JS：数字数组排序
来源：http://uj.521024.cn

[...arr].sort((a, b) => a - b)
来源：http://bg.nicolike.cn

[U91] JS：对象键值遍历
来源：http://gp.szsharing.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cb.nszjky.cn

[U92] JS：深拷贝
来源：http://oc.yuntaijiaju.cn

structuredClone(obj)
来源：http://vz.bookmarksfly.cn

[U93] JS：模板字符串
来源：http://bp.bookmarksfly.cn

`共 ${n} 条`
来源：http://fk.hahajie.cn

[U94] JS：箭头函数
来源：http://ct.chemitech.net.cn

const double = x => x * 2;
来源：http://pt.shtwfgs.cn

[U95] JS：Promise 包装
来源：http://nq.nszjky.cn

new Promise((resolve, reject) => {})
来源：http://qd.colortex.cn

[U96] JS：async/await 与异常
来源：http://ez.muxihuayi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cj.shtwfgs.cn

[U97] JS：并发请求
来源：http://jm.huanxung.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ee.hnjuh.cn

[U98] JS：fetch 带 JSON
来源：http://py.szxytkj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vv.nicolike.cn

[U99] JS：事件监听
来源：http://my.newstarts.cn

el.addEventListener("click", e => {})
来源：http://gc.szxytkj.cn

[U100] JS：DOM 查询
来源：http://bm.jianghongdianzi.cn

document.querySelector(".item")
来源：http://yf.shxzukj.cn

[U101] JS：classList 操作
来源：http://fq.muxihuayi.cn

el.classList.toggle("active")
来源：http://mc.chemitech.net.cn

[U102] JS：本地存储
来源：http://ro.lnxyls.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://mu.huixinmuqiang.cn

[U103] JS：定时器
来源：http://dr.shxzskj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://eh.shtwfgs.cn

[U104] JS：防抖
来源：http://bh.colortex.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tf.muxihuayi.cn

[U105] JS：节流
来源：http://cb.jctech888.com.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lh.bjjhwx.cn

[U106] JS：日期格式化
来源：http://yy.wgjwhj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sh.nszjky.cn

[U107] JS：数字千分位
来源：http://uu.newstarts.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tb.huixinmuqiang.cn

[U108] JS：随机整数
来源：http://be.bjjhwx.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bx.wgjwhj.cn

[U109] JS：数组分组
来源：http://ea.lnxyls.cn

Object.groupBy(arr, x => x.type)
来源：http://oy.wgjwhj.cn

[U110] JS：数组分块
来源：http://ty.hnjuh.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://og.bjjhwx.cn

[U111] JS：对象转 Map
来源：http://nc.nicolike.cn

new Map(Object.entries(obj))
来源：http://qh.shtwfgs.cn

[U112] JS：字符串补位
来源：http://jj.hnjuh.cn

"7".padStart(3, "0")
来源：http://ox.hahajie.cn


<!-- 参考信息 -->