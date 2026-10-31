代发 wailian999

[T23] Swift：函数
来源：http://ri.shtwfgs.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pc.colortex.cn

[T24] Swift：闭包
来源：http://tt.nicolike.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://hc.hahajie.cn

[T25] Swift：结构体
来源：http://gx.9csxet.cn

struct P { var x: Int }
来源：http://in.shtwfgs.cn

[T26] Swift：类与重写
来源：http://ma.szxytkj.cn

class A: Base { override func f() {} }
来源：http://or.muxihuayi.cn

[T27] Swift：错误处理
来源：http://tx.hnjuh.cn

do { try f() } catch { print(error) }
来源：http://sf.muxihuayi.cn

[T28] Swift：枚举
来源：http://om.huanxung.cn

enum Color { case red, green }
来源：http://ul.shxzskj.cn

[T29] Swift：guard 提前返回
来源：http://iv.hahajie.cn

guard let x = opt else { return }
来源：http://tx.hahajie.cn

[T30] Swift：协议
来源：http://xo.huixiangedu.cn

protocol Shape { func area() -> Double }
来源：http://rz.shxzskj.cn

[T31] Lua：Hello World
来源：http://qy.jianghongdianzi.cn

print("Hello")
来源：http://qu.9csxet.cn

[T32] Lua：局部变量
来源：http://an.asd995.cn

local a = 1
来源：http://yr.colortex.cn

[T33] Lua：表（数组）
来源：http://vi.szsharing.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://cy.panjiajie.cn

[T34] Lua：遍历表
来源：http://dt.colortex.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://fe.lnxyls.cn

[T35] Lua：字典表
来源：http://yo.yuexingan06.cn

local d = { a = 1 };  d.b = 2
来源：http://jp.nicolike.cn

[T36] Lua：函数
来源：http://pl.huanxung.cn

function add(a, b) return a + b end
来源：http://uc.asd995.cn

[T37] Lua：字符串拼接
来源：http://mi.shxzskj.cn

"a" .. "b"
来源：http://pf.shxzskj.cn

[T38] Lua：条件
来源：http://iv.asd995.cn

if x > 0 then print("正") end
来源：http://vy.huanxung.cn

[T39] Lua：模式匹配
来源：http://dg.nszjky.cn

string.find(s, "%d+")
来源：http://fn.jctech888.com.cn

[T40] Lua：元表
来源：http://ak.yuntaijiaju.cn

setmetatable({}, { __index = base })
来源：http://us.jianghongdianzi.cn

[T41] Perl：Hello World
来源：http://db.shtwfgs.cn

print "Hello\n";
来源：http://yr.newstarts.cn

[T42] Perl：变量类型
来源：http://sm.shtwfgs.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fk.asd995.cn

[T43] Perl：字符串插值
来源：http://ys.muxihuayi.cn

"值: $a"
来源：http://hr.lnxyls.cn

[T44] Perl：条件
来源：http://nd.hahajie.cn

if ($a > 0) { print "正"; }
来源：http://ch.yuntaijiaju.cn

[T45] Perl：数组遍历
来源：http://pj.bookmarksfly.cn

for my $x (@arr) { print $x; }
来源：http://kb.asd995.cn

[T46] Perl：哈希操作
来源：http://vm.haigaiapp.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dd.shtwfgs.cn

[T47] Perl：正则捕获
来源：http://cm.huanxung.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rc.9csxet.cn

[T48] Perl：正则替换
来源：http://hn.asd995.cn

$s =~ s/old/new/g;
来源：http://cf.asd995.cn

[T49] Perl：函数
来源：http://lc.gzmigu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vm.nszjky.cn

[T50] Perl：逐行读文件
来源：http://sq.jianghongdianzi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://da.yuexingan06.cn

while (my $line = <$fh>) { print $line; }
来源：http://fj.muxihuayi.cn

[T51] Scala：Hello World
来源：http://lo.9csxet.cn

println("Hello")
来源：http://vt.jianghongdianzi.cn

[T52] Scala：变量
来源：http://av.9csxet.cn

