代发 wailian999

[T19] Swift：可选绑定
来源：http://kc.bjjhwx.cn

if let n = opt { print(n) }
来源：http://qs.shxzukj.cn

[T20] Swift：数组操作
来源：http://ii.yuntaijiaju.cn

var a = [1, 2, 3];  a.append(4)
来源：http://uo.gzmigu.cn

[T21] Swift：遍历
来源：http://tn.shxzskj.cn

for x in a { print(x) }
来源：http://ll.haigaiapp.cn

[T22] Swift：字典
来源：http://fp.wgjwhj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://un.521024.cn

[T23] Swift：函数
来源：http://fu.gzmigu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://au.9csxet.cn

[T24] Swift：闭包
来源：http://qz.bookmarksfly.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://az.huixiangedu.cn

[T25] Swift：结构体
来源：http://kr.nszjky.cn

struct P { var x: Int }
来源：http://rl.colortex.cn

[T26] Swift：类与重写
来源：http://cb.asd995.cn

class A: Base { override func f() {} }
来源：http://il.yuntaijiaju.cn

[T27] Swift：错误处理
来源：http://ky.yuntaijiaju.cn

do { try f() } catch { print(error) }
来源：http://jf.shxzukj.cn

[T28] Swift：枚举
来源：http://vj.9csxet.cn

enum Color { case red, green }
来源：http://bl.muxihuayi.cn

[T29] Swift：guard 提前返回
来源：http://bv.asd995.cn

guard let x = opt else { return }
来源：http://ey.wgjwhj.cn

[T30] Swift：协议
来源：http://tl.shxzskj.cn

protocol Shape { func area() -> Double }
来源：http://be.asd995.cn

[T31] Lua：Hello World
来源：http://mz.wgjwhj.cn

print("Hello")
来源：http://vy.huixiangedu.cn

[T32] Lua：局部变量
来源：http://ww.yuntaijiaju.cn

local a = 1
来源：http://hi.muxihuayi.cn

[T33] Lua：表（数组）
来源：http://gl.lnxyls.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://br.shxzskj.cn

[T34] Lua：遍历表
来源：http://hu.colortex.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gf.hahajie.cn

[T35] Lua：字典表
来源：http://we.wgjwhj.cn

local d = { a = 1 };  d.b = 2
来源：http://iq.shtwfgs.cn

[T36] Lua：函数
来源：http://vt.haigaiapp.cn

function add(a, b) return a + b end
来源：http://lh.shxzskj.cn

[T37] Lua：字符串拼接
来源：http://nx.bookmarksfly.cn

"a" .. "b"
来源：http://qz.bookmarksfly.cn

[T38] Lua：条件
来源：http://zh.colortex.cn

if x > 0 then print("正") end
来源：http://ck.jctech888.com.cn

[T39] Lua：模式匹配
来源：http://az.9csxet.cn

string.find(s, "%d+")
来源：http://fx.yuexingan06.cn

[T40] Lua：元表
来源：http://qk.nszjky.cn

setmetatable({}, { __index = base })
来源：http://xe.huixinmuqiang.cn

[T41] Perl：Hello World
来源：http://sn.panjiajie.cn

print "Hello\n";
来源：http://ad.haigaiapp.cn

[T42] Perl：变量类型
来源：http://fe.lnxyls.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hl.huanxung.cn

[T43] Perl：字符串插值
来源：http://dl.colortex.cn

"值: $a"
来源：http://lq.nszjky.cn

[T44] Perl：条件
来源：http://br.shtwfgs.cn

if ($a > 0) { print "正"; }
来源：http://yc.521024.cn

[T45] Perl：数组遍历
来源：http://wj.shxzukj.cn

for my $x (@arr) { print $x; }
来源：http://tn.newstarts.cn

[T46] Perl：哈希操作
来源：http://ze.asd995.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vx.9csxet.cn

[T47] Perl：正则捕获
来源：http://xf.szsharing.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wh.yuntaijiaju.cn

[T48] Perl：正则替换
来源：http://rp.lnxyls.cn

