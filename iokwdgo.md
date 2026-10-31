代发 wailian999

[T29] Swift：guard 提前返回
来源：http://lo.panjiajie.cn

guard let x = opt else { return }
来源：http://ct.jctech888.com.cn

[T30] Swift：协议
来源：http://bj.huanxung.cn

protocol Shape { func area() -> Double }
来源：http://af.szxytkj.cn

[T31] Lua：Hello World
来源：http://gm.bookmarksfly.cn

print("Hello")
来源：http://bg.wgjwhj.cn

[T32] Lua：局部变量
来源：http://br.jctech888.com.cn

local a = 1
来源：http://pw.newstarts.cn

[T33] Lua：表（数组）
来源：http://ln.gzmigu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://nf.lnxyls.cn

[T34] Lua：遍历表
来源：http://ks.asd995.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://id.asd995.cn

[T35] Lua：字典表
来源：http://kb.bookmarksfly.cn

local d = { a = 1 };  d.b = 2
来源：http://ro.huanxung.cn

[T36] Lua：函数
来源：http://ah.shtwfgs.cn

function add(a, b) return a + b end
来源：http://cx.jctech888.com.cn

[T37] Lua：字符串拼接
来源：http://km.chemitech.net.cn

"a" .. "b"
来源：http://qd.huanxung.cn

[T38] Lua：条件
来源：http://ta.shtwfgs.cn

if x > 0 then print("正") end
来源：http://xd.shxzukj.cn

[T39] Lua：模式匹配
来源：http://ya.huanxung.cn

string.find(s, "%d+")
来源：http://mo.bjjhwx.cn

[T40] Lua：元表
来源：http://vd.panjiajie.cn

setmetatable({}, { __index = base })
来源：http://fa.yuexingan06.cn

[T41] Perl：Hello World
来源：http://cb.yuexingan06.cn

print "Hello\n";
来源：http://gl.nicolike.cn

[T42] Perl：变量类型
来源：http://dd.newstarts.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ai.yuexingan06.cn

[T43] Perl：字符串插值
来源：http://yk.nicolike.cn

"值: $a"
来源：http://ri.chemitech.net.cn

[T44] Perl：条件
来源：http://cx.nicolike.cn

if ($a > 0) { print "正"; }
来源：http://rw.wgjwhj.cn

[T45] Perl：数组遍历
来源：http://bm.bjjhwx.cn

for my $x (@arr) { print $x; }
来源：http://kh.9csxet.cn

[T46] Perl：哈希操作
来源：http://lz.yuntaijiaju.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pz.huixiangedu.cn

[T47] Perl：正则捕获
来源：http://jy.hahajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://tc.hnjuh.cn

[T48] Perl：正则替换
来源：http://cy.huixinmuqiang.cn

$s =~ s/old/new/g;
来源：http://eq.shtwfgs.cn

[T49] Perl：函数
来源：http://sj.chemitech.net.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gf.lnxyls.cn

[T50] Perl：逐行读文件
来源：http://hg.nszjky.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://en.jctech888.com.cn

while (my $line = <$fh>) { print $line; }
来源：http://bt.jctech888.com.cn

[T51] Scala：Hello World
来源：http://fl.nicolike.cn

println("Hello")
来源：http://rl.jianghongdianzi.cn

[T52] Scala：变量
来源：http://ix.lnxyls.cn

val a = 1;  var b = 2
来源：http://kz.yuntaijiaju.cn

[T53] Scala：字符串插值
来源：http://lo.nicolike.cn

s"值: $b"
来源：http://bv.jianghongdianzi.cn

[T54] Scala：集合映射
来源：http://mf.huixiangedu.cn

List(1, 2, 3).map(_ * 2)
来源：http://rs.huanxung.cn

[T55] Scala：集合过滤
来源：http://xh.haigaiapp.cn

List(1, 2, 3).filter(_ > 1)
来源：http://zg.colortex.cn

[T56] Scala：样例类
来源：http://xj.chemitech.net.cn

case class User(name: String, age: Int)
来源：http://lf.huixinmuqiang.cn

