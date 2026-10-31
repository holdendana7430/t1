代发 wailian999

[T33] Lua：表（数组）
来源：http://fp.521024.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://cq.huanxung.cn

[T34] Lua：遍历表
来源：http://ia.szxytkj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ir.colortex.cn

[T35] Lua：字典表
来源：http://cv.asd995.cn

local d = { a = 1 };  d.b = 2
来源：http://eu.panjiajie.cn

[T36] Lua：函数
来源：http://ng.szsharing.cn

function add(a, b) return a + b end
来源：http://ff.szxytkj.cn

[T37] Lua：字符串拼接
来源：http://zb.bjjhwx.cn

"a" .. "b"
来源：http://xa.huixinmuqiang.cn

[T38] Lua：条件
来源：http://eg.asd995.cn

if x > 0 then print("正") end
来源：http://zm.huanxung.cn

[T39] Lua：模式匹配
来源：http://hw.hahajie.cn

string.find(s, "%d+")
来源：http://rz.huixiangedu.cn

[T40] Lua：元表
来源：http://sr.521024.cn

setmetatable({}, { __index = base })
来源：http://et.panjiajie.cn

[T41] Perl：Hello World
来源：http://sv.nicolike.cn

print "Hello\n";
来源：http://gz.yuexingan06.cn

[T42] Perl：变量类型
来源：http://on.shxzukj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pi.muxihuayi.cn

[T43] Perl：字符串插值
来源：http://ma.hahajie.cn

"值: $a"
来源：http://yx.yuntaijiaju.cn

[T44] Perl：条件
来源：http://ek.haigaiapp.cn

if ($a > 0) { print "正"; }
来源：http://pm.shtwfgs.cn

[T45] Perl：数组遍历
来源：http://qe.jianghongdianzi.cn

for my $x (@arr) { print $x; }
来源：http://ns.shtwfgs.cn

[T46] Perl：哈希操作
来源：http://rg.hahajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xk.yuntaijiaju.cn

[T47] Perl：正则捕获
来源：http://ed.yuexingan06.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://td.521024.cn

[T48] Perl：正则替换
来源：http://on.asd995.cn

$s =~ s/old/new/g;
来源：http://ww.hahajie.cn

[T49] Perl：函数
来源：http://th.nszjky.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://os.shtwfgs.cn

[T50] Perl：逐行读文件
来源：http://bf.haigaiapp.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://dt.yuntaijiaju.cn

while (my $line = <$fh>) { print $line; }
来源：http://qt.newstarts.cn

[T51] Scala：Hello World
来源：http://sc.nicolike.cn

println("Hello")
来源：http://dc.huixinmuqiang.cn

[T52] Scala：变量
来源：http://te.hnjuh.cn

val a = 1;  var b = 2
来源：http://zw.wgjwhj.cn

[T53] Scala：字符串插值
来源：http://da.jianghongdianzi.cn

s"值: $b"
来源：http://il.szsharing.cn

[T54] Scala：集合映射
来源：http://ji.panjiajie.cn

List(1, 2, 3).map(_ * 2)
来源：http://ga.huixinmuqiang.cn

[T55] Scala：集合过滤
来源：http://ss.huixiangedu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ba.szsharing.cn

[T56] Scala：样例类
来源：http://mp.nszjky.cn

case class User(name: String, age: Int)
来源：http://fd.yuexingan06.cn

[T57] Scala：模式匹配
来源：http://ld.jctech888.com.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ds.9csxet.cn

[T58] Scala：函数定义
来源：http://vo.jianghongdianzi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://sd.yuntaijiaju.cn

[T59] Scala：循环
来源：http://dl.huixiangedu.cn

for (i <- 1 to 10) println(i)
来源：http://gg.bookmarksfly.cn

[T60] Scala：折叠
来源：http://bn.jianghongdianzi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cc.colortex.cn

================================================================================
来源：http://mu.huixinmuqiang.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zr.bjjhwx.cn

================================================================================
来源：http://dx.9csxet.cn

