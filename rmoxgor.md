代发 wailian999

[U15] Py：高精度计时
来源：http://dz.newstarts.cn

t = time.perf_counter()
来源：http://pq.panjiajie.cn

[U16] Py：命令行参数解析
来源：http://cz.panjiajie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://en.hahajie.cn

[U17] Py：初始化日志
来源：http://zu.jianghongdianzi.cn

logging.basicConfig(level=logging.INFO)
来源：http://vx.bjjhwx.cn

[U18] Py：预编译正则
来源：http://bc.jianghongdianzi.cn

pat = re.compile(r"\d+")
来源：http://xg.nszjky.cn

[U19] Py：正则替换带回调
来源：http://bg.521024.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ax.colortex.cn

[U20] Py：缓存函数结果
来源：http://gd.gzmigu.cn

@functools.lru_cache(maxsize=None)
来源：http://ml.hahajie.cn

[U21] Py：自定义上下文管理器
来源：http://zn.yuexingan06.cn

@contextlib.contextmanager
来源：http://wt.asd995.cn

[U22] Py：矩阵转置
来源：http://bt.bjjhwx.cn

list(zip(*m))
来源：http://sq.jianghongdianzi.cn

[U23] Py：分块读取大文件
来源：http://mc.yuexingan06.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cw.shxzskj.cn

[U24] Py：路径操作
来源：http://iw.colortex.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vm.asd995.cn

[U25] Py：CSV 按字典读
来源：http://hv.nszjky.cn

csv.DictReader(f)
来源：http://pg.wgjwhj.cn

[U26] Py：并发下载
来源：http://rz.nszjky.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nu.lnxyls.cn

[U27] Py：异步 HTTP
来源：http://mj.szxytkj.cn

aiohttp.ClientSession() 配合 async with
来源：http://gi.bjjhwx.cn

[U28] Py：类型别名
来源：http://lb.bjjhwx.cn

UserId = int
来源：http://ki.huixiangedu.cn

[U29] Py：属性校验
来源：http://lf.huixiangedu.cn

@property 与 @x.setter 配合
来源：http://xl.hnjuh.cn

[U30] Py：数据类
来源：http://zf.521024.cn

@dataclass(slots=True)
来源：http://ta.nszjky.cn

[U31] Py：单测
来源：http://uw.muxihuayi.cn

python -m pytest -q
来源：http://kg.colortex.cn

[U32] Py：代码格式化
来源：http://fj.yuntaijiaju.cn

ruff format . && ruff check --fix .
来源：http://uh.lnxyls.cn

[U33] Py：打包发布
来源：http://rg.jctech888.com.cn

python -m build  （依赖 pyproject.toml）
来源：http://tq.newstarts.cn

[U34] Py：判断编码
来源：http://sh.nszjky.cn

chardet.detect(raw)
来源：http://jl.521024.cn

[U35] Py：发送邮件
来源：http://ln.yuntaijiaju.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rf.521024.cn

[U36] Py：定时任务
来源：http://ig.nszjky.cn

schedule.every(10).minutes.do(job)
来源：http://ds.szxytkj.cn

[U37] Py：读写 Excel
来源：http://os.9csxet.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ho.szsharing.cn

[U38] Py：获取脚本所在目录
来源：http://jc.asd995.cn

Path(__file__).resolve().parent
来源：http://ss.bjjhwx.cn

[U39] Py：判断是否在交互环境
来源：http://gf.9csxet.cn

sys.stdout.isatty()
来源：http://co.wgjwhj.cn

[U40] Py：打印到标准错误
来源：http://vi.bookmarksfly.cn

print("err", file=sys.stderr)
来源：http://cq.lnxyls.cn

[U41] PHP：初始化 Composer 项目
来源：http://ez.gzmigu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://af.shxzukj.cn

[U42] PHP：PSR-4 自动加载
来源：http://uc.nszjky.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hr.gzmigu.cn

[U43] PHP：声明命名空间
来源：http://rc.huanxung.cn

namespace App\Http;
来源：http://nd.shxzukj.cn

[U44] PHP：开启严格类型
来源：http://xw.szsharing.cn

declare(strict_types=1);
来源：http://ci.asd995.cn

[U45] PHP：类型声明与返回类型
来源：http://bh.shtwfgs.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://zr.chemitech.net.cn

[U46] PHP：可空类型
来源：http://wq.nszjky.cn

?string $name = null
来源：http://kk.bookmarksfly.cn

[U47] PHP：联合类型
来源：http://kt.shxzskj.cn

int|string $id
来源：http://pt.haigaiapp.cn

