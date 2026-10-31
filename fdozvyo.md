代发 wailian999

[T47] Perl：正则捕获
来源：http://ho.szsharing.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://yy.bookmarksfly.cn

[T48] Perl：正则替换
来源：http://cj.szxytkj.cn

$s =~ s/old/new/g;
来源：http://ez.chemitech.net.cn

[T49] Perl：函数
来源：http://zg.chemitech.net.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hg.lnxyls.cn

[T50] Perl：逐行读文件
来源：http://dh.muxihuayi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ql.9csxet.cn

while (my $line = <$fh>) { print $line; }
来源：http://zt.shtwfgs.cn

[T51] Scala：Hello World
来源：http://ce.9csxet.cn

println("Hello")
来源：http://pw.9csxet.cn

[T52] Scala：变量
来源：http://lz.lnxyls.cn

val a = 1;  var b = 2
来源：http://fd.yuntaijiaju.cn

[T53] Scala：字符串插值
来源：http://pv.gzmigu.cn

s"值: $b"
来源：http://ew.521024.cn

[T54] Scala：集合映射
来源：http://oq.nszjky.cn

List(1, 2, 3).map(_ * 2)
来源：http://bi.szsharing.cn

[T55] Scala：集合过滤
来源：http://hw.szsharing.cn

List(1, 2, 3).filter(_ > 1)
来源：http://dv.yuexingan06.cn

[T56] Scala：样例类
来源：http://sd.521024.cn

case class User(name: String, age: Int)
来源：http://ae.hahajie.cn

[T57] Scala：模式匹配
来源：http://xi.muxihuayi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://yg.hnjuh.cn

[T58] Scala：函数定义
来源：http://mx.colortex.cn

def add(a: Int, b: Int): Int = a + b
来源：http://yz.huixinmuqiang.cn

[T59] Scala：循环
来源：http://lw.huanxung.cn

for (i <- 1 to 10) println(i)
来源：http://sa.huanxung.cn

[T60] Scala：折叠
来源：http://wr.yuexingan06.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zp.haigaiapp.cn

================================================================================
来源：http://qh.wgjwhj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cp.jctech888.com.cn

================================================================================
来源：http://tx.gzmigu.cn

[U01] Py：创建虚拟环境
来源：http://ub.chemitech.net.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ww.asd995.cn

[U02] Py：导出 / 安装依赖
来源：http://gr.yuntaijiaju.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zy.huanxung.cn

[U03] Py：加载 .env 配置
来源：http://pi.hnjuh.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fs.lnxyls.cn

[U04] Py：变量调试打印
来源：http://nk.gzmigu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jr.hnjuh.cn

[U05] Py：列表去重且保序
来源：http://xl.bookmarksfly.cn

list(dict.fromkeys(arr))
来源：http://hk.yuntaijiaju.cn

[U06] Py：合并两个字典
来源：http://og.huixiangedu.cn

{**a, **b}
来源：http://xl.huanxung.cn

[U07] Py：反转字典键值
来源：http://bw.huanxung.cn

{v: k for k, v in d.items()}
来源：http://qm.yuntaijiaju.cn

[U08] Py：展平二维列表
来源：http://eu.shxzskj.cn

[y for x in nested for y in x]
来源：http://zy.panjiajie.cn

[U09] Py：字典取最大值的键
来源：http://hs.colortex.cn

max(d, key=d.get)
来源：http://bd.szsharing.cn

[U10] Py：按值排序字典
来源：http://wo.hnjuh.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fb.hnjuh.cn

[U11] Py：生成器表达式
来源：http://im.9csxet.cn

(x * 2 for x in arr)
来源：http://gx.shxzukj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ip.9csxet.cn

Counter(arr).most_common(3)
来源：http://dj.szxytkj.cn

[U13] Py：固定长度队列
来源：http://aj.asd995.cn

deque(maxlen=10)
来源：http://qm.jctech888.com.cn

[U14] Py：分组收集到列表
来源：http://od.panjiajie.cn

