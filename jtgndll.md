代发 wailian999

[T25] Swift：结构体
来源：http://gr.hnjuh.cn

struct P { var x: Int }
来源：http://hq.9csxet.cn

[T26] Swift：类与重写
来源：http://gf.jianghongdianzi.cn

class A: Base { override func f() {} }
来源：http://uv.lnxyls.cn

[T27] Swift：错误处理
来源：http://js.shxzukj.cn

do { try f() } catch { print(error) }
来源：http://dt.szxytkj.cn

[T28] Swift：枚举
来源：http://hz.asd995.cn

enum Color { case red, green }
来源：http://wn.hahajie.cn

[T29] Swift：guard 提前返回
来源：http://hg.shxzskj.cn

guard let x = opt else { return }
来源：http://hb.yuexingan06.cn

[T30] Swift：协议
来源：http://vm.nszjky.cn

protocol Shape { func area() -> Double }
来源：http://ob.jctech888.com.cn

[T31] Lua：Hello World
来源：http://rq.huixiangedu.cn

print("Hello")
来源：http://ew.huanxung.cn

[T32] Lua：局部变量
来源：http://gb.9csxet.cn

local a = 1
来源：http://qa.bookmarksfly.cn

[T33] Lua：表（数组）
来源：http://if.hnjuh.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hy.shtwfgs.cn

[T34] Lua：遍历表
来源：http://wo.huixinmuqiang.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://cu.lnxyls.cn

[T35] Lua：字典表
来源：http://ut.huanxung.cn

local d = { a = 1 };  d.b = 2
来源：http://he.wgjwhj.cn

[T36] Lua：函数
来源：http://sx.huixinmuqiang.cn

function add(a, b) return a + b end
来源：http://ls.chemitech.net.cn

[T37] Lua：字符串拼接
来源：http://jg.jctech888.com.cn

"a" .. "b"
来源：http://hf.panjiajie.cn

[T38] Lua：条件
来源：http://kw.chemitech.net.cn

if x > 0 then print("正") end
来源：http://ep.hnjuh.cn

[T39] Lua：模式匹配
来源：http://zu.jctech888.com.cn

string.find(s, "%d+")
来源：http://fh.newstarts.cn

[T40] Lua：元表
来源：http://uc.panjiajie.cn

setmetatable({}, { __index = base })
来源：http://zk.jianghongdianzi.cn

[T41] Perl：Hello World
来源：http://ks.huanxung.cn

print "Hello\n";
来源：http://im.gzmigu.cn

[T42] Perl：变量类型
来源：http://cp.521024.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yt.chemitech.net.cn

[T43] Perl：字符串插值
来源：http://tv.colortex.cn

"值: $a"
来源：http://re.huixinmuqiang.cn

[T44] Perl：条件
来源：http://wr.nicolike.cn

if ($a > 0) { print "正"; }
来源：http://jn.chemitech.net.cn

[T45] Perl：数组遍历
来源：http://ke.nicolike.cn

for my $x (@arr) { print $x; }
来源：http://qe.huixinmuqiang.cn

[T46] Perl：哈希操作
来源：http://on.hnjuh.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://es.newstarts.cn

[T47] Perl：正则捕获
来源：http://ml.colortex.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://da.panjiajie.cn

[T48] Perl：正则替换
来源：http://jw.shxzskj.cn

$s =~ s/old/new/g;
来源：http://sc.huanxung.cn

[T49] Perl：函数
来源：http://wq.panjiajie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://az.hahajie.cn

[T50] Perl：逐行读文件
来源：http://bc.haigaiapp.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wr.gzmigu.cn

while (my $line = <$fh>) { print $line; }
来源：http://jn.nszjky.cn

[T51] Scala：Hello World
来源：http://ek.newstarts.cn

println("Hello")
来源：http://ph.nszjky.cn

[T52] Scala：变量
来源：http://ju.hahajie.cn

val a = 1;  var b = 2
来源：http://cu.nicolike.cn

[T53] Scala：字符串插值
来源：http://tj.shtwfgs.cn

