代发 wailian999

[U01] Py：创建虚拟环境
来源：http://rf.shxzukj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bl.chemitech.net.cn

[U02] Py：导出 / 安装依赖
来源：http://if.panjiajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qx.szsharing.cn

[U03] Py：加载 .env 配置
来源：http://hb.huanxung.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fg.asd995.cn

[U04] Py：变量调试打印
来源：http://fn.huixinmuqiang.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ta.huixinmuqiang.cn

[U05] Py：列表去重且保序
来源：http://tm.yuntaijiaju.cn

list(dict.fromkeys(arr))
来源：http://op.muxihuayi.cn

[U06] Py：合并两个字典
来源：http://lp.shxzskj.cn

{**a, **b}
来源：http://za.shtwfgs.cn

[U07] Py：反转字典键值
来源：http://eb.huixiangedu.cn

{v: k for k, v in d.items()}
来源：http://hj.yuexingan06.cn

[U08] Py：展平二维列表
来源：http://zp.chemitech.net.cn

[y for x in nested for y in x]
来源：http://jt.shtwfgs.cn

[U09] Py：字典取最大值的键
来源：http://fj.hnjuh.cn

max(d, key=d.get)
来源：http://uz.bookmarksfly.cn

[U10] Py：按值排序字典
来源：http://nh.wgjwhj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nw.yuexingan06.cn

[U11] Py：生成器表达式
来源：http://yi.lnxyls.cn

(x * 2 for x in arr)
来源：http://ii.bookmarksfly.cn

[U12] Py：取出现最多的 3 个元素
来源：http://bc.521024.cn

Counter(arr).most_common(3)
来源：http://cj.muxihuayi.cn

[U13] Py：固定长度队列
来源：http://hy.panjiajie.cn

deque(maxlen=10)
来源：http://kz.panjiajie.cn

[U14] Py：分组收集到列表
来源：http://xl.nszjky.cn

defaultdict(list)
来源：http://he.muxihuayi.cn

[U15] Py：高精度计时
来源：http://pr.jctech888.com.cn

t = time.perf_counter()
来源：http://hz.hnjuh.cn

[U16] Py：命令行参数解析
来源：http://lp.wgjwhj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sd.huixinmuqiang.cn

[U17] Py：初始化日志
来源：http://tx.bookmarksfly.cn

logging.basicConfig(level=logging.INFO)
来源：http://mi.9csxet.cn

[U18] Py：预编译正则
来源：http://dh.huixiangedu.cn

pat = re.compile(r"\d+")
来源：http://ef.szxytkj.cn

[U19] Py：正则替换带回调
来源：http://mn.bjjhwx.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hp.muxihuayi.cn

[U20] Py：缓存函数结果
来源：http://mi.shxzukj.cn

@functools.lru_cache(maxsize=None)
来源：http://di.wgjwhj.cn

[U21] Py：自定义上下文管理器
来源：http://iz.hnjuh.cn

@contextlib.contextmanager
来源：http://ki.lnxyls.cn

[U22] Py：矩阵转置
来源：http://lz.bookmarksfly.cn

list(zip(*m))
来源：http://az.hahajie.cn

[U23] Py：分块读取大文件
来源：http://rc.wgjwhj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lv.szsharing.cn

[U24] Py：路径操作
来源：http://il.nicolike.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nt.muxihuayi.cn

[U25] Py：CSV 按字典读
来源：http://hp.lnxyls.cn

csv.DictReader(f)
来源：http://ce.hahajie.cn

[U26] Py：并发下载
来源：http://kj.newstarts.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ol.jianghongdianzi.cn

[U27] Py：异步 HTTP
来源：http://oi.jianghongdianzi.cn

aiohttp.ClientSession() 配合 async with
来源：http://aa.bookmarksfly.cn

[U28] Py：类型别名
来源：http://pr.asd995.cn

UserId = int
来源：http://my.newstarts.cn

