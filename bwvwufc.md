代发 wailian999

[T19] Swift：可选绑定
来源：http://nd.521024.cn

if let n = opt { print(n) }
来源：http://xm.panjiajie.cn

[T20] Swift：数组操作
来源：http://sp.huanxung.cn

var a = [1, 2, 3];  a.append(4)
来源：http://cn.lnxyls.cn

[T21] Swift：遍历
来源：http://dv.muxihuayi.cn

for x in a { print(x) }
来源：http://ir.shtwfgs.cn

[T22] Swift：字典
来源：http://jz.shxzskj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://jz.shxzskj.cn

[T23] Swift：函数
来源：http://br.huanxung.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dn.9csxet.cn

[T24] Swift：闭包
来源：http://xb.muxihuayi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://cd.jctech888.com.cn

[T25] Swift：结构体
来源：http://fv.shxzskj.cn

struct P { var x: Int }
来源：http://zd.9csxet.cn

[T26] Swift：类与重写
来源：http://oz.huanxung.cn

class A: Base { override func f() {} }
来源：http://si.hnjuh.cn

[T27] Swift：错误处理
来源：http://oa.nicolike.cn

do { try f() } catch { print(error) }
来源：http://ep.nszjky.cn

[T28] Swift：枚举
来源：http://wg.jctech888.com.cn

enum Color { case red, green }
来源：http://oc.haigaiapp.cn

[T29] Swift：guard 提前返回
来源：http://xw.lnxyls.cn

guard let x = opt else { return }
来源：http://xp.nicolike.cn

[T30] Swift：协议
来源：http://kl.shxzskj.cn

protocol Shape { func area() -> Double }
来源：http://xu.521024.cn

[T31] Lua：Hello World
来源：http://kq.yuexingan06.cn

print("Hello")
来源：http://ky.shtwfgs.cn

[T32] Lua：局部变量
来源：http://xb.panjiajie.cn

local a = 1
来源：http://gm.hnjuh.cn

[T33] Lua：表（数组）
来源：http://jj.nszjky.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://an.nszjky.cn

[T34] Lua：遍历表
来源：http://oa.asd995.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://uv.haigaiapp.cn

[T35] Lua：字典表
来源：http://ht.lnxyls.cn

local d = { a = 1 };  d.b = 2
来源：http://va.szsharing.cn

[T36] Lua：函数
来源：http://qx.szsharing.cn

function add(a, b) return a + b end
来源：http://zv.haigaiapp.cn

[T37] Lua：字符串拼接
来源：http://fo.panjiajie.cn

"a" .. "b"
来源：http://dx.shxzskj.cn

[T38] Lua：条件
来源：http://yf.lnxyls.cn

if x > 0 then print("正") end
来源：http://dt.huanxung.cn

[T39] Lua：模式匹配
来源：http://de.lnxyls.cn

string.find(s, "%d+")
来源：http://rl.chemitech.net.cn

[T40] Lua：元表
来源：http://cd.huanxung.cn

setmetatable({}, { __index = base })
来源：http://if.chemitech.net.cn

[T41] Perl：Hello World
来源：http://ws.jianghongdianzi.cn

print "Hello\n";
来源：http://dq.szsharing.cn

[T42] Perl：变量类型
来源：http://kc.521024.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yx.newstarts.cn

[T43] Perl：字符串插值
来源：http://db.hahajie.cn

"值: $a"
来源：http://kr.panjiajie.cn

[T44] Perl：条件
来源：http://yk.nicolike.cn

if ($a > 0) { print "正"; }
来源：http://aj.huixinmuqiang.cn

[T45] Perl：数组遍历
来源：http://bg.muxihuayi.cn

for my $x (@arr) { print $x; }
来源：http://bd.szsharing.cn

[T46] Perl：哈希操作
来源：http://um.hahajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ps.szxytkj.cn

[T47] Perl：正则捕获
来源：http://df.haigaiapp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xj.shtwfgs.cn

