代发 wailian999

[T37] Lua：字符串拼接
来源：http://cb.huanxung.cn

"a" .. "b"
来源：http://rg.panjiajie.cn

[T38] Lua：条件
来源：http://mz.yuntaijiaju.cn

if x > 0 then print("正") end
来源：http://xm.shxzukj.cn

[T39] Lua：模式匹配
来源：http://og.bjjhwx.cn

string.find(s, "%d+")
来源：http://qa.huanxung.cn

[T40] Lua：元表
来源：http://kn.shxzukj.cn

setmetatable({}, { __index = base })
来源：http://yl.bookmarksfly.cn

[T41] Perl：Hello World
来源：http://ju.muxihuayi.cn

print "Hello\n";
来源：http://ge.haigaiapp.cn

[T42] Perl：变量类型
来源：http://lu.yuntaijiaju.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wg.colortex.cn

[T43] Perl：字符串插值
来源：http://fj.yuexingan06.cn

"值: $a"
来源：http://os.yuexingan06.cn

[T44] Perl：条件
来源：http://oo.shxzskj.cn

if ($a > 0) { print "正"; }
来源：http://wb.nszjky.cn

[T45] Perl：数组遍历
来源：http://kb.haigaiapp.cn

for my $x (@arr) { print $x; }
来源：http://ih.haigaiapp.cn

[T46] Perl：哈希操作
来源：http://fd.shtwfgs.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tk.huixiangedu.cn

[T47] Perl：正则捕获
来源：http://uu.szsharing.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://sn.colortex.cn

[T48] Perl：正则替换
来源：http://em.hnjuh.cn

$s =~ s/old/new/g;
来源：http://zr.muxihuayi.cn

[T49] Perl：函数
来源：http://mh.hnjuh.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ti.jctech888.com.cn

[T50] Perl：逐行读文件
来源：http://io.jctech888.com.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ub.gzmigu.cn

while (my $line = <$fh>) { print $line; }
来源：http://xu.panjiajie.cn

[T51] Scala：Hello World
来源：http://cv.szxytkj.cn

println("Hello")
来源：http://gy.lnxyls.cn

[T52] Scala：变量
来源：http://vl.9csxet.cn

val a = 1;  var b = 2
来源：http://aw.chemitech.net.cn

[T53] Scala：字符串插值
来源：http://lr.huanxung.cn

s"值: $b"
来源：http://qi.shtwfgs.cn

[T54] Scala：集合映射
来源：http://yq.wgjwhj.cn

List(1, 2, 3).map(_ * 2)
来源：http://om.hahajie.cn

[T55] Scala：集合过滤
来源：http://sn.jctech888.com.cn

List(1, 2, 3).filter(_ > 1)
来源：http://bf.gzmigu.cn

[T56] Scala：样例类
来源：http://nw.haigaiapp.cn

case class User(name: String, age: Int)
来源：http://nt.9csxet.cn

[T57] Scala：模式匹配
来源：http://jj.lnxyls.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://or.huixiangedu.cn

[T58] Scala：函数定义
来源：http://tu.szxytkj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ul.asd995.cn

[T59] Scala：循环
来源：http://fx.huixiangedu.cn

for (i <- 1 to 10) println(i)
来源：http://ji.nszjky.cn

[T60] Scala：折叠
来源：http://jd.muxihuayi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ap.shxzskj.cn

================================================================================
来源：http://ns.asd995.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://us.asd995.cn

================================================================================
来源：http://ql.9csxet.cn

[U01] Py：创建虚拟环境
来源：http://gj.chemitech.net.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ou.colortex.cn

[U02] Py：导出 / 安装依赖
来源：http://my.nicolike.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tr.hahajie.cn

[U03] Py：加载 .env 配置
来源：http://pt.gzmigu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qi.chemitech.net.cn

[U04] Py：变量调试打印
来源：http://ui.huixinmuqiang.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lm.chemitech.net.cn

[U05] Py：列表去重且保序
来源：http://xh.panjiajie.cn

