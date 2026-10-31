代发 wailian999

[T29] Swift：guard 提前返回
来源：http://hk.asd995.cn

guard let x = opt else { return }
来源：http://nc.hahajie.cn

[T30] Swift：协议
来源：http://mk.521024.cn

protocol Shape { func area() -> Double }
来源：http://xc.newstarts.cn

[T31] Lua：Hello World
来源：http://ve.521024.cn

print("Hello")
来源：http://iy.9csxet.cn

[T32] Lua：局部变量
来源：http://xd.hnjuh.cn

local a = 1
来源：http://kf.huanxung.cn

[T33] Lua：表（数组）
来源：http://xv.hnjuh.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wu.9csxet.cn

[T34] Lua：遍历表
来源：http://nx.gzmigu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://io.shxzukj.cn

[T35] Lua：字典表
来源：http://wh.bjjhwx.cn

local d = { a = 1 };  d.b = 2
来源：http://yy.wgjwhj.cn

[T36] Lua：函数
来源：http://jm.chemitech.net.cn

function add(a, b) return a + b end
来源：http://jq.nicolike.cn

[T37] Lua：字符串拼接
来源：http://we.jianghongdianzi.cn

"a" .. "b"
来源：http://nl.huanxung.cn

[T38] Lua：条件
来源：http://ru.yuexingan06.cn

if x > 0 then print("正") end
来源：http://rf.bjjhwx.cn

[T39] Lua：模式匹配
来源：http://uf.haigaiapp.cn

string.find(s, "%d+")
来源：http://mt.9csxet.cn

[T40] Lua：元表
来源：http://up.bjjhwx.cn

setmetatable({}, { __index = base })
来源：http://dm.hahajie.cn

[T41] Perl：Hello World
来源：http://lw.muxihuayi.cn

print "Hello\n";
来源：http://vj.muxihuayi.cn

[T42] Perl：变量类型
来源：http://rr.nicolike.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ma.gzmigu.cn

[T43] Perl：字符串插值
来源：http://lt.lnxyls.cn

"值: $a"
来源：http://av.panjiajie.cn

[T44] Perl：条件
来源：http://na.jianghongdianzi.cn

if ($a > 0) { print "正"; }
来源：http://ur.shxzskj.cn

[T45] Perl：数组遍历
来源：http://lt.bookmarksfly.cn

for my $x (@arr) { print $x; }
来源：http://me.lnxyls.cn

[T46] Perl：哈希操作
来源：http://tk.newstarts.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qx.newstarts.cn

[T47] Perl：正则捕获
来源：http://as.shxzukj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://un.asd995.cn

[T48] Perl：正则替换
来源：http://hf.huixinmuqiang.cn

$s =~ s/old/new/g;
来源：http://sn.521024.cn

[T49] Perl：函数
来源：http://eg.gzmigu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jh.asd995.cn

[T50] Perl：逐行读文件
来源：http://ng.szsharing.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://vj.yuntaijiaju.cn

while (my $line = <$fh>) { print $line; }
来源：http://qo.lnxyls.cn

[T51] Scala：Hello World
来源：http://sx.jianghongdianzi.cn

println("Hello")
来源：http://sl.gzmigu.cn

[T52] Scala：变量
来源：http://zg.asd995.cn

val a = 1;  var b = 2
来源：http://qv.shtwfgs.cn

[T53] Scala：字符串插值
来源：http://fi.panjiajie.cn

s"值: $b"
来源：http://wk.521024.cn

[T54] Scala：集合映射
来源：http://gm.hnjuh.cn

List(1, 2, 3).map(_ * 2)
来源：http://pz.szsharing.cn

[T55] Scala：集合过滤
来源：http://bu.shxzskj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ok.shxzukj.cn

[T56] Scala：样例类
来源：http://ze.shtwfgs.cn

case class User(name: String, age: Int)
来源：http://sw.yuexingan06.cn

[T57] Scala：模式匹配
来源：http://oa.szxytkj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ub.gzmigu.cn

