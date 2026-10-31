代发 wailian999

[T31] Lua：Hello World
来源：http://sa.bjjhwx.cn

print("Hello")
来源：http://ds.jctech888.com.cn

[T32] Lua：局部变量
来源：http://on.colortex.cn

local a = 1
来源：http://vf.asd995.cn

[T33] Lua：表（数组）
来源：http://vz.wgjwhj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://dy.huixinmuqiang.cn

[T34] Lua：遍历表
来源：http://nn.hnjuh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rw.9csxet.cn

[T35] Lua：字典表
来源：http://uz.szxytkj.cn

local d = { a = 1 };  d.b = 2
来源：http://gk.huanxung.cn

[T36] Lua：函数
来源：http://pq.lnxyls.cn

function add(a, b) return a + b end
来源：http://pv.bookmarksfly.cn

[T37] Lua：字符串拼接
来源：http://ub.szsharing.cn

"a" .. "b"
来源：http://um.shxzukj.cn

[T38] Lua：条件
来源：http://ls.szsharing.cn

if x > 0 then print("正") end
来源：http://kb.asd995.cn

[T39] Lua：模式匹配
来源：http://jc.9csxet.cn

string.find(s, "%d+")
来源：http://qc.lnxyls.cn

[T40] Lua：元表
来源：http://tf.shtwfgs.cn

setmetatable({}, { __index = base })
来源：http://sl.szsharing.cn

[T41] Perl：Hello World
来源：http://nk.huanxung.cn

print "Hello\n";
来源：http://fb.huixiangedu.cn

[T42] Perl：变量类型
来源：http://ep.yuntaijiaju.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kf.szsharing.cn

[T43] Perl：字符串插值
来源：http://dh.haigaiapp.cn

"值: $a"
来源：http://ua.chemitech.net.cn

[T44] Perl：条件
来源：http://aw.huixinmuqiang.cn

if ($a > 0) { print "正"; }
来源：http://hq.huixiangedu.cn

[T45] Perl：数组遍历
来源：http://wb.colortex.cn

for my $x (@arr) { print $x; }
来源：http://xt.wgjwhj.cn

[T46] Perl：哈希操作
来源：http://ch.yuexingan06.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ay.newstarts.cn

[T47] Perl：正则捕获
来源：http://zf.hahajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rd.yuexingan06.cn

[T48] Perl：正则替换
来源：http://lu.szxytkj.cn

$s =~ s/old/new/g;
来源：http://fs.szxytkj.cn

[T49] Perl：函数
来源：http://qq.huixinmuqiang.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pt.bookmarksfly.cn

[T50] Perl：逐行读文件
来源：http://fi.hahajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ro.hnjuh.cn

while (my $line = <$fh>) { print $line; }
来源：http://eu.huixinmuqiang.cn

[T51] Scala：Hello World
来源：http://jt.lnxyls.cn

println("Hello")
来源：http://tk.shxzukj.cn

[T52] Scala：变量
来源：http://zv.9csxet.cn

val a = 1;  var b = 2
来源：http://dw.jianghongdianzi.cn

[T53] Scala：字符串插值
来源：http://ps.hnjuh.cn

s"值: $b"
来源：http://sr.lnxyls.cn

[T54] Scala：集合映射
来源：http://gn.szsharing.cn

List(1, 2, 3).map(_ * 2)
来源：http://qw.shxzukj.cn

[T55] Scala：集合过滤
来源：http://ln.asd995.cn

List(1, 2, 3).filter(_ > 1)
来源：http://lm.jianghongdianzi.cn

[T56] Scala：样例类
来源：http://bv.haigaiapp.cn

case class User(name: String, age: Int)
来源：http://cu.shxzukj.cn

[T57] Scala：模式匹配
来源：http://ec.szsharing.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://sn.bookmarksfly.cn

[T58] Scala：函数定义
来源：http://zo.hahajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bh.haigaiapp.cn

[T59] Scala：循环
来源：http://zy.newstarts.cn

for (i <- 1 to 10) println(i)
来源：http://td.nszjky.cn