[T57] Scala：模式匹配
来源：http://lp.panjiajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://de.9csxet.cn

[T58] Scala：函数定义
来源：http://ia.hnjuh.cn

def add(a: Int, b: Int): Int = a + b
来源：http://jc.bjjhwx.cn

[T59] Scala：循环
来源：http://zk.yuexingan06.cn

for (i <- 1 to 10) println(i)
来源：http://pd.gzmigu.cn

[T60] Scala：折叠
来源：http://ab.huixiangedu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sv.gzmigu.cn

================================================================================
来源：http://im.yuexingan06.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ay.szxytkj.cn

================================================================================
来源：http://co.huixiangedu.cn

[U01] Py：创建虚拟环境
来源：http://pq.shtwfgs.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jq.panjiajie.cn

[U02] Py：导出 / 安装依赖
来源：http://sn.shxzskj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nv.shxzskj.cn

[U03] Py：加载 .env 配置
来源：http://ld.hahajie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ch.yuntaijiaju.cn

[U04] Py：变量调试打印
来源：http://fp.jctech888.com.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://is.newstarts.cn

[U05] Py：列表去重且保序
来源：http://gw.huixiangedu.cn

list(dict.fromkeys(arr))
来源：http://tt.asd995.cn

[U06] Py：合并两个字典
来源：http://id.muxihuayi.cn

{**a, **b}
来源：http://ye.asd995.cn

[U07] Py：反转字典键值
来源：http://pl.shxzskj.cn

{v: k for k, v in d.items()}
来源：http://yz.shxzskj.cn

[U08] Py：展平二维列表
来源：http://qe.szxytkj.cn

[y for x in nested for y in x]
来源：http://ji.panjiajie.cn

[U09] Py：字典取最大值的键
来源：http://de.huanxung.cn

max(d, key=d.get)
来源：http://wm.shxzukj.cn

[U10] Py：按值排序字典
来源：http://qa.hnjuh.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yy.huixiangedu.cn

[U11] Py：生成器表达式
来源：http://zs.haigaiapp.cn

(x * 2 for x in arr)
来源：http://zs.shxzskj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qv.bookmarksfly.cn

Counter(arr).most_common(3)
来源：http://qu.nicolike.cn

[U13] Py：固定长度队列
来源：http://as.521024.cn

deque(maxlen=10)
来源：http://ch.colortex.cn

[U14] Py：分组收集到列表
来源：http://an.bjjhwx.cn

defaultdict(list)
来源：http://cp.lnxyls.cn

[U15] Py：高精度计时
来源：http://po.muxihuayi.cn

t = time.perf_counter()
来源：http://hk.9csxet.cn

[U16] Py：命令行参数解析
来源：http://bk.haigaiapp.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vc.colortex.cn

[U17] Py：初始化日志
来源：http://vg.yuntaijiaju.cn

logging.basicConfig(level=logging.INFO)
来源：http://gx.yuntaijiaju.cn

[U18] Py：预编译正则
来源：http://kq.asd995.cn

pat = re.compile(r"\d+")
来源：http://hy.wgjwhj.cn

[U19] Py：正则替换带回调
来源：http://vc.nicolike.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://an.huixiangedu.cn

[U20] Py：缓存函数结果
来源：http://qt.newstarts.cn

@functools.lru_cache(maxsize=None)
来源：http://af.bookmarksfly.cn

[U21] Py：自定义上下文管理器
来源：http://bj.bookmarksfly.cn

@contextlib.contextmanager
来源：http://ax.wgjwhj.cn

[U22] Py：矩阵转置
来源：http://tr.wgjwhj.cn

list(zip(*m))
来源：http://mh.huixiangedu.cn

[U23] Py：分块读取大文件
来源：http://og.yuntaijiaju.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ur.hahajie.cn

[U24] Py：路径操作
来源：http://su.jctech888.com.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ei.yuntaijiaju.cn

[U25] Py：CSV 按字典读
来源：http://vx.9csxet.cn

csv.DictReader(f)
来源：http://rn.huanxung.cn

