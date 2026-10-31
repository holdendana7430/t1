代发 wailian999

[T29] Swift：guard 提前返回
来源：http://mj.panjiajie.cn

guard let x = opt else { return }
来源：http://pm.nszjky.cn

[T30] Swift：协议
来源：http://iy.huixinmuqiang.cn

protocol Shape { func area() -> Double }
来源：http://oa.yuntaijiaju.cn

[T31] Lua：Hello World
来源：http://jq.wgjwhj.cn

print("Hello")
来源：http://vs.gzmigu.cn

[T32] Lua：局部变量
来源：http://if.huixiangedu.cn

local a = 1
来源：http://ef.huixiangedu.cn

[T33] Lua：表（数组）
来源：http://mk.521024.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://eb.yuntaijiaju.cn

[T34] Lua：遍历表
来源：http://xg.jctech888.com.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://eg.521024.cn

[T35] Lua：字典表
来源：http://lk.shtwfgs.cn

local d = { a = 1 };  d.b = 2
来源：http://rw.bjjhwx.cn

[T36] Lua：函数
来源：http://td.jctech888.com.cn

function add(a, b) return a + b end
来源：http://yh.gzmigu.cn

[T37] Lua：字符串拼接
来源：http://cd.colortex.cn

"a" .. "b"
来源：http://ov.gzmigu.cn

[T38] Lua：条件
来源：http://mw.chemitech.net.cn

if x > 0 then print("正") end
来源：http://hx.wgjwhj.cn

[T39] Lua：模式匹配
来源：http://be.nszjky.cn

string.find(s, "%d+")
来源：http://tq.huixiangedu.cn

[T40] Lua：元表
来源：http://fv.yuexingan06.cn

setmetatable({}, { __index = base })
来源：http://oj.jianghongdianzi.cn

[T41] Perl：Hello World
来源：http://go.hnjuh.cn

print "Hello\n";
来源：http://lz.shtwfgs.cn

[T42] Perl：变量类型
来源：http://qi.jctech888.com.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ma.lnxyls.cn

[T43] Perl：字符串插值
来源：http://gg.colortex.cn

"值: $a"
来源：http://vp.colortex.cn

[T44] Perl：条件
来源：http://vp.huanxung.cn

if ($a > 0) { print "正"; }
来源：http://cm.yuexingan06.cn

[T45] Perl：数组遍历
来源：http://pg.9csxet.cn

for my $x (@arr) { print $x; }
来源：http://he.jianghongdianzi.cn

[T46] Perl：哈希操作
来源：http://xh.szsharing.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vf.huixinmuqiang.cn

[T47] Perl：正则捕获
来源：http://bm.yuexingan06.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rs.shxzukj.cn

[T48] Perl：正则替换
来源：http://le.newstarts.cn

$s =~ s/old/new/g;
来源：http://ed.9csxet.cn

[T49] Perl：函数
来源：http://ly.huixinmuqiang.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ee.jctech888.com.cn

[T50] Perl：逐行读文件
来源：http://rl.chemitech.net.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rd.newstarts.cn

while (my $line = <$fh>) { print $line; }
来源：http://li.asd995.cn

[T51] Scala：Hello World
来源：http://pk.jctech888.com.cn

println("Hello")
来源：http://wr.shxzskj.cn

[T52] Scala：变量
来源：http://xw.bookmarksfly.cn

val a = 1;  var b = 2
来源：http://nr.colortex.cn

[T53] Scala：字符串插值
来源：http://zg.huixinmuqiang.cn

s"值: $b"
来源：http://dc.hnjuh.cn

[T54] Scala：集合映射
来源：http://gk.lnxyls.cn

List(1, 2, 3).map(_ * 2)
来源：http://hk.newstarts.cn

[T55] Scala：集合过滤
来源：http://kc.shtwfgs.cn

List(1, 2, 3).filter(_ > 1)
来源：http://la.chemitech.net.cn

[T56] Scala：样例类
来源：http://wa.huixiangedu.cn

case class User(name: String, age: Int)
来源：http://ps.haigaiapp.cn