[U48] PHP：纯枚举
来源：http://gi.jianghongdianzi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ea.haigaiapp.cn

[U49] PHP：只读属性
来源：http://ro.gzmigu.cn

public readonly string $name
来源：http://os.huixinmuqiang.cn

[U50] PHP：构造器属性提升
来源：http://to.gzmigu.cn

public function __construct(private int $id) {}
来源：http://pg.yuntaijiaju.cn

[U51] PHP：数组解构
来源：http://ok.haigaiapp.cn

[$a, $b] = $arr;
来源：http://ip.szxytkj.cn

[U52] PHP：箭头函数
来源：http://pv.shtwfgs.cn

$double = fn($x) => $x * 2;
来源：http://up.shxzukj.cn

[U53] PHP：空合并运算符
来源：http://pc.jctech888.com.cn

$v = $a ?? $b ?? "default";
来源：http://rz.bjjhwx.cn

[U54] PHP：空安全调用
来源：http://xp.newstarts.cn

$obj?->method()
来源：http://ec.shxzukj.cn

[U55] PHP：match 表达式
来源：http://aw.shtwfgs.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://if.bjjhwx.cn

[U56] PHP：命名参数
来源：http://ph.nicolike.cn

f(a: 1, b: 2)
来源：http://as.muxihuayi.cn

[U57] PHP：字符串插值
来源：http://id.colortex.cn

"值: {$a}"
来源：http://vu.jctech888.com.cn

[U58] PHP：数组三件套
来源：http://ae.shtwfgs.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pc.9csxet.cn

[U59] PHP：自定义排序
来源：http://au.shtwfgs.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ee.shtwfgs.cn

[U60] PHP：JSON 编解码
来源：http://wu.nicolike.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ta.yuexingan06.cn

[U61] PHP：正则
来源：http://mz.szsharing.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mu.colortex.cn

[U62] PHP：日期对象
来源：http://qg.hahajie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vd.szxytkj.cn

[U63] PHP：文件读写
来源：http://ky.jianghongdianzi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ea.newstarts.cn

[U64] PHP：目录遍历
来源：http://td.szxytkj.cn

glob("dir/*.php");  scandir("dir");
来源：http://re.9csxet.cn

[U65] PHP：会话
来源：http://vw.szxytkj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://er.nicolike.cn

[U66] PHP：设置 Cookie
来源：http://dq.panjiajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gc.yuntaijiaju.cn

[U67] PHP：处理文件上传
来源：http://cg.jianghongdianzi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pb.shtwfgs.cn

[U68] PHP：PDO 连接
来源：http://hf.newstarts.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nk.nszjky.cn

[U69] PHP：PDO 预处理
来源：http://xq.jianghongdianzi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cp.asd995.cn

[U70] PHP：PDO 事务
来源：http://fc.newstarts.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://id.szxytkj.cn

[U71] PHP：抛出异常
来源：http://bj.nicolike.cn

throw new RuntimeException("失败", 500);
来源：http://yy.nicolike.cn

[U72] PHP：写错误日志
来源：http://af.chemitech.net.cn

error_log("失败: " . $e->getMessage());
来源：http://bz.panjiajie.cn

[U73] PHP：读取 ini 配置
来源：http://jq.jctech888.com.cn

parse_ini_file("config.ini", true)
来源：http://ur.jianghongdianzi.cn

[U74] PHP：读取环境变量
来源：http://bx.panjiajie.cn

getenv("APP_ENV") ?: "production"
来源：http://ny.bookmarksfly.cn

[U75] PHP：依赖注入
来源：http://fp.newstarts.cn

composer require psr/container
来源：http://fl.nszjky.cn

[U76] PHP：简单路由
来源：http://ed.colortex.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://so.szxytkj.cn

[U77] PHP：模板渲染
来源：http://ts.chemitech.net.cn

composer require twig/twig
来源：http://pc.huanxung.cn

[U78] PHP：单元测试
来源：http://mh.haigaiapp.cn

composer require --dev phpunit/phpunit
来源：http://pw.521024.cn

[U79] PHP：静态分析
来源：http://df.panjiajie.cn

composer require --dev phpstan/phpstan
来源：http://pw.hahajie.cn

[U80] PHP：代码规范修复
来源：http://sa.colortex.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://yj.wgjwhj.cn

[U81] JS：初始化项目
来源：http://ji.521024.cn

npm init -y;  npm i express
来源：http://mh.521024.cn

[U82] JS：package.json 脚本
来源：http://xg.haigaiapp.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ah.asd995.cn

