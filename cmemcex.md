代发 wailian999

[T45] Perl：数组遍历
来源：http://yb.shtwfgs.cn

for my $x (@arr) { print $x; }
来源：http://gr.muxihuayi.cn

[T46] Perl：哈希操作
来源：http://kp.lnxyls.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nb.panjiajie.cn

[T47] Perl：正则捕获
来源：http://xa.huanxung.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ob.huixinmuqiang.cn

[T48] Perl：正则替换
来源：http://hr.bjjhwx.cn

$s =~ s/old/new/g;
来源：http://ls.chemitech.net.cn

[T49] Perl：函数
来源：http://je.szxytkj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://up.jianghongdianzi.cn

[T50] Perl：逐行读文件
来源：http://ye.shxzukj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ob.panjiajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://in.gzmigu.cn

[T51] Scala：Hello World
来源：http://zh.bookmarksfly.cn

println("Hello")
来源：http://pw.szxytkj.cn

[T52] Scala：变量
来源：http://jr.wgjwhj.cn

val a = 1;  var b = 2
来源：http://nu.jctech888.com.cn

[T53] Scala：字符串插值
来源：http://dp.panjiajie.cn

s"值: $b"
来源：http://hm.colortex.cn

[T54] Scala：集合映射
来源：http://jh.asd995.cn

List(1, 2, 3).map(_ * 2)
来源：http://sj.huanxung.cn

[T55] Scala：集合过滤
来源：http://xw.lnxyls.cn

List(1, 2, 3).filter(_ > 1)
来源：http://hv.yuexingan06.cn

[T56] Scala：样例类
来源：http://sy.jctech888.com.cn

case class User(name: String, age: Int)
来源：http://lj.muxihuayi.cn

[T57] Scala：模式匹配
来源：http://ym.9csxet.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://rx.panjiajie.cn

[T58] Scala：函数定义
来源：http://ss.yuntaijiaju.cn

def add(a: Int, b: Int): Int = a + b
来源：http://za.shtwfgs.cn

[T59] Scala：循环
来源：http://wt.huixiangedu.cn

for (i <- 1 to 10) println(i)
来源：http://gl.huanxung.cn

[T60] Scala：折叠
来源：http://ed.wgjwhj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lw.jianghongdianzi.cn

================================================================================
来源：http://ux.newstarts.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ue.colortex.cn

================================================================================
来源：http://de.huanxung.cn

[U01] Py：创建虚拟环境
来源：http://mo.newstarts.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vh.hnjuh.cn

[U02] Py：导出 / 安装依赖
来源：http://cu.lnxyls.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mv.shtwfgs.cn

[U03] Py：加载 .env 配置
来源：http://gr.shxzskj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xq.bjjhwx.cn

[U04] Py：变量调试打印
来源：http://vr.szxytkj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://es.huixinmuqiang.cn

[U05] Py：列表去重且保序
来源：http://ei.jianghongdianzi.cn

list(dict.fromkeys(arr))
来源：http://qh.shxzukj.cn

[U06] Py：合并两个字典
来源：http://cb.asd995.cn

{**a, **b}
来源：http://oa.jianghongdianzi.cn

[U07] Py：反转字典键值
来源：http://fl.colortex.cn

{v: k for k, v in d.items()}
来源：http://to.asd995.cn

[U08] Py：展平二维列表
来源：http://yo.jctech888.com.cn

[y for x in nested for y in x]
来源：http://bp.muxihuayi.cn

[U09] Py：字典取最大值的键
来源：http://nx.hahajie.cn

max(d, key=d.get)
来源：http://sm.haigaiapp.cn

[U10] Py：按值排序字典
来源：http://oj.521024.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uh.shtwfgs.cn

[U11] Py：生成器表达式
来源：http://rc.jianghongdianzi.cn

(x * 2 for x in arr)
来源：http://rw.gzmigu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://hh.huixiangedu.cn

Counter(arr).most_common(3)
来源：http://rk.huixiangedu.cn

[U13] Py：固定长度队列
来源：http://mj.muxihuayi.cn

