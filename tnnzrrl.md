代发 wailian999

[T25] Swift：结构体
来源：http://uf.wgjwhj.cn

struct P { var x: Int }
来源：http://aj.hahajie.cn

[T26] Swift：类与重写
来源：http://yd.yuexingan06.cn

class A: Base { override func f() {} }
来源：http://if.hahajie.cn

[T27] Swift：错误处理
来源：http://nm.nicolike.cn

do { try f() } catch { print(error) }
来源：http://hn.chemitech.net.cn

[T28] Swift：枚举
来源：http://mp.huixiangedu.cn

enum Color { case red, green }
来源：http://af.panjiajie.cn

[T29] Swift：guard 提前返回
来源：http://yf.haigaiapp.cn

guard let x = opt else { return }
来源：http://ni.huanxung.cn

[T30] Swift：协议
来源：http://ao.szxytkj.cn

protocol Shape { func area() -> Double }
来源：http://ge.gzmigu.cn

[T31] Lua：Hello World
来源：http://ib.huixinmuqiang.cn

print("Hello")
来源：http://nt.nszjky.cn

[T32] Lua：局部变量
来源：http://uz.wgjwhj.cn

local a = 1
来源：http://hf.jianghongdianzi.cn

[T33] Lua：表（数组）
来源：http://we.newstarts.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ig.nszjky.cn

[T34] Lua：遍历表
来源：http://ng.jianghongdianzi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ll.521024.cn

[T35] Lua：字典表
来源：http://jy.huixiangedu.cn

local d = { a = 1 };  d.b = 2
来源：http://ap.wgjwhj.cn

[T36] Lua：函数
来源：http://mm.muxihuayi.cn

function add(a, b) return a + b end
来源：http://fz.szsharing.cn

[T37] Lua：字符串拼接
来源：http://vj.haigaiapp.cn

"a" .. "b"
来源：http://js.shxzukj.cn

[T38] Lua：条件
来源：http://jh.shxzskj.cn

if x > 0 then print("正") end
来源：http://yj.newstarts.cn

[T39] Lua：模式匹配
来源：http://cd.nicolike.cn

string.find(s, "%d+")
来源：http://aw.9csxet.cn

[T40] Lua：元表
来源：http://ds.szsharing.cn

setmetatable({}, { __index = base })
来源：http://zy.shxzskj.cn

[T41] Perl：Hello World
来源：http://nf.szxytkj.cn

print "Hello\n";
来源：http://yo.lnxyls.cn

[T42] Perl：变量类型
来源：http://bu.szsharing.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mz.muxihuayi.cn

[T43] Perl：字符串插值
来源：http://ov.lnxyls.cn

"值: $a"
来源：http://pi.szsharing.cn

[T44] Perl：条件
来源：http://ng.haigaiapp.cn

if ($a > 0) { print "正"; }
来源：http://qw.nszjky.cn

[T45] Perl：数组遍历
来源：http://ov.yuexingan06.cn

for my $x (@arr) { print $x; }
来源：http://mr.9csxet.cn

[T46] Perl：哈希操作
来源：http://ma.wgjwhj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cm.wgjwhj.cn

[T47] Perl：正则捕获
来源：http://kh.9csxet.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://nu.hahajie.cn

[T48] Perl：正则替换
来源：http://xv.huixinmuqiang.cn

$s =~ s/old/new/g;
来源：http://cx.shxzskj.cn

[T49] Perl：函数
来源：http://ci.szsharing.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://op.newstarts.cn

[T50] Perl：逐行读文件
来源：http://fd.newstarts.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ui.hahajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://aa.huixinmuqiang.cn

[T51] Scala：Hello World
来源：http://bv.chemitech.net.cn

println("Hello")
来源：http://ef.shxzskj.cn

[T52] Scala：变量
来源：http://rc.lnxyls.cn

val a = 1;  var b = 2
来源：http://pb.gzmigu.cn

[T53] Scala：字符串插值
来源：http://lv.nszjky.cn

