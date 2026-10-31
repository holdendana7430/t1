代发 wailian999

[U09] Py：字典取最大值的键
来源：http://an.gzmigu.cn

max(d, key=d.get)
来源：http://rw.panjiajie.cn

[U10] Py：按值排序字典
来源：http://yz.szxytkj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wd.yuntaijiaju.cn

[U11] Py：生成器表达式
来源：http://vy.nicolike.cn

(x * 2 for x in arr)
来源：http://zw.jctech888.com.cn

[U12] Py：取出现最多的 3 个元素
来源：http://eq.yuexingan06.cn

Counter(arr).most_common(3)
来源：http://it.shxzskj.cn

[U13] Py：固定长度队列
来源：http://lt.nszjky.cn

deque(maxlen=10)
来源：http://ue.wgjwhj.cn

[U14] Py：分组收集到列表
来源：http://so.nszjky.cn

defaultdict(list)
来源：http://uv.chemitech.net.cn

[U15] Py：高精度计时
来源：http://cp.9csxet.cn

t = time.perf_counter()
来源：http://ej.9csxet.cn

[U16] Py：命令行参数解析
来源：http://cd.chemitech.net.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dn.bjjhwx.cn

[U17] Py：初始化日志
来源：http://fq.huixinmuqiang.cn

logging.basicConfig(level=logging.INFO)
来源：http://fo.colortex.cn

[U18] Py：预编译正则
来源：http://yv.nszjky.cn

pat = re.compile(r"\d+")
来源：http://jf.bjjhwx.cn

[U19] Py：正则替换带回调
来源：http://ui.lnxyls.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://oo.chemitech.net.cn

[U20] Py：缓存函数结果
来源：http://qe.bookmarksfly.cn

@functools.lru_cache(maxsize=None)
来源：http://uu.haigaiapp.cn

[U21] Py：自定义上下文管理器
来源：http://ce.shtwfgs.cn

@contextlib.contextmanager
来源：http://xg.muxihuayi.cn

[U22] Py：矩阵转置
来源：http://zj.yuexingan06.cn

list(zip(*m))
来源：http://ad.asd995.cn

[U23] Py：分块读取大文件
来源：http://nv.jctech888.com.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vl.haigaiapp.cn

[U24] Py：路径操作
来源：http://uu.huanxung.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rp.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://yc.panjiajie.cn

csv.DictReader(f)
来源：http://ya.szxytkj.cn

[U26] Py：并发下载
来源：http://yp.newstarts.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://oy.haigaiapp.cn

[U27] Py：异步 HTTP
来源：http://ip.huixiangedu.cn

aiohttp.ClientSession() 配合 async with
来源：http://qo.colortex.cn

[U28] Py：类型别名
来源：http://jq.asd995.cn

UserId = int
来源：http://ns.hnjuh.cn

[U29] Py：属性校验
来源：http://ex.muxihuayi.cn

@property 与 @x.setter 配合
来源：http://bf.nszjky.cn

[U30] Py：数据类
来源：http://fl.hahajie.cn

@dataclass(slots=True)
来源：http://kz.bjjhwx.cn

[U31] Py：单测
来源：http://xu.yuexingan06.cn

python -m pytest -q
来源：http://fb.szxytkj.cn

[U32] Py：代码格式化
来源：http://ge.muxihuayi.cn

ruff format . && ruff check --fix .
来源：http://kh.gzmigu.cn

[U33] Py：打包发布
来源：http://nj.lnxyls.cn

python -m build  （依赖 pyproject.toml）
来源：http://la.muxihuayi.cn

[U34] Py：判断编码
来源：http://ni.hahajie.cn

chardet.detect(raw)
来源：http://hw.jianghongdianzi.cn

[U35] Py：发送邮件
来源：http://kw.yuexingan06.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hy.panjiajie.cn

[U36] Py：定时任务
来源：http://om.muxihuayi.cn

schedule.every(10).minutes.do(job)
来源：http://xd.asd995.cn

[U37] Py：读写 Excel
来源：http://tf.shxzskj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ax.9csxet.cn

[U38] Py：获取脚本所在目录
来源：http://sg.newstarts.cn

Path(__file__).resolve().parent
来源：http://do.521024.cn

[U39] Py：判断是否在交互环境
来源：http://tc.huixinmuqiang.cn

sys.stdout.isatty()
来源：http://by.hahajie.cn

[U40] Py：打印到标准错误
来源：http://gb.bookmarksfly.cn

print("err", file=sys.stderr)
来源：http://tw.chemitech.net.cn

[U41] PHP：初始化 Composer 项目
来源：http://pp.bookmarksfly.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://as.lnxyls.cn

[U42] PHP：PSR-4 自动加载
来源：http://fq.colortex.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tr.shxzukj.cn

