代发 wailian999

[T23] Swift：函数
来源：http://wg.lnxyls.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yn.hahajie.cn

[T24] Swift：闭包
来源：http://hu.panjiajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://pl.newstarts.cn

[T25] Swift：结构体
来源：http://vm.hahajie.cn

struct P { var x: Int }
来源：http://bc.chemitech.net.cn

[T26] Swift：类与重写
来源：http://mp.jctech888.com.cn

class A: Base { override func f() {} }
来源：http://hi.haigaiapp.cn

[T27] Swift：错误处理
来源：http://gg.newstarts.cn

do { try f() } catch { print(error) }
来源：http://cm.nicolike.cn

[T28] Swift：枚举
来源：http://al.newstarts.cn

enum Color { case red, green }
来源：http://ej.huanxung.cn

[T29] Swift：guard 提前返回
来源：http://oy.colortex.cn

guard let x = opt else { return }
来源：http://pd.muxihuayi.cn

[T30] Swift：协议
来源：http://oy.bjjhwx.cn

protocol Shape { func area() -> Double }
来源：http://xq.hnjuh.cn

[T31] Lua：Hello World
来源：http://mx.9csxet.cn

print("Hello")
来源：http://sz.yuexingan06.cn

[T32] Lua：局部变量
来源：http://oe.wgjwhj.cn

local a = 1
来源：http://gz.huanxung.cn

[T33] Lua：表（数组）
来源：http://oy.chemitech.net.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://gw.bookmarksfly.cn

[T34] Lua：遍历表
来源：http://dm.huanxung.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ux.muxihuayi.cn

[T35] Lua：字典表
来源：http://ba.huixiangedu.cn

local d = { a = 1 };  d.b = 2
来源：http://os.huixinmuqiang.cn

[T36] Lua：函数
来源：http://hk.asd995.cn

function add(a, b) return a + b end
来源：http://fc.shxzukj.cn

[T37] Lua：字符串拼接
来源：http://gz.hnjuh.cn

"a" .. "b"
来源：http://fn.yuexingan06.cn

[T38] Lua：条件
来源：http://bz.nszjky.cn

if x > 0 then print("正") end
来源：http://rp.yuntaijiaju.cn

[T39] Lua：模式匹配
来源：http://el.szxytkj.cn

string.find(s, "%d+")
来源：http://gd.shxzukj.cn

[T40] Lua：元表
来源：http://tf.lnxyls.cn

setmetatable({}, { __index = base })
来源：http://ly.9csxet.cn

[T41] Perl：Hello World
来源：http://rc.shxzskj.cn

print "Hello\n";
来源：http://gf.shtwfgs.cn

[T42] Perl：变量类型
来源：http://xr.jianghongdianzi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ab.gzmigu.cn

[T43] Perl：字符串插值
来源：http://un.huixiangedu.cn

"值: $a"
来源：http://rp.yuntaijiaju.cn

[T44] Perl：条件
来源：http://tr.huixinmuqiang.cn

if ($a > 0) { print "正"; }
来源：http://cj.shtwfgs.cn

[T45] Perl：数组遍历
来源：http://jo.nicolike.cn

for my $x (@arr) { print $x; }
来源：http://xw.colortex.cn

[T46] Perl：哈希操作
来源：http://we.chemitech.net.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://yo.haigaiapp.cn

[T47] Perl：正则捕获
来源：http://xf.nszjky.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://iz.bookmarksfly.cn

[T48] Perl：正则替换
来源：http://xi.huixiangedu.cn

$s =~ s/old/new/g;
来源：http://le.shxzukj.cn

[T49] Perl：函数
来源：http://bh.lnxyls.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cy.chemitech.net.cn

[T50] Perl：逐行读文件
来源：http://dn.hahajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ti.muxihuayi.cn

while (my $line = <$fh>) { print $line; }
来源：http://lk.newstarts.cn

[T51] Scala：Hello World
来源：http://wv.shtwfgs.cn

println("Hello")
来源：http://ou.9csxet.cn

