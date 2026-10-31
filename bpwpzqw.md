代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yc.wgjwhj.cn

================================================================================
来源：http://jv.shxzukj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ce.wgjwhj.cn

================================================================================
来源：http://fz.9csxet.cn

[U01] Py：创建虚拟环境
来源：http://ge.hahajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://np.asd995.cn

[U02] Py：导出 / 安装依赖
来源：http://dv.bjjhwx.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://av.yuexingan06.cn

[U03] Py：加载 .env 配置
来源：http://ou.jianghongdianzi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ub.gzmigu.cn

[U04] Py：变量调试打印
来源：http://ep.yuexingan06.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ej.hnjuh.cn

[U05] Py：列表去重且保序
来源：http://df.muxihuayi.cn

list(dict.fromkeys(arr))
来源：http://wl.wgjwhj.cn

[U06] Py：合并两个字典
来源：http://dq.nszjky.cn

{**a, **b}
来源：http://ed.szsharing.cn

[U07] Py：反转字典键值
来源：http://ih.shxzukj.cn

{v: k for k, v in d.items()}
来源：http://fs.chemitech.net.cn

[U08] Py：展平二维列表
来源：http://ci.chemitech.net.cn

[y for x in nested for y in x]
来源：http://yp.shxzukj.cn

[U09] Py：字典取最大值的键
来源：http://ht.muxihuayi.cn

max(d, key=d.get)
来源：http://ir.shxzukj.cn

[U10] Py：按值排序字典
来源：http://in.bookmarksfly.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dh.szsharing.cn

[U11] Py：生成器表达式
来源：http://cy.szsharing.cn

(x * 2 for x in arr)
来源：http://ko.9csxet.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ty.wgjwhj.cn

Counter(arr).most_common(3)
来源：http://et.muxihuayi.cn

[U13] Py：固定长度队列
来源：http://dx.521024.cn

deque(maxlen=10)
来源：http://wg.colortex.cn

[U14] Py：分组收集到列表
来源：http://wp.nszjky.cn

defaultdict(list)
来源：http://df.huanxung.cn

[U15] Py：高精度计时
来源：http://yv.wgjwhj.cn

t = time.perf_counter()
来源：http://ls.szxytkj.cn

[U16] Py：命令行参数解析
来源：http://zv.panjiajie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qn.bookmarksfly.cn

[U17] Py：初始化日志
来源：http://mt.wgjwhj.cn

logging.basicConfig(level=logging.INFO)
来源：http://fn.chemitech.net.cn

[U18] Py：预编译正则
来源：http://rs.shxzskj.cn

pat = re.compile(r"\d+")
来源：http://mb.hahajie.cn

[U19] Py：正则替换带回调
来源：http://md.bookmarksfly.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xv.hahajie.cn

[U20] Py：缓存函数结果
来源：http://rn.bjjhwx.cn

@functools.lru_cache(maxsize=None)
来源：http://oz.jianghongdianzi.cn

[U21] Py：自定义上下文管理器
来源：http://fc.muxihuayi.cn

@contextlib.contextmanager
来源：http://tp.newstarts.cn

[U22] Py：矩阵转置
来源：http://sq.chemitech.net.cn

list(zip(*m))
来源：http://yw.wgjwhj.cn

[U23] Py：分块读取大文件
来源：http://lw.szsharing.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nl.jianghongdianzi.cn

[U24] Py：路径操作
来源：http://qp.szsharing.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xl.nszjky.cn

[U25] Py：CSV 按字典读
来源：http://rc.lnxyls.cn

csv.DictReader(f)
来源：http://hp.bookmarksfly.cn

[U26] Py：并发下载
来源：http://hr.huixinmuqiang.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://if.wgjwhj.cn

[U27] Py：异步 HTTP
来源：http://fv.muxihuayi.cn

aiohttp.ClientSession() 配合 async with
来源：http://wj.shtwfgs.cn

[U28] Py：类型别名
来源：http://ua.colortex.cn

UserId = int
来源：http://zq.nszjky.cn

[U29] Py：属性校验
来源：http://or.bookmarksfly.cn

@property 与 @x.setter 配合
来源：http://wj.shxzskj.cn

[U30] Py：数据类
来源：http://dv.huanxung.cn

@dataclass(slots=True)
来源：http://xl.lnxyls.cn

[U31] Py：单测
来源：http://gg.yuntaijiaju.cn

python -m pytest -q
来源：http://dd.panjiajie.cn

[U32] Py：代码格式化
来源：http://ms.hahajie.cn

ruff format . && ruff check --fix .
来源：http://ra.newstarts.cn

[U33] Py：打包发布
来源：http://kx.gzmigu.cn

python -m build  （依赖 pyproject.toml）
来源：http://rj.newstarts.cn

