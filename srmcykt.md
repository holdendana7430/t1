代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://el.colortex.cn

[T55] Scala：集合过滤
来源：http://kr.asd995.cn

List(1, 2, 3).filter(_ > 1)
来源：http://yo.chemitech.net.cn

[T56] Scala：样例类
来源：http://gv.haigaiapp.cn

case class User(name: String, age: Int)
来源：http://bv.shxzukj.cn

[T57] Scala：模式匹配
来源：http://tg.haigaiapp.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://pd.gzmigu.cn

[T58] Scala：函数定义
来源：http://em.haigaiapp.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fb.bjjhwx.cn

[T59] Scala：循环
来源：http://yg.hnjuh.cn

for (i <- 1 to 10) println(i)
来源：http://ni.hahajie.cn

[T60] Scala：折叠
来源：http://tq.hnjuh.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dn.yuntaijiaju.cn

================================================================================
来源：http://hv.hahajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://po.jianghongdianzi.cn

================================================================================
来源：http://xx.521024.cn

[U01] Py：创建虚拟环境
来源：http://ek.haigaiapp.cn

python -m venv .venv && source .venv/bin/activate
来源：http://rf.huixinmuqiang.cn

[U02] Py：导出 / 安装依赖
来源：http://dx.shtwfgs.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://li.huixinmuqiang.cn

[U03] Py：加载 .env 配置
来源：http://bj.muxihuayi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qu.huixinmuqiang.cn

[U04] Py：变量调试打印
来源：http://bz.asd995.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://uq.szxytkj.cn

[U05] Py：列表去重且保序
来源：http://nl.szsharing.cn

list(dict.fromkeys(arr))
来源：http://te.jctech888.com.cn

[U06] Py：合并两个字典
来源：http://xz.szxytkj.cn

{**a, **b}
来源：http://uo.huixiangedu.cn

[U07] Py：反转字典键值
来源：http://gr.gzmigu.cn

{v: k for k, v in d.items()}
来源：http://ac.jianghongdianzi.cn

[U08] Py：展平二维列表
来源：http://rs.szxytkj.cn

[y for x in nested for y in x]
来源：http://qo.gzmigu.cn

[U09] Py：字典取最大值的键
来源：http://iy.huixinmuqiang.cn

max(d, key=d.get)
来源：http://qx.jianghongdianzi.cn

[U10] Py：按值排序字典
来源：http://ll.nszjky.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.wgjwhj.cn

[U11] Py：生成器表达式
来源：http://jg.panjiajie.cn

(x * 2 for x in arr)
来源：http://pm.panjiajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://km.yuntaijiaju.cn

Counter(arr).most_common(3)
来源：http://tv.nicolike.cn

[U13] Py：固定长度队列
来源：http://vu.huanxung.cn

deque(maxlen=10)
来源：http://rc.huixiangedu.cn

[U14] Py：分组收集到列表
来源：http://lp.asd995.cn

defaultdict(list)
来源：http://im.hnjuh.cn

[U15] Py：高精度计时
来源：http://hb.huixinmuqiang.cn

t = time.perf_counter()
来源：http://gf.huixiangedu.cn

[U16] Py：命令行参数解析
来源：http://nf.521024.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://th.szxytkj.cn

[U17] Py：初始化日志
来源：http://ez.jctech888.com.cn

logging.basicConfig(level=logging.INFO)
来源：http://lr.bjjhwx.cn

[U18] Py：预编译正则
来源：http://jb.huixinmuqiang.cn

pat = re.compile(r"\d+")
来源：http://tj.gzmigu.cn

[U19] Py：正则替换带回调
来源：http://el.hahajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zi.nicolike.cn

[U20] Py：缓存函数结果
来源：http://sq.chemitech.net.cn

@functools.lru_cache(maxsize=None)
来源：http://zv.muxihuayi.cn

