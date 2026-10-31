代发 wailian999

[T47] Perl：正则捕获
来源：http://dz.hnjuh.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jl.szsharing.cn

[T48] Perl：正则替换
来源：http://ax.asd995.cn

$s =~ s/old/new/g;
来源：http://kf.szsharing.cn

[T49] Perl：函数
来源：http://ks.muxihuayi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dv.9csxet.cn

[T50] Perl：逐行读文件
来源：http://pq.yuntaijiaju.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://oq.521024.cn

while (my $line = <$fh>) { print $line; }
来源：http://xi.shxzskj.cn

[T51] Scala：Hello World
来源：http://nm.nicolike.cn

println("Hello")
来源：http://tb.bjjhwx.cn

[T52] Scala：变量
来源：http://md.colortex.cn

val a = 1;  var b = 2
来源：http://ep.chemitech.net.cn

[T53] Scala：字符串插值
来源：http://fy.muxihuayi.cn

s"值: $b"
来源：http://bt.chemitech.net.cn

[T54] Scala：集合映射
来源：http://mv.huixiangedu.cn

List(1, 2, 3).map(_ * 2)
来源：http://nn.szxytkj.cn

[T55] Scala：集合过滤
来源：http://ge.jianghongdianzi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gq.yuntaijiaju.cn

[T56] Scala：样例类
来源：http://ou.huixiangedu.cn

case class User(name: String, age: Int)
来源：http://bd.nicolike.cn

[T57] Scala：模式匹配
来源：http://pb.huanxung.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://dd.szsharing.cn

[T58] Scala：函数定义
来源：http://mv.shxzukj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://iq.shtwfgs.cn

[T59] Scala：循环
来源：http://ng.muxihuayi.cn

for (i <- 1 to 10) println(i)
来源：http://eq.muxihuayi.cn

[T60] Scala：折叠
来源：http://wb.yuexingan06.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bw.huixiangedu.cn

================================================================================
来源：http://ms.haigaiapp.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zn.asd995.cn

================================================================================
来源：http://tj.wgjwhj.cn

[U01] Py：创建虚拟环境
来源：http://oz.521024.cn

python -m venv .venv && source .venv/bin/activate
来源：http://kq.chemitech.net.cn

[U02] Py：导出 / 安装依赖
来源：http://iz.gzmigu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ew.bookmarksfly.cn

[U03] Py：加载 .env 配置
来源：http://xh.shtwfgs.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://jl.9csxet.cn

[U04] Py：变量调试打印
来源：http://nt.colortex.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hf.nszjky.cn

[U05] Py：列表去重且保序
来源：http://wu.huanxung.cn

list(dict.fromkeys(arr))
来源：http://lk.asd995.cn

[U06] Py：合并两个字典
来源：http://jv.jianghongdianzi.cn

{**a, **b}
来源：http://nn.lnxyls.cn

[U07] Py：反转字典键值
来源：http://hk.szsharing.cn

{v: k for k, v in d.items()}
来源：http://lu.521024.cn

[U08] Py：展平二维列表
来源：http://ex.bookmarksfly.cn

[y for x in nested for y in x]
来源：http://wz.jianghongdianzi.cn

[U09] Py：字典取最大值的键
来源：http://yr.nszjky.cn

max(d, key=d.get)
来源：http://wi.lnxyls.cn

[U10] Py：按值排序字典
来源：http://xw.huixinmuqiang.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gv.chemitech.net.cn

[U11] Py：生成器表达式
来源：http://gg.colortex.cn

(x * 2 for x in arr)
来源：http://li.yuntaijiaju.cn

[U12] Py：取出现最多的 3 个元素
来源：http://kf.haigaiapp.cn

Counter(arr).most_common(3)
来源：http://gw.szsharing.cn

[U13] Py：固定长度队列
来源：http://be.szxytkj.cn

deque(maxlen=10)
来源：http://oz.panjiajie.cn

[U14] Py：分组收集到列表
来源：http://uf.shtwfgs.cn

defaultdict(list)
来源：http://tm.yuntaijiaju.cn

