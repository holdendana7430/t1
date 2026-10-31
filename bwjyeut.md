代发 wailian999

[T23] Swift：函数
来源：http://xv.gzmigu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ix.shtwfgs.cn

[T24] Swift：闭包
来源：http://bn.huixinmuqiang.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ug.muxihuayi.cn

[T25] Swift：结构体
来源：http://gc.lnxyls.cn

struct P { var x: Int }
来源：http://fh.colortex.cn

[T26] Swift：类与重写
来源：http://ps.yuntaijiaju.cn

class A: Base { override func f() {} }
来源：http://kb.newstarts.cn

[T27] Swift：错误处理
来源：http://hh.panjiajie.cn

do { try f() } catch { print(error) }
来源：http://hu.wgjwhj.cn

[T28] Swift：枚举
来源：http://rv.newstarts.cn

enum Color { case red, green }
来源：http://aj.jianghongdianzi.cn

[T29] Swift：guard 提前返回
来源：http://hq.haigaiapp.cn

guard let x = opt else { return }
来源：http://et.muxihuayi.cn

[T30] Swift：协议
来源：http://dw.jctech888.com.cn

protocol Shape { func area() -> Double }
来源：http://cm.nszjky.cn

[T31] Lua：Hello World
来源：http://hf.asd995.cn

print("Hello")
来源：http://bg.9csxet.cn

[T32] Lua：局部变量
来源：http://hg.yuexingan06.cn

local a = 1
来源：http://io.newstarts.cn

[T33] Lua：表（数组）
来源：http://jq.haigaiapp.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://pr.shxzskj.cn

[T34] Lua：遍历表
来源：http://db.yuntaijiaju.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://kc.yuexingan06.cn

[T35] Lua：字典表
来源：http://is.nicolike.cn

local d = { a = 1 };  d.b = 2
来源：http://ic.huixinmuqiang.cn

[T36] Lua：函数
来源：http://qf.newstarts.cn

function add(a, b) return a + b end
来源：http://ma.muxihuayi.cn

[T37] Lua：字符串拼接
来源：http://zm.yuntaijiaju.cn

"a" .. "b"
来源：http://al.lnxyls.cn

[T38] Lua：条件
来源：http://kk.shxzukj.cn

if x > 0 then print("正") end
来源：http://xx.yuntaijiaju.cn

[T39] Lua：模式匹配
来源：http://bk.jianghongdianzi.cn

string.find(s, "%d+")
来源：http://bh.shtwfgs.cn

[T40] Lua：元表
来源：http://sf.nszjky.cn

setmetatable({}, { __index = base })
来源：http://yl.nicolike.cn

[T41] Perl：Hello World
来源：http://ql.hnjuh.cn

print "Hello\n";
来源：http://ia.bookmarksfly.cn

[T42] Perl：变量类型
来源：http://wn.chemitech.net.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zv.yuexingan06.cn

[T43] Perl：字符串插值
来源：http://jh.yuexingan06.cn

"值: $a"
来源：http://lb.wgjwhj.cn

[T44] Perl：条件
来源：http://mn.muxihuayi.cn

if ($a > 0) { print "正"; }
来源：http://jj.chemitech.net.cn

[T45] Perl：数组遍历
来源：http://zp.haigaiapp.cn

for my $x (@arr) { print $x; }
来源：http://rd.lnxyls.cn

[T46] Perl：哈希操作
来源：http://oa.bookmarksfly.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qr.lnxyls.cn

[T47] Perl：正则捕获
来源：http://cz.hnjuh.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://gg.yuexingan06.cn

[T48] Perl：正则替换
来源：http://jg.shxzukj.cn

$s =~ s/old/new/g;
来源：http://ql.huixiangedu.cn

[T49] Perl：函数
来源：http://xi.yuexingan06.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qv.colortex.cn

[T50] Perl：逐行读文件
来源：http://mq.nszjky.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://oi.lnxyls.cn

while (my $line = <$fh>) { print $line; }
来源：http://dm.asd995.cn

[T51] Scala：Hello World
来源：http://pg.lnxyls.cn

