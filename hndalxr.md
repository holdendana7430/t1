代发 wailian999

[U01] Py：创建虚拟环境
来源：http://yx.hahajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ww.newstarts.cn

[U02] Py：导出 / 安装依赖
来源：http://lg.haigaiapp.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ve.asd995.cn

[U03] Py：加载 .env 配置
来源：http://la.muxihuayi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wn.jianghongdianzi.cn

[U04] Py：变量调试打印
来源：http://kw.nszjky.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ee.hahajie.cn

[U05] Py：列表去重且保序
来源：http://sv.huixiangedu.cn

list(dict.fromkeys(arr))
来源：http://bq.chemitech.net.cn

[U06] Py：合并两个字典
来源：http://lq.hahajie.cn

{**a, **b}
来源：http://oh.hnjuh.cn

[U07] Py：反转字典键值
来源：http://zu.colortex.cn

{v: k for k, v in d.items()}
来源：http://wp.panjiajie.cn

[U08] Py：展平二维列表
来源：http://zy.szsharing.cn

[y for x in nested for y in x]
来源：http://cd.panjiajie.cn

[U09] Py：字典取最大值的键
来源：http://xt.hnjuh.cn

max(d, key=d.get)
来源：http://br.yuntaijiaju.cn

[U10] Py：按值排序字典
来源：http://wg.szsharing.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lq.nicolike.cn

[U11] Py：生成器表达式
来源：http://so.colortex.cn

(x * 2 for x in arr)
来源：http://uz.panjiajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://fc.huanxung.cn

Counter(arr).most_common(3)
来源：http://bb.shxzukj.cn

[U13] Py：固定长度队列
来源：http://hv.nszjky.cn

deque(maxlen=10)
来源：http://rm.521024.cn

[U14] Py：分组收集到列表
来源：http://ep.jianghongdianzi.cn

defaultdict(list)
来源：http://nc.colortex.cn

[U15] Py：高精度计时
来源：http://hu.huixinmuqiang.cn

t = time.perf_counter()
来源：http://vp.jianghongdianzi.cn

[U16] Py：命令行参数解析
来源：http://gn.9csxet.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xt.bjjhwx.cn

[U17] Py：初始化日志
来源：http://xh.nicolike.cn

logging.basicConfig(level=logging.INFO)
来源：http://ra.wgjwhj.cn

[U18] Py：预编译正则
来源：http://nx.colortex.cn

pat = re.compile(r"\d+")
来源：http://zn.nszjky.cn

[U19] Py：正则替换带回调
来源：http://qm.shtwfgs.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dh.shxzskj.cn

[U20] Py：缓存函数结果
来源：http://gr.bookmarksfly.cn

@functools.lru_cache(maxsize=None)
来源：http://fj.wgjwhj.cn

[U21] Py：自定义上下文管理器
来源：http://ac.bookmarksfly.cn

@contextlib.contextmanager
来源：http://wx.nicolike.cn

[U22] Py：矩阵转置
来源：http://jw.szxytkj.cn

list(zip(*m))
来源：http://jj.haigaiapp.cn

[U23] Py：分块读取大文件
来源：http://cx.wgjwhj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qy.lnxyls.cn

[U24] Py：路径操作
来源：http://yi.nicolike.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mt.yuexingan06.cn

[U25] Py：CSV 按字典读
来源：http://kf.bjjhwx.cn

csv.DictReader(f)
来源：http://kf.gzmigu.cn

[U26] Py：并发下载
来源：http://al.bookmarksfly.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://id.huanxung.cn

[U27] Py：异步 HTTP
来源：http://xz.haigaiapp.cn

aiohttp.ClientSession() 配合 async with
来源：http://zg.9csxet.cn

[U28] Py：类型别名
来源：http://hq.jianghongdianzi.cn

UserId = int
来源：http://sa.shxzukj.cn

[U29] Py：属性校验
来源：http://jj.asd995.cn

@property 与 @x.setter 配合
来源：http://dy.nszjky.cn

[U30] Py：数据类
来源：http://br.haigaiapp.cn

@dataclass(slots=True)
来源：http://fs.huixiangedu.cn

[U31] Py：单测
来源：http://zp.nicolike.cn

python -m pytest -q
来源：http://js.newstarts.cn

[U32] Py：代码格式化
来源：http://gg.nszjky.cn

ruff format . && ruff check --fix .
来源：http://vw.nicolike.cn

[U33] Py：打包发布
来源：http://ik.jctech888.com.cn

python -m build  （依赖 pyproject.toml）
来源：http://jg.lnxyls.cn

[U34] Py：判断编码
来源：http://vl.asd995.cn

chardet.detect(raw)
来源：http://hd.huixinmuqiang.cn

[U35] Py：发送邮件
来源：http://ps.szxytkj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pd.shtwfgs.cn

