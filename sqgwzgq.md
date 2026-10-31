代发 wailian999

[U05] Py：列表去重且保序
来源：http://mp.chemitech.net.cn

list(dict.fromkeys(arr))
来源：http://lz.gzmigu.cn

[U06] Py：合并两个字典
来源：http://mr.hnjuh.cn

{**a, **b}
来源：http://yu.shtwfgs.cn

[U07] Py：反转字典键值
来源：http://yk.newstarts.cn

{v: k for k, v in d.items()}
来源：http://lr.hnjuh.cn

[U08] Py：展平二维列表
来源：http://aw.colortex.cn

[y for x in nested for y in x]
来源：http://sb.shxzskj.cn

[U09] Py：字典取最大值的键
来源：http://mk.szxytkj.cn

max(d, key=d.get)
来源：http://ur.shxzukj.cn

[U10] Py：按值排序字典
来源：http://vz.gzmigu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gt.hahajie.cn

[U11] Py：生成器表达式
来源：http://jb.szsharing.cn

(x * 2 for x in arr)
来源：http://rc.bookmarksfly.cn

[U12] Py：取出现最多的 3 个元素
来源：http://oh.huixiangedu.cn

Counter(arr).most_common(3)
来源：http://ga.szxytkj.cn

[U13] Py：固定长度队列
来源：http://gn.szxytkj.cn

deque(maxlen=10)
来源：http://uj.newstarts.cn

[U14] Py：分组收集到列表
来源：http://tm.muxihuayi.cn

defaultdict(list)
来源：http://ul.shxzskj.cn

[U15] Py：高精度计时
来源：http://mn.szsharing.cn

t = time.perf_counter()
来源：http://vf.huanxung.cn

[U16] Py：命令行参数解析
来源：http://cn.lnxyls.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zt.szsharing.cn

[U17] Py：初始化日志
来源：http://pn.jctech888.com.cn

logging.basicConfig(level=logging.INFO)
来源：http://np.muxihuayi.cn

[U18] Py：预编译正则
来源：http://wz.jianghongdianzi.cn

pat = re.compile(r"\d+")
来源：http://yq.nicolike.cn

[U19] Py：正则替换带回调
来源：http://eg.9csxet.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nr.huixinmuqiang.cn

[U20] Py：缓存函数结果
来源：http://om.bookmarksfly.cn

@functools.lru_cache(maxsize=None)
来源：http://dp.jianghongdianzi.cn

[U21] Py：自定义上下文管理器
来源：http://cb.newstarts.cn

@contextlib.contextmanager
来源：http://dj.yuntaijiaju.cn

[U22] Py：矩阵转置
来源：http://dy.hnjuh.cn

list(zip(*m))
来源：http://iz.newstarts.cn

[U23] Py：分块读取大文件
来源：http://fb.wgjwhj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ws.521024.cn

[U24] Py：路径操作
来源：http://du.asd995.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zb.shxzskj.cn

[U25] Py：CSV 按字典读
来源：http://hu.jctech888.com.cn

csv.DictReader(f)
来源：http://ic.szsharing.cn

[U26] Py：并发下载
来源：http://wi.521024.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qx.shtwfgs.cn

[U27] Py：异步 HTTP
来源：http://oz.hahajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://ah.yuexingan06.cn

[U28] Py：类型别名
来源：http://aq.asd995.cn

UserId = int
来源：http://pe.szxytkj.cn

[U29] Py：属性校验
来源：http://hf.newstarts.cn

@property 与 @x.setter 配合
来源：http://mn.9csxet.cn

[U30] Py：数据类
来源：http://yu.hahajie.cn

@dataclass(slots=True)
来源：http://ii.huixinmuqiang.cn

[U31] Py：单测
来源：http://ko.huanxung.cn

python -m pytest -q
来源：http://ao.gzmigu.cn

[U32] Py：代码格式化
来源：http://wo.panjiajie.cn

ruff format . && ruff check --fix .
来源：http://fh.haigaiapp.cn

[U33] Py：打包发布
来源：http://cf.szxytkj.cn

python -m build  （依赖 pyproject.toml）
来源：http://kz.gzmigu.cn

[U34] Py：判断编码
来源：http://et.newstarts.cn

chardet.detect(raw)
来源：http://dl.colortex.cn

[U35] Py：发送邮件
来源：http://tb.muxihuayi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ha.colortex.cn

[U36] Py：定时任务
来源：http://ht.bookmarksfly.cn

schedule.every(10).minutes.do(job)
来源：http://gd.chemitech.net.cn

[U37] Py：读写 Excel
来源：http://qc.9csxet.cn

pandas.read_excel / DataFrame.to_excel
来源：http://yu.wgjwhj.cn

[U38] Py：获取脚本所在目录
来源：http://tm.jianghongdianzi.cn

