代发 wailian999

[T31] Lua：Hello World
来源：http://qj.panjiajie.cn

print("Hello")
来源：http://wj.hnjuh.cn

[T32] Lua：局部变量
来源：http://ui.jctech888.com.cn

local a = 1
来源：http://yl.panjiajie.cn

[T33] Lua：表（数组）
来源：http://bz.huixiangedu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://yk.huanxung.cn

[T34] Lua：遍历表
来源：http://tr.bookmarksfly.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://tm.colortex.cn

[T35] Lua：字典表
来源：http://hn.bjjhwx.cn

local d = { a = 1 };  d.b = 2
来源：http://wo.bookmarksfly.cn

[T36] Lua：函数
来源：http://nb.chemitech.net.cn

function add(a, b) return a + b end
来源：http://xb.panjiajie.cn

[T37] Lua：字符串拼接
来源：http://yq.nszjky.cn

"a" .. "b"
来源：http://zf.newstarts.cn

[T38] Lua：条件
来源：http://vu.asd995.cn

if x > 0 then print("正") end
来源：http://un.huanxung.cn

[T39] Lua：模式匹配
来源：http://su.huixiangedu.cn

string.find(s, "%d+")
来源：http://xq.hahajie.cn

[T40] Lua：元表
来源：http://dr.9csxet.cn

setmetatable({}, { __index = base })
来源：http://rs.panjiajie.cn

[T41] Perl：Hello World
来源：http://vk.nszjky.cn

print "Hello\n";
来源：http://ac.haigaiapp.cn

[T42] Perl：变量类型
来源：http://ne.gzmigu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lu.chemitech.net.cn

[T43] Perl：字符串插值
来源：http://rz.szsharing.cn

"值: $a"
来源：http://rx.hahajie.cn

[T44] Perl：条件
来源：http://bl.huixiangedu.cn

if ($a > 0) { print "正"; }
来源：http://kj.nicolike.cn

[T45] Perl：数组遍历
来源：http://df.jctech888.com.cn

for my $x (@arr) { print $x; }
来源：http://rv.shxzukj.cn

[T46] Perl：哈希操作
来源：http://ky.haigaiapp.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qv.lnxyls.cn

[T47] Perl：正则捕获
来源：http://jm.chemitech.net.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://tz.hahajie.cn

[T48] Perl：正则替换
来源：http://ko.shtwfgs.cn

$s =~ s/old/new/g;
来源：http://yp.hahajie.cn

[T49] Perl：函数
来源：http://mq.bjjhwx.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sy.yuexingan06.cn

[T50] Perl：逐行读文件
来源：http://zn.huanxung.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://yf.shtwfgs.cn

while (my $line = <$fh>) { print $line; }
来源：http://or.yuntaijiaju.cn

[T51] Scala：Hello World
来源：http://cf.haigaiapp.cn

println("Hello")
来源：http://eb.nszjky.cn

[T52] Scala：变量
来源：http://vy.521024.cn

val a = 1;  var b = 2
来源：http://zf.muxihuayi.cn

[T53] Scala：字符串插值
来源：http://pk.bjjhwx.cn

s"值: $b"
来源：http://eu.szsharing.cn

[T54] Scala：集合映射
来源：http://uj.521024.cn

List(1, 2, 3).map(_ * 2)
来源：http://gm.huixinmuqiang.cn

[T55] Scala：集合过滤
来源：http://rx.huixiangedu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://mn.bjjhwx.cn

[T56] Scala：样例类
来源：http://uq.jctech888.com.cn

case class User(name: String, age: Int)
来源：http://th.gzmigu.cn

[T57] Scala：模式匹配
来源：http://vk.nicolike.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://sw.szsharing.cn

[T58] Scala：函数定义
来源：http://it.yuntaijiaju.cn

def add(a: Int, b: Int): Int = a + b
来源：http://jx.nicolike.cn

[T59] Scala：循环
来源：http://tf.jianghongdianzi.cn

for (i <- 1 to 10) println(i)
来源：http://kq.huixinmuqiang.cn

