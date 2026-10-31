代发 wailian999

[T19] Swift：可选绑定
来源：http://tw.521024.cn

if let n = opt { print(n) }
来源：http://yl.szsharing.cn

[T20] Swift：数组操作
来源：http://vw.chemitech.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://vj.huixiangedu.cn

[T21] Swift：遍历
来源：http://bq.9csxet.cn

for x in a { print(x) }
来源：http://ni.jianghongdianzi.cn

[T22] Swift：字典
来源：http://nh.panjiajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mv.jctech888.com.cn

[T23] Swift：函数
来源：http://pw.szsharing.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ao.yuntaijiaju.cn

[T24] Swift：闭包
来源：http://jb.yuexingan06.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://df.wgjwhj.cn

[T25] Swift：结构体
来源：http://gy.huixinmuqiang.cn

struct P { var x: Int }
来源：http://fp.hahajie.cn

[T26] Swift：类与重写
来源：http://ow.jianghongdianzi.cn

class A: Base { override func f() {} }
来源：http://rh.bookmarksfly.cn

[T27] Swift：错误处理
来源：http://vy.yuntaijiaju.cn

do { try f() } catch { print(error) }
来源：http://he.huanxung.cn

[T28] Swift：枚举
来源：http://jr.panjiajie.cn

enum Color { case red, green }
来源：http://ci.hahajie.cn

[T29] Swift：guard 提前返回
来源：http://ss.bjjhwx.cn

guard let x = opt else { return }
来源：http://zl.521024.cn

[T30] Swift：协议
来源：http://uh.bjjhwx.cn

protocol Shape { func area() -> Double }
来源：http://yg.nicolike.cn

[T31] Lua：Hello World
来源：http://yz.9csxet.cn

print("Hello")
来源：http://hy.yuexingan06.cn

[T32] Lua：局部变量
来源：http://ap.hnjuh.cn

local a = 1
来源：http://gn.huixiangedu.cn

[T33] Lua：表（数组）
来源：http://vo.huixiangedu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://yo.chemitech.net.cn

[T34] Lua：遍历表
来源：http://jj.yuexingan06.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://wa.bookmarksfly.cn

[T35] Lua：字典表
来源：http://fs.huixiangedu.cn

local d = { a = 1 };  d.b = 2
来源：http://un.asd995.cn

[T36] Lua：函数
来源：http://ny.haigaiapp.cn

function add(a, b) return a + b end
来源：http://tp.huixinmuqiang.cn

[T37] Lua：字符串拼接
来源：http://up.panjiajie.cn

"a" .. "b"
来源：http://aw.szsharing.cn

[T38] Lua：条件
来源：http://fx.hahajie.cn

if x > 0 then print("正") end
来源：http://db.szxytkj.cn

[T39] Lua：模式匹配
来源：http://ur.huixinmuqiang.cn

string.find(s, "%d+")
来源：http://uf.nszjky.cn

[T40] Lua：元表
来源：http://ax.muxihuayi.cn

setmetatable({}, { __index = base })
来源：http://dp.muxihuayi.cn

[T41] Perl：Hello World
来源：http://nc.szxytkj.cn

print "Hello\n";
来源：http://iw.lnxyls.cn

[T42] Perl：变量类型
来源：http://mp.szxytkj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ry.hnjuh.cn

[T43] Perl：字符串插值
来源：http://nq.bjjhwx.cn

"值: $a"
来源：http://lc.panjiajie.cn

[T44] Perl：条件
来源：http://eb.muxihuayi.cn

if ($a > 0) { print "正"; }
来源：http://jq.newstarts.cn

[T45] Perl：数组遍历
来源：http://wv.shtwfgs.cn

for my $x (@arr) { print $x; }
来源：http://dz.szsharing.cn

[T46] Perl：哈希操作
来源：http://np.jianghongdianzi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://td.haigaiapp.cn

[T47] Perl：正则捕获
来源：http://gr.haigaiapp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rd.bookmarksfly.cn

[T48] Perl：正则替换
来源：http://ly.hnjuh.cn