[U21] Py：自定义上下文管理器
来源：http://ek.bookmarksfly.cn

@contextlib.contextmanager
来源：http://bj.hnjuh.cn

[U22] Py：矩阵转置
来源：http://ix.haigaiapp.cn

list(zip(*m))
来源：http://sp.yuntaijiaju.cn

[U23] Py：分块读取大文件
来源：http://xs.hnjuh.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ja.panjiajie.cn

[U24] Py：路径操作
来源：http://gm.huixiangedu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cj.colortex.cn

[U25] Py：CSV 按字典读
来源：http://nr.newstarts.cn

csv.DictReader(f)
来源：http://jb.yuntaijiaju.cn

[U26] Py：并发下载
来源：http://au.gzmigu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jz.huixinmuqiang.cn

[U27] Py：异步 HTTP
来源：http://tq.haigaiapp.cn

aiohttp.ClientSession() 配合 async with
来源：http://ub.shxzskj.cn

[U28] Py：类型别名
来源：http://pg.shtwfgs.cn

UserId = int
来源：http://sj.szsharing.cn

[U29] Py：属性校验
来源：http://nm.shxzukj.cn

@property 与 @x.setter 配合
来源：http://dq.nicolike.cn

[U30] Py：数据类
来源：http://vv.lnxyls.cn

@dataclass(slots=True)
来源：http://la.haigaiapp.cn

[U31] Py：单测
来源：http://zp.yuexingan06.cn

python -m pytest -q
来源：http://hh.huixinmuqiang.cn

[U32] Py：代码格式化
来源：http://ci.shxzukj.cn

ruff format . && ruff check --fix .
来源：http://ng.huanxung.cn

[U33] Py：打包发布
来源：http://tg.nicolike.cn

python -m build  （依赖 pyproject.toml）
来源：http://ko.hahajie.cn

[U34] Py：判断编码
来源：http://be.szxytkj.cn

chardet.detect(raw)
来源：http://ge.bjjhwx.cn

[U35] Py：发送邮件
来源：http://ip.gzmigu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rn.huixinmuqiang.cn

[U36] Py：定时任务
来源：http://wb.yuntaijiaju.cn

schedule.every(10).minutes.do(job)
来源：http://xp.chemitech.net.cn

[U37] Py：读写 Excel
来源：http://pz.panjiajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://lt.bjjhwx.cn

[U38] Py：获取脚本所在目录
来源：http://xb.szsharing.cn

Path(__file__).resolve().parent
来源：http://qm.huanxung.cn

[U39] Py：判断是否在交互环境
来源：http://fb.asd995.cn

sys.stdout.isatty()
来源：http://ro.newstarts.cn

[U40] Py：打印到标准错误
来源：http://vr.yuexingan06.cn

print("err", file=sys.stderr)
来源：http://bt.huixiangedu.cn

[U41] PHP：初始化 Composer 项目
来源：http://qb.gzmigu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://vu.nicolike.cn

[U42] PHP：PSR-4 自动加载
来源：http://en.gzmigu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zi.lnxyls.cn

[U43] PHP：声明命名空间
来源：http://tx.gzmigu.cn

namespace App\Http;
来源：http://aj.bookmarksfly.cn

[U44] PHP：开启严格类型
来源：http://lw.hnjuh.cn

declare(strict_types=1);
来源：http://uj.nszjky.cn

[U45] PHP：类型声明与返回类型
来源：http://cw.huanxung.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://je.huanxung.cn

[U46] PHP：可空类型
来源：http://cb.shxzskj.cn

?string $name = null
来源：http://wz.jianghongdianzi.cn

[U47] PHP：联合类型
来源：http://ca.chemitech.net.cn

int|string $id
来源：http://ek.huixiangedu.cn

[U48] PHP：纯枚举
来源：http://gm.yuexingan06.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wh.huixinmuqiang.cn

[U49] PHP：只读属性
来源：http://hq.szsharing.cn

