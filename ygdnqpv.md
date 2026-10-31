代发 wailian999

[U01] Py：创建虚拟环境
来源：http://ig.huixinmuqiang.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ah.chemitech.net.cn

[U02] Py：导出 / 安装依赖
来源：http://aj.bjjhwx.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xl.szxytkj.cn

[U03] Py：加载 .env 配置
来源：http://kg.asd995.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://hu.hnjuh.cn

[U04] Py：变量调试打印
来源：http://gq.asd995.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gz.nszjky.cn

[U05] Py：列表去重且保序
来源：http://wg.huanxung.cn

list(dict.fromkeys(arr))
来源：http://bq.muxihuayi.cn

[U06] Py：合并两个字典
来源：http://ub.shxzskj.cn

{**a, **b}
来源：http://zm.nicolike.cn

[U07] Py：反转字典键值
来源：http://ro.hnjuh.cn

{v: k for k, v in d.items()}
来源：http://es.asd995.cn

[U08] Py：展平二维列表
来源：http://zw.hahajie.cn

[y for x in nested for y in x]
来源：http://yd.wgjwhj.cn

[U09] Py：字典取最大值的键
来源：http://hb.muxihuayi.cn

max(d, key=d.get)
来源：http://rx.yuexingan06.cn

[U10] Py：按值排序字典
来源：http://we.gzmigu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nl.wgjwhj.cn

[U11] Py：生成器表达式
来源：http://px.szsharing.cn

(x * 2 for x in arr)
来源：http://uk.huixinmuqiang.cn

[U12] Py：取出现最多的 3 个元素
来源：http://aw.haigaiapp.cn

Counter(arr).most_common(3)
来源：http://th.szsharing.cn

[U13] Py：固定长度队列
来源：http://su.yuntaijiaju.cn

deque(maxlen=10)
来源：http://xc.hahajie.cn

[U14] Py：分组收集到列表
来源：http://fh.huixinmuqiang.cn

defaultdict(list)
来源：http://ne.huixinmuqiang.cn

[U15] Py：高精度计时
来源：http://oc.jctech888.com.cn

t = time.perf_counter()
来源：http://yo.shtwfgs.cn

[U16] Py：命令行参数解析
来源：http://ma.muxihuayi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qb.bjjhwx.cn

[U17] Py：初始化日志
来源：http://tj.szsharing.cn

logging.basicConfig(level=logging.INFO)
来源：http://nv.yuexingan06.cn

[U18] Py：预编译正则
来源：http://un.wgjwhj.cn

pat = re.compile(r"\d+")
来源：http://xu.szsharing.cn

[U19] Py：正则替换带回调
来源：http://dd.wgjwhj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yl.lnxyls.cn

[U20] Py：缓存函数结果
来源：http://nv.nicolike.cn

@functools.lru_cache(maxsize=None)
来源：http://jw.shxzukj.cn

[U21] Py：自定义上下文管理器
来源：http://rt.wgjwhj.cn

@contextlib.contextmanager
来源：http://mr.wgjwhj.cn

[U22] Py：矩阵转置
来源：http://sg.muxihuayi.cn

list(zip(*m))
来源：http://bp.bjjhwx.cn

[U23] Py：分块读取大文件
来源：http://cz.huanxung.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wj.jianghongdianzi.cn

[U24] Py：路径操作
来源：http://jl.lnxyls.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zq.muxihuayi.cn

[U25] Py：CSV 按字典读
来源：http://ll.9csxet.cn

csv.DictReader(f)
来源：http://so.gzmigu.cn

[U26] Py：并发下载
来源：http://uk.colortex.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kc.yuexingan06.cn

[U27] Py：异步 HTTP
来源：http://xl.lnxyls.cn

aiohttp.ClientSession() 配合 async with
来源：http://pc.nicolike.cn

[U28] Py：类型别名
来源：http://nr.szsharing.cn

UserId = int
来源：http://bv.chemitech.net.cn