[T48] Perl：正则替换
来源：http://lr.yuntaijiaju.cn

$s =~ s/old/new/g;
来源：http://ql.9csxet.cn

[T49] Perl：函数
来源：http://mr.nszjky.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ps.huixinmuqiang.cn

[T50] Perl：逐行读文件
来源：http://qp.colortex.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ex.szsharing.cn

while (my $line = <$fh>) { print $line; }
来源：http://lb.yuexingan06.cn

[T51] Scala：Hello World
来源：http://sp.shtwfgs.cn

println("Hello")
来源：http://yu.chemitech.net.cn

[T52] Scala：变量
来源：http://du.gzmigu.cn

val a = 1;  var b = 2
来源：http://xi.colortex.cn

[T53] Scala：字符串插值
来源：http://mz.jianghongdianzi.cn

s"值: $b"
来源：http://bw.jianghongdianzi.cn

[T54] Scala：集合映射
来源：http://ov.huixiangedu.cn

List(1, 2, 3).map(_ * 2)
来源：http://sv.shxzskj.cn

[T55] Scala：集合过滤
来源：http://yz.nszjky.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ju.wgjwhj.cn

[T56] Scala：样例类
来源：http://sb.lnxyls.cn

case class User(name: String, age: Int)
来源：http://ge.nszjky.cn

[T57] Scala：模式匹配
来源：http://qs.nszjky.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://hi.gzmigu.cn

[T58] Scala：函数定义
来源：http://fh.newstarts.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ln.nicolike.cn

[T59] Scala：循环
来源：http://aj.jctech888.com.cn

for (i <- 1 to 10) println(i)
来源：http://tl.9csxet.cn

[T60] Scala：折叠
来源：http://nt.jctech888.com.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://op.newstarts.cn

================================================================================
来源：http://oe.lnxyls.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://da.lnxyls.cn

================================================================================
来源：http://pv.bookmarksfly.cn

[U01] Py：创建虚拟环境
来源：http://wa.huixiangedu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mz.szsharing.cn

[U02] Py：导出 / 安装依赖
来源：http://bz.bookmarksfly.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yj.bjjhwx.cn

[U03] Py：加载 .env 配置
来源：http://cb.newstarts.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://pd.wgjwhj.cn

[U04] Py：变量调试打印
来源：http://gh.yuntaijiaju.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://yx.jctech888.com.cn

[U05] Py：列表去重且保序
来源：http://hk.521024.cn

list(dict.fromkeys(arr))
来源：http://ds.panjiajie.cn

[U06] Py：合并两个字典
来源：http://ug.shtwfgs.cn

{**a, **b}
来源：http://qz.huixinmuqiang.cn

[U07] Py：反转字典键值
来源：http://sb.chemitech.net.cn

{v: k for k, v in d.items()}
来源：http://nh.szxytkj.cn

[U08] Py：展平二维列表
来源：http://ge.asd995.cn

[y for x in nested for y in x]
来源：http://cb.colortex.cn

[U09] Py：字典取最大值的键
来源：http://ee.newstarts.cn

max(d, key=d.get)
来源：http://zo.huixinmuqiang.cn

[U10] Py：按值排序字典
来源：http://br.lnxyls.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jk.muxihuayi.cn

[U11] Py：生成器表达式
来源：http://me.yuexingan06.cn

(x * 2 for x in arr)
来源：http://gl.panjiajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ss.huixiangedu.cn

Counter(arr).most_common(3)
来源：http://xd.jctech888.com.cn

[U13] Py：固定长度队列
来源：http://lf.colortex.cn

deque(maxlen=10)
来源：http://rn.jianghongdianzi.cn

[U14] Py：分组收集到列表
来源：http://og.hnjuh.cn

defaultdict(list)
来源：http://zd.jctech888.com.cn

[U15] Py：高精度计时
来源：http://xq.szxytkj.cn

t = time.perf_counter()
来源：http://ly.yuexingan06.cn

[U16] Py：命令行参数解析
来源：http://bq.haigaiapp.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ww.bookmarksfly.cn

