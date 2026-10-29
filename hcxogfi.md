代发 wailian999

[U17] Py：初始化日志
来源：http://baike.fehbvm.com/Article/details/gyeucednq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/gnjbmyydc.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.zdbjq.cn/Article/details/gasuhgxno.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fehbvm.com/Article/details/gycjjitfm.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.hesvh.cn/Article/details/gerquqxlg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fehbvm.com/Article/details/gnlvrhqpg.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.hesvh.cn/Article/details/geteefmgc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fehbvm.com/Article/details/gcktgsbkv.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fehbvm.com/Article/details/gwebxdkvf.sHtML

@contextlib.contextmanager
来源：http://m.share.hesvh.cn/Article/details/gzpnpqnfd.sHtML

[U22] Py：矩阵转置
来源：http://m.share.hesvh.cn/Article/details/gidnfmfvv.sHtML

list(zip(*m))
来源：http://www.share.fehbvm.com/Article/details/ghajvrsrk.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.zdbjq.cn/Article/details/gijxsogeu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fehbvm.com/Article/details/gnwhhheks.sHtML

[U24] Py：路径操作
来源：http://m.share.fehbvm.com/Article/details/gxgzohkxt.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gtfrvrpib.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.zdbjq.cn/Article/details/gtcoutyul.sHtML

csv.DictReader(f)
来源：http://mobile.hesvh.cn/Article/details/gedjcinat.sHtML

[U26] Py：并发下载
来源：http://read.share.zdbjq.cn/Article/details/guxdjurlq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fehbvm.com/Article/details/gqpihqaad.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.hesvh.cn/Article/details/gncnuagcc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fehbvm.com/Article/details/gtqiygzol.sHtML

[U28] Py：类型别名
来源：http://wap.fehbvm.com/Article/details/gpfiohyqe.sHtML

UserId = int
来源：http://mobile.fehbvm.com/Article/details/gxejnkabq.sHtML

[U29] Py：属性校验
来源：http://baike.zdbjq.cn/Article/details/ggskscxpn.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.hesvh.cn/Article/details/gohjnoifh.sHtML

[U30] Py：数据类
来源：http://www.blog.fehbvm.com/Article/details/gxficwkye.sHtML

@dataclass(slots=True)
来源：http://mobile.zdbjq.cn/Article/details/geooujnmm.sHtML

[U31] Py：单测
来源：http://read.share.zdbjq.cn/Article/details/gzcbeuqcd.sHtML

python -m pytest -q
来源：http://blog.zdbjq.cn/Article/details/gdwwmmuzp.sHtML

[U32] Py：代码格式化
来源：http://www.blog.zdbjq.cn/Article/details/gllyyhrbl.sHtML

ruff format . && ruff check --fix .
来源：http://blog.zdbjq.cn/Article/details/gwfaqumor.sHtML

[U33] Py：打包发布
来源：http://3g.hesvh.cn/Article/details/gezvqycgb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.zdbjq.cn/Article/details/gqqlokmvc.sHtML

[U34] Py：判断编码
来源：http://www.m.share.hesvh.cn/Article/details/gkiozylth.sHtML

chardet.detect(raw)
来源：http://www.blog.zdbjq.cn/Article/details/gickhcyuo.sHtML

[U35] Py：发送邮件
来源：http://mobile.fehbvm.com/Article/details/gfdzciybf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fehbvm.com/Article/details/gbabfyvup.sHtML

[U36] Py：定时任务
来源：http://m.share.fehbvm.com/Article/details/ganlvepzn.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fehbvm.com/Article/details/gvsrekabl.sHtML

[U37] Py：读写 Excel
来源：http://blog.fehbvm.com/Article/details/grmjuronw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fehbvm.com/Article/details/gdtuipsir.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fehbvm.com/Article/details/gzlwclbmb.sHtML

Path(__file__).resolve().parent
来源：http://baike.hesvh.cn/Article/details/gpqguycgv.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fehbvm.com/Article/details/gqyfqfwsm.sHtML

sys.stdout.isatty()
来源：http://www.blog.fehbvm.com/Article/details/gnmsitmbo.sHtML

[U40] Py：打印到标准错误
来源：http://baike.hesvh.cn/Article/details/gdjiepsca.sHtML

print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/govwrrsse.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.zdbjq.cn/Article/details/gwfixglbr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.zdbjq.cn/Article/details/ggiflzfou.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.hesvh.cn/Article/details/gndshhsdm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.zdbjq.cn/Article/details/gbjznptyy.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gkzvtmfsp.sHtML

