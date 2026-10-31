代发 wailian999

[T23] Swift：函数
来源：http://na.shxzskj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yl.szxytkj.cn

[T24] Swift：闭包
来源：http://cy.huanxung.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://we.hahajie.cn

[T25] Swift：结构体
来源：http://nz.jctech888.com.cn

struct P { var x: Int }
来源：http://em.jctech888.com.cn

[T26] Swift：类与重写
来源：http://mq.gzmigu.cn

class A: Base { override func f() {} }
来源：http://jr.jctech888.com.cn

[T27] Swift：错误处理
来源：http://il.nicolike.cn

do { try f() } catch { print(error) }
来源：http://er.hahajie.cn

[T28] Swift：枚举
来源：http://cj.jianghongdianzi.cn

enum Color { case red, green }
来源：http://om.muxihuayi.cn

[T29] Swift：guard 提前返回
来源：http://ce.huanxung.cn

guard let x = opt else { return }
来源：http://gb.huixinmuqiang.cn

[T30] Swift：协议
来源：http://dq.panjiajie.cn

protocol Shape { func area() -> Double }
来源：http://me.521024.cn

[T31] Lua：Hello World
来源：http://ep.yuntaijiaju.cn

print("Hello")
来源：http://rg.shxzskj.cn

[T32] Lua：局部变量
来源：http://sf.huanxung.cn

local a = 1
来源：http://xn.newstarts.cn

[T33] Lua：表（数组）
来源：http://ea.panjiajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ob.szsharing.cn

[T34] Lua：遍历表
来源：http://ej.shtwfgs.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rv.hahajie.cn

[T35] Lua：字典表
来源：http://kg.bookmarksfly.cn

local d = { a = 1 };  d.b = 2
来源：http://yz.huixiangedu.cn

[T36] Lua：函数
来源：http://zl.huixinmuqiang.cn

function add(a, b) return a + b end
来源：http://wb.hnjuh.cn

[T37] Lua：字符串拼接
来源：http://en.newstarts.cn

"a" .. "b"
来源：http://hy.szsharing.cn

[T38] Lua：条件
来源：http://bn.jctech888.com.cn

if x > 0 then print("正") end
来源：http://mt.bookmarksfly.cn

[T39] Lua：模式匹配
来源：http://uz.jctech888.com.cn

string.find(s, "%d+")
来源：http://gt.huanxung.cn

[T40] Lua：元表
来源：http://ki.shtwfgs.cn

setmetatable({}, { __index = base })
来源：http://wf.yuexingan06.cn

[T41] Perl：Hello World
来源：http://te.szsharing.cn

print "Hello\n";
来源：http://km.hnjuh.cn

[T42] Perl：变量类型
来源：http://wa.huanxung.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mq.szsharing.cn

[T43] Perl：字符串插值
来源：http://ua.huixiangedu.cn

"值: $a"
来源：http://dz.jctech888.com.cn

[T44] Perl：条件
来源：http://pp.haigaiapp.cn

if ($a > 0) { print "正"; }
来源：http://kx.hahajie.cn

[T45] Perl：数组遍历
来源：http://fp.szxytkj.cn

for my $x (@arr) { print $x; }
来源：http://iz.szsharing.cn

[T46] Perl：哈希操作
来源：http://ap.haigaiapp.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://yi.yuntaijiaju.cn

[T47] Perl：正则捕获
来源：http://mq.szsharing.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ck.colortex.cn

[T48] Perl：正则替换
来源：http://vk.9csxet.cn

$s =~ s/old/new/g;
来源：http://sh.shxzskj.cn

[T49] Perl：函数
来源：http://tb.bookmarksfly.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://px.haigaiapp.cn

[T50] Perl：逐行读文件
来源：http://uc.shxzukj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://kb.muxihuayi.cn

while (my $line = <$fh>) { print $line; }
来源：http://fw.bookmarksfly.cn

[T51] Scala：Hello World
来源：http://jk.huixinmuqiang.cn

println("Hello")
来源：http://cr.lnxyls.cn

