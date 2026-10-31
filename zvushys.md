代发 wailian999

[T31] Lua：Hello World
来源：http://ep.lnxyls.cn

print("Hello")
来源：http://uj.yuntaijiaju.cn

[T32] Lua：局部变量
来源：http://aq.huixiangedu.cn

local a = 1
来源：http://pd.shxzukj.cn

[T33] Lua：表（数组）
来源：http://xc.haigaiapp.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wk.bookmarksfly.cn

[T34] Lua：遍历表
来源：http://xl.chemitech.net.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://oi.521024.cn

[T35] Lua：字典表
来源：http://aq.newstarts.cn

local d = { a = 1 };  d.b = 2
来源：http://ko.hnjuh.cn

[T36] Lua：函数
来源：http://dt.521024.cn

function add(a, b) return a + b end
来源：http://im.yuntaijiaju.cn

[T37] Lua：字符串拼接
来源：http://xy.jctech888.com.cn

"a" .. "b"
来源：http://ta.yuntaijiaju.cn

[T38] Lua：条件
来源：http://od.nicolike.cn

if x > 0 then print("正") end
来源：http://st.chemitech.net.cn

[T39] Lua：模式匹配
来源：http://yp.nszjky.cn

string.find(s, "%d+")
来源：http://fp.huixinmuqiang.cn

[T40] Lua：元表
来源：http://kx.gzmigu.cn

setmetatable({}, { __index = base })
来源：http://js.nicolike.cn

[T41] Perl：Hello World
来源：http://dg.asd995.cn

print "Hello\n";
来源：http://pr.huixiangedu.cn

[T42] Perl：变量类型
来源：http://vv.huixinmuqiang.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lp.lnxyls.cn

[T43] Perl：字符串插值
来源：http://fc.hahajie.cn

"值: $a"
来源：http://xq.bookmarksfly.cn

[T44] Perl：条件
来源：http://gb.jianghongdianzi.cn

if ($a > 0) { print "正"; }
来源：http://qr.yuexingan06.cn

[T45] Perl：数组遍历
来源：http://iq.wgjwhj.cn

for my $x (@arr) { print $x; }
来源：http://ar.yuntaijiaju.cn

[T46] Perl：哈希操作
来源：http://lh.521024.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gf.lnxyls.cn

[T47] Perl：正则捕获
来源：http://zz.panjiajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://kf.nicolike.cn

[T48] Perl：正则替换
来源：http://be.lnxyls.cn

$s =~ s/old/new/g;
来源：http://ah.newstarts.cn

[T49] Perl：函数
来源：http://up.muxihuayi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://af.szsharing.cn

[T50] Perl：逐行读文件
来源：http://nh.9csxet.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://yx.huixinmuqiang.cn

while (my $line = <$fh>) { print $line; }
来源：http://uc.wgjwhj.cn

[T51] Scala：Hello World
来源：http://ww.yuexingan06.cn

println("Hello")
来源：http://mc.szxytkj.cn

[T52] Scala：变量
来源：http://np.colortex.cn

val a = 1;  var b = 2
来源：http://ii.szxytkj.cn

[T53] Scala：字符串插值
来源：http://dd.szsharing.cn

s"值: $b"
来源：http://ap.huixiangedu.cn

[T54] Scala：集合映射
来源：http://sd.gzmigu.cn

List(1, 2, 3).map(_ * 2)
来源：http://si.newstarts.cn

[T55] Scala：集合过滤
来源：http://et.jianghongdianzi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wk.nszjky.cn

[T56] Scala：样例类
来源：http://ug.asd995.cn

case class User(name: String, age: Int)
来源：http://jx.yuexingan06.cn

[T57] Scala：模式匹配
来源：http://eb.bjjhwx.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://uc.shxzukj.cn

[T58] Scala：函数定义
来源：http://px.huanxung.cn

def add(a: Int, b: Int): Int = a + b
来源：http://oa.nszjky.cn

[T59] Scala：循环
来源：http://fe.panjiajie.cn

