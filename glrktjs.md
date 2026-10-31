代发 wailian999

[T37] Lua：字符串拼接
来源：http://vg.huanxung.cn

"a" .. "b"
来源：http://mq.panjiajie.cn

[T38] Lua：条件
来源：http://ty.9csxet.cn

if x > 0 then print("正") end
来源：http://nm.huanxung.cn

[T39] Lua：模式匹配
来源：http://bn.bjjhwx.cn

string.find(s, "%d+")
来源：http://zd.szsharing.cn

[T40] Lua：元表
来源：http://gc.yuntaijiaju.cn

setmetatable({}, { __index = base })
来源：http://tl.9csxet.cn

[T41] Perl：Hello World
来源：http://xc.nszjky.cn

print "Hello\n";
来源：http://af.szxytkj.cn

[T42] Perl：变量类型
来源：http://tb.bookmarksfly.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ct.panjiajie.cn

[T43] Perl：字符串插值
来源：http://di.lnxyls.cn

"值: $a"
来源：http://jn.szsharing.cn

[T44] Perl：条件
来源：http://lq.huixinmuqiang.cn

if ($a > 0) { print "正"; }
来源：http://xy.yuexingan06.cn

[T45] Perl：数组遍历
来源：http://hw.yuexingan06.cn

for my $x (@arr) { print $x; }
来源：http://vo.chemitech.net.cn

[T46] Perl：哈希操作
来源：http://xj.yuexingan06.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kp.chemitech.net.cn

[T47] Perl：正则捕获
来源：http://wq.asd995.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://yv.szxytkj.cn

[T48] Perl：正则替换
来源：http://us.yuntaijiaju.cn

$s =~ s/old/new/g;
来源：http://kq.nszjky.cn

[T49] Perl：函数
来源：http://vb.jianghongdianzi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wp.huanxung.cn

[T50] Perl：逐行读文件
来源：http://lw.shxzskj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://mk.jianghongdianzi.cn

while (my $line = <$fh>) { print $line; }
来源：http://sa.huanxung.cn

[T51] Scala：Hello World
来源：http://ay.hahajie.cn

println("Hello")
来源：http://ts.nszjky.cn

[T52] Scala：变量
来源：http://gx.9csxet.cn

val a = 1;  var b = 2
来源：http://xk.jianghongdianzi.cn

[T53] Scala：字符串插值
来源：http://bq.bookmarksfly.cn

s"值: $b"
来源：http://xn.jianghongdianzi.cn

[T54] Scala：集合映射
来源：http://hu.muxihuayi.cn

List(1, 2, 3).map(_ * 2)
来源：http://qs.szxytkj.cn

[T55] Scala：集合过滤
来源：http://qb.521024.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wi.hnjuh.cn

[T56] Scala：样例类
来源：http://mt.bjjhwx.cn

case class User(name: String, age: Int)
来源：http://hz.shxzukj.cn

[T57] Scala：模式匹配
来源：http://by.yuntaijiaju.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fr.shtwfgs.cn

[T58] Scala：函数定义
来源：http://hl.jianghongdianzi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ou.hahajie.cn

[T59] Scala：循环
来源：http://yh.shxzukj.cn

for (i <- 1 to 10) println(i)
来源：http://bl.bookmarksfly.cn

[T60] Scala：折叠
来源：http://ie.bookmarksfly.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fg.nicolike.cn

================================================================================
来源：http://al.huixiangedu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qv.muxihuayi.cn

================================================================================
来源：http://nr.bjjhwx.cn

[U01] Py：创建虚拟环境
来源：http://zw.nicolike.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bj.nicolike.cn

[U02] Py：导出 / 安装依赖
来源：http://aj.jctech888.com.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fz.nszjky.cn

[U03] Py：加载 .env 配置
来源：http://of.asd995.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://nd.521024.cn

[U04] Py：变量调试打印
来源：http://nr.bookmarksfly.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ms.9csxet.cn

[U05] Py：列表去重且保序
来源：http://on.hahajie.cn

