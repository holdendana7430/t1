代发 wailian999

[T41] Perl：Hello World
来源：http://hd.nicolike.cn

print "Hello\n";
来源：http://bk.hnjuh.cn

[T42] Perl：变量类型
来源：http://jp.huixiangedu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://om.jctech888.com.cn

[T43] Perl：字符串插值
来源：http://do.9csxet.cn

"值: $a"
来源：http://tl.9csxet.cn

[T44] Perl：条件
来源：http://ut.yuexingan06.cn

if ($a > 0) { print "正"; }
来源：http://uc.shtwfgs.cn

[T45] Perl：数组遍历
来源：http://wi.szxytkj.cn

for my $x (@arr) { print $x; }
来源：http://ln.hnjuh.cn

[T46] Perl：哈希操作
来源：http://fl.nszjky.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://na.lnxyls.cn

[T47] Perl：正则捕获
来源：http://pk.nszjky.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://bz.wgjwhj.cn

[T48] Perl：正则替换
来源：http://ou.9csxet.cn

$s =~ s/old/new/g;
来源：http://hl.nicolike.cn

[T49] Perl：函数
来源：http://xp.yuexingan06.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mh.yuntaijiaju.cn

[T50] Perl：逐行读文件
来源：http://jf.bjjhwx.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ga.bookmarksfly.cn

while (my $line = <$fh>) { print $line; }
来源：http://pj.9csxet.cn

[T51] Scala：Hello World
来源：http://rt.asd995.cn

println("Hello")
来源：http://ao.huanxung.cn

[T52] Scala：变量
来源：http://ta.haigaiapp.cn

val a = 1;  var b = 2
来源：http://gi.nszjky.cn

[T53] Scala：字符串插值
来源：http://gy.jianghongdianzi.cn

s"值: $b"
来源：http://fx.shxzskj.cn

[T54] Scala：集合映射
来源：http://gj.chemitech.net.cn

List(1, 2, 3).map(_ * 2)
来源：http://gk.bjjhwx.cn

[T55] Scala：集合过滤
来源：http://wv.wgjwhj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://nz.huixiangedu.cn

[T56] Scala：样例类
来源：http://xr.9csxet.cn

case class User(name: String, age: Int)
来源：http://dz.muxihuayi.cn

[T57] Scala：模式匹配
来源：http://md.bookmarksfly.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://uh.muxihuayi.cn

[T58] Scala：函数定义
来源：http://eq.jctech888.com.cn

def add(a: Int, b: Int): Int = a + b
来源：http://cq.huanxung.cn

[T59] Scala：循环
来源：http://ct.haigaiapp.cn

for (i <- 1 to 10) println(i)
来源：http://tw.gzmigu.cn

[T60] Scala：折叠
来源：http://ki.colortex.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zm.huixiangedu.cn

================================================================================
来源：http://vq.nszjky.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jm.bjjhwx.cn

================================================================================
来源：http://ej.wgjwhj.cn

[U01] Py：创建虚拟环境
来源：http://zh.jctech888.com.cn

python -m venv .venv && source .venv/bin/activate
来源：http://rw.bookmarksfly.cn

[U02] Py：导出 / 安装依赖
来源：http://xy.huixinmuqiang.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ir.panjiajie.cn

[U03] Py：加载 .env 配置
来源：http://xc.shtwfgs.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://cl.yuntaijiaju.cn

[U04] Py：变量调试打印
来源：http://tn.huanxung.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zt.9csxet.cn

[U05] Py：列表去重且保序
来源：http://qp.bjjhwx.cn

list(dict.fromkeys(arr))
来源：http://qh.yuntaijiaju.cn

[U06] Py：合并两个字典
来源：http://pi.521024.cn

{**a, **b}
来源：http://wd.muxihuayi.cn

[U07] Py：反转字典键值
来源：http://xs.szxytkj.cn

{v: k for k, v in d.items()}
来源：http://bp.shtwfgs.cn

[U08] Py：展平二维列表
来源：http://du.nszjky.cn

