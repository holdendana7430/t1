代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hs.hnjuh.cn

================================================================================
来源：http://hl.wgjwhj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://le.yuntaijiaju.cn

================================================================================
来源：http://kf.yuexingan06.cn

[U01] Py：创建虚拟环境
来源：http://fo.panjiajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://yo.huixiangedu.cn

[U02] Py：导出 / 安装依赖
来源：http://bn.jianghongdianzi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fh.asd995.cn

[U03] Py：加载 .env 配置
来源：http://nu.huanxung.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ch.szsharing.cn

[U04] Py：变量调试打印
来源：http://xa.huixiangedu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hd.szsharing.cn

[U05] Py：列表去重且保序
来源：http://to.muxihuayi.cn

list(dict.fromkeys(arr))
来源：http://ei.nicolike.cn

[U06] Py：合并两个字典
来源：http://ry.szsharing.cn

{**a, **b}
来源：http://jn.9csxet.cn

[U07] Py：反转字典键值
来源：http://fr.hahajie.cn

{v: k for k, v in d.items()}
来源：http://wp.huixinmuqiang.cn

[U08] Py：展平二维列表
来源：http://rm.haigaiapp.cn

[y for x in nested for y in x]
来源：http://hq.521024.cn

[U09] Py：字典取最大值的键
来源：http://zc.yuntaijiaju.cn

max(d, key=d.get)
来源：http://kx.9csxet.cn

[U10] Py：按值排序字典
来源：http://uf.haigaiapp.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wo.huanxung.cn

[U11] Py：生成器表达式
来源：http://hn.hnjuh.cn

(x * 2 for x in arr)
来源：http://nf.hnjuh.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rq.huixiangedu.cn

Counter(arr).most_common(3)
来源：http://sx.asd995.cn

[U13] Py：固定长度队列
来源：http://vs.gzmigu.cn

deque(maxlen=10)
来源：http://po.newstarts.cn

[U14] Py：分组收集到列表
来源：http://se.asd995.cn

defaultdict(list)
来源：http://xi.huixiangedu.cn

[U15] Py：高精度计时
来源：http://zo.huanxung.cn

t = time.perf_counter()
来源：http://cu.haigaiapp.cn

[U16] Py：命令行参数解析
来源：http://iy.haigaiapp.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ih.lnxyls.cn

[U17] Py：初始化日志
来源：http://fo.jctech888.com.cn

logging.basicConfig(level=logging.INFO)
来源：http://bc.panjiajie.cn

[U18] Py：预编译正则
来源：http://af.gzmigu.cn

pat = re.compile(r"\d+")
来源：http://nx.gzmigu.cn

[U19] Py：正则替换带回调
来源：http://ta.9csxet.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bk.bookmarksfly.cn

[U20] Py：缓存函数结果
来源：http://zq.jianghongdianzi.cn

@functools.lru_cache(maxsize=None)
来源：http://zi.gzmigu.cn

[U21] Py：自定义上下文管理器
来源：http://nh.shxzskj.cn

@contextlib.contextmanager
来源：http://cb.521024.cn

[U22] Py：矩阵转置
来源：http://jk.colortex.cn

list(zip(*m))
来源：http://pm.colortex.cn

[U23] Py：分块读取大文件
来源：http://yd.lnxyls.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gq.huixinmuqiang.cn

[U24] Py：路径操作
来源：http://cs.haigaiapp.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nn.yuexingan06.cn

[U25] Py：CSV 按字典读
来源：http://sv.muxihuayi.cn

csv.DictReader(f)
来源：http://ly.colortex.cn

[U26] Py：并发下载
来源：http://sr.bjjhwx.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ok.nicolike.cn

[U27] Py：异步 HTTP
来源：http://ht.gzmigu.cn

aiohttp.ClientSession() 配合 async with
来源：http://eo.yuntaijiaju.cn

[U28] Py：类型别名
来源：http://bs.huixinmuqiang.cn

UserId = int
来源：http://xz.chemitech.net.cn

[U29] Py：属性校验
来源：http://yi.gzmigu.cn

@property 与 @x.setter 配合
来源：http://zt.newstarts.cn

[U30] Py：数据类
来源：http://rg.shtwfgs.cn

@dataclass(slots=True)
来源：http://ju.huanxung.cn

[U31] Py：单测
来源：http://uq.newstarts.cn

python -m pytest -q
来源：http://vl.jianghongdianzi.cn

[U32] Py：代码格式化
来源：http://sg.haigaiapp.cn

ruff format . && ruff check --fix .
来源：http://em.jctech888.com.cn

[U33] Py：打包发布
来源：http://gm.bookmarksfly.cn

python -m build  （依赖 pyproject.toml）
来源：http://fq.nszjky.cn

