代发 wailian999

[U15] Py：高精度计时
来源：http://wy.lnxyls.cn

t = time.perf_counter()
来源：http://me.yuexingan06.cn

[U16] Py：命令行参数解析
来源：http://bs.huanxung.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mf.yuexingan06.cn

[U17] Py：初始化日志
来源：http://nt.lnxyls.cn

logging.basicConfig(level=logging.INFO)
来源：http://jx.yuntaijiaju.cn

[U18] Py：预编译正则
来源：http://xl.hahajie.cn

pat = re.compile(r"\d+")
来源：http://vg.yuntaijiaju.cn

[U19] Py：正则替换带回调
来源：http://xf.nszjky.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ec.yuexingan06.cn

[U20] Py：缓存函数结果
来源：http://rq.bjjhwx.cn

@functools.lru_cache(maxsize=None)
来源：http://zk.gzmigu.cn

[U21] Py：自定义上下文管理器
来源：http://kq.szxytkj.cn

@contextlib.contextmanager
来源：http://vk.yuexingan06.cn

[U22] Py：矩阵转置
来源：http://uo.bjjhwx.cn

list(zip(*m))
来源：http://ln.hnjuh.cn

[U23] Py：分块读取大文件
来源：http://vs.huixinmuqiang.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ed.shxzukj.cn

[U24] Py：路径操作
来源：http://gs.hahajie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://on.colortex.cn

[U25] Py：CSV 按字典读
来源：http://tw.shxzukj.cn

csv.DictReader(f)
来源：http://no.chemitech.net.cn

[U26] Py：并发下载
来源：http://cl.bjjhwx.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yl.colortex.cn

[U27] Py：异步 HTTP
来源：http://gc.newstarts.cn

aiohttp.ClientSession() 配合 async with
来源：http://im.bjjhwx.cn

[U28] Py：类型别名
来源：http://if.shxzskj.cn

UserId = int
来源：http://pq.nicolike.cn

[U29] Py：属性校验
来源：http://cx.gzmigu.cn

@property 与 @x.setter 配合
来源：http://rj.bjjhwx.cn

[U30] Py：数据类
来源：http://qq.colortex.cn

@dataclass(slots=True)
来源：http://hv.lnxyls.cn

[U31] Py：单测
来源：http://ng.szxytkj.cn

python -m pytest -q
来源：http://af.shxzukj.cn

[U32] Py：代码格式化
来源：http://iy.jctech888.com.cn

ruff format . && ruff check --fix .
来源：http://rd.bjjhwx.cn

[U33] Py：打包发布
来源：http://dx.newstarts.cn

python -m build  （依赖 pyproject.toml）
来源：http://kd.9csxet.cn

[U34] Py：判断编码
来源：http://rq.colortex.cn

chardet.detect(raw)
来源：http://to.jctech888.com.cn

[U35] Py：发送邮件
来源：http://ws.newstarts.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cv.jianghongdianzi.cn

[U36] Py：定时任务
来源：http://ui.szxytkj.cn

schedule.every(10).minutes.do(job)
来源：http://sa.jctech888.com.cn

[U37] Py：读写 Excel
来源：http://si.chemitech.net.cn

pandas.read_excel / DataFrame.to_excel
来源：http://vl.jianghongdianzi.cn

[U38] Py：获取脚本所在目录
来源：http://bp.shxzskj.cn

Path(__file__).resolve().parent
来源：http://jy.wgjwhj.cn

[U39] Py：判断是否在交互环境
来源：http://pw.nszjky.cn

sys.stdout.isatty()
来源：http://yz.jianghongdianzi.cn

[U40] Py：打印到标准错误
来源：http://aa.shxzukj.cn

print("err", file=sys.stderr)
来源：http://wt.asd995.cn

[U41] PHP：初始化 Composer 项目
来源：http://fr.nszjky.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ik.521024.cn

[U42] PHP：PSR-4 自动加载
来源：http://gg.shtwfgs.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ww.haigaiapp.cn

[U43] PHP：声明命名空间
来源：http://im.nicolike.cn

namespace App\Http;
来源：http://kw.hahajie.cn

[U44] PHP：开启严格类型
来源：http://ov.521024.cn

declare(strict_types=1);
来源：http://cd.jianghongdianzi.cn

[U45] PHP：类型声明与返回类型
来源：http://oj.newstarts.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://hn.lnxyls.cn

[U46] PHP：可空类型
来源：http://mr.chemitech.net.cn

?string $name = null
来源：http://wr.szsharing.cn

[U47] PHP：联合类型
来源：http://ds.9csxet.cn

