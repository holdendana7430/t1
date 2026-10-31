代发 wailian999

[T31] Lua：Hello World
来源：http://fw.asd995.cn

print("Hello")
来源：http://er.shxzukj.cn

[T32] Lua：局部变量
来源：http://fc.bookmarksfly.cn

local a = 1
来源：http://pp.szsharing.cn

[T33] Lua：表（数组）
来源：http://ug.nicolike.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wm.shxzskj.cn

[T34] Lua：遍历表
来源：http://tg.jianghongdianzi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://lt.muxihuayi.cn

[T35] Lua：字典表
来源：http://mw.shtwfgs.cn

local d = { a = 1 };  d.b = 2
来源：http://sq.gzmigu.cn

[T36] Lua：函数
来源：http://rw.9csxet.cn

function add(a, b) return a + b end
来源：http://wj.yuntaijiaju.cn

[T37] Lua：字符串拼接
来源：http://gb.szxytkj.cn

"a" .. "b"
来源：http://qz.nicolike.cn

[T38] Lua：条件
来源：http://fm.huanxung.cn

if x > 0 then print("正") end
来源：http://uf.huixiangedu.cn

[T39] Lua：模式匹配
来源：http://ai.hnjuh.cn

string.find(s, "%d+")
来源：http://lk.haigaiapp.cn

[T40] Lua：元表
来源：http://wl.haigaiapp.cn

setmetatable({}, { __index = base })
来源：http://fl.shxzukj.cn

[T41] Perl：Hello World
来源：http://lp.huixiangedu.cn

print "Hello\n";
来源：http://ej.panjiajie.cn

[T42] Perl：变量类型
来源：http://fg.haigaiapp.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ve.lnxyls.cn

[T43] Perl：字符串插值
来源：http://rh.jctech888.com.cn

"值: $a"
来源：http://kb.yuntaijiaju.cn

[T44] Perl：条件
来源：http://jq.huixinmuqiang.cn

if ($a > 0) { print "正"; }
来源：http://ua.colortex.cn

[T45] Perl：数组遍历
来源：http://oc.colortex.cn

for my $x (@arr) { print $x; }
来源：http://bl.jianghongdianzi.cn

[T46] Perl：哈希操作
来源：http://uq.gzmigu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://eo.shxzukj.cn

[T47] Perl：正则捕获
来源：http://qd.bjjhwx.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://sl.hahajie.cn

[T48] Perl：正则替换
来源：http://yl.jianghongdianzi.cn

$s =~ s/old/new/g;
来源：http://fs.muxihuayi.cn

[T49] Perl：函数
来源：http://mk.9csxet.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lx.521024.cn

[T50] Perl：逐行读文件
来源：http://bp.wgjwhj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://cb.huixinmuqiang.cn

while (my $line = <$fh>) { print $line; }
来源：http://mq.haigaiapp.cn

[T51] Scala：Hello World
来源：http://jw.shtwfgs.cn

println("Hello")
来源：http://bu.yuntaijiaju.cn

[T52] Scala：变量
来源：http://gs.bjjhwx.cn

val a = 1;  var b = 2
来源：http://ql.huixiangedu.cn

[T53] Scala：字符串插值
来源：http://us.szxytkj.cn

s"值: $b"
来源：http://un.9csxet.cn

[T54] Scala：集合映射
来源：http://mn.nicolike.cn

List(1, 2, 3).map(_ * 2)
来源：http://xu.hahajie.cn

[T55] Scala：集合过滤
来源：http://et.panjiajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://yl.panjiajie.cn

[T56] Scala：样例类
来源：http://mk.nicolike.cn

case class User(name: String, age: Int)
来源：http://yq.shxzukj.cn

[T57] Scala：模式匹配
来源：http://qt.yuntaijiaju.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vu.yuexingan06.cn

[T58] Scala：函数定义
来源：http://tm.gzmigu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://uw.hnjuh.cn

[T59] Scala：循环
来源：http://na.wgjwhj.cn

for (i <- 1 to 10) println(i)
来源：http://rb.jctech888.com.cn

