代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xz.wgjwhj.cn

================================================================================
来源：http://rx.shxzskj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://iq.huixiangedu.cn

================================================================================
来源：http://yw.asd995.cn

[U01] Py：创建虚拟环境
来源：http://wu.bjjhwx.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bo.yuntaijiaju.cn

[U02] Py：导出 / 安装依赖
来源：http://kb.yuexingan06.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://to.hnjuh.cn

[U03] Py：加载 .env 配置
来源：http://ht.haigaiapp.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://tt.szxytkj.cn

[U04] Py：变量调试打印
来源：http://om.shxzskj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://na.shxzukj.cn

[U05] Py：列表去重且保序
来源：http://in.wgjwhj.cn

list(dict.fromkeys(arr))
来源：http://th.newstarts.cn

[U06] Py：合并两个字典
来源：http://sk.newstarts.cn

{**a, **b}
来源：http://rq.huixiangedu.cn

[U07] Py：反转字典键值
来源：http://mq.bookmarksfly.cn

{v: k for k, v in d.items()}
来源：http://mn.huanxung.cn

[U08] Py：展平二维列表
来源：http://qo.9csxet.cn

[y for x in nested for y in x]
来源：http://hl.yuexingan06.cn

[U09] Py：字典取最大值的键
来源：http://vj.shtwfgs.cn

max(d, key=d.get)
来源：http://mq.nszjky.cn

[U10] Py：按值排序字典
来源：http://qu.521024.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lr.colortex.cn

[U11] Py：生成器表达式
来源：http://hw.521024.cn

(x * 2 for x in arr)
来源：http://qj.bookmarksfly.cn

[U12] Py：取出现最多的 3 个元素
来源：http://oi.newstarts.cn

Counter(arr).most_common(3)
来源：http://fp.wgjwhj.cn

[U13] Py：固定长度队列
来源：http://li.521024.cn

deque(maxlen=10)
来源：http://gc.huanxung.cn

[U14] Py：分组收集到列表
来源：http://gv.colortex.cn

defaultdict(list)
来源：http://cr.521024.cn

[U15] Py：高精度计时
来源：http://mp.panjiajie.cn

t = time.perf_counter()
来源：http://dv.huixinmuqiang.cn

[U16] Py：命令行参数解析
来源：http://bo.szxytkj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lq.wgjwhj.cn

[U17] Py：初始化日志
来源：http://qa.hnjuh.cn

logging.basicConfig(level=logging.INFO)
来源：http://gp.9csxet.cn

[U18] Py：预编译正则
来源：http://yb.szxytkj.cn

pat = re.compile(r"\d+")
来源：http://we.9csxet.cn

[U19] Py：正则替换带回调
来源：http://sw.shxzukj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ww.wgjwhj.cn

[U20] Py：缓存函数结果
来源：http://zp.shtwfgs.cn

@functools.lru_cache(maxsize=None)
来源：http://ne.haigaiapp.cn

[U21] Py：自定义上下文管理器
来源：http://sv.shxzskj.cn

@contextlib.contextmanager
来源：http://eb.chemitech.net.cn

[U22] Py：矩阵转置
来源：http://lp.bjjhwx.cn

list(zip(*m))
来源：http://eu.yuexingan06.cn

[U23] Py：分块读取大文件
来源：http://yx.newstarts.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pa.shtwfgs.cn

[U24] Py：路径操作
来源：http://lq.yuntaijiaju.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fj.panjiajie.cn

[U25] Py：CSV 按字典读
来源：http://ui.panjiajie.cn

csv.DictReader(f)
来源：http://jk.bjjhwx.cn

[U26] Py：并发下载
来源：http://yn.huixinmuqiang.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bk.lnxyls.cn

[U27] Py：异步 HTTP
来源：http://cv.jctech888.com.cn

aiohttp.ClientSession() 配合 async with
来源：http://ka.asd995.cn

[U28] Py：类型别名
来源：http://fj.panjiajie.cn

UserId = int
来源：http://gz.huixiangedu.cn

[U29] Py：属性校验
来源：http://ov.nicolike.cn

@property 与 @x.setter 配合
来源：http://gf.wgjwhj.cn

[U30] Py：数据类
来源：http://ye.huixinmuqiang.cn

@dataclass(slots=True)
来源：http://gp.shxzskj.cn

[U31] Py：单测
来源：http://wv.lnxyls.cn

python -m pytest -q
来源：http://kz.bjjhwx.cn

[U32] Py：代码格式化
来源：http://sl.colortex.cn

ruff format . && ruff check --fix .
来源：http://qk.gzmigu.cn

[U33] Py：打包发布
来源：http://kh.shtwfgs.cn

python -m build  （依赖 pyproject.toml）
来源：http://rw.wgjwhj.cn

[U34] Py：判断编码
来源：http://xb.wgjwhj.cn

