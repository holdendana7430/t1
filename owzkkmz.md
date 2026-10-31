代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://qr.521024.cn

[T51] Scala：Hello World
来源：http://by.shtwfgs.cn

println("Hello")
来源：http://zc.shxzukj.cn

[T52] Scala：变量
来源：http://oo.colortex.cn

val a = 1;  var b = 2
来源：http://jc.panjiajie.cn

[T53] Scala：字符串插值
来源：http://gz.colortex.cn

s"值: $b"
来源：http://cu.yuntaijiaju.cn

[T54] Scala：集合映射
来源：http://yd.haigaiapp.cn

List(1, 2, 3).map(_ * 2)
来源：http://hs.bookmarksfly.cn

[T55] Scala：集合过滤
来源：http://yz.jctech888.com.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ca.bjjhwx.cn

[T56] Scala：样例类
来源：http://ix.shtwfgs.cn

case class User(name: String, age: Int)
来源：http://ej.asd995.cn

[T57] Scala：模式匹配
来源：http://bh.gzmigu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vy.lnxyls.cn

[T58] Scala：函数定义
来源：http://bm.yuntaijiaju.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gr.shxzukj.cn

[T59] Scala：循环
来源：http://qf.lnxyls.cn

for (i <- 1 to 10) println(i)
来源：http://bw.colortex.cn

[T60] Scala：折叠
来源：http://oe.newstarts.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gl.lnxyls.cn

================================================================================
来源：http://cz.yuexingan06.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tt.521024.cn

================================================================================
来源：http://hu.jctech888.com.cn

[U01] Py：创建虚拟环境
来源：http://rb.wgjwhj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zf.yuntaijiaju.cn

[U02] Py：导出 / 安装依赖
来源：http://fr.wgjwhj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://im.hahajie.cn

[U03] Py：加载 .env 配置
来源：http://mk.hahajie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fn.panjiajie.cn

[U04] Py：变量调试打印
来源：http://xs.nicolike.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://od.huanxung.cn

[U05] Py：列表去重且保序
来源：http://mc.yuexingan06.cn

list(dict.fromkeys(arr))
来源：http://yk.colortex.cn

[U06] Py：合并两个字典
来源：http://im.bjjhwx.cn

{**a, **b}
来源：http://cc.yuntaijiaju.cn

[U07] Py：反转字典键值
来源：http://sg.szsharing.cn

{v: k for k, v in d.items()}
来源：http://kq.shxzskj.cn

[U08] Py：展平二维列表
来源：http://jp.nicolike.cn

[y for x in nested for y in x]
来源：http://gl.huanxung.cn

[U09] Py：字典取最大值的键
来源：http://np.hnjuh.cn

max(d, key=d.get)
来源：http://vd.newstarts.cn

[U10] Py：按值排序字典
来源：http://ev.shxzskj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mf.nszjky.cn

[U11] Py：生成器表达式
来源：http://fn.shxzukj.cn

(x * 2 for x in arr)
来源：http://mg.colortex.cn

[U12] Py：取出现最多的 3 个元素
来源：http://gz.huixinmuqiang.cn

Counter(arr).most_common(3)
来源：http://nd.bjjhwx.cn

[U13] Py：固定长度队列
来源：http://gx.nszjky.cn

deque(maxlen=10)
来源：http://cb.nszjky.cn

[U14] Py：分组收集到列表
来源：http://zj.hnjuh.cn

defaultdict(list)
来源：http://ma.yuntaijiaju.cn

[U15] Py：高精度计时
来源：http://iu.521024.cn

t = time.perf_counter()
来源：http://zq.shtwfgs.cn

[U16] Py：命令行参数解析
来源：http://pl.yuexingan06.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xk.9csxet.cn

[U17] Py：初始化日志
来源：http://ro.muxihuayi.cn

logging.basicConfig(level=logging.INFO)
来源：http://rb.panjiajie.cn

[U18] Py：预编译正则
来源：http://lf.asd995.cn