s"值: $b"
来源：http://aq.hahajie.cn

[T54] Scala：集合映射
来源：http://cr.huanxung.cn

List(1, 2, 3).map(_ * 2)
来源：http://yw.lnxyls.cn

[T55] Scala：集合过滤
来源：http://ew.jianghongdianzi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fq.shtwfgs.cn

[T56] Scala：样例类
来源：http://qd.shxzukj.cn

case class User(name: String, age: Int)
来源：http://ls.jianghongdianzi.cn

[T57] Scala：模式匹配
来源：http://ix.lnxyls.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://va.lnxyls.cn

[T58] Scala：函数定义
来源：http://cg.521024.cn

def add(a: Int, b: Int): Int = a + b
来源：http://tc.colortex.cn

[T59] Scala：循环
来源：http://hj.huixiangedu.cn

for (i <- 1 to 10) println(i)
来源：http://zc.huanxung.cn

[T60] Scala：折叠
来源：http://ed.nszjky.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://df.nicolike.cn

================================================================================
来源：http://gn.lnxyls.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hx.szsharing.cn

================================================================================
来源：http://ty.asd995.cn

[U01] Py：创建虚拟环境
来源：http://zb.huixinmuqiang.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bq.newstarts.cn

[U02] Py：导出 / 安装依赖
来源：http://dz.jianghongdianzi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lj.hnjuh.cn

[U03] Py：加载 .env 配置
来源：http://wv.shxzskj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://cf.panjiajie.cn

[U04] Py：变量调试打印
来源：http://xz.haigaiapp.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vf.jctech888.com.cn

[U05] Py：列表去重且保序
来源：http://ty.shtwfgs.cn

list(dict.fromkeys(arr))
来源：http://jt.shxzskj.cn

[U06] Py：合并两个字典
来源：http://wp.gzmigu.cn

{**a, **b}
来源：http://cw.nicolike.cn

[U07] Py：反转字典键值
来源：http://rr.huanxung.cn

{v: k for k, v in d.items()}
来源：http://ju.yuntaijiaju.cn

[U08] Py：展平二维列表
来源：http://jo.huanxung.cn

[y for x in nested for y in x]
来源：http://lk.szsharing.cn

[U09] Py：字典取最大值的键
来源：http://sf.hnjuh.cn

max(d, key=d.get)
来源：http://os.yuntaijiaju.cn

[U10] Py：按值排序字典
来源：http://mm.panjiajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zc.hnjuh.cn

[U11] Py：生成器表达式
来源：http://vf.asd995.cn

(x * 2 for x in arr)
来源：http://zp.chemitech.net.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rj.huixinmuqiang.cn

Counter(arr).most_common(3)
来源：http://db.jianghongdianzi.cn

[U13] Py：固定长度队列
来源：http://ut.lnxyls.cn

deque(maxlen=10)
来源：http://fi.bookmarksfly.cn

[U14] Py：分组收集到列表
来源：http://vm.shtwfgs.cn

defaultdict(list)
来源：http://fp.szxytkj.cn

[U15] Py：高精度计时
来源：http://ke.shxzskj.cn

t = time.perf_counter()
来源：http://mx.nicolike.cn

[U16] Py：命令行参数解析
来源：http://mk.bjjhwx.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zf.panjiajie.cn

[U17] Py：初始化日志
来源：http://xd.521024.cn

logging.basicConfig(level=logging.INFO)
来源：http://ye.huanxung.cn

[U18] Py：预编译正则
来源：http://ny.hnjuh.cn

pat = re.compile(r"\d+")
来源：http://aj.jctech888.com.cn

[U19] Py：正则替换带回调
来源：http://wm.gzmigu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wb.yuexingan06.cn

[U20] Py：缓存函数结果
来源：http://bk.521024.cn

@functools.lru_cache(maxsize=None)
来源：http://gm.asd995.cn

[U21] Py：自定义上下文管理器
来源：http://fm.asd995.cn

@contextlib.contextmanager
来源：http://au.szxytkj.cn

