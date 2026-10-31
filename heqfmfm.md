代发 wailian999

[T21] Swift：遍历
来源：http://le.huixiangedu.cn

for x in a { print(x) }
来源：http://ru.colortex.cn

[T22] Swift：字典
来源：http://cb.colortex.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vp.gzmigu.cn

[T23] Swift：函数
来源：http://pi.asd995.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bu.chemitech.net.cn

[T24] Swift：闭包
来源：http://yj.jianghongdianzi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vc.yuntaijiaju.cn

[T25] Swift：结构体
来源：http://rk.521024.cn

struct P { var x: Int }
来源：http://yj.asd995.cn

[T26] Swift：类与重写
来源：http://ot.lnxyls.cn

class A: Base { override func f() {} }
来源：http://lc.huixiangedu.cn

[T27] Swift：错误处理
来源：http://ly.asd995.cn

do { try f() } catch { print(error) }
来源：http://vt.jianghongdianzi.cn

[T28] Swift：枚举
来源：http://vy.wgjwhj.cn

enum Color { case red, green }
来源：http://bp.jctech888.com.cn

[T29] Swift：guard 提前返回
来源：http://sd.521024.cn

guard let x = opt else { return }
来源：http://qn.asd995.cn

[T30] Swift：协议
来源：http://ji.muxihuayi.cn

protocol Shape { func area() -> Double }
来源：http://id.szxytkj.cn

[T31] Lua：Hello World
来源：http://xc.nicolike.cn

print("Hello")
来源：http://ij.huixinmuqiang.cn

[T32] Lua：局部变量
来源：http://xg.shxzukj.cn

local a = 1
来源：http://kh.szsharing.cn

[T33] Lua：表（数组）
来源：http://qy.hahajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://yv.chemitech.net.cn

[T34] Lua：遍历表
来源：http://kk.yuexingan06.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://mf.chemitech.net.cn

[T35] Lua：字典表
来源：http://he.haigaiapp.cn

local d = { a = 1 };  d.b = 2
来源：http://xi.jianghongdianzi.cn

[T36] Lua：函数
来源：http://io.wgjwhj.cn

function add(a, b) return a + b end
来源：http://nm.bookmarksfly.cn

[T37] Lua：字符串拼接
来源：http://ro.huixinmuqiang.cn

"a" .. "b"
来源：http://es.521024.cn

[T38] Lua：条件
来源：http://on.shtwfgs.cn

if x > 0 then print("正") end
来源：http://zd.szxytkj.cn

[T39] Lua：模式匹配
来源：http://xt.hnjuh.cn

string.find(s, "%d+")
来源：http://kx.yuntaijiaju.cn

[T40] Lua：元表
来源：http://bo.panjiajie.cn

setmetatable({}, { __index = base })
来源：http://xe.wgjwhj.cn

[T41] Perl：Hello World
来源：http://fg.hnjuh.cn

print "Hello\n";
来源：http://pb.asd995.cn

[T42] Perl：变量类型
来源：http://rz.szxytkj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ml.haigaiapp.cn

[T43] Perl：字符串插值
来源：http://il.521024.cn

"值: $a"
来源：http://jg.gzmigu.cn

[T44] Perl：条件
来源：http://re.9csxet.cn

if ($a > 0) { print "正"; }
来源：http://cw.shxzskj.cn

[T45] Perl：数组遍历
来源：http://bx.huixiangedu.cn

for my $x (@arr) { print $x; }
来源：http://up.shtwfgs.cn

[T46] Perl：哈希操作
来源：http://aj.nicolike.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://os.gzmigu.cn

[T47] Perl：正则捕获
来源：http://xw.huixiangedu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ol.gzmigu.cn

[T48] Perl：正则替换
来源：http://ja.shtwfgs.cn

$s =~ s/old/new/g;
来源：http://hz.gzmigu.cn

[T49] Perl：函数
来源：http://nf.asd995.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ed.colortex.cn

[T50] Perl：逐行读文件
来源：http://ur.asd995.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://lk.haigaiapp.cn