defaultdict(list)
来源：http://fv.lnxyls.cn

[U15] Py：高精度计时
来源：http://rw.yuntaijiaju.cn

t = time.perf_counter()
来源：http://qs.huixinmuqiang.cn

[U16] Py：命令行参数解析
来源：http://pw.shxzskj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nz.muxihuayi.cn

[U17] Py：初始化日志
来源：http://om.huanxung.cn

logging.basicConfig(level=logging.INFO)
来源：http://jb.bookmarksfly.cn

[U18] Py：预编译正则
来源：http://hs.hahajie.cn

pat = re.compile(r"\d+")
来源：http://ny.panjiajie.cn

[U19] Py：正则替换带回调
来源：http://js.newstarts.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yu.asd995.cn

[U20] Py：缓存函数结果
来源：http://gu.shtwfgs.cn

@functools.lru_cache(maxsize=None)
来源：http://wg.jctech888.com.cn

[U21] Py：自定义上下文管理器
来源：http://cv.shxzskj.cn

@contextlib.contextmanager
来源：http://ah.jctech888.com.cn

[U22] Py：矩阵转置
来源：http://bv.chemitech.net.cn

list(zip(*m))
来源：http://vu.szxytkj.cn

[U23] Py：分块读取大文件
来源：http://vi.asd995.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xm.lnxyls.cn

[U24] Py：路径操作
来源：http://jx.shxzskj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ff.colortex.cn

[U25] Py：CSV 按字典读
来源：http://rm.jianghongdianzi.cn

csv.DictReader(f)
来源：http://jf.jctech888.com.cn

[U26] Py：并发下载
来源：http://rg.colortex.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ln.bookmarksfly.cn

[U27] Py：异步 HTTP
来源：http://vb.gzmigu.cn

aiohttp.ClientSession() 配合 async with
来源：http://nt.haigaiapp.cn

[U28] Py：类型别名
来源：http://zo.huixiangedu.cn

UserId = int
来源：http://wd.hahajie.cn

[U29] Py：属性校验
来源：http://zx.jctech888.com.cn

@property 与 @x.setter 配合
来源：http://nz.panjiajie.cn

[U30] Py：数据类
来源：http://yw.nszjky.cn

@dataclass(slots=True)
来源：http://wv.bjjhwx.cn

[U31] Py：单测
来源：http://rf.colortex.cn

python -m pytest -q
来源：http://kb.9csxet.cn

[U32] Py：代码格式化
来源：http://nh.haigaiapp.cn

ruff format . && ruff check --fix .
来源：http://yr.muxihuayi.cn

[U33] Py：打包发布
来源：http://os.nszjky.cn

python -m build  （依赖 pyproject.toml）
来源：http://nn.bookmarksfly.cn

[U34] Py：判断编码
来源：http://mw.szsharing.cn

chardet.detect(raw)
来源：http://bj.jianghongdianzi.cn

[U35] Py：发送邮件
来源：http://rm.panjiajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://oc.shxzukj.cn

[U36] Py：定时任务
来源：http://gk.newstarts.cn

schedule.every(10).minutes.do(job)
来源：http://ij.huixinmuqiang.cn

[U37] Py：读写 Excel
来源：http://dc.panjiajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://pl.haigaiapp.cn

[U38] Py：获取脚本所在目录
来源：http://am.asd995.cn

Path(__file__).resolve().parent
来源：http://zt.jianghongdianzi.cn

[U39] Py：判断是否在交互环境
来源：http://km.521024.cn

sys.stdout.isatty()
来源：http://ap.chemitech.net.cn

[U40] Py：打印到标准错误
来源：http://un.gzmigu.cn

print("err", file=sys.stderr)
来源：http://rq.szxytkj.cn

[U41] PHP：初始化 Composer 项目
来源：http://mi.huanxung.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://tj.nszjky.cn

[U42] PHP：PSR-4 自动加载
来源：http://ez.szxytkj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ex.nicolike.cn

[U43] PHP：声明命名空间
来源：http://mo.bjjhwx.cn

