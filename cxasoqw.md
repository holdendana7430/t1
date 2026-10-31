代发 wailian999

[T21] Swift：遍历
来源：http://lg.gzmigu.cn

for x in a { print(x) }
来源：http://ow.shxzukj.cn

[T22] Swift：字典
来源：http://ul.szsharing.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ih.wgjwhj.cn

[T23] Swift：函数
来源：http://rg.nszjky.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kp.huanxung.cn

[T24] Swift：闭包
来源：http://rz.jianghongdianzi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://tx.521024.cn

[T25] Swift：结构体
来源：http://gs.jianghongdianzi.cn

struct P { var x: Int }
来源：http://yh.wgjwhj.cn

[T26] Swift：类与重写
来源：http://up.gzmigu.cn

class A: Base { override func f() {} }
来源：http://ej.hnjuh.cn

[T27] Swift：错误处理
来源：http://vg.bookmarksfly.cn

do { try f() } catch { print(error) }
来源：http://rg.wgjwhj.cn

[T28] Swift：枚举
来源：http://ez.nicolike.cn

enum Color { case red, green }
来源：http://xn.asd995.cn

[T29] Swift：guard 提前返回
来源：http://ho.huanxung.cn

guard let x = opt else { return }
来源：http://rn.jctech888.com.cn

[T30] Swift：协议
来源：http://bi.hnjuh.cn

protocol Shape { func area() -> Double }
来源：http://gq.lnxyls.cn

[T31] Lua：Hello World
来源：http://bt.newstarts.cn

print("Hello")
来源：http://fw.panjiajie.cn

[T32] Lua：局部变量
来源：http://pu.wgjwhj.cn

local a = 1
来源：http://yk.nszjky.cn

[T33] Lua：表（数组）
来源：http://zi.hahajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zq.chemitech.net.cn

[T34] Lua：遍历表
来源：http://xf.huixiangedu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qo.gzmigu.cn

[T35] Lua：字典表
来源：http://vz.szsharing.cn

local d = { a = 1 };  d.b = 2
来源：http://cm.gzmigu.cn

[T36] Lua：函数
来源：http://vx.colortex.cn

function add(a, b) return a + b end
来源：http://in.wgjwhj.cn

[T37] Lua：字符串拼接
来源：http://qs.yuexingan06.cn

"a" .. "b"
来源：http://me.shxzukj.cn

[T38] Lua：条件
来源：http://dj.panjiajie.cn

if x > 0 then print("正") end
来源：http://ed.521024.cn

[T39] Lua：模式匹配
来源：http://rl.yuntaijiaju.cn

string.find(s, "%d+")
来源：http://nw.shtwfgs.cn

[T40] Lua：元表
来源：http://zt.muxihuayi.cn

setmetatable({}, { __index = base })
来源：http://ms.bookmarksfly.cn

[T41] Perl：Hello World
来源：http://sx.shxzskj.cn

print "Hello\n";
来源：http://dh.szxytkj.cn

[T42] Perl：变量类型
来源：http://hf.hahajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pb.chemitech.net.cn

[T43] Perl：字符串插值
来源：http://qy.jctech888.com.cn

"值: $a"
来源：http://uq.bjjhwx.cn

[T44] Perl：条件
来源：http://hb.jianghongdianzi.cn

if ($a > 0) { print "正"; }
来源：http://nu.wgjwhj.cn

[T45] Perl：数组遍历
来源：http://ie.huixiangedu.cn

for my $x (@arr) { print $x; }
来源：http://ah.jianghongdianzi.cn

[T46] Perl：哈希操作
来源：http://iv.nszjky.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jq.nicolike.cn

[T47] Perl：正则捕获
来源：http://cg.gzmigu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wd.huixinmuqiang.cn

[T48] Perl：正则替换
来源：http://bn.huixiangedu.cn

$s =~ s/old/new/g;
来源：http://jr.lnxyls.cn

[T49] Perl：函数
来源：http://mb.shxzskj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://aj.wgjwhj.cn

