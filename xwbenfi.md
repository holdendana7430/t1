代发 wailian999

[T19] Swift：可选绑定
来源：http://el.szxytkj.cn

if let n = opt { print(n) }
来源：http://ex.huanxung.cn

[T20] Swift：数组操作
来源：http://hh.haigaiapp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gc.yuntaijiaju.cn

[T21] Swift：遍历
来源：http://yw.nszjky.cn

for x in a { print(x) }
来源：http://zy.bjjhwx.cn

[T22] Swift：字典
来源：http://iw.nicolike.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ch.yuexingan06.cn

[T23] Swift：函数
来源：http://yo.hnjuh.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lu.yuntaijiaju.cn

[T24] Swift：闭包
来源：http://yf.colortex.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://au.yuexingan06.cn

[T25] Swift：结构体
来源：http://oj.nicolike.cn

struct P { var x: Int }
来源：http://ub.colortex.cn

[T26] Swift：类与重写
来源：http://mu.huanxung.cn

class A: Base { override func f() {} }
来源：http://pp.asd995.cn

[T27] Swift：错误处理
来源：http://sx.yuntaijiaju.cn

do { try f() } catch { print(error) }
来源：http://qo.bjjhwx.cn

[T28] Swift：枚举
来源：http://gp.colortex.cn

enum Color { case red, green }
来源：http://jn.nicolike.cn

[T29] Swift：guard 提前返回
来源：http://qz.panjiajie.cn

guard let x = opt else { return }
来源：http://lp.newstarts.cn

[T30] Swift：协议
来源：http://jk.nicolike.cn

protocol Shape { func area() -> Double }
来源：http://kw.huixinmuqiang.cn

[T31] Lua：Hello World
来源：http://iv.nszjky.cn

print("Hello")
来源：http://lg.nszjky.cn

[T32] Lua：局部变量
来源：http://gl.chemitech.net.cn

local a = 1
来源：http://rf.lnxyls.cn

[T33] Lua：表（数组）
来源：http://ch.wgjwhj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://gx.jctech888.com.cn

[T34] Lua：遍历表
来源：http://gi.asd995.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://po.nszjky.cn

[T35] Lua：字典表
来源：http://dw.nszjky.cn

local d = { a = 1 };  d.b = 2
来源：http://mn.panjiajie.cn

[T36] Lua：函数
来源：http://wc.521024.cn

function add(a, b) return a + b end
来源：http://px.panjiajie.cn

[T37] Lua：字符串拼接
来源：http://qy.521024.cn

"a" .. "b"
来源：http://zr.bjjhwx.cn

[T38] Lua：条件
来源：http://hf.chemitech.net.cn

if x > 0 then print("正") end
来源：http://ql.jctech888.com.cn

[T39] Lua：模式匹配
来源：http://hq.jctech888.com.cn

string.find(s, "%d+")
来源：http://jn.muxihuayi.cn

[T40] Lua：元表
来源：http://xr.hahajie.cn

setmetatable({}, { __index = base })
来源：http://qz.hnjuh.cn

[T41] Perl：Hello World
来源：http://mi.gzmigu.cn

print "Hello\n";
来源：http://nw.newstarts.cn

[T42] Perl：变量类型
来源：http://or.wgjwhj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ad.newstarts.cn

[T43] Perl：字符串插值
来源：http://nk.shxzukj.cn

"值: $a"
来源：http://gn.bookmarksfly.cn

[T44] Perl：条件
来源：http://xi.bjjhwx.cn

if ($a > 0) { print "正"; }
来源：http://nf.521024.cn

[T45] Perl：数组遍历
来源：http://gw.bjjhwx.cn

for my $x (@arr) { print $x; }
来源：http://jn.521024.cn

[T46] Perl：哈希操作
来源：http://ph.asd995.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sk.hnjuh.cn

[T47] Perl：正则捕获
来源：http://vb.huixinmuqiang.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://zc.hnjuh.cn

[T48] Perl：正则替换
来源：http://fp.huixinmuqiang.cn

