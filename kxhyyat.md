代发 wailian999

[T21] Swift：遍历
来源：http://dm.jianghongdianzi.cn

for x in a { print(x) }
来源：http://ee.huixinmuqiang.cn

[T22] Swift：字典
来源：http://wg.muxihuayi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://qg.haigaiapp.cn

[T23] Swift：函数
来源：http://md.bookmarksfly.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sr.newstarts.cn

[T24] Swift：闭包
来源：http://jw.muxihuayi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vo.nszjky.cn

[T25] Swift：结构体
来源：http://kt.colortex.cn

struct P { var x: Int }
来源：http://jx.asd995.cn

[T26] Swift：类与重写
来源：http://tf.colortex.cn

class A: Base { override func f() {} }
来源：http://tp.hahajie.cn

[T27] Swift：错误处理
来源：http://ln.panjiajie.cn

do { try f() } catch { print(error) }
来源：http://wc.nicolike.cn

[T28] Swift：枚举
来源：http://he.bookmarksfly.cn

enum Color { case red, green }
来源：http://ty.huixinmuqiang.cn

[T29] Swift：guard 提前返回
来源：http://kb.jianghongdianzi.cn

guard let x = opt else { return }
来源：http://zw.bookmarksfly.cn

[T30] Swift：协议
来源：http://gk.bookmarksfly.cn

protocol Shape { func area() -> Double }
来源：http://cz.panjiajie.cn

[T31] Lua：Hello World
来源：http://ca.521024.cn

print("Hello")
来源：http://rc.szsharing.cn

[T32] Lua：局部变量
来源：http://so.yuexingan06.cn

local a = 1
来源：http://hy.shtwfgs.cn

[T33] Lua：表（数组）
来源：http://py.hahajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ke.muxihuayi.cn

[T34] Lua：遍历表
来源：http://xe.colortex.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ac.muxihuayi.cn

[T35] Lua：字典表
来源：http://xc.shxzukj.cn

local d = { a = 1 };  d.b = 2
来源：http://wx.bookmarksfly.cn

[T36] Lua：函数
来源：http://ca.shxzukj.cn

function add(a, b) return a + b end
来源：http://fa.yuexingan06.cn

[T37] Lua：字符串拼接
来源：http://kc.asd995.cn

"a" .. "b"
来源：http://be.muxihuayi.cn

[T38] Lua：条件
来源：http://qi.chemitech.net.cn

if x > 0 then print("正") end
来源：http://wz.bjjhwx.cn

[T39] Lua：模式匹配
来源：http://mz.wgjwhj.cn

string.find(s, "%d+")
来源：http://tz.lnxyls.cn

[T40] Lua：元表
来源：http://mm.chemitech.net.cn

setmetatable({}, { __index = base })
来源：http://zc.bookmarksfly.cn

[T41] Perl：Hello World
来源：http://um.shtwfgs.cn

print "Hello\n";
来源：http://kz.szsharing.cn

[T42] Perl：变量类型
来源：http://ay.yuntaijiaju.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yl.shxzskj.cn

[T43] Perl：字符串插值
来源：http://ax.9csxet.cn

"值: $a"
来源：http://gm.huixiangedu.cn

[T44] Perl：条件
来源：http://uw.nszjky.cn

if ($a > 0) { print "正"; }
来源：http://zr.wgjwhj.cn

[T45] Perl：数组遍历
来源：http://sc.lnxyls.cn

for my $x (@arr) { print $x; }
来源：http://xm.szxytkj.cn

[T46] Perl：哈希操作
来源：http://zp.huixinmuqiang.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ww.newstarts.cn

[T47] Perl：正则捕获
来源：http://gf.huixiangedu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xo.shxzukj.cn

[T48] Perl：正则替换
来源：http://tc.lnxyls.cn

$s =~ s/old/new/g;
来源：http://uz.jctech888.com.cn

[T49] Perl：函数
来源：http://id.hnjuh.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://uq.shxzukj.cn

