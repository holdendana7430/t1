代发 wailian999

[T17] Swift：变量与常量
来源：http://dn.chemitech.net.cn

var a = 1;  let b = 2
来源：http://bo.yuntaijiaju.cn

[T18] Swift：字符串插值
来源：http://yh.huanxung.cn

"值: \(b)"
来源：http://yg.nicolike.cn

[T19] Swift：可选绑定
来源：http://kx.shxzukj.cn

if let n = opt { print(n) }
来源：http://cq.521024.cn

[T20] Swift：数组操作
来源：http://ch.yuexingan06.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xf.jctech888.com.cn

[T21] Swift：遍历
来源：http://ne.jctech888.com.cn

for x in a { print(x) }
来源：http://ji.haigaiapp.cn

[T22] Swift：字典
来源：http://qy.asd995.cn

var d = ["a": 1];  d["b"] = 2
来源：http://jf.gzmigu.cn

[T23] Swift：函数
来源：http://li.huixiangedu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qo.huanxung.cn

[T24] Swift：闭包
来源：http://xm.shxzskj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://dt.asd995.cn

[T25] Swift：结构体
来源：http://cw.huixiangedu.cn

struct P { var x: Int }
来源：http://yg.shxzskj.cn

[T26] Swift：类与重写
来源：http://ro.yuntaijiaju.cn

class A: Base { override func f() {} }
来源：http://ci.hahajie.cn

[T27] Swift：错误处理
来源：http://pa.colortex.cn

do { try f() } catch { print(error) }
来源：http://xz.hahajie.cn

[T28] Swift：枚举
来源：http://eg.huixinmuqiang.cn

enum Color { case red, green }
来源：http://wy.szxytkj.cn

[T29] Swift：guard 提前返回
来源：http://qw.hnjuh.cn

guard let x = opt else { return }
来源：http://sz.haigaiapp.cn

[T30] Swift：协议
来源：http://gk.szsharing.cn

protocol Shape { func area() -> Double }
来源：http://kx.yuexingan06.cn

[T31] Lua：Hello World
来源：http://ym.szsharing.cn

print("Hello")
来源：http://ki.hahajie.cn

[T32] Lua：局部变量
来源：http://rr.wgjwhj.cn

local a = 1
来源：http://qr.huixinmuqiang.cn

[T33] Lua：表（数组）
来源：http://os.newstarts.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ee.gzmigu.cn

[T34] Lua：遍历表
来源：http://kn.huanxung.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ig.haigaiapp.cn

[T35] Lua：字典表
来源：http://hg.hahajie.cn

local d = { a = 1 };  d.b = 2
来源：http://yu.521024.cn

[T36] Lua：函数
来源：http://rk.shxzukj.cn

function add(a, b) return a + b end
来源：http://tp.huanxung.cn

[T37] Lua：字符串拼接
来源：http://rj.szsharing.cn

"a" .. "b"
来源：http://ow.huixiangedu.cn

[T38] Lua：条件
来源：http://lv.shtwfgs.cn

if x > 0 then print("正") end
来源：http://jc.bjjhwx.cn

[T39] Lua：模式匹配
来源：http://lq.muxihuayi.cn

string.find(s, "%d+")
来源：http://ko.shxzukj.cn

[T40] Lua：元表
来源：http://no.lnxyls.cn

setmetatable({}, { __index = base })
来源：http://vs.hahajie.cn

[T41] Perl：Hello World
来源：http://fv.jianghongdianzi.cn

print "Hello\n";
来源：http://ie.521024.cn

[T42] Perl：变量类型
来源：http://rl.shtwfgs.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cb.lnxyls.cn

[T43] Perl：字符串插值
来源：http://yj.bjjhwx.cn

"值: $a"
来源：http://pe.szsharing.cn

[T44] Perl：条件
来源：http://cx.wgjwhj.cn

if ($a > 0) { print "正"; }
来源：http://il.jianghongdianzi.cn

[T45] Perl：数组遍历
来源：http://es.colortex.cn

