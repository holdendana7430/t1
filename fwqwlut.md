代发 wailian999

[T21] Swift：遍历
来源：http://mn.bookmarksfly.cn

for x in a { print(x) }
来源：http://kx.yuexingan06.cn

[T22] Swift：字典
来源：http://on.bjjhwx.cn

var d = ["a": 1];  d["b"] = 2
来源：http://iq.newstarts.cn

[T23] Swift：函数
来源：http://je.muxihuayi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vz.colortex.cn

[T24] Swift：闭包
来源：http://ar.muxihuayi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qm.hahajie.cn

[T25] Swift：结构体
来源：http://uv.lnxyls.cn

struct P { var x: Int }
来源：http://dz.haigaiapp.cn

[T26] Swift：类与重写
来源：http://dj.bookmarksfly.cn

class A: Base { override func f() {} }
来源：http://zq.newstarts.cn

[T27] Swift：错误处理
来源：http://kd.szsharing.cn

do { try f() } catch { print(error) }
来源：http://ph.521024.cn

[T28] Swift：枚举
来源：http://pm.shxzukj.cn

enum Color { case red, green }
来源：http://qs.bookmarksfly.cn

[T29] Swift：guard 提前返回
来源：http://fy.wgjwhj.cn

guard let x = opt else { return }
来源：http://hj.asd995.cn

[T30] Swift：协议
来源：http://pc.yuexingan06.cn

protocol Shape { func area() -> Double }
来源：http://ni.huixinmuqiang.cn

[T31] Lua：Hello World
来源：http://du.bookmarksfly.cn

print("Hello")
来源：http://qz.wgjwhj.cn

[T32] Lua：局部变量
来源：http://ae.nicolike.cn

local a = 1
来源：http://jk.shtwfgs.cn

[T33] Lua：表（数组）
来源：http://ol.asd995.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://os.yuntaijiaju.cn

[T34] Lua：遍历表
来源：http://nz.jianghongdianzi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://dg.9csxet.cn

[T35] Lua：字典表
来源：http://jy.nszjky.cn

local d = { a = 1 };  d.b = 2
来源：http://ju.huixinmuqiang.cn

[T36] Lua：函数
来源：http://uq.wgjwhj.cn

function add(a, b) return a + b end
来源：http://ei.shxzskj.cn

[T37] Lua：字符串拼接
来源：http://eg.colortex.cn

"a" .. "b"
来源：http://hw.haigaiapp.cn

[T38] Lua：条件
来源：http://ov.yuntaijiaju.cn

if x > 0 then print("正") end
来源：http://xe.huanxung.cn

[T39] Lua：模式匹配
来源：http://rp.newstarts.cn

string.find(s, "%d+")
来源：http://bk.521024.cn

[T40] Lua：元表
来源：http://wi.szxytkj.cn

setmetatable({}, { __index = base })
来源：http://ek.bookmarksfly.cn

[T41] Perl：Hello World
来源：http://sb.chemitech.net.cn

print "Hello\n";
来源：http://cf.huixiangedu.cn

[T42] Perl：变量类型
来源：http://dq.9csxet.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jg.chemitech.net.cn

[T43] Perl：字符串插值
来源：http://ak.colortex.cn

"值: $a"
来源：http://gd.nszjky.cn

[T44] Perl：条件
来源：http://km.muxihuayi.cn

if ($a > 0) { print "正"; }
来源：http://gh.nszjky.cn

[T45] Perl：数组遍历
来源：http://ru.bjjhwx.cn

for my $x (@arr) { print $x; }
来源：http://rv.huixiangedu.cn

[T46] Perl：哈希操作
来源：http://mc.shxzukj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mz.yuexingan06.cn

[T47] Perl：正则捕获
来源：http://cy.panjiajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pm.9csxet.cn

[T48] Perl：正则替换
来源：http://qy.yuexingan06.cn

$s =~ s/old/new/g;
来源：http://ua.bookmarksfly.cn

[T49] Perl：函数
来源：http://gn.newstarts.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ox.yuntaijiaju.cn

