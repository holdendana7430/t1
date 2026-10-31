代发 wailian999

[T27] Swift：错误处理
来源：http://wi.asd995.cn

do { try f() } catch { print(error) }
来源：http://pn.shxzskj.cn

[T28] Swift：枚举
来源：http://gs.hahajie.cn

enum Color { case red, green }
来源：http://sw.bjjhwx.cn

[T29] Swift：guard 提前返回
来源：http://lb.colortex.cn

guard let x = opt else { return }
来源：http://is.hnjuh.cn

[T30] Swift：协议
来源：http://ob.hahajie.cn

protocol Shape { func area() -> Double }
来源：http://zs.chemitech.net.cn

[T31] Lua：Hello World
来源：http://nk.newstarts.cn

print("Hello")
来源：http://vm.muxihuayi.cn

[T32] Lua：局部变量
来源：http://xl.bookmarksfly.cn

local a = 1
来源：http://gh.yuexingan06.cn

[T33] Lua：表（数组）
来源：http://iy.colortex.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://iv.jctech888.com.cn

[T34] Lua：遍历表
来源：http://xj.colortex.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://lf.szxytkj.cn

[T35] Lua：字典表
来源：http://qu.9csxet.cn

local d = { a = 1 };  d.b = 2
来源：http://mh.9csxet.cn

[T36] Lua：函数
来源：http://yu.lnxyls.cn

function add(a, b) return a + b end
来源：http://mb.shtwfgs.cn

[T37] Lua：字符串拼接
来源：http://vi.chemitech.net.cn

"a" .. "b"
来源：http://ia.shxzukj.cn

[T38] Lua：条件
来源：http://pa.colortex.cn

if x > 0 then print("正") end
来源：http://vg.wgjwhj.cn

[T39] Lua：模式匹配
来源：http://fi.shxzskj.cn

string.find(s, "%d+")
来源：http://rm.panjiajie.cn

[T40] Lua：元表
来源：http://gz.jianghongdianzi.cn

setmetatable({}, { __index = base })
来源：http://yc.9csxet.cn

[T41] Perl：Hello World
来源：http://rd.shxzskj.cn

print "Hello\n";
来源：http://ab.szxytkj.cn

[T42] Perl：变量类型
来源：http://ux.yuntaijiaju.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jg.wgjwhj.cn

[T43] Perl：字符串插值
来源：http://xw.huanxung.cn

"值: $a"
来源：http://ok.gzmigu.cn

[T44] Perl：条件
来源：http://tr.lnxyls.cn

if ($a > 0) { print "正"; }
来源：http://lz.szsharing.cn

[T45] Perl：数组遍历
来源：http://vx.shxzukj.cn

for my $x (@arr) { print $x; }
来源：http://iz.521024.cn

[T46] Perl：哈希操作
来源：http://yb.newstarts.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nk.nicolike.cn

[T47] Perl：正则捕获
来源：http://ou.shtwfgs.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://kb.shtwfgs.cn

[T48] Perl：正则替换
来源：http://hg.szsharing.cn

$s =~ s/old/new/g;
来源：http://mk.bookmarksfly.cn

[T49] Perl：函数
来源：http://zm.gzmigu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cd.hnjuh.cn

[T50] Perl：逐行读文件
来源：http://rq.nicolike.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://cb.yuexingan06.cn

while (my $line = <$fh>) { print $line; }
来源：http://dp.bjjhwx.cn

[T51] Scala：Hello World
来源：http://ly.jianghongdianzi.cn

println("Hello")
来源：http://ip.panjiajie.cn

[T52] Scala：变量
来源：http://oz.9csxet.cn

val a = 1;  var b = 2
来源：http://jc.asd995.cn

[T53] Scala：字符串插值
来源：http://pz.asd995.cn

s"值: $b"
来源：http://uv.newstarts.cn

[T54] Scala：集合映射
来源：http://tx.newstarts.cn

List(1, 2, 3).map(_ * 2)
来源：http://yu.huanxung.cn

