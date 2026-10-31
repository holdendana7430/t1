代发 wailian999

[T27] Swift：错误处理
来源：http://mp.shxzukj.cn

do { try f() } catch { print(error) }
来源：http://cv.hnjuh.cn

[T28] Swift：枚举
来源：http://jq.asd995.cn

enum Color { case red, green }
来源：http://ij.szsharing.cn

[T29] Swift：guard 提前返回
来源：http://qf.yuntaijiaju.cn

guard let x = opt else { return }
来源：http://rr.wgjwhj.cn

[T30] Swift：协议
来源：http://ia.gzmigu.cn

protocol Shape { func area() -> Double }
来源：http://ok.panjiajie.cn

[T31] Lua：Hello World
来源：http://qq.bookmarksfly.cn

print("Hello")
来源：http://zt.yuexingan06.cn

[T32] Lua：局部变量
来源：http://yn.newstarts.cn

local a = 1
来源：http://sa.huixinmuqiang.cn

[T33] Lua：表（数组）
来源：http://zk.bjjhwx.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://br.hahajie.cn

[T34] Lua：遍历表
来源：http://ax.huanxung.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://hc.nszjky.cn

[T35] Lua：字典表
来源：http://ch.asd995.cn

local d = { a = 1 };  d.b = 2
来源：http://gz.szxytkj.cn

[T36] Lua：函数
来源：http://tc.9csxet.cn

function add(a, b) return a + b end
来源：http://gc.yuexingan06.cn

[T37] Lua：字符串拼接
来源：http://dk.szxytkj.cn

"a" .. "b"
来源：http://jf.szsharing.cn

[T38] Lua：条件
来源：http://nb.hahajie.cn

if x > 0 then print("正") end
来源：http://dt.yuexingan06.cn

[T39] Lua：模式匹配
来源：http://dj.hnjuh.cn

string.find(s, "%d+")
来源：http://tj.huixinmuqiang.cn

[T40] Lua：元表
来源：http://ej.shtwfgs.cn

setmetatable({}, { __index = base })
来源：http://jg.bjjhwx.cn

[T41] Perl：Hello World
来源：http://xg.jctech888.com.cn

print "Hello\n";
来源：http://up.newstarts.cn

[T42] Perl：变量类型
来源：http://rz.szsharing.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://we.panjiajie.cn

[T43] Perl：字符串插值
来源：http://pq.huixinmuqiang.cn

"值: $a"
来源：http://mi.shxzukj.cn

[T44] Perl：条件
来源：http://ga.chemitech.net.cn

if ($a > 0) { print "正"; }
来源：http://gj.huixinmuqiang.cn

[T45] Perl：数组遍历
来源：http://mg.panjiajie.cn

for my $x (@arr) { print $x; }
来源：http://mk.bjjhwx.cn

[T46] Perl：哈希操作
来源：http://fa.shxzukj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tf.haigaiapp.cn

[T47] Perl：正则捕获
来源：http://hb.9csxet.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ls.szsharing.cn

[T48] Perl：正则替换
来源：http://ti.shxzskj.cn

$s =~ s/old/new/g;
来源：http://kc.shxzukj.cn

[T49] Perl：函数
来源：http://zy.nicolike.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ju.shxzukj.cn

[T50] Perl：逐行读文件
来源：http://vb.bjjhwx.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ew.haigaiapp.cn

while (my $line = <$fh>) { print $line; }
来源：http://oc.jianghongdianzi.cn

[T51] Scala：Hello World
来源：http://fh.nicolike.cn

println("Hello")
来源：http://vf.panjiajie.cn

[T52] Scala：变量
来源：http://zb.muxihuayi.cn

val a = 1;  var b = 2
来源：http://un.haigaiapp.cn

[T53] Scala：字符串插值
来源：http://be.9csxet.cn

s"值: $b"
来源：http://jo.asd995.cn

[T54] Scala：集合映射
来源：http://in.newstarts.cn

List(1, 2, 3).map(_ * 2)
来源：http://dj.huixiangedu.cn