[U29] Py：属性校验
来源：http://vz.asd995.cn

@property 与 @x.setter 配合
来源：http://pl.szsharing.cn

[U30] Py：数据类
来源：http://ev.shxzukj.cn

@dataclass(slots=True)
来源：http://ae.panjiajie.cn

[U31] Py：单测
来源：http://ft.lnxyls.cn

python -m pytest -q
来源：http://tl.haigaiapp.cn

[U32] Py：代码格式化
来源：http://uz.huixinmuqiang.cn

ruff format . && ruff check --fix .
来源：http://fx.chemitech.net.cn

[U33] Py：打包发布
来源：http://gs.nszjky.cn

python -m build  （依赖 pyproject.toml）
来源：http://gn.nicolike.cn

[U34] Py：判断编码
来源：http://zm.szxytkj.cn

chardet.detect(raw)
来源：http://qc.panjiajie.cn

[U35] Py：发送邮件
来源：http://re.asd995.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dh.shxzukj.cn

[U36] Py：定时任务
来源：http://lb.asd995.cn

schedule.every(10).minutes.do(job)
来源：http://yq.gzmigu.cn

[U37] Py：读写 Excel
来源：http://lm.shxzukj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://kq.nicolike.cn

[U38] Py：获取脚本所在目录
来源：http://gv.shxzukj.cn

Path(__file__).resolve().parent
来源：http://gh.huixinmuqiang.cn

[U39] Py：判断是否在交互环境
来源：http://tn.hahajie.cn

sys.stdout.isatty()
来源：http://wr.haigaiapp.cn

[U40] Py：打印到标准错误
来源：http://nq.yuexingan06.cn

print("err", file=sys.stderr)
来源：http://dy.huixinmuqiang.cn

[U41] PHP：初始化 Composer 项目
来源：http://yc.hnjuh.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://cd.newstarts.cn

[U42] PHP：PSR-4 自动加载
来源：http://nz.jianghongdianzi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ep.lnxyls.cn

[U43] PHP：声明命名空间
来源：http://pk.521024.cn

namespace App\Http;
来源：http://jr.asd995.cn

[U44] PHP：开启严格类型
来源：http://fh.nszjky.cn

declare(strict_types=1);
来源：http://iw.newstarts.cn

[U45] PHP：类型声明与返回类型
来源：http://gb.panjiajie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://yk.bookmarksfly.cn

[U46] PHP：可空类型
来源：http://xr.hahajie.cn

?string $name = null
来源：http://yg.hnjuh.cn

[U47] PHP：联合类型
来源：http://ju.yuntaijiaju.cn

int|string $id
来源：http://nx.9csxet.cn

[U48] PHP：纯枚举
来源：http://rc.huixinmuqiang.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nt.gzmigu.cn

[U49] PHP：只读属性
来源：http://yk.wgjwhj.cn

public readonly string $name
来源：http://ho.jianghongdianzi.cn

[U50] PHP：构造器属性提升
来源：http://hh.lnxyls.cn

public function __construct(private int $id) {}
来源：http://ru.521024.cn

[U51] PHP：数组解构
来源：http://dt.asd995.cn

[$a, $b] = $arr;
来源：http://zu.huixiangedu.cn

[U52] PHP：箭头函数
来源：http://ig.haigaiapp.cn

$double = fn($x) => $x * 2;
来源：http://wh.yuexingan06.cn

[U53] PHP：空合并运算符
来源：http://oz.jctech888.com.cn

$v = $a ?? $b ?? "default";
来源：http://te.bookmarksfly.cn

[U54] PHP：空安全调用
来源：http://gn.szsharing.cn

$obj?->method()
来源：http://om.bjjhwx.cn

[U55] PHP：match 表达式
来源：http://lb.nicolike.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lx.chemitech.net.cn

[U56] PHP：命名参数
来源：http://xt.colortex.cn

