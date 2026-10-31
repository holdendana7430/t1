代发 wailian999

[T39] Lua：模式匹配
来源：http://uo.yuntaijiaju.cn

string.find(s, "%d+")
来源：http://ll.jianghongdianzi.cn

[T40] Lua：元表
来源：http://xv.huixiangedu.cn

setmetatable({}, { __index = base })
来源：http://dd.newstarts.cn

[T41] Perl：Hello World
来源：http://qx.nicolike.cn

print "Hello\n";
来源：http://cg.szsharing.cn

[T42] Perl：变量类型
来源：http://cb.shtwfgs.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://or.chemitech.net.cn

[T43] Perl：字符串插值
来源：http://uv.muxihuayi.cn

"值: $a"
来源：http://do.muxihuayi.cn

[T44] Perl：条件
来源：http://rk.bookmarksfly.cn

if ($a > 0) { print "正"; }
来源：http://yi.jctech888.com.cn

[T45] Perl：数组遍历
来源：http://vy.lnxyls.cn

for my $x (@arr) { print $x; }
来源：http://ee.asd995.cn

[T46] Perl：哈希操作
来源：http://xz.panjiajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ea.jianghongdianzi.cn

[T47] Perl：正则捕获
来源：http://fo.huixinmuqiang.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://gd.gzmigu.cn

[T48] Perl：正则替换
来源：http://gk.shtwfgs.cn

$s =~ s/old/new/g;
来源：http://mp.hnjuh.cn

[T49] Perl：函数
来源：http://jr.yuntaijiaju.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dt.nszjky.cn

[T50] Perl：逐行读文件
来源：http://cx.panjiajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://cu.huixinmuqiang.cn

while (my $line = <$fh>) { print $line; }
来源：http://in.nicolike.cn

[T51] Scala：Hello World
来源：http://jm.521024.cn

println("Hello")
来源：http://cr.gzmigu.cn

[T52] Scala：变量
来源：http://vd.yuexingan06.cn

val a = 1;  var b = 2
来源：http://jp.9csxet.cn

[T53] Scala：字符串插值
来源：http://en.bjjhwx.cn

s"值: $b"
来源：http://pf.szxytkj.cn

[T54] Scala：集合映射
来源：http://ei.huixinmuqiang.cn

List(1, 2, 3).map(_ * 2)
来源：http://gi.9csxet.cn

[T55] Scala：集合过滤
来源：http://ii.bjjhwx.cn

List(1, 2, 3).filter(_ > 1)
来源：http://lp.jianghongdianzi.cn

[T56] Scala：样例类
来源：http://ww.bjjhwx.cn

case class User(name: String, age: Int)
来源：http://um.9csxet.cn

[T57] Scala：模式匹配
来源：http://mk.huixiangedu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://es.9csxet.cn

[T58] Scala：函数定义
来源：http://ix.gzmigu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://na.nicolike.cn

[T59] Scala：循环
来源：http://hb.huanxung.cn

for (i <- 1 to 10) println(i)
来源：http://oi.huanxung.cn

[T60] Scala：折叠
来源：http://di.hahajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wk.gzmigu.cn

================================================================================
来源：http://jl.bjjhwx.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dw.hahajie.cn

================================================================================
来源：http://ec.newstarts.cn

[U01] Py：创建虚拟环境
来源：http://zm.hnjuh.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ai.wgjwhj.cn

[U02] Py：导出 / 安装依赖
来源：http://sh.nszjky.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://df.panjiajie.cn

[U03] Py：加载 .env 配置
来源：http://as.521024.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://iq.haigaiapp.cn

[U04] Py：变量调试打印
来源：http://cb.lnxyls.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://at.wgjwhj.cn

[U05] Py：列表去重且保序
来源：http://za.newstarts.cn

list(dict.fromkeys(arr))
来源：http://yl.huixinmuqiang.cn

[U06] Py：合并两个字典
来源：http://rm.panjiajie.cn

{**a, **b}
来源：http://uo.chemitech.net.cn

[U07] Py：反转字典键值
来源：http://bq.521024.cn

