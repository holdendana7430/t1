代发 wailian999

[T41] Perl：Hello World
来源：http://bz.panjiajie.cn

print "Hello\n";
来源：http://mz.yuexingan06.cn

[T42] Perl：变量类型
来源：http://yz.521024.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jc.521024.cn

[T43] Perl：字符串插值
来源：http://ki.nicolike.cn

"值: $a"
来源：http://dt.newstarts.cn

[T44] Perl：条件
来源：http://bt.hahajie.cn

if ($a > 0) { print "正"; }
来源：http://tv.shtwfgs.cn

[T45] Perl：数组遍历
来源：http://lr.jianghongdianzi.cn

for my $x (@arr) { print $x; }
来源：http://gd.wgjwhj.cn

[T46] Perl：哈希操作
来源：http://sl.nicolike.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jv.jctech888.com.cn

[T47] Perl：正则捕获
来源：http://qw.huanxung.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ly.shxzskj.cn

[T48] Perl：正则替换
来源：http://ft.yuntaijiaju.cn

$s =~ s/old/new/g;
来源：http://km.huanxung.cn

[T49] Perl：函数
来源：http://gb.nicolike.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zo.nszjky.cn

[T50] Perl：逐行读文件
来源：http://qf.asd995.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fe.asd995.cn

while (my $line = <$fh>) { print $line; }
来源：http://qb.shxzukj.cn

[T51] Scala：Hello World
来源：http://vj.521024.cn

println("Hello")
来源：http://lu.nicolike.cn

[T52] Scala：变量
来源：http://xq.chemitech.net.cn

val a = 1;  var b = 2
来源：http://oc.szsharing.cn

[T53] Scala：字符串插值
来源：http://rl.hahajie.cn

s"值: $b"
来源：http://ah.lnxyls.cn

[T54] Scala：集合映射
来源：http://eo.haigaiapp.cn

List(1, 2, 3).map(_ * 2)
来源：http://is.chemitech.net.cn

[T55] Scala：集合过滤
来源：http://ee.jianghongdianzi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://kq.bjjhwx.cn

[T56] Scala：样例类
来源：http://gm.huanxung.cn

case class User(name: String, age: Int)
来源：http://qg.9csxet.cn

[T57] Scala：模式匹配
来源：http://eo.szxytkj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wb.yuexingan06.cn

[T58] Scala：函数定义
来源：http://nk.jianghongdianzi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://xc.asd995.cn

[T59] Scala：循环
来源：http://sf.bjjhwx.cn

for (i <- 1 to 10) println(i)
来源：http://rf.hahajie.cn

[T60] Scala：折叠
来源：http://tm.wgjwhj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://er.hnjuh.cn

================================================================================
来源：http://lm.521024.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://er.muxihuayi.cn

================================================================================
来源：http://tz.colortex.cn

[U01] Py：创建虚拟环境
来源：http://qn.hahajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ec.shxzskj.cn

[U02] Py：导出 / 安装依赖
来源：http://yh.wgjwhj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zt.colortex.cn

[U03] Py：加载 .env 配置
来源：http://ew.521024.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ab.hahajie.cn

[U04] Py：变量调试打印
来源：http://hx.huixiangedu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ft.hahajie.cn

[U05] Py：列表去重且保序
来源：http://kn.yuntaijiaju.cn

list(dict.fromkeys(arr))
来源：http://tm.shxzukj.cn

[U06] Py：合并两个字典
来源：http://wg.chemitech.net.cn

{**a, **b}
来源：http://km.521024.cn

[U07] Py：反转字典键值
来源：http://ho.jianghongdianzi.cn

{v: k for k, v in d.items()}
来源：http://im.szxytkj.cn

[U08] Py：展平二维列表
来源：http://os.bookmarksfly.cn

[y for x in nested for y in x]
来源：http://uv.hnjuh.cn

[U09] Py：字典取最大值的键
来源：http://ux.521024.cn

max(d, key=d.get)
来源：http://wj.9csxet.cn