[U43] PHP：声明命名空间
来源：http://oh.jianghongdianzi.cn

namespace App\Http;
来源：http://dq.nicolike.cn

[U44] PHP：开启严格类型
来源：http://fd.wgjwhj.cn

declare(strict_types=1);
来源：http://pa.shxzskj.cn

[U45] PHP：类型声明与返回类型
来源：http://au.yuexingan06.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ow.gzmigu.cn

[U46] PHP：可空类型
来源：http://fq.yuexingan06.cn

?string $name = null
来源：http://zw.jctech888.com.cn

[U47] PHP：联合类型
来源：http://vt.hahajie.cn

int|string $id
来源：http://oa.bookmarksfly.cn

[U48] PHP：纯枚举
来源：http://wh.huixinmuqiang.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qo.szsharing.cn

[U49] PHP：只读属性
来源：http://yg.jctech888.com.cn

public readonly string $name
来源：http://xo.haigaiapp.cn

[U50] PHP：构造器属性提升
来源：http://wu.hnjuh.cn

public function __construct(private int $id) {}
来源：http://ck.shtwfgs.cn

[U51] PHP：数组解构
来源：http://ii.shtwfgs.cn

[$a, $b] = $arr;
来源：http://op.yuexingan06.cn

[U52] PHP：箭头函数
来源：http://wa.huixinmuqiang.cn

$double = fn($x) => $x * 2;
来源：http://sr.chemitech.net.cn

[U53] PHP：空合并运算符
来源：http://rk.jctech888.com.cn

$v = $a ?? $b ?? "default";
来源：http://jn.hahajie.cn

[U54] PHP：空安全调用
来源：http://rq.gzmigu.cn

$obj?->method()
来源：http://px.jianghongdianzi.cn

[U55] PHP：match 表达式
来源：http://qo.9csxet.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xr.521024.cn

[U56] PHP：命名参数
来源：http://fl.asd995.cn

f(a: 1, b: 2)
来源：http://pb.521024.cn

[U57] PHP：字符串插值
来源：http://as.asd995.cn

"值: {$a}"
来源：http://mt.panjiajie.cn

[U58] PHP：数组三件套
来源：http://jn.wgjwhj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xd.huixinmuqiang.cn

[U59] PHP：自定义排序
来源：http://ue.lnxyls.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fh.yuexingan06.cn

[U60] PHP：JSON 编解码
来源：http://jp.huixinmuqiang.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fh.szsharing.cn

[U61] PHP：正则
来源：http://sh.nszjky.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cl.521024.cn

[U62] PHP：日期对象
来源：http://yr.nicolike.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://eo.hnjuh.cn

[U63] PHP：文件读写
来源：http://bi.panjiajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ck.panjiajie.cn

[U64] PHP：目录遍历
来源：http://hc.wgjwhj.cn

glob("dir/*.php");  scandir("dir");
来源：http://mc.haigaiapp.cn

[U65] PHP：会话
来源：http://xq.huanxung.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://bf.jianghongdianzi.cn

[U66] PHP：设置 Cookie
来源：http://kg.newstarts.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hy.chemitech.net.cn

[U67] PHP：处理文件上传
来源：http://cl.jctech888.com.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gn.muxihuayi.cn

[U68] PHP：PDO 连接
来源：http://ar.huixinmuqiang.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rc.yuntaijiaju.cn

[U69] PHP：PDO 预处理
来源：http://rc.panjiajie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ck.newstarts.cn

[U70] PHP：PDO 事务
来源：http://yj.szxytkj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pj.yuntaijiaju.cn

[U71] PHP：抛出异常
来源：http://yb.yuntaijiaju.cn

throw new RuntimeException("失败", 500);
来源：http://wj.muxihuayi.cn

[U72] PHP：写错误日志
来源：http://id.szxytkj.cn

error_log("失败: " . $e->getMessage());
来源：http://hw.521024.cn

[U73] PHP：读取 ini 配置
来源：http://oo.bookmarksfly.cn

parse_ini_file("config.ini", true)
来源：http://tt.gzmigu.cn

[U74] PHP：读取环境变量
来源：http://ar.huanxung.cn

getenv("APP_ENV") ?: "production"
来源：http://au.jianghongdianzi.cn

[U75] PHP：依赖注入
来源：http://sm.newstarts.cn

composer require psr/container
来源：http://dt.9csxet.cn

[U76] PHP：简单路由
来源：http://hg.szsharing.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lm.shxzskj.cn

[U77] PHP：模板渲染
来源：http://yz.521024.cn

composer require twig/twig
来源：http://np.asd995.cn

[U78] PHP：单元测试
来源：http://yi.huanxung.cn

