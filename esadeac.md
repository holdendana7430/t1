代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://wu.wgjwhj.cn

[T51] Scala：Hello World
来源：http://vw.szsharing.cn

println("Hello")
来源：http://id.chemitech.net.cn

[T52] Scala：变量
来源：http://uu.shxzukj.cn

val a = 1;  var b = 2
来源：http://hq.szxytkj.cn

[T53] Scala：字符串插值
来源：http://qc.nszjky.cn

s"值: $b"
来源：http://er.chemitech.net.cn

[T54] Scala：集合映射
来源：http://ki.jctech888.com.cn

List(1, 2, 3).map(_ * 2)
来源：http://ln.jianghongdianzi.cn

[T55] Scala：集合过滤
来源：http://fd.huixiangedu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xf.shxzukj.cn

[T56] Scala：样例类
来源：http://ka.szsharing.cn

case class User(name: String, age: Int)
来源：http://qz.shxzskj.cn

[T57] Scala：模式匹配
来源：http://bv.chemitech.net.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://bt.newstarts.cn

[T58] Scala：函数定义
来源：http://sn.wgjwhj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://uz.nszjky.cn

[T59] Scala：循环
来源：http://au.jianghongdianzi.cn

for (i <- 1 to 10) println(i)
来源：http://xd.hnjuh.cn

[T60] Scala：折叠
来源：http://df.newstarts.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fd.hnjuh.cn

================================================================================
来源：http://og.shxzukj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wg.chemitech.net.cn

================================================================================
来源：http://gl.colortex.cn

[U01] Py：创建虚拟环境
来源：http://ga.yuntaijiaju.cn

python -m venv .venv && source .venv/bin/activate
来源：http://de.jctech888.com.cn

[U02] Py：导出 / 安装依赖
来源：http://nj.shtwfgs.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mj.shxzskj.cn

[U03] Py：加载 .env 配置
来源：http://pb.nszjky.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fq.szxytkj.cn

[U04] Py：变量调试打印
来源：http://uv.9csxet.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wk.shxzskj.cn

[U05] Py：列表去重且保序
来源：http://xo.521024.cn

list(dict.fromkeys(arr))
来源：http://ym.huanxung.cn

[U06] Py：合并两个字典
来源：http://gq.haigaiapp.cn

{**a, **b}
来源：http://si.shxzskj.cn

[U07] Py：反转字典键值
来源：http://jd.panjiajie.cn

{v: k for k, v in d.items()}
来源：http://bz.hahajie.cn

[U08] Py：展平二维列表
来源：http://ou.yuexingan06.cn

[y for x in nested for y in x]
来源：http://wx.asd995.cn

[U09] Py：字典取最大值的键
来源：http://yb.huixiangedu.cn

max(d, key=d.get)
来源：http://lv.yuexingan06.cn

[U10] Py：按值排序字典
来源：http://li.szxytkj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wy.hnjuh.cn

[U11] Py：生成器表达式
来源：http://ml.colortex.cn

(x * 2 for x in arr)
来源：http://ag.9csxet.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ku.panjiajie.cn

Counter(arr).most_common(3)
来源：http://wc.huixinmuqiang.cn

[U13] Py：固定长度队列
来源：http://cz.yuntaijiaju.cn

deque(maxlen=10)
来源：http://jd.huixiangedu.cn

[U14] Py：分组收集到列表
来源：http://jl.jianghongdianzi.cn

defaultdict(list)
来源：http://db.huixinmuqiang.cn

[U15] Py：高精度计时
来源：http://re.haigaiapp.cn

t = time.perf_counter()
来源：http://aa.nszjky.cn

[U16] Py：命令行参数解析
来源：http://gp.nszjky.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dy.newstarts.cn

[U17] Py：初始化日志
来源：http://im.lnxyls.cn

logging.basicConfig(level=logging.INFO)
来源：http://un.yuntaijiaju.cn

[U18] Py：预编译正则
来源：http://tm.muxihuayi.cn