pat = re.compile(r"\d+")
来源：http://bs.szxytkj.cn

[U19] Py：正则替换带回调
来源：http://vf.hahajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nd.521024.cn

[U20] Py：缓存函数结果
来源：http://xn.jctech888.com.cn

@functools.lru_cache(maxsize=None)
来源：http://ox.jctech888.com.cn

[U21] Py：自定义上下文管理器
来源：http://vg.asd995.cn

@contextlib.contextmanager
来源：http://yr.bookmarksfly.cn

[U22] Py：矩阵转置
来源：http://lv.muxihuayi.cn

list(zip(*m))
来源：http://je.asd995.cn

[U23] Py：分块读取大文件
来源：http://qg.lnxyls.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ju.yuntaijiaju.cn

[U24] Py：路径操作
来源：http://vf.shxzskj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://id.szxytkj.cn

[U25] Py：CSV 按字典读
来源：http://ny.nszjky.cn

csv.DictReader(f)
来源：http://bw.yuntaijiaju.cn

[U26] Py：并发下载
来源：http://rn.hnjuh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nf.hnjuh.cn

[U27] Py：异步 HTTP
来源：http://aq.szxytkj.cn

aiohttp.ClientSession() 配合 async with
来源：http://fh.yuexingan06.cn

[U28] Py：类型别名
来源：http://mf.jctech888.com.cn

UserId = int
来源：http://mg.jianghongdianzi.cn

[U29] Py：属性校验
来源：http://it.lnxyls.cn

@property 与 @x.setter 配合
来源：http://xb.hahajie.cn

[U30] Py：数据类
来源：http://wn.wgjwhj.cn

@dataclass(slots=True)
来源：http://gq.jctech888.com.cn

[U31] Py：单测
来源：http://vr.jianghongdianzi.cn

python -m pytest -q
来源：http://bq.colortex.cn

[U32] Py：代码格式化
来源：http://un.shxzukj.cn

ruff format . && ruff check --fix .
来源：http://an.panjiajie.cn

[U33] Py：打包发布
来源：http://gq.bookmarksfly.cn

python -m build  （依赖 pyproject.toml）
来源：http://nq.colortex.cn

[U34] Py：判断编码
来源：http://wb.szxytkj.cn

chardet.detect(raw)
来源：http://te.nszjky.cn

[U35] Py：发送邮件
来源：http://un.jianghongdianzi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ym.nicolike.cn

[U36] Py：定时任务
来源：http://bm.newstarts.cn

schedule.every(10).minutes.do(job)
来源：http://er.panjiajie.cn

[U37] Py：读写 Excel
来源：http://ph.nszjky.cn

pandas.read_excel / DataFrame.to_excel
来源：http://fz.wgjwhj.cn

[U38] Py：获取脚本所在目录
来源：http://vg.yuexingan06.cn

Path(__file__).resolve().parent
来源：http://km.panjiajie.cn

[U39] Py：判断是否在交互环境
来源：http://sa.jctech888.com.cn

sys.stdout.isatty()
来源：http://yw.shtwfgs.cn

[U40] Py：打印到标准错误
来源：http://sr.shxzukj.cn

print("err", file=sys.stderr)
来源：http://ui.lnxyls.cn

[U41] PHP：初始化 Composer 项目
来源：http://ok.gzmigu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://cf.haigaiapp.cn

[U42] PHP：PSR-4 自动加载
来源：http://go.panjiajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mf.asd995.cn

[U43] PHP：声明命名空间
来源：http://oy.haigaiapp.cn

namespace App\Http;
来源：http://vn.huanxung.cn

[U44] PHP：开启严格类型
来源：http://tp.newstarts.cn

declare(strict_types=1);
来源：http://dn.yuntaijiaju.cn

[U45] PHP：类型声明与返回类型
来源：http://lo.newstarts.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://wb.gzmigu.cn

[U46] PHP：可空类型
来源：http://gc.bjjhwx.cn