[T50] Perl：逐行读文件
来源：http://or.jctech888.com.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://bt.muxihuayi.cn

while (my $line = <$fh>) { print $line; }
来源：http://vq.bjjhwx.cn

[T51] Scala：Hello World
来源：http://mm.colortex.cn

println("Hello")
来源：http://tr.bjjhwx.cn

[T52] Scala：变量
来源：http://ko.newstarts.cn

val a = 1;  var b = 2
来源：http://xp.gzmigu.cn

[T53] Scala：字符串插值
来源：http://uc.huanxung.cn

s"值: $b"
来源：http://ld.jctech888.com.cn

[T54] Scala：集合映射
来源：http://np.huixiangedu.cn

List(1, 2, 3).map(_ * 2)
来源：http://qg.huanxung.cn

[T55] Scala：集合过滤
来源：http://yl.yuntaijiaju.cn

List(1, 2, 3).filter(_ > 1)
来源：http://rs.colortex.cn

[T56] Scala：样例类
来源：http://jf.shxzukj.cn

case class User(name: String, age: Int)
来源：http://lt.szxytkj.cn

[T57] Scala：模式匹配
来源：http://ot.newstarts.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://kf.shtwfgs.cn

[T58] Scala：函数定义
来源：http://lj.nicolike.cn

def add(a: Int, b: Int): Int = a + b
来源：http://we.szsharing.cn

[T59] Scala：循环
来源：http://as.hahajie.cn

for (i <- 1 to 10) println(i)
来源：http://hh.hahajie.cn

[T60] Scala：折叠
来源：http://qr.muxihuayi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ot.gzmigu.cn

================================================================================
来源：http://go.newstarts.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tl.yuexingan06.cn

================================================================================
来源：http://yr.panjiajie.cn

[U01] Py：创建虚拟环境
来源：http://mh.colortex.cn

python -m venv .venv && source .venv/bin/activate
来源：http://so.asd995.cn

[U02] Py：导出 / 安装依赖
来源：http://jx.colortex.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wj.asd995.cn

[U03] Py：加载 .env 配置
来源：http://jb.shxzskj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://kn.haigaiapp.cn

[U04] Py：变量调试打印
来源：http://zl.nicolike.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gm.shtwfgs.cn

[U05] Py：列表去重且保序
来源：http://qk.521024.cn

list(dict.fromkeys(arr))
来源：http://ka.shtwfgs.cn

[U06] Py：合并两个字典
来源：http://yk.gzmigu.cn

{**a, **b}
来源：http://hk.bjjhwx.cn

[U07] Py：反转字典键值
来源：http://zu.shtwfgs.cn

{v: k for k, v in d.items()}
来源：http://gg.asd995.cn

[U08] Py：展平二维列表
来源：http://xq.wgjwhj.cn

[y for x in nested for y in x]
来源：http://hn.shxzskj.cn

[U09] Py：字典取最大值的键
来源：http://tk.nszjky.cn

max(d, key=d.get)
来源：http://ts.haigaiapp.cn

[U10] Py：按值排序字典
来源：http://yu.szxytkj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rq.huixinmuqiang.cn

[U11] Py：生成器表达式
来源：http://wn.colortex.cn

(x * 2 for x in arr)
来源：http://ly.shxzskj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ft.jianghongdianzi.cn

Counter(arr).most_common(3)
来源：http://sv.hnjuh.cn

[U13] Py：固定长度队列
来源：http://qe.huixinmuqiang.cn

deque(maxlen=10)
来源：http://sx.newstarts.cn

[U14] Py：分组收集到列表
来源：http://ed.nszjky.cn

defaultdict(list)
来源：http://ny.hnjuh.cn

[U15] Py：高精度计时
来源：http://bm.lnxyls.cn

t = time.perf_counter()
来源：http://lr.panjiajie.cn

[U16] Py：命令行参数解析
来源：http://ta.hahajie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ch.muxihuayi.cn

[U17] Py：初始化日志
来源：http://tz.wgjwhj.cn

logging.basicConfig(level=logging.INFO)
来源：http://tn.szsharing.cn

