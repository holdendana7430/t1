代发 wailian999

[T23] Swift：函数
来源：http://gh.lnxyls.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rc.9csxet.cn

[T24] Swift：闭包
来源：http://st.szsharing.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xn.colortex.cn

[T25] Swift：结构体
来源：http://gr.jianghongdianzi.cn

struct P { var x: Int }
来源：http://iq.nicolike.cn

[T26] Swift：类与重写
来源：http://fb.chemitech.net.cn

class A: Base { override func f() {} }
来源：http://mr.wgjwhj.cn

[T27] Swift：错误处理
来源：http://es.hahajie.cn

do { try f() } catch { print(error) }
来源：http://rm.yuexingan06.cn

[T28] Swift：枚举
来源：http://oc.chemitech.net.cn

enum Color { case red, green }
来源：http://wt.jianghongdianzi.cn

[T29] Swift：guard 提前返回
来源：http://gl.jianghongdianzi.cn

guard let x = opt else { return }
来源：http://kw.hahajie.cn

[T30] Swift：协议
来源：http://sb.colortex.cn

protocol Shape { func area() -> Double }
来源：http://fj.9csxet.cn

[T31] Lua：Hello World
来源：http://jz.jianghongdianzi.cn

print("Hello")
来源：http://jn.jianghongdianzi.cn

[T32] Lua：局部变量
来源：http://hh.haigaiapp.cn

local a = 1
来源：http://go.9csxet.cn

[T33] Lua：表（数组）
来源：http://sc.szsharing.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zq.colortex.cn

[T34] Lua：遍历表
来源：http://eq.shtwfgs.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://fr.yuntaijiaju.cn

[T35] Lua：字典表
来源：http://ez.shxzukj.cn

local d = { a = 1 };  d.b = 2
来源：http://uq.gzmigu.cn

[T36] Lua：函数
来源：http://nm.nszjky.cn

function add(a, b) return a + b end
来源：http://ky.521024.cn

[T37] Lua：字符串拼接
来源：http://tr.asd995.cn

"a" .. "b"
来源：http://ru.haigaiapp.cn

[T38] Lua：条件
来源：http://ug.9csxet.cn

if x > 0 then print("正") end
来源：http://wp.jctech888.com.cn

[T39] Lua：模式匹配
来源：http://yh.panjiajie.cn

string.find(s, "%d+")
来源：http://xg.hnjuh.cn

[T40] Lua：元表
来源：http://on.colortex.cn

setmetatable({}, { __index = base })
来源：http://wj.huixiangedu.cn

[T41] Perl：Hello World
来源：http://em.huanxung.cn

print "Hello\n";
来源：http://oi.jianghongdianzi.cn

[T42] Perl：变量类型
来源：http://ke.nicolike.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://eq.chemitech.net.cn

[T43] Perl：字符串插值
来源：http://zo.yuexingan06.cn

"值: $a"
来源：http://aa.gzmigu.cn

[T44] Perl：条件
来源：http://wy.nszjky.cn

if ($a > 0) { print "正"; }
来源：http://vh.shtwfgs.cn

[T45] Perl：数组遍历
来源：http://ip.bookmarksfly.cn

for my $x (@arr) { print $x; }
来源：http://ql.lnxyls.cn

[T46] Perl：哈希操作
来源：http://ip.shxzskj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uz.huixiangedu.cn

[T47] Perl：正则捕获
来源：http://mt.nicolike.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pc.haigaiapp.cn

[T48] Perl：正则替换
来源：http://sc.nicolike.cn

$s =~ s/old/new/g;
来源：http://jj.bookmarksfly.cn

[T49] Perl：函数
来源：http://cj.muxihuayi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ej.huanxung.cn

[T50] Perl：逐行读文件
来源：http://ir.shtwfgs.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xg.huixiangedu.cn

while (my $line = <$fh>) { print $line; }
来源：http://eu.muxihuayi.cn

[T51] Scala：Hello World
来源：http://kp.bookmarksfly.cn

println("Hello")
来源：http://nd.colortex.cn

