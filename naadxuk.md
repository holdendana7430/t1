代发 wailian999

[U09] Py：字典取最大值的键
来源：http://iz.yuexingan06.cn

max(d, key=d.get)
来源：http://lj.chemitech.net.cn

[U10] Py：按值排序字典
来源：http://xg.nicolike.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ud.newstarts.cn

[U11] Py：生成器表达式
来源：http://ik.hahajie.cn

(x * 2 for x in arr)
来源：http://lr.yuexingan06.cn

[U12] Py：取出现最多的 3 个元素
来源：http://fu.colortex.cn

Counter(arr).most_common(3)
来源：http://tk.muxihuayi.cn

[U13] Py：固定长度队列
来源：http://gk.521024.cn

deque(maxlen=10)
来源：http://lo.shtwfgs.cn

[U14] Py：分组收集到列表
来源：http://ww.panjiajie.cn

defaultdict(list)
来源：http://hk.yuexingan06.cn

[U15] Py：高精度计时
来源：http://hw.wgjwhj.cn

t = time.perf_counter()
来源：http://az.chemitech.net.cn

[U16] Py：命令行参数解析
来源：http://zl.newstarts.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sc.hnjuh.cn

[U17] Py：初始化日志
来源：http://po.bookmarksfly.cn

logging.basicConfig(level=logging.INFO)
来源：http://qo.yuntaijiaju.cn

[U18] Py：预编译正则
来源：http://ll.colortex.cn

pat = re.compile(r"\d+")
来源：http://zs.wgjwhj.cn

[U19] Py：正则替换带回调
来源：http://lu.muxihuayi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vj.huanxung.cn

[U20] Py：缓存函数结果
来源：http://wx.521024.cn

@functools.lru_cache(maxsize=None)
来源：http://mf.wgjwhj.cn

[U21] Py：自定义上下文管理器
来源：http://ds.bookmarksfly.cn

@contextlib.contextmanager
来源：http://ht.muxihuayi.cn

[U22] Py：矩阵转置
来源：http://xk.hnjuh.cn

list(zip(*m))
来源：http://od.yuexingan06.cn

[U23] Py：分块读取大文件
来源：http://vn.huixiangedu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gi.asd995.cn

[U24] Py：路径操作
来源：http://al.asd995.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.521024.cn

[U25] Py：CSV 按字典读
来源：http://xj.szxytkj.cn

csv.DictReader(f)
来源：http://gi.lnxyls.cn

[U26] Py：并发下载
来源：http://hp.yuexingan06.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qz.nszjky.cn

[U27] Py：异步 HTTP
来源：http://pq.shxzukj.cn

aiohttp.ClientSession() 配合 async with
来源：http://zg.bjjhwx.cn

[U28] Py：类型别名
来源：http://ax.huixinmuqiang.cn

UserId = int
来源：http://uh.jctech888.com.cn

[U29] Py：属性校验
来源：http://fy.asd995.cn

@property 与 @x.setter 配合
来源：http://ha.muxihuayi.cn

[U30] Py：数据类
来源：http://je.hnjuh.cn

@dataclass(slots=True)
来源：http://lq.gzmigu.cn

[U31] Py：单测
来源：http://em.hnjuh.cn

python -m pytest -q
来源：http://qf.hnjuh.cn

[U32] Py：代码格式化
来源：http://pr.szsharing.cn

ruff format . && ruff check --fix .
来源：http://nt.huixiangedu.cn

[U33] Py：打包发布
来源：http://wh.szxytkj.cn

python -m build  （依赖 pyproject.toml）
来源：http://rs.shxzukj.cn

[U34] Py：判断编码
来源：http://zm.nicolike.cn

chardet.detect(raw)
来源：http://hs.szsharing.cn

[U35] Py：发送邮件
来源：http://rd.newstarts.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vx.szsharing.cn

[U36] Py：定时任务
来源：http://ne.panjiajie.cn

schedule.every(10).minutes.do(job)
来源：http://nh.jctech888.com.cn

[U37] Py：读写 Excel
来源：http://px.huanxung.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qv.huixiangedu.cn

[U38] Py：获取脚本所在目录
来源：http://xv.colortex.cn

Path(__file__).resolve().parent
来源：http://ro.jianghongdianzi.cn

[U39] Py：判断是否在交互环境
来源：http://fd.gzmigu.cn

sys.stdout.isatty()
来源：http://ie.szxytkj.cn

[U40] Py：打印到标准错误
来源：http://ju.yuntaijiaju.cn

print("err", file=sys.stderr)
来源：http://ay.jctech888.com.cn

