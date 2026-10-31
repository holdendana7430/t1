代发 wailian999

[T25] Swift：结构体
来源：http://vz.521024.cn

struct P { var x: Int }
来源：http://rf.szsharing.cn

[T26] Swift：类与重写
来源：http://do.haigaiapp.cn

class A: Base { override func f() {} }
来源：http://ao.shxzukj.cn

[T27] Swift：错误处理
来源：http://fh.gzmigu.cn

do { try f() } catch { print(error) }
来源：http://wg.shxzskj.cn

[T28] Swift：枚举
来源：http://je.yuntaijiaju.cn

enum Color { case red, green }
来源：http://ij.panjiajie.cn

[T29] Swift：guard 提前返回
来源：http://go.gzmigu.cn

guard let x = opt else { return }
来源：http://jk.gzmigu.cn

[T30] Swift：协议
来源：http://nw.nszjky.cn

protocol Shape { func area() -> Double }
来源：http://kk.hahajie.cn

[T31] Lua：Hello World
来源：http://dw.hahajie.cn

print("Hello")
来源：http://sq.shxzukj.cn

[T32] Lua：局部变量
来源：http://vl.bjjhwx.cn

local a = 1
来源：http://vr.shxzukj.cn

[T33] Lua：表（数组）
来源：http://wd.521024.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://tm.yuexingan06.cn

[T34] Lua：遍历表
来源：http://dq.bookmarksfly.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ic.jianghongdianzi.cn

[T35] Lua：字典表
来源：http://kl.jctech888.com.cn

local d = { a = 1 };  d.b = 2
来源：http://xj.bjjhwx.cn

[T36] Lua：函数
来源：http://zf.gzmigu.cn

function add(a, b) return a + b end
来源：http://gr.newstarts.cn

[T37] Lua：字符串拼接
来源：http://tf.newstarts.cn

"a" .. "b"
来源：http://gy.gzmigu.cn

[T38] Lua：条件
来源：http://dn.9csxet.cn

if x > 0 then print("正") end
来源：http://gw.huixiangedu.cn

[T39] Lua：模式匹配
来源：http://ta.newstarts.cn

string.find(s, "%d+")
来源：http://wq.huanxung.cn

[T40] Lua：元表
来源：http://gz.hnjuh.cn

setmetatable({}, { __index = base })
来源：http://tr.hahajie.cn

[T41] Perl：Hello World
来源：http://py.lnxyls.cn

print "Hello\n";
来源：http://ew.bjjhwx.cn

[T42] Perl：变量类型
来源：http://jb.hahajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jz.hahajie.cn

[T43] Perl：字符串插值
来源：http://gj.bookmarksfly.cn

"值: $a"
来源：http://oo.jctech888.com.cn

[T44] Perl：条件
来源：http://im.lnxyls.cn

if ($a > 0) { print "正"; }
来源：http://as.yuntaijiaju.cn

[T45] Perl：数组遍历
来源：http://zg.huixiangedu.cn

for my $x (@arr) { print $x; }
来源：http://cc.szxytkj.cn

[T46] Perl：哈希操作
来源：http://cc.huixinmuqiang.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://es.shtwfgs.cn

[T47] Perl：正则捕获
来源：http://ys.bookmarksfly.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://et.yuntaijiaju.cn

[T48] Perl：正则替换
来源：http://rg.szsharing.cn

$s =~ s/old/new/g;
来源：http://gg.szxytkj.cn

[T49] Perl：函数
来源：http://vs.wgjwhj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://br.jctech888.com.cn

[T50] Perl：逐行读文件
来源：http://zl.hnjuh.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://df.newstarts.cn

while (my $line = <$fh>) { print $line; }
来源：http://ic.panjiajie.cn

[T51] Scala：Hello World
来源：http://rq.muxihuayi.cn

println("Hello")
来源：http://dt.gzmigu.cn

[T52] Scala：变量
来源：http://zf.gzmigu.cn

val a = 1;  var b = 2
来源：http://pu.shxzskj.cn

