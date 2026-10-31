代发 wailian999

[T29] Swift：guard 提前返回
来源：http://rz.huixiangedu.cn

guard let x = opt else { return }
来源：http://nj.jianghongdianzi.cn

[T30] Swift：协议
来源：http://pp.bookmarksfly.cn

protocol Shape { func area() -> Double }
来源：http://og.newstarts.cn

[T31] Lua：Hello World
来源：http://eo.newstarts.cn

print("Hello")
来源：http://ml.jctech888.com.cn

[T32] Lua：局部变量
来源：http://ig.yuexingan06.cn

local a = 1
来源：http://qe.bookmarksfly.cn

[T33] Lua：表（数组）
来源：http://gb.szxytkj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hi.hahajie.cn

[T34] Lua：遍历表
来源：http://wt.chemitech.net.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qc.szxytkj.cn

[T35] Lua：字典表
来源：http://ag.wgjwhj.cn

local d = { a = 1 };  d.b = 2
来源：http://yq.lnxyls.cn

[T36] Lua：函数
来源：http://ed.huixiangedu.cn

function add(a, b) return a + b end
来源：http://ly.shxzskj.cn

[T37] Lua：字符串拼接
来源：http://pz.jctech888.com.cn

"a" .. "b"
来源：http://gh.szxytkj.cn

[T38] Lua：条件
来源：http://ws.bookmarksfly.cn

if x > 0 then print("正") end
来源：http://hm.shxzskj.cn

[T39] Lua：模式匹配
来源：http://kv.chemitech.net.cn

string.find(s, "%d+")
来源：http://ij.shtwfgs.cn

[T40] Lua：元表
来源：http://ws.muxihuayi.cn

setmetatable({}, { __index = base })
来源：http://ya.chemitech.net.cn

[T41] Perl：Hello World
来源：http://cn.hnjuh.cn

print "Hello\n";
来源：http://ep.shtwfgs.cn

[T42] Perl：变量类型
来源：http://dk.colortex.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ss.jianghongdianzi.cn

[T43] Perl：字符串插值
来源：http://bi.newstarts.cn

"值: $a"
来源：http://ft.szxytkj.cn

[T44] Perl：条件
来源：http://bq.shxzukj.cn

if ($a > 0) { print "正"; }
来源：http://fn.huanxung.cn

[T45] Perl：数组遍历
来源：http://xl.jctech888.com.cn

for my $x (@arr) { print $x; }
来源：http://ul.newstarts.cn

[T46] Perl：哈希操作
来源：http://lh.panjiajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vs.hnjuh.cn

[T47] Perl：正则捕获
来源：http://la.haigaiapp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xv.huixiangedu.cn

[T48] Perl：正则替换
来源：http://nw.bookmarksfly.cn

$s =~ s/old/new/g;
来源：http://lv.huanxung.cn

[T49] Perl：函数
来源：http://ru.gzmigu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sf.jctech888.com.cn

[T50] Perl：逐行读文件
来源：http://iq.szxytkj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://uu.hahajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://ck.chemitech.net.cn

[T51] Scala：Hello World
来源：http://vk.chemitech.net.cn

println("Hello")
来源：http://lu.shtwfgs.cn

[T52] Scala：变量
来源：http://cl.huixinmuqiang.cn

val a = 1;  var b = 2
来源：http://yb.nszjky.cn

[T53] Scala：字符串插值
来源：http://bx.shtwfgs.cn

s"值: $b"
来源：http://rz.huanxung.cn

[T54] Scala：集合映射
来源：http://rv.bookmarksfly.cn

List(1, 2, 3).map(_ * 2)
来源：http://sl.newstarts.cn

[T55] Scala：集合过滤
来源：http://qy.jctech888.com.cn

List(1, 2, 3).filter(_ > 1)
来源：http://tc.asd995.cn

[T56] Scala：样例类
来源：http://tk.nszjky.cn

case class User(name: String, age: Int)
来源：http://bk.lnxyls.cn

