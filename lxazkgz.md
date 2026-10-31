代发 wailian999

[U01] Py：创建虚拟环境
来源：http://rp.yuntaijiaju.cn

python -m venv .venv && source .venv/bin/activate
来源：http://oh.wgjwhj.cn

[U02] Py：导出 / 安装依赖
来源：http://zz.szxytkj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pc.9csxet.cn

[U03] Py：加载 .env 配置
来源：http://nq.bookmarksfly.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://jc.nicolike.cn

[U04] Py：变量调试打印
来源：http://zr.jianghongdianzi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pz.wgjwhj.cn

[U05] Py：列表去重且保序
来源：http://no.szsharing.cn

list(dict.fromkeys(arr))
来源：http://ds.bjjhwx.cn

[U06] Py：合并两个字典
来源：http://fd.hahajie.cn

{**a, **b}
来源：http://oi.szxytkj.cn

[U07] Py：反转字典键值
来源：http://it.wgjwhj.cn

{v: k for k, v in d.items()}
来源：http://xf.nicolike.cn

[U08] Py：展平二维列表
来源：http://it.wgjwhj.cn

[y for x in nested for y in x]
来源：http://gr.huixiangedu.cn

[U09] Py：字典取最大值的键
来源：http://iu.nicolike.cn

max(d, key=d.get)
来源：http://nl.panjiajie.cn

[U10] Py：按值排序字典
来源：http://ui.jctech888.com.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uv.szxytkj.cn

[U11] Py：生成器表达式
来源：http://wd.colortex.cn

(x * 2 for x in arr)
来源：http://wu.lnxyls.cn

[U12] Py：取出现最多的 3 个元素
来源：http://sf.lnxyls.cn

Counter(arr).most_common(3)
来源：http://sp.9csxet.cn

[U13] Py：固定长度队列
来源：http://cq.shxzukj.cn

deque(maxlen=10)
来源：http://cb.panjiajie.cn

[U14] Py：分组收集到列表
来源：http://zl.chemitech.net.cn

defaultdict(list)
来源：http://hy.wgjwhj.cn

[U15] Py：高精度计时
来源：http://eb.muxihuayi.cn

t = time.perf_counter()
来源：http://zf.hnjuh.cn

[U16] Py：命令行参数解析
来源：http://qc.gzmigu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mm.szsharing.cn

[U17] Py：初始化日志
来源：http://yt.newstarts.cn

logging.basicConfig(level=logging.INFO)
来源：http://tl.shtwfgs.cn

[U18] Py：预编译正则
来源：http://px.shtwfgs.cn

pat = re.compile(r"\d+")
来源：http://xv.jctech888.com.cn

[U19] Py：正则替换带回调
来源：http://zq.muxihuayi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dt.wgjwhj.cn

[U20] Py：缓存函数结果
来源：http://bi.huixiangedu.cn

@functools.lru_cache(maxsize=None)
来源：http://wx.jctech888.com.cn

[U21] Py：自定义上下文管理器
来源：http://tp.jctech888.com.cn

@contextlib.contextmanager
来源：http://lz.yuntaijiaju.cn

[U22] Py：矩阵转置
来源：http://zl.bjjhwx.cn

list(zip(*m))
来源：http://nx.shxzukj.cn

[U23] Py：分块读取大文件
来源：http://io.panjiajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ma.bookmarksfly.cn

[U24] Py：路径操作
来源：http://ei.jctech888.com.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gv.haigaiapp.cn

[U25] Py：CSV 按字典读
来源：http://mw.hahajie.cn

csv.DictReader(f)
来源：http://bx.huixinmuqiang.cn

[U26] Py：并发下载
来源：http://hn.jctech888.com.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pb.nicolike.cn

[U27] Py：异步 HTTP
来源：http://pp.hnjuh.cn

aiohttp.ClientSession() 配合 async with
来源：http://pn.wgjwhj.cn

