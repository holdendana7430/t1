代发 wailian999

[T23] Swift：函数
来源：http://vq.shxzukj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lu.shxzskj.cn

[T24] Swift：闭包
来源：http://lk.yuntaijiaju.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gd.yuntaijiaju.cn

[T25] Swift：结构体
来源：http://dd.asd995.cn

struct P { var x: Int }
来源：http://hl.chemitech.net.cn

[T26] Swift：类与重写
来源：http://xk.hnjuh.cn

class A: Base { override func f() {} }
来源：http://nb.hnjuh.cn

[T27] Swift：错误处理
来源：http://bi.asd995.cn

do { try f() } catch { print(error) }
来源：http://gv.asd995.cn

[T28] Swift：枚举
来源：http://gb.shtwfgs.cn

enum Color { case red, green }
来源：http://do.9csxet.cn

[T29] Swift：guard 提前返回
来源：http://tt.jianghongdianzi.cn

guard let x = opt else { return }
来源：http://ya.jianghongdianzi.cn

[T30] Swift：协议
来源：http://ii.yuntaijiaju.cn

protocol Shape { func area() -> Double }
来源：http://cs.bjjhwx.cn

[T31] Lua：Hello World
来源：http://pr.huixinmuqiang.cn

print("Hello")
来源：http://wr.lnxyls.cn

[T32] Lua：局部变量
来源：http://nu.asd995.cn

local a = 1
来源：http://lg.shxzskj.cn

[T33] Lua：表（数组）
来源：http://iv.hnjuh.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ao.yuntaijiaju.cn

[T34] Lua：遍历表
来源：http://zr.chemitech.net.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rp.yuexingan06.cn

[T35] Lua：字典表
来源：http://wd.nicolike.cn

local d = { a = 1 };  d.b = 2
来源：http://sh.nicolike.cn

[T36] Lua：函数
来源：http://vd.chemitech.net.cn

function add(a, b) return a + b end
来源：http://he.bookmarksfly.cn

[T37] Lua：字符串拼接
来源：http://rj.haigaiapp.cn

"a" .. "b"
来源：http://jv.asd995.cn

[T38] Lua：条件
来源：http://pd.shtwfgs.cn

if x > 0 then print("正") end
来源：http://go.lnxyls.cn

[T39] Lua：模式匹配
来源：http://qo.newstarts.cn

string.find(s, "%d+")
来源：http://dj.hnjuh.cn

[T40] Lua：元表
来源：http://sz.shxzskj.cn

setmetatable({}, { __index = base })
来源：http://sq.lnxyls.cn

[T41] Perl：Hello World
来源：http://yc.lnxyls.cn

print "Hello\n";
来源：http://ue.wgjwhj.cn

[T42] Perl：变量类型
来源：http://bp.nszjky.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sc.haigaiapp.cn

[T43] Perl：字符串插值
来源：http://qk.huixiangedu.cn

"值: $a"
来源：http://rj.jianghongdianzi.cn

[T44] Perl：条件
来源：http://lu.panjiajie.cn

if ($a > 0) { print "正"; }
来源：http://fo.521024.cn

[T45] Perl：数组遍历
来源：http://vw.shtwfgs.cn

for my $x (@arr) { print $x; }
来源：http://mk.chemitech.net.cn

[T46] Perl：哈希操作
来源：http://vx.hnjuh.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kd.shtwfgs.cn

[T47] Perl：正则捕获
来源：http://fq.shxzskj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://fo.huanxung.cn

[T48] Perl：正则替换
来源：http://lr.hnjuh.cn

$s =~ s/old/new/g;
来源：http://bw.chemitech.net.cn

[T49] Perl：函数
来源：http://af.jctech888.com.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rl.bjjhwx.cn

[T50] Perl：逐行读文件
来源：http://fh.haigaiapp.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://dp.shxzskj.cn

while (my $line = <$fh>) { print $line; }
来源：http://sv.lnxyls.cn

[T51] Scala：Hello World
来源：http://ru.bookmarksfly.cn

println("Hello")
来源：http://td.chemitech.net.cn