[T57] Scala：模式匹配
来源：http://qr.huixinmuqiang.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fd.huixiangedu.cn

[T58] Scala：函数定义
来源：http://ou.shxzukj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://mk.huixinmuqiang.cn

[T59] Scala：循环
来源：http://ym.szxytkj.cn

for (i <- 1 to 10) println(i)
来源：http://bv.haigaiapp.cn

[T60] Scala：折叠
来源：http://jb.huixiangedu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cq.nszjky.cn

================================================================================
来源：http://pb.muxihuayi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kf.haigaiapp.cn

================================================================================
来源：http://ie.hnjuh.cn

[U01] Py：创建虚拟环境
来源：http://sk.lnxyls.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wy.panjiajie.cn

[U02] Py：导出 / 安装依赖
来源：http://bv.bjjhwx.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://oi.shxzukj.cn

[U03] Py：加载 .env 配置
来源：http://nb.9csxet.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://vb.shtwfgs.cn

[U04] Py：变量调试打印
来源：http://be.bookmarksfly.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ov.panjiajie.cn

[U05] Py：列表去重且保序
来源：http://zd.9csxet.cn

list(dict.fromkeys(arr))
来源：http://ni.jianghongdianzi.cn

[U06] Py：合并两个字典
来源：http://ht.shtwfgs.cn

{**a, **b}
来源：http://ct.newstarts.cn

[U07] Py：反转字典键值
来源：http://dg.yuntaijiaju.cn

{v: k for k, v in d.items()}
来源：http://co.huanxung.cn

[U08] Py：展平二维列表
来源：http://wd.shtwfgs.cn

[y for x in nested for y in x]
来源：http://vh.bjjhwx.cn

[U09] Py：字典取最大值的键
来源：http://gq.shxzskj.cn

max(d, key=d.get)
来源：http://bi.szxytkj.cn

[U10] Py：按值排序字典
来源：http://cn.nicolike.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wu.yuexingan06.cn

[U11] Py：生成器表达式
来源：http://cj.hahajie.cn

(x * 2 for x in arr)
来源：http://ll.hnjuh.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qb.wgjwhj.cn

Counter(arr).most_common(3)
来源：http://go.9csxet.cn

[U13] Py：固定长度队列
来源：http://xu.haigaiapp.cn

deque(maxlen=10)
来源：http://sa.huanxung.cn

[U14] Py：分组收集到列表
来源：http://qs.9csxet.cn

defaultdict(list)
来源：http://cn.wgjwhj.cn

[U15] Py：高精度计时
来源：http://eu.szsharing.cn

t = time.perf_counter()
来源：http://dm.chemitech.net.cn

[U16] Py：命令行参数解析
来源：http://to.bjjhwx.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tv.haigaiapp.cn

[U17] Py：初始化日志
来源：http://dh.9csxet.cn

logging.basicConfig(level=logging.INFO)
来源：http://jz.yuntaijiaju.cn

[U18] Py：预编译正则
来源：http://sk.9csxet.cn

pat = re.compile(r"\d+")
来源：http://xk.huanxung.cn

[U19] Py：正则替换带回调
来源：http://yg.hnjuh.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mx.chemitech.net.cn

[U20] Py：缓存函数结果
来源：http://mr.nicolike.cn

@functools.lru_cache(maxsize=None)
来源：http://rm.shtwfgs.cn

[U21] Py：自定义上下文管理器
来源：http://fh.huixiangedu.cn

@contextlib.contextmanager
来源：http://zo.hahajie.cn

[U22] Py：矩阵转置
来源：http://ve.asd995.cn

list(zip(*m))
来源：http://mw.jianghongdianzi.cn

[U23] Py：分块读取大文件
来源：http://xd.szxytkj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qp.asd995.cn

[U24] Py：路径操作
来源：http://kc.szxytkj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fc.colortex.cn

[U25] Py：CSV 按字典读
来源：http://nk.asd995.cn

csv.DictReader(f)
来源：http://gi.huixiangedu.cn

[U26] Py：并发下载
来源：http://da.bjjhwx.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nv.newstarts.cn

