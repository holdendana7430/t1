代发 wailian999

val a = 1;  var b = 2
来源：http://fc.shxzskj.cn

[T53] Scala：字符串插值
来源：http://iv.nicolike.cn

s"值: $b"
来源：http://hv.huixiangedu.cn

[T54] Scala：集合映射
来源：http://nx.jctech888.com.cn

List(1, 2, 3).map(_ * 2)
来源：http://hy.bjjhwx.cn

[T55] Scala：集合过滤
来源：http://gw.521024.cn

List(1, 2, 3).filter(_ > 1)
来源：http://dw.yuexingan06.cn

[T56] Scala：样例类
来源：http://uh.nicolike.cn

case class User(name: String, age: Int)
来源：http://aq.bjjhwx.cn

[T57] Scala：模式匹配
来源：http://sb.newstarts.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://qs.9csxet.cn

[T58] Scala：函数定义
来源：http://lo.nszjky.cn

def add(a: Int, b: Int): Int = a + b
来源：http://cd.szsharing.cn

[T59] Scala：循环
来源：http://uu.panjiajie.cn

for (i <- 1 to 10) println(i)
来源：http://sn.shtwfgs.cn

[T60] Scala：折叠
来源：http://sl.szxytkj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zw.newstarts.cn

================================================================================
来源：http://yx.muxihuayi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vz.huanxung.cn

================================================================================
来源：http://my.bjjhwx.cn

[U01] Py：创建虚拟环境
来源：http://cv.huanxung.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ml.shxzukj.cn

[U02] Py：导出 / 安装依赖
来源：http://av.521024.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ll.nicolike.cn

[U03] Py：加载 .env 配置
来源：http://rq.jianghongdianzi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://mz.nicolike.cn

[U04] Py：变量调试打印
来源：http://dh.panjiajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lq.chemitech.net.cn

[U05] Py：列表去重且保序
来源：http://hi.huixiangedu.cn

list(dict.fromkeys(arr))
来源：http://td.shxzukj.cn

[U06] Py：合并两个字典
来源：http://fr.muxihuayi.cn

{**a, **b}
来源：http://xi.muxihuayi.cn

[U07] Py：反转字典键值
来源：http://nz.jctech888.com.cn

{v: k for k, v in d.items()}
来源：http://cr.shxzskj.cn

[U08] Py：展平二维列表
来源：http://ot.jctech888.com.cn

[y for x in nested for y in x]
来源：http://fb.shtwfgs.cn

[U09] Py：字典取最大值的键
来源：http://ny.huixinmuqiang.cn

max(d, key=d.get)
来源：http://cj.panjiajie.cn

[U10] Py：按值排序字典
来源：http://uj.jianghongdianzi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wn.shxzskj.cn

[U11] Py：生成器表达式
来源：http://wl.haigaiapp.cn

(x * 2 for x in arr)
来源：http://dl.chemitech.net.cn

[U12] Py：取出现最多的 3 个元素
来源：http://vt.shxzskj.cn

Counter(arr).most_common(3)
来源：http://cv.shtwfgs.cn

[U13] Py：固定长度队列
来源：http://sc.9csxet.cn

deque(maxlen=10)
来源：http://mh.yuexingan06.cn

[U14] Py：分组收集到列表
来源：http://tn.bookmarksfly.cn

defaultdict(list)
来源：http://iw.newstarts.cn

[U15] Py：高精度计时
来源：http://uo.asd995.cn

t = time.perf_counter()
来源：http://sp.gzmigu.cn

[U16] Py：命令行参数解析
来源：http://zq.huixiangedu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dj.jianghongdianzi.cn

[U17] Py：初始化日志
来源：http://tc.chemitech.net.cn

logging.basicConfig(level=logging.INFO)
来源：http://gq.muxihuayi.cn

[U18] Py：预编译正则
来源：http://hx.521024.cn