[T52] Scala：变量
来源：http://is.panjiajie.cn

val a = 1;  var b = 2
来源：http://bb.panjiajie.cn

[T53] Scala：字符串插值
来源：http://qi.huixiangedu.cn

s"值: $b"
来源：http://rk.asd995.cn

[T54] Scala：集合映射
来源：http://wu.521024.cn

List(1, 2, 3).map(_ * 2)
来源：http://ay.hahajie.cn

[T55] Scala：集合过滤
来源：http://cf.colortex.cn

List(1, 2, 3).filter(_ > 1)
来源：http://uq.jianghongdianzi.cn

[T56] Scala：样例类
来源：http://sj.chemitech.net.cn

case class User(name: String, age: Int)
来源：http://lz.newstarts.cn

[T57] Scala：模式匹配
来源：http://ni.9csxet.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://la.shtwfgs.cn

[T58] Scala：函数定义
来源：http://ai.521024.cn

def add(a: Int, b: Int): Int = a + b
来源：http://aw.szxytkj.cn

[T59] Scala：循环
来源：http://cn.panjiajie.cn

for (i <- 1 to 10) println(i)
来源：http://tp.shxzukj.cn

[T60] Scala：折叠
来源：http://om.yuexingan06.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zp.shxzskj.cn

================================================================================
来源：http://rd.gzmigu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ao.shxzukj.cn

================================================================================
来源：http://lh.szsharing.cn

[U01] Py：创建虚拟环境
来源：http://jh.hnjuh.cn

python -m venv .venv && source .venv/bin/activate
来源：http://hm.hnjuh.cn

[U02] Py：导出 / 安装依赖
来源：http://wi.shxzskj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://it.haigaiapp.cn

[U03] Py：加载 .env 配置
来源：http://ps.gzmigu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://jq.huanxung.cn

[U04] Py：变量调试打印
来源：http://lz.asd995.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://td.asd995.cn

[U05] Py：列表去重且保序
来源：http://le.haigaiapp.cn

list(dict.fromkeys(arr))
来源：http://fm.gzmigu.cn

[U06] Py：合并两个字典
来源：http://kq.huixiangedu.cn

{**a, **b}
来源：http://nw.9csxet.cn

[U07] Py：反转字典键值
来源：http://cc.newstarts.cn

{v: k for k, v in d.items()}
来源：http://lj.jianghongdianzi.cn

[U08] Py：展平二维列表
来源：http://dm.nszjky.cn

[y for x in nested for y in x]
来源：http://jd.asd995.cn

[U09] Py：字典取最大值的键
来源：http://cp.shtwfgs.cn

max(d, key=d.get)
来源：http://zw.colortex.cn

[U10] Py：按值排序字典
来源：http://cn.lnxyls.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hn.chemitech.net.cn

[U11] Py：生成器表达式
来源：http://nf.wgjwhj.cn

(x * 2 for x in arr)
来源：http://nw.newstarts.cn

[U12] Py：取出现最多的 3 个元素
来源：http://nz.9csxet.cn

Counter(arr).most_common(3)
来源：http://ru.gzmigu.cn

[U13] Py：固定长度队列
来源：http://fo.nicolike.cn

deque(maxlen=10)
来源：http://hl.szxytkj.cn

[U14] Py：分组收集到列表
来源：http://kf.hnjuh.cn

defaultdict(list)
来源：http://lx.asd995.cn

[U15] Py：高精度计时
来源：http://kr.colortex.cn

t = time.perf_counter()
来源：http://le.shxzskj.cn

[U16] Py：命令行参数解析
来源：http://ol.newstarts.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rm.shxzukj.cn

[U17] Py：初始化日志
来源：http://ic.muxihuayi.cn

logging.basicConfig(level=logging.INFO)
来源：http://ul.haigaiapp.cn

[U18] Py：预编译正则
来源：http://pv.shxzukj.cn

pat = re.compile(r"\d+")
来源：http://hu.nicolike.cn

[U19] Py：正则替换带回调
来源：http://mx.jctech888.com.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lm.jianghongdianzi.cn