[T50] Perl：逐行读文件
来源：http://ly.huixinmuqiang.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rk.newstarts.cn

while (my $line = <$fh>) { print $line; }
来源：http://lk.jctech888.com.cn

[T51] Scala：Hello World
来源：http://ud.shtwfgs.cn

println("Hello")
来源：http://qi.asd995.cn

[T52] Scala：变量
来源：http://dy.hahajie.cn

val a = 1;  var b = 2
来源：http://md.huanxung.cn

[T53] Scala：字符串插值
来源：http://sg.521024.cn

s"值: $b"
来源：http://je.newstarts.cn

[T54] Scala：集合映射
来源：http://yw.shxzukj.cn

List(1, 2, 3).map(_ * 2)
来源：http://sh.asd995.cn

[T55] Scala：集合过滤
来源：http://wn.lnxyls.cn

List(1, 2, 3).filter(_ > 1)
来源：http://on.yuexingan06.cn

[T56] Scala：样例类
来源：http://hd.hahajie.cn

case class User(name: String, age: Int)
来源：http://se.521024.cn

[T57] Scala：模式匹配
来源：http://uj.lnxyls.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://yd.hahajie.cn

[T58] Scala：函数定义
来源：http://zr.newstarts.cn

def add(a: Int, b: Int): Int = a + b
来源：http://kf.nicolike.cn

[T59] Scala：循环
来源：http://lv.521024.cn

for (i <- 1 to 10) println(i)
来源：http://yz.shxzukj.cn

[T60] Scala：折叠
来源：http://bl.hahajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rb.asd995.cn

================================================================================
来源：http://dn.colortex.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dm.colortex.cn

================================================================================
来源：http://to.shxzukj.cn

[U01] Py：创建虚拟环境
来源：http://vg.hnjuh.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zh.jctech888.com.cn

[U02] Py：导出 / 安装依赖
来源：http://ea.jctech888.com.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wz.bjjhwx.cn

[U03] Py：加载 .env 配置
来源：http://lo.chemitech.net.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://pe.haigaiapp.cn

[U04] Py：变量调试打印
来源：http://qa.asd995.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ua.asd995.cn

[U05] Py：列表去重且保序
来源：http://hj.panjiajie.cn

list(dict.fromkeys(arr))
来源：http://ne.hnjuh.cn

[U06] Py：合并两个字典
来源：http://ra.lnxyls.cn

{**a, **b}
来源：http://if.newstarts.cn

[U07] Py：反转字典键值
来源：http://dd.hahajie.cn

{v: k for k, v in d.items()}
来源：http://vn.asd995.cn

[U08] Py：展平二维列表
来源：http://wt.asd995.cn

[y for x in nested for y in x]
来源：http://ri.nszjky.cn

[U09] Py：字典取最大值的键
来源：http://yj.huixinmuqiang.cn

max(d, key=d.get)
来源：http://kh.yuntaijiaju.cn

[U10] Py：按值排序字典
来源：http://bl.shtwfgs.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uf.bjjhwx.cn

[U11] Py：生成器表达式
来源：http://sm.jianghongdianzi.cn

(x * 2 for x in arr)
来源：http://es.521024.cn

[U12] Py：取出现最多的 3 个元素
来源：http://jv.hnjuh.cn

Counter(arr).most_common(3)
来源：http://rf.521024.cn

[U13] Py：固定长度队列
来源：http://ag.szxytkj.cn

deque(maxlen=10)
来源：http://nv.nszjky.cn

[U14] Py：分组收集到列表
来源：http://wh.muxihuayi.cn

defaultdict(list)
来源：http://jn.gzmigu.cn

[U15] Py：高精度计时
来源：http://oo.shxzskj.cn

t = time.perf_counter()
来源：http://tm.jianghongdianzi.cn

[U16] Py：命令行参数解析
来源：http://ot.colortex.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://di.nszjky.cn

[U17] Py：初始化日志
来源：http://rk.9csxet.cn

logging.basicConfig(level=logging.INFO)
来源：http://as.wgjwhj.cn

