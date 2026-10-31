代发 wailian999

[T19] Swift：可选绑定
来源：http://yb.hnjuh.cn

if let n = opt { print(n) }
来源：http://ft.gzmigu.cn

[T20] Swift：数组操作
来源：http://ct.yuntaijiaju.cn

var a = [1, 2, 3];  a.append(4)
来源：http://at.huixiangedu.cn

[T21] Swift：遍历
来源：http://ym.newstarts.cn

for x in a { print(x) }
来源：http://qw.huanxung.cn

[T22] Swift：字典
来源：http://fo.jctech888.com.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ot.wgjwhj.cn

[T23] Swift：函数
来源：http://zl.shxzukj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://to.muxihuayi.cn

[T24] Swift：闭包
来源：http://mq.jctech888.com.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ap.hnjuh.cn

[T25] Swift：结构体
来源：http://wq.nszjky.cn

struct P { var x: Int }
来源：http://ab.szsharing.cn

[T26] Swift：类与重写
来源：http://fi.yuexingan06.cn

class A: Base { override func f() {} }
来源：http://bk.jctech888.com.cn

[T27] Swift：错误处理
来源：http://wz.chemitech.net.cn

do { try f() } catch { print(error) }
来源：http://nu.asd995.cn

[T28] Swift：枚举
来源：http://cp.521024.cn

enum Color { case red, green }
来源：http://zf.nszjky.cn

[T29] Swift：guard 提前返回
来源：http://db.haigaiapp.cn

guard let x = opt else { return }
来源：http://rp.haigaiapp.cn

[T30] Swift：协议
来源：http://zw.huanxung.cn

protocol Shape { func area() -> Double }
来源：http://qi.shtwfgs.cn

[T31] Lua：Hello World
来源：http://rc.asd995.cn

print("Hello")
来源：http://lr.nicolike.cn

[T32] Lua：局部变量
来源：http://sk.521024.cn

local a = 1
来源：http://yy.lnxyls.cn

[T33] Lua：表（数组）
来源：http://jv.yuntaijiaju.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://dy.muxihuayi.cn

[T34] Lua：遍历表
来源：http://ll.haigaiapp.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://uc.huixinmuqiang.cn

[T35] Lua：字典表
来源：http://st.nszjky.cn

local d = { a = 1 };  d.b = 2
来源：http://ae.jianghongdianzi.cn

[T36] Lua：函数
来源：http://xq.huanxung.cn

function add(a, b) return a + b end
来源：http://hv.chemitech.net.cn

[T37] Lua：字符串拼接
来源：http://hm.nicolike.cn

"a" .. "b"
来源：http://ut.szsharing.cn

[T38] Lua：条件
来源：http://rw.newstarts.cn

if x > 0 then print("正") end
来源：http://wh.szsharing.cn

[T39] Lua：模式匹配
来源：http://xs.jctech888.com.cn

string.find(s, "%d+")
来源：http://lz.jianghongdianzi.cn

[T40] Lua：元表
来源：http://qe.yuntaijiaju.cn

setmetatable({}, { __index = base })
来源：http://ed.panjiajie.cn

[T41] Perl：Hello World
来源：http://ej.gzmigu.cn

print "Hello\n";
来源：http://rw.huixinmuqiang.cn

[T42] Perl：变量类型
来源：http://cr.newstarts.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gr.jctech888.com.cn

[T43] Perl：字符串插值
来源：http://ku.muxihuayi.cn

"值: $a"
来源：http://ct.huanxung.cn

[T44] Perl：条件
来源：http://pk.jianghongdianzi.cn

if ($a > 0) { print "正"; }
来源：http://qv.newstarts.cn

[T45] Perl：数组遍历
来源：http://ow.521024.cn

for my $x (@arr) { print $x; }
来源：http://zr.chemitech.net.cn

[T46] Perl：哈希操作
来源：http://iv.colortex.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dq.huixiangedu.cn

[T47] Perl：正则捕获
来源：http://zo.bjjhwx.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://nr.asd995.cn

