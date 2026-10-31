代发 wailian999

[T23] Swift：函数
来源：http://ew.panjiajie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pn.panjiajie.cn

[T24] Swift：闭包
来源：http://tt.9csxet.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://cy.bookmarksfly.cn

[T25] Swift：结构体
来源：http://hw.bjjhwx.cn

struct P { var x: Int }
来源：http://ba.muxihuayi.cn

[T26] Swift：类与重写
来源：http://cp.yuexingan06.cn

class A: Base { override func f() {} }
来源：http://cw.shxzukj.cn

[T27] Swift：错误处理
来源：http://qr.huixiangedu.cn

do { try f() } catch { print(error) }
来源：http://kl.huixinmuqiang.cn

[T28] Swift：枚举
来源：http://uj.bjjhwx.cn

enum Color { case red, green }
来源：http://zp.chemitech.net.cn

[T29] Swift：guard 提前返回
来源：http://di.lnxyls.cn

guard let x = opt else { return }
来源：http://js.muxihuayi.cn

[T30] Swift：协议
来源：http://rp.shxzskj.cn

protocol Shape { func area() -> Double }
来源：http://xl.yuntaijiaju.cn

[T31] Lua：Hello World
来源：http://zw.panjiajie.cn

print("Hello")
来源：http://mx.chemitech.net.cn

[T32] Lua：局部变量
来源：http://pk.huixiangedu.cn

local a = 1
来源：http://ap.bookmarksfly.cn

[T33] Lua：表（数组）
来源：http://rf.nicolike.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://az.9csxet.cn

[T34] Lua：遍历表
来源：http://bo.gzmigu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://mr.huixiangedu.cn

[T35] Lua：字典表
来源：http://pu.shtwfgs.cn

local d = { a = 1 };  d.b = 2
来源：http://dh.jctech888.com.cn

[T36] Lua：函数
来源：http://yk.shxzskj.cn

function add(a, b) return a + b end
来源：http://qn.lnxyls.cn

[T37] Lua：字符串拼接
来源：http://tn.chemitech.net.cn

"a" .. "b"
来源：http://hy.huixiangedu.cn

[T38] Lua：条件
来源：http://jk.521024.cn

if x > 0 then print("正") end
来源：http://zv.gzmigu.cn

[T39] Lua：模式匹配
来源：http://al.bjjhwx.cn

string.find(s, "%d+")
来源：http://xv.huixiangedu.cn

[T40] Lua：元表
来源：http://ye.wgjwhj.cn

setmetatable({}, { __index = base })
来源：http://qh.shtwfgs.cn

[T41] Perl：Hello World
来源：http://ym.chemitech.net.cn

print "Hello\n";
来源：http://xd.chemitech.net.cn

[T42] Perl：变量类型
来源：http://ww.muxihuayi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xt.shxzskj.cn

[T43] Perl：字符串插值
来源：http://rg.newstarts.cn

"值: $a"
来源：http://zl.haigaiapp.cn

[T44] Perl：条件
来源：http://fk.shxzukj.cn

if ($a > 0) { print "正"; }
来源：http://pw.bjjhwx.cn

[T45] Perl：数组遍历
来源：http://uo.szxytkj.cn

for my $x (@arr) { print $x; }
来源：http://wb.bjjhwx.cn

[T46] Perl：哈希操作
来源：http://tr.lnxyls.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xm.9csxet.cn

[T47] Perl：正则捕获
来源：http://gz.asd995.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ue.wgjwhj.cn

[T48] Perl：正则替换
来源：http://qx.szsharing.cn

$s =~ s/old/new/g;
来源：http://cj.huixinmuqiang.cn

[T49] Perl：函数
来源：http://ss.shtwfgs.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ar.shxzukj.cn

[T50] Perl：逐行读文件
来源：http://co.nszjky.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rh.huixinmuqiang.cn

while (my $line = <$fh>) { print $line; }
来源：http://de.muxihuayi.cn

[T51] Scala：Hello World
来源：http://hv.wgjwhj.cn

println("Hello")
来源：http://pl.szxytkj.cn