[T52] Scala：变量
来源：http://ip.jctech888.com.cn

val a = 1;  var b = 2
来源：http://it.jctech888.com.cn

[T53] Scala：字符串插值
来源：http://lh.nszjky.cn

s"值: $b"
来源：http://pu.bjjhwx.cn

[T54] Scala：集合映射
来源：http://ga.muxihuayi.cn

List(1, 2, 3).map(_ * 2)
来源：http://nl.huixinmuqiang.cn

[T55] Scala：集合过滤
来源：http://br.hahajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://tn.muxihuayi.cn

[T56] Scala：样例类
来源：http://in.shxzukj.cn

case class User(name: String, age: Int)
来源：http://qj.hnjuh.cn

[T57] Scala：模式匹配
来源：http://pk.nszjky.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://mv.szxytkj.cn

[T58] Scala：函数定义
来源：http://nz.huixiangedu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ta.huixinmuqiang.cn

[T59] Scala：循环
来源：http://th.asd995.cn

for (i <- 1 to 10) println(i)
来源：http://ak.newstarts.cn

[T60] Scala：折叠
来源：http://eh.nszjky.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bq.chemitech.net.cn

================================================================================
来源：http://sl.nicolike.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zm.haigaiapp.cn

================================================================================
来源：http://cu.yuexingan06.cn

[U01] Py：创建虚拟环境
来源：http://gz.lnxyls.cn

python -m venv .venv && source .venv/bin/activate
来源：http://eo.shxzukj.cn

[U02] Py：导出 / 安装依赖
来源：http://qj.szxytkj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hh.lnxyls.cn

[U03] Py：加载 .env 配置
来源：http://ac.haigaiapp.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ih.nszjky.cn

[U04] Py：变量调试打印
来源：http://va.haigaiapp.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mz.shxzskj.cn

[U05] Py：列表去重且保序
来源：http://jp.panjiajie.cn

list(dict.fromkeys(arr))
来源：http://rf.shxzukj.cn

[U06] Py：合并两个字典
来源：http://ey.szsharing.cn

{**a, **b}
来源：http://dd.chemitech.net.cn

[U07] Py：反转字典键值
来源：http://wc.hnjuh.cn

{v: k for k, v in d.items()}
来源：http://ue.jianghongdianzi.cn

[U08] Py：展平二维列表
来源：http://sm.asd995.cn

[y for x in nested for y in x]
来源：http://fe.shtwfgs.cn

[U09] Py：字典取最大值的键
来源：http://kj.lnxyls.cn

max(d, key=d.get)
来源：http://jg.jianghongdianzi.cn

[U10] Py：按值排序字典
来源：http://bc.newstarts.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nq.huixinmuqiang.cn

[U11] Py：生成器表达式
来源：http://ey.bjjhwx.cn

(x * 2 for x in arr)
来源：http://km.shxzukj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://nu.asd995.cn

Counter(arr).most_common(3)
来源：http://hg.jianghongdianzi.cn

[U13] Py：固定长度队列
来源：http://pi.szsharing.cn

deque(maxlen=10)
来源：http://sh.bookmarksfly.cn

[U14] Py：分组收集到列表
来源：http://nb.shxzukj.cn

defaultdict(list)
来源：http://np.hahajie.cn

[U15] Py：高精度计时
来源：http://eg.szxytkj.cn

t = time.perf_counter()
来源：http://at.gzmigu.cn

[U16] Py：命令行参数解析
来源：http://gf.nicolike.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sa.huanxung.cn

[U17] Py：初始化日志
来源：http://ub.szsharing.cn

logging.basicConfig(level=logging.INFO)
来源：http://bs.hnjuh.cn

[U18] Py：预编译正则
来源：http://jm.gzmigu.cn

pat = re.compile(r"\d+")
来源：http://mq.521024.cn

[U19] Py：正则替换带回调
来源：http://jy.bookmarksfly.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://iw.bookmarksfly.cn

[U20] Py：缓存函数结果
来源：http://ja.hnjuh.cn