[y for x in nested for y in x]
来源：http://fa.wgjwhj.cn

[U09] Py：字典取最大值的键
来源：http://fj.newstarts.cn

max(d, key=d.get)
来源：http://eo.chemitech.net.cn

[U10] Py：按值排序字典
来源：http://ik.lnxyls.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mc.colortex.cn

[U11] Py：生成器表达式
来源：http://fq.shtwfgs.cn

(x * 2 for x in arr)
来源：http://ar.nicolike.cn

[U12] Py：取出现最多的 3 个元素
来源：http://aa.chemitech.net.cn

Counter(arr).most_common(3)
来源：http://jr.colortex.cn

[U13] Py：固定长度队列
来源：http://oq.muxihuayi.cn

deque(maxlen=10)
来源：http://ab.shtwfgs.cn

[U14] Py：分组收集到列表
来源：http://ns.asd995.cn

defaultdict(list)
来源：http://xt.9csxet.cn

[U15] Py：高精度计时
来源：http://ku.jctech888.com.cn

t = time.perf_counter()
来源：http://jg.huanxung.cn

[U16] Py：命令行参数解析
来源：http://dp.muxihuayi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://da.nicolike.cn

[U17] Py：初始化日志
来源：http://ny.nszjky.cn

logging.basicConfig(level=logging.INFO)
来源：http://qm.shxzskj.cn

[U18] Py：预编译正则
来源：http://qf.muxihuayi.cn

pat = re.compile(r"\d+")
来源：http://gf.nicolike.cn

[U19] Py：正则替换带回调
来源：http://un.muxihuayi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ik.gzmigu.cn

[U20] Py：缓存函数结果
来源：http://dc.newstarts.cn

@functools.lru_cache(maxsize=None)
来源：http://wy.jctech888.com.cn

[U21] Py：自定义上下文管理器
来源：http://bc.shxzskj.cn

@contextlib.contextmanager
来源：http://ue.gzmigu.cn

[U22] Py：矩阵转置
来源：http://kg.shtwfgs.cn

list(zip(*m))
来源：http://wi.shtwfgs.cn

[U23] Py：分块读取大文件
来源：http://sf.shxzskj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vb.colortex.cn

[U24] Py：路径操作
来源：http://zs.gzmigu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ab.hahajie.cn

[U25] Py：CSV 按字典读
来源：http://ou.asd995.cn

csv.DictReader(f)
来源：http://lf.yuntaijiaju.cn

[U26] Py：并发下载
来源：http://wp.asd995.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bz.huanxung.cn

[U27] Py：异步 HTTP
来源：http://nb.huixiangedu.cn

aiohttp.ClientSession() 配合 async with
来源：http://rh.jctech888.com.cn

[U28] Py：类型别名
来源：http://ja.521024.cn

UserId = int
来源：http://yn.nszjky.cn

[U29] Py：属性校验
来源：http://me.gzmigu.cn

@property 与 @x.setter 配合
来源：http://hf.shxzukj.cn

[U30] Py：数据类
来源：http://af.asd995.cn

@dataclass(slots=True)
来源：http://qw.hahajie.cn

[U31] Py：单测
来源：http://cp.nicolike.cn

python -m pytest -q
来源：http://td.521024.cn

[U32] Py：代码格式化
来源：http://nn.lnxyls.cn

ruff format . && ruff check --fix .
来源：http://mw.shtwfgs.cn

[U33] Py：打包发布
来源：http://aw.bookmarksfly.cn

python -m build  （依赖 pyproject.toml）
来源：http://ka.newstarts.cn

[U34] Py：判断编码
来源：http://og.shxzskj.cn

chardet.detect(raw)
来源：http://xc.9csxet.cn

[U35] Py：发送邮件
来源：http://zd.gzmigu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jb.yuntaijiaju.cn

[U36] Py：定时任务
来源：http://ky.muxihuayi.cn

schedule.every(10).minutes.do(job)
来源：http://ds.jianghongdianzi.cn

[U37] Py：读写 Excel
来源：http://hb.521024.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ax.jctech888.com.cn

