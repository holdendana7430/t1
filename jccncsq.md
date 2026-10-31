代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://mc.colortex.cn

[T59] Scala：循环
来源：http://xv.yuntaijiaju.cn

for (i <- 1 to 10) println(i)
来源：http://al.asd995.cn

[T60] Scala：折叠
来源：http://gj.bookmarksfly.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://iw.nszjky.cn

================================================================================
来源：http://tn.szxytkj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ez.huanxung.cn

================================================================================
来源：http://xr.bjjhwx.cn

[U01] Py：创建虚拟环境
来源：http://pa.hahajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://sf.wgjwhj.cn

[U02] Py：导出 / 安装依赖
来源：http://cr.hnjuh.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tz.wgjwhj.cn

[U03] Py：加载 .env 配置
来源：http://uw.haigaiapp.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qd.shxzskj.cn

[U04] Py：变量调试打印
来源：http://bt.muxihuayi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bg.jctech888.com.cn

[U05] Py：列表去重且保序
来源：http://ji.szxytkj.cn

list(dict.fromkeys(arr))
来源：http://nx.shxzukj.cn

[U06] Py：合并两个字典
来源：http://fu.shxzskj.cn

{**a, **b}
来源：http://li.colortex.cn

[U07] Py：反转字典键值
来源：http://kd.asd995.cn

{v: k for k, v in d.items()}
来源：http://bi.bookmarksfly.cn

[U08] Py：展平二维列表
来源：http://pu.panjiajie.cn

[y for x in nested for y in x]
来源：http://mv.yuexingan06.cn

[U09] Py：字典取最大值的键
来源：http://ut.jctech888.com.cn

max(d, key=d.get)
来源：http://pk.gzmigu.cn

[U10] Py：按值排序字典
来源：http://xd.9csxet.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ol.shxzskj.cn

[U11] Py：生成器表达式
来源：http://kz.shxzskj.cn

(x * 2 for x in arr)
来源：http://yq.nszjky.cn

[U12] Py：取出现最多的 3 个元素
来源：http://jn.szxytkj.cn

Counter(arr).most_common(3)
来源：http://mo.nicolike.cn

[U13] Py：固定长度队列
来源：http://qv.lnxyls.cn

deque(maxlen=10)
来源：http://fk.jctech888.com.cn

[U14] Py：分组收集到列表
来源：http://rx.bjjhwx.cn

defaultdict(list)
来源：http://xg.hnjuh.cn

[U15] Py：高精度计时
来源：http://rj.yuexingan06.cn

t = time.perf_counter()
来源：http://je.huanxung.cn

[U16] Py：命令行参数解析
来源：http://cw.haigaiapp.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qq.szxytkj.cn

[U17] Py：初始化日志
来源：http://ke.nicolike.cn

logging.basicConfig(level=logging.INFO)
来源：http://og.shxzukj.cn

[U18] Py：预编译正则
来源：http://vt.szxytkj.cn

pat = re.compile(r"\d+")
来源：http://yy.bjjhwx.cn

[U19] Py：正则替换带回调
来源：http://ct.shtwfgs.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lv.521024.cn

[U20] Py：缓存函数结果
来源：http://ax.asd995.cn

@functools.lru_cache(maxsize=None)
来源：http://bl.szxytkj.cn

[U21] Py：自定义上下文管理器
来源：http://ag.huixiangedu.cn

@contextlib.contextmanager
来源：http://tn.gzmigu.cn

[U22] Py：矩阵转置
来源：http://ug.haigaiapp.cn

list(zip(*m))
来源：http://eu.bookmarksfly.cn

[U23] Py：分块读取大文件
来源：http://yz.yuntaijiaju.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vb.colortex.cn

[U24] Py：路径操作
来源：http://ht.huixinmuqiang.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://as.muxihuayi.cn

[U25] Py：CSV 按字典读
来源：http://cc.huanxung.cn