[U01] Py：创建虚拟环境
来源：http://sl.shtwfgs.cn

python -m venv .venv && source .venv/bin/activate
来源：http://kd.yuntaijiaju.cn

[U02] Py：导出 / 安装依赖
来源：http://nm.asd995.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jn.gzmigu.cn

[U03] Py：加载 .env 配置
来源：http://ut.gzmigu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://yp.hnjuh.cn

[U04] Py：变量调试打印
来源：http://jc.haigaiapp.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hm.panjiajie.cn

[U05] Py：列表去重且保序
来源：http://kt.haigaiapp.cn

list(dict.fromkeys(arr))
来源：http://uc.hnjuh.cn

[U06] Py：合并两个字典
来源：http://av.shxzskj.cn

{**a, **b}
来源：http://cw.shxzskj.cn

[U07] Py：反转字典键值
来源：http://tg.szxytkj.cn

{v: k for k, v in d.items()}
来源：http://qc.jctech888.com.cn

[U08] Py：展平二维列表
来源：http://kf.gzmigu.cn

[y for x in nested for y in x]
来源：http://gu.haigaiapp.cn

[U09] Py：字典取最大值的键
来源：http://xf.asd995.cn

max(d, key=d.get)
来源：http://sb.nicolike.cn

[U10] Py：按值排序字典
来源：http://is.yuexingan06.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jv.shxzskj.cn

[U11] Py：生成器表达式
来源：http://ys.huixinmuqiang.cn

(x * 2 for x in arr)
来源：http://ib.nicolike.cn

[U12] Py：取出现最多的 3 个元素
来源：http://jb.chemitech.net.cn

Counter(arr).most_common(3)
来源：http://bf.szxytkj.cn

[U13] Py：固定长度队列
来源：http://lz.asd995.cn

deque(maxlen=10)
来源：http://te.huixiangedu.cn

[U14] Py：分组收集到列表
来源：http://kf.colortex.cn

defaultdict(list)
来源：http://ce.huixinmuqiang.cn

[U15] Py：高精度计时
来源：http://en.szsharing.cn

t = time.perf_counter()
来源：http://pe.newstarts.cn

[U16] Py：命令行参数解析
来源：http://rx.bjjhwx.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://je.szsharing.cn

[U17] Py：初始化日志
来源：http://un.asd995.cn

logging.basicConfig(level=logging.INFO)
来源：http://io.wgjwhj.cn

[U18] Py：预编译正则
来源：http://iy.jctech888.com.cn

pat = re.compile(r"\d+")
来源：http://pc.bjjhwx.cn

[U19] Py：正则替换带回调
来源：http://rm.nicolike.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nv.hahajie.cn

[U20] Py：缓存函数结果
来源：http://pr.lnxyls.cn

@functools.lru_cache(maxsize=None)
来源：http://xi.nszjky.cn

[U21] Py：自定义上下文管理器
来源：http://yh.chemitech.net.cn

@contextlib.contextmanager
来源：http://ed.huixiangedu.cn

[U22] Py：矩阵转置
来源：http://tq.nicolike.cn

list(zip(*m))
来源：http://kv.asd995.cn

[U23] Py：分块读取大文件
来源：http://uc.hahajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dg.bjjhwx.cn

[U24] Py：路径操作
来源：http://lm.bjjhwx.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hj.huixinmuqiang.cn

[U25] Py：CSV 按字典读
来源：http://az.chemitech.net.cn

csv.DictReader(f)
来源：http://or.shxzukj.cn

[U26] Py：并发下载
来源：http://eh.lnxyls.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cs.huixinmuqiang.cn

[U27] Py：异步 HTTP
来源：http://kd.muxihuayi.cn

aiohttp.ClientSession() 配合 async with
来源：http://we.shxzukj.cn

[U28] Py：类型别名
来源：http://bu.shxzukj.cn

UserId = int
来源：http://jq.asd995.cn

[U29] Py：属性校验
来源：http://hx.yuexingan06.cn

@property 与 @x.setter 配合
来源：http://lc.muxihuayi.cn

