代发 wailian999

[U03] Py：加载 .env 配置
来源：http://jc.szxytkj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ra.bookmarksfly.cn

[U04] Py：变量调试打印
来源：http://su.haigaiapp.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://be.bookmarksfly.cn

[U05] Py：列表去重且保序
来源：http://fe.shxzskj.cn

list(dict.fromkeys(arr))
来源：http://gw.nicolike.cn

[U06] Py：合并两个字典
来源：http://jd.haigaiapp.cn

{**a, **b}
来源：http://eq.shxzskj.cn

[U07] Py：反转字典键值
来源：http://sg.chemitech.net.cn

{v: k for k, v in d.items()}
来源：http://ul.jctech888.com.cn

[U08] Py：展平二维列表
来源：http://zk.huixinmuqiang.cn

[y for x in nested for y in x]
来源：http://ka.521024.cn

[U09] Py：字典取最大值的键
来源：http://hh.521024.cn

max(d, key=d.get)
来源：http://bx.szxytkj.cn

[U10] Py：按值排序字典
来源：http://qs.shtwfgs.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ab.huanxung.cn

[U11] Py：生成器表达式
来源：http://kp.szxytkj.cn

(x * 2 for x in arr)
来源：http://mi.newstarts.cn

[U12] Py：取出现最多的 3 个元素
来源：http://dw.asd995.cn

Counter(arr).most_common(3)
来源：http://pd.haigaiapp.cn

[U13] Py：固定长度队列
来源：http://ae.szxytkj.cn

deque(maxlen=10)
来源：http://ny.gzmigu.cn

[U14] Py：分组收集到列表
来源：http://cm.wgjwhj.cn

defaultdict(list)
来源：http://oa.9csxet.cn

[U15] Py：高精度计时
来源：http://qw.bjjhwx.cn

t = time.perf_counter()
来源：http://an.jianghongdianzi.cn

[U16] Py：命令行参数解析
来源：http://ey.huixiangedu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://co.gzmigu.cn

[U17] Py：初始化日志
来源：http://bo.yuexingan06.cn

logging.basicConfig(level=logging.INFO)
来源：http://qn.huanxung.cn

[U18] Py：预编译正则
来源：http://ku.newstarts.cn

pat = re.compile(r"\d+")
来源：http://bs.shxzskj.cn

[U19] Py：正则替换带回调
来源：http://yq.newstarts.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sf.bjjhwx.cn

[U20] Py：缓存函数结果
来源：http://hb.yuntaijiaju.cn

@functools.lru_cache(maxsize=None)
来源：http://sa.hahajie.cn

[U21] Py：自定义上下文管理器
来源：http://gx.hnjuh.cn

@contextlib.contextmanager
来源：http://tc.huixiangedu.cn

[U22] Py：矩阵转置
来源：http://xe.jctech888.com.cn

list(zip(*m))
来源：http://ca.szsharing.cn

[U23] Py：分块读取大文件
来源：http://pz.huanxung.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://av.9csxet.cn

[U24] Py：路径操作
来源：http://fb.bookmarksfly.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yo.huixiangedu.cn

[U25] Py：CSV 按字典读
来源：http://dg.bjjhwx.cn

csv.DictReader(f)
来源：http://vf.wgjwhj.cn

[U26] Py：并发下载
来源：http://zm.panjiajie.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wd.yuexingan06.cn

[U27] Py：异步 HTTP
来源：http://me.wgjwhj.cn

aiohttp.ClientSession() 配合 async with
来源：http://hx.521024.cn

[U28] Py：类型别名
来源：http://te.panjiajie.cn

UserId = int
来源：http://tj.nszjky.cn

[U29] Py：属性校验
来源：http://vp.huixiangedu.cn

@property 与 @x.setter 配合
来源：http://wk.jianghongdianzi.cn

[U30] Py：数据类
来源：http://vq.colortex.cn

@dataclass(slots=True)
来源：http://bs.chemitech.net.cn

[U31] Py：单测
来源：http://fw.shxzukj.cn

python -m pytest -q
来源：http://go.wgjwhj.cn

[U32] Py：代码格式化
来源：http://yj.yuexingan06.cn

ruff format . && ruff check --fix .
来源：http://ou.bookmarksfly.cn

[U33] Py：打包发布
来源：http://vd.shxzukj.cn

python -m build  （依赖 pyproject.toml）
来源：http://oy.panjiajie.cn

[U34] Py：判断编码
来源：http://rr.huanxung.cn

chardet.detect(raw)
来源：http://qy.colortex.cn

[U35] Py：发送邮件
来源：http://ty.9csxet.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xt.panjiajie.cn

[U36] Py：定时任务
来源：http://pn.jctech888.com.cn

schedule.every(10).minutes.do(job)
来源：http://nj.asd995.cn

