代发 wailian999

[T25] Swift：结构体
来源：http://xk.9csxet.cn

struct P { var x: Int }
来源：http://do.nicolike.cn

[T26] Swift：类与重写
来源：http://qt.bookmarksfly.cn

class A: Base { override func f() {} }
来源：http://vc.panjiajie.cn

[T27] Swift：错误处理
来源：http://oj.shxzskj.cn

do { try f() } catch { print(error) }
来源：http://ic.521024.cn

[T28] Swift：枚举
来源：http://rq.hahajie.cn

enum Color { case red, green }
来源：http://ty.nicolike.cn

[T29] Swift：guard 提前返回
来源：http://sy.szsharing.cn

guard let x = opt else { return }
来源：http://wh.nicolike.cn

[T30] Swift：协议
来源：http://sa.newstarts.cn

protocol Shape { func area() -> Double }
来源：http://it.wgjwhj.cn

[T31] Lua：Hello World
来源：http://bo.szxytkj.cn

print("Hello")
来源：http://gj.colortex.cn

[T32] Lua：局部变量
来源：http://ld.colortex.cn

local a = 1
来源：http://mk.asd995.cn

[T33] Lua：表（数组）
来源：http://xu.muxihuayi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wa.shtwfgs.cn

[T34] Lua：遍历表
来源：http://df.huixinmuqiang.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://jf.yuntaijiaju.cn

[T35] Lua：字典表
来源：http://ds.bjjhwx.cn

local d = { a = 1 };  d.b = 2
来源：http://pq.521024.cn

[T36] Lua：函数
来源：http://ki.colortex.cn

function add(a, b) return a + b end
来源：http://wy.lnxyls.cn

[T37] Lua：字符串拼接
来源：http://du.hnjuh.cn

"a" .. "b"
来源：http://fo.newstarts.cn

[T38] Lua：条件
来源：http://pv.yuntaijiaju.cn

if x > 0 then print("正") end
来源：http://yo.nicolike.cn

[T39] Lua：模式匹配
来源：http://yj.muxihuayi.cn

string.find(s, "%d+")
来源：http://pg.huixinmuqiang.cn

[T40] Lua：元表
来源：http://hr.huanxung.cn

setmetatable({}, { __index = base })
来源：http://nz.nszjky.cn

[T41] Perl：Hello World
来源：http://md.hnjuh.cn

print "Hello\n";
来源：http://he.chemitech.net.cn

[T42] Perl：变量类型
来源：http://wq.huixinmuqiang.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mx.gzmigu.cn

[T43] Perl：字符串插值
来源：http://hy.hahajie.cn

"值: $a"
来源：http://ip.shtwfgs.cn

[T44] Perl：条件
来源：http://nh.521024.cn

if ($a > 0) { print "正"; }
来源：http://xo.hahajie.cn

[T45] Perl：数组遍历
来源：http://vv.yuntaijiaju.cn

for my $x (@arr) { print $x; }
来源：http://fh.shxzukj.cn

[T46] Perl：哈希操作
来源：http://nt.haigaiapp.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nj.bjjhwx.cn

[T47] Perl：正则捕获
来源：http://ih.jianghongdianzi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://zs.haigaiapp.cn

[T48] Perl：正则替换
来源：http://dx.newstarts.cn

$s =~ s/old/new/g;
来源：http://rm.hahajie.cn

[T49] Perl：函数
来源：http://pw.hnjuh.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ik.hahajie.cn

[T50] Perl：逐行读文件
来源：http://qn.9csxet.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qm.jianghongdianzi.cn

while (my $line = <$fh>) { print $line; }
来源：http://zz.shxzukj.cn

[T51] Scala：Hello World
来源：http://zu.shxzukj.cn

println("Hello")
来源：http://xd.huixiangedu.cn

[T52] Scala：变量
来源：http://cq.bookmarksfly.cn

val a = 1;  var b = 2
来源：http://uh.lnxyls.cn

[T53] Scala：字符串插值
来源：http://zx.szxytkj.cn