s"值: $b"
来源：http://qy.panjiajie.cn

[T54] Scala：集合映射
来源：http://ol.haigaiapp.cn

List(1, 2, 3).map(_ * 2)
来源：http://ff.huanxung.cn

[T55] Scala：集合过滤
来源：http://hf.panjiajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://jc.jianghongdianzi.cn

[T56] Scala：样例类
来源：http://fj.haigaiapp.cn

case class User(name: String, age: Int)
来源：http://nd.jianghongdianzi.cn

[T57] Scala：模式匹配
来源：http://ve.521024.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://bo.wgjwhj.cn

[T58] Scala：函数定义
来源：http://zp.jianghongdianzi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://um.yuexingan06.cn

[T59] Scala：循环
来源：http://bm.bookmarksfly.cn

for (i <- 1 to 10) println(i)
来源：http://xo.hahajie.cn

[T60] Scala：折叠
来源：http://hv.szsharing.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fl.huixinmuqiang.cn

================================================================================
来源：http://ds.huanxung.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wb.chemitech.net.cn

================================================================================
来源：http://lq.huixinmuqiang.cn

[U01] Py：创建虚拟环境
来源：http://rw.lnxyls.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ut.wgjwhj.cn

[U02] Py：导出 / 安装依赖
来源：http://mf.haigaiapp.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rx.huixiangedu.cn

[U03] Py：加载 .env 配置
来源：http://pp.colortex.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://pz.huixinmuqiang.cn

[U04] Py：变量调试打印
来源：http://we.521024.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tu.bookmarksfly.cn

[U05] Py：列表去重且保序
来源：http://mo.nszjky.cn

list(dict.fromkeys(arr))
来源：http://ga.hnjuh.cn

[U06] Py：合并两个字典
来源：http://ae.gzmigu.cn

{**a, **b}
来源：http://ub.asd995.cn

[U07] Py：反转字典键值
来源：http://dr.huixinmuqiang.cn

{v: k for k, v in d.items()}
来源：http://xg.haigaiapp.cn

[U08] Py：展平二维列表
来源：http://dc.521024.cn

[y for x in nested for y in x]
来源：http://yy.hnjuh.cn

[U09] Py：字典取最大值的键
来源：http://sb.huanxung.cn

max(d, key=d.get)
来源：http://kp.chemitech.net.cn

[U10] Py：按值排序字典
来源：http://ps.panjiajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fb.chemitech.net.cn

[U11] Py：生成器表达式
来源：http://of.colortex.cn

(x * 2 for x in arr)
来源：http://jf.huanxung.cn

[U12] Py：取出现最多的 3 个元素
来源：http://tu.haigaiapp.cn

Counter(arr).most_common(3)
来源：http://cq.haigaiapp.cn

[U13] Py：固定长度队列
来源：http://ro.shtwfgs.cn

deque(maxlen=10)
来源：http://zh.colortex.cn

[U14] Py：分组收集到列表
来源：http://sv.shtwfgs.cn

defaultdict(list)
来源：http://gm.nicolike.cn

[U15] Py：高精度计时
来源：http://tp.chemitech.net.cn

t = time.perf_counter()
来源：http://wm.huixinmuqiang.cn

[U16] Py：命令行参数解析
来源：http://pu.lnxyls.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wj.huixiangedu.cn

[U17] Py：初始化日志
来源：http://av.9csxet.cn

logging.basicConfig(level=logging.INFO)
来源：http://zo.521024.cn

[U18] Py：预编译正则
来源：http://cm.gzmigu.cn

pat = re.compile(r"\d+")
来源：http://ue.huixinmuqiang.cn

[U19] Py：正则替换带回调
来源：http://sz.panjiajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yn.shxzukj.cn

[U20] Py：缓存函数结果
来源：http://ox.shxzukj.cn

@functools.lru_cache(maxsize=None)
来源：http://mz.bookmarksfly.cn

[U21] Py：自定义上下文管理器
来源：http://tg.yuntaijiaju.cn

@contextlib.contextmanager
来源：http://fa.szsharing.cn

