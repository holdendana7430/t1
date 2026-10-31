代发 wailian999

[T25] Swift：结构体
来源：http://vi.huixinmuqiang.cn

struct P { var x: Int }
来源：http://cr.nszjky.cn

[T26] Swift：类与重写
来源：http://ap.nszjky.cn

class A: Base { override func f() {} }
来源：http://is.yuexingan06.cn

[T27] Swift：错误处理
来源：http://yn.haigaiapp.cn

do { try f() } catch { print(error) }
来源：http://vr.colortex.cn

[T28] Swift：枚举
来源：http://me.9csxet.cn

enum Color { case red, green }
来源：http://zx.asd995.cn

[T29] Swift：guard 提前返回
来源：http://qb.lnxyls.cn

guard let x = opt else { return }
来源：http://qc.yuexingan06.cn

[T30] Swift：协议
来源：http://pn.chemitech.net.cn

protocol Shape { func area() -> Double }
来源：http://lp.shxzukj.cn

[T31] Lua：Hello World
来源：http://ve.wgjwhj.cn

print("Hello")
来源：http://ud.jctech888.com.cn

[T32] Lua：局部变量
来源：http://cj.shxzukj.cn

local a = 1
来源：http://rf.nszjky.cn

[T33] Lua：表（数组）
来源：http://il.shxzukj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://kx.panjiajie.cn

[T34] Lua：遍历表
来源：http://sf.asd995.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ql.shxzukj.cn

[T35] Lua：字典表
来源：http://ad.szsharing.cn

local d = { a = 1 };  d.b = 2
来源：http://lj.hahajie.cn

[T36] Lua：函数
来源：http://kd.colortex.cn

function add(a, b) return a + b end
来源：http://ns.jctech888.com.cn

[T37] Lua：字符串拼接
来源：http://hy.gzmigu.cn

"a" .. "b"
来源：http://eb.bjjhwx.cn

[T38] Lua：条件
来源：http://rx.bjjhwx.cn

if x > 0 then print("正") end
来源：http://cw.colortex.cn

[T39] Lua：模式匹配
来源：http://cg.hahajie.cn

string.find(s, "%d+")
来源：http://ak.huanxung.cn

[T40] Lua：元表
来源：http://dk.9csxet.cn

setmetatable({}, { __index = base })
来源：http://gt.colortex.cn

[T41] Perl：Hello World
来源：http://ev.colortex.cn

print "Hello\n";
来源：http://no.asd995.cn

[T42] Perl：变量类型
来源：http://ui.panjiajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qj.hnjuh.cn

[T43] Perl：字符串插值
来源：http://vz.wgjwhj.cn

"值: $a"
来源：http://qv.bookmarksfly.cn

[T44] Perl：条件
来源：http://gt.chemitech.net.cn

if ($a > 0) { print "正"; }
来源：http://kj.shtwfgs.cn

[T45] Perl：数组遍历
来源：http://nf.bookmarksfly.cn

for my $x (@arr) { print $x; }
来源：http://hf.521024.cn

[T46] Perl：哈希操作
来源：http://aj.shxzskj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zq.wgjwhj.cn

[T47] Perl：正则捕获
来源：http://mx.9csxet.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ux.shtwfgs.cn

[T48] Perl：正则替换
来源：http://sg.yuexingan06.cn

$s =~ s/old/new/g;
来源：http://vj.jianghongdianzi.cn

[T49] Perl：函数
来源：http://ji.yuntaijiaju.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ku.nicolike.cn

[T50] Perl：逐行读文件
来源：http://vw.chemitech.net.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ui.hahajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://dl.panjiajie.cn

[T51] Scala：Hello World
来源：http://zw.shxzukj.cn

println("Hello")
来源：http://yc.yuntaijiaju.cn

[T52] Scala：变量
来源：http://re.nicolike.cn

val a = 1;  var b = 2
来源：http://af.huanxung.cn

[T53] Scala：字符串插值
来源：http://ot.hnjuh.cn

