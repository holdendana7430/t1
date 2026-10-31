代发 wailian999

[T23] Swift：函数
来源：http://uq.9csxet.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wj.yuntaijiaju.cn

[T24] Swift：闭包
来源：http://ef.huanxung.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://yw.huanxung.cn

[T25] Swift：结构体
来源：http://uj.huanxung.cn

struct P { var x: Int }
来源：http://ga.bjjhwx.cn

[T26] Swift：类与重写
来源：http://aj.bookmarksfly.cn

class A: Base { override func f() {} }
来源：http://lx.haigaiapp.cn

[T27] Swift：错误处理
来源：http://rs.bjjhwx.cn

do { try f() } catch { print(error) }
来源：http://bk.521024.cn

[T28] Swift：枚举
来源：http://mu.yuexingan06.cn

enum Color { case red, green }
来源：http://zo.wgjwhj.cn

[T29] Swift：guard 提前返回
来源：http://ah.bjjhwx.cn

guard let x = opt else { return }
来源：http://vr.jianghongdianzi.cn

[T30] Swift：协议
来源：http://oy.haigaiapp.cn

protocol Shape { func area() -> Double }
来源：http://ly.521024.cn

[T31] Lua：Hello World
来源：http://ht.nicolike.cn

print("Hello")
来源：http://jw.yuexingan06.cn

[T32] Lua：局部变量
来源：http://pt.yuexingan06.cn

local a = 1
来源：http://jj.panjiajie.cn

[T33] Lua：表（数组）
来源：http://xv.9csxet.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://em.huanxung.cn

[T34] Lua：遍历表
来源：http://ga.huixiangedu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://xo.yuntaijiaju.cn

[T35] Lua：字典表
来源：http://lk.wgjwhj.cn

local d = { a = 1 };  d.b = 2
来源：http://iy.huanxung.cn

[T36] Lua：函数
来源：http://wo.lnxyls.cn

function add(a, b) return a + b end
来源：http://ko.huixiangedu.cn

[T37] Lua：字符串拼接
来源：http://wo.shxzukj.cn

"a" .. "b"
来源：http://ft.muxihuayi.cn

[T38] Lua：条件
来源：http://hy.shxzukj.cn

if x > 0 then print("正") end
来源：http://hb.huanxung.cn

[T39] Lua：模式匹配
来源：http://kf.huixinmuqiang.cn

string.find(s, "%d+")
来源：http://ky.shtwfgs.cn

[T40] Lua：元表
来源：http://bf.9csxet.cn

setmetatable({}, { __index = base })
来源：http://si.lnxyls.cn

[T41] Perl：Hello World
来源：http://gw.bjjhwx.cn

print "Hello\n";
来源：http://kb.haigaiapp.cn

[T42] Perl：变量类型
来源：http://ef.szsharing.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dh.newstarts.cn

[T43] Perl：字符串插值
来源：http://fb.521024.cn

"值: $a"
来源：http://il.colortex.cn

[T44] Perl：条件
来源：http://ec.nicolike.cn

if ($a > 0) { print "正"; }
来源：http://tm.panjiajie.cn

[T45] Perl：数组遍历
来源：http://wf.szsharing.cn

for my $x (@arr) { print $x; }
来源：http://es.hahajie.cn

[T46] Perl：哈希操作
来源：http://ua.gzmigu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ak.szsharing.cn

[T47] Perl：正则捕获
来源：http://ia.szsharing.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://lq.panjiajie.cn

[T48] Perl：正则替换
来源：http://nu.wgjwhj.cn

$s =~ s/old/new/g;
来源：http://yv.hahajie.cn

[T49] Perl：函数
来源：http://ug.chemitech.net.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wu.jctech888.com.cn

[T50] Perl：逐行读文件
来源：http://ir.huixiangedu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zs.jctech888.com.cn

while (my $line = <$fh>) { print $line; }
来源：http://na.9csxet.cn

[T51] Scala：Hello World
来源：http://ym.bookmarksfly.cn

println("Hello")
来源：http://sn.jctech888.com.cn