[T57] Scala：模式匹配
来源：http://ot.521024.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://bt.bookmarksfly.cn

[T58] Scala：函数定义
来源：http://ab.wgjwhj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://sg.yuntaijiaju.cn

[T59] Scala：循环
来源：http://jf.hnjuh.cn

for (i <- 1 to 10) println(i)
来源：http://vh.lnxyls.cn

[T60] Scala：折叠
来源：http://lb.yuexingan06.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lk.huanxung.cn

================================================================================
来源：http://zv.jianghongdianzi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vt.lnxyls.cn

================================================================================
来源：http://fg.huanxung.cn

[U01] Py：创建虚拟环境
来源：http://to.wgjwhj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://xc.hnjuh.cn

[U02] Py：导出 / 安装依赖
来源：http://yv.nszjky.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ve.yuexingan06.cn

[U03] Py：加载 .env 配置
来源：http://aw.hahajie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://yn.jianghongdianzi.cn

[U04] Py：变量调试打印
来源：http://oz.nicolike.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qg.huixiangedu.cn

[U05] Py：列表去重且保序
来源：http://hy.shxzskj.cn

list(dict.fromkeys(arr))
来源：http://nz.bookmarksfly.cn

[U06] Py：合并两个字典
来源：http://vw.huixiangedu.cn

{**a, **b}
来源：http://vu.yuntaijiaju.cn

[U07] Py：反转字典键值
来源：http://ud.521024.cn

{v: k for k, v in d.items()}
来源：http://zm.haigaiapp.cn

[U08] Py：展平二维列表
来源：http://ct.hahajie.cn

[y for x in nested for y in x]
来源：http://cq.hnjuh.cn

[U09] Py：字典取最大值的键
来源：http://zk.huanxung.cn

max(d, key=d.get)
来源：http://tp.szxytkj.cn

[U10] Py：按值排序字典
来源：http://hj.nszjky.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jr.nszjky.cn

[U11] Py：生成器表达式
来源：http://np.yuntaijiaju.cn

(x * 2 for x in arr)
来源：http://ix.wgjwhj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://gc.nicolike.cn

Counter(arr).most_common(3)
来源：http://zv.9csxet.cn

[U13] Py：固定长度队列
来源：http://vv.bookmarksfly.cn

deque(maxlen=10)
来源：http://ze.huixinmuqiang.cn

[U14] Py：分组收集到列表
来源：http://ef.521024.cn

defaultdict(list)
来源：http://ds.chemitech.net.cn

[U15] Py：高精度计时
来源：http://zg.yuexingan06.cn

t = time.perf_counter()
来源：http://ml.shxzskj.cn

[U16] Py：命令行参数解析
来源：http://gy.haigaiapp.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hv.nicolike.cn

[U17] Py：初始化日志
来源：http://mp.shtwfgs.cn

logging.basicConfig(level=logging.INFO)
来源：http://sr.huixiangedu.cn

[U18] Py：预编译正则
来源：http://ma.jianghongdianzi.cn

pat = re.compile(r"\d+")
来源：http://xy.huixinmuqiang.cn

[U19] Py：正则替换带回调
来源：http://ps.asd995.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pi.shxzukj.cn

[U20] Py：缓存函数结果
来源：http://bd.bookmarksfly.cn

@functools.lru_cache(maxsize=None)
来源：http://yj.shtwfgs.cn

[U21] Py：自定义上下文管理器
来源：http://hc.hahajie.cn

@contextlib.contextmanager
来源：http://dd.bookmarksfly.cn

[U22] Py：矩阵转置
来源：http://do.jianghongdianzi.cn

list(zip(*m))
来源：http://ou.shtwfgs.cn

[U23] Py：分块读取大文件
来源：http://ri.nicolike.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xn.bjjhwx.cn

[U24] Py：路径操作
来源：http://ob.shxzukj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jh.shxzukj.cn

[U25] Py：CSV 按字典读
来源：http://pg.bookmarksfly.cn

csv.DictReader(f)
来源：http://db.bjjhwx.cn