$s =~ s/old/new/g;
来源：http://mz.bookmarksfly.cn

[T49] Perl：函数
来源：http://zy.shxzskj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://aw.gzmigu.cn

[T50] Perl：逐行读文件
来源：http://uk.szxytkj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xe.jctech888.com.cn

while (my $line = <$fh>) { print $line; }
来源：http://ac.shtwfgs.cn

[T51] Scala：Hello World
来源：http://iu.hnjuh.cn

println("Hello")
来源：http://po.panjiajie.cn

[T52] Scala：变量
来源：http://dd.521024.cn

val a = 1;  var b = 2
来源：http://pu.hnjuh.cn

[T53] Scala：字符串插值
来源：http://ns.hahajie.cn

s"值: $b"
来源：http://vd.colortex.cn

[T54] Scala：集合映射
来源：http://fu.bjjhwx.cn

List(1, 2, 3).map(_ * 2)
来源：http://cj.asd995.cn

[T55] Scala：集合过滤
来源：http://ys.wgjwhj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://kf.shxzukj.cn

[T56] Scala：样例类
来源：http://pm.asd995.cn

case class User(name: String, age: Int)
来源：http://ak.bjjhwx.cn

[T57] Scala：模式匹配
来源：http://mi.yuexingan06.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fw.wgjwhj.cn

[T58] Scala：函数定义
来源：http://fo.wgjwhj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://mm.chemitech.net.cn

[T59] Scala：循环
来源：http://lz.newstarts.cn

for (i <- 1 to 10) println(i)
来源：http://cj.haigaiapp.cn

[T60] Scala：折叠
来源：http://ya.chemitech.net.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gn.nicolike.cn

================================================================================
来源：http://cv.muxihuayi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yg.chemitech.net.cn

================================================================================
来源：http://eu.huixinmuqiang.cn

[U01] Py：创建虚拟环境
来源：http://sb.jctech888.com.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jz.shxzukj.cn

[U02] Py：导出 / 安装依赖
来源：http://oy.shxzukj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ic.yuntaijiaju.cn

[U03] Py：加载 .env 配置
来源：http://hf.haigaiapp.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rd.shxzskj.cn

[U04] Py：变量调试打印
来源：http://ch.hahajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xr.yuntaijiaju.cn

[U05] Py：列表去重且保序
来源：http://kv.nszjky.cn

list(dict.fromkeys(arr))
来源：http://cq.yuexingan06.cn

[U06] Py：合并两个字典
来源：http://wb.nicolike.cn

{**a, **b}
来源：http://dr.bjjhwx.cn

[U07] Py：反转字典键值
来源：http://ev.jctech888.com.cn

{v: k for k, v in d.items()}
来源：http://rp.jctech888.com.cn

[U08] Py：展平二维列表
来源：http://iw.yuexingan06.cn

[y for x in nested for y in x]
来源：http://tn.szxytkj.cn

[U09] Py：字典取最大值的键
来源：http://np.asd995.cn

max(d, key=d.get)
来源：http://so.huanxung.cn

[U10] Py：按值排序字典
来源：http://va.lnxyls.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vi.nicolike.cn

[U11] Py：生成器表达式
来源：http://gt.521024.cn

(x * 2 for x in arr)
来源：http://my.jctech888.com.cn

[U12] Py：取出现最多的 3 个元素
来源：http://az.shxzukj.cn

Counter(arr).most_common(3)
来源：http://ip.yuntaijiaju.cn

[U13] Py：固定长度队列
来源：http://sr.asd995.cn

deque(maxlen=10)
来源：http://eg.nszjky.cn

[U14] Py：分组收集到列表
来源：http://df.bjjhwx.cn

defaultdict(list)
来源：http://ke.nszjky.cn

[U15] Py：高精度计时
来源：http://sf.9csxet.cn

t = time.perf_counter()
来源：http://jf.colortex.cn

[U16] Py：命令行参数解析
来源：http://ah.yuntaijiaju.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ht.bjjhwx.cn