[U29] Py：属性校验
来源：http://uk.shtwfgs.cn

@property 与 @x.setter 配合
来源：http://zu.nszjky.cn

[U30] Py：数据类
来源：http://we.huixiangedu.cn

@dataclass(slots=True)
来源：http://ze.nicolike.cn

[U31] Py：单测
来源：http://rc.bjjhwx.cn

python -m pytest -q
来源：http://tr.panjiajie.cn

[U32] Py：代码格式化
来源：http://pd.muxihuayi.cn

ruff format . && ruff check --fix .
来源：http://fi.huanxung.cn

[U33] Py：打包发布
来源：http://ia.9csxet.cn

python -m build  （依赖 pyproject.toml）
来源：http://xr.muxihuayi.cn

[U34] Py：判断编码
来源：http://qq.yuntaijiaju.cn

chardet.detect(raw)
来源：http://gz.bookmarksfly.cn

[U35] Py：发送邮件
来源：http://mr.hnjuh.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zs.yuexingan06.cn

[U36] Py：定时任务
来源：http://ql.nszjky.cn

schedule.every(10).minutes.do(job)
来源：http://dg.nicolike.cn

[U37] Py：读写 Excel
来源：http://ob.haigaiapp.cn

pandas.read_excel / DataFrame.to_excel
来源：http://nd.yuexingan06.cn

[U38] Py：获取脚本所在目录
来源：http://nl.colortex.cn

Path(__file__).resolve().parent
来源：http://ax.muxihuayi.cn

[U39] Py：判断是否在交互环境
来源：http://pl.hnjuh.cn

sys.stdout.isatty()
来源：http://nn.lnxyls.cn

[U40] Py：打印到标准错误
来源：http://ka.yuntaijiaju.cn

print("err", file=sys.stderr)
来源：http://bm.shtwfgs.cn

[U41] PHP：初始化 Composer 项目
来源：http://qt.jctech888.com.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ck.lnxyls.cn

[U42] PHP：PSR-4 自动加载
来源：http://ib.shtwfgs.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pn.haigaiapp.cn

[U43] PHP：声明命名空间
来源：http://dn.newstarts.cn

namespace App\Http;
来源：http://tp.521024.cn

[U44] PHP：开启严格类型
来源：http://xm.wgjwhj.cn

declare(strict_types=1);
来源：http://xu.9csxet.cn

[U45] PHP：类型声明与返回类型
来源：http://ga.521024.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ah.colortex.cn

[U46] PHP：可空类型
来源：http://zi.jctech888.com.cn

?string $name = null
来源：http://sf.panjiajie.cn

[U47] PHP：联合类型
来源：http://la.521024.cn

int|string $id
来源：http://wy.huixiangedu.cn

[U48] PHP：纯枚举
来源：http://sk.panjiajie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wi.nicolike.cn

[U49] PHP：只读属性
来源：http://iz.lnxyls.cn

public readonly string $name
来源：http://jk.nicolike.cn

[U50] PHP：构造器属性提升
来源：http://bb.yuntaijiaju.cn

public function __construct(private int $id) {}
来源：http://pw.nicolike.cn

[U51] PHP：数组解构
来源：http://dr.wgjwhj.cn

[$a, $b] = $arr;
来源：http://je.wgjwhj.cn

[U52] PHP：箭头函数
来源：http://gr.newstarts.cn

$double = fn($x) => $x * 2;
来源：http://ul.gzmigu.cn

[U53] PHP：空合并运算符
来源：http://fy.hnjuh.cn

$v = $a ?? $b ?? "default";
来源：http://nz.newstarts.cn

[U54] PHP：空安全调用
来源：http://cd.colortex.cn

$obj?->method()
来源：http://gx.yuntaijiaju.cn

[U55] PHP：match 表达式
来源：http://wk.yuntaijiaju.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zt.hnjuh.cn

[U56] PHP：命名参数
来源：http://li.asd995.cn

