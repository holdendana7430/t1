代发 wailian999

[U11] Py：生成器表达式
来源：http://mo.bjjhwx.cn

(x * 2 for x in arr)
来源：http://xc.521024.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ep.bjjhwx.cn

Counter(arr).most_common(3)
来源：http://mh.haigaiapp.cn

[U13] Py：固定长度队列
来源：http://vr.shtwfgs.cn

deque(maxlen=10)
来源：http://ru.9csxet.cn

[U14] Py：分组收集到列表
来源：http://pe.shtwfgs.cn

defaultdict(list)
来源：http://aq.newstarts.cn

[U15] Py：高精度计时
来源：http://ud.shxzukj.cn

t = time.perf_counter()
来源：http://qv.szsharing.cn

[U16] Py：命令行参数解析
来源：http://xm.huixinmuqiang.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wq.shxzukj.cn

[U17] Py：初始化日志
来源：http://bm.bjjhwx.cn

logging.basicConfig(level=logging.INFO)
来源：http://gp.lnxyls.cn

[U18] Py：预编译正则
来源：http://ue.jianghongdianzi.cn

pat = re.compile(r"\d+")
来源：http://sm.hahajie.cn

[U19] Py：正则替换带回调
来源：http://qe.szsharing.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lx.huixinmuqiang.cn

[U20] Py：缓存函数结果
来源：http://zj.nicolike.cn

@functools.lru_cache(maxsize=None)
来源：http://aq.nszjky.cn

[U21] Py：自定义上下文管理器
来源：http://xz.jctech888.com.cn

@contextlib.contextmanager
来源：http://yj.panjiajie.cn

[U22] Py：矩阵转置
来源：http://wk.nszjky.cn

list(zip(*m))
来源：http://nl.asd995.cn

[U23] Py：分块读取大文件
来源：http://hj.bjjhwx.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sm.panjiajie.cn

[U24] Py：路径操作
来源：http://kk.szsharing.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rl.muxihuayi.cn

[U25] Py：CSV 按字典读
来源：http://au.hnjuh.cn

csv.DictReader(f)
来源：http://qo.yuexingan06.cn

[U26] Py：并发下载
来源：http://sz.lnxyls.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rh.bookmarksfly.cn

[U27] Py：异步 HTTP
来源：http://dd.shxzskj.cn

aiohttp.ClientSession() 配合 async with
来源：http://kj.gzmigu.cn

[U28] Py：类型别名
来源：http://sq.9csxet.cn

UserId = int
来源：http://ri.szsharing.cn

[U29] Py：属性校验
来源：http://rp.huanxung.cn

@property 与 @x.setter 配合
来源：http://bt.bookmarksfly.cn

[U30] Py：数据类
来源：http://fi.asd995.cn

@dataclass(slots=True)
来源：http://vj.chemitech.net.cn

[U31] Py：单测
来源：http://vj.wgjwhj.cn

python -m pytest -q
来源：http://vf.muxihuayi.cn

[U32] Py：代码格式化
来源：http://gh.szxytkj.cn

ruff format . && ruff check --fix .
来源：http://dx.szsharing.cn

[U33] Py：打包发布
来源：http://ra.chemitech.net.cn

python -m build  （依赖 pyproject.toml）
来源：http://rt.newstarts.cn

[U34] Py：判断编码
来源：http://gk.szxytkj.cn

chardet.detect(raw)
来源：http://hn.wgjwhj.cn

[U35] Py：发送邮件
来源：http://mk.hahajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fu.lnxyls.cn

[U36] Py：定时任务
来源：http://os.huixinmuqiang.cn

schedule.every(10).minutes.do(job)
来源：http://ry.szxytkj.cn

[U37] Py：读写 Excel
来源：http://jx.hnjuh.cn

pandas.read_excel / DataFrame.to_excel
来源：http://yx.chemitech.net.cn

[U38] Py：获取脚本所在目录
来源：http://qn.wgjwhj.cn

Path(__file__).resolve().parent
来源：http://yv.asd995.cn

[U39] Py：判断是否在交互环境
来源：http://ts.chemitech.net.cn

sys.stdout.isatty()
来源：http://iy.wgjwhj.cn

[U40] Py：打印到标准错误
来源：http://ki.shxzukj.cn

print("err", file=sys.stderr)
来源：http://xv.hnjuh.cn

[U41] PHP：初始化 Composer 项目
来源：http://ul.shxzukj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://kf.huixiangedu.cn

[U42] PHP：PSR-4 自动加载
来源：http://gu.521024.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rh.9csxet.cn

[U43] PHP：声明命名空间
来源：http://kr.nszjky.cn

