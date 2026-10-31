代发 wailian999

[T37] Lua：字符串拼接
来源：http://qb.jianghongdianzi.cn

"a" .. "b"
来源：http://tz.bookmarksfly.cn

[T38] Lua：条件
来源：http://jb.nicolike.cn

if x > 0 then print("正") end
来源：http://ix.bjjhwx.cn

[T39] Lua：模式匹配
来源：http://wh.huixiangedu.cn

string.find(s, "%d+")
来源：http://ul.gzmigu.cn

[T40] Lua：元表
来源：http://co.szxytkj.cn

setmetatable({}, { __index = base })
来源：http://lm.shtwfgs.cn

[T41] Perl：Hello World
来源：http://at.haigaiapp.cn

print "Hello\n";
来源：http://pk.nicolike.cn

[T42] Perl：变量类型
来源：http://wz.huanxung.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wq.hnjuh.cn

[T43] Perl：字符串插值
来源：http://qm.asd995.cn

"值: $a"
来源：http://zd.nicolike.cn

[T44] Perl：条件
来源：http://im.jctech888.com.cn

if ($a > 0) { print "正"; }
来源：http://ji.asd995.cn

[T45] Perl：数组遍历
来源：http://is.szxytkj.cn

for my $x (@arr) { print $x; }
来源：http://wk.szxytkj.cn

[T46] Perl：哈希操作
来源：http://we.huixinmuqiang.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qq.jctech888.com.cn

[T47] Perl：正则捕获
来源：http://mf.muxihuayi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ko.nicolike.cn

[T48] Perl：正则替换
来源：http://ff.szxytkj.cn

$s =~ s/old/new/g;
来源：http://bo.bookmarksfly.cn

[T49] Perl：函数
来源：http://qv.colortex.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zs.bookmarksfly.cn

[T50] Perl：逐行读文件
来源：http://bk.asd995.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://lv.521024.cn

while (my $line = <$fh>) { print $line; }
来源：http://ip.bookmarksfly.cn

[T51] Scala：Hello World
来源：http://tu.jianghongdianzi.cn

println("Hello")
来源：http://qa.chemitech.net.cn

[T52] Scala：变量
来源：http://xe.panjiajie.cn

val a = 1;  var b = 2
来源：http://eq.nicolike.cn

[T53] Scala：字符串插值
来源：http://em.panjiajie.cn

s"值: $b"
来源：http://rh.nszjky.cn

[T54] Scala：集合映射
来源：http://tp.nszjky.cn

List(1, 2, 3).map(_ * 2)
来源：http://uh.szxytkj.cn

[T55] Scala：集合过滤
来源：http://ql.szsharing.cn

List(1, 2, 3).filter(_ > 1)
来源：http://pu.yuexingan06.cn

[T56] Scala：样例类
来源：http://ma.jctech888.com.cn

case class User(name: String, age: Int)
来源：http://yh.asd995.cn

[T57] Scala：模式匹配
来源：http://wp.szsharing.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tu.asd995.cn

[T58] Scala：函数定义
来源：http://bs.panjiajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ih.shxzukj.cn

[T59] Scala：循环
来源：http://bk.shtwfgs.cn

for (i <- 1 to 10) println(i)
来源：http://bs.newstarts.cn

[T60] Scala：折叠
来源：http://rg.gzmigu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://eq.521024.cn

================================================================================
来源：http://eu.521024.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://db.muxihuayi.cn

================================================================================
来源：http://ze.asd995.cn

[U01] Py：创建虚拟环境
来源：http://wc.521024.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wg.huixiangedu.cn

[U02] Py：导出 / 安装依赖
来源：http://uf.jctech888.com.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gp.bookmarksfly.cn

[U03] Py：加载 .env 配置
来源：http://vi.9csxet.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wz.lnxyls.cn

[U04] Py：变量调试打印
来源：http://ui.jctech888.com.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ok.huixinmuqiang.cn

[U05] Py：列表去重且保序
来源：http://vy.yuntaijiaju.cn