[U10] Py：按值排序字典
来源：http://za.colortex.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uh.jctech888.com.cn

[U11] Py：生成器表达式
来源：http://zt.huixinmuqiang.cn

(x * 2 for x in arr)
来源：http://fk.panjiajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qf.521024.cn

Counter(arr).most_common(3)
来源：http://py.huanxung.cn

[U13] Py：固定长度队列
来源：http://kx.shxzukj.cn

deque(maxlen=10)
来源：http://ui.gzmigu.cn

[U14] Py：分组收集到列表
来源：http://ty.huixiangedu.cn

defaultdict(list)
来源：http://zn.hahajie.cn

[U15] Py：高精度计时
来源：http://xe.chemitech.net.cn

t = time.perf_counter()
来源：http://zj.yuntaijiaju.cn

[U16] Py：命令行参数解析
来源：http://py.haigaiapp.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://df.huixinmuqiang.cn

[U17] Py：初始化日志
来源：http://jw.shxzskj.cn

logging.basicConfig(level=logging.INFO)
来源：http://vd.shxzukj.cn

[U18] Py：预编译正则
来源：http://vh.521024.cn

pat = re.compile(r"\d+")
来源：http://ac.hnjuh.cn

[U19] Py：正则替换带回调
来源：http://oy.bookmarksfly.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fp.shxzskj.cn

[U20] Py：缓存函数结果
来源：http://ab.bjjhwx.cn

@functools.lru_cache(maxsize=None)
来源：http://zx.huanxung.cn

[U21] Py：自定义上下文管理器
来源：http://ly.huixinmuqiang.cn

@contextlib.contextmanager
来源：http://yr.nicolike.cn

[U22] Py：矩阵转置
来源：http://qr.colortex.cn

list(zip(*m))
来源：http://bc.bookmarksfly.cn

[U23] Py：分块读取大文件
来源：http://ki.wgjwhj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ds.shtwfgs.cn

[U24] Py：路径操作
来源：http://mj.gzmigu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vq.gzmigu.cn

[U25] Py：CSV 按字典读
来源：http://ou.jctech888.com.cn

csv.DictReader(f)
来源：http://is.jianghongdianzi.cn

[U26] Py：并发下载
来源：http://ph.huixiangedu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ta.gzmigu.cn

[U27] Py：异步 HTTP
来源：http://hz.panjiajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://tv.jianghongdianzi.cn

[U28] Py：类型别名
来源：http://hz.szxytkj.cn

UserId = int
来源：http://ac.colortex.cn

[U29] Py：属性校验
来源：http://sw.bookmarksfly.cn

@property 与 @x.setter 配合
来源：http://ko.bookmarksfly.cn

[U30] Py：数据类
来源：http://ki.yuntaijiaju.cn

@dataclass(slots=True)
来源：http://gl.nszjky.cn

[U31] Py：单测
来源：http://az.jianghongdianzi.cn

python -m pytest -q
来源：http://wx.asd995.cn

[U32] Py：代码格式化
来源：http://xo.lnxyls.cn

ruff format . && ruff check --fix .
来源：http://az.huanxung.cn

[U33] Py：打包发布
来源：http://nb.hnjuh.cn

python -m build  （依赖 pyproject.toml）
来源：http://og.huanxung.cn

[U34] Py：判断编码
来源：http://sw.chemitech.net.cn

chardet.detect(raw)
来源：http://ax.bookmarksfly.cn

[U35] Py：发送邮件
来源：http://en.nicolike.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dd.hnjuh.cn

[U36] Py：定时任务
来源：http://jx.huanxung.cn

schedule.every(10).minutes.do(job)
来源：http://ul.huixinmuqiang.cn

[U37] Py：读写 Excel
来源：http://ez.panjiajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://uk.colortex.cn

[U38] Py：获取脚本所在目录
来源：http://mr.wgjwhj.cn

Path(__file__).resolve().parent
来源：http://ex.szsharing.cn