[T50] Perl：逐行读文件
来源：http://qw.shxzskj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://bm.szsharing.cn

while (my $line = <$fh>) { print $line; }
来源：http://ww.shxzskj.cn

[T51] Scala：Hello World
来源：http://og.panjiajie.cn

println("Hello")
来源：http://zo.chemitech.net.cn

[T52] Scala：变量
来源：http://th.muxihuayi.cn

val a = 1;  var b = 2
来源：http://qy.chemitech.net.cn

[T53] Scala：字符串插值
来源：http://nn.wgjwhj.cn

s"值: $b"
来源：http://gg.yuexingan06.cn

[T54] Scala：集合映射
来源：http://gl.nszjky.cn

List(1, 2, 3).map(_ * 2)
来源：http://os.wgjwhj.cn

[T55] Scala：集合过滤
来源：http://ht.chemitech.net.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ao.szsharing.cn

[T56] Scala：样例类
来源：http://ts.gzmigu.cn

case class User(name: String, age: Int)
来源：http://up.yuntaijiaju.cn

[T57] Scala：模式匹配
来源：http://yu.shxzukj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ih.colortex.cn

[T58] Scala：函数定义
来源：http://qx.huixiangedu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://xp.yuntaijiaju.cn

[T59] Scala：循环
来源：http://ky.haigaiapp.cn

for (i <- 1 to 10) println(i)
来源：http://gm.hnjuh.cn

[T60] Scala：折叠
来源：http://ak.nszjky.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fs.yuexingan06.cn

================================================================================
来源：http://al.hahajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lg.nszjky.cn

================================================================================
来源：http://xm.yuntaijiaju.cn

[U01] Py：创建虚拟环境
来源：http://zu.lnxyls.cn

python -m venv .venv && source .venv/bin/activate
来源：http://pj.shtwfgs.cn

[U02] Py：导出 / 安装依赖
来源：http://fl.nicolike.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hm.newstarts.cn

[U03] Py：加载 .env 配置
来源：http://ai.jianghongdianzi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://yj.9csxet.cn

[U04] Py：变量调试打印
来源：http://aq.szxytkj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cw.wgjwhj.cn

[U05] Py：列表去重且保序
来源：http://nz.huixinmuqiang.cn

list(dict.fromkeys(arr))
来源：http://pb.colortex.cn

[U06] Py：合并两个字典
来源：http://af.jctech888.com.cn

{**a, **b}
来源：http://qv.521024.cn

[U07] Py：反转字典键值
来源：http://va.lnxyls.cn

{v: k for k, v in d.items()}
来源：http://iv.shxzskj.cn

[U08] Py：展平二维列表
来源：http://ln.asd995.cn

[y for x in nested for y in x]
来源：http://bb.panjiajie.cn

[U09] Py：字典取最大值的键
来源：http://vt.chemitech.net.cn

max(d, key=d.get)
来源：http://dq.521024.cn

[U10] Py：按值排序字典
来源：http://jn.newstarts.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vj.muxihuayi.cn

[U11] Py：生成器表达式
来源：http://fg.shxzskj.cn

(x * 2 for x in arr)
来源：http://lr.asd995.cn

[U12] Py：取出现最多的 3 个元素
来源：http://oz.szsharing.cn

Counter(arr).most_common(3)
来源：http://xq.gzmigu.cn

[U13] Py：固定长度队列
来源：http://lb.shtwfgs.cn

deque(maxlen=10)
来源：http://eq.hahajie.cn

[U14] Py：分组收集到列表
来源：http://gc.yuexingan06.cn

defaultdict(list)
来源：http://xf.gzmigu.cn

[U15] Py：高精度计时
来源：http://zr.521024.cn

t = time.perf_counter()
来源：http://cm.hnjuh.cn

[U16] Py：命令行参数解析
来源：http://gu.shtwfgs.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ar.chemitech.net.cn

[U17] Py：初始化日志
来源：http://uo.colortex.cn

logging.basicConfig(level=logging.INFO)
来源：http://gk.jctech888.com.cn

