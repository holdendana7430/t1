代发 wailian999

[T33] Lua：表（数组）
来源：http://uk.yuexingan06.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://me.muxihuayi.cn

[T34] Lua：遍历表
来源：http://vl.chemitech.net.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://fp.shtwfgs.cn

[T35] Lua：字典表
来源：http://ud.huixinmuqiang.cn

local d = { a = 1 };  d.b = 2
来源：http://zb.szsharing.cn

[T36] Lua：函数
来源：http://nm.chemitech.net.cn

function add(a, b) return a + b end
来源：http://xo.muxihuayi.cn

[T37] Lua：字符串拼接
来源：http://ju.chemitech.net.cn

"a" .. "b"
来源：http://dp.chemitech.net.cn

[T38] Lua：条件
来源：http://bm.huanxung.cn

if x > 0 then print("正") end
来源：http://la.shxzskj.cn

[T39] Lua：模式匹配
来源：http://mz.newstarts.cn

string.find(s, "%d+")
来源：http://bx.bookmarksfly.cn

[T40] Lua：元表
来源：http://rm.huixinmuqiang.cn

setmetatable({}, { __index = base })
来源：http://mt.hnjuh.cn

[T41] Perl：Hello World
来源：http://dm.gzmigu.cn

print "Hello\n";
来源：http://yi.szsharing.cn

[T42] Perl：变量类型
来源：http://qo.szsharing.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pp.9csxet.cn

[T43] Perl：字符串插值
来源：http://ky.shtwfgs.cn

"值: $a"
来源：http://cm.jianghongdianzi.cn

[T44] Perl：条件
来源：http://dq.521024.cn

if ($a > 0) { print "正"; }
来源：http://ex.shxzskj.cn

[T45] Perl：数组遍历
来源：http://fh.shtwfgs.cn

for my $x (@arr) { print $x; }
来源：http://mo.jianghongdianzi.cn

[T46] Perl：哈希操作
来源：http://fu.panjiajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vt.shtwfgs.cn

[T47] Perl：正则捕获
来源：http://oa.szxytkj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://lt.colortex.cn

[T48] Perl：正则替换
来源：http://wf.newstarts.cn

$s =~ s/old/new/g;
来源：http://wd.panjiajie.cn

[T49] Perl：函数
来源：http://hg.hahajie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ne.bookmarksfly.cn

[T50] Perl：逐行读文件
来源：http://lb.muxihuayi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://cd.huanxung.cn

while (my $line = <$fh>) { print $line; }
来源：http://lo.521024.cn

[T51] Scala：Hello World
来源：http://rq.newstarts.cn

println("Hello")
来源：http://hq.gzmigu.cn

[T52] Scala：变量
来源：http://hb.yuntaijiaju.cn

val a = 1;  var b = 2
来源：http://xu.asd995.cn

[T53] Scala：字符串插值
来源：http://hs.huixinmuqiang.cn

s"值: $b"
来源：http://vo.gzmigu.cn

[T54] Scala：集合映射
来源：http://jw.shtwfgs.cn

List(1, 2, 3).map(_ * 2)
来源：http://ne.yuexingan06.cn

[T55] Scala：集合过滤
来源：http://ov.haigaiapp.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qr.panjiajie.cn

[T56] Scala：样例类
来源：http://fl.nszjky.cn

case class User(name: String, age: Int)
来源：http://fh.panjiajie.cn

[T57] Scala：模式匹配
来源：http://bu.lnxyls.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://va.huixiangedu.cn

[T58] Scala：函数定义
来源：http://pl.bjjhwx.cn

def add(a: Int, b: Int): Int = a + b
来源：http://pc.haigaiapp.cn

[T59] Scala：循环
来源：http://jx.muxihuayi.cn

for (i <- 1 to 10) println(i)
来源：http://cq.9csxet.cn

[T60] Scala：折叠
来源：http://lm.wgjwhj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ox.hahajie.cn

================================================================================
来源：http://ff.hahajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ma.lnxyls.cn

================================================================================
来源：http://hn.bjjhwx.cn