[U38] Py：获取脚本所在目录
来源：http://gh.colortex.cn

Path(__file__).resolve().parent
来源：http://ed.colortex.cn

[U39] Py：判断是否在交互环境
来源：http://lo.yuntaijiaju.cn

sys.stdout.isatty()
来源：http://sj.521024.cn

[U40] Py：打印到标准错误
来源：http://ln.hahajie.cn

print("err", file=sys.stderr)
来源：http://dl.shtwfgs.cn

[U41] PHP：初始化 Composer 项目
来源：http://pp.shtwfgs.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://pj.hnjuh.cn

[U42] PHP：PSR-4 自动加载
来源：http://ak.szsharing.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ox.jianghongdianzi.cn

[U43] PHP：声明命名空间
来源：http://rk.huixiangedu.cn

namespace App\Http;
来源：http://fp.shxzukj.cn

[U44] PHP：开启严格类型
来源：http://an.hahajie.cn

declare(strict_types=1);
来源：http://mz.521024.cn

[U45] PHP：类型声明与返回类型
来源：http://lq.jctech888.com.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://xf.nszjky.cn

[U46] PHP：可空类型
来源：http://lh.huixinmuqiang.cn

?string $name = null
来源：http://ml.gzmigu.cn

[U47] PHP：联合类型
来源：http://st.shtwfgs.cn

int|string $id
来源：http://gg.huanxung.cn

[U48] PHP：纯枚举
来源：http://ey.shxzukj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lh.jianghongdianzi.cn

[U49] PHP：只读属性
来源：http://vh.nicolike.cn

public readonly string $name
来源：http://ca.yuexingan06.cn

[U50] PHP：构造器属性提升
来源：http://rk.huanxung.cn

public function __construct(private int $id) {}
来源：http://gc.chemitech.net.cn

[U51] PHP：数组解构
来源：http://am.asd995.cn

[$a, $b] = $arr;
来源：http://af.nicolike.cn

[U52] PHP：箭头函数
来源：http://wv.nszjky.cn

$double = fn($x) => $x * 2;
来源：http://ng.huixinmuqiang.cn

[U53] PHP：空合并运算符
来源：http://ox.asd995.cn

$v = $a ?? $b ?? "default";
来源：http://vo.shxzukj.cn

[U54] PHP：空安全调用
来源：http://dr.nicolike.cn

$obj?->method()
来源：http://wr.bjjhwx.cn

[U55] PHP：match 表达式
来源：http://ki.haigaiapp.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ni.bjjhwx.cn

[U56] PHP：命名参数
来源：http://uq.huixinmuqiang.cn

f(a: 1, b: 2)
来源：http://xi.panjiajie.cn

[U57] PHP：字符串插值
来源：http://hn.yuntaijiaju.cn

"值: {$a}"
来源：http://qd.yuntaijiaju.cn

[U58] PHP：数组三件套
来源：http://rq.hahajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cy.haigaiapp.cn

[U59] PHP：自定义排序
来源：http://cj.wgjwhj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yn.bjjhwx.cn

[U60] PHP：JSON 编解码
来源：http://lp.shtwfgs.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xv.wgjwhj.cn

[U61] PHP：正则
来源：http://nb.chemitech.net.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gn.521024.cn

[U62] PHP：日期对象
来源：http://si.lnxyls.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://at.shxzskj.cn

[U63] PHP：文件读写
来源：http://sq.shxzukj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://po.bjjhwx.cn

[U64] PHP：目录遍历
来源：http://qh.szsharing.cn

glob("dir/*.php");  scandir("dir");
来源：http://zw.asd995.cn

[U65] PHP：会话
来源：http://ys.521024.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://br.szxytkj.cn

[U66] PHP：设置 Cookie
来源：http://ax.szsharing.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zb.gzmigu.cn

[U67] PHP：处理文件上传
来源：http://hu.szsharing.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qo.yuexingan06.cn

[U68] PHP：PDO 连接
来源：http://mq.huixinmuqiang.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mj.szsharing.cn

