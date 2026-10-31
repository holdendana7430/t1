代发 wailian999

[U05] Py：列表去重且保序
来源：http://na.hahajie.cn

list(dict.fromkeys(arr))
来源：http://lu.jctech888.com.cn

[U06] Py：合并两个字典
来源：http://zu.huanxung.cn

{**a, **b}
来源：http://wt.shxzskj.cn

[U07] Py：反转字典键值
来源：http://zl.newstarts.cn

{v: k for k, v in d.items()}
来源：http://ya.hahajie.cn

[U08] Py：展平二维列表
来源：http://yw.szsharing.cn

[y for x in nested for y in x]
来源：http://ur.521024.cn

[U09] Py：字典取最大值的键
来源：http://ex.9csxet.cn

max(d, key=d.get)
来源：http://vf.huixiangedu.cn

[U10] Py：按值排序字典
来源：http://zm.huixinmuqiang.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ww.asd995.cn

[U11] Py：生成器表达式
来源：http://xg.9csxet.cn

(x * 2 for x in arr)
来源：http://jq.bookmarksfly.cn

[U12] Py：取出现最多的 3 个元素
来源：http://sy.huixiangedu.cn

Counter(arr).most_common(3)
来源：http://sd.muxihuayi.cn

[U13] Py：固定长度队列
来源：http://cu.shxzskj.cn

deque(maxlen=10)
来源：http://ii.newstarts.cn

[U14] Py：分组收集到列表
来源：http://mv.9csxet.cn

defaultdict(list)
来源：http://dv.yuntaijiaju.cn

[U15] Py：高精度计时
来源：http://tw.bookmarksfly.cn

t = time.perf_counter()
来源：http://yj.newstarts.cn

[U16] Py：命令行参数解析
来源：http://da.nszjky.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hh.gzmigu.cn

[U17] Py：初始化日志
来源：http://lv.shtwfgs.cn

logging.basicConfig(level=logging.INFO)
来源：http://ep.hahajie.cn

[U18] Py：预编译正则
来源：http://kj.muxihuayi.cn

pat = re.compile(r"\d+")
来源：http://tu.jianghongdianzi.cn

[U19] Py：正则替换带回调
来源：http://bt.asd995.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nl.asd995.cn

[U20] Py：缓存函数结果
来源：http://pa.chemitech.net.cn

@functools.lru_cache(maxsize=None)
来源：http://ut.muxihuayi.cn

[U21] Py：自定义上下文管理器
来源：http://bg.lnxyls.cn

@contextlib.contextmanager
来源：http://nt.newstarts.cn

[U22] Py：矩阵转置
来源：http://uw.colortex.cn

list(zip(*m))
来源：http://sa.jctech888.com.cn

[U23] Py：分块读取大文件
来源：http://yv.shtwfgs.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://np.szxytkj.cn

[U24] Py：路径操作
来源：http://oz.nicolike.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jb.shtwfgs.cn

[U25] Py：CSV 按字典读
来源：http://tj.szsharing.cn

csv.DictReader(f)
来源：http://uu.jianghongdianzi.cn

[U26] Py：并发下载
来源：http://wz.jctech888.com.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xj.chemitech.net.cn

[U27] Py：异步 HTTP
来源：http://fx.huixiangedu.cn

aiohttp.ClientSession() 配合 async with
来源：http://on.bookmarksfly.cn

[U28] Py：类型别名
来源：http://wu.colortex.cn

UserId = int
来源：http://gn.gzmigu.cn

[U29] Py：属性校验
来源：http://sn.colortex.cn

@property 与 @x.setter 配合
来源：http://ld.muxihuayi.cn

[U30] Py：数据类
来源：http://ev.huixiangedu.cn

@dataclass(slots=True)
来源：http://yq.jianghongdianzi.cn

[U31] Py：单测
来源：http://ji.huixiangedu.cn

python -m pytest -q
来源：http://ch.9csxet.cn