println("Hello")
来源：http://wu.huixiangedu.cn

[T52] Scala：变量
来源：http://ia.nszjky.cn

val a = 1;  var b = 2
来源：http://bg.lnxyls.cn

[T53] Scala：字符串插值
来源：http://bx.yuntaijiaju.cn

s"值: $b"
来源：http://ix.chemitech.net.cn

[T54] Scala：集合映射
来源：http://sv.jianghongdianzi.cn

List(1, 2, 3).map(_ * 2)
来源：http://jl.nszjky.cn

[T55] Scala：集合过滤
来源：http://sa.shxzukj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ms.shxzukj.cn

[T56] Scala：样例类
来源：http://pd.nszjky.cn

case class User(name: String, age: Int)
来源：http://qo.yuexingan06.cn

[T57] Scala：模式匹配
来源：http://ys.huanxung.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://lf.shtwfgs.cn

[T58] Scala：函数定义
来源：http://sz.jianghongdianzi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zq.colortex.cn

[T59] Scala：循环
来源：http://sp.haigaiapp.cn

for (i <- 1 to 10) println(i)
来源：http://kc.hnjuh.cn

[T60] Scala：折叠
来源：http://ms.shxzukj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qo.shxzukj.cn

================================================================================
来源：http://ps.shtwfgs.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ow.jianghongdianzi.cn

================================================================================
来源：http://kz.lnxyls.cn

[U01] Py：创建虚拟环境
来源：http://ep.szsharing.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ux.szxytkj.cn

[U02] Py：导出 / 安装依赖
来源：http://jm.chemitech.net.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nk.shxzskj.cn

[U03] Py：加载 .env 配置
来源：http://wi.yuntaijiaju.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ci.shxzskj.cn

[U04] Py：变量调试打印
来源：http://lc.hnjuh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ig.bookmarksfly.cn

[U05] Py：列表去重且保序
来源：http://yw.gzmigu.cn

list(dict.fromkeys(arr))
来源：http://nk.9csxet.cn

[U06] Py：合并两个字典
来源：http://xj.hahajie.cn

{**a, **b}
来源：http://rj.lnxyls.cn

[U07] Py：反转字典键值
来源：http://gk.jctech888.com.cn

{v: k for k, v in d.items()}
来源：http://nj.colortex.cn

[U08] Py：展平二维列表
来源：http://zi.szxytkj.cn

[y for x in nested for y in x]
来源：http://lv.szsharing.cn

[U09] Py：字典取最大值的键
来源：http://no.gzmigu.cn

max(d, key=d.get)
来源：http://dk.shtwfgs.cn

[U10] Py：按值排序字典
来源：http://zy.bookmarksfly.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rk.jianghongdianzi.cn

[U11] Py：生成器表达式
来源：http://rr.nszjky.cn

(x * 2 for x in arr)
来源：http://ca.wgjwhj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://yv.muxihuayi.cn

Counter(arr).most_common(3)
来源：http://cb.yuexingan06.cn

[U13] Py：固定长度队列
来源：http://yh.bjjhwx.cn

deque(maxlen=10)
来源：http://pq.chemitech.net.cn

[U14] Py：分组收集到列表
来源：http://xs.jctech888.com.cn

defaultdict(list)
来源：http://pc.521024.cn

[U15] Py：高精度计时
来源：http://mj.szsharing.cn

t = time.perf_counter()
来源：http://aq.lnxyls.cn

[U16] Py：命令行参数解析
来源：http://vw.huanxung.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://od.panjiajie.cn

[U17] Py：初始化日志
来源：http://mz.newstarts.cn

logging.basicConfig(level=logging.INFO)
来源：http://tj.huanxung.cn

[U18] Py：预编译正则
来源：http://yj.huanxung.cn

pat = re.compile(r"\d+")
来源：http://yf.haigaiapp.cn

[U19] Py：正则替换带回调
来源：http://fm.gzmigu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pp.shxzskj.cn

[U20] Py：缓存函数结果
来源：http://ov.nicolike.cn

