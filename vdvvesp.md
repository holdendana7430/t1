代发 wailian999

[T19] Swift：可选绑定
来源：http://uf.wgjwhj.cn

if let n = opt { print(n) }
来源：http://ui.lnxyls.cn

[T20] Swift：数组操作
来源：http://jr.jianghongdianzi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://tk.hnjuh.cn

[T21] Swift：遍历
来源：http://yr.jctech888.com.cn

for x in a { print(x) }
来源：http://uo.muxihuayi.cn

[T22] Swift：字典
来源：http://dl.jianghongdianzi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://kp.wgjwhj.cn

[T23] Swift：函数
来源：http://ls.asd995.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qm.hahajie.cn

[T24] Swift：闭包
来源：http://zl.colortex.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://bq.huixinmuqiang.cn

[T25] Swift：结构体
来源：http://rz.gzmigu.cn

struct P { var x: Int }
来源：http://jh.shxzukj.cn

[T26] Swift：类与重写
来源：http://wm.lnxyls.cn

class A: Base { override func f() {} }
来源：http://zq.huanxung.cn

[T27] Swift：错误处理
来源：http://dy.newstarts.cn

do { try f() } catch { print(error) }
来源：http://qm.521024.cn

[T28] Swift：枚举
来源：http://ka.nszjky.cn

enum Color { case red, green }
来源：http://mr.lnxyls.cn

[T29] Swift：guard 提前返回
来源：http://vb.9csxet.cn

guard let x = opt else { return }
来源：http://xg.muxihuayi.cn

[T30] Swift：协议
来源：http://ce.shtwfgs.cn

protocol Shape { func area() -> Double }
来源：http://lh.huanxung.cn

[T31] Lua：Hello World
来源：http://tw.wgjwhj.cn

print("Hello")
来源：http://us.shtwfgs.cn

[T32] Lua：局部变量
来源：http://gw.huanxung.cn

local a = 1
来源：http://dz.hahajie.cn

[T33] Lua：表（数组）
来源：http://xs.shxzukj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ms.chemitech.net.cn

[T34] Lua：遍历表
来源：http://kc.szsharing.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://go.bjjhwx.cn

[T35] Lua：字典表
来源：http://st.hahajie.cn

local d = { a = 1 };  d.b = 2
来源：http://mr.haigaiapp.cn

[T36] Lua：函数
来源：http://em.wgjwhj.cn

function add(a, b) return a + b end
来源：http://qh.shtwfgs.cn

[T37] Lua：字符串拼接
来源：http://sk.gzmigu.cn

"a" .. "b"
来源：http://ch.jianghongdianzi.cn

[T38] Lua：条件
来源：http://mw.szsharing.cn

if x > 0 then print("正") end
来源：http://ii.huixiangedu.cn

[T39] Lua：模式匹配
来源：http://iw.9csxet.cn

string.find(s, "%d+")
来源：http://br.haigaiapp.cn

[T40] Lua：元表
来源：http://fe.9csxet.cn

setmetatable({}, { __index = base })
来源：http://za.521024.cn

[T41] Perl：Hello World
来源：http://hw.521024.cn

print "Hello\n";
来源：http://gq.panjiajie.cn

[T42] Perl：变量类型
来源：http://xu.bjjhwx.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://np.szxytkj.cn

[T43] Perl：字符串插值
来源：http://sn.chemitech.net.cn

"值: $a"
来源：http://af.lnxyls.cn

[T44] Perl：条件
来源：http://qz.bjjhwx.cn

if ($a > 0) { print "正"; }
来源：http://cz.newstarts.cn

[T45] Perl：数组遍历
来源：http://az.chemitech.net.cn

for my $x (@arr) { print $x; }
来源：http://jy.colortex.cn

[T46] Perl：哈希操作
来源：http://gd.szsharing.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lq.hahajie.cn

[T47] Perl：正则捕获
来源：http://bk.9csxet.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://lj.bjjhwx.cn

[T48] Perl：正则替换
来源：http://cd.521024.cn

$s =~ s/old/new/g;
来源：http://hg.bookmarksfly.cn