[U30] Py：数据类
来源：http://gh.huixinmuqiang.cn

@dataclass(slots=True)
来源：http://zr.bjjhwx.cn

[U31] Py：单测
来源：http://kp.panjiajie.cn

python -m pytest -q
来源：http://qe.muxihuayi.cn

[U32] Py：代码格式化
来源：http://jb.bookmarksfly.cn

ruff format . && ruff check --fix .
来源：http://wq.panjiajie.cn

[U33] Py：打包发布
来源：http://gm.wgjwhj.cn

python -m build  （依赖 pyproject.toml）
来源：http://kg.haigaiapp.cn

[U34] Py：判断编码
来源：http://xx.shtwfgs.cn

chardet.detect(raw)
来源：http://cj.bjjhwx.cn

[U35] Py：发送邮件
来源：http://fk.huanxung.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xt.521024.cn

[U36] Py：定时任务
来源：http://tb.shxzskj.cn

schedule.every(10).minutes.do(job)
来源：http://hi.chemitech.net.cn

[U37] Py：读写 Excel
来源：http://zy.shxzskj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ex.shxzukj.cn

[U38] Py：获取脚本所在目录
来源：http://gi.panjiajie.cn

Path(__file__).resolve().parent
来源：http://qx.jianghongdianzi.cn

[U39] Py：判断是否在交互环境
来源：http://vy.chemitech.net.cn

sys.stdout.isatty()
来源：http://it.panjiajie.cn

[U40] Py：打印到标准错误
来源：http://tk.jctech888.com.cn

print("err", file=sys.stderr)
来源：http://li.panjiajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://li.yuexingan06.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://hl.bjjhwx.cn

[U42] PHP：PSR-4 自动加载
来源：http://fr.chemitech.net.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://km.colortex.cn

[U43] PHP：声明命名空间
来源：http://kv.panjiajie.cn

namespace App\Http;
来源：http://xx.jctech888.com.cn

[U44] PHP：开启严格类型
来源：http://zd.newstarts.cn

declare(strict_types=1);
来源：http://ez.huixinmuqiang.cn

[U45] PHP：类型声明与返回类型
来源：http://tc.hnjuh.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://nm.hahajie.cn

[U46] PHP：可空类型
来源：http://hz.bjjhwx.cn

?string $name = null
来源：http://zx.newstarts.cn

[U47] PHP：联合类型
来源：http://wy.huanxung.cn

int|string $id
来源：http://jr.colortex.cn

[U48] PHP：纯枚举
来源：http://ox.gzmigu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qz.nicolike.cn

[U49] PHP：只读属性
来源：http://fn.521024.cn

public readonly string $name
来源：http://hx.haigaiapp.cn

[U50] PHP：构造器属性提升
来源：http://xs.haigaiapp.cn

public function __construct(private int $id) {}
来源：http://ie.9csxet.cn

[U51] PHP：数组解构
来源：http://lv.nszjky.cn

[$a, $b] = $arr;
来源：http://iu.jctech888.com.cn

[U52] PHP：箭头函数
来源：http://ka.muxihuayi.cn

$double = fn($x) => $x * 2;
来源：http://xb.yuexingan06.cn

[U53] PHP：空合并运算符
来源：http://sn.hnjuh.cn

$v = $a ?? $b ?? "default";
来源：http://ct.521024.cn

[U54] PHP：空安全调用
来源：http://dz.chemitech.net.cn

$obj?->method()
来源：http://hz.panjiajie.cn

[U55] PHP：match 表达式
来源：http://af.wgjwhj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mc.9csxet.cn

[U56] PHP：命名参数
来源：http://gl.szxytkj.cn

f(a: 1, b: 2)
来源：http://ac.521024.cn

[U57] PHP：字符串插值
来源：http://fk.chemitech.net.cn

"值: {$a}"
来源：http://xa.gzmigu.cn

[U58] PHP：数组三件套
来源：http://ql.shxzukj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rd.bookmarksfly.cn

[U59] PHP：自定义排序
来源：http://jb.panjiajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qi.muxihuayi.cn

