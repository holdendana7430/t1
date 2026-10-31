代发 wailian999

[U01] Py：创建虚拟环境
来源：http://mk.colortex.cn

python -m venv .venv && source .venv/bin/activate
来源：http://es.shxzukj.cn

[U02] Py：导出 / 安装依赖
来源：http://du.521024.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fc.panjiajie.cn

[U03] Py：加载 .env 配置
来源：http://gd.haigaiapp.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ut.chemitech.net.cn

[U04] Py：变量调试打印
来源：http://th.gzmigu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gr.bookmarksfly.cn

[U05] Py：列表去重且保序
来源：http://jd.huixinmuqiang.cn

list(dict.fromkeys(arr))
来源：http://sw.521024.cn

[U06] Py：合并两个字典
来源：http://ey.haigaiapp.cn

{**a, **b}
来源：http://jy.yuexingan06.cn

[U07] Py：反转字典键值
来源：http://ss.colortex.cn

{v: k for k, v in d.items()}
来源：http://jr.bjjhwx.cn

[U08] Py：展平二维列表
来源：http://fd.521024.cn

[y for x in nested for y in x]
来源：http://zr.bjjhwx.cn

[U09] Py：字典取最大值的键
来源：http://wm.shxzukj.cn

max(d, key=d.get)
来源：http://qt.nicolike.cn

[U10] Py：按值排序字典
来源：http://ko.jianghongdianzi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pe.haigaiapp.cn

[U11] Py：生成器表达式
来源：http://mh.hahajie.cn

(x * 2 for x in arr)
来源：http://qt.chemitech.net.cn

[U12] Py：取出现最多的 3 个元素
来源：http://cm.hnjuh.cn

Counter(arr).most_common(3)
来源：http://uf.gzmigu.cn

[U13] Py：固定长度队列
来源：http://ks.haigaiapp.cn

deque(maxlen=10)
来源：http://jy.9csxet.cn

[U14] Py：分组收集到列表
来源：http://rj.yuntaijiaju.cn

defaultdict(list)
来源：http://ur.gzmigu.cn

[U15] Py：高精度计时
来源：http://ux.jctech888.com.cn

t = time.perf_counter()
来源：http://tt.huixiangedu.cn

[U16] Py：命令行参数解析
来源：http://qw.bookmarksfly.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gv.nszjky.cn

[U17] Py：初始化日志
来源：http://uz.jianghongdianzi.cn

logging.basicConfig(level=logging.INFO)
来源：http://sa.hahajie.cn

[U18] Py：预编译正则
来源：http://tu.bookmarksfly.cn

pat = re.compile(r"\d+")
来源：http://tz.9csxet.cn

[U19] Py：正则替换带回调
来源：http://ni.szxytkj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hd.jianghongdianzi.cn

[U20] Py：缓存函数结果
来源：http://ny.shtwfgs.cn

@functools.lru_cache(maxsize=None)
来源：http://no.lnxyls.cn

[U21] Py：自定义上下文管理器
来源：http://pl.bookmarksfly.cn

@contextlib.contextmanager
来源：http://la.lnxyls.cn

[U22] Py：矩阵转置
来源：http://yt.nicolike.cn

list(zip(*m))
来源：http://xy.huanxung.cn

[U23] Py：分块读取大文件
来源：http://wf.asd995.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yt.yuntaijiaju.cn

[U24] Py：路径操作
来源：http://gz.yuexingan06.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://uj.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://jw.colortex.cn

csv.DictReader(f)
来源：http://ok.bjjhwx.cn

[U26] Py：并发下载
来源：http://oy.lnxyls.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tq.bjjhwx.cn

[U27] Py：异步 HTTP
来源：http://ef.newstarts.cn

aiohttp.ClientSession() 配合 async with
来源：http://gc.panjiajie.cn

[U28] Py：类型别名
来源：http://vg.gzmigu.cn

