代发 wailian999

[T19] Swift：可选绑定
来源：http://xn.shxzskj.cn

if let n = opt { print(n) }
来源：http://zf.shxzukj.cn

[T20] Swift：数组操作
来源：http://ro.muxihuayi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://sh.jctech888.com.cn

[T21] Swift：遍历
来源：http://ie.bookmarksfly.cn

for x in a { print(x) }
来源：http://gc.szxytkj.cn

[T22] Swift：字典
来源：http://ej.huixiangedu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ig.muxihuayi.cn

[T23] Swift：函数
来源：http://wm.panjiajie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dq.shtwfgs.cn

[T24] Swift：闭包
来源：http://bi.nicolike.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ru.panjiajie.cn

[T25] Swift：结构体
来源：http://py.haigaiapp.cn

struct P { var x: Int }
来源：http://vd.gzmigu.cn

[T26] Swift：类与重写
来源：http://mf.bookmarksfly.cn

class A: Base { override func f() {} }
来源：http://gv.huixinmuqiang.cn

[T27] Swift：错误处理
来源：http://ex.wgjwhj.cn

do { try f() } catch { print(error) }
来源：http://pe.lnxyls.cn

[T28] Swift：枚举
来源：http://px.chemitech.net.cn

enum Color { case red, green }
来源：http://ja.szsharing.cn

[T29] Swift：guard 提前返回
来源：http://wj.huixinmuqiang.cn

guard let x = opt else { return }
来源：http://kh.nszjky.cn

[T30] Swift：协议
来源：http://fy.jianghongdianzi.cn

protocol Shape { func area() -> Double }
来源：http://jg.hahajie.cn

[T31] Lua：Hello World
来源：http://qj.shtwfgs.cn

print("Hello")
来源：http://kq.panjiajie.cn

[T32] Lua：局部变量
来源：http://la.wgjwhj.cn

local a = 1
来源：http://ho.lnxyls.cn

[T33] Lua：表（数组）
来源：http://ck.muxihuayi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://od.huixiangedu.cn

[T34] Lua：遍历表
来源：http://vx.jctech888.com.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://cy.9csxet.cn

[T35] Lua：字典表
来源：http://sb.nicolike.cn

local d = { a = 1 };  d.b = 2
来源：http://bo.shxzukj.cn

[T36] Lua：函数
来源：http://jf.hahajie.cn

function add(a, b) return a + b end
来源：http://ig.asd995.cn

[T37] Lua：字符串拼接
来源：http://gv.shxzukj.cn

"a" .. "b"
来源：http://fh.bookmarksfly.cn

[T38] Lua：条件
来源：http://gg.jianghongdianzi.cn

if x > 0 then print("正") end
来源：http://md.gzmigu.cn

[T39] Lua：模式匹配
来源：http://mq.jctech888.com.cn

string.find(s, "%d+")
来源：http://zp.shxzskj.cn

[T40] Lua：元表
来源：http://cd.lnxyls.cn

setmetatable({}, { __index = base })
来源：http://in.wgjwhj.cn

[T41] Perl：Hello World
来源：http://od.bookmarksfly.cn

print "Hello\n";
来源：http://gt.asd995.cn

[T42] Perl：变量类型
来源：http://pq.huixiangedu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pd.szsharing.cn

[T43] Perl：字符串插值
来源：http://kp.bookmarksfly.cn

"值: $a"
来源：http://qz.yuntaijiaju.cn

[T44] Perl：条件
来源：http://nu.nicolike.cn

if ($a > 0) { print "正"; }
来源：http://ks.yuexingan06.cn

[T45] Perl：数组遍历
来源：http://yc.lnxyls.cn

for my $x (@arr) { print $x; }
来源：http://na.szxytkj.cn

[T46] Perl：哈希操作
来源：http://ii.gzmigu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wr.huanxung.cn

[T47] Perl：正则捕获
来源：http://gr.hnjuh.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://zv.newstarts.cn

[T48] Perl：正则替换
来源：http://cn.nicolike.cn

