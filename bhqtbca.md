代发 wailian999

[T41] Perl：Hello World
来源：http://ro.yuntaijiaju.cn

print "Hello\n";
来源：http://ps.nicolike.cn

[T42] Perl：变量类型
来源：http://rq.newstarts.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xb.yuexingan06.cn

[T43] Perl：字符串插值
来源：http://wb.colortex.cn

"值: $a"
来源：http://he.9csxet.cn

[T44] Perl：条件
来源：http://ro.bjjhwx.cn

if ($a > 0) { print "正"; }
来源：http://lw.hahajie.cn

[T45] Perl：数组遍历
来源：http://th.bjjhwx.cn

for my $x (@arr) { print $x; }
来源：http://zg.bjjhwx.cn

[T46] Perl：哈希操作
来源：http://po.bjjhwx.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ul.huanxung.cn

[T47] Perl：正则捕获
来源：http://ne.nicolike.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://gz.gzmigu.cn

[T48] Perl：正则替换
来源：http://pt.chemitech.net.cn

$s =~ s/old/new/g;
来源：http://hb.muxihuayi.cn

[T49] Perl：函数
来源：http://rk.huixiangedu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pu.gzmigu.cn

[T50] Perl：逐行读文件
来源：http://qd.newstarts.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://iw.newstarts.cn

while (my $line = <$fh>) { print $line; }
来源：http://mk.bookmarksfly.cn

[T51] Scala：Hello World
来源：http://ht.521024.cn

println("Hello")
来源：http://qm.nicolike.cn

[T52] Scala：变量
来源：http://lu.hahajie.cn

val a = 1;  var b = 2
来源：http://di.shxzukj.cn

[T53] Scala：字符串插值
来源：http://re.huanxung.cn

s"值: $b"
来源：http://la.nszjky.cn

[T54] Scala：集合映射
来源：http://iv.haigaiapp.cn

List(1, 2, 3).map(_ * 2)
来源：http://ht.jianghongdianzi.cn

[T55] Scala：集合过滤
来源：http://yw.bjjhwx.cn

List(1, 2, 3).filter(_ > 1)
来源：http://eo.jianghongdianzi.cn

[T56] Scala：样例类
来源：http://vn.muxihuayi.cn

case class User(name: String, age: Int)
来源：http://sw.panjiajie.cn

[T57] Scala：模式匹配
来源：http://tr.szsharing.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://oq.hahajie.cn

[T58] Scala：函数定义
来源：http://hw.shtwfgs.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ej.yuexingan06.cn

[T59] Scala：循环
来源：http://px.yuntaijiaju.cn

for (i <- 1 to 10) println(i)
来源：http://ep.jctech888.com.cn

[T60] Scala：折叠
来源：http://sz.jctech888.com.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kk.shxzukj.cn

================================================================================
来源：http://nx.shtwfgs.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wz.9csxet.cn

================================================================================
来源：http://hg.gzmigu.cn

[U01] Py：创建虚拟环境
来源：http://lp.bookmarksfly.cn

python -m venv .venv && source .venv/bin/activate
来源：http://gz.huanxung.cn

[U02] Py：导出 / 安装依赖
来源：http://ay.9csxet.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ez.521024.cn

[U03] Py：加载 .env 配置
来源：http://qs.chemitech.net.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://no.lnxyls.cn

[U04] Py：变量调试打印
来源：http://ws.jianghongdianzi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sp.szxytkj.cn

[U05] Py：列表去重且保序
来源：http://xs.521024.cn

list(dict.fromkeys(arr))
来源：http://wy.newstarts.cn

[U06] Py：合并两个字典
来源：http://tk.jctech888.com.cn

{**a, **b}
来源：http://wc.hnjuh.cn

[U07] Py：反转字典键值
来源：http://lx.bjjhwx.cn

{v: k for k, v in d.items()}
来源：http://ql.jianghongdianzi.cn

[U08] Py：展平二维列表
来源：http://ic.521024.cn

[y for x in nested for y in x]
来源：http://un.hnjuh.cn

