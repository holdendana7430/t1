代发 wailian999

[T21] Swift：遍历
来源：http://wd.nszjky.cn

for x in a { print(x) }
来源：http://mv.haigaiapp.cn

[T22] Swift：字典
来源：http://uc.521024.cn

var d = ["a": 1];  d["b"] = 2
来源：http://lz.wgjwhj.cn

[T23] Swift：函数
来源：http://nc.9csxet.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://za.9csxet.cn

[T24] Swift：闭包
来源：http://fj.jianghongdianzi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ol.hnjuh.cn

[T25] Swift：结构体
来源：http://tr.szsharing.cn

struct P { var x: Int }
来源：http://nn.huixiangedu.cn

[T26] Swift：类与重写
来源：http://cy.muxihuayi.cn

class A: Base { override func f() {} }
来源：http://um.yuntaijiaju.cn

[T27] Swift：错误处理
来源：http://dt.bjjhwx.cn

do { try f() } catch { print(error) }
来源：http://bx.huixinmuqiang.cn

[T28] Swift：枚举
来源：http://ka.haigaiapp.cn

enum Color { case red, green }
来源：http://rr.huanxung.cn

[T29] Swift：guard 提前返回
来源：http://zq.szxytkj.cn

guard let x = opt else { return }
来源：http://rb.shtwfgs.cn

[T30] Swift：协议
来源：http://jo.lnxyls.cn

protocol Shape { func area() -> Double }
来源：http://es.szxytkj.cn

[T31] Lua：Hello World
来源：http://ke.hnjuh.cn

print("Hello")
来源：http://re.newstarts.cn

[T32] Lua：局部变量
来源：http://bg.szxytkj.cn

local a = 1
来源：http://vt.huixinmuqiang.cn

[T33] Lua：表（数组）
来源：http://eq.gzmigu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://em.yuntaijiaju.cn

[T34] Lua：遍历表
来源：http://qg.panjiajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://pe.9csxet.cn

[T35] Lua：字典表
来源：http://oh.yuexingan06.cn

local d = { a = 1 };  d.b = 2
来源：http://cc.huixiangedu.cn

[T36] Lua：函数
来源：http://ch.shxzukj.cn

function add(a, b) return a + b end
来源：http://yo.jianghongdianzi.cn

[T37] Lua：字符串拼接
来源：http://vv.gzmigu.cn

"a" .. "b"
来源：http://oa.shxzukj.cn

[T38] Lua：条件
来源：http://ia.shtwfgs.cn

if x > 0 then print("正") end
来源：http://xa.huixinmuqiang.cn

[T39] Lua：模式匹配
来源：http://ga.huixiangedu.cn

string.find(s, "%d+")
来源：http://je.huixinmuqiang.cn

[T40] Lua：元表
来源：http://zt.huanxung.cn

setmetatable({}, { __index = base })
来源：http://jf.shxzskj.cn

[T41] Perl：Hello World
来源：http://qr.huanxung.cn

print "Hello\n";
来源：http://dh.gzmigu.cn

[T42] Perl：变量类型
来源：http://bn.jianghongdianzi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://se.bjjhwx.cn

[T43] Perl：字符串插值
来源：http://wq.hnjuh.cn

"值: $a"
来源：http://lc.lnxyls.cn

[T44] Perl：条件
来源：http://ob.huanxung.cn

if ($a > 0) { print "正"; }
来源：http://qm.szxytkj.cn

[T45] Perl：数组遍历
来源：http://ne.yuntaijiaju.cn

for my $x (@arr) { print $x; }
来源：http://rt.szsharing.cn

[T46] Perl：哈希操作
来源：http://jk.panjiajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nc.yuexingan06.cn

[T47] Perl：正则捕获
来源：http://uu.shxzskj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://cv.chemitech.net.cn

[T48] Perl：正则替换
来源：http://sc.yuexingan06.cn

$s =~ s/old/new/g;
来源：http://ql.asd995.cn

