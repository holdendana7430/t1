代发 wailian999

[T37] Lua：字符串拼接
来源：http://as.nszjky.cn

"a" .. "b"
来源：http://zs.haigaiapp.cn

[T38] Lua：条件
来源：http://oq.colortex.cn

if x > 0 then print("正") end
来源：http://gq.colortex.cn

[T39] Lua：模式匹配
来源：http://ei.jianghongdianzi.cn

string.find(s, "%d+")
来源：http://bf.huanxung.cn

[T40] Lua：元表
来源：http://jg.hnjuh.cn

setmetatable({}, { __index = base })
来源：http://em.muxihuayi.cn

[T41] Perl：Hello World
来源：http://dj.lnxyls.cn

print "Hello\n";
来源：http://cc.shtwfgs.cn

[T42] Perl：变量类型
来源：http://ot.huixiangedu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://im.shtwfgs.cn

[T43] Perl：字符串插值
来源：http://mc.asd995.cn

"值: $a"
来源：http://dg.yuexingan06.cn

[T44] Perl：条件
来源：http://oy.asd995.cn

if ($a > 0) { print "正"; }
来源：http://fk.9csxet.cn

[T45] Perl：数组遍历
来源：http://of.haigaiapp.cn

for my $x (@arr) { print $x; }
来源：http://pn.shxzskj.cn

[T46] Perl：哈希操作
来源：http://ds.hnjuh.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nf.chemitech.net.cn

[T47] Perl：正则捕获
来源：http://hd.colortex.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://yz.hnjuh.cn

[T48] Perl：正则替换
来源：http://iv.newstarts.cn

$s =~ s/old/new/g;
来源：http://na.shxzukj.cn

[T49] Perl：函数
来源：http://vk.jctech888.com.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cy.colortex.cn

[T50] Perl：逐行读文件
来源：http://cb.521024.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xf.haigaiapp.cn

while (my $line = <$fh>) { print $line; }
来源：http://bn.chemitech.net.cn

[T51] Scala：Hello World
来源：http://tm.jctech888.com.cn

println("Hello")
来源：http://rh.huixiangedu.cn

[T52] Scala：变量
来源：http://ns.muxihuayi.cn

val a = 1;  var b = 2
来源：http://lf.bookmarksfly.cn

[T53] Scala：字符串插值
来源：http://jo.szsharing.cn

s"值: $b"
来源：http://cp.lnxyls.cn

[T54] Scala：集合映射
来源：http://cp.muxihuayi.cn

List(1, 2, 3).map(_ * 2)
来源：http://yl.nicolike.cn

[T55] Scala：集合过滤
来源：http://ha.panjiajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://kc.shxzskj.cn

[T56] Scala：样例类
来源：http://xv.gzmigu.cn

case class User(name: String, age: Int)
来源：http://vx.huixiangedu.cn

[T57] Scala：模式匹配
来源：http://ix.chemitech.net.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://jp.szxytkj.cn

[T58] Scala：函数定义
来源：http://zh.chemitech.net.cn

def add(a: Int, b: Int): Int = a + b
来源：http://rj.hahajie.cn

[T59] Scala：循环
来源：http://ku.yuntaijiaju.cn

for (i <- 1 to 10) println(i)
来源：http://mm.nicolike.cn

[T60] Scala：折叠
来源：http://yb.szsharing.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ac.yuntaijiaju.cn

================================================================================
来源：http://ip.newstarts.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hy.asd995.cn

================================================================================
来源：http://na.bjjhwx.cn

[U01] Py：创建虚拟环境
来源：http://yk.szxytkj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://gu.521024.cn

[U02] Py：导出 / 安装依赖
来源：http://hd.wgjwhj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ae.bookmarksfly.cn

[U03] Py：加载 .env 配置
来源：http://dc.hnjuh.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://tr.szxytkj.cn

[U04] Py：变量调试打印
来源：http://uw.szsharing.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://co.yuntaijiaju.cn

[U05] Py：列表去重且保序
来源：http://ah.lnxyls.cn

list(dict.fromkeys(arr))
来源：http://vi.muxihuayi.cn

