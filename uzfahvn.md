代发 wailian999

[T21] Swift：遍历
来源：http://ax.bookmarksfly.cn

for x in a { print(x) }
来源：http://lj.colortex.cn

[T22] Swift：字典
来源：http://bc.bjjhwx.cn

var d = ["a": 1];  d["b"] = 2
来源：http://qz.nszjky.cn

[T23] Swift：函数
来源：http://wb.jctech888.com.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mg.521024.cn

[T24] Swift：闭包
来源：http://qu.jianghongdianzi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://cp.newstarts.cn

[T25] Swift：结构体
来源：http://cz.nszjky.cn

struct P { var x: Int }
来源：http://yr.9csxet.cn

[T26] Swift：类与重写
来源：http://ui.huixiangedu.cn

class A: Base { override func f() {} }
来源：http://gl.newstarts.cn

[T27] Swift：错误处理
来源：http://pq.521024.cn

do { try f() } catch { print(error) }
来源：http://pi.nszjky.cn

[T28] Swift：枚举
来源：http://wz.panjiajie.cn

enum Color { case red, green }
来源：http://ny.szxytkj.cn

[T29] Swift：guard 提前返回
来源：http://zn.chemitech.net.cn

guard let x = opt else { return }
来源：http://sp.szxytkj.cn

[T30] Swift：协议
来源：http://jb.9csxet.cn

protocol Shape { func area() -> Double }
来源：http://ge.lnxyls.cn

[T31] Lua：Hello World
来源：http://wx.521024.cn

print("Hello")
来源：http://xd.haigaiapp.cn

[T32] Lua：局部变量
来源：http://sb.lnxyls.cn

local a = 1
来源：http://ny.newstarts.cn

[T33] Lua：表（数组）
来源：http://af.bookmarksfly.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://qg.colortex.cn

[T34] Lua：遍历表
来源：http://dx.521024.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://pi.shxzukj.cn

[T35] Lua：字典表
来源：http://le.huixiangedu.cn

local d = { a = 1 };  d.b = 2
来源：http://mz.wgjwhj.cn

[T36] Lua：函数
来源：http://rx.521024.cn

function add(a, b) return a + b end
来源：http://kf.wgjwhj.cn

[T37] Lua：字符串拼接
来源：http://eq.shtwfgs.cn

"a" .. "b"
来源：http://pm.hnjuh.cn

[T38] Lua：条件
来源：http://wp.bjjhwx.cn

if x > 0 then print("正") end
来源：http://dk.wgjwhj.cn

[T39] Lua：模式匹配
来源：http://bs.yuntaijiaju.cn

string.find(s, "%d+")
来源：http://vk.yuntaijiaju.cn

[T40] Lua：元表
来源：http://go.shxzskj.cn

setmetatable({}, { __index = base })
来源：http://wv.huixinmuqiang.cn

[T41] Perl：Hello World
来源：http://jy.hahajie.cn

print "Hello\n";
来源：http://fc.hahajie.cn

[T42] Perl：变量类型
来源：http://vd.521024.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rl.asd995.cn

[T43] Perl：字符串插值
来源：http://qa.shtwfgs.cn

"值: $a"
来源：http://qv.shxzskj.cn

[T44] Perl：条件
来源：http://xc.chemitech.net.cn

if ($a > 0) { print "正"; }
来源：http://lg.9csxet.cn

[T45] Perl：数组遍历
来源：http://cg.nicolike.cn

for my $x (@arr) { print $x; }
来源：http://er.hahajie.cn

[T46] Perl：哈希操作
来源：http://ar.jctech888.com.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kw.shxzukj.cn

[T47] Perl：正则捕获
来源：http://ch.lnxyls.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ju.jianghongdianzi.cn

[T48] Perl：正则替换
来源：http://dt.521024.cn

$s =~ s/old/new/g;
来源：http://vj.shxzukj.cn

[T49] Perl：函数
来源：http://ky.haigaiapp.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ls.hnjuh.cn

[T50] Perl：逐行读文件
来源：http://ni.colortex.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ii.hnjuh.cn