[T49] Perl：函数
来源：http://uh.szsharing.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://du.hnjuh.cn

[T50] Perl：逐行读文件
来源：http://hw.panjiajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://sp.hahajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://eo.shtwfgs.cn

[T51] Scala：Hello World
来源：http://ov.huixinmuqiang.cn

println("Hello")
来源：http://dl.colortex.cn

[T52] Scala：变量
来源：http://nr.huixinmuqiang.cn

val a = 1;  var b = 2
来源：http://ff.shxzukj.cn

[T53] Scala：字符串插值
来源：http://fx.huixiangedu.cn

s"值: $b"
来源：http://kt.asd995.cn

[T54] Scala：集合映射
来源：http://bv.shxzskj.cn

List(1, 2, 3).map(_ * 2)
来源：http://xy.szxytkj.cn

[T55] Scala：集合过滤
来源：http://jj.shtwfgs.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xt.newstarts.cn

[T56] Scala：样例类
来源：http://es.haigaiapp.cn

case class User(name: String, age: Int)
来源：http://rr.huixiangedu.cn

[T57] Scala：模式匹配
来源：http://po.muxihuayi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wv.panjiajie.cn

[T58] Scala：函数定义
来源：http://hb.huixiangedu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ry.huanxung.cn

[T59] Scala：循环
来源：http://qt.bjjhwx.cn

for (i <- 1 to 10) println(i)
来源：http://rb.shtwfgs.cn

[T60] Scala：折叠
来源：http://xq.muxihuayi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dc.szxytkj.cn

================================================================================
来源：http://hx.newstarts.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ym.shtwfgs.cn

================================================================================
来源：http://qm.muxihuayi.cn

[U01] Py：创建虚拟环境
来源：http://ud.huixinmuqiang.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qb.bookmarksfly.cn

[U02] Py：导出 / 安装依赖
来源：http://rb.szxytkj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ya.muxihuayi.cn

[U03] Py：加载 .env 配置
来源：http://fn.yuntaijiaju.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://vx.huixiangedu.cn

[U04] Py：变量调试打印
来源：http://mp.nszjky.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zi.jianghongdianzi.cn

[U05] Py：列表去重且保序
来源：http://yb.huixiangedu.cn

list(dict.fromkeys(arr))
来源：http://si.shtwfgs.cn

[U06] Py：合并两个字典
来源：http://fc.huanxung.cn

{**a, **b}
来源：http://ck.chemitech.net.cn

[U07] Py：反转字典键值
来源：http://ie.haigaiapp.cn

{v: k for k, v in d.items()}
来源：http://kq.9csxet.cn

[U08] Py：展平二维列表
来源：http://jb.colortex.cn

[y for x in nested for y in x]
来源：http://io.521024.cn

[U09] Py：字典取最大值的键
来源：http://ut.9csxet.cn

max(d, key=d.get)
来源：http://dr.nszjky.cn

[U10] Py：按值排序字典
来源：http://wx.shxzukj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bq.chemitech.net.cn

[U11] Py：生成器表达式
来源：http://ti.521024.cn

(x * 2 for x in arr)
来源：http://rp.shxzukj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ll.yuntaijiaju.cn

Counter(arr).most_common(3)
来源：http://md.panjiajie.cn

[U13] Py：固定长度队列
来源：http://ww.newstarts.cn

deque(maxlen=10)
来源：http://ef.huanxung.cn

[U14] Py：分组收集到列表
来源：http://cl.yuntaijiaju.cn

defaultdict(list)
来源：http://nz.colortex.cn

[U15] Py：高精度计时
来源：http://uv.asd995.cn

t = time.perf_counter()
来源：http://pn.haigaiapp.cn

[U16] Py：命令行参数解析
来源：http://qz.yuexingan06.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hg.hahajie.cn

[U17] Py：初始化日志
来源：http://yf.huanxung.cn

logging.basicConfig(level=logging.INFO)
来源：http://rf.bjjhwx.cn

[U18] Py：预编译正则
来源：http://eo.huixinmuqiang.cn

