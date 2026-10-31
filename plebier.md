代发 wailian999

[T39] Lua：模式匹配
来源：http://ay.nicolike.cn

string.find(s, "%d+")
来源：http://gp.newstarts.cn

[T40] Lua：元表
来源：http://ck.bookmarksfly.cn

setmetatable({}, { __index = base })
来源：http://hd.521024.cn

[T41] Perl：Hello World
来源：http://xe.9csxet.cn

print "Hello\n";
来源：http://zo.asd995.cn

[T42] Perl：变量类型
来源：http://wn.jianghongdianzi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://we.colortex.cn

[T43] Perl：字符串插值
来源：http://bj.panjiajie.cn

"值: $a"
来源：http://pr.huixiangedu.cn

[T44] Perl：条件
来源：http://fa.shxzskj.cn

if ($a > 0) { print "正"; }
来源：http://wm.521024.cn

[T45] Perl：数组遍历
来源：http://km.wgjwhj.cn

for my $x (@arr) { print $x; }
来源：http://qu.haigaiapp.cn

[T46] Perl：哈希操作
来源：http://ll.asd995.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zw.newstarts.cn

[T47] Perl：正则捕获
来源：http://zj.colortex.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://gz.huixiangedu.cn

[T48] Perl：正则替换
来源：http://bp.muxihuayi.cn

$s =~ s/old/new/g;
来源：http://xq.huanxung.cn

[T49] Perl：函数
来源：http://lg.yuexingan06.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lh.chemitech.net.cn

[T50] Perl：逐行读文件
来源：http://bg.bjjhwx.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://vn.shxzskj.cn

while (my $line = <$fh>) { print $line; }
来源：http://oo.nicolike.cn

[T51] Scala：Hello World
来源：http://ji.shxzukj.cn

println("Hello")
来源：http://jt.muxihuayi.cn

[T52] Scala：变量
来源：http://oa.huixinmuqiang.cn

val a = 1;  var b = 2
来源：http://rd.panjiajie.cn

[T53] Scala：字符串插值
来源：http://nk.huanxung.cn

s"值: $b"
来源：http://uq.521024.cn

[T54] Scala：集合映射
来源：http://nv.shxzskj.cn

List(1, 2, 3).map(_ * 2)
来源：http://ej.hahajie.cn

[T55] Scala：集合过滤
来源：http://eq.muxihuayi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://vz.jctech888.com.cn

[T56] Scala：样例类
来源：http://ob.bookmarksfly.cn

case class User(name: String, age: Int)
来源：http://lg.wgjwhj.cn

[T57] Scala：模式匹配
来源：http://cs.muxihuayi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://hv.shxzskj.cn

[T58] Scala：函数定义
来源：http://ds.asd995.cn

def add(a: Int, b: Int): Int = a + b
来源：http://yr.panjiajie.cn

[T59] Scala：循环
来源：http://ui.yuexingan06.cn

for (i <- 1 to 10) println(i)
来源：http://jx.nicolike.cn

[T60] Scala：折叠
来源：http://jq.yuexingan06.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://aq.lnxyls.cn

================================================================================
来源：http://re.shtwfgs.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lj.panjiajie.cn

================================================================================
来源：http://hx.lnxyls.cn

[U01] Py：创建虚拟环境
来源：http://ge.bjjhwx.cn

python -m venv .venv && source .venv/bin/activate
来源：http://la.hahajie.cn

[U02] Py：导出 / 安装依赖
来源：http://uu.szsharing.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gm.shxzskj.cn

[U03] Py：加载 .env 配置
来源：http://rm.bookmarksfly.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://hq.szsharing.cn

[U04] Py：变量调试打印
来源：http://fq.hahajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://de.lnxyls.cn

[U05] Py：列表去重且保序
来源：http://qq.jctech888.com.cn

list(dict.fromkeys(arr))
来源：http://zp.muxihuayi.cn

[U06] Py：合并两个字典
来源：http://zc.nicolike.cn

{**a, **b}
来源：http://ls.shxzukj.cn

