代发 wailian999

[T29] Swift：guard 提前返回
来源：http://ax.gzmigu.cn

guard let x = opt else { return }
来源：http://cs.newstarts.cn

[T30] Swift：协议
来源：http://yn.huixiangedu.cn

protocol Shape { func area() -> Double }
来源：http://dt.9csxet.cn

[T31] Lua：Hello World
来源：http://hz.nszjky.cn

print("Hello")
来源：http://fp.haigaiapp.cn

[T32] Lua：局部变量
来源：http://rf.521024.cn

local a = 1
来源：http://pj.wgjwhj.cn

[T33] Lua：表（数组）
来源：http://lw.huanxung.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ap.9csxet.cn

[T34] Lua：遍历表
来源：http://eq.9csxet.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://fh.bookmarksfly.cn

[T35] Lua：字典表
来源：http://dz.nicolike.cn

local d = { a = 1 };  d.b = 2
来源：http://bc.szsharing.cn

[T36] Lua：函数
来源：http://rb.lnxyls.cn

function add(a, b) return a + b end
来源：http://dp.shtwfgs.cn

[T37] Lua：字符串拼接
来源：http://mu.wgjwhj.cn

"a" .. "b"
来源：http://rm.hahajie.cn

[T38] Lua：条件
来源：http://qp.panjiajie.cn

if x > 0 then print("正") end
来源：http://uk.9csxet.cn

[T39] Lua：模式匹配
来源：http://dd.haigaiapp.cn

string.find(s, "%d+")
来源：http://it.yuntaijiaju.cn

[T40] Lua：元表
来源：http://ui.chemitech.net.cn

setmetatable({}, { __index = base })
来源：http://oe.szxytkj.cn

[T41] Perl：Hello World
来源：http://ly.hnjuh.cn

print "Hello\n";
来源：http://ho.chemitech.net.cn

[T42] Perl：变量类型
来源：http://zh.jctech888.com.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vs.asd995.cn

[T43] Perl：字符串插值
来源：http://mg.wgjwhj.cn

"值: $a"
来源：http://hf.wgjwhj.cn

[T44] Perl：条件
来源：http://gi.chemitech.net.cn

if ($a > 0) { print "正"; }
来源：http://kv.bjjhwx.cn

[T45] Perl：数组遍历
来源：http://ds.wgjwhj.cn

for my $x (@arr) { print $x; }
来源：http://dy.muxihuayi.cn

[T46] Perl：哈希操作
来源：http://kp.bjjhwx.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sn.shxzskj.cn

[T47] Perl：正则捕获
来源：http://xc.huixiangedu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://tm.gzmigu.cn

[T48] Perl：正则替换
来源：http://mv.bjjhwx.cn

$s =~ s/old/new/g;
来源：http://br.colortex.cn

[T49] Perl：函数
来源：http://cg.shtwfgs.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://go.yuntaijiaju.cn

[T50] Perl：逐行读文件
来源：http://pv.nicolike.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://hl.bookmarksfly.cn

while (my $line = <$fh>) { print $line; }
来源：http://ox.szsharing.cn

[T51] Scala：Hello World
来源：http://cj.521024.cn

println("Hello")
来源：http://hi.huanxung.cn

[T52] Scala：变量
来源：http://nt.jianghongdianzi.cn

val a = 1;  var b = 2
来源：http://wt.szxytkj.cn

[T53] Scala：字符串插值
来源：http://it.jctech888.com.cn

s"值: $b"
来源：http://om.lnxyls.cn

[T54] Scala：集合映射
来源：http://pc.muxihuayi.cn

List(1, 2, 3).map(_ * 2)
来源：http://dv.muxihuayi.cn

[T55] Scala：集合过滤
来源：http://bo.jianghongdianzi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://kj.shtwfgs.cn

[T56] Scala：样例类
来源：http://tu.bjjhwx.cn

case class User(name: String, age: Int)
来源：http://tl.huanxung.cn

[T57] Scala：模式匹配
来源：http://gt.newstarts.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://hm.wgjwhj.cn

