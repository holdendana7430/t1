代发 wailian999

[T21] Swift：遍历
来源：http://ku.shxzskj.cn

for x in a { print(x) }
来源：http://ds.nicolike.cn

[T22] Swift：字典
来源：http://ud.newstarts.cn

var d = ["a": 1];  d["b"] = 2
来源：http://st.jianghongdianzi.cn

[T23] Swift：函数
来源：http://sf.521024.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sl.bjjhwx.cn

[T24] Swift：闭包
来源：http://zr.chemitech.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://cp.newstarts.cn

[T25] Swift：结构体
来源：http://bx.shxzskj.cn

struct P { var x: Int }
来源：http://ku.jianghongdianzi.cn

[T26] Swift：类与重写
来源：http://ci.bjjhwx.cn

class A: Base { override func f() {} }
来源：http://uc.521024.cn

[T27] Swift：错误处理
来源：http://cx.huixinmuqiang.cn

do { try f() } catch { print(error) }
来源：http://vk.huanxung.cn

[T28] Swift：枚举
来源：http://xt.bookmarksfly.cn

enum Color { case red, green }
来源：http://fa.yuntaijiaju.cn

[T29] Swift：guard 提前返回
来源：http://ib.bjjhwx.cn

guard let x = opt else { return }
来源：http://oc.newstarts.cn

[T30] Swift：协议
来源：http://iu.szxytkj.cn

protocol Shape { func area() -> Double }
来源：http://jn.bjjhwx.cn

[T31] Lua：Hello World
来源：http://fc.shtwfgs.cn

print("Hello")
来源：http://zg.newstarts.cn

[T32] Lua：局部变量
来源：http://jx.bookmarksfly.cn

local a = 1
来源：http://fc.nszjky.cn

[T33] Lua：表（数组）
来源：http://or.nszjky.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zn.huixiangedu.cn

[T34] Lua：遍历表
来源：http://nw.colortex.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://cv.szxytkj.cn

[T35] Lua：字典表
来源：http://mi.asd995.cn

local d = { a = 1 };  d.b = 2
来源：http://qc.chemitech.net.cn

[T36] Lua：函数
来源：http://ip.lnxyls.cn

function add(a, b) return a + b end
来源：http://jf.newstarts.cn

[T37] Lua：字符串拼接
来源：http://nv.jianghongdianzi.cn

"a" .. "b"
来源：http://oy.nicolike.cn

[T38] Lua：条件
来源：http://se.huixinmuqiang.cn

if x > 0 then print("正") end
来源：http://og.chemitech.net.cn

[T39] Lua：模式匹配
来源：http://ti.huanxung.cn

string.find(s, "%d+")
来源：http://ln.panjiajie.cn

[T40] Lua：元表
来源：http://nt.shxzukj.cn

setmetatable({}, { __index = base })
来源：http://ur.nicolike.cn

[T41] Perl：Hello World
来源：http://jv.shxzskj.cn

print "Hello\n";
来源：http://qb.huixiangedu.cn

[T42] Perl：变量类型
来源：http://qi.yuntaijiaju.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bz.shtwfgs.cn

[T43] Perl：字符串插值
来源：http://vi.521024.cn

"值: $a"
来源：http://fz.huixinmuqiang.cn

[T44] Perl：条件
来源：http://es.jctech888.com.cn

if ($a > 0) { print "正"; }
来源：http://so.9csxet.cn

[T45] Perl：数组遍历
来源：http://ih.wgjwhj.cn

for my $x (@arr) { print $x; }
来源：http://hq.jctech888.com.cn

[T46] Perl：哈希操作
来源：http://iw.haigaiapp.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lv.wgjwhj.cn

[T47] Perl：正则捕获
来源：http://uc.shtwfgs.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://zm.bjjhwx.cn

[T48] Perl：正则替换
来源：http://ba.asd995.cn

$s =~ s/old/new/g;
来源：http://km.haigaiapp.cn

[T49] Perl：函数
来源：http://zm.huanxung.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lq.hahajie.cn