pat = re.compile(r"\d+")
来源：http://nv.huixiangedu.cn

[U19] Py：正则替换带回调
来源：http://wj.szsharing.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lo.szsharing.cn

[U20] Py：缓存函数结果
来源：http://hn.jianghongdianzi.cn

@functools.lru_cache(maxsize=None)
来源：http://pe.panjiajie.cn

[U21] Py：自定义上下文管理器
来源：http://dt.newstarts.cn

@contextlib.contextmanager
来源：http://ha.hnjuh.cn

[U22] Py：矩阵转置
来源：http://zs.szxytkj.cn

list(zip(*m))
来源：http://bx.colortex.cn

[U23] Py：分块读取大文件
来源：http://pz.yuntaijiaju.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nu.nszjky.cn

[U24] Py：路径操作
来源：http://hn.wgjwhj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://on.szsharing.cn

[U25] Py：CSV 按字典读
来源：http://qz.jianghongdianzi.cn

csv.DictReader(f)
来源：http://bu.colortex.cn

[U26] Py：并发下载
来源：http://iv.gzmigu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gj.yuntaijiaju.cn

[U27] Py：异步 HTTP
来源：http://lp.newstarts.cn

aiohttp.ClientSession() 配合 async with
来源：http://md.shtwfgs.cn

[U28] Py：类型别名
来源：http://ul.bjjhwx.cn

UserId = int
来源：http://ju.jctech888.com.cn

[U29] Py：属性校验
来源：http://ov.chemitech.net.cn

@property 与 @x.setter 配合
来源：http://ub.asd995.cn

[U30] Py：数据类
来源：http://ti.9csxet.cn

@dataclass(slots=True)
来源：http://qd.hnjuh.cn

[U31] Py：单测
来源：http://hh.bookmarksfly.cn

python -m pytest -q
来源：http://qa.yuntaijiaju.cn

[U32] Py：代码格式化
来源：http://hy.panjiajie.cn

ruff format . && ruff check --fix .
来源：http://wf.panjiajie.cn

[U33] Py：打包发布
来源：http://lk.hahajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://ym.haigaiapp.cn

[U34] Py：判断编码
来源：http://am.yuexingan06.cn

chardet.detect(raw)
来源：http://wp.huixinmuqiang.cn

[U35] Py：发送邮件
来源：http://de.yuntaijiaju.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qx.nicolike.cn

[U36] Py：定时任务
来源：http://we.shtwfgs.cn

schedule.every(10).minutes.do(job)
来源：http://nh.bjjhwx.cn

[U37] Py：读写 Excel
来源：http://sc.nszjky.cn

pandas.read_excel / DataFrame.to_excel
来源：http://kk.lnxyls.cn

[U38] Py：获取脚本所在目录
来源：http://ee.521024.cn

Path(__file__).resolve().parent
来源：http://hy.nicolike.cn

[U39] Py：判断是否在交互环境
来源：http://lt.hahajie.cn

sys.stdout.isatty()
来源：http://xd.szsharing.cn

[U40] Py：打印到标准错误
来源：http://yi.bookmarksfly.cn

print("err", file=sys.stderr)
来源：http://zy.wgjwhj.cn

[U41] PHP：初始化 Composer 项目
来源：http://mx.bjjhwx.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ua.muxihuayi.cn

[U42] PHP：PSR-4 自动加载
来源：http://dz.hnjuh.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kp.newstarts.cn

[U43] PHP：声明命名空间
来源：http://ui.lnxyls.cn

namespace App\Http;
来源：http://hn.wgjwhj.cn

[U44] PHP：开启严格类型
来源：http://oa.muxihuayi.cn

declare(strict_types=1);
来源：http://ab.jianghongdianzi.cn

[U45] PHP：类型声明与返回类型
来源：http://uf.9csxet.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ar.wgjwhj.cn

[U46] PHP：可空类型
来源：http://cv.hnjuh.cn