$s =~ s/old/new/g;
来源：http://ut.muxihuayi.cn

[T49] Perl：函数
来源：http://ia.jianghongdianzi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://iz.jctech888.com.cn

[T50] Perl：逐行读文件
来源：http://cl.yuexingan06.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ct.bjjhwx.cn

while (my $line = <$fh>) { print $line; }
来源：http://nw.shxzskj.cn

[T51] Scala：Hello World
来源：http://rx.huanxung.cn

println("Hello")
来源：http://qc.huanxung.cn

[T52] Scala：变量
来源：http://ax.nicolike.cn

val a = 1;  var b = 2
来源：http://am.muxihuayi.cn

[T53] Scala：字符串插值
来源：http://rc.bjjhwx.cn

s"值: $b"
来源：http://vd.gzmigu.cn

[T54] Scala：集合映射
来源：http://kc.bookmarksfly.cn

List(1, 2, 3).map(_ * 2)
来源：http://bl.hahajie.cn

[T55] Scala：集合过滤
来源：http://ya.panjiajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://jy.hnjuh.cn

[T56] Scala：样例类
来源：http://sm.yuntaijiaju.cn

case class User(name: String, age: Int)
来源：http://dv.panjiajie.cn

[T57] Scala：模式匹配
来源：http://so.lnxyls.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://dy.lnxyls.cn

[T58] Scala：函数定义
来源：http://mw.shxzskj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://qq.asd995.cn

[T59] Scala：循环
来源：http://es.shxzskj.cn

for (i <- 1 to 10) println(i)
来源：http://pz.hahajie.cn

[T60] Scala：折叠
来源：http://xl.newstarts.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mq.chemitech.net.cn

================================================================================
来源：http://cw.yuexingan06.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yv.huixiangedu.cn

================================================================================
来源：http://pe.jctech888.com.cn

[U01] Py：创建虚拟环境
来源：http://bp.muxihuayi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vr.hahajie.cn

[U02] Py：导出 / 安装依赖
来源：http://sp.huixinmuqiang.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://er.szxytkj.cn

[U03] Py：加载 .env 配置
来源：http://sh.bookmarksfly.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://pu.yuntaijiaju.cn

[U04] Py：变量调试打印
来源：http://ob.haigaiapp.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sf.muxihuayi.cn

[U05] Py：列表去重且保序
来源：http://ou.shxzukj.cn

list(dict.fromkeys(arr))
来源：http://mp.asd995.cn

[U06] Py：合并两个字典
来源：http://ac.colortex.cn

{**a, **b}
来源：http://zn.szsharing.cn

[U07] Py：反转字典键值
来源：http://dc.chemitech.net.cn

{v: k for k, v in d.items()}
来源：http://id.newstarts.cn

[U08] Py：展平二维列表
来源：http://yo.huixinmuqiang.cn

[y for x in nested for y in x]
来源：http://rn.jctech888.com.cn

[U09] Py：字典取最大值的键
来源：http://ic.gzmigu.cn

max(d, key=d.get)
来源：http://ph.yuexingan06.cn

[U10] Py：按值排序字典
来源：http://ir.hnjuh.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sh.wgjwhj.cn

[U11] Py：生成器表达式
来源：http://or.hnjuh.cn

(x * 2 for x in arr)
来源：http://bz.panjiajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://fr.lnxyls.cn

Counter(arr).most_common(3)
来源：http://oy.shxzskj.cn

[U13] Py：固定长度队列
来源：http://eh.9csxet.cn

deque(maxlen=10)
来源：http://ul.jctech888.com.cn

[U14] Py：分组收集到列表
来源：http://rm.shtwfgs.cn

defaultdict(list)
来源：http://fy.jctech888.com.cn

[U15] Py：高精度计时
来源：http://uu.521024.cn

t = time.perf_counter()
来源：http://lc.521024.cn

[U16] Py：命令行参数解析
来源：http://px.9csxet.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pe.huanxung.cn

[U17] Py：初始化日志
来源：http://wn.szxytkj.cn

