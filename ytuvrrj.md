代发 wailian999

[T31] Lua：Hello World
来源：http://jc.yuntaijiaju.cn

print("Hello")
来源：http://jk.huixiangedu.cn

[T32] Lua：局部变量
来源：http://xs.nszjky.cn

local a = 1
来源：http://dj.521024.cn

[T33] Lua：表（数组）
来源：http://vf.bookmarksfly.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://it.bjjhwx.cn

[T34] Lua：遍历表
来源：http://sx.wgjwhj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ia.muxihuayi.cn

[T35] Lua：字典表
来源：http://ln.bookmarksfly.cn

local d = { a = 1 };  d.b = 2
来源：http://cp.shxzskj.cn

[T36] Lua：函数
来源：http://oa.gzmigu.cn

function add(a, b) return a + b end
来源：http://ay.newstarts.cn

[T37] Lua：字符串拼接
来源：http://sx.bjjhwx.cn

"a" .. "b"
来源：http://qm.nicolike.cn

[T38] Lua：条件
来源：http://zt.muxihuayi.cn

if x > 0 then print("正") end
来源：http://cj.lnxyls.cn

[T39] Lua：模式匹配
来源：http://mf.wgjwhj.cn

string.find(s, "%d+")
来源：http://ag.shxzskj.cn

[T40] Lua：元表
来源：http://sq.hahajie.cn

setmetatable({}, { __index = base })
来源：http://ep.521024.cn

[T41] Perl：Hello World
来源：http://qn.shxzukj.cn

print "Hello\n";
来源：http://bw.521024.cn

[T42] Perl：变量类型
来源：http://ij.shxzukj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lq.gzmigu.cn

[T43] Perl：字符串插值
来源：http://xz.hnjuh.cn

"值: $a"
来源：http://vc.hahajie.cn

[T44] Perl：条件
来源：http://ht.shxzskj.cn

if ($a > 0) { print "正"; }
来源：http://ow.nicolike.cn

[T45] Perl：数组遍历
来源：http://up.lnxyls.cn

for my $x (@arr) { print $x; }
来源：http://ab.9csxet.cn

[T46] Perl：哈希操作
来源：http://fq.chemitech.net.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://aw.nicolike.cn

[T47] Perl：正则捕获
来源：http://uu.szsharing.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qp.huixiangedu.cn

[T48] Perl：正则替换
来源：http://qo.hahajie.cn

$s =~ s/old/new/g;
来源：http://nd.hahajie.cn

[T49] Perl：函数
来源：http://po.szxytkj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mg.shxzukj.cn

[T50] Perl：逐行读文件
来源：http://jy.haigaiapp.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://jv.szxytkj.cn

while (my $line = <$fh>) { print $line; }
来源：http://ku.nicolike.cn

[T51] Scala：Hello World
来源：http://sz.muxihuayi.cn

println("Hello")
来源：http://lt.lnxyls.cn

[T52] Scala：变量
来源：http://bt.hnjuh.cn

val a = 1;  var b = 2
来源：http://sb.wgjwhj.cn

[T53] Scala：字符串插值
来源：http://fl.szsharing.cn

s"值: $b"
来源：http://le.hnjuh.cn

[T54] Scala：集合映射
来源：http://jq.chemitech.net.cn

List(1, 2, 3).map(_ * 2)
来源：http://fr.huixinmuqiang.cn

[T55] Scala：集合过滤
来源：http://mz.panjiajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://dr.hahajie.cn

[T56] Scala：样例类
来源：http://xs.jianghongdianzi.cn

case class User(name: String, age: Int)
来源：http://ry.jianghongdianzi.cn

[T57] Scala：模式匹配
来源：http://kz.huixinmuqiang.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://dq.panjiajie.cn

[T58] Scala：函数定义
来源：http://rq.jctech888.com.cn

def add(a: Int, b: Int): Int = a + b
来源：http://je.newstarts.cn

[T59] Scala：循环
来源：http://pa.muxihuayi.cn

for (i <- 1 to 10) println(i)
来源：http://fp.huixinmuqiang.cn

