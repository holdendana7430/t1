代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vg.panjiajie.cn

================================================================================
来源：http://fi.huanxung.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pp.9csxet.cn

================================================================================
来源：http://pj.gzmigu.cn

[U01] Py：创建虚拟环境
来源：http://yo.chemitech.net.cn

python -m venv .venv && source .venv/bin/activate
来源：http://td.shtwfgs.cn

[U02] Py：导出 / 安装依赖
来源：http://qw.chemitech.net.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bk.hnjuh.cn

[U03] Py：加载 .env 配置
来源：http://tp.colortex.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ch.jianghongdianzi.cn

[U04] Py：变量调试打印
来源：http://ac.huixinmuqiang.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hc.yuexingan06.cn

[U05] Py：列表去重且保序
来源：http://vl.chemitech.net.cn

list(dict.fromkeys(arr))
来源：http://if.jianghongdianzi.cn

[U06] Py：合并两个字典
来源：http://qa.asd995.cn

{**a, **b}
来源：http://pd.yuexingan06.cn

[U07] Py：反转字典键值
来源：http://nj.jctech888.com.cn

{v: k for k, v in d.items()}
来源：http://gm.huanxung.cn

[U08] Py：展平二维列表
来源：http://mi.9csxet.cn

[y for x in nested for y in x]
来源：http://dy.asd995.cn

[U09] Py：字典取最大值的键
来源：http://kv.hnjuh.cn

max(d, key=d.get)
来源：http://qv.huanxung.cn

[U10] Py：按值排序字典
来源：http://gz.huixinmuqiang.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ob.yuexingan06.cn

[U11] Py：生成器表达式
来源：http://mq.asd995.cn

(x * 2 for x in arr)
来源：http://wt.bjjhwx.cn

[U12] Py：取出现最多的 3 个元素
来源：http://sz.szxytkj.cn

Counter(arr).most_common(3)
来源：http://ks.shxzukj.cn

[U13] Py：固定长度队列
来源：http://iv.bookmarksfly.cn

deque(maxlen=10)
来源：http://ec.nszjky.cn

[U14] Py：分组收集到列表
来源：http://tb.huixiangedu.cn

defaultdict(list)
来源：http://rx.huixiangedu.cn

[U15] Py：高精度计时
来源：http://ah.hahajie.cn

t = time.perf_counter()
来源：http://vv.jianghongdianzi.cn

[U16] Py：命令行参数解析
来源：http://tw.shxzskj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pu.shxzukj.cn

[U17] Py：初始化日志
来源：http://yq.hnjuh.cn

logging.basicConfig(level=logging.INFO)
来源：http://aj.shxzskj.cn

[U18] Py：预编译正则
来源：http://jg.9csxet.cn

pat = re.compile(r"\d+")
来源：http://ml.asd995.cn

[U19] Py：正则替换带回调
来源：http://wi.colortex.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ek.muxihuayi.cn

[U20] Py：缓存函数结果
来源：http://fr.huixinmuqiang.cn

@functools.lru_cache(maxsize=None)
来源：http://ou.shxzukj.cn

[U21] Py：自定义上下文管理器
来源：http://tg.shxzukj.cn

@contextlib.contextmanager
来源：http://xs.wgjwhj.cn

[U22] Py：矩阵转置
来源：http://yo.9csxet.cn

list(zip(*m))
来源：http://pv.gzmigu.cn

[U23] Py：分块读取大文件
来源：http://dy.yuntaijiaju.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jr.haigaiapp.cn

[U24] Py：路径操作
来源：http://rt.nicolike.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://sh.521024.cn

[U25] Py：CSV 按字典读
来源：http://lr.colortex.cn

csv.DictReader(f)
来源：http://tm.9csxet.cn

[U26] Py：并发下载
来源：http://sc.asd995.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kp.huixiangedu.cn

[U27] Py：异步 HTTP
来源：http://sa.gzmigu.cn

aiohttp.ClientSession() 配合 async with
来源：http://do.hnjuh.cn

[U28] Py：类型别名
来源：http://pv.9csxet.cn

UserId = int
来源：http://aw.panjiajie.cn

[U29] Py：属性校验
来源：http://tb.9csxet.cn

@property 与 @x.setter 配合
来源：http://li.yuexingan06.cn

[U30] Py：数据类
来源：http://xw.asd995.cn

@dataclass(slots=True)
来源：http://wf.colortex.cn

[U31] Py：单测
来源：http://pl.huanxung.cn

python -m pytest -q
来源：http://wn.chemitech.net.cn

[U32] Py：代码格式化
来源：http://mg.yuntaijiaju.cn

ruff format . && ruff check --fix .
来源：http://ek.yuexingan06.cn

[U33] Py：打包发布
来源：http://gk.bjjhwx.cn

