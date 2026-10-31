代发 wailian999

[T27] Swift：错误处理
来源：http://ew.yuexingan06.cn

do { try f() } catch { print(error) }
来源：http://jv.colortex.cn

[T28] Swift：枚举
来源：http://ew.szsharing.cn

enum Color { case red, green }
来源：http://jp.yuntaijiaju.cn

[T29] Swift：guard 提前返回
来源：http://ge.hahajie.cn

guard let x = opt else { return }
来源：http://om.yuexingan06.cn

[T30] Swift：协议
来源：http://kq.9csxet.cn

protocol Shape { func area() -> Double }
来源：http://ah.9csxet.cn

[T31] Lua：Hello World
来源：http://dg.shtwfgs.cn

print("Hello")
来源：http://tf.muxihuayi.cn

[T32] Lua：局部变量
来源：http://pv.hahajie.cn

local a = 1
来源：http://dt.jianghongdianzi.cn

[T33] Lua：表（数组）
来源：http://bg.gzmigu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://mq.521024.cn

[T34] Lua：遍历表
来源：http://ca.shxzukj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ze.bjjhwx.cn

[T35] Lua：字典表
来源：http://kp.wgjwhj.cn

local d = { a = 1 };  d.b = 2
来源：http://lh.asd995.cn

[T36] Lua：函数
来源：http://wa.asd995.cn

function add(a, b) return a + b end
来源：http://ir.jctech888.com.cn

[T37] Lua：字符串拼接
来源：http://nv.521024.cn

"a" .. "b"
来源：http://ee.chemitech.net.cn

[T38] Lua：条件
来源：http://pp.jctech888.com.cn

if x > 0 then print("正") end
来源：http://fz.shxzskj.cn

[T39] Lua：模式匹配
来源：http://yv.lnxyls.cn

string.find(s, "%d+")
来源：http://zs.wgjwhj.cn

[T40] Lua：元表
来源：http://tj.shxzskj.cn

setmetatable({}, { __index = base })
来源：http://ls.panjiajie.cn

[T41] Perl：Hello World
来源：http://ad.gzmigu.cn

print "Hello\n";
来源：http://si.yuexingan06.cn

[T42] Perl：变量类型
来源：http://tz.newstarts.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tj.jianghongdianzi.cn

[T43] Perl：字符串插值
来源：http://pd.szsharing.cn

"值: $a"
来源：http://kg.hnjuh.cn

[T44] Perl：条件
来源：http://ml.shxzukj.cn

if ($a > 0) { print "正"; }
来源：http://hx.9csxet.cn

[T45] Perl：数组遍历
来源：http://ft.huixiangedu.cn

for my $x (@arr) { print $x; }
来源：http://dt.yuntaijiaju.cn

[T46] Perl：哈希操作
来源：http://cp.nicolike.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ob.nszjky.cn

[T47] Perl：正则捕获
来源：http://wt.huixinmuqiang.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ue.muxihuayi.cn

[T48] Perl：正则替换
来源：http://ls.hnjuh.cn

$s =~ s/old/new/g;
来源：http://zx.jianghongdianzi.cn

[T49] Perl：函数
来源：http://xb.hnjuh.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ue.shxzskj.cn

[T50] Perl：逐行读文件
来源：http://dr.gzmigu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://tj.shtwfgs.cn

while (my $line = <$fh>) { print $line; }
来源：http://de.yuntaijiaju.cn

[T51] Scala：Hello World
来源：http://dv.jctech888.com.cn

println("Hello")
来源：http://fo.huixinmuqiang.cn

[T52] Scala：变量
来源：http://cr.yuntaijiaju.cn

val a = 1;  var b = 2
来源：http://gy.huixinmuqiang.cn

[T53] Scala：字符串插值
来源：http://eu.hnjuh.cn

s"值: $b"
来源：http://bz.bjjhwx.cn

[T54] Scala：集合映射
来源：http://nq.bookmarksfly.cn

List(1, 2, 3).map(_ * 2)
来源：http://sv.shxzskj.cn

