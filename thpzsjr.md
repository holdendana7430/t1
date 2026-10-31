代发 wailian999

[U13] Py：固定长度队列
来源：http://hh.huanxung.cn

deque(maxlen=10)
来源：http://ch.muxihuayi.cn

[U14] Py：分组收集到列表
来源：http://dh.bjjhwx.cn

defaultdict(list)
来源：http://ls.shxzukj.cn

[U15] Py：高精度计时
来源：http://zo.bjjhwx.cn

t = time.perf_counter()
来源：http://id.haigaiapp.cn

[U16] Py：命令行参数解析
来源：http://mt.gzmigu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ei.hahajie.cn

[U17] Py：初始化日志
来源：http://je.bjjhwx.cn

logging.basicConfig(level=logging.INFO)
来源：http://wc.yuexingan06.cn

[U18] Py：预编译正则
来源：http://xv.huixiangedu.cn

pat = re.compile(r"\d+")
来源：http://bh.shxzukj.cn

[U19] Py：正则替换带回调
来源：http://kr.9csxet.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fu.szxytkj.cn

[U20] Py：缓存函数结果
来源：http://pl.jianghongdianzi.cn

@functools.lru_cache(maxsize=None)
来源：http://yk.huanxung.cn

[U21] Py：自定义上下文管理器
来源：http://fb.asd995.cn

@contextlib.contextmanager
来源：http://nf.nicolike.cn

[U22] Py：矩阵转置
来源：http://qr.muxihuayi.cn

list(zip(*m))
来源：http://rg.newstarts.cn

[U23] Py：分块读取大文件
来源：http://xc.jctech888.com.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vw.szxytkj.cn

[U24] Py：路径操作
来源：http://qx.asd995.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lh.panjiajie.cn

[U25] Py：CSV 按字典读
来源：http://rp.colortex.cn

csv.DictReader(f)
来源：http://mv.bjjhwx.cn

[U26] Py：并发下载
来源：http://ks.bookmarksfly.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fh.jianghongdianzi.cn

[U27] Py：异步 HTTP
来源：http://tm.shtwfgs.cn

aiohttp.ClientSession() 配合 async with
来源：http://rz.newstarts.cn

[U28] Py：类型别名
来源：http://af.shtwfgs.cn

UserId = int
来源：http://vn.szxytkj.cn

[U29] Py：属性校验
来源：http://sv.521024.cn

@property 与 @x.setter 配合
来源：http://vr.lnxyls.cn

[U30] Py：数据类
来源：http://tg.huixiangedu.cn

@dataclass(slots=True)
来源：http://qs.haigaiapp.cn

[U31] Py：单测
来源：http://og.shxzukj.cn

python -m pytest -q
来源：http://at.muxihuayi.cn

[U32] Py：代码格式化
来源：http://yw.nszjky.cn

ruff format . && ruff check --fix .
来源：http://tc.shxzskj.cn

[U33] Py：打包发布
来源：http://ln.huixinmuqiang.cn

python -m build  （依赖 pyproject.toml）
来源：http://fa.jctech888.com.cn

[U34] Py：判断编码
来源：http://ae.bjjhwx.cn

chardet.detect(raw)
来源：http://pz.nszjky.cn

[U35] Py：发送邮件
来源：http://mc.huanxung.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bo.chemitech.net.cn

[U36] Py：定时任务
来源：http://ew.bjjhwx.cn

schedule.every(10).minutes.do(job)
来源：http://fu.asd995.cn

[U37] Py：读写 Excel
来源：http://wh.muxihuayi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://rm.lnxyls.cn

[U38] Py：获取脚本所在目录
来源：http://gj.gzmigu.cn

Path(__file__).resolve().parent
来源：http://sn.newstarts.cn

[U39] Py：判断是否在交互环境
来源：http://qz.shxzskj.cn

sys.stdout.isatty()
来源：http://bq.hnjuh.cn

[U40] Py：打印到标准错误
来源：http://mm.521024.cn

print("err", file=sys.stderr)
来源：http://yh.chemitech.net.cn

[U41] PHP：初始化 Composer 项目
来源：http://av.wgjwhj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://tt.colortex.cn

[U42] PHP：PSR-4 自动加载
来源：http://zv.asd995.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ok.lnxyls.cn

[U43] PHP：声明命名空间
来源：http://of.haigaiapp.cn

namespace App\Http;
来源：http://jo.hnjuh.cn

[U44] PHP：开启严格类型
来源：http://kv.jianghongdianzi.cn

declare(strict_types=1);
来源：http://on.hahajie.cn

[U45] PHP：类型声明与返回类型
来源：http://dc.hnjuh.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://od.szsharing.cn