[U15] Py：高精度计时
来源：http://hd.hahajie.cn

t = time.perf_counter()
来源：http://xy.jctech888.com.cn

[U16] Py：命令行参数解析
来源：http://uu.jctech888.com.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ke.521024.cn

[U17] Py：初始化日志
来源：http://rz.hnjuh.cn

logging.basicConfig(level=logging.INFO)
来源：http://bs.chemitech.net.cn

[U18] Py：预编译正则
来源：http://np.yuntaijiaju.cn

pat = re.compile(r"\d+")
来源：http://fj.haigaiapp.cn

[U19] Py：正则替换带回调
来源：http://eb.szsharing.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ai.jctech888.com.cn

[U20] Py：缓存函数结果
来源：http://rw.jctech888.com.cn

@functools.lru_cache(maxsize=None)
来源：http://le.haigaiapp.cn

[U21] Py：自定义上下文管理器
来源：http://kj.jctech888.com.cn

@contextlib.contextmanager
来源：http://lq.haigaiapp.cn

[U22] Py：矩阵转置
来源：http://aw.huixinmuqiang.cn

list(zip(*m))
来源：http://ur.haigaiapp.cn

[U23] Py：分块读取大文件
来源：http://wo.panjiajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pf.bjjhwx.cn

[U24] Py：路径操作
来源：http://nz.shxzskj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://oh.wgjwhj.cn

[U25] Py：CSV 按字典读
来源：http://mz.jctech888.com.cn

csv.DictReader(f)
来源：http://zx.huixiangedu.cn

[U26] Py：并发下载
来源：http://nl.panjiajie.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hw.haigaiapp.cn

[U27] Py：异步 HTTP
来源：http://qj.huixiangedu.cn

aiohttp.ClientSession() 配合 async with
来源：http://ef.huixiangedu.cn

[U28] Py：类型别名
来源：http://nq.szxytkj.cn

UserId = int
来源：http://ro.nicolike.cn

[U29] Py：属性校验
来源：http://np.jctech888.com.cn

@property 与 @x.setter 配合
来源：http://mj.nszjky.cn

[U30] Py：数据类
来源：http://fv.colortex.cn

@dataclass(slots=True)
来源：http://kf.bookmarksfly.cn

[U31] Py：单测
来源：http://be.huixinmuqiang.cn

python -m pytest -q
来源：http://qe.shxzukj.cn

[U32] Py：代码格式化
来源：http://cx.yuexingan06.cn

ruff format . && ruff check --fix .
来源：http://gm.shtwfgs.cn

[U33] Py：打包发布
来源：http://jm.lnxyls.cn

python -m build  （依赖 pyproject.toml）
来源：http://ub.colortex.cn

[U34] Py：判断编码
来源：http://bq.lnxyls.cn

chardet.detect(raw)
来源：http://fl.yuntaijiaju.cn

[U35] Py：发送邮件
来源：http://tw.gzmigu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ix.haigaiapp.cn

[U36] Py：定时任务
来源：http://ws.nicolike.cn

schedule.every(10).minutes.do(job)
来源：http://sr.muxihuayi.cn

[U37] Py：读写 Excel
来源：http://bg.lnxyls.cn

pandas.read_excel / DataFrame.to_excel
来源：http://pw.gzmigu.cn

[U38] Py：获取脚本所在目录
来源：http://gm.yuntaijiaju.cn

Path(__file__).resolve().parent
来源：http://pq.jctech888.com.cn

[U39] Py：判断是否在交互环境
来源：http://ty.jctech888.com.cn

sys.stdout.isatty()
来源：http://tx.yuntaijiaju.cn

[U40] Py：打印到标准错误
来源：http://dy.muxihuayi.cn

print("err", file=sys.stderr)
来源：http://qx.9csxet.cn

[U41] PHP：初始化 Composer 项目
来源：http://gm.chemitech.net.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://fi.colortex.cn

[U42] PHP：PSR-4 自动加载
来源：http://gv.haigaiapp.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nd.asd995.cn

