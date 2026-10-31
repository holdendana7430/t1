代发 wailian999

[T35] Lua：字典表
来源：http://se.jctech888.com.cn

local d = { a = 1 };  d.b = 2
来源：http://rx.hahajie.cn

[T36] Lua：函数
来源：http://et.yuexingan06.cn

function add(a, b) return a + b end
来源：http://zw.jianghongdianzi.cn

[T37] Lua：字符串拼接
来源：http://je.yuntaijiaju.cn

"a" .. "b"
来源：http://db.huixinmuqiang.cn

[T38] Lua：条件
来源：http://qe.szxytkj.cn

if x > 0 then print("正") end
来源：http://yh.hnjuh.cn

[T39] Lua：模式匹配
来源：http://je.bjjhwx.cn

string.find(s, "%d+")
来源：http://st.jianghongdianzi.cn

[T40] Lua：元表
来源：http://so.hnjuh.cn

setmetatable({}, { __index = base })
来源：http://zf.hnjuh.cn

[T41] Perl：Hello World
来源：http://fj.asd995.cn

print "Hello\n";
来源：http://yr.nicolike.cn

[T42] Perl：变量类型
来源：http://yv.shxzskj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fg.hahajie.cn

[T43] Perl：字符串插值
来源：http://fe.szsharing.cn

"值: $a"
来源：http://pe.lnxyls.cn

[T44] Perl：条件
来源：http://ju.521024.cn

if ($a > 0) { print "正"; }
来源：http://ho.gzmigu.cn

[T45] Perl：数组遍历
来源：http://uv.bookmarksfly.cn

for my $x (@arr) { print $x; }
来源：http://bt.jctech888.com.cn

[T46] Perl：哈希操作
来源：http://gf.szsharing.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rl.huixinmuqiang.cn

[T47] Perl：正则捕获
来源：http://pl.szsharing.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dd.yuntaijiaju.cn

[T48] Perl：正则替换
来源：http://fk.haigaiapp.cn

$s =~ s/old/new/g;
来源：http://gq.colortex.cn

[T49] Perl：函数
来源：http://vm.yuexingan06.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ns.szxytkj.cn

[T50] Perl：逐行读文件
来源：http://ne.chemitech.net.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://da.yuexingan06.cn

while (my $line = <$fh>) { print $line; }
来源：http://dk.yuntaijiaju.cn

[T51] Scala：Hello World
来源：http://qq.nszjky.cn

println("Hello")
来源：http://pp.wgjwhj.cn

[T52] Scala：变量
来源：http://mx.huanxung.cn

val a = 1;  var b = 2
来源：http://gd.shxzukj.cn

[T53] Scala：字符串插值
来源：http://yz.nicolike.cn

s"值: $b"
来源：http://lu.huanxung.cn

[T54] Scala：集合映射
来源：http://ko.bookmarksfly.cn

List(1, 2, 3).map(_ * 2)
来源：http://wn.jianghongdianzi.cn

[T55] Scala：集合过滤
来源：http://of.hnjuh.cn

List(1, 2, 3).filter(_ > 1)
来源：http://sd.bjjhwx.cn

[T56] Scala：样例类
来源：http://nb.jianghongdianzi.cn

case class User(name: String, age: Int)
来源：http://zk.huanxung.cn

[T57] Scala：模式匹配
来源：http://hg.nszjky.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vr.huixiangedu.cn

[T58] Scala：函数定义
来源：http://zv.hnjuh.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gr.szsharing.cn

[T59] Scala：循环
来源：http://ux.nszjky.cn

for (i <- 1 to 10) println(i)
来源：http://ic.hnjuh.cn

[T60] Scala：折叠
来源：http://jt.lnxyls.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xp.hahajie.cn

================================================================================
来源：http://ra.panjiajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hd.521024.cn

================================================================================
来源：http://zc.haigaiapp.cn

[U01] Py：创建虚拟环境
来源：http://uv.chemitech.net.cn

python -m venv .venv && source .venv/bin/activate
来源：http://tw.colortex.cn