[U34] Py：判断编码
来源：http://gp.colortex.cn

chardet.detect(raw)
来源：http://hd.nszjky.cn

[U35] Py：发送邮件
来源：http://wf.chemitech.net.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hv.shxzskj.cn

[U36] Py：定时任务
来源：http://uf.yuntaijiaju.cn

schedule.every(10).minutes.do(job)
来源：http://ig.bjjhwx.cn

[U37] Py：读写 Excel
来源：http://xh.huixiangedu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qt.szxytkj.cn

[U38] Py：获取脚本所在目录
来源：http://ly.jctech888.com.cn

Path(__file__).resolve().parent
来源：http://xf.huixinmuqiang.cn

[U39] Py：判断是否在交互环境
来源：http://mo.bookmarksfly.cn

sys.stdout.isatty()
来源：http://zd.bookmarksfly.cn

[U40] Py：打印到标准错误
来源：http://mx.nicolike.cn

print("err", file=sys.stderr)
来源：http://yn.gzmigu.cn

[U41] PHP：初始化 Composer 项目
来源：http://wu.haigaiapp.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://np.521024.cn

[U42] PHP：PSR-4 自动加载
来源：http://sk.haigaiapp.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yl.asd995.cn

[U43] PHP：声明命名空间
来源：http://wc.bjjhwx.cn

namespace App\Http;
来源：http://oc.huanxung.cn

[U44] PHP：开启严格类型
来源：http://iz.shxzukj.cn

declare(strict_types=1);
来源：http://ev.haigaiapp.cn

[U45] PHP：类型声明与返回类型
来源：http://sp.muxihuayi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qp.521024.cn

[U46] PHP：可空类型
来源：http://kt.lnxyls.cn

?string $name = null
来源：http://xx.huixiangedu.cn

[U47] PHP：联合类型
来源：http://yz.szxytkj.cn

int|string $id
来源：http://vx.muxihuayi.cn

[U48] PHP：纯枚举
来源：http://ud.hahajie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fm.521024.cn

[U49] PHP：只读属性
来源：http://jf.wgjwhj.cn

public readonly string $name
来源：http://av.huixiangedu.cn

[U50] PHP：构造器属性提升
来源：http://fd.asd995.cn

public function __construct(private int $id) {}
来源：http://dw.521024.cn

[U51] PHP：数组解构
来源：http://oh.gzmigu.cn

[$a, $b] = $arr;
来源：http://ck.lnxyls.cn

[U52] PHP：箭头函数
来源：http://es.shtwfgs.cn

$double = fn($x) => $x * 2;
来源：http://qo.huanxung.cn

[U53] PHP：空合并运算符
来源：http://oj.huixiangedu.cn

$v = $a ?? $b ?? "default";
来源：http://wf.haigaiapp.cn

[U54] PHP：空安全调用
来源：http://ux.yuntaijiaju.cn

$obj?->method()
来源：http://eb.chemitech.net.cn

[U55] PHP：match 表达式
来源：http://aw.jctech888.com.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cl.bjjhwx.cn

[U56] PHP：命名参数
来源：http://ij.wgjwhj.cn

f(a: 1, b: 2)
来源：http://vb.bjjhwx.cn

[U57] PHP：字符串插值
来源：http://bq.jianghongdianzi.cn

"值: {$a}"
来源：http://ah.shxzukj.cn

[U58] PHP：数组三件套
来源：http://la.lnxyls.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://so.szxytkj.cn

[U59] PHP：自定义排序
来源：http://pm.huixiangedu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rq.yuntaijiaju.cn

[U60] PHP：JSON 编解码
来源：http://bk.chemitech.net.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ji.yuexingan06.cn

[U61] PHP：正则
来源：http://om.bookmarksfly.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qd.bjjhwx.cn

[U62] PHP：日期对象
来源：http://qt.521024.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kd.muxihuayi.cn

[U63] PHP：文件读写
来源：http://oz.bookmarksfly.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vf.huixinmuqiang.cn

[U64] PHP：目录遍历
来源：http://vm.asd995.cn

glob("dir/*.php");  scandir("dir");
来源：http://qn.szxytkj.cn

[U65] PHP：会话
来源：http://dd.huanxung.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://xn.bookmarksfly.cn

[U66] PHP：设置 Cookie
来源：http://zn.jianghongdianzi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ud.nicolike.cn

[U67] PHP：处理文件上传
来源：http://ql.newstarts.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nd.hnjuh.cn

[U68] PHP：PDO 连接
来源：http://zi.szxytkj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wp.9csxet.cn

[U69] PHP：PDO 预处理
来源：http://ai.muxihuayi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ci.shxzukj.cn

[U70] PHP：PDO 事务
来源：http://zo.shtwfgs.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://or.muxihuayi.cn

