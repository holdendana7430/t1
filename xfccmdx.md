代发 wailian999

[T31] Lua：Hello World
来源：http://jj.9csxet.cn

print("Hello")
来源：http://ne.gzmigu.cn

[T32] Lua：局部变量
来源：http://xb.haigaiapp.cn

local a = 1
来源：http://qs.shtwfgs.cn

[T33] Lua：表（数组）
来源：http://ue.chemitech.net.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://dl.yuntaijiaju.cn

[T34] Lua：遍历表
来源：http://uo.asd995.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://mj.jianghongdianzi.cn

[T35] Lua：字典表
来源：http://fz.shxzukj.cn

local d = { a = 1 };  d.b = 2
来源：http://si.hnjuh.cn

[T36] Lua：函数
来源：http://kk.huixiangedu.cn

function add(a, b) return a + b end
来源：http://cn.newstarts.cn

[T37] Lua：字符串拼接
来源：http://tn.wgjwhj.cn

"a" .. "b"
来源：http://db.bookmarksfly.cn

[T38] Lua：条件
来源：http://kj.haigaiapp.cn

if x > 0 then print("正") end
来源：http://zt.hnjuh.cn

[T39] Lua：模式匹配
来源：http://he.nicolike.cn

string.find(s, "%d+")
来源：http://ez.9csxet.cn

[T40] Lua：元表
来源：http://nv.newstarts.cn

setmetatable({}, { __index = base })
来源：http://le.nszjky.cn

[T41] Perl：Hello World
来源：http://nw.bookmarksfly.cn

print "Hello\n";
来源：http://tv.shtwfgs.cn

[T42] Perl：变量类型
来源：http://jy.szsharing.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://je.yuntaijiaju.cn

[T43] Perl：字符串插值
来源：http://pv.huixinmuqiang.cn

"值: $a"
来源：http://mt.muxihuayi.cn

[T44] Perl：条件
来源：http://sj.colortex.cn

if ($a > 0) { print "正"; }
来源：http://jz.colortex.cn

[T45] Perl：数组遍历
来源：http://na.yuexingan06.cn

for my $x (@arr) { print $x; }
来源：http://xz.yuexingan06.cn

[T46] Perl：哈希操作
来源：http://mn.szsharing.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nu.bjjhwx.cn

[T47] Perl：正则捕获
来源：http://qr.9csxet.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://oy.colortex.cn

[T48] Perl：正则替换
来源：http://dt.yuexingan06.cn

$s =~ s/old/new/g;
来源：http://ri.haigaiapp.cn

[T49] Perl：函数
来源：http://az.colortex.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vq.shxzukj.cn

[T50] Perl：逐行读文件
来源：http://nc.9csxet.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://jf.asd995.cn

while (my $line = <$fh>) { print $line; }
来源：http://sm.colortex.cn

[T51] Scala：Hello World
来源：http://uc.yuexingan06.cn

println("Hello")
来源：http://sg.hnjuh.cn

[T52] Scala：变量
来源：http://bj.muxihuayi.cn

val a = 1;  var b = 2
来源：http://wo.521024.cn

[T53] Scala：字符串插值
来源：http://jv.panjiajie.cn

s"值: $b"
来源：http://rk.yuntaijiaju.cn

[T54] Scala：集合映射
来源：http://en.panjiajie.cn

List(1, 2, 3).map(_ * 2)
来源：http://pl.panjiajie.cn

[T55] Scala：集合过滤
来源：http://dm.jianghongdianzi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://eg.lnxyls.cn

[T56] Scala：样例类
来源：http://lb.huixiangedu.cn

case class User(name: String, age: Int)
来源：http://bo.521024.cn

[T57] Scala：模式匹配
来源：http://px.asd995.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://yw.szxytkj.cn

[T58] Scala：函数定义
来源：http://ix.colortex.cn

def add(a: Int, b: Int): Int = a + b
来源：http://jq.bjjhwx.cn

[T59] Scala：循环
来源：http://tz.asd995.cn

for (i <- 1 to 10) println(i)
来源：http://fh.panjiajie.cn