public readonly string $name
来源：http://gv.muxihuayi.cn

[U50] PHP：构造器属性提升
来源：http://zk.shxzskj.cn

public function __construct(private int $id) {}
来源：http://hi.nicolike.cn

[U51] PHP：数组解构
来源：http://io.9csxet.cn

[$a, $b] = $arr;
来源：http://qa.shtwfgs.cn

[U52] PHP：箭头函数
来源：http://ng.yuntaijiaju.cn

$double = fn($x) => $x * 2;
来源：http://hk.wgjwhj.cn

[U53] PHP：空合并运算符
来源：http://dr.szxytkj.cn

$v = $a ?? $b ?? "default";
来源：http://gq.newstarts.cn

[U54] PHP：空安全调用
来源：http://fm.wgjwhj.cn

$obj?->method()
来源：http://aa.nszjky.cn

[U55] PHP：match 表达式
来源：http://jv.gzmigu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gn.hnjuh.cn

[U56] PHP：命名参数
来源：http://qy.jianghongdianzi.cn

f(a: 1, b: 2)
来源：http://ai.jctech888.com.cn

[U57] PHP：字符串插值
来源：http://ly.nicolike.cn

"值: {$a}"
来源：http://ef.yuntaijiaju.cn

[U58] PHP：数组三件套
来源：http://ox.shxzukj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://iz.huixinmuqiang.cn

[U59] PHP：自定义排序
来源：http://eo.panjiajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vj.lnxyls.cn

[U60] PHP：JSON 编解码
来源：http://rv.newstarts.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ly.huanxung.cn

[U61] PHP：正则
来源：http://xx.huanxung.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yo.nszjky.cn

[U62] PHP：日期对象
来源：http://xd.muxihuayi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ks.9csxet.cn

[U63] PHP：文件读写
来源：http://ry.bjjhwx.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jh.colortex.cn

[U64] PHP：目录遍历
来源：http://kh.newstarts.cn

glob("dir/*.php");  scandir("dir");
来源：http://ce.nicolike.cn

[U65] PHP：会话
来源：http://kd.asd995.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://lg.chemitech.net.cn

[U66] PHP：设置 Cookie
来源：http://th.521024.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://oy.nszjky.cn

[U67] PHP：处理文件上传
来源：http://yy.jianghongdianzi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kh.huixiangedu.cn

[U68] PHP：PDO 连接
来源：http://ni.hnjuh.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xi.szxytkj.cn

[U69] PHP：PDO 预处理
来源：http://he.wgjwhj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xf.bjjhwx.cn

[U70] PHP：PDO 事务
来源：http://kd.gzmigu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://va.hahajie.cn

[U71] PHP：抛出异常
来源：http://tr.muxihuayi.cn

throw new RuntimeException("失败", 500);
来源：http://wx.huixiangedu.cn

[U72] PHP：写错误日志
来源：http://gr.nicolike.cn

error_log("失败: " . $e->getMessage());
来源：http://qd.huanxung.cn

[U73] PHP：读取 ini 配置
来源：http://iy.panjiajie.cn

parse_ini_file("config.ini", true)
来源：http://hq.colortex.cn

[U74] PHP：读取环境变量
来源：http://go.huanxung.cn

getenv("APP_ENV") ?: "production"
来源：http://dw.gzmigu.cn

[U75] PHP：依赖注入
来源：http://qa.shxzskj.cn

composer require psr/container
来源：http://jf.nicolike.cn

[U76] PHP：简单路由
来源：http://rc.jctech888.com.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tg.521024.cn

[U77] PHP：模板渲染
来源：http://or.521024.cn

composer require twig/twig
来源：http://ks.hnjuh.cn

[U78] PHP：单元测试
来源：http://ye.szxytkj.cn

composer require --dev phpunit/phpunit
来源：http://fa.gzmigu.cn

[U79] PHP：静态分析
来源：http://kp.9csxet.cn