f(a: 1, b: 2)
来源：http://uw.szxytkj.cn

[U57] PHP：字符串插值
来源：http://fj.huixinmuqiang.cn

"值: {$a}"
来源：http://xo.panjiajie.cn

[U58] PHP：数组三件套
来源：http://yv.hahajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tz.chemitech.net.cn

[U59] PHP：自定义排序
来源：http://kt.szxytkj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ak.colortex.cn

[U60] PHP：JSON 编解码
来源：http://uc.huixinmuqiang.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://no.muxihuayi.cn

[U61] PHP：正则
来源：http://fg.shxzukj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bu.nszjky.cn

[U62] PHP：日期对象
来源：http://zn.panjiajie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ny.bjjhwx.cn

[U63] PHP：文件读写
来源：http://jb.shxzukj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gh.yuntaijiaju.cn

[U64] PHP：目录遍历
来源：http://fb.shxzukj.cn

glob("dir/*.php");  scandir("dir");
来源：http://hx.shxzukj.cn

[U65] PHP：会话
来源：http://km.shxzukj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rl.muxihuayi.cn

[U66] PHP：设置 Cookie
来源：http://ap.yuexingan06.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xa.huixiangedu.cn

[U67] PHP：处理文件上传
来源：http://vj.lnxyls.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jp.bookmarksfly.cn

[U68] PHP：PDO 连接
来源：http://em.jianghongdianzi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wb.szxytkj.cn

[U69] PHP：PDO 预处理
来源：http://ej.haigaiapp.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cc.asd995.cn

[U70] PHP：PDO 事务
来源：http://xc.nicolike.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ii.hnjuh.cn

[U71] PHP：抛出异常
来源：http://hq.nicolike.cn

throw new RuntimeException("失败", 500);
来源：http://wk.bookmarksfly.cn

[U72] PHP：写错误日志
来源：http://fj.yuntaijiaju.cn

error_log("失败: " . $e->getMessage());
来源：http://cj.muxihuayi.cn

[U73] PHP：读取 ini 配置
来源：http://sg.shtwfgs.cn

parse_ini_file("config.ini", true)
来源：http://nd.gzmigu.cn

[U74] PHP：读取环境变量
来源：http://ev.shxzskj.cn

getenv("APP_ENV") ?: "production"
来源：http://td.jianghongdianzi.cn

[U75] PHP：依赖注入
来源：http://ha.huanxung.cn

composer require psr/container
来源：http://th.colortex.cn

[U76] PHP：简单路由
来源：http://di.9csxet.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ra.huixinmuqiang.cn

[U77] PHP：模板渲染
来源：http://iw.nszjky.cn

composer require twig/twig
来源：http://uz.jctech888.com.cn

[U78] PHP：单元测试
来源：http://kv.shtwfgs.cn

composer require --dev phpunit/phpunit
来源：http://gh.shtwfgs.cn

[U79] PHP：静态分析
来源：http://rm.wgjwhj.cn

composer require --dev phpstan/phpstan
来源：http://ta.newstarts.cn

[U80] PHP：代码规范修复
来源：http://cg.jctech888.com.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jc.jianghongdianzi.cn

[U81] JS：初始化项目
来源：http://gn.bookmarksfly.cn

npm init -y;  npm i express
来源：http://iy.asd995.cn

[U82] JS：package.json 脚本
来源：http://bv.yuexingan06.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://eu.asd995.cn

[U83] JS：ES Module 导入导出
来源：http://jg.yuntaijiaju.cn

export const a = 1;  import { a } from "./m.js";
来源：http://tv.huanxung.cn

[U84] JS：CommonJS 写法
来源：http://gy.shtwfgs.cn

module.exports = { a };  const { a } = require("./m");
来源：http://te.shxzskj.cn

[U85] JS：可选链
来源：http://ps.521024.cn

a?.b?.c
来源：http://dq.shxzskj.cn

