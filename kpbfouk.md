代发 wailian999

[T33] Lua：表（数组）
来源：http://fk.asd995.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hs.chemitech.net.cn

[T34] Lua：遍历表
来源：http://ji.bookmarksfly.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://fs.shxzukj.cn

[T35] Lua：字典表
来源：http://pi.huixiangedu.cn

local d = { a = 1 };  d.b = 2
来源：http://st.gzmigu.cn

[T36] Lua：函数
来源：http://sg.muxihuayi.cn

function add(a, b) return a + b end
来源：http://eu.lnxyls.cn

[T37] Lua：字符串拼接
来源：http://fz.hnjuh.cn

"a" .. "b"
来源：http://if.bookmarksfly.cn

[T38] Lua：条件
来源：http://ey.huanxung.cn

if x > 0 then print("正") end
来源：http://ta.bookmarksfly.cn

[T39] Lua：模式匹配
来源：http://cq.szxytkj.cn

string.find(s, "%d+")
来源：http://xt.jctech888.com.cn

[T40] Lua：元表
来源：http://rm.521024.cn

setmetatable({}, { __index = base })
来源：http://kv.lnxyls.cn

[T41] Perl：Hello World
来源：http://zz.shxzukj.cn

print "Hello\n";
来源：http://bs.szsharing.cn

[T42] Perl：变量类型
来源：http://bc.huixinmuqiang.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qs.newstarts.cn

[T43] Perl：字符串插值
来源：http://ve.gzmigu.cn

"值: $a"
来源：http://nd.lnxyls.cn

[T44] Perl：条件
来源：http://ll.yuntaijiaju.cn

if ($a > 0) { print "正"; }
来源：http://ww.nszjky.cn

[T45] Perl：数组遍历
来源：http://gi.newstarts.cn

for my $x (@arr) { print $x; }
来源：http://vt.newstarts.cn

[T46] Perl：哈希操作
来源：http://gj.521024.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lj.nszjky.cn

[T47] Perl：正则捕获
来源：http://fc.hahajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://kj.yuexingan06.cn

[T48] Perl：正则替换
来源：http://ii.huixinmuqiang.cn

$s =~ s/old/new/g;
来源：http://vp.hnjuh.cn

[T49] Perl：函数
来源：http://hu.panjiajie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://do.yuntaijiaju.cn

[T50] Perl：逐行读文件
来源：http://ol.huixinmuqiang.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://bm.gzmigu.cn

while (my $line = <$fh>) { print $line; }
来源：http://zr.wgjwhj.cn

[T51] Scala：Hello World
来源：http://xs.shxzukj.cn

println("Hello")
来源：http://go.shxzukj.cn

[T52] Scala：变量
来源：http://us.newstarts.cn

val a = 1;  var b = 2
来源：http://az.gzmigu.cn

[T53] Scala：字符串插值
来源：http://vp.panjiajie.cn

s"值: $b"
来源：http://qb.yuexingan06.cn

[T54] Scala：集合映射
来源：http://jz.panjiajie.cn

List(1, 2, 3).map(_ * 2)
来源：http://cs.9csxet.cn

[T55] Scala：集合过滤
来源：http://uk.hnjuh.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ld.jianghongdianzi.cn

[T56] Scala：样例类
来源：http://mz.gzmigu.cn

case class User(name: String, age: Int)
来源：http://vo.yuexingan06.cn

[T57] Scala：模式匹配
来源：http://xx.521024.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ef.huixinmuqiang.cn

[T58] Scala：函数定义
来源：http://nm.huixiangedu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://yc.wgjwhj.cn

[T59] Scala：循环
来源：http://gc.hnjuh.cn

for (i <- 1 to 10) println(i)
来源：http://zb.hahajie.cn

[T60] Scala：折叠
来源：http://fe.newstarts.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jn.hahajie.cn

================================================================================
来源：http://st.gzmigu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kx.chemitech.net.cn

================================================================================
来源：http://hs.huixinmuqiang.cn

