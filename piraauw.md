代发 wailian999

[T39] Lua：模式匹配
来源：http://gp.newstarts.cn

string.find(s, "%d+")
来源：http://su.521024.cn

[T40] Lua：元表
来源：http://pl.huanxung.cn

setmetatable({}, { __index = base })
来源：http://kw.muxihuayi.cn

[T41] Perl：Hello World
来源：http://eg.chemitech.net.cn

print "Hello\n";
来源：http://mk.yuexingan06.cn

[T42] Perl：变量类型
来源：http://mw.521024.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://he.huixiangedu.cn

[T43] Perl：字符串插值
来源：http://oj.szxytkj.cn

"值: $a"
来源：http://jv.hahajie.cn

[T44] Perl：条件
来源：http://sd.bjjhwx.cn

if ($a > 0) { print "正"; }
来源：http://ju.shxzskj.cn

[T45] Perl：数组遍历
来源：http://ob.huanxung.cn

for my $x (@arr) { print $x; }
来源：http://mo.lnxyls.cn

[T46] Perl：哈希操作
来源：http://br.yuntaijiaju.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tv.haigaiapp.cn

[T47] Perl：正则捕获
来源：http://jn.9csxet.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wg.wgjwhj.cn

[T48] Perl：正则替换
来源：http://mw.bjjhwx.cn

$s =~ s/old/new/g;
来源：http://jj.panjiajie.cn

[T49] Perl：函数
来源：http://hp.huanxung.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ku.521024.cn

[T50] Perl：逐行读文件
来源：http://qk.yuexingan06.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://eq.gzmigu.cn

while (my $line = <$fh>) { print $line; }
来源：http://ui.shtwfgs.cn

[T51] Scala：Hello World
来源：http://mw.nszjky.cn

println("Hello")
来源：http://pw.jctech888.com.cn

[T52] Scala：变量
来源：http://pn.szxytkj.cn

val a = 1;  var b = 2
来源：http://cj.bjjhwx.cn

[T53] Scala：字符串插值
来源：http://vb.nicolike.cn

s"值: $b"
来源：http://nh.huanxung.cn

[T54] Scala：集合映射
来源：http://cy.szsharing.cn

List(1, 2, 3).map(_ * 2)
来源：http://ex.nicolike.cn

[T55] Scala：集合过滤
来源：http://vo.huanxung.cn

List(1, 2, 3).filter(_ > 1)
来源：http://st.newstarts.cn

[T56] Scala：样例类
来源：http://qe.haigaiapp.cn

case class User(name: String, age: Int)
来源：http://sg.szxytkj.cn

[T57] Scala：模式匹配
来源：http://ob.hahajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fp.huixinmuqiang.cn

[T58] Scala：函数定义
来源：http://vi.szxytkj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ty.haigaiapp.cn

[T59] Scala：循环
来源：http://xk.yuntaijiaju.cn

for (i <- 1 to 10) println(i)
来源：http://nz.hahajie.cn

[T60] Scala：折叠
来源：http://ul.huanxung.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mc.yuntaijiaju.cn

================================================================================
来源：http://wv.yuntaijiaju.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ny.newstarts.cn

================================================================================
来源：http://jr.colortex.cn

[U01] Py：创建虚拟环境
来源：http://hq.shxzukj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://az.bjjhwx.cn

[U02] Py：导出 / 安装依赖
来源：http://yk.chemitech.net.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qr.chemitech.net.cn

[U03] Py：加载 .env 配置
来源：http://da.huanxung.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://jv.chemitech.net.cn

[U04] Py：变量调试打印
来源：http://qp.huanxung.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mh.szsharing.cn

[U05] Py：列表去重且保序
来源：http://ru.szsharing.cn

list(dict.fromkeys(arr))
来源：http://nk.huixinmuqiang.cn

[U06] Py：合并两个字典
来源：http://eh.colortex.cn

{**a, **b}
来源：http://ix.gzmigu.cn

[U07] Py：反转字典键值
来源：http://yl.jctech888.com.cn

