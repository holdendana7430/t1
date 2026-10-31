代发 wailian999

[T27] Swift：错误处理
来源：http://dt.szsharing.cn

do { try f() } catch { print(error) }
来源：http://vj.shxzukj.cn

[T28] Swift：枚举
来源：http://qy.hahajie.cn

enum Color { case red, green }
来源：http://cr.bjjhwx.cn

[T29] Swift：guard 提前返回
来源：http://mu.yuntaijiaju.cn

guard let x = opt else { return }
来源：http://pj.jianghongdianzi.cn

[T30] Swift：协议
来源：http://vx.huixinmuqiang.cn

protocol Shape { func area() -> Double }
来源：http://ov.nszjky.cn

[T31] Lua：Hello World
来源：http://po.szxytkj.cn

print("Hello")
来源：http://ix.colortex.cn

[T32] Lua：局部变量
来源：http://dc.muxihuayi.cn

local a = 1
来源：http://sm.bjjhwx.cn

[T33] Lua：表（数组）
来源：http://ls.nszjky.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://qn.lnxyls.cn

[T34] Lua：遍历表
来源：http://ca.bjjhwx.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://we.yuntaijiaju.cn

[T35] Lua：字典表
来源：http://dz.huixinmuqiang.cn

local d = { a = 1 };  d.b = 2
来源：http://ew.hnjuh.cn

[T36] Lua：函数
来源：http://gu.yuexingan06.cn

function add(a, b) return a + b end
来源：http://ov.huanxung.cn

[T37] Lua：字符串拼接
来源：http://pa.huixiangedu.cn

"a" .. "b"
来源：http://tt.szsharing.cn

[T38] Lua：条件
来源：http://yh.szsharing.cn

if x > 0 then print("正") end
来源：http://zz.yuntaijiaju.cn

[T39] Lua：模式匹配
来源：http://ec.colortex.cn

string.find(s, "%d+")
来源：http://vw.chemitech.net.cn

[T40] Lua：元表
来源：http://jx.asd995.cn

setmetatable({}, { __index = base })
来源：http://sg.hnjuh.cn

[T41] Perl：Hello World
来源：http://og.wgjwhj.cn

print "Hello\n";
来源：http://fr.jianghongdianzi.cn

[T42] Perl：变量类型
来源：http://di.jctech888.com.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ke.9csxet.cn

[T43] Perl：字符串插值
来源：http://tz.huixinmuqiang.cn

"值: $a"
来源：http://yu.huanxung.cn

[T44] Perl：条件
来源：http://us.hahajie.cn

if ($a > 0) { print "正"; }
来源：http://as.bookmarksfly.cn

[T45] Perl：数组遍历
来源：http://zt.shtwfgs.cn

for my $x (@arr) { print $x; }
来源：http://ob.shtwfgs.cn

[T46] Perl：哈希操作
来源：http://dz.yuntaijiaju.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fs.huixiangedu.cn

[T47] Perl：正则捕获
来源：http://nr.bookmarksfly.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://hv.9csxet.cn

[T48] Perl：正则替换
来源：http://xd.yuntaijiaju.cn

$s =~ s/old/new/g;
来源：http://qj.bjjhwx.cn

[T49] Perl：函数
来源：http://kd.muxihuayi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fc.huixiangedu.cn

[T50] Perl：逐行读文件
来源：http://ym.huixiangedu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zh.shtwfgs.cn

while (my $line = <$fh>) { print $line; }
来源：http://wb.bjjhwx.cn

[T51] Scala：Hello World
来源：http://pz.newstarts.cn

println("Hello")
来源：http://qq.nicolike.cn

[T52] Scala：变量
来源：http://ul.nicolike.cn

val a = 1;  var b = 2
来源：http://ho.szxytkj.cn

[T53] Scala：字符串插值
来源：http://yd.521024.cn

s"值: $b"
来源：http://rw.muxihuayi.cn

[T54] Scala：集合映射
来源：http://yq.hnjuh.cn

