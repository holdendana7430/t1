代发 wailian999

[T29] Swift：guard 提前返回
来源：http://wf.asd995.cn

guard let x = opt else { return }
来源：http://xz.asd995.cn

[T30] Swift：协议
来源：http://ef.nicolike.cn

protocol Shape { func area() -> Double }
来源：http://il.shxzukj.cn

[T31] Lua：Hello World
来源：http://os.wgjwhj.cn

print("Hello")
来源：http://uf.colortex.cn

[T32] Lua：局部变量
来源：http://jk.chemitech.net.cn

local a = 1
来源：http://ab.shtwfgs.cn

[T33] Lua：表（数组）
来源：http://yr.huanxung.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://qv.521024.cn

[T34] Lua：遍历表
来源：http://kl.shxzskj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://if.yuexingan06.cn

[T35] Lua：字典表
来源：http://tf.lnxyls.cn

local d = { a = 1 };  d.b = 2
来源：http://lq.shtwfgs.cn

[T36] Lua：函数
来源：http://ug.haigaiapp.cn

function add(a, b) return a + b end
来源：http://gt.bjjhwx.cn

[T37] Lua：字符串拼接
来源：http://zt.jianghongdianzi.cn

"a" .. "b"
来源：http://wz.haigaiapp.cn

[T38] Lua：条件
来源：http://yi.newstarts.cn

if x > 0 then print("正") end
来源：http://zy.muxihuayi.cn

[T39] Lua：模式匹配
来源：http://ce.chemitech.net.cn

string.find(s, "%d+")
来源：http://js.hnjuh.cn

[T40] Lua：元表
来源：http://go.bjjhwx.cn

setmetatable({}, { __index = base })
来源：http://ls.newstarts.cn

[T41] Perl：Hello World
来源：http://tl.521024.cn

print "Hello\n";
来源：http://qp.huanxung.cn

[T42] Perl：变量类型
来源：http://jz.newstarts.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://be.huixinmuqiang.cn

[T43] Perl：字符串插值
来源：http://pz.muxihuayi.cn

"值: $a"
来源：http://tf.521024.cn

[T44] Perl：条件
来源：http://wz.wgjwhj.cn

if ($a > 0) { print "正"; }
来源：http://on.lnxyls.cn

[T45] Perl：数组遍历
来源：http://nj.nszjky.cn

for my $x (@arr) { print $x; }
来源：http://dl.huixiangedu.cn

[T46] Perl：哈希操作
来源：http://uv.huixinmuqiang.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fd.yuexingan06.cn

[T47] Perl：正则捕获
来源：http://hn.jctech888.com.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://bx.panjiajie.cn

[T48] Perl：正则替换
来源：http://yq.muxihuayi.cn

$s =~ s/old/new/g;
来源：http://rb.panjiajie.cn

[T49] Perl：函数
来源：http://gk.521024.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lx.chemitech.net.cn

[T50] Perl：逐行读文件
来源：http://rt.haigaiapp.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://cf.lnxyls.cn

while (my $line = <$fh>) { print $line; }
来源：http://kf.jianghongdianzi.cn

[T51] Scala：Hello World
来源：http://qv.bjjhwx.cn

println("Hello")
来源：http://uv.shxzskj.cn

[T52] Scala：变量
来源：http://ve.bjjhwx.cn

val a = 1;  var b = 2
来源：http://eh.newstarts.cn

[T53] Scala：字符串插值
来源：http://pr.gzmigu.cn

s"值: $b"
来源：http://es.lnxyls.cn

[T54] Scala：集合映射
来源：http://mz.huixinmuqiang.cn

List(1, 2, 3).map(_ * 2)
来源：http://zi.panjiajie.cn

[T55] Scala：集合过滤
来源：http://uz.jctech888.com.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qc.521024.cn

[T56] Scala：样例类
来源：http://du.colortex.cn

case class User(name: String, age: Int)
来源：http://xd.wgjwhj.cn

