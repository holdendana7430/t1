代发 wailian999

[T31] Lua：Hello World
来源：http://zv.huixiangedu.cn

print("Hello")
来源：http://ln.asd995.cn

[T32] Lua：局部变量
来源：http://vw.gzmigu.cn

local a = 1
来源：http://xv.lnxyls.cn

[T33] Lua：表（数组）
来源：http://ya.chemitech.net.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://oe.asd995.cn

[T34] Lua：遍历表
来源：http://jf.shxzukj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://za.newstarts.cn

[T35] Lua：字典表
来源：http://sd.huixiangedu.cn

local d = { a = 1 };  d.b = 2
来源：http://jc.panjiajie.cn

[T36] Lua：函数
来源：http://ob.9csxet.cn

function add(a, b) return a + b end
来源：http://ui.jianghongdianzi.cn

[T37] Lua：字符串拼接
来源：http://xp.yuexingan06.cn

"a" .. "b"
来源：http://st.huanxung.cn

[T38] Lua：条件
来源：http://zc.jianghongdianzi.cn

if x > 0 then print("正") end
来源：http://la.hnjuh.cn

[T39] Lua：模式匹配
来源：http://is.wgjwhj.cn

string.find(s, "%d+")
来源：http://ec.muxihuayi.cn

[T40] Lua：元表
来源：http://kx.shxzukj.cn

setmetatable({}, { __index = base })
来源：http://pp.chemitech.net.cn

[T41] Perl：Hello World
来源：http://uh.nicolike.cn

print "Hello\n";
来源：http://lj.nicolike.cn

[T42] Perl：变量类型
来源：http://cs.hnjuh.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sm.huixinmuqiang.cn

[T43] Perl：字符串插值
来源：http://iw.szsharing.cn

"值: $a"
来源：http://go.bjjhwx.cn

[T44] Perl：条件
来源：http://gt.huixinmuqiang.cn

if ($a > 0) { print "正"; }
来源：http://kn.newstarts.cn

[T45] Perl：数组遍历
来源：http://ew.nicolike.cn

for my $x (@arr) { print $x; }
来源：http://us.hahajie.cn

[T46] Perl：哈希操作
来源：http://hj.huanxung.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ru.hnjuh.cn

[T47] Perl：正则捕获
来源：http://ce.szxytkj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://mx.nicolike.cn

[T48] Perl：正则替换
来源：http://et.asd995.cn

$s =~ s/old/new/g;
来源：http://fu.asd995.cn

[T49] Perl：函数
来源：http://nq.yuexingan06.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ky.wgjwhj.cn

[T50] Perl：逐行读文件
来源：http://lt.nszjky.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rq.shxzukj.cn

while (my $line = <$fh>) { print $line; }
来源：http://wq.huanxung.cn

[T51] Scala：Hello World
来源：http://my.jianghongdianzi.cn

println("Hello")
来源：http://ty.shxzskj.cn

[T52] Scala：变量
来源：http://mp.huanxung.cn

val a = 1;  var b = 2
来源：http://ln.muxihuayi.cn

[T53] Scala：字符串插值
来源：http://cl.hnjuh.cn

s"值: $b"
来源：http://ja.nicolike.cn

[T54] Scala：集合映射
来源：http://zb.jctech888.com.cn

List(1, 2, 3).map(_ * 2)
来源：http://ym.panjiajie.cn

[T55] Scala：集合过滤
来源：http://st.huixinmuqiang.cn

List(1, 2, 3).filter(_ > 1)
来源：http://nx.chemitech.net.cn

[T56] Scala：样例类
来源：http://ja.haigaiapp.cn

case class User(name: String, age: Int)
来源：http://uv.huixinmuqiang.cn

[T57] Scala：模式匹配
来源：http://ba.gzmigu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://qt.nszjky.cn

[T58] Scala：函数定义
来源：http://mq.hnjuh.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zw.yuexingan06.cn

[T59] Scala：循环
来源：http://vn.nicolike.cn

for (i <- 1 to 10) println(i)
来源：http://rc.huanxung.cn