{v: k for k, v in d.items()}
来源：http://fl.chemitech.net.cn

[U08] Py：展平二维列表
来源：http://ne.yuexingan06.cn

[y for x in nested for y in x]
来源：http://sg.gzmigu.cn

[U09] Py：字典取最大值的键
来源：http://kp.szxytkj.cn

max(d, key=d.get)
来源：http://ai.bookmarksfly.cn

[U10] Py：按值排序字典
来源：http://xw.hahajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qg.newstarts.cn

[U11] Py：生成器表达式
来源：http://op.huixiangedu.cn

(x * 2 for x in arr)
来源：http://ks.haigaiapp.cn

[U12] Py：取出现最多的 3 个元素
来源：http://hr.shxzukj.cn

Counter(arr).most_common(3)
来源：http://ma.shxzskj.cn

[U13] Py：固定长度队列
来源：http://su.huixiangedu.cn

deque(maxlen=10)
来源：http://ca.asd995.cn

[U14] Py：分组收集到列表
来源：http://hz.chemitech.net.cn

defaultdict(list)
来源：http://pb.bjjhwx.cn

[U15] Py：高精度计时
来源：http://zp.bookmarksfly.cn

t = time.perf_counter()
来源：http://nu.wgjwhj.cn

[U16] Py：命令行参数解析
来源：http://dm.nszjky.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ir.muxihuayi.cn

[U17] Py：初始化日志
来源：http://ks.shxzukj.cn

logging.basicConfig(level=logging.INFO)
来源：http://ds.nszjky.cn

[U18] Py：预编译正则
来源：http://xc.gzmigu.cn

pat = re.compile(r"\d+")
来源：http://eh.shxzukj.cn

[U19] Py：正则替换带回调
来源：http://yp.wgjwhj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wd.chemitech.net.cn

[U20] Py：缓存函数结果
来源：http://ty.9csxet.cn

@functools.lru_cache(maxsize=None)
来源：http://cc.muxihuayi.cn

[U21] Py：自定义上下文管理器
来源：http://dj.wgjwhj.cn

@contextlib.contextmanager
来源：http://cm.huixinmuqiang.cn

[U22] Py：矩阵转置
来源：http://ix.521024.cn

list(zip(*m))
来源：http://hb.newstarts.cn

[U23] Py：分块读取大文件
来源：http://of.chemitech.net.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rh.muxihuayi.cn

[U24] Py：路径操作
来源：http://dc.newstarts.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dn.szsharing.cn

[U25] Py：CSV 按字典读
来源：http://hk.bjjhwx.cn

csv.DictReader(f)
来源：http://rr.colortex.cn

[U26] Py：并发下载
来源：http://hs.jianghongdianzi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qs.hahajie.cn

[U27] Py：异步 HTTP
来源：http://sj.shtwfgs.cn

aiohttp.ClientSession() 配合 async with
来源：http://ww.bookmarksfly.cn

[U28] Py：类型别名
来源：http://hu.huanxung.cn

UserId = int
来源：http://hn.hnjuh.cn

[U29] Py：属性校验
来源：http://ac.szsharing.cn

@property 与 @x.setter 配合
来源：http://bu.haigaiapp.cn

[U30] Py：数据类
来源：http://zx.newstarts.cn

@dataclass(slots=True)
来源：http://gr.huixinmuqiang.cn

[U31] Py：单测
来源：http://lo.jianghongdianzi.cn

python -m pytest -q
来源：http://dj.yuntaijiaju.cn

[U32] Py：代码格式化
来源：http://ol.bjjhwx.cn

ruff format . && ruff check --fix .
来源：http://ed.szxytkj.cn

[U33] Py：打包发布
来源：http://bp.521024.cn

python -m build  （依赖 pyproject.toml）
来源：http://rh.huixinmuqiang.cn

[U34] Py：判断编码
来源：http://ec.bjjhwx.cn

chardet.detect(raw)
来源：http://ah.jianghongdianzi.cn

[U35] Py：发送邮件
来源：http://ys.yuexingan06.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cz.huanxung.cn