[T52] Scala：变量
来源：http://vs.bookmarksfly.cn

val a = 1;  var b = 2
来源：http://cv.jctech888.com.cn

[T53] Scala：字符串插值
来源：http://dr.bookmarksfly.cn

s"值: $b"
来源：http://aj.gzmigu.cn

[T54] Scala：集合映射
来源：http://sl.shxzskj.cn

List(1, 2, 3).map(_ * 2)
来源：http://ct.szxytkj.cn

[T55] Scala：集合过滤
来源：http://pa.szxytkj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qa.jctech888.com.cn

[T56] Scala：样例类
来源：http://ch.hnjuh.cn

case class User(name: String, age: Int)
来源：http://uv.9csxet.cn

[T57] Scala：模式匹配
来源：http://xv.9csxet.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ak.nszjky.cn

[T58] Scala：函数定义
来源：http://hy.asd995.cn

def add(a: Int, b: Int): Int = a + b
来源：http://um.asd995.cn

[T59] Scala：循环
来源：http://xx.chemitech.net.cn

for (i <- 1 to 10) println(i)
来源：http://jm.bjjhwx.cn

[T60] Scala：折叠
来源：http://yq.521024.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ow.huixinmuqiang.cn

================================================================================
来源：http://oc.hnjuh.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ou.nszjky.cn

================================================================================
来源：http://vh.yuntaijiaju.cn

[U01] Py：创建虚拟环境
来源：http://yc.asd995.cn

python -m venv .venv && source .venv/bin/activate
来源：http://js.huixinmuqiang.cn

[U02] Py：导出 / 安装依赖
来源：http://gj.panjiajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://el.521024.cn

[U03] Py：加载 .env 配置
来源：http://zv.wgjwhj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://nq.huixiangedu.cn

[U04] Py：变量调试打印
来源：http://ec.szxytkj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://su.9csxet.cn

[U05] Py：列表去重且保序
来源：http://ru.szxytkj.cn

list(dict.fromkeys(arr))
来源：http://ch.panjiajie.cn

[U06] Py：合并两个字典
来源：http://ml.haigaiapp.cn

{**a, **b}
来源：http://gc.szsharing.cn

[U07] Py：反转字典键值
来源：http://qe.chemitech.net.cn

{v: k for k, v in d.items()}
来源：http://ae.9csxet.cn

[U08] Py：展平二维列表
来源：http://hy.shtwfgs.cn

[y for x in nested for y in x]
来源：http://xh.lnxyls.cn

[U09] Py：字典取最大值的键
来源：http://ju.huixinmuqiang.cn

max(d, key=d.get)
来源：http://ja.hahajie.cn

[U10] Py：按值排序字典
来源：http://kh.9csxet.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dt.lnxyls.cn

[U11] Py：生成器表达式
来源：http://ka.jianghongdianzi.cn

(x * 2 for x in arr)
来源：http://ml.521024.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rf.colortex.cn

Counter(arr).most_common(3)
来源：http://tp.bookmarksfly.cn

[U13] Py：固定长度队列
来源：http://vt.shxzukj.cn

deque(maxlen=10)
来源：http://zz.lnxyls.cn

[U14] Py：分组收集到列表
来源：http://na.lnxyls.cn

defaultdict(list)
来源：http://qm.panjiajie.cn

[U15] Py：高精度计时
来源：http://ou.shxzukj.cn

t = time.perf_counter()
来源：http://st.hahajie.cn

[U16] Py：命令行参数解析
来源：http://xy.asd995.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xh.bjjhwx.cn

[U17] Py：初始化日志
来源：http://qy.muxihuayi.cn

logging.basicConfig(level=logging.INFO)
来源：http://zf.521024.cn

[U18] Py：预编译正则
来源：http://wv.hahajie.cn

pat = re.compile(r"\d+")
来源：http://ph.521024.cn

[U19] Py：正则替换带回调
来源：http://qw.szxytkj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qc.nszjky.cn

[U20] Py：缓存函数结果
来源：http://hi.yuexingan06.cn