[T60] Scala：折叠
来源：http://fz.yuexingan06.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://uu.hahajie.cn

================================================================================
来源：http://ml.shxzukj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dj.colortex.cn

================================================================================
来源：http://zq.colortex.cn

[U01] Py：创建虚拟环境
来源：http://gx.haigaiapp.cn

python -m venv .venv && source .venv/bin/activate
来源：http://hp.lnxyls.cn

[U02] Py：导出 / 安装依赖
来源：http://kx.huixinmuqiang.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xj.panjiajie.cn

[U03] Py：加载 .env 配置
来源：http://is.gzmigu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xi.jctech888.com.cn

[U04] Py：变量调试打印
来源：http://tt.huanxung.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rc.bjjhwx.cn

[U05] Py：列表去重且保序
来源：http://re.haigaiapp.cn

list(dict.fromkeys(arr))
来源：http://hy.newstarts.cn

[U06] Py：合并两个字典
来源：http://wi.lnxyls.cn

{**a, **b}
来源：http://yi.chemitech.net.cn

[U07] Py：反转字典键值
来源：http://zn.muxihuayi.cn

{v: k for k, v in d.items()}
来源：http://sz.yuexingan06.cn

[U08] Py：展平二维列表
来源：http://af.szxytkj.cn

[y for x in nested for y in x]
来源：http://zb.bjjhwx.cn

[U09] Py：字典取最大值的键
来源：http://hc.jianghongdianzi.cn

max(d, key=d.get)
来源：http://pc.jianghongdianzi.cn

[U10] Py：按值排序字典
来源：http://ae.hahajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ad.shxzukj.cn

[U11] Py：生成器表达式
来源：http://ge.huanxung.cn

(x * 2 for x in arr)
来源：http://ik.nszjky.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ib.asd995.cn

Counter(arr).most_common(3)
来源：http://dw.yuntaijiaju.cn

[U13] Py：固定长度队列
来源：http://yw.haigaiapp.cn

deque(maxlen=10)
来源：http://xj.panjiajie.cn

[U14] Py：分组收集到列表
来源：http://bs.jctech888.com.cn

defaultdict(list)
来源：http://ol.yuexingan06.cn

[U15] Py：高精度计时
来源：http://lm.lnxyls.cn

t = time.perf_counter()
来源：http://ub.jianghongdianzi.cn

[U16] Py：命令行参数解析
来源：http://st.asd995.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ft.szxytkj.cn

[U17] Py：初始化日志
来源：http://km.chemitech.net.cn

logging.basicConfig(level=logging.INFO)
来源：http://qe.lnxyls.cn

[U18] Py：预编译正则
来源：http://ua.shxzskj.cn

pat = re.compile(r"\d+")
来源：http://la.szxytkj.cn

[U19] Py：正则替换带回调
来源：http://vb.bookmarksfly.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ef.panjiajie.cn

[U20] Py：缓存函数结果
来源：http://rm.shxzskj.cn

@functools.lru_cache(maxsize=None)
来源：http://xf.colortex.cn

[U21] Py：自定义上下文管理器
来源：http://md.newstarts.cn

@contextlib.contextmanager
来源：http://lv.hahajie.cn

[U22] Py：矩阵转置
来源：http://qb.bookmarksfly.cn

list(zip(*m))
来源：http://mt.yuntaijiaju.cn

[U23] Py：分块读取大文件
来源：http://mw.huixiangedu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ii.bookmarksfly.cn

[U24] Py：路径操作
来源：http://fl.jianghongdianzi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ld.bookmarksfly.cn

[U25] Py：CSV 按字典读
来源：http://wq.hahajie.cn

csv.DictReader(f)
来源：http://kd.nszjky.cn

[U26] Py：并发下载
来源：http://pf.huanxung.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xp.jianghongdianzi.cn

[U27] Py：异步 HTTP
来源：http://at.nicolike.cn

aiohttp.ClientSession() 配合 async with
来源：http://ej.chemitech.net.cn

[U28] Py：类型别名
来源：http://ll.yuntaijiaju.cn