{v: k for k, v in d.items()}
来源：http://ko.yuexingan06.cn

[U08] Py：展平二维列表
来源：http://id.yuexingan06.cn

[y for x in nested for y in x]
来源：http://ue.panjiajie.cn

[U09] Py：字典取最大值的键
来源：http://cy.9csxet.cn

max(d, key=d.get)
来源：http://rf.huanxung.cn

[U10] Py：按值排序字典
来源：http://nr.hahajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mh.bookmarksfly.cn

[U11] Py：生成器表达式
来源：http://hx.szsharing.cn

(x * 2 for x in arr)
来源：http://rw.muxihuayi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ov.szxytkj.cn

Counter(arr).most_common(3)
来源：http://bl.huixinmuqiang.cn

[U13] Py：固定长度队列
来源：http://zo.bjjhwx.cn

deque(maxlen=10)
来源：http://qw.jctech888.com.cn

[U14] Py：分组收集到列表
来源：http://rj.panjiajie.cn

defaultdict(list)
来源：http://hq.yuexingan06.cn

[U15] Py：高精度计时
来源：http://lu.9csxet.cn

t = time.perf_counter()
来源：http://qe.yuexingan06.cn

[U16] Py：命令行参数解析
来源：http://vf.wgjwhj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yy.yuexingan06.cn

[U17] Py：初始化日志
来源：http://rb.nicolike.cn

logging.basicConfig(level=logging.INFO)
来源：http://do.shtwfgs.cn

[U18] Py：预编译正则
来源：http://jj.gzmigu.cn

pat = re.compile(r"\d+")
来源：http://ay.shtwfgs.cn

[U19] Py：正则替换带回调
来源：http://po.huanxung.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hc.nszjky.cn

[U20] Py：缓存函数结果
来源：http://xh.szxytkj.cn

@functools.lru_cache(maxsize=None)
来源：http://yc.panjiajie.cn

[U21] Py：自定义上下文管理器
来源：http://py.shxzskj.cn

@contextlib.contextmanager
来源：http://io.nicolike.cn

[U22] Py：矩阵转置
来源：http://wl.hahajie.cn

list(zip(*m))
来源：http://bu.haigaiapp.cn

[U23] Py：分块读取大文件
来源：http://me.yuexingan06.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rg.jianghongdianzi.cn

[U24] Py：路径操作
来源：http://rg.haigaiapp.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fv.colortex.cn

[U25] Py：CSV 按字典读
来源：http://zw.9csxet.cn

csv.DictReader(f)
来源：http://jm.huanxung.cn

[U26] Py：并发下载
来源：http://mz.shxzukj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fg.9csxet.cn

[U27] Py：异步 HTTP
来源：http://op.hnjuh.cn

aiohttp.ClientSession() 配合 async with
来源：http://pr.hahajie.cn

[U28] Py：类型别名
来源：http://ts.bookmarksfly.cn

UserId = int
来源：http://tr.newstarts.cn

[U29] Py：属性校验
来源：http://cc.szxytkj.cn

@property 与 @x.setter 配合
来源：http://ps.wgjwhj.cn

[U30] Py：数据类
来源：http://df.shtwfgs.cn

@dataclass(slots=True)
来源：http://up.bookmarksfly.cn

[U31] Py：单测
来源：http://vj.wgjwhj.cn

python -m pytest -q
来源：http://yt.wgjwhj.cn

[U32] Py：代码格式化
来源：http://vb.shtwfgs.cn

ruff format . && ruff check --fix .
来源：http://mv.bookmarksfly.cn

[U33] Py：打包发布
来源：http://jq.yuntaijiaju.cn

python -m build  （依赖 pyproject.toml）
来源：http://jz.shxzukj.cn

[U34] Py：判断编码
来源：http://bv.gzmigu.cn

chardet.detect(raw)
来源：http://du.szxytkj.cn

[U35] Py：发送邮件
来源：http://qd.shxzskj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://uw.hahajie.cn

[U36] Py：定时任务
来源：http://ix.huixiangedu.cn

schedule.every(10).minutes.do(job)
来源：http://ax.shxzukj.cn

