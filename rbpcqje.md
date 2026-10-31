代发 wailian999

[U11] Py：生成器表达式
来源：http://wf.panjiajie.cn

(x * 2 for x in arr)
来源：http://xw.yuexingan06.cn

[U12] Py：取出现最多的 3 个元素
来源：http://yb.huixiangedu.cn

Counter(arr).most_common(3)
来源：http://ad.hahajie.cn

[U13] Py：固定长度队列
来源：http://wd.colortex.cn

deque(maxlen=10)
来源：http://dm.panjiajie.cn

[U14] Py：分组收集到列表
来源：http://ep.szxytkj.cn

defaultdict(list)
来源：http://so.chemitech.net.cn

[U15] Py：高精度计时
来源：http://tv.hahajie.cn

t = time.perf_counter()
来源：http://oj.bjjhwx.cn

[U16] Py：命令行参数解析
来源：http://dt.jianghongdianzi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wx.huixiangedu.cn

[U17] Py：初始化日志
来源：http://xh.shtwfgs.cn

logging.basicConfig(level=logging.INFO)
来源：http://sa.wgjwhj.cn

[U18] Py：预编译正则
来源：http://gw.yuexingan06.cn

pat = re.compile(r"\d+")
来源：http://cm.muxihuayi.cn

[U19] Py：正则替换带回调
来源：http://je.wgjwhj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ev.szsharing.cn

[U20] Py：缓存函数结果
来源：http://nf.yuntaijiaju.cn

@functools.lru_cache(maxsize=None)
来源：http://et.lnxyls.cn

[U21] Py：自定义上下文管理器
来源：http://ld.colortex.cn

@contextlib.contextmanager
来源：http://bu.huixinmuqiang.cn

[U22] Py：矩阵转置
来源：http://zg.lnxyls.cn

list(zip(*m))
来源：http://ws.newstarts.cn

[U23] Py：分块读取大文件
来源：http://nj.szsharing.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tw.huixinmuqiang.cn

[U24] Py：路径操作
来源：http://gy.lnxyls.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xv.chemitech.net.cn

[U25] Py：CSV 按字典读
来源：http://bd.shxzskj.cn

csv.DictReader(f)
来源：http://iy.nszjky.cn

[U26] Py：并发下载
来源：http://ke.bjjhwx.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hj.asd995.cn

[U27] Py：异步 HTTP
来源：http://iz.bookmarksfly.cn

aiohttp.ClientSession() 配合 async with
来源：http://qi.yuexingan06.cn

[U28] Py：类型别名
来源：http://wa.szxytkj.cn

UserId = int
来源：http://uv.shtwfgs.cn

[U29] Py：属性校验
来源：http://hx.nicolike.cn

@property 与 @x.setter 配合
来源：http://uz.nszjky.cn

[U30] Py：数据类
来源：http://gk.jctech888.com.cn

@dataclass(slots=True)
来源：http://kq.hahajie.cn

[U31] Py：单测
来源：http://jv.hahajie.cn

python -m pytest -q
来源：http://ih.jctech888.com.cn

[U32] Py：代码格式化
来源：http://xo.gzmigu.cn

ruff format . && ruff check --fix .
来源：http://ap.wgjwhj.cn

[U33] Py：打包发布
来源：http://su.nicolike.cn

python -m build  （依赖 pyproject.toml）
来源：http://pu.chemitech.net.cn

[U34] Py：判断编码
来源：http://kp.nszjky.cn

chardet.detect(raw)
来源：http://lf.hnjuh.cn

[U35] Py：发送邮件
来源：http://oj.wgjwhj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hm.9csxet.cn

[U36] Py：定时任务
来源：http://eg.521024.cn

schedule.every(10).minutes.do(job)
来源：http://bh.jctech888.com.cn

[U37] Py：读写 Excel
来源：http://qh.bjjhwx.cn

pandas.read_excel / DataFrame.to_excel
来源：http://hk.colortex.cn

[U38] Py：获取脚本所在目录
来源：http://lo.yuntaijiaju.cn

Path(__file__).resolve().parent
来源：http://ry.gzmigu.cn

[U39] Py：判断是否在交互环境
来源：http://yv.haigaiapp.cn

sys.stdout.isatty()
来源：http://uq.nicolike.cn

[U40] Py：打印到标准错误
来源：http://nn.gzmigu.cn

print("err", file=sys.stderr)
来源：http://pq.shtwfgs.cn

[U41] PHP：初始化 Composer 项目
来源：http://rd.muxihuayi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://bn.huanxung.cn

[U42] PHP：PSR-4 自动加载
来源：http://uh.panjiajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ud.nszjky.cn

[U43] PHP：声明命名空间
来源：http://nl.wgjwhj.cn