UserId = int
来源：http://ni.huixinmuqiang.cn

[U29] Py：属性校验
来源：http://ev.muxihuayi.cn

@property 与 @x.setter 配合
来源：http://ui.shtwfgs.cn

[U30] Py：数据类
来源：http://ln.huixiangedu.cn

@dataclass(slots=True)
来源：http://vj.jctech888.com.cn

[U31] Py：单测
来源：http://iv.muxihuayi.cn

python -m pytest -q
来源：http://cx.521024.cn

[U32] Py：代码格式化
来源：http://jc.bookmarksfly.cn

ruff format . && ruff check --fix .
来源：http://cv.jctech888.com.cn

[U33] Py：打包发布
来源：http://ga.9csxet.cn

python -m build  （依赖 pyproject.toml）
来源：http://vw.bookmarksfly.cn

[U34] Py：判断编码
来源：http://kg.jctech888.com.cn

chardet.detect(raw)
来源：http://zu.chemitech.net.cn

[U35] Py：发送邮件
来源：http://iv.newstarts.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://sa.chemitech.net.cn

[U36] Py：定时任务
来源：http://ix.haigaiapp.cn

schedule.every(10).minutes.do(job)
来源：http://go.yuexingan06.cn

[U37] Py：读写 Excel
来源：http://ll.asd995.cn

pandas.read_excel / DataFrame.to_excel
来源：http://aq.nszjky.cn

[U38] Py：获取脚本所在目录
来源：http://av.9csxet.cn

Path(__file__).resolve().parent
来源：http://oa.panjiajie.cn

[U39] Py：判断是否在交互环境
来源：http://mz.yuexingan06.cn

sys.stdout.isatty()
来源：http://rv.colortex.cn

[U40] Py：打印到标准错误
来源：http://yt.panjiajie.cn

print("err", file=sys.stderr)
来源：http://fq.colortex.cn

[U41] PHP：初始化 Composer 项目
来源：http://kt.huixinmuqiang.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ka.9csxet.cn

[U42] PHP：PSR-4 自动加载
来源：http://aj.haigaiapp.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://oi.nszjky.cn

[U43] PHP：声明命名空间
来源：http://ts.szsharing.cn

namespace App\Http;
来源：http://je.colortex.cn

[U44] PHP：开启严格类型
来源：http://hx.shtwfgs.cn

declare(strict_types=1);
来源：http://gw.bjjhwx.cn

[U45] PHP：类型声明与返回类型
来源：http://et.szxytkj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://df.newstarts.cn

[U46] PHP：可空类型
来源：http://po.9csxet.cn

?string $name = null
来源：http://uw.shxzukj.cn

[U47] PHP：联合类型
来源：http://kc.yuexingan06.cn

int|string $id
来源：http://om.yuntaijiaju.cn

[U48] PHP：纯枚举
来源：http://st.521024.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pn.nszjky.cn

[U49] PHP：只读属性
来源：http://cg.shtwfgs.cn

public readonly string $name
来源：http://qd.panjiajie.cn

[U50] PHP：构造器属性提升
来源：http://ss.bookmarksfly.cn

public function __construct(private int $id) {}
来源：http://ep.huixiangedu.cn

[U51] PHP：数组解构
来源：http://cb.hnjuh.cn

[$a, $b] = $arr;
来源：http://se.lnxyls.cn

[U52] PHP：箭头函数
来源：http://ym.szsharing.cn

$double = fn($x) => $x * 2;
来源：http://rl.huixiangedu.cn

[U53] PHP：空合并运算符
来源：http://ce.bookmarksfly.cn

$v = $a ?? $b ?? "default";
来源：http://kq.newstarts.cn

[U54] PHP：空安全调用
来源：http://kf.shxzskj.cn

$obj?->method()
来源：http://ck.muxihuayi.cn

[U55] PHP：match 表达式
来源：http://un.haigaiapp.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qz.panjiajie.cn

[U56] PHP：命名参数
来源：http://ha.nszjky.cn