pat = re.compile(r"\d+")
来源：http://yx.lnxyls.cn

[U19] Py：正则替换带回调
来源：http://pc.wgjwhj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rn.colortex.cn

[U20] Py：缓存函数结果
来源：http://le.shtwfgs.cn

@functools.lru_cache(maxsize=None)
来源：http://sn.gzmigu.cn

[U21] Py：自定义上下文管理器
来源：http://ed.jianghongdianzi.cn

@contextlib.contextmanager
来源：http://ax.colortex.cn

[U22] Py：矩阵转置
来源：http://hi.muxihuayi.cn

list(zip(*m))
来源：http://zf.jctech888.com.cn

[U23] Py：分块读取大文件
来源：http://eu.asd995.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qz.jctech888.com.cn

[U24] Py：路径操作
来源：http://ts.gzmigu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yv.huixiangedu.cn

[U25] Py：CSV 按字典读
来源：http://wp.bjjhwx.cn

csv.DictReader(f)
来源：http://nn.muxihuayi.cn

[U26] Py：并发下载
来源：http://ja.shxzskj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mx.jctech888.com.cn

[U27] Py：异步 HTTP
来源：http://si.gzmigu.cn

aiohttp.ClientSession() 配合 async with
来源：http://kz.panjiajie.cn

[U28] Py：类型别名
来源：http://iq.huixinmuqiang.cn

UserId = int
来源：http://tv.9csxet.cn

[U29] Py：属性校验
来源：http://hw.shtwfgs.cn

@property 与 @x.setter 配合
来源：http://fz.bjjhwx.cn

[U30] Py：数据类
来源：http://pb.lnxyls.cn

@dataclass(slots=True)
来源：http://ef.gzmigu.cn

[U31] Py：单测
来源：http://kn.shtwfgs.cn

python -m pytest -q
来源：http://xb.szxytkj.cn

[U32] Py：代码格式化
来源：http://zj.newstarts.cn

ruff format . && ruff check --fix .
来源：http://vr.yuntaijiaju.cn

[U33] Py：打包发布
来源：http://ae.colortex.cn

python -m build  （依赖 pyproject.toml）
来源：http://et.521024.cn

[U34] Py：判断编码
来源：http://zd.jianghongdianzi.cn

chardet.detect(raw)
来源：http://ik.newstarts.cn

[U35] Py：发送邮件
来源：http://bk.huixiangedu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://on.nszjky.cn

[U36] Py：定时任务
来源：http://nn.szxytkj.cn

schedule.every(10).minutes.do(job)
来源：http://it.muxihuayi.cn

[U37] Py：读写 Excel
来源：http://gh.521024.cn

pandas.read_excel / DataFrame.to_excel
来源：http://lc.huanxung.cn

[U38] Py：获取脚本所在目录
来源：http://pw.9csxet.cn

Path(__file__).resolve().parent
来源：http://of.szxytkj.cn

[U39] Py：判断是否在交互环境
来源：http://ch.haigaiapp.cn

sys.stdout.isatty()
来源：http://bg.colortex.cn

[U40] Py：打印到标准错误
来源：http://vw.wgjwhj.cn

print("err", file=sys.stderr)
来源：http://bt.hahajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://rd.newstarts.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qy.hnjuh.cn

[U42] PHP：PSR-4 自动加载
来源：http://mk.hnjuh.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wh.szsharing.cn

[U43] PHP：声明命名空间
来源：http://qp.muxihuayi.cn

namespace App\Http;
来源：http://fk.chemitech.net.cn

[U44] PHP：开启严格类型
来源：http://wp.shxzukj.cn

declare(strict_types=1);
来源：http://ku.bookmarksfly.cn

[U45] PHP：类型声明与返回类型
来源：http://ld.jianghongdianzi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://rt.shtwfgs.cn

[U46] PHP：可空类型
来源：http://jm.jianghongdianzi.cn

?string $name = null
来源：http://we.haigaiapp.cn

