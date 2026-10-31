代发 wailian999

[T19] Swift：可选绑定
来源：http://ra.szsharing.cn

if let n = opt { print(n) }
来源：http://of.lnxyls.cn

[T20] Swift：数组操作
来源：http://xp.gzmigu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qt.szsharing.cn

[T21] Swift：遍历
来源：http://op.lnxyls.cn

for x in a { print(x) }
来源：http://vi.lnxyls.cn

[T22] Swift：字典
来源：http://ws.shxzskj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://bf.shxzukj.cn

[T23] Swift：函数
来源：http://ku.huixinmuqiang.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ro.shtwfgs.cn

[T24] Swift：闭包
来源：http://ak.jianghongdianzi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://nw.shxzskj.cn

[T25] Swift：结构体
来源：http://fn.muxihuayi.cn

struct P { var x: Int }
来源：http://rh.shxzukj.cn

[T26] Swift：类与重写
来源：http://hw.hahajie.cn

class A: Base { override func f() {} }
来源：http://vc.hnjuh.cn

[T27] Swift：错误处理
来源：http://tu.muxihuayi.cn

do { try f() } catch { print(error) }
来源：http://sm.bjjhwx.cn

[T28] Swift：枚举
来源：http://lf.yuntaijiaju.cn

enum Color { case red, green }
来源：http://wi.lnxyls.cn

[T29] Swift：guard 提前返回
来源：http://ed.panjiajie.cn

guard let x = opt else { return }
来源：http://dg.huixiangedu.cn

[T30] Swift：协议
来源：http://gb.wgjwhj.cn

protocol Shape { func area() -> Double }
来源：http://xy.jianghongdianzi.cn

[T31] Lua：Hello World
来源：http://qw.huixinmuqiang.cn

print("Hello")
来源：http://mp.wgjwhj.cn

[T32] Lua：局部变量
来源：http://zt.chemitech.net.cn

local a = 1
来源：http://wb.bjjhwx.cn

[T33] Lua：表（数组）
来源：http://rp.gzmigu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fp.nicolike.cn

[T34] Lua：遍历表
来源：http://mi.nszjky.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vd.nszjky.cn

[T35] Lua：字典表
来源：http://kq.huixinmuqiang.cn

local d = { a = 1 };  d.b = 2
来源：http://te.gzmigu.cn

[T36] Lua：函数
来源：http://im.chemitech.net.cn

function add(a, b) return a + b end
来源：http://uk.colortex.cn

[T37] Lua：字符串拼接
来源：http://ex.9csxet.cn

"a" .. "b"
来源：http://zr.9csxet.cn

[T38] Lua：条件
来源：http://ar.muxihuayi.cn

if x > 0 then print("正") end
来源：http://ml.szxytkj.cn

[T39] Lua：模式匹配
来源：http://nn.szsharing.cn

string.find(s, "%d+")
来源：http://vq.nszjky.cn

[T40] Lua：元表
来源：http://vg.hnjuh.cn

setmetatable({}, { __index = base })
来源：http://lz.muxihuayi.cn

[T41] Perl：Hello World
来源：http://si.gzmigu.cn

print "Hello\n";
来源：http://er.shxzskj.cn

[T42] Perl：变量类型
来源：http://ip.haigaiapp.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xz.wgjwhj.cn

[T43] Perl：字符串插值
来源：http://ek.asd995.cn

"值: $a"
来源：http://df.huanxung.cn

[T44] Perl：条件
来源：http://di.yuexingan06.cn

if ($a > 0) { print "正"; }
来源：http://ro.jianghongdianzi.cn

[T45] Perl：数组遍历
来源：http://eo.shxzukj.cn

for my $x (@arr) { print $x; }
来源：http://bh.hahajie.cn

[T46] Perl：哈希操作
来源：http://ud.gzmigu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ob.panjiajie.cn

[T47] Perl：正则捕获
来源：http://kb.bookmarksfly.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://tv.asd995.cn

[T48] Perl：正则替换
来源：http://fi.panjiajie.cn