@functools.lru_cache(maxsize=None)
来源：http://bw.jianghongdianzi.cn

[U21] Py：自定义上下文管理器
来源：http://oe.bjjhwx.cn

@contextlib.contextmanager
来源：http://ft.yuexingan06.cn

[U22] Py：矩阵转置
来源：http://eg.yuntaijiaju.cn

list(zip(*m))
来源：http://qb.jianghongdianzi.cn

[U23] Py：分块读取大文件
来源：http://od.yuexingan06.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mf.panjiajie.cn

[U24] Py：路径操作
来源：http://om.chemitech.net.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xt.nicolike.cn

[U25] Py：CSV 按字典读
来源：http://xw.bookmarksfly.cn

csv.DictReader(f)
来源：http://sh.9csxet.cn

[U26] Py：并发下载
来源：http://zd.shtwfgs.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vy.huixiangedu.cn

[U27] Py：异步 HTTP
来源：http://yx.yuexingan06.cn

aiohttp.ClientSession() 配合 async with
来源：http://xx.wgjwhj.cn

[U28] Py：类型别名
来源：http://hb.muxihuayi.cn

UserId = int
来源：http://kp.shxzukj.cn

[U29] Py：属性校验
来源：http://id.nszjky.cn

@property 与 @x.setter 配合
来源：http://jg.huixiangedu.cn

[U30] Py：数据类
来源：http://xg.yuexingan06.cn

@dataclass(slots=True)
来源：http://rz.chemitech.net.cn

[U31] Py：单测
来源：http://cl.panjiajie.cn

python -m pytest -q
来源：http://dd.muxihuayi.cn

[U32] Py：代码格式化
来源：http://xg.huixiangedu.cn

ruff format . && ruff check --fix .
来源：http://ja.newstarts.cn

[U33] Py：打包发布
来源：http://vc.shtwfgs.cn

python -m build  （依赖 pyproject.toml）
来源：http://lv.shtwfgs.cn

[U34] Py：判断编码
来源：http://rf.huixinmuqiang.cn

chardet.detect(raw)
来源：http://ja.bookmarksfly.cn

[U35] Py：发送邮件
来源：http://iw.bjjhwx.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ww.gzmigu.cn

[U36] Py：定时任务
来源：http://dm.yuexingan06.cn

schedule.every(10).minutes.do(job)
来源：http://gn.haigaiapp.cn

[U37] Py：读写 Excel
来源：http://ei.jctech888.com.cn

pandas.read_excel / DataFrame.to_excel
来源：http://is.chemitech.net.cn

[U38] Py：获取脚本所在目录
来源：http://qn.nszjky.cn

Path(__file__).resolve().parent
来源：http://np.wgjwhj.cn

[U39] Py：判断是否在交互环境
来源：http://ze.huixiangedu.cn

sys.stdout.isatty()
来源：http://hq.yuexingan06.cn

[U40] Py：打印到标准错误
来源：http://ge.jianghongdianzi.cn

print("err", file=sys.stderr)
来源：http://dq.asd995.cn

[U41] PHP：初始化 Composer 项目
来源：http://vw.chemitech.net.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ml.muxihuayi.cn

[U42] PHP：PSR-4 自动加载
来源：http://or.nszjky.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bv.szxytkj.cn

[U43] PHP：声明命名空间
来源：http://fa.chemitech.net.cn

namespace App\Http;
来源：http://cl.lnxyls.cn

[U44] PHP：开启严格类型
来源：http://ha.jianghongdianzi.cn

declare(strict_types=1);
来源：http://hg.shxzskj.cn

[U45] PHP：类型声明与返回类型
来源：http://vq.nszjky.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://hi.shxzskj.cn

[U46] PHP：可空类型
来源：http://zw.huixiangedu.cn

?string $name = null
来源：http://vf.panjiajie.cn

[U47] PHP：联合类型
来源：http://zm.asd995.cn

int|string $id
来源：http://rp.jianghongdianzi.cn

[U48] PHP：纯枚举
来源：http://zc.huixiangedu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sf.panjiajie.cn