for (i <- 1 to 10) println(i)
来源：http://yb.wgjwhj.cn

[T60] Scala：折叠
来源：http://yl.jianghongdianzi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vm.9csxet.cn

================================================================================
来源：http://uv.yuexingan06.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hv.wgjwhj.cn

================================================================================
来源：http://mx.hnjuh.cn

[U01] Py：创建虚拟环境
来源：http://xe.yuntaijiaju.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bp.newstarts.cn

[U02] Py：导出 / 安装依赖
来源：http://vc.wgjwhj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://la.asd995.cn

[U03] Py：加载 .env 配置
来源：http://eg.gzmigu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://dk.hnjuh.cn

[U04] Py：变量调试打印
来源：http://pp.jianghongdianzi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://yw.huixinmuqiang.cn

[U05] Py：列表去重且保序
来源：http://et.hnjuh.cn

list(dict.fromkeys(arr))
来源：http://nu.jctech888.com.cn

[U06] Py：合并两个字典
来源：http://ut.jctech888.com.cn

{**a, **b}
来源：http://jw.yuexingan06.cn

[U07] Py：反转字典键值
来源：http://ft.shxzukj.cn

{v: k for k, v in d.items()}
来源：http://iw.muxihuayi.cn

[U08] Py：展平二维列表
来源：http://ag.yuntaijiaju.cn

[y for x in nested for y in x]
来源：http://ry.wgjwhj.cn

[U09] Py：字典取最大值的键
来源：http://sb.chemitech.net.cn

max(d, key=d.get)
来源：http://hv.yuntaijiaju.cn

[U10] Py：按值排序字典
来源：http://zl.jianghongdianzi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hq.huixiangedu.cn

[U11] Py：生成器表达式
来源：http://jf.jianghongdianzi.cn

(x * 2 for x in arr)
来源：http://qc.jctech888.com.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lz.gzmigu.cn

Counter(arr).most_common(3)
来源：http://jd.shtwfgs.cn

[U13] Py：固定长度队列
来源：http://hz.bookmarksfly.cn

deque(maxlen=10)
来源：http://ap.9csxet.cn

[U14] Py：分组收集到列表
来源：http://to.nicolike.cn

defaultdict(list)
来源：http://av.colortex.cn

[U15] Py：高精度计时
来源：http://rn.521024.cn

t = time.perf_counter()
来源：http://hh.gzmigu.cn

[U16] Py：命令行参数解析
来源：http://kx.panjiajie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wo.521024.cn

[U17] Py：初始化日志
来源：http://tc.bookmarksfly.cn

logging.basicConfig(level=logging.INFO)
来源：http://hc.szsharing.cn

[U18] Py：预编译正则
来源：http://be.bookmarksfly.cn

pat = re.compile(r"\d+")
来源：http://qo.wgjwhj.cn

[U19] Py：正则替换带回调
来源：http://aq.szxytkj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qp.szsharing.cn

[U20] Py：缓存函数结果
来源：http://cm.panjiajie.cn

@functools.lru_cache(maxsize=None)
来源：http://fx.nicolike.cn

[U21] Py：自定义上下文管理器
来源：http://on.hnjuh.cn

@contextlib.contextmanager
来源：http://jy.nicolike.cn

[U22] Py：矩阵转置
来源：http://wu.szxytkj.cn

list(zip(*m))
来源：http://ir.huixiangedu.cn

[U23] Py：分块读取大文件
来源：http://ei.wgjwhj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tu.jctech888.com.cn

[U24] Py：路径操作
来源：http://oa.bjjhwx.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ui.newstarts.cn

[U25] Py：CSV 按字典读
来源：http://yo.nszjky.cn

csv.DictReader(f)
来源：http://rm.bookmarksfly.cn

[U26] Py：并发下载
来源：http://df.nszjky.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vi.shxzukj.cn

[U27] Py：异步 HTTP
来源：http://hf.bookmarksfly.cn

aiohttp.ClientSession() 配合 async with
来源：http://lc.nicolike.cn

[U28] Py：类型别名
来源：http://cy.newstarts.cn