Path(__file__).resolve().parent
来源：http://ez.jctech888.com.cn

[U39] Py：判断是否在交互环境
来源：http://fo.gzmigu.cn

sys.stdout.isatty()
来源：http://tu.shtwfgs.cn

[U40] Py：打印到标准错误
来源：http://ku.hahajie.cn

print("err", file=sys.stderr)
来源：http://qg.huanxung.cn

[U41] PHP：初始化 Composer 项目
来源：http://uf.muxihuayi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ak.haigaiapp.cn

[U42] PHP：PSR-4 自动加载
来源：http://oo.shxzukj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dz.nszjky.cn

[U43] PHP：声明命名空间
来源：http://sd.bookmarksfly.cn

namespace App\Http;
来源：http://qg.lnxyls.cn

[U44] PHP：开启严格类型
来源：http://up.bjjhwx.cn

declare(strict_types=1);
来源：http://rc.shtwfgs.cn

[U45] PHP：类型声明与返回类型
来源：http://kj.szxytkj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://su.newstarts.cn

[U46] PHP：可空类型
来源：http://su.muxihuayi.cn

?string $name = null
来源：http://pz.gzmigu.cn

[U47] PHP：联合类型
来源：http://tw.nszjky.cn

int|string $id
来源：http://ci.yuexingan06.cn

[U48] PHP：纯枚举
来源：http://dj.yuntaijiaju.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tx.bookmarksfly.cn

[U49] PHP：只读属性
来源：http://iw.wgjwhj.cn

public readonly string $name
来源：http://vs.hahajie.cn

[U50] PHP：构造器属性提升
来源：http://ut.bookmarksfly.cn

public function __construct(private int $id) {}
来源：http://wq.huanxung.cn

[U51] PHP：数组解构
来源：http://wd.yuexingan06.cn

[$a, $b] = $arr;
来源：http://xa.nszjky.cn

[U52] PHP：箭头函数
来源：http://za.bookmarksfly.cn

$double = fn($x) => $x * 2;
来源：http://mb.newstarts.cn

[U53] PHP：空合并运算符
来源：http://ho.bjjhwx.cn

$v = $a ?? $b ?? "default";
来源：http://ln.wgjwhj.cn

[U54] PHP：空安全调用
来源：http://sy.gzmigu.cn

$obj?->method()
来源：http://og.huanxung.cn

[U55] PHP：match 表达式
来源：http://be.bookmarksfly.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ea.lnxyls.cn

[U56] PHP：命名参数
来源：http://xm.bookmarksfly.cn

f(a: 1, b: 2)
来源：http://ip.jctech888.com.cn

[U57] PHP：字符串插值
来源：http://lj.huanxung.cn

"值: {$a}"
来源：http://ub.asd995.cn

[U58] PHP：数组三件套
来源：http://pr.shxzskj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ky.newstarts.cn

[U59] PHP：自定义排序
来源：http://tx.haigaiapp.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gl.nicolike.cn

[U60] PHP：JSON 编解码
来源：http://vm.yuexingan06.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bw.newstarts.cn

[U61] PHP：正则
来源：http://ud.hnjuh.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gk.huanxung.cn

[U62] PHP：日期对象
来源：http://ob.colortex.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cg.hahajie.cn

[U63] PHP：文件读写
来源：http://ex.shtwfgs.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hs.wgjwhj.cn

[U64] PHP：目录遍历
来源：http://iv.yuexingan06.cn

glob("dir/*.php");  scandir("dir");
来源：http://la.bookmarksfly.cn

[U65] PHP：会话
来源：http://tc.bookmarksfly.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vu.yuntaijiaju.cn

[U66] PHP：设置 Cookie
来源：http://qh.yuntaijiaju.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ju.haigaiapp.cn

[U67] PHP：处理文件上传
来源：http://jh.muxihuayi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://as.jianghongdianzi.cn

[U68] PHP：PDO 连接
来源：http://ab.wgjwhj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ox.521024.cn

[U69] PHP：PDO 预处理
来源：http://sy.wgjwhj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yv.newstarts.cn

[U70] PHP：PDO 事务
来源：http://kj.newstarts.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tv.hahajie.cn

[U71] PHP：抛出异常
来源：http://qx.hnjuh.cn

throw new RuntimeException("失败", 500);
来源：http://da.asd995.cn

[U72] PHP：写错误日志
来源：http://fk.bjjhwx.cn

error_log("失败: " . $e->getMessage());
来源：http://sg.wgjwhj.cn

[U73] PHP：读取 ini 配置
来源：http://fl.huixinmuqiang.cn

parse_ini_file("config.ini", true)
来源：http://vu.nszjky.cn

[U74] PHP：读取环境变量
来源：http://pg.521024.cn

getenv("APP_ENV") ?: "production"
来源：http://cj.gzmigu.cn