$s =~ s/old/new/g;
来源：http://ei.nicolike.cn

[T49] Perl：函数
来源：http://nj.shtwfgs.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sr.bookmarksfly.cn

[T50] Perl：逐行读文件
来源：http://hc.hahajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://cp.shxzskj.cn

while (my $line = <$fh>) { print $line; }
来源：http://eh.haigaiapp.cn

[T51] Scala：Hello World
来源：http://sv.9csxet.cn

println("Hello")
来源：http://xn.shtwfgs.cn

[T52] Scala：变量
来源：http://mz.wgjwhj.cn

val a = 1;  var b = 2
来源：http://om.chemitech.net.cn

[T53] Scala：字符串插值
来源：http://rx.hnjuh.cn

s"值: $b"
来源：http://kt.asd995.cn

[T54] Scala：集合映射
来源：http://sh.szxytkj.cn

List(1, 2, 3).map(_ * 2)
来源：http://qq.jctech888.com.cn

[T55] Scala：集合过滤
来源：http://bg.muxihuayi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://og.asd995.cn

[T56] Scala：样例类
来源：http://ju.panjiajie.cn

case class User(name: String, age: Int)
来源：http://ze.nicolike.cn

[T57] Scala：模式匹配
来源：http://uu.bookmarksfly.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tr.haigaiapp.cn

[T58] Scala：函数定义
来源：http://xi.bjjhwx.cn

def add(a: Int, b: Int): Int = a + b
来源：http://cb.hnjuh.cn

[T59] Scala：循环
来源：http://ru.shxzskj.cn

for (i <- 1 to 10) println(i)
来源：http://kz.bookmarksfly.cn

[T60] Scala：折叠
来源：http://pl.jianghongdianzi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ej.panjiajie.cn

================================================================================
来源：http://ai.9csxet.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lf.jctech888.com.cn

================================================================================
来源：http://in.newstarts.cn

[U01] Py：创建虚拟环境
来源：http://ut.panjiajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://hz.colortex.cn

[U02] Py：导出 / 安装依赖
来源：http://qu.9csxet.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ah.szxytkj.cn

[U03] Py：加载 .env 配置
来源：http://jc.shxzskj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ln.panjiajie.cn

[U04] Py：变量调试打印
来源：http://bk.lnxyls.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ti.521024.cn

[U05] Py：列表去重且保序
来源：http://eu.huixiangedu.cn

list(dict.fromkeys(arr))
来源：http://qv.bjjhwx.cn

[U06] Py：合并两个字典
来源：http://br.colortex.cn

{**a, **b}
来源：http://ab.chemitech.net.cn

[U07] Py：反转字典键值
来源：http://an.colortex.cn

{v: k for k, v in d.items()}
来源：http://uw.shxzskj.cn

[U08] Py：展平二维列表
来源：http://eh.gzmigu.cn

[y for x in nested for y in x]
来源：http://xh.yuexingan06.cn

[U09] Py：字典取最大值的键
来源：http://os.muxihuayi.cn

max(d, key=d.get)
来源：http://mr.shxzskj.cn

[U10] Py：按值排序字典
来源：http://sv.huixinmuqiang.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uh.yuexingan06.cn

[U11] Py：生成器表达式
来源：http://uw.huanxung.cn

(x * 2 for x in arr)
来源：http://us.521024.cn

[U12] Py：取出现最多的 3 个元素
来源：http://vg.shxzskj.cn

Counter(arr).most_common(3)
来源：http://ss.yuntaijiaju.cn

[U13] Py：固定长度队列
来源：http://hh.szxytkj.cn

deque(maxlen=10)
来源：http://nz.hnjuh.cn

[U14] Py：分组收集到列表
来源：http://gs.wgjwhj.cn

defaultdict(list)
来源：http://da.shtwfgs.cn

[U15] Py：高精度计时
来源：http://pz.bookmarksfly.cn

t = time.perf_counter()
来源：http://bx.nicolike.cn

[U16] Py：命令行参数解析
来源：http://eq.bjjhwx.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sv.jctech888.com.cn