[T49] Perl：函数
来源：http://fy.haigaiapp.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://oz.nicolike.cn

[T50] Perl：逐行读文件
来源：http://vh.521024.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ib.muxihuayi.cn

while (my $line = <$fh>) { print $line; }
来源：http://gg.bookmarksfly.cn

[T51] Scala：Hello World
来源：http://tq.hnjuh.cn

println("Hello")
来源：http://qx.shxzskj.cn

[T52] Scala：变量
来源：http://be.muxihuayi.cn

val a = 1;  var b = 2
来源：http://tr.wgjwhj.cn

[T53] Scala：字符串插值
来源：http://qm.nszjky.cn

s"值: $b"
来源：http://sp.huanxung.cn

[T54] Scala：集合映射
来源：http://go.gzmigu.cn

List(1, 2, 3).map(_ * 2)
来源：http://cp.panjiajie.cn

[T55] Scala：集合过滤
来源：http://wr.asd995.cn

List(1, 2, 3).filter(_ > 1)
来源：http://mg.huixinmuqiang.cn

[T56] Scala：样例类
来源：http://ot.shxzskj.cn

case class User(name: String, age: Int)
来源：http://je.yuexingan06.cn

[T57] Scala：模式匹配
来源：http://vz.jianghongdianzi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://cm.huixiangedu.cn

[T58] Scala：函数定义
来源：http://od.haigaiapp.cn

def add(a: Int, b: Int): Int = a + b
来源：http://og.wgjwhj.cn

[T59] Scala：循环
来源：http://cb.jctech888.com.cn

for (i <- 1 to 10) println(i)
来源：http://fl.hnjuh.cn

[T60] Scala：折叠
来源：http://sm.chemitech.net.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ne.hahajie.cn

================================================================================
来源：http://xm.huixiangedu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rl.shxzukj.cn

================================================================================
来源：http://lh.hahajie.cn

[U01] Py：创建虚拟环境
来源：http://sp.yuexingan06.cn

python -m venv .venv && source .venv/bin/activate
来源：http://yn.colortex.cn

[U02] Py：导出 / 安装依赖
来源：http://gt.szxytkj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ao.nszjky.cn

[U03] Py：加载 .env 配置
来源：http://jc.shxzskj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://sw.yuntaijiaju.cn

[U04] Py：变量调试打印
来源：http://te.wgjwhj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ac.lnxyls.cn

[U05] Py：列表去重且保序
来源：http://wt.newstarts.cn

list(dict.fromkeys(arr))
来源：http://bx.szxytkj.cn

[U06] Py：合并两个字典
来源：http://no.bookmarksfly.cn

{**a, **b}
来源：http://mu.szsharing.cn

[U07] Py：反转字典键值
来源：http://by.szsharing.cn

{v: k for k, v in d.items()}
来源：http://mc.nicolike.cn

[U08] Py：展平二维列表
来源：http://lq.muxihuayi.cn

[y for x in nested for y in x]
来源：http://ta.nicolike.cn

[U09] Py：字典取最大值的键
来源：http://wu.shxzskj.cn

max(d, key=d.get)
来源：http://zp.panjiajie.cn

[U10] Py：按值排序字典
来源：http://mu.gzmigu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bi.szxytkj.cn

[U11] Py：生成器表达式
来源：http://ww.haigaiapp.cn

(x * 2 for x in arr)
来源：http://pl.szsharing.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ju.yuexingan06.cn

Counter(arr).most_common(3)
来源：http://sa.huixiangedu.cn

[U13] Py：固定长度队列
来源：http://os.lnxyls.cn

deque(maxlen=10)
来源：http://jr.chemitech.net.cn

[U14] Py：分组收集到列表
来源：http://ex.muxihuayi.cn

defaultdict(list)
来源：http://tk.jianghongdianzi.cn

[U15] Py：高精度计时
来源：http://nh.haigaiapp.cn

t = time.perf_counter()
来源：http://yz.huixinmuqiang.cn

[U16] Py：命令行参数解析
来源：http://rd.gzmigu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jl.huanxung.cn

