代发 wailian999

[T33] Lua：表（数组）
来源：http://xi.newstarts.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xv.huixiangedu.cn

[T34] Lua：遍历表
来源：http://he.huanxung.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://fy.bjjhwx.cn

[T35] Lua：字典表
来源：http://nv.jctech888.com.cn

local d = { a = 1 };  d.b = 2
来源：http://jz.9csxet.cn

[T36] Lua：函数
来源：http://wb.yuexingan06.cn

function add(a, b) return a + b end
来源：http://mv.colortex.cn

[T37] Lua：字符串拼接
来源：http://vg.bookmarksfly.cn

"a" .. "b"
来源：http://zd.szsharing.cn

[T38] Lua：条件
来源：http://si.panjiajie.cn

if x > 0 then print("正") end
来源：http://ys.shtwfgs.cn

[T39] Lua：模式匹配
来源：http://lz.chemitech.net.cn

string.find(s, "%d+")
来源：http://zi.yuexingan06.cn

[T40] Lua：元表
来源：http://wp.colortex.cn

setmetatable({}, { __index = base })
来源：http://cr.lnxyls.cn

[T41] Perl：Hello World
来源：http://ht.jctech888.com.cn

print "Hello\n";
来源：http://tv.chemitech.net.cn

[T42] Perl：变量类型
来源：http://ei.yuntaijiaju.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mt.haigaiapp.cn

[T43] Perl：字符串插值
来源：http://vl.521024.cn

"值: $a"
来源：http://mu.gzmigu.cn

[T44] Perl：条件
来源：http://xc.haigaiapp.cn

if ($a > 0) { print "正"; }
来源：http://ho.shtwfgs.cn

[T45] Perl：数组遍历
来源：http://hm.gzmigu.cn

for my $x (@arr) { print $x; }
来源：http://md.panjiajie.cn

[T46] Perl：哈希操作
来源：http://xo.wgjwhj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gn.9csxet.cn

[T47] Perl：正则捕获
来源：http://rj.huixiangedu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://sc.gzmigu.cn

[T48] Perl：正则替换
来源：http://ds.asd995.cn

$s =~ s/old/new/g;
来源：http://hj.huanxung.cn

[T49] Perl：函数
来源：http://tt.jctech888.com.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hd.haigaiapp.cn

[T50] Perl：逐行读文件
来源：http://do.yuexingan06.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://yq.newstarts.cn

while (my $line = <$fh>) { print $line; }
来源：http://zz.haigaiapp.cn

[T51] Scala：Hello World
来源：http://oa.jianghongdianzi.cn

println("Hello")
来源：http://oo.huanxung.cn

[T52] Scala：变量
来源：http://be.bookmarksfly.cn

val a = 1;  var b = 2
来源：http://ng.colortex.cn

[T53] Scala：字符串插值
来源：http://sr.colortex.cn

s"值: $b"
来源：http://pu.hahajie.cn

[T54] Scala：集合映射
来源：http://kv.9csxet.cn

List(1, 2, 3).map(_ * 2)
来源：http://mj.yuntaijiaju.cn

[T55] Scala：集合过滤
来源：http://tl.colortex.cn

List(1, 2, 3).filter(_ > 1)
来源：http://mj.jianghongdianzi.cn

[T56] Scala：样例类
来源：http://ro.chemitech.net.cn

case class User(name: String, age: Int)
来源：http://jt.yuntaijiaju.cn

[T57] Scala：模式匹配
来源：http://up.nszjky.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://jt.newstarts.cn

[T58] Scala：函数定义
来源：http://nm.shxzukj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://do.asd995.cn

[T59] Scala：循环
来源：http://oo.szsharing.cn

for (i <- 1 to 10) println(i)
来源：http://ga.chemitech.net.cn

[T60] Scala：折叠
来源：http://sf.muxihuayi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mj.lnxyls.cn

================================================================================
来源：http://qs.shxzukj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ai.haigaiapp.cn

================================================================================
来源：http://iz.shxzskj.cn

[U01] Py：创建虚拟环境
来源：http://yf.haigaiapp.cn