[U17] Py：初始化日志
来源：http://ri.9csxet.cn

logging.basicConfig(level=logging.INFO)
来源：http://qv.bjjhwx.cn

[U18] Py：预编译正则
来源：http://me.wgjwhj.cn

pat = re.compile(r"\d+")
来源：http://mo.nicolike.cn

[U19] Py：正则替换带回调
来源：http://is.lnxyls.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yi.asd995.cn

[U20] Py：缓存函数结果
来源：http://cw.jctech888.com.cn

@functools.lru_cache(maxsize=None)
来源：http://xd.gzmigu.cn

[U21] Py：自定义上下文管理器
来源：http://ql.szxytkj.cn

@contextlib.contextmanager
来源：http://py.521024.cn

[U22] Py：矩阵转置
来源：http://ro.shxzskj.cn

list(zip(*m))
来源：http://jd.jctech888.com.cn

[U23] Py：分块读取大文件
来源：http://mi.yuntaijiaju.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ym.colortex.cn

[U24] Py：路径操作
来源：http://gp.huixinmuqiang.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ik.muxihuayi.cn

[U25] Py：CSV 按字典读
来源：http://tu.nszjky.cn

csv.DictReader(f)
来源：http://uu.szsharing.cn

[U26] Py：并发下载
来源：http://kq.huixinmuqiang.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://le.9csxet.cn

[U27] Py：异步 HTTP
来源：http://yt.521024.cn

aiohttp.ClientSession() 配合 async with
来源：http://rc.jianghongdianzi.cn

[U28] Py：类型别名
来源：http://cg.panjiajie.cn

UserId = int
来源：http://jm.haigaiapp.cn

[U29] Py：属性校验
来源：http://hp.panjiajie.cn

@property 与 @x.setter 配合
来源：http://iw.nszjky.cn

[U30] Py：数据类
来源：http://di.haigaiapp.cn

@dataclass(slots=True)
来源：http://vv.hahajie.cn

[U31] Py：单测
来源：http://px.szxytkj.cn

python -m pytest -q
来源：http://au.muxihuayi.cn

[U32] Py：代码格式化
来源：http://fd.huixinmuqiang.cn

ruff format . && ruff check --fix .
来源：http://qp.muxihuayi.cn

[U33] Py：打包发布
来源：http://rd.shtwfgs.cn

python -m build  （依赖 pyproject.toml）
来源：http://rb.shxzskj.cn

[U34] Py：判断编码
来源：http://uj.yuexingan06.cn

chardet.detect(raw)
来源：http://mr.lnxyls.cn

[U35] Py：发送邮件
来源：http://pk.521024.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ed.lnxyls.cn

[U36] Py：定时任务
来源：http://jo.bookmarksfly.cn

schedule.every(10).minutes.do(job)
来源：http://rh.lnxyls.cn

[U37] Py：读写 Excel
来源：http://of.asd995.cn

pandas.read_excel / DataFrame.to_excel
来源：http://dd.gzmigu.cn

[U38] Py：获取脚本所在目录
来源：http://tg.panjiajie.cn

Path(__file__).resolve().parent
来源：http://ip.bookmarksfly.cn

[U39] Py：判断是否在交互环境
来源：http://fk.shxzskj.cn

sys.stdout.isatty()
来源：http://vc.bookmarksfly.cn

[U40] Py：打印到标准错误
来源：http://cg.shxzskj.cn

print("err", file=sys.stderr)
来源：http://po.bjjhwx.cn

[U41] PHP：初始化 Composer 项目
来源：http://ey.lnxyls.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://np.lnxyls.cn

[U42] PHP：PSR-4 自动加载
来源：http://vy.muxihuayi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qr.shxzukj.cn

[U43] PHP：声明命名空间
来源：http://ah.yuexingan06.cn

namespace App\Http;
来源：http://nl.gzmigu.cn

[U44] PHP：开启严格类型
来源：http://jo.bookmarksfly.cn

declare(strict_types=1);
来源：http://ps.newstarts.cn