csv.DictReader(f)
来源：http://it.yuntaijiaju.cn

[U26] Py：并发下载
来源：http://ee.huixinmuqiang.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xe.9csxet.cn

[U27] Py：异步 HTTP
来源：http://gj.hnjuh.cn

aiohttp.ClientSession() 配合 async with
来源：http://pv.shxzukj.cn

[U28] Py：类型别名
来源：http://as.colortex.cn

UserId = int
来源：http://uq.nicolike.cn

[U29] Py：属性校验
来源：http://em.muxihuayi.cn

@property 与 @x.setter 配合
来源：http://mg.szsharing.cn

[U30] Py：数据类
来源：http://ip.muxihuayi.cn

@dataclass(slots=True)
来源：http://si.bjjhwx.cn

[U31] Py：单测
来源：http://ry.bookmarksfly.cn

python -m pytest -q
来源：http://om.newstarts.cn

[U32] Py：代码格式化
来源：http://kh.asd995.cn

ruff format . && ruff check --fix .
来源：http://wu.panjiajie.cn

[U33] Py：打包发布
来源：http://wi.huixinmuqiang.cn

python -m build  （依赖 pyproject.toml）
来源：http://ec.huanxung.cn

[U34] Py：判断编码
来源：http://ve.hahajie.cn

chardet.detect(raw)
来源：http://mz.jianghongdianzi.cn

[U35] Py：发送邮件
来源：http://op.jianghongdianzi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xt.jctech888.com.cn

[U36] Py：定时任务
来源：http://up.szsharing.cn

schedule.every(10).minutes.do(job)
来源：http://ub.panjiajie.cn

[U37] Py：读写 Excel
来源：http://pm.lnxyls.cn

pandas.read_excel / DataFrame.to_excel
来源：http://uo.shxzskj.cn

[U38] Py：获取脚本所在目录
来源：http://og.jctech888.com.cn

Path(__file__).resolve().parent
来源：http://lg.nicolike.cn

[U39] Py：判断是否在交互环境
来源：http://pj.chemitech.net.cn

sys.stdout.isatty()
来源：http://cg.asd995.cn

[U40] Py：打印到标准错误
来源：http://jv.szxytkj.cn

print("err", file=sys.stderr)
来源：http://if.muxihuayi.cn

[U41] PHP：初始化 Composer 项目
来源：http://uc.jianghongdianzi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ku.nszjky.cn

[U42] PHP：PSR-4 自动加载
来源：http://as.wgjwhj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lb.nszjky.cn

[U43] PHP：声明命名空间
来源：http://im.gzmigu.cn

namespace App\Http;
来源：http://db.yuntaijiaju.cn

[U44] PHP：开启严格类型
来源：http://qp.panjiajie.cn

declare(strict_types=1);
来源：http://aj.huixinmuqiang.cn

[U45] PHP：类型声明与返回类型
来源：http://dr.shxzukj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://kp.bookmarksfly.cn

[U46] PHP：可空类型
来源：http://ja.newstarts.cn

?string $name = null
来源：http://cj.shtwfgs.cn

[U47] PHP：联合类型
来源：http://ob.szxytkj.cn

int|string $id
来源：http://ta.nicolike.cn

[U48] PHP：纯枚举
来源：http://la.nszjky.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qj.huixiangedu.cn

[U49] PHP：只读属性
来源：http://ym.haigaiapp.cn

public readonly string $name
来源：http://gw.huixiangedu.cn

[U50] PHP：构造器属性提升
来源：http://au.bjjhwx.cn

public function __construct(private int $id) {}
来源：http://ka.nicolike.cn

[U51] PHP：数组解构
来源：http://wo.muxihuayi.cn

[$a, $b] = $arr;
来源：http://yg.yuntaijiaju.cn

[U52] PHP：箭头函数
来源：http://bz.9csxet.cn

$double = fn($x) => $x * 2;
来源：http://at.muxihuayi.cn

