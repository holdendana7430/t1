代发 wailian999

[U01] Py：创建虚拟环境
来源：http://qg.colortex.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mm.nicolike.cn

[U02] Py：导出 / 安装依赖
来源：http://xr.chemitech.net.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cn.muxihuayi.cn

[U03] Py：加载 .env 配置
来源：http://re.9csxet.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gu.lnxyls.cn

[U04] Py：变量调试打印
来源：http://fh.wgjwhj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fh.muxihuayi.cn

[U05] Py：列表去重且保序
来源：http://eu.nicolike.cn

list(dict.fromkeys(arr))
来源：http://wv.yuexingan06.cn

[U06] Py：合并两个字典
来源：http://gb.gzmigu.cn

{**a, **b}
来源：http://yr.haigaiapp.cn

[U07] Py：反转字典键值
来源：http://wj.yuexingan06.cn

{v: k for k, v in d.items()}
来源：http://gc.colortex.cn

[U08] Py：展平二维列表
来源：http://kq.yuexingan06.cn

[y for x in nested for y in x]
来源：http://hy.hnjuh.cn

[U09] Py：字典取最大值的键
来源：http://nb.shxzukj.cn

max(d, key=d.get)
来源：http://pq.jctech888.com.cn

[U10] Py：按值排序字典
来源：http://rq.bjjhwx.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ri.haigaiapp.cn

[U11] Py：生成器表达式
来源：http://pw.chemitech.net.cn

(x * 2 for x in arr)
来源：http://zy.muxihuayi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://vv.newstarts.cn

Counter(arr).most_common(3)
来源：http://bm.panjiajie.cn

[U13] Py：固定长度队列
来源：http://mi.panjiajie.cn

deque(maxlen=10)
来源：http://vr.gzmigu.cn

[U14] Py：分组收集到列表
来源：http://zk.lnxyls.cn

defaultdict(list)
来源：http://hs.muxihuayi.cn

[U15] Py：高精度计时
来源：http://ze.nszjky.cn

t = time.perf_counter()
来源：http://zv.huixinmuqiang.cn

[U16] Py：命令行参数解析
来源：http://jr.lnxyls.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rh.bookmarksfly.cn

[U17] Py：初始化日志
来源：http://wi.panjiajie.cn

logging.basicConfig(level=logging.INFO)
来源：http://ic.huixiangedu.cn

[U18] Py：预编译正则
来源：http://yb.hahajie.cn

pat = re.compile(r"\d+")
来源：http://xo.panjiajie.cn

[U19] Py：正则替换带回调
来源：http://wq.nszjky.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qd.wgjwhj.cn

[U20] Py：缓存函数结果
来源：http://ph.haigaiapp.cn

@functools.lru_cache(maxsize=None)
来源：http://ov.jctech888.com.cn

[U21] Py：自定义上下文管理器
来源：http://eq.chemitech.net.cn

@contextlib.contextmanager
来源：http://rm.9csxet.cn

[U22] Py：矩阵转置
来源：http://av.9csxet.cn

list(zip(*m))
来源：http://qg.asd995.cn

[U23] Py：分块读取大文件
来源：http://qj.huanxung.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://at.hnjuh.cn

[U24] Py：路径操作
来源：http://bp.szxytkj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lr.shtwfgs.cn

[U25] Py：CSV 按字典读
来源：http://zv.shtwfgs.cn

csv.DictReader(f)
来源：http://cc.hnjuh.cn

[U26] Py：并发下载
来源：http://lk.szxytkj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gf.hahajie.cn

[U27] Py：异步 HTTP
来源：http://cp.9csxet.cn

aiohttp.ClientSession() 配合 async with
来源：http://qr.panjiajie.cn

[U28] Py：类型别名
来源：http://xl.szsharing.cn

UserId = int
来源：http://jt.jianghongdianzi.cn

[U29] Py：属性校验
来源：http://ia.szsharing.cn

@property 与 @x.setter 配合
来源：http://lf.shtwfgs.cn

[U30] Py：数据类
来源：http://jm.nicolike.cn

@dataclass(slots=True)
来源：http://wp.muxihuayi.cn

[U31] Py：单测
来源：http://ok.huixiangedu.cn

python -m pytest -q
来源：http://ec.panjiajie.cn

[U32] Py：代码格式化
来源：http://ro.jctech888.com.cn

ruff format . && ruff check --fix .
来源：http://rj.nicolike.cn

[U33] Py：打包发布
来源：http://tq.jctech888.com.cn

python -m build  （依赖 pyproject.toml）
来源：http://tt.nszjky.cn

[U34] Py：判断编码
来源：http://mk.newstarts.cn

chardet.detect(raw)
来源：http://sg.shtwfgs.cn

[U35] Py：发送邮件
来源：http://mk.szsharing.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gx.colortex.cn