[T55] Scala：集合过滤
来源：http://rd.jianghongdianzi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://zk.colortex.cn

[T56] Scala：样例类
来源：http://mx.newstarts.cn

case class User(name: String, age: Int)
来源：http://fw.bjjhwx.cn

[T57] Scala：模式匹配
来源：http://gv.shtwfgs.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://bd.szxytkj.cn

[T58] Scala：函数定义
来源：http://kf.gzmigu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://rc.gzmigu.cn

[T59] Scala：循环
来源：http://cm.huixiangedu.cn

for (i <- 1 to 10) println(i)
来源：http://ta.shxzskj.cn

[T60] Scala：折叠
来源：http://zt.nicolike.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tg.panjiajie.cn

================================================================================
来源：http://cb.9csxet.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ag.panjiajie.cn

================================================================================
来源：http://kw.huanxung.cn

[U01] Py：创建虚拟环境
来源：http://xu.szsharing.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ta.bjjhwx.cn

[U02] Py：导出 / 安装依赖
来源：http://ou.chemitech.net.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://aa.panjiajie.cn

[U03] Py：加载 .env 配置
来源：http://eg.shxzukj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://im.521024.cn

[U04] Py：变量调试打印
来源：http://cc.521024.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hf.521024.cn

[U05] Py：列表去重且保序
来源：http://ld.521024.cn

list(dict.fromkeys(arr))
来源：http://se.nszjky.cn

[U06] Py：合并两个字典
来源：http://bo.nicolike.cn

{**a, **b}
来源：http://gg.bookmarksfly.cn

[U07] Py：反转字典键值
来源：http://ao.bookmarksfly.cn

{v: k for k, v in d.items()}
来源：http://dt.shxzskj.cn

[U08] Py：展平二维列表
来源：http://ls.asd995.cn

[y for x in nested for y in x]
来源：http://xu.colortex.cn

[U09] Py：字典取最大值的键
来源：http://km.panjiajie.cn

max(d, key=d.get)
来源：http://yc.521024.cn

[U10] Py：按值排序字典
来源：http://jo.colortex.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nj.asd995.cn

[U11] Py：生成器表达式
来源：http://on.shtwfgs.cn

(x * 2 for x in arr)
来源：http://xj.wgjwhj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://tz.haigaiapp.cn

Counter(arr).most_common(3)
来源：http://oi.muxihuayi.cn

[U13] Py：固定长度队列
来源：http://tx.wgjwhj.cn

deque(maxlen=10)
来源：http://tx.wgjwhj.cn

[U14] Py：分组收集到列表
来源：http://wg.huanxung.cn

defaultdict(list)
来源：http://kd.muxihuayi.cn

[U15] Py：高精度计时
来源：http://pg.huanxung.cn

t = time.perf_counter()
来源：http://kc.colortex.cn

[U16] Py：命令行参数解析
来源：http://ii.haigaiapp.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qs.colortex.cn

[U17] Py：初始化日志
来源：http://ei.hnjuh.cn

logging.basicConfig(level=logging.INFO)
来源：http://vj.9csxet.cn

[U18] Py：预编译正则
来源：http://tz.521024.cn

pat = re.compile(r"\d+")
来源：http://oa.bjjhwx.cn

[U19] Py：正则替换带回调
来源：http://fp.huixinmuqiang.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xw.hahajie.cn

[U20] Py：缓存函数结果
来源：http://jm.bookmarksfly.cn

@functools.lru_cache(maxsize=None)
来源：http://gy.jianghongdianzi.cn

[U21] Py：自定义上下文管理器
来源：http://wv.szxytkj.cn

@contextlib.contextmanager
来源：http://ee.bookmarksfly.cn

[U22] Py：矩阵转置
来源：http://kd.521024.cn

list(zip(*m))
来源：http://mj.lnxyls.cn

[U23] Py：分块读取大文件
来源：http://rz.muxihuayi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tg.nicolike.cn

[U24] Py：路径操作
来源：http://vg.chemitech.net.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://af.nszjky.cn

