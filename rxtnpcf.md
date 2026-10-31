代发 wailian999

[T41] Perl：Hello World
来源：http://pv.shxzukj.cn

print "Hello\n";
来源：http://ii.huixinmuqiang.cn

[T42] Perl：变量类型
来源：http://mf.haigaiapp.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jr.szsharing.cn

[T43] Perl：字符串插值
来源：http://pe.huixiangedu.cn

"值: $a"
来源：http://vr.asd995.cn

[T44] Perl：条件
来源：http://cc.hnjuh.cn

if ($a > 0) { print "正"; }
来源：http://ve.huanxung.cn

[T45] Perl：数组遍历
来源：http://lk.huixinmuqiang.cn

for my $x (@arr) { print $x; }
来源：http://gf.szsharing.cn

[T46] Perl：哈希操作
来源：http://sh.hahajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jm.szxytkj.cn

[T47] Perl：正则捕获
来源：http://tf.hnjuh.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ct.szxytkj.cn

[T48] Perl：正则替换
来源：http://ea.colortex.cn

$s =~ s/old/new/g;
来源：http://my.shxzukj.cn

[T49] Perl：函数
来源：http://uq.asd995.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xu.wgjwhj.cn

[T50] Perl：逐行读文件
来源：http://yj.newstarts.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://la.gzmigu.cn

while (my $line = <$fh>) { print $line; }
来源：http://xy.haigaiapp.cn

[T51] Scala：Hello World
来源：http://vd.haigaiapp.cn

println("Hello")
来源：http://zz.yuntaijiaju.cn

[T52] Scala：变量
来源：http://dx.huixiangedu.cn

val a = 1;  var b = 2
来源：http://fq.jianghongdianzi.cn

[T53] Scala：字符串插值
来源：http://qq.panjiajie.cn

s"值: $b"
来源：http://vh.bookmarksfly.cn

[T54] Scala：集合映射
来源：http://iz.szsharing.cn

List(1, 2, 3).map(_ * 2)
来源：http://xs.nszjky.cn

[T55] Scala：集合过滤
来源：http://yu.9csxet.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xp.bjjhwx.cn

[T56] Scala：样例类
来源：http://ym.wgjwhj.cn

case class User(name: String, age: Int)
来源：http://mp.newstarts.cn

[T57] Scala：模式匹配
来源：http://xe.newstarts.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://at.gzmigu.cn

[T58] Scala：函数定义
来源：http://ak.muxihuayi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://rh.wgjwhj.cn

[T59] Scala：循环
来源：http://og.huixiangedu.cn

for (i <- 1 to 10) println(i)
来源：http://kn.gzmigu.cn

[T60] Scala：折叠
来源：http://hg.bookmarksfly.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vc.wgjwhj.cn

================================================================================
来源：http://du.shxzukj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://om.shxzukj.cn

================================================================================
来源：http://tz.wgjwhj.cn

[U01] Py：创建虚拟环境
来源：http://yj.jctech888.com.cn

python -m venv .venv && source .venv/bin/activate
来源：http://os.newstarts.cn

[U02] Py：导出 / 安装依赖
来源：http://aj.nszjky.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rb.hnjuh.cn

[U03] Py：加载 .env 配置
来源：http://bc.521024.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://dy.huixinmuqiang.cn

[U04] Py：变量调试打印
来源：http://ec.asd995.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ql.lnxyls.cn

[U05] Py：列表去重且保序
来源：http://be.asd995.cn

list(dict.fromkeys(arr))
来源：http://aj.yuexingan06.cn

[U06] Py：合并两个字典
来源：http://pw.nszjky.cn

{**a, **b}
来源：http://er.bjjhwx.cn

[U07] Py：反转字典键值
来源：http://ri.nicolike.cn

{v: k for k, v in d.items()}
来源：http://xq.chemitech.net.cn

[U08] Py：展平二维列表
来源：http://qq.asd995.cn

[y for x in nested for y in x]
来源：http://dl.szsharing.cn

[U09] Py：字典取最大值的键
来源：http://qk.jctech888.com.cn