[U43] PHP：声明命名空间
来源：http://nr.chemitech.net.cn

namespace App\Http;
来源：http://ma.muxihuayi.cn

[U44] PHP：开启严格类型
来源：http://nq.colortex.cn

declare(strict_types=1);
来源：http://no.huixinmuqiang.cn

[U45] PHP：类型声明与返回类型
来源：http://ht.yuexingan06.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://om.hnjuh.cn

[U46] PHP：可空类型
来源：http://yq.bjjhwx.cn

?string $name = null
来源：http://ns.huixiangedu.cn

[U47] PHP：联合类型
来源：http://uz.muxihuayi.cn

int|string $id
来源：http://ol.521024.cn

[U48] PHP：纯枚举
来源：http://nq.szxytkj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jv.huixiangedu.cn

[U49] PHP：只读属性
来源：http://bu.panjiajie.cn

public readonly string $name
来源：http://nj.lnxyls.cn

[U50] PHP：构造器属性提升
来源：http://xj.asd995.cn

public function __construct(private int $id) {}
来源：http://fe.jctech888.com.cn

[U51] PHP：数组解构
来源：http://jk.panjiajie.cn

[$a, $b] = $arr;
来源：http://ac.shxzukj.cn

[U52] PHP：箭头函数
来源：http://yt.jctech888.com.cn

$double = fn($x) => $x * 2;
来源：http://fr.hnjuh.cn

[U53] PHP：空合并运算符
来源：http://rl.shtwfgs.cn

$v = $a ?? $b ?? "default";
来源：http://yj.hahajie.cn

[U54] PHP：空安全调用
来源：http://ma.jianghongdianzi.cn

$obj?->method()
来源：http://mk.9csxet.cn

[U55] PHP：match 表达式
来源：http://vn.asd995.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://it.asd995.cn

[U56] PHP：命名参数
来源：http://rt.wgjwhj.cn

f(a: 1, b: 2)
来源：http://sm.bookmarksfly.cn

[U57] PHP：字符串插值
来源：http://kt.wgjwhj.cn

"值: {$a}"
来源：http://ld.shtwfgs.cn

[U58] PHP：数组三件套
来源：http://ad.bookmarksfly.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mj.szsharing.cn

[U59] PHP：自定义排序
来源：http://ai.lnxyls.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wc.521024.cn

[U60] PHP：JSON 编解码
来源：http://ls.panjiajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qd.hnjuh.cn

[U61] PHP：正则
来源：http://xy.9csxet.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://eg.yuexingan06.cn

[U62] PHP：日期对象
来源：http://gt.bookmarksfly.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rd.huanxung.cn

[U63] PHP：文件读写
来源：http://gc.yuntaijiaju.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://cy.shtwfgs.cn

[U64] PHP：目录遍历
来源：http://dp.yuexingan06.cn

glob("dir/*.php");  scandir("dir");
来源：http://rv.chemitech.net.cn

[U65] PHP：会话
来源：http://df.jianghongdianzi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://cu.lnxyls.cn

[U66] PHP：设置 Cookie
来源：http://yu.hahajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fo.newstarts.cn

[U67] PHP：处理文件上传
来源：http://kr.muxihuayi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ze.huanxung.cn

[U68] PHP：PDO 连接
来源：http://bd.lnxyls.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fn.jctech888.com.cn

[U69] PHP：PDO 预处理
来源：http://kd.asd995.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://uk.haigaiapp.cn

[U70] PHP：PDO 事务
来源：http://io.521024.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wk.shxzukj.cn

[U71] PHP：抛出异常
来源：http://dc.9csxet.cn

throw new RuntimeException("失败", 500);
来源：http://kj.9csxet.cn

[U72] PHP：写错误日志
来源：http://gl.nicolike.cn

error_log("失败: " . $e->getMessage());
来源：http://fk.panjiajie.cn

[U73] PHP：读取 ini 配置
来源：http://vq.yuntaijiaju.cn

parse_ini_file("config.ini", true)
来源：http://uf.nicolike.cn

