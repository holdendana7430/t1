代发 wailian999

[T29] Swift：guard 提前返回
来源：http://mq.hahajie.cn

guard let x = opt else { return }
来源：http://xw.wgjwhj.cn

[T30] Swift：协议
来源：http://kh.panjiajie.cn

protocol Shape { func area() -> Double }
来源：http://bq.521024.cn

[T31] Lua：Hello World
来源：http://og.muxihuayi.cn

print("Hello")
来源：http://vr.colortex.cn

[T32] Lua：局部变量
来源：http://ay.wgjwhj.cn

local a = 1
来源：http://ak.nicolike.cn

[T33] Lua：表（数组）
来源：http://ha.521024.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://gc.wgjwhj.cn

[T34] Lua：遍历表
来源：http://hb.haigaiapp.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://hv.9csxet.cn

[T35] Lua：字典表
来源：http://zv.shtwfgs.cn

local d = { a = 1 };  d.b = 2
来源：http://pq.jctech888.com.cn

[T36] Lua：函数
来源：http://zp.muxihuayi.cn

function add(a, b) return a + b end
来源：http://sb.bookmarksfly.cn

[T37] Lua：字符串拼接
来源：http://qi.nicolike.cn

"a" .. "b"
来源：http://jg.shxzukj.cn

[T38] Lua：条件
来源：http://jg.9csxet.cn

if x > 0 then print("正") end
来源：http://tu.huixiangedu.cn

[T39] Lua：模式匹配
来源：http://zp.colortex.cn

string.find(s, "%d+")
来源：http://tw.muxihuayi.cn

[T40] Lua：元表
来源：http://dn.szsharing.cn

setmetatable({}, { __index = base })
来源：http://ky.newstarts.cn

[T41] Perl：Hello World
来源：http://gj.nszjky.cn

print "Hello\n";
来源：http://eo.shxzskj.cn

[T42] Perl：变量类型
来源：http://dr.gzmigu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zh.hahajie.cn

[T43] Perl：字符串插值
来源：http://pg.wgjwhj.cn

"值: $a"
来源：http://wn.jctech888.com.cn

[T44] Perl：条件
来源：http://fg.gzmigu.cn

if ($a > 0) { print "正"; }
来源：http://ap.521024.cn

[T45] Perl：数组遍历
来源：http://ih.gzmigu.cn

for my $x (@arr) { print $x; }
来源：http://ts.colortex.cn

[T46] Perl：哈希操作
来源：http://cp.haigaiapp.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://la.9csxet.cn

[T47] Perl：正则捕获
来源：http://br.newstarts.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://cc.muxihuayi.cn

[T48] Perl：正则替换
来源：http://nm.yuexingan06.cn

$s =~ s/old/new/g;
来源：http://kv.huixinmuqiang.cn

[T49] Perl：函数
来源：http://dv.bookmarksfly.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ah.asd995.cn

[T50] Perl：逐行读文件
来源：http://cc.szsharing.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://aq.shxzukj.cn

while (my $line = <$fh>) { print $line; }
来源：http://ki.hnjuh.cn

[T51] Scala：Hello World
来源：http://ux.newstarts.cn

println("Hello")
来源：http://fe.huixiangedu.cn

[T52] Scala：变量
来源：http://rc.panjiajie.cn

val a = 1;  var b = 2
来源：http://xp.shtwfgs.cn

[T53] Scala：字符串插值
来源：http://bb.asd995.cn

s"值: $b"
来源：http://rm.bjjhwx.cn

[T54] Scala：集合映射
来源：http://di.bjjhwx.cn

List(1, 2, 3).map(_ * 2)
来源：http://bh.panjiajie.cn

[T55] Scala：集合过滤
来源：http://ef.haigaiapp.cn

List(1, 2, 3).filter(_ > 1)
来源：http://yo.panjiajie.cn

[T56] Scala：样例类
来源：http://vv.szxytkj.cn

case class User(name: String, age: Int)
来源：http://ro.9csxet.cn

