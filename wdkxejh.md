代发 wailian999

[U19] Py：正则替换带回调
来源：http://sy.szsharing.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fl.newstarts.cn

[U20] Py：缓存函数结果
来源：http://gy.hnjuh.cn

@functools.lru_cache(maxsize=None)
来源：http://as.szsharing.cn

[U21] Py：自定义上下文管理器
来源：http://vp.9csxet.cn

@contextlib.contextmanager
来源：http://sv.newstarts.cn

[U22] Py：矩阵转置
来源：http://lv.muxihuayi.cn

list(zip(*m))
来源：http://ky.yuexingan06.cn

[U23] Py：分块读取大文件
来源：http://ja.huanxung.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://of.hahajie.cn

[U24] Py：路径操作
来源：http://gj.jianghongdianzi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bu.gzmigu.cn

[U25] Py：CSV 按字典读
来源：http://wk.shxzskj.cn

csv.DictReader(f)
来源：http://wg.shxzskj.cn

[U26] Py：并发下载
来源：http://nb.szsharing.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bp.shxzukj.cn

[U27] Py：异步 HTTP
来源：http://qf.nszjky.cn

aiohttp.ClientSession() 配合 async with
来源：http://ce.nszjky.cn

[U28] Py：类型别名
来源：http://lw.nszjky.cn

UserId = int
来源：http://zj.haigaiapp.cn

[U29] Py：属性校验
来源：http://zy.nicolike.cn

@property 与 @x.setter 配合
来源：http://td.lnxyls.cn

[U30] Py：数据类
来源：http://ht.yuexingan06.cn

@dataclass(slots=True)
来源：http://ln.haigaiapp.cn

[U31] Py：单测
来源：http://pa.wgjwhj.cn

python -m pytest -q
来源：http://be.yuexingan06.cn

[U32] Py：代码格式化
来源：http://ln.shxzskj.cn

ruff format . && ruff check --fix .
来源：http://xi.colortex.cn

[U33] Py：打包发布
来源：http://xj.panjiajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://od.wgjwhj.cn

[U34] Py：判断编码
来源：http://ru.9csxet.cn

chardet.detect(raw)
来源：http://ra.lnxyls.cn

[U35] Py：发送邮件
来源：http://jg.9csxet.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xm.asd995.cn

[U36] Py：定时任务
来源：http://qv.9csxet.cn

schedule.every(10).minutes.do(job)
来源：http://vu.szxytkj.cn

[U37] Py：读写 Excel
来源：http://qq.colortex.cn

pandas.read_excel / DataFrame.to_excel
来源：http://he.9csxet.cn

[U38] Py：获取脚本所在目录
来源：http://gz.huixiangedu.cn

Path(__file__).resolve().parent
来源：http://yp.jianghongdianzi.cn

[U39] Py：判断是否在交互环境
来源：http://yg.newstarts.cn

sys.stdout.isatty()
来源：http://xq.yuexingan06.cn

[U40] Py：打印到标准错误
来源：http://zi.jctech888.com.cn

print("err", file=sys.stderr)
来源：http://qu.szxytkj.cn

[U41] PHP：初始化 Composer 项目
来源：http://kb.huanxung.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xl.yuntaijiaju.cn

[U42] PHP：PSR-4 自动加载
来源：http://nh.muxihuayi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pm.wgjwhj.cn

[U43] PHP：声明命名空间
来源：http://lu.shtwfgs.cn

namespace App\Http;
来源：http://mx.huixiangedu.cn

[U44] PHP：开启严格类型
来源：http://hh.huanxung.cn

declare(strict_types=1);
来源：http://jj.nicolike.cn

[U45] PHP：类型声明与返回类型
来源：http://gm.9csxet.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://cb.hnjuh.cn

[U46] PHP：可空类型
来源：http://yq.bjjhwx.cn

?string $name = null
来源：http://ka.szsharing.cn

[U47] PHP：联合类型
来源：http://zl.wgjwhj.cn

int|string $id
来源：http://nc.huanxung.cn

[U48] PHP：纯枚举
来源：http://dy.jctech888.com.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://in.nszjky.cn

[U49] PHP：只读属性
来源：http://gf.gzmigu.cn

public readonly string $name
来源：http://lu.huixiangedu.cn

[U50] PHP：构造器属性提升
来源：http://co.muxihuayi.cn

public function __construct(private int $id) {}
来源：http://cw.yuntaijiaju.cn

[U51] PHP：数组解构
来源：http://mo.huixiangedu.cn