[U18] Py：预编译正则
来源：http://xa.shtwfgs.cn

pat = re.compile(r"\d+")
来源：http://mq.bookmarksfly.cn

[U19] Py：正则替换带回调
来源：http://rs.shxzskj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wu.shxzskj.cn

[U20] Py：缓存函数结果
来源：http://ra.nicolike.cn

@functools.lru_cache(maxsize=None)
来源：http://jx.yuexingan06.cn

[U21] Py：自定义上下文管理器
来源：http://ax.huixiangedu.cn

@contextlib.contextmanager
来源：http://jk.9csxet.cn

[U22] Py：矩阵转置
来源：http://fu.bjjhwx.cn

list(zip(*m))
来源：http://ux.lnxyls.cn

[U23] Py：分块读取大文件
来源：http://tm.nicolike.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ui.szxytkj.cn

[U24] Py：路径操作
来源：http://cr.shxzskj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xb.wgjwhj.cn

[U25] Py：CSV 按字典读
来源：http://tn.lnxyls.cn

csv.DictReader(f)
来源：http://gj.521024.cn

[U26] Py：并发下载
来源：http://wp.bjjhwx.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lw.yuntaijiaju.cn

[U27] Py：异步 HTTP
来源：http://ph.jianghongdianzi.cn

aiohttp.ClientSession() 配合 async with
来源：http://ob.szxytkj.cn

[U28] Py：类型别名
来源：http://mo.jctech888.com.cn

UserId = int
来源：http://od.szxytkj.cn

[U29] Py：属性校验
来源：http://pe.shxzskj.cn

@property 与 @x.setter 配合
来源：http://zv.nszjky.cn

[U30] Py：数据类
来源：http://pl.shxzskj.cn

@dataclass(slots=True)
来源：http://wj.jianghongdianzi.cn

[U31] Py：单测
来源：http://vm.gzmigu.cn

python -m pytest -q
来源：http://gf.wgjwhj.cn

[U32] Py：代码格式化
来源：http://ng.nicolike.cn

ruff format . && ruff check --fix .
来源：http://kj.bjjhwx.cn

[U33] Py：打包发布
来源：http://xr.shxzskj.cn

python -m build  （依赖 pyproject.toml）
来源：http://tq.521024.cn

[U34] Py：判断编码
来源：http://pc.haigaiapp.cn

chardet.detect(raw)
来源：http://yv.bookmarksfly.cn

[U35] Py：发送邮件
来源：http://la.chemitech.net.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nd.521024.cn

[U36] Py：定时任务
来源：http://mv.haigaiapp.cn

schedule.every(10).minutes.do(job)
来源：http://og.huixinmuqiang.cn

[U37] Py：读写 Excel
来源：http://kb.panjiajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://tp.bookmarksfly.cn

[U38] Py：获取脚本所在目录
来源：http://iq.bookmarksfly.cn

Path(__file__).resolve().parent
来源：http://sd.szsharing.cn

[U39] Py：判断是否在交互环境
来源：http://qo.bjjhwx.cn

sys.stdout.isatty()
来源：http://uz.shxzskj.cn

[U40] Py：打印到标准错误
来源：http://ot.chemitech.net.cn

print("err", file=sys.stderr)
来源：http://da.shxzskj.cn

[U41] PHP：初始化 Composer 项目
来源：http://gc.yuntaijiaju.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://vj.shxzskj.cn

[U42] PHP：PSR-4 自动加载
来源：http://cl.jianghongdianzi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pa.panjiajie.cn

[U43] PHP：声明命名空间
来源：http://jk.bjjhwx.cn

namespace App\Http;
来源：http://ce.huixiangedu.cn

[U44] PHP：开启严格类型
来源：http://ey.nszjky.cn

declare(strict_types=1);
来源：http://bq.9csxet.cn

[U45] PHP：类型声明与返回类型
来源：http://as.521024.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://dp.wgjwhj.cn

[U46] PHP：可空类型
来源：http://go.colortex.cn

?string $name = null
来源：http://db.shxzskj.cn

