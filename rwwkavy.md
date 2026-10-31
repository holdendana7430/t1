代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kl.hnjuh.cn

================================================================================
来源：http://ar.szxytkj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ln.panjiajie.cn

================================================================================
来源：http://bg.jctech888.com.cn

[U01] Py：创建虚拟环境
来源：http://es.yuexingan06.cn

python -m venv .venv && source .venv/bin/activate
来源：http://fu.shxzskj.cn

[U02] Py：导出 / 安装依赖
来源：http://ox.shtwfgs.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wx.huixiangedu.cn

[U03] Py：加载 .env 配置
来源：http://ft.shxzukj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://tk.hnjuh.cn

[U04] Py：变量调试打印
来源：http://yj.szxytkj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qe.yuexingan06.cn

[U05] Py：列表去重且保序
来源：http://yd.huixiangedu.cn

list(dict.fromkeys(arr))
来源：http://qt.wgjwhj.cn

[U06] Py：合并两个字典
来源：http://du.nszjky.cn

{**a, **b}
来源：http://ek.newstarts.cn

[U07] Py：反转字典键值
来源：http://oc.hahajie.cn

{v: k for k, v in d.items()}
来源：http://jq.huixinmuqiang.cn

[U08] Py：展平二维列表
来源：http://kc.nicolike.cn

[y for x in nested for y in x]
来源：http://xw.panjiajie.cn

[U09] Py：字典取最大值的键
来源：http://xv.shxzukj.cn

max(d, key=d.get)
来源：http://mh.9csxet.cn

[U10] Py：按值排序字典
来源：http://hu.wgjwhj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jp.colortex.cn

[U11] Py：生成器表达式
来源：http://qm.nszjky.cn

(x * 2 for x in arr)
来源：http://ax.jianghongdianzi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mz.521024.cn

Counter(arr).most_common(3)
来源：http://ki.yuexingan06.cn

[U13] Py：固定长度队列
来源：http://cm.jctech888.com.cn

deque(maxlen=10)
来源：http://vi.jctech888.com.cn

[U14] Py：分组收集到列表
来源：http://mx.shtwfgs.cn

defaultdict(list)
来源：http://ew.jctech888.com.cn

[U15] Py：高精度计时
来源：http://rb.shxzskj.cn

t = time.perf_counter()
来源：http://ct.chemitech.net.cn

[U16] Py：命令行参数解析
来源：http://ld.colortex.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pw.9csxet.cn

[U17] Py：初始化日志
来源：http://du.huixiangedu.cn

logging.basicConfig(level=logging.INFO)
来源：http://ab.shtwfgs.cn

[U18] Py：预编译正则
来源：http://ne.hahajie.cn

pat = re.compile(r"\d+")
来源：http://fo.gzmigu.cn

[U19] Py：正则替换带回调
来源：http://mb.chemitech.net.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://an.szsharing.cn

[U20] Py：缓存函数结果
来源：http://rh.shxzukj.cn

@functools.lru_cache(maxsize=None)
来源：http://ap.bookmarksfly.cn

[U21] Py：自定义上下文管理器
来源：http://gl.jianghongdianzi.cn

@contextlib.contextmanager
来源：http://vg.huixiangedu.cn

[U22] Py：矩阵转置
来源：http://oz.szsharing.cn

list(zip(*m))
来源：http://ik.huixinmuqiang.cn

[U23] Py：分块读取大文件
来源：http://mk.szsharing.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gs.nicolike.cn

[U24] Py：路径操作
来源：http://eo.shtwfgs.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nh.huixiangedu.cn

[U25] Py：CSV 按字典读
来源：http://qw.panjiajie.cn

csv.DictReader(f)
来源：http://hv.huixinmuqiang.cn

[U26] Py：并发下载
来源：http://kz.hnjuh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ib.shxzskj.cn

[U27] Py：异步 HTTP
来源：http://pr.lnxyls.cn

aiohttp.ClientSession() 配合 async with
来源：http://ae.szxytkj.cn

[U28] Py：类型别名
来源：http://kr.jctech888.com.cn

UserId = int
来源：http://xx.panjiajie.cn

[U29] Py：属性校验
来源：http://tu.wgjwhj.cn

@property 与 @x.setter 配合
来源：http://ur.panjiajie.cn

[U30] Py：数据类
来源：http://wf.lnxyls.cn

@dataclass(slots=True)
来源：http://kv.chemitech.net.cn

[U31] Py：单测
来源：http://il.wgjwhj.cn

python -m pytest -q
来源：http://sl.gzmigu.cn

[U32] Py：代码格式化
来源：http://yt.szsharing.cn

ruff format . && ruff check --fix .
来源：http://bc.shxzskj.cn

[U33] Py：打包发布
来源：http://jk.asd995.cn