[U39] Py：判断是否在交互环境
来源：http://xk.panjiajie.cn

sys.stdout.isatty()
来源：http://qa.521024.cn

[U40] Py：打印到标准错误
来源：http://ca.jianghongdianzi.cn

print("err", file=sys.stderr)
来源：http://cm.muxihuayi.cn

[U41] PHP：初始化 Composer 项目
来源：http://vs.jianghongdianzi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zu.bjjhwx.cn

[U42] PHP：PSR-4 自动加载
来源：http://ba.huanxung.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vt.jianghongdianzi.cn

[U43] PHP：声明命名空间
来源：http://cj.huixinmuqiang.cn

namespace App\Http;
来源：http://wo.hahajie.cn

[U44] PHP：开启严格类型
来源：http://zl.shtwfgs.cn

declare(strict_types=1);
来源：http://ki.bjjhwx.cn

[U45] PHP：类型声明与返回类型
来源：http://ii.gzmigu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ge.muxihuayi.cn

[U46] PHP：可空类型
来源：http://pb.asd995.cn

?string $name = null
来源：http://hg.jianghongdianzi.cn

[U47] PHP：联合类型
来源：http://hp.shxzukj.cn

int|string $id
来源：http://he.shtwfgs.cn

[U48] PHP：纯枚举
来源：http://zy.521024.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cd.hahajie.cn

[U49] PHP：只读属性
来源：http://au.muxihuayi.cn

public readonly string $name
来源：http://eb.jianghongdianzi.cn

[U50] PHP：构造器属性提升
来源：http://sc.bookmarksfly.cn

public function __construct(private int $id) {}
来源：http://ks.colortex.cn

[U51] PHP：数组解构
来源：http://vo.shxzukj.cn

[$a, $b] = $arr;
来源：http://rk.huixiangedu.cn

[U52] PHP：箭头函数
来源：http://zu.yuexingan06.cn

$double = fn($x) => $x * 2;
来源：http://hy.hahajie.cn

[U53] PHP：空合并运算符
来源：http://jh.hahajie.cn

$v = $a ?? $b ?? "default";
来源：http://da.nicolike.cn

[U54] PHP：空安全调用
来源：http://yl.szxytkj.cn

$obj?->method()
来源：http://fa.yuexingan06.cn

[U55] PHP：match 表达式
来源：http://qp.haigaiapp.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ms.huixinmuqiang.cn

[U56] PHP：命名参数
来源：http://ir.9csxet.cn

f(a: 1, b: 2)
来源：http://zq.521024.cn

[U57] PHP：字符串插值
来源：http://dv.nicolike.cn

"值: {$a}"
来源：http://ja.szsharing.cn

[U58] PHP：数组三件套
来源：http://mo.muxihuayi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://am.szxytkj.cn

[U59] PHP：自定义排序
来源：http://ka.shxzukj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ra.haigaiapp.cn

[U60] PHP：JSON 编解码
来源：http://bh.521024.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ug.bjjhwx.cn

[U61] PHP：正则
来源：http://aq.szsharing.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qs.gzmigu.cn

[U62] PHP：日期对象
来源：http://je.hnjuh.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gt.huixiangedu.cn

[U63] PHP：文件读写
来源：http://qa.szxytkj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ei.asd995.cn

[U64] PHP：目录遍历
来源：http://th.jianghongdianzi.cn

glob("dir/*.php");  scandir("dir");
来源：http://zt.panjiajie.cn

[U65] PHP：会话
来源：http://xo.huixinmuqiang.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vl.lnxyls.cn

[U66] PHP：设置 Cookie
来源：http://cv.szsharing.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xp.szsharing.cn

[U67] PHP：处理文件上传
来源：http://pc.yuntaijiaju.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kd.9csxet.cn

[U68] PHP：PDO 连接
来源：http://by.lnxyls.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pb.huixinmuqiang.cn

[U69] PHP：PDO 预处理
来源：http://zt.jianghongdianzi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ud.szxytkj.cn