[U17] Py：初始化日志
来源：http://nz.9csxet.cn

logging.basicConfig(level=logging.INFO)
来源：http://mn.hnjuh.cn

[U18] Py：预编译正则
来源：http://px.yuexingan06.cn

pat = re.compile(r"\d+")
来源：http://nz.bookmarksfly.cn

[U19] Py：正则替换带回调
来源：http://pz.shtwfgs.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hk.haigaiapp.cn

[U20] Py：缓存函数结果
来源：http://cu.shtwfgs.cn

@functools.lru_cache(maxsize=None)
来源：http://sq.asd995.cn

[U21] Py：自定义上下文管理器
来源：http://tv.huixiangedu.cn

@contextlib.contextmanager
来源：http://xy.nicolike.cn

[U22] Py：矩阵转置
来源：http://ya.colortex.cn

list(zip(*m))
来源：http://pm.chemitech.net.cn

[U23] Py：分块读取大文件
来源：http://ui.nszjky.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fm.hnjuh.cn

[U24] Py：路径操作
来源：http://sg.wgjwhj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://sl.lnxyls.cn

[U25] Py：CSV 按字典读
来源：http://bm.yuntaijiaju.cn

csv.DictReader(f)
来源：http://xn.nicolike.cn

[U26] Py：并发下载
来源：http://fa.nszjky.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vf.9csxet.cn

[U27] Py：异步 HTTP
来源：http://us.nszjky.cn

aiohttp.ClientSession() 配合 async with
来源：http://ki.huanxung.cn

[U28] Py：类型别名
来源：http://sj.haigaiapp.cn

UserId = int
来源：http://xj.huixiangedu.cn

[U29] Py：属性校验
来源：http://wy.muxihuayi.cn

@property 与 @x.setter 配合
来源：http://qz.huixinmuqiang.cn

[U30] Py：数据类
来源：http://jh.hnjuh.cn

@dataclass(slots=True)
来源：http://in.nicolike.cn

[U31] Py：单测
来源：http://nm.lnxyls.cn

python -m pytest -q
来源：http://ue.huanxung.cn

[U32] Py：代码格式化
来源：http://pq.nicolike.cn

ruff format . && ruff check --fix .
来源：http://jo.jianghongdianzi.cn

[U33] Py：打包发布
来源：http://vf.521024.cn

python -m build  （依赖 pyproject.toml）
来源：http://ht.hahajie.cn

[U34] Py：判断编码
来源：http://hm.nicolike.cn

chardet.detect(raw)
来源：http://gt.shxzukj.cn

[U35] Py：发送邮件
来源：http://ev.shxzukj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hs.shxzukj.cn

[U36] Py：定时任务
来源：http://rz.yuexingan06.cn

schedule.every(10).minutes.do(job)
来源：http://zo.muxihuayi.cn

[U37] Py：读写 Excel
来源：http://lm.bjjhwx.cn

pandas.read_excel / DataFrame.to_excel
来源：http://to.colortex.cn

[U38] Py：获取脚本所在目录
来源：http://nv.nszjky.cn

Path(__file__).resolve().parent
来源：http://au.bookmarksfly.cn

[U39] Py：判断是否在交互环境
来源：http://io.yuntaijiaju.cn

sys.stdout.isatty()
来源：http://yi.521024.cn

[U40] Py：打印到标准错误
来源：http://lz.nicolike.cn

print("err", file=sys.stderr)
来源：http://za.yuexingan06.cn

[U41] PHP：初始化 Composer 项目
来源：http://wh.haigaiapp.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jd.huanxung.cn

[U42] PHP：PSR-4 自动加载
来源：http://yo.szxytkj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lz.szxytkj.cn

[U43] PHP：声明命名空间
来源：http://rs.panjiajie.cn

namespace App\Http;
来源：http://ql.haigaiapp.cn

[U44] PHP：开启严格类型
来源：http://vk.szxytkj.cn

declare(strict_types=1);
来源：http://nm.hahajie.cn

[U45] PHP：类型声明与返回类型
来源：http://py.shxzskj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://un.huixinmuqiang.cn

