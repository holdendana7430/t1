代发 wailian999

[T37] Lua：字符串拼接
来源：http://lp.chemitech.net.cn

"a" .. "b"
来源：http://ci.wgjwhj.cn

[T38] Lua：条件
来源：http://lc.huixiangedu.cn

if x > 0 then print("正") end
来源：http://wx.newstarts.cn

[T39] Lua：模式匹配
来源：http://tm.haigaiapp.cn

string.find(s, "%d+")
来源：http://kw.bjjhwx.cn

[T40] Lua：元表
来源：http://zf.lnxyls.cn

setmetatable({}, { __index = base })
来源：http://al.shtwfgs.cn

[T41] Perl：Hello World
来源：http://ou.jctech888.com.cn

print "Hello\n";
来源：http://yi.wgjwhj.cn

[T42] Perl：变量类型
来源：http://sh.shtwfgs.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://od.huanxung.cn

[T43] Perl：字符串插值
来源：http://ld.colortex.cn

"值: $a"
来源：http://gp.colortex.cn

[T44] Perl：条件
来源：http://cp.lnxyls.cn

if ($a > 0) { print "正"; }
来源：http://ry.lnxyls.cn

[T45] Perl：数组遍历
来源：http://uu.shxzukj.cn

for my $x (@arr) { print $x; }
来源：http://ab.jianghongdianzi.cn

[T46] Perl：哈希操作
来源：http://gz.yuntaijiaju.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sd.hahajie.cn

[T47] Perl：正则捕获
来源：http://ko.shtwfgs.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qr.huanxung.cn

[T48] Perl：正则替换
来源：http://ei.hnjuh.cn

$s =~ s/old/new/g;
来源：http://wy.hnjuh.cn

[T49] Perl：函数
来源：http://yt.shxzukj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://va.shxzukj.cn

[T50] Perl：逐行读文件
来源：http://tl.jctech888.com.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xv.hnjuh.cn

while (my $line = <$fh>) { print $line; }
来源：http://wl.shxzukj.cn

[T51] Scala：Hello World
来源：http://pl.bjjhwx.cn

println("Hello")
来源：http://jv.gzmigu.cn

[T52] Scala：变量
来源：http://zo.521024.cn

val a = 1;  var b = 2
来源：http://ga.jctech888.com.cn

[T53] Scala：字符串插值
来源：http://np.asd995.cn

s"值: $b"
来源：http://ho.jctech888.com.cn

[T54] Scala：集合映射
来源：http://fe.nszjky.cn

List(1, 2, 3).map(_ * 2)
来源：http://jg.hnjuh.cn

[T55] Scala：集合过滤
来源：http://ld.szsharing.cn

List(1, 2, 3).filter(_ > 1)
来源：http://nd.521024.cn

[T56] Scala：样例类
来源：http://lk.szsharing.cn

case class User(name: String, age: Int)
来源：http://hm.szsharing.cn

[T57] Scala：模式匹配
来源：http://fw.asd995.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gn.nszjky.cn

[T58] Scala：函数定义
来源：http://zn.haigaiapp.cn

def add(a: Int, b: Int): Int = a + b
来源：http://jx.panjiajie.cn

[T59] Scala：循环
来源：http://mh.gzmigu.cn

for (i <- 1 to 10) println(i)
来源：http://ft.jianghongdianzi.cn

[T60] Scala：折叠
来源：http://rk.9csxet.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hj.asd995.cn

================================================================================
来源：http://tu.huanxung.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bp.shtwfgs.cn

================================================================================
来源：http://pk.521024.cn

[U01] Py：创建虚拟环境
来源：http://cm.hnjuh.cn

python -m venv .venv && source .venv/bin/activate
来源：http://yk.haigaiapp.cn

[U02] Py：导出 / 安装依赖
来源：http://vb.521024.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bx.bookmarksfly.cn

[U03] Py：加载 .env 配置
来源：http://al.szsharing.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://hu.gzmigu.cn

[U04] Py：变量调试打印
来源：http://an.hnjuh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ff.shtwfgs.cn