[U02] Py：导出 / 安装依赖
来源：http://lu.huixiangedu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.panjiajie.cn

[U03] Py：加载 .env 配置
来源：http://gf.shtwfgs.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gr.muxihuayi.cn

[U04] Py：变量调试打印
来源：http://gu.newstarts.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sj.gzmigu.cn

[U05] Py：列表去重且保序
来源：http://su.haigaiapp.cn

list(dict.fromkeys(arr))
来源：http://ve.gzmigu.cn

[U06] Py：合并两个字典
来源：http://nb.shxzukj.cn

{**a, **b}
来源：http://wk.huixinmuqiang.cn

[U07] Py：反转字典键值
来源：http://uy.muxihuayi.cn

{v: k for k, v in d.items()}
来源：http://mo.huixiangedu.cn

[U08] Py：展平二维列表
来源：http://jr.521024.cn

[y for x in nested for y in x]
来源：http://nv.hnjuh.cn

[U09] Py：字典取最大值的键
来源：http://gd.huixiangedu.cn

max(d, key=d.get)
来源：http://xk.newstarts.cn

[U10] Py：按值排序字典
来源：http://qd.huixiangedu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cj.huixinmuqiang.cn

[U11] Py：生成器表达式
来源：http://vq.muxihuayi.cn

(x * 2 for x in arr)
来源：http://jl.chemitech.net.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ng.shxzskj.cn

Counter(arr).most_common(3)
来源：http://op.szsharing.cn

[U13] Py：固定长度队列
来源：http://wt.huixiangedu.cn

deque(maxlen=10)
来源：http://lo.nszjky.cn

[U14] Py：分组收集到列表
来源：http://nn.nicolike.cn

defaultdict(list)
来源：http://ib.huixiangedu.cn

[U15] Py：高精度计时
来源：http://ye.haigaiapp.cn

t = time.perf_counter()
来源：http://gc.yuexingan06.cn

[U16] Py：命令行参数解析
来源：http://kd.hahajie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ac.shxzukj.cn

[U17] Py：初始化日志
来源：http://cn.yuexingan06.cn

logging.basicConfig(level=logging.INFO)
来源：http://vm.colortex.cn

[U18] Py：预编译正则
来源：http://rm.newstarts.cn

pat = re.compile(r"\d+")
来源：http://hi.shxzskj.cn

[U19] Py：正则替换带回调
来源：http://xa.panjiajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ug.asd995.cn

[U20] Py：缓存函数结果
来源：http://wn.newstarts.cn

@functools.lru_cache(maxsize=None)
来源：http://bc.yuntaijiaju.cn

[U21] Py：自定义上下文管理器
来源：http://kl.asd995.cn

@contextlib.contextmanager
来源：http://lu.yuntaijiaju.cn

[U22] Py：矩阵转置
来源：http://oi.shxzukj.cn

list(zip(*m))
来源：http://yi.huixiangedu.cn

[U23] Py：分块读取大文件
来源：http://by.gzmigu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ma.newstarts.cn

[U24] Py：路径操作
来源：http://oq.521024.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://sw.jctech888.com.cn

[U25] Py：CSV 按字典读
来源：http://yh.muxihuayi.cn

csv.DictReader(f)
来源：http://dz.muxihuayi.cn

[U26] Py：并发下载
来源：http://oo.521024.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wm.nszjky.cn

[U27] Py：异步 HTTP
来源：http://vm.szsharing.cn

aiohttp.ClientSession() 配合 async with
来源：http://hk.bjjhwx.cn

[U28] Py：类型别名
来源：http://ug.muxihuayi.cn

UserId = int
来源：http://ke.bookmarksfly.cn

[U29] Py：属性校验
来源：http://ab.bjjhwx.cn

@property 与 @x.setter 配合
来源：http://nm.nszjky.cn

[U30] Py：数据类
来源：http://rg.yuexingan06.cn

@dataclass(slots=True)
来源：http://ds.newstarts.cn

[U31] Py：单测
来源：http://oi.hnjuh.cn

python -m pytest -q
来源：http://zi.muxihuayi.cn