int|string $id
来源：http://ij.lnxyls.cn

[U48] PHP：纯枚举
来源：http://yk.jianghongdianzi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://er.hnjuh.cn

[U49] PHP：只读属性
来源：http://ys.szsharing.cn

public readonly string $name
来源：http://kp.huanxung.cn

[U50] PHP：构造器属性提升
来源：http://kg.nszjky.cn

public function __construct(private int $id) {}
来源：http://ox.shtwfgs.cn

[U51] PHP：数组解构
来源：http://ua.shtwfgs.cn

[$a, $b] = $arr;
来源：http://cv.chemitech.net.cn

[U52] PHP：箭头函数
来源：http://sw.gzmigu.cn

$double = fn($x) => $x * 2;
来源：http://ep.521024.cn

[U53] PHP：空合并运算符
来源：http://qp.wgjwhj.cn

$v = $a ?? $b ?? "default";
来源：http://pp.lnxyls.cn

[U54] PHP：空安全调用
来源：http://yw.hahajie.cn

$obj?->method()
来源：http://ge.shtwfgs.cn

[U55] PHP：match 表达式
来源：http://qe.haigaiapp.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ll.muxihuayi.cn

[U56] PHP：命名参数
来源：http://ke.asd995.cn

f(a: 1, b: 2)
来源：http://qr.haigaiapp.cn

[U57] PHP：字符串插值
来源：http://er.haigaiapp.cn

"值: {$a}"
来源：http://we.nicolike.cn

[U58] PHP：数组三件套
来源：http://gi.newstarts.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://db.chemitech.net.cn

[U59] PHP：自定义排序
来源：http://jv.shxzskj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gi.hnjuh.cn

[U60] PHP：JSON 编解码
来源：http://wi.colortex.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://em.wgjwhj.cn

[U61] PHP：正则
来源：http://bx.9csxet.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qh.shxzukj.cn

[U62] PHP：日期对象
来源：http://lh.muxihuayi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ge.hnjuh.cn

[U63] PHP：文件读写
来源：http://ek.colortex.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://od.9csxet.cn

[U64] PHP：目录遍历
来源：http://uc.521024.cn

glob("dir/*.php");  scandir("dir");
来源：http://ii.bookmarksfly.cn

[U65] PHP：会话
来源：http://ev.haigaiapp.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://np.jctech888.com.cn

[U66] PHP：设置 Cookie
来源：http://uo.nszjky.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://he.jianghongdianzi.cn

[U67] PHP：处理文件上传
来源：http://uk.colortex.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://in.gzmigu.cn

[U68] PHP：PDO 连接
来源：http://kn.521024.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://sn.haigaiapp.cn

[U69] PHP：PDO 预处理
来源：http://nj.hahajie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hf.bookmarksfly.cn

[U70] PHP：PDO 事务
来源：http://cz.panjiajie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://oa.nicolike.cn

[U71] PHP：抛出异常
来源：http://wn.yuexingan06.cn

throw new RuntimeException("失败", 500);
来源：http://lt.shtwfgs.cn

[U72] PHP：写错误日志
来源：http://pt.hahajie.cn

error_log("失败: " . $e->getMessage());
来源：http://xx.lnxyls.cn

[U73] PHP：读取 ini 配置
来源：http://co.huanxung.cn

parse_ini_file("config.ini", true)
来源：http://io.huixinmuqiang.cn

[U74] PHP：读取环境变量
来源：http://wo.shxzukj.cn

getenv("APP_ENV") ?: "production"
来源：http://ob.szxytkj.cn

[U75] PHP：依赖注入
来源：http://ae.jctech888.com.cn

composer require psr/container
来源：http://hw.newstarts.cn

[U76] PHP：简单路由
来源：http://cx.hahajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://iz.hnjuh.cn

[U77] PHP：模板渲染
来源：http://gf.yuexingan06.cn

composer require twig/twig
来源：http://th.huixinmuqiang.cn

[U78] PHP：单元测试
来源：http://nq.shxzskj.cn

composer require --dev phpunit/phpunit
来源：http://zn.hahajie.cn

[U79] PHP：静态分析
来源：http://hz.chemitech.net.cn

composer require --dev phpstan/phpstan
来源：http://kw.nszjky.cn

[U80] PHP：代码规范修复
来源：http://br.hnjuh.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jm.panjiajie.cn

[U81] JS：初始化项目
来源：http://qv.bookmarksfly.cn

npm init -y;  npm i express
来源：http://vv.hnjuh.cn

[U82] JS：package.json 脚本
来源：http://qf.chemitech.net.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mc.nicolike.cn