namespace App\Http;
来源：http://li.yuntaijiaju.cn

[U44] PHP：开启严格类型
来源：http://nj.jctech888.com.cn

declare(strict_types=1);
来源：http://zj.newstarts.cn

[U45] PHP：类型声明与返回类型
来源：http://jo.shxzskj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://nn.newstarts.cn

[U46] PHP：可空类型
来源：http://ui.chemitech.net.cn

?string $name = null
来源：http://iu.szxytkj.cn

[U47] PHP：联合类型
来源：http://pf.haigaiapp.cn

int|string $id
来源：http://gm.yuntaijiaju.cn

[U48] PHP：纯枚举
来源：http://wp.jctech888.com.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qs.jctech888.com.cn

[U49] PHP：只读属性
来源：http://ow.haigaiapp.cn

public readonly string $name
来源：http://oi.huixinmuqiang.cn

[U50] PHP：构造器属性提升
来源：http://am.chemitech.net.cn

public function __construct(private int $id) {}
来源：http://ev.shxzukj.cn

[U51] PHP：数组解构
来源：http://dt.nicolike.cn

[$a, $b] = $arr;
来源：http://ta.huanxung.cn

[U52] PHP：箭头函数
来源：http://vs.muxihuayi.cn

$double = fn($x) => $x * 2;
来源：http://ec.bjjhwx.cn

[U53] PHP：空合并运算符
来源：http://ng.jianghongdianzi.cn

$v = $a ?? $b ?? "default";
来源：http://iy.asd995.cn

[U54] PHP：空安全调用
来源：http://lf.szsharing.cn

$obj?->method()
来源：http://kj.nicolike.cn

[U55] PHP：match 表达式
来源：http://si.yuntaijiaju.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hg.panjiajie.cn

[U56] PHP：命名参数
来源：http://ff.huixiangedu.cn

f(a: 1, b: 2)
来源：http://lo.521024.cn

[U57] PHP：字符串插值
来源：http://oh.panjiajie.cn

"值: {$a}"
来源：http://tw.hnjuh.cn

[U58] PHP：数组三件套
来源：http://uu.521024.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wt.huixiangedu.cn

[U59] PHP：自定义排序
来源：http://qh.shtwfgs.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ws.muxihuayi.cn

[U60] PHP：JSON 编解码
来源：http://rp.gzmigu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ai.shxzskj.cn

[U61] PHP：正则
来源：http://qe.9csxet.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pc.521024.cn

[U62] PHP：日期对象
来源：http://wx.nicolike.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ln.haigaiapp.cn

[U63] PHP：文件读写
来源：http://rk.521024.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ka.521024.cn

[U64] PHP：目录遍历
来源：http://ib.shxzskj.cn

glob("dir/*.php");  scandir("dir");
来源：http://rs.yuntaijiaju.cn

[U65] PHP：会话
来源：http://mo.muxihuayi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://bh.wgjwhj.cn

[U66] PHP：设置 Cookie
来源：http://fy.szxytkj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nt.szxytkj.cn

[U67] PHP：处理文件上传
来源：http://cq.szxytkj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pq.shxzskj.cn

[U68] PHP：PDO 连接
来源：http://fs.chemitech.net.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://et.9csxet.cn

[U69] PHP：PDO 预处理
来源：http://fl.panjiajie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xf.nszjky.cn

[U70] PHP：PDO 事务
来源：http://fq.asd995.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://au.gzmigu.cn

[U71] PHP：抛出异常
来源：http://yw.newstarts.cn

throw new RuntimeException("失败", 500);
来源：http://vo.nszjky.cn

[U72] PHP：写错误日志
来源：http://kj.shtwfgs.cn

error_log("失败: " . $e->getMessage());
来源：http://oi.bookmarksfly.cn

[U73] PHP：读取 ini 配置
来源：http://xy.hnjuh.cn

parse_ini_file("config.ini", true)
来源：http://jy.yuntaijiaju.cn

[U74] PHP：读取环境变量
来源：http://pf.shxzskj.cn

getenv("APP_ENV") ?: "production"
来源：http://qn.jianghongdianzi.cn

[U75] PHP：依赖注入
来源：http://vl.wgjwhj.cn

composer require psr/container
来源：http://fm.bjjhwx.cn

[U76] PHP：简单路由
来源：http://lm.nicolike.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mj.asd995.cn

[U77] PHP：模板渲染
来源：http://yw.hnjuh.cn

composer require twig/twig
来源：http://lm.lnxyls.cn

[U78] PHP：单元测试
来源：http://da.jianghongdianzi.cn

composer require --dev phpunit/phpunit
来源：http://so.chemitech.net.cn

[U79] PHP：静态分析
来源：http://yr.hahajie.cn