[U01] Py：创建虚拟环境
来源：http://nu.9csxet.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ox.colortex.cn

[U02] Py：导出 / 安装依赖
来源：http://yw.wgjwhj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://md.haigaiapp.cn

[U03] Py：加载 .env 配置
来源：http://na.shxzukj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://jo.szxytkj.cn

[U04] Py：变量调试打印
来源：http://lq.chemitech.net.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jd.haigaiapp.cn

[U05] Py：列表去重且保序
来源：http://jb.panjiajie.cn

list(dict.fromkeys(arr))
来源：http://iv.chemitech.net.cn

[U06] Py：合并两个字典
来源：http://eb.szxytkj.cn

{**a, **b}
来源：http://py.haigaiapp.cn

[U07] Py：反转字典键值
来源：http://ox.asd995.cn

{v: k for k, v in d.items()}
来源：http://jl.yuntaijiaju.cn

[U08] Py：展平二维列表
来源：http://ob.huixinmuqiang.cn

[y for x in nested for y in x]
来源：http://ei.chemitech.net.cn

[U09] Py：字典取最大值的键
来源：http://bt.9csxet.cn

max(d, key=d.get)
来源：http://ke.jctech888.com.cn

[U10] Py：按值排序字典
来源：http://bm.hnjuh.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sj.nszjky.cn

[U11] Py：生成器表达式
来源：http://wp.yuntaijiaju.cn

(x * 2 for x in arr)
来源：http://wn.huixinmuqiang.cn

[U12] Py：取出现最多的 3 个元素
来源：http://di.shxzukj.cn

Counter(arr).most_common(3)
来源：http://bl.yuexingan06.cn

[U13] Py：固定长度队列
来源：http://zg.jianghongdianzi.cn

deque(maxlen=10)
来源：http://eb.shxzukj.cn

[U14] Py：分组收集到列表
来源：http://nz.521024.cn

defaultdict(list)
来源：http://xr.wgjwhj.cn

[U15] Py：高精度计时
来源：http://hx.hahajie.cn

t = time.perf_counter()
来源：http://pi.jianghongdianzi.cn

[U16] Py：命令行参数解析
来源：http://fc.9csxet.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hy.hahajie.cn

[U17] Py：初始化日志
来源：http://ih.szxytkj.cn

logging.basicConfig(level=logging.INFO)
来源：http://po.shxzukj.cn

[U18] Py：预编译正则
来源：http://it.gzmigu.cn

pat = re.compile(r"\d+")
来源：http://ci.haigaiapp.cn

[U19] Py：正则替换带回调
来源：http://av.hahajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://io.9csxet.cn

[U20] Py：缓存函数结果
来源：http://pm.nicolike.cn

@functools.lru_cache(maxsize=None)
来源：http://uw.huanxung.cn

[U21] Py：自定义上下文管理器
来源：http://oq.9csxet.cn

@contextlib.contextmanager
来源：http://zv.szxytkj.cn

[U22] Py：矩阵转置
来源：http://qj.panjiajie.cn

list(zip(*m))
来源：http://dc.nicolike.cn

[U23] Py：分块读取大文件
来源：http://nh.asd995.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vm.gzmigu.cn

[U24] Py：路径操作
来源：http://of.huixiangedu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ca.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://mu.gzmigu.cn

csv.DictReader(f)
来源：http://zp.shxzskj.cn

[U26] Py：并发下载
来源：http://ei.asd995.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bg.bookmarksfly.cn

[U27] Py：异步 HTTP
来源：http://nh.nicolike.cn

aiohttp.ClientSession() 配合 async with
来源：http://zb.gzmigu.cn

[U28] Py：类型别名
来源：http://vp.shtwfgs.cn

UserId = int
来源：http://ir.huixinmuqiang.cn

[U29] Py：属性校验
来源：http://lk.yuexingan06.cn

@property 与 @x.setter 配合
来源：http://nz.wgjwhj.cn

[U30] Py：数据类
来源：http://vm.colortex.cn