python -m build  （依赖 pyproject.toml）
来源：http://nh.yuntaijiaju.cn

[U34] Py：判断编码
来源：http://ux.newstarts.cn

chardet.detect(raw)
来源：http://uz.521024.cn

[U35] Py：发送邮件
来源：http://xo.shxzukj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dz.nicolike.cn

[U36] Py：定时任务
来源：http://rj.colortex.cn

schedule.every(10).minutes.do(job)
来源：http://ul.shtwfgs.cn

[U37] Py：读写 Excel
来源：http://gv.hahajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ul.asd995.cn

[U38] Py：获取脚本所在目录
来源：http://ls.haigaiapp.cn

Path(__file__).resolve().parent
来源：http://da.hnjuh.cn

[U39] Py：判断是否在交互环境
来源：http://bc.yuexingan06.cn

sys.stdout.isatty()
来源：http://la.yuntaijiaju.cn

[U40] Py：打印到标准错误
来源：http://tp.wgjwhj.cn

print("err", file=sys.stderr)
来源：http://ug.muxihuayi.cn

[U41] PHP：初始化 Composer 项目
来源：http://bv.gzmigu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://dc.colortex.cn

[U42] PHP：PSR-4 自动加载
来源：http://qs.newstarts.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://la.hahajie.cn

[U43] PHP：声明命名空间
来源：http://vz.bookmarksfly.cn

namespace App\Http;
来源：http://ec.colortex.cn

[U44] PHP：开启严格类型
来源：http://fw.nicolike.cn

declare(strict_types=1);
来源：http://au.huanxung.cn

[U45] PHP：类型声明与返回类型
来源：http://ch.lnxyls.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://lr.yuntaijiaju.cn

[U46] PHP：可空类型
来源：http://iv.colortex.cn

?string $name = null
来源：http://ds.haigaiapp.cn

[U47] PHP：联合类型
来源：http://px.szsharing.cn

int|string $id
来源：http://ug.huanxung.cn

[U48] PHP：纯枚举
来源：http://wh.szsharing.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://if.hahajie.cn

[U49] PHP：只读属性
来源：http://ox.panjiajie.cn

public readonly string $name
来源：http://fi.huanxung.cn

[U50] PHP：构造器属性提升
来源：http://tl.bjjhwx.cn

public function __construct(private int $id) {}
来源：http://qe.chemitech.net.cn

[U51] PHP：数组解构
来源：http://yj.bjjhwx.cn

[$a, $b] = $arr;
来源：http://gc.huixiangedu.cn

[U52] PHP：箭头函数
来源：http://cw.nszjky.cn

$double = fn($x) => $x * 2;
来源：http://ak.lnxyls.cn

[U53] PHP：空合并运算符
来源：http://xx.yuexingan06.cn

$v = $a ?? $b ?? "default";
来源：http://hh.bookmarksfly.cn

[U54] PHP：空安全调用
来源：http://yw.huanxung.cn

$obj?->method()
来源：http://sm.szxytkj.cn

[U55] PHP：match 表达式
来源：http://ct.jianghongdianzi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://sg.hnjuh.cn

[U56] PHP：命名参数
来源：http://as.huixinmuqiang.cn

f(a: 1, b: 2)
来源：http://sr.gzmigu.cn

[U57] PHP：字符串插值
来源：http://rk.yuntaijiaju.cn

"值: {$a}"
来源：http://qh.nszjky.cn

[U58] PHP：数组三件套
来源：http://zd.521024.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://iw.gzmigu.cn

[U59] PHP：自定义排序
来源：http://zw.yuexingan06.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oz.hahajie.cn

[U60] PHP：JSON 编解码
来源：http://up.hnjuh.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ro.9csxet.cn

[U61] PHP：正则
来源：http://ji.jctech888.com.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xg.newstarts.cn

[U62] PHP：日期对象
来源：http://bj.colortex.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rf.huanxung.cn

[U63] PHP：文件读写
来源：http://sw.huixinmuqiang.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jh.wgjwhj.cn

[U64] PHP：目录遍历
来源：http://lr.9csxet.cn

glob("dir/*.php");  scandir("dir");
来源：http://ch.huanxung.cn

[U65] PHP：会话
来源：http://gp.jctech888.com.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://jj.yuexingan06.cn

[U66] PHP：设置 Cookie
来源：http://fo.szsharing.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://el.huixiangedu.cn

[U67] PHP：处理文件上传
来源：http://mq.asd995.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://il.huixinmuqiang.cn

[U68] PHP：PDO 连接
来源：http://lz.szxytkj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://iz.hahajie.cn

[U69] PHP：PDO 预处理
来源：http://vk.huanxung.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qf.chemitech.net.cn

[U70] PHP：PDO 事务
来源：http://bb.shtwfgs.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kn.shxzskj.cn

[U71] PHP：抛出异常
来源：http://qy.newstarts.cn

