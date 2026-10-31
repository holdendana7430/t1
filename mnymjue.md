代发 wailian999

[T19] Swift：可选绑定
来源：http://xu.hnjuh.cn

if let n = opt { print(n) }
来源：http://qk.shtwfgs.cn

[T20] Swift：数组操作
来源：http://vj.gzmigu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://eu.yuntaijiaju.cn

[T21] Swift：遍历
来源：http://rw.huanxung.cn

for x in a { print(x) }
来源：http://dm.yuntaijiaju.cn

[T22] Swift：字典
来源：http://nr.colortex.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zu.newstarts.cn

[T23] Swift：函数
来源：http://pq.huanxung.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://du.hahajie.cn

[T24] Swift：闭包
来源：http://oi.wgjwhj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://lt.newstarts.cn

[T25] Swift：结构体
来源：http://ss.hnjuh.cn

struct P { var x: Int }
来源：http://pl.521024.cn

[T26] Swift：类与重写
来源：http://oo.shxzukj.cn

class A: Base { override func f() {} }
来源：http://wd.hahajie.cn

[T27] Swift：错误处理
来源：http://ne.lnxyls.cn

do { try f() } catch { print(error) }
来源：http://ia.asd995.cn

[T28] Swift：枚举
来源：http://ne.huixiangedu.cn

enum Color { case red, green }
来源：http://bn.huixiangedu.cn

[T29] Swift：guard 提前返回
来源：http://xu.shxzskj.cn

guard let x = opt else { return }
来源：http://md.nszjky.cn

[T30] Swift：协议
来源：http://wy.shxzskj.cn

protocol Shape { func area() -> Double }
来源：http://ie.9csxet.cn

[T31] Lua：Hello World
来源：http://wb.huixiangedu.cn

print("Hello")
来源：http://hr.jctech888.com.cn

[T32] Lua：局部变量
来源：http://no.hahajie.cn

local a = 1
来源：http://sr.jctech888.com.cn

[T33] Lua：表（数组）
来源：http://dx.shtwfgs.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://by.muxihuayi.cn

[T34] Lua：遍历表
来源：http://vw.gzmigu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ga.wgjwhj.cn

[T35] Lua：字典表
来源：http://da.521024.cn

local d = { a = 1 };  d.b = 2
来源：http://rv.521024.cn

[T36] Lua：函数
来源：http://ut.wgjwhj.cn

function add(a, b) return a + b end
来源：http://bs.colortex.cn

[T37] Lua：字符串拼接
来源：http://gj.haigaiapp.cn

"a" .. "b"
来源：http://cd.gzmigu.cn

[T38] Lua：条件
来源：http://st.bjjhwx.cn

if x > 0 then print("正") end
来源：http://mm.hnjuh.cn

[T39] Lua：模式匹配
来源：http://gj.newstarts.cn

string.find(s, "%d+")
来源：http://ic.huanxung.cn

[T40] Lua：元表
来源：http://zq.9csxet.cn

setmetatable({}, { __index = base })
来源：http://ke.hahajie.cn

[T41] Perl：Hello World
来源：http://hm.nicolike.cn

print "Hello\n";
来源：http://vo.jianghongdianzi.cn

[T42] Perl：变量类型
来源：http://sm.shxzskj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yx.jctech888.com.cn

[T43] Perl：字符串插值
来源：http://bb.hahajie.cn

"值: $a"
来源：http://hv.shtwfgs.cn

[T44] Perl：条件
来源：http://zn.shxzskj.cn

if ($a > 0) { print "正"; }
来源：http://un.szxytkj.cn

[T45] Perl：数组遍历
来源：http://ne.bjjhwx.cn

for my $x (@arr) { print $x; }
来源：http://tp.gzmigu.cn

[T46] Perl：哈希操作
来源：http://av.szxytkj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lq.shxzskj.cn

[T47] Perl：正则捕获
来源：http://uq.haigaiapp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ob.nicolike.cn

[T48] Perl：正则替换
来源：http://az.muxihuayi.cn