composer require --dev phpunit/phpunit
来源：http://ci.9csxet.cn

[U79] PHP：静态分析
来源：http://bw.shtwfgs.cn

composer require --dev phpstan/phpstan
来源：http://xu.szsharing.cn

[U80] PHP：代码规范修复
来源：http://zm.shtwfgs.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://up.newstarts.cn

[U81] JS：初始化项目
来源：http://xw.haigaiapp.cn

npm init -y;  npm i express
来源：http://cz.panjiajie.cn

[U82] JS：package.json 脚本
来源：http://tp.panjiajie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cc.yuexingan06.cn

[U83] JS：ES Module 导入导出
来源：http://ak.jctech888.com.cn

export const a = 1;  import { a } from "./m.js";
来源：http://cp.bjjhwx.cn

[U84] JS：CommonJS 写法
来源：http://rd.bookmarksfly.cn

module.exports = { a };  const { a } = require("./m");
来源：http://fr.bjjhwx.cn

[U85] JS：可选链
来源：http://vp.colortex.cn

a?.b?.c
来源：http://gq.hahajie.cn

[U86] JS：空值合并
来源：http://ob.lnxyls.cn

a ?? b
来源：http://ti.bookmarksfly.cn

[U87] JS：解构默认值
来源：http://ue.newstarts.cn

const { a = 1, b = 2 } = obj;
来源：http://us.shxzskj.cn

[U88] JS：对象展开合并
来源：http://sw.shxzskj.cn

{ ...a, ...b }
来源：http://gk.colortex.cn

[U89] JS：数组去重
来源：http://rs.jianghongdianzi.cn

[...new Set(arr)]
来源：http://iu.gzmigu.cn

[U90] JS：数字数组排序
来源：http://iw.szxytkj.cn

[...arr].sort((a, b) => a - b)
来源：http://fa.9csxet.cn

[U91] JS：对象键值遍历
来源：http://lx.jctech888.com.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vm.nicolike.cn

[U92] JS：深拷贝
来源：http://xk.panjiajie.cn

structuredClone(obj)
来源：http://on.panjiajie.cn

[U93] JS：模板字符串
来源：http://ax.asd995.cn

`共 ${n} 条`
来源：http://mr.yuntaijiaju.cn

[U94] JS：箭头函数
来源：http://mp.huixinmuqiang.cn

const double = x => x * 2;
来源：http://ey.huanxung.cn

[U95] JS：Promise 包装
来源：http://xn.haigaiapp.cn

new Promise((resolve, reject) => {})
来源：http://ln.shtwfgs.cn

[U96] JS：async/await 与异常
来源：http://ou.shtwfgs.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ir.shxzukj.cn

[U97] JS：并发请求
来源：http://lb.haigaiapp.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://fo.521024.cn

[U98] JS：fetch 带 JSON
来源：http://bg.yuexingan06.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ju.hahajie.cn

[U99] JS：事件监听
来源：http://fo.muxihuayi.cn

el.addEventListener("click", e => {})
来源：http://km.shxzskj.cn

[U100] JS：DOM 查询
来源：http://kj.haigaiapp.cn

document.querySelector(".item")
来源：http://ct.panjiajie.cn

[U101] JS：classList 操作
来源：http://tx.colortex.cn

el.classList.toggle("active")
来源：http://qw.szsharing.cn

[U102] JS：本地存储
来源：http://pk.newstarts.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://gi.huanxung.cn

[U103] JS：定时器
来源：http://va.hahajie.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://sb.bookmarksfly.cn

[U104] JS：防抖
来源：http://sj.panjiajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lm.asd995.cn

[U105] JS：节流
来源：http://oc.huixiangedu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://by.colortex.cn

[U106] JS：日期格式化
来源：http://xe.colortex.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ov.nszjky.cn

[U107] JS：数字千分位
来源：http://li.shxzskj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zl.yuntaijiaju.cn

[U108] JS：随机整数
来源：http://ko.hnjuh.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jh.shtwfgs.cn

[U109] JS：数组分组
来源：http://mk.haigaiapp.cn

Object.groupBy(arr, x => x.type)
来源：http://oy.huixiangedu.cn

[U110] JS：数组分块
来源：http://lt.shxzukj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ij.nicolike.cn

[U111] JS：对象转 Map
来源：http://mf.szsharing.cn

new Map(Object.entries(obj))
来源：http://ua.szxytkj.cn

[U112] JS：字符串补位
来源：http://rz.panjiajie.cn

"7".padStart(3, "0")
来源：http://tz.jctech888.com.cn

[U113] JS：正则替换全部
来源：http://sd.shxzukj.cn

s.replaceAll("a", "b")
来源：http://cu.muxihuayi.cn

