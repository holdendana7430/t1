代发 wailian999

val a = 1;  var b = 2
来源：http://sc.521024.cn

[T53] Scala：字符串插值
来源：http://vz.nicolike.cn

s"值: $b"
来源：http://uv.jctech888.com.cn

[T54] Scala：集合映射
来源：http://lz.shtwfgs.cn

List(1, 2, 3).map(_ * 2)
来源：http://up.shxzskj.cn

[T55] Scala：集合过滤
来源：http://ot.muxihuayi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xk.yuexingan06.cn

[T56] Scala：样例类
来源：http://ie.yuexingan06.cn

case class User(name: String, age: Int)
来源：http://fs.newstarts.cn

[T57] Scala：模式匹配
来源：http://ir.huixinmuqiang.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://mj.huanxung.cn

[T58] Scala：函数定义
来源：http://ex.lnxyls.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ur.huixiangedu.cn

[T59] Scala：循环
来源：http://di.nszjky.cn

for (i <- 1 to 10) println(i)
来源：http://nf.szsharing.cn

[T60] Scala：折叠
来源：http://df.yuntaijiaju.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pl.9csxet.cn

================================================================================
来源：http://gw.szsharing.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mm.wgjwhj.cn

================================================================================
来源：http://cz.huanxung.cn

[U01] Py：创建虚拟环境
来源：http://oe.jianghongdianzi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://up.shxzskj.cn

[U02] Py：导出 / 安装依赖
来源：http://fb.shxzukj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://po.huixiangedu.cn

[U03] Py：加载 .env 配置
来源：http://vd.lnxyls.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://iq.nicolike.cn

[U04] Py：变量调试打印
来源：http://yw.chemitech.net.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fs.shxzskj.cn

[U05] Py：列表去重且保序
来源：http://kt.szxytkj.cn

list(dict.fromkeys(arr))
来源：http://il.nszjky.cn

[U06] Py：合并两个字典
来源：http://fk.colortex.cn

{**a, **b}
来源：http://jb.huixinmuqiang.cn

[U07] Py：反转字典键值
来源：http://ok.lnxyls.cn

{v: k for k, v in d.items()}
来源：http://pz.chemitech.net.cn

[U08] Py：展平二维列表
来源：http://nr.bjjhwx.cn

[y for x in nested for y in x]
来源：http://ci.nicolike.cn

[U09] Py：字典取最大值的键
来源：http://rf.nszjky.cn

max(d, key=d.get)
来源：http://zw.gzmigu.cn

[U10] Py：按值排序字典
来源：http://qj.shxzukj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jf.bjjhwx.cn

[U11] Py：生成器表达式
来源：http://rh.bjjhwx.cn

(x * 2 for x in arr)
来源：http://uy.nicolike.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lf.hnjuh.cn

Counter(arr).most_common(3)
来源：http://fz.haigaiapp.cn

[U13] Py：固定长度队列
来源：http://uh.shxzskj.cn

deque(maxlen=10)
来源：http://uf.haigaiapp.cn

[U14] Py：分组收集到列表
来源：http://lc.wgjwhj.cn

defaultdict(list)
来源：http://dt.yuntaijiaju.cn

[U15] Py：高精度计时
来源：http://cm.9csxet.cn

t = time.perf_counter()
来源：http://gh.wgjwhj.cn

[U16] Py：命令行参数解析
来源：http://le.bjjhwx.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fj.colortex.cn

[U17] Py：初始化日志
来源：http://fj.huixiangedu.cn

logging.basicConfig(level=logging.INFO)
来源：http://dj.huixinmuqiang.cn

[U18] Py：预编译正则
来源：http://gu.haigaiapp.cn

pat = re.compile(r"\d+")
来源：http://ct.haigaiapp.cn

[U19] Py：正则替换带回调
来源：http://ho.huixinmuqiang.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ti.bookmarksfly.cn

[U20] Py：缓存函数结果
来源：http://hw.yuntaijiaju.cn

@functools.lru_cache(maxsize=None)
来源：http://km.szsharing.cn

[U21] Py：自定义上下文管理器
来源：http://uz.nicolike.cn

@contextlib.contextmanager
来源：http://dc.shtwfgs.cn

[U22] Py：矩阵转置
来源：http://ec.9csxet.cn

list(zip(*m))
来源：http://dn.lnxyls.cn

[U23] Py：分块读取大文件
来源：http://fz.shxzskj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xz.bjjhwx.cn

[U24] Py：路径操作
来源：http://bv.bjjhwx.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fv.yuexingan06.cn

[U25] Py：CSV 按字典读
来源：http://ik.shxzukj.cn

csv.DictReader(f)
来源：http://bf.szsharing.cn

[U26] Py：并发下载
来源：http://fv.muxihuayi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pd.huixinmuqiang.cn