[T50] Perl：逐行读文件
来源：http://hj.lnxyls.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rd.yuexingan06.cn

while (my $line = <$fh>) { print $line; }
来源：http://hu.nicolike.cn

[T51] Scala：Hello World
来源：http://pw.chemitech.net.cn

println("Hello")
来源：http://lh.jctech888.com.cn

[T52] Scala：变量
来源：http://vl.huanxung.cn

val a = 1;  var b = 2
来源：http://vv.nicolike.cn

[T53] Scala：字符串插值
来源：http://nx.colortex.cn

s"值: $b"
来源：http://aj.yuntaijiaju.cn

[T54] Scala：集合映射
来源：http://ck.nicolike.cn

List(1, 2, 3).map(_ * 2)
来源：http://my.yuntaijiaju.cn

[T55] Scala：集合过滤
来源：http://ce.jianghongdianzi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ka.chemitech.net.cn

[T56] Scala：样例类
来源：http://kt.gzmigu.cn

case class User(name: String, age: Int)
来源：http://ez.szxytkj.cn

[T57] Scala：模式匹配
来源：http://wi.bjjhwx.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tr.yuexingan06.cn

[T58] Scala：函数定义
来源：http://lj.lnxyls.cn

def add(a: Int, b: Int): Int = a + b
来源：http://oa.hnjuh.cn

[T59] Scala：循环
来源：http://gi.bjjhwx.cn

for (i <- 1 to 10) println(i)
来源：http://rf.nicolike.cn

[T60] Scala：折叠
来源：http://ye.haigaiapp.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://uv.9csxet.cn

================================================================================
来源：http://et.asd995.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zq.lnxyls.cn

================================================================================
来源：http://cq.haigaiapp.cn

[U01] Py：创建虚拟环境
来源：http://gg.huixiangedu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://xn.nicolike.cn

[U02] Py：导出 / 安装依赖
来源：http://lb.bjjhwx.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xa.panjiajie.cn

[U03] Py：加载 .env 配置
来源：http://pq.shxzskj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://dp.shxzskj.cn

[U04] Py：变量调试打印
来源：http://cy.gzmigu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wa.chemitech.net.cn

[U05] Py：列表去重且保序
来源：http://hz.shtwfgs.cn

list(dict.fromkeys(arr))
来源：http://wh.hnjuh.cn

[U06] Py：合并两个字典
来源：http://fl.huixiangedu.cn

{**a, **b}
来源：http://db.jctech888.com.cn

[U07] Py：反转字典键值
来源：http://hw.haigaiapp.cn

{v: k for k, v in d.items()}
来源：http://au.nicolike.cn

[U08] Py：展平二维列表
来源：http://tv.szsharing.cn

[y for x in nested for y in x]
来源：http://ln.muxihuayi.cn

[U09] Py：字典取最大值的键
来源：http://ze.huixiangedu.cn

max(d, key=d.get)
来源：http://qs.nszjky.cn

[U10] Py：按值排序字典
来源：http://jm.szxytkj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pq.wgjwhj.cn

[U11] Py：生成器表达式
来源：http://zi.shtwfgs.cn

(x * 2 for x in arr)
来源：http://sd.wgjwhj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qd.szxytkj.cn

Counter(arr).most_common(3)
来源：http://ge.asd995.cn

[U13] Py：固定长度队列
来源：http://yw.hahajie.cn

deque(maxlen=10)
来源：http://ne.panjiajie.cn

[U14] Py：分组收集到列表
来源：http://nr.huixiangedu.cn

defaultdict(list)
来源：http://pc.jianghongdianzi.cn

[U15] Py：高精度计时
来源：http://fo.shtwfgs.cn

t = time.perf_counter()
来源：http://mv.yuexingan06.cn

[U16] Py：命令行参数解析
来源：http://or.huixinmuqiang.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nr.huixinmuqiang.cn

[U17] Py：初始化日志
来源：http://xa.jctech888.com.cn

logging.basicConfig(level=logging.INFO)
来源：http://fq.chemitech.net.cn