[T55] Scala：集合过滤
来源：http://zl.yuexingan06.cn

List(1, 2, 3).filter(_ > 1)
来源：http://hi.hahajie.cn

[T56] Scala：样例类
来源：http://td.yuexingan06.cn

case class User(name: String, age: Int)
来源：http://qv.huanxung.cn

[T57] Scala：模式匹配
来源：http://cw.lnxyls.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://dr.jctech888.com.cn

[T58] Scala：函数定义
来源：http://ip.hnjuh.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gh.muxihuayi.cn

[T59] Scala：循环
来源：http://tg.colortex.cn

for (i <- 1 to 10) println(i)
来源：http://sn.szsharing.cn

[T60] Scala：折叠
来源：http://os.huixinmuqiang.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qp.bookmarksfly.cn

================================================================================
来源：http://sv.colortex.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zu.panjiajie.cn

================================================================================
来源：http://hg.bjjhwx.cn

[U01] Py：创建虚拟环境
来源：http://xm.chemitech.net.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wx.bookmarksfly.cn

[U02] Py：导出 / 安装依赖
来源：http://cp.haigaiapp.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ex.nszjky.cn

[U03] Py：加载 .env 配置
来源：http://ab.hahajie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zc.bookmarksfly.cn

[U04] Py：变量调试打印
来源：http://fz.bookmarksfly.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nh.9csxet.cn

[U05] Py：列表去重且保序
来源：http://gm.jctech888.com.cn

list(dict.fromkeys(arr))
来源：http://wx.jctech888.com.cn

[U06] Py：合并两个字典
来源：http://fi.muxihuayi.cn

{**a, **b}
来源：http://yx.newstarts.cn

[U07] Py：反转字典键值
来源：http://yi.huixinmuqiang.cn

{v: k for k, v in d.items()}
来源：http://sf.shtwfgs.cn

[U08] Py：展平二维列表
来源：http://zo.jianghongdianzi.cn

[y for x in nested for y in x]
来源：http://qu.huixinmuqiang.cn

[U09] Py：字典取最大值的键
来源：http://cs.huixiangedu.cn

max(d, key=d.get)
来源：http://ld.nszjky.cn

[U10] Py：按值排序字典
来源：http://ld.chemitech.net.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ql.9csxet.cn

[U11] Py：生成器表达式
来源：http://xt.hahajie.cn

(x * 2 for x in arr)
来源：http://gn.lnxyls.cn

[U12] Py：取出现最多的 3 个元素
来源：http://dl.lnxyls.cn

Counter(arr).most_common(3)
来源：http://ou.nicolike.cn

[U13] Py：固定长度队列
来源：http://kf.newstarts.cn

deque(maxlen=10)
来源：http://uw.panjiajie.cn

[U14] Py：分组收集到列表
来源：http://xv.shxzukj.cn

defaultdict(list)
来源：http://pk.shxzukj.cn

[U15] Py：高精度计时
来源：http://lo.huixinmuqiang.cn

t = time.perf_counter()
来源：http://qd.9csxet.cn

[U16] Py：命令行参数解析
来源：http://vy.haigaiapp.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zj.bookmarksfly.cn

[U17] Py：初始化日志
来源：http://cj.gzmigu.cn

logging.basicConfig(level=logging.INFO)
来源：http://gu.haigaiapp.cn

[U18] Py：预编译正则
来源：http://gs.huixinmuqiang.cn

pat = re.compile(r"\d+")
来源：http://bs.huixiangedu.cn

[U19] Py：正则替换带回调
来源：http://xo.hahajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nc.nszjky.cn

[U20] Py：缓存函数结果
来源：http://uv.shtwfgs.cn

@functools.lru_cache(maxsize=None)
来源：http://sn.huixiangedu.cn

[U21] Py：自定义上下文管理器
来源：http://jg.wgjwhj.cn

@contextlib.contextmanager
来源：http://sr.jianghongdianzi.cn

[U22] Py：矩阵转置
来源：http://ry.szsharing.cn

list(zip(*m))
来源：http://sl.szsharing.cn

