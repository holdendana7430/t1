代发 wailian999

[T23] Swift：函数
来源：http://wr.shtwfgs.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tx.bjjhwx.cn

[T24] Swift：闭包
来源：http://xt.huanxung.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://bv.shxzskj.cn

[T25] Swift：结构体
来源：http://oy.jianghongdianzi.cn

struct P { var x: Int }
来源：http://iw.huixinmuqiang.cn

[T26] Swift：类与重写
来源：http://ez.shxzukj.cn

class A: Base { override func f() {} }
来源：http://mk.bookmarksfly.cn

[T27] Swift：错误处理
来源：http://dw.shtwfgs.cn

do { try f() } catch { print(error) }
来源：http://de.huixinmuqiang.cn

[T28] Swift：枚举
来源：http://yv.newstarts.cn

enum Color { case red, green }
来源：http://ap.asd995.cn

[T29] Swift：guard 提前返回
来源：http://kr.szxytkj.cn

guard let x = opt else { return }
来源：http://ga.lnxyls.cn

[T30] Swift：协议
来源：http://qp.shtwfgs.cn

protocol Shape { func area() -> Double }
来源：http://no.bookmarksfly.cn

[T31] Lua：Hello World
来源：http://yg.jctech888.com.cn

print("Hello")
来源：http://os.nicolike.cn

[T32] Lua：局部变量
来源：http://zp.chemitech.net.cn

local a = 1
来源：http://pj.nszjky.cn

[T33] Lua：表（数组）
来源：http://yj.chemitech.net.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ap.bjjhwx.cn

[T34] Lua：遍历表
来源：http://vp.bjjhwx.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://bz.lnxyls.cn

[T35] Lua：字典表
来源：http://zn.newstarts.cn

local d = { a = 1 };  d.b = 2
来源：http://op.9csxet.cn

[T36] Lua：函数
来源：http://by.newstarts.cn

function add(a, b) return a + b end
来源：http://ze.yuexingan06.cn

[T37] Lua：字符串拼接
来源：http://sz.wgjwhj.cn

"a" .. "b"
来源：http://wc.hahajie.cn

[T38] Lua：条件
来源：http://cz.chemitech.net.cn

if x > 0 then print("正") end
来源：http://gk.hahajie.cn

[T39] Lua：模式匹配
来源：http://xy.colortex.cn

string.find(s, "%d+")
来源：http://zz.szsharing.cn

[T40] Lua：元表
来源：http://uc.huanxung.cn

setmetatable({}, { __index = base })
来源：http://in.shxzskj.cn

[T41] Perl：Hello World
来源：http://nc.nszjky.cn

print "Hello\n";
来源：http://iw.huixinmuqiang.cn

[T42] Perl：变量类型
来源：http://av.colortex.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fk.muxihuayi.cn

[T43] Perl：字符串插值
来源：http://lc.yuexingan06.cn

"值: $a"
来源：http://kh.asd995.cn

[T44] Perl：条件
来源：http://cr.asd995.cn

if ($a > 0) { print "正"; }
来源：http://mh.muxihuayi.cn

[T45] Perl：数组遍历
来源：http://po.newstarts.cn

for my $x (@arr) { print $x; }
来源：http://lx.newstarts.cn

[T46] Perl：哈希操作
来源：http://wh.521024.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ze.colortex.cn

[T47] Perl：正则捕获
来源：http://is.huixiangedu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://zj.wgjwhj.cn

[T48] Perl：正则替换
来源：http://ir.huixinmuqiang.cn

$s =~ s/old/new/g;
来源：http://qx.szxytkj.cn

[T49] Perl：函数
来源：http://pt.huixinmuqiang.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fv.shxzskj.cn

[T50] Perl：逐行读文件
来源：http://ri.hnjuh.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://en.jctech888.com.cn

while (my $line = <$fh>) { print $line; }
来源：http://ec.colortex.cn

[T51] Scala：Hello World
来源：http://kv.lnxyls.cn

println("Hello")
来源：http://dd.asd995.cn