[U37] Py：读写 Excel
来源：http://kb.jctech888.com.cn

pandas.read_excel / DataFrame.to_excel
来源：http://dn.hnjuh.cn

[U38] Py：获取脚本所在目录
来源：http://se.hnjuh.cn

Path(__file__).resolve().parent
来源：http://oy.chemitech.net.cn

[U39] Py：判断是否在交互环境
来源：http://ce.521024.cn

sys.stdout.isatty()
来源：http://yo.bjjhwx.cn

[U40] Py：打印到标准错误
来源：http://ep.panjiajie.cn

print("err", file=sys.stderr)
来源：http://ce.haigaiapp.cn

[U41] PHP：初始化 Composer 项目
来源：http://cw.nicolike.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ot.huixinmuqiang.cn

[U42] PHP：PSR-4 自动加载
来源：http://jd.yuexingan06.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tj.muxihuayi.cn

[U43] PHP：声明命名空间
来源：http://oz.chemitech.net.cn

namespace App\Http;
来源：http://kp.9csxet.cn

[U44] PHP：开启严格类型
来源：http://to.hnjuh.cn

declare(strict_types=1);
来源：http://lv.huixiangedu.cn

[U45] PHP：类型声明与返回类型
来源：http://ms.bookmarksfly.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://uz.asd995.cn

[U46] PHP：可空类型
来源：http://pn.9csxet.cn

?string $name = null
来源：http://ef.nszjky.cn

[U47] PHP：联合类型
来源：http://fc.newstarts.cn

int|string $id
来源：http://am.colortex.cn

[U48] PHP：纯枚举
来源：http://lj.nicolike.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xa.szsharing.cn

[U49] PHP：只读属性
来源：http://jz.wgjwhj.cn

public readonly string $name
来源：http://pt.muxihuayi.cn

[U50] PHP：构造器属性提升
来源：http://gr.lnxyls.cn

public function __construct(private int $id) {}
来源：http://xt.shxzskj.cn

[U51] PHP：数组解构
来源：http://ij.newstarts.cn

[$a, $b] = $arr;
来源：http://hz.hnjuh.cn

[U52] PHP：箭头函数
来源：http://oz.newstarts.cn

$double = fn($x) => $x * 2;
来源：http://cr.chemitech.net.cn

[U53] PHP：空合并运算符
来源：http://oa.bookmarksfly.cn

$v = $a ?? $b ?? "default";
来源：http://mt.bjjhwx.cn

[U54] PHP：空安全调用
来源：http://lg.szxytkj.cn

$obj?->method()
来源：http://fx.lnxyls.cn

[U55] PHP：match 表达式
来源：http://cl.bjjhwx.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gu.panjiajie.cn

[U56] PHP：命名参数
来源：http://wa.asd995.cn

f(a: 1, b: 2)
来源：http://rq.chemitech.net.cn

[U57] PHP：字符串插值
来源：http://sp.chemitech.net.cn

"值: {$a}"
来源：http://gn.yuntaijiaju.cn

[U58] PHP：数组三件套
来源：http://lk.chemitech.net.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fx.szxytkj.cn

[U59] PHP：自定义排序
来源：http://un.yuntaijiaju.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ey.newstarts.cn

[U60] PHP：JSON 编解码
来源：http://lv.lnxyls.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tg.hahajie.cn

[U61] PHP：正则
来源：http://ft.bjjhwx.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vc.haigaiapp.cn

[U62] PHP：日期对象
来源：http://pt.szsharing.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lf.newstarts.cn

[U63] PHP：文件读写
来源：http://jz.szsharing.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://cv.newstarts.cn

[U64] PHP：目录遍历
来源：http://er.jctech888.com.cn

glob("dir/*.php");  scandir("dir");
来源：http://iu.jianghongdianzi.cn

[U65] PHP：会话
来源：http://bs.muxihuayi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://oa.jctech888.com.cn

[U66] PHP：设置 Cookie
来源：http://kj.shxzukj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lq.colortex.cn

[U67] PHP：处理文件上传
来源：http://ox.asd995.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ik.huanxung.cn

[U68] PHP：PDO 连接
来源：http://ab.9csxet.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lo.haigaiapp.cn

[U69] PHP：PDO 预处理
来源：http://jj.yuexingan06.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rj.bjjhwx.cn

[U70] PHP：PDO 事务
来源：http://qy.muxihuayi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vy.nicolike.cn

[U71] PHP：抛出异常
来源：http://rq.newstarts.cn

throw new RuntimeException("失败", 500);
来源：http://xa.hahajie.cn

[U72] PHP：写错误日志
来源：http://ub.panjiajie.cn

error_log("失败: " . $e->getMessage());
来源：http://re.shxzskj.cn

[U73] PHP：读取 ini 配置
来源：http://oz.huixinmuqiang.cn

