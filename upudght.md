代发 wailian999

[T43] Perl：字符串插值
来源：http://ds.hahajie.cn

"值: $a"
来源：http://vt.colortex.cn

[T44] Perl：条件
来源：http://hd.9csxet.cn

if ($a > 0) { print "正"; }
来源：http://nz.nszjky.cn

[T45] Perl：数组遍历
来源：http://yf.bookmarksfly.cn

for my $x (@arr) { print $x; }
来源：http://qi.hahajie.cn

[T46] Perl：哈希操作
来源：http://gb.bjjhwx.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uz.szxytkj.cn

[T47] Perl：正则捕获
来源：http://cz.shxzukj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://an.wgjwhj.cn

[T48] Perl：正则替换
来源：http://dj.huixinmuqiang.cn

$s =~ s/old/new/g;
来源：http://mn.haigaiapp.cn

[T49] Perl：函数
来源：http://cy.muxihuayi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lz.huanxung.cn

[T50] Perl：逐行读文件
来源：http://br.shxzskj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://nw.nicolike.cn

while (my $line = <$fh>) { print $line; }
来源：http://cx.bookmarksfly.cn

[T51] Scala：Hello World
来源：http://ak.hahajie.cn

println("Hello")
来源：http://fn.colortex.cn

[T52] Scala：变量
来源：http://yl.yuexingan06.cn

val a = 1;  var b = 2
来源：http://kn.chemitech.net.cn

[T53] Scala：字符串插值
来源：http://mq.nszjky.cn

s"值: $b"
来源：http://fp.colortex.cn

[T54] Scala：集合映射
来源：http://jx.yuexingan06.cn

List(1, 2, 3).map(_ * 2)
来源：http://sr.nicolike.cn

[T55] Scala：集合过滤
来源：http://ma.lnxyls.cn

List(1, 2, 3).filter(_ > 1)
来源：http://rw.huixiangedu.cn

[T56] Scala：样例类
来源：http://ge.521024.cn

case class User(name: String, age: Int)
来源：http://go.bookmarksfly.cn

[T57] Scala：模式匹配
来源：http://yi.bjjhwx.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://pe.bookmarksfly.cn

[T58] Scala：函数定义
来源：http://bx.gzmigu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://co.jianghongdianzi.cn

[T59] Scala：循环
来源：http://eb.chemitech.net.cn

for (i <- 1 to 10) println(i)
来源：http://bk.nicolike.cn

[T60] Scala：折叠
来源：http://eh.jianghongdianzi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vx.chemitech.net.cn

================================================================================
来源：http://qx.huanxung.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wy.yuexingan06.cn

================================================================================
来源：http://ro.muxihuayi.cn

[U01] Py：创建虚拟环境
来源：http://md.hahajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bb.bjjhwx.cn

[U02] Py：导出 / 安装依赖
来源：http://gn.haigaiapp.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wo.lnxyls.cn

[U03] Py：加载 .env 配置
来源：http://ku.szsharing.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://oi.szxytkj.cn

[U04] Py：变量调试打印
来源：http://hu.nicolike.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ni.nicolike.cn

[U05] Py：列表去重且保序
来源：http://jn.muxihuayi.cn

list(dict.fromkeys(arr))
来源：http://dd.bookmarksfly.cn

[U06] Py：合并两个字典
来源：http://ly.bjjhwx.cn

{**a, **b}
来源：http://uo.wgjwhj.cn

[U07] Py：反转字典键值
来源：http://tk.shxzskj.cn

{v: k for k, v in d.items()}
来源：http://ve.huixinmuqiang.cn

[U08] Py：展平二维列表
来源：http://as.yuexingan06.cn

[y for x in nested for y in x]
来源：http://ix.hahajie.cn

[U09] Py：字典取最大值的键
来源：http://fs.haigaiapp.cn

max(d, key=d.get)
来源：http://ip.521024.cn

[U10] Py：按值排序字典
来源：http://wf.shxzukj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gv.hahajie.cn