[T52] Scala：变量
来源：http://wn.muxihuayi.cn

val a = 1;  var b = 2
来源：http://sx.gzmigu.cn

[T53] Scala：字符串插值
来源：http://tb.lnxyls.cn

s"值: $b"
来源：http://pb.nszjky.cn

[T54] Scala：集合映射
来源：http://qf.huanxung.cn

List(1, 2, 3).map(_ * 2)
来源：http://kv.asd995.cn

[T55] Scala：集合过滤
来源：http://ng.shtwfgs.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ar.newstarts.cn

[T56] Scala：样例类
来源：http://ub.hahajie.cn

case class User(name: String, age: Int)
来源：http://ur.asd995.cn

[T57] Scala：模式匹配
来源：http://vn.9csxet.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://zc.yuexingan06.cn

[T58] Scala：函数定义
来源：http://cs.shxzskj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://oo.bookmarksfly.cn

[T59] Scala：循环
来源：http://aq.shtwfgs.cn

for (i <- 1 to 10) println(i)
来源：http://ft.shxzukj.cn

[T60] Scala：折叠
来源：http://om.huixinmuqiang.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tl.yuexingan06.cn

================================================================================
来源：http://je.huixinmuqiang.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xa.wgjwhj.cn

================================================================================
来源：http://hf.9csxet.cn

[U01] Py：创建虚拟环境
来源：http://rp.panjiajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://gk.nszjky.cn

[U02] Py：导出 / 安装依赖
来源：http://aa.szxytkj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mw.jianghongdianzi.cn

[U03] Py：加载 .env 配置
来源：http://gb.jianghongdianzi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://mr.szsharing.cn

[U04] Py：变量调试打印
来源：http://zy.szxytkj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ni.colortex.cn

[U05] Py：列表去重且保序
来源：http://gb.haigaiapp.cn

list(dict.fromkeys(arr))
来源：http://lv.shxzskj.cn

[U06] Py：合并两个字典
来源：http://sl.yuntaijiaju.cn

{**a, **b}
来源：http://sf.huanxung.cn

[U07] Py：反转字典键值
来源：http://sn.shxzukj.cn

{v: k for k, v in d.items()}
来源：http://km.nszjky.cn

[U08] Py：展平二维列表
来源：http://sl.asd995.cn

[y for x in nested for y in x]
来源：http://om.bjjhwx.cn

[U09] Py：字典取最大值的键
来源：http://ub.yuntaijiaju.cn

max(d, key=d.get)
来源：http://us.jianghongdianzi.cn

[U10] Py：按值排序字典
来源：http://gw.jianghongdianzi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tz.asd995.cn

[U11] Py：生成器表达式
来源：http://mr.gzmigu.cn

(x * 2 for x in arr)
来源：http://qr.huixiangedu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://bv.huixinmuqiang.cn

Counter(arr).most_common(3)
来源：http://wj.wgjwhj.cn

[U13] Py：固定长度队列
来源：http://uq.jctech888.com.cn

deque(maxlen=10)
来源：http://va.bjjhwx.cn

[U14] Py：分组收集到列表
来源：http://xk.wgjwhj.cn

defaultdict(list)
来源：http://mw.huanxung.cn

[U15] Py：高精度计时
来源：http://zy.yuntaijiaju.cn

t = time.perf_counter()
来源：http://ke.yuntaijiaju.cn

[U16] Py：命令行参数解析
来源：http://mr.huanxung.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dj.bjjhwx.cn

[U17] Py：初始化日志
来源：http://nu.bjjhwx.cn

logging.basicConfig(level=logging.INFO)
来源：http://oh.gzmigu.cn

[U18] Py：预编译正则
来源：http://pd.shxzskj.cn

pat = re.compile(r"\d+")
来源：http://vm.colortex.cn

[U19] Py：正则替换带回调
来源：http://tx.colortex.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ti.haigaiapp.cn

[U20] Py：缓存函数结果
来源：http://lt.lnxyls.cn

