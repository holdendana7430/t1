代发 wailian999

[U11] Py：生成器表达式
来源：http://ow.panjiajie.cn

(x * 2 for x in arr)
来源：http://nr.huixinmuqiang.cn

[U12] Py：取出现最多的 3 个元素
来源：http://vn.shxzukj.cn

Counter(arr).most_common(3)
来源：http://rf.haigaiapp.cn

[U13] Py：固定长度队列
来源：http://ea.wgjwhj.cn

deque(maxlen=10)
来源：http://nl.shxzskj.cn

[U14] Py：分组收集到列表
来源：http://lu.jctech888.com.cn

defaultdict(list)
来源：http://rh.szxytkj.cn

[U15] Py：高精度计时
来源：http://yf.yuexingan06.cn

t = time.perf_counter()
来源：http://dl.jianghongdianzi.cn

[U16] Py：命令行参数解析
来源：http://xm.gzmigu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://eu.shtwfgs.cn

[U17] Py：初始化日志
来源：http://zi.gzmigu.cn

logging.basicConfig(level=logging.INFO)
来源：http://hx.haigaiapp.cn

[U18] Py：预编译正则
来源：http://ba.szxytkj.cn

pat = re.compile(r"\d+")
来源：http://ok.hahajie.cn

[U19] Py：正则替换带回调
来源：http://em.bjjhwx.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zh.bjjhwx.cn

[U20] Py：缓存函数结果
来源：http://kn.bookmarksfly.cn

@functools.lru_cache(maxsize=None)
来源：http://ek.shxzukj.cn

[U21] Py：自定义上下文管理器
来源：http://gp.muxihuayi.cn

@contextlib.contextmanager
来源：http://dw.bjjhwx.cn

[U22] Py：矩阵转置
来源：http://jp.newstarts.cn

list(zip(*m))
来源：http://rk.shxzskj.cn

[U23] Py：分块读取大文件
来源：http://eo.jctech888.com.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pa.9csxet.cn

[U24] Py：路径操作
来源：http://xe.chemitech.net.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rc.jianghongdianzi.cn

[U25] Py：CSV 按字典读
来源：http://zo.szsharing.cn

csv.DictReader(f)
来源：http://du.521024.cn

[U26] Py：并发下载
来源：http://ag.yuntaijiaju.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dj.yuntaijiaju.cn

[U27] Py：异步 HTTP
来源：http://bd.hahajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://ud.chemitech.net.cn

[U28] Py：类型别名
来源：http://pn.huixiangedu.cn

UserId = int
来源：http://oq.szsharing.cn

[U29] Py：属性校验
来源：http://bl.asd995.cn

@property 与 @x.setter 配合
来源：http://ja.jctech888.com.cn

[U30] Py：数据类
来源：http://hg.szsharing.cn

@dataclass(slots=True)
来源：http://bd.bjjhwx.cn

[U31] Py：单测
来源：http://qt.yuntaijiaju.cn

python -m pytest -q
来源：http://wj.colortex.cn

[U32] Py：代码格式化
来源：http://wh.shxzukj.cn

ruff format . && ruff check --fix .
来源：http://zm.muxihuayi.cn

[U33] Py：打包发布
来源：http://jm.bjjhwx.cn

python -m build  （依赖 pyproject.toml）
来源：http://hv.hnjuh.cn

[U34] Py：判断编码
来源：http://hb.shxzskj.cn

chardet.detect(raw)
来源：http://dd.521024.cn

[U35] Py：发送邮件
来源：http://qq.yuntaijiaju.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qj.yuntaijiaju.cn

[U36] Py：定时任务
来源：http://bh.colortex.cn

schedule.every(10).minutes.do(job)
来源：http://et.szsharing.cn

[U37] Py：读写 Excel
来源：http://fc.hnjuh.cn

pandas.read_excel / DataFrame.to_excel
来源：http://oh.yuntaijiaju.cn

[U38] Py：获取脚本所在目录
来源：http://fs.jianghongdianzi.cn

Path(__file__).resolve().parent
来源：http://tb.shxzukj.cn

[U39] Py：判断是否在交互环境
来源：http://rl.newstarts.cn

sys.stdout.isatty()
来源：http://ch.yuntaijiaju.cn

[U40] Py：打印到标准错误
来源：http://bk.lnxyls.cn

print("err", file=sys.stderr)
来源：http://qi.nszjky.cn

[U41] PHP：初始化 Composer 项目
来源：http://uj.jianghongdianzi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://dq.nszjky.cn

[U42] PHP：PSR-4 自动加载
来源：http://ja.szsharing.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vj.bookmarksfly.cn

