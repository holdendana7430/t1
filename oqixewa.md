代发 wailian999

[T43] Perl：字符串插值
来源：http://ti.bookmarksfly.cn

"值: $a"
来源：http://ug.bookmarksfly.cn

[T44] Perl：条件
来源：http://tg.nicolike.cn

if ($a > 0) { print "正"; }
来源：http://xb.huanxung.cn

[T45] Perl：数组遍历
来源：http://xf.muxihuayi.cn

for my $x (@arr) { print $x; }
来源：http://re.szxytkj.cn

[T46] Perl：哈希操作
来源：http://oe.colortex.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://iu.9csxet.cn

[T47] Perl：正则捕获
来源：http://vh.muxihuayi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://tt.huixiangedu.cn

[T48] Perl：正则替换
来源：http://sr.shxzukj.cn

$s =~ s/old/new/g;
来源：http://bm.shxzskj.cn

[T49] Perl：函数
来源：http://dy.huanxung.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://iz.hnjuh.cn

[T50] Perl：逐行读文件
来源：http://kf.jianghongdianzi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ba.shtwfgs.cn

while (my $line = <$fh>) { print $line; }
来源：http://hc.nszjky.cn

[T51] Scala：Hello World
来源：http://bl.lnxyls.cn

println("Hello")
来源：http://qq.szsharing.cn

[T52] Scala：变量
来源：http://gg.nszjky.cn

val a = 1;  var b = 2
来源：http://up.newstarts.cn

[T53] Scala：字符串插值
来源：http://fs.hahajie.cn

s"值: $b"
来源：http://zk.asd995.cn

[T54] Scala：集合映射
来源：http://hr.shxzskj.cn

List(1, 2, 3).map(_ * 2)
来源：http://xf.bjjhwx.cn

[T55] Scala：集合过滤
来源：http://mp.haigaiapp.cn

List(1, 2, 3).filter(_ > 1)
来源：http://un.chemitech.net.cn

[T56] Scala：样例类
来源：http://xo.yuntaijiaju.cn

case class User(name: String, age: Int)
来源：http://li.bjjhwx.cn

[T57] Scala：模式匹配
来源：http://cr.yuexingan06.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ct.yuntaijiaju.cn

[T58] Scala：函数定义
来源：http://vv.gzmigu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ae.nicolike.cn

[T59] Scala：循环
来源：http://ej.bjjhwx.cn

for (i <- 1 to 10) println(i)
来源：http://bx.szsharing.cn

[T60] Scala：折叠
来源：http://ec.yuntaijiaju.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ye.shtwfgs.cn

================================================================================
来源：http://cu.bookmarksfly.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ax.huixinmuqiang.cn

================================================================================
来源：http://wm.yuntaijiaju.cn

[U01] Py：创建虚拟环境
来源：http://uo.wgjwhj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://fq.bjjhwx.cn

[U02] Py：导出 / 安装依赖
来源：http://dm.hnjuh.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yf.colortex.cn

[U03] Py：加载 .env 配置
来源：http://dt.huixiangedu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ic.nicolike.cn

[U04] Py：变量调试打印
来源：http://oe.hahajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mz.huanxung.cn

[U05] Py：列表去重且保序
来源：http://fm.chemitech.net.cn

list(dict.fromkeys(arr))
来源：http://iu.szxytkj.cn

[U06] Py：合并两个字典
来源：http://ja.shxzskj.cn

{**a, **b}
来源：http://lb.hahajie.cn

[U07] Py：反转字典键值
来源：http://zk.yuexingan06.cn

{v: k for k, v in d.items()}
来源：http://hm.shxzskj.cn

[U08] Py：展平二维列表
来源：http://hl.panjiajie.cn

[y for x in nested for y in x]
来源：http://vc.shxzukj.cn

[U09] Py：字典取最大值的键
来源：http://cf.wgjwhj.cn

max(d, key=d.get)
来源：http://lz.haigaiapp.cn

[U10] Py：按值排序字典
来源：http://se.shxzukj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ve.nicolike.cn