[U36] Py：定时任务
来源：http://uh.jctech888.com.cn

schedule.every(10).minutes.do(job)
来源：http://ql.521024.cn

[U37] Py：读写 Excel
来源：http://zw.yuntaijiaju.cn

pandas.read_excel / DataFrame.to_excel
来源：http://tc.shxzskj.cn

[U38] Py：获取脚本所在目录
来源：http://hk.9csxet.cn

Path(__file__).resolve().parent
来源：http://dz.nicolike.cn

[U39] Py：判断是否在交互环境
来源：http://mv.szsharing.cn

sys.stdout.isatty()
来源：http://un.huixiangedu.cn

[U40] Py：打印到标准错误
来源：http://qs.asd995.cn

print("err", file=sys.stderr)
来源：http://ep.shtwfgs.cn

[U41] PHP：初始化 Composer 项目
来源：http://ys.521024.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://bh.yuntaijiaju.cn

[U42] PHP：PSR-4 自动加载
来源：http://vw.szsharing.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lc.szsharing.cn

[U43] PHP：声明命名空间
来源：http://et.nszjky.cn

namespace App\Http;
来源：http://cz.hahajie.cn

[U44] PHP：开启严格类型
来源：http://oo.haigaiapp.cn

declare(strict_types=1);
来源：http://co.wgjwhj.cn

[U45] PHP：类型声明与返回类型
来源：http://fe.shtwfgs.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ac.521024.cn

[U46] PHP：可空类型
来源：http://on.panjiajie.cn

?string $name = null
来源：http://by.nicolike.cn

[U47] PHP：联合类型
来源：http://pt.bjjhwx.cn

int|string $id
来源：http://mm.9csxet.cn

[U48] PHP：纯枚举
来源：http://cb.yuexingan06.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zp.shxzukj.cn

[U49] PHP：只读属性
来源：http://sv.lnxyls.cn

public readonly string $name
来源：http://fm.bjjhwx.cn

[U50] PHP：构造器属性提升
来源：http://iq.shtwfgs.cn

public function __construct(private int $id) {}
来源：http://qf.asd995.cn

[U51] PHP：数组解构
来源：http://wj.muxihuayi.cn

[$a, $b] = $arr;
来源：http://yt.shxzskj.cn

[U52] PHP：箭头函数
来源：http://uo.panjiajie.cn

$double = fn($x) => $x * 2;
来源：http://ah.9csxet.cn

[U53] PHP：空合并运算符
来源：http://dt.muxihuayi.cn

$v = $a ?? $b ?? "default";
来源：http://wf.huixinmuqiang.cn

[U54] PHP：空安全调用
来源：http://qx.huanxung.cn

$obj?->method()
来源：http://rb.colortex.cn

[U55] PHP：match 表达式
来源：http://it.wgjwhj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kn.wgjwhj.cn

[U56] PHP：命名参数
来源：http://jm.panjiajie.cn

f(a: 1, b: 2)
来源：http://zq.szxytkj.cn

[U57] PHP：字符串插值
来源：http://os.lnxyls.cn

"值: {$a}"
来源：http://ks.newstarts.cn

[U58] PHP：数组三件套
来源：http://ot.bjjhwx.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://dd.hnjuh.cn

[U59] PHP：自定义排序
来源：http://vm.huanxung.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wr.nszjky.cn

[U60] PHP：JSON 编解码
来源：http://no.hahajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://df.szsharing.cn

[U61] PHP：正则
来源：http://zo.9csxet.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kd.colortex.cn

[U62] PHP：日期对象
来源：http://tf.bookmarksfly.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rd.gzmigu.cn

[U63] PHP：文件读写
来源：http://te.szxytkj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ay.shxzukj.cn

[U64] PHP：目录遍历
来源：http://la.szsharing.cn

glob("dir/*.php");  scandir("dir");
来源：http://oo.jianghongdianzi.cn

[U65] PHP：会话
来源：http://my.hahajie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://gb.gzmigu.cn

[U66] PHP：设置 Cookie
来源：http://lt.panjiajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ga.muxihuayi.cn

[U67] PHP：处理文件上传
来源：http://pn.haigaiapp.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://uo.wgjwhj.cn

[U68] PHP：PDO 连接
来源：http://zr.9csxet.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dj.hahajie.cn

[U69] PHP：PDO 预处理
来源：http://cf.nszjky.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kl.yuexingan06.cn

[U70] PHP：PDO 事务
来源：http://gl.9csxet.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xu.panjiajie.cn

[U71] PHP：抛出异常
来源：http://qz.asd995.cn

throw new RuntimeException("失败", 500);
来源：http://lt.shxzskj.cn

[U72] PHP：写错误日志
来源：http://ey.nszjky.cn