[U09] Py：字典取最大值的键
来源：http://yj.hahajie.cn

max(d, key=d.get)
来源：http://gt.jctech888.com.cn

[U10] Py：按值排序字典
来源：http://jq.wgjwhj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gm.nszjky.cn

[U11] Py：生成器表达式
来源：http://qs.lnxyls.cn

(x * 2 for x in arr)
来源：http://bn.shxzskj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rn.chemitech.net.cn

Counter(arr).most_common(3)
来源：http://mw.shxzukj.cn

[U13] Py：固定长度队列
来源：http://ok.huanxung.cn

deque(maxlen=10)
来源：http://za.muxihuayi.cn

[U14] Py：分组收集到列表
来源：http://rg.asd995.cn

defaultdict(list)
来源：http://cd.521024.cn

[U15] Py：高精度计时
来源：http://pf.jianghongdianzi.cn

t = time.perf_counter()
来源：http://ve.nicolike.cn

[U16] Py：命令行参数解析
来源：http://ir.muxihuayi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qy.shtwfgs.cn

[U17] Py：初始化日志
来源：http://pc.huanxung.cn

logging.basicConfig(level=logging.INFO)
来源：http://vn.muxihuayi.cn

[U18] Py：预编译正则
来源：http://op.huanxung.cn

pat = re.compile(r"\d+")
来源：http://xg.muxihuayi.cn

[U19] Py：正则替换带回调
来源：http://ef.szxytkj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ie.nicolike.cn

[U20] Py：缓存函数结果
来源：http://kv.gzmigu.cn

@functools.lru_cache(maxsize=None)
来源：http://wy.gzmigu.cn

[U21] Py：自定义上下文管理器
来源：http://cm.chemitech.net.cn

@contextlib.contextmanager
来源：http://vo.yuntaijiaju.cn

[U22] Py：矩阵转置
来源：http://nw.szsharing.cn

list(zip(*m))
来源：http://xi.jctech888.com.cn

[U23] Py：分块读取大文件
来源：http://nb.jianghongdianzi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jp.colortex.cn

[U24] Py：路径操作
来源：http://qn.haigaiapp.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nm.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://sf.huixiangedu.cn

csv.DictReader(f)
来源：http://tw.nicolike.cn

[U26] Py：并发下载
来源：http://mm.haigaiapp.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ck.yuexingan06.cn

[U27] Py：异步 HTTP
来源：http://hz.bookmarksfly.cn

aiohttp.ClientSession() 配合 async with
来源：http://cx.haigaiapp.cn

[U28] Py：类型别名
来源：http://as.bjjhwx.cn

UserId = int
来源：http://oy.shtwfgs.cn

[U29] Py：属性校验
来源：http://wc.huanxung.cn

@property 与 @x.setter 配合
来源：http://gu.newstarts.cn

[U30] Py：数据类
来源：http://ir.yuexingan06.cn

@dataclass(slots=True)
来源：http://zl.521024.cn

[U31] Py：单测
来源：http://lk.bjjhwx.cn

python -m pytest -q
来源：http://iy.yuntaijiaju.cn

[U32] Py：代码格式化
来源：http://kx.bookmarksfly.cn

ruff format . && ruff check --fix .
来源：http://tu.panjiajie.cn

[U33] Py：打包发布
来源：http://ah.gzmigu.cn

python -m build  （依赖 pyproject.toml）
来源：http://im.shxzukj.cn

[U34] Py：判断编码
来源：http://sk.hnjuh.cn

chardet.detect(raw)
来源：http://jg.wgjwhj.cn

[U35] Py：发送邮件
来源：http://ie.huixiangedu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gn.panjiajie.cn

[U36] Py：定时任务
来源：http://ee.panjiajie.cn

schedule.every(10).minutes.do(job)
来源：http://hi.shtwfgs.cn

[U37] Py：读写 Excel
来源：http://id.haigaiapp.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jv.huixinmuqiang.cn

[U38] Py：获取脚本所在目录
来源：http://jc.huixiangedu.cn