[U36] Py：定时任务
来源：http://nj.9csxet.cn

schedule.every(10).minutes.do(job)
来源：http://bt.colortex.cn

[U37] Py：读写 Excel
来源：http://eg.jianghongdianzi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://id.panjiajie.cn

[U38] Py：获取脚本所在目录
来源：http://fs.bjjhwx.cn

Path(__file__).resolve().parent
来源：http://aw.asd995.cn

[U39] Py：判断是否在交互环境
来源：http://yw.haigaiapp.cn

sys.stdout.isatty()
来源：http://sg.nszjky.cn

[U40] Py：打印到标准错误
来源：http://sb.asd995.cn

print("err", file=sys.stderr)
来源：http://ig.9csxet.cn

[U41] PHP：初始化 Composer 项目
来源：http://sr.huanxung.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://yc.nszjky.cn

[U42] PHP：PSR-4 自动加载
来源：http://bv.shxzukj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ia.chemitech.net.cn

[U43] PHP：声明命名空间
来源：http://rj.wgjwhj.cn

namespace App\Http;
来源：http://tm.521024.cn

[U44] PHP：开启严格类型
来源：http://eo.newstarts.cn

declare(strict_types=1);
来源：http://jk.gzmigu.cn

[U45] PHP：类型声明与返回类型
来源：http://fk.huixiangedu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://wt.shxzskj.cn

[U46] PHP：可空类型
来源：http://ur.haigaiapp.cn

?string $name = null
来源：http://gm.szsharing.cn

[U47] PHP：联合类型
来源：http://oa.huixiangedu.cn

int|string $id
来源：http://yp.jctech888.com.cn

[U48] PHP：纯枚举
来源：http://lg.colortex.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vi.huixiangedu.cn

[U49] PHP：只读属性
来源：http://he.lnxyls.cn

public readonly string $name
来源：http://nb.bookmarksfly.cn

[U50] PHP：构造器属性提升
来源：http://aj.gzmigu.cn

public function __construct(private int $id) {}
来源：http://qf.asd995.cn

[U51] PHP：数组解构
来源：http://xo.wgjwhj.cn

[$a, $b] = $arr;
来源：http://xc.hnjuh.cn

[U52] PHP：箭头函数
来源：http://ja.szxytkj.cn

$double = fn($x) => $x * 2;
来源：http://xl.521024.cn

[U53] PHP：空合并运算符
来源：http://oa.nicolike.cn

$v = $a ?? $b ?? "default";
来源：http://gf.nicolike.cn

[U54] PHP：空安全调用
来源：http://rz.yuexingan06.cn

$obj?->method()
来源：http://ci.hnjuh.cn

[U55] PHP：match 表达式
来源：http://nh.hnjuh.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://oj.haigaiapp.cn

[U56] PHP：命名参数
来源：http://vo.newstarts.cn

f(a: 1, b: 2)
来源：http://nf.shxzskj.cn

[U57] PHP：字符串插值
来源：http://to.bookmarksfly.cn

"值: {$a}"
来源：http://iv.hahajie.cn

[U58] PHP：数组三件套
来源：http://mg.bjjhwx.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gu.hahajie.cn

[U59] PHP：自定义排序
来源：http://oe.bjjhwx.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rf.huixiangedu.cn

[U60] PHP：JSON 编解码
来源：http://fg.haigaiapp.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://sf.szsharing.cn

[U61] PHP：正则
来源：http://yk.jianghongdianzi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xc.yuexingan06.cn

[U62] PHP：日期对象
来源：http://ch.muxihuayi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gj.bookmarksfly.cn

[U63] PHP：文件读写
来源：http://rw.szxytkj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qg.jctech888.com.cn

[U64] PHP：目录遍历
来源：http://tu.jianghongdianzi.cn

glob("dir/*.php");  scandir("dir");
来源：http://eu.yuntaijiaju.cn

[U65] PHP：会话
来源：http://xk.muxihuayi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://cb.panjiajie.cn

[U66] PHP：设置 Cookie
来源：http://xg.jianghongdianzi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ee.szsharing.cn

[U67] PHP：处理文件上传
来源：http://io.szsharing.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lg.bookmarksfly.cn

[U68] PHP：PDO 连接
来源：http://up.huixiangedu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://df.lnxyls.cn

[U69] PHP：PDO 预处理
来源：http://bm.nicolike.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vn.asd995.cn

[U70] PHP：PDO 事务
来源：http://so.newstarts.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ga.newstarts.cn

[U71] PHP：抛出异常
来源：http://kg.huixiangedu.cn

throw new RuntimeException("失败", 500);
来源：http://sv.szsharing.cn

[U72] PHP：写错误日志
来源：http://px.shxzukj.cn

error_log("失败: " . $e->getMessage());
来源：http://ox.lnxyls.cn

