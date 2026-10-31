代发 wailian999

[T25] Swift：结构体
来源：http://bx.newstarts.cn

struct P { var x: Int }
来源：http://ux.jctech888.com.cn

[T26] Swift：类与重写
来源：http://oz.huanxung.cn

class A: Base { override func f() {} }
来源：http://cf.panjiajie.cn

[T27] Swift：错误处理
来源：http://hm.gzmigu.cn

do { try f() } catch { print(error) }
来源：http://da.9csxet.cn

[T28] Swift：枚举
来源：http://nq.huixiangedu.cn

enum Color { case red, green }
来源：http://sh.9csxet.cn

[T29] Swift：guard 提前返回
来源：http://we.521024.cn

guard let x = opt else { return }
来源：http://iy.newstarts.cn

[T30] Swift：协议
来源：http://mw.panjiajie.cn

protocol Shape { func area() -> Double }
来源：http://oc.muxihuayi.cn

[T31] Lua：Hello World
来源：http://ew.newstarts.cn

print("Hello")
来源：http://az.panjiajie.cn

[T32] Lua：局部变量
来源：http://io.chemitech.net.cn

local a = 1
来源：http://zo.shtwfgs.cn

[T33] Lua：表（数组）
来源：http://tt.jianghongdianzi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ox.shtwfgs.cn

[T34] Lua：遍历表
来源：http://dl.gzmigu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ti.wgjwhj.cn

[T35] Lua：字典表
来源：http://kp.asd995.cn

local d = { a = 1 };  d.b = 2
来源：http://ju.haigaiapp.cn

[T36] Lua：函数
来源：http://ku.bookmarksfly.cn

function add(a, b) return a + b end
来源：http://en.hnjuh.cn

[T37] Lua：字符串拼接
来源：http://ut.huixiangedu.cn

"a" .. "b"
来源：http://cr.jctech888.com.cn

[T38] Lua：条件
来源：http://by.lnxyls.cn

if x > 0 then print("正") end
来源：http://nm.chemitech.net.cn

[T39] Lua：模式匹配
来源：http://bo.gzmigu.cn

string.find(s, "%d+")
来源：http://qn.nicolike.cn

[T40] Lua：元表
来源：http://jj.shxzskj.cn

setmetatable({}, { __index = base })
来源：http://sx.yuntaijiaju.cn

[T41] Perl：Hello World
来源：http://bv.huanxung.cn

print "Hello\n";
来源：http://cy.hnjuh.cn

[T42] Perl：变量类型
来源：http://rg.yuntaijiaju.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cn.shxzukj.cn

[T43] Perl：字符串插值
来源：http://gm.asd995.cn

"值: $a"
来源：http://yu.gzmigu.cn

[T44] Perl：条件
来源：http://jr.asd995.cn

if ($a > 0) { print "正"; }
来源：http://xp.jianghongdianzi.cn

[T45] Perl：数组遍历
来源：http://ce.shxzskj.cn

for my $x (@arr) { print $x; }
来源：http://ot.gzmigu.cn

[T46] Perl：哈希操作
来源：http://bn.shtwfgs.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uf.bjjhwx.cn

[T47] Perl：正则捕获
来源：http://rq.lnxyls.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pb.asd995.cn

[T48] Perl：正则替换
来源：http://mx.9csxet.cn

$s =~ s/old/new/g;
来源：http://xu.hahajie.cn

[T49] Perl：函数
来源：http://di.hahajie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://oc.asd995.cn

[T50] Perl：逐行读文件
来源：http://vy.gzmigu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://du.lnxyls.cn

while (my $line = <$fh>) { print $line; }
来源：http://ce.bookmarksfly.cn

[T51] Scala：Hello World
来源：http://lv.szsharing.cn

println("Hello")
来源：http://jk.haigaiapp.cn

[T52] Scala：变量
来源：http://mt.nszjky.cn

val a = 1;  var b = 2
来源：http://oe.shxzukj.cn

[T53] Scala：字符串插值
来源：http://sy.chemitech.net.cn

