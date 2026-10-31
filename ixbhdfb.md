代发 wailian999

[T29] Swift：guard 提前返回
来源：http://vh.huanxung.cn

guard let x = opt else { return }
来源：http://om.lnxyls.cn

[T30] Swift：协议
来源：http://in.huixiangedu.cn

protocol Shape { func area() -> Double }
来源：http://ts.yuexingan06.cn

[T31] Lua：Hello World
来源：http://qn.bjjhwx.cn

print("Hello")
来源：http://tx.shxzukj.cn

[T32] Lua：局部变量
来源：http://cx.bookmarksfly.cn

local a = 1
来源：http://oc.szxytkj.cn

[T33] Lua：表（数组）
来源：http://jj.9csxet.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://bg.huixiangedu.cn

[T34] Lua：遍历表
来源：http://nu.nicolike.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vn.huixinmuqiang.cn

[T35] Lua：字典表
来源：http://fb.shxzskj.cn

local d = { a = 1 };  d.b = 2
来源：http://kz.szsharing.cn

[T36] Lua：函数
来源：http://bw.shxzskj.cn

function add(a, b) return a + b end
来源：http://ou.nicolike.cn

[T37] Lua：字符串拼接
来源：http://os.colortex.cn

"a" .. "b"
来源：http://fp.hnjuh.cn

[T38] Lua：条件
来源：http://fw.shtwfgs.cn

if x > 0 then print("正") end
来源：http://ny.szxytkj.cn

[T39] Lua：模式匹配
来源：http://vd.bookmarksfly.cn

string.find(s, "%d+")
来源：http://me.huixinmuqiang.cn

[T40] Lua：元表
来源：http://mr.huixiangedu.cn

setmetatable({}, { __index = base })
来源：http://fs.shxzskj.cn

[T41] Perl：Hello World
来源：http://up.lnxyls.cn

print "Hello\n";
来源：http://rq.yuexingan06.cn

[T42] Perl：变量类型
来源：http://ak.newstarts.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://my.bookmarksfly.cn

[T43] Perl：字符串插值
来源：http://yj.huixiangedu.cn

"值: $a"
来源：http://mx.jctech888.com.cn

[T44] Perl：条件
来源：http://qm.yuntaijiaju.cn

if ($a > 0) { print "正"; }
来源：http://oo.panjiajie.cn

[T45] Perl：数组遍历
来源：http://tm.nicolike.cn

for my $x (@arr) { print $x; }
来源：http://wl.jctech888.com.cn

[T46] Perl：哈希操作
来源：http://vu.yuntaijiaju.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sm.yuntaijiaju.cn

[T47] Perl：正则捕获
来源：http://rg.huixiangedu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jk.colortex.cn

[T48] Perl：正则替换
来源：http://xs.shxzskj.cn

$s =~ s/old/new/g;
来源：http://ju.nicolike.cn

[T49] Perl：函数
来源：http://ja.lnxyls.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sj.huixiangedu.cn

[T50] Perl：逐行读文件
来源：http://ql.nicolike.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zi.gzmigu.cn

while (my $line = <$fh>) { print $line; }
来源：http://nv.yuexingan06.cn

[T51] Scala：Hello World
来源：http://wf.shxzskj.cn

println("Hello")
来源：http://iz.asd995.cn

[T52] Scala：变量
来源：http://js.muxihuayi.cn

val a = 1;  var b = 2
来源：http://pl.gzmigu.cn

[T53] Scala：字符串插值
来源：http://ch.szxytkj.cn

s"值: $b"
来源：http://hw.9csxet.cn

[T54] Scala：集合映射
来源：http://uz.asd995.cn

List(1, 2, 3).map(_ * 2)
来源：http://vg.newstarts.cn

[T55] Scala：集合过滤
来源：http://nz.lnxyls.cn

List(1, 2, 3).filter(_ > 1)
来源：http://se.wgjwhj.cn

[T56] Scala：样例类
来源：http://yw.huanxung.cn

case class User(name: String, age: Int)
来源：http://mj.colortex.cn