[T58] Scala：函数定义
来源：http://jd.nicolike.cn

def add(a: Int, b: Int): Int = a + b
来源：http://yd.huixiangedu.cn

[T59] Scala：循环
来源：http://jq.muxihuayi.cn

for (i <- 1 to 10) println(i)
来源：http://no.jianghongdianzi.cn

[T60] Scala：折叠
来源：http://cb.gzmigu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xa.huixinmuqiang.cn

================================================================================
来源：http://bk.huanxung.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://la.shxzskj.cn

================================================================================
来源：http://sm.szxytkj.cn

[U01] Py：创建虚拟环境
来源：http://fl.newstarts.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mb.chemitech.net.cn

[U02] Py：导出 / 安装依赖
来源：http://de.bjjhwx.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://he.yuexingan06.cn

[U03] Py：加载 .env 配置
来源：http://qb.huixinmuqiang.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://lx.huanxung.cn

[U04] Py：变量调试打印
来源：http://lw.chemitech.net.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ag.bookmarksfly.cn

[U05] Py：列表去重且保序
来源：http://rh.hahajie.cn

list(dict.fromkeys(arr))
来源：http://fj.bjjhwx.cn

[U06] Py：合并两个字典
来源：http://kg.szxytkj.cn

{**a, **b}
来源：http://rg.yuexingan06.cn

[U07] Py：反转字典键值
来源：http://xb.bjjhwx.cn

{v: k for k, v in d.items()}
来源：http://fe.bjjhwx.cn

[U08] Py：展平二维列表
来源：http://ml.bjjhwx.cn

[y for x in nested for y in x]
来源：http://wx.muxihuayi.cn

[U09] Py：字典取最大值的键
来源：http://va.lnxyls.cn

max(d, key=d.get)
来源：http://dh.lnxyls.cn

[U10] Py：按值排序字典
来源：http://zr.newstarts.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mw.jianghongdianzi.cn

[U11] Py：生成器表达式
来源：http://gd.chemitech.net.cn

(x * 2 for x in arr)
来源：http://jj.nicolike.cn

[U12] Py：取出现最多的 3 个元素
来源：http://pi.huixiangedu.cn

Counter(arr).most_common(3)
来源：http://rx.521024.cn

[U13] Py：固定长度队列
来源：http://sv.nszjky.cn

deque(maxlen=10)
来源：http://fo.shxzukj.cn

[U14] Py：分组收集到列表
来源：http://ey.shxzskj.cn

defaultdict(list)
来源：http://zb.huanxung.cn

[U15] Py：高精度计时
来源：http://lw.asd995.cn

t = time.perf_counter()
来源：http://hq.yuntaijiaju.cn

[U16] Py：命令行参数解析
来源：http://en.jctech888.com.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://it.lnxyls.cn

[U17] Py：初始化日志
来源：http://se.jianghongdianzi.cn

logging.basicConfig(level=logging.INFO)
来源：http://qx.yuexingan06.cn

[U18] Py：预编译正则
来源：http://kt.szxytkj.cn

pat = re.compile(r"\d+")
来源：http://db.szxytkj.cn

[U19] Py：正则替换带回调
来源：http://fj.shxzukj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kq.wgjwhj.cn

[U20] Py：缓存函数结果
来源：http://cr.gzmigu.cn

@functools.lru_cache(maxsize=None)
来源：http://mf.gzmigu.cn

[U21] Py：自定义上下文管理器
来源：http://uc.jianghongdianzi.cn

@contextlib.contextmanager
来源：http://sm.szsharing.cn

[U22] Py：矩阵转置
来源：http://oz.nicolike.cn

list(zip(*m))
来源：http://ux.9csxet.cn

[U23] Py：分块读取大文件
来源：http://oe.nicolike.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nu.szsharing.cn

[U24] Py：路径操作
来源：http://st.bookmarksfly.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fd.wgjwhj.cn

[U25] Py：CSV 按字典读
来源：http://be.newstarts.cn

csv.DictReader(f)
来源：http://ox.huixinmuqiang.cn

[U26] Py：并发下载
来源：http://er.panjiajie.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rl.shxzukj.cn