s"值: $b"
来源：http://bg.colortex.cn

[T54] Scala：集合映射
来源：http://ag.huixiangedu.cn

List(1, 2, 3).map(_ * 2)
来源：http://br.nicolike.cn

[T55] Scala：集合过滤
来源：http://wn.lnxyls.cn

List(1, 2, 3).filter(_ > 1)
来源：http://oc.bjjhwx.cn

[T56] Scala：样例类
来源：http://vr.muxihuayi.cn

case class User(name: String, age: Int)
来源：http://xc.panjiajie.cn

[T57] Scala：模式匹配
来源：http://rx.nicolike.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://cl.chemitech.net.cn

[T58] Scala：函数定义
来源：http://cw.huixiangedu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ta.haigaiapp.cn

[T59] Scala：循环
来源：http://rv.shxzukj.cn

for (i <- 1 to 10) println(i)
来源：http://xj.muxihuayi.cn

[T60] Scala：折叠
来源：http://fn.yuexingan06.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nh.colortex.cn

================================================================================
来源：http://fz.panjiajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sv.nszjky.cn

================================================================================
来源：http://qj.huixiangedu.cn

[U01] Py：创建虚拟环境
来源：http://pw.szxytkj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://xc.haigaiapp.cn

[U02] Py：导出 / 安装依赖
来源：http://nv.huanxung.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pz.hahajie.cn

[U03] Py：加载 .env 配置
来源：http://ue.panjiajie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zv.yuexingan06.cn

[U04] Py：变量调试打印
来源：http://fp.yuexingan06.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://el.newstarts.cn

[U05] Py：列表去重且保序
来源：http://en.bjjhwx.cn

list(dict.fromkeys(arr))
来源：http://zo.shxzskj.cn

[U06] Py：合并两个字典
来源：http://if.shxzukj.cn

{**a, **b}
来源：http://ge.jianghongdianzi.cn

[U07] Py：反转字典键值
来源：http://pp.chemitech.net.cn

{v: k for k, v in d.items()}
来源：http://fh.gzmigu.cn

[U08] Py：展平二维列表
来源：http://hg.huixinmuqiang.cn

[y for x in nested for y in x]
来源：http://xe.bookmarksfly.cn

[U09] Py：字典取最大值的键
来源：http://my.jianghongdianzi.cn

max(d, key=d.get)
来源：http://qj.szsharing.cn

[U10] Py：按值排序字典
来源：http://up.wgjwhj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://il.shtwfgs.cn

[U11] Py：生成器表达式
来源：http://ds.hahajie.cn

(x * 2 for x in arr)
来源：http://it.wgjwhj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://nz.huixiangedu.cn

Counter(arr).most_common(3)
来源：http://zj.gzmigu.cn

[U13] Py：固定长度队列
来源：http://yu.shxzukj.cn

deque(maxlen=10)
来源：http://bp.huixiangedu.cn

[U14] Py：分组收集到列表
来源：http://rr.shxzukj.cn

defaultdict(list)
来源：http://hs.asd995.cn

[U15] Py：高精度计时
来源：http://pn.nicolike.cn

t = time.perf_counter()
来源：http://zb.huixinmuqiang.cn

[U16] Py：命令行参数解析
来源：http://hl.bjjhwx.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://my.szxytkj.cn

[U17] Py：初始化日志
来源：http://xu.panjiajie.cn

logging.basicConfig(level=logging.INFO)
来源：http://ch.szsharing.cn

[U18] Py：预编译正则
来源：http://bu.panjiajie.cn

pat = re.compile(r"\d+")
来源：http://av.yuntaijiaju.cn

[U19] Py：正则替换带回调
来源：http://fc.shtwfgs.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://no.lnxyls.cn

[U20] Py：缓存函数结果
来源：http://jl.shxzukj.cn

@functools.lru_cache(maxsize=None)
来源：http://kv.haigaiapp.cn

[U21] Py：自定义上下文管理器
来源：http://ww.chemitech.net.cn

@contextlib.contextmanager
来源：http://et.newstarts.cn