[U28] Py：类型别名
来源：http://en.521024.cn

UserId = int
来源：http://fp.9csxet.cn

[U29] Py：属性校验
来源：http://dr.yuexingan06.cn

@property 与 @x.setter 配合
来源：http://va.huixinmuqiang.cn

[U30] Py：数据类
来源：http://ds.szsharing.cn

@dataclass(slots=True)
来源：http://ay.jianghongdianzi.cn

[U31] Py：单测
来源：http://xh.gzmigu.cn

python -m pytest -q
来源：http://lf.huixinmuqiang.cn

[U32] Py：代码格式化
来源：http://rh.nicolike.cn

ruff format . && ruff check --fix .
来源：http://ek.nicolike.cn

[U33] Py：打包发布
来源：http://ef.521024.cn

python -m build  （依赖 pyproject.toml）
来源：http://ro.newstarts.cn

[U34] Py：判断编码
来源：http://jg.jianghongdianzi.cn

chardet.detect(raw)
来源：http://qe.9csxet.cn

[U35] Py：发送邮件
来源：http://cx.bookmarksfly.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mw.szxytkj.cn

[U36] Py：定时任务
来源：http://rh.9csxet.cn

schedule.every(10).minutes.do(job)
来源：http://it.hnjuh.cn

[U37] Py：读写 Excel
来源：http://le.huanxung.cn

pandas.read_excel / DataFrame.to_excel
来源：http://es.jctech888.com.cn

[U38] Py：获取脚本所在目录
来源：http://bb.panjiajie.cn

Path(__file__).resolve().parent
来源：http://sj.huixinmuqiang.cn

[U39] Py：判断是否在交互环境
来源：http://me.newstarts.cn

sys.stdout.isatty()
来源：http://yr.muxihuayi.cn

[U40] Py：打印到标准错误
来源：http://ou.hahajie.cn

print("err", file=sys.stderr)
来源：http://xg.huixiangedu.cn

[U41] PHP：初始化 Composer 项目
来源：http://fl.muxihuayi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://kv.gzmigu.cn

[U42] PHP：PSR-4 自动加载
来源：http://gq.panjiajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xq.wgjwhj.cn

[U43] PHP：声明命名空间
来源：http://jr.szsharing.cn

namespace App\Http;
来源：http://zr.jianghongdianzi.cn

[U44] PHP：开启严格类型
来源：http://xq.haigaiapp.cn

declare(strict_types=1);
来源：http://cy.chemitech.net.cn

[U45] PHP：类型声明与返回类型
来源：http://ze.bookmarksfly.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jb.wgjwhj.cn

[U46] PHP：可空类型
来源：http://kw.hahajie.cn

?string $name = null
来源：http://vt.asd995.cn

[U47] PHP：联合类型
来源：http://gt.huanxung.cn

int|string $id
来源：http://hg.wgjwhj.cn

[U48] PHP：纯枚举
来源：http://yb.shxzukj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rf.panjiajie.cn

[U49] PHP：只读属性
来源：http://sq.huanxung.cn

public readonly string $name
来源：http://nn.jianghongdianzi.cn

[U50] PHP：构造器属性提升
来源：http://fr.hnjuh.cn

public function __construct(private int $id) {}
来源：http://uj.newstarts.cn

[U51] PHP：数组解构
来源：http://bi.shxzskj.cn

[$a, $b] = $arr;
来源：http://dt.shxzukj.cn

[U52] PHP：箭头函数
来源：http://gh.hnjuh.cn

$double = fn($x) => $x * 2;
来源：http://oy.bookmarksfly.cn

[U53] PHP：空合并运算符
来源：http://de.jctech888.com.cn

$v = $a ?? $b ?? "default";
来源：http://du.lnxyls.cn

[U54] PHP：空安全调用
来源：http://th.nicolike.cn

$obj?->method()
来源：http://qm.9csxet.cn