error_log("失败: " . $e->getMessage());
来源：http://lb.newstarts.cn

[U73] PHP：读取 ini 配置
来源：http://ub.muxihuayi.cn

parse_ini_file("config.ini", true)
来源：http://zv.szxytkj.cn

[U74] PHP：读取环境变量
来源：http://ox.jctech888.com.cn

getenv("APP_ENV") ?: "production"
来源：http://ib.jctech888.com.cn

[U75] PHP：依赖注入
来源：http://lz.nicolike.cn

composer require psr/container
来源：http://kg.nszjky.cn

[U76] PHP：简单路由
来源：http://gj.bjjhwx.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tg.shxzskj.cn

[U77] PHP：模板渲染
来源：http://cq.szsharing.cn

composer require twig/twig
来源：http://mu.521024.cn

[U78] PHP：单元测试
来源：http://wa.hahajie.cn

composer require --dev phpunit/phpunit
来源：http://ik.haigaiapp.cn

[U79] PHP：静态分析
来源：http://ae.nicolike.cn

composer require --dev phpstan/phpstan
来源：http://zj.jianghongdianzi.cn

[U80] PHP：代码规范修复
来源：http://ld.hnjuh.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://yt.wgjwhj.cn

[U81] JS：初始化项目
来源：http://fu.huixinmuqiang.cn

npm init -y;  npm i express
来源：http://wj.gzmigu.cn

[U82] JS：package.json 脚本
来源：http://tb.hnjuh.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qj.yuntaijiaju.cn

[U83] JS：ES Module 导入导出
来源：http://jr.szxytkj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://le.muxihuayi.cn

[U84] JS：CommonJS 写法
来源：http://qd.yuexingan06.cn

module.exports = { a };  const { a } = require("./m");
来源：http://st.asd995.cn

[U85] JS：可选链
来源：http://mu.yuntaijiaju.cn

a?.b?.c
来源：http://gk.huixiangedu.cn

[U86] JS：空值合并
来源：http://ue.szxytkj.cn

a ?? b
来源：http://rs.wgjwhj.cn

[U87] JS：解构默认值
来源：http://bx.nszjky.cn

const { a = 1, b = 2 } = obj;
来源：http://ir.hnjuh.cn

[U88] JS：对象展开合并
来源：http://ut.hahajie.cn

{ ...a, ...b }
来源：http://kw.newstarts.cn

[U89] JS：数组去重
来源：http://eo.panjiajie.cn

[...new Set(arr)]
来源：http://gh.panjiajie.cn

[U90] JS：数字数组排序
来源：http://yi.haigaiapp.cn

[...arr].sort((a, b) => a - b)
来源：http://mu.shxzskj.cn

[U91] JS：对象键值遍历
来源：http://mg.muxihuayi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ow.yuexingan06.cn

[U92] JS：深拷贝
来源：http://vf.huanxung.cn

structuredClone(obj)
来源：http://xr.9csxet.cn

[U93] JS：模板字符串
来源：http://ip.hahajie.cn

`共 ${n} 条`
来源：http://cb.nicolike.cn

[U94] JS：箭头函数
来源：http://ml.shxzskj.cn

const double = x => x * 2;
来源：http://om.shxzskj.cn

[U95] JS：Promise 包装
来源：http://qr.newstarts.cn

new Promise((resolve, reject) => {})
来源：http://xj.newstarts.cn

[U96] JS：async/await 与异常
来源：http://kq.jianghongdianzi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pf.asd995.cn

[U97] JS：并发请求
来源：http://ba.9csxet.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://no.colortex.cn

[U98] JS：fetch 带 JSON
来源：http://gj.chemitech.net.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qk.panjiajie.cn

[U99] JS：事件监听
来源：http://rh.yuexingan06.cn

el.addEventListener("click", e => {})
来源：http://pq.jctech888.com.cn

[U100] JS：DOM 查询
来源：http://aj.muxihuayi.cn

document.querySelector(".item")
来源：http://fi.haigaiapp.cn

[U101] JS：classList 操作
来源：http://uo.521024.cn

el.classList.toggle("active")
来源：http://lm.lnxyls.cn

[U102] JS：本地存储
来源：http://ip.bookmarksfly.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://tf.szxytkj.cn

[U103] JS：定时器
来源：http://tz.newstarts.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wx.bookmarksfly.cn

[U104] JS：防抖
来源：http://xc.hahajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wk.newstarts.cn

[U105] JS：节流
来源：http://ne.asd995.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://az.huixinmuqiang.cn

[U106] JS：日期格式化
来源：http://dq.huixinmuqiang.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jt.chemitech.net.cn

[U107] JS：数字千分位
来源：http://ty.asd995.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gs.521024.cn

[U108] JS：随机整数
来源：http://at.yuntaijiaju.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qe.haigaiapp.cn

