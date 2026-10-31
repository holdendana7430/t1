代发 wailian999

[T45] Perl：数组遍历
来源：http://qe.jctech888.com.cn

for my $x (@arr) { print $x; }
来源：http://ga.shxzskj.cn

[T46] Perl：哈希操作
来源：http://qw.shxzskj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kd.newstarts.cn

[T47] Perl：正则捕获
来源：http://bj.nszjky.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://af.newstarts.cn

[T48] Perl：正则替换
来源：http://nf.nicolike.cn

$s =~ s/old/new/g;
来源：http://rt.nszjky.cn

[T49] Perl：函数
来源：http://dz.lnxyls.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ca.muxihuayi.cn

[T50] Perl：逐行读文件
来源：http://gq.nszjky.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wg.shtwfgs.cn

while (my $line = <$fh>) { print $line; }
来源：http://yk.muxihuayi.cn

[T51] Scala：Hello World
来源：http://kk.yuntaijiaju.cn

println("Hello")
来源：http://lv.chemitech.net.cn

[T52] Scala：变量
来源：http://xz.panjiajie.cn

val a = 1;  var b = 2
来源：http://dh.newstarts.cn

[T53] Scala：字符串插值
来源：http://ii.bjjhwx.cn

s"值: $b"
来源：http://io.huixiangedu.cn

[T54] Scala：集合映射
来源：http://bn.hahajie.cn

List(1, 2, 3).map(_ * 2)
来源：http://fv.bookmarksfly.cn

[T55] Scala：集合过滤
来源：http://is.szsharing.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wo.lnxyls.cn

[T56] Scala：样例类
来源：http://tc.yuexingan06.cn

case class User(name: String, age: Int)
来源：http://hu.szxytkj.cn

[T57] Scala：模式匹配
来源：http://pp.nicolike.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://hr.nicolike.cn

[T58] Scala：函数定义
来源：http://eb.nszjky.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bn.haigaiapp.cn

[T59] Scala：循环
来源：http://jg.nszjky.cn

for (i <- 1 to 10) println(i)
来源：http://ns.huixiangedu.cn

[T60] Scala：折叠
来源：http://us.lnxyls.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tu.wgjwhj.cn

================================================================================
来源：http://uv.haigaiapp.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ks.asd995.cn

================================================================================
来源：http://cu.newstarts.cn

[U01] Py：创建虚拟环境
来源：http://zc.shxzukj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://os.9csxet.cn

[U02] Py：导出 / 安装依赖
来源：http://qn.chemitech.net.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yr.newstarts.cn

[U03] Py：加载 .env 配置
来源：http://ag.yuexingan06.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://np.newstarts.cn

[U04] Py：变量调试打印
来源：http://mw.huixiangedu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hi.huixinmuqiang.cn

[U05] Py：列表去重且保序
来源：http://pu.nicolike.cn

list(dict.fromkeys(arr))
来源：http://hw.bjjhwx.cn

[U06] Py：合并两个字典
来源：http://eg.nszjky.cn

{**a, **b}
来源：http://xo.jctech888.com.cn

[U07] Py：反转字典键值
来源：http://nq.colortex.cn

{v: k for k, v in d.items()}
来源：http://wm.yuexingan06.cn

[U08] Py：展平二维列表
来源：http://mw.9csxet.cn

[y for x in nested for y in x]
来源：http://jd.szsharing.cn

[U09] Py：字典取最大值的键
来源：http://mu.yuexingan06.cn

max(d, key=d.get)
来源：http://xs.shtwfgs.cn

[U10] Py：按值排序字典
来源：http://xh.asd995.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ix.wgjwhj.cn

[U11] Py：生成器表达式
来源：http://sd.hnjuh.cn

(x * 2 for x in arr)
来源：http://hu.muxihuayi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lf.nszjky.cn

Counter(arr).most_common(3)
来源：http://ib.bookmarksfly.cn

[U13] Py：固定长度队列
来源：http://cg.shxzskj.cn