UserId = int
来源：http://bx.hnjuh.cn

[U29] Py：属性校验
来源：http://fr.hnjuh.cn

@property 与 @x.setter 配合
来源：http://dg.asd995.cn

[U30] Py：数据类
来源：http://nv.newstarts.cn

@dataclass(slots=True)
来源：http://hg.9csxet.cn

[U31] Py：单测
来源：http://lr.shtwfgs.cn

python -m pytest -q
来源：http://ri.szsharing.cn

[U32] Py：代码格式化
来源：http://zh.lnxyls.cn

ruff format . && ruff check --fix .
来源：http://nl.521024.cn

[U33] Py：打包发布
来源：http://fn.huixiangedu.cn

python -m build  （依赖 pyproject.toml）
来源：http://fz.yuntaijiaju.cn

[U34] Py：判断编码
来源：http://wu.szsharing.cn

chardet.detect(raw)
来源：http://bm.szsharing.cn

[U35] Py：发送邮件
来源：http://sy.9csxet.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://er.hahajie.cn

[U36] Py：定时任务
来源：http://te.gzmigu.cn

schedule.every(10).minutes.do(job)
来源：http://qu.bookmarksfly.cn

[U37] Py：读写 Excel
来源：http://vo.jctech888.com.cn

pandas.read_excel / DataFrame.to_excel
来源：http://kz.hahajie.cn

[U38] Py：获取脚本所在目录
来源：http://zp.shxzukj.cn

Path(__file__).resolve().parent
来源：http://ai.muxihuayi.cn

[U39] Py：判断是否在交互环境
来源：http://vt.hahajie.cn

sys.stdout.isatty()
来源：http://nb.bjjhwx.cn

[U40] Py：打印到标准错误
来源：http://if.panjiajie.cn

print("err", file=sys.stderr)
来源：http://zt.huanxung.cn

[U41] PHP：初始化 Composer 项目
来源：http://jq.wgjwhj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://oc.newstarts.cn

[U42] PHP：PSR-4 自动加载
来源：http://eq.shxzukj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tz.muxihuayi.cn

[U43] PHP：声明命名空间
来源：http://xn.nszjky.cn

namespace App\Http;
来源：http://xb.szxytkj.cn

[U44] PHP：开启严格类型
来源：http://yp.yuntaijiaju.cn

declare(strict_types=1);
来源：http://nn.9csxet.cn

[U45] PHP：类型声明与返回类型
来源：http://km.colortex.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://rd.colortex.cn

[U46] PHP：可空类型
来源：http://vj.jianghongdianzi.cn

?string $name = null
来源：http://zk.yuntaijiaju.cn

[U47] PHP：联合类型
来源：http://fv.wgjwhj.cn

int|string $id
来源：http://ix.colortex.cn

[U48] PHP：纯枚举
来源：http://jj.yuntaijiaju.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lc.nszjky.cn

[U49] PHP：只读属性
来源：http://it.asd995.cn

public readonly string $name
来源：http://rh.jctech888.com.cn

[U50] PHP：构造器属性提升
来源：http://mt.wgjwhj.cn

public function __construct(private int $id) {}
来源：http://bd.shxzukj.cn

[U51] PHP：数组解构
来源：http://yy.panjiajie.cn

[$a, $b] = $arr;
来源：http://gz.nszjky.cn

[U52] PHP：箭头函数
来源：http://sm.asd995.cn

$double = fn($x) => $x * 2;
来源：http://tj.szsharing.cn

[U53] PHP：空合并运算符
来源：http://wd.jianghongdianzi.cn

$v = $a ?? $b ?? "default";
来源：http://eb.nicolike.cn

[U54] PHP：空安全调用
来源：http://ez.chemitech.net.cn

$obj?->method()
来源：http://zv.shxzskj.cn

[U55] PHP：match 表达式
来源：http://uy.huixinmuqiang.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://us.newstarts.cn

[U56] PHP：命名参数
来源：http://sh.haigaiapp.cn

