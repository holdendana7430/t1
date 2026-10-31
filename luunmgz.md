代发 wailian999

[T25] Swift：结构体
来源：http://qh.jctech888.com.cn

struct P { var x: Int }
来源：http://lz.nszjky.cn

[T26] Swift：类与重写
来源：http://mj.bookmarksfly.cn

class A: Base { override func f() {} }
来源：http://xc.yuexingan06.cn

[T27] Swift：错误处理
来源：http://lf.asd995.cn

do { try f() } catch { print(error) }
来源：http://kb.hnjuh.cn

[T28] Swift：枚举
来源：http://bk.521024.cn

enum Color { case red, green }
来源：http://hf.shxzukj.cn

[T29] Swift：guard 提前返回
来源：http://iq.newstarts.cn

guard let x = opt else { return }
来源：http://ib.huanxung.cn

[T30] Swift：协议
来源：http://ga.szxytkj.cn

protocol Shape { func area() -> Double }
来源：http://dc.gzmigu.cn

[T31] Lua：Hello World
来源：http://wj.gzmigu.cn

print("Hello")
来源：http://gx.nicolike.cn

[T32] Lua：局部变量
来源：http://yp.huixinmuqiang.cn

local a = 1
来源：http://je.bjjhwx.cn

[T33] Lua：表（数组）
来源：http://ib.shxzskj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://yn.panjiajie.cn

[T34] Lua：遍历表
来源：http://vx.shxzskj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://xw.panjiajie.cn

[T35] Lua：字典表
来源：http://jt.newstarts.cn

local d = { a = 1 };  d.b = 2
来源：http://ld.yuexingan06.cn

[T36] Lua：函数
来源：http://qq.shxzukj.cn

function add(a, b) return a + b end
来源：http://ip.bjjhwx.cn

[T37] Lua：字符串拼接
来源：http://zw.shxzskj.cn

"a" .. "b"
来源：http://zu.521024.cn

[T38] Lua：条件
来源：http://lc.bookmarksfly.cn

if x > 0 then print("正") end
来源：http://jh.szsharing.cn

[T39] Lua：模式匹配
来源：http://pl.gzmigu.cn

string.find(s, "%d+")
来源：http://tx.hahajie.cn

[T40] Lua：元表
来源：http://kq.huixinmuqiang.cn

setmetatable({}, { __index = base })
来源：http://cx.nszjky.cn

[T41] Perl：Hello World
来源：http://ib.yuntaijiaju.cn

print "Hello\n";
来源：http://cu.wgjwhj.cn

[T42] Perl：变量类型
来源：http://hq.nicolike.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://im.chemitech.net.cn

[T43] Perl：字符串插值
来源：http://ls.jianghongdianzi.cn

"值: $a"
来源：http://kb.shtwfgs.cn

[T44] Perl：条件
来源：http://kn.lnxyls.cn

if ($a > 0) { print "正"; }
来源：http://vt.asd995.cn

[T45] Perl：数组遍历
来源：http://bk.nicolike.cn

for my $x (@arr) { print $x; }
来源：http://do.nicolike.cn

[T46] Perl：哈希操作
来源：http://ys.huixinmuqiang.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jf.szxytkj.cn

[T47] Perl：正则捕获
来源：http://yh.szxytkj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://uj.hahajie.cn

[T48] Perl：正则替换
来源：http://iy.521024.cn

$s =~ s/old/new/g;
来源：http://zd.bookmarksfly.cn

[T49] Perl：函数
来源：http://ra.huixiangedu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xi.shxzukj.cn

[T50] Perl：逐行读文件
来源：http://rd.hahajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://tx.bjjhwx.cn

while (my $line = <$fh>) { print $line; }
来源：http://bc.hahajie.cn

[T51] Scala：Hello World
来源：http://uf.hnjuh.cn

println("Hello")
来源：http://tx.bjjhwx.cn

[T52] Scala：变量
来源：http://ue.panjiajie.cn

val a = 1;  var b = 2
来源：http://pl.hnjuh.cn