deque(maxlen=10)
来源：http://sl.jctech888.com.cn

[U14] Py：分组收集到列表
来源：http://lt.szxytkj.cn

defaultdict(list)
来源：http://gz.szsharing.cn

[U15] Py：高精度计时
来源：http://fj.huanxung.cn

t = time.perf_counter()
来源：http://pr.nicolike.cn

[U16] Py：命令行参数解析
来源：http://oa.szsharing.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ln.szsharing.cn

[U17] Py：初始化日志
来源：http://gl.newstarts.cn

logging.basicConfig(level=logging.INFO)
来源：http://ac.521024.cn

[U18] Py：预编译正则
来源：http://ks.jctech888.com.cn

pat = re.compile(r"\d+")
来源：http://vp.szxytkj.cn

[U19] Py：正则替换带回调
来源：http://ll.shxzukj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gl.gzmigu.cn

[U20] Py：缓存函数结果
来源：http://wz.shtwfgs.cn

@functools.lru_cache(maxsize=None)
来源：http://jv.521024.cn

[U21] Py：自定义上下文管理器
来源：http://yc.colortex.cn

@contextlib.contextmanager
来源：http://hg.panjiajie.cn

[U22] Py：矩阵转置
来源：http://db.bookmarksfly.cn

list(zip(*m))
来源：http://be.asd995.cn

[U23] Py：分块读取大文件
来源：http://mv.haigaiapp.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rn.shxzskj.cn

[U24] Py：路径操作
来源：http://vf.colortex.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rp.9csxet.cn

[U25] Py：CSV 按字典读
来源：http://bc.jianghongdianzi.cn

csv.DictReader(f)
来源：http://ro.szxytkj.cn

[U26] Py：并发下载
来源：http://bo.9csxet.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gt.jctech888.com.cn

[U27] Py：异步 HTTP
来源：http://vq.gzmigu.cn

aiohttp.ClientSession() 配合 async with
来源：http://iv.muxihuayi.cn

[U28] Py：类型别名
来源：http://cr.haigaiapp.cn

UserId = int
来源：http://fj.panjiajie.cn

[U29] Py：属性校验
来源：http://ao.shtwfgs.cn

@property 与 @x.setter 配合
来源：http://gl.huanxung.cn

[U30] Py：数据类
来源：http://mz.newstarts.cn

@dataclass(slots=True)
来源：http://yz.huanxung.cn

[U31] Py：单测
来源：http://mk.nicolike.cn

python -m pytest -q
来源：http://yd.521024.cn

[U32] Py：代码格式化
来源：http://dr.muxihuayi.cn

ruff format . && ruff check --fix .
来源：http://lm.muxihuayi.cn

[U33] Py：打包发布
来源：http://vr.panjiajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://sb.panjiajie.cn

[U34] Py：判断编码
来源：http://sh.gzmigu.cn

chardet.detect(raw)
来源：http://lq.huixiangedu.cn

[U35] Py：发送邮件
来源：http://ey.jianghongdianzi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tc.szsharing.cn

[U36] Py：定时任务
来源：http://xq.hnjuh.cn

schedule.every(10).minutes.do(job)
来源：http://mm.szsharing.cn

[U37] Py：读写 Excel
来源：http://ev.lnxyls.cn

pandas.read_excel / DataFrame.to_excel
来源：http://bq.huixinmuqiang.cn

[U38] Py：获取脚本所在目录
来源：http://fc.yuntaijiaju.cn

Path(__file__).resolve().parent
来源：http://rx.muxihuayi.cn

[U39] Py：判断是否在交互环境
来源：http://ai.shxzukj.cn

sys.stdout.isatty()
来源：http://xi.asd995.cn

[U40] Py：打印到标准错误
来源：http://rx.huixinmuqiang.cn

print("err", file=sys.stderr)
来源：http://me.gzmigu.cn

[U41] PHP：初始化 Composer 项目
来源：http://ip.wgjwhj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://kb.colortex.cn