[U22] Py：矩阵转置
来源：http://hf.yuexingan06.cn

list(zip(*m))
来源：http://rp.asd995.cn

[U23] Py：分块读取大文件
来源：http://eo.nszjky.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://db.hnjuh.cn

[U24] Py：路径操作
来源：http://hs.nszjky.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ci.hahajie.cn

[U25] Py：CSV 按字典读
来源：http://ih.gzmigu.cn

csv.DictReader(f)
来源：http://tj.chemitech.net.cn

[U26] Py：并发下载
来源：http://wi.huanxung.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ha.colortex.cn

[U27] Py：异步 HTTP
来源：http://cs.hnjuh.cn

aiohttp.ClientSession() 配合 async with
来源：http://hv.newstarts.cn

[U28] Py：类型别名
来源：http://uh.hahajie.cn

UserId = int
来源：http://cj.jianghongdianzi.cn

[U29] Py：属性校验
来源：http://tk.muxihuayi.cn

@property 与 @x.setter 配合
来源：http://sm.wgjwhj.cn

[U30] Py：数据类
来源：http://vv.yuexingan06.cn

@dataclass(slots=True)
来源：http://cy.shxzukj.cn

[U31] Py：单测
来源：http://bp.shxzukj.cn

python -m pytest -q
来源：http://lt.huanxung.cn

[U32] Py：代码格式化
来源：http://iu.9csxet.cn

ruff format . && ruff check --fix .
来源：http://ho.panjiajie.cn

[U33] Py：打包发布
来源：http://wr.lnxyls.cn

python -m build  （依赖 pyproject.toml）
来源：http://jj.muxihuayi.cn

[U34] Py：判断编码
来源：http://kv.521024.cn

chardet.detect(raw)
来源：http://qu.9csxet.cn

[U35] Py：发送邮件
来源：http://ln.gzmigu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dt.bjjhwx.cn

[U36] Py：定时任务
来源：http://it.9csxet.cn

schedule.every(10).minutes.do(job)
来源：http://sz.jctech888.com.cn

[U37] Py：读写 Excel
来源：http://ly.muxihuayi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://lr.haigaiapp.cn

[U38] Py：获取脚本所在目录
来源：http://uk.muxihuayi.cn

Path(__file__).resolve().parent
来源：http://yg.shxzskj.cn

[U39] Py：判断是否在交互环境
来源：http://qu.chemitech.net.cn

sys.stdout.isatty()
来源：http://hr.haigaiapp.cn

[U40] Py：打印到标准错误
来源：http://hh.nicolike.cn

print("err", file=sys.stderr)
来源：http://tm.hnjuh.cn

[U41] PHP：初始化 Composer 项目
来源：http://et.shtwfgs.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://cf.shxzskj.cn

[U42] PHP：PSR-4 自动加载
来源：http://wq.nicolike.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sb.szxytkj.cn

[U43] PHP：声明命名空间
来源：http://gy.asd995.cn

namespace App\Http;
来源：http://sw.lnxyls.cn

[U44] PHP：开启严格类型
来源：http://jc.jctech888.com.cn

declare(strict_types=1);
来源：http://qs.bjjhwx.cn

[U45] PHP：类型声明与返回类型
来源：http://gz.gzmigu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://np.panjiajie.cn

[U46] PHP：可空类型
来源：http://vm.hnjuh.cn

?string $name = null
来源：http://db.lnxyls.cn

[U47] PHP：联合类型
来源：http://tl.wgjwhj.cn

int|string $id
来源：http://lw.colortex.cn

[U48] PHP：纯枚举
来源：http://ai.huanxung.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://oo.bjjhwx.cn

[U49] PHP：只读属性
来源：http://fr.shtwfgs.cn

public readonly string $name
来源：http://xy.shxzskj.cn

[U50] PHP：构造器属性提升
来源：http://tp.muxihuayi.cn

public function __construct(private int $id) {}
来源：http://en.huixinmuqiang.cn

[U51] PHP：数组解构
来源：http://xl.huixinmuqiang.cn