[T52] Scala：变量
来源：http://na.panjiajie.cn

val a = 1;  var b = 2
来源：http://nc.huixiangedu.cn

[T53] Scala：字符串插值
来源：http://fh.bjjhwx.cn

s"值: $b"
来源：http://wb.jctech888.com.cn

[T54] Scala：集合映射
来源：http://is.bjjhwx.cn

List(1, 2, 3).map(_ * 2)
来源：http://ky.szsharing.cn

[T55] Scala：集合过滤
来源：http://py.hnjuh.cn

List(1, 2, 3).filter(_ > 1)
来源：http://eo.newstarts.cn

[T56] Scala：样例类
来源：http://ai.huixinmuqiang.cn

case class User(name: String, age: Int)
来源：http://zl.jctech888.com.cn

[T57] Scala：模式匹配
来源：http://pi.shtwfgs.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://lk.huixiangedu.cn

[T58] Scala：函数定义
来源：http://co.colortex.cn

def add(a: Int, b: Int): Int = a + b
来源：http://dm.nszjky.cn

[T59] Scala：循环
来源：http://qf.szsharing.cn

for (i <- 1 to 10) println(i)
来源：http://bk.nszjky.cn

[T60] Scala：折叠
来源：http://qx.panjiajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bd.shxzukj.cn

================================================================================
来源：http://ek.gzmigu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gh.yuexingan06.cn

================================================================================
来源：http://mr.wgjwhj.cn

[U01] Py：创建虚拟环境
来源：http://bp.bookmarksfly.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ub.panjiajie.cn

[U02] Py：导出 / 安装依赖
来源：http://uv.colortex.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mp.lnxyls.cn

[U03] Py：加载 .env 配置
来源：http://ou.shtwfgs.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ak.gzmigu.cn

[U04] Py：变量调试打印
来源：http://ir.huanxung.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bc.jctech888.com.cn

[U05] Py：列表去重且保序
来源：http://xm.szxytkj.cn

list(dict.fromkeys(arr))
来源：http://hw.chemitech.net.cn

[U06] Py：合并两个字典
来源：http://et.bjjhwx.cn

{**a, **b}
来源：http://hm.haigaiapp.cn

[U07] Py：反转字典键值
来源：http://qa.huixiangedu.cn

{v: k for k, v in d.items()}
来源：http://so.bookmarksfly.cn

[U08] Py：展平二维列表
来源：http://np.shtwfgs.cn

[y for x in nested for y in x]
来源：http://as.hahajie.cn

[U09] Py：字典取最大值的键
来源：http://tt.9csxet.cn

max(d, key=d.get)
来源：http://df.nicolike.cn

[U10] Py：按值排序字典
来源：http://fd.huanxung.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cu.colortex.cn

[U11] Py：生成器表达式
来源：http://qa.yuntaijiaju.cn

(x * 2 for x in arr)
来源：http://up.yuntaijiaju.cn

[U12] Py：取出现最多的 3 个元素
来源：http://po.gzmigu.cn

Counter(arr).most_common(3)
来源：http://fh.hnjuh.cn

[U13] Py：固定长度队列
来源：http://zu.bjjhwx.cn

deque(maxlen=10)
来源：http://lz.jctech888.com.cn

[U14] Py：分组收集到列表
来源：http://he.huixiangedu.cn

defaultdict(list)
来源：http://dz.yuexingan06.cn

[U15] Py：高精度计时
来源：http://jz.asd995.cn

t = time.perf_counter()
来源：http://lt.asd995.cn

[U16] Py：命令行参数解析
来源：http://hn.muxihuayi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ca.bjjhwx.cn

[U17] Py：初始化日志
来源：http://cr.huanxung.cn

logging.basicConfig(level=logging.INFO)
来源：http://ld.shxzskj.cn

[U18] Py：预编译正则
来源：http://ys.shxzskj.cn

pat = re.compile(r"\d+")
来源：http://fn.gzmigu.cn

[U19] Py：正则替换带回调
来源：http://pn.asd995.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xz.asd995.cn