[T53] Scala：字符串插值
来源：http://ti.szsharing.cn

s"值: $b"
来源：http://yu.asd995.cn

[T54] Scala：集合映射
来源：http://rf.shtwfgs.cn

List(1, 2, 3).map(_ * 2)
来源：http://bs.chemitech.net.cn

[T55] Scala：集合过滤
来源：http://zm.hahajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://rm.huixinmuqiang.cn

[T56] Scala：样例类
来源：http://bm.9csxet.cn

case class User(name: String, age: Int)
来源：http://lj.shtwfgs.cn

[T57] Scala：模式匹配
来源：http://mo.huixiangedu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://en.521024.cn

[T58] Scala：函数定义
来源：http://hp.muxihuayi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zy.jianghongdianzi.cn

[T59] Scala：循环
来源：http://eq.shxzskj.cn

for (i <- 1 to 10) println(i)
来源：http://mq.gzmigu.cn

[T60] Scala：折叠
来源：http://oq.gzmigu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tb.lnxyls.cn

================================================================================
来源：http://vy.shxzskj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://el.nszjky.cn

================================================================================
来源：http://ey.shxzskj.cn

[U01] Py：创建虚拟环境
来源：http://mt.wgjwhj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://pf.newstarts.cn

[U02] Py：导出 / 安装依赖
来源：http://vj.nicolike.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mp.gzmigu.cn

[U03] Py：加载 .env 配置
来源：http://qv.nicolike.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zp.9csxet.cn

[U04] Py：变量调试打印
来源：http://tr.haigaiapp.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rx.szsharing.cn

[U05] Py：列表去重且保序
来源：http://uc.shxzskj.cn

list(dict.fromkeys(arr))
来源：http://zv.nicolike.cn

[U06] Py：合并两个字典
来源：http://ve.521024.cn

{**a, **b}
来源：http://gb.jctech888.com.cn

[U07] Py：反转字典键值
来源：http://zf.jianghongdianzi.cn

{v: k for k, v in d.items()}
来源：http://ig.shtwfgs.cn

[U08] Py：展平二维列表
来源：http://uj.shxzskj.cn

[y for x in nested for y in x]
来源：http://ef.jctech888.com.cn

[U09] Py：字典取最大值的键
来源：http://su.nicolike.cn

max(d, key=d.get)
来源：http://ow.shtwfgs.cn

[U10] Py：按值排序字典
来源：http://js.szxytkj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mx.yuexingan06.cn

[U11] Py：生成器表达式
来源：http://ui.yuntaijiaju.cn

(x * 2 for x in arr)
来源：http://ln.lnxyls.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ld.bjjhwx.cn

Counter(arr).most_common(3)
来源：http://eq.jianghongdianzi.cn

[U13] Py：固定长度队列
来源：http://vc.newstarts.cn

deque(maxlen=10)
来源：http://rb.huixiangedu.cn

[U14] Py：分组收集到列表
来源：http://wj.lnxyls.cn

defaultdict(list)
来源：http://hw.colortex.cn

[U15] Py：高精度计时
来源：http://px.nszjky.cn

t = time.perf_counter()
来源：http://ih.wgjwhj.cn

[U16] Py：命令行参数解析
来源：http://wx.gzmigu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://th.hahajie.cn

[U17] Py：初始化日志
来源：http://yf.jctech888.com.cn

logging.basicConfig(level=logging.INFO)
来源：http://jz.9csxet.cn

[U18] Py：预编译正则
来源：http://gu.shxzskj.cn

pat = re.compile(r"\d+")
来源：http://yr.muxihuayi.cn

[U19] Py：正则替换带回调
来源：http://lb.nszjky.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ge.hnjuh.cn

[U20] Py：缓存函数结果
来源：http://mw.521024.cn

@functools.lru_cache(maxsize=None)
来源：http://ic.yuexingan06.cn

[U21] Py：自定义上下文管理器
来源：http://sg.bjjhwx.cn

@contextlib.contextmanager
来源：http://nz.panjiajie.cn