f(a: 1, b: 2)
来源：http://fp.bookmarksfly.cn

[U57] PHP：字符串插值
来源：http://mj.huixinmuqiang.cn

"值: {$a}"
来源：http://ny.yuntaijiaju.cn

[U58] PHP：数组三件套
来源：http://lj.yuntaijiaju.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://if.haigaiapp.cn

[U59] PHP：自定义排序
来源：http://pc.szsharing.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rp.jianghongdianzi.cn

[U60] PHP：JSON 编解码
来源：http://oe.hahajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vn.huixiangedu.cn

[U61] PHP：正则
来源：http://xw.wgjwhj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ef.asd995.cn

[U62] PHP：日期对象
来源：http://tz.wgjwhj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tc.huixinmuqiang.cn

[U63] PHP：文件读写
来源：http://ya.asd995.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kg.newstarts.cn

[U64] PHP：目录遍历
来源：http://gp.huanxung.cn

glob("dir/*.php");  scandir("dir");
来源：http://ow.shxzskj.cn

[U65] PHP：会话
来源：http://zv.jctech888.com.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ep.nszjky.cn

[U66] PHP：设置 Cookie
来源：http://sl.nicolike.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qc.newstarts.cn

[U67] PHP：处理文件上传
来源：http://hq.yuexingan06.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ps.bjjhwx.cn

[U68] PHP：PDO 连接
来源：http://ol.nszjky.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fs.huixiangedu.cn

[U69] PHP：PDO 预处理
来源：http://hi.jctech888.com.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xf.asd995.cn

[U70] PHP：PDO 事务
来源：http://to.9csxet.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fr.wgjwhj.cn

[U71] PHP：抛出异常
来源：http://jj.szsharing.cn

throw new RuntimeException("失败", 500);
来源：http://yd.newstarts.cn

[U72] PHP：写错误日志
来源：http://xu.nszjky.cn

error_log("失败: " . $e->getMessage());
来源：http://ww.nszjky.cn

[U73] PHP：读取 ini 配置
来源：http://em.panjiajie.cn

parse_ini_file("config.ini", true)
来源：http://tj.shtwfgs.cn

[U74] PHP：读取环境变量
来源：http://bv.asd995.cn

getenv("APP_ENV") ?: "production"
来源：http://du.chemitech.net.cn

[U75] PHP：依赖注入
来源：http://fu.panjiajie.cn

composer require psr/container
来源：http://nx.hahajie.cn

[U76] PHP：简单路由
来源：http://gi.bjjhwx.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qv.newstarts.cn

[U77] PHP：模板渲染
来源：http://ed.shxzskj.cn

composer require twig/twig
来源：http://bv.szsharing.cn

[U78] PHP：单元测试
来源：http://xs.panjiajie.cn

composer require --dev phpunit/phpunit
来源：http://fu.nicolike.cn

[U79] PHP：静态分析
来源：http://cd.szsharing.cn

composer require --dev phpstan/phpstan
来源：http://qz.9csxet.cn

[U80] PHP：代码规范修复
来源：http://lw.wgjwhj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://sj.szxytkj.cn

[U81] JS：初始化项目
来源：http://ma.hnjuh.cn

npm init -y;  npm i express
来源：http://hx.9csxet.cn

[U82] JS：package.json 脚本
来源：http://lh.lnxyls.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ap.huixiangedu.cn

[U83] JS：ES Module 导入导出
来源：http://am.hahajie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://as.szxytkj.cn

[U84] JS：CommonJS 写法
来源：http://hk.jctech888.com.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wx.9csxet.cn

[U85] JS：可选链
来源：http://cs.szxytkj.cn

a?.b?.c
来源：http://xj.muxihuayi.cn

[U86] JS：空值合并
来源：http://vv.newstarts.cn

a ?? b
来源：http://ro.muxihuayi.cn

[U87] JS：解构默认值
来源：http://dm.bookmarksfly.cn

const { a = 1, b = 2 } = obj;
来源：http://ix.chemitech.net.cn

[U88] JS：对象展开合并
来源：http://de.gzmigu.cn

