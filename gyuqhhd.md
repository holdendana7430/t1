代发 wailian999

[T43] Perl：字符串插值
来源：http://in.panjiajie.cn

"值: $a"
来源：http://gu.newstarts.cn

[T44] Perl：条件
来源：http://nd.hahajie.cn

if ($a > 0) { print "正"; }
来源：http://ak.yuntaijiaju.cn

[T45] Perl：数组遍历
来源：http://fh.panjiajie.cn

for my $x (@arr) { print $x; }
来源：http://uh.nicolike.cn

[T46] Perl：哈希操作
来源：http://ao.yuntaijiaju.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pc.lnxyls.cn

[T47] Perl：正则捕获
来源：http://yb.lnxyls.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://gh.nszjky.cn

[T48] Perl：正则替换
来源：http://zr.yuntaijiaju.cn

$s =~ s/old/new/g;
来源：http://ph.yuntaijiaju.cn

[T49] Perl：函数
来源：http://mv.shxzukj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vm.muxihuayi.cn

[T50] Perl：逐行读文件
来源：http://ag.jctech888.com.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://oy.wgjwhj.cn

while (my $line = <$fh>) { print $line; }
来源：http://rn.jianghongdianzi.cn

[T51] Scala：Hello World
来源：http://es.gzmigu.cn

println("Hello")
来源：http://la.shtwfgs.cn

[T52] Scala：变量
来源：http://ei.newstarts.cn

val a = 1;  var b = 2
来源：http://iw.shxzskj.cn

[T53] Scala：字符串插值
来源：http://pp.szxytkj.cn

s"值: $b"
来源：http://rn.colortex.cn

[T54] Scala：集合映射
来源：http://pe.shxzskj.cn

List(1, 2, 3).map(_ * 2)
来源：http://ox.bjjhwx.cn

[T55] Scala：集合过滤
来源：http://oc.bookmarksfly.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ev.wgjwhj.cn

[T56] Scala：样例类
来源：http://jf.9csxet.cn

case class User(name: String, age: Int)
来源：http://rm.szxytkj.cn

[T57] Scala：模式匹配
来源：http://yw.szsharing.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vn.nicolike.cn

[T58] Scala：函数定义
来源：http://ot.wgjwhj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zm.yuntaijiaju.cn

[T59] Scala：循环
来源：http://co.huixiangedu.cn

for (i <- 1 to 10) println(i)
来源：http://wl.shxzskj.cn

[T60] Scala：折叠
来源：http://vf.haigaiapp.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hl.bookmarksfly.cn

================================================================================
来源：http://ed.haigaiapp.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ne.shxzskj.cn

================================================================================
来源：http://vf.wgjwhj.cn

[U01] Py：创建虚拟环境
来源：http://ch.huanxung.cn

python -m venv .venv && source .venv/bin/activate
来源：http://yk.bjjhwx.cn

[U02] Py：导出 / 安装依赖
来源：http://ze.yuexingan06.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nf.shxzskj.cn

[U03] Py：加载 .env 配置
来源：http://iq.huanxung.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://nd.hnjuh.cn

[U04] Py：变量调试打印
来源：http://fk.jctech888.com.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xc.lnxyls.cn

[U05] Py：列表去重且保序
来源：http://gf.huixinmuqiang.cn

list(dict.fromkeys(arr))
来源：http://vr.521024.cn

[U06] Py：合并两个字典
来源：http://wf.bookmarksfly.cn

{**a, **b}
来源：http://ol.panjiajie.cn

[U07] Py：反转字典键值
来源：http://pd.lnxyls.cn

{v: k for k, v in d.items()}
来源：http://lh.shxzskj.cn

[U08] Py：展平二维列表
来源：http://tu.lnxyls.cn

[y for x in nested for y in x]
来源：http://zt.9csxet.cn

[U09] Py：字典取最大值的键
来源：http://uw.huixinmuqiang.cn

max(d, key=d.get)
来源：http://qa.shxzukj.cn

[U10] Py：按值排序字典
来源：http://jr.9csxet.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ik.newstarts.cn

