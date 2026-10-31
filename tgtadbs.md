代发 wailian999

case class User(name: String, age: Int)
来源：http://hq.9csxet.cn

[T57] Scala：模式匹配
来源：http://my.jctech888.com.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://xd.chemitech.net.cn

[T58] Scala：函数定义
来源：http://io.asd995.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ft.szxytkj.cn

[T59] Scala：循环
来源：http://gf.panjiajie.cn

for (i <- 1 to 10) println(i)
来源：http://an.bookmarksfly.cn

[T60] Scala：折叠
来源：http://ju.jianghongdianzi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nm.yuntaijiaju.cn

================================================================================
来源：http://sq.asd995.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qf.szsharing.cn

================================================================================
来源：http://vn.hahajie.cn

[U01] Py：创建虚拟环境
来源：http://ba.panjiajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://xk.colortex.cn

[U02] Py：导出 / 安装依赖
来源：http://ky.muxihuayi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ht.yuexingan06.cn

[U03] Py：加载 .env 配置
来源：http://xl.jianghongdianzi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://lh.bjjhwx.cn

[U04] Py：变量调试打印
来源：http://hm.hahajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kz.huanxung.cn

[U05] Py：列表去重且保序
来源：http://el.newstarts.cn

list(dict.fromkeys(arr))
来源：http://ni.9csxet.cn

[U06] Py：合并两个字典
来源：http://je.colortex.cn

{**a, **b}
来源：http://ed.nicolike.cn

[U07] Py：反转字典键值
来源：http://bv.szsharing.cn

{v: k for k, v in d.items()}
来源：http://em.yuntaijiaju.cn

[U08] Py：展平二维列表
来源：http://by.chemitech.net.cn

[y for x in nested for y in x]
来源：http://qi.haigaiapp.cn

[U09] Py：字典取最大值的键
来源：http://je.nicolike.cn

max(d, key=d.get)
来源：http://wh.asd995.cn

[U10] Py：按值排序字典
来源：http://wf.bookmarksfly.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nj.yuexingan06.cn

[U11] Py：生成器表达式
来源：http://zg.yuntaijiaju.cn

(x * 2 for x in arr)
来源：http://tt.wgjwhj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ow.hahajie.cn

Counter(arr).most_common(3)
来源：http://vn.yuexingan06.cn

[U13] Py：固定长度队列
来源：http://dg.colortex.cn

deque(maxlen=10)
来源：http://yl.asd995.cn

[U14] Py：分组收集到列表
来源：http://mq.9csxet.cn

defaultdict(list)
来源：http://ol.huixiangedu.cn

[U15] Py：高精度计时
来源：http://lz.muxihuayi.cn

t = time.perf_counter()
来源：http://nh.asd995.cn

[U16] Py：命令行参数解析
来源：http://ih.nszjky.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xb.bjjhwx.cn

[U17] Py：初始化日志
来源：http://cr.bookmarksfly.cn

logging.basicConfig(level=logging.INFO)
来源：http://fq.yuntaijiaju.cn

[U18] Py：预编译正则
来源：http://cj.asd995.cn

pat = re.compile(r"\d+")
来源：http://jt.bjjhwx.cn

[U19] Py：正则替换带回调
来源：http://ec.bookmarksfly.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ib.shxzukj.cn

[U20] Py：缓存函数结果
来源：http://ia.szsharing.cn

@functools.lru_cache(maxsize=None)
来源：http://sv.szxytkj.cn

[U21] Py：自定义上下文管理器
来源：http://ey.huixinmuqiang.cn

@contextlib.contextmanager
来源：http://bv.hahajie.cn

[U22] Py：矩阵转置
来源：http://eh.yuntaijiaju.cn

list(zip(*m))
来源：http://yd.nszjky.cn

[U23] Py：分块读取大文件
来源：http://yl.colortex.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gv.nszjky.cn

[U24] Py：路径操作
来源：http://ar.521024.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ad.asd995.cn

[U25] Py：CSV 按字典读
来源：http://hk.9csxet.cn

csv.DictReader(f)
来源：http://tt.nicolike.cn

[U26] Py：并发下载
来源：http://pu.hahajie.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kk.shxzskj.cn

[U27] Py：异步 HTTP
来源：http://va.hnjuh.cn

aiohttp.ClientSession() 配合 async with
来源：http://zq.lnxyls.cn

[U28] Py：类型别名
来源：http://bw.wgjwhj.cn

UserId = int
来源：http://ab.bjjhwx.cn

[U29] Py：属性校验
来源：http://dj.wgjwhj.cn

@property 与 @x.setter 配合
来源：http://bw.huixinmuqiang.cn

[U30] Py：数据类
来源：http://pl.nicolike.cn

@dataclass(slots=True)
来源：http://rf.shtwfgs.cn

[U31] Py：单测
来源：http://jg.wgjwhj.cn