namespace App\Http;
来源：http://www.share.hesvh.cn/Article/details/gdnixetzf.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.zdbjq.cn/Article/details/gmoaqacwq.sHtML

declare(strict_types=1);
来源：http://baike.fehbvm.com/Article/details/gtfjrxqcr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fehbvm.com/Article/details/gvxrhfbla.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/goxzkgxmu.sHtML

[U46] PHP：可空类型
来源：http://blog.hesvh.cn/Article/details/gqxlrummt.sHtML

?string $name = null
来源：http://www.m.share.zdbjq.cn/Article/details/gozxvherd.sHtML

[U47] PHP：联合类型
来源：http://blog.hesvh.cn/Article/details/gpkbdjbth.sHtML

int|string $id
来源：http://www.blog.zdbjq.cn/Article/details/gpxxumxyl.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fehbvm.com/Article/details/guzmndgch.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.zdbjq.cn/Article/details/gbuewjvxi.sHtML

[U49] PHP：只读属性
来源：http://read.share.fehbvm.com/Article/details/gylneydyn.sHtML

public readonly string $name
来源：http://m.share.fehbvm.com/Article/details/gkokfnnji.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/gqggceoav.sHtML

public function __construct(private int $id) {}
来源：http://www.share.zdbjq.cn/Article/details/ggpjmdxne.sHtML

[U51] PHP：数组解构
来源：http://read.share.zdbjq.cn/Article/details/glahtuuth.sHtML

[$a, $b] = $arr;
来源：http://read.share.hesvh.cn/Article/details/gwcrvnmmx.sHtML

[U52] PHP：箭头函数
来源：http://wap.hesvh.cn/Article/details/gpobqtycu.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fehbvm.com/Article/details/gysqfusex.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.hesvh.cn/Article/details/gjztvshti.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.zdbjq.cn/Article/details/gjpcibdwd.sHtML

[U54] PHP：空安全调用
来源：http://3g.fehbvm.com/Article/details/gvzxiuznp.sHtML

$obj?->method()
来源：http://3g.zdbjq.cn/Article/details/gomoqbyit.sHtML

[U55] PHP：match 表达式
来源：http://blog.fehbvm.com/Article/details/gotllchjm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fehbvm.com/Article/details/gwxjjcmlw.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/gsuhhggmq.sHtML

f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gutryddoh.sHtML

[U57] PHP：字符串插值
来源：http://baike.hesvh.cn/Article/details/guwzoedqz.sHtML

"值: {$a}"
来源：http://m.share.zdbjq.cn/Article/details/gejadcjcz.sHtML

[U58] PHP：数组三件套
来源：http://baike.zdbjq.cn/Article/details/ggskgeddi.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.hesvh.cn/Article/details/ghycxzcxp.sHtML

[U59] PHP：自定义排序
来源：http://wap.hesvh.cn/Article/details/gduchklgh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gtiixizmm.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.zdbjq.cn/Article/details/gzgvlrzgm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fehbvm.com/Article/details/giojldrri.sHtML

[U61] PHP：正则
来源：http://www.blog.zdbjq.cn/Article/details/gtqfkvuso.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gvyzfzami.sHtML

[U62] PHP：日期对象
来源：http://3g.hesvh.cn/Article/details/gkdiazauj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fehbvm.com/Article/details/gjlcwfdto.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fehbvm.com/Article/details/gsqibgdbc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.hesvh.cn/Article/details/gqznjgydc.sHtML

[U64] PHP：目录遍历
来源：http://read.share.zdbjq.cn/Article/details/gzzjzchgk.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fehbvm.com/Article/details/gijtlpybi.sHtML

[U65] PHP：会话
来源：http://www.share.fehbvm.com/Article/details/gpnvxebba.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gyjhraxtg.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.hesvh.cn/Article/details/gsueajisv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.hesvh.cn/Article/details/gzcbykvmm.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fehbvm.com/Article/details/gvrgklvxa.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.zdbjq.cn/Article/details/gagwbzvub.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.zdbjq.cn/Article/details/gjabrcjoy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fehbvm.com/Article/details/gzbypkscl.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.hesvh.cn/Article/details/gafevlyow.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.hesvh.cn/Article/details/gxlmhekzc.sHtML

[U70] PHP：PDO 事务
来源：http://3g.hesvh.cn/Article/details/gehsmpzpg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.zdbjq.cn/Article/details/gapkqjfbq.sHtML

[U71] PHP：抛出异常
来源：http://m.share.hesvh.cn/Article/details/gvewmxqhi.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.zdbjq.cn/Article/details/gpbqsppis.sHtML

