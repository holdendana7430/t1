代发 wailian999

[T25] Swift：结构体
来源：http://eh.huanxung.cn

struct P { var x: Int }
来源：http://dr.jianghongdianzi.cn

[T26] Swift：类与重写
来源：http://jo.hnjuh.cn

class A: Base { override func f() {} }
来源：http://db.newstarts.cn

[T27] Swift：错误处理
来源：http://pm.jianghongdianzi.cn

do { try f() } catch { print(error) }
来源：http://po.yuexingan06.cn

[T28] Swift：枚举
来源：http://ku.wgjwhj.cn

enum Color { case red, green }
来源：http://wu.muxihuayi.cn

[T29] Swift：guard 提前返回
来源：http://co.nicolike.cn

guard let x = opt else { return }
来源：http://zk.huanxung.cn

[T30] Swift：协议
来源：http://qs.nicolike.cn

protocol Shape { func area() -> Double }
来源：http://fs.muxihuayi.cn

[T31] Lua：Hello World
来源：http://ht.yuntaijiaju.cn

print("Hello")
来源：http://bn.nszjky.cn

[T32] Lua：局部变量
来源：http://np.panjiajie.cn

local a = 1
来源：http://pd.hnjuh.cn

[T33] Lua：表（数组）
来源：http://hf.jctech888.com.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ed.huanxung.cn

[T34] Lua：遍历表
来源：http://fa.newstarts.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ac.lnxyls.cn

[T35] Lua：字典表
来源：http://au.jianghongdianzi.cn

local d = { a = 1 };  d.b = 2
来源：http://dj.asd995.cn

[T36] Lua：函数
来源：http://ir.jianghongdianzi.cn

function add(a, b) return a + b end
来源：http://xf.gzmigu.cn

[T37] Lua：字符串拼接
来源：http://kj.hnjuh.cn

"a" .. "b"
来源：http://vh.shtwfgs.cn

[T38] Lua：条件
来源：http://on.wgjwhj.cn

if x > 0 then print("正") end
来源：http://xa.szxytkj.cn

[T39] Lua：模式匹配
来源：http://hk.huixiangedu.cn

string.find(s, "%d+")
来源：http://pa.yuexingan06.cn

[T40] Lua：元表
来源：http://qz.shtwfgs.cn

setmetatable({}, { __index = base })
来源：http://nq.lnxyls.cn

[T41] Perl：Hello World
来源：http://eq.gzmigu.cn

print "Hello\n";
来源：http://uj.wgjwhj.cn

[T42] Perl：变量类型
来源：http://qx.jianghongdianzi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gg.hnjuh.cn

[T43] Perl：字符串插值
来源：http://zk.shtwfgs.cn

"值: $a"
来源：http://pf.lnxyls.cn

[T44] Perl：条件
来源：http://nv.lnxyls.cn

if ($a > 0) { print "正"; }
来源：http://tu.bjjhwx.cn

[T45] Perl：数组遍历
来源：http://xo.shxzukj.cn

for my $x (@arr) { print $x; }
来源：http://hu.jianghongdianzi.cn

[T46] Perl：哈希操作
来源：http://fo.hahajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ai.nicolike.cn

[T47] Perl：正则捕获
来源：http://lf.gzmigu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://oc.colortex.cn

[T48] Perl：正则替换
来源：http://ya.9csxet.cn

$s =~ s/old/new/g;
来源：http://nl.9csxet.cn

[T49] Perl：函数
来源：http://xw.521024.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xw.yuexingan06.cn

[T50] Perl：逐行读文件
来源：http://tv.jianghongdianzi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ds.colortex.cn

while (my $line = <$fh>) { print $line; }
来源：http://tu.chemitech.net.cn

[T51] Scala：Hello World
来源：http://gy.colortex.cn

println("Hello")
来源：http://vu.panjiajie.cn

[T52] Scala：变量
来源：http://vw.huanxung.cn

val a = 1;  var b = 2
来源：http://sn.panjiajie.cn

[T53] Scala：字符串插值
来源：http://fq.huixiangedu.cn