[U17] Py：初始化日志
来源：http://ac.lnxyls.cn

logging.basicConfig(level=logging.INFO)
来源：http://tg.asd995.cn

[U18] Py：预编译正则
来源：http://vm.lnxyls.cn

pat = re.compile(r"\d+")
来源：http://zo.yuexingan06.cn

[U19] Py：正则替换带回调
来源：http://ni.huixiangedu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ev.shxzskj.cn

[U20] Py：缓存函数结果
来源：http://eq.muxihuayi.cn

@functools.lru_cache(maxsize=None)
来源：http://bg.yuntaijiaju.cn

[U21] Py：自定义上下文管理器
来源：http://ty.colortex.cn

@contextlib.contextmanager
来源：http://us.hahajie.cn

[U22] Py：矩阵转置
来源：http://xm.wgjwhj.cn

list(zip(*m))
来源：http://si.yuexingan06.cn

[U23] Py：分块读取大文件
来源：http://kb.chemitech.net.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hw.chemitech.net.cn

[U24] Py：路径操作
来源：http://bn.shtwfgs.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nu.haigaiapp.cn

[U25] Py：CSV 按字典读
来源：http://ki.bjjhwx.cn

csv.DictReader(f)
来源：http://sv.521024.cn

[U26] Py：并发下载
来源：http://vs.shxzskj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xw.panjiajie.cn

[U27] Py：异步 HTTP
来源：http://xg.shxzukj.cn

aiohttp.ClientSession() 配合 async with
来源：http://lf.huixinmuqiang.cn

[U28] Py：类型别名
来源：http://fj.hnjuh.cn

UserId = int
来源：http://gx.lnxyls.cn

[U29] Py：属性校验
来源：http://sk.szxytkj.cn

@property 与 @x.setter 配合
来源：http://lp.shtwfgs.cn

[U30] Py：数据类
来源：http://dd.shtwfgs.cn

@dataclass(slots=True)
来源：http://ee.9csxet.cn

[U31] Py：单测
来源：http://ul.colortex.cn

python -m pytest -q
来源：http://sb.newstarts.cn

[U32] Py：代码格式化
来源：http://pk.szxytkj.cn

ruff format . && ruff check --fix .
来源：http://te.yuexingan06.cn

[U33] Py：打包发布
来源：http://qp.yuexingan06.cn

python -m build  （依赖 pyproject.toml）
来源：http://lh.shxzukj.cn

[U34] Py：判断编码
来源：http://ae.wgjwhj.cn

chardet.detect(raw)
来源：http://ck.nicolike.cn

[U35] Py：发送邮件
来源：http://pv.huanxung.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yw.newstarts.cn

[U36] Py：定时任务
来源：http://tu.jianghongdianzi.cn

schedule.every(10).minutes.do(job)
来源：http://ox.521024.cn

[U37] Py：读写 Excel
来源：http://yh.hnjuh.cn

pandas.read_excel / DataFrame.to_excel
来源：http://rj.asd995.cn

[U38] Py：获取脚本所在目录
来源：http://xq.521024.cn

Path(__file__).resolve().parent
来源：http://px.huixiangedu.cn

[U39] Py：判断是否在交互环境
来源：http://kv.wgjwhj.cn

sys.stdout.isatty()
来源：http://mc.shtwfgs.cn

[U40] Py：打印到标准错误
来源：http://ro.newstarts.cn

print("err", file=sys.stderr)
来源：http://bt.panjiajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://ye.yuexingan06.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://wf.huanxung.cn

[U42] PHP：PSR-4 自动加载
来源：http://cj.521024.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vb.jctech888.com.cn

[U43] PHP：声明命名空间
来源：http://ng.lnxyls.cn

namespace App\Http;
来源：http://wp.asd995.cn

[U44] PHP：开启严格类型
来源：http://rv.haigaiapp.cn

declare(strict_types=1);
来源：http://pk.hnjuh.cn

[U45] PHP：类型声明与返回类型
来源：http://iq.yuntaijiaju.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://oq.szxytkj.cn