while (my $line = <$fh>) { print $line; }
来源：http://ux.yuntaijiaju.cn

[T51] Scala：Hello World
来源：http://mn.bookmarksfly.cn

println("Hello")
来源：http://gr.lnxyls.cn

[T52] Scala：变量
来源：http://rh.yuexingan06.cn

val a = 1;  var b = 2
来源：http://bn.jianghongdianzi.cn

[T53] Scala：字符串插值
来源：http://hx.wgjwhj.cn

s"值: $b"
来源：http://sx.newstarts.cn

[T54] Scala：集合映射
来源：http://vz.wgjwhj.cn

List(1, 2, 3).map(_ * 2)
来源：http://wy.wgjwhj.cn

[T55] Scala：集合过滤
来源：http://th.bjjhwx.cn

List(1, 2, 3).filter(_ > 1)
来源：http://jr.shtwfgs.cn

[T56] Scala：样例类
来源：http://yl.hnjuh.cn

case class User(name: String, age: Int)
来源：http://mb.shxzukj.cn

[T57] Scala：模式匹配
来源：http://sn.muxihuayi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://cb.bjjhwx.cn

[T58] Scala：函数定义
来源：http://ri.wgjwhj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://cd.huixiangedu.cn

[T59] Scala：循环
来源：http://lz.nicolike.cn

for (i <- 1 to 10) println(i)
来源：http://dc.jctech888.com.cn

[T60] Scala：折叠
来源：http://hc.bookmarksfly.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ka.shxzskj.cn

================================================================================
来源：http://vc.huixinmuqiang.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ix.hnjuh.cn

================================================================================
来源：http://nd.nicolike.cn

[U01] Py：创建虚拟环境
来源：http://oe.bookmarksfly.cn

python -m venv .venv && source .venv/bin/activate
来源：http://hw.shtwfgs.cn

[U02] Py：导出 / 安装依赖
来源：http://dg.wgjwhj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bs.yuexingan06.cn

[U03] Py：加载 .env 配置
来源：http://sb.huixiangedu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://vm.shtwfgs.cn

[U04] Py：变量调试打印
来源：http://dv.lnxyls.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ug.bjjhwx.cn

[U05] Py：列表去重且保序
来源：http://xl.9csxet.cn

list(dict.fromkeys(arr))
来源：http://vj.hnjuh.cn

[U06] Py：合并两个字典
来源：http://ig.szxytkj.cn

{**a, **b}
来源：http://ke.haigaiapp.cn

[U07] Py：反转字典键值
来源：http://va.asd995.cn

{v: k for k, v in d.items()}
来源：http://er.huanxung.cn

[U08] Py：展平二维列表
来源：http://zz.newstarts.cn

[y for x in nested for y in x]
来源：http://wq.newstarts.cn

[U09] Py：字典取最大值的键
来源：http://tt.huanxung.cn

max(d, key=d.get)
来源：http://di.nicolike.cn

[U10] Py：按值排序字典
来源：http://dm.huixinmuqiang.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sk.hnjuh.cn

[U11] Py：生成器表达式
来源：http://ya.huanxung.cn

(x * 2 for x in arr)
来源：http://ok.jctech888.com.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ve.szsharing.cn

Counter(arr).most_common(3)
来源：http://gj.nszjky.cn

[U13] Py：固定长度队列
来源：http://ba.huixinmuqiang.cn

deque(maxlen=10)
来源：http://ts.jctech888.com.cn

[U14] Py：分组收集到列表
来源：http://rs.newstarts.cn

defaultdict(list)
来源：http://mc.panjiajie.cn

[U15] Py：高精度计时
来源：http://qn.chemitech.net.cn

t = time.perf_counter()
来源：http://io.colortex.cn

[U16] Py：命令行参数解析
来源：http://cw.panjiajie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tz.hnjuh.cn

[U17] Py：初始化日志
来源：http://ar.huanxung.cn

logging.basicConfig(level=logging.INFO)
来源：http://vk.yuntaijiaju.cn

