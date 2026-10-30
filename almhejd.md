代发 wailian999

[U19] Py：正则替换带回调
来源：http://blog.hesvh.cn/Article/details/gxgmrpmdj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.zdbjq.cn/Article/details/gkrepqpch.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.hesvh.cn/Article/details/guodivwki.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.hesvh.cn/Article/details/gntfklxil.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.hesvh.cn/Article/details/grkyoedsi.sHtML

@contextlib.contextmanager
来源：http://www.share.fehbvm.com/Article/details/ghsbveswd.sHtML

[U22] Py：矩阵转置
来源：http://wap.zdbjq.cn/Article/details/gbgntrwli.sHtML

list(zip(*m))
来源：http://read.share.zdbjq.cn/Article/details/goqixddqn.sHtML

[U23] Py：分块读取大文件
来源：http://wap.hesvh.cn/Article/details/glygswree.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/gnhpjpiun.sHtML

[U24] Py：路径操作
来源：http://3g.hesvh.cn/Article/details/gjoyecyeo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gvufvyjvl.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.zdbjq.cn/Article/details/grxinefwd.sHtML

csv.DictReader(f)
来源：http://wap.zdbjq.cn/Article/details/gieisaslr.sHtML

[U26] Py：并发下载
来源：http://wap.fehbvm.com/Article/details/gnrrtjeeg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.zdbjq.cn/Article/details/gszbtztzi.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/gibdjqdyg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.zdbjq.cn/Article/details/gfezihipi.sHtML

[U28] Py：类型别名
来源：http://blog.hesvh.cn/Article/details/gnqrkiaez.sHtML

UserId = int
来源：http://3g.zdbjq.cn/Article/details/gpgjzhbyu.sHtML

[U29] Py：属性校验
来源：http://www.m.share.zdbjq.cn/Article/details/gefrimime.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fehbvm.com/Article/details/gpfmpujgz.sHtML

[U30] Py：数据类
来源：http://baike.fehbvm.com/Article/details/gugknjajv.sHtML

@dataclass(slots=True)
来源：http://3g.hesvh.cn/Article/details/gwyerjayo.sHtML

[U31] Py：单测
来源：http://www.m.share.zdbjq.cn/Article/details/gvyikbbso.sHtML

python -m pytest -q
来源：http://baike.hesvh.cn/Article/details/ganruqkfn.sHtML

[U32] Py：代码格式化
来源：http://blog.zdbjq.cn/Article/details/gueeifaxf.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fehbvm.com/Article/details/gpncykkyn.sHtML

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/glypfiams.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.hesvh.cn/Article/details/gkugsrboj.sHtML

[U34] Py：判断编码
来源：http://wap.fehbvm.com/Article/details/grjrgythf.sHtML

chardet.detect(raw)
来源：http://baike.fehbvm.com/Article/details/gbvbmdepq.sHtML

[U35] Py：发送邮件
来源：http://m.share.fehbvm.com/Article/details/gbqplnwno.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fehbvm.com/Article/details/guhvlbujk.sHtML

[U36] Py：定时任务
来源：http://mobile.fehbvm.com/Article/details/gvcnonzgs.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.hesvh.cn/Article/details/gesnndvvf.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fehbvm.com/Article/details/ghqilntiy.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fehbvm.com/Article/details/gzsgjnmpq.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.hesvh.cn/Article/details/gehovknmd.sHtML

Path(__file__).resolve().parent
来源：http://read.share.hesvh.cn/Article/details/ggwltdygs.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.zdbjq.cn/Article/details/gulwhursd.sHtML

sys.stdout.isatty()
来源：http://www.blog.fehbvm.com/Article/details/gxiwaxmwk.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fehbvm.com/Article/details/gkwnikypq.sHtML

print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/gpwncrmdv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.hesvh.cn/Article/details/gcirrsoai.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.zdbjq.cn/Article/details/glnmiober.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fehbvm.com/Article/details/gzxkpwrgo.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.hesvh.cn/Article/details/gmvvzlfpe.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.zdbjq.cn/Article/details/geybprugj.sHtML

namespace App\Http;
来源：http://www.share.zdbjq.cn/Article/details/govnblinq.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fehbvm.com/Article/details/ghhzutxht.sHtML

declare(strict_types=1);
来源：http://baike.zdbjq.cn/Article/details/gfnkajxyh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.hesvh.cn/Article/details/gyacjnxdh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/glqzarxbl.sHtML

[U46] PHP：可空类型
来源：http://read.share.hesvh.cn/Article/details/gkedavvqm.sHtML