f(a: 1, b: 2)
来源：http://cg.lnxyls.cn

[U57] PHP：字符串插值
来源：http://em.jctech888.com.cn

"值: {$a}"
来源：http://fw.asd995.cn

[U58] PHP：数组三件套
来源：http://gk.yuntaijiaju.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://za.panjiajie.cn

[U59] PHP：自定义排序
来源：http://cl.jianghongdianzi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://io.huixiangedu.cn

[U60] PHP：JSON 编解码
来源：http://of.haigaiapp.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://oe.szsharing.cn

[U61] PHP：正则
来源：http://ty.521024.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ld.shxzukj.cn

[U62] PHP：日期对象
来源：http://jo.huixinmuqiang.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://eg.panjiajie.cn

[U63] PHP：文件读写
来源：http://kf.jianghongdianzi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://cn.bookmarksfly.cn

[U64] PHP：目录遍历
来源：http://wk.wgjwhj.cn

glob("dir/*.php");  scandir("dir");
来源：http://lf.shxzskj.cn

[U65] PHP：会话
来源：http://rb.shxzukj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ct.jctech888.com.cn

[U66] PHP：设置 Cookie
来源：http://by.bookmarksfly.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cc.huixiangedu.cn

[U67] PHP：处理文件上传
来源：http://ma.haigaiapp.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qu.hahajie.cn

[U68] PHP：PDO 连接
来源：http://kx.hahajie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nz.muxihuayi.cn

[U69] PHP：PDO 预处理
来源：http://yb.jctech888.com.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://aj.chemitech.net.cn

[U70] PHP：PDO 事务
来源：http://pz.shxzskj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tg.panjiajie.cn

[U71] PHP：抛出异常
来源：http://hg.bjjhwx.cn

throw new RuntimeException("失败", 500);
来源：http://ik.jianghongdianzi.cn

[U72] PHP：写错误日志
来源：http://tj.jianghongdianzi.cn

error_log("失败: " . $e->getMessage());
来源：http://ph.shxzskj.cn

[U73] PHP：读取 ini 配置
来源：http://ui.hnjuh.cn

parse_ini_file("config.ini", true)
来源：http://an.szsharing.cn

[U74] PHP：读取环境变量
来源：http://dq.huixiangedu.cn

getenv("APP_ENV") ?: "production"
来源：http://jb.521024.cn

[U75] PHP：依赖注入
来源：http://tb.hnjuh.cn

composer require psr/container
来源：http://cy.hnjuh.cn

[U76] PHP：简单路由
来源：http://tq.huixiangedu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://oz.jctech888.com.cn

[U77] PHP：模板渲染
来源：http://je.huixiangedu.cn

composer require twig/twig
来源：http://jo.yuexingan06.cn

[U78] PHP：单元测试
来源：http://vu.9csxet.cn

composer require --dev phpunit/phpunit
来源：http://hk.yuntaijiaju.cn

[U79] PHP：静态分析
来源：http://ma.hnjuh.cn

composer require --dev phpstan/phpstan
来源：http://vc.jianghongdianzi.cn

[U80] PHP：代码规范修复
来源：http://yv.yuexingan06.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jo.colortex.cn

[U81] JS：初始化项目
来源：http://gr.yuntaijiaju.cn

npm init -y;  npm i express
来源：http://fs.lnxyls.cn

[U82] JS：package.json 脚本
来源：http://ci.yuexingan06.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jb.yuntaijiaju.cn

[U83] JS：ES Module 导入导出
来源：http://ma.shtwfgs.cn

export const a = 1;  import { a } from "./m.js";
来源：http://gl.newstarts.cn

[U84] JS：CommonJS 写法
来源：http://lj.huixiangedu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://fm.huanxung.cn

[U85] JS：可选链
来源：http://wb.panjiajie.cn

a?.b?.c
来源：http://mx.huanxung.cn