logging.basicConfig(level=logging.INFO)
来源：http://jg.9csxet.cn

[U18] Py：预编译正则
来源：http://oh.jctech888.com.cn

pat = re.compile(r"\d+")
来源：http://fa.yuexingan06.cn

[U19] Py：正则替换带回调
来源：http://sj.hahajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zy.jctech888.com.cn

[U20] Py：缓存函数结果
来源：http://ra.panjiajie.cn

@functools.lru_cache(maxsize=None)
来源：http://iu.jctech888.com.cn

[U21] Py：自定义上下文管理器
来源：http://mb.szxytkj.cn

@contextlib.contextmanager
来源：http://pd.9csxet.cn

[U22] Py：矩阵转置
来源：http://zz.hahajie.cn

list(zip(*m))
来源：http://gu.huanxung.cn

[U23] Py：分块读取大文件
来源：http://pj.nicolike.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://si.szsharing.cn

[U24] Py：路径操作
来源：http://gx.shtwfgs.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://uf.chemitech.net.cn

[U25] Py：CSV 按字典读
来源：http://qu.asd995.cn

csv.DictReader(f)
来源：http://tn.newstarts.cn

[U26] Py：并发下载
来源：http://ke.szsharing.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rt.lnxyls.cn

[U27] Py：异步 HTTP
来源：http://ga.nicolike.cn

aiohttp.ClientSession() 配合 async with
来源：http://un.9csxet.cn

[U28] Py：类型别名
来源：http://pb.chemitech.net.cn

UserId = int
来源：http://pq.shtwfgs.cn

[U29] Py：属性校验
来源：http://ho.panjiajie.cn

@property 与 @x.setter 配合
来源：http://jh.521024.cn

[U30] Py：数据类
来源：http://wh.jianghongdianzi.cn

@dataclass(slots=True)
来源：http://ay.jctech888.com.cn

[U31] Py：单测
来源：http://cy.gzmigu.cn

python -m pytest -q
来源：http://ib.haigaiapp.cn

[U32] Py：代码格式化
来源：http://ta.haigaiapp.cn

ruff format . && ruff check --fix .
来源：http://bf.shtwfgs.cn

[U33] Py：打包发布
来源：http://au.shxzukj.cn

python -m build  （依赖 pyproject.toml）
来源：http://zy.huixiangedu.cn

[U34] Py：判断编码
来源：http://sg.wgjwhj.cn

chardet.detect(raw)
来源：http://pz.jctech888.com.cn

[U35] Py：发送邮件
来源：http://sz.bjjhwx.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cf.shxzukj.cn

[U36] Py：定时任务
来源：http://zf.bookmarksfly.cn

schedule.every(10).minutes.do(job)
来源：http://ml.szxytkj.cn

[U37] Py：读写 Excel
来源：http://jc.panjiajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://fe.hahajie.cn

[U38] Py：获取脚本所在目录
来源：http://tw.szsharing.cn

Path(__file__).resolve().parent
来源：http://ks.yuexingan06.cn

[U39] Py：判断是否在交互环境
来源：http://zz.szsharing.cn

sys.stdout.isatty()
来源：http://oz.chemitech.net.cn

[U40] Py：打印到标准错误
来源：http://tt.huixiangedu.cn

print("err", file=sys.stderr)
来源：http://sl.jctech888.com.cn

[U41] PHP：初始化 Composer 项目
来源：http://ht.jctech888.com.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xa.9csxet.cn

[U42] PHP：PSR-4 自动加载
来源：http://yj.hahajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yz.gzmigu.cn

[U43] PHP：声明命名空间
来源：http://nz.muxihuayi.cn

namespace App\Http;
来源：http://ff.shxzukj.cn

[U44] PHP：开启严格类型
来源：http://tk.bjjhwx.cn

declare(strict_types=1);
来源：http://qy.yuntaijiaju.cn

[U45] PHP：类型声明与返回类型
来源：http://wa.gzmigu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://xn.haigaiapp.cn