[T48] Perl：正则替换
来源：http://xi.chemitech.net.cn

$s =~ s/old/new/g;
来源：http://oq.9csxet.cn

[T49] Perl：函数
来源：http://fm.huanxung.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zo.szxytkj.cn

[T50] Perl：逐行读文件
来源：http://qg.lnxyls.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ob.huixiangedu.cn

while (my $line = <$fh>) { print $line; }
来源：http://ms.lnxyls.cn

[T51] Scala：Hello World
来源：http://ak.panjiajie.cn

println("Hello")
来源：http://so.hahajie.cn

[T52] Scala：变量
来源：http://gm.521024.cn

val a = 1;  var b = 2
来源：http://tc.yuntaijiaju.cn

[T53] Scala：字符串插值
来源：http://fk.nszjky.cn

s"值: $b"
来源：http://sp.gzmigu.cn

[T54] Scala：集合映射
来源：http://cl.9csxet.cn

List(1, 2, 3).map(_ * 2)
来源：http://wg.521024.cn

[T55] Scala：集合过滤
来源：http://lm.haigaiapp.cn

List(1, 2, 3).filter(_ > 1)
来源：http://oc.yuexingan06.cn

[T56] Scala：样例类
来源：http://ct.panjiajie.cn

case class User(name: String, age: Int)
来源：http://uu.haigaiapp.cn

[T57] Scala：模式匹配
来源：http://fj.shtwfgs.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://xo.wgjwhj.cn

[T58] Scala：函数定义
来源：http://pc.bjjhwx.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zy.nicolike.cn

[T59] Scala：循环
来源：http://in.shxzukj.cn

for (i <- 1 to 10) println(i)
来源：http://wf.haigaiapp.cn

[T60] Scala：折叠
来源：http://xf.asd995.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pj.hnjuh.cn

================================================================================
来源：http://dn.asd995.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ij.newstarts.cn

================================================================================
来源：http://gw.bjjhwx.cn

[U01] Py：创建虚拟环境
来源：http://he.jctech888.com.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qw.shtwfgs.cn

[U02] Py：导出 / 安装依赖
来源：http://pq.muxihuayi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qm.shxzukj.cn

[U03] Py：加载 .env 配置
来源：http://fp.huanxung.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://cv.bookmarksfly.cn

[U04] Py：变量调试打印
来源：http://hs.chemitech.net.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ny.szxytkj.cn

[U05] Py：列表去重且保序
来源：http://il.521024.cn

list(dict.fromkeys(arr))
来源：http://dq.asd995.cn

[U06] Py：合并两个字典
来源：http://ej.wgjwhj.cn

{**a, **b}
来源：http://mf.nszjky.cn

[U07] Py：反转字典键值
来源：http://kd.chemitech.net.cn

{v: k for k, v in d.items()}
来源：http://vk.shxzukj.cn

[U08] Py：展平二维列表
来源：http://se.huanxung.cn

[y for x in nested for y in x]
来源：http://jl.jianghongdianzi.cn

[U09] Py：字典取最大值的键
来源：http://ce.9csxet.cn

max(d, key=d.get)
来源：http://md.huanxung.cn

[U10] Py：按值排序字典
来源：http://tn.bookmarksfly.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jo.szsharing.cn

[U11] Py：生成器表达式
来源：http://nd.asd995.cn

(x * 2 for x in arr)
来源：http://cn.huanxung.cn

[U12] Py：取出现最多的 3 个元素
来源：http://er.lnxyls.cn

Counter(arr).most_common(3)
来源：http://yf.nszjky.cn

[U13] Py：固定长度队列
来源：http://af.9csxet.cn

deque(maxlen=10)
来源：http://cw.shxzukj.cn

[U14] Py：分组收集到列表
来源：http://lo.gzmigu.cn

defaultdict(list)
来源：http://zw.9csxet.cn

[U15] Py：高精度计时
来源：http://lz.muxihuayi.cn

t = time.perf_counter()
来源：http://xz.newstarts.cn

[U16] Py：命令行参数解析
来源：http://pb.huixiangedu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yr.9csxet.cn

