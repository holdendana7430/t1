代发 wailian999

[U07] Py：反转字典键值
来源：http://sj.huixinmuqiang.cn

{v: k for k, v in d.items()}
来源：http://qc.asd995.cn

[U08] Py：展平二维列表
来源：http://kw.bjjhwx.cn

[y for x in nested for y in x]
来源：http://hs.huanxung.cn

[U09] Py：字典取最大值的键
来源：http://fq.jctech888.com.cn

max(d, key=d.get)
来源：http://xt.shxzukj.cn

[U10] Py：按值排序字典
来源：http://oq.wgjwhj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nj.nszjky.cn

[U11] Py：生成器表达式
来源：http://tf.jianghongdianzi.cn

(x * 2 for x in arr)
来源：http://bq.nszjky.cn

[U12] Py：取出现最多的 3 个元素
来源：http://bn.chemitech.net.cn

Counter(arr).most_common(3)
来源：http://bb.wgjwhj.cn

[U13] Py：固定长度队列
来源：http://kc.shxzukj.cn

deque(maxlen=10)
来源：http://jc.yuexingan06.cn

[U14] Py：分组收集到列表
来源：http://js.nszjky.cn

defaultdict(list)
来源：http://my.panjiajie.cn

[U15] Py：高精度计时
来源：http://qk.hahajie.cn

t = time.perf_counter()
来源：http://eq.newstarts.cn

[U16] Py：命令行参数解析
来源：http://bj.shxzukj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hy.huanxung.cn

[U17] Py：初始化日志
来源：http://di.hnjuh.cn

logging.basicConfig(level=logging.INFO)
来源：http://hs.huixinmuqiang.cn

[U18] Py：预编译正则
来源：http://du.hnjuh.cn

pat = re.compile(r"\d+")
来源：http://wu.shxzukj.cn

[U19] Py：正则替换带回调
来源：http://lx.bookmarksfly.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ke.gzmigu.cn

[U20] Py：缓存函数结果
来源：http://hu.huanxung.cn

@functools.lru_cache(maxsize=None)
来源：http://rs.wgjwhj.cn

[U21] Py：自定义上下文管理器
来源：http://fb.9csxet.cn

@contextlib.contextmanager
来源：http://qi.bjjhwx.cn

[U22] Py：矩阵转置
来源：http://in.haigaiapp.cn

list(zip(*m))
来源：http://sb.huixinmuqiang.cn

[U23] Py：分块读取大文件
来源：http://an.colortex.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rn.nicolike.cn

[U24] Py：路径操作
来源：http://ub.nszjky.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://eu.huixiangedu.cn

[U25] Py：CSV 按字典读
来源：http://tk.asd995.cn

csv.DictReader(f)
来源：http://yy.huanxung.cn

[U26] Py：并发下载
来源：http://gv.shxzskj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mt.bookmarksfly.cn

[U27] Py：异步 HTTP
来源：http://nj.muxihuayi.cn

aiohttp.ClientSession() 配合 async with
来源：http://ge.muxihuayi.cn

[U28] Py：类型别名
来源：http://ij.huixiangedu.cn

UserId = int
来源：http://na.colortex.cn

[U29] Py：属性校验
来源：http://cv.huixinmuqiang.cn

@property 与 @x.setter 配合
来源：http://ox.bjjhwx.cn

[U30] Py：数据类
来源：http://ab.jianghongdianzi.cn

@dataclass(slots=True)
来源：http://nd.nicolike.cn

[U31] Py：单测
来源：http://sc.szxytkj.cn

python -m pytest -q
来源：http://vn.muxihuayi.cn

[U32] Py：代码格式化
来源：http://px.szsharing.cn

ruff format . && ruff check --fix .
来源：http://zb.wgjwhj.cn

[U33] Py：打包发布
来源：http://bm.chemitech.net.cn

python -m build  （依赖 pyproject.toml）
来源：http://ky.nszjky.cn

[U34] Py：判断编码
来源：http://sj.bookmarksfly.cn

chardet.detect(raw)
来源：http://dz.jianghongdianzi.cn

[U35] Py：发送邮件
来源：http://gt.9csxet.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mt.colortex.cn

[U36] Py：定时任务
来源：http://mn.chemitech.net.cn

schedule.every(10).minutes.do(job)
来源：http://gu.9csxet.cn

[U37] Py：读写 Excel
来源：http://vp.huanxung.cn

pandas.read_excel / DataFrame.to_excel
来源：http://bb.haigaiapp.cn

[U38] Py：获取脚本所在目录
来源：http://rd.yuntaijiaju.cn

Path(__file__).resolve().parent
来源：http://gv.wgjwhj.cn

[U39] Py：判断是否在交互环境
来源：http://ak.yuntaijiaju.cn

