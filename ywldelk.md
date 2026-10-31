代发 wailian999

[T19] Swift：可选绑定
来源：http://pe.shxzskj.cn

if let n = opt { print(n) }
来源：http://vb.bjjhwx.cn

[T20] Swift：数组操作
来源：http://vf.bookmarksfly.cn

var a = [1, 2, 3];  a.append(4)
来源：http://va.9csxet.cn

[T21] Swift：遍历
来源：http://ot.nicolike.cn

for x in a { print(x) }
来源：http://ib.huanxung.cn

[T22] Swift：字典
来源：http://zn.haigaiapp.cn

var d = ["a": 1];  d["b"] = 2
来源：http://bt.szsharing.cn

[T23] Swift：函数
来源：http://tm.muxihuayi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vk.bjjhwx.cn

[T24] Swift：闭包
来源：http://wx.nszjky.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://up.521024.cn

[T25] Swift：结构体
来源：http://uq.bjjhwx.cn

struct P { var x: Int }
来源：http://du.hahajie.cn

[T26] Swift：类与重写
来源：http://qj.chemitech.net.cn

class A: Base { override func f() {} }
来源：http://un.shxzukj.cn

[T27] Swift：错误处理
来源：http://bl.lnxyls.cn

do { try f() } catch { print(error) }
来源：http://nq.muxihuayi.cn

[T28] Swift：枚举
来源：http://bh.nicolike.cn

enum Color { case red, green }
来源：http://rh.nszjky.cn

[T29] Swift：guard 提前返回
来源：http://ps.muxihuayi.cn

guard let x = opt else { return }
来源：http://iz.newstarts.cn

[T30] Swift：协议
来源：http://hn.colortex.cn

protocol Shape { func area() -> Double }
来源：http://at.shxzskj.cn

[T31] Lua：Hello World
来源：http://lz.shxzskj.cn

print("Hello")
来源：http://sq.shxzukj.cn

[T32] Lua：局部变量
来源：http://vg.yuexingan06.cn

local a = 1
来源：http://fg.hahajie.cn

[T33] Lua：表（数组）
来源：http://kc.yuexingan06.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wp.asd995.cn

[T34] Lua：遍历表
来源：http://pm.9csxet.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://yp.chemitech.net.cn

[T35] Lua：字典表
来源：http://th.jctech888.com.cn

local d = { a = 1 };  d.b = 2
来源：http://rw.9csxet.cn

[T36] Lua：函数
来源：http://td.newstarts.cn

function add(a, b) return a + b end
来源：http://qx.shtwfgs.cn

[T37] Lua：字符串拼接
来源：http://tj.hahajie.cn

"a" .. "b"
来源：http://fq.nszjky.cn

[T38] Lua：条件
来源：http://pz.shxzskj.cn

if x > 0 then print("正") end
来源：http://wt.shxzukj.cn

[T39] Lua：模式匹配
来源：http://bz.huixiangedu.cn

string.find(s, "%d+")
来源：http://wp.szsharing.cn

[T40] Lua：元表
来源：http://jr.nszjky.cn

setmetatable({}, { __index = base })
来源：http://og.nicolike.cn

[T41] Perl：Hello World
来源：http://su.shtwfgs.cn

print "Hello\n";
来源：http://be.asd995.cn

[T42] Perl：变量类型
来源：http://ya.yuexingan06.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bs.nicolike.cn

[T43] Perl：字符串插值
来源：http://ly.hahajie.cn

"值: $a"
来源：http://oa.lnxyls.cn

[T44] Perl：条件
来源：http://dt.newstarts.cn

if ($a > 0) { print "正"; }
来源：http://wz.nicolike.cn

[T45] Perl：数组遍历
来源：http://kp.jctech888.com.cn

for my $x (@arr) { print $x; }
来源：http://us.yuexingan06.cn

[T46] Perl：哈希操作
来源：http://qo.jctech888.com.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hm.bookmarksfly.cn

[T47] Perl：正则捕获
来源：http://wq.huixinmuqiang.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jb.colortex.cn

