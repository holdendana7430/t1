代发 wailian999

[U07] Py：反转字典键值
来源：http://oo.panjiajie.cn

{v: k for k, v in d.items()}
来源：http://yl.muxihuayi.cn

[U08] Py：展平二维列表
来源：http://em.9csxet.cn

[y for x in nested for y in x]
来源：http://so.9csxet.cn

[U09] Py：字典取最大值的键
来源：http://hw.jianghongdianzi.cn

max(d, key=d.get)
来源：http://an.yuexingan06.cn

[U10] Py：按值排序字典
来源：http://sm.jianghongdianzi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yn.521024.cn

[U11] Py：生成器表达式
来源：http://mn.panjiajie.cn

(x * 2 for x in arr)
来源：http://fm.jctech888.com.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ue.muxihuayi.cn

Counter(arr).most_common(3)
来源：http://mc.hahajie.cn

[U13] Py：固定长度队列
来源：http://us.nszjky.cn

deque(maxlen=10)
来源：http://tu.9csxet.cn

[U14] Py：分组收集到列表
来源：http://pt.hahajie.cn

defaultdict(list)
来源：http://ye.shtwfgs.cn

[U15] Py：高精度计时
来源：http://xi.yuntaijiaju.cn

t = time.perf_counter()
来源：http://zu.hahajie.cn

[U16] Py：命令行参数解析
来源：http://rs.nszjky.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fx.nszjky.cn

[U17] Py：初始化日志
来源：http://lz.panjiajie.cn

logging.basicConfig(level=logging.INFO)
来源：http://tn.huanxung.cn

[U18] Py：预编译正则
来源：http://tb.huixinmuqiang.cn

pat = re.compile(r"\d+")
来源：http://is.nszjky.cn

[U19] Py：正则替换带回调
来源：http://rc.wgjwhj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cr.huanxung.cn

[U20] Py：缓存函数结果
来源：http://vo.asd995.cn

@functools.lru_cache(maxsize=None)
来源：http://jy.nicolike.cn

[U21] Py：自定义上下文管理器
来源：http://fk.szsharing.cn

@contextlib.contextmanager
来源：http://zp.shxzukj.cn

[U22] Py：矩阵转置
来源：http://fo.bookmarksfly.cn

list(zip(*m))
来源：http://cv.szxytkj.cn

[U23] Py：分块读取大文件
来源：http://wr.lnxyls.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cf.jctech888.com.cn

[U24] Py：路径操作
来源：http://ui.bookmarksfly.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jm.muxihuayi.cn

[U25] Py：CSV 按字典读
来源：http://cu.huixinmuqiang.cn

csv.DictReader(f)
来源：http://fl.szxytkj.cn

[U26] Py：并发下载
来源：http://my.muxihuayi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fk.nszjky.cn

[U27] Py：异步 HTTP
来源：http://xr.9csxet.cn

aiohttp.ClientSession() 配合 async with
来源：http://un.9csxet.cn

[U28] Py：类型别名
来源：http://tb.521024.cn

UserId = int
来源：http://gs.newstarts.cn

[U29] Py：属性校验
来源：http://tp.jianghongdianzi.cn

@property 与 @x.setter 配合
来源：http://bf.newstarts.cn

[U30] Py：数据类
来源：http://pt.muxihuayi.cn

@dataclass(slots=True)
来源：http://gw.newstarts.cn

[U31] Py：单测
来源：http://vw.hahajie.cn

python -m pytest -q
来源：http://sr.hnjuh.cn

[U32] Py：代码格式化
来源：http://zo.asd995.cn

ruff format . && ruff check --fix .
来源：http://aq.colortex.cn

[U33] Py：打包发布
来源：http://we.chemitech.net.cn

python -m build  （依赖 pyproject.toml）
来源：http://fp.muxihuayi.cn

[U34] Py：判断编码
来源：http://kn.szxytkj.cn

chardet.detect(raw)
来源：http://bs.bjjhwx.cn

[U35] Py：发送邮件
来源：http://ae.jctech888.com.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://uu.nszjky.cn

[U36] Py：定时任务
来源：http://ja.haigaiapp.cn

schedule.every(10).minutes.do(job)
来源：http://fm.huixinmuqiang.cn

[U37] Py：读写 Excel
来源：http://in.wgjwhj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ti.nicolike.cn

[U38] Py：获取脚本所在目录
来源：http://jl.szxytkj.cn

Path(__file__).resolve().parent
来源：http://pl.nszjky.cn

[U39] Py：判断是否在交互环境
来源：http://ls.shxzskj.cn

sys.stdout.isatty()
来源：http://qr.shxzskj.cn

[U40] Py：打印到标准错误
来源：http://si.shtwfgs.cn