[U26] Py：并发下载
来源：http://kr.newstarts.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zk.shxzukj.cn

[U27] Py：异步 HTTP
来源：http://mw.haigaiapp.cn

aiohttp.ClientSession() 配合 async with
来源：http://mr.bookmarksfly.cn

[U28] Py：类型别名
来源：http://vs.huixinmuqiang.cn

UserId = int
来源：http://vi.muxihuayi.cn

[U29] Py：属性校验
来源：http://ga.jianghongdianzi.cn

@property 与 @x.setter 配合
来源：http://bz.521024.cn

[U30] Py：数据类
来源：http://ax.nicolike.cn

@dataclass(slots=True)
来源：http://cc.bjjhwx.cn

[U31] Py：单测
来源：http://xf.gzmigu.cn

python -m pytest -q
来源：http://nt.yuexingan06.cn

[U32] Py：代码格式化
来源：http://dp.hahajie.cn

ruff format . && ruff check --fix .
来源：http://bt.nicolike.cn

[U33] Py：打包发布
来源：http://cr.jctech888.com.cn

python -m build  （依赖 pyproject.toml）
来源：http://hj.shtwfgs.cn

[U34] Py：判断编码
来源：http://mq.muxihuayi.cn

chardet.detect(raw)
来源：http://pq.521024.cn

[U35] Py：发送邮件
来源：http://lo.nszjky.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vv.yuntaijiaju.cn

[U36] Py：定时任务
来源：http://xl.huanxung.cn

schedule.every(10).minutes.do(job)
来源：http://rc.shtwfgs.cn

[U37] Py：读写 Excel
来源：http://ae.nszjky.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ls.521024.cn

[U38] Py：获取脚本所在目录
来源：http://jq.nszjky.cn

Path(__file__).resolve().parent
来源：http://qx.yuexingan06.cn

[U39] Py：判断是否在交互环境
来源：http://hf.hahajie.cn

sys.stdout.isatty()
来源：http://ao.muxihuayi.cn

[U40] Py：打印到标准错误
来源：http://fl.lnxyls.cn

print("err", file=sys.stderr)
来源：http://ie.huixinmuqiang.cn

[U41] PHP：初始化 Composer 项目
来源：http://nz.huixinmuqiang.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xj.shxzukj.cn

[U42] PHP：PSR-4 自动加载
来源：http://ys.jianghongdianzi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ag.yuexingan06.cn

[U43] PHP：声明命名空间
来源：http://yr.bjjhwx.cn

namespace App\Http;
来源：http://sw.newstarts.cn

[U44] PHP：开启严格类型
来源：http://vh.hnjuh.cn

declare(strict_types=1);
来源：http://ob.9csxet.cn

[U45] PHP：类型声明与返回类型
来源：http://er.jianghongdianzi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://yk.jctech888.com.cn

[U46] PHP：可空类型
来源：http://hj.haigaiapp.cn

?string $name = null
来源：http://rv.asd995.cn

[U47] PHP：联合类型
来源：http://cq.chemitech.net.cn

int|string $id
来源：http://cv.shtwfgs.cn

[U48] PHP：纯枚举
来源：http://oc.yuntaijiaju.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ey.521024.cn

[U49] PHP：只读属性
来源：http://vt.shtwfgs.cn

public readonly string $name
来源：http://av.huixinmuqiang.cn

[U50] PHP：构造器属性提升
来源：http://jm.huixiangedu.cn

public function __construct(private int $id) {}
来源：http://qm.haigaiapp.cn

[U51] PHP：数组解构
来源：http://pn.nszjky.cn

[$a, $b] = $arr;
来源：http://ch.shxzskj.cn

[U52] PHP：箭头函数
来源：http://og.jianghongdianzi.cn

$double = fn($x) => $x * 2;
来源：http://xl.wgjwhj.cn

[U53] PHP：空合并运算符
来源：http://if.shtwfgs.cn

$v = $a ?? $b ?? "default";
来源：http://in.huixiangedu.cn

