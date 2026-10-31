代发 wailian999

[T29] Swift：guard 提前返回
来源：http://fd.shxzukj.cn

guard let x = opt else { return }
来源：http://ov.shxzskj.cn

[T30] Swift：协议
来源：http://kt.shxzukj.cn

protocol Shape { func area() -> Double }
来源：http://pf.shxzskj.cn

[T31] Lua：Hello World
来源：http://ra.yuexingan06.cn

print("Hello")
来源：http://yg.bjjhwx.cn

[T32] Lua：局部变量
来源：http://fn.jctech888.com.cn

local a = 1
来源：http://po.huixinmuqiang.cn

[T33] Lua：表（数组）
来源：http://kn.wgjwhj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hq.9csxet.cn

[T34] Lua：遍历表
来源：http://mq.szsharing.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qj.newstarts.cn

[T35] Lua：字典表
来源：http://ng.hahajie.cn

local d = { a = 1 };  d.b = 2
来源：http://fr.panjiajie.cn

[T36] Lua：函数
来源：http://pg.newstarts.cn

function add(a, b) return a + b end
来源：http://xx.shxzukj.cn

[T37] Lua：字符串拼接
来源：http://nq.asd995.cn

"a" .. "b"
来源：http://wv.yuntaijiaju.cn

[T38] Lua：条件
来源：http://zl.colortex.cn

if x > 0 then print("正") end
来源：http://fs.lnxyls.cn

[T39] Lua：模式匹配
来源：http://ho.521024.cn

string.find(s, "%d+")
来源：http://yx.hahajie.cn

[T40] Lua：元表
来源：http://jp.shtwfgs.cn

setmetatable({}, { __index = base })
来源：http://xv.newstarts.cn

[T41] Perl：Hello World
来源：http://zd.szsharing.cn

print "Hello\n";
来源：http://ma.szxytkj.cn

[T42] Perl：变量类型
来源：http://pa.panjiajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bc.lnxyls.cn

[T43] Perl：字符串插值
来源：http://ip.haigaiapp.cn

"值: $a"
来源：http://of.asd995.cn

[T44] Perl：条件
来源：http://jd.asd995.cn

if ($a > 0) { print "正"; }
来源：http://yq.muxihuayi.cn

[T45] Perl：数组遍历
来源：http://cf.huixiangedu.cn

for my $x (@arr) { print $x; }
来源：http://fp.newstarts.cn

[T46] Perl：哈希操作
来源：http://oj.wgjwhj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mz.lnxyls.cn

[T47] Perl：正则捕获
来源：http://da.nicolike.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://nl.yuexingan06.cn

[T48] Perl：正则替换
来源：http://tu.yuntaijiaju.cn

$s =~ s/old/new/g;
来源：http://dw.colortex.cn

[T49] Perl：函数
来源：http://aq.shxzskj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ey.szsharing.cn

[T50] Perl：逐行读文件
来源：http://uw.huixinmuqiang.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://kz.szxytkj.cn

while (my $line = <$fh>) { print $line; }
来源：http://ce.haigaiapp.cn

[T51] Scala：Hello World
来源：http://ja.panjiajie.cn

println("Hello")
来源：http://tm.huixinmuqiang.cn

[T52] Scala：变量
来源：http://ko.chemitech.net.cn

val a = 1;  var b = 2
来源：http://sj.hahajie.cn

[T53] Scala：字符串插值
来源：http://pi.haigaiapp.cn

s"值: $b"
来源：http://yg.szsharing.cn

[T54] Scala：集合映射
来源：http://vi.panjiajie.cn

List(1, 2, 3).map(_ * 2)
来源：http://oh.9csxet.cn

[T55] Scala：集合过滤
来源：http://gv.yuexingan06.cn

List(1, 2, 3).filter(_ > 1)
来源：http://sz.szsharing.cn

[T56] Scala：样例类
来源：http://le.panjiajie.cn

case class User(name: String, age: Int)
来源：http://lx.bookmarksfly.cn

[T57] Scala：模式匹配
来源：http://pb.colortex.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://of.colortex.cn