List(1, 2, 3).map(_ * 2)
来源：http://fa.hnjuh.cn

[T55] Scala：集合过滤
来源：http://xe.wgjwhj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://zl.huixinmuqiang.cn

[T56] Scala：样例类
来源：http://qz.yuntaijiaju.cn

case class User(name: String, age: Int)
来源：http://tb.yuexingan06.cn

[T57] Scala：模式匹配
来源：http://mh.panjiajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ij.chemitech.net.cn

[T58] Scala：函数定义
来源：http://mq.bjjhwx.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zl.wgjwhj.cn

[T59] Scala：循环
来源：http://tl.shxzskj.cn

for (i <- 1 to 10) println(i)
来源：http://ob.haigaiapp.cn

[T60] Scala：折叠
来源：http://fb.hnjuh.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://eu.gzmigu.cn

================================================================================
来源：http://zu.9csxet.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yi.newstarts.cn

================================================================================
来源：http://xr.lnxyls.cn

[U01] Py：创建虚拟环境
来源：http://kb.shxzukj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ta.gzmigu.cn

[U02] Py：导出 / 安装依赖
来源：http://kg.hnjuh.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hn.colortex.cn

[U03] Py：加载 .env 配置
来源：http://tb.9csxet.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://sr.shxzukj.cn

[U04] Py：变量调试打印
来源：http://va.lnxyls.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gl.shxzskj.cn

[U05] Py：列表去重且保序
来源：http://lc.chemitech.net.cn

list(dict.fromkeys(arr))
来源：http://oc.chemitech.net.cn

[U06] Py：合并两个字典
来源：http://kq.jctech888.com.cn

{**a, **b}
来源：http://dq.chemitech.net.cn

[U07] Py：反转字典键值
来源：http://nj.panjiajie.cn

{v: k for k, v in d.items()}
来源：http://ua.hahajie.cn

[U08] Py：展平二维列表
来源：http://bz.shxzukj.cn

[y for x in nested for y in x]
来源：http://jp.muxihuayi.cn

[U09] Py：字典取最大值的键
来源：http://wv.haigaiapp.cn

max(d, key=d.get)
来源：http://fr.hnjuh.cn

[U10] Py：按值排序字典
来源：http://op.panjiajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ii.bjjhwx.cn

[U11] Py：生成器表达式
来源：http://bb.hahajie.cn

(x * 2 for x in arr)
来源：http://iv.521024.cn

[U12] Py：取出现最多的 3 个元素
来源：http://cp.yuexingan06.cn

Counter(arr).most_common(3)
来源：http://my.hahajie.cn

[U13] Py：固定长度队列
来源：http://uc.shtwfgs.cn

deque(maxlen=10)
来源：http://eb.asd995.cn

[U14] Py：分组收集到列表
来源：http://fz.chemitech.net.cn

defaultdict(list)
来源：http://jb.yuexingan06.cn

[U15] Py：高精度计时
来源：http://yj.huixinmuqiang.cn

t = time.perf_counter()
来源：http://ba.colortex.cn

[U16] Py：命令行参数解析
来源：http://rg.yuexingan06.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jx.asd995.cn

[U17] Py：初始化日志
来源：http://dx.shtwfgs.cn

logging.basicConfig(level=logging.INFO)
来源：http://jt.9csxet.cn

[U18] Py：预编译正则
来源：http://uh.nicolike.cn

pat = re.compile(r"\d+")
来源：http://ey.hnjuh.cn

[U19] Py：正则替换带回调
来源：http://gr.yuntaijiaju.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cw.newstarts.cn

[U20] Py：缓存函数结果
来源：http://ac.colortex.cn

@functools.lru_cache(maxsize=None)
来源：http://ds.gzmigu.cn

[U21] Py：自定义上下文管理器
来源：http://gr.hahajie.cn

@contextlib.contextmanager
来源：http://ja.newstarts.cn

[U22] Py：矩阵转置
来源：http://gh.yuexingan06.cn

list(zip(*m))
来源：http://fc.huixinmuqiang.cn