[U01] Py：创建虚拟环境
来源：http://jh.gzmigu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://hp.521024.cn

[U02] Py：导出 / 安装依赖
来源：http://eb.huixinmuqiang.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://df.nicolike.cn

[U03] Py：加载 .env 配置
来源：http://oi.szxytkj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://tg.newstarts.cn

[U04] Py：变量调试打印
来源：http://lo.hahajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://om.muxihuayi.cn

[U05] Py：列表去重且保序
来源：http://pm.huanxung.cn

list(dict.fromkeys(arr))
来源：http://gx.bjjhwx.cn

[U06] Py：合并两个字典
来源：http://ue.lnxyls.cn

{**a, **b}
来源：http://xa.shxzukj.cn

[U07] Py：反转字典键值
来源：http://ee.shtwfgs.cn

{v: k for k, v in d.items()}
来源：http://vy.shxzukj.cn

[U08] Py：展平二维列表
来源：http://th.yuexingan06.cn

[y for x in nested for y in x]
来源：http://cd.colortex.cn

[U09] Py：字典取最大值的键
来源：http://wl.asd995.cn

max(d, key=d.get)
来源：http://cs.hnjuh.cn

[U10] Py：按值排序字典
来源：http://mk.shxzskj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://is.wgjwhj.cn

[U11] Py：生成器表达式
来源：http://zq.bjjhwx.cn

(x * 2 for x in arr)
来源：http://qp.wgjwhj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xn.panjiajie.cn

Counter(arr).most_common(3)
来源：http://pn.chemitech.net.cn

[U13] Py：固定长度队列
来源：http://fo.wgjwhj.cn

deque(maxlen=10)
来源：http://gt.hahajie.cn

[U14] Py：分组收集到列表
来源：http://av.asd995.cn

defaultdict(list)
来源：http://wk.huixiangedu.cn

[U15] Py：高精度计时
来源：http://rq.yuntaijiaju.cn

t = time.perf_counter()
来源：http://lz.huixiangedu.cn

[U16] Py：命令行参数解析
来源：http://gn.hnjuh.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kx.bjjhwx.cn

[U17] Py：初始化日志
来源：http://is.hahajie.cn

logging.basicConfig(level=logging.INFO)
来源：http://wf.hnjuh.cn

[U18] Py：预编译正则
来源：http://pa.huixiangedu.cn

pat = re.compile(r"\d+")
来源：http://xr.colortex.cn

[U19] Py：正则替换带回调
来源：http://er.colortex.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xf.colortex.cn

[U20] Py：缓存函数结果
来源：http://om.szxytkj.cn

@functools.lru_cache(maxsize=None)
来源：http://rc.jctech888.com.cn

[U21] Py：自定义上下文管理器
来源：http://xe.521024.cn

@contextlib.contextmanager
来源：http://nq.9csxet.cn

[U22] Py：矩阵转置
来源：http://qv.huixiangedu.cn

list(zip(*m))
来源：http://ya.huixinmuqiang.cn

[U23] Py：分块读取大文件
来源：http://hs.hnjuh.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ou.chemitech.net.cn

[U24] Py：路径操作
来源：http://io.huixinmuqiang.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hj.haigaiapp.cn

[U25] Py：CSV 按字典读
来源：http://gy.colortex.cn

csv.DictReader(f)
来源：http://co.nicolike.cn

[U26] Py：并发下载
来源：http://nm.szxytkj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vv.newstarts.cn

[U27] Py：异步 HTTP
来源：http://jk.bjjhwx.cn

aiohttp.ClientSession() 配合 async with
来源：http://vm.521024.cn

[U28] Py：类型别名
来源：http://qp.huanxung.cn

UserId = int
来源：http://mz.shxzskj.cn

[U29] Py：属性校验
来源：http://bq.9csxet.cn

@property 与 @x.setter 配合
来源：http://dv.asd995.cn

[U30] Py：数据类
来源：http://ro.asd995.cn

@dataclass(slots=True)
来源：http://rc.muxihuayi.cn

