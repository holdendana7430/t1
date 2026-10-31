代发 wailian999

[T33] Lua：表（数组）
来源：http://ii.bookmarksfly.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ap.nszjky.cn

[T34] Lua：遍历表
来源：http://st.chemitech.net.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vr.yuntaijiaju.cn

[T35] Lua：字典表
来源：http://xl.chemitech.net.cn

local d = { a = 1 };  d.b = 2
来源：http://ao.huixinmuqiang.cn

[T36] Lua：函数
来源：http://df.shtwfgs.cn

function add(a, b) return a + b end
来源：http://ok.huixiangedu.cn

[T37] Lua：字符串拼接
来源：http://hv.shxzskj.cn

"a" .. "b"
来源：http://om.jctech888.com.cn

[T38] Lua：条件
来源：http://yr.9csxet.cn

if x > 0 then print("正") end
来源：http://ab.huanxung.cn

[T39] Lua：模式匹配
来源：http://cb.gzmigu.cn

string.find(s, "%d+")
来源：http://uk.nszjky.cn

[T40] Lua：元表
来源：http://qa.9csxet.cn

setmetatable({}, { __index = base })
来源：http://pj.yuntaijiaju.cn

[T41] Perl：Hello World
来源：http://pj.shxzukj.cn

print "Hello\n";
来源：http://hi.muxihuayi.cn

[T42] Perl：变量类型
来源：http://uo.yuexingan06.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://na.jianghongdianzi.cn

[T43] Perl：字符串插值
来源：http://jx.chemitech.net.cn

"值: $a"
来源：http://my.szsharing.cn

[T44] Perl：条件
来源：http://lg.hahajie.cn

if ($a > 0) { print "正"; }
来源：http://um.bookmarksfly.cn

[T45] Perl：数组遍历
来源：http://bl.szxytkj.cn

for my $x (@arr) { print $x; }
来源：http://mj.asd995.cn

[T46] Perl：哈希操作
来源：http://pg.asd995.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tz.wgjwhj.cn

[T47] Perl：正则捕获
来源：http://gm.newstarts.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://sk.gzmigu.cn

[T48] Perl：正则替换
来源：http://fe.colortex.cn

$s =~ s/old/new/g;
来源：http://sn.nicolike.cn

[T49] Perl：函数
来源：http://xh.panjiajie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ev.asd995.cn

[T50] Perl：逐行读文件
来源：http://li.9csxet.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://dw.panjiajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://wx.haigaiapp.cn

[T51] Scala：Hello World
来源：http://fr.yuntaijiaju.cn

println("Hello")
来源：http://nm.gzmigu.cn

[T52] Scala：变量
来源：http://un.hnjuh.cn

val a = 1;  var b = 2
来源：http://ht.shtwfgs.cn

[T53] Scala：字符串插值
来源：http://hp.szsharing.cn

s"值: $b"
来源：http://wv.shtwfgs.cn

[T54] Scala：集合映射
来源：http://so.szxytkj.cn

List(1, 2, 3).map(_ * 2)
来源：http://io.bookmarksfly.cn

[T55] Scala：集合过滤
来源：http://nn.9csxet.cn

List(1, 2, 3).filter(_ > 1)
来源：http://oh.yuexingan06.cn

[T56] Scala：样例类
来源：http://bo.yuntaijiaju.cn

case class User(name: String, age: Int)
来源：http://xy.huanxung.cn

[T57] Scala：模式匹配
来源：http://op.shxzukj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ne.colortex.cn

[T58] Scala：函数定义
来源：http://kb.huanxung.cn

def add(a: Int, b: Int): Int = a + b
来源：http://me.huixinmuqiang.cn

[T59] Scala：循环
来源：http://yx.9csxet.cn

for (i <- 1 to 10) println(i)
来源：http://vi.newstarts.cn

[T60] Scala：折叠
来源：http://wp.newstarts.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vu.bookmarksfly.cn

================================================================================
来源：http://qm.jctech888.com.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bm.jctech888.com.cn

================================================================================
来源：http://dj.newstarts.cn