[T57] Scala：模式匹配
来源：http://vj.hnjuh.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://da.muxihuayi.cn

[T58] Scala：函数定义
来源：http://wk.shxzukj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://co.huixiangedu.cn

[T59] Scala：循环
来源：http://ws.bjjhwx.cn

for (i <- 1 to 10) println(i)
来源：http://vz.gzmigu.cn

[T60] Scala：折叠
来源：http://cc.newstarts.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ry.jianghongdianzi.cn

================================================================================
来源：http://ql.newstarts.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://eq.panjiajie.cn

================================================================================
来源：http://nt.wgjwhj.cn

[U01] Py：创建虚拟环境
来源：http://lp.bookmarksfly.cn

python -m venv .venv && source .venv/bin/activate
来源：http://es.yuexingan06.cn

[U02] Py：导出 / 安装依赖
来源：http://pc.jianghongdianzi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://br.szxytkj.cn

[U03] Py：加载 .env 配置
来源：http://ct.panjiajie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xq.nszjky.cn

[U04] Py：变量调试打印
来源：http://os.hnjuh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gr.lnxyls.cn

[U05] Py：列表去重且保序
来源：http://ay.hahajie.cn

list(dict.fromkeys(arr))
来源：http://nl.521024.cn

[U06] Py：合并两个字典
来源：http://bc.haigaiapp.cn

{**a, **b}
来源：http://ub.wgjwhj.cn

[U07] Py：反转字典键值
来源：http://kb.haigaiapp.cn

{v: k for k, v in d.items()}
来源：http://bw.asd995.cn

[U08] Py：展平二维列表
来源：http://ku.asd995.cn

[y for x in nested for y in x]
来源：http://zg.wgjwhj.cn

[U09] Py：字典取最大值的键
来源：http://eq.muxihuayi.cn

max(d, key=d.get)
来源：http://ui.newstarts.cn

[U10] Py：按值排序字典
来源：http://ef.panjiajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kg.bjjhwx.cn

[U11] Py：生成器表达式
来源：http://xk.gzmigu.cn

(x * 2 for x in arr)
来源：http://jr.newstarts.cn

[U12] Py：取出现最多的 3 个元素
来源：http://om.nicolike.cn

Counter(arr).most_common(3)
来源：http://ik.muxihuayi.cn

[U13] Py：固定长度队列
来源：http://mx.yuexingan06.cn

deque(maxlen=10)
来源：http://sf.jctech888.com.cn

[U14] Py：分组收集到列表
来源：http://ad.muxihuayi.cn

defaultdict(list)
来源：http://un.shxzukj.cn

[U15] Py：高精度计时
来源：http://vx.haigaiapp.cn

t = time.perf_counter()
来源：http://fl.panjiajie.cn

[U16] Py：命令行参数解析
来源：http://se.bookmarksfly.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kw.hahajie.cn

[U17] Py：初始化日志
来源：http://pz.jctech888.com.cn

logging.basicConfig(level=logging.INFO)
来源：http://ut.szxytkj.cn

[U18] Py：预编译正则
来源：http://dj.521024.cn

pat = re.compile(r"\d+")
来源：http://xi.yuntaijiaju.cn

[U19] Py：正则替换带回调
来源：http://ms.hnjuh.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xj.521024.cn

[U20] Py：缓存函数结果
来源：http://fi.gzmigu.cn

@functools.lru_cache(maxsize=None)
来源：http://in.jianghongdianzi.cn

[U21] Py：自定义上下文管理器
来源：http://mp.szxytkj.cn

@contextlib.contextmanager
来源：http://xt.szsharing.cn

[U22] Py：矩阵转置
来源：http://ov.9csxet.cn

list(zip(*m))
来源：http://wg.shxzskj.cn

[U23] Py：分块读取大文件
来源：http://ua.gzmigu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://uv.yuexingan06.cn

[U24] Py：路径操作
来源：http://yq.chemitech.net.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mh.huanxung.cn

[U25] Py：CSV 按字典读
来源：http://jp.9csxet.cn

csv.DictReader(f)
来源：http://md.szxytkj.cn