print("err", file=sys.stderr)
来源：http://qb.shtwfgs.cn

[U41] PHP：初始化 Composer 项目
来源：http://xr.bookmarksfly.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xz.szxytkj.cn

[U42] PHP：PSR-4 自动加载
来源：http://dx.521024.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yq.nicolike.cn

[U43] PHP：声明命名空间
来源：http://ze.chemitech.net.cn

namespace App\Http;
来源：http://tz.huixiangedu.cn

[U44] PHP：开启严格类型
来源：http://nt.gzmigu.cn

declare(strict_types=1);
来源：http://nw.newstarts.cn

[U45] PHP：类型声明与返回类型
来源：http://yl.szsharing.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bu.shtwfgs.cn

[U46] PHP：可空类型
来源：http://xx.shxzukj.cn

?string $name = null
来源：http://yq.9csxet.cn

[U47] PHP：联合类型
来源：http://gi.muxihuayi.cn

int|string $id
来源：http://mf.haigaiapp.cn

[U48] PHP：纯枚举
来源：http://qi.bjjhwx.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zj.asd995.cn

[U49] PHP：只读属性
来源：http://mn.muxihuayi.cn

public readonly string $name
来源：http://ks.bjjhwx.cn

[U50] PHP：构造器属性提升
来源：http://yw.muxihuayi.cn

public function __construct(private int $id) {}
来源：http://ci.shtwfgs.cn

[U51] PHP：数组解构
来源：http://jj.521024.cn

[$a, $b] = $arr;
来源：http://hg.szxytkj.cn

[U52] PHP：箭头函数
来源：http://ov.yuntaijiaju.cn

$double = fn($x) => $x * 2;
来源：http://tq.muxihuayi.cn

[U53] PHP：空合并运算符
来源：http://kj.shtwfgs.cn

$v = $a ?? $b ?? "default";
来源：http://rd.chemitech.net.cn

[U54] PHP：空安全调用
来源：http://do.chemitech.net.cn

$obj?->method()
来源：http://rm.yuexingan06.cn

[U55] PHP：match 表达式
来源：http://sp.huixiangedu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lt.asd995.cn

[U56] PHP：命名参数
来源：http://ww.nicolike.cn

f(a: 1, b: 2)
来源：http://ta.hnjuh.cn

[U57] PHP：字符串插值
来源：http://tj.521024.cn

"值: {$a}"
来源：http://ao.jctech888.com.cn

[U58] PHP：数组三件套
来源：http://oh.lnxyls.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cl.lnxyls.cn

[U59] PHP：自定义排序
来源：http://rp.huanxung.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ug.shxzukj.cn

[U60] PHP：JSON 编解码
来源：http://qz.szsharing.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://oy.hnjuh.cn

[U61] PHP：正则
来源：http://nv.9csxet.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hm.hahajie.cn

[U62] PHP：日期对象
来源：http://pa.bjjhwx.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ns.shxzskj.cn

[U63] PHP：文件读写
来源：http://hc.hnjuh.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jw.muxihuayi.cn

[U64] PHP：目录遍历
来源：http://oo.shxzukj.cn

glob("dir/*.php");  scandir("dir");
来源：http://kz.haigaiapp.cn

[U65] PHP：会话
来源：http://ez.huixiangedu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ci.huixiangedu.cn

[U66] PHP：设置 Cookie
来源：http://dv.yuntaijiaju.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ps.lnxyls.cn

[U67] PHP：处理文件上传
来源：http://ff.huanxung.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xt.hnjuh.cn

[U68] PHP：PDO 连接
来源：http://kc.9csxet.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://oh.nicolike.cn

[U69] PHP：PDO 预处理
来源：http://sv.9csxet.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ds.huixinmuqiang.cn

[U70] PHP：PDO 事务
来源：http://vg.jctech888.com.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vi.haigaiapp.cn

[U71] PHP：抛出异常
来源：http://bg.newstarts.cn

throw new RuntimeException("失败", 500);
来源：http://ko.bjjhwx.cn

[U72] PHP：写错误日志
来源：http://vy.yuntaijiaju.cn

error_log("失败: " . $e->getMessage());
来源：http://ds.gzmigu.cn

[U73] PHP：读取 ini 配置
来源：http://qb.colortex.cn

parse_ini_file("config.ini", true)
来源：http://pv.muxihuayi.cn

[U74] PHP：读取环境变量
来源：http://ll.shtwfgs.cn

getenv("APP_ENV") ?: "production"
来源：http://dw.nszjky.cn

[U75] PHP：依赖注入
来源：http://eg.shxzskj.cn

composer require psr/container
来源：http://qs.nszjky.cn

[U76] PHP：简单路由
来源：http://yt.bookmarksfly.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dg.newstarts.cn