chardet.detect(raw)
来源：http://kk.hahajie.cn

[U35] Py：发送邮件
来源：http://rm.huanxung.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rk.yuntaijiaju.cn

[U36] Py：定时任务
来源：http://dn.newstarts.cn

schedule.every(10).minutes.do(job)
来源：http://gq.hnjuh.cn

[U37] Py：读写 Excel
来源：http://ju.nicolike.cn

pandas.read_excel / DataFrame.to_excel
来源：http://gm.yuexingan06.cn

[U38] Py：获取脚本所在目录
来源：http://ys.panjiajie.cn

Path(__file__).resolve().parent
来源：http://ky.jianghongdianzi.cn

[U39] Py：判断是否在交互环境
来源：http://nv.panjiajie.cn

sys.stdout.isatty()
来源：http://pl.szsharing.cn

[U40] Py：打印到标准错误
来源：http://od.gzmigu.cn

print("err", file=sys.stderr)
来源：http://jz.lnxyls.cn

[U41] PHP：初始化 Composer 项目
来源：http://ru.colortex.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://sw.colortex.cn

[U42] PHP：PSR-4 自动加载
来源：http://zg.bookmarksfly.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ru.asd995.cn

[U43] PHP：声明命名空间
来源：http://zz.521024.cn

namespace App\Http;
来源：http://ot.jianghongdianzi.cn

[U44] PHP：开启严格类型
来源：http://uy.gzmigu.cn

declare(strict_types=1);
来源：http://xo.yuexingan06.cn

[U45] PHP：类型声明与返回类型
来源：http://ip.szxytkj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://xh.asd995.cn

[U46] PHP：可空类型
来源：http://kl.gzmigu.cn

?string $name = null
来源：http://tp.hahajie.cn

[U47] PHP：联合类型
来源：http://nf.panjiajie.cn

int|string $id
来源：http://vz.yuntaijiaju.cn

[U48] PHP：纯枚举
来源：http://tb.haigaiapp.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wu.shxzukj.cn

[U49] PHP：只读属性
来源：http://gv.yuexingan06.cn

public readonly string $name
来源：http://zo.lnxyls.cn

[U50] PHP：构造器属性提升
来源：http://el.nszjky.cn

public function __construct(private int $id) {}
来源：http://wa.yuexingan06.cn

[U51] PHP：数组解构
来源：http://zf.yuntaijiaju.cn

[$a, $b] = $arr;
来源：http://yw.shxzukj.cn

[U52] PHP：箭头函数
来源：http://em.asd995.cn

$double = fn($x) => $x * 2;
来源：http://su.jianghongdianzi.cn

[U53] PHP：空合并运算符
来源：http://va.panjiajie.cn

$v = $a ?? $b ?? "default";
来源：http://wm.huanxung.cn

[U54] PHP：空安全调用
来源：http://km.szxytkj.cn

$obj?->method()
来源：http://qo.jctech888.com.cn

[U55] PHP：match 表达式
来源：http://sp.hnjuh.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xz.colortex.cn

[U56] PHP：命名参数
来源：http://tj.bookmarksfly.cn

f(a: 1, b: 2)
来源：http://el.nicolike.cn

[U57] PHP：字符串插值
来源：http://cv.shxzukj.cn

"值: {$a}"
来源：http://ul.shxzukj.cn

[U58] PHP：数组三件套
来源：http://ox.yuntaijiaju.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ag.muxihuayi.cn

[U59] PHP：自定义排序
来源：http://ve.newstarts.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jx.huanxung.cn

[U60] PHP：JSON 编解码
来源：http://px.panjiajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ly.jctech888.com.cn

[U61] PHP：正则
来源：http://mp.521024.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dm.gzmigu.cn

[U62] PHP：日期对象
来源：http://gv.colortex.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ce.shxzukj.cn

[U63] PHP：文件读写
来源：http://qs.hnjuh.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xq.muxihuayi.cn

[U64] PHP：目录遍历
来源：http://sf.szxytkj.cn

glob("dir/*.php");  scandir("dir");
来源：http://si.muxihuayi.cn

[U65] PHP：会话
来源：http://qe.nszjky.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rt.asd995.cn

[U66] PHP：设置 Cookie
来源：http://vo.huixiangedu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ol.huanxung.cn

[U67] PHP：处理文件上传
来源：http://cu.wgjwhj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://td.newstarts.cn

[U68] PHP：PDO 连接
来源：http://hn.521024.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wa.huixinmuqiang.cn

[U69] PHP：PDO 预处理
来源：http://qe.521024.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dz.huixiangedu.cn

[U70] PHP：PDO 事务
来源：http://ck.gzmigu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cg.yuexingan06.cn

[U71] PHP：抛出异常
来源：http://tw.asd995.cn