[U60] PHP：JSON 编解码
来源：http://rw.nszjky.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cf.chemitech.net.cn

[U61] PHP：正则
来源：http://sg.wgjwhj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ko.huanxung.cn

[U62] PHP：日期对象
来源：http://ak.nicolike.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uu.szsharing.cn

[U63] PHP：文件读写
来源：http://iy.hnjuh.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ae.9csxet.cn

[U64] PHP：目录遍历
来源：http://eo.9csxet.cn

glob("dir/*.php");  scandir("dir");
来源：http://st.shxzukj.cn

[U65] PHP：会话
来源：http://zw.panjiajie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://wk.jctech888.com.cn

[U66] PHP：设置 Cookie
来源：http://wu.gzmigu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cb.huixinmuqiang.cn

[U67] PHP：处理文件上传
来源：http://gk.nicolike.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hn.yuexingan06.cn

[U68] PHP：PDO 连接
来源：http://pz.colortex.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://um.huixiangedu.cn

[U69] PHP：PDO 预处理
来源：http://ld.jianghongdianzi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lg.gzmigu.cn

[U70] PHP：PDO 事务
来源：http://cq.chemitech.net.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lq.521024.cn

[U71] PHP：抛出异常
来源：http://xw.haigaiapp.cn

throw new RuntimeException("失败", 500);
来源：http://jw.colortex.cn

[U72] PHP：写错误日志
来源：http://tt.wgjwhj.cn

error_log("失败: " . $e->getMessage());
来源：http://tx.wgjwhj.cn

[U73] PHP：读取 ini 配置
来源：http://wy.9csxet.cn

parse_ini_file("config.ini", true)
来源：http://fi.521024.cn

[U74] PHP：读取环境变量
来源：http://xq.nszjky.cn

getenv("APP_ENV") ?: "production"
来源：http://ic.szsharing.cn

[U75] PHP：依赖注入
来源：http://aj.huixiangedu.cn

composer require psr/container
来源：http://gc.wgjwhj.cn

[U76] PHP：简单路由
来源：http://hl.haigaiapp.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bi.jctech888.com.cn

[U77] PHP：模板渲染
来源：http://jq.nszjky.cn

composer require twig/twig
来源：http://su.wgjwhj.cn

[U78] PHP：单元测试
来源：http://gc.gzmigu.cn

composer require --dev phpunit/phpunit
来源：http://au.haigaiapp.cn

[U79] PHP：静态分析
来源：http://sn.hnjuh.cn

composer require --dev phpstan/phpstan
来源：http://tt.colortex.cn

[U80] PHP：代码规范修复
来源：http://cw.wgjwhj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ui.yuntaijiaju.cn

[U81] JS：初始化项目
来源：http://pa.521024.cn

npm init -y;  npm i express
来源：http://pc.szsharing.cn

[U82] JS：package.json 脚本
来源：http://mj.asd995.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zl.newstarts.cn

[U83] JS：ES Module 导入导出
来源：http://ni.nszjky.cn

export const a = 1;  import { a } from "./m.js";
来源：http://nc.haigaiapp.cn

[U84] JS：CommonJS 写法
来源：http://ni.muxihuayi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ip.wgjwhj.cn

[U85] JS：可选链
来源：http://gk.muxihuayi.cn

a?.b?.c
来源：http://ve.nszjky.cn

[U86] JS：空值合并
来源：http://pu.shxzskj.cn

a ?? b
来源：http://vy.bookmarksfly.cn

[U87] JS：解构默认值
来源：http://ig.jctech888.com.cn

const { a = 1, b = 2 } = obj;
来源：http://fb.jctech888.com.cn

[U88] JS：对象展开合并
来源：http://xi.huanxung.cn

{ ...a, ...b }
来源：http://gd.bjjhwx.cn

[U89] JS：数组去重
来源：http://on.huanxung.cn

[...new Set(arr)]
来源：http://ma.nszjky.cn

[U90] JS：数字数组排序
来源：http://zj.newstarts.cn

