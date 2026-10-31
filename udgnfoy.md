代发 wailian999

[U03] Py：加载 .env 配置
来源：http://ou.nicolike.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ba.muxihuayi.cn

[U04] Py：变量调试打印
来源：http://nj.muxihuayi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://uo.colortex.cn

[U05] Py：列表去重且保序
来源：http://it.chemitech.net.cn

list(dict.fromkeys(arr))
来源：http://cr.chemitech.net.cn

[U06] Py：合并两个字典
来源：http://ic.panjiajie.cn

{**a, **b}
来源：http://ay.yuntaijiaju.cn

[U07] Py：反转字典键值
来源：http://vw.huanxung.cn

{v: k for k, v in d.items()}
来源：http://en.newstarts.cn

[U08] Py：展平二维列表
来源：http://ta.jctech888.com.cn

[y for x in nested for y in x]
来源：http://ls.wgjwhj.cn

[U09] Py：字典取最大值的键
来源：http://lr.nicolike.cn

max(d, key=d.get)
来源：http://ih.hahajie.cn

[U10] Py：按值排序字典
来源：http://au.yuexingan06.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ve.521024.cn

[U11] Py：生成器表达式
来源：http://mx.gzmigu.cn

(x * 2 for x in arr)
来源：http://vw.asd995.cn

[U12] Py：取出现最多的 3 个元素
来源：http://jv.newstarts.cn

Counter(arr).most_common(3)
来源：http://cy.jianghongdianzi.cn

[U13] Py：固定长度队列
来源：http://xr.hahajie.cn

deque(maxlen=10)
来源：http://cx.hahajie.cn

[U14] Py：分组收集到列表
来源：http://hb.9csxet.cn

defaultdict(list)
来源：http://bf.szxytkj.cn

[U15] Py：高精度计时
来源：http://pm.huixinmuqiang.cn

t = time.perf_counter()
来源：http://gl.hahajie.cn

[U16] Py：命令行参数解析
来源：http://nk.newstarts.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cb.yuexingan06.cn

[U17] Py：初始化日志
来源：http://fx.yuntaijiaju.cn

logging.basicConfig(level=logging.INFO)
来源：http://pp.jianghongdianzi.cn

[U18] Py：预编译正则
来源：http://iz.haigaiapp.cn

pat = re.compile(r"\d+")
来源：http://qo.szxytkj.cn

[U19] Py：正则替换带回调
来源：http://lv.521024.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cf.huixiangedu.cn

[U20] Py：缓存函数结果
来源：http://wo.hnjuh.cn

@functools.lru_cache(maxsize=None)
来源：http://ib.panjiajie.cn

[U21] Py：自定义上下文管理器
来源：http://ny.colortex.cn

@contextlib.contextmanager
来源：http://my.yuexingan06.cn

[U22] Py：矩阵转置
来源：http://in.huixiangedu.cn

list(zip(*m))
来源：http://rt.huixiangedu.cn

[U23] Py：分块读取大文件
来源：http://cl.shxzskj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zo.szsharing.cn

[U24] Py：路径操作
来源：http://iw.521024.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zb.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://xh.panjiajie.cn

csv.DictReader(f)
来源：http://dz.521024.cn

[U26] Py：并发下载
来源：http://bk.szsharing.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://as.bjjhwx.cn

[U27] Py：异步 HTTP
来源：http://ce.bjjhwx.cn

aiohttp.ClientSession() 配合 async with
来源：http://pl.jctech888.com.cn

[U28] Py：类型别名
来源：http://xp.9csxet.cn

UserId = int
来源：http://pn.hnjuh.cn

[U29] Py：属性校验
来源：http://zz.huixinmuqiang.cn

@property 与 @x.setter 配合
来源：http://zy.lnxyls.cn

[U30] Py：数据类
来源：http://fa.bookmarksfly.cn

@dataclass(slots=True)
来源：http://iq.shtwfgs.cn

[U31] Py：单测
来源：http://ur.panjiajie.cn

python -m pytest -q
来源：http://gg.asd995.cn

[U32] Py：代码格式化
来源：http://up.haigaiapp.cn

ruff format . && ruff check --fix .
来源：http://cc.521024.cn

[U33] Py：打包发布
来源：http://jv.panjiajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://kk.521024.cn

[U34] Py：判断编码
来源：http://ly.muxihuayi.cn

chardet.detect(raw)
来源：http://ma.chemitech.net.cn

[U35] Py：发送邮件
来源：http://ut.nszjky.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yh.shtwfgs.cn

[U36] Py：定时任务
来源：http://lw.nicolike.cn

schedule.every(10).minutes.do(job)
来源：http://co.yuntaijiaju.cn

[U37] Py：读写 Excel
来源：http://za.szsharing.cn