@functools.lru_cache(maxsize=None)
来源：http://ay.hnjuh.cn

[U21] Py：自定义上下文管理器
来源：http://ck.muxihuayi.cn

@contextlib.contextmanager
来源：http://qx.colortex.cn

[U22] Py：矩阵转置
来源：http://pr.521024.cn

list(zip(*m))
来源：http://rv.chemitech.net.cn

[U23] Py：分块读取大文件
来源：http://hx.szsharing.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xq.shtwfgs.cn

[U24] Py：路径操作
来源：http://vk.hnjuh.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nt.panjiajie.cn

[U25] Py：CSV 按字典读
来源：http://lg.nszjky.cn

csv.DictReader(f)
来源：http://ho.lnxyls.cn

[U26] Py：并发下载
来源：http://uh.jctech888.com.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wj.jctech888.com.cn

[U27] Py：异步 HTTP
来源：http://fr.huanxung.cn

aiohttp.ClientSession() 配合 async with
来源：http://kg.chemitech.net.cn

[U28] Py：类型别名
来源：http://ql.hnjuh.cn

UserId = int
来源：http://mc.chemitech.net.cn

[U29] Py：属性校验
来源：http://qf.jctech888.com.cn

@property 与 @x.setter 配合
来源：http://ce.shtwfgs.cn

[U30] Py：数据类
来源：http://jw.huixiangedu.cn

@dataclass(slots=True)
来源：http://rp.bookmarksfly.cn

[U31] Py：单测
来源：http://xr.huanxung.cn

python -m pytest -q
来源：http://cd.wgjwhj.cn

[U32] Py：代码格式化
来源：http://gq.521024.cn

ruff format . && ruff check --fix .
来源：http://iz.lnxyls.cn

[U33] Py：打包发布
来源：http://mp.bjjhwx.cn

python -m build  （依赖 pyproject.toml）
来源：http://cy.panjiajie.cn

[U34] Py：判断编码
来源：http://as.bjjhwx.cn

chardet.detect(raw)
来源：http://av.yuexingan06.cn

[U35] Py：发送邮件
来源：http://es.huanxung.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ck.bjjhwx.cn

[U36] Py：定时任务
来源：http://el.bjjhwx.cn

schedule.every(10).minutes.do(job)
来源：http://iz.szsharing.cn

[U37] Py：读写 Excel
来源：http://hx.nszjky.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ly.bookmarksfly.cn

[U38] Py：获取脚本所在目录
来源：http://xu.yuexingan06.cn

Path(__file__).resolve().parent
来源：http://xx.nicolike.cn

[U39] Py：判断是否在交互环境
来源：http://ei.shxzskj.cn

sys.stdout.isatty()
来源：http://xe.huixinmuqiang.cn

[U40] Py：打印到标准错误
来源：http://ac.521024.cn

print("err", file=sys.stderr)
来源：http://gt.bookmarksfly.cn

[U41] PHP：初始化 Composer 项目
来源：http://mc.gzmigu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://us.yuexingan06.cn

[U42] PHP：PSR-4 自动加载
来源：http://cs.jctech888.com.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bw.jctech888.com.cn

[U43] PHP：声明命名空间
来源：http://wi.szsharing.cn

namespace App\Http;
来源：http://uv.wgjwhj.cn

[U44] PHP：开启严格类型
来源：http://tb.nicolike.cn

declare(strict_types=1);
来源：http://le.haigaiapp.cn

[U45] PHP：类型声明与返回类型
来源：http://go.huixiangedu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://dh.bookmarksfly.cn

[U46] PHP：可空类型
来源：http://jh.wgjwhj.cn

?string $name = null
来源：http://si.yuntaijiaju.cn

[U47] PHP：联合类型
来源：http://jh.bjjhwx.cn

int|string $id
来源：http://fj.chemitech.net.cn

[U48] PHP：纯枚举
来源：http://vi.asd995.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ni.jianghongdianzi.cn

[U49] PHP：只读属性
来源：http://jl.panjiajie.cn

public readonly string $name
来源：http://rx.panjiajie.cn

