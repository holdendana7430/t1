代发 wailian999

[U01] Py：创建虚拟环境
来源：http://vy.huanxung.cn

python -m venv .venv && source .venv/bin/activate
来源：http://fl.nszjky.cn

[U02] Py：导出 / 安装依赖
来源：http://qc.nicolike.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://sq.jctech888.com.cn

[U03] Py：加载 .env 配置
来源：http://ka.jctech888.com.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://np.jctech888.com.cn

[U04] Py：变量调试打印
来源：http://ix.jianghongdianzi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rj.szxytkj.cn

[U05] Py：列表去重且保序
来源：http://kv.521024.cn

list(dict.fromkeys(arr))
来源：http://xf.jctech888.com.cn

[U06] Py：合并两个字典
来源：http://ib.jctech888.com.cn

{**a, **b}
来源：http://ld.huixiangedu.cn

[U07] Py：反转字典键值
来源：http://gg.newstarts.cn

{v: k for k, v in d.items()}
来源：http://yl.shtwfgs.cn

[U08] Py：展平二维列表
来源：http://lz.nszjky.cn

[y for x in nested for y in x]
来源：http://wa.shxzukj.cn

[U09] Py：字典取最大值的键
来源：http://fn.yuexingan06.cn

max(d, key=d.get)
来源：http://fx.lnxyls.cn

[U10] Py：按值排序字典
来源：http://yr.asd995.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qc.yuexingan06.cn

[U11] Py：生成器表达式
来源：http://jb.szsharing.cn

(x * 2 for x in arr)
来源：http://qw.szsharing.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mm.huanxung.cn

Counter(arr).most_common(3)
来源：http://ge.huixinmuqiang.cn

[U13] Py：固定长度队列
来源：http://yd.yuexingan06.cn

deque(maxlen=10)
来源：http://sl.shtwfgs.cn

[U14] Py：分组收集到列表
来源：http://mp.colortex.cn

defaultdict(list)
来源：http://gk.panjiajie.cn

[U15] Py：高精度计时
来源：http://it.colortex.cn

t = time.perf_counter()
来源：http://am.jctech888.com.cn

[U16] Py：命令行参数解析
来源：http://xq.gzmigu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zx.yuexingan06.cn

[U17] Py：初始化日志
来源：http://ai.hahajie.cn

logging.basicConfig(level=logging.INFO)
来源：http://jm.jianghongdianzi.cn

[U18] Py：预编译正则
来源：http://li.chemitech.net.cn

pat = re.compile(r"\d+")
来源：http://id.huanxung.cn

[U19] Py：正则替换带回调
来源：http://yv.shtwfgs.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://df.asd995.cn

[U20] Py：缓存函数结果
来源：http://dh.jianghongdianzi.cn

@functools.lru_cache(maxsize=None)
来源：http://fa.nszjky.cn

[U21] Py：自定义上下文管理器
来源：http://yj.shtwfgs.cn

@contextlib.contextmanager
来源：http://td.asd995.cn

[U22] Py：矩阵转置
来源：http://st.lnxyls.cn

list(zip(*m))
来源：http://wk.jctech888.com.cn

[U23] Py：分块读取大文件
来源：http://up.nszjky.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gs.lnxyls.cn

[U24] Py：路径操作
来源：http://gf.huanxung.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pw.wgjwhj.cn

[U25] Py：CSV 按字典读
来源：http://av.wgjwhj.cn

csv.DictReader(f)
来源：http://uv.lnxyls.cn

[U26] Py：并发下载
来源：http://qp.hnjuh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ea.nicolike.cn

[U27] Py：异步 HTTP
来源：http://bw.panjiajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://kv.newstarts.cn

[U28] Py：类型别名
来源：http://dc.9csxet.cn

UserId = int
来源：http://ie.yuntaijiaju.cn

[U29] Py：属性校验
来源：http://mx.521024.cn

@property 与 @x.setter 配合
来源：http://lw.shtwfgs.cn

[U30] Py：数据类
来源：http://si.wgjwhj.cn

@dataclass(slots=True)
来源：http://yl.huanxung.cn

[U31] Py：单测
来源：http://uz.hahajie.cn

python -m pytest -q
来源：http://yy.9csxet.cn

[U32] Py：代码格式化
来源：http://gt.nicolike.cn

ruff format . && ruff check --fix .
来源：http://xq.shtwfgs.cn

[U33] Py：打包发布
来源：http://wc.colortex.cn

python -m build  （依赖 pyproject.toml）
来源：http://hj.shtwfgs.cn

[U34] Py：判断编码
来源：http://ce.shxzskj.cn

chardet.detect(raw)
来源：http://zi.colortex.cn

[U35] Py：发送邮件
来源：http://vw.shxzskj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ec.bookmarksfly.cn