[U46] PHP：可空类型
来源：http://gt.newstarts.cn

?string $name = null
来源：http://aj.jctech888.com.cn

[U47] PHP：联合类型
来源：http://tk.colortex.cn

int|string $id
来源：http://ms.panjiajie.cn

[U48] PHP：纯枚举
来源：http://wi.9csxet.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lv.chemitech.net.cn

[U49] PHP：只读属性
来源：http://ta.newstarts.cn

public readonly string $name
来源：http://rn.yuexingan06.cn

[U50] PHP：构造器属性提升
来源：http://mz.gzmigu.cn

public function __construct(private int $id) {}
来源：http://ai.nicolike.cn

[U51] PHP：数组解构
来源：http://il.huixinmuqiang.cn

[$a, $b] = $arr;
来源：http://ih.hahajie.cn

[U52] PHP：箭头函数
来源：http://ly.lnxyls.cn

$double = fn($x) => $x * 2;
来源：http://mn.gzmigu.cn

[U53] PHP：空合并运算符
来源：http://ui.chemitech.net.cn

$v = $a ?? $b ?? "default";
来源：http://vj.haigaiapp.cn

[U54] PHP：空安全调用
来源：http://by.muxihuayi.cn

$obj?->method()
来源：http://ig.yuntaijiaju.cn

[U55] PHP：match 表达式
来源：http://eg.yuntaijiaju.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ls.szxytkj.cn

[U56] PHP：命名参数
来源：http://zu.hahajie.cn

f(a: 1, b: 2)
来源：http://gt.lnxyls.cn

[U57] PHP：字符串插值
来源：http://kz.panjiajie.cn

"值: {$a}"
来源：http://fh.nszjky.cn

[U58] PHP：数组三件套
来源：http://gs.shxzskj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ny.9csxet.cn

[U59] PHP：自定义排序
来源：http://wi.muxihuayi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qk.bookmarksfly.cn

[U60] PHP：JSON 编解码
来源：http://ti.nszjky.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ic.panjiajie.cn

[U61] PHP：正则
来源：http://gp.shxzukj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://io.hnjuh.cn

[U62] PHP：日期对象
来源：http://fr.haigaiapp.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nm.nszjky.cn

[U63] PHP：文件读写
来源：http://hv.bookmarksfly.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zj.gzmigu.cn

[U64] PHP：目录遍历
来源：http://pj.shxzukj.cn

glob("dir/*.php");  scandir("dir");
来源：http://al.asd995.cn

[U65] PHP：会话
来源：http://ie.haigaiapp.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://wd.bookmarksfly.cn

[U66] PHP：设置 Cookie
来源：http://go.newstarts.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sv.huanxung.cn

[U67] PHP：处理文件上传
来源：http://vr.newstarts.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vv.521024.cn

[U68] PHP：PDO 连接
来源：http://jm.jctech888.com.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pb.asd995.cn

[U69] PHP：PDO 预处理
来源：http://xd.haigaiapp.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yu.huanxung.cn

[U70] PHP：PDO 事务
来源：http://rv.hnjuh.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lb.yuexingan06.cn

[U71] PHP：抛出异常
来源：http://bl.jctech888.com.cn

throw new RuntimeException("失败", 500);
来源：http://qn.shtwfgs.cn

[U72] PHP：写错误日志
来源：http://zz.muxihuayi.cn

error_log("失败: " . $e->getMessage());
来源：http://gl.huixinmuqiang.cn

[U73] PHP：读取 ini 配置
来源：http://kd.hahajie.cn

parse_ini_file("config.ini", true)
来源：http://fb.bjjhwx.cn

[U74] PHP：读取环境变量
来源：http://fo.huanxung.cn

getenv("APP_ENV") ?: "production"
来源：http://zz.521024.cn

[U75] PHP：依赖注入
来源：http://pt.newstarts.cn

composer require psr/container
来源：http://yj.bjjhwx.cn

[U76] PHP：简单路由
来源：http://nx.huanxung.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tl.yuexingan06.cn

[U77] PHP：模板渲染
来源：http://bk.hnjuh.cn

composer require twig/twig
来源：http://ts.panjiajie.cn

[U78] PHP：单元测试
来源：http://ox.hahajie.cn

composer require --dev phpunit/phpunit
来源：http://xa.shxzukj.cn

[U79] PHP：静态分析
来源：http://ta.yuntaijiaju.cn

composer require --dev phpstan/phpstan
来源：http://cy.szxytkj.cn

[U80] PHP：代码规范修复
来源：http://mj.chemitech.net.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://pg.panjiajie.cn