[U55] PHP：match 表达式
来源：http://xb.shxzukj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cq.colortex.cn

[U56] PHP：命名参数
来源：http://nj.jianghongdianzi.cn

f(a: 1, b: 2)
来源：http://nd.hnjuh.cn

[U57] PHP：字符串插值
来源：http://ho.shxzskj.cn

"值: {$a}"
来源：http://pj.wgjwhj.cn

[U58] PHP：数组三件套
来源：http://ab.hahajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lc.huanxung.cn

[U59] PHP：自定义排序
来源：http://ge.521024.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ct.yuexingan06.cn

[U60] PHP：JSON 编解码
来源：http://ps.yuntaijiaju.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://op.colortex.cn

[U61] PHP：正则
来源：http://fp.9csxet.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pu.muxihuayi.cn

[U62] PHP：日期对象
来源：http://xz.shxzukj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zp.gzmigu.cn

[U63] PHP：文件读写
来源：http://de.huanxung.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hr.huanxung.cn

[U64] PHP：目录遍历
来源：http://jt.szxytkj.cn

glob("dir/*.php");  scandir("dir");
来源：http://ix.nszjky.cn

[U65] PHP：会话
来源：http://fk.lnxyls.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://qs.asd995.cn

[U66] PHP：设置 Cookie
来源：http://bv.chemitech.net.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mf.huanxung.cn

[U67] PHP：处理文件上传
来源：http://pr.lnxyls.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qx.wgjwhj.cn

[U68] PHP：PDO 连接
来源：http://fe.hnjuh.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ko.hnjuh.cn

[U69] PHP：PDO 预处理
来源：http://mc.gzmigu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://du.yuntaijiaju.cn

[U70] PHP：PDO 事务
来源：http://dx.wgjwhj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ca.bjjhwx.cn

[U71] PHP：抛出异常
来源：http://bx.huanxung.cn

throw new RuntimeException("失败", 500);
来源：http://wk.shxzukj.cn

[U72] PHP：写错误日志
来源：http://hc.shxzukj.cn

error_log("失败: " . $e->getMessage());
来源：http://qe.jctech888.com.cn

[U73] PHP：读取 ini 配置
来源：http://ip.hnjuh.cn

parse_ini_file("config.ini", true)
来源：http://ga.chemitech.net.cn

[U74] PHP：读取环境变量
来源：http://zt.hahajie.cn

getenv("APP_ENV") ?: "production"
来源：http://hr.gzmigu.cn

[U75] PHP：依赖注入
来源：http://de.521024.cn

composer require psr/container
来源：http://wd.asd995.cn

[U76] PHP：简单路由
来源：http://wd.nszjky.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gr.haigaiapp.cn

[U77] PHP：模板渲染
来源：http://ep.jctech888.com.cn

composer require twig/twig
来源：http://mi.jianghongdianzi.cn

[U78] PHP：单元测试
来源：http://ay.shxzukj.cn

composer require --dev phpunit/phpunit
来源：http://pt.jianghongdianzi.cn

[U79] PHP：静态分析
来源：http://lp.yuntaijiaju.cn

composer require --dev phpstan/phpstan
来源：http://gb.nicolike.cn

[U80] PHP：代码规范修复
来源：http://ja.9csxet.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://cu.yuexingan06.cn

[U81] JS：初始化项目
来源：http://pa.jctech888.com.cn

npm init -y;  npm i express
来源：http://zo.colortex.cn

[U82] JS：package.json 脚本
来源：http://mz.shxzukj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://em.nicolike.cn

[U83] JS：ES Module 导入导出
来源：http://sf.nszjky.cn

export const a = 1;  import { a } from "./m.js";
来源：http://it.hnjuh.cn

[U84] JS：CommonJS 写法
来源：http://aa.lnxyls.cn

module.exports = { a };  const { a } = require("./m");
来源：http://mg.muxihuayi.cn

[U85] JS：可选链
来源：http://fg.shxzskj.cn