list(dict.fromkeys(arr))
来源：http://mt.nicolike.cn

[U06] Py：合并两个字典
来源：http://ja.haigaiapp.cn

{**a, **b}
来源：http://fk.huixiangedu.cn

[U07] Py：反转字典键值
来源：http://qz.yuexingan06.cn

{v: k for k, v in d.items()}
来源：http://av.521024.cn

[U08] Py：展平二维列表
来源：http://rl.gzmigu.cn

[y for x in nested for y in x]
来源：http://sr.yuexingan06.cn

[U09] Py：字典取最大值的键
来源：http://jt.huixinmuqiang.cn

max(d, key=d.get)
来源：http://sh.nszjky.cn

[U10] Py：按值排序字典
来源：http://bj.shxzskj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kp.haigaiapp.cn

[U11] Py：生成器表达式
来源：http://kw.gzmigu.cn

(x * 2 for x in arr)
来源：http://mv.gzmigu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xe.wgjwhj.cn

Counter(arr).most_common(3)
来源：http://cm.nszjky.cn

[U13] Py：固定长度队列
来源：http://wi.521024.cn

deque(maxlen=10)
来源：http://hm.hahajie.cn

[U14] Py：分组收集到列表
来源：http://te.nszjky.cn

defaultdict(list)
来源：http://zz.hahajie.cn

[U15] Py：高精度计时
来源：http://jy.9csxet.cn

t = time.perf_counter()
来源：http://nt.yuexingan06.cn

[U16] Py：命令行参数解析
来源：http://gl.szsharing.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ui.szsharing.cn

[U17] Py：初始化日志
来源：http://tm.shtwfgs.cn

logging.basicConfig(level=logging.INFO)
来源：http://ns.newstarts.cn

[U18] Py：预编译正则
来源：http://wc.chemitech.net.cn

pat = re.compile(r"\d+")
来源：http://hw.chemitech.net.cn

[U19] Py：正则替换带回调
来源：http://rx.yuntaijiaju.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ks.asd995.cn

[U20] Py：缓存函数结果
来源：http://ue.yuexingan06.cn

@functools.lru_cache(maxsize=None)
来源：http://xe.521024.cn

[U21] Py：自定义上下文管理器
来源：http://md.jctech888.com.cn

@contextlib.contextmanager
来源：http://ol.nicolike.cn

[U22] Py：矩阵转置
来源：http://od.yuntaijiaju.cn

list(zip(*m))
来源：http://tv.hnjuh.cn

[U23] Py：分块读取大文件
来源：http://mn.panjiajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wn.wgjwhj.cn

[U24] Py：路径操作
来源：http://km.shtwfgs.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mx.colortex.cn

[U25] Py：CSV 按字典读
来源：http://rc.muxihuayi.cn

csv.DictReader(f)
来源：http://qr.muxihuayi.cn

[U26] Py：并发下载
来源：http://jb.huixinmuqiang.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kf.chemitech.net.cn

[U27] Py：异步 HTTP
来源：http://sy.hahajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://kp.gzmigu.cn

[U28] Py：类型别名
来源：http://lo.colortex.cn

UserId = int
来源：http://ou.hahajie.cn

[U29] Py：属性校验
来源：http://ut.shtwfgs.cn

@property 与 @x.setter 配合
来源：http://ri.yuntaijiaju.cn

[U30] Py：数据类
来源：http://al.huanxung.cn

@dataclass(slots=True)
来源：http://jr.wgjwhj.cn

[U31] Py：单测
来源：http://pq.szxytkj.cn

python -m pytest -q
来源：http://qb.panjiajie.cn

[U32] Py：代码格式化
来源：http://uy.szxytkj.cn

ruff format . && ruff check --fix .
来源：http://et.szxytkj.cn

[U33] Py：打包发布
来源：http://qw.hnjuh.cn

python -m build  （依赖 pyproject.toml）
来源：http://oj.shxzskj.cn

[U34] Py：判断编码
来源：http://nm.wgjwhj.cn