parse_ini_file("config.ini", true)
来源：http://hz.lnxyls.cn

[U74] PHP：读取环境变量
来源：http://yp.asd995.cn

getenv("APP_ENV") ?: "production"
来源：http://gd.szxytkj.cn

[U75] PHP：依赖注入
来源：http://jr.jianghongdianzi.cn

composer require psr/container
来源：http://ce.shxzskj.cn

[U76] PHP：简单路由
来源：http://bg.huixiangedu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://op.huanxung.cn

[U77] PHP：模板渲染
来源：http://xz.szsharing.cn

composer require twig/twig
来源：http://kn.shtwfgs.cn

[U78] PHP：单元测试
来源：http://zn.panjiajie.cn

composer require --dev phpunit/phpunit
来源：http://am.shxzskj.cn

[U79] PHP：静态分析
来源：http://os.hahajie.cn

composer require --dev phpstan/phpstan
来源：http://qh.nszjky.cn

[U80] PHP：代码规范修复
来源：http://lw.panjiajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://rj.nicolike.cn

[U81] JS：初始化项目
来源：http://ue.shxzskj.cn

npm init -y;  npm i express
来源：http://se.wgjwhj.cn

[U82] JS：package.json 脚本
来源：http://wc.chemitech.net.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cs.lnxyls.cn

[U83] JS：ES Module 导入导出
来源：http://wf.newstarts.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ar.gzmigu.cn

[U84] JS：CommonJS 写法
来源：http://ry.lnxyls.cn

module.exports = { a };  const { a } = require("./m");
来源：http://tr.huixiangedu.cn

[U85] JS：可选链
来源：http://ry.newstarts.cn

a?.b?.c
来源：http://ua.bookmarksfly.cn

[U86] JS：空值合并
来源：http://zn.szxytkj.cn

a ?? b
来源：http://eb.asd995.cn

[U87] JS：解构默认值
来源：http://kk.shxzukj.cn

const { a = 1, b = 2 } = obj;
来源：http://kz.muxihuayi.cn

[U88] JS：对象展开合并
来源：http://rl.nszjky.cn

{ ...a, ...b }
来源：http://nw.szxytkj.cn

[U89] JS：数组去重
来源：http://jx.asd995.cn

[...new Set(arr)]
来源：http://xr.muxihuayi.cn

[U90] JS：数字数组排序
来源：http://pt.huanxung.cn

[...arr].sort((a, b) => a - b)
来源：http://mw.chemitech.net.cn

[U91] JS：对象键值遍历
来源：http://gk.newstarts.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pd.haigaiapp.cn

[U92] JS：深拷贝
来源：http://xt.shxzukj.cn

structuredClone(obj)
来源：http://tm.lnxyls.cn

[U93] JS：模板字符串
来源：http://fc.asd995.cn

`共 ${n} 条`
来源：http://lz.huixiangedu.cn

[U94] JS：箭头函数
来源：http://pu.szxytkj.cn

const double = x => x * 2;
来源：http://yf.muxihuayi.cn

[U95] JS：Promise 包装
来源：http://kw.wgjwhj.cn

new Promise((resolve, reject) => {})
来源：http://oz.muxihuayi.cn

[U96] JS：async/await 与异常
来源：http://iq.huixinmuqiang.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://in.9csxet.cn

[U97] JS：并发请求
来源：http://xp.newstarts.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://pd.panjiajie.cn

[U98] JS：fetch 带 JSON
来源：http://nt.shxzskj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fj.huixinmuqiang.cn

[U99] JS：事件监听
来源：http://jr.asd995.cn

el.addEventListener("click", e => {})
来源：http://ut.nicolike.cn

[U100] JS：DOM 查询
来源：http://ve.jianghongdianzi.cn

document.querySelector(".item")
来源：http://tu.newstarts.cn

[U101] JS：classList 操作
来源：http://wv.hahajie.cn

el.classList.toggle("active")
来源：http://rg.chemitech.net.cn

[U102] JS：本地存储
来源：http://nb.gzmigu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://qn.yuexingan06.cn

[U103] JS：定时器
来源：http://dr.yuntaijiaju.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kr.bjjhwx.cn

[U104] JS：防抖
来源：http://va.panjiajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ib.yuntaijiaju.cn

[U105] JS：节流
来源：http://pe.wgjwhj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ae.shxzukj.cn

[U106] JS：日期格式化
来源：http://tg.jctech888.com.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bt.hnjuh.cn

[U107] JS：数字千分位
来源：http://fh.shxzskj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qj.panjiajie.cn

[U108] JS：随机整数
来源：http://ek.nicolike.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dh.bjjhwx.cn

[U109] JS：数组分组
来源：http://qp.nszjky.cn

Object.groupBy(arr, x => x.type)
来源：http://qp.haigaiapp.cn