[U36] Py：定时任务
来源：http://ll.szsharing.cn

schedule.every(10).minutes.do(job)
来源：http://nk.shtwfgs.cn

[U37] Py：读写 Excel
来源：http://du.asd995.cn

pandas.read_excel / DataFrame.to_excel
来源：http://aq.521024.cn

[U38] Py：获取脚本所在目录
来源：http://yc.9csxet.cn

Path(__file__).resolve().parent
来源：http://uh.shtwfgs.cn

[U39] Py：判断是否在交互环境
来源：http://ta.muxihuayi.cn

sys.stdout.isatty()
来源：http://vi.szxytkj.cn

[U40] Py：打印到标准错误
来源：http://xl.jctech888.com.cn

print("err", file=sys.stderr)
来源：http://nq.wgjwhj.cn

[U41] PHP：初始化 Composer 项目
来源：http://hp.9csxet.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://bn.szxytkj.cn

[U42] PHP：PSR-4 自动加载
来源：http://tp.hahajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hx.yuntaijiaju.cn

[U43] PHP：声明命名空间
来源：http://dl.huixiangedu.cn

namespace App\Http;
来源：http://ck.hahajie.cn

[U44] PHP：开启严格类型
来源：http://os.gzmigu.cn

declare(strict_types=1);
来源：http://tp.jctech888.com.cn

[U45] PHP：类型声明与返回类型
来源：http://pv.huixiangedu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://tf.jianghongdianzi.cn

[U46] PHP：可空类型
来源：http://kb.asd995.cn

?string $name = null
来源：http://fn.jctech888.com.cn

[U47] PHP：联合类型
来源：http://am.jianghongdianzi.cn

int|string $id
来源：http://ke.nszjky.cn

[U48] PHP：纯枚举
来源：http://sj.muxihuayi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wv.bookmarksfly.cn

[U49] PHP：只读属性
来源：http://dt.haigaiapp.cn

public readonly string $name
来源：http://pt.huanxung.cn

[U50] PHP：构造器属性提升
来源：http://ne.9csxet.cn

public function __construct(private int $id) {}
来源：http://su.shxzukj.cn

[U51] PHP：数组解构
来源：http://rh.hahajie.cn

[$a, $b] = $arr;
来源：http://aq.shxzukj.cn

[U52] PHP：箭头函数
来源：http://or.521024.cn

$double = fn($x) => $x * 2;
来源：http://pv.gzmigu.cn

[U53] PHP：空合并运算符
来源：http://zs.jianghongdianzi.cn

$v = $a ?? $b ?? "default";
来源：http://ud.shxzukj.cn

[U54] PHP：空安全调用
来源：http://zk.nicolike.cn

$obj?->method()
来源：http://ap.lnxyls.cn

[U55] PHP：match 表达式
来源：http://en.panjiajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ok.panjiajie.cn

[U56] PHP：命名参数
来源：http://xp.bjjhwx.cn

f(a: 1, b: 2)
来源：http://te.shxzukj.cn

[U57] PHP：字符串插值
来源：http://ea.newstarts.cn

"值: {$a}"
来源：http://vx.bjjhwx.cn

[U58] PHP：数组三件套
来源：http://mf.521024.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ld.chemitech.net.cn

[U59] PHP：自定义排序
来源：http://rw.bookmarksfly.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ni.szsharing.cn

[U60] PHP：JSON 编解码
来源：http://di.haigaiapp.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kt.hnjuh.cn

[U61] PHP：正则
来源：http://gb.szsharing.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://df.huixinmuqiang.cn

[U62] PHP：日期对象
来源：http://yl.lnxyls.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rh.bjjhwx.cn

[U63] PHP：文件读写
来源：http://jh.bjjhwx.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://iv.haigaiapp.cn

[U64] PHP：目录遍历
来源：http://ct.hnjuh.cn

glob("dir/*.php");  scandir("dir");
来源：http://yp.haigaiapp.cn

[U65] PHP：会话
来源：http://hx.colortex.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://xq.shxzukj.cn

[U66] PHP：设置 Cookie
来源：http://ot.bookmarksfly.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cv.521024.cn

[U67] PHP：处理文件上传
来源：http://ro.nszjky.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zh.chemitech.net.cn

[U68] PHP：PDO 连接
来源：http://di.huanxung.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zl.shxzukj.cn

[U69] PHP：PDO 预处理
来源：http://eu.521024.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://or.hahajie.cn

[U70] PHP：PDO 事务
来源：http://zy.colortex.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qf.bjjhwx.cn

[U71] PHP：抛出异常
来源：http://yz.asd995.cn

throw new RuntimeException("失败", 500);
来源：http://nn.yuntaijiaju.cn

[U72] PHP：写错误日志
来源：http://hs.huixiangedu.cn

