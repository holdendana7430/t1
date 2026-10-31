代发 wailian999

[T25] Swift：结构体
来源：http://vt.szxytkj.cn

struct P { var x: Int }
来源：http://jn.nicolike.cn

[T26] Swift：类与重写
来源：http://ny.huanxung.cn

class A: Base { override func f() {} }
来源：http://pc.9csxet.cn

[T27] Swift：错误处理
来源：http://jm.wgjwhj.cn

do { try f() } catch { print(error) }
来源：http://jo.newstarts.cn

[T28] Swift：枚举
来源：http://ir.szxytkj.cn

enum Color { case red, green }
来源：http://bk.haigaiapp.cn

[T29] Swift：guard 提前返回
来源：http://lf.yuntaijiaju.cn

guard let x = opt else { return }
来源：http://zs.hnjuh.cn

[T30] Swift：协议
来源：http://ra.nszjky.cn

protocol Shape { func area() -> Double }
来源：http://wk.szxytkj.cn

[T31] Lua：Hello World
来源：http://ny.chemitech.net.cn

print("Hello")
来源：http://hi.newstarts.cn

[T32] Lua：局部变量
来源：http://on.yuntaijiaju.cn

local a = 1
来源：http://ix.hnjuh.cn

[T33] Lua：表（数组）
来源：http://ym.wgjwhj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://od.nicolike.cn

[T34] Lua：遍历表
来源：http://yp.nicolike.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://lq.jctech888.com.cn

[T35] Lua：字典表
来源：http://vq.shxzukj.cn

local d = { a = 1 };  d.b = 2
来源：http://bb.asd995.cn

[T36] Lua：函数
来源：http://vo.huixinmuqiang.cn

function add(a, b) return a + b end
来源：http://ri.yuexingan06.cn

[T37] Lua：字符串拼接
来源：http://iq.yuexingan06.cn

"a" .. "b"
来源：http://uh.muxihuayi.cn

[T38] Lua：条件
来源：http://hz.huanxung.cn

if x > 0 then print("正") end
来源：http://pn.szsharing.cn

[T39] Lua：模式匹配
来源：http://kc.lnxyls.cn

string.find(s, "%d+")
来源：http://su.shtwfgs.cn

[T40] Lua：元表
来源：http://re.haigaiapp.cn

setmetatable({}, { __index = base })
来源：http://ep.jctech888.com.cn

[T41] Perl：Hello World
来源：http://ji.jctech888.com.cn

print "Hello\n";
来源：http://nz.nicolike.cn

[T42] Perl：变量类型
来源：http://dy.szxytkj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ja.haigaiapp.cn

[T43] Perl：字符串插值
来源：http://mg.shxzukj.cn

"值: $a"
来源：http://rz.nszjky.cn

[T44] Perl：条件
来源：http://gb.muxihuayi.cn

if ($a > 0) { print "正"; }
来源：http://nd.haigaiapp.cn

[T45] Perl：数组遍历
来源：http://qe.hnjuh.cn

for my $x (@arr) { print $x; }
来源：http://tz.newstarts.cn

[T46] Perl：哈希操作
来源：http://vi.521024.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vx.nszjky.cn

[T47] Perl：正则捕获
来源：http://lq.nicolike.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dh.colortex.cn

[T48] Perl：正则替换
来源：http://vx.bjjhwx.cn

$s =~ s/old/new/g;
来源：http://yz.jianghongdianzi.cn

[T49] Perl：函数
来源：http://ls.yuexingan06.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ap.hnjuh.cn

[T50] Perl：逐行读文件
来源：http://fg.wgjwhj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fv.huixinmuqiang.cn

while (my $line = <$fh>) { print $line; }
来源：http://vh.szsharing.cn

[T51] Scala：Hello World
来源：http://rx.bookmarksfly.cn

println("Hello")
来源：http://bb.shxzskj.cn

[T52] Scala：变量
来源：http://ew.gzmigu.cn

val a = 1;  var b = 2
来源：http://gv.huanxung.cn