[U06] Py：合并两个字典
来源：http://ar.jianghongdianzi.cn

{**a, **b}
来源：http://fz.haigaiapp.cn

[U07] Py：反转字典键值
来源：http://tj.wgjwhj.cn

{v: k for k, v in d.items()}
来源：http://hv.shxzskj.cn

[U08] Py：展平二维列表
来源：http://le.9csxet.cn

[y for x in nested for y in x]
来源：http://mc.muxihuayi.cn

[U09] Py：字典取最大值的键
来源：http://uu.jianghongdianzi.cn

max(d, key=d.get)
来源：http://rz.jctech888.com.cn

[U10] Py：按值排序字典
来源：http://ml.colortex.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zw.newstarts.cn

[U11] Py：生成器表达式
来源：http://kx.panjiajie.cn

(x * 2 for x in arr)
来源：http://je.chemitech.net.cn

[U12] Py：取出现最多的 3 个元素
来源：http://pc.hnjuh.cn

Counter(arr).most_common(3)
来源：http://lb.yuexingan06.cn

[U13] Py：固定长度队列
来源：http://oc.huixiangedu.cn

deque(maxlen=10)
来源：http://cw.jianghongdianzi.cn

[U14] Py：分组收集到列表
来源：http://uf.jctech888.com.cn

defaultdict(list)
来源：http://vv.bjjhwx.cn

[U15] Py：高精度计时
来源：http://xq.asd995.cn

t = time.perf_counter()
来源：http://ox.panjiajie.cn

[U16] Py：命令行参数解析
来源：http://us.yuntaijiaju.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dp.panjiajie.cn

[U17] Py：初始化日志
来源：http://wr.colortex.cn

logging.basicConfig(level=logging.INFO)
来源：http://ak.panjiajie.cn

[U18] Py：预编译正则
来源：http://la.shxzskj.cn

pat = re.compile(r"\d+")
来源：http://si.shxzukj.cn

[U19] Py：正则替换带回调
来源：http://gj.shxzskj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://av.9csxet.cn

[U20] Py：缓存函数结果
来源：http://go.panjiajie.cn

@functools.lru_cache(maxsize=None)
来源：http://qi.nicolike.cn

[U21] Py：自定义上下文管理器
来源：http://kg.yuntaijiaju.cn

@contextlib.contextmanager
来源：http://lp.newstarts.cn

[U22] Py：矩阵转置
来源：http://oy.szsharing.cn

list(zip(*m))
来源：http://aw.nicolike.cn

[U23] Py：分块读取大文件
来源：http://ue.9csxet.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pq.bjjhwx.cn

[U24] Py：路径操作
来源：http://zs.nicolike.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ae.colortex.cn

[U25] Py：CSV 按字典读
来源：http://tq.asd995.cn

csv.DictReader(f)
来源：http://ea.nszjky.cn

[U26] Py：并发下载
来源：http://mg.lnxyls.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nc.shtwfgs.cn

[U27] Py：异步 HTTP
来源：http://ni.shtwfgs.cn

aiohttp.ClientSession() 配合 async with
来源：http://eh.shtwfgs.cn

[U28] Py：类型别名
来源：http://zr.bookmarksfly.cn

UserId = int
来源：http://mv.yuexingan06.cn

[U29] Py：属性校验
来源：http://vg.jctech888.com.cn

@property 与 @x.setter 配合
来源：http://dj.nszjky.cn

[U30] Py：数据类
来源：http://xl.muxihuayi.cn

@dataclass(slots=True)
来源：http://ri.wgjwhj.cn

[U31] Py：单测
来源：http://by.bookmarksfly.cn

python -m pytest -q
来源：http://fm.shtwfgs.cn

[U32] Py：代码格式化
来源：http://hg.jianghongdianzi.cn

ruff format . && ruff check --fix .
来源：http://dy.jianghongdianzi.cn

[U33] Py：打包发布
来源：http://vm.chemitech.net.cn

python -m build  （依赖 pyproject.toml）
来源：http://ob.shxzskj.cn

