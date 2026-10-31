代发 wailian999

[U03] Py：加载 .env 配置
来源：http://ve.yuexingan06.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://if.haigaiapp.cn

[U04] Py：变量调试打印
来源：http://uo.shxzukj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pd.wgjwhj.cn

[U05] Py：列表去重且保序
来源：http://fg.yuexingan06.cn

list(dict.fromkeys(arr))
来源：http://uf.szxytkj.cn

[U06] Py：合并两个字典
来源：http://xr.haigaiapp.cn

{**a, **b}
来源：http://rn.bookmarksfly.cn

[U07] Py：反转字典键值
来源：http://zb.huanxung.cn

{v: k for k, v in d.items()}
来源：http://sv.huixiangedu.cn

[U08] Py：展平二维列表
来源：http://rd.shtwfgs.cn

[y for x in nested for y in x]
来源：http://my.szxytkj.cn

[U09] Py：字典取最大值的键
来源：http://tb.panjiajie.cn

max(d, key=d.get)
来源：http://vc.chemitech.net.cn

[U10] Py：按值排序字典
来源：http://ky.huanxung.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://os.yuexingan06.cn

[U11] Py：生成器表达式
来源：http://fe.wgjwhj.cn

(x * 2 for x in arr)
来源：http://wb.newstarts.cn

[U12] Py：取出现最多的 3 个元素
来源：http://jh.nicolike.cn

Counter(arr).most_common(3)
来源：http://yp.chemitech.net.cn

[U13] Py：固定长度队列
来源：http://gp.9csxet.cn

deque(maxlen=10)
来源：http://kn.bjjhwx.cn

[U14] Py：分组收集到列表
来源：http://ii.nicolike.cn

defaultdict(list)
来源：http://ev.lnxyls.cn

[U15] Py：高精度计时
来源：http://ws.panjiajie.cn

t = time.perf_counter()
来源：http://ac.nszjky.cn

[U16] Py：命令行参数解析
来源：http://he.szxytkj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fc.szsharing.cn

[U17] Py：初始化日志
来源：http://nr.gzmigu.cn

logging.basicConfig(level=logging.INFO)
来源：http://gw.yuntaijiaju.cn

[U18] Py：预编译正则
来源：http://pt.yuntaijiaju.cn

pat = re.compile(r"\d+")
来源：http://rw.asd995.cn

[U19] Py：正则替换带回调
来源：http://ri.jctech888.com.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rb.jctech888.com.cn

[U20] Py：缓存函数结果
来源：http://ha.521024.cn

@functools.lru_cache(maxsize=None)
来源：http://by.newstarts.cn

[U21] Py：自定义上下文管理器
来源：http://kn.huixinmuqiang.cn

@contextlib.contextmanager
来源：http://hu.jianghongdianzi.cn

[U22] Py：矩阵转置
来源：http://nr.huanxung.cn

list(zip(*m))
来源：http://mi.yuexingan06.cn

[U23] Py：分块读取大文件
来源：http://ha.chemitech.net.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qc.newstarts.cn

[U24] Py：路径操作
来源：http://vb.gzmigu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://aw.521024.cn

[U25] Py：CSV 按字典读
来源：http://gs.yuexingan06.cn

csv.DictReader(f)
来源：http://rn.huixinmuqiang.cn

[U26] Py：并发下载
来源：http://jd.hnjuh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://np.szxytkj.cn

[U27] Py：异步 HTTP
来源：http://wr.colortex.cn

aiohttp.ClientSession() 配合 async with
来源：http://rk.nicolike.cn

[U28] Py：类型别名
来源：http://mv.asd995.cn

UserId = int
来源：http://fe.huixiangedu.cn

[U29] Py：属性校验
来源：http://ae.yuntaijiaju.cn

@property 与 @x.setter 配合
来源：http://qa.9csxet.cn

[U30] Py：数据类
来源：http://dl.newstarts.cn