[U05] Py：列表去重且保序
来源：http://cc.panjiajie.cn

list(dict.fromkeys(arr))
来源：http://dv.bjjhwx.cn

[U06] Py：合并两个字典
来源：http://ax.9csxet.cn

{**a, **b}
来源：http://jt.9csxet.cn

[U07] Py：反转字典键值
来源：http://hj.jianghongdianzi.cn

{v: k for k, v in d.items()}
来源：http://iz.huanxung.cn

[U08] Py：展平二维列表
来源：http://qr.nszjky.cn

[y for x in nested for y in x]
来源：http://uy.shxzskj.cn

[U09] Py：字典取最大值的键
来源：http://ns.asd995.cn

max(d, key=d.get)
来源：http://rh.yuexingan06.cn

[U10] Py：按值排序字典
来源：http://jg.chemitech.net.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wf.yuexingan06.cn

[U11] Py：生成器表达式
来源：http://vf.newstarts.cn

(x * 2 for x in arr)
来源：http://rk.huixinmuqiang.cn

[U12] Py：取出现最多的 3 个元素
来源：http://vy.huixinmuqiang.cn

Counter(arr).most_common(3)
来源：http://bw.gzmigu.cn

[U13] Py：固定长度队列
来源：http://ll.muxihuayi.cn

deque(maxlen=10)
来源：http://up.yuexingan06.cn

[U14] Py：分组收集到列表
来源：http://zk.huixiangedu.cn

defaultdict(list)
来源：http://gq.shxzskj.cn

[U15] Py：高精度计时
来源：http://yj.szxytkj.cn

t = time.perf_counter()
来源：http://zh.huixiangedu.cn

[U16] Py：命令行参数解析
来源：http://wa.szsharing.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zf.asd995.cn

[U17] Py：初始化日志
来源：http://za.gzmigu.cn

logging.basicConfig(level=logging.INFO)
来源：http://vz.lnxyls.cn

[U18] Py：预编译正则
来源：http://wt.9csxet.cn

pat = re.compile(r"\d+")
来源：http://fg.muxihuayi.cn

[U19] Py：正则替换带回调
来源：http://if.bookmarksfly.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lr.521024.cn

[U20] Py：缓存函数结果
来源：http://ni.muxihuayi.cn

@functools.lru_cache(maxsize=None)
来源：http://ao.panjiajie.cn

[U21] Py：自定义上下文管理器
来源：http://iu.chemitech.net.cn

@contextlib.contextmanager
来源：http://ep.9csxet.cn

[U22] Py：矩阵转置
来源：http://bk.9csxet.cn

list(zip(*m))
来源：http://ya.lnxyls.cn

[U23] Py：分块读取大文件
来源：http://wq.muxihuayi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jy.jctech888.com.cn

[U24] Py：路径操作
来源：http://wy.shtwfgs.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bg.wgjwhj.cn

[U25] Py：CSV 按字典读
来源：http://nr.yuntaijiaju.cn

csv.DictReader(f)
来源：http://xi.shtwfgs.cn

[U26] Py：并发下载
来源：http://in.9csxet.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pc.nszjky.cn

[U27] Py：异步 HTTP
来源：http://if.newstarts.cn

aiohttp.ClientSession() 配合 async with
来源：http://rs.hnjuh.cn

[U28] Py：类型别名
来源：http://qi.colortex.cn

UserId = int
来源：http://wt.huixinmuqiang.cn

[U29] Py：属性校验
来源：http://qe.szxytkj.cn

@property 与 @x.setter 配合
来源：http://by.szsharing.cn

[U30] Py：数据类
来源：http://bt.yuexingan06.cn

@dataclass(slots=True)
来源：http://vd.chemitech.net.cn

[U31] Py：单测
来源：http://ew.colortex.cn

python -m pytest -q
来源：http://ze.colortex.cn

[U32] Py：代码格式化
来源：http://to.asd995.cn

ruff format . && ruff check --fix .
来源：http://fc.muxihuayi.cn

[U33] Py：打包发布
来源：http://be.shxzskj.cn