max(d, key=d.get)
来源：http://yo.shxzukj.cn

[U10] Py：按值排序字典
来源：http://zv.shxzskj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sm.colortex.cn

[U11] Py：生成器表达式
来源：http://cp.nszjky.cn

(x * 2 for x in arr)
来源：http://es.colortex.cn

[U12] Py：取出现最多的 3 个元素
来源：http://oq.asd995.cn

Counter(arr).most_common(3)
来源：http://pp.lnxyls.cn

[U13] Py：固定长度队列
来源：http://vw.szsharing.cn

deque(maxlen=10)
来源：http://oh.newstarts.cn

[U14] Py：分组收集到列表
来源：http://hq.gzmigu.cn

defaultdict(list)
来源：http://hr.jianghongdianzi.cn

[U15] Py：高精度计时
来源：http://dm.nszjky.cn

t = time.perf_counter()
来源：http://cp.haigaiapp.cn

[U16] Py：命令行参数解析
来源：http://gz.bjjhwx.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kb.yuexingan06.cn

[U17] Py：初始化日志
来源：http://mo.huanxung.cn

logging.basicConfig(level=logging.INFO)
来源：http://se.shtwfgs.cn

[U18] Py：预编译正则
来源：http://ar.wgjwhj.cn

pat = re.compile(r"\d+")
来源：http://hj.asd995.cn

[U19] Py：正则替换带回调
来源：http://bk.panjiajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dk.shxzukj.cn

[U20] Py：缓存函数结果
来源：http://sq.huanxung.cn

@functools.lru_cache(maxsize=None)
来源：http://bs.jianghongdianzi.cn

[U21] Py：自定义上下文管理器
来源：http://kl.hnjuh.cn

@contextlib.contextmanager
来源：http://hp.jianghongdianzi.cn

[U22] Py：矩阵转置
来源：http://ss.gzmigu.cn

list(zip(*m))
来源：http://vc.szxytkj.cn

[U23] Py：分块读取大文件
来源：http://ok.yuntaijiaju.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mz.huanxung.cn

[U24] Py：路径操作
来源：http://rm.huixiangedu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ek.huixiangedu.cn

[U25] Py：CSV 按字典读
来源：http://gp.huixiangedu.cn

csv.DictReader(f)
来源：http://dl.asd995.cn

[U26] Py：并发下载
来源：http://nx.muxihuayi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rz.muxihuayi.cn

[U27] Py：异步 HTTP
来源：http://gg.szxytkj.cn

aiohttp.ClientSession() 配合 async with
来源：http://xk.shxzskj.cn

[U28] Py：类型别名
来源：http://vy.szxytkj.cn

UserId = int
来源：http://eq.shtwfgs.cn

[U29] Py：属性校验
来源：http://zn.521024.cn

@property 与 @x.setter 配合
来源：http://xx.shxzukj.cn

[U30] Py：数据类
来源：http://th.szxytkj.cn

@dataclass(slots=True)
来源：http://ii.huixinmuqiang.cn

[U31] Py：单测
来源：http://su.lnxyls.cn

python -m pytest -q
来源：http://ix.bookmarksfly.cn

[U32] Py：代码格式化
来源：http://bo.shtwfgs.cn

ruff format . && ruff check --fix .
来源：http://wq.panjiajie.cn

[U33] Py：打包发布
来源：http://hz.colortex.cn

python -m build  （依赖 pyproject.toml）
来源：http://sn.jctech888.com.cn

[U34] Py：判断编码
来源：http://cs.colortex.cn

chardet.detect(raw)
来源：http://uh.bookmarksfly.cn

[U35] Py：发送邮件
来源：http://nn.521024.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dr.shtwfgs.cn

[U36] Py：定时任务
来源：http://go.jctech888.com.cn

schedule.every(10).minutes.do(job)
来源：http://yw.huixiangedu.cn

[U37] Py：读写 Excel
来源：http://rc.wgjwhj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qr.asd995.cn

[U38] Py：获取脚本所在目录
来源：http://gr.bookmarksfly.cn

