代发 wailian999

[T27] Swift：错误处理
来源：http://or.jianghongdianzi.cn

do { try f() } catch { print(error) }
来源：http://cq.9csxet.cn

[T28] Swift：枚举
来源：http://lu.wgjwhj.cn

enum Color { case red, green }
来源：http://ex.wgjwhj.cn

[T29] Swift：guard 提前返回
来源：http://tn.521024.cn

guard let x = opt else { return }
来源：http://eh.colortex.cn

[T30] Swift：协议
来源：http://au.chemitech.net.cn

protocol Shape { func area() -> Double }
来源：http://ys.huixiangedu.cn

[T31] Lua：Hello World
来源：http://xv.bookmarksfly.cn

print("Hello")
来源：http://zm.yuntaijiaju.cn

[T32] Lua：局部变量
来源：http://br.chemitech.net.cn

local a = 1
来源：http://ck.huixiangedu.cn

[T33] Lua：表（数组）
来源：http://ux.yuntaijiaju.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://dp.colortex.cn

[T34] Lua：遍历表
来源：http://sq.huixinmuqiang.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://cj.hnjuh.cn

[T35] Lua：字典表
来源：http://tr.lnxyls.cn

local d = { a = 1 };  d.b = 2
来源：http://th.bookmarksfly.cn

[T36] Lua：函数
来源：http://lj.nszjky.cn

function add(a, b) return a + b end
来源：http://tq.wgjwhj.cn

[T37] Lua：字符串拼接
来源：http://di.nszjky.cn

"a" .. "b"
来源：http://zh.shxzukj.cn

[T38] Lua：条件
来源：http://tq.muxihuayi.cn

if x > 0 then print("正") end
来源：http://rq.nszjky.cn

[T39] Lua：模式匹配
来源：http://gv.shtwfgs.cn

string.find(s, "%d+")
来源：http://jv.huixiangedu.cn

[T40] Lua：元表
来源：http://vz.shxzukj.cn

setmetatable({}, { __index = base })
来源：http://dj.szsharing.cn

[T41] Perl：Hello World
来源：http://xj.muxihuayi.cn

print "Hello\n";
来源：http://ls.jianghongdianzi.cn

[T42] Perl：变量类型
来源：http://iw.jianghongdianzi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ul.bookmarksfly.cn

[T43] Perl：字符串插值
来源：http://li.panjiajie.cn

"值: $a"
来源：http://cy.shxzukj.cn

[T44] Perl：条件
来源：http://tp.shxzskj.cn

if ($a > 0) { print "正"; }
来源：http://tw.colortex.cn

[T45] Perl：数组遍历
来源：http://rt.gzmigu.cn

for my $x (@arr) { print $x; }
来源：http://tk.chemitech.net.cn

[T46] Perl：哈希操作
来源：http://qp.asd995.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://re.huixiangedu.cn

[T47] Perl：正则捕获
来源：http://fb.yuntaijiaju.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qt.shxzukj.cn

[T48] Perl：正则替换
来源：http://ay.muxihuayi.cn

$s =~ s/old/new/g;
来源：http://ex.yuntaijiaju.cn

[T49] Perl：函数
来源：http://ia.shtwfgs.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tr.panjiajie.cn

[T50] Perl：逐行读文件
来源：http://sp.colortex.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://kl.huixiangedu.cn

while (my $line = <$fh>) { print $line; }
来源：http://ww.szsharing.cn

[T51] Scala：Hello World
来源：http://gm.asd995.cn

println("Hello")
来源：http://eh.jctech888.com.cn

[T52] Scala：变量
来源：http://yu.shtwfgs.cn

val a = 1;  var b = 2
来源：http://sd.gzmigu.cn

[T53] Scala：字符串插值
来源：http://jj.jianghongdianzi.cn

s"值: $b"
来源：http://vu.nszjky.cn

[T54] Scala：集合映射
来源：http://dy.wgjwhj.cn

List(1, 2, 3).map(_ * 2)
来源：http://op.521024.cn