python -m pytest -q
来源：http://bm.hnjuh.cn

[U32] Py：代码格式化
来源：http://ue.asd995.cn

ruff format . && ruff check --fix .
来源：http://ez.huixiangedu.cn

[U33] Py：打包发布
来源：http://el.jctech888.com.cn

python -m build  （依赖 pyproject.toml）
来源：http://an.huixinmuqiang.cn

[U34] Py：判断编码
来源：http://ao.haigaiapp.cn

chardet.detect(raw)
来源：http://xi.szsharing.cn

[U35] Py：发送邮件
来源：http://ug.chemitech.net.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wj.huanxung.cn

[U36] Py：定时任务
来源：http://wf.shtwfgs.cn

schedule.every(10).minutes.do(job)
来源：http://nu.gzmigu.cn

[U37] Py：读写 Excel
来源：http://qg.gzmigu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://zm.hahajie.cn

[U38] Py：获取脚本所在目录
来源：http://rv.nszjky.cn

Path(__file__).resolve().parent
来源：http://jx.haigaiapp.cn

[U39] Py：判断是否在交互环境
来源：http://nz.lnxyls.cn

sys.stdout.isatty()
来源：http://cd.szxytkj.cn

[U40] Py：打印到标准错误
来源：http://bc.nicolike.cn

print("err", file=sys.stderr)
来源：http://jn.hahajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://rb.huanxung.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gr.yuexingan06.cn

[U42] PHP：PSR-4 自动加载
来源：http://iz.muxihuayi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://iq.szxytkj.cn

[U43] PHP：声明命名空间
来源：http://pw.gzmigu.cn

namespace App\Http;
来源：http://do.521024.cn

[U44] PHP：开启严格类型
来源：http://rd.yuntaijiaju.cn

declare(strict_types=1);
来源：http://vp.haigaiapp.cn

[U45] PHP：类型声明与返回类型
来源：http://tv.bjjhwx.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://sm.wgjwhj.cn

[U46] PHP：可空类型
来源：http://kn.huixinmuqiang.cn

?string $name = null
来源：http://wk.nszjky.cn

[U47] PHP：联合类型
来源：http://ip.shxzskj.cn

int|string $id
来源：http://ox.9csxet.cn

[U48] PHP：纯枚举
来源：http://as.jianghongdianzi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dn.shxzukj.cn

[U49] PHP：只读属性
来源：http://ig.huixiangedu.cn

public readonly string $name
来源：http://xu.asd995.cn

[U50] PHP：构造器属性提升
来源：http://hf.huanxung.cn

public function __construct(private int $id) {}
来源：http://uv.szxytkj.cn

[U51] PHP：数组解构
来源：http://zh.wgjwhj.cn

[$a, $b] = $arr;
来源：http://ip.shtwfgs.cn

[U52] PHP：箭头函数
来源：http://jp.huixiangedu.cn

$double = fn($x) => $x * 2;
来源：http://cb.haigaiapp.cn

[U53] PHP：空合并运算符
来源：http://rj.szxytkj.cn

$v = $a ?? $b ?? "default";
来源：http://qh.huanxung.cn

[U54] PHP：空安全调用
来源：http://xa.bjjhwx.cn

$obj?->method()
来源：http://pd.huanxung.cn

[U55] PHP：match 表达式
来源：http://fg.nszjky.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rh.gzmigu.cn

[U56] PHP：命名参数
来源：http://oh.gzmigu.cn

f(a: 1, b: 2)
来源：http://kw.jctech888.com.cn

[U57] PHP：字符串插值
来源：http://rv.shtwfgs.cn

"值: {$a}"
来源：http://yt.colortex.cn

[U58] PHP：数组三件套
来源：http://wo.colortex.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jz.muxihuayi.cn

[U59] PHP：自定义排序
来源：http://zh.jctech888.com.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xr.9csxet.cn

[U60] PHP：JSON 编解码
来源：http://yd.521024.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cu.nicolike.cn

[U61] PHP：正则
来源：http://vm.colortex.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kx.panjiajie.cn

[U62] PHP：日期对象
来源：http://ws.haigaiapp.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://am.bjjhwx.cn

[U63] PHP：文件读写
来源：http://fg.hnjuh.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nn.jianghongdianzi.cn

[U64] PHP：目录遍历
来源：http://ff.colortex.cn

glob("dir/*.php");  scandir("dir");
来源：http://dj.bjjhwx.cn

[U65] PHP：会话
来源：http://ye.nicolike.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://aw.yuexingan06.cn

[U66] PHP：设置 Cookie
来源：http://tz.yuntaijiaju.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fq.szsharing.cn

[U67] PHP：处理文件上传
来源：http://cr.521024.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://es.chemitech.net.cn

[U68] PHP：PDO 连接
来源：http://hb.nszjky.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tp.jctech888.com.cn