[U49] PHP：只读属性
来源：http://hv.9csxet.cn

public readonly string $name
来源：http://cw.jctech888.com.cn

[U50] PHP：构造器属性提升
来源：http://qx.muxihuayi.cn

public function __construct(private int $id) {}
来源：http://ds.nicolike.cn

[U51] PHP：数组解构
来源：http://nj.gzmigu.cn

[$a, $b] = $arr;
来源：http://rl.colortex.cn

[U52] PHP：箭头函数
来源：http://eg.9csxet.cn

$double = fn($x) => $x * 2;
来源：http://eo.newstarts.cn

[U53] PHP：空合并运算符
来源：http://ra.chemitech.net.cn

$v = $a ?? $b ?? "default";
来源：http://zg.521024.cn

[U54] PHP：空安全调用
来源：http://co.bookmarksfly.cn

$obj?->method()
来源：http://me.jianghongdianzi.cn

[U55] PHP：match 表达式
来源：http://qt.szxytkj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bm.haigaiapp.cn

[U56] PHP：命名参数
来源：http://vm.bjjhwx.cn

f(a: 1, b: 2)
来源：http://rg.yuntaijiaju.cn

[U57] PHP：字符串插值
来源：http://hl.nszjky.cn

"值: {$a}"
来源：http://if.shxzukj.cn

[U58] PHP：数组三件套
来源：http://vh.gzmigu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://la.gzmigu.cn

[U59] PHP：自定义排序
来源：http://by.521024.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pl.szxytkj.cn

[U60] PHP：JSON 编解码
来源：http://cl.muxihuayi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fi.haigaiapp.cn

[U61] PHP：正则
来源：http://gs.szsharing.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ez.szxytkj.cn

[U62] PHP：日期对象
来源：http://fs.yuexingan06.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nk.bookmarksfly.cn

[U63] PHP：文件读写
来源：http://if.hahajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mz.shxzukj.cn

[U64] PHP：目录遍历
来源：http://ua.shxzukj.cn

glob("dir/*.php");  scandir("dir");
来源：http://yt.nicolike.cn

[U65] PHP：会话
来源：http://gj.jctech888.com.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ou.szxytkj.cn

[U66] PHP：设置 Cookie
来源：http://xj.yuexingan06.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ze.yuexingan06.cn

[U67] PHP：处理文件上传
来源：http://ln.lnxyls.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ha.asd995.cn

[U68] PHP：PDO 连接
来源：http://wi.colortex.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gx.jctech888.com.cn

[U69] PHP：PDO 预处理
来源：http://fc.haigaiapp.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jy.huixiangedu.cn

[U70] PHP：PDO 事务
来源：http://ft.huixiangedu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bo.shxzukj.cn

[U71] PHP：抛出异常
来源：http://id.huanxung.cn

throw new RuntimeException("失败", 500);
来源：http://hx.panjiajie.cn

[U72] PHP：写错误日志
来源：http://cx.chemitech.net.cn

error_log("失败: " . $e->getMessage());
来源：http://px.nicolike.cn

[U73] PHP：读取 ini 配置
来源：http://qf.bjjhwx.cn

parse_ini_file("config.ini", true)
来源：http://up.wgjwhj.cn

[U74] PHP：读取环境变量
来源：http://jf.jctech888.com.cn

getenv("APP_ENV") ?: "production"
来源：http://st.521024.cn

[U75] PHP：依赖注入
来源：http://on.bookmarksfly.cn

composer require psr/container
来源：http://bd.nicolike.cn

[U76] PHP：简单路由
来源：http://uu.bookmarksfly.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wv.hahajie.cn

[U77] PHP：模板渲染
来源：http://va.huanxung.cn

composer require twig/twig
来源：http://no.muxihuayi.cn

[U78] PHP：单元测试
来源：http://mf.nszjky.cn

composer require --dev phpunit/phpunit
来源：http://dl.haigaiapp.cn

[U79] PHP：静态分析
来源：http://ea.huixiangedu.cn

composer require --dev phpstan/phpstan
来源：http://wu.gzmigu.cn