val a = 1;  var b = 2
来源：http://yx.jianghongdianzi.cn

[T53] Scala：字符串插值
来源：http://pb.jctech888.com.cn

s"值: $b"
来源：http://lj.jianghongdianzi.cn

[T54] Scala：集合映射
来源：http://yq.wgjwhj.cn

List(1, 2, 3).map(_ * 2)
来源：http://gh.muxihuayi.cn

[T55] Scala：集合过滤
来源：http://rg.huanxung.cn

List(1, 2, 3).filter(_ > 1)
来源：http://me.newstarts.cn

[T56] Scala：样例类
来源：http://qq.shxzukj.cn

case class User(name: String, age: Int)
来源：http://pz.shxzukj.cn

[T57] Scala：模式匹配
来源：http://og.szsharing.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://il.asd995.cn

[T58] Scala：函数定义
来源：http://py.shtwfgs.cn

def add(a: Int, b: Int): Int = a + b
来源：http://lw.panjiajie.cn

[T59] Scala：循环
来源：http://kj.yuntaijiaju.cn

for (i <- 1 to 10) println(i)
来源：http://aj.shtwfgs.cn

[T60] Scala：折叠
来源：http://ej.yuexingan06.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sl.newstarts.cn

================================================================================
来源：http://zh.hahajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pb.shxzskj.cn

================================================================================
来源：http://fe.shxzskj.cn

[U01] Py：创建虚拟环境
来源：http://oz.newstarts.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ki.huixiangedu.cn

[U02] Py：导出 / 安装依赖
来源：http://nb.shxzskj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://eg.jctech888.com.cn

[U03] Py：加载 .env 配置
来源：http://yx.yuexingan06.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://mz.hnjuh.cn

[U04] Py：变量调试打印
来源：http://tu.panjiajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://au.newstarts.cn

[U05] Py：列表去重且保序
来源：http://jx.9csxet.cn

list(dict.fromkeys(arr))
来源：http://mf.chemitech.net.cn

[U06] Py：合并两个字典
来源：http://vf.shxzskj.cn

{**a, **b}
来源：http://ns.yuexingan06.cn

[U07] Py：反转字典键值
来源：http://tv.9csxet.cn

{v: k for k, v in d.items()}
来源：http://po.shxzskj.cn

[U08] Py：展平二维列表
来源：http://hj.newstarts.cn

[y for x in nested for y in x]
来源：http://wf.shxzskj.cn

[U09] Py：字典取最大值的键
来源：http://om.bookmarksfly.cn

max(d, key=d.get)
来源：http://rf.huanxung.cn

[U10] Py：按值排序字典
来源：http://zy.jctech888.com.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kr.bjjhwx.cn

[U11] Py：生成器表达式
来源：http://yy.huixinmuqiang.cn

(x * 2 for x in arr)
来源：http://rj.shtwfgs.cn

[U12] Py：取出现最多的 3 个元素
来源：http://pq.nszjky.cn

Counter(arr).most_common(3)
来源：http://ca.szsharing.cn

[U13] Py：固定长度队列
来源：http://ta.muxihuayi.cn

deque(maxlen=10)
来源：http://uj.huixinmuqiang.cn

[U14] Py：分组收集到列表
来源：http://il.asd995.cn

defaultdict(list)
来源：http://vn.jianghongdianzi.cn

[U15] Py：高精度计时
来源：http://zo.szxytkj.cn

t = time.perf_counter()
来源：http://oo.yuntaijiaju.cn

[U16] Py：命令行参数解析
来源：http://so.chemitech.net.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://no.wgjwhj.cn

[U17] Py：初始化日志
来源：http://zm.9csxet.cn

logging.basicConfig(level=logging.INFO)
来源：http://ft.shxzskj.cn

[U18] Py：预编译正则
来源：http://yp.bookmarksfly.cn

pat = re.compile(r"\d+")
来源：http://ia.newstarts.cn

[U19] Py：正则替换带回调
来源：http://wc.chemitech.net.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fi.nicolike.cn