[T57] Scala：模式匹配
来源：http://hl.asd995.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://pb.haigaiapp.cn

[T58] Scala：函数定义
来源：http://iw.nicolike.cn

def add(a: Int, b: Int): Int = a + b
来源：http://kh.newstarts.cn

[T59] Scala：循环
来源：http://qq.9csxet.cn

for (i <- 1 to 10) println(i)
来源：http://el.gzmigu.cn

[T60] Scala：折叠
来源：http://hb.asd995.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yi.shxzskj.cn

================================================================================
来源：http://sf.asd995.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fs.haigaiapp.cn

================================================================================
来源：http://nv.jianghongdianzi.cn

[U01] Py：创建虚拟环境
来源：http://ap.nicolike.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ol.521024.cn

[U02] Py：导出 / 安装依赖
来源：http://gy.shxzukj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zf.chemitech.net.cn

[U03] Py：加载 .env 配置
来源：http://nf.asd995.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://es.yuntaijiaju.cn

[U04] Py：变量调试打印
来源：http://wm.chemitech.net.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bw.asd995.cn

[U05] Py：列表去重且保序
来源：http://ds.hahajie.cn

list(dict.fromkeys(arr))
来源：http://as.huanxung.cn

[U06] Py：合并两个字典
来源：http://ga.lnxyls.cn

{**a, **b}
来源：http://th.jctech888.com.cn

[U07] Py：反转字典键值
来源：http://ua.hnjuh.cn

{v: k for k, v in d.items()}
来源：http://pu.521024.cn

[U08] Py：展平二维列表
来源：http://dk.9csxet.cn

[y for x in nested for y in x]
来源：http://pq.yuexingan06.cn

[U09] Py：字典取最大值的键
来源：http://wl.panjiajie.cn

max(d, key=d.get)
来源：http://to.bookmarksfly.cn

[U10] Py：按值排序字典
来源：http://yw.521024.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ws.huixiangedu.cn

[U11] Py：生成器表达式
来源：http://io.asd995.cn

(x * 2 for x in arr)
来源：http://df.newstarts.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ht.huixiangedu.cn

Counter(arr).most_common(3)
来源：http://tr.huixiangedu.cn

[U13] Py：固定长度队列
来源：http://cx.nicolike.cn

deque(maxlen=10)
来源：http://wq.gzmigu.cn

[U14] Py：分组收集到列表
来源：http://vx.jctech888.com.cn

defaultdict(list)
来源：http://jl.9csxet.cn

[U15] Py：高精度计时
来源：http://rt.gzmigu.cn

t = time.perf_counter()
来源：http://eu.9csxet.cn

[U16] Py：命令行参数解析
来源：http://cv.gzmigu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://co.nicolike.cn

[U17] Py：初始化日志
来源：http://yi.hahajie.cn

logging.basicConfig(level=logging.INFO)
来源：http://hf.jctech888.com.cn

[U18] Py：预编译正则
来源：http://uc.yuexingan06.cn

pat = re.compile(r"\d+")
来源：http://sm.shtwfgs.cn

[U19] Py：正则替换带回调
来源：http://ve.jianghongdianzi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ot.lnxyls.cn

[U20] Py：缓存函数结果
来源：http://ik.jctech888.com.cn

@functools.lru_cache(maxsize=None)
来源：http://kk.shxzskj.cn

[U21] Py：自定义上下文管理器
来源：http://ai.huanxung.cn

@contextlib.contextmanager
来源：http://kk.jianghongdianzi.cn

[U22] Py：矩阵转置
来源：http://hk.yuexingan06.cn

list(zip(*m))
来源：http://bc.521024.cn

[U23] Py：分块读取大文件
来源：http://rt.lnxyls.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jm.yuntaijiaju.cn

[U24] Py：路径操作
来源：http://ei.shxzskj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yp.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://wr.szsharing.cn

csv.DictReader(f)
来源：http://xz.huixiangedu.cn

[U26] Py：并发下载
来源：http://pc.shxzskj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ie.colortex.cn