?string $name = null
来源：http://nl.wgjwhj.cn

[U47] PHP：联合类型
来源：http://rd.szsharing.cn

int|string $id
来源：http://wy.521024.cn

[U48] PHP：纯枚举
来源：http://ln.yuexingan06.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tr.yuntaijiaju.cn

[U49] PHP：只读属性
来源：http://bc.wgjwhj.cn

public readonly string $name
来源：http://kh.shxzukj.cn

[U50] PHP：构造器属性提升
来源：http://bm.jianghongdianzi.cn

public function __construct(private int $id) {}
来源：http://tq.panjiajie.cn

[U51] PHP：数组解构
来源：http://hk.bookmarksfly.cn

[$a, $b] = $arr;
来源：http://dm.panjiajie.cn

[U52] PHP：箭头函数
来源：http://kg.huanxung.cn

$double = fn($x) => $x * 2;
来源：http://un.huixiangedu.cn

[U53] PHP：空合并运算符
来源：http://hz.lnxyls.cn

$v = $a ?? $b ?? "default";
来源：http://wq.panjiajie.cn

[U54] PHP：空安全调用
来源：http://il.nszjky.cn

$obj?->method()
来源：http://kk.jianghongdianzi.cn

[U55] PHP：match 表达式
来源：http://bv.shxzukj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kw.bjjhwx.cn

[U56] PHP：命名参数
来源：http://os.bjjhwx.cn

f(a: 1, b: 2)
来源：http://ng.hnjuh.cn

[U57] PHP：字符串插值
来源：http://ir.yuexingan06.cn

"值: {$a}"
来源：http://xm.huixiangedu.cn

[U58] PHP：数组三件套
来源：http://fn.shxzskj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ru.shxzukj.cn

[U59] PHP：自定义排序
来源：http://wt.shxzukj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pc.yuexingan06.cn

[U60] PHP：JSON 编解码
来源：http://su.bookmarksfly.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://al.hahajie.cn

[U61] PHP：正则
来源：http://la.bjjhwx.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hk.huanxung.cn

[U62] PHP：日期对象
来源：http://vp.bjjhwx.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://er.colortex.cn

[U63] PHP：文件读写
来源：http://xm.huixiangedu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://id.bjjhwx.cn

[U64] PHP：目录遍历
来源：http://ez.shxzukj.cn

glob("dir/*.php");  scandir("dir");
来源：http://ho.nicolike.cn

[U65] PHP：会话
来源：http://rv.yuntaijiaju.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ks.huanxung.cn

[U66] PHP：设置 Cookie
来源：http://qf.gzmigu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://oy.szsharing.cn

[U67] PHP：处理文件上传
来源：http://rn.lnxyls.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mt.lnxyls.cn

[U68] PHP：PDO 连接
来源：http://lw.shtwfgs.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hp.chemitech.net.cn

[U69] PHP：PDO 预处理
来源：http://az.nicolike.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jn.gzmigu.cn

[U70] PHP：PDO 事务
来源：http://fe.newstarts.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zd.bjjhwx.cn

[U71] PHP：抛出异常
来源：http://os.szsharing.cn

throw new RuntimeException("失败", 500);
来源：http://cn.bookmarksfly.cn

[U72] PHP：写错误日志
来源：http://rd.9csxet.cn

error_log("失败: " . $e->getMessage());
来源：http://fb.yuntaijiaju.cn

[U73] PHP：读取 ini 配置
来源：http://ow.chemitech.net.cn

parse_ini_file("config.ini", true)
来源：http://qf.521024.cn

[U74] PHP：读取环境变量
来源：http://ai.hnjuh.cn

getenv("APP_ENV") ?: "production"
来源：http://mm.9csxet.cn

[U75] PHP：依赖注入
来源：http://fz.shtwfgs.cn

composer require psr/container
来源：http://kl.hahajie.cn

[U76] PHP：简单路由
来源：http://ir.521024.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rz.colortex.cn

[U77] PHP：模板渲染
来源：http://xa.bjjhwx.cn