while (my $line = <$fh>) { print $line; }
来源：http://sw.asd995.cn

[T51] Scala：Hello World
来源：http://cv.lnxyls.cn

println("Hello")
来源：http://hs.yuntaijiaju.cn

[T52] Scala：变量
来源：http://iv.yuexingan06.cn

val a = 1;  var b = 2
来源：http://cx.521024.cn

[T53] Scala：字符串插值
来源：http://vc.jianghongdianzi.cn

s"值: $b"
来源：http://uv.521024.cn

[T54] Scala：集合映射
来源：http://om.shtwfgs.cn

List(1, 2, 3).map(_ * 2)
来源：http://xr.shtwfgs.cn

[T55] Scala：集合过滤
来源：http://uz.shxzskj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qa.newstarts.cn

[T56] Scala：样例类
来源：http://ms.yuntaijiaju.cn

case class User(name: String, age: Int)
来源：http://sf.nicolike.cn

[T57] Scala：模式匹配
来源：http://hj.bookmarksfly.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://nd.nszjky.cn

[T58] Scala：函数定义
来源：http://up.lnxyls.cn

def add(a: Int, b: Int): Int = a + b
来源：http://jp.panjiajie.cn

[T59] Scala：循环
来源：http://dv.nicolike.cn

for (i <- 1 to 10) println(i)
来源：http://jf.521024.cn

[T60] Scala：折叠
来源：http://fg.shxzukj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://na.yuntaijiaju.cn

================================================================================
来源：http://tn.jctech888.com.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jd.lnxyls.cn

================================================================================
来源：http://xj.wgjwhj.cn

[U01] Py：创建虚拟环境
来源：http://mf.bjjhwx.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jc.gzmigu.cn

[U02] Py：导出 / 安装依赖
来源：http://sf.bookmarksfly.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xe.panjiajie.cn

[U03] Py：加载 .env 配置
来源：http://zy.colortex.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zk.hnjuh.cn

[U04] Py：变量调试打印
来源：http://qe.nszjky.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bd.bjjhwx.cn

[U05] Py：列表去重且保序
来源：http://lr.szsharing.cn

list(dict.fromkeys(arr))
来源：http://ga.521024.cn

[U06] Py：合并两个字典
来源：http://fl.gzmigu.cn

{**a, **b}
来源：http://zz.lnxyls.cn

[U07] Py：反转字典键值
来源：http://fa.shtwfgs.cn

{v: k for k, v in d.items()}
来源：http://tt.jianghongdianzi.cn

[U08] Py：展平二维列表
来源：http://gg.asd995.cn

[y for x in nested for y in x]
来源：http://fo.huixinmuqiang.cn

[U09] Py：字典取最大值的键
来源：http://ja.yuntaijiaju.cn

max(d, key=d.get)
来源：http://ef.wgjwhj.cn

[U10] Py：按值排序字典
来源：http://xt.szxytkj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ud.yuntaijiaju.cn

[U11] Py：生成器表达式
来源：http://pq.panjiajie.cn

(x * 2 for x in arr)
来源：http://fb.huixinmuqiang.cn

[U12] Py：取出现最多的 3 个元素
来源：http://et.wgjwhj.cn

Counter(arr).most_common(3)
来源：http://xy.panjiajie.cn

[U13] Py：固定长度队列
来源：http://ii.jianghongdianzi.cn

deque(maxlen=10)
来源：http://ap.panjiajie.cn

[U14] Py：分组收集到列表
来源：http://sp.muxihuayi.cn

defaultdict(list)
来源：http://dr.lnxyls.cn

[U15] Py：高精度计时
来源：http://gr.yuexingan06.cn

t = time.perf_counter()
来源：http://op.asd995.cn

[U16] Py：命令行参数解析
来源：http://fj.panjiajie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://me.yuntaijiaju.cn

[U17] Py：初始化日志
来源：http://uh.colortex.cn

logging.basicConfig(level=logging.INFO)
来源：http://fw.nszjky.cn