[U32] Py：代码格式化
来源：http://os.lnxyls.cn

ruff format . && ruff check --fix .
来源：http://gi.huixiangedu.cn

[U33] Py：打包发布
来源：http://jx.huixinmuqiang.cn

python -m build  （依赖 pyproject.toml）
来源：http://zp.jctech888.com.cn

[U34] Py：判断编码
来源：http://xt.521024.cn

chardet.detect(raw)
来源：http://up.yuntaijiaju.cn

[U35] Py：发送邮件
来源：http://en.hahajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ze.nszjky.cn

[U36] Py：定时任务
来源：http://qj.jctech888.com.cn

schedule.every(10).minutes.do(job)
来源：http://lf.shxzskj.cn

[U37] Py：读写 Excel
来源：http://nz.huanxung.cn

pandas.read_excel / DataFrame.to_excel
来源：http://dx.yuntaijiaju.cn

[U38] Py：获取脚本所在目录
来源：http://jy.szxytkj.cn

Path(__file__).resolve().parent
来源：http://wa.szxytkj.cn

[U39] Py：判断是否在交互环境
来源：http://ez.haigaiapp.cn

sys.stdout.isatty()
来源：http://xk.shxzskj.cn

[U40] Py：打印到标准错误
来源：http://ql.chemitech.net.cn

print("err", file=sys.stderr)
来源：http://wl.shtwfgs.cn

[U41] PHP：初始化 Composer 项目
来源：http://gx.szxytkj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://wz.asd995.cn

[U42] PHP：PSR-4 自动加载
来源：http://wh.szsharing.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vh.newstarts.cn

[U43] PHP：声明命名空间
来源：http://jn.bjjhwx.cn

namespace App\Http;
来源：http://wm.shxzskj.cn

[U44] PHP：开启严格类型
来源：http://hp.gzmigu.cn

declare(strict_types=1);
来源：http://mj.nicolike.cn

[U45] PHP：类型声明与返回类型
来源：http://fq.nicolike.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://nw.shxzskj.cn

[U46] PHP：可空类型
来源：http://pi.521024.cn

?string $name = null
来源：http://qd.9csxet.cn

[U47] PHP：联合类型
来源：http://cw.huixiangedu.cn

int|string $id
来源：http://zu.huixinmuqiang.cn

[U48] PHP：纯枚举
来源：http://tf.jctech888.com.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cn.jianghongdianzi.cn

[U49] PHP：只读属性
来源：http://pd.shxzukj.cn

public readonly string $name
来源：http://nu.szsharing.cn

[U50] PHP：构造器属性提升
来源：http://kl.huixiangedu.cn

public function __construct(private int $id) {}
来源：http://gn.asd995.cn

[U51] PHP：数组解构
来源：http://ue.hahajie.cn

[$a, $b] = $arr;
来源：http://fe.yuexingan06.cn

[U52] PHP：箭头函数
来源：http://gj.newstarts.cn

$double = fn($x) => $x * 2;
来源：http://zz.lnxyls.cn

[U53] PHP：空合并运算符
来源：http://fa.shxzskj.cn

$v = $a ?? $b ?? "default";
来源：http://gt.jianghongdianzi.cn

[U54] PHP：空安全调用
来源：http://hx.hnjuh.cn

$obj?->method()
来源：http://pj.lnxyls.cn

[U55] PHP：match 表达式
来源：http://am.nicolike.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rj.huixinmuqiang.cn

[U56] PHP：命名参数
来源：http://pv.lnxyls.cn

f(a: 1, b: 2)
来源：http://kx.bookmarksfly.cn

[U57] PHP：字符串插值
来源：http://dq.asd995.cn

"值: {$a}"
来源：http://xf.yuntaijiaju.cn

[U58] PHP：数组三件套
来源：http://xy.hahajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ix.shxzskj.cn