composer require --dev phpstan/phpstan
来源：http://jh.nszjky.cn

[U80] PHP：代码规范修复
来源：http://vl.521024.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://lc.hnjuh.cn

[U81] JS：初始化项目
来源：http://ef.asd995.cn

npm init -y;  npm i express
来源：http://sw.wgjwhj.cn

[U82] JS：package.json 脚本
来源：http://uu.jianghongdianzi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cf.huixinmuqiang.cn

[U83] JS：ES Module 导入导出
来源：http://re.bookmarksfly.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ch.hahajie.cn

[U84] JS：CommonJS 写法
来源：http://li.jianghongdianzi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://rj.szxytkj.cn

[U85] JS：可选链
来源：http://xf.huixinmuqiang.cn

a?.b?.c
来源：http://cv.panjiajie.cn

[U86] JS：空值合并
来源：http://fo.shxzukj.cn

a ?? b
来源：http://ls.colortex.cn

[U87] JS：解构默认值
来源：http://yt.bjjhwx.cn

const { a = 1, b = 2 } = obj;
来源：http://ll.jianghongdianzi.cn

[U88] JS：对象展开合并
来源：http://yf.hahajie.cn

{ ...a, ...b }
来源：http://ii.hahajie.cn

[U89] JS：数组去重
来源：http://yr.521024.cn

[...new Set(arr)]
来源：http://rr.9csxet.cn

[U90] JS：数字数组排序
来源：http://ox.colortex.cn

[...arr].sort((a, b) => a - b)
来源：http://dm.521024.cn

[U91] JS：对象键值遍历
来源：http://na.nicolike.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hg.9csxet.cn

[U92] JS：深拷贝
来源：http://te.szsharing.cn

structuredClone(obj)
来源：http://tz.shxzskj.cn

[U93] JS：模板字符串
来源：http://hm.lnxyls.cn

`共 ${n} 条`
来源：http://zk.asd995.cn

[U94] JS：箭头函数
来源：http://it.wgjwhj.cn

const double = x => x * 2;
来源：http://ra.chemitech.net.cn

[U95] JS：Promise 包装
来源：http://ie.szsharing.cn

new Promise((resolve, reject) => {})
来源：http://ew.shxzukj.cn

[U96] JS：async/await 与异常
来源：http://xp.jianghongdianzi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fv.521024.cn

[U97] JS：并发请求
来源：http://qv.asd995.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://xn.huixinmuqiang.cn

[U98] JS：fetch 带 JSON
来源：http://ff.huixinmuqiang.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://id.colortex.cn

[U99] JS：事件监听
来源：http://mq.nszjky.cn

el.addEventListener("click", e => {})
来源：http://aa.521024.cn

[U100] JS：DOM 查询
来源：http://rt.yuexingan06.cn

document.querySelector(".item")
来源：http://hq.szxytkj.cn

[U101] JS：classList 操作
来源：http://eo.hnjuh.cn

el.classList.toggle("active")
来源：http://ke.shtwfgs.cn

[U102] JS：本地存储
来源：http://jj.yuexingan06.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ka.gzmigu.cn

[U103] JS：定时器
来源：http://ja.nszjky.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wq.huixiangedu.cn

[U104] JS：防抖
来源：http://vg.521024.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pi.9csxet.cn

[U105] JS：节流
来源：http://oj.gzmigu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ae.szsharing.cn

[U106] JS：日期格式化
来源：http://sd.jianghongdianzi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://in.huanxung.cn

[U107] JS：数字千分位
来源：http://as.huanxung.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://us.muxihuayi.cn

[U108] JS：随机整数
来源：http://gt.bookmarksfly.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nn.hahajie.cn

[U109] JS：数组分组
来源：http://el.huixiangedu.cn

Object.groupBy(arr, x => x.type)
来源：http://vo.9csxet.cn