python -m venv .venv && source .venv/bin/activate
来源：http://su.hnjuh.cn

[U02] Py：导出 / 安装依赖
来源：http://fs.9csxet.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://sm.szxytkj.cn

[U03] Py：加载 .env 配置
来源：http://lk.chemitech.net.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://dn.shxzukj.cn

[U04] Py：变量调试打印
来源：http://id.9csxet.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://su.newstarts.cn

[U05] Py：列表去重且保序
来源：http://za.chemitech.net.cn

list(dict.fromkeys(arr))
来源：http://be.bookmarksfly.cn

[U06] Py：合并两个字典
来源：http://om.colortex.cn

{**a, **b}
来源：http://ms.gzmigu.cn

[U07] Py：反转字典键值
来源：http://dj.shtwfgs.cn

{v: k for k, v in d.items()}
来源：http://cb.hahajie.cn

[U08] Py：展平二维列表
来源：http://bf.hnjuh.cn

[y for x in nested for y in x]
来源：http://ux.panjiajie.cn

[U09] Py：字典取最大值的键
来源：http://bo.szsharing.cn

max(d, key=d.get)
来源：http://sa.yuexingan06.cn

[U10] Py：按值排序字典
来源：http://et.bjjhwx.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wt.wgjwhj.cn

[U11] Py：生成器表达式
来源：http://fo.shxzskj.cn

(x * 2 for x in arr)
来源：http://fs.gzmigu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://eq.521024.cn

Counter(arr).most_common(3)
来源：http://ql.bjjhwx.cn

[U13] Py：固定长度队列
来源：http://jp.huixinmuqiang.cn

deque(maxlen=10)
来源：http://xs.521024.cn

[U14] Py：分组收集到列表
来源：http://zo.nszjky.cn

defaultdict(list)
来源：http://gl.huanxung.cn

[U15] Py：高精度计时
来源：http://fx.9csxet.cn

t = time.perf_counter()
来源：http://lb.yuntaijiaju.cn

[U16] Py：命令行参数解析
来源：http://pd.bookmarksfly.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ml.shxzskj.cn

[U17] Py：初始化日志
来源：http://bj.wgjwhj.cn

logging.basicConfig(level=logging.INFO)
来源：http://ie.huixiangedu.cn

[U18] Py：预编译正则
来源：http://dc.szxytkj.cn

pat = re.compile(r"\d+")
来源：http://wo.yuntaijiaju.cn

[U19] Py：正则替换带回调
来源：http://ur.bookmarksfly.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mi.panjiajie.cn

[U20] Py：缓存函数结果
来源：http://dm.shtwfgs.cn

@functools.lru_cache(maxsize=None)
来源：http://kk.hnjuh.cn

[U21] Py：自定义上下文管理器
来源：http://gw.huixinmuqiang.cn

@contextlib.contextmanager
来源：http://to.szsharing.cn

[U22] Py：矩阵转置
来源：http://vf.hnjuh.cn

list(zip(*m))
来源：http://rv.hahajie.cn

[U23] Py：分块读取大文件
来源：http://it.lnxyls.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rj.nicolike.cn

[U24] Py：路径操作
来源：http://vb.nszjky.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://to.nszjky.cn

[U25] Py：CSV 按字典读
来源：http://ao.muxihuayi.cn

csv.DictReader(f)
来源：http://fr.gzmigu.cn

[U26] Py：并发下载
来源：http://qg.bjjhwx.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kr.bjjhwx.cn

[U27] Py：异步 HTTP
来源：http://hp.nicolike.cn

aiohttp.ClientSession() 配合 async with
来源：http://zj.bookmarksfly.cn

[U28] Py：类型别名
来源：http://aj.hahajie.cn

UserId = int
来源：http://we.szsharing.cn

[U29] Py：属性校验
来源：http://vk.colortex.cn

@property 与 @x.setter 配合
来源：http://md.yuntaijiaju.cn

[U30] Py：数据类
来源：http://td.bookmarksfly.cn

@dataclass(slots=True)
来源：http://pq.shtwfgs.cn