[U34] Py：判断编码
来源：http://yw.bookmarksfly.cn

chardet.detect(raw)
来源：http://ew.shxzskj.cn

[U35] Py：发送邮件
来源：http://jm.nszjky.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ax.nszjky.cn

[U36] Py：定时任务
来源：http://lp.chemitech.net.cn

schedule.every(10).minutes.do(job)
来源：http://su.nszjky.cn

[U37] Py：读写 Excel
来源：http://ht.lnxyls.cn

pandas.read_excel / DataFrame.to_excel
来源：http://xx.muxihuayi.cn

[U38] Py：获取脚本所在目录
来源：http://vr.newstarts.cn

Path(__file__).resolve().parent
来源：http://bz.hahajie.cn

[U39] Py：判断是否在交互环境
来源：http://sl.bjjhwx.cn

sys.stdout.isatty()
来源：http://gd.nicolike.cn

[U40] Py：打印到标准错误
来源：http://at.asd995.cn

print("err", file=sys.stderr)
来源：http://rf.shxzskj.cn

[U41] PHP：初始化 Composer 项目
来源：http://up.lnxyls.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zf.521024.cn

[U42] PHP：PSR-4 自动加载
来源：http://ep.szsharing.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yb.wgjwhj.cn

[U43] PHP：声明命名空间
来源：http://gk.bjjhwx.cn

namespace App\Http;
来源：http://ok.jianghongdianzi.cn

[U44] PHP：开启严格类型
来源：http://oa.chemitech.net.cn

declare(strict_types=1);
来源：http://hp.haigaiapp.cn

[U45] PHP：类型声明与返回类型
来源：http://ga.huixinmuqiang.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://fi.huixinmuqiang.cn

[U46] PHP：可空类型
来源：http://xx.panjiajie.cn

?string $name = null
来源：http://jd.yuntaijiaju.cn

[U47] PHP：联合类型
来源：http://hp.szxytkj.cn

int|string $id
来源：http://iw.panjiajie.cn

[U48] PHP：纯枚举
来源：http://sm.newstarts.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zr.shtwfgs.cn

[U49] PHP：只读属性
来源：http://tf.jianghongdianzi.cn

public readonly string $name
来源：http://ks.wgjwhj.cn

[U50] PHP：构造器属性提升
来源：http://br.wgjwhj.cn

public function __construct(private int $id) {}
来源：http://nq.bookmarksfly.cn

[U51] PHP：数组解构
来源：http://bh.huanxung.cn

[$a, $b] = $arr;
来源：http://vh.colortex.cn

[U52] PHP：箭头函数
来源：http://zl.yuntaijiaju.cn

$double = fn($x) => $x * 2;
来源：http://pd.lnxyls.cn

[U53] PHP：空合并运算符
来源：http://le.haigaiapp.cn

$v = $a ?? $b ?? "default";
来源：http://sw.nicolike.cn

[U54] PHP：空安全调用
来源：http://og.muxihuayi.cn

$obj?->method()
来源：http://cb.hnjuh.cn

[U55] PHP：match 表达式
来源：http://lo.shtwfgs.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://oh.521024.cn

[U56] PHP：命名参数
来源：http://vk.nszjky.cn

f(a: 1, b: 2)
来源：http://qo.hahajie.cn

[U57] PHP：字符串插值
来源：http://ta.gzmigu.cn

"值: {$a}"
来源：http://hf.jctech888.com.cn

[U58] PHP：数组三件套
来源：http://it.wgjwhj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fs.haigaiapp.cn

[U59] PHP：自定义排序
来源：http://wu.gzmigu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ry.muxihuayi.cn

[U60] PHP：JSON 编解码
来源：http://xa.9csxet.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rl.521024.cn

[U61] PHP：正则
来源：http://hc.gzmigu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pk.yuexingan06.cn

[U62] PHP：日期对象
来源：http://gp.huanxung.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sx.szxytkj.cn

[U63] PHP：文件读写
来源：http://dl.shxzskj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dl.jctech888.com.cn

[U64] PHP：目录遍历
来源：http://as.nicolike.cn

glob("dir/*.php");  scandir("dir");
来源：http://hs.huixinmuqiang.cn

[U65] PHP：会话
来源：http://rh.colortex.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rb.9csxet.cn

[U66] PHP：设置 Cookie
来源：http://ql.chemitech.net.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hb.lnxyls.cn

[U67] PHP：处理文件上传
来源：http://tq.gzmigu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qy.nszjky.cn

[U68] PHP：PDO 连接
来源：http://zx.jianghongdianzi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yg.colortex.cn

[U69] PHP：PDO 预处理
来源：http://ac.huanxung.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fc.yuexingan06.cn

[U70] PHP：PDO 事务
来源：http://ac.asd995.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ji.muxihuayi.cn