throw new RuntimeException("失败", 500);
来源：http://ol.hnjuh.cn

[U72] PHP：写错误日志
来源：http://xh.yuntaijiaju.cn

error_log("失败: " . $e->getMessage());
来源：http://so.9csxet.cn

[U73] PHP：读取 ini 配置
来源：http://vd.jctech888.com.cn

parse_ini_file("config.ini", true)
来源：http://ir.lnxyls.cn

[U74] PHP：读取环境变量
来源：http://qv.nicolike.cn

getenv("APP_ENV") ?: "production"
来源：http://bq.lnxyls.cn

[U75] PHP：依赖注入
来源：http://bc.shxzskj.cn

composer require psr/container
来源：http://qb.muxihuayi.cn

[U76] PHP：简单路由
来源：http://th.asd995.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://uf.szxytkj.cn

[U77] PHP：模板渲染
来源：http://zh.szxytkj.cn

composer require twig/twig
来源：http://qg.hahajie.cn

[U78] PHP：单元测试
来源：http://lz.colortex.cn

composer require --dev phpunit/phpunit
来源：http://il.wgjwhj.cn

[U79] PHP：静态分析
来源：http://kv.bookmarksfly.cn

composer require --dev phpstan/phpstan
来源：http://pi.shxzskj.cn

[U80] PHP：代码规范修复
来源：http://rs.szsharing.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://sx.lnxyls.cn

[U81] JS：初始化项目
来源：http://yr.shxzskj.cn

npm init -y;  npm i express
来源：http://vq.bookmarksfly.cn

[U82] JS：package.json 脚本
来源：http://cj.shxzukj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cg.huanxung.cn

[U83] JS：ES Module 导入导出
来源：http://fx.9csxet.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zg.9csxet.cn

[U84] JS：CommonJS 写法
来源：http://mr.lnxyls.cn

module.exports = { a };  const { a } = require("./m");
来源：http://cx.szxytkj.cn

[U85] JS：可选链
来源：http://cm.nszjky.cn

a?.b?.c
来源：http://ao.hnjuh.cn

[U86] JS：空值合并
来源：http://gt.yuexingan06.cn

a ?? b
来源：http://dl.shxzukj.cn

[U87] JS：解构默认值
来源：http://pa.szsharing.cn

const { a = 1, b = 2 } = obj;
来源：http://fr.asd995.cn

[U88] JS：对象展开合并
来源：http://fa.huanxung.cn

{ ...a, ...b }
来源：http://cb.huixinmuqiang.cn

[U89] JS：数组去重
来源：http://ck.panjiajie.cn

[...new Set(arr)]
来源：http://pb.huanxung.cn

[U90] JS：数字数组排序
来源：http://gr.shxzskj.cn

[...arr].sort((a, b) => a - b)
来源：http://xj.9csxet.cn

[U91] JS：对象键值遍历
来源：http://pw.yuexingan06.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://da.9csxet.cn

[U92] JS：深拷贝
来源：http://hy.asd995.cn

structuredClone(obj)
来源：http://kc.jianghongdianzi.cn

[U93] JS：模板字符串
来源：http://cu.lnxyls.cn

`共 ${n} 条`
来源：http://xh.colortex.cn

[U94] JS：箭头函数
来源：http://sl.nicolike.cn

const double = x => x * 2;
来源：http://nf.nicolike.cn

[U95] JS：Promise 包装
来源：http://wr.szxytkj.cn

new Promise((resolve, reject) => {})
来源：http://in.shxzukj.cn

[U96] JS：async/await 与异常
来源：http://fl.hahajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gl.chemitech.net.cn

[U97] JS：并发请求
来源：http://ji.9csxet.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://yu.yuexingan06.cn

[U98] JS：fetch 带 JSON
来源：http://gn.521024.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jd.bookmarksfly.cn

[U99] JS：事件监听
来源：http://fe.chemitech.net.cn

el.addEventListener("click", e => {})
来源：http://lb.colortex.cn

[U100] JS：DOM 查询
来源：http://vj.muxihuayi.cn

document.querySelector(".item")
来源：http://yq.gzmigu.cn

[U101] JS：classList 操作
来源：http://qf.chemitech.net.cn

el.classList.toggle("active")
来源：http://zj.gzmigu.cn

[U102] JS：本地存储
来源：http://wj.asd995.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ap.haigaiapp.cn

[U103] JS：定时器
来源：http://rj.shxzskj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://eh.shtwfgs.cn

[U104] JS：防抖
来源：http://wm.szxytkj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qa.asd995.cn

[U105] JS：节流
来源：http://ub.jianghongdianzi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://iz.lnxyls.cn

[U106] JS：日期格式化
来源：http://ye.asd995.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xk.nszjky.cn