[U41] PHP：初始化 Composer 项目
来源：http://sz.lnxyls.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://yk.hahajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://nt.yuexingan06.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kg.bookmarksfly.cn

[U43] PHP：声明命名空间
来源：http://uj.hnjuh.cn

namespace App\Http;
来源：http://rg.yuexingan06.cn

[U44] PHP：开启严格类型
来源：http://kj.wgjwhj.cn

declare(strict_types=1);
来源：http://tt.chemitech.net.cn

[U45] PHP：类型声明与返回类型
来源：http://xh.hahajie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://zk.shxzskj.cn

[U46] PHP：可空类型
来源：http://jk.shxzskj.cn

?string $name = null
来源：http://rm.lnxyls.cn

[U47] PHP：联合类型
来源：http://dp.gzmigu.cn

int|string $id
来源：http://wu.panjiajie.cn

[U48] PHP：纯枚举
来源：http://qu.hahajie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fz.lnxyls.cn

[U49] PHP：只读属性
来源：http://oj.panjiajie.cn

public readonly string $name
来源：http://zd.nicolike.cn

[U50] PHP：构造器属性提升
来源：http://kw.jianghongdianzi.cn

public function __construct(private int $id) {}
来源：http://sy.panjiajie.cn

[U51] PHP：数组解构
来源：http://sq.yuexingan06.cn

[$a, $b] = $arr;
来源：http://yv.9csxet.cn

[U52] PHP：箭头函数
来源：http://kv.colortex.cn

$double = fn($x) => $x * 2;
来源：http://od.huanxung.cn

[U53] PHP：空合并运算符
来源：http://ho.panjiajie.cn

$v = $a ?? $b ?? "default";
来源：http://td.hnjuh.cn

[U54] PHP：空安全调用
来源：http://fw.yuexingan06.cn

$obj?->method()
来源：http://nj.jctech888.com.cn

[U55] PHP：match 表达式
来源：http://sc.huixiangedu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fy.hahajie.cn

[U56] PHP：命名参数
来源：http://dj.bookmarksfly.cn

f(a: 1, b: 2)
来源：http://hj.colortex.cn

[U57] PHP：字符串插值
来源：http://py.gzmigu.cn

"值: {$a}"
来源：http://uy.huixinmuqiang.cn

[U58] PHP：数组三件套
来源：http://xp.9csxet.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://et.asd995.cn

[U59] PHP：自定义排序
来源：http://nh.jianghongdianzi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oc.shxzukj.cn

[U60] PHP：JSON 编解码
来源：http://ea.huanxung.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jx.yuntaijiaju.cn

[U61] PHP：正则
来源：http://sr.hahajie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sb.panjiajie.cn

[U62] PHP：日期对象
来源：http://ug.shxzskj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kc.nszjky.cn

[U63] PHP：文件读写
来源：http://sw.nszjky.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://iu.colortex.cn

[U64] PHP：目录遍历
来源：http://vz.chemitech.net.cn

glob("dir/*.php");  scandir("dir");
来源：http://iq.huanxung.cn

[U65] PHP：会话
来源：http://pm.521024.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://az.bjjhwx.cn

[U66] PHP：设置 Cookie
来源：http://jr.panjiajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vk.nicolike.cn

[U67] PHP：处理文件上传
来源：http://br.yuexingan06.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jf.shxzukj.cn

[U68] PHP：PDO 连接
来源：http://wj.jianghongdianzi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kw.jianghongdianzi.cn

[U69] PHP：PDO 预处理
来源：http://ng.9csxet.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gu.yuexingan06.cn

[U70] PHP：PDO 事务
来源：http://og.jctech888.com.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://co.muxihuayi.cn

[U71] PHP：抛出异常
来源：http://bh.9csxet.cn

throw new RuntimeException("失败", 500);
来源：http://pk.jctech888.com.cn

[U72] PHP：写错误日志
来源：http://dd.muxihuayi.cn

error_log("失败: " . $e->getMessage());
来源：http://gh.huixiangedu.cn

[U73] PHP：读取 ini 配置
来源：http://wf.shxzskj.cn

parse_ini_file("config.ini", true)
来源：http://yy.chemitech.net.cn

[U74] PHP：读取环境变量
来源：http://lw.lnxyls.cn

getenv("APP_ENV") ?: "production"
来源：http://cs.yuntaijiaju.cn

[U75] PHP：依赖注入
来源：http://nx.asd995.cn

composer require psr/container
来源：http://rt.szsharing.cn

[U76] PHP：简单路由
来源：http://ji.nicolike.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wy.huanxung.cn

[U77] PHP：模板渲染
来源：http://zv.bookmarksfly.cn

composer require twig/twig
来源：http://vv.huixiangedu.cn