[U73] PHP：读取 ini 配置
来源：http://ee.521024.cn

parse_ini_file("config.ini", true)
来源：http://pd.shxzskj.cn

[U74] PHP：读取环境变量
来源：http://ue.bjjhwx.cn

getenv("APP_ENV") ?: "production"
来源：http://xl.chemitech.net.cn

[U75] PHP：依赖注入
来源：http://im.shxzskj.cn

composer require psr/container
来源：http://da.muxihuayi.cn

[U76] PHP：简单路由
来源：http://ms.haigaiapp.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://om.szsharing.cn

[U77] PHP：模板渲染
来源：http://ko.huixiangedu.cn

composer require twig/twig
来源：http://eg.panjiajie.cn

[U78] PHP：单元测试
来源：http://ax.521024.cn

composer require --dev phpunit/phpunit
来源：http://jy.wgjwhj.cn

[U79] PHP：静态分析
来源：http://dt.huixinmuqiang.cn

composer require --dev phpstan/phpstan
来源：http://pv.szxytkj.cn

[U80] PHP：代码规范修复
来源：http://hp.hahajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://mv.shxzukj.cn

[U81] JS：初始化项目
来源：http://bt.huanxung.cn

npm init -y;  npm i express
来源：http://gw.nszjky.cn

[U82] JS：package.json 脚本
来源：http://xa.hnjuh.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yu.asd995.cn

[U83] JS：ES Module 导入导出
来源：http://ox.hnjuh.cn

export const a = 1;  import { a } from "./m.js";
来源：http://nb.shxzukj.cn

[U84] JS：CommonJS 写法
来源：http://cz.hnjuh.cn

module.exports = { a };  const { a } = require("./m");
来源：http://go.9csxet.cn

[U85] JS：可选链
来源：http://mv.yuntaijiaju.cn

a?.b?.c
来源：http://pd.huanxung.cn

[U86] JS：空值合并
来源：http://df.wgjwhj.cn

a ?? b
来源：http://so.chemitech.net.cn

[U87] JS：解构默认值
来源：http://vl.shxzukj.cn

const { a = 1, b = 2 } = obj;
来源：http://sa.521024.cn

[U88] JS：对象展开合并
来源：http://tv.shtwfgs.cn

{ ...a, ...b }
来源：http://km.521024.cn

[U89] JS：数组去重
来源：http://qm.gzmigu.cn

[...new Set(arr)]
来源：http://rz.huanxung.cn

[U90] JS：数字数组排序
来源：http://rh.shxzukj.cn

[...arr].sort((a, b) => a - b)
来源：http://ok.lnxyls.cn

[U91] JS：对象键值遍历
来源：http://he.szsharing.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xv.bookmarksfly.cn

[U92] JS：深拷贝
来源：http://oq.huixiangedu.cn

structuredClone(obj)
来源：http://hy.hahajie.cn

[U93] JS：模板字符串
来源：http://py.huixinmuqiang.cn

`共 ${n} 条`
来源：http://de.newstarts.cn

[U94] JS：箭头函数
来源：http://hg.gzmigu.cn

const double = x => x * 2;
来源：http://hd.colortex.cn

[U95] JS：Promise 包装
来源：http://bj.jianghongdianzi.cn

new Promise((resolve, reject) => {})
来源：http://zw.gzmigu.cn

[U96] JS：async/await 与异常
来源：http://rd.shtwfgs.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ur.bookmarksfly.cn

[U97] JS：并发请求
来源：http://gg.haigaiapp.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vy.wgjwhj.cn

[U98] JS：fetch 带 JSON
来源：http://id.huixiangedu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dv.521024.cn

[U99] JS：事件监听
来源：http://rn.9csxet.cn

el.addEventListener("click", e => {})
来源：http://qn.bjjhwx.cn

[U100] JS：DOM 查询
来源：http://wb.huixinmuqiang.cn

document.querySelector(".item")
来源：http://di.huixiangedu.cn

[U101] JS：classList 操作
来源：http://xx.hahajie.cn

el.classList.toggle("active")
来源：http://si.yuntaijiaju.cn

[U102] JS：本地存储
来源：http://jc.yuntaijiaju.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wn.panjiajie.cn

[U103] JS：定时器
来源：http://il.shxzskj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://cy.muxihuayi.cn

[U104] JS：防抖
来源：http://gf.asd995.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dy.hnjuh.cn

[U105] JS：节流
来源：http://cg.shtwfgs.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zi.muxihuayi.cn

[U106] JS：日期格式化
来源：http://jy.hnjuh.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ly.chemitech.net.cn

[U107] JS：数字千分位
来源：http://ez.wgjwhj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://id.wgjwhj.cn

[U108] JS：随机整数
来源：http://ta.bjjhwx.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fq.wgjwhj.cn