{ ...a, ...b }
来源：http://uw.newstarts.cn

[U89] JS：数组去重
来源：http://fa.szxytkj.cn

[...new Set(arr)]
来源：http://gb.nszjky.cn

[U90] JS：数字数组排序
来源：http://de.yuexingan06.cn

[...arr].sort((a, b) => a - b)
来源：http://lc.jianghongdianzi.cn

[U91] JS：对象键值遍历
来源：http://os.nicolike.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ge.bookmarksfly.cn

[U92] JS：深拷贝
来源：http://kx.yuntaijiaju.cn

structuredClone(obj)
来源：http://cs.shxzskj.cn

[U93] JS：模板字符串
来源：http://pe.chemitech.net.cn

`共 ${n} 条`
来源：http://sb.yuexingan06.cn

[U94] JS：箭头函数
来源：http://vy.yuexingan06.cn

const double = x => x * 2;
来源：http://ph.newstarts.cn

[U95] JS：Promise 包装
来源：http://bg.bjjhwx.cn

new Promise((resolve, reject) => {})
来源：http://tl.panjiajie.cn

[U96] JS：async/await 与异常
来源：http://ru.newstarts.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dk.colortex.cn

[U97] JS：并发请求
来源：http://ae.yuexingan06.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ux.jctech888.com.cn

[U98] JS：fetch 带 JSON
来源：http://xe.colortex.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vk.panjiajie.cn

[U99] JS：事件监听
来源：http://mh.shxzukj.cn

el.addEventListener("click", e => {})
来源：http://xj.yuntaijiaju.cn

[U100] JS：DOM 查询
来源：http://rp.szsharing.cn

document.querySelector(".item")
来源：http://wu.panjiajie.cn

[U101] JS：classList 操作
来源：http://ul.haigaiapp.cn

el.classList.toggle("active")
来源：http://zt.hahajie.cn

[U102] JS：本地存储
来源：http://np.shxzukj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ew.9csxet.cn

[U103] JS：定时器
来源：http://fh.szxytkj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://em.9csxet.cn

[U104] JS：防抖
来源：http://rl.shxzskj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lt.bjjhwx.cn

[U105] JS：节流
来源：http://qs.yuntaijiaju.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xz.nszjky.cn

[U106] JS：日期格式化
来源：http://hr.chemitech.net.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zu.yuexingan06.cn

[U107] JS：数字千分位
来源：http://rp.hahajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kh.shxzskj.cn

[U108] JS：随机整数
来源：http://eg.gzmigu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gs.yuexingan06.cn

[U109] JS：数组分组
来源：http://lw.9csxet.cn

Object.groupBy(arr, x => x.type)
来源：http://jh.521024.cn

[U110] JS：数组分块
来源：http://sv.chemitech.net.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qm.wgjwhj.cn

[U111] JS：对象转 Map
来源：http://ma.521024.cn

new Map(Object.entries(obj))
来源：http://lj.jianghongdianzi.cn

[U112] JS：字符串补位
来源：http://at.hahajie.cn

"7".padStart(3, "0")
来源：http://bd.521024.cn

[U113] JS：正则替换全部
来源：http://qc.yuntaijiaju.cn

s.replaceAll("a", "b")
来源：http://jt.nszjky.cn

[U114] JS：JSON 深比较
来源：http://oc.nicolike.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://os.muxihuayi.cn

[U115] JS：生成 UUID
来源：http://rq.yuexingan06.cn

crypto.randomUUID()
来源：http://oq.colortex.cn

[U116] JS：类型检查（JSDoc）
来源：http://um.bjjhwx.cn

/** @param {string} name */ function f(name) {}
来源：http://yb.nicolike.cn

[U117] JS：单元测试
来源：http://sj.shxzskj.cn

npm i -D vitest;  npx vitest
来源：http://pv.shxzskj.cn

[U118] JS：开发服务器
来源：http://ln.521024.cn

npm i -D vite;  npx vite
来源：http://gq.muxihuayi.cn


<!-- 参考信息 -->