composer require twig/twig
来源：http://rm.nicolike.cn

[U78] PHP：单元测试
来源：http://ar.bookmarksfly.cn

composer require --dev phpunit/phpunit
来源：http://pv.lnxyls.cn

[U79] PHP：静态分析
来源：http://ob.nszjky.cn

composer require --dev phpstan/phpstan
来源：http://oq.wgjwhj.cn

[U80] PHP：代码规范修复
来源：http://tz.shxzukj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://oo.gzmigu.cn

[U81] JS：初始化项目
来源：http://sk.bookmarksfly.cn

npm init -y;  npm i express
来源：http://yz.shxzukj.cn

[U82] JS：package.json 脚本
来源：http://et.bookmarksfly.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bi.muxihuayi.cn

[U83] JS：ES Module 导入导出
来源：http://eh.chemitech.net.cn

export const a = 1;  import { a } from "./m.js";
来源：http://yw.haigaiapp.cn

[U84] JS：CommonJS 写法
来源：http://vu.521024.cn

module.exports = { a };  const { a } = require("./m");
来源：http://hz.bjjhwx.cn

[U85] JS：可选链
来源：http://lo.nicolike.cn

a?.b?.c
来源：http://ku.haigaiapp.cn

[U86] JS：空值合并
来源：http://oy.huanxung.cn

a ?? b
来源：http://oj.chemitech.net.cn

[U87] JS：解构默认值
来源：http://dd.huanxung.cn

const { a = 1, b = 2 } = obj;
来源：http://ur.bookmarksfly.cn

[U88] JS：对象展开合并
来源：http://ob.bjjhwx.cn

{ ...a, ...b }
来源：http://cq.huixinmuqiang.cn

[U89] JS：数组去重
来源：http://am.chemitech.net.cn

[...new Set(arr)]
来源：http://xz.jianghongdianzi.cn

[U90] JS：数字数组排序
来源：http://gj.hahajie.cn

[...arr].sort((a, b) => a - b)
来源：http://ec.bjjhwx.cn

[U91] JS：对象键值遍历
来源：http://cq.huixinmuqiang.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qm.gzmigu.cn

[U92] JS：深拷贝
来源：http://gn.szxytkj.cn

structuredClone(obj)
来源：http://fh.bookmarksfly.cn

[U93] JS：模板字符串
来源：http://pr.shtwfgs.cn

`共 ${n} 条`
来源：http://kz.haigaiapp.cn

[U94] JS：箭头函数
来源：http://pf.hahajie.cn

const double = x => x * 2;
来源：http://dk.panjiajie.cn

[U95] JS：Promise 包装
来源：http://so.bjjhwx.cn

new Promise((resolve, reject) => {})
来源：http://df.szsharing.cn

[U96] JS：async/await 与异常
来源：http://ze.newstarts.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ab.szxytkj.cn

[U97] JS：并发请求
来源：http://gp.colortex.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://cf.wgjwhj.cn

[U98] JS：fetch 带 JSON
来源：http://rj.jianghongdianzi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://oh.hnjuh.cn

[U99] JS：事件监听
来源：http://mr.wgjwhj.cn

el.addEventListener("click", e => {})
来源：http://gz.yuexingan06.cn

[U100] JS：DOM 查询
来源：http://zs.huixiangedu.cn

document.querySelector(".item")
来源：http://nn.gzmigu.cn

[U101] JS：classList 操作
来源：http://aa.asd995.cn

el.classList.toggle("active")
来源：http://qp.jctech888.com.cn

[U102] JS：本地存储
来源：http://bw.colortex.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://dn.huanxung.cn

[U103] JS：定时器
来源：http://un.gzmigu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fw.jianghongdianzi.cn

[U104] JS：防抖
来源：http://by.huanxung.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uf.chemitech.net.cn

[U105] JS：节流
来源：http://ju.haigaiapp.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nd.shxzskj.cn