[U22] Py：矩阵转置
来源：http://rp.chemitech.net.cn

list(zip(*m))
来源：http://xd.szsharing.cn

[U23] Py：分块读取大文件
来源：http://ha.nicolike.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://oh.jianghongdianzi.cn

[U24] Py：路径操作
来源：http://xi.newstarts.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cu.szsharing.cn

[U25] Py：CSV 按字典读
来源：http://ut.szsharing.cn

csv.DictReader(f)
来源：http://gu.wgjwhj.cn

[U26] Py：并发下载
来源：http://or.colortex.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yn.huanxung.cn

[U27] Py：异步 HTTP
来源：http://dw.asd995.cn

aiohttp.ClientSession() 配合 async with
来源：http://js.9csxet.cn

[U28] Py：类型别名
来源：http://mo.huanxung.cn

UserId = int
来源：http://kh.9csxet.cn

[U29] Py：属性校验
来源：http://dv.asd995.cn

@property 与 @x.setter 配合
来源：http://fa.chemitech.net.cn

[U30] Py：数据类
来源：http://ng.nszjky.cn

@dataclass(slots=True)
来源：http://qt.hahajie.cn

[U31] Py：单测
来源：http://up.lnxyls.cn

python -m pytest -q
来源：http://ua.9csxet.cn

[U32] Py：代码格式化
来源：http://zx.huanxung.cn

ruff format . && ruff check --fix .
来源：http://xa.nicolike.cn

[U33] Py：打包发布
来源：http://cf.wgjwhj.cn

python -m build  （依赖 pyproject.toml）
来源：http://ch.yuexingan06.cn

[U34] Py：判断编码
来源：http://sv.shxzskj.cn

chardet.detect(raw)
来源：http://vo.yuexingan06.cn

[U35] Py：发送邮件
来源：http://gz.nszjky.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ar.bookmarksfly.cn

[U36] Py：定时任务
来源：http://ez.9csxet.cn

schedule.every(10).minutes.do(job)
来源：http://bi.hahajie.cn

[U37] Py：读写 Excel
来源：http://tl.hahajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://fp.yuntaijiaju.cn

[U38] Py：获取脚本所在目录
来源：http://ue.lnxyls.cn

Path(__file__).resolve().parent
来源：http://tu.jianghongdianzi.cn

[U39] Py：判断是否在交互环境
来源：http://cj.521024.cn

sys.stdout.isatty()
来源：http://ih.521024.cn

[U40] Py：打印到标准错误
来源：http://ki.bookmarksfly.cn

print("err", file=sys.stderr)
来源：http://tu.szsharing.cn

[U41] PHP：初始化 Composer 项目
来源：http://qj.lnxyls.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zc.huixinmuqiang.cn

[U42] PHP：PSR-4 自动加载
来源：http://od.hahajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pn.yuntaijiaju.cn

[U43] PHP：声明命名空间
来源：http://uy.haigaiapp.cn

namespace App\Http;
来源：http://qw.bookmarksfly.cn

[U44] PHP：开启严格类型
来源：http://rs.newstarts.cn

declare(strict_types=1);
来源：http://js.szxytkj.cn

[U45] PHP：类型声明与返回类型
来源：http://pp.wgjwhj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://mq.hnjuh.cn

[U46] PHP：可空类型
来源：http://wi.9csxet.cn

?string $name = null
来源：http://yr.hahajie.cn

[U47] PHP：联合类型
来源：http://rn.shxzukj.cn

int|string $id
来源：http://up.hahajie.cn

[U48] PHP：纯枚举
来源：http://cj.colortex.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dz.yuexingan06.cn

[U49] PHP：只读属性
来源：http://gl.szxytkj.cn

public readonly string $name
来源：http://ta.colortex.cn

[U50] PHP：构造器属性提升
来源：http://rd.panjiajie.cn

public function __construct(private int $id) {}
来源：http://as.nszjky.cn

[U51] PHP：数组解构
来源：http://yy.yuexingan06.cn