[U37] Py：读写 Excel
来源：http://vd.szsharing.cn

pandas.read_excel / DataFrame.to_excel
来源：http://hl.shtwfgs.cn

[U38] Py：获取脚本所在目录
来源：http://aq.jctech888.com.cn

Path(__file__).resolve().parent
来源：http://an.hahajie.cn

[U39] Py：判断是否在交互环境
来源：http://qq.gzmigu.cn

sys.stdout.isatty()
来源：http://rh.haigaiapp.cn

[U40] Py：打印到标准错误
来源：http://bf.haigaiapp.cn

print("err", file=sys.stderr)
来源：http://cc.shxzukj.cn

[U41] PHP：初始化 Composer 项目
来源：http://eq.szxytkj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://rq.lnxyls.cn

[U42] PHP：PSR-4 自动加载
来源：http://yw.521024.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://af.colortex.cn

[U43] PHP：声明命名空间
来源：http://kb.wgjwhj.cn

namespace App\Http;
来源：http://sq.huanxung.cn

[U44] PHP：开启严格类型
来源：http://em.szxytkj.cn

declare(strict_types=1);
来源：http://nd.hahajie.cn

[U45] PHP：类型声明与返回类型
来源：http://yd.hnjuh.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://zw.hnjuh.cn

[U46] PHP：可空类型
来源：http://va.wgjwhj.cn

?string $name = null
来源：http://wb.jianghongdianzi.cn

[U47] PHP：联合类型
来源：http://on.haigaiapp.cn

int|string $id
来源：http://qw.yuexingan06.cn

[U48] PHP：纯枚举
来源：http://qx.521024.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jj.bjjhwx.cn

[U49] PHP：只读属性
来源：http://kp.bjjhwx.cn

public readonly string $name
来源：http://lv.asd995.cn

[U50] PHP：构造器属性提升
来源：http://eu.huanxung.cn

public function __construct(private int $id) {}
来源：http://pe.shxzukj.cn

[U51] PHP：数组解构
来源：http://dy.newstarts.cn

[$a, $b] = $arr;
来源：http://jq.bjjhwx.cn

[U52] PHP：箭头函数
来源：http://nk.jianghongdianzi.cn

$double = fn($x) => $x * 2;
来源：http://ps.colortex.cn

[U53] PHP：空合并运算符
来源：http://wl.jianghongdianzi.cn

$v = $a ?? $b ?? "default";
来源：http://bz.huixiangedu.cn

[U54] PHP：空安全调用
来源：http://hi.shtwfgs.cn

$obj?->method()
来源：http://bb.colortex.cn

[U55] PHP：match 表达式
来源：http://ue.huixinmuqiang.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wj.haigaiapp.cn

[U56] PHP：命名参数
来源：http://ri.gzmigu.cn

f(a: 1, b: 2)
来源：http://lg.muxihuayi.cn

[U57] PHP：字符串插值
来源：http://op.haigaiapp.cn

"值: {$a}"
来源：http://hh.hahajie.cn

[U58] PHP：数组三件套
来源：http://fu.gzmigu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ms.asd995.cn

[U59] PHP：自定义排序
来源：http://ty.gzmigu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://at.shxzskj.cn

[U60] PHP：JSON 编解码
来源：http://of.huanxung.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cg.gzmigu.cn

[U61] PHP：正则
来源：http://ia.bjjhwx.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bw.yuntaijiaju.cn

[U62] PHP：日期对象
来源：http://ge.muxihuayi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vu.lnxyls.cn

[U63] PHP：文件读写
来源：http://ur.shtwfgs.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jx.gzmigu.cn

[U64] PHP：目录遍历
来源：http://pz.shtwfgs.cn

glob("dir/*.php");  scandir("dir");
来源：http://xc.bookmarksfly.cn

[U65] PHP：会话
来源：http://hg.521024.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kb.shxzskj.cn

[U66] PHP：设置 Cookie
来源：http://wj.wgjwhj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mp.newstarts.cn

