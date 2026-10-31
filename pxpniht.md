代发 wailian999

[U11] Py：生成器表达式
来源：http://kj.shxzukj.cn

(x * 2 for x in arr)
来源：http://qx.colortex.cn

[U12] Py：取出现最多的 3 个元素
来源：http://et.muxihuayi.cn

Counter(arr).most_common(3)
来源：http://or.muxihuayi.cn

[U13] Py：固定长度队列
来源：http://qq.hahajie.cn

deque(maxlen=10)
来源：http://rg.jianghongdianzi.cn

[U14] Py：分组收集到列表
来源：http://gt.szsharing.cn

defaultdict(list)
来源：http://co.jianghongdianzi.cn

[U15] Py：高精度计时
来源：http://ts.hahajie.cn

t = time.perf_counter()
来源：http://ed.nicolike.cn

[U16] Py：命令行参数解析
来源：http://nx.shxzskj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pu.shxzskj.cn

[U17] Py：初始化日志
来源：http://bc.9csxet.cn

logging.basicConfig(level=logging.INFO)
来源：http://xq.asd995.cn

[U18] Py：预编译正则
来源：http://am.shtwfgs.cn

pat = re.compile(r"\d+")
来源：http://yd.bookmarksfly.cn

[U19] Py：正则替换带回调
来源：http://dq.lnxyls.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yy.nicolike.cn

[U20] Py：缓存函数结果
来源：http://xz.huanxung.cn

@functools.lru_cache(maxsize=None)
来源：http://lf.shtwfgs.cn

[U21] Py：自定义上下文管理器
来源：http://et.hahajie.cn

@contextlib.contextmanager
来源：http://na.shtwfgs.cn

[U22] Py：矩阵转置
来源：http://md.lnxyls.cn

list(zip(*m))
来源：http://dp.gzmigu.cn

[U23] Py：分块读取大文件
来源：http://hf.shxzukj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qn.haigaiapp.cn

[U24] Py：路径操作
来源：http://ld.gzmigu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ck.szsharing.cn

[U25] Py：CSV 按字典读
来源：http://sh.hahajie.cn

csv.DictReader(f)
来源：http://tz.gzmigu.cn

[U26] Py：并发下载
来源：http://bw.9csxet.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ab.bookmarksfly.cn

[U27] Py：异步 HTTP
来源：http://bl.chemitech.net.cn

aiohttp.ClientSession() 配合 async with
来源：http://hz.panjiajie.cn

[U28] Py：类型别名
来源：http://zw.bookmarksfly.cn

UserId = int
来源：http://dj.asd995.cn

[U29] Py：属性校验
来源：http://rf.colortex.cn

@property 与 @x.setter 配合
来源：http://sr.huanxung.cn

[U30] Py：数据类
来源：http://io.panjiajie.cn

@dataclass(slots=True)
来源：http://og.shxzskj.cn

[U31] Py：单测
来源：http://xt.huixiangedu.cn

python -m pytest -q
来源：http://vl.gzmigu.cn

[U32] Py：代码格式化
来源：http://el.haigaiapp.cn

ruff format . && ruff check --fix .
来源：http://nw.szxytkj.cn

[U33] Py：打包发布
来源：http://tq.colortex.cn

python -m build  （依赖 pyproject.toml）
来源：http://yt.huanxung.cn

[U34] Py：判断编码
来源：http://rh.nszjky.cn

chardet.detect(raw)
来源：http://yb.colortex.cn

[U35] Py：发送邮件
来源：http://jl.gzmigu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pg.asd995.cn

[U36] Py：定时任务
来源：http://lw.yuexingan06.cn

schedule.every(10).minutes.do(job)
来源：http://gk.bookmarksfly.cn

[U37] Py：读写 Excel
来源：http://ve.nszjky.cn

pandas.read_excel / DataFrame.to_excel
来源：http://zg.9csxet.cn

[U38] Py：获取脚本所在目录
来源：http://sp.newstarts.cn

Path(__file__).resolve().parent
来源：http://ph.shtwfgs.cn

[U39] Py：判断是否在交互环境
来源：http://nm.jianghongdianzi.cn

sys.stdout.isatty()
来源：http://bt.jianghongdianzi.cn

[U40] Py：打印到标准错误
来源：http://fb.nszjky.cn

print("err", file=sys.stderr)
来源：http://il.haigaiapp.cn

[U41] PHP：初始化 Composer 项目
来源：http://ag.chemitech.net.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xg.hahajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://kx.yuexingan06.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://av.hahajie.cn

[U43] PHP：声明命名空间
来源：http://cn.huixiangedu.cn

namespace App\Http;
来源：http://zv.shxzskj.cn

