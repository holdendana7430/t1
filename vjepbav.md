代发 wailian999

[T29] Swift：guard 提前返回
来源：http://wj.newstarts.cn

guard let x = opt else { return }
来源：http://qh.yuntaijiaju.cn

[T30] Swift：协议
来源：http://mb.muxihuayi.cn

protocol Shape { func area() -> Double }
来源：http://ni.9csxet.cn

[T31] Lua：Hello World
来源：http://iz.shxzskj.cn

print("Hello")
来源：http://cr.9csxet.cn

[T32] Lua：局部变量
来源：http://dt.jctech888.com.cn

local a = 1
来源：http://rw.szsharing.cn

[T33] Lua：表（数组）
来源：http://ko.nicolike.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://oh.szsharing.cn

[T34] Lua：遍历表
来源：http://zv.panjiajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://uq.hnjuh.cn

[T35] Lua：字典表
来源：http://ix.newstarts.cn

local d = { a = 1 };  d.b = 2
来源：http://ku.colortex.cn

[T36] Lua：函数
来源：http://zb.yuntaijiaju.cn

function add(a, b) return a + b end
来源：http://zc.shtwfgs.cn

[T37] Lua：字符串拼接
来源：http://xm.521024.cn

"a" .. "b"
来源：http://wg.yuexingan06.cn

[T38] Lua：条件
来源：http://rt.hnjuh.cn

if x > 0 then print("正") end
来源：http://rg.szsharing.cn

[T39] Lua：模式匹配
来源：http://mq.gzmigu.cn

string.find(s, "%d+")
来源：http://vu.jianghongdianzi.cn

[T40] Lua：元表
来源：http://tk.bjjhwx.cn

setmetatable({}, { __index = base })
来源：http://th.521024.cn

[T41] Perl：Hello World
来源：http://kh.yuexingan06.cn

print "Hello\n";
来源：http://le.shtwfgs.cn

[T42] Perl：变量类型
来源：http://wt.bjjhwx.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ac.shxzukj.cn

[T43] Perl：字符串插值
来源：http://gp.jianghongdianzi.cn

"值: $a"
来源：http://bw.newstarts.cn

[T44] Perl：条件
来源：http://wb.jctech888.com.cn

if ($a > 0) { print "正"; }
来源：http://wi.szxytkj.cn

[T45] Perl：数组遍历
来源：http://wf.chemitech.net.cn

for my $x (@arr) { print $x; }
来源：http://xu.521024.cn

[T46] Perl：哈希操作
来源：http://ry.colortex.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kh.wgjwhj.cn

[T47] Perl：正则捕获
来源：http://th.szxytkj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://gx.szxytkj.cn

[T48] Perl：正则替换
来源：http://bx.nszjky.cn

$s =~ s/old/new/g;
来源：http://te.yuexingan06.cn

[T49] Perl：函数
来源：http://wv.lnxyls.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ab.huixinmuqiang.cn

[T50] Perl：逐行读文件
来源：http://hp.521024.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zi.jctech888.com.cn

while (my $line = <$fh>) { print $line; }
来源：http://pu.muxihuayi.cn

[T51] Scala：Hello World
来源：http://ig.521024.cn

println("Hello")
来源：http://lc.asd995.cn

[T52] Scala：变量
来源：http://eg.asd995.cn

val a = 1;  var b = 2
来源：http://kc.colortex.cn

[T53] Scala：字符串插值
来源：http://kg.haigaiapp.cn

s"值: $b"
来源：http://gi.shxzskj.cn

[T54] Scala：集合映射
来源：http://wi.hahajie.cn

List(1, 2, 3).map(_ * 2)
来源：http://gs.asd995.cn

[T55] Scala：集合过滤
来源：http://ya.muxihuayi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://hv.shxzukj.cn

[T56] Scala：样例类
来源：http://wd.szxytkj.cn

case class User(name: String, age: Int)
来源：http://mt.huanxung.cn

[T57] Scala：模式匹配
来源：http://lf.wgjwhj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wp.hahajie.cn