[U71] PHP：抛出异常
来源：http://av.shtwfgs.cn

throw new RuntimeException("失败", 500);
来源：http://vf.asd995.cn

[U72] PHP：写错误日志
来源：http://nv.wgjwhj.cn

error_log("失败: " . $e->getMessage());
来源：http://vv.huixiangedu.cn

[U73] PHP：读取 ini 配置
来源：http://fn.huanxung.cn

parse_ini_file("config.ini", true)
来源：http://gm.panjiajie.cn

[U74] PHP：读取环境变量
来源：http://fo.jianghongdianzi.cn

getenv("APP_ENV") ?: "production"
来源：http://dp.haigaiapp.cn

[U75] PHP：依赖注入
来源：http://ll.jctech888.com.cn

composer require psr/container
来源：http://ew.wgjwhj.cn

[U76] PHP：简单路由
来源：http://pz.szxytkj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xd.521024.cn

[U77] PHP：模板渲染
来源：http://bl.521024.cn

composer require twig/twig
来源：http://mh.gzmigu.cn

[U78] PHP：单元测试
来源：http://ys.nszjky.cn

composer require --dev phpunit/phpunit
来源：http://oc.521024.cn

[U79] PHP：静态分析
来源：http://vw.nicolike.cn

composer require --dev phpstan/phpstan
来源：http://ds.shtwfgs.cn

[U80] PHP：代码规范修复
来源：http://qi.shtwfgs.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://cm.jianghongdianzi.cn

[U81] JS：初始化项目
来源：http://of.szsharing.cn

npm init -y;  npm i express
来源：http://jf.nszjky.cn

[U82] JS：package.json 脚本
来源：http://ll.jctech888.com.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wb.newstarts.cn

[U83] JS：ES Module 导入导出
来源：http://jq.jianghongdianzi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://hr.huanxung.cn

[U84] JS：CommonJS 写法
来源：http://ed.gzmigu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://jy.yuexingan06.cn

[U85] JS：可选链
来源：http://nr.muxihuayi.cn

a?.b?.c
来源：http://jy.huixinmuqiang.cn

[U86] JS：空值合并
来源：http://hg.nszjky.cn

a ?? b
来源：http://rp.jctech888.com.cn

[U87] JS：解构默认值
来源：http://jc.asd995.cn

const { a = 1, b = 2 } = obj;
来源：http://jc.asd995.cn

[U88] JS：对象展开合并
来源：http://np.shtwfgs.cn

{ ...a, ...b }
来源：http://qd.gzmigu.cn

[U89] JS：数组去重
来源：http://cb.521024.cn

[...new Set(arr)]
来源：http://ar.gzmigu.cn

[U90] JS：数字数组排序
来源：http://ez.jianghongdianzi.cn

[...arr].sort((a, b) => a - b)
来源：http://ls.jianghongdianzi.cn

[U91] JS：对象键值遍历
来源：http://ns.521024.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rz.bookmarksfly.cn

[U92] JS：深拷贝
来源：http://uq.nszjky.cn

structuredClone(obj)
来源：http://or.muxihuayi.cn

[U93] JS：模板字符串
来源：http://qa.shxzukj.cn

`共 ${n} 条`
来源：http://zl.huanxung.cn

[U94] JS：箭头函数
来源：http://vt.hnjuh.cn

const double = x => x * 2;
来源：http://uv.yuexingan06.cn

[U95] JS：Promise 包装
来源：http://os.jianghongdianzi.cn

new Promise((resolve, reject) => {})
来源：http://ag.panjiajie.cn

[U96] JS：async/await 与异常
来源：http://nh.chemitech.net.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ez.gzmigu.cn

[U97] JS：并发请求
来源：http://kd.huixiangedu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://oh.jctech888.com.cn

[U98] JS：fetch 带 JSON
来源：http://ly.huanxung.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://my.szsharing.cn

[U99] JS：事件监听
来源：http://al.huixiangedu.cn

el.addEventListener("click", e => {})
来源：http://si.yuntaijiaju.cn

[U100] JS：DOM 查询
来源：http://qm.szxytkj.cn

document.querySelector(".item")
来源：http://sa.huixinmuqiang.cn

[U101] JS：classList 操作
来源：http://yj.shtwfgs.cn

el.classList.toggle("active")
来源：http://ee.bjjhwx.cn

[U102] JS：本地存储
来源：http://uu.9csxet.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ug.shxzukj.cn

[U103] JS：定时器
来源：http://mj.huixinmuqiang.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zq.asd995.cn

[U104] JS：防抖
来源：http://cj.hahajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qr.huixiangedu.cn

[U105] JS：节流
来源：http://kf.hahajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://io.nicolike.cn

[U106] JS：日期格式化
来源：http://pr.szsharing.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jb.9csxet.cn