?string $name = null
来源：http://wap.zdbjq.cn/Article/details/gzldlcjef.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.hesvh.cn/Article/details/gjvzcjrkl.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/gtmjqonqb.sHtML

[U48] PHP：纯枚举
来源：http://read.share.zdbjq.cn/Article/details/ggqqwmfgb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.zdbjq.cn/Article/details/gtznykcde.sHtML

[U49] PHP：只读属性
来源：http://mobile.fehbvm.com/Article/details/gkzxbocfy.sHtML

public readonly string $name
来源：http://www.m.share.hesvh.cn/Article/details/gcmrkqtax.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.hesvh.cn/Article/details/gutgatafz.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.hesvh.cn/Article/details/gabcddepm.sHtML

[U51] PHP：数组解构
来源：http://m.share.zdbjq.cn/Article/details/gzyeqxotb.sHtML

[$a, $b] = $arr;
来源：http://www.share.fehbvm.com/Article/details/gsunriggb.sHtML

[U52] PHP：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gemxakafz.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gvoiriupa.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.hesvh.cn/Article/details/ggcxytibr.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fehbvm.com/Article/details/gzppmfdgc.sHtML

[U54] PHP：空安全调用
来源：http://mobile.zdbjq.cn/Article/details/gsmnmskiy.sHtML

$obj?->method()
来源：http://www.blog.fehbvm.com/Article/details/gtjyzfyct.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gmdqvwcdz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fehbvm.com/Article/details/gvdzmghok.sHtML

[U56] PHP：命名参数
来源：http://mobile.fehbvm.com/Article/details/gxykonlyt.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gecvrksyv.sHtML

[U57] PHP：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/glzwoxkjw.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/glrwtifto.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.hesvh.cn/Article/details/ggvyhupss.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.zdbjq.cn/Article/details/glgdpqpga.sHtML

[U59] PHP：自定义排序
来源：http://read.share.hesvh.cn/Article/details/golqqlipx.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/glrpoapyk.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.hesvh.cn/Article/details/gxtegvxvd.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fehbvm.com/Article/details/grdafkuey.sHtML

[U61] PHP：正则
来源：http://3g.hesvh.cn/Article/details/gcdqhbprq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gutngedjo.sHtML

[U62] PHP：日期对象
来源：http://blog.hesvh.cn/Article/details/gsgryhcpq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.zdbjq.cn/Article/details/gqiicvzry.sHtML

[U63] PHP：文件读写
来源：http://m.share.fehbvm.com/Article/details/gguxxsmyn.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.zdbjq.cn/Article/details/gjwcvsqjr.sHtML

[U64] PHP：目录遍历
来源：http://read.share.zdbjq.cn/Article/details/gjrxpgixu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.zdbjq.cn/Article/details/graqzdywu.sHtML

[U65] PHP：会话
来源：http://www.blog.zdbjq.cn/Article/details/gjtuidrxt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fehbvm.com/Article/details/gycrdkrmy.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.hesvh.cn/Article/details/gpyfnzlch.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.zdbjq.cn/Article/details/gjqdopjkm.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fehbvm.com/Article/details/gefomomqn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.hesvh.cn/Article/details/gwnyenyjc.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.zdbjq.cn/Article/details/gxvysqrrt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.zdbjq.cn/Article/details/gjcaeqjeg.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fehbvm.com/Article/details/gwdpisjzz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fehbvm.com/Article/details/gudgasrmg.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gbkhcaldg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fehbvm.com/Article/details/gzedjjyli.sHtML

[U71] PHP：抛出异常
来源：http://wap.zdbjq.cn/Article/details/gmmhqytnk.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.zdbjq.cn/Article/details/gtnvmtrrq.sHtML

[U72] PHP：写错误日志
来源：http://read.share.zdbjq.cn/Article/details/guqddghfg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.hesvh.cn/Article/details/glqprexuo.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fehbvm.com/Article/details/gwabpgttc.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.zdbjq.cn/Article/details/ghoxmezva.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gmcldtcjn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fehbvm.com/Article/details/ggazqvjbm.sHtML

[U75] PHP：依赖注入
来源：http://baike.hesvh.cn/Article/details/gwxondzbr.sHtML

composer require psr/container
来源：http://m.share.zdbjq.cn/Article/details/ggvjwltnl.sHtML

[U76] PHP：简单路由
来源：http://3g.hesvh.cn/Article/details/gfgsfmtwi.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.zdbjq.cn/Article/details/gtkxwujqs.sHtML