deque(maxlen=10)
来源：http://rj.jianghongdianzi.cn

[U14] Py：分组收集到列表
来源：http://nl.nszjky.cn

defaultdict(list)
来源：http://cp.hahajie.cn

[U15] Py：高精度计时
来源：http://fk.huixiangedu.cn

t = time.perf_counter()
来源：http://bk.shxzukj.cn

[U16] Py：命令行参数解析
来源：http://zs.521024.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://no.nszjky.cn

[U17] Py：初始化日志
来源：http://fe.panjiajie.cn

logging.basicConfig(level=logging.INFO)
来源：http://de.bjjhwx.cn

[U18] Py：预编译正则
来源：http://kn.jianghongdianzi.cn

pat = re.compile(r"\d+")
来源：http://at.hnjuh.cn

[U19] Py：正则替换带回调
来源：http://hn.huixiangedu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ps.shtwfgs.cn

[U20] Py：缓存函数结果
来源：http://ek.bjjhwx.cn

@functools.lru_cache(maxsize=None)
来源：http://by.wgjwhj.cn

[U21] Py：自定义上下文管理器
来源：http://uq.muxihuayi.cn

@contextlib.contextmanager
来源：http://va.colortex.cn

[U22] Py：矩阵转置
来源：http://xv.haigaiapp.cn

list(zip(*m))
来源：http://cr.huixinmuqiang.cn

[U23] Py：分块读取大文件
来源：http://mb.hahajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cc.shxzukj.cn

[U24] Py：路径操作
来源：http://zk.huanxung.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://eb.yuntaijiaju.cn

[U25] Py：CSV 按字典读
来源：http://ps.panjiajie.cn

csv.DictReader(f)
来源：http://hf.huanxung.cn

[U26] Py：并发下载
来源：http://mf.chemitech.net.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zz.huixinmuqiang.cn

[U27] Py：异步 HTTP
来源：http://xl.hnjuh.cn

aiohttp.ClientSession() 配合 async with
来源：http://gq.shxzukj.cn

[U28] Py：类型别名
来源：http://qi.szxytkj.cn

UserId = int
来源：http://tw.nszjky.cn

[U29] Py：属性校验
来源：http://cb.szsharing.cn

@property 与 @x.setter 配合
来源：http://ul.huixiangedu.cn

[U30] Py：数据类
来源：http://xd.panjiajie.cn

@dataclass(slots=True)
来源：http://nu.shtwfgs.cn

[U31] Py：单测
来源：http://sm.chemitech.net.cn

python -m pytest -q
来源：http://mn.nszjky.cn

[U32] Py：代码格式化
来源：http://ru.9csxet.cn

ruff format . && ruff check --fix .
来源：http://qd.bookmarksfly.cn

[U33] Py：打包发布
来源：http://lj.huixiangedu.cn

python -m build  （依赖 pyproject.toml）
来源：http://zn.szsharing.cn

[U34] Py：判断编码
来源：http://hw.asd995.cn

chardet.detect(raw)
来源：http://wt.521024.cn

[U35] Py：发送邮件
来源：http://yi.shxzukj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gg.huixiangedu.cn

[U36] Py：定时任务
来源：http://fy.9csxet.cn

schedule.every(10).minutes.do(job)
来源：http://vw.huixinmuqiang.cn

[U37] Py：读写 Excel
来源：http://tp.yuexingan06.cn

pandas.read_excel / DataFrame.to_excel
来源：http://bd.lnxyls.cn

[U38] Py：获取脚本所在目录
来源：http://uq.hnjuh.cn

Path(__file__).resolve().parent
来源：http://ml.asd995.cn

[U39] Py：判断是否在交互环境
来源：http://mo.hnjuh.cn

sys.stdout.isatty()
来源：http://pd.yuntaijiaju.cn

[U40] Py：打印到标准错误
来源：http://mi.newstarts.cn

print("err", file=sys.stderr)
来源：http://rl.shtwfgs.cn

[U41] PHP：初始化 Composer 项目
来源：http://xi.yuntaijiaju.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://dq.yuexingan06.cn