s"值: $b"
来源：http://pa.panjiajie.cn

[T54] Scala：集合映射
来源：http://pb.newstarts.cn

List(1, 2, 3).map(_ * 2)
来源：http://jj.gzmigu.cn

[T55] Scala：集合过滤
来源：http://tl.yuntaijiaju.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gn.bookmarksfly.cn

[T56] Scala：样例类
来源：http://br.huixinmuqiang.cn

case class User(name: String, age: Int)
来源：http://ar.jctech888.com.cn

[T57] Scala：模式匹配
来源：http://tt.gzmigu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://mw.huixiangedu.cn

[T58] Scala：函数定义
来源：http://xg.521024.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ql.panjiajie.cn

[T59] Scala：循环
来源：http://yq.huixinmuqiang.cn

for (i <- 1 to 10) println(i)
来源：http://qr.521024.cn

[T60] Scala：折叠
来源：http://be.bookmarksfly.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dx.chemitech.net.cn

================================================================================
来源：http://pu.nicolike.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ei.chemitech.net.cn

================================================================================
来源：http://fn.521024.cn

[U01] Py：创建虚拟环境
来源：http://bx.nszjky.cn

python -m venv .venv && source .venv/bin/activate
来源：http://aq.yuexingan06.cn

[U02] Py：导出 / 安装依赖
来源：http://gr.hahajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ni.szsharing.cn

[U03] Py：加载 .env 配置
来源：http://ss.yuntaijiaju.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://lv.asd995.cn

[U04] Py：变量调试打印
来源：http://fw.huanxung.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hc.muxihuayi.cn

[U05] Py：列表去重且保序
来源：http://va.lnxyls.cn

list(dict.fromkeys(arr))
来源：http://od.hahajie.cn

[U06] Py：合并两个字典
来源：http://od.bookmarksfly.cn

{**a, **b}
来源：http://sk.yuexingan06.cn

[U07] Py：反转字典键值
来源：http://sv.lnxyls.cn

{v: k for k, v in d.items()}
来源：http://tv.lnxyls.cn

[U08] Py：展平二维列表
来源：http://ss.shxzukj.cn

[y for x in nested for y in x]
来源：http://ku.521024.cn

[U09] Py：字典取最大值的键
来源：http://pa.haigaiapp.cn

max(d, key=d.get)
来源：http://mg.9csxet.cn

[U10] Py：按值排序字典
来源：http://ny.bjjhwx.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cf.haigaiapp.cn

[U11] Py：生成器表达式
来源：http://ro.jianghongdianzi.cn

(x * 2 for x in arr)
来源：http://de.9csxet.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xr.hahajie.cn

Counter(arr).most_common(3)
来源：http://ei.521024.cn

[U13] Py：固定长度队列
来源：http://yh.nicolike.cn

deque(maxlen=10)
来源：http://ul.hahajie.cn

[U14] Py：分组收集到列表
来源：http://rt.wgjwhj.cn

defaultdict(list)
来源：http://je.haigaiapp.cn

[U15] Py：高精度计时
来源：http://ds.yuntaijiaju.cn

t = time.perf_counter()
来源：http://hi.yuexingan06.cn

[U16] Py：命令行参数解析
来源：http://zc.huanxung.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ni.yuexingan06.cn

[U17] Py：初始化日志
来源：http://fz.szxytkj.cn

logging.basicConfig(level=logging.INFO)
来源：http://dh.jctech888.com.cn

[U18] Py：预编译正则
来源：http://pk.bookmarksfly.cn

pat = re.compile(r"\d+")
来源：http://xh.jctech888.com.cn

[U19] Py：正则替换带回调
来源：http://xw.huixinmuqiang.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jf.colortex.cn

[U20] Py：缓存函数结果
来源：http://zp.huanxung.cn

@functools.lru_cache(maxsize=None)
来源：http://vz.hnjuh.cn

[U21] Py：自定义上下文管理器
来源：http://xg.nszjky.cn

@contextlib.contextmanager
来源：http://cs.asd995.cn