[T60] Scala：折叠
来源：http://dq.shtwfgs.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dw.gzmigu.cn

================================================================================
来源：http://gs.521024.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pe.muxihuayi.cn

================================================================================
来源：http://yz.colortex.cn

[U01] Py：创建虚拟环境
来源：http://ew.9csxet.cn

python -m venv .venv && source .venv/bin/activate
来源：http://hg.chemitech.net.cn

[U02] Py：导出 / 安装依赖
来源：http://wn.panjiajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mj.chemitech.net.cn

[U03] Py：加载 .env 配置
来源：http://gp.szsharing.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://cq.521024.cn

[U04] Py：变量调试打印
来源：http://qn.haigaiapp.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tt.shtwfgs.cn

[U05] Py：列表去重且保序
来源：http://iy.szxytkj.cn

list(dict.fromkeys(arr))
来源：http://lj.nszjky.cn

[U06] Py：合并两个字典
来源：http://ig.nicolike.cn

{**a, **b}
来源：http://zl.haigaiapp.cn

[U07] Py：反转字典键值
来源：http://pq.asd995.cn

{v: k for k, v in d.items()}
来源：http://ts.yuntaijiaju.cn

[U08] Py：展平二维列表
来源：http://nu.lnxyls.cn

[y for x in nested for y in x]
来源：http://xh.shxzukj.cn

[U09] Py：字典取最大值的键
来源：http://zi.nicolike.cn

max(d, key=d.get)
来源：http://gp.bookmarksfly.cn

[U10] Py：按值排序字典
来源：http://dk.szxytkj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tl.newstarts.cn

[U11] Py：生成器表达式
来源：http://yj.wgjwhj.cn

(x * 2 for x in arr)
来源：http://nq.521024.cn

[U12] Py：取出现最多的 3 个元素
来源：http://pw.chemitech.net.cn

Counter(arr).most_common(3)
来源：http://kf.521024.cn

[U13] Py：固定长度队列
来源：http://cq.hnjuh.cn

deque(maxlen=10)
来源：http://ab.yuntaijiaju.cn

[U14] Py：分组收集到列表
来源：http://bl.muxihuayi.cn

defaultdict(list)
来源：http://vw.chemitech.net.cn

[U15] Py：高精度计时
来源：http://pl.nicolike.cn

t = time.perf_counter()
来源：http://wa.9csxet.cn

[U16] Py：命令行参数解析
来源：http://mb.chemitech.net.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ts.bjjhwx.cn

[U17] Py：初始化日志
来源：http://ln.jianghongdianzi.cn

logging.basicConfig(level=logging.INFO)
来源：http://hq.nicolike.cn

[U18] Py：预编译正则
来源：http://bu.shxzskj.cn

pat = re.compile(r"\d+")
来源：http://jj.haigaiapp.cn

[U19] Py：正则替换带回调
来源：http://hh.huanxung.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ig.nszjky.cn

[U20] Py：缓存函数结果
来源：http://gf.colortex.cn

@functools.lru_cache(maxsize=None)
来源：http://rv.shtwfgs.cn

[U21] Py：自定义上下文管理器
来源：http://gc.9csxet.cn

@contextlib.contextmanager
来源：http://pr.nicolike.cn

[U22] Py：矩阵转置
来源：http://kr.shtwfgs.cn

list(zip(*m))
来源：http://ky.hnjuh.cn

[U23] Py：分块读取大文件
来源：http://ue.huixiangedu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qo.lnxyls.cn

[U24] Py：路径操作
来源：http://gn.bjjhwx.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://co.shxzskj.cn

[U25] Py：CSV 按字典读
来源：http://cp.asd995.cn

csv.DictReader(f)
来源：http://yv.gzmigu.cn

[U26] Py：并发下载
来源：http://qd.9csxet.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ea.bookmarksfly.cn

[U27] Py：异步 HTTP
来源：http://ne.jianghongdianzi.cn

aiohttp.ClientSession() 配合 async with
来源：http://qw.wgjwhj.cn

[U28] Py：类型别名
来源：http://lo.huanxung.cn