[U81] JS：初始化项目
来源：http://dk.nicolike.cn

npm init -y;  npm i express
来源：http://hs.haigaiapp.cn

[U82] JS：package.json 脚本
来源：http://uc.shxzskj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tk.asd995.cn

[U83] JS：ES Module 导入导出
来源：http://rh.521024.cn

export const a = 1;  import { a } from "./m.js";
来源：http://kp.szxytkj.cn

[U84] JS：CommonJS 写法
来源：http://kc.jianghongdianzi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://nd.shtwfgs.cn

[U85] JS：可选链
来源：http://fd.hnjuh.cn

a?.b?.c
来源：http://sf.wgjwhj.cn

[U86] JS：空值合并
来源：http://ws.shtwfgs.cn

a ?? b
来源：http://vn.521024.cn

[U87] JS：解构默认值
来源：http://sp.nszjky.cn

const { a = 1, b = 2 } = obj;
来源：http://hq.muxihuayi.cn

[U88] JS：对象展开合并
来源：http://vu.shxzukj.cn

{ ...a, ...b }
来源：http://tl.wgjwhj.cn

[U89] JS：数组去重
来源：http://ck.gzmigu.cn

[...new Set(arr)]
来源：http://ng.szxytkj.cn

[U90] JS：数字数组排序
来源：http://xu.newstarts.cn

[...arr].sort((a, b) => a - b)
来源：http://zo.huixinmuqiang.cn

[U91] JS：对象键值遍历
来源：http://no.shxzukj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mh.muxihuayi.cn

[U92] JS：深拷贝
来源：http://dj.haigaiapp.cn

structuredClone(obj)
来源：http://bu.huixiangedu.cn

[U93] JS：模板字符串
来源：http://xb.yuntaijiaju.cn

`共 ${n} 条`
来源：http://xf.jianghongdianzi.cn

[U94] JS：箭头函数
来源：http://er.hnjuh.cn

const double = x => x * 2;
来源：http://vz.bookmarksfly.cn

[U95] JS：Promise 包装
来源：http://mg.yuntaijiaju.cn

new Promise((resolve, reject) => {})
来源：http://hp.panjiajie.cn

[U96] JS：async/await 与异常
来源：http://oy.colortex.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dh.shxzukj.cn

[U97] JS：并发请求
来源：http://jg.521024.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://iv.shtwfgs.cn

[U98] JS：fetch 带 JSON
来源：http://sk.nszjky.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cl.panjiajie.cn

[U99] JS：事件监听
来源：http://wz.shtwfgs.cn

el.addEventListener("click", e => {})
来源：http://rk.szsharing.cn

[U100] JS：DOM 查询
来源：http://rk.yuexingan06.cn

document.querySelector(".item")
来源：http://ow.shxzskj.cn

[U101] JS：classList 操作
来源：http://fn.huixiangedu.cn

el.classList.toggle("active")
来源：http://pr.bjjhwx.cn

[U102] JS：本地存储
来源：http://wr.wgjwhj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://mn.muxihuayi.cn

[U103] JS：定时器
来源：http://lm.nszjky.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gn.huixiangedu.cn

[U104] JS：防抖
来源：http://zt.nicolike.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://io.chemitech.net.cn

[U105] JS：节流
来源：http://ce.bjjhwx.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ku.jctech888.com.cn

[U106] JS：日期格式化
来源：http://bh.haigaiapp.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wh.muxihuayi.cn

[U107] JS：数字千分位
来源：http://vf.huanxung.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ns.lnxyls.cn

[U108] JS：随机整数
来源：http://rg.jianghongdianzi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ll.bookmarksfly.cn

[U109] JS：数组分组
来源：http://fs.jctech888.com.cn

Object.groupBy(arr, x => x.type)
来源：http://zb.bookmarksfly.cn

[U110] JS：数组分块
来源：http://bh.muxihuayi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zn.panjiajie.cn

[U111] JS：对象转 Map
来源：http://lr.nicolike.cn

new Map(Object.entries(obj))
来源：http://fh.hahajie.cn

[U112] JS：字符串补位
来源：http://pd.nicolike.cn

"7".padStart(3, "0")
来源：http://lb.huanxung.cn

[U113] JS：正则替换全部
来源：http://lr.shxzskj.cn

s.replaceAll("a", "b")
来源：http://eo.521024.cn

[U114] JS：JSON 深比较
来源：http://vk.shxzukj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://po.colortex.cn

[U115] JS：生成 UUID
来源：http://an.panjiajie.cn

crypto.randomUUID()
来源：http://lt.521024.cn

[U116] JS：类型检查（JSDoc）
来源：http://qw.szxytkj.cn

