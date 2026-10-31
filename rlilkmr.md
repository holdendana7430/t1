代发 wailian999

[T33] Lua：表（数组）
来源：http://mn.huixiangedu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://jg.jctech888.com.cn

[T34] Lua：遍历表
来源：http://se.shxzukj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://uf.haigaiapp.cn

[T35] Lua：字典表
来源：http://sw.huixinmuqiang.cn

local d = { a = 1 };  d.b = 2
来源：http://ts.panjiajie.cn

[T36] Lua：函数
来源：http://tf.hnjuh.cn

function add(a, b) return a + b end
来源：http://ix.huixinmuqiang.cn

[T37] Lua：字符串拼接
来源：http://jk.huanxung.cn

"a" .. "b"
来源：http://ws.panjiajie.cn

[T38] Lua：条件
来源：http://kt.yuntaijiaju.cn

if x > 0 then print("正") end
来源：http://ji.bjjhwx.cn

[T39] Lua：模式匹配
来源：http://fe.yuexingan06.cn

string.find(s, "%d+")
来源：http://pg.haigaiapp.cn

[T40] Lua：元表
来源：http://qa.nicolike.cn

setmetatable({}, { __index = base })
来源：http://cz.wgjwhj.cn

[T41] Perl：Hello World
来源：http://mw.hahajie.cn

print "Hello\n";
来源：http://ta.newstarts.cn

[T42] Perl：变量类型
来源：http://es.lnxyls.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fk.bjjhwx.cn

[T43] Perl：字符串插值
来源：http://tn.yuexingan06.cn

"值: $a"
来源：http://rr.haigaiapp.cn

[T44] Perl：条件
来源：http://qp.jianghongdianzi.cn

if ($a > 0) { print "正"; }
来源：http://ad.nszjky.cn

[T45] Perl：数组遍历
来源：http://of.nszjky.cn

for my $x (@arr) { print $x; }
来源：http://bu.shxzskj.cn

[T46] Perl：哈希操作
来源：http://vq.szxytkj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ii.panjiajie.cn

[T47] Perl：正则捕获
来源：http://pf.huanxung.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://yq.szsharing.cn

[T48] Perl：正则替换
来源：http://vz.newstarts.cn

$s =~ s/old/new/g;
来源：http://ld.lnxyls.cn

[T49] Perl：函数
来源：http://nd.colortex.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yy.lnxyls.cn

[T50] Perl：逐行读文件
来源：http://wt.panjiajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://vc.colortex.cn

while (my $line = <$fh>) { print $line; }
来源：http://ce.chemitech.net.cn

[T51] Scala：Hello World
来源：http://gn.shxzukj.cn

println("Hello")
来源：http://ar.newstarts.cn

[T52] Scala：变量
来源：http://wa.szxytkj.cn

val a = 1;  var b = 2
来源：http://iz.huixiangedu.cn

[T53] Scala：字符串插值
来源：http://my.shxzskj.cn

s"值: $b"
来源：http://wv.yuntaijiaju.cn

[T54] Scala：集合映射
来源：http://af.muxihuayi.cn

List(1, 2, 3).map(_ * 2)
来源：http://da.hahajie.cn

[T55] Scala：集合过滤
来源：http://cj.colortex.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ns.521024.cn

[T56] Scala：样例类
来源：http://kv.bjjhwx.cn

case class User(name: String, age: Int)
来源：http://ku.haigaiapp.cn

[T57] Scala：模式匹配
来源：http://om.colortex.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://bu.shxzukj.cn

[T58] Scala：函数定义
来源：http://gb.jianghongdianzi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://qy.asd995.cn

[T59] Scala：循环
来源：http://il.huixiangedu.cn

for (i <- 1 to 10) println(i)
来源：http://ez.gzmigu.cn

[T60] Scala：折叠
来源：http://hs.huixinmuqiang.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ti.shtwfgs.cn

================================================================================
来源：http://br.huixiangedu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vh.yuntaijiaju.cn

================================================================================
来源：http://mj.hnjuh.cn