@functools.lru_cache(maxsize=None)
来源：http://ar.nicolike.cn

[U21] Py：自定义上下文管理器
来源：http://vr.shxzskj.cn

@contextlib.contextmanager
来源：http://de.bjjhwx.cn

[U22] Py：矩阵转置
来源：http://dm.hnjuh.cn

list(zip(*m))
来源：http://oj.yuntaijiaju.cn

[U23] Py：分块读取大文件
来源：http://kb.9csxet.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ob.yuexingan06.cn

[U24] Py：路径操作
来源：http://sf.shxzskj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wv.huixinmuqiang.cn

[U25] Py：CSV 按字典读
来源：http://mr.jianghongdianzi.cn

csv.DictReader(f)
来源：http://aq.nicolike.cn

[U26] Py：并发下载
来源：http://hg.bjjhwx.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://uu.nszjky.cn

[U27] Py：异步 HTTP
来源：http://za.colortex.cn

aiohttp.ClientSession() 配合 async with
来源：http://zg.shtwfgs.cn

[U28] Py：类型别名
来源：http://mq.muxihuayi.cn

UserId = int
来源：http://tj.9csxet.cn

[U29] Py：属性校验
来源：http://qo.shtwfgs.cn

@property 与 @x.setter 配合
来源：http://mn.nicolike.cn

[U30] Py：数据类
来源：http://hl.gzmigu.cn

@dataclass(slots=True)
来源：http://nd.chemitech.net.cn

[U31] Py：单测
来源：http://vy.huixiangedu.cn

python -m pytest -q
来源：http://ed.newstarts.cn

[U32] Py：代码格式化
来源：http://cg.jctech888.com.cn

ruff format . && ruff check --fix .
来源：http://ic.wgjwhj.cn

[U33] Py：打包发布
来源：http://fn.gzmigu.cn

python -m build  （依赖 pyproject.toml）
来源：http://dq.shxzukj.cn

[U34] Py：判断编码
来源：http://si.jctech888.com.cn

chardet.detect(raw)
来源：http://nj.bjjhwx.cn

[U35] Py：发送邮件
来源：http://li.bookmarksfly.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dj.gzmigu.cn

[U36] Py：定时任务
来源：http://ea.szxytkj.cn

schedule.every(10).minutes.do(job)
来源：http://ll.shtwfgs.cn

[U37] Py：读写 Excel
来源：http://kx.lnxyls.cn

pandas.read_excel / DataFrame.to_excel
来源：http://gc.haigaiapp.cn

[U38] Py：获取脚本所在目录
来源：http://bg.asd995.cn

Path(__file__).resolve().parent
来源：http://sx.newstarts.cn

[U39] Py：判断是否在交互环境
来源：http://cs.bjjhwx.cn

sys.stdout.isatty()
来源：http://rb.nicolike.cn

[U40] Py：打印到标准错误
来源：http://vd.jianghongdianzi.cn

print("err", file=sys.stderr)
来源：http://tu.szxytkj.cn

[U41] PHP：初始化 Composer 项目
来源：http://mm.newstarts.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://bl.muxihuayi.cn

[U42] PHP：PSR-4 自动加载
来源：http://pj.shxzskj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yb.newstarts.cn

[U43] PHP：声明命名空间
来源：http://sw.colortex.cn

namespace App\Http;
来源：http://lk.nicolike.cn

[U44] PHP：开启严格类型
来源：http://df.jctech888.com.cn

declare(strict_types=1);
来源：http://df.bookmarksfly.cn

[U45] PHP：类型声明与返回类型
来源：http://vl.haigaiapp.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://yd.chemitech.net.cn

[U46] PHP：可空类型
来源：http://ey.yuntaijiaju.cn

?string $name = null
来源：http://vh.muxihuayi.cn

[U47] PHP：联合类型
来源：http://kb.gzmigu.cn

int|string $id
来源：http://qx.lnxyls.cn

[U48] PHP：纯枚举
来源：http://cc.nszjky.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tv.colortex.cn

[U49] PHP：只读属性
来源：http://uu.shxzukj.cn