[T60] Scala：折叠
来源：http://sm.szsharing.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ub.huanxung.cn

================================================================================
来源：http://ql.hahajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://td.huixiangedu.cn

================================================================================
来源：http://bi.huanxung.cn

[U01] Py：创建虚拟环境
来源：http://xn.shxzskj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://pm.shxzukj.cn

[U02] Py：导出 / 安装依赖
来源：http://dr.szxytkj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ro.colortex.cn

[U03] Py：加载 .env 配置
来源：http://pj.huanxung.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://nn.yuntaijiaju.cn

[U04] Py：变量调试打印
来源：http://fz.colortex.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ki.chemitech.net.cn

[U05] Py：列表去重且保序
来源：http://aa.9csxet.cn

list(dict.fromkeys(arr))
来源：http://tp.newstarts.cn

[U06] Py：合并两个字典
来源：http://ib.521024.cn

{**a, **b}
来源：http://ez.szxytkj.cn

[U07] Py：反转字典键值
来源：http://tk.newstarts.cn

{v: k for k, v in d.items()}
来源：http://fl.bookmarksfly.cn

[U08] Py：展平二维列表
来源：http://mf.huixinmuqiang.cn

[y for x in nested for y in x]
来源：http://jx.asd995.cn

[U09] Py：字典取最大值的键
来源：http://ud.gzmigu.cn

max(d, key=d.get)
来源：http://jt.haigaiapp.cn

[U10] Py：按值排序字典
来源：http://xn.panjiajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dj.shxzukj.cn

[U11] Py：生成器表达式
来源：http://qm.panjiajie.cn

(x * 2 for x in arr)
来源：http://kn.huixinmuqiang.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rr.hnjuh.cn

Counter(arr).most_common(3)
来源：http://sd.bookmarksfly.cn

[U13] Py：固定长度队列
来源：http://ev.chemitech.net.cn

deque(maxlen=10)
来源：http://zq.jctech888.com.cn

[U14] Py：分组收集到列表
来源：http://xu.yuexingan06.cn

defaultdict(list)
来源：http://nn.hnjuh.cn

[U15] Py：高精度计时
来源：http://zf.newstarts.cn

t = time.perf_counter()
来源：http://rf.newstarts.cn

[U16] Py：命令行参数解析
来源：http://hw.szsharing.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sj.muxihuayi.cn

[U17] Py：初始化日志
来源：http://cn.bjjhwx.cn

logging.basicConfig(level=logging.INFO)
来源：http://uz.wgjwhj.cn

[U18] Py：预编译正则
来源：http://ii.shxzskj.cn

pat = re.compile(r"\d+")
来源：http://xe.521024.cn

[U19] Py：正则替换带回调
来源：http://wf.wgjwhj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ks.nicolike.cn

[U20] Py：缓存函数结果
来源：http://qv.szsharing.cn

@functools.lru_cache(maxsize=None)
来源：http://dm.yuexingan06.cn

[U21] Py：自定义上下文管理器
来源：http://dp.521024.cn

@contextlib.contextmanager
来源：http://eb.muxihuayi.cn

[U22] Py：矩阵转置
来源：http://ru.panjiajie.cn

list(zip(*m))
来源：http://ya.szxytkj.cn

[U23] Py：分块读取大文件
来源：http://ud.9csxet.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pd.muxihuayi.cn

[U24] Py：路径操作
来源：http://lb.chemitech.net.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dh.nicolike.cn

[U25] Py：CSV 按字典读
来源：http://qh.shtwfgs.cn

csv.DictReader(f)
来源：http://in.asd995.cn

[U26] Py：并发下载
来源：http://ou.huanxung.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ho.muxihuayi.cn

[U27] Py：异步 HTTP
来源：http://cd.jctech888.com.cn

aiohttp.ClientSession() 配合 async with
来源：http://hc.colortex.cn

[U28] Py：类型别名
来源：http://do.shtwfgs.cn

UserId = int
来源：http://sp.hnjuh.cn

[U29] Py：属性校验
来源：http://qt.szsharing.cn