[T55] Scala：集合过滤
来源：http://hh.wgjwhj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://oy.bookmarksfly.cn

[T56] Scala：样例类
来源：http://bo.yuexingan06.cn

case class User(name: String, age: Int)
来源：http://xo.bjjhwx.cn

[T57] Scala：模式匹配
来源：http://df.huixinmuqiang.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wr.shtwfgs.cn

[T58] Scala：函数定义
来源：http://bq.yuexingan06.cn

def add(a: Int, b: Int): Int = a + b
来源：http://rh.nszjky.cn

[T59] Scala：循环
来源：http://ln.huixiangedu.cn

for (i <- 1 to 10) println(i)
来源：http://va.nszjky.cn

[T60] Scala：折叠
来源：http://ov.asd995.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ro.shxzskj.cn

================================================================================
来源：http://li.hnjuh.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rb.haigaiapp.cn

================================================================================
来源：http://ql.muxihuayi.cn

[U01] Py：创建虚拟环境
来源：http://wj.jctech888.com.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bk.szsharing.cn

[U02] Py：导出 / 安装依赖
来源：http://yq.wgjwhj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cs.lnxyls.cn

[U03] Py：加载 .env 配置
来源：http://yt.asd995.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zh.yuexingan06.cn

[U04] Py：变量调试打印
来源：http://wd.shxzukj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nm.521024.cn

[U05] Py：列表去重且保序
来源：http://tq.colortex.cn

list(dict.fromkeys(arr))
来源：http://gb.9csxet.cn

[U06] Py：合并两个字典
来源：http://td.bookmarksfly.cn

{**a, **b}
来源：http://qx.chemitech.net.cn

[U07] Py：反转字典键值
来源：http://qg.muxihuayi.cn

{v: k for k, v in d.items()}
来源：http://ee.wgjwhj.cn

[U08] Py：展平二维列表
来源：http://ib.jctech888.com.cn

[y for x in nested for y in x]
来源：http://qq.huixiangedu.cn

[U09] Py：字典取最大值的键
来源：http://ch.shxzukj.cn

max(d, key=d.get)
来源：http://zl.9csxet.cn

[U10] Py：按值排序字典
来源：http://pv.bjjhwx.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ph.hahajie.cn

[U11] Py：生成器表达式
来源：http://mw.yuntaijiaju.cn

(x * 2 for x in arr)
来源：http://vd.wgjwhj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://gu.hnjuh.cn

Counter(arr).most_common(3)
来源：http://tf.newstarts.cn

[U13] Py：固定长度队列
来源：http://yb.9csxet.cn

deque(maxlen=10)
来源：http://ga.bookmarksfly.cn

[U14] Py：分组收集到列表
来源：http://pr.asd995.cn

defaultdict(list)
来源：http://nf.huixinmuqiang.cn

[U15] Py：高精度计时
来源：http://zp.nicolike.cn

t = time.perf_counter()
来源：http://hk.wgjwhj.cn

[U16] Py：命令行参数解析
来源：http://dv.bookmarksfly.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vg.nszjky.cn

[U17] Py：初始化日志
来源：http://cx.chemitech.net.cn

logging.basicConfig(level=logging.INFO)
来源：http://at.hnjuh.cn

[U18] Py：预编译正则
来源：http://yz.shxzskj.cn

pat = re.compile(r"\d+")
来源：http://ja.yuntaijiaju.cn

[U19] Py：正则替换带回调
来源：http://sp.newstarts.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://es.hnjuh.cn

[U20] Py：缓存函数结果
来源：http://kq.hnjuh.cn

@functools.lru_cache(maxsize=None)
来源：http://bs.huixinmuqiang.cn

[U21] Py：自定义上下文管理器
来源：http://jc.521024.cn

@contextlib.contextmanager
来源：http://jo.nicolike.cn

[U22] Py：矩阵转置
来源：http://uw.yuntaijiaju.cn

list(zip(*m))
来源：http://lb.haigaiapp.cn

[U23] Py：分块读取大文件
来源：http://tw.haigaiapp.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lr.bjjhwx.cn