[T57] Scala：模式匹配
来源：http://sx.chemitech.net.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://sz.yuntaijiaju.cn

[T58] Scala：函数定义
来源：http://nl.nszjky.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ia.haigaiapp.cn

[T59] Scala：循环
来源：http://pu.szxytkj.cn

for (i <- 1 to 10) println(i)
来源：http://sg.shxzskj.cn

[T60] Scala：折叠
来源：http://yt.huixiangedu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vo.huanxung.cn

================================================================================
来源：http://rr.shxzskj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mx.jctech888.com.cn

================================================================================
来源：http://wo.huixinmuqiang.cn

[U01] Py：创建虚拟环境
来源：http://pk.wgjwhj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zk.huanxung.cn

[U02] Py：导出 / 安装依赖
来源：http://fn.gzmigu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ig.shxzukj.cn

[U03] Py：加载 .env 配置
来源：http://sw.shtwfgs.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://kb.shxzskj.cn

[U04] Py：变量调试打印
来源：http://vd.newstarts.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://aq.szsharing.cn

[U05] Py：列表去重且保序
来源：http://ab.9csxet.cn

list(dict.fromkeys(arr))
来源：http://kj.bjjhwx.cn

[U06] Py：合并两个字典
来源：http://hh.huanxung.cn

{**a, **b}
来源：http://tq.nszjky.cn

[U07] Py：反转字典键值
来源：http://ll.yuexingan06.cn

{v: k for k, v in d.items()}
来源：http://kv.huixiangedu.cn

[U08] Py：展平二维列表
来源：http://lt.521024.cn

[y for x in nested for y in x]
来源：http://au.colortex.cn

[U09] Py：字典取最大值的键
来源：http://cl.jianghongdianzi.cn

max(d, key=d.get)
来源：http://ic.yuntaijiaju.cn

[U10] Py：按值排序字典
来源：http://ej.huanxung.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wa.hahajie.cn

[U11] Py：生成器表达式
来源：http://va.yuntaijiaju.cn

(x * 2 for x in arr)
来源：http://ak.huixiangedu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://kz.wgjwhj.cn

Counter(arr).most_common(3)
来源：http://us.521024.cn

[U13] Py：固定长度队列
来源：http://dv.panjiajie.cn

deque(maxlen=10)
来源：http://ef.shxzskj.cn

[U14] Py：分组收集到列表
来源：http://nb.muxihuayi.cn

defaultdict(list)
来源：http://eb.szsharing.cn

[U15] Py：高精度计时
来源：http://rv.hnjuh.cn

t = time.perf_counter()
来源：http://ce.521024.cn

[U16] Py：命令行参数解析
来源：http://ut.bookmarksfly.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ui.haigaiapp.cn

[U17] Py：初始化日志
来源：http://yf.jianghongdianzi.cn

logging.basicConfig(level=logging.INFO)
来源：http://ch.yuntaijiaju.cn

[U18] Py：预编译正则
来源：http://rm.shtwfgs.cn

pat = re.compile(r"\d+")
来源：http://ng.hnjuh.cn

[U19] Py：正则替换带回调
来源：http://tc.huanxung.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gc.colortex.cn

[U20] Py：缓存函数结果
来源：http://nf.9csxet.cn

@functools.lru_cache(maxsize=None)
来源：http://cq.jctech888.com.cn

[U21] Py：自定义上下文管理器
来源：http://gu.huixiangedu.cn

@contextlib.contextmanager
来源：http://do.szsharing.cn

[U22] Py：矩阵转置
来源：http://vb.nszjky.cn

list(zip(*m))
来源：http://fv.nszjky.cn

[U23] Py：分块读取大文件
来源：http://lw.yuntaijiaju.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ez.nszjky.cn

[U24] Py：路径操作
来源：http://ba.huixinmuqiang.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ca.yuntaijiaju.cn

[U25] Py：CSV 按字典读
来源：http://xs.haigaiapp.cn

csv.DictReader(f)
来源：http://nq.9csxet.cn

[U26] Py：并发下载
来源：http://jv.colortex.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qr.shtwfgs.cn

