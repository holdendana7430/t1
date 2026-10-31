代发 wailian999

[T17] Swift：变量与常量
来源：http://wu.shxzukj.cn

var a = 1;  let b = 2
来源：http://uf.haigaiapp.cn

[T18] Swift：字符串插值
来源：http://im.shxzskj.cn

"值: \(b)"
来源：http://ay.haigaiapp.cn

[T19] Swift：可选绑定
来源：http://bg.asd995.cn

if let n = opt { print(n) }
来源：http://nh.hnjuh.cn

[T20] Swift：数组操作
来源：http://qj.jctech888.com.cn

var a = [1, 2, 3];  a.append(4)
来源：http://wf.nszjky.cn

[T21] Swift：遍历
来源：http://uv.chemitech.net.cn

for x in a { print(x) }
来源：http://ko.bjjhwx.cn

[T22] Swift：字典
来源：http://ws.nicolike.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vo.haigaiapp.cn

[T23] Swift：函数
来源：http://ww.bookmarksfly.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qv.nicolike.cn

[T24] Swift：闭包
来源：http://tl.wgjwhj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ih.bjjhwx.cn

[T25] Swift：结构体
来源：http://dx.9csxet.cn

struct P { var x: Int }
来源：http://im.bjjhwx.cn

[T26] Swift：类与重写
来源：http://ki.yuexingan06.cn

class A: Base { override func f() {} }
来源：http://ox.bookmarksfly.cn

[T27] Swift：错误处理
来源：http://ds.jctech888.com.cn

do { try f() } catch { print(error) }
来源：http://zx.wgjwhj.cn

[T28] Swift：枚举
来源：http://ja.gzmigu.cn

enum Color { case red, green }
来源：http://ta.9csxet.cn

[T29] Swift：guard 提前返回
来源：http://uo.wgjwhj.cn

guard let x = opt else { return }
来源：http://bb.9csxet.cn

[T30] Swift：协议
来源：http://bx.gzmigu.cn

protocol Shape { func area() -> Double }
来源：http://ta.nicolike.cn

[T31] Lua：Hello World
来源：http://zi.muxihuayi.cn

print("Hello")
来源：http://hq.jianghongdianzi.cn

[T32] Lua：局部变量
来源：http://eq.huixiangedu.cn

local a = 1
来源：http://dv.yuntaijiaju.cn

[T33] Lua：表（数组）
来源：http://ib.chemitech.net.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://te.bookmarksfly.cn

[T34] Lua：遍历表
来源：http://md.hahajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ox.hahajie.cn

[T35] Lua：字典表
来源：http://wd.jctech888.com.cn

local d = { a = 1 };  d.b = 2
来源：http://jn.asd995.cn

[T36] Lua：函数
来源：http://qs.szxytkj.cn

function add(a, b) return a + b end
来源：http://fu.newstarts.cn

[T37] Lua：字符串拼接
来源：http://lk.colortex.cn

"a" .. "b"
来源：http://na.521024.cn

[T38] Lua：条件
来源：http://gz.hnjuh.cn

if x > 0 then print("正") end
来源：http://ho.muxihuayi.cn

[T39] Lua：模式匹配
来源：http://rv.lnxyls.cn

string.find(s, "%d+")
来源：http://he.nszjky.cn

[T40] Lua：元表
来源：http://mi.521024.cn

setmetatable({}, { __index = base })
来源：http://ae.jctech888.com.cn

[T41] Perl：Hello World
来源：http://ec.muxihuayi.cn

print "Hello\n";
来源：http://yv.lnxyls.cn

[T42] Perl：变量类型
来源：http://aw.wgjwhj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cm.shtwfgs.cn

[T43] Perl：字符串插值
来源：http://hg.jianghongdianzi.cn

"值: $a"
来源：http://cw.9csxet.cn

[T44] Perl：条件
来源：http://li.huixiangedu.cn

if ($a > 0) { print "正"; }
来源：http://uq.jianghongdianzi.cn

[T45] Perl：数组遍历
来源：http://uq.huanxung.cn