[U77] PHP：模板渲染
来源：http://m.share.zdbjq.cn/Article/details/giekpuskq.sHtML

composer require twig/twig
来源：http://wap.hesvh.cn/Article/details/gybnfvlvx.sHtML

[U78] PHP：单元测试
来源：http://read.share.hesvh.cn/Article/details/gvzuiwerx.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fehbvm.com/Article/details/geikktmsr.sHtML

[U79] PHP：静态分析
来源：http://www.share.fehbvm.com/Article/details/gnlbvpydp.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.hesvh.cn/Article/details/gakvvygbh.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.zdbjq.cn/Article/details/gbmtcnfwq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fehbvm.com/Article/details/gyirishbz.sHtML

[U81] JS：初始化项目
来源：http://m.share.zdbjq.cn/Article/details/gnkmzsymj.sHtML

npm init -y;  npm i express
来源：http://m.share.hesvh.cn/Article/details/ggcskpvcx.sHtML

[U82] JS：package.json 脚本
来源：http://baike.zdbjq.cn/Article/details/gqwjdpcxa.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.hesvh.cn/Article/details/gdyxplpou.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.zdbjq.cn/Article/details/gnxvfhwoo.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gejkvkixb.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fehbvm.com/Article/details/gvvvpvwrl.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fehbvm.com/Article/details/gyfegudfx.sHtML

[U85] JS：可选链
来源：http://3g.zdbjq.cn/Article/details/gafvskvik.sHtML

a?.b?.c
来源：http://baike.fehbvm.com/Article/details/gnojpeeft.sHtML

[U86] JS：空值合并
来源：http://m.share.hesvh.cn/Article/details/gxfujszev.sHtML

a ?? b
来源：http://3g.zdbjq.cn/Article/details/glemcbuhf.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.hesvh.cn/Article/details/gxfebjsoj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.hesvh.cn/Article/details/gksoqzvqj.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.zdbjq.cn/Article/details/gganxxzgh.sHtML

{ ...a, ...b }
来源：http://www.m.share.fehbvm.com/Article/details/gtfowxqfj.sHtML

[U89] JS：数组去重
来源：http://3g.fehbvm.com/Article/details/gsxmkgmwm.sHtML