[T53] Scala：字符串插值
来源：http://ai.jianghongdianzi.cn

s"值: $b"
来源：http://zk.9csxet.cn

[T54] Scala：集合映射
来源：http://we.9csxet.cn

List(1, 2, 3).map(_ * 2)
来源：http://nz.shtwfgs.cn

[T55] Scala：集合过滤
来源：http://xp.jctech888.com.cn

List(1, 2, 3).filter(_ > 1)
来源：http://vk.9csxet.cn

[T56] Scala：样例类
来源：http://hi.nszjky.cn

case class User(name: String, age: Int)
来源：http://qk.521024.cn

[T57] Scala：模式匹配
来源：http://xq.hahajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vh.yuntaijiaju.cn

[T58] Scala：函数定义
来源：http://lv.jctech888.com.cn

def add(a: Int, b: Int): Int = a + b
来源：http://dk.newstarts.cn

[T59] Scala：循环
来源：http://ln.newstarts.cn

for (i <- 1 to 10) println(i)
来源：http://gj.szsharing.cn

[T60] Scala：折叠
来源：http://zv.szxytkj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rc.huanxung.cn

================================================================================
来源：http://bx.szxytkj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hs.jianghongdianzi.cn

================================================================================
来源：http://ok.wgjwhj.cn

[U01] Py：创建虚拟环境
来源：http://ec.shxzukj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://xx.wgjwhj.cn

[U02] Py：导出 / 安装依赖
来源：http://vr.wgjwhj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rv.huixiangedu.cn

[U03] Py：加载 .env 配置
来源：http://qm.newstarts.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://hy.bjjhwx.cn

[U04] Py：变量调试打印
来源：http://qr.colortex.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ka.yuexingan06.cn

[U05] Py：列表去重且保序
来源：http://fu.asd995.cn

list(dict.fromkeys(arr))
来源：http://rx.colortex.cn

[U06] Py：合并两个字典
来源：http://jg.chemitech.net.cn

{**a, **b}
来源：http://fe.shtwfgs.cn

[U07] Py：反转字典键值
来源：http://py.jianghongdianzi.cn

{v: k for k, v in d.items()}
来源：http://os.nszjky.cn

[U08] Py：展平二维列表
来源：http://gd.szsharing.cn

[y for x in nested for y in x]
来源：http://uk.newstarts.cn

[U09] Py：字典取最大值的键
来源：http://ng.nicolike.cn

max(d, key=d.get)
来源：http://zp.shxzskj.cn

[U10] Py：按值排序字典
来源：http://uy.9csxet.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qq.jctech888.com.cn

[U11] Py：生成器表达式
来源：http://rk.muxihuayi.cn

(x * 2 for x in arr)
来源：http://jt.nszjky.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xc.yuntaijiaju.cn

Counter(arr).most_common(3)
来源：http://ty.nicolike.cn

[U13] Py：固定长度队列
来源：http://vy.521024.cn

deque(maxlen=10)
来源：http://nv.bookmarksfly.cn

[U14] Py：分组收集到列表
来源：http://ev.lnxyls.cn

defaultdict(list)
来源：http://gn.wgjwhj.cn

[U15] Py：高精度计时
来源：http://nx.lnxyls.cn

t = time.perf_counter()
来源：http://yh.huixinmuqiang.cn

[U16] Py：命令行参数解析
来源：http://mc.colortex.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://il.bjjhwx.cn

[U17] Py：初始化日志
来源：http://bn.521024.cn

logging.basicConfig(level=logging.INFO)
来源：http://an.hahajie.cn

[U18] Py：预编译正则
来源：http://ht.chemitech.net.cn

pat = re.compile(r"\d+")
来源：http://hl.newstarts.cn

[U19] Py：正则替换带回调
来源：http://ol.newstarts.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bs.haigaiapp.cn

[U20] Py：缓存函数结果
来源：http://kj.colortex.cn

@functools.lru_cache(maxsize=None)
来源：http://er.lnxyls.cn

[U21] Py：自定义上下文管理器
来源：http://vz.jianghongdianzi.cn