[U72] PHP：写错误日志
来源：http://baike.zdbjq.cn/Article/details/gzbqrnhpw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.zdbjq.cn/Article/details/gwvetyzcf.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fehbvm.com/Article/details/grekpqhhr.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.zdbjq.cn/Article/details/goweebauh.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gdjrspmsk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.hesvh.cn/Article/details/glgoxutjb.sHtML

[U75] PHP：依赖注入
来源：http://baike.fehbvm.com/Article/details/gfhlbtlcf.sHtML

composer require psr/container
来源：http://mobile.zdbjq.cn/Article/details/gqwovkjjq.sHtML

[U76] PHP：简单路由
来源：http://baike.zdbjq.cn/Article/details/gtfnzhlqo.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.hesvh.cn/Article/details/gfqgluyec.sHtML

[U77] PHP：模板渲染
来源：http://wap.hesvh.cn/Article/details/ggnbtjmxq.sHtML

composer require twig/twig
来源：http://baike.fehbvm.com/Article/details/gmvbexwpw.sHtML

[U78] PHP：单元测试
来源：http://read.share.hesvh.cn/Article/details/gdgftkonp.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fehbvm.com/Article/details/gxbgxming.sHtML

[U79] PHP：静态分析
来源：http://3g.zdbjq.cn/Article/details/gnzeuaeep.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.hesvh.cn/Article/details/giqhepxci.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fehbvm.com/Article/details/gyqveoint.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.hesvh.cn/Article/details/gghaumsbv.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.zdbjq.cn/Article/details/ggkynagub.sHtML

npm init -y;  npm i express
来源：http://m.share.zdbjq.cn/Article/details/grxzoqwrs.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.zdbjq.cn/Article/details/giqnkjlqf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fehbvm.com/Article/details/ggxrlqwrt.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.zdbjq.cn/Article/details/gqwifqpfq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/guebjmkdi.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.zdbjq.cn/Article/details/gylbocnkr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.hesvh.cn/Article/details/ghjqeqzlm.sHtML

[U85] JS：可选链
来源：http://wap.hesvh.cn/Article/details/gxjgpmvsa.sHtML

a?.b?.c
来源：http://read.share.fehbvm.com/Article/details/gvxfuubpb.sHtML

[U86] JS：空值合并
来源：http://baike.zdbjq.cn/Article/details/guxzqlzaa.sHtML

a ?? b
来源：http://blog.zdbjq.cn/Article/details/gbeiuokta.sHtML

[U87] JS：解构默认值
来源：http://read.share.zdbjq.cn/Article/details/gikhslcaq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fehbvm.com/Article/details/gtvkaqwvw.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.zdbjq.cn/Article/details/gzkolzyoh.sHtML

{ ...a, ...b }
来源：http://m.share.hesvh.cn/Article/details/gyoxukkoh.sHtML

[U89] JS：数组去重
来源：http://read.share.zdbjq.cn/Article/details/gaqsmztdf.sHtML