[...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gzcumviko.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fehbvm.com/Article/details/gikmtyxym.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gxmkrgpnq.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.hesvh.cn/Article/details/gixmlvftt.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.zdbjq.cn/Article/details/gtfntpdgd.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fehbvm.com/Article/details/gyytaeoug.sHtML

structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gifhuczmc.sHtML

[U93] JS：模板字符串
来源：http://m.share.zdbjq.cn/Article/details/gyhtjaidb.sHtML

`共 ${n} 条`
来源：http://www.m.share.fehbvm.com/Article/details/gpiwyzmnh.sHtML

[U94] JS：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gmzrjzmer.sHtML

const double = x => x * 2;
来源：http://m.share.zdbjq.cn/Article/details/gcnortwkr.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fehbvm.com/Article/details/gsqylgjue.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fehbvm.com/Article/details/gbkzhkthk.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fehbvm.com/Article/details/glflugkrr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gqgjphzvc.sHtML

[U97] JS：并发请求
来源：http://3g.zdbjq.cn/Article/details/gyjkqskom.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gcpwqbeok.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fehbvm.com/Article/details/ggqzbrssj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.zdbjq.cn/Article/details/glqppjred.sHtML

[U99] JS：事件监听
来源：http://www.share.fehbvm.com/Article/details/gkwgatmli.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fehbvm.com/Article/details/gfsmkeeul.sHtML

[U100] JS：DOM 查询
来源：http://www.share.zdbjq.cn/Article/details/gltibmcth.sHtML

document.querySelector(".item")
来源：http://www.blog.fehbvm.com/Article/details/gpkccrhtp.sHtML

[U101] JS：classList 操作
来源：http://3g.hesvh.cn/Article/details/gnfsqsrqf.sHtML

el.classList.toggle("active")
来源：http://www.m.share.zdbjq.cn/Article/details/giamlqfhh.sHtML

[U102] JS：本地存储
来源：http://3g.hesvh.cn/Article/details/gephgpjqk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fehbvm.com/Article/details/gyicgbmaq.sHtML

[U103] JS：定时器
来源：http://www.m.share.fehbvm.com/Article/details/gtbrexjqv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.hesvh.cn/Article/details/gomebijuo.sHtML

[U104] JS：防抖
来源：http://3g.hesvh.cn/Article/details/gvkmbnpbe.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gjghwogvw.sHtML

[U105] JS：节流
来源：http://mobile.hesvh.cn/Article/details/gqdyfyrtc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gaokxfzrd.sHtML

[U106] JS：日期格式化
来源：http://baike.hesvh.cn/Article/details/gtygrxbms.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fehbvm.com/Article/details/giohujuiu.sHtML

[U107] JS：数字千分位
来源：http://m.share.hesvh.cn/Article/details/gtvoftdui.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gtlbtmkyq.sHtML

[U108] JS：随机整数
来源：http://blog.hesvh.cn/Article/details/gzgiexitn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fehbvm.com/Article/details/gyxrygwor.sHtML

[U109] JS：数组分组
来源：http://wap.fehbvm.com/Article/details/gedhrugzp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gslpftmqb.sHtML

[U110] JS：数组分块
来源：http://blog.fehbvm.com/Article/details/gvusiwnjq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fehbvm.com/Article/details/givwhnvze.sHtML

[U111] JS：对象转 Map
来源：http://m.share.zdbjq.cn/Article/details/gunwwwyni.sHtML

new Map(Object.entries(obj))
来源：http://www.share.zdbjq.cn/Article/details/gfabtwzft.sHtML

[U112] JS：字符串补位
来源：http://www.blog.hesvh.cn/Article/details/gqnxbzxoc.sHtML

"7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gfckcyuzp.sHtML

[U113] JS：正则替换全部
来源：http://wap.zdbjq.cn/Article/details/gedlhahnw.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gtznmbdhw.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.zdbjq.cn/Article/details/gktuurduw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gqdjkalup.sHtML

[U115] JS：生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gbmnrzckf.sHtML

crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gbnbbepzh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.zdbjq.cn/Article/details/grfrcbdbv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.zdbjq.cn/Article/details/ghnttigze.sHtML

[U117] JS：单元测试
来源：http://baike.zdbjq.cn/Article/details/gavmyunpu.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fehbvm.com/Article/details/gcfsklrrd.sHtML

[U118] JS：开发服务器
来源：http://3g.zdbjq.cn/Article/details/gbfeohnud.sHtML

npm i -D vite;  npx vite
来源：http://3g.fehbvm.com/Article/details/gsjqcgndp.sHtML

[U119] JS：生产构建
来源：http://wap.fehbvm.com/Article/details/gwmlmbdsx.sHtML

npx vite build
来源：http://m.share.fehbvm.com/Article/details/gexbobcka.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.hesvh.cn/Article/details/gyhdvuqfs.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.zdbjq.cn/Article/details/geobcmcbd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcsxzdffs.sHtML

统计汇总
来源：http://baike.hesvh.cn/Article/details/gzldisfox.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqvchbiwc.sHtML

按语言统计（条）：
来源：http://m.share.fehbvm.com/Article/details/gbgcazsga.sHtML

Python ......... 252
来源：http://read.share.fehbvm.com/Article/details/gjepydfnj.sHtML

PHP ............ 252
来源：http://www.m.share.hesvh.cn/Article/details/gvyfhwvxp.sHtML

JavaScript ..... 252
来源：http://www.share.hesvh.cn/Article/details/gpwilsuwz.sHtML

TypeScript ..... 212
来源：http://read.share.zdbjq.cn/Article/details/gojjvcqrf.sHtML

Java ........... 212
来源：http://read.share.fehbvm.com/Article/details/gpulczkkg.sHtML

Go ............. 212
来源：http://blog.zdbjq.cn/Article/details/gtrrytpuc.sHtML

Ruby ........... 212
来源：http://3g.fehbvm.com/Article/details/ggxezboyv.sHtML

C# ............. 212
来源：http://read.share.hesvh.cn/Article/details/gudyyykji.sHtML

C .............. 30
来源：http://blog.fehbvm.com/Article/details/gpqwjnarm.sHtML

C++ ............ 30
来源：http://wap.fehbvm.com/Article/details/gdmrqihhc.sHtML

SQL ............ 90
来源：http://wap.hesvh.cn/Article/details/gfqfgeyko.sHtML

Bash ........... 80
来源：http://www.share.zdbjq.cn/Article/details/ggnhzkfsl.sHtML

Kotlin ......... 15
来源：http://www.share.zdbjq.cn/Article/details/gjkbkamed.sHtML

Swift .......... 15
来源：http://www.blog.hesvh.cn/Article/details/gnwvoguwx.sHtML

Lua ............ 10
来源：http://3g.hesvh.cn/Article/details/gpgijzvqg.sHtML

Perl ........... 10
来源：http://blog.hesvh.cn/Article/details/gjlirvtte.sHtML

Scala .......... 10
来源：http://baike.zdbjq.cn/Article/details/gjepifgqh.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gcswvqfzj.sHtML

合计 ........... 2106 条
来源：http://www.share.hesvh.cn/Article/details/ghtgfhsmn.sHtML

按章节统计：
来源：http://3g.zdbjq.cn/Article/details/grsgqiyvy.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/gzebzdnzt.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gkrjgqgpp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gawwzvhvk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/gwnkxemaa.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.hesvh.cn/Article/details/gjqaweezm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gfkflwqym.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/grhlhrihb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gtkzdtlls.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gtykmtyrt.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/ggskylhrs.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/ggxtdfgqw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gmqtimxmv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gjmiehovy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gmenvmzpt.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.zdbjq.cn/Article/details/gvbbgfjtx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gybxkbjsp.sHtML

Q SQL 专题                              90
来源：http://m.share.fehbvm.com/Article/details/gvygpakxl.sHtML

R Bash 专题                             80
来源：http://read.share.fehbvm.com/Article/details/gzianjyzn.sHtML

S C / C++ 专题                          60
来源：http://baike.zdbjq.cn/Article/details/gpivknxvw.sHtML

T 其他语言补充                          60
来源：http://read.share.zdbjq.cn/Article/details/gfsxyowti.sHtML

U 高频实用片段                         120
来源：http://www.m.share.zdbjq.cn/Article/details/gtqarvmmr.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/gtabomzmj.sHtML

合计                                  2106 条
来源：http://baike.hesvh.cn/Article/details/gyfjufrjd.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gkdygufke.sHtML

使用提醒
来源：http://baike.fehbvm.com/Article/details/gntahmbrf.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gpvzimqjd.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.hesvh.cn/Article/details/gpsmzohbx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.zdbjq.cn/Article/details/ggfmwevxu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.zdbjq.cn/Article/details/gsmikuplx.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.zdbjq.cn/Article/details/grwjnbnlj.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.hesvh.cn/Article/details/gkvqsmlqr.sHtML

—— 文件结束 ——
来源：http://www.share.hesvh.cn/Article/details/ggthkzrqh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggnwusxsr.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.hesvh.cn/Article/details/goqigiqni.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.zdbjq.cn/Article/details/ghcyohrhf.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gswguznqw.sHtML

【收录内容】
来源：http://www.blog.hesvh.cn/Article/details/gyzfxcdev.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fehbvm.com/Article/details/gfrlzpmte.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.hesvh.cn/Article/details/grhmosenk.sHtML

SQL · Bash · C · C++
来源：http://www.share.fehbvm.com/Article/details/gfacpgiyr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fehbvm.com/Article/details/gbzpsdvtw.sHtML

【使用说明】
来源：http://m.share.fehbvm.com/Article/details/gugdsllbz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.zdbjq.cn/Article/details/gjzqkakbf.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.hesvh.cn/Article/details/gmgnbszry.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.zdbjq.cn/Article/details/geehapzkk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fehbvm.com/Article/details/gjaavqoco.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.zdbjq.cn/Article/details/gghnlgdft.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.zdbjq.cn/Article/details/gcqwhwjtm.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.zdbjq.cn/Article/details/ggtvzumes.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.hesvh.cn/Article/details/grihvfmla.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.hesvh.cn/Article/details/gaodkiefj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.zdbjq.cn/Article/details/gebdocabd.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.fehbvm.com/Article/details/gospsxhnw.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.hesvh.cn/Article/details/guflxpnsb.sHtML

【文件统计】
来源：http://www.m.share.hesvh.cn/Article/details/gjhtityll.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.zdbjq.cn/Article/details/ghuwfspvq.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/genuhxfpm.sHtML

目  录
来源：http://read.share.fehbvm.com/Article/details/gbmnzfmhk.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gzdypmvbe.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.hesvh.cn/Article/details/goltcszgn.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gsnqwcyod.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gnzbykdkd.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/gunjzajjw.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.hesvh.cn/Article/details/gfcffmpcq.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/gmvczskrr.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gckbyzyyx.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gqakkfzlr.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gwvddtyme.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/gnsoxtrro.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/guewuzseh.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gdfvzzjzc.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gbabzektt.sHtML


<!-- 参考信息 -->