[U47] PHP：联合类型
来源：http://xt.jctech888.com.cn

int|string $id
来源：http://ty.hahajie.cn

[U48] PHP：纯枚举
来源：http://tm.muxihuayi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://az.shxzukj.cn

[U49] PHP：只读属性
来源：http://ti.jctech888.com.cn

public readonly string $name
来源：http://yd.haigaiapp.cn

[U50] PHP：构造器属性提升
来源：http://io.shxzskj.cn

public function __construct(private int $id) {}
来源：http://ia.lnxyls.cn

[U51] PHP：数组解构
来源：http://qq.huixiangedu.cn

[$a, $b] = $arr;
来源：http://zo.colortex.cn

[U52] PHP：箭头函数
来源：http://ez.newstarts.cn

$double = fn($x) => $x * 2;
来源：http://fm.muxihuayi.cn

[U53] PHP：空合并运算符
来源：http://au.huanxung.cn

$v = $a ?? $b ?? "default";
来源：http://kf.9csxet.cn

[U54] PHP：空安全调用
来源：http://qf.9csxet.cn

$obj?->method()
来源：http://om.szsharing.cn

[U55] PHP：match 表达式
来源：http://na.shtwfgs.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://um.szxytkj.cn

[U56] PHP：命名参数
来源：http://dv.chemitech.net.cn

f(a: 1, b: 2)
来源：http://as.lnxyls.cn

[U57] PHP：字符串插值
来源：http://eg.muxihuayi.cn

"值: {$a}"
来源：http://nc.bjjhwx.cn

[U58] PHP：数组三件套
来源：http://ye.shtwfgs.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wc.colortex.cn

[U59] PHP：自定义排序
来源：http://ds.lnxyls.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jo.huanxung.cn

[U60] PHP：JSON 编解码
来源：http://zk.gzmigu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xd.shtwfgs.cn

[U61] PHP：正则
来源：http://tz.muxihuayi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://af.nszjky.cn

[U62] PHP：日期对象
来源：http://au.nszjky.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://je.colortex.cn

[U63] PHP：文件读写
来源：http://ae.szxytkj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qb.hnjuh.cn

[U64] PHP：目录遍历
来源：http://zk.chemitech.net.cn

glob("dir/*.php");  scandir("dir");
来源：http://cy.nicolike.cn

[U65] PHP：会话
来源：http://gm.shxzukj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://nx.huanxung.cn

[U66] PHP：设置 Cookie
来源：http://pz.szxytkj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fu.yuntaijiaju.cn

[U67] PHP：处理文件上传
来源：http://vl.asd995.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jy.shxzukj.cn

[U68] PHP：PDO 连接
来源：http://so.panjiajie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gr.haigaiapp.cn

[U69] PHP：PDO 预处理
来源：http://db.huixiangedu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fj.gzmigu.cn

[U70] PHP：PDO 事务
来源：http://ye.huanxung.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qp.shxzukj.cn

[U71] PHP：抛出异常
来源：http://za.hahajie.cn

throw new RuntimeException("失败", 500);
来源：http://hp.newstarts.cn

[U72] PHP：写错误日志
来源：http://ks.bookmarksfly.cn

error_log("失败: " . $e->getMessage());
来源：http://wn.jctech888.com.cn

[U73] PHP：读取 ini 配置
来源：http://uj.newstarts.cn

parse_ini_file("config.ini", true)
来源：http://wk.jianghongdianzi.cn

[U74] PHP：读取环境变量
来源：http://qw.newstarts.cn

getenv("APP_ENV") ?: "production"
来源：http://cv.hahajie.cn

[U75] PHP：依赖注入
来源：http://qw.huixinmuqiang.cn

composer require psr/container
来源：http://xw.yuexingan06.cn

[U76] PHP：简单路由
来源：http://bi.lnxyls.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yz.yuexingan06.cn

[U77] PHP：模板渲染
来源：http://ba.521024.cn

composer require twig/twig
来源：http://nu.chemitech.net.cn