@dataclass(slots=True)
来源：http://jz.huixiangedu.cn

[U31] Py：单测
来源：http://wr.shtwfgs.cn

python -m pytest -q
来源：http://sj.yuntaijiaju.cn

[U32] Py：代码格式化
来源：http://vp.nicolike.cn

ruff format . && ruff check --fix .
来源：http://yj.shxzskj.cn

[U33] Py：打包发布
来源：http://dh.huanxung.cn

python -m build  （依赖 pyproject.toml）
来源：http://wn.haigaiapp.cn

[U34] Py：判断编码
来源：http://ij.newstarts.cn

chardet.detect(raw)
来源：http://jp.nicolike.cn

[U35] Py：发送邮件
来源：http://jz.huanxung.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wu.szxytkj.cn

[U36] Py：定时任务
来源：http://mb.chemitech.net.cn

schedule.every(10).minutes.do(job)
来源：http://nj.asd995.cn

[U37] Py：读写 Excel
来源：http://wa.gzmigu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://tl.muxihuayi.cn

[U38] Py：获取脚本所在目录
来源：http://no.newstarts.cn

Path(__file__).resolve().parent
来源：http://sb.huixiangedu.cn

[U39] Py：判断是否在交互环境
来源：http://vz.9csxet.cn

sys.stdout.isatty()
来源：http://hn.panjiajie.cn

[U40] Py：打印到标准错误
来源：http://nl.bookmarksfly.cn

print("err", file=sys.stderr)
来源：http://go.bookmarksfly.cn

[U41] PHP：初始化 Composer 项目
来源：http://km.9csxet.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://sq.szsharing.cn

[U42] PHP：PSR-4 自动加载
来源：http://en.chemitech.net.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mv.yuntaijiaju.cn

[U43] PHP：声明命名空间
来源：http://vl.9csxet.cn

namespace App\Http;
来源：http://cq.nszjky.cn

[U44] PHP：开启严格类型
来源：http://iz.hnjuh.cn

declare(strict_types=1);
来源：http://hx.szxytkj.cn

[U45] PHP：类型声明与返回类型
来源：http://de.asd995.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qn.huanxung.cn

[U46] PHP：可空类型
来源：http://wu.huanxung.cn

?string $name = null
来源：http://zm.shxzukj.cn

[U47] PHP：联合类型
来源：http://nm.nszjky.cn

int|string $id
来源：http://jv.huanxung.cn

[U48] PHP：纯枚举
来源：http://rt.jctech888.com.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xs.nicolike.cn

[U49] PHP：只读属性
来源：http://wr.szsharing.cn

public readonly string $name
来源：http://yl.bjjhwx.cn

[U50] PHP：构造器属性提升
来源：http://yj.colortex.cn

public function __construct(private int $id) {}
来源：http://rr.huanxung.cn

[U51] PHP：数组解构
来源：http://ye.hahajie.cn

[$a, $b] = $arr;
来源：http://vk.asd995.cn

[U52] PHP：箭头函数
来源：http://ca.shxzskj.cn

$double = fn($x) => $x * 2;
来源：http://mv.wgjwhj.cn

[U53] PHP：空合并运算符
来源：http://vt.panjiajie.cn

$v = $a ?? $b ?? "default";
来源：http://cs.nszjky.cn

[U54] PHP：空安全调用
来源：http://ah.gzmigu.cn

$obj?->method()
来源：http://xe.newstarts.cn

[U55] PHP：match 表达式
来源：http://qg.shxzskj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://em.9csxet.cn

[U56] PHP：命名参数
来源：http://uj.jctech888.com.cn

f(a: 1, b: 2)
来源：http://ll.jctech888.com.cn

[U57] PHP：字符串插值
来源：http://ss.yuexingan06.cn

"值: {$a}"
来源：http://xs.nszjky.cn

[U58] PHP：数组三件套
来源：http://vs.bookmarksfly.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://sy.huixiangedu.cn