[U18] Py：预编译正则
来源：http://rd.chemitech.net.cn

pat = re.compile(r"\d+")
来源：http://sv.521024.cn

[U19] Py：正则替换带回调
来源：http://vk.nszjky.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://io.chemitech.net.cn

[U20] Py：缓存函数结果
来源：http://ys.hnjuh.cn

@functools.lru_cache(maxsize=None)
来源：http://zr.haigaiapp.cn

[U21] Py：自定义上下文管理器
来源：http://dv.nicolike.cn

@contextlib.contextmanager
来源：http://hz.shxzukj.cn

[U22] Py：矩阵转置
来源：http://um.lnxyls.cn

list(zip(*m))
来源：http://ky.huixinmuqiang.cn

[U23] Py：分块读取大文件
来源：http://cl.panjiajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://se.9csxet.cn

[U24] Py：路径操作
来源：http://na.jianghongdianzi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ry.521024.cn

[U25] Py：CSV 按字典读
来源：http://ib.panjiajie.cn

csv.DictReader(f)
来源：http://bd.huixinmuqiang.cn

[U26] Py：并发下载
来源：http://ga.hnjuh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cq.szxytkj.cn

[U27] Py：异步 HTTP
来源：http://dq.asd995.cn

aiohttp.ClientSession() 配合 async with
来源：http://ae.lnxyls.cn

[U28] Py：类型别名
来源：http://aq.bookmarksfly.cn

UserId = int
来源：http://ko.9csxet.cn

[U29] Py：属性校验
来源：http://nx.shtwfgs.cn

@property 与 @x.setter 配合
来源：http://pd.szsharing.cn

[U30] Py：数据类
来源：http://yp.nicolike.cn

@dataclass(slots=True)
来源：http://ok.muxihuayi.cn

[U31] Py：单测
来源：http://hq.shxzskj.cn

python -m pytest -q
来源：http://ed.newstarts.cn

[U32] Py：代码格式化
来源：http://hu.shxzukj.cn

ruff format . && ruff check --fix .
来源：http://ht.nicolike.cn

[U33] Py：打包发布
来源：http://hq.gzmigu.cn

python -m build  （依赖 pyproject.toml）
来源：http://hk.wgjwhj.cn

[U34] Py：判断编码
来源：http://nm.chemitech.net.cn

chardet.detect(raw)
来源：http://fu.jctech888.com.cn

[U35] Py：发送邮件
来源：http://oz.asd995.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bq.muxihuayi.cn

[U36] Py：定时任务
来源：http://ku.colortex.cn

schedule.every(10).minutes.do(job)
来源：http://ei.jianghongdianzi.cn

[U37] Py：读写 Excel
来源：http://zk.haigaiapp.cn

pandas.read_excel / DataFrame.to_excel
来源：http://bq.bookmarksfly.cn

[U38] Py：获取脚本所在目录
来源：http://oa.shxzskj.cn

Path(__file__).resolve().parent
来源：http://vx.muxihuayi.cn

[U39] Py：判断是否在交互环境
来源：http://hi.hnjuh.cn

sys.stdout.isatty()
来源：http://kq.bjjhwx.cn

[U40] Py：打印到标准错误
来源：http://ct.bookmarksfly.cn

print("err", file=sys.stderr)
来源：http://ep.jctech888.com.cn

[U41] PHP：初始化 Composer 项目
来源：http://sv.yuntaijiaju.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jx.jianghongdianzi.cn

[U42] PHP：PSR-4 自动加载
来源：http://vj.shxzskj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dv.huixiangedu.cn

[U43] PHP：声明命名空间
来源：http://xr.nszjky.cn

namespace App\Http;
来源：http://mf.colortex.cn

[U44] PHP：开启严格类型
来源：http://kg.asd995.cn

declare(strict_types=1);
来源：http://xh.521024.cn

[U45] PHP：类型声明与返回类型
来源：http://jt.haigaiapp.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://gt.gzmigu.cn

[U46] PHP：可空类型
来源：http://oe.shxzskj.cn

?string $name = null
来源：http://ix.lnxyls.cn