namespace App\Http;
来源：http://zt.nicolike.cn

[U44] PHP：开启严格类型
来源：http://ys.shtwfgs.cn

declare(strict_types=1);
来源：http://dh.bjjhwx.cn

[U45] PHP：类型声明与返回类型
来源：http://lg.huixiangedu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://cd.shtwfgs.cn

[U46] PHP：可空类型
来源：http://jg.chemitech.net.cn

?string $name = null
来源：http://tt.9csxet.cn

[U47] PHP：联合类型
来源：http://tk.panjiajie.cn

int|string $id
来源：http://vs.huixiangedu.cn

[U48] PHP：纯枚举
来源：http://cz.shtwfgs.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cv.bjjhwx.cn

[U49] PHP：只读属性
来源：http://kg.newstarts.cn

public readonly string $name
来源：http://hg.yuexingan06.cn

[U50] PHP：构造器属性提升
来源：http://cn.bookmarksfly.cn

public function __construct(private int $id) {}
来源：http://ht.muxihuayi.cn

[U51] PHP：数组解构
来源：http://wv.shtwfgs.cn

[$a, $b] = $arr;
来源：http://oy.huanxung.cn

[U52] PHP：箭头函数
来源：http://zf.shxzukj.cn

$double = fn($x) => $x * 2;
来源：http://si.shxzskj.cn

[U53] PHP：空合并运算符
来源：http://bu.hnjuh.cn

$v = $a ?? $b ?? "default";
来源：http://ay.wgjwhj.cn

[U54] PHP：空安全调用
来源：http://fm.muxihuayi.cn

$obj?->method()
来源：http://aj.hnjuh.cn

[U55] PHP：match 表达式
来源：http://xe.huixiangedu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ix.bookmarksfly.cn

[U56] PHP：命名参数
来源：http://gf.bookmarksfly.cn

f(a: 1, b: 2)
来源：http://ma.szsharing.cn

[U57] PHP：字符串插值
来源：http://tq.yuntaijiaju.cn

"值: {$a}"
来源：http://ib.asd995.cn

[U58] PHP：数组三件套
来源：http://kk.521024.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mi.gzmigu.cn

[U59] PHP：自定义排序
来源：http://vy.chemitech.net.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://as.huixinmuqiang.cn

[U60] PHP：JSON 编解码
来源：http://yt.bjjhwx.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hf.521024.cn

[U61] PHP：正则
来源：http://ke.nszjky.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wr.hnjuh.cn

[U62] PHP：日期对象
来源：http://qb.shxzukj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ma.szsharing.cn

[U63] PHP：文件读写
来源：http://sn.haigaiapp.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://df.colortex.cn

[U64] PHP：目录遍历
来源：http://qh.huanxung.cn

glob("dir/*.php");  scandir("dir");
来源：http://fh.bookmarksfly.cn

[U65] PHP：会话
来源：http://hy.shxzskj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vx.nszjky.cn

[U66] PHP：设置 Cookie
来源：http://dx.9csxet.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xn.newstarts.cn

[U67] PHP：处理文件上传
来源：http://fq.lnxyls.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zp.szsharing.cn

[U68] PHP：PDO 连接
来源：http://mm.nicolike.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wh.shxzskj.cn

[U69] PHP：PDO 预处理
来源：http://wv.lnxyls.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ny.chemitech.net.cn

[U70] PHP：PDO 事务
来源：http://ur.nszjky.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://li.gzmigu.cn

[U71] PHP：抛出异常
来源：http://gx.hahajie.cn

throw new RuntimeException("失败", 500);
来源：http://ad.jctech888.com.cn

[U72] PHP：写错误日志
来源：http://xx.newstarts.cn

error_log("失败: " . $e->getMessage());
来源：http://ov.huanxung.cn

[U73] PHP：读取 ini 配置
来源：http://rk.newstarts.cn

parse_ini_file("config.ini", true)
来源：http://zq.bookmarksfly.cn

[U74] PHP：读取环境变量
来源：http://nr.haigaiapp.cn