f(a: 1, b: 2)
来源：http://zc.hnjuh.cn

[U57] PHP：字符串插值
来源：http://fg.wgjwhj.cn

"值: {$a}"
来源：http://wb.shxzskj.cn

[U58] PHP：数组三件套
来源：http://bl.wgjwhj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://db.chemitech.net.cn

[U59] PHP：自定义排序
来源：http://sl.hahajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rp.hahajie.cn

[U60] PHP：JSON 编解码
来源：http://jf.bookmarksfly.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vv.jianghongdianzi.cn

[U61] PHP：正则
来源：http://ox.newstarts.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bw.521024.cn

[U62] PHP：日期对象
来源：http://iw.yuntaijiaju.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ku.haigaiapp.cn

[U63] PHP：文件读写
来源：http://nj.panjiajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vi.bookmarksfly.cn

[U64] PHP：目录遍历
来源：http://xl.huanxung.cn

glob("dir/*.php");  scandir("dir");
来源：http://il.huanxung.cn

[U65] PHP：会话
来源：http://co.muxihuayi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://fc.bjjhwx.cn

[U66] PHP：设置 Cookie
来源：http://it.huixiangedu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zw.bookmarksfly.cn

[U67] PHP：处理文件上传
来源：http://lm.colortex.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bh.huixinmuqiang.cn

[U68] PHP：PDO 连接
来源：http://po.asd995.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vd.9csxet.cn

[U69] PHP：PDO 预处理
来源：http://qv.lnxyls.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mw.9csxet.cn

[U70] PHP：PDO 事务
来源：http://ln.szsharing.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ht.haigaiapp.cn

[U71] PHP：抛出异常
来源：http://ge.shtwfgs.cn

throw new RuntimeException("失败", 500);
来源：http://xb.bookmarksfly.cn

[U72] PHP：写错误日志
来源：http://ck.shxzskj.cn

error_log("失败: " . $e->getMessage());
来源：http://st.hahajie.cn

[U73] PHP：读取 ini 配置
来源：http://aj.newstarts.cn

parse_ini_file("config.ini", true)
来源：http://zq.shtwfgs.cn

[U74] PHP：读取环境变量
来源：http://hn.hnjuh.cn

getenv("APP_ENV") ?: "production"
来源：http://mg.jianghongdianzi.cn

[U75] PHP：依赖注入
来源：http://yi.lnxyls.cn

composer require psr/container
来源：http://ks.huanxung.cn

[U76] PHP：简单路由
来源：http://jb.hnjuh.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hv.panjiajie.cn

[U77] PHP：模板渲染
来源：http://ck.nicolike.cn

composer require twig/twig
来源：http://tu.shxzskj.cn

[U78] PHP：单元测试
来源：http://fh.szxytkj.cn

composer require --dev phpunit/phpunit
来源：http://zm.chemitech.net.cn

[U79] PHP：静态分析
来源：http://fj.nszjky.cn

composer require --dev phpstan/phpstan
来源：http://qo.shxzukj.cn

[U80] PHP：代码规范修复
来源：http://zw.lnxyls.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://aq.huanxung.cn

[U81] JS：初始化项目
来源：http://mz.jctech888.com.cn

npm init -y;  npm i express
来源：http://hv.muxihuayi.cn

[U82] JS：package.json 脚本
来源：http://cb.wgjwhj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kn.lnxyls.cn

[U83] JS：ES Module 导入导出
来源：http://uf.szxytkj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xg.asd995.cn

[U84] JS：CommonJS 写法
来源：http://ow.muxihuayi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://px.asd995.cn

[U85] JS：可选链
来源：http://yq.shxzukj.cn

a?.b?.c
来源：http://tc.521024.cn

[U86] JS：空值合并
来源：http://jx.gzmigu.cn

a ?? b
来源：http://hs.szsharing.cn

[U87] JS：解构默认值
来源：http://ze.yuexingan06.cn

const { a = 1, b = 2 } = obj;
来源：http://zi.nicolike.cn

[U88] JS：对象展开合并
来源：http://rj.szsharing.cn