[U07] Py：反转字典键值
来源：http://im.shtwfgs.cn

{v: k for k, v in d.items()}
来源：http://qx.jctech888.com.cn

[U08] Py：展平二维列表
来源：http://ib.shtwfgs.cn

[y for x in nested for y in x]
来源：http://qn.bookmarksfly.cn

[U09] Py：字典取最大值的键
来源：http://ac.asd995.cn

max(d, key=d.get)
来源：http://yx.jianghongdianzi.cn

[U10] Py：按值排序字典
来源：http://rw.521024.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://je.shtwfgs.cn

[U11] Py：生成器表达式
来源：http://kp.hnjuh.cn

(x * 2 for x in arr)
来源：http://ik.huanxung.cn

[U12] Py：取出现最多的 3 个元素
来源：http://wl.asd995.cn

Counter(arr).most_common(3)
来源：http://ef.shxzukj.cn

[U13] Py：固定长度队列
来源：http://lp.huanxung.cn

deque(maxlen=10)
来源：http://bh.hahajie.cn

[U14] Py：分组收集到列表
来源：http://ij.asd995.cn

defaultdict(list)
来源：http://no.shxzukj.cn

[U15] Py：高精度计时
来源：http://au.szsharing.cn

t = time.perf_counter()
来源：http://eu.bookmarksfly.cn

[U16] Py：命令行参数解析
来源：http://iq.bjjhwx.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://uv.haigaiapp.cn

[U17] Py：初始化日志
来源：http://wz.9csxet.cn

logging.basicConfig(level=logging.INFO)
来源：http://xu.wgjwhj.cn

[U18] Py：预编译正则
来源：http://rm.muxihuayi.cn

pat = re.compile(r"\d+")
来源：http://lj.shxzukj.cn

[U19] Py：正则替换带回调
来源：http://as.lnxyls.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ue.521024.cn

[U20] Py：缓存函数结果
来源：http://ip.asd995.cn

@functools.lru_cache(maxsize=None)
来源：http://rt.panjiajie.cn

[U21] Py：自定义上下文管理器
来源：http://ug.lnxyls.cn

@contextlib.contextmanager
来源：http://qh.shxzukj.cn

[U22] Py：矩阵转置
来源：http://ap.nszjky.cn

list(zip(*m))
来源：http://mz.jctech888.com.cn

[U23] Py：分块读取大文件
来源：http://dj.szsharing.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mk.shxzskj.cn

[U24] Py：路径操作
来源：http://dk.hnjuh.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://my.shxzskj.cn

[U25] Py：CSV 按字典读
来源：http://ue.bookmarksfly.cn

csv.DictReader(f)
来源：http://ra.9csxet.cn

[U26] Py：并发下载
来源：http://lq.yuexingan06.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ta.jianghongdianzi.cn

[U27] Py：异步 HTTP
来源：http://op.gzmigu.cn

aiohttp.ClientSession() 配合 async with
来源：http://iy.colortex.cn

[U28] Py：类型别名
来源：http://ur.huixiangedu.cn

UserId = int
来源：http://ym.szxytkj.cn

[U29] Py：属性校验
来源：http://tz.chemitech.net.cn

@property 与 @x.setter 配合
来源：http://vz.asd995.cn

[U30] Py：数据类
来源：http://jf.huixinmuqiang.cn

@dataclass(slots=True)
来源：http://ts.nicolike.cn

[U31] Py：单测
来源：http://kc.szsharing.cn

python -m pytest -q
来源：http://hg.yuexingan06.cn

[U32] Py：代码格式化
来源：http://vu.huanxung.cn

ruff format . && ruff check --fix .
来源：http://ov.haigaiapp.cn

[U33] Py：打包发布
来源：http://zd.jianghongdianzi.cn

python -m build  （依赖 pyproject.toml）
来源：http://sn.jianghongdianzi.cn

[U34] Py：判断编码
来源：http://ip.521024.cn

chardet.detect(raw)
来源：http://zj.lnxyls.cn

[U35] Py：发送邮件
来源：http://lt.colortex.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ha.wgjwhj.cn