[U20] Py：缓存函数结果
来源：http://qn.shxzskj.cn

@functools.lru_cache(maxsize=None)
来源：http://vm.szxytkj.cn

[U21] Py：自定义上下文管理器
来源：http://dl.9csxet.cn

@contextlib.contextmanager
来源：http://gt.9csxet.cn

[U22] Py：矩阵转置
来源：http://ez.hahajie.cn

list(zip(*m))
来源：http://vd.9csxet.cn

[U23] Py：分块读取大文件
来源：http://pm.shxzukj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://uf.huixiangedu.cn

[U24] Py：路径操作
来源：http://ei.521024.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kb.szsharing.cn

[U25] Py：CSV 按字典读
来源：http://ne.colortex.cn

csv.DictReader(f)
来源：http://th.yuntaijiaju.cn

[U26] Py：并发下载
来源：http://wk.bjjhwx.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://oy.nszjky.cn

[U27] Py：异步 HTTP
来源：http://vt.yuntaijiaju.cn

aiohttp.ClientSession() 配合 async with
来源：http://ef.haigaiapp.cn

[U28] Py：类型别名
来源：http://vf.shxzskj.cn

UserId = int
来源：http://nw.9csxet.cn

[U29] Py：属性校验
来源：http://ym.bjjhwx.cn

@property 与 @x.setter 配合
来源：http://sy.szxytkj.cn

[U30] Py：数据类
来源：http://aa.jctech888.com.cn

@dataclass(slots=True)
来源：http://zz.huixinmuqiang.cn

[U31] Py：单测
来源：http://dg.yuexingan06.cn

python -m pytest -q
来源：http://yi.panjiajie.cn

[U32] Py：代码格式化
来源：http://ba.szsharing.cn

ruff format . && ruff check --fix .
来源：http://yw.bookmarksfly.cn

[U33] Py：打包发布
来源：http://zj.bjjhwx.cn

python -m build  （依赖 pyproject.toml）
来源：http://pb.hnjuh.cn

[U34] Py：判断编码
来源：http://cm.yuntaijiaju.cn

chardet.detect(raw)
来源：http://lm.shtwfgs.cn

[U35] Py：发送邮件
来源：http://qh.asd995.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zs.shxzukj.cn

[U36] Py：定时任务
来源：http://uu.jianghongdianzi.cn

schedule.every(10).minutes.do(job)
来源：http://ua.panjiajie.cn

[U37] Py：读写 Excel
来源：http://pm.hnjuh.cn

pandas.read_excel / DataFrame.to_excel
来源：http://rm.haigaiapp.cn

[U38] Py：获取脚本所在目录
来源：http://bm.panjiajie.cn

Path(__file__).resolve().parent
来源：http://va.szsharing.cn

[U39] Py：判断是否在交互环境
来源：http://eh.szsharing.cn

sys.stdout.isatty()
来源：http://mh.colortex.cn

[U40] Py：打印到标准错误
来源：http://qy.nicolike.cn

print("err", file=sys.stderr)
来源：http://oj.colortex.cn

[U41] PHP：初始化 Composer 项目
来源：http://gy.panjiajie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qg.colortex.cn

[U42] PHP：PSR-4 自动加载
来源：http://fg.panjiajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ou.shtwfgs.cn

[U43] PHP：声明命名空间
来源：http://mk.colortex.cn

namespace App\Http;
来源：http://tc.gzmigu.cn

[U44] PHP：开启严格类型
来源：http://ke.shxzskj.cn

declare(strict_types=1);
来源：http://lw.panjiajie.cn

[U45] PHP：类型声明与返回类型
来源：http://fi.muxihuayi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://pp.bjjhwx.cn

[U46] PHP：可空类型
来源：http://mi.huanxung.cn

?string $name = null
来源：http://gf.huixinmuqiang.cn

[U47] PHP：联合类型
来源：http://si.bjjhwx.cn

int|string $id
来源：http://nc.muxihuayi.cn