[T60] Scala：折叠
来源：http://ox.huanxung.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lq.chemitech.net.cn

================================================================================
来源：http://ag.colortex.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qu.szsharing.cn

================================================================================
来源：http://qc.newstarts.cn

[U01] Py：创建虚拟环境
来源：http://wc.521024.cn

python -m venv .venv && source .venv/bin/activate
来源：http://rb.asd995.cn

[U02] Py：导出 / 安装依赖
来源：http://ed.haigaiapp.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gx.chemitech.net.cn

[U03] Py：加载 .env 配置
来源：http://ow.shtwfgs.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qx.nicolike.cn

[U04] Py：变量调试打印
来源：http://wn.yuexingan06.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://yh.szxytkj.cn

[U05] Py：列表去重且保序
来源：http://tz.jianghongdianzi.cn

list(dict.fromkeys(arr))
来源：http://ko.newstarts.cn

[U06] Py：合并两个字典
来源：http://zf.jctech888.com.cn

{**a, **b}
来源：http://xq.muxihuayi.cn

[U07] Py：反转字典键值
来源：http://wg.lnxyls.cn

{v: k for k, v in d.items()}
来源：http://so.chemitech.net.cn

[U08] Py：展平二维列表
来源：http://pv.hahajie.cn

[y for x in nested for y in x]
来源：http://fa.szsharing.cn

[U09] Py：字典取最大值的键
来源：http://gv.gzmigu.cn

max(d, key=d.get)
来源：http://ep.521024.cn

[U10] Py：按值排序字典
来源：http://om.nicolike.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lg.lnxyls.cn

[U11] Py：生成器表达式
来源：http://qm.panjiajie.cn

(x * 2 for x in arr)
来源：http://nv.szxytkj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rr.nszjky.cn

Counter(arr).most_common(3)
来源：http://re.szsharing.cn

[U13] Py：固定长度队列
来源：http://dv.shtwfgs.cn

deque(maxlen=10)
来源：http://jq.huixiangedu.cn

[U14] Py：分组收集到列表
来源：http://df.shtwfgs.cn

defaultdict(list)
来源：http://xf.hahajie.cn

[U15] Py：高精度计时
来源：http://wc.muxihuayi.cn

t = time.perf_counter()
来源：http://ub.hnjuh.cn

[U16] Py：命令行参数解析
来源：http://ch.asd995.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ax.yuntaijiaju.cn

[U17] Py：初始化日志
来源：http://hh.szxytkj.cn

logging.basicConfig(level=logging.INFO)
来源：http://cv.hnjuh.cn

[U18] Py：预编译正则
来源：http://gt.haigaiapp.cn

pat = re.compile(r"\d+")
来源：http://dk.yuexingan06.cn

[U19] Py：正则替换带回调
来源：http://bm.huixiangedu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rz.colortex.cn

[U20] Py：缓存函数结果
来源：http://xs.yuexingan06.cn

@functools.lru_cache(maxsize=None)
来源：http://ih.bookmarksfly.cn

[U21] Py：自定义上下文管理器
来源：http://nv.wgjwhj.cn

@contextlib.contextmanager
来源：http://ei.nszjky.cn

[U22] Py：矩阵转置
来源：http://ts.panjiajie.cn

list(zip(*m))
来源：http://rh.chemitech.net.cn

[U23] Py：分块读取大文件
来源：http://cf.yuntaijiaju.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tj.haigaiapp.cn

[U24] Py：路径操作
来源：http://ho.shxzukj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pl.nszjky.cn

[U25] Py：CSV 按字典读
来源：http://yk.szsharing.cn

csv.DictReader(f)
来源：http://zu.yuntaijiaju.cn

[U26] Py：并发下载
来源：http://di.huixiangedu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xq.panjiajie.cn

[U27] Py：异步 HTTP
来源：http://lx.huixinmuqiang.cn

aiohttp.ClientSession() 配合 async with
来源：http://cb.szxytkj.cn

[U28] Py：类型别名
来源：http://ru.yuntaijiaju.cn