a?.b?.c
来源：http://tk.muxihuayi.cn

[U86] JS：空值合并
来源：http://nv.shtwfgs.cn

a ?? b
来源：http://qj.gzmigu.cn

[U87] JS：解构默认值
来源：http://nm.colortex.cn

const { a = 1, b = 2 } = obj;
来源：http://vk.nszjky.cn

[U88] JS：对象展开合并
来源：http://at.521024.cn

{ ...a, ...b }
来源：http://gr.9csxet.cn

[U89] JS：数组去重
来源：http://zl.nicolike.cn

[...new Set(arr)]
来源：http://xg.asd995.cn

[U90] JS：数字数组排序
来源：http://wz.bjjhwx.cn

[...arr].sort((a, b) => a - b)
来源：http://lc.shxzukj.cn

[U91] JS：对象键值遍历
来源：http://ox.yuexingan06.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fo.huixinmuqiang.cn

[U92] JS：深拷贝
来源：http://tp.huanxung.cn

structuredClone(obj)
来源：http://gx.colortex.cn

[U93] JS：模板字符串
来源：http://iy.nicolike.cn

`共 ${n} 条`
来源：http://gf.wgjwhj.cn

[U94] JS：箭头函数
来源：http://em.jctech888.com.cn

const double = x => x * 2;
来源：http://eo.9csxet.cn

[U95] JS：Promise 包装
来源：http://jl.521024.cn

new Promise((resolve, reject) => {})
来源：http://df.szsharing.cn

[U96] JS：async/await 与异常
来源：http://qt.jianghongdianzi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sn.hnjuh.cn

[U97] JS：并发请求
来源：http://ff.521024.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://tp.shtwfgs.cn

[U98] JS：fetch 带 JSON
来源：http://jf.muxihuayi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zp.szsharing.cn

[U99] JS：事件监听
来源：http://vt.shxzskj.cn

el.addEventListener("click", e => {})
来源：http://lm.521024.cn

[U100] JS：DOM 查询
来源：http://ba.huixiangedu.cn

document.querySelector(".item")
来源：http://lb.hahajie.cn

[U101] JS：classList 操作
来源：http://xd.bjjhwx.cn

el.classList.toggle("active")
来源：http://ol.wgjwhj.cn

[U102] JS：本地存储
来源：http://rb.shxzukj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://up.bjjhwx.cn

[U103] JS：定时器
来源：http://dz.bjjhwx.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://eo.muxihuayi.cn

[U104] JS：防抖
来源：http://gk.bjjhwx.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fq.yuntaijiaju.cn

[U105] JS：节流
来源：http://rt.hnjuh.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ay.jctech888.com.cn

[U106] JS：日期格式化
来源：http://kz.shtwfgs.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xk.yuntaijiaju.cn

[U107] JS：数字千分位
来源：http://ua.colortex.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jy.shxzskj.cn

[U108] JS：随机整数
来源：http://do.hahajie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://uu.yuntaijiaju.cn

[U109] JS：数组分组
来源：http://au.yuexingan06.cn

Object.groupBy(arr, x => x.type)
来源：http://ff.nszjky.cn

[U110] JS：数组分块
来源：http://qh.panjiajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ap.colortex.cn

[U111] JS：对象转 Map
来源：http://tt.shxzukj.cn

new Map(Object.entries(obj))
来源：http://qu.muxihuayi.cn

[U112] JS：字符串补位
来源：http://it.yuexingan06.cn

"7".padStart(3, "0")
来源：http://vj.shxzukj.cn

[U113] JS：正则替换全部
来源：http://mn.shtwfgs.cn

s.replaceAll("a", "b")
来源：http://ks.huixinmuqiang.cn

[U114] JS：JSON 深比较
来源：http://gt.nicolike.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://iq.newstarts.cn

[U115] JS：生成 UUID
来源：http://nu.nicolike.cn