[U20] Py：缓存函数结果
来源：http://sl.hahajie.cn

@functools.lru_cache(maxsize=None)
来源：http://gz.szxytkj.cn

[U21] Py：自定义上下文管理器
来源：http://ss.wgjwhj.cn

@contextlib.contextmanager
来源：http://sg.yuntaijiaju.cn

[U22] Py：矩阵转置
来源：http://oi.9csxet.cn

list(zip(*m))
来源：http://ct.wgjwhj.cn

[U23] Py：分块读取大文件
来源：http://dg.hnjuh.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://md.bookmarksfly.cn

[U24] Py：路径操作
来源：http://hp.newstarts.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kh.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://pz.shxzukj.cn

csv.DictReader(f)
来源：http://nh.chemitech.net.cn

[U26] Py：并发下载
来源：http://tk.gzmigu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pt.hnjuh.cn

[U27] Py：异步 HTTP
来源：http://zn.asd995.cn

aiohttp.ClientSession() 配合 async with
来源：http://qi.huanxung.cn

[U28] Py：类型别名
来源：http://yb.haigaiapp.cn

UserId = int
来源：http://cb.nicolike.cn

[U29] Py：属性校验
来源：http://na.huixinmuqiang.cn

@property 与 @x.setter 配合
来源：http://hq.haigaiapp.cn

[U30] Py：数据类
来源：http://yz.szsharing.cn

@dataclass(slots=True)
来源：http://ab.lnxyls.cn

[U31] Py：单测
来源：http://fg.shxzskj.cn

python -m pytest -q
来源：http://yo.panjiajie.cn

[U32] Py：代码格式化
来源：http://gd.muxihuayi.cn

ruff format . && ruff check --fix .
来源：http://nw.panjiajie.cn

[U33] Py：打包发布
来源：http://vc.bookmarksfly.cn

python -m build  （依赖 pyproject.toml）
来源：http://wy.jctech888.com.cn

[U34] Py：判断编码
来源：http://hl.wgjwhj.cn

chardet.detect(raw)
来源：http://xs.jctech888.com.cn

[U35] Py：发送邮件
来源：http://sg.muxihuayi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tf.chemitech.net.cn

[U36] Py：定时任务
来源：http://sy.lnxyls.cn

schedule.every(10).minutes.do(job)
来源：http://uh.bjjhwx.cn

[U37] Py：读写 Excel
来源：http://wq.panjiajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://mb.huanxung.cn

[U38] Py：获取脚本所在目录
来源：http://hc.huixiangedu.cn

Path(__file__).resolve().parent
来源：http://jx.jctech888.com.cn

[U39] Py：判断是否在交互环境
来源：http://ug.shxzukj.cn

sys.stdout.isatty()
来源：http://ak.bjjhwx.cn

[U40] Py：打印到标准错误
来源：http://hq.shxzukj.cn

print("err", file=sys.stderr)
来源：http://yi.yuexingan06.cn

[U41] PHP：初始化 Composer 项目
来源：http://qy.yuntaijiaju.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ab.yuntaijiaju.cn

[U42] PHP：PSR-4 自动加载
来源：http://tg.hahajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xo.lnxyls.cn

[U43] PHP：声明命名空间
来源：http://sj.yuntaijiaju.cn

namespace App\Http;
来源：http://qa.chemitech.net.cn

[U44] PHP：开启严格类型
来源：http://te.bookmarksfly.cn

declare(strict_types=1);
来源：http://ij.bjjhwx.cn

[U45] PHP：类型声明与返回类型
来源：http://rw.chemitech.net.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://xt.asd995.cn

[U46] PHP：可空类型
来源：http://ug.bjjhwx.cn

?string $name = null
来源：http://el.chemitech.net.cn

[U47] PHP：联合类型
来源：http://sq.shxzukj.cn

int|string $id
来源：http://du.shxzskj.cn

[U48] PHP：纯枚举
来源：http://ay.hnjuh.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gm.nszjky.cn