[U26] Py：并发下载
来源：http://we.yuexingan06.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://iv.asd995.cn

[U27] Py：异步 HTTP
来源：http://wf.szsharing.cn

aiohttp.ClientSession() 配合 async with
来源：http://lr.hnjuh.cn

[U28] Py：类型别名
来源：http://hg.panjiajie.cn

UserId = int
来源：http://ru.lnxyls.cn

[U29] Py：属性校验
来源：http://fe.nicolike.cn

@property 与 @x.setter 配合
来源：http://fn.haigaiapp.cn

[U30] Py：数据类
来源：http://fx.asd995.cn

@dataclass(slots=True)
来源：http://sx.nszjky.cn

[U31] Py：单测
来源：http://hn.colortex.cn

python -m pytest -q
来源：http://wk.haigaiapp.cn

[U32] Py：代码格式化
来源：http://hq.nszjky.cn

ruff format . && ruff check --fix .
来源：http://vg.yuntaijiaju.cn

[U33] Py：打包发布
来源：http://rm.shxzukj.cn

python -m build  （依赖 pyproject.toml）
来源：http://bg.shxzukj.cn

[U34] Py：判断编码
来源：http://ij.bookmarksfly.cn

chardet.detect(raw)
来源：http://wk.gzmigu.cn

[U35] Py：发送邮件
来源：http://ja.shxzskj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ok.panjiajie.cn

[U36] Py：定时任务
来源：http://pr.haigaiapp.cn

schedule.every(10).minutes.do(job)
来源：http://kz.gzmigu.cn

[U37] Py：读写 Excel
来源：http://tb.521024.cn

pandas.read_excel / DataFrame.to_excel
来源：http://bt.haigaiapp.cn

[U38] Py：获取脚本所在目录
来源：http://kj.jianghongdianzi.cn

Path(__file__).resolve().parent
来源：http://aw.yuntaijiaju.cn

[U39] Py：判断是否在交互环境
来源：http://tf.yuexingan06.cn

sys.stdout.isatty()
来源：http://jm.huixinmuqiang.cn

[U40] Py：打印到标准错误
来源：http://tt.9csxet.cn

print("err", file=sys.stderr)
来源：http://mn.szxytkj.cn

[U41] PHP：初始化 Composer 项目
来源：http://sb.asd995.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://pc.wgjwhj.cn

[U42] PHP：PSR-4 自动加载
来源：http://tm.huixinmuqiang.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gy.shxzskj.cn

[U43] PHP：声明命名空间
来源：http://qd.jctech888.com.cn

namespace App\Http;
来源：http://go.lnxyls.cn

[U44] PHP：开启严格类型
来源：http://hp.yuntaijiaju.cn

declare(strict_types=1);
来源：http://pm.yuntaijiaju.cn

[U45] PHP：类型声明与返回类型
来源：http://qm.shxzskj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qi.asd995.cn

[U46] PHP：可空类型
来源：http://mu.huanxung.cn

?string $name = null
来源：http://dh.bookmarksfly.cn

[U47] PHP：联合类型
来源：http://gw.huanxung.cn

int|string $id
来源：http://gj.colortex.cn

[U48] PHP：纯枚举
来源：http://ro.9csxet.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://iy.lnxyls.cn

[U49] PHP：只读属性
来源：http://zg.haigaiapp.cn

public readonly string $name
来源：http://gn.szxytkj.cn

[U50] PHP：构造器属性提升
来源：http://mx.nicolike.cn

public function __construct(private int $id) {}
来源：http://no.shtwfgs.cn

[U51] PHP：数组解构
来源：http://vj.bookmarksfly.cn

[$a, $b] = $arr;
来源：http://ov.bjjhwx.cn

[U52] PHP：箭头函数
来源：http://ee.chemitech.net.cn

$double = fn($x) => $x * 2;
来源：http://dy.huixinmuqiang.cn

[U53] PHP：空合并运算符
来源：http://je.9csxet.cn

$v = $a ?? $b ?? "default";
来源：http://vu.nszjky.cn