list(dict.fromkeys(arr))
来源：http://rp.chemitech.net.cn

[U06] Py：合并两个字典
来源：http://ym.yuexingan06.cn

{**a, **b}
来源：http://tj.huixiangedu.cn

[U07] Py：反转字典键值
来源：http://yd.szsharing.cn

{v: k for k, v in d.items()}
来源：http://my.colortex.cn

[U08] Py：展平二维列表
来源：http://sc.shtwfgs.cn

[y for x in nested for y in x]
来源：http://xp.panjiajie.cn

[U09] Py：字典取最大值的键
来源：http://gd.huixinmuqiang.cn

max(d, key=d.get)
来源：http://sz.nszjky.cn

[U10] Py：按值排序字典
来源：http://lv.newstarts.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qm.szxytkj.cn

[U11] Py：生成器表达式
来源：http://iy.hahajie.cn

(x * 2 for x in arr)
来源：http://xf.shtwfgs.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mx.lnxyls.cn

Counter(arr).most_common(3)
来源：http://nf.521024.cn

[U13] Py：固定长度队列
来源：http://eh.bjjhwx.cn

deque(maxlen=10)
来源：http://af.jianghongdianzi.cn

[U14] Py：分组收集到列表
来源：http://ws.muxihuayi.cn

defaultdict(list)
来源：http://pz.nszjky.cn

[U15] Py：高精度计时
来源：http://gs.shtwfgs.cn

t = time.perf_counter()
来源：http://ou.newstarts.cn

[U16] Py：命令行参数解析
来源：http://tr.jctech888.com.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://at.jctech888.com.cn

[U17] Py：初始化日志
来源：http://po.nicolike.cn

logging.basicConfig(level=logging.INFO)
来源：http://st.wgjwhj.cn

[U18] Py：预编译正则
来源：http://bh.jctech888.com.cn

pat = re.compile(r"\d+")
来源：http://qw.chemitech.net.cn

[U19] Py：正则替换带回调
来源：http://ry.lnxyls.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://te.shxzukj.cn

[U20] Py：缓存函数结果
来源：http://tl.szsharing.cn

@functools.lru_cache(maxsize=None)
来源：http://zy.huanxung.cn

[U21] Py：自定义上下文管理器
来源：http://tc.lnxyls.cn

@contextlib.contextmanager
来源：http://mg.hnjuh.cn

[U22] Py：矩阵转置
来源：http://am.huixiangedu.cn

list(zip(*m))
来源：http://ef.jianghongdianzi.cn

[U23] Py：分块读取大文件
来源：http://dv.chemitech.net.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yr.9csxet.cn

[U24] Py：路径操作
来源：http://uq.shtwfgs.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zy.huanxung.cn

[U25] Py：CSV 按字典读
来源：http://kd.jctech888.com.cn

csv.DictReader(f)
来源：http://pv.bjjhwx.cn

[U26] Py：并发下载
来源：http://iy.shtwfgs.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ha.panjiajie.cn

[U27] Py：异步 HTTP
来源：http://qy.521024.cn

aiohttp.ClientSession() 配合 async with
来源：http://lc.9csxet.cn

[U28] Py：类型别名
来源：http://ii.yuexingan06.cn

UserId = int
来源：http://dd.chemitech.net.cn

[U29] Py：属性校验
来源：http://wl.muxihuayi.cn

@property 与 @x.setter 配合
来源：http://pg.huixinmuqiang.cn

[U30] Py：数据类
来源：http://kb.521024.cn

@dataclass(slots=True)
来源：http://th.muxihuayi.cn

[U31] Py：单测
来源：http://se.panjiajie.cn

python -m pytest -q
来源：http://gu.9csxet.cn

[U32] Py：代码格式化
来源：http://vj.colortex.cn

ruff format . && ruff check --fix .
来源：http://wb.shxzskj.cn

[U33] Py：打包发布
来源：http://dw.9csxet.cn

python -m build  （依赖 pyproject.toml）
来源：http://ky.521024.cn

[U34] Py：判断编码
来源：http://st.huixiangedu.cn