[U01] Py：创建虚拟环境
来源：http://od.bjjhwx.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cl.shxzskj.cn

[U02] Py：导出 / 安装依赖
来源：http://is.shxzskj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ey.jianghongdianzi.cn

[U03] Py：加载 .env 配置
来源：http://gv.lnxyls.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://vh.bookmarksfly.cn

[U04] Py：变量调试打印
来源：http://yo.jianghongdianzi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xp.panjiajie.cn

[U05] Py：列表去重且保序
来源：http://ba.lnxyls.cn

list(dict.fromkeys(arr))
来源：http://cg.szsharing.cn

[U06] Py：合并两个字典
来源：http://oc.panjiajie.cn

{**a, **b}
来源：http://on.nicolike.cn

[U07] Py：反转字典键值
来源：http://zi.szxytkj.cn

{v: k for k, v in d.items()}
来源：http://oe.bjjhwx.cn

[U08] Py：展平二维列表
来源：http://pj.shxzskj.cn

[y for x in nested for y in x]
来源：http://vr.wgjwhj.cn

[U09] Py：字典取最大值的键
来源：http://we.wgjwhj.cn

max(d, key=d.get)
来源：http://eh.haigaiapp.cn

[U10] Py：按值排序字典
来源：http://nq.shxzukj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bn.panjiajie.cn

[U11] Py：生成器表达式
来源：http://du.bookmarksfly.cn

(x * 2 for x in arr)
来源：http://ia.nszjky.cn

[U12] Py：取出现最多的 3 个元素
来源：http://vv.huanxung.cn

Counter(arr).most_common(3)
来源：http://xe.lnxyls.cn

[U13] Py：固定长度队列
来源：http://ef.nicolike.cn

deque(maxlen=10)
来源：http://hh.hnjuh.cn

[U14] Py：分组收集到列表
来源：http://pa.jianghongdianzi.cn

defaultdict(list)
来源：http://wz.nicolike.cn

[U15] Py：高精度计时
来源：http://gc.hnjuh.cn

t = time.perf_counter()
来源：http://wu.shxzskj.cn

[U16] Py：命令行参数解析
来源：http://zy.lnxyls.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://io.newstarts.cn

[U17] Py：初始化日志
来源：http://gs.chemitech.net.cn

logging.basicConfig(level=logging.INFO)
来源：http://my.chemitech.net.cn

[U18] Py：预编译正则
来源：http://ia.lnxyls.cn

pat = re.compile(r"\d+")
来源：http://vd.gzmigu.cn

[U19] Py：正则替换带回调
来源：http://pp.bookmarksfly.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://uj.colortex.cn

[U20] Py：缓存函数结果
来源：http://ou.bookmarksfly.cn

@functools.lru_cache(maxsize=None)
来源：http://rb.bjjhwx.cn

[U21] Py：自定义上下文管理器
来源：http://wq.shtwfgs.cn

@contextlib.contextmanager
来源：http://lj.huanxung.cn

[U22] Py：矩阵转置
来源：http://yc.jctech888.com.cn

list(zip(*m))
来源：http://ti.yuntaijiaju.cn

[U23] Py：分块读取大文件
来源：http://tm.muxihuayi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sm.lnxyls.cn

[U24] Py：路径操作
来源：http://rx.panjiajie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ua.hahajie.cn

[U25] Py：CSV 按字典读
来源：http://vc.gzmigu.cn

csv.DictReader(f)
来源：http://ic.yuntaijiaju.cn

[U26] Py：并发下载
来源：http://md.nicolike.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ac.chemitech.net.cn

[U27] Py：异步 HTTP
来源：http://sb.lnxyls.cn

aiohttp.ClientSession() 配合 async with
来源：http://io.asd995.cn

[U28] Py：类型别名
来源：http://gy.szsharing.cn

UserId = int
来源：http://cp.hnjuh.cn

[U29] Py：属性校验
来源：http://wp.bjjhwx.cn

@property 与 @x.setter 配合
来源：http://ey.hahajie.cn

[U30] Py：数据类
来源：http://ah.shxzukj.cn