[U26] Py：并发下载
来源：http://jt.shtwfgs.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ey.colortex.cn

[U27] Py：异步 HTTP
来源：http://lx.asd995.cn

aiohttp.ClientSession() 配合 async with
来源：http://ni.nicolike.cn

[U28] Py：类型别名
来源：http://ur.yuexingan06.cn

UserId = int
来源：http://oh.9csxet.cn

[U29] Py：属性校验
来源：http://tu.nszjky.cn

@property 与 @x.setter 配合
来源：http://mf.shxzskj.cn

[U30] Py：数据类
来源：http://pg.newstarts.cn

@dataclass(slots=True)
来源：http://sf.gzmigu.cn

[U31] Py：单测
来源：http://gy.muxihuayi.cn

python -m pytest -q
来源：http://fz.shxzukj.cn

[U32] Py：代码格式化
来源：http://ql.lnxyls.cn

ruff format . && ruff check --fix .
来源：http://ky.szxytkj.cn

[U33] Py：打包发布
来源：http://jp.9csxet.cn

python -m build  （依赖 pyproject.toml）
来源：http://zx.shxzukj.cn

[U34] Py：判断编码
来源：http://qp.wgjwhj.cn

chardet.detect(raw)
来源：http://pi.panjiajie.cn

[U35] Py：发送邮件
来源：http://gt.shxzukj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qm.shxzukj.cn

[U36] Py：定时任务
来源：http://jn.9csxet.cn

schedule.every(10).minutes.do(job)
来源：http://se.asd995.cn

[U37] Py：读写 Excel
来源：http://gh.huixinmuqiang.cn

pandas.read_excel / DataFrame.to_excel
来源：http://gu.yuntaijiaju.cn

[U38] Py：获取脚本所在目录
来源：http://no.huanxung.cn

Path(__file__).resolve().parent
来源：http://xa.hnjuh.cn

[U39] Py：判断是否在交互环境
来源：http://qx.lnxyls.cn

sys.stdout.isatty()
来源：http://fc.yuntaijiaju.cn

[U40] Py：打印到标准错误
来源：http://vw.bjjhwx.cn

print("err", file=sys.stderr)
来源：http://gn.newstarts.cn

[U41] PHP：初始化 Composer 项目
来源：http://go.bookmarksfly.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ak.gzmigu.cn

[U42] PHP：PSR-4 自动加载
来源：http://xe.newstarts.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dq.asd995.cn

[U43] PHP：声明命名空间
来源：http://mw.bjjhwx.cn

namespace App\Http;
来源：http://lp.jctech888.com.cn

[U44] PHP：开启严格类型
来源：http://xj.jctech888.com.cn

declare(strict_types=1);
来源：http://vh.nicolike.cn

[U45] PHP：类型声明与返回类型
来源：http://qq.nicolike.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://zt.newstarts.cn

[U46] PHP：可空类型
来源：http://uh.nicolike.cn

?string $name = null
来源：http://jj.nszjky.cn

[U47] PHP：联合类型
来源：http://od.nszjky.cn

int|string $id
来源：http://rl.hnjuh.cn

[U48] PHP：纯枚举
来源：http://gl.muxihuayi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://di.huanxung.cn

[U49] PHP：只读属性
来源：http://yr.hnjuh.cn

public readonly string $name
来源：http://yy.haigaiapp.cn

[U50] PHP：构造器属性提升
来源：http://vh.colortex.cn

public function __construct(private int $id) {}
来源：http://wc.colortex.cn

[U51] PHP：数组解构
来源：http://fm.lnxyls.cn

[$a, $b] = $arr;
来源：http://dn.hnjuh.cn

[U52] PHP：箭头函数
来源：http://mb.huixinmuqiang.cn

$double = fn($x) => $x * 2;
来源：http://xz.yuntaijiaju.cn

[U53] PHP：空合并运算符
来源：http://rf.jianghongdianzi.cn

$v = $a ?? $b ?? "default";
来源：http://du.shxzskj.cn

[U54] PHP：空安全调用
来源：http://ov.panjiajie.cn

$obj?->method()
来源：http://jq.shtwfgs.cn

