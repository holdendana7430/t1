代发 wailian999

[T43] Perl：字符串插值
来源：http://es.asd995.cn

"值: $a"
来源：http://ha.jianghongdianzi.cn

[T44] Perl：条件
来源：http://tb.asd995.cn

if ($a > 0) { print "正"; }
来源：http://sz.shxzukj.cn

[T45] Perl：数组遍历
来源：http://sl.wgjwhj.cn

for my $x (@arr) { print $x; }
来源：http://ht.gzmigu.cn

[T46] Perl：哈希操作
来源：http://vx.nicolike.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sp.yuntaijiaju.cn

[T47] Perl：正则捕获
来源：http://xg.muxihuayi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ta.nszjky.cn

[T48] Perl：正则替换
来源：http://tt.chemitech.net.cn

$s =~ s/old/new/g;
来源：http://bu.wgjwhj.cn

[T49] Perl：函数
来源：http://bk.jctech888.com.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ri.lnxyls.cn

[T50] Perl：逐行读文件
来源：http://va.shtwfgs.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://uh.huixiangedu.cn

while (my $line = <$fh>) { print $line; }
来源：http://ws.szsharing.cn

[T51] Scala：Hello World
来源：http://qi.521024.cn

println("Hello")
来源：http://np.newstarts.cn

[T52] Scala：变量
来源：http://ur.521024.cn

val a = 1;  var b = 2
来源：http://zv.newstarts.cn

[T53] Scala：字符串插值
来源：http://ip.yuntaijiaju.cn

s"值: $b"
来源：http://eq.nszjky.cn

[T54] Scala：集合映射
来源：http://mw.bjjhwx.cn

List(1, 2, 3).map(_ * 2)
来源：http://qs.shxzukj.cn

[T55] Scala：集合过滤
来源：http://wg.gzmigu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://cx.colortex.cn

[T56] Scala：样例类
来源：http://sy.9csxet.cn

case class User(name: String, age: Int)
来源：http://uk.lnxyls.cn

[T57] Scala：模式匹配
来源：http://rg.jianghongdianzi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://cl.huixinmuqiang.cn

[T58] Scala：函数定义
来源：http://eb.jctech888.com.cn

def add(a: Int, b: Int): Int = a + b
来源：http://nx.newstarts.cn

[T59] Scala：循环
来源：http://xs.panjiajie.cn

for (i <- 1 to 10) println(i)
来源：http://eo.szxytkj.cn

[T60] Scala：折叠
来源：http://sw.yuexingan06.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bm.jctech888.com.cn

================================================================================
来源：http://bs.yuntaijiaju.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://iu.szsharing.cn

================================================================================
来源：http://hn.huanxung.cn

[U01] Py：创建虚拟环境
来源：http://nc.szsharing.cn

python -m venv .venv && source .venv/bin/activate
来源：http://sb.colortex.cn

[U02] Py：导出 / 安装依赖
来源：http://ty.shtwfgs.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lx.yuntaijiaju.cn

[U03] Py：加载 .env 配置
来源：http://am.9csxet.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://io.szsharing.cn

[U04] Py：变量调试打印
来源：http://xx.lnxyls.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rx.asd995.cn

[U05] Py：列表去重且保序
来源：http://iv.shxzskj.cn

list(dict.fromkeys(arr))
来源：http://pw.lnxyls.cn

[U06] Py：合并两个字典
来源：http://sh.shtwfgs.cn

{**a, **b}
来源：http://ye.chemitech.net.cn

[U07] Py：反转字典键值
来源：http://xe.521024.cn

{v: k for k, v in d.items()}
来源：http://wd.colortex.cn

[U08] Py：展平二维列表
来源：http://ur.huanxung.cn

[y for x in nested for y in x]
来源：http://pn.wgjwhj.cn

[U09] Py：字典取最大值的键
来源：http://yg.haigaiapp.cn

max(d, key=d.get)
来源：http://kh.jctech888.com.cn

[U10] Py：按值排序字典
来源：http://zy.hnjuh.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jv.jianghongdianzi.cn