[T58] Scala：函数定义
来源：http://ra.panjiajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://uk.nszjky.cn

[T59] Scala：循环
来源：http://gc.huixinmuqiang.cn

for (i <- 1 to 10) println(i)
来源：http://gy.huixinmuqiang.cn

[T60] Scala：折叠
来源：http://uu.gzmigu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nh.newstarts.cn

================================================================================
来源：http://ra.asd995.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ge.shtwfgs.cn

================================================================================
来源：http://og.nicolike.cn

[U01] Py：创建虚拟环境
来源：http://lx.panjiajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wp.hnjuh.cn

[U02] Py：导出 / 安装依赖
来源：http://nv.lnxyls.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ai.hahajie.cn

[U03] Py：加载 .env 配置
来源：http://xh.huixinmuqiang.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ld.newstarts.cn

[U04] Py：变量调试打印
来源：http://bs.szxytkj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://br.muxihuayi.cn

[U05] Py：列表去重且保序
来源：http://xt.chemitech.net.cn

list(dict.fromkeys(arr))
来源：http://sh.shtwfgs.cn

[U06] Py：合并两个字典
来源：http://ey.521024.cn

{**a, **b}
来源：http://co.muxihuayi.cn

[U07] Py：反转字典键值
来源：http://mn.shtwfgs.cn

{v: k for k, v in d.items()}
来源：http://pw.haigaiapp.cn

[U08] Py：展平二维列表
来源：http://km.newstarts.cn

[y for x in nested for y in x]
来源：http://du.shtwfgs.cn

[U09] Py：字典取最大值的键
来源：http://xl.bookmarksfly.cn

max(d, key=d.get)
来源：http://bw.bookmarksfly.cn

[U10] Py：按值排序字典
来源：http://it.panjiajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ep.yuexingan06.cn

[U11] Py：生成器表达式
来源：http://lo.bookmarksfly.cn

(x * 2 for x in arr)
来源：http://oy.shxzskj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://no.huixiangedu.cn

Counter(arr).most_common(3)
来源：http://rj.9csxet.cn

[U13] Py：固定长度队列
来源：http://lf.asd995.cn

deque(maxlen=10)
来源：http://oe.jctech888.com.cn

[U14] Py：分组收集到列表
来源：http://rj.lnxyls.cn

defaultdict(list)
来源：http://uf.yuntaijiaju.cn

[U15] Py：高精度计时
来源：http://zg.shxzukj.cn

t = time.perf_counter()
来源：http://ag.shxzukj.cn

[U16] Py：命令行参数解析
来源：http://bw.szxytkj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yw.chemitech.net.cn

[U17] Py：初始化日志
来源：http://fh.yuexingan06.cn

logging.basicConfig(level=logging.INFO)
来源：http://hs.huanxung.cn

[U18] Py：预编译正则
来源：http://mb.newstarts.cn

pat = re.compile(r"\d+")
来源：http://kh.521024.cn

[U19] Py：正则替换带回调
来源：http://kf.gzmigu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://na.hahajie.cn

[U20] Py：缓存函数结果
来源：http://il.jctech888.com.cn

@functools.lru_cache(maxsize=None)
来源：http://st.huixinmuqiang.cn

[U21] Py：自定义上下文管理器
来源：http://yz.shxzukj.cn

@contextlib.contextmanager
来源：http://lh.bjjhwx.cn

[U22] Py：矩阵转置
来源：http://sr.haigaiapp.cn

list(zip(*m))
来源：http://dx.9csxet.cn

[U23] Py：分块读取大文件
来源：http://oj.nszjky.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sp.shxzskj.cn

[U24] Py：路径操作
来源：http://wu.jctech888.com.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qs.jctech888.com.cn

[U25] Py：CSV 按字典读
来源：http://cz.panjiajie.cn

csv.DictReader(f)
来源：http://zi.gzmigu.cn

[U26] Py：并发下载
来源：http://zo.huixinmuqiang.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wk.shtwfgs.cn