[U54] PHP：空安全调用
来源：http://nr.huanxung.cn

$obj?->method()
来源：http://er.lnxyls.cn

[U55] PHP：match 表达式
来源：http://wt.hahajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zt.jianghongdianzi.cn

[U56] PHP：命名参数
来源：http://fw.huanxung.cn

f(a: 1, b: 2)
来源：http://ch.wgjwhj.cn

[U57] PHP：字符串插值
来源：http://wf.nicolike.cn

"值: {$a}"
来源：http://sb.lnxyls.cn

[U58] PHP：数组三件套
来源：http://sl.jctech888.com.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hj.newstarts.cn

[U59] PHP：自定义排序
来源：http://ee.chemitech.net.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ta.shxzukj.cn

[U60] PHP：JSON 编解码
来源：http://fx.huanxung.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ab.chemitech.net.cn

[U61] PHP：正则
来源：http://iv.lnxyls.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gg.shxzskj.cn

[U62] PHP：日期对象
来源：http://cg.bookmarksfly.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bs.gzmigu.cn

[U63] PHP：文件读写
来源：http://tk.huanxung.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xf.huanxung.cn

[U64] PHP：目录遍历
来源：http://db.huanxung.cn

glob("dir/*.php");  scandir("dir");
来源：http://ls.hnjuh.cn

[U65] PHP：会话
来源：http://kj.jctech888.com.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ft.521024.cn

[U66] PHP：设置 Cookie
来源：http://tp.asd995.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fo.shtwfgs.cn

[U67] PHP：处理文件上传
来源：http://bs.huixiangedu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://os.nicolike.cn

[U68] PHP：PDO 连接
来源：http://ea.szsharing.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://my.shtwfgs.cn

[U69] PHP：PDO 预处理
来源：http://tj.521024.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pd.colortex.cn

[U70] PHP：PDO 事务
来源：http://yn.hahajie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dy.shtwfgs.cn

[U71] PHP：抛出异常
来源：http://am.szxytkj.cn

throw new RuntimeException("失败", 500);
来源：http://yp.hnjuh.cn

[U72] PHP：写错误日志
来源：http://rr.huixiangedu.cn

error_log("失败: " . $e->getMessage());
来源：http://hg.panjiajie.cn

[U73] PHP：读取 ini 配置
来源：http://pl.shxzskj.cn

parse_ini_file("config.ini", true)
来源：http://id.521024.cn

[U74] PHP：读取环境变量
来源：http://er.asd995.cn

getenv("APP_ENV") ?: "production"
来源：http://by.nicolike.cn

[U75] PHP：依赖注入
来源：http://ij.muxihuayi.cn

composer require psr/container
来源：http://qb.gzmigu.cn

[U76] PHP：简单路由
来源：http://ro.szsharing.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yw.jctech888.com.cn

[U77] PHP：模板渲染
来源：http://nk.shxzskj.cn

composer require twig/twig
来源：http://te.nszjky.cn

[U78] PHP：单元测试
来源：http://sc.yuntaijiaju.cn

composer require --dev phpunit/phpunit
来源：http://ay.yuntaijiaju.cn

[U79] PHP：静态分析
来源：http://ch.panjiajie.cn

composer require --dev phpstan/phpstan
来源：http://tc.9csxet.cn

[U80] PHP：代码规范修复
来源：http://zz.shtwfgs.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://vt.yuntaijiaju.cn

[U81] JS：初始化项目
来源：http://se.nicolike.cn

npm init -y;  npm i express
来源：http://dl.newstarts.cn

[U82] JS：package.json 脚本
来源：http://yv.jianghongdianzi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rz.521024.cn

[U83] JS：ES Module 导入导出
来源：http://qz.gzmigu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://fw.bookmarksfly.cn

[U84] JS：CommonJS 写法
来源：http://dq.yuexingan06.cn

module.exports = { a };  const { a } = require("./m");
来源：http://mb.huixiangedu.cn

[U85] JS：可选链
来源：http://rf.bjjhwx.cn

a?.b?.c
来源：http://om.hahajie.cn

