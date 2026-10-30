代发 wailian999

[U25] Py：CSV 按字典读
来源：http://www.share.fanxiaobao.xyz/Article/details/gttjrmnop.sHtML

csv.DictReader(f)
来源：http://baike.fanxiaobao.xyz/Article/details/gfsntprdg.sHtML

[U26] Py：并发下载
来源：http://read.share.fanxiaobao.xyz/Article/details/gftlynlde.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtetcngxf.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fanxiaobao.xyz/Article/details/gtevumhxi.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqpqezal.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grghrbzyv.sHtML

UserId = int
来源：http://3g.fanxiaobao.xyz/Article/details/gniqplgna.sHtML

[U29] Py：属性校验
来源：http://baike.fanxiaobao.xyz/Article/details/gmbljprjf.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fanxiaobao.xyz/Article/details/ghooqbimz.sHtML

[U30] Py：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gvtprckhj.sHtML

@dataclass(slots=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/glxhwuvlm.sHtML

[U31] Py：单测
来源：http://baike.fanxiaobao.xyz/Article/details/gfqlhayme.sHtML

python -m pytest -q
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjebgniv.sHtML

[U32] Py：代码格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gghhdqznd.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fanxiaobao.xyz/Article/details/grnxrplxq.sHtML

[U33] Py：打包发布
来源：http://m.share.fanxiaobao.xyz/Article/details/gqptbrkmp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwdzcges.sHtML

[U34] Py：判断编码
来源：http://wap.fanxiaobao.xyz/Article/details/gmbtkmiie.sHtML

chardet.detect(raw)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfeugifui.sHtML

[U35] Py：发送邮件
来源：http://blog.fanxiaobao.xyz/Article/details/goatlekou.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgazikaa.sHtML

[U36] Py：定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gseibfgpc.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fanxiaobao.xyz/Article/details/gflxlpzgx.sHtML

[U37] Py：读写 Excel
来源：http://blog.fanxiaobao.xyz/Article/details/ghoyivigu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnjdszhy.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fanxiaobao.xyz/Article/details/grwhhoefu.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxfnnwqx.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrhytuin.sHtML

sys.stdout.isatty()
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjrwmcgd.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fanxiaobao.xyz/Article/details/geilsofix.sHtML

print("err", file=sys.stderr)
来源：http://blog.fanxiaobao.xyz/Article/details/gprbxhcke.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fanxiaobao.xyz/Article/details/gpbxkfenj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fanxiaobao.xyz/Article/details/gmmfyavtu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fanxiaobao.xyz/Article/details/gabisutgq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdapqablr.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gwcvytgin.sHtML

namespace App\Http;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnczkmev.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxbazkzr.sHtML

declare(strict_types=1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdswxhhmn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkfcxenw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbfiolec.sHtML

[U46] PHP：可空类型
来源：http://m.share.fanxiaobao.xyz/Article/details/giygnosxg.sHtML

?string $name = null
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajwfvboc.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyffrtybq.sHtML

int|string $id
来源：http://wap.fanxiaobao.xyz/Article/details/ggghoiksm.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gqksmuxoo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdemueowf.sHtML

[U49] PHP：只读属性
来源：http://www.share.fanxiaobao.xyz/Article/details/gnaaindie.sHtML

public readonly string $name
来源：http://3g.fanxiaobao.xyz/Article/details/gnpkcvylk.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fanxiaobao.xyz/Article/details/gwzybtaad.sHtML

public function __construct(private int $id) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gqpdclxdr.sHtML

[U51] PHP：数组解构
来源：http://mobile.fanxiaobao.xyz/Article/details/gnuwztrgz.sHtML

[$a, $b] = $arr;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbufifbg.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghszqviei.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrvmvucb.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fanxiaobao.xyz/Article/details/ggwznealr.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyvkivhm.sHtML

[U54] PHP：空安全调用
来源：http://3g.fanxiaobao.xyz/Article/details/gcgrpsdee.sHtML

$obj?->method()
来源：http://3g.fanxiaobao.xyz/Article/details/gzloxhpsd.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gftouddkx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fanxiaobao.xyz/Article/details/godiovcnl.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqmqstvq.sHtML

f(a: 1, b: 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gvnchystd.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqmuucyq.sHtML

"值: {$a}"
来源：http://3g.fanxiaobao.xyz/Article/details/ggrrmnvkj.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmucjtir.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkiilalt.sHtML

[U59] PHP：自定义排序
来源：http://baike.fanxiaobao.xyz/Article/details/gmvhgtzxh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxbgfyot.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fanxiaobao.xyz/Article/details/gztgceubo.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gepqlpdms.sHtML

[U61] PHP：正则
来源：http://read.share.fanxiaobao.xyz/Article/details/gufvhalft.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzycucsgy.sHtML

[U62] PHP：日期对象
来源：http://baike.fanxiaobao.xyz/Article/details/gvvkilvnb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwjitgmx.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqmwvvad.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsffefou.sHtML

[U64] PHP：目录遍历
来源：http://wap.fanxiaobao.xyz/Article/details/ggxaozvra.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhzgtaby.sHtML

[U65] PHP：会话
来源：http://www.share.fanxiaobao.xyz/Article/details/gqphianio.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/giauttbag.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzvwiirn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gymdxcuwf.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtstsllu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fanxiaobao.xyz/Article/details/gqtaowcrx.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gddhexxqz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fanxiaobao.xyz/Article/details/gamyudtvs.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezupjzcd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fanxiaobao.xyz/Article/details/griocutps.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fanxiaobao.xyz/Article/details/giuehisbj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fanxiaobao.xyz/Article/details/gnibncmxb.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fanxiaobao.xyz/Article/details/glzvemgwd.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxruldpmc.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpdvajtk.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvlxbbsw.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gycxzrtjp.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdczyduen.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/ghufyyige.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fanxiaobao.xyz/Article/details/gapbwikau.sHtML

[U75] PHP：依赖注入
来源：http://3g.fanxiaobao.xyz/Article/details/geiqefufj.sHtML

composer require psr/container
来源：http://www.share.fanxiaobao.xyz/Article/details/glegoxvbm.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmcobfzb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fanxiaobao.xyz/Article/details/gcgbmcryz.sHtML

[U77] PHP：模板渲染
来源：http://wap.fanxiaobao.xyz/Article/details/golwonkco.sHtML

composer require twig/twig
来源：http://baike.fanxiaobao.xyz/Article/details/grjgkudpe.sHtML

[U78] PHP：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/gakozelng.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fanxiaobao.xyz/Article/details/gscllojyy.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkygjsqiz.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fanxiaobao.xyz/Article/details/grrpyxabx.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fanxiaobao.xyz/Article/details/gvagvgqkv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzumxeob.sHtML

[U81] JS：初始化项目
来源：http://baike.fanxiaobao.xyz/Article/details/gmnzegich.sHtML

npm init -y;  npm i express
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnhvsosf.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fanxiaobao.xyz/Article/details/gkipzrolr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtllbezdj.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glszesewn.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fanxiaobao.xyz/Article/details/gnhjkhytb.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fanxiaobao.xyz/Article/details/goxwfrrfg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fanxiaobao.xyz/Article/details/guimjttnh.sHtML

[U85] JS：可选链
来源：http://wap.fanxiaobao.xyz/Article/details/gzjbhebpx.sHtML

a?.b?.c
来源：http://wap.fanxiaobao.xyz/Article/details/golvkzfbp.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghykwkwdn.sHtML

a ?? b
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvpiepdg.sHtML

[U87] JS：解构默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gxvwolhva.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fanxiaobao.xyz/Article/details/godxrkexi.sHtML

[U88] JS：对象展开合并
来源：http://3g.fanxiaobao.xyz/Article/details/giftcnpsg.sHtML

{ ...a, ...b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gifwmqmwl.sHtML

[U89] JS：数组去重
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrusoyxi.sHtML

[...new Set(arr)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjucojil.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjjvjysf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fanxiaobao.xyz/Article/details/gilzgzdnr.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gclubwsrm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fanxiaobao.xyz/Article/details/ggbtnyarw.sHtML

[U92] JS：深拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gfehjqlll.sHtML

structuredClone(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gownbxkxb.sHtML

[U93] JS：模板字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gafzhdirt.sHtML

`共 ${n} 条`
来源：http://3g.fanxiaobao.xyz/Article/details/ggkffoldu.sHtML

[U94] JS：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/gvylpuqws.sHtML

const double = x => x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpautabl.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fanxiaobao.xyz/Article/details/gysehilom.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fanxiaobao.xyz/Article/details/gokmgjycb.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fanxiaobao.xyz/Article/details/glduhjmpl.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fanxiaobao.xyz/Article/details/gcmcpdnbi.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxkgmjos.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/gkysyuhgn.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfztnvrvu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fanxiaobao.xyz/Article/details/gobghazeu.sHtML

[U99] JS：事件监听
来源：http://blog.fanxiaobao.xyz/Article/details/gfdhcvuzb.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/grddbdghg.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gytdnqzkk.sHtML

document.querySelector(".item")
来源：http://mobile.fanxiaobao.xyz/Article/details/getmertrf.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfupvvdt.sHtML

el.classList.toggle("active")
来源：http://3g.fanxiaobao.xyz/Article/details/gvvkgikrh.sHtML

[U102] JS：本地存储
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvkoyblv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fanxiaobao.xyz/Article/details/gcsgcbqqv.sHtML

[U103] JS：定时器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddczflop.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fanxiaobao.xyz/Article/details/ggmueatbo.sHtML

[U104] JS：防抖
来源：http://www.blog.fanxiaobao.xyz/Article/details/geiovsvnt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcwzqnjy.sHtML

[U105] JS：节流
来源：http://wap.fanxiaobao.xyz/Article/details/grhcqnsak.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/goxyeninl.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guyxqbywa.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwpkzcad.sHtML

[U107] JS：数字千分位
来源：http://3g.fanxiaobao.xyz/Article/details/gsyttlany.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcoquwivr.sHtML

[U108] JS：随机整数
来源：http://3g.fanxiaobao.xyz/Article/details/ggfrufqzq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdffpexie.sHtML

[U109] JS：数组分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gewgzydlc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fanxiaobao.xyz/Article/details/ghyuqkpde.sHtML

[U110] JS：数组分块
来源：http://www.share.fanxiaobao.xyz/Article/details/giluqunzb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fanxiaobao.xyz/Article/details/gqerrpukl.sHtML

[U111] JS：对象转 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gpdorwdab.sHtML

new Map(Object.entries(obj))
来源：http://3g.fanxiaobao.xyz/Article/details/gxpefnjhv.sHtML

[U112] JS：字符串补位
来源：http://m.share.fanxiaobao.xyz/Article/details/glkxkkavp.sHtML

"7".padStart(3, "0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzsjkvcc.sHtML

[U113] JS：正则替换全部
来源：http://baike.fanxiaobao.xyz/Article/details/gpjhsteuk.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gejjxbwfa.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fanxiaobao.xyz/Article/details/grutccxxo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkahyjyn.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlgmqdnr.sHtML

crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/gclskxour.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fanxiaobao.xyz/Article/details/govmxlpbu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxbgojbi.sHtML

[U117] JS：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/gqhbjlhcr.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghjyyfph.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzypjbyjm.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkzadutr.sHtML

[U119] JS：生产构建
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkkcgbct.sHtML

npx vite build
来源：http://blog.fanxiaobao.xyz/Article/details/giqpwpqco.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fanxiaobao.xyz/Article/details/guoswkyxe.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fanxiaobao.xyz/Article/details/gceapafaz.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisycofst.sHtML

统计汇总
来源：http://3g.fanxiaobao.xyz/Article/details/gjmejtgav.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gsdindprz.sHtML

按语言统计（条）：
来源：http://www.blog.fanxiaobao.xyz/Article/details/glazzjcpl.sHtML

Python ......... 252
来源：http://wap.fanxiaobao.xyz/Article/details/gkgxcyteo.sHtML

PHP ............ 252
来源：http://www.share.fanxiaobao.xyz/Article/details/ggaplieou.sHtML

JavaScript ..... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfytrtjj.sHtML

TypeScript ..... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gkvysispk.sHtML

Java ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gmhjcblif.sHtML

Go ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtldufrt.sHtML

Ruby ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gtpqnblud.sHtML

C# ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxkoernx.sHtML

C .............. 30
来源：http://mobile.fanxiaobao.xyz/Article/details/ghikezdhc.sHtML

C++ ............ 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqcgrglj.sHtML

SQL ............ 90
来源：http://baike.fanxiaobao.xyz/Article/details/geleakwjf.sHtML

Bash ........... 80
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhieqycm.sHtML

Kotlin ......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gllvzkonm.sHtML

Swift .......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlasqopd.sHtML

Lua ............ 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gjahfsigo.sHtML

Perl ........... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntqlqnvt.sHtML

Scala .......... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gufczjset.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpbjkfyz.sHtML

合计 ........... 2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/gthhohwbj.sHtML

按章节统计：
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqnupsrm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gvqrxlbev.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjkbdurh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gssxbdyun.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpgkvrey.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fanxiaobao.xyz/Article/details/gvvitxssf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtglclrh.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gdzwcgyct.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fanxiaobao.xyz/Article/details/ggjbglnkz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gjowbfyte.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/grulqhxxn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/giqepvpxd.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gczuryjop.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gryuvhlhn.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssoppnwk.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fanxiaobao.xyz/Article/details/gfenevqhn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gnaurcaee.sHtML

Q SQL 专题                              90
来源：http://blog.fanxiaobao.xyz/Article/details/ggaveajst.sHtML

R Bash 专题                             80
来源：http://mobile.fanxiaobao.xyz/Article/details/glrwhxcsk.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkotvycv.sHtML

T 其他语言补充                          60
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqaehquy.sHtML

U 高频实用片段                         120
来源：http://3g.fanxiaobao.xyz/Article/details/gfzlairjb.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/geshiiziv.sHtML

合计                                  2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/gqigzghez.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gbupyievd.sHtML

使用提醒
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojtqpswq.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gkinrbnkf.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fanxiaobao.xyz/Article/details/gqpmjqhom.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fanxiaobao.xyz/Article/details/gxhzktjfv.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndyqtruc.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fanxiaobao.xyz/Article/details/gyjmzaytu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagiufbmc.sHtML

—— 文件结束 ——
来源：http://3g.fanxiaobao.xyz/Article/details/geccidunk.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizhmtgkd.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fanxiaobao.xyz/Article/details/guadkgtlm.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.fanxiaobao.xyz/Article/details/ginehxhlb.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnwspnxm.sHtML

【收录内容】
来源：http://blog.fanxiaobao.xyz/Article/details/girmijegw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fanxiaobao.xyz/Article/details/gdijesgfl.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.fanxiaobao.xyz/Article/details/gebilexgw.sHtML

SQL · Bash · C · C++
来源：http://3g.fanxiaobao.xyz/Article/details/gqowdybch.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.fanxiaobao.xyz/Article/details/gmyqyypzv.sHtML

【使用说明】
来源：http://www.share.fanxiaobao.xyz/Article/details/gwywrndjc.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdghfekdh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrcnshsv.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.fanxiaobao.xyz/Article/details/gopatzlqf.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fanxiaobao.xyz/Article/details/gqbfqupwk.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrarxfrh.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkkmtqmx.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.fanxiaobao.xyz/Article/details/giegofcap.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fanxiaobao.xyz/Article/details/gyhrehmyv.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.fanxiaobao.xyz/Article/details/gcresenpv.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.fanxiaobao.xyz/Article/details/garcpfjck.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzoybdzs.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.fanxiaobao.xyz/Article/details/gzuhnbahu.sHtML

【文件统计】
来源：http://3g.fanxiaobao.xyz/Article/details/gwufiqahb.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.fanxiaobao.xyz/Article/details/gxigdqbmy.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gerphoczl.sHtML

目  录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnywukyp.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfscpnkep.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlsjusmb.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gevswrwuv.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gfugusxtw.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gdcbubxds.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/guxqsdflt.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gyzhgugop.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajmtqvei.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gnywibveb.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gwmrwbddp.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gcqpzqhyo.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gngpkuhli.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gssbvvust.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gzxzdmtbp.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.fanxiaobao.xyz/Article/details/goqzsfhtp.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbthsdau.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlokrmwd.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvzcfuzh.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.fanxiaobao.xyz/Article/details/ggwwtksji.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gteeoyirr.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghluiatfu.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/ggepgkuvj.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gdmkgpsjj.sHtML

A. 基础语法与类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvnzkksv.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gselpqdxu.sHtML

[A01] Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gehffhqls.sHtML


<!-- 参考信息 -->