/** @param {string} name */ function f(name) {}
来源：http://cx.bjjhwx.cn

[U117] JS：单元测试
来源：http://ae.nicolike.cn

npm i -D vitest;  npx vitest
来源：http://ci.jctech888.com.cn

[U118] JS：开发服务器
来源：http://uy.shtwfgs.cn

npm i -D vite;  npx vite
来源：http://om.nicolike.cn

[U119] JS：生产构建
来源：http://un.chemitech.net.cn

npx vite build
来源：http://mg.shtwfgs.cn

[U120] JS：读取环境变量（Vite）
来源：http://vq.shxzskj.cn

import.meta.env.VITE_API_URL
来源：http://vf.huixiangedu.cn

================================================================================
来源：http://kg.huixinmuqiang.cn

统计汇总
来源：http://iu.szxytkj.cn

================================================================================
来源：http://iz.colortex.cn

按语言统计（条）：
来源：http://bd.szsharing.cn

Python ......... 252
来源：http://om.nszjky.cn

PHP ............ 252
来源：http://iq.wgjwhj.cn

JavaScript ..... 252
来源：http://pg.bookmarksfly.cn

TypeScript ..... 212
来源：http://xx.lnxyls.cn

Java ........... 212
来源：http://gw.lnxyls.cn

Go ............. 212
来源：http://dz.9csxet.cn

Ruby ........... 212
来源：http://zc.muxihuayi.cn

C# ............. 212
来源：http://ao.chemitech.net.cn

C .............. 30
来源：http://kc.chemitech.net.cn

C++ ............ 30
来源：http://qx.hahajie.cn

SQL ............ 90
来源：http://ma.lnxyls.cn

Bash ........... 80
来源：http://mu.jctech888.com.cn

Kotlin ......... 15
来源：http://uy.9csxet.cn

Swift .......... 15
来源：http://zc.shtwfgs.cn

Lua ............ 10
来源：http://vh.bjjhwx.cn

Perl ........... 10
来源：http://ua.hnjuh.cn

Scala .......... 10
来源：http://ep.jianghongdianzi.cn

------------------------------------
来源：http://mq.yuexingan06.cn

合计 ........... 2106 条
来源：http://tj.9csxet.cn

按章节统计：
来源：http://ty.huixiangedu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hy.haigaiapp.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ax.newstarts.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hn.yuntaijiaju.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ti.521024.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bz.gzmigu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://eh.jctech888.com.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://us.huixiangedu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gi.jctech888.com.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tq.gzmigu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ha.nicolike.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gh.panjiajie.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cr.bookmarksfly.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ua.nszjky.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sg.jctech888.com.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://oi.panjiajie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://nb.asd995.cn

Q SQL 专题                              90
来源：http://xj.yuntaijiaju.cn

R Bash 专题                             80
来源：http://uw.hahajie.cn

S C / C++ 专题                          60
来源：http://jm.shtwfgs.cn

T 其他语言补充                          60
来源：http://li.muxihuayi.cn

U 高频实用片段                         120
来源：http://nh.wgjwhj.cn

------------------------------------
来源：http://la.jctech888.com.cn

合计                                  2106 条
来源：http://em.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://ya.9csxet.cn

使用提醒
来源：http://bs.newstarts.cn

--------------------------------------------------------------------------------
来源：http://bl.szxytkj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://br.huixinmuqiang.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://nd.asd995.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ta.huixiangedu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://eb.9csxet.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rc.jctech888.com.cn

—— 文件结束 ——
来源：http://rp.muxihuayi.cn

================================================================================
来源：http://ks.shxzskj.cn

程序语言常见例子速查手册（2024 版）
来源：http://yv.szxytkj.cn

Common Programming Examples Cheat Book
来源：http://gz.gzmigu.cn

================================================================================
来源：http://sb.colortex.cn

【收录内容】
来源：http://nu.bookmarksfly.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ia.jctech888.com.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://lv.gzmigu.cn

SQL · Bash · C · C++
来源：http://hi.huixiangedu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://uq.huanxung.cn

【使用说明】
来源：http://wc.521024.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ra.chemitech.net.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rt.nicolike.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wi.nszjky.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ey.shxzukj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://te.wgjwhj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lb.huixiangedu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bk.huixinmuqiang.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://oj.muxihuayi.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://up.hnjuh.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://eg.newstarts.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://oz.shxzskj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ax.jctech888.com.cn

【文件统计】
来源：http://eg.bjjhwx.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cs.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://gk.newstarts.cn

目  录
来源：http://xi.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://ct.jianghongdianzi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ba.9csxet.cn


<!-- 参考信息 -->