Path(__file__).resolve().parent
来源：http://ra.huanxung.cn

[U39] Py：判断是否在交互环境
来源：http://iw.newstarts.cn

sys.stdout.isatty()
来源：http://kb.shxzskj.cn

[U40] Py：打印到标准错误
来源：http://ft.hahajie.cn

print("err", file=sys.stderr)
来源：http://cz.huixinmuqiang.cn

[U41] PHP：初始化 Composer 项目
来源：http://bn.muxihuayi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://wn.shxzukj.cn

[U42] PHP：PSR-4 自动加载
来源：http://lp.shxzukj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gf.jctech888.com.cn

[U43] PHP：声明命名空间
来源：http://ox.gzmigu.cn

namespace App\Http;
来源：http://eq.szxytkj.cn

[U44] PHP：开启严格类型
来源：http://is.yuexingan06.cn

declare(strict_types=1);
来源：http://ah.wgjwhj.cn

[U45] PHP：类型声明与返回类型
来源：http://dg.hnjuh.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://pf.gzmigu.cn

[U46] PHP：可空类型
来源：http://ha.shxzskj.cn

?string $name = null
来源：http://ez.jctech888.com.cn

[U47] PHP：联合类型
来源：http://jy.szsharing.cn

int|string $id
来源：http://ej.nicolike.cn

[U48] PHP：纯枚举
来源：http://er.shxzskj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tf.szxytkj.cn

[U49] PHP：只读属性
来源：http://vk.hahajie.cn

public readonly string $name
来源：http://nl.9csxet.cn

[U50] PHP：构造器属性提升
来源：http://om.szsharing.cn

public function __construct(private int $id) {}
来源：http://uj.muxihuayi.cn

[U51] PHP：数组解构
来源：http://ct.newstarts.cn

[$a, $b] = $arr;
来源：http://qt.hnjuh.cn

[U52] PHP：箭头函数
来源：http://pp.hnjuh.cn

$double = fn($x) => $x * 2;
来源：http://lh.haigaiapp.cn

[U53] PHP：空合并运算符
来源：http://ll.szxytkj.cn

$v = $a ?? $b ?? "default";
来源：http://oq.bookmarksfly.cn

[U54] PHP：空安全调用
来源：http://xc.huixinmuqiang.cn

$obj?->method()
来源：http://ws.huanxung.cn

[U55] PHP：match 表达式
来源：http://vj.colortex.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://as.shxzukj.cn

[U56] PHP：命名参数
来源：http://aw.huixiangedu.cn

f(a: 1, b: 2)
来源：http://mo.nszjky.cn

[U57] PHP：字符串插值
来源：http://yb.bjjhwx.cn

"值: {$a}"
来源：http://dx.bjjhwx.cn

[U58] PHP：数组三件套
来源：http://ok.yuntaijiaju.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ve.shtwfgs.cn

[U59] PHP：自定义排序
来源：http://mg.newstarts.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jc.9csxet.cn

[U60] PHP：JSON 编解码
来源：http://la.jctech888.com.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vv.colortex.cn

[U61] PHP：正则
来源：http://lq.hahajie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://iw.gzmigu.cn

[U62] PHP：日期对象
来源：http://yf.asd995.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kt.521024.cn

[U63] PHP：文件读写
来源：http://ty.chemitech.net.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sy.9csxet.cn

[U64] PHP：目录遍历
来源：http://uj.lnxyls.cn

glob("dir/*.php");  scandir("dir");
来源：http://hi.huanxung.cn

[U65] PHP：会话
来源：http://jj.colortex.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://wb.nszjky.cn

[U66] PHP：设置 Cookie
来源：http://ya.wgjwhj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nk.jianghongdianzi.cn

[U67] PHP：处理文件上传
来源：http://ri.yuexingan06.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zl.shtwfgs.cn

[U68] PHP：PDO 连接
来源：http://wg.521024.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://oo.chemitech.net.cn

[U69] PHP：PDO 预处理
来源：http://cg.colortex.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tm.nszjky.cn