namespace App\Http;
来源：http://yz.newstarts.cn

[U44] PHP：开启严格类型
来源：http://yi.muxihuayi.cn

declare(strict_types=1);
来源：http://zd.lnxyls.cn

[U45] PHP：类型声明与返回类型
来源：http://bu.huixiangedu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jg.bjjhwx.cn

[U46] PHP：可空类型
来源：http://qo.jianghongdianzi.cn

?string $name = null
来源：http://vv.nicolike.cn

[U47] PHP：联合类型
来源：http://ud.shtwfgs.cn

int|string $id
来源：http://nf.huanxung.cn

[U48] PHP：纯枚举
来源：http://fm.huanxung.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lm.hahajie.cn

[U49] PHP：只读属性
来源：http://ql.chemitech.net.cn

public readonly string $name
来源：http://wh.muxihuayi.cn

[U50] PHP：构造器属性提升
来源：http://ff.huixinmuqiang.cn

public function __construct(private int $id) {}
来源：http://oc.haigaiapp.cn

[U51] PHP：数组解构
来源：http://vz.shtwfgs.cn

[$a, $b] = $arr;
来源：http://ex.wgjwhj.cn

[U52] PHP：箭头函数
来源：http://ry.shtwfgs.cn

$double = fn($x) => $x * 2;
来源：http://iu.shxzskj.cn

[U53] PHP：空合并运算符
来源：http://wl.szxytkj.cn

$v = $a ?? $b ?? "default";
来源：http://et.panjiajie.cn

[U54] PHP：空安全调用
来源：http://ly.yuntaijiaju.cn

$obj?->method()
来源：http://hx.panjiajie.cn

[U55] PHP：match 表达式
来源：http://qg.9csxet.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://at.panjiajie.cn

[U56] PHP：命名参数
来源：http://my.jctech888.com.cn

f(a: 1, b: 2)
来源：http://ly.nicolike.cn

[U57] PHP：字符串插值
来源：http://xb.newstarts.cn

"值: {$a}"
来源：http://oh.hahajie.cn

[U58] PHP：数组三件套
来源：http://gv.huanxung.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ug.wgjwhj.cn

[U59] PHP：自定义排序
来源：http://wz.muxihuayi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gi.jianghongdianzi.cn

[U60] PHP：JSON 编解码
来源：http://hj.haigaiapp.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lk.jianghongdianzi.cn

[U61] PHP：正则
来源：http://cs.lnxyls.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zg.szsharing.cn

[U62] PHP：日期对象
来源：http://kn.chemitech.net.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gi.haigaiapp.cn

[U63] PHP：文件读写
来源：http://wn.jianghongdianzi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://us.huanxung.cn

[U64] PHP：目录遍历
来源：http://sn.szsharing.cn

glob("dir/*.php");  scandir("dir");
来源：http://sq.wgjwhj.cn

[U65] PHP：会话
来源：http://dj.huixinmuqiang.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://hp.muxihuayi.cn

[U66] PHP：设置 Cookie
来源：http://yq.jctech888.com.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qv.huixinmuqiang.cn

[U67] PHP：处理文件上传
来源：http://di.hahajie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rq.nicolike.cn

[U68] PHP：PDO 连接
来源：http://ye.nicolike.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://th.nicolike.cn

[U69] PHP：PDO 预处理
来源：http://rp.szxytkj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://io.gzmigu.cn

[U70] PHP：PDO 事务
来源：http://bo.shxzukj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dr.asd995.cn

[U71] PHP：抛出异常
来源：http://ez.huixinmuqiang.cn

throw new RuntimeException("失败", 500);
来源：http://jg.chemitech.net.cn

[U72] PHP：写错误日志
来源：http://kq.chemitech.net.cn

error_log("失败: " . $e->getMessage());
来源：http://xt.9csxet.cn

[U73] PHP：读取 ini 配置
来源：http://zr.szxytkj.cn

parse_ini_file("config.ini", true)
来源：http://lm.nicolike.cn

[U74] PHP：读取环境变量
来源：http://ub.colortex.cn

getenv("APP_ENV") ?: "production"
来源：http://sn.lnxyls.cn

[U75] PHP：依赖注入
来源：http://qe.521024.cn

composer require psr/container
来源：http://ig.gzmigu.cn

[U76] PHP：简单路由
来源：http://ij.szsharing.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fz.9csxet.cn

[U77] PHP：模板渲染
来源：http://av.panjiajie.cn

composer require twig/twig
来源：http://yn.huixiangedu.cn

[U78] PHP：单元测试
来源：http://vn.szxytkj.cn

composer require --dev phpunit/phpunit
来源：http://tg.shxzukj.cn