@contextlib.contextmanager
来源：http://rz.bookmarksfly.cn

[U22] Py：矩阵转置
来源：http://ic.szsharing.cn

list(zip(*m))
来源：http://vp.yuexingan06.cn

[U23] Py：分块读取大文件
来源：http://si.chemitech.net.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ja.nszjky.cn

[U24] Py：路径操作
来源：http://jx.panjiajie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ik.colortex.cn

[U25] Py：CSV 按字典读
来源：http://lg.jianghongdianzi.cn

csv.DictReader(f)
来源：http://xd.bjjhwx.cn

[U26] Py：并发下载
来源：http://gp.nicolike.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://sa.jctech888.com.cn

[U27] Py：异步 HTTP
来源：http://qu.lnxyls.cn

aiohttp.ClientSession() 配合 async with
来源：http://wa.szxytkj.cn

[U28] Py：类型别名
来源：http://eu.haigaiapp.cn

UserId = int
来源：http://uv.huixiangedu.cn

[U29] Py：属性校验
来源：http://bj.chemitech.net.cn

@property 与 @x.setter 配合
来源：http://zg.lnxyls.cn

[U30] Py：数据类
来源：http://aw.hnjuh.cn

@dataclass(slots=True)
来源：http://bt.muxihuayi.cn

[U31] Py：单测
来源：http://ux.gzmigu.cn

python -m pytest -q
来源：http://di.huixinmuqiang.cn

[U32] Py：代码格式化
来源：http://pm.huixiangedu.cn

ruff format . && ruff check --fix .
来源：http://vn.yuntaijiaju.cn

[U33] Py：打包发布
来源：http://dw.lnxyls.cn

python -m build  （依赖 pyproject.toml）
来源：http://bu.shxzukj.cn

[U34] Py：判断编码
来源：http://ub.haigaiapp.cn

chardet.detect(raw)
来源：http://rc.nszjky.cn

[U35] Py：发送邮件
来源：http://fy.jctech888.com.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tk.521024.cn

[U36] Py：定时任务
来源：http://kp.lnxyls.cn

schedule.every(10).minutes.do(job)
来源：http://hw.nicolike.cn

[U37] Py：读写 Excel
来源：http://fb.shtwfgs.cn

pandas.read_excel / DataFrame.to_excel
来源：http://sn.haigaiapp.cn

[U38] Py：获取脚本所在目录
来源：http://ra.gzmigu.cn

Path(__file__).resolve().parent
来源：http://pc.shxzukj.cn

[U39] Py：判断是否在交互环境
来源：http://sa.chemitech.net.cn

sys.stdout.isatty()
来源：http://dv.nicolike.cn

[U40] Py：打印到标准错误
来源：http://ud.huixiangedu.cn

print("err", file=sys.stderr)
来源：http://gp.shxzskj.cn

[U41] PHP：初始化 Composer 项目
来源：http://oi.hahajie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://nz.panjiajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://oz.hnjuh.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://is.szsharing.cn

[U43] PHP：声明命名空间
来源：http://fj.yuexingan06.cn

namespace App\Http;
来源：http://gt.nicolike.cn

[U44] PHP：开启严格类型
来源：http://ks.jctech888.com.cn

declare(strict_types=1);
来源：http://qj.colortex.cn

[U45] PHP：类型声明与返回类型
来源：http://jk.yuntaijiaju.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://rc.hnjuh.cn

[U46] PHP：可空类型
来源：http://dt.yuntaijiaju.cn

?string $name = null
来源：http://of.bjjhwx.cn

[U47] PHP：联合类型
来源：http://ry.haigaiapp.cn

int|string $id
来源：http://xi.shtwfgs.cn

[U48] PHP：纯枚举
来源：http://zp.szsharing.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ds.colortex.cn

[U49] PHP：只读属性
来源：http://tf.chemitech.net.cn

public readonly string $name
来源：http://jt.wgjwhj.cn

[U50] PHP：构造器属性提升
来源：http://fl.szxytkj.cn

public function __construct(private int $id) {}
来源：http://if.muxihuayi.cn