chardet.detect(raw)
来源：http://mc.521024.cn

[U35] Py：发送邮件
来源：http://qb.szxytkj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wh.huanxung.cn

[U36] Py：定时任务
来源：http://nv.szxytkj.cn

schedule.every(10).minutes.do(job)
来源：http://qt.bookmarksfly.cn

[U37] Py：读写 Excel
来源：http://yl.yuntaijiaju.cn

pandas.read_excel / DataFrame.to_excel
来源：http://fe.shxzskj.cn

[U38] Py：获取脚本所在目录
来源：http://tt.szxytkj.cn

Path(__file__).resolve().parent
来源：http://bf.bookmarksfly.cn

[U39] Py：判断是否在交互环境
来源：http://fc.bjjhwx.cn

sys.stdout.isatty()
来源：http://ek.nszjky.cn

[U40] Py：打印到标准错误
来源：http://om.bjjhwx.cn

print("err", file=sys.stderr)
来源：http://qw.hnjuh.cn

[U41] PHP：初始化 Composer 项目
来源：http://mq.szxytkj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://mt.panjiajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://sd.hahajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lb.newstarts.cn

[U43] PHP：声明命名空间
来源：http://vy.gzmigu.cn

namespace App\Http;
来源：http://qu.nszjky.cn

[U44] PHP：开启严格类型
来源：http://sd.yuntaijiaju.cn

declare(strict_types=1);
来源：http://vi.nicolike.cn

[U45] PHP：类型声明与返回类型
来源：http://be.shxzukj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bn.shxzskj.cn

[U46] PHP：可空类型
来源：http://ob.panjiajie.cn

?string $name = null
来源：http://cg.haigaiapp.cn

[U47] PHP：联合类型
来源：http://lq.bjjhwx.cn

int|string $id
来源：http://uv.muxihuayi.cn

[U48] PHP：纯枚举
来源：http://jo.shtwfgs.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nf.hahajie.cn

[U49] PHP：只读属性
来源：http://ou.huixiangedu.cn

public readonly string $name
来源：http://hu.chemitech.net.cn

[U50] PHP：构造器属性提升
来源：http://xd.szsharing.cn

public function __construct(private int $id) {}
来源：http://ns.huanxung.cn

[U51] PHP：数组解构
来源：http://er.huanxung.cn

[$a, $b] = $arr;
来源：http://dq.521024.cn

[U52] PHP：箭头函数
来源：http://rn.haigaiapp.cn

$double = fn($x) => $x * 2;
来源：http://pu.bjjhwx.cn

[U53] PHP：空合并运算符
来源：http://tp.gzmigu.cn

$v = $a ?? $b ?? "default";
来源：http://kr.asd995.cn

[U54] PHP：空安全调用
来源：http://ou.yuexingan06.cn

$obj?->method()
来源：http://ss.521024.cn

[U55] PHP：match 表达式
来源：http://cc.shtwfgs.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xx.bookmarksfly.cn

[U56] PHP：命名参数
来源：http://fk.shxzskj.cn

f(a: 1, b: 2)
来源：http://pv.nicolike.cn

[U57] PHP：字符串插值
来源：http://fj.lnxyls.cn

"值: {$a}"
来源：http://ro.521024.cn

[U58] PHP：数组三件套
来源：http://zc.jianghongdianzi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://od.shxzskj.cn

[U59] PHP：自定义排序
来源：http://vi.newstarts.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qy.nszjky.cn

[U60] PHP：JSON 编解码
来源：http://pj.haigaiapp.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wv.nicolike.cn

[U61] PHP：正则
来源：http://px.chemitech.net.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wc.haigaiapp.cn

[U62] PHP：日期对象
来源：http://ip.huanxung.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rq.asd995.cn

[U63] PHP：文件读写
来源：http://kq.hnjuh.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://au.huanxung.cn

[U64] PHP：目录遍历
来源：http://up.wgjwhj.cn

glob("dir/*.php");  scandir("dir");
来源：http://dx.colortex.cn