[T55] Scala：集合过滤
来源：http://hb.bjjhwx.cn

List(1, 2, 3).filter(_ > 1)
来源：http://nw.jctech888.com.cn

[T56] Scala：样例类
来源：http://an.nicolike.cn

case class User(name: String, age: Int)
来源：http://fq.jctech888.com.cn

[T57] Scala：模式匹配
来源：http://el.shxzukj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vn.jianghongdianzi.cn

[T58] Scala：函数定义
来源：http://uu.huixinmuqiang.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ah.nszjky.cn

[T59] Scala：循环
来源：http://zr.panjiajie.cn

for (i <- 1 to 10) println(i)
来源：http://cc.panjiajie.cn

[T60] Scala：折叠
来源：http://km.nicolike.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rf.shxzskj.cn

================================================================================
来源：http://pp.newstarts.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kk.jianghongdianzi.cn

================================================================================
来源：http://ss.bookmarksfly.cn

[U01] Py：创建虚拟环境
来源：http://cf.nszjky.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ru.jianghongdianzi.cn

[U02] Py：导出 / 安装依赖
来源：http://ts.nicolike.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dc.yuntaijiaju.cn

[U03] Py：加载 .env 配置
来源：http://ab.shxzskj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ys.colortex.cn

[U04] Py：变量调试打印
来源：http://et.jianghongdianzi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kf.bookmarksfly.cn

[U05] Py：列表去重且保序
来源：http://hs.szxytkj.cn

list(dict.fromkeys(arr))
来源：http://cc.szxytkj.cn

[U06] Py：合并两个字典
来源：http://rb.huixinmuqiang.cn

{**a, **b}
来源：http://rg.gzmigu.cn

[U07] Py：反转字典键值
来源：http://lr.bookmarksfly.cn

{v: k for k, v in d.items()}
来源：http://ur.szsharing.cn

[U08] Py：展平二维列表
来源：http://nz.jctech888.com.cn

[y for x in nested for y in x]
来源：http://xc.shxzukj.cn

[U09] Py：字典取最大值的键
来源：http://fc.yuntaijiaju.cn

max(d, key=d.get)
来源：http://hn.yuntaijiaju.cn

[U10] Py：按值排序字典
来源：http://vs.nszjky.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sw.huixinmuqiang.cn

[U11] Py：生成器表达式
来源：http://sh.huixinmuqiang.cn

(x * 2 for x in arr)
来源：http://lu.wgjwhj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qg.shtwfgs.cn

Counter(arr).most_common(3)
来源：http://ij.shxzskj.cn

[U13] Py：固定长度队列
来源：http://se.wgjwhj.cn

deque(maxlen=10)
来源：http://nj.chemitech.net.cn

[U14] Py：分组收集到列表
来源：http://ps.jianghongdianzi.cn

defaultdict(list)
来源：http://tu.nszjky.cn

[U15] Py：高精度计时
来源：http://xi.nszjky.cn

t = time.perf_counter()
来源：http://xw.newstarts.cn

[U16] Py：命令行参数解析
来源：http://pk.muxihuayi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yf.huixiangedu.cn

[U17] Py：初始化日志
来源：http://gb.jctech888.com.cn

logging.basicConfig(level=logging.INFO)
来源：http://yd.shxzukj.cn

[U18] Py：预编译正则
来源：http://fl.bjjhwx.cn

pat = re.compile(r"\d+")
来源：http://ye.hnjuh.cn

[U19] Py：正则替换带回调
来源：http://yt.9csxet.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gc.yuntaijiaju.cn

[U20] Py：缓存函数结果
来源：http://fx.asd995.cn

@functools.lru_cache(maxsize=None)
来源：http://pi.jianghongdianzi.cn

[U21] Py：自定义上下文管理器
来源：http://ue.shxzskj.cn

@contextlib.contextmanager
来源：http://xw.lnxyls.cn

[U22] Py：矩阵转置
来源：http://nq.shtwfgs.cn

list(zip(*m))
来源：http://ib.lnxyls.cn