[U36] Py：定时任务
来源：http://zu.colortex.cn

schedule.every(10).minutes.do(job)
来源：http://uy.asd995.cn

[U37] Py：读写 Excel
来源：http://go.colortex.cn

pandas.read_excel / DataFrame.to_excel
来源：http://lq.huixinmuqiang.cn

[U38] Py：获取脚本所在目录
来源：http://mx.huixinmuqiang.cn

Path(__file__).resolve().parent
来源：http://lv.jianghongdianzi.cn

[U39] Py：判断是否在交互环境
来源：http://gm.hahajie.cn

sys.stdout.isatty()
来源：http://be.bookmarksfly.cn

[U40] Py：打印到标准错误
来源：http://xe.nszjky.cn

print("err", file=sys.stderr)
来源：http://bg.shtwfgs.cn

[U41] PHP：初始化 Composer 项目
来源：http://zf.shxzukj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://dw.shtwfgs.cn

[U42] PHP：PSR-4 自动加载
来源：http://yj.yuntaijiaju.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qp.chemitech.net.cn

[U43] PHP：声明命名空间
来源：http://et.lnxyls.cn

namespace App\Http;
来源：http://bd.jctech888.com.cn

[U44] PHP：开启严格类型
来源：http://bv.hnjuh.cn

declare(strict_types=1);
来源：http://yc.wgjwhj.cn

[U45] PHP：类型声明与返回类型
来源：http://yj.shtwfgs.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://um.wgjwhj.cn

[U46] PHP：可空类型
来源：http://gi.jianghongdianzi.cn

?string $name = null
来源：http://zx.wgjwhj.cn

[U47] PHP：联合类型
来源：http://jv.nszjky.cn

int|string $id
来源：http://rn.haigaiapp.cn

[U48] PHP：纯枚举
来源：http://le.gzmigu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dp.newstarts.cn

[U49] PHP：只读属性
来源：http://mq.yuexingan06.cn

public readonly string $name
来源：http://wm.newstarts.cn

[U50] PHP：构造器属性提升
来源：http://zu.colortex.cn

public function __construct(private int $id) {}
来源：http://xs.shtwfgs.cn

[U51] PHP：数组解构
来源：http://sp.szsharing.cn

[$a, $b] = $arr;
来源：http://zb.haigaiapp.cn

[U52] PHP：箭头函数
来源：http://xg.wgjwhj.cn

$double = fn($x) => $x * 2;
来源：http://vf.huixinmuqiang.cn

[U53] PHP：空合并运算符
来源：http://ed.muxihuayi.cn

$v = $a ?? $b ?? "default";
来源：http://ku.bjjhwx.cn

[U54] PHP：空安全调用
来源：http://ui.huanxung.cn

$obj?->method()
来源：http://tg.bookmarksfly.cn

[U55] PHP：match 表达式
来源：http://gf.lnxyls.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wu.asd995.cn

[U56] PHP：命名参数
来源：http://xf.colortex.cn

f(a: 1, b: 2)
来源：http://dv.wgjwhj.cn

[U57] PHP：字符串插值
来源：http://gk.jctech888.com.cn

"值: {$a}"
来源：http://ul.bookmarksfly.cn

[U58] PHP：数组三件套
来源：http://gp.bookmarksfly.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gh.chemitech.net.cn

[U59] PHP：自定义排序
来源：http://rl.yuexingan06.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bc.asd995.cn

[U60] PHP：JSON 编解码
来源：http://yj.jianghongdianzi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lb.asd995.cn

[U61] PHP：正则
来源：http://fq.szxytkj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pf.521024.cn

[U62] PHP：日期对象
来源：http://if.szxytkj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nm.muxihuayi.cn

[U63] PHP：文件读写
来源：http://no.szxytkj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xw.nszjky.cn

[U64] PHP：目录遍历
来源：http://lz.nszjky.cn

glob("dir/*.php");  scandir("dir");
来源：http://yl.panjiajie.cn

[U65] PHP：会话
来源：http://qh.colortex.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://gp.huanxung.cn

[U66] PHP：设置 Cookie
来源：http://nh.hnjuh.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kg.jianghongdianzi.cn