[U11] Py：生成器表达式
来源：http://fc.jianghongdianzi.cn

(x * 2 for x in arr)
来源：http://hi.gzmigu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://sq.shxzskj.cn

Counter(arr).most_common(3)
来源：http://jt.panjiajie.cn

[U13] Py：固定长度队列
来源：http://tm.9csxet.cn

deque(maxlen=10)
来源：http://zh.shtwfgs.cn

[U14] Py：分组收集到列表
来源：http://ox.gzmigu.cn

defaultdict(list)
来源：http://rn.bjjhwx.cn

[U15] Py：高精度计时
来源：http://hf.huixinmuqiang.cn

t = time.perf_counter()
来源：http://wz.lnxyls.cn

[U16] Py：命令行参数解析
来源：http://fk.nicolike.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yq.521024.cn

[U17] Py：初始化日志
来源：http://mr.hahajie.cn

logging.basicConfig(level=logging.INFO)
来源：http://lq.szxytkj.cn

[U18] Py：预编译正则
来源：http://pg.yuexingan06.cn

pat = re.compile(r"\d+")
来源：http://nx.9csxet.cn

[U19] Py：正则替换带回调
来源：http://kk.nicolike.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mo.haigaiapp.cn

[U20] Py：缓存函数结果
来源：http://zs.huanxung.cn

@functools.lru_cache(maxsize=None)
来源：http://nr.huanxung.cn

[U21] Py：自定义上下文管理器
来源：http://zt.muxihuayi.cn

@contextlib.contextmanager
来源：http://pg.huixinmuqiang.cn

[U22] Py：矩阵转置
来源：http://ba.shxzskj.cn

list(zip(*m))
来源：http://wt.huixinmuqiang.cn

[U23] Py：分块读取大文件
来源：http://us.bookmarksfly.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ba.yuexingan06.cn

[U24] Py：路径操作
来源：http://jy.szsharing.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yy.jianghongdianzi.cn

[U25] Py：CSV 按字典读
来源：http://vl.bookmarksfly.cn

csv.DictReader(f)
来源：http://hf.bookmarksfly.cn

[U26] Py：并发下载
来源：http://bb.haigaiapp.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://sv.hahajie.cn

[U27] Py：异步 HTTP
来源：http://wt.muxihuayi.cn

aiohttp.ClientSession() 配合 async with
来源：http://zt.szsharing.cn

[U28] Py：类型别名
来源：http://nt.jctech888.com.cn

UserId = int
来源：http://zd.haigaiapp.cn

[U29] Py：属性校验
来源：http://zp.colortex.cn

@property 与 @x.setter 配合
来源：http://jf.wgjwhj.cn

[U30] Py：数据类
来源：http://uc.haigaiapp.cn

@dataclass(slots=True)
来源：http://qg.haigaiapp.cn

[U31] Py：单测
来源：http://nf.lnxyls.cn

python -m pytest -q
来源：http://aj.shxzskj.cn

[U32] Py：代码格式化
来源：http://vt.yuexingan06.cn

ruff format . && ruff check --fix .
来源：http://pg.szxytkj.cn

[U33] Py：打包发布
来源：http://wg.shtwfgs.cn

python -m build  （依赖 pyproject.toml）
来源：http://fx.yuexingan06.cn

[U34] Py：判断编码
来源：http://gn.panjiajie.cn

chardet.detect(raw)
来源：http://ud.gzmigu.cn

[U35] Py：发送邮件
来源：http://cc.huanxung.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nl.shxzskj.cn

[U36] Py：定时任务
来源：http://id.nicolike.cn

schedule.every(10).minutes.do(job)
来源：http://oe.yuntaijiaju.cn

[U37] Py：读写 Excel
来源：http://ao.jianghongdianzi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://en.huanxung.cn

[U38] Py：获取脚本所在目录
来源：http://cu.jctech888.com.cn

Path(__file__).resolve().parent
来源：http://fj.bookmarksfly.cn

[U39] Py：判断是否在交互环境
来源：http://ak.newstarts.cn

sys.stdout.isatty()
来源：http://dj.haigaiapp.cn