sys.stdout.isatty()
来源：http://vx.colortex.cn

[U40] Py：打印到标准错误
来源：http://ws.panjiajie.cn

print("err", file=sys.stderr)
来源：http://ci.bookmarksfly.cn

[U41] PHP：初始化 Composer 项目
来源：http://hj.asd995.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://bv.9csxet.cn

[U42] PHP：PSR-4 自动加载
来源：http://db.yuntaijiaju.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://is.shxzukj.cn

[U43] PHP：声明命名空间
来源：http://aw.muxihuayi.cn

namespace App\Http;
来源：http://we.nszjky.cn

[U44] PHP：开启严格类型
来源：http://hr.szxytkj.cn

declare(strict_types=1);
来源：http://ck.panjiajie.cn

[U45] PHP：类型声明与返回类型
来源：http://fo.gzmigu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qk.hnjuh.cn

[U46] PHP：可空类型
来源：http://ll.lnxyls.cn

?string $name = null
来源：http://tb.nicolike.cn

[U47] PHP：联合类型
来源：http://vh.colortex.cn

int|string $id
来源：http://ay.jctech888.com.cn

[U48] PHP：纯枚举
来源：http://gn.lnxyls.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ho.colortex.cn

[U49] PHP：只读属性
来源：http://to.asd995.cn

public readonly string $name
来源：http://bd.chemitech.net.cn

[U50] PHP：构造器属性提升
来源：http://om.asd995.cn

public function __construct(private int $id) {}
来源：http://nv.yuntaijiaju.cn

[U51] PHP：数组解构
来源：http://ry.wgjwhj.cn

[$a, $b] = $arr;
来源：http://yi.muxihuayi.cn

[U52] PHP：箭头函数
来源：http://gt.shxzskj.cn

$double = fn($x) => $x * 2;
来源：http://fp.bookmarksfly.cn

[U53] PHP：空合并运算符
来源：http://uk.wgjwhj.cn

$v = $a ?? $b ?? "default";
来源：http://kb.muxihuayi.cn

[U54] PHP：空安全调用
来源：http://md.nszjky.cn

$obj?->method()
来源：http://tc.hnjuh.cn

[U55] PHP：match 表达式
来源：http://jx.9csxet.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uz.szsharing.cn

[U56] PHP：命名参数
来源：http://mu.521024.cn

f(a: 1, b: 2)
来源：http://qn.hnjuh.cn

[U57] PHP：字符串插值
来源：http://dr.nszjky.cn

"值: {$a}"
来源：http://hr.shxzukj.cn

[U58] PHP：数组三件套
来源：http://ui.yuexingan06.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://st.521024.cn

[U59] PHP：自定义排序
来源：http://sr.asd995.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xm.huanxung.cn

[U60] PHP：JSON 编解码
来源：http://yp.haigaiapp.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vr.hnjuh.cn

[U61] PHP：正则
来源：http://qm.szsharing.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dw.jianghongdianzi.cn

[U62] PHP：日期对象
来源：http://qw.jctech888.com.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bl.shtwfgs.cn

[U63] PHP：文件读写
来源：http://iy.lnxyls.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hx.huanxung.cn

[U64] PHP：目录遍历
来源：http://uc.shtwfgs.cn

glob("dir/*.php");  scandir("dir");
来源：http://ie.shxzskj.cn

[U65] PHP：会话
来源：http://ce.9csxet.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://qd.panjiajie.cn

[U66] PHP：设置 Cookie
来源：http://yn.huixinmuqiang.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tb.chemitech.net.cn

[U67] PHP：处理文件上传
来源：http://jr.bjjhwx.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://aq.szxytkj.cn

[U68] PHP：PDO 连接
来源：http://tq.yuntaijiaju.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jg.gzmigu.cn

[U69] PHP：PDO 预处理
来源：http://tv.shtwfgs.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dm.huixiangedu.cn

[U70] PHP：PDO 事务
来源：http://vx.lnxyls.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ra.yuexingan06.cn

[U71] PHP：抛出异常
来源：http://vp.colortex.cn

throw new RuntimeException("失败", 500);
来源：http://ar.wgjwhj.cn

[U72] PHP：写错误日志
来源：http://hv.szxytkj.cn

error_log("失败: " . $e->getMessage());
来源：http://om.hahajie.cn

[U73] PHP：读取 ini 配置
来源：http://qz.colortex.cn

parse_ini_file("config.ini", true)
来源：http://kz.shtwfgs.cn

[U74] PHP：读取环境变量
来源：http://dn.shtwfgs.cn

getenv("APP_ENV") ?: "production"
来源：http://mg.szxytkj.cn

[U75] PHP：依赖注入
来源：http://cu.huixinmuqiang.cn

composer require psr/container
来源：http://wg.bjjhwx.cn