@dataclass(slots=True)
来源：http://jy.bookmarksfly.cn

[U31] Py：单测
来源：http://ev.haigaiapp.cn

python -m pytest -q
来源：http://jr.huixinmuqiang.cn

[U32] Py：代码格式化
来源：http://jm.colortex.cn

ruff format . && ruff check --fix .
来源：http://dd.hahajie.cn

[U33] Py：打包发布
来源：http://yx.newstarts.cn

python -m build  （依赖 pyproject.toml）
来源：http://zi.9csxet.cn

[U34] Py：判断编码
来源：http://pm.wgjwhj.cn

chardet.detect(raw)
来源：http://xj.huixinmuqiang.cn

[U35] Py：发送邮件
来源：http://lv.hahajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hj.nicolike.cn

[U36] Py：定时任务
来源：http://ks.huixinmuqiang.cn

schedule.every(10).minutes.do(job)
来源：http://vw.yuexingan06.cn

[U37] Py：读写 Excel
来源：http://yx.yuexingan06.cn

pandas.read_excel / DataFrame.to_excel
来源：http://vl.nszjky.cn

[U38] Py：获取脚本所在目录
来源：http://wt.haigaiapp.cn

Path(__file__).resolve().parent
来源：http://be.9csxet.cn

[U39] Py：判断是否在交互环境
来源：http://tt.lnxyls.cn

sys.stdout.isatty()
来源：http://gc.panjiajie.cn

[U40] Py：打印到标准错误
来源：http://do.haigaiapp.cn

print("err", file=sys.stderr)
来源：http://xg.yuexingan06.cn

[U41] PHP：初始化 Composer 项目
来源：http://lj.chemitech.net.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://up.nszjky.cn

[U42] PHP：PSR-4 自动加载
来源：http://lr.newstarts.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zj.jctech888.com.cn

[U43] PHP：声明命名空间
来源：http://yn.szxytkj.cn

namespace App\Http;
来源：http://jj.nicolike.cn

[U44] PHP：开启严格类型
来源：http://mt.asd995.cn

declare(strict_types=1);
来源：http://bx.lnxyls.cn

[U45] PHP：类型声明与返回类型
来源：http://bu.bookmarksfly.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://wa.wgjwhj.cn

[U46] PHP：可空类型
来源：http://ms.chemitech.net.cn

?string $name = null
来源：http://fh.jianghongdianzi.cn

[U47] PHP：联合类型
来源：http://qe.hnjuh.cn

int|string $id
来源：http://et.9csxet.cn

[U48] PHP：纯枚举
来源：http://yw.asd995.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wq.shtwfgs.cn

[U49] PHP：只读属性
来源：http://rf.gzmigu.cn

public readonly string $name
来源：http://vs.wgjwhj.cn

[U50] PHP：构造器属性提升
来源：http://us.gzmigu.cn

public function __construct(private int $id) {}
来源：http://gc.bookmarksfly.cn

[U51] PHP：数组解构
来源：http://ep.shxzskj.cn

[$a, $b] = $arr;
来源：http://je.hnjuh.cn

[U52] PHP：箭头函数
来源：http://ux.yuexingan06.cn

$double = fn($x) => $x * 2;
来源：http://vu.muxihuayi.cn

[U53] PHP：空合并运算符
来源：http://cf.colortex.cn

$v = $a ?? $b ?? "default";
来源：http://ct.huixinmuqiang.cn

[U54] PHP：空安全调用
来源：http://ht.lnxyls.cn

$obj?->method()
来源：http://yx.hahajie.cn

[U55] PHP：match 表达式
来源：http://im.newstarts.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ej.haigaiapp.cn

[U56] PHP：命名参数
来源：http://qn.nszjky.cn

f(a: 1, b: 2)
来源：http://xq.huanxung.cn

[U57] PHP：字符串插值
来源：http://xo.panjiajie.cn

"值: {$a}"
来源：http://xr.colortex.cn

[U58] PHP：数组三件套
来源：http://ki.shtwfgs.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nk.panjiajie.cn