[U11] Py：生成器表达式
来源：http://gk.huixiangedu.cn

(x * 2 for x in arr)
来源：http://ir.huixinmuqiang.cn

[U12] Py：取出现最多的 3 个元素
来源：http://la.asd995.cn

Counter(arr).most_common(3)
来源：http://zh.nszjky.cn

[U13] Py：固定长度队列
来源：http://sx.szxytkj.cn

deque(maxlen=10)
来源：http://sq.huixiangedu.cn

[U14] Py：分组收集到列表
来源：http://qt.nszjky.cn

defaultdict(list)
来源：http://ii.hnjuh.cn

[U15] Py：高精度计时
来源：http://fs.panjiajie.cn

t = time.perf_counter()
来源：http://zk.wgjwhj.cn

[U16] Py：命令行参数解析
来源：http://ij.asd995.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yi.hahajie.cn

[U17] Py：初始化日志
来源：http://un.bookmarksfly.cn

logging.basicConfig(level=logging.INFO)
来源：http://bi.shxzskj.cn

[U18] Py：预编译正则
来源：http://rx.huixinmuqiang.cn

pat = re.compile(r"\d+")
来源：http://de.bookmarksfly.cn

[U19] Py：正则替换带回调
来源：http://by.yuntaijiaju.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://oi.shxzukj.cn

[U20] Py：缓存函数结果
来源：http://mb.shxzukj.cn

@functools.lru_cache(maxsize=None)
来源：http://gn.haigaiapp.cn

[U21] Py：自定义上下文管理器
来源：http://xk.wgjwhj.cn

@contextlib.contextmanager
来源：http://aj.gzmigu.cn

[U22] Py：矩阵转置
来源：http://vh.chemitech.net.cn

list(zip(*m))
来源：http://pz.shtwfgs.cn

[U23] Py：分块读取大文件
来源：http://hr.bookmarksfly.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nm.yuntaijiaju.cn

[U24] Py：路径操作
来源：http://zq.chemitech.net.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gh.shtwfgs.cn

[U25] Py：CSV 按字典读
来源：http://aa.wgjwhj.cn

csv.DictReader(f)
来源：http://dd.bjjhwx.cn

[U26] Py：并发下载
来源：http://re.jctech888.com.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://an.szxytkj.cn

[U27] Py：异步 HTTP
来源：http://km.szsharing.cn

aiohttp.ClientSession() 配合 async with
来源：http://uo.chemitech.net.cn

[U28] Py：类型别名
来源：http://zk.asd995.cn

UserId = int
来源：http://gq.huixinmuqiang.cn

[U29] Py：属性校验
来源：http://yp.wgjwhj.cn

@property 与 @x.setter 配合
来源：http://kc.yuntaijiaju.cn

[U30] Py：数据类
来源：http://iw.lnxyls.cn

@dataclass(slots=True)
来源：http://oh.hahajie.cn

[U31] Py：单测
来源：http://vc.9csxet.cn

python -m pytest -q
来源：http://qs.lnxyls.cn

[U32] Py：代码格式化
来源：http://zo.shtwfgs.cn

ruff format . && ruff check --fix .
来源：http://st.newstarts.cn

[U33] Py：打包发布
来源：http://fi.lnxyls.cn

python -m build  （依赖 pyproject.toml）
来源：http://vd.chemitech.net.cn

[U34] Py：判断编码
来源：http://gw.asd995.cn

chardet.detect(raw)
来源：http://lp.nicolike.cn

[U35] Py：发送邮件
来源：http://ib.huixinmuqiang.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hy.521024.cn

[U36] Py：定时任务
来源：http://bt.lnxyls.cn

schedule.every(10).minutes.do(job)
来源：http://rw.yuntaijiaju.cn

[U37] Py：读写 Excel
来源：http://ou.wgjwhj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://uz.huixiangedu.cn

[U38] Py：获取脚本所在目录
来源：http://az.haigaiapp.cn

Path(__file__).resolve().parent
来源：http://dk.nicolike.cn

[U39] Py：判断是否在交互环境
来源：http://ba.wgjwhj.cn