[$a, $b] = $arr;
来源：http://gt.szsharing.cn

[U52] PHP：箭头函数
来源：http://ap.nszjky.cn

$double = fn($x) => $x * 2;
来源：http://to.huanxung.cn

[U53] PHP：空合并运算符
来源：http://cq.shxzskj.cn

$v = $a ?? $b ?? "default";
来源：http://wt.bjjhwx.cn

[U54] PHP：空安全调用
来源：http://dk.huanxung.cn

$obj?->method()
来源：http://nf.muxihuayi.cn

[U55] PHP：match 表达式
来源：http://su.wgjwhj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wp.colortex.cn

[U56] PHP：命名参数
来源：http://en.muxihuayi.cn

f(a: 1, b: 2)
来源：http://xc.lnxyls.cn

[U57] PHP：字符串插值
来源：http://gm.shxzskj.cn

"值: {$a}"
来源：http://gf.yuexingan06.cn

[U58] PHP：数组三件套
来源：http://xu.huixiangedu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fz.521024.cn

[U59] PHP：自定义排序
来源：http://qh.9csxet.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://en.wgjwhj.cn

[U60] PHP：JSON 编解码
来源：http://fh.jianghongdianzi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zb.bookmarksfly.cn

[U61] PHP：正则
来源：http://qc.521024.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://an.521024.cn

[U62] PHP：日期对象
来源：http://dh.chemitech.net.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://op.lnxyls.cn

[U63] PHP：文件读写
来源：http://zw.huixiangedu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zx.nszjky.cn

[U64] PHP：目录遍历
来源：http://gx.panjiajie.cn

glob("dir/*.php");  scandir("dir");
来源：http://wz.newstarts.cn

[U65] PHP：会话
来源：http://yw.panjiajie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kj.lnxyls.cn

[U66] PHP：设置 Cookie
来源：http://aa.chemitech.net.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mb.huixiangedu.cn

[U67] PHP：处理文件上传
来源：http://hz.yuntaijiaju.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dn.bjjhwx.cn

[U68] PHP：PDO 连接
来源：http://ha.colortex.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tt.wgjwhj.cn

[U69] PHP：PDO 预处理
来源：http://zz.jctech888.com.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hv.hnjuh.cn

[U70] PHP：PDO 事务
来源：http://zx.bookmarksfly.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cx.hnjuh.cn

[U71] PHP：抛出异常
来源：http://ad.asd995.cn

throw new RuntimeException("失败", 500);
来源：http://un.yuntaijiaju.cn

[U72] PHP：写错误日志
来源：http://wl.jctech888.com.cn

error_log("失败: " . $e->getMessage());
来源：http://mt.szxytkj.cn

[U73] PHP：读取 ini 配置
来源：http://xh.szsharing.cn

parse_ini_file("config.ini", true)
来源：http://bv.yuntaijiaju.cn

[U74] PHP：读取环境变量
来源：http://ea.chemitech.net.cn

getenv("APP_ENV") ?: "production"
来源：http://pn.huixiangedu.cn

[U75] PHP：依赖注入
来源：http://xn.gzmigu.cn

composer require psr/container
来源：http://hq.haigaiapp.cn

[U76] PHP：简单路由
来源：http://wr.yuntaijiaju.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lx.hnjuh.cn

[U77] PHP：模板渲染
来源：http://qh.521024.cn

composer require twig/twig
来源：http://fk.huixiangedu.cn

[U78] PHP：单元测试
来源：http://lw.nicolike.cn

composer require --dev phpunit/phpunit
来源：http://au.szxytkj.cn

[U79] PHP：静态分析
来源：http://jl.shxzukj.cn

composer require --dev phpstan/phpstan
来源：http://jr.huixiangedu.cn

[U80] PHP：代码规范修复
来源：http://wz.newstarts.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://si.shxzskj.cn

[U81] JS：初始化项目
来源：http://qg.newstarts.cn

npm init -y;  npm i express
来源：http://mp.bookmarksfly.cn