[U18] Py：预编译正则
来源：http://pt.huanxung.cn

pat = re.compile(r"\d+")
来源：http://fe.szxytkj.cn

[U19] Py：正则替换带回调
来源：http://pu.szsharing.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vl.szxytkj.cn

[U20] Py：缓存函数结果
来源：http://pw.gzmigu.cn

@functools.lru_cache(maxsize=None)
来源：http://zw.panjiajie.cn

[U21] Py：自定义上下文管理器
来源：http://gb.szsharing.cn

@contextlib.contextmanager
来源：http://zo.muxihuayi.cn

[U22] Py：矩阵转置
来源：http://jd.newstarts.cn

list(zip(*m))
来源：http://qp.lnxyls.cn

[U23] Py：分块读取大文件
来源：http://im.asd995.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fz.jianghongdianzi.cn

[U24] Py：路径操作
来源：http://tk.panjiajie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://am.asd995.cn

[U25] Py：CSV 按字典读
来源：http://ea.9csxet.cn

csv.DictReader(f)
来源：http://bl.521024.cn

[U26] Py：并发下载
来源：http://fi.szsharing.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hg.huixiangedu.cn

[U27] Py：异步 HTTP
来源：http://pg.hahajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://nc.huixiangedu.cn

[U28] Py：类型别名
来源：http://oq.jctech888.com.cn

UserId = int
来源：http://dl.newstarts.cn

[U29] Py：属性校验
来源：http://gd.colortex.cn

@property 与 @x.setter 配合
来源：http://th.521024.cn

[U30] Py：数据类
来源：http://bo.nszjky.cn

@dataclass(slots=True)
来源：http://vb.jianghongdianzi.cn

[U31] Py：单测
来源：http://mh.bjjhwx.cn

python -m pytest -q
来源：http://ls.huanxung.cn

[U32] Py：代码格式化
来源：http://yc.hnjuh.cn

ruff format . && ruff check --fix .
来源：http://tw.yuntaijiaju.cn

[U33] Py：打包发布
来源：http://fk.colortex.cn

python -m build  （依赖 pyproject.toml）
来源：http://my.muxihuayi.cn

[U34] Py：判断编码
来源：http://zh.bookmarksfly.cn

chardet.detect(raw)
来源：http://rl.shxzskj.cn

[U35] Py：发送邮件
来源：http://vm.nszjky.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yx.muxihuayi.cn

[U36] Py：定时任务
来源：http://dn.huixinmuqiang.cn

schedule.every(10).minutes.do(job)
来源：http://il.lnxyls.cn

[U37] Py：读写 Excel
来源：http://pp.9csxet.cn

pandas.read_excel / DataFrame.to_excel
来源：http://zm.huixinmuqiang.cn

[U38] Py：获取脚本所在目录
来源：http://kp.yuexingan06.cn

Path(__file__).resolve().parent
来源：http://px.huixinmuqiang.cn

[U39] Py：判断是否在交互环境
来源：http://lh.nicolike.cn

sys.stdout.isatty()
来源：http://lj.haigaiapp.cn

[U40] Py：打印到标准错误
来源：http://dz.huanxung.cn

print("err", file=sys.stderr)
来源：http://kv.gzmigu.cn

[U41] PHP：初始化 Composer 项目
来源：http://tk.huixiangedu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ly.hahajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://ef.asd995.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zq.colortex.cn

[U43] PHP：声明命名空间
来源：http://md.bookmarksfly.cn

namespace App\Http;
来源：http://xa.521024.cn

[U44] PHP：开启严格类型
来源：http://gv.jctech888.com.cn

declare(strict_types=1);
来源：http://bu.wgjwhj.cn

[U45] PHP：类型声明与返回类型
来源：http://ki.newstarts.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bp.szsharing.cn

[U46] PHP：可空类型
来源：http://so.nicolike.cn

?string $name = null
来源：http://vy.panjiajie.cn

[U47] PHP：联合类型
来源：http://qw.szsharing.cn