[U76] PHP：简单路由
来源：http://cr.hahajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xf.9csxet.cn

[U77] PHP：模板渲染
来源：http://jx.muxihuayi.cn

composer require twig/twig
来源：http://nu.gzmigu.cn

[U78] PHP：单元测试
来源：http://oy.huixinmuqiang.cn

composer require --dev phpunit/phpunit
来源：http://wf.huixinmuqiang.cn

[U79] PHP：静态分析
来源：http://yt.asd995.cn

composer require --dev phpstan/phpstan
来源：http://hi.jianghongdianzi.cn

[U80] PHP：代码规范修复
来源：http://nh.haigaiapp.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://gd.wgjwhj.cn

[U81] JS：初始化项目
来源：http://xz.huixinmuqiang.cn

npm init -y;  npm i express
来源：http://xb.huixinmuqiang.cn

[U82] JS：package.json 脚本
来源：http://km.hnjuh.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vy.szsharing.cn

[U83] JS：ES Module 导入导出
来源：http://mn.shxzukj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://wz.521024.cn

[U84] JS：CommonJS 写法
来源：http://as.nszjky.cn

module.exports = { a };  const { a } = require("./m");
来源：http://vj.wgjwhj.cn

[U85] JS：可选链
来源：http://qh.shtwfgs.cn

a?.b?.c
来源：http://br.huixinmuqiang.cn

[U86] JS：空值合并
来源：http://ff.nszjky.cn

a ?? b
来源：http://ci.gzmigu.cn

[U87] JS：解构默认值
来源：http://sr.colortex.cn

const { a = 1, b = 2 } = obj;
来源：http://fa.haigaiapp.cn

[U88] JS：对象展开合并
来源：http://fa.huixiangedu.cn

{ ...a, ...b }
来源：http://ha.lnxyls.cn

[U89] JS：数组去重
来源：http://gm.bjjhwx.cn

[...new Set(arr)]
来源：http://vy.hahajie.cn

[U90] JS：数字数组排序
来源：http://zi.lnxyls.cn

[...arr].sort((a, b) => a - b)
来源：http://qp.asd995.cn

[U91] JS：对象键值遍历
来源：http://mc.wgjwhj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://co.haigaiapp.cn

[U92] JS：深拷贝
来源：http://fn.9csxet.cn

structuredClone(obj)
来源：http://bl.szxytkj.cn

[U93] JS：模板字符串
来源：http://na.colortex.cn

`共 ${n} 条`
来源：http://zh.wgjwhj.cn

[U94] JS：箭头函数
来源：http://rn.nicolike.cn

const double = x => x * 2;
来源：http://ir.szxytkj.cn

[U95] JS：Promise 包装
来源：http://rn.chemitech.net.cn

new Promise((resolve, reject) => {})
来源：http://zw.gzmigu.cn

[U96] JS：async/await 与异常
来源：http://ly.hahajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ap.nszjky.cn

[U97] JS：并发请求
来源：http://sa.bjjhwx.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://wg.yuntaijiaju.cn

[U98] JS：fetch 带 JSON
来源：http://nq.shtwfgs.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qa.muxihuayi.cn

[U99] JS：事件监听
来源：http://to.huixiangedu.cn

el.addEventListener("click", e => {})
来源：http://hn.bjjhwx.cn

[U100] JS：DOM 查询
来源：http://qq.jianghongdianzi.cn

document.querySelector(".item")
来源：http://vu.szsharing.cn

[U101] JS：classList 操作
来源：http://xo.asd995.cn

el.classList.toggle("active")
来源：http://em.lnxyls.cn

[U102] JS：本地存储
来源：http://jt.yuexingan06.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jw.wgjwhj.cn

[U103] JS：定时器
来源：http://sg.yuexingan06.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kp.nicolike.cn

[U104] JS：防抖
来源：http://gw.huanxung.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bn.hahajie.cn

[U105] JS：节流
来源：http://fe.nszjky.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lv.nicolike.cn

[U106] JS：日期格式化
来源：http://qn.lnxyls.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zj.huixiangedu.cn

[U107] JS：数字千分位
来源：http://mv.shtwfgs.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ws.huanxung.cn

[U108] JS：随机整数
来源：http://te.shxzskj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ko.huixiangedu.cn

[U109] JS：数组分组
来源：http://sl.hnjuh.cn

Object.groupBy(arr, x => x.type)
来源：http://sy.9csxet.cn

[U110] JS：数组分块
来源：http://gl.yuexingan06.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://av.newstarts.cn

[U111] JS：对象转 Map
来源：http://ec.nszjky.cn

new Map(Object.entries(obj))
来源：http://zi.hnjuh.cn

[U112] JS：字符串补位
来源：http://zw.nicolike.cn

"7".padStart(3, "0")
来源：http://xc.9csxet.cn