UserId = int
来源：http://tm.chemitech.net.cn

[U29] Py：属性校验
来源：http://ub.huixiangedu.cn

@property 与 @x.setter 配合
来源：http://hg.gzmigu.cn

[U30] Py：数据类
来源：http://ce.yuntaijiaju.cn

@dataclass(slots=True)
来源：http://bg.shtwfgs.cn

[U31] Py：单测
来源：http://ey.521024.cn

python -m pytest -q
来源：http://wp.shtwfgs.cn

[U32] Py：代码格式化
来源：http://wp.hahajie.cn

ruff format . && ruff check --fix .
来源：http://jz.hnjuh.cn

[U33] Py：打包发布
来源：http://np.shtwfgs.cn

python -m build  （依赖 pyproject.toml）
来源：http://xh.gzmigu.cn

[U34] Py：判断编码
来源：http://xs.9csxet.cn

chardet.detect(raw)
来源：http://gj.huanxung.cn

[U35] Py：发送邮件
来源：http://po.jianghongdianzi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ud.panjiajie.cn

[U36] Py：定时任务
来源：http://nz.yuexingan06.cn

schedule.every(10).minutes.do(job)
来源：http://um.wgjwhj.cn

[U37] Py：读写 Excel
来源：http://in.bjjhwx.cn

pandas.read_excel / DataFrame.to_excel
来源：http://pu.yuntaijiaju.cn

[U38] Py：获取脚本所在目录
来源：http://kl.szxytkj.cn

Path(__file__).resolve().parent
来源：http://mx.shxzskj.cn

[U39] Py：判断是否在交互环境
来源：http://lh.lnxyls.cn

sys.stdout.isatty()
来源：http://mh.gzmigu.cn

[U40] Py：打印到标准错误
来源：http://oh.shtwfgs.cn

print("err", file=sys.stderr)
来源：http://os.shxzskj.cn

[U41] PHP：初始化 Composer 项目
来源：http://pt.yuexingan06.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://lz.hahajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://ph.szxytkj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gy.yuexingan06.cn

[U43] PHP：声明命名空间
来源：http://we.panjiajie.cn

namespace App\Http;
来源：http://te.haigaiapp.cn

[U44] PHP：开启严格类型
来源：http://zh.colortex.cn

declare(strict_types=1);
来源：http://zo.lnxyls.cn

[U45] PHP：类型声明与返回类型
来源：http://ss.bookmarksfly.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bp.huixiangedu.cn

[U46] PHP：可空类型
来源：http://pt.huixiangedu.cn

?string $name = null
来源：http://px.huixiangedu.cn

[U47] PHP：联合类型
来源：http://wf.newstarts.cn

int|string $id
来源：http://xb.wgjwhj.cn

[U48] PHP：纯枚举
来源：http://sc.gzmigu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lf.nszjky.cn

[U49] PHP：只读属性
来源：http://vi.bjjhwx.cn

public readonly string $name
来源：http://kj.muxihuayi.cn

[U50] PHP：构造器属性提升
来源：http://dp.jianghongdianzi.cn

public function __construct(private int $id) {}
来源：http://cb.muxihuayi.cn

[U51] PHP：数组解构
来源：http://ge.huanxung.cn

[$a, $b] = $arr;
来源：http://dd.muxihuayi.cn

[U52] PHP：箭头函数
来源：http://zt.wgjwhj.cn

$double = fn($x) => $x * 2;
来源：http://fc.yuexingan06.cn

[U53] PHP：空合并运算符
来源：http://ze.newstarts.cn

$v = $a ?? $b ?? "default";
来源：http://tj.nszjky.cn

[U54] PHP：空安全调用
来源：http://nc.yuntaijiaju.cn

$obj?->method()
来源：http://sr.wgjwhj.cn

[U55] PHP：match 表达式
来源：http://ux.hnjuh.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ly.jianghongdianzi.cn