[U18] Py：预编译正则
来源：http://uy.nszjky.cn

pat = re.compile(r"\d+")
来源：http://sr.huixinmuqiang.cn

[U19] Py：正则替换带回调
来源：http://vs.jctech888.com.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://aq.huanxung.cn

[U20] Py：缓存函数结果
来源：http://ak.shxzukj.cn

@functools.lru_cache(maxsize=None)
来源：http://vw.shxzskj.cn

[U21] Py：自定义上下文管理器
来源：http://bb.newstarts.cn

@contextlib.contextmanager
来源：http://qc.panjiajie.cn

[U22] Py：矩阵转置
来源：http://kq.jianghongdianzi.cn

list(zip(*m))
来源：http://ja.nicolike.cn

[U23] Py：分块读取大文件
来源：http://ek.panjiajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wc.shxzukj.cn

[U24] Py：路径操作
来源：http://gs.shxzukj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zz.haigaiapp.cn

[U25] Py：CSV 按字典读
来源：http://ul.hahajie.cn

csv.DictReader(f)
来源：http://io.muxihuayi.cn

[U26] Py：并发下载
来源：http://pb.shxzukj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wn.asd995.cn

[U27] Py：异步 HTTP
来源：http://xm.muxihuayi.cn

aiohttp.ClientSession() 配合 async with
来源：http://iu.huanxung.cn

[U28] Py：类型别名
来源：http://ip.yuexingan06.cn

UserId = int
来源：http://te.gzmigu.cn

[U29] Py：属性校验
来源：http://tj.haigaiapp.cn

@property 与 @x.setter 配合
来源：http://ap.huanxung.cn

[U30] Py：数据类
来源：http://qo.shtwfgs.cn

@dataclass(slots=True)
来源：http://zj.nszjky.cn

[U31] Py：单测
来源：http://pz.asd995.cn

python -m pytest -q
来源：http://jw.huanxung.cn

[U32] Py：代码格式化
来源：http://uw.szsharing.cn

ruff format . && ruff check --fix .
来源：http://li.bookmarksfly.cn

[U33] Py：打包发布
来源：http://bu.hnjuh.cn

python -m build  （依赖 pyproject.toml）
来源：http://ha.gzmigu.cn

[U34] Py：判断编码
来源：http://qk.szxytkj.cn

chardet.detect(raw)
来源：http://vm.chemitech.net.cn

[U35] Py：发送邮件
来源：http://jk.521024.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://uj.huixinmuqiang.cn

[U36] Py：定时任务
来源：http://js.shtwfgs.cn

schedule.every(10).minutes.do(job)
来源：http://nu.hahajie.cn

[U37] Py：读写 Excel
来源：http://vw.szxytkj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ph.panjiajie.cn

[U38] Py：获取脚本所在目录
来源：http://pw.huixiangedu.cn

Path(__file__).resolve().parent
来源：http://es.nszjky.cn

[U39] Py：判断是否在交互环境
来源：http://uq.bookmarksfly.cn

sys.stdout.isatty()
来源：http://cr.haigaiapp.cn

[U40] Py：打印到标准错误
来源：http://is.yuexingan06.cn

print("err", file=sys.stderr)
来源：http://yt.521024.cn

[U41] PHP：初始化 Composer 项目
来源：http://uk.haigaiapp.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://kf.yuexingan06.cn

[U42] PHP：PSR-4 自动加载
来源：http://so.9csxet.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vr.chemitech.net.cn

[U43] PHP：声明命名空间
来源：http://uv.huixinmuqiang.cn

namespace App\Http;
来源：http://tr.huixinmuqiang.cn

[U44] PHP：开启严格类型
来源：http://za.yuntaijiaju.cn

declare(strict_types=1);
来源：http://ap.muxihuayi.cn

[U45] PHP：类型声明与返回类型
来源：http://yk.lnxyls.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://pg.jianghongdianzi.cn

[U46] PHP：可空类型
来源：http://lh.muxihuayi.cn

?string $name = null
来源：http://kl.hahajie.cn