[U27] Py：异步 HTTP
来源：http://ic.wgjwhj.cn

aiohttp.ClientSession() 配合 async with
来源：http://gx.huixiangedu.cn

[U28] Py：类型别名
来源：http://tg.hnjuh.cn

UserId = int
来源：http://vn.colortex.cn

[U29] Py：属性校验
来源：http://iu.wgjwhj.cn

@property 与 @x.setter 配合
来源：http://kj.hnjuh.cn

[U30] Py：数据类
来源：http://cg.shxzskj.cn

@dataclass(slots=True)
来源：http://pt.9csxet.cn

[U31] Py：单测
来源：http://ry.shtwfgs.cn

python -m pytest -q
来源：http://zz.nszjky.cn

[U32] Py：代码格式化
来源：http://jj.521024.cn

ruff format . && ruff check --fix .
来源：http://zd.bookmarksfly.cn

[U33] Py：打包发布
来源：http://fb.yuntaijiaju.cn

python -m build  （依赖 pyproject.toml）
来源：http://fp.jianghongdianzi.cn

[U34] Py：判断编码
来源：http://lj.wgjwhj.cn

chardet.detect(raw)
来源：http://vy.haigaiapp.cn

[U35] Py：发送邮件
来源：http://uw.gzmigu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mj.nszjky.cn

[U36] Py：定时任务
来源：http://ya.newstarts.cn

schedule.every(10).minutes.do(job)
来源：http://pb.shxzskj.cn

[U37] Py：读写 Excel
来源：http://dz.shtwfgs.cn

pandas.read_excel / DataFrame.to_excel
来源：http://gs.huixiangedu.cn

[U38] Py：获取脚本所在目录
来源：http://my.colortex.cn

Path(__file__).resolve().parent
来源：http://nf.newstarts.cn

[U39] Py：判断是否在交互环境
来源：http://ss.szsharing.cn

sys.stdout.isatty()
来源：http://xm.shxzukj.cn

[U40] Py：打印到标准错误
来源：http://mn.wgjwhj.cn

print("err", file=sys.stderr)
来源：http://un.jctech888.com.cn

[U41] PHP：初始化 Composer 项目
来源：http://wn.muxihuayi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://to.lnxyls.cn

[U42] PHP：PSR-4 自动加载
来源：http://tf.shxzskj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fu.hnjuh.cn

[U43] PHP：声明命名空间
来源：http://ka.jctech888.com.cn

namespace App\Http;
来源：http://oq.shtwfgs.cn

[U44] PHP：开启严格类型
来源：http://dp.shxzukj.cn

declare(strict_types=1);
来源：http://ao.shxzukj.cn

[U45] PHP：类型声明与返回类型
来源：http://rb.muxihuayi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://mj.szsharing.cn

[U46] PHP：可空类型
来源：http://rr.szxytkj.cn

?string $name = null
来源：http://ks.yuntaijiaju.cn

[U47] PHP：联合类型
来源：http://ll.hnjuh.cn

int|string $id
来源：http://qx.panjiajie.cn

[U48] PHP：纯枚举
来源：http://ur.jctech888.com.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mi.haigaiapp.cn

[U49] PHP：只读属性
来源：http://rx.gzmigu.cn

public readonly string $name
来源：http://zq.huixinmuqiang.cn

[U50] PHP：构造器属性提升
来源：http://ud.nszjky.cn

public function __construct(private int $id) {}
来源：http://jy.panjiajie.cn

[U51] PHP：数组解构
来源：http://hr.hahajie.cn

[$a, $b] = $arr;
来源：http://kk.szsharing.cn

[U52] PHP：箭头函数
来源：http://ov.shxzskj.cn

$double = fn($x) => $x * 2;
来源：http://sq.shxzskj.cn

[U53] PHP：空合并运算符
来源：http://rc.shxzukj.cn

$v = $a ?? $b ?? "default";
来源：http://cr.521024.cn

[U54] PHP：空安全调用
来源：http://ip.9csxet.cn

$obj?->method()
来源：http://re.shxzskj.cn