[U18] Py：预编译正则
来源：http://ca.szxytkj.cn

pat = re.compile(r"\d+")
来源：http://qh.nicolike.cn

[U19] Py：正则替换带回调
来源：http://cc.yuntaijiaju.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kx.huixinmuqiang.cn

[U20] Py：缓存函数结果
来源：http://ne.wgjwhj.cn

@functools.lru_cache(maxsize=None)
来源：http://vy.chemitech.net.cn

[U21] Py：自定义上下文管理器
来源：http://hr.nszjky.cn

@contextlib.contextmanager
来源：http://kt.9csxet.cn

[U22] Py：矩阵转置
来源：http://kj.yuntaijiaju.cn

list(zip(*m))
来源：http://zk.wgjwhj.cn

[U23] Py：分块读取大文件
来源：http://rg.szsharing.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://st.jctech888.com.cn

[U24] Py：路径操作
来源：http://hi.colortex.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://go.gzmigu.cn

[U25] Py：CSV 按字典读
来源：http://jw.panjiajie.cn

csv.DictReader(f)
来源：http://mq.newstarts.cn

[U26] Py：并发下载
来源：http://rz.szxytkj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://oi.hnjuh.cn

[U27] Py：异步 HTTP
来源：http://gh.hahajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://ul.szsharing.cn

[U28] Py：类型别名
来源：http://rq.wgjwhj.cn

UserId = int
来源：http://nh.huanxung.cn

[U29] Py：属性校验
来源：http://gv.szxytkj.cn

@property 与 @x.setter 配合
来源：http://hb.shxzukj.cn

[U30] Py：数据类
来源：http://tw.asd995.cn

@dataclass(slots=True)
来源：http://tc.hnjuh.cn

[U31] Py：单测
来源：http://dt.szsharing.cn

python -m pytest -q
来源：http://cc.huixinmuqiang.cn

[U32] Py：代码格式化
来源：http://no.shxzukj.cn

ruff format . && ruff check --fix .
来源：http://zf.huanxung.cn

[U33] Py：打包发布
来源：http://qr.chemitech.net.cn

python -m build  （依赖 pyproject.toml）
来源：http://wz.szxytkj.cn

[U34] Py：判断编码
来源：http://vf.shxzukj.cn

chardet.detect(raw)
来源：http://zk.panjiajie.cn

[U35] Py：发送邮件
来源：http://pd.panjiajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ji.huixiangedu.cn

[U36] Py：定时任务
来源：http://az.muxihuayi.cn

schedule.every(10).minutes.do(job)
来源：http://ms.chemitech.net.cn

[U37] Py：读写 Excel
来源：http://yb.shtwfgs.cn

pandas.read_excel / DataFrame.to_excel
来源：http://mr.nicolike.cn

[U38] Py：获取脚本所在目录
来源：http://uq.asd995.cn

Path(__file__).resolve().parent
来源：http://ur.colortex.cn

[U39] Py：判断是否在交互环境
来源：http://lc.gzmigu.cn

sys.stdout.isatty()
来源：http://lq.newstarts.cn

[U40] Py：打印到标准错误
来源：http://ik.jianghongdianzi.cn

print("err", file=sys.stderr)
来源：http://ms.9csxet.cn

[U41] PHP：初始化 Composer 项目
来源：http://tb.bookmarksfly.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ok.bjjhwx.cn

[U42] PHP：PSR-4 自动加载
来源：http://dz.bjjhwx.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wm.yuexingan06.cn

[U43] PHP：声明命名空间
来源：http://tl.521024.cn

namespace App\Http;
来源：http://vi.bookmarksfly.cn

[U44] PHP：开启严格类型
来源：http://nd.wgjwhj.cn

declare(strict_types=1);
来源：http://pc.muxihuayi.cn

[U45] PHP：类型声明与返回类型
来源：http://lf.newstarts.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://hj.yuexingan06.cn

[U46] PHP：可空类型
来源：http://fq.yuntaijiaju.cn

?string $name = null
来源：http://ib.chemitech.net.cn