[U59] PHP：自定义排序
来源：http://kq.colortex.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bv.lnxyls.cn

[U60] PHP：JSON 编解码
来源：http://lr.gzmigu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kk.yuexingan06.cn

[U61] PHP：正则
来源：http://fe.gzmigu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://am.jianghongdianzi.cn

[U62] PHP：日期对象
来源：http://zj.nszjky.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fe.jctech888.com.cn

[U63] PHP：文件读写
来源：http://hf.jianghongdianzi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kg.haigaiapp.cn

[U64] PHP：目录遍历
来源：http://wi.gzmigu.cn

glob("dir/*.php");  scandir("dir");
来源：http://dy.huanxung.cn

[U65] PHP：会话
来源：http://lj.hahajie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://dw.huanxung.cn

[U66] PHP：设置 Cookie
来源：http://kd.yuexingan06.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nk.gzmigu.cn

[U67] PHP：处理文件上传
来源：http://ol.wgjwhj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bn.panjiajie.cn

[U68] PHP：PDO 连接
来源：http://tq.jctech888.com.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nj.szxytkj.cn

[U69] PHP：PDO 预处理
来源：http://lj.9csxet.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://on.hnjuh.cn

[U70] PHP：PDO 事务
来源：http://np.wgjwhj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rm.9csxet.cn

[U71] PHP：抛出异常
来源：http://tg.gzmigu.cn

throw new RuntimeException("失败", 500);
来源：http://sl.wgjwhj.cn

[U72] PHP：写错误日志
来源：http://ow.shtwfgs.cn

error_log("失败: " . $e->getMessage());
来源：http://bj.szsharing.cn

[U73] PHP：读取 ini 配置
来源：http://ea.9csxet.cn

parse_ini_file("config.ini", true)
来源：http://uj.huanxung.cn

[U74] PHP：读取环境变量
来源：http://sm.bookmarksfly.cn

getenv("APP_ENV") ?: "production"
来源：http://co.szsharing.cn

[U75] PHP：依赖注入
来源：http://sp.jctech888.com.cn

composer require psr/container
来源：http://cd.nszjky.cn

[U76] PHP：简单路由
来源：http://eq.chemitech.net.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sf.panjiajie.cn

[U77] PHP：模板渲染
来源：http://uj.9csxet.cn

composer require twig/twig
来源：http://aa.bookmarksfly.cn

[U78] PHP：单元测试
来源：http://op.nicolike.cn

composer require --dev phpunit/phpunit
来源：http://cf.hnjuh.cn

[U79] PHP：静态分析
来源：http://qv.shtwfgs.cn

composer require --dev phpstan/phpstan
来源：http://vg.huixinmuqiang.cn

[U80] PHP：代码规范修复
来源：http://ck.gzmigu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://po.shtwfgs.cn

[U81] JS：初始化项目
来源：http://xb.panjiajie.cn

npm init -y;  npm i express
来源：http://jl.lnxyls.cn

[U82] JS：package.json 脚本
来源：http://cd.szsharing.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ln.yuexingan06.cn

[U83] JS：ES Module 导入导出
来源：http://gz.shtwfgs.cn

export const a = 1;  import { a } from "./m.js";
来源：http://pi.bjjhwx.cn

[U84] JS：CommonJS 写法
来源：http://xs.haigaiapp.cn

module.exports = { a };  const { a } = require("./m");
来源：http://df.jctech888.com.cn

[U85] JS：可选链
来源：http://ll.shxzukj.cn

a?.b?.c
来源：http://fs.colortex.cn

[U86] JS：空值合并
来源：http://qz.shxzukj.cn

a ?? b
来源：http://ej.szxytkj.cn

[U87] JS：解构默认值
来源：http://ta.521024.cn

const { a = 1, b = 2 } = obj;
来源：http://xq.huixinmuqiang.cn

[U88] JS：对象展开合并
来源：http://gy.shtwfgs.cn