crypto.randomUUID()
来源：http://ww.jctech888.com.cn

[U116] JS：类型检查（JSDoc）
来源：http://nb.nicolike.cn

/** @param {string} name */ function f(name) {}
来源：http://gv.szsharing.cn

[U117] JS：单元测试
来源：http://qs.gzmigu.cn

npm i -D vitest;  npx vitest
来源：http://ib.9csxet.cn

[U118] JS：开发服务器
来源：http://an.521024.cn

npm i -D vite;  npx vite
来源：http://aq.lnxyls.cn

[U119] JS：生产构建
来源：http://yo.jianghongdianzi.cn

npx vite build
来源：http://ae.shxzukj.cn

[U120] JS：读取环境变量（Vite）
来源：http://wo.shtwfgs.cn

import.meta.env.VITE_API_URL
来源：http://zj.haigaiapp.cn

================================================================================
来源：http://js.yuntaijiaju.cn

统计汇总
来源：http://ov.bookmarksfly.cn

================================================================================
来源：http://dx.colortex.cn

按语言统计（条）：
来源：http://xd.jianghongdianzi.cn

Python ......... 252
来源：http://ch.9csxet.cn

PHP ............ 252
来源：http://mv.nicolike.cn

JavaScript ..... 252
来源：http://oi.chemitech.net.cn

TypeScript ..... 212
来源：http://vu.asd995.cn

Java ........... 212
来源：http://gs.lnxyls.cn

Go ............. 212
来源：http://wa.newstarts.cn

Ruby ........... 212
来源：http://ca.shtwfgs.cn

C# ............. 212
来源：http://lm.huixiangedu.cn

C .............. 30
来源：http://ee.jctech888.com.cn

C++ ............ 30
来源：http://ww.hnjuh.cn

SQL ............ 90
来源：http://gg.colortex.cn

Bash ........... 80
来源：http://ya.jctech888.com.cn

Kotlin ......... 15
来源：http://su.lnxyls.cn

Swift .......... 15
来源：http://km.521024.cn

Lua ............ 10
来源：http://hw.lnxyls.cn

Perl ........... 10
来源：http://as.szxytkj.cn

Scala .......... 10
来源：http://le.shxzukj.cn

------------------------------------
来源：http://hy.huixiangedu.cn

合计 ........... 2106 条
来源：http://yf.yuexingan06.cn

按章节统计：
来源：http://xs.szxytkj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bx.panjiajie.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://di.huanxung.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vq.asd995.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://uc.hnjuh.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dp.szsharing.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fr.huanxung.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://um.shxzukj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xj.jianghongdianzi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qx.hnjuh.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mk.hnjuh.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ju.9csxet.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mk.asd995.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ql.hnjuh.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dg.panjiajie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://uy.huanxung.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vv.muxihuayi.cn

Q SQL 专题                              90
来源：http://at.colortex.cn

R Bash 专题                             80
来源：http://pj.szxytkj.cn

S C / C++ 专题                          60
来源：http://cl.jianghongdianzi.cn

T 其他语言补充                          60
来源：http://sa.bookmarksfly.cn

U 高频实用片段                         120
来源：http://aw.hahajie.cn

------------------------------------
来源：http://ov.huixiangedu.cn

合计                                  2106 条
来源：http://gz.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://yt.muxihuayi.cn

使用提醒
来源：http://zv.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://ov.hnjuh.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vi.hahajie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ez.szxytkj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xu.szxytkj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://gy.shxzskj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://pe.wgjwhj.cn

—— 文件结束 ——
来源：http://tw.jctech888.com.cn

================================================================================
来源：http://xz.huixinmuqiang.cn

程序语言常见例子速查手册（2024 版）
来源：http://kw.haigaiapp.cn

Common Programming Examples Cheat Book
来源：http://ub.yuexingan06.cn

================================================================================
来源：http://db.shxzskj.cn


<!-- 参考信息 -->