[U18] Py：预编译正则
来源：http://ze.bjjhwx.cn

pat = re.compile(r"\d+")
来源：http://kq.huixiangedu.cn

[U19] Py：正则替换带回调
来源：http://sp.9csxet.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yz.9csxet.cn

[U20] Py：缓存函数结果
来源：http://ff.hahajie.cn

@functools.lru_cache(maxsize=None)
来源：http://zu.huixinmuqiang.cn

[U21] Py：自定义上下文管理器
来源：http://ns.huixiangedu.cn

@contextlib.contextmanager
来源：http://xy.nszjky.cn

[U22] Py：矩阵转置
来源：http://aj.muxihuayi.cn

list(zip(*m))
来源：http://hw.colortex.cn

[U23] Py：分块读取大文件
来源：http://pr.muxihuayi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hh.9csxet.cn

[U24] Py：路径操作
来源：http://zq.asd995.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://sy.hnjuh.cn

[U25] Py：CSV 按字典读
来源：http://vg.bjjhwx.cn

csv.DictReader(f)
来源：http://oe.panjiajie.cn

[U26] Py：并发下载
来源：http://jo.bookmarksfly.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://et.haigaiapp.cn

[U27] Py：异步 HTTP
来源：http://qq.jctech888.com.cn

aiohttp.ClientSession() 配合 async with
来源：http://mc.521024.cn

[U28] Py：类型别名
来源：http://ce.nszjky.cn

UserId = int
来源：http://ir.jctech888.com.cn

[U29] Py：属性校验
来源：http://jj.gzmigu.cn

@property 与 @x.setter 配合
来源：http://ft.bjjhwx.cn

[U30] Py：数据类
来源：http://hy.colortex.cn

@dataclass(slots=True)
来源：http://kj.hnjuh.cn

[U31] Py：单测
来源：http://vp.jianghongdianzi.cn

python -m pytest -q
来源：http://oi.bookmarksfly.cn

[U32] Py：代码格式化
来源：http://ss.lnxyls.cn

ruff format . && ruff check --fix .
来源：http://pe.panjiajie.cn

[U33] Py：打包发布
来源：http://yh.bjjhwx.cn

python -m build  （依赖 pyproject.toml）
来源：http://fj.panjiajie.cn

[U34] Py：判断编码
来源：http://xg.9csxet.cn

chardet.detect(raw)
来源：http://sg.yuexingan06.cn

[U35] Py：发送邮件
来源：http://ce.muxihuayi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://oj.haigaiapp.cn

[U36] Py：定时任务
来源：http://bb.colortex.cn

schedule.every(10).minutes.do(job)
来源：http://hq.yuntaijiaju.cn

[U37] Py：读写 Excel
来源：http://qk.shxzskj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://vv.shtwfgs.cn

[U38] Py：获取脚本所在目录
来源：http://bi.huixiangedu.cn

Path(__file__).resolve().parent
来源：http://sn.bjjhwx.cn

[U39] Py：判断是否在交互环境
来源：http://xp.bookmarksfly.cn

sys.stdout.isatty()
来源：http://hz.haigaiapp.cn

[U40] Py：打印到标准错误
来源：http://by.shxzukj.cn

print("err", file=sys.stderr)
来源：http://ax.newstarts.cn

[U41] PHP：初始化 Composer 项目
来源：http://cv.gzmigu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://pk.jctech888.com.cn

[U42] PHP：PSR-4 自动加载
来源：http://qw.wgjwhj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dz.huanxung.cn

[U43] PHP：声明命名空间
来源：http://im.jianghongdianzi.cn

namespace App\Http;
来源：http://jr.nicolike.cn

[U44] PHP：开启严格类型
来源：http://az.huixiangedu.cn

declare(strict_types=1);
来源：http://qi.bookmarksfly.cn

[U45] PHP：类型声明与返回类型
来源：http://wf.jianghongdianzi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://au.huixinmuqiang.cn

[U46] PHP：可空类型
来源：http://ug.asd995.cn

?string $name = null
来源：http://uu.gzmigu.cn

