代发 wailian999

[T39] Lua：模式匹配
来源：http://dn.gzmigu.cn

string.find(s, "%d+")
来源：http://kr.521024.cn

[T40] Lua：元表
来源：http://bh.huixinmuqiang.cn

setmetatable({}, { __index = base })
来源：http://ow.521024.cn

[T41] Perl：Hello World
来源：http://jw.haigaiapp.cn

print "Hello\n";
来源：http://qb.newstarts.cn

[T42] Perl：变量类型
来源：http://ci.nszjky.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ip.bookmarksfly.cn

[T43] Perl：字符串插值
来源：http://if.nicolike.cn

"值: $a"
来源：http://ge.chemitech.net.cn

[T44] Perl：条件
来源：http://yk.yuntaijiaju.cn

if ($a > 0) { print "正"; }
来源：http://ue.yuexingan06.cn

[T45] Perl：数组遍历
来源：http://rg.yuexingan06.cn

for my $x (@arr) { print $x; }
来源：http://tv.huixinmuqiang.cn

[T46] Perl：哈希操作
来源：http://qh.newstarts.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kf.hahajie.cn

[T47] Perl：正则捕获
来源：http://kv.jianghongdianzi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wi.szsharing.cn

[T48] Perl：正则替换
来源：http://kf.hahajie.cn

$s =~ s/old/new/g;
来源：http://cg.bjjhwx.cn

[T49] Perl：函数
来源：http://ac.colortex.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wy.panjiajie.cn

[T50] Perl：逐行读文件
来源：http://eg.shtwfgs.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://hj.huixiangedu.cn

while (my $line = <$fh>) { print $line; }
来源：http://ms.newstarts.cn

[T51] Scala：Hello World
来源：http://di.nszjky.cn

println("Hello")
来源：http://hj.nszjky.cn

[T52] Scala：变量
来源：http://aq.9csxet.cn

val a = 1;  var b = 2
来源：http://fk.szsharing.cn

[T53] Scala：字符串插值
来源：http://oi.521024.cn

s"值: $b"
来源：http://eq.521024.cn

[T54] Scala：集合映射
来源：http://pl.colortex.cn

List(1, 2, 3).map(_ * 2)
来源：http://gl.gzmigu.cn

[T55] Scala：集合过滤
来源：http://yd.nicolike.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ka.asd995.cn

[T56] Scala：样例类
来源：http://ra.shxzukj.cn

case class User(name: String, age: Int)
来源：http://rj.muxihuayi.cn

[T57] Scala：模式匹配
来源：http://va.jctech888.com.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://yz.nicolike.cn

[T58] Scala：函数定义
来源：http://eq.bookmarksfly.cn

def add(a: Int, b: Int): Int = a + b
来源：http://cn.shxzskj.cn

[T59] Scala：循环
来源：http://yq.yuexingan06.cn

for (i <- 1 to 10) println(i)
来源：http://iv.szxytkj.cn

[T60] Scala：折叠
来源：http://bx.muxihuayi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xk.521024.cn

================================================================================
来源：http://bd.huanxung.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hl.shxzskj.cn

================================================================================
来源：http://oa.muxihuayi.cn

[U01] Py：创建虚拟环境
来源：http://zw.nicolike.cn

python -m venv .venv && source .venv/bin/activate
来源：http://je.hnjuh.cn

[U02] Py：导出 / 安装依赖
来源：http://xw.shxzskj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dp.shxzskj.cn

[U03] Py：加载 .env 配置
来源：http://mo.chemitech.net.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ph.521024.cn

[U04] Py：变量调试打印
来源：http://cm.asd995.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dg.nszjky.cn

[U05] Py：列表去重且保序
来源：http://oo.asd995.cn

list(dict.fromkeys(arr))
来源：http://ht.nszjky.cn

[U06] Py：合并两个字典
来源：http://ss.lnxyls.cn

{**a, **b}
来源：http://mi.newstarts.cn

[U07] Py：反转字典键值
来源：http://ol.colortex.cn