s"值: $b"
来源：http://va.asd995.cn

[T54] Scala：集合映射
来源：http://kc.haigaiapp.cn

List(1, 2, 3).map(_ * 2)
来源：http://if.chemitech.net.cn

[T55] Scala：集合过滤
来源：http://gg.jianghongdianzi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fv.jctech888.com.cn

[T56] Scala：样例类
来源：http://gt.jctech888.com.cn

case class User(name: String, age: Int)
来源：http://xt.hnjuh.cn

[T57] Scala：模式匹配
来源：http://wy.newstarts.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tp.shtwfgs.cn

[T58] Scala：函数定义
来源：http://pw.bookmarksfly.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fd.chemitech.net.cn

[T59] Scala：循环
来源：http://lo.szxytkj.cn

for (i <- 1 to 10) println(i)
来源：http://tb.gzmigu.cn

[T60] Scala：折叠
来源：http://ev.szxytkj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nj.nicolike.cn

================================================================================
来源：http://ww.shxzskj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qn.colortex.cn

================================================================================
来源：http://mg.hnjuh.cn

[U01] Py：创建虚拟环境
来源：http://tp.colortex.cn

python -m venv .venv && source .venv/bin/activate
来源：http://dl.huixiangedu.cn

[U02] Py：导出 / 安装依赖
来源：http://ob.yuexingan06.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ge.nicolike.cn

[U03] Py：加载 .env 配置
来源：http://cd.newstarts.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://er.yuexingan06.cn

[U04] Py：变量调试打印
来源：http://vq.hnjuh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zt.bookmarksfly.cn

[U05] Py：列表去重且保序
来源：http://xe.huanxung.cn

list(dict.fromkeys(arr))
来源：http://av.gzmigu.cn

[U06] Py：合并两个字典
来源：http://ki.hahajie.cn

{**a, **b}
来源：http://te.jctech888.com.cn

[U07] Py：反转字典键值
来源：http://ut.gzmigu.cn

{v: k for k, v in d.items()}
来源：http://wt.szxytkj.cn

[U08] Py：展平二维列表
来源：http://zp.chemitech.net.cn

[y for x in nested for y in x]
来源：http://vj.panjiajie.cn

[U09] Py：字典取最大值的键
来源：http://fa.jctech888.com.cn

max(d, key=d.get)
来源：http://sl.shxzskj.cn

[U10] Py：按值排序字典
来源：http://eb.chemitech.net.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mb.shxzukj.cn

[U11] Py：生成器表达式
来源：http://tt.hahajie.cn

(x * 2 for x in arr)
来源：http://ku.shxzskj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://hy.huixiangedu.cn

Counter(arr).most_common(3)
来源：http://bp.lnxyls.cn

[U13] Py：固定长度队列
来源：http://gu.bookmarksfly.cn

deque(maxlen=10)
来源：http://iu.jianghongdianzi.cn

[U14] Py：分组收集到列表
来源：http://oa.shxzskj.cn

defaultdict(list)
来源：http://dd.colortex.cn

[U15] Py：高精度计时
来源：http://dp.shxzukj.cn

t = time.perf_counter()
来源：http://ea.nszjky.cn

[U16] Py：命令行参数解析
来源：http://cr.huixiangedu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nm.panjiajie.cn

[U17] Py：初始化日志
来源：http://ge.shtwfgs.cn

logging.basicConfig(level=logging.INFO)
来源：http://yf.colortex.cn

[U18] Py：预编译正则
来源：http://pz.bookmarksfly.cn

pat = re.compile(r"\d+")
来源：http://zo.huanxung.cn

[U19] Py：正则替换带回调
来源：http://yt.chemitech.net.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mh.muxihuayi.cn

[U20] Py：缓存函数结果
来源：http://za.lnxyls.cn

@functools.lru_cache(maxsize=None)
来源：http://vk.nszjky.cn

[U21] Py：自定义上下文管理器
来源：http://tg.shxzskj.cn

@contextlib.contextmanager
来源：http://gk.yuexingan06.cn