[U43] PHP：声明命名空间
来源：http://je.chemitech.net.cn

namespace App\Http;
来源：http://rg.colortex.cn

[U44] PHP：开启严格类型
来源：http://ek.yuexingan06.cn

declare(strict_types=1);
来源：http://lx.szxytkj.cn

[U45] PHP：类型声明与返回类型
来源：http://rb.huixiangedu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://mu.gzmigu.cn

[U46] PHP：可空类型
来源：http://xq.521024.cn

?string $name = null
来源：http://rm.asd995.cn

[U47] PHP：联合类型
来源：http://hb.szxytkj.cn

int|string $id
来源：http://ih.muxihuayi.cn

[U48] PHP：纯枚举
来源：http://ay.gzmigu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gy.hnjuh.cn

[U49] PHP：只读属性
来源：http://wd.muxihuayi.cn

public readonly string $name
来源：http://wj.lnxyls.cn

[U50] PHP：构造器属性提升
来源：http://ja.bookmarksfly.cn

public function __construct(private int $id) {}
来源：http://vd.panjiajie.cn

[U51] PHP：数组解构
来源：http://ly.shtwfgs.cn

[$a, $b] = $arr;
来源：http://he.wgjwhj.cn

[U52] PHP：箭头函数
来源：http://pk.asd995.cn

$double = fn($x) => $x * 2;
来源：http://bb.haigaiapp.cn

[U53] PHP：空合并运算符
来源：http://xj.chemitech.net.cn

$v = $a ?? $b ?? "default";
来源：http://md.szsharing.cn

[U54] PHP：空安全调用
来源：http://gk.9csxet.cn

$obj?->method()
来源：http://cy.shtwfgs.cn

[U55] PHP：match 表达式
来源：http://ne.jctech888.com.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jb.szxytkj.cn

[U56] PHP：命名参数
来源：http://iq.shxzukj.cn

f(a: 1, b: 2)
来源：http://qp.gzmigu.cn

[U57] PHP：字符串插值
来源：http://fd.newstarts.cn

"值: {$a}"
来源：http://nm.lnxyls.cn

[U58] PHP：数组三件套
来源：http://sp.huixiangedu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lb.bjjhwx.cn

[U59] PHP：自定义排序
来源：http://hw.huixinmuqiang.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fc.huanxung.cn

[U60] PHP：JSON 编解码
来源：http://yo.panjiajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://uq.lnxyls.cn

[U61] PHP：正则
来源：http://fl.shtwfgs.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cg.yuntaijiaju.cn

[U62] PHP：日期对象
来源：http://qo.wgjwhj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kc.yuntaijiaju.cn

[U63] PHP：文件读写
来源：http://bd.hahajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://he.shxzukj.cn

[U64] PHP：目录遍历
来源：http://zz.bjjhwx.cn

glob("dir/*.php");  scandir("dir");
来源：http://pz.hahajie.cn

[U65] PHP：会话
来源：http://np.hahajie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://it.hahajie.cn

[U66] PHP：设置 Cookie
来源：http://yl.jctech888.com.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vv.nicolike.cn

[U67] PHP：处理文件上传
来源：http://zg.nicolike.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://uz.wgjwhj.cn

[U68] PHP：PDO 连接
来源：http://ad.huanxung.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tq.521024.cn

[U69] PHP：PDO 预处理
来源：http://ne.colortex.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sh.colortex.cn

[U70] PHP：PDO 事务
来源：http://qu.szxytkj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://je.huixiangedu.cn

[U71] PHP：抛出异常
来源：http://ag.newstarts.cn

throw new RuntimeException("失败", 500);
来源：http://iq.lnxyls.cn

[U72] PHP：写错误日志
来源：http://jr.jianghongdianzi.cn

error_log("失败: " . $e->getMessage());
来源：http://ku.chemitech.net.cn

[U73] PHP：读取 ini 配置
来源：http://wi.9csxet.cn

parse_ini_file("config.ini", true)
来源：http://dq.chemitech.net.cn

[U74] PHP：读取环境变量
来源：http://sr.asd995.cn

getenv("APP_ENV") ?: "production"
来源：http://kc.wgjwhj.cn

[U75] PHP：依赖注入
来源：http://pa.szsharing.cn

composer require psr/container
来源：http://ef.lnxyls.cn

[U76] PHP：简单路由
来源：http://fh.shxzukj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xf.bjjhwx.cn

[U77] PHP：模板渲染
来源：http://el.nicolike.cn

composer require twig/twig
来源：http://oa.hahajie.cn

[U78] PHP：单元测试
来源：http://bm.nicolike.cn

composer require --dev phpunit/phpunit
来源：http://tl.hahajie.cn