pat = re.compile(r"\d+")
来源：http://ie.yuntaijiaju.cn

[U19] Py：正则替换带回调
来源：http://eq.chemitech.net.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ke.9csxet.cn

[U20] Py：缓存函数结果
来源：http://vm.9csxet.cn

@functools.lru_cache(maxsize=None)
来源：http://ws.wgjwhj.cn

[U21] Py：自定义上下文管理器
来源：http://tm.chemitech.net.cn

@contextlib.contextmanager
来源：http://xb.bjjhwx.cn

[U22] Py：矩阵转置
来源：http://tf.colortex.cn

list(zip(*m))
来源：http://xw.szsharing.cn

[U23] Py：分块读取大文件
来源：http://mi.huixiangedu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ps.nicolike.cn

[U24] Py：路径操作
来源：http://ed.yuexingan06.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wx.asd995.cn

[U25] Py：CSV 按字典读
来源：http://pp.chemitech.net.cn

csv.DictReader(f)
来源：http://wt.muxihuayi.cn

[U26] Py：并发下载
来源：http://st.asd995.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ca.haigaiapp.cn

[U27] Py：异步 HTTP
来源：http://ku.nszjky.cn

aiohttp.ClientSession() 配合 async with
来源：http://qs.wgjwhj.cn

[U28] Py：类型别名
来源：http://ml.newstarts.cn

UserId = int
来源：http://fr.nicolike.cn

[U29] Py：属性校验
来源：http://qo.nicolike.cn

@property 与 @x.setter 配合
来源：http://kn.chemitech.net.cn

[U30] Py：数据类
来源：http://we.nicolike.cn

@dataclass(slots=True)
来源：http://jt.panjiajie.cn

[U31] Py：单测
来源：http://yy.colortex.cn

python -m pytest -q
来源：http://dg.huixinmuqiang.cn

[U32] Py：代码格式化
来源：http://nv.lnxyls.cn

ruff format . && ruff check --fix .
来源：http://sd.colortex.cn

[U33] Py：打包发布
来源：http://fp.huixinmuqiang.cn

python -m build  （依赖 pyproject.toml）
来源：http://lt.hahajie.cn

[U34] Py：判断编码
来源：http://ey.bookmarksfly.cn

chardet.detect(raw)
来源：http://lq.jctech888.com.cn

[U35] Py：发送邮件
来源：http://gc.newstarts.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jz.huixinmuqiang.cn

[U36] Py：定时任务
来源：http://yj.shtwfgs.cn

schedule.every(10).minutes.do(job)
来源：http://ly.haigaiapp.cn

[U37] Py：读写 Excel
来源：http://zj.gzmigu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ab.colortex.cn

[U38] Py：获取脚本所在目录
来源：http://mc.nszjky.cn

Path(__file__).resolve().parent
来源：http://ln.9csxet.cn

[U39] Py：判断是否在交互环境
来源：http://ny.hnjuh.cn

sys.stdout.isatty()
来源：http://uk.huixiangedu.cn

[U40] Py：打印到标准错误
来源：http://bv.gzmigu.cn

print("err", file=sys.stderr)
来源：http://cq.shxzukj.cn

[U41] PHP：初始化 Composer 项目
来源：http://jp.shtwfgs.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://dy.shxzukj.cn

[U42] PHP：PSR-4 自动加载
来源：http://ge.gzmigu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xl.colortex.cn

[U43] PHP：声明命名空间
来源：http://hy.szxytkj.cn

namespace App\Http;
来源：http://uf.jianghongdianzi.cn

[U44] PHP：开启严格类型
来源：http://yk.haigaiapp.cn

declare(strict_types=1);
来源：http://yl.nszjky.cn

[U45] PHP：类型声明与返回类型
来源：http://sh.newstarts.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://yz.chemitech.net.cn

[U46] PHP：可空类型
来源：http://kj.jianghongdianzi.cn

?string $name = null
来源：http://pe.haigaiapp.cn