[U51] PHP：数组解构
来源：http://fq.yuexingan06.cn

[$a, $b] = $arr;
来源：http://ct.jianghongdianzi.cn

[U52] PHP：箭头函数
来源：http://no.newstarts.cn

$double = fn($x) => $x * 2;
来源：http://tm.jianghongdianzi.cn

[U53] PHP：空合并运算符
来源：http://nt.nicolike.cn

$v = $a ?? $b ?? "default";
来源：http://vx.9csxet.cn

[U54] PHP：空安全调用
来源：http://uq.colortex.cn

$obj?->method()
来源：http://sb.huixiangedu.cn

[U55] PHP：match 表达式
来源：http://qd.shxzukj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xq.9csxet.cn

[U56] PHP：命名参数
来源：http://bc.hahajie.cn

f(a: 1, b: 2)
来源：http://re.nszjky.cn

[U57] PHP：字符串插值
来源：http://fd.haigaiapp.cn

"值: {$a}"
来源：http://ez.bookmarksfly.cn

[U58] PHP：数组三件套
来源：http://dm.szxytkj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xu.muxihuayi.cn

[U59] PHP：自定义排序
来源：http://mm.wgjwhj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dl.nicolike.cn

[U60] PHP：JSON 编解码
来源：http://vm.huixinmuqiang.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://do.szsharing.cn

[U61] PHP：正则
来源：http://ya.colortex.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ah.szsharing.cn

[U62] PHP：日期对象
来源：http://oh.huanxung.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ca.hnjuh.cn

[U63] PHP：文件读写
来源：http://yu.haigaiapp.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xi.panjiajie.cn

[U64] PHP：目录遍历
来源：http://ay.nszjky.cn

glob("dir/*.php");  scandir("dir");
来源：http://sh.9csxet.cn

[U65] PHP：会话
来源：http://xl.shxzskj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://sj.hnjuh.cn

[U66] PHP：设置 Cookie
来源：http://aj.colortex.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nu.haigaiapp.cn

[U67] PHP：处理文件上传
来源：http://hx.szsharing.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pq.gzmigu.cn

[U68] PHP：PDO 连接
来源：http://nv.newstarts.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nx.shxzukj.cn

[U69] PHP：PDO 预处理
来源：http://nv.huixiangedu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ps.wgjwhj.cn

[U70] PHP：PDO 事务
来源：http://bi.hahajie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kz.hnjuh.cn

[U71] PHP：抛出异常
来源：http://vh.jianghongdianzi.cn

throw new RuntimeException("失败", 500);
来源：http://la.asd995.cn

[U72] PHP：写错误日志
来源：http://rj.newstarts.cn

error_log("失败: " . $e->getMessage());
来源：http://yk.shtwfgs.cn

[U73] PHP：读取 ini 配置
来源：http://er.9csxet.cn

parse_ini_file("config.ini", true)
来源：http://uj.jctech888.com.cn

[U74] PHP：读取环境变量
来源：http://cs.gzmigu.cn

getenv("APP_ENV") ?: "production"
来源：http://fr.yuntaijiaju.cn

[U75] PHP：依赖注入
来源：http://qs.shxzukj.cn

composer require psr/container
来源：http://eu.lnxyls.cn

[U76] PHP：简单路由
来源：http://bt.panjiajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://we.bjjhwx.cn

[U77] PHP：模板渲染
来源：http://wh.szsharing.cn

composer require twig/twig
来源：http://ss.huixinmuqiang.cn

[U78] PHP：单元测试
来源：http://km.jianghongdianzi.cn

composer require --dev phpunit/phpunit
来源：http://fg.hnjuh.cn

[U79] PHP：静态分析
来源：http://dd.hnjuh.cn

composer require --dev phpstan/phpstan
来源：http://vk.haigaiapp.cn

[U80] PHP：代码规范修复
来源：http://gs.chemitech.net.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xa.szsharing.cn

[U81] JS：初始化项目
来源：http://dz.hnjuh.cn

npm init -y;  npm i express
来源：http://vj.shtwfgs.cn