[U27] Py：异步 HTTP
来源：http://wf.huixiangedu.cn

aiohttp.ClientSession() 配合 async with
来源：http://kt.bjjhwx.cn

[U28] Py：类型别名
来源：http://ag.shtwfgs.cn

UserId = int
来源：http://ej.hnjuh.cn

[U29] Py：属性校验
来源：http://jz.huixiangedu.cn

@property 与 @x.setter 配合
来源：http://uv.huanxung.cn

[U30] Py：数据类
来源：http://lh.nicolike.cn

@dataclass(slots=True)
来源：http://ks.huixinmuqiang.cn

[U31] Py：单测
来源：http://ue.jianghongdianzi.cn

python -m pytest -q
来源：http://cg.hahajie.cn

[U32] Py：代码格式化
来源：http://mk.huixinmuqiang.cn

ruff format . && ruff check --fix .
来源：http://ow.bookmarksfly.cn

[U33] Py：打包发布
来源：http://hx.colortex.cn

python -m build  （依赖 pyproject.toml）
来源：http://wr.jctech888.com.cn

[U34] Py：判断编码
来源：http://xp.asd995.cn

chardet.detect(raw)
来源：http://gj.hahajie.cn

[U35] Py：发送邮件
来源：http://ah.muxihuayi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fd.newstarts.cn

[U36] Py：定时任务
来源：http://qk.colortex.cn

schedule.every(10).minutes.do(job)
来源：http://jf.muxihuayi.cn

[U37] Py：读写 Excel
来源：http://um.shxzukj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://yt.521024.cn

[U38] Py：获取脚本所在目录
来源：http://uy.shxzukj.cn

Path(__file__).resolve().parent
来源：http://zb.bjjhwx.cn

[U39] Py：判断是否在交互环境
来源：http://jj.nicolike.cn

sys.stdout.isatty()
来源：http://tn.gzmigu.cn

[U40] Py：打印到标准错误
来源：http://ed.huixinmuqiang.cn

print("err", file=sys.stderr)
来源：http://gm.shtwfgs.cn

[U41] PHP：初始化 Composer 项目
来源：http://vp.huixinmuqiang.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://mv.chemitech.net.cn

[U42] PHP：PSR-4 自动加载
来源：http://fu.hahajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fy.lnxyls.cn

[U43] PHP：声明命名空间
来源：http://gu.9csxet.cn

namespace App\Http;
来源：http://mc.bjjhwx.cn

[U44] PHP：开启严格类型
来源：http://yo.colortex.cn

declare(strict_types=1);
来源：http://ix.shxzukj.cn

[U45] PHP：类型声明与返回类型
来源：http://uw.haigaiapp.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ht.hnjuh.cn

[U46] PHP：可空类型
来源：http://tk.chemitech.net.cn

?string $name = null
来源：http://wr.huixiangedu.cn

[U47] PHP：联合类型
来源：http://ma.panjiajie.cn

int|string $id
来源：http://oj.shxzukj.cn

[U48] PHP：纯枚举
来源：http://gc.nszjky.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ea.nicolike.cn

[U49] PHP：只读属性
来源：http://ry.colortex.cn

public readonly string $name
来源：http://tu.asd995.cn

[U50] PHP：构造器属性提升
来源：http://vc.huixinmuqiang.cn

public function __construct(private int $id) {}
来源：http://dj.jianghongdianzi.cn

[U51] PHP：数组解构
来源：http://it.hahajie.cn

[$a, $b] = $arr;
来源：http://rz.chemitech.net.cn

[U52] PHP：箭头函数
来源：http://ml.nicolike.cn

$double = fn($x) => $x * 2;
来源：http://so.newstarts.cn

[U53] PHP：空合并运算符
来源：http://tw.yuexingan06.cn

$v = $a ?? $b ?? "default";
来源：http://ic.colortex.cn

[U54] PHP：空安全调用
来源：http://iy.shxzukj.cn

$obj?->method()
来源：http://jm.bookmarksfly.cn