[U77] PHP：模板渲染
来源：http://up.huanxung.cn

composer require twig/twig
来源：http://ia.chemitech.net.cn

[U78] PHP：单元测试
来源：http://oz.szsharing.cn

composer require --dev phpunit/phpunit
来源：http://wc.szsharing.cn

[U79] PHP：静态分析
来源：http://ig.asd995.cn

composer require --dev phpstan/phpstan
来源：http://xz.muxihuayi.cn

[U80] PHP：代码规范修复
来源：http://yn.panjiajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://fx.haigaiapp.cn

[U81] JS：初始化项目
来源：http://cv.wgjwhj.cn

npm init -y;  npm i express
来源：http://ez.huixinmuqiang.cn

[U82] JS：package.json 脚本
来源：http://az.nicolike.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://iv.hnjuh.cn

[U83] JS：ES Module 导入导出
来源：http://nb.wgjwhj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://yz.9csxet.cn

[U84] JS：CommonJS 写法
来源：http://ii.nszjky.cn

module.exports = { a };  const { a } = require("./m");
来源：http://fi.szxytkj.cn

[U85] JS：可选链
来源：http://py.colortex.cn

a?.b?.c
来源：http://kh.muxihuayi.cn

[U86] JS：空值合并
来源：http://kk.shxzskj.cn

a ?? b
来源：http://zq.shxzukj.cn

[U87] JS：解构默认值
来源：http://co.gzmigu.cn

const { a = 1, b = 2 } = obj;
来源：http://ui.521024.cn

[U88] JS：对象展开合并
来源：http://lj.hahajie.cn

{ ...a, ...b }
来源：http://ck.huixiangedu.cn

[U89] JS：数组去重
来源：http://dl.huanxung.cn

[...new Set(arr)]
来源：http://ni.asd995.cn

[U90] JS：数字数组排序
来源：http://vk.gzmigu.cn

[...arr].sort((a, b) => a - b)
来源：http://bl.shxzskj.cn

[U91] JS：对象键值遍历
来源：http://lh.yuntaijiaju.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zw.jctech888.com.cn

[U92] JS：深拷贝
来源：http://hw.yuntaijiaju.cn

structuredClone(obj)
来源：http://nm.nicolike.cn

[U93] JS：模板字符串
来源：http://xf.huanxung.cn

`共 ${n} 条`
来源：http://ck.hnjuh.cn

[U94] JS：箭头函数
来源：http://as.nicolike.cn

const double = x => x * 2;
来源：http://rx.jianghongdianzi.cn

[U95] JS：Promise 包装
来源：http://jr.chemitech.net.cn

new Promise((resolve, reject) => {})
来源：http://sa.bjjhwx.cn

[U96] JS：async/await 与异常
来源：http://yv.szsharing.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zw.bjjhwx.cn

[U97] JS：并发请求
来源：http://fs.hahajie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://md.yuexingan06.cn

[U98] JS：fetch 带 JSON
来源：http://ev.nszjky.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://od.lnxyls.cn

[U99] JS：事件监听
来源：http://ko.haigaiapp.cn

el.addEventListener("click", e => {})
来源：http://it.shxzskj.cn

[U100] JS：DOM 查询
来源：http://ws.nicolike.cn

document.querySelector(".item")
来源：http://zn.bjjhwx.cn

[U101] JS：classList 操作
来源：http://wr.szsharing.cn

el.classList.toggle("active")
来源：http://du.yuexingan06.cn

[U102] JS：本地存储
来源：http://ha.bookmarksfly.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ul.huixiangedu.cn

[U103] JS：定时器
来源：http://ls.jctech888.com.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bd.huixiangedu.cn

[U104] JS：防抖
来源：http://mz.colortex.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ga.chemitech.net.cn

[U105] JS：节流
来源：http://xq.jianghongdianzi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mu.bjjhwx.cn

[U106] JS：日期格式化
来源：http://is.nicolike.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yt.shxzukj.cn

[U107] JS：数字千分位
来源：http://vq.szxytkj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dx.lnxyls.cn

[U108] JS：随机整数
来源：http://ro.hnjuh.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://if.bookmarksfly.cn

[U109] JS：数组分组
来源：http://eq.hahajie.cn

Object.groupBy(arr, x => x.type)
来源：http://bb.szsharing.cn

[U110] JS：数组分块
来源：http://ty.szxytkj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xv.szxytkj.cn

[U111] JS：对象转 Map
来源：http://zl.shxzukj.cn

new Map(Object.entries(obj))
来源：http://cy.hahajie.cn

[U112] JS：字符串补位
来源：http://mk.panjiajie.cn

"7".padStart(3, "0")
来源：http://nl.szxytkj.cn

[U113] JS：正则替换全部
来源：http://az.nicolike.cn