[U69] PHP：PDO 预处理
来源：http://sh.colortex.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ik.521024.cn

[U70] PHP：PDO 事务
来源：http://hb.chemitech.net.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ds.wgjwhj.cn

[U71] PHP：抛出异常
来源：http://iq.huixinmuqiang.cn

throw new RuntimeException("失败", 500);
来源：http://ln.huanxung.cn

[U72] PHP：写错误日志
来源：http://hk.huixinmuqiang.cn

error_log("失败: " . $e->getMessage());
来源：http://wm.jianghongdianzi.cn

[U73] PHP：读取 ini 配置
来源：http://zc.huanxung.cn

parse_ini_file("config.ini", true)
来源：http://js.hahajie.cn

[U74] PHP：读取环境变量
来源：http://ns.shxzskj.cn

getenv("APP_ENV") ?: "production"
来源：http://il.haigaiapp.cn

[U75] PHP：依赖注入
来源：http://hh.huixinmuqiang.cn

composer require psr/container
来源：http://gi.newstarts.cn

[U76] PHP：简单路由
来源：http://oj.shtwfgs.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://db.shtwfgs.cn

[U77] PHP：模板渲染
来源：http://ur.shxzukj.cn

composer require twig/twig
来源：http://vf.bjjhwx.cn

[U78] PHP：单元测试
来源：http://hr.huixinmuqiang.cn

composer require --dev phpunit/phpunit
来源：http://zg.muxihuayi.cn

[U79] PHP：静态分析
来源：http://yl.521024.cn

composer require --dev phpstan/phpstan
来源：http://cm.bookmarksfly.cn

[U80] PHP：代码规范修复
来源：http://nu.bookmarksfly.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ym.bjjhwx.cn

[U81] JS：初始化项目
来源：http://jp.huixinmuqiang.cn

npm init -y;  npm i express
来源：http://wi.shxzukj.cn

[U82] JS：package.json 脚本
来源：http://ii.szsharing.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nl.panjiajie.cn

[U83] JS：ES Module 导入导出
来源：http://th.hahajie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://kw.szxytkj.cn

[U84] JS：CommonJS 写法
来源：http://dv.hahajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://gh.huixinmuqiang.cn

[U85] JS：可选链
来源：http://bn.huixiangedu.cn

a?.b?.c
来源：http://yf.lnxyls.cn

[U86] JS：空值合并
来源：http://vi.yuexingan06.cn

a ?? b
来源：http://yt.huanxung.cn

[U87] JS：解构默认值
来源：http://cq.bookmarksfly.cn

const { a = 1, b = 2 } = obj;
来源：http://uq.huanxung.cn

[U88] JS：对象展开合并
来源：http://ja.bookmarksfly.cn

{ ...a, ...b }
来源：http://ly.haigaiapp.cn

[U89] JS：数组去重
来源：http://fo.chemitech.net.cn

[...new Set(arr)]
来源：http://oe.shtwfgs.cn

[U90] JS：数字数组排序
来源：http://wa.haigaiapp.cn

[...arr].sort((a, b) => a - b)
来源：http://al.9csxet.cn

[U91] JS：对象键值遍历
来源：http://pm.jctech888.com.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ov.hahajie.cn

[U92] JS：深拷贝
来源：http://ct.muxihuayi.cn

structuredClone(obj)
来源：http://ww.jianghongdianzi.cn

[U93] JS：模板字符串
来源：http://sh.521024.cn

`共 ${n} 条`
来源：http://vu.haigaiapp.cn

[U94] JS：箭头函数
来源：http://pi.szsharing.cn

const double = x => x * 2;
来源：http://oe.haigaiapp.cn

[U95] JS：Promise 包装
来源：http://cn.newstarts.cn

new Promise((resolve, reject) => {})
来源：http://xp.nszjky.cn

[U96] JS：async/await 与异常
来源：http://oy.gzmigu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qy.gzmigu.cn

[U97] JS：并发请求
来源：http://er.huixinmuqiang.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bn.haigaiapp.cn

[U98] JS：fetch 带 JSON
来源：http://oy.huanxung.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ui.521024.cn