[U24] Py：路径操作
来源：http://us.colortex.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zs.9csxet.cn

[U25] Py：CSV 按字典读
来源：http://mg.yuntaijiaju.cn

csv.DictReader(f)
来源：http://qt.521024.cn

[U26] Py：并发下载
来源：http://pr.asd995.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xw.bookmarksfly.cn

[U27] Py：异步 HTTP
来源：http://ga.wgjwhj.cn

aiohttp.ClientSession() 配合 async with
来源：http://tn.jianghongdianzi.cn

[U28] Py：类型别名
来源：http://fa.huixinmuqiang.cn

UserId = int
来源：http://iq.yuexingan06.cn

[U29] Py：属性校验
来源：http://jw.muxihuayi.cn

@property 与 @x.setter 配合
来源：http://em.muxihuayi.cn

[U30] Py：数据类
来源：http://ci.szsharing.cn

@dataclass(slots=True)
来源：http://gb.bookmarksfly.cn

[U31] Py：单测
来源：http://pk.huixinmuqiang.cn

python -m pytest -q
来源：http://ee.szsharing.cn

[U32] Py：代码格式化
来源：http://ue.huanxung.cn

ruff format . && ruff check --fix .
来源：http://ok.colortex.cn

[U33] Py：打包发布
来源：http://xc.yuexingan06.cn

python -m build  （依赖 pyproject.toml）
来源：http://af.yuexingan06.cn

[U34] Py：判断编码
来源：http://nt.nicolike.cn

chardet.detect(raw)
来源：http://hl.nszjky.cn

[U35] Py：发送邮件
来源：http://pb.yuexingan06.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tj.hahajie.cn

[U36] Py：定时任务
来源：http://vc.hahajie.cn

schedule.every(10).minutes.do(job)
来源：http://ob.nszjky.cn

[U37] Py：读写 Excel
来源：http://au.hahajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jn.lnxyls.cn

[U38] Py：获取脚本所在目录
来源：http://ha.hnjuh.cn

Path(__file__).resolve().parent
来源：http://en.panjiajie.cn

[U39] Py：判断是否在交互环境
来源：http://sb.nicolike.cn

sys.stdout.isatty()
来源：http://ni.hahajie.cn

[U40] Py：打印到标准错误
来源：http://er.huanxung.cn

print("err", file=sys.stderr)
来源：http://er.huanxung.cn

[U41] PHP：初始化 Composer 项目
来源：http://hz.haigaiapp.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://yw.lnxyls.cn

[U42] PHP：PSR-4 自动加载
来源：http://db.jctech888.com.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yd.nicolike.cn

[U43] PHP：声明命名空间
来源：http://jk.asd995.cn

namespace App\Http;
来源：http://dc.newstarts.cn

[U44] PHP：开启严格类型
来源：http://oi.asd995.cn

declare(strict_types=1);
来源：http://lx.jianghongdianzi.cn

[U45] PHP：类型声明与返回类型
来源：http://yy.jctech888.com.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://np.lnxyls.cn

[U46] PHP：可空类型
来源：http://xn.9csxet.cn

?string $name = null
来源：http://rm.huanxung.cn

[U47] PHP：联合类型
来源：http://as.muxihuayi.cn

int|string $id
来源：http://ne.nszjky.cn

[U48] PHP：纯枚举
来源：http://oh.szxytkj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bg.shtwfgs.cn

[U49] PHP：只读属性
来源：http://pu.hahajie.cn

public readonly string $name
来源：http://go.521024.cn

[U50] PHP：构造器属性提升
来源：http://uc.asd995.cn

public function __construct(private int $id) {}
来源：http://lm.jianghongdianzi.cn

[U51] PHP：数组解构
来源：http://in.hnjuh.cn

[$a, $b] = $arr;
来源：http://li.panjiajie.cn

[U52] PHP：箭头函数
来源：http://ti.colortex.cn

$double = fn($x) => $x * 2;
来源：http://mb.szxytkj.cn

