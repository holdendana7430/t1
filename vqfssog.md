代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://baike.fanxiaobao.xyz/Article/details/gfzfaggbq.sHtML

@contextlib.contextmanager
来源：http://read.share.fanxiaobao.xyz/Article/details/gffwapqxl.sHtML

[U22] Py：矩阵转置
来源：http://baike.fanxiaobao.xyz/Article/details/gxhchikes.sHtML

list(zip(*m))
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnknvovs.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxyotxli.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblfkghsb.sHtML

[U24] Py：路径操作
来源：http://baike.fanxiaobao.xyz/Article/details/gytzpimgz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsxuszpz.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fanxiaobao.xyz/Article/details/gqharofnz.sHtML

csv.DictReader(f)
来源：http://baike.fanxiaobao.xyz/Article/details/gazesmeuj.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwuttdki.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdagiskt.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgqdmqpq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fanxiaobao.xyz/Article/details/guktayrfa.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/gvgvzourd.sHtML

UserId = int
来源：http://wap.fanxiaobao.xyz/Article/details/gybxjdifp.sHtML

[U29] Py：属性校验
来源：http://3g.fanxiaobao.xyz/Article/details/gqafsjwnt.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fanxiaobao.xyz/Article/details/glwkwoski.sHtML

[U30] Py：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gtuldvzkn.sHtML