getenv("APP_ENV") ?: "production"
来源：http://dq.shxzskj.cn

[U75] PHP：依赖注入
来源：http://hy.panjiajie.cn

composer require psr/container
来源：http://sr.huixinmuqiang.cn

[U76] PHP：简单路由
来源：http://sa.szxytkj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lj.bjjhwx.cn

[U77] PHP：模板渲染
来源：http://bt.yuntaijiaju.cn

composer require twig/twig
来源：http://ro.asd995.cn

[U78] PHP：单元测试
来源：http://kr.yuntaijiaju.cn

composer require --dev phpunit/phpunit
来源：http://ko.nszjky.cn

[U79] PHP：静态分析
来源：http://wk.yuexingan06.cn

composer require --dev phpstan/phpstan
来源：http://qa.yuexingan06.cn

[U80] PHP：代码规范修复
来源：http://ge.colortex.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://dr.asd995.cn

[U81] JS：初始化项目
来源：http://zp.chemitech.net.cn

npm init -y;  npm i express
来源：http://vj.panjiajie.cn

[U82] JS：package.json 脚本
来源：http://jv.szxytkj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ex.wgjwhj.cn

[U83] JS：ES Module 导入导出
来源：http://mm.nszjky.cn

export const a = 1;  import { a } from "./m.js";
来源：http://lf.bjjhwx.cn

[U84] JS：CommonJS 写法
来源：http://gr.yuexingan06.cn

module.exports = { a };  const { a } = require("./m");
来源：http://pk.nicolike.cn

[U85] JS：可选链
来源：http://zj.colortex.cn

a?.b?.c
来源：http://kk.lnxyls.cn

[U86] JS：空值合并
来源：http://rs.huixiangedu.cn

a ?? b
来源：http://fz.nszjky.cn

[U87] JS：解构默认值
来源：http://st.huanxung.cn

const { a = 1, b = 2 } = obj;
来源：http://eb.shxzukj.cn

[U88] JS：对象展开合并
来源：http://xo.wgjwhj.cn

{ ...a, ...b }
来源：http://cn.colortex.cn

[U89] JS：数组去重
来源：http://iz.huixinmuqiang.cn

[...new Set(arr)]
来源：http://nw.bookmarksfly.cn

[U90] JS：数字数组排序
来源：http://xb.huixinmuqiang.cn

[...arr].sort((a, b) => a - b)
来源：http://qo.bjjhwx.cn

[U91] JS：对象键值遍历
来源：http://dm.jianghongdianzi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://au.muxihuayi.cn

[U92] JS：深拷贝
来源：http://sc.nszjky.cn

structuredClone(obj)
来源：http://mv.huixinmuqiang.cn

[U93] JS：模板字符串
来源：http://fg.newstarts.cn

`共 ${n} 条`
来源：http://ct.bjjhwx.cn

[U94] JS：箭头函数
来源：http://rn.haigaiapp.cn

const double = x => x * 2;
来源：http://ju.wgjwhj.cn

[U95] JS：Promise 包装
来源：http://us.nszjky.cn

new Promise((resolve, reject) => {})
来源：http://zl.nszjky.cn

[U96] JS：async/await 与异常
来源：http://qr.nszjky.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ft.wgjwhj.cn

[U97] JS：并发请求
来源：http://jo.shxzukj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://xm.colortex.cn

[U98] JS：fetch 带 JSON
来源：http://kr.hnjuh.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dp.huanxung.cn

[U99] JS：事件监听
来源：http://ol.szxytkj.cn

el.addEventListener("click", e => {})
来源：http://bx.yuntaijiaju.cn

[U100] JS：DOM 查询
来源：http://ur.nicolike.cn

document.querySelector(".item")
来源：http://ly.colortex.cn

[U101] JS：classList 操作
来源：http://cc.newstarts.cn

el.classList.toggle("active")
来源：http://in.nszjky.cn

[U102] JS：本地存储
来源：http://vp.hnjuh.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://es.gzmigu.cn