[U22] Py：矩阵转置
来源：http://cf.yuexingan06.cn

list(zip(*m))
来源：http://qj.hahajie.cn

[U23] Py：分块读取大文件
来源：http://qr.colortex.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xy.shtwfgs.cn

[U24] Py：路径操作
来源：http://dc.haigaiapp.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://sn.nszjky.cn

[U25] Py：CSV 按字典读
来源：http://xi.haigaiapp.cn

csv.DictReader(f)
来源：http://py.jianghongdianzi.cn

[U26] Py：并发下载
来源：http://js.yuntaijiaju.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bj.9csxet.cn

[U27] Py：异步 HTTP
来源：http://ea.panjiajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://qk.shtwfgs.cn

[U28] Py：类型别名
来源：http://fo.shtwfgs.cn

UserId = int
来源：http://qd.9csxet.cn

[U29] Py：属性校验
来源：http://mq.colortex.cn

@property 与 @x.setter 配合
来源：http://ra.gzmigu.cn

[U30] Py：数据类
来源：http://og.yuntaijiaju.cn

@dataclass(slots=True)
来源：http://el.huixiangedu.cn

[U31] Py：单测
来源：http://ax.hahajie.cn

python -m pytest -q
来源：http://le.hahajie.cn

[U32] Py：代码格式化
来源：http://ll.9csxet.cn

ruff format . && ruff check --fix .
来源：http://vm.jianghongdianzi.cn

[U33] Py：打包发布
来源：http://hr.yuexingan06.cn

python -m build  （依赖 pyproject.toml）
来源：http://uo.wgjwhj.cn

[U34] Py：判断编码
来源：http://lu.huixinmuqiang.cn

chardet.detect(raw)
来源：http://lq.newstarts.cn

[U35] Py：发送邮件
来源：http://pi.hahajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ng.newstarts.cn

[U36] Py：定时任务
来源：http://zj.jctech888.com.cn

schedule.every(10).minutes.do(job)
来源：http://xm.shxzukj.cn

[U37] Py：读写 Excel
来源：http://rv.lnxyls.cn

pandas.read_excel / DataFrame.to_excel
来源：http://cc.colortex.cn

[U38] Py：获取脚本所在目录
来源：http://cv.haigaiapp.cn

Path(__file__).resolve().parent
来源：http://oi.shtwfgs.cn

[U39] Py：判断是否在交互环境
来源：http://pn.shxzskj.cn

sys.stdout.isatty()
来源：http://bq.shtwfgs.cn

[U40] Py：打印到标准错误
来源：http://pw.nszjky.cn

print("err", file=sys.stderr)
来源：http://hn.yuexingan06.cn

[U41] PHP：初始化 Composer 项目
来源：http://kb.wgjwhj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://se.gzmigu.cn

[U42] PHP：PSR-4 自动加载
来源：http://fs.521024.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qr.yuntaijiaju.cn

[U43] PHP：声明命名空间
来源：http://yc.lnxyls.cn

namespace App\Http;
来源：http://ae.nszjky.cn

[U44] PHP：开启严格类型
来源：http://yh.jianghongdianzi.cn

declare(strict_types=1);
来源：http://gf.asd995.cn

[U45] PHP：类型声明与返回类型
来源：http://jz.jianghongdianzi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://yd.jianghongdianzi.cn

[U46] PHP：可空类型
来源：http://tr.colortex.cn

?string $name = null
来源：http://lp.huanxung.cn

[U47] PHP：联合类型
来源：http://cm.colortex.cn

int|string $id
来源：http://ro.panjiajie.cn

[U48] PHP：纯枚举
来源：http://zi.shxzskj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ky.szsharing.cn

[U49] PHP：只读属性
来源：http://jc.szxytkj.cn

public readonly string $name
来源：http://sq.haigaiapp.cn

[U50] PHP：构造器属性提升
来源：http://yd.huanxung.cn

public function __construct(private int $id) {}
来源：http://mk.asd995.cn