sys.stdout.isatty()
来源：http://bc.shtwfgs.cn

[U40] Py：打印到标准错误
来源：http://ry.yuexingan06.cn

print("err", file=sys.stderr)
来源：http://zl.9csxet.cn

[U41] PHP：初始化 Composer 项目
来源：http://au.nszjky.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://eh.huixiangedu.cn

[U42] PHP：PSR-4 自动加载
来源：http://rd.jctech888.com.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zp.hahajie.cn

[U43] PHP：声明命名空间
来源：http://ez.shxzukj.cn

namespace App\Http;
来源：http://bw.521024.cn

[U44] PHP：开启严格类型
来源：http://ms.nicolike.cn

declare(strict_types=1);
来源：http://st.bjjhwx.cn

[U45] PHP：类型声明与返回类型
来源：http://dq.bookmarksfly.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://vj.huanxung.cn

[U46] PHP：可空类型
来源：http://at.hnjuh.cn

?string $name = null
来源：http://pb.bjjhwx.cn

[U47] PHP：联合类型
来源：http://mf.lnxyls.cn

int|string $id
来源：http://wj.nszjky.cn

[U48] PHP：纯枚举
来源：http://xe.chemitech.net.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xs.yuntaijiaju.cn

[U49] PHP：只读属性
来源：http://da.szxytkj.cn

public readonly string $name
来源：http://ut.szsharing.cn

[U50] PHP：构造器属性提升
来源：http://ke.szxytkj.cn

public function __construct(private int $id) {}
来源：http://il.gzmigu.cn

[U51] PHP：数组解构
来源：http://cf.yuntaijiaju.cn

[$a, $b] = $arr;
来源：http://qa.asd995.cn

[U52] PHP：箭头函数
来源：http://lf.chemitech.net.cn

$double = fn($x) => $x * 2;
来源：http://zm.wgjwhj.cn

[U53] PHP：空合并运算符
来源：http://ow.huanxung.cn

$v = $a ?? $b ?? "default";
来源：http://kn.muxihuayi.cn

[U54] PHP：空安全调用
来源：http://hw.haigaiapp.cn

$obj?->method()
来源：http://iy.muxihuayi.cn

[U55] PHP：match 表达式
来源：http://id.yuntaijiaju.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pa.yuexingan06.cn

[U56] PHP：命名参数
来源：http://wm.shtwfgs.cn

f(a: 1, b: 2)
来源：http://wb.shxzukj.cn

[U57] PHP：字符串插值
来源：http://ra.szxytkj.cn

"值: {$a}"
来源：http://jf.asd995.cn

[U58] PHP：数组三件套
来源：http://oj.521024.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lg.jctech888.com.cn

[U59] PHP：自定义排序
来源：http://pd.jctech888.com.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nu.hahajie.cn

[U60] PHP：JSON 编解码
来源：http://of.shxzskj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hn.jctech888.com.cn

[U61] PHP：正则
来源：http://ft.asd995.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://su.gzmigu.cn

[U62] PHP：日期对象
来源：http://jg.chemitech.net.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mm.shxzukj.cn

[U63] PHP：文件读写
来源：http://cx.hahajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ug.panjiajie.cn

[U64] PHP：目录遍历
来源：http://ap.9csxet.cn

glob("dir/*.php");  scandir("dir");
来源：http://yc.lnxyls.cn

[U65] PHP：会话
来源：http://kb.chemitech.net.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://iy.nicolike.cn

[U66] PHP：设置 Cookie
来源：http://za.yuntaijiaju.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rw.newstarts.cn

[U67] PHP：处理文件上传
来源：http://py.nszjky.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xo.szxytkj.cn

[U68] PHP：PDO 连接
来源：http://wy.jianghongdianzi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kz.bookmarksfly.cn

[U69] PHP：PDO 预处理
来源：http://bg.panjiajie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ud.asd995.cn

[U70] PHP：PDO 事务
来源：http://cd.521024.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sw.shxzskj.cn

[U71] PHP：抛出异常
来源：http://ys.bookmarksfly.cn