[U20] Py：缓存函数结果
来源：http://sx.asd995.cn

@functools.lru_cache(maxsize=None)
来源：http://zk.jianghongdianzi.cn

[U21] Py：自定义上下文管理器
来源：http://jw.nicolike.cn

@contextlib.contextmanager
来源：http://lo.haigaiapp.cn

[U22] Py：矩阵转置
来源：http://eg.colortex.cn

list(zip(*m))
来源：http://je.shxzukj.cn

[U23] Py：分块读取大文件
来源：http://la.haigaiapp.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ex.haigaiapp.cn

[U24] Py：路径操作
来源：http://rw.shxzukj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ja.szsharing.cn

[U25] Py：CSV 按字典读
来源：http://dl.bookmarksfly.cn

csv.DictReader(f)
来源：http://wa.muxihuayi.cn

[U26] Py：并发下载
来源：http://ut.chemitech.net.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qi.shxzskj.cn

[U27] Py：异步 HTTP
来源：http://su.chemitech.net.cn

aiohttp.ClientSession() 配合 async with
来源：http://oo.colortex.cn

[U28] Py：类型别名
来源：http://id.shtwfgs.cn

UserId = int
来源：http://cu.bookmarksfly.cn

[U29] Py：属性校验
来源：http://vs.gzmigu.cn

@property 与 @x.setter 配合
来源：http://vc.gzmigu.cn

[U30] Py：数据类
来源：http://vi.muxihuayi.cn

@dataclass(slots=True)
来源：http://ga.huanxung.cn

[U31] Py：单测
来源：http://or.lnxyls.cn

python -m pytest -q
来源：http://pt.shtwfgs.cn

[U32] Py：代码格式化
来源：http://sc.hnjuh.cn

ruff format . && ruff check --fix .
来源：http://ns.asd995.cn

[U33] Py：打包发布
来源：http://fb.yuexingan06.cn

python -m build  （依赖 pyproject.toml）
来源：http://cz.colortex.cn

[U34] Py：判断编码
来源：http://vn.asd995.cn

chardet.detect(raw)
来源：http://zi.szxytkj.cn

[U35] Py：发送邮件
来源：http://qg.huixinmuqiang.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zj.nicolike.cn

[U36] Py：定时任务
来源：http://xn.jianghongdianzi.cn

schedule.every(10).minutes.do(job)
来源：http://vi.nszjky.cn

[U37] Py：读写 Excel
来源：http://co.bjjhwx.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ai.hnjuh.cn

[U38] Py：获取脚本所在目录
来源：http://rp.hahajie.cn

Path(__file__).resolve().parent
来源：http://gd.nszjky.cn

[U39] Py：判断是否在交互环境
来源：http://nz.hahajie.cn

sys.stdout.isatty()
来源：http://gn.9csxet.cn

[U40] Py：打印到标准错误
来源：http://yg.nszjky.cn

print("err", file=sys.stderr)
来源：http://cd.nicolike.cn

[U41] PHP：初始化 Composer 项目
来源：http://st.lnxyls.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://nz.jianghongdianzi.cn

[U42] PHP：PSR-4 自动加载
来源：http://ap.szxytkj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ak.shxzukj.cn

[U43] PHP：声明命名空间
来源：http://nf.yuexingan06.cn

namespace App\Http;
来源：http://lr.panjiajie.cn

[U44] PHP：开启严格类型
来源：http://kz.haigaiapp.cn

declare(strict_types=1);
来源：http://bi.jctech888.com.cn

[U45] PHP：类型声明与返回类型
来源：http://kc.panjiajie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://xf.newstarts.cn

[U46] PHP：可空类型
来源：http://uz.bookmarksfly.cn

?string $name = null
来源：http://jy.muxihuayi.cn

[U47] PHP：联合类型
来源：http://qo.bjjhwx.cn

int|string $id
来源：http://ym.gzmigu.cn

[U48] PHP：纯枚举
来源：http://gg.wgjwhj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ft.shxzukj.cn

[U49] PHP：只读属性
来源：http://xq.muxihuayi.cn