[U27] Py：异步 HTTP
来源：http://eh.bookmarksfly.cn

aiohttp.ClientSession() 配合 async with
来源：http://gl.yuexingan06.cn

[U28] Py：类型别名
来源：http://ev.shtwfgs.cn

UserId = int
来源：http://mz.9csxet.cn

[U29] Py：属性校验
来源：http://dn.9csxet.cn

@property 与 @x.setter 配合
来源：http://nn.jianghongdianzi.cn

[U30] Py：数据类
来源：http://sm.panjiajie.cn

@dataclass(slots=True)
来源：http://hx.shxzukj.cn

[U31] Py：单测
来源：http://kk.nszjky.cn

python -m pytest -q
来源：http://rt.szxytkj.cn

[U32] Py：代码格式化
来源：http://ty.shtwfgs.cn

ruff format . && ruff check --fix .
来源：http://ac.gzmigu.cn

[U33] Py：打包发布
来源：http://ar.nicolike.cn

python -m build  （依赖 pyproject.toml）
来源：http://us.panjiajie.cn

[U34] Py：判断编码
来源：http://ky.asd995.cn

chardet.detect(raw)
来源：http://wm.jianghongdianzi.cn

[U35] Py：发送邮件
来源：http://ot.shxzskj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lw.asd995.cn

[U36] Py：定时任务
来源：http://ah.huixiangedu.cn

schedule.every(10).minutes.do(job)
来源：http://fj.asd995.cn

[U37] Py：读写 Excel
来源：http://gl.shxzukj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://kw.nicolike.cn

[U38] Py：获取脚本所在目录
来源：http://qt.nszjky.cn

Path(__file__).resolve().parent
来源：http://rc.bjjhwx.cn

[U39] Py：判断是否在交互环境
来源：http://fv.colortex.cn

sys.stdout.isatty()
来源：http://ym.shtwfgs.cn

[U40] Py：打印到标准错误
来源：http://vh.newstarts.cn

print("err", file=sys.stderr)
来源：http://kq.panjiajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://mk.hnjuh.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://yb.newstarts.cn

[U42] PHP：PSR-4 自动加载
来源：http://vy.newstarts.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wc.huixiangedu.cn

[U43] PHP：声明命名空间
来源：http://ke.shtwfgs.cn

namespace App\Http;
来源：http://dy.newstarts.cn

[U44] PHP：开启严格类型
来源：http://sf.panjiajie.cn

declare(strict_types=1);
来源：http://fp.jctech888.com.cn

[U45] PHP：类型声明与返回类型
来源：http://pb.jctech888.com.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ng.chemitech.net.cn

[U46] PHP：可空类型
来源：http://is.szsharing.cn

?string $name = null
来源：http://yu.huixiangedu.cn

[U47] PHP：联合类型
来源：http://et.panjiajie.cn

int|string $id
来源：http://gy.nicolike.cn

[U48] PHP：纯枚举
来源：http://tv.shxzskj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://oc.shxzukj.cn

[U49] PHP：只读属性
来源：http://fm.hahajie.cn

public readonly string $name
来源：http://vl.wgjwhj.cn

[U50] PHP：构造器属性提升
来源：http://sp.gzmigu.cn

public function __construct(private int $id) {}
来源：http://ck.huanxung.cn

[U51] PHP：数组解构
来源：http://sv.nicolike.cn

[$a, $b] = $arr;
来源：http://hd.panjiajie.cn

[U52] PHP：箭头函数
来源：http://yi.hnjuh.cn

$double = fn($x) => $x * 2;
来源：http://ud.szsharing.cn

[U53] PHP：空合并运算符
来源：http://mn.nicolike.cn

$v = $a ?? $b ?? "default";
来源：http://lc.nicolike.cn

[U54] PHP：空安全调用
来源：http://fi.gzmigu.cn

$obj?->method()
来源：http://ax.yuntaijiaju.cn

[U55] PHP：match 表达式
来源：http://ty.lnxyls.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ty.521024.cn

[U56] PHP：命名参数
来源：http://jk.wgjwhj.cn

f(a: 1, b: 2)
来源：http://os.shtwfgs.cn

[U57] PHP：字符串插值
来源：http://xh.jctech888.com.cn

"值: {$a}"
来源：http://pe.panjiajie.cn

[U58] PHP：数组三件套
来源：http://vj.521024.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://uo.lnxyls.cn

[U59] PHP：自定义排序
来源：http://cg.hahajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vk.yuexingan06.cn

[U60] PHP：JSON 编解码
来源：http://tr.521024.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zz.huixinmuqiang.cn

[U61] PHP：正则
来源：http://fj.colortex.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ce.muxihuayi.cn

[U62] PHP：日期对象
来源：http://wu.asd995.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ec.nszjky.cn

[U63] PHP：文件读写
来源：http://hf.yuexingan06.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://we.wgjwhj.cn