[U86] JS：空值合并
来源：http://wb.jctech888.com.cn

a ?? b
来源：http://oy.bookmarksfly.cn

[U87] JS：解构默认值
来源：http://yu.nszjky.cn

const { a = 1, b = 2 } = obj;
来源：http://fi.wgjwhj.cn

[U88] JS：对象展开合并
来源：http://nt.muxihuayi.cn

{ ...a, ...b }
来源：http://pp.jctech888.com.cn

[U89] JS：数组去重
来源：http://ru.gzmigu.cn

[...new Set(arr)]
来源：http://bx.shxzskj.cn

[U90] JS：数字数组排序
来源：http://vg.jctech888.com.cn

[...arr].sort((a, b) => a - b)
来源：http://ur.lnxyls.cn

[U91] JS：对象键值遍历
来源：http://fe.jianghongdianzi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://de.521024.cn

[U92] JS：深拷贝
来源：http://ni.bookmarksfly.cn

structuredClone(obj)
来源：http://si.szsharing.cn

[U93] JS：模板字符串
来源：http://ii.hahajie.cn

`共 ${n} 条`
来源：http://yd.yuexingan06.cn

[U94] JS：箭头函数
来源：http://ww.szsharing.cn

const double = x => x * 2;
来源：http://nc.shtwfgs.cn

[U95] JS：Promise 包装
来源：http://jq.newstarts.cn

new Promise((resolve, reject) => {})
来源：http://ji.bjjhwx.cn

[U96] JS：async/await 与异常
来源：http://ud.hahajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yr.bjjhwx.cn

[U97] JS：并发请求
来源：http://cp.asd995.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://tw.bookmarksfly.cn

[U98] JS：fetch 带 JSON
来源：http://rd.lnxyls.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xf.shxzskj.cn

[U99] JS：事件监听
来源：http://vg.newstarts.cn

el.addEventListener("click", e => {})
来源：http://xb.shtwfgs.cn

[U100] JS：DOM 查询
来源：http://vs.wgjwhj.cn

document.querySelector(".item")
来源：http://up.521024.cn

[U101] JS：classList 操作
来源：http://wv.jianghongdianzi.cn

el.classList.toggle("active")
来源：http://uz.yuexingan06.cn

[U102] JS：本地存储
来源：http://yc.shxzukj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ql.colortex.cn

[U103] JS：定时器
来源：http://dm.yuntaijiaju.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ok.huixiangedu.cn

[U104] JS：防抖
来源：http://zg.bookmarksfly.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zl.hnjuh.cn

[U105] JS：节流
来源：http://ps.jctech888.com.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bg.lnxyls.cn

[U106] JS：日期格式化
来源：http://zp.jianghongdianzi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://im.yuexingan06.cn

[U107] JS：数字千分位
来源：http://zd.yuexingan06.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wt.huixinmuqiang.cn

[U108] JS：随机整数
来源：http://cp.yuntaijiaju.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hc.gzmigu.cn

[U109] JS：数组分组
来源：http://wa.jianghongdianzi.cn

Object.groupBy(arr, x => x.type)
来源：http://jw.huixiangedu.cn

[U110] JS：数组分块
来源：http://zt.bjjhwx.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tq.colortex.cn

[U111] JS：对象转 Map
来源：http://rg.newstarts.cn

new Map(Object.entries(obj))
来源：http://ud.shxzskj.cn

[U112] JS：字符串补位
来源：http://ap.huixiangedu.cn

"7".padStart(3, "0")
来源：http://ao.wgjwhj.cn

[U113] JS：正则替换全部
来源：http://mj.newstarts.cn

s.replaceAll("a", "b")
来源：http://mo.chemitech.net.cn

[U114] JS：JSON 深比较
来源：http://ow.hahajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ni.hahajie.cn

[U115] JS：生成 UUID
来源：http://ti.9csxet.cn