$s =~ s/old/new/g;
来源：http://gu.wgjwhj.cn

[T49] Perl：函数
来源：http://qi.colortex.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nq.muxihuayi.cn

[T50] Perl：逐行读文件
来源：http://cp.nicolike.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xh.yuntaijiaju.cn

while (my $line = <$fh>) { print $line; }
来源：http://ar.nicolike.cn

[T51] Scala：Hello World
来源：http://nm.nszjky.cn

println("Hello")
来源：http://ae.jctech888.com.cn

[T52] Scala：变量
来源：http://hl.hnjuh.cn

val a = 1;  var b = 2
来源：http://xw.521024.cn

[T53] Scala：字符串插值
来源：http://cg.huixiangedu.cn

s"值: $b"
来源：http://qt.haigaiapp.cn

[T54] Scala：集合映射
来源：http://pn.bjjhwx.cn

List(1, 2, 3).map(_ * 2)
来源：http://ca.gzmigu.cn

[T55] Scala：集合过滤
来源：http://nl.jianghongdianzi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://tj.colortex.cn

[T56] Scala：样例类
来源：http://ss.huanxung.cn

case class User(name: String, age: Int)
来源：http://eo.huixinmuqiang.cn

[T57] Scala：模式匹配
来源：http://ng.nicolike.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://kh.nszjky.cn

[T58] Scala：函数定义
来源：http://yh.asd995.cn

def add(a: Int, b: Int): Int = a + b
来源：http://je.shxzukj.cn

[T59] Scala：循环
来源：http://ik.nszjky.cn

for (i <- 1 to 10) println(i)
来源：http://qs.hahajie.cn

[T60] Scala：折叠
来源：http://ww.chemitech.net.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dp.yuntaijiaju.cn

================================================================================
来源：http://wa.yuexingan06.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pz.hahajie.cn

================================================================================
来源：http://mp.colortex.cn

[U01] Py：创建虚拟环境
来源：http://ee.shxzskj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jj.hnjuh.cn

[U02] Py：导出 / 安装依赖
来源：http://sp.haigaiapp.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ez.panjiajie.cn

[U03] Py：加载 .env 配置
来源：http://sb.newstarts.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wk.wgjwhj.cn

[U04] Py：变量调试打印
来源：http://lh.hahajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ua.huixiangedu.cn

[U05] Py：列表去重且保序
来源：http://ev.shxzskj.cn

list(dict.fromkeys(arr))
来源：http://vg.haigaiapp.cn

[U06] Py：合并两个字典
来源：http://ew.nicolike.cn

{**a, **b}
来源：http://db.bookmarksfly.cn

[U07] Py：反转字典键值
来源：http://fq.yuntaijiaju.cn

{v: k for k, v in d.items()}
来源：http://zm.521024.cn

[U08] Py：展平二维列表
来源：http://nh.nszjky.cn

[y for x in nested for y in x]
来源：http://ly.521024.cn

[U09] Py：字典取最大值的键
来源：http://mn.szsharing.cn

max(d, key=d.get)
来源：http://zy.gzmigu.cn

[U10] Py：按值排序字典
来源：http://ge.wgjwhj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fk.asd995.cn

[U11] Py：生成器表达式
来源：http://vn.yuexingan06.cn

(x * 2 for x in arr)
来源：http://dz.bookmarksfly.cn

[U12] Py：取出现最多的 3 个元素
来源：http://uy.huanxung.cn

Counter(arr).most_common(3)
来源：http://rv.gzmigu.cn

[U13] Py：固定长度队列
来源：http://xf.panjiajie.cn

deque(maxlen=10)
来源：http://le.lnxyls.cn

[U14] Py：分组收集到列表
来源：http://dj.chemitech.net.cn

defaultdict(list)
来源：http://gl.szxytkj.cn

[U15] Py：高精度计时
来源：http://wy.muxihuayi.cn

t = time.perf_counter()
来源：http://pc.huixinmuqiang.cn

[U16] Py：命令行参数解析
来源：http://fe.haigaiapp.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rp.jianghongdianzi.cn