[U17] Py：初始化日志
来源：http://vz.colortex.cn

logging.basicConfig(level=logging.INFO)
来源：http://ae.bjjhwx.cn

[U18] Py：预编译正则
来源：http://ko.muxihuayi.cn

pat = re.compile(r"\d+")
来源：http://bn.haigaiapp.cn

[U19] Py：正则替换带回调
来源：http://ak.huanxung.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pv.newstarts.cn

[U20] Py：缓存函数结果
来源：http://pq.huixiangedu.cn

@functools.lru_cache(maxsize=None)
来源：http://kj.bookmarksfly.cn

[U21] Py：自定义上下文管理器
来源：http://av.szxytkj.cn

@contextlib.contextmanager
来源：http://to.shxzukj.cn

[U22] Py：矩阵转置
来源：http://iw.bookmarksfly.cn

list(zip(*m))
来源：http://ll.yuntaijiaju.cn

[U23] Py：分块读取大文件
来源：http://qx.haigaiapp.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pe.huixiangedu.cn

[U24] Py：路径操作
来源：http://ky.chemitech.net.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://go.wgjwhj.cn

[U25] Py：CSV 按字典读
来源：http://bn.huanxung.cn

csv.DictReader(f)
来源：http://qv.jctech888.com.cn

[U26] Py：并发下载
来源：http://yt.shtwfgs.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mr.muxihuayi.cn

[U27] Py：异步 HTTP
来源：http://im.jianghongdianzi.cn

aiohttp.ClientSession() 配合 async with
来源：http://tj.hahajie.cn

[U28] Py：类型别名
来源：http://yb.lnxyls.cn

UserId = int
来源：http://mn.chemitech.net.cn

[U29] Py：属性校验
来源：http://yw.panjiajie.cn

@property 与 @x.setter 配合
来源：http://da.shxzskj.cn

[U30] Py：数据类
来源：http://lf.chemitech.net.cn

@dataclass(slots=True)
来源：http://fj.asd995.cn

[U31] Py：单测
来源：http://sf.colortex.cn

python -m pytest -q
来源：http://lm.gzmigu.cn

[U32] Py：代码格式化
来源：http://iy.shxzukj.cn

ruff format . && ruff check --fix .
来源：http://vi.gzmigu.cn

[U33] Py：打包发布
来源：http://mq.huixiangedu.cn

python -m build  （依赖 pyproject.toml）
来源：http://mo.shxzskj.cn

[U34] Py：判断编码
来源：http://im.nicolike.cn

chardet.detect(raw)
来源：http://bz.huixinmuqiang.cn

[U35] Py：发送邮件
来源：http://nv.huanxung.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zg.9csxet.cn

[U36] Py：定时任务
来源：http://dj.yuntaijiaju.cn

schedule.every(10).minutes.do(job)
来源：http://bw.szxytkj.cn

[U37] Py：读写 Excel
来源：http://nn.gzmigu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://kb.shxzukj.cn

[U38] Py：获取脚本所在目录
来源：http://za.hahajie.cn

Path(__file__).resolve().parent
来源：http://eb.lnxyls.cn

[U39] Py：判断是否在交互环境
来源：http://np.yuntaijiaju.cn

sys.stdout.isatty()
来源：http://mx.haigaiapp.cn

[U40] Py：打印到标准错误
来源：http://ax.shtwfgs.cn

print("err", file=sys.stderr)
来源：http://op.jctech888.com.cn

[U41] PHP：初始化 Composer 项目
来源：http://dd.lnxyls.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ta.szsharing.cn

[U42] PHP：PSR-4 自动加载
来源：http://rn.szsharing.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kw.shxzukj.cn

[U43] PHP：声明命名空间
来源：http://ny.szxytkj.cn

namespace App\Http;
来源：http://yc.wgjwhj.cn

[U44] PHP：开启严格类型
来源：http://qx.shtwfgs.cn

declare(strict_types=1);
来源：http://nm.521024.cn

[U45] PHP：类型声明与返回类型
来源：http://oh.shxzskj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://pl.gzmigu.cn