[U42] PHP：PSR-4 自动加载
来源：http://uk.muxihuayi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ll.colortex.cn

[U43] PHP：声明命名空间
来源：http://cx.shxzskj.cn

namespace App\Http;
来源：http://ah.muxihuayi.cn

[U44] PHP：开启严格类型
来源：http://fy.muxihuayi.cn

declare(strict_types=1);
来源：http://mz.jianghongdianzi.cn

[U45] PHP：类型声明与返回类型
来源：http://ms.shxzskj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://cp.szsharing.cn

[U46] PHP：可空类型
来源：http://up.yuntaijiaju.cn

?string $name = null
来源：http://go.lnxyls.cn

[U47] PHP：联合类型
来源：http://lg.nicolike.cn

int|string $id
来源：http://ug.hnjuh.cn

[U48] PHP：纯枚举
来源：http://gz.bookmarksfly.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ck.nszjky.cn

[U49] PHP：只读属性
来源：http://fk.szxytkj.cn

public readonly string $name
来源：http://pf.shtwfgs.cn

[U50] PHP：构造器属性提升
来源：http://dw.nicolike.cn

public function __construct(private int $id) {}
来源：http://ax.muxihuayi.cn

[U51] PHP：数组解构
来源：http://fg.szsharing.cn

[$a, $b] = $arr;
来源：http://ip.chemitech.net.cn

[U52] PHP：箭头函数
来源：http://ak.jianghongdianzi.cn

$double = fn($x) => $x * 2;
来源：http://ae.shtwfgs.cn

[U53] PHP：空合并运算符
来源：http://ny.nicolike.cn

$v = $a ?? $b ?? "default";
来源：http://av.muxihuayi.cn

[U54] PHP：空安全调用
来源：http://kb.wgjwhj.cn

$obj?->method()
来源：http://br.shtwfgs.cn

[U55] PHP：match 表达式
来源：http://cl.colortex.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ty.huanxung.cn

[U56] PHP：命名参数
来源：http://ku.shtwfgs.cn

f(a: 1, b: 2)
来源：http://kj.colortex.cn

[U57] PHP：字符串插值
来源：http://ty.panjiajie.cn

"值: {$a}"
来源：http://rm.chemitech.net.cn

[U58] PHP：数组三件套
来源：http://bf.lnxyls.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qr.gzmigu.cn

[U59] PHP：自定义排序
来源：http://ds.huixiangedu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wr.haigaiapp.cn

[U60] PHP：JSON 编解码
来源：http://ga.huanxung.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rb.panjiajie.cn

[U61] PHP：正则
来源：http://zh.huixinmuqiang.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pp.muxihuayi.cn

[U62] PHP：日期对象
来源：http://tl.asd995.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://as.szxytkj.cn

[U63] PHP：文件读写
来源：http://ek.shxzukj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ca.shxzukj.cn

[U64] PHP：目录遍历
来源：http://ua.huixinmuqiang.cn

glob("dir/*.php");  scandir("dir");
来源：http://yy.asd995.cn

[U65] PHP：会话
来源：http://ck.huixiangedu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://le.yuntaijiaju.cn

[U66] PHP：设置 Cookie
来源：http://nm.haigaiapp.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sa.panjiajie.cn

[U67] PHP：处理文件上传
来源：http://il.hahajie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lt.szsharing.cn

[U68] PHP：PDO 连接
来源：http://sg.lnxyls.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uf.szsharing.cn

[U69] PHP：PDO 预处理
来源：http://bv.hnjuh.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sz.huixinmuqiang.cn

[U70] PHP：PDO 事务
来源：http://sm.521024.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xs.haigaiapp.cn

[U71] PHP：抛出异常
来源：http://je.521024.cn

throw new RuntimeException("失败", 500);
来源：http://gu.szxytkj.cn

[U72] PHP：写错误日志
来源：http://zd.bjjhwx.cn

error_log("失败: " . $e->getMessage());
来源：http://hv.yuntaijiaju.cn

[U73] PHP：读取 ini 配置
来源：http://tn.nicolike.cn