[U79] PHP：静态分析
来源：http://xp.lnxyls.cn

composer require --dev phpstan/phpstan
来源：http://oy.9csxet.cn

[U80] PHP：代码规范修复
来源：http://ue.bjjhwx.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://fw.9csxet.cn

[U81] JS：初始化项目
来源：http://vg.colortex.cn

npm init -y;  npm i express
来源：http://yy.yuexingan06.cn

[U82] JS：package.json 脚本
来源：http://cc.yuntaijiaju.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nl.gzmigu.cn

[U83] JS：ES Module 导入导出
来源：http://xu.muxihuayi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://uc.newstarts.cn

[U84] JS：CommonJS 写法
来源：http://fp.hnjuh.cn

module.exports = { a };  const { a } = require("./m");
来源：http://zv.szsharing.cn

[U85] JS：可选链
来源：http://vo.huanxung.cn

a?.b?.c
来源：http://gd.yuntaijiaju.cn

[U86] JS：空值合并
来源：http://mf.bookmarksfly.cn

a ?? b
来源：http://iq.chemitech.net.cn

[U87] JS：解构默认值
来源：http://op.muxihuayi.cn

const { a = 1, b = 2 } = obj;
来源：http://vd.szxytkj.cn

[U88] JS：对象展开合并
来源：http://cw.szxytkj.cn

{ ...a, ...b }
来源：http://ua.shtwfgs.cn

[U89] JS：数组去重
来源：http://vb.yuntaijiaju.cn

[...new Set(arr)]
来源：http://nh.nszjky.cn

[U90] JS：数字数组排序
来源：http://tf.hnjuh.cn

[...arr].sort((a, b) => a - b)
来源：http://fv.jctech888.com.cn

[U91] JS：对象键值遍历
来源：http://qo.yuntaijiaju.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ll.521024.cn

[U92] JS：深拷贝
来源：http://zm.jctech888.com.cn

structuredClone(obj)
来源：http://qc.gzmigu.cn

[U93] JS：模板字符串
来源：http://dw.shxzukj.cn

`共 ${n} 条`
来源：http://vd.asd995.cn

[U94] JS：箭头函数
来源：http://it.jctech888.com.cn

const double = x => x * 2;
来源：http://aw.lnxyls.cn

[U95] JS：Promise 包装
来源：http://sl.nicolike.cn

new Promise((resolve, reject) => {})
来源：http://qv.haigaiapp.cn

[U96] JS：async/await 与异常
来源：http://cc.newstarts.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mz.9csxet.cn

[U97] JS：并发请求
来源：http://fe.colortex.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://yg.colortex.cn

[U98] JS：fetch 带 JSON
来源：http://pb.szsharing.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ge.wgjwhj.cn

[U99] JS：事件监听
来源：http://rx.huanxung.cn

el.addEventListener("click", e => {})
来源：http://sy.lnxyls.cn

[U100] JS：DOM 查询
来源：http://pm.yuntaijiaju.cn

document.querySelector(".item")
来源：http://ga.hahajie.cn

[U101] JS：classList 操作
来源：http://cf.shxzukj.cn

el.classList.toggle("active")
来源：http://ca.bookmarksfly.cn

[U102] JS：本地存储
来源：http://xk.colortex.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://fc.hahajie.cn

[U103] JS：定时器
来源：http://ux.nicolike.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uu.shtwfgs.cn

[U104] JS：防抖
来源：http://wo.chemitech.net.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eo.jianghongdianzi.cn

[U105] JS：节流
来源：http://gn.bookmarksfly.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ae.yuntaijiaju.cn

[U106] JS：日期格式化
来源：http://ye.szsharing.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ph.hnjuh.cn

[U107] JS：数字千分位
来源：http://ho.panjiajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qa.huixinmuqiang.cn

[U108] JS：随机整数
来源：http://ju.521024.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vs.bjjhwx.cn

[U109] JS：数组分组
来源：http://hg.colortex.cn

Object.groupBy(arr, x => x.type)
来源：http://uf.huanxung.cn

[U110] JS：数组分块
来源：http://oa.521024.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ms.hnjuh.cn

[U111] JS：对象转 Map
来源：http://mk.yuexingan06.cn

new Map(Object.entries(obj))
来源：http://ep.jctech888.com.cn

[U112] JS：字符串补位
来源：http://ow.muxihuayi.cn

"7".padStart(3, "0")
来源：http://rx.huanxung.cn

[U113] JS：正则替换全部
来源：http://qi.hnjuh.cn

s.replaceAll("a", "b")
来源：http://vt.bookmarksfly.cn

[U114] JS：JSON 深比较
来源：http://zk.newstarts.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://tx.hahajie.cn