for my $x (@arr) { print $x; }
来源：http://ue.szsharing.cn

[T46] Perl：哈希操作
来源：http://xz.huanxung.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uo.huixinmuqiang.cn

[T47] Perl：正则捕获
来源：http://oh.nicolike.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://is.szxytkj.cn

[T48] Perl：正则替换
来源：http://qd.muxihuayi.cn

$s =~ s/old/new/g;
来源：http://hy.yuntaijiaju.cn

[T49] Perl：函数
来源：http://nd.newstarts.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://el.huanxung.cn

[T50] Perl：逐行读文件
来源：http://ki.lnxyls.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://vz.shxzukj.cn

while (my $line = <$fh>) { print $line; }
来源：http://mo.bookmarksfly.cn

[T51] Scala：Hello World
来源：http://hb.panjiajie.cn

println("Hello")
来源：http://yn.shtwfgs.cn

[T52] Scala：变量
来源：http://cs.huanxung.cn

val a = 1;  var b = 2
来源：http://mq.haigaiapp.cn

[T53] Scala：字符串插值
来源：http://ja.yuntaijiaju.cn

s"值: $b"
来源：http://ff.wgjwhj.cn

[T54] Scala：集合映射
来源：http://sp.jctech888.com.cn

List(1, 2, 3).map(_ * 2)
来源：http://kh.huixinmuqiang.cn

[T55] Scala：集合过滤
来源：http://hr.muxihuayi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xa.bjjhwx.cn

[T56] Scala：样例类
来源：http://wt.9csxet.cn

case class User(name: String, age: Int)
来源：http://ck.yuntaijiaju.cn

[T57] Scala：模式匹配
来源：http://pl.shtwfgs.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ed.panjiajie.cn

[T58] Scala：函数定义
来源：http://ph.szsharing.cn

def add(a: Int, b: Int): Int = a + b
来源：http://pb.9csxet.cn

[T59] Scala：循环
来源：http://je.jianghongdianzi.cn

for (i <- 1 to 10) println(i)
来源：http://qe.hnjuh.cn

[T60] Scala：折叠
来源：http://tj.huanxung.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sr.yuexingan06.cn

================================================================================
来源：http://lh.bookmarksfly.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tq.bjjhwx.cn

================================================================================
来源：http://pr.bjjhwx.cn

[U01] Py：创建虚拟环境
来源：http://ny.shxzskj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vr.szsharing.cn

[U02] Py：导出 / 安装依赖
来源：http://ro.panjiajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://th.huixiangedu.cn

[U03] Py：加载 .env 配置
来源：http://at.huanxung.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ql.hahajie.cn

[U04] Py：变量调试打印
来源：http://ae.bjjhwx.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rm.yuntaijiaju.cn

[U05] Py：列表去重且保序
来源：http://qp.yuexingan06.cn

list(dict.fromkeys(arr))
来源：http://cd.9csxet.cn

[U06] Py：合并两个字典
来源：http://pn.yuexingan06.cn

{**a, **b}
来源：http://xb.colortex.cn

[U07] Py：反转字典键值
来源：http://oj.nicolike.cn

{v: k for k, v in d.items()}
来源：http://fy.asd995.cn

[U08] Py：展平二维列表
来源：http://lo.bjjhwx.cn

[y for x in nested for y in x]
来源：http://uc.muxihuayi.cn

[U09] Py：字典取最大值的键
来源：http://yo.panjiajie.cn

max(d, key=d.get)
来源：http://mg.hahajie.cn

[U10] Py：按值排序字典
来源：http://nu.haigaiapp.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ie.panjiajie.cn

[U11] Py：生成器表达式
来源：http://qg.huixinmuqiang.cn

(x * 2 for x in arr)
来源：http://me.521024.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mo.yuntaijiaju.cn

Counter(arr).most_common(3)
来源：http://lw.szxytkj.cn

[U13] Py：固定长度队列
来源：http://mn.newstarts.cn

deque(maxlen=10)
来源：http://ab.521024.cn

[U14] Py：分组收集到列表
来源：http://bk.521024.cn

defaultdict(list)
来源：http://gr.shtwfgs.cn