[U55] PHP：match 表达式
来源：http://fj.bookmarksfly.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jq.shxzskj.cn

[U56] PHP：命名参数
来源：http://jj.huixinmuqiang.cn

f(a: 1, b: 2)
来源：http://du.panjiajie.cn

[U57] PHP：字符串插值
来源：http://pc.asd995.cn

"值: {$a}"
来源：http://po.huanxung.cn

[U58] PHP：数组三件套
来源：http://pg.jianghongdianzi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rd.panjiajie.cn

[U59] PHP：自定义排序
来源：http://sa.wgjwhj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://se.colortex.cn

[U60] PHP：JSON 编解码
来源：http://gw.hnjuh.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yj.nicolike.cn

[U61] PHP：正则
来源：http://sh.jianghongdianzi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://du.nicolike.cn

[U62] PHP：日期对象
来源：http://px.shxzskj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zi.gzmigu.cn

[U63] PHP：文件读写
来源：http://sw.szsharing.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yd.shxzskj.cn

[U64] PHP：目录遍历
来源：http://hv.jctech888.com.cn

glob("dir/*.php");  scandir("dir");
来源：http://pw.jianghongdianzi.cn

[U65] PHP：会话
来源：http://sj.gzmigu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ie.szxytkj.cn

[U66] PHP：设置 Cookie
来源：http://ev.9csxet.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nk.huixiangedu.cn

[U67] PHP：处理文件上传
来源：http://li.yuntaijiaju.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://by.szxytkj.cn

[U68] PHP：PDO 连接
来源：http://sx.muxihuayi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://sd.shtwfgs.cn

[U69] PHP：PDO 预处理
来源：http://eh.jctech888.com.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ch.muxihuayi.cn

[U70] PHP：PDO 事务
来源：http://ds.shtwfgs.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://if.huixinmuqiang.cn

[U71] PHP：抛出异常
来源：http://ly.haigaiapp.cn

throw new RuntimeException("失败", 500);
来源：http://th.asd995.cn

[U72] PHP：写错误日志
来源：http://cs.521024.cn

error_log("失败: " . $e->getMessage());
来源：http://ji.newstarts.cn

[U73] PHP：读取 ini 配置
来源：http://dn.hnjuh.cn

parse_ini_file("config.ini", true)
来源：http://fq.nicolike.cn

[U74] PHP：读取环境变量
来源：http://fv.colortex.cn

getenv("APP_ENV") ?: "production"
来源：http://vd.asd995.cn

[U75] PHP：依赖注入
来源：http://kw.yuexingan06.cn

composer require psr/container
来源：http://fl.shtwfgs.cn

[U76] PHP：简单路由
来源：http://wh.panjiajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dn.nszjky.cn

[U77] PHP：模板渲染
来源：http://pu.chemitech.net.cn

composer require twig/twig
来源：http://de.shtwfgs.cn

[U78] PHP：单元测试
来源：http://ty.nszjky.cn

composer require --dev phpunit/phpunit
来源：http://hg.hahajie.cn

[U79] PHP：静态分析
来源：http://tn.huixiangedu.cn

composer require --dev phpstan/phpstan
来源：http://cv.panjiajie.cn

[U80] PHP：代码规范修复
来源：http://rb.jianghongdianzi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://mk.9csxet.cn

[U81] JS：初始化项目
来源：http://ur.jctech888.com.cn

npm init -y;  npm i express
来源：http://ya.chemitech.net.cn

[U82] JS：package.json 脚本
来源：http://xx.chemitech.net.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://is.lnxyls.cn

[U83] JS：ES Module 导入导出
来源：http://ls.nicolike.cn

export const a = 1;  import { a } from "./m.js";
来源：http://lf.muxihuayi.cn

[U84] JS：CommonJS 写法
来源：http://fr.yuexingan06.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ac.shtwfgs.cn

[U85] JS：可选链
来源：http://vs.chemitech.net.cn

a?.b?.c
来源：http://ab.9csxet.cn

[U86] JS：空值合并
来源：http://tt.szsharing.cn