[U56] PHP：命名参数
来源：http://fh.newstarts.cn

f(a: 1, b: 2)
来源：http://ad.yuntaijiaju.cn

[U57] PHP：字符串插值
来源：http://fu.yuntaijiaju.cn

"值: {$a}"
来源：http://xq.nszjky.cn

[U58] PHP：数组三件套
来源：http://zy.huixinmuqiang.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mk.shxzskj.cn

[U59] PHP：自定义排序
来源：http://xa.9csxet.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qj.haigaiapp.cn

[U60] PHP：JSON 编解码
来源：http://jy.huixiangedu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dj.nszjky.cn

[U61] PHP：正则
来源：http://wk.nicolike.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fv.szxytkj.cn

[U62] PHP：日期对象
来源：http://fp.9csxet.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vu.szxytkj.cn

[U63] PHP：文件读写
来源：http://vt.nicolike.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wn.wgjwhj.cn

[U64] PHP：目录遍历
来源：http://bb.asd995.cn

glob("dir/*.php");  scandir("dir");
来源：http://mq.panjiajie.cn

[U65] PHP：会话
来源：http://gc.haigaiapp.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://gr.szxytkj.cn

[U66] PHP：设置 Cookie
来源：http://gv.9csxet.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ez.szsharing.cn

[U67] PHP：处理文件上传
来源：http://vr.szxytkj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://us.huixiangedu.cn

[U68] PHP：PDO 连接
来源：http://qx.panjiajie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gl.shxzskj.cn

[U69] PHP：PDO 预处理
来源：http://zs.wgjwhj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://as.bookmarksfly.cn

[U70] PHP：PDO 事务
来源：http://xd.nicolike.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nm.muxihuayi.cn

[U71] PHP：抛出异常
来源：http://rg.hnjuh.cn

throw new RuntimeException("失败", 500);
来源：http://vb.hnjuh.cn

[U72] PHP：写错误日志
来源：http://hw.yuexingan06.cn

error_log("失败: " . $e->getMessage());
来源：http://iw.shtwfgs.cn

[U73] PHP：读取 ini 配置
来源：http://tn.yuntaijiaju.cn

parse_ini_file("config.ini", true)
来源：http://vl.shtwfgs.cn

[U74] PHP：读取环境变量
来源：http://bh.asd995.cn

getenv("APP_ENV") ?: "production"
来源：http://yi.shtwfgs.cn

[U75] PHP：依赖注入
来源：http://tv.huixinmuqiang.cn

composer require psr/container
来源：http://gq.jianghongdianzi.cn

[U76] PHP：简单路由
来源：http://zt.nicolike.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://al.gzmigu.cn

[U77] PHP：模板渲染
来源：http://cp.huixinmuqiang.cn

composer require twig/twig
来源：http://cw.shxzukj.cn

[U78] PHP：单元测试
来源：http://pz.yuexingan06.cn

composer require --dev phpunit/phpunit
来源：http://ez.asd995.cn

[U79] PHP：静态分析
来源：http://qr.nszjky.cn

composer require --dev phpstan/phpstan
来源：http://mu.newstarts.cn

[U80] PHP：代码规范修复
来源：http://ua.jctech888.com.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://nh.haigaiapp.cn

[U81] JS：初始化项目
来源：http://ar.hahajie.cn

npm init -y;  npm i express
来源：http://dv.nicolike.cn

[U82] JS：package.json 脚本
来源：http://ww.hnjuh.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wx.wgjwhj.cn

[U83] JS：ES Module 导入导出
来源：http://tv.asd995.cn

export const a = 1;  import { a } from "./m.js";
来源：http://jx.bjjhwx.cn

[U84] JS：CommonJS 写法
来源：http://ru.huixiangedu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://pd.hnjuh.cn

[U85] JS：可选链
来源：http://gt.9csxet.cn

a?.b?.c
来源：http://uv.nszjky.cn

[U86] JS：空值合并
来源：http://wq.yuexingan06.cn