$s =~ s/old/new/g;
来源：http://vk.hahajie.cn

[T49] Perl：函数
来源：http://vs.jianghongdianzi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gr.hahajie.cn

[T50] Perl：逐行读文件
来源：http://xy.szxytkj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://jf.gzmigu.cn

while (my $line = <$fh>) { print $line; }
来源：http://sa.huanxung.cn

[T51] Scala：Hello World
来源：http://cu.newstarts.cn

println("Hello")
来源：http://zf.asd995.cn

[T52] Scala：变量
来源：http://ij.bookmarksfly.cn

val a = 1;  var b = 2
来源：http://ic.szxytkj.cn

[T53] Scala：字符串插值
来源：http://ox.shxzskj.cn

s"值: $b"
来源：http://kq.shxzskj.cn

[T54] Scala：集合映射
来源：http://if.yuexingan06.cn

List(1, 2, 3).map(_ * 2)
来源：http://xn.bjjhwx.cn

[T55] Scala：集合过滤
来源：http://lg.jctech888.com.cn

List(1, 2, 3).filter(_ > 1)
来源：http://mm.asd995.cn

[T56] Scala：样例类
来源：http://xb.jianghongdianzi.cn

case class User(name: String, age: Int)
来源：http://vw.yuexingan06.cn

[T57] Scala：模式匹配
来源：http://cx.bjjhwx.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://db.muxihuayi.cn

[T58] Scala：函数定义
来源：http://bp.shxzskj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://hj.szsharing.cn

[T59] Scala：循环
来源：http://av.gzmigu.cn

for (i <- 1 to 10) println(i)
来源：http://az.hahajie.cn

[T60] Scala：折叠
来源：http://ig.muxihuayi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qi.bookmarksfly.cn

================================================================================
来源：http://dz.panjiajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fj.huanxung.cn

================================================================================
来源：http://lm.wgjwhj.cn

[U01] Py：创建虚拟环境
来源：http://ev.panjiajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nu.jctech888.com.cn

[U02] Py：导出 / 安装依赖
来源：http://bg.szsharing.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tm.nicolike.cn

[U03] Py：加载 .env 配置
来源：http://ya.shtwfgs.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rq.nicolike.cn

[U04] Py：变量调试打印
来源：http://mf.shxzskj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pp.lnxyls.cn

[U05] Py：列表去重且保序
来源：http://zr.huixinmuqiang.cn

list(dict.fromkeys(arr))
来源：http://ab.muxihuayi.cn

[U06] Py：合并两个字典
来源：http://uq.asd995.cn

{**a, **b}
来源：http://kx.jianghongdianzi.cn

[U07] Py：反转字典键值
来源：http://gg.shxzskj.cn

{v: k for k, v in d.items()}
来源：http://pl.huixiangedu.cn

[U08] Py：展平二维列表
来源：http://ju.huixiangedu.cn

[y for x in nested for y in x]
来源：http://ia.asd995.cn

[U09] Py：字典取最大值的键
来源：http://wp.yuexingan06.cn

max(d, key=d.get)
来源：http://qo.asd995.cn

[U10] Py：按值排序字典
来源：http://th.shtwfgs.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sf.colortex.cn

[U11] Py：生成器表达式
来源：http://cs.shtwfgs.cn

(x * 2 for x in arr)
来源：http://lf.bjjhwx.cn

[U12] Py：取出现最多的 3 个元素
来源：http://bk.yuexingan06.cn

Counter(arr).most_common(3)
来源：http://fq.hahajie.cn

[U13] Py：固定长度队列
来源：http://vb.gzmigu.cn

deque(maxlen=10)
来源：http://fg.yuntaijiaju.cn

[U14] Py：分组收集到列表
来源：http://jf.panjiajie.cn

defaultdict(list)
来源：http://tj.bookmarksfly.cn

[U15] Py：高精度计时
来源：http://de.nicolike.cn

t = time.perf_counter()
来源：http://xn.huixiangedu.cn

[U16] Py：命令行参数解析
来源：http://ex.jctech888.com.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yz.bookmarksfly.cn