[U78] PHP：单元测试
来源：http://if.521024.cn

composer require --dev phpunit/phpunit
来源：http://gt.szxytkj.cn

[U79] PHP：静态分析
来源：http://go.huixinmuqiang.cn

composer require --dev phpstan/phpstan
来源：http://ch.yuexingan06.cn

[U80] PHP：代码规范修复
来源：http://ea.szsharing.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ki.newstarts.cn

[U81] JS：初始化项目
来源：http://mo.shxzskj.cn

npm init -y;  npm i express
来源：http://qq.9csxet.cn

[U82] JS：package.json 脚本
来源：http://tj.jctech888.com.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ss.hnjuh.cn

[U83] JS：ES Module 导入导出
来源：http://xh.nszjky.cn

export const a = 1;  import { a } from "./m.js";
来源：http://fi.asd995.cn

[U84] JS：CommonJS 写法
来源：http://gr.shxzukj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://pr.newstarts.cn

[U85] JS：可选链
来源：http://xv.haigaiapp.cn

a?.b?.c
来源：http://ws.szsharing.cn

[U86] JS：空值合并
来源：http://mr.yuntaijiaju.cn

a ?? b
来源：http://rp.nszjky.cn

[U87] JS：解构默认值
来源：http://js.hnjuh.cn

const { a = 1, b = 2 } = obj;
来源：http://tf.huixiangedu.cn

[U88] JS：对象展开合并
来源：http://fu.asd995.cn

{ ...a, ...b }
来源：http://fl.yuexingan06.cn

[U89] JS：数组去重
来源：http://yb.asd995.cn

[...new Set(arr)]
来源：http://qt.colortex.cn

[U90] JS：数字数组排序
来源：http://tz.yuexingan06.cn

[...arr].sort((a, b) => a - b)
来源：http://ju.bookmarksfly.cn

[U91] JS：对象键值遍历
来源：http://dw.huixiangedu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qe.szxytkj.cn

[U92] JS：深拷贝
来源：http://mf.hnjuh.cn

structuredClone(obj)
来源：http://sn.wgjwhj.cn

[U93] JS：模板字符串
来源：http://ya.szxytkj.cn

`共 ${n} 条`
来源：http://bx.yuexingan06.cn

[U94] JS：箭头函数
来源：http://tx.chemitech.net.cn

const double = x => x * 2;
来源：http://bf.hahajie.cn

[U95] JS：Promise 包装
来源：http://km.lnxyls.cn

new Promise((resolve, reject) => {})
来源：http://sw.asd995.cn

[U96] JS：async/await 与异常
来源：http://bu.chemitech.net.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ou.gzmigu.cn

[U97] JS：并发请求
来源：http://ie.huixiangedu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://km.jianghongdianzi.cn

[U98] JS：fetch 带 JSON
来源：http://yo.panjiajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ws.panjiajie.cn

[U99] JS：事件监听
来源：http://nz.shxzukj.cn

el.addEventListener("click", e => {})
来源：http://uq.gzmigu.cn

[U100] JS：DOM 查询
来源：http://rv.newstarts.cn

document.querySelector(".item")
来源：http://tv.gzmigu.cn

[U101] JS：classList 操作
来源：http://cs.haigaiapp.cn

el.classList.toggle("active")
来源：http://dj.521024.cn

[U102] JS：本地存储
来源：http://ud.shxzukj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://zs.lnxyls.cn

[U103] JS：定时器
来源：http://xu.jianghongdianzi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://so.shtwfgs.cn

[U104] JS：防抖
来源：http://yn.huanxung.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fa.gzmigu.cn

[U105] JS：节流
来源：http://tf.jctech888.com.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qw.shxzskj.cn

[U106] JS：日期格式化
来源：http://ah.asd995.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rp.nszjky.cn

[U107] JS：数字千分位
来源：http://cs.lnxyls.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ws.newstarts.cn

[U108] JS：随机整数
来源：http://oc.lnxyls.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jf.jctech888.com.cn


<!-- 参考信息 -->