[U32] Py：代码格式化
来源：http://kg.bjjhwx.cn

ruff format . && ruff check --fix .
来源：http://yr.shxzskj.cn

[U33] Py：打包发布
来源：http://bx.nicolike.cn

python -m build  （依赖 pyproject.toml）
来源：http://gp.panjiajie.cn

[U34] Py：判断编码
来源：http://fy.panjiajie.cn

chardet.detect(raw)
来源：http://vg.bookmarksfly.cn

[U35] Py：发送邮件
来源：http://hb.nszjky.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ow.hahajie.cn

[U36] Py：定时任务
来源：http://oq.hnjuh.cn

schedule.every(10).minutes.do(job)
来源：http://lz.shtwfgs.cn

[U37] Py：读写 Excel
来源：http://sq.shtwfgs.cn

pandas.read_excel / DataFrame.to_excel
来源：http://tb.shxzukj.cn

[U38] Py：获取脚本所在目录
来源：http://aj.gzmigu.cn

Path(__file__).resolve().parent
来源：http://ee.muxihuayi.cn

[U39] Py：判断是否在交互环境
来源：http://dt.shtwfgs.cn

sys.stdout.isatty()
来源：http://iz.muxihuayi.cn

[U40] Py：打印到标准错误
来源：http://xs.shtwfgs.cn

print("err", file=sys.stderr)
来源：http://rg.newstarts.cn

[U41] PHP：初始化 Composer 项目
来源：http://lh.panjiajie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://pt.hahajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://dp.nszjky.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pg.huanxung.cn

[U43] PHP：声明命名空间
来源：http://tt.hnjuh.cn

namespace App\Http;
来源：http://eh.wgjwhj.cn

[U44] PHP：开启严格类型
来源：http://ix.newstarts.cn

declare(strict_types=1);
来源：http://mp.colortex.cn

[U45] PHP：类型声明与返回类型
来源：http://cn.bookmarksfly.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://at.szsharing.cn

[U46] PHP：可空类型
来源：http://rc.nszjky.cn

?string $name = null
来源：http://qy.9csxet.cn

[U47] PHP：联合类型
来源：http://jx.bookmarksfly.cn

int|string $id
来源：http://vf.9csxet.cn

[U48] PHP：纯枚举
来源：http://bb.haigaiapp.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ol.szxytkj.cn

[U49] PHP：只读属性
来源：http://vn.jianghongdianzi.cn

public readonly string $name
来源：http://xx.asd995.cn

[U50] PHP：构造器属性提升
来源：http://ym.asd995.cn

public function __construct(private int $id) {}
来源：http://of.colortex.cn

[U51] PHP：数组解构
来源：http://bj.nicolike.cn

[$a, $b] = $arr;
来源：http://on.szsharing.cn

[U52] PHP：箭头函数
来源：http://ob.lnxyls.cn

$double = fn($x) => $x * 2;
来源：http://fa.9csxet.cn

[U53] PHP：空合并运算符
来源：http://no.newstarts.cn

$v = $a ?? $b ?? "default";
来源：http://lh.wgjwhj.cn

[U54] PHP：空安全调用
来源：http://ai.hahajie.cn

$obj?->method()
来源：http://pm.hahajie.cn

[U55] PHP：match 表达式
来源：http://yr.newstarts.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://su.yuexingan06.cn

[U56] PHP：命名参数
来源：http://ou.huanxung.cn

f(a: 1, b: 2)
来源：http://ep.lnxyls.cn

[U57] PHP：字符串插值
来源：http://zr.huixinmuqiang.cn

"值: {$a}"
来源：http://vr.panjiajie.cn

[U58] PHP：数组三件套
来源：http://mv.bookmarksfly.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ba.huanxung.cn

[U59] PHP：自定义排序
来源：http://mj.9csxet.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rq.haigaiapp.cn

[U60] PHP：JSON 编解码
来源：http://ov.yuntaijiaju.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://uf.shtwfgs.cn

[U61] PHP：正则
来源：http://wk.bookmarksfly.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tc.jianghongdianzi.cn