[U109] JS：数组分组
来源：http://mh.lnxyls.cn

Object.groupBy(arr, x => x.type)
来源：http://kc.colortex.cn

[U110] JS：数组分块
来源：http://no.colortex.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kz.asd995.cn

[U111] JS：对象转 Map
来源：http://hj.yuexingan06.cn

new Map(Object.entries(obj))
来源：http://ac.bookmarksfly.cn

[U112] JS：字符串补位
来源：http://dj.shxzukj.cn

"7".padStart(3, "0")
来源：http://cc.jctech888.com.cn

[U113] JS：正则替换全部
来源：http://ak.chemitech.net.cn

s.replaceAll("a", "b")
来源：http://li.chemitech.net.cn

[U114] JS：JSON 深比较
来源：http://cd.jctech888.com.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://rc.shtwfgs.cn

[U115] JS：生成 UUID
来源：http://jt.bookmarksfly.cn

crypto.randomUUID()
来源：http://cs.panjiajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://hg.asd995.cn

/** @param {string} name */ function f(name) {}
来源：http://kf.asd995.cn

[U117] JS：单元测试
来源：http://rh.wgjwhj.cn

npm i -D vitest;  npx vitest
来源：http://qa.bjjhwx.cn

[U118] JS：开发服务器
来源：http://rx.shxzskj.cn

npm i -D vite;  npx vite
来源：http://fz.lnxyls.cn

[U119] JS：生产构建
来源：http://ba.haigaiapp.cn

npx vite build
来源：http://lx.shxzskj.cn

[U120] JS：读取环境变量（Vite）
来源：http://gw.chemitech.net.cn

import.meta.env.VITE_API_URL
来源：http://om.shxzskj.cn

================================================================================
来源：http://lh.lnxyls.cn

统计汇总
来源：http://wm.hnjuh.cn

================================================================================
来源：http://wz.hnjuh.cn

按语言统计（条）：
来源：http://gg.gzmigu.cn

Python ......... 252
来源：http://zt.9csxet.cn

PHP ............ 252
来源：http://vy.wgjwhj.cn

JavaScript ..... 252
来源：http://pv.9csxet.cn

TypeScript ..... 212
来源：http://zs.bookmarksfly.cn

Java ........... 212
来源：http://mz.9csxet.cn

Go ............. 212
来源：http://mi.newstarts.cn

Ruby ........... 212
来源：http://pm.szxytkj.cn

C# ............. 212
来源：http://rv.wgjwhj.cn

C .............. 30
来源：http://yt.shxzskj.cn

C++ ............ 30
来源：http://hn.lnxyls.cn

SQL ............ 90
来源：http://ub.nszjky.cn

Bash ........... 80
来源：http://ws.yuntaijiaju.cn

Kotlin ......... 15
来源：http://ib.huixiangedu.cn

Swift .......... 15
来源：http://sa.jctech888.com.cn

Lua ............ 10
来源：http://zs.huanxung.cn

Perl ........... 10
来源：http://pz.colortex.cn

Scala .......... 10
来源：http://qt.yuexingan06.cn

------------------------------------
来源：http://de.nszjky.cn

合计 ........... 2106 条
来源：http://ky.yuexingan06.cn

按章节统计：
来源：http://is.hahajie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wu.huanxung.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xo.gzmigu.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://oy.szsharing.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://yd.haigaiapp.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zj.szsharing.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ef.521024.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tp.521024.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mo.colortex.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gx.huixinmuqiang.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://eh.bookmarksfly.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zg.colortex.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xa.shtwfgs.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vi.9csxet.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gk.wgjwhj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ps.wgjwhj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://sb.lnxyls.cn

Q SQL 专题                              90
来源：http://vu.muxihuayi.cn

R Bash 专题                             80
来源：http://vt.lnxyls.cn

S C / C++ 专题                          60
来源：http://fc.bookmarksfly.cn

T 其他语言补充                          60
来源：http://qf.colortex.cn

U 高频实用片段                         120
来源：http://np.hnjuh.cn

------------------------------------
来源：http://do.lnxyls.cn

合计                                  2106 条
来源：http://pv.hahajie.cn

--------------------------------------------------------------------------------
来源：http://zz.shtwfgs.cn

使用提醒
来源：http://db.nszjky.cn

--------------------------------------------------------------------------------
来源：http://nt.huixiangedu.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ej.nicolike.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jn.wgjwhj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://dg.shtwfgs.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ag.shxzskj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gu.hnjuh.cn

—— 文件结束 ——
来源：http://yd.521024.cn

================================================================================
来源：http://er.huanxung.cn

程序语言常见例子速查手册（2024 版）
来源：http://er.hahajie.cn

Common Programming Examples Cheat Book
来源：http://iz.gzmigu.cn

================================================================================
来源：http://nz.nszjky.cn


<!-- 参考信息 -->