[U27] Py：异步 HTTP
来源：http://rv.lnxyls.cn

aiohttp.ClientSession() 配合 async with
来源：http://vb.muxihuayi.cn

[U28] Py：类型别名
来源：http://pb.9csxet.cn

UserId = int
来源：http://xk.nszjky.cn

[U29] Py：属性校验
来源：http://wu.newstarts.cn

@property 与 @x.setter 配合
来源：http://kl.bjjhwx.cn

[U30] Py：数据类
来源：http://nm.huixinmuqiang.cn

@dataclass(slots=True)
来源：http://hn.chemitech.net.cn

[U31] Py：单测
来源：http://bb.bookmarksfly.cn

python -m pytest -q
来源：http://jw.huanxung.cn

[U32] Py：代码格式化
来源：http://gn.haigaiapp.cn

ruff format . && ruff check --fix .
来源：http://vj.yuexingan06.cn

[U33] Py：打包发布
来源：http://cz.panjiajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://wq.shtwfgs.cn

[U34] Py：判断编码
来源：http://lq.521024.cn

chardet.detect(raw)
来源：http://dz.shxzukj.cn

[U35] Py：发送邮件
来源：http://rc.521024.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dg.hahajie.cn

[U36] Py：定时任务
来源：http://hr.haigaiapp.cn

schedule.every(10).minutes.do(job)
来源：http://og.jctech888.com.cn

[U37] Py：读写 Excel
来源：http://mv.szxytkj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://hi.bookmarksfly.cn

[U38] Py：获取脚本所在目录
来源：http://ei.jianghongdianzi.cn

Path(__file__).resolve().parent
来源：http://ze.gzmigu.cn

[U39] Py：判断是否在交互环境
来源：http://xj.yuntaijiaju.cn

sys.stdout.isatty()
来源：http://zx.wgjwhj.cn

[U40] Py：打印到标准错误
来源：http://zt.yuexingan06.cn

print("err", file=sys.stderr)
来源：http://fv.newstarts.cn

[U41] PHP：初始化 Composer 项目
来源：http://qq.jctech888.com.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://hr.haigaiapp.cn

[U42] PHP：PSR-4 自动加载
来源：http://mp.shxzukj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zy.chemitech.net.cn

[U43] PHP：声明命名空间
来源：http://gw.newstarts.cn

namespace App\Http;
来源：http://ob.szsharing.cn

[U44] PHP：开启严格类型
来源：http://ta.bjjhwx.cn

declare(strict_types=1);
来源：http://aw.hahajie.cn

[U45] PHP：类型声明与返回类型
来源：http://wo.yuntaijiaju.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://al.nszjky.cn

[U46] PHP：可空类型
来源：http://sw.huixinmuqiang.cn

?string $name = null
来源：http://pg.yuntaijiaju.cn

[U47] PHP：联合类型
来源：http://nc.newstarts.cn

int|string $id
来源：http://sl.yuntaijiaju.cn

[U48] PHP：纯枚举
来源：http://ao.nicolike.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fd.newstarts.cn

[U49] PHP：只读属性
来源：http://zc.jctech888.com.cn

public readonly string $name
来源：http://ev.shxzskj.cn

[U50] PHP：构造器属性提升
来源：http://sf.hahajie.cn

public function __construct(private int $id) {}
来源：http://ls.huixiangedu.cn

[U51] PHP：数组解构
来源：http://nu.shxzukj.cn

[$a, $b] = $arr;
来源：http://sy.gzmigu.cn

[U52] PHP：箭头函数
来源：http://xx.hahajie.cn

$double = fn($x) => $x * 2;
来源：http://xf.lnxyls.cn

[U53] PHP：空合并运算符
来源：http://mi.wgjwhj.cn

$v = $a ?? $b ?? "default";
来源：http://xq.muxihuayi.cn

[U54] PHP：空安全调用
来源：http://ga.yuexingan06.cn

$obj?->method()
来源：http://sx.szxytkj.cn

