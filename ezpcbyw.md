代发 wailian999

[U07] Py：反转字典键值
来源：http://jc.huixiangedu.cn

{v: k for k, v in d.items()}
来源：http://rj.muxihuayi.cn

[U08] Py：展平二维列表
来源：http://xq.shxzukj.cn

[y for x in nested for y in x]
来源：http://sl.huixinmuqiang.cn

[U09] Py：字典取最大值的键
来源：http://cu.chemitech.net.cn

max(d, key=d.get)
来源：http://xt.wgjwhj.cn

[U10] Py：按值排序字典
来源：http://bl.panjiajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://oz.wgjwhj.cn

[U11] Py：生成器表达式
来源：http://wy.jianghongdianzi.cn

(x * 2 for x in arr)
来源：http://ko.9csxet.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lx.nszjky.cn

Counter(arr).most_common(3)
来源：http://wk.panjiajie.cn

[U13] Py：固定长度队列
来源：http://ll.shtwfgs.cn

deque(maxlen=10)
来源：http://ld.huixiangedu.cn

[U14] Py：分组收集到列表
来源：http://eq.lnxyls.cn

defaultdict(list)
来源：http://bf.hahajie.cn

[U15] Py：高精度计时
来源：http://kn.nszjky.cn

t = time.perf_counter()
来源：http://lq.nszjky.cn

[U16] Py：命令行参数解析
来源：http://iv.jctech888.com.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dd.wgjwhj.cn

[U17] Py：初始化日志
来源：http://mn.nicolike.cn

logging.basicConfig(level=logging.INFO)
来源：http://jh.haigaiapp.cn

[U18] Py：预编译正则
来源：http://fd.haigaiapp.cn

pat = re.compile(r"\d+")
来源：http://ay.yuexingan06.cn

[U19] Py：正则替换带回调
来源：http://at.shxzskj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hs.shxzskj.cn

[U20] Py：缓存函数结果
来源：http://li.hahajie.cn

@functools.lru_cache(maxsize=None)
来源：http://xv.shxzskj.cn

[U21] Py：自定义上下文管理器
来源：http://jc.newstarts.cn

@contextlib.contextmanager
来源：http://xu.bookmarksfly.cn

[U22] Py：矩阵转置
来源：http://kx.shtwfgs.cn

list(zip(*m))
来源：http://cx.lnxyls.cn

[U23] Py：分块读取大文件
来源：http://ce.bookmarksfly.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fn.521024.cn

[U24] Py：路径操作
来源：http://ya.yuntaijiaju.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mo.huixiangedu.cn

[U25] Py：CSV 按字典读
来源：http://cl.chemitech.net.cn

csv.DictReader(f)
来源：http://zk.hahajie.cn

[U26] Py：并发下载
来源：http://cf.panjiajie.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wf.jctech888.com.cn

[U27] Py：异步 HTTP
来源：http://nm.nszjky.cn

aiohttp.ClientSession() 配合 async with
来源：http://st.521024.cn

[U28] Py：类型别名
来源：http://up.jctech888.com.cn

UserId = int
来源：http://to.shxzskj.cn

[U29] Py：属性校验
来源：http://wu.jctech888.com.cn

@property 与 @x.setter 配合
来源：http://fh.haigaiapp.cn

[U30] Py：数据类
来源：http://we.yuexingan06.cn

@dataclass(slots=True)
来源：http://re.shtwfgs.cn

[U31] Py：单测
来源：http://vn.huixinmuqiang.cn

python -m pytest -q
来源：http://dy.szsharing.cn

[U32] Py：代码格式化
来源：http://zj.jianghongdianzi.cn

ruff format . && ruff check --fix .
来源：http://zh.shxzskj.cn

[U33] Py：打包发布
来源：http://dw.colortex.cn

python -m build  （依赖 pyproject.toml）
来源：http://mk.asd995.cn

[U34] Py：判断编码
来源：http://je.lnxyls.cn

chardet.detect(raw)
来源：http://ch.9csxet.cn

[U35] Py：发送邮件
来源：http://nk.panjiajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tb.huanxung.cn

[U36] Py：定时任务
来源：http://pt.521024.cn

schedule.every(10).minutes.do(job)
来源：http://rs.yuntaijiaju.cn

[U37] Py：读写 Excel
来源：http://mu.bookmarksfly.cn

pandas.read_excel / DataFrame.to_excel
来源：http://dz.bjjhwx.cn

[U38] Py：获取脚本所在目录
来源：http://vs.szxytkj.cn

Path(__file__).resolve().parent
来源：http://th.nicolike.cn

[U39] Py：判断是否在交互环境
来源：http://ch.panjiajie.cn

sys.stdout.isatty()
来源：http://me.chemitech.net.cn