[U22] Py：矩阵转置
来源：http://nu.haigaiapp.cn

list(zip(*m))
来源：http://mi.yuntaijiaju.cn

[U23] Py：分块读取大文件
来源：http://iv.wgjwhj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ui.wgjwhj.cn

[U24] Py：路径操作
来源：http://vl.wgjwhj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ty.panjiajie.cn

[U25] Py：CSV 按字典读
来源：http://ot.gzmigu.cn

csv.DictReader(f)
来源：http://gh.jianghongdianzi.cn

[U26] Py：并发下载
来源：http://he.huanxung.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vr.szsharing.cn

[U27] Py：异步 HTTP
来源：http://ft.hahajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://ik.wgjwhj.cn

[U28] Py：类型别名
来源：http://hd.colortex.cn

UserId = int
来源：http://nv.jctech888.com.cn

[U29] Py：属性校验
来源：http://cr.szxytkj.cn

@property 与 @x.setter 配合
来源：http://st.asd995.cn

[U30] Py：数据类
来源：http://iz.hahajie.cn

@dataclass(slots=True)
来源：http://mq.9csxet.cn

[U31] Py：单测
来源：http://yt.huanxung.cn

python -m pytest -q
来源：http://we.jianghongdianzi.cn

[U32] Py：代码格式化
来源：http://kw.nicolike.cn

ruff format . && ruff check --fix .
来源：http://af.hahajie.cn

[U33] Py：打包发布
来源：http://ty.shxzukj.cn

python -m build  （依赖 pyproject.toml）
来源：http://lm.shtwfgs.cn

[U34] Py：判断编码
来源：http://ax.huixinmuqiang.cn

chardet.detect(raw)
来源：http://td.huanxung.cn

[U35] Py：发送邮件
来源：http://wn.shtwfgs.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zx.gzmigu.cn

[U36] Py：定时任务
来源：http://nv.wgjwhj.cn

schedule.every(10).minutes.do(job)
来源：http://kd.521024.cn

[U37] Py：读写 Excel
来源：http://ke.nicolike.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ho.huanxung.cn

[U38] Py：获取脚本所在目录
来源：http://dz.bjjhwx.cn

Path(__file__).resolve().parent
来源：http://gx.panjiajie.cn

[U39] Py：判断是否在交互环境
来源：http://pl.yuntaijiaju.cn

sys.stdout.isatty()
来源：http://jh.nszjky.cn

[U40] Py：打印到标准错误
来源：http://ev.521024.cn

print("err", file=sys.stderr)
来源：http://ti.wgjwhj.cn

[U41] PHP：初始化 Composer 项目
来源：http://rv.bookmarksfly.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://rb.shxzskj.cn

[U42] PHP：PSR-4 自动加载
来源：http://vp.szsharing.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rv.nszjky.cn

[U43] PHP：声明命名空间
来源：http://ux.shxzskj.cn

namespace App\Http;
来源：http://ag.muxihuayi.cn

[U44] PHP：开启严格类型
来源：http://ef.hnjuh.cn

declare(strict_types=1);
来源：http://vu.colortex.cn

[U45] PHP：类型声明与返回类型
来源：http://wy.chemitech.net.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://as.muxihuayi.cn

[U46] PHP：可空类型
来源：http://jf.nicolike.cn

?string $name = null
来源：http://eu.shxzskj.cn

[U47] PHP：联合类型
来源：http://ae.9csxet.cn

int|string $id
来源：http://cm.jctech888.com.cn

[U48] PHP：纯枚举
来源：http://ex.nszjky.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rj.haigaiapp.cn

[U49] PHP：只读属性
来源：http://to.bookmarksfly.cn

public readonly string $name
来源：http://pj.haigaiapp.cn

[U50] PHP：构造器属性提升
来源：http://jo.panjiajie.cn

public function __construct(private int $id) {}
来源：http://az.lnxyls.cn

[U51] PHP：数组解构
来源：http://dw.jianghongdianzi.cn