[U11] Py：生成器表达式
来源：http://vm.yuntaijiaju.cn

(x * 2 for x in arr)
来源：http://fj.muxihuayi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ou.hnjuh.cn

Counter(arr).most_common(3)
来源：http://zb.chemitech.net.cn

[U13] Py：固定长度队列
来源：http://zs.hnjuh.cn

deque(maxlen=10)
来源：http://ur.huixiangedu.cn

[U14] Py：分组收集到列表
来源：http://bp.yuexingan06.cn

defaultdict(list)
来源：http://dy.huixinmuqiang.cn

[U15] Py：高精度计时
来源：http://dm.wgjwhj.cn

t = time.perf_counter()
来源：http://sz.chemitech.net.cn

[U16] Py：命令行参数解析
来源：http://pt.nicolike.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mn.szxytkj.cn

[U17] Py：初始化日志
来源：http://gh.521024.cn

logging.basicConfig(level=logging.INFO)
来源：http://ei.panjiajie.cn

[U18] Py：预编译正则
来源：http://gx.gzmigu.cn

pat = re.compile(r"\d+")
来源：http://cv.huixinmuqiang.cn

[U19] Py：正则替换带回调
来源：http://zi.jianghongdianzi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gj.panjiajie.cn

[U20] Py：缓存函数结果
来源：http://eo.asd995.cn

@functools.lru_cache(maxsize=None)
来源：http://ns.jctech888.com.cn

[U21] Py：自定义上下文管理器
来源：http://ex.nicolike.cn

@contextlib.contextmanager
来源：http://go.huixiangedu.cn

[U22] Py：矩阵转置
来源：http://ja.szxytkj.cn

list(zip(*m))
来源：http://ex.panjiajie.cn

[U23] Py：分块读取大文件
来源：http://jr.wgjwhj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://va.hahajie.cn

[U24] Py：路径操作
来源：http://eb.jctech888.com.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wk.chemitech.net.cn

[U25] Py：CSV 按字典读
来源：http://gu.yuexingan06.cn

csv.DictReader(f)
来源：http://dz.colortex.cn

[U26] Py：并发下载
来源：http://sl.huixinmuqiang.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rz.huixinmuqiang.cn

[U27] Py：异步 HTTP
来源：http://wt.hahajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://ca.newstarts.cn

[U28] Py：类型别名
来源：http://vm.bjjhwx.cn

UserId = int
来源：http://cu.yuexingan06.cn

[U29] Py：属性校验
来源：http://tj.muxihuayi.cn

@property 与 @x.setter 配合
来源：http://kp.hnjuh.cn

[U30] Py：数据类
来源：http://ux.hahajie.cn

@dataclass(slots=True)
来源：http://wz.lnxyls.cn

[U31] Py：单测
来源：http://ht.shxzukj.cn

python -m pytest -q
来源：http://lf.huanxung.cn

[U32] Py：代码格式化
来源：http://mi.huixinmuqiang.cn

ruff format . && ruff check --fix .
来源：http://xn.nszjky.cn

[U33] Py：打包发布
来源：http://uf.hahajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://wc.szsharing.cn

[U34] Py：判断编码
来源：http://fx.jianghongdianzi.cn

chardet.detect(raw)
来源：http://br.haigaiapp.cn

[U35] Py：发送邮件
来源：http://rx.muxihuayi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vz.jianghongdianzi.cn

[U36] Py：定时任务
来源：http://yf.panjiajie.cn

schedule.every(10).minutes.do(job)
来源：http://va.panjiajie.cn

[U37] Py：读写 Excel
来源：http://si.jianghongdianzi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://bg.yuntaijiaju.cn

[U38] Py：获取脚本所在目录
来源：http://mh.yuntaijiaju.cn

Path(__file__).resolve().parent
来源：http://ms.lnxyls.cn

[U39] Py：判断是否在交互环境
来源：http://fb.szsharing.cn

sys.stdout.isatty()
来源：http://uj.jianghongdianzi.cn