[U83] JS：ES Module 导入导出
来源：http://hl.huixiangedu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qt.shtwfgs.cn

[U84] JS：CommonJS 写法
来源：http://hj.hnjuh.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wa.yuntaijiaju.cn

[U85] JS：可选链
来源：http://gd.shtwfgs.cn

a?.b?.c
来源：http://su.huixiangedu.cn

[U86] JS：空值合并
来源：http://rc.bjjhwx.cn

a ?? b
来源：http://kn.shtwfgs.cn

[U87] JS：解构默认值
来源：http://lh.hnjuh.cn

const { a = 1, b = 2 } = obj;
来源：http://qv.huixinmuqiang.cn

[U88] JS：对象展开合并
来源：http://qv.huixinmuqiang.cn

{ ...a, ...b }
来源：http://pq.9csxet.cn

[U89] JS：数组去重
来源：http://rt.lnxyls.cn

[...new Set(arr)]
来源：http://og.wgjwhj.cn

[U90] JS：数字数组排序
来源：http://lu.jctech888.com.cn

[...arr].sort((a, b) => a - b)
来源：http://hw.nicolike.cn

[U91] JS：对象键值遍历
来源：http://uy.521024.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://sb.huanxung.cn

[U92] JS：深拷贝
来源：http://mk.shxzukj.cn

structuredClone(obj)
来源：http://jg.huanxung.cn

[U93] JS：模板字符串
来源：http://ag.bjjhwx.cn

`共 ${n} 条`
来源：http://yr.bookmarksfly.cn

[U94] JS：箭头函数
来源：http://uc.muxihuayi.cn

const double = x => x * 2;
来源：http://ew.huixiangedu.cn

[U95] JS：Promise 包装
来源：http://ic.nicolike.cn

new Promise((resolve, reject) => {})
来源：http://rp.yuexingan06.cn

[U96] JS：async/await 与异常
来源：http://iz.newstarts.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vp.chemitech.net.cn

[U97] JS：并发请求
来源：http://vc.bjjhwx.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://xd.shtwfgs.cn

[U98] JS：fetch 带 JSON
来源：http://it.yuexingan06.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cf.szxytkj.cn

[U99] JS：事件监听
来源：http://gf.yuntaijiaju.cn

el.addEventListener("click", e => {})
来源：http://eo.9csxet.cn

[U100] JS：DOM 查询
来源：http://tl.chemitech.net.cn

document.querySelector(".item")
来源：http://jh.muxihuayi.cn

[U101] JS：classList 操作
来源：http://em.chemitech.net.cn

el.classList.toggle("active")
来源：http://ar.shtwfgs.cn

[U102] JS：本地存储
来源：http://bb.bjjhwx.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://mq.521024.cn

[U103] JS：定时器
来源：http://hk.shxzukj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://oc.szsharing.cn

[U104] JS：防抖
来源：http://xl.9csxet.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uq.bjjhwx.cn

[U105] JS：节流
来源：http://or.asd995.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jl.jctech888.com.cn

[U106] JS：日期格式化
来源：http://gj.szsharing.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cc.gzmigu.cn

[U107] JS：数字千分位
来源：http://dz.jianghongdianzi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mb.huixiangedu.cn

[U108] JS：随机整数
来源：http://kb.haigaiapp.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zl.chemitech.net.cn

[U109] JS：数组分组
来源：http://sb.szxytkj.cn

Object.groupBy(arr, x => x.type)
来源：http://yd.szsharing.cn

[U110] JS：数组分块
来源：http://zw.521024.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vq.haigaiapp.cn

[U111] JS：对象转 Map
来源：http://vd.panjiajie.cn

new Map(Object.entries(obj))
来源：http://if.haigaiapp.cn

[U112] JS：字符串补位
来源：http://yz.huixinmuqiang.cn

"7".padStart(3, "0")
来源：http://nn.jianghongdianzi.cn

[U113] JS：正则替换全部
来源：http://up.colortex.cn

s.replaceAll("a", "b")
来源：http://ch.bookmarksfly.cn

[U114] JS：JSON 深比较
来源：http://ta.shtwfgs.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hl.yuntaijiaju.cn

[U115] JS：生成 UUID
来源：http://vv.haigaiapp.cn

crypto.randomUUID()
来源：http://io.chemitech.net.cn

[U116] JS：类型检查（JSDoc）
来源：http://vt.yuntaijiaju.cn

/** @param {string} name */ function f(name) {}
来源：http://ge.huixiangedu.cn

[U117] JS：单元测试
来源：http://re.szsharing.cn