UserId = int
来源：http://jf.wgjwhj.cn

[U29] Py：属性校验
来源：http://my.lnxyls.cn

@property 与 @x.setter 配合
来源：http://xl.yuexingan06.cn

[U30] Py：数据类
来源：http://pq.wgjwhj.cn

@dataclass(slots=True)
来源：http://qt.wgjwhj.cn

[U31] Py：单测
来源：http://ah.lnxyls.cn

python -m pytest -q
来源：http://ks.muxihuayi.cn

[U32] Py：代码格式化
来源：http://st.hnjuh.cn

ruff format . && ruff check --fix .
来源：http://vt.huanxung.cn

[U33] Py：打包发布
来源：http://gt.szsharing.cn

python -m build  （依赖 pyproject.toml）
来源：http://pp.asd995.cn

[U34] Py：判断编码
来源：http://yq.panjiajie.cn

chardet.detect(raw)
来源：http://ud.panjiajie.cn

[U35] Py：发送邮件
来源：http://yk.jctech888.com.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ja.9csxet.cn

[U36] Py：定时任务
来源：http://lb.yuexingan06.cn

schedule.every(10).minutes.do(job)
来源：http://rs.bjjhwx.cn

[U37] Py：读写 Excel
来源：http://gf.chemitech.net.cn

pandas.read_excel / DataFrame.to_excel
来源：http://zg.nszjky.cn

[U38] Py：获取脚本所在目录
来源：http://vm.huanxung.cn

Path(__file__).resolve().parent
来源：http://fh.szsharing.cn

[U39] Py：判断是否在交互环境
来源：http://cq.gzmigu.cn

sys.stdout.isatty()
来源：http://br.hahajie.cn

[U40] Py：打印到标准错误
来源：http://fm.chemitech.net.cn

print("err", file=sys.stderr)
来源：http://ye.nszjky.cn

[U41] PHP：初始化 Composer 项目
来源：http://me.bjjhwx.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ja.szxytkj.cn

[U42] PHP：PSR-4 自动加载
来源：http://tk.9csxet.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zv.jianghongdianzi.cn

[U43] PHP：声明命名空间
来源：http://ro.szsharing.cn

namespace App\Http;
来源：http://ed.gzmigu.cn

[U44] PHP：开启严格类型
来源：http://eu.huixiangedu.cn

declare(strict_types=1);
来源：http://cg.wgjwhj.cn

[U45] PHP：类型声明与返回类型
来源：http://dc.huixinmuqiang.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://tc.521024.cn

[U46] PHP：可空类型
来源：http://cj.panjiajie.cn

?string $name = null
来源：http://ll.bjjhwx.cn

[U47] PHP：联合类型
来源：http://ev.gzmigu.cn

int|string $id
来源：http://hi.asd995.cn

[U48] PHP：纯枚举
来源：http://hz.wgjwhj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://us.colortex.cn

[U49] PHP：只读属性
来源：http://vb.hahajie.cn

public readonly string $name
来源：http://rr.yuexingan06.cn

[U50] PHP：构造器属性提升
来源：http://qu.jianghongdianzi.cn

public function __construct(private int $id) {}
来源：http://el.521024.cn

[U51] PHP：数组解构
来源：http://le.haigaiapp.cn

[$a, $b] = $arr;
来源：http://ec.nicolike.cn

[U52] PHP：箭头函数
来源：http://kj.muxihuayi.cn

$double = fn($x) => $x * 2;
来源：http://xp.newstarts.cn

[U53] PHP：空合并运算符
来源：http://fp.wgjwhj.cn

$v = $a ?? $b ?? "default";
来源：http://vi.nicolike.cn

[U54] PHP：空安全调用
来源：http://fw.colortex.cn

$obj?->method()
来源：http://ib.panjiajie.cn

[U55] PHP：match 表达式
来源：http://ql.bjjhwx.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ya.jctech888.com.cn

[U56] PHP：命名参数
来源：http://sw.shtwfgs.cn

f(a: 1, b: 2)
来源：http://rz.colortex.cn

[U57] PHP：字符串插值
来源：http://tb.muxihuayi.cn