[U71] PHP：抛出异常
来源：http://xr.jctech888.com.cn

throw new RuntimeException("失败", 500);
来源：http://gq.shxzskj.cn

[U72] PHP：写错误日志
来源：http://pf.wgjwhj.cn

error_log("失败: " . $e->getMessage());
来源：http://rk.nicolike.cn

[U73] PHP：读取 ini 配置
来源：http://zr.bjjhwx.cn

parse_ini_file("config.ini", true)
来源：http://ei.panjiajie.cn

[U74] PHP：读取环境变量
来源：http://pn.yuexingan06.cn

getenv("APP_ENV") ?: "production"
来源：http://gd.huixinmuqiang.cn

[U75] PHP：依赖注入
来源：http://yc.9csxet.cn

composer require psr/container
来源：http://yz.huixiangedu.cn

[U76] PHP：简单路由
来源：http://vp.bjjhwx.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://da.asd995.cn

[U77] PHP：模板渲染
来源：http://zu.chemitech.net.cn

composer require twig/twig
来源：http://ty.szsharing.cn

[U78] PHP：单元测试
来源：http://le.nszjky.cn

composer require --dev phpunit/phpunit
来源：http://xq.huixinmuqiang.cn

[U79] PHP：静态分析
来源：http://ka.hnjuh.cn

composer require --dev phpstan/phpstan
来源：http://bp.colortex.cn

[U80] PHP：代码规范修复
来源：http://uf.szxytkj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://cz.9csxet.cn

[U81] JS：初始化项目
来源：http://nv.huixiangedu.cn

npm init -y;  npm i express
来源：http://oy.hahajie.cn

[U82] JS：package.json 脚本
来源：http://rz.jctech888.com.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xz.521024.cn

[U83] JS：ES Module 导入导出
来源：http://sr.jianghongdianzi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://cr.hnjuh.cn

[U84] JS：CommonJS 写法
来源：http://nf.nicolike.cn

module.exports = { a };  const { a } = require("./m");
来源：http://vb.yuexingan06.cn

[U85] JS：可选链
来源：http://rh.521024.cn

a?.b?.c
来源：http://rs.szsharing.cn

[U86] JS：空值合并
来源：http://is.521024.cn

a ?? b
来源：http://lk.colortex.cn

[U87] JS：解构默认值
来源：http://ej.9csxet.cn

const { a = 1, b = 2 } = obj;
来源：http://er.wgjwhj.cn

[U88] JS：对象展开合并
来源：http://rg.panjiajie.cn

{ ...a, ...b }
来源：http://vo.9csxet.cn

[U89] JS：数组去重
来源：http://la.521024.cn

[...new Set(arr)]
来源：http://de.chemitech.net.cn

[U90] JS：数字数组排序
来源：http://it.nszjky.cn

[...arr].sort((a, b) => a - b)
来源：http://km.shtwfgs.cn

[U91] JS：对象键值遍历
来源：http://sj.chemitech.net.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ly.nicolike.cn

[U92] JS：深拷贝
来源：http://rw.bjjhwx.cn

structuredClone(obj)
来源：http://mk.nicolike.cn

[U93] JS：模板字符串
来源：http://ge.yuexingan06.cn

`共 ${n} 条`
来源：http://yi.asd995.cn

[U94] JS：箭头函数
来源：http://yr.colortex.cn

const double = x => x * 2;
来源：http://ur.hnjuh.cn

[U95] JS：Promise 包装
来源：http://ts.521024.cn

new Promise((resolve, reject) => {})
来源：http://jy.szxytkj.cn

[U96] JS：async/await 与异常
来源：http://ue.huixinmuqiang.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hg.wgjwhj.cn

[U97] JS：并发请求
来源：http://vq.colortex.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bz.yuntaijiaju.cn

[U98] JS：fetch 带 JSON
来源：http://di.haigaiapp.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tv.shxzukj.cn

[U99] JS：事件监听
来源：http://ss.wgjwhj.cn

el.addEventListener("click", e => {})
来源：http://ws.huixiangedu.cn

[U100] JS：DOM 查询
来源：http://ea.newstarts.cn

document.querySelector(".item")
来源：http://jq.9csxet.cn

[U101] JS：classList 操作
来源：http://pe.521024.cn

el.classList.toggle("active")
来源：http://zu.yuexingan06.cn

[U102] JS：本地存储
来源：http://xd.9csxet.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ir.hnjuh.cn

[U103] JS：定时器
来源：http://be.bjjhwx.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://sp.521024.cn

[U104] JS：防抖
来源：http://gm.jctech888.com.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nx.szsharing.cn

[U105] JS：节流
来源：http://li.shtwfgs.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wn.chemitech.net.cn