[T58] Scala：函数定义
来源：http://oa.jctech888.com.cn

def add(a: Int, b: Int): Int = a + b
来源：http://aq.huixinmuqiang.cn

[T59] Scala：循环
来源：http://qy.bjjhwx.cn

for (i <- 1 to 10) println(i)
来源：http://rg.jctech888.com.cn

[T60] Scala：折叠
来源：http://vl.panjiajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ih.9csxet.cn

================================================================================
来源：http://dm.shtwfgs.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ap.shxzukj.cn

================================================================================
来源：http://zr.shtwfgs.cn

[U01] Py：创建虚拟环境
来源：http://lg.hahajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zm.jianghongdianzi.cn

[U02] Py：导出 / 安装依赖
来源：http://rs.9csxet.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://im.colortex.cn

[U03] Py：加载 .env 配置
来源：http://ul.jctech888.com.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://uu.haigaiapp.cn

[U04] Py：变量调试打印
来源：http://hb.nicolike.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vj.nicolike.cn

[U05] Py：列表去重且保序
来源：http://ud.yuexingan06.cn

list(dict.fromkeys(arr))
来源：http://wy.huixinmuqiang.cn

[U06] Py：合并两个字典
来源：http://qq.521024.cn

{**a, **b}
来源：http://ks.shxzskj.cn

[U07] Py：反转字典键值
来源：http://nm.521024.cn

{v: k for k, v in d.items()}
来源：http://ra.521024.cn

[U08] Py：展平二维列表
来源：http://tj.yuexingan06.cn

[y for x in nested for y in x]
来源：http://io.bjjhwx.cn

[U09] Py：字典取最大值的键
来源：http://mc.shxzskj.cn

max(d, key=d.get)
来源：http://eh.hnjuh.cn

[U10] Py：按值排序字典
来源：http://ba.nicolike.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gg.newstarts.cn

[U11] Py：生成器表达式
来源：http://pn.hahajie.cn

(x * 2 for x in arr)
来源：http://li.chemitech.net.cn

[U12] Py：取出现最多的 3 个元素
来源：http://im.huixiangedu.cn

Counter(arr).most_common(3)
来源：http://yr.shxzskj.cn

[U13] Py：固定长度队列
来源：http://uz.yuexingan06.cn

deque(maxlen=10)
来源：http://rq.nicolike.cn

[U14] Py：分组收集到列表
来源：http://yb.jianghongdianzi.cn

defaultdict(list)
来源：http://qu.gzmigu.cn

[U15] Py：高精度计时
来源：http://gx.shxzukj.cn

t = time.perf_counter()
来源：http://lw.huixinmuqiang.cn

[U16] Py：命令行参数解析
来源：http://iq.muxihuayi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zk.521024.cn

[U17] Py：初始化日志
来源：http://iy.chemitech.net.cn

logging.basicConfig(level=logging.INFO)
来源：http://bn.hnjuh.cn

[U18] Py：预编译正则
来源：http://wh.lnxyls.cn

pat = re.compile(r"\d+")
来源：http://ij.szsharing.cn

[U19] Py：正则替换带回调
来源：http://ki.huixinmuqiang.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fm.lnxyls.cn

[U20] Py：缓存函数结果
来源：http://cv.nicolike.cn

@functools.lru_cache(maxsize=None)
来源：http://ev.haigaiapp.cn

[U21] Py：自定义上下文管理器
来源：http://kd.huanxung.cn

@contextlib.contextmanager
来源：http://zp.panjiajie.cn

[U22] Py：矩阵转置
来源：http://cc.jctech888.com.cn

list(zip(*m))
来源：http://zn.9csxet.cn

[U23] Py：分块读取大文件
来源：http://op.huixinmuqiang.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://im.haigaiapp.cn

[U24] Py：路径操作
来源：http://zk.huixinmuqiang.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bu.yuntaijiaju.cn

[U25] Py：CSV 按字典读
来源：http://ex.jctech888.com.cn

csv.DictReader(f)
来源：http://so.nszjky.cn