[U46] PHP：可空类型
来源：http://lm.panjiajie.cn

?string $name = null
来源：http://hv.jianghongdianzi.cn

[U47] PHP：联合类型
来源：http://dd.muxihuayi.cn

int|string $id
来源：http://ip.muxihuayi.cn

[U48] PHP：纯枚举
来源：http://tq.wgjwhj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ux.hnjuh.cn

[U49] PHP：只读属性
来源：http://vl.yuexingan06.cn

public readonly string $name
来源：http://ry.huanxung.cn

[U50] PHP：构造器属性提升
来源：http://gd.shxzskj.cn

public function __construct(private int $id) {}
来源：http://wl.gzmigu.cn

[U51] PHP：数组解构
来源：http://ki.panjiajie.cn

[$a, $b] = $arr;
来源：http://rg.huixinmuqiang.cn

[U52] PHP：箭头函数
来源：http://cu.muxihuayi.cn

$double = fn($x) => $x * 2;
来源：http://xz.szxytkj.cn

[U53] PHP：空合并运算符
来源：http://uu.muxihuayi.cn

$v = $a ?? $b ?? "default";
来源：http://wl.colortex.cn

[U54] PHP：空安全调用
来源：http://ar.jianghongdianzi.cn

$obj?->method()
来源：http://cu.9csxet.cn

[U55] PHP：match 表达式
来源：http://eb.asd995.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cm.asd995.cn

[U56] PHP：命名参数
来源：http://ec.muxihuayi.cn

f(a: 1, b: 2)
来源：http://ei.yuntaijiaju.cn

[U57] PHP：字符串插值
来源：http://yz.muxihuayi.cn

"值: {$a}"
来源：http://rl.shxzukj.cn

[U58] PHP：数组三件套
来源：http://ai.jctech888.com.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ak.szsharing.cn

[U59] PHP：自定义排序
来源：http://fr.shxzukj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xy.muxihuayi.cn

[U60] PHP：JSON 编解码
来源：http://zo.521024.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gm.huixinmuqiang.cn

[U61] PHP：正则
来源：http://fh.wgjwhj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fk.yuntaijiaju.cn

[U62] PHP：日期对象
来源：http://ha.hnjuh.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qq.yuexingan06.cn

[U63] PHP：文件读写
来源：http://ol.hahajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ps.nszjky.cn

[U64] PHP：目录遍历
来源：http://ip.lnxyls.cn

glob("dir/*.php");  scandir("dir");
来源：http://pd.nicolike.cn

[U65] PHP：会话
来源：http://zq.huanxung.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://gy.huixinmuqiang.cn

[U66] PHP：设置 Cookie
来源：http://vq.asd995.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kx.huixiangedu.cn

[U67] PHP：处理文件上传
来源：http://dl.shtwfgs.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://iz.haigaiapp.cn

[U68] PHP：PDO 连接
来源：http://kv.lnxyls.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://in.huanxung.cn

[U69] PHP：PDO 预处理
来源：http://lt.jctech888.com.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mc.nszjky.cn

[U70] PHP：PDO 事务
来源：http://tk.asd995.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kg.huixiangedu.cn

[U71] PHP：抛出异常
来源：http://np.asd995.cn

throw new RuntimeException("失败", 500);
来源：http://hm.yuexingan06.cn

[U72] PHP：写错误日志
来源：http://kz.panjiajie.cn

error_log("失败: " . $e->getMessage());
来源：http://rp.nszjky.cn

[U73] PHP：读取 ini 配置
来源：http://ai.szxytkj.cn

parse_ini_file("config.ini", true)
来源：http://qh.haigaiapp.cn

[U74] PHP：读取环境变量
来源：http://su.colortex.cn

getenv("APP_ENV") ?: "production"
来源：http://ta.9csxet.cn

[U75] PHP：依赖注入
来源：http://oj.colortex.cn

composer require psr/container
来源：http://rk.yuexingan06.cn

[U76] PHP：简单路由
来源：http://od.jctech888.com.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zb.muxihuayi.cn