{v: k for k, v in d.items()}
来源：http://lm.panjiajie.cn

[U08] Py：展平二维列表
来源：http://ph.szsharing.cn

[y for x in nested for y in x]
来源：http://gm.huixinmuqiang.cn

[U09] Py：字典取最大值的键
来源：http://us.huixinmuqiang.cn

max(d, key=d.get)
来源：http://wj.yuexingan06.cn

[U10] Py：按值排序字典
来源：http://kh.huixinmuqiang.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tz.haigaiapp.cn

[U11] Py：生成器表达式
来源：http://da.asd995.cn

(x * 2 for x in arr)
来源：http://cg.hahajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://jh.bjjhwx.cn

Counter(arr).most_common(3)
来源：http://pb.szxytkj.cn

[U13] Py：固定长度队列
来源：http://in.haigaiapp.cn

deque(maxlen=10)
来源：http://fl.hnjuh.cn

[U14] Py：分组收集到列表
来源：http://uq.shxzukj.cn

defaultdict(list)
来源：http://sw.shxzukj.cn

[U15] Py：高精度计时
来源：http://go.asd995.cn

t = time.perf_counter()
来源：http://aw.hahajie.cn

[U16] Py：命令行参数解析
来源：http://ym.jianghongdianzi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ya.nszjky.cn

[U17] Py：初始化日志
来源：http://vc.muxihuayi.cn

logging.basicConfig(level=logging.INFO)
来源：http://on.szxytkj.cn

[U18] Py：预编译正则
来源：http://xo.shxzskj.cn

pat = re.compile(r"\d+")
来源：http://zy.panjiajie.cn

[U19] Py：正则替换带回调
来源：http://da.bjjhwx.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qt.bjjhwx.cn

[U20] Py：缓存函数结果
来源：http://bv.haigaiapp.cn

@functools.lru_cache(maxsize=None)
来源：http://en.9csxet.cn

[U21] Py：自定义上下文管理器
来源：http://io.nszjky.cn

@contextlib.contextmanager
来源：http://lm.chemitech.net.cn

[U22] Py：矩阵转置
来源：http://xf.colortex.cn

list(zip(*m))
来源：http://qp.hnjuh.cn

[U23] Py：分块读取大文件
来源：http://vc.huanxung.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://su.colortex.cn

[U24] Py：路径操作
来源：http://so.colortex.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wn.wgjwhj.cn

[U25] Py：CSV 按字典读
来源：http://hl.yuexingan06.cn

csv.DictReader(f)
来源：http://rt.nicolike.cn

[U26] Py：并发下载
来源：http://uy.jianghongdianzi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wh.shxzskj.cn

[U27] Py：异步 HTTP
来源：http://ma.bjjhwx.cn

aiohttp.ClientSession() 配合 async with
来源：http://gy.szsharing.cn

[U28] Py：类型别名
来源：http://cl.gzmigu.cn

UserId = int
来源：http://qf.asd995.cn

[U29] Py：属性校验
来源：http://wx.chemitech.net.cn

@property 与 @x.setter 配合
来源：http://iz.szxytkj.cn

[U30] Py：数据类
来源：http://sh.huanxung.cn

@dataclass(slots=True)
来源：http://xe.bookmarksfly.cn

[U31] Py：单测
来源：http://os.szsharing.cn

python -m pytest -q
来源：http://nk.shxzskj.cn

[U32] Py：代码格式化
来源：http://er.jctech888.com.cn

ruff format . && ruff check --fix .
来源：http://rv.bjjhwx.cn

[U33] Py：打包发布
来源：http://ep.bjjhwx.cn

python -m build  （依赖 pyproject.toml）
来源：http://la.bjjhwx.cn

[U34] Py：判断编码
来源：http://jm.szxytkj.cn

chardet.detect(raw)
来源：http://qg.huixiangedu.cn

[U35] Py：发送邮件
来源：http://cd.nicolike.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fj.chemitech.net.cn

[U36] Py：定时任务
来源：http://nd.panjiajie.cn

