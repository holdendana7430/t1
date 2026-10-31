代发 wailian999

[T43] Perl：字符串插值
来源：http://fp.szxytkj.cn

"值: $a"
来源：http://yy.muxihuayi.cn

[T44] Perl：条件
来源：http://ih.huanxung.cn

if ($a > 0) { print "正"; }
来源：http://gi.jianghongdianzi.cn

[T45] Perl：数组遍历
来源：http://vs.nicolike.cn

for my $x (@arr) { print $x; }
来源：http://hx.nszjky.cn

[T46] Perl：哈希操作
来源：http://vg.asd995.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zi.nicolike.cn

[T47] Perl：正则捕获
来源：http://pj.haigaiapp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://br.szxytkj.cn

[T48] Perl：正则替换
来源：http://fq.yuexingan06.cn

$s =~ s/old/new/g;
来源：http://td.shxzukj.cn

[T49] Perl：函数
来源：http://lh.bookmarksfly.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.colortex.cn

[T50] Perl：逐行读文件
来源：http://xl.shtwfgs.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wc.huixiangedu.cn

while (my $line = <$fh>) { print $line; }
来源：http://cg.haigaiapp.cn

[T51] Scala：Hello World
来源：http://bd.jctech888.com.cn

println("Hello")
来源：http://bi.bookmarksfly.cn

[T52] Scala：变量
来源：http://rb.yuntaijiaju.cn

val a = 1;  var b = 2
来源：http://de.nszjky.cn

[T53] Scala：字符串插值
来源：http://mc.panjiajie.cn

s"值: $b"
来源：http://ta.chemitech.net.cn

[T54] Scala：集合映射
来源：http://ji.yuexingan06.cn

List(1, 2, 3).map(_ * 2)
来源：http://dw.shxzukj.cn

[T55] Scala：集合过滤
来源：http://lo.shxzukj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://yf.521024.cn

[T56] Scala：样例类
来源：http://df.nszjky.cn

case class User(name: String, age: Int)
来源：http://uz.huixiangedu.cn

[T57] Scala：模式匹配
来源：http://rz.szsharing.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://al.nszjky.cn

[T58] Scala：函数定义
来源：http://cu.jianghongdianzi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://yz.bookmarksfly.cn

[T59] Scala：循环
来源：http://sb.yuexingan06.cn

for (i <- 1 to 10) println(i)
来源：http://ct.lnxyls.cn

[T60] Scala：折叠
来源：http://tx.huanxung.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://at.yuexingan06.cn

================================================================================
来源：http://rt.yuntaijiaju.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wf.shtwfgs.cn

================================================================================
来源：http://hn.chemitech.net.cn

[U01] Py：创建虚拟环境
来源：http://fl.jianghongdianzi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://hg.jctech888.com.cn

[U02] Py：导出 / 安装依赖
来源：http://dc.yuexingan06.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cu.yuexingan06.cn

[U03] Py：加载 .env 配置
来源：http://mc.szsharing.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://hg.bookmarksfly.cn

[U04] Py：变量调试打印
来源：http://no.szxytkj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fd.bookmarksfly.cn

[U05] Py：列表去重且保序
来源：http://kc.hahajie.cn

list(dict.fromkeys(arr))
来源：http://qg.wgjwhj.cn

[U06] Py：合并两个字典
来源：http://qy.hahajie.cn

{**a, **b}
来源：http://cm.wgjwhj.cn

[U07] Py：反转字典键值
来源：http://je.yuexingan06.cn

{v: k for k, v in d.items()}
来源：http://bc.521024.cn

[U08] Py：展平二维列表
来源：http://ce.shtwfgs.cn

[y for x in nested for y in x]
来源：http://nb.shtwfgs.cn

[U09] Py：字典取最大值的键
来源：http://py.shxzukj.cn

max(d, key=d.get)
来源：http://xm.shtwfgs.cn

[U10] Py：按值排序字典
来源：http://wl.yuntaijiaju.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jj.lnxyls.cn

[U11] Py：生成器表达式
来源：http://tj.chemitech.net.cn