[U40] Py：打印到标准错误
来源：http://aj.nicolike.cn

print("err", file=sys.stderr)
来源：http://zg.521024.cn

[U41] PHP：初始化 Composer 项目
来源：http://lr.chemitech.net.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://za.huixinmuqiang.cn

[U42] PHP：PSR-4 自动加载
来源：http://jr.hnjuh.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ek.colortex.cn

[U43] PHP：声明命名空间
来源：http://fx.shxzskj.cn

namespace App\Http;
来源：http://wp.shxzskj.cn

[U44] PHP：开启严格类型
来源：http://ug.shxzskj.cn

declare(strict_types=1);
来源：http://vk.gzmigu.cn

[U45] PHP：类型声明与返回类型
来源：http://eq.yuexingan06.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qk.yuntaijiaju.cn

[U46] PHP：可空类型
来源：http://ti.huixinmuqiang.cn

?string $name = null
来源：http://sa.shxzukj.cn

[U47] PHP：联合类型
来源：http://by.521024.cn

int|string $id
来源：http://tv.huixinmuqiang.cn

[U48] PHP：纯枚举
来源：http://sw.hnjuh.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ew.521024.cn

[U49] PHP：只读属性
来源：http://tq.yuntaijiaju.cn

public readonly string $name
来源：http://ns.colortex.cn

[U50] PHP：构造器属性提升
来源：http://on.lnxyls.cn

public function __construct(private int $id) {}
来源：http://jg.huixinmuqiang.cn

[U51] PHP：数组解构
来源：http://cy.shxzukj.cn

[$a, $b] = $arr;
来源：http://ij.muxihuayi.cn

[U52] PHP：箭头函数
来源：http://fb.huixiangedu.cn

$double = fn($x) => $x * 2;
来源：http://lh.bookmarksfly.cn

[U53] PHP：空合并运算符
来源：http://st.nicolike.cn

$v = $a ?? $b ?? "default";
来源：http://ez.jctech888.com.cn

[U54] PHP：空安全调用
来源：http://rr.colortex.cn

$obj?->method()
来源：http://rp.shxzskj.cn

[U55] PHP：match 表达式
来源：http://gt.wgjwhj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ki.szsharing.cn

[U56] PHP：命名参数
来源：http://ak.hnjuh.cn

f(a: 1, b: 2)
来源：http://rz.jctech888.com.cn

[U57] PHP：字符串插值
来源：http://xc.hnjuh.cn

"值: {$a}"
来源：http://dy.shxzskj.cn

[U58] PHP：数组三件套
来源：http://pg.hnjuh.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yk.huixiangedu.cn

[U59] PHP：自定义排序
来源：http://wf.yuexingan06.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ff.huanxung.cn

[U60] PHP：JSON 编解码
来源：http://va.colortex.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zl.lnxyls.cn

[U61] PHP：正则
来源：http://tx.jctech888.com.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ku.newstarts.cn

[U62] PHP：日期对象
来源：http://ru.9csxet.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://aw.jianghongdianzi.cn

[U63] PHP：文件读写
来源：http://va.huanxung.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://oy.szxytkj.cn

[U64] PHP：目录遍历
来源：http://wo.huixinmuqiang.cn

glob("dir/*.php");  scandir("dir");
来源：http://my.521024.cn

[U65] PHP：会话
来源：http://is.bjjhwx.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ty.lnxyls.cn

[U66] PHP：设置 Cookie
来源：http://ho.bjjhwx.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kq.colortex.cn

[U67] PHP：处理文件上传
来源：http://ww.nicolike.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zn.huixinmuqiang.cn

[U68] PHP：PDO 连接
来源：http://gu.shxzskj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rx.wgjwhj.cn

[U69] PHP：PDO 预处理
来源：http://uz.shxzukj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cv.panjiajie.cn

[U70] PHP：PDO 事务
来源：http://nq.szxytkj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://je.chemitech.net.cn

[U71] PHP：抛出异常
来源：http://kn.hnjuh.cn