composer require --dev phpstan/phpstan
来源：http://qb.jctech888.com.cn

[U80] PHP：代码规范修复
来源：http://sp.huixiangedu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://uf.haigaiapp.cn

[U81] JS：初始化项目
来源：http://is.shxzukj.cn

npm init -y;  npm i express
来源：http://rq.asd995.cn

[U82] JS：package.json 脚本
来源：http://nd.hnjuh.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ul.muxihuayi.cn

[U83] JS：ES Module 导入导出
来源：http://vf.panjiajie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://yz.gzmigu.cn

[U84] JS：CommonJS 写法
来源：http://bt.shtwfgs.cn

module.exports = { a };  const { a } = require("./m");
来源：http://lm.colortex.cn

[U85] JS：可选链
来源：http://gd.muxihuayi.cn

a?.b?.c
来源：http://ji.huixiangedu.cn

[U86] JS：空值合并
来源：http://za.lnxyls.cn

a ?? b
来源：http://ix.hahajie.cn

[U87] JS：解构默认值
来源：http://mg.muxihuayi.cn

const { a = 1, b = 2 } = obj;
来源：http://io.huixiangedu.cn

[U88] JS：对象展开合并
来源：http://ci.huanxung.cn

{ ...a, ...b }
来源：http://or.lnxyls.cn

[U89] JS：数组去重
来源：http://lt.shxzskj.cn

[...new Set(arr)]
来源：http://ok.wgjwhj.cn

[U90] JS：数字数组排序
来源：http://lb.jianghongdianzi.cn

[...arr].sort((a, b) => a - b)
来源：http://ex.shxzukj.cn

[U91] JS：对象键值遍历
来源：http://qq.gzmigu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://sl.nicolike.cn

[U92] JS：深拷贝
来源：http://hx.521024.cn

structuredClone(obj)
来源：http://kb.chemitech.net.cn

[U93] JS：模板字符串
来源：http://ob.lnxyls.cn

`共 ${n} 条`
来源：http://ju.huanxung.cn

[U94] JS：箭头函数
来源：http://gl.lnxyls.cn

const double = x => x * 2;
来源：http://kz.yuntaijiaju.cn

[U95] JS：Promise 包装
来源：http://sh.lnxyls.cn

new Promise((resolve, reject) => {})
来源：http://il.newstarts.cn

[U96] JS：async/await 与异常
来源：http://yv.bjjhwx.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://av.yuntaijiaju.cn

[U97] JS：并发请求
来源：http://fy.lnxyls.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bp.hnjuh.cn

[U98] JS：fetch 带 JSON
来源：http://pz.9csxet.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ex.chemitech.net.cn

[U99] JS：事件监听
来源：http://fm.bookmarksfly.cn

el.addEventListener("click", e => {})
来源：http://zm.hnjuh.cn

[U100] JS：DOM 查询
来源：http://cw.jianghongdianzi.cn

document.querySelector(".item")
来源：http://uj.shxzskj.cn

[U101] JS：classList 操作
来源：http://zo.gzmigu.cn

el.classList.toggle("active")
来源：http://xt.asd995.cn

[U102] JS：本地存储
来源：http://bl.shtwfgs.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://gk.szxytkj.cn

[U103] JS：定时器
来源：http://zp.huixinmuqiang.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rb.shtwfgs.cn

[U104] JS：防抖
来源：http://wx.muxihuayi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hg.521024.cn

[U105] JS：节流
来源：http://md.panjiajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://uw.hahajie.cn

[U106] JS：日期格式化
来源：http://xw.szsharing.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vn.shxzskj.cn

[U107] JS：数字千分位
来源：http://qi.yuexingan06.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://un.muxihuayi.cn

[U108] JS：随机整数
来源：http://yd.bookmarksfly.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vh.haigaiapp.cn

[U109] JS：数组分组
来源：http://ku.yuntaijiaju.cn

Object.groupBy(arr, x => x.type)
来源：http://rg.wgjwhj.cn

[U110] JS：数组分块
来源：http://kp.gzmigu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dk.9csxet.cn

[U111] JS：对象转 Map
来源：http://et.szsharing.cn

new Map(Object.entries(obj))
来源：http://at.gzmigu.cn

[U112] JS：字符串补位
来源：http://rr.shxzukj.cn

"7".padStart(3, "0")
来源：http://ty.gzmigu.cn

[U113] JS：正则替换全部
来源：http://jd.nicolike.cn

s.replaceAll("a", "b")
来源：http://cd.jianghongdianzi.cn

[U114] JS：JSON 深比较
来源：http://hf.shxzskj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://yf.haigaiapp.cn

[U115] JS：生成 UUID
来源：http://an.chemitech.net.cn