python -m build  （依赖 pyproject.toml）
来源：http://vs.huanxung.cn

[U34] Py：判断编码
来源：http://ij.huixinmuqiang.cn

chardet.detect(raw)
来源：http://fo.muxihuayi.cn

[U35] Py：发送邮件
来源：http://kt.haigaiapp.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gp.521024.cn

[U36] Py：定时任务
来源：http://hl.nicolike.cn

schedule.every(10).minutes.do(job)
来源：http://rr.shtwfgs.cn

[U37] Py：读写 Excel
来源：http://cc.jianghongdianzi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://pw.panjiajie.cn

[U38] Py：获取脚本所在目录
来源：http://og.szxytkj.cn

Path(__file__).resolve().parent
来源：http://kb.shtwfgs.cn

[U39] Py：判断是否在交互环境
来源：http://zg.szsharing.cn

sys.stdout.isatty()
来源：http://dg.nicolike.cn

[U40] Py：打印到标准错误
来源：http://vr.szxytkj.cn

print("err", file=sys.stderr)
来源：http://ro.yuexingan06.cn

[U41] PHP：初始化 Composer 项目
来源：http://qi.chemitech.net.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qn.nszjky.cn

[U42] PHP：PSR-4 自动加载
来源：http://zj.gzmigu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rz.nszjky.cn

[U43] PHP：声明命名空间
来源：http://xx.panjiajie.cn

namespace App\Http;
来源：http://zb.panjiajie.cn

[U44] PHP：开启严格类型
来源：http://ko.newstarts.cn

declare(strict_types=1);
来源：http://of.hahajie.cn

[U45] PHP：类型声明与返回类型
来源：http://bo.jianghongdianzi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qn.haigaiapp.cn

[U46] PHP：可空类型
来源：http://cl.chemitech.net.cn

?string $name = null
来源：http://tc.bjjhwx.cn

[U47] PHP：联合类型
来源：http://cu.colortex.cn

int|string $id
来源：http://hv.gzmigu.cn

[U48] PHP：纯枚举
来源：http://cj.shxzskj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gl.huixinmuqiang.cn

[U49] PHP：只读属性
来源：http://fs.newstarts.cn

public readonly string $name
来源：http://yn.huixiangedu.cn

[U50] PHP：构造器属性提升
来源：http://mk.muxihuayi.cn

public function __construct(private int $id) {}
来源：http://dv.lnxyls.cn

[U51] PHP：数组解构
来源：http://qw.jianghongdianzi.cn

[$a, $b] = $arr;
来源：http://dt.chemitech.net.cn

[U52] PHP：箭头函数
来源：http://kx.haigaiapp.cn

$double = fn($x) => $x * 2;
来源：http://zc.yuntaijiaju.cn

[U53] PHP：空合并运算符
来源：http://xc.nszjky.cn

$v = $a ?? $b ?? "default";
来源：http://nv.szxytkj.cn

[U54] PHP：空安全调用
来源：http://ti.lnxyls.cn

$obj?->method()
来源：http://yh.huixinmuqiang.cn

[U55] PHP：match 表达式
来源：http://js.hnjuh.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nn.shxzskj.cn

[U56] PHP：命名参数
来源：http://xv.chemitech.net.cn

f(a: 1, b: 2)
来源：http://ne.lnxyls.cn

[U57] PHP：字符串插值
来源：http://cz.yuexingan06.cn

"值: {$a}"
来源：http://qw.colortex.cn

[U58] PHP：数组三件套
来源：http://ac.yuntaijiaju.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kj.jianghongdianzi.cn

[U59] PHP：自定义排序
来源：http://jn.szsharing.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gr.shxzskj.cn

[U60] PHP：JSON 编解码
来源：http://wm.yuexingan06.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bc.asd995.cn

[U61] PHP：正则
来源：http://mz.asd995.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fb.hahajie.cn

[U62] PHP：日期对象
来源：http://jf.szsharing.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wv.hahajie.cn

[U63] PHP：文件读写
来源：http://fs.yuntaijiaju.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ku.colortex.cn

[U64] PHP：目录遍历
来源：http://oh.huixinmuqiang.cn

glob("dir/*.php");  scandir("dir");
来源：http://yd.bjjhwx.cn

[U65] PHP：会话
来源：http://ai.asd995.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://hf.colortex.cn

[U66] PHP：设置 Cookie
来源：http://gc.nszjky.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://li.wgjwhj.cn

[U67] PHP：处理文件上传
来源：http://oj.huixinmuqiang.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lw.asd995.cn

[U68] PHP：PDO 连接
来源：http://ue.hnjuh.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zv.huanxung.cn

[U69] PHP：PDO 预处理
来源：http://tw.hahajie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ac.szxytkj.cn