[U27] Py：异步 HTTP
来源：http://oe.shxzukj.cn

aiohttp.ClientSession() 配合 async with
来源：http://el.muxihuayi.cn

[U28] Py：类型别名
来源：http://lx.hahajie.cn

UserId = int
来源：http://ax.yuexingan06.cn

[U29] Py：属性校验
来源：http://lq.jctech888.com.cn

@property 与 @x.setter 配合
来源：http://mw.bjjhwx.cn

[U30] Py：数据类
来源：http://do.521024.cn

@dataclass(slots=True)
来源：http://yi.yuexingan06.cn

[U31] Py：单测
来源：http://pw.muxihuayi.cn

python -m pytest -q
来源：http://eu.muxihuayi.cn

[U32] Py：代码格式化
来源：http://ru.asd995.cn

ruff format . && ruff check --fix .
来源：http://hs.bjjhwx.cn

[U33] Py：打包发布
来源：http://qo.nicolike.cn

python -m build  （依赖 pyproject.toml）
来源：http://ib.yuntaijiaju.cn

[U34] Py：判断编码
来源：http://bj.yuexingan06.cn

chardet.detect(raw)
来源：http://mq.muxihuayi.cn

[U35] Py：发送邮件
来源：http://sc.huanxung.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ws.bookmarksfly.cn

[U36] Py：定时任务
来源：http://ka.huixiangedu.cn

schedule.every(10).minutes.do(job)
来源：http://kk.yuntaijiaju.cn

[U37] Py：读写 Excel
来源：http://uk.gzmigu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://mx.lnxyls.cn

[U38] Py：获取脚本所在目录
来源：http://wb.chemitech.net.cn

Path(__file__).resolve().parent
来源：http://ob.newstarts.cn

[U39] Py：判断是否在交互环境
来源：http://dh.panjiajie.cn

sys.stdout.isatty()
来源：http://ew.huixinmuqiang.cn

[U40] Py：打印到标准错误
来源：http://ry.shtwfgs.cn

print("err", file=sys.stderr)
来源：http://em.wgjwhj.cn

[U41] PHP：初始化 Composer 项目
来源：http://wb.muxihuayi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://sb.521024.cn

[U42] PHP：PSR-4 自动加载
来源：http://mq.asd995.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pi.jctech888.com.cn

[U43] PHP：声明命名空间
来源：http://ji.szxytkj.cn

namespace App\Http;
来源：http://iy.shxzskj.cn

[U44] PHP：开启严格类型
来源：http://sm.yuexingan06.cn

declare(strict_types=1);
来源：http://dq.huixinmuqiang.cn

[U45] PHP：类型声明与返回类型
来源：http://ya.muxihuayi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://gt.newstarts.cn

[U46] PHP：可空类型
来源：http://xu.yuexingan06.cn

?string $name = null
来源：http://qx.szsharing.cn

[U47] PHP：联合类型
来源：http://rl.haigaiapp.cn

int|string $id
来源：http://rk.shtwfgs.cn

[U48] PHP：纯枚举
来源：http://jt.bjjhwx.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vb.521024.cn

[U49] PHP：只读属性
来源：http://lk.gzmigu.cn

public readonly string $name
来源：http://mw.jianghongdianzi.cn

[U50] PHP：构造器属性提升
来源：http://cm.chemitech.net.cn

public function __construct(private int $id) {}
来源：http://ak.muxihuayi.cn

[U51] PHP：数组解构
来源：http://sy.huanxung.cn

[$a, $b] = $arr;
来源：http://mw.jctech888.com.cn

[U52] PHP：箭头函数
来源：http://xi.muxihuayi.cn

$double = fn($x) => $x * 2;
来源：http://gp.shxzskj.cn

[U53] PHP：空合并运算符
来源：http://kg.hnjuh.cn

$v = $a ?? $b ?? "default";
来源：http://ye.yuexingan06.cn

[U54] PHP：空安全调用
来源：http://nb.bookmarksfly.cn

$obj?->method()
来源：http://bo.hnjuh.cn