[U64] PHP：目录遍历
来源：http://wp.newstarts.cn

glob("dir/*.php");  scandir("dir");
来源：http://ue.nszjky.cn

[U65] PHP：会话
来源：http://qs.nicolike.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ej.nicolike.cn

[U66] PHP：设置 Cookie
来源：http://pw.521024.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://es.nszjky.cn

[U67] PHP：处理文件上传
来源：http://ab.bjjhwx.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fd.haigaiapp.cn

[U68] PHP：PDO 连接
来源：http://yh.chemitech.net.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fu.nicolike.cn

[U69] PHP：PDO 预处理
来源：http://sl.newstarts.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gq.jctech888.com.cn

[U70] PHP：PDO 事务
来源：http://jm.shxzskj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ei.haigaiapp.cn

[U71] PHP：抛出异常
来源：http://xn.jctech888.com.cn

throw new RuntimeException("失败", 500);
来源：http://gy.nszjky.cn

[U72] PHP：写错误日志
来源：http://lz.nszjky.cn

error_log("失败: " . $e->getMessage());
来源：http://cm.nszjky.cn

[U73] PHP：读取 ini 配置
来源：http://jj.bookmarksfly.cn

parse_ini_file("config.ini", true)
来源：http://jg.huixiangedu.cn

[U74] PHP：读取环境变量
来源：http://jn.szxytkj.cn

getenv("APP_ENV") ?: "production"
来源：http://rr.bookmarksfly.cn

[U75] PHP：依赖注入
来源：http://xc.hahajie.cn

composer require psr/container
来源：http://xd.huixiangedu.cn

[U76] PHP：简单路由
来源：http://wg.521024.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jz.szsharing.cn

[U77] PHP：模板渲染
来源：http://ha.bookmarksfly.cn

composer require twig/twig
来源：http://ic.huixinmuqiang.cn

[U78] PHP：单元测试
来源：http://xs.chemitech.net.cn

composer require --dev phpunit/phpunit
来源：http://ej.haigaiapp.cn

[U79] PHP：静态分析
来源：http://wb.jctech888.com.cn

composer require --dev phpstan/phpstan
来源：http://ba.yuexingan06.cn

[U80] PHP：代码规范修复
来源：http://md.shtwfgs.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://aw.bookmarksfly.cn

[U81] JS：初始化项目
来源：http://sz.panjiajie.cn

npm init -y;  npm i express
来源：http://vt.huixiangedu.cn

[U82] JS：package.json 脚本
来源：http://xx.wgjwhj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lh.chemitech.net.cn

[U83] JS：ES Module 导入导出
来源：http://po.9csxet.cn

export const a = 1;  import { a } from "./m.js";
来源：http://bg.521024.cn

[U84] JS：CommonJS 写法
来源：http://bz.nszjky.cn

module.exports = { a };  const { a } = require("./m");
来源：http://pc.wgjwhj.cn

[U85] JS：可选链
来源：http://jo.nszjky.cn

a?.b?.c
来源：http://vt.yuexingan06.cn

[U86] JS：空值合并
来源：http://zk.huixiangedu.cn

a ?? b
来源：http://xr.haigaiapp.cn

[U87] JS：解构默认值
来源：http://fo.521024.cn

const { a = 1, b = 2 } = obj;
来源：http://yd.panjiajie.cn

[U88] JS：对象展开合并
来源：http://nm.haigaiapp.cn

{ ...a, ...b }
来源：http://ok.nicolike.cn

[U89] JS：数组去重
来源：http://sr.asd995.cn

[...new Set(arr)]
来源：http://ry.panjiajie.cn

[U90] JS：数字数组排序
来源：http://zm.bjjhwx.cn

[...arr].sort((a, b) => a - b)
来源：http://bl.muxihuayi.cn

[U91] JS：对象键值遍历
来源：http://db.chemitech.net.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ll.chemitech.net.cn

[U92] JS：深拷贝
来源：http://wk.521024.cn

structuredClone(obj)
来源：http://ro.gzmigu.cn

[U93] JS：模板字符串
来源：http://io.huixinmuqiang.cn

`共 ${n} 条`
来源：http://sv.shxzukj.cn

[U94] JS：箭头函数
来源：http://ku.lnxyls.cn

const double = x => x * 2;
来源：http://kh.shtwfgs.cn

[U95] JS：Promise 包装
来源：http://lq.9csxet.cn

new Promise((resolve, reject) => {})
来源：http://sr.panjiajie.cn

[U96] JS：async/await 与异常
来源：http://xb.hahajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bl.nicolike.cn

[U97] JS：并发请求
来源：http://gm.jctech888.com.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://pn.shxzukj.cn

[U98] JS：fetch 带 JSON
来源：http://pn.szsharing.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mk.szxytkj.cn