throw new RuntimeException("失败", 500);
来源：http://ag.shtwfgs.cn

[U72] PHP：写错误日志
来源：http://wh.bookmarksfly.cn

error_log("失败: " . $e->getMessage());
来源：http://bt.haigaiapp.cn

[U73] PHP：读取 ini 配置
来源：http://ya.jctech888.com.cn

parse_ini_file("config.ini", true)
来源：http://wl.bookmarksfly.cn

[U74] PHP：读取环境变量
来源：http://jc.chemitech.net.cn

getenv("APP_ENV") ?: "production"
来源：http://pi.huixinmuqiang.cn

[U75] PHP：依赖注入
来源：http://mr.colortex.cn

composer require psr/container
来源：http://ok.newstarts.cn

[U76] PHP：简单路由
来源：http://ul.muxihuayi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vo.szxytkj.cn

[U77] PHP：模板渲染
来源：http://vj.wgjwhj.cn

composer require twig/twig
来源：http://bi.jianghongdianzi.cn

[U78] PHP：单元测试
来源：http://gg.shxzskj.cn

composer require --dev phpunit/phpunit
来源：http://tm.gzmigu.cn

[U79] PHP：静态分析
来源：http://kg.9csxet.cn

composer require --dev phpstan/phpstan
来源：http://mv.nicolike.cn

[U80] PHP：代码规范修复
来源：http://br.shtwfgs.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://cm.bookmarksfly.cn

[U81] JS：初始化项目
来源：http://st.haigaiapp.cn

npm init -y;  npm i express
来源：http://mf.lnxyls.cn

[U82] JS：package.json 脚本
来源：http://eq.chemitech.net.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gw.huixiangedu.cn

[U83] JS：ES Module 导入导出
来源：http://me.nszjky.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zk.szsharing.cn

[U84] JS：CommonJS 写法
来源：http://qu.newstarts.cn

module.exports = { a };  const { a } = require("./m");
来源：http://nr.newstarts.cn

[U85] JS：可选链
来源：http://ij.hahajie.cn

a?.b?.c
来源：http://hy.gzmigu.cn

[U86] JS：空值合并
来源：http://qv.huixinmuqiang.cn

a ?? b
来源：http://vt.bjjhwx.cn

[U87] JS：解构默认值
来源：http://ed.muxihuayi.cn

const { a = 1, b = 2 } = obj;
来源：http://ev.jctech888.com.cn

[U88] JS：对象展开合并
来源：http://ar.szxytkj.cn

{ ...a, ...b }
来源：http://qe.huixiangedu.cn

[U89] JS：数组去重
来源：http://ov.szxytkj.cn

[...new Set(arr)]
来源：http://xc.newstarts.cn

[U90] JS：数字数组排序
来源：http://xm.szxytkj.cn

[...arr].sort((a, b) => a - b)
来源：http://gm.panjiajie.cn

[U91] JS：对象键值遍历
来源：http://sj.9csxet.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lu.huixinmuqiang.cn

[U92] JS：深拷贝
来源：http://ei.szxytkj.cn

structuredClone(obj)
来源：http://ck.huixinmuqiang.cn

[U93] JS：模板字符串
来源：http://ui.panjiajie.cn

`共 ${n} 条`
来源：http://kq.nszjky.cn

[U94] JS：箭头函数
来源：http://zk.wgjwhj.cn

const double = x => x * 2;
来源：http://ti.huanxung.cn

[U95] JS：Promise 包装
来源：http://hh.szsharing.cn

new Promise((resolve, reject) => {})
来源：http://bi.newstarts.cn

[U96] JS：async/await 与异常
来源：http://db.muxihuayi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qy.bjjhwx.cn

[U97] JS：并发请求
来源：http://pm.chemitech.net.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://uz.huixiangedu.cn

[U98] JS：fetch 带 JSON
来源：http://vj.wgjwhj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hr.muxihuayi.cn

[U99] JS：事件监听
来源：http://nd.chemitech.net.cn

el.addEventListener("click", e => {})
来源：http://ko.szsharing.cn

[U100] JS：DOM 查询
来源：http://wt.jianghongdianzi.cn

document.querySelector(".item")
来源：http://aq.nszjky.cn

[U101] JS：classList 操作
来源：http://jr.chemitech.net.cn

el.classList.toggle("active")
来源：http://ct.bjjhwx.cn

[U102] JS：本地存储
来源：http://ku.shtwfgs.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://tp.bjjhwx.cn

[U103] JS：定时器
来源：http://ro.shxzukj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ah.521024.cn

[U104] JS：防抖
来源：http://lh.colortex.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tz.szsharing.cn

[U105] JS：节流
来源：http://ld.panjiajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dg.szsharing.cn

[U106] JS：日期格式化
来源：http://jg.colortex.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nj.colortex.cn