[U51] PHP：数组解构
来源：http://af.colortex.cn

[$a, $b] = $arr;
来源：http://pv.shtwfgs.cn

[U52] PHP：箭头函数
来源：http://ur.muxihuayi.cn

$double = fn($x) => $x * 2;
来源：http://ah.asd995.cn

[U53] PHP：空合并运算符
来源：http://bn.huixiangedu.cn

$v = $a ?? $b ?? "default";
来源：http://fa.huixiangedu.cn

[U54] PHP：空安全调用
来源：http://mt.huixiangedu.cn

$obj?->method()
来源：http://fd.huixiangedu.cn

[U55] PHP：match 表达式
来源：http://uy.yuntaijiaju.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pp.jctech888.com.cn

[U56] PHP：命名参数
来源：http://im.huixinmuqiang.cn

f(a: 1, b: 2)
来源：http://ik.nszjky.cn

[U57] PHP：字符串插值
来源：http://rb.huanxung.cn

"值: {$a}"
来源：http://wo.wgjwhj.cn

[U58] PHP：数组三件套
来源：http://dr.nszjky.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://st.bjjhwx.cn

[U59] PHP：自定义排序
来源：http://iy.chemitech.net.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ki.panjiajie.cn

[U60] PHP：JSON 编解码
来源：http://eq.muxihuayi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ea.nicolike.cn

[U61] PHP：正则
来源：http://ws.shxzukj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sw.9csxet.cn

[U62] PHP：日期对象
来源：http://ar.wgjwhj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ex.jctech888.com.cn

[U63] PHP：文件读写
来源：http://be.shtwfgs.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rj.huanxung.cn

[U64] PHP：目录遍历
来源：http://wz.haigaiapp.cn

glob("dir/*.php");  scandir("dir");
来源：http://ms.newstarts.cn

[U65] PHP：会话
来源：http://jy.shtwfgs.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://lu.szxytkj.cn

[U66] PHP：设置 Cookie
来源：http://wg.bookmarksfly.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xy.chemitech.net.cn

[U67] PHP：处理文件上传
来源：http://he.hahajie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vn.521024.cn

[U68] PHP：PDO 连接
来源：http://rs.szsharing.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ks.jianghongdianzi.cn

[U69] PHP：PDO 预处理
来源：http://sd.nszjky.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hj.521024.cn

[U70] PHP：PDO 事务
来源：http://vf.lnxyls.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ei.nszjky.cn

[U71] PHP：抛出异常
来源：http://yk.nicolike.cn

throw new RuntimeException("失败", 500);
来源：http://bb.asd995.cn

[U72] PHP：写错误日志
来源：http://pt.szsharing.cn

error_log("失败: " . $e->getMessage());
来源：http://op.gzmigu.cn

[U73] PHP：读取 ini 配置
来源：http://ho.jianghongdianzi.cn

parse_ini_file("config.ini", true)
来源：http://ir.szxytkj.cn

[U74] PHP：读取环境变量
来源：http://vo.szsharing.cn

getenv("APP_ENV") ?: "production"
来源：http://xd.nicolike.cn

[U75] PHP：依赖注入
来源：http://ft.jctech888.com.cn

composer require psr/container
来源：http://fa.wgjwhj.cn

[U76] PHP：简单路由
来源：http://if.lnxyls.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bj.yuntaijiaju.cn

[U77] PHP：模板渲染
来源：http://kb.panjiajie.cn

composer require twig/twig
来源：http://ac.chemitech.net.cn

[U78] PHP：单元测试
来源：http://yv.yuexingan06.cn

composer require --dev phpunit/phpunit
来源：http://nf.hnjuh.cn

[U79] PHP：静态分析
来源：http://xc.shxzukj.cn

composer require --dev phpstan/phpstan
来源：http://uh.panjiajie.cn

[U80] PHP：代码规范修复
来源：http://ud.shxzskj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://pg.gzmigu.cn

[U81] JS：初始化项目
来源：http://zj.panjiajie.cn

npm init -y;  npm i express
来源：http://eq.shxzskj.cn

[U82] JS：package.json 脚本
来源：http://hj.chemitech.net.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fs.panjiajie.cn

[U83] JS：ES Module 导入导出
来源：http://rz.bjjhwx.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zh.huixiangedu.cn

[U84] JS：CommonJS 写法
来源：http://lc.huixiangedu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ih.newstarts.cn

[U85] JS：可选链
来源：http://kq.lnxyls.cn

a?.b?.c
来源：http://we.hahajie.cn

[U86] JS：空值合并
来源：http://rz.shxzskj.cn

a ?? b
来源：http://fj.yuntaijiaju.cn

[U87] JS：解构默认值
来源：http://ps.szsharing.cn

const { a = 1, b = 2 } = obj;
来源：http://yj.521024.cn

[U88] JS：对象展开合并
来源：http://lj.bjjhwx.cn

{ ...a, ...b }
来源：http://jv.9csxet.cn

[U89] JS：数组去重
来源：http://qz.newstarts.cn

[...new Set(arr)]
来源：http://dg.bookmarksfly.cn

[U90] JS：数字数组排序
来源：http://km.521024.cn

[...arr].sort((a, b) => a - b)
来源：http://eo.9csxet.cn

[U91] JS：对象键值遍历
来源：http://hh.colortex.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xd.chemitech.net.cn

[U92] JS：深拷贝
来源：http://wk.hahajie.cn

structuredClone(obj)
来源：http://cb.bookmarksfly.cn

[U93] JS：模板字符串
来源：http://yo.chemitech.net.cn

`共 ${n} 条`
来源：http://bj.muxihuayi.cn

[U94] JS：箭头函数
来源：http://cc.szxytkj.cn

const double = x => x * 2;
来源：http://va.bjjhwx.cn

[U95] JS：Promise 包装
来源：http://dt.jctech888.com.cn

new Promise((resolve, reject) => {})
来源：http://rd.lnxyls.cn

[U96] JS：async/await 与异常
来源：http://gs.shxzskj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gv.hnjuh.cn

[U97] JS：并发请求
来源：http://qi.shxzskj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ah.jianghongdianzi.cn

[U98] JS：fetch 带 JSON
来源：http://td.bjjhwx.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mx.jctech888.com.cn

[U99] JS：事件监听
来源：http://uc.yuexingan06.cn

el.addEventListener("click", e => {})
来源：http://cj.jianghongdianzi.cn

[U100] JS：DOM 查询
来源：http://st.hahajie.cn

document.querySelector(".item")
来源：http://lm.yuntaijiaju.cn

[U101] JS：classList 操作
来源：http://no.huanxung.cn

el.classList.toggle("active")
来源：http://vb.shxzskj.cn

[U102] JS：本地存储
来源：http://ic.wgjwhj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://rb.huixiangedu.cn

[U103] JS：定时器
来源：http://ce.lnxyls.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yy.asd995.cn

[U104] JS：防抖
来源：http://dg.szxytkj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ds.hnjuh.cn

[U105] JS：节流
来源：http://lz.521024.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jl.jianghongdianzi.cn

[U106] JS：日期格式化
来源：http://fr.jctech888.com.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dn.hnjuh.cn

[U107] JS：数字千分位
来源：http://vj.szxytkj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ul.szxytkj.cn

[U108] JS：随机整数
来源：http://cv.jianghongdianzi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xt.hnjuh.cn

[U109] JS：数组分组
来源：http://ml.szxytkj.cn

Object.groupBy(arr, x => x.type)
来源：http://ll.bookmarksfly.cn

[U110] JS：数组分块
来源：http://bm.hnjuh.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xd.hnjuh.cn

[U111] JS：对象转 Map
来源：http://bg.hahajie.cn

new Map(Object.entries(obj))
来源：http://kv.huixinmuqiang.cn

[U112] JS：字符串补位
来源：http://vz.huixinmuqiang.cn

"7".padStart(3, "0")
来源：http://qh.szsharing.cn


<!-- 参考信息 -->