[T52] Scala：变量
来源：http://jb.hahajie.cn

val a = 1;  var b = 2
来源：http://yk.jctech888.com.cn

[T53] Scala：字符串插值
来源：http://fg.bjjhwx.cn

s"值: $b"
来源：http://ff.shxzskj.cn

[T54] Scala：集合映射
来源：http://gz.huixiangedu.cn

List(1, 2, 3).map(_ * 2)
来源：http://va.jianghongdianzi.cn

[T55] Scala：集合过滤
来源：http://ck.nszjky.cn

List(1, 2, 3).filter(_ > 1)
来源：http://bb.chemitech.net.cn

[T56] Scala：样例类
来源：http://qu.jctech888.com.cn

case class User(name: String, age: Int)
来源：http://nc.newstarts.cn

[T57] Scala：模式匹配
来源：http://bm.hahajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://xx.shxzukj.cn

[T58] Scala：函数定义
来源：http://uu.huixinmuqiang.cn

def add(a: Int, b: Int): Int = a + b
来源：http://op.nicolike.cn

[T59] Scala：循环
来源：http://uo.asd995.cn

for (i <- 1 to 10) println(i)
来源：http://uy.shxzukj.cn

[T60] Scala：折叠
来源：http://um.jctech888.com.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hs.huixiangedu.cn

================================================================================
来源：http://zi.yuexingan06.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://du.muxihuayi.cn

================================================================================
来源：http://hb.huanxung.cn

[U01] Py：创建虚拟环境
来源：http://jj.huixiangedu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://gh.huanxung.cn

[U02] Py：导出 / 安装依赖
来源：http://vj.jianghongdianzi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rl.shxzukj.cn

[U03] Py：加载 .env 配置
来源：http://bw.szsharing.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://te.bookmarksfly.cn

[U04] Py：变量调试打印
来源：http://bp.521024.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://id.wgjwhj.cn

[U05] Py：列表去重且保序
来源：http://bs.szxytkj.cn

list(dict.fromkeys(arr))
来源：http://cz.lnxyls.cn

[U06] Py：合并两个字典
来源：http://yf.haigaiapp.cn

{**a, **b}
来源：http://rq.521024.cn

[U07] Py：反转字典键值
来源：http://ou.wgjwhj.cn

{v: k for k, v in d.items()}
来源：http://se.chemitech.net.cn

[U08] Py：展平二维列表
来源：http://fq.jctech888.com.cn

[y for x in nested for y in x]
来源：http://pt.gzmigu.cn

[U09] Py：字典取最大值的键
来源：http://iw.colortex.cn

max(d, key=d.get)
来源：http://hu.jctech888.com.cn

[U10] Py：按值排序字典
来源：http://st.colortex.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hc.asd995.cn

[U11] Py：生成器表达式
来源：http://la.muxihuayi.cn

(x * 2 for x in arr)
来源：http://rs.muxihuayi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zq.gzmigu.cn

Counter(arr).most_common(3)
来源：http://gj.lnxyls.cn

[U13] Py：固定长度队列
来源：http://fa.nszjky.cn

deque(maxlen=10)
来源：http://eg.hnjuh.cn

[U14] Py：分组收集到列表
来源：http://ow.yuntaijiaju.cn

defaultdict(list)
来源：http://cg.yuntaijiaju.cn

[U15] Py：高精度计时
来源：http://yd.lnxyls.cn

t = time.perf_counter()
来源：http://ym.huanxung.cn

[U16] Py：命令行参数解析
来源：http://qz.chemitech.net.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bz.shtwfgs.cn

[U17] Py：初始化日志
来源：http://mw.shtwfgs.cn

logging.basicConfig(level=logging.INFO)
来源：http://ps.yuexingan06.cn

[U18] Py：预编译正则
来源：http://lp.bjjhwx.cn

pat = re.compile(r"\d+")
来源：http://jn.9csxet.cn

[U19] Py：正则替换带回调
来源：http://es.szsharing.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sq.shxzskj.cn

[U20] Py：缓存函数结果
来源：http://fk.hnjuh.cn