[...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gzhpflyfr.sHtML

[U90] JS：数字数组排序
来源：http://m.share.hesvh.cn/Article/details/gyleccxuo.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gqlpbylff.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.zdbjq.cn/Article/details/gpzclhxun.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.zdbjq.cn/Article/details/gnbvsomaj.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gjygfbaoc.sHtML

structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gqqbgcect.sHtML

[U93] JS：模板字符串
来源：http://mobile.zdbjq.cn/Article/details/grtnunbpe.sHtML

`共 ${n} 条`
来源：http://www.blog.zdbjq.cn/Article/details/gqbrgzron.sHtML

[U94] JS：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gdkqbrane.sHtML

const double = x => x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gftusptmb.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.zdbjq.cn/Article/details/gsrnxyjwj.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fehbvm.com/Article/details/gvyitpzro.sHtML

[U96] JS：async/await 与异常
来源：http://wap.zdbjq.cn/Article/details/gtqffotxe.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gxkrunybz.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/gloekjxvn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/guzcyqyxn.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.hesvh.cn/Article/details/gurrbwcbw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.zdbjq.cn/Article/details/gbtlwnlfi.sHtML

[U99] JS：事件监听
来源：http://3g.zdbjq.cn/Article/details/glwjmemid.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fehbvm.com/Article/details/gtbekoxjr.sHtML

[U100] JS：DOM 查询
来源：http://3g.zdbjq.cn/Article/details/gjnoftflr.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/gjpagdleq.sHtML

[U101] JS：classList 操作
来源：http://mobile.zdbjq.cn/Article/details/gafnpanez.sHtML

el.classList.toggle("active")
来源：http://3g.zdbjq.cn/Article/details/gecftbjbp.sHtML

[U102] JS：本地存储
来源：http://www.share.zdbjq.cn/Article/details/gpwtybymt.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.hesvh.cn/Article/details/gyvssvetr.sHtML

[U103] JS：定时器
来源：http://mobile.zdbjq.cn/Article/details/gmvlhkggc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fehbvm.com/Article/details/goyqfiarb.sHtML

[U104] JS：防抖
来源：http://m.share.hesvh.cn/Article/details/gxrehxzgu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gnnhwlbbo.sHtML

[U105] JS：节流
来源：http://blog.hesvh.cn/Article/details/gsvyhkmsw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.hesvh.cn/Article/details/gkusttpku.sHtML

[U106] JS：日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gtnocjhzw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.hesvh.cn/Article/details/glwfptokk.sHtML

[U107] JS：数字千分位
来源：http://mobile.hesvh.cn/Article/details/gmpzuqvgb.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gmipluxno.sHtML

[U108] JS：随机整数
来源：http://m.share.hesvh.cn/Article/details/gajfdpldk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fehbvm.com/Article/details/ggbmytvtk.sHtML

[U109] JS：数组分组
来源：http://www.share.fehbvm.com/Article/details/guvwsbrxb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gakpjlbee.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/gvpyscvuv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.zdbjq.cn/Article/details/gqvkqroxj.sHtML

[U111] JS：对象转 Map
来源：http://baike.fehbvm.com/Article/details/geptsrhov.sHtML

new Map(Object.entries(obj))
来源：http://3g.hesvh.cn/Article/details/gonuqkrdf.sHtML

[U112] JS：字符串补位
来源：http://www.blog.hesvh.cn/Article/details/gurmavecf.sHtML

"7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gvhzsptcr.sHtML

[U113] JS：正则替换全部
来源：http://3g.fehbvm.com/Article/details/gcacdpode.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gmnpjalpm.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fehbvm.com/Article/details/gmxsppoom.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gvxtsrzsi.sHtML

[U115] JS：生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gaujinfut.sHtML

crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/garjzmmxm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.hesvh.cn/Article/details/gyfjmqmhu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.hesvh.cn/Article/details/gzebpsexc.sHtML

[U117] JS：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gxsvqvjgt.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.hesvh.cn/Article/details/gwmcsyewz.sHtML

[U118] JS：开发服务器
来源：http://www.blog.hesvh.cn/Article/details/gfqxiltbp.sHtML

npm i -D vite;  npx vite
来源：http://www.share.zdbjq.cn/Article/details/gbvsekxzo.sHtML

[U119] JS：生产构建
来源：http://blog.hesvh.cn/Article/details/gijwbgzgc.sHtML

npx vite build
来源：http://mobile.hesvh.cn/Article/details/gezpuurtp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.zdbjq.cn/Article/details/gdbregfvg.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.hesvh.cn/Article/details/gyijzuuuq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdrretltz.sHtML

统计汇总
来源：http://www.blog.hesvh.cn/Article/details/gkcudjmpk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvxfthdyn.sHtML

按语言统计（条）：
来源：http://www.blog.hesvh.cn/Article/details/guagujxhi.sHtML

Python ......... 252
来源：http://www.share.zdbjq.cn/Article/details/gziehontl.sHtML

PHP ............ 252
来源：http://baike.hesvh.cn/Article/details/gjqtvaiye.sHtML

JavaScript ..... 252
来源：http://3g.hesvh.cn/Article/details/gdxhzqwkh.sHtML

TypeScript ..... 212
来源：http://blog.zdbjq.cn/Article/details/gvfgmexlz.sHtML

Java ........... 212
来源：http://read.share.hesvh.cn/Article/details/gdsqjnpgw.sHtML

Go ............. 212
来源：http://baike.fehbvm.com/Article/details/gazpmgurp.sHtML

Ruby ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gkizwnxqg.sHtML

C# ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gvisaoyqn.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/glejmskuv.sHtML

C++ ............ 30
来源：http://wap.hesvh.cn/Article/details/gdwojqncf.sHtML

SQL ............ 90
来源：http://mobile.fehbvm.com/Article/details/gftrxllhe.sHtML

Bash ........... 80
来源：http://www.blog.fehbvm.com/Article/details/giraobobh.sHtML

Kotlin ......... 15
来源：http://baike.zdbjq.cn/Article/details/ghpsksfvu.sHtML

Swift .......... 15
来源：http://www.blog.hesvh.cn/Article/details/gueyhvudl.sHtML

Lua ............ 10
来源：http://www.share.fehbvm.com/Article/details/gpxdnqjmo.sHtML

Perl ........... 10
来源：http://baike.fehbvm.com/Article/details/gzktktict.sHtML

Scala .......... 10
来源：http://3g.fehbvm.com/Article/details/gpeowhnjw.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gseffgico.sHtML

合计 ........... 2106 条
来源：http://blog.hesvh.cn/Article/details/gesohgtss.sHtML

按章节统计：
来源：http://wap.hesvh.cn/Article/details/ggczxkpdn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gbnbtluvs.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gpbifzdcb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gknmvlodb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gbvaprmeg.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fehbvm.com/Article/details/gibkrqahc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/gmxxukntp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gmrkyqjwy.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gkyyhfgro.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gwittjcqo.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gaxbdqmrp.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gpgslrtzw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gwumwfmtu.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gioguolat.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gitdlxmsd.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.zdbjq.cn/Article/details/gosqzcrkn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/ghdvnatvb.sHtML

Q SQL 专题                              90
来源：http://mobile.fehbvm.com/Article/details/gjtouptyz.sHtML

R Bash 专题                             80
来源：http://baike.fehbvm.com/Article/details/gmwbmzmyw.sHtML

S C / C++ 专题                          60
来源：http://blog.zdbjq.cn/Article/details/ghgkrjzpf.sHtML

T 其他语言补充                          60
来源：http://www.share.zdbjq.cn/Article/details/gaqabusmn.sHtML

U 高频实用片段                         120
来源：http://m.share.hesvh.cn/Article/details/gfedzmkjm.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gzcsglizr.sHtML

合计                                  2106 条
来源：http://read.share.zdbjq.cn/Article/details/gpmbftodr.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gdijmwqwa.sHtML

使用提醒
来源：http://wap.zdbjq.cn/Article/details/gieuhisns.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gzuhwsjkb.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fehbvm.com/Article/details/gjgzgnrja.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.hesvh.cn/Article/details/gibpncenw.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.zdbjq.cn/Article/details/gnyryhpjj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fehbvm.com/Article/details/ghlkdvnyo.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.zdbjq.cn/Article/details/govoxzjew.sHtML

—— 文件结束 ——
来源：http://baike.hesvh.cn/Article/details/gxtmvcvac.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/guyhiuyom.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fehbvm.com/Article/details/gtldiwpys.sHtML

Common Programming Examples Cheat Book
来源：http://blog.hesvh.cn/Article/details/gknygfrar.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjwvqnyhl.sHtML

【收录内容】
来源：http://wap.hesvh.cn/Article/details/gzxzlgrsx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.zdbjq.cn/Article/details/gexvazjhq.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.zdbjq.cn/Article/details/gkerxihrs.sHtML

SQL · Bash · C · C++
来源：http://baike.zdbjq.cn/Article/details/gbsvollev.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fehbvm.com/Article/details/ggmwanixi.sHtML

【使用说明】
来源：http://read.share.fehbvm.com/Article/details/grvrcusym.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.fehbvm.com/Article/details/gnrhkprrg.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.zdbjq.cn/Article/details/gijdkwxbg.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.hesvh.cn/Article/details/gmbjonyat.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fehbvm.com/Article/details/gkweuqwhm.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.hesvh.cn/Article/details/gefsogjae.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.zdbjq.cn/Article/details/goquyrnwn.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.hesvh.cn/Article/details/gsolngmkn.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.hesvh.cn/Article/details/gubszjxsb.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.zdbjq.cn/Article/details/gocwuurzk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.fehbvm.com/Article/details/gnqsguhrr.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fehbvm.com/Article/details/gqabjgoqk.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.hesvh.cn/Article/details/glngqxarq.sHtML

【文件统计】
来源：http://read.share.fehbvm.com/Article/details/gkfxnuiti.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.hesvh.cn/Article/details/gcmvvsniq.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gselbiaij.sHtML

目  录
来源：http://wap.fehbvm.com/Article/details/gmlwgfxab.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gxvdmkoet.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.hesvh.cn/Article/details/gwoxlajvw.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gzgcvyjsg.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/gfjekgbjo.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/gdkxtlwrb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.hesvh.cn/Article/details/gvzygnxrz.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/gaczvugun.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gzyxibsrc.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/gqjwmeawt.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gfogofcpf.sHtML


<!-- 参考信息 -->