[U40] Py：打印到标准错误
来源：http://ga.hnjuh.cn

print("err", file=sys.stderr)
来源：http://ns.hnjuh.cn

[U41] PHP：初始化 Composer 项目
来源：http://ft.newstarts.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://aj.shxzukj.cn

[U42] PHP：PSR-4 自动加载
来源：http://iu.shxzukj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ip.bookmarksfly.cn

[U43] PHP：声明命名空间
来源：http://mk.szxytkj.cn

namespace App\Http;
来源：http://gs.panjiajie.cn

[U44] PHP：开启严格类型
来源：http://mc.nicolike.cn

declare(strict_types=1);
来源：http://sw.newstarts.cn

[U45] PHP：类型声明与返回类型
来源：http://ty.huanxung.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://gw.bookmarksfly.cn

[U46] PHP：可空类型
来源：http://vl.bookmarksfly.cn

?string $name = null
来源：http://lt.huanxung.cn

[U47] PHP：联合类型
来源：http://pq.hahajie.cn

int|string $id
来源：http://df.bjjhwx.cn

[U48] PHP：纯枚举
来源：http://sd.nicolike.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lz.nszjky.cn

[U49] PHP：只读属性
来源：http://mr.huixinmuqiang.cn

public readonly string $name
来源：http://ue.jianghongdianzi.cn

[U50] PHP：构造器属性提升
来源：http://xa.gzmigu.cn

public function __construct(private int $id) {}
来源：http://ul.wgjwhj.cn

[U51] PHP：数组解构
来源：http://dc.nszjky.cn

[$a, $b] = $arr;
来源：http://mh.yuexingan06.cn

[U52] PHP：箭头函数
来源：http://dq.huanxung.cn

$double = fn($x) => $x * 2;
来源：http://kn.shxzukj.cn

[U53] PHP：空合并运算符
来源：http://oz.yuntaijiaju.cn

$v = $a ?? $b ?? "default";
来源：http://ec.bjjhwx.cn

[U54] PHP：空安全调用
来源：http://ub.shxzukj.cn

$obj?->method()
来源：http://ss.szsharing.cn

[U55] PHP：match 表达式
来源：http://dr.szsharing.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xe.shxzskj.cn

[U56] PHP：命名参数
来源：http://ld.szsharing.cn

f(a: 1, b: 2)
来源：http://pl.panjiajie.cn

[U57] PHP：字符串插值
来源：http://np.shxzskj.cn

"值: {$a}"
来源：http://sp.9csxet.cn

[U58] PHP：数组三件套
来源：http://sp.huixinmuqiang.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zf.colortex.cn

[U59] PHP：自定义排序
来源：http://aj.jctech888.com.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rx.huixiangedu.cn

[U60] PHP：JSON 编解码
来源：http://co.nicolike.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gv.yuntaijiaju.cn

[U61] PHP：正则
来源：http://ap.lnxyls.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kh.shxzskj.cn

[U62] PHP：日期对象
来源：http://qf.9csxet.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hy.hahajie.cn

[U63] PHP：文件读写
来源：http://jg.yuntaijiaju.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://la.hnjuh.cn

[U64] PHP：目录遍历
来源：http://uf.huixiangedu.cn

glob("dir/*.php");  scandir("dir");
来源：http://lh.9csxet.cn

[U65] PHP：会话
来源：http://dc.newstarts.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://lx.huanxung.cn

[U66] PHP：设置 Cookie
来源：http://nm.haigaiapp.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jt.haigaiapp.cn

[U67] PHP：处理文件上传
来源：http://ow.hahajie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://th.yuexingan06.cn

[U68] PHP：PDO 连接
来源：http://ly.lnxyls.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ca.newstarts.cn

[U69] PHP：PDO 预处理
来源：http://dg.nicolike.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vj.szxytkj.cn

[U70] PHP：PDO 事务
来源：http://vi.bjjhwx.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ah.asd995.cn

[U71] PHP：抛出异常
来源：http://hr.huixinmuqiang.cn

throw new RuntimeException("失败", 500);
来源：http://eg.521024.cn

[U72] PHP：写错误日志
来源：http://dc.bookmarksfly.cn

error_log("失败: " . $e->getMessage());
来源：http://iq.huixiangedu.cn

[U73] PHP：读取 ini 配置
来源：http://ak.colortex.cn

parse_ini_file("config.ini", true)
来源：http://sq.haigaiapp.cn

[U74] PHP：读取环境变量
来源：http://xi.jianghongdianzi.cn

getenv("APP_ENV") ?: "production"
来源：http://kr.yuexingan06.cn

[U75] PHP：依赖注入
来源：http://jf.panjiajie.cn

composer require psr/container
来源：http://oy.nicolike.cn

[U76] PHP：简单路由
来源：http://hf.nicolike.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pd.colortex.cn