[T52] Scala：变量
来源：http://yh.521024.cn

val a = 1;  var b = 2
来源：http://hp.lnxyls.cn

[T53] Scala：字符串插值
来源：http://yx.bjjhwx.cn

s"值: $b"
来源：http://to.bjjhwx.cn

[T54] Scala：集合映射
来源：http://ee.9csxet.cn

List(1, 2, 3).map(_ * 2)
来源：http://mp.bookmarksfly.cn

[T55] Scala：集合过滤
来源：http://et.gzmigu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://yv.521024.cn

[T56] Scala：样例类
来源：http://nn.szsharing.cn

case class User(name: String, age: Int)
来源：http://oa.shxzukj.cn

[T57] Scala：模式匹配
来源：http://tj.9csxet.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ty.lnxyls.cn

[T58] Scala：函数定义
来源：http://pu.panjiajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://qw.shtwfgs.cn

[T59] Scala：循环
来源：http://gn.jianghongdianzi.cn

for (i <- 1 to 10) println(i)
来源：http://uo.hahajie.cn

[T60] Scala：折叠
来源：http://ei.shxzukj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ay.bookmarksfly.cn

================================================================================
来源：http://hh.chemitech.net.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ro.huixinmuqiang.cn

================================================================================
来源：http://ko.huixinmuqiang.cn

[U01] Py：创建虚拟环境
来源：http://pm.chemitech.net.cn

python -m venv .venv && source .venv/bin/activate
来源：http://he.haigaiapp.cn

[U02] Py：导出 / 安装依赖
来源：http://wr.szxytkj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yv.nicolike.cn

[U03] Py：加载 .env 配置
来源：http://av.hahajie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://tf.nicolike.cn

[U04] Py：变量调试打印
来源：http://dv.nicolike.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sx.huixinmuqiang.cn

[U05] Py：列表去重且保序
来源：http://sm.huanxung.cn

list(dict.fromkeys(arr))
来源：http://nw.haigaiapp.cn

[U06] Py：合并两个字典
来源：http://oq.muxihuayi.cn

{**a, **b}
来源：http://ec.jianghongdianzi.cn

[U07] Py：反转字典键值
来源：http://vm.bookmarksfly.cn

{v: k for k, v in d.items()}
来源：http://wk.hahajie.cn

[U08] Py：展平二维列表
来源：http://io.chemitech.net.cn

[y for x in nested for y in x]
来源：http://kz.asd995.cn

[U09] Py：字典取最大值的键
来源：http://lz.9csxet.cn

max(d, key=d.get)
来源：http://hy.huanxung.cn

[U10] Py：按值排序字典
来源：http://fl.hahajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fd.newstarts.cn

[U11] Py：生成器表达式
来源：http://wj.muxihuayi.cn

(x * 2 for x in arr)
来源：http://vw.nszjky.cn

[U12] Py：取出现最多的 3 个元素
来源：http://as.haigaiapp.cn

Counter(arr).most_common(3)
来源：http://xw.jctech888.com.cn

[U13] Py：固定长度队列
来源：http://tb.shtwfgs.cn

deque(maxlen=10)
来源：http://lo.bookmarksfly.cn

[U14] Py：分组收集到列表
来源：http://co.hahajie.cn

defaultdict(list)
来源：http://ow.huixiangedu.cn

[U15] Py：高精度计时
来源：http://kp.yuexingan06.cn

t = time.perf_counter()
来源：http://wr.huanxung.cn

[U16] Py：命令行参数解析
来源：http://xq.yuexingan06.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hf.colortex.cn

[U17] Py：初始化日志
来源：http://kf.huixiangedu.cn

logging.basicConfig(level=logging.INFO)
来源：http://uu.szxytkj.cn

[U18] Py：预编译正则
来源：http://qj.gzmigu.cn

pat = re.compile(r"\d+")
来源：http://zz.huixiangedu.cn

[U19] Py：正则替换带回调
来源：http://ft.haigaiapp.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jo.haigaiapp.cn