[U50] PHP：构造器属性提升
来源：http://jk.panjiajie.cn

public function __construct(private int $id) {}
来源：http://kt.jctech888.com.cn

[U51] PHP：数组解构
来源：http://li.huixinmuqiang.cn

[$a, $b] = $arr;
来源：http://zs.hahajie.cn

[U52] PHP：箭头函数
来源：http://hx.shtwfgs.cn

$double = fn($x) => $x * 2;
来源：http://kt.hahajie.cn

[U53] PHP：空合并运算符
来源：http://dn.bjjhwx.cn

$v = $a ?? $b ?? "default";
来源：http://du.wgjwhj.cn

[U54] PHP：空安全调用
来源：http://wt.lnxyls.cn

$obj?->method()
来源：http://vr.yuexingan06.cn

[U55] PHP：match 表达式
来源：http://qx.huixinmuqiang.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://sn.nicolike.cn

[U56] PHP：命名参数
来源：http://yz.jianghongdianzi.cn

f(a: 1, b: 2)
来源：http://hj.haigaiapp.cn

[U57] PHP：字符串插值
来源：http://my.hnjuh.cn

"值: {$a}"
来源：http://ey.shxzukj.cn

[U58] PHP：数组三件套
来源：http://sz.yuexingan06.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://uw.huixiangedu.cn

[U59] PHP：自定义排序
来源：http://np.9csxet.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uh.szxytkj.cn

[U60] PHP：JSON 编解码
来源：http://vx.colortex.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rt.nicolike.cn

[U61] PHP：正则
来源：http://kj.szxytkj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vi.lnxyls.cn

[U62] PHP：日期对象
来源：http://vu.lnxyls.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jr.521024.cn

[U63] PHP：文件读写
来源：http://ys.bookmarksfly.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mx.asd995.cn

[U64] PHP：目录遍历
来源：http://wx.jctech888.com.cn

glob("dir/*.php");  scandir("dir");
来源：http://be.9csxet.cn

[U65] PHP：会话
来源：http://zf.nszjky.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://fe.wgjwhj.cn

[U66] PHP：设置 Cookie
来源：http://jk.muxihuayi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xo.jianghongdianzi.cn

[U67] PHP：处理文件上传
来源：http://nd.hahajie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vc.jianghongdianzi.cn

[U68] PHP：PDO 连接
来源：http://vm.haigaiapp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xz.hahajie.cn

[U69] PHP：PDO 预处理
来源：http://xr.nszjky.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lf.jianghongdianzi.cn

[U70] PHP：PDO 事务
来源：http://ey.yuexingan06.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dl.yuntaijiaju.cn

[U71] PHP：抛出异常
来源：http://rl.yuntaijiaju.cn

throw new RuntimeException("失败", 500);
来源：http://dw.newstarts.cn

[U72] PHP：写错误日志
来源：http://iw.panjiajie.cn

error_log("失败: " . $e->getMessage());
来源：http://ww.nszjky.cn

[U73] PHP：读取 ini 配置
来源：http://sp.bookmarksfly.cn

parse_ini_file("config.ini", true)
来源：http://oh.huanxung.cn

[U74] PHP：读取环境变量
来源：http://nz.bookmarksfly.cn

getenv("APP_ENV") ?: "production"
来源：http://ki.asd995.cn

[U75] PHP：依赖注入
来源：http://wf.szsharing.cn

composer require psr/container
来源：http://vh.hnjuh.cn

[U76] PHP：简单路由
来源：http://qn.bjjhwx.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lj.haigaiapp.cn

[U77] PHP：模板渲染
来源：http://ny.yuntaijiaju.cn

composer require twig/twig
来源：http://gy.bjjhwx.cn

[U78] PHP：单元测试
来源：http://ox.yuntaijiaju.cn

composer require --dev phpunit/phpunit
来源：http://li.shxzukj.cn

[U79] PHP：静态分析
来源：http://um.9csxet.cn

composer require --dev phpstan/phpstan
来源：http://xf.hahajie.cn