[T48] Perl：正则替换
来源：http://zh.szxytkj.cn

$s =~ s/old/new/g;
来源：http://ph.yuntaijiaju.cn

[T49] Perl：函数
来源：http://tq.jctech888.com.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nq.jctech888.com.cn

[T50] Perl：逐行读文件
来源：http://md.shxzukj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://jy.yuexingan06.cn

while (my $line = <$fh>) { print $line; }
来源：http://os.shxzukj.cn

[T51] Scala：Hello World
来源：http://ml.521024.cn

println("Hello")
来源：http://we.hahajie.cn

[T52] Scala：变量
来源：http://kq.jianghongdianzi.cn

val a = 1;  var b = 2
来源：http://jw.huixinmuqiang.cn

[T53] Scala：字符串插值
来源：http://fn.chemitech.net.cn

s"值: $b"
来源：http://qo.newstarts.cn

[T54] Scala：集合映射
来源：http://eq.wgjwhj.cn

List(1, 2, 3).map(_ * 2)
来源：http://wm.hnjuh.cn

[T55] Scala：集合过滤
来源：http://lj.yuntaijiaju.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fc.szxytkj.cn

[T56] Scala：样例类
来源：http://et.bjjhwx.cn

case class User(name: String, age: Int)
来源：http://ca.shtwfgs.cn

[T57] Scala：模式匹配
来源：http://ow.gzmigu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gv.nszjky.cn

[T58] Scala：函数定义
来源：http://fi.9csxet.cn

def add(a: Int, b: Int): Int = a + b
来源：http://cy.yuntaijiaju.cn

[T59] Scala：循环
来源：http://zr.szsharing.cn

for (i <- 1 to 10) println(i)
来源：http://ti.bjjhwx.cn

[T60] Scala：折叠
来源：http://tz.haigaiapp.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vv.asd995.cn

================================================================================
来源：http://yl.wgjwhj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://uy.bookmarksfly.cn

================================================================================
来源：http://vv.szxytkj.cn

[U01] Py：创建虚拟环境
来源：http://sm.haigaiapp.cn

python -m venv .venv && source .venv/bin/activate
来源：http://lp.bookmarksfly.cn

[U02] Py：导出 / 安装依赖
来源：http://tt.521024.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://be.bookmarksfly.cn

[U03] Py：加载 .env 配置
来源：http://gi.bjjhwx.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://tq.shxzskj.cn

[U04] Py：变量调试打印
来源：http://er.shxzukj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nx.yuexingan06.cn

[U05] Py：列表去重且保序
来源：http://zf.jctech888.com.cn

list(dict.fromkeys(arr))
来源：http://jf.huanxung.cn

[U06] Py：合并两个字典
来源：http://uf.shxzskj.cn

{**a, **b}
来源：http://md.panjiajie.cn

[U07] Py：反转字典键值
来源：http://ub.lnxyls.cn

{v: k for k, v in d.items()}
来源：http://pw.chemitech.net.cn

[U08] Py：展平二维列表
来源：http://js.nicolike.cn

[y for x in nested for y in x]
来源：http://me.nszjky.cn

[U09] Py：字典取最大值的键
来源：http://oc.haigaiapp.cn

max(d, key=d.get)
来源：http://dv.szsharing.cn

[U10] Py：按值排序字典
来源：http://ce.newstarts.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qd.newstarts.cn

[U11] Py：生成器表达式
来源：http://mi.nicolike.cn

(x * 2 for x in arr)
来源：http://ca.muxihuayi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://cr.bjjhwx.cn

Counter(arr).most_common(3)
来源：http://sa.jianghongdianzi.cn

[U13] Py：固定长度队列
来源：http://mp.hahajie.cn

deque(maxlen=10)
来源：http://hj.yuexingan06.cn

[U14] Py：分组收集到列表
来源：http://vk.hahajie.cn

defaultdict(list)
来源：http://is.huixinmuqiang.cn

[U15] Py：高精度计时
来源：http://vv.shtwfgs.cn

t = time.perf_counter()
来源：http://cd.yuntaijiaju.cn