[U42] PHP：PSR-4 自动加载
来源：http://ie.szxytkj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qt.huixiangedu.cn

[U43] PHP：声明命名空间
来源：http://ik.lnxyls.cn

namespace App\Http;
来源：http://ul.szsharing.cn

[U44] PHP：开启严格类型
来源：http://jq.haigaiapp.cn

declare(strict_types=1);
来源：http://ir.szxytkj.cn

[U45] PHP：类型声明与返回类型
来源：http://kq.bjjhwx.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://uw.shxzskj.cn

[U46] PHP：可空类型
来源：http://co.nszjky.cn

?string $name = null
来源：http://li.nicolike.cn

[U47] PHP：联合类型
来源：http://ck.nszjky.cn

int|string $id
来源：http://zy.newstarts.cn

[U48] PHP：纯枚举
来源：http://yp.jianghongdianzi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://et.521024.cn

[U49] PHP：只读属性
来源：http://qh.huixiangedu.cn

public readonly string $name
来源：http://hx.hnjuh.cn

[U50] PHP：构造器属性提升
来源：http://ly.szsharing.cn

public function __construct(private int $id) {}
来源：http://di.shxzskj.cn

[U51] PHP：数组解构
来源：http://vm.huixiangedu.cn

[$a, $b] = $arr;
来源：http://kj.hahajie.cn

[U52] PHP：箭头函数
来源：http://zj.szsharing.cn

$double = fn($x) => $x * 2;
来源：http://av.521024.cn

[U53] PHP：空合并运算符
来源：http://tk.muxihuayi.cn

$v = $a ?? $b ?? "default";
来源：http://mc.szxytkj.cn

[U54] PHP：空安全调用
来源：http://nb.huixiangedu.cn

$obj?->method()
来源：http://me.nszjky.cn

[U55] PHP：match 表达式
来源：http://ni.colortex.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nu.jctech888.com.cn

[U56] PHP：命名参数
来源：http://rr.szsharing.cn

f(a: 1, b: 2)
来源：http://ht.yuntaijiaju.cn

[U57] PHP：字符串插值
来源：http://by.nicolike.cn

"值: {$a}"
来源：http://pf.nicolike.cn

[U58] PHP：数组三件套
来源：http://df.hahajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://km.nszjky.cn

[U59] PHP：自定义排序
来源：http://vj.panjiajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ju.shxzukj.cn

[U60] PHP：JSON 编解码
来源：http://ka.bjjhwx.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://of.huixiangedu.cn

[U61] PHP：正则
来源：http://os.wgjwhj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gu.colortex.cn

[U62] PHP：日期对象
来源：http://ez.bjjhwx.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vz.newstarts.cn

[U63] PHP：文件读写
来源：http://hd.yuexingan06.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ip.newstarts.cn

[U64] PHP：目录遍历
来源：http://hi.colortex.cn

glob("dir/*.php");  scandir("dir");
来源：http://uh.bjjhwx.cn

[U65] PHP：会话
来源：http://qf.wgjwhj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ff.bjjhwx.cn

[U66] PHP：设置 Cookie
来源：http://do.chemitech.net.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sn.huixiangedu.cn

[U67] PHP：处理文件上传
来源：http://yo.hnjuh.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cf.gzmigu.cn

[U68] PHP：PDO 连接
来源：http://kw.bookmarksfly.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ct.nicolike.cn

[U69] PHP：PDO 预处理
来源：http://ir.jctech888.com.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ll.hnjuh.cn

[U70] PHP：PDO 事务
来源：http://ng.yuntaijiaju.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bo.yuntaijiaju.cn

[U71] PHP：抛出异常
来源：http://vu.lnxyls.cn

throw new RuntimeException("失败", 500);
来源：http://xs.huixinmuqiang.cn

[U72] PHP：写错误日志
来源：http://jd.shtwfgs.cn

error_log("失败: " . $e->getMessage());
来源：http://vs.yuntaijiaju.cn