[U47] PHP：联合类型
来源：http://vu.9csxet.cn

int|string $id
来源：http://nj.haigaiapp.cn

[U48] PHP：纯枚举
来源：http://ve.haigaiapp.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://oz.hnjuh.cn

[U49] PHP：只读属性
来源：http://xy.colortex.cn

public readonly string $name
来源：http://pe.bjjhwx.cn

[U50] PHP：构造器属性提升
来源：http://fv.jianghongdianzi.cn

public function __construct(private int $id) {}
来源：http://as.hnjuh.cn

[U51] PHP：数组解构
来源：http://ac.bjjhwx.cn

[$a, $b] = $arr;
来源：http://eh.wgjwhj.cn

[U52] PHP：箭头函数
来源：http://ao.huixiangedu.cn

$double = fn($x) => $x * 2;
来源：http://gf.jctech888.com.cn

[U53] PHP：空合并运算符
来源：http://rx.panjiajie.cn

$v = $a ?? $b ?? "default";
来源：http://mt.521024.cn

[U54] PHP：空安全调用
来源：http://ku.szxytkj.cn

$obj?->method()
来源：http://lt.nszjky.cn

[U55] PHP：match 表达式
来源：http://ff.panjiajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wa.yuexingan06.cn

[U56] PHP：命名参数
来源：http://gv.jianghongdianzi.cn

f(a: 1, b: 2)
来源：http://ju.newstarts.cn

[U57] PHP：字符串插值
来源：http://jb.nszjky.cn

"值: {$a}"
来源：http://hl.muxihuayi.cn

[U58] PHP：数组三件套
来源：http://ei.shxzukj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vl.hnjuh.cn

[U59] PHP：自定义排序
来源：http://ks.hnjuh.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://er.szxytkj.cn

[U60] PHP：JSON 编解码
来源：http://wp.newstarts.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pv.nicolike.cn

[U61] PHP：正则
来源：http://zu.bjjhwx.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vw.colortex.cn

[U62] PHP：日期对象
来源：http://ow.huixiangedu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://oq.haigaiapp.cn

[U63] PHP：文件读写
来源：http://va.jctech888.com.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ka.muxihuayi.cn

[U64] PHP：目录遍历
来源：http://we.shtwfgs.cn

glob("dir/*.php");  scandir("dir");
来源：http://nh.bjjhwx.cn

[U65] PHP：会话
来源：http://nw.huanxung.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://jt.nicolike.cn

[U66] PHP：设置 Cookie
来源：http://xw.bookmarksfly.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://md.gzmigu.cn

[U67] PHP：处理文件上传
来源：http://dh.521024.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://by.9csxet.cn

[U68] PHP：PDO 连接
来源：http://jm.huanxung.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jj.hahajie.cn

[U69] PHP：PDO 预处理
来源：http://tx.asd995.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://im.nicolike.cn

[U70] PHP：PDO 事务
来源：http://tq.9csxet.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wq.newstarts.cn

[U71] PHP：抛出异常
来源：http://rh.521024.cn

throw new RuntimeException("失败", 500);
来源：http://fl.shtwfgs.cn

[U72] PHP：写错误日志
来源：http://qn.hahajie.cn

error_log("失败: " . $e->getMessage());
来源：http://cw.chemitech.net.cn

[U73] PHP：读取 ini 配置
来源：http://ds.yuexingan06.cn

parse_ini_file("config.ini", true)
来源：http://zt.yuntaijiaju.cn

[U74] PHP：读取环境变量
来源：http://nd.shxzskj.cn

getenv("APP_ENV") ?: "production"
来源：http://gk.yuexingan06.cn

[U75] PHP：依赖注入
来源：http://wi.521024.cn

composer require psr/container
来源：http://pp.chemitech.net.cn

[U76] PHP：简单路由
来源：http://wk.huanxung.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ne.shxzskj.cn

[U77] PHP：模板渲染
来源：http://pn.newstarts.cn

composer require twig/twig
来源：http://je.huanxung.cn