[U31] Py：单测
来源：http://dz.nicolike.cn

python -m pytest -q
来源：http://ej.szxytkj.cn

[U32] Py：代码格式化
来源：http://ss.newstarts.cn

ruff format . && ruff check --fix .
来源：http://uc.szsharing.cn

[U33] Py：打包发布
来源：http://fz.jianghongdianzi.cn

python -m build  （依赖 pyproject.toml）
来源：http://zw.panjiajie.cn

[U34] Py：判断编码
来源：http://nb.bookmarksfly.cn

chardet.detect(raw)
来源：http://pp.colortex.cn

[U35] Py：发送邮件
来源：http://vn.521024.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qn.shtwfgs.cn

[U36] Py：定时任务
来源：http://jt.521024.cn

schedule.every(10).minutes.do(job)
来源：http://mo.yuntaijiaju.cn

[U37] Py：读写 Excel
来源：http://kv.bookmarksfly.cn

pandas.read_excel / DataFrame.to_excel
来源：http://lr.huanxung.cn

[U38] Py：获取脚本所在目录
来源：http://pe.yuexingan06.cn

Path(__file__).resolve().parent
来源：http://ts.hnjuh.cn

[U39] Py：判断是否在交互环境
来源：http://lo.shxzukj.cn

sys.stdout.isatty()
来源：http://vo.lnxyls.cn

[U40] Py：打印到标准错误
来源：http://hz.bookmarksfly.cn

print("err", file=sys.stderr)
来源：http://xg.huixiangedu.cn

[U41] PHP：初始化 Composer 项目
来源：http://kz.bookmarksfly.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ey.newstarts.cn

[U42] PHP：PSR-4 自动加载
来源：http://au.jianghongdianzi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://se.521024.cn

[U43] PHP：声明命名空间
来源：http://zx.shxzukj.cn

namespace App\Http;
来源：http://zv.shtwfgs.cn

[U44] PHP：开启严格类型
来源：http://cn.yuntaijiaju.cn

declare(strict_types=1);
来源：http://vz.shtwfgs.cn

[U45] PHP：类型声明与返回类型
来源：http://rz.wgjwhj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://tg.yuntaijiaju.cn

[U46] PHP：可空类型
来源：http://kr.shxzskj.cn

?string $name = null
来源：http://uy.huanxung.cn

[U47] PHP：联合类型
来源：http://gr.muxihuayi.cn

int|string $id
来源：http://md.panjiajie.cn

[U48] PHP：纯枚举
来源：http://up.colortex.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://iu.9csxet.cn

[U49] PHP：只读属性
来源：http://uf.muxihuayi.cn

public readonly string $name
来源：http://qx.wgjwhj.cn

[U50] PHP：构造器属性提升
来源：http://mt.huixiangedu.cn

public function __construct(private int $id) {}
来源：http://he.newstarts.cn

[U51] PHP：数组解构
来源：http://wg.yuexingan06.cn

[$a, $b] = $arr;
来源：http://am.jianghongdianzi.cn

[U52] PHP：箭头函数
来源：http://wr.shxzskj.cn

$double = fn($x) => $x * 2;
来源：http://dk.newstarts.cn

[U53] PHP：空合并运算符
来源：http://dl.szxytkj.cn

$v = $a ?? $b ?? "default";
来源：http://ys.bjjhwx.cn

[U54] PHP：空安全调用
来源：http://zl.yuexingan06.cn

$obj?->method()
来源：http://xu.muxihuayi.cn

[U55] PHP：match 表达式
来源：http://hx.muxihuayi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://na.huixinmuqiang.cn

[U56] PHP：命名参数
来源：http://pz.panjiajie.cn

f(a: 1, b: 2)
来源：http://tb.wgjwhj.cn

[U57] PHP：字符串插值
来源：http://io.yuntaijiaju.cn

"值: {$a}"
来源：http://im.huixinmuqiang.cn

[U58] PHP：数组三件套
来源：http://ey.haigaiapp.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pc.yuexingan06.cn