[U16] Py：命令行参数解析
来源：http://yg.huixiangedu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nv.521024.cn

[U17] Py：初始化日志
来源：http://st.shxzukj.cn

logging.basicConfig(level=logging.INFO)
来源：http://aj.shxzskj.cn

[U18] Py：预编译正则
来源：http://os.bookmarksfly.cn

pat = re.compile(r"\d+")
来源：http://sv.haigaiapp.cn

[U19] Py：正则替换带回调
来源：http://fz.haigaiapp.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xa.jctech888.com.cn

[U20] Py：缓存函数结果
来源：http://cj.shxzskj.cn

@functools.lru_cache(maxsize=None)
来源：http://iz.nszjky.cn

[U21] Py：自定义上下文管理器
来源：http://wd.hahajie.cn

@contextlib.contextmanager
来源：http://ro.yuntaijiaju.cn

[U22] Py：矩阵转置
来源：http://ts.muxihuayi.cn

list(zip(*m))
来源：http://mt.asd995.cn

[U23] Py：分块读取大文件
来源：http://ul.jianghongdianzi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bz.lnxyls.cn

[U24] Py：路径操作
来源：http://yp.nicolike.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://an.chemitech.net.cn

[U25] Py：CSV 按字典读
来源：http://ql.shxzskj.cn

csv.DictReader(f)
来源：http://nc.newstarts.cn

[U26] Py：并发下载
来源：http://bh.jianghongdianzi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rf.wgjwhj.cn

[U27] Py：异步 HTTP
来源：http://bq.huanxung.cn

aiohttp.ClientSession() 配合 async with
来源：http://oh.yuexingan06.cn

[U28] Py：类型别名
来源：http://us.lnxyls.cn

UserId = int
来源：http://tj.hahajie.cn

[U29] Py：属性校验
来源：http://se.nszjky.cn

@property 与 @x.setter 配合
来源：http://pp.shxzskj.cn

[U30] Py：数据类
来源：http://xl.haigaiapp.cn

@dataclass(slots=True)
来源：http://hz.nicolike.cn

[U31] Py：单测
来源：http://zp.jctech888.com.cn

python -m pytest -q
来源：http://xd.szxytkj.cn

[U32] Py：代码格式化
来源：http://ii.hahajie.cn

ruff format . && ruff check --fix .
来源：http://ya.nszjky.cn

[U33] Py：打包发布
来源：http://bl.wgjwhj.cn

python -m build  （依赖 pyproject.toml）
来源：http://pv.jctech888.com.cn

[U34] Py：判断编码
来源：http://sr.szxytkj.cn

chardet.detect(raw)
来源：http://px.szxytkj.cn

[U35] Py：发送邮件
来源：http://vh.nszjky.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xd.panjiajie.cn

[U36] Py：定时任务
来源：http://gb.hnjuh.cn

schedule.every(10).minutes.do(job)
来源：http://nq.muxihuayi.cn

[U37] Py：读写 Excel
来源：http://dv.yuntaijiaju.cn

pandas.read_excel / DataFrame.to_excel
来源：http://di.chemitech.net.cn

[U38] Py：获取脚本所在目录
来源：http://eu.9csxet.cn

Path(__file__).resolve().parent
来源：http://yu.521024.cn

[U39] Py：判断是否在交互环境
来源：http://zj.jianghongdianzi.cn

sys.stdout.isatty()
来源：http://or.huixinmuqiang.cn

[U40] Py：打印到标准错误
来源：http://kl.shxzskj.cn

print("err", file=sys.stderr)
来源：http://ty.newstarts.cn

[U41] PHP：初始化 Composer 项目
来源：http://ks.yuexingan06.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://mi.shtwfgs.cn

[U42] PHP：PSR-4 自动加载
来源：http://dc.shxzukj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jr.hahajie.cn

[U43] PHP：声明命名空间
来源：http://vv.muxihuayi.cn

namespace App\Http;
来源：http://gu.wgjwhj.cn

[U44] PHP：开启严格类型
来源：http://tw.newstarts.cn