[U55] PHP：match 表达式
来源：http://kt.gzmigu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tq.nszjky.cn

[U56] PHP：命名参数
来源：http://iq.bookmarksfly.cn

f(a: 1, b: 2)
来源：http://rc.chemitech.net.cn

[U57] PHP：字符串插值
来源：http://mj.521024.cn

"值: {$a}"
来源：http://uk.hahajie.cn

[U58] PHP：数组三件套
来源：http://pu.newstarts.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ra.chemitech.net.cn

[U59] PHP：自定义排序
来源：http://nn.gzmigu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nt.huixinmuqiang.cn

[U60] PHP：JSON 编解码
来源：http://fg.lnxyls.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vm.szxytkj.cn

[U61] PHP：正则
来源：http://fa.9csxet.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qh.panjiajie.cn

[U62] PHP：日期对象
来源：http://sj.huixinmuqiang.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bb.nicolike.cn

[U63] PHP：文件读写
来源：http://ws.huixiangedu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ca.jianghongdianzi.cn

[U64] PHP：目录遍历
来源：http://gl.huixiangedu.cn

glob("dir/*.php");  scandir("dir");
来源：http://wb.wgjwhj.cn

[U65] PHP：会话
来源：http://or.lnxyls.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://zd.gzmigu.cn

[U66] PHP：设置 Cookie
来源：http://hi.shxzukj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jo.shtwfgs.cn

[U67] PHP：处理文件上传
来源：http://yx.jctech888.com.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sy.chemitech.net.cn

[U68] PHP：PDO 连接
来源：http://js.9csxet.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ir.yuntaijiaju.cn

[U69] PHP：PDO 预处理
来源：http://jy.panjiajie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sf.asd995.cn

[U70] PHP：PDO 事务
来源：http://mj.bookmarksfly.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://is.yuntaijiaju.cn

[U71] PHP：抛出异常
来源：http://no.jianghongdianzi.cn

throw new RuntimeException("失败", 500);
来源：http://zm.shxzskj.cn

[U72] PHP：写错误日志
来源：http://qf.haigaiapp.cn

error_log("失败: " . $e->getMessage());
来源：http://va.yuexingan06.cn

[U73] PHP：读取 ini 配置
来源：http://mg.wgjwhj.cn

parse_ini_file("config.ini", true)
来源：http://jf.bjjhwx.cn

[U74] PHP：读取环境变量
来源：http://zv.chemitech.net.cn

getenv("APP_ENV") ?: "production"
来源：http://ab.521024.cn

[U75] PHP：依赖注入
来源：http://aj.jctech888.com.cn

composer require psr/container
来源：http://xq.hahajie.cn

[U76] PHP：简单路由
来源：http://wx.gzmigu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://av.huixiangedu.cn

[U77] PHP：模板渲染
来源：http://on.szxytkj.cn

composer require twig/twig
来源：http://bu.asd995.cn

[U78] PHP：单元测试
来源：http://aw.bookmarksfly.cn

composer require --dev phpunit/phpunit
来源：http://ze.haigaiapp.cn

[U79] PHP：静态分析
来源：http://zc.panjiajie.cn

composer require --dev phpstan/phpstan
来源：http://za.yuntaijiaju.cn

[U80] PHP：代码规范修复
来源：http://xl.yuexingan06.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ah.muxihuayi.cn

[U81] JS：初始化项目
来源：http://xn.9csxet.cn

npm init -y;  npm i express
来源：http://wt.yuexingan06.cn

[U82] JS：package.json 脚本
来源：http://uu.nicolike.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bh.wgjwhj.cn

[U83] JS：ES Module 导入导出
来源：http://is.wgjwhj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xh.bookmarksfly.cn

[U84] JS：CommonJS 写法
来源：http://nh.9csxet.cn

module.exports = { a };  const { a } = require("./m");
来源：http://jh.asd995.cn

[U85] JS：可选链
来源：http://qv.jianghongdianzi.cn

a?.b?.c
来源：http://us.szxytkj.cn