[$a, $b] = $arr;
来源：http://ej.nszjky.cn

[U52] PHP：箭头函数
来源：http://gy.huanxung.cn

$double = fn($x) => $x * 2;
来源：http://dq.chemitech.net.cn

[U53] PHP：空合并运算符
来源：http://no.szxytkj.cn

$v = $a ?? $b ?? "default";
来源：http://ix.bjjhwx.cn

[U54] PHP：空安全调用
来源：http://xs.wgjwhj.cn

$obj?->method()
来源：http://al.hnjuh.cn

[U55] PHP：match 表达式
来源：http://es.jctech888.com.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ut.521024.cn

[U56] PHP：命名参数
来源：http://dp.lnxyls.cn

f(a: 1, b: 2)
来源：http://yz.nicolike.cn

[U57] PHP：字符串插值
来源：http://sr.asd995.cn

"值: {$a}"
来源：http://um.lnxyls.cn

[U58] PHP：数组三件套
来源：http://lj.9csxet.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qe.shtwfgs.cn

[U59] PHP：自定义排序
来源：http://ge.yuexingan06.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xs.nicolike.cn

[U60] PHP：JSON 编解码
来源：http://mm.bookmarksfly.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cm.chemitech.net.cn

[U61] PHP：正则
来源：http://mq.shxzskj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pa.gzmigu.cn

[U62] PHP：日期对象
来源：http://wv.szsharing.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ep.huixiangedu.cn

[U63] PHP：文件读写
来源：http://zn.yuntaijiaju.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mr.gzmigu.cn

[U64] PHP：目录遍历
来源：http://kh.bookmarksfly.cn

glob("dir/*.php");  scandir("dir");
来源：http://se.yuntaijiaju.cn

[U65] PHP：会话
来源：http://pf.huixinmuqiang.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://wt.9csxet.cn

[U66] PHP：设置 Cookie
来源：http://kq.chemitech.net.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://it.chemitech.net.cn

[U67] PHP：处理文件上传
来源：http://qn.newstarts.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kx.yuexingan06.cn

[U68] PHP：PDO 连接
来源：http://ao.newstarts.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yj.newstarts.cn

[U69] PHP：PDO 预处理
来源：http://zh.shxzskj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tr.yuexingan06.cn

[U70] PHP：PDO 事务
来源：http://wx.panjiajie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ak.szsharing.cn

[U71] PHP：抛出异常
来源：http://bj.haigaiapp.cn

throw new RuntimeException("失败", 500);
来源：http://if.lnxyls.cn

[U72] PHP：写错误日志
来源：http://cx.newstarts.cn

error_log("失败: " . $e->getMessage());
来源：http://jw.gzmigu.cn

[U73] PHP：读取 ini 配置
来源：http://du.huixiangedu.cn

parse_ini_file("config.ini", true)
来源：http://ov.huanxung.cn

[U74] PHP：读取环境变量
来源：http://lh.wgjwhj.cn

getenv("APP_ENV") ?: "production"
来源：http://xz.9csxet.cn

[U75] PHP：依赖注入
来源：http://vx.bookmarksfly.cn

composer require psr/container
来源：http://ka.hahajie.cn

[U76] PHP：简单路由
来源：http://th.yuntaijiaju.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dn.huixinmuqiang.cn

[U77] PHP：模板渲染
来源：http://ly.nicolike.cn

composer require twig/twig
来源：http://ek.lnxyls.cn

[U78] PHP：单元测试
来源：http://rw.panjiajie.cn

composer require --dev phpunit/phpunit
来源：http://zt.huixiangedu.cn

[U79] PHP：静态分析
来源：http://hj.chemitech.net.cn

composer require --dev phpstan/phpstan
来源：http://fj.bookmarksfly.cn

[U80] PHP：代码规范修复
来源：http://hq.shxzskj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jm.9csxet.cn

[U81] JS：初始化项目
来源：http://yq.chemitech.net.cn

npm init -y;  npm i express
来源：http://yv.shxzskj.cn