@functools.lru_cache(maxsize=None)
来源：http://sd.shxzukj.cn

[U21] Py：自定义上下文管理器
来源：http://ev.huixiangedu.cn

@contextlib.contextmanager
来源：http://pv.asd995.cn

[U22] Py：矩阵转置
来源：http://cf.jianghongdianzi.cn

list(zip(*m))
来源：http://aj.haigaiapp.cn

[U23] Py：分块读取大文件
来源：http://am.huixinmuqiang.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://oj.huixinmuqiang.cn

[U24] Py：路径操作
来源：http://oy.huanxung.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ne.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://uj.huanxung.cn

csv.DictReader(f)
来源：http://iu.colortex.cn

[U26] Py：并发下载
来源：http://vg.hnjuh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://eg.521024.cn

[U27] Py：异步 HTTP
来源：http://sr.hnjuh.cn

aiohttp.ClientSession() 配合 async with
来源：http://nr.szxytkj.cn

[U28] Py：类型别名
来源：http://fc.chemitech.net.cn

UserId = int
来源：http://ig.bookmarksfly.cn

[U29] Py：属性校验
来源：http://gz.wgjwhj.cn

@property 与 @x.setter 配合
来源：http://hp.nszjky.cn

[U30] Py：数据类
来源：http://uj.gzmigu.cn

@dataclass(slots=True)
来源：http://as.huanxung.cn

[U31] Py：单测
来源：http://lv.shxzskj.cn

python -m pytest -q
来源：http://qh.szsharing.cn

[U32] Py：代码格式化
来源：http://cq.szsharing.cn

ruff format . && ruff check --fix .
来源：http://nb.9csxet.cn

[U33] Py：打包发布
来源：http://ra.nszjky.cn

python -m build  （依赖 pyproject.toml）
来源：http://rx.lnxyls.cn

[U34] Py：判断编码
来源：http://lf.jianghongdianzi.cn

chardet.detect(raw)
来源：http://jw.bookmarksfly.cn

[U35] Py：发送邮件
来源：http://ts.shtwfgs.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ru.shxzukj.cn

[U36] Py：定时任务
来源：http://gr.jianghongdianzi.cn

schedule.every(10).minutes.do(job)
来源：http://qc.bjjhwx.cn

[U37] Py：读写 Excel
来源：http://sv.nszjky.cn

pandas.read_excel / DataFrame.to_excel
来源：http://sv.wgjwhj.cn

[U38] Py：获取脚本所在目录
来源：http://ob.shxzskj.cn

Path(__file__).resolve().parent
来源：http://wt.hnjuh.cn

[U39] Py：判断是否在交互环境
来源：http://iv.lnxyls.cn

sys.stdout.isatty()
来源：http://sm.521024.cn

[U40] Py：打印到标准错误
来源：http://kw.newstarts.cn

print("err", file=sys.stderr)
来源：http://ld.huixiangedu.cn

[U41] PHP：初始化 Composer 项目
来源：http://zs.shxzukj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jx.huixiangedu.cn

[U42] PHP：PSR-4 自动加载
来源：http://wa.bookmarksfly.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qn.colortex.cn

[U43] PHP：声明命名空间
来源：http://xj.newstarts.cn

namespace App\Http;
来源：http://ct.gzmigu.cn

[U44] PHP：开启严格类型
来源：http://zg.chemitech.net.cn

declare(strict_types=1);
来源：http://fy.lnxyls.cn

[U45] PHP：类型声明与返回类型
来源：http://ga.nszjky.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://iu.jianghongdianzi.cn

[U46] PHP：可空类型
来源：http://ze.muxihuayi.cn

?string $name = null
来源：http://wx.lnxyls.cn

[U47] PHP：联合类型
来源：http://pk.nszjky.cn

int|string $id
来源：http://or.haigaiapp.cn

[U48] PHP：纯枚举
来源：http://eh.nicolike.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tl.9csxet.cn

[U49] PHP：只读属性
来源：http://qp.gzmigu.cn

public readonly string $name
来源：http://ya.gzmigu.cn