public readonly string $name
来源：http://pj.gzmigu.cn

[U50] PHP：构造器属性提升
来源：http://ci.shtwfgs.cn

public function __construct(private int $id) {}
来源：http://ze.panjiajie.cn

[U51] PHP：数组解构
来源：http://xk.yuntaijiaju.cn

[$a, $b] = $arr;
来源：http://zb.asd995.cn

[U52] PHP：箭头函数
来源：http://nn.yuexingan06.cn

$double = fn($x) => $x * 2;
来源：http://yb.jctech888.com.cn

[U53] PHP：空合并运算符
来源：http://ct.chemitech.net.cn

$v = $a ?? $b ?? "default";
来源：http://cm.bjjhwx.cn

[U54] PHP：空安全调用
来源：http://vo.hahajie.cn

$obj?->method()
来源：http://pm.jianghongdianzi.cn

[U55] PHP：match 表达式
来源：http://sn.huixiangedu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tb.wgjwhj.cn

[U56] PHP：命名参数
来源：http://kz.wgjwhj.cn

f(a: 1, b: 2)
来源：http://qr.shtwfgs.cn

[U57] PHP：字符串插值
来源：http://yb.bookmarksfly.cn

"值: {$a}"
来源：http://tv.9csxet.cn

[U58] PHP：数组三件套
来源：http://iz.colortex.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hc.9csxet.cn

[U59] PHP：自定义排序
来源：http://fo.jianghongdianzi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eo.lnxyls.cn

[U60] PHP：JSON 编解码
来源：http://qr.521024.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ar.jctech888.com.cn

[U61] PHP：正则
来源：http://hx.lnxyls.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://oh.gzmigu.cn

[U62] PHP：日期对象
来源：http://qf.haigaiapp.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://do.9csxet.cn

[U63] PHP：文件读写
来源：http://ri.yuexingan06.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zv.chemitech.net.cn

[U64] PHP：目录遍历
来源：http://kg.huixinmuqiang.cn

glob("dir/*.php");  scandir("dir");
来源：http://fh.yuntaijiaju.cn

[U65] PHP：会话
来源：http://po.colortex.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rm.9csxet.cn

[U66] PHP：设置 Cookie
来源：http://pc.9csxet.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yf.9csxet.cn

[U67] PHP：处理文件上传
来源：http://nh.521024.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bm.panjiajie.cn

[U68] PHP：PDO 连接
来源：http://eu.hahajie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gn.huixinmuqiang.cn

[U69] PHP：PDO 预处理
来源：http://jj.jianghongdianzi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://or.newstarts.cn

[U70] PHP：PDO 事务
来源：http://di.haigaiapp.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ty.nicolike.cn

[U71] PHP：抛出异常
来源：http://uc.chemitech.net.cn

throw new RuntimeException("失败", 500);
来源：http://ak.yuntaijiaju.cn

[U72] PHP：写错误日志
来源：http://af.szxytkj.cn

error_log("失败: " . $e->getMessage());
来源：http://hl.gzmigu.cn

[U73] PHP：读取 ini 配置
来源：http://yx.yuntaijiaju.cn

parse_ini_file("config.ini", true)
来源：http://ox.lnxyls.cn

[U74] PHP：读取环境变量
来源：http://dw.huixiangedu.cn

getenv("APP_ENV") ?: "production"
来源：http://yx.bjjhwx.cn

[U75] PHP：依赖注入
来源：http://lv.yuexingan06.cn

composer require psr/container
来源：http://fp.9csxet.cn

[U76] PHP：简单路由
来源：http://pp.shxzukj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lg.shxzskj.cn

[U77] PHP：模板渲染
来源：http://gp.jctech888.com.cn

composer require twig/twig
来源：http://db.wgjwhj.cn

[U78] PHP：单元测试
来源：http://br.szsharing.cn

composer require --dev phpunit/phpunit
来源：http://fg.bjjhwx.cn

[U79] PHP：静态分析
来源：http://gj.gzmigu.cn

composer require --dev phpstan/phpstan
来源：http://rq.asd995.cn