[U55] PHP：match 表达式
来源：http://ss.hahajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pw.nszjky.cn

[U56] PHP：命名参数
来源：http://dt.asd995.cn

f(a: 1, b: 2)
来源：http://bf.hnjuh.cn

[U57] PHP：字符串插值
来源：http://lr.yuntaijiaju.cn

"值: {$a}"
来源：http://xu.bookmarksfly.cn

[U58] PHP：数组三件套
来源：http://kn.nszjky.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://aq.haigaiapp.cn

[U59] PHP：自定义排序
来源：http://vz.shxzukj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mw.colortex.cn

[U60] PHP：JSON 编解码
来源：http://lq.9csxet.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mc.colortex.cn

[U61] PHP：正则
来源：http://rl.bjjhwx.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ei.lnxyls.cn

[U62] PHP：日期对象
来源：http://fm.huixinmuqiang.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bx.chemitech.net.cn

[U63] PHP：文件读写
来源：http://ac.nszjky.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ux.bjjhwx.cn

[U64] PHP：目录遍历
来源：http://uj.chemitech.net.cn

glob("dir/*.php");  scandir("dir");
来源：http://dg.nicolike.cn

[U65] PHP：会话
来源：http://dq.nszjky.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://xp.bjjhwx.cn

[U66] PHP：设置 Cookie
来源：http://sx.521024.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kf.yuntaijiaju.cn

[U67] PHP：处理文件上传
来源：http://kt.asd995.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wc.szsharing.cn

[U68] PHP：PDO 连接
来源：http://rd.jianghongdianzi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rw.colortex.cn

[U69] PHP：PDO 预处理
来源：http://mw.yuexingan06.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://js.yuntaijiaju.cn

[U70] PHP：PDO 事务
来源：http://rj.huixinmuqiang.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zj.9csxet.cn

[U71] PHP：抛出异常
来源：http://wx.huixinmuqiang.cn

throw new RuntimeException("失败", 500);
来源：http://lc.nszjky.cn

[U72] PHP：写错误日志
来源：http://qo.shxzskj.cn

error_log("失败: " . $e->getMessage());
来源：http://jn.lnxyls.cn

[U73] PHP：读取 ini 配置
来源：http://jh.szsharing.cn

parse_ini_file("config.ini", true)
来源：http://bh.yuexingan06.cn

[U74] PHP：读取环境变量
来源：http://gd.chemitech.net.cn

getenv("APP_ENV") ?: "production"
来源：http://ti.shxzskj.cn

[U75] PHP：依赖注入
来源：http://pl.newstarts.cn

composer require psr/container
来源：http://zq.huanxung.cn

[U76] PHP：简单路由
来源：http://ga.szsharing.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ie.jctech888.com.cn

[U77] PHP：模板渲染
来源：http://kr.shxzskj.cn

composer require twig/twig
来源：http://mp.panjiajie.cn

[U78] PHP：单元测试
来源：http://hn.jianghongdianzi.cn

composer require --dev phpunit/phpunit
来源：http://lg.jianghongdianzi.cn

[U79] PHP：静态分析
来源：http://bw.hahajie.cn

composer require --dev phpstan/phpstan
来源：http://zd.huanxung.cn

[U80] PHP：代码规范修复
来源：http://mq.hnjuh.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://fd.yuexingan06.cn

[U81] JS：初始化项目
来源：http://tr.huanxung.cn

npm init -y;  npm i express
来源：http://sp.nicolike.cn

[U82] JS：package.json 脚本
来源：http://qy.shxzukj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ti.yuexingan06.cn

[U83] JS：ES Module 导入导出
来源：http://ea.yuntaijiaju.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ts.gzmigu.cn

[U84] JS：CommonJS 写法
来源：http://xu.huanxung.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wg.yuntaijiaju.cn

[U85] JS：可选链
来源：http://sx.lnxyls.cn

a?.b?.c
来源：http://by.huanxung.cn

[U86] JS：空值合并
来源：http://ik.haigaiapp.cn

a ?? b
来源：http://op.bjjhwx.cn