[U70] PHP：PDO 事务
来源：http://vx.bjjhwx.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ch.huixinmuqiang.cn

[U71] PHP：抛出异常
来源：http://dr.bjjhwx.cn

throw new RuntimeException("失败", 500);
来源：http://di.panjiajie.cn

[U72] PHP：写错误日志
来源：http://ss.jianghongdianzi.cn

error_log("失败: " . $e->getMessage());
来源：http://nq.huixinmuqiang.cn

[U73] PHP：读取 ini 配置
来源：http://xo.lnxyls.cn

parse_ini_file("config.ini", true)
来源：http://qu.jctech888.com.cn

[U74] PHP：读取环境变量
来源：http://zt.szsharing.cn

getenv("APP_ENV") ?: "production"
来源：http://az.szxytkj.cn

[U75] PHP：依赖注入
来源：http://ao.yuexingan06.cn

composer require psr/container
来源：http://ti.bookmarksfly.cn

[U76] PHP：简单路由
来源：http://dp.shtwfgs.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kx.shxzukj.cn

[U77] PHP：模板渲染
来源：http://nm.521024.cn

composer require twig/twig
来源：http://wv.gzmigu.cn

[U78] PHP：单元测试
来源：http://nr.gzmigu.cn

composer require --dev phpunit/phpunit
来源：http://nj.panjiajie.cn

[U79] PHP：静态分析
来源：http://po.szxytkj.cn

composer require --dev phpstan/phpstan
来源：http://hg.huixinmuqiang.cn

[U80] PHP：代码规范修复
来源：http://ug.huixiangedu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://id.szxytkj.cn

[U81] JS：初始化项目
来源：http://ky.bjjhwx.cn

npm init -y;  npm i express
来源：http://vm.yuntaijiaju.cn

[U82] JS：package.json 脚本
来源：http://vm.hahajie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jt.chemitech.net.cn

[U83] JS：ES Module 导入导出
来源：http://ih.bjjhwx.cn

export const a = 1;  import { a } from "./m.js";
来源：http://fg.lnxyls.cn

[U84] JS：CommonJS 写法
来源：http://gp.jianghongdianzi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wt.shxzukj.cn

[U85] JS：可选链
来源：http://fe.wgjwhj.cn

a?.b?.c
来源：http://dy.shtwfgs.cn

[U86] JS：空值合并
来源：http://wj.nicolike.cn

a ?? b
来源：http://cb.nicolike.cn

[U87] JS：解构默认值
来源：http://af.shtwfgs.cn

const { a = 1, b = 2 } = obj;
来源：http://ix.jianghongdianzi.cn

[U88] JS：对象展开合并
来源：http://vo.nicolike.cn

{ ...a, ...b }
来源：http://ht.yuntaijiaju.cn

[U89] JS：数组去重
来源：http://as.muxihuayi.cn

[...new Set(arr)]
来源：http://pf.newstarts.cn

[U90] JS：数字数组排序
来源：http://sx.gzmigu.cn

[...arr].sort((a, b) => a - b)
来源：http://mb.9csxet.cn

[U91] JS：对象键值遍历
来源：http://gn.yuexingan06.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gu.jianghongdianzi.cn

[U92] JS：深拷贝
来源：http://fh.haigaiapp.cn

structuredClone(obj)
来源：http://dp.szxytkj.cn

[U93] JS：模板字符串
来源：http://yz.bookmarksfly.cn

`共 ${n} 条`
来源：http://ni.9csxet.cn

[U94] JS：箭头函数
来源：http://qx.nszjky.cn

const double = x => x * 2;
来源：http://kc.haigaiapp.cn

[U95] JS：Promise 包装
来源：http://el.hahajie.cn

new Promise((resolve, reject) => {})
来源：http://fi.shxzukj.cn

[U96] JS：async/await 与异常
来源：http://je.jctech888.com.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xf.yuntaijiaju.cn

[U97] JS：并发请求
来源：http://mp.jianghongdianzi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ca.hnjuh.cn

[U98] JS：fetch 带 JSON
来源：http://ru.panjiajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://oe.gzmigu.cn