[U114] JS：JSON 深比较
来源：http://nh.nicolike.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://mb.9csxet.cn

[U115] JS：生成 UUID
来源：http://in.huixiangedu.cn

crypto.randomUUID()
来源：http://ak.521024.cn

[U116] JS：类型检查（JSDoc）
来源：http://qk.huixinmuqiang.cn

/** @param {string} name */ function f(name) {}
来源：http://ks.gzmigu.cn

[U117] JS：单元测试
来源：http://fl.shxzukj.cn

npm i -D vitest;  npx vitest
来源：http://ah.yuntaijiaju.cn

[U118] JS：开发服务器
来源：http://ae.bjjhwx.cn

npm i -D vite;  npx vite
来源：http://sk.chemitech.net.cn

[U119] JS：生产构建
来源：http://fw.huanxung.cn

npx vite build
来源：http://fm.asd995.cn

[U120] JS：读取环境变量（Vite）
来源：http://rf.hnjuh.cn

import.meta.env.VITE_API_URL
来源：http://ys.jctech888.com.cn

================================================================================
来源：http://rl.jctech888.com.cn

统计汇总
来源：http://pv.nszjky.cn

================================================================================
来源：http://vs.shxzukj.cn

按语言统计（条）：
来源：http://jf.nicolike.cn

Python ......... 252
来源：http://qk.panjiajie.cn

PHP ............ 252
来源：http://js.muxihuayi.cn

JavaScript ..... 252
来源：http://yk.shxzukj.cn

TypeScript ..... 212
来源：http://cz.shxzskj.cn

Java ........... 212
来源：http://gd.haigaiapp.cn

Go ............. 212
来源：http://vm.haigaiapp.cn

Ruby ........... 212
来源：http://jq.asd995.cn

C# ............. 212
来源：http://rl.szxytkj.cn

C .............. 30
来源：http://ro.muxihuayi.cn

C++ ............ 30
来源：http://nl.newstarts.cn

SQL ............ 90
来源：http://tx.huixiangedu.cn

Bash ........... 80
来源：http://jw.chemitech.net.cn

Kotlin ......... 15
来源：http://nr.nszjky.cn

Swift .......... 15
来源：http://cs.szsharing.cn

Lua ............ 10
来源：http://ra.shtwfgs.cn

Perl ........... 10
来源：http://df.jctech888.com.cn

Scala .......... 10
来源：http://hx.shxzskj.cn

------------------------------------
来源：http://tx.panjiajie.cn

合计 ........... 2106 条
来源：http://hy.jianghongdianzi.cn

按章节统计：
来源：http://ag.szxytkj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://aw.jctech888.com.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://sn.hahajie.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://sb.jianghongdianzi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gx.panjiajie.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://oy.yuntaijiaju.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rt.jctech888.com.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pb.huixinmuqiang.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tx.shxzskj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fh.jianghongdianzi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ut.jianghongdianzi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xi.haigaiapp.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ku.haigaiapp.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://to.panjiajie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ng.huixinmuqiang.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ku.bjjhwx.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ny.yuexingan06.cn

Q SQL 专题                              90
来源：http://xo.szsharing.cn

R Bash 专题                             80
来源：http://vl.nszjky.cn

S C / C++ 专题                          60
来源：http://iq.bookmarksfly.cn

T 其他语言补充                          60
来源：http://ds.521024.cn

U 高频实用片段                         120
来源：http://yt.jianghongdianzi.cn

------------------------------------
来源：http://au.asd995.cn

合计                                  2106 条
来源：http://mf.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://zb.bjjhwx.cn

使用提醒
来源：http://gv.huanxung.cn

--------------------------------------------------------------------------------
来源：http://gc.shxzukj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wn.yuexingan06.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rs.lnxyls.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lz.shtwfgs.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ky.chemitech.net.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://py.lnxyls.cn

—— 文件结束 ——
来源：http://fa.hnjuh.cn

================================================================================
来源：http://xf.huixiangedu.cn

程序语言常见例子速查手册（2024 版）
来源：http://ur.shtwfgs.cn

Common Programming Examples Cheat Book
来源：http://sd.nicolike.cn

================================================================================
来源：http://pi.newstarts.cn

【收录内容】
来源：http://hu.gzmigu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://hb.yuntaijiaju.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ht.521024.cn

SQL · Bash · C · C++
来源：http://oj.nicolike.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://js.huanxung.cn

【使用说明】
来源：http://nx.asd995.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://sq.shxzukj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://we.muxihuayi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rp.521024.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://me.lnxyls.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://dg.huixiangedu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://if.shtwfgs.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tx.yuntaijiaju.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qd.lnxyls.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://dj.jctech888.com.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://aa.jctech888.com.cn


<!-- 参考信息 -->