[U75] PHP：依赖注入
来源：http://rq.bookmarksfly.cn

composer require psr/container
来源：http://gw.bjjhwx.cn

[U76] PHP：简单路由
来源：http://yl.521024.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ri.jianghongdianzi.cn

[U77] PHP：模板渲染
来源：http://hb.bookmarksfly.cn

composer require twig/twig
来源：http://gw.szsharing.cn

[U78] PHP：单元测试
来源：http://qq.panjiajie.cn

composer require --dev phpunit/phpunit
来源：http://qo.9csxet.cn

[U79] PHP：静态分析
来源：http://jx.jctech888.com.cn

composer require --dev phpstan/phpstan
来源：http://do.yuexingan06.cn

[U80] PHP：代码规范修复
来源：http://ap.huixiangedu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qp.lnxyls.cn

[U81] JS：初始化项目
来源：http://ef.jianghongdianzi.cn

npm init -y;  npm i express
来源：http://at.bjjhwx.cn

[U82] JS：package.json 脚本
来源：http://zc.haigaiapp.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nc.newstarts.cn

[U83] JS：ES Module 导入导出
来源：http://rm.huanxung.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ir.wgjwhj.cn

[U84] JS：CommonJS 写法
来源：http://zi.haigaiapp.cn

module.exports = { a };  const { a } = require("./m");
来源：http://bs.hahajie.cn

[U85] JS：可选链
来源：http://cp.hnjuh.cn

a?.b?.c
来源：http://cw.chemitech.net.cn

[U86] JS：空值合并
来源：http://tn.hahajie.cn

a ?? b
来源：http://ck.huixiangedu.cn

[U87] JS：解构默认值
来源：http://lw.bjjhwx.cn

const { a = 1, b = 2 } = obj;
来源：http://qk.jctech888.com.cn

[U88] JS：对象展开合并
来源：http://fk.szxytkj.cn

{ ...a, ...b }
来源：http://bf.huixinmuqiang.cn

[U89] JS：数组去重
来源：http://zd.huanxung.cn

[...new Set(arr)]
来源：http://vm.shtwfgs.cn

[U90] JS：数字数组排序
来源：http://cw.yuexingan06.cn

[...arr].sort((a, b) => a - b)
来源：http://me.wgjwhj.cn

[U91] JS：对象键值遍历
来源：http://cm.haigaiapp.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yv.szxytkj.cn

[U92] JS：深拷贝
来源：http://nl.huixiangedu.cn

structuredClone(obj)
来源：http://fs.lnxyls.cn

[U93] JS：模板字符串
来源：http://xn.521024.cn

`共 ${n} 条`
来源：http://fl.muxihuayi.cn

[U94] JS：箭头函数
来源：http://ii.szsharing.cn

const double = x => x * 2;
来源：http://vb.lnxyls.cn

[U95] JS：Promise 包装
来源：http://it.bjjhwx.cn

new Promise((resolve, reject) => {})
来源：http://qs.szsharing.cn

[U96] JS：async/await 与异常
来源：http://tz.jctech888.com.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vc.panjiajie.cn

[U97] JS：并发请求
来源：http://zt.shxzskj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://au.bjjhwx.cn

[U98] JS：fetch 带 JSON
来源：http://dx.hnjuh.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://py.bookmarksfly.cn

[U99] JS：事件监听
来源：http://ar.521024.cn

el.addEventListener("click", e => {})
来源：http://db.panjiajie.cn

[U100] JS：DOM 查询
来源：http://sn.colortex.cn

document.querySelector(".item")
来源：http://he.muxihuayi.cn

[U101] JS：classList 操作
来源：http://pa.hahajie.cn

el.classList.toggle("active")
来源：http://yc.szsharing.cn

[U102] JS：本地存储
来源：http://yj.colortex.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://pa.jctech888.com.cn

[U103] JS：定时器
来源：http://ca.shtwfgs.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fj.wgjwhj.cn

[U104] JS：防抖
来源：http://rj.bjjhwx.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://br.bjjhwx.cn

[U105] JS：节流
来源：http://ea.yuntaijiaju.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://oz.panjiajie.cn

[U106] JS：日期格式化
来源：http://uw.szxytkj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yv.colortex.cn

[U107] JS：数字千分位
来源：http://mn.szxytkj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hi.shxzukj.cn

[U108] JS：随机整数
来源：http://pc.gzmigu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gs.jctech888.com.cn

[U109] JS：数组分组
来源：http://wc.yuexingan06.cn

Object.groupBy(arr, x => x.type)
来源：http://oy.shxzukj.cn

[U110] JS：数组分块
来源：http://ge.hnjuh.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ln.jctech888.com.cn

[U111] JS：对象转 Map
来源：http://jl.shxzukj.cn