[U115] JS：生成 UUID
来源：http://ku.hahajie.cn

crypto.randomUUID()
来源：http://mf.panjiajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://et.gzmigu.cn

/** @param {string} name */ function f(name) {}
来源：http://ke.chemitech.net.cn

[U117] JS：单元测试
来源：http://tc.bjjhwx.cn

npm i -D vitest;  npx vitest
来源：http://cd.szxytkj.cn

[U118] JS：开发服务器
来源：http://xy.haigaiapp.cn

npm i -D vite;  npx vite
来源：http://dd.szxytkj.cn

[U119] JS：生产构建
来源：http://wi.asd995.cn

npx vite build
来源：http://lx.huixiangedu.cn

[U120] JS：读取环境变量（Vite）
来源：http://gk.szxytkj.cn

import.meta.env.VITE_API_URL
来源：http://vx.newstarts.cn

================================================================================
来源：http://lt.521024.cn

统计汇总
来源：http://wi.9csxet.cn

================================================================================
来源：http://kg.shtwfgs.cn

按语言统计（条）：
来源：http://cx.huanxung.cn

Python ......... 252
来源：http://bq.9csxet.cn

PHP ............ 252
来源：http://kj.colortex.cn

JavaScript ..... 252
来源：http://ho.yuntaijiaju.cn

TypeScript ..... 212
来源：http://dj.muxihuayi.cn

Java ........... 212
来源：http://gb.huixinmuqiang.cn

Go ............. 212
来源：http://pk.shtwfgs.cn

Ruby ........... 212
来源：http://cs.bookmarksfly.cn

C# ............. 212
来源：http://df.lnxyls.cn

C .............. 30
来源：http://ks.shxzskj.cn

C++ ............ 30
来源：http://cx.szxytkj.cn

SQL ............ 90
来源：http://qn.jianghongdianzi.cn

Bash ........... 80
来源：http://nm.hnjuh.cn

Kotlin ......... 15
来源：http://dq.nicolike.cn

Swift .......... 15
来源：http://iw.gzmigu.cn

Lua ............ 10
来源：http://uc.shxzukj.cn

Perl ........... 10
来源：http://db.nszjky.cn

Scala .......... 10
来源：http://xr.nicolike.cn

------------------------------------
来源：http://oq.chemitech.net.cn

合计 ........... 2106 条
来源：http://sq.szxytkj.cn

按章节统计：
来源：http://ig.lnxyls.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cf.szxytkj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qp.yuntaijiaju.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gu.bjjhwx.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://by.gzmigu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ih.jianghongdianzi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sn.huanxung.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hn.hahajie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gm.huixiangedu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://eb.huixinmuqiang.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xm.shxzukj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ut.huixinmuqiang.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jy.nszjky.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ta.haigaiapp.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://te.yuexingan06.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://aw.521024.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://av.nszjky.cn

Q SQL 专题                              90
来源：http://ps.szsharing.cn

R Bash 专题                             80
来源：http://vk.colortex.cn

S C / C++ 专题                          60
来源：http://op.nszjky.cn

T 其他语言补充                          60
来源：http://dh.lnxyls.cn

U 高频实用片段                         120
来源：http://ql.muxihuayi.cn

------------------------------------
来源：http://qx.shtwfgs.cn

合计                                  2106 条
来源：http://fs.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://gu.szxytkj.cn

使用提醒
来源：http://zz.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://or.yuexingan06.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cd.jianghongdianzi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://na.huixiangedu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ph.hnjuh.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ej.bjjhwx.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rs.wgjwhj.cn

—— 文件结束 ——
来源：http://fl.wgjwhj.cn

================================================================================
来源：http://mh.muxihuayi.cn

程序语言常见例子速查手册（2024 版）
来源：http://qv.szsharing.cn

Common Programming Examples Cheat Book
来源：http://cy.bjjhwx.cn

================================================================================
来源：http://ra.panjiajie.cn

【收录内容】
来源：http://iu.nszjky.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://vn.asd995.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hr.bookmarksfly.cn

SQL · Bash · C · C++
来源：http://no.szxytkj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xw.lnxyls.cn

【使用说明】
来源：http://mt.haigaiapp.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lz.yuexingan06.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ie.shxzukj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://yn.newstarts.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://kf.huixiangedu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ik.muxihuayi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qw.jctech888.com.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tz.bjjhwx.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://yf.shtwfgs.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yk.huanxung.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://kr.gzmigu.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://fh.szsharing.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://sl.jianghongdianzi.cn

【文件统计】
来源：http://jk.chemitech.net.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hu.newstarts.cn


<!-- 参考信息 -->