[U34] Py：判断编码
来源：http://oe.newstarts.cn

chardet.detect(raw)
来源：http://ui.newstarts.cn

[U35] Py：发送邮件
来源：http://rh.hnjuh.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://si.huixiangedu.cn

[U36] Py：定时任务
来源：http://ty.szsharing.cn

schedule.every(10).minutes.do(job)
来源：http://qx.szxytkj.cn

[U37] Py：读写 Excel
来源：http://qg.colortex.cn

pandas.read_excel / DataFrame.to_excel
来源：http://gh.bjjhwx.cn

[U38] Py：获取脚本所在目录
来源：http://os.huanxung.cn

Path(__file__).resolve().parent
来源：http://qd.521024.cn

[U39] Py：判断是否在交互环境
来源：http://eu.hnjuh.cn

sys.stdout.isatty()
来源：http://vx.jctech888.com.cn

[U40] Py：打印到标准错误
来源：http://vf.panjiajie.cn

print("err", file=sys.stderr)
来源：http://zs.szsharing.cn

[U41] PHP：初始化 Composer 项目
来源：http://fb.hahajie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://pp.huixinmuqiang.cn

[U42] PHP：PSR-4 自动加载
来源：http://gb.yuexingan06.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vs.szsharing.cn

[U43] PHP：声明命名空间
来源：http://cl.shxzukj.cn

namespace App\Http;
来源：http://yb.shtwfgs.cn

[U44] PHP：开启严格类型
来源：http://hy.szsharing.cn

declare(strict_types=1);
来源：http://as.shxzskj.cn

[U45] PHP：类型声明与返回类型
来源：http://gt.lnxyls.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://mz.shxzukj.cn

[U46] PHP：可空类型
来源：http://xt.jianghongdianzi.cn

?string $name = null
来源：http://ln.szxytkj.cn

[U47] PHP：联合类型
来源：http://qu.huixiangedu.cn

int|string $id
来源：http://yc.jctech888.com.cn

[U48] PHP：纯枚举
来源：http://uh.yuntaijiaju.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fe.haigaiapp.cn

[U49] PHP：只读属性
来源：http://cc.nszjky.cn

public readonly string $name
来源：http://wi.huixiangedu.cn

[U50] PHP：构造器属性提升
来源：http://pl.szxytkj.cn

public function __construct(private int $id) {}
来源：http://kb.chemitech.net.cn

[U51] PHP：数组解构
来源：http://zg.hnjuh.cn

[$a, $b] = $arr;
来源：http://qg.521024.cn

[U52] PHP：箭头函数
来源：http://ba.muxihuayi.cn

$double = fn($x) => $x * 2;
来源：http://hq.521024.cn

[U53] PHP：空合并运算符
来源：http://yu.lnxyls.cn

$v = $a ?? $b ?? "default";
来源：http://wd.shxzukj.cn

[U54] PHP：空安全调用
来源：http://vw.nicolike.cn

$obj?->method()
来源：http://kr.panjiajie.cn

[U55] PHP：match 表达式
来源：http://bp.huanxung.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zu.colortex.cn

[U56] PHP：命名参数
来源：http://lh.bookmarksfly.cn

f(a: 1, b: 2)
来源：http://qu.hahajie.cn

[U57] PHP：字符串插值
来源：http://if.hahajie.cn

"值: {$a}"
来源：http://gv.huixiangedu.cn

[U58] PHP：数组三件套
来源：http://ls.muxihuayi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rj.nszjky.cn

[U59] PHP：自定义排序
来源：http://gh.shxzskj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gb.shtwfgs.cn

[U60] PHP：JSON 编解码
来源：http://hg.lnxyls.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vm.lnxyls.cn

[U61] PHP：正则
来源：http://fi.shxzskj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://db.shxzukj.cn

[U62] PHP：日期对象
来源：http://tf.bjjhwx.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://za.haigaiapp.cn

[U63] PHP：文件读写
来源：http://rn.yuexingan06.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pz.shxzukj.cn

[U64] PHP：目录遍历
来源：http://mv.chemitech.net.cn