[U107] JS：数字千分位
来源：http://ks.muxihuayi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ps.nszjky.cn

[U108] JS：随机整数
来源：http://np.muxihuayi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tc.chemitech.net.cn

[U109] JS：数组分组
来源：http://be.haigaiapp.cn

Object.groupBy(arr, x => x.type)
来源：http://jk.bookmarksfly.cn

[U110] JS：数组分块
来源：http://kn.jctech888.com.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://uu.newstarts.cn

[U111] JS：对象转 Map
来源：http://wj.haigaiapp.cn

new Map(Object.entries(obj))
来源：http://ir.szxytkj.cn

[U112] JS：字符串补位
来源：http://mn.hahajie.cn

"7".padStart(3, "0")
来源：http://la.521024.cn

[U113] JS：正则替换全部
来源：http://or.hahajie.cn

s.replaceAll("a", "b")
来源：http://og.panjiajie.cn

[U114] JS：JSON 深比较
来源：http://vz.szsharing.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vc.muxihuayi.cn

[U115] JS：生成 UUID
来源：http://dg.nicolike.cn

crypto.randomUUID()
来源：http://kw.jianghongdianzi.cn

[U116] JS：类型检查（JSDoc）
来源：http://ol.521024.cn

/** @param {string} name */ function f(name) {}
来源：http://iz.yuexingan06.cn

[U117] JS：单元测试
来源：http://ro.jctech888.com.cn

npm i -D vitest;  npx vitest
来源：http://mg.huanxung.cn

[U118] JS：开发服务器
来源：http://yd.hnjuh.cn

npm i -D vite;  npx vite
来源：http://fv.shtwfgs.cn

[U119] JS：生产构建
来源：http://nv.asd995.cn

npx vite build
来源：http://km.haigaiapp.cn

[U120] JS：读取环境变量（Vite）
来源：http://xn.panjiajie.cn

import.meta.env.VITE_API_URL
来源：http://ch.gzmigu.cn

================================================================================
来源：http://uj.bjjhwx.cn

统计汇总
来源：http://nl.asd995.cn

================================================================================
来源：http://rx.huixiangedu.cn

按语言统计（条）：
来源：http://qq.nszjky.cn

Python ......... 252
来源：http://hv.szsharing.cn

PHP ............ 252
来源：http://ik.jianghongdianzi.cn

JavaScript ..... 252
来源：http://zc.nicolike.cn

TypeScript ..... 212
来源：http://zm.hnjuh.cn

Java ........... 212
来源：http://ii.lnxyls.cn

Go ............. 212
来源：http://oq.nicolike.cn

Ruby ........... 212
来源：http://lb.szsharing.cn

C# ............. 212
来源：http://hg.521024.cn

C .............. 30
来源：http://wb.huanxung.cn

C++ ............ 30
来源：http://sz.hahajie.cn

SQL ............ 90
来源：http://ba.nszjky.cn

Bash ........... 80
来源：http://sk.jianghongdianzi.cn

Kotlin ......... 15
来源：http://zu.shxzskj.cn

Swift .......... 15
来源：http://lx.shtwfgs.cn

Lua ............ 10
来源：http://zb.521024.cn

Perl ........... 10
来源：http://ae.9csxet.cn

Scala .......... 10
来源：http://er.haigaiapp.cn

------------------------------------
来源：http://gf.muxihuayi.cn

合计 ........... 2106 条
来源：http://hs.szxytkj.cn

按章节统计：
来源：http://bs.szxytkj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://im.muxihuayi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ag.szxytkj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hf.bjjhwx.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://tx.hahajie.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wm.haigaiapp.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ru.wgjwhj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xu.521024.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://sq.panjiajie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ni.jctech888.com.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xb.lnxyls.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rm.huanxung.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zo.panjiajie.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wf.9csxet.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kx.yuntaijiaju.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ay.521024.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://sv.wgjwhj.cn

Q SQL 专题                              90
来源：http://ca.panjiajie.cn

R Bash 专题                             80
来源：http://fq.gzmigu.cn

S C / C++ 专题                          60
来源：http://jr.huanxung.cn

T 其他语言补充                          60
来源：http://cj.colortex.cn

U 高频实用片段                         120
来源：http://at.szsharing.cn

------------------------------------
来源：http://ym.huixinmuqiang.cn

合计                                  2106 条
来源：http://ku.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://my.nicolike.cn

使用提醒
来源：http://sb.colortex.cn

--------------------------------------------------------------------------------
来源：http://gl.bookmarksfly.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rs.wgjwhj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ql.yuntaijiaju.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gu.muxihuayi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://gs.yuntaijiaju.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mp.szxytkj.cn

—— 文件结束 ——
来源：http://hg.jctech888.com.cn


<!-- 参考信息 -->