{ ...a, ...b }
来源：http://bc.yuexingan06.cn

[U89] JS：数组去重
来源：http://yk.hahajie.cn

[...new Set(arr)]
来源：http://mo.colortex.cn

[U90] JS：数字数组排序
来源：http://qq.haigaiapp.cn

[...arr].sort((a, b) => a - b)
来源：http://la.shxzukj.cn

[U91] JS：对象键值遍历
来源：http://kg.szxytkj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cm.huanxung.cn

[U92] JS：深拷贝
来源：http://vz.hahajie.cn

structuredClone(obj)
来源：http://dw.chemitech.net.cn

[U93] JS：模板字符串
来源：http://yw.szxytkj.cn

`共 ${n} 条`
来源：http://pi.szsharing.cn

[U94] JS：箭头函数
来源：http://cs.shxzskj.cn

const double = x => x * 2;
来源：http://fi.hnjuh.cn

[U95] JS：Promise 包装
来源：http://tm.szsharing.cn

new Promise((resolve, reject) => {})
来源：http://bf.huanxung.cn

[U96] JS：async/await 与异常
来源：http://xm.bjjhwx.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xv.shxzukj.cn

[U97] JS：并发请求
来源：http://dt.colortex.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ul.hnjuh.cn

[U98] JS：fetch 带 JSON
来源：http://vt.muxihuayi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mu.nicolike.cn

[U99] JS：事件监听
来源：http://og.asd995.cn

el.addEventListener("click", e => {})
来源：http://qo.szxytkj.cn

[U100] JS：DOM 查询
来源：http://pb.asd995.cn

document.querySelector(".item")
来源：http://sl.colortex.cn

[U101] JS：classList 操作
来源：http://ek.szxytkj.cn

el.classList.toggle("active")
来源：http://od.newstarts.cn

[U102] JS：本地存储
来源：http://lx.gzmigu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ok.hahajie.cn

[U103] JS：定时器
来源：http://dq.szsharing.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://my.huixinmuqiang.cn

[U104] JS：防抖
来源：http://sy.shxzskj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kw.bookmarksfly.cn

[U105] JS：节流
来源：http://hn.haigaiapp.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ip.wgjwhj.cn

[U106] JS：日期格式化
来源：http://at.hnjuh.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ap.yuntaijiaju.cn

[U107] JS：数字千分位
来源：http://qn.yuntaijiaju.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xr.jianghongdianzi.cn

[U108] JS：随机整数
来源：http://ln.huixinmuqiang.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ue.nszjky.cn

[U109] JS：数组分组
来源：http://xk.szsharing.cn

Object.groupBy(arr, x => x.type)
来源：http://xz.muxihuayi.cn

[U110] JS：数组分块
来源：http://xa.521024.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://aj.521024.cn

[U111] JS：对象转 Map
来源：http://ak.shxzukj.cn

new Map(Object.entries(obj))
来源：http://oz.asd995.cn

[U112] JS：字符串补位
来源：http://ac.szsharing.cn

"7".padStart(3, "0")
来源：http://rh.bookmarksfly.cn

[U113] JS：正则替换全部
来源：http://yx.huixiangedu.cn

s.replaceAll("a", "b")
来源：http://go.521024.cn

[U114] JS：JSON 深比较
来源：http://dt.521024.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://au.hnjuh.cn

[U115] JS：生成 UUID
来源：http://kf.huanxung.cn

crypto.randomUUID()
来源：http://ej.shxzskj.cn

[U116] JS：类型检查（JSDoc）
来源：http://se.nszjky.cn

/** @param {string} name */ function f(name) {}
来源：http://pn.asd995.cn

[U117] JS：单元测试
来源：http://jc.521024.cn

npm i -D vitest;  npx vitest
来源：http://ff.jctech888.com.cn

[U118] JS：开发服务器
来源：http://uo.colortex.cn