glob("dir/*.php");  scandir("dir");
来源：http://wx.hahajie.cn

[U65] PHP：会话
来源：http://ms.shxzukj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://fq.chemitech.net.cn

[U66] PHP：设置 Cookie
来源：http://pr.9csxet.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vr.jianghongdianzi.cn

[U67] PHP：处理文件上传
来源：http://nd.muxihuayi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hi.hahajie.cn

[U68] PHP：PDO 连接
来源：http://da.yuntaijiaju.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ji.jianghongdianzi.cn

[U69] PHP：PDO 预处理
来源：http://bg.chemitech.net.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xh.bjjhwx.cn

[U70] PHP：PDO 事务
来源：http://zd.huanxung.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gf.asd995.cn

[U71] PHP：抛出异常
来源：http://ae.panjiajie.cn

throw new RuntimeException("失败", 500);
来源：http://ls.bjjhwx.cn

[U72] PHP：写错误日志
来源：http://wl.muxihuayi.cn

error_log("失败: " . $e->getMessage());
来源：http://gl.newstarts.cn

[U73] PHP：读取 ini 配置
来源：http://zm.newstarts.cn

parse_ini_file("config.ini", true)
来源：http://es.colortex.cn

[U74] PHP：读取环境变量
来源：http://pc.colortex.cn

getenv("APP_ENV") ?: "production"
来源：http://wh.shtwfgs.cn

[U75] PHP：依赖注入
来源：http://ib.szsharing.cn

composer require psr/container
来源：http://oe.huixinmuqiang.cn

[U76] PHP：简单路由
来源：http://lq.shtwfgs.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ll.haigaiapp.cn

[U77] PHP：模板渲染
来源：http://aw.shxzskj.cn

composer require twig/twig
来源：http://te.panjiajie.cn

[U78] PHP：单元测试
来源：http://lq.hahajie.cn

composer require --dev phpunit/phpunit
来源：http://ru.szxytkj.cn

[U79] PHP：静态分析
来源：http://xs.bookmarksfly.cn

composer require --dev phpstan/phpstan
来源：http://ca.newstarts.cn

[U80] PHP：代码规范修复
来源：http://zw.nszjky.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ej.jianghongdianzi.cn

[U81] JS：初始化项目
来源：http://zh.jctech888.com.cn

npm init -y;  npm i express
来源：http://qk.521024.cn

[U82] JS：package.json 脚本
来源：http://nt.jianghongdianzi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wj.muxihuayi.cn

[U83] JS：ES Module 导入导出
来源：http://at.jctech888.com.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ik.panjiajie.cn

[U84] JS：CommonJS 写法
来源：http://ls.huanxung.cn

module.exports = { a };  const { a } = require("./m");
来源：http://hc.shxzukj.cn

[U85] JS：可选链
来源：http://zk.nszjky.cn

a?.b?.c
来源：http://kt.haigaiapp.cn

[U86] JS：空值合并
来源：http://pd.gzmigu.cn

a ?? b
来源：http://ac.shtwfgs.cn

[U87] JS：解构默认值
来源：http://ut.haigaiapp.cn

const { a = 1, b = 2 } = obj;
来源：http://cf.chemitech.net.cn

[U88] JS：对象展开合并
来源：http://lh.jianghongdianzi.cn

{ ...a, ...b }
来源：http://qy.huixiangedu.cn

[U89] JS：数组去重
来源：http://fm.yuntaijiaju.cn

[...new Set(arr)]
来源：http://ur.9csxet.cn

[U90] JS：数字数组排序
来源：http://jp.haigaiapp.cn

[...arr].sort((a, b) => a - b)
来源：http://im.jctech888.com.cn

[U91] JS：对象键值遍历
来源：http://fj.nszjky.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hr.muxihuayi.cn

[U92] JS：深拷贝
来源：http://wa.shxzskj.cn

structuredClone(obj)
来源：http://vj.colortex.cn

[U93] JS：模板字符串
来源：http://zs.jianghongdianzi.cn

`共 ${n} 条`
来源：http://vh.asd995.cn