[T53] Scala：字符串插值
来源：http://dk.yuexingan06.cn

s"值: $b"
来源：http://ba.yuexingan06.cn

[T54] Scala：集合映射
来源：http://tc.szxytkj.cn

List(1, 2, 3).map(_ * 2)
来源：http://kh.nicolike.cn

[T55] Scala：集合过滤
来源：http://xm.muxihuayi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://px.hnjuh.cn

[T56] Scala：样例类
来源：http://xi.chemitech.net.cn

case class User(name: String, age: Int)
来源：http://ac.yuexingan06.cn

[T57] Scala：模式匹配
来源：http://ym.hahajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ca.gzmigu.cn

[T58] Scala：函数定义
来源：http://yd.panjiajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wn.nicolike.cn

[T59] Scala：循环
来源：http://qg.lnxyls.cn

for (i <- 1 to 10) println(i)
来源：http://tt.521024.cn

[T60] Scala：折叠
来源：http://wa.huixiangedu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vc.szxytkj.cn

================================================================================
来源：http://fo.huixiangedu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xq.szsharing.cn

================================================================================
来源：http://zj.yuntaijiaju.cn

[U01] Py：创建虚拟环境
来源：http://ui.panjiajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://fx.huanxung.cn

[U02] Py：导出 / 安装依赖
来源：http://hm.haigaiapp.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mo.asd995.cn

[U03] Py：加载 .env 配置
来源：http://mu.colortex.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ra.huixiangedu.cn

[U04] Py：变量调试打印
来源：http://uk.521024.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dj.wgjwhj.cn

[U05] Py：列表去重且保序
来源：http://dg.jctech888.com.cn

list(dict.fromkeys(arr))
来源：http://dm.jctech888.com.cn

[U06] Py：合并两个字典
来源：http://xe.jianghongdianzi.cn

{**a, **b}
来源：http://qc.shxzukj.cn

[U07] Py：反转字典键值
来源：http://no.nicolike.cn

{v: k for k, v in d.items()}
来源：http://xg.haigaiapp.cn

[U08] Py：展平二维列表
来源：http://ss.lnxyls.cn

[y for x in nested for y in x]
来源：http://eb.szxytkj.cn

[U09] Py：字典取最大值的键
来源：http://yw.shxzskj.cn

max(d, key=d.get)
来源：http://pn.wgjwhj.cn

[U10] Py：按值排序字典
来源：http://fw.yuntaijiaju.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cr.shtwfgs.cn

[U11] Py：生成器表达式
来源：http://fw.gzmigu.cn

(x * 2 for x in arr)
来源：http://ut.hnjuh.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zd.shxzukj.cn

Counter(arr).most_common(3)
来源：http://nq.szsharing.cn

[U13] Py：固定长度队列
来源：http://xl.panjiajie.cn

deque(maxlen=10)
来源：http://ch.lnxyls.cn

[U14] Py：分组收集到列表
来源：http://oo.shxzskj.cn

defaultdict(list)
来源：http://wb.huixinmuqiang.cn

[U15] Py：高精度计时
来源：http://ht.521024.cn

t = time.perf_counter()
来源：http://fg.hnjuh.cn

[U16] Py：命令行参数解析
来源：http://xs.huanxung.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yq.bookmarksfly.cn

[U17] Py：初始化日志
来源：http://mu.shxzukj.cn

logging.basicConfig(level=logging.INFO)
来源：http://yh.9csxet.cn

[U18] Py：预编译正则
来源：http://oc.hahajie.cn

pat = re.compile(r"\d+")
来源：http://zy.chemitech.net.cn

[U19] Py：正则替换带回调
来源：http://ec.huixiangedu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ew.newstarts.cn

[U20] Py：缓存函数结果
来源：http://bx.huanxung.cn

@functools.lru_cache(maxsize=None)
来源：http://ni.shtwfgs.cn

[U21] Py：自定义上下文管理器
来源：http://og.521024.cn

@contextlib.contextmanager
来源：http://vt.gzmigu.cn