[U48] PHP：纯枚举
来源：http://qq.nicolike.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nk.yuntaijiaju.cn

[U49] PHP：只读属性
来源：http://ws.chemitech.net.cn

public readonly string $name
来源：http://wl.huixinmuqiang.cn

[U50] PHP：构造器属性提升
来源：http://ga.jctech888.com.cn

public function __construct(private int $id) {}
来源：http://kz.huixiangedu.cn

[U51] PHP：数组解构
来源：http://zp.wgjwhj.cn

[$a, $b] = $arr;
来源：http://bq.yuntaijiaju.cn

[U52] PHP：箭头函数
来源：http://dd.colortex.cn

$double = fn($x) => $x * 2;
来源：http://vn.szxytkj.cn

[U53] PHP：空合并运算符
来源：http://le.gzmigu.cn

$v = $a ?? $b ?? "default";
来源：http://qd.szsharing.cn

[U54] PHP：空安全调用
来源：http://ck.yuntaijiaju.cn

$obj?->method()
来源：http://tq.yuexingan06.cn

[U55] PHP：match 表达式
来源：http://ne.yuexingan06.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://co.asd995.cn

[U56] PHP：命名参数
来源：http://mr.haigaiapp.cn

f(a: 1, b: 2)
来源：http://on.colortex.cn

[U57] PHP：字符串插值
来源：http://an.colortex.cn

"值: {$a}"
来源：http://gf.yuexingan06.cn

[U58] PHP：数组三件套
来源：http://rf.hahajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vf.wgjwhj.cn

[U59] PHP：自定义排序
来源：http://st.521024.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cv.chemitech.net.cn

[U60] PHP：JSON 编解码
来源：http://ml.hahajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vy.gzmigu.cn

[U61] PHP：正则
来源：http://dn.bookmarksfly.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ux.chemitech.net.cn

[U62] PHP：日期对象
来源：http://gw.shxzukj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xd.colortex.cn

[U63] PHP：文件读写
来源：http://jm.521024.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://eu.hnjuh.cn

[U64] PHP：目录遍历
来源：http://ui.yuntaijiaju.cn

glob("dir/*.php");  scandir("dir");
来源：http://hb.asd995.cn

[U65] PHP：会话
来源：http://ns.szxytkj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://bh.newstarts.cn

[U66] PHP：设置 Cookie
来源：http://uy.nicolike.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ko.muxihuayi.cn

[U67] PHP：处理文件上传
来源：http://ux.wgjwhj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vj.szsharing.cn

[U68] PHP：PDO 连接
来源：http://di.gzmigu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dz.panjiajie.cn

[U69] PHP：PDO 预处理
来源：http://yt.szsharing.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jp.panjiajie.cn

[U70] PHP：PDO 事务
来源：http://as.haigaiapp.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ht.huanxung.cn

[U71] PHP：抛出异常
来源：http://ln.lnxyls.cn

throw new RuntimeException("失败", 500);
来源：http://na.haigaiapp.cn

[U72] PHP：写错误日志
来源：http://wr.wgjwhj.cn

error_log("失败: " . $e->getMessage());
来源：http://qt.jianghongdianzi.cn

[U73] PHP：读取 ini 配置
来源：http://fw.bjjhwx.cn

parse_ini_file("config.ini", true)
来源：http://xh.bookmarksfly.cn

[U74] PHP：读取环境变量
来源：http://es.asd995.cn

getenv("APP_ENV") ?: "production"
来源：http://cf.gzmigu.cn

[U75] PHP：依赖注入
来源：http://eg.szxytkj.cn

composer require psr/container
来源：http://km.chemitech.net.cn

[U76] PHP：简单路由
来源：http://ju.hahajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ou.shxzukj.cn

[U77] PHP：模板渲染
来源：http://vi.asd995.cn

composer require twig/twig
来源：http://lc.jctech888.com.cn

[U78] PHP：单元测试
来源：http://vp.bjjhwx.cn

composer require --dev phpunit/phpunit
来源：http://vm.shxzukj.cn