throw new RuntimeException("失败", 500);
来源：http://xj.newstarts.cn

[U72] PHP：写错误日志
来源：http://ip.shtwfgs.cn

error_log("失败: " . $e->getMessage());
来源：http://tn.panjiajie.cn

[U73] PHP：读取 ini 配置
来源：http://hb.panjiajie.cn

parse_ini_file("config.ini", true)
来源：http://fd.yuntaijiaju.cn

[U74] PHP：读取环境变量
来源：http://ml.panjiajie.cn

getenv("APP_ENV") ?: "production"
来源：http://kq.9csxet.cn

[U75] PHP：依赖注入
来源：http://vx.jctech888.com.cn

composer require psr/container
来源：http://jb.muxihuayi.cn

[U76] PHP：简单路由
来源：http://rz.lnxyls.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hc.yuntaijiaju.cn

[U77] PHP：模板渲染
来源：http://kv.521024.cn

composer require twig/twig
来源：http://bm.yuexingan06.cn

[U78] PHP：单元测试
来源：http://ui.yuntaijiaju.cn

composer require --dev phpunit/phpunit
来源：http://dp.nicolike.cn

[U79] PHP：静态分析
来源：http://fw.yuexingan06.cn

composer require --dev phpstan/phpstan
来源：http://ak.muxihuayi.cn

[U80] PHP：代码规范修复
来源：http://yw.bookmarksfly.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://vm.yuexingan06.cn

[U81] JS：初始化项目
来源：http://lr.szxytkj.cn

npm init -y;  npm i express
来源：http://wa.yuexingan06.cn

[U82] JS：package.json 脚本
来源：http://yd.9csxet.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lc.panjiajie.cn

[U83] JS：ES Module 导入导出
来源：http://rs.shxzskj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://kj.gzmigu.cn

[U84] JS：CommonJS 写法
来源：http://be.9csxet.cn

module.exports = { a };  const { a } = require("./m");
来源：http://qn.shxzukj.cn

[U85] JS：可选链
来源：http://ul.hnjuh.cn

a?.b?.c
来源：http://kj.9csxet.cn

[U86] JS：空值合并
来源：http://ls.jctech888.com.cn

a ?? b
来源：http://ye.nicolike.cn

[U87] JS：解构默认值
来源：http://de.newstarts.cn

const { a = 1, b = 2 } = obj;
来源：http://va.shxzskj.cn

[U88] JS：对象展开合并
来源：http://ao.gzmigu.cn

{ ...a, ...b }
来源：http://di.nicolike.cn

[U89] JS：数组去重
来源：http://qh.yuexingan06.cn

[...new Set(arr)]
来源：http://zh.huixiangedu.cn

[U90] JS：数字数组排序
来源：http://ks.bookmarksfly.cn

[...arr].sort((a, b) => a - b)
来源：http://hp.asd995.cn

[U91] JS：对象键值遍历
来源：http://hi.haigaiapp.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gq.muxihuayi.cn

[U92] JS：深拷贝
来源：http://yb.yuntaijiaju.cn

structuredClone(obj)
来源：http://mg.bookmarksfly.cn

[U93] JS：模板字符串
来源：http://kc.nicolike.cn

`共 ${n} 条`
来源：http://rg.chemitech.net.cn

[U94] JS：箭头函数
来源：http://vy.jctech888.com.cn

const double = x => x * 2;
来源：http://ng.wgjwhj.cn

[U95] JS：Promise 包装
来源：http://kc.hnjuh.cn

new Promise((resolve, reject) => {})
来源：http://il.hnjuh.cn

[U96] JS：async/await 与异常
来源：http://oc.huanxung.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qz.yuexingan06.cn

[U97] JS：并发请求
来源：http://pd.chemitech.net.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://pf.hnjuh.cn

[U98] JS：fetch 带 JSON
来源：http://li.shxzukj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cc.hahajie.cn

[U99] JS：事件监听
来源：http://tv.nicolike.cn

el.addEventListener("click", e => {})
来源：http://ii.gzmigu.cn