[U78] PHP：单元测试
来源：http://et.haigaiapp.cn

composer require --dev phpunit/phpunit
来源：http://xx.huixinmuqiang.cn

[U79] PHP：静态分析
来源：http://xl.shtwfgs.cn

composer require --dev phpstan/phpstan
来源：http://vd.521024.cn

[U80] PHP：代码规范修复
来源：http://to.gzmigu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://wp.shxzukj.cn

[U81] JS：初始化项目
来源：http://ov.9csxet.cn

npm init -y;  npm i express
来源：http://xd.haigaiapp.cn

[U82] JS：package.json 脚本
来源：http://lj.lnxyls.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bv.huanxung.cn

[U83] JS：ES Module 导入导出
来源：http://ku.jianghongdianzi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ib.lnxyls.cn

[U84] JS：CommonJS 写法
来源：http://cu.lnxyls.cn

module.exports = { a };  const { a } = require("./m");
来源：http://kx.shxzskj.cn

[U85] JS：可选链
来源：http://yj.huixinmuqiang.cn

a?.b?.c
来源：http://jy.shxzskj.cn

[U86] JS：空值合并
来源：http://gc.gzmigu.cn

a ?? b
来源：http://lt.colortex.cn

[U87] JS：解构默认值
来源：http://vm.nszjky.cn

const { a = 1, b = 2 } = obj;
来源：http://af.lnxyls.cn

[U88] JS：对象展开合并
来源：http://eu.hnjuh.cn

{ ...a, ...b }
来源：http://wn.chemitech.net.cn

[U89] JS：数组去重
来源：http://iz.newstarts.cn

[...new Set(arr)]
来源：http://fh.hahajie.cn

[U90] JS：数字数组排序
来源：http://kp.bookmarksfly.cn

[...arr].sort((a, b) => a - b)
来源：http://vh.shxzskj.cn

[U91] JS：对象键值遍历
来源：http://tw.newstarts.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lb.hnjuh.cn

[U92] JS：深拷贝
来源：http://ov.huixinmuqiang.cn

structuredClone(obj)
来源：http://wq.lnxyls.cn

[U93] JS：模板字符串
来源：http://nv.yuntaijiaju.cn

`共 ${n} 条`
来源：http://no.muxihuayi.cn

[U94] JS：箭头函数
来源：http://vc.shtwfgs.cn

const double = x => x * 2;
来源：http://ru.haigaiapp.cn

[U95] JS：Promise 包装
来源：http://gh.panjiajie.cn

new Promise((resolve, reject) => {})
来源：http://kf.huixinmuqiang.cn

[U96] JS：async/await 与异常
来源：http://uw.newstarts.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vw.panjiajie.cn

[U97] JS：并发请求
来源：http://xq.panjiajie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qj.hnjuh.cn

[U98] JS：fetch 带 JSON
来源：http://lj.newstarts.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vx.szsharing.cn

[U99] JS：事件监听
来源：http://il.yuexingan06.cn

el.addEventListener("click", e => {})
来源：http://dd.huixiangedu.cn

[U100] JS：DOM 查询
来源：http://xy.jctech888.com.cn

document.querySelector(".item")
来源：http://tb.huixinmuqiang.cn

[U101] JS：classList 操作
来源：http://qj.gzmigu.cn

el.classList.toggle("active")
来源：http://ol.huixinmuqiang.cn

[U102] JS：本地存储
来源：http://tn.bookmarksfly.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ue.gzmigu.cn

[U103] JS：定时器
来源：http://dc.lnxyls.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dn.colortex.cn

[U104] JS：防抖
来源：http://jv.hahajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ak.panjiajie.cn

[U105] JS：节流
来源：http://xe.shxzukj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wz.colortex.cn

[U106] JS：日期格式化
来源：http://ss.huixinmuqiang.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://np.colortex.cn

[U107] JS：数字千分位
来源：http://yc.wgjwhj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ht.521024.cn

[U108] JS：随机整数
来源：http://qu.muxihuayi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wa.bjjhwx.cn


<!-- 参考信息 -->