[U49] PHP：只读属性
来源：http://sz.bookmarksfly.cn

public readonly string $name
来源：http://gw.jctech888.com.cn

[U50] PHP：构造器属性提升
来源：http://my.nicolike.cn

public function __construct(private int $id) {}
来源：http://ca.shxzskj.cn

[U51] PHP：数组解构
来源：http://zr.huanxung.cn

[$a, $b] = $arr;
来源：http://dx.huanxung.cn

[U52] PHP：箭头函数
来源：http://yd.jianghongdianzi.cn

$double = fn($x) => $x * 2;
来源：http://yp.bookmarksfly.cn

[U53] PHP：空合并运算符
来源：http://rv.shtwfgs.cn

$v = $a ?? $b ?? "default";
来源：http://ql.huixinmuqiang.cn

[U54] PHP：空安全调用
来源：http://va.newstarts.cn

$obj?->method()
来源：http://ey.wgjwhj.cn

[U55] PHP：match 表达式
来源：http://ic.jctech888.com.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cu.lnxyls.cn

[U56] PHP：命名参数
来源：http://jx.bookmarksfly.cn

f(a: 1, b: 2)
来源：http://id.jianghongdianzi.cn

[U57] PHP：字符串插值
来源：http://tx.bjjhwx.cn

"值: {$a}"
来源：http://gk.huanxung.cn

[U58] PHP：数组三件套
来源：http://ak.lnxyls.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wx.yuntaijiaju.cn

[U59] PHP：自定义排序
来源：http://ru.szxytkj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yz.bookmarksfly.cn

[U60] PHP：JSON 编解码
来源：http://lg.bjjhwx.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fx.jianghongdianzi.cn

[U61] PHP：正则
来源：http://bo.nicolike.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hy.huixiangedu.cn

[U62] PHP：日期对象
来源：http://ph.521024.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ol.gzmigu.cn

[U63] PHP：文件读写
来源：http://th.wgjwhj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wa.nicolike.cn

[U64] PHP：目录遍历
来源：http://oc.hahajie.cn

glob("dir/*.php");  scandir("dir");
来源：http://en.jianghongdianzi.cn

[U65] PHP：会话
来源：http://qn.nszjky.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://it.huixiangedu.cn

[U66] PHP：设置 Cookie
来源：http://sk.panjiajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qs.haigaiapp.cn

[U67] PHP：处理文件上传
来源：http://lz.lnxyls.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ni.shxzukj.cn

[U68] PHP：PDO 连接
来源：http://ze.haigaiapp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://oo.colortex.cn

[U69] PHP：PDO 预处理
来源：http://bm.colortex.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ta.yuntaijiaju.cn

[U70] PHP：PDO 事务
来源：http://ie.gzmigu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ac.bjjhwx.cn

[U71] PHP：抛出异常
来源：http://bj.szxytkj.cn

throw new RuntimeException("失败", 500);
来源：http://la.haigaiapp.cn

[U72] PHP：写错误日志
来源：http://ft.huixinmuqiang.cn

error_log("失败: " . $e->getMessage());
来源：http://ls.colortex.cn

[U73] PHP：读取 ini 配置
来源：http://ie.muxihuayi.cn

parse_ini_file("config.ini", true)
来源：http://gh.asd995.cn

[U74] PHP：读取环境变量
来源：http://ah.asd995.cn

getenv("APP_ENV") ?: "production"
来源：http://sf.newstarts.cn

[U75] PHP：依赖注入
来源：http://ie.szsharing.cn

composer require psr/container
来源：http://ug.9csxet.cn

[U76] PHP：简单路由
来源：http://gm.newstarts.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xy.shxzskj.cn

[U77] PHP：模板渲染
来源：http://jx.chemitech.net.cn

composer require twig/twig
来源：http://xa.521024.cn

[U78] PHP：单元测试
来源：http://aj.nszjky.cn

composer require --dev phpunit/phpunit
来源：http://ik.bjjhwx.cn

[U79] PHP：静态分析
来源：http://zx.gzmigu.cn