$s =~ s/old/new/g;
来源：http://en.shxzskj.cn

[T49] Perl：函数
来源：http://tt.huanxung.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fk.bjjhwx.cn

[T50] Perl：逐行读文件
来源：http://nl.shxzukj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://sf.muxihuayi.cn

while (my $line = <$fh>) { print $line; }
来源：http://mk.asd995.cn

[T51] Scala：Hello World
来源：http://po.gzmigu.cn

println("Hello")
来源：http://ax.huixiangedu.cn

[T52] Scala：变量
来源：http://hq.huanxung.cn

val a = 1;  var b = 2
来源：http://uq.521024.cn

[T53] Scala：字符串插值
来源：http://ix.9csxet.cn

s"值: $b"
来源：http://yu.szxytkj.cn

[T54] Scala：集合映射
来源：http://fh.haigaiapp.cn

List(1, 2, 3).map(_ * 2)
来源：http://zw.nicolike.cn

[T55] Scala：集合过滤
来源：http://kq.shtwfgs.cn

List(1, 2, 3).filter(_ > 1)
来源：http://of.yuntaijiaju.cn

[T56] Scala：样例类
来源：http://hm.colortex.cn

case class User(name: String, age: Int)
来源：http://ld.asd995.cn

[T57] Scala：模式匹配
来源：http://tb.shxzskj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://rw.szxytkj.cn

[T58] Scala：函数定义
来源：http://ug.wgjwhj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://mr.9csxet.cn

[T59] Scala：循环
来源：http://bm.jianghongdianzi.cn

for (i <- 1 to 10) println(i)
来源：http://ww.newstarts.cn

[T60] Scala：折叠
来源：http://db.shxzukj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jk.gzmigu.cn

================================================================================
来源：http://fl.bjjhwx.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wt.lnxyls.cn

================================================================================
来源：http://fd.huanxung.cn

[U01] Py：创建虚拟环境
来源：http://tf.gzmigu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nr.bookmarksfly.cn

[U02] Py：导出 / 安装依赖
来源：http://vm.huixiangedu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vi.nszjky.cn

[U03] Py：加载 .env 配置
来源：http://ha.newstarts.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://by.wgjwhj.cn

[U04] Py：变量调试打印
来源：http://vs.shxzukj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zs.szxytkj.cn

[U05] Py：列表去重且保序
来源：http://vw.wgjwhj.cn

list(dict.fromkeys(arr))
来源：http://qq.asd995.cn

[U06] Py：合并两个字典
来源：http://xk.9csxet.cn

{**a, **b}
来源：http://kj.asd995.cn

[U07] Py：反转字典键值
来源：http://qn.haigaiapp.cn

{v: k for k, v in d.items()}
来源：http://dn.chemitech.net.cn

[U08] Py：展平二维列表
来源：http://fo.huanxung.cn

[y for x in nested for y in x]
来源：http://qu.muxihuayi.cn

[U09] Py：字典取最大值的键
来源：http://ji.hahajie.cn

max(d, key=d.get)
来源：http://va.hnjuh.cn

[U10] Py：按值排序字典
来源：http://up.hahajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cz.bjjhwx.cn

[U11] Py：生成器表达式
来源：http://vz.huixinmuqiang.cn

(x * 2 for x in arr)
来源：http://xh.bjjhwx.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xy.hahajie.cn

Counter(arr).most_common(3)
来源：http://mo.gzmigu.cn

[U13] Py：固定长度队列
来源：http://vx.jctech888.com.cn

deque(maxlen=10)
来源：http://ey.nszjky.cn

[U14] Py：分组收集到列表
来源：http://hr.nszjky.cn

defaultdict(list)
来源：http://ua.huanxung.cn

[U15] Py：高精度计时
来源：http://oz.bjjhwx.cn

t = time.perf_counter()
来源：http://lz.wgjwhj.cn

[U16] Py：命令行参数解析
来源：http://ps.huixiangedu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dk.bjjhwx.cn

[U17] Py：初始化日志
来源：http://zj.haigaiapp.cn