[U67] PHP：处理文件上传
来源：http://jg.shtwfgs.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rh.jianghongdianzi.cn

[U68] PHP：PDO 连接
来源：http://oz.huixinmuqiang.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jn.huixiangedu.cn

[U69] PHP：PDO 预处理
来源：http://yw.hahajie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hd.huixinmuqiang.cn

[U70] PHP：PDO 事务
来源：http://dg.hnjuh.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zp.hnjuh.cn

[U71] PHP：抛出异常
来源：http://dg.panjiajie.cn

throw new RuntimeException("失败", 500);
来源：http://xt.huixiangedu.cn

[U72] PHP：写错误日志
来源：http://bn.shxzukj.cn

error_log("失败: " . $e->getMessage());
来源：http://dl.szxytkj.cn

[U73] PHP：读取 ini 配置
来源：http://bo.9csxet.cn

parse_ini_file("config.ini", true)
来源：http://pf.szsharing.cn

[U74] PHP：读取环境变量
来源：http://fj.hahajie.cn

getenv("APP_ENV") ?: "production"
来源：http://xf.chemitech.net.cn

[U75] PHP：依赖注入
来源：http://bd.9csxet.cn

composer require psr/container
来源：http://bj.shxzukj.cn

[U76] PHP：简单路由
来源：http://za.colortex.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gk.haigaiapp.cn

[U77] PHP：模板渲染
来源：http://ei.asd995.cn

composer require twig/twig
来源：http://kb.muxihuayi.cn

[U78] PHP：单元测试
来源：http://ev.huanxung.cn

composer require --dev phpunit/phpunit
来源：http://dx.nicolike.cn

[U79] PHP：静态分析
来源：http://ts.hnjuh.cn

composer require --dev phpstan/phpstan
来源：http://al.huanxung.cn

[U80] PHP：代码规范修复
来源：http://yz.asd995.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qv.shxzskj.cn

[U81] JS：初始化项目
来源：http://ji.bjjhwx.cn

npm init -y;  npm i express
来源：http://yf.chemitech.net.cn

[U82] JS：package.json 脚本
来源：http://pd.gzmigu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gt.muxihuayi.cn

[U83] JS：ES Module 导入导出
来源：http://gz.asd995.cn

export const a = 1;  import { a } from "./m.js";
来源：http://jb.asd995.cn

[U84] JS：CommonJS 写法
来源：http://dt.9csxet.cn

module.exports = { a };  const { a } = require("./m");
来源：http://we.yuntaijiaju.cn

[U85] JS：可选链
来源：http://eb.lnxyls.cn

a?.b?.c
来源：http://au.yuexingan06.cn

[U86] JS：空值合并
来源：http://uk.yuntaijiaju.cn

a ?? b
来源：http://ds.hahajie.cn

[U87] JS：解构默认值
来源：http://qz.jctech888.com.cn

const { a = 1, b = 2 } = obj;
来源：http://yy.huixiangedu.cn

[U88] JS：对象展开合并
来源：http://re.chemitech.net.cn

{ ...a, ...b }
来源：http://rr.gzmigu.cn

[U89] JS：数组去重
来源：http://vn.huixinmuqiang.cn

[...new Set(arr)]
来源：http://sw.nicolike.cn

[U90] JS：数字数组排序
来源：http://um.shxzskj.cn

[...arr].sort((a, b) => a - b)
来源：http://zq.haigaiapp.cn

[U91] JS：对象键值遍历
来源：http://qz.nszjky.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://be.jctech888.com.cn

[U92] JS：深拷贝
来源：http://bz.nszjky.cn

structuredClone(obj)
来源：http://hh.yuexingan06.cn

[U93] JS：模板字符串
来源：http://hj.hnjuh.cn

`共 ${n} 条`
来源：http://cz.9csxet.cn

[U94] JS：箭头函数
来源：http://up.muxihuayi.cn

const double = x => x * 2;
来源：http://xt.nicolike.cn

[U95] JS：Promise 包装
来源：http://mi.chemitech.net.cn

