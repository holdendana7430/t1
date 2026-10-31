代发 wailian999

[T25] Swift：结构体
来源：http://ld.haigaiapp.cn

struct P { var x: Int }
来源：http://yq.newstarts.cn

[T26] Swift：类与重写
来源：http://pp.nicolike.cn

class A: Base { override func f() {} }
来源：http://lk.hahajie.cn

[T27] Swift：错误处理
来源：http://uh.yuntaijiaju.cn

do { try f() } catch { print(error) }
来源：http://id.shxzukj.cn

[T28] Swift：枚举
来源：http://rv.colortex.cn

enum Color { case red, green }
来源：http://rt.nicolike.cn

[T29] Swift：guard 提前返回
来源：http://kd.bookmarksfly.cn

guard let x = opt else { return }
来源：http://xo.gzmigu.cn

[T30] Swift：协议
来源：http://zt.shtwfgs.cn

protocol Shape { func area() -> Double }
来源：http://qu.bjjhwx.cn

[T31] Lua：Hello World
来源：http://jh.jianghongdianzi.cn

print("Hello")
来源：http://zx.colortex.cn

[T32] Lua：局部变量
来源：http://ti.wgjwhj.cn

local a = 1
来源：http://vh.jianghongdianzi.cn

[T33] Lua：表（数组）
来源：http://ao.szxytkj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://bv.9csxet.cn

[T34] Lua：遍历表
来源：http://hg.colortex.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://op.newstarts.cn

[T35] Lua：字典表
来源：http://xp.haigaiapp.cn

local d = { a = 1 };  d.b = 2
来源：http://ib.chemitech.net.cn

[T36] Lua：函数
来源：http://ws.hahajie.cn

function add(a, b) return a + b end
来源：http://ep.nicolike.cn

[T37] Lua：字符串拼接
来源：http://qz.gzmigu.cn

"a" .. "b"
来源：http://jp.wgjwhj.cn

[T38] Lua：条件
来源：http://fe.yuntaijiaju.cn

if x > 0 then print("正") end
来源：http://sh.muxihuayi.cn

[T39] Lua：模式匹配
来源：http://of.szsharing.cn

string.find(s, "%d+")
来源：http://ju.asd995.cn

[T40] Lua：元表
来源：http://jq.jctech888.com.cn

setmetatable({}, { __index = base })
来源：http://jf.panjiajie.cn

[T41] Perl：Hello World
来源：http://wr.yuexingan06.cn

print "Hello\n";
来源：http://wx.lnxyls.cn

[T42] Perl：变量类型
来源：http://en.bjjhwx.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xr.bookmarksfly.cn

[T43] Perl：字符串插值
来源：http://uc.nszjky.cn

"值: $a"
来源：http://jl.haigaiapp.cn

[T44] Perl：条件
来源：http://lb.newstarts.cn

if ($a > 0) { print "正"; }
来源：http://wb.szxytkj.cn

[T45] Perl：数组遍历
来源：http://lw.shxzskj.cn

for my $x (@arr) { print $x; }
来源：http://yx.huixinmuqiang.cn

[T46] Perl：哈希操作
来源：http://ox.lnxyls.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jb.colortex.cn

[T47] Perl：正则捕获
来源：http://rs.jianghongdianzi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://cp.shxzukj.cn

[T48] Perl：正则替换
来源：http://yk.521024.cn

$s =~ s/old/new/g;
来源：http://ej.asd995.cn

[T49] Perl：函数
来源：http://dt.gzmigu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tr.hahajie.cn

[T50] Perl：逐行读文件
来源：http://vo.haigaiapp.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rn.nicolike.cn

while (my $line = <$fh>) { print $line; }
来源：http://fh.bjjhwx.cn

[T51] Scala：Hello World
来源：http://hb.521024.cn

println("Hello")
来源：http://zc.hahajie.cn

[T52] Scala：变量
来源：http://bi.521024.cn

val a = 1;  var b = 2
来源：http://zh.muxihuayi.cn

[T53] Scala：字符串插值
来源：http://tj.muxihuayi.cn