@dataclass(slots=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbnwcqhq.sHtML

[U31] Py：单测
来源：http://read.share.fanxiaobao.xyz/Article/details/gbamtuifu.sHtML

python -m pytest -q
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggscykqib.sHtML

[U32] Py：代码格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gamshebjc.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fanxiaobao.xyz/Article/details/gkezysrzt.sHtML

[U33] Py：打包发布
来源：http://wap.fanxiaobao.xyz/Article/details/giggqhszd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fanxiaobao.xyz/Article/details/gpvcfgnvw.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuvpspkx.sHtML

chardet.detect(raw)
来源：http://www.share.fanxiaobao.xyz/Article/details/gptigoard.sHtML

[U35] Py：发送邮件
来源：http://blog.fanxiaobao.xyz/Article/details/guhinikok.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzhnwjjl.sHtML

[U36] Py：定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gfknowtdg.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplrqnpgp.sHtML

[U37] Py：读写 Excel
来源：http://3g.fanxiaobao.xyz/Article/details/ganoefmqc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fanxiaobao.xyz/Article/details/gxamsgdhw.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxgscyoy.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyagysyps.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gjyegkdry.sHtML

sys.stdout.isatty()
来源：http://m.share.fanxiaobao.xyz/Article/details/gghyrxlhy.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gathjcjqh.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtniahne.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwjbqwdp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fanxiaobao.xyz/Article/details/gziugokui.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fanxiaobao.xyz/Article/details/gxqrttokr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqsyqckg.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbpatcbv.sHtML

namespace App\Http;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpspsxji.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyxbsfdi.sHtML

declare(strict_types=1);
来源：http://wap.fanxiaobao.xyz/Article/details/gkhmnlnsn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fanxiaobao.xyz/Article/details/gtzpjqzul.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmffaacry.sHtML

[U46] PHP：可空类型
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxzgqzrm.sHtML

?string $name = null
来源：http://wap.fanxiaobao.xyz/Article/details/gqtzkajfd.sHtML

[U47] PHP：联合类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gghijtuvb.sHtML

int|string $id
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjnropqu.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gofraixzu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvfuzjvr.sHtML

[U49] PHP：只读属性
来源：http://wap.fanxiaobao.xyz/Article/details/guknidsdd.sHtML

public readonly string $name
来源：http://baike.fanxiaobao.xyz/Article/details/gnuwqxrce.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbygzonm.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgxpgheh.sHtML

[U51] PHP：数组解构
来源：http://3g.fanxiaobao.xyz/Article/details/ghjningxl.sHtML

[$a, $b] = $arr;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxvaysrj.sHtML

[U52] PHP：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/gbmnxasat.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/gucikqvwx.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaytiplue.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmwktwln.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjiwwjhg.sHtML

$obj?->method()
来源：http://3g.fanxiaobao.xyz/Article/details/gtfpqkqty.sHtML

[U55] PHP：match 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gohdtsmmy.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmdrsblv.sHtML

[U56] PHP：命名参数
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwxnobtg.sHtML

f(a: 1, b: 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gncunfbgb.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtyyozry.sHtML

"值: {$a}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcjppejo.sHtML

[U58] PHP：数组三件套
来源：http://wap.fanxiaobao.xyz/Article/details/gevupezzn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gngvlauea.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjavbuyt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcncekiez.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fanxiaobao.xyz/Article/details/gdohhnsab.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcvqavgv.sHtML

[U61] PHP：正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmswthjtw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzsfjphou.sHtML

[U62] PHP：日期对象
来源：http://blog.fanxiaobao.xyz/Article/details/gacbtfmbe.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvhhjgkj.sHtML

[U63] PHP：文件读写
来源：http://mobile.fanxiaobao.xyz/Article/details/ggayljeyd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvxtoice.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbnprpoq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fanxiaobao.xyz/Article/details/gnssjuxey.sHtML

[U65] PHP：会话
来源：http://mobile.fanxiaobao.xyz/Article/details/gffrkbbkb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqthorust.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjfosdrl.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gjsmyvsdv.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxgbeomw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcaavargn.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gosopzrrg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fanxiaobao.xyz/Article/details/gwvdpypkq.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fanxiaobao.xyz/Article/details/ganjuzmuk.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fanxiaobao.xyz/Article/details/gbgtsronf.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gryroojcq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdcewgvn.sHtML

[U71] PHP：抛出异常
来源：http://blog.fanxiaobao.xyz/Article/details/gdlmyblia.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fanxiaobao.xyz/Article/details/gebirwcxw.sHtML

[U72] PHP：写错误日志
来源：http://baike.fanxiaobao.xyz/Article/details/gzimwazdf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fanxiaobao.xyz/Article/details/gkmdpbwze.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fanxiaobao.xyz/Article/details/gxdjtgagv.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnxazbxt.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gzuxmitgj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fanxiaobao.xyz/Article/details/gtzgiyaha.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fanxiaobao.xyz/Article/details/geibzuyos.sHtML

composer require psr/container
来源：http://blog.fanxiaobao.xyz/Article/details/ginmwpwlh.sHtML

[U76] PHP：简单路由
来源：http://wap.fanxiaobao.xyz/Article/details/ggjwgfcfi.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpccspfew.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fanxiaobao.xyz/Article/details/grbbwugxr.sHtML

composer require twig/twig
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvzcjtgg.sHtML

[U78] PHP：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/gffkdrcxj.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikrvgmdo.sHtML

[U79] PHP：静态分析
来源：http://baike.fanxiaobao.xyz/Article/details/gkpofmaol.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fanxiaobao.xyz/Article/details/gwbknetfw.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fanxiaobao.xyz/Article/details/gjapqwcbh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahyfuufm.sHtML

[U81] JS：初始化项目
来源：http://mobile.fanxiaobao.xyz/Article/details/gaagupgub.sHtML

npm init -y;  npm i express
来源：http://mobile.fanxiaobao.xyz/Article/details/geyrgtrti.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgrkcmuo.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvbkwrso.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fanxiaobao.xyz/Article/details/gxyrgrrjd.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fanxiaobao.xyz/Article/details/gydoplmcm.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fanxiaobao.xyz/Article/details/gswvxdxye.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fanxiaobao.xyz/Article/details/gvlbwmpod.sHtML

[U85] JS：可选链
来源：http://baike.fanxiaobao.xyz/Article/details/gvivjofoe.sHtML

a?.b?.c
来源：http://wap.fanxiaobao.xyz/Article/details/gsazjjppy.sHtML

[U86] JS：空值合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gcebxxhrb.sHtML

a ?? b
来源：http://wap.fanxiaobao.xyz/Article/details/gushnxolc.sHtML

[U87] JS：解构默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gayzyuvte.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fanxiaobao.xyz/Article/details/gwvplgpjp.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsypodmm.sHtML

{ ...a, ...b }
来源：http://wap.fanxiaobao.xyz/Article/details/garsuhkuz.sHtML

[U89] JS：数组去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gcuzqkstu.sHtML

[...new Set(arr)]
来源：http://3g.fanxiaobao.xyz/Article/details/gxickfxee.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqtwclhc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fanxiaobao.xyz/Article/details/ghakwzfea.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gxauhedgo.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fanxiaobao.xyz/Article/details/gomfondtt.sHtML

[U92] JS：深拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gnuhqvbco.sHtML

structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbhjocgq.sHtML

[U93] JS：模板字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gyydpzkez.sHtML

`共 ${n} 条`
来源：http://read.share.fanxiaobao.xyz/Article/details/ggddppygf.sHtML

[U94] JS：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/grtqjkbge.sHtML

const double = x => x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/gybcrhwdz.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsmwkpac.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fanxiaobao.xyz/Article/details/gypnoxckb.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokykgads.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/gdfnpcjsk.sHtML

[U97] JS：并发请求
来源：http://read.share.fanxiaobao.xyz/Article/details/gkotzbjrr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fanxiaobao.xyz/Article/details/gfhgzneif.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmfhbynf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fanxiaobao.xyz/Article/details/glbmfrajy.sHtML

[U99] JS：事件监听
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcwccdtx.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhcezykt.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glljfmynb.sHtML

document.querySelector(".item")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjqoghej.sHtML

[U101] JS：classList 操作
来源：http://3g.fanxiaobao.xyz/Article/details/gnvliurbc.sHtML

el.classList.toggle("active")
来源：http://blog.fanxiaobao.xyz/Article/details/gdtwbpruu.sHtML

[U102] JS：本地存储
来源：http://read.share.fanxiaobao.xyz/Article/details/gazeoevmk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fanxiaobao.xyz/Article/details/gtffghrzu.sHtML

[U103] JS：定时器
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvqozzqf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjemocisd.sHtML

[U104] JS：防抖
来源：http://mobile.fanxiaobao.xyz/Article/details/gcksvgbfk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/guejbprzc.sHtML

[U105] JS：节流
来源：http://mobile.fanxiaobao.xyz/Article/details/gcuyrdjep.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gdxnzmqiy.sHtML

[U106] JS：日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtmmxoze.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fanxiaobao.xyz/Article/details/grdwjxsuy.sHtML

[U107] JS：数字千分位
来源：http://wap.fanxiaobao.xyz/Article/details/ghittxgdi.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwavcbai.sHtML

[U108] JS：随机整数
来源：http://3g.fanxiaobao.xyz/Article/details/gnsnbgrot.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fanxiaobao.xyz/Article/details/gftqugjtr.sHtML

[U109] JS：数组分组
来源：http://3g.fanxiaobao.xyz/Article/details/gjxuezyls.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzfokpax.sHtML

[U110] JS：数组分块
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjnwevjw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fanxiaobao.xyz/Article/details/gviorpury.sHtML

[U111] JS：对象转 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gknvmsejq.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjwyvpha.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzibitubx.sHtML

"7".padStart(3, "0")
来源：http://wap.fanxiaobao.xyz/Article/details/gzgvlphjh.sHtML

[U113] JS：正则替换全部
来源：http://wap.fanxiaobao.xyz/Article/details/gqqhbdzsl.sHtML

s.replaceAll("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gntzeacap.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwtxiwil.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggminxoxc.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnsiircd.sHtML

crypto.randomUUID()
来源：http://blog.fanxiaobao.xyz/Article/details/gcwtyndov.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmrxbnet.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspgqazkz.sHtML

[U117] JS：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/gvuwiwxel.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fanxiaobao.xyz/Article/details/gwukplyob.sHtML

[U118] JS：开发服务器
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyytrfie.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxokrohl.sHtML

[U119] JS：生产构建
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkmkylzp.sHtML

npx vite build
来源：http://baike.fanxiaobao.xyz/Article/details/gyceebrpz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fanxiaobao.xyz/Article/details/gkavxfbyg.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fanxiaobao.xyz/Article/details/gdpoyhone.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfnhumrz.sHtML

统计汇总
来源：http://baike.fanxiaobao.xyz/Article/details/gqsdaikzg.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqltfuap.sHtML

按语言统计（条）：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwpsskpq.sHtML

Python ......... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmlbpmsv.sHtML

PHP ............ 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtifgkrxx.sHtML

JavaScript ..... 252
来源：http://baike.fanxiaobao.xyz/Article/details/gdesdgtsy.sHtML

TypeScript ..... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvfahtdm.sHtML

Java ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdweybin.sHtML

Go ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/gusnifooy.sHtML

Ruby ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gdfodmtry.sHtML

C# ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guettslto.sHtML

C .............. 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofgskjgl.sHtML

C++ ............ 30
来源：http://mobile.fanxiaobao.xyz/Article/details/giijlcwos.sHtML

SQL ............ 90
来源：http://3g.fanxiaobao.xyz/Article/details/gsyzvpwam.sHtML

Bash ........... 80
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqvoggzr.sHtML

Kotlin ......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/grzwfnqkr.sHtML

Swift .......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gdvqahgaj.sHtML

Lua ............ 10
来源：http://baike.fanxiaobao.xyz/Article/details/gpleuxear.sHtML

Perl ........... 10
来源：http://wap.fanxiaobao.xyz/Article/details/goairxavt.sHtML

Scala .......... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmevgrpm.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/giqdqfnfp.sHtML

合计 ........... 2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gyphjhrhv.sHtML

按章节统计：
来源：http://blog.fanxiaobao.xyz/Article/details/gsjqzneck.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzomnecxx.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gipwnyodx.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gtxffdtoy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtghwols.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fanxiaobao.xyz/Article/details/gfyaztfvx.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzjjfdkr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/glqjmtpuq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyqyzwdv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/guqgtvnqs.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fanxiaobao.xyz/Article/details/glsysrxlr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gukqvuiuc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gspzjvxlw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwbbsrps.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbayupaa.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fanxiaobao.xyz/Article/details/gshtgvpxt.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gbofjzgug.sHtML

Q SQL 专题                              90
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrrvbard.sHtML

R Bash 专题                             80
来源：http://blog.fanxiaobao.xyz/Article/details/gwpshbebv.sHtML

S C / C++ 专题                          60
来源：http://3g.fanxiaobao.xyz/Article/details/gzzpftiqm.sHtML

T 其他语言补充                          60
来源：http://mobile.fanxiaobao.xyz/Article/details/gddxhiqxo.sHtML

U 高频实用片段                         120
来源：http://m.share.fanxiaobao.xyz/Article/details/gczwfahpi.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gerutyvcp.sHtML

合计                                  2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gnudlqszb.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gqiwwubyk.sHtML

使用提醒
来源：http://read.share.fanxiaobao.xyz/Article/details/gejnazhls.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gprnyaslp.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fanxiaobao.xyz/Article/details/gffjvnjyy.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmpcrkul.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fanxiaobao.xyz/Article/details/gprcexstd.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fanxiaobao.xyz/Article/details/gzaeyaose.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.fanxiaobao.xyz/Article/details/gxiuovhnb.sHtML

—— 文件结束 ——
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehislesa.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gyipytoha.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fanxiaobao.xyz/Article/details/gluyjiqpt.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqnrodpp.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycyjofyg.sHtML

【收录内容】
来源：http://wap.fanxiaobao.xyz/Article/details/gplkyashz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyejoqix.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqqjdzmq.sHtML

SQL · Bash · C · C++
来源：http://www.share.fanxiaobao.xyz/Article/details/gaytlobiv.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtwtwxbu.sHtML

【使用说明】
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgpuithd.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.fanxiaobao.xyz/Article/details/gqyjmvnpw.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.fanxiaobao.xyz/Article/details/ggunqsuta.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyuptntt.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnynvxax.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fanxiaobao.xyz/Article/details/gdysyqtod.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fanxiaobao.xyz/Article/details/gdmmylymw.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.fanxiaobao.xyz/Article/details/gozdhwfxf.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fanxiaobao.xyz/Article/details/gdptjxwbo.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.fanxiaobao.xyz/Article/details/gzlzxlogk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjikxkde.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fanxiaobao.xyz/Article/details/gcufmlutw.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.fanxiaobao.xyz/Article/details/glopgzaai.sHtML

【文件统计】
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzqeiinj.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.fanxiaobao.xyz/Article/details/gycbpkdrp.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmavzrkhg.sHtML

目  录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezuxzagi.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/grxeaftuv.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gvfzqyuyc.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.fanxiaobao.xyz/Article/details/grmwjnaso.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsuvrixva.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gtcwzzlzr.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gzghcdnoa.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gycbxhpxm.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.fanxiaobao.xyz/Article/details/glmiugivj.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gllqvnqat.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gpmrqcimx.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcygumlcu.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrcftfeo.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqglwvzuo.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gpgonvxgm.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.fanxiaobao.xyz/Article/details/ghfwefiel.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gylxmqwxy.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gzpxhfhol.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjebxijf.sHtML


<!-- 参考信息 -->