[U20] Py：缓存函数结果
来源：http://cf.nicolike.cn

@functools.lru_cache(maxsize=None)
来源：http://op.jctech888.com.cn

[U21] Py：自定义上下文管理器
来源：http://en.muxihuayi.cn

@contextlib.contextmanager
来源：http://uz.jctech888.com.cn

[U22] Py：矩阵转置
来源：http://do.panjiajie.cn

list(zip(*m))
来源：http://vp.haigaiapp.cn

[U23] Py：分块读取大文件
来源：http://qc.shxzskj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ya.gzmigu.cn

[U24] Py：路径操作
来源：http://qe.muxihuayi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kj.9csxet.cn

[U25] Py：CSV 按字典读
来源：http://my.shxzukj.cn

csv.DictReader(f)
来源：http://st.jctech888.com.cn

[U26] Py：并发下载
来源：http://ur.wgjwhj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xr.lnxyls.cn

[U27] Py：异步 HTTP
来源：http://up.shxzskj.cn

aiohttp.ClientSession() 配合 async with
来源：http://nu.asd995.cn

[U28] Py：类型别名
来源：http://zx.chemitech.net.cn

UserId = int
来源：http://qp.jctech888.com.cn

[U29] Py：属性校验
来源：http://ug.huixinmuqiang.cn

@property 与 @x.setter 配合
来源：http://wj.nszjky.cn

[U30] Py：数据类
来源：http://cy.colortex.cn

@dataclass(slots=True)
来源：http://sv.gzmigu.cn

[U31] Py：单测
来源：http://xn.huixiangedu.cn

python -m pytest -q
来源：http://al.wgjwhj.cn

[U32] Py：代码格式化
来源：http://jy.asd995.cn

ruff format . && ruff check --fix .
来源：http://mp.lnxyls.cn

[U33] Py：打包发布
来源：http://ih.huixinmuqiang.cn

python -m build  （依赖 pyproject.toml）
来源：http://br.huanxung.cn

[U34] Py：判断编码
来源：http://xu.shxzskj.cn

chardet.detect(raw)
来源：http://tn.gzmigu.cn

[U35] Py：发送邮件
来源：http://cr.gzmigu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vc.szsharing.cn

[U36] Py：定时任务
来源：http://ct.bjjhwx.cn

schedule.every(10).minutes.do(job)
来源：http://nz.huixinmuqiang.cn

[U37] Py：读写 Excel
来源：http://sf.szxytkj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://sx.shxzskj.cn

[U38] Py：获取脚本所在目录
来源：http://db.chemitech.net.cn

Path(__file__).resolve().parent
来源：http://fg.shxzskj.cn

[U39] Py：判断是否在交互环境
来源：http://ja.lnxyls.cn

sys.stdout.isatty()
来源：http://dz.nicolike.cn

[U40] Py：打印到标准错误
来源：http://sb.9csxet.cn

print("err", file=sys.stderr)
来源：http://no.shxzskj.cn

[U41] PHP：初始化 Composer 项目
来源：http://ww.hnjuh.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://bj.521024.cn

[U42] PHP：PSR-4 自动加载
来源：http://wn.bjjhwx.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ep.hahajie.cn

[U43] PHP：声明命名空间
来源：http://xg.newstarts.cn

namespace App\Http;
来源：http://pa.panjiajie.cn

[U44] PHP：开启严格类型
来源：http://pd.huixiangedu.cn

declare(strict_types=1);
来源：http://gs.jctech888.com.cn

[U45] PHP：类型声明与返回类型
来源：http://sv.hahajie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ch.shxzskj.cn

[U46] PHP：可空类型
来源：http://mi.newstarts.cn

?string $name = null
来源：http://im.hnjuh.cn

[U47] PHP：联合类型
来源：http://ey.shxzskj.cn

int|string $id
来源：http://lk.chemitech.net.cn

[U48] PHP：纯枚举
来源：http://pf.szxytkj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lh.huixinmuqiang.cn

[U49] PHP：只读属性
来源：http://xn.shxzskj.cn