[U74] PHP：读取环境变量
来源：http://mw.asd995.cn

getenv("APP_ENV") ?: "production"
来源：http://qr.hahajie.cn

[U75] PHP：依赖注入
来源：http://wf.bjjhwx.cn

composer require psr/container
来源：http://bd.jctech888.com.cn

[U76] PHP：简单路由
来源：http://hh.huanxung.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vw.colortex.cn

[U77] PHP：模板渲染
来源：http://ms.hahajie.cn

composer require twig/twig
来源：http://dc.hahajie.cn

[U78] PHP：单元测试
来源：http://gi.nszjky.cn

composer require --dev phpunit/phpunit
来源：http://ly.asd995.cn

[U79] PHP：静态分析
来源：http://dw.szsharing.cn

composer require --dev phpstan/phpstan
来源：http://pz.jctech888.com.cn

[U80] PHP：代码规范修复
来源：http://ol.bookmarksfly.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://gc.yuexingan06.cn

[U81] JS：初始化项目
来源：http://hl.lnxyls.cn

npm init -y;  npm i express
来源：http://bl.haigaiapp.cn

[U82] JS：package.json 脚本
来源：http://fy.huixinmuqiang.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ns.yuexingan06.cn

[U83] JS：ES Module 导入导出
来源：http://aa.shxzskj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://gb.521024.cn

[U84] JS：CommonJS 写法
来源：http://xa.nicolike.cn

module.exports = { a };  const { a } = require("./m");
来源：http://pv.colortex.cn

[U85] JS：可选链
来源：http://dj.asd995.cn

a?.b?.c
来源：http://ol.nicolike.cn

[U86] JS：空值合并
来源：http://sh.yuntaijiaju.cn

a ?? b
来源：http://ze.jctech888.com.cn

[U87] JS：解构默认值
来源：http://ts.panjiajie.cn

const { a = 1, b = 2 } = obj;
来源：http://gt.hahajie.cn

[U88] JS：对象展开合并
来源：http://bx.jianghongdianzi.cn

{ ...a, ...b }
来源：http://zy.haigaiapp.cn

[U89] JS：数组去重
来源：http://ts.shtwfgs.cn

[...new Set(arr)]
来源：http://oa.9csxet.cn

[U90] JS：数字数组排序
来源：http://pm.bookmarksfly.cn

[...arr].sort((a, b) => a - b)
来源：http://ju.nszjky.cn

[U91] JS：对象键值遍历
来源：http://kk.shtwfgs.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ty.wgjwhj.cn

[U92] JS：深拷贝
来源：http://zl.bjjhwx.cn

structuredClone(obj)
来源：http://ma.szsharing.cn

[U93] JS：模板字符串
来源：http://ko.hahajie.cn

`共 ${n} 条`
来源：http://mn.wgjwhj.cn

[U94] JS：箭头函数
来源：http://em.newstarts.cn

const double = x => x * 2;
来源：http://wf.newstarts.cn

[U95] JS：Promise 包装
来源：http://aw.nszjky.cn

new Promise((resolve, reject) => {})
来源：http://ch.hahajie.cn

[U96] JS：async/await 与异常
来源：http://wy.chemitech.net.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xv.huixiangedu.cn

[U97] JS：并发请求
来源：http://iu.lnxyls.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ew.shxzukj.cn

[U98] JS：fetch 带 JSON
来源：http://zf.nszjky.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tb.9csxet.cn

[U99] JS：事件监听
来源：http://nl.jianghongdianzi.cn

el.addEventListener("click", e => {})
来源：http://zn.521024.cn

[U100] JS：DOM 查询
来源：http://kh.jianghongdianzi.cn

document.querySelector(".item")
来源：http://xf.521024.cn

[U101] JS：classList 操作
来源：http://su.muxihuayi.cn

el.classList.toggle("active")
来源：http://wb.muxihuayi.cn

[U102] JS：本地存储
来源：http://ez.szsharing.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://oi.colortex.cn

[U103] JS：定时器
来源：http://qs.wgjwhj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fi.nszjky.cn