[U40] Py：打印到标准错误
来源：http://bj.yuexingan06.cn

print("err", file=sys.stderr)
来源：http://dx.wgjwhj.cn

[U41] PHP：初始化 Composer 项目
来源：http://ga.521024.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://bv.huanxung.cn

[U42] PHP：PSR-4 自动加载
来源：http://qz.bjjhwx.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ca.yuexingan06.cn

[U43] PHP：声明命名空间
来源：http://ma.huixiangedu.cn

namespace App\Http;
来源：http://sd.521024.cn

[U44] PHP：开启严格类型
来源：http://pt.shtwfgs.cn

declare(strict_types=1);
来源：http://fc.yuntaijiaju.cn

[U45] PHP：类型声明与返回类型
来源：http://hv.huixinmuqiang.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://vy.shxzskj.cn

[U46] PHP：可空类型
来源：http://ey.muxihuayi.cn

?string $name = null
来源：http://ub.panjiajie.cn

[U47] PHP：联合类型
来源：http://lt.huixiangedu.cn

int|string $id
来源：http://fa.yuntaijiaju.cn

[U48] PHP：纯枚举
来源：http://rc.colortex.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xb.hahajie.cn

[U49] PHP：只读属性
来源：http://ha.hahajie.cn

public readonly string $name
来源：http://jv.chemitech.net.cn

[U50] PHP：构造器属性提升
来源：http://md.bjjhwx.cn

public function __construct(private int $id) {}
来源：http://sb.gzmigu.cn

[U51] PHP：数组解构
来源：http://yo.colortex.cn

[$a, $b] = $arr;
来源：http://re.huixinmuqiang.cn

[U52] PHP：箭头函数
来源：http://fj.haigaiapp.cn

$double = fn($x) => $x * 2;
来源：http://rt.shtwfgs.cn

[U53] PHP：空合并运算符
来源：http://nw.shtwfgs.cn

$v = $a ?? $b ?? "default";
来源：http://dw.bookmarksfly.cn

[U54] PHP：空安全调用
来源：http://wi.yuexingan06.cn

$obj?->method()
来源：http://yd.newstarts.cn

[U55] PHP：match 表达式
来源：http://ed.szsharing.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://df.9csxet.cn

[U56] PHP：命名参数
来源：http://lv.shtwfgs.cn

f(a: 1, b: 2)
来源：http://cq.shxzskj.cn

[U57] PHP：字符串插值
来源：http://nk.szsharing.cn

"值: {$a}"
来源：http://rv.yuexingan06.cn

[U58] PHP：数组三件套
来源：http://nx.muxihuayi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kx.newstarts.cn

[U59] PHP：自定义排序
来源：http://xb.jianghongdianzi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uh.jianghongdianzi.cn

[U60] PHP：JSON 编解码
来源：http://lt.hnjuh.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kz.haigaiapp.cn

[U61] PHP：正则
来源：http://na.chemitech.net.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rw.huixinmuqiang.cn

[U62] PHP：日期对象
来源：http://qa.shxzukj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zd.huixinmuqiang.cn

[U63] PHP：文件读写
来源：http://or.gzmigu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xb.yuntaijiaju.cn

[U64] PHP：目录遍历
来源：http://vh.asd995.cn

glob("dir/*.php");  scandir("dir");
来源：http://og.bookmarksfly.cn

[U65] PHP：会话
来源：http://ce.jianghongdianzi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://eb.nszjky.cn

[U66] PHP：设置 Cookie
来源：http://ek.chemitech.net.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sk.jctech888.com.cn

[U67] PHP：处理文件上传
来源：http://km.jianghongdianzi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lr.9csxet.cn

[U68] PHP：PDO 连接
来源：http://sk.huixiangedu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xw.panjiajie.cn

[U69] PHP：PDO 预处理
来源：http://cl.521024.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ax.hnjuh.cn

[U70] PHP：PDO 事务
来源：http://wi.gzmigu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jr.chemitech.net.cn

[U71] PHP：抛出异常
来源：http://yj.jianghongdianzi.cn