[U22] Py：矩阵转置
来源：http://wo.nszjky.cn

list(zip(*m))
来源：http://qe.huixinmuqiang.cn

[U23] Py：分块读取大文件
来源：http://vk.huixinmuqiang.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://od.chemitech.net.cn

[U24] Py：路径操作
来源：http://ru.yuexingan06.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ju.nicolike.cn

[U25] Py：CSV 按字典读
来源：http://qg.newstarts.cn

csv.DictReader(f)
来源：http://gx.huixiangedu.cn

[U26] Py：并发下载
来源：http://rs.jctech888.com.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bs.haigaiapp.cn

[U27] Py：异步 HTTP
来源：http://jd.nszjky.cn

aiohttp.ClientSession() 配合 async with
来源：http://kl.szsharing.cn

[U28] Py：类型别名
来源：http://em.shxzskj.cn

UserId = int
来源：http://yj.jctech888.com.cn

[U29] Py：属性校验
来源：http://id.panjiajie.cn

@property 与 @x.setter 配合
来源：http://np.yuntaijiaju.cn

[U30] Py：数据类
来源：http://fd.yuexingan06.cn

@dataclass(slots=True)
来源：http://qf.haigaiapp.cn

[U31] Py：单测
来源：http://hn.hahajie.cn

python -m pytest -q
来源：http://wh.shtwfgs.cn

[U32] Py：代码格式化
来源：http://ux.jctech888.com.cn

ruff format . && ruff check --fix .
来源：http://fl.shxzskj.cn

[U33] Py：打包发布
来源：http://dr.szxytkj.cn

python -m build  （依赖 pyproject.toml）
来源：http://vl.colortex.cn

[U34] Py：判断编码
来源：http://th.bookmarksfly.cn

chardet.detect(raw)
来源：http://ch.muxihuayi.cn

[U35] Py：发送邮件
来源：http://pj.lnxyls.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://og.lnxyls.cn

[U36] Py：定时任务
来源：http://ru.jctech888.com.cn

schedule.every(10).minutes.do(job)
来源：http://vv.huixinmuqiang.cn

[U37] Py：读写 Excel
来源：http://hb.nicolike.cn

pandas.read_excel / DataFrame.to_excel
来源：http://vg.hnjuh.cn

[U38] Py：获取脚本所在目录
来源：http://ge.muxihuayi.cn

Path(__file__).resolve().parent
来源：http://fo.shxzskj.cn

[U39] Py：判断是否在交互环境
来源：http://hs.bookmarksfly.cn

sys.stdout.isatty()
来源：http://wb.szxytkj.cn

[U40] Py：打印到标准错误
来源：http://va.9csxet.cn

print("err", file=sys.stderr)
来源：http://dl.yuntaijiaju.cn

[U41] PHP：初始化 Composer 项目
来源：http://pp.hahajie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ji.wgjwhj.cn

[U42] PHP：PSR-4 自动加载
来源：http://ir.huixiangedu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vv.chemitech.net.cn

[U43] PHP：声明命名空间
来源：http://ds.521024.cn

namespace App\Http;
来源：http://mr.newstarts.cn

[U44] PHP：开启严格类型
来源：http://fs.shtwfgs.cn

declare(strict_types=1);
来源：http://rq.huixiangedu.cn

[U45] PHP：类型声明与返回类型
来源：http://ni.chemitech.net.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://em.szsharing.cn

[U46] PHP：可空类型
来源：http://so.muxihuayi.cn

?string $name = null
来源：http://un.9csxet.cn

[U47] PHP：联合类型
来源：http://ah.muxihuayi.cn

int|string $id
来源：http://rp.yuexingan06.cn

[U48] PHP：纯枚举
来源：http://bh.newstarts.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kc.bjjhwx.cn

[U49] PHP：只读属性
来源：http://ro.muxihuayi.cn

public readonly string $name
来源：http://gr.newstarts.cn

[U50] PHP：构造器属性提升
来源：http://cs.muxihuayi.cn

public function __construct(private int $id) {}
来源：http://xg.asd995.cn