public readonly string $name
来源：http://fb.newstarts.cn

[U50] PHP：构造器属性提升
来源：http://sb.huanxung.cn

public function __construct(private int $id) {}
来源：http://pi.hahajie.cn

[U51] PHP：数组解构
来源：http://aq.muxihuayi.cn

[$a, $b] = $arr;
来源：http://hj.newstarts.cn

[U52] PHP：箭头函数
来源：http://on.9csxet.cn

$double = fn($x) => $x * 2;
来源：http://xh.nszjky.cn

[U53] PHP：空合并运算符
来源：http://jg.gzmigu.cn

$v = $a ?? $b ?? "default";
来源：http://tx.newstarts.cn

[U54] PHP：空安全调用
来源：http://mc.wgjwhj.cn

$obj?->method()
来源：http://qi.9csxet.cn

[U55] PHP：match 表达式
来源：http://vq.yuntaijiaju.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://im.huanxung.cn

[U56] PHP：命名参数
来源：http://nt.jianghongdianzi.cn

f(a: 1, b: 2)
来源：http://re.jianghongdianzi.cn

[U57] PHP：字符串插值
来源：http://jv.huixiangedu.cn

"值: {$a}"
来源：http://wq.colortex.cn

[U58] PHP：数组三件套
来源：http://tv.nszjky.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://sg.asd995.cn

[U59] PHP：自定义排序
来源：http://bk.nicolike.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cm.szxytkj.cn

[U60] PHP：JSON 编解码
来源：http://db.bjjhwx.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rm.bjjhwx.cn

[U61] PHP：正则
来源：http://by.nicolike.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gn.nicolike.cn

[U62] PHP：日期对象
来源：http://lb.huixiangedu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nf.chemitech.net.cn

[U63] PHP：文件读写
来源：http://yy.chemitech.net.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yi.shxzskj.cn

[U64] PHP：目录遍历
来源：http://us.muxihuayi.cn

glob("dir/*.php");  scandir("dir");
来源：http://vg.hnjuh.cn

[U65] PHP：会话
来源：http://sk.newstarts.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rg.muxihuayi.cn

[U66] PHP：设置 Cookie
来源：http://ay.bookmarksfly.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ko.521024.cn

[U67] PHP：处理文件上传
来源：http://nx.bookmarksfly.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hx.panjiajie.cn

[U68] PHP：PDO 连接
来源：http://lu.jctech888.com.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uz.gzmigu.cn

[U69] PHP：PDO 预处理
来源：http://to.nicolike.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fp.chemitech.net.cn

[U70] PHP：PDO 事务
来源：http://cm.huixiangedu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ct.colortex.cn

[U71] PHP：抛出异常
来源：http://ep.muxihuayi.cn

throw new RuntimeException("失败", 500);
来源：http://wq.bookmarksfly.cn

[U72] PHP：写错误日志
来源：http://bv.szsharing.cn

error_log("失败: " . $e->getMessage());
来源：http://gz.newstarts.cn

[U73] PHP：读取 ini 配置
来源：http://cl.chemitech.net.cn

parse_ini_file("config.ini", true)
来源：http://lt.szxytkj.cn

[U74] PHP：读取环境变量
来源：http://ps.nicolike.cn

getenv("APP_ENV") ?: "production"
来源：http://ax.szxytkj.cn

[U75] PHP：依赖注入
来源：http://kf.bookmarksfly.cn

composer require psr/container
来源：http://yc.9csxet.cn

[U76] PHP：简单路由
来源：http://ia.yuntaijiaju.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://py.huanxung.cn

[U77] PHP：模板渲染
来源：http://tc.bjjhwx.cn

composer require twig/twig
来源：http://hb.colortex.cn

[U78] PHP：单元测试
来源：http://gj.szsharing.cn

composer require --dev phpunit/phpunit
来源：http://iw.shxzukj.cn

[U79] PHP：静态分析
来源：http://id.nicolike.cn

composer require --dev phpstan/phpstan
来源：http://bn.newstarts.cn