[U110] JS：数组分块
来源：http://sa.bjjhwx.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://uw.colortex.cn

[U111] JS：对象转 Map
来源：http://ix.nszjky.cn

new Map(Object.entries(obj))
来源：http://dh.shxzukj.cn

[U112] JS：字符串补位
来源：http://mh.nicolike.cn

"7".padStart(3, "0")
来源：http://nd.gzmigu.cn

[U113] JS：正则替换全部
来源：http://qw.hnjuh.cn

s.replaceAll("a", "b")
来源：http://pq.bookmarksfly.cn

[U114] JS：JSON 深比较
来源：http://fn.nicolike.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://et.haigaiapp.cn

[U115] JS：生成 UUID
来源：http://ar.nicolike.cn

crypto.randomUUID()
来源：http://ku.hahajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://xi.shxzskj.cn

/** @param {string} name */ function f(name) {}
来源：http://zt.shxzukj.cn

[U117] JS：单元测试
来源：http://dy.huixinmuqiang.cn

npm i -D vitest;  npx vitest
来源：http://pn.huanxung.cn

[U118] JS：开发服务器
来源：http://sp.yuexingan06.cn

npm i -D vite;  npx vite
来源：http://sg.shtwfgs.cn

[U119] JS：生产构建
来源：http://vp.huanxung.cn

npx vite build
来源：http://ct.asd995.cn

[U120] JS：读取环境变量（Vite）
来源：http://sc.9csxet.cn

import.meta.env.VITE_API_URL
来源：http://wj.nszjky.cn

================================================================================
来源：http://kk.shtwfgs.cn

统计汇总
来源：http://fe.shtwfgs.cn

================================================================================
来源：http://cf.bjjhwx.cn

按语言统计（条）：
来源：http://yg.colortex.cn

Python ......... 252
来源：http://wj.szsharing.cn

PHP ............ 252
来源：http://ug.hnjuh.cn

JavaScript ..... 252
来源：http://ye.chemitech.net.cn

TypeScript ..... 212
来源：http://oe.huixiangedu.cn

Java ........... 212
来源：http://mf.colortex.cn

Go ............. 212
来源：http://cc.9csxet.cn

Ruby ........... 212
来源：http://cs.muxihuayi.cn

C# ............. 212
来源：http://jr.panjiajie.cn

C .............. 30
来源：http://gk.nicolike.cn

C++ ............ 30
来源：http://rr.newstarts.cn

SQL ............ 90
来源：http://fq.gzmigu.cn

Bash ........... 80
来源：http://zm.521024.cn

Kotlin ......... 15
来源：http://we.newstarts.cn

Swift .......... 15
来源：http://gw.shxzskj.cn

Lua ............ 10
来源：http://wx.bookmarksfly.cn

Perl ........... 10
来源：http://ta.yuexingan06.cn

Scala .......... 10
来源：http://rf.huanxung.cn

------------------------------------
来源：http://mp.asd995.cn

合计 ........... 2106 条
来源：http://ac.bookmarksfly.cn

按章节统计：
来源：http://bk.521024.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ws.szxytkj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://sf.yuexingan06.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fl.newstarts.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fy.huixiangedu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://sb.newstarts.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://us.panjiajie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ml.521024.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wx.haigaiapp.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hg.jctech888.com.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://px.panjiajie.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bj.chemitech.net.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dn.colortex.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ox.colortex.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kw.9csxet.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wv.newstarts.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mq.gzmigu.cn

Q SQL 专题                              90
来源：http://ix.jianghongdianzi.cn

R Bash 专题                             80
来源：http://wa.panjiajie.cn

S C / C++ 专题                          60
来源：http://nd.colortex.cn

T 其他语言补充                          60
来源：http://iv.szsharing.cn

U 高频实用片段                         120
来源：http://ql.bjjhwx.cn

------------------------------------
来源：http://ry.asd995.cn

合计                                  2106 条
来源：http://tk.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://hg.shtwfgs.cn

使用提醒
来源：http://ga.nszjky.cn

--------------------------------------------------------------------------------
来源：http://hm.szxytkj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tc.shxzskj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dq.huixinmuqiang.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://sw.yuexingan06.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://jd.colortex.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://aw.gzmigu.cn

—— 文件结束 ——
来源：http://lc.shxzukj.cn

================================================================================
来源：http://mi.shxzskj.cn

程序语言常见例子速查手册（2024 版）
来源：http://oo.newstarts.cn

Common Programming Examples Cheat Book
来源：http://sl.newstarts.cn

================================================================================
来源：http://cq.521024.cn

【收录内容】
来源：http://ll.hahajie.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://im.nicolike.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hc.asd995.cn

SQL · Bash · C · C++
来源：http://jv.shtwfgs.cn


<!-- 参考信息 -->