[U46] PHP：可空类型
来源：http://ag.muxihuayi.cn

?string $name = null
来源：http://no.newstarts.cn

[U47] PHP：联合类型
来源：http://xz.hahajie.cn

int|string $id
来源：http://fe.shxzskj.cn

[U48] PHP：纯枚举
来源：http://nu.newstarts.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bv.hnjuh.cn

[U49] PHP：只读属性
来源：http://jn.huixiangedu.cn

public readonly string $name
来源：http://ts.nicolike.cn

[U50] PHP：构造器属性提升
来源：http://hs.shtwfgs.cn

public function __construct(private int $id) {}
来源：http://vs.bjjhwx.cn

[U51] PHP：数组解构
来源：http://tp.shxzukj.cn

[$a, $b] = $arr;
来源：http://sn.newstarts.cn

[U52] PHP：箭头函数
来源：http://th.bjjhwx.cn

$double = fn($x) => $x * 2;
来源：http://hi.newstarts.cn

[U53] PHP：空合并运算符
来源：http://fd.shxzukj.cn

$v = $a ?? $b ?? "default";
来源：http://lc.nicolike.cn

[U54] PHP：空安全调用
来源：http://rf.bjjhwx.cn

$obj?->method()
来源：http://yj.hnjuh.cn

[U55] PHP：match 表达式
来源：http://ec.chemitech.net.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://il.huixiangedu.cn

[U56] PHP：命名参数
来源：http://ye.huixiangedu.cn

f(a: 1, b: 2)
来源：http://zb.hnjuh.cn

[U57] PHP：字符串插值
来源：http://sg.wgjwhj.cn

"值: {$a}"
来源：http://cg.hnjuh.cn

[U58] PHP：数组三件套
来源：http://kg.nicolike.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xu.muxihuayi.cn

[U59] PHP：自定义排序
来源：http://az.shtwfgs.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gd.lnxyls.cn

[U60] PHP：JSON 编解码
来源：http://lj.nicolike.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yf.huanxung.cn

[U61] PHP：正则
来源：http://rc.shxzukj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://np.nicolike.cn

[U62] PHP：日期对象
来源：http://cv.yuntaijiaju.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xx.nszjky.cn

[U63] PHP：文件读写
来源：http://ga.shtwfgs.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kc.wgjwhj.cn

[U64] PHP：目录遍历
来源：http://ua.gzmigu.cn

glob("dir/*.php");  scandir("dir");
来源：http://sa.hahajie.cn

[U65] PHP：会话
来源：http://rp.shxzukj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rz.asd995.cn

[U66] PHP：设置 Cookie
来源：http://mz.huanxung.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ln.jianghongdianzi.cn

[U67] PHP：处理文件上传
来源：http://iq.huixiangedu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sd.yuntaijiaju.cn

[U68] PHP：PDO 连接
来源：http://cx.colortex.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ky.nszjky.cn

[U69] PHP：PDO 预处理
来源：http://xf.colortex.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ds.521024.cn

[U70] PHP：PDO 事务
来源：http://it.bookmarksfly.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vg.szsharing.cn

[U71] PHP：抛出异常
来源：http://yh.szsharing.cn

throw new RuntimeException("失败", 500);
来源：http://jk.gzmigu.cn

[U72] PHP：写错误日志
来源：http://wc.shxzskj.cn

error_log("失败: " . $e->getMessage());
来源：http://wt.bookmarksfly.cn

[U73] PHP：读取 ini 配置
来源：http://xh.colortex.cn

parse_ini_file("config.ini", true)
来源：http://fl.huixinmuqiang.cn

[U74] PHP：读取环境变量
来源：http://xv.muxihuayi.cn

getenv("APP_ENV") ?: "production"
来源：http://yo.huixinmuqiang.cn

[U75] PHP：依赖注入
来源：http://hi.yuntaijiaju.cn

composer require psr/container
来源：http://ll.muxihuayi.cn

[U76] PHP：简单路由
来源：http://aj.521024.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ib.huixinmuqiang.cn