for my $x (@arr) { print $x; }
来源：http://zt.haigaiapp.cn

[T46] Perl：哈希操作
来源：http://uz.chemitech.net.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ij.jctech888.com.cn

[T47] Perl：正则捕获
来源：http://kl.szsharing.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://px.shtwfgs.cn

[T48] Perl：正则替换
来源：http://bf.haigaiapp.cn

$s =~ s/old/new/g;
来源：http://tm.shtwfgs.cn

[T49] Perl：函数
来源：http://id.hahajie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://uv.shtwfgs.cn

[T50] Perl：逐行读文件
来源：http://rh.bookmarksfly.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://nc.panjiajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://vv.shtwfgs.cn

[T51] Scala：Hello World
来源：http://xf.shxzskj.cn

println("Hello")
来源：http://ft.gzmigu.cn

[T52] Scala：变量
来源：http://nv.shxzukj.cn

val a = 1;  var b = 2
来源：http://if.hnjuh.cn

[T53] Scala：字符串插值
来源：http://au.szxytkj.cn

s"值: $b"
来源：http://dl.9csxet.cn

[T54] Scala：集合映射
来源：http://ap.hnjuh.cn

List(1, 2, 3).map(_ * 2)
来源：http://kc.lnxyls.cn

[T55] Scala：集合过滤
来源：http://cq.wgjwhj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://kw.wgjwhj.cn

[T56] Scala：样例类
来源：http://bu.bookmarksfly.cn

case class User(name: String, age: Int)
来源：http://tp.9csxet.cn

[T57] Scala：模式匹配
来源：http://et.yuntaijiaju.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://kw.szsharing.cn

[T58] Scala：函数定义
来源：http://uy.hnjuh.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gm.panjiajie.cn

[T59] Scala：循环
来源：http://mc.shtwfgs.cn

for (i <- 1 to 10) println(i)
来源：http://jv.szxytkj.cn

[T60] Scala：折叠
来源：http://nr.gzmigu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ts.nicolike.cn

================================================================================
来源：http://qs.colortex.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vn.hnjuh.cn

================================================================================
来源：http://at.9csxet.cn

[U01] Py：创建虚拟环境
来源：http://ny.muxihuayi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zz.wgjwhj.cn

[U02] Py：导出 / 安装依赖
来源：http://ul.panjiajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mm.yuexingan06.cn

[U03] Py：加载 .env 配置
来源：http://ya.shxzskj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://im.nszjky.cn

[U04] Py：变量调试打印
来源：http://ah.muxihuayi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kz.haigaiapp.cn

[U05] Py：列表去重且保序
来源：http://cl.jianghongdianzi.cn

list(dict.fromkeys(arr))
来源：http://su.panjiajie.cn

[U06] Py：合并两个字典
来源：http://mi.yuexingan06.cn

{**a, **b}
来源：http://us.521024.cn

[U07] Py：反转字典键值
来源：http://dc.nicolike.cn

{v: k for k, v in d.items()}
来源：http://da.hnjuh.cn

[U08] Py：展平二维列表
来源：http://dm.colortex.cn

[y for x in nested for y in x]
来源：http://pa.gzmigu.cn

[U09] Py：字典取最大值的键
来源：http://qe.panjiajie.cn

max(d, key=d.get)
来源：http://ua.muxihuayi.cn

[U10] Py：按值排序字典
来源：http://yi.huixinmuqiang.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hl.jianghongdianzi.cn

[U11] Py：生成器表达式
来源：http://cg.hahajie.cn

(x * 2 for x in arr)
来源：http://dn.shxzskj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://uz.9csxet.cn

Counter(arr).most_common(3)
来源：http://ua.haigaiapp.cn

[U13] Py：固定长度队列
来源：http://er.jianghongdianzi.cn

deque(maxlen=10)
来源：http://lq.chemitech.net.cn

[U14] Py：分组收集到列表
来源：http://yw.hahajie.cn

defaultdict(list)
来源：http://qv.hnjuh.cn

[U15] Py：高精度计时
来源：http://ta.chemitech.net.cn