[U15] Py：高精度计时
来源：http://cm.nicolike.cn

t = time.perf_counter()
来源：http://lz.gzmigu.cn

[U16] Py：命令行参数解析
来源：http://zh.shxzukj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://uo.jianghongdianzi.cn

[U17] Py：初始化日志
来源：http://tl.shxzukj.cn

logging.basicConfig(level=logging.INFO)
来源：http://mj.nicolike.cn

[U18] Py：预编译正则
来源：http://os.521024.cn

pat = re.compile(r"\d+")
来源：http://eh.yuntaijiaju.cn

[U19] Py：正则替换带回调
来源：http://sy.gzmigu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hu.newstarts.cn

[U20] Py：缓存函数结果
来源：http://ke.jctech888.com.cn

@functools.lru_cache(maxsize=None)
来源：http://yn.szxytkj.cn

[U21] Py：自定义上下文管理器
来源：http://uw.muxihuayi.cn

@contextlib.contextmanager
来源：http://ma.gzmigu.cn

[U22] Py：矩阵转置
来源：http://xo.chemitech.net.cn

list(zip(*m))
来源：http://qo.gzmigu.cn

[U23] Py：分块读取大文件
来源：http://ax.gzmigu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xb.muxihuayi.cn

[U24] Py：路径操作
来源：http://gf.bookmarksfly.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mw.huixinmuqiang.cn

[U25] Py：CSV 按字典读
来源：http://xj.jctech888.com.cn

csv.DictReader(f)
来源：http://ld.jctech888.com.cn

[U26] Py：并发下载
来源：http://aq.jctech888.com.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hp.colortex.cn

[U27] Py：异步 HTTP
来源：http://rh.gzmigu.cn

aiohttp.ClientSession() 配合 async with
来源：http://ft.panjiajie.cn

[U28] Py：类型别名
来源：http://qa.nszjky.cn

UserId = int
来源：http://fo.jctech888.com.cn

[U29] Py：属性校验
来源：http://ji.hnjuh.cn

@property 与 @x.setter 配合
来源：http://ia.bookmarksfly.cn

[U30] Py：数据类
来源：http://jy.shtwfgs.cn

@dataclass(slots=True)
来源：http://rk.shxzskj.cn

[U31] Py：单测
来源：http://al.lnxyls.cn

python -m pytest -q
来源：http://xt.asd995.cn

[U32] Py：代码格式化
来源：http://zc.haigaiapp.cn

ruff format . && ruff check --fix .
来源：http://uq.newstarts.cn

[U33] Py：打包发布
来源：http://hk.9csxet.cn

python -m build  （依赖 pyproject.toml）
来源：http://vj.huixinmuqiang.cn

[U34] Py：判断编码
来源：http://oe.521024.cn

chardet.detect(raw)
来源：http://jj.huanxung.cn

[U35] Py：发送邮件
来源：http://fz.nszjky.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ya.jctech888.com.cn

[U36] Py：定时任务
来源：http://ua.muxihuayi.cn

schedule.every(10).minutes.do(job)
来源：http://yz.huanxung.cn

[U37] Py：读写 Excel
来源：http://bf.nicolike.cn

pandas.read_excel / DataFrame.to_excel
来源：http://nw.gzmigu.cn

[U38] Py：获取脚本所在目录
来源：http://rl.shxzukj.cn

Path(__file__).resolve().parent
来源：http://pw.panjiajie.cn

[U39] Py：判断是否在交互环境
来源：http://fk.bjjhwx.cn

sys.stdout.isatty()
来源：http://re.nszjky.cn

[U40] Py：打印到标准错误
来源：http://si.panjiajie.cn

print("err", file=sys.stderr)
来源：http://bo.nszjky.cn

[U41] PHP：初始化 Composer 项目
来源：http://rk.hahajie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xc.colortex.cn

[U42] PHP：PSR-4 自动加载
来源：http://cm.nicolike.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nq.panjiajie.cn

[U43] PHP：声明命名空间
来源：http://mn.lnxyls.cn

namespace App\Http;
来源：http://nu.shtwfgs.cn