[U86] JS：空值合并
来源：http://fo.haigaiapp.cn

a ?? b
来源：http://dj.lnxyls.cn

[U87] JS：解构默认值
来源：http://cd.haigaiapp.cn

const { a = 1, b = 2 } = obj;
来源：http://yc.colortex.cn

[U88] JS：对象展开合并
来源：http://mm.szsharing.cn

{ ...a, ...b }
来源：http://ou.nicolike.cn

[U89] JS：数组去重
来源：http://ot.shxzskj.cn

[...new Set(arr)]
来源：http://gu.haigaiapp.cn

[U90] JS：数字数组排序
来源：http://yq.jianghongdianzi.cn

[...arr].sort((a, b) => a - b)
来源：http://px.wgjwhj.cn

[U91] JS：对象键值遍历
来源：http://hj.haigaiapp.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rs.jianghongdianzi.cn

[U92] JS：深拷贝
来源：http://li.9csxet.cn

structuredClone(obj)
来源：http://jc.bookmarksfly.cn

[U93] JS：模板字符串
来源：http://uc.hahajie.cn

`共 ${n} 条`
来源：http://fi.asd995.cn

[U94] JS：箭头函数
来源：http://js.hahajie.cn

const double = x => x * 2;
来源：http://lc.jctech888.com.cn

[U95] JS：Promise 包装
来源：http://vk.hnjuh.cn

new Promise((resolve, reject) => {})
来源：http://hw.521024.cn

[U96] JS：async/await 与异常
来源：http://lj.huixiangedu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rg.jctech888.com.cn

[U97] JS：并发请求
来源：http://al.gzmigu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://um.asd995.cn

[U98] JS：fetch 带 JSON
来源：http://af.hnjuh.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yq.hnjuh.cn

[U99] JS：事件监听
来源：http://uz.asd995.cn

el.addEventListener("click", e => {})
来源：http://hj.yuntaijiaju.cn

[U100] JS：DOM 查询
来源：http://en.asd995.cn

document.querySelector(".item")
来源：http://ia.muxihuayi.cn

[U101] JS：classList 操作
来源：http://ae.bjjhwx.cn

el.classList.toggle("active")
来源：http://if.szsharing.cn

[U102] JS：本地存储
来源：http://on.shxzukj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://mh.521024.cn

[U103] JS：定时器
来源：http://sh.yuntaijiaju.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ln.hahajie.cn

[U104] JS：防抖
来源：http://wv.gzmigu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://au.newstarts.cn

[U105] JS：节流
来源：http://el.bjjhwx.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lk.9csxet.cn

[U106] JS：日期格式化
来源：http://io.9csxet.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pz.521024.cn

[U107] JS：数字千分位
来源：http://ei.haigaiapp.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rk.chemitech.net.cn

[U108] JS：随机整数
来源：http://yo.bjjhwx.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pd.chemitech.net.cn

[U109] JS：数组分组
来源：http://ht.huanxung.cn

Object.groupBy(arr, x => x.type)
来源：http://sw.huixinmuqiang.cn

[U110] JS：数组分块
来源：http://yl.asd995.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tp.colortex.cn

[U111] JS：对象转 Map
来源：http://vi.9csxet.cn

new Map(Object.entries(obj))
来源：http://nq.szsharing.cn

[U112] JS：字符串补位
来源：http://ur.jctech888.com.cn

"7".padStart(3, "0")
来源：http://mc.colortex.cn

[U113] JS：正则替换全部
来源：http://ww.shtwfgs.cn

s.replaceAll("a", "b")
来源：http://mm.bookmarksfly.cn

[U114] JS：JSON 深比较
来源：http://mc.colortex.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://jv.bjjhwx.cn

[U115] JS：生成 UUID
来源：http://uq.huanxung.cn

crypto.randomUUID()
来源：http://uq.bookmarksfly.cn

[U116] JS：类型检查（JSDoc）
来源：http://zi.yuexingan06.cn

/** @param {string} name */ function f(name) {}
来源：http://lv.asd995.cn


<!-- 参考信息 -->