[U22] Py：矩阵转置
来源：http://js.newstarts.cn

list(zip(*m))
来源：http://wk.bjjhwx.cn

[U23] Py：分块读取大文件
来源：http://hj.jianghongdianzi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ub.yuexingan06.cn

[U24] Py：路径操作
来源：http://dm.nszjky.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://id.yuntaijiaju.cn

[U25] Py：CSV 按字典读
来源：http://gb.szxytkj.cn

csv.DictReader(f)
来源：http://zl.shtwfgs.cn

[U26] Py：并发下载
来源：http://pb.gzmigu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ax.haigaiapp.cn

[U27] Py：异步 HTTP
来源：http://wz.shxzskj.cn

aiohttp.ClientSession() 配合 async with
来源：http://ml.szxytkj.cn

[U28] Py：类型别名
来源：http://da.hnjuh.cn

UserId = int
来源：http://ps.521024.cn

[U29] Py：属性校验
来源：http://jg.haigaiapp.cn

@property 与 @x.setter 配合
来源：http://wr.jianghongdianzi.cn

[U30] Py：数据类
来源：http://rt.asd995.cn

@dataclass(slots=True)
来源：http://oi.lnxyls.cn

[U31] Py：单测
来源：http://vw.nszjky.cn

python -m pytest -q
来源：http://ld.szsharing.cn

[U32] Py：代码格式化
来源：http://vk.szxytkj.cn

ruff format . && ruff check --fix .
来源：http://et.shxzukj.cn

[U33] Py：打包发布
来源：http://jr.bjjhwx.cn

python -m build  （依赖 pyproject.toml）
来源：http://fx.shxzukj.cn

[U34] Py：判断编码
来源：http://xf.jctech888.com.cn

chardet.detect(raw)
来源：http://op.huixiangedu.cn

[U35] Py：发送邮件
来源：http://jj.wgjwhj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bi.colortex.cn

[U36] Py：定时任务
来源：http://rb.nicolike.cn

schedule.every(10).minutes.do(job)
来源：http://pc.huanxung.cn

[U37] Py：读写 Excel
来源：http://qv.szxytkj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://mu.szxytkj.cn

[U38] Py：获取脚本所在目录
来源：http://mt.shxzskj.cn

Path(__file__).resolve().parent
来源：http://sj.huixinmuqiang.cn

[U39] Py：判断是否在交互环境
来源：http://lf.9csxet.cn

sys.stdout.isatty()
来源：http://xx.shxzskj.cn

[U40] Py：打印到标准错误
来源：http://tv.hahajie.cn

print("err", file=sys.stderr)
来源：http://sx.bookmarksfly.cn

[U41] PHP：初始化 Composer 项目
来源：http://xu.shxzukj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ss.shtwfgs.cn

[U42] PHP：PSR-4 自动加载
来源：http://lk.haigaiapp.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sm.lnxyls.cn

[U43] PHP：声明命名空间
来源：http://jp.newstarts.cn

namespace App\Http;
来源：http://lc.chemitech.net.cn

[U44] PHP：开启严格类型
来源：http://ko.yuexingan06.cn

declare(strict_types=1);
来源：http://vi.huixiangedu.cn

[U45] PHP：类型声明与返回类型
来源：http://pj.jianghongdianzi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qj.yuntaijiaju.cn

[U46] PHP：可空类型
来源：http://td.haigaiapp.cn

?string $name = null
来源：http://af.huixinmuqiang.cn

[U47] PHP：联合类型
来源：http://to.yuntaijiaju.cn

int|string $id
来源：http://ko.gzmigu.cn

[U48] PHP：纯枚举
来源：http://jr.yuexingan06.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vj.hahajie.cn

[U49] PHP：只读属性
来源：http://xw.newstarts.cn

public readonly string $name
来源：http://so.chemitech.net.cn

[U50] PHP：构造器属性提升
来源：http://cx.szxytkj.cn

public function __construct(private int $id) {}
来源：http://ky.521024.cn