[U110] JS：数组分块
来源：http://tu.asd995.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fw.lnxyls.cn

[U111] JS：对象转 Map
来源：http://ns.wgjwhj.cn

new Map(Object.entries(obj))
来源：http://nz.bjjhwx.cn

[U112] JS：字符串补位
来源：http://rl.szxytkj.cn

"7".padStart(3, "0")
来源：http://xg.shtwfgs.cn

[U113] JS：正则替换全部
来源：http://sp.huixinmuqiang.cn

s.replaceAll("a", "b")
来源：http://yr.nszjky.cn

[U114] JS：JSON 深比较
来源：http://jq.hnjuh.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://mp.jianghongdianzi.cn

[U115] JS：生成 UUID
来源：http://tv.lnxyls.cn

crypto.randomUUID()
来源：http://az.huixinmuqiang.cn

[U116] JS：类型检查（JSDoc）
来源：http://ig.huixiangedu.cn

/** @param {string} name */ function f(name) {}
来源：http://ha.lnxyls.cn

[U117] JS：单元测试
来源：http://aw.9csxet.cn

npm i -D vitest;  npx vitest
来源：http://nz.nicolike.cn

[U118] JS：开发服务器
来源：http://zr.wgjwhj.cn

npm i -D vite;  npx vite
来源：http://ej.colortex.cn

[U119] JS：生产构建
来源：http://vf.gzmigu.cn

npx vite build
来源：http://gi.huixiangedu.cn

[U120] JS：读取环境变量（Vite）
来源：http://el.huixinmuqiang.cn

import.meta.env.VITE_API_URL
来源：http://xi.chemitech.net.cn

================================================================================
来源：http://ps.muxihuayi.cn

统计汇总
来源：http://ps.jianghongdianzi.cn

================================================================================
来源：http://ws.colortex.cn

按语言统计（条）：
来源：http://ml.muxihuayi.cn

Python ......... 252
来源：http://ju.muxihuayi.cn

PHP ............ 252
来源：http://dv.521024.cn

JavaScript ..... 252
来源：http://ew.jctech888.com.cn

TypeScript ..... 212
来源：http://kn.panjiajie.cn

Java ........... 212
来源：http://xx.bookmarksfly.cn

Go ............. 212
来源：http://br.nicolike.cn

Ruby ........... 212
来源：http://yr.chemitech.net.cn

C# ............. 212
来源：http://up.huixiangedu.cn

C .............. 30
来源：http://xx.bookmarksfly.cn

C++ ............ 30
来源：http://ca.nicolike.cn

SQL ............ 90
来源：http://ts.jctech888.com.cn

Bash ........... 80
来源：http://dl.yuntaijiaju.cn

Kotlin ......... 15
来源：http://rg.szsharing.cn

Swift .......... 15
来源：http://kr.colortex.cn

Lua ............ 10
来源：http://gj.szxytkj.cn

Perl ........... 10
来源：http://ko.hahajie.cn

Scala .......... 10
来源：http://wz.huixinmuqiang.cn

------------------------------------
来源：http://au.newstarts.cn

合计 ........... 2106 条
来源：http://ll.chemitech.net.cn

按章节统计：
来源：http://yi.jianghongdianzi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yu.shxzukj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://oy.gzmigu.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://sd.szsharing.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fs.nszjky.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mq.shxzskj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ru.shtwfgs.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://eb.hahajie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://yi.lnxyls.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tz.szsharing.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fx.jianghongdianzi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vm.shxzukj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://la.shtwfgs.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xk.huanxung.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wz.wgjwhj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://su.9csxet.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rd.huanxung.cn

Q SQL 专题                              90
来源：http://nk.huanxung.cn

R Bash 专题                             80
来源：http://et.bjjhwx.cn

S C / C++ 专题                          60
来源：http://yx.panjiajie.cn

T 其他语言补充                          60
来源：http://jk.nicolike.cn


<!-- 参考信息 -->