[U44] PHP：开启严格类型
来源：http://oc.gzmigu.cn

declare(strict_types=1);
来源：http://as.521024.cn

[U45] PHP：类型声明与返回类型
来源：http://su.jctech888.com.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://iy.gzmigu.cn

[U46] PHP：可空类型
来源：http://ez.newstarts.cn

?string $name = null
来源：http://no.521024.cn

[U47] PHP：联合类型
来源：http://gs.hnjuh.cn

int|string $id
来源：http://eo.wgjwhj.cn

[U48] PHP：纯枚举
来源：http://ek.lnxyls.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ao.jianghongdianzi.cn

[U49] PHP：只读属性
来源：http://nw.panjiajie.cn

public readonly string $name
来源：http://jx.asd995.cn

[U50] PHP：构造器属性提升
来源：http://uv.9csxet.cn

public function __construct(private int $id) {}
来源：http://wk.panjiajie.cn

[U51] PHP：数组解构
来源：http://qt.newstarts.cn

[$a, $b] = $arr;
来源：http://lt.newstarts.cn

[U52] PHP：箭头函数
来源：http://cy.yuexingan06.cn

$double = fn($x) => $x * 2;
来源：http://mv.yuntaijiaju.cn

[U53] PHP：空合并运算符
来源：http://iv.shtwfgs.cn

$v = $a ?? $b ?? "default";
来源：http://vk.shxzukj.cn

[U54] PHP：空安全调用
来源：http://jb.newstarts.cn

$obj?->method()
来源：http://tb.jianghongdianzi.cn

[U55] PHP：match 表达式
来源：http://bd.wgjwhj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tp.chemitech.net.cn

[U56] PHP：命名参数
来源：http://zn.shxzskj.cn

f(a: 1, b: 2)
来源：http://xs.huanxung.cn

[U57] PHP：字符串插值
来源：http://aa.huixinmuqiang.cn

"值: {$a}"
来源：http://dz.yuexingan06.cn

[U58] PHP：数组三件套
来源：http://km.szsharing.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nu.jianghongdianzi.cn

[U59] PHP：自定义排序
来源：http://qp.jianghongdianzi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rc.521024.cn

[U60] PHP：JSON 编解码
来源：http://we.szsharing.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://sj.huixinmuqiang.cn

[U61] PHP：正则
来源：http://uc.shtwfgs.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yq.bookmarksfly.cn

[U62] PHP：日期对象
来源：http://oe.huanxung.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kr.nszjky.cn

[U63] PHP：文件读写
来源：http://by.nszjky.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rx.hnjuh.cn

[U64] PHP：目录遍历
来源：http://bc.huixinmuqiang.cn

glob("dir/*.php");  scandir("dir");
来源：http://wn.chemitech.net.cn

[U65] PHP：会话
来源：http://rc.szxytkj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://jv.521024.cn

[U66] PHP：设置 Cookie
来源：http://if.szxytkj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ew.huixiangedu.cn

[U67] PHP：处理文件上传
来源：http://fd.nszjky.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ia.huanxung.cn

[U68] PHP：PDO 连接
来源：http://vc.hnjuh.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tj.nszjky.cn

[U69] PHP：PDO 预处理
来源：http://cm.szxytkj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dq.521024.cn

[U70] PHP：PDO 事务
来源：http://ln.hnjuh.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://it.hahajie.cn

[U71] PHP：抛出异常
来源：http://wb.szsharing.cn

throw new RuntimeException("失败", 500);
来源：http://tv.bookmarksfly.cn

[U72] PHP：写错误日志
来源：http://bw.gzmigu.cn

error_log("失败: " . $e->getMessage());
来源：http://xn.yuexingan06.cn

[U73] PHP：读取 ini 配置
来源：http://wy.shxzukj.cn

parse_ini_file("config.ini", true)
来源：http://bw.yuexingan06.cn

[U74] PHP：读取环境变量
来源：http://hk.gzmigu.cn

getenv("APP_ENV") ?: "production"
来源：http://rh.chemitech.net.cn