[U78] PHP：单元测试
来源：http://hg.haigaiapp.cn

composer require --dev phpunit/phpunit
来源：http://vp.shxzskj.cn

[U79] PHP：静态分析
来源：http://dn.wgjwhj.cn

composer require --dev phpstan/phpstan
来源：http://qg.haigaiapp.cn

[U80] PHP：代码规范修复
来源：http://yk.nicolike.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://sd.huixiangedu.cn

[U81] JS：初始化项目
来源：http://zw.lnxyls.cn

npm init -y;  npm i express
来源：http://ig.muxihuayi.cn

[U82] JS：package.json 脚本
来源：http://dk.shtwfgs.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://df.nicolike.cn

[U83] JS：ES Module 导入导出
来源：http://ot.nszjky.cn

export const a = 1;  import { a } from "./m.js";
来源：http://my.shxzukj.cn

[U84] JS：CommonJS 写法
来源：http://pm.9csxet.cn

module.exports = { a };  const { a } = require("./m");
来源：http://je.nicolike.cn

[U85] JS：可选链
来源：http://yf.gzmigu.cn

a?.b?.c
来源：http://rh.nszjky.cn

[U86] JS：空值合并
来源：http://cz.hnjuh.cn

a ?? b
来源：http://nx.colortex.cn

[U87] JS：解构默认值
来源：http://or.jctech888.com.cn

const { a = 1, b = 2 } = obj;
来源：http://ia.bookmarksfly.cn

[U88] JS：对象展开合并
来源：http://za.hnjuh.cn

{ ...a, ...b }
来源：http://lq.hahajie.cn

[U89] JS：数组去重
来源：http://rk.yuexingan06.cn

[...new Set(arr)]
来源：http://ye.huixiangedu.cn

[U90] JS：数字数组排序
来源：http://ow.shxzukj.cn

[...arr].sort((a, b) => a - b)
来源：http://em.newstarts.cn

[U91] JS：对象键值遍历
来源：http://jz.huixiangedu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rq.shxzskj.cn

[U92] JS：深拷贝
来源：http://qz.gzmigu.cn

structuredClone(obj)
来源：http://np.hnjuh.cn

[U93] JS：模板字符串
来源：http://fg.jctech888.com.cn

`共 ${n} 条`
来源：http://fl.hnjuh.cn

[U94] JS：箭头函数
来源：http://ph.shxzukj.cn

const double = x => x * 2;
来源：http://km.chemitech.net.cn

[U95] JS：Promise 包装
来源：http://kg.lnxyls.cn

new Promise((resolve, reject) => {})
来源：http://dg.shxzukj.cn

[U96] JS：async/await 与异常
来源：http://zu.newstarts.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lo.wgjwhj.cn

[U97] JS：并发请求
来源：http://av.lnxyls.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://hq.shxzskj.cn

[U98] JS：fetch 带 JSON
来源：http://ek.newstarts.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://it.yuexingan06.cn

[U99] JS：事件监听
来源：http://xk.lnxyls.cn

el.addEventListener("click", e => {})
来源：http://du.huixiangedu.cn

[U100] JS：DOM 查询
来源：http://vr.521024.cn

document.querySelector(".item")
来源：http://iu.hahajie.cn

[U101] JS：classList 操作
来源：http://md.muxihuayi.cn

el.classList.toggle("active")
来源：http://gr.huanxung.cn

[U102] JS：本地存储
来源：http://co.yuntaijiaju.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://py.nszjky.cn

[U103] JS：定时器
来源：http://by.shxzukj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ey.shtwfgs.cn

[U104] JS：防抖
来源：http://oy.bookmarksfly.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hy.panjiajie.cn

[U105] JS：节流
来源：http://qh.shxzskj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gu.521024.cn

[U106] JS：日期格式化
来源：http://jm.521024.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zt.gzmigu.cn

[U107] JS：数字千分位
来源：http://mg.asd995.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dt.jianghongdianzi.cn

[U108] JS：随机整数
来源：http://pd.shxzskj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wk.jctech888.com.cn

[U109] JS：数组分组
来源：http://yu.szsharing.cn

Object.groupBy(arr, x => x.type)
来源：http://wr.nszjky.cn

[U110] JS：数组分块
来源：http://cm.gzmigu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ej.lnxyls.cn

[U111] JS：对象转 Map
来源：http://at.9csxet.cn

new Map(Object.entries(obj))
来源：http://bp.yuexingan06.cn

[U112] JS：字符串补位
来源：http://vj.szsharing.cn

"7".padStart(3, "0")
来源：http://ws.muxihuayi.cn

[U113] JS：正则替换全部
来源：http://et.yuexingan06.cn