(x * 2 for x in arr)
来源：http://do.huixinmuqiang.cn

[U12] Py：取出现最多的 3 个元素
来源：http://tw.asd995.cn

Counter(arr).most_common(3)
来源：http://pz.colortex.cn

[U13] Py：固定长度队列
来源：http://uw.nszjky.cn

deque(maxlen=10)
来源：http://zz.9csxet.cn

[U14] Py：分组收集到列表
来源：http://qs.muxihuayi.cn

defaultdict(list)
来源：http://uc.bjjhwx.cn

[U15] Py：高精度计时
来源：http://qh.9csxet.cn

t = time.perf_counter()
来源：http://jt.huanxung.cn

[U16] Py：命令行参数解析
来源：http://ig.newstarts.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pg.chemitech.net.cn

[U17] Py：初始化日志
来源：http://dq.bjjhwx.cn

logging.basicConfig(level=logging.INFO)
来源：http://fw.yuexingan06.cn

[U18] Py：预编译正则
来源：http://an.jctech888.com.cn

pat = re.compile(r"\d+")
来源：http://ji.9csxet.cn

[U19] Py：正则替换带回调
来源：http://ki.nicolike.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nv.gzmigu.cn

[U20] Py：缓存函数结果
来源：http://vg.shxzukj.cn

@functools.lru_cache(maxsize=None)
来源：http://qf.9csxet.cn

[U21] Py：自定义上下文管理器
来源：http://ew.panjiajie.cn

@contextlib.contextmanager
来源：http://kp.521024.cn

[U22] Py：矩阵转置
来源：http://li.yuexingan06.cn

list(zip(*m))
来源：http://ak.nicolike.cn

[U23] Py：分块读取大文件
来源：http://dn.bookmarksfly.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ch.huanxung.cn

[U24] Py：路径操作
来源：http://mg.521024.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://st.muxihuayi.cn

[U25] Py：CSV 按字典读
来源：http://lb.jctech888.com.cn

csv.DictReader(f)
来源：http://nc.lnxyls.cn

[U26] Py：并发下载
来源：http://jp.colortex.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pc.newstarts.cn

[U27] Py：异步 HTTP
来源：http://vz.yuexingan06.cn

aiohttp.ClientSession() 配合 async with
来源：http://be.newstarts.cn

[U28] Py：类型别名
来源：http://kg.huixiangedu.cn

UserId = int
来源：http://rk.muxihuayi.cn

[U29] Py：属性校验
来源：http://iu.521024.cn

@property 与 @x.setter 配合
来源：http://lv.colortex.cn

[U30] Py：数据类
来源：http://fg.panjiajie.cn

@dataclass(slots=True)
来源：http://ul.bookmarksfly.cn

[U31] Py：单测
来源：http://te.hnjuh.cn

python -m pytest -q
来源：http://jk.bookmarksfly.cn

[U32] Py：代码格式化
来源：http://nt.asd995.cn

ruff format . && ruff check --fix .
来源：http://dv.chemitech.net.cn

[U33] Py：打包发布
来源：http://nt.hnjuh.cn

python -m build  （依赖 pyproject.toml）
来源：http://gp.shxzskj.cn

[U34] Py：判断编码
来源：http://ql.szsharing.cn

chardet.detect(raw)
来源：http://mz.chemitech.net.cn

[U35] Py：发送邮件
来源：http://sa.nszjky.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://sf.jctech888.com.cn

[U36] Py：定时任务
来源：http://gm.bjjhwx.cn

schedule.every(10).minutes.do(job)
来源：http://hh.huanxung.cn

[U37] Py：读写 Excel
来源：http://uq.shtwfgs.cn

pandas.read_excel / DataFrame.to_excel
来源：http://iz.jianghongdianzi.cn

[U38] Py：获取脚本所在目录
来源：http://qe.521024.cn

Path(__file__).resolve().parent
来源：http://kv.9csxet.cn

[U39] Py：判断是否在交互环境
来源：http://mp.asd995.cn