[U65] PHP：会话
来源：http://gt.newstarts.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://dg.szxytkj.cn

[U66] PHP：设置 Cookie
来源：http://bo.yuntaijiaju.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rl.yuntaijiaju.cn

[U67] PHP：处理文件上传
来源：http://vg.haigaiapp.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mi.huanxung.cn

[U68] PHP：PDO 连接
来源：http://gb.asd995.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ef.lnxyls.cn

[U69] PHP：PDO 预处理
来源：http://wp.hahajie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://df.shxzskj.cn

[U70] PHP：PDO 事务
来源：http://vz.huanxung.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hi.newstarts.cn

[U71] PHP：抛出异常
来源：http://ra.muxihuayi.cn

throw new RuntimeException("失败", 500);
来源：http://ft.newstarts.cn

[U72] PHP：写错误日志
来源：http://bu.jctech888.com.cn

error_log("失败: " . $e->getMessage());
来源：http://gz.jianghongdianzi.cn

[U73] PHP：读取 ini 配置
来源：http://hf.jianghongdianzi.cn

parse_ini_file("config.ini", true)
来源：http://mz.huanxung.cn

[U74] PHP：读取环境变量
来源：http://sd.hahajie.cn

getenv("APP_ENV") ?: "production"
来源：http://kx.nszjky.cn

[U75] PHP：依赖注入
来源：http://qk.hahajie.cn

composer require psr/container
来源：http://ky.haigaiapp.cn

[U76] PHP：简单路由
来源：http://tq.nszjky.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hh.huanxung.cn

[U77] PHP：模板渲染
来源：http://np.nszjky.cn

composer require twig/twig
来源：http://gs.jctech888.com.cn

[U78] PHP：单元测试
来源：http://nb.shxzukj.cn

composer require --dev phpunit/phpunit
来源：http://af.hahajie.cn

[U79] PHP：静态分析
来源：http://dj.hahajie.cn

composer require --dev phpstan/phpstan
来源：http://ko.huixinmuqiang.cn

[U80] PHP：代码规范修复
来源：http://hk.huixiangedu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://un.hnjuh.cn

[U81] JS：初始化项目
来源：http://lg.haigaiapp.cn

npm init -y;  npm i express
来源：http://lb.521024.cn

[U82] JS：package.json 脚本
来源：http://lw.panjiajie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cz.szsharing.cn

[U83] JS：ES Module 导入导出
来源：http://vv.colortex.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xx.hnjuh.cn

[U84] JS：CommonJS 写法
来源：http://yo.haigaiapp.cn

module.exports = { a };  const { a } = require("./m");
来源：http://pj.jctech888.com.cn

[U85] JS：可选链
来源：http://vb.chemitech.net.cn

a?.b?.c
来源：http://td.bookmarksfly.cn

[U86] JS：空值合并
来源：http://va.521024.cn

a ?? b
来源：http://xe.chemitech.net.cn

[U87] JS：解构默认值
来源：http://pn.yuntaijiaju.cn

const { a = 1, b = 2 } = obj;
来源：http://sz.shxzskj.cn

[U88] JS：对象展开合并
来源：http://jz.jctech888.com.cn

{ ...a, ...b }
来源：http://qy.newstarts.cn

[U89] JS：数组去重
来源：http://eg.muxihuayi.cn

[...new Set(arr)]
来源：http://lo.521024.cn

[U90] JS：数字数组排序
来源：http://so.jianghongdianzi.cn

[...arr].sort((a, b) => a - b)
来源：http://ct.yuexingan06.cn

[U91] JS：对象键值遍历
来源：http://xl.chemitech.net.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://en.asd995.cn

[U92] JS：深拷贝
来源：http://jf.huanxung.cn

structuredClone(obj)
来源：http://tu.haigaiapp.cn

[U93] JS：模板字符串
来源：http://sn.yuexingan06.cn

`共 ${n} 条`
来源：http://kc.szsharing.cn

[U94] JS：箭头函数
来源：http://nl.haigaiapp.cn