[U51] PHP：数组解构
来源：http://vb.shtwfgs.cn

[$a, $b] = $arr;
来源：http://en.yuexingan06.cn

[U52] PHP：箭头函数
来源：http://vs.nicolike.cn

$double = fn($x) => $x * 2;
来源：http://aq.lnxyls.cn

[U53] PHP：空合并运算符
来源：http://md.shxzskj.cn

$v = $a ?? $b ?? "default";
来源：http://yq.hahajie.cn

[U54] PHP：空安全调用
来源：http://oy.bjjhwx.cn

$obj?->method()
来源：http://zl.521024.cn

[U55] PHP：match 表达式
来源：http://cj.huixiangedu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ul.szxytkj.cn

[U56] PHP：命名参数
来源：http://qa.szsharing.cn

f(a: 1, b: 2)
来源：http://xq.yuexingan06.cn

[U57] PHP：字符串插值
来源：http://bl.yuntaijiaju.cn

"值: {$a}"
来源：http://rl.huanxung.cn

[U58] PHP：数组三件套
来源：http://nf.asd995.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wk.haigaiapp.cn

[U59] PHP：自定义排序
来源：http://gd.jctech888.com.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ho.shtwfgs.cn

[U60] PHP：JSON 编解码
来源：http://om.shtwfgs.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cn.newstarts.cn

[U61] PHP：正则
来源：http://ll.bjjhwx.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://oz.huanxung.cn

[U62] PHP：日期对象
来源：http://km.szxytkj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tj.muxihuayi.cn

[U63] PHP：文件读写
来源：http://ia.huanxung.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hg.hahajie.cn

[U64] PHP：目录遍历
来源：http://et.shtwfgs.cn

glob("dir/*.php");  scandir("dir");
来源：http://vf.panjiajie.cn

[U65] PHP：会话
来源：http://la.nszjky.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://fd.nicolike.cn

[U66] PHP：设置 Cookie
来源：http://cz.newstarts.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tg.bjjhwx.cn

[U67] PHP：处理文件上传
来源：http://pn.lnxyls.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jc.nszjky.cn

[U68] PHP：PDO 连接
来源：http://ep.nicolike.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ji.panjiajie.cn

[U69] PHP：PDO 预处理
来源：http://ws.521024.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vk.nszjky.cn

[U70] PHP：PDO 事务
来源：http://or.panjiajie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hm.521024.cn

[U71] PHP：抛出异常
来源：http://ke.newstarts.cn

throw new RuntimeException("失败", 500);
来源：http://jr.szxytkj.cn

[U72] PHP：写错误日志
来源：http://iy.newstarts.cn

error_log("失败: " . $e->getMessage());
来源：http://dp.bookmarksfly.cn

[U73] PHP：读取 ini 配置
来源：http://sq.szsharing.cn

parse_ini_file("config.ini", true)
来源：http://xf.szsharing.cn

[U74] PHP：读取环境变量
来源：http://sl.nszjky.cn

getenv("APP_ENV") ?: "production"
来源：http://jz.jianghongdianzi.cn

[U75] PHP：依赖注入
来源：http://af.chemitech.net.cn

composer require psr/container
来源：http://sk.wgjwhj.cn

[U76] PHP：简单路由
来源：http://if.huixiangedu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ve.colortex.cn

[U77] PHP：模板渲染
来源：http://ks.jctech888.com.cn

composer require twig/twig
来源：http://vh.lnxyls.cn

[U78] PHP：单元测试
来源：http://vg.jctech888.com.cn

composer require --dev phpunit/phpunit
来源：http://op.jctech888.com.cn

[U79] PHP：静态分析
来源：http://tg.hahajie.cn

composer require --dev phpstan/phpstan
来源：http://zl.nszjky.cn

[U80] PHP：代码规范修复
来源：http://tk.521024.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://hs.521024.cn

[U81] JS：初始化项目
来源：http://ue.nicolike.cn

npm init -y;  npm i express
来源：http://yu.hahajie.cn