list(dict.fromkeys(arr))
来源：http://eb.hahajie.cn

[U06] Py：合并两个字典
来源：http://do.wgjwhj.cn

{**a, **b}
来源：http://bj.panjiajie.cn

[U07] Py：反转字典键值
来源：http://yg.gzmigu.cn

{v: k for k, v in d.items()}
来源：http://ji.haigaiapp.cn

[U08] Py：展平二维列表
来源：http://un.yuntaijiaju.cn

[y for x in nested for y in x]
来源：http://bv.huixiangedu.cn

[U09] Py：字典取最大值的键
来源：http://py.huixinmuqiang.cn

max(d, key=d.get)
来源：http://ei.shxzukj.cn

[U10] Py：按值排序字典
来源：http://ea.asd995.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://oe.shxzskj.cn

[U11] Py：生成器表达式
来源：http://ld.hnjuh.cn

(x * 2 for x in arr)
来源：http://kk.gzmigu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://oa.szsharing.cn

Counter(arr).most_common(3)
来源：http://lb.haigaiapp.cn

[U13] Py：固定长度队列
来源：http://pc.huixinmuqiang.cn

deque(maxlen=10)
来源：http://hi.yuexingan06.cn

[U14] Py：分组收集到列表
来源：http://ui.asd995.cn

defaultdict(list)
来源：http://ca.wgjwhj.cn

[U15] Py：高精度计时
来源：http://tu.huanxung.cn

t = time.perf_counter()
来源：http://xe.haigaiapp.cn

[U16] Py：命令行参数解析
来源：http://he.nszjky.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jj.hnjuh.cn

[U17] Py：初始化日志
来源：http://nu.asd995.cn

logging.basicConfig(level=logging.INFO)
来源：http://hq.newstarts.cn

[U18] Py：预编译正则
来源：http://vp.nicolike.cn

pat = re.compile(r"\d+")
来源：http://vp.521024.cn

[U19] Py：正则替换带回调
来源：http://nx.huixiangedu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rn.panjiajie.cn

[U20] Py：缓存函数结果
来源：http://qx.bookmarksfly.cn

@functools.lru_cache(maxsize=None)
来源：http://sv.nszjky.cn

[U21] Py：自定义上下文管理器
来源：http://pp.shtwfgs.cn

@contextlib.contextmanager
来源：http://sa.chemitech.net.cn

[U22] Py：矩阵转置
来源：http://gc.huixinmuqiang.cn

list(zip(*m))
来源：http://ah.szxytkj.cn

[U23] Py：分块读取大文件
来源：http://jn.shxzukj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vt.wgjwhj.cn

[U24] Py：路径操作
来源：http://tt.colortex.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://va.szsharing.cn

[U25] Py：CSV 按字典读
来源：http://ra.colortex.cn

csv.DictReader(f)
来源：http://lx.szxytkj.cn

[U26] Py：并发下载
来源：http://nt.yuexingan06.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pp.9csxet.cn

[U27] Py：异步 HTTP
来源：http://qn.panjiajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://xf.hahajie.cn

[U28] Py：类型别名
来源：http://jl.nicolike.cn

UserId = int
来源：http://ag.521024.cn

[U29] Py：属性校验
来源：http://qt.shxzskj.cn

@property 与 @x.setter 配合
来源：http://yx.9csxet.cn

[U30] Py：数据类
来源：http://ua.szsharing.cn

@dataclass(slots=True)
来源：http://ps.521024.cn

[U31] Py：单测
来源：http://iq.haigaiapp.cn

python -m pytest -q
来源：http://gc.huixiangedu.cn

[U32] Py：代码格式化
来源：http://cz.9csxet.cn

ruff format . && ruff check --fix .
来源：http://nz.wgjwhj.cn

[U33] Py：打包发布
来源：http://hz.yuntaijiaju.cn

python -m build  （依赖 pyproject.toml）
来源：http://eg.shxzukj.cn

[U34] Py：判断编码
来源：http://jy.szxytkj.cn

chardet.detect(raw)
来源：http://ty.shtwfgs.cn