@property 与 @x.setter 配合
来源：http://ho.shxzukj.cn

[U30] Py：数据类
来源：http://ju.gzmigu.cn

@dataclass(slots=True)
来源：http://qp.newstarts.cn

[U31] Py：单测
来源：http://bv.nszjky.cn

python -m pytest -q
来源：http://sj.gzmigu.cn

[U32] Py：代码格式化
来源：http://gf.wgjwhj.cn

ruff format . && ruff check --fix .
来源：http://ds.bjjhwx.cn

[U33] Py：打包发布
来源：http://ld.bjjhwx.cn

python -m build  （依赖 pyproject.toml）
来源：http://ov.lnxyls.cn

[U34] Py：判断编码
来源：http://ac.newstarts.cn

chardet.detect(raw)
来源：http://pv.nicolike.cn

[U35] Py：发送邮件
来源：http://ns.hahajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ci.shtwfgs.cn

[U36] Py：定时任务
来源：http://yt.wgjwhj.cn

schedule.every(10).minutes.do(job)
来源：http://qn.9csxet.cn

[U37] Py：读写 Excel
来源：http://xk.haigaiapp.cn

pandas.read_excel / DataFrame.to_excel
来源：http://we.wgjwhj.cn

[U38] Py：获取脚本所在目录
来源：http://su.nszjky.cn

Path(__file__).resolve().parent
来源：http://lu.9csxet.cn

[U39] Py：判断是否在交互环境
来源：http://fz.shxzskj.cn

sys.stdout.isatty()
来源：http://wd.bjjhwx.cn

[U40] Py：打印到标准错误
来源：http://qw.jctech888.com.cn

print("err", file=sys.stderr)
来源：http://bv.huixinmuqiang.cn

[U41] PHP：初始化 Composer 项目
来源：http://az.bjjhwx.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://cq.yuntaijiaju.cn

[U42] PHP：PSR-4 自动加载
来源：http://yb.nszjky.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wk.chemitech.net.cn

[U43] PHP：声明命名空间
来源：http://da.muxihuayi.cn

namespace App\Http;
来源：http://mj.huanxung.cn

[U44] PHP：开启严格类型
来源：http://mz.nszjky.cn

declare(strict_types=1);
来源：http://bt.panjiajie.cn

[U45] PHP：类型声明与返回类型
来源：http://lh.9csxet.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://nr.colortex.cn

[U46] PHP：可空类型
来源：http://gu.yuexingan06.cn

?string $name = null
来源：http://nd.yuexingan06.cn

[U47] PHP：联合类型
来源：http://wq.panjiajie.cn

int|string $id
来源：http://pi.haigaiapp.cn

[U48] PHP：纯枚举
来源：http://bh.hahajie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ea.gzmigu.cn

[U49] PHP：只读属性
来源：http://ud.shtwfgs.cn

public readonly string $name
来源：http://rg.asd995.cn

[U50] PHP：构造器属性提升
来源：http://wo.hahajie.cn

public function __construct(private int $id) {}
来源：http://vr.szsharing.cn

[U51] PHP：数组解构
来源：http://im.bjjhwx.cn

[$a, $b] = $arr;
来源：http://uj.colortex.cn

[U52] PHP：箭头函数
来源：http://qj.muxihuayi.cn

$double = fn($x) => $x * 2;
来源：http://vm.chemitech.net.cn

[U53] PHP：空合并运算符
来源：http://ba.hahajie.cn

$v = $a ?? $b ?? "default";
来源：http://py.lnxyls.cn

[U54] PHP：空安全调用
来源：http://kx.asd995.cn

$obj?->method()
来源：http://cx.huixinmuqiang.cn

[U55] PHP：match 表达式
来源：http://lm.hahajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jo.gzmigu.cn

[U56] PHP：命名参数
来源：http://ah.bookmarksfly.cn

f(a: 1, b: 2)
来源：http://ly.bookmarksfly.cn

[U57] PHP：字符串插值
来源：http://vz.haigaiapp.cn

"值: {$a}"
来源：http://yr.nicolike.cn