[U51] PHP：数组解构
来源：http://ma.huixinmuqiang.cn

[$a, $b] = $arr;
来源：http://qd.huixinmuqiang.cn

[U52] PHP：箭头函数
来源：http://nz.panjiajie.cn

$double = fn($x) => $x * 2;
来源：http://ko.shxzskj.cn

[U53] PHP：空合并运算符
来源：http://or.muxihuayi.cn

$v = $a ?? $b ?? "default";
来源：http://nb.bookmarksfly.cn

[U54] PHP：空安全调用
来源：http://vk.9csxet.cn

$obj?->method()
来源：http://ln.huixinmuqiang.cn

[U55] PHP：match 表达式
来源：http://cn.asd995.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hl.521024.cn

[U56] PHP：命名参数
来源：http://eo.chemitech.net.cn

f(a: 1, b: 2)
来源：http://io.newstarts.cn

[U57] PHP：字符串插值
来源：http://wl.gzmigu.cn

"值: {$a}"
来源：http://hp.huixinmuqiang.cn

[U58] PHP：数组三件套
来源：http://pe.panjiajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lq.wgjwhj.cn

[U59] PHP：自定义排序
来源：http://gb.lnxyls.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ht.lnxyls.cn

[U60] PHP：JSON 编解码
来源：http://hp.chemitech.net.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fs.hahajie.cn

[U61] PHP：正则
来源：http://vf.chemitech.net.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kd.chemitech.net.cn

[U62] PHP：日期对象
来源：http://oa.521024.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://id.shtwfgs.cn

[U63] PHP：文件读写
来源：http://wf.newstarts.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bm.521024.cn

[U64] PHP：目录遍历
来源：http://sg.yuntaijiaju.cn

glob("dir/*.php");  scandir("dir");
来源：http://if.wgjwhj.cn

[U65] PHP：会话
来源：http://mq.chemitech.net.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ko.jianghongdianzi.cn

[U66] PHP：设置 Cookie
来源：http://wi.hahajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wv.haigaiapp.cn

[U67] PHP：处理文件上传
来源：http://ls.hahajie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xv.yuntaijiaju.cn

[U68] PHP：PDO 连接
来源：http://ey.bjjhwx.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lp.shxzukj.cn

[U69] PHP：PDO 预处理
来源：http://jv.jianghongdianzi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vl.muxihuayi.cn

[U70] PHP：PDO 事务
来源：http://su.hahajie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dc.yuexingan06.cn

[U71] PHP：抛出异常
来源：http://iq.shtwfgs.cn

throw new RuntimeException("失败", 500);
来源：http://id.yuntaijiaju.cn

[U72] PHP：写错误日志
来源：http://ta.szxytkj.cn

error_log("失败: " . $e->getMessage());
来源：http://eo.lnxyls.cn

[U73] PHP：读取 ini 配置
来源：http://fg.bjjhwx.cn

parse_ini_file("config.ini", true)
来源：http://pl.newstarts.cn

[U74] PHP：读取环境变量
来源：http://zs.newstarts.cn

getenv("APP_ENV") ?: "production"
来源：http://qo.muxihuayi.cn

[U75] PHP：依赖注入
来源：http://ac.panjiajie.cn

composer require psr/container
来源：http://cp.szxytkj.cn

[U76] PHP：简单路由
来源：http://pw.chemitech.net.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wi.nicolike.cn

[U77] PHP：模板渲染
来源：http://rd.huanxung.cn

composer require twig/twig
来源：http://qe.521024.cn

[U78] PHP：单元测试
来源：http://pi.nszjky.cn

composer require --dev phpunit/phpunit
来源：http://zf.521024.cn

[U79] PHP：静态分析
来源：http://bz.shxzskj.cn

composer require --dev phpstan/phpstan
来源：http://rx.gzmigu.cn

[U80] PHP：代码规范修复
来源：http://dh.newstarts.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ey.bookmarksfly.cn

[U81] JS：初始化项目
来源：http://bj.haigaiapp.cn