[$a, $b] = $arr;
来源：http://jn.gzmigu.cn

[U52] PHP：箭头函数
来源：http://ed.chemitech.net.cn

$double = fn($x) => $x * 2;
来源：http://tc.nszjky.cn

[U53] PHP：空合并运算符
来源：http://dl.yuexingan06.cn

$v = $a ?? $b ?? "default";
来源：http://ht.chemitech.net.cn

[U54] PHP：空安全调用
来源：http://ei.jctech888.com.cn

$obj?->method()
来源：http://gw.huixiangedu.cn

[U55] PHP：match 表达式
来源：http://pf.huanxung.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ch.jianghongdianzi.cn

[U56] PHP：命名参数
来源：http://lc.newstarts.cn

f(a: 1, b: 2)
来源：http://bw.hahajie.cn

[U57] PHP：字符串插值
来源：http://zj.jctech888.com.cn

"值: {$a}"
来源：http://rh.jctech888.com.cn

[U58] PHP：数组三件套
来源：http://uu.shxzskj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fa.huixinmuqiang.cn

[U59] PHP：自定义排序
来源：http://os.521024.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://td.colortex.cn

[U60] PHP：JSON 编解码
来源：http://to.huixinmuqiang.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gd.jianghongdianzi.cn

[U61] PHP：正则
来源：http://zy.shxzukj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zi.jctech888.com.cn

[U62] PHP：日期对象
来源：http://jn.shxzskj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rn.shxzukj.cn

[U63] PHP：文件读写
来源：http://bp.gzmigu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pm.yuntaijiaju.cn

[U64] PHP：目录遍历
来源：http://vn.bookmarksfly.cn

glob("dir/*.php");  scandir("dir");
来源：http://ay.huixiangedu.cn

[U65] PHP：会话
来源：http://xi.szsharing.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://da.huixiangedu.cn

[U66] PHP：设置 Cookie
来源：http://om.colortex.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kd.huanxung.cn

[U67] PHP：处理文件上传
来源：http://gy.asd995.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kt.haigaiapp.cn

[U68] PHP：PDO 连接
来源：http://zk.wgjwhj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://su.hnjuh.cn

[U69] PHP：PDO 预处理
来源：http://po.nszjky.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wd.shxzukj.cn

[U70] PHP：PDO 事务
来源：http://dj.9csxet.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xo.nicolike.cn

[U71] PHP：抛出异常
来源：http://fj.muxihuayi.cn

throw new RuntimeException("失败", 500);
来源：http://ko.hahajie.cn

[U72] PHP：写错误日志
来源：http://xm.haigaiapp.cn

error_log("失败: " . $e->getMessage());
来源：http://mm.szxytkj.cn

[U73] PHP：读取 ini 配置
来源：http://oc.yuexingan06.cn

parse_ini_file("config.ini", true)
来源：http://bz.chemitech.net.cn

[U74] PHP：读取环境变量
来源：http://ho.shtwfgs.cn

getenv("APP_ENV") ?: "production"
来源：http://op.gzmigu.cn

[U75] PHP：依赖注入
来源：http://dd.haigaiapp.cn

composer require psr/container
来源：http://rt.colortex.cn

[U76] PHP：简单路由
来源：http://ar.huanxung.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://uy.huixiangedu.cn

[U77] PHP：模板渲染
来源：http://rz.lnxyls.cn

composer require twig/twig
来源：http://ar.hahajie.cn

[U78] PHP：单元测试
来源：http://tr.asd995.cn

composer require --dev phpunit/phpunit
来源：http://tu.haigaiapp.cn

[U79] PHP：静态分析
来源：http://am.shxzskj.cn

composer require --dev phpstan/phpstan
来源：http://yl.bookmarksfly.cn

[U80] PHP：代码规范修复
来源：http://ds.szsharing.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://im.huixiangedu.cn

[U81] JS：初始化项目
来源：http://su.lnxyls.cn

npm init -y;  npm i express
来源：http://zv.lnxyls.cn

[U82] JS：package.json 脚本
来源：http://eh.bookmarksfly.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ij.szxytkj.cn

[U83] JS：ES Module 导入导出
来源：http://rj.haigaiapp.cn

export const a = 1;  import { a } from "./m.js";
来源：http://je.lnxyls.cn

[U84] JS：CommonJS 写法
来源：http://cm.shxzskj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://qb.hnjuh.cn

[U85] JS：可选链
来源：http://kg.shtwfgs.cn