chardet.detect(raw)
来源：http://wj.jctech888.com.cn

[U35] Py：发送邮件
来源：http://tm.nszjky.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://sa.9csxet.cn

[U36] Py：定时任务
来源：http://wf.nicolike.cn

schedule.every(10).minutes.do(job)
来源：http://ro.yuntaijiaju.cn

[U37] Py：读写 Excel
来源：http://gp.chemitech.net.cn

pandas.read_excel / DataFrame.to_excel
来源：http://fr.panjiajie.cn

[U38] Py：获取脚本所在目录
来源：http://yo.shtwfgs.cn

Path(__file__).resolve().parent
来源：http://os.shxzukj.cn

[U39] Py：判断是否在交互环境
来源：http://qw.muxihuayi.cn

sys.stdout.isatty()
来源：http://lz.hnjuh.cn

[U40] Py：打印到标准错误
来源：http://ya.muxihuayi.cn

print("err", file=sys.stderr)
来源：http://eo.jctech888.com.cn

[U41] PHP：初始化 Composer 项目
来源：http://pi.newstarts.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://nb.shxzukj.cn

[U42] PHP：PSR-4 自动加载
来源：http://nj.colortex.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tx.lnxyls.cn

[U43] PHP：声明命名空间
来源：http://ba.521024.cn

namespace App\Http;
来源：http://sy.wgjwhj.cn

[U44] PHP：开启严格类型
来源：http://an.lnxyls.cn

declare(strict_types=1);
来源：http://yd.jianghongdianzi.cn

[U45] PHP：类型声明与返回类型
来源：http://rb.szsharing.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://dw.yuexingan06.cn

[U46] PHP：可空类型
来源：http://lm.asd995.cn

?string $name = null
来源：http://ja.wgjwhj.cn

[U47] PHP：联合类型
来源：http://mq.lnxyls.cn

int|string $id
来源：http://ng.bjjhwx.cn

[U48] PHP：纯枚举
来源：http://de.hnjuh.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://il.nicolike.cn

[U49] PHP：只读属性
来源：http://lu.gzmigu.cn

public readonly string $name
来源：http://ug.gzmigu.cn

[U50] PHP：构造器属性提升
来源：http://mq.9csxet.cn

public function __construct(private int $id) {}
来源：http://es.shxzukj.cn

[U51] PHP：数组解构
来源：http://jv.bookmarksfly.cn

[$a, $b] = $arr;
来源：http://jf.colortex.cn

[U52] PHP：箭头函数
来源：http://gi.wgjwhj.cn

$double = fn($x) => $x * 2;
来源：http://fr.shtwfgs.cn

[U53] PHP：空合并运算符
来源：http://bs.shtwfgs.cn

$v = $a ?? $b ?? "default";
来源：http://pp.wgjwhj.cn

[U54] PHP：空安全调用
来源：http://at.shtwfgs.cn

$obj?->method()
来源：http://hk.muxihuayi.cn

[U55] PHP：match 表达式
来源：http://ax.gzmigu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dm.lnxyls.cn

[U56] PHP：命名参数
来源：http://kw.hahajie.cn

f(a: 1, b: 2)
来源：http://ic.shxzskj.cn

[U57] PHP：字符串插值
来源：http://tk.jianghongdianzi.cn

"值: {$a}"
来源：http://nx.bjjhwx.cn

[U58] PHP：数组三件套
来源：http://ef.9csxet.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kh.shxzskj.cn

[U59] PHP：自定义排序
来源：http://xg.gzmigu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ch.chemitech.net.cn

[U60] PHP：JSON 编解码
来源：http://lq.bookmarksfly.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xt.gzmigu.cn

[U61] PHP：正则
来源：http://wi.shxzukj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://og.jianghongdianzi.cn

[U62] PHP：日期对象
来源：http://ug.yuexingan06.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rw.panjiajie.cn

[U63] PHP：文件读写
来源：http://aa.yuexingan06.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ct.wgjwhj.cn

[U64] PHP：目录遍历
来源：http://wt.hahajie.cn