[T60] Scala：折叠
来源：http://is.bjjhwx.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hn.chemitech.net.cn

================================================================================
来源：http://cx.gzmigu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nd.szsharing.cn

================================================================================
来源：http://ek.521024.cn

[U01] Py：创建虚拟环境
来源：http://ws.shtwfgs.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bp.jianghongdianzi.cn

[U02] Py：导出 / 安装依赖
来源：http://mw.asd995.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nn.bookmarksfly.cn

[U03] Py：加载 .env 配置
来源：http://hm.panjiajie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://sw.shxzukj.cn

[U04] Py：变量调试打印
来源：http://jk.huixiangedu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jz.newstarts.cn

[U05] Py：列表去重且保序
来源：http://uq.jctech888.com.cn

list(dict.fromkeys(arr))
来源：http://xp.chemitech.net.cn

[U06] Py：合并两个字典
来源：http://ct.yuexingan06.cn

{**a, **b}
来源：http://qx.huixiangedu.cn

[U07] Py：反转字典键值
来源：http://tn.bookmarksfly.cn

{v: k for k, v in d.items()}
来源：http://oz.hahajie.cn

[U08] Py：展平二维列表
来源：http://qd.nszjky.cn

[y for x in nested for y in x]
来源：http://qo.muxihuayi.cn

[U09] Py：字典取最大值的键
来源：http://qx.shxzskj.cn

max(d, key=d.get)
来源：http://mz.jianghongdianzi.cn

[U10] Py：按值排序字典
来源：http://fw.newstarts.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fc.yuntaijiaju.cn

[U11] Py：生成器表达式
来源：http://kk.chemitech.net.cn

(x * 2 for x in arr)
来源：http://vk.bjjhwx.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ey.panjiajie.cn

Counter(arr).most_common(3)
来源：http://aj.huixiangedu.cn

[U13] Py：固定长度队列
来源：http://fa.bjjhwx.cn

deque(maxlen=10)
来源：http://dr.szxytkj.cn

[U14] Py：分组收集到列表
来源：http://ro.nszjky.cn

defaultdict(list)
来源：http://la.huixiangedu.cn

[U15] Py：高精度计时
来源：http://dv.jctech888.com.cn

t = time.perf_counter()
来源：http://ow.szsharing.cn

[U16] Py：命令行参数解析
来源：http://qj.haigaiapp.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yd.asd995.cn

[U17] Py：初始化日志
来源：http://iq.bookmarksfly.cn

logging.basicConfig(level=logging.INFO)
来源：http://hq.szsharing.cn

[U18] Py：预编译正则
来源：http://fg.chemitech.net.cn

pat = re.compile(r"\d+")
来源：http://in.jctech888.com.cn

[U19] Py：正则替换带回调
来源：http://xv.chemitech.net.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zq.wgjwhj.cn

[U20] Py：缓存函数结果
来源：http://kt.panjiajie.cn

@functools.lru_cache(maxsize=None)
来源：http://go.9csxet.cn

[U21] Py：自定义上下文管理器
来源：http://lx.yuexingan06.cn

@contextlib.contextmanager
来源：http://ya.bjjhwx.cn

[U22] Py：矩阵转置
来源：http://en.wgjwhj.cn

list(zip(*m))
来源：http://lg.hnjuh.cn

[U23] Py：分块读取大文件
来源：http://zf.newstarts.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ox.shtwfgs.cn

[U24] Py：路径操作
来源：http://eq.yuntaijiaju.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.newstarts.cn

[U25] Py：CSV 按字典读
来源：http://xp.bookmarksfly.cn

csv.DictReader(f)
来源：http://an.muxihuayi.cn

[U26] Py：并发下载
来源：http://vs.shtwfgs.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qy.newstarts.cn

[U27] Py：异步 HTTP
来源：http://sg.muxihuayi.cn

aiohttp.ClientSession() 配合 async with
来源：http://st.bookmarksfly.cn

[U28] Py：类型别名
来源：http://mc.szsharing.cn