[U47] PHP：联合类型
来源：http://lr.shtwfgs.cn

int|string $id
来源：http://hy.shxzukj.cn

[U48] PHP：纯枚举
来源：http://qx.yuntaijiaju.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yy.lnxyls.cn

[U49] PHP：只读属性
来源：http://xx.hahajie.cn

public readonly string $name
来源：http://bz.huanxung.cn

[U50] PHP：构造器属性提升
来源：http://qp.shxzskj.cn

public function __construct(private int $id) {}
来源：http://pu.lnxyls.cn

[U51] PHP：数组解构
来源：http://jn.shxzukj.cn

[$a, $b] = $arr;
来源：http://wj.chemitech.net.cn

[U52] PHP：箭头函数
来源：http://uk.lnxyls.cn

$double = fn($x) => $x * 2;
来源：http://gf.bookmarksfly.cn

[U53] PHP：空合并运算符
来源：http://zd.huixinmuqiang.cn

$v = $a ?? $b ?? "default";
来源：http://uu.lnxyls.cn

[U54] PHP：空安全调用
来源：http://bo.nicolike.cn

$obj?->method()
来源：http://bo.chemitech.net.cn

[U55] PHP：match 表达式
来源：http://fe.521024.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wh.colortex.cn

[U56] PHP：命名参数
来源：http://qp.haigaiapp.cn

f(a: 1, b: 2)
来源：http://nd.shxzukj.cn

[U57] PHP：字符串插值
来源：http://kd.chemitech.net.cn

"值: {$a}"
来源：http://cd.yuntaijiaju.cn

[U58] PHP：数组三件套
来源：http://rc.9csxet.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wl.colortex.cn

[U59] PHP：自定义排序
来源：http://dg.haigaiapp.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pm.hahajie.cn

[U60] PHP：JSON 编解码
来源：http://fp.huixinmuqiang.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fq.9csxet.cn

[U61] PHP：正则
来源：http://pq.nszjky.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qq.yuntaijiaju.cn

[U62] PHP：日期对象
来源：http://bc.huanxung.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jg.9csxet.cn

[U63] PHP：文件读写
来源：http://to.panjiajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ui.521024.cn

[U64] PHP：目录遍历
来源：http://zp.nicolike.cn

glob("dir/*.php");  scandir("dir");
来源：http://mq.yuexingan06.cn

[U65] PHP：会话
来源：http://nl.wgjwhj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vq.hahajie.cn

[U66] PHP：设置 Cookie
来源：http://jt.hnjuh.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mz.521024.cn

[U67] PHP：处理文件上传
来源：http://zt.bookmarksfly.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ir.shxzskj.cn

[U68] PHP：PDO 连接
来源：http://nw.asd995.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://iv.521024.cn

[U69] PHP：PDO 预处理
来源：http://mz.panjiajie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ye.asd995.cn

[U70] PHP：PDO 事务
来源：http://cg.huixinmuqiang.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fx.shxzskj.cn

[U71] PHP：抛出异常
来源：http://wj.chemitech.net.cn

throw new RuntimeException("失败", 500);
来源：http://yx.haigaiapp.cn

[U72] PHP：写错误日志
来源：http://on.nszjky.cn

error_log("失败: " . $e->getMessage());
来源：http://yq.shxzskj.cn

[U73] PHP：读取 ini 配置
来源：http://ah.shxzukj.cn

parse_ini_file("config.ini", true)
来源：http://in.521024.cn

[U74] PHP：读取环境变量
来源：http://kj.lnxyls.cn

getenv("APP_ENV") ?: "production"
来源：http://om.yuexingan06.cn

[U75] PHP：依赖注入
来源：http://wp.newstarts.cn

composer require psr/container
来源：http://zf.muxihuayi.cn

[U76] PHP：简单路由
来源：http://yw.huixiangedu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nn.nszjky.cn

[U77] PHP：模板渲染
来源：http://oq.nszjky.cn

composer require twig/twig
来源：http://ib.shtwfgs.cn