[U106] JS：日期格式化
来源：http://gs.huixinmuqiang.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kp.panjiajie.cn

[U107] JS：数字千分位
来源：http://ez.szxytkj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cf.hahajie.cn

[U108] JS：随机整数
来源：http://fb.panjiajie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://td.521024.cn

[U109] JS：数组分组
来源：http://db.muxihuayi.cn

Object.groupBy(arr, x => x.type)
来源：http://jw.yuexingan06.cn

[U110] JS：数组分块
来源：http://xt.wgjwhj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zy.hnjuh.cn

[U111] JS：对象转 Map
来源：http://dh.jctech888.com.cn

new Map(Object.entries(obj))
来源：http://lu.shtwfgs.cn

[U112] JS：字符串补位
来源：http://jp.9csxet.cn

"7".padStart(3, "0")
来源：http://qp.yuntaijiaju.cn

[U113] JS：正则替换全部
来源：http://qm.lnxyls.cn

s.replaceAll("a", "b")
来源：http://qq.wgjwhj.cn

[U114] JS：JSON 深比较
来源：http://pb.jianghongdianzi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ep.jianghongdianzi.cn

[U115] JS：生成 UUID
来源：http://va.gzmigu.cn

crypto.randomUUID()
来源：http://sd.bjjhwx.cn

[U116] JS：类型检查（JSDoc）
来源：http://gy.lnxyls.cn

/** @param {string} name */ function f(name) {}
来源：http://bh.nicolike.cn

[U117] JS：单元测试
来源：http://hi.nicolike.cn

npm i -D vitest;  npx vitest
来源：http://qv.szsharing.cn

[U118] JS：开发服务器
来源：http://ao.bjjhwx.cn

npm i -D vite;  npx vite
来源：http://is.bjjhwx.cn

[U119] JS：生产构建
来源：http://uu.shtwfgs.cn

npx vite build
来源：http://os.nszjky.cn

[U120] JS：读取环境变量（Vite）
来源：http://vw.yuexingan06.cn

import.meta.env.VITE_API_URL
来源：http://ly.nszjky.cn

================================================================================
来源：http://bu.shtwfgs.cn

统计汇总
来源：http://pz.asd995.cn

================================================================================
来源：http://cv.colortex.cn

按语言统计（条）：
来源：http://ln.hahajie.cn

Python ......... 252
来源：http://eg.yuntaijiaju.cn

PHP ............ 252
来源：http://en.asd995.cn

JavaScript ..... 252
来源：http://jo.hahajie.cn

TypeScript ..... 212
来源：http://sy.szxytkj.cn

Java ........... 212
来源：http://pd.yuexingan06.cn

Go ............. 212
来源：http://ez.nicolike.cn

Ruby ........... 212
来源：http://zx.huixinmuqiang.cn

C# ............. 212
来源：http://ao.szsharing.cn

C .............. 30
来源：http://rg.huanxung.cn

C++ ............ 30
来源：http://zs.hnjuh.cn

SQL ............ 90
来源：http://vp.9csxet.cn

Bash ........... 80
来源：http://yc.newstarts.cn

Kotlin ......... 15
来源：http://vd.szsharing.cn

Swift .......... 15
来源：http://vf.panjiajie.cn

Lua ............ 10
来源：http://nw.huixiangedu.cn

Perl ........... 10
来源：http://uh.hahajie.cn

Scala .......... 10
来源：http://ls.nszjky.cn

------------------------------------
来源：http://io.lnxyls.cn

合计 ........... 2106 条
来源：http://fh.szxytkj.cn

按章节统计：
来源：http://ol.asd995.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ha.nicolike.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xc.hahajie.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mq.521024.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ae.huixiangedu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xf.huixinmuqiang.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://eb.chemitech.net.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://eo.9csxet.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://da.521024.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vf.asd995.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xx.haigaiapp.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://uk.huixiangedu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gu.jctech888.com.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nh.nicolike.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hy.yuexingan06.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ty.521024.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ry.huanxung.cn

Q SQL 专题                              90
来源：http://ks.nicolike.cn

R Bash 专题                             80
来源：http://jh.gzmigu.cn

S C / C++ 专题                          60
来源：http://wa.panjiajie.cn

T 其他语言补充                          60
来源：http://ra.jianghongdianzi.cn

U 高频实用片段                         120
来源：http://fu.bookmarksfly.cn

------------------------------------
来源：http://aq.yuexingan06.cn

合计                                  2106 条
来源：http://ie.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://il.nszjky.cn

使用提醒
来源：http://jn.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://zn.huanxung.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://pr.huixinmuqiang.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vj.muxihuayi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://je.newstarts.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://zx.shtwfgs.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gn.huixiangedu.cn

—— 文件结束 ——
来源：http://ew.521024.cn


<!-- 参考信息 -->