[U23] Py：分块读取大文件
来源：http://cm.haigaiapp.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://oo.9csxet.cn

[U24] Py：路径操作
来源：http://mf.haigaiapp.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vb.lnxyls.cn

[U25] Py：CSV 按字典读
来源：http://rd.haigaiapp.cn

csv.DictReader(f)
来源：http://kw.asd995.cn

[U26] Py：并发下载
来源：http://lp.huixiangedu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://eo.panjiajie.cn

[U27] Py：异步 HTTP
来源：http://rh.haigaiapp.cn

aiohttp.ClientSession() 配合 async with
来源：http://fa.haigaiapp.cn

[U28] Py：类型别名
来源：http://ow.huanxung.cn

UserId = int
来源：http://td.521024.cn

[U29] Py：属性校验
来源：http://zk.huixiangedu.cn

@property 与 @x.setter 配合
来源：http://fs.gzmigu.cn

[U30] Py：数据类
来源：http://ld.panjiajie.cn

@dataclass(slots=True)
来源：http://sb.szxytkj.cn

[U31] Py：单测
来源：http://bk.521024.cn

python -m pytest -q
来源：http://hm.gzmigu.cn

[U32] Py：代码格式化
来源：http://jl.lnxyls.cn

ruff format . && ruff check --fix .
来源：http://li.bjjhwx.cn

[U33] Py：打包发布
来源：http://uf.colortex.cn

python -m build  （依赖 pyproject.toml）
来源：http://at.gzmigu.cn

[U34] Py：判断编码
来源：http://wd.jctech888.com.cn

chardet.detect(raw)
来源：http://vd.9csxet.cn

[U35] Py：发送邮件
来源：http://yv.wgjwhj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hl.muxihuayi.cn

[U36] Py：定时任务
来源：http://yl.yuexingan06.cn

schedule.every(10).minutes.do(job)
来源：http://jj.huixiangedu.cn

[U37] Py：读写 Excel
来源：http://vk.yuexingan06.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jz.hahajie.cn

[U38] Py：获取脚本所在目录
来源：http://oh.jctech888.com.cn

Path(__file__).resolve().parent
来源：http://ef.szxytkj.cn

[U39] Py：判断是否在交互环境
来源：http://wx.521024.cn

sys.stdout.isatty()
来源：http://ip.colortex.cn

[U40] Py：打印到标准错误
来源：http://xs.gzmigu.cn

print("err", file=sys.stderr)
来源：http://jo.szxytkj.cn

[U41] PHP：初始化 Composer 项目
来源：http://km.521024.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gg.9csxet.cn

[U42] PHP：PSR-4 自动加载
来源：http://ij.wgjwhj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ap.521024.cn

[U43] PHP：声明命名空间
来源：http://dx.huanxung.cn

namespace App\Http;
来源：http://xt.wgjwhj.cn

[U44] PHP：开启严格类型
来源：http://eo.521024.cn

declare(strict_types=1);
来源：http://bk.colortex.cn

[U45] PHP：类型声明与返回类型
来源：http://zw.bjjhwx.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ln.huixiangedu.cn

[U46] PHP：可空类型
来源：http://bi.colortex.cn

?string $name = null
来源：http://tx.shtwfgs.cn

[U47] PHP：联合类型
来源：http://qw.521024.cn

int|string $id
来源：http://wk.szsharing.cn

[U48] PHP：纯枚举
来源：http://ya.gzmigu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vs.muxihuayi.cn

[U49] PHP：只读属性
来源：http://po.chemitech.net.cn

public readonly string $name
来源：http://mj.bookmarksfly.cn

[U50] PHP：构造器属性提升
来源：http://vc.9csxet.cn

public function __construct(private int $id) {}
来源：http://qz.muxihuayi.cn

[U51] PHP：数组解构
来源：http://jz.yuexingan06.cn

[$a, $b] = $arr;
来源：http://ct.wgjwhj.cn

[U52] PHP：箭头函数
来源：http://zo.bookmarksfly.cn

$double = fn($x) => $x * 2;
来源：http://xc.asd995.cn