[U55] PHP：match 表达式
来源：http://mk.huanxung.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jo.chemitech.net.cn

[U56] PHP：命名参数
来源：http://rh.huixiangedu.cn

f(a: 1, b: 2)
来源：http://zw.panjiajie.cn

[U57] PHP：字符串插值
来源：http://ym.panjiajie.cn

"值: {$a}"
来源：http://dv.wgjwhj.cn

[U58] PHP：数组三件套
来源：http://ep.jctech888.com.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gm.nszjky.cn

[U59] PHP：自定义排序
来源：http://nu.shtwfgs.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zd.panjiajie.cn

[U60] PHP：JSON 编解码
来源：http://cw.newstarts.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xu.hahajie.cn

[U61] PHP：正则
来源：http://tv.huixinmuqiang.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zj.gzmigu.cn

[U62] PHP：日期对象
来源：http://uv.shxzskj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zf.jianghongdianzi.cn

[U63] PHP：文件读写
来源：http://pe.nicolike.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://or.haigaiapp.cn

[U64] PHP：目录遍历
来源：http://qh.szxytkj.cn

glob("dir/*.php");  scandir("dir");
来源：http://bx.nszjky.cn

[U65] PHP：会话
来源：http://jd.newstarts.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ov.asd995.cn

[U66] PHP：设置 Cookie
来源：http://xh.nicolike.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kl.521024.cn

[U67] PHP：处理文件上传
来源：http://mz.huanxung.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nw.shxzukj.cn

[U68] PHP：PDO 连接
来源：http://jz.wgjwhj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wu.huixinmuqiang.cn

[U69] PHP：PDO 预处理
来源：http://tg.hnjuh.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rt.jctech888.com.cn

[U70] PHP：PDO 事务
来源：http://iv.yuexingan06.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://je.haigaiapp.cn

[U71] PHP：抛出异常
来源：http://ww.9csxet.cn

throw new RuntimeException("失败", 500);
来源：http://tt.lnxyls.cn

[U72] PHP：写错误日志
来源：http://xr.jianghongdianzi.cn

error_log("失败: " . $e->getMessage());
来源：http://ij.huixinmuqiang.cn

[U73] PHP：读取 ini 配置
来源：http://yy.szxytkj.cn

parse_ini_file("config.ini", true)
来源：http://mi.bookmarksfly.cn

[U74] PHP：读取环境变量
来源：http://xy.huanxung.cn

getenv("APP_ENV") ?: "production"
来源：http://xh.panjiajie.cn

[U75] PHP：依赖注入
来源：http://il.shtwfgs.cn

composer require psr/container
来源：http://rp.huixinmuqiang.cn

[U76] PHP：简单路由
来源：http://wr.lnxyls.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yj.shxzskj.cn

[U77] PHP：模板渲染
来源：http://ei.gzmigu.cn

composer require twig/twig
来源：http://jz.hnjuh.cn

[U78] PHP：单元测试
来源：http://jo.wgjwhj.cn

composer require --dev phpunit/phpunit
来源：http://vz.szsharing.cn

[U79] PHP：静态分析
来源：http://bc.wgjwhj.cn

composer require --dev phpstan/phpstan
来源：http://zx.wgjwhj.cn

[U80] PHP：代码规范修复
来源：http://mv.yuexingan06.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://yw.hahajie.cn

[U81] JS：初始化项目
来源：http://ui.szxytkj.cn

npm init -y;  npm i express
来源：http://cq.wgjwhj.cn

[U82] JS：package.json 脚本
来源：http://gr.hahajie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nw.muxihuayi.cn

[U83] JS：ES Module 导入导出
来源：http://qr.hnjuh.cn

export const a = 1;  import { a } from "./m.js";
来源：http://bi.521024.cn

[U84] JS：CommonJS 写法
来源：http://al.huixinmuqiang.cn

module.exports = { a };  const { a } = require("./m");
来源：http://yy.huixinmuqiang.cn

[U85] JS：可选链
来源：http://yv.lnxyls.cn

a?.b?.c
来源：http://px.huixinmuqiang.cn