UserId = int
来源：http://lj.chemitech.net.cn

[U29] Py：属性校验
来源：http://um.asd995.cn

@property 与 @x.setter 配合
来源：http://ts.jianghongdianzi.cn

[U30] Py：数据类
来源：http://lf.shxzskj.cn

@dataclass(slots=True)
来源：http://rf.hnjuh.cn

[U31] Py：单测
来源：http://gs.newstarts.cn

python -m pytest -q
来源：http://om.muxihuayi.cn

[U32] Py：代码格式化
来源：http://ri.shtwfgs.cn

ruff format . && ruff check --fix .
来源：http://yb.lnxyls.cn

[U33] Py：打包发布
来源：http://zb.muxihuayi.cn

python -m build  （依赖 pyproject.toml）
来源：http://ys.panjiajie.cn

[U34] Py：判断编码
来源：http://ui.wgjwhj.cn

chardet.detect(raw)
来源：http://mi.chemitech.net.cn

[U35] Py：发送邮件
来源：http://uj.szsharing.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mi.shxzukj.cn

[U36] Py：定时任务
来源：http://lz.haigaiapp.cn

schedule.every(10).minutes.do(job)
来源：http://yo.szxytkj.cn

[U37] Py：读写 Excel
来源：http://rk.jianghongdianzi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://cs.hahajie.cn

[U38] Py：获取脚本所在目录
来源：http://go.chemitech.net.cn

Path(__file__).resolve().parent
来源：http://wh.huixiangedu.cn

[U39] Py：判断是否在交互环境
来源：http://kq.colortex.cn

sys.stdout.isatty()
来源：http://aj.jianghongdianzi.cn

[U40] Py：打印到标准错误
来源：http://mx.newstarts.cn

print("err", file=sys.stderr)
来源：http://jz.huixiangedu.cn

[U41] PHP：初始化 Composer 项目
来源：http://ei.yuntaijiaju.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://df.bjjhwx.cn

[U42] PHP：PSR-4 自动加载
来源：http://gm.hahajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vb.yuexingan06.cn

[U43] PHP：声明命名空间
来源：http://vh.nszjky.cn

namespace App\Http;
来源：http://sd.szxytkj.cn

[U44] PHP：开启严格类型
来源：http://ef.jctech888.com.cn

declare(strict_types=1);
来源：http://no.chemitech.net.cn

[U45] PHP：类型声明与返回类型
来源：http://qu.gzmigu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ad.asd995.cn

[U46] PHP：可空类型
来源：http://mu.hnjuh.cn

?string $name = null
来源：http://sw.yuntaijiaju.cn

[U47] PHP：联合类型
来源：http://fw.shxzskj.cn

int|string $id
来源：http://nn.muxihuayi.cn

[U48] PHP：纯枚举
来源：http://an.hnjuh.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rm.nszjky.cn

[U49] PHP：只读属性
来源：http://fd.bjjhwx.cn

public readonly string $name
来源：http://ub.gzmigu.cn

[U50] PHP：构造器属性提升
来源：http://cy.yuexingan06.cn

public function __construct(private int $id) {}
来源：http://fl.shtwfgs.cn

[U51] PHP：数组解构
来源：http://dr.nszjky.cn

[$a, $b] = $arr;
来源：http://ea.hahajie.cn

[U52] PHP：箭头函数
来源：http://ej.hnjuh.cn

$double = fn($x) => $x * 2;
来源：http://jp.szxytkj.cn

[U53] PHP：空合并运算符
来源：http://mn.haigaiapp.cn

$v = $a ?? $b ?? "default";
来源：http://ri.yuntaijiaju.cn

[U54] PHP：空安全调用
来源：http://bb.yuntaijiaju.cn

$obj?->method()
来源：http://wi.hnjuh.cn

[U55] PHP：match 表达式
来源：http://xe.yuntaijiaju.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://le.9csxet.cn

[U56] PHP：命名参数
来源：http://lm.muxihuayi.cn

f(a: 1, b: 2)
来源：http://im.hahajie.cn