declare(strict_types=1);
来源：http://wo.yuntaijiaju.cn

[U45] PHP：类型声明与返回类型
来源：http://rf.huixiangedu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ff.lnxyls.cn

[U46] PHP：可空类型
来源：http://bv.shxzskj.cn

?string $name = null
来源：http://lk.hahajie.cn

[U47] PHP：联合类型
来源：http://vy.9csxet.cn

int|string $id
来源：http://uy.colortex.cn

[U48] PHP：纯枚举
来源：http://cd.wgjwhj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zr.yuexingan06.cn

[U49] PHP：只读属性
来源：http://yf.shtwfgs.cn

public readonly string $name
来源：http://rw.huixiangedu.cn

[U50] PHP：构造器属性提升
来源：http://no.yuntaijiaju.cn

public function __construct(private int $id) {}
来源：http://gq.521024.cn

[U51] PHP：数组解构
来源：http://ja.asd995.cn

[$a, $b] = $arr;
来源：http://ij.shxzskj.cn

[U52] PHP：箭头函数
来源：http://fe.gzmigu.cn

$double = fn($x) => $x * 2;
来源：http://tm.panjiajie.cn

[U53] PHP：空合并运算符
来源：http://se.shxzukj.cn

$v = $a ?? $b ?? "default";
来源：http://jp.jctech888.com.cn

[U54] PHP：空安全调用
来源：http://ei.colortex.cn

$obj?->method()
来源：http://wu.lnxyls.cn

[U55] PHP：match 表达式
来源：http://np.wgjwhj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vz.huixinmuqiang.cn

[U56] PHP：命名参数
来源：http://ih.nicolike.cn

f(a: 1, b: 2)
来源：http://ku.nicolike.cn

[U57] PHP：字符串插值
来源：http://ir.szxytkj.cn

"值: {$a}"
来源：http://km.muxihuayi.cn

[U58] PHP：数组三件套
来源：http://zv.bookmarksfly.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vy.bookmarksfly.cn

[U59] PHP：自定义排序
来源：http://he.nicolike.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sk.huixinmuqiang.cn

[U60] PHP：JSON 编解码
来源：http://bp.asd995.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pk.shxzukj.cn

[U61] PHP：正则
来源：http://xo.huixiangedu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ue.haigaiapp.cn

[U62] PHP：日期对象
来源：http://yx.asd995.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gl.nszjky.cn

[U63] PHP：文件读写
来源：http://go.nicolike.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ou.wgjwhj.cn

[U64] PHP：目录遍历
来源：http://nl.shxzukj.cn

glob("dir/*.php");  scandir("dir");
来源：http://hn.yuexingan06.cn

[U65] PHP：会话
来源：http://ti.hahajie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rh.gzmigu.cn

[U66] PHP：设置 Cookie
来源：http://hz.asd995.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jn.jctech888.com.cn

[U67] PHP：处理文件上传
来源：http://lu.huixinmuqiang.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ju.yuntaijiaju.cn

[U68] PHP：PDO 连接
来源：http://ri.muxihuayi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gv.hnjuh.cn

[U69] PHP：PDO 预处理
来源：http://rk.szxytkj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://iu.huixinmuqiang.cn

[U70] PHP：PDO 事务
来源：http://xi.shxzukj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qi.hnjuh.cn

[U71] PHP：抛出异常
来源：http://ij.colortex.cn

throw new RuntimeException("失败", 500);
来源：http://vx.hnjuh.cn

[U72] PHP：写错误日志
来源：http://lk.gzmigu.cn

error_log("失败: " . $e->getMessage());
来源：http://md.shtwfgs.cn

[U73] PHP：读取 ini 配置
来源：http://kx.huanxung.cn

parse_ini_file("config.ini", true)
来源：http://nd.huixiangedu.cn

[U74] PHP：读取环境变量
来源：http://xh.szxytkj.cn

getenv("APP_ENV") ?: "production"
来源：http://gs.521024.cn

[U75] PHP：依赖注入
来源：http://xp.521024.cn

composer require psr/container
来源：http://js.521024.cn