[T58] Scala：函数定义
来源：http://do.jctech888.com.cn

def add(a: Int, b: Int): Int = a + b
来源：http://qr.lnxyls.cn

[T59] Scala：循环
来源：http://wd.huixinmuqiang.cn

for (i <- 1 to 10) println(i)
来源：http://ih.hnjuh.cn

[T60] Scala：折叠
来源：http://gy.shxzukj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jv.huixiangedu.cn

================================================================================
来源：http://rp.jianghongdianzi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://aa.hahajie.cn

================================================================================
来源：http://ch.huixiangedu.cn

[U01] Py：创建虚拟环境
来源：http://ba.nicolike.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qw.shxzukj.cn

[U02] Py：导出 / 安装依赖
来源：http://za.lnxyls.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cp.yuexingan06.cn

[U03] Py：加载 .env 配置
来源：http://fg.huixiangedu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://py.asd995.cn

[U04] Py：变量调试打印
来源：http://hx.lnxyls.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wa.newstarts.cn

[U05] Py：列表去重且保序
来源：http://dp.9csxet.cn

list(dict.fromkeys(arr))
来源：http://lh.521024.cn

[U06] Py：合并两个字典
来源：http://dl.chemitech.net.cn

{**a, **b}
来源：http://zg.chemitech.net.cn

[U07] Py：反转字典键值
来源：http://ks.panjiajie.cn

{v: k for k, v in d.items()}
来源：http://dd.shxzukj.cn

[U08] Py：展平二维列表
来源：http://cq.nicolike.cn

[y for x in nested for y in x]
来源：http://id.9csxet.cn

[U09] Py：字典取最大值的键
来源：http://zl.shxzskj.cn

max(d, key=d.get)
来源：http://rs.colortex.cn

[U10] Py：按值排序字典
来源：http://iz.szxytkj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mo.bjjhwx.cn

[U11] Py：生成器表达式
来源：http://rk.shxzskj.cn

(x * 2 for x in arr)
来源：http://gp.yuexingan06.cn

[U12] Py：取出现最多的 3 个元素
来源：http://yw.wgjwhj.cn

Counter(arr).most_common(3)
来源：http://rt.huanxung.cn

[U13] Py：固定长度队列
来源：http://yp.huixiangedu.cn

deque(maxlen=10)
来源：http://bz.haigaiapp.cn

[U14] Py：分组收集到列表
来源：http://yl.szxytkj.cn

defaultdict(list)
来源：http://mp.jianghongdianzi.cn

[U15] Py：高精度计时
来源：http://zk.bjjhwx.cn

t = time.perf_counter()
来源：http://sj.shxzukj.cn

[U16] Py：命令行参数解析
来源：http://vt.szxytkj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vx.haigaiapp.cn

[U17] Py：初始化日志
来源：http://gn.nicolike.cn

logging.basicConfig(level=logging.INFO)
来源：http://gf.huanxung.cn

[U18] Py：预编译正则
来源：http://ji.521024.cn

pat = re.compile(r"\d+")
来源：http://xu.huixiangedu.cn

[U19] Py：正则替换带回调
来源：http://fs.hnjuh.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rh.jctech888.com.cn

[U20] Py：缓存函数结果
来源：http://xk.jctech888.com.cn

@functools.lru_cache(maxsize=None)
来源：http://pu.huanxung.cn

[U21] Py：自定义上下文管理器
来源：http://tw.colortex.cn

@contextlib.contextmanager
来源：http://za.521024.cn

[U22] Py：矩阵转置
来源：http://hg.huixiangedu.cn

list(zip(*m))
来源：http://zn.panjiajie.cn

[U23] Py：分块读取大文件
来源：http://sm.huanxung.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pa.panjiajie.cn

[U24] Py：路径操作
来源：http://ms.hahajie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jv.newstarts.cn

[U25] Py：CSV 按字典读
来源：http://bo.huixiangedu.cn

csv.DictReader(f)
来源：http://kt.haigaiapp.cn