[U47] PHP：联合类型
来源：http://bv.huixinmuqiang.cn

int|string $id
来源：http://wg.9csxet.cn

[U48] PHP：纯枚举
来源：http://px.hahajie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rb.szsharing.cn

[U49] PHP：只读属性
来源：http://cp.panjiajie.cn

public readonly string $name
来源：http://uy.shxzukj.cn

[U50] PHP：构造器属性提升
来源：http://tv.bookmarksfly.cn

public function __construct(private int $id) {}
来源：http://rc.newstarts.cn

[U51] PHP：数组解构
来源：http://vb.chemitech.net.cn

[$a, $b] = $arr;
来源：http://ko.hnjuh.cn

[U52] PHP：箭头函数
来源：http://sd.muxihuayi.cn

$double = fn($x) => $x * 2;
来源：http://hc.asd995.cn

[U53] PHP：空合并运算符
来源：http://jh.shxzukj.cn

$v = $a ?? $b ?? "default";
来源：http://mm.nicolike.cn

[U54] PHP：空安全调用
来源：http://yf.9csxet.cn

$obj?->method()
来源：http://px.9csxet.cn

[U55] PHP：match 表达式
来源：http://yg.huanxung.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hx.huanxung.cn

[U56] PHP：命名参数
来源：http://dm.gzmigu.cn

f(a: 1, b: 2)
来源：http://pi.lnxyls.cn

[U57] PHP：字符串插值
来源：http://zy.szxytkj.cn

"值: {$a}"
来源：http://zj.bookmarksfly.cn

[U58] PHP：数组三件套
来源：http://ry.panjiajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gw.yuexingan06.cn

[U59] PHP：自定义排序
来源：http://pp.chemitech.net.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qa.newstarts.cn

[U60] PHP：JSON 编解码
来源：http://yg.shxzukj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hw.nszjky.cn

[U61] PHP：正则
来源：http://ic.nszjky.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cs.huanxung.cn

[U62] PHP：日期对象
来源：http://hg.521024.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jw.nszjky.cn

[U63] PHP：文件读写
来源：http://fl.bookmarksfly.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://my.lnxyls.cn

[U64] PHP：目录遍历
来源：http://fg.newstarts.cn

glob("dir/*.php");  scandir("dir");
来源：http://dv.nszjky.cn

[U65] PHP：会话
来源：http://nj.nszjky.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://pr.gzmigu.cn

[U66] PHP：设置 Cookie
来源：http://in.nicolike.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kn.asd995.cn

[U67] PHP：处理文件上传
来源：http://da.wgjwhj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wx.hahajie.cn

[U68] PHP：PDO 连接
来源：http://iq.yuntaijiaju.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://km.lnxyls.cn

[U69] PHP：PDO 预处理
来源：http://iz.nicolike.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ds.chemitech.net.cn

[U70] PHP：PDO 事务
来源：http://mx.jctech888.com.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sa.bjjhwx.cn

[U71] PHP：抛出异常
来源：http://vd.shxzukj.cn

throw new RuntimeException("失败", 500);
来源：http://ou.nicolike.cn

[U72] PHP：写错误日志
来源：http://gf.chemitech.net.cn

error_log("失败: " . $e->getMessage());
来源：http://dh.colortex.cn

[U73] PHP：读取 ini 配置
来源：http://fl.wgjwhj.cn

parse_ini_file("config.ini", true)
来源：http://eu.jctech888.com.cn

[U74] PHP：读取环境变量
来源：http://ge.szsharing.cn

getenv("APP_ENV") ?: "production"
来源：http://kn.bookmarksfly.cn

[U75] PHP：依赖注入
来源：http://bl.szsharing.cn

composer require psr/container
来源：http://uz.panjiajie.cn

[U76] PHP：简单路由
来源：http://wl.huanxung.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sx.lnxyls.cn

[U77] PHP：模板渲染
来源：http://mh.yuntaijiaju.cn