[U80] PHP：代码规范修复
来源：http://ks.huanxung.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://kc.shxzukj.cn

[U81] JS：初始化项目
来源：http://dr.asd995.cn

npm init -y;  npm i express
来源：http://cq.shxzukj.cn

[U82] JS：package.json 脚本
来源：http://gx.9csxet.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kl.wgjwhj.cn

[U83] JS：ES Module 导入导出
来源：http://qi.nszjky.cn

export const a = 1;  import { a } from "./m.js";
来源：http://rr.szsharing.cn

[U84] JS：CommonJS 写法
来源：http://ix.9csxet.cn

module.exports = { a };  const { a } = require("./m");
来源：http://sm.szxytkj.cn

[U85] JS：可选链
来源：http://iz.chemitech.net.cn

a?.b?.c
来源：http://nc.asd995.cn

[U86] JS：空值合并
来源：http://ph.colortex.cn

a ?? b
来源：http://lw.lnxyls.cn

[U87] JS：解构默认值
来源：http://zo.yuntaijiaju.cn

const { a = 1, b = 2 } = obj;
来源：http://zs.panjiajie.cn

[U88] JS：对象展开合并
来源：http://hr.szxytkj.cn

{ ...a, ...b }
来源：http://sm.9csxet.cn

[U89] JS：数组去重
来源：http://kp.szxytkj.cn

[...new Set(arr)]
来源：http://gt.wgjwhj.cn

[U90] JS：数字数组排序
来源：http://ws.hnjuh.cn

[...arr].sort((a, b) => a - b)
来源：http://bn.shxzskj.cn

[U91] JS：对象键值遍历
来源：http://ka.haigaiapp.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vt.wgjwhj.cn

[U92] JS：深拷贝
来源：http://xz.gzmigu.cn

structuredClone(obj)
来源：http://fs.asd995.cn

[U93] JS：模板字符串
来源：http://rh.panjiajie.cn

`共 ${n} 条`
来源：http://wy.hnjuh.cn

[U94] JS：箭头函数
来源：http://ej.haigaiapp.cn

const double = x => x * 2;
来源：http://dy.huixinmuqiang.cn

[U95] JS：Promise 包装
来源：http://bc.bjjhwx.cn

new Promise((resolve, reject) => {})
来源：http://lo.shtwfgs.cn

[U96] JS：async/await 与异常
来源：http://ej.colortex.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xx.bjjhwx.cn

[U97] JS：并发请求
来源：http://at.shxzukj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bl.muxihuayi.cn

[U98] JS：fetch 带 JSON
来源：http://gx.szsharing.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ru.chemitech.net.cn

[U99] JS：事件监听
来源：http://ea.9csxet.cn

el.addEventListener("click", e => {})
来源：http://xk.hahajie.cn

[U100] JS：DOM 查询
来源：http://pa.newstarts.cn

document.querySelector(".item")
来源：http://xe.yuexingan06.cn

[U101] JS：classList 操作
来源：http://rp.521024.cn

el.classList.toggle("active")
来源：http://wl.hnjuh.cn

[U102] JS：本地存储
来源：http://vu.szsharing.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://br.chemitech.net.cn

[U103] JS：定时器
来源：http://dp.hnjuh.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://sz.lnxyls.cn

[U104] JS：防抖
来源：http://nc.lnxyls.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fm.nicolike.cn

[U105] JS：节流
来源：http://kj.shxzskj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yo.nszjky.cn

[U106] JS：日期格式化
来源：http://gm.bjjhwx.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://eo.jctech888.com.cn

[U107] JS：数字千分位
来源：http://xz.colortex.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sq.jianghongdianzi.cn

[U108] JS：随机整数
来源：http://tj.nicolike.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://se.hnjuh.cn

[U109] JS：数组分组
来源：http://me.bjjhwx.cn

Object.groupBy(arr, x => x.type)
来源：http://dy.yuexingan06.cn

[U110] JS：数组分块
来源：http://vf.bjjhwx.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ls.newstarts.cn


<!-- 参考信息 -->