[U80] PHP：代码规范修复
来源：http://nh.szxytkj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ji.wgjwhj.cn

[U81] JS：初始化项目
来源：http://id.bjjhwx.cn

npm init -y;  npm i express
来源：http://xy.yuexingan06.cn

[U82] JS：package.json 脚本
来源：http://hx.muxihuayi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hp.szxytkj.cn

[U83] JS：ES Module 导入导出
来源：http://xv.shxzskj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ue.asd995.cn

[U84] JS：CommonJS 写法
来源：http://zo.9csxet.cn

module.exports = { a };  const { a } = require("./m");
来源：http://am.nszjky.cn

[U85] JS：可选链
来源：http://ux.nicolike.cn

a?.b?.c
来源：http://pg.gzmigu.cn

[U86] JS：空值合并
来源：http://dp.bookmarksfly.cn

a ?? b
来源：http://kv.haigaiapp.cn

[U87] JS：解构默认值
来源：http://bb.hahajie.cn

const { a = 1, b = 2 } = obj;
来源：http://sl.wgjwhj.cn

[U88] JS：对象展开合并
来源：http://cl.hahajie.cn

{ ...a, ...b }
来源：http://ve.hnjuh.cn

[U89] JS：数组去重
来源：http://wm.colortex.cn

[...new Set(arr)]
来源：http://kq.yuntaijiaju.cn

[U90] JS：数字数组排序
来源：http://hj.yuntaijiaju.cn

[...arr].sort((a, b) => a - b)
来源：http://nl.szxytkj.cn

[U91] JS：对象键值遍历
来源：http://xe.gzmigu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ex.nicolike.cn

[U92] JS：深拷贝
来源：http://mm.szsharing.cn

structuredClone(obj)
来源：http://ew.muxihuayi.cn

[U93] JS：模板字符串
来源：http://vq.9csxet.cn

`共 ${n} 条`
来源：http://ms.bookmarksfly.cn

[U94] JS：箭头函数
来源：http://ar.wgjwhj.cn

const double = x => x * 2;
来源：http://me.shxzukj.cn

[U95] JS：Promise 包装
来源：http://kt.huixiangedu.cn

new Promise((resolve, reject) => {})
来源：http://pa.bookmarksfly.cn

[U96] JS：async/await 与异常
来源：http://cv.wgjwhj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pq.huixinmuqiang.cn

[U97] JS：并发请求
来源：http://ha.colortex.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qk.hnjuh.cn

[U98] JS：fetch 带 JSON
来源：http://nh.521024.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://us.shtwfgs.cn

[U99] JS：事件监听
来源：http://qf.lnxyls.cn

el.addEventListener("click", e => {})
来源：http://to.shtwfgs.cn

[U100] JS：DOM 查询
来源：http://kl.haigaiapp.cn

document.querySelector(".item")
来源：http://io.muxihuayi.cn

[U101] JS：classList 操作
来源：http://wd.muxihuayi.cn

el.classList.toggle("active")
来源：http://im.szxytkj.cn

[U102] JS：本地存储
来源：http://lz.shxzukj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ic.yuntaijiaju.cn

[U103] JS：定时器
来源：http://yz.bookmarksfly.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://cn.jctech888.com.cn

[U104] JS：防抖
来源：http://yu.gzmigu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cl.huanxung.cn

[U105] JS：节流
来源：http://zi.haigaiapp.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://if.huixiangedu.cn

[U106] JS：日期格式化
来源：http://gh.bookmarksfly.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hh.hahajie.cn

[U107] JS：数字千分位
来源：http://my.bookmarksfly.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://od.newstarts.cn

[U108] JS：随机整数
来源：http://dr.yuntaijiaju.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fo.jianghongdianzi.cn

[U109] JS：数组分组
来源：http://qr.hnjuh.cn

Object.groupBy(arr, x => x.type)
来源：http://bc.shxzskj.cn

[U110] JS：数组分块
来源：http://wo.shtwfgs.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gx.nszjky.cn


<!-- 参考信息 -->