[U47] PHP：联合类型
来源：http://lj.bjjhwx.cn

int|string $id
来源：http://ad.muxihuayi.cn

[U48] PHP：纯枚举
来源：http://rs.9csxet.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fz.huixiangedu.cn

[U49] PHP：只读属性
来源：http://lq.huixinmuqiang.cn

public readonly string $name
来源：http://oh.asd995.cn

[U50] PHP：构造器属性提升
来源：http://aw.huixiangedu.cn

public function __construct(private int $id) {}
来源：http://yd.newstarts.cn

[U51] PHP：数组解构
来源：http://mc.shxzskj.cn

[$a, $b] = $arr;
来源：http://es.newstarts.cn

[U52] PHP：箭头函数
来源：http://xc.asd995.cn

$double = fn($x) => $x * 2;
来源：http://he.jctech888.com.cn

[U53] PHP：空合并运算符
来源：http://gr.newstarts.cn

$v = $a ?? $b ?? "default";
来源：http://na.muxihuayi.cn

[U54] PHP：空安全调用
来源：http://tp.gzmigu.cn

$obj?->method()
来源：http://xn.bookmarksfly.cn

[U55] PHP：match 表达式
来源：http://vz.yuexingan06.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jx.yuexingan06.cn

[U56] PHP：命名参数
来源：http://fx.nszjky.cn

f(a: 1, b: 2)
来源：http://lp.521024.cn

[U57] PHP：字符串插值
来源：http://xs.nicolike.cn

"值: {$a}"
来源：http://pv.shtwfgs.cn

[U58] PHP：数组三件套
来源：http://mc.jctech888.com.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://dv.jianghongdianzi.cn

[U59] PHP：自定义排序
来源：http://el.jctech888.com.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ui.bookmarksfly.cn

[U60] PHP：JSON 编解码
来源：http://lp.hnjuh.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dc.shxzskj.cn

[U61] PHP：正则
来源：http://wt.hahajie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bj.lnxyls.cn

[U62] PHP：日期对象
来源：http://st.panjiajie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hx.shxzskj.cn

[U63] PHP：文件读写
来源：http://fq.hnjuh.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pq.gzmigu.cn

[U64] PHP：目录遍历
来源：http://zj.huixinmuqiang.cn

glob("dir/*.php");  scandir("dir");
来源：http://hx.huixiangedu.cn

[U65] PHP：会话
来源：http://lz.shtwfgs.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ir.newstarts.cn

[U66] PHP：设置 Cookie
来源：http://pc.bjjhwx.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://br.huixiangedu.cn

[U67] PHP：处理文件上传
来源：http://yy.521024.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pp.asd995.cn

[U68] PHP：PDO 连接
来源：http://oh.shxzskj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vu.nszjky.cn

[U69] PHP：PDO 预处理
来源：http://gq.asd995.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://uz.panjiajie.cn

[U70] PHP：PDO 事务
来源：http://xr.asd995.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ws.bjjhwx.cn

[U71] PHP：抛出异常
来源：http://bq.muxihuayi.cn

throw new RuntimeException("失败", 500);
来源：http://ts.hnjuh.cn

[U72] PHP：写错误日志
来源：http://rv.jctech888.com.cn

error_log("失败: " . $e->getMessage());
来源：http://rq.9csxet.cn

[U73] PHP：读取 ini 配置
来源：http://sn.shxzukj.cn

parse_ini_file("config.ini", true)
来源：http://gr.hnjuh.cn

[U74] PHP：读取环境变量
来源：http://nb.9csxet.cn

getenv("APP_ENV") ?: "production"
来源：http://nc.wgjwhj.cn

[U75] PHP：依赖注入
来源：http://cf.huixiangedu.cn

composer require psr/container
来源：http://wa.yuntaijiaju.cn

[U76] PHP：简单路由
来源：http://tm.colortex.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yr.yuexingan06.cn

[U77] PHP：模板渲染
来源：http://yp.muxihuayi.cn

composer require twig/twig
来源：http://uq.521024.cn

