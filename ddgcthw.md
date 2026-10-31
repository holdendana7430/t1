代发 wailian999

[T31] Lua：Hello World
来源：http://wh.muxihuayi.cn

print("Hello")
来源：http://lk.panjiajie.cn

[T32] Lua：局部变量
来源：http://pa.gzmigu.cn

local a = 1
来源：http://ns.yuntaijiaju.cn

[T33] Lua：表（数组）
来源：http://cj.newstarts.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://rf.panjiajie.cn

[T34] Lua：遍历表
来源：http://no.nszjky.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://tw.bookmarksfly.cn

[T35] Lua：字典表
来源：http://yx.colortex.cn

local d = { a = 1 };  d.b = 2
来源：http://fl.jctech888.com.cn

[T36] Lua：函数
来源：http://ww.szxytkj.cn

function add(a, b) return a + b end
来源：http://zb.jianghongdianzi.cn

[T37] Lua：字符串拼接
来源：http://lz.colortex.cn

"a" .. "b"
来源：http://ro.chemitech.net.cn

[T38] Lua：条件
来源：http://nv.colortex.cn

if x > 0 then print("正") end
来源：http://gp.nszjky.cn

[T39] Lua：模式匹配
来源：http://he.huixinmuqiang.cn

string.find(s, "%d+")
来源：http://xs.szxytkj.cn

[T40] Lua：元表
来源：http://zo.asd995.cn

setmetatable({}, { __index = base })
来源：http://br.haigaiapp.cn

[T41] Perl：Hello World
来源：http://sp.huixinmuqiang.cn

print "Hello\n";
来源：http://uq.haigaiapp.cn

[T42] Perl：变量类型
来源：http://xb.9csxet.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ih.hnjuh.cn

[T43] Perl：字符串插值
来源：http://fn.shxzskj.cn

"值: $a"
来源：http://nk.jctech888.com.cn

[T44] Perl：条件
来源：http://ts.lnxyls.cn

if ($a > 0) { print "正"; }
来源：http://fk.huixiangedu.cn

[T45] Perl：数组遍历
来源：http://qw.bookmarksfly.cn

for my $x (@arr) { print $x; }
来源：http://qf.szxytkj.cn

[T46] Perl：哈希操作
来源：http://xv.newstarts.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://yw.bjjhwx.cn

[T47] Perl：正则捕获
来源：http://ni.wgjwhj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wd.bjjhwx.cn

[T48] Perl：正则替换
来源：http://gq.gzmigu.cn

$s =~ s/old/new/g;
来源：http://yt.huixiangedu.cn

[T49] Perl：函数
来源：http://st.colortex.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://be.asd995.cn

[T50] Perl：逐行读文件
来源：http://ok.wgjwhj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://gm.yuntaijiaju.cn

while (my $line = <$fh>) { print $line; }
来源：http://cc.huixiangedu.cn

[T51] Scala：Hello World
来源：http://ay.yuntaijiaju.cn

println("Hello")
来源：http://sc.shtwfgs.cn

[T52] Scala：变量
来源：http://hr.nicolike.cn

val a = 1;  var b = 2
来源：http://mb.9csxet.cn

[T53] Scala：字符串插值
来源：http://be.nszjky.cn

s"值: $b"
来源：http://zk.huixinmuqiang.cn

[T54] Scala：集合映射
来源：http://xi.bookmarksfly.cn

List(1, 2, 3).map(_ * 2)
来源：http://px.panjiajie.cn

[T55] Scala：集合过滤
来源：http://hr.szxytkj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://nf.shtwfgs.cn

[T56] Scala：样例类
来源：http://hi.shxzskj.cn

case class User(name: String, age: Int)
来源：http://qw.yuexingan06.cn

[T57] Scala：模式匹配
来源：http://wu.yuexingan06.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vi.colortex.cn

[T58] Scala：函数定义
来源：http://vx.shxzukj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://xn.haigaiapp.cn

[T59] Scala：循环
来源：http://wd.yuexingan06.cn

for (i <- 1 to 10) println(i)
来源：http://ew.szxytkj.cn