[U82] JS：package.json 脚本
来源：http://kv.lnxyls.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hv.hahajie.cn

[U83] JS：ES Module 导入导出
来源：http://qq.wgjwhj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://uy.szsharing.cn

[U84] JS：CommonJS 写法
来源：http://sa.gzmigu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://pa.yuntaijiaju.cn

[U85] JS：可选链
来源：http://db.nszjky.cn

a?.b?.c
来源：http://th.newstarts.cn

[U86] JS：空值合并
来源：http://ru.newstarts.cn

a ?? b
来源：http://gl.lnxyls.cn

[U87] JS：解构默认值
来源：http://nh.bookmarksfly.cn

const { a = 1, b = 2 } = obj;
来源：http://ra.huixiangedu.cn

[U88] JS：对象展开合并
来源：http://rs.wgjwhj.cn

{ ...a, ...b }
来源：http://uw.huixinmuqiang.cn

[U89] JS：数组去重
来源：http://oy.521024.cn

[...new Set(arr)]
来源：http://oh.521024.cn

[U90] JS：数字数组排序
来源：http://bh.szsharing.cn

[...arr].sort((a, b) => a - b)
来源：http://hi.bjjhwx.cn

[U91] JS：对象键值遍历
来源：http://xu.panjiajie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ak.huanxung.cn

[U92] JS：深拷贝
来源：http://xk.huixinmuqiang.cn

structuredClone(obj)
来源：http://sk.szxytkj.cn

[U93] JS：模板字符串
来源：http://fn.panjiajie.cn

`共 ${n} 条`
来源：http://yd.muxihuayi.cn

[U94] JS：箭头函数
来源：http://kp.shtwfgs.cn

const double = x => x * 2;
来源：http://dq.nszjky.cn

[U95] JS：Promise 包装
来源：http://ww.haigaiapp.cn

new Promise((resolve, reject) => {})
来源：http://kp.asd995.cn

[U96] JS：async/await 与异常
来源：http://tk.9csxet.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fu.nszjky.cn

[U97] JS：并发请求
来源：http://zi.szxytkj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://id.hnjuh.cn

[U98] JS：fetch 带 JSON
来源：http://xg.gzmigu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jl.muxihuayi.cn

[U99] JS：事件监听
来源：http://vq.chemitech.net.cn

el.addEventListener("click", e => {})
来源：http://hg.szxytkj.cn

[U100] JS：DOM 查询
来源：http://lw.yuntaijiaju.cn

document.querySelector(".item")
来源：http://ps.bjjhwx.cn

[U101] JS：classList 操作
来源：http://oa.bookmarksfly.cn

el.classList.toggle("active")
来源：http://xj.huanxung.cn

[U102] JS：本地存储
来源：http://lu.huanxung.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://td.wgjwhj.cn

[U103] JS：定时器
来源：http://nk.muxihuayi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uy.bookmarksfly.cn

[U104] JS：防抖
来源：http://cv.lnxyls.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uy.szsharing.cn

[U105] JS：节流
来源：http://vt.yuexingan06.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ey.haigaiapp.cn

[U106] JS：日期格式化
来源：http://ix.colortex.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cc.huixinmuqiang.cn

[U107] JS：数字千分位
来源：http://nr.huixinmuqiang.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cy.bookmarksfly.cn

[U108] JS：随机整数
来源：http://mr.nszjky.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wu.huixinmuqiang.cn

[U109] JS：数组分组
来源：http://km.szxytkj.cn

Object.groupBy(arr, x => x.type)
来源：http://ab.yuexingan06.cn

[U110] JS：数组分块
来源：http://sf.9csxet.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ip.9csxet.cn

[U111] JS：对象转 Map
来源：http://nl.yuexingan06.cn

new Map(Object.entries(obj))
来源：http://eo.bjjhwx.cn

[U112] JS：字符串补位
来源：http://wv.yuexingan06.cn

"7".padStart(3, "0")
来源：http://rz.shxzskj.cn


<!-- 参考信息 -->