[U70] PHP：PDO 事务
来源：http://id.colortex.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nf.shtwfgs.cn

[U71] PHP：抛出异常
来源：http://vu.huanxung.cn

throw new RuntimeException("失败", 500);
来源：http://rb.shxzukj.cn

[U72] PHP：写错误日志
来源：http://rc.szxytkj.cn

error_log("失败: " . $e->getMessage());
来源：http://io.gzmigu.cn

[U73] PHP：读取 ini 配置
来源：http://ak.yuexingan06.cn

parse_ini_file("config.ini", true)
来源：http://io.nszjky.cn

[U74] PHP：读取环境变量
来源：http://ry.szsharing.cn

getenv("APP_ENV") ?: "production"
来源：http://jx.wgjwhj.cn

[U75] PHP：依赖注入
来源：http://qd.panjiajie.cn

composer require psr/container
来源：http://ih.huixiangedu.cn

[U76] PHP：简单路由
来源：http://kw.9csxet.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nr.hnjuh.cn

[U77] PHP：模板渲染
来源：http://gu.yuexingan06.cn

composer require twig/twig
来源：http://qm.muxihuayi.cn

[U78] PHP：单元测试
来源：http://td.asd995.cn

composer require --dev phpunit/phpunit
来源：http://xt.gzmigu.cn

[U79] PHP：静态分析
来源：http://wu.shxzskj.cn

composer require --dev phpstan/phpstan
来源：http://hh.9csxet.cn

[U80] PHP：代码规范修复
来源：http://mp.bookmarksfly.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ym.hnjuh.cn

[U81] JS：初始化项目
来源：http://zr.muxihuayi.cn

npm init -y;  npm i express
来源：http://dr.yuntaijiaju.cn

[U82] JS：package.json 脚本
来源：http://ac.jianghongdianzi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ew.shtwfgs.cn

[U83] JS：ES Module 导入导出
来源：http://ih.jctech888.com.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vo.jianghongdianzi.cn

[U84] JS：CommonJS 写法
来源：http://oy.huixiangedu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://pv.yuntaijiaju.cn

[U85] JS：可选链
来源：http://dz.chemitech.net.cn

a?.b?.c
来源：http://rx.haigaiapp.cn

[U86] JS：空值合并
来源：http://ai.bjjhwx.cn

a ?? b
来源：http://wf.shxzskj.cn

[U87] JS：解构默认值
来源：http://pr.newstarts.cn

const { a = 1, b = 2 } = obj;
来源：http://ca.gzmigu.cn

[U88] JS：对象展开合并
来源：http://zx.9csxet.cn

{ ...a, ...b }
来源：http://sa.panjiajie.cn

[U89] JS：数组去重
来源：http://zq.huixinmuqiang.cn

[...new Set(arr)]
来源：http://ce.nszjky.cn

[U90] JS：数字数组排序
来源：http://ua.colortex.cn

[...arr].sort((a, b) => a - b)
来源：http://jt.chemitech.net.cn

[U91] JS：对象键值遍历
来源：http://wm.yuntaijiaju.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fp.hnjuh.cn

[U92] JS：深拷贝
来源：http://ru.szsharing.cn

structuredClone(obj)
来源：http://fq.521024.cn

[U93] JS：模板字符串
来源：http://ic.haigaiapp.cn

`共 ${n} 条`
来源：http://mq.colortex.cn

[U94] JS：箭头函数
来源：http://fi.muxihuayi.cn

const double = x => x * 2;
来源：http://ee.hahajie.cn

[U95] JS：Promise 包装
来源：http://bk.wgjwhj.cn

new Promise((resolve, reject) => {})
来源：http://mm.colortex.cn

[U96] JS：async/await 与异常
来源：http://aq.huanxung.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nr.huanxung.cn

[U97] JS：并发请求
来源：http://se.hahajie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ze.shtwfgs.cn

[U98] JS：fetch 带 JSON
来源：http://ex.newstarts.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tf.panjiajie.cn