[U77] PHP：模板渲染
来源：http://zh.szxytkj.cn

composer require twig/twig
来源：http://ug.shxzukj.cn

[U78] PHP：单元测试
来源：http://hw.hnjuh.cn

composer require --dev phpunit/phpunit
来源：http://in.huanxung.cn

[U79] PHP：静态分析
来源：http://uw.hahajie.cn

composer require --dev phpstan/phpstan
来源：http://dg.bjjhwx.cn

[U80] PHP：代码规范修复
来源：http://qd.newstarts.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://cy.hahajie.cn

[U81] JS：初始化项目
来源：http://jw.huixinmuqiang.cn

npm init -y;  npm i express
来源：http://go.nicolike.cn

[U82] JS：package.json 脚本
来源：http://pj.jctech888.com.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://eh.bjjhwx.cn

[U83] JS：ES Module 导入导出
来源：http://je.shxzskj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://tm.bookmarksfly.cn

[U84] JS：CommonJS 写法
来源：http://ws.asd995.cn

module.exports = { a };  const { a } = require("./m");
来源：http://le.jctech888.com.cn

[U85] JS：可选链
来源：http://ln.hnjuh.cn

a?.b?.c
来源：http://sr.jianghongdianzi.cn

[U86] JS：空值合并
来源：http://xl.shxzukj.cn

a ?? b
来源：http://fk.panjiajie.cn

[U87] JS：解构默认值
来源：http://ld.haigaiapp.cn

const { a = 1, b = 2 } = obj;
来源：http://jg.hnjuh.cn

[U88] JS：对象展开合并
来源：http://hf.huixiangedu.cn

{ ...a, ...b }
来源：http://wm.huixinmuqiang.cn

[U89] JS：数组去重
来源：http://vl.szsharing.cn

[...new Set(arr)]
来源：http://jb.hnjuh.cn

[U90] JS：数字数组排序
来源：http://ei.bjjhwx.cn

[...arr].sort((a, b) => a - b)
来源：http://cg.9csxet.cn

[U91] JS：对象键值遍历
来源：http://mr.yuntaijiaju.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lg.haigaiapp.cn

[U92] JS：深拷贝
来源：http://rl.panjiajie.cn

structuredClone(obj)
来源：http://ww.szxytkj.cn

[U93] JS：模板字符串
来源：http://pp.asd995.cn

`共 ${n} 条`
来源：http://hq.shxzskj.cn

[U94] JS：箭头函数
来源：http://ua.asd995.cn

const double = x => x * 2;
来源：http://jk.nicolike.cn

[U95] JS：Promise 包装
来源：http://yf.haigaiapp.cn

new Promise((resolve, reject) => {})
来源：http://sx.nicolike.cn

[U96] JS：async/await 与异常
来源：http://ft.nicolike.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://iu.newstarts.cn

[U97] JS：并发请求
来源：http://wj.9csxet.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ts.521024.cn

[U98] JS：fetch 带 JSON
来源：http://ho.shxzukj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hu.huixiangedu.cn

[U99] JS：事件监听
来源：http://zk.jianghongdianzi.cn

el.addEventListener("click", e => {})
来源：http://tb.huanxung.cn

[U100] JS：DOM 查询
来源：http://mh.lnxyls.cn

document.querySelector(".item")
来源：http://nq.nicolike.cn

[U101] JS：classList 操作
来源：http://hf.jctech888.com.cn

el.classList.toggle("active")
来源：http://hm.chemitech.net.cn

[U102] JS：本地存储
来源：http://zn.szxytkj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ax.newstarts.cn

[U103] JS：定时器
来源：http://or.colortex.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vo.521024.cn

[U104] JS：防抖
来源：http://zh.521024.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://or.bjjhwx.cn

[U105] JS：节流
来源：http://iq.gzmigu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yp.yuntaijiaju.cn

[U106] JS：日期格式化
来源：http://zp.muxihuayi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ot.yuexingan06.cn


<!-- 参考信息 -->