[U01] Py：创建虚拟环境
来源：http://xc.muxihuayi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vv.bjjhwx.cn

[U02] Py：导出 / 安装依赖
来源：http://vo.bjjhwx.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fw.chemitech.net.cn

[U03] Py：加载 .env 配置
来源：http://uj.shtwfgs.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://mg.huixiangedu.cn

[U04] Py：变量调试打印
来源：http://tk.colortex.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jp.gzmigu.cn

[U05] Py：列表去重且保序
来源：http://na.haigaiapp.cn

list(dict.fromkeys(arr))
来源：http://nv.szxytkj.cn

[U06] Py：合并两个字典
来源：http://jy.chemitech.net.cn

{**a, **b}
来源：http://kn.panjiajie.cn

[U07] Py：反转字典键值
来源：http://tf.huanxung.cn

{v: k for k, v in d.items()}
来源：http://je.lnxyls.cn

[U08] Py：展平二维列表
来源：http://fe.chemitech.net.cn

[y for x in nested for y in x]
来源：http://uy.szxytkj.cn

[U09] Py：字典取最大值的键
来源：http://mr.jctech888.com.cn

max(d, key=d.get)
来源：http://cu.hnjuh.cn

[U10] Py：按值排序字典
来源：http://ko.szsharing.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jh.huanxung.cn

[U11] Py：生成器表达式
来源：http://zy.shtwfgs.cn

(x * 2 for x in arr)
来源：http://lb.yuexingan06.cn

[U12] Py：取出现最多的 3 个元素
来源：http://eh.haigaiapp.cn

Counter(arr).most_common(3)
来源：http://bv.521024.cn

[U13] Py：固定长度队列
来源：http://td.bookmarksfly.cn

deque(maxlen=10)
来源：http://bv.colortex.cn

[U14] Py：分组收集到列表
来源：http://cg.yuntaijiaju.cn

defaultdict(list)
来源：http://xu.jctech888.com.cn

[U15] Py：高精度计时
来源：http://fl.newstarts.cn

t = time.perf_counter()
来源：http://ne.chemitech.net.cn

[U16] Py：命令行参数解析
来源：http://ak.szxytkj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ji.521024.cn

[U17] Py：初始化日志
来源：http://ny.newstarts.cn

logging.basicConfig(level=logging.INFO)
来源：http://ht.hahajie.cn

[U18] Py：预编译正则
来源：http://pt.gzmigu.cn

pat = re.compile(r"\d+")
来源：http://de.asd995.cn

[U19] Py：正则替换带回调
来源：http://jg.huixinmuqiang.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sx.shxzskj.cn

[U20] Py：缓存函数结果
来源：http://bt.shxzskj.cn

@functools.lru_cache(maxsize=None)
来源：http://pc.chemitech.net.cn

[U21] Py：自定义上下文管理器
来源：http://dc.shtwfgs.cn

@contextlib.contextmanager
来源：http://ih.szsharing.cn

[U22] Py：矩阵转置
来源：http://pj.haigaiapp.cn

list(zip(*m))
来源：http://el.newstarts.cn

[U23] Py：分块读取大文件
来源：http://hz.panjiajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jt.hnjuh.cn

[U24] Py：路径操作
来源：http://jl.nicolike.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ec.wgjwhj.cn

[U25] Py：CSV 按字典读
来源：http://hh.bjjhwx.cn

csv.DictReader(f)
来源：http://ob.huanxung.cn

[U26] Py：并发下载
来源：http://kh.nszjky.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://he.huixiangedu.cn

[U27] Py：异步 HTTP
来源：http://zq.yuntaijiaju.cn

aiohttp.ClientSession() 配合 async with
来源：http://wv.huixinmuqiang.cn

[U28] Py：类型别名
来源：http://tg.huixiangedu.cn

UserId = int
来源：http://kv.bjjhwx.cn

[U29] Py：属性校验
来源：http://oz.nszjky.cn

@property 与 @x.setter 配合
来源：http://cn.9csxet.cn