npm init -y;  npm i express
来源：http://lg.haigaiapp.cn

[U82] JS：package.json 脚本
来源：http://lv.521024.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://uo.hnjuh.cn

[U83] JS：ES Module 导入导出
来源：http://zv.9csxet.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zi.bookmarksfly.cn

[U84] JS：CommonJS 写法
来源：http://oe.huixinmuqiang.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ea.nszjky.cn

[U85] JS：可选链
来源：http://af.gzmigu.cn

a?.b?.c
来源：http://jj.gzmigu.cn

[U86] JS：空值合并
来源：http://jp.chemitech.net.cn

a ?? b
来源：http://er.shxzskj.cn

[U87] JS：解构默认值
来源：http://yz.yuexingan06.cn

const { a = 1, b = 2 } = obj;
来源：http://iq.nicolike.cn

[U88] JS：对象展开合并
来源：http://tl.yuexingan06.cn

{ ...a, ...b }
来源：http://qh.szsharing.cn

[U89] JS：数组去重
来源：http://cb.huixiangedu.cn

[...new Set(arr)]
来源：http://aa.newstarts.cn

[U90] JS：数字数组排序
来源：http://ok.hnjuh.cn

[...arr].sort((a, b) => a - b)
来源：http://xw.colortex.cn

[U91] JS：对象键值遍历
来源：http://dz.yuexingan06.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yo.bookmarksfly.cn

[U92] JS：深拷贝
来源：http://ux.bookmarksfly.cn

structuredClone(obj)
来源：http://od.hahajie.cn

[U93] JS：模板字符串
来源：http://ep.asd995.cn

`共 ${n} 条`
来源：http://hu.szsharing.cn

[U94] JS：箭头函数
来源：http://ul.shxzukj.cn

const double = x => x * 2;
来源：http://uz.shxzukj.cn

[U95] JS：Promise 包装
来源：http://ss.asd995.cn

new Promise((resolve, reject) => {})
来源：http://ld.hahajie.cn

[U96] JS：async/await 与异常
来源：http://mr.huixinmuqiang.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kh.asd995.cn

[U97] JS：并发请求
来源：http://ot.jianghongdianzi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://fi.bjjhwx.cn

[U98] JS：fetch 带 JSON
来源：http://ww.lnxyls.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tv.asd995.cn

[U99] JS：事件监听
来源：http://kr.haigaiapp.cn

el.addEventListener("click", e => {})
来源：http://bx.yuexingan06.cn

[U100] JS：DOM 查询
来源：http://nq.wgjwhj.cn

document.querySelector(".item")
来源：http://cv.panjiajie.cn

[U101] JS：classList 操作
来源：http://kn.lnxyls.cn

el.classList.toggle("active")
来源：http://ln.lnxyls.cn

[U102] JS：本地存储
来源：http://ii.huanxung.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://yf.asd995.cn

[U103] JS：定时器
来源：http://un.wgjwhj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zy.lnxyls.cn

[U104] JS：防抖
来源：http://wa.shxzukj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bl.hahajie.cn

[U105] JS：节流
来源：http://yg.jctech888.com.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gm.bookmarksfly.cn

[U106] JS：日期格式化
来源：http://tv.asd995.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fe.huixiangedu.cn

[U107] JS：数字千分位
来源：http://be.muxihuayi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://em.newstarts.cn

[U108] JS：随机整数
来源：http://do.bookmarksfly.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rt.szxytkj.cn

[U109] JS：数组分组
来源：http://vw.wgjwhj.cn

Object.groupBy(arr, x => x.type)
来源：http://pm.hahajie.cn

[U110] JS：数组分块
来源：http://td.gzmigu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://il.gzmigu.cn

[U111] JS：对象转 Map
来源：http://rb.newstarts.cn

new Map(Object.entries(obj))
来源：http://ny.panjiajie.cn

[U112] JS：字符串补位
来源：http://uc.huixinmuqiang.cn

"7".padStart(3, "0")
来源：http://mg.shtwfgs.cn


<!-- 参考信息 -->