[T60] Scala：折叠
来源：http://wh.newstarts.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jp.szxytkj.cn

================================================================================
来源：http://gh.gzmigu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kh.newstarts.cn

================================================================================
来源：http://ud.hahajie.cn

[U01] Py：创建虚拟环境
来源：http://zj.hahajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wu.nicolike.cn

[U02] Py：导出 / 安装依赖
来源：http://hk.muxihuayi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yq.nicolike.cn

[U03] Py：加载 .env 配置
来源：http://zv.hnjuh.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://za.hnjuh.cn

[U04] Py：变量调试打印
来源：http://yp.hnjuh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bg.panjiajie.cn

[U05] Py：列表去重且保序
来源：http://kr.gzmigu.cn

list(dict.fromkeys(arr))
来源：http://rn.haigaiapp.cn

[U06] Py：合并两个字典
来源：http://nh.yuntaijiaju.cn

{**a, **b}
来源：http://lg.szxytkj.cn

[U07] Py：反转字典键值
来源：http://ap.bookmarksfly.cn

{v: k for k, v in d.items()}
来源：http://wd.asd995.cn

[U08] Py：展平二维列表
来源：http://rj.shxzskj.cn

[y for x in nested for y in x]
来源：http://zi.gzmigu.cn

[U09] Py：字典取最大值的键
来源：http://fu.lnxyls.cn

max(d, key=d.get)
来源：http://yg.colortex.cn

[U10] Py：按值排序字典
来源：http://lf.hnjuh.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wh.nszjky.cn

[U11] Py：生成器表达式
来源：http://hp.panjiajie.cn

(x * 2 for x in arr)
来源：http://rk.szxytkj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ob.bjjhwx.cn

Counter(arr).most_common(3)
来源：http://ya.muxihuayi.cn

[U13] Py：固定长度队列
来源：http://sw.shxzskj.cn

deque(maxlen=10)
来源：http://ty.nicolike.cn

[U14] Py：分组收集到列表
来源：http://yi.hahajie.cn

defaultdict(list)
来源：http://um.yuexingan06.cn

[U15] Py：高精度计时
来源：http://xn.nicolike.cn

t = time.perf_counter()
来源：http://zi.bookmarksfly.cn

[U16] Py：命令行参数解析
来源：http://rw.szxytkj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://iv.asd995.cn

[U17] Py：初始化日志
来源：http://hh.521024.cn

logging.basicConfig(level=logging.INFO)
来源：http://jl.huanxung.cn

[U18] Py：预编译正则
来源：http://kh.huixinmuqiang.cn

pat = re.compile(r"\d+")
来源：http://wn.jctech888.com.cn

[U19] Py：正则替换带回调
来源：http://aj.bookmarksfly.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lz.nszjky.cn

[U20] Py：缓存函数结果
来源：http://gq.muxihuayi.cn

@functools.lru_cache(maxsize=None)
来源：http://ny.chemitech.net.cn

[U21] Py：自定义上下文管理器
来源：http://ul.haigaiapp.cn

@contextlib.contextmanager
来源：http://gm.jctech888.com.cn

[U22] Py：矩阵转置
来源：http://ed.jianghongdianzi.cn

list(zip(*m))
来源：http://gb.bookmarksfly.cn

[U23] Py：分块读取大文件
来源：http://rk.shtwfgs.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pb.nicolike.cn

[U24] Py：路径操作
来源：http://qt.jctech888.com.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hk.gzmigu.cn

[U25] Py：CSV 按字典读
来源：http://pz.nicolike.cn

csv.DictReader(f)
来源：http://gg.shtwfgs.cn

[U26] Py：并发下载
来源：http://ge.newstarts.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fa.asd995.cn

[U27] Py：异步 HTTP
来源：http://zk.gzmigu.cn

aiohttp.ClientSession() 配合 async with
来源：http://jn.szsharing.cn

[U28] Py：类型别名
来源：http://ya.shxzskj.cn

UserId = int
来源：http://oz.huixinmuqiang.cn