[U107] JS：数字千分位
来源：http://kd.haigaiapp.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fi.huanxung.cn

[U108] JS：随机整数
来源：http://nm.bjjhwx.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ho.yuexingan06.cn

[U109] JS：数组分组
来源：http://jk.wgjwhj.cn

Object.groupBy(arr, x => x.type)
来源：http://cd.panjiajie.cn

[U110] JS：数组分块
来源：http://bh.lnxyls.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://aq.colortex.cn

[U111] JS：对象转 Map
来源：http://ln.huixinmuqiang.cn

new Map(Object.entries(obj))
来源：http://kp.bjjhwx.cn

[U112] JS：字符串补位
来源：http://xy.lnxyls.cn

"7".padStart(3, "0")
来源：http://rw.bjjhwx.cn

[U113] JS：正则替换全部
来源：http://ww.colortex.cn

s.replaceAll("a", "b")
来源：http://st.yuexingan06.cn

[U114] JS：JSON 深比较
来源：http://cy.szxytkj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://gn.shxzukj.cn

[U115] JS：生成 UUID
来源：http://uu.hnjuh.cn

crypto.randomUUID()
来源：http://hf.hnjuh.cn

[U116] JS：类型检查（JSDoc）
来源：http://cu.panjiajie.cn

/** @param {string} name */ function f(name) {}
来源：http://wc.hahajie.cn

[U117] JS：单元测试
来源：http://up.521024.cn

npm i -D vitest;  npx vitest
来源：http://jb.bookmarksfly.cn

[U118] JS：开发服务器
来源：http://nu.jctech888.com.cn

npm i -D vite;  npx vite
来源：http://kt.wgjwhj.cn

[U119] JS：生产构建
来源：http://de.panjiajie.cn

npx vite build
来源：http://xi.9csxet.cn

[U120] JS：读取环境变量（Vite）
来源：http://io.wgjwhj.cn

import.meta.env.VITE_API_URL
来源：http://fe.shxzukj.cn

================================================================================
来源：http://jo.newstarts.cn

统计汇总
来源：http://sz.wgjwhj.cn

================================================================================
来源：http://up.521024.cn

按语言统计（条）：
来源：http://fp.yuexingan06.cn

Python ......... 252
来源：http://av.gzmigu.cn

PHP ............ 252
来源：http://sl.yuntaijiaju.cn

JavaScript ..... 252
来源：http://en.nicolike.cn

TypeScript ..... 212
来源：http://il.yuntaijiaju.cn

Java ........... 212
来源：http://om.9csxet.cn

Go ............. 212
来源：http://eh.hahajie.cn

Ruby ........... 212
来源：http://jt.yuexingan06.cn

C# ............. 212
来源：http://tw.haigaiapp.cn

C .............. 30
来源：http://cz.bjjhwx.cn

C++ ............ 30
来源：http://jn.yuexingan06.cn

SQL ............ 90
来源：http://hr.jianghongdianzi.cn

Bash ........... 80
来源：http://md.hahajie.cn

Kotlin ......... 15
来源：http://dl.chemitech.net.cn

Swift .......... 15
来源：http://sz.panjiajie.cn

Lua ............ 10
来源：http://bq.huixinmuqiang.cn

Perl ........... 10
来源：http://wn.colortex.cn

Scala .......... 10
来源：http://cn.muxihuayi.cn

------------------------------------
来源：http://iu.huanxung.cn

合计 ........... 2106 条
来源：http://om.chemitech.net.cn

按章节统计：
来源：http://tq.szxytkj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ch.shxzskj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fy.nszjky.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://aa.szxytkj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gb.shxzukj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qk.lnxyls.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rj.nicolike.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://im.jctech888.com.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jc.shxzukj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ze.wgjwhj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vl.newstarts.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tq.bjjhwx.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rc.bookmarksfly.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ms.bjjhwx.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jw.521024.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tx.lnxyls.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vh.gzmigu.cn

Q SQL 专题                              90
来源：http://pt.hnjuh.cn

R Bash 专题                             80
来源：http://bn.shxzukj.cn

S C / C++ 专题                          60
来源：http://ks.yuntaijiaju.cn

T 其他语言补充                          60
来源：http://ui.chemitech.net.cn

U 高频实用片段                         120
来源：http://wl.shxzskj.cn

------------------------------------
来源：http://xp.yuexingan06.cn

合计                                  2106 条
来源：http://pa.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://gb.shxzukj.cn

使用提醒
来源：http://sl.szsharing.cn

--------------------------------------------------------------------------------
来源：http://hr.bjjhwx.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gd.521024.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://sm.chemitech.net.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bs.muxihuayi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://wc.hahajie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mm.jctech888.com.cn

—— 文件结束 ——
来源：http://vp.hnjuh.cn


<!-- 参考信息 -->