a ?? b
来源：http://oi.panjiajie.cn

[U87] JS：解构默认值
来源：http://bt.hnjuh.cn

const { a = 1, b = 2 } = obj;
来源：http://kv.gzmigu.cn

[U88] JS：对象展开合并
来源：http://rn.haigaiapp.cn

{ ...a, ...b }
来源：http://xe.hahajie.cn

[U89] JS：数组去重
来源：http://dk.521024.cn

[...new Set(arr)]
来源：http://vl.muxihuayi.cn

[U90] JS：数字数组排序
来源：http://ho.nicolike.cn

[...arr].sort((a, b) => a - b)
来源：http://qv.asd995.cn

[U91] JS：对象键值遍历
来源：http://pa.hahajie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pz.yuexingan06.cn

[U92] JS：深拷贝
来源：http://ym.521024.cn

structuredClone(obj)
来源：http://jz.yuntaijiaju.cn

[U93] JS：模板字符串
来源：http://bp.521024.cn

`共 ${n} 条`
来源：http://qg.wgjwhj.cn

[U94] JS：箭头函数
来源：http://pb.szsharing.cn

const double = x => x * 2;
来源：http://nj.wgjwhj.cn

[U95] JS：Promise 包装
来源：http://ch.521024.cn

new Promise((resolve, reject) => {})
来源：http://tc.bookmarksfly.cn

[U96] JS：async/await 与异常
来源：http://rv.huanxung.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mj.yuexingan06.cn

[U97] JS：并发请求
来源：http://ai.shxzukj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://oz.nszjky.cn

[U98] JS：fetch 带 JSON
来源：http://nm.bookmarksfly.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mq.shxzukj.cn

[U99] JS：事件监听
来源：http://gf.chemitech.net.cn

el.addEventListener("click", e => {})
来源：http://mu.haigaiapp.cn

[U100] JS：DOM 查询
来源：http://hx.huixiangedu.cn

document.querySelector(".item")
来源：http://pu.chemitech.net.cn

[U101] JS：classList 操作
来源：http://up.haigaiapp.cn

el.classList.toggle("active")
来源：http://fv.9csxet.cn

[U102] JS：本地存储
来源：http://ev.huanxung.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://it.huixiangedu.cn

[U103] JS：定时器
来源：http://jo.muxihuayi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ri.asd995.cn

[U104] JS：防抖
来源：http://gm.colortex.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wa.jctech888.com.cn

[U105] JS：节流
来源：http://jl.panjiajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wq.hahajie.cn

[U106] JS：日期格式化
来源：http://yd.shtwfgs.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xe.newstarts.cn

[U107] JS：数字千分位
来源：http://zu.chemitech.net.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ro.hnjuh.cn

[U108] JS：随机整数
来源：http://db.jianghongdianzi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yf.shxzskj.cn

[U109] JS：数组分组
来源：http://ot.chemitech.net.cn

Object.groupBy(arr, x => x.type)
来源：http://uc.huanxung.cn

[U110] JS：数组分块
来源：http://zl.huixinmuqiang.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mu.huixiangedu.cn

[U111] JS：对象转 Map
来源：http://ww.jianghongdianzi.cn

new Map(Object.entries(obj))
来源：http://ho.huixinmuqiang.cn

[U112] JS：字符串补位
来源：http://rl.nicolike.cn

"7".padStart(3, "0")
来源：http://yi.nicolike.cn

[U113] JS：正则替换全部
来源：http://rw.hnjuh.cn

s.replaceAll("a", "b")
来源：http://fj.hnjuh.cn

[U114] JS：JSON 深比较
来源：http://yd.bookmarksfly.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://zh.bookmarksfly.cn

[U115] JS：生成 UUID
来源：http://mh.521024.cn

crypto.randomUUID()
来源：http://rt.newstarts.cn