"值: {$a}"
来源：http://zd.shtwfgs.cn

[U58] PHP：数组三件套
来源：http://dv.jctech888.com.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ck.chemitech.net.cn

[U59] PHP：自定义排序
来源：http://tw.shtwfgs.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ya.yuexingan06.cn

[U60] PHP：JSON 编解码
来源：http://lz.muxihuayi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://be.szsharing.cn

[U61] PHP：正则
来源：http://hc.szxytkj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://js.chemitech.net.cn

[U62] PHP：日期对象
来源：http://gg.huixinmuqiang.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sb.yuntaijiaju.cn

[U63] PHP：文件读写
来源：http://as.huixiangedu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fo.bjjhwx.cn

[U64] PHP：目录遍历
来源：http://rl.shxzskj.cn

glob("dir/*.php");  scandir("dir");
来源：http://wk.521024.cn

[U65] PHP：会话
来源：http://ip.haigaiapp.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://dt.yuntaijiaju.cn

[U66] PHP：设置 Cookie
来源：http://kd.szxytkj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ze.huixiangedu.cn

[U67] PHP：处理文件上传
来源：http://ed.shxzskj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sc.haigaiapp.cn

[U68] PHP：PDO 连接
来源：http://bf.9csxet.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wj.haigaiapp.cn

[U69] PHP：PDO 预处理
来源：http://qh.shxzukj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hf.szsharing.cn

[U70] PHP：PDO 事务
来源：http://xk.nicolike.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pr.nszjky.cn

[U71] PHP：抛出异常
来源：http://os.chemitech.net.cn

throw new RuntimeException("失败", 500);
来源：http://yt.muxihuayi.cn

[U72] PHP：写错误日志
来源：http://ou.hahajie.cn

error_log("失败: " . $e->getMessage());
来源：http://ue.shtwfgs.cn

[U73] PHP：读取 ini 配置
来源：http://mj.wgjwhj.cn

parse_ini_file("config.ini", true)
来源：http://aq.szxytkj.cn

[U74] PHP：读取环境变量
来源：http://yl.hahajie.cn

getenv("APP_ENV") ?: "production"
来源：http://dt.yuexingan06.cn

[U75] PHP：依赖注入
来源：http://fk.panjiajie.cn

composer require psr/container
来源：http://fp.bjjhwx.cn

[U76] PHP：简单路由
来源：http://yu.newstarts.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lw.huixinmuqiang.cn

[U77] PHP：模板渲染
来源：http://ga.hahajie.cn

composer require twig/twig
来源：http://sl.newstarts.cn

[U78] PHP：单元测试
来源：http://wa.chemitech.net.cn

composer require --dev phpunit/phpunit
来源：http://kr.muxihuayi.cn

[U79] PHP：静态分析
来源：http://ot.huixiangedu.cn

composer require --dev phpstan/phpstan
来源：http://rq.shtwfgs.cn

[U80] PHP：代码规范修复
来源：http://lq.panjiajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://dx.bjjhwx.cn

[U81] JS：初始化项目
来源：http://zf.chemitech.net.cn

npm init -y;  npm i express
来源：http://uo.yuexingan06.cn

[U82] JS：package.json 脚本
来源：http://kv.hahajie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ld.jctech888.com.cn

[U83] JS：ES Module 导入导出
来源：http://sj.shxzukj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qr.hnjuh.cn

[U84] JS：CommonJS 写法
来源：http://si.521024.cn

module.exports = { a };  const { a } = require("./m");
来源：http://gw.panjiajie.cn

[U85] JS：可选链
来源：http://ex.nszjky.cn

a?.b?.c
来源：http://st.gzmigu.cn

[U86] JS：空值合并
来源：http://ha.jianghongdianzi.cn

a ?? b
来源：http://dg.hahajie.cn

[U87] JS：解构默认值
来源：http://hn.hahajie.cn

const { a = 1, b = 2 } = obj;
来源：http://qk.lnxyls.cn

[U88] JS：对象展开合并
来源：http://nq.jctech888.com.cn