glob("dir/*.php");  scandir("dir");
来源：http://nv.panjiajie.cn

[U65] PHP：会话
来源：http://ns.chemitech.net.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://yj.huixinmuqiang.cn

[U66] PHP：设置 Cookie
来源：http://cc.9csxet.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lk.huanxung.cn

[U67] PHP：处理文件上传
来源：http://hu.hahajie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wk.yuntaijiaju.cn

[U68] PHP：PDO 连接
来源：http://qd.asd995.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nb.hnjuh.cn

[U69] PHP：PDO 预处理
来源：http://ll.shxzukj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bp.asd995.cn

[U70] PHP：PDO 事务
来源：http://mg.9csxet.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kb.yuexingan06.cn

[U71] PHP：抛出异常
来源：http://ym.yuntaijiaju.cn

throw new RuntimeException("失败", 500);
来源：http://uj.chemitech.net.cn

[U72] PHP：写错误日志
来源：http://yi.9csxet.cn

error_log("失败: " . $e->getMessage());
来源：http://rw.chemitech.net.cn

[U73] PHP：读取 ini 配置
来源：http://wp.huixinmuqiang.cn

parse_ini_file("config.ini", true)
来源：http://gu.huanxung.cn

[U74] PHP：读取环境变量
来源：http://lx.nszjky.cn

getenv("APP_ENV") ?: "production"
来源：http://tm.asd995.cn

[U75] PHP：依赖注入
来源：http://ow.szxytkj.cn

composer require psr/container
来源：http://kw.gzmigu.cn

[U76] PHP：简单路由
来源：http://kr.shxzukj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xk.nicolike.cn

[U77] PHP：模板渲染
来源：http://bd.gzmigu.cn

composer require twig/twig
来源：http://lr.521024.cn

[U78] PHP：单元测试
来源：http://sr.nicolike.cn

composer require --dev phpunit/phpunit
来源：http://mc.jianghongdianzi.cn

[U79] PHP：静态分析
来源：http://oj.yuexingan06.cn

composer require --dev phpstan/phpstan
来源：http://gd.nicolike.cn

[U80] PHP：代码规范修复
来源：http://bh.newstarts.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://po.nicolike.cn

[U81] JS：初始化项目
来源：http://af.yuntaijiaju.cn

npm init -y;  npm i express
来源：http://nt.jctech888.com.cn

[U82] JS：package.json 脚本
来源：http://jh.hahajie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nj.colortex.cn

[U83] JS：ES Module 导入导出
来源：http://ub.colortex.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xo.asd995.cn

[U84] JS：CommonJS 写法
来源：http://py.shtwfgs.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ea.gzmigu.cn

[U85] JS：可选链
来源：http://oc.chemitech.net.cn

a?.b?.c
来源：http://xa.huixinmuqiang.cn

[U86] JS：空值合并
来源：http://gs.szsharing.cn

a ?? b
来源：http://rg.gzmigu.cn

[U87] JS：解构默认值
来源：http://or.colortex.cn

const { a = 1, b = 2 } = obj;
来源：http://gg.bjjhwx.cn

[U88] JS：对象展开合并
来源：http://ab.shxzukj.cn

{ ...a, ...b }
来源：http://uj.asd995.cn

[U89] JS：数组去重
来源：http://yr.huixiangedu.cn

[...new Set(arr)]
来源：http://en.panjiajie.cn

[U90] JS：数字数组排序
来源：http://cm.nszjky.cn

[...arr].sort((a, b) => a - b)
来源：http://tg.9csxet.cn

[U91] JS：对象键值遍历
来源：http://xh.colortex.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yl.lnxyls.cn

[U92] JS：深拷贝
来源：http://gr.muxihuayi.cn

structuredClone(obj)
来源：http://oi.szxytkj.cn

[U93] JS：模板字符串
来源：http://zv.nicolike.cn

`共 ${n} 条`
来源：http://yh.huanxung.cn

[U94] JS：箭头函数
来源：http://ac.jianghongdianzi.cn