[U58] PHP：数组三件套
来源：http://re.jianghongdianzi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kv.nicolike.cn

[U59] PHP：自定义排序
来源：http://nb.muxihuayi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nj.asd995.cn

[U60] PHP：JSON 编解码
来源：http://ud.newstarts.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xt.hahajie.cn

[U61] PHP：正则
来源：http://xj.nicolike.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rx.jianghongdianzi.cn

[U62] PHP：日期对象
来源：http://tn.shtwfgs.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bb.bookmarksfly.cn

[U63] PHP：文件读写
来源：http://yz.nicolike.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bt.lnxyls.cn

[U64] PHP：目录遍历
来源：http://ot.panjiajie.cn

glob("dir/*.php");  scandir("dir");
来源：http://qm.shtwfgs.cn

[U65] PHP：会话
来源：http://aj.szxytkj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kx.szxytkj.cn

[U66] PHP：设置 Cookie
来源：http://zh.panjiajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wv.newstarts.cn

[U67] PHP：处理文件上传
来源：http://va.jctech888.com.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hy.hahajie.cn

[U68] PHP：PDO 连接
来源：http://oq.szsharing.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cj.asd995.cn

[U69] PHP：PDO 预处理
来源：http://zh.asd995.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sc.huixiangedu.cn

[U70] PHP：PDO 事务
来源：http://oj.muxihuayi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rg.muxihuayi.cn

[U71] PHP：抛出异常
来源：http://nb.szxytkj.cn

throw new RuntimeException("失败", 500);
来源：http://fy.huixinmuqiang.cn

[U72] PHP：写错误日志
来源：http://cv.lnxyls.cn

error_log("失败: " . $e->getMessage());
来源：http://dg.bjjhwx.cn

[U73] PHP：读取 ini 配置
来源：http://dj.szsharing.cn

parse_ini_file("config.ini", true)
来源：http://bb.jctech888.com.cn

[U74] PHP：读取环境变量
来源：http://il.gzmigu.cn

getenv("APP_ENV") ?: "production"
来源：http://ul.asd995.cn

[U75] PHP：依赖注入
来源：http://gq.wgjwhj.cn

composer require psr/container
来源：http://fn.hahajie.cn

[U76] PHP：简单路由
来源：http://hu.huixinmuqiang.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ps.shtwfgs.cn

[U77] PHP：模板渲染
来源：http://ls.muxihuayi.cn

composer require twig/twig
来源：http://kx.szsharing.cn

[U78] PHP：单元测试
来源：http://ss.nszjky.cn

composer require --dev phpunit/phpunit
来源：http://ek.chemitech.net.cn

[U79] PHP：静态分析
来源：http://et.shtwfgs.cn

composer require --dev phpstan/phpstan
来源：http://nn.chemitech.net.cn

[U80] PHP：代码规范修复
来源：http://qi.521024.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://oi.yuexingan06.cn

[U81] JS：初始化项目
来源：http://pp.newstarts.cn

npm init -y;  npm i express
来源：http://se.bjjhwx.cn

[U82] JS：package.json 脚本
来源：http://ai.yuntaijiaju.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gq.szsharing.cn

[U83] JS：ES Module 导入导出
来源：http://zk.colortex.cn

export const a = 1;  import { a } from "./m.js";
来源：http://hm.colortex.cn

[U84] JS：CommonJS 写法
来源：http://wy.521024.cn

module.exports = { a };  const { a } = require("./m");
来源：http://cw.haigaiapp.cn

[U85] JS：可选链
来源：http://ou.huanxung.cn

a?.b?.c
来源：http://ud.yuntaijiaju.cn

[U86] JS：空值合并
来源：http://td.nszjky.cn

a ?? b
来源：http://xo.chemitech.net.cn

[U87] JS：解构默认值
来源：http://py.shxzukj.cn

const { a = 1, b = 2 } = obj;
来源：http://rx.jianghongdianzi.cn

[U88] JS：对象展开合并
来源：http://vv.yuntaijiaju.cn