[U70] PHP：PDO 事务
来源：http://sh.szsharing.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tr.yuntaijiaju.cn

[U71] PHP：抛出异常
来源：http://ko.nicolike.cn

throw new RuntimeException("失败", 500);
来源：http://vw.wgjwhj.cn

[U72] PHP：写错误日志
来源：http://le.newstarts.cn

error_log("失败: " . $e->getMessage());
来源：http://ui.haigaiapp.cn

[U73] PHP：读取 ini 配置
来源：http://uo.bjjhwx.cn

parse_ini_file("config.ini", true)
来源：http://vl.shtwfgs.cn

[U74] PHP：读取环境变量
来源：http://no.521024.cn

getenv("APP_ENV") ?: "production"
来源：http://ju.nicolike.cn

[U75] PHP：依赖注入
来源：http://sd.huixinmuqiang.cn

composer require psr/container
来源：http://dq.colortex.cn

[U76] PHP：简单路由
来源：http://nd.huanxung.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kp.colortex.cn

[U77] PHP：模板渲染
来源：http://om.huixiangedu.cn

composer require twig/twig
来源：http://jr.bjjhwx.cn

[U78] PHP：单元测试
来源：http://yt.gzmigu.cn

composer require --dev phpunit/phpunit
来源：http://dc.gzmigu.cn

[U79] PHP：静态分析
来源：http://wx.szsharing.cn

composer require --dev phpstan/phpstan
来源：http://jn.yuntaijiaju.cn

[U80] PHP：代码规范修复
来源：http://vj.panjiajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ga.hahajie.cn

[U81] JS：初始化项目
来源：http://ap.bookmarksfly.cn

npm init -y;  npm i express
来源：http://tw.shxzskj.cn

[U82] JS：package.json 脚本
来源：http://zi.huixiangedu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qm.yuexingan06.cn

[U83] JS：ES Module 导入导出
来源：http://zt.shxzukj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ld.shtwfgs.cn

[U84] JS：CommonJS 写法
来源：http://aw.chemitech.net.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ut.jctech888.com.cn

[U85] JS：可选链
来源：http://me.521024.cn

a?.b?.c
来源：http://bf.bookmarksfly.cn

[U86] JS：空值合并
来源：http://ma.yuexingan06.cn

a ?? b
来源：http://zk.wgjwhj.cn

[U87] JS：解构默认值
来源：http://vn.huixiangedu.cn

const { a = 1, b = 2 } = obj;
来源：http://dy.yuntaijiaju.cn

[U88] JS：对象展开合并
来源：http://ap.yuntaijiaju.cn

{ ...a, ...b }
来源：http://uz.bjjhwx.cn

[U89] JS：数组去重
来源：http://aw.huixiangedu.cn

[...new Set(arr)]
来源：http://gp.yuexingan06.cn

[U90] JS：数字数组排序
来源：http://yh.9csxet.cn

[...arr].sort((a, b) => a - b)
来源：http://gn.newstarts.cn

[U91] JS：对象键值遍历
来源：http://ta.hnjuh.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://te.huixiangedu.cn

[U92] JS：深拷贝
来源：http://ww.lnxyls.cn

structuredClone(obj)
来源：http://uj.asd995.cn

[U93] JS：模板字符串
来源：http://uc.huanxung.cn

`共 ${n} 条`
来源：http://qn.huanxung.cn

[U94] JS：箭头函数
来源：http://tb.muxihuayi.cn

const double = x => x * 2;
来源：http://rg.szsharing.cn

[U95] JS：Promise 包装
来源：http://nm.yuntaijiaju.cn

new Promise((resolve, reject) => {})
来源：http://il.yuexingan06.cn

[U96] JS：async/await 与异常
来源：http://kn.wgjwhj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jc.jctech888.com.cn

[U97] JS：并发请求
来源：http://nn.hnjuh.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://tw.huanxung.cn

[U98] JS：fetch 带 JSON
来源：http://df.szxytkj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rq.nicolike.cn

[U99] JS：事件监听
来源：http://kc.asd995.cn

el.addEventListener("click", e => {})
来源：http://sq.newstarts.cn

[U100] JS：DOM 查询
来源：http://jm.9csxet.cn

document.querySelector(".item")
来源：http://na.szsharing.cn

[U101] JS：classList 操作
来源：http://ey.huanxung.cn

el.classList.toggle("active")
来源：http://bd.jctech888.com.cn

[U102] JS：本地存储
来源：http://ho.9csxet.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://la.lnxyls.cn

[U103] JS：定时器
来源：http://kg.9csxet.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://th.huanxung.cn

[U104] JS：防抖
来源：http://mk.nicolike.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jj.muxihuayi.cn

[U105] JS：节流
来源：http://ne.huixinmuqiang.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://uv.asd995.cn