[U53] PHP：空合并运算符
来源：http://gp.muxihuayi.cn

$v = $a ?? $b ?? "default";
来源：http://lr.shtwfgs.cn

[U54] PHP：空安全调用
来源：http://wa.panjiajie.cn

$obj?->method()
来源：http://zv.shxzskj.cn

[U55] PHP：match 表达式
来源：http://yq.9csxet.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cz.bjjhwx.cn

[U56] PHP：命名参数
来源：http://fw.huanxung.cn

f(a: 1, b: 2)
来源：http://gu.bjjhwx.cn

[U57] PHP：字符串插值
来源：http://wo.wgjwhj.cn

"值: {$a}"
来源：http://vx.gzmigu.cn

[U58] PHP：数组三件套
来源：http://zd.huixiangedu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jk.shtwfgs.cn

[U59] PHP：自定义排序
来源：http://uw.yuntaijiaju.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cw.jianghongdianzi.cn

[U60] PHP：JSON 编解码
来源：http://ug.panjiajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://sd.hnjuh.cn

[U61] PHP：正则
来源：http://ql.szxytkj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qq.yuntaijiaju.cn

[U62] PHP：日期对象
来源：http://gq.haigaiapp.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://od.yuntaijiaju.cn

[U63] PHP：文件读写
来源：http://yx.huixiangedu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://po.muxihuayi.cn

[U64] PHP：目录遍历
来源：http://zx.nszjky.cn

glob("dir/*.php");  scandir("dir");
来源：http://dr.yuexingan06.cn

[U65] PHP：会话
来源：http://bo.jianghongdianzi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://sz.huixiangedu.cn

[U66] PHP：设置 Cookie
来源：http://ry.huixiangedu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rb.jctech888.com.cn

[U67] PHP：处理文件上传
来源：http://nz.newstarts.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://td.jianghongdianzi.cn

[U68] PHP：PDO 连接
来源：http://pf.haigaiapp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://om.yuexingan06.cn

[U69] PHP：PDO 预处理
来源：http://av.lnxyls.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xv.lnxyls.cn

[U70] PHP：PDO 事务
来源：http://cm.shtwfgs.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ql.gzmigu.cn

[U71] PHP：抛出异常
来源：http://rd.szxytkj.cn

throw new RuntimeException("失败", 500);
来源：http://ed.colortex.cn

[U72] PHP：写错误日志
来源：http://vh.nicolike.cn

error_log("失败: " . $e->getMessage());
来源：http://nv.colortex.cn

[U73] PHP：读取 ini 配置
来源：http://fe.asd995.cn

parse_ini_file("config.ini", true)
来源：http://zz.bjjhwx.cn

[U74] PHP：读取环境变量
来源：http://ww.shxzukj.cn

getenv("APP_ENV") ?: "production"
来源：http://eo.shtwfgs.cn

[U75] PHP：依赖注入
来源：http://ux.hnjuh.cn

composer require psr/container
来源：http://nu.haigaiapp.cn

[U76] PHP：简单路由
来源：http://ja.bookmarksfly.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nb.shtwfgs.cn

[U77] PHP：模板渲染
来源：http://yn.szxytkj.cn

composer require twig/twig
来源：http://bd.nszjky.cn

[U78] PHP：单元测试
来源：http://ak.shxzukj.cn

composer require --dev phpunit/phpunit
来源：http://cl.bjjhwx.cn

[U79] PHP：静态分析
来源：http://xu.bookmarksfly.cn

composer require --dev phpstan/phpstan
来源：http://an.huanxung.cn

[U80] PHP：代码规范修复
来源：http://ln.haigaiapp.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://kw.jctech888.com.cn

[U81] JS：初始化项目
来源：http://fc.colortex.cn

npm init -y;  npm i express
来源：http://rt.colortex.cn

[U82] JS：package.json 脚本
来源：http://kv.bookmarksfly.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ym.bjjhwx.cn