python -m build  （依赖 pyproject.toml）
来源：http://aj.bjjhwx.cn

[U34] Py：判断编码
来源：http://rw.jctech888.com.cn

chardet.detect(raw)
来源：http://lq.haigaiapp.cn

[U35] Py：发送邮件
来源：http://wa.panjiajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dn.bookmarksfly.cn

[U36] Py：定时任务
来源：http://cx.lnxyls.cn

schedule.every(10).minutes.do(job)
来源：http://gx.shtwfgs.cn

[U37] Py：读写 Excel
来源：http://ci.shtwfgs.cn

pandas.read_excel / DataFrame.to_excel
来源：http://li.nicolike.cn

[U38] Py：获取脚本所在目录
来源：http://zd.haigaiapp.cn

Path(__file__).resolve().parent
来源：http://dh.szxytkj.cn

[U39] Py：判断是否在交互环境
来源：http://gd.yuexingan06.cn

sys.stdout.isatty()
来源：http://id.shxzukj.cn

[U40] Py：打印到标准错误
来源：http://tp.bjjhwx.cn

print("err", file=sys.stderr)
来源：http://cq.szsharing.cn

[U41] PHP：初始化 Composer 项目
来源：http://ww.9csxet.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xk.panjiajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://mx.muxihuayi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qp.nicolike.cn

[U43] PHP：声明命名空间
来源：http://bk.hahajie.cn

namespace App\Http;
来源：http://zc.hnjuh.cn

[U44] PHP：开启严格类型
来源：http://mf.shtwfgs.cn

declare(strict_types=1);
来源：http://ll.huanxung.cn

[U45] PHP：类型声明与返回类型
来源：http://lp.jianghongdianzi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://pa.gzmigu.cn

[U46] PHP：可空类型
来源：http://rb.521024.cn

?string $name = null
来源：http://qk.panjiajie.cn

[U47] PHP：联合类型
来源：http://dr.shtwfgs.cn

int|string $id
来源：http://cb.hahajie.cn

[U48] PHP：纯枚举
来源：http://ga.nszjky.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nn.shxzukj.cn

[U49] PHP：只读属性
来源：http://ch.lnxyls.cn

public readonly string $name
来源：http://wh.jctech888.com.cn

[U50] PHP：构造器属性提升
来源：http://cn.panjiajie.cn

public function __construct(private int $id) {}
来源：http://pf.chemitech.net.cn

[U51] PHP：数组解构
来源：http://xr.wgjwhj.cn

[$a, $b] = $arr;
来源：http://us.shxzukj.cn

[U52] PHP：箭头函数
来源：http://ua.nicolike.cn

$double = fn($x) => $x * 2;
来源：http://ag.521024.cn

[U53] PHP：空合并运算符
来源：http://dc.newstarts.cn

$v = $a ?? $b ?? "default";
来源：http://gn.asd995.cn

[U54] PHP：空安全调用
来源：http://ea.bookmarksfly.cn

$obj?->method()
来源：http://mv.huixiangedu.cn

[U55] PHP：match 表达式
来源：http://hk.panjiajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zo.521024.cn

[U56] PHP：命名参数
来源：http://of.szsharing.cn

f(a: 1, b: 2)
来源：http://xn.nicolike.cn

[U57] PHP：字符串插值
来源：http://gy.huanxung.cn

"值: {$a}"
来源：http://az.wgjwhj.cn

[U58] PHP：数组三件套
来源：http://rg.lnxyls.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zx.nicolike.cn

[U59] PHP：自定义排序
来源：http://pd.newstarts.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oc.shtwfgs.cn

[U60] PHP：JSON 编解码
来源：http://ra.jianghongdianzi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ae.gzmigu.cn

[U61] PHP：正则
来源：http://yw.huixinmuqiang.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nw.panjiajie.cn

[U62] PHP：日期对象
来源：http://ez.hahajie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wl.gzmigu.cn

[U63] PHP：文件读写
来源：http://mk.hnjuh.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wz.panjiajie.cn

[U64] PHP：目录遍历
来源：http://vi.huixinmuqiang.cn