[U23] Py：分块读取大文件
来源：http://ea.jctech888.com.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lq.shxzskj.cn

[U24] Py：路径操作
来源：http://wm.gzmigu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xg.521024.cn

[U25] Py：CSV 按字典读
来源：http://iz.jctech888.com.cn

csv.DictReader(f)
来源：http://iy.9csxet.cn

[U26] Py：并发下载
来源：http://rq.jianghongdianzi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wq.bookmarksfly.cn

[U27] Py：异步 HTTP
来源：http://gp.bjjhwx.cn

aiohttp.ClientSession() 配合 async with
来源：http://cl.shxzskj.cn

[U28] Py：类型别名
来源：http://hb.nszjky.cn

UserId = int
来源：http://ci.panjiajie.cn

[U29] Py：属性校验
来源：http://gv.wgjwhj.cn

@property 与 @x.setter 配合
来源：http://wx.hahajie.cn

[U30] Py：数据类
来源：http://xm.shtwfgs.cn

@dataclass(slots=True)
来源：http://xs.hnjuh.cn

[U31] Py：单测
来源：http://ly.nszjky.cn

python -m pytest -q
来源：http://uo.nszjky.cn

[U32] Py：代码格式化
来源：http://kj.szxytkj.cn

ruff format . && ruff check --fix .
来源：http://xt.wgjwhj.cn

[U33] Py：打包发布
来源：http://dn.hahajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://mf.yuexingan06.cn

[U34] Py：判断编码
来源：http://wl.colortex.cn

chardet.detect(raw)
来源：http://os.huanxung.cn

[U35] Py：发送邮件
来源：http://jp.colortex.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gk.jianghongdianzi.cn

[U36] Py：定时任务
来源：http://qs.lnxyls.cn

schedule.every(10).minutes.do(job)
来源：http://bi.newstarts.cn

[U37] Py：读写 Excel
来源：http://nn.panjiajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://xm.bookmarksfly.cn

[U38] Py：获取脚本所在目录
来源：http://at.nszjky.cn

Path(__file__).resolve().parent
来源：http://gy.nszjky.cn

[U39] Py：判断是否在交互环境
来源：http://fq.bjjhwx.cn

sys.stdout.isatty()
来源：http://sb.yuntaijiaju.cn

[U40] Py：打印到标准错误
来源：http://zo.huanxung.cn

print("err", file=sys.stderr)
来源：http://gy.hnjuh.cn

[U41] PHP：初始化 Composer 项目
来源：http://bs.bookmarksfly.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://lb.szsharing.cn

[U42] PHP：PSR-4 自动加载
来源：http://te.bookmarksfly.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qt.bjjhwx.cn

[U43] PHP：声明命名空间
来源：http://tp.szxytkj.cn

namespace App\Http;
来源：http://xb.muxihuayi.cn

[U44] PHP：开启严格类型
来源：http://ov.huixiangedu.cn

declare(strict_types=1);
来源：http://xn.huixiangedu.cn

[U45] PHP：类型声明与返回类型
来源：http://yb.jctech888.com.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://xf.muxihuayi.cn

[U46] PHP：可空类型
来源：http://wq.colortex.cn

?string $name = null
来源：http://iv.haigaiapp.cn

[U47] PHP：联合类型
来源：http://ma.haigaiapp.cn

int|string $id
来源：http://lm.haigaiapp.cn

[U48] PHP：纯枚举
来源：http://iz.huixinmuqiang.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://on.lnxyls.cn

[U49] PHP：只读属性
来源：http://jb.hahajie.cn

public readonly string $name
来源：http://kq.gzmigu.cn

[U50] PHP：构造器属性提升
来源：http://yj.bjjhwx.cn

public function __construct(private int $id) {}
来源：http://wq.jianghongdianzi.cn

[U51] PHP：数组解构
来源：http://ju.shxzskj.cn

[$a, $b] = $arr;
来源：http://vf.chemitech.net.cn

[U52] PHP：箭头函数
来源：http://dp.yuntaijiaju.cn