?string $name = null
来源：http://va.wgjwhj.cn

[U47] PHP：联合类型
来源：http://ei.colortex.cn

int|string $id
来源：http://rz.yuexingan06.cn

[U48] PHP：纯枚举
来源：http://kh.jctech888.com.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://io.panjiajie.cn

[U49] PHP：只读属性
来源：http://th.wgjwhj.cn

public readonly string $name
来源：http://hn.colortex.cn

[U50] PHP：构造器属性提升
来源：http://av.bjjhwx.cn

public function __construct(private int $id) {}
来源：http://cu.521024.cn

[U51] PHP：数组解构
来源：http://zu.szsharing.cn

[$a, $b] = $arr;
来源：http://ml.yuexingan06.cn

[U52] PHP：箭头函数
来源：http://rt.huanxung.cn

$double = fn($x) => $x * 2;
来源：http://mt.bookmarksfly.cn

[U53] PHP：空合并运算符
来源：http://gw.shxzskj.cn

$v = $a ?? $b ?? "default";
来源：http://tz.haigaiapp.cn

[U54] PHP：空安全调用
来源：http://ec.muxihuayi.cn

$obj?->method()
来源：http://st.bjjhwx.cn

[U55] PHP：match 表达式
来源：http://nm.jctech888.com.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://of.bookmarksfly.cn

[U56] PHP：命名参数
来源：http://ru.huixiangedu.cn

f(a: 1, b: 2)
来源：http://ly.newstarts.cn

[U57] PHP：字符串插值
来源：http://sf.nszjky.cn

"值: {$a}"
来源：http://hb.shtwfgs.cn

[U58] PHP：数组三件套
来源：http://yx.wgjwhj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://sa.bookmarksfly.cn

[U59] PHP：自定义排序
来源：http://gu.colortex.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nd.szxytkj.cn

[U60] PHP：JSON 编解码
来源：http://os.wgjwhj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lc.nicolike.cn

[U61] PHP：正则
来源：http://nb.szsharing.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rc.szxytkj.cn

[U62] PHP：日期对象
来源：http://vm.jianghongdianzi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ms.muxihuayi.cn

[U63] PHP：文件读写
来源：http://zh.bookmarksfly.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sv.hnjuh.cn

[U64] PHP：目录遍历
来源：http://bq.asd995.cn

glob("dir/*.php");  scandir("dir");
来源：http://sg.shxzskj.cn

[U65] PHP：会话
来源：http://bi.9csxet.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://da.colortex.cn

[U66] PHP：设置 Cookie
来源：http://fa.lnxyls.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://if.jctech888.com.cn

[U67] PHP：处理文件上传
来源：http://tt.yuntaijiaju.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ox.yuexingan06.cn

[U68] PHP：PDO 连接
来源：http://vx.shtwfgs.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://os.bjjhwx.cn

[U69] PHP：PDO 预处理
来源：http://ua.asd995.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://du.521024.cn

[U70] PHP：PDO 事务
来源：http://qo.shxzukj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://td.wgjwhj.cn

[U71] PHP：抛出异常
来源：http://gv.nszjky.cn

throw new RuntimeException("失败", 500);
来源：http://wk.wgjwhj.cn

[U72] PHP：写错误日志
来源：http://ab.yuexingan06.cn

error_log("失败: " . $e->getMessage());
来源：http://es.huixiangedu.cn

[U73] PHP：读取 ini 配置
来源：http://qv.huixiangedu.cn

parse_ini_file("config.ini", true)
来源：http://hd.chemitech.net.cn

[U74] PHP：读取环境变量
来源：http://sb.521024.cn

getenv("APP_ENV") ?: "production"
来源：http://js.shxzukj.cn

[U75] PHP：依赖注入
来源：http://xx.jctech888.com.cn

composer require psr/container
来源：http://wt.nicolike.cn

[U76] PHP：简单路由
来源：http://ff.huixinmuqiang.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nj.haigaiapp.cn

