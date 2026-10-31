代发 wailian999

[T11] Kotlin：协程
来源：http://hx.nszjky.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xg.shxzskj.cn

[T12] Kotlin：解构声明
来源：http://mx.colortex.cn

val (a, b) = Pair(1, 2)
来源：http://ic.muxihuayi.cn

[T13] Kotlin：只读 Map
来源：http://uc.bookmarksfly.cn

val m = mapOf("a" to 1)
来源：http://ss.szsharing.cn

[T14] Kotlin：循环
来源：http://zs.nicolike.cn

for (i in 1..10) println(i)
来源：http://mz.jianghongdianzi.cn

[T15] Kotlin：接口
来源：http://bo.521024.cn

interface Shape { fun area(): Double }
来源：http://ax.huanxung.cn

[T16] Swift：Hello World
来源：http://sh.yuntaijiaju.cn

print("Hello")
来源：http://bx.wgjwhj.cn

[T17] Swift：变量与常量
来源：http://eg.yuntaijiaju.cn

var a = 1;  let b = 2
来源：http://vq.huixinmuqiang.cn

[T18] Swift：字符串插值
来源：http://mj.chemitech.net.cn

"值: \(b)"
来源：http://xx.bjjhwx.cn

[T19] Swift：可选绑定
来源：http://df.szxytkj.cn

if let n = opt { print(n) }
来源：http://bj.9csxet.cn

[T20] Swift：数组操作
来源：http://yw.jianghongdianzi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://si.gzmigu.cn

[T21] Swift：遍历
来源：http://xd.colortex.cn

for x in a { print(x) }
来源：http://nh.panjiajie.cn

[T22] Swift：字典
来源：http://ax.wgjwhj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://oo.gzmigu.cn

[T23] Swift：函数
来源：http://nl.shxzskj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jq.huixinmuqiang.cn

[T24] Swift：闭包
来源：http://gh.muxihuayi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xz.jianghongdianzi.cn

[T25] Swift：结构体
来源：http://na.jctech888.com.cn

struct P { var x: Int }
来源：http://to.shtwfgs.cn

[T26] Swift：类与重写
来源：http://qn.yuntaijiaju.cn

class A: Base { override func f() {} }
来源：http://qw.bookmarksfly.cn

[T27] Swift：错误处理
来源：http://pc.hnjuh.cn

do { try f() } catch { print(error) }
来源：http://ux.yuntaijiaju.cn

[T28] Swift：枚举
来源：http://dg.shtwfgs.cn

enum Color { case red, green }
来源：http://su.hahajie.cn

[T29] Swift：guard 提前返回
来源：http://ye.shxzukj.cn

guard let x = opt else { return }
来源：http://xu.asd995.cn

[T30] Swift：协议
来源：http://mr.huanxung.cn

protocol Shape { func area() -> Double }
来源：http://iq.szxytkj.cn

[T31] Lua：Hello World
来源：http://jf.panjiajie.cn

print("Hello")
来源：http://vq.szxytkj.cn

[T32] Lua：局部变量
来源：http://lf.huixiangedu.cn

local a = 1
来源：http://lq.huixinmuqiang.cn

[T33] Lua：表（数组）
来源：http://xs.9csxet.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hx.lnxyls.cn

[T34] Lua：遍历表
来源：http://gi.huanxung.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ng.yuntaijiaju.cn

[T35] Lua：字典表
来源：http://od.nicolike.cn

local d = { a = 1 };  d.b = 2
来源：http://lu.lnxyls.cn

[T36] Lua：函数
来源：http://or.jianghongdianzi.cn

function add(a, b) return a + b end
来源：http://is.szxytkj.cn

[T37] Lua：字符串拼接
来源：http://jd.hahajie.cn

"a" .. "b"
来源：http://nf.lnxyls.cn

[T38] Lua：条件
来源：http://ly.bjjhwx.cn

if x > 0 then print("正") end
来源：http://ao.haigaiapp.cn

[T39] Lua：模式匹配
来源：http://ie.yuexingan06.cn

string.find(s, "%d+")
来源：http://gi.newstarts.cn

[T40] Lua：元表
来源：http://ei.huixiangedu.cn

setmetatable({}, { __index = base })
来源：http://cu.szxytkj.cn

[T41] Perl：Hello World
来源：http://ja.shtwfgs.cn

print "Hello\n";
来源：http://nr.jianghongdianzi.cn

[T42] Perl：变量类型
来源：http://cv.nicolike.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ar.szxytkj.cn

[T43] Perl：字符串插值
来源：http://ue.hnjuh.cn

"值: $a"
来源：http://sg.9csxet.cn

[T44] Perl：条件
来源：http://uz.chemitech.net.cn

if ($a > 0) { print "正"; }
来源：http://qs.asd995.cn

[T45] Perl：数组遍历
来源：http://ph.9csxet.cn

for my $x (@arr) { print $x; }
来源：http://ba.haigaiapp.cn

[T46] Perl：哈希操作
来源：http://mc.lnxyls.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cd.nicolike.cn

[T47] Perl：正则捕获
来源：http://ll.panjiajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ms.hnjuh.cn

[T48] Perl：正则替换
来源：http://jy.huixiangedu.cn

$s =~ s/old/new/g;
来源：http://bg.jianghongdianzi.cn

[T49] Perl：函数
来源：http://na.szsharing.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://oi.hahajie.cn

[T50] Perl：逐行读文件
来源：http://vc.bjjhwx.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fx.shxzskj.cn

while (my $line = <$fh>) { print $line; }
来源：http://mc.huixinmuqiang.cn

[T51] Scala：Hello World
来源：http://qs.521024.cn

println("Hello")
来源：http://gm.bookmarksfly.cn

[T52] Scala：变量
来源：http://tu.jctech888.com.cn

val a = 1;  var b = 2
来源：http://il.chemitech.net.cn

[T53] Scala：字符串插值
来源：http://fd.hnjuh.cn

s"值: $b"
来源：http://ma.colortex.cn

[T54] Scala：集合映射
来源：http://ui.hnjuh.cn

List(1, 2, 3).map(_ * 2)
来源：http://bb.asd995.cn

[T55] Scala：集合过滤
来源：http://ue.shxzukj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://pp.bookmarksfly.cn

[T56] Scala：样例类
来源：http://nc.lnxyls.cn

case class User(name: String, age: Int)
来源：http://ch.shxzskj.cn

[T57] Scala：模式匹配
来源：http://cd.szsharing.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://rk.newstarts.cn

[T58] Scala：函数定义
来源：http://wc.nszjky.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ne.colortex.cn

[T59] Scala：循环
来源：http://rj.wgjwhj.cn

for (i <- 1 to 10) println(i)
来源：http://mh.hahajie.cn

[T60] Scala：折叠
来源：http://pt.bjjhwx.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ew.nszjky.cn

================================================================================
来源：http://nq.colortex.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mq.nszjky.cn

================================================================================
来源：http://go.huixiangedu.cn

[U01] Py：创建虚拟环境
来源：http://rr.huixiangedu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://lx.shxzskj.cn

[U02] Py：导出 / 安装依赖
来源：http://lb.shxzukj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://un.shxzukj.cn

[U03] Py：加载 .env 配置
来源：http://oc.jianghongdianzi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rm.hahajie.cn

[U04] Py：变量调试打印
来源：http://ri.nszjky.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ew.nszjky.cn

[U05] Py：列表去重且保序
来源：http://be.shxzukj.cn

list(dict.fromkeys(arr))
来源：http://ge.muxihuayi.cn

[U06] Py：合并两个字典
来源：http://uy.gzmigu.cn

{**a, **b}
来源：http://yi.jctech888.com.cn

[U07] Py：反转字典键值
来源：http://it.huixinmuqiang.cn

{v: k for k, v in d.items()}
来源：http://fz.jianghongdianzi.cn

[U08] Py：展平二维列表
来源：http://qy.lnxyls.cn

[y for x in nested for y in x]
来源：http://eh.521024.cn

[U09] Py：字典取最大值的键
来源：http://nx.chemitech.net.cn

max(d, key=d.get)
来源：http://uc.521024.cn

[U10] Py：按值排序字典
来源：http://wx.huixinmuqiang.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://oo.bookmarksfly.cn

[U11] Py：生成器表达式
来源：http://lm.bookmarksfly.cn

(x * 2 for x in arr)
来源：http://lf.huixiangedu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://yk.chemitech.net.cn

Counter(arr).most_common(3)
来源：http://rt.yuntaijiaju.cn

[U13] Py：固定长度队列
来源：http://iq.panjiajie.cn

deque(maxlen=10)
来源：http://ip.jianghongdianzi.cn

[U14] Py：分组收集到列表
来源：http://mh.szsharing.cn

defaultdict(list)
来源：http://ej.chemitech.net.cn

[U15] Py：高精度计时
来源：http://iz.yuntaijiaju.cn

t = time.perf_counter()
来源：http://hr.gzmigu.cn

[U16] Py：命令行参数解析
来源：http://sp.bookmarksfly.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ww.muxihuayi.cn

[U17] Py：初始化日志
来源：http://sx.9csxet.cn

logging.basicConfig(level=logging.INFO)
来源：http://sp.newstarts.cn

[U18] Py：预编译正则
来源：http://su.hnjuh.cn

pat = re.compile(r"\d+")
来源：http://jg.9csxet.cn

[U19] Py：正则替换带回调
来源：http://cb.521024.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jd.huanxung.cn

[U20] Py：缓存函数结果
来源：http://tq.huanxung.cn

@functools.lru_cache(maxsize=None)
来源：http://ni.jianghongdianzi.cn

[U21] Py：自定义上下文管理器
来源：http://lw.newstarts.cn

@contextlib.contextmanager
来源：http://sf.jctech888.com.cn

[U22] Py：矩阵转置
来源：http://ut.bjjhwx.cn

list(zip(*m))
来源：http://fk.jctech888.com.cn

[U23] Py：分块读取大文件
来源：http://wt.chemitech.net.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bi.yuntaijiaju.cn

[U24] Py：路径操作
来源：http://bc.yuntaijiaju.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hu.gzmigu.cn

[U25] Py：CSV 按字典读
来源：http://pr.huixinmuqiang.cn

csv.DictReader(f)
来源：http://bi.shxzskj.cn

[U26] Py：并发下载
来源：http://eq.chemitech.net.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gb.jctech888.com.cn

[U27] Py：异步 HTTP
来源：http://da.hahajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://xz.colortex.cn

[U28] Py：类型别名
来源：http://ej.szsharing.cn

UserId = int
来源：http://gh.jianghongdianzi.cn

[U29] Py：属性校验
来源：http://ia.shxzskj.cn

@property 与 @x.setter 配合
来源：http://ny.yuntaijiaju.cn

[U30] Py：数据类
来源：http://yf.huixiangedu.cn

@dataclass(slots=True)
来源：http://hq.asd995.cn

[U31] Py：单测
来源：http://ep.jctech888.com.cn

python -m pytest -q
来源：http://cr.lnxyls.cn

[U32] Py：代码格式化
来源：http://yf.gzmigu.cn

ruff format . && ruff check --fix .
来源：http://kf.lnxyls.cn

[U33] Py：打包发布
来源：http://zj.yuexingan06.cn

python -m build  （依赖 pyproject.toml）
来源：http://pi.yuntaijiaju.cn

[U34] Py：判断编码
来源：http://rz.yuntaijiaju.cn

chardet.detect(raw)
来源：http://to.gzmigu.cn

[U35] Py：发送邮件
来源：http://qr.shxzukj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hd.shxzukj.cn

[U36] Py：定时任务
来源：http://bi.hahajie.cn

schedule.every(10).minutes.do(job)
来源：http://ye.gzmigu.cn

[U37] Py：读写 Excel
来源：http://ov.muxihuayi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://vh.yuntaijiaju.cn

[U38] Py：获取脚本所在目录
来源：http://pt.panjiajie.cn

Path(__file__).resolve().parent
来源：http://zn.huixinmuqiang.cn

[U39] Py：判断是否在交互环境
来源：http://es.yuexingan06.cn

sys.stdout.isatty()
来源：http://gc.lnxyls.cn

[U40] Py：打印到标准错误
来源：http://kw.szsharing.cn

print("err", file=sys.stderr)
来源：http://jj.gzmigu.cn

[U41] PHP：初始化 Composer 项目
来源：http://se.chemitech.net.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://aa.bjjhwx.cn

[U42] PHP：PSR-4 自动加载
来源：http://cn.wgjwhj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gi.huixiangedu.cn

[U43] PHP：声明命名空间
来源：http://cy.jianghongdianzi.cn

namespace App\Http;
来源：http://fl.9csxet.cn

[U44] PHP：开启严格类型
来源：http://zb.szxytkj.cn

declare(strict_types=1);
来源：http://sa.huixiangedu.cn

[U45] PHP：类型声明与返回类型
来源：http://tj.nicolike.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://if.nszjky.cn

[U46] PHP：可空类型
来源：http://cv.9csxet.cn

?string $name = null
来源：http://cy.gzmigu.cn

[U47] PHP：联合类型
来源：http://st.huanxung.cn

int|string $id
来源：http://oc.haigaiapp.cn

[U48] PHP：纯枚举
来源：http://wr.haigaiapp.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rn.nicolike.cn

[U49] PHP：只读属性
来源：http://qa.szxytkj.cn

public readonly string $name
来源：http://lb.hnjuh.cn

[U50] PHP：构造器属性提升
来源：http://il.jctech888.com.cn

public function __construct(private int $id) {}
来源：http://lj.newstarts.cn

[U51] PHP：数组解构
来源：http://ky.asd995.cn

[$a, $b] = $arr;
来源：http://qe.szxytkj.cn

[U52] PHP：箭头函数
来源：http://ek.hahajie.cn

$double = fn($x) => $x * 2;
来源：http://km.colortex.cn

[U53] PHP：空合并运算符
来源：http://uy.nszjky.cn

$v = $a ?? $b ?? "default";
来源：http://cg.szxytkj.cn

[U54] PHP：空安全调用
来源：http://wn.shxzskj.cn

$obj?->method()
来源：http://xh.newstarts.cn

[U55] PHP：match 表达式
来源：http://ms.yuntaijiaju.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://sc.bjjhwx.cn

[U56] PHP：命名参数
来源：http://up.9csxet.cn

f(a: 1, b: 2)
来源：http://ji.gzmigu.cn

[U57] PHP：字符串插值
来源：http://kx.521024.cn

"值: {$a}"
来源：http://kf.hahajie.cn

[U58] PHP：数组三件套
来源：http://im.gzmigu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://sb.szxytkj.cn

[U59] PHP：自定义排序
来源：http://hs.panjiajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pr.hahajie.cn

[U60] PHP：JSON 编解码
来源：http://rg.jianghongdianzi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hp.gzmigu.cn

[U61] PHP：正则
来源：http://ks.nszjky.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zd.shxzskj.cn

[U62] PHP：日期对象
来源：http://bx.lnxyls.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vk.yuntaijiaju.cn

[U63] PHP：文件读写
来源：http://ul.521024.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ap.colortex.cn

[U64] PHP：目录遍历
来源：http://oe.haigaiapp.cn

glob("dir/*.php");  scandir("dir");
来源：http://jq.bjjhwx.cn

[U65] PHP：会话
来源：http://iz.huixinmuqiang.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://gf.lnxyls.cn

[U66] PHP：设置 Cookie
来源：http://gx.huixinmuqiang.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nw.9csxet.cn

[U67] PHP：处理文件上传
来源：http://zh.szxytkj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fb.muxihuayi.cn

[U68] PHP：PDO 连接
来源：http://fv.nszjky.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ab.colortex.cn

[U69] PHP：PDO 预处理
来源：http://rz.huixiangedu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yf.hnjuh.cn

[U70] PHP：PDO 事务
来源：http://gk.muxihuayi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qy.haigaiapp.cn

[U71] PHP：抛出异常
来源：http://oe.szsharing.cn

throw new RuntimeException("失败", 500);
来源：http://og.panjiajie.cn

[U72] PHP：写错误日志
来源：http://pc.haigaiapp.cn

error_log("失败: " . $e->getMessage());
来源：http://kb.521024.cn

[U73] PHP：读取 ini 配置
来源：http://gt.muxihuayi.cn

parse_ini_file("config.ini", true)
来源：http://dy.yuexingan06.cn

[U74] PHP：读取环境变量
来源：http://rp.haigaiapp.cn

getenv("APP_ENV") ?: "production"
来源：http://pi.huixinmuqiang.cn

[U75] PHP：依赖注入
来源：http://au.szxytkj.cn

composer require psr/container
来源：http://fo.hahajie.cn

[U76] PHP：简单路由
来源：http://pj.haigaiapp.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xi.jctech888.com.cn

[U77] PHP：模板渲染
来源：http://yb.haigaiapp.cn

composer require twig/twig
来源：http://zl.nicolike.cn

[U78] PHP：单元测试
来源：http://mm.shxzukj.cn

composer require --dev phpunit/phpunit
来源：http://nn.szsharing.cn

[U79] PHP：静态分析
来源：http://os.yuexingan06.cn

composer require --dev phpstan/phpstan
来源：http://sm.jctech888.com.cn

[U80] PHP：代码规范修复
来源：http://xx.bjjhwx.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ww.newstarts.cn

[U81] JS：初始化项目
来源：http://od.huixinmuqiang.cn

npm init -y;  npm i express
来源：http://kk.gzmigu.cn

[U82] JS：package.json 脚本
来源：http://mj.haigaiapp.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vn.huixiangedu.cn

[U83] JS：ES Module 导入导出
来源：http://uo.colortex.cn

export const a = 1;  import { a } from "./m.js";
来源：http://wo.yuntaijiaju.cn

[U84] JS：CommonJS 写法
来源：http://lx.haigaiapp.cn

module.exports = { a };  const { a } = require("./m");
来源：http://zt.chemitech.net.cn

[U85] JS：可选链
来源：http://pi.haigaiapp.cn

a?.b?.c
来源：http://ei.shxzskj.cn

[U86] JS：空值合并
来源：http://yd.521024.cn

a ?? b
来源：http://ey.szxytkj.cn

[U87] JS：解构默认值
来源：http://mp.nicolike.cn

const { a = 1, b = 2 } = obj;
来源：http://wo.nicolike.cn

[U88] JS：对象展开合并
来源：http://fj.muxihuayi.cn

{ ...a, ...b }
来源：http://ez.yuexingan06.cn

[U89] JS：数组去重
来源：http://vf.muxihuayi.cn

[...new Set(arr)]
来源：http://zc.yuntaijiaju.cn

[U90] JS：数字数组排序
来源：http://wq.yuexingan06.cn

[...arr].sort((a, b) => a - b)
来源：http://tp.yuntaijiaju.cn

[U91] JS：对象键值遍历
来源：http://ro.jctech888.com.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xh.jctech888.com.cn

[U92] JS：深拷贝
来源：http://dp.nszjky.cn

structuredClone(obj)
来源：http://oa.gzmigu.cn

[U93] JS：模板字符串
来源：http://wd.bjjhwx.cn

`共 ${n} 条`
来源：http://rv.hnjuh.cn

[U94] JS：箭头函数
来源：http://yq.chemitech.net.cn

const double = x => x * 2;
来源：http://pw.9csxet.cn

[U95] JS：Promise 包装
来源：http://vs.muxihuayi.cn

new Promise((resolve, reject) => {})
来源：http://og.nszjky.cn

[U96] JS：async/await 与异常
来源：http://em.lnxyls.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ew.asd995.cn

[U97] JS：并发请求
来源：http://qc.9csxet.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ze.lnxyls.cn

[U98] JS：fetch 带 JSON
来源：http://su.wgjwhj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qd.521024.cn


<!-- 参考信息 -->