[U94] JS：箭头函数
来源：http://ks.gzmigu.cn

const double = x => x * 2;
来源：http://pt.shtwfgs.cn

[U95] JS：Promise 包装
来源：http://et.521024.cn

new Promise((resolve, reject) => {})
来源：http://ue.panjiajie.cn

[U96] JS：async/await 与异常
来源：http://nl.lnxyls.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://uu.nicolike.cn

[U97] JS：并发请求
来源：http://df.colortex.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://pz.gzmigu.cn

[U98] JS：fetch 带 JSON
来源：http://xe.colortex.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ws.521024.cn

[U99] JS：事件监听
来源：http://be.jianghongdianzi.cn

el.addEventListener("click", e => {})
来源：http://uu.haigaiapp.cn

[U100] JS：DOM 查询
来源：http://zh.panjiajie.cn

document.querySelector(".item")
来源：http://dx.huixiangedu.cn

[U101] JS：classList 操作
来源：http://vk.yuexingan06.cn

el.classList.toggle("active")
来源：http://az.muxihuayi.cn

[U102] JS：本地存储
来源：http://mk.bookmarksfly.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://io.shtwfgs.cn

[U103] JS：定时器
来源：http://lu.huixiangedu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://az.huixiangedu.cn

[U104] JS：防抖
来源：http://tb.huixiangedu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dd.haigaiapp.cn

[U105] JS：节流
来源：http://pk.panjiajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://au.muxihuayi.cn

[U106] JS：日期格式化
来源：http://vp.newstarts.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jy.yuexingan06.cn

[U107] JS：数字千分位
来源：http://nf.bookmarksfly.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bt.haigaiapp.cn

[U108] JS：随机整数
来源：http://ll.nicolike.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://md.jianghongdianzi.cn

[U109] JS：数组分组
来源：http://sa.szxytkj.cn

Object.groupBy(arr, x => x.type)
来源：http://ps.muxihuayi.cn

[U110] JS：数组分块
来源：http://uz.jianghongdianzi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pw.jianghongdianzi.cn

[U111] JS：对象转 Map
来源：http://kk.jctech888.com.cn

new Map(Object.entries(obj))
来源：http://xm.colortex.cn

[U112] JS：字符串补位
来源：http://ki.newstarts.cn

"7".padStart(3, "0")
来源：http://wo.9csxet.cn

[U113] JS：正则替换全部
来源：http://fz.huixinmuqiang.cn

s.replaceAll("a", "b")
来源：http://nb.chemitech.net.cn

[U114] JS：JSON 深比较
来源：http://tk.haigaiapp.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://xq.chemitech.net.cn

[U115] JS：生成 UUID
来源：http://tg.shxzskj.cn

crypto.randomUUID()
来源：http://ls.huanxung.cn

[U116] JS：类型检查（JSDoc）
来源：http://jc.gzmigu.cn

/** @param {string} name */ function f(name) {}
来源：http://gv.9csxet.cn

[U117] JS：单元测试
来源：http://pr.hnjuh.cn

npm i -D vitest;  npx vitest
来源：http://to.szsharing.cn

[U118] JS：开发服务器
来源：http://el.huixiangedu.cn

npm i -D vite;  npx vite
来源：http://zw.chemitech.net.cn

[U119] JS：生产构建
来源：http://xs.yuexingan06.cn

npx vite build
来源：http://zt.shxzukj.cn

[U120] JS：读取环境变量（Vite）
来源：http://bc.nicolike.cn

import.meta.env.VITE_API_URL
来源：http://gl.newstarts.cn

================================================================================
来源：http://ba.szsharing.cn

统计汇总
来源：http://ph.jctech888.com.cn

================================================================================
来源：http://vq.asd995.cn

按语言统计（条）：
来源：http://vf.asd995.cn

Python ......... 252
来源：http://pl.wgjwhj.cn

PHP ............ 252
来源：http://ga.muxihuayi.cn

JavaScript ..... 252
来源：http://hp.yuexingan06.cn

TypeScript ..... 212
来源：http://gu.lnxyls.cn


<!-- 参考信息 -->