[U77] PHP：模板渲染
来源：http://om.yuexingan06.cn

composer require twig/twig
来源：http://xt.newstarts.cn

[U78] PHP：单元测试
来源：http://gr.521024.cn

composer require --dev phpunit/phpunit
来源：http://qx.chemitech.net.cn

[U79] PHP：静态分析
来源：http://xk.gzmigu.cn

composer require --dev phpstan/phpstan
来源：http://bb.nszjky.cn

[U80] PHP：代码规范修复
来源：http://wc.9csxet.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://vn.yuntaijiaju.cn

[U81] JS：初始化项目
来源：http://hv.huanxung.cn

npm init -y;  npm i express
来源：http://ek.hnjuh.cn

[U82] JS：package.json 脚本
来源：http://li.jctech888.com.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://uh.huixinmuqiang.cn

[U83] JS：ES Module 导入导出
来源：http://wh.9csxet.cn

export const a = 1;  import { a } from "./m.js";
来源：http://yp.521024.cn

[U84] JS：CommonJS 写法
来源：http://ws.hnjuh.cn

module.exports = { a };  const { a } = require("./m");
来源：http://xz.gzmigu.cn

[U85] JS：可选链
来源：http://pn.yuntaijiaju.cn

a?.b?.c
来源：http://rd.huixiangedu.cn

[U86] JS：空值合并
来源：http://kl.bjjhwx.cn

a ?? b
来源：http://uw.521024.cn

[U87] JS：解构默认值
来源：http://kw.lnxyls.cn

const { a = 1, b = 2 } = obj;
来源：http://mq.yuexingan06.cn

[U88] JS：对象展开合并
来源：http://cz.nszjky.cn

{ ...a, ...b }
来源：http://ur.jctech888.com.cn

[U89] JS：数组去重
来源：http://zv.huixiangedu.cn

[...new Set(arr)]
来源：http://ip.gzmigu.cn

[U90] JS：数字数组排序
来源：http://xp.newstarts.cn

[...arr].sort((a, b) => a - b)
来源：http://dy.muxihuayi.cn

[U91] JS：对象键值遍历
来源：http://to.chemitech.net.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kw.shxzukj.cn

[U92] JS：深拷贝
来源：http://ri.hnjuh.cn

structuredClone(obj)
来源：http://ig.wgjwhj.cn

[U93] JS：模板字符串
来源：http://ea.nszjky.cn

`共 ${n} 条`
来源：http://sz.bookmarksfly.cn

[U94] JS：箭头函数
来源：http://pg.newstarts.cn

const double = x => x * 2;
来源：http://vb.jianghongdianzi.cn

[U95] JS：Promise 包装
来源：http://ak.colortex.cn

new Promise((resolve, reject) => {})
来源：http://zt.huixinmuqiang.cn

[U96] JS：async/await 与异常
来源：http://do.shxzukj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gu.lnxyls.cn

[U97] JS：并发请求
来源：http://ao.newstarts.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rq.szxytkj.cn

[U98] JS：fetch 带 JSON
来源：http://lz.asd995.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gj.huixinmuqiang.cn

[U99] JS：事件监听
来源：http://zz.haigaiapp.cn

el.addEventListener("click", e => {})
来源：http://dx.jianghongdianzi.cn

[U100] JS：DOM 查询
来源：http://hn.gzmigu.cn

document.querySelector(".item")
来源：http://mp.gzmigu.cn

[U101] JS：classList 操作
来源：http://kg.haigaiapp.cn

el.classList.toggle("active")
来源：http://bv.szxytkj.cn

[U102] JS：本地存储
来源：http://ln.panjiajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://dl.jctech888.com.cn

[U103] JS：定时器
来源：http://bj.nicolike.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ze.nszjky.cn

[U104] JS：防抖
来源：http://km.chemitech.net.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zu.yuexingan06.cn

[U105] JS：节流
来源：http://hc.wgjwhj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cv.521024.cn