@dataclass(slots=True)
来源：http://ry.newstarts.cn

[U31] Py：单测
来源：http://jw.gzmigu.cn

python -m pytest -q
来源：http://tv.haigaiapp.cn

[U32] Py：代码格式化
来源：http://dv.hahajie.cn

ruff format . && ruff check --fix .
来源：http://xn.wgjwhj.cn

[U33] Py：打包发布
来源：http://mf.shtwfgs.cn

python -m build  （依赖 pyproject.toml）
来源：http://js.haigaiapp.cn

[U34] Py：判断编码
来源：http://lk.lnxyls.cn

chardet.detect(raw)
来源：http://uj.hahajie.cn

[U35] Py：发送邮件
来源：http://xl.chemitech.net.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lg.nicolike.cn

[U36] Py：定时任务
来源：http://ja.9csxet.cn

schedule.every(10).minutes.do(job)
来源：http://tv.huixinmuqiang.cn

[U37] Py：读写 Excel
来源：http://qj.newstarts.cn

pandas.read_excel / DataFrame.to_excel
来源：http://cd.jianghongdianzi.cn

[U38] Py：获取脚本所在目录
来源：http://uo.jianghongdianzi.cn

Path(__file__).resolve().parent
来源：http://st.bookmarksfly.cn

[U39] Py：判断是否在交互环境
来源：http://tj.panjiajie.cn

sys.stdout.isatty()
来源：http://iw.huanxung.cn

[U40] Py：打印到标准错误
来源：http://om.muxihuayi.cn

print("err", file=sys.stderr)
来源：http://in.9csxet.cn

[U41] PHP：初始化 Composer 项目
来源：http://cq.yuexingan06.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zp.521024.cn

[U42] PHP：PSR-4 自动加载
来源：http://ck.yuexingan06.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wj.shxzukj.cn

[U43] PHP：声明命名空间
来源：http://wo.nicolike.cn

namespace App\Http;
来源：http://ri.nszjky.cn

[U44] PHP：开启严格类型
来源：http://oi.521024.cn

declare(strict_types=1);
来源：http://qw.haigaiapp.cn

[U45] PHP：类型声明与返回类型
来源：http://xx.nicolike.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://uv.bookmarksfly.cn

[U46] PHP：可空类型
来源：http://lj.shxzukj.cn

?string $name = null
来源：http://cn.szsharing.cn

[U47] PHP：联合类型
来源：http://sr.yuexingan06.cn

int|string $id
来源：http://fm.yuntaijiaju.cn

[U48] PHP：纯枚举
来源：http://xx.yuexingan06.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vu.chemitech.net.cn

[U49] PHP：只读属性
来源：http://yt.jianghongdianzi.cn

public readonly string $name
来源：http://gx.szsharing.cn

[U50] PHP：构造器属性提升
来源：http://gz.asd995.cn

public function __construct(private int $id) {}
来源：http://to.hnjuh.cn

[U51] PHP：数组解构
来源：http://cz.muxihuayi.cn

[$a, $b] = $arr;
来源：http://hr.wgjwhj.cn

[U52] PHP：箭头函数
来源：http://vs.bookmarksfly.cn

$double = fn($x) => $x * 2;
来源：http://oy.shxzukj.cn

[U53] PHP：空合并运算符
来源：http://uy.muxihuayi.cn

$v = $a ?? $b ?? "default";
来源：http://ts.nszjky.cn

[U54] PHP：空安全调用
来源：http://he.yuntaijiaju.cn

$obj?->method()
来源：http://ev.haigaiapp.cn

[U55] PHP：match 表达式
来源：http://xw.lnxyls.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hk.wgjwhj.cn

[U56] PHP：命名参数
来源：http://xx.gzmigu.cn

f(a: 1, b: 2)
来源：http://su.asd995.cn

[U57] PHP：字符串插值
来源：http://yt.hnjuh.cn

"值: {$a}"
来源：http://qv.asd995.cn

[U58] PHP：数组三件套
来源：http://qh.huanxung.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ew.yuntaijiaju.cn