sys.stdout.isatty()
来源：http://fz.9csxet.cn

[U40] Py：打印到标准错误
来源：http://gu.jctech888.com.cn

print("err", file=sys.stderr)
来源：http://ak.shxzukj.cn

[U41] PHP：初始化 Composer 项目
来源：http://kh.szsharing.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://uc.bookmarksfly.cn

[U42] PHP：PSR-4 自动加载
来源：http://db.haigaiapp.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ns.nicolike.cn

[U43] PHP：声明命名空间
来源：http://nl.chemitech.net.cn

namespace App\Http;
来源：http://fv.colortex.cn

[U44] PHP：开启严格类型
来源：http://ee.haigaiapp.cn

declare(strict_types=1);
来源：http://yk.muxihuayi.cn

[U45] PHP：类型声明与返回类型
来源：http://lv.9csxet.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://sb.hnjuh.cn

[U46] PHP：可空类型
来源：http://qo.shxzukj.cn

?string $name = null
来源：http://ec.bjjhwx.cn

[U47] PHP：联合类型
来源：http://xc.yuexingan06.cn

int|string $id
来源：http://uk.yuntaijiaju.cn

[U48] PHP：纯枚举
来源：http://jz.jctech888.com.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yj.9csxet.cn

[U49] PHP：只读属性
来源：http://za.gzmigu.cn

public readonly string $name
来源：http://cb.haigaiapp.cn

[U50] PHP：构造器属性提升
来源：http://hf.yuexingan06.cn

public function __construct(private int $id) {}
来源：http://ne.521024.cn

[U51] PHP：数组解构
来源：http://rm.huanxung.cn

[$a, $b] = $arr;
来源：http://ip.shtwfgs.cn

[U52] PHP：箭头函数
来源：http://xc.muxihuayi.cn

$double = fn($x) => $x * 2;
来源：http://cl.bookmarksfly.cn

[U53] PHP：空合并运算符
来源：http://km.bjjhwx.cn

$v = $a ?? $b ?? "default";
来源：http://me.huanxung.cn

[U54] PHP：空安全调用
来源：http://ho.yuexingan06.cn

$obj?->method()
来源：http://sx.huanxung.cn

[U55] PHP：match 表达式
来源：http://as.huixinmuqiang.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gi.szxytkj.cn

[U56] PHP：命名参数
来源：http://gi.panjiajie.cn

f(a: 1, b: 2)
来源：http://jb.szsharing.cn

[U57] PHP：字符串插值
来源：http://fx.haigaiapp.cn

"值: {$a}"
来源：http://cn.huixinmuqiang.cn

[U58] PHP：数组三件套
来源：http://hg.haigaiapp.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ck.szsharing.cn

[U59] PHP：自定义排序
来源：http://wv.nicolike.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rf.muxihuayi.cn

[U60] PHP：JSON 编解码
来源：http://nk.hahajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ka.colortex.cn

[U61] PHP：正则
来源：http://ql.shtwfgs.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ub.nicolike.cn

[U62] PHP：日期对象
来源：http://gp.9csxet.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ec.muxihuayi.cn

[U63] PHP：文件读写
来源：http://iz.huanxung.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kb.jctech888.com.cn

[U64] PHP：目录遍历
来源：http://py.bookmarksfly.cn

glob("dir/*.php");  scandir("dir");
来源：http://tu.huanxung.cn

[U65] PHP：会话
来源：http://dl.newstarts.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ks.yuexingan06.cn

[U66] PHP：设置 Cookie
来源：http://kg.shtwfgs.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ql.hahajie.cn

[U67] PHP：处理文件上传
来源：http://nm.colortex.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zt.haigaiapp.cn

[U68] PHP：PDO 连接
来源：http://sm.muxihuayi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vk.szxytkj.cn

[U69] PHP：PDO 预处理
来源：http://xr.asd995.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://on.bookmarksfly.cn

[U70] PHP：PDO 事务
来源：http://iw.lnxyls.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lc.9csxet.cn

[U71] PHP：抛出异常
来源：http://dg.huixiangedu.cn