crypto.randomUUID()
来源：http://en.wgjwhj.cn

[U116] JS：类型检查（JSDoc）
来源：http://ft.huanxung.cn

/** @param {string} name */ function f(name) {}
来源：http://sn.bookmarksfly.cn

[U117] JS：单元测试
来源：http://us.gzmigu.cn

npm i -D vitest;  npx vitest
来源：http://hp.bookmarksfly.cn

[U118] JS：开发服务器
来源：http://pd.huanxung.cn

npm i -D vite;  npx vite
来源：http://sp.gzmigu.cn

[U119] JS：生产构建
来源：http://gr.hahajie.cn

npx vite build
来源：http://jq.muxihuayi.cn

[U120] JS：读取环境变量（Vite）
来源：http://pv.huixinmuqiang.cn

import.meta.env.VITE_API_URL
来源：http://pn.asd995.cn

================================================================================
来源：http://rh.asd995.cn

统计汇总
来源：http://ev.jctech888.com.cn

================================================================================
来源：http://zb.newstarts.cn

按语言统计（条）：
来源：http://tm.hnjuh.cn

Python ......... 252
来源：http://te.shxzukj.cn

PHP ............ 252
来源：http://ey.szsharing.cn

JavaScript ..... 252
来源：http://kb.huixinmuqiang.cn

TypeScript ..... 212
来源：http://gt.wgjwhj.cn

Java ........... 212
来源：http://gv.521024.cn

Go ............. 212
来源：http://ni.szxytkj.cn

Ruby ........... 212
来源：http://cz.yuexingan06.cn

C# ............. 212
来源：http://wg.shtwfgs.cn

C .............. 30
来源：http://ti.nszjky.cn

C++ ............ 30
来源：http://jm.szsharing.cn

SQL ............ 90
来源：http://ai.bjjhwx.cn

Bash ........... 80
来源：http://cf.shtwfgs.cn

Kotlin ......... 15
来源：http://qt.huixiangedu.cn

Swift .......... 15
来源：http://bi.huixiangedu.cn

Lua ............ 10
来源：http://zw.bookmarksfly.cn

Perl ........... 10
来源：http://ek.wgjwhj.cn

Scala .......... 10
来源：http://ri.shxzukj.cn

------------------------------------
来源：http://xo.hnjuh.cn

合计 ........... 2106 条
来源：http://kg.newstarts.cn

按章节统计：
来源：http://jt.huixiangedu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jb.colortex.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://up.haigaiapp.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wj.huanxung.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ny.wgjwhj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://yv.shxzskj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qy.colortex.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rn.szxytkj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lw.shxzukj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yp.szxytkj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://va.521024.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jx.lnxyls.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://va.lnxyls.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dg.shtwfgs.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ip.yuexingan06.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mb.shxzskj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cf.bjjhwx.cn

Q SQL 专题                              90
来源：http://kh.yuexingan06.cn

R Bash 专题                             80
来源：http://lc.hnjuh.cn

S C / C++ 专题                          60
来源：http://ub.521024.cn

T 其他语言补充                          60
来源：http://jt.hahajie.cn

U 高频实用片段                         120
来源：http://yd.szxytkj.cn

------------------------------------
来源：http://yk.bjjhwx.cn

合计                                  2106 条
来源：http://bx.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://sp.gzmigu.cn

使用提醒
来源：http://hy.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://vc.szxytkj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kj.9csxet.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://in.huanxung.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://sm.yuntaijiaju.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://rb.jianghongdianzi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://eb.nszjky.cn

—— 文件结束 ——
来源：http://zf.shxzukj.cn

================================================================================
来源：http://mr.huanxung.cn

程序语言常见例子速查手册（2024 版）
来源：http://te.hnjuh.cn

Common Programming Examples Cheat Book
来源：http://nf.chemitech.net.cn

================================================================================
来源：http://bt.shxzskj.cn


<!-- 参考信息 -->