[U67] PHP：处理文件上传
来源：http://uj.shxzskj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://we.hahajie.cn

[U68] PHP：PDO 连接
来源：http://xh.chemitech.net.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nb.hnjuh.cn

[U69] PHP：PDO 预处理
来源：http://ox.chemitech.net.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rn.lnxyls.cn

[U70] PHP：PDO 事务
来源：http://eu.nicolike.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yg.wgjwhj.cn

[U71] PHP：抛出异常
来源：http://yw.jianghongdianzi.cn

throw new RuntimeException("失败", 500);
来源：http://vk.521024.cn

[U72] PHP：写错误日志
来源：http://ir.huixiangedu.cn

error_log("失败: " . $e->getMessage());
来源：http://fy.huixinmuqiang.cn

[U73] PHP：读取 ini 配置
来源：http://yp.huixinmuqiang.cn

parse_ini_file("config.ini", true)
来源：http://pl.yuntaijiaju.cn

[U74] PHP：读取环境变量
来源：http://zj.muxihuayi.cn

getenv("APP_ENV") ?: "production"
来源：http://sx.newstarts.cn

[U75] PHP：依赖注入
来源：http://zc.jianghongdianzi.cn

composer require psr/container
来源：http://zj.colortex.cn

[U76] PHP：简单路由
来源：http://vn.hnjuh.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://oj.colortex.cn

[U77] PHP：模板渲染
来源：http://ik.hahajie.cn

composer require twig/twig
来源：http://ib.shxzukj.cn

[U78] PHP：单元测试
来源：http://si.jctech888.com.cn

composer require --dev phpunit/phpunit
来源：http://qh.bookmarksfly.cn

[U79] PHP：静态分析
来源：http://eo.szxytkj.cn

composer require --dev phpstan/phpstan
来源：http://vh.lnxyls.cn

[U80] PHP：代码规范修复
来源：http://dm.asd995.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://yr.nicolike.cn

[U81] JS：初始化项目
来源：http://nw.muxihuayi.cn

npm init -y;  npm i express
来源：http://fw.yuntaijiaju.cn

[U82] JS：package.json 脚本
来源：http://ef.haigaiapp.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://eo.szxytkj.cn

[U83] JS：ES Module 导入导出
来源：http://sm.szxytkj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ed.muxihuayi.cn

[U84] JS：CommonJS 写法
来源：http://qh.yuexingan06.cn

module.exports = { a };  const { a } = require("./m");
来源：http://gd.huixiangedu.cn

[U85] JS：可选链
来源：http://by.shxzukj.cn

a?.b?.c
来源：http://yt.huanxung.cn

[U86] JS：空值合并
来源：http://id.lnxyls.cn

a ?? b
来源：http://ft.521024.cn

[U87] JS：解构默认值
来源：http://ba.muxihuayi.cn

const { a = 1, b = 2 } = obj;
来源：http://wr.wgjwhj.cn

[U88] JS：对象展开合并
来源：http://ac.shtwfgs.cn

{ ...a, ...b }
来源：http://aa.shxzukj.cn

[U89] JS：数组去重
来源：http://mv.9csxet.cn

[...new Set(arr)]
来源：http://tf.521024.cn

[U90] JS：数字数组排序
来源：http://ha.yuntaijiaju.cn

[...arr].sort((a, b) => a - b)
来源：http://jl.gzmigu.cn

[U91] JS：对象键值遍历
来源：http://io.szsharing.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jw.shtwfgs.cn

[U92] JS：深拷贝
来源：http://dx.huanxung.cn

structuredClone(obj)
来源：http://qd.nszjky.cn

[U93] JS：模板字符串
来源：http://id.521024.cn

`共 ${n} 条`
来源：http://ff.bookmarksfly.cn

[U94] JS：箭头函数
来源：http://jl.yuexingan06.cn

const double = x => x * 2;
来源：http://gq.nszjky.cn

[U95] JS：Promise 包装
来源：http://ak.9csxet.cn

new Promise((resolve, reject) => {})
来源：http://qd.jianghongdianzi.cn