[U45] PHP：类型声明与返回类型
来源：http://ra.chemitech.net.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ve.521024.cn

[U46] PHP：可空类型
来源：http://fz.bookmarksfly.cn

?string $name = null
来源：http://ch.panjiajie.cn

[U47] PHP：联合类型
来源：http://gg.nszjky.cn

int|string $id
来源：http://dr.newstarts.cn

[U48] PHP：纯枚举
来源：http://ya.wgjwhj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gm.shtwfgs.cn

[U49] PHP：只读属性
来源：http://pv.bjjhwx.cn

public readonly string $name
来源：http://zy.gzmigu.cn

[U50] PHP：构造器属性提升
来源：http://dy.nicolike.cn

public function __construct(private int $id) {}
来源：http://or.szxytkj.cn

[U51] PHP：数组解构
来源：http://bs.colortex.cn

[$a, $b] = $arr;
来源：http://ip.shxzskj.cn

[U52] PHP：箭头函数
来源：http://ts.shxzukj.cn

$double = fn($x) => $x * 2;
来源：http://qn.wgjwhj.cn

[U53] PHP：空合并运算符
来源：http://qx.lnxyls.cn

$v = $a ?? $b ?? "default";
来源：http://po.nszjky.cn

[U54] PHP：空安全调用
来源：http://nw.jianghongdianzi.cn

$obj?->method()
来源：http://pi.asd995.cn

[U55] PHP：match 表达式
来源：http://lo.lnxyls.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://aq.muxihuayi.cn

[U56] PHP：命名参数
来源：http://wb.jianghongdianzi.cn

f(a: 1, b: 2)
来源：http://js.nszjky.cn

[U57] PHP：字符串插值
来源：http://tt.chemitech.net.cn

"值: {$a}"
来源：http://dp.shxzskj.cn

[U58] PHP：数组三件套
来源：http://ga.nicolike.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mm.huixinmuqiang.cn

[U59] PHP：自定义排序
来源：http://qv.hnjuh.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ok.hahajie.cn

[U60] PHP：JSON 编解码
来源：http://vz.lnxyls.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://to.szsharing.cn

[U61] PHP：正则
来源：http://ne.hahajie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fc.szsharing.cn

[U62] PHP：日期对象
来源：http://tz.hnjuh.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fl.bookmarksfly.cn

[U63] PHP：文件读写
来源：http://rq.huanxung.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nx.yuntaijiaju.cn

[U64] PHP：目录遍历
来源：http://ed.panjiajie.cn

glob("dir/*.php");  scandir("dir");
来源：http://sw.shxzukj.cn

[U65] PHP：会话
来源：http://qr.muxihuayi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ym.shxzskj.cn

[U66] PHP：设置 Cookie
来源：http://dr.yuexingan06.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lw.lnxyls.cn

[U67] PHP：处理文件上传
来源：http://ul.nicolike.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hx.gzmigu.cn

[U68] PHP：PDO 连接
来源：http://sh.nicolike.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hv.shxzukj.cn

[U69] PHP：PDO 预处理
来源：http://cf.szxytkj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nk.jianghongdianzi.cn

[U70] PHP：PDO 事务
来源：http://dd.9csxet.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ax.shtwfgs.cn

[U71] PHP：抛出异常
来源：http://ef.yuntaijiaju.cn

throw new RuntimeException("失败", 500);
来源：http://ul.bjjhwx.cn

[U72] PHP：写错误日志
来源：http://nm.colortex.cn

error_log("失败: " . $e->getMessage());
来源：http://vx.nicolike.cn

[U73] PHP：读取 ini 配置
来源：http://rb.521024.cn

parse_ini_file("config.ini", true)
来源：http://bo.colortex.cn

[U74] PHP：读取环境变量
来源：http://ve.shxzukj.cn

getenv("APP_ENV") ?: "production"
来源：http://si.muxihuayi.cn

[U75] PHP：依赖注入
来源：http://vg.nicolike.cn

composer require psr/container
来源：http://bj.huixiangedu.cn