schedule.every(10).minutes.do(job)
来源：http://rx.huixinmuqiang.cn

[U37] Py：读写 Excel
来源：http://pm.jianghongdianzi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://zb.shxzskj.cn

[U38] Py：获取脚本所在目录
来源：http://ld.shxzukj.cn

Path(__file__).resolve().parent
来源：http://we.newstarts.cn

[U39] Py：判断是否在交互环境
来源：http://zn.huanxung.cn

sys.stdout.isatty()
来源：http://mv.chemitech.net.cn

[U40] Py：打印到标准错误
来源：http://mu.9csxet.cn

print("err", file=sys.stderr)
来源：http://vr.chemitech.net.cn

[U41] PHP：初始化 Composer 项目
来源：http://mk.newstarts.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xq.gzmigu.cn

[U42] PHP：PSR-4 自动加载
来源：http://up.521024.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bp.huixiangedu.cn

[U43] PHP：声明命名空间
来源：http://je.bookmarksfly.cn

namespace App\Http;
来源：http://vx.nicolike.cn

[U44] PHP：开启严格类型
来源：http://cy.nicolike.cn

declare(strict_types=1);
来源：http://hr.huanxung.cn

[U45] PHP：类型声明与返回类型
来源：http://pz.lnxyls.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bc.chemitech.net.cn

[U46] PHP：可空类型
来源：http://lz.newstarts.cn

?string $name = null
来源：http://tw.jctech888.com.cn

[U47] PHP：联合类型
来源：http://hz.wgjwhj.cn

int|string $id
来源：http://ex.huanxung.cn

[U48] PHP：纯枚举
来源：http://uw.yuntaijiaju.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yf.panjiajie.cn

[U49] PHP：只读属性
来源：http://nt.lnxyls.cn

public readonly string $name
来源：http://hn.nicolike.cn

[U50] PHP：构造器属性提升
来源：http://xi.szxytkj.cn

public function __construct(private int $id) {}
来源：http://jw.huixiangedu.cn

[U51] PHP：数组解构
来源：http://pp.wgjwhj.cn

[$a, $b] = $arr;
来源：http://wl.gzmigu.cn

[U52] PHP：箭头函数
来源：http://dv.asd995.cn

$double = fn($x) => $x * 2;
来源：http://kj.huixiangedu.cn

[U53] PHP：空合并运算符
来源：http://sn.muxihuayi.cn

$v = $a ?? $b ?? "default";
来源：http://hk.bookmarksfly.cn

[U54] PHP：空安全调用
来源：http://ow.panjiajie.cn

$obj?->method()
来源：http://oc.521024.cn

[U55] PHP：match 表达式
来源：http://xy.9csxet.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fm.colortex.cn

[U56] PHP：命名参数
来源：http://ht.panjiajie.cn

f(a: 1, b: 2)
来源：http://nf.shxzskj.cn

[U57] PHP：字符串插值
来源：http://mg.shtwfgs.cn

"值: {$a}"
来源：http://kz.haigaiapp.cn

[U58] PHP：数组三件套
来源：http://il.9csxet.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://dx.wgjwhj.cn

[U59] PHP：自定义排序
来源：http://kn.colortex.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://km.newstarts.cn

[U60] PHP：JSON 编解码
来源：http://rg.newstarts.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hs.huixiangedu.cn

[U61] PHP：正则
来源：http://pb.jctech888.com.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tj.yuexingan06.cn

[U62] PHP：日期对象
来源：http://ya.hahajie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bm.nszjky.cn

[U63] PHP：文件读写
来源：http://xf.szsharing.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qj.shxzskj.cn

[U64] PHP：目录遍历
来源：http://dy.hahajie.cn

glob("dir/*.php");  scandir("dir");
来源：http://fh.yuexingan06.cn

[U65] PHP：会话
来源：http://yh.nicolike.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://pj.lnxyls.cn

[U66] PHP：设置 Cookie
来源：http://mm.hnjuh.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cm.bjjhwx.cn