a ?? b
来源：http://tn.colortex.cn

[U87] JS：解构默认值
来源：http://fr.shtwfgs.cn

const { a = 1, b = 2 } = obj;
来源：http://hr.hahajie.cn

[U88] JS：对象展开合并
来源：http://wy.huixinmuqiang.cn

{ ...a, ...b }
来源：http://ag.bookmarksfly.cn

[U89] JS：数组去重
来源：http://xq.hnjuh.cn

[...new Set(arr)]
来源：http://iy.chemitech.net.cn

[U90] JS：数字数组排序
来源：http://nk.szxytkj.cn

[...arr].sort((a, b) => a - b)
来源：http://uy.szxytkj.cn

[U91] JS：对象键值遍历
来源：http://zv.szsharing.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vv.panjiajie.cn

[U92] JS：深拷贝
来源：http://mf.huixinmuqiang.cn

structuredClone(obj)
来源：http://my.yuntaijiaju.cn

[U93] JS：模板字符串
来源：http://qm.muxihuayi.cn

`共 ${n} 条`
来源：http://aw.bookmarksfly.cn

[U94] JS：箭头函数
来源：http://lm.bjjhwx.cn

const double = x => x * 2;
来源：http://bh.shtwfgs.cn

[U95] JS：Promise 包装
来源：http://hf.nicolike.cn

new Promise((resolve, reject) => {})
来源：http://wh.wgjwhj.cn

[U96] JS：async/await 与异常
来源：http://vf.newstarts.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ef.hnjuh.cn

[U97] JS：并发请求
来源：http://eg.bookmarksfly.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rh.huixinmuqiang.cn

[U98] JS：fetch 带 JSON
来源：http://rb.asd995.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://sw.chemitech.net.cn

[U99] JS：事件监听
来源：http://zu.shtwfgs.cn

el.addEventListener("click", e => {})
来源：http://cx.shxzskj.cn

[U100] JS：DOM 查询
来源：http://db.shtwfgs.cn

document.querySelector(".item")
来源：http://lr.chemitech.net.cn

[U101] JS：classList 操作
来源：http://vu.lnxyls.cn

el.classList.toggle("active")
来源：http://lk.jianghongdianzi.cn

[U102] JS：本地存储
来源：http://zm.lnxyls.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://kx.jctech888.com.cn

[U103] JS：定时器
来源：http://qo.chemitech.net.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ey.muxihuayi.cn

[U104] JS：防抖
来源：http://vz.gzmigu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ua.shxzskj.cn

[U105] JS：节流
来源：http://ei.nszjky.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ua.jianghongdianzi.cn

[U106] JS：日期格式化
来源：http://qi.bjjhwx.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cf.newstarts.cn

[U107] JS：数字千分位
来源：http://xv.colortex.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kk.chemitech.net.cn

[U108] JS：随机整数
来源：http://ec.panjiajie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bq.huixiangedu.cn

[U109] JS：数组分组
来源：http://su.shtwfgs.cn

Object.groupBy(arr, x => x.type)
来源：http://ch.nicolike.cn

[U110] JS：数组分块
来源：http://sc.shxzukj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gn.huanxung.cn

[U111] JS：对象转 Map
来源：http://uw.hnjuh.cn

new Map(Object.entries(obj))
来源：http://ty.panjiajie.cn

[U112] JS：字符串补位
来源：http://xb.yuntaijiaju.cn

"7".padStart(3, "0")
来源：http://oi.wgjwhj.cn

[U113] JS：正则替换全部
来源：http://er.jctech888.com.cn

s.replaceAll("a", "b")
来源：http://cw.shtwfgs.cn

[U114] JS：JSON 深比较
来源：http://jc.jctech888.com.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://bc.shxzskj.cn

[U115] JS：生成 UUID
来源：http://vk.chemitech.net.cn

crypto.randomUUID()
来源：http://xt.szxytkj.cn

[U116] JS：类型检查（JSDoc）
来源：http://kx.9csxet.cn

/** @param {string} name */ function f(name) {}
来源：http://vt.jctech888.com.cn


<!-- 参考信息 -->