[U80] PHP：代码规范修复
来源：http://vq.jianghongdianzi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://po.newstarts.cn

[U81] JS：初始化项目
来源：http://me.bjjhwx.cn

npm init -y;  npm i express
来源：http://jq.521024.cn

[U82] JS：package.json 脚本
来源：http://up.9csxet.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://eb.bjjhwx.cn

[U83] JS：ES Module 导入导出
来源：http://gy.huanxung.cn

export const a = 1;  import { a } from "./m.js";
来源：http://bj.asd995.cn

[U84] JS：CommonJS 写法
来源：http://xx.colortex.cn

module.exports = { a };  const { a } = require("./m");
来源：http://hv.shtwfgs.cn

[U85] JS：可选链
来源：http://hj.yuexingan06.cn

a?.b?.c
来源：http://or.gzmigu.cn

[U86] JS：空值合并
来源：http://yn.panjiajie.cn

a ?? b
来源：http://cs.shxzskj.cn

[U87] JS：解构默认值
来源：http://wj.asd995.cn

const { a = 1, b = 2 } = obj;
来源：http://mt.wgjwhj.cn

[U88] JS：对象展开合并
来源：http://qy.muxihuayi.cn

{ ...a, ...b }
来源：http://ru.asd995.cn

[U89] JS：数组去重
来源：http://px.hnjuh.cn

[...new Set(arr)]
来源：http://zc.bookmarksfly.cn

[U90] JS：数字数组排序
来源：http://yx.shxzskj.cn

[...arr].sort((a, b) => a - b)
来源：http://pm.shtwfgs.cn

[U91] JS：对象键值遍历
来源：http://pe.bjjhwx.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cq.521024.cn

[U92] JS：深拷贝
来源：http://ph.muxihuayi.cn

structuredClone(obj)
来源：http://dk.huixinmuqiang.cn

[U93] JS：模板字符串
来源：http://dx.jianghongdianzi.cn

`共 ${n} 条`
来源：http://ir.gzmigu.cn

[U94] JS：箭头函数
来源：http://yv.huanxung.cn

const double = x => x * 2;
来源：http://cr.nszjky.cn

[U95] JS：Promise 包装
来源：http://hc.521024.cn

new Promise((resolve, reject) => {})
来源：http://tn.panjiajie.cn

[U96] JS：async/await 与异常
来源：http://yk.szxytkj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rj.huixinmuqiang.cn

[U97] JS：并发请求
来源：http://ux.shxzskj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vl.nicolike.cn

[U98] JS：fetch 带 JSON
来源：http://tc.asd995.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zq.jianghongdianzi.cn

[U99] JS：事件监听
来源：http://fa.szsharing.cn

el.addEventListener("click", e => {})
来源：http://ap.bookmarksfly.cn

[U100] JS：DOM 查询
来源：http://hq.hnjuh.cn

document.querySelector(".item")
来源：http://dr.huixinmuqiang.cn

[U101] JS：classList 操作
来源：http://mo.9csxet.cn

el.classList.toggle("active")
来源：http://et.shxzukj.cn

[U102] JS：本地存储
来源：http://sr.szxytkj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://kc.szsharing.cn

[U103] JS：定时器
来源：http://ct.haigaiapp.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ww.huixiangedu.cn

[U104] JS：防抖
来源：http://vi.shxzukj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nz.hahajie.cn

[U105] JS：节流
来源：http://yx.szxytkj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lg.bookmarksfly.cn

[U106] JS：日期格式化
来源：http://ni.gzmigu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hf.wgjwhj.cn

[U107] JS：数字千分位
来源：http://zm.nszjky.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yh.muxihuayi.cn

[U108] JS：随机整数
来源：http://ei.chemitech.net.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pg.shxzukj.cn

[U109] JS：数组分组
来源：http://pf.521024.cn

Object.groupBy(arr, x => x.type)
来源：http://wc.huixinmuqiang.cn

[U110] JS：数组分块
来源：http://dg.asd995.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vf.huixinmuqiang.cn


<!-- 参考信息 -->