[U17] Py：初始化日志
来源：http://ah.shxzskj.cn

logging.basicConfig(level=logging.INFO)
来源：http://uz.nszjky.cn

[U18] Py：预编译正则
来源：http://hw.yuntaijiaju.cn

pat = re.compile(r"\d+")
来源：http://rp.panjiajie.cn

[U19] Py：正则替换带回调
来源：http://iy.haigaiapp.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ol.hnjuh.cn

[U20] Py：缓存函数结果
来源：http://ew.shxzukj.cn

@functools.lru_cache(maxsize=None)
来源：http://ew.hahajie.cn

[U21] Py：自定义上下文管理器
来源：http://mf.yuntaijiaju.cn

@contextlib.contextmanager
来源：http://qh.shxzukj.cn

[U22] Py：矩阵转置
来源：http://ax.jianghongdianzi.cn

list(zip(*m))
来源：http://hh.szxytkj.cn

[U23] Py：分块读取大文件
来源：http://ol.wgjwhj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hv.panjiajie.cn

[U24] Py：路径操作
来源：http://di.panjiajie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://uf.yuexingan06.cn

[U25] Py：CSV 按字典读
来源：http://ov.jianghongdianzi.cn

csv.DictReader(f)
来源：http://lr.jctech888.com.cn

[U26] Py：并发下载
来源：http://kj.szsharing.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nj.haigaiapp.cn

[U27] Py：异步 HTTP
来源：http://db.nicolike.cn

aiohttp.ClientSession() 配合 async with
来源：http://qw.yuntaijiaju.cn

[U28] Py：类型别名
来源：http://su.521024.cn

UserId = int
来源：http://ut.hahajie.cn

[U29] Py：属性校验
来源：http://us.szxytkj.cn

@property 与 @x.setter 配合
来源：http://kz.nicolike.cn

[U30] Py：数据类
来源：http://iv.nszjky.cn

@dataclass(slots=True)
来源：http://wh.jctech888.com.cn

[U31] Py：单测
来源：http://wd.9csxet.cn

python -m pytest -q
来源：http://tm.nicolike.cn

[U32] Py：代码格式化
来源：http://lk.gzmigu.cn

ruff format . && ruff check --fix .
来源：http://yc.bookmarksfly.cn

[U33] Py：打包发布
来源：http://wh.nicolike.cn

python -m build  （依赖 pyproject.toml）
来源：http://yw.hnjuh.cn

[U34] Py：判断编码
来源：http://pg.szxytkj.cn

chardet.detect(raw)
来源：http://al.bjjhwx.cn

[U35] Py：发送邮件
来源：http://ex.nszjky.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lb.521024.cn

[U36] Py：定时任务
来源：http://as.haigaiapp.cn

schedule.every(10).minutes.do(job)
来源：http://za.chemitech.net.cn

[U37] Py：读写 Excel
来源：http://zm.szsharing.cn

pandas.read_excel / DataFrame.to_excel
来源：http://vx.yuntaijiaju.cn

[U38] Py：获取脚本所在目录
来源：http://ga.huixiangedu.cn

Path(__file__).resolve().parent
来源：http://qf.hnjuh.cn

[U39] Py：判断是否在交互环境
来源：http://ni.szsharing.cn

sys.stdout.isatty()
来源：http://ww.jianghongdianzi.cn

[U40] Py：打印到标准错误
来源：http://bh.jctech888.com.cn

print("err", file=sys.stderr)
来源：http://tf.szxytkj.cn

[U41] PHP：初始化 Composer 项目
来源：http://ex.shxzskj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://kq.hahajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://fw.jctech888.com.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://aj.szxytkj.cn

[U43] PHP：声明命名空间
来源：http://xm.gzmigu.cn

namespace App\Http;
来源：http://vn.newstarts.cn

[U44] PHP：开启严格类型
来源：http://ka.hnjuh.cn

declare(strict_types=1);
来源：http://hg.521024.cn

[U45] PHP：类型声明与返回类型
来源：http://zl.9csxet.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://xv.hahajie.cn