[U67] PHP：处理文件上传
来源：http://zz.szsharing.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yz.jianghongdianzi.cn

[U68] PHP：PDO 连接
来源：http://dd.gzmigu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://do.hahajie.cn

[U69] PHP：PDO 预处理
来源：http://ex.hahajie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ry.9csxet.cn

[U70] PHP：PDO 事务
来源：http://nw.521024.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yj.haigaiapp.cn

[U71] PHP：抛出异常
来源：http://ko.lnxyls.cn

throw new RuntimeException("失败", 500);
来源：http://hi.panjiajie.cn

[U72] PHP：写错误日志
来源：http://or.newstarts.cn

error_log("失败: " . $e->getMessage());
来源：http://nn.wgjwhj.cn

[U73] PHP：读取 ini 配置
来源：http://zt.jianghongdianzi.cn

parse_ini_file("config.ini", true)
来源：http://ht.9csxet.cn

[U74] PHP：读取环境变量
来源：http://ws.huixiangedu.cn

getenv("APP_ENV") ?: "production"
来源：http://mv.newstarts.cn

[U75] PHP：依赖注入
来源：http://ei.nszjky.cn

composer require psr/container
来源：http://zf.huixinmuqiang.cn

[U76] PHP：简单路由
来源：http://di.huixinmuqiang.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fw.hnjuh.cn

[U77] PHP：模板渲染
来源：http://uw.colortex.cn

composer require twig/twig
来源：http://nh.muxihuayi.cn

[U78] PHP：单元测试
来源：http://gr.chemitech.net.cn

composer require --dev phpunit/phpunit
来源：http://rm.yuntaijiaju.cn

[U79] PHP：静态分析
来源：http://vg.szsharing.cn

composer require --dev phpstan/phpstan
来源：http://ky.nszjky.cn

[U80] PHP：代码规范修复
来源：http://zi.bjjhwx.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://vn.jctech888.com.cn

[U81] JS：初始化项目
来源：http://bk.panjiajie.cn

npm init -y;  npm i express
来源：http://fb.chemitech.net.cn

[U82] JS：package.json 脚本
来源：http://es.huixinmuqiang.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yc.jianghongdianzi.cn

[U83] JS：ES Module 导入导出
来源：http://ue.chemitech.net.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ac.bjjhwx.cn

[U84] JS：CommonJS 写法
来源：http://la.bookmarksfly.cn

module.exports = { a };  const { a } = require("./m");
来源：http://yl.hahajie.cn

[U85] JS：可选链
来源：http://iq.asd995.cn

a?.b?.c
来源：http://cp.521024.cn

[U86] JS：空值合并
来源：http://mr.hahajie.cn

a ?? b
来源：http://xw.hnjuh.cn

[U87] JS：解构默认值
来源：http://bn.yuntaijiaju.cn

const { a = 1, b = 2 } = obj;
来源：http://jm.haigaiapp.cn

[U88] JS：对象展开合并
来源：http://qu.huanxung.cn

{ ...a, ...b }
来源：http://uc.shtwfgs.cn

[U89] JS：数组去重
来源：http://ga.nicolike.cn

[...new Set(arr)]
来源：http://nd.hahajie.cn

[U90] JS：数字数组排序
来源：http://fm.shxzukj.cn

[...arr].sort((a, b) => a - b)
来源：http://xr.9csxet.cn

[U91] JS：对象键值遍历
来源：http://xf.shxzskj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kh.gzmigu.cn

[U92] JS：深拷贝
来源：http://na.szxytkj.cn

structuredClone(obj)
来源：http://ul.hahajie.cn

[U93] JS：模板字符串
来源：http://gh.shxzskj.cn

`共 ${n} 条`
来源：http://xv.haigaiapp.cn

[U94] JS：箭头函数
来源：http://hw.521024.cn

const double = x => x * 2;
来源：http://tv.521024.cn

[U95] JS：Promise 包装
来源：http://bi.panjiajie.cn

new Promise((resolve, reject) => {})
来源：http://nv.chemitech.net.cn