[U77] PHP：模板渲染
来源：http://pv.jctech888.com.cn

composer require twig/twig
来源：http://jm.huixinmuqiang.cn

[U78] PHP：单元测试
来源：http://aa.panjiajie.cn

composer require --dev phpunit/phpunit
来源：http://lt.bjjhwx.cn

[U79] PHP：静态分析
来源：http://ld.jctech888.com.cn

composer require --dev phpstan/phpstan
来源：http://xq.huixinmuqiang.cn

[U80] PHP：代码规范修复
来源：http://eh.bjjhwx.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://bf.jianghongdianzi.cn

[U81] JS：初始化项目
来源：http://wv.colortex.cn

npm init -y;  npm i express
来源：http://dd.szxytkj.cn

[U82] JS：package.json 脚本
来源：http://pk.jianghongdianzi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jh.shxzskj.cn

[U83] JS：ES Module 导入导出
来源：http://iq.yuntaijiaju.cn

export const a = 1;  import { a } from "./m.js";
来源：http://br.yuntaijiaju.cn

[U84] JS：CommonJS 写法
来源：http://kc.yuexingan06.cn

module.exports = { a };  const { a } = require("./m");
来源：http://bk.huixinmuqiang.cn

[U85] JS：可选链
来源：http://rk.wgjwhj.cn

a?.b?.c
来源：http://re.szxytkj.cn

[U86] JS：空值合并
来源：http://ef.chemitech.net.cn

a ?? b
来源：http://kv.muxihuayi.cn

[U87] JS：解构默认值
来源：http://fw.wgjwhj.cn

const { a = 1, b = 2 } = obj;
来源：http://rd.521024.cn

[U88] JS：对象展开合并
来源：http://mu.bookmarksfly.cn

{ ...a, ...b }
来源：http://me.yuexingan06.cn

[U89] JS：数组去重
来源：http://pw.wgjwhj.cn

[...new Set(arr)]
来源：http://hf.hahajie.cn

[U90] JS：数字数组排序
来源：http://ji.chemitech.net.cn

[...arr].sort((a, b) => a - b)
来源：http://vt.huanxung.cn

[U91] JS：对象键值遍历
来源：http://hf.colortex.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xc.gzmigu.cn

[U92] JS：深拷贝
来源：http://mq.yuexingan06.cn

structuredClone(obj)
来源：http://ww.521024.cn

[U93] JS：模板字符串
来源：http://cy.szxytkj.cn

`共 ${n} 条`
来源：http://ia.jianghongdianzi.cn

[U94] JS：箭头函数
来源：http://ud.yuntaijiaju.cn

const double = x => x * 2;
来源：http://yy.huixiangedu.cn

[U95] JS：Promise 包装
来源：http://io.wgjwhj.cn

new Promise((resolve, reject) => {})
来源：http://sh.colortex.cn

[U96] JS：async/await 与异常
来源：http://fk.huixinmuqiang.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://eo.huanxung.cn

[U97] JS：并发请求
来源：http://cr.jctech888.com.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://am.521024.cn

[U98] JS：fetch 带 JSON
来源：http://xu.yuntaijiaju.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ad.colortex.cn

[U99] JS：事件监听
来源：http://af.shxzukj.cn

el.addEventListener("click", e => {})
来源：http://ud.bookmarksfly.cn

[U100] JS：DOM 查询
来源：http://dv.colortex.cn

document.querySelector(".item")
来源：http://ip.asd995.cn

[U101] JS：classList 操作
来源：http://yh.521024.cn

el.classList.toggle("active")
来源：http://wd.chemitech.net.cn

[U102] JS：本地存储
来源：http://ac.shtwfgs.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xh.nicolike.cn

[U103] JS：定时器
来源：http://hz.chemitech.net.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ay.wgjwhj.cn

[U104] JS：防抖
来源：http://da.hahajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ta.gzmigu.cn

[U105] JS：节流
来源：http://db.muxihuayi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tl.huixiangedu.cn

[U106] JS：日期格式化
来源：http://tf.gzmigu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dd.yuexingan06.cn

[U107] JS：数字千分位
来源：http://iz.huixinmuqiang.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bx.huixinmuqiang.cn

[U108] JS：随机整数
来源：http://nx.shxzukj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zm.chemitech.net.cn

[U109] JS：数组分组
来源：http://qu.muxihuayi.cn

Object.groupBy(arr, x => x.type)
来源：http://iw.nszjky.cn

[U110] JS：数组分块
来源：http://fb.hahajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://te.jctech888.com.cn

[U111] JS：对象转 Map
来源：http://qz.huanxung.cn

new Map(Object.entries(obj))
来源：http://vw.nicolike.cn