[U53] PHP：空合并运算符
来源：http://fy.asd995.cn

$v = $a ?? $b ?? "default";
来源：http://ss.hnjuh.cn

[U54] PHP：空安全调用
来源：http://lk.lnxyls.cn

$obj?->method()
来源：http://eh.chemitech.net.cn

[U55] PHP：match 表达式
来源：http://qw.yuntaijiaju.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vr.huixiangedu.cn

[U56] PHP：命名参数
来源：http://sl.panjiajie.cn

f(a: 1, b: 2)
来源：http://pr.huixiangedu.cn

[U57] PHP：字符串插值
来源：http://eh.hahajie.cn

"值: {$a}"
来源：http://tw.huanxung.cn

[U58] PHP：数组三件套
来源：http://yd.huixinmuqiang.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fd.wgjwhj.cn

[U59] PHP：自定义排序
来源：http://zb.hnjuh.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jl.hahajie.cn

[U60] PHP：JSON 编解码
来源：http://ew.nszjky.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://sw.muxihuayi.cn

[U61] PHP：正则
来源：http://it.wgjwhj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qf.521024.cn

[U62] PHP：日期对象
来源：http://nb.shxzukj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ea.haigaiapp.cn

[U63] PHP：文件读写
来源：http://gp.gzmigu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yk.yuexingan06.cn

[U64] PHP：目录遍历
来源：http://bt.muxihuayi.cn

glob("dir/*.php");  scandir("dir");
来源：http://qq.yuexingan06.cn

[U65] PHP：会话
来源：http://vl.muxihuayi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ja.bookmarksfly.cn

[U66] PHP：设置 Cookie
来源：http://ig.jctech888.com.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://oi.hnjuh.cn

[U67] PHP：处理文件上传
来源：http://qn.gzmigu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vd.huixinmuqiang.cn

[U68] PHP：PDO 连接
来源：http://zh.asd995.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://du.muxihuayi.cn

[U69] PHP：PDO 预处理
来源：http://hb.shxzukj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rn.colortex.cn

[U70] PHP：PDO 事务
来源：http://mg.huixiangedu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rd.panjiajie.cn

[U71] PHP：抛出异常
来源：http://jh.colortex.cn

throw new RuntimeException("失败", 500);
来源：http://gd.asd995.cn

[U72] PHP：写错误日志
来源：http://de.gzmigu.cn

error_log("失败: " . $e->getMessage());
来源：http://nz.shtwfgs.cn

[U73] PHP：读取 ini 配置
来源：http://fd.szsharing.cn

parse_ini_file("config.ini", true)
来源：http://ad.9csxet.cn

[U74] PHP：读取环境变量
来源：http://cf.huixinmuqiang.cn

getenv("APP_ENV") ?: "production"
来源：http://fr.shxzukj.cn

[U75] PHP：依赖注入
来源：http://uo.lnxyls.cn

composer require psr/container
来源：http://oy.jianghongdianzi.cn

[U76] PHP：简单路由
来源：http://kb.shxzskj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ew.shtwfgs.cn

[U77] PHP：模板渲染
来源：http://gp.asd995.cn

composer require twig/twig
来源：http://mb.szsharing.cn

[U78] PHP：单元测试
来源：http://hm.shxzskj.cn

composer require --dev phpunit/phpunit
来源：http://ib.huixinmuqiang.cn

[U79] PHP：静态分析
来源：http://hd.huixiangedu.cn

composer require --dev phpstan/phpstan
来源：http://sf.lnxyls.cn

[U80] PHP：代码规范修复
来源：http://wl.bookmarksfly.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ka.wgjwhj.cn

[U81] JS：初始化项目
来源：http://ei.9csxet.cn

npm init -y;  npm i express
来源：http://ct.asd995.cn

[U82] JS：package.json 脚本
来源：http://sm.szsharing.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vn.wgjwhj.cn

[U83] JS：ES Module 导入导出
来源：http://ii.jianghongdianzi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://lo.jctech888.com.cn