s"值: $b"
来源：http://mw.9csxet.cn

[T54] Scala：集合映射
来源：http://ny.wgjwhj.cn

List(1, 2, 3).map(_ * 2)
来源：http://uc.shtwfgs.cn

[T55] Scala：集合过滤
来源：http://qu.jianghongdianzi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://km.huixiangedu.cn

[T56] Scala：样例类
来源：http://is.jianghongdianzi.cn

case class User(name: String, age: Int)
来源：http://hb.chemitech.net.cn

[T57] Scala：模式匹配
来源：http://ut.bjjhwx.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://qq.bjjhwx.cn

[T58] Scala：函数定义
来源：http://lh.wgjwhj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fm.9csxet.cn

[T59] Scala：循环
来源：http://ns.chemitech.net.cn

for (i <- 1 to 10) println(i)
来源：http://pl.nszjky.cn

[T60] Scala：折叠
来源：http://eh.bjjhwx.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kx.huixinmuqiang.cn

================================================================================
来源：http://kl.9csxet.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sy.yuntaijiaju.cn

================================================================================
来源：http://wr.521024.cn

[U01] Py：创建虚拟环境
来源：http://iv.shxzukj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bh.huixinmuqiang.cn

[U02] Py：导出 / 安装依赖
来源：http://zj.muxihuayi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://an.bjjhwx.cn

[U03] Py：加载 .env 配置
来源：http://mq.9csxet.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://tj.muxihuayi.cn

[U04] Py：变量调试打印
来源：http://vc.gzmigu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://va.hahajie.cn

[U05] Py：列表去重且保序
来源：http://zh.bookmarksfly.cn

list(dict.fromkeys(arr))
来源：http://an.chemitech.net.cn

[U06] Py：合并两个字典
来源：http://jb.yuexingan06.cn

{**a, **b}
来源：http://kw.huixinmuqiang.cn

[U07] Py：反转字典键值
来源：http://yv.haigaiapp.cn

{v: k for k, v in d.items()}
来源：http://ce.chemitech.net.cn

[U08] Py：展平二维列表
来源：http://kl.huixinmuqiang.cn

[y for x in nested for y in x]
来源：http://rt.huixinmuqiang.cn

[U09] Py：字典取最大值的键
来源：http://lj.muxihuayi.cn

max(d, key=d.get)
来源：http://ei.lnxyls.cn

[U10] Py：按值排序字典
来源：http://pk.yuntaijiaju.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mu.muxihuayi.cn

[U11] Py：生成器表达式
来源：http://ya.szxytkj.cn

(x * 2 for x in arr)
来源：http://za.asd995.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ml.jctech888.com.cn

Counter(arr).most_common(3)
来源：http://rf.haigaiapp.cn

[U13] Py：固定长度队列
来源：http://xc.huixinmuqiang.cn

deque(maxlen=10)
来源：http://ag.nicolike.cn

[U14] Py：分组收集到列表
来源：http://ff.muxihuayi.cn

defaultdict(list)
来源：http://nd.huixiangedu.cn

[U15] Py：高精度计时
来源：http://wi.asd995.cn

t = time.perf_counter()
来源：http://fe.bjjhwx.cn

[U16] Py：命令行参数解析
来源：http://tg.panjiajie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xd.bookmarksfly.cn

[U17] Py：初始化日志
来源：http://rz.newstarts.cn

logging.basicConfig(level=logging.INFO)
来源：http://dm.szxytkj.cn

[U18] Py：预编译正则
来源：http://al.haigaiapp.cn

pat = re.compile(r"\d+")
来源：http://eu.gzmigu.cn

[U19] Py：正则替换带回调
来源：http://jf.shtwfgs.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ci.szxytkj.cn

[U20] Py：缓存函数结果
来源：http://ko.muxihuayi.cn

@functools.lru_cache(maxsize=None)
来源：http://jb.bookmarksfly.cn

[U21] Py：自定义上下文管理器
来源：http://ie.shtwfgs.cn

@contextlib.contextmanager
来源：http://iz.lnxyls.cn