[U112] JS：字符串补位
来源：http://qa.newstarts.cn

"7".padStart(3, "0")
来源：http://jw.shxzskj.cn

[U113] JS：正则替换全部
来源：http://xs.yuntaijiaju.cn

s.replaceAll("a", "b")
来源：http://ql.newstarts.cn

[U114] JS：JSON 深比较
来源：http://vd.hnjuh.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://dg.yuexingan06.cn

[U115] JS：生成 UUID
来源：http://gh.521024.cn

crypto.randomUUID()
来源：http://wb.asd995.cn

[U116] JS：类型检查（JSDoc）
来源：http://ag.bookmarksfly.cn

/** @param {string} name */ function f(name) {}
来源：http://dh.nszjky.cn

[U117] JS：单元测试
来源：http://bc.hnjuh.cn

npm i -D vitest;  npx vitest
来源：http://ha.9csxet.cn

[U118] JS：开发服务器
来源：http://dg.asd995.cn

npm i -D vite;  npx vite
来源：http://kh.colortex.cn

[U119] JS：生产构建
来源：http://ou.muxihuayi.cn

npx vite build
来源：http://kv.newstarts.cn

[U120] JS：读取环境变量（Vite）
来源：http://xf.jianghongdianzi.cn

import.meta.env.VITE_API_URL
来源：http://gq.szsharing.cn

================================================================================
来源：http://gf.shxzskj.cn

统计汇总
来源：http://ah.bookmarksfly.cn

================================================================================
来源：http://nd.szsharing.cn

按语言统计（条）：
来源：http://mr.9csxet.cn

Python ......... 252
来源：http://ug.huixinmuqiang.cn

PHP ............ 252
来源：http://fn.huanxung.cn

JavaScript ..... 252
来源：http://ap.panjiajie.cn

TypeScript ..... 212
来源：http://rj.hahajie.cn

Java ........... 212
来源：http://wz.shtwfgs.cn

Go ............. 212
来源：http://ki.szxytkj.cn

Ruby ........... 212
来源：http://jh.nicolike.cn

C# ............. 212
来源：http://lu.jianghongdianzi.cn

C .............. 30
来源：http://tw.gzmigu.cn

C++ ............ 30
来源：http://zx.newstarts.cn

SQL ............ 90
来源：http://fe.szxytkj.cn

Bash ........... 80
来源：http://ra.szsharing.cn

Kotlin ......... 15
来源：http://tp.asd995.cn

Swift .......... 15
来源：http://bf.chemitech.net.cn

Lua ............ 10
来源：http://xj.newstarts.cn

Perl ........... 10
来源：http://us.lnxyls.cn

Scala .......... 10
来源：http://no.yuexingan06.cn

------------------------------------
来源：http://ll.yuexingan06.cn

合计 ........... 2106 条
来源：http://cr.newstarts.cn

按章节统计：
来源：http://ht.wgjwhj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dp.shtwfgs.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kb.newstarts.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vj.chemitech.net.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ai.huixiangedu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://yb.jianghongdianzi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xh.hahajie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://my.newstarts.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vy.lnxyls.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wz.shxzukj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tk.shxzskj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ij.yuexingan06.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vm.huanxung.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://op.newstarts.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zv.lnxyls.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hu.jctech888.com.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gw.shxzskj.cn

Q SQL 专题                              90
来源：http://of.panjiajie.cn

R Bash 专题                             80
来源：http://th.521024.cn

S C / C++ 专题                          60
来源：http://nz.9csxet.cn

T 其他语言补充                          60
来源：http://ps.hahajie.cn

U 高频实用片段                         120
来源：http://cr.9csxet.cn

------------------------------------
来源：http://rg.nicolike.cn

合计                                  2106 条
来源：http://cw.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://kf.bookmarksfly.cn

使用提醒
来源：http://bx.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://ld.szsharing.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zv.huixiangedu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mu.gzmigu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gw.521024.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://zy.jianghongdianzi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ki.nicolike.cn

—— 文件结束 ——
来源：http://fq.szxytkj.cn

================================================================================
来源：http://zb.jctech888.com.cn

程序语言常见例子速查手册（2024 版）
来源：http://tt.yuntaijiaju.cn

Common Programming Examples Cheat Book
来源：http://tk.shxzukj.cn

================================================================================
来源：http://gw.shxzukj.cn

【收录内容】
来源：http://mh.huanxung.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://sl.newstarts.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://kr.huanxung.cn

SQL · Bash · C · C++
来源：http://jr.nicolike.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://oq.jianghongdianzi.cn

【使用说明】
来源：http://fe.nszjky.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ca.huixiangedu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://oh.haigaiapp.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wx.shxzukj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yj.jianghongdianzi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://cs.newstarts.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qx.colortex.cn


<!-- 参考信息 -->