throw new RuntimeException("失败", 500);
来源：http://ca.shxzukj.cn

[U72] PHP：写错误日志
来源：http://av.shxzskj.cn

error_log("失败: " . $e->getMessage());
来源：http://qk.panjiajie.cn

[U73] PHP：读取 ini 配置
来源：http://le.9csxet.cn

parse_ini_file("config.ini", true)
来源：http://qi.nicolike.cn

[U74] PHP：读取环境变量
来源：http://sw.yuntaijiaju.cn

getenv("APP_ENV") ?: "production"
来源：http://cv.szsharing.cn

[U75] PHP：依赖注入
来源：http://sf.shxzukj.cn

composer require psr/container
来源：http://iw.521024.cn

[U76] PHP：简单路由
来源：http://vo.shtwfgs.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fu.bjjhwx.cn

[U77] PHP：模板渲染
来源：http://sf.9csxet.cn

composer require twig/twig
来源：http://de.521024.cn

[U78] PHP：单元测试
来源：http://wh.jianghongdianzi.cn

composer require --dev phpunit/phpunit
来源：http://wr.newstarts.cn

[U79] PHP：静态分析
来源：http://uf.521024.cn

composer require --dev phpstan/phpstan
来源：http://hr.nszjky.cn

[U80] PHP：代码规范修复
来源：http://qc.szxytkj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://hj.jianghongdianzi.cn

[U81] JS：初始化项目
来源：http://wg.yuexingan06.cn

npm init -y;  npm i express
来源：http://wi.huanxung.cn

[U82] JS：package.json 脚本
来源：http://li.lnxyls.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fz.jctech888.com.cn

[U83] JS：ES Module 导入导出
来源：http://gd.nicolike.cn

export const a = 1;  import { a } from "./m.js";
来源：http://yy.bjjhwx.cn

[U84] JS：CommonJS 写法
来源：http://tz.asd995.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ul.newstarts.cn

[U85] JS：可选链
来源：http://tu.szsharing.cn

a?.b?.c
来源：http://fq.haigaiapp.cn

[U86] JS：空值合并
来源：http://vf.nicolike.cn

a ?? b
来源：http://un.521024.cn

[U87] JS：解构默认值
来源：http://zq.haigaiapp.cn

const { a = 1, b = 2 } = obj;
来源：http://fq.newstarts.cn

[U88] JS：对象展开合并
来源：http://do.yuntaijiaju.cn

{ ...a, ...b }
来源：http://gg.bjjhwx.cn

[U89] JS：数组去重
来源：http://ec.szxytkj.cn

[...new Set(arr)]
来源：http://bo.wgjwhj.cn

[U90] JS：数字数组排序
来源：http://gc.bjjhwx.cn

[...arr].sort((a, b) => a - b)
来源：http://zf.szsharing.cn

[U91] JS：对象键值遍历
来源：http://yn.huixiangedu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vw.jctech888.com.cn

[U92] JS：深拷贝
来源：http://kx.jctech888.com.cn

structuredClone(obj)
来源：http://bp.jianghongdianzi.cn

[U93] JS：模板字符串
来源：http://be.jctech888.com.cn

`共 ${n} 条`
来源：http://ka.nszjky.cn

[U94] JS：箭头函数
来源：http://xf.bjjhwx.cn

const double = x => x * 2;
来源：http://uy.gzmigu.cn

[U95] JS：Promise 包装
来源：http://hs.shxzskj.cn

new Promise((resolve, reject) => {})
来源：http://zi.nszjky.cn

[U96] JS：async/await 与异常
来源：http://rg.521024.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gs.huanxung.cn

[U97] JS：并发请求
来源：http://jt.chemitech.net.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://cp.9csxet.cn

[U98] JS：fetch 带 JSON
来源：http://fs.shxzskj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gm.jctech888.com.cn

[U99] JS：事件监听
来源：http://th.hahajie.cn

el.addEventListener("click", e => {})
来源：http://ru.huixiangedu.cn

[U100] JS：DOM 查询
来源：http://bk.jianghongdianzi.cn