[U11] Py：生成器表达式
来源：http://uc.jctech888.com.cn

(x * 2 for x in arr)
来源：http://bk.shtwfgs.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ff.9csxet.cn

Counter(arr).most_common(3)
来源：http://ry.nszjky.cn

[U13] Py：固定长度队列
来源：http://vb.bjjhwx.cn

deque(maxlen=10)
来源：http://ws.muxihuayi.cn

[U14] Py：分组收集到列表
来源：http://ts.gzmigu.cn

defaultdict(list)
来源：http://bw.nszjky.cn

[U15] Py：高精度计时
来源：http://fq.wgjwhj.cn

t = time.perf_counter()
来源：http://lu.wgjwhj.cn

[U16] Py：命令行参数解析
来源：http://xm.bookmarksfly.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nv.yuntaijiaju.cn

[U17] Py：初始化日志
来源：http://qv.newstarts.cn

logging.basicConfig(level=logging.INFO)
来源：http://gt.wgjwhj.cn

[U18] Py：预编译正则
来源：http://zl.chemitech.net.cn

pat = re.compile(r"\d+")
来源：http://rx.asd995.cn

[U19] Py：正则替换带回调
来源：http://sz.521024.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://os.521024.cn

[U20] Py：缓存函数结果
来源：http://zz.9csxet.cn

@functools.lru_cache(maxsize=None)
来源：http://zw.shtwfgs.cn

[U21] Py：自定义上下文管理器
来源：http://rm.bjjhwx.cn

@contextlib.contextmanager
来源：http://ds.yuexingan06.cn

[U22] Py：矩阵转置
来源：http://er.huanxung.cn

list(zip(*m))
来源：http://fw.jctech888.com.cn

[U23] Py：分块读取大文件
来源：http://ya.shxzukj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ve.jianghongdianzi.cn

[U24] Py：路径操作
来源：http://on.bookmarksfly.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tj.hahajie.cn

[U25] Py：CSV 按字典读
来源：http://zb.hahajie.cn

csv.DictReader(f)
来源：http://zx.muxihuayi.cn

[U26] Py：并发下载
来源：http://gn.huanxung.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wp.muxihuayi.cn

[U27] Py：异步 HTTP
来源：http://nq.huanxung.cn

aiohttp.ClientSession() 配合 async with
来源：http://ru.colortex.cn

[U28] Py：类型别名
来源：http://lg.lnxyls.cn

UserId = int
来源：http://kp.panjiajie.cn

[U29] Py：属性校验
来源：http://ja.szsharing.cn

@property 与 @x.setter 配合
来源：http://mb.haigaiapp.cn

[U30] Py：数据类
来源：http://yr.szsharing.cn

@dataclass(slots=True)
来源：http://gd.521024.cn

[U31] Py：单测
来源：http://de.huixinmuqiang.cn

python -m pytest -q
来源：http://wi.newstarts.cn

[U32] Py：代码格式化
来源：http://ma.jctech888.com.cn

ruff format . && ruff check --fix .
来源：http://id.jianghongdianzi.cn

[U33] Py：打包发布
来源：http://af.huixiangedu.cn

python -m build  （依赖 pyproject.toml）
来源：http://rp.jctech888.com.cn

[U34] Py：判断编码
来源：http://fm.nszjky.cn

chardet.detect(raw)
来源：http://tw.yuntaijiaju.cn

[U35] Py：发送邮件
来源：http://fo.newstarts.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://be.asd995.cn

[U36] Py：定时任务
来源：http://bm.colortex.cn

schedule.every(10).minutes.do(job)
来源：http://aw.521024.cn

[U37] Py：读写 Excel
来源：http://ax.huixiangedu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://cv.huanxung.cn

[U38] Py：获取脚本所在目录
来源：http://ai.nszjky.cn

Path(__file__).resolve().parent
来源：http://ad.yuexingan06.cn

[U39] Py：判断是否在交互环境
来源：http://ks.lnxyls.cn

sys.stdout.isatty()
来源：http://gf.shxzskj.cn