logging.basicConfig(level=logging.INFO)
来源：http://xt.haigaiapp.cn

[U18] Py：预编译正则
来源：http://sm.bookmarksfly.cn

pat = re.compile(r"\d+")
来源：http://yj.shtwfgs.cn

[U19] Py：正则替换带回调
来源：http://ob.shtwfgs.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rw.bookmarksfly.cn

[U20] Py：缓存函数结果
来源：http://jl.colortex.cn

@functools.lru_cache(maxsize=None)
来源：http://ne.shxzukj.cn

[U21] Py：自定义上下文管理器
来源：http://jx.shxzskj.cn

@contextlib.contextmanager
来源：http://cf.panjiajie.cn

[U22] Py：矩阵转置
来源：http://im.huixinmuqiang.cn

list(zip(*m))
来源：http://fj.huanxung.cn

[U23] Py：分块读取大文件
来源：http://ur.muxihuayi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ap.nicolike.cn

[U24] Py：路径操作
来源：http://pm.szsharing.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xk.9csxet.cn

[U25] Py：CSV 按字典读
来源：http://bn.huixiangedu.cn

csv.DictReader(f)
来源：http://hr.newstarts.cn

[U26] Py：并发下载
来源：http://lq.szsharing.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://um.haigaiapp.cn

[U27] Py：异步 HTTP
来源：http://fs.colortex.cn

aiohttp.ClientSession() 配合 async with
来源：http://qm.bookmarksfly.cn

[U28] Py：类型别名
来源：http://qt.hahajie.cn

UserId = int
来源：http://by.shtwfgs.cn

[U29] Py：属性校验
来源：http://tg.hahajie.cn

@property 与 @x.setter 配合
来源：http://xz.muxihuayi.cn

[U30] Py：数据类
来源：http://pe.chemitech.net.cn

@dataclass(slots=True)
来源：http://jh.nicolike.cn

[U31] Py：单测
来源：http://tq.9csxet.cn

python -m pytest -q
来源：http://qh.shxzukj.cn

[U32] Py：代码格式化
来源：http://nt.huixinmuqiang.cn

ruff format . && ruff check --fix .
来源：http://jy.jctech888.com.cn

[U33] Py：打包发布
来源：http://bz.shtwfgs.cn

python -m build  （依赖 pyproject.toml）
来源：http://xm.bjjhwx.cn

[U34] Py：判断编码
来源：http://ow.yuexingan06.cn

chardet.detect(raw)
来源：http://bp.colortex.cn

[U35] Py：发送邮件
来源：http://ij.gzmigu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://uh.nszjky.cn

[U36] Py：定时任务
来源：http://nk.panjiajie.cn

schedule.every(10).minutes.do(job)
来源：http://un.huanxung.cn

[U37] Py：读写 Excel
来源：http://zt.shxzskj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://zn.nszjky.cn

[U38] Py：获取脚本所在目录
来源：http://of.521024.cn

Path(__file__).resolve().parent
来源：http://pz.lnxyls.cn

[U39] Py：判断是否在交互环境
来源：http://ar.lnxyls.cn

sys.stdout.isatty()
来源：http://rw.9csxet.cn

[U40] Py：打印到标准错误
来源：http://hj.hnjuh.cn

print("err", file=sys.stderr)
来源：http://yw.shxzukj.cn

[U41] PHP：初始化 Composer 项目
来源：http://jd.hahajie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://pg.9csxet.cn

[U42] PHP：PSR-4 自动加载
来源：http://tl.hahajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://uw.jctech888.com.cn

[U43] PHP：声明命名空间
来源：http://kg.huixinmuqiang.cn

namespace App\Http;
来源：http://cu.9csxet.cn

[U44] PHP：开启严格类型
来源：http://va.jctech888.com.cn

declare(strict_types=1);
来源：http://ct.haigaiapp.cn

[U45] PHP：类型声明与返回类型
来源：http://ej.hahajie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://yu.colortex.cn

[U46] PHP：可空类型
来源：http://fz.gzmigu.cn