[U26] Py：并发下载
来源：http://us.9csxet.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jv.shxzukj.cn

[U27] Py：异步 HTTP
来源：http://ft.huixinmuqiang.cn

aiohttp.ClientSession() 配合 async with
来源：http://qy.newstarts.cn

[U28] Py：类型别名
来源：http://oi.yuntaijiaju.cn

UserId = int
来源：http://en.nszjky.cn

[U29] Py：属性校验
来源：http://lg.hahajie.cn

@property 与 @x.setter 配合
来源：http://is.muxihuayi.cn

[U30] Py：数据类
来源：http://bg.nicolike.cn

@dataclass(slots=True)
来源：http://zv.huixinmuqiang.cn

[U31] Py：单测
来源：http://rc.yuexingan06.cn

python -m pytest -q
来源：http://rp.huixinmuqiang.cn

[U32] Py：代码格式化
来源：http://dk.shxzukj.cn

ruff format . && ruff check --fix .
来源：http://uj.shtwfgs.cn

[U33] Py：打包发布
来源：http://cj.colortex.cn

python -m build  （依赖 pyproject.toml）
来源：http://xf.yuntaijiaju.cn

[U34] Py：判断编码
来源：http://ia.hahajie.cn

chardet.detect(raw)
来源：http://gp.nicolike.cn

[U35] Py：发送邮件
来源：http://mx.lnxyls.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vr.bookmarksfly.cn

[U36] Py：定时任务
来源：http://vf.newstarts.cn

schedule.every(10).minutes.do(job)
来源：http://xg.newstarts.cn

[U37] Py：读写 Excel
来源：http://sh.nszjky.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ig.asd995.cn

[U38] Py：获取脚本所在目录
来源：http://fv.huanxung.cn

Path(__file__).resolve().parent
来源：http://ia.haigaiapp.cn

[U39] Py：判断是否在交互环境
来源：http://gb.nicolike.cn

sys.stdout.isatty()
来源：http://ce.9csxet.cn

[U40] Py：打印到标准错误
来源：http://dg.yuntaijiaju.cn

print("err", file=sys.stderr)
来源：http://du.haigaiapp.cn

[U41] PHP：初始化 Composer 项目
来源：http://rf.gzmigu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gj.gzmigu.cn

[U42] PHP：PSR-4 自动加载
来源：http://my.hahajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rl.9csxet.cn

[U43] PHP：声明命名空间
来源：http://np.nicolike.cn

namespace App\Http;
来源：http://un.wgjwhj.cn

[U44] PHP：开启严格类型
来源：http://aa.newstarts.cn

declare(strict_types=1);
来源：http://oe.nszjky.cn

[U45] PHP：类型声明与返回类型
来源：http://qx.muxihuayi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ty.hahajie.cn

[U46] PHP：可空类型
来源：http://st.hahajie.cn

?string $name = null
来源：http://ht.jctech888.com.cn

[U47] PHP：联合类型
来源：http://uo.chemitech.net.cn

int|string $id
来源：http://vr.panjiajie.cn

[U48] PHP：纯枚举
来源：http://dt.9csxet.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://iy.colortex.cn

[U49] PHP：只读属性
来源：http://rv.yuexingan06.cn

public readonly string $name
来源：http://ii.huanxung.cn

[U50] PHP：构造器属性提升
来源：http://pt.hahajie.cn

public function __construct(private int $id) {}
来源：http://ts.bookmarksfly.cn

[U51] PHP：数组解构
来源：http://qi.haigaiapp.cn

[$a, $b] = $arr;
来源：http://xj.newstarts.cn

[U52] PHP：箭头函数
来源：http://sv.huixinmuqiang.cn

$double = fn($x) => $x * 2;
来源：http://hg.yuexingan06.cn

[U53] PHP：空合并运算符
来源：http://cb.bookmarksfly.cn

$v = $a ?? $b ?? "default";
来源：http://dc.9csxet.cn

[U54] PHP：空安全调用
来源：http://be.szxytkj.cn

$obj?->method()
来源：http://ny.yuexingan06.cn