[U80] PHP：代码规范修复
来源：http://op.hahajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://pz.colortex.cn

[U81] JS：初始化项目
来源：http://jc.huixiangedu.cn

npm init -y;  npm i express
来源：http://fo.panjiajie.cn

[U82] JS：package.json 脚本
来源：http://iv.nszjky.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://oc.gzmigu.cn

[U83] JS：ES Module 导入导出
来源：http://yt.yuntaijiaju.cn

export const a = 1;  import { a } from "./m.js";
来源：http://hj.shxzukj.cn

[U84] JS：CommonJS 写法
来源：http://xo.bookmarksfly.cn

module.exports = { a };  const { a } = require("./m");
来源：http://hh.bjjhwx.cn

[U85] JS：可选链
来源：http://uj.jianghongdianzi.cn

a?.b?.c
来源：http://xu.bjjhwx.cn

[U86] JS：空值合并
来源：http://pu.szsharing.cn

a ?? b
来源：http://rb.colortex.cn

[U87] JS：解构默认值
来源：http://gz.shxzskj.cn

const { a = 1, b = 2 } = obj;
来源：http://ks.asd995.cn

[U88] JS：对象展开合并
来源：http://td.shtwfgs.cn

{ ...a, ...b }
来源：http://bw.gzmigu.cn

[U89] JS：数组去重
来源：http://to.yuexingan06.cn

[...new Set(arr)]
来源：http://sa.huixinmuqiang.cn

[U90] JS：数字数组排序
来源：http://fb.chemitech.net.cn

[...arr].sort((a, b) => a - b)
来源：http://rp.chemitech.net.cn

[U91] JS：对象键值遍历
来源：http://sb.hahajie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://du.haigaiapp.cn

[U92] JS：深拷贝
来源：http://hp.szsharing.cn

structuredClone(obj)
来源：http://ue.asd995.cn

[U93] JS：模板字符串
来源：http://wl.jianghongdianzi.cn

`共 ${n} 条`
来源：http://io.gzmigu.cn

[U94] JS：箭头函数
来源：http://ly.wgjwhj.cn

const double = x => x * 2;
来源：http://pn.yuexingan06.cn

[U95] JS：Promise 包装
来源：http://rq.asd995.cn

new Promise((resolve, reject) => {})
来源：http://bt.bjjhwx.cn

[U96] JS：async/await 与异常
来源：http://dk.nicolike.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bc.yuexingan06.cn

[U97] JS：并发请求
来源：http://fi.shxzskj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ws.9csxet.cn

[U98] JS：fetch 带 JSON
来源：http://gq.gzmigu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://va.szsharing.cn

[U99] JS：事件监听
来源：http://kl.jianghongdianzi.cn

el.addEventListener("click", e => {})
来源：http://on.shxzukj.cn

[U100] JS：DOM 查询
来源：http://au.colortex.cn

document.querySelector(".item")
来源：http://za.9csxet.cn

[U101] JS：classList 操作
来源：http://jh.huixiangedu.cn

el.classList.toggle("active")
来源：http://ri.huixiangedu.cn

[U102] JS：本地存储
来源：http://su.yuntaijiaju.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xv.szsharing.cn

[U103] JS：定时器
来源：http://fg.colortex.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rt.bookmarksfly.cn

[U104] JS：防抖
来源：http://si.nszjky.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pk.shtwfgs.cn

[U105] JS：节流
来源：http://ix.yuexingan06.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gq.yuexingan06.cn

[U106] JS：日期格式化
来源：http://ee.haigaiapp.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yc.lnxyls.cn

[U107] JS：数字千分位
来源：http://fn.shtwfgs.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cr.chemitech.net.cn

[U108] JS：随机整数
来源：http://yv.shxzskj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://or.gzmigu.cn

[U109] JS：数组分组
来源：http://da.shxzukj.cn

Object.groupBy(arr, x => x.type)
来源：http://al.yuntaijiaju.cn

[U110] JS：数组分块
来源：http://hn.panjiajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://td.panjiajie.cn


<!-- 参考信息 -->