[U26] Py：并发下载
来源：http://yi.hahajie.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hs.szsharing.cn

[U27] Py：异步 HTTP
来源：http://yw.shxzukj.cn

aiohttp.ClientSession() 配合 async with
来源：http://ac.yuexingan06.cn

[U28] Py：类型别名
来源：http://qd.chemitech.net.cn

UserId = int
来源：http://hq.9csxet.cn

[U29] Py：属性校验
来源：http://df.wgjwhj.cn

@property 与 @x.setter 配合
来源：http://wb.asd995.cn

[U30] Py：数据类
来源：http://pt.huixiangedu.cn

@dataclass(slots=True)
来源：http://xu.lnxyls.cn

[U31] Py：单测
来源：http://xy.shxzukj.cn

python -m pytest -q
来源：http://qg.szxytkj.cn

[U32] Py：代码格式化
来源：http://xi.bookmarksfly.cn

ruff format . && ruff check --fix .
来源：http://ru.wgjwhj.cn

[U33] Py：打包发布
来源：http://vr.panjiajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://xl.szsharing.cn

[U34] Py：判断编码
来源：http://af.shxzskj.cn

chardet.detect(raw)
来源：http://ll.jianghongdianzi.cn

[U35] Py：发送邮件
来源：http://wx.colortex.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kd.shxzukj.cn

[U36] Py：定时任务
来源：http://jy.chemitech.net.cn

schedule.every(10).minutes.do(job)
来源：http://zf.huanxung.cn

[U37] Py：读写 Excel
来源：http://md.shxzskj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://gc.panjiajie.cn

[U38] Py：获取脚本所在目录
来源：http://ke.shtwfgs.cn

Path(__file__).resolve().parent
来源：http://tp.panjiajie.cn

[U39] Py：判断是否在交互环境
来源：http://et.wgjwhj.cn

sys.stdout.isatty()
来源：http://wm.shxzskj.cn

[U40] Py：打印到标准错误
来源：http://ac.colortex.cn

print("err", file=sys.stderr)
来源：http://jg.nicolike.cn

[U41] PHP：初始化 Composer 项目
来源：http://gq.jianghongdianzi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://il.9csxet.cn

[U42] PHP：PSR-4 自动加载
来源：http://xl.szxytkj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xl.bookmarksfly.cn

[U43] PHP：声明命名空间
来源：http://fh.gzmigu.cn

namespace App\Http;
来源：http://kk.huanxung.cn

[U44] PHP：开启严格类型
来源：http://gx.hahajie.cn

declare(strict_types=1);
来源：http://qy.shxzskj.cn

[U45] PHP：类型声明与返回类型
来源：http://jj.521024.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qq.chemitech.net.cn

[U46] PHP：可空类型
来源：http://bj.panjiajie.cn

?string $name = null
来源：http://xj.yuntaijiaju.cn

[U47] PHP：联合类型
来源：http://qn.hahajie.cn

int|string $id
来源：http://bn.bjjhwx.cn

[U48] PHP：纯枚举
来源：http://td.asd995.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sg.haigaiapp.cn

[U49] PHP：只读属性
来源：http://jk.yuexingan06.cn

public readonly string $name
来源：http://zp.yuntaijiaju.cn

[U50] PHP：构造器属性提升
来源：http://lg.huixiangedu.cn

public function __construct(private int $id) {}
来源：http://ep.9csxet.cn

[U51] PHP：数组解构
来源：http://dz.huixiangedu.cn

[$a, $b] = $arr;
来源：http://ca.nszjky.cn

[U52] PHP：箭头函数
来源：http://xk.jctech888.com.cn

$double = fn($x) => $x * 2;
来源：http://pj.szsharing.cn

[U53] PHP：空合并运算符
来源：http://rq.bookmarksfly.cn

$v = $a ?? $b ?? "default";
来源：http://oe.bjjhwx.cn

[U54] PHP：空安全调用
来源：http://vi.9csxet.cn

$obj?->method()
来源：http://pe.newstarts.cn