[U59] PHP：自定义排序
来源：http://ha.panjiajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fl.panjiajie.cn

[U60] PHP：JSON 编解码
来源：http://jw.colortex.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qo.lnxyls.cn

[U61] PHP：正则
来源：http://qz.yuntaijiaju.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://du.szxytkj.cn

[U62] PHP：日期对象
来源：http://ip.shtwfgs.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zh.yuntaijiaju.cn

[U63] PHP：文件读写
来源：http://ox.nicolike.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hj.wgjwhj.cn

[U64] PHP：目录遍历
来源：http://zd.huanxung.cn

glob("dir/*.php");  scandir("dir");
来源：http://zm.huanxung.cn

[U65] PHP：会话
来源：http://az.shxzukj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://qk.nicolike.cn

[U66] PHP：设置 Cookie
来源：http://xb.gzmigu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bq.huixinmuqiang.cn

[U67] PHP：处理文件上传
来源：http://it.bjjhwx.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fj.bjjhwx.cn

[U68] PHP：PDO 连接
来源：http://bj.huixiangedu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ag.nszjky.cn

[U69] PHP：PDO 预处理
来源：http://wf.szsharing.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ts.hnjuh.cn

[U70] PHP：PDO 事务
来源：http://ox.wgjwhj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ps.hahajie.cn

[U71] PHP：抛出异常
来源：http://rr.gzmigu.cn

throw new RuntimeException("失败", 500);
来源：http://ia.newstarts.cn

[U72] PHP：写错误日志
来源：http://ea.yuexingan06.cn

error_log("失败: " . $e->getMessage());
来源：http://ot.haigaiapp.cn

[U73] PHP：读取 ini 配置
来源：http://rj.panjiajie.cn

parse_ini_file("config.ini", true)
来源：http://br.haigaiapp.cn

[U74] PHP：读取环境变量
来源：http://xx.hahajie.cn

getenv("APP_ENV") ?: "production"
来源：http://lf.huixiangedu.cn

[U75] PHP：依赖注入
来源：http://qj.yuexingan06.cn

composer require psr/container
来源：http://wh.9csxet.cn

[U76] PHP：简单路由
来源：http://wp.huixiangedu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gi.yuexingan06.cn

[U77] PHP：模板渲染
来源：http://hs.shtwfgs.cn

composer require twig/twig
来源：http://yt.huixiangedu.cn

[U78] PHP：单元测试
来源：http://dp.hnjuh.cn

composer require --dev phpunit/phpunit
来源：http://xg.nszjky.cn

[U79] PHP：静态分析
来源：http://tq.gzmigu.cn

composer require --dev phpstan/phpstan
来源：http://zw.gzmigu.cn

[U80] PHP：代码规范修复
来源：http://zz.bookmarksfly.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://mm.lnxyls.cn

[U81] JS：初始化项目
来源：http://ez.wgjwhj.cn

npm init -y;  npm i express
来源：http://cn.szsharing.cn

[U82] JS：package.json 脚本
来源：http://pg.bookmarksfly.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tv.shxzskj.cn

[U83] JS：ES Module 导入导出
来源：http://bw.asd995.cn

export const a = 1;  import { a } from "./m.js";
来源：http://da.hahajie.cn

[U84] JS：CommonJS 写法
来源：http://xj.newstarts.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ca.shtwfgs.cn

[U85] JS：可选链
来源：http://nx.asd995.cn

a?.b?.c
来源：http://om.shtwfgs.cn

[U86] JS：空值合并
来源：http://df.huixinmuqiang.cn

a ?? b
来源：http://zg.nicolike.cn

[U87] JS：解构默认值
来源：http://vs.huixinmuqiang.cn

const { a = 1, b = 2 } = obj;
来源：http://sq.jianghongdianzi.cn

[U88] JS：对象展开合并
来源：http://eu.521024.cn