const double = x => x * 2;
来源：http://rc.bookmarksfly.cn

[U95] JS：Promise 包装
来源：http://xl.huixinmuqiang.cn

new Promise((resolve, reject) => {})
来源：http://qw.muxihuayi.cn

[U96] JS：async/await 与异常
来源：http://gt.newstarts.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bf.jctech888.com.cn

[U97] JS：并发请求
来源：http://he.szxytkj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://sw.jctech888.com.cn

[U98] JS：fetch 带 JSON
来源：http://jc.huanxung.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hu.hnjuh.cn

[U99] JS：事件监听
来源：http://zr.huanxung.cn

el.addEventListener("click", e => {})
来源：http://fs.bjjhwx.cn

[U100] JS：DOM 查询
来源：http://hr.muxihuayi.cn

document.querySelector(".item")
来源：http://ql.asd995.cn

[U101] JS：classList 操作
来源：http://fz.lnxyls.cn

el.classList.toggle("active")
来源：http://hx.shxzskj.cn

[U102] JS：本地存储
来源：http://fk.huixinmuqiang.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://pe.panjiajie.cn

[U103] JS：定时器
来源：http://le.asd995.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://cf.521024.cn

[U104] JS：防抖
来源：http://zk.shxzskj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nm.nszjky.cn

[U105] JS：节流
来源：http://ap.szsharing.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fu.huixiangedu.cn

[U106] JS：日期格式化
来源：http://sq.wgjwhj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dr.yuexingan06.cn

[U107] JS：数字千分位
来源：http://et.jianghongdianzi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sd.521024.cn

[U108] JS：随机整数
来源：http://fk.hnjuh.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vr.shtwfgs.cn

[U109] JS：数组分组
来源：http://kh.bookmarksfly.cn

Object.groupBy(arr, x => x.type)
来源：http://sr.yuntaijiaju.cn

[U110] JS：数组分块
来源：http://zl.huixinmuqiang.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zk.huixiangedu.cn

[U111] JS：对象转 Map
来源：http://qe.newstarts.cn

new Map(Object.entries(obj))
来源：http://dk.chemitech.net.cn

[U112] JS：字符串补位
来源：http://gc.wgjwhj.cn

"7".padStart(3, "0")
来源：http://ou.yuntaijiaju.cn

[U113] JS：正则替换全部
来源：http://ok.muxihuayi.cn

s.replaceAll("a", "b")
来源：http://vf.wgjwhj.cn

[U114] JS：JSON 深比较
来源：http://ux.shtwfgs.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hu.huixiangedu.cn

[U115] JS：生成 UUID
来源：http://dv.muxihuayi.cn

crypto.randomUUID()
来源：http://py.panjiajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://df.bookmarksfly.cn

/** @param {string} name */ function f(name) {}
来源：http://ll.shtwfgs.cn

[U117] JS：单元测试
来源：http://ca.asd995.cn

npm i -D vitest;  npx vitest
来源：http://vg.huixinmuqiang.cn

[U118] JS：开发服务器
来源：http://pw.gzmigu.cn

npm i -D vite;  npx vite
来源：http://za.nicolike.cn

[U119] JS：生产构建
来源：http://yr.lnxyls.cn

npx vite build
来源：http://wy.huixinmuqiang.cn

[U120] JS：读取环境变量（Vite）
来源：http://py.shxzukj.cn

import.meta.env.VITE_API_URL
来源：http://cj.huanxung.cn

================================================================================
来源：http://ch.bookmarksfly.cn

统计汇总
来源：http://en.newstarts.cn

================================================================================
来源：http://lx.nicolike.cn

按语言统计（条）：
来源：http://eh.huixinmuqiang.cn

Python ......... 252
来源：http://me.bookmarksfly.cn

PHP ............ 252
来源：http://sp.wgjwhj.cn

JavaScript ..... 252
来源：http://bt.chemitech.net.cn

TypeScript ..... 212
来源：http://nl.yuntaijiaju.cn


<!-- 参考信息 -->