[U55] PHP：match 表达式
来源：http://rs.9csxet.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gi.panjiajie.cn

[U56] PHP：命名参数
来源：http://xl.huixinmuqiang.cn

f(a: 1, b: 2)
来源：http://dk.hnjuh.cn

[U57] PHP：字符串插值
来源：http://fr.yuexingan06.cn

"值: {$a}"
来源：http://ic.colortex.cn

[U58] PHP：数组三件套
来源：http://pi.shxzukj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fc.jianghongdianzi.cn

[U59] PHP：自定义排序
来源：http://ba.szxytkj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://el.hahajie.cn

[U60] PHP：JSON 编解码
来源：http://iw.yuexingan06.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pm.nicolike.cn

[U61] PHP：正则
来源：http://jk.jctech888.com.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://an.hahajie.cn

[U62] PHP：日期对象
来源：http://fj.nszjky.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://di.yuexingan06.cn

[U63] PHP：文件读写
来源：http://mj.panjiajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zl.yuntaijiaju.cn

[U64] PHP：目录遍历
来源：http://fp.haigaiapp.cn

glob("dir/*.php");  scandir("dir");
来源：http://cl.nicolike.cn

[U65] PHP：会话
来源：http://sj.wgjwhj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ek.asd995.cn

[U66] PHP：设置 Cookie
来源：http://zr.yuexingan06.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ps.lnxyls.cn

[U67] PHP：处理文件上传
来源：http://jk.bookmarksfly.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xz.nicolike.cn

[U68] PHP：PDO 连接
来源：http://ya.gzmigu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xn.szsharing.cn

[U69] PHP：PDO 预处理
来源：http://wh.asd995.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kq.bjjhwx.cn

[U70] PHP：PDO 事务
来源：http://ut.9csxet.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fo.yuntaijiaju.cn

[U71] PHP：抛出异常
来源：http://fi.shtwfgs.cn

throw new RuntimeException("失败", 500);
来源：http://sw.colortex.cn

[U72] PHP：写错误日志
来源：http://bo.asd995.cn

error_log("失败: " . $e->getMessage());
来源：http://wu.yuexingan06.cn

[U73] PHP：读取 ini 配置
来源：http://vx.haigaiapp.cn

parse_ini_file("config.ini", true)
来源：http://zr.lnxyls.cn

[U74] PHP：读取环境变量
来源：http://qq.szsharing.cn

getenv("APP_ENV") ?: "production"
来源：http://hp.yuexingan06.cn

[U75] PHP：依赖注入
来源：http://ul.wgjwhj.cn

composer require psr/container
来源：http://lq.hahajie.cn

[U76] PHP：简单路由
来源：http://eg.szsharing.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bv.newstarts.cn

[U77] PHP：模板渲染
来源：http://rn.bjjhwx.cn

composer require twig/twig
来源：http://zp.bookmarksfly.cn

[U78] PHP：单元测试
来源：http://cq.shtwfgs.cn

composer require --dev phpunit/phpunit
来源：http://sw.newstarts.cn

[U79] PHP：静态分析
来源：http://en.bjjhwx.cn

composer require --dev phpstan/phpstan
来源：http://oh.panjiajie.cn

[U80] PHP：代码规范修复
来源：http://ge.wgjwhj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ai.szsharing.cn

[U81] JS：初始化项目
来源：http://ki.wgjwhj.cn

npm init -y;  npm i express
来源：http://or.shxzskj.cn

[U82] JS：package.json 脚本
来源：http://lk.chemitech.net.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ju.muxihuayi.cn

[U83] JS：ES Module 导入导出
来源：http://hj.bookmarksfly.cn

export const a = 1;  import { a } from "./m.js";
来源：http://lm.huixiangedu.cn

[U84] JS：CommonJS 写法
来源：http://kb.shtwfgs.cn

module.exports = { a };  const { a } = require("./m");
来源：http://iq.lnxyls.cn

[U85] JS：可选链
来源：http://kr.shxzukj.cn

a?.b?.c
来源：http://mq.chemitech.net.cn

[U86] JS：空值合并
来源：http://if.panjiajie.cn