[U87] JS：解构默认值
来源：http://ja.szxytkj.cn

const { a = 1, b = 2 } = obj;
来源：http://bg.chemitech.net.cn

[U88] JS：对象展开合并
来源：http://go.asd995.cn

{ ...a, ...b }
来源：http://vn.yuexingan06.cn

[U89] JS：数组去重
来源：http://ds.panjiajie.cn

[...new Set(arr)]
来源：http://bz.newstarts.cn

[U90] JS：数字数组排序
来源：http://it.nicolike.cn

[...arr].sort((a, b) => a - b)
来源：http://tc.huixinmuqiang.cn

[U91] JS：对象键值遍历
来源：http://sm.haigaiapp.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dn.hahajie.cn

[U92] JS：深拷贝
来源：http://rl.hahajie.cn

structuredClone(obj)
来源：http://ej.newstarts.cn

[U93] JS：模板字符串
来源：http://xd.asd995.cn

`共 ${n} 条`
来源：http://zt.szsharing.cn

[U94] JS：箭头函数
来源：http://wt.521024.cn

const double = x => x * 2;
来源：http://fb.muxihuayi.cn

[U95] JS：Promise 包装
来源：http://cm.bookmarksfly.cn

new Promise((resolve, reject) => {})
来源：http://oi.jctech888.com.cn

[U96] JS：async/await 与异常
来源：http://gn.bjjhwx.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://oc.521024.cn

[U97] JS：并发请求
来源：http://cw.shxzskj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://to.jctech888.com.cn

[U98] JS：fetch 带 JSON
来源：http://fl.panjiajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ry.bookmarksfly.cn

[U99] JS：事件监听
来源：http://yw.bjjhwx.cn

el.addEventListener("click", e => {})
来源：http://zu.huixiangedu.cn

[U100] JS：DOM 查询
来源：http://my.wgjwhj.cn

document.querySelector(".item")
来源：http://ku.huanxung.cn

[U101] JS：classList 操作
来源：http://hn.szxytkj.cn

el.classList.toggle("active")
来源：http://xe.haigaiapp.cn

[U102] JS：本地存储
来源：http://dz.yuntaijiaju.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ku.asd995.cn

[U103] JS：定时器
来源：http://pp.shxzukj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ge.huixiangedu.cn

[U104] JS：防抖
来源：http://ec.asd995.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://os.colortex.cn

[U105] JS：节流
来源：http://kc.9csxet.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gu.huanxung.cn

[U106] JS：日期格式化
来源：http://rc.colortex.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lm.jianghongdianzi.cn

[U107] JS：数字千分位
来源：http://dd.nszjky.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ak.bookmarksfly.cn

[U108] JS：随机整数
来源：http://ma.yuntaijiaju.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://aj.gzmigu.cn

[U109] JS：数组分组
来源：http://sy.panjiajie.cn

Object.groupBy(arr, x => x.type)
来源：http://wl.lnxyls.cn

[U110] JS：数组分块
来源：http://ei.bjjhwx.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://db.shtwfgs.cn

[U111] JS：对象转 Map
来源：http://hq.huixiangedu.cn

new Map(Object.entries(obj))
来源：http://fc.chemitech.net.cn

[U112] JS：字符串补位
来源：http://gc.huixiangedu.cn

"7".padStart(3, "0")
来源：http://op.yuexingan06.cn

[U113] JS：正则替换全部
来源：http://ee.shtwfgs.cn

s.replaceAll("a", "b")
来源：http://sw.nicolike.cn

[U114] JS：JSON 深比较
来源：http://nr.colortex.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://gh.panjiajie.cn

[U115] JS：生成 UUID
来源：http://jw.nicolike.cn

crypto.randomUUID()
来源：http://ww.lnxyls.cn

[U116] JS：类型检查（JSDoc）
来源：http://xv.shtwfgs.cn

/** @param {string} name */ function f(name) {}
来源：http://bg.huanxung.cn


<!-- 参考信息 -->