pandas.read_excel / DataFrame.to_excel
来源：http://gn.chemitech.net.cn

[U38] Py：获取脚本所在目录
来源：http://es.9csxet.cn

Path(__file__).resolve().parent
来源：http://zw.muxihuayi.cn

[U39] Py：判断是否在交互环境
来源：http://ff.szxytkj.cn

sys.stdout.isatty()
来源：http://ve.chemitech.net.cn

[U40] Py：打印到标准错误
来源：http://ep.asd995.cn

print("err", file=sys.stderr)
来源：http://pn.asd995.cn

[U41] PHP：初始化 Composer 项目
来源：http://wr.9csxet.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gz.nicolike.cn

[U42] PHP：PSR-4 自动加载
来源：http://in.panjiajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wy.wgjwhj.cn

[U43] PHP：声明命名空间
来源：http://pt.haigaiapp.cn

namespace App\Http;
来源：http://jp.bjjhwx.cn

[U44] PHP：开启严格类型
来源：http://vy.wgjwhj.cn

declare(strict_types=1);
来源：http://jb.newstarts.cn

[U45] PHP：类型声明与返回类型
来源：http://jk.chemitech.net.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ud.asd995.cn

[U46] PHP：可空类型
来源：http://cb.newstarts.cn

?string $name = null
来源：http://jh.hahajie.cn

[U47] PHP：联合类型
来源：http://af.shxzskj.cn

int|string $id
来源：http://ad.nicolike.cn

[U48] PHP：纯枚举
来源：http://wl.9csxet.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tc.colortex.cn

[U49] PHP：只读属性
来源：http://xd.chemitech.net.cn

public readonly string $name
来源：http://pt.szxytkj.cn

[U50] PHP：构造器属性提升
来源：http://ux.szsharing.cn

public function __construct(private int $id) {}
来源：http://fs.bookmarksfly.cn

[U51] PHP：数组解构
来源：http://dx.nicolike.cn

[$a, $b] = $arr;
来源：http://fp.yuexingan06.cn

[U52] PHP：箭头函数
来源：http://qe.colortex.cn

$double = fn($x) => $x * 2;
来源：http://jk.hahajie.cn

[U53] PHP：空合并运算符
来源：http://ua.haigaiapp.cn

$v = $a ?? $b ?? "default";
来源：http://or.hahajie.cn

[U54] PHP：空安全调用
来源：http://zr.lnxyls.cn

$obj?->method()
来源：http://vp.huixinmuqiang.cn

[U55] PHP：match 表达式
来源：http://ml.gzmigu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xf.yuntaijiaju.cn

[U56] PHP：命名参数
来源：http://fn.nszjky.cn

f(a: 1, b: 2)
来源：http://ie.9csxet.cn

[U57] PHP：字符串插值
来源：http://oh.shtwfgs.cn

"值: {$a}"
来源：http://be.chemitech.net.cn

[U58] PHP：数组三件套
来源：http://fp.shxzukj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fh.panjiajie.cn

[U59] PHP：自定义排序
来源：http://vm.jctech888.com.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ea.nicolike.cn

[U60] PHP：JSON 编解码
来源：http://wi.huixinmuqiang.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fi.nszjky.cn

[U61] PHP：正则
来源：http://od.hnjuh.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ln.haigaiapp.cn

[U62] PHP：日期对象
来源：http://qn.bookmarksfly.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://su.hnjuh.cn

[U63] PHP：文件读写
来源：http://ab.muxihuayi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ph.yuntaijiaju.cn

[U64] PHP：目录遍历
来源：http://kd.huanxung.cn

glob("dir/*.php");  scandir("dir");
来源：http://vr.muxihuayi.cn

[U65] PHP：会话
来源：http://ru.huixinmuqiang.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://db.haigaiapp.cn

[U66] PHP：设置 Cookie
来源：http://mp.chemitech.net.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://uz.bookmarksfly.cn

[U67] PHP：处理文件上传
来源：http://ux.asd995.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ju.shxzukj.cn

[U68] PHP：PDO 连接
来源：http://rc.yuntaijiaju.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ph.yuntaijiaju.cn

[U69] PHP：PDO 预处理
来源：http://ni.gzmigu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://uw.lnxyls.cn

[U70] PHP：PDO 事务
来源：http://im.muxihuayi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://il.huixinmuqiang.cn

[U71] PHP：抛出异常
来源：http://ur.nicolike.cn

throw new RuntimeException("失败", 500);
来源：http://qi.shtwfgs.cn

[U72] PHP：写错误日志
来源：http://ip.nicolike.cn

error_log("失败: " . $e->getMessage());
来源：http://mp.asd995.cn

[U73] PHP：读取 ini 配置
来源：http://vo.panjiajie.cn

parse_ini_file("config.ini", true)
来源：http://oa.gzmigu.cn