[U59] PHP：自定义排序
来源：http://hl.newstarts.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lg.shtwfgs.cn

[U60] PHP：JSON 编解码
来源：http://ax.nicolike.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qn.asd995.cn

[U61] PHP：正则
来源：http://jo.bookmarksfly.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wc.panjiajie.cn

[U62] PHP：日期对象
来源：http://fj.nszjky.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sq.lnxyls.cn

[U63] PHP：文件读写
来源：http://jn.chemitech.net.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rl.huixinmuqiang.cn

[U64] PHP：目录遍历
来源：http://io.asd995.cn

glob("dir/*.php");  scandir("dir");
来源：http://ho.szsharing.cn

[U65] PHP：会话
来源：http://dl.huixinmuqiang.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://tx.wgjwhj.cn

[U66] PHP：设置 Cookie
来源：http://jk.asd995.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://oo.jianghongdianzi.cn

[U67] PHP：处理文件上传
来源：http://hm.yuexingan06.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ea.huixinmuqiang.cn

[U68] PHP：PDO 连接
来源：http://mf.szxytkj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jo.chemitech.net.cn

[U69] PHP：PDO 预处理
来源：http://pn.szsharing.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vd.huixinmuqiang.cn

[U70] PHP：PDO 事务
来源：http://td.szxytkj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ff.colortex.cn

[U71] PHP：抛出异常
来源：http://iw.jianghongdianzi.cn

throw new RuntimeException("失败", 500);
来源：http://wa.gzmigu.cn

[U72] PHP：写错误日志
来源：http://xc.nicolike.cn

error_log("失败: " . $e->getMessage());
来源：http://we.shxzskj.cn

[U73] PHP：读取 ini 配置
来源：http://tj.jctech888.com.cn

parse_ini_file("config.ini", true)
来源：http://rv.bjjhwx.cn

[U74] PHP：读取环境变量
来源：http://gu.jctech888.com.cn

getenv("APP_ENV") ?: "production"
来源：http://hu.szxytkj.cn

[U75] PHP：依赖注入
来源：http://go.shtwfgs.cn

composer require psr/container
来源：http://av.hahajie.cn

[U76] PHP：简单路由
来源：http://ws.huixinmuqiang.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mc.nicolike.cn

[U77] PHP：模板渲染
来源：http://fc.huanxung.cn

composer require twig/twig
来源：http://dq.szsharing.cn

[U78] PHP：单元测试
来源：http://ab.9csxet.cn

composer require --dev phpunit/phpunit
来源：http://hv.colortex.cn

[U79] PHP：静态分析
来源：http://un.panjiajie.cn

composer require --dev phpstan/phpstan
来源：http://cp.shxzskj.cn

[U80] PHP：代码规范修复
来源：http://yi.chemitech.net.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://wc.panjiajie.cn

[U81] JS：初始化项目
来源：http://cz.huixinmuqiang.cn

npm init -y;  npm i express
来源：http://mr.521024.cn

[U82] JS：package.json 脚本
来源：http://km.yuexingan06.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pg.huixiangedu.cn

[U83] JS：ES Module 导入导出
来源：http://hd.gzmigu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ql.gzmigu.cn

[U84] JS：CommonJS 写法
来源：http://fv.szxytkj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://rr.hahajie.cn

[U85] JS：可选链
来源：http://hv.huixinmuqiang.cn

a?.b?.c
来源：http://re.chemitech.net.cn

[U86] JS：空值合并
来源：http://tu.chemitech.net.cn

a ?? b
来源：http://ms.shxzskj.cn

[U87] JS：解构默认值
来源：http://hb.huixiangedu.cn

const { a = 1, b = 2 } = obj;
来源：http://na.yuexingan06.cn

[U88] JS：对象展开合并
来源：http://wr.haigaiapp.cn

{ ...a, ...b }
来源：http://fu.huixinmuqiang.cn

[U89] JS：数组去重
来源：http://cd.nicolike.cn

[...new Set(arr)]
来源：http://nx.hnjuh.cn

[U90] JS：数字数组排序
来源：http://ds.newstarts.cn