npm i -D vite;  npx vite
来源：http://av.nicolike.cn

[U119] JS：生产构建
来源：http://hz.9csxet.cn

npx vite build
来源：http://mc.chemitech.net.cn

[U120] JS：读取环境变量（Vite）
来源：http://bk.newstarts.cn

import.meta.env.VITE_API_URL
来源：http://fp.haigaiapp.cn

================================================================================
来源：http://fc.panjiajie.cn

统计汇总
来源：http://hw.chemitech.net.cn

================================================================================
来源：http://kd.newstarts.cn

按语言统计（条）：
来源：http://zz.nicolike.cn

Python ......... 252
来源：http://nq.bjjhwx.cn

PHP ............ 252
来源：http://fe.muxihuayi.cn

JavaScript ..... 252
来源：http://ti.hnjuh.cn

TypeScript ..... 212
来源：http://xq.nicolike.cn

Java ........... 212
来源：http://gk.huixinmuqiang.cn

Go ............. 212
来源：http://jz.yuntaijiaju.cn

Ruby ........... 212
来源：http://dy.bjjhwx.cn

C# ............. 212
来源：http://tv.chemitech.net.cn

C .............. 30
来源：http://yq.szsharing.cn

C++ ............ 30
来源：http://vi.hnjuh.cn

SQL ............ 90
来源：http://ya.szxytkj.cn

Bash ........... 80
来源：http://xo.9csxet.cn

Kotlin ......... 15
来源：http://cq.hnjuh.cn

Swift .......... 15
来源：http://zq.nicolike.cn

Lua ............ 10
来源：http://nx.panjiajie.cn

Perl ........... 10
来源：http://mk.wgjwhj.cn

Scala .......... 10
来源：http://tk.shxzskj.cn

------------------------------------
来源：http://gg.muxihuayi.cn

合计 ........... 2106 条
来源：http://zz.lnxyls.cn

按章节统计：
来源：http://pk.bjjhwx.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xz.yuntaijiaju.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://sz.panjiajie.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://px.szxytkj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.bookmarksfly.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nd.bjjhwx.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wd.colortex.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://sc.gzmigu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://sm.panjiajie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lj.hahajie.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xo.asd995.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ew.wgjwhj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rs.newstarts.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nj.yuntaijiaju.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ch.wgjwhj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ld.521024.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gj.shxzukj.cn

Q SQL 专题                              90
来源：http://ky.bjjhwx.cn

R Bash 专题                             80
来源：http://sr.yuexingan06.cn

S C / C++ 专题                          60
来源：http://mh.asd995.cn

T 其他语言补充                          60
来源：http://fo.muxihuayi.cn

U 高频实用片段                         120
来源：http://tb.szsharing.cn

------------------------------------
来源：http://hh.9csxet.cn

合计                                  2106 条
来源：http://ym.9csxet.cn

--------------------------------------------------------------------------------
来源：http://fv.yuntaijiaju.cn

使用提醒
来源：http://uu.newstarts.cn

--------------------------------------------------------------------------------
来源：http://mn.nicolike.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://op.shtwfgs.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://yg.szsharing.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ig.bookmarksfly.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://vy.hnjuh.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://uv.muxihuayi.cn

—— 文件结束 ——
来源：http://wj.yuexingan06.cn

================================================================================
来源：http://zb.nicolike.cn

程序语言常见例子速查手册（2024 版）
来源：http://or.lnxyls.cn

Common Programming Examples Cheat Book
来源：http://tq.wgjwhj.cn

================================================================================
来源：http://et.gzmigu.cn

【收录内容】
来源：http://yc.jctech888.com.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://fk.shxzskj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zx.chemitech.net.cn

SQL · Bash · C · C++
来源：http://wn.hnjuh.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mn.newstarts.cn

【使用说明】
来源：http://ds.9csxet.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rt.lnxyls.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://lh.wgjwhj.cn


<!-- 参考信息 -->