[U86] JS：空值合并
来源：http://zl.colortex.cn

a ?? b
来源：http://zl.muxihuayi.cn

[U87] JS：解构默认值
来源：http://bg.bjjhwx.cn

const { a = 1, b = 2 } = obj;
来源：http://jq.panjiajie.cn

[U88] JS：对象展开合并
来源：http://jb.521024.cn

{ ...a, ...b }
来源：http://vs.haigaiapp.cn

[U89] JS：数组去重
来源：http://vu.huixinmuqiang.cn

[...new Set(arr)]
来源：http://wt.hahajie.cn

[U90] JS：数字数组排序
来源：http://ah.bookmarksfly.cn

[...arr].sort((a, b) => a - b)
来源：http://yd.szsharing.cn

[U91] JS：对象键值遍历
来源：http://be.shxzukj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://by.huixinmuqiang.cn

[U92] JS：深拷贝
来源：http://lv.9csxet.cn

structuredClone(obj)
来源：http://uz.newstarts.cn

[U93] JS：模板字符串
来源：http://oj.newstarts.cn

`共 ${n} 条`
来源：http://wi.chemitech.net.cn

[U94] JS：箭头函数
来源：http://ov.jianghongdianzi.cn

const double = x => x * 2;
来源：http://ta.muxihuayi.cn

[U95] JS：Promise 包装
来源：http://ch.nszjky.cn

new Promise((resolve, reject) => {})
来源：http://yt.hnjuh.cn

[U96] JS：async/await 与异常
来源：http://zq.shtwfgs.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yg.9csxet.cn

[U97] JS：并发请求
来源：http://kz.bjjhwx.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ym.colortex.cn

[U98] JS：fetch 带 JSON
来源：http://ii.jianghongdianzi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bq.hahajie.cn

[U99] JS：事件监听
来源：http://zp.wgjwhj.cn

el.addEventListener("click", e => {})
来源：http://pn.huixinmuqiang.cn

[U100] JS：DOM 查询
来源：http://zd.chemitech.net.cn

document.querySelector(".item")
来源：http://tt.panjiajie.cn

[U101] JS：classList 操作
来源：http://rq.asd995.cn

el.classList.toggle("active")
来源：http://la.szxytkj.cn

[U102] JS：本地存储
来源：http://uy.muxihuayi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://my.hnjuh.cn

[U103] JS：定时器
来源：http://ne.jctech888.com.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rl.9csxet.cn

[U104] JS：防抖
来源：http://yy.hahajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dw.bookmarksfly.cn

[U105] JS：节流
来源：http://tt.panjiajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hm.9csxet.cn

[U106] JS：日期格式化
来源：http://aa.haigaiapp.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bl.shtwfgs.cn

[U107] JS：数字千分位
来源：http://wi.yuntaijiaju.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vr.huixinmuqiang.cn

[U108] JS：随机整数
来源：http://mo.panjiajie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cu.shtwfgs.cn

[U109] JS：数组分组
来源：http://eb.muxihuayi.cn

Object.groupBy(arr, x => x.type)
来源：http://iz.shxzukj.cn

[U110] JS：数组分块
来源：http://fw.huanxung.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://sq.newstarts.cn

[U111] JS：对象转 Map
来源：http://bx.lnxyls.cn

new Map(Object.entries(obj))
来源：http://lx.huanxung.cn

[U112] JS：字符串补位
来源：http://ze.wgjwhj.cn

"7".padStart(3, "0")
来源：http://kw.bookmarksfly.cn

[U113] JS：正则替换全部
来源：http://co.colortex.cn

s.replaceAll("a", "b")
来源：http://fc.nszjky.cn

[U114] JS：JSON 深比较
来源：http://vm.shxzukj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://at.9csxet.cn

[U115] JS：生成 UUID
来源：http://gu.wgjwhj.cn

crypto.randomUUID()
来源：http://vt.hnjuh.cn