[U86] JS：空值合并
来源：http://kg.huixinmuqiang.cn

a ?? b
来源：http://mw.nicolike.cn

[U87] JS：解构默认值
来源：http://fm.yuexingan06.cn

const { a = 1, b = 2 } = obj;
来源：http://mn.bookmarksfly.cn

[U88] JS：对象展开合并
来源：http://wx.colortex.cn

{ ...a, ...b }
来源：http://wy.jctech888.com.cn

[U89] JS：数组去重
来源：http://jj.panjiajie.cn

[...new Set(arr)]
来源：http://ci.huanxung.cn

[U90] JS：数字数组排序
来源：http://mj.wgjwhj.cn

[...arr].sort((a, b) => a - b)
来源：http://cn.hahajie.cn

[U91] JS：对象键值遍历
来源：http://il.shtwfgs.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ei.9csxet.cn

[U92] JS：深拷贝
来源：http://cu.muxihuayi.cn

structuredClone(obj)
来源：http://lw.shxzskj.cn

[U93] JS：模板字符串
来源：http://hs.shxzskj.cn

`共 ${n} 条`
来源：http://nc.chemitech.net.cn

[U94] JS：箭头函数
来源：http://ti.521024.cn

const double = x => x * 2;
来源：http://cj.newstarts.cn

[U95] JS：Promise 包装
来源：http://tn.521024.cn

new Promise((resolve, reject) => {})
来源：http://sf.gzmigu.cn

[U96] JS：async/await 与异常
来源：http://qr.huanxung.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rd.shxzukj.cn

[U97] JS：并发请求
来源：http://xx.wgjwhj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://kx.hahajie.cn

[U98] JS：fetch 带 JSON
来源：http://zt.newstarts.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kn.panjiajie.cn

[U99] JS：事件监听
来源：http://cx.haigaiapp.cn

el.addEventListener("click", e => {})
来源：http://kg.chemitech.net.cn

[U100] JS：DOM 查询
来源：http://ms.shtwfgs.cn

document.querySelector(".item")
来源：http://ha.muxihuayi.cn

[U101] JS：classList 操作
来源：http://xm.521024.cn

el.classList.toggle("active")
来源：http://hm.shxzukj.cn

[U102] JS：本地存储
来源：http://zk.newstarts.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://nm.huixinmuqiang.cn

[U103] JS：定时器
来源：http://rc.521024.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yf.hnjuh.cn

[U104] JS：防抖
来源：http://fr.huanxung.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://at.nszjky.cn

[U105] JS：节流
来源：http://oc.521024.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yi.yuexingan06.cn

[U106] JS：日期格式化
来源：http://pv.hahajie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fy.shtwfgs.cn

[U107] JS：数字千分位
来源：http://jr.bjjhwx.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fg.wgjwhj.cn

[U108] JS：随机整数
来源：http://no.newstarts.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tr.hahajie.cn

[U109] JS：数组分组
来源：http://wj.panjiajie.cn

Object.groupBy(arr, x => x.type)
来源：http://dc.shtwfgs.cn

[U110] JS：数组分块
来源：http://yj.haigaiapp.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gd.szsharing.cn

[U111] JS：对象转 Map
来源：http://hw.jianghongdianzi.cn

new Map(Object.entries(obj))
来源：http://af.lnxyls.cn

[U112] JS：字符串补位
来源：http://ub.panjiajie.cn

"7".padStart(3, "0")
来源：http://zy.newstarts.cn

[U113] JS：正则替换全部
来源：http://mb.gzmigu.cn

s.replaceAll("a", "b")
来源：http://ex.jianghongdianzi.cn

[U114] JS：JSON 深比较
来源：http://jh.yuexingan06.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://bl.bjjhwx.cn

[U115] JS：生成 UUID
来源：http://ja.huixinmuqiang.cn

crypto.randomUUID()
来源：http://tl.lnxyls.cn

[U116] JS：类型检查（JSDoc）
来源：http://po.colortex.cn

/** @param {string} name */ function f(name) {}
来源：http://sf.asd995.cn


<!-- 参考信息 -->