[U46] PHP：可空类型
来源：http://qc.9csxet.cn

?string $name = null
来源：http://gu.wgjwhj.cn

[U47] PHP：联合类型
来源：http://wr.shtwfgs.cn

int|string $id
来源：http://oc.colortex.cn

[U48] PHP：纯枚举
来源：http://sn.huixiangedu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gh.521024.cn

[U49] PHP：只读属性
来源：http://dp.yuntaijiaju.cn

public readonly string $name
来源：http://xu.hnjuh.cn

[U50] PHP：构造器属性提升
来源：http://ck.nicolike.cn

public function __construct(private int $id) {}
来源：http://fo.hnjuh.cn

[U51] PHP：数组解构
来源：http://uc.nicolike.cn

[$a, $b] = $arr;
来源：http://bz.hnjuh.cn

[U52] PHP：箭头函数
来源：http://xe.szxytkj.cn

$double = fn($x) => $x * 2;
来源：http://qq.bjjhwx.cn

[U53] PHP：空合并运算符
来源：http://eo.yuntaijiaju.cn

$v = $a ?? $b ?? "default";
来源：http://jw.chemitech.net.cn

[U54] PHP：空安全调用
来源：http://jc.muxihuayi.cn

$obj?->method()
来源：http://oa.9csxet.cn

[U55] PHP：match 表达式
来源：http://tk.huixinmuqiang.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dv.chemitech.net.cn

[U56] PHP：命名参数
来源：http://al.haigaiapp.cn

f(a: 1, b: 2)
来源：http://mf.panjiajie.cn

[U57] PHP：字符串插值
来源：http://ju.huixiangedu.cn

"值: {$a}"
来源：http://es.yuntaijiaju.cn

[U58] PHP：数组三件套
来源：http://fb.9csxet.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zp.shxzskj.cn

[U59] PHP：自定义排序
来源：http://ns.wgjwhj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fs.huixinmuqiang.cn

[U60] PHP：JSON 编解码
来源：http://eq.bookmarksfly.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qq.newstarts.cn

[U61] PHP：正则
来源：http://gt.newstarts.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://th.521024.cn

[U62] PHP：日期对象
来源：http://ak.nicolike.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yh.9csxet.cn

[U63] PHP：文件读写
来源：http://eu.panjiajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ab.muxihuayi.cn

[U64] PHP：目录遍历
来源：http://pq.jctech888.com.cn

glob("dir/*.php");  scandir("dir");
来源：http://zt.nszjky.cn

[U65] PHP：会话
来源：http://tc.jianghongdianzi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://cy.colortex.cn

[U66] PHP：设置 Cookie
来源：http://vf.szxytkj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ef.521024.cn

[U67] PHP：处理文件上传
来源：http://hc.newstarts.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vf.hnjuh.cn

[U68] PHP：PDO 连接
来源：http://kf.gzmigu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fq.chemitech.net.cn

[U69] PHP：PDO 预处理
来源：http://em.asd995.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://oz.yuexingan06.cn

[U70] PHP：PDO 事务
来源：http://bb.colortex.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xw.hnjuh.cn

[U71] PHP：抛出异常
来源：http://ob.haigaiapp.cn

throw new RuntimeException("失败", 500);
来源：http://et.haigaiapp.cn

[U72] PHP：写错误日志
来源：http://jv.yuntaijiaju.cn

error_log("失败: " . $e->getMessage());
来源：http://jy.szxytkj.cn

[U73] PHP：读取 ini 配置
来源：http://so.haigaiapp.cn

parse_ini_file("config.ini", true)
来源：http://nm.colortex.cn

[U74] PHP：读取环境变量
来源：http://iv.yuntaijiaju.cn

getenv("APP_ENV") ?: "production"
来源：http://uo.asd995.cn

[U75] PHP：依赖注入
来源：http://rj.muxihuayi.cn

composer require psr/container
来源：http://oi.haigaiapp.cn

[U76] PHP：简单路由
来源：http://uz.shxzukj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nm.hnjuh.cn

[U77] PHP：模板渲染
来源：http://qt.muxihuayi.cn

composer require twig/twig
来源：http://fw.shtwfgs.cn

[U78] PHP：单元测试
来源：http://mp.yuexingan06.cn

composer require --dev phpunit/phpunit
来源：http://mn.gzmigu.cn

[U79] PHP：静态分析
来源：http://mx.colortex.cn

composer require --dev phpstan/phpstan
来源：http://lv.bjjhwx.cn

[U80] PHP：代码规范修复
来源：http://nu.bookmarksfly.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://he.asd995.cn

[U81] JS：初始化项目
来源：http://wn.gzmigu.cn

npm init -y;  npm i express
来源：http://uq.newstarts.cn

[U82] JS：package.json 脚本
来源：http://yj.shxzukj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nh.huixinmuqiang.cn

[U83] JS：ES Module 导入导出
来源：http://hq.wgjwhj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ue.bjjhwx.cn

[U84] JS：CommonJS 写法
来源：http://cn.521024.cn

module.exports = { a };  const { a } = require("./m");
来源：http://hd.jctech888.com.cn

[U85] JS：可选链
来源：http://nt.panjiajie.cn

a?.b?.c
来源：http://tn.nicolike.cn

[U86] JS：空值合并
来源：http://rx.muxihuayi.cn

a ?? b
来源：http://vw.huixiangedu.cn

[U87] JS：解构默认值
来源：http://cw.shxzskj.cn

const { a = 1, b = 2 } = obj;
来源：http://lt.shxzskj.cn

[U88] JS：对象展开合并
来源：http://et.nicolike.cn

{ ...a, ...b }
来源：http://dl.huanxung.cn

[U89] JS：数组去重
来源：http://wx.nicolike.cn

[...new Set(arr)]
来源：http://hu.521024.cn

[U90] JS：数字数组排序
来源：http://ey.colortex.cn

[...arr].sort((a, b) => a - b)
来源：http://tq.hahajie.cn

[U91] JS：对象键值遍历
来源：http://um.huanxung.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gm.shtwfgs.cn

[U92] JS：深拷贝
来源：http://ut.szsharing.cn

structuredClone(obj)
来源：http://pi.nicolike.cn

[U93] JS：模板字符串
来源：http://ux.lnxyls.cn

`共 ${n} 条`
来源：http://te.wgjwhj.cn

[U94] JS：箭头函数
来源：http://td.jianghongdianzi.cn

const double = x => x * 2;
来源：http://al.shxzukj.cn

[U95] JS：Promise 包装
来源：http://hi.newstarts.cn

new Promise((resolve, reject) => {})
来源：http://cb.huanxung.cn

[U96] JS：async/await 与异常
来源：http://ot.bjjhwx.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ir.bjjhwx.cn

[U97] JS：并发请求
来源：http://nm.nszjky.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bz.yuexingan06.cn

[U98] JS：fetch 带 JSON
来源：http://ns.521024.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cd.bjjhwx.cn

[U99] JS：事件监听
来源：http://ew.lnxyls.cn

el.addEventListener("click", e => {})
来源：http://xp.shxzskj.cn

[U100] JS：DOM 查询
来源：http://vk.jctech888.com.cn

document.querySelector(".item")
来源：http://md.shxzskj.cn

[U101] JS：classList 操作
来源：http://vd.yuntaijiaju.cn

el.classList.toggle("active")
来源：http://lo.huanxung.cn

[U102] JS：本地存储
来源：http://rh.haigaiapp.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://rn.shtwfgs.cn

[U103] JS：定时器
来源：http://pd.huanxung.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yq.jctech888.com.cn

[U104] JS：防抖
来源：http://ub.szsharing.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pe.huixinmuqiang.cn

[U105] JS：节流
来源：http://fk.jctech888.com.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gm.huixiangedu.cn

[U106] JS：日期格式化
来源：http://pv.haigaiapp.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nw.panjiajie.cn


<!-- 参考信息 -->