{ ...a, ...b }
来源：http://hr.yuntaijiaju.cn

[U89] JS：数组去重
来源：http://mt.bookmarksfly.cn

[...new Set(arr)]
来源：http://rw.yuntaijiaju.cn

[U90] JS：数字数组排序
来源：http://pj.nicolike.cn

[...arr].sort((a, b) => a - b)
来源：http://ue.szxytkj.cn

[U91] JS：对象键值遍历
来源：http://kl.asd995.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://an.jianghongdianzi.cn

[U92] JS：深拷贝
来源：http://is.nszjky.cn

structuredClone(obj)
来源：http://pm.chemitech.net.cn

[U93] JS：模板字符串
来源：http://br.9csxet.cn

`共 ${n} 条`
来源：http://us.huanxung.cn

[U94] JS：箭头函数
来源：http://tq.lnxyls.cn

const double = x => x * 2;
来源：http://vm.colortex.cn

[U95] JS：Promise 包装
来源：http://ne.yuexingan06.cn

new Promise((resolve, reject) => {})
来源：http://if.lnxyls.cn

[U96] JS：async/await 与异常
来源：http://pe.nicolike.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jd.panjiajie.cn

[U97] JS：并发请求
来源：http://qs.bjjhwx.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ml.bjjhwx.cn

[U98] JS：fetch 带 JSON
来源：http://mc.gzmigu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://sd.huixiangedu.cn

[U99] JS：事件监听
来源：http://wh.shxzukj.cn

el.addEventListener("click", e => {})
来源：http://rj.yuntaijiaju.cn

[U100] JS：DOM 查询
来源：http://tm.huixinmuqiang.cn

document.querySelector(".item")
来源：http://oa.lnxyls.cn

[U101] JS：classList 操作
来源：http://fk.lnxyls.cn

el.classList.toggle("active")
来源：http://sp.asd995.cn

[U102] JS：本地存储
来源：http://ji.shxzukj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://dq.shxzskj.cn

[U103] JS：定时器
来源：http://ms.9csxet.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wh.huixinmuqiang.cn

[U104] JS：防抖
来源：http://rd.9csxet.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cf.jctech888.com.cn

[U105] JS：节流
来源：http://bt.panjiajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wu.lnxyls.cn

[U106] JS：日期格式化
来源：http://rx.hahajie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cr.bjjhwx.cn

[U107] JS：数字千分位
来源：http://qn.newstarts.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://az.gzmigu.cn

[U108] JS：随机整数
来源：http://sz.yuexingan06.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wf.yuexingan06.cn

[U109] JS：数组分组
来源：http://xq.colortex.cn

Object.groupBy(arr, x => x.type)
来源：http://uf.newstarts.cn

[U110] JS：数组分块
来源：http://so.jctech888.com.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bc.shxzukj.cn

[U111] JS：对象转 Map
来源：http://cu.shtwfgs.cn

new Map(Object.entries(obj))
来源：http://qj.yuexingan06.cn

[U112] JS：字符串补位
来源：http://cl.yuexingan06.cn

"7".padStart(3, "0")
来源：http://ka.huixinmuqiang.cn

[U113] JS：正则替换全部
来源：http://hi.muxihuayi.cn

s.replaceAll("a", "b")
来源：http://nc.huixiangedu.cn

[U114] JS：JSON 深比较
来源：http://re.nicolike.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://yd.wgjwhj.cn

[U115] JS：生成 UUID
来源：http://tu.wgjwhj.cn

crypto.randomUUID()
来源：http://ye.colortex.cn

[U116] JS：类型检查（JSDoc）
来源：http://qz.bjjhwx.cn

/** @param {string} name */ function f(name) {}
来源：http://sh.huixinmuqiang.cn

[U117] JS：单元测试
来源：http://ol.jianghongdianzi.cn

npm i -D vitest;  npx vitest
来源：http://fu.szxytkj.cn