[U17] Py：初始化日志
来源：http://ai.wgjwhj.cn

logging.basicConfig(level=logging.INFO)
来源：http://xt.haigaiapp.cn

[U18] Py：预编译正则
来源：http://mu.asd995.cn

pat = re.compile(r"\d+")
来源：http://et.szsharing.cn

[U19] Py：正则替换带回调
来源：http://qm.bjjhwx.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sk.asd995.cn

[U20] Py：缓存函数结果
来源：http://pj.shtwfgs.cn

@functools.lru_cache(maxsize=None)
来源：http://bj.nszjky.cn

[U21] Py：自定义上下文管理器
来源：http://gr.panjiajie.cn

@contextlib.contextmanager
来源：http://to.521024.cn

[U22] Py：矩阵转置
来源：http://oa.lnxyls.cn

list(zip(*m))
来源：http://za.nszjky.cn

[U23] Py：分块读取大文件
来源：http://un.szxytkj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hf.shxzukj.cn

[U24] Py：路径操作
来源：http://hv.nszjky.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://we.asd995.cn

[U25] Py：CSV 按字典读
来源：http://pl.shtwfgs.cn

csv.DictReader(f)
来源：http://fb.lnxyls.cn

[U26] Py：并发下载
来源：http://sf.szsharing.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rp.nicolike.cn

[U27] Py：异步 HTTP
来源：http://ts.nszjky.cn

aiohttp.ClientSession() 配合 async with
来源：http://wa.shxzskj.cn

[U28] Py：类型别名
来源：http://lm.haigaiapp.cn

UserId = int
来源：http://ky.bookmarksfly.cn

[U29] Py：属性校验
来源：http://lo.muxihuayi.cn

@property 与 @x.setter 配合
来源：http://jz.yuexingan06.cn

[U30] Py：数据类
来源：http://at.szxytkj.cn

@dataclass(slots=True)
来源：http://db.colortex.cn

[U31] Py：单测
来源：http://ka.shxzukj.cn

python -m pytest -q
来源：http://dl.9csxet.cn

[U32] Py：代码格式化
来源：http://rq.nicolike.cn

ruff format . && ruff check --fix .
来源：http://wm.haigaiapp.cn

[U33] Py：打包发布
来源：http://ai.huixinmuqiang.cn

python -m build  （依赖 pyproject.toml）
来源：http://yg.nszjky.cn

[U34] Py：判断编码
来源：http://fy.szsharing.cn

chardet.detect(raw)
来源：http://vk.yuexingan06.cn

[U35] Py：发送邮件
来源：http://ep.hahajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pp.szxytkj.cn

[U36] Py：定时任务
来源：http://mo.chemitech.net.cn

schedule.every(10).minutes.do(job)
来源：http://dj.bjjhwx.cn

[U37] Py：读写 Excel
来源：http://ry.jianghongdianzi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ts.jianghongdianzi.cn

[U38] Py：获取脚本所在目录
来源：http://fa.newstarts.cn

Path(__file__).resolve().parent
来源：http://jj.asd995.cn

[U39] Py：判断是否在交互环境
来源：http://tj.9csxet.cn

sys.stdout.isatty()
来源：http://wq.yuntaijiaju.cn

[U40] Py：打印到标准错误
来源：http://dd.nicolike.cn

print("err", file=sys.stderr)
来源：http://ec.shxzukj.cn

[U41] PHP：初始化 Composer 项目
来源：http://to.nicolike.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qw.yuexingan06.cn

[U42] PHP：PSR-4 自动加载
来源：http://jn.newstarts.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hl.nicolike.cn

[U43] PHP：声明命名空间
来源：http://wg.shxzukj.cn

namespace App\Http;
来源：http://cl.521024.cn

[U44] PHP：开启严格类型
来源：http://jh.shxzukj.cn

declare(strict_types=1);
来源：http://zs.521024.cn

[U45] PHP：类型声明与返回类型
来源：http://ld.lnxyls.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ky.yuntaijiaju.cn