[U35] Py：发送邮件
来源：http://we.yuexingan06.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qf.yuexingan06.cn

[U36] Py：定时任务
来源：http://gv.chemitech.net.cn

schedule.every(10).minutes.do(job)
来源：http://ts.szxytkj.cn

[U37] Py：读写 Excel
来源：http://bo.huixinmuqiang.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ic.bookmarksfly.cn

[U38] Py：获取脚本所在目录
来源：http://sf.muxihuayi.cn

Path(__file__).resolve().parent
来源：http://kw.muxihuayi.cn

[U39] Py：判断是否在交互环境
来源：http://fv.jctech888.com.cn

sys.stdout.isatty()
来源：http://cx.haigaiapp.cn

[U40] Py：打印到标准错误
来源：http://rs.lnxyls.cn

print("err", file=sys.stderr)
来源：http://ll.shxzukj.cn

[U41] PHP：初始化 Composer 项目
来源：http://gy.huixiangedu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zn.gzmigu.cn

[U42] PHP：PSR-4 自动加载
来源：http://ud.hnjuh.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gw.jctech888.com.cn

[U43] PHP：声明命名空间
来源：http://un.newstarts.cn

namespace App\Http;
来源：http://ue.huixinmuqiang.cn

[U44] PHP：开启严格类型
来源：http://rd.yuexingan06.cn

declare(strict_types=1);
来源：http://xm.yuexingan06.cn

[U45] PHP：类型声明与返回类型
来源：http://nq.huanxung.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jk.bjjhwx.cn

[U46] PHP：可空类型
来源：http://se.hnjuh.cn

?string $name = null
来源：http://pp.newstarts.cn

[U47] PHP：联合类型
来源：http://jb.newstarts.cn

int|string $id
来源：http://du.nicolike.cn

[U48] PHP：纯枚举
来源：http://kw.newstarts.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cc.panjiajie.cn

[U49] PHP：只读属性
来源：http://it.chemitech.net.cn

public readonly string $name
来源：http://rz.asd995.cn

[U50] PHP：构造器属性提升
来源：http://xv.yuexingan06.cn

public function __construct(private int $id) {}
来源：http://sq.shtwfgs.cn

[U51] PHP：数组解构
来源：http://rh.chemitech.net.cn

[$a, $b] = $arr;
来源：http://hv.bookmarksfly.cn

[U52] PHP：箭头函数
来源：http://uu.9csxet.cn

$double = fn($x) => $x * 2;
来源：http://qi.bjjhwx.cn

[U53] PHP：空合并运算符
来源：http://qh.yuntaijiaju.cn

$v = $a ?? $b ?? "default";
来源：http://rq.panjiajie.cn

[U54] PHP：空安全调用
来源：http://sb.wgjwhj.cn

$obj?->method()
来源：http://wf.haigaiapp.cn

[U55] PHP：match 表达式
来源：http://fq.muxihuayi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zz.lnxyls.cn

[U56] PHP：命名参数
来源：http://cu.chemitech.net.cn

f(a: 1, b: 2)
来源：http://oa.jctech888.com.cn

[U57] PHP：字符串插值
来源：http://dy.hahajie.cn

"值: {$a}"
来源：http://cx.panjiajie.cn

[U58] PHP：数组三件套
来源：http://bi.yuntaijiaju.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nk.panjiajie.cn

[U59] PHP：自定义排序
来源：http://iy.hnjuh.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mg.521024.cn

[U60] PHP：JSON 编解码
来源：http://iu.chemitech.net.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://nh.nszjky.cn

[U61] PHP：正则
来源：http://ok.asd995.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mk.jianghongdianzi.cn

[U62] PHP：日期对象
来源：http://gk.yuexingan06.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wz.panjiajie.cn

[U63] PHP：文件读写
来源：http://ng.shtwfgs.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mo.9csxet.cn

[U64] PHP：目录遍历
来源：http://qr.chemitech.net.cn

glob("dir/*.php");  scandir("dir");
来源：http://cq.huixiangedu.cn