[U59] PHP：自定义排序
来源：http://bh.muxihuayi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bw.newstarts.cn

[U60] PHP：JSON 编解码
来源：http://cz.shxzskj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qr.yuntaijiaju.cn

[U61] PHP：正则
来源：http://vb.chemitech.net.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ia.huanxung.cn

[U62] PHP：日期对象
来源：http://nh.chemitech.net.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qe.hnjuh.cn

[U63] PHP：文件读写
来源：http://pk.shxzskj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mm.panjiajie.cn

[U64] PHP：目录遍历
来源：http://rl.jctech888.com.cn

glob("dir/*.php");  scandir("dir");
来源：http://qp.521024.cn

[U65] PHP：会话
来源：http://ca.szxytkj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://qo.9csxet.cn

[U66] PHP：设置 Cookie
来源：http://gk.521024.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bo.shxzukj.cn

[U67] PHP：处理文件上传
来源：http://kg.szsharing.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wc.asd995.cn

[U68] PHP：PDO 连接
来源：http://zq.panjiajie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yq.nszjky.cn

[U69] PHP：PDO 预处理
来源：http://yo.wgjwhj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lx.haigaiapp.cn

[U70] PHP：PDO 事务
来源：http://rx.panjiajie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ii.9csxet.cn

[U71] PHP：抛出异常
来源：http://ww.newstarts.cn

throw new RuntimeException("失败", 500);
来源：http://as.9csxet.cn

[U72] PHP：写错误日志
来源：http://nc.shxzskj.cn

error_log("失败: " . $e->getMessage());
来源：http://zz.yuntaijiaju.cn

[U73] PHP：读取 ini 配置
来源：http://ss.huanxung.cn

parse_ini_file("config.ini", true)
来源：http://vo.colortex.cn

[U74] PHP：读取环境变量
来源：http://xw.szxytkj.cn

getenv("APP_ENV") ?: "production"
来源：http://ik.asd995.cn

[U75] PHP：依赖注入
来源：http://vn.9csxet.cn

composer require psr/container
来源：http://et.bjjhwx.cn

[U76] PHP：简单路由
来源：http://nx.bjjhwx.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://it.haigaiapp.cn

[U77] PHP：模板渲染
来源：http://wu.bjjhwx.cn

composer require twig/twig
来源：http://qm.wgjwhj.cn

[U78] PHP：单元测试
来源：http://ak.nicolike.cn

composer require --dev phpunit/phpunit
来源：http://cp.szsharing.cn

[U79] PHP：静态分析
来源：http://oc.521024.cn

composer require --dev phpstan/phpstan
来源：http://iy.nicolike.cn

[U80] PHP：代码规范修复
来源：http://wl.huixiangedu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://rt.chemitech.net.cn

[U81] JS：初始化项目
来源：http://yv.muxihuayi.cn

npm init -y;  npm i express
来源：http://wo.hahajie.cn

[U82] JS：package.json 脚本
来源：http://dy.wgjwhj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cu.huixinmuqiang.cn

[U83] JS：ES Module 导入导出
来源：http://uh.jianghongdianzi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://uy.hnjuh.cn

[U84] JS：CommonJS 写法
来源：http://fy.bookmarksfly.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ta.huanxung.cn

[U85] JS：可选链
来源：http://et.wgjwhj.cn

a?.b?.c
来源：http://ng.hahajie.cn

[U86] JS：空值合并
来源：http://nl.huixiangedu.cn

a ?? b
来源：http://ya.huanxung.cn

[U87] JS：解构默认值
来源：http://dg.huixinmuqiang.cn

const { a = 1, b = 2 } = obj;
来源：http://cv.szxytkj.cn

[U88] JS：对象展开合并
来源：http://ds.shxzskj.cn

{ ...a, ...b }
来源：http://ni.haigaiapp.cn

[U89] JS：数组去重
来源：http://mi.shtwfgs.cn

[...new Set(arr)]
来源：http://iw.haigaiapp.cn

[U90] JS：数字数组排序
来源：http://fl.hnjuh.cn