{ ...a, ...b }
来源：http://et.colortex.cn

[U89] JS：数组去重
来源：http://ko.yuntaijiaju.cn

[...new Set(arr)]
来源：http://mo.hnjuh.cn

[U90] JS：数字数组排序
来源：http://mi.wgjwhj.cn

[...arr].sort((a, b) => a - b)
来源：http://wd.lnxyls.cn

[U91] JS：对象键值遍历
来源：http://gc.szxytkj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xy.hahajie.cn

[U92] JS：深拷贝
来源：http://fi.panjiajie.cn

structuredClone(obj)
来源：http://ip.muxihuayi.cn

[U93] JS：模板字符串
来源：http://nu.asd995.cn

`共 ${n} 条`
来源：http://ik.muxihuayi.cn

[U94] JS：箭头函数
来源：http://ki.nicolike.cn

const double = x => x * 2;
来源：http://yf.9csxet.cn

[U95] JS：Promise 包装
来源：http://bb.chemitech.net.cn

new Promise((resolve, reject) => {})
来源：http://dd.chemitech.net.cn

[U96] JS：async/await 与异常
来源：http://bs.nicolike.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://eg.hahajie.cn

[U97] JS：并发请求
来源：http://zb.muxihuayi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://jh.gzmigu.cn

[U98] JS：fetch 带 JSON
来源：http://mr.bjjhwx.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gz.hnjuh.cn

[U99] JS：事件监听
来源：http://ow.jctech888.com.cn

el.addEventListener("click", e => {})
来源：http://kn.szsharing.cn

[U100] JS：DOM 查询
来源：http://kg.hahajie.cn

document.querySelector(".item")
来源：http://kh.hahajie.cn

[U101] JS：classList 操作
来源：http://bu.shxzukj.cn

el.classList.toggle("active")
来源：http://zk.hnjuh.cn

[U102] JS：本地存储
来源：http://si.shtwfgs.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://go.szxytkj.cn

[U103] JS：定时器
来源：http://ke.yuntaijiaju.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ed.hnjuh.cn

[U104] JS：防抖
来源：http://zk.szxytkj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://en.nszjky.cn

[U105] JS：节流
来源：http://fg.9csxet.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pi.colortex.cn

[U106] JS：日期格式化
来源：http://ve.shtwfgs.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://em.huixinmuqiang.cn

[U107] JS：数字千分位
来源：http://yl.bjjhwx.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ku.shxzukj.cn

[U108] JS：随机整数
来源：http://yf.huanxung.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ze.szsharing.cn

[U109] JS：数组分组
来源：http://tf.521024.cn

Object.groupBy(arr, x => x.type)
来源：http://qk.huixinmuqiang.cn

[U110] JS：数组分块
来源：http://uh.shxzukj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tm.gzmigu.cn

[U111] JS：对象转 Map
来源：http://gf.hahajie.cn

new Map(Object.entries(obj))
来源：http://sv.muxihuayi.cn

[U112] JS：字符串补位
来源：http://rd.jianghongdianzi.cn

"7".padStart(3, "0")
来源：http://zo.shtwfgs.cn

[U113] JS：正则替换全部
来源：http://cw.huanxung.cn

s.replaceAll("a", "b")
来源：http://pd.521024.cn

[U114] JS：JSON 深比较
来源：http://hd.szxytkj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://lh.huixinmuqiang.cn

[U115] JS：生成 UUID
来源：http://vk.shxzukj.cn

crypto.randomUUID()
来源：http://xk.bookmarksfly.cn

[U116] JS：类型检查（JSDoc）
来源：http://bg.shxzskj.cn

/** @param {string} name */ function f(name) {}
来源：http://xd.yuntaijiaju.cn

[U117] JS：单元测试
来源：http://ng.chemitech.net.cn

npm i -D vitest;  npx vitest
来源：http://nx.jianghongdianzi.cn

[U118] JS：开发服务器
来源：http://qz.9csxet.cn

npm i -D vite;  npx vite
来源：http://mz.wgjwhj.cn


<!-- 参考信息 -->