[U29] Py：属性校验
来源：http://qe.yuexingan06.cn

@property 与 @x.setter 配合
来源：http://by.lnxyls.cn

[U30] Py：数据类
来源：http://lq.gzmigu.cn

@dataclass(slots=True)
来源：http://xv.haigaiapp.cn

[U31] Py：单测
来源：http://ad.lnxyls.cn

python -m pytest -q
来源：http://kq.bjjhwx.cn

[U32] Py：代码格式化
来源：http://jk.wgjwhj.cn

ruff format . && ruff check --fix .
来源：http://ni.nszjky.cn

[U33] Py：打包发布
来源：http://zd.huixiangedu.cn

python -m build  （依赖 pyproject.toml）
来源：http://sx.gzmigu.cn

[U34] Py：判断编码
来源：http://tq.9csxet.cn

chardet.detect(raw)
来源：http://pd.bjjhwx.cn

[U35] Py：发送邮件
来源：http://bu.huixiangedu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yo.szxytkj.cn

[U36] Py：定时任务
来源：http://jf.wgjwhj.cn

schedule.every(10).minutes.do(job)
来源：http://bv.9csxet.cn

[U37] Py：读写 Excel
来源：http://vr.hnjuh.cn

pandas.read_excel / DataFrame.to_excel
来源：http://cb.hnjuh.cn

[U38] Py：获取脚本所在目录
来源：http://lm.yuexingan06.cn

Path(__file__).resolve().parent
来源：http://pr.shxzukj.cn

[U39] Py：判断是否在交互环境
来源：http://yh.shxzskj.cn

sys.stdout.isatty()
来源：http://ha.gzmigu.cn

[U40] Py：打印到标准错误
来源：http://bw.szxytkj.cn

print("err", file=sys.stderr)
来源：http://ka.panjiajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://pt.shtwfgs.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qv.huixinmuqiang.cn

[U42] PHP：PSR-4 自动加载
来源：http://vx.haigaiapp.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jd.nszjky.cn

[U43] PHP：声明命名空间
来源：http://kr.jctech888.com.cn

namespace App\Http;
来源：http://jf.szsharing.cn

[U44] PHP：开启严格类型
来源：http://jm.shxzukj.cn

declare(strict_types=1);
来源：http://yu.colortex.cn

[U45] PHP：类型声明与返回类型
来源：http://mo.shxzskj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://uk.bjjhwx.cn

[U46] PHP：可空类型
来源：http://nw.colortex.cn

?string $name = null
来源：http://bj.shxzskj.cn

[U47] PHP：联合类型
来源：http://aw.huixiangedu.cn

int|string $id
来源：http://rj.haigaiapp.cn

[U48] PHP：纯枚举
来源：http://cu.shxzskj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mp.shtwfgs.cn

[U49] PHP：只读属性
来源：http://bp.bjjhwx.cn

public readonly string $name
来源：http://kj.nicolike.cn

[U50] PHP：构造器属性提升
来源：http://bn.jianghongdianzi.cn

public function __construct(private int $id) {}
来源：http://eq.521024.cn

[U51] PHP：数组解构
来源：http://gs.bookmarksfly.cn

[$a, $b] = $arr;
来源：http://tf.nicolike.cn

[U52] PHP：箭头函数
来源：http://kl.bjjhwx.cn

$double = fn($x) => $x * 2;
来源：http://uv.bookmarksfly.cn

[U53] PHP：空合并运算符
来源：http://fk.huixiangedu.cn

$v = $a ?? $b ?? "default";
来源：http://fk.shxzskj.cn

[U54] PHP：空安全调用
来源：http://og.yuexingan06.cn

$obj?->method()
来源：http://vn.haigaiapp.cn

[U55] PHP：match 表达式
来源：http://io.nszjky.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://op.shtwfgs.cn

[U56] PHP：命名参数
来源：http://fp.521024.cn

f(a: 1, b: 2)
来源：http://gr.9csxet.cn

[U57] PHP：字符串插值
来源：http://mx.haigaiapp.cn