s"值: $b"
来源：http://vk.nszjky.cn

[T54] Scala：集合映射
来源：http://si.huixiangedu.cn

List(1, 2, 3).map(_ * 2)
来源：http://gk.jctech888.com.cn

[T55] Scala：集合过滤
来源：http://lf.wgjwhj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://zo.haigaiapp.cn

[T56] Scala：样例类
来源：http://ql.jctech888.com.cn

case class User(name: String, age: Int)
来源：http://lx.bjjhwx.cn

[T57] Scala：模式匹配
来源：http://mp.szsharing.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fi.yuntaijiaju.cn

[T58] Scala：函数定义
来源：http://sp.wgjwhj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bs.bookmarksfly.cn

[T59] Scala：循环
来源：http://rs.yuexingan06.cn

for (i <- 1 to 10) println(i)
来源：http://hp.bjjhwx.cn

[T60] Scala：折叠
来源：http://ft.hahajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pj.yuexingan06.cn

================================================================================
来源：http://pb.hnjuh.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kv.shxzukj.cn

================================================================================
来源：http://al.colortex.cn

[U01] Py：创建虚拟环境
来源：http://el.wgjwhj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://gn.huixinmuqiang.cn

[U02] Py：导出 / 安装依赖
来源：http://tm.nicolike.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://br.wgjwhj.cn

[U03] Py：加载 .env 配置
来源：http://fh.gzmigu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fa.shtwfgs.cn

[U04] Py：变量调试打印
来源：http://ek.9csxet.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lu.huanxung.cn

[U05] Py：列表去重且保序
来源：http://dr.chemitech.net.cn

list(dict.fromkeys(arr))
来源：http://to.yuexingan06.cn

[U06] Py：合并两个字典
来源：http://os.jctech888.com.cn

{**a, **b}
来源：http://ln.huixinmuqiang.cn

[U07] Py：反转字典键值
来源：http://oq.newstarts.cn

{v: k for k, v in d.items()}
来源：http://lu.yuexingan06.cn

[U08] Py：展平二维列表
来源：http://ov.szsharing.cn

[y for x in nested for y in x]
来源：http://zr.bjjhwx.cn

[U09] Py：字典取最大值的键
来源：http://zd.haigaiapp.cn

max(d, key=d.get)
来源：http://tq.shtwfgs.cn

[U10] Py：按值排序字典
来源：http://is.huixiangedu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uw.panjiajie.cn

[U11] Py：生成器表达式
来源：http://st.nszjky.cn

(x * 2 for x in arr)
来源：http://xb.shtwfgs.cn

[U12] Py：取出现最多的 3 个元素
来源：http://js.huixinmuqiang.cn

Counter(arr).most_common(3)
来源：http://kd.newstarts.cn

[U13] Py：固定长度队列
来源：http://id.huixinmuqiang.cn

deque(maxlen=10)
来源：http://rr.521024.cn

[U14] Py：分组收集到列表
来源：http://nf.lnxyls.cn

defaultdict(list)
来源：http://pu.chemitech.net.cn

[U15] Py：高精度计时
来源：http://ao.9csxet.cn

t = time.perf_counter()
来源：http://vr.panjiajie.cn

[U16] Py：命令行参数解析
来源：http://rw.jctech888.com.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://du.521024.cn

[U17] Py：初始化日志
来源：http://pb.shtwfgs.cn

logging.basicConfig(level=logging.INFO)
来源：http://vu.colortex.cn

[U18] Py：预编译正则
来源：http://xv.gzmigu.cn

pat = re.compile(r"\d+")
来源：http://ki.jianghongdianzi.cn

[U19] Py：正则替换带回调
来源：http://kb.jianghongdianzi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ay.panjiajie.cn

[U20] Py：缓存函数结果
来源：http://pg.nszjky.cn

@functools.lru_cache(maxsize=None)
来源：http://vs.9csxet.cn

[U21] Py：自定义上下文管理器
来源：http://zh.muxihuayi.cn