{ ...a, ...b }
来源：http://wg.huixiangedu.cn

[U89] JS：数组去重
来源：http://sf.szxytkj.cn

[...new Set(arr)]
来源：http://yt.shxzskj.cn

[U90] JS：数字数组排序
来源：http://ir.shxzukj.cn

[...arr].sort((a, b) => a - b)
来源：http://yo.gzmigu.cn

[U91] JS：对象键值遍历
来源：http://la.yuntaijiaju.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gd.yuexingan06.cn

[U92] JS：深拷贝
来源：http://qx.hahajie.cn

structuredClone(obj)
来源：http://dj.panjiajie.cn

[U93] JS：模板字符串
来源：http://sw.huixinmuqiang.cn

`共 ${n} 条`
来源：http://xc.hahajie.cn

[U94] JS：箭头函数
来源：http://vt.muxihuayi.cn

const double = x => x * 2;
来源：http://et.szsharing.cn

[U95] JS：Promise 包装
来源：http://zs.lnxyls.cn

new Promise((resolve, reject) => {})
来源：http://uj.huixiangedu.cn

[U96] JS：async/await 与异常
来源：http://pz.szsharing.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://st.lnxyls.cn

[U97] JS：并发请求
来源：http://vx.shtwfgs.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://cl.521024.cn

[U98] JS：fetch 带 JSON
来源：http://dr.lnxyls.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://so.yuntaijiaju.cn

[U99] JS：事件监听
来源：http://qa.huixiangedu.cn

el.addEventListener("click", e => {})
来源：http://px.huanxung.cn

[U100] JS：DOM 查询
来源：http://io.chemitech.net.cn

document.querySelector(".item")
来源：http://mu.yuexingan06.cn

[U101] JS：classList 操作
来源：http://gv.szxytkj.cn

el.classList.toggle("active")
来源：http://wd.nszjky.cn

[U102] JS：本地存储
来源：http://ux.szxytkj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://zr.szsharing.cn

[U103] JS：定时器
来源：http://rj.haigaiapp.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vk.yuntaijiaju.cn

[U104] JS：防抖
来源：http://kj.521024.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fc.hahajie.cn

[U105] JS：节流
来源：http://jb.haigaiapp.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mr.huixiangedu.cn

[U106] JS：日期格式化
来源：http://zy.yuntaijiaju.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hd.shxzukj.cn

[U107] JS：数字千分位
来源：http://qd.asd995.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mz.lnxyls.cn

[U108] JS：随机整数
来源：http://ds.hahajie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fe.yuntaijiaju.cn

[U109] JS：数组分组
来源：http://ao.colortex.cn

Object.groupBy(arr, x => x.type)
来源：http://oh.szsharing.cn

[U110] JS：数组分块
来源：http://yb.yuntaijiaju.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wo.szxytkj.cn

[U111] JS：对象转 Map
来源：http://st.huixiangedu.cn

new Map(Object.entries(obj))
来源：http://hy.lnxyls.cn

[U112] JS：字符串补位
来源：http://bp.521024.cn

"7".padStart(3, "0")
来源：http://or.jctech888.com.cn

[U113] JS：正则替换全部
来源：http://xe.shxzukj.cn

s.replaceAll("a", "b")
来源：http://ah.huanxung.cn

[U114] JS：JSON 深比较
来源：http://rn.yuexingan06.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://pk.huanxung.cn

[U115] JS：生成 UUID
来源：http://uf.nicolike.cn

crypto.randomUUID()
来源：http://em.szxytkj.cn

[U116] JS：类型检查（JSDoc）
来源：http://tb.haigaiapp.cn

/** @param {string} name */ function f(name) {}
来源：http://ol.jctech888.com.cn

[U117] JS：单元测试
来源：http://ca.szsharing.cn

npm i -D vitest;  npx vitest
来源：http://ra.521024.cn

[U118] JS：开发服务器
来源：http://ic.chemitech.net.cn

npm i -D vite;  npx vite
来源：http://oo.nicolike.cn


<!-- 参考信息 -->