[U73] PHP：读取 ini 配置
来源：http://at.colortex.cn

parse_ini_file("config.ini", true)
来源：http://lc.yuntaijiaju.cn

[U74] PHP：读取环境变量
来源：http://cz.panjiajie.cn

getenv("APP_ENV") ?: "production"
来源：http://lq.jianghongdianzi.cn

[U75] PHP：依赖注入
来源：http://np.shtwfgs.cn

composer require psr/container
来源：http://fb.shxzukj.cn

[U76] PHP：简单路由
来源：http://pd.yuexingan06.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pq.newstarts.cn

[U77] PHP：模板渲染
来源：http://rp.shxzukj.cn

composer require twig/twig
来源：http://ge.yuexingan06.cn

[U78] PHP：单元测试
来源：http://kf.haigaiapp.cn

composer require --dev phpunit/phpunit
来源：http://oi.shxzukj.cn

[U79] PHP：静态分析
来源：http://wv.hnjuh.cn

composer require --dev phpstan/phpstan
来源：http://hs.521024.cn

[U80] PHP：代码规范修复
来源：http://ue.szxytkj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ys.szsharing.cn

[U81] JS：初始化项目
来源：http://gh.newstarts.cn

npm init -y;  npm i express
来源：http://jn.521024.cn

[U82] JS：package.json 脚本
来源：http://iq.newstarts.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wo.shxzukj.cn

[U83] JS：ES Module 导入导出
来源：http://oz.shtwfgs.cn

export const a = 1;  import { a } from "./m.js";
来源：http://jh.shxzskj.cn

[U84] JS：CommonJS 写法
来源：http://kl.huixiangedu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://lf.huixinmuqiang.cn

[U85] JS：可选链
来源：http://ul.huixiangedu.cn

a?.b?.c
来源：http://bh.nicolike.cn

[U86] JS：空值合并
来源：http://nj.huixiangedu.cn

a ?? b
来源：http://pc.shtwfgs.cn

[U87] JS：解构默认值
来源：http://uo.muxihuayi.cn

const { a = 1, b = 2 } = obj;
来源：http://wn.panjiajie.cn

[U88] JS：对象展开合并
来源：http://je.521024.cn

{ ...a, ...b }
来源：http://rb.panjiajie.cn

[U89] JS：数组去重
来源：http://lf.nszjky.cn

[...new Set(arr)]
来源：http://xh.panjiajie.cn

[U90] JS：数字数组排序
来源：http://xm.jianghongdianzi.cn

[...arr].sort((a, b) => a - b)
来源：http://sk.asd995.cn

[U91] JS：对象键值遍历
来源：http://lw.521024.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://op.haigaiapp.cn

[U92] JS：深拷贝
来源：http://ov.jianghongdianzi.cn

structuredClone(obj)
来源：http://sh.huixiangedu.cn

[U93] JS：模板字符串
来源：http://yl.lnxyls.cn

`共 ${n} 条`
来源：http://ba.panjiajie.cn

[U94] JS：箭头函数
来源：http://aj.chemitech.net.cn

const double = x => x * 2;
来源：http://zs.haigaiapp.cn

[U95] JS：Promise 包装
来源：http://ja.nicolike.cn

new Promise((resolve, reject) => {})
来源：http://vj.szsharing.cn

[U96] JS：async/await 与异常
来源：http://pa.yuexingan06.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ok.yuntaijiaju.cn

[U97] JS：并发请求
来源：http://qf.lnxyls.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://pk.nicolike.cn

[U98] JS：fetch 带 JSON
来源：http://yl.huanxung.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://at.szxytkj.cn

[U99] JS：事件监听
来源：http://ff.muxihuayi.cn

el.addEventListener("click", e => {})
来源：http://nc.9csxet.cn

[U100] JS：DOM 查询
来源：http://hf.jianghongdianzi.cn

document.querySelector(".item")
来源：http://gx.shxzskj.cn

[U101] JS：classList 操作
来源：http://dw.szxytkj.cn

el.classList.toggle("active")
来源：http://rz.yuntaijiaju.cn