[U96] JS：async/await 与异常
来源：http://uo.9csxet.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qe.wgjwhj.cn

[U97] JS：并发请求
来源：http://cz.huixiangedu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bk.nszjky.cn

[U98] JS：fetch 带 JSON
来源：http://nz.muxihuayi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rn.muxihuayi.cn

[U99] JS：事件监听
来源：http://cm.yuexingan06.cn

el.addEventListener("click", e => {})
来源：http://je.szxytkj.cn

[U100] JS：DOM 查询
来源：http://cv.jctech888.com.cn

document.querySelector(".item")
来源：http://gf.bookmarksfly.cn

[U101] JS：classList 操作
来源：http://fk.szxytkj.cn

el.classList.toggle("active")
来源：http://or.shxzukj.cn

[U102] JS：本地存储
来源：http://ah.muxihuayi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://hb.jianghongdianzi.cn

[U103] JS：定时器
来源：http://sf.huanxung.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://eq.huixinmuqiang.cn

[U104] JS：防抖
来源：http://df.yuntaijiaju.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wo.521024.cn

[U105] JS：节流
来源：http://ro.newstarts.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gs.chemitech.net.cn

[U106] JS：日期格式化
来源：http://qj.wgjwhj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yf.jianghongdianzi.cn

[U107] JS：数字千分位
来源：http://nr.nicolike.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ry.nicolike.cn

[U108] JS：随机整数
来源：http://wa.bookmarksfly.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bx.asd995.cn

[U109] JS：数组分组
来源：http://vk.szsharing.cn

Object.groupBy(arr, x => x.type)
来源：http://hp.muxihuayi.cn

[U110] JS：数组分块
来源：http://ay.panjiajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wj.szxytkj.cn

[U111] JS：对象转 Map
来源：http://ou.asd995.cn

new Map(Object.entries(obj))
来源：http://uz.asd995.cn

[U112] JS：字符串补位
来源：http://ym.huixiangedu.cn

"7".padStart(3, "0")
来源：http://li.szsharing.cn

[U113] JS：正则替换全部
来源：http://hk.panjiajie.cn

s.replaceAll("a", "b")
来源：http://kp.nszjky.cn

[U114] JS：JSON 深比较
来源：http://rc.bookmarksfly.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://sk.bookmarksfly.cn

[U115] JS：生成 UUID
来源：http://xb.szsharing.cn

crypto.randomUUID()
来源：http://mk.jctech888.com.cn

[U116] JS：类型检查（JSDoc）
来源：http://zp.gzmigu.cn

/** @param {string} name */ function f(name) {}
来源：http://jq.panjiajie.cn

[U117] JS：单元测试
来源：http://ud.521024.cn

npm i -D vitest;  npx vitest
来源：http://su.haigaiapp.cn

[U118] JS：开发服务器
来源：http://zr.shtwfgs.cn

npm i -D vite;  npx vite
来源：http://vy.521024.cn

[U119] JS：生产构建
来源：http://kp.hnjuh.cn

npx vite build
来源：http://hu.panjiajie.cn

[U120] JS：读取环境变量（Vite）
来源：http://td.9csxet.cn

import.meta.env.VITE_API_URL
来源：http://kx.jianghongdianzi.cn

================================================================================
来源：http://se.huixinmuqiang.cn

统计汇总
来源：http://hf.hnjuh.cn

================================================================================
来源：http://pw.szxytkj.cn

按语言统计（条）：
来源：http://xb.haigaiapp.cn

Python ......... 252
来源：http://ku.shtwfgs.cn

PHP ............ 252
来源：http://qi.jianghongdianzi.cn

JavaScript ..... 252
来源：http://ya.szxytkj.cn

TypeScript ..... 212
来源：http://na.hnjuh.cn

Java ........... 212
来源：http://gz.huixiangedu.cn

Go ............. 212
来源：http://kd.bjjhwx.cn

Ruby ........... 212
来源：http://wr.wgjwhj.cn

C# ............. 212
来源：http://fh.nszjky.cn


<!-- 参考信息 -->