throw new RuntimeException("失败", 500);
来源：http://eg.colortex.cn

[U72] PHP：写错误日志
来源：http://hb.huanxung.cn

error_log("失败: " . $e->getMessage());
来源：http://vf.9csxet.cn

[U73] PHP：读取 ini 配置
来源：http://ea.newstarts.cn

parse_ini_file("config.ini", true)
来源：http://dw.chemitech.net.cn

[U74] PHP：读取环境变量
来源：http://om.muxihuayi.cn

getenv("APP_ENV") ?: "production"
来源：http://ck.muxihuayi.cn

[U75] PHP：依赖注入
来源：http://wp.haigaiapp.cn

composer require psr/container
来源：http://ty.9csxet.cn

[U76] PHP：简单路由
来源：http://iw.yuntaijiaju.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vl.bookmarksfly.cn

[U77] PHP：模板渲染
来源：http://wz.yuntaijiaju.cn

composer require twig/twig
来源：http://qf.huixinmuqiang.cn

[U78] PHP：单元测试
来源：http://bl.shtwfgs.cn

composer require --dev phpunit/phpunit
来源：http://pm.bookmarksfly.cn

[U79] PHP：静态分析
来源：http://wm.haigaiapp.cn

composer require --dev phpstan/phpstan
来源：http://ti.9csxet.cn

[U80] PHP：代码规范修复
来源：http://ft.asd995.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://iy.szxytkj.cn

[U81] JS：初始化项目
来源：http://wb.yuexingan06.cn

npm init -y;  npm i express
来源：http://to.yuntaijiaju.cn

[U82] JS：package.json 脚本
来源：http://bd.muxihuayi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sk.chemitech.net.cn

[U83] JS：ES Module 导入导出
来源：http://ft.shtwfgs.cn

export const a = 1;  import { a } from "./m.js";
来源：http://mj.9csxet.cn

[U84] JS：CommonJS 写法
来源：http://bl.jianghongdianzi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://aw.521024.cn

[U85] JS：可选链
来源：http://uw.bjjhwx.cn

a?.b?.c
来源：http://gh.huixiangedu.cn

[U86] JS：空值合并
来源：http://lu.nszjky.cn

a ?? b
来源：http://jh.asd995.cn

[U87] JS：解构默认值
来源：http://nq.huixinmuqiang.cn

const { a = 1, b = 2 } = obj;
来源：http://pz.shxzskj.cn

[U88] JS：对象展开合并
来源：http://av.colortex.cn

{ ...a, ...b }
来源：http://ne.wgjwhj.cn

[U89] JS：数组去重
来源：http://be.hnjuh.cn

[...new Set(arr)]
来源：http://hc.gzmigu.cn

[U90] JS：数字数组排序
来源：http://yw.shxzskj.cn

[...arr].sort((a, b) => a - b)
来源：http://hz.panjiajie.cn

[U91] JS：对象键值遍历
来源：http://in.nszjky.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kq.shtwfgs.cn

[U92] JS：深拷贝
来源：http://st.huixinmuqiang.cn

structuredClone(obj)
来源：http://lp.huanxung.cn

[U93] JS：模板字符串
来源：http://ol.jctech888.com.cn

`共 ${n} 条`
来源：http://jx.jianghongdianzi.cn

[U94] JS：箭头函数
来源：http://mu.shtwfgs.cn

const double = x => x * 2;
来源：http://xd.wgjwhj.cn

[U95] JS：Promise 包装
来源：http://mx.muxihuayi.cn

new Promise((resolve, reject) => {})
来源：http://xi.hnjuh.cn

[U96] JS：async/await 与异常
来源：http://oy.huixinmuqiang.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rr.shxzskj.cn

[U97] JS：并发请求
来源：http://io.szxytkj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zp.huixiangedu.cn

[U98] JS：fetch 带 JSON
来源：http://jm.bjjhwx.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xs.szxytkj.cn

[U99] JS：事件监听
来源：http://eo.bjjhwx.cn

el.addEventListener("click", e => {})
来源：http://gs.newstarts.cn