public readonly string $name
来源：http://gk.bjjhwx.cn

[U50] PHP：构造器属性提升
来源：http://js.bookmarksfly.cn

public function __construct(private int $id) {}
来源：http://wj.huanxung.cn

[U51] PHP：数组解构
来源：http://om.chemitech.net.cn

[$a, $b] = $arr;
来源：http://tu.nszjky.cn

[U52] PHP：箭头函数
来源：http://gg.jctech888.com.cn

$double = fn($x) => $x * 2;
来源：http://bl.yuexingan06.cn

[U53] PHP：空合并运算符
来源：http://nb.521024.cn

$v = $a ?? $b ?? "default";
来源：http://ci.bookmarksfly.cn

[U54] PHP：空安全调用
来源：http://hj.lnxyls.cn

$obj?->method()
来源：http://ql.9csxet.cn

[U55] PHP：match 表达式
来源：http://cl.haigaiapp.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ay.bookmarksfly.cn

[U56] PHP：命名参数
来源：http://cv.hnjuh.cn

f(a: 1, b: 2)
来源：http://am.huanxung.cn

[U57] PHP：字符串插值
来源：http://vq.szsharing.cn

"值: {$a}"
来源：http://iq.lnxyls.cn

[U58] PHP：数组三件套
来源：http://fl.shtwfgs.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yd.nicolike.cn

[U59] PHP：自定义排序
来源：http://oj.gzmigu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ey.huixiangedu.cn

[U60] PHP：JSON 编解码
来源：http://er.shxzukj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bv.yuexingan06.cn

[U61] PHP：正则
来源：http://hx.haigaiapp.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hd.shxzukj.cn

[U62] PHP：日期对象
来源：http://jw.chemitech.net.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gh.muxihuayi.cn

[U63] PHP：文件读写
来源：http://ei.huanxung.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pn.szxytkj.cn

[U64] PHP：目录遍历
来源：http://rt.haigaiapp.cn

glob("dir/*.php");  scandir("dir");
来源：http://ya.newstarts.cn

[U65] PHP：会话
来源：http://jg.wgjwhj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vs.shxzukj.cn

[U66] PHP：设置 Cookie
来源：http://ke.bookmarksfly.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ut.hahajie.cn

[U67] PHP：处理文件上传
来源：http://ov.nicolike.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://le.yuexingan06.cn

[U68] PHP：PDO 连接
来源：http://qh.jctech888.com.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cy.yuntaijiaju.cn

[U69] PHP：PDO 预处理
来源：http://ao.colortex.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pj.chemitech.net.cn

[U70] PHP：PDO 事务
来源：http://ze.nszjky.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tt.shtwfgs.cn

[U71] PHP：抛出异常
来源：http://yd.colortex.cn

throw new RuntimeException("失败", 500);
来源：http://px.szsharing.cn

[U72] PHP：写错误日志
来源：http://ph.muxihuayi.cn

error_log("失败: " . $e->getMessage());
来源：http://in.bjjhwx.cn

[U73] PHP：读取 ini 配置
来源：http://sc.9csxet.cn

parse_ini_file("config.ini", true)
来源：http://cj.hahajie.cn

[U74] PHP：读取环境变量
来源：http://lp.jctech888.com.cn

getenv("APP_ENV") ?: "production"
来源：http://jb.huixinmuqiang.cn

[U75] PHP：依赖注入
来源：http://yu.panjiajie.cn

composer require psr/container
来源：http://km.shtwfgs.cn

[U76] PHP：简单路由
来源：http://es.shxzukj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yv.shxzskj.cn

[U77] PHP：模板渲染
来源：http://zf.521024.cn

composer require twig/twig
来源：http://og.chemitech.net.cn

[U78] PHP：单元测试
来源：http://uk.jctech888.com.cn

composer require --dev phpunit/phpunit
来源：http://sk.yuexingan06.cn

[U79] PHP：静态分析
来源：http://ye.jianghongdianzi.cn

composer require --dev phpstan/phpstan
来源：http://zl.hahajie.cn