[U22] Py：矩阵转置
来源：http://nw.szxytkj.cn

list(zip(*m))
来源：http://vu.muxihuayi.cn

[U23] Py：分块读取大文件
来源：http://ey.yuexingan06.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mg.nszjky.cn

[U24] Py：路径操作
来源：http://up.newstarts.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ki.muxihuayi.cn

[U25] Py：CSV 按字典读
来源：http://jo.muxihuayi.cn

csv.DictReader(f)
来源：http://pe.bjjhwx.cn

[U26] Py：并发下载
来源：http://kj.shxzukj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yy.chemitech.net.cn

[U27] Py：异步 HTTP
来源：http://fw.521024.cn

aiohttp.ClientSession() 配合 async with
来源：http://je.hnjuh.cn

[U28] Py：类型别名
来源：http://ys.nszjky.cn

UserId = int
来源：http://ty.hnjuh.cn

[U29] Py：属性校验
来源：http://mp.shtwfgs.cn

@property 与 @x.setter 配合
来源：http://jb.gzmigu.cn

[U30] Py：数据类
来源：http://ig.hahajie.cn

@dataclass(slots=True)
来源：http://qc.yuntaijiaju.cn

[U31] Py：单测
来源：http://pe.9csxet.cn

python -m pytest -q
来源：http://xn.521024.cn

[U32] Py：代码格式化
来源：http://no.jctech888.com.cn

ruff format . && ruff check --fix .
来源：http://an.nszjky.cn

[U33] Py：打包发布
来源：http://iz.jianghongdianzi.cn

python -m build  （依赖 pyproject.toml）
来源：http://qm.521024.cn

[U34] Py：判断编码
来源：http://qp.yuntaijiaju.cn

chardet.detect(raw)
来源：http://mb.jctech888.com.cn

[U35] Py：发送邮件
来源：http://if.haigaiapp.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zf.gzmigu.cn

[U36] Py：定时任务
来源：http://ht.huixinmuqiang.cn

schedule.every(10).minutes.do(job)
来源：http://ds.lnxyls.cn

[U37] Py：读写 Excel
来源：http://ws.yuexingan06.cn

pandas.read_excel / DataFrame.to_excel
来源：http://en.szsharing.cn

[U38] Py：获取脚本所在目录
来源：http://kw.bjjhwx.cn

Path(__file__).resolve().parent
来源：http://ic.newstarts.cn

[U39] Py：判断是否在交互环境
来源：http://if.521024.cn

sys.stdout.isatty()
来源：http://nx.bjjhwx.cn

[U40] Py：打印到标准错误
来源：http://id.bookmarksfly.cn

print("err", file=sys.stderr)
来源：http://fy.huixinmuqiang.cn

[U41] PHP：初始化 Composer 项目
来源：http://ci.lnxyls.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://il.szsharing.cn

[U42] PHP：PSR-4 自动加载
来源：http://bp.jianghongdianzi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sz.huixiangedu.cn

[U43] PHP：声明命名空间
来源：http://ok.hnjuh.cn

namespace App\Http;
来源：http://ac.shtwfgs.cn

[U44] PHP：开启严格类型
来源：http://bh.jctech888.com.cn

declare(strict_types=1);
来源：http://jq.hnjuh.cn

[U45] PHP：类型声明与返回类型
来源：http://gq.lnxyls.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bo.panjiajie.cn

[U46] PHP：可空类型
来源：http://mp.szxytkj.cn

?string $name = null
来源：http://bi.shtwfgs.cn

[U47] PHP：联合类型
来源：http://gd.huixinmuqiang.cn

int|string $id
来源：http://xu.yuntaijiaju.cn

[U48] PHP：纯枚举
来源：http://we.shxzukj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hp.muxihuayi.cn

[U49] PHP：只读属性
来源：http://vi.wgjwhj.cn

public readonly string $name
来源：http://us.jianghongdianzi.cn

[U50] PHP：构造器属性提升
来源：http://lr.jctech888.com.cn

public function __construct(private int $id) {}
来源：http://pn.yuntaijiaju.cn