t = time.perf_counter()
来源：http://fv.9csxet.cn

[U16] Py：命令行参数解析
来源：http://bm.haigaiapp.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yj.chemitech.net.cn

[U17] Py：初始化日志
来源：http://rv.shxzukj.cn

logging.basicConfig(level=logging.INFO)
来源：http://uw.hnjuh.cn

[U18] Py：预编译正则
来源：http://fa.521024.cn

pat = re.compile(r"\d+")
来源：http://id.chemitech.net.cn

[U19] Py：正则替换带回调
来源：http://el.huixiangedu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ht.haigaiapp.cn

[U20] Py：缓存函数结果
来源：http://ki.szxytkj.cn

@functools.lru_cache(maxsize=None)
来源：http://gt.panjiajie.cn

[U21] Py：自定义上下文管理器
来源：http://cu.huixiangedu.cn

@contextlib.contextmanager
来源：http://ku.yuntaijiaju.cn

[U22] Py：矩阵转置
来源：http://xn.hahajie.cn

list(zip(*m))
来源：http://po.newstarts.cn

[U23] Py：分块读取大文件
来源：http://sc.hnjuh.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gr.yuntaijiaju.cn

[U24] Py：路径操作
来源：http://nn.haigaiapp.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://in.shxzskj.cn

[U25] Py：CSV 按字典读
来源：http://vc.chemitech.net.cn

csv.DictReader(f)
来源：http://cw.hahajie.cn

[U26] Py：并发下载
来源：http://rn.muxihuayi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hi.shxzskj.cn

[U27] Py：异步 HTTP
来源：http://ki.shxzukj.cn

aiohttp.ClientSession() 配合 async with
来源：http://lf.panjiajie.cn

[U28] Py：类型别名
来源：http://nm.huixinmuqiang.cn

UserId = int
来源：http://ln.shxzskj.cn

[U29] Py：属性校验
来源：http://qd.bookmarksfly.cn

@property 与 @x.setter 配合
来源：http://ji.shxzukj.cn

[U30] Py：数据类
来源：http://du.hnjuh.cn

@dataclass(slots=True)
来源：http://aa.nszjky.cn

[U31] Py：单测
来源：http://xj.panjiajie.cn

python -m pytest -q
来源：http://mc.muxihuayi.cn

[U32] Py：代码格式化
来源：http://zf.521024.cn

ruff format . && ruff check --fix .
来源：http://wb.wgjwhj.cn

[U33] Py：打包发布
来源：http://ej.huixinmuqiang.cn

python -m build  （依赖 pyproject.toml）
来源：http://wk.bookmarksfly.cn

[U34] Py：判断编码
来源：http://kl.szsharing.cn

chardet.detect(raw)
来源：http://rx.colortex.cn

[U35] Py：发送邮件
来源：http://fx.haigaiapp.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fi.hnjuh.cn

[U36] Py：定时任务
来源：http://sx.lnxyls.cn

schedule.every(10).minutes.do(job)
来源：http://yd.panjiajie.cn

[U37] Py：读写 Excel
来源：http://qj.nicolike.cn

pandas.read_excel / DataFrame.to_excel
来源：http://dd.jianghongdianzi.cn

[U38] Py：获取脚本所在目录
来源：http://ef.yuexingan06.cn

Path(__file__).resolve().parent
来源：http://by.hnjuh.cn

[U39] Py：判断是否在交互环境
来源：http://gu.lnxyls.cn

sys.stdout.isatty()
来源：http://vi.yuntaijiaju.cn

[U40] Py：打印到标准错误
来源：http://sb.gzmigu.cn

print("err", file=sys.stderr)
来源：http://dk.huixiangedu.cn

[U41] PHP：初始化 Composer 项目
来源：http://uo.yuntaijiaju.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://pe.9csxet.cn

[U42] PHP：PSR-4 自动加载
来源：http://tw.yuntaijiaju.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fw.bookmarksfly.cn

[U43] PHP：声明命名空间
来源：http://ft.huixiangedu.cn