[U83] JS：ES Module 导入导出
来源：http://xi.9csxet.cn

export const a = 1;  import { a } from "./m.js";
来源：http://gt.nszjky.cn

[U84] JS：CommonJS 写法
来源：http://xw.panjiajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://go.gzmigu.cn

[U85] JS：可选链
来源：http://gl.wgjwhj.cn

a?.b?.c
来源：http://cs.haigaiapp.cn

[U86] JS：空值合并
来源：http://zh.asd995.cn

a ?? b
来源：http://nz.huanxung.cn

[U87] JS：解构默认值
来源：http://oz.yuntaijiaju.cn

const { a = 1, b = 2 } = obj;
来源：http://vo.colortex.cn

[U88] JS：对象展开合并
来源：http://xt.colortex.cn

{ ...a, ...b }
来源：http://gx.panjiajie.cn

[U89] JS：数组去重
来源：http://hc.haigaiapp.cn

[...new Set(arr)]
来源：http://li.jianghongdianzi.cn

[U90] JS：数字数组排序
来源：http://dr.panjiajie.cn

[...arr].sort((a, b) => a - b)
来源：http://vv.chemitech.net.cn

[U91] JS：对象键值遍历
来源：http://zu.jianghongdianzi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://sx.huanxung.cn

[U92] JS：深拷贝
来源：http://hp.bjjhwx.cn

structuredClone(obj)
来源：http://ku.lnxyls.cn

[U93] JS：模板字符串
来源：http://ft.newstarts.cn

`共 ${n} 条`
来源：http://us.wgjwhj.cn

[U94] JS：箭头函数
来源：http://bg.haigaiapp.cn

const double = x => x * 2;
来源：http://tj.nszjky.cn

[U95] JS：Promise 包装
来源：http://od.shxzukj.cn

new Promise((resolve, reject) => {})
来源：http://tq.haigaiapp.cn

[U96] JS：async/await 与异常
来源：http://gk.jianghongdianzi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vw.colortex.cn

[U97] JS：并发请求
来源：http://ay.colortex.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://mz.shtwfgs.cn

[U98] JS：fetch 带 JSON
来源：http://qm.hnjuh.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hh.521024.cn

[U99] JS：事件监听
来源：http://fz.szsharing.cn

el.addEventListener("click", e => {})
来源：http://ci.panjiajie.cn

[U100] JS：DOM 查询
来源：http://zz.wgjwhj.cn

document.querySelector(".item")
来源：http://oc.jianghongdianzi.cn

[U101] JS：classList 操作
来源：http://sc.muxihuayi.cn

el.classList.toggle("active")
来源：http://zi.wgjwhj.cn

[U102] JS：本地存储
来源：http://wg.bjjhwx.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://zi.bjjhwx.cn

[U103] JS：定时器
来源：http://nv.panjiajie.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vs.panjiajie.cn

[U104] JS：防抖
来源：http://em.huixiangedu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xx.szsharing.cn

[U105] JS：节流
来源：http://gx.asd995.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rl.hnjuh.cn

[U106] JS：日期格式化
来源：http://zt.gzmigu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bc.jianghongdianzi.cn

[U107] JS：数字千分位
来源：http://nd.panjiajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uk.huixinmuqiang.cn

[U108] JS：随机整数
来源：http://gj.shxzukj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ct.nszjky.cn

[U109] JS：数组分组
来源：http://ev.yuexingan06.cn

Object.groupBy(arr, x => x.type)
来源：http://ic.huixiangedu.cn

[U110] JS：数组分块
来源：http://gg.muxihuayi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tt.hnjuh.cn

[U111] JS：对象转 Map
来源：http://wm.hahajie.cn

new Map(Object.entries(obj))
来源：http://oa.szsharing.cn

[U112] JS：字符串补位
来源：http://qu.nicolike.cn

"7".padStart(3, "0")
来源：http://pg.chemitech.net.cn

[U113] JS：正则替换全部
来源：http://lj.chemitech.net.cn

s.replaceAll("a", "b")
来源：http://jy.shxzukj.cn

[U114] JS：JSON 深比较
来源：http://bs.colortex.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://su.jctech888.com.cn

[U115] JS：生成 UUID
来源：http://uz.jianghongdianzi.cn

crypto.randomUUID()
来源：http://lh.haigaiapp.cn

[U116] JS：类型检查（JSDoc）
来源：http://kl.nszjky.cn

/** @param {string} name */ function f(name) {}
来源：http://fz.panjiajie.cn

[U117] JS：单元测试
来源：http://px.lnxyls.cn

npm i -D vitest;  npx vitest
来源：http://cf.yuntaijiaju.cn