@contextlib.contextmanager
来源：http://ea.bjjhwx.cn

[U22] Py：矩阵转置
来源：http://il.gzmigu.cn

list(zip(*m))
来源：http://ce.lnxyls.cn

[U23] Py：分块读取大文件
来源：http://ez.hahajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ha.shxzskj.cn

[U24] Py：路径操作
来源：http://eu.nszjky.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qk.colortex.cn

[U25] Py：CSV 按字典读
来源：http://rf.muxihuayi.cn

csv.DictReader(f)
来源：http://lf.panjiajie.cn

[U26] Py：并发下载
来源：http://bb.huanxung.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pm.jctech888.com.cn

[U27] Py：异步 HTTP
来源：http://tt.shtwfgs.cn

aiohttp.ClientSession() 配合 async with
来源：http://wh.yuexingan06.cn

[U28] Py：类型别名
来源：http://vi.panjiajie.cn

UserId = int
来源：http://kg.asd995.cn

[U29] Py：属性校验
来源：http://mt.nicolike.cn

@property 与 @x.setter 配合
来源：http://yr.huixinmuqiang.cn

[U30] Py：数据类
来源：http://te.yuntaijiaju.cn

@dataclass(slots=True)
来源：http://hl.panjiajie.cn

[U31] Py：单测
来源：http://jp.wgjwhj.cn

python -m pytest -q
来源：http://ut.huanxung.cn

[U32] Py：代码格式化
来源：http://qp.hahajie.cn

ruff format . && ruff check --fix .
来源：http://ms.chemitech.net.cn

[U33] Py：打包发布
来源：http://de.huanxung.cn

python -m build  （依赖 pyproject.toml）
来源：http://ku.shxzukj.cn

[U34] Py：判断编码
来源：http://sc.shtwfgs.cn

chardet.detect(raw)
来源：http://my.chemitech.net.cn

[U35] Py：发送邮件
来源：http://it.huixinmuqiang.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pz.szsharing.cn

[U36] Py：定时任务
来源：http://qi.wgjwhj.cn

schedule.every(10).minutes.do(job)
来源：http://fi.haigaiapp.cn

[U37] Py：读写 Excel
来源：http://pe.jianghongdianzi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://mi.panjiajie.cn

[U38] Py：获取脚本所在目录
来源：http://aa.9csxet.cn

Path(__file__).resolve().parent
来源：http://pu.huanxung.cn

[U39] Py：判断是否在交互环境
来源：http://cf.huixinmuqiang.cn

sys.stdout.isatty()
来源：http://jj.huixiangedu.cn

[U40] Py：打印到标准错误
来源：http://iv.haigaiapp.cn

print("err", file=sys.stderr)
来源：http://ke.huixiangedu.cn

[U41] PHP：初始化 Composer 项目
来源：http://tz.panjiajie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xo.colortex.cn

[U42] PHP：PSR-4 自动加载
来源：http://pr.yuntaijiaju.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sl.muxihuayi.cn

[U43] PHP：声明命名空间
来源：http://op.huixinmuqiang.cn

namespace App\Http;
来源：http://tg.gzmigu.cn

[U44] PHP：开启严格类型
来源：http://qm.muxihuayi.cn

declare(strict_types=1);
来源：http://lr.yuntaijiaju.cn

[U45] PHP：类型声明与返回类型
来源：http://se.9csxet.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bx.jianghongdianzi.cn

[U46] PHP：可空类型
来源：http://lu.shxzskj.cn

?string $name = null
来源：http://yp.nicolike.cn

[U47] PHP：联合类型
来源：http://lh.asd995.cn

int|string $id
来源：http://wn.shxzskj.cn

[U48] PHP：纯枚举
来源：http://tn.panjiajie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://si.newstarts.cn

[U49] PHP：只读属性
来源：http://bc.shxzukj.cn

public readonly string $name
来源：http://ff.521024.cn

[U50] PHP：构造器属性提升
来源：http://ks.lnxyls.cn

public function __construct(private int $id) {}
来源：http://zj.haigaiapp.cn