[U30] Py：数据类
来源：http://zj.bookmarksfly.cn

@dataclass(slots=True)
来源：http://jy.yuntaijiaju.cn

[U31] Py：单测
来源：http://yi.asd995.cn

python -m pytest -q
来源：http://hi.szxytkj.cn

[U32] Py：代码格式化
来源：http://ag.nicolike.cn

ruff format . && ruff check --fix .
来源：http://rr.colortex.cn

[U33] Py：打包发布
来源：http://kn.haigaiapp.cn

python -m build  （依赖 pyproject.toml）
来源：http://re.asd995.cn

[U34] Py：判断编码
来源：http://pe.asd995.cn

chardet.detect(raw)
来源：http://ke.panjiajie.cn

[U35] Py：发送邮件
来源：http://kk.shxzukj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://sw.shxzukj.cn

[U36] Py：定时任务
来源：http://uh.521024.cn

schedule.every(10).minutes.do(job)
来源：http://qr.shtwfgs.cn

[U37] Py：读写 Excel
来源：http://zw.hahajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://fq.nszjky.cn

[U38] Py：获取脚本所在目录
来源：http://aq.gzmigu.cn

Path(__file__).resolve().parent
来源：http://vi.hnjuh.cn

[U39] Py：判断是否在交互环境
来源：http://df.szsharing.cn

sys.stdout.isatty()
来源：http://ui.hnjuh.cn

[U40] Py：打印到标准错误
来源：http://xm.newstarts.cn

print("err", file=sys.stderr)
来源：http://ff.colortex.cn

[U41] PHP：初始化 Composer 项目
来源：http://og.muxihuayi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qy.shxzskj.cn

[U42] PHP：PSR-4 自动加载
来源：http://zp.shtwfgs.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fs.huixiangedu.cn

[U43] PHP：声明命名空间
来源：http://oz.panjiajie.cn

namespace App\Http;
来源：http://az.jianghongdianzi.cn

[U44] PHP：开启严格类型
来源：http://kf.nicolike.cn

declare(strict_types=1);
来源：http://vu.szxytkj.cn

[U45] PHP：类型声明与返回类型
来源：http://xb.shtwfgs.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://lu.newstarts.cn

[U46] PHP：可空类型
来源：http://bn.panjiajie.cn

?string $name = null
来源：http://xd.huanxung.cn

[U47] PHP：联合类型
来源：http://qp.huanxung.cn

int|string $id
来源：http://rk.jctech888.com.cn

[U48] PHP：纯枚举
来源：http://el.lnxyls.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ml.huanxung.cn

[U49] PHP：只读属性
来源：http://ma.jctech888.com.cn

public readonly string $name
来源：http://gx.hnjuh.cn

[U50] PHP：构造器属性提升
来源：http://mx.shxzskj.cn

public function __construct(private int $id) {}
来源：http://rm.gzmigu.cn

[U51] PHP：数组解构
来源：http://lo.yuntaijiaju.cn

[$a, $b] = $arr;
来源：http://gh.asd995.cn

[U52] PHP：箭头函数
来源：http://bz.haigaiapp.cn

$double = fn($x) => $x * 2;
来源：http://vv.jianghongdianzi.cn

[U53] PHP：空合并运算符
来源：http://qw.muxihuayi.cn

$v = $a ?? $b ?? "default";
来源：http://qh.yuntaijiaju.cn

[U54] PHP：空安全调用
来源：http://ka.muxihuayi.cn

$obj?->method()
来源：http://ko.huixiangedu.cn

[U55] PHP：match 表达式
来源：http://lx.gzmigu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mg.szxytkj.cn

[U56] PHP：命名参数
来源：http://bd.szsharing.cn

f(a: 1, b: 2)
来源：http://at.gzmigu.cn

[U57] PHP：字符串插值
来源：http://vl.521024.cn

"值: {$a}"
来源：http://hl.521024.cn

[U58] PHP：数组三件套
来源：http://eg.szsharing.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fe.szxytkj.cn

[U59] PHP：自定义排序
来源：http://rj.bjjhwx.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fr.jctech888.com.cn