[U77] PHP：模板渲染
来源：http://ry.bjjhwx.cn

composer require twig/twig
来源：http://tx.jctech888.com.cn

[U78] PHP：单元测试
来源：http://zl.lnxyls.cn

composer require --dev phpunit/phpunit
来源：http://ky.lnxyls.cn

[U79] PHP：静态分析
来源：http://up.shxzukj.cn

composer require --dev phpstan/phpstan
来源：http://sh.huixiangedu.cn

[U80] PHP：代码规范修复
来源：http://lr.gzmigu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ok.shxzukj.cn

[U81] JS：初始化项目
来源：http://lh.szsharing.cn

npm init -y;  npm i express
来源：http://sg.bookmarksfly.cn

[U82] JS：package.json 脚本
来源：http://db.muxihuayi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mc.muxihuayi.cn

[U83] JS：ES Module 导入导出
来源：http://bp.yuexingan06.cn

export const a = 1;  import { a } from "./m.js";
来源：http://lc.huixinmuqiang.cn

[U84] JS：CommonJS 写法
来源：http://mk.jctech888.com.cn

module.exports = { a };  const { a } = require("./m");
来源：http://mp.shtwfgs.cn

[U85] JS：可选链
来源：http://oz.jianghongdianzi.cn

a?.b?.c
来源：http://rq.9csxet.cn

[U86] JS：空值合并
来源：http://vt.nszjky.cn

a ?? b
来源：http://mn.lnxyls.cn

[U87] JS：解构默认值
来源：http://my.shxzukj.cn

const { a = 1, b = 2 } = obj;
来源：http://ar.jianghongdianzi.cn

[U88] JS：对象展开合并
来源：http://yy.nszjky.cn

{ ...a, ...b }
来源：http://sm.asd995.cn

[U89] JS：数组去重
来源：http://es.yuntaijiaju.cn

[...new Set(arr)]
来源：http://lh.colortex.cn

[U90] JS：数字数组排序
来源：http://ok.nicolike.cn

[...arr].sort((a, b) => a - b)
来源：http://zx.nszjky.cn

[U91] JS：对象键值遍历
来源：http://nc.9csxet.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ly.nicolike.cn

[U92] JS：深拷贝
来源：http://qn.nszjky.cn

structuredClone(obj)
来源：http://ht.yuexingan06.cn

[U93] JS：模板字符串
来源：http://li.shtwfgs.cn

`共 ${n} 条`
来源：http://ri.panjiajie.cn

[U94] JS：箭头函数
来源：http://rx.jianghongdianzi.cn

const double = x => x * 2;
来源：http://hi.panjiajie.cn

[U95] JS：Promise 包装
来源：http://wr.jctech888.com.cn

new Promise((resolve, reject) => {})
来源：http://ye.jianghongdianzi.cn

[U96] JS：async/await 与异常
来源：http://rd.9csxet.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xd.chemitech.net.cn

[U97] JS：并发请求
来源：http://vz.haigaiapp.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://pu.muxihuayi.cn

[U98] JS：fetch 带 JSON
来源：http://gu.hnjuh.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bv.yuntaijiaju.cn

[U99] JS：事件监听
来源：http://ag.yuexingan06.cn

el.addEventListener("click", e => {})
来源：http://cv.chemitech.net.cn

[U100] JS：DOM 查询
来源：http://hn.shtwfgs.cn

document.querySelector(".item")
来源：http://tf.lnxyls.cn

[U101] JS：classList 操作
来源：http://kg.chemitech.net.cn

el.classList.toggle("active")
来源：http://ic.asd995.cn

[U102] JS：本地存储
来源：http://hh.lnxyls.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wo.huixinmuqiang.cn

[U103] JS：定时器
来源：http://gf.yuexingan06.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mf.hnjuh.cn

[U104] JS：防抖
来源：http://xg.shxzukj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ty.hahajie.cn

[U105] JS：节流
来源：http://ri.huixinmuqiang.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vh.bookmarksfly.cn

[U106] JS：日期格式化
来源：http://kn.lnxyls.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qj.chemitech.net.cn


<!-- 参考信息 -->