document.querySelector(".item")
来源：http://sz.szxytkj.cn

[U101] JS：classList 操作
来源：http://ur.shxzukj.cn

el.classList.toggle("active")
来源：http://rm.jianghongdianzi.cn

[U102] JS：本地存储
来源：http://eu.521024.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://cb.szxytkj.cn

[U103] JS：定时器
来源：http://bg.wgjwhj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qv.yuexingan06.cn

[U104] JS：防抖
来源：http://oj.nszjky.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pw.hnjuh.cn

[U105] JS：节流
来源：http://zy.panjiajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cz.9csxet.cn

[U106] JS：日期格式化
来源：http://rt.colortex.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://um.nszjky.cn

[U107] JS：数字千分位
来源：http://hz.jctech888.com.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://re.jianghongdianzi.cn

[U108] JS：随机整数
来源：http://ea.521024.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://et.nicolike.cn

[U109] JS：数组分组
来源：http://pi.hnjuh.cn

Object.groupBy(arr, x => x.type)
来源：http://yn.wgjwhj.cn

[U110] JS：数组分块
来源：http://kw.nicolike.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yc.newstarts.cn

[U111] JS：对象转 Map
来源：http://va.gzmigu.cn

new Map(Object.entries(obj))
来源：http://ie.521024.cn

[U112] JS：字符串补位
来源：http://vk.newstarts.cn

"7".padStart(3, "0")
来源：http://qj.shtwfgs.cn

[U113] JS：正则替换全部
来源：http://su.shxzskj.cn

s.replaceAll("a", "b")
来源：http://ed.hnjuh.cn

[U114] JS：JSON 深比较
来源：http://hw.shxzukj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ik.521024.cn

[U115] JS：生成 UUID
来源：http://yq.hnjuh.cn

crypto.randomUUID()
来源：http://ed.wgjwhj.cn

[U116] JS：类型检查（JSDoc）
来源：http://qp.shxzukj.cn

/** @param {string} name */ function f(name) {}
来源：http://da.huanxung.cn

[U117] JS：单元测试
来源：http://nm.shxzukj.cn

npm i -D vitest;  npx vitest
来源：http://xt.9csxet.cn

[U118] JS：开发服务器
来源：http://wl.521024.cn

npm i -D vite;  npx vite
来源：http://ci.chemitech.net.cn

[U119] JS：生产构建
来源：http://tp.newstarts.cn

npx vite build
来源：http://hj.wgjwhj.cn

[U120] JS：读取环境变量（Vite）
来源：http://zm.huixinmuqiang.cn

import.meta.env.VITE_API_URL
来源：http://cb.asd995.cn

================================================================================
来源：http://xu.9csxet.cn

统计汇总
来源：http://bt.yuexingan06.cn

================================================================================
来源：http://ek.9csxet.cn

按语言统计（条）：
来源：http://hj.bookmarksfly.cn

Python ......... 252
来源：http://et.huixiangedu.cn

PHP ............ 252
来源：http://ah.huixiangedu.cn

JavaScript ..... 252
来源：http://ia.shxzukj.cn

TypeScript ..... 212
来源：http://jn.bookmarksfly.cn

Java ........... 212
来源：http://ys.colortex.cn

Go ............. 212
来源：http://ut.nszjky.cn

Ruby ........... 212
来源：http://mf.hahajie.cn

C# ............. 212
来源：http://bp.nszjky.cn

C .............. 30
来源：http://xk.muxihuayi.cn

C++ ............ 30
来源：http://mj.huixinmuqiang.cn

SQL ............ 90
来源：http://ip.muxihuayi.cn

Bash ........... 80
来源：http://ex.asd995.cn

Kotlin ......... 15
来源：http://uq.haigaiapp.cn

Swift .......... 15
来源：http://mc.gzmigu.cn

Lua ............ 10
来源：http://zz.huixinmuqiang.cn

Perl ........... 10
来源：http://et.yuntaijiaju.cn


<!-- 参考信息 -->