[U46] PHP：可空类型
来源：http://ck.huixiangedu.cn

?string $name = null
来源：http://vz.gzmigu.cn

[U47] PHP：联合类型
来源：http://jc.shtwfgs.cn

int|string $id
来源：http://wq.wgjwhj.cn

[U48] PHP：纯枚举
来源：http://ez.shtwfgs.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gc.huixiangedu.cn

[U49] PHP：只读属性
来源：http://ps.jianghongdianzi.cn

public readonly string $name
来源：http://np.wgjwhj.cn

[U50] PHP：构造器属性提升
来源：http://kl.521024.cn

public function __construct(private int $id) {}
来源：http://ko.huixinmuqiang.cn

[U51] PHP：数组解构
来源：http://ch.huixiangedu.cn

[$a, $b] = $arr;
来源：http://iw.hahajie.cn

[U52] PHP：箭头函数
来源：http://fm.yuntaijiaju.cn

$double = fn($x) => $x * 2;
来源：http://dr.9csxet.cn

[U53] PHP：空合并运算符
来源：http://ld.gzmigu.cn

$v = $a ?? $b ?? "default";
来源：http://zo.bjjhwx.cn

[U54] PHP：空安全调用
来源：http://xa.yuexingan06.cn

$obj?->method()
来源：http://yl.huanxung.cn

[U55] PHP：match 表达式
来源：http://cj.hnjuh.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ql.wgjwhj.cn

[U56] PHP：命名参数
来源：http://dt.asd995.cn

f(a: 1, b: 2)
来源：http://yy.9csxet.cn

[U57] PHP：字符串插值
来源：http://lc.shxzukj.cn

"值: {$a}"
来源：http://lo.gzmigu.cn

[U58] PHP：数组三件套
来源：http://yp.haigaiapp.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ul.wgjwhj.cn

[U59] PHP：自定义排序
来源：http://et.szxytkj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ul.szsharing.cn

[U60] PHP：JSON 编解码
来源：http://as.yuntaijiaju.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rn.huanxung.cn

[U61] PHP：正则
来源：http://rt.newstarts.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ac.nszjky.cn

[U62] PHP：日期对象
来源：http://vq.jctech888.com.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ju.hnjuh.cn

[U63] PHP：文件读写
来源：http://zf.wgjwhj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ph.shtwfgs.cn

[U64] PHP：目录遍历
来源：http://ve.panjiajie.cn

glob("dir/*.php");  scandir("dir");
来源：http://yf.hnjuh.cn

[U65] PHP：会话
来源：http://tn.newstarts.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://dy.yuntaijiaju.cn

[U66] PHP：设置 Cookie
来源：http://iz.lnxyls.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lj.yuntaijiaju.cn

[U67] PHP：处理文件上传
来源：http://dr.jianghongdianzi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ww.shtwfgs.cn

[U68] PHP：PDO 连接
来源：http://hn.jctech888.com.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gv.shxzskj.cn

[U69] PHP：PDO 预处理
来源：http://oq.shxzskj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wo.9csxet.cn

[U70] PHP：PDO 事务
来源：http://lw.haigaiapp.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gk.yuntaijiaju.cn

[U71] PHP：抛出异常
来源：http://wm.shxzukj.cn

throw new RuntimeException("失败", 500);
来源：http://we.newstarts.cn

[U72] PHP：写错误日志
来源：http://ha.haigaiapp.cn

error_log("失败: " . $e->getMessage());
来源：http://nv.nszjky.cn

[U73] PHP：读取 ini 配置
来源：http://yw.yuexingan06.cn

parse_ini_file("config.ini", true)
来源：http://qq.huixinmuqiang.cn

[U74] PHP：读取环境变量
来源：http://ob.nicolike.cn

getenv("APP_ENV") ?: "production"
来源：http://us.newstarts.cn

[U75] PHP：依赖注入
来源：http://fe.9csxet.cn

composer require psr/container
来源：http://hj.chemitech.net.cn

[U76] PHP：简单路由
来源：http://jq.lnxyls.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jg.huanxung.cn