[U69] PHP：PDO 预处理
来源：http://hv.szsharing.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tr.jctech888.com.cn

[U70] PHP：PDO 事务
来源：http://ym.shtwfgs.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://as.muxihuayi.cn

[U71] PHP：抛出异常
来源：http://mj.colortex.cn

throw new RuntimeException("失败", 500);
来源：http://gp.shxzukj.cn

[U72] PHP：写错误日志
来源：http://tc.haigaiapp.cn

error_log("失败: " . $e->getMessage());
来源：http://bo.yuntaijiaju.cn

[U73] PHP：读取 ini 配置
来源：http://pn.hahajie.cn

parse_ini_file("config.ini", true)
来源：http://gq.lnxyls.cn

[U74] PHP：读取环境变量
来源：http://or.9csxet.cn

getenv("APP_ENV") ?: "production"
来源：http://jm.yuntaijiaju.cn

[U75] PHP：依赖注入
来源：http://rj.huixiangedu.cn

composer require psr/container
来源：http://hk.huanxung.cn

[U76] PHP：简单路由
来源：http://wz.panjiajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nh.szsharing.cn

[U77] PHP：模板渲染
来源：http://bn.szxytkj.cn

composer require twig/twig
来源：http://xx.hnjuh.cn

[U78] PHP：单元测试
来源：http://is.nszjky.cn

composer require --dev phpunit/phpunit
来源：http://ys.szsharing.cn

[U79] PHP：静态分析
来源：http://ju.lnxyls.cn

composer require --dev phpstan/phpstan
来源：http://qk.yuntaijiaju.cn

[U80] PHP：代码规范修复
来源：http://du.wgjwhj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://zn.jctech888.com.cn

[U81] JS：初始化项目
来源：http://ct.newstarts.cn

npm init -y;  npm i express
来源：http://oy.colortex.cn

[U82] JS：package.json 脚本
来源：http://yb.wgjwhj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lu.521024.cn

[U83] JS：ES Module 导入导出
来源：http://ft.jctech888.com.cn

export const a = 1;  import { a } from "./m.js";
来源：http://wc.colortex.cn

[U84] JS：CommonJS 写法
来源：http://jg.shxzskj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ik.yuntaijiaju.cn

[U85] JS：可选链
来源：http://ow.9csxet.cn

a?.b?.c
来源：http://na.shxzskj.cn

[U86] JS：空值合并
来源：http://wi.shxzskj.cn

a ?? b
来源：http://oe.nszjky.cn

[U87] JS：解构默认值
来源：http://pv.colortex.cn

const { a = 1, b = 2 } = obj;
来源：http://mh.bookmarksfly.cn

[U88] JS：对象展开合并
来源：http://kg.newstarts.cn

{ ...a, ...b }
来源：http://no.nicolike.cn

[U89] JS：数组去重
来源：http://ww.9csxet.cn

[...new Set(arr)]
来源：http://wr.jianghongdianzi.cn

[U90] JS：数字数组排序
来源：http://xy.nszjky.cn

[...arr].sort((a, b) => a - b)
来源：http://kb.bjjhwx.cn

[U91] JS：对象键值遍历
来源：http://dr.szsharing.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mc.yuexingan06.cn

[U92] JS：深拷贝
来源：http://rs.asd995.cn

structuredClone(obj)
来源：http://ur.jianghongdianzi.cn

[U93] JS：模板字符串
来源：http://qd.lnxyls.cn

`共 ${n} 条`
来源：http://xx.shtwfgs.cn

[U94] JS：箭头函数
来源：http://yv.shxzskj.cn

const double = x => x * 2;
来源：http://ey.newstarts.cn

[U95] JS：Promise 包装
来源：http://ed.hnjuh.cn

new Promise((resolve, reject) => {})
来源：http://dm.panjiajie.cn

[U96] JS：async/await 与异常
来源：http://so.nicolike.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wk.bjjhwx.cn

[U97] JS：并发请求
来源：http://dc.yuexingan06.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://tc.muxihuayi.cn

[U98] JS：fetch 带 JSON
来源：http://ml.szxytkj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://sw.jctech888.com.cn

[U99] JS：事件监听
来源：http://pn.wgjwhj.cn

el.addEventListener("click", e => {})
来源：http://st.haigaiapp.cn

[U100] JS：DOM 查询
来源：http://sn.jctech888.com.cn

document.querySelector(".item")
来源：http://fc.bookmarksfly.cn

[U101] JS：classList 操作
来源：http://gq.panjiajie.cn

el.classList.toggle("active")
来源：http://ew.bookmarksfly.cn

[U102] JS：本地存储
来源：http://tj.colortex.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://yf.jianghongdianzi.cn

[U103] JS：定时器
来源：http://tk.9csxet.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ek.muxihuayi.cn