[U99] JS：事件监听
来源：http://yi.gzmigu.cn

el.addEventListener("click", e => {})
来源：http://nq.nicolike.cn

[U100] JS：DOM 查询
来源：http://tq.nszjky.cn

document.querySelector(".item")
来源：http://vn.521024.cn

[U101] JS：classList 操作
来源：http://jf.gzmigu.cn

el.classList.toggle("active")
来源：http://io.szsharing.cn

[U102] JS：本地存储
来源：http://at.huixinmuqiang.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://bu.lnxyls.cn

[U103] JS：定时器
来源：http://gx.lnxyls.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ht.521024.cn

[U104] JS：防抖
来源：http://st.panjiajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qb.yuntaijiaju.cn

[U105] JS：节流
来源：http://za.shxzskj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fr.hahajie.cn

[U106] JS：日期格式化
来源：http://xl.szxytkj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ra.jctech888.com.cn

[U107] JS：数字千分位
来源：http://av.9csxet.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bq.gzmigu.cn

[U108] JS：随机整数
来源：http://ez.521024.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jq.szxytkj.cn

[U109] JS：数组分组
来源：http://ze.shtwfgs.cn

Object.groupBy(arr, x => x.type)
来源：http://wv.hahajie.cn

[U110] JS：数组分块
来源：http://gz.jctech888.com.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://un.shxzskj.cn

[U111] JS：对象转 Map
来源：http://wb.521024.cn

new Map(Object.entries(obj))
来源：http://lx.szsharing.cn

[U112] JS：字符串补位
来源：http://ba.hahajie.cn

"7".padStart(3, "0")
来源：http://wg.yuexingan06.cn

[U113] JS：正则替换全部
来源：http://ip.9csxet.cn

s.replaceAll("a", "b")
来源：http://nw.szsharing.cn

[U114] JS：JSON 深比较
来源：http://um.szsharing.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://pr.szsharing.cn

[U115] JS：生成 UUID
来源：http://xz.chemitech.net.cn

crypto.randomUUID()
来源：http://mw.szxytkj.cn

[U116] JS：类型检查（JSDoc）
来源：http://zh.yuntaijiaju.cn

/** @param {string} name */ function f(name) {}
来源：http://kx.nszjky.cn

[U117] JS：单元测试
来源：http://fh.newstarts.cn

npm i -D vitest;  npx vitest
来源：http://pj.colortex.cn

[U118] JS：开发服务器
来源：http://zc.chemitech.net.cn

npm i -D vite;  npx vite
来源：http://po.haigaiapp.cn

[U119] JS：生产构建
来源：http://uo.gzmigu.cn

npx vite build
来源：http://xo.bjjhwx.cn

[U120] JS：读取环境变量（Vite）
来源：http://zj.asd995.cn

import.meta.env.VITE_API_URL
来源：http://wx.muxihuayi.cn

================================================================================
来源：http://cv.bjjhwx.cn

统计汇总
来源：http://lu.haigaiapp.cn

================================================================================
来源：http://kr.shxzskj.cn

按语言统计（条）：
来源：http://cl.gzmigu.cn

Python ......... 252
来源：http://rk.wgjwhj.cn

PHP ............ 252
来源：http://xm.shxzukj.cn

JavaScript ..... 252
来源：http://di.yuexingan06.cn

TypeScript ..... 212
来源：http://lg.521024.cn

Java ........... 212
来源：http://wp.wgjwhj.cn

Go ............. 212
来源：http://vq.nicolike.cn

Ruby ........... 212
来源：http://tp.muxihuayi.cn

C# ............. 212
来源：http://wo.newstarts.cn

C .............. 30
来源：http://ni.nszjky.cn

C++ ............ 30
来源：http://mf.9csxet.cn

SQL ............ 90
来源：http://ju.panjiajie.cn

Bash ........... 80
来源：http://ik.bjjhwx.cn

Kotlin ......... 15
来源：http://sm.yuntaijiaju.cn

Swift .......... 15
来源：http://wz.haigaiapp.cn

Lua ............ 10
来源：http://ry.shxzskj.cn

Perl ........... 10
来源：http://jh.bjjhwx.cn

Scala .......... 10
来源：http://nv.jctech888.com.cn

------------------------------------
来源：http://hu.gzmigu.cn

合计 ........... 2106 条
来源：http://dg.lnxyls.cn

按章节统计：
来源：http://aq.yuexingan06.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nc.nicolike.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wo.szxytkj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://no.colortex.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qj.newstarts.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://op.bookmarksfly.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ld.huanxung.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rr.hnjuh.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kq.chemitech.net.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bp.jianghongdianzi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ag.huanxung.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dt.newstarts.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cn.hahajie.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ls.bjjhwx.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fv.jianghongdianzi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zc.jianghongdianzi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://px.chemitech.net.cn


<!-- 参考信息 -->