[U76] PHP：简单路由
来源：http://xt.szsharing.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pj.shxzskj.cn

[U77] PHP：模板渲染
来源：http://rq.shxzskj.cn

composer require twig/twig
来源：http://sy.huixinmuqiang.cn

[U78] PHP：单元测试
来源：http://zg.huanxung.cn

composer require --dev phpunit/phpunit
来源：http://hn.newstarts.cn

[U79] PHP：静态分析
来源：http://am.shxzskj.cn

composer require --dev phpstan/phpstan
来源：http://ib.shxzskj.cn

[U80] PHP：代码规范修复
来源：http://lk.gzmigu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://uf.chemitech.net.cn

[U81] JS：初始化项目
来源：http://zy.hahajie.cn

npm init -y;  npm i express
来源：http://qt.shtwfgs.cn

[U82] JS：package.json 脚本
来源：http://lr.huixiangedu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nz.shtwfgs.cn

[U83] JS：ES Module 导入导出
来源：http://as.newstarts.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qj.colortex.cn

[U84] JS：CommonJS 写法
来源：http://vh.hahajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://pe.jianghongdianzi.cn

[U85] JS：可选链
来源：http://vl.jianghongdianzi.cn

a?.b?.c
来源：http://kl.szxytkj.cn

[U86] JS：空值合并
来源：http://kf.nszjky.cn

a ?? b
来源：http://wr.szxytkj.cn

[U87] JS：解构默认值
来源：http://qx.nszjky.cn

const { a = 1, b = 2 } = obj;
来源：http://bi.huanxung.cn

[U88] JS：对象展开合并
来源：http://uv.gzmigu.cn

{ ...a, ...b }
来源：http://hc.shtwfgs.cn

[U89] JS：数组去重
来源：http://qc.huanxung.cn

[...new Set(arr)]
来源：http://qe.yuntaijiaju.cn

[U90] JS：数字数组排序
来源：http://sh.nicolike.cn

[...arr].sort((a, b) => a - b)
来源：http://gg.huixinmuqiang.cn

[U91] JS：对象键值遍历
来源：http://pf.wgjwhj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ar.colortex.cn

[U92] JS：深拷贝
来源：http://so.9csxet.cn

structuredClone(obj)
来源：http://lk.jianghongdianzi.cn

[U93] JS：模板字符串
来源：http://xz.hnjuh.cn

`共 ${n} 条`
来源：http://si.yuexingan06.cn

[U94] JS：箭头函数
来源：http://vl.chemitech.net.cn

const double = x => x * 2;
来源：http://su.shxzukj.cn

[U95] JS：Promise 包装
来源：http://lv.shxzskj.cn

new Promise((resolve, reject) => {})
来源：http://lt.bookmarksfly.cn

[U96] JS：async/await 与异常
来源：http://of.panjiajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gh.asd995.cn

[U97] JS：并发请求
来源：http://hi.bjjhwx.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qn.hnjuh.cn

[U98] JS：fetch 带 JSON
来源：http://da.szsharing.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mj.jianghongdianzi.cn

[U99] JS：事件监听
来源：http://jp.jianghongdianzi.cn

el.addEventListener("click", e => {})
来源：http://cc.shxzskj.cn

[U100] JS：DOM 查询
来源：http://ad.bookmarksfly.cn

document.querySelector(".item")
来源：http://uu.asd995.cn

[U101] JS：classList 操作
来源：http://iz.asd995.cn

el.classList.toggle("active")
来源：http://um.hnjuh.cn

[U102] JS：本地存储
来源：http://pq.wgjwhj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://tc.lnxyls.cn

[U103] JS：定时器
来源：http://rf.haigaiapp.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yq.wgjwhj.cn

[U104] JS：防抖
来源：http://ca.huanxung.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cz.hahajie.cn

[U105] JS：节流
来源：http://jq.jctech888.com.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mx.jctech888.com.cn

[U106] JS：日期格式化
来源：http://nu.huixinmuqiang.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ek.wgjwhj.cn


<!-- 参考信息 -->