[U27] Py：异步 HTTP
来源：http://ni.nicolike.cn

aiohttp.ClientSession() 配合 async with
来源：http://dj.jianghongdianzi.cn

[U28] Py：类型别名
来源：http://vp.bjjhwx.cn

UserId = int
来源：http://aj.nszjky.cn

[U29] Py：属性校验
来源：http://li.huixinmuqiang.cn

@property 与 @x.setter 配合
来源：http://oi.szsharing.cn

[U30] Py：数据类
来源：http://ft.szxytkj.cn

@dataclass(slots=True)
来源：http://kb.wgjwhj.cn

[U31] Py：单测
来源：http://vg.chemitech.net.cn

python -m pytest -q
来源：http://fw.panjiajie.cn

[U32] Py：代码格式化
来源：http://rz.shtwfgs.cn

ruff format . && ruff check --fix .
来源：http://fb.yuntaijiaju.cn

[U33] Py：打包发布
来源：http://vh.shtwfgs.cn

python -m build  （依赖 pyproject.toml）
来源：http://gh.colortex.cn

[U34] Py：判断编码
来源：http://vp.newstarts.cn

chardet.detect(raw)
来源：http://dj.szsharing.cn

[U35] Py：发送邮件
来源：http://cn.521024.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://us.yuntaijiaju.cn

[U36] Py：定时任务
来源：http://uh.shxzukj.cn

schedule.every(10).minutes.do(job)
来源：http://ix.jctech888.com.cn

[U37] Py：读写 Excel
来源：http://qx.gzmigu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ut.shxzskj.cn

[U38] Py：获取脚本所在目录
来源：http://rf.shxzukj.cn

Path(__file__).resolve().parent
来源：http://wm.muxihuayi.cn

[U39] Py：判断是否在交互环境
来源：http://tc.panjiajie.cn

sys.stdout.isatty()
来源：http://of.huanxung.cn

[U40] Py：打印到标准错误
来源：http://nt.wgjwhj.cn

print("err", file=sys.stderr)
来源：http://xx.haigaiapp.cn

[U41] PHP：初始化 Composer 项目
来源：http://bs.shxzskj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://rc.hahajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://qb.yuexingan06.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ex.hahajie.cn

[U43] PHP：声明命名空间
来源：http://gz.shtwfgs.cn

namespace App\Http;
来源：http://mz.jianghongdianzi.cn

[U44] PHP：开启严格类型
来源：http://sl.bookmarksfly.cn

declare(strict_types=1);
来源：http://vv.jianghongdianzi.cn

[U45] PHP：类型声明与返回类型
来源：http://wb.szxytkj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://sz.wgjwhj.cn

[U46] PHP：可空类型
来源：http://tr.hnjuh.cn

?string $name = null
来源：http://md.chemitech.net.cn

[U47] PHP：联合类型
来源：http://pj.muxihuayi.cn

int|string $id
来源：http://un.chemitech.net.cn

[U48] PHP：纯枚举
来源：http://fr.chemitech.net.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xt.haigaiapp.cn

[U49] PHP：只读属性
来源：http://uo.haigaiapp.cn

public readonly string $name
来源：http://if.9csxet.cn

[U50] PHP：构造器属性提升
来源：http://fh.haigaiapp.cn

public function __construct(private int $id) {}
来源：http://di.hnjuh.cn

[U51] PHP：数组解构
来源：http://ko.huixinmuqiang.cn

[$a, $b] = $arr;
来源：http://fd.haigaiapp.cn

[U52] PHP：箭头函数
来源：http://ke.szsharing.cn

$double = fn($x) => $x * 2;
来源：http://no.nszjky.cn

[U53] PHP：空合并运算符
来源：http://wv.huixiangedu.cn

$v = $a ?? $b ?? "default";
来源：http://yk.shxzukj.cn

[U54] PHP：空安全调用
来源：http://dn.shxzskj.cn

$obj?->method()
来源：http://ws.newstarts.cn

[U55] PHP：match 表达式
来源：http://ll.nicolike.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://sh.hahajie.cn