int|string $id
来源：http://gg.huixiangedu.cn

[U48] PHP：纯枚举
来源：http://mh.jianghongdianzi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dx.jctech888.com.cn

[U49] PHP：只读属性
来源：http://gl.jctech888.com.cn

public readonly string $name
来源：http://ht.huixinmuqiang.cn

[U50] PHP：构造器属性提升
来源：http://tg.shtwfgs.cn

public function __construct(private int $id) {}
来源：http://aw.bookmarksfly.cn

[U51] PHP：数组解构
来源：http://xv.colortex.cn

[$a, $b] = $arr;
来源：http://cp.haigaiapp.cn

[U52] PHP：箭头函数
来源：http://nx.yuntaijiaju.cn

$double = fn($x) => $x * 2;
来源：http://qf.shtwfgs.cn

[U53] PHP：空合并运算符
来源：http://bp.huixiangedu.cn

$v = $a ?? $b ?? "default";
来源：http://ym.521024.cn

[U54] PHP：空安全调用
来源：http://dx.colortex.cn

$obj?->method()
来源：http://rz.lnxyls.cn

[U55] PHP：match 表达式
来源：http://gw.jctech888.com.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zd.hnjuh.cn

[U56] PHP：命名参数
来源：http://yd.huixinmuqiang.cn

f(a: 1, b: 2)
来源：http://rb.nicolike.cn

[U57] PHP：字符串插值
来源：http://ll.bjjhwx.cn

"值: {$a}"
来源：http://ub.hnjuh.cn

[U58] PHP：数组三件套
来源：http://vr.shtwfgs.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nw.gzmigu.cn

[U59] PHP：自定义排序
来源：http://hu.szxytkj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ux.hnjuh.cn

[U60] PHP：JSON 编解码
来源：http://uu.bjjhwx.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cg.wgjwhj.cn

[U61] PHP：正则
来源：http://dd.nicolike.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xq.9csxet.cn

[U62] PHP：日期对象
来源：http://cd.huixinmuqiang.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fh.shtwfgs.cn

[U63] PHP：文件读写
来源：http://bz.hnjuh.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rn.szxytkj.cn

[U64] PHP：目录遍历
来源：http://ai.wgjwhj.cn

glob("dir/*.php");  scandir("dir");
来源：http://nj.yuexingan06.cn

[U65] PHP：会话
来源：http://sw.asd995.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ax.jctech888.com.cn

[U66] PHP：设置 Cookie
来源：http://rf.wgjwhj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rn.wgjwhj.cn

[U67] PHP：处理文件上传
来源：http://xr.newstarts.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ff.panjiajie.cn

[U68] PHP：PDO 连接
来源：http://nm.nicolike.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mm.shxzskj.cn

[U69] PHP：PDO 预处理
来源：http://nl.newstarts.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cw.hnjuh.cn

[U70] PHP：PDO 事务
来源：http://jk.huixiangedu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://it.bjjhwx.cn

[U71] PHP：抛出异常
来源：http://qu.nicolike.cn

throw new RuntimeException("失败", 500);
来源：http://ux.asd995.cn

[U72] PHP：写错误日志
来源：http://un.asd995.cn

error_log("失败: " . $e->getMessage());
来源：http://rn.haigaiapp.cn

[U73] PHP：读取 ini 配置
来源：http://ch.muxihuayi.cn

parse_ini_file("config.ini", true)
来源：http://dp.asd995.cn

[U74] PHP：读取环境变量
来源：http://ou.nicolike.cn

getenv("APP_ENV") ?: "production"
来源：http://ag.muxihuayi.cn

[U75] PHP：依赖注入
来源：http://qk.huanxung.cn

composer require psr/container
来源：http://pz.huixiangedu.cn

[U76] PHP：简单路由
来源：http://pk.panjiajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rg.hahajie.cn

[U77] PHP：模板渲染
来源：http://dt.gzmigu.cn

composer require twig/twig
来源：http://xy.9csxet.cn

[U78] PHP：单元测试
来源：http://uo.bookmarksfly.cn