[U109] JS：数组分组
来源：http://jm.newstarts.cn

Object.groupBy(arr, x => x.type)
来源：http://ki.huixiangedu.cn

[U110] JS：数组分块
来源：http://fc.hnjuh.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mw.jctech888.com.cn

[U111] JS：对象转 Map
来源：http://uu.bjjhwx.cn

new Map(Object.entries(obj))
来源：http://zk.panjiajie.cn

[U112] JS：字符串补位
来源：http://tg.bjjhwx.cn

"7".padStart(3, "0")
来源：http://va.asd995.cn

[U113] JS：正则替换全部
来源：http://ai.lnxyls.cn

s.replaceAll("a", "b")
来源：http://zh.hahajie.cn

[U114] JS：JSON 深比较
来源：http://gr.9csxet.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ty.shxzukj.cn

[U115] JS：生成 UUID
来源：http://uu.nicolike.cn

crypto.randomUUID()
来源：http://dd.shxzskj.cn

[U116] JS：类型检查（JSDoc）
来源：http://tt.muxihuayi.cn

/** @param {string} name */ function f(name) {}
来源：http://tb.521024.cn

[U117] JS：单元测试
来源：http://rj.chemitech.net.cn

npm i -D vitest;  npx vitest
来源：http://du.lnxyls.cn

[U118] JS：开发服务器
来源：http://rl.9csxet.cn

npm i -D vite;  npx vite
来源：http://ao.shtwfgs.cn

[U119] JS：生产构建
来源：http://pq.shtwfgs.cn

npx vite build
来源：http://ze.huixinmuqiang.cn

[U120] JS：读取环境变量（Vite）
来源：http://fs.panjiajie.cn

import.meta.env.VITE_API_URL
来源：http://ec.colortex.cn

================================================================================
来源：http://en.huixinmuqiang.cn

统计汇总
来源：http://pu.521024.cn

================================================================================
来源：http://vk.521024.cn

按语言统计（条）：
来源：http://rr.gzmigu.cn

Python ......... 252
来源：http://in.szxytkj.cn

PHP ............ 252
来源：http://mq.gzmigu.cn

JavaScript ..... 252
来源：http://dt.panjiajie.cn

TypeScript ..... 212
来源：http://wc.nicolike.cn

Java ........... 212
来源：http://an.shxzskj.cn

Go ............. 212
来源：http://bl.chemitech.net.cn

Ruby ........... 212
来源：http://bv.panjiajie.cn

C# ............. 212
来源：http://bj.nszjky.cn

C .............. 30
来源：http://gd.gzmigu.cn

C++ ............ 30
来源：http://qq.521024.cn

SQL ............ 90
来源：http://sz.shxzskj.cn

Bash ........... 80
来源：http://gj.hahajie.cn

Kotlin ......... 15
来源：http://qh.jctech888.com.cn

Swift .......... 15
来源：http://vy.gzmigu.cn

Lua ............ 10
来源：http://jp.huixiangedu.cn

Perl ........... 10
来源：http://gt.gzmigu.cn

Scala .......... 10
来源：http://uz.szxytkj.cn

------------------------------------
来源：http://qs.szxytkj.cn

合计 ........... 2106 条
来源：http://tw.nicolike.cn

按章节统计：
来源：http://xh.wgjwhj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ml.nszjky.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pv.hahajie.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lb.jianghongdianzi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kb.bookmarksfly.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ak.shxzukj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ey.9csxet.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qx.muxihuayi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pq.nicolike.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://la.shxzukj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ys.shtwfgs.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jq.wgjwhj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://uk.hahajie.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xr.szxytkj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sy.yuexingan06.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vo.shxzukj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ck.shxzskj.cn

Q SQL 专题                              90
来源：http://wo.hnjuh.cn

R Bash 专题                             80
来源：http://hy.521024.cn

S C / C++ 专题                          60
来源：http://tm.huixiangedu.cn

T 其他语言补充                          60
来源：http://oc.haigaiapp.cn

U 高频实用片段                         120
来源：http://yj.newstarts.cn

------------------------------------
来源：http://yh.muxihuayi.cn

合计                                  2106 条
来源：http://km.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://iu.shtwfgs.cn

使用提醒
来源：http://wk.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://fr.jianghongdianzi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nu.yuntaijiaju.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xz.521024.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bo.wgjwhj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://rg.shtwfgs.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jk.colortex.cn

—— 文件结束 ——
来源：http://rj.9csxet.cn

================================================================================
来源：http://ys.haigaiapp.cn

程序语言常见例子速查手册（2024 版）
来源：http://yr.chemitech.net.cn

Common Programming Examples Cheat Book
来源：http://ry.shxzskj.cn

================================================================================
来源：http://el.bjjhwx.cn


<!-- 参考信息 -->