[$a, $b] = $arr;
来源：http://hr.huixinmuqiang.cn

[U52] PHP：箭头函数
来源：http://kd.bjjhwx.cn

$double = fn($x) => $x * 2;
来源：http://pm.szxytkj.cn

[U53] PHP：空合并运算符
来源：http://fj.hnjuh.cn

$v = $a ?? $b ?? "default";
来源：http://nj.shxzskj.cn

[U54] PHP：空安全调用
来源：http://of.hahajie.cn

$obj?->method()
来源：http://sb.bjjhwx.cn

[U55] PHP：match 表达式
来源：http://zh.wgjwhj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cj.bjjhwx.cn

[U56] PHP：命名参数
来源：http://eh.gzmigu.cn

f(a: 1, b: 2)
来源：http://kp.hahajie.cn

[U57] PHP：字符串插值
来源：http://iq.szsharing.cn

"值: {$a}"
来源：http://ro.jianghongdianzi.cn

[U58] PHP：数组三件套
来源：http://mu.shxzskj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vk.nicolike.cn

[U59] PHP：自定义排序
来源：http://qy.shtwfgs.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mx.newstarts.cn

[U60] PHP：JSON 编解码
来源：http://be.chemitech.net.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cw.bookmarksfly.cn

[U61] PHP：正则
来源：http://yb.bookmarksfly.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xl.huixiangedu.cn

[U62] PHP：日期对象
来源：http://iv.colortex.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bi.lnxyls.cn

[U63] PHP：文件读写
来源：http://tc.jianghongdianzi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gd.521024.cn

[U64] PHP：目录遍历
来源：http://rn.muxihuayi.cn

glob("dir/*.php");  scandir("dir");
来源：http://oy.muxihuayi.cn

[U65] PHP：会话
来源：http://ez.hnjuh.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rk.9csxet.cn

[U66] PHP：设置 Cookie
来源：http://wn.szsharing.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://be.yuexingan06.cn

[U67] PHP：处理文件上传
来源：http://ce.wgjwhj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nt.yuntaijiaju.cn

[U68] PHP：PDO 连接
来源：http://es.yuntaijiaju.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ky.szsharing.cn

[U69] PHP：PDO 预处理
来源：http://lx.newstarts.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fr.colortex.cn

[U70] PHP：PDO 事务
来源：http://hg.yuntaijiaju.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ej.shxzskj.cn

[U71] PHP：抛出异常
来源：http://ab.yuntaijiaju.cn

throw new RuntimeException("失败", 500);
来源：http://dt.jctech888.com.cn

[U72] PHP：写错误日志
来源：http://fg.newstarts.cn

error_log("失败: " . $e->getMessage());
来源：http://db.szxytkj.cn

[U73] PHP：读取 ini 配置
来源：http://qs.yuexingan06.cn

parse_ini_file("config.ini", true)
来源：http://kk.huixinmuqiang.cn

[U74] PHP：读取环境变量
来源：http://wt.shxzukj.cn

getenv("APP_ENV") ?: "production"
来源：http://ok.lnxyls.cn

[U75] PHP：依赖注入
来源：http://pi.jianghongdianzi.cn

composer require psr/container
来源：http://pq.nicolike.cn

[U76] PHP：简单路由
来源：http://lv.chemitech.net.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pf.panjiajie.cn

[U77] PHP：模板渲染
来源：http://pd.newstarts.cn

composer require twig/twig
来源：http://sk.chemitech.net.cn

[U78] PHP：单元测试
来源：http://zn.yuntaijiaju.cn

composer require --dev phpunit/phpunit
来源：http://zj.yuntaijiaju.cn

[U79] PHP：静态分析
来源：http://dz.nicolike.cn

composer require --dev phpstan/phpstan
来源：http://lx.yuntaijiaju.cn

[U80] PHP：代码规范修复
来源：http://rk.szxytkj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://hu.nszjky.cn

[U81] JS：初始化项目
来源：http://zu.521024.cn

npm init -y;  npm i express
来源：http://gf.newstarts.cn