composer require --dev phpunit/phpunit
来源：http://yu.shtwfgs.cn

[U79] PHP：静态分析
来源：http://hr.wgjwhj.cn

composer require --dev phpstan/phpstan
来源：http://vd.colortex.cn

[U80] PHP：代码规范修复
来源：http://he.521024.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://mm.panjiajie.cn

[U81] JS：初始化项目
来源：http://xd.panjiajie.cn

npm init -y;  npm i express
来源：http://zr.shtwfgs.cn

[U82] JS：package.json 脚本
来源：http://xa.jianghongdianzi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ls.chemitech.net.cn

[U83] JS：ES Module 导入导出
来源：http://wp.yuexingan06.cn

export const a = 1;  import { a } from "./m.js";
来源：http://gg.hahajie.cn

[U84] JS：CommonJS 写法
来源：http://my.wgjwhj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://bd.muxihuayi.cn

[U85] JS：可选链
来源：http://hn.wgjwhj.cn

a?.b?.c
来源：http://nh.yuexingan06.cn

[U86] JS：空值合并
来源：http://ck.shxzukj.cn

a ?? b
来源：http://tq.muxihuayi.cn

[U87] JS：解构默认值
来源：http://we.yuexingan06.cn

const { a = 1, b = 2 } = obj;
来源：http://fc.shxzskj.cn

[U88] JS：对象展开合并
来源：http://xg.shxzskj.cn

{ ...a, ...b }
来源：http://ft.yuntaijiaju.cn

[U89] JS：数组去重
来源：http://rt.yuexingan06.cn

[...new Set(arr)]
来源：http://jm.szxytkj.cn

[U90] JS：数字数组排序
来源：http://yu.muxihuayi.cn

[...arr].sort((a, b) => a - b)
来源：http://hx.szxytkj.cn

[U91] JS：对象键值遍历
来源：http://vg.panjiajie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://br.wgjwhj.cn

[U92] JS：深拷贝
来源：http://pd.shxzukj.cn

structuredClone(obj)
来源：http://pt.nicolike.cn

[U93] JS：模板字符串
来源：http://qp.nszjky.cn

`共 ${n} 条`
来源：http://cd.yuexingan06.cn

[U94] JS：箭头函数
来源：http://zd.chemitech.net.cn

const double = x => x * 2;
来源：http://jg.9csxet.cn

[U95] JS：Promise 包装
来源：http://nv.haigaiapp.cn

new Promise((resolve, reject) => {})
来源：http://tm.gzmigu.cn

[U96] JS：async/await 与异常
来源：http://xi.yuexingan06.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://go.9csxet.cn

[U97] JS：并发请求
来源：http://fn.shxzukj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://sh.9csxet.cn

[U98] JS：fetch 带 JSON
来源：http://xo.wgjwhj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vu.haigaiapp.cn

[U99] JS：事件监听
来源：http://rv.nszjky.cn

el.addEventListener("click", e => {})
来源：http://mp.nicolike.cn

[U100] JS：DOM 查询
来源：http://lh.yuntaijiaju.cn

document.querySelector(".item")
来源：http://gp.gzmigu.cn

[U101] JS：classList 操作
来源：http://ov.chemitech.net.cn

el.classList.toggle("active")
来源：http://hm.wgjwhj.cn

[U102] JS：本地存储
来源：http://gz.asd995.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://nj.jianghongdianzi.cn

[U103] JS：定时器
来源：http://ia.wgjwhj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vq.gzmigu.cn

[U104] JS：防抖
来源：http://md.newstarts.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://en.jianghongdianzi.cn

[U105] JS：节流
来源：http://oq.haigaiapp.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ti.muxihuayi.cn

[U106] JS：日期格式化
来源：http://zv.newstarts.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://je.shxzukj.cn

[U107] JS：数字千分位
来源：http://zc.yuexingan06.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cs.muxihuayi.cn

[U108] JS：随机整数
来源：http://jq.szxytkj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://uj.9csxet.cn


<!-- 参考信息 -->