[U82] JS：package.json 脚本
来源：http://zw.lnxyls.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://no.wgjwhj.cn

[U83] JS：ES Module 导入导出
来源：http://fg.9csxet.cn

export const a = 1;  import { a } from "./m.js";
来源：http://cu.huixiangedu.cn

[U84] JS：CommonJS 写法
来源：http://wv.shxzukj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://la.hahajie.cn

[U85] JS：可选链
来源：http://zr.nicolike.cn

a?.b?.c
来源：http://po.9csxet.cn

[U86] JS：空值合并
来源：http://rt.asd995.cn

a ?? b
来源：http://cv.asd995.cn

[U87] JS：解构默认值
来源：http://an.jctech888.com.cn

const { a = 1, b = 2 } = obj;
来源：http://ha.chemitech.net.cn

[U88] JS：对象展开合并
来源：http://oh.bookmarksfly.cn

{ ...a, ...b }
来源：http://nv.nszjky.cn

[U89] JS：数组去重
来源：http://ft.9csxet.cn

[...new Set(arr)]
来源：http://pz.panjiajie.cn

[U90] JS：数字数组排序
来源：http://jc.9csxet.cn

[...arr].sort((a, b) => a - b)
来源：http://rs.shtwfgs.cn

[U91] JS：对象键值遍历
来源：http://ix.colortex.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tq.hahajie.cn

[U92] JS：深拷贝
来源：http://kg.shxzskj.cn

structuredClone(obj)
来源：http://uc.yuntaijiaju.cn

[U93] JS：模板字符串
来源：http://jo.bjjhwx.cn

`共 ${n} 条`
来源：http://gy.yuexingan06.cn

[U94] JS：箭头函数
来源：http://db.panjiajie.cn

const double = x => x * 2;
来源：http://va.shtwfgs.cn

[U95] JS：Promise 包装
来源：http://nr.nszjky.cn

new Promise((resolve, reject) => {})
来源：http://ms.chemitech.net.cn

[U96] JS：async/await 与异常
来源：http://qz.szxytkj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pk.hnjuh.cn

[U97] JS：并发请求
来源：http://zx.newstarts.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://uh.hahajie.cn

[U98] JS：fetch 带 JSON
来源：http://zk.lnxyls.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cu.lnxyls.cn

[U99] JS：事件监听
来源：http://af.wgjwhj.cn

el.addEventListener("click", e => {})
来源：http://jm.bjjhwx.cn

[U100] JS：DOM 查询
来源：http://kh.chemitech.net.cn

document.querySelector(".item")
来源：http://pf.muxihuayi.cn

[U101] JS：classList 操作
来源：http://ml.nszjky.cn

el.classList.toggle("active")
来源：http://ki.muxihuayi.cn

[U102] JS：本地存储
来源：http://tz.szxytkj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xa.shxzskj.cn

[U103] JS：定时器
来源：http://vl.asd995.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ji.gzmigu.cn

[U104] JS：防抖
来源：http://tz.szxytkj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ro.jctech888.com.cn

[U105] JS：节流
来源：http://kv.yuntaijiaju.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dd.hahajie.cn

[U106] JS：日期格式化
来源：http://cx.haigaiapp.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hl.colortex.cn

[U107] JS：数字千分位
来源：http://jy.haigaiapp.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ju.wgjwhj.cn

[U108] JS：随机整数
来源：http://ht.jctech888.com.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mc.panjiajie.cn

[U109] JS：数组分组
来源：http://en.szxytkj.cn

Object.groupBy(arr, x => x.type)
来源：http://jk.haigaiapp.cn

[U110] JS：数组分块
来源：http://nh.chemitech.net.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qg.muxihuayi.cn

[U111] JS：对象转 Map
来源：http://cd.wgjwhj.cn

new Map(Object.entries(obj))
来源：http://pt.hahajie.cn

[U112] JS：字符串补位
来源：http://do.gzmigu.cn

"7".padStart(3, "0")
来源：http://gf.9csxet.cn


<!-- 参考信息 -->