[U57] PHP：字符串插值
来源：http://re.haigaiapp.cn

"值: {$a}"
来源：http://fk.yuexingan06.cn

[U58] PHP：数组三件套
来源：http://xa.yuexingan06.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ie.9csxet.cn

[U59] PHP：自定义排序
来源：http://mq.muxihuayi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jh.shtwfgs.cn

[U60] PHP：JSON 编解码
来源：http://kx.huanxung.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zh.szxytkj.cn

[U61] PHP：正则
来源：http://jm.szsharing.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dg.nicolike.cn

[U62] PHP：日期对象
来源：http://ii.newstarts.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://oq.szsharing.cn

[U63] PHP：文件读写
来源：http://su.asd995.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://py.chemitech.net.cn

[U64] PHP：目录遍历
来源：http://da.szsharing.cn

glob("dir/*.php");  scandir("dir");
来源：http://gu.yuexingan06.cn

[U65] PHP：会话
来源：http://to.bookmarksfly.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kg.chemitech.net.cn

[U66] PHP：设置 Cookie
来源：http://xu.yuexingan06.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vu.yuexingan06.cn

[U67] PHP：处理文件上传
来源：http://hu.gzmigu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sc.bookmarksfly.cn

[U68] PHP：PDO 连接
来源：http://wa.shxzskj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gr.lnxyls.cn

[U69] PHP：PDO 预处理
来源：http://jf.bjjhwx.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nh.shtwfgs.cn

[U70] PHP：PDO 事务
来源：http://gi.wgjwhj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bq.szsharing.cn

[U71] PHP：抛出异常
来源：http://ay.szsharing.cn

throw new RuntimeException("失败", 500);
来源：http://as.huixiangedu.cn

[U72] PHP：写错误日志
来源：http://pg.colortex.cn

error_log("失败: " . $e->getMessage());
来源：http://il.newstarts.cn

[U73] PHP：读取 ini 配置
来源：http://hs.jctech888.com.cn

parse_ini_file("config.ini", true)
来源：http://mm.panjiajie.cn

[U74] PHP：读取环境变量
来源：http://cc.shxzskj.cn

getenv("APP_ENV") ?: "production"
来源：http://xf.wgjwhj.cn

[U75] PHP：依赖注入
来源：http://vw.nicolike.cn

composer require psr/container
来源：http://oc.jianghongdianzi.cn

[U76] PHP：简单路由
来源：http://ne.szsharing.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.nicolike.cn

[U77] PHP：模板渲染
来源：http://zc.nicolike.cn

composer require twig/twig
来源：http://rb.nicolike.cn

[U78] PHP：单元测试
来源：http://xb.huixinmuqiang.cn

composer require --dev phpunit/phpunit
来源：http://qn.muxihuayi.cn

[U79] PHP：静态分析
来源：http://em.huixiangedu.cn

composer require --dev phpstan/phpstan
来源：http://iv.huixiangedu.cn

[U80] PHP：代码规范修复
来源：http://ga.huanxung.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://uk.lnxyls.cn

[U81] JS：初始化项目
来源：http://gu.521024.cn

npm init -y;  npm i express
来源：http://ml.newstarts.cn

[U82] JS：package.json 脚本
来源：http://sh.haigaiapp.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://no.muxihuayi.cn

[U83] JS：ES Module 导入导出
来源：http://hs.szsharing.cn

export const a = 1;  import { a } from "./m.js";
来源：http://gw.asd995.cn

[U84] JS：CommonJS 写法
来源：http://fn.jianghongdianzi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://jo.nszjky.cn

[U85] JS：可选链
来源：http://nu.szxytkj.cn

a?.b?.c
来源：http://jq.521024.cn

[U86] JS：空值合并
来源：http://pw.jctech888.com.cn

a ?? b
来源：http://bn.nszjky.cn

[U87] JS：解构默认值
来源：http://qn.chemitech.net.cn

const { a = 1, b = 2 } = obj;
来源：http://fv.huixinmuqiang.cn

[U88] JS：对象展开合并
来源：http://ic.nicolike.cn