@functools.lru_cache(maxsize=None)
来源：http://lm.hahajie.cn

[U21] Py：自定义上下文管理器
来源：http://cj.hahajie.cn

@contextlib.contextmanager
来源：http://wr.colortex.cn

[U22] Py：矩阵转置
来源：http://ap.szsharing.cn

list(zip(*m))
来源：http://ub.shtwfgs.cn

[U23] Py：分块读取大文件
来源：http://jj.nicolike.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vi.szxytkj.cn

[U24] Py：路径操作
来源：http://uw.yuntaijiaju.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ms.hnjuh.cn

[U25] Py：CSV 按字典读
来源：http://pu.newstarts.cn

csv.DictReader(f)
来源：http://ac.chemitech.net.cn

[U26] Py：并发下载
来源：http://ii.9csxet.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://oc.jctech888.com.cn

[U27] Py：异步 HTTP
来源：http://nn.hnjuh.cn

aiohttp.ClientSession() 配合 async with
来源：http://sv.yuntaijiaju.cn

[U28] Py：类型别名
来源：http://xf.nszjky.cn

UserId = int
来源：http://yx.gzmigu.cn

[U29] Py：属性校验
来源：http://pu.shtwfgs.cn

@property 与 @x.setter 配合
来源：http://kd.chemitech.net.cn

[U30] Py：数据类
来源：http://uj.szxytkj.cn

@dataclass(slots=True)
来源：http://kz.hnjuh.cn

[U31] Py：单测
来源：http://zj.panjiajie.cn

python -m pytest -q
来源：http://hk.521024.cn

[U32] Py：代码格式化
来源：http://lj.shxzskj.cn

ruff format . && ruff check --fix .
来源：http://zc.chemitech.net.cn

[U33] Py：打包发布
来源：http://zi.colortex.cn

python -m build  （依赖 pyproject.toml）
来源：http://hr.nszjky.cn

[U34] Py：判断编码
来源：http://uz.panjiajie.cn

chardet.detect(raw)
来源：http://ly.jianghongdianzi.cn

[U35] Py：发送邮件
来源：http://fz.haigaiapp.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tv.521024.cn

[U36] Py：定时任务
来源：http://ar.yuexingan06.cn

schedule.every(10).minutes.do(job)
来源：http://bn.szxytkj.cn

[U37] Py：读写 Excel
来源：http://lj.bjjhwx.cn

pandas.read_excel / DataFrame.to_excel
来源：http://it.chemitech.net.cn

[U38] Py：获取脚本所在目录
来源：http://zl.bookmarksfly.cn

Path(__file__).resolve().parent
来源：http://no.newstarts.cn

[U39] Py：判断是否在交互环境
来源：http://ww.9csxet.cn

sys.stdout.isatty()
来源：http://wm.panjiajie.cn

[U40] Py：打印到标准错误
来源：http://sz.bookmarksfly.cn

print("err", file=sys.stderr)
来源：http://gz.chemitech.net.cn

[U41] PHP：初始化 Composer 项目
来源：http://by.shxzskj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ol.huanxung.cn

[U42] PHP：PSR-4 自动加载
来源：http://zv.huanxung.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ns.colortex.cn

[U43] PHP：声明命名空间
来源：http://mj.521024.cn

namespace App\Http;
来源：http://pm.jianghongdianzi.cn

[U44] PHP：开启严格类型
来源：http://xu.panjiajie.cn

declare(strict_types=1);
来源：http://qx.gzmigu.cn

[U45] PHP：类型声明与返回类型
来源：http://ab.lnxyls.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://is.hahajie.cn

[U46] PHP：可空类型
来源：http://cy.chemitech.net.cn

?string $name = null
来源：http://je.huixiangedu.cn

[U47] PHP：联合类型
来源：http://pq.521024.cn

int|string $id
来源：http://fm.521024.cn

[U48] PHP：纯枚举
来源：http://ol.huixiangedu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ej.yuntaijiaju.cn

[U49] PHP：只读属性
来源：http://hn.shxzukj.cn