[U51] PHP：数组解构
来源：http://ah.newstarts.cn

[$a, $b] = $arr;
来源：http://sa.lnxyls.cn

[U52] PHP：箭头函数
来源：http://dx.521024.cn

$double = fn($x) => $x * 2;
来源：http://tq.szxytkj.cn

[U53] PHP：空合并运算符
来源：http://ou.lnxyls.cn

$v = $a ?? $b ?? "default";
来源：http://wm.nicolike.cn

[U54] PHP：空安全调用
来源：http://vr.bookmarksfly.cn

$obj?->method()
来源：http://pu.hnjuh.cn

[U55] PHP：match 表达式
来源：http://fl.shxzukj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dc.9csxet.cn

[U56] PHP：命名参数
来源：http://jj.gzmigu.cn

f(a: 1, b: 2)
来源：http://pg.hnjuh.cn

[U57] PHP：字符串插值
来源：http://mx.szxytkj.cn

"值: {$a}"
来源：http://le.lnxyls.cn

[U58] PHP：数组三件套
来源：http://sx.huixiangedu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://au.shxzukj.cn

[U59] PHP：自定义排序
来源：http://cg.huixinmuqiang.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mv.hnjuh.cn

[U60] PHP：JSON 编解码
来源：http://ja.lnxyls.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rj.bjjhwx.cn

[U61] PHP：正则
来源：http://so.colortex.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ar.szsharing.cn

[U62] PHP：日期对象
来源：http://no.hahajie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://an.jctech888.com.cn

[U63] PHP：文件读写
来源：http://kb.huanxung.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ye.jctech888.com.cn

[U64] PHP：目录遍历
来源：http://uu.jctech888.com.cn

glob("dir/*.php");  scandir("dir");
来源：http://st.wgjwhj.cn

[U65] PHP：会话
来源：http://ws.9csxet.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kj.colortex.cn

[U66] PHP：设置 Cookie
来源：http://gc.chemitech.net.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://iv.bookmarksfly.cn

[U67] PHP：处理文件上传
来源：http://sb.huixiangedu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vk.chemitech.net.cn

[U68] PHP：PDO 连接
来源：http://vf.521024.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://io.jctech888.com.cn

[U69] PHP：PDO 预处理
来源：http://co.wgjwhj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://si.lnxyls.cn

[U70] PHP：PDO 事务
来源：http://mx.bjjhwx.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ze.hnjuh.cn

[U71] PHP：抛出异常
来源：http://cy.nszjky.cn

throw new RuntimeException("失败", 500);
来源：http://tu.colortex.cn

[U72] PHP：写错误日志
来源：http://ph.szxytkj.cn

error_log("失败: " . $e->getMessage());
来源：http://wq.521024.cn

[U73] PHP：读取 ini 配置
来源：http://kf.nszjky.cn

parse_ini_file("config.ini", true)
来源：http://ni.521024.cn

[U74] PHP：读取环境变量
来源：http://dx.asd995.cn

getenv("APP_ENV") ?: "production"
来源：http://yz.panjiajie.cn

[U75] PHP：依赖注入
来源：http://sa.521024.cn

composer require psr/container
来源：http://mi.szxytkj.cn

[U76] PHP：简单路由
来源：http://ip.huixiangedu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dp.lnxyls.cn

[U77] PHP：模板渲染
来源：http://pk.jianghongdianzi.cn

composer require twig/twig
来源：http://bp.newstarts.cn

[U78] PHP：单元测试
来源：http://cl.lnxyls.cn

composer require --dev phpunit/phpunit
来源：http://lu.jctech888.com.cn

[U79] PHP：静态分析
来源：http://ko.szsharing.cn

composer require --dev phpstan/phpstan
来源：http://ke.colortex.cn

[U80] PHP：代码规范修复
来源：http://ji.nicolike.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ef.huixiangedu.cn

[U81] JS：初始化项目
来源：http://jw.yuntaijiaju.cn

npm init -y;  npm i express
来源：http://pf.colortex.cn