[U47] PHP：联合类型
来源：http://an.lnxyls.cn

int|string $id
来源：http://qt.9csxet.cn

[U48] PHP：纯枚举
来源：http://hn.yuexingan06.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ou.asd995.cn

[U49] PHP：只读属性
来源：http://wz.hahajie.cn

public readonly string $name
来源：http://ex.nszjky.cn

[U50] PHP：构造器属性提升
来源：http://tz.9csxet.cn

public function __construct(private int $id) {}
来源：http://ek.hahajie.cn

[U51] PHP：数组解构
来源：http://ft.yuexingan06.cn

[$a, $b] = $arr;
来源：http://on.wgjwhj.cn

[U52] PHP：箭头函数
来源：http://nl.nszjky.cn

$double = fn($x) => $x * 2;
来源：http://ai.bjjhwx.cn

[U53] PHP：空合并运算符
来源：http://uw.colortex.cn

$v = $a ?? $b ?? "default";
来源：http://yi.hahajie.cn

[U54] PHP：空安全调用
来源：http://vp.shxzskj.cn

$obj?->method()
来源：http://mt.chemitech.net.cn

[U55] PHP：match 表达式
来源：http://tc.huanxung.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bc.9csxet.cn

[U56] PHP：命名参数
来源：http://fj.shxzskj.cn

f(a: 1, b: 2)
来源：http://jg.wgjwhj.cn

[U57] PHP：字符串插值
来源：http://bo.szxytkj.cn

"值: {$a}"
来源：http://ta.huanxung.cn

[U58] PHP：数组三件套
来源：http://eb.shxzskj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qw.jianghongdianzi.cn

[U59] PHP：自定义排序
来源：http://br.yuntaijiaju.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ze.shxzskj.cn

[U60] PHP：JSON 编解码
来源：http://og.bjjhwx.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pd.panjiajie.cn

[U61] PHP：正则
来源：http://lw.shxzskj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hl.newstarts.cn

[U62] PHP：日期对象
来源：http://tu.chemitech.net.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zq.panjiajie.cn

[U63] PHP：文件读写
来源：http://wp.huixiangedu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://li.shtwfgs.cn

[U64] PHP：目录遍历
来源：http://fd.chemitech.net.cn

glob("dir/*.php");  scandir("dir");
来源：http://ux.hnjuh.cn

[U65] PHP：会话
来源：http://vm.asd995.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://gl.bookmarksfly.cn

[U66] PHP：设置 Cookie
来源：http://ly.jianghongdianzi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bh.jianghongdianzi.cn

[U67] PHP：处理文件上传
来源：http://ja.chemitech.net.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://po.nicolike.cn

[U68] PHP：PDO 连接
来源：http://lg.yuntaijiaju.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lj.huixiangedu.cn

[U69] PHP：PDO 预处理
来源：http://wv.shxzskj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hb.panjiajie.cn

[U70] PHP：PDO 事务
来源：http://si.wgjwhj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://no.panjiajie.cn

[U71] PHP：抛出异常
来源：http://dc.nicolike.cn

throw new RuntimeException("失败", 500);
来源：http://af.bookmarksfly.cn

[U72] PHP：写错误日志
来源：http://zu.lnxyls.cn

error_log("失败: " . $e->getMessage());
来源：http://zb.yuexingan06.cn

[U73] PHP：读取 ini 配置
来源：http://kq.hahajie.cn

parse_ini_file("config.ini", true)
来源：http://lo.panjiajie.cn

[U74] PHP：读取环境变量
来源：http://eh.gzmigu.cn

getenv("APP_ENV") ?: "production"
来源：http://rk.huixinmuqiang.cn

[U75] PHP：依赖注入
来源：http://yl.panjiajie.cn

composer require psr/container
来源：http://gg.szxytkj.cn

[U76] PHP：简单路由
来源：http://ug.bjjhwx.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gy.colortex.cn

[U77] PHP：模板渲染
来源：http://ew.hnjuh.cn

composer require twig/twig
来源：http://dt.shxzukj.cn