[U118] JS：开发服务器
来源：http://ju.szsharing.cn

npm i -D vite;  npx vite
来源：http://az.muxihuayi.cn

[U119] JS：生产构建
来源：http://zk.haigaiapp.cn

npx vite build
来源：http://ho.gzmigu.cn

[U120] JS：读取环境变量（Vite）
来源：http://gl.521024.cn

import.meta.env.VITE_API_URL
来源：http://tm.shtwfgs.cn

================================================================================
来源：http://mn.wgjwhj.cn

统计汇总
来源：http://pa.colortex.cn

================================================================================
来源：http://nn.nicolike.cn

按语言统计（条）：
来源：http://el.newstarts.cn

Python ......... 252
来源：http://gi.huixinmuqiang.cn

PHP ............ 252
来源：http://tf.jctech888.com.cn

JavaScript ..... 252
来源：http://bg.hahajie.cn

TypeScript ..... 212
来源：http://mr.szxytkj.cn

Java ........... 212
来源：http://ml.yuntaijiaju.cn

Go ............. 212
来源：http://iy.muxihuayi.cn

Ruby ........... 212
来源：http://bm.shxzukj.cn

C# ............. 212
来源：http://zl.yuntaijiaju.cn

C .............. 30
来源：http://ze.yuntaijiaju.cn

C++ ............ 30
来源：http://rb.newstarts.cn

SQL ............ 90
来源：http://pz.panjiajie.cn

Bash ........... 80
来源：http://hh.szxytkj.cn

Kotlin ......... 15
来源：http://rs.gzmigu.cn

Swift .......... 15
来源：http://as.hnjuh.cn

Lua ............ 10
来源：http://wd.yuntaijiaju.cn

Perl ........... 10
来源：http://ed.bjjhwx.cn

Scala .......... 10
来源：http://wp.muxihuayi.cn

------------------------------------
来源：http://tq.gzmigu.cn

合计 ........... 2106 条
来源：http://lq.yuexingan06.cn

按章节统计：
来源：http://wl.huixiangedu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qt.haigaiapp.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://sa.yuexingan06.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nq.huixiangedu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ax.hahajie.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ti.huixinmuqiang.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nb.yuntaijiaju.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://eq.hahajie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ro.huanxung.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pd.huixinmuqiang.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ny.shxzskj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ys.bjjhwx.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kt.szxytkj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://az.szsharing.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lo.jianghongdianzi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rt.huixiangedu.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gb.9csxet.cn

Q SQL 专题                              90
来源：http://az.9csxet.cn

R Bash 专题                             80
来源：http://oz.nszjky.cn

S C / C++ 专题                          60
来源：http://qz.nicolike.cn

T 其他语言补充                          60
来源：http://pv.huanxung.cn

U 高频实用片段                         120
来源：http://vb.jianghongdianzi.cn

------------------------------------
来源：http://kk.chemitech.net.cn

合计                                  2106 条
来源：http://yd.521024.cn

--------------------------------------------------------------------------------
来源：http://yg.nszjky.cn

使用提醒
来源：http://po.nszjky.cn

--------------------------------------------------------------------------------
来源：http://uj.bjjhwx.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://av.yuntaijiaju.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jq.hahajie.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lc.hnjuh.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://fu.chemitech.net.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kz.haigaiapp.cn

—— 文件结束 ——
来源：http://yc.colortex.cn

================================================================================
来源：http://xi.colortex.cn

程序语言常见例子速查手册（2024 版）
来源：http://ro.haigaiapp.cn

Common Programming Examples Cheat Book
来源：http://oc.yuntaijiaju.cn

================================================================================
来源：http://au.szxytkj.cn

【收录内容】
来源：http://hv.jianghongdianzi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://tj.huanxung.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://kb.yuntaijiaju.cn

SQL · Bash · C · C++
来源：http://ww.haigaiapp.cn


<!-- 参考信息 -->