composer require twig/twig
来源：http://ay.shxzskj.cn

[U78] PHP：单元测试
来源：http://ua.nicolike.cn

composer require --dev phpunit/phpunit
来源：http://bn.shxzukj.cn

[U79] PHP：静态分析
来源：http://ug.jctech888.com.cn

composer require --dev phpstan/phpstan
来源：http://cq.hnjuh.cn

[U80] PHP：代码规范修复
来源：http://kk.9csxet.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://gx.asd995.cn

[U81] JS：初始化项目
来源：http://sz.nicolike.cn

npm init -y;  npm i express
来源：http://xm.muxihuayi.cn

[U82] JS：package.json 脚本
来源：http://wj.hnjuh.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zq.521024.cn

[U83] JS：ES Module 导入导出
来源：http://ka.wgjwhj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://hf.szsharing.cn

[U84] JS：CommonJS 写法
来源：http://qp.panjiajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ob.newstarts.cn

[U85] JS：可选链
来源：http://nq.hnjuh.cn

a?.b?.c
来源：http://cs.wgjwhj.cn

[U86] JS：空值合并
来源：http://vy.gzmigu.cn

a ?? b
来源：http://cv.szsharing.cn

[U87] JS：解构默认值
来源：http://oi.muxihuayi.cn

const { a = 1, b = 2 } = obj;
来源：http://sc.gzmigu.cn

[U88] JS：对象展开合并
来源：http://fj.haigaiapp.cn

{ ...a, ...b }
来源：http://py.panjiajie.cn

[U89] JS：数组去重
来源：http://ab.nszjky.cn

[...new Set(arr)]
来源：http://ob.panjiajie.cn

[U90] JS：数字数组排序
来源：http://kx.colortex.cn

[...arr].sort((a, b) => a - b)
来源：http://dv.panjiajie.cn

[U91] JS：对象键值遍历
来源：http://cp.gzmigu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kg.521024.cn

[U92] JS：深拷贝
来源：http://lr.yuexingan06.cn

structuredClone(obj)
来源：http://fh.huanxung.cn

[U93] JS：模板字符串
来源：http://rg.shxzskj.cn

`共 ${n} 条`
来源：http://pa.bookmarksfly.cn

[U94] JS：箭头函数
来源：http://qr.panjiajie.cn

const double = x => x * 2;
来源：http://pn.lnxyls.cn

[U95] JS：Promise 包装
来源：http://xc.huixiangedu.cn

new Promise((resolve, reject) => {})
来源：http://go.jianghongdianzi.cn

[U96] JS：async/await 与异常
来源：http://re.gzmigu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zi.szxytkj.cn

[U97] JS：并发请求
来源：http://ui.wgjwhj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vh.newstarts.cn

[U98] JS：fetch 带 JSON
来源：http://du.szxytkj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vr.yuntaijiaju.cn

[U99] JS：事件监听
来源：http://rc.hnjuh.cn

el.addEventListener("click", e => {})
来源：http://zb.521024.cn

[U100] JS：DOM 查询
来源：http://dx.bjjhwx.cn

document.querySelector(".item")
来源：http://rx.szsharing.cn

[U101] JS：classList 操作
来源：http://qv.huixiangedu.cn

el.classList.toggle("active")
来源：http://al.huixiangedu.cn

[U102] JS：本地存储
来源：http://xj.nszjky.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://lj.chemitech.net.cn

[U103] JS：定时器
来源：http://pk.colortex.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xm.huixiangedu.cn

[U104] JS：防抖
来源：http://wy.nszjky.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xh.huixiangedu.cn

[U105] JS：节流
来源：http://sn.hnjuh.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ko.huixinmuqiang.cn

[U106] JS：日期格式化
来源：http://mc.chemitech.net.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ae.gzmigu.cn

[U107] JS：数字千分位
来源：http://dl.nszjky.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uo.lnxyls.cn