[U62] PHP：日期对象
来源：http://ki.521024.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rw.yuexingan06.cn

[U63] PHP：文件读写
来源：http://dr.nicolike.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vx.panjiajie.cn

[U64] PHP：目录遍历
来源：http://kh.shxzukj.cn

glob("dir/*.php");  scandir("dir");
来源：http://pn.shxzskj.cn

[U65] PHP：会话
来源：http://ft.panjiajie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://qg.lnxyls.cn

[U66] PHP：设置 Cookie
来源：http://hw.shxzukj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xr.panjiajie.cn

[U67] PHP：处理文件上传
来源：http://xy.chemitech.net.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pr.hnjuh.cn

[U68] PHP：PDO 连接
来源：http://sd.9csxet.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://li.colortex.cn

[U69] PHP：PDO 预处理
来源：http://zi.haigaiapp.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fa.haigaiapp.cn

[U70] PHP：PDO 事务
来源：http://ny.yuexingan06.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pz.haigaiapp.cn

[U71] PHP：抛出异常
来源：http://cr.szxytkj.cn

throw new RuntimeException("失败", 500);
来源：http://ag.hnjuh.cn

[U72] PHP：写错误日志
来源：http://dw.bjjhwx.cn

error_log("失败: " . $e->getMessage());
来源：http://qu.colortex.cn

[U73] PHP：读取 ini 配置
来源：http://mw.shxzukj.cn

parse_ini_file("config.ini", true)
来源：http://au.hahajie.cn

[U74] PHP：读取环境变量
来源：http://qj.wgjwhj.cn

getenv("APP_ENV") ?: "production"
来源：http://cr.lnxyls.cn

[U75] PHP：依赖注入
来源：http://vt.chemitech.net.cn

composer require psr/container
来源：http://zs.huixiangedu.cn

[U76] PHP：简单路由
来源：http://gk.panjiajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fg.bjjhwx.cn

[U77] PHP：模板渲染
来源：http://mn.shxzskj.cn

composer require twig/twig
来源：http://do.9csxet.cn

[U78] PHP：单元测试
来源：http://jr.chemitech.net.cn

composer require --dev phpunit/phpunit
来源：http://ay.shtwfgs.cn

[U79] PHP：静态分析
来源：http://pl.hnjuh.cn

composer require --dev phpstan/phpstan
来源：http://rr.jianghongdianzi.cn

[U80] PHP：代码规范修复
来源：http://ha.shxzukj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://st.chemitech.net.cn

[U81] JS：初始化项目
来源：http://tz.huixinmuqiang.cn

npm init -y;  npm i express
来源：http://mh.shxzskj.cn

[U82] JS：package.json 脚本
来源：http://sq.nicolike.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://va.huixiangedu.cn

[U83] JS：ES Module 导入导出
来源：http://ey.shxzukj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ax.shxzskj.cn

[U84] JS：CommonJS 写法
来源：http://jl.9csxet.cn

module.exports = { a };  const { a } = require("./m");
来源：http://it.huanxung.cn

[U85] JS：可选链
来源：http://hb.colortex.cn

a?.b?.c
来源：http://wq.nszjky.cn

[U86] JS：空值合并
来源：http://gy.yuexingan06.cn

a ?? b
来源：http://as.yuexingan06.cn

[U87] JS：解构默认值
来源：http://so.hnjuh.cn

const { a = 1, b = 2 } = obj;
来源：http://kn.huanxung.cn

[U88] JS：对象展开合并
来源：http://if.asd995.cn

{ ...a, ...b }
来源：http://lj.colortex.cn

[U89] JS：数组去重
来源：http://kz.haigaiapp.cn

[...new Set(arr)]
来源：http://lh.chemitech.net.cn

[U90] JS：数字数组排序
来源：http://oc.asd995.cn

[...arr].sort((a, b) => a - b)
来源：http://sj.shxzskj.cn

[U91] JS：对象键值遍历
来源：http://kf.9csxet.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ux.shxzukj.cn

[U92] JS：深拷贝
来源：http://rk.jctech888.com.cn