[U40] Py：打印到标准错误
来源：http://eo.nszjky.cn

print("err", file=sys.stderr)
来源：http://ff.shxzukj.cn

[U41] PHP：初始化 Composer 项目
来源：http://ss.huanxung.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ge.jianghongdianzi.cn

[U42] PHP：PSR-4 自动加载
来源：http://zs.hahajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vl.nszjky.cn

[U43] PHP：声明命名空间
来源：http://wf.521024.cn

namespace App\Http;
来源：http://cm.huixiangedu.cn

[U44] PHP：开启严格类型
来源：http://na.huanxung.cn

declare(strict_types=1);
来源：http://ol.asd995.cn

[U45] PHP：类型声明与返回类型
来源：http://ii.nicolike.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://og.szxytkj.cn

[U46] PHP：可空类型
来源：http://xn.chemitech.net.cn

?string $name = null
来源：http://rw.shxzskj.cn

[U47] PHP：联合类型
来源：http://tl.jctech888.com.cn

int|string $id
来源：http://bd.wgjwhj.cn

[U48] PHP：纯枚举
来源：http://tw.newstarts.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sv.9csxet.cn

[U49] PHP：只读属性
来源：http://ez.huixiangedu.cn

public readonly string $name
来源：http://ip.szxytkj.cn

[U50] PHP：构造器属性提升
来源：http://mc.asd995.cn

public function __construct(private int $id) {}
来源：http://go.newstarts.cn

[U51] PHP：数组解构
来源：http://yj.lnxyls.cn

[$a, $b] = $arr;
来源：http://jt.bookmarksfly.cn

[U52] PHP：箭头函数
来源：http://tl.asd995.cn

$double = fn($x) => $x * 2;
来源：http://nb.shtwfgs.cn

[U53] PHP：空合并运算符
来源：http://zf.panjiajie.cn

$v = $a ?? $b ?? "default";
来源：http://qx.9csxet.cn

[U54] PHP：空安全调用
来源：http://hf.521024.cn

$obj?->method()
来源：http://uw.521024.cn

[U55] PHP：match 表达式
来源：http://ll.nicolike.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ld.gzmigu.cn

[U56] PHP：命名参数
来源：http://ro.9csxet.cn

f(a: 1, b: 2)
来源：http://cq.szsharing.cn

[U57] PHP：字符串插值
来源：http://gz.szxytkj.cn

"值: {$a}"
来源：http://vv.szxytkj.cn

[U58] PHP：数组三件套
来源：http://cj.szsharing.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fb.huixinmuqiang.cn

[U59] PHP：自定义排序
来源：http://do.haigaiapp.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mf.bookmarksfly.cn

[U60] PHP：JSON 编解码
来源：http://uv.szsharing.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bo.hahajie.cn

[U61] PHP：正则
来源：http://nm.szsharing.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rm.lnxyls.cn

[U62] PHP：日期对象
来源：http://vb.nicolike.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vx.szxytkj.cn

[U63] PHP：文件读写
来源：http://sl.gzmigu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://aw.lnxyls.cn

[U64] PHP：目录遍历
来源：http://ag.shtwfgs.cn

glob("dir/*.php");  scandir("dir");
来源：http://ny.jctech888.com.cn

[U65] PHP：会话
来源：http://za.hahajie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ax.panjiajie.cn

[U66] PHP：设置 Cookie
来源：http://la.jctech888.com.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kd.huanxung.cn

[U67] PHP：处理文件上传
来源：http://re.hnjuh.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ct.shxzskj.cn

[U68] PHP：PDO 连接
来源：http://md.bookmarksfly.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cq.asd995.cn

[U69] PHP：PDO 预处理
来源：http://da.szxytkj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xw.shtwfgs.cn

[U70] PHP：PDO 事务
来源：http://cx.hahajie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gl.shxzukj.cn

[U71] PHP：抛出异常
来源：http://jw.jctech888.com.cn

throw new RuntimeException("失败", 500);
来源：http://zx.huixiangedu.cn