[U44] PHP：开启严格类型
来源：http://fz.jctech888.com.cn

declare(strict_types=1);
来源：http://bs.bjjhwx.cn

[U45] PHP：类型声明与返回类型
来源：http://kf.shxzukj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://cy.colortex.cn

[U46] PHP：可空类型
来源：http://vb.szxytkj.cn

?string $name = null
来源：http://un.huanxung.cn

[U47] PHP：联合类型
来源：http://pn.nicolike.cn

int|string $id
来源：http://ue.huanxung.cn

[U48] PHP：纯枚举
来源：http://nw.huanxung.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://np.wgjwhj.cn

[U49] PHP：只读属性
来源：http://km.huixiangedu.cn

public readonly string $name
来源：http://xv.asd995.cn

[U50] PHP：构造器属性提升
来源：http://bg.521024.cn

public function __construct(private int $id) {}
来源：http://cw.bookmarksfly.cn

[U51] PHP：数组解构
来源：http://ti.panjiajie.cn

[$a, $b] = $arr;
来源：http://lq.muxihuayi.cn

[U52] PHP：箭头函数
来源：http://or.panjiajie.cn

$double = fn($x) => $x * 2;
来源：http://do.szxytkj.cn

[U53] PHP：空合并运算符
来源：http://gk.asd995.cn

$v = $a ?? $b ?? "default";
来源：http://js.shxzukj.cn

[U54] PHP：空安全调用
来源：http://py.nicolike.cn

$obj?->method()
来源：http://wy.newstarts.cn

[U55] PHP：match 表达式
来源：http://yu.panjiajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jq.nszjky.cn

[U56] PHP：命名参数
来源：http://sj.9csxet.cn

f(a: 1, b: 2)
来源：http://ya.hahajie.cn

[U57] PHP：字符串插值
来源：http://kg.newstarts.cn

"值: {$a}"
来源：http://hw.gzmigu.cn

[U58] PHP：数组三件套
来源：http://qe.muxihuayi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xv.muxihuayi.cn

[U59] PHP：自定义排序
来源：http://en.haigaiapp.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uh.huanxung.cn

[U60] PHP：JSON 编解码
来源：http://hd.jianghongdianzi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wd.huixinmuqiang.cn

[U61] PHP：正则
来源：http://wg.huixinmuqiang.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lm.jctech888.com.cn

[U62] PHP：日期对象
来源：http://lv.muxihuayi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jl.wgjwhj.cn

[U63] PHP：文件读写
来源：http://uk.hnjuh.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pc.gzmigu.cn

[U64] PHP：目录遍历
来源：http://ue.yuexingan06.cn

glob("dir/*.php");  scandir("dir");
来源：http://yl.gzmigu.cn

[U65] PHP：会话
来源：http://oi.muxihuayi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://yg.nicolike.cn

[U66] PHP：设置 Cookie
来源：http://ot.yuntaijiaju.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vj.9csxet.cn

[U67] PHP：处理文件上传
来源：http://hv.jianghongdianzi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://iv.chemitech.net.cn

[U68] PHP：PDO 连接
来源：http://ch.asd995.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ko.nszjky.cn

[U69] PHP：PDO 预处理
来源：http://oc.521024.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cf.shxzskj.cn

[U70] PHP：PDO 事务
来源：http://ld.shxzukj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://oy.colortex.cn

[U71] PHP：抛出异常
来源：http://mf.nszjky.cn

throw new RuntimeException("失败", 500);
来源：http://ly.nszjky.cn

[U72] PHP：写错误日志
来源：http://mz.lnxyls.cn

error_log("失败: " . $e->getMessage());
来源：http://gy.shxzskj.cn

[U73] PHP：读取 ini 配置
来源：http://ya.jctech888.com.cn

parse_ini_file("config.ini", true)
来源：http://xp.hahajie.cn

[U74] PHP：读取环境变量
来源：http://mw.shtwfgs.cn

getenv("APP_ENV") ?: "production"
来源：http://pl.jianghongdianzi.cn

[U75] PHP：依赖注入
来源：http://dq.colortex.cn

composer require psr/container
来源：http://pr.huixinmuqiang.cn

[U76] PHP：简单路由
来源：http://mn.shxzukj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bv.colortex.cn

[U77] PHP：模板渲染
来源：http://qp.shxzukj.cn

composer require twig/twig
来源：http://mk.shtwfgs.cn

[U78] PHP：单元测试
来源：http://pb.huanxung.cn

composer require --dev phpunit/phpunit
来源：http://zs.wgjwhj.cn

[U79] PHP：静态分析
来源：http://fc.jianghongdianzi.cn

composer require --dev phpstan/phpstan
来源：http://qd.lnxyls.cn