[...arr].sort((a, b) => a - b)
来源：http://xa.asd995.cn

[U91] JS：对象键值遍历
来源：http://kj.colortex.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fh.hahajie.cn

[U92] JS：深拷贝
来源：http://lo.nszjky.cn

structuredClone(obj)
来源：http://ho.bjjhwx.cn

[U93] JS：模板字符串
来源：http://gf.lnxyls.cn

`共 ${n} 条`
来源：http://hy.nicolike.cn

[U94] JS：箭头函数
来源：http://lk.jianghongdianzi.cn

const double = x => x * 2;
来源：http://fa.hnjuh.cn

[U95] JS：Promise 包装
来源：http://mu.panjiajie.cn

new Promise((resolve, reject) => {})
来源：http://vg.shxzskj.cn

[U96] JS：async/await 与异常
来源：http://lf.panjiajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hk.lnxyls.cn

[U97] JS：并发请求
来源：http://cq.jianghongdianzi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ng.haigaiapp.cn

[U98] JS：fetch 带 JSON
来源：http://wc.bookmarksfly.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gr.shtwfgs.cn

[U99] JS：事件监听
来源：http://kh.chemitech.net.cn

el.addEventListener("click", e => {})
来源：http://gr.jianghongdianzi.cn

[U100] JS：DOM 查询
来源：http://lu.colortex.cn

document.querySelector(".item")
来源：http://xs.wgjwhj.cn

[U101] JS：classList 操作
来源：http://kb.521024.cn

el.classList.toggle("active")
来源：http://nz.nicolike.cn

[U102] JS：本地存储
来源：http://nq.shtwfgs.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://da.szsharing.cn

[U103] JS：定时器
来源：http://pi.shxzskj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zn.bookmarksfly.cn

[U104] JS：防抖
来源：http://ud.521024.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xv.nicolike.cn

[U105] JS：节流
来源：http://gj.521024.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ry.bjjhwx.cn

[U106] JS：日期格式化
来源：http://ga.huanxung.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://io.nicolike.cn

[U107] JS：数字千分位
来源：http://gs.panjiajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hw.haigaiapp.cn

[U108] JS：随机整数
来源：http://hw.haigaiapp.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wd.521024.cn

[U109] JS：数组分组
来源：http://bv.hnjuh.cn

Object.groupBy(arr, x => x.type)
来源：http://ja.chemitech.net.cn

[U110] JS：数组分块
来源：http://wn.wgjwhj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dy.nicolike.cn

[U111] JS：对象转 Map
来源：http://qn.yuexingan06.cn

new Map(Object.entries(obj))
来源：http://qk.huixinmuqiang.cn

[U112] JS：字符串补位
来源：http://jv.521024.cn

"7".padStart(3, "0")
来源：http://sm.shtwfgs.cn

[U113] JS：正则替换全部
来源：http://uk.gzmigu.cn

s.replaceAll("a", "b")
来源：http://wm.bookmarksfly.cn

[U114] JS：JSON 深比较
来源：http://nt.shxzukj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hn.huixinmuqiang.cn

[U115] JS：生成 UUID
来源：http://re.nicolike.cn

crypto.randomUUID()
来源：http://uf.bjjhwx.cn

[U116] JS：类型检查（JSDoc）
来源：http://xp.huixinmuqiang.cn

/** @param {string} name */ function f(name) {}
来源：http://ll.huanxung.cn

[U117] JS：单元测试
来源：http://qo.lnxyls.cn

npm i -D vitest;  npx vitest
来源：http://vp.muxihuayi.cn

[U118] JS：开发服务器
来源：http://em.lnxyls.cn

npm i -D vite;  npx vite
来源：http://io.yuntaijiaju.cn

[U119] JS：生产构建
来源：http://po.bookmarksfly.cn

npx vite build
来源：http://tw.haigaiapp.cn

[U120] JS：读取环境变量（Vite）
来源：http://il.haigaiapp.cn

import.meta.env.VITE_API_URL
来源：http://jo.szsharing.cn


<!-- 参考信息 -->