[U53] PHP：空合并运算符
来源：http://uz.huixinmuqiang.cn

$v = $a ?? $b ?? "default";
来源：http://cf.colortex.cn

[U54] PHP：空安全调用
来源：http://ew.9csxet.cn

$obj?->method()
来源：http://au.huixiangedu.cn

[U55] PHP：match 表达式
来源：http://mw.bjjhwx.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rt.asd995.cn

[U56] PHP：命名参数
来源：http://ch.newstarts.cn

f(a: 1, b: 2)
来源：http://gd.yuntaijiaju.cn

[U57] PHP：字符串插值
来源：http://qd.yuntaijiaju.cn

"值: {$a}"
来源：http://ox.jianghongdianzi.cn

[U58] PHP：数组三件套
来源：http://uw.521024.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mj.haigaiapp.cn

[U59] PHP：自定义排序
来源：http://gp.yuexingan06.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ww.bjjhwx.cn

[U60] PHP：JSON 编解码
来源：http://mh.jianghongdianzi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pn.asd995.cn

[U61] PHP：正则
来源：http://jk.szsharing.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ct.bjjhwx.cn

[U62] PHP：日期对象
来源：http://tz.shxzskj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ck.haigaiapp.cn

[U63] PHP：文件读写
来源：http://vk.521024.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rh.panjiajie.cn

[U64] PHP：目录遍历
来源：http://yd.bookmarksfly.cn

glob("dir/*.php");  scandir("dir");
来源：http://gs.hnjuh.cn

[U65] PHP：会话
来源：http://cw.521024.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ca.szsharing.cn

[U66] PHP：设置 Cookie
来源：http://rk.9csxet.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ey.panjiajie.cn

[U67] PHP：处理文件上传
来源：http://wp.szsharing.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://uy.yuntaijiaju.cn

[U68] PHP：PDO 连接
来源：http://lx.jctech888.com.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ko.newstarts.cn

[U69] PHP：PDO 预处理
来源：http://xy.nszjky.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nn.bjjhwx.cn

[U70] PHP：PDO 事务
来源：http://kn.chemitech.net.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gg.bookmarksfly.cn

[U71] PHP：抛出异常
来源：http://bl.9csxet.cn

throw new RuntimeException("失败", 500);
来源：http://yz.lnxyls.cn

[U72] PHP：写错误日志
来源：http://pt.nszjky.cn

error_log("失败: " . $e->getMessage());
来源：http://rj.chemitech.net.cn

[U73] PHP：读取 ini 配置
来源：http://hp.huanxung.cn

parse_ini_file("config.ini", true)
来源：http://zi.bjjhwx.cn

[U74] PHP：读取环境变量
来源：http://wk.hahajie.cn

getenv("APP_ENV") ?: "production"
来源：http://pn.521024.cn

[U75] PHP：依赖注入
来源：http://mq.lnxyls.cn

composer require psr/container
来源：http://se.521024.cn

[U76] PHP：简单路由
来源：http://bb.muxihuayi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ez.szsharing.cn

[U77] PHP：模板渲染
来源：http://zw.nicolike.cn

composer require twig/twig
来源：http://pc.lnxyls.cn

[U78] PHP：单元测试
来源：http://lu.huixiangedu.cn

composer require --dev phpunit/phpunit
来源：http://zz.yuntaijiaju.cn

[U79] PHP：静态分析
来源：http://yx.9csxet.cn

composer require --dev phpstan/phpstan
来源：http://ar.521024.cn

[U80] PHP：代码规范修复
来源：http://oj.haigaiapp.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://el.wgjwhj.cn

[U81] JS：初始化项目
来源：http://db.yuexingan06.cn

npm init -y;  npm i express
来源：http://ra.9csxet.cn

[U82] JS：package.json 脚本
来源：http://gm.521024.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fl.huanxung.cn

[U83] JS：ES Module 导入导出
来源：http://eq.haigaiapp.cn

export const a = 1;  import { a } from "./m.js";
来源：http://aq.asd995.cn

[U84] JS：CommonJS 写法
来源：http://bo.chemitech.net.cn