[U25] Py：CSV 按字典读
来源：http://bp.yuntaijiaju.cn

csv.DictReader(f)
来源：http://wn.muxihuayi.cn

[U26] Py：并发下载
来源：http://nt.bjjhwx.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://eb.huixinmuqiang.cn

[U27] Py：异步 HTTP
来源：http://mq.wgjwhj.cn

aiohttp.ClientSession() 配合 async with
来源：http://yn.szsharing.cn

[U28] Py：类型别名
来源：http://mp.newstarts.cn

UserId = int
来源：http://tb.nszjky.cn

[U29] Py：属性校验
来源：http://jp.hnjuh.cn

@property 与 @x.setter 配合
来源：http://jx.huanxung.cn

[U30] Py：数据类
来源：http://nk.shtwfgs.cn

@dataclass(slots=True)
来源：http://qu.panjiajie.cn

[U31] Py：单测
来源：http://uy.hahajie.cn

python -m pytest -q
来源：http://pw.bjjhwx.cn

[U32] Py：代码格式化
来源：http://rp.bjjhwx.cn

ruff format . && ruff check --fix .
来源：http://fm.asd995.cn

[U33] Py：打包发布
来源：http://bi.bjjhwx.cn

python -m build  （依赖 pyproject.toml）
来源：http://of.nicolike.cn

[U34] Py：判断编码
来源：http://ht.bookmarksfly.cn

chardet.detect(raw)
来源：http://yx.szxytkj.cn

[U35] Py：发送邮件
来源：http://vl.yuntaijiaju.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bg.panjiajie.cn

[U36] Py：定时任务
来源：http://lr.nicolike.cn

schedule.every(10).minutes.do(job)
来源：http://ir.jianghongdianzi.cn

[U37] Py：读写 Excel
来源：http://an.bjjhwx.cn

pandas.read_excel / DataFrame.to_excel
来源：http://oc.huixiangedu.cn

[U38] Py：获取脚本所在目录
来源：http://sh.wgjwhj.cn

Path(__file__).resolve().parent
来源：http://ec.bookmarksfly.cn

[U39] Py：判断是否在交互环境
来源：http://zw.muxihuayi.cn

sys.stdout.isatty()
来源：http://pl.521024.cn

[U40] Py：打印到标准错误
来源：http://cj.yuntaijiaju.cn

print("err", file=sys.stderr)
来源：http://lc.colortex.cn

[U41] PHP：初始化 Composer 项目
来源：http://fi.shxzskj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://fv.huixinmuqiang.cn

[U42] PHP：PSR-4 自动加载
来源：http://ba.nszjky.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rn.haigaiapp.cn

[U43] PHP：声明命名空间
来源：http://za.colortex.cn

namespace App\Http;
来源：http://vu.muxihuayi.cn

[U44] PHP：开启严格类型
来源：http://dp.szsharing.cn

declare(strict_types=1);
来源：http://vm.huixiangedu.cn

[U45] PHP：类型声明与返回类型
来源：http://os.521024.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://vc.9csxet.cn

[U46] PHP：可空类型
来源：http://qz.hahajie.cn

?string $name = null
来源：http://fm.521024.cn

[U47] PHP：联合类型
来源：http://gr.shtwfgs.cn

int|string $id
来源：http://kf.bookmarksfly.cn

[U48] PHP：纯枚举
来源：http://zl.bjjhwx.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ze.hahajie.cn

[U49] PHP：只读属性
来源：http://fo.chemitech.net.cn

public readonly string $name
来源：http://vc.chemitech.net.cn

[U50] PHP：构造器属性提升
来源：http://hh.yuexingan06.cn

public function __construct(private int $id) {}
来源：http://nx.szxytkj.cn

[U51] PHP：数组解构
来源：http://rp.yuexingan06.cn

[$a, $b] = $arr;
来源：http://po.521024.cn

[U52] PHP：箭头函数
来源：http://cn.bjjhwx.cn

$double = fn($x) => $x * 2;
来源：http://xl.hnjuh.cn

[U53] PHP：空合并运算符
来源：http://lp.jctech888.com.cn