error_log("失败: " . $e->getMessage());
来源：http://im.hahajie.cn

[U73] PHP：读取 ini 配置
来源：http://je.huanxung.cn

parse_ini_file("config.ini", true)
来源：http://iy.shxzukj.cn

[U74] PHP：读取环境变量
来源：http://rv.haigaiapp.cn

getenv("APP_ENV") ?: "production"
来源：http://cr.hahajie.cn

[U75] PHP：依赖注入
来源：http://so.yuntaijiaju.cn

composer require psr/container
来源：http://tz.hnjuh.cn

[U76] PHP：简单路由
来源：http://sk.521024.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gg.yuntaijiaju.cn

[U77] PHP：模板渲染
来源：http://mr.nszjky.cn

composer require twig/twig
来源：http://re.colortex.cn

[U78] PHP：单元测试
来源：http://az.huixiangedu.cn

composer require --dev phpunit/phpunit
来源：http://lh.521024.cn

[U79] PHP：静态分析
来源：http://as.shxzukj.cn

composer require --dev phpstan/phpstan
来源：http://kf.9csxet.cn

[U80] PHP：代码规范修复
来源：http://zs.huixiangedu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ee.hahajie.cn

[U81] JS：初始化项目
来源：http://tb.hnjuh.cn

npm init -y;  npm i express
来源：http://ha.huixinmuqiang.cn

[U82] JS：package.json 脚本
来源：http://qe.huixiangedu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mv.9csxet.cn

[U83] JS：ES Module 导入导出
来源：http://lf.nszjky.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ym.huanxung.cn

[U84] JS：CommonJS 写法
来源：http://yy.huanxung.cn

module.exports = { a };  const { a } = require("./m");
来源：http://am.yuntaijiaju.cn

[U85] JS：可选链
来源：http://rn.yuexingan06.cn

a?.b?.c
来源：http://ol.yuexingan06.cn

[U86] JS：空值合并
来源：http://ga.hahajie.cn

a ?? b
来源：http://qu.yuexingan06.cn

[U87] JS：解构默认值
来源：http://vu.bookmarksfly.cn

const { a = 1, b = 2 } = obj;
来源：http://au.wgjwhj.cn

[U88] JS：对象展开合并
来源：http://ix.huixiangedu.cn

{ ...a, ...b }
来源：http://io.szsharing.cn

[U89] JS：数组去重
来源：http://zy.hahajie.cn

[...new Set(arr)]
来源：http://ho.shxzskj.cn

[U90] JS：数字数组排序
来源：http://yz.asd995.cn

[...arr].sort((a, b) => a - b)
来源：http://rw.szxytkj.cn

[U91] JS：对象键值遍历
来源：http://xz.shtwfgs.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gr.bjjhwx.cn

[U92] JS：深拷贝
来源：http://wv.chemitech.net.cn

structuredClone(obj)
来源：http://vz.chemitech.net.cn

[U93] JS：模板字符串
来源：http://to.huanxung.cn

`共 ${n} 条`
来源：http://jp.gzmigu.cn

[U94] JS：箭头函数
来源：http://fu.huixiangedu.cn

const double = x => x * 2;
来源：http://dt.szsharing.cn

[U95] JS：Promise 包装
来源：http://ke.szxytkj.cn

new Promise((resolve, reject) => {})
来源：http://nl.gzmigu.cn

[U96] JS：async/await 与异常
来源：http://rb.shxzskj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ws.yuntaijiaju.cn

[U97] JS：并发请求
来源：http://up.huanxung.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://nj.bjjhwx.cn

[U98] JS：fetch 带 JSON
来源：http://sm.hahajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fn.newstarts.cn

[U99] JS：事件监听
来源：http://lr.521024.cn

el.addEventListener("click", e => {})
来源：http://rq.muxihuayi.cn

[U100] JS：DOM 查询
来源：http://ru.nszjky.cn

document.querySelector(".item")
来源：http://xs.9csxet.cn

[U101] JS：classList 操作
来源：http://ns.asd995.cn

el.classList.toggle("active")
来源：http://ld.huanxung.cn

[U102] JS：本地存储
来源：http://ba.jianghongdianzi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ji.colortex.cn

[U103] JS：定时器
来源：http://pb.gzmigu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lc.jctech888.com.cn

[U104] JS：防抖
来源：http://tt.panjiajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pe.jctech888.com.cn

[U105] JS：节流
来源：http://el.nszjky.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vs.szsharing.cn

[U106] JS：日期格式化
来源：http://gr.colortex.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xz.muxihuayi.cn

[U107] JS：数字千分位
来源：http://ix.haigaiapp.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nh.panjiajie.cn

[U108] JS：随机整数
来源：http://pg.huixiangedu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dz.nszjky.cn

[U109] JS：数组分组
来源：http://zp.huixiangedu.cn