s.replaceAll("a", "b")
来源：http://mk.newstarts.cn

[U114] JS：JSON 深比较
来源：http://id.szsharing.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://wq.bookmarksfly.cn

[U115] JS：生成 UUID
来源：http://jk.muxihuayi.cn

crypto.randomUUID()
来源：http://vc.shxzukj.cn

[U116] JS：类型检查（JSDoc）
来源：http://sk.asd995.cn

/** @param {string} name */ function f(name) {}
来源：http://xu.gzmigu.cn

[U117] JS：单元测试
来源：http://op.521024.cn

npm i -D vitest;  npx vitest
来源：http://tv.jctech888.com.cn

[U118] JS：开发服务器
来源：http://go.muxihuayi.cn

npm i -D vite;  npx vite
来源：http://av.hahajie.cn

[U119] JS：生产构建
来源：http://gx.szsharing.cn

npx vite build
来源：http://ft.shxzukj.cn

[U120] JS：读取环境变量（Vite）
来源：http://tr.wgjwhj.cn

import.meta.env.VITE_API_URL
来源：http://us.huanxung.cn

================================================================================
来源：http://gu.newstarts.cn

统计汇总
来源：http://ca.hahajie.cn

================================================================================
来源：http://xi.chemitech.net.cn

按语言统计（条）：
来源：http://gh.shxzskj.cn

Python ......... 252
来源：http://qr.9csxet.cn

PHP ............ 252
来源：http://ew.yuntaijiaju.cn

JavaScript ..... 252
来源：http://rp.haigaiapp.cn

TypeScript ..... 212
来源：http://ti.shtwfgs.cn

Java ........... 212
来源：http://xu.panjiajie.cn

Go ............. 212
来源：http://cp.shxzukj.cn

Ruby ........... 212
来源：http://eh.newstarts.cn

C# ............. 212
来源：http://cx.panjiajie.cn

C .............. 30
来源：http://bx.shtwfgs.cn

C++ ............ 30
来源：http://in.huanxung.cn

SQL ............ 90
来源：http://jg.newstarts.cn

Bash ........... 80
来源：http://sd.bjjhwx.cn

Kotlin ......... 15
来源：http://zn.huixiangedu.cn

Swift .......... 15
来源：http://zt.shtwfgs.cn

Lua ............ 10
来源：http://gb.hnjuh.cn

Perl ........... 10
来源：http://fe.shtwfgs.cn

Scala .......... 10
来源：http://by.lnxyls.cn

------------------------------------
来源：http://fs.colortex.cn

合计 ........... 2106 条
来源：http://dc.9csxet.cn

按章节统计：
来源：http://gq.wgjwhj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hd.szxytkj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lx.haigaiapp.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wl.haigaiapp.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dn.shtwfgs.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://iu.huanxung.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ey.shxzskj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jm.nicolike.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xi.huanxung.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ce.newstarts.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dy.jctech888.com.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tp.lnxyls.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://bs.muxihuayi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qu.nicolike.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kb.huixinmuqiang.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wl.shxzskj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hy.chemitech.net.cn

Q SQL 专题                              90
来源：http://hq.huixinmuqiang.cn

R Bash 专题                             80
来源：http://zl.lnxyls.cn

S C / C++ 专题                          60
来源：http://sk.bjjhwx.cn

T 其他语言补充                          60
来源：http://lp.haigaiapp.cn

U 高频实用片段                         120
来源：http://dw.huanxung.cn

------------------------------------
来源：http://mn.bjjhwx.cn

合计                                  2106 条
来源：http://nm.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://ul.colortex.cn

使用提醒
来源：http://gb.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://sx.hahajie.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://oa.hnjuh.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ed.9csxet.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ba.szsharing.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://cn.bjjhwx.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://sm.shtwfgs.cn

—— 文件结束 ——
来源：http://xc.shxzukj.cn

================================================================================
来源：http://qy.yuntaijiaju.cn

程序语言常见例子速查手册（2024 版）
来源：http://cv.szsharing.cn

Common Programming Examples Cheat Book
来源：http://vm.szsharing.cn

================================================================================
来源：http://wl.huanxung.cn

【收录内容】
来源：http://wt.newstarts.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://hu.bookmarksfly.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vj.colortex.cn

SQL · Bash · C · C++
来源：http://jc.shxzskj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ik.521024.cn

【使用说明】
来源：http://vf.panjiajie.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cw.jctech888.com.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ty.haigaiapp.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://yc.shxzukj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://md.9csxet.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://wu.wgjwhj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jp.lnxyls.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ea.9csxet.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dd.asd995.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ln.nicolike.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ay.shxzskj.cn


<!-- 参考信息 -->