$v = $a ?? $b ?? "default";
来源：http://vo.shxzukj.cn

[U54] PHP：空安全调用
来源：http://rz.hnjuh.cn

$obj?->method()
来源：http://om.chemitech.net.cn

[U55] PHP：match 表达式
来源：http://do.shtwfgs.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yj.hahajie.cn

[U56] PHP：命名参数
来源：http://hw.yuexingan06.cn

f(a: 1, b: 2)
来源：http://ze.huanxung.cn

[U57] PHP：字符串插值
来源：http://cj.lnxyls.cn

"值: {$a}"
来源：http://ot.yuexingan06.cn

[U58] PHP：数组三件套
来源：http://lt.hahajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ox.huanxung.cn

[U59] PHP：自定义排序
来源：http://jo.huixiangedu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vf.bjjhwx.cn

[U60] PHP：JSON 编解码
来源：http://nq.521024.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hq.chemitech.net.cn

[U61] PHP：正则
来源：http://rq.shxzukj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://oe.shxzskj.cn

[U62] PHP：日期对象
来源：http://wt.yuexingan06.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://um.gzmigu.cn

[U63] PHP：文件读写
来源：http://pp.hnjuh.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ie.yuexingan06.cn

[U64] PHP：目录遍历
来源：http://rn.bookmarksfly.cn

glob("dir/*.php");  scandir("dir");
来源：http://pd.bookmarksfly.cn

[U65] PHP：会话
来源：http://fy.nszjky.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://dk.hahajie.cn

[U66] PHP：设置 Cookie
来源：http://kw.huanxung.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mr.nicolike.cn

[U67] PHP：处理文件上传
来源：http://ei.521024.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xb.hahajie.cn

[U68] PHP：PDO 连接
来源：http://mj.bookmarksfly.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cv.jianghongdianzi.cn

[U69] PHP：PDO 预处理
来源：http://oo.gzmigu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://de.hnjuh.cn

[U70] PHP：PDO 事务
来源：http://zo.colortex.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qj.szxytkj.cn

[U71] PHP：抛出异常
来源：http://xu.yuntaijiaju.cn

throw new RuntimeException("失败", 500);
来源：http://qt.huixinmuqiang.cn

[U72] PHP：写错误日志
来源：http://jg.gzmigu.cn

error_log("失败: " . $e->getMessage());
来源：http://gt.huixinmuqiang.cn

[U73] PHP：读取 ini 配置
来源：http://ub.szxytkj.cn

parse_ini_file("config.ini", true)
来源：http://hk.gzmigu.cn

[U74] PHP：读取环境变量
来源：http://mm.chemitech.net.cn

getenv("APP_ENV") ?: "production"
来源：http://bm.huixinmuqiang.cn

[U75] PHP：依赖注入
来源：http://iu.bjjhwx.cn

composer require psr/container
来源：http://en.szsharing.cn

[U76] PHP：简单路由
来源：http://bt.yuexingan06.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ab.szsharing.cn

[U77] PHP：模板渲染
来源：http://vs.yuntaijiaju.cn

composer require twig/twig
来源：http://cv.huixinmuqiang.cn

[U78] PHP：单元测试
来源：http://ae.jianghongdianzi.cn

composer require --dev phpunit/phpunit
来源：http://ji.521024.cn

[U79] PHP：静态分析
来源：http://jd.hnjuh.cn

composer require --dev phpstan/phpstan
来源：http://hc.nszjky.cn

[U80] PHP：代码规范修复
来源：http://ww.yuexingan06.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://fb.wgjwhj.cn

[U81] JS：初始化项目
来源：http://co.gzmigu.cn

npm init -y;  npm i express
来源：http://vs.jctech888.com.cn

[U82] JS：package.json 脚本
来源：http://sv.hnjuh.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ed.yuntaijiaju.cn

[U83] JS：ES Module 导入导出
来源：http://eh.chemitech.net.cn

export const a = 1;  import { a } from "./m.js";
来源：http://rs.hnjuh.cn