[U36] Py：定时任务
来源：http://im.yuntaijiaju.cn

schedule.every(10).minutes.do(job)
来源：http://pi.hnjuh.cn

[U37] Py：读写 Excel
来源：http://ld.shtwfgs.cn

pandas.read_excel / DataFrame.to_excel
来源：http://kh.jianghongdianzi.cn

[U38] Py：获取脚本所在目录
来源：http://pe.asd995.cn

Path(__file__).resolve().parent
来源：http://zn.asd995.cn

[U39] Py：判断是否在交互环境
来源：http://hy.wgjwhj.cn

sys.stdout.isatty()
来源：http://ra.chemitech.net.cn

[U40] Py：打印到标准错误
来源：http://uk.colortex.cn

print("err", file=sys.stderr)
来源：http://ew.huixiangedu.cn

[U41] PHP：初始化 Composer 项目
来源：http://ku.szxytkj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://sy.jianghongdianzi.cn

[U42] PHP：PSR-4 自动加载
来源：http://fe.shxzukj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kz.yuexingan06.cn

[U43] PHP：声明命名空间
来源：http://cm.panjiajie.cn

namespace App\Http;
来源：http://mh.shxzskj.cn

[U44] PHP：开启严格类型
来源：http://kc.bjjhwx.cn

declare(strict_types=1);
来源：http://ux.jianghongdianzi.cn

[U45] PHP：类型声明与返回类型
来源：http://et.521024.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://tr.hahajie.cn

[U46] PHP：可空类型
来源：http://ju.haigaiapp.cn

?string $name = null
来源：http://vs.shxzukj.cn

[U47] PHP：联合类型
来源：http://it.gzmigu.cn

int|string $id
来源：http://nt.asd995.cn

[U48] PHP：纯枚举
来源：http://fx.gzmigu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zn.asd995.cn

[U49] PHP：只读属性
来源：http://qp.huixiangedu.cn

public readonly string $name
来源：http://iw.9csxet.cn

[U50] PHP：构造器属性提升
来源：http://yn.nszjky.cn

public function __construct(private int $id) {}
来源：http://yi.chemitech.net.cn

[U51] PHP：数组解构
来源：http://ff.wgjwhj.cn

[$a, $b] = $arr;
来源：http://em.bjjhwx.cn

[U52] PHP：箭头函数
来源：http://ho.yuntaijiaju.cn

$double = fn($x) => $x * 2;
来源：http://vt.huixinmuqiang.cn

[U53] PHP：空合并运算符
来源：http://uf.yuexingan06.cn

$v = $a ?? $b ?? "default";
来源：http://ft.bjjhwx.cn

[U54] PHP：空安全调用
来源：http://vk.muxihuayi.cn

$obj?->method()
来源：http://hs.yuexingan06.cn

[U55] PHP：match 表达式
来源：http://is.szsharing.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vu.9csxet.cn

[U56] PHP：命名参数
来源：http://vw.panjiajie.cn

f(a: 1, b: 2)
来源：http://da.9csxet.cn

[U57] PHP：字符串插值
来源：http://at.muxihuayi.cn

"值: {$a}"
来源：http://dp.lnxyls.cn

[U58] PHP：数组三件套
来源：http://yd.hnjuh.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fp.huanxung.cn

[U59] PHP：自定义排序
来源：http://vy.panjiajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ut.muxihuayi.cn

[U60] PHP：JSON 编解码
来源：http://qh.asd995.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ew.9csxet.cn

[U61] PHP：正则
来源：http://ya.jianghongdianzi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ix.shtwfgs.cn

[U62] PHP：日期对象
来源：http://nl.hahajie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lz.asd995.cn

[U63] PHP：文件读写
来源：http://kx.szsharing.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fw.colortex.cn

[U64] PHP：目录遍历
来源：http://xh.huanxung.cn

glob("dir/*.php");  scandir("dir");
来源：http://ti.newstarts.cn

[U65] PHP：会话
来源：http://xf.huixinmuqiang.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ot.yuntaijiaju.cn