[U96] JS：async/await 与异常
来源：http://ou.szxytkj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mi.bjjhwx.cn

[U97] JS：并发请求
来源：http://fz.lnxyls.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ws.nszjky.cn

[U98] JS：fetch 带 JSON
来源：http://bj.bookmarksfly.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pu.9csxet.cn

[U99] JS：事件监听
来源：http://dl.chemitech.net.cn

el.addEventListener("click", e => {})
来源：http://mo.521024.cn

[U100] JS：DOM 查询
来源：http://cx.bookmarksfly.cn

document.querySelector(".item")
来源：http://tz.huixinmuqiang.cn

[U101] JS：classList 操作
来源：http://qv.shtwfgs.cn

el.classList.toggle("active")
来源：http://ze.muxihuayi.cn

[U102] JS：本地存储
来源：http://dl.hahajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ct.jctech888.com.cn

[U103] JS：定时器
来源：http://nj.colortex.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vl.gzmigu.cn

[U104] JS：防抖
来源：http://ab.521024.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ek.nszjky.cn

[U105] JS：节流
来源：http://ab.haigaiapp.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mz.szsharing.cn

[U106] JS：日期格式化
来源：http://qn.muxihuayi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tp.yuexingan06.cn

[U107] JS：数字千分位
来源：http://cy.huixinmuqiang.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xb.bjjhwx.cn

[U108] JS：随机整数
来源：http://ml.9csxet.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ri.nszjky.cn

[U109] JS：数组分组
来源：http://qr.yuexingan06.cn

Object.groupBy(arr, x => x.type)
来源：http://ph.nicolike.cn

[U110] JS：数组分块
来源：http://bd.huixiangedu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zr.yuntaijiaju.cn

[U111] JS：对象转 Map
来源：http://pn.szxytkj.cn

new Map(Object.entries(obj))
来源：http://nw.hnjuh.cn

[U112] JS：字符串补位
来源：http://lj.jianghongdianzi.cn

"7".padStart(3, "0")
来源：http://dq.hnjuh.cn

[U113] JS：正则替换全部
来源：http://ql.yuexingan06.cn

s.replaceAll("a", "b")
来源：http://qa.bjjhwx.cn

[U114] JS：JSON 深比较
来源：http://mi.bjjhwx.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://mi.yuexingan06.cn

[U115] JS：生成 UUID
来源：http://ln.szsharing.cn

crypto.randomUUID()
来源：http://nz.wgjwhj.cn

[U116] JS：类型检查（JSDoc）
来源：http://hk.chemitech.net.cn

/** @param {string} name */ function f(name) {}
来源：http://pz.szxytkj.cn

[U117] JS：单元测试
来源：http://wk.nszjky.cn

npm i -D vitest;  npx vitest
来源：http://il.huixinmuqiang.cn

[U118] JS：开发服务器
来源：http://ah.chemitech.net.cn

npm i -D vite;  npx vite
来源：http://fa.szxytkj.cn

[U119] JS：生产构建
来源：http://cd.shxzskj.cn

npx vite build
来源：http://zh.nicolike.cn

[U120] JS：读取环境变量（Vite）
来源：http://rr.bookmarksfly.cn

import.meta.env.VITE_API_URL
来源：http://cg.bookmarksfly.cn

================================================================================
来源：http://qq.huixiangedu.cn

统计汇总
来源：http://tv.muxihuayi.cn

================================================================================
来源：http://et.hnjuh.cn

按语言统计（条）：
来源：http://mh.yuntaijiaju.cn

Python ......... 252
来源：http://oa.wgjwhj.cn

PHP ............ 252
来源：http://zq.huixiangedu.cn

JavaScript ..... 252
来源：http://qn.nicolike.cn

TypeScript ..... 212
来源：http://wm.asd995.cn

Java ........... 212
来源：http://zh.huixiangedu.cn

Go ............. 212
来源：http://ws.gzmigu.cn

Ruby ........... 212
来源：http://ix.asd995.cn

C# ............. 212
来源：http://dr.jianghongdianzi.cn


<!-- 参考信息 -->