?string $name = null
来源：http://az.9csxet.cn

[U47] PHP：联合类型
来源：http://no.muxihuayi.cn

int|string $id
来源：http://bs.yuexingan06.cn

[U48] PHP：纯枚举
来源：http://yk.yuntaijiaju.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xb.521024.cn

[U49] PHP：只读属性
来源：http://vy.lnxyls.cn

public readonly string $name
来源：http://oz.newstarts.cn

[U50] PHP：构造器属性提升
来源：http://gu.chemitech.net.cn

public function __construct(private int $id) {}
来源：http://pw.muxihuayi.cn

[U51] PHP：数组解构
来源：http://cy.yuntaijiaju.cn

[$a, $b] = $arr;
来源：http://pk.newstarts.cn

[U52] PHP：箭头函数
来源：http://zn.haigaiapp.cn

$double = fn($x) => $x * 2;
来源：http://bm.newstarts.cn

[U53] PHP：空合并运算符
来源：http://zo.newstarts.cn

$v = $a ?? $b ?? "default";
来源：http://eg.chemitech.net.cn

[U54] PHP：空安全调用
来源：http://td.nszjky.cn

$obj?->method()
来源：http://uf.shxzskj.cn

[U55] PHP：match 表达式
来源：http://rx.bjjhwx.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://sc.bookmarksfly.cn

[U56] PHP：命名参数
来源：http://wp.wgjwhj.cn

f(a: 1, b: 2)
来源：http://do.521024.cn

[U57] PHP：字符串插值
来源：http://la.shxzskj.cn

"值: {$a}"
来源：http://uk.szsharing.cn

[U58] PHP：数组三件套
来源：http://od.jctech888.com.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fz.huixiangedu.cn

[U59] PHP：自定义排序
来源：http://vb.asd995.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://im.yuexingan06.cn

[U60] PHP：JSON 编解码
来源：http://xe.szxytkj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wo.jianghongdianzi.cn

[U61] PHP：正则
来源：http://iu.jctech888.com.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bg.bookmarksfly.cn

[U62] PHP：日期对象
来源：http://io.huanxung.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://oo.shxzskj.cn

[U63] PHP：文件读写
来源：http://zb.panjiajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bo.hahajie.cn

[U64] PHP：目录遍历
来源：http://zn.nszjky.cn

glob("dir/*.php");  scandir("dir");
来源：http://ml.nicolike.cn

[U65] PHP：会话
来源：http://vm.wgjwhj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ra.yuntaijiaju.cn

[U66] PHP：设置 Cookie
来源：http://fp.chemitech.net.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mc.9csxet.cn

[U67] PHP：处理文件上传
来源：http://xc.chemitech.net.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ey.hahajie.cn

[U68] PHP：PDO 连接
来源：http://gk.shtwfgs.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ou.jianghongdianzi.cn

[U69] PHP：PDO 预处理
来源：http://ui.521024.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ln.lnxyls.cn

[U70] PHP：PDO 事务
来源：http://jf.jianghongdianzi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://eq.bookmarksfly.cn

[U71] PHP：抛出异常
来源：http://io.szxytkj.cn

throw new RuntimeException("失败", 500);
来源：http://pq.chemitech.net.cn

[U72] PHP：写错误日志
来源：http://gj.bjjhwx.cn

error_log("失败: " . $e->getMessage());
来源：http://wx.gzmigu.cn

[U73] PHP：读取 ini 配置
来源：http://qo.jianghongdianzi.cn

parse_ini_file("config.ini", true)
来源：http://sv.jianghongdianzi.cn

[U74] PHP：读取环境变量
来源：http://uf.jctech888.com.cn

getenv("APP_ENV") ?: "production"
来源：http://gc.hahajie.cn

[U75] PHP：依赖注入
来源：http://uc.shxzukj.cn

composer require psr/container
来源：http://jj.newstarts.cn

[U76] PHP：简单路由
来源：http://dc.hnjuh.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://am.huixiangedu.cn

[U77] PHP：模板渲染
来源：http://ip.bjjhwx.cn