[U65] PHP：会话
来源：http://nj.szsharing.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://aa.huanxung.cn

[U66] PHP：设置 Cookie
来源：http://od.lnxyls.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sb.yuexingan06.cn

[U67] PHP：处理文件上传
来源：http://nr.muxihuayi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qf.szsharing.cn

[U68] PHP：PDO 连接
来源：http://id.szsharing.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ch.shtwfgs.cn

[U69] PHP：PDO 预处理
来源：http://jd.shxzukj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jq.shxzskj.cn

[U70] PHP：PDO 事务
来源：http://wx.nszjky.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qz.hahajie.cn

[U71] PHP：抛出异常
来源：http://cd.huixiangedu.cn

throw new RuntimeException("失败", 500);
来源：http://yk.szsharing.cn

[U72] PHP：写错误日志
来源：http://uu.huixinmuqiang.cn

error_log("失败: " . $e->getMessage());
来源：http://af.huixiangedu.cn

[U73] PHP：读取 ini 配置
来源：http://ks.shtwfgs.cn

parse_ini_file("config.ini", true)
来源：http://sb.newstarts.cn

[U74] PHP：读取环境变量
来源：http://sy.newstarts.cn

getenv("APP_ENV") ?: "production"
来源：http://qo.haigaiapp.cn

[U75] PHP：依赖注入
来源：http://wo.shtwfgs.cn

composer require psr/container
来源：http://pz.szxytkj.cn

[U76] PHP：简单路由
来源：http://ia.szxytkj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tk.yuexingan06.cn

[U77] PHP：模板渲染
来源：http://yl.jianghongdianzi.cn

composer require twig/twig
来源：http://ti.haigaiapp.cn

[U78] PHP：单元测试
来源：http://yf.hahajie.cn

composer require --dev phpunit/phpunit
来源：http://iw.szxytkj.cn

[U79] PHP：静态分析
来源：http://fa.gzmigu.cn

composer require --dev phpstan/phpstan
来源：http://zi.jctech888.com.cn

[U80] PHP：代码规范修复
来源：http://oa.yuexingan06.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://if.muxihuayi.cn

[U81] JS：初始化项目
来源：http://uj.bookmarksfly.cn

npm init -y;  npm i express
来源：http://kz.shtwfgs.cn

[U82] JS：package.json 脚本
来源：http://gx.jctech888.com.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qx.shxzukj.cn

[U83] JS：ES Module 导入导出
来源：http://sx.haigaiapp.cn

export const a = 1;  import { a } from "./m.js";
来源：http://yd.hahajie.cn

[U84] JS：CommonJS 写法
来源：http://zk.hnjuh.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ov.muxihuayi.cn

[U85] JS：可选链
来源：http://xw.hahajie.cn

a?.b?.c
来源：http://rt.yuexingan06.cn

[U86] JS：空值合并
来源：http://mx.colortex.cn

a ?? b
来源：http://kg.shxzukj.cn

[U87] JS：解构默认值
来源：http://qt.jianghongdianzi.cn

const { a = 1, b = 2 } = obj;
来源：http://ct.colortex.cn

[U88] JS：对象展开合并
来源：http://ku.newstarts.cn

{ ...a, ...b }
来源：http://wg.shxzukj.cn

[U89] JS：数组去重
来源：http://xk.szsharing.cn

[...new Set(arr)]
来源：http://of.asd995.cn

[U90] JS：数字数组排序
来源：http://ec.nszjky.cn

[...arr].sort((a, b) => a - b)
来源：http://ru.wgjwhj.cn

[U91] JS：对象键值遍历
来源：http://pn.bookmarksfly.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cf.yuexingan06.cn

[U92] JS：深拷贝
来源：http://dl.shxzskj.cn

structuredClone(obj)
来源：http://ob.jctech888.com.cn

[U93] JS：模板字符串
来源：http://pr.shxzskj.cn

`共 ${n} 条`
来源：http://xq.nszjky.cn

[U94] JS：箭头函数
来源：http://gm.panjiajie.cn