[U72] PHP：写错误日志
来源：http://so.muxihuayi.cn

error_log("失败: " . $e->getMessage());
来源：http://wf.yuexingan06.cn

[U73] PHP：读取 ini 配置
来源：http://xj.wgjwhj.cn

parse_ini_file("config.ini", true)
来源：http://ez.gzmigu.cn

[U74] PHP：读取环境变量
来源：http://uh.newstarts.cn

getenv("APP_ENV") ?: "production"
来源：http://ie.jctech888.com.cn

[U75] PHP：依赖注入
来源：http://ia.huixinmuqiang.cn

composer require psr/container
来源：http://pw.9csxet.cn

[U76] PHP：简单路由
来源：http://jf.chemitech.net.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ux.szxytkj.cn

[U77] PHP：模板渲染
来源：http://ze.hahajie.cn

composer require twig/twig
来源：http://eo.bjjhwx.cn

[U78] PHP：单元测试
来源：http://fz.yuntaijiaju.cn

composer require --dev phpunit/phpunit
来源：http://ne.colortex.cn

[U79] PHP：静态分析
来源：http://sh.bookmarksfly.cn

composer require --dev phpstan/phpstan
来源：http://nw.hahajie.cn

[U80] PHP：代码规范修复
来源：http://ei.bjjhwx.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://gf.muxihuayi.cn

[U81] JS：初始化项目
来源：http://of.nszjky.cn

npm init -y;  npm i express
来源：http://ae.szsharing.cn

[U82] JS：package.json 脚本
来源：http://yf.shxzskj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ou.9csxet.cn

[U83] JS：ES Module 导入导出
来源：http://sx.szsharing.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vt.hnjuh.cn

[U84] JS：CommonJS 写法
来源：http://qh.haigaiapp.cn

module.exports = { a };  const { a } = require("./m");
来源：http://id.muxihuayi.cn

[U85] JS：可选链
来源：http://fm.szsharing.cn

a?.b?.c
来源：http://hr.huixiangedu.cn

[U86] JS：空值合并
来源：http://bw.asd995.cn

a ?? b
来源：http://ef.muxihuayi.cn

[U87] JS：解构默认值
来源：http://hr.huixiangedu.cn

const { a = 1, b = 2 } = obj;
来源：http://yx.jianghongdianzi.cn

[U88] JS：对象展开合并
来源：http://bi.hahajie.cn

{ ...a, ...b }
来源：http://ua.huixiangedu.cn

[U89] JS：数组去重
来源：http://ga.muxihuayi.cn

[...new Set(arr)]
来源：http://fx.jianghongdianzi.cn

[U90] JS：数字数组排序
来源：http://ma.gzmigu.cn

[...arr].sort((a, b) => a - b)
来源：http://oj.huixinmuqiang.cn

[U91] JS：对象键值遍历
来源：http://qa.lnxyls.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://je.gzmigu.cn

[U92] JS：深拷贝
来源：http://iy.newstarts.cn

structuredClone(obj)
来源：http://st.shxzukj.cn

[U93] JS：模板字符串
来源：http://tm.shtwfgs.cn

`共 ${n} 条`
来源：http://ec.shxzskj.cn

[U94] JS：箭头函数
来源：http://bx.szxytkj.cn

const double = x => x * 2;
来源：http://ic.wgjwhj.cn

[U95] JS：Promise 包装
来源：http://ja.szxytkj.cn

new Promise((resolve, reject) => {})
来源：http://tk.colortex.cn

[U96] JS：async/await 与异常
来源：http://pu.jianghongdianzi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cu.haigaiapp.cn

[U97] JS：并发请求
来源：http://sc.szsharing.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://it.lnxyls.cn

[U98] JS：fetch 带 JSON
来源：http://ii.9csxet.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://sz.521024.cn

[U99] JS：事件监听
来源：http://ya.jctech888.com.cn

el.addEventListener("click", e => {})
来源：http://ml.shxzskj.cn

[U100] JS：DOM 查询
来源：http://ys.bookmarksfly.cn