[U78] PHP：单元测试
来源：http://cg.521024.cn

composer require --dev phpunit/phpunit
来源：http://fb.shtwfgs.cn

[U79] PHP：静态分析
来源：http://os.haigaiapp.cn

composer require --dev phpstan/phpstan
来源：http://uo.huanxung.cn

[U80] PHP：代码规范修复
来源：http://ge.shtwfgs.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://cr.panjiajie.cn

[U81] JS：初始化项目
来源：http://ej.wgjwhj.cn

npm init -y;  npm i express
来源：http://nc.huixinmuqiang.cn

[U82] JS：package.json 脚本
来源：http://uw.wgjwhj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ph.bjjhwx.cn

[U83] JS：ES Module 导入导出
来源：http://tk.shtwfgs.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vz.huixinmuqiang.cn

[U84] JS：CommonJS 写法
来源：http://eg.newstarts.cn

module.exports = { a };  const { a } = require("./m");
来源：http://cw.hahajie.cn

[U85] JS：可选链
来源：http://jv.gzmigu.cn

a?.b?.c
来源：http://oa.hnjuh.cn

[U86] JS：空值合并
来源：http://pd.shtwfgs.cn

a ?? b
来源：http://ht.colortex.cn

[U87] JS：解构默认值
来源：http://il.huanxung.cn

const { a = 1, b = 2 } = obj;
来源：http://ok.lnxyls.cn

[U88] JS：对象展开合并
来源：http://su.huixiangedu.cn

{ ...a, ...b }
来源：http://yc.chemitech.net.cn

[U89] JS：数组去重
来源：http://vz.shtwfgs.cn

[...new Set(arr)]
来源：http://ft.yuexingan06.cn

[U90] JS：数字数组排序
来源：http://bb.huixiangedu.cn

[...arr].sort((a, b) => a - b)
来源：http://wm.szsharing.cn

[U91] JS：对象键值遍历
来源：http://oy.521024.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://sh.bjjhwx.cn

[U92] JS：深拷贝
来源：http://py.newstarts.cn

structuredClone(obj)
来源：http://og.shtwfgs.cn

[U93] JS：模板字符串
来源：http://ng.gzmigu.cn

`共 ${n} 条`
来源：http://dp.hnjuh.cn

[U94] JS：箭头函数
来源：http://sc.9csxet.cn

const double = x => x * 2;
来源：http://ei.yuexingan06.cn

[U95] JS：Promise 包装
来源：http://xd.muxihuayi.cn

new Promise((resolve, reject) => {})
来源：http://vb.huixiangedu.cn

[U96] JS：async/await 与异常
来源：http://bh.hahajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://oi.muxihuayi.cn

[U97] JS：并发请求
来源：http://if.huixinmuqiang.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vc.bookmarksfly.cn

[U98] JS：fetch 带 JSON
来源：http://sj.asd995.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://he.yuntaijiaju.cn

[U99] JS：事件监听
来源：http://uf.huanxung.cn

el.addEventListener("click", e => {})
来源：http://yk.9csxet.cn

[U100] JS：DOM 查询
来源：http://td.gzmigu.cn

document.querySelector(".item")
来源：http://nw.muxihuayi.cn

[U101] JS：classList 操作
来源：http://yq.muxihuayi.cn

el.classList.toggle("active")
来源：http://io.chemitech.net.cn

[U102] JS：本地存储
来源：http://hb.colortex.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://by.haigaiapp.cn

[U103] JS：定时器
来源：http://ve.asd995.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ic.521024.cn

[U104] JS：防抖
来源：http://bx.shxzukj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ab.bjjhwx.cn

[U105] JS：节流
来源：http://au.chemitech.net.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wg.wgjwhj.cn

[U106] JS：日期格式化
来源：http://hg.hnjuh.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dw.wgjwhj.cn

[U107] JS：数字千分位
来源：http://hs.haigaiapp.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fi.yuexingan06.cn

[U108] JS：随机整数
来源：http://nz.lnxyls.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nq.hahajie.cn


<!-- 参考信息 -->