composer require --dev phpstan/phpstan
来源：http://pk.shxzukj.cn

[U80] PHP：代码规范修复
来源：http://jn.muxihuayi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ii.shtwfgs.cn

[U81] JS：初始化项目
来源：http://tx.wgjwhj.cn

npm init -y;  npm i express
来源：http://dp.colortex.cn

[U82] JS：package.json 脚本
来源：http://kf.yuexingan06.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xv.hnjuh.cn

[U83] JS：ES Module 导入导出
来源：http://fc.huixiangedu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://un.panjiajie.cn

[U84] JS：CommonJS 写法
来源：http://vf.newstarts.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ai.hnjuh.cn

[U85] JS：可选链
来源：http://ko.jctech888.com.cn

a?.b?.c
来源：http://nl.jctech888.com.cn

[U86] JS：空值合并
来源：http://am.nicolike.cn

a ?? b
来源：http://lp.nicolike.cn

[U87] JS：解构默认值
来源：http://am.haigaiapp.cn

const { a = 1, b = 2 } = obj;
来源：http://hy.chemitech.net.cn

[U88] JS：对象展开合并
来源：http://cg.gzmigu.cn

{ ...a, ...b }
来源：http://qo.9csxet.cn

[U89] JS：数组去重
来源：http://ti.huixinmuqiang.cn

[...new Set(arr)]
来源：http://tc.haigaiapp.cn

[U90] JS：数字数组排序
来源：http://zf.nszjky.cn

[...arr].sort((a, b) => a - b)
来源：http://us.nszjky.cn

[U91] JS：对象键值遍历
来源：http://hg.521024.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://et.yuntaijiaju.cn

[U92] JS：深拷贝
来源：http://pw.shxzukj.cn

structuredClone(obj)
来源：http://qp.9csxet.cn

[U93] JS：模板字符串
来源：http://zd.yuntaijiaju.cn

`共 ${n} 条`
来源：http://qa.chemitech.net.cn

[U94] JS：箭头函数
来源：http://hb.jianghongdianzi.cn

const double = x => x * 2;
来源：http://ij.shtwfgs.cn

[U95] JS：Promise 包装
来源：http://ii.hnjuh.cn

new Promise((resolve, reject) => {})
来源：http://ud.shxzskj.cn

[U96] JS：async/await 与异常
来源：http://hd.shxzukj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nd.bjjhwx.cn

[U97] JS：并发请求
来源：http://is.colortex.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://uo.shtwfgs.cn

[U98] JS：fetch 带 JSON
来源：http://kr.muxihuayi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ju.jianghongdianzi.cn

[U99] JS：事件监听
来源：http://hg.chemitech.net.cn

el.addEventListener("click", e => {})
来源：http://rt.shxzskj.cn

[U100] JS：DOM 查询
来源：http://zp.muxihuayi.cn

document.querySelector(".item")
来源：http://ra.huanxung.cn

[U101] JS：classList 操作
来源：http://vm.muxihuayi.cn

el.classList.toggle("active")
来源：http://eo.shxzukj.cn

[U102] JS：本地存储
来源：http://lm.hahajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ai.shtwfgs.cn

[U103] JS：定时器
来源：http://km.nicolike.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://sb.yuntaijiaju.cn

[U104] JS：防抖
来源：http://qq.asd995.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mj.panjiajie.cn

[U105] JS：节流
来源：http://sb.lnxyls.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ld.asd995.cn

[U106] JS：日期格式化
来源：http://ky.huixiangedu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fq.hnjuh.cn

[U107] JS：数字千分位
来源：http://zp.shxzukj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ym.9csxet.cn

[U108] JS：随机整数
来源：http://yp.yuexingan06.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pb.colortex.cn

[U109] JS：数组分组
来源：http://kc.jianghongdianzi.cn

Object.groupBy(arr, x => x.type)
来源：http://ky.szsharing.cn

[U110] JS：数组分块
来源：http://wt.yuexingan06.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://px.bookmarksfly.cn


<!-- 参考信息 -->