document.querySelector(".item")
来源：http://xy.gzmigu.cn

[U101] JS：classList 操作
来源：http://qw.nicolike.cn

el.classList.toggle("active")
来源：http://fe.gzmigu.cn

[U102] JS：本地存储
来源：http://qu.bjjhwx.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://yy.shtwfgs.cn

[U103] JS：定时器
来源：http://sm.jianghongdianzi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rc.521024.cn

[U104] JS：防抖
来源：http://lt.hnjuh.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zk.chemitech.net.cn

[U105] JS：节流
来源：http://ie.yuntaijiaju.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://uu.nicolike.cn

[U106] JS：日期格式化
来源：http://nl.panjiajie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ay.jctech888.com.cn

[U107] JS：数字千分位
来源：http://xd.chemitech.net.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sm.shxzukj.cn

[U108] JS：随机整数
来源：http://nx.nszjky.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cv.muxihuayi.cn

[U109] JS：数组分组
来源：http://lx.shtwfgs.cn

Object.groupBy(arr, x => x.type)
来源：http://ci.szxytkj.cn

[U110] JS：数组分块
来源：http://us.hnjuh.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ek.bookmarksfly.cn

[U111] JS：对象转 Map
来源：http://mt.colortex.cn

new Map(Object.entries(obj))
来源：http://ii.hahajie.cn

[U112] JS：字符串补位
来源：http://nh.gzmigu.cn

"7".padStart(3, "0")
来源：http://da.hahajie.cn

[U113] JS：正则替换全部
来源：http://ho.haigaiapp.cn

s.replaceAll("a", "b")
来源：http://cj.gzmigu.cn

[U114] JS：JSON 深比较
来源：http://vq.panjiajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://xa.newstarts.cn

[U115] JS：生成 UUID
来源：http://xp.jctech888.com.cn

crypto.randomUUID()
来源：http://uq.huanxung.cn

[U116] JS：类型检查（JSDoc）
来源：http://bu.9csxet.cn

/** @param {string} name */ function f(name) {}
来源：http://eb.hnjuh.cn

[U117] JS：单元测试
来源：http://us.hnjuh.cn

npm i -D vitest;  npx vitest
来源：http://jv.szsharing.cn

[U118] JS：开发服务器
来源：http://vc.asd995.cn

npm i -D vite;  npx vite
来源：http://sn.muxihuayi.cn

[U119] JS：生产构建
来源：http://bq.huixinmuqiang.cn

npx vite build
来源：http://bx.szxytkj.cn

[U120] JS：读取环境变量（Vite）
来源：http://sh.shtwfgs.cn

import.meta.env.VITE_API_URL
来源：http://lm.chemitech.net.cn

================================================================================
来源：http://gq.haigaiapp.cn

统计汇总
来源：http://ls.gzmigu.cn

================================================================================
来源：http://pb.panjiajie.cn

按语言统计（条）：
来源：http://yw.szsharing.cn

Python ......... 252
来源：http://qj.shtwfgs.cn

PHP ............ 252
来源：http://vo.wgjwhj.cn

JavaScript ..... 252
来源：http://wn.hnjuh.cn

TypeScript ..... 212
来源：http://vf.haigaiapp.cn

Java ........... 212
来源：http://ak.szsharing.cn

Go ............. 212
来源：http://tn.9csxet.cn

Ruby ........... 212
来源：http://cb.szxytkj.cn

C# ............. 212
来源：http://jj.nicolike.cn

C .............. 30
来源：http://pi.newstarts.cn

C++ ............ 30
来源：http://qj.jianghongdianzi.cn

SQL ............ 90
来源：http://vt.shtwfgs.cn

Bash ........... 80
来源：http://od.szsharing.cn

Kotlin ......... 15
来源：http://gr.nszjky.cn

Swift .......... 15
来源：http://xt.yuexingan06.cn

Lua ............ 10
来源：http://le.yuntaijiaju.cn

Perl ........... 10
来源：http://rl.panjiajie.cn


<!-- 参考信息 -->