[T60] Scala：折叠
来源：http://al.haigaiapp.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://uf.jianghongdianzi.cn

================================================================================
来源：http://hc.nszjky.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rt.muxihuayi.cn

================================================================================
来源：http://ln.jianghongdianzi.cn

[U01] Py：创建虚拟环境
来源：http://xi.wgjwhj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nd.huanxung.cn

[U02] Py：导出 / 安装依赖
来源：http://lo.hahajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wj.huanxung.cn

[U03] Py：加载 .env 配置
来源：http://ji.nszjky.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xd.asd995.cn

[U04] Py：变量调试打印
来源：http://dz.shtwfgs.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pt.chemitech.net.cn

[U05] Py：列表去重且保序
来源：http://ri.huanxung.cn

list(dict.fromkeys(arr))
来源：http://rv.shxzskj.cn

[U06] Py：合并两个字典
来源：http://ye.bookmarksfly.cn

{**a, **b}
来源：http://sm.chemitech.net.cn

[U07] Py：反转字典键值
来源：http://du.9csxet.cn

{v: k for k, v in d.items()}
来源：http://cz.gzmigu.cn

[U08] Py：展平二维列表
来源：http://th.bjjhwx.cn

[y for x in nested for y in x]
来源：http://md.asd995.cn

[U09] Py：字典取最大值的键
来源：http://qm.asd995.cn

max(d, key=d.get)
来源：http://br.panjiajie.cn

[U10] Py：按值排序字典
来源：http://rl.521024.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wr.shtwfgs.cn

[U11] Py：生成器表达式
来源：http://lb.huanxung.cn

(x * 2 for x in arr)
来源：http://pf.wgjwhj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xz.colortex.cn

Counter(arr).most_common(3)
来源：http://ix.wgjwhj.cn

[U13] Py：固定长度队列
来源：http://je.wgjwhj.cn

deque(maxlen=10)
来源：http://jk.huixiangedu.cn

[U14] Py：分组收集到列表
来源：http://dt.gzmigu.cn

defaultdict(list)
来源：http://vy.wgjwhj.cn

[U15] Py：高精度计时
来源：http://lm.haigaiapp.cn

t = time.perf_counter()
来源：http://wc.wgjwhj.cn

[U16] Py：命令行参数解析
来源：http://fy.bjjhwx.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vx.asd995.cn

[U17] Py：初始化日志
来源：http://og.shtwfgs.cn

logging.basicConfig(level=logging.INFO)
来源：http://gx.newstarts.cn

[U18] Py：预编译正则
来源：http://wg.shxzukj.cn

pat = re.compile(r"\d+")
来源：http://dq.jctech888.com.cn

[U19] Py：正则替换带回调
来源：http://pn.yuexingan06.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zb.bookmarksfly.cn

[U20] Py：缓存函数结果
来源：http://zu.newstarts.cn

@functools.lru_cache(maxsize=None)
来源：http://nq.shxzskj.cn

[U21] Py：自定义上下文管理器
来源：http://xs.huixiangedu.cn

@contextlib.contextmanager
来源：http://zl.yuexingan06.cn

[U22] Py：矩阵转置
来源：http://gh.gzmigu.cn

list(zip(*m))
来源：http://bc.colortex.cn

[U23] Py：分块读取大文件
来源：http://rg.nicolike.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://no.hnjuh.cn

[U24] Py：路径操作
来源：http://dg.newstarts.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kd.shxzukj.cn

[U25] Py：CSV 按字典读
来源：http://ux.nszjky.cn

csv.DictReader(f)
来源：http://tj.szxytkj.cn

[U26] Py：并发下载
来源：http://di.hahajie.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jo.gzmigu.cn

[U27] Py：异步 HTTP
来源：http://ta.muxihuayi.cn

aiohttp.ClientSession() 配合 async with
来源：http://gi.shxzskj.cn

[U28] Py：类型别名
来源：http://kj.shxzskj.cn

UserId = int
来源：http://rq.nicolike.cn