new Promise((resolve, reject) => {})
来源：http://md.lnxyls.cn

[U96] JS：async/await 与异常
来源：http://hq.lnxyls.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lq.521024.cn

[U97] JS：并发请求
来源：http://es.huanxung.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://oj.yuexingan06.cn

[U98] JS：fetch 带 JSON
来源：http://xn.huanxung.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pg.huixiangedu.cn

[U99] JS：事件监听
来源：http://bu.bjjhwx.cn

el.addEventListener("click", e => {})
来源：http://pb.huanxung.cn

[U100] JS：DOM 查询
来源：http://pu.yuexingan06.cn

document.querySelector(".item")
来源：http://ne.jctech888.com.cn

[U101] JS：classList 操作
来源：http://hw.9csxet.cn

el.classList.toggle("active")
来源：http://ck.bookmarksfly.cn

[U102] JS：本地存储
来源：http://vk.bookmarksfly.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://rj.huixiangedu.cn

[U103] JS：定时器
来源：http://qx.jctech888.com.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kp.colortex.cn

[U104] JS：防抖
来源：http://aj.huanxung.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yj.jianghongdianzi.cn

[U105] JS：节流
来源：http://dt.colortex.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rt.jctech888.com.cn

[U106] JS：日期格式化
来源：http://br.shxzskj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xc.lnxyls.cn

[U107] JS：数字千分位
来源：http://yd.nszjky.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zb.colortex.cn

[U108] JS：随机整数
来源：http://cu.yuexingan06.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ao.gzmigu.cn

[U109] JS：数组分组
来源：http://zk.asd995.cn

Object.groupBy(arr, x => x.type)
来源：http://tb.panjiajie.cn

[U110] JS：数组分块
来源：http://ry.chemitech.net.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jp.9csxet.cn

[U111] JS：对象转 Map
来源：http://jj.nszjky.cn

new Map(Object.entries(obj))
来源：http://zh.szxytkj.cn

[U112] JS：字符串补位
来源：http://vt.huanxung.cn

"7".padStart(3, "0")
来源：http://zp.hnjuh.cn

[U113] JS：正则替换全部
来源：http://uo.nszjky.cn

s.replaceAll("a", "b")
来源：http://je.bookmarksfly.cn

[U114] JS：JSON 深比较
来源：http://ir.colortex.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://tg.shtwfgs.cn

[U115] JS：生成 UUID
来源：http://ud.newstarts.cn

crypto.randomUUID()
来源：http://fz.yuexingan06.cn

[U116] JS：类型检查（JSDoc）
来源：http://vm.nicolike.cn

/** @param {string} name */ function f(name) {}
来源：http://zl.muxihuayi.cn

[U117] JS：单元测试
来源：http://hj.shtwfgs.cn

npm i -D vitest;  npx vitest
来源：http://rb.szxytkj.cn

[U118] JS：开发服务器
来源：http://tz.szsharing.cn

npm i -D vite;  npx vite
来源：http://my.chemitech.net.cn

[U119] JS：生产构建
来源：http://es.nicolike.cn

npx vite build
来源：http://xw.colortex.cn

[U120] JS：读取环境变量（Vite）
来源：http://sg.haigaiapp.cn

import.meta.env.VITE_API_URL
来源：http://ll.muxihuayi.cn

================================================================================
来源：http://hn.asd995.cn

统计汇总
来源：http://ix.bookmarksfly.cn

================================================================================
来源：http://bs.huixiangedu.cn

按语言统计（条）：
来源：http://it.521024.cn

Python ......... 252
来源：http://cb.lnxyls.cn

PHP ............ 252
来源：http://sk.haigaiapp.cn

JavaScript ..... 252
来源：http://nh.hahajie.cn

TypeScript ..... 212
来源：http://zo.asd995.cn

Java ........... 212
来源：http://zr.shxzskj.cn

Go ............. 212
来源：http://fj.wgjwhj.cn

Ruby ........... 212
来源：http://ms.hnjuh.cn

C# ............. 212
来源：http://ls.wgjwhj.cn


<!-- 参考信息 -->