[U79] PHP：静态分析
来源：http://ms.chemitech.net.cn

composer require --dev phpstan/phpstan
来源：http://wa.huanxung.cn

[U80] PHP：代码规范修复
来源：http://yu.shxzukj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://zk.gzmigu.cn

[U81] JS：初始化项目
来源：http://ey.jianghongdianzi.cn

npm init -y;  npm i express
来源：http://sl.521024.cn

[U82] JS：package.json 脚本
来源：http://tw.hahajie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lj.hahajie.cn

[U83] JS：ES Module 导入导出
来源：http://po.panjiajie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://dz.wgjwhj.cn

[U84] JS：CommonJS 写法
来源：http://oh.chemitech.net.cn

module.exports = { a };  const { a } = require("./m");
来源：http://yw.shxzukj.cn

[U85] JS：可选链
来源：http://nx.jianghongdianzi.cn

a?.b?.c
来源：http://sy.panjiajie.cn

[U86] JS：空值合并
来源：http://bb.lnxyls.cn

a ?? b
来源：http://ou.wgjwhj.cn

[U87] JS：解构默认值
来源：http://qu.lnxyls.cn

const { a = 1, b = 2 } = obj;
来源：http://qb.panjiajie.cn

[U88] JS：对象展开合并
来源：http://fo.gzmigu.cn

{ ...a, ...b }
来源：http://ph.nszjky.cn

[U89] JS：数组去重
来源：http://od.521024.cn

[...new Set(arr)]
来源：http://so.colortex.cn

[U90] JS：数字数组排序
来源：http://sr.haigaiapp.cn

[...arr].sort((a, b) => a - b)
来源：http://qj.yuntaijiaju.cn

[U91] JS：对象键值遍历
来源：http://ko.shtwfgs.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nd.szsharing.cn

[U92] JS：深拷贝
来源：http://bv.lnxyls.cn

structuredClone(obj)
来源：http://nd.muxihuayi.cn

[U93] JS：模板字符串
来源：http://jj.panjiajie.cn

`共 ${n} 条`
来源：http://bc.bjjhwx.cn

[U94] JS：箭头函数
来源：http://pa.shxzukj.cn

const double = x => x * 2;
来源：http://sw.wgjwhj.cn

[U95] JS：Promise 包装
来源：http://ma.asd995.cn

new Promise((resolve, reject) => {})
来源：http://zt.bjjhwx.cn

[U96] JS：async/await 与异常
来源：http://nd.bjjhwx.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qp.gzmigu.cn

[U97] JS：并发请求
来源：http://fy.gzmigu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ei.lnxyls.cn

[U98] JS：fetch 带 JSON
来源：http://la.9csxet.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jg.asd995.cn

[U99] JS：事件监听
来源：http://zv.9csxet.cn

el.addEventListener("click", e => {})
来源：http://gg.shxzukj.cn

[U100] JS：DOM 查询
来源：http://if.colortex.cn

document.querySelector(".item")
来源：http://pn.szsharing.cn

[U101] JS：classList 操作
来源：http://cg.szsharing.cn

el.classList.toggle("active")
来源：http://cc.shxzukj.cn

[U102] JS：本地存储
来源：http://xa.chemitech.net.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ms.szsharing.cn

[U103] JS：定时器
来源：http://kw.huixinmuqiang.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ll.nszjky.cn

[U104] JS：防抖
来源：http://sy.colortex.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jc.521024.cn

[U105] JS：节流
来源：http://iu.haigaiapp.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vn.szxytkj.cn

[U106] JS：日期格式化
来源：http://tg.newstarts.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vy.newstarts.cn

[U107] JS：数字千分位
来源：http://fb.jctech888.com.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cq.521024.cn

[U108] JS：随机整数
来源：http://th.newstarts.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tc.shxzskj.cn

[U109] JS：数组分组
来源：http://zb.panjiajie.cn

Object.groupBy(arr, x => x.type)
来源：http://kv.panjiajie.cn

[U110] JS：数组分块
来源：http://bz.panjiajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://eq.colortex.cn

[U111] JS：对象转 Map
来源：http://yb.bjjhwx.cn

new Map(Object.entries(obj))
来源：http://vu.hahajie.cn

[U112] JS：字符串补位
来源：http://em.szxytkj.cn

"7".padStart(3, "0")
来源：http://sr.jianghongdianzi.cn

[U113] JS：正则替换全部
来源：http://bc.haigaiapp.cn

s.replaceAll("a", "b")
来源：http://fw.szxytkj.cn

[U114] JS：JSON 深比较
来源：http://df.yuexingan06.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://pa.huixiangedu.cn

[U115] JS：生成 UUID
来源：http://rf.huanxung.cn