"值: {$a}"
来源：http://vo.asd995.cn

[U58] PHP：数组三件套
来源：http://uq.hahajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pt.shxzskj.cn

[U59] PHP：自定义排序
来源：http://hu.yuntaijiaju.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gv.haigaiapp.cn

[U60] PHP：JSON 编解码
来源：http://ac.szxytkj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cy.521024.cn

[U61] PHP：正则
来源：http://pn.chemitech.net.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lz.hahajie.cn

[U62] PHP：日期对象
来源：http://eo.nszjky.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ay.huanxung.cn

[U63] PHP：文件读写
来源：http://hj.huixiangedu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qc.nszjky.cn

[U64] PHP：目录遍历
来源：http://vi.colortex.cn

glob("dir/*.php");  scandir("dir");
来源：http://ii.huixiangedu.cn

[U65] PHP：会话
来源：http://iq.bookmarksfly.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://id.9csxet.cn

[U66] PHP：设置 Cookie
来源：http://pm.shtwfgs.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vr.huixinmuqiang.cn

[U67] PHP：处理文件上传
来源：http://za.asd995.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kd.szxytkj.cn

[U68] PHP：PDO 连接
来源：http://bo.jctech888.com.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gv.yuexingan06.cn

[U69] PHP：PDO 预处理
来源：http://ta.huixinmuqiang.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sy.huixiangedu.cn

[U70] PHP：PDO 事务
来源：http://fm.wgjwhj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ru.shtwfgs.cn

[U71] PHP：抛出异常
来源：http://cq.panjiajie.cn

throw new RuntimeException("失败", 500);
来源：http://tt.szxytkj.cn

[U72] PHP：写错误日志
来源：http://hm.huixiangedu.cn

error_log("失败: " . $e->getMessage());
来源：http://lm.nicolike.cn

[U73] PHP：读取 ini 配置
来源：http://oe.yuntaijiaju.cn

parse_ini_file("config.ini", true)
来源：http://sc.9csxet.cn

[U74] PHP：读取环境变量
来源：http://xm.9csxet.cn

getenv("APP_ENV") ?: "production"
来源：http://vl.asd995.cn

[U75] PHP：依赖注入
来源：http://th.521024.cn

composer require psr/container
来源：http://pg.szsharing.cn

[U76] PHP：简单路由
来源：http://nw.chemitech.net.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ds.haigaiapp.cn

[U77] PHP：模板渲染
来源：http://wf.panjiajie.cn

composer require twig/twig
来源：http://ei.9csxet.cn

[U78] PHP：单元测试
来源：http://hd.nszjky.cn

composer require --dev phpunit/phpunit
来源：http://om.yuexingan06.cn

[U79] PHP：静态分析
来源：http://rr.panjiajie.cn

composer require --dev phpstan/phpstan
来源：http://rr.jctech888.com.cn

[U80] PHP：代码规范修复
来源：http://zt.nicolike.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://rq.jianghongdianzi.cn

[U81] JS：初始化项目
来源：http://lr.wgjwhj.cn

npm init -y;  npm i express
来源：http://dr.shxzskj.cn

[U82] JS：package.json 脚本
来源：http://la.hnjuh.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ot.shxzskj.cn

[U83] JS：ES Module 导入导出
来源：http://tp.huixinmuqiang.cn

export const a = 1;  import { a } from "./m.js";
来源：http://yn.bjjhwx.cn

[U84] JS：CommonJS 写法
来源：http://wg.bjjhwx.cn

module.exports = { a };  const { a } = require("./m");
来源：http://by.bookmarksfly.cn

[U85] JS：可选链
来源：http://vc.bookmarksfly.cn

a?.b?.c
来源：http://me.bjjhwx.cn

[U86] JS：空值合并
来源：http://px.colortex.cn

a ?? b
来源：http://cz.9csxet.cn

[U87] JS：解构默认值
来源：http://iu.nicolike.cn

const { a = 1, b = 2 } = obj;
来源：http://hm.muxihuayi.cn

[U88] JS：对象展开合并
来源：http://ki.shxzukj.cn