[U104] JS：防抖
来源：http://jr.huixinmuqiang.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fi.bjjhwx.cn

[U105] JS：节流
来源：http://ee.huixinmuqiang.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sf.lnxyls.cn

[U106] JS：日期格式化
来源：http://tn.jianghongdianzi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nc.shxzukj.cn

[U107] JS：数字千分位
来源：http://uy.huanxung.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vw.huanxung.cn

[U108] JS：随机整数
来源：http://dg.huixinmuqiang.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gb.shxzukj.cn

[U109] JS：数组分组
来源：http://rb.hahajie.cn

Object.groupBy(arr, x => x.type)
来源：http://mi.yuntaijiaju.cn

[U110] JS：数组分块
来源：http://cq.nicolike.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qj.9csxet.cn

[U111] JS：对象转 Map
来源：http://wu.bookmarksfly.cn

new Map(Object.entries(obj))
来源：http://pu.jianghongdianzi.cn

[U112] JS：字符串补位
来源：http://sq.wgjwhj.cn

"7".padStart(3, "0")
来源：http://nv.gzmigu.cn

[U113] JS：正则替换全部
来源：http://xx.gzmigu.cn

s.replaceAll("a", "b")
来源：http://kg.wgjwhj.cn

[U114] JS：JSON 深比较
来源：http://ki.colortex.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://yu.bookmarksfly.cn

[U115] JS：生成 UUID
来源：http://wd.bjjhwx.cn

crypto.randomUUID()
来源：http://fb.lnxyls.cn

[U116] JS：类型检查（JSDoc）
来源：http://qk.muxihuayi.cn

/** @param {string} name */ function f(name) {}
来源：http://jo.jctech888.com.cn

[U117] JS：单元测试
来源：http://bs.hahajie.cn

npm i -D vitest;  npx vitest
来源：http://uo.9csxet.cn

[U118] JS：开发服务器
来源：http://pt.chemitech.net.cn

npm i -D vite;  npx vite
来源：http://ti.szsharing.cn

[U119] JS：生产构建
来源：http://nx.panjiajie.cn

npx vite build
来源：http://pp.szxytkj.cn

[U120] JS：读取环境变量（Vite）
来源：http://mm.jctech888.com.cn

import.meta.env.VITE_API_URL
来源：http://dt.shtwfgs.cn

================================================================================
来源：http://fp.huanxung.cn

统计汇总
来源：http://uh.yuntaijiaju.cn

================================================================================
来源：http://fp.nicolike.cn

按语言统计（条）：
来源：http://ew.yuexingan06.cn

Python ......... 252
来源：http://fv.yuntaijiaju.cn

PHP ............ 252
来源：http://wv.chemitech.net.cn

JavaScript ..... 252
来源：http://jy.asd995.cn

TypeScript ..... 212
来源：http://pd.yuntaijiaju.cn

Java ........... 212
来源：http://iu.muxihuayi.cn

Go ............. 212
来源：http://we.wgjwhj.cn

Ruby ........... 212
来源：http://qb.yuexingan06.cn

C# ............. 212
来源：http://nr.lnxyls.cn

C .............. 30
来源：http://al.shtwfgs.cn

C++ ............ 30
来源：http://nz.lnxyls.cn

SQL ............ 90
来源：http://ug.muxihuayi.cn

Bash ........... 80
来源：http://zl.jctech888.com.cn

Kotlin ......... 15
来源：http://vz.hnjuh.cn

Swift .......... 15
来源：http://jo.bjjhwx.cn

Lua ............ 10
来源：http://hf.muxihuayi.cn

Perl ........... 10
来源：http://wn.muxihuayi.cn

Scala .......... 10
来源：http://fg.szxytkj.cn

------------------------------------
来源：http://nm.asd995.cn

合计 ........... 2106 条
来源：http://oh.shtwfgs.cn

按章节统计：
来源：http://ma.9csxet.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lv.szsharing.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://um.jianghongdianzi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pt.wgjwhj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qm.colortex.cn


<!-- 参考信息 -->