[U31] Py：单测
来源：http://bq.newstarts.cn

python -m pytest -q
来源：http://oh.muxihuayi.cn

[U32] Py：代码格式化
来源：http://vv.colortex.cn

ruff format . && ruff check --fix .
来源：http://gk.huixiangedu.cn

[U33] Py：打包发布
来源：http://zl.wgjwhj.cn

python -m build  （依赖 pyproject.toml）
来源：http://tx.hnjuh.cn

[U34] Py：判断编码
来源：http://pi.hahajie.cn

chardet.detect(raw)
来源：http://ji.muxihuayi.cn

[U35] Py：发送邮件
来源：http://pb.hnjuh.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ty.gzmigu.cn

[U36] Py：定时任务
来源：http://uv.9csxet.cn

schedule.every(10).minutes.do(job)
来源：http://kh.haigaiapp.cn

[U37] Py：读写 Excel
来源：http://oc.gzmigu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://pb.yuntaijiaju.cn

[U38] Py：获取脚本所在目录
来源：http://wo.shxzukj.cn

Path(__file__).resolve().parent
来源：http://bb.colortex.cn

[U39] Py：判断是否在交互环境
来源：http://jk.jctech888.com.cn

sys.stdout.isatty()
来源：http://aw.huixiangedu.cn

[U40] Py：打印到标准错误
来源：http://ww.chemitech.net.cn

print("err", file=sys.stderr)
来源：http://kv.hnjuh.cn

[U41] PHP：初始化 Composer 项目
来源：http://hl.panjiajie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://tr.shxzskj.cn

[U42] PHP：PSR-4 自动加载
来源：http://zr.bookmarksfly.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ao.gzmigu.cn

[U43] PHP：声明命名空间
来源：http://uj.chemitech.net.cn

namespace App\Http;
来源：http://ii.newstarts.cn

[U44] PHP：开启严格类型
来源：http://oy.hnjuh.cn

declare(strict_types=1);
来源：http://ij.gzmigu.cn

[U45] PHP：类型声明与返回类型
来源：http://wt.jianghongdianzi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://vu.colortex.cn

[U46] PHP：可空类型
来源：http://ag.yuexingan06.cn

?string $name = null
来源：http://jp.shxzskj.cn

[U47] PHP：联合类型
来源：http://gn.newstarts.cn

int|string $id
来源：http://gi.huanxung.cn

[U48] PHP：纯枚举
来源：http://op.huixiangedu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ms.jianghongdianzi.cn

[U49] PHP：只读属性
来源：http://qo.nszjky.cn

public readonly string $name
来源：http://jf.wgjwhj.cn

[U50] PHP：构造器属性提升
来源：http://ws.shxzskj.cn

public function __construct(private int $id) {}
来源：http://vd.gzmigu.cn

[U51] PHP：数组解构
来源：http://rc.huixiangedu.cn

[$a, $b] = $arr;
来源：http://fp.szsharing.cn

[U52] PHP：箭头函数
来源：http://vy.chemitech.net.cn

$double = fn($x) => $x * 2;
来源：http://zr.huixinmuqiang.cn

[U53] PHP：空合并运算符
来源：http://ap.9csxet.cn

$v = $a ?? $b ?? "default";
来源：http://uq.huixinmuqiang.cn

[U54] PHP：空安全调用
来源：http://ka.colortex.cn

$obj?->method()
来源：http://rk.shxzskj.cn

[U55] PHP：match 表达式
来源：http://mz.szsharing.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jt.haigaiapp.cn

[U56] PHP：命名参数
来源：http://eo.jianghongdianzi.cn

f(a: 1, b: 2)
来源：http://ur.huanxung.cn

[U57] PHP：字符串插值
来源：http://dq.gzmigu.cn

"值: {$a}"
来源：http://aj.asd995.cn

[U58] PHP：数组三件套
来源：http://eq.bjjhwx.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ul.szsharing.cn

[U59] PHP：自定义排序
来源：http://ma.bookmarksfly.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rs.panjiajie.cn