[U116] JS：类型检查（JSDoc）
来源：http://pf.bjjhwx.cn

/** @param {string} name */ function f(name) {}
来源：http://bs.huixiangedu.cn

[U117] JS：单元测试
来源：http://mc.asd995.cn

npm i -D vitest;  npx vitest
来源：http://pl.521024.cn

[U118] JS：开发服务器
来源：http://wh.yuexingan06.cn

npm i -D vite;  npx vite
来源：http://mm.hnjuh.cn

[U119] JS：生产构建
来源：http://jj.yuntaijiaju.cn

npx vite build
来源：http://ui.bjjhwx.cn

[U120] JS：读取环境变量（Vite）
来源：http://li.hahajie.cn

import.meta.env.VITE_API_URL
来源：http://ae.hnjuh.cn

================================================================================
来源：http://bc.huixinmuqiang.cn

统计汇总
来源：http://in.9csxet.cn

================================================================================
来源：http://ew.hahajie.cn

按语言统计（条）：
来源：http://zs.asd995.cn

Python ......... 252
来源：http://kp.521024.cn

PHP ............ 252
来源：http://hk.newstarts.cn

JavaScript ..... 252
来源：http://mw.huixiangedu.cn

TypeScript ..... 212
来源：http://fh.newstarts.cn

Java ........... 212
来源：http://jv.newstarts.cn

Go ............. 212
来源：http://mq.newstarts.cn

Ruby ........... 212
来源：http://mi.hnjuh.cn

C# ............. 212
来源：http://mq.haigaiapp.cn

C .............. 30
来源：http://jl.szxytkj.cn

C++ ............ 30
来源：http://cv.shxzskj.cn

SQL ............ 90
来源：http://gl.lnxyls.cn

Bash ........... 80
来源：http://sa.nicolike.cn

Kotlin ......... 15
来源：http://dd.huixiangedu.cn

Swift .......... 15
来源：http://qb.szxytkj.cn

Lua ............ 10
来源：http://fm.szxytkj.cn

Perl ........... 10
来源：http://la.521024.cn

Scala .......... 10
来源：http://jp.panjiajie.cn

------------------------------------
来源：http://by.nicolike.cn

合计 ........... 2106 条
来源：http://wa.panjiajie.cn

按章节统计：
来源：http://gg.hahajie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qo.hahajie.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qq.szsharing.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://yp.huixinmuqiang.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://el.muxihuayi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wl.haigaiapp.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gz.asd995.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jo.nszjky.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fk.colortex.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yf.asd995.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ty.jianghongdianzi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vf.lnxyls.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ob.haigaiapp.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wh.9csxet.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hf.gzmigu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://th.chemitech.net.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://iw.bjjhwx.cn

Q SQL 专题                              90
来源：http://ca.jctech888.com.cn

R Bash 专题                             80
来源：http://al.jctech888.com.cn

S C / C++ 专题                          60
来源：http://nz.szxytkj.cn

T 其他语言补充                          60
来源：http://fx.hahajie.cn

U 高频实用片段                         120
来源：http://as.panjiajie.cn

------------------------------------
来源：http://gc.muxihuayi.cn

合计                                  2106 条
来源：http://tc.521024.cn

--------------------------------------------------------------------------------
来源：http://kv.yuntaijiaju.cn

使用提醒
来源：http://jd.szsharing.cn

--------------------------------------------------------------------------------
来源：http://gj.nszjky.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ny.muxihuayi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ke.newstarts.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ew.shtwfgs.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://jk.shxzskj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jd.wgjwhj.cn

—— 文件结束 ——
来源：http://uq.shxzukj.cn

================================================================================
来源：http://rn.muxihuayi.cn

程序语言常见例子速查手册（2024 版）
来源：http://st.huixiangedu.cn

Common Programming Examples Cheat Book
来源：http://vq.panjiajie.cn

================================================================================
来源：http://rc.bjjhwx.cn


<!-- 参考信息 -->