[U78] PHP：单元测试
来源：http://mw.521024.cn

composer require --dev phpunit/phpunit
来源：http://tr.asd995.cn

[U79] PHP：静态分析
来源：http://wu.haigaiapp.cn

composer require --dev phpstan/phpstan
来源：http://de.panjiajie.cn

[U80] PHP：代码规范修复
来源：http://xk.521024.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jj.shxzukj.cn

[U81] JS：初始化项目
来源：http://yy.9csxet.cn

npm init -y;  npm i express
来源：http://tb.wgjwhj.cn

[U82] JS：package.json 脚本
来源：http://rx.szxytkj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sw.wgjwhj.cn

[U83] JS：ES Module 导入导出
来源：http://qo.hahajie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://et.jianghongdianzi.cn

[U84] JS：CommonJS 写法
来源：http://vc.chemitech.net.cn

module.exports = { a };  const { a } = require("./m");
来源：http://or.muxihuayi.cn

[U85] JS：可选链
来源：http://pi.huixiangedu.cn

a?.b?.c
来源：http://jo.521024.cn

[U86] JS：空值合并
来源：http://ym.chemitech.net.cn

a ?? b
来源：http://db.9csxet.cn

[U87] JS：解构默认值
来源：http://ul.jctech888.com.cn

const { a = 1, b = 2 } = obj;
来源：http://ox.bookmarksfly.cn

[U88] JS：对象展开合并
来源：http://vy.shxzukj.cn

{ ...a, ...b }
来源：http://rm.gzmigu.cn

[U89] JS：数组去重
来源：http://om.hahajie.cn

[...new Set(arr)]
来源：http://zw.colortex.cn

[U90] JS：数字数组排序
来源：http://tm.gzmigu.cn

[...arr].sort((a, b) => a - b)
来源：http://wy.yuexingan06.cn

[U91] JS：对象键值遍历
来源：http://qt.colortex.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mk.newstarts.cn

[U92] JS：深拷贝
来源：http://ad.jianghongdianzi.cn

structuredClone(obj)
来源：http://eg.lnxyls.cn

[U93] JS：模板字符串
来源：http://tc.hahajie.cn

`共 ${n} 条`
来源：http://gz.shxzukj.cn

[U94] JS：箭头函数
来源：http://ts.szxytkj.cn

const double = x => x * 2;
来源：http://il.lnxyls.cn

[U95] JS：Promise 包装
来源：http://er.jctech888.com.cn

new Promise((resolve, reject) => {})
来源：http://co.wgjwhj.cn

[U96] JS：async/await 与异常
来源：http://go.haigaiapp.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://le.jianghongdianzi.cn

[U97] JS：并发请求
来源：http://xk.shxzukj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://as.wgjwhj.cn

[U98] JS：fetch 带 JSON
来源：http://kb.szxytkj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://me.shxzskj.cn

[U99] JS：事件监听
来源：http://hr.lnxyls.cn

el.addEventListener("click", e => {})
来源：http://ty.huixiangedu.cn

[U100] JS：DOM 查询
来源：http://au.wgjwhj.cn

document.querySelector(".item")
来源：http://hv.chemitech.net.cn

[U101] JS：classList 操作
来源：http://bz.bjjhwx.cn

el.classList.toggle("active")
来源：http://oh.9csxet.cn

[U102] JS：本地存储
来源：http://nr.jianghongdianzi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ul.szxytkj.cn

[U103] JS：定时器
来源：http://ds.yuntaijiaju.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ug.szxytkj.cn

[U104] JS：防抖
来源：http://qy.huixinmuqiang.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jw.asd995.cn

[U105] JS：节流
来源：http://de.chemitech.net.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ft.gzmigu.cn

[U106] JS：日期格式化
来源：http://va.shtwfgs.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gm.newstarts.cn

[U107] JS：数字千分位
来源：http://pp.shxzskj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xu.huanxung.cn

[U108] JS：随机整数
来源：http://xv.521024.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jj.nszjky.cn


<!-- 参考信息 -->