[U83] JS：ES Module 导入导出
来源：http://mb.shxzukj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://iy.szxytkj.cn

[U84] JS：CommonJS 写法
来源：http://yn.9csxet.cn

module.exports = { a };  const { a } = require("./m");
来源：http://zv.chemitech.net.cn

[U85] JS：可选链
来源：http://hv.nszjky.cn

a?.b?.c
来源：http://pq.chemitech.net.cn

[U86] JS：空值合并
来源：http://iy.jianghongdianzi.cn

a ?? b
来源：http://qg.shtwfgs.cn

[U87] JS：解构默认值
来源：http://ti.hahajie.cn

const { a = 1, b = 2 } = obj;
来源：http://ff.hnjuh.cn

[U88] JS：对象展开合并
来源：http://mg.jctech888.com.cn

{ ...a, ...b }
来源：http://am.newstarts.cn

[U89] JS：数组去重
来源：http://gx.jctech888.com.cn

[...new Set(arr)]
来源：http://zx.9csxet.cn

[U90] JS：数字数组排序
来源：http://kg.jctech888.com.cn

[...arr].sort((a, b) => a - b)
来源：http://iu.muxihuayi.cn

[U91] JS：对象键值遍历
来源：http://ko.szxytkj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cj.hnjuh.cn

[U92] JS：深拷贝
来源：http://ba.panjiajie.cn

structuredClone(obj)
来源：http://ov.newstarts.cn

[U93] JS：模板字符串
来源：http://wp.hnjuh.cn

`共 ${n} 条`
来源：http://pc.521024.cn

[U94] JS：箭头函数
来源：http://jf.jianghongdianzi.cn

const double = x => x * 2;
来源：http://af.jctech888.com.cn

[U95] JS：Promise 包装
来源：http://di.jianghongdianzi.cn

new Promise((resolve, reject) => {})
来源：http://pv.shtwfgs.cn

[U96] JS：async/await 与异常
来源：http://gp.bookmarksfly.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cu.yuexingan06.cn

[U97] JS：并发请求
来源：http://eq.gzmigu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bg.shxzukj.cn

[U98] JS：fetch 带 JSON
来源：http://ic.haigaiapp.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gt.shtwfgs.cn

[U99] JS：事件监听
来源：http://ss.muxihuayi.cn

el.addEventListener("click", e => {})
来源：http://dq.newstarts.cn

[U100] JS：DOM 查询
来源：http://sf.shxzskj.cn

document.querySelector(".item")
来源：http://rk.yuexingan06.cn

[U101] JS：classList 操作
来源：http://eq.haigaiapp.cn

el.classList.toggle("active")
来源：http://gg.9csxet.cn

[U102] JS：本地存储
来源：http://lb.chemitech.net.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://dp.521024.cn

[U103] JS：定时器
来源：http://ds.huixiangedu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://az.gzmigu.cn

[U104] JS：防抖
来源：http://lk.chemitech.net.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gc.muxihuayi.cn

[U105] JS：节流
来源：http://uf.bookmarksfly.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ks.nszjky.cn

[U106] JS：日期格式化
来源：http://lb.chemitech.net.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bf.huixiangedu.cn

[U107] JS：数字千分位
来源：http://wv.shtwfgs.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pb.asd995.cn

[U108] JS：随机整数
来源：http://yg.chemitech.net.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yn.newstarts.cn

[U109] JS：数组分组
来源：http://vv.colortex.cn

Object.groupBy(arr, x => x.type)
来源：http://dj.lnxyls.cn

[U110] JS：数组分块
来源：http://lw.jctech888.com.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ge.wgjwhj.cn

[U111] JS：对象转 Map
来源：http://za.shxzukj.cn

new Map(Object.entries(obj))
来源：http://po.shxzskj.cn

[U112] JS：字符串补位
来源：http://tu.wgjwhj.cn