crypto.randomUUID()
来源：http://sj.huixinmuqiang.cn

[U116] JS：类型检查（JSDoc）
来源：http://vm.muxihuayi.cn

/** @param {string} name */ function f(name) {}
来源：http://we.9csxet.cn

[U117] JS：单元测试
来源：http://yc.haigaiapp.cn

npm i -D vitest;  npx vitest
来源：http://ck.huixiangedu.cn

[U118] JS：开发服务器
来源：http://if.yuexingan06.cn

npm i -D vite;  npx vite
来源：http://ji.szxytkj.cn

[U119] JS：生产构建
来源：http://yu.lnxyls.cn

npx vite build
来源：http://bn.gzmigu.cn

[U120] JS：读取环境变量（Vite）
来源：http://zg.bookmarksfly.cn

import.meta.env.VITE_API_URL
来源：http://ii.wgjwhj.cn

================================================================================
来源：http://ca.nicolike.cn

统计汇总
来源：http://hl.hnjuh.cn

================================================================================
来源：http://tw.colortex.cn

按语言统计（条）：
来源：http://up.shxzukj.cn

Python ......... 252
来源：http://jh.jctech888.com.cn

PHP ............ 252
来源：http://ae.panjiajie.cn

JavaScript ..... 252
来源：http://mr.hnjuh.cn

TypeScript ..... 212
来源：http://ug.jctech888.com.cn

Java ........... 212
来源：http://ke.nicolike.cn

Go ............. 212
来源：http://qs.haigaiapp.cn

Ruby ........... 212
来源：http://zk.lnxyls.cn

C# ............. 212
来源：http://uu.muxihuayi.cn

C .............. 30
来源：http://cy.bookmarksfly.cn

C++ ............ 30
来源：http://dk.shxzskj.cn

SQL ............ 90
来源：http://hl.muxihuayi.cn

Bash ........... 80
来源：http://fn.szxytkj.cn

Kotlin ......... 15
来源：http://gw.bookmarksfly.cn

Swift .......... 15
来源：http://tf.jctech888.com.cn

Lua ............ 10
来源：http://nn.muxihuayi.cn

Perl ........... 10
来源：http://ki.huixinmuqiang.cn

Scala .......... 10
来源：http://ej.nszjky.cn

------------------------------------
来源：http://mj.huixinmuqiang.cn

合计 ........... 2106 条
来源：http://ak.yuntaijiaju.cn

按章节统计：
来源：http://uy.szxytkj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ww.nicolike.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ur.szsharing.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://sj.hahajie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://uf.shxzukj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bm.hnjuh.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ca.jctech888.com.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ba.hnjuh.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://aj.shtwfgs.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://cb.bookmarksfly.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xr.muxihuayi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zu.shxzskj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mf.9csxet.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zf.521024.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://uc.szsharing.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://an.hahajie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ys.yuntaijiaju.cn

Q SQL 专题                              90
来源：http://mi.bjjhwx.cn

R Bash 专题                             80
来源：http://bm.hnjuh.cn

S C / C++ 专题                          60
来源：http://tn.muxihuayi.cn

T 其他语言补充                          60
来源：http://jk.colortex.cn

U 高频实用片段                         120
来源：http://ln.bookmarksfly.cn

------------------------------------
来源：http://we.huixinmuqiang.cn

合计                                  2106 条
来源：http://za.9csxet.cn

--------------------------------------------------------------------------------
来源：http://rv.colortex.cn

使用提醒
来源：http://pj.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://hm.bjjhwx.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vi.bjjhwx.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ci.szsharing.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://uk.lnxyls.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://fy.szxytkj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dp.hahajie.cn

—— 文件结束 ——
来源：http://ub.szsharing.cn

================================================================================
来源：http://hp.521024.cn

程序语言常见例子速查手册（2024 版）
来源：http://rg.nicolike.cn

Common Programming Examples Cheat Book
来源：http://bo.asd995.cn

================================================================================
来源：http://ax.shtwfgs.cn

【收录内容】
来源：http://id.yuexingan06.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://kw.szxytkj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xf.hahajie.cn

SQL · Bash · C · C++
来源：http://gb.haigaiapp.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dv.huixiangedu.cn

【使用说明】
来源：http://yp.panjiajie.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://sl.haigaiapp.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://pd.colortex.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://au.yuntaijiaju.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gg.bjjhwx.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://yn.shxzskj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vy.shxzukj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ct.hnjuh.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xn.panjiajie.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://aw.jctech888.com.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qv.gzmigu.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rg.nicolike.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://oe.chemitech.net.cn

【文件统计】
来源：http://op.nszjky.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://uq.szsharing.cn


<!-- 参考信息 -->