public readonly string $name
来源：http://hv.newstarts.cn

[U50] PHP：构造器属性提升
来源：http://lm.gzmigu.cn

public function __construct(private int $id) {}
来源：http://bc.shtwfgs.cn

[U51] PHP：数组解构
来源：http://kq.nszjky.cn

[$a, $b] = $arr;
来源：http://rd.jctech888.com.cn

[U52] PHP：箭头函数
来源：http://ct.szxytkj.cn

$double = fn($x) => $x * 2;
来源：http://rz.colortex.cn

[U53] PHP：空合并运算符
来源：http://xb.colortex.cn

$v = $a ?? $b ?? "default";
来源：http://ys.bookmarksfly.cn

[U54] PHP：空安全调用
来源：http://me.colortex.cn

$obj?->method()
来源：http://iz.shxzskj.cn

[U55] PHP：match 表达式
来源：http://kt.521024.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vw.gzmigu.cn

[U56] PHP：命名参数
来源：http://vu.bjjhwx.cn

f(a: 1, b: 2)
来源：http://yk.nszjky.cn

[U57] PHP：字符串插值
来源：http://qy.lnxyls.cn

"值: {$a}"
来源：http://bn.nszjky.cn

[U58] PHP：数组三件套
来源：http://wc.521024.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yo.huanxung.cn

[U59] PHP：自定义排序
来源：http://sr.jctech888.com.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rs.nicolike.cn

[U60] PHP：JSON 编解码
来源：http://yz.huanxung.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ev.chemitech.net.cn

[U61] PHP：正则
来源：http://gp.huixiangedu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://so.jianghongdianzi.cn

[U62] PHP：日期对象
来源：http://xe.wgjwhj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hq.bjjhwx.cn

[U63] PHP：文件读写
来源：http://xt.shxzskj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vz.wgjwhj.cn

[U64] PHP：目录遍历
来源：http://lr.hnjuh.cn

glob("dir/*.php");  scandir("dir");
来源：http://mo.asd995.cn

[U65] PHP：会话
来源：http://lt.shtwfgs.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://io.panjiajie.cn

[U66] PHP：设置 Cookie
来源：http://pi.shxzskj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wz.huixinmuqiang.cn

[U67] PHP：处理文件上传
来源：http://zj.newstarts.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sb.colortex.cn

[U68] PHP：PDO 连接
来源：http://cu.yuntaijiaju.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wz.panjiajie.cn

[U69] PHP：PDO 预处理
来源：http://cw.szxytkj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://np.nicolike.cn

[U70] PHP：PDO 事务
来源：http://pr.haigaiapp.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tr.huanxung.cn

[U71] PHP：抛出异常
来源：http://pp.shtwfgs.cn

throw new RuntimeException("失败", 500);
来源：http://uk.bookmarksfly.cn

[U72] PHP：写错误日志
来源：http://db.yuntaijiaju.cn

error_log("失败: " . $e->getMessage());
来源：http://lf.newstarts.cn

[U73] PHP：读取 ini 配置
来源：http://jk.shxzskj.cn

parse_ini_file("config.ini", true)
来源：http://ex.muxihuayi.cn

[U74] PHP：读取环境变量
来源：http://cz.yuntaijiaju.cn

getenv("APP_ENV") ?: "production"
来源：http://mm.9csxet.cn

[U75] PHP：依赖注入
来源：http://lx.shtwfgs.cn

composer require psr/container
来源：http://kp.yuntaijiaju.cn

[U76] PHP：简单路由
来源：http://lp.nicolike.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://km.hnjuh.cn

[U77] PHP：模板渲染
来源：http://pp.huixiangedu.cn

composer require twig/twig
来源：http://ux.huixinmuqiang.cn

[U78] PHP：单元测试
来源：http://jc.shtwfgs.cn

composer require --dev phpunit/phpunit
来源：http://ja.nszjky.cn

[U79] PHP：静态分析
来源：http://vw.hahajie.cn

composer require --dev phpstan/phpstan
来源：http://uc.nicolike.cn