UserId = int
来源：http://vj.huixiangedu.cn

[U29] Py：属性校验
来源：http://ad.colortex.cn

@property 与 @x.setter 配合
来源：http://dj.521024.cn

[U30] Py：数据类
来源：http://ey.bookmarksfly.cn

@dataclass(slots=True)
来源：http://wd.huixiangedu.cn

[U31] Py：单测
来源：http://uq.9csxet.cn

python -m pytest -q
来源：http://iq.asd995.cn

[U32] Py：代码格式化
来源：http://oe.newstarts.cn

ruff format . && ruff check --fix .
来源：http://vs.lnxyls.cn

[U33] Py：打包发布
来源：http://yp.shxzskj.cn

python -m build  （依赖 pyproject.toml）
来源：http://uw.huixinmuqiang.cn

[U34] Py：判断编码
来源：http://bt.jctech888.com.cn

chardet.detect(raw)
来源：http://oy.yuntaijiaju.cn

[U35] Py：发送邮件
来源：http://lh.muxihuayi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wr.szxytkj.cn

[U36] Py：定时任务
来源：http://kz.nicolike.cn

schedule.every(10).minutes.do(job)
来源：http://dy.shxzskj.cn

[U37] Py：读写 Excel
来源：http://uy.huixiangedu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wj.bjjhwx.cn

[U38] Py：获取脚本所在目录
来源：http://fy.asd995.cn

Path(__file__).resolve().parent
来源：http://gp.521024.cn

[U39] Py：判断是否在交互环境
来源：http://nq.colortex.cn

sys.stdout.isatty()
来源：http://by.newstarts.cn

[U40] Py：打印到标准错误
来源：http://jx.shxzskj.cn

print("err", file=sys.stderr)
来源：http://tm.wgjwhj.cn

[U41] PHP：初始化 Composer 项目
来源：http://sq.lnxyls.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://dk.newstarts.cn

[U42] PHP：PSR-4 自动加载
来源：http://pr.huixiangedu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fq.szsharing.cn

[U43] PHP：声明命名空间
来源：http://fy.bjjhwx.cn

namespace App\Http;
来源：http://pu.lnxyls.cn

[U44] PHP：开启严格类型
来源：http://yo.shxzskj.cn

declare(strict_types=1);
来源：http://ce.wgjwhj.cn

[U45] PHP：类型声明与返回类型
来源：http://nt.wgjwhj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ju.9csxet.cn

[U46] PHP：可空类型
来源：http://pp.gzmigu.cn

?string $name = null
来源：http://kc.szsharing.cn

[U47] PHP：联合类型
来源：http://fo.bjjhwx.cn

int|string $id
来源：http://ki.panjiajie.cn

[U48] PHP：纯枚举
来源：http://jc.muxihuayi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://au.hnjuh.cn

[U49] PHP：只读属性
来源：http://zb.panjiajie.cn

public readonly string $name
来源：http://uy.huanxung.cn

[U50] PHP：构造器属性提升
来源：http://mb.yuntaijiaju.cn

public function __construct(private int $id) {}
来源：http://lm.muxihuayi.cn

[U51] PHP：数组解构
来源：http://ve.colortex.cn

[$a, $b] = $arr;
来源：http://pp.colortex.cn

[U52] PHP：箭头函数
来源：http://jp.colortex.cn

$double = fn($x) => $x * 2;
来源：http://pb.colortex.cn

[U53] PHP：空合并运算符
来源：http://sw.asd995.cn

$v = $a ?? $b ?? "default";
来源：http://ux.huanxung.cn

[U54] PHP：空安全调用
来源：http://au.szsharing.cn

$obj?->method()
来源：http://jf.panjiajie.cn

[U55] PHP：match 表达式
来源：http://cd.huixiangedu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zd.yuntaijiaju.cn

[U56] PHP：命名参数
来源：http://av.huanxung.cn

f(a: 1, b: 2)
来源：http://cs.yuntaijiaju.cn

[U57] PHP：字符串插值
来源：http://xi.huixinmuqiang.cn