[U84] JS：CommonJS 写法
来源：http://ui.bjjhwx.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ml.shxzskj.cn

[U85] JS：可选链
来源：http://xm.panjiajie.cn

a?.b?.c
来源：http://ua.nicolike.cn

[U86] JS：空值合并
来源：http://hp.newstarts.cn

a ?? b
来源：http://ub.haigaiapp.cn

[U87] JS：解构默认值
来源：http://tj.newstarts.cn

const { a = 1, b = 2 } = obj;
来源：http://ed.chemitech.net.cn

[U88] JS：对象展开合并
来源：http://fw.yuntaijiaju.cn

{ ...a, ...b }
来源：http://ky.colortex.cn

[U89] JS：数组去重
来源：http://ji.hahajie.cn

[...new Set(arr)]
来源：http://de.jctech888.com.cn

[U90] JS：数字数组排序
来源：http://wo.szxytkj.cn

[...arr].sort((a, b) => a - b)
来源：http://rx.haigaiapp.cn

[U91] JS：对象键值遍历
来源：http://is.colortex.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bi.yuexingan06.cn

[U92] JS：深拷贝
来源：http://ja.chemitech.net.cn

structuredClone(obj)
来源：http://yy.newstarts.cn

[U93] JS：模板字符串
来源：http://qu.hnjuh.cn

`共 ${n} 条`
来源：http://qv.gzmigu.cn

[U94] JS：箭头函数
来源：http://wj.jctech888.com.cn

const double = x => x * 2;
来源：http://sa.hnjuh.cn

[U95] JS：Promise 包装
来源：http://cd.colortex.cn

new Promise((resolve, reject) => {})
来源：http://aj.szxytkj.cn

[U96] JS：async/await 与异常
来源：http://bo.colortex.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://am.asd995.cn

[U97] JS：并发请求
来源：http://gk.521024.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://hx.521024.cn

[U98] JS：fetch 带 JSON
来源：http://sw.521024.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ze.hahajie.cn

[U99] JS：事件监听
来源：http://zb.panjiajie.cn

el.addEventListener("click", e => {})
来源：http://jg.muxihuayi.cn

[U100] JS：DOM 查询
来源：http://br.newstarts.cn

document.querySelector(".item")
来源：http://it.521024.cn

[U101] JS：classList 操作
来源：http://mg.9csxet.cn

el.classList.toggle("active")
来源：http://ry.muxihuayi.cn

[U102] JS：本地存储
来源：http://gp.jianghongdianzi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://pb.huixiangedu.cn

[U103] JS：定时器
来源：http://rk.jianghongdianzi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nc.lnxyls.cn

[U104] JS：防抖
来源：http://uq.gzmigu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ly.jctech888.com.cn

[U105] JS：节流
来源：http://dt.muxihuayi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sy.szxytkj.cn

[U106] JS：日期格式化
来源：http://kg.colortex.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dh.yuntaijiaju.cn

[U107] JS：数字千分位
来源：http://pi.haigaiapp.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ki.shxzukj.cn

[U108] JS：随机整数
来源：http://dx.bookmarksfly.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ej.gzmigu.cn

[U109] JS：数组分组
来源：http://an.yuntaijiaju.cn

Object.groupBy(arr, x => x.type)
来源：http://xz.wgjwhj.cn

[U110] JS：数组分块
来源：http://mp.nicolike.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wc.jianghongdianzi.cn

[U111] JS：对象转 Map
来源：http://yt.newstarts.cn

new Map(Object.entries(obj))
来源：http://uj.yuntaijiaju.cn

[U112] JS：字符串补位
来源：http://fd.gzmigu.cn

"7".padStart(3, "0")
来源：http://kd.bookmarksfly.cn

[U113] JS：正则替换全部
来源：http://yv.huixiangedu.cn

s.replaceAll("a", "b")
来源：http://nv.bjjhwx.cn

[U114] JS：JSON 深比较
来源：http://tq.nicolike.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://wh.newstarts.cn


<!-- 参考信息 -->