[U66] PHP：设置 Cookie
来源：http://gp.jctech888.com.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zq.shtwfgs.cn

[U67] PHP：处理文件上传
来源：http://dw.nszjky.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://in.asd995.cn

[U68] PHP：PDO 连接
来源：http://ee.yuexingan06.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dh.shxzukj.cn

[U69] PHP：PDO 预处理
来源：http://fm.9csxet.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://uc.jianghongdianzi.cn

[U70] PHP：PDO 事务
来源：http://bw.newstarts.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cf.lnxyls.cn

[U71] PHP：抛出异常
来源：http://rm.gzmigu.cn

throw new RuntimeException("失败", 500);
来源：http://eq.huixinmuqiang.cn

[U72] PHP：写错误日志
来源：http://uj.huixinmuqiang.cn

error_log("失败: " . $e->getMessage());
来源：http://hn.bookmarksfly.cn

[U73] PHP：读取 ini 配置
来源：http://ug.szsharing.cn

parse_ini_file("config.ini", true)
来源：http://hs.asd995.cn

[U74] PHP：读取环境变量
来源：http://ht.bookmarksfly.cn

getenv("APP_ENV") ?: "production"
来源：http://qu.nszjky.cn

[U75] PHP：依赖注入
来源：http://iv.yuexingan06.cn

composer require psr/container
来源：http://dk.szsharing.cn

[U76] PHP：简单路由
来源：http://gk.9csxet.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nh.yuntaijiaju.cn

[U77] PHP：模板渲染
来源：http://qm.jianghongdianzi.cn

composer require twig/twig
来源：http://xz.gzmigu.cn

[U78] PHP：单元测试
来源：http://vz.szsharing.cn

composer require --dev phpunit/phpunit
来源：http://ew.yuexingan06.cn

[U79] PHP：静态分析
来源：http://pf.9csxet.cn

composer require --dev phpstan/phpstan
来源：http://cl.jianghongdianzi.cn

[U80] PHP：代码规范修复
来源：http://um.szsharing.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://nt.nszjky.cn

[U81] JS：初始化项目
来源：http://iv.muxihuayi.cn

npm init -y;  npm i express
来源：http://us.jctech888.com.cn

[U82] JS：package.json 脚本
来源：http://xq.newstarts.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ak.asd995.cn

[U83] JS：ES Module 导入导出
来源：http://ss.9csxet.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ce.shtwfgs.cn

[U84] JS：CommonJS 写法
来源：http://pz.szsharing.cn

module.exports = { a };  const { a } = require("./m");
来源：http://yp.szxytkj.cn

[U85] JS：可选链
来源：http://ih.asd995.cn

a?.b?.c
来源：http://am.bookmarksfly.cn

[U86] JS：空值合并
来源：http://av.shxzskj.cn

a ?? b
来源：http://ux.szxytkj.cn

[U87] JS：解构默认值
来源：http://mc.newstarts.cn

const { a = 1, b = 2 } = obj;
来源：http://df.muxihuayi.cn

[U88] JS：对象展开合并
来源：http://cy.jctech888.com.cn

{ ...a, ...b }
来源：http://pv.wgjwhj.cn

[U89] JS：数组去重
来源：http://vc.szsharing.cn

[...new Set(arr)]
来源：http://dn.shxzukj.cn

[U90] JS：数字数组排序
来源：http://rj.szxytkj.cn

[...arr].sort((a, b) => a - b)
来源：http://sd.hahajie.cn

[U91] JS：对象键值遍历
来源：http://tj.chemitech.net.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://oq.huixiangedu.cn

[U92] JS：深拷贝
来源：http://iq.nszjky.cn

structuredClone(obj)
来源：http://iu.szxytkj.cn

[U93] JS：模板字符串
来源：http://fz.yuexingan06.cn

`共 ${n} 条`
来源：http://bf.jianghongdianzi.cn

[U94] JS：箭头函数
来源：http://gg.hahajie.cn

const double = x => x * 2;
来源：http://bs.9csxet.cn

[U95] JS：Promise 包装
来源：http://st.yuexingan06.cn