a ?? b
来源：http://yh.asd995.cn

[U87] JS：解构默认值
来源：http://zq.9csxet.cn

const { a = 1, b = 2 } = obj;
来源：http://pc.nicolike.cn

[U88] JS：对象展开合并
来源：http://fy.newstarts.cn

{ ...a, ...b }
来源：http://yo.yuexingan06.cn

[U89] JS：数组去重
来源：http://rp.nszjky.cn

[...new Set(arr)]
来源：http://hs.yuexingan06.cn

[U90] JS：数字数组排序
来源：http://ak.hnjuh.cn

[...arr].sort((a, b) => a - b)
来源：http://in.nicolike.cn

[U91] JS：对象键值遍历
来源：http://ue.szsharing.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://uy.yuntaijiaju.cn

[U92] JS：深拷贝
来源：http://rr.jctech888.com.cn

structuredClone(obj)
来源：http://id.shxzukj.cn

[U93] JS：模板字符串
来源：http://rn.yuntaijiaju.cn

`共 ${n} 条`
来源：http://rh.newstarts.cn

[U94] JS：箭头函数
来源：http://gi.nszjky.cn

const double = x => x * 2;
来源：http://nn.bjjhwx.cn

[U95] JS：Promise 包装
来源：http://we.521024.cn

new Promise((resolve, reject) => {})
来源：http://ld.lnxyls.cn

[U96] JS：async/await 与异常
来源：http://qj.muxihuayi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pn.newstarts.cn

[U97] JS：并发请求
来源：http://dr.yuexingan06.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://xh.yuntaijiaju.cn

[U98] JS：fetch 带 JSON
来源：http://oc.haigaiapp.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tj.huanxung.cn

[U99] JS：事件监听
来源：http://nf.jianghongdianzi.cn

el.addEventListener("click", e => {})
来源：http://wr.huixinmuqiang.cn

[U100] JS：DOM 查询
来源：http://sg.szxytkj.cn

document.querySelector(".item")
来源：http://ho.521024.cn

[U101] JS：classList 操作
来源：http://pf.jctech888.com.cn

el.classList.toggle("active")
来源：http://dr.bookmarksfly.cn

[U102] JS：本地存储
来源：http://fl.bookmarksfly.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://bz.shxzskj.cn

[U103] JS：定时器
来源：http://wi.huixiangedu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hq.521024.cn

[U104] JS：防抖
来源：http://eu.huanxung.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gc.bjjhwx.cn

[U105] JS：节流
来源：http://sf.huixinmuqiang.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lz.jctech888.com.cn

[U106] JS：日期格式化
来源：http://gl.jctech888.com.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hp.asd995.cn

[U107] JS：数字千分位
来源：http://xh.shxzskj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zl.wgjwhj.cn

[U108] JS：随机整数
来源：http://ne.bookmarksfly.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gl.521024.cn

[U109] JS：数组分组
来源：http://vm.wgjwhj.cn

Object.groupBy(arr, x => x.type)
来源：http://vg.yuntaijiaju.cn

[U110] JS：数组分块
来源：http://gy.nszjky.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jz.521024.cn

[U111] JS：对象转 Map
来源：http://ws.nicolike.cn

new Map(Object.entries(obj))
来源：http://pe.jctech888.com.cn

[U112] JS：字符串补位
来源：http://us.muxihuayi.cn

"7".padStart(3, "0")
来源：http://ay.szxytkj.cn

[U113] JS：正则替换全部
来源：http://za.yuntaijiaju.cn

s.replaceAll("a", "b")
来源：http://hp.bookmarksfly.cn

[U114] JS：JSON 深比较
来源：http://qv.panjiajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://jl.shxzukj.cn

[U115] JS：生成 UUID
来源：http://ah.huixiangedu.cn

crypto.randomUUID()
来源：http://kz.haigaiapp.cn

[U116] JS：类型检查（JSDoc）
来源：http://pk.wgjwhj.cn

/** @param {string} name */ function f(name) {}
来源：http://fa.jctech888.com.cn


<!-- 参考信息 -->