namespace App\Http;
来源：http://mx.chemitech.net.cn

[U44] PHP：开启严格类型
来源：http://ym.muxihuayi.cn

declare(strict_types=1);
来源：http://fp.asd995.cn

[U45] PHP：类型声明与返回类型
来源：http://cn.huixiangedu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://rm.hahajie.cn

[U46] PHP：可空类型
来源：http://by.yuexingan06.cn

?string $name = null
来源：http://uh.521024.cn

[U47] PHP：联合类型
来源：http://vy.jctech888.com.cn

int|string $id
来源：http://az.asd995.cn

[U48] PHP：纯枚举
来源：http://sx.szxytkj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ri.wgjwhj.cn

[U49] PHP：只读属性
来源：http://lq.yuexingan06.cn

public readonly string $name
来源：http://ln.panjiajie.cn

[U50] PHP：构造器属性提升
来源：http://su.shxzukj.cn

public function __construct(private int $id) {}
来源：http://qc.521024.cn

[U51] PHP：数组解构
来源：http://bk.lnxyls.cn

[$a, $b] = $arr;
来源：http://kc.9csxet.cn

[U52] PHP：箭头函数
来源：http://ad.yuexingan06.cn

$double = fn($x) => $x * 2;
来源：http://bz.huixinmuqiang.cn

[U53] PHP：空合并运算符
来源：http://xq.lnxyls.cn

$v = $a ?? $b ?? "default";
来源：http://br.huixinmuqiang.cn

[U54] PHP：空安全调用
来源：http://sb.huixiangedu.cn

$obj?->method()
来源：http://yz.newstarts.cn

[U55] PHP：match 表达式
来源：http://et.lnxyls.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zt.haigaiapp.cn

[U56] PHP：命名参数
来源：http://pi.521024.cn

f(a: 1, b: 2)
来源：http://tp.hnjuh.cn

[U57] PHP：字符串插值
来源：http://np.huanxung.cn

"值: {$a}"
来源：http://wj.newstarts.cn

[U58] PHP：数组三件套
来源：http://lf.panjiajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://eg.gzmigu.cn

[U59] PHP：自定义排序
来源：http://go.nicolike.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ac.muxihuayi.cn

[U60] PHP：JSON 编解码
来源：http://dj.szxytkj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://in.nicolike.cn

[U61] PHP：正则
来源：http://et.hnjuh.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://up.muxihuayi.cn

[U62] PHP：日期对象
来源：http://dm.shtwfgs.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qx.colortex.cn

[U63] PHP：文件读写
来源：http://rr.jianghongdianzi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bv.nszjky.cn

[U64] PHP：目录遍历
来源：http://gz.panjiajie.cn

glob("dir/*.php");  scandir("dir");
来源：http://ts.shxzukj.cn

[U65] PHP：会话
来源：http://se.yuntaijiaju.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://jg.lnxyls.cn

[U66] PHP：设置 Cookie
来源：http://pk.bookmarksfly.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://na.lnxyls.cn

[U67] PHP：处理文件上传
来源：http://hs.haigaiapp.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sr.szxytkj.cn

[U68] PHP：PDO 连接
来源：http://gt.bookmarksfly.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vp.huixiangedu.cn

[U69] PHP：PDO 预处理
来源：http://of.gzmigu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://np.shxzukj.cn

[U70] PHP：PDO 事务
来源：http://kl.chemitech.net.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://aa.yuexingan06.cn

[U71] PHP：抛出异常
来源：http://nj.huixiangedu.cn

throw new RuntimeException("失败", 500);
来源：http://is.panjiajie.cn

[U72] PHP：写错误日志
来源：http://no.huixiangedu.cn

error_log("失败: " . $e->getMessage());
来源：http://yo.shtwfgs.cn

[U73] PHP：读取 ini 配置
来源：http://sc.9csxet.cn

parse_ini_file("config.ini", true)
来源：http://ua.gzmigu.cn

[U74] PHP：读取环境变量
来源：http://bb.newstarts.cn