[U55] PHP：match 表达式
来源：http://ox.huanxung.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uh.szxytkj.cn

[U56] PHP：命名参数
来源：http://ko.chemitech.net.cn

f(a: 1, b: 2)
来源：http://ga.bookmarksfly.cn

[U57] PHP：字符串插值
来源：http://da.newstarts.cn

"值: {$a}"
来源：http://ek.hahajie.cn

[U58] PHP：数组三件套
来源：http://ax.wgjwhj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ok.lnxyls.cn

[U59] PHP：自定义排序
来源：http://al.nszjky.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pu.szxytkj.cn

[U60] PHP：JSON 编解码
来源：http://uq.newstarts.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yr.wgjwhj.cn

[U61] PHP：正则
来源：http://qu.wgjwhj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qo.colortex.cn

[U62] PHP：日期对象
来源：http://cf.wgjwhj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ra.lnxyls.cn

[U63] PHP：文件读写
来源：http://da.hahajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://aq.9csxet.cn

[U64] PHP：目录遍历
来源：http://gs.chemitech.net.cn

glob("dir/*.php");  scandir("dir");
来源：http://em.muxihuayi.cn

[U65] PHP：会话
来源：http://ak.521024.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://yg.hahajie.cn

[U66] PHP：设置 Cookie
来源：http://ss.huixinmuqiang.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sn.colortex.cn

[U67] PHP：处理文件上传
来源：http://je.muxihuayi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ed.panjiajie.cn

[U68] PHP：PDO 连接
来源：http://rg.asd995.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kd.huixinmuqiang.cn

[U69] PHP：PDO 预处理
来源：http://bd.newstarts.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ur.gzmigu.cn

[U70] PHP：PDO 事务
来源：http://ca.wgjwhj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hh.nszjky.cn

[U71] PHP：抛出异常
来源：http://st.huixinmuqiang.cn

throw new RuntimeException("失败", 500);
来源：http://ei.hahajie.cn

[U72] PHP：写错误日志
来源：http://ga.chemitech.net.cn

error_log("失败: " . $e->getMessage());
来源：http://xm.shxzukj.cn

[U73] PHP：读取 ini 配置
来源：http://vk.521024.cn

parse_ini_file("config.ini", true)
来源：http://we.muxihuayi.cn

[U74] PHP：读取环境变量
来源：http://fu.muxihuayi.cn

getenv("APP_ENV") ?: "production"
来源：http://hh.szxytkj.cn

[U75] PHP：依赖注入
来源：http://kv.shtwfgs.cn

composer require psr/container
来源：http://cr.shxzskj.cn

[U76] PHP：简单路由
来源：http://yr.colortex.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vi.szxytkj.cn

[U77] PHP：模板渲染
来源：http://dn.gzmigu.cn

composer require twig/twig
来源：http://vu.haigaiapp.cn

[U78] PHP：单元测试
来源：http://tp.jianghongdianzi.cn

composer require --dev phpunit/phpunit
来源：http://ff.jianghongdianzi.cn

[U79] PHP：静态分析
来源：http://bz.huixiangedu.cn

composer require --dev phpstan/phpstan
来源：http://my.szxytkj.cn

[U80] PHP：代码规范修复
来源：http://ab.nszjky.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ch.yuntaijiaju.cn

[U81] JS：初始化项目
来源：http://ja.muxihuayi.cn

npm init -y;  npm i express
来源：http://hl.nicolike.cn

[U82] JS：package.json 脚本
来源：http://wk.hahajie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://oc.panjiajie.cn

[U83] JS：ES Module 导入导出
来源：http://lr.huanxung.cn

export const a = 1;  import { a } from "./m.js";
来源：http://wx.shtwfgs.cn

[U84] JS：CommonJS 写法
来源：http://xt.jianghongdianzi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wl.hahajie.cn

[U85] JS：可选链
来源：http://fg.wgjwhj.cn

a?.b?.c
来源：http://xn.huanxung.cn