[U56] PHP：命名参数
来源：http://tf.huixinmuqiang.cn

f(a: 1, b: 2)
来源：http://wk.huanxung.cn

[U57] PHP：字符串插值
来源：http://pb.huixiangedu.cn

"值: {$a}"
来源：http://zf.shxzukj.cn

[U58] PHP：数组三件套
来源：http://yf.huanxung.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://aq.newstarts.cn

[U59] PHP：自定义排序
来源：http://vr.jctech888.com.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vp.shtwfgs.cn

[U60] PHP：JSON 编解码
来源：http://tv.wgjwhj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qj.hnjuh.cn

[U61] PHP：正则
来源：http://kn.huixinmuqiang.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://iw.shxzskj.cn

[U62] PHP：日期对象
来源：http://uk.haigaiapp.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qr.521024.cn

[U63] PHP：文件读写
来源：http://fx.hnjuh.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ic.szxytkj.cn

[U64] PHP：目录遍历
来源：http://we.nicolike.cn

glob("dir/*.php");  scandir("dir");
来源：http://rr.newstarts.cn

[U65] PHP：会话
来源：http://fp.shxzukj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rd.hnjuh.cn

[U66] PHP：设置 Cookie
来源：http://mh.9csxet.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rs.huixinmuqiang.cn

[U67] PHP：处理文件上传
来源：http://mb.wgjwhj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ga.nszjky.cn

[U68] PHP：PDO 连接
来源：http://rb.szsharing.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kt.hnjuh.cn

[U69] PHP：PDO 预处理
来源：http://jz.hnjuh.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://iv.521024.cn

[U70] PHP：PDO 事务
来源：http://bu.huixinmuqiang.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://se.huixinmuqiang.cn

[U71] PHP：抛出异常
来源：http://pp.yuexingan06.cn

throw new RuntimeException("失败", 500);
来源：http://mg.newstarts.cn

[U72] PHP：写错误日志
来源：http://bd.521024.cn

error_log("失败: " . $e->getMessage());
来源：http://uw.hahajie.cn

[U73] PHP：读取 ini 配置
来源：http://ww.jianghongdianzi.cn

parse_ini_file("config.ini", true)
来源：http://oi.szsharing.cn

[U74] PHP：读取环境变量
来源：http://bz.yuntaijiaju.cn

getenv("APP_ENV") ?: "production"
来源：http://zr.huanxung.cn

[U75] PHP：依赖注入
来源：http://zh.bookmarksfly.cn

composer require psr/container
来源：http://dv.yuntaijiaju.cn

[U76] PHP：简单路由
来源：http://rg.huanxung.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ul.szxytkj.cn

[U77] PHP：模板渲染
来源：http://xq.521024.cn

composer require twig/twig
来源：http://pt.yuntaijiaju.cn

[U78] PHP：单元测试
来源：http://wd.nszjky.cn

composer require --dev phpunit/phpunit
来源：http://ur.chemitech.net.cn

[U79] PHP：静态分析
来源：http://fg.jctech888.com.cn

composer require --dev phpstan/phpstan
来源：http://re.521024.cn

[U80] PHP：代码规范修复
来源：http://js.nszjky.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qi.nszjky.cn

[U81] JS：初始化项目
来源：http://kj.gzmigu.cn

npm init -y;  npm i express
来源：http://ay.colortex.cn

[U82] JS：package.json 脚本
来源：http://tc.hahajie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://eq.521024.cn

[U83] JS：ES Module 导入导出
来源：http://ys.panjiajie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zw.bjjhwx.cn

[U84] JS：CommonJS 写法
来源：http://ju.haigaiapp.cn

module.exports = { a };  const { a } = require("./m");
来源：http://kw.colortex.cn

[U85] JS：可选链
来源：http://xf.lnxyls.cn

a?.b?.c
来源：http://lc.muxihuayi.cn

[U86] JS：空值合并
来源：http://hr.newstarts.cn

a ?? b
来源：http://pk.panjiajie.cn