[U100] JS：DOM 查询
来源：http://tu.panjiajie.cn

document.querySelector(".item")
来源：http://ag.muxihuayi.cn

[U101] JS：classList 操作
来源：http://ql.bookmarksfly.cn

el.classList.toggle("active")
来源：http://xh.hnjuh.cn

[U102] JS：本地存储
来源：http://dt.newstarts.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://oi.shxzukj.cn

[U103] JS：定时器
来源：http://id.haigaiapp.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pq.szsharing.cn

[U104] JS：防抖
来源：http://mm.gzmigu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qu.yuntaijiaju.cn

[U105] JS：节流
来源：http://ba.newstarts.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qs.nicolike.cn

[U106] JS：日期格式化
来源：http://hh.huixiangedu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zc.521024.cn

[U107] JS：数字千分位
来源：http://ri.bjjhwx.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pn.huixiangedu.cn

[U108] JS：随机整数
来源：http://mr.shxzukj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://am.bjjhwx.cn

[U109] JS：数组分组
来源：http://fa.haigaiapp.cn

Object.groupBy(arr, x => x.type)
来源：http://bj.asd995.cn

[U110] JS：数组分块
来源：http://uc.szxytkj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fb.bjjhwx.cn

[U111] JS：对象转 Map
来源：http://ab.huixiangedu.cn

new Map(Object.entries(obj))
来源：http://ny.shxzskj.cn

[U112] JS：字符串补位
来源：http://ut.yuntaijiaju.cn

"7".padStart(3, "0")
来源：http://rd.shxzskj.cn

[U113] JS：正则替换全部
来源：http://bm.nszjky.cn

s.replaceAll("a", "b")
来源：http://pu.jianghongdianzi.cn

[U114] JS：JSON 深比较
来源：http://ko.lnxyls.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ub.asd995.cn

[U115] JS：生成 UUID
来源：http://if.muxihuayi.cn

crypto.randomUUID()
来源：http://rd.asd995.cn

[U116] JS：类型检查（JSDoc）
来源：http://ex.szsharing.cn

/** @param {string} name */ function f(name) {}
来源：http://jd.bookmarksfly.cn

[U117] JS：单元测试
来源：http://fd.jianghongdianzi.cn

npm i -D vitest;  npx vitest
来源：http://su.lnxyls.cn

[U118] JS：开发服务器
来源：http://pw.9csxet.cn

npm i -D vite;  npx vite
来源：http://ow.nszjky.cn

[U119] JS：生产构建
来源：http://ot.9csxet.cn

npx vite build
来源：http://xe.nszjky.cn

[U120] JS：读取环境变量（Vite）
来源：http://ox.huixiangedu.cn

import.meta.env.VITE_API_URL
来源：http://mc.panjiajie.cn

================================================================================
来源：http://ss.gzmigu.cn

统计汇总
来源：http://wo.gzmigu.cn

================================================================================
来源：http://rl.521024.cn

按语言统计（条）：
来源：http://bk.521024.cn

Python ......... 252
来源：http://hl.panjiajie.cn

PHP ............ 252
来源：http://ij.huanxung.cn

JavaScript ..... 252
来源：http://rb.bookmarksfly.cn

TypeScript ..... 212
来源：http://xa.nicolike.cn

Java ........... 212
来源：http://cg.shtwfgs.cn

Go ............. 212
来源：http://ks.yuexingan06.cn

Ruby ........... 212
来源：http://zj.lnxyls.cn

C# ............. 212
来源：http://ya.asd995.cn

C .............. 30
来源：http://pe.521024.cn

C++ ............ 30
来源：http://dr.newstarts.cn

SQL ............ 90
来源：http://nu.521024.cn

Bash ........... 80
来源：http://sw.bjjhwx.cn

Kotlin ......... 15
来源：http://oq.yuntaijiaju.cn

Swift .......... 15
来源：http://ug.wgjwhj.cn

Lua ............ 10
来源：http://fa.wgjwhj.cn

Perl ........... 10
来源：http://uw.shtwfgs.cn


<!-- 参考信息 -->