[U51] PHP：数组解构
来源：http://gz.hnjuh.cn

[$a, $b] = $arr;
来源：http://gj.szsharing.cn

[U52] PHP：箭头函数
来源：http://xr.lnxyls.cn

$double = fn($x) => $x * 2;
来源：http://lv.asd995.cn

[U53] PHP：空合并运算符
来源：http://zk.lnxyls.cn

$v = $a ?? $b ?? "default";
来源：http://ji.huanxung.cn

[U54] PHP：空安全调用
来源：http://fa.asd995.cn

$obj?->method()
来源：http://at.bjjhwx.cn

[U55] PHP：match 表达式
来源：http://eu.panjiajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://al.chemitech.net.cn

[U56] PHP：命名参数
来源：http://ea.yuntaijiaju.cn

f(a: 1, b: 2)
来源：http://ql.newstarts.cn

[U57] PHP：字符串插值
来源：http://pq.bjjhwx.cn

"值: {$a}"
来源：http://yd.szxytkj.cn

[U58] PHP：数组三件套
来源：http://ig.nicolike.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wt.lnxyls.cn

[U59] PHP：自定义排序
来源：http://bp.haigaiapp.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kj.asd995.cn

[U60] PHP：JSON 编解码
来源：http://gz.bookmarksfly.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://nh.jianghongdianzi.cn

[U61] PHP：正则
来源：http://zu.chemitech.net.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dp.shxzukj.cn

[U62] PHP：日期对象
来源：http://he.muxihuayi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lm.jctech888.com.cn

[U63] PHP：文件读写
来源：http://ls.shxzukj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://us.hahajie.cn

[U64] PHP：目录遍历
来源：http://qr.yuexingan06.cn

glob("dir/*.php");  scandir("dir");
来源：http://ef.hnjuh.cn

[U65] PHP：会话
来源：http://jp.nicolike.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://pu.huixinmuqiang.cn

[U66] PHP：设置 Cookie
来源：http://rg.yuexingan06.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dd.chemitech.net.cn

[U67] PHP：处理文件上传
来源：http://wj.muxihuayi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://os.huixinmuqiang.cn

[U68] PHP：PDO 连接
来源：http://kr.szxytkj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yj.asd995.cn

[U69] PHP：PDO 预处理
来源：http://bk.huixiangedu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wo.yuntaijiaju.cn

[U70] PHP：PDO 事务
来源：http://cu.9csxet.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wm.shxzskj.cn

[U71] PHP：抛出异常
来源：http://gh.jianghongdianzi.cn

throw new RuntimeException("失败", 500);
来源：http://ok.huixinmuqiang.cn

[U72] PHP：写错误日志
来源：http://ao.asd995.cn

error_log("失败: " . $e->getMessage());
来源：http://bb.hahajie.cn

[U73] PHP：读取 ini 配置
来源：http://ya.huixiangedu.cn

parse_ini_file("config.ini", true)
来源：http://de.newstarts.cn

[U74] PHP：读取环境变量
来源：http://fp.9csxet.cn

getenv("APP_ENV") ?: "production"
来源：http://ip.asd995.cn

[U75] PHP：依赖注入
来源：http://zq.yuntaijiaju.cn

composer require psr/container
来源：http://cf.lnxyls.cn

[U76] PHP：简单路由
来源：http://ml.bjjhwx.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qd.gzmigu.cn

[U77] PHP：模板渲染
来源：http://xc.hnjuh.cn

composer require twig/twig
来源：http://jh.haigaiapp.cn

[U78] PHP：单元测试
来源：http://eo.gzmigu.cn

composer require --dev phpunit/phpunit
来源：http://gk.shtwfgs.cn

[U79] PHP：静态分析
来源：http://qg.jianghongdianzi.cn

composer require --dev phpstan/phpstan
来源：http://bj.jianghongdianzi.cn

[U80] PHP：代码规范修复
来源：http://qy.9csxet.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://je.colortex.cn

[U81] JS：初始化项目
来源：http://oa.newstarts.cn