[U80] PHP：代码规范修复
来源：http://rt.hahajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://gp.wgjwhj.cn

[U81] JS：初始化项目
来源：http://kj.hahajie.cn

npm init -y;  npm i express
来源：http://pr.szxytkj.cn

[U82] JS：package.json 脚本
来源：http://gm.yuexingan06.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nj.nicolike.cn

[U83] JS：ES Module 导入导出
来源：http://zr.shxzukj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://mu.lnxyls.cn

[U84] JS：CommonJS 写法
来源：http://ze.colortex.cn

module.exports = { a };  const { a } = require("./m");
来源：http://cb.nicolike.cn

[U85] JS：可选链
来源：http://nj.9csxet.cn

a?.b?.c
来源：http://my.shxzukj.cn

[U86] JS：空值合并
来源：http://bb.huixiangedu.cn

a ?? b
来源：http://vp.asd995.cn

[U87] JS：解构默认值
来源：http://lr.yuexingan06.cn

const { a = 1, b = 2 } = obj;
来源：http://mu.yuexingan06.cn

[U88] JS：对象展开合并
来源：http://un.yuntaijiaju.cn

{ ...a, ...b }
来源：http://ir.shxzskj.cn

[U89] JS：数组去重
来源：http://lu.shtwfgs.cn

[...new Set(arr)]
来源：http://ab.huixinmuqiang.cn

[U90] JS：数字数组排序
来源：http://vn.gzmigu.cn

[...arr].sort((a, b) => a - b)
来源：http://op.hahajie.cn

[U91] JS：对象键值遍历
来源：http://fl.panjiajie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bq.lnxyls.cn

[U92] JS：深拷贝
来源：http://ew.lnxyls.cn

structuredClone(obj)
来源：http://kj.yuexingan06.cn

[U93] JS：模板字符串
来源：http://ld.huixinmuqiang.cn

`共 ${n} 条`
来源：http://sq.bjjhwx.cn

[U94] JS：箭头函数
来源：http://qm.huanxung.cn

const double = x => x * 2;
来源：http://tx.jianghongdianzi.cn

[U95] JS：Promise 包装
来源：http://pv.521024.cn

new Promise((resolve, reject) => {})
来源：http://pl.szsharing.cn

[U96] JS：async/await 与异常
来源：http://jk.yuexingan06.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://go.hnjuh.cn

[U97] JS：并发请求
来源：http://pj.jianghongdianzi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://gv.521024.cn

[U98] JS：fetch 带 JSON
来源：http://uq.szsharing.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pt.gzmigu.cn

[U99] JS：事件监听
来源：http://ng.yuntaijiaju.cn

el.addEventListener("click", e => {})
来源：http://hn.nicolike.cn

[U100] JS：DOM 查询
来源：http://cf.huixiangedu.cn

document.querySelector(".item")
来源：http://cc.shtwfgs.cn

[U101] JS：classList 操作
来源：http://cd.jianghongdianzi.cn

el.classList.toggle("active")
来源：http://ed.hnjuh.cn

[U102] JS：本地存储
来源：http://cb.jctech888.com.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ic.wgjwhj.cn

[U103] JS：定时器
来源：http://ut.huixiangedu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xv.jctech888.com.cn

[U104] JS：防抖
来源：http://di.lnxyls.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lv.haigaiapp.cn

[U105] JS：节流
来源：http://oh.huixinmuqiang.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gq.newstarts.cn

[U106] JS：日期格式化
来源：http://mc.shxzskj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dg.521024.cn

[U107] JS：数字千分位
来源：http://eb.yuexingan06.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ap.lnxyls.cn

[U108] JS：随机整数
来源：http://ra.huixiangedu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zl.nszjky.cn

[U109] JS：数组分组
来源：http://il.9csxet.cn

Object.groupBy(arr, x => x.type)
来源：http://ce.shtwfgs.cn

[U110] JS：数组分块
来源：http://qk.haigaiapp.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kq.panjiajie.cn


<!-- 参考信息 -->