[U23] Py：分块读取大文件
来源：http://iz.chemitech.net.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rm.szsharing.cn

[U24] Py：路径操作
来源：http://ha.asd995.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wt.huanxung.cn

[U25] Py：CSV 按字典读
来源：http://rp.shxzskj.cn

csv.DictReader(f)
来源：http://vi.szxytkj.cn

[U26] Py：并发下载
来源：http://pg.shxzukj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ww.hahajie.cn

[U27] Py：异步 HTTP
来源：http://ef.bjjhwx.cn

aiohttp.ClientSession() 配合 async with
来源：http://kw.9csxet.cn

[U28] Py：类型别名
来源：http://dh.jctech888.com.cn

UserId = int
来源：http://jy.asd995.cn

[U29] Py：属性校验
来源：http://ph.521024.cn

@property 与 @x.setter 配合
来源：http://pr.newstarts.cn

[U30] Py：数据类
来源：http://bl.nicolike.cn

@dataclass(slots=True)
来源：http://yn.huixiangedu.cn

[U31] Py：单测
来源：http://fl.lnxyls.cn

python -m pytest -q
来源：http://xt.nicolike.cn

[U32] Py：代码格式化
来源：http://hz.9csxet.cn

ruff format . && ruff check --fix .
来源：http://it.jctech888.com.cn

[U33] Py：打包发布
来源：http://jo.gzmigu.cn

python -m build  （依赖 pyproject.toml）
来源：http://vo.hahajie.cn

[U34] Py：判断编码
来源：http://yj.jctech888.com.cn

chardet.detect(raw)
来源：http://ao.shxzukj.cn

[U35] Py：发送邮件
来源：http://im.szsharing.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nd.asd995.cn

[U36] Py：定时任务
来源：http://us.yuntaijiaju.cn

schedule.every(10).minutes.do(job)
来源：http://lj.jctech888.com.cn

[U37] Py：读写 Excel
来源：http://cy.gzmigu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://go.haigaiapp.cn

[U38] Py：获取脚本所在目录
来源：http://hd.jctech888.com.cn

Path(__file__).resolve().parent
来源：http://na.haigaiapp.cn

[U39] Py：判断是否在交互环境
来源：http://ah.newstarts.cn

sys.stdout.isatty()
来源：http://vz.colortex.cn

[U40] Py：打印到标准错误
来源：http://vs.yuntaijiaju.cn

print("err", file=sys.stderr)
来源：http://nu.haigaiapp.cn

[U41] PHP：初始化 Composer 项目
来源：http://pt.newstarts.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zk.huanxung.cn

[U42] PHP：PSR-4 自动加载
来源：http://tv.nicolike.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sf.muxihuayi.cn

[U43] PHP：声明命名空间
来源：http://qn.colortex.cn

namespace App\Http;
来源：http://us.shxzukj.cn

[U44] PHP：开启严格类型
来源：http://gk.shtwfgs.cn

declare(strict_types=1);
来源：http://mi.haigaiapp.cn

[U45] PHP：类型声明与返回类型
来源：http://vr.hahajie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://se.jctech888.com.cn

[U46] PHP：可空类型
来源：http://yx.muxihuayi.cn

?string $name = null
来源：http://pi.nszjky.cn

[U47] PHP：联合类型
来源：http://zh.newstarts.cn

int|string $id
来源：http://my.shxzukj.cn

[U48] PHP：纯枚举
来源：http://xq.lnxyls.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vq.jctech888.com.cn

[U49] PHP：只读属性
来源：http://py.panjiajie.cn

public readonly string $name
来源：http://hp.gzmigu.cn

[U50] PHP：构造器属性提升
来源：http://iy.yuexingan06.cn

public function __construct(private int $id) {}
来源：http://kj.huixinmuqiang.cn

[U51] PHP：数组解构
来源：http://fi.nszjky.cn

[$a, $b] = $arr;
来源：http://aw.gzmigu.cn

[U52] PHP：箭头函数
来源：http://qr.shxzskj.cn