[U60] PHP：JSON 编解码
来源：http://eu.muxihuayi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fj.huixinmuqiang.cn

[U61] PHP：正则
来源：http://hu.chemitech.net.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hu.huanxung.cn

[U62] PHP：日期对象
来源：http://dx.chemitech.net.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zk.newstarts.cn

[U63] PHP：文件读写
来源：http://ax.gzmigu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://cs.shtwfgs.cn

[U64] PHP：目录遍历
来源：http://rv.haigaiapp.cn

glob("dir/*.php");  scandir("dir");
来源：http://md.bjjhwx.cn

[U65] PHP：会话
来源：http://na.newstarts.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://uo.nszjky.cn

[U66] PHP：设置 Cookie
来源：http://kv.9csxet.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vt.huixiangedu.cn

[U67] PHP：处理文件上传
来源：http://il.colortex.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wm.huanxung.cn

[U68] PHP：PDO 连接
来源：http://lb.bookmarksfly.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fm.jianghongdianzi.cn

[U69] PHP：PDO 预处理
来源：http://az.panjiajie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xz.wgjwhj.cn

[U70] PHP：PDO 事务
来源：http://tf.huixiangedu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ke.jctech888.com.cn

[U71] PHP：抛出异常
来源：http://st.yuexingan06.cn

throw new RuntimeException("失败", 500);
来源：http://gs.huixiangedu.cn

[U72] PHP：写错误日志
来源：http://je.yuexingan06.cn

error_log("失败: " . $e->getMessage());
来源：http://hg.newstarts.cn

[U73] PHP：读取 ini 配置
来源：http://be.9csxet.cn

parse_ini_file("config.ini", true)
来源：http://fa.9csxet.cn

[U74] PHP：读取环境变量
来源：http://to.chemitech.net.cn

getenv("APP_ENV") ?: "production"
来源：http://ar.panjiajie.cn

[U75] PHP：依赖注入
来源：http://gq.hahajie.cn

composer require psr/container
来源：http://xg.panjiajie.cn

[U76] PHP：简单路由
来源：http://ac.asd995.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://em.huixiangedu.cn

[U77] PHP：模板渲染
来源：http://kj.jctech888.com.cn

composer require twig/twig
来源：http://pf.521024.cn

[U78] PHP：单元测试
来源：http://fo.hnjuh.cn

composer require --dev phpunit/phpunit
来源：http://jt.huixinmuqiang.cn

[U79] PHP：静态分析
来源：http://vp.huixinmuqiang.cn

composer require --dev phpstan/phpstan
来源：http://ur.521024.cn

[U80] PHP：代码规范修复
来源：http://vk.huixiangedu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://zo.shtwfgs.cn

[U81] JS：初始化项目
来源：http://re.szxytkj.cn

npm init -y;  npm i express
来源：http://yn.szsharing.cn

[U82] JS：package.json 脚本
来源：http://gw.nszjky.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zu.shtwfgs.cn

[U83] JS：ES Module 导入导出
来源：http://jw.panjiajie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://rb.hnjuh.cn

[U84] JS：CommonJS 写法
来源：http://tx.huixinmuqiang.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wi.shxzukj.cn

[U85] JS：可选链
来源：http://ib.jianghongdianzi.cn

a?.b?.c
来源：http://wx.9csxet.cn

[U86] JS：空值合并
来源：http://jv.yuntaijiaju.cn

a ?? b
来源：http://ru.521024.cn

[U87] JS：解构默认值
来源：http://yv.bookmarksfly.cn

const { a = 1, b = 2 } = obj;
来源：http://pr.shxzskj.cn

[U88] JS：对象展开合并
来源：http://yh.wgjwhj.cn

{ ...a, ...b }
来源：http://al.nszjky.cn

[U89] JS：数组去重
来源：http://uv.szxytkj.cn

[...new Set(arr)]
来源：http://xv.nicolike.cn

[U90] JS：数字数组排序
来源：http://sa.huanxung.cn