Object.groupBy(arr, x => x.type)
来源：http://qe.nszjky.cn

[U110] JS：数组分块
来源：http://rc.szxytkj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://uc.colortex.cn

[U111] JS：对象转 Map
来源：http://tj.wgjwhj.cn

new Map(Object.entries(obj))
来源：http://tr.yuexingan06.cn

[U112] JS：字符串补位
来源：http://oz.gzmigu.cn

"7".padStart(3, "0")
来源：http://de.9csxet.cn

[U113] JS：正则替换全部
来源：http://mj.shtwfgs.cn

s.replaceAll("a", "b")
来源：http://zn.9csxet.cn

[U114] JS：JSON 深比较
来源：http://af.shxzukj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://jq.bjjhwx.cn

[U115] JS：生成 UUID
来源：http://ux.lnxyls.cn

crypto.randomUUID()
来源：http://yi.nszjky.cn

[U116] JS：类型检查（JSDoc）
来源：http://fb.9csxet.cn

/** @param {string} name */ function f(name) {}
来源：http://wj.521024.cn

[U117] JS：单元测试
来源：http://xa.bjjhwx.cn

npm i -D vitest;  npx vitest
来源：http://bk.newstarts.cn

[U118] JS：开发服务器
来源：http://nu.bjjhwx.cn

npm i -D vite;  npx vite
来源：http://br.shxzskj.cn

[U119] JS：生产构建
来源：http://lz.wgjwhj.cn

npx vite build
来源：http://yz.lnxyls.cn

[U120] JS：读取环境变量（Vite）
来源：http://ov.szxytkj.cn

import.meta.env.VITE_API_URL
来源：http://qh.521024.cn

================================================================================
来源：http://ii.hnjuh.cn

统计汇总
来源：http://fb.hnjuh.cn

================================================================================
来源：http://gr.bookmarksfly.cn

按语言统计（条）：
来源：http://nw.lnxyls.cn

Python ......... 252
来源：http://qv.jctech888.com.cn

PHP ............ 252
来源：http://th.huixiangedu.cn

JavaScript ..... 252
来源：http://yi.panjiajie.cn

TypeScript ..... 212
来源：http://qn.nicolike.cn

Java ........... 212
来源：http://wu.jianghongdianzi.cn

Go ............. 212
来源：http://jl.yuntaijiaju.cn

Ruby ........... 212
来源：http://zi.shxzskj.cn

C# ............. 212
来源：http://cv.newstarts.cn

C .............. 30
来源：http://ct.haigaiapp.cn

C++ ............ 30
来源：http://by.yuntaijiaju.cn

SQL ............ 90
来源：http://ai.hnjuh.cn

Bash ........... 80
来源：http://em.bookmarksfly.cn

Kotlin ......... 15
来源：http://ro.huanxung.cn

Swift .......... 15
来源：http://mi.bookmarksfly.cn

Lua ............ 10
来源：http://ry.szxytkj.cn

Perl ........... 10
来源：http://yl.bjjhwx.cn

Scala .......... 10
来源：http://sl.panjiajie.cn

------------------------------------
来源：http://zz.jianghongdianzi.cn

合计 ........... 2106 条
来源：http://io.muxihuayi.cn

按章节统计：
来源：http://ai.szsharing.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://oc.yuexingan06.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ks.szxytkj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://su.nicolike.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vk.521024.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ly.szsharing.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pj.hnjuh.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wk.wgjwhj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jl.shxzukj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hc.lnxyls.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hb.bjjhwx.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fj.nicolike.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zb.muxihuayi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://yf.lnxyls.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pp.shxzukj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hy.newstarts.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yd.wgjwhj.cn

Q SQL 专题                              90
来源：http://np.huixinmuqiang.cn

R Bash 专题                             80
来源：http://sy.huixinmuqiang.cn

S C / C++ 专题                          60
来源：http://za.yuntaijiaju.cn

T 其他语言补充                          60
来源：http://wx.bjjhwx.cn

U 高频实用片段                         120
来源：http://ck.huanxung.cn

------------------------------------
来源：http://sn.shtwfgs.cn

合计                                  2106 条
来源：http://vk.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://pq.newstarts.cn

使用提醒
来源：http://fc.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://uj.gzmigu.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ym.huanxung.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ab.bookmarksfly.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ao.chemitech.net.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ir.9csxet.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mr.hnjuh.cn

—— 文件结束 ——
来源：http://pq.bjjhwx.cn

================================================================================
来源：http://tx.asd995.cn

程序语言常见例子速查手册（2024 版）
来源：http://zq.shxzskj.cn

Common Programming Examples Cheat Book
来源：http://mw.panjiajie.cn

================================================================================
来源：http://ii.szsharing.cn


<!-- 参考信息 -->