"值: {$a}"
来源：http://ew.wgjwhj.cn

[U58] PHP：数组三件套
来源：http://pn.huixinmuqiang.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bd.colortex.cn

[U59] PHP：自定义排序
来源：http://ct.szxytkj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gz.jianghongdianzi.cn

[U60] PHP：JSON 编解码
来源：http://iw.bookmarksfly.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ff.huixinmuqiang.cn

[U61] PHP：正则
来源：http://sg.jianghongdianzi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fc.shtwfgs.cn

[U62] PHP：日期对象
来源：http://ea.huixinmuqiang.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hi.9csxet.cn

[U63] PHP：文件读写
来源：http://ce.521024.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jm.bjjhwx.cn

[U64] PHP：目录遍历
来源：http://xm.haigaiapp.cn

glob("dir/*.php");  scandir("dir");
来源：http://ls.yuexingan06.cn

[U65] PHP：会话
来源：http://bn.newstarts.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://iu.9csxet.cn

[U66] PHP：设置 Cookie
来源：http://hm.colortex.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ji.nszjky.cn

[U67] PHP：处理文件上传
来源：http://td.newstarts.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://os.huanxung.cn

[U68] PHP：PDO 连接
来源：http://qq.jctech888.com.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://et.hnjuh.cn

[U69] PHP：PDO 预处理
来源：http://km.lnxyls.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ij.huixiangedu.cn

[U70] PHP：PDO 事务
来源：http://pp.chemitech.net.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vp.gzmigu.cn

[U71] PHP：抛出异常
来源：http://yb.szxytkj.cn

throw new RuntimeException("失败", 500);
来源：http://fw.wgjwhj.cn

[U72] PHP：写错误日志
来源：http://db.hnjuh.cn

error_log("失败: " . $e->getMessage());
来源：http://il.shtwfgs.cn

[U73] PHP：读取 ini 配置
来源：http://jp.shxzskj.cn

parse_ini_file("config.ini", true)
来源：http://co.hahajie.cn

[U74] PHP：读取环境变量
来源：http://fj.haigaiapp.cn

getenv("APP_ENV") ?: "production"
来源：http://aw.hahajie.cn

[U75] PHP：依赖注入
来源：http://cp.bookmarksfly.cn

composer require psr/container
来源：http://py.newstarts.cn

[U76] PHP：简单路由
来源：http://qg.shxzukj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xt.shxzukj.cn

[U77] PHP：模板渲染
来源：http://hd.hahajie.cn

composer require twig/twig
来源：http://ad.nszjky.cn

[U78] PHP：单元测试
来源：http://gw.yuntaijiaju.cn

composer require --dev phpunit/phpunit
来源：http://pa.chemitech.net.cn

[U79] PHP：静态分析
来源：http://gr.jianghongdianzi.cn

composer require --dev phpstan/phpstan
来源：http://cj.lnxyls.cn

[U80] PHP：代码规范修复
来源：http://ng.gzmigu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ah.newstarts.cn

[U81] JS：初始化项目
来源：http://wa.shxzskj.cn

npm init -y;  npm i express
来源：http://nl.szsharing.cn

[U82] JS：package.json 脚本
来源：http://dr.szxytkj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://uy.hahajie.cn

[U83] JS：ES Module 导入导出
来源：http://aj.hnjuh.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ow.gzmigu.cn

[U84] JS：CommonJS 写法
来源：http://ro.lnxyls.cn

module.exports = { a };  const { a } = require("./m");
来源：http://zy.9csxet.cn

[U85] JS：可选链
来源：http://ab.szsharing.cn

a?.b?.c
来源：http://pz.bjjhwx.cn

[U86] JS：空值合并
来源：http://oj.panjiajie.cn

a ?? b
来源：http://rn.nszjky.cn

[U87] JS：解构默认值
来源：http://in.huixinmuqiang.cn

const { a = 1, b = 2 } = obj;
来源：http://dk.szxytkj.cn

[U88] JS：对象展开合并
来源：http://ho.hahajie.cn

{ ...a, ...b }
来源：http://gn.shtwfgs.cn