[U118] JS：开发服务器
来源：http://uw.jctech888.com.cn

npm i -D vite;  npx vite
来源：http://tv.hnjuh.cn

[U119] JS：生产构建
来源：http://em.shtwfgs.cn

npx vite build
来源：http://oc.shxzskj.cn

[U120] JS：读取环境变量（Vite）
来源：http://vj.521024.cn

import.meta.env.VITE_API_URL
来源：http://bw.lnxyls.cn

================================================================================
来源：http://gq.bjjhwx.cn

统计汇总
来源：http://pn.jianghongdianzi.cn

================================================================================
来源：http://ht.wgjwhj.cn

按语言统计（条）：
来源：http://uv.huanxung.cn

Python ......... 252
来源：http://ki.shxzskj.cn

PHP ............ 252
来源：http://qz.9csxet.cn

JavaScript ..... 252
来源：http://hv.lnxyls.cn

TypeScript ..... 212
来源：http://cv.panjiajie.cn

Java ........... 212
来源：http://yt.newstarts.cn

Go ............. 212
来源：http://ou.9csxet.cn

Ruby ........... 212
来源：http://jz.shtwfgs.cn

C# ............. 212
来源：http://uc.shxzskj.cn

C .............. 30
来源：http://ev.lnxyls.cn

C++ ............ 30
来源：http://vm.yuexingan06.cn

SQL ............ 90
来源：http://kq.shtwfgs.cn

Bash ........... 80
来源：http://nj.huixinmuqiang.cn

Kotlin ......... 15
来源：http://cs.nicolike.cn

Swift .......... 15
来源：http://ai.huixinmuqiang.cn

Lua ............ 10
来源：http://pu.szsharing.cn

Perl ........... 10
来源：http://xa.colortex.cn

Scala .......... 10
来源：http://vr.lnxyls.cn

------------------------------------
来源：http://do.panjiajie.cn

合计 ........... 2106 条
来源：http://au.bookmarksfly.cn

按章节统计：
来源：http://yk.huanxung.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://of.shxzukj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://na.bookmarksfly.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qn.haigaiapp.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qm.yuexingan06.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://by.szsharing.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mq.yuntaijiaju.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vw.bjjhwx.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://sk.huanxung.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ng.huixinmuqiang.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vs.newstarts.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bu.huanxung.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://uw.muxihuayi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nz.szsharing.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ji.colortex.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://is.haigaiapp.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tg.jctech888.com.cn

Q SQL 专题                              90
来源：http://xd.shxzukj.cn

R Bash 专题                             80
来源：http://gl.huanxung.cn

S C / C++ 专题                          60
来源：http://sl.bjjhwx.cn

T 其他语言补充                          60
来源：http://os.hnjuh.cn

U 高频实用片段                         120
来源：http://rs.panjiajie.cn

------------------------------------
来源：http://jx.chemitech.net.cn

合计                                  2106 条
来源：http://ja.colortex.cn

--------------------------------------------------------------------------------
来源：http://yi.newstarts.cn

使用提醒
来源：http://ts.nszjky.cn

--------------------------------------------------------------------------------
来源：http://dx.yuexingan06.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lc.colortex.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rw.shtwfgs.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://dz.hnjuh.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://pu.szsharing.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://uh.jianghongdianzi.cn

—— 文件结束 ——
来源：http://ds.muxihuayi.cn

================================================================================
来源：http://rh.jctech888.com.cn

程序语言常见例子速查手册（2024 版）
来源：http://vl.wgjwhj.cn

Common Programming Examples Cheat Book
来源：http://vk.bjjhwx.cn

================================================================================
来源：http://bo.yuexingan06.cn

【收录内容】
来源：http://jo.szsharing.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://rn.szsharing.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hr.huanxung.cn

SQL · Bash · C · C++
来源：http://rt.lnxyls.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://oa.jianghongdianzi.cn

【使用说明】
来源：http://hu.gzmigu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://sv.asd995.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://sa.shtwfgs.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lz.shxzskj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://tc.chemitech.net.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://yr.jctech888.com.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://cz.bjjhwx.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://to.newstarts.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nf.hahajie.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://re.jctech888.com.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fm.szsharing.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://cn.jianghongdianzi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://sb.huixiangedu.cn

【文件统计】
来源：http://ig.panjiajie.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vu.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://nm.9csxet.cn

目  录
来源：http://gc.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://np.nszjky.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fx.gzmigu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bd.jianghongdianzi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fu.huanxung.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fv.huixinmuqiang.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://pi.huixiangedu.cn


<!-- 参考信息 -->