{ ...a, ...b }
来源：http://yj.asd995.cn

[U89] JS：数组去重
来源：http://yd.lnxyls.cn

[...new Set(arr)]
来源：http://vs.colortex.cn

[U90] JS：数字数组排序
来源：http://cn.jctech888.com.cn

[...arr].sort((a, b) => a - b)
来源：http://od.jctech888.com.cn

[U91] JS：对象键值遍历
来源：http://lt.newstarts.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dh.9csxet.cn

[U92] JS：深拷贝
来源：http://iz.shxzskj.cn

structuredClone(obj)
来源：http://gm.bookmarksfly.cn

[U93] JS：模板字符串
来源：http://vr.521024.cn

`共 ${n} 条`
来源：http://fe.521024.cn

[U94] JS：箭头函数
来源：http://az.nszjky.cn

const double = x => x * 2;
来源：http://hw.9csxet.cn

[U95] JS：Promise 包装
来源：http://px.muxihuayi.cn

new Promise((resolve, reject) => {})
来源：http://ly.bjjhwx.cn

[U96] JS：async/await 与异常
来源：http://yh.521024.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sy.shxzskj.cn

[U97] JS：并发请求
来源：http://vy.huixinmuqiang.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ei.asd995.cn

[U98] JS：fetch 带 JSON
来源：http://fq.nszjky.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ns.yuntaijiaju.cn

[U99] JS：事件监听
来源：http://bl.muxihuayi.cn

el.addEventListener("click", e => {})
来源：http://eu.wgjwhj.cn

[U100] JS：DOM 查询
来源：http://dq.hahajie.cn

document.querySelector(".item")
来源：http://he.szsharing.cn

[U101] JS：classList 操作
来源：http://wo.nszjky.cn

el.classList.toggle("active")
来源：http://fl.wgjwhj.cn

[U102] JS：本地存储
来源：http://ch.lnxyls.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://nb.521024.cn

[U103] JS：定时器
来源：http://vk.szsharing.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ay.haigaiapp.cn

[U104] JS：防抖
来源：http://wh.huixiangedu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vb.shxzukj.cn

[U105] JS：节流
来源：http://zc.nszjky.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rd.521024.cn

[U106] JS：日期格式化
来源：http://ys.jctech888.com.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vm.521024.cn

[U107] JS：数字千分位
来源：http://ao.asd995.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rx.wgjwhj.cn

[U108] JS：随机整数
来源：http://ub.yuexingan06.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fq.bjjhwx.cn

[U109] JS：数组分组
来源：http://fh.9csxet.cn

Object.groupBy(arr, x => x.type)
来源：http://il.gzmigu.cn

[U110] JS：数组分块
来源：http://ck.nicolike.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://oa.9csxet.cn

[U111] JS：对象转 Map
来源：http://ye.panjiajie.cn

new Map(Object.entries(obj))
来源：http://sr.bookmarksfly.cn

[U112] JS：字符串补位
来源：http://jy.panjiajie.cn

"7".padStart(3, "0")
来源：http://xb.wgjwhj.cn

[U113] JS：正则替换全部
来源：http://vi.panjiajie.cn

s.replaceAll("a", "b")
来源：http://xr.521024.cn

[U114] JS：JSON 深比较
来源：http://fq.bookmarksfly.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://rp.szxytkj.cn

[U115] JS：生成 UUID
来源：http://hp.nicolike.cn

crypto.randomUUID()
来源：http://xh.huixinmuqiang.cn

[U116] JS：类型检查（JSDoc）
来源：http://iu.jianghongdianzi.cn

/** @param {string} name */ function f(name) {}
来源：http://vv.521024.cn

[U117] JS：单元测试
来源：http://bz.gzmigu.cn

npm i -D vitest;  npx vitest
来源：http://np.huixinmuqiang.cn

[U118] JS：开发服务器
来源：http://zv.jianghongdianzi.cn

npm i -D vite;  npx vite
来源：http://np.yuntaijiaju.cn


<!-- 参考信息 -->