[U17] Py：初始化日志
来源：http://lo.nszjky.cn

logging.basicConfig(level=logging.INFO)
来源：http://xb.lnxyls.cn

[U18] Py：预编译正则
来源：http://jd.jianghongdianzi.cn

pat = re.compile(r"\d+")
来源：http://ol.nicolike.cn

[U19] Py：正则替换带回调
来源：http://ng.gzmigu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fc.bjjhwx.cn

[U20] Py：缓存函数结果
来源：http://hg.hahajie.cn

@functools.lru_cache(maxsize=None)
来源：http://pu.newstarts.cn

[U21] Py：自定义上下文管理器
来源：http://su.yuntaijiaju.cn

@contextlib.contextmanager
来源：http://tb.muxihuayi.cn

[U22] Py：矩阵转置
来源：http://de.szsharing.cn

list(zip(*m))
来源：http://ie.huixinmuqiang.cn

[U23] Py：分块读取大文件
来源：http://tb.huanxung.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fn.gzmigu.cn

[U24] Py：路径操作
来源：http://wj.asd995.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xw.szxytkj.cn

[U25] Py：CSV 按字典读
来源：http://tq.colortex.cn

csv.DictReader(f)
来源：http://vo.jctech888.com.cn

[U26] Py：并发下载
来源：http://la.yuexingan06.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mu.huixinmuqiang.cn

[U27] Py：异步 HTTP
来源：http://lh.yuntaijiaju.cn

aiohttp.ClientSession() 配合 async with
来源：http://wn.9csxet.cn

[U28] Py：类型别名
来源：http://jc.jctech888.com.cn

UserId = int
来源：http://gr.haigaiapp.cn

[U29] Py：属性校验
来源：http://ou.shxzukj.cn

@property 与 @x.setter 配合
来源：http://sp.yuntaijiaju.cn

[U30] Py：数据类
来源：http://at.nszjky.cn

@dataclass(slots=True)
来源：http://uj.haigaiapp.cn

[U31] Py：单测
来源：http://vi.521024.cn

python -m pytest -q
来源：http://ze.shxzskj.cn

[U32] Py：代码格式化
来源：http://yy.9csxet.cn

ruff format . && ruff check --fix .
来源：http://ee.jctech888.com.cn

[U33] Py：打包发布
来源：http://tx.lnxyls.cn

python -m build  （依赖 pyproject.toml）
来源：http://gf.yuntaijiaju.cn

[U34] Py：判断编码
来源：http://rw.haigaiapp.cn

chardet.detect(raw)
来源：http://xd.yuexingan06.cn

[U35] Py：发送邮件
来源：http://fo.shtwfgs.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yz.shxzskj.cn

[U36] Py：定时任务
来源：http://cx.nszjky.cn

schedule.every(10).minutes.do(job)
来源：http://kf.huanxung.cn

[U37] Py：读写 Excel
来源：http://gb.nicolike.cn

pandas.read_excel / DataFrame.to_excel
来源：http://hq.wgjwhj.cn

[U38] Py：获取脚本所在目录
来源：http://ka.szsharing.cn

Path(__file__).resolve().parent
来源：http://br.asd995.cn

[U39] Py：判断是否在交互环境
来源：http://kk.jianghongdianzi.cn

sys.stdout.isatty()
来源：http://iy.hahajie.cn

[U40] Py：打印到标准错误
来源：http://yj.panjiajie.cn

print("err", file=sys.stderr)
来源：http://ww.hahajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://jz.muxihuayi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://fg.shxzskj.cn

[U42] PHP：PSR-4 自动加载
来源：http://ha.chemitech.net.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gj.shxzskj.cn

[U43] PHP：声明命名空间
来源：http://zo.szsharing.cn

namespace App\Http;
来源：http://dn.9csxet.cn

[U44] PHP：开启严格类型
来源：http://pk.nicolike.cn

declare(strict_types=1);
来源：http://qa.colortex.cn

[U45] PHP：类型声明与返回类型
来源：http://ic.shtwfgs.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ak.shxzskj.cn