[U47] PHP：联合类型
来源：http://ca.szxytkj.cn

int|string $id
来源：http://pp.huixinmuqiang.cn

[U48] PHP：纯枚举
来源：http://xx.nszjky.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jc.bookmarksfly.cn

[U49] PHP：只读属性
来源：http://kg.panjiajie.cn

public readonly string $name
来源：http://bx.nicolike.cn

[U50] PHP：构造器属性提升
来源：http://ih.asd995.cn

public function __construct(private int $id) {}
来源：http://tm.newstarts.cn

[U51] PHP：数组解构
来源：http://og.shxzukj.cn

[$a, $b] = $arr;
来源：http://dt.muxihuayi.cn

[U52] PHP：箭头函数
来源：http://sv.shtwfgs.cn

$double = fn($x) => $x * 2;
来源：http://th.shtwfgs.cn

[U53] PHP：空合并运算符
来源：http://rc.yuntaijiaju.cn

$v = $a ?? $b ?? "default";
来源：http://ji.asd995.cn

[U54] PHP：空安全调用
来源：http://si.asd995.cn

$obj?->method()
来源：http://ok.muxihuayi.cn

[U55] PHP：match 表达式
来源：http://cf.bookmarksfly.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://et.jctech888.com.cn

[U56] PHP：命名参数
来源：http://sa.huanxung.cn

f(a: 1, b: 2)
来源：http://oi.szsharing.cn

[U57] PHP：字符串插值
来源：http://gq.muxihuayi.cn

"值: {$a}"
来源：http://yk.bookmarksfly.cn

[U58] PHP：数组三件套
来源：http://jv.jianghongdianzi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yy.chemitech.net.cn

[U59] PHP：自定义排序
来源：http://we.bookmarksfly.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cz.wgjwhj.cn

[U60] PHP：JSON 编解码
来源：http://lh.newstarts.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fg.colortex.cn

[U61] PHP：正则
来源：http://kp.muxihuayi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hh.asd995.cn

[U62] PHP：日期对象
来源：http://bo.bookmarksfly.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://so.wgjwhj.cn

[U63] PHP：文件读写
来源：http://vj.chemitech.net.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mp.chemitech.net.cn

[U64] PHP：目录遍历
来源：http://wx.szsharing.cn

glob("dir/*.php");  scandir("dir");
来源：http://vp.wgjwhj.cn

[U65] PHP：会话
来源：http://nv.newstarts.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://xy.chemitech.net.cn

[U66] PHP：设置 Cookie
来源：http://yx.shxzukj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gg.bookmarksfly.cn

[U67] PHP：处理文件上传
来源：http://tj.hahajie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kz.szsharing.cn

[U68] PHP：PDO 连接
来源：http://ur.hnjuh.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qp.newstarts.cn

[U69] PHP：PDO 预处理
来源：http://rk.huanxung.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pn.shxzukj.cn

[U70] PHP：PDO 事务
来源：http://bb.jctech888.com.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vj.szxytkj.cn

[U71] PHP：抛出异常
来源：http://db.szsharing.cn

throw new RuntimeException("失败", 500);
来源：http://xh.shxzukj.cn

[U72] PHP：写错误日志
来源：http://pv.9csxet.cn

error_log("失败: " . $e->getMessage());
来源：http://jd.shxzukj.cn

[U73] PHP：读取 ini 配置
来源：http://ab.newstarts.cn

parse_ini_file("config.ini", true)
来源：http://my.yuntaijiaju.cn

[U74] PHP：读取环境变量
来源：http://mt.huixinmuqiang.cn

getenv("APP_ENV") ?: "production"
来源：http://wx.521024.cn

[U75] PHP：依赖注入
来源：http://vp.yuexingan06.cn

composer require psr/container
来源：http://sp.gzmigu.cn

[U76] PHP：简单路由
来源：http://ai.haigaiapp.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bn.huixiangedu.cn

[U77] PHP：模板渲染
来源：http://mq.asd995.cn

composer require twig/twig
来源：http://yp.hahajie.cn