[U113] JS：正则替换全部
来源：http://vi.bookmarksfly.cn

s.replaceAll("a", "b")
来源：http://jc.colortex.cn

[U114] JS：JSON 深比较
来源：http://ep.nszjky.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ad.gzmigu.cn

[U115] JS：生成 UUID
来源：http://su.wgjwhj.cn

crypto.randomUUID()
来源：http://mx.huixinmuqiang.cn

[U116] JS：类型检查（JSDoc）
来源：http://bp.shtwfgs.cn

/** @param {string} name */ function f(name) {}
来源：http://av.hahajie.cn

[U117] JS：单元测试
来源：http://sx.szsharing.cn

npm i -D vitest;  npx vitest
来源：http://jq.huixinmuqiang.cn

[U118] JS：开发服务器
来源：http://uv.chemitech.net.cn

npm i -D vite;  npx vite
来源：http://as.szxytkj.cn

[U119] JS：生产构建
来源：http://hi.hahajie.cn

npx vite build
来源：http://lc.huixiangedu.cn

[U120] JS：读取环境变量（Vite）
来源：http://gc.jianghongdianzi.cn

import.meta.env.VITE_API_URL
来源：http://su.huanxung.cn

================================================================================
来源：http://oc.9csxet.cn

统计汇总
来源：http://gt.chemitech.net.cn

================================================================================
来源：http://ol.nszjky.cn

按语言统计（条）：
来源：http://ws.nicolike.cn

Python ......... 252
来源：http://ag.hnjuh.cn

PHP ............ 252
来源：http://cy.huixinmuqiang.cn

JavaScript ..... 252
来源：http://aw.shtwfgs.cn

TypeScript ..... 212
来源：http://zq.bjjhwx.cn

Java ........... 212
来源：http://cj.szxytkj.cn

Go ............. 212
来源：http://zn.panjiajie.cn

Ruby ........... 212
来源：http://gt.jctech888.com.cn

C# ............. 212
来源：http://kn.chemitech.net.cn

C .............. 30
来源：http://ac.bjjhwx.cn

C++ ............ 30
来源：http://on.jianghongdianzi.cn

SQL ............ 90
来源：http://ps.bjjhwx.cn

Bash ........... 80
来源：http://na.huanxung.cn

Kotlin ......... 15
来源：http://on.wgjwhj.cn

Swift .......... 15
来源：http://fb.lnxyls.cn

Lua ............ 10
来源：http://oi.wgjwhj.cn

Perl ........... 10
来源：http://lm.lnxyls.cn

Scala .......... 10
来源：http://ol.szxytkj.cn

------------------------------------
来源：http://jl.jctech888.com.cn

合计 ........... 2106 条
来源：http://nt.newstarts.cn

按章节统计：
来源：http://kr.asd995.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lo.hnjuh.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kf.shxzukj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tl.shtwfgs.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gd.yuexingan06.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zs.521024.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zf.jctech888.com.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cc.colortex.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gl.asd995.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ur.huixinmuqiang.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wm.lnxyls.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://oc.huixinmuqiang.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qf.haigaiapp.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://cm.gzmigu.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sn.yuexingan06.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ez.newstarts.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wg.hnjuh.cn

Q SQL 专题                              90
来源：http://mt.szsharing.cn

R Bash 专题                             80
来源：http://mc.wgjwhj.cn

S C / C++ 专题                          60
来源：http://ac.huixinmuqiang.cn

T 其他语言补充                          60
来源：http://or.szsharing.cn

U 高频实用片段                         120
来源：http://or.9csxet.cn

------------------------------------
来源：http://av.jctech888.com.cn

合计                                  2106 条
来源：http://sj.hahajie.cn

--------------------------------------------------------------------------------
来源：http://sb.panjiajie.cn

使用提醒
来源：http://rl.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://rd.colortex.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nm.521024.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ma.chemitech.net.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://us.shxzukj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://nt.shxzskj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gw.szxytkj.cn

—— 文件结束 ——
来源：http://vd.muxihuayi.cn

================================================================================
来源：http://dm.bjjhwx.cn

程序语言常见例子速查手册（2024 版）
来源：http://ax.huixinmuqiang.cn

Common Programming Examples Cheat Book
来源：http://pm.521024.cn

================================================================================
来源：http://iq.nicolike.cn

【收录内容】
来源：http://gf.szsharing.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://du.hnjuh.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tm.nszjky.cn

SQL · Bash · C · C++
来源：http://dn.nicolike.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://no.haigaiapp.cn

【使用说明】
来源：http://yo.asd995.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wj.521024.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ru.jctech888.com.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qn.bjjhwx.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://tj.wgjwhj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ss.huanxung.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xz.szxytkj.cn


<!-- 参考信息 -->