[U82] JS：package.json 脚本
来源：http://zc.hnjuh.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hu.lnxyls.cn

[U83] JS：ES Module 导入导出
来源：http://ur.shtwfgs.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xv.bjjhwx.cn

[U84] JS：CommonJS 写法
来源：http://ln.yuntaijiaju.cn

module.exports = { a };  const { a } = require("./m");
来源：http://os.haigaiapp.cn

[U85] JS：可选链
来源：http://mu.wgjwhj.cn

a?.b?.c
来源：http://ku.asd995.cn

[U86] JS：空值合并
来源：http://yf.asd995.cn

a ?? b
来源：http://cy.chemitech.net.cn

[U87] JS：解构默认值
来源：http://se.521024.cn

const { a = 1, b = 2 } = obj;
来源：http://oa.newstarts.cn

[U88] JS：对象展开合并
来源：http://dn.asd995.cn

{ ...a, ...b }
来源：http://lf.yuexingan06.cn

[U89] JS：数组去重
来源：http://ze.muxihuayi.cn

[...new Set(arr)]
来源：http://so.huixiangedu.cn

[U90] JS：数字数组排序
来源：http://pm.9csxet.cn

[...arr].sort((a, b) => a - b)
来源：http://wv.szxytkj.cn

[U91] JS：对象键值遍历
来源：http://ib.yuntaijiaju.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ox.newstarts.cn

[U92] JS：深拷贝
来源：http://tz.yuntaijiaju.cn

structuredClone(obj)
来源：http://op.nicolike.cn

[U93] JS：模板字符串
来源：http://hk.asd995.cn

`共 ${n} 条`
来源：http://zt.lnxyls.cn

[U94] JS：箭头函数
来源：http://al.bjjhwx.cn

const double = x => x * 2;
来源：http://kj.bjjhwx.cn

[U95] JS：Promise 包装
来源：http://th.szxytkj.cn

new Promise((resolve, reject) => {})
来源：http://wd.shxzukj.cn

[U96] JS：async/await 与异常
来源：http://sf.shxzskj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dj.hahajie.cn

[U97] JS：并发请求
来源：http://fh.521024.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qy.muxihuayi.cn

[U98] JS：fetch 带 JSON
来源：http://up.szxytkj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fc.huixinmuqiang.cn

[U99] JS：事件监听
来源：http://gz.colortex.cn

el.addEventListener("click", e => {})
来源：http://km.nszjky.cn

[U100] JS：DOM 查询
来源：http://mh.huixinmuqiang.cn

document.querySelector(".item")
来源：http://kw.jianghongdianzi.cn

[U101] JS：classList 操作
来源：http://ne.yuntaijiaju.cn

el.classList.toggle("active")
来源：http://nc.chemitech.net.cn

[U102] JS：本地存储
来源：http://ta.hnjuh.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://dq.hnjuh.cn

[U103] JS：定时器
来源：http://qy.wgjwhj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://sf.newstarts.cn

[U104] JS：防抖
来源：http://kg.bjjhwx.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xb.huixinmuqiang.cn

[U105] JS：节流
来源：http://vo.wgjwhj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ax.jctech888.com.cn

[U106] JS：日期格式化
来源：http://ap.jianghongdianzi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hq.jianghongdianzi.cn

[U107] JS：数字千分位
来源：http://mq.bookmarksfly.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cp.chemitech.net.cn

[U108] JS：随机整数
来源：http://uo.szxytkj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qe.jianghongdianzi.cn

[U109] JS：数组分组
来源：http://pu.nszjky.cn

Object.groupBy(arr, x => x.type)
来源：http://ph.jctech888.com.cn

[U110] JS：数组分块
来源：http://xe.shtwfgs.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ir.wgjwhj.cn

[U111] JS：对象转 Map
来源：http://kb.shxzukj.cn

new Map(Object.entries(obj))
来源：http://xn.521024.cn

[U112] JS：字符串补位
来源：http://nm.lnxyls.cn

"7".padStart(3, "0")
来源：http://oy.huixiangedu.cn


<!-- 参考信息 -->