s.replaceAll("a", "b")
来源：http://ih.hahajie.cn

[U114] JS：JSON 深比较
来源：http://kh.bookmarksfly.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ca.hnjuh.cn

[U115] JS：生成 UUID
来源：http://cc.panjiajie.cn

crypto.randomUUID()
来源：http://sj.huixinmuqiang.cn

[U116] JS：类型检查（JSDoc）
来源：http://ra.colortex.cn

/** @param {string} name */ function f(name) {}
来源：http://xo.newstarts.cn

[U117] JS：单元测试
来源：http://lv.lnxyls.cn

npm i -D vitest;  npx vitest
来源：http://qp.shtwfgs.cn

[U118] JS：开发服务器
来源：http://vu.huanxung.cn

npm i -D vite;  npx vite
来源：http://ru.bookmarksfly.cn

[U119] JS：生产构建
来源：http://bl.nicolike.cn

npx vite build
来源：http://ba.gzmigu.cn

[U120] JS：读取环境变量（Vite）
来源：http://rz.newstarts.cn

import.meta.env.VITE_API_URL
来源：http://df.muxihuayi.cn

================================================================================
来源：http://yl.shxzskj.cn

统计汇总
来源：http://hi.lnxyls.cn

================================================================================
来源：http://zr.newstarts.cn

按语言统计（条）：
来源：http://hk.gzmigu.cn

Python ......... 252
来源：http://gw.gzmigu.cn

PHP ............ 252
来源：http://ko.huanxung.cn

JavaScript ..... 252
来源：http://ll.szxytkj.cn

TypeScript ..... 212
来源：http://jp.szsharing.cn

Java ........... 212
来源：http://zr.shxzukj.cn

Go ............. 212
来源：http://sq.521024.cn

Ruby ........... 212
来源：http://jc.yuntaijiaju.cn

C# ............. 212
来源：http://wq.bookmarksfly.cn

C .............. 30
来源：http://ev.lnxyls.cn

C++ ............ 30
来源：http://yw.nicolike.cn

SQL ............ 90
来源：http://gm.hnjuh.cn

Bash ........... 80
来源：http://tq.huixinmuqiang.cn

Kotlin ......... 15
来源：http://pe.jianghongdianzi.cn

Swift .......... 15
来源：http://xl.colortex.cn

Lua ............ 10
来源：http://al.szxytkj.cn

Perl ........... 10
来源：http://gh.asd995.cn

Scala .......... 10
来源：http://kg.bjjhwx.cn

------------------------------------
来源：http://ig.hnjuh.cn

合计 ........... 2106 条
来源：http://mz.muxihuayi.cn

按章节统计：
来源：http://ha.huixinmuqiang.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tw.shtwfgs.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xu.bookmarksfly.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://il.asd995.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nu.chemitech.net.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ks.haigaiapp.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://eh.nicolike.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://uq.bookmarksfly.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ty.panjiajie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xj.huixiangedu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mw.yuexingan06.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vj.hahajie.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rj.lnxyls.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ce.bjjhwx.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://eo.huixiangedu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zz.chemitech.net.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fu.shxzskj.cn

Q SQL 专题                              90
来源：http://zj.chemitech.net.cn

R Bash 专题                             80
来源：http://dj.szsharing.cn

S C / C++ 专题                          60
来源：http://ow.muxihuayi.cn

T 其他语言补充                          60
来源：http://fw.haigaiapp.cn

U 高频实用片段                         120
来源：http://iu.jctech888.com.cn

------------------------------------
来源：http://xd.hahajie.cn

合计                                  2106 条
来源：http://kb.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://ez.yuexingan06.cn

使用提醒
来源：http://ao.huanxung.cn

--------------------------------------------------------------------------------
来源：http://de.asd995.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vm.yuntaijiaju.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wv.shxzukj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bt.shxzukj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://gx.huixiangedu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://yj.yuntaijiaju.cn

—— 文件结束 ——
来源：http://yi.gzmigu.cn

================================================================================
来源：http://pz.huixiangedu.cn

程序语言常见例子速查手册（2024 版）
来源：http://po.huixiangedu.cn

Common Programming Examples Cheat Book
来源：http://re.huixinmuqiang.cn

================================================================================
来源：http://kv.newstarts.cn

【收录内容】
来源：http://de.haigaiapp.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://xs.521024.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jf.haigaiapp.cn

SQL · Bash · C · C++
来源：http://dc.lnxyls.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qy.9csxet.cn

【使用说明】
来源：http://yr.bjjhwx.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://jo.jianghongdianzi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ws.chemitech.net.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://li.shxzskj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xv.wgjwhj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://jo.9csxet.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xx.hnjuh.cn


<!-- 参考信息 -->