[U46] PHP：可空类型
来源：http://sm.jctech888.com.cn

?string $name = null
来源：http://cn.shtwfgs.cn

[U47] PHP：联合类型
来源：http://ly.bjjhwx.cn

int|string $id
来源：http://vq.hahajie.cn

[U48] PHP：纯枚举
来源：http://fi.jianghongdianzi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nm.chemitech.net.cn

[U49] PHP：只读属性
来源：http://qr.jianghongdianzi.cn

public readonly string $name
来源：http://oj.huanxung.cn

[U50] PHP：构造器属性提升
来源：http://hf.9csxet.cn

public function __construct(private int $id) {}
来源：http://pl.yuntaijiaju.cn

[U51] PHP：数组解构
来源：http://ym.chemitech.net.cn

[$a, $b] = $arr;
来源：http://da.hahajie.cn

[U52] PHP：箭头函数
来源：http://kn.haigaiapp.cn

$double = fn($x) => $x * 2;
来源：http://la.lnxyls.cn

[U53] PHP：空合并运算符
来源：http://nd.chemitech.net.cn

$v = $a ?? $b ?? "default";
来源：http://cp.huixiangedu.cn

[U54] PHP：空安全调用
来源：http://ju.jctech888.com.cn

$obj?->method()
来源：http://gs.chemitech.net.cn

[U55] PHP：match 表达式
来源：http://ti.hnjuh.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zp.nicolike.cn

[U56] PHP：命名参数
来源：http://ue.newstarts.cn

f(a: 1, b: 2)
来源：http://tb.bookmarksfly.cn

[U57] PHP：字符串插值
来源：http://nf.wgjwhj.cn

"值: {$a}"
来源：http://qk.huanxung.cn

[U58] PHP：数组三件套
来源：http://ag.colortex.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nr.yuntaijiaju.cn

[U59] PHP：自定义排序
来源：http://dp.shxzukj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pj.lnxyls.cn

[U60] PHP：JSON 编解码
来源：http://he.chemitech.net.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://uj.hahajie.cn

[U61] PHP：正则
来源：http://lq.colortex.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://no.szxytkj.cn

[U62] PHP：日期对象
来源：http://hn.szsharing.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zl.colortex.cn

[U63] PHP：文件读写
来源：http://bv.asd995.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sm.shxzskj.cn

[U64] PHP：目录遍历
来源：http://ca.yuexingan06.cn

glob("dir/*.php");  scandir("dir");
来源：http://mz.9csxet.cn

[U65] PHP：会话
来源：http://au.shxzukj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://qy.nicolike.cn

[U66] PHP：设置 Cookie
来源：http://zq.huanxung.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tr.gzmigu.cn

[U67] PHP：处理文件上传
来源：http://kr.jianghongdianzi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ev.newstarts.cn

[U68] PHP：PDO 连接
来源：http://bc.521024.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nf.panjiajie.cn

[U69] PHP：PDO 预处理
来源：http://qo.wgjwhj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bw.muxihuayi.cn

[U70] PHP：PDO 事务
来源：http://ii.newstarts.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ps.9csxet.cn

[U71] PHP：抛出异常
来源：http://cf.lnxyls.cn

throw new RuntimeException("失败", 500);
来源：http://cz.asd995.cn

[U72] PHP：写错误日志
来源：http://nk.gzmigu.cn

error_log("失败: " . $e->getMessage());
来源：http://eu.nicolike.cn

[U73] PHP：读取 ini 配置
来源：http://pl.yuntaijiaju.cn

parse_ini_file("config.ini", true)
来源：http://cg.panjiajie.cn

[U74] PHP：读取环境变量
来源：http://xd.panjiajie.cn

getenv("APP_ENV") ?: "production"
来源：http://mf.shtwfgs.cn

[U75] PHP：依赖注入
来源：http://lr.lnxyls.cn

composer require psr/container
来源：http://zq.hahajie.cn

[U76] PHP：简单路由
来源：http://ww.huixinmuqiang.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://it.wgjwhj.cn