getenv("APP_ENV") ?: "production"
来源：http://qw.9csxet.cn

[U75] PHP：依赖注入
来源：http://iw.szsharing.cn

composer require psr/container
来源：http://wr.huixiangedu.cn

[U76] PHP：简单路由
来源：http://rp.521024.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dd.gzmigu.cn

[U77] PHP：模板渲染
来源：http://om.huanxung.cn

composer require twig/twig
来源：http://li.shxzukj.cn

[U78] PHP：单元测试
来源：http://wd.wgjwhj.cn

composer require --dev phpunit/phpunit
来源：http://xn.nicolike.cn

[U79] PHP：静态分析
来源：http://qu.hahajie.cn

composer require --dev phpstan/phpstan
来源：http://bd.nicolike.cn

[U80] PHP：代码规范修复
来源：http://rd.szxytkj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qz.9csxet.cn

[U81] JS：初始化项目
来源：http://yp.521024.cn

npm init -y;  npm i express
来源：http://qn.bookmarksfly.cn

[U82] JS：package.json 脚本
来源：http://yp.bjjhwx.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pf.yuexingan06.cn

[U83] JS：ES Module 导入导出
来源：http://yy.wgjwhj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ck.newstarts.cn

[U84] JS：CommonJS 写法
来源：http://cc.chemitech.net.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ue.colortex.cn

[U85] JS：可选链
来源：http://ey.jianghongdianzi.cn

a?.b?.c
来源：http://nj.lnxyls.cn

[U86] JS：空值合并
来源：http://je.yuntaijiaju.cn

a ?? b
来源：http://ff.bookmarksfly.cn

[U87] JS：解构默认值
来源：http://bc.szsharing.cn

const { a = 1, b = 2 } = obj;
来源：http://cy.nicolike.cn

[U88] JS：对象展开合并
来源：http://fd.yuntaijiaju.cn

{ ...a, ...b }
来源：http://so.lnxyls.cn

[U89] JS：数组去重
来源：http://eq.yuntaijiaju.cn

[...new Set(arr)]
来源：http://dw.521024.cn

[U90] JS：数字数组排序
来源：http://xm.nicolike.cn

[...arr].sort((a, b) => a - b)
来源：http://om.muxihuayi.cn

[U91] JS：对象键值遍历
来源：http://hr.newstarts.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ap.nicolike.cn

[U92] JS：深拷贝
来源：http://sh.wgjwhj.cn

structuredClone(obj)
来源：http://ku.asd995.cn

[U93] JS：模板字符串
来源：http://yl.newstarts.cn

`共 ${n} 条`
来源：http://mu.hahajie.cn

[U94] JS：箭头函数
来源：http://gp.colortex.cn

const double = x => x * 2;
来源：http://xc.huixinmuqiang.cn

[U95] JS：Promise 包装
来源：http://ac.gzmigu.cn

new Promise((resolve, reject) => {})
来源：http://jy.huixiangedu.cn

[U96] JS：async/await 与异常
来源：http://mk.szsharing.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jv.huixinmuqiang.cn

[U97] JS：并发请求
来源：http://ms.szsharing.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://gc.521024.cn

[U98] JS：fetch 带 JSON
来源：http://gd.chemitech.net.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://id.hnjuh.cn

[U99] JS：事件监听
来源：http://ih.wgjwhj.cn

el.addEventListener("click", e => {})
来源：http://pb.colortex.cn

[U100] JS：DOM 查询
来源：http://uv.hahajie.cn

document.querySelector(".item")
来源：http://la.9csxet.cn

[U101] JS：classList 操作
来源：http://dx.wgjwhj.cn

el.classList.toggle("active")
来源：http://ft.bjjhwx.cn

[U102] JS：本地存储
来源：http://ac.wgjwhj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://aw.huixiangedu.cn

[U103] JS：定时器
来源：http://de.panjiajie.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://op.nszjky.cn

[U104] JS：防抖
来源：http://hi.nszjky.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ti.bookmarksfly.cn


<!-- 参考信息 -->