[U74] PHP：读取环境变量
来源：http://kw.9csxet.cn

getenv("APP_ENV") ?: "production"
来源：http://kk.jctech888.com.cn

[U75] PHP：依赖注入
来源：http://ty.yuntaijiaju.cn

composer require psr/container
来源：http://yx.huanxung.cn

[U76] PHP：简单路由
来源：http://mg.szsharing.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vg.wgjwhj.cn

[U77] PHP：模板渲染
来源：http://ka.bookmarksfly.cn

composer require twig/twig
来源：http://uj.shxzukj.cn

[U78] PHP：单元测试
来源：http://ur.yuntaijiaju.cn

composer require --dev phpunit/phpunit
来源：http://gf.nicolike.cn

[U79] PHP：静态分析
来源：http://mn.nicolike.cn

composer require --dev phpstan/phpstan
来源：http://nh.newstarts.cn

[U80] PHP：代码规范修复
来源：http://ct.hahajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ib.colortex.cn

[U81] JS：初始化项目
来源：http://xf.jctech888.com.cn

npm init -y;  npm i express
来源：http://wi.panjiajie.cn

[U82] JS：package.json 脚本
来源：http://ok.gzmigu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ku.yuexingan06.cn

[U83] JS：ES Module 导入导出
来源：http://xt.asd995.cn

export const a = 1;  import { a } from "./m.js";
来源：http://dr.huixiangedu.cn

[U84] JS：CommonJS 写法
来源：http://hc.bjjhwx.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wa.521024.cn

[U85] JS：可选链
来源：http://ev.huixiangedu.cn

a?.b?.c
来源：http://en.jianghongdianzi.cn

[U86] JS：空值合并
来源：http://fd.9csxet.cn

a ?? b
来源：http://wr.wgjwhj.cn

[U87] JS：解构默认值
来源：http://xn.nszjky.cn

const { a = 1, b = 2 } = obj;
来源：http://iu.colortex.cn

[U88] JS：对象展开合并
来源：http://uk.haigaiapp.cn

{ ...a, ...b }
来源：http://wj.yuexingan06.cn

[U89] JS：数组去重
来源：http://rq.hahajie.cn

[...new Set(arr)]
来源：http://lh.jianghongdianzi.cn

[U90] JS：数字数组排序
来源：http://pg.gzmigu.cn

[...arr].sort((a, b) => a - b)
来源：http://qo.colortex.cn

[U91] JS：对象键值遍历
来源：http://ec.wgjwhj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cg.haigaiapp.cn

[U92] JS：深拷贝
来源：http://wv.jctech888.com.cn

structuredClone(obj)
来源：http://ei.huixinmuqiang.cn

[U93] JS：模板字符串
来源：http://qe.huixiangedu.cn

`共 ${n} 条`
来源：http://gd.panjiajie.cn

[U94] JS：箭头函数
来源：http://ic.shxzskj.cn

const double = x => x * 2;
来源：http://br.shxzukj.cn

[U95] JS：Promise 包装
来源：http://wj.shxzukj.cn

new Promise((resolve, reject) => {})
来源：http://dv.shtwfgs.cn

[U96] JS：async/await 与异常
来源：http://up.huanxung.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ig.jianghongdianzi.cn

[U97] JS：并发请求
来源：http://xg.yuexingan06.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://es.lnxyls.cn

[U98] JS：fetch 带 JSON
来源：http://bs.hnjuh.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kz.hahajie.cn

[U99] JS：事件监听
来源：http://rp.hahajie.cn

el.addEventListener("click", e => {})
来源：http://zy.shxzukj.cn

[U100] JS：DOM 查询
来源：http://ie.hahajie.cn

document.querySelector(".item")
来源：http://ks.yuntaijiaju.cn

[U101] JS：classList 操作
来源：http://tj.yuntaijiaju.cn

el.classList.toggle("active")
来源：http://he.shxzskj.cn

[U102] JS：本地存储
来源：http://yy.jianghongdianzi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://qr.bjjhwx.cn

[U103] JS：定时器
来源：http://hg.wgjwhj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ls.huixinmuqiang.cn

[U104] JS：防抖
来源：http://at.jctech888.com.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pz.9csxet.cn

[U105] JS：节流
来源：http://cd.jctech888.com.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zi.hahajie.cn

[U106] JS：日期格式化
来源：http://vm.huixinmuqiang.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wy.lnxyls.cn

[U107] JS：数字千分位
来源：http://vd.asd995.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ea.shxzukj.cn

[U108] JS：随机整数
来源：http://au.wgjwhj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tu.chemitech.net.cn

[U109] JS：数组分组
来源：http://yh.shtwfgs.cn

Object.groupBy(arr, x => x.type)
来源：http://ur.521024.cn

[U110] JS：数组分块
来源：http://fr.huanxung.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kg.bookmarksfly.cn