[...arr].sort((a, b) => a - b)
来源：http://sr.szsharing.cn

[U91] JS：对象键值遍历
来源：http://cl.asd995.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ar.hahajie.cn

[U92] JS：深拷贝
来源：http://kr.huixiangedu.cn

structuredClone(obj)
来源：http://qm.colortex.cn

[U93] JS：模板字符串
来源：http://dz.huixiangedu.cn

`共 ${n} 条`
来源：http://gs.colortex.cn

[U94] JS：箭头函数
来源：http://ir.bjjhwx.cn

const double = x => x * 2;
来源：http://xb.jianghongdianzi.cn

[U95] JS：Promise 包装
来源：http://zx.colortex.cn

new Promise((resolve, reject) => {})
来源：http://fj.shxzukj.cn

[U96] JS：async/await 与异常
来源：http://wo.colortex.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://we.colortex.cn

[U97] JS：并发请求
来源：http://rg.bookmarksfly.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://yg.haigaiapp.cn

[U98] JS：fetch 带 JSON
来源：http://nr.hahajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bz.jianghongdianzi.cn

[U99] JS：事件监听
来源：http://oc.nicolike.cn

el.addEventListener("click", e => {})
来源：http://zg.lnxyls.cn

[U100] JS：DOM 查询
来源：http://nn.colortex.cn

document.querySelector(".item")
来源：http://ai.hnjuh.cn

[U101] JS：classList 操作
来源：http://nm.hnjuh.cn

el.classList.toggle("active")
来源：http://tc.yuexingan06.cn

[U102] JS：本地存储
来源：http://vt.hnjuh.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://fy.panjiajie.cn

[U103] JS：定时器
来源：http://li.huanxung.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kw.muxihuayi.cn

[U104] JS：防抖
来源：http://my.szsharing.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nx.521024.cn

[U105] JS：节流
来源：http://xi.szsharing.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nt.gzmigu.cn

[U106] JS：日期格式化
来源：http://sv.521024.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sr.shxzukj.cn

[U107] JS：数字千分位
来源：http://ou.szxytkj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ng.nszjky.cn

[U108] JS：随机整数
来源：http://xt.gzmigu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://la.bookmarksfly.cn

[U109] JS：数组分组
来源：http://ks.huixinmuqiang.cn

Object.groupBy(arr, x => x.type)
来源：http://ly.panjiajie.cn

[U110] JS：数组分块
来源：http://mv.chemitech.net.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ug.asd995.cn

[U111] JS：对象转 Map
来源：http://cd.shtwfgs.cn

new Map(Object.entries(obj))
来源：http://lb.panjiajie.cn

[U112] JS：字符串补位
来源：http://df.muxihuayi.cn

"7".padStart(3, "0")
来源：http://dx.shtwfgs.cn

[U113] JS：正则替换全部
来源：http://bk.szsharing.cn

s.replaceAll("a", "b")
来源：http://be.yuntaijiaju.cn

[U114] JS：JSON 深比较
来源：http://gs.gzmigu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://xq.shxzukj.cn

[U115] JS：生成 UUID
来源：http://yq.gzmigu.cn

crypto.randomUUID()
来源：http://jc.muxihuayi.cn

[U116] JS：类型检查（JSDoc）
来源：http://qn.chemitech.net.cn

/** @param {string} name */ function f(name) {}
来源：http://ue.521024.cn

[U117] JS：单元测试
来源：http://ga.chemitech.net.cn

npm i -D vitest;  npx vitest
来源：http://ck.huanxung.cn

[U118] JS：开发服务器
来源：http://ho.gzmigu.cn

npm i -D vite;  npx vite
来源：http://ke.yuntaijiaju.cn

[U119] JS：生产构建
来源：http://ol.jianghongdianzi.cn

npx vite build
来源：http://kk.shtwfgs.cn

[U120] JS：读取环境变量（Vite）
来源：http://gs.newstarts.cn

import.meta.env.VITE_API_URL
来源：http://eh.521024.cn


<!-- 参考信息 -->