[U99] JS：事件监听
来源：http://vk.jctech888.com.cn

el.addEventListener("click", e => {})
来源：http://xk.panjiajie.cn

[U100] JS：DOM 查询
来源：http://fz.lnxyls.cn

document.querySelector(".item")
来源：http://mi.newstarts.cn

[U101] JS：classList 操作
来源：http://ys.muxihuayi.cn

el.classList.toggle("active")
来源：http://pv.hahajie.cn

[U102] JS：本地存储
来源：http://pe.huanxung.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://fw.haigaiapp.cn

[U103] JS：定时器
来源：http://gk.bjjhwx.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lp.jianghongdianzi.cn

[U104] JS：防抖
来源：http://we.hnjuh.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vj.szxytkj.cn

[U105] JS：节流
来源：http://gw.hahajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lf.jctech888.com.cn

[U106] JS：日期格式化
来源：http://cp.nicolike.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pj.gzmigu.cn

[U107] JS：数字千分位
来源：http://hy.jianghongdianzi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://he.9csxet.cn

[U108] JS：随机整数
来源：http://tk.shxzskj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://sr.muxihuayi.cn

[U109] JS：数组分组
来源：http://ga.huixiangedu.cn

Object.groupBy(arr, x => x.type)
来源：http://ny.shxzukj.cn

[U110] JS：数组分块
来源：http://kb.asd995.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ns.bjjhwx.cn

[U111] JS：对象转 Map
来源：http://uv.yuexingan06.cn

new Map(Object.entries(obj))
来源：http://av.muxihuayi.cn

[U112] JS：字符串补位
来源：http://yo.bookmarksfly.cn

"7".padStart(3, "0")
来源：http://vi.nszjky.cn

[U113] JS：正则替换全部
来源：http://rt.hnjuh.cn

s.replaceAll("a", "b")
来源：http://uc.9csxet.cn

[U114] JS：JSON 深比较
来源：http://zc.521024.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ri.huixiangedu.cn

[U115] JS：生成 UUID
来源：http://sc.shtwfgs.cn

crypto.randomUUID()
来源：http://yg.huixiangedu.cn

[U116] JS：类型检查（JSDoc）
来源：http://mx.panjiajie.cn

/** @param {string} name */ function f(name) {}
来源：http://nu.hnjuh.cn

[U117] JS：单元测试
来源：http://ir.jianghongdianzi.cn

npm i -D vitest;  npx vitest
来源：http://bx.bjjhwx.cn

[U118] JS：开发服务器
来源：http://jq.shtwfgs.cn

npm i -D vite;  npx vite
来源：http://cu.nszjky.cn

[U119] JS：生产构建
来源：http://ux.jctech888.com.cn

npx vite build
来源：http://sc.huixinmuqiang.cn

[U120] JS：读取环境变量（Vite）
来源：http://dk.asd995.cn

import.meta.env.VITE_API_URL
来源：http://zc.shxzskj.cn

================================================================================
来源：http://do.hnjuh.cn

统计汇总
来源：http://ss.9csxet.cn

================================================================================
来源：http://jw.chemitech.net.cn

按语言统计（条）：
来源：http://zg.jctech888.com.cn

Python ......... 252
来源：http://yr.huixiangedu.cn

PHP ............ 252
来源：http://ra.gzmigu.cn

JavaScript ..... 252
来源：http://pv.chemitech.net.cn

TypeScript ..... 212
来源：http://ss.szxytkj.cn

Java ........... 212
来源：http://hp.asd995.cn

Go ............. 212
来源：http://zq.chemitech.net.cn

Ruby ........... 212
来源：http://mb.bjjhwx.cn

C# ............. 212
来源：http://ur.chemitech.net.cn

C .............. 30
来源：http://jz.wgjwhj.cn

C++ ............ 30
来源：http://kv.huixinmuqiang.cn

SQL ............ 90
来源：http://ax.wgjwhj.cn

Bash ........... 80
来源：http://gn.nszjky.cn


<!-- 参考信息 -->