[U89] JS：数组去重
来源：http://no.szxytkj.cn

[...new Set(arr)]
来源：http://yt.huanxung.cn

[U90] JS：数字数组排序
来源：http://bg.szxytkj.cn

[...arr].sort((a, b) => a - b)
来源：http://jq.colortex.cn

[U91] JS：对象键值遍历
来源：http://zz.huixiangedu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jz.yuexingan06.cn

[U92] JS：深拷贝
来源：http://iu.jianghongdianzi.cn

structuredClone(obj)
来源：http://bx.asd995.cn

[U93] JS：模板字符串
来源：http://pt.bookmarksfly.cn

`共 ${n} 条`
来源：http://wj.haigaiapp.cn

[U94] JS：箭头函数
来源：http://rk.lnxyls.cn

const double = x => x * 2;
来源：http://xa.521024.cn

[U95] JS：Promise 包装
来源：http://ou.yuntaijiaju.cn

new Promise((resolve, reject) => {})
来源：http://rc.jianghongdianzi.cn

[U96] JS：async/await 与异常
来源：http://gx.colortex.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wn.jctech888.com.cn

[U97] JS：并发请求
来源：http://js.521024.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://xu.jctech888.com.cn

[U98] JS：fetch 带 JSON
来源：http://yx.hnjuh.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://so.yuntaijiaju.cn

[U99] JS：事件监听
来源：http://nd.nicolike.cn

el.addEventListener("click", e => {})
来源：http://mh.yuntaijiaju.cn

[U100] JS：DOM 查询
来源：http://rg.wgjwhj.cn

document.querySelector(".item")
来源：http://iv.nicolike.cn

[U101] JS：classList 操作
来源：http://wz.shxzukj.cn

el.classList.toggle("active")
来源：http://yq.haigaiapp.cn

[U102] JS：本地存储
来源：http://ox.shtwfgs.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://zy.wgjwhj.cn

[U103] JS：定时器
来源：http://ph.bjjhwx.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ay.haigaiapp.cn

[U104] JS：防抖
来源：http://fp.colortex.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gi.shtwfgs.cn

[U105] JS：节流
来源：http://jg.shxzukj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://df.newstarts.cn

[U106] JS：日期格式化
来源：http://kt.gzmigu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tj.jctech888.com.cn

[U107] JS：数字千分位
来源：http://hi.wgjwhj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yo.szxytkj.cn

[U108] JS：随机整数
来源：http://wo.nszjky.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xr.shtwfgs.cn

[U109] JS：数组分组
来源：http://bd.gzmigu.cn

Object.groupBy(arr, x => x.type)
来源：http://tk.nicolike.cn

[U110] JS：数组分块
来源：http://iw.szsharing.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://sb.huixinmuqiang.cn

[U111] JS：对象转 Map
来源：http://mv.shtwfgs.cn

new Map(Object.entries(obj))
来源：http://rj.huixinmuqiang.cn

[U112] JS：字符串补位
来源：http://ph.szsharing.cn

"7".padStart(3, "0")
来源：http://du.nicolike.cn

[U113] JS：正则替换全部
来源：http://mc.lnxyls.cn

s.replaceAll("a", "b")
来源：http://ds.hnjuh.cn

[U114] JS：JSON 深比较
来源：http://uv.yuntaijiaju.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://cl.shxzukj.cn

[U115] JS：生成 UUID
来源：http://zh.lnxyls.cn

crypto.randomUUID()
来源：http://ro.huixiangedu.cn

[U116] JS：类型检查（JSDoc）
来源：http://qs.wgjwhj.cn

/** @param {string} name */ function f(name) {}
来源：http://al.shtwfgs.cn

[U117] JS：单元测试
来源：http://mf.haigaiapp.cn

npm i -D vitest;  npx vitest
来源：http://ek.bookmarksfly.cn

[U118] JS：开发服务器
来源：http://xr.lnxyls.cn

npm i -D vite;  npx vite
来源：http://sj.bjjhwx.cn


<!-- 参考信息 -->