[U55] PHP：match 表达式
来源：http://bn.szsharing.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hh.szsharing.cn

[U56] PHP：命名参数
来源：http://fm.hnjuh.cn

f(a: 1, b: 2)
来源：http://bc.newstarts.cn

[U57] PHP：字符串插值
来源：http://hh.yuexingan06.cn

"值: {$a}"
来源：http://zu.haigaiapp.cn

[U58] PHP：数组三件套
来源：http://rr.bookmarksfly.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ws.newstarts.cn

[U59] PHP：自定义排序
来源：http://li.bjjhwx.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dx.yuntaijiaju.cn

[U60] PHP：JSON 编解码
来源：http://it.shxzukj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ml.hnjuh.cn

[U61] PHP：正则
来源：http://at.shxzskj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kq.panjiajie.cn

[U62] PHP：日期对象
来源：http://pp.9csxet.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ud.lnxyls.cn

[U63] PHP：文件读写
来源：http://my.nicolike.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dx.bjjhwx.cn

[U64] PHP：目录遍历
来源：http://em.bjjhwx.cn

glob("dir/*.php");  scandir("dir");
来源：http://td.521024.cn

[U65] PHP：会话
来源：http://ou.jianghongdianzi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ea.jianghongdianzi.cn

[U66] PHP：设置 Cookie
来源：http://cy.yuexingan06.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bx.colortex.cn

[U67] PHP：处理文件上传
来源：http://kq.wgjwhj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mc.panjiajie.cn

[U68] PHP：PDO 连接
来源：http://kt.huanxung.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lv.jctech888.com.cn

[U69] PHP：PDO 预处理
来源：http://ui.muxihuayi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wb.muxihuayi.cn

[U70] PHP：PDO 事务
来源：http://mp.shtwfgs.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mk.hnjuh.cn

[U71] PHP：抛出异常
来源：http://ic.9csxet.cn

throw new RuntimeException("失败", 500);
来源：http://qs.hahajie.cn

[U72] PHP：写错误日志
来源：http://fj.shtwfgs.cn

error_log("失败: " . $e->getMessage());
来源：http://cr.nszjky.cn

[U73] PHP：读取 ini 配置
来源：http://wq.shxzukj.cn

parse_ini_file("config.ini", true)
来源：http://rx.yuntaijiaju.cn

[U74] PHP：读取环境变量
来源：http://ts.9csxet.cn

getenv("APP_ENV") ?: "production"
来源：http://qa.panjiajie.cn

[U75] PHP：依赖注入
来源：http://so.hnjuh.cn

composer require psr/container
来源：http://kx.shxzukj.cn

[U76] PHP：简单路由
来源：http://xg.yuntaijiaju.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yc.yuexingan06.cn

[U77] PHP：模板渲染
来源：http://hw.521024.cn

composer require twig/twig
来源：http://xf.panjiajie.cn

[U78] PHP：单元测试
来源：http://uq.shtwfgs.cn

composer require --dev phpunit/phpunit
来源：http://ky.bjjhwx.cn

[U79] PHP：静态分析
来源：http://ki.shxzskj.cn

composer require --dev phpstan/phpstan
来源：http://tq.bjjhwx.cn

[U80] PHP：代码规范修复
来源：http://cf.jctech888.com.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://uo.muxihuayi.cn

[U81] JS：初始化项目
来源：http://hw.gzmigu.cn

npm init -y;  npm i express
来源：http://gj.bjjhwx.cn

[U82] JS：package.json 脚本
来源：http://my.haigaiapp.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://my.yuntaijiaju.cn

[U83] JS：ES Module 导入导出
来源：http://vg.muxihuayi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://bi.szsharing.cn

[U84] JS：CommonJS 写法
来源：http://dr.asd995.cn

module.exports = { a };  const { a } = require("./m");
来源：http://cr.shtwfgs.cn

[U85] JS：可选链
来源：http://ox.szxytkj.cn

a?.b?.c
来源：http://or.yuntaijiaju.cn