[U29] Py：属性校验
来源：http://vl.huixiangedu.cn

@property 与 @x.setter 配合
来源：http://vp.bookmarksfly.cn

[U30] Py：数据类
来源：http://yk.lnxyls.cn

@dataclass(slots=True)
来源：http://ql.asd995.cn

[U31] Py：单测
来源：http://uo.huanxung.cn

python -m pytest -q
来源：http://kc.lnxyls.cn

[U32] Py：代码格式化
来源：http://li.nicolike.cn

ruff format . && ruff check --fix .
来源：http://bc.newstarts.cn

[U33] Py：打包发布
来源：http://hx.nszjky.cn

python -m build  （依赖 pyproject.toml）
来源：http://iz.hnjuh.cn

[U34] Py：判断编码
来源：http://wc.bjjhwx.cn

chardet.detect(raw)
来源：http://xb.chemitech.net.cn

[U35] Py：发送邮件
来源：http://ua.colortex.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mg.chemitech.net.cn

[U36] Py：定时任务
来源：http://zv.shtwfgs.cn

schedule.every(10).minutes.do(job)
来源：http://yz.yuexingan06.cn

[U37] Py：读写 Excel
来源：http://ma.yuexingan06.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ky.jctech888.com.cn

[U38] Py：获取脚本所在目录
来源：http://jj.hnjuh.cn

Path(__file__).resolve().parent
来源：http://mb.yuntaijiaju.cn

[U39] Py：判断是否在交互环境
来源：http://my.bookmarksfly.cn

sys.stdout.isatty()
来源：http://xu.asd995.cn

[U40] Py：打印到标准错误
来源：http://yl.panjiajie.cn

print("err", file=sys.stderr)
来源：http://ad.hnjuh.cn

[U41] PHP：初始化 Composer 项目
来源：http://kp.jianghongdianzi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://tf.shtwfgs.cn

[U42] PHP：PSR-4 自动加载
来源：http://tc.yuntaijiaju.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gh.huanxung.cn

[U43] PHP：声明命名空间
来源：http://nm.hnjuh.cn

namespace App\Http;
来源：http://qu.newstarts.cn

[U44] PHP：开启严格类型
来源：http://ot.9csxet.cn

declare(strict_types=1);
来源：http://kt.yuntaijiaju.cn

[U45] PHP：类型声明与返回类型
来源：http://lh.yuntaijiaju.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jm.jianghongdianzi.cn

[U46] PHP：可空类型
来源：http://tw.bjjhwx.cn

?string $name = null
来源：http://rv.shxzukj.cn

[U47] PHP：联合类型
来源：http://zb.shxzskj.cn

int|string $id
来源：http://ah.nicolike.cn

[U48] PHP：纯枚举
来源：http://jx.bookmarksfly.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vm.shtwfgs.cn

[U49] PHP：只读属性
来源：http://lh.asd995.cn

public readonly string $name
来源：http://jc.hahajie.cn

[U50] PHP：构造器属性提升
来源：http://lk.muxihuayi.cn

public function __construct(private int $id) {}
来源：http://mu.bjjhwx.cn

[U51] PHP：数组解构
来源：http://di.haigaiapp.cn

[$a, $b] = $arr;
来源：http://tn.bjjhwx.cn

[U52] PHP：箭头函数
来源：http://de.hnjuh.cn

$double = fn($x) => $x * 2;
来源：http://sd.gzmigu.cn

[U53] PHP：空合并运算符
来源：http://ll.shxzskj.cn

$v = $a ?? $b ?? "default";
来源：http://gv.asd995.cn

[U54] PHP：空安全调用
来源：http://yd.hnjuh.cn

$obj?->method()
来源：http://ci.yuexingan06.cn

[U55] PHP：match 表达式
来源：http://qq.asd995.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qv.wgjwhj.cn

[U56] PHP：命名参数
来源：http://ce.nicolike.cn

f(a: 1, b: 2)
来源：http://un.bookmarksfly.cn

[U57] PHP：字符串插值
来源：http://gp.gzmigu.cn