[U78] PHP：单元测试
来源：http://dc.newstarts.cn

composer require --dev phpunit/phpunit
来源：http://pp.nszjky.cn

[U79] PHP：静态分析
来源：http://dk.huanxung.cn

composer require --dev phpstan/phpstan
来源：http://cq.szsharing.cn

[U80] PHP：代码规范修复
来源：http://er.szxytkj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xg.9csxet.cn

[U81] JS：初始化项目
来源：http://ym.jctech888.com.cn

npm init -y;  npm i express
来源：http://no.haigaiapp.cn

[U82] JS：package.json 脚本
来源：http://jx.yuntaijiaju.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fx.panjiajie.cn

[U83] JS：ES Module 导入导出
来源：http://pz.nszjky.cn

export const a = 1;  import { a } from "./m.js";
来源：http://iz.huanxung.cn

[U84] JS：CommonJS 写法
来源：http://jg.huixiangedu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://yh.huixiangedu.cn

[U85] JS：可选链
来源：http://ic.9csxet.cn

a?.b?.c
来源：http://id.yuexingan06.cn

[U86] JS：空值合并
来源：http://oa.shxzskj.cn

a ?? b
来源：http://jq.yuexingan06.cn

[U87] JS：解构默认值
来源：http://lm.hahajie.cn

const { a = 1, b = 2 } = obj;
来源：http://me.newstarts.cn

[U88] JS：对象展开合并
来源：http://dg.bookmarksfly.cn

{ ...a, ...b }
来源：http://ob.nszjky.cn

[U89] JS：数组去重
来源：http://wz.hahajie.cn

[...new Set(arr)]
来源：http://wa.shtwfgs.cn

[U90] JS：数字数组排序
来源：http://iy.huixinmuqiang.cn

[...arr].sort((a, b) => a - b)
来源：http://nt.jianghongdianzi.cn

[U91] JS：对象键值遍历
来源：http://rb.nicolike.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fv.wgjwhj.cn

[U92] JS：深拷贝
来源：http://os.yuntaijiaju.cn

structuredClone(obj)
来源：http://es.muxihuayi.cn

[U93] JS：模板字符串
来源：http://pd.yuntaijiaju.cn

`共 ${n} 条`
来源：http://ks.gzmigu.cn

[U94] JS：箭头函数
来源：http://on.huanxung.cn

const double = x => x * 2;
来源：http://lm.muxihuayi.cn

[U95] JS：Promise 包装
来源：http://or.szxytkj.cn

new Promise((resolve, reject) => {})
来源：http://tk.haigaiapp.cn

[U96] JS：async/await 与异常
来源：http://qq.shtwfgs.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sm.huixinmuqiang.cn

[U97] JS：并发请求
来源：http://wy.szxytkj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vd.gzmigu.cn

[U98] JS：fetch 带 JSON
来源：http://km.muxihuayi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wh.nszjky.cn

[U99] JS：事件监听
来源：http://hp.shxzukj.cn

el.addEventListener("click", e => {})
来源：http://jc.hnjuh.cn

[U100] JS：DOM 查询
来源：http://rc.huixinmuqiang.cn

document.querySelector(".item")
来源：http://oz.asd995.cn

[U101] JS：classList 操作
来源：http://nl.nszjky.cn

el.classList.toggle("active")
来源：http://cc.chemitech.net.cn

[U102] JS：本地存储
来源：http://oe.asd995.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://sw.muxihuayi.cn

[U103] JS：定时器
来源：http://wm.asd995.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yc.wgjwhj.cn

[U104] JS：防抖
来源：http://gc.nszjky.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yk.bookmarksfly.cn

[U105] JS：节流
来源：http://wi.nszjky.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xu.lnxyls.cn

[U106] JS：日期格式化
来源：http://mc.muxihuayi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ns.bookmarksfly.cn

[U107] JS：数字千分位
来源：http://bl.yuntaijiaju.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xk.szxytkj.cn

[U108] JS：随机整数
来源：http://uq.nszjky.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://uz.hahajie.cn


<!-- 参考信息 -->