[U86] JS：空值合并
来源：http://mz.bjjhwx.cn

a ?? b
来源：http://nv.newstarts.cn

[U87] JS：解构默认值
来源：http://kv.yuntaijiaju.cn

const { a = 1, b = 2 } = obj;
来源：http://ab.hahajie.cn

[U88] JS：对象展开合并
来源：http://kd.lnxyls.cn

{ ...a, ...b }
来源：http://nq.colortex.cn

[U89] JS：数组去重
来源：http://yv.bjjhwx.cn

[...new Set(arr)]
来源：http://hw.shxzukj.cn

[U90] JS：数字数组排序
来源：http://ay.asd995.cn

[...arr].sort((a, b) => a - b)
来源：http://sj.521024.cn

[U91] JS：对象键值遍历
来源：http://hi.nicolike.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bi.nszjky.cn

[U92] JS：深拷贝
来源：http://tq.panjiajie.cn

structuredClone(obj)
来源：http://bc.newstarts.cn

[U93] JS：模板字符串
来源：http://zd.9csxet.cn

`共 ${n} 条`
来源：http://vu.huanxung.cn

[U94] JS：箭头函数
来源：http://mw.wgjwhj.cn

const double = x => x * 2;
来源：http://um.shxzskj.cn

[U95] JS：Promise 包装
来源：http://md.newstarts.cn

new Promise((resolve, reject) => {})
来源：http://jj.nszjky.cn

[U96] JS：async/await 与异常
来源：http://ta.newstarts.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://df.9csxet.cn

[U97] JS：并发请求
来源：http://mu.nszjky.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://pm.yuntaijiaju.cn

[U98] JS：fetch 带 JSON
来源：http://tc.muxihuayi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rc.panjiajie.cn

[U99] JS：事件监听
来源：http://rf.521024.cn

el.addEventListener("click", e => {})
来源：http://ed.nicolike.cn

[U100] JS：DOM 查询
来源：http://yv.huixiangedu.cn

document.querySelector(".item")
来源：http://ca.wgjwhj.cn

[U101] JS：classList 操作
来源：http://kw.hahajie.cn

el.classList.toggle("active")
来源：http://ke.panjiajie.cn

[U102] JS：本地存储
来源：http://mf.shtwfgs.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://gd.haigaiapp.cn

[U103] JS：定时器
来源：http://tk.jianghongdianzi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dc.521024.cn

[U104] JS：防抖
来源：http://np.huixiangedu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://md.521024.cn

[U105] JS：节流
来源：http://ko.9csxet.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lz.521024.cn

[U106] JS：日期格式化
来源：http://be.9csxet.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://he.jctech888.com.cn

[U107] JS：数字千分位
来源：http://oo.shxzukj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vu.nszjky.cn

[U108] JS：随机整数
来源：http://gt.shxzukj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://or.szsharing.cn

[U109] JS：数组分组
来源：http://id.shxzskj.cn

Object.groupBy(arr, x => x.type)
来源：http://bp.lnxyls.cn

[U110] JS：数组分块
来源：http://ct.bjjhwx.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ou.gzmigu.cn

[U111] JS：对象转 Map
来源：http://eh.hahajie.cn

new Map(Object.entries(obj))
来源：http://rp.lnxyls.cn

[U112] JS：字符串补位
来源：http://kw.szsharing.cn

"7".padStart(3, "0")
来源：http://ty.yuntaijiaju.cn

[U113] JS：正则替换全部
来源：http://va.shxzskj.cn

s.replaceAll("a", "b")
来源：http://ei.asd995.cn

[U114] JS：JSON 深比较
来源：http://oa.szsharing.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://wn.lnxyls.cn

[U115] JS：生成 UUID
来源：http://wi.szsharing.cn

crypto.randomUUID()
来源：http://tv.colortex.cn

[U116] JS：类型检查（JSDoc）
来源：http://dq.yuntaijiaju.cn

/** @param {string} name */ function f(name) {}
来源：http://qz.panjiajie.cn


<!-- 参考信息 -->