"值: {$a}"
来源：http://oo.colortex.cn

[U58] PHP：数组三件套
来源：http://sz.jctech888.com.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zi.chemitech.net.cn

[U59] PHP：自定义排序
来源：http://de.chemitech.net.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lk.521024.cn

[U60] PHP：JSON 编解码
来源：http://ei.nszjky.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://sp.yuexingan06.cn

[U61] PHP：正则
来源：http://xp.shtwfgs.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fz.asd995.cn

[U62] PHP：日期对象
来源：http://ui.huixinmuqiang.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://od.hnjuh.cn

[U63] PHP：文件读写
来源：http://om.muxihuayi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vo.shtwfgs.cn

[U64] PHP：目录遍历
来源：http://ya.521024.cn

glob("dir/*.php");  scandir("dir");
来源：http://ys.panjiajie.cn

[U65] PHP：会话
来源：http://rc.bookmarksfly.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ts.chemitech.net.cn

[U66] PHP：设置 Cookie
来源：http://ba.bookmarksfly.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ns.jctech888.com.cn

[U67] PHP：处理文件上传
来源：http://ta.huanxung.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yx.nszjky.cn

[U68] PHP：PDO 连接
来源：http://pr.huanxung.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ax.jianghongdianzi.cn

[U69] PHP：PDO 预处理
来源：http://zd.hnjuh.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wy.521024.cn

[U70] PHP：PDO 事务
来源：http://on.bookmarksfly.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jy.bookmarksfly.cn

[U71] PHP：抛出异常
来源：http://af.huixinmuqiang.cn

throw new RuntimeException("失败", 500);
来源：http://wa.asd995.cn

[U72] PHP：写错误日志
来源：http://nl.bjjhwx.cn

error_log("失败: " . $e->getMessage());
来源：http://nx.nicolike.cn

[U73] PHP：读取 ini 配置
来源：http://cs.muxihuayi.cn

parse_ini_file("config.ini", true)
来源：http://fu.yuntaijiaju.cn

[U74] PHP：读取环境变量
来源：http://wk.bookmarksfly.cn

getenv("APP_ENV") ?: "production"
来源：http://sp.panjiajie.cn

[U75] PHP：依赖注入
来源：http://rz.huixiangedu.cn

composer require psr/container
来源：http://jj.huanxung.cn

[U76] PHP：简单路由
来源：http://dd.newstarts.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kx.huixinmuqiang.cn

[U77] PHP：模板渲染
来源：http://cq.9csxet.cn

composer require twig/twig
来源：http://vb.colortex.cn

[U78] PHP：单元测试
来源：http://ws.panjiajie.cn

composer require --dev phpunit/phpunit
来源：http://jb.huixinmuqiang.cn

[U79] PHP：静态分析
来源：http://vy.lnxyls.cn

composer require --dev phpstan/phpstan
来源：http://nt.bookmarksfly.cn

[U80] PHP：代码规范修复
来源：http://sv.521024.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://rj.huixiangedu.cn

[U81] JS：初始化项目
来源：http://zw.asd995.cn

npm init -y;  npm i express
来源：http://me.lnxyls.cn

[U82] JS：package.json 脚本
来源：http://nq.szxytkj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://aj.huanxung.cn

[U83] JS：ES Module 导入导出
来源：http://po.bookmarksfly.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ea.bookmarksfly.cn

[U84] JS：CommonJS 写法
来源：http://ra.yuntaijiaju.cn

module.exports = { a };  const { a } = require("./m");
来源：http://an.jctech888.com.cn

[U85] JS：可选链
来源：http://vf.wgjwhj.cn

a?.b?.c
来源：http://cx.nicolike.cn

[U86] JS：空值合并
来源：http://uj.yuntaijiaju.cn

a ?? b
来源：http://hl.szsharing.cn

[U87] JS：解构默认值
来源：http://hn.asd995.cn

const { a = 1, b = 2 } = obj;
来源：http://cp.jctech888.com.cn

[U88] JS：对象展开合并
来源：http://pj.nszjky.cn