npm i -D vitest;  npx vitest
来源：http://om.lnxyls.cn

[U118] JS：开发服务器
来源：http://bj.jianghongdianzi.cn

npm i -D vite;  npx vite
来源：http://hv.huanxung.cn

[U119] JS：生产构建
来源：http://vv.huixinmuqiang.cn

npx vite build
来源：http://zc.shxzskj.cn

[U120] JS：读取环境变量（Vite）
来源：http://im.bjjhwx.cn

import.meta.env.VITE_API_URL
来源：http://kx.haigaiapp.cn

================================================================================
来源：http://ld.chemitech.net.cn

统计汇总
来源：http://tb.szsharing.cn

================================================================================
来源：http://fs.521024.cn

按语言统计（条）：
来源：http://mi.yuexingan06.cn

Python ......... 252
来源：http://bz.nicolike.cn

PHP ............ 252
来源：http://ln.asd995.cn

JavaScript ..... 252
来源：http://mj.nszjky.cn

TypeScript ..... 212
来源：http://ji.jctech888.com.cn

Java ........... 212
来源：http://dn.9csxet.cn

Go ............. 212
来源：http://do.jctech888.com.cn

Ruby ........... 212
来源：http://gh.wgjwhj.cn

C# ............. 212
来源：http://dd.asd995.cn

C .............. 30
来源：http://td.huixiangedu.cn

C++ ............ 30
来源：http://zc.haigaiapp.cn

SQL ............ 90
来源：http://iv.huanxung.cn

Bash ........... 80
来源：http://jj.asd995.cn

Kotlin ......... 15
来源：http://zy.hahajie.cn

Swift .......... 15
来源：http://pr.huixinmuqiang.cn

Lua ............ 10
来源：http://kp.huixinmuqiang.cn

Perl ........... 10
来源：http://qg.yuntaijiaju.cn

Scala .......... 10
来源：http://xw.huixiangedu.cn

------------------------------------
来源：http://vp.huixiangedu.cn

合计 ........... 2106 条
来源：http://sn.szxytkj.cn

按章节统计：
来源：http://yy.yuexingan06.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lv.bookmarksfly.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gj.szsharing.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wt.newstarts.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://br.jianghongdianzi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ek.hahajie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kg.huixiangedu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ec.huanxung.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xl.gzmigu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qg.wgjwhj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://pw.bjjhwx.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wl.hnjuh.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pv.yuntaijiaju.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jy.huanxung.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bw.huixiangedu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://di.yuntaijiaju.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ar.jctech888.com.cn

Q SQL 专题                              90
来源：http://ny.jianghongdianzi.cn

R Bash 专题                             80
来源：http://dv.szxytkj.cn

S C / C++ 专题                          60
来源：http://nq.shxzskj.cn

T 其他语言补充                          60
来源：http://yf.9csxet.cn

U 高频实用片段                         120
来源：http://uq.huixiangedu.cn

------------------------------------
来源：http://lr.huixiangedu.cn

合计                                  2106 条
来源：http://yd.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://xw.colortex.cn

使用提醒
来源：http://dr.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://je.9csxet.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://el.9csxet.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vm.lnxyls.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qn.wgjwhj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://qs.colortex.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wm.521024.cn

—— 文件结束 ——
来源：http://pj.wgjwhj.cn

================================================================================
来源：http://iz.nszjky.cn

程序语言常见例子速查手册（2024 版）
来源：http://ah.chemitech.net.cn

Common Programming Examples Cheat Book
来源：http://sz.nicolike.cn

================================================================================
来源：http://cg.bjjhwx.cn

【收录内容】
来源：http://ni.wgjwhj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ei.521024.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nw.jianghongdianzi.cn

SQL · Bash · C · C++
来源：http://xg.shxzskj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://th.gzmigu.cn

【使用说明】
来源：http://qp.colortex.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fi.gzmigu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://lg.nicolike.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ca.szsharing.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mx.huanxung.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://bt.szsharing.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://kt.huixiangedu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lp.huanxung.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ig.hahajie.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ec.shtwfgs.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wv.newstarts.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dt.shtwfgs.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://no.wgjwhj.cn

【文件统计】
来源：http://be.shxzskj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gz.huanxung.cn

--------------------------------------------------------------------------------
来源：http://xq.newstarts.cn

目  录
来源：http://in.nicolike.cn

--------------------------------------------------------------------------------
来源：http://uy.bookmarksfly.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ra.szxytkj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://sj.chemitech.net.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://dl.521024.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://gy.yuntaijiaju.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wn.jctech888.com.cn


<!-- 参考信息 -->