[U106] JS：日期格式化
来源：http://dr.szxytkj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xw.muxihuayi.cn

[U107] JS：数字千分位
来源：http://tp.colortex.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ni.huixinmuqiang.cn

[U108] JS：随机整数
来源：http://nu.asd995.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://da.bookmarksfly.cn

[U109] JS：数组分组
来源：http://ul.shxzskj.cn

Object.groupBy(arr, x => x.type)
来源：http://cg.nicolike.cn

[U110] JS：数组分块
来源：http://bk.haigaiapp.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kf.szsharing.cn

[U111] JS：对象转 Map
来源：http://gu.asd995.cn

new Map(Object.entries(obj))
来源：http://rg.hnjuh.cn

[U112] JS：字符串补位
来源：http://tc.hnjuh.cn

"7".padStart(3, "0")
来源：http://rf.szsharing.cn

[U113] JS：正则替换全部
来源：http://sc.yuntaijiaju.cn

s.replaceAll("a", "b")
来源：http://gl.shtwfgs.cn

[U114] JS：JSON 深比较
来源：http://wp.shxzukj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://dk.newstarts.cn

[U115] JS：生成 UUID
来源：http://gy.hnjuh.cn

crypto.randomUUID()
来源：http://dz.muxihuayi.cn

[U116] JS：类型检查（JSDoc）
来源：http://ls.shxzukj.cn

/** @param {string} name */ function f(name) {}
来源：http://zm.yuexingan06.cn

[U117] JS：单元测试
来源：http://pi.lnxyls.cn

npm i -D vitest;  npx vitest
来源：http://hm.panjiajie.cn

[U118] JS：开发服务器
来源：http://nk.9csxet.cn

npm i -D vite;  npx vite
来源：http://ho.muxihuayi.cn

[U119] JS：生产构建
来源：http://de.newstarts.cn

npx vite build
来源：http://jw.hnjuh.cn

[U120] JS：读取环境变量（Vite）
来源：http://im.haigaiapp.cn

import.meta.env.VITE_API_URL
来源：http://rf.huixinmuqiang.cn

================================================================================
来源：http://jv.hahajie.cn

统计汇总
来源：http://iq.colortex.cn

================================================================================
来源：http://bg.9csxet.cn

按语言统计（条）：
来源：http://ju.colortex.cn

Python ......... 252
来源：http://pa.9csxet.cn

PHP ............ 252
来源：http://kx.huanxung.cn

JavaScript ..... 252
来源：http://kf.yuntaijiaju.cn

TypeScript ..... 212
来源：http://qn.yuntaijiaju.cn

Java ........... 212
来源：http://zi.yuexingan06.cn

Go ............. 212
来源：http://ll.nszjky.cn

Ruby ........... 212
来源：http://xw.panjiajie.cn

C# ............. 212
来源：http://ue.jctech888.com.cn

C .............. 30
来源：http://ox.huixinmuqiang.cn

C++ ............ 30
来源：http://ki.yuntaijiaju.cn

SQL ............ 90
来源：http://vf.shxzukj.cn

Bash ........... 80
来源：http://hs.jianghongdianzi.cn

Kotlin ......... 15
来源：http://ap.hnjuh.cn

Swift .......... 15
来源：http://yn.jianghongdianzi.cn

Lua ............ 10
来源：http://ek.521024.cn

Perl ........... 10
来源：http://ii.lnxyls.cn

Scala .......... 10
来源：http://ep.huixiangedu.cn

------------------------------------
来源：http://sl.yuntaijiaju.cn

合计 ........... 2106 条
来源：http://kz.haigaiapp.cn

按章节统计：
来源：http://zo.nicolike.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ms.huixinmuqiang.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bw.bjjhwx.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pq.hahajie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zb.muxihuayi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lc.huixiangedu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fr.jctech888.com.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.lnxyls.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://da.newstarts.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wd.hnjuh.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://sn.nicolike.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ka.wgjwhj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wm.wgjwhj.cn


<!-- 参考信息 -->