{ ...a, ...b }
来源：http://bl.szsharing.cn

[U89] JS：数组去重
来源：http://ap.jctech888.com.cn

[...new Set(arr)]
来源：http://qa.shxzukj.cn

[U90] JS：数字数组排序
来源：http://av.hnjuh.cn

[...arr].sort((a, b) => a - b)
来源：http://rz.nszjky.cn

[U91] JS：对象键值遍历
来源：http://tt.hnjuh.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xi.huanxung.cn

[U92] JS：深拷贝
来源：http://fa.haigaiapp.cn

structuredClone(obj)
来源：http://ux.9csxet.cn

[U93] JS：模板字符串
来源：http://es.colortex.cn

`共 ${n} 条`
来源：http://fp.yuexingan06.cn

[U94] JS：箭头函数
来源：http://nv.shxzskj.cn

const double = x => x * 2;
来源：http://el.huixiangedu.cn

[U95] JS：Promise 包装
来源：http://sk.jctech888.com.cn

new Promise((resolve, reject) => {})
来源：http://uh.nszjky.cn

[U96] JS：async/await 与异常
来源：http://bs.521024.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kb.szsharing.cn

[U97] JS：并发请求
来源：http://zr.muxihuayi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://hj.szsharing.cn

[U98] JS：fetch 带 JSON
来源：http://oc.lnxyls.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zs.hnjuh.cn

[U99] JS：事件监听
来源：http://cc.9csxet.cn

el.addEventListener("click", e => {})
来源：http://vc.hnjuh.cn

[U100] JS：DOM 查询
来源：http://ya.nicolike.cn

document.querySelector(".item")
来源：http://ki.chemitech.net.cn

[U101] JS：classList 操作
来源：http://dh.shxzskj.cn

el.classList.toggle("active")
来源：http://va.bookmarksfly.cn

[U102] JS：本地存储
来源：http://qg.newstarts.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://lq.jianghongdianzi.cn

[U103] JS：定时器
来源：http://va.bjjhwx.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bx.hahajie.cn

[U104] JS：防抖
来源：http://uo.muxihuayi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iy.newstarts.cn

[U105] JS：节流
来源：http://fc.shtwfgs.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jw.asd995.cn

[U106] JS：日期格式化
来源：http://fu.shxzukj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.bjjhwx.cn

[U107] JS：数字千分位
来源：http://od.newstarts.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mz.jianghongdianzi.cn

[U108] JS：随机整数
来源：http://hn.newstarts.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vo.gzmigu.cn

[U109] JS：数组分组
来源：http://kb.nszjky.cn

Object.groupBy(arr, x => x.type)
来源：http://xo.jctech888.com.cn

[U110] JS：数组分块
来源：http://iy.panjiajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ry.asd995.cn

[U111] JS：对象转 Map
来源：http://gr.bookmarksfly.cn

new Map(Object.entries(obj))
来源：http://rj.521024.cn

[U112] JS：字符串补位
来源：http://ae.newstarts.cn

"7".padStart(3, "0")
来源：http://or.bookmarksfly.cn

[U113] JS：正则替换全部
来源：http://ib.jctech888.com.cn

s.replaceAll("a", "b")
来源：http://gz.szxytkj.cn

[U114] JS：JSON 深比较
来源：http://oc.yuexingan06.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://cl.bjjhwx.cn

[U115] JS：生成 UUID
来源：http://jz.haigaiapp.cn

crypto.randomUUID()
来源：http://jy.szxytkj.cn

[U116] JS：类型检查（JSDoc）
来源：http://wz.gzmigu.cn

/** @param {string} name */ function f(name) {}
来源：http://pz.jianghongdianzi.cn

[U117] JS：单元测试
来源：http://yo.jianghongdianzi.cn

npm i -D vitest;  npx vitest
来源：http://yq.newstarts.cn

[U118] JS：开发服务器
来源：http://pn.gzmigu.cn

npm i -D vite;  npx vite
来源：http://os.yuexingan06.cn


<!-- 参考信息 -->