[U78] PHP：单元测试
来源：http://vq.haigaiapp.cn

composer require --dev phpunit/phpunit
来源：http://js.szsharing.cn

[U79] PHP：静态分析
来源：http://ge.huixinmuqiang.cn

composer require --dev phpstan/phpstan
来源：http://br.huixiangedu.cn

[U80] PHP：代码规范修复
来源：http://ps.huanxung.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://fs.lnxyls.cn

[U81] JS：初始化项目
来源：http://mr.nicolike.cn

npm init -y;  npm i express
来源：http://zn.szxytkj.cn

[U82] JS：package.json 脚本
来源：http://kl.yuexingan06.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nn.shtwfgs.cn

[U83] JS：ES Module 导入导出
来源：http://ur.szxytkj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://dv.521024.cn

[U84] JS：CommonJS 写法
来源：http://to.szxytkj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://lx.yuexingan06.cn

[U85] JS：可选链
来源：http://qo.gzmigu.cn

a?.b?.c
来源：http://fp.chemitech.net.cn

[U86] JS：空值合并
来源：http://cz.hahajie.cn

a ?? b
来源：http://qg.yuexingan06.cn

[U87] JS：解构默认值
来源：http://qs.muxihuayi.cn

const { a = 1, b = 2 } = obj;
来源：http://br.haigaiapp.cn

[U88] JS：对象展开合并
来源：http://ya.jctech888.com.cn

{ ...a, ...b }
来源：http://zk.shxzskj.cn

[U89] JS：数组去重
来源：http://ml.hahajie.cn

[...new Set(arr)]
来源：http://cf.muxihuayi.cn

[U90] JS：数字数组排序
来源：http://xo.yuntaijiaju.cn

[...arr].sort((a, b) => a - b)
来源：http://iw.haigaiapp.cn

[U91] JS：对象键值遍历
来源：http://li.huanxung.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bq.haigaiapp.cn

[U92] JS：深拷贝
来源：http://rb.bookmarksfly.cn

structuredClone(obj)
来源：http://sy.yuntaijiaju.cn

[U93] JS：模板字符串
来源：http://ay.nszjky.cn

`共 ${n} 条`
来源：http://ka.jianghongdianzi.cn

[U94] JS：箭头函数
来源：http://et.hahajie.cn

const double = x => x * 2;
来源：http://zc.szsharing.cn

[U95] JS：Promise 包装
来源：http://jn.gzmigu.cn

new Promise((resolve, reject) => {})
来源：http://vv.huixiangedu.cn

[U96] JS：async/await 与异常
来源：http://gg.shxzskj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fi.jctech888.com.cn

[U97] JS：并发请求
来源：http://oh.szxytkj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://xl.huanxung.cn

[U98] JS：fetch 带 JSON
来源：http://cn.yuntaijiaju.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://di.yuexingan06.cn

[U99] JS：事件监听
来源：http://jv.hahajie.cn

el.addEventListener("click", e => {})
来源：http://zp.jctech888.com.cn

[U100] JS：DOM 查询
来源：http://go.shtwfgs.cn

document.querySelector(".item")
来源：http://uu.bjjhwx.cn

[U101] JS：classList 操作
来源：http://ps.9csxet.cn

el.classList.toggle("active")
来源：http://cq.yuntaijiaju.cn

[U102] JS：本地存储
来源：http://ps.9csxet.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ti.szxytkj.cn

[U103] JS：定时器
来源：http://ls.szxytkj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://oz.wgjwhj.cn

[U104] JS：防抖
来源：http://xl.bjjhwx.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aj.huanxung.cn

[U105] JS：节流
来源：http://ew.huixiangedu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rd.huixiangedu.cn

[U106] JS：日期格式化
来源：http://vn.asd995.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pk.shxzukj.cn

[U107] JS：数字千分位
来源：http://rb.huixinmuqiang.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://om.huixiangedu.cn

[U108] JS：随机整数
来源：http://xr.huixinmuqiang.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ol.asd995.cn


<!-- 参考信息 -->