structuredClone(obj)
来源：http://ew.9csxet.cn

[U93] JS：模板字符串
来源：http://dt.hnjuh.cn

`共 ${n} 条`
来源：http://oe.haigaiapp.cn

[U94] JS：箭头函数
来源：http://kn.shxzskj.cn

const double = x => x * 2;
来源：http://be.haigaiapp.cn

[U95] JS：Promise 包装
来源：http://od.hahajie.cn

new Promise((resolve, reject) => {})
来源：http://po.jctech888.com.cn

[U96] JS：async/await 与异常
来源：http://ew.colortex.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dj.huixinmuqiang.cn

[U97] JS：并发请求
来源：http://rh.huixiangedu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://tb.hnjuh.cn

[U98] JS：fetch 带 JSON
来源：http://qz.gzmigu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xt.jianghongdianzi.cn

[U99] JS：事件监听
来源：http://sv.szsharing.cn

el.addEventListener("click", e => {})
来源：http://zf.shxzskj.cn

[U100] JS：DOM 查询
来源：http://wm.chemitech.net.cn

document.querySelector(".item")
来源：http://ry.huanxung.cn

[U101] JS：classList 操作
来源：http://bu.jianghongdianzi.cn

el.classList.toggle("active")
来源：http://st.bookmarksfly.cn

[U102] JS：本地存储
来源：http://ca.asd995.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://vs.huixiangedu.cn

[U103] JS：定时器
来源：http://av.jctech888.com.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kk.yuexingan06.cn

[U104] JS：防抖
来源：http://ol.newstarts.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mi.nicolike.cn

[U105] JS：节流
来源：http://uf.lnxyls.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kb.bjjhwx.cn

[U106] JS：日期格式化
来源：http://lo.jianghongdianzi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dy.chemitech.net.cn

[U107] JS：数字千分位
来源：http://wu.szxytkj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ki.hahajie.cn

[U108] JS：随机整数
来源：http://gn.yuexingan06.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cm.bjjhwx.cn

[U109] JS：数组分组
来源：http://yl.shxzskj.cn

Object.groupBy(arr, x => x.type)
来源：http://bv.szxytkj.cn

[U110] JS：数组分块
来源：http://ni.yuntaijiaju.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gy.jctech888.com.cn

[U111] JS：对象转 Map
来源：http://gj.gzmigu.cn

new Map(Object.entries(obj))
来源：http://fq.shxzskj.cn

[U112] JS：字符串补位
来源：http://vd.shxzukj.cn

"7".padStart(3, "0")
来源：http://ot.jianghongdianzi.cn

[U113] JS：正则替换全部
来源：http://ll.nicolike.cn

s.replaceAll("a", "b")
来源：http://fo.jctech888.com.cn

[U114] JS：JSON 深比较
来源：http://vb.haigaiapp.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://yy.hahajie.cn

[U115] JS：生成 UUID
来源：http://xh.huanxung.cn

crypto.randomUUID()
来源：http://ga.szxytkj.cn

[U116] JS：类型检查（JSDoc）
来源：http://zy.huixinmuqiang.cn

/** @param {string} name */ function f(name) {}
来源：http://hu.asd995.cn

[U117] JS：单元测试
来源：http://lh.haigaiapp.cn

npm i -D vitest;  npx vitest
来源：http://eh.newstarts.cn

[U118] JS：开发服务器
来源：http://no.shxzskj.cn

npm i -D vite;  npx vite
来源：http://uv.huanxung.cn

[U119] JS：生产构建
来源：http://cj.521024.cn

npx vite build
来源：http://tq.panjiajie.cn

[U120] JS：读取环境变量（Vite）
来源：http://cb.chemitech.net.cn

import.meta.env.VITE_API_URL
来源：http://ah.jctech888.com.cn

================================================================================
来源：http://mn.huixinmuqiang.cn

统计汇总
来源：http://cl.szsharing.cn

================================================================================
来源：http://xw.panjiajie.cn

按语言统计（条）：
来源：http://rp.panjiajie.cn


<!-- 参考信息 -->