const double = x => x * 2;
来源：http://jv.panjiajie.cn

[U95] JS：Promise 包装
来源：http://dw.huixinmuqiang.cn

new Promise((resolve, reject) => {})
来源：http://wb.szxytkj.cn

[U96] JS：async/await 与异常
来源：http://mi.jianghongdianzi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ze.shtwfgs.cn

[U97] JS：并发请求
来源：http://qj.shxzskj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://fs.colortex.cn

[U98] JS：fetch 带 JSON
来源：http://ax.yuntaijiaju.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mx.bjjhwx.cn

[U99] JS：事件监听
来源：http://nn.9csxet.cn

el.addEventListener("click", e => {})
来源：http://vl.huanxung.cn

[U100] JS：DOM 查询
来源：http://zg.muxihuayi.cn

document.querySelector(".item")
来源：http://ep.gzmigu.cn

[U101] JS：classList 操作
来源：http://mz.jctech888.com.cn

el.classList.toggle("active")
来源：http://di.shtwfgs.cn

[U102] JS：本地存储
来源：http://op.hahajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wb.hnjuh.cn

[U103] JS：定时器
来源：http://lt.szxytkj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gr.yuntaijiaju.cn

[U104] JS：防抖
来源：http://ee.szsharing.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xw.huanxung.cn

[U105] JS：节流
来源：http://ni.9csxet.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gh.shxzukj.cn

[U106] JS：日期格式化
来源：http://ba.huixinmuqiang.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://os.chemitech.net.cn

[U107] JS：数字千分位
来源：http://bd.shxzskj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wd.szxytkj.cn

[U108] JS：随机整数
来源：http://wz.huixinmuqiang.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://sa.hahajie.cn

[U109] JS：数组分组
来源：http://tc.9csxet.cn

Object.groupBy(arr, x => x.type)
来源：http://vc.jianghongdianzi.cn

[U110] JS：数组分块
来源：http://mj.jctech888.com.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://un.521024.cn

[U111] JS：对象转 Map
来源：http://jy.huanxung.cn

new Map(Object.entries(obj))
来源：http://wm.yuntaijiaju.cn

[U112] JS：字符串补位
来源：http://wk.bjjhwx.cn

"7".padStart(3, "0")
来源：http://nb.panjiajie.cn

[U113] JS：正则替换全部
来源：http://ag.newstarts.cn

s.replaceAll("a", "b")
来源：http://ql.bjjhwx.cn

[U114] JS：JSON 深比较
来源：http://xy.colortex.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ao.jianghongdianzi.cn

[U115] JS：生成 UUID
来源：http://if.muxihuayi.cn

crypto.randomUUID()
来源：http://nc.panjiajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://hr.bookmarksfly.cn

/** @param {string} name */ function f(name) {}
来源：http://tc.chemitech.net.cn

[U117] JS：单元测试
来源：http://tu.haigaiapp.cn

npm i -D vitest;  npx vitest
来源：http://vn.lnxyls.cn

[U118] JS：开发服务器
来源：http://we.szsharing.cn

npm i -D vite;  npx vite
来源：http://ys.chemitech.net.cn

[U119] JS：生产构建
来源：http://oa.szxytkj.cn

npx vite build
来源：http://fz.shxzukj.cn

[U120] JS：读取环境变量（Vite）
来源：http://oz.hnjuh.cn

import.meta.env.VITE_API_URL
来源：http://nd.yuexingan06.cn

================================================================================
来源：http://ms.yuntaijiaju.cn

统计汇总
来源：http://rf.huixiangedu.cn

================================================================================
来源：http://wi.jctech888.com.cn

按语言统计（条）：
来源：http://ie.szsharing.cn

Python ......... 252
来源：http://qp.panjiajie.cn

PHP ............ 252
来源：http://mi.gzmigu.cn

JavaScript ..... 252
来源：http://ce.wgjwhj.cn

TypeScript ..... 212
来源：http://dk.panjiajie.cn


<!-- 参考信息 -->