[U103] JS：定时器
来源：http://xs.hahajie.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://aq.521024.cn

[U104] JS：防抖
来源：http://vo.szsharing.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ma.huixinmuqiang.cn

[U105] JS：节流
来源：http://lj.shtwfgs.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dm.nicolike.cn

[U106] JS：日期格式化
来源：http://rt.szsharing.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xd.nicolike.cn

[U107] JS：数字千分位
来源：http://gz.wgjwhj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://my.bookmarksfly.cn

[U108] JS：随机整数
来源：http://xa.bjjhwx.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cf.shxzukj.cn

[U109] JS：数组分组
来源：http://uk.huixinmuqiang.cn

Object.groupBy(arr, x => x.type)
来源：http://yh.szxytkj.cn

[U110] JS：数组分块
来源：http://kg.nszjky.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qm.haigaiapp.cn

[U111] JS：对象转 Map
来源：http://tn.shxzukj.cn

new Map(Object.entries(obj))
来源：http://do.521024.cn

[U112] JS：字符串补位
来源：http://vg.shtwfgs.cn

"7".padStart(3, "0")
来源：http://el.bjjhwx.cn

[U113] JS：正则替换全部
来源：http://re.asd995.cn

s.replaceAll("a", "b")
来源：http://tn.szxytkj.cn

[U114] JS：JSON 深比较
来源：http://cr.panjiajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://fo.jianghongdianzi.cn

[U115] JS：生成 UUID
来源：http://ap.521024.cn

crypto.randomUUID()
来源：http://sb.gzmigu.cn

[U116] JS：类型检查（JSDoc）
来源：http://xi.shxzukj.cn

/** @param {string} name */ function f(name) {}
来源：http://hf.lnxyls.cn

[U117] JS：单元测试
来源：http://ib.jianghongdianzi.cn

npm i -D vitest;  npx vitest
来源：http://wn.hnjuh.cn

[U118] JS：开发服务器
来源：http://yh.shtwfgs.cn

npm i -D vite;  npx vite
来源：http://oq.gzmigu.cn

[U119] JS：生产构建
来源：http://rp.jctech888.com.cn

npx vite build
来源：http://df.panjiajie.cn

[U120] JS：读取环境变量（Vite）
来源：http://uf.nszjky.cn

import.meta.env.VITE_API_URL
来源：http://ts.hahajie.cn

================================================================================
来源：http://rt.muxihuayi.cn

统计汇总
来源：http://zo.shtwfgs.cn

================================================================================
来源：http://yo.hahajie.cn

按语言统计（条）：
来源：http://km.yuexingan06.cn

Python ......... 252
来源：http://ob.yuntaijiaju.cn

PHP ............ 252
来源：http://tc.szxytkj.cn

JavaScript ..... 252
来源：http://du.huixinmuqiang.cn

TypeScript ..... 212
来源：http://yx.lnxyls.cn

Java ........... 212
来源：http://ae.bookmarksfly.cn

Go ............. 212
来源：http://zm.szsharing.cn

Ruby ........... 212
来源：http://zl.colortex.cn

C# ............. 212
来源：http://pd.nszjky.cn

C .............. 30
来源：http://yc.gzmigu.cn

C++ ............ 30
来源：http://kj.hnjuh.cn

SQL ............ 90
来源：http://tx.wgjwhj.cn

Bash ........... 80
来源：http://ln.gzmigu.cn

Kotlin ......... 15
来源：http://vt.huanxung.cn

Swift .......... 15
来源：http://tr.bjjhwx.cn

Lua ............ 10
来源：http://wt.newstarts.cn

Perl ........... 10
来源：http://bd.lnxyls.cn

Scala .......... 10
来源：http://vc.panjiajie.cn

------------------------------------
来源：http://er.gzmigu.cn

合计 ........... 2106 条
来源：http://ux.szxytkj.cn

按章节统计：
来源：http://xv.nszjky.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gc.chemitech.net.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gz.shxzskj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xx.bookmarksfly.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ug.huanxung.cn


<!-- 参考信息 -->