[U54] PHP：空安全调用
来源：http://ob.jctech888.com.cn

$obj?->method()
来源：http://db.shxzskj.cn

[U55] PHP：match 表达式
来源：http://yy.bookmarksfly.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bv.shxzskj.cn

[U56] PHP：命名参数
来源：http://cu.muxihuayi.cn

f(a: 1, b: 2)
来源：http://xw.huanxung.cn

[U57] PHP：字符串插值
来源：http://uq.huixinmuqiang.cn

"值: {$a}"
来源：http://ez.shxzukj.cn

[U58] PHP：数组三件套
来源：http://nw.huixinmuqiang.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jb.colortex.cn

[U59] PHP：自定义排序
来源：http://uf.gzmigu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xl.wgjwhj.cn

[U60] PHP：JSON 编解码
来源：http://tg.jctech888.com.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://uh.jctech888.com.cn

[U61] PHP：正则
来源：http://ol.wgjwhj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rf.521024.cn

[U62] PHP：日期对象
来源：http://nb.521024.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ad.asd995.cn

[U63] PHP：文件读写
来源：http://fi.newstarts.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zw.hahajie.cn

[U64] PHP：目录遍历
来源：http://fd.jianghongdianzi.cn

glob("dir/*.php");  scandir("dir");
来源：http://zo.panjiajie.cn

[U65] PHP：会话
来源：http://vr.yuntaijiaju.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://qj.jctech888.com.cn

[U66] PHP：设置 Cookie
来源：http://ka.huanxung.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wz.chemitech.net.cn

[U67] PHP：处理文件上传
来源：http://jm.hnjuh.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cv.jianghongdianzi.cn

[U68] PHP：PDO 连接
来源：http://wg.nszjky.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yc.haigaiapp.cn

[U69] PHP：PDO 预处理
来源：http://yu.shxzskj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vl.521024.cn

[U70] PHP：PDO 事务
来源：http://oz.shtwfgs.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dk.yuntaijiaju.cn

[U71] PHP：抛出异常
来源：http://li.bjjhwx.cn

throw new RuntimeException("失败", 500);
来源：http://um.yuntaijiaju.cn

[U72] PHP：写错误日志
来源：http://fs.newstarts.cn

error_log("失败: " . $e->getMessage());
来源：http://py.shxzskj.cn

[U73] PHP：读取 ini 配置
来源：http://oq.jianghongdianzi.cn

parse_ini_file("config.ini", true)
来源：http://mu.nszjky.cn

[U74] PHP：读取环境变量
来源：http://qq.hnjuh.cn

getenv("APP_ENV") ?: "production"
来源：http://ru.wgjwhj.cn

[U75] PHP：依赖注入
来源：http://cb.colortex.cn

composer require psr/container
来源：http://yz.chemitech.net.cn

[U76] PHP：简单路由
来源：http://fb.nszjky.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xt.nszjky.cn

[U77] PHP：模板渲染
来源：http://to.newstarts.cn

composer require twig/twig
来源：http://ka.muxihuayi.cn

[U78] PHP：单元测试
来源：http://gr.521024.cn

composer require --dev phpunit/phpunit
来源：http://qr.hnjuh.cn

[U79] PHP：静态分析
来源：http://vr.521024.cn

composer require --dev phpstan/phpstan
来源：http://xl.panjiajie.cn

[U80] PHP：代码规范修复
来源：http://dj.colortex.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://yd.jianghongdianzi.cn

[U81] JS：初始化项目
来源：http://mw.shtwfgs.cn

npm init -y;  npm i express
来源：http://yz.jctech888.com.cn

[U82] JS：package.json 脚本
来源：http://vg.szxytkj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kh.jctech888.com.cn

[U83] JS：ES Module 导入导出
来源：http://me.gzmigu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://wr.szsharing.cn

[U84] JS：CommonJS 写法
来源：http://di.huanxung.cn

module.exports = { a };  const { a } = require("./m");
来源：http://dp.asd995.cn

[U85] JS：可选链
来源：http://au.gzmigu.cn

a?.b?.c
来源：http://gl.chemitech.net.cn