{ ...a, ...b }
来源：http://mx.shxzskj.cn

[U89] JS：数组去重
来源：http://pa.asd995.cn

[...new Set(arr)]
来源：http://zi.wgjwhj.cn

[U90] JS：数字数组排序
来源：http://wr.szsharing.cn

[...arr].sort((a, b) => a - b)
来源：http://lq.bookmarksfly.cn

[U91] JS：对象键值遍历
来源：http://dp.gzmigu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://oe.nszjky.cn

[U92] JS：深拷贝
来源：http://re.muxihuayi.cn

structuredClone(obj)
来源：http://cp.9csxet.cn

[U93] JS：模板字符串
来源：http://go.huanxung.cn

`共 ${n} 条`
来源：http://it.newstarts.cn

[U94] JS：箭头函数
来源：http://ad.lnxyls.cn

const double = x => x * 2;
来源：http://zu.bjjhwx.cn

[U95] JS：Promise 包装
来源：http://pb.huanxung.cn

new Promise((resolve, reject) => {})
来源：http://pr.gzmigu.cn

[U96] JS：async/await 与异常
来源：http://wf.chemitech.net.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wr.wgjwhj.cn

[U97] JS：并发请求
来源：http://ke.jianghongdianzi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://re.panjiajie.cn

[U98] JS：fetch 带 JSON
来源：http://pr.shxzukj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nu.yuexingan06.cn

[U99] JS：事件监听
来源：http://wr.gzmigu.cn

el.addEventListener("click", e => {})
来源：http://rv.huanxung.cn

[U100] JS：DOM 查询
来源：http://wy.yuexingan06.cn

document.querySelector(".item")
来源：http://yh.szsharing.cn

[U101] JS：classList 操作
来源：http://tq.lnxyls.cn

el.classList.toggle("active")
来源：http://re.huanxung.cn

[U102] JS：本地存储
来源：http://mh.lnxyls.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xm.9csxet.cn

[U103] JS：定时器
来源：http://zc.newstarts.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jj.9csxet.cn

[U104] JS：防抖
来源：http://gr.panjiajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://py.colortex.cn

[U105] JS：节流
来源：http://rz.yuntaijiaju.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bm.jctech888.com.cn

[U106] JS：日期格式化
来源：http://me.nszjky.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ol.nicolike.cn

[U107] JS：数字千分位
来源：http://ef.haigaiapp.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://me.colortex.cn

[U108] JS：随机整数
来源：http://pf.huixiangedu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vw.newstarts.cn

[U109] JS：数组分组
来源：http://ai.huixinmuqiang.cn

Object.groupBy(arr, x => x.type)
来源：http://jk.wgjwhj.cn

[U110] JS：数组分块
来源：http://os.bjjhwx.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bv.szsharing.cn

[U111] JS：对象转 Map
来源：http://gs.gzmigu.cn

new Map(Object.entries(obj))
来源：http://oy.wgjwhj.cn

[U112] JS：字符串补位
来源：http://lg.shxzukj.cn

"7".padStart(3, "0")
来源：http://uc.shtwfgs.cn

[U113] JS：正则替换全部
来源：http://na.shxzukj.cn

s.replaceAll("a", "b")
来源：http://ff.asd995.cn

[U114] JS：JSON 深比较
来源：http://lu.yuntaijiaju.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://tv.huixinmuqiang.cn

[U115] JS：生成 UUID
来源：http://iv.wgjwhj.cn

crypto.randomUUID()
来源：http://xh.newstarts.cn

[U116] JS：类型检查（JSDoc）
来源：http://pv.jianghongdianzi.cn

/** @param {string} name */ function f(name) {}
来源：http://et.huixiangedu.cn

[U117] JS：单元测试
来源：http://do.lnxyls.cn

npm i -D vitest;  npx vitest
来源：http://ta.haigaiapp.cn

[U118] JS：开发服务器
来源：http://pl.haigaiapp.cn

npm i -D vite;  npx vite
来源：http://gp.hnjuh.cn


<!-- 参考信息 -->