throw new RuntimeException("失败", 500);
来源：http://bb.lnxyls.cn

[U72] PHP：写错误日志
来源：http://jt.huixinmuqiang.cn

error_log("失败: " . $e->getMessage());
来源：http://ns.nicolike.cn

[U73] PHP：读取 ini 配置
来源：http://wr.9csxet.cn

parse_ini_file("config.ini", true)
来源：http://ky.haigaiapp.cn

[U74] PHP：读取环境变量
来源：http://mr.haigaiapp.cn

getenv("APP_ENV") ?: "production"
来源：http://jh.lnxyls.cn

[U75] PHP：依赖注入
来源：http://nw.huixiangedu.cn

composer require psr/container
来源：http://aj.szxytkj.cn

[U76] PHP：简单路由
来源：http://wj.yuntaijiaju.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vk.asd995.cn

[U77] PHP：模板渲染
来源：http://df.jctech888.com.cn

composer require twig/twig
来源：http://kc.hnjuh.cn

[U78] PHP：单元测试
来源：http://qy.shxzskj.cn

composer require --dev phpunit/phpunit
来源：http://pq.huixinmuqiang.cn

[U79] PHP：静态分析
来源：http://qa.bookmarksfly.cn

composer require --dev phpstan/phpstan
来源：http://dl.shxzukj.cn

[U80] PHP：代码规范修复
来源：http://mm.yuntaijiaju.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://bi.chemitech.net.cn

[U81] JS：初始化项目
来源：http://ja.shxzskj.cn

npm init -y;  npm i express
来源：http://nx.shtwfgs.cn

[U82] JS：package.json 脚本
来源：http://nc.521024.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zb.asd995.cn

[U83] JS：ES Module 导入导出
来源：http://lm.shxzukj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vm.521024.cn

[U84] JS：CommonJS 写法
来源：http://ja.nszjky.cn

module.exports = { a };  const { a } = require("./m");
来源：http://te.yuexingan06.cn

[U85] JS：可选链
来源：http://ah.gzmigu.cn

a?.b?.c
来源：http://za.9csxet.cn

[U86] JS：空值合并
来源：http://fn.colortex.cn

a ?? b
来源：http://ro.shxzskj.cn

[U87] JS：解构默认值
来源：http://ld.chemitech.net.cn

const { a = 1, b = 2 } = obj;
来源：http://va.shtwfgs.cn

[U88] JS：对象展开合并
来源：http://zk.szxytkj.cn

{ ...a, ...b }
来源：http://ts.panjiajie.cn

[U89] JS：数组去重
来源：http://ld.huanxung.cn

[...new Set(arr)]
来源：http://av.yuexingan06.cn

[U90] JS：数字数组排序
来源：http://rn.chemitech.net.cn

[...arr].sort((a, b) => a - b)
来源：http://am.hnjuh.cn

[U91] JS：对象键值遍历
来源：http://fo.hnjuh.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://be.huixinmuqiang.cn

[U92] JS：深拷贝
来源：http://nq.huanxung.cn

structuredClone(obj)
来源：http://ij.wgjwhj.cn

[U93] JS：模板字符串
来源：http://at.colortex.cn

`共 ${n} 条`
来源：http://de.chemitech.net.cn

[U94] JS：箭头函数
来源：http://jy.haigaiapp.cn

const double = x => x * 2;
来源：http://wg.hnjuh.cn

[U95] JS：Promise 包装
来源：http://dc.jianghongdianzi.cn

new Promise((resolve, reject) => {})
来源：http://cw.haigaiapp.cn

[U96] JS：async/await 与异常
来源：http://ps.wgjwhj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pl.lnxyls.cn

[U97] JS：并发请求
来源：http://fe.wgjwhj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://hm.nszjky.cn

[U98] JS：fetch 带 JSON
来源：http://or.bjjhwx.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cx.bookmarksfly.cn

[U99] JS：事件监听
来源：http://qp.521024.cn

el.addEventListener("click", e => {})
来源：http://ly.shtwfgs.cn