[U80] PHP：代码规范修复
来源：http://wc.bookmarksfly.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://cv.521024.cn

[U81] JS：初始化项目
来源：http://su.yuntaijiaju.cn

npm init -y;  npm i express
来源：http://sw.shtwfgs.cn

[U82] JS：package.json 脚本
来源：http://xa.chemitech.net.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://na.asd995.cn

[U83] JS：ES Module 导入导出
来源：http://qq.szsharing.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xn.lnxyls.cn

[U84] JS：CommonJS 写法
来源：http://js.lnxyls.cn

module.exports = { a };  const { a } = require("./m");
来源：http://oa.jianghongdianzi.cn

[U85] JS：可选链
来源：http://am.szsharing.cn

a?.b?.c
来源：http://xs.gzmigu.cn

[U86] JS：空值合并
来源：http://yz.hahajie.cn

a ?? b
来源：http://tg.jianghongdianzi.cn

[U87] JS：解构默认值
来源：http://ut.asd995.cn

const { a = 1, b = 2 } = obj;
来源：http://ly.huixiangedu.cn

[U88] JS：对象展开合并
来源：http://ju.szsharing.cn

{ ...a, ...b }
来源：http://mn.szxytkj.cn

[U89] JS：数组去重
来源：http://op.szxytkj.cn

[...new Set(arr)]
来源：http://pk.gzmigu.cn

[U90] JS：数字数组排序
来源：http://ms.gzmigu.cn

[...arr].sort((a, b) => a - b)
来源：http://vc.jctech888.com.cn

[U91] JS：对象键值遍历
来源：http://ec.newstarts.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xw.shxzukj.cn

[U92] JS：深拷贝
来源：http://jt.huixiangedu.cn

structuredClone(obj)
来源：http://hd.jianghongdianzi.cn

[U93] JS：模板字符串
来源：http://tm.haigaiapp.cn

`共 ${n} 条`
来源：http://wm.shtwfgs.cn

[U94] JS：箭头函数
来源：http://ov.bjjhwx.cn

const double = x => x * 2;
来源：http://nc.huixinmuqiang.cn

[U95] JS：Promise 包装
来源：http://nz.hnjuh.cn

new Promise((resolve, reject) => {})
来源：http://yh.bookmarksfly.cn

[U96] JS：async/await 与异常
来源：http://dq.521024.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yc.szxytkj.cn

[U97] JS：并发请求
来源：http://wo.bjjhwx.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://kg.huixiangedu.cn

[U98] JS：fetch 带 JSON
来源：http://el.yuexingan06.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xv.yuntaijiaju.cn

[U99] JS：事件监听
来源：http://de.huixinmuqiang.cn

el.addEventListener("click", e => {})
来源：http://hw.shxzukj.cn

[U100] JS：DOM 查询
来源：http://qn.huanxung.cn

document.querySelector(".item")
来源：http://zh.9csxet.cn

[U101] JS：classList 操作
来源：http://on.521024.cn

el.classList.toggle("active")
来源：http://zw.hahajie.cn

[U102] JS：本地存储
来源：http://lk.521024.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ky.shtwfgs.cn

[U103] JS：定时器
来源：http://zf.shtwfgs.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wb.wgjwhj.cn

[U104] JS：防抖
来源：http://ta.huanxung.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tn.shxzskj.cn

[U105] JS：节流
来源：http://dp.jianghongdianzi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://af.shxzukj.cn

[U106] JS：日期格式化
来源：http://cl.yuexingan06.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bl.szsharing.cn

[U107] JS：数字千分位
来源：http://hf.jianghongdianzi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cb.wgjwhj.cn

[U108] JS：随机整数
来源：http://gv.yuntaijiaju.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cv.lnxyls.cn

[U109] JS：数组分组
来源：http://dk.521024.cn

Object.groupBy(arr, x => x.type)
来源：http://hw.huixinmuqiang.cn

[U110] JS：数组分块
来源：http://uc.jianghongdianzi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ef.shxzskj.cn

[U111] JS：对象转 Map
来源：http://lm.jctech888.com.cn

new Map(Object.entries(obj))
来源：http://yr.jctech888.com.cn

[U112] JS：字符串补位
来源：http://mr.nszjky.cn

"7".padStart(3, "0")
来源：http://gk.yuexingan06.cn

[U113] JS：正则替换全部
来源：http://ol.521024.cn

s.replaceAll("a", "b")
来源：http://vf.haigaiapp.cn

[U114] JS：JSON 深比较
来源：http://on.nszjky.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://wr.huixiangedu.cn

[U115] JS：生成 UUID
来源：http://dc.muxihuayi.cn