[U102] JS：本地存储
来源：http://dy.newstarts.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://vh.newstarts.cn

[U103] JS：定时器
来源：http://ir.huixinmuqiang.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hu.szsharing.cn

[U104] JS：防抖
来源：http://jd.newstarts.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mz.nicolike.cn

[U105] JS：节流
来源：http://ba.chemitech.net.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xb.muxihuayi.cn

[U106] JS：日期格式化
来源：http://cs.jianghongdianzi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lx.lnxyls.cn

[U107] JS：数字千分位
来源：http://qu.huixinmuqiang.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sg.lnxyls.cn

[U108] JS：随机整数
来源：http://vx.lnxyls.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nv.bjjhwx.cn

[U109] JS：数组分组
来源：http://xk.yuexingan06.cn

Object.groupBy(arr, x => x.type)
来源：http://kt.bjjhwx.cn

[U110] JS：数组分块
来源：http://qb.huixiangedu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ny.huanxung.cn

[U111] JS：对象转 Map
来源：http://jd.haigaiapp.cn

new Map(Object.entries(obj))
来源：http://dr.521024.cn

[U112] JS：字符串补位
来源：http://qx.lnxyls.cn

"7".padStart(3, "0")
来源：http://hb.panjiajie.cn

[U113] JS：正则替换全部
来源：http://ah.jctech888.com.cn

s.replaceAll("a", "b")
来源：http://vn.wgjwhj.cn

[U114] JS：JSON 深比较
来源：http://it.jctech888.com.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://er.lnxyls.cn

[U115] JS：生成 UUID
来源：http://jk.bookmarksfly.cn

crypto.randomUUID()
来源：http://wx.muxihuayi.cn

[U116] JS：类型检查（JSDoc）
来源：http://gr.panjiajie.cn

/** @param {string} name */ function f(name) {}
来源：http://me.nszjky.cn

[U117] JS：单元测试
来源：http://yj.huixiangedu.cn

npm i -D vitest;  npx vitest
来源：http://hk.szsharing.cn

[U118] JS：开发服务器
来源：http://dw.szsharing.cn

npm i -D vite;  npx vite
来源：http://ju.shxzskj.cn

[U119] JS：生产构建
来源：http://vr.shtwfgs.cn

npx vite build
来源：http://xk.lnxyls.cn

[U120] JS：读取环境变量（Vite）
来源：http://zz.hahajie.cn

import.meta.env.VITE_API_URL
来源：http://ep.haigaiapp.cn

================================================================================
来源：http://gh.bookmarksfly.cn

统计汇总
来源：http://lj.bjjhwx.cn

================================================================================
来源：http://jn.9csxet.cn

按语言统计（条）：
来源：http://lk.szxytkj.cn

Python ......... 252
来源：http://pt.lnxyls.cn

PHP ............ 252
来源：http://sr.shtwfgs.cn

JavaScript ..... 252
来源：http://zm.hahajie.cn

TypeScript ..... 212
来源：http://sm.chemitech.net.cn

Java ........... 212
来源：http://yq.asd995.cn

Go ............. 212
来源：http://fv.9csxet.cn

Ruby ........... 212
来源：http://za.jctech888.com.cn

C# ............. 212
来源：http://us.jianghongdianzi.cn

C .............. 30
来源：http://nx.nszjky.cn

C++ ............ 30
来源：http://yn.huanxung.cn

SQL ............ 90
来源：http://jb.nszjky.cn

Bash ........... 80
来源：http://bk.panjiajie.cn

Kotlin ......... 15
来源：http://dv.yuntaijiaju.cn

Swift .......... 15
来源：http://bt.chemitech.net.cn

Lua ............ 10
来源：http://pv.nicolike.cn

Perl ........... 10
来源：http://vm.hahajie.cn

Scala .......... 10
来源：http://pj.521024.cn

------------------------------------
来源：http://ee.szxytkj.cn

合计 ........... 2106 条
来源：http://tq.panjiajie.cn

按章节统计：
来源：http://am.shxzukj.cn


<!-- 参考信息 -->