[U22] Py：矩阵转置
来源：http://nt.bjjhwx.cn

list(zip(*m))
来源：http://sr.huanxung.cn

[U23] Py：分块读取大文件
来源：http://az.shtwfgs.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ou.9csxet.cn

[U24] Py：路径操作
来源：http://aj.gzmigu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://re.szsharing.cn

[U25] Py：CSV 按字典读
来源：http://zh.521024.cn

csv.DictReader(f)
来源：http://hi.huixiangedu.cn

[U26] Py：并发下载
来源：http://rs.9csxet.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cp.huanxung.cn

[U27] Py：异步 HTTP
来源：http://wf.chemitech.net.cn

aiohttp.ClientSession() 配合 async with
来源：http://vm.shxzskj.cn

[U28] Py：类型别名
来源：http://vv.huanxung.cn

UserId = int
来源：http://dn.muxihuayi.cn

[U29] Py：属性校验
来源：http://tk.jianghongdianzi.cn

@property 与 @x.setter 配合
来源：http://oy.lnxyls.cn

[U30] Py：数据类
来源：http://lv.9csxet.cn

@dataclass(slots=True)
来源：http://rp.jianghongdianzi.cn

[U31] Py：单测
来源：http://wr.gzmigu.cn

python -m pytest -q
来源：http://xh.muxihuayi.cn

[U32] Py：代码格式化
来源：http://rv.szxytkj.cn

ruff format . && ruff check --fix .
来源：http://tr.panjiajie.cn

[U33] Py：打包发布
来源：http://xw.szxytkj.cn

python -m build  （依赖 pyproject.toml）
来源：http://pd.wgjwhj.cn

[U34] Py：判断编码
来源：http://zc.9csxet.cn

chardet.detect(raw)
来源：http://mu.colortex.cn

[U35] Py：发送邮件
来源：http://si.nszjky.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kc.hnjuh.cn

[U36] Py：定时任务
来源：http://ft.panjiajie.cn

schedule.every(10).minutes.do(job)
来源：http://uv.521024.cn

[U37] Py：读写 Excel
来源：http://lu.shxzskj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://sl.chemitech.net.cn

[U38] Py：获取脚本所在目录
来源：http://ub.haigaiapp.cn

Path(__file__).resolve().parent
来源：http://wu.szsharing.cn

[U39] Py：判断是否在交互环境
来源：http://vs.yuntaijiaju.cn

sys.stdout.isatty()
来源：http://ka.shxzukj.cn

[U40] Py：打印到标准错误
来源：http://xs.chemitech.net.cn

print("err", file=sys.stderr)
来源：http://zm.yuexingan06.cn

[U41] PHP：初始化 Composer 项目
来源：http://xj.bookmarksfly.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://au.szsharing.cn

[U42] PHP：PSR-4 自动加载
来源：http://ke.bookmarksfly.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tq.szxytkj.cn

[U43] PHP：声明命名空间
来源：http://de.yuexingan06.cn

namespace App\Http;
来源：http://qd.521024.cn

[U44] PHP：开启严格类型
来源：http://rd.jctech888.com.cn

declare(strict_types=1);
来源：http://ku.haigaiapp.cn

[U45] PHP：类型声明与返回类型
来源：http://hz.huixinmuqiang.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://oj.chemitech.net.cn

[U46] PHP：可空类型
来源：http://jh.chemitech.net.cn

?string $name = null
来源：http://iy.lnxyls.cn

[U47] PHP：联合类型
来源：http://cr.wgjwhj.cn

int|string $id
来源：http://ek.huixiangedu.cn

[U48] PHP：纯枚举
来源：http://yg.lnxyls.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nn.huixinmuqiang.cn

[U49] PHP：只读属性
来源：http://vj.szxytkj.cn

public readonly string $name
来源：http://dh.lnxyls.cn

[U50] PHP：构造器属性提升
来源：http://ln.shxzskj.cn

public function __construct(private int $id) {}
来源：http://ib.shtwfgs.cn