npm init -y;  npm i express
来源：http://qb.chemitech.net.cn

[U82] JS：package.json 脚本
来源：http://lu.bjjhwx.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://oa.yuexingan06.cn

[U83] JS：ES Module 导入导出
来源：http://iq.nicolike.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xx.9csxet.cn

[U84] JS：CommonJS 写法
来源：http://yd.colortex.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ra.shxzukj.cn

[U85] JS：可选链
来源：http://je.shxzskj.cn

a?.b?.c
来源：http://aj.jianghongdianzi.cn

[U86] JS：空值合并
来源：http://ov.nicolike.cn

a ?? b
来源：http://fc.szxytkj.cn

[U87] JS：解构默认值
来源：http://mm.huixinmuqiang.cn

const { a = 1, b = 2 } = obj;
来源：http://ra.huanxung.cn

[U88] JS：对象展开合并
来源：http://wp.jctech888.com.cn

{ ...a, ...b }
来源：http://lc.yuntaijiaju.cn

[U89] JS：数组去重
来源：http://na.nszjky.cn

[...new Set(arr)]
来源：http://pf.jctech888.com.cn

[U90] JS：数字数组排序
来源：http://qq.nicolike.cn

[...arr].sort((a, b) => a - b)
来源：http://ib.jianghongdianzi.cn

[U91] JS：对象键值遍历
来源：http://bg.colortex.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://oc.huixiangedu.cn

[U92] JS：深拷贝
来源：http://zi.shxzskj.cn

structuredClone(obj)
来源：http://ly.szxytkj.cn

[U93] JS：模板字符串
来源：http://uq.muxihuayi.cn

`共 ${n} 条`
来源：http://kr.szsharing.cn

[U94] JS：箭头函数
来源：http://se.huixinmuqiang.cn

const double = x => x * 2;
来源：http://sw.9csxet.cn

[U95] JS：Promise 包装
来源：http://sq.panjiajie.cn

new Promise((resolve, reject) => {})
来源：http://lg.hnjuh.cn

[U96] JS：async/await 与异常
来源：http://th.nicolike.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lr.yuntaijiaju.cn

[U97] JS：并发请求
来源：http://rb.nszjky.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ow.bookmarksfly.cn

[U98] JS：fetch 带 JSON
来源：http://ob.chemitech.net.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://md.hahajie.cn

[U99] JS：事件监听
来源：http://sq.jctech888.com.cn

el.addEventListener("click", e => {})
来源：http://jy.jctech888.com.cn

[U100] JS：DOM 查询
来源：http://vh.colortex.cn

document.querySelector(".item")
来源：http://ol.521024.cn

[U101] JS：classList 操作
来源：http://vf.gzmigu.cn

el.classList.toggle("active")
来源：http://sl.lnxyls.cn

[U102] JS：本地存储
来源：http://wf.shxzukj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://bp.9csxet.cn

[U103] JS：定时器
来源：http://wp.nszjky.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pu.hahajie.cn

[U104] JS：防抖
来源：http://as.jctech888.com.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sn.nicolike.cn

[U105] JS：节流
来源：http://rq.colortex.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fb.yuexingan06.cn

[U106] JS：日期格式化
来源：http://ut.hnjuh.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://os.panjiajie.cn

[U107] JS：数字千分位
来源：http://ia.gzmigu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kw.521024.cn

[U108] JS：随机整数
来源：http://by.huanxung.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xj.haigaiapp.cn

[U109] JS：数组分组
来源：http://ji.nicolike.cn

Object.groupBy(arr, x => x.type)
来源：http://yo.bjjhwx.cn

[U110] JS：数组分块
来源：http://he.nicolike.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://aw.szxytkj.cn

[U111] JS：对象转 Map
来源：http://ue.hnjuh.cn

new Map(Object.entries(obj))
来源：http://sc.yuntaijiaju.cn

[U112] JS：字符串补位
来源：http://rg.huixiangedu.cn

"7".padStart(3, "0")
来源：http://ia.hnjuh.cn


<!-- 参考信息 -->