Path(__file__).resolve().parent
来源：http://xg.szxytkj.cn

[U39] Py：判断是否在交互环境
来源：http://jl.huanxung.cn

sys.stdout.isatty()
来源：http://tm.hnjuh.cn

[U40] Py：打印到标准错误
来源：http://wf.chemitech.net.cn

print("err", file=sys.stderr)
来源：http://jl.haigaiapp.cn

[U41] PHP：初始化 Composer 项目
来源：http://st.huanxung.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zx.shtwfgs.cn

[U42] PHP：PSR-4 自动加载
来源：http://rk.huixinmuqiang.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pt.jctech888.com.cn

[U43] PHP：声明命名空间
来源：http://en.colortex.cn

namespace App\Http;
来源：http://xz.haigaiapp.cn

[U44] PHP：开启严格类型
来源：http://ze.huixinmuqiang.cn

declare(strict_types=1);
来源：http://lc.hnjuh.cn

[U45] PHP：类型声明与返回类型
来源：http://pm.yuexingan06.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://zq.bookmarksfly.cn

[U46] PHP：可空类型
来源：http://ug.colortex.cn

?string $name = null
来源：http://st.szsharing.cn

[U47] PHP：联合类型
来源：http://ib.wgjwhj.cn

int|string $id
来源：http://jd.jctech888.com.cn

[U48] PHP：纯枚举
来源：http://aj.bjjhwx.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gu.huanxung.cn

[U49] PHP：只读属性
来源：http://fc.muxihuayi.cn

public readonly string $name
来源：http://rt.hnjuh.cn

[U50] PHP：构造器属性提升
来源：http://gw.jianghongdianzi.cn

public function __construct(private int $id) {}
来源：http://by.hahajie.cn

[U51] PHP：数组解构
来源：http://pf.yuexingan06.cn

[$a, $b] = $arr;
来源：http://ql.szxytkj.cn

[U52] PHP：箭头函数
来源：http://it.huixinmuqiang.cn

$double = fn($x) => $x * 2;
来源：http://ol.jianghongdianzi.cn

[U53] PHP：空合并运算符
来源：http://do.yuntaijiaju.cn

$v = $a ?? $b ?? "default";
来源：http://lg.bjjhwx.cn

[U54] PHP：空安全调用
来源：http://sg.huixinmuqiang.cn

$obj?->method()
来源：http://dj.shxzskj.cn

[U55] PHP：match 表达式
来源：http://hr.huixinmuqiang.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fg.yuntaijiaju.cn

[U56] PHP：命名参数
来源：http://ga.colortex.cn

f(a: 1, b: 2)
来源：http://mu.huixinmuqiang.cn

[U57] PHP：字符串插值
来源：http://fa.shxzskj.cn

"值: {$a}"
来源：http://aj.nicolike.cn

[U58] PHP：数组三件套
来源：http://jo.hnjuh.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hq.newstarts.cn

[U59] PHP：自定义排序
来源：http://yw.chemitech.net.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sb.huixiangedu.cn

[U60] PHP：JSON 编解码
来源：http://jt.nicolike.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ur.huixinmuqiang.cn

[U61] PHP：正则
来源：http://qi.huixinmuqiang.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://un.521024.cn

[U62] PHP：日期对象
来源：http://gk.huanxung.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uo.haigaiapp.cn

[U63] PHP：文件读写
来源：http://dz.shtwfgs.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yt.9csxet.cn

[U64] PHP：目录遍历
来源：http://ai.wgjwhj.cn

glob("dir/*.php");  scandir("dir");
来源：http://kv.huixiangedu.cn

[U65] PHP：会话
来源：http://cy.yuexingan06.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ck.9csxet.cn

[U66] PHP：设置 Cookie
来源：http://ai.yuntaijiaju.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zu.huixiangedu.cn

[U67] PHP：处理文件上传
来源：http://cz.haigaiapp.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lu.gzmigu.cn

[U68] PHP：PDO 连接
来源：http://ae.hnjuh.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lw.bookmarksfly.cn