new Map(Object.entries(obj))
来源：http://zc.huixiangedu.cn

[U112] JS：字符串补位
来源：http://wl.bjjhwx.cn

"7".padStart(3, "0")
来源：http://ks.huixinmuqiang.cn

[U113] JS：正则替换全部
来源：http://to.nicolike.cn

s.replaceAll("a", "b")
来源：http://we.bookmarksfly.cn

[U114] JS：JSON 深比较
来源：http://gl.gzmigu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://py.521024.cn

[U115] JS：生成 UUID
来源：http://bv.asd995.cn

crypto.randomUUID()
来源：http://nc.chemitech.net.cn

[U116] JS：类型检查（JSDoc）
来源：http://ar.newstarts.cn

/** @param {string} name */ function f(name) {}
来源：http://yk.asd995.cn

[U117] JS：单元测试
来源：http://jy.bookmarksfly.cn

npm i -D vitest;  npx vitest
来源：http://ej.chemitech.net.cn

[U118] JS：开发服务器
来源：http://go.bjjhwx.cn

npm i -D vite;  npx vite
来源：http://pe.asd995.cn

[U119] JS：生产构建
来源：http://lv.yuntaijiaju.cn

npx vite build
来源：http://oq.asd995.cn

[U120] JS：读取环境变量（Vite）
来源：http://dp.newstarts.cn

import.meta.env.VITE_API_URL
来源：http://el.chemitech.net.cn

================================================================================
来源：http://iu.521024.cn

统计汇总
来源：http://li.yuexingan06.cn

================================================================================
来源：http://wo.szxytkj.cn

按语言统计（条）：
来源：http://hg.asd995.cn

Python ......... 252
来源：http://sj.nszjky.cn

PHP ............ 252
来源：http://ub.nicolike.cn

JavaScript ..... 252
来源：http://uk.shxzukj.cn

TypeScript ..... 212
来源：http://yu.colortex.cn

Java ........... 212
来源：http://ul.lnxyls.cn

Go ............. 212
来源：http://gh.hahajie.cn

Ruby ........... 212
来源：http://ox.shtwfgs.cn

C# ............. 212
来源：http://ls.yuntaijiaju.cn

C .............. 30
来源：http://ib.lnxyls.cn

C++ ............ 30
来源：http://jm.gzmigu.cn

SQL ............ 90
来源：http://il.panjiajie.cn

Bash ........... 80
来源：http://vx.nicolike.cn

Kotlin ......... 15
来源：http://qf.bookmarksfly.cn

Swift .......... 15
来源：http://pz.yuntaijiaju.cn

Lua ............ 10
来源：http://da.gzmigu.cn

Perl ........... 10
来源：http://gs.yuexingan06.cn

Scala .......... 10
来源：http://kq.nszjky.cn

------------------------------------
来源：http://un.szsharing.cn

合计 ........... 2106 条
来源：http://kq.shtwfgs.cn

按章节统计：
来源：http://rf.chemitech.net.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dp.nicolike.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nc.haigaiapp.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ty.asd995.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://by.hnjuh.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ay.hnjuh.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pz.yuntaijiaju.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kp.nszjky.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ea.521024.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vr.hnjuh.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yd.521024.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qx.521024.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fv.shxzukj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://do.shxzukj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pk.huanxung.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dr.shxzskj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rf.nicolike.cn

Q SQL 专题                              90
来源：http://yh.hnjuh.cn

R Bash 专题                             80
来源：http://wm.haigaiapp.cn

S C / C++ 专题                          60
来源：http://ij.chemitech.net.cn

T 其他语言补充                          60
来源：http://na.szxytkj.cn

U 高频实用片段                         120
来源：http://lv.nszjky.cn

------------------------------------
来源：http://dc.yuexingan06.cn

合计                                  2106 条
来源：http://sb.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://ud.shxzukj.cn

使用提醒
来源：http://by.hahajie.cn

--------------------------------------------------------------------------------
来源：http://eq.haigaiapp.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jo.hahajie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://yk.nszjky.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vu.yuntaijiaju.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://mr.bookmarksfly.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://tz.9csxet.cn

—— 文件结束 ——
来源：http://ab.jianghongdianzi.cn

================================================================================
来源：http://qp.szxytkj.cn

程序语言常见例子速查手册（2024 版）
来源：http://mj.asd995.cn

Common Programming Examples Cheat Book
来源：http://is.chemitech.net.cn

================================================================================
来源：http://hd.jctech888.com.cn

【收录内容】
来源：http://hl.muxihuayi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://yu.shxzskj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bj.chemitech.net.cn

SQL · Bash · C · C++
来源：http://kb.bookmarksfly.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://um.muxihuayi.cn

【使用说明】
来源：http://du.newstarts.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gc.huanxung.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bw.yuexingan06.cn


<!-- 参考信息 -->