crypto.randomUUID()
来源：http://to.shtwfgs.cn

[U116] JS：类型检查（JSDoc）
来源：http://aw.panjiajie.cn

/** @param {string} name */ function f(name) {}
来源：http://ob.9csxet.cn

[U117] JS：单元测试
来源：http://oy.hnjuh.cn

npm i -D vitest;  npx vitest
来源：http://ch.hnjuh.cn

[U118] JS：开发服务器
来源：http://hm.asd995.cn

npm i -D vite;  npx vite
来源：http://zs.szsharing.cn

[U119] JS：生产构建
来源：http://zy.hahajie.cn

npx vite build
来源：http://cp.huixiangedu.cn

[U120] JS：读取环境变量（Vite）
来源：http://id.huixiangedu.cn

import.meta.env.VITE_API_URL
来源：http://ew.huanxung.cn

================================================================================
来源：http://pj.jctech888.com.cn

统计汇总
来源：http://gy.huanxung.cn

================================================================================
来源：http://ut.panjiajie.cn

按语言统计（条）：
来源：http://oy.jctech888.com.cn

Python ......... 252
来源：http://kl.huixiangedu.cn

PHP ............ 252
来源：http://wf.szxytkj.cn

JavaScript ..... 252
来源：http://ka.muxihuayi.cn

TypeScript ..... 212
来源：http://yq.szxytkj.cn

Java ........... 212
来源：http://xg.nicolike.cn

Go ............. 212
来源：http://uf.yuexingan06.cn

Ruby ........... 212
来源：http://bs.newstarts.cn

C# ............. 212
来源：http://yz.muxihuayi.cn

C .............. 30
来源：http://cz.shxzukj.cn

C++ ............ 30
来源：http://ox.gzmigu.cn

SQL ............ 90
来源：http://yp.hnjuh.cn

Bash ........... 80
来源：http://yq.szsharing.cn

Kotlin ......... 15
来源：http://vf.szxytkj.cn

Swift .......... 15
来源：http://cq.lnxyls.cn

Lua ............ 10
来源：http://zs.yuexingan06.cn

Perl ........... 10
来源：http://yn.jianghongdianzi.cn

Scala .......... 10
来源：http://op.huixinmuqiang.cn

------------------------------------
来源：http://xz.hnjuh.cn

合计 ........... 2106 条
来源：http://vr.yuntaijiaju.cn

按章节统计：
来源：http://bp.huanxung.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wv.shtwfgs.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yc.yuexingan06.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ww.jianghongdianzi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jf.szxytkj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lo.huixinmuqiang.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bb.nicolike.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ny.szxytkj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hy.haigaiapp.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mr.szsharing.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nv.huanxung.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wk.panjiajie.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://oj.bjjhwx.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ur.szxytkj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sm.shxzskj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fp.yuexingan06.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://db.yuntaijiaju.cn

Q SQL 专题                              90
来源：http://im.colortex.cn

R Bash 专题                             80
来源：http://vj.bjjhwx.cn

S C / C++ 专题                          60
来源：http://xn.shtwfgs.cn

T 其他语言补充                          60
来源：http://ai.panjiajie.cn

U 高频实用片段                         120
来源：http://ks.chemitech.net.cn

------------------------------------
来源：http://fo.bjjhwx.cn

合计                                  2106 条
来源：http://dk.hahajie.cn

--------------------------------------------------------------------------------
来源：http://mi.9csxet.cn

使用提醒
来源：http://ur.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://ss.chemitech.net.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kl.shxzskj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://kx.jctech888.com.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rw.szxytkj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://jg.huanxung.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mj.jctech888.com.cn

—— 文件结束 ——
来源：http://wh.bookmarksfly.cn

================================================================================
来源：http://jn.shtwfgs.cn

程序语言常见例子速查手册（2024 版）
来源：http://eh.yuexingan06.cn

Common Programming Examples Cheat Book
来源：http://xg.asd995.cn

================================================================================
来源：http://yb.hnjuh.cn

【收录内容】
来源：http://jj.jianghongdianzi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://se.jctech888.com.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://dg.muxihuayi.cn

SQL · Bash · C · C++
来源：http://ha.muxihuayi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://fa.bookmarksfly.cn

【使用说明】
来源：http://yf.gzmigu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://yg.huixinmuqiang.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rh.newstarts.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://fk.hnjuh.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xg.gzmigu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://jw.bookmarksfly.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lm.bjjhwx.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ut.huanxung.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://al.chemitech.net.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://nc.shtwfgs.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gi.shxzukj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://cu.jianghongdianzi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jg.shxzskj.cn

【文件统计】
来源：http://eb.newstarts.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ho.newstarts.cn


<!-- 参考信息 -->