[U76] PHP：简单路由
来源：http://ie.muxihuayi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://af.chemitech.net.cn

[U77] PHP：模板渲染
来源：http://bl.bjjhwx.cn

composer require twig/twig
来源：http://js.haigaiapp.cn

[U78] PHP：单元测试
来源：http://kk.chemitech.net.cn

composer require --dev phpunit/phpunit
来源：http://fs.huanxung.cn

[U79] PHP：静态分析
来源：http://hb.chemitech.net.cn

composer require --dev phpstan/phpstan
来源：http://kf.szxytkj.cn

[U80] PHP：代码规范修复
来源：http://aq.lnxyls.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://rb.wgjwhj.cn

[U81] JS：初始化项目
来源：http://pq.yuexingan06.cn

npm init -y;  npm i express
来源：http://df.521024.cn

[U82] JS：package.json 脚本
来源：http://us.muxihuayi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tg.shtwfgs.cn

[U83] JS：ES Module 导入导出
来源：http://eo.haigaiapp.cn

export const a = 1;  import { a } from "./m.js";
来源：http://oo.szsharing.cn

[U84] JS：CommonJS 写法
来源：http://yg.panjiajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://kc.shxzskj.cn

[U85] JS：可选链
来源：http://xx.shxzukj.cn

a?.b?.c
来源：http://uw.jctech888.com.cn

[U86] JS：空值合并
来源：http://vm.huanxung.cn

a ?? b
来源：http://oe.shtwfgs.cn

[U87] JS：解构默认值
来源：http://zx.asd995.cn

const { a = 1, b = 2 } = obj;
来源：http://vm.yuntaijiaju.cn

[U88] JS：对象展开合并
来源：http://gs.9csxet.cn

{ ...a, ...b }
来源：http://lu.huixinmuqiang.cn

[U89] JS：数组去重
来源：http://kz.bookmarksfly.cn

[...new Set(arr)]
来源：http://ji.lnxyls.cn

[U90] JS：数字数组排序
来源：http://tu.huanxung.cn

[...arr].sort((a, b) => a - b)
来源：http://gp.hahajie.cn

[U91] JS：对象键值遍历
来源：http://qv.huixiangedu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tf.huixiangedu.cn

[U92] JS：深拷贝
来源：http://su.gzmigu.cn

structuredClone(obj)
来源：http://hs.huixiangedu.cn

[U93] JS：模板字符串
来源：http://sa.huanxung.cn

`共 ${n} 条`
来源：http://ky.huanxung.cn

[U94] JS：箭头函数
来源：http://ma.bookmarksfly.cn

const double = x => x * 2;
来源：http://cf.shxzukj.cn

[U95] JS：Promise 包装
来源：http://vp.huanxung.cn

new Promise((resolve, reject) => {})
来源：http://ec.wgjwhj.cn

[U96] JS：async/await 与异常
来源：http://bd.szsharing.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pf.hahajie.cn

[U97] JS：并发请求
来源：http://xx.nicolike.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zq.nszjky.cn

[U98] JS：fetch 带 JSON
来源：http://pe.shxzskj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lb.9csxet.cn

[U99] JS：事件监听
来源：http://is.muxihuayi.cn

el.addEventListener("click", e => {})
来源：http://xs.huixinmuqiang.cn

[U100] JS：DOM 查询
来源：http://vx.haigaiapp.cn

document.querySelector(".item")
来源：http://fm.9csxet.cn

[U101] JS：classList 操作
来源：http://vt.panjiajie.cn

el.classList.toggle("active")
来源：http://ww.521024.cn

[U102] JS：本地存储
来源：http://xm.9csxet.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ni.huixiangedu.cn

[U103] JS：定时器
来源：http://im.huanxung.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://im.colortex.cn

[U104] JS：防抖
来源：http://dy.9csxet.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vs.huanxung.cn

[U105] JS：节流
来源：http://ya.hahajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ee.bookmarksfly.cn

[U106] JS：日期格式化
来源：http://yc.asd995.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xt.jianghongdianzi.cn


<!-- 参考信息 -->