[U80] PHP：代码规范修复
来源：http://pz.521024.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://py.szsharing.cn

[U81] JS：初始化项目
来源：http://al.nicolike.cn

npm init -y;  npm i express
来源：http://wp.nicolike.cn

[U82] JS：package.json 脚本
来源：http://vo.jctech888.com.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xa.jianghongdianzi.cn

[U83] JS：ES Module 导入导出
来源：http://el.521024.cn

export const a = 1;  import { a } from "./m.js";
来源：http://yw.muxihuayi.cn

[U84] JS：CommonJS 写法
来源：http://bi.chemitech.net.cn

module.exports = { a };  const { a } = require("./m");
来源：http://xa.panjiajie.cn

[U85] JS：可选链
来源：http://et.szsharing.cn

a?.b?.c
来源：http://gi.szsharing.cn

[U86] JS：空值合并
来源：http://ux.521024.cn

a ?? b
来源：http://le.yuntaijiaju.cn

[U87] JS：解构默认值
来源：http://pb.hnjuh.cn

const { a = 1, b = 2 } = obj;
来源：http://kb.haigaiapp.cn

[U88] JS：对象展开合并
来源：http://sn.huanxung.cn

{ ...a, ...b }
来源：http://br.gzmigu.cn

[U89] JS：数组去重
来源：http://pl.newstarts.cn

[...new Set(arr)]
来源：http://yu.szxytkj.cn

[U90] JS：数字数组排序
来源：http://vl.bjjhwx.cn

[...arr].sort((a, b) => a - b)
来源：http://vq.haigaiapp.cn

[U91] JS：对象键值遍历
来源：http://jz.szsharing.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ab.muxihuayi.cn

[U92] JS：深拷贝
来源：http://iy.panjiajie.cn

structuredClone(obj)
来源：http://tv.nszjky.cn

[U93] JS：模板字符串
来源：http://lx.bjjhwx.cn

`共 ${n} 条`
来源：http://is.wgjwhj.cn

[U94] JS：箭头函数
来源：http://it.haigaiapp.cn

const double = x => x * 2;
来源：http://df.jianghongdianzi.cn

[U95] JS：Promise 包装
来源：http://to.bookmarksfly.cn

new Promise((resolve, reject) => {})
来源：http://cj.wgjwhj.cn

[U96] JS：async/await 与异常
来源：http://zg.shxzukj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yi.bookmarksfly.cn

[U97] JS：并发请求
来源：http://lv.huixinmuqiang.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://un.hahajie.cn

[U98] JS：fetch 带 JSON
来源：http://yr.chemitech.net.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nj.jianghongdianzi.cn

[U99] JS：事件监听
来源：http://ox.yuntaijiaju.cn

el.addEventListener("click", e => {})
来源：http://nm.chemitech.net.cn

[U100] JS：DOM 查询
来源：http://sa.hahajie.cn

document.querySelector(".item")
来源：http://gx.bookmarksfly.cn

[U101] JS：classList 操作
来源：http://hs.shxzukj.cn

el.classList.toggle("active")
来源：http://on.bjjhwx.cn

[U102] JS：本地存储
来源：http://rn.szsharing.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ny.hnjuh.cn

[U103] JS：定时器
来源：http://sx.9csxet.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ql.shxzskj.cn

[U104] JS：防抖
来源：http://ln.huixinmuqiang.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xl.521024.cn

[U105] JS：节流
来源：http://ny.haigaiapp.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cm.huanxung.cn

[U106] JS：日期格式化
来源：http://eq.chemitech.net.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ru.shxzskj.cn

[U107] JS：数字千分位
来源：http://nh.nicolike.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sb.colortex.cn

[U108] JS：随机整数
来源：http://di.yuntaijiaju.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wr.shtwfgs.cn

[U109] JS：数组分组
来源：http://pj.wgjwhj.cn

Object.groupBy(arr, x => x.type)
来源：http://cj.jianghongdianzi.cn

[U110] JS：数组分块
来源：http://jq.gzmigu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hn.nicolike.cn


<!-- 参考信息 -->