[U69] PHP：PDO 预处理
来源：http://ac.asd995.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://my.szxytkj.cn

[U70] PHP：PDO 事务
来源：http://xk.jctech888.com.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ia.haigaiapp.cn

[U71] PHP：抛出异常
来源：http://ot.colortex.cn

throw new RuntimeException("失败", 500);
来源：http://cz.521024.cn

[U72] PHP：写错误日志
来源：http://hm.asd995.cn

error_log("失败: " . $e->getMessage());
来源：http://la.yuexingan06.cn

[U73] PHP：读取 ini 配置
来源：http://eo.newstarts.cn

parse_ini_file("config.ini", true)
来源：http://rz.colortex.cn

[U74] PHP：读取环境变量
来源：http://wd.newstarts.cn

getenv("APP_ENV") ?: "production"
来源：http://aj.9csxet.cn

[U75] PHP：依赖注入
来源：http://uj.521024.cn

composer require psr/container
来源：http://dy.huanxung.cn

[U76] PHP：简单路由
来源：http://bs.chemitech.net.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vq.newstarts.cn

[U77] PHP：模板渲染
来源：http://gc.hahajie.cn

composer require twig/twig
来源：http://up.shxzukj.cn

[U78] PHP：单元测试
来源：http://yf.huixiangedu.cn

composer require --dev phpunit/phpunit
来源：http://mr.hnjuh.cn

[U79] PHP：静态分析
来源：http://bd.szxytkj.cn

composer require --dev phpstan/phpstan
来源：http://po.shxzskj.cn

[U80] PHP：代码规范修复
来源：http://lv.9csxet.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://rn.9csxet.cn

[U81] JS：初始化项目
来源：http://tt.bjjhwx.cn

npm init -y;  npm i express
来源：http://jv.newstarts.cn

[U82] JS：package.json 脚本
来源：http://ai.shtwfgs.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xh.gzmigu.cn

[U83] JS：ES Module 导入导出
来源：http://ea.shxzskj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://fb.shxzukj.cn

[U84] JS：CommonJS 写法
来源：http://xb.haigaiapp.cn

module.exports = { a };  const { a } = require("./m");
来源：http://bp.asd995.cn

[U85] JS：可选链
来源：http://ku.haigaiapp.cn

a?.b?.c
来源：http://de.gzmigu.cn

[U86] JS：空值合并
来源：http://az.panjiajie.cn

a ?? b
来源：http://vz.gzmigu.cn

[U87] JS：解构默认值
来源：http://sk.wgjwhj.cn

const { a = 1, b = 2 } = obj;
来源：http://ji.lnxyls.cn

[U88] JS：对象展开合并
来源：http://eo.newstarts.cn

{ ...a, ...b }
来源：http://uc.9csxet.cn

[U89] JS：数组去重
来源：http://in.shtwfgs.cn

[...new Set(arr)]
来源：http://ol.wgjwhj.cn

[U90] JS：数字数组排序
来源：http://nj.yuexingan06.cn

[...arr].sort((a, b) => a - b)
来源：http://sc.shxzukj.cn

[U91] JS：对象键值遍历
来源：http://ir.lnxyls.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tx.yuexingan06.cn

[U92] JS：深拷贝
来源：http://cq.jianghongdianzi.cn

structuredClone(obj)
来源：http://ek.hnjuh.cn

[U93] JS：模板字符串
来源：http://zs.nicolike.cn

`共 ${n} 条`
来源：http://fa.huixinmuqiang.cn

[U94] JS：箭头函数
来源：http://ez.shxzukj.cn

const double = x => x * 2;
来源：http://cb.muxihuayi.cn

[U95] JS：Promise 包装
来源：http://mu.huixiangedu.cn

new Promise((resolve, reject) => {})
来源：http://sr.shxzukj.cn

[U96] JS：async/await 与异常
来源：http://ot.bookmarksfly.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wm.muxihuayi.cn

[U97] JS：并发请求
来源：http://hd.gzmigu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://du.nicolike.cn