$double = fn($x) => $x * 2;
来源：http://wo.hnjuh.cn

[U53] PHP：空合并运算符
来源：http://hc.bookmarksfly.cn

$v = $a ?? $b ?? "default";
来源：http://fj.huanxung.cn

[U54] PHP：空安全调用
来源：http://np.bjjhwx.cn

$obj?->method()
来源：http://qs.9csxet.cn

[U55] PHP：match 表达式
来源：http://xj.newstarts.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jy.haigaiapp.cn

[U56] PHP：命名参数
来源：http://qm.colortex.cn

f(a: 1, b: 2)
来源：http://rl.wgjwhj.cn

[U57] PHP：字符串插值
来源：http://fa.huanxung.cn

"值: {$a}"
来源：http://xu.asd995.cn

[U58] PHP：数组三件套
来源：http://wh.huanxung.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rc.asd995.cn

[U59] PHP：自定义排序
来源：http://cq.shtwfgs.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uz.szsharing.cn

[U60] PHP：JSON 编解码
来源：http://yh.chemitech.net.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://td.shxzskj.cn

[U61] PHP：正则
来源：http://wf.huixinmuqiang.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qm.hahajie.cn

[U62] PHP：日期对象
来源：http://am.shtwfgs.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wl.newstarts.cn

[U63] PHP：文件读写
来源：http://qz.shxzskj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wg.huixiangedu.cn

[U64] PHP：目录遍历
来源：http://bq.lnxyls.cn

glob("dir/*.php");  scandir("dir");
来源：http://rs.lnxyls.cn

[U65] PHP：会话
来源：http://zr.panjiajie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ro.huixinmuqiang.cn

[U66] PHP：设置 Cookie
来源：http://lt.yuntaijiaju.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lj.hahajie.cn

[U67] PHP：处理文件上传
来源：http://eo.bookmarksfly.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mz.shtwfgs.cn

[U68] PHP：PDO 连接
来源：http://ps.panjiajie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qp.shtwfgs.cn

[U69] PHP：PDO 预处理
来源：http://sp.lnxyls.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bb.lnxyls.cn

[U70] PHP：PDO 事务
来源：http://rm.jctech888.com.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vq.hahajie.cn

[U71] PHP：抛出异常
来源：http://xd.521024.cn

throw new RuntimeException("失败", 500);
来源：http://rj.yuntaijiaju.cn

[U72] PHP：写错误日志
来源：http://cn.newstarts.cn

error_log("失败: " . $e->getMessage());
来源：http://xk.huixinmuqiang.cn

[U73] PHP：读取 ini 配置
来源：http://xq.hnjuh.cn

parse_ini_file("config.ini", true)
来源：http://ko.huixinmuqiang.cn

[U74] PHP：读取环境变量
来源：http://ag.shtwfgs.cn

getenv("APP_ENV") ?: "production"
来源：http://lz.shxzskj.cn

[U75] PHP：依赖注入
来源：http://ce.yuexingan06.cn

composer require psr/container
来源：http://uk.9csxet.cn

[U76] PHP：简单路由
来源：http://za.colortex.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yb.jianghongdianzi.cn

[U77] PHP：模板渲染
来源：http://td.muxihuayi.cn

composer require twig/twig
来源：http://sc.gzmigu.cn

[U78] PHP：单元测试
来源：http://pu.huixinmuqiang.cn

composer require --dev phpunit/phpunit
来源：http://bj.colortex.cn

[U79] PHP：静态分析
来源：http://ep.yuexingan06.cn

composer require --dev phpstan/phpstan
来源：http://qu.wgjwhj.cn

[U80] PHP：代码规范修复
来源：http://mk.panjiajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://rh.yuexingan06.cn

[U81] JS：初始化项目
来源：http://wl.huixiangedu.cn

npm init -y;  npm i express
来源：http://rh.nszjky.cn

[U82] JS：package.json 脚本
来源：http://le.wgjwhj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fc.muxihuayi.cn

[U83] JS：ES Module 导入导出
来源：http://eh.hnjuh.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ii.szxytkj.cn