[U50] PHP：构造器属性提升
来源：http://xs.huixinmuqiang.cn

public function __construct(private int $id) {}
来源：http://bl.jianghongdianzi.cn

[U51] PHP：数组解构
来源：http://xi.nicolike.cn

[$a, $b] = $arr;
来源：http://oi.shxzukj.cn

[U52] PHP：箭头函数
来源：http://sj.newstarts.cn

$double = fn($x) => $x * 2;
来源：http://fn.hahajie.cn

[U53] PHP：空合并运算符
来源：http://en.szsharing.cn

$v = $a ?? $b ?? "default";
来源：http://pv.hahajie.cn

[U54] PHP：空安全调用
来源：http://xu.lnxyls.cn

$obj?->method()
来源：http://qg.bookmarksfly.cn

[U55] PHP：match 表达式
来源：http://sn.bookmarksfly.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://au.haigaiapp.cn

[U56] PHP：命名参数
来源：http://it.shxzskj.cn

f(a: 1, b: 2)
来源：http://fm.huanxung.cn

[U57] PHP：字符串插值
来源：http://gd.huixiangedu.cn

"值: {$a}"
来源：http://gr.yuntaijiaju.cn

[U58] PHP：数组三件套
来源：http://xr.shtwfgs.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kg.huixiangedu.cn

[U59] PHP：自定义排序
来源：http://yx.9csxet.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pq.hnjuh.cn

[U60] PHP：JSON 编解码
来源：http://aw.wgjwhj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://nq.shxzukj.cn

[U61] PHP：正则
来源：http://rk.jianghongdianzi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ax.haigaiapp.cn

[U62] PHP：日期对象
来源：http://pf.lnxyls.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fq.bookmarksfly.cn

[U63] PHP：文件读写
来源：http://me.huixinmuqiang.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://so.szsharing.cn

[U64] PHP：目录遍历
来源：http://rl.szsharing.cn

glob("dir/*.php");  scandir("dir");
来源：http://ka.chemitech.net.cn

[U65] PHP：会话
来源：http://ym.yuexingan06.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://en.bookmarksfly.cn

[U66] PHP：设置 Cookie
来源：http://ww.wgjwhj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jz.shxzukj.cn

[U67] PHP：处理文件上传
来源：http://bi.nszjky.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tc.yuexingan06.cn

[U68] PHP：PDO 连接
来源：http://wv.bookmarksfly.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vb.nicolike.cn

[U69] PHP：PDO 预处理
来源：http://na.bookmarksfly.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xz.asd995.cn

[U70] PHP：PDO 事务
来源：http://wl.shtwfgs.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vt.wgjwhj.cn

[U71] PHP：抛出异常
来源：http://am.shtwfgs.cn

throw new RuntimeException("失败", 500);
来源：http://lv.asd995.cn

[U72] PHP：写错误日志
来源：http://iq.hnjuh.cn

error_log("失败: " . $e->getMessage());
来源：http://qz.huixiangedu.cn

[U73] PHP：读取 ini 配置
来源：http://lp.shxzukj.cn

parse_ini_file("config.ini", true)
来源：http://fz.shxzskj.cn

[U74] PHP：读取环境变量
来源：http://ed.panjiajie.cn

getenv("APP_ENV") ?: "production"
来源：http://vv.bookmarksfly.cn

[U75] PHP：依赖注入
来源：http://bf.asd995.cn

composer require psr/container
来源：http://fw.hnjuh.cn

[U76] PHP：简单路由
来源：http://lq.wgjwhj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gv.gzmigu.cn

[U77] PHP：模板渲染
来源：http://zd.nicolike.cn

composer require twig/twig
来源：http://iq.muxihuayi.cn

[U78] PHP：单元测试
来源：http://cw.jianghongdianzi.cn

composer require --dev phpunit/phpunit
来源：http://vm.wgjwhj.cn

[U79] PHP：静态分析
来源：http://pq.shxzskj.cn

composer require --dev phpstan/phpstan
来源：http://wc.jctech888.com.cn