[U111] JS：对象转 Map
来源：http://rr.shxzukj.cn

new Map(Object.entries(obj))
来源：http://ao.yuexingan06.cn

[U112] JS：字符串补位
来源：http://oq.bjjhwx.cn

"7".padStart(3, "0")
来源：http://td.nszjky.cn

[U113] JS：正则替换全部
来源：http://lb.newstarts.cn

s.replaceAll("a", "b")
来源：http://fv.newstarts.cn

[U114] JS：JSON 深比较
来源：http://sc.yuntaijiaju.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ub.shxzskj.cn

[U115] JS：生成 UUID
来源：http://yt.chemitech.net.cn

crypto.randomUUID()
来源：http://mj.panjiajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://na.huixinmuqiang.cn

/** @param {string} name */ function f(name) {}
来源：http://jj.jianghongdianzi.cn

[U117] JS：单元测试
来源：http://ws.bookmarksfly.cn

npm i -D vitest;  npx vitest
来源：http://ex.muxihuayi.cn

[U118] JS：开发服务器
来源：http://nw.colortex.cn

npm i -D vite;  npx vite
来源：http://ct.shxzskj.cn

[U119] JS：生产构建
来源：http://ke.lnxyls.cn

npx vite build
来源：http://ka.huixinmuqiang.cn

[U120] JS：读取环境变量（Vite）
来源：http://mu.shtwfgs.cn

import.meta.env.VITE_API_URL
来源：http://cq.lnxyls.cn

================================================================================
来源：http://gy.szxytkj.cn

统计汇总
来源：http://ha.jianghongdianzi.cn

================================================================================
来源：http://ya.shtwfgs.cn

按语言统计（条）：
来源：http://qa.jianghongdianzi.cn

Python ......... 252
来源：http://ku.panjiajie.cn

PHP ............ 252
来源：http://oz.yuexingan06.cn

JavaScript ..... 252
来源：http://kx.shxzskj.cn

TypeScript ..... 212
来源：http://yj.szsharing.cn

Java ........... 212
来源：http://ve.521024.cn

Go ............. 212
来源：http://ad.lnxyls.cn

Ruby ........... 212
来源：http://wf.gzmigu.cn

C# ............. 212
来源：http://yz.newstarts.cn

C .............. 30
来源：http://ov.yuntaijiaju.cn

C++ ............ 30
来源：http://bd.lnxyls.cn

SQL ............ 90
来源：http://gw.shtwfgs.cn

Bash ........... 80
来源：http://so.haigaiapp.cn

Kotlin ......... 15
来源：http://bi.bookmarksfly.cn

Swift .......... 15
来源：http://fq.szxytkj.cn

Lua ............ 10
来源：http://br.szsharing.cn

Perl ........... 10
来源：http://iu.gzmigu.cn

Scala .......... 10
来源：http://bm.asd995.cn

------------------------------------
来源：http://uy.nicolike.cn

合计 ........... 2106 条
来源：http://tf.nszjky.cn

按章节统计：
来源：http://az.asd995.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://pf.jctech888.com.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://es.bookmarksfly.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ox.lnxyls.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ca.asd995.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ki.jianghongdianzi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qi.nicolike.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pd.shtwfgs.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fg.yuntaijiaju.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://di.haigaiapp.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nr.chemitech.net.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kg.jianghongdianzi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fw.huixinmuqiang.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://li.colortex.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zq.asd995.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rh.wgjwhj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qz.bookmarksfly.cn

Q SQL 专题                              90
来源：http://yx.wgjwhj.cn

R Bash 专题                             80
来源：http://hw.szxytkj.cn

S C / C++ 专题                          60
来源：http://pu.szxytkj.cn

T 其他语言补充                          60
来源：http://iv.nszjky.cn

U 高频实用片段                         120
来源：http://rp.chemitech.net.cn

------------------------------------
来源：http://ia.shtwfgs.cn

合计                                  2106 条
来源：http://ow.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://iy.jianghongdianzi.cn

使用提醒
来源：http://xy.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://ph.shtwfgs.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fh.bjjhwx.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gy.bjjhwx.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ia.colortex.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ov.panjiajie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://oa.hahajie.cn

—— 文件结束 ——
来源：http://zz.hahajie.cn

================================================================================
来源：http://lu.huixiangedu.cn

程序语言常见例子速查手册（2024 版）
来源：http://xu.hnjuh.cn

Common Programming Examples Cheat Book
来源：http://up.chemitech.net.cn

================================================================================
来源：http://vh.yuexingan06.cn

【收录内容】
来源：http://lq.521024.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ph.bookmarksfly.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://yg.haigaiapp.cn

SQL · Bash · C · C++
来源：http://di.huixinmuqiang.cn


<!-- 参考信息 -->