[U46] PHP：可空类型
来源：http://tg.gzmigu.cn

?string $name = null
来源：http://qo.shxzskj.cn

[U47] PHP：联合类型
来源：http://hn.hnjuh.cn

int|string $id
来源：http://fn.yuntaijiaju.cn

[U48] PHP：纯枚举
来源：http://kn.huixiangedu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fx.chemitech.net.cn

[U49] PHP：只读属性
来源：http://dy.chemitech.net.cn

public readonly string $name
来源：http://hm.bookmarksfly.cn

[U50] PHP：构造器属性提升
来源：http://xm.bookmarksfly.cn

public function __construct(private int $id) {}
来源：http://hd.newstarts.cn

[U51] PHP：数组解构
来源：http://yc.hnjuh.cn

[$a, $b] = $arr;
来源：http://ol.huanxung.cn

[U52] PHP：箭头函数
来源：http://op.521024.cn

$double = fn($x) => $x * 2;
来源：http://si.nszjky.cn

[U53] PHP：空合并运算符
来源：http://xk.yuntaijiaju.cn

$v = $a ?? $b ?? "default";
来源：http://zx.panjiajie.cn

[U54] PHP：空安全调用
来源：http://tz.shxzskj.cn

$obj?->method()
来源：http://ro.bookmarksfly.cn

[U55] PHP：match 表达式
来源：http://lu.wgjwhj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dn.jctech888.com.cn

[U56] PHP：命名参数
来源：http://ty.haigaiapp.cn

f(a: 1, b: 2)
来源：http://pn.yuexingan06.cn

[U57] PHP：字符串插值
来源：http://sp.shxzskj.cn

"值: {$a}"
来源：http://vj.gzmigu.cn

[U58] PHP：数组三件套
来源：http://mv.bjjhwx.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ac.panjiajie.cn

[U59] PHP：自定义排序
来源：http://rr.szxytkj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gl.nicolike.cn

[U60] PHP：JSON 编解码
来源：http://li.yuexingan06.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cq.huixinmuqiang.cn

[U61] PHP：正则
来源：http://vn.nicolike.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vx.gzmigu.cn

[U62] PHP：日期对象
来源：http://hv.shxzukj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bz.nicolike.cn

[U63] PHP：文件读写
来源：http://mv.nicolike.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mc.lnxyls.cn

[U64] PHP：目录遍历
来源：http://zw.gzmigu.cn

glob("dir/*.php");  scandir("dir");
来源：http://oh.huixiangedu.cn

[U65] PHP：会话
来源：http://kb.hahajie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://tv.lnxyls.cn

[U66] PHP：设置 Cookie
来源：http://gg.asd995.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ja.yuntaijiaju.cn

[U67] PHP：处理文件上传
来源：http://nm.panjiajie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vw.9csxet.cn

[U68] PHP：PDO 连接
来源：http://gt.huixinmuqiang.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nn.yuntaijiaju.cn

[U69] PHP：PDO 预处理
来源：http://ea.bjjhwx.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tx.lnxyls.cn

[U70] PHP：PDO 事务
来源：http://ks.colortex.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vj.jctech888.com.cn

[U71] PHP：抛出异常
来源：http://bu.hnjuh.cn

throw new RuntimeException("失败", 500);
来源：http://qk.jianghongdianzi.cn

[U72] PHP：写错误日志
来源：http://tw.szsharing.cn

error_log("失败: " . $e->getMessage());
来源：http://qx.jianghongdianzi.cn

[U73] PHP：读取 ini 配置
来源：http://zi.yuexingan06.cn

parse_ini_file("config.ini", true)
来源：http://xi.nszjky.cn

[U74] PHP：读取环境变量
来源：http://fh.bookmarksfly.cn

getenv("APP_ENV") ?: "production"
来源：http://ec.lnxyls.cn

[U75] PHP：依赖注入
来源：http://me.521024.cn

composer require psr/container
来源：http://cn.jianghongdianzi.cn

[U76] PHP：简单路由
来源：http://ia.huixinmuqiang.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ge.szxytkj.cn