[U104] JS：防抖
来源：http://hr.bjjhwx.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uu.newstarts.cn

[U105] JS：节流
来源：http://mo.szsharing.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ks.yuntaijiaju.cn

[U106] JS：日期格式化
来源：http://pb.asd995.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://em.muxihuayi.cn

[U107] JS：数字千分位
来源：http://ac.bookmarksfly.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wt.9csxet.cn

[U108] JS：随机整数
来源：http://wa.jianghongdianzi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rc.haigaiapp.cn

[U109] JS：数组分组
来源：http://dw.bookmarksfly.cn

Object.groupBy(arr, x => x.type)
来源：http://ma.wgjwhj.cn

[U110] JS：数组分块
来源：http://ry.newstarts.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://su.nszjky.cn

[U111] JS：对象转 Map
来源：http://nx.yuexingan06.cn

new Map(Object.entries(obj))
来源：http://uz.hahajie.cn

[U112] JS：字符串补位
来源：http://oh.szsharing.cn

"7".padStart(3, "0")
来源：http://ij.lnxyls.cn

[U113] JS：正则替换全部
来源：http://pp.bjjhwx.cn

s.replaceAll("a", "b")
来源：http://bz.shxzukj.cn

[U114] JS：JSON 深比较
来源：http://aw.chemitech.net.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ur.shtwfgs.cn

[U115] JS：生成 UUID
来源：http://ve.nszjky.cn

crypto.randomUUID()
来源：http://kf.jctech888.com.cn

[U116] JS：类型检查（JSDoc）
来源：http://uy.huixiangedu.cn

/** @param {string} name */ function f(name) {}
来源：http://nb.shxzukj.cn

[U117] JS：单元测试
来源：http://gr.shxzukj.cn

npm i -D vitest;  npx vitest
来源：http://sr.nicolike.cn

[U118] JS：开发服务器
来源：http://qp.szxytkj.cn

npm i -D vite;  npx vite
来源：http://fa.wgjwhj.cn

[U119] JS：生产构建
来源：http://xq.shxzukj.cn

npx vite build
来源：http://mg.shtwfgs.cn

[U120] JS：读取环境变量（Vite）
来源：http://qv.newstarts.cn

import.meta.env.VITE_API_URL
来源：http://cb.haigaiapp.cn

================================================================================
来源：http://td.521024.cn

统计汇总
来源：http://cl.nszjky.cn

================================================================================
来源：http://in.nicolike.cn

按语言统计（条）：
来源：http://to.haigaiapp.cn

Python ......... 252
来源：http://im.shxzskj.cn

PHP ............ 252
来源：http://nq.gzmigu.cn

JavaScript ..... 252
来源：http://al.nicolike.cn

TypeScript ..... 212
来源：http://jj.huixinmuqiang.cn

Java ........... 212
来源：http://mt.wgjwhj.cn

Go ............. 212
来源：http://ba.nszjky.cn

Ruby ........... 212
来源：http://eo.jianghongdianzi.cn

C# ............. 212
来源：http://kz.yuntaijiaju.cn

C .............. 30
来源：http://yl.yuexingan06.cn

C++ ............ 30
来源：http://cs.huixinmuqiang.cn

SQL ............ 90
来源：http://ex.asd995.cn

Bash ........... 80
来源：http://fx.bookmarksfly.cn

Kotlin ......... 15
来源：http://oy.521024.cn

Swift .......... 15
来源：http://sb.shxzskj.cn

Lua ............ 10
来源：http://ie.nicolike.cn

Perl ........... 10
来源：http://ep.521024.cn

Scala .......... 10
来源：http://mr.shxzukj.cn

------------------------------------
来源：http://hb.muxihuayi.cn

合计 ........... 2106 条
来源：http://is.yuntaijiaju.cn

按章节统计：
来源：http://gg.haigaiapp.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bo.yuntaijiaju.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ll.bookmarksfly.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://va.bookmarksfly.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cn.szxytkj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fa.muxihuayi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wt.huixiangedu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mj.gzmigu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://za.panjiajie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bi.newstarts.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mr.szxytkj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tv.chemitech.net.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jn.gzmigu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jv.yuexingan06.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ze.nszjky.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wl.asd995.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://kx.newstarts.cn

Q SQL 专题                              90
来源：http://rk.jctech888.com.cn

R Bash 专题                             80
来源：http://ms.panjiajie.cn

S C / C++ 专题                          60
来源：http://ri.shxzskj.cn

T 其他语言补充                          60
来源：http://wq.gzmigu.cn

U 高频实用片段                         120
来源：http://oh.nicolike.cn

------------------------------------
来源：http://zb.yuexingan06.cn

合计                                  2106 条
来源：http://pa.newstarts.cn

--------------------------------------------------------------------------------
来源：http://ea.asd995.cn


<!-- 参考信息 -->