[U100] JS：DOM 查询
来源：http://zt.haigaiapp.cn

document.querySelector(".item")
来源：http://wi.asd995.cn

[U101] JS：classList 操作
来源：http://io.bookmarksfly.cn

el.classList.toggle("active")
来源：http://bo.panjiajie.cn

[U102] JS：本地存储
来源：http://qj.muxihuayi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://rv.bjjhwx.cn

[U103] JS：定时器
来源：http://ph.bjjhwx.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ig.wgjwhj.cn

[U104] JS：防抖
来源：http://up.szxytkj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://na.bookmarksfly.cn

[U105] JS：节流
来源：http://kt.yuexingan06.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ni.jianghongdianzi.cn

[U106] JS：日期格式化
来源：http://ys.haigaiapp.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://eh.nicolike.cn

[U107] JS：数字千分位
来源：http://wk.asd995.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hk.huixinmuqiang.cn

[U108] JS：随机整数
来源：http://vx.521024.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pe.9csxet.cn

[U109] JS：数组分组
来源：http://cz.newstarts.cn

Object.groupBy(arr, x => x.type)
来源：http://mh.muxihuayi.cn

[U110] JS：数组分块
来源：http://qr.nszjky.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://va.nszjky.cn

[U111] JS：对象转 Map
来源：http://vp.huixinmuqiang.cn

new Map(Object.entries(obj))
来源：http://bh.asd995.cn

[U112] JS：字符串补位
来源：http://nq.colortex.cn

"7".padStart(3, "0")
来源：http://pd.bookmarksfly.cn

[U113] JS：正则替换全部
来源：http://ys.yuntaijiaju.cn

s.replaceAll("a", "b")
来源：http://vm.haigaiapp.cn

[U114] JS：JSON 深比较
来源：http://hq.shtwfgs.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://mc.nicolike.cn

[U115] JS：生成 UUID
来源：http://dk.nszjky.cn

crypto.randomUUID()
来源：http://ym.9csxet.cn

[U116] JS：类型检查（JSDoc）
来源：http://tl.9csxet.cn

/** @param {string} name */ function f(name) {}
来源：http://uo.wgjwhj.cn

[U117] JS：单元测试
来源：http://th.asd995.cn

npm i -D vitest;  npx vitest
来源：http://og.shxzukj.cn

[U118] JS：开发服务器
来源：http://xg.haigaiapp.cn

npm i -D vite;  npx vite
来源：http://wt.jctech888.com.cn

[U119] JS：生产构建
来源：http://dg.9csxet.cn

npx vite build
来源：http://nm.hnjuh.cn

[U120] JS：读取环境变量（Vite）
来源：http://mh.panjiajie.cn

import.meta.env.VITE_API_URL
来源：http://ws.9csxet.cn

================================================================================
来源：http://mu.chemitech.net.cn

统计汇总
来源：http://wu.asd995.cn

================================================================================
来源：http://ch.shtwfgs.cn

按语言统计（条）：
来源：http://xf.newstarts.cn

Python ......... 252
来源：http://sc.lnxyls.cn

PHP ............ 252
来源：http://jd.hahajie.cn

JavaScript ..... 252
来源：http://ly.bjjhwx.cn

TypeScript ..... 212
来源：http://le.huixiangedu.cn

Java ........... 212
来源：http://tk.yuntaijiaju.cn

Go ............. 212
来源：http://cl.haigaiapp.cn

Ruby ........... 212
来源：http://vq.521024.cn

C# ............. 212
来源：http://bp.asd995.cn

C .............. 30
来源：http://mu.asd995.cn

C++ ............ 30
来源：http://yb.yuexingan06.cn

SQL ............ 90
来源：http://zc.asd995.cn

Bash ........... 80
来源：http://tv.nicolike.cn

Kotlin ......... 15
来源：http://sd.huixinmuqiang.cn

Swift .......... 15
来源：http://hj.shxzukj.cn

Lua ............ 10
来源：http://yk.9csxet.cn

Perl ........... 10
来源：http://aq.nicolike.cn


<!-- 参考信息 -->