[U116] JS：类型检查（JSDoc）
来源：http://hf.nszjky.cn

/** @param {string} name */ function f(name) {}
来源：http://dy.nicolike.cn

[U117] JS：单元测试
来源：http://hq.yuntaijiaju.cn

npm i -D vitest;  npx vitest
来源：http://aq.panjiajie.cn

[U118] JS：开发服务器
来源：http://nf.shxzukj.cn

npm i -D vite;  npx vite
来源：http://zy.newstarts.cn

[U119] JS：生产构建
来源：http://rq.asd995.cn

npx vite build
来源：http://vb.muxihuayi.cn

[U120] JS：读取环境变量（Vite）
来源：http://dl.yuexingan06.cn

import.meta.env.VITE_API_URL
来源：http://tu.jianghongdianzi.cn

================================================================================
来源：http://re.hnjuh.cn

统计汇总
来源：http://sa.huanxung.cn

================================================================================
来源：http://xt.bjjhwx.cn

按语言统计（条）：
来源：http://hk.hahajie.cn

Python ......... 252
来源：http://qq.szxytkj.cn

PHP ............ 252
来源：http://vp.521024.cn

JavaScript ..... 252
来源：http://bo.chemitech.net.cn

TypeScript ..... 212
来源：http://ca.huanxung.cn

Java ........... 212
来源：http://uk.gzmigu.cn

Go ............. 212
来源：http://dq.9csxet.cn

Ruby ........... 212
来源：http://bb.asd995.cn

C# ............. 212
来源：http://kn.bjjhwx.cn

C .............. 30
来源：http://gf.chemitech.net.cn

C++ ............ 30
来源：http://zc.yuntaijiaju.cn

SQL ............ 90
来源：http://wj.chemitech.net.cn

Bash ........... 80
来源：http://bu.bjjhwx.cn

Kotlin ......... 15
来源：http://qj.wgjwhj.cn

Swift .......... 15
来源：http://si.panjiajie.cn

Lua ............ 10
来源：http://hj.yuexingan06.cn

Perl ........... 10
来源：http://zy.jctech888.com.cn

Scala .......... 10
来源：http://nq.panjiajie.cn

------------------------------------
来源：http://rr.yuntaijiaju.cn

合计 ........... 2106 条
来源：http://zj.9csxet.cn

按章节统计：
来源：http://th.hnjuh.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rz.huixiangedu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wu.shxzukj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://sg.bookmarksfly.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://oz.colortex.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ny.521024.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://py.nicolike.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wv.hnjuh.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://to.newstarts.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://sb.szsharing.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://pt.shxzukj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cv.yuntaijiaju.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wv.nicolike.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gw.chemitech.net.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ll.nicolike.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zy.lnxyls.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ck.hahajie.cn

Q SQL 专题                              90
来源：http://rk.jctech888.com.cn

R Bash 专题                             80
来源：http://at.huixinmuqiang.cn

S C / C++ 专题                          60
来源：http://uq.muxihuayi.cn

T 其他语言补充                          60
来源：http://qo.wgjwhj.cn

U 高频实用片段                         120
来源：http://oi.huanxung.cn

------------------------------------
来源：http://jr.panjiajie.cn

合计                                  2106 条
来源：http://ke.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://tj.hahajie.cn

使用提醒
来源：http://mu.521024.cn

--------------------------------------------------------------------------------
来源：http://yf.shxzskj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kd.lnxyls.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bm.shxzskj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qf.huixinmuqiang.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ep.gzmigu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fl.hahajie.cn

—— 文件结束 ——
来源：http://fp.shxzukj.cn

================================================================================
来源：http://as.hnjuh.cn

程序语言常见例子速查手册（2024 版）
来源：http://va.wgjwhj.cn

Common Programming Examples Cheat Book
来源：http://ib.9csxet.cn

================================================================================
来源：http://wg.huixinmuqiang.cn


<!-- 参考信息 -->