[U100] JS：DOM 查询
来源：http://xn.yuexingan06.cn

document.querySelector(".item")
来源：http://ly.521024.cn

[U101] JS：classList 操作
来源：http://aj.nszjky.cn

el.classList.toggle("active")
来源：http://yu.nszjky.cn

[U102] JS：本地存储
来源：http://xk.szsharing.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://fc.muxihuayi.cn

[U103] JS：定时器
来源：http://gk.chemitech.net.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xn.nicolike.cn

[U104] JS：防抖
来源：http://mf.muxihuayi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ty.yuntaijiaju.cn

[U105] JS：节流
来源：http://hb.nszjky.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cs.shxzskj.cn

[U106] JS：日期格式化
来源：http://pr.nszjky.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://er.szsharing.cn

[U107] JS：数字千分位
来源：http://kd.nicolike.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qd.szsharing.cn

[U108] JS：随机整数
来源：http://jj.huixiangedu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vv.shtwfgs.cn

[U109] JS：数组分组
来源：http://mj.nszjky.cn

Object.groupBy(arr, x => x.type)
来源：http://nb.lnxyls.cn

[U110] JS：数组分块
来源：http://el.lnxyls.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ad.jianghongdianzi.cn

[U111] JS：对象转 Map
来源：http://ty.jianghongdianzi.cn

new Map(Object.entries(obj))
来源：http://xl.9csxet.cn

[U112] JS：字符串补位
来源：http://ii.asd995.cn

"7".padStart(3, "0")
来源：http://tq.yuntaijiaju.cn

[U113] JS：正则替换全部
来源：http://cj.shtwfgs.cn

s.replaceAll("a", "b")
来源：http://pi.bjjhwx.cn

[U114] JS：JSON 深比较
来源：http://js.panjiajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ca.bjjhwx.cn

[U115] JS：生成 UUID
来源：http://lv.bjjhwx.cn

crypto.randomUUID()
来源：http://gk.asd995.cn

[U116] JS：类型检查（JSDoc）
来源：http://kk.newstarts.cn

/** @param {string} name */ function f(name) {}
来源：http://qn.nicolike.cn

[U117] JS：单元测试
来源：http://zu.jianghongdianzi.cn

npm i -D vitest;  npx vitest
来源：http://rs.shtwfgs.cn

[U118] JS：开发服务器
来源：http://hi.jianghongdianzi.cn

npm i -D vite;  npx vite
来源：http://xc.huanxung.cn

[U119] JS：生产构建
来源：http://ac.huixiangedu.cn

npx vite build
来源：http://gq.nszjky.cn

[U120] JS：读取环境变量（Vite）
来源：http://nr.muxihuayi.cn

import.meta.env.VITE_API_URL
来源：http://pn.newstarts.cn

================================================================================
来源：http://el.jctech888.com.cn

统计汇总
来源：http://ys.panjiajie.cn

================================================================================
来源：http://rv.haigaiapp.cn

按语言统计（条）：
来源：http://rt.bjjhwx.cn

Python ......... 252
来源：http://lv.jianghongdianzi.cn

PHP ............ 252
来源：http://be.szsharing.cn

JavaScript ..... 252
来源：http://zp.panjiajie.cn

TypeScript ..... 212
来源：http://dc.shtwfgs.cn

Java ........... 212
来源：http://vh.nicolike.cn

Go ............. 212
来源：http://ul.panjiajie.cn

Ruby ........... 212
来源：http://lw.chemitech.net.cn

C# ............. 212
来源：http://xx.haigaiapp.cn

C .............. 30
来源：http://lr.yuexingan06.cn

C++ ............ 30
来源：http://fa.yuexingan06.cn

SQL ............ 90
来源：http://xl.9csxet.cn

Bash ........... 80
来源：http://pj.jctech888.com.cn

Kotlin ......... 15
来源：http://hp.szsharing.cn

Swift .......... 15
来源：http://lo.9csxet.cn

Lua ............ 10
来源：http://cj.hahajie.cn

Perl ........... 10
来源：http://kg.yuexingan06.cn


<!-- 参考信息 -->