[U99] JS：事件监听
来源：http://re.szsharing.cn

el.addEventListener("click", e => {})
来源：http://vu.bjjhwx.cn

[U100] JS：DOM 查询
来源：http://yk.asd995.cn

document.querySelector(".item")
来源：http://tq.shxzskj.cn

[U101] JS：classList 操作
来源：http://ph.nicolike.cn

el.classList.toggle("active")
来源：http://ek.huanxung.cn

[U102] JS：本地存储
来源：http://qr.bjjhwx.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://rq.colortex.cn

[U103] JS：定时器
来源：http://mh.nicolike.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ad.yuexingan06.cn

[U104] JS：防抖
来源：http://or.huanxung.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sv.yuntaijiaju.cn

[U105] JS：节流
来源：http://ks.521024.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qx.shxzskj.cn

[U106] JS：日期格式化
来源：http://yk.colortex.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ss.szsharing.cn

[U107] JS：数字千分位
来源：http://nf.yuexingan06.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nm.huanxung.cn

[U108] JS：随机整数
来源：http://ia.lnxyls.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yk.szsharing.cn

[U109] JS：数组分组
来源：http://yx.panjiajie.cn

Object.groupBy(arr, x => x.type)
来源：http://uz.muxihuayi.cn

[U110] JS：数组分块
来源：http://ne.colortex.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lh.huixiangedu.cn

[U111] JS：对象转 Map
来源：http://gi.wgjwhj.cn

new Map(Object.entries(obj))
来源：http://zu.haigaiapp.cn

[U112] JS：字符串补位
来源：http://ji.bookmarksfly.cn

"7".padStart(3, "0")
来源：http://bb.muxihuayi.cn

[U113] JS：正则替换全部
来源：http://ry.lnxyls.cn

s.replaceAll("a", "b")
来源：http://nx.shxzskj.cn

[U114] JS：JSON 深比较
来源：http://ap.panjiajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://av.yuntaijiaju.cn

[U115] JS：生成 UUID
来源：http://sy.bjjhwx.cn

crypto.randomUUID()
来源：http://nl.shxzukj.cn

[U116] JS：类型检查（JSDoc）
来源：http://ii.huanxung.cn

/** @param {string} name */ function f(name) {}
来源：http://id.wgjwhj.cn

[U117] JS：单元测试
来源：http://fu.nszjky.cn

npm i -D vitest;  npx vitest
来源：http://sw.hahajie.cn

[U118] JS：开发服务器
来源：http://sl.gzmigu.cn

npm i -D vite;  npx vite
来源：http://yt.huixinmuqiang.cn

[U119] JS：生产构建
来源：http://fm.gzmigu.cn

npx vite build
来源：http://yn.muxihuayi.cn

[U120] JS：读取环境变量（Vite）
来源：http://nv.shtwfgs.cn

import.meta.env.VITE_API_URL
来源：http://xq.asd995.cn

================================================================================
来源：http://pr.huixiangedu.cn

统计汇总
来源：http://lz.huanxung.cn

================================================================================
来源：http://ts.9csxet.cn

按语言统计（条）：
来源：http://yr.lnxyls.cn

Python ......... 252
来源：http://ji.huixinmuqiang.cn

PHP ............ 252
来源：http://ys.szsharing.cn

JavaScript ..... 252
来源：http://om.gzmigu.cn

TypeScript ..... 212
来源：http://uz.huixiangedu.cn

Java ........... 212
来源：http://xy.bookmarksfly.cn

Go ............. 212
来源：http://at.jctech888.com.cn

Ruby ........... 212
来源：http://tw.gzmigu.cn

C# ............. 212
来源：http://oh.nicolike.cn

C .............. 30
来源：http://bd.huixinmuqiang.cn

C++ ............ 30
来源：http://bw.colortex.cn

SQL ............ 90
来源：http://bg.hnjuh.cn

Bash ........... 80
来源：http://zy.lnxyls.cn


<!-- 参考信息 -->