[U98] JS：fetch 带 JSON
来源：http://kl.gzmigu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jv.bookmarksfly.cn

[U99] JS：事件监听
来源：http://de.wgjwhj.cn

el.addEventListener("click", e => {})
来源：http://ze.bookmarksfly.cn

[U100] JS：DOM 查询
来源：http://bl.jctech888.com.cn

document.querySelector(".item")
来源：http://mi.521024.cn

[U101] JS：classList 操作
来源：http://ac.wgjwhj.cn

el.classList.toggle("active")
来源：http://fr.jctech888.com.cn

[U102] JS：本地存储
来源：http://ul.szsharing.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://fx.shxzukj.cn

[U103] JS：定时器
来源：http://dk.hahajie.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fs.jianghongdianzi.cn

[U104] JS：防抖
来源：http://zo.yuntaijiaju.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eq.nszjky.cn

[U105] JS：节流
来源：http://oa.bjjhwx.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wf.shtwfgs.cn

[U106] JS：日期格式化
来源：http://zr.huixinmuqiang.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ik.huixinmuqiang.cn

[U107] JS：数字千分位
来源：http://vo.newstarts.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jy.521024.cn

[U108] JS：随机整数
来源：http://gt.szsharing.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fi.chemitech.net.cn

[U109] JS：数组分组
来源：http://jy.asd995.cn

Object.groupBy(arr, x => x.type)
来源：http://kk.bjjhwx.cn

[U110] JS：数组分块
来源：http://ey.9csxet.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://uk.bjjhwx.cn

[U111] JS：对象转 Map
来源：http://rg.521024.cn

new Map(Object.entries(obj))
来源：http://np.haigaiapp.cn

[U112] JS：字符串补位
来源：http://lt.panjiajie.cn

"7".padStart(3, "0")
来源：http://rl.huanxung.cn

[U113] JS：正则替换全部
来源：http://yn.gzmigu.cn

s.replaceAll("a", "b")
来源：http://mt.asd995.cn

[U114] JS：JSON 深比较
来源：http://gi.wgjwhj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://oo.lnxyls.cn

[U115] JS：生成 UUID
来源：http://ud.wgjwhj.cn

crypto.randomUUID()
来源：http://re.jianghongdianzi.cn

[U116] JS：类型检查（JSDoc）
来源：http://ds.bookmarksfly.cn

/** @param {string} name */ function f(name) {}
来源：http://af.shxzukj.cn

[U117] JS：单元测试
来源：http://af.lnxyls.cn

npm i -D vitest;  npx vitest
来源：http://yb.wgjwhj.cn

[U118] JS：开发服务器
来源：http://fl.shxzskj.cn

npm i -D vite;  npx vite
来源：http://rc.gzmigu.cn

[U119] JS：生产构建
来源：http://fs.huixiangedu.cn

npx vite build
来源：http://ev.yuntaijiaju.cn

[U120] JS：读取环境变量（Vite）
来源：http://so.jianghongdianzi.cn

import.meta.env.VITE_API_URL
来源：http://co.szxytkj.cn

================================================================================
来源：http://lx.haigaiapp.cn

统计汇总
来源：http://sl.szsharing.cn

================================================================================
来源：http://we.colortex.cn

按语言统计（条）：
来源：http://xt.wgjwhj.cn

Python ......... 252
来源：http://or.colortex.cn

PHP ............ 252
来源：http://gc.hahajie.cn

JavaScript ..... 252
来源：http://uo.shxzukj.cn

TypeScript ..... 212
来源：http://vm.nszjky.cn

Java ........... 212
来源：http://zv.colortex.cn

Go ............. 212
来源：http://sw.colortex.cn

Ruby ........... 212
来源：http://fy.muxihuayi.cn

C# ............. 212
来源：http://jd.521024.cn

C .............. 30
来源：http://gv.9csxet.cn

C++ ............ 30
来源：http://ar.asd995.cn

SQL ............ 90
来源：http://io.haigaiapp.cn

Bash ........... 80
来源：http://pc.lnxyls.cn


<!-- 参考信息 -->