[U60] PHP：JSON 编解码
来源：http://gj.colortex.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xb.szxytkj.cn

[U61] PHP：正则
来源：http://zi.szsharing.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dz.jctech888.com.cn

[U62] PHP：日期对象
来源：http://bz.shxzskj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bl.gzmigu.cn

[U63] PHP：文件读写
来源：http://tt.huixinmuqiang.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sd.hahajie.cn

[U64] PHP：目录遍历
来源：http://tj.newstarts.cn

glob("dir/*.php");  scandir("dir");
来源：http://ov.bookmarksfly.cn

[U65] PHP：会话
来源：http://wz.muxihuayi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://pf.hnjuh.cn

[U66] PHP：设置 Cookie
来源：http://yx.bookmarksfly.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sc.nszjky.cn

[U67] PHP：处理文件上传
来源：http://mn.yuntaijiaju.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://li.9csxet.cn

[U68] PHP：PDO 连接
来源：http://co.wgjwhj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yp.hahajie.cn

[U69] PHP：PDO 预处理
来源：http://qh.nszjky.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://aw.bjjhwx.cn

[U70] PHP：PDO 事务
来源：http://vh.gzmigu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nr.szxytkj.cn

[U71] PHP：抛出异常
来源：http://fs.nicolike.cn

throw new RuntimeException("失败", 500);
来源：http://xf.huixinmuqiang.cn

[U72] PHP：写错误日志
来源：http://mh.521024.cn

error_log("失败: " . $e->getMessage());
来源：http://zz.shxzskj.cn

[U73] PHP：读取 ini 配置
来源：http://uj.huixiangedu.cn

parse_ini_file("config.ini", true)
来源：http://am.521024.cn

[U74] PHP：读取环境变量
来源：http://na.hnjuh.cn

getenv("APP_ENV") ?: "production"
来源：http://cp.huixinmuqiang.cn

[U75] PHP：依赖注入
来源：http://qv.huixiangedu.cn

composer require psr/container
来源：http://ci.yuntaijiaju.cn

[U76] PHP：简单路由
来源：http://ua.huanxung.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://iz.nszjky.cn

[U77] PHP：模板渲染
来源：http://qp.hnjuh.cn

composer require twig/twig
来源：http://oe.huanxung.cn

[U78] PHP：单元测试
来源：http://ny.szxytkj.cn

composer require --dev phpunit/phpunit
来源：http://wz.hnjuh.cn

[U79] PHP：静态分析
来源：http://rl.nicolike.cn

composer require --dev phpstan/phpstan
来源：http://ir.huixinmuqiang.cn

[U80] PHP：代码规范修复
来源：http://pg.huanxung.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://dh.bookmarksfly.cn

[U81] JS：初始化项目
来源：http://ye.asd995.cn

npm init -y;  npm i express
来源：http://nt.yuexingan06.cn

[U82] JS：package.json 脚本
来源：http://fx.nszjky.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xr.shxzskj.cn

[U83] JS：ES Module 导入导出
来源：http://lc.huixiangedu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://jr.nicolike.cn

[U84] JS：CommonJS 写法
来源：http://dh.9csxet.cn

module.exports = { a };  const { a } = require("./m");
来源：http://th.lnxyls.cn

[U85] JS：可选链
来源：http://ym.newstarts.cn

a?.b?.c
来源：http://wr.yuexingan06.cn

[U86] JS：空值合并
来源：http://xf.huixinmuqiang.cn

a ?? b
来源：http://zv.shtwfgs.cn

[U87] JS：解构默认值
来源：http://iy.hnjuh.cn

const { a = 1, b = 2 } = obj;
来源：http://am.hahajie.cn

[U88] JS：对象展开合并
来源：http://vj.newstarts.cn

{ ...a, ...b }
来源：http://ki.huixiangedu.cn

[U89] JS：数组去重
来源：http://pz.jianghongdianzi.cn

[...new Set(arr)]
来源：http://pi.haigaiapp.cn

[U90] JS：数字数组排序
来源：http://yi.yuntaijiaju.cn