[U84] JS：CommonJS 写法
来源：http://zc.wgjwhj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://vb.newstarts.cn

[U85] JS：可选链
来源：http://do.hahajie.cn

a?.b?.c
来源：http://vw.panjiajie.cn

[U86] JS：空值合并
来源：http://sw.521024.cn

a ?? b
来源：http://yo.shxzukj.cn

[U87] JS：解构默认值
来源：http://id.panjiajie.cn

const { a = 1, b = 2 } = obj;
来源：http://tp.lnxyls.cn

[U88] JS：对象展开合并
来源：http://sj.bookmarksfly.cn

{ ...a, ...b }
来源：http://lc.gzmigu.cn

[U89] JS：数组去重
来源：http://cp.asd995.cn

[...new Set(arr)]
来源：http://jq.huixinmuqiang.cn

[U90] JS：数字数组排序
来源：http://zd.nicolike.cn

[...arr].sort((a, b) => a - b)
来源：http://un.nicolike.cn

[U91] JS：对象键值遍历
来源：http://oa.szsharing.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mx.yuexingan06.cn

[U92] JS：深拷贝
来源：http://bl.9csxet.cn

structuredClone(obj)
来源：http://vh.bjjhwx.cn

[U93] JS：模板字符串
来源：http://ls.lnxyls.cn

`共 ${n} 条`
来源：http://uw.chemitech.net.cn

[U94] JS：箭头函数
来源：http://dm.huixiangedu.cn

const double = x => x * 2;
来源：http://aq.bookmarksfly.cn

[U95] JS：Promise 包装
来源：http://nz.huanxung.cn

new Promise((resolve, reject) => {})
来源：http://sq.yuntaijiaju.cn

[U96] JS：async/await 与异常
来源：http://nx.colortex.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mf.panjiajie.cn

[U97] JS：并发请求
来源：http://bt.szxytkj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://om.huixiangedu.cn

[U98] JS：fetch 带 JSON
来源：http://nt.shtwfgs.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kf.huixinmuqiang.cn

[U99] JS：事件监听
来源：http://pk.hnjuh.cn

el.addEventListener("click", e => {})
来源：http://cr.newstarts.cn

[U100] JS：DOM 查询
来源：http://je.jctech888.com.cn

document.querySelector(".item")
来源：http://zv.9csxet.cn

[U101] JS：classList 操作
来源：http://hs.panjiajie.cn

el.classList.toggle("active")
来源：http://xc.bjjhwx.cn

[U102] JS：本地存储
来源：http://yf.huanxung.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://dk.gzmigu.cn

[U103] JS：定时器
来源：http://xr.shtwfgs.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://oc.bjjhwx.cn

[U104] JS：防抖
来源：http://lg.bjjhwx.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vx.newstarts.cn

[U105] JS：节流
来源：http://eq.colortex.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dh.huixinmuqiang.cn

[U106] JS：日期格式化
来源：http://lc.hahajie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://si.huixinmuqiang.cn

[U107] JS：数字千分位
来源：http://ns.asd995.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yl.gzmigu.cn

[U108] JS：随机整数
来源：http://zl.shtwfgs.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ag.bjjhwx.cn

[U109] JS：数组分组
来源：http://lm.9csxet.cn

Object.groupBy(arr, x => x.type)
来源：http://ke.gzmigu.cn

[U110] JS：数组分块
来源：http://zh.newstarts.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jg.shxzskj.cn

[U111] JS：对象转 Map
来源：http://ln.hnjuh.cn

new Map(Object.entries(obj))
来源：http://ch.lnxyls.cn

[U112] JS：字符串补位
来源：http://mq.colortex.cn

"7".padStart(3, "0")
来源：http://pl.shxzskj.cn

[U113] JS：正则替换全部
来源：http://lc.huanxung.cn

s.replaceAll("a", "b")
来源：http://sl.9csxet.cn

[U114] JS：JSON 深比较
来源：http://ts.lnxyls.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://at.muxihuayi.cn


<!-- 参考信息 -->