[U59] PHP：自定义排序
来源：http://ph.hahajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uh.shxzskj.cn

[U60] PHP：JSON 编解码
来源：http://pw.huanxung.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bi.chemitech.net.cn

[U61] PHP：正则
来源：http://tc.shxzskj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cu.wgjwhj.cn

[U62] PHP：日期对象
来源：http://zp.szxytkj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://to.521024.cn

[U63] PHP：文件读写
来源：http://ow.9csxet.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vd.haigaiapp.cn

[U64] PHP：目录遍历
来源：http://dy.yuexingan06.cn

glob("dir/*.php");  scandir("dir");
来源：http://hw.nszjky.cn

[U65] PHP：会话
来源：http://pi.shxzskj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://fm.colortex.cn

[U66] PHP：设置 Cookie
来源：http://hx.521024.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ql.huixiangedu.cn

[U67] PHP：处理文件上传
来源：http://us.nicolike.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kb.nszjky.cn

[U68] PHP：PDO 连接
来源：http://du.chemitech.net.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qk.lnxyls.cn

[U69] PHP：PDO 预处理
来源：http://wn.muxihuayi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sg.bjjhwx.cn

[U70] PHP：PDO 事务
来源：http://bv.yuntaijiaju.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ci.wgjwhj.cn

[U71] PHP：抛出异常
来源：http://cl.521024.cn

throw new RuntimeException("失败", 500);
来源：http://il.chemitech.net.cn

[U72] PHP：写错误日志
来源：http://xl.newstarts.cn

error_log("失败: " . $e->getMessage());
来源：http://jt.huanxung.cn

[U73] PHP：读取 ini 配置
来源：http://ec.jianghongdianzi.cn

parse_ini_file("config.ini", true)
来源：http://gi.hahajie.cn

[U74] PHP：读取环境变量
来源：http://dk.muxihuayi.cn

getenv("APP_ENV") ?: "production"
来源：http://rt.shxzukj.cn

[U75] PHP：依赖注入
来源：http://ka.nszjky.cn

composer require psr/container
来源：http://aq.bjjhwx.cn

[U76] PHP：简单路由
来源：http://gr.shxzskj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fn.jianghongdianzi.cn

[U77] PHP：模板渲染
来源：http://vq.muxihuayi.cn

composer require twig/twig
来源：http://hh.bookmarksfly.cn

[U78] PHP：单元测试
来源：http://lt.huixiangedu.cn

composer require --dev phpunit/phpunit
来源：http://yy.asd995.cn

[U79] PHP：静态分析
来源：http://xs.nszjky.cn

composer require --dev phpstan/phpstan
来源：http://uu.nszjky.cn

[U80] PHP：代码规范修复
来源：http://bk.9csxet.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://br.yuntaijiaju.cn

[U81] JS：初始化项目
来源：http://tz.521024.cn

npm init -y;  npm i express
来源：http://vg.huanxung.cn

[U82] JS：package.json 脚本
来源：http://hn.shtwfgs.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ol.jianghongdianzi.cn

[U83] JS：ES Module 导入导出
来源：http://bg.shtwfgs.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zb.panjiajie.cn

[U84] JS：CommonJS 写法
来源：http://yq.huixiangedu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://dn.haigaiapp.cn

[U85] JS：可选链
来源：http://ct.muxihuayi.cn

a?.b?.c
来源：http://pm.nicolike.cn

[U86] JS：空值合并
来源：http://el.colortex.cn

a ?? b
来源：http://hs.jianghongdianzi.cn

[U87] JS：解构默认值
来源：http://gr.hahajie.cn

const { a = 1, b = 2 } = obj;
来源：http://zs.yuexingan06.cn

[U88] JS：对象展开合并
来源：http://xy.yuexingan06.cn

{ ...a, ...b }
来源：http://if.colortex.cn

[U89] JS：数组去重
来源：http://qu.szsharing.cn

[...new Set(arr)]
来源：http://dr.nicolike.cn

[U90] JS：数字数组排序
来源：http://kj.hahajie.cn