[U79] PHP：静态分析
来源：http://dt.panjiajie.cn

composer require --dev phpstan/phpstan
来源：http://kk.asd995.cn

[U80] PHP：代码规范修复
来源：http://ld.shxzukj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://wc.jctech888.com.cn

[U81] JS：初始化项目
来源：http://ra.hahajie.cn

npm init -y;  npm i express
来源：http://lw.wgjwhj.cn

[U82] JS：package.json 脚本
来源：http://jn.huixinmuqiang.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tz.huanxung.cn

[U83] JS：ES Module 导入导出
来源：http://yx.szxytkj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://af.521024.cn

[U84] JS：CommonJS 写法
来源：http://xn.shxzskj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://zg.hahajie.cn

[U85] JS：可选链
来源：http://lz.muxihuayi.cn

a?.b?.c
来源：http://ar.newstarts.cn

[U86] JS：空值合并
来源：http://nn.shtwfgs.cn

a ?? b
来源：http://xi.huixinmuqiang.cn

[U87] JS：解构默认值
来源：http://wq.wgjwhj.cn

const { a = 1, b = 2 } = obj;
来源：http://jd.panjiajie.cn

[U88] JS：对象展开合并
来源：http://zw.nicolike.cn

{ ...a, ...b }
来源：http://gx.521024.cn

[U89] JS：数组去重
来源：http://qj.521024.cn

[...new Set(arr)]
来源：http://kh.521024.cn

[U90] JS：数字数组排序
来源：http://ip.newstarts.cn

[...arr].sort((a, b) => a - b)
来源：http://zg.huixinmuqiang.cn

[U91] JS：对象键值遍历
来源：http://lv.huixiangedu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ar.huixinmuqiang.cn

[U92] JS：深拷贝
来源：http://ep.szxytkj.cn

structuredClone(obj)
来源：http://zb.lnxyls.cn

[U93] JS：模板字符串
来源：http://ep.huixinmuqiang.cn

`共 ${n} 条`
来源：http://rv.gzmigu.cn

[U94] JS：箭头函数
来源：http://ju.yuexingan06.cn

const double = x => x * 2;
来源：http://lr.nicolike.cn

[U95] JS：Promise 包装
来源：http://di.colortex.cn

new Promise((resolve, reject) => {})
来源：http://re.hahajie.cn

[U96] JS：async/await 与异常
来源：http://hf.hnjuh.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tm.newstarts.cn

[U97] JS：并发请求
来源：http://bn.haigaiapp.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qk.521024.cn

[U98] JS：fetch 带 JSON
来源：http://en.szsharing.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mb.nicolike.cn

[U99] JS：事件监听
来源：http://hv.colortex.cn

el.addEventListener("click", e => {})
来源：http://qo.asd995.cn

[U100] JS：DOM 查询
来源：http://yn.hahajie.cn

document.querySelector(".item")
来源：http://yp.nicolike.cn

[U101] JS：classList 操作
来源：http://ns.nicolike.cn

el.classList.toggle("active")
来源：http://fo.521024.cn

[U102] JS：本地存储
来源：http://ob.szsharing.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://il.newstarts.cn

[U103] JS：定时器
来源：http://dj.bookmarksfly.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vj.9csxet.cn

[U104] JS：防抖
来源：http://qz.haigaiapp.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oj.shxzskj.cn

[U105] JS：节流
来源：http://pa.shxzskj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cw.shxzskj.cn

[U106] JS：日期格式化
来源：http://vz.bookmarksfly.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ly.yuntaijiaju.cn

[U107] JS：数字千分位
来源：http://lg.szsharing.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fz.shtwfgs.cn

[U108] JS：随机整数
来源：http://ds.szsharing.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fb.jianghongdianzi.cn

[U109] JS：数组分组
来源：http://nk.huanxung.cn

Object.groupBy(arr, x => x.type)
来源：http://bi.yuexingan06.cn

[U110] JS：数组分块
来源：http://qv.muxihuayi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lv.huanxung.cn


<!-- 参考信息 -->