glob("dir/*.php");  scandir("dir");
来源：http://th.panjiajie.cn

[U65] PHP：会话
来源：http://da.shxzukj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://lk.szsharing.cn

[U66] PHP：设置 Cookie
来源：http://hq.hnjuh.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mr.lnxyls.cn

[U67] PHP：处理文件上传
来源：http://io.yuexingan06.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dh.newstarts.cn

[U68] PHP：PDO 连接
来源：http://au.jianghongdianzi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wm.gzmigu.cn

[U69] PHP：PDO 预处理
来源：http://ou.colortex.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gz.bjjhwx.cn

[U70] PHP：PDO 事务
来源：http://oc.bookmarksfly.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ym.hahajie.cn

[U71] PHP：抛出异常
来源：http://su.szxytkj.cn

throw new RuntimeException("失败", 500);
来源：http://vf.yuexingan06.cn

[U72] PHP：写错误日志
来源：http://vf.chemitech.net.cn

error_log("失败: " . $e->getMessage());
来源：http://qa.szxytkj.cn

[U73] PHP：读取 ini 配置
来源：http://sn.shxzukj.cn

parse_ini_file("config.ini", true)
来源：http://jp.gzmigu.cn

[U74] PHP：读取环境变量
来源：http://jp.9csxet.cn

getenv("APP_ENV") ?: "production"
来源：http://he.huixiangedu.cn

[U75] PHP：依赖注入
来源：http://jx.nicolike.cn

composer require psr/container
来源：http://lr.huixinmuqiang.cn

[U76] PHP：简单路由
来源：http://gf.shtwfgs.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://aq.nicolike.cn

[U77] PHP：模板渲染
来源：http://ga.muxihuayi.cn

composer require twig/twig
来源：http://ij.hnjuh.cn

[U78] PHP：单元测试
来源：http://wt.bjjhwx.cn

composer require --dev phpunit/phpunit
来源：http://bc.jctech888.com.cn

[U79] PHP：静态分析
来源：http://xi.yuntaijiaju.cn

composer require --dev phpstan/phpstan
来源：http://sw.szxytkj.cn

[U80] PHP：代码规范修复
来源：http://ud.nicolike.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://pj.huixiangedu.cn

[U81] JS：初始化项目
来源：http://bm.shxzskj.cn

npm init -y;  npm i express
来源：http://ov.gzmigu.cn

[U82] JS：package.json 脚本
来源：http://xu.shxzukj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xq.jctech888.com.cn

[U83] JS：ES Module 导入导出
来源：http://kr.szxytkj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://bt.521024.cn

[U84] JS：CommonJS 写法
来源：http://ae.shtwfgs.cn

module.exports = { a };  const { a } = require("./m");
来源：http://oe.shtwfgs.cn

[U85] JS：可选链
来源：http://pa.nszjky.cn

a?.b?.c
来源：http://qw.wgjwhj.cn

[U86] JS：空值合并
来源：http://cv.huixinmuqiang.cn

a ?? b
来源：http://gm.hnjuh.cn

[U87] JS：解构默认值
来源：http://jp.shxzukj.cn

const { a = 1, b = 2 } = obj;
来源：http://wy.yuntaijiaju.cn

[U88] JS：对象展开合并
来源：http://hp.colortex.cn

{ ...a, ...b }
来源：http://ub.haigaiapp.cn

[U89] JS：数组去重
来源：http://iz.newstarts.cn

[...new Set(arr)]
来源：http://tr.shtwfgs.cn

[U90] JS：数字数组排序
来源：http://tz.hnjuh.cn

[...arr].sort((a, b) => a - b)
来源：http://re.shxzskj.cn

[U91] JS：对象键值遍历
来源：http://vd.nicolike.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yg.szsharing.cn

[U92] JS：深拷贝
来源：http://dh.jctech888.com.cn

structuredClone(obj)
来源：http://yu.yuntaijiaju.cn

[U93] JS：模板字符串
来源：http://uv.nszjky.cn

`共 ${n} 条`
来源：http://jg.newstarts.cn