$double = fn($x) => $x * 2;
来源：http://po.jctech888.com.cn

[U53] PHP：空合并运算符
来源：http://ud.yuexingan06.cn

$v = $a ?? $b ?? "default";
来源：http://yu.huanxung.cn

[U54] PHP：空安全调用
来源：http://ze.asd995.cn

$obj?->method()
来源：http://ap.shxzskj.cn

[U55] PHP：match 表达式
来源：http://qd.bjjhwx.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fs.521024.cn

[U56] PHP：命名参数
来源：http://qh.bookmarksfly.cn

f(a: 1, b: 2)
来源：http://do.hahajie.cn

[U57] PHP：字符串插值
来源：http://vb.bookmarksfly.cn

"值: {$a}"
来源：http://lj.nicolike.cn

[U58] PHP：数组三件套
来源：http://nm.colortex.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hi.panjiajie.cn

[U59] PHP：自定义排序
来源：http://uu.huixinmuqiang.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nv.9csxet.cn

[U60] PHP：JSON 编解码
来源：http://qe.yuexingan06.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cd.colortex.cn

[U61] PHP：正则
来源：http://og.huixiangedu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wr.asd995.cn

[U62] PHP：日期对象
来源：http://pm.szsharing.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ar.bjjhwx.cn

[U63] PHP：文件读写
来源：http://mp.hnjuh.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sb.shxzskj.cn

[U64] PHP：目录遍历
来源：http://ei.wgjwhj.cn

glob("dir/*.php");  scandir("dir");
来源：http://is.shxzskj.cn

[U65] PHP：会话
来源：http://bb.huanxung.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ze.jctech888.com.cn

[U66] PHP：设置 Cookie
来源：http://mc.colortex.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ru.shtwfgs.cn

[U67] PHP：处理文件上传
来源：http://ta.muxihuayi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mc.9csxet.cn

[U68] PHP：PDO 连接
来源：http://bw.colortex.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yk.nszjky.cn

[U69] PHP：PDO 预处理
来源：http://lc.gzmigu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dx.nszjky.cn

[U70] PHP：PDO 事务
来源：http://oj.szxytkj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fn.9csxet.cn

[U71] PHP：抛出异常
来源：http://nw.hnjuh.cn

throw new RuntimeException("失败", 500);
来源：http://dh.shtwfgs.cn

[U72] PHP：写错误日志
来源：http://je.colortex.cn

error_log("失败: " . $e->getMessage());
来源：http://pc.shxzskj.cn

[U73] PHP：读取 ini 配置
来源：http://bz.colortex.cn

parse_ini_file("config.ini", true)
来源：http://fh.jctech888.com.cn

[U74] PHP：读取环境变量
来源：http://fz.szsharing.cn

getenv("APP_ENV") ?: "production"
来源：http://js.jianghongdianzi.cn

[U75] PHP：依赖注入
来源：http://uz.hnjuh.cn

composer require psr/container
来源：http://pg.bookmarksfly.cn

[U76] PHP：简单路由
来源：http://at.colortex.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://eo.wgjwhj.cn

[U77] PHP：模板渲染
来源：http://kc.muxihuayi.cn

composer require twig/twig
来源：http://nc.jianghongdianzi.cn

[U78] PHP：单元测试
来源：http://qf.shxzukj.cn

composer require --dev phpunit/phpunit
来源：http://qu.521024.cn

[U79] PHP：静态分析
来源：http://lu.jianghongdianzi.cn

composer require --dev phpstan/phpstan
来源：http://ni.jianghongdianzi.cn

[U80] PHP：代码规范修复
来源：http://gr.wgjwhj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://si.nicolike.cn

[U81] JS：初始化项目
来源：http://qx.wgjwhj.cn

npm init -y;  npm i express
来源：http://vo.jctech888.com.cn

[U82] JS：package.json 脚本
来源：http://if.panjiajie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ws.shxzskj.cn

[U83] JS：ES Module 导入导出
来源：http://td.chemitech.net.cn

export const a = 1;  import { a } from "./m.js";
来源：http://nh.shtwfgs.cn