[U82] JS：package.json 脚本
来源：http://ik.huanxung.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fm.jianghongdianzi.cn

[U83] JS：ES Module 导入导出
来源：http://uo.hahajie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vk.yuexingan06.cn

[U84] JS：CommonJS 写法
来源：http://vz.haigaiapp.cn

module.exports = { a };  const { a } = require("./m");
来源：http://cc.shxzskj.cn

[U85] JS：可选链
来源：http://qs.yuexingan06.cn

a?.b?.c
来源：http://cq.huixiangedu.cn

[U86] JS：空值合并
来源：http://xs.haigaiapp.cn

a ?? b
来源：http://rb.huixinmuqiang.cn

[U87] JS：解构默认值
来源：http://xr.hahajie.cn

const { a = 1, b = 2 } = obj;
来源：http://jy.asd995.cn

[U88] JS：对象展开合并
来源：http://gv.jianghongdianzi.cn

{ ...a, ...b }
来源：http://yp.chemitech.net.cn

[U89] JS：数组去重
来源：http://fp.yuexingan06.cn

[...new Set(arr)]
来源：http://fe.lnxyls.cn

[U90] JS：数字数组排序
来源：http://ej.huixinmuqiang.cn

[...arr].sort((a, b) => a - b)
来源：http://nc.yuntaijiaju.cn

[U91] JS：对象键值遍历
来源：http://mw.lnxyls.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ql.szxytkj.cn

[U92] JS：深拷贝
来源：http://nu.szxytkj.cn

structuredClone(obj)
来源：http://un.huixinmuqiang.cn

[U93] JS：模板字符串
来源：http://xx.haigaiapp.cn

`共 ${n} 条`
来源：http://bb.jianghongdianzi.cn

[U94] JS：箭头函数
来源：http://cd.nicolike.cn

const double = x => x * 2;
来源：http://wi.asd995.cn

[U95] JS：Promise 包装
来源：http://gr.521024.cn

new Promise((resolve, reject) => {})
来源：http://ma.asd995.cn

[U96] JS：async/await 与异常
来源：http://zv.bjjhwx.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wr.szsharing.cn

[U97] JS：并发请求
来源：http://av.asd995.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ht.szsharing.cn

[U98] JS：fetch 带 JSON
来源：http://uf.huixiangedu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lw.hnjuh.cn

[U99] JS：事件监听
来源：http://bf.nicolike.cn

el.addEventListener("click", e => {})
来源：http://hc.huixinmuqiang.cn

[U100] JS：DOM 查询
来源：http://jf.hahajie.cn

document.querySelector(".item")
来源：http://gf.chemitech.net.cn

[U101] JS：classList 操作
来源：http://ci.yuntaijiaju.cn

el.classList.toggle("active")
来源：http://wx.nicolike.cn

[U102] JS：本地存储
来源：http://iv.hahajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://fc.wgjwhj.cn

[U103] JS：定时器
来源：http://yy.yuexingan06.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zo.huixiangedu.cn

[U104] JS：防抖
来源：http://wi.colortex.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zh.lnxyls.cn

[U105] JS：节流
来源：http://tq.huixinmuqiang.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://oe.colortex.cn

[U106] JS：日期格式化
来源：http://bf.huixinmuqiang.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ft.shtwfgs.cn

[U107] JS：数字千分位
来源：http://bi.huixinmuqiang.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://la.bookmarksfly.cn

[U108] JS：随机整数
来源：http://en.chemitech.net.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bt.bjjhwx.cn

[U109] JS：数组分组
来源：http://fs.yuexingan06.cn

Object.groupBy(arr, x => x.type)
来源：http://ia.hnjuh.cn

[U110] JS：数组分块
来源：http://ap.9csxet.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://en.jctech888.com.cn

[U111] JS：对象转 Map
来源：http://uc.colortex.cn

new Map(Object.entries(obj))
来源：http://pq.shxzukj.cn

[U112] JS：字符串补位
来源：http://ib.szxytkj.cn

"7".padStart(3, "0")
来源：http://zf.shxzskj.cn


<!-- 参考信息 -->