[U84] JS：CommonJS 写法
来源：http://bx.lnxyls.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ei.asd995.cn

[U85] JS：可选链
来源：http://oz.hnjuh.cn

a?.b?.c
来源：http://fg.shxzukj.cn

[U86] JS：空值合并
来源：http://dk.szsharing.cn

a ?? b
来源：http://th.jianghongdianzi.cn

[U87] JS：解构默认值
来源：http://po.nicolike.cn

const { a = 1, b = 2 } = obj;
来源：http://yc.huixiangedu.cn

[U88] JS：对象展开合并
来源：http://op.nicolike.cn

{ ...a, ...b }
来源：http://mg.bjjhwx.cn

[U89] JS：数组去重
来源：http://xs.huanxung.cn

[...new Set(arr)]
来源：http://kf.newstarts.cn

[U90] JS：数字数组排序
来源：http://yl.yuexingan06.cn

[...arr].sort((a, b) => a - b)
来源：http://na.colortex.cn

[U91] JS：对象键值遍历
来源：http://rv.asd995.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://az.panjiajie.cn

[U92] JS：深拷贝
来源：http://gr.chemitech.net.cn

structuredClone(obj)
来源：http://pn.lnxyls.cn

[U93] JS：模板字符串
来源：http://uo.jianghongdianzi.cn

`共 ${n} 条`
来源：http://wl.shxzskj.cn

[U94] JS：箭头函数
来源：http://zp.yuntaijiaju.cn

const double = x => x * 2;
来源：http://sk.nszjky.cn

[U95] JS：Promise 包装
来源：http://pc.yuntaijiaju.cn

new Promise((resolve, reject) => {})
来源：http://rc.chemitech.net.cn

[U96] JS：async/await 与异常
来源：http://pn.jianghongdianzi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rs.chemitech.net.cn

[U97] JS：并发请求
来源：http://dq.yuexingan06.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://gt.shxzskj.cn

[U98] JS：fetch 带 JSON
来源：http://ad.yuexingan06.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wz.shtwfgs.cn

[U99] JS：事件监听
来源：http://zx.gzmigu.cn

el.addEventListener("click", e => {})
来源：http://tj.haigaiapp.cn

[U100] JS：DOM 查询
来源：http://mn.asd995.cn

document.querySelector(".item")
来源：http://sc.bookmarksfly.cn

[U101] JS：classList 操作
来源：http://wv.hahajie.cn

el.classList.toggle("active")
来源：http://gz.shxzskj.cn

[U102] JS：本地存储
来源：http://rj.huixinmuqiang.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://no.colortex.cn

[U103] JS：定时器
来源：http://ko.huixinmuqiang.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ha.hnjuh.cn

[U104] JS：防抖
来源：http://wr.nicolike.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bj.bookmarksfly.cn

[U105] JS：节流
来源：http://fu.gzmigu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nd.newstarts.cn

[U106] JS：日期格式化
来源：http://ob.jianghongdianzi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pb.hahajie.cn

[U107] JS：数字千分位
来源：http://nq.9csxet.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bd.lnxyls.cn

[U108] JS：随机整数
来源：http://lc.hahajie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wc.huanxung.cn

[U109] JS：数组分组
来源：http://eo.szsharing.cn

Object.groupBy(arr, x => x.type)
来源：http://vd.shxzukj.cn

[U110] JS：数组分块
来源：http://iq.nszjky.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rs.panjiajie.cn

[U111] JS：对象转 Map
来源：http://vi.panjiajie.cn

new Map(Object.entries(obj))
来源：http://nw.newstarts.cn

[U112] JS：字符串补位
来源：http://va.lnxyls.cn

"7".padStart(3, "0")
来源：http://ck.yuntaijiaju.cn

[U113] JS：正则替换全部
来源：http://cr.huixinmuqiang.cn

s.replaceAll("a", "b")
来源：http://ve.nicolike.cn

[U114] JS：JSON 深比较
来源：http://bv.nszjky.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://im.yuntaijiaju.cn


<!-- 参考信息 -->