a?.b?.c
来源：http://ot.yuntaijiaju.cn

[U86] JS：空值合并
来源：http://kq.muxihuayi.cn

a ?? b
来源：http://jc.yuexingan06.cn

[U87] JS：解构默认值
来源：http://cv.szsharing.cn

const { a = 1, b = 2 } = obj;
来源：http://ie.muxihuayi.cn

[U88] JS：对象展开合并
来源：http://zj.wgjwhj.cn

{ ...a, ...b }
来源：http://yy.colortex.cn

[U89] JS：数组去重
来源：http://kz.yuntaijiaju.cn

[...new Set(arr)]
来源：http://xd.wgjwhj.cn

[U90] JS：数字数组排序
来源：http://kp.chemitech.net.cn

[...arr].sort((a, b) => a - b)
来源：http://wx.521024.cn

[U91] JS：对象键值遍历
来源：http://fl.yuntaijiaju.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fu.huixinmuqiang.cn

[U92] JS：深拷贝
来源：http://zw.muxihuayi.cn

structuredClone(obj)
来源：http://co.yuntaijiaju.cn

[U93] JS：模板字符串
来源：http://yh.chemitech.net.cn

`共 ${n} 条`
来源：http://cw.haigaiapp.cn

[U94] JS：箭头函数
来源：http://zs.szsharing.cn

const double = x => x * 2;
来源：http://ut.colortex.cn

[U95] JS：Promise 包装
来源：http://lw.asd995.cn

new Promise((resolve, reject) => {})
来源：http://hs.asd995.cn

[U96] JS：async/await 与异常
来源：http://cy.muxihuayi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xm.haigaiapp.cn

[U97] JS：并发请求
来源：http://zm.yuexingan06.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ln.huixiangedu.cn

[U98] JS：fetch 带 JSON
来源：http://lq.jctech888.com.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://br.wgjwhj.cn

[U99] JS：事件监听
来源：http://av.yuexingan06.cn

el.addEventListener("click", e => {})
来源：http://hr.yuexingan06.cn

[U100] JS：DOM 查询
来源：http://ei.shxzukj.cn

document.querySelector(".item")
来源：http://cr.bookmarksfly.cn

[U101] JS：classList 操作
来源：http://ee.shxzukj.cn

el.classList.toggle("active")
来源：http://sy.newstarts.cn

[U102] JS：本地存储
来源：http://xz.bookmarksfly.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://mk.9csxet.cn

[U103] JS：定时器
来源：http://av.521024.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lj.lnxyls.cn

[U104] JS：防抖
来源：http://js.haigaiapp.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bo.nszjky.cn

[U105] JS：节流
来源：http://fq.chemitech.net.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gl.shtwfgs.cn

[U106] JS：日期格式化
来源：http://cr.haigaiapp.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://be.gzmigu.cn

[U107] JS：数字千分位
来源：http://xr.muxihuayi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lh.jctech888.com.cn

[U108] JS：随机整数
来源：http://dl.huanxung.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://sp.asd995.cn

[U109] JS：数组分组
来源：http://sw.lnxyls.cn

Object.groupBy(arr, x => x.type)
来源：http://qz.huixiangedu.cn

[U110] JS：数组分块
来源：http://ly.colortex.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gx.newstarts.cn

[U111] JS：对象转 Map
来源：http://cf.shxzskj.cn

new Map(Object.entries(obj))
来源：http://eg.nszjky.cn

[U112] JS：字符串补位
来源：http://gi.9csxet.cn

"7".padStart(3, "0")
来源：http://rk.wgjwhj.cn

[U113] JS：正则替换全部
来源：http://tq.wgjwhj.cn

s.replaceAll("a", "b")
来源：http://po.521024.cn

[U114] JS：JSON 深比较
来源：http://uy.jianghongdianzi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://sf.bookmarksfly.cn

[U115] JS：生成 UUID
来源：http://fm.muxihuayi.cn

crypto.randomUUID()
来源：http://be.jctech888.com.cn

[U116] JS：类型检查（JSDoc）
来源：http://yn.asd995.cn

/** @param {string} name */ function f(name) {}
来源：http://aj.bjjhwx.cn

[U117] JS：单元测试
来源：http://fz.hnjuh.cn

npm i -D vitest;  npx vitest
来源：http://pb.nszjky.cn

[U118] JS：开发服务器
来源：http://vu.lnxyls.cn

npm i -D vite;  npx vite
来源：http://ek.szxytkj.cn