[U82] JS：package.json 脚本
来源：http://if.lnxyls.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pk.asd995.cn

[U83] JS：ES Module 导入导出
来源：http://fg.huixinmuqiang.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ue.huixiangedu.cn

[U84] JS：CommonJS 写法
来源：http://lw.huixiangedu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://qi.shtwfgs.cn

[U85] JS：可选链
来源：http://id.shtwfgs.cn

a?.b?.c
来源：http://ir.shxzskj.cn

[U86] JS：空值合并
来源：http://zv.chemitech.net.cn

a ?? b
来源：http://mt.jctech888.com.cn

[U87] JS：解构默认值
来源：http://dj.nicolike.cn

const { a = 1, b = 2 } = obj;
来源：http://ck.9csxet.cn

[U88] JS：对象展开合并
来源：http://ee.lnxyls.cn

{ ...a, ...b }
来源：http://ok.huanxung.cn

[U89] JS：数组去重
来源：http://gy.shxzskj.cn

[...new Set(arr)]
来源：http://yr.haigaiapp.cn

[U90] JS：数字数组排序
来源：http://bo.nszjky.cn

[...arr].sort((a, b) => a - b)
来源：http://ua.9csxet.cn

[U91] JS：对象键值遍历
来源：http://zv.wgjwhj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://td.yuexingan06.cn

[U92] JS：深拷贝
来源：http://rf.hnjuh.cn

structuredClone(obj)
来源：http://mk.gzmigu.cn

[U93] JS：模板字符串
来源：http://vb.huanxung.cn

`共 ${n} 条`
来源：http://yo.lnxyls.cn

[U94] JS：箭头函数
来源：http://fv.nicolike.cn

const double = x => x * 2;
来源：http://cn.yuexingan06.cn

[U95] JS：Promise 包装
来源：http://sj.huixiangedu.cn

new Promise((resolve, reject) => {})
来源：http://oh.shxzukj.cn

[U96] JS：async/await 与异常
来源：http://rk.gzmigu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dz.9csxet.cn

[U97] JS：并发请求
来源：http://qk.hnjuh.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://lu.shtwfgs.cn

[U98] JS：fetch 带 JSON
来源：http://mo.huixinmuqiang.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rx.nicolike.cn

[U99] JS：事件监听
来源：http://no.panjiajie.cn

el.addEventListener("click", e => {})
来源：http://pq.huixiangedu.cn

[U100] JS：DOM 查询
来源：http://yf.shxzukj.cn

document.querySelector(".item")
来源：http://oq.asd995.cn

[U101] JS：classList 操作
来源：http://qf.muxihuayi.cn

el.classList.toggle("active")
来源：http://hc.huanxung.cn

[U102] JS：本地存储
来源：http://ec.newstarts.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://rp.bjjhwx.cn

[U103] JS：定时器
来源：http://bl.haigaiapp.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ul.wgjwhj.cn

[U104] JS：防抖
来源：http://dp.szsharing.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vq.huanxung.cn

[U105] JS：节流
来源：http://ba.yuntaijiaju.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hy.bookmarksfly.cn

[U106] JS：日期格式化
来源：http://ls.bookmarksfly.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lb.huanxung.cn

[U107] JS：数字千分位
来源：http://hz.muxihuayi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dc.bjjhwx.cn

[U108] JS：随机整数
来源：http://oh.huixiangedu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hp.bookmarksfly.cn

[U109] JS：数组分组
来源：http://jd.yuntaijiaju.cn

Object.groupBy(arr, x => x.type)
来源：http://yw.jctech888.com.cn

[U110] JS：数组分块
来源：http://ky.hnjuh.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xq.hnjuh.cn

[U111] JS：对象转 Map
来源：http://nu.yuntaijiaju.cn

new Map(Object.entries(obj))
来源：http://jk.huixinmuqiang.cn

[U112] JS：字符串补位
来源：http://uk.szsharing.cn

"7".padStart(3, "0")
来源：http://gr.huanxung.cn


<!-- 参考信息 -->