[U108] JS：随机整数
来源：http://bz.gzmigu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gw.colortex.cn

[U109] JS：数组分组
来源：http://ti.bjjhwx.cn

Object.groupBy(arr, x => x.type)
来源：http://ax.huixinmuqiang.cn

[U110] JS：数组分块
来源：http://qc.hahajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ol.hahajie.cn

[U111] JS：对象转 Map
来源：http://of.szxytkj.cn

new Map(Object.entries(obj))
来源：http://ef.lnxyls.cn

[U112] JS：字符串补位
来源：http://nq.colortex.cn

"7".padStart(3, "0")
来源：http://yi.huixinmuqiang.cn

[U113] JS：正则替换全部
来源：http://qw.jctech888.com.cn

s.replaceAll("a", "b")
来源：http://pw.newstarts.cn

[U114] JS：JSON 深比较
来源：http://px.9csxet.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://nj.muxihuayi.cn

[U115] JS：生成 UUID
来源：http://dz.yuntaijiaju.cn

crypto.randomUUID()
来源：http://wm.newstarts.cn

[U116] JS：类型检查（JSDoc）
来源：http://ct.huixiangedu.cn

/** @param {string} name */ function f(name) {}
来源：http://xv.gzmigu.cn

[U117] JS：单元测试
来源：http://tf.muxihuayi.cn

npm i -D vitest;  npx vitest
来源：http://uu.jctech888.com.cn

[U118] JS：开发服务器
来源：http://ve.szsharing.cn

npm i -D vite;  npx vite
来源：http://wf.shtwfgs.cn

[U119] JS：生产构建
来源：http://wj.shxzukj.cn

npx vite build
来源：http://cy.huixinmuqiang.cn

[U120] JS：读取环境变量（Vite）
来源：http://di.szsharing.cn

import.meta.env.VITE_API_URL
来源：http://ig.muxihuayi.cn

================================================================================
来源：http://ak.chemitech.net.cn

统计汇总
来源：http://de.yuntaijiaju.cn

================================================================================
来源：http://yg.muxihuayi.cn

按语言统计（条）：
来源：http://yo.nicolike.cn

Python ......... 252
来源：http://rf.szsharing.cn

PHP ............ 252
来源：http://nx.shtwfgs.cn

JavaScript ..... 252
来源：http://bw.jctech888.com.cn

TypeScript ..... 212
来源：http://lm.hahajie.cn

Java ........... 212
来源：http://ll.haigaiapp.cn

Go ............. 212
来源：http://ec.nszjky.cn

Ruby ........... 212
来源：http://zn.wgjwhj.cn

C# ............. 212
来源：http://kn.bjjhwx.cn

C .............. 30
来源：http://nt.bjjhwx.cn

C++ ............ 30
来源：http://oo.wgjwhj.cn

SQL ............ 90
来源：http://ij.newstarts.cn

Bash ........... 80
来源：http://vo.chemitech.net.cn

Kotlin ......... 15
来源：http://by.nicolike.cn

Swift .......... 15
来源：http://uh.nszjky.cn

Lua ............ 10
来源：http://yv.newstarts.cn

Perl ........... 10
来源：http://qh.szxytkj.cn

Scala .......... 10
来源：http://mx.gzmigu.cn

------------------------------------
来源：http://pm.shxzukj.cn

合计 ........... 2106 条
来源：http://av.nicolike.cn

按章节统计：
来源：http://zw.521024.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ar.huixiangedu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://eq.wgjwhj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://yv.bjjhwx.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://or.wgjwhj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://id.jianghongdianzi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ml.shtwfgs.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ba.huixinmuqiang.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vj.nicolike.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ud.panjiajie.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hx.nicolike.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://su.huixinmuqiang.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://so.muxihuayi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://yu.yuexingan06.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://re.chemitech.net.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dx.shxzskj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://oc.shxzskj.cn


<!-- 参考信息 -->