{ ...a, ...b }
来源：http://of.yuntaijiaju.cn

[U89] JS：数组去重
来源：http://oe.hnjuh.cn

[...new Set(arr)]
来源：http://px.bookmarksfly.cn

[U90] JS：数字数组排序
来源：http://xw.yuntaijiaju.cn

[...arr].sort((a, b) => a - b)
来源：http://pa.shxzskj.cn

[U91] JS：对象键值遍历
来源：http://kl.wgjwhj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lj.asd995.cn

[U92] JS：深拷贝
来源：http://ki.wgjwhj.cn

structuredClone(obj)
来源：http://hn.bookmarksfly.cn

[U93] JS：模板字符串
来源：http://oh.shxzukj.cn

`共 ${n} 条`
来源：http://rt.shtwfgs.cn

[U94] JS：箭头函数
来源：http://ba.panjiajie.cn

const double = x => x * 2;
来源：http://cy.hahajie.cn

[U95] JS：Promise 包装
来源：http://bq.bookmarksfly.cn

new Promise((resolve, reject) => {})
来源：http://jp.gzmigu.cn

[U96] JS：async/await 与异常
来源：http://sx.huixiangedu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gi.haigaiapp.cn

[U97] JS：并发请求
来源：http://is.haigaiapp.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://mw.bookmarksfly.cn

[U98] JS：fetch 带 JSON
来源：http://gb.szxytkj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rk.jianghongdianzi.cn

[U99] JS：事件监听
来源：http://iz.shtwfgs.cn

el.addEventListener("click", e => {})
来源：http://cd.bookmarksfly.cn

[U100] JS：DOM 查询
来源：http://hw.bookmarksfly.cn

document.querySelector(".item")
来源：http://gv.9csxet.cn

[U101] JS：classList 操作
来源：http://ic.szxytkj.cn

el.classList.toggle("active")
来源：http://gg.hahajie.cn

[U102] JS：本地存储
来源：http://yv.shtwfgs.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://gs.521024.cn

[U103] JS：定时器
来源：http://wo.jctech888.com.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ur.nicolike.cn

[U104] JS：防抖
来源：http://yw.szxytkj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://az.panjiajie.cn

[U105] JS：节流
来源：http://rc.bookmarksfly.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://oy.9csxet.cn

[U106] JS：日期格式化
来源：http://dc.huanxung.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ad.huixinmuqiang.cn

[U107] JS：数字千分位
来源：http://lv.nicolike.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gq.wgjwhj.cn

[U108] JS：随机整数
来源：http://vo.asd995.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gs.hahajie.cn

[U109] JS：数组分组
来源：http://ck.shxzukj.cn

Object.groupBy(arr, x => x.type)
来源：http://ki.huixiangedu.cn

[U110] JS：数组分块
来源：http://wt.hahajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://st.huixinmuqiang.cn

[U111] JS：对象转 Map
来源：http://yd.newstarts.cn

new Map(Object.entries(obj))
来源：http://fo.jianghongdianzi.cn

[U112] JS：字符串补位
来源：http://eq.hnjuh.cn

"7".padStart(3, "0")
来源：http://bg.huanxung.cn

[U113] JS：正则替换全部
来源：http://gi.szxytkj.cn

s.replaceAll("a", "b")
来源：http://gq.9csxet.cn

[U114] JS：JSON 深比较
来源：http://cn.huixinmuqiang.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://gl.jianghongdianzi.cn

[U115] JS：生成 UUID
来源：http://ti.muxihuayi.cn

crypto.randomUUID()
来源：http://if.gzmigu.cn

[U116] JS：类型检查（JSDoc）
来源：http://lh.521024.cn

/** @param {string} name */ function f(name) {}
来源：http://md.muxihuayi.cn

[U117] JS：单元测试
来源：http://kp.nicolike.cn

npm i -D vitest;  npx vitest
来源：http://tt.lnxyls.cn

[U118] JS：开发服务器
来源：http://bk.bjjhwx.cn

npm i -D vite;  npx vite
来源：http://mo.bjjhwx.cn


<!-- 参考信息 -->