crypto.randomUUID()
来源：http://vd.szxytkj.cn

[U116] JS：类型检查（JSDoc）
来源：http://kk.chemitech.net.cn

/** @param {string} name */ function f(name) {}
来源：http://ng.shtwfgs.cn

[U117] JS：单元测试
来源：http://wg.bookmarksfly.cn

npm i -D vitest;  npx vitest
来源：http://dh.yuexingan06.cn

[U118] JS：开发服务器
来源：http://ta.gzmigu.cn

npm i -D vite;  npx vite
来源：http://hs.bookmarksfly.cn

[U119] JS：生产构建
来源：http://mz.asd995.cn

npx vite build
来源：http://te.newstarts.cn

[U120] JS：读取环境变量（Vite）
来源：http://xb.szsharing.cn

import.meta.env.VITE_API_URL
来源：http://vk.huanxung.cn

================================================================================
来源：http://mn.asd995.cn

统计汇总
来源：http://kj.shxzukj.cn

================================================================================
来源：http://ma.muxihuayi.cn

按语言统计（条）：
来源：http://mi.yuntaijiaju.cn

Python ......... 252
来源：http://hu.huixiangedu.cn

PHP ............ 252
来源：http://if.521024.cn

JavaScript ..... 252
来源：http://vk.chemitech.net.cn

TypeScript ..... 212
来源：http://jq.huixiangedu.cn

Java ........... 212
来源：http://yu.hahajie.cn

Go ............. 212
来源：http://kg.521024.cn

Ruby ........... 212
来源：http://iz.szsharing.cn

C# ............. 212
来源：http://hc.chemitech.net.cn

C .............. 30
来源：http://eb.gzmigu.cn

C++ ............ 30
来源：http://yf.panjiajie.cn

SQL ............ 90
来源：http://ho.shxzskj.cn

Bash ........... 80
来源：http://xu.chemitech.net.cn

Kotlin ......... 15
来源：http://aj.gzmigu.cn

Swift .......... 15
来源：http://ee.shxzskj.cn

Lua ............ 10
来源：http://fx.yuntaijiaju.cn

Perl ........... 10
来源：http://ma.nszjky.cn

Scala .......... 10
来源：http://uv.szxytkj.cn

------------------------------------
来源：http://qy.huixinmuqiang.cn

合计 ........... 2106 条
来源：http://kh.yuntaijiaju.cn

按章节统计：
来源：http://ej.lnxyls.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nm.panjiajie.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wo.muxihuayi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bu.hnjuh.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cb.9csxet.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wc.9csxet.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://te.lnxyls.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zl.521024.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://go.panjiajie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://km.jctech888.com.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://te.jctech888.com.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jy.nszjky.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wq.szsharing.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://cv.szxytkj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://nr.9csxet.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://so.shtwfgs.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mk.chemitech.net.cn

Q SQL 专题                              90
来源：http://fw.521024.cn

R Bash 专题                             80
来源：http://eo.bookmarksfly.cn

S C / C++ 专题                          60
来源：http://tl.jianghongdianzi.cn

T 其他语言补充                          60
来源：http://sx.9csxet.cn

U 高频实用片段                         120
来源：http://zx.nszjky.cn

------------------------------------
来源：http://jy.huixiangedu.cn

合计                                  2106 条
来源：http://zh.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://qr.jianghongdianzi.cn

使用提醒
来源：http://da.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://xn.yuntaijiaju.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ub.nszjky.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://lc.colortex.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gx.asd995.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://zr.lnxyls.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qm.9csxet.cn

—— 文件结束 ——
来源：http://sb.hahajie.cn

================================================================================
来源：http://wm.bookmarksfly.cn

程序语言常见例子速查手册（2024 版）
来源：http://gm.panjiajie.cn

Common Programming Examples Cheat Book
来源：http://dt.yuntaijiaju.cn

================================================================================
来源：http://mr.gzmigu.cn

【收录内容】
来源：http://gw.jianghongdianzi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://xf.wgjwhj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://sw.yuexingan06.cn

SQL · Bash · C · C++
来源：http://yd.bookmarksfly.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://cd.huixiangedu.cn

【使用说明】
来源：http://ua.asd995.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://eg.wgjwhj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dv.jianghongdianzi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ey.huixiangedu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qd.hnjuh.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ij.jianghongdianzi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://fy.szxytkj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lt.gzmigu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://kd.newstarts.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lx.huixinmuqiang.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zn.huixiangedu.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lu.yuntaijiaju.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fh.jianghongdianzi.cn

【文件统计】
来源：http://hz.jctech888.com.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hr.huanxung.cn


<!-- 参考信息 -->