[U84] JS：CommonJS 写法
来源：http://jw.hnjuh.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ci.nicolike.cn

[U85] JS：可选链
来源：http://ar.jctech888.com.cn

a?.b?.c
来源：http://cx.lnxyls.cn

[U86] JS：空值合并
来源：http://sj.bjjhwx.cn

a ?? b
来源：http://rb.asd995.cn

[U87] JS：解构默认值
来源：http://xi.shxzskj.cn

const { a = 1, b = 2 } = obj;
来源：http://uc.yuexingan06.cn

[U88] JS：对象展开合并
来源：http://ns.asd995.cn

{ ...a, ...b }
来源：http://pd.huixiangedu.cn

[U89] JS：数组去重
来源：http://js.colortex.cn

[...new Set(arr)]
来源：http://sx.newstarts.cn

[U90] JS：数字数组排序
来源：http://eu.jianghongdianzi.cn

[...arr].sort((a, b) => a - b)
来源：http://vg.muxihuayi.cn

[U91] JS：对象键值遍历
来源：http://vd.9csxet.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ss.yuntaijiaju.cn

[U92] JS：深拷贝
来源：http://ad.muxihuayi.cn

structuredClone(obj)
来源：http://co.yuexingan06.cn

[U93] JS：模板字符串
来源：http://cx.asd995.cn

`共 ${n} 条`
来源：http://ot.shxzskj.cn

[U94] JS：箭头函数
来源：http://td.521024.cn

const double = x => x * 2;
来源：http://kj.huanxung.cn

[U95] JS：Promise 包装
来源：http://pc.colortex.cn

new Promise((resolve, reject) => {})
来源：http://oa.newstarts.cn

[U96] JS：async/await 与异常
来源：http://ok.huixinmuqiang.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://eh.colortex.cn

[U97] JS：并发请求
来源：http://jx.bjjhwx.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://py.bjjhwx.cn

[U98] JS：fetch 带 JSON
来源：http://ef.asd995.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.shxzskj.cn

[U99] JS：事件监听
来源：http://fg.jctech888.com.cn

el.addEventListener("click", e => {})
来源：http://sl.hahajie.cn

[U100] JS：DOM 查询
来源：http://mo.lnxyls.cn

document.querySelector(".item")
来源：http://kn.huixinmuqiang.cn

[U101] JS：classList 操作
来源：http://rw.hahajie.cn

el.classList.toggle("active")
来源：http://cr.gzmigu.cn

[U102] JS：本地存储
来源：http://mi.9csxet.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://tk.shxzskj.cn

[U103] JS：定时器
来源：http://yv.shtwfgs.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://cu.shxzskj.cn

[U104] JS：防抖
来源：http://fr.szsharing.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uo.gzmigu.cn

[U105] JS：节流
来源：http://ou.asd995.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rx.wgjwhj.cn

[U106] JS：日期格式化
来源：http://zm.szxytkj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ci.yuntaijiaju.cn

[U107] JS：数字千分位
来源：http://dc.chemitech.net.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lv.jianghongdianzi.cn

[U108] JS：随机整数
来源：http://ya.lnxyls.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qn.newstarts.cn

[U109] JS：数组分组
来源：http://qv.asd995.cn

Object.groupBy(arr, x => x.type)
来源：http://nm.jctech888.com.cn

[U110] JS：数组分块
来源：http://fg.chemitech.net.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://iw.gzmigu.cn

[U111] JS：对象转 Map
来源：http://de.521024.cn

new Map(Object.entries(obj))
来源：http://rz.yuntaijiaju.cn

[U112] JS：字符串补位
来源：http://vi.hahajie.cn

"7".padStart(3, "0")
来源：http://zm.bjjhwx.cn

[U113] JS：正则替换全部
来源：http://ox.huanxung.cn

s.replaceAll("a", "b")
来源：http://ry.nszjky.cn

[U114] JS：JSON 深比较
来源：http://jl.yuexingan06.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ju.jianghongdianzi.cn


<!-- 参考信息 -->