composer require twig/twig
来源：http://yf.lnxyls.cn

[U78] PHP：单元测试
来源：http://jk.asd995.cn

composer require --dev phpunit/phpunit
来源：http://xq.asd995.cn

[U79] PHP：静态分析
来源：http://tp.9csxet.cn

composer require --dev phpstan/phpstan
来源：http://ze.haigaiapp.cn

[U80] PHP：代码规范修复
来源：http://sx.panjiajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://cj.haigaiapp.cn

[U81] JS：初始化项目
来源：http://cj.yuntaijiaju.cn

npm init -y;  npm i express
来源：http://ju.hahajie.cn

[U82] JS：package.json 脚本
来源：http://fe.lnxyls.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kz.hahajie.cn

[U83] JS：ES Module 导入导出
来源：http://ji.lnxyls.cn

export const a = 1;  import { a } from "./m.js";
来源：http://lj.wgjwhj.cn

[U84] JS：CommonJS 写法
来源：http://fn.9csxet.cn

module.exports = { a };  const { a } = require("./m");
来源：http://df.szxytkj.cn

[U85] JS：可选链
来源：http://ts.muxihuayi.cn

a?.b?.c
来源：http://zm.panjiajie.cn

[U86] JS：空值合并
来源：http://pc.shxzskj.cn

a ?? b
来源：http://mp.hnjuh.cn

[U87] JS：解构默认值
来源：http://ii.szxytkj.cn

const { a = 1, b = 2 } = obj;
来源：http://wc.bookmarksfly.cn

[U88] JS：对象展开合并
来源：http://rr.bookmarksfly.cn

{ ...a, ...b }
来源：http://xm.shxzukj.cn

[U89] JS：数组去重
来源：http://gc.521024.cn

[...new Set(arr)]
来源：http://yo.lnxyls.cn

[U90] JS：数字数组排序
来源：http://xp.nicolike.cn

[...arr].sort((a, b) => a - b)
来源：http://wi.bjjhwx.cn

[U91] JS：对象键值遍历
来源：http://vs.shxzukj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ox.huixinmuqiang.cn

[U92] JS：深拷贝
来源：http://os.shxzukj.cn

structuredClone(obj)
来源：http://gi.panjiajie.cn

[U93] JS：模板字符串
来源：http://ws.hahajie.cn

`共 ${n} 条`
来源：http://rw.jianghongdianzi.cn

[U94] JS：箭头函数
来源：http://iu.gzmigu.cn

const double = x => x * 2;
来源：http://mg.huixinmuqiang.cn

[U95] JS：Promise 包装
来源：http://li.nicolike.cn

new Promise((resolve, reject) => {})
来源：http://mg.hnjuh.cn

[U96] JS：async/await 与异常
来源：http://gt.huixinmuqiang.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mi.521024.cn

[U97] JS：并发请求
来源：http://qq.haigaiapp.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://kk.asd995.cn

[U98] JS：fetch 带 JSON
来源：http://el.yuexingan06.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kz.haigaiapp.cn

[U99] JS：事件监听
来源：http://kp.haigaiapp.cn

el.addEventListener("click", e => {})
来源：http://yk.nicolike.cn

[U100] JS：DOM 查询
来源：http://tn.nszjky.cn

document.querySelector(".item")
来源：http://dz.shxzskj.cn

[U101] JS：classList 操作
来源：http://jv.hahajie.cn

el.classList.toggle("active")
来源：http://ow.szsharing.cn

[U102] JS：本地存储
来源：http://pp.chemitech.net.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://mp.hahajie.cn

[U103] JS：定时器
来源：http://fh.yuntaijiaju.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dw.nszjky.cn

[U104] JS：防抖
来源：http://eh.hnjuh.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jd.huixiangedu.cn

[U105] JS：节流
来源：http://jq.panjiajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ck.jianghongdianzi.cn

[U106] JS：日期格式化
来源：http://ch.chemitech.net.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ij.yuntaijiaju.cn


<!-- 参考信息 -->