[U99] JS：事件监听
来源：http://bx.nicolike.cn

el.addEventListener("click", e => {})
来源：http://be.bookmarksfly.cn

[U100] JS：DOM 查询
来源：http://bo.521024.cn

document.querySelector(".item")
来源：http://qf.bjjhwx.cn

[U101] JS：classList 操作
来源：http://ql.huixinmuqiang.cn

el.classList.toggle("active")
来源：http://ju.shxzukj.cn

[U102] JS：本地存储
来源：http://ia.nszjky.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ya.shtwfgs.cn

[U103] JS：定时器
来源：http://qa.yuntaijiaju.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vu.nszjky.cn

[U104] JS：防抖
来源：http://cb.asd995.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tm.szxytkj.cn

[U105] JS：节流
来源：http://ey.yuexingan06.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fx.hnjuh.cn

[U106] JS：日期格式化
来源：http://iw.bookmarksfly.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qe.wgjwhj.cn

[U107] JS：数字千分位
来源：http://jk.nszjky.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wk.nicolike.cn

[U108] JS：随机整数
来源：http://ul.shxzskj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ar.yuexingan06.cn

[U109] JS：数组分组
来源：http://dh.lnxyls.cn

Object.groupBy(arr, x => x.type)
来源：http://pt.muxihuayi.cn

[U110] JS：数组分块
来源：http://yz.chemitech.net.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jl.chemitech.net.cn

[U111] JS：对象转 Map
来源：http://gj.yuexingan06.cn

new Map(Object.entries(obj))
来源：http://pr.newstarts.cn

[U112] JS：字符串补位
来源：http://lc.szxytkj.cn

"7".padStart(3, "0")
来源：http://tu.muxihuayi.cn

[U113] JS：正则替换全部
来源：http://mx.huixinmuqiang.cn

s.replaceAll("a", "b")
来源：http://ja.nszjky.cn

[U114] JS：JSON 深比较
来源：http://in.jianghongdianzi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://lu.haigaiapp.cn

[U115] JS：生成 UUID
来源：http://es.szxytkj.cn

crypto.randomUUID()
来源：http://hk.szsharing.cn

[U116] JS：类型检查（JSDoc）
来源：http://js.lnxyls.cn

/** @param {string} name */ function f(name) {}
来源：http://wm.szxytkj.cn

[U117] JS：单元测试
来源：http://ox.shxzukj.cn

npm i -D vitest;  npx vitest
来源：http://fc.shxzukj.cn

[U118] JS：开发服务器
来源：http://te.asd995.cn

npm i -D vite;  npx vite
来源：http://mb.nszjky.cn

[U119] JS：生产构建
来源：http://qb.bjjhwx.cn

npx vite build
来源：http://ow.wgjwhj.cn

[U120] JS：读取环境变量（Vite）
来源：http://kt.huixinmuqiang.cn

import.meta.env.VITE_API_URL
来源：http://gz.jctech888.com.cn

================================================================================
来源：http://ka.yuntaijiaju.cn

统计汇总
来源：http://gt.asd995.cn

================================================================================
来源：http://xg.muxihuayi.cn

按语言统计（条）：
来源：http://pr.nicolike.cn

Python ......... 252
来源：http://vt.chemitech.net.cn

PHP ............ 252
来源：http://rk.muxihuayi.cn

JavaScript ..... 252
来源：http://yc.wgjwhj.cn

TypeScript ..... 212
来源：http://hm.nszjky.cn

Java ........... 212
来源：http://qb.nicolike.cn

Go ............. 212
来源：http://qa.szxytkj.cn

Ruby ........... 212
来源：http://kp.nszjky.cn

C# ............. 212
来源：http://ae.9csxet.cn

C .............. 30
来源：http://zy.yuexingan06.cn

C++ ............ 30
来源：http://sk.huanxung.cn

SQL ............ 90
来源：http://do.jctech888.com.cn

Bash ........... 80
来源：http://yv.szsharing.cn


<!-- 参考信息 -->