[U51] PHP：数组解构
来源：http://sz.jianghongdianzi.cn

[$a, $b] = $arr;
来源：http://lr.521024.cn

[U52] PHP：箭头函数
来源：http://rd.colortex.cn

$double = fn($x) => $x * 2;
来源：http://ew.nicolike.cn

[U53] PHP：空合并运算符
来源：http://mg.hnjuh.cn

$v = $a ?? $b ?? "default";
来源：http://zq.9csxet.cn

[U54] PHP：空安全调用
来源：http://xx.shxzskj.cn

$obj?->method()
来源：http://om.jctech888.com.cn

[U55] PHP：match 表达式
来源：http://xk.chemitech.net.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://eu.szxytkj.cn

[U56] PHP：命名参数
来源：http://qk.colortex.cn

f(a: 1, b: 2)
来源：http://st.jctech888.com.cn

[U57] PHP：字符串插值
来源：http://rk.huanxung.cn

"值: {$a}"
来源：http://mb.colortex.cn

[U58] PHP：数组三件套
来源：http://cg.szsharing.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bs.bjjhwx.cn

[U59] PHP：自定义排序
来源：http://lz.gzmigu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ur.huanxung.cn

[U60] PHP：JSON 编解码
来源：http://kn.panjiajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vx.shxzskj.cn

[U61] PHP：正则
来源：http://zz.hahajie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hv.panjiajie.cn

[U62] PHP：日期对象
来源：http://fv.bookmarksfly.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yx.nicolike.cn

[U63] PHP：文件读写
来源：http://yc.521024.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://eb.hahajie.cn

[U64] PHP：目录遍历
来源：http://po.bjjhwx.cn

glob("dir/*.php");  scandir("dir");
来源：http://up.newstarts.cn

[U65] PHP：会话
来源：http://yf.521024.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ab.bookmarksfly.cn

[U66] PHP：设置 Cookie
来源：http://ka.bjjhwx.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sx.muxihuayi.cn

[U67] PHP：处理文件上传
来源：http://qv.bjjhwx.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sn.521024.cn

[U68] PHP：PDO 连接
来源：http://da.jctech888.com.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://el.colortex.cn

[U69] PHP：PDO 预处理
来源：http://oy.bjjhwx.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ia.newstarts.cn

[U70] PHP：PDO 事务
来源：http://fe.huixiangedu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sy.nicolike.cn

[U71] PHP：抛出异常
来源：http://vv.asd995.cn

throw new RuntimeException("失败", 500);
来源：http://xy.nicolike.cn

[U72] PHP：写错误日志
来源：http://ys.szsharing.cn

error_log("失败: " . $e->getMessage());
来源：http://mz.hnjuh.cn

[U73] PHP：读取 ini 配置
来源：http://jf.szxytkj.cn

parse_ini_file("config.ini", true)
来源：http://kb.haigaiapp.cn

[U74] PHP：读取环境变量
来源：http://tf.521024.cn

getenv("APP_ENV") ?: "production"
来源：http://ke.panjiajie.cn

[U75] PHP：依赖注入
来源：http://ov.nicolike.cn

composer require psr/container
来源：http://wq.colortex.cn

[U76] PHP：简单路由
来源：http://yl.bookmarksfly.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://be.521024.cn

[U77] PHP：模板渲染
来源：http://mc.newstarts.cn

composer require twig/twig
来源：http://xm.hahajie.cn

[U78] PHP：单元测试
来源：http://tj.gzmigu.cn

composer require --dev phpunit/phpunit
来源：http://kl.hahajie.cn

[U79] PHP：静态分析
来源：http://om.lnxyls.cn

composer require --dev phpstan/phpstan
来源：http://dt.hahajie.cn

[U80] PHP：代码规范修复
来源：http://hi.shxzukj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qj.wgjwhj.cn

[U81] JS：初始化项目
来源：http://hb.bjjhwx.cn

npm init -y;  npm i express
来源：http://nu.huixiangedu.cn