[...arr].sort((a, b) => a - b)
来源：http://pt.lnxyls.cn

[U91] JS：对象键值遍历
来源：http://qp.bjjhwx.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://sx.yuntaijiaju.cn

[U92] JS：深拷贝
来源：http://ri.szsharing.cn

structuredClone(obj)
来源：http://cv.huanxung.cn

[U93] JS：模板字符串
来源：http://hy.shxzukj.cn

`共 ${n} 条`
来源：http://wo.haigaiapp.cn

[U94] JS：箭头函数
来源：http://yo.huanxung.cn

const double = x => x * 2;
来源：http://ur.szsharing.cn

[U95] JS：Promise 包装
来源：http://ei.panjiajie.cn

new Promise((resolve, reject) => {})
来源：http://lo.jianghongdianzi.cn

[U96] JS：async/await 与异常
来源：http://fy.szxytkj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hi.szxytkj.cn

[U97] JS：并发请求
来源：http://zt.szxytkj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ep.shtwfgs.cn

[U98] JS：fetch 带 JSON
来源：http://tg.newstarts.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kk.chemitech.net.cn

[U99] JS：事件监听
来源：http://kz.yuntaijiaju.cn

el.addEventListener("click", e => {})
来源：http://bn.shtwfgs.cn

[U100] JS：DOM 查询
来源：http://gd.asd995.cn

document.querySelector(".item")
来源：http://ne.huanxung.cn

[U101] JS：classList 操作
来源：http://mb.haigaiapp.cn

el.classList.toggle("active")
来源：http://ad.yuexingan06.cn

[U102] JS：本地存储
来源：http://yq.521024.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://rl.wgjwhj.cn

[U103] JS：定时器
来源：http://ks.huixiangedu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xy.shxzukj.cn

[U104] JS：防抖
来源：http://xl.wgjwhj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lt.nicolike.cn

[U105] JS：节流
来源：http://ct.jctech888.com.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xx.nszjky.cn

[U106] JS：日期格式化
来源：http://rj.muxihuayi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xv.hahajie.cn

[U107] JS：数字千分位
来源：http://kd.haigaiapp.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jw.nicolike.cn

[U108] JS：随机整数
来源：http://xm.hnjuh.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hw.chemitech.net.cn

[U109] JS：数组分组
来源：http://mx.szsharing.cn

Object.groupBy(arr, x => x.type)
来源：http://pb.hnjuh.cn

[U110] JS：数组分块
来源：http://wi.szxytkj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ot.hahajie.cn

[U111] JS：对象转 Map
来源：http://wb.huixinmuqiang.cn

new Map(Object.entries(obj))
来源：http://on.bookmarksfly.cn

[U112] JS：字符串补位
来源：http://pc.yuexingan06.cn

"7".padStart(3, "0")
来源：http://xk.shxzskj.cn

[U113] JS：正则替换全部
来源：http://wf.muxihuayi.cn

s.replaceAll("a", "b")
来源：http://ye.newstarts.cn

[U114] JS：JSON 深比较
来源：http://mf.shxzukj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://mk.521024.cn

[U115] JS：生成 UUID
来源：http://yb.muxihuayi.cn

crypto.randomUUID()
来源：http://cw.panjiajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://vr.yuexingan06.cn

/** @param {string} name */ function f(name) {}
来源：http://qm.521024.cn

[U117] JS：单元测试
来源：http://mk.huanxung.cn

npm i -D vitest;  npx vitest
来源：http://vw.shxzukj.cn

[U118] JS：开发服务器
来源：http://eb.jianghongdianzi.cn

npm i -D vite;  npx vite
来源：http://ff.bjjhwx.cn

[U119] JS：生产构建
来源：http://yt.521024.cn

npx vite build
来源：http://uk.gzmigu.cn

[U120] JS：读取环境变量（Vite）
来源：http://nl.jctech888.com.cn

import.meta.env.VITE_API_URL
来源：http://up.521024.cn


<!-- 参考信息 -->