[U77] PHP：模板渲染
来源：http://qk.yuexingan06.cn

composer require twig/twig
来源：http://zo.huanxung.cn

[U78] PHP：单元测试
来源：http://el.hahajie.cn

composer require --dev phpunit/phpunit
来源：http://vs.newstarts.cn

[U79] PHP：静态分析
来源：http://sf.yuexingan06.cn

composer require --dev phpstan/phpstan
来源：http://oc.lnxyls.cn

[U80] PHP：代码规范修复
来源：http://fh.wgjwhj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://av.wgjwhj.cn

[U81] JS：初始化项目
来源：http://qh.shxzukj.cn

npm init -y;  npm i express
来源：http://nb.shxzukj.cn

[U82] JS：package.json 脚本
来源：http://hb.colortex.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nt.colortex.cn

[U83] JS：ES Module 导入导出
来源：http://hp.lnxyls.cn

export const a = 1;  import { a } from "./m.js";
来源：http://sx.szxytkj.cn

[U84] JS：CommonJS 写法
来源：http://pa.shtwfgs.cn

module.exports = { a };  const { a } = require("./m");
来源：http://qk.521024.cn

[U85] JS：可选链
来源：http://hu.huixiangedu.cn

a?.b?.c
来源：http://yy.nicolike.cn

[U86] JS：空值合并
来源：http://aw.lnxyls.cn

a ?? b
来源：http://bs.colortex.cn

[U87] JS：解构默认值
来源：http://at.9csxet.cn

const { a = 1, b = 2 } = obj;
来源：http://nr.colortex.cn

[U88] JS：对象展开合并
来源：http://wa.hnjuh.cn

{ ...a, ...b }
来源：http://hf.huixiangedu.cn

[U89] JS：数组去重
来源：http://ro.gzmigu.cn

[...new Set(arr)]
来源：http://xt.szsharing.cn

[U90] JS：数字数组排序
来源：http://lw.shxzukj.cn

[...arr].sort((a, b) => a - b)
来源：http://sx.shxzskj.cn

[U91] JS：对象键值遍历
来源：http://fp.huixiangedu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ic.521024.cn

[U92] JS：深拷贝
来源：http://et.chemitech.net.cn

structuredClone(obj)
来源：http://kf.jctech888.com.cn

[U93] JS：模板字符串
来源：http://si.newstarts.cn

`共 ${n} 条`
来源：http://ds.huanxung.cn

[U94] JS：箭头函数
来源：http://to.jctech888.com.cn

const double = x => x * 2;
来源：http://pa.muxihuayi.cn

[U95] JS：Promise 包装
来源：http://gt.shtwfgs.cn

new Promise((resolve, reject) => {})
来源：http://sq.huanxung.cn

[U96] JS：async/await 与异常
来源：http://uz.gzmigu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://iy.521024.cn

[U97] JS：并发请求
来源：http://yv.yuexingan06.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://sn.shxzskj.cn

[U98] JS：fetch 带 JSON
来源：http://ji.bookmarksfly.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gq.szsharing.cn

[U99] JS：事件监听
来源：http://pk.muxihuayi.cn

el.addEventListener("click", e => {})
来源：http://wt.yuntaijiaju.cn

[U100] JS：DOM 查询
来源：http://zi.huixinmuqiang.cn

document.querySelector(".item")
来源：http://gc.newstarts.cn

[U101] JS：classList 操作
来源：http://td.shxzukj.cn

el.classList.toggle("active")
来源：http://na.newstarts.cn

[U102] JS：本地存储
来源：http://go.panjiajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://uo.gzmigu.cn

[U103] JS：定时器
来源：http://mo.huixinmuqiang.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gj.szsharing.cn

[U104] JS：防抖
来源：http://xp.521024.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bs.huixiangedu.cn

[U105] JS：节流
来源：http://km.9csxet.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yg.asd995.cn

[U106] JS：日期格式化
来源：http://kr.huanxung.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://id.shxzukj.cn


<!-- 参考信息 -->