[...arr].sort((a, b) => a - b)
来源：http://iz.hahajie.cn

[U91] JS：对象键值遍历
来源：http://jk.jctech888.com.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xj.yuntaijiaju.cn

[U92] JS：深拷贝
来源：http://wl.chemitech.net.cn

structuredClone(obj)
来源：http://ov.shtwfgs.cn

[U93] JS：模板字符串
来源：http://yh.jianghongdianzi.cn

`共 ${n} 条`
来源：http://vp.szxytkj.cn

[U94] JS：箭头函数
来源：http://wi.shxzskj.cn

const double = x => x * 2;
来源：http://nc.huixiangedu.cn

[U95] JS：Promise 包装
来源：http://ty.hahajie.cn

new Promise((resolve, reject) => {})
来源：http://zb.yuntaijiaju.cn

[U96] JS：async/await 与异常
来源：http://ky.jctech888.com.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ha.yuexingan06.cn

[U97] JS：并发请求
来源：http://qx.bookmarksfly.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://eg.chemitech.net.cn

[U98] JS：fetch 带 JSON
来源：http://hf.muxihuayi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rc.bjjhwx.cn

[U99] JS：事件监听
来源：http://uk.wgjwhj.cn

el.addEventListener("click", e => {})
来源：http://ko.521024.cn

[U100] JS：DOM 查询
来源：http://jm.newstarts.cn

document.querySelector(".item")
来源：http://zt.chemitech.net.cn

[U101] JS：classList 操作
来源：http://qr.yuntaijiaju.cn

el.classList.toggle("active")
来源：http://yb.521024.cn

[U102] JS：本地存储
来源：http://tq.521024.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xd.asd995.cn

[U103] JS：定时器
来源：http://oe.nicolike.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fd.yuexingan06.cn

[U104] JS：防抖
来源：http://nz.9csxet.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hk.bookmarksfly.cn

[U105] JS：节流
来源：http://js.yuntaijiaju.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://be.521024.cn

[U106] JS：日期格式化
来源：http://yv.nszjky.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dq.muxihuayi.cn

[U107] JS：数字千分位
来源：http://tz.asd995.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vc.haigaiapp.cn

[U108] JS：随机整数
来源：http://bi.colortex.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fb.shxzskj.cn

[U109] JS：数组分组
来源：http://cq.jctech888.com.cn

Object.groupBy(arr, x => x.type)
来源：http://tm.shtwfgs.cn

[U110] JS：数组分块
来源：http://qw.shxzskj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ah.panjiajie.cn

[U111] JS：对象转 Map
来源：http://ax.yuexingan06.cn

new Map(Object.entries(obj))
来源：http://qw.hnjuh.cn

[U112] JS：字符串补位
来源：http://ue.hahajie.cn

"7".padStart(3, "0")
来源：http://eo.colortex.cn

[U113] JS：正则替换全部
来源：http://cj.521024.cn

s.replaceAll("a", "b")
来源：http://mk.521024.cn

[U114] JS：JSON 深比较
来源：http://ua.jianghongdianzi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://zl.shxzskj.cn

[U115] JS：生成 UUID
来源：http://ml.gzmigu.cn

crypto.randomUUID()
来源：http://py.bookmarksfly.cn

[U116] JS：类型检查（JSDoc）
来源：http://pe.muxihuayi.cn

/** @param {string} name */ function f(name) {}
来源：http://ue.newstarts.cn

[U117] JS：单元测试
来源：http://cr.gzmigu.cn

npm i -D vitest;  npx vitest
来源：http://ks.wgjwhj.cn

[U118] JS：开发服务器
来源：http://aa.colortex.cn

npm i -D vite;  npx vite
来源：http://pv.jctech888.com.cn

[U119] JS：生产构建
来源：http://ai.hnjuh.cn

npx vite build
来源：http://hr.gzmigu.cn

[U120] JS：读取环境变量（Vite）
来源：http://bq.chemitech.net.cn

import.meta.env.VITE_API_URL
来源：http://vi.szxytkj.cn


<!-- 参考信息 -->