[...arr].sort((a, b) => a - b)
来源：http://zs.huixinmuqiang.cn

[U91] JS：对象键值遍历
来源：http://pp.bookmarksfly.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://id.asd995.cn

[U92] JS：深拷贝
来源：http://zh.yuexingan06.cn

structuredClone(obj)
来源：http://fi.colortex.cn

[U93] JS：模板字符串
来源：http://bv.huixiangedu.cn

`共 ${n} 条`
来源：http://hw.jctech888.com.cn

[U94] JS：箭头函数
来源：http://ed.gzmigu.cn

const double = x => x * 2;
来源：http://id.chemitech.net.cn

[U95] JS：Promise 包装
来源：http://cq.huanxung.cn

new Promise((resolve, reject) => {})
来源：http://fs.asd995.cn

[U96] JS：async/await 与异常
来源：http://mf.shtwfgs.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tm.yuntaijiaju.cn

[U97] JS：并发请求
来源：http://xg.yuexingan06.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ih.521024.cn

[U98] JS：fetch 带 JSON
来源：http://jd.wgjwhj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://uk.huixinmuqiang.cn

[U99] JS：事件监听
来源：http://zv.hahajie.cn

el.addEventListener("click", e => {})
来源：http://de.nszjky.cn

[U100] JS：DOM 查询
来源：http://cq.chemitech.net.cn

document.querySelector(".item")
来源：http://tx.wgjwhj.cn

[U101] JS：classList 操作
来源：http://iz.colortex.cn

el.classList.toggle("active")
来源：http://og.hnjuh.cn

[U102] JS：本地存储
来源：http://jg.bookmarksfly.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jn.9csxet.cn

[U103] JS：定时器
来源：http://wa.huixiangedu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nq.bookmarksfly.cn

[U104] JS：防抖
来源：http://wk.nszjky.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qc.huixiangedu.cn

[U105] JS：节流
来源：http://tp.huanxung.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bm.muxihuayi.cn

[U106] JS：日期格式化
来源：http://eg.jctech888.com.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ao.shxzskj.cn

[U107] JS：数字千分位
来源：http://rf.newstarts.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lr.gzmigu.cn

[U108] JS：随机整数
来源：http://tg.huanxung.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ny.huixiangedu.cn

[U109] JS：数组分组
来源：http://fy.yuexingan06.cn

Object.groupBy(arr, x => x.type)
来源：http://vb.shxzukj.cn

[U110] JS：数组分块
来源：http://yi.asd995.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dw.jianghongdianzi.cn

[U111] JS：对象转 Map
来源：http://sw.521024.cn

new Map(Object.entries(obj))
来源：http://ka.hahajie.cn

[U112] JS：字符串补位
来源：http://st.shxzskj.cn

"7".padStart(3, "0")
来源：http://dw.hahajie.cn

[U113] JS：正则替换全部
来源：http://px.huixiangedu.cn

s.replaceAll("a", "b")
来源：http://xm.huanxung.cn

[U114] JS：JSON 深比较
来源：http://xk.szxytkj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://rr.chemitech.net.cn

[U115] JS：生成 UUID
来源：http://da.huixiangedu.cn

crypto.randomUUID()
来源：http://gd.huixiangedu.cn

[U116] JS：类型检查（JSDoc）
来源：http://aq.muxihuayi.cn

/** @param {string} name */ function f(name) {}
来源：http://ao.wgjwhj.cn

[U117] JS：单元测试
来源：http://nb.shxzukj.cn

npm i -D vitest;  npx vitest
来源：http://gq.bjjhwx.cn

[U118] JS：开发服务器
来源：http://kc.bjjhwx.cn

npm i -D vite;  npx vite
来源：http://qw.haigaiapp.cn

[U119] JS：生产构建
来源：http://kn.huixinmuqiang.cn

npx vite build
来源：http://tx.shxzskj.cn

[U120] JS：读取环境变量（Vite）
来源：http://uh.bookmarksfly.cn

import.meta.env.VITE_API_URL
来源：http://le.asd995.cn


<!-- 参考信息 -->