[U94] JS：箭头函数
来源：http://sp.shtwfgs.cn

const double = x => x * 2;
来源：http://xw.szxytkj.cn

[U95] JS：Promise 包装
来源：http://hu.yuntaijiaju.cn

new Promise((resolve, reject) => {})
来源：http://rd.huanxung.cn

[U96] JS：async/await 与异常
来源：http://kl.huanxung.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hq.lnxyls.cn

[U97] JS：并发请求
来源：http://wm.nszjky.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://se.hnjuh.cn

[U98] JS：fetch 带 JSON
来源：http://dd.wgjwhj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ls.huixinmuqiang.cn

[U99] JS：事件监听
来源：http://lf.yuntaijiaju.cn

el.addEventListener("click", e => {})
来源：http://vg.asd995.cn

[U100] JS：DOM 查询
来源：http://hy.huixiangedu.cn

document.querySelector(".item")
来源：http://xq.huixiangedu.cn

[U101] JS：classList 操作
来源：http://gc.hnjuh.cn

el.classList.toggle("active")
来源：http://cl.shtwfgs.cn

[U102] JS：本地存储
来源：http://tv.huixinmuqiang.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://qf.huanxung.cn

[U103] JS：定时器
来源：http://ra.jianghongdianzi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://za.jianghongdianzi.cn

[U104] JS：防抖
来源：http://wi.shxzukj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bu.panjiajie.cn

[U105] JS：节流
来源：http://il.asd995.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zv.huixiangedu.cn

[U106] JS：日期格式化
来源：http://sq.yuntaijiaju.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fo.shxzukj.cn

[U107] JS：数字千分位
来源：http://sh.szsharing.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bh.bookmarksfly.cn

[U108] JS：随机整数
来源：http://xm.yuntaijiaju.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://px.hnjuh.cn

[U109] JS：数组分组
来源：http://gn.huanxung.cn

Object.groupBy(arr, x => x.type)
来源：http://yt.hahajie.cn

[U110] JS：数组分块
来源：http://jt.haigaiapp.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lr.nszjky.cn

[U111] JS：对象转 Map
来源：http://nh.szsharing.cn

new Map(Object.entries(obj))
来源：http://zl.wgjwhj.cn

[U112] JS：字符串补位
来源：http://hi.haigaiapp.cn

"7".padStart(3, "0")
来源：http://ga.yuntaijiaju.cn

[U113] JS：正则替换全部
来源：http://az.panjiajie.cn

s.replaceAll("a", "b")
来源：http://tf.wgjwhj.cn

[U114] JS：JSON 深比较
来源：http://tj.hnjuh.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://aj.bookmarksfly.cn

[U115] JS：生成 UUID
来源：http://xz.gzmigu.cn

crypto.randomUUID()
来源：http://gd.panjiajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://ys.muxihuayi.cn

/** @param {string} name */ function f(name) {}
来源：http://qe.yuntaijiaju.cn

[U117] JS：单元测试
来源：http://bd.huanxung.cn

npm i -D vitest;  npx vitest
来源：http://oh.asd995.cn

[U118] JS：开发服务器
来源：http://rw.muxihuayi.cn

npm i -D vite;  npx vite
来源：http://zx.haigaiapp.cn

[U119] JS：生产构建
来源：http://mv.hahajie.cn

npx vite build
来源：http://qu.haigaiapp.cn

[U120] JS：读取环境变量（Vite）
来源：http://im.newstarts.cn

import.meta.env.VITE_API_URL
来源：http://of.huanxung.cn

================================================================================
来源：http://wv.nszjky.cn

统计汇总
来源：http://qz.jianghongdianzi.cn

================================================================================
来源：http://pt.muxihuayi.cn

按语言统计（条）：
来源：http://fw.wgjwhj.cn

Python ......... 252
来源：http://iy.jctech888.com.cn

PHP ............ 252
来源：http://wz.yuexingan06.cn

JavaScript ..... 252
来源：http://ru.gzmigu.cn

TypeScript ..... 212
来源：http://xx.bookmarksfly.cn


<!-- 参考信息 -->