[...arr].sort((a, b) => a - b)
来源：http://th.chemitech.net.cn

[U91] JS：对象键值遍历
来源：http://el.yuexingan06.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cd.bjjhwx.cn

[U92] JS：深拷贝
来源：http://wf.chemitech.net.cn

structuredClone(obj)
来源：http://yq.bjjhwx.cn

[U93] JS：模板字符串
来源：http://fo.jctech888.com.cn

`共 ${n} 条`
来源：http://zg.shtwfgs.cn

[U94] JS：箭头函数
来源：http://mo.yuntaijiaju.cn

const double = x => x * 2;
来源：http://wp.shxzukj.cn

[U95] JS：Promise 包装
来源：http://tr.asd995.cn

new Promise((resolve, reject) => {})
来源：http://zk.lnxyls.cn

[U96] JS：async/await 与异常
来源：http://aj.bjjhwx.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vf.panjiajie.cn

[U97] JS：并发请求
来源：http://gi.muxihuayi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vs.panjiajie.cn

[U98] JS：fetch 带 JSON
来源：http://df.szxytkj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://no.shxzskj.cn

[U99] JS：事件监听
来源：http://kj.hahajie.cn

el.addEventListener("click", e => {})
来源：http://hy.newstarts.cn

[U100] JS：DOM 查询
来源：http://fi.newstarts.cn

document.querySelector(".item")
来源：http://bn.521024.cn

[U101] JS：classList 操作
来源：http://xw.yuexingan06.cn

el.classList.toggle("active")
来源：http://ug.jianghongdianzi.cn

[U102] JS：本地存储
来源：http://hs.bjjhwx.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://cb.huixinmuqiang.cn

[U103] JS：定时器
来源：http://yg.panjiajie.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ww.nszjky.cn

[U104] JS：防抖
来源：http://hl.muxihuayi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dl.asd995.cn

[U105] JS：节流
来源：http://bd.panjiajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dc.jctech888.com.cn

[U106] JS：日期格式化
来源：http://xr.huixiangedu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yn.gzmigu.cn

[U107] JS：数字千分位
来源：http://jn.newstarts.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kj.yuntaijiaju.cn

[U108] JS：随机整数
来源：http://fg.newstarts.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ue.hahajie.cn

[U109] JS：数组分组
来源：http://wd.yuexingan06.cn

Object.groupBy(arr, x => x.type)
来源：http://yg.9csxet.cn

[U110] JS：数组分块
来源：http://fx.bjjhwx.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fh.hnjuh.cn

[U111] JS：对象转 Map
来源：http://xx.huixiangedu.cn

new Map(Object.entries(obj))
来源：http://xc.nszjky.cn

[U112] JS：字符串补位
来源：http://cp.yuntaijiaju.cn

"7".padStart(3, "0")
来源：http://hi.521024.cn

[U113] JS：正则替换全部
来源：http://an.szsharing.cn

s.replaceAll("a", "b")
来源：http://er.muxihuayi.cn

[U114] JS：JSON 深比较
来源：http://zd.colortex.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qj.9csxet.cn

[U115] JS：生成 UUID
来源：http://vy.bjjhwx.cn

crypto.randomUUID()
来源：http://wy.jianghongdianzi.cn

[U116] JS：类型检查（JSDoc）
来源：http://zy.nicolike.cn

/** @param {string} name */ function f(name) {}
来源：http://tt.huixinmuqiang.cn

[U117] JS：单元测试
来源：http://vu.hnjuh.cn

npm i -D vitest;  npx vitest
来源：http://xh.9csxet.cn

[U118] JS：开发服务器
来源：http://gr.muxihuayi.cn

npm i -D vite;  npx vite
来源：http://qp.huixinmuqiang.cn

[U119] JS：生产构建
来源：http://ag.bjjhwx.cn

npx vite build
来源：http://ce.gzmigu.cn

[U120] JS：读取环境变量（Vite）
来源：http://ir.huanxung.cn

import.meta.env.VITE_API_URL
来源：http://dw.colortex.cn


<!-- 参考信息 -->