parse_ini_file("config.ini", true)
来源：http://rg.bjjhwx.cn

[U74] PHP：读取环境变量
来源：http://vx.huanxung.cn

getenv("APP_ENV") ?: "production"
来源：http://ij.szxytkj.cn

[U75] PHP：依赖注入
来源：http://jx.9csxet.cn

composer require psr/container
来源：http://vc.huixinmuqiang.cn

[U76] PHP：简单路由
来源：http://ss.szxytkj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qc.shtwfgs.cn

[U77] PHP：模板渲染
来源：http://rh.hnjuh.cn

composer require twig/twig
来源：http://hc.521024.cn

[U78] PHP：单元测试
来源：http://rr.jianghongdianzi.cn

composer require --dev phpunit/phpunit
来源：http://hr.gzmigu.cn

[U79] PHP：静态分析
来源：http://lh.szsharing.cn

composer require --dev phpstan/phpstan
来源：http://cy.nicolike.cn

[U80] PHP：代码规范修复
来源：http://we.szxytkj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ih.huixiangedu.cn

[U81] JS：初始化项目
来源：http://zp.muxihuayi.cn

npm init -y;  npm i express
来源：http://xm.szxytkj.cn

[U82] JS：package.json 脚本
来源：http://cd.hnjuh.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gn.haigaiapp.cn

[U83] JS：ES Module 导入导出
来源：http://lv.bookmarksfly.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ht.haigaiapp.cn

[U84] JS：CommonJS 写法
来源：http://oo.lnxyls.cn

module.exports = { a };  const { a } = require("./m");
来源：http://xg.gzmigu.cn

[U85] JS：可选链
来源：http://tx.521024.cn

a?.b?.c
来源：http://ta.shxzukj.cn

[U86] JS：空值合并
来源：http://ow.chemitech.net.cn

a ?? b
来源：http://dv.9csxet.cn

[U87] JS：解构默认值
来源：http://wb.szxytkj.cn

const { a = 1, b = 2 } = obj;
来源：http://ls.hahajie.cn

[U88] JS：对象展开合并
来源：http://ex.hahajie.cn

{ ...a, ...b }
来源：http://vr.shxzskj.cn

[U89] JS：数组去重
来源：http://do.asd995.cn

[...new Set(arr)]
来源：http://jn.panjiajie.cn

[U90] JS：数字数组排序
来源：http://hl.hnjuh.cn

[...arr].sort((a, b) => a - b)
来源：http://rf.hnjuh.cn

[U91] JS：对象键值遍历
来源：http://gn.asd995.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://np.bookmarksfly.cn

[U92] JS：深拷贝
来源：http://rx.gzmigu.cn

structuredClone(obj)
来源：http://wn.panjiajie.cn

[U93] JS：模板字符串
来源：http://jo.gzmigu.cn

`共 ${n} 条`
来源：http://mh.szsharing.cn

[U94] JS：箭头函数
来源：http://zy.asd995.cn

const double = x => x * 2;
来源：http://zq.9csxet.cn

[U95] JS：Promise 包装
来源：http://cj.chemitech.net.cn

new Promise((resolve, reject) => {})
来源：http://mz.szsharing.cn

[U96] JS：async/await 与异常
来源：http://yk.panjiajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://eq.huixinmuqiang.cn

[U97] JS：并发请求
来源：http://ae.huixinmuqiang.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://pp.szxytkj.cn

[U98] JS：fetch 带 JSON
来源：http://wa.bjjhwx.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vv.panjiajie.cn

[U99] JS：事件监听
来源：http://yr.szsharing.cn

el.addEventListener("click", e => {})
来源：http://or.huixinmuqiang.cn

[U100] JS：DOM 查询
来源：http://df.asd995.cn

document.querySelector(".item")
来源：http://hd.9csxet.cn

[U101] JS：classList 操作
来源：http://bz.9csxet.cn

el.classList.toggle("active")
来源：http://kj.hnjuh.cn