new Promise((resolve, reject) => {})
来源：http://xi.lnxyls.cn

[U96] JS：async/await 与异常
来源：http://nx.yuexingan06.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mm.hnjuh.cn

[U97] JS：并发请求
来源：http://tz.9csxet.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://gi.newstarts.cn

[U98] JS：fetch 带 JSON
来源：http://qe.huixinmuqiang.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xe.nicolike.cn

[U99] JS：事件监听
来源：http://lx.szsharing.cn

el.addEventListener("click", e => {})
来源：http://fp.yuntaijiaju.cn

[U100] JS：DOM 查询
来源：http://vw.szsharing.cn

document.querySelector(".item")
来源：http://ze.jctech888.com.cn

[U101] JS：classList 操作
来源：http://gx.chemitech.net.cn

el.classList.toggle("active")
来源：http://qs.bjjhwx.cn

[U102] JS：本地存储
来源：http://if.panjiajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://mv.asd995.cn

[U103] JS：定时器
来源：http://ep.wgjwhj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ee.shtwfgs.cn

[U104] JS：防抖
来源：http://vx.hahajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://en.szsharing.cn

[U105] JS：节流
来源：http://dx.jianghongdianzi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nu.huixiangedu.cn

[U106] JS：日期格式化
来源：http://bt.yuntaijiaju.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qq.szxytkj.cn

[U107] JS：数字千分位
来源：http://dy.jctech888.com.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wp.gzmigu.cn

[U108] JS：随机整数
来源：http://qv.chemitech.net.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cm.szxytkj.cn

[U109] JS：数组分组
来源：http://dq.szxytkj.cn

Object.groupBy(arr, x => x.type)
来源：http://iu.bjjhwx.cn

[U110] JS：数组分块
来源：http://ja.hahajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zz.shxzukj.cn

[U111] JS：对象转 Map
来源：http://ls.haigaiapp.cn

new Map(Object.entries(obj))
来源：http://xx.bjjhwx.cn

[U112] JS：字符串补位
来源：http://rq.shxzskj.cn

"7".padStart(3, "0")
来源：http://ts.yuntaijiaju.cn

[U113] JS：正则替换全部
来源：http://ts.9csxet.cn

s.replaceAll("a", "b")
来源：http://jd.jianghongdianzi.cn

[U114] JS：JSON 深比较
来源：http://rf.muxihuayi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://uh.asd995.cn

[U115] JS：生成 UUID
来源：http://ad.huixiangedu.cn

crypto.randomUUID()
来源：http://ws.hahajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://tz.shxzukj.cn

/** @param {string} name */ function f(name) {}
来源：http://bt.jianghongdianzi.cn

[U117] JS：单元测试
来源：http://se.asd995.cn

npm i -D vitest;  npx vitest
来源：http://jv.colortex.cn

[U118] JS：开发服务器
来源：http://hu.shxzskj.cn

npm i -D vite;  npx vite
来源：http://oi.huixinmuqiang.cn

[U119] JS：生产构建
来源：http://yb.nszjky.cn

npx vite build
来源：http://zx.muxihuayi.cn

[U120] JS：读取环境变量（Vite）
来源：http://mb.bjjhwx.cn

import.meta.env.VITE_API_URL
来源：http://if.shxzskj.cn

================================================================================
来源：http://ik.huixiangedu.cn

统计汇总
来源：http://wb.huanxung.cn

================================================================================
来源：http://eo.colortex.cn

按语言统计（条）：
来源：http://co.shxzskj.cn

Python ......... 252
来源：http://fg.panjiajie.cn

PHP ............ 252
来源：http://uy.szsharing.cn

JavaScript ..... 252
来源：http://pk.nicolike.cn

TypeScript ..... 212
来源：http://xo.shxzukj.cn

Java ........... 212
来源：http://xh.colortex.cn

Go ............. 212
来源：http://to.gzmigu.cn

Ruby ........... 212
来源：http://vs.521024.cn

C# ............. 212
来源：http://yf.muxihuayi.cn


<!-- 参考信息 -->