[U107] JS：数字千分位
来源：http://yt.nicolike.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ak.yuntaijiaju.cn

[U108] JS：随机整数
来源：http://wk.521024.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kn.yuntaijiaju.cn

[U109] JS：数组分组
来源：http://ui.gzmigu.cn

Object.groupBy(arr, x => x.type)
来源：http://et.shtwfgs.cn

[U110] JS：数组分块
来源：http://ur.wgjwhj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://po.bookmarksfly.cn

[U111] JS：对象转 Map
来源：http://qp.newstarts.cn

new Map(Object.entries(obj))
来源：http://zl.huixiangedu.cn

[U112] JS：字符串补位
来源：http://hj.szxytkj.cn

"7".padStart(3, "0")
来源：http://hp.bookmarksfly.cn

[U113] JS：正则替换全部
来源：http://kj.colortex.cn

s.replaceAll("a", "b")
来源：http://fb.hnjuh.cn

[U114] JS：JSON 深比较
来源：http://tw.yuntaijiaju.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vv.jianghongdianzi.cn

[U115] JS：生成 UUID
来源：http://tx.muxihuayi.cn

crypto.randomUUID()
来源：http://yc.haigaiapp.cn

[U116] JS：类型检查（JSDoc）
来源：http://vd.yuexingan06.cn

/** @param {string} name */ function f(name) {}
来源：http://vs.szxytkj.cn

[U117] JS：单元测试
来源：http://mh.huanxung.cn

npm i -D vitest;  npx vitest
来源：http://wl.yuexingan06.cn

[U118] JS：开发服务器
来源：http://uz.jctech888.com.cn

npm i -D vite;  npx vite
来源：http://ng.haigaiapp.cn

[U119] JS：生产构建
来源：http://av.nicolike.cn

npx vite build
来源：http://xc.huixiangedu.cn

[U120] JS：读取环境变量（Vite）
来源：http://td.bjjhwx.cn

import.meta.env.VITE_API_URL
来源：http://nj.gzmigu.cn

================================================================================
来源：http://zj.wgjwhj.cn

统计汇总
来源：http://ku.shxzukj.cn

================================================================================
来源：http://xc.shxzskj.cn

按语言统计（条）：
来源：http://zy.shxzskj.cn

Python ......... 252
来源：http://ir.huixinmuqiang.cn

PHP ............ 252
来源：http://vs.haigaiapp.cn

JavaScript ..... 252
来源：http://xm.hahajie.cn

TypeScript ..... 212
来源：http://mb.shtwfgs.cn

Java ........... 212
来源：http://es.wgjwhj.cn

Go ............. 212
来源：http://wi.nicolike.cn

Ruby ........... 212
来源：http://dt.9csxet.cn

C# ............. 212
来源：http://fm.bookmarksfly.cn

C .............. 30
来源：http://kk.shxzukj.cn

C++ ............ 30
来源：http://fz.gzmigu.cn

SQL ............ 90
来源：http://lh.yuexingan06.cn

Bash ........... 80
来源：http://sx.jianghongdianzi.cn

Kotlin ......... 15
来源：http://sh.jctech888.com.cn

Swift .......... 15
来源：http://yy.chemitech.net.cn

Lua ............ 10
来源：http://kg.yuntaijiaju.cn

Perl ........... 10
来源：http://en.huixinmuqiang.cn

Scala .......... 10
来源：http://ui.muxihuayi.cn

------------------------------------
来源：http://qd.panjiajie.cn

合计 ........... 2106 条
来源：http://kl.yuntaijiaju.cn

按章节统计：
来源：http://xu.nicolike.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zz.nszjky.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dl.lnxyls.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ds.gzmigu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://si.shtwfgs.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ey.gzmigu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zk.hahajie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fd.panjiajie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qe.jianghongdianzi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pe.jctech888.com.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yh.huanxung.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bp.hnjuh.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cy.colortex.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://sk.jctech888.com.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pm.shxzukj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ye.haigaiapp.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wn.szsharing.cn

Q SQL 专题                              90
来源：http://rc.haigaiapp.cn

R Bash 专题                             80
来源：http://df.haigaiapp.cn

S C / C++ 专题                          60
来源：http://zy.muxihuayi.cn

T 其他语言补充                          60
来源：http://vc.jctech888.com.cn

U 高频实用片段                         120
来源：http://ql.huixinmuqiang.cn

------------------------------------
来源：http://ks.hnjuh.cn

合计                                  2106 条
来源：http://wq.nszjky.cn

--------------------------------------------------------------------------------
来源：http://ml.chemitech.net.cn

使用提醒
来源：http://cc.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://iu.nicolike.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lf.521024.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ij.hahajie.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ua.hnjuh.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://gw.huanxung.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kr.shxzskj.cn

—— 文件结束 ——
来源：http://pf.9csxet.cn


<!-- 参考信息 -->