[U80] PHP：代码规范修复
来源：http://vl.colortex.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://lj.jianghongdianzi.cn

[U81] JS：初始化项目
来源：http://us.9csxet.cn

npm init -y;  npm i express
来源：http://bf.shxzukj.cn

[U82] JS：package.json 脚本
来源：http://kx.colortex.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wz.shxzskj.cn

[U83] JS：ES Module 导入导出
来源：http://xg.haigaiapp.cn

export const a = 1;  import { a } from "./m.js";
来源：http://mu.gzmigu.cn

[U84] JS：CommonJS 写法
来源：http://dy.szsharing.cn

module.exports = { a };  const { a } = require("./m");
来源：http://xz.jctech888.com.cn

[U85] JS：可选链
来源：http://nw.hahajie.cn

a?.b?.c
来源：http://mi.shxzukj.cn

[U86] JS：空值合并
来源：http://ug.bookmarksfly.cn

a ?? b
来源：http://xt.chemitech.net.cn

[U87] JS：解构默认值
来源：http://ev.huixinmuqiang.cn

const { a = 1, b = 2 } = obj;
来源：http://hs.huixinmuqiang.cn

[U88] JS：对象展开合并
来源：http://yp.huanxung.cn

{ ...a, ...b }
来源：http://qw.jianghongdianzi.cn

[U89] JS：数组去重
来源：http://yz.521024.cn

[...new Set(arr)]
来源：http://ne.hnjuh.cn

[U90] JS：数字数组排序
来源：http://gk.9csxet.cn

[...arr].sort((a, b) => a - b)
来源：http://ad.shtwfgs.cn

[U91] JS：对象键值遍历
来源：http://sa.hnjuh.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ox.shxzukj.cn

[U92] JS：深拷贝
来源：http://xt.yuexingan06.cn

structuredClone(obj)
来源：http://vs.shtwfgs.cn

[U93] JS：模板字符串
来源：http://ka.haigaiapp.cn

`共 ${n} 条`
来源：http://jf.shxzukj.cn

[U94] JS：箭头函数
来源：http://sq.hnjuh.cn

const double = x => x * 2;
来源：http://hg.bookmarksfly.cn

[U95] JS：Promise 包装
来源：http://bu.yuntaijiaju.cn

new Promise((resolve, reject) => {})
来源：http://zk.521024.cn

[U96] JS：async/await 与异常
来源：http://hx.gzmigu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cg.bjjhwx.cn

[U97] JS：并发请求
来源：http://ua.gzmigu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://th.hahajie.cn

[U98] JS：fetch 带 JSON
来源：http://vq.newstarts.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tt.hahajie.cn

[U99] JS：事件监听
来源：http://ae.9csxet.cn

el.addEventListener("click", e => {})
来源：http://za.newstarts.cn

[U100] JS：DOM 查询
来源：http://nt.muxihuayi.cn

document.querySelector(".item")
来源：http://zg.hnjuh.cn

[U101] JS：classList 操作
来源：http://uv.shxzskj.cn

el.classList.toggle("active")
来源：http://aj.haigaiapp.cn

[U102] JS：本地存储
来源：http://fw.huixiangedu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://cl.haigaiapp.cn

[U103] JS：定时器
来源：http://mh.nicolike.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xo.haigaiapp.cn

[U104] JS：防抖
来源：http://ee.szxytkj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://py.nicolike.cn

[U105] JS：节流
来源：http://jk.asd995.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jl.szsharing.cn

[U106] JS：日期格式化
来源：http://qu.bookmarksfly.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yc.nicolike.cn

[U107] JS：数字千分位
来源：http://my.hnjuh.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bq.9csxet.cn

[U108] JS：随机整数
来源：http://xy.hnjuh.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rd.hnjuh.cn

[U109] JS：数组分组
来源：http://ov.521024.cn

Object.groupBy(arr, x => x.type)
来源：http://gt.wgjwhj.cn

[U110] JS：数组分块
来源：http://xb.huixinmuqiang.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pg.nszjky.cn


<!-- 参考信息 -->