const double = x => x * 2;
来源：http://xy.hnjuh.cn

[U95] JS：Promise 包装
来源：http://yv.9csxet.cn

new Promise((resolve, reject) => {})
来源：http://sv.huanxung.cn

[U96] JS：async/await 与异常
来源：http://rf.bjjhwx.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vc.newstarts.cn

[U97] JS：并发请求
来源：http://hd.hahajie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://to.hnjuh.cn

[U98] JS：fetch 带 JSON
来源：http://eq.haigaiapp.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://im.huanxung.cn

[U99] JS：事件监听
来源：http://cd.newstarts.cn

el.addEventListener("click", e => {})
来源：http://xv.huanxung.cn

[U100] JS：DOM 查询
来源：http://zl.colortex.cn

document.querySelector(".item")
来源：http://zm.wgjwhj.cn

[U101] JS：classList 操作
来源：http://ab.9csxet.cn

el.classList.toggle("active")
来源：http://rc.shxzukj.cn

[U102] JS：本地存储
来源：http://iv.panjiajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://pm.huixinmuqiang.cn

[U103] JS：定时器
来源：http://ol.bookmarksfly.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://er.521024.cn

[U104] JS：防抖
来源：http://nm.muxihuayi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rr.gzmigu.cn

[U105] JS：节流
来源：http://ck.szxytkj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qu.huixinmuqiang.cn

[U106] JS：日期格式化
来源：http://mf.yuntaijiaju.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://aa.nicolike.cn

[U107] JS：数字千分位
来源：http://lz.yuntaijiaju.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ni.hahajie.cn

[U108] JS：随机整数
来源：http://hl.lnxyls.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ro.muxihuayi.cn

[U109] JS：数组分组
来源：http://pb.haigaiapp.cn

Object.groupBy(arr, x => x.type)
来源：http://up.huixinmuqiang.cn

[U110] JS：数组分块
来源：http://ir.yuntaijiaju.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mv.wgjwhj.cn

[U111] JS：对象转 Map
来源：http://vi.nszjky.cn

new Map(Object.entries(obj))
来源：http://gx.szxytkj.cn

[U112] JS：字符串补位
来源：http://nz.nicolike.cn

"7".padStart(3, "0")
来源：http://ja.bookmarksfly.cn

[U113] JS：正则替换全部
来源：http://zl.asd995.cn

s.replaceAll("a", "b")
来源：http://vi.bjjhwx.cn

[U114] JS：JSON 深比较
来源：http://vf.bookmarksfly.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vr.chemitech.net.cn

[U115] JS：生成 UUID
来源：http://vx.bookmarksfly.cn

crypto.randomUUID()
来源：http://it.huixiangedu.cn

[U116] JS：类型检查（JSDoc）
来源：http://ae.shtwfgs.cn

/** @param {string} name */ function f(name) {}
来源：http://ih.jianghongdianzi.cn

[U117] JS：单元测试
来源：http://pb.wgjwhj.cn

npm i -D vitest;  npx vitest
来源：http://wc.panjiajie.cn

[U118] JS：开发服务器
来源：http://na.jctech888.com.cn

npm i -D vite;  npx vite
来源：http://hb.hahajie.cn

[U119] JS：生产构建
来源：http://wb.huixinmuqiang.cn

npx vite build
来源：http://wy.9csxet.cn

[U120] JS：读取环境变量（Vite）
来源：http://eg.jianghongdianzi.cn

import.meta.env.VITE_API_URL
来源：http://fc.szsharing.cn

================================================================================
来源：http://pp.shtwfgs.cn

统计汇总
来源：http://fl.wgjwhj.cn

================================================================================
来源：http://tt.hnjuh.cn

按语言统计（条）：
来源：http://kw.bookmarksfly.cn

Python ......... 252
来源：http://ib.newstarts.cn

PHP ............ 252
来源：http://xv.521024.cn

JavaScript ..... 252
来源：http://fe.gzmigu.cn

TypeScript ..... 212
来源：http://qw.yuexingan06.cn


<!-- 参考信息 -->