[U106] JS：日期格式化
来源：http://db.hnjuh.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xy.muxihuayi.cn

[U107] JS：数字千分位
来源：http://ma.nicolike.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hw.hahajie.cn

[U108] JS：随机整数
来源：http://yk.bjjhwx.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tm.hnjuh.cn

[U109] JS：数组分组
来源：http://jp.haigaiapp.cn

Object.groupBy(arr, x => x.type)
来源：http://mt.szsharing.cn

[U110] JS：数组分块
来源：http://kt.gzmigu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nr.shtwfgs.cn

[U111] JS：对象转 Map
来源：http://dn.yuexingan06.cn

new Map(Object.entries(obj))
来源：http://lr.huanxung.cn

[U112] JS：字符串补位
来源：http://ke.chemitech.net.cn

"7".padStart(3, "0")
来源：http://lx.bjjhwx.cn

[U113] JS：正则替换全部
来源：http://od.521024.cn

s.replaceAll("a", "b")
来源：http://mx.jianghongdianzi.cn

[U114] JS：JSON 深比较
来源：http://ik.yuexingan06.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://wm.colortex.cn

[U115] JS：生成 UUID
来源：http://cd.shxzskj.cn

crypto.randomUUID()
来源：http://ul.nicolike.cn

[U116] JS：类型检查（JSDoc）
来源：http://lw.wgjwhj.cn

/** @param {string} name */ function f(name) {}
来源：http://au.shxzskj.cn

[U117] JS：单元测试
来源：http://ve.521024.cn

npm i -D vitest;  npx vitest
来源：http://vs.nicolike.cn

[U118] JS：开发服务器
来源：http://zl.colortex.cn

npm i -D vite;  npx vite
来源：http://tb.asd995.cn

[U119] JS：生产构建
来源：http://af.yuexingan06.cn

npx vite build
来源：http://ih.yuexingan06.cn

[U120] JS：读取环境变量（Vite）
来源：http://jc.nicolike.cn

import.meta.env.VITE_API_URL
来源：http://nx.asd995.cn

================================================================================
来源：http://us.haigaiapp.cn

统计汇总
来源：http://ru.szsharing.cn

================================================================================
来源：http://ku.521024.cn

按语言统计（条）：
来源：http://vf.wgjwhj.cn

Python ......... 252
来源：http://cy.gzmigu.cn

PHP ............ 252
来源：http://gp.lnxyls.cn

JavaScript ..... 252
来源：http://nf.yuntaijiaju.cn

TypeScript ..... 212
来源：http://zt.shxzukj.cn

Java ........... 212
来源：http://rw.gzmigu.cn

Go ............. 212
来源：http://as.nicolike.cn

Ruby ........... 212
来源：http://ho.chemitech.net.cn

C# ............. 212
来源：http://wz.shxzukj.cn

C .............. 30
来源：http://yu.huixinmuqiang.cn

C++ ............ 30
来源：http://yx.bookmarksfly.cn

SQL ............ 90
来源：http://ml.chemitech.net.cn

Bash ........... 80
来源：http://ku.huixinmuqiang.cn

Kotlin ......... 15
来源：http://bo.jctech888.com.cn

Swift .......... 15
来源：http://oc.jctech888.com.cn

Lua ............ 10
来源：http://gg.panjiajie.cn

Perl ........... 10
来源：http://ob.lnxyls.cn

Scala .......... 10
来源：http://kx.521024.cn

------------------------------------
来源：http://ds.lnxyls.cn

合计 ........... 2106 条
来源：http://ov.9csxet.cn

按章节统计：
来源：http://zx.hnjuh.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xj.yuntaijiaju.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ru.jctech888.com.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tk.shxzskj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nr.panjiajie.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ic.shxzskj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://aq.nicolike.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zk.bookmarksfly.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pp.9csxet.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://em.asd995.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ud.jctech888.com.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xe.huixinmuqiang.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wu.shxzukj.cn


<!-- 参考信息 -->