[U77] PHP：模板渲染
来源：http://xm.szsharing.cn

composer require twig/twig
来源：http://ty.newstarts.cn

[U78] PHP：单元测试
来源：http://qq.hnjuh.cn

composer require --dev phpunit/phpunit
来源：http://io.wgjwhj.cn

[U79] PHP：静态分析
来源：http://qd.hnjuh.cn

composer require --dev phpstan/phpstan
来源：http://xw.gzmigu.cn

[U80] PHP：代码规范修复
来源：http://lu.colortex.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://mx.panjiajie.cn

[U81] JS：初始化项目
来源：http://yl.521024.cn

npm init -y;  npm i express
来源：http://px.521024.cn

[U82] JS：package.json 脚本
来源：http://el.szxytkj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cc.chemitech.net.cn

[U83] JS：ES Module 导入导出
来源：http://go.lnxyls.cn

export const a = 1;  import { a } from "./m.js";
来源：http://tx.hahajie.cn

[U84] JS：CommonJS 写法
来源：http://yq.bjjhwx.cn

module.exports = { a };  const { a } = require("./m");
来源：http://gr.shxzukj.cn

[U85] JS：可选链
来源：http://mt.huanxung.cn

a?.b?.c
来源：http://gc.huanxung.cn

[U86] JS：空值合并
来源：http://zq.huixiangedu.cn

a ?? b
来源：http://zu.9csxet.cn

[U87] JS：解构默认值
来源：http://oy.huixiangedu.cn

const { a = 1, b = 2 } = obj;
来源：http://og.newstarts.cn

[U88] JS：对象展开合并
来源：http://er.huixiangedu.cn

{ ...a, ...b }
来源：http://ia.gzmigu.cn

[U89] JS：数组去重
来源：http://lm.nicolike.cn

[...new Set(arr)]
来源：http://nx.9csxet.cn

[U90] JS：数字数组排序
来源：http://ye.jctech888.com.cn

[...arr].sort((a, b) => a - b)
来源：http://ik.bjjhwx.cn

[U91] JS：对象键值遍历
来源：http://fp.yuexingan06.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hl.huixiangedu.cn

[U92] JS：深拷贝
来源：http://rg.panjiajie.cn

structuredClone(obj)
来源：http://vw.newstarts.cn

[U93] JS：模板字符串
来源：http://yw.szxytkj.cn

`共 ${n} 条`
来源：http://ey.huixinmuqiang.cn

[U94] JS：箭头函数
来源：http://wx.shtwfgs.cn

const double = x => x * 2;
来源：http://jh.newstarts.cn

[U95] JS：Promise 包装
来源：http://tf.shtwfgs.cn

new Promise((resolve, reject) => {})
来源：http://nu.wgjwhj.cn

[U96] JS：async/await 与异常
来源：http://vb.nszjky.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nv.9csxet.cn

[U97] JS：并发请求
来源：http://jc.nicolike.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://av.colortex.cn

[U98] JS：fetch 带 JSON
来源：http://yf.hnjuh.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hf.chemitech.net.cn

[U99] JS：事件监听
来源：http://zz.jianghongdianzi.cn

el.addEventListener("click", e => {})
来源：http://jc.colortex.cn

[U100] JS：DOM 查询
来源：http://er.9csxet.cn

document.querySelector(".item")
来源：http://jc.shtwfgs.cn

[U101] JS：classList 操作
来源：http://np.panjiajie.cn

el.classList.toggle("active")
来源：http://rp.gzmigu.cn

[U102] JS：本地存储
来源：http://go.nicolike.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://cz.muxihuayi.cn

[U103] JS：定时器
来源：http://sm.yuntaijiaju.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rk.huanxung.cn

[U104] JS：防抖
来源：http://rz.lnxyls.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ch.nszjky.cn

[U105] JS：节流
来源：http://fy.colortex.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qi.huixiangedu.cn

[U106] JS：日期格式化
来源：http://df.jctech888.com.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://db.nszjky.cn


<!-- 参考信息 -->