[U77] PHP：模板渲染
来源：http://oo.bookmarksfly.cn

composer require twig/twig
来源：http://fh.9csxet.cn

[U78] PHP：单元测试
来源：http://wn.panjiajie.cn

composer require --dev phpunit/phpunit
来源：http://en.szxytkj.cn

[U79] PHP：静态分析
来源：http://gl.yuexingan06.cn

composer require --dev phpstan/phpstan
来源：http://rk.jianghongdianzi.cn

[U80] PHP：代码规范修复
来源：http://lg.shxzskj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://dr.shtwfgs.cn

[U81] JS：初始化项目
来源：http://gc.haigaiapp.cn

npm init -y;  npm i express
来源：http://ib.shtwfgs.cn

[U82] JS：package.json 脚本
来源：http://cq.muxihuayi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yf.haigaiapp.cn

[U83] JS：ES Module 导入导出
来源：http://ys.nszjky.cn

export const a = 1;  import { a } from "./m.js";
来源：http://nz.bjjhwx.cn

[U84] JS：CommonJS 写法
来源：http://em.huixinmuqiang.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ed.9csxet.cn

[U85] JS：可选链
来源：http://ww.bookmarksfly.cn

a?.b?.c
来源：http://rd.jianghongdianzi.cn

[U86] JS：空值合并
来源：http://wo.bookmarksfly.cn

a ?? b
来源：http://im.haigaiapp.cn

[U87] JS：解构默认值
来源：http://iw.lnxyls.cn

const { a = 1, b = 2 } = obj;
来源：http://sk.nszjky.cn

[U88] JS：对象展开合并
来源：http://nw.szsharing.cn

{ ...a, ...b }
来源：http://gp.jianghongdianzi.cn

[U89] JS：数组去重
来源：http://rv.colortex.cn

[...new Set(arr)]
来源：http://qv.newstarts.cn

[U90] JS：数字数组排序
来源：http://xe.hnjuh.cn

[...arr].sort((a, b) => a - b)
来源：http://pu.lnxyls.cn

[U91] JS：对象键值遍历
来源：http://rt.colortex.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vw.muxihuayi.cn

[U92] JS：深拷贝
来源：http://kk.huanxung.cn

structuredClone(obj)
来源：http://iq.newstarts.cn

[U93] JS：模板字符串
来源：http://la.bjjhwx.cn

`共 ${n} 条`
来源：http://ua.shtwfgs.cn

[U94] JS：箭头函数
来源：http://mg.shxzskj.cn

const double = x => x * 2;
来源：http://jn.hnjuh.cn

[U95] JS：Promise 包装
来源：http://bd.hnjuh.cn

new Promise((resolve, reject) => {})
来源：http://vm.shxzskj.cn

[U96] JS：async/await 与异常
来源：http://uk.asd995.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ye.shtwfgs.cn

[U97] JS：并发请求
来源：http://da.colortex.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://lj.wgjwhj.cn

[U98] JS：fetch 带 JSON
来源：http://ce.bookmarksfly.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://uz.shxzskj.cn

[U99] JS：事件监听
来源：http://rh.9csxet.cn

el.addEventListener("click", e => {})
来源：http://mt.bookmarksfly.cn

[U100] JS：DOM 查询
来源：http://sd.szxytkj.cn

document.querySelector(".item")
来源：http://es.jctech888.com.cn

[U101] JS：classList 操作
来源：http://un.szsharing.cn

el.classList.toggle("active")
来源：http://jw.wgjwhj.cn

[U102] JS：本地存储
来源：http://pq.chemitech.net.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ds.szxytkj.cn

[U103] JS：定时器
来源：http://ql.bookmarksfly.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://do.asd995.cn

[U104] JS：防抖
来源：http://ck.nszjky.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ay.nicolike.cn

[U105] JS：节流
来源：http://tb.colortex.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yt.nszjky.cn

[U106] JS：日期格式化
来源：http://rc.gzmigu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lf.nszjky.cn


<!-- 参考信息 -->