module.exports = { a };  const { a } = require("./m");
来源：http://dg.newstarts.cn

[U85] JS：可选链
来源：http://qk.yuexingan06.cn

a?.b?.c
来源：http://xu.szsharing.cn

[U86] JS：空值合并
来源：http://xr.szxytkj.cn

a ?? b
来源：http://bz.muxihuayi.cn

[U87] JS：解构默认值
来源：http://qc.nszjky.cn

const { a = 1, b = 2 } = obj;
来源：http://ek.521024.cn

[U88] JS：对象展开合并
来源：http://xu.lnxyls.cn

{ ...a, ...b }
来源：http://fl.wgjwhj.cn

[U89] JS：数组去重
来源：http://do.yuexingan06.cn

[...new Set(arr)]
来源：http://cq.lnxyls.cn

[U90] JS：数字数组排序
来源：http://ig.yuntaijiaju.cn

[...arr].sort((a, b) => a - b)
来源：http://to.haigaiapp.cn

[U91] JS：对象键值遍历
来源：http://jj.nicolike.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://go.shxzskj.cn

[U92] JS：深拷贝
来源：http://la.jianghongdianzi.cn

structuredClone(obj)
来源：http://cn.shxzukj.cn

[U93] JS：模板字符串
来源：http://vv.gzmigu.cn

`共 ${n} 条`
来源：http://gc.asd995.cn

[U94] JS：箭头函数
来源：http://ym.chemitech.net.cn

const double = x => x * 2;
来源：http://ln.bjjhwx.cn

[U95] JS：Promise 包装
来源：http://nb.panjiajie.cn

new Promise((resolve, reject) => {})
来源：http://fj.gzmigu.cn

[U96] JS：async/await 与异常
来源：http://uu.gzmigu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://aw.shtwfgs.cn

[U97] JS：并发请求
来源：http://tr.huixinmuqiang.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://nu.haigaiapp.cn

[U98] JS：fetch 带 JSON
来源：http://sc.nszjky.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://sa.hahajie.cn

[U99] JS：事件监听
来源：http://ri.chemitech.net.cn

el.addEventListener("click", e => {})
来源：http://gf.yuexingan06.cn

[U100] JS：DOM 查询
来源：http://fc.jctech888.com.cn

document.querySelector(".item")
来源：http://bf.panjiajie.cn

[U101] JS：classList 操作
来源：http://sh.szsharing.cn

el.classList.toggle("active")
来源：http://sz.bjjhwx.cn

[U102] JS：本地存储
来源：http://ul.huanxung.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://gq.hnjuh.cn

[U103] JS：定时器
来源：http://jp.huixiangedu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uc.panjiajie.cn

[U104] JS：防抖
来源：http://oo.colortex.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ds.nszjky.cn

[U105] JS：节流
来源：http://fq.yuntaijiaju.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://je.szsharing.cn

[U106] JS：日期格式化
来源：http://cy.newstarts.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ex.hnjuh.cn

[U107] JS：数字千分位
来源：http://cp.shtwfgs.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ks.newstarts.cn

[U108] JS：随机整数
来源：http://rz.wgjwhj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lw.newstarts.cn

[U109] JS：数组分组
来源：http://ft.szxytkj.cn

Object.groupBy(arr, x => x.type)
来源：http://fg.nszjky.cn

[U110] JS：数组分块
来源：http://ev.huixinmuqiang.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ox.hnjuh.cn

[U111] JS：对象转 Map
来源：http://eh.wgjwhj.cn

new Map(Object.entries(obj))
来源：http://gn.newstarts.cn

[U112] JS：字符串补位
来源：http://zg.gzmigu.cn

"7".padStart(3, "0")
来源：http://ew.shxzskj.cn

[U113] JS：正则替换全部
来源：http://ll.chemitech.net.cn

s.replaceAll("a", "b")
来源：http://qz.huanxung.cn

[U114] JS：JSON 深比较
来源：http://en.shxzukj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://sx.521024.cn


<!-- 参考信息 -->