[U119] JS：生产构建
来源：http://op.szxytkj.cn

npx vite build
来源：http://sp.nicolike.cn

[U120] JS：读取环境变量（Vite）
来源：http://wx.huanxung.cn

import.meta.env.VITE_API_URL
来源：http://mv.colortex.cn

================================================================================
来源：http://gl.yuexingan06.cn

统计汇总
来源：http://qr.gzmigu.cn

================================================================================
来源：http://ym.huanxung.cn

按语言统计（条）：
来源：http://aa.jctech888.com.cn

Python ......... 252
来源：http://jf.huixinmuqiang.cn

PHP ............ 252
来源：http://tu.jctech888.com.cn

JavaScript ..... 252
来源：http://ck.nicolike.cn

TypeScript ..... 212
来源：http://wj.szsharing.cn

Java ........... 212
来源：http://mf.lnxyls.cn

Go ............. 212
来源：http://zz.newstarts.cn

Ruby ........... 212
来源：http://np.colortex.cn

C# ............. 212
来源：http://xs.chemitech.net.cn

C .............. 30
来源：http://sl.yuntaijiaju.cn

C++ ............ 30
来源：http://lx.haigaiapp.cn

SQL ............ 90
来源：http://mm.muxihuayi.cn

Bash ........... 80
来源：http://gu.yuexingan06.cn

Kotlin ......... 15
来源：http://oz.szsharing.cn

Swift .......... 15
来源：http://er.szxytkj.cn

Lua ............ 10
来源：http://io.szsharing.cn

Perl ........... 10
来源：http://fi.yuntaijiaju.cn

Scala .......... 10
来源：http://zh.nszjky.cn

------------------------------------
来源：http://nb.huixinmuqiang.cn

合计 ........... 2106 条
来源：http://mz.huixiangedu.cn

按章节统计：
来源：http://fh.szsharing.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://za.huixiangedu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kj.asd995.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qc.yuexingan06.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kh.yuntaijiaju.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bv.chemitech.net.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bt.yuexingan06.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ea.nszjky.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kc.lnxyls.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hm.asd995.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ey.shxzukj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gt.shtwfgs.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zi.haigaiapp.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vh.colortex.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ee.521024.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://sn.lnxyls.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xb.colortex.cn

Q SQL 专题                              90
来源：http://rr.muxihuayi.cn

R Bash 专题                             80
来源：http://qp.bookmarksfly.cn

S C / C++ 专题                          60
来源：http://nd.yuexingan06.cn

T 其他语言补充                          60
来源：http://lo.gzmigu.cn

U 高频实用片段                         120
来源：http://xn.lnxyls.cn

------------------------------------
来源：http://ts.newstarts.cn

合计                                  2106 条
来源：http://vk.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://me.huixinmuqiang.cn

使用提醒
来源：http://qa.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://qv.gzmigu.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ae.panjiajie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://lk.nicolike.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fd.nszjky.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ef.hnjuh.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gm.chemitech.net.cn

—— 文件结束 ——
来源：http://bb.asd995.cn

================================================================================
来源：http://pw.yuntaijiaju.cn

程序语言常见例子速查手册（2024 版）
来源：http://ns.huixinmuqiang.cn

Common Programming Examples Cheat Book
来源：http://jw.huanxung.cn

================================================================================
来源：http://qm.nszjky.cn

【收录内容】
来源：http://dp.yuexingan06.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://cs.yuntaijiaju.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tr.yuntaijiaju.cn

SQL · Bash · C · C++
来源：http://zj.huixiangedu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ny.jctech888.com.cn

【使用说明】
来源：http://qu.lnxyls.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qe.9csxet.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://md.521024.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ev.huixinmuqiang.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yv.asd995.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://wd.shtwfgs.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vr.yuntaijiaju.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bs.colortex.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zc.chemitech.net.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hb.huanxung.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rp.wgjwhj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mm.colortex.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vy.chemitech.net.cn

【文件统计】
来源：http://xn.jianghongdianzi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ma.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://jc.muxihuayi.cn

目  录
来源：http://zq.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://eq.jianghongdianzi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kc.521024.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://fb.hnjuh.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://yk.nszjky.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dz.panjiajie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vh.wgjwhj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qk.colortex.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://au.yuexingan06.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ep.jianghongdianzi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jf.bookmarksfly.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://od.jianghongdianzi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://iq.newstarts.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://th.nicolike.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qw.shtwfgs.cn


<!-- 参考信息 -->