[U86] JS：空值合并
来源：http://gq.asd995.cn

a ?? b
来源：http://tk.haigaiapp.cn

[U87] JS：解构默认值
来源：http://fr.asd995.cn

const { a = 1, b = 2 } = obj;
来源：http://jc.newstarts.cn

[U88] JS：对象展开合并
来源：http://jq.huanxung.cn

{ ...a, ...b }
来源：http://re.nszjky.cn

[U89] JS：数组去重
来源：http://yh.jianghongdianzi.cn

[...new Set(arr)]
来源：http://zr.huixinmuqiang.cn

[U90] JS：数字数组排序
来源：http://sk.yuexingan06.cn

[...arr].sort((a, b) => a - b)
来源：http://et.gzmigu.cn

[U91] JS：对象键值遍历
来源：http://yy.hnjuh.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fk.shtwfgs.cn

[U92] JS：深拷贝
来源：http://tn.wgjwhj.cn

structuredClone(obj)
来源：http://id.colortex.cn

[U93] JS：模板字符串
来源：http://wx.bookmarksfly.cn

`共 ${n} 条`
来源：http://ni.lnxyls.cn

[U94] JS：箭头函数
来源：http://pt.szsharing.cn

const double = x => x * 2;
来源：http://gu.asd995.cn

[U95] JS：Promise 包装
来源：http://ng.hahajie.cn

new Promise((resolve, reject) => {})
来源：http://oy.colortex.cn

[U96] JS：async/await 与异常
来源：http://gq.bookmarksfly.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://iu.haigaiapp.cn

[U97] JS：并发请求
来源：http://wf.panjiajie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://mm.9csxet.cn

[U98] JS：fetch 带 JSON
来源：http://vz.bjjhwx.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://in.hnjuh.cn

[U99] JS：事件监听
来源：http://nw.yuexingan06.cn

el.addEventListener("click", e => {})
来源：http://dt.521024.cn

[U100] JS：DOM 查询
来源：http://zx.szxytkj.cn

document.querySelector(".item")
来源：http://oq.lnxyls.cn

[U101] JS：classList 操作
来源：http://sv.colortex.cn

el.classList.toggle("active")
来源：http://dd.szxytkj.cn

[U102] JS：本地存储
来源：http://qh.wgjwhj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ta.wgjwhj.cn

[U103] JS：定时器
来源：http://gr.bjjhwx.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://aw.hahajie.cn

[U104] JS：防抖
来源：http://zj.shtwfgs.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fa.shxzskj.cn

[U105] JS：节流
来源：http://qz.jctech888.com.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://aj.colortex.cn

[U106] JS：日期格式化
来源：http://wl.jianghongdianzi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://np.shtwfgs.cn

[U107] JS：数字千分位
来源：http://ho.szxytkj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ep.bookmarksfly.cn

[U108] JS：随机整数
来源：http://yv.huixiangedu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pa.nicolike.cn

[U109] JS：数组分组
来源：http://pf.colortex.cn

Object.groupBy(arr, x => x.type)
来源：http://ql.shtwfgs.cn

[U110] JS：数组分块
来源：http://ou.shxzukj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://iv.hnjuh.cn

[U111] JS：对象转 Map
来源：http://zz.nicolike.cn

new Map(Object.entries(obj))
来源：http://yc.bookmarksfly.cn

[U112] JS：字符串补位
来源：http://vy.asd995.cn

"7".padStart(3, "0")
来源：http://kp.jctech888.com.cn

[U113] JS：正则替换全部
来源：http://te.521024.cn

s.replaceAll("a", "b")
来源：http://cj.shxzukj.cn

[U114] JS：JSON 深比较
来源：http://ry.hahajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://nz.gzmigu.cn

[U115] JS：生成 UUID
来源：http://rn.panjiajie.cn

crypto.randomUUID()
来源：http://ad.huixiangedu.cn

[U116] JS：类型检查（JSDoc）
来源：http://bp.szsharing.cn

/** @param {string} name */ function f(name) {}
来源：http://gs.521024.cn


<!-- 参考信息 -->