[U82] JS：package.json 脚本
来源：http://uq.chemitech.net.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://co.panjiajie.cn

[U83] JS：ES Module 导入导出
来源：http://mi.panjiajie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ft.colortex.cn

[U84] JS：CommonJS 写法
来源：http://ds.huixinmuqiang.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wt.panjiajie.cn

[U85] JS：可选链
来源：http://pn.lnxyls.cn

a?.b?.c
来源：http://zf.huixinmuqiang.cn

[U86] JS：空值合并
来源：http://zm.muxihuayi.cn

a ?? b
来源：http://dx.bjjhwx.cn

[U87] JS：解构默认值
来源：http://dq.hnjuh.cn

const { a = 1, b = 2 } = obj;
来源：http://xc.panjiajie.cn

[U88] JS：对象展开合并
来源：http://sj.haigaiapp.cn

{ ...a, ...b }
来源：http://bs.bookmarksfly.cn

[U89] JS：数组去重
来源：http://fi.szxytkj.cn

[...new Set(arr)]
来源：http://nx.shxzskj.cn

[U90] JS：数字数组排序
来源：http://wm.jianghongdianzi.cn

[...arr].sort((a, b) => a - b)
来源：http://qh.nszjky.cn

[U91] JS：对象键值遍历
来源：http://bo.yuntaijiaju.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ql.jctech888.com.cn

[U92] JS：深拷贝
来源：http://ew.panjiajie.cn

structuredClone(obj)
来源：http://hy.hahajie.cn

[U93] JS：模板字符串
来源：http://bd.9csxet.cn

`共 ${n} 条`
来源：http://up.huixinmuqiang.cn

[U94] JS：箭头函数
来源：http://ho.panjiajie.cn

const double = x => x * 2;
来源：http://hq.asd995.cn

[U95] JS：Promise 包装
来源：http://fa.9csxet.cn

new Promise((resolve, reject) => {})
来源：http://fg.huanxung.cn

[U96] JS：async/await 与异常
来源：http://rh.muxihuayi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://id.jianghongdianzi.cn

[U97] JS：并发请求
来源：http://hl.huixinmuqiang.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ur.huixinmuqiang.cn

[U98] JS：fetch 带 JSON
来源：http://aj.nszjky.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qu.newstarts.cn

[U99] JS：事件监听
来源：http://fl.haigaiapp.cn

el.addEventListener("click", e => {})
来源：http://vj.shxzukj.cn

[U100] JS：DOM 查询
来源：http://gp.wgjwhj.cn

document.querySelector(".item")
来源：http://it.szsharing.cn

[U101] JS：classList 操作
来源：http://iu.gzmigu.cn

el.classList.toggle("active")
来源：http://ua.asd995.cn

[U102] JS：本地存储
来源：http://sw.wgjwhj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ot.wgjwhj.cn

[U103] JS：定时器
来源：http://xj.bjjhwx.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://et.huanxung.cn

[U104] JS：防抖
来源：http://sb.jianghongdianzi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ml.haigaiapp.cn

[U105] JS：节流
来源：http://qc.jctech888.com.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jr.wgjwhj.cn

[U106] JS：日期格式化
来源：http://pq.shxzskj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cd.nicolike.cn

[U107] JS：数字千分位
来源：http://tm.wgjwhj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yz.shxzukj.cn

[U108] JS：随机整数
来源：http://os.nszjky.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ap.huixiangedu.cn

[U109] JS：数组分组
来源：http://yk.szxytkj.cn

Object.groupBy(arr, x => x.type)
来源：http://iw.shxzskj.cn

[U110] JS：数组分块
来源：http://yb.yuexingan06.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dp.shxzukj.cn

[U111] JS：对象转 Map
来源：http://ve.huanxung.cn

new Map(Object.entries(obj))
来源：http://gg.haigaiapp.cn

[U112] JS：字符串补位
来源：http://da.hnjuh.cn

"7".padStart(3, "0")
来源：http://wy.colortex.cn


<!-- 参考信息 -->