[U87] JS：解构默认值
来源：http://yo.huixiangedu.cn

const { a = 1, b = 2 } = obj;
来源：http://ab.wgjwhj.cn

[U88] JS：对象展开合并
来源：http://rw.huixinmuqiang.cn

{ ...a, ...b }
来源：http://lk.huixinmuqiang.cn

[U89] JS：数组去重
来源：http://im.asd995.cn

[...new Set(arr)]
来源：http://af.jianghongdianzi.cn

[U90] JS：数字数组排序
来源：http://lq.hahajie.cn

[...arr].sort((a, b) => a - b)
来源：http://gd.panjiajie.cn

[U91] JS：对象键值遍历
来源：http://fx.panjiajie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jk.9csxet.cn

[U92] JS：深拷贝
来源：http://ea.huixiangedu.cn

structuredClone(obj)
来源：http://kt.shxzskj.cn

[U93] JS：模板字符串
来源：http://dw.szsharing.cn

`共 ${n} 条`
来源：http://ih.huixiangedu.cn

[U94] JS：箭头函数
来源：http://ji.bjjhwx.cn

const double = x => x * 2;
来源：http://xt.yuexingan06.cn

[U95] JS：Promise 包装
来源：http://fs.haigaiapp.cn

new Promise((resolve, reject) => {})
来源：http://yj.huixiangedu.cn

[U96] JS：async/await 与异常
来源：http://kp.asd995.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://uj.colortex.cn

[U97] JS：并发请求
来源：http://gh.gzmigu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://cj.nicolike.cn

[U98] JS：fetch 带 JSON
来源：http://of.nicolike.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bv.huanxung.cn

[U99] JS：事件监听
来源：http://do.nszjky.cn

el.addEventListener("click", e => {})
来源：http://xm.huixiangedu.cn

[U100] JS：DOM 查询
来源：http://qn.asd995.cn

document.querySelector(".item")
来源：http://mt.haigaiapp.cn

[U101] JS：classList 操作
来源：http://gd.szsharing.cn

el.classList.toggle("active")
来源：http://er.colortex.cn

[U102] JS：本地存储
来源：http://jd.jianghongdianzi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://my.gzmigu.cn

[U103] JS：定时器
来源：http://lt.lnxyls.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://am.hnjuh.cn

[U104] JS：防抖
来源：http://cg.wgjwhj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bf.huixiangedu.cn

[U105] JS：节流
来源：http://iw.yuntaijiaju.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qp.chemitech.net.cn

[U106] JS：日期格式化
来源：http://ki.shxzskj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kh.shtwfgs.cn

[U107] JS：数字千分位
来源：http://ju.huixiangedu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lt.jctech888.com.cn

[U108] JS：随机整数
来源：http://zy.chemitech.net.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fk.wgjwhj.cn

[U109] JS：数组分组
来源：http://da.chemitech.net.cn

Object.groupBy(arr, x => x.type)
来源：http://ml.hahajie.cn

[U110] JS：数组分块
来源：http://no.9csxet.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vq.wgjwhj.cn

[U111] JS：对象转 Map
来源：http://qr.chemitech.net.cn

new Map(Object.entries(obj))
来源：http://gv.nszjky.cn

[U112] JS：字符串补位
来源：http://mo.jianghongdianzi.cn

"7".padStart(3, "0")
来源：http://hf.szsharing.cn

[U113] JS：正则替换全部
来源：http://cw.colortex.cn

s.replaceAll("a", "b")
来源：http://rz.wgjwhj.cn

[U114] JS：JSON 深比较
来源：http://pb.jianghongdianzi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://sd.hnjuh.cn

[U115] JS：生成 UUID
来源：http://nv.jianghongdianzi.cn

crypto.randomUUID()
来源：http://kd.bookmarksfly.cn

[U116] JS：类型检查（JSDoc）
来源：http://eu.szxytkj.cn

/** @param {string} name */ function f(name) {}
来源：http://vr.shxzskj.cn


<!-- 参考信息 -->