[U106] JS：日期格式化
来源：http://nq.newstarts.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ky.muxihuayi.cn

[U107] JS：数字千分位
来源：http://ei.shxzukj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://np.shxzukj.cn

[U108] JS：随机整数
来源：http://ph.colortex.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ak.nszjky.cn

[U109] JS：数组分组
来源：http://dt.haigaiapp.cn

Object.groupBy(arr, x => x.type)
来源：http://cf.huixinmuqiang.cn

[U110] JS：数组分块
来源：http://pr.nicolike.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cr.szxytkj.cn

[U111] JS：对象转 Map
来源：http://db.gzmigu.cn

new Map(Object.entries(obj))
来源：http://ex.jctech888.com.cn

[U112] JS：字符串补位
来源：http://ht.nicolike.cn

"7".padStart(3, "0")
来源：http://fq.newstarts.cn

[U113] JS：正则替换全部
来源：http://ss.colortex.cn

s.replaceAll("a", "b")
来源：http://os.lnxyls.cn

[U114] JS：JSON 深比较
来源：http://pr.bjjhwx.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://lr.shxzukj.cn

[U115] JS：生成 UUID
来源：http://gt.huixiangedu.cn

crypto.randomUUID()
来源：http://mb.jctech888.com.cn

[U116] JS：类型检查（JSDoc）
来源：http://fx.nicolike.cn

/** @param {string} name */ function f(name) {}
来源：http://ky.hahajie.cn

[U117] JS：单元测试
来源：http://td.huixiangedu.cn

npm i -D vitest;  npx vitest
来源：http://al.chemitech.net.cn

[U118] JS：开发服务器
来源：http://av.lnxyls.cn

npm i -D vite;  npx vite
来源：http://zq.gzmigu.cn

[U119] JS：生产构建
来源：http://fp.colortex.cn

npx vite build
来源：http://wk.hnjuh.cn

[U120] JS：读取环境变量（Vite）
来源：http://yw.haigaiapp.cn

import.meta.env.VITE_API_URL
来源：http://ly.hnjuh.cn

================================================================================
来源：http://fr.asd995.cn

统计汇总
来源：http://rr.newstarts.cn

================================================================================
来源：http://wz.asd995.cn

按语言统计（条）：
来源：http://te.shtwfgs.cn

Python ......... 252
来源：http://iq.nicolike.cn

PHP ............ 252
来源：http://wl.9csxet.cn

JavaScript ..... 252
来源：http://ok.yuexingan06.cn

TypeScript ..... 212
来源：http://hz.huanxung.cn

Java ........... 212
来源：http://vr.nszjky.cn

Go ............. 212
来源：http://wu.wgjwhj.cn

Ruby ........... 212
来源：http://ov.hnjuh.cn

C# ............. 212
来源：http://pl.gzmigu.cn

C .............. 30
来源：http://az.gzmigu.cn

C++ ............ 30
来源：http://ie.shtwfgs.cn

SQL ............ 90
来源：http://vm.haigaiapp.cn

Bash ........... 80
来源：http://xs.szxytkj.cn

Kotlin ......... 15
来源：http://ix.yuexingan06.cn

Swift .......... 15
来源：http://jt.9csxet.cn

Lua ............ 10
来源：http://lb.wgjwhj.cn

Perl ........... 10
来源：http://kf.huixinmuqiang.cn

Scala .......... 10
来源：http://rb.hnjuh.cn

------------------------------------
来源：http://np.jctech888.com.cn

合计 ........... 2106 条
来源：http://gq.szsharing.cn

按章节统计：
来源：http://pz.szsharing.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://my.hahajie.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://de.huixinmuqiang.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lx.wgjwhj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://sc.muxihuayi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dj.bjjhwx.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wm.nszjky.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://az.newstarts.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bc.nszjky.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://or.hnjuh.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mw.jctech888.com.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ob.hahajie.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fq.haigaiapp.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gi.nicolike.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zb.jctech888.com.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kj.gzmigu.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qa.9csxet.cn

Q SQL 专题                              90
来源：http://kz.shxzukj.cn

R Bash 专题                             80
来源：http://zh.huanxung.cn

S C / C++ 专题                          60
来源：http://yk.bjjhwx.cn

T 其他语言补充                          60
来源：http://uq.jianghongdianzi.cn

U 高频实用片段                         120
来源：http://rb.szsharing.cn

------------------------------------
来源：http://fv.jctech888.com.cn

合计                                  2106 条
来源：http://rv.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://zb.hnjuh.cn

使用提醒
来源：http://dd.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://jg.newstarts.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jh.bjjhwx.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ql.yuntaijiaju.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yb.hahajie.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://tv.colortex.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://yp.jctech888.com.cn

—— 文件结束 ——
来源：http://jx.hnjuh.cn


<!-- 参考信息 -->