[U86] JS：空值合并
来源：http://ah.yuntaijiaju.cn

a ?? b
来源：http://oa.bookmarksfly.cn

[U87] JS：解构默认值
来源：http://bq.bjjhwx.cn

const { a = 1, b = 2 } = obj;
来源：http://ha.lnxyls.cn

[U88] JS：对象展开合并
来源：http://vw.newstarts.cn

{ ...a, ...b }
来源：http://mo.hahajie.cn

[U89] JS：数组去重
来源：http://rr.nicolike.cn

[...new Set(arr)]
来源：http://wq.chemitech.net.cn

[U90] JS：数字数组排序
来源：http://rt.9csxet.cn

[...arr].sort((a, b) => a - b)
来源：http://kb.haigaiapp.cn

[U91] JS：对象键值遍历
来源：http://gn.panjiajie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ss.bjjhwx.cn

[U92] JS：深拷贝
来源：http://lh.shxzukj.cn

structuredClone(obj)
来源：http://xr.haigaiapp.cn

[U93] JS：模板字符串
来源：http://gh.asd995.cn

`共 ${n} 条`
来源：http://we.szxytkj.cn

[U94] JS：箭头函数
来源：http://bm.bjjhwx.cn

const double = x => x * 2;
来源：http://ha.hnjuh.cn

[U95] JS：Promise 包装
来源：http://zo.colortex.cn

new Promise((resolve, reject) => {})
来源：http://dy.yuntaijiaju.cn

[U96] JS：async/await 与异常
来源：http://yy.jctech888.com.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cs.jianghongdianzi.cn

[U97] JS：并发请求
来源：http://zc.9csxet.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.haigaiapp.cn

[U98] JS：fetch 带 JSON
来源：http://bx.colortex.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cf.huixinmuqiang.cn

[U99] JS：事件监听
来源：http://si.nicolike.cn

el.addEventListener("click", e => {})
来源：http://ip.wgjwhj.cn

[U100] JS：DOM 查询
来源：http://nq.huixiangedu.cn

document.querySelector(".item")
来源：http://lw.asd995.cn

[U101] JS：classList 操作
来源：http://lj.lnxyls.cn

el.classList.toggle("active")
来源：http://hn.colortex.cn

[U102] JS：本地存储
来源：http://jk.nicolike.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://by.asd995.cn

[U103] JS：定时器
来源：http://rl.nicolike.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://eg.muxihuayi.cn

[U104] JS：防抖
来源：http://cx.gzmigu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gb.9csxet.cn

[U105] JS：节流
来源：http://jn.jianghongdianzi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sk.asd995.cn

[U106] JS：日期格式化
来源：http://av.nszjky.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bm.huixiangedu.cn

[U107] JS：数字千分位
来源：http://pa.huanxung.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sn.nszjky.cn

[U108] JS：随机整数
来源：http://oj.colortex.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ki.newstarts.cn

[U109] JS：数组分组
来源：http://vj.asd995.cn

Object.groupBy(arr, x => x.type)
来源：http://tb.szxytkj.cn

[U110] JS：数组分块
来源：http://fs.newstarts.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lw.muxihuayi.cn

[U111] JS：对象转 Map
来源：http://cl.lnxyls.cn

new Map(Object.entries(obj))
来源：http://bf.bjjhwx.cn

[U112] JS：字符串补位
来源：http://nf.huanxung.cn

"7".padStart(3, "0")
来源：http://wf.lnxyls.cn

[U113] JS：正则替换全部
来源：http://wk.panjiajie.cn

s.replaceAll("a", "b")
来源：http://dq.jctech888.com.cn

[U114] JS：JSON 深比较
来源：http://vq.jctech888.com.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://yi.chemitech.net.cn

[U115] JS：生成 UUID
来源：http://zo.chemitech.net.cn

crypto.randomUUID()
来源：http://fl.asd995.cn

[U116] JS：类型检查（JSDoc）
来源：http://wn.521024.cn

/** @param {string} name */ function f(name) {}
来源：http://qf.lnxyls.cn


<!-- 参考信息 -->