"7".padStart(3, "0")
来源：http://ru.wgjwhj.cn

[U113] JS：正则替换全部
来源：http://vl.yuntaijiaju.cn

s.replaceAll("a", "b")
来源：http://ew.chemitech.net.cn

[U114] JS：JSON 深比较
来源：http://gk.szsharing.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://jh.lnxyls.cn

[U115] JS：生成 UUID
来源：http://rx.szxytkj.cn

crypto.randomUUID()
来源：http://az.shxzskj.cn

[U116] JS：类型检查（JSDoc）
来源：http://du.colortex.cn

/** @param {string} name */ function f(name) {}
来源：http://vf.9csxet.cn

[U117] JS：单元测试
来源：http://nu.bjjhwx.cn

npm i -D vitest;  npx vitest
来源：http://ta.jianghongdianzi.cn

[U118] JS：开发服务器
来源：http://md.newstarts.cn

npm i -D vite;  npx vite
来源：http://oe.colortex.cn

[U119] JS：生产构建
来源：http://lh.huixinmuqiang.cn

npx vite build
来源：http://dr.gzmigu.cn

[U120] JS：读取环境变量（Vite）
来源：http://gn.wgjwhj.cn

import.meta.env.VITE_API_URL
来源：http://km.yuexingan06.cn

================================================================================
来源：http://jz.muxihuayi.cn

统计汇总
来源：http://ii.bookmarksfly.cn

================================================================================
来源：http://fi.muxihuayi.cn

按语言统计（条）：
来源：http://iu.huixinmuqiang.cn

Python ......... 252
来源：http://se.newstarts.cn

PHP ............ 252
来源：http://uy.szsharing.cn

JavaScript ..... 252
来源：http://os.huixinmuqiang.cn

TypeScript ..... 212
来源：http://fl.9csxet.cn

Java ........... 212
来源：http://yr.colortex.cn

Go ............. 212
来源：http://zu.shxzskj.cn

Ruby ........... 212
来源：http://xd.huanxung.cn

C# ............. 212
来源：http://vs.bookmarksfly.cn

C .............. 30
来源：http://nd.chemitech.net.cn

C++ ............ 30
来源：http://tp.wgjwhj.cn

SQL ............ 90
来源：http://dd.newstarts.cn

Bash ........... 80
来源：http://fd.521024.cn

Kotlin ......... 15
来源：http://kt.jctech888.com.cn

Swift .......... 15
来源：http://li.huanxung.cn

Lua ............ 10
来源：http://hx.szsharing.cn

Perl ........... 10
来源：http://fv.nicolike.cn

Scala .......... 10
来源：http://ad.huixinmuqiang.cn

------------------------------------
来源：http://sg.9csxet.cn

合计 ........... 2106 条
来源：http://xh.newstarts.cn

按章节统计：
来源：http://le.szxytkj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yi.muxihuayi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yf.chemitech.net.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fn.asd995.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bu.yuexingan06.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.asd995.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pe.szxytkj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rm.nicolike.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://yc.hnjuh.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zw.jianghongdianzi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://js.newstarts.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://io.panjiajie.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xm.yuexingan06.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ls.jctech888.com.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://la.colortex.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pc.asd995.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://nt.shxzskj.cn

Q SQL 专题                              90
来源：http://yw.9csxet.cn

R Bash 专题                             80
来源：http://mm.hnjuh.cn

S C / C++ 专题                          60
来源：http://vy.asd995.cn

T 其他语言补充                          60
来源：http://oe.bookmarksfly.cn

U 高频实用片段                         120
来源：http://ug.chemitech.net.cn

------------------------------------
来源：http://wp.szsharing.cn

合计                                  2106 条
来源：http://jk.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://cd.chemitech.net.cn

使用提醒
来源：http://xb.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://lq.jctech888.com.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://sr.hnjuh.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zr.bjjhwx.cn


<!-- 参考信息 -->