[U75] PHP：依赖注入
来源：http://kv.hahajie.cn

composer require psr/container
来源：http://ua.shtwfgs.cn

[U76] PHP：简单路由
来源：http://ji.shxzukj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lo.colortex.cn

[U77] PHP：模板渲染
来源：http://bu.wgjwhj.cn

composer require twig/twig
来源：http://px.wgjwhj.cn

[U78] PHP：单元测试
来源：http://ck.521024.cn

composer require --dev phpunit/phpunit
来源：http://kr.521024.cn

[U79] PHP：静态分析
来源：http://kq.wgjwhj.cn

composer require --dev phpstan/phpstan
来源：http://zc.shxzukj.cn

[U80] PHP：代码规范修复
来源：http://zh.hahajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://do.haigaiapp.cn

[U81] JS：初始化项目
来源：http://hv.colortex.cn

npm init -y;  npm i express
来源：http://ow.gzmigu.cn

[U82] JS：package.json 脚本
来源：http://zw.bookmarksfly.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lz.haigaiapp.cn

[U83] JS：ES Module 导入导出
来源：http://gm.lnxyls.cn

export const a = 1;  import { a } from "./m.js";
来源：http://rb.huanxung.cn

[U84] JS：CommonJS 写法
来源：http://hg.huixinmuqiang.cn

module.exports = { a };  const { a } = require("./m");
来源：http://gt.chemitech.net.cn

[U85] JS：可选链
来源：http://ws.hnjuh.cn

a?.b?.c
来源：http://hq.wgjwhj.cn

[U86] JS：空值合并
来源：http://vp.panjiajie.cn

a ?? b
来源：http://io.jctech888.com.cn

[U87] JS：解构默认值
来源：http://ss.gzmigu.cn

const { a = 1, b = 2 } = obj;
来源：http://le.9csxet.cn

[U88] JS：对象展开合并
来源：http://vk.huanxung.cn

{ ...a, ...b }
来源：http://jj.bjjhwx.cn

[U89] JS：数组去重
来源：http://dm.newstarts.cn

[...new Set(arr)]
来源：http://cs.shxzskj.cn

[U90] JS：数字数组排序
来源：http://mu.shtwfgs.cn

[...arr].sort((a, b) => a - b)
来源：http://kc.szxytkj.cn

[U91] JS：对象键值遍历
来源：http://yy.huixinmuqiang.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pc.yuexingan06.cn

[U92] JS：深拷贝
来源：http://ky.haigaiapp.cn

structuredClone(obj)
来源：http://hj.nszjky.cn

[U93] JS：模板字符串
来源：http://do.huanxung.cn

`共 ${n} 条`
来源：http://ug.yuntaijiaju.cn

[U94] JS：箭头函数
来源：http://wk.chemitech.net.cn

const double = x => x * 2;
来源：http://uj.yuntaijiaju.cn

[U95] JS：Promise 包装
来源：http://wm.muxihuayi.cn

new Promise((resolve, reject) => {})
来源：http://wm.huixiangedu.cn

[U96] JS：async/await 与异常
来源：http://mn.panjiajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vp.szxytkj.cn

[U97] JS：并发请求
来源：http://qp.yuntaijiaju.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://sm.szsharing.cn

[U98] JS：fetch 带 JSON
来源：http://rh.colortex.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ir.jctech888.com.cn

[U99] JS：事件监听
来源：http://wd.szsharing.cn

el.addEventListener("click", e => {})
来源：http://hd.bjjhwx.cn

[U100] JS：DOM 查询
来源：http://be.yuexingan06.cn

document.querySelector(".item")
来源：http://fx.shxzskj.cn

[U101] JS：classList 操作
来源：http://sn.huanxung.cn

el.classList.toggle("active")
来源：http://gi.bjjhwx.cn

[U102] JS：本地存储
来源：http://qj.nicolike.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ec.bookmarksfly.cn

[U103] JS：定时器
来源：http://hk.nszjky.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bh.shxzskj.cn

[U104] JS：防抖
来源：http://cl.gzmigu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jh.gzmigu.cn


<!-- 参考信息 -->