[U102] JS：本地存储
来源：http://lv.hahajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://qu.hahajie.cn

[U103] JS：定时器
来源：http://ql.asd995.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ww.bjjhwx.cn

[U104] JS：防抖
来源：http://nh.hahajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lj.gzmigu.cn

[U105] JS：节流
来源：http://xo.huanxung.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://og.wgjwhj.cn

[U106] JS：日期格式化
来源：http://mk.huixiangedu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tz.colortex.cn

[U107] JS：数字千分位
来源：http://on.nicolike.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zh.huixiangedu.cn

[U108] JS：随机整数
来源：http://xv.shxzukj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lk.hahajie.cn

[U109] JS：数组分组
来源：http://eh.gzmigu.cn

Object.groupBy(arr, x => x.type)
来源：http://qx.szsharing.cn

[U110] JS：数组分块
来源：http://hu.nicolike.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rp.yuexingan06.cn

[U111] JS：对象转 Map
来源：http://jy.shtwfgs.cn

new Map(Object.entries(obj))
来源：http://mf.nicolike.cn

[U112] JS：字符串补位
来源：http://tj.gzmigu.cn

"7".padStart(3, "0")
来源：http://ot.huixiangedu.cn

[U113] JS：正则替换全部
来源：http://nd.jianghongdianzi.cn

s.replaceAll("a", "b")
来源：http://sq.huixiangedu.cn

[U114] JS：JSON 深比较
来源：http://ok.szxytkj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://zu.shxzskj.cn

[U115] JS：生成 UUID
来源：http://lo.shxzskj.cn

crypto.randomUUID()
来源：http://vr.bjjhwx.cn

[U116] JS：类型检查（JSDoc）
来源：http://ig.521024.cn

/** @param {string} name */ function f(name) {}
来源：http://tl.szxytkj.cn

[U117] JS：单元测试
来源：http://ki.lnxyls.cn

npm i -D vitest;  npx vitest
来源：http://dd.szxytkj.cn

[U118] JS：开发服务器
来源：http://du.muxihuayi.cn

npm i -D vite;  npx vite
来源：http://ka.szsharing.cn

[U119] JS：生产构建
来源：http://tv.yuntaijiaju.cn

npx vite build
来源：http://wd.gzmigu.cn

[U120] JS：读取环境变量（Vite）
来源：http://hz.hahajie.cn

import.meta.env.VITE_API_URL
来源：http://us.newstarts.cn

================================================================================
来源：http://yj.521024.cn

统计汇总
来源：http://yx.chemitech.net.cn

================================================================================
来源：http://oh.9csxet.cn

按语言统计（条）：
来源：http://gv.huanxung.cn

Python ......... 252
来源：http://rb.9csxet.cn

PHP ............ 252
来源：http://lh.lnxyls.cn

JavaScript ..... 252
来源：http://mk.huixinmuqiang.cn

TypeScript ..... 212
来源：http://sd.wgjwhj.cn

Java ........... 212
来源：http://pj.yuexingan06.cn

Go ............. 212
来源：http://ai.lnxyls.cn

Ruby ........... 212
来源：http://eg.haigaiapp.cn

C# ............. 212
来源：http://yu.panjiajie.cn

C .............. 30
来源：http://cw.haigaiapp.cn

C++ ............ 30
来源：http://hd.asd995.cn

SQL ............ 90
来源：http://he.haigaiapp.cn

Bash ........... 80
来源：http://ds.9csxet.cn

Kotlin ......... 15
来源：http://ia.asd995.cn

Swift .......... 15
来源：http://il.shtwfgs.cn

Lua ............ 10
来源：http://nc.huixinmuqiang.cn

Perl ........... 10
来源：http://js.haigaiapp.cn

Scala .......... 10
来源：http://ua.huixinmuqiang.cn

------------------------------------
来源：http://ai.nszjky.cn

合计 ........... 2106 条
来源：http://hw.lnxyls.cn

按章节统计：
来源：http://dk.chemitech.net.cn


<!-- 参考信息 -->