[U86] JS：空值合并
来源：http://ya.colortex.cn

a ?? b
来源：http://zo.szxytkj.cn

[U87] JS：解构默认值
来源：http://rh.521024.cn

const { a = 1, b = 2 } = obj;
来源：http://kf.szsharing.cn

[U88] JS：对象展开合并
来源：http://qh.yuntaijiaju.cn

{ ...a, ...b }
来源：http://cy.521024.cn

[U89] JS：数组去重
来源：http://yh.szsharing.cn

[...new Set(arr)]
来源：http://xd.panjiajie.cn

[U90] JS：数字数组排序
来源：http://wy.huanxung.cn

[...arr].sort((a, b) => a - b)
来源：http://um.hnjuh.cn

[U91] JS：对象键值遍历
来源：http://ob.panjiajie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pd.gzmigu.cn

[U92] JS：深拷贝
来源：http://vx.lnxyls.cn

structuredClone(obj)
来源：http://xe.gzmigu.cn

[U93] JS：模板字符串
来源：http://za.shxzukj.cn

`共 ${n} 条`
来源：http://cq.wgjwhj.cn

[U94] JS：箭头函数
来源：http://pn.chemitech.net.cn

const double = x => x * 2;
来源：http://hp.521024.cn

[U95] JS：Promise 包装
来源：http://ha.muxihuayi.cn

new Promise((resolve, reject) => {})
来源：http://to.asd995.cn

[U96] JS：async/await 与异常
来源：http://uf.nicolike.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xa.jctech888.com.cn

[U97] JS：并发请求
来源：http://lv.jianghongdianzi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://hr.haigaiapp.cn

[U98] JS：fetch 带 JSON
来源：http://ny.haigaiapp.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://un.chemitech.net.cn

[U99] JS：事件监听
来源：http://ue.huixiangedu.cn

el.addEventListener("click", e => {})
来源：http://os.panjiajie.cn

[U100] JS：DOM 查询
来源：http://an.9csxet.cn

document.querySelector(".item")
来源：http://qn.nicolike.cn

[U101] JS：classList 操作
来源：http://iq.huanxung.cn

el.classList.toggle("active")
来源：http://kt.jctech888.com.cn

[U102] JS：本地存储
来源：http://oe.lnxyls.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://tv.bookmarksfly.cn

[U103] JS：定时器
来源：http://si.nszjky.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wl.wgjwhj.cn

[U104] JS：防抖
来源：http://ab.gzmigu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://si.muxihuayi.cn

[U105] JS：节流
来源：http://pi.yuntaijiaju.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hf.panjiajie.cn

[U106] JS：日期格式化
来源：http://qo.huixiangedu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lc.521024.cn

[U107] JS：数字千分位
来源：http://ju.hnjuh.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://he.szsharing.cn

[U108] JS：随机整数
来源：http://pc.asd995.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nd.9csxet.cn

[U109] JS：数组分组
来源：http://ou.newstarts.cn

Object.groupBy(arr, x => x.type)
来源：http://dv.colortex.cn

[U110] JS：数组分块
来源：http://tf.521024.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mx.jctech888.com.cn

[U111] JS：对象转 Map
来源：http://jx.shxzskj.cn

new Map(Object.entries(obj))
来源：http://me.chemitech.net.cn

[U112] JS：字符串补位
来源：http://qg.gzmigu.cn

"7".padStart(3, "0")
来源：http://pv.9csxet.cn

[U113] JS：正则替换全部
来源：http://jk.haigaiapp.cn

s.replaceAll("a", "b")
来源：http://ou.huixiangedu.cn

[U114] JS：JSON 深比较
来源：http://qk.9csxet.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://iy.asd995.cn

[U115] JS：生成 UUID
来源：http://lo.colortex.cn

crypto.randomUUID()
来源：http://je.asd995.cn

[U116] JS：类型检查（JSDoc）
来源：http://lv.bookmarksfly.cn

/** @param {string} name */ function f(name) {}
来源：http://fw.nszjky.cn


<!-- 参考信息 -->