[U82] JS：package.json 脚本
来源：http://mi.huixinmuqiang.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zv.hnjuh.cn

[U83] JS：ES Module 导入导出
来源：http://jh.nicolike.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ow.shxzskj.cn

[U84] JS：CommonJS 写法
来源：http://vl.panjiajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://cf.jianghongdianzi.cn

[U85] JS：可选链
来源：http://jj.nicolike.cn

a?.b?.c
来源：http://fk.bjjhwx.cn

[U86] JS：空值合并
来源：http://kq.lnxyls.cn

a ?? b
来源：http://ih.haigaiapp.cn

[U87] JS：解构默认值
来源：http://pn.bookmarksfly.cn

const { a = 1, b = 2 } = obj;
来源：http://dx.chemitech.net.cn

[U88] JS：对象展开合并
来源：http://gt.jianghongdianzi.cn

{ ...a, ...b }
来源：http://td.huixiangedu.cn

[U89] JS：数组去重
来源：http://zl.szxytkj.cn

[...new Set(arr)]
来源：http://wj.nszjky.cn

[U90] JS：数字数组排序
来源：http://ae.huixinmuqiang.cn

[...arr].sort((a, b) => a - b)
来源：http://pk.jianghongdianzi.cn

[U91] JS：对象键值遍历
来源：http://wb.huixiangedu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ls.colortex.cn

[U92] JS：深拷贝
来源：http://fe.wgjwhj.cn

structuredClone(obj)
来源：http://qd.shxzukj.cn

[U93] JS：模板字符串
来源：http://sl.yuntaijiaju.cn

`共 ${n} 条`
来源：http://cu.shtwfgs.cn

[U94] JS：箭头函数
来源：http://ry.huixinmuqiang.cn

const double = x => x * 2;
来源：http://fr.huixinmuqiang.cn

[U95] JS：Promise 包装
来源：http://gm.9csxet.cn

new Promise((resolve, reject) => {})
来源：http://vp.521024.cn

[U96] JS：async/await 与异常
来源：http://xm.szxytkj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://by.yuexingan06.cn

[U97] JS：并发请求
来源：http://xn.jctech888.com.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ar.wgjwhj.cn

[U98] JS：fetch 带 JSON
来源：http://xl.hnjuh.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ua.jianghongdianzi.cn

[U99] JS：事件监听
来源：http://uk.bookmarksfly.cn

el.addEventListener("click", e => {})
来源：http://kk.lnxyls.cn

[U100] JS：DOM 查询
来源：http://oq.huixiangedu.cn

document.querySelector(".item")
来源：http://tf.colortex.cn

[U101] JS：classList 操作
来源：http://ws.9csxet.cn

el.classList.toggle("active")
来源：http://gu.jctech888.com.cn

[U102] JS：本地存储
来源：http://zh.shtwfgs.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://mq.szsharing.cn

[U103] JS：定时器
来源：http://ok.wgjwhj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lc.newstarts.cn

[U104] JS：防抖
来源：http://bv.shtwfgs.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gw.asd995.cn

[U105] JS：节流
来源：http://wh.521024.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tq.nszjky.cn

[U106] JS：日期格式化
来源：http://yp.muxihuayi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gv.jctech888.com.cn

[U107] JS：数字千分位
来源：http://wr.9csxet.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yy.huanxung.cn

[U108] JS：随机整数
来源：http://ye.wgjwhj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dg.lnxyls.cn

[U109] JS：数组分组
来源：http://ri.yuexingan06.cn

Object.groupBy(arr, x => x.type)
来源：http://eq.nicolike.cn

[U110] JS：数组分块
来源：http://yg.gzmigu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://da.bookmarksfly.cn

[U111] JS：对象转 Map
来源：http://nr.muxihuayi.cn

new Map(Object.entries(obj))
来源：http://uu.szsharing.cn

[U112] JS：字符串补位
来源：http://nw.jianghongdianzi.cn

"7".padStart(3, "0")
来源：http://hz.shtwfgs.cn


<!-- 参考信息 -->