[U46] PHP：可空类型
来源：http://gb.shtwfgs.cn

?string $name = null
来源：http://ln.muxihuayi.cn

[U47] PHP：联合类型
来源：http://xs.huixinmuqiang.cn

int|string $id
来源：http://lk.bookmarksfly.cn

[U48] PHP：纯枚举
来源：http://ov.newstarts.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hs.nicolike.cn

[U49] PHP：只读属性
来源：http://wq.yuntaijiaju.cn

public readonly string $name
来源：http://pd.yuexingan06.cn

[U50] PHP：构造器属性提升
来源：http://fm.bookmarksfly.cn

public function __construct(private int $id) {}
来源：http://gj.nszjky.cn

[U51] PHP：数组解构
来源：http://ep.haigaiapp.cn

[$a, $b] = $arr;
来源：http://py.hnjuh.cn

[U52] PHP：箭头函数
来源：http://zd.muxihuayi.cn

$double = fn($x) => $x * 2;
来源：http://wu.huixiangedu.cn

[U53] PHP：空合并运算符
来源：http://uw.bookmarksfly.cn

$v = $a ?? $b ?? "default";
来源：http://vk.gzmigu.cn

[U54] PHP：空安全调用
来源：http://lp.bookmarksfly.cn

$obj?->method()
来源：http://eo.muxihuayi.cn

[U55] PHP：match 表达式
来源：http://ug.huixiangedu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ll.asd995.cn

[U56] PHP：命名参数
来源：http://kn.huixiangedu.cn

f(a: 1, b: 2)
来源：http://wt.bjjhwx.cn

[U57] PHP：字符串插值
来源：http://hx.nszjky.cn

"值: {$a}"
来源：http://wk.hnjuh.cn

[U58] PHP：数组三件套
来源：http://uv.wgjwhj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://sb.huixiangedu.cn

[U59] PHP：自定义排序
来源：http://nm.nszjky.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://im.huixiangedu.cn

[U60] PHP：JSON 编解码
来源：http://wj.shtwfgs.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://iz.haigaiapp.cn

[U61] PHP：正则
来源：http://yr.asd995.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yk.colortex.cn

[U62] PHP：日期对象
来源：http://ty.shxzukj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dw.huixiangedu.cn

[U63] PHP：文件读写
来源：http://xq.muxihuayi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nv.jianghongdianzi.cn

[U64] PHP：目录遍历
来源：http://va.nszjky.cn

glob("dir/*.php");  scandir("dir");
来源：http://mo.wgjwhj.cn

[U65] PHP：会话
来源：http://vz.panjiajie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ua.asd995.cn

[U66] PHP：设置 Cookie
来源：http://as.panjiajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bk.jianghongdianzi.cn

[U67] PHP：处理文件上传
来源：http://tl.muxihuayi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://eh.huixiangedu.cn

[U68] PHP：PDO 连接
来源：http://iu.panjiajie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fc.wgjwhj.cn

[U69] PHP：PDO 预处理
来源：http://cr.huixiangedu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ej.hahajie.cn

[U70] PHP：PDO 事务
来源：http://rr.huanxung.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pq.hahajie.cn

[U71] PHP：抛出异常
来源：http://gd.lnxyls.cn

throw new RuntimeException("失败", 500);
来源：http://pt.hahajie.cn

[U72] PHP：写错误日志
来源：http://wh.yuntaijiaju.cn

error_log("失败: " . $e->getMessage());
来源：http://mo.bjjhwx.cn

[U73] PHP：读取 ini 配置
来源：http://to.colortex.cn

parse_ini_file("config.ini", true)
来源：http://am.lnxyls.cn

[U74] PHP：读取环境变量
来源：http://dt.521024.cn

getenv("APP_ENV") ?: "production"
来源：http://yz.panjiajie.cn

[U75] PHP：依赖注入
来源：http://xs.szxytkj.cn

composer require psr/container
来源：http://sx.wgjwhj.cn

[U76] PHP：简单路由
来源：http://uk.newstarts.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://os.szsharing.cn

[U77] PHP：模板渲染
来源：http://zw.colortex.cn

composer require twig/twig
来源：http://ns.jctech888.com.cn

[U78] PHP：单元测试
来源：http://hi.szsharing.cn

composer require --dev phpunit/phpunit
来源：http://la.521024.cn

[U79] PHP：静态分析
来源：http://cq.wgjwhj.cn

composer require --dev phpstan/phpstan
来源：http://xl.nszjky.cn

[U80] PHP：代码规范修复
来源：http://yg.panjiajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://gt.shxzskj.cn

[U81] JS：初始化项目
来源：http://ct.shxzukj.cn

npm init -y;  npm i express
来源：http://kz.asd995.cn

[U82] JS：package.json 脚本
来源：http://pw.huixiangedu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://il.hahajie.cn

[U83] JS：ES Module 导入导出
来源：http://ae.haigaiapp.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ws.521024.cn

[U84] JS：CommonJS 写法
来源：http://nx.shxzskj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ab.nicolike.cn

[U85] JS：可选链
来源：http://fk.haigaiapp.cn

a?.b?.c
来源：http://bk.gzmigu.cn

[U86] JS：空值合并
来源：http://gg.szsharing.cn

a ?? b
来源：http://oa.chemitech.net.cn

[U87] JS：解构默认值
来源：http://dd.newstarts.cn

const { a = 1, b = 2 } = obj;
来源：http://tl.hahajie.cn

[U88] JS：对象展开合并
来源：http://pu.yuexingan06.cn

{ ...a, ...b }
来源：http://oc.shxzskj.cn

[U89] JS：数组去重
来源：http://my.shxzukj.cn

[...new Set(arr)]
来源：http://qr.asd995.cn

[U90] JS：数字数组排序
来源：http://xi.asd995.cn

[...arr].sort((a, b) => a - b)
来源：http://bm.nszjky.cn

[U91] JS：对象键值遍历
来源：http://nq.lnxyls.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kl.shtwfgs.cn

[U92] JS：深拷贝
来源：http://gx.huixiangedu.cn

structuredClone(obj)
来源：http://om.huixinmuqiang.cn

[U93] JS：模板字符串
来源：http://tt.szxytkj.cn

`共 ${n} 条`
来源：http://je.hahajie.cn

[U94] JS：箭头函数
来源：http://ev.huanxung.cn

const double = x => x * 2;
来源：http://oo.nicolike.cn

[U95] JS：Promise 包装
来源：http://of.nszjky.cn

new Promise((resolve, reject) => {})
来源：http://zj.9csxet.cn

[U96] JS：async/await 与异常
来源：http://du.chemitech.net.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gj.asd995.cn

[U97] JS：并发请求
来源：http://gs.nicolike.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://jb.newstarts.cn

[U98] JS：fetch 带 JSON
来源：http://hs.lnxyls.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zc.gzmigu.cn

[U99] JS：事件监听
来源：http://jj.haigaiapp.cn

el.addEventListener("click", e => {})
来源：http://vc.shxzskj.cn

[U100] JS：DOM 查询
来源：http://zo.szsharing.cn

document.querySelector(".item")
来源：http://ad.huixinmuqiang.cn

[U101] JS：classList 操作
来源：http://jy.jianghongdianzi.cn

el.classList.toggle("active")
来源：http://hi.nicolike.cn

[U102] JS：本地存储
来源：http://cl.gzmigu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://tp.nszjky.cn

[U103] JS：定时器
来源：http://df.panjiajie.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ad.jianghongdianzi.cn

[U104] JS：防抖
来源：http://rv.nicolike.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://co.muxihuayi.cn

[U105] JS：节流
来源：http://pv.huixinmuqiang.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rm.9csxet.cn

[U106] JS：日期格式化
来源：http://pv.nszjky.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://et.yuexingan06.cn


<!-- 参考信息 -->