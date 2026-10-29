代发 wailian999

[U27] Py：异步 HTTP
来源：http://www.m.share.hesvh.cn/Article/details/gfgfxwqhb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fehbvm.com/Article/details/grzojpqvo.sHtML

[U28] Py：类型别名
来源：http://www.blog.hesvh.cn/Article/details/gjvhriewy.sHtML

UserId = int
来源：http://read.share.zdbjq.cn/Article/details/gygataqyr.sHtML

[U29] Py：属性校验
来源：http://mobile.hesvh.cn/Article/details/gvogfrlma.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fehbvm.com/Article/details/grxwtpmdp.sHtML

[U30] Py：数据类
来源：http://baike.zdbjq.cn/Article/details/gkznkpexi.sHtML

@dataclass(slots=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gaopcyepn.sHtML

[U31] Py：单测
来源：http://m.share.fehbvm.com/Article/details/gaykelayt.sHtML

python -m pytest -q
来源：http://m.share.zdbjq.cn/Article/details/gffobilya.sHtML

[U32] Py：代码格式化
来源：http://m.share.hesvh.cn/Article/details/gxyltmvuj.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.hesvh.cn/Article/details/gfrncfvwn.sHtML

[U33] Py：打包发布
来源：http://www.share.zdbjq.cn/Article/details/gysobzlzj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/guxstmfay.sHtML

[U34] Py：判断编码
来源：http://www.blog.hesvh.cn/Article/details/gobicbicx.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/gjkdslcts.sHtML

[U35] Py：发送邮件
来源：http://blog.fehbvm.com/Article/details/gilensmfg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.hesvh.cn/Article/details/gmcqhzohh.sHtML

[U36] Py：定时任务
来源：http://blog.zdbjq.cn/Article/details/gwwqxzinb.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fehbvm.com/Article/details/gnrxipodr.sHtML

[U37] Py：读写 Excel
来源：http://m.share.hesvh.cn/Article/details/gyvkzrapw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fehbvm.com/Article/details/gujhdhyvb.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.hesvh.cn/Article/details/gplfniyre.sHtML

Path(__file__).resolve().parent
来源：http://wap.fehbvm.com/Article/details/gkzmejuyu.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fehbvm.com/Article/details/gamzjxzga.sHtML

sys.stdout.isatty()
来源：http://wap.hesvh.cn/Article/details/guvbyqfiv.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.hesvh.cn/Article/details/geofuvonq.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gxccvfugu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/gkaystspd.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gulxfrytf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fehbvm.com/Article/details/gbkjooksc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.zdbjq.cn/Article/details/gsarpgnpi.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.hesvh.cn/Article/details/gawaipptb.sHtML

namespace App\Http;
来源：http://www.share.zdbjq.cn/Article/details/guakjckjr.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.hesvh.cn/Article/details/gvqlkfcdi.sHtML

declare(strict_types=1);
来源：http://www.share.zdbjq.cn/Article/details/gtuvewlmx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.hesvh.cn/Article/details/gyzqmaevg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/ggrbcfihu.sHtML

[U46] PHP：可空类型
来源：http://baike.zdbjq.cn/Article/details/gajgulekj.sHtML

?string $name = null
来源：http://mobile.fehbvm.com/Article/details/gzegpouji.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fehbvm.com/Article/details/gbgeavrfa.sHtML

int|string $id
来源：http://www.blog.zdbjq.cn/Article/details/ggyhdwslb.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fehbvm.com/Article/details/gsdmsrfel.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.zdbjq.cn/Article/details/gwdcubyub.sHtML

[U49] PHP：只读属性
来源：http://m.share.zdbjq.cn/Article/details/guameblhh.sHtML

public readonly string $name
来源：http://m.share.hesvh.cn/Article/details/gyhegghnx.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fehbvm.com/Article/details/gecigdrar.sHtML

public function __construct(private int $id) {}
来源：http://m.share.hesvh.cn/Article/details/grazyxgvk.sHtML

[U51] PHP：数组解构
来源：http://baike.hesvh.cn/Article/details/guwcxxngu.sHtML

[$a, $b] = $arr;
来源：http://read.share.zdbjq.cn/Article/details/gizkfkaig.sHtML

[U52] PHP：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gxxsjrcfy.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gwrocynxr.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/gvuutweuk.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/ggihsqukr.sHtML

[U54] PHP：空安全调用
来源：http://baike.hesvh.cn/Article/details/gswrxfcnc.sHtML

$obj?->method()
来源：http://www.share.zdbjq.cn/Article/details/gmwvdoczx.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.hesvh.cn/Article/details/gnchfpifa.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/gywupfvjs.sHtML

[U56] PHP：命名参数
来源：http://mobile.hesvh.cn/Article/details/gvrwvzppo.sHtML

f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gbfsjvgxm.sHtML

[U57] PHP：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gkodxpgmx.sHtML

"值: {$a}"
来源：http://www.share.zdbjq.cn/Article/details/giaigkerd.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/gxqttoebd.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.zdbjq.cn/Article/details/gvkorgolf.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.hesvh.cn/Article/details/grcmtodgy.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gwnxgepgr.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.hesvh.cn/Article/details/grgcjqywd.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.zdbjq.cn/Article/details/geocgzeid.sHtML

[U61] PHP：正则
来源：http://m.share.hesvh.cn/Article/details/gjwujnnud.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gbweindqi.sHtML

[U62] PHP：日期对象
来源：http://wap.fehbvm.com/Article/details/ghqipyryr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.zdbjq.cn/Article/details/gystimxrq.sHtML

[U63] PHP：文件读写
来源：http://3g.zdbjq.cn/Article/details/gkcdvwygv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.hesvh.cn/Article/details/glhfifsze.sHtML

[U64] PHP：目录遍历
来源：http://wap.zdbjq.cn/Article/details/gofpnbiqa.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.zdbjq.cn/Article/details/gzmwtfkhb.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/gyrxucler.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gyuqzfspk.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.zdbjq.cn/Article/details/gwruczfme.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fehbvm.com/Article/details/gyflmeyff.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.zdbjq.cn/Article/details/gzoecfyez.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.hesvh.cn/Article/details/giluwilbs.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fehbvm.com/Article/details/gogeiiqcy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.hesvh.cn/Article/details/gstazyhpn.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.hesvh.cn/Article/details/gcgqstpub.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.zdbjq.cn/Article/details/gnxndrkwa.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.zdbjq.cn/Article/details/ggyprqhdl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.zdbjq.cn/Article/details/gurjflxiq.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/gifrcqmzc.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gxtyettuk.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.zdbjq.cn/Article/details/gpaozkjqj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.zdbjq.cn/Article/details/gyeeqmzsr.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.hesvh.cn/Article/details/guzxfscrc.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.zdbjq.cn/Article/details/gshbfzivf.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gievclpur.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fehbvm.com/Article/details/gqmprwkuu.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.hesvh.cn/Article/details/gbjvtfilt.sHtML

composer require psr/container
来源：http://www.m.share.zdbjq.cn/Article/details/gxvzklxfx.sHtML

[U76] PHP：简单路由
来源：http://m.share.hesvh.cn/Article/details/gkkhgnreq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.hesvh.cn/Article/details/gbtggzewl.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fehbvm.com/Article/details/gjwkozywi.sHtML

composer require twig/twig
来源：http://blog.zdbjq.cn/Article/details/gaiexqbuu.sHtML

[U78] PHP：单元测试
来源：http://mobile.hesvh.cn/Article/details/gumqzbhok.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fehbvm.com/Article/details/grsngxmkv.sHtML

[U79] PHP：静态分析
来源：http://3g.hesvh.cn/Article/details/gdnqxoxjo.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.zdbjq.cn/Article/details/gebjamxvt.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.zdbjq.cn/Article/details/gihvofehh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fehbvm.com/Article/details/grcxzafaq.sHtML

[U81] JS：初始化项目
来源：http://baike.zdbjq.cn/Article/details/gqdbbgrkl.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/gritujirs.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.zdbjq.cn/Article/details/gzsgfalce.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.zdbjq.cn/Article/details/gzlwdpajn.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fehbvm.com/Article/details/gefmlfgpf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/geplyuftt.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fehbvm.com/Article/details/guntpsxrg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fehbvm.com/Article/details/gooiebmel.sHtML

[U85] JS：可选链
来源：http://wap.zdbjq.cn/Article/details/gdewhmdpp.sHtML

a?.b?.c
来源：http://www.share.hesvh.cn/Article/details/gspgiqnfg.sHtML

[U86] JS：空值合并
来源：http://www.blog.hesvh.cn/Article/details/gdeydzvpa.sHtML

a ?? b
来源：http://www.share.fehbvm.com/Article/details/grdhqhdpt.sHtML

[U87] JS：解构默认值
来源：http://m.share.zdbjq.cn/Article/details/gkrfojrsc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.hesvh.cn/Article/details/gbzpwokdr.sHtML

[U88] JS：对象展开合并
来源：http://3g.hesvh.cn/Article/details/gzqxjohfg.sHtML

{ ...a, ...b }
来源：http://read.share.fehbvm.com/Article/details/gekntglkn.sHtML

[U89] JS：数组去重
来源：http://m.share.fehbvm.com/Article/details/gccpazulz.sHtML

[...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/ggruihjha.sHtML

[U90] JS：数字数组排序
来源：http://wap.zdbjq.cn/Article/details/gtruzlrde.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/ganitizyv.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.hesvh.cn/Article/details/gsxfagrgo.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.hesvh.cn/Article/details/gkeklfnvs.sHtML

[U92] JS：深拷贝
来源：http://baike.zdbjq.cn/Article/details/gbagwimaw.sHtML

structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/gfobooqzm.sHtML

[U93] JS：模板字符串
来源：http://blog.fehbvm.com/Article/details/gjqwviwbk.sHtML

`共 ${n} 条`
来源：http://baike.fehbvm.com/Article/details/giluhyyns.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gurvrghbb.sHtML

const double = x => x * 2;
来源：http://3g.fehbvm.com/Article/details/gqwuhbwkb.sHtML

[U95] JS：Promise 包装
来源：http://m.share.hesvh.cn/Article/details/ghgohejme.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.zdbjq.cn/Article/details/ginoavmgb.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fehbvm.com/Article/details/gofxzdlxe.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gcmpctrkc.sHtML

[U97] JS：并发请求
来源：http://read.share.zdbjq.cn/Article/details/gjzopnaqn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gywoyjaav.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.hesvh.cn/Article/details/gqkehfpao.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fehbvm.com/Article/details/grkhycytt.sHtML

[U99] JS：事件监听
来源：http://m.share.zdbjq.cn/Article/details/gjzsxcfcv.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.zdbjq.cn/Article/details/gqvowemcb.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fehbvm.com/Article/details/grmkivcpi.sHtML

document.querySelector(".item")
来源：http://www.m.share.hesvh.cn/Article/details/gjkfjqkeu.sHtML

[U101] JS：classList 操作
来源：http://www.share.zdbjq.cn/Article/details/gpexoqlhl.sHtML

el.classList.toggle("active")
来源：http://www.blog.hesvh.cn/Article/details/gnuvmjmmg.sHtML

[U102] JS：本地存储
来源：http://www.blog.hesvh.cn/Article/details/gbjdvcygz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.zdbjq.cn/Article/details/ghzcsovfh.sHtML

[U103] JS：定时器
来源：http://www.m.share.fehbvm.com/Article/details/ggvheferg.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fehbvm.com/Article/details/gchnqtilb.sHtML

[U104] JS：防抖
来源：http://read.share.zdbjq.cn/Article/details/gwittomtk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gkglmbtwc.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/gzwhiesfq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fehbvm.com/Article/details/gygnszcrv.sHtML

[U106] JS：日期格式化
来源：http://read.share.hesvh.cn/Article/details/ggjidnyxf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fehbvm.com/Article/details/gnafwfztv.sHtML

[U107] JS：数字千分位
来源：http://blog.hesvh.cn/Article/details/gbknrqiuu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/guwkrkqxw.sHtML

[U108] JS：随机整数
来源：http://baike.hesvh.cn/Article/details/gruwkdvig.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.zdbjq.cn/Article/details/gwqbcsjfi.sHtML

[U109] JS：数组分组
来源：http://mobile.hesvh.cn/Article/details/grbcnsmam.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gqooivreh.sHtML

[U110] JS：数组分块
来源：http://mobile.hesvh.cn/Article/details/gdojbmprd.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/gookmiazt.sHtML

[U111] JS：对象转 Map
来源：http://wap.hesvh.cn/Article/details/ggmjxvaye.sHtML

new Map(Object.entries(obj))
来源：http://blog.hesvh.cn/Article/details/gjhxzzxae.sHtML

[U112] JS：字符串补位
来源：http://www.share.hesvh.cn/Article/details/gyeajwhuk.sHtML

"7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/ghmxvgpft.sHtML

[U113] JS：正则替换全部
来源：http://baike.zdbjq.cn/Article/details/gdrveauym.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/grdjmzbae.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.hesvh.cn/Article/details/gvfbfyhje.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gmudkhssi.sHtML

[U115] JS：生成 UUID
来源：http://www.share.hesvh.cn/Article/details/genolrzff.sHtML

crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gfuprrrkm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fehbvm.com/Article/details/gruxbliqh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.zdbjq.cn/Article/details/gmxehuvqr.sHtML

[U117] JS：单元测试
来源：http://3g.zdbjq.cn/Article/details/gtaafkjyc.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.zdbjq.cn/Article/details/geazkktdc.sHtML

[U118] JS：开发服务器
来源：http://3g.fehbvm.com/Article/details/gbgwsknej.sHtML

npm i -D vite;  npx vite
来源：http://m.share.hesvh.cn/Article/details/gvntqrheo.sHtML

[U119] JS：生产构建
来源：http://m.share.zdbjq.cn/Article/details/gqsmejbcm.sHtML

npx vite build
来源：http://blog.hesvh.cn/Article/details/gcxcexpsm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.zdbjq.cn/Article/details/gdwqnpfzk.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.zdbjq.cn/Article/details/gekyouzvh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfgqbhlsu.sHtML

统计汇总
来源：http://3g.fehbvm.com/Article/details/gebqhnfre.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gorjxeamu.sHtML

按语言统计（条）：
来源：http://www.share.hesvh.cn/Article/details/gamsbbshe.sHtML

Python ......... 252
来源：http://baike.hesvh.cn/Article/details/gipgatolg.sHtML

PHP ............ 252
来源：http://wap.fehbvm.com/Article/details/gxcxvettf.sHtML

JavaScript ..... 252
来源：http://www.share.hesvh.cn/Article/details/glzqldwlu.sHtML

TypeScript ..... 212
来源：http://m.share.zdbjq.cn/Article/details/gbmdyxtob.sHtML

Java ........... 212
来源：http://mobile.hesvh.cn/Article/details/gqbtuzzct.sHtML

Go ............. 212
来源：http://baike.zdbjq.cn/Article/details/gmhddnolb.sHtML

Ruby ........... 212
来源：http://m.share.fehbvm.com/Article/details/grobuddai.sHtML

C# ............. 212
来源：http://3g.zdbjq.cn/Article/details/gqkjgfqaz.sHtML

C .............. 30
来源：http://mobile.zdbjq.cn/Article/details/gnbfychzx.sHtML

C++ ............ 30
来源：http://3g.fehbvm.com/Article/details/gjubkrzhq.sHtML

SQL ............ 90
来源：http://wap.fehbvm.com/Article/details/gsdtkenzg.sHtML

Bash ........... 80
来源：http://www.m.share.fehbvm.com/Article/details/gsiawxdmj.sHtML

Kotlin ......... 15
来源：http://baike.zdbjq.cn/Article/details/gpmtzpghw.sHtML

Swift .......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gdchqlalq.sHtML

Lua ............ 10
来源：http://wap.hesvh.cn/Article/details/geuyrhmoi.sHtML

Perl ........... 10
来源：http://m.share.hesvh.cn/Article/details/gkkbeutyd.sHtML

Scala .......... 10
来源：http://www.m.share.fehbvm.com/Article/details/gylzvxoos.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gtmvjtmwm.sHtML

合计 ........... 2106 条
来源：http://www.blog.hesvh.cn/Article/details/gjxzmbasn.sHtML

按章节统计：
来源：http://www.m.share.hesvh.cn/Article/details/guzbsnwag.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/glbccgqvd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gxfacpgmy.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gmxvehdns.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/ggfsbtrjh.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.zdbjq.cn/Article/details/gnqgmzowi.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/gfzlwpcjy.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gqgiomuhn.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gjwgibfpx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gicqofynf.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/glwybufie.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gqfrzmgdu.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gcbyyclcb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gngnuniaz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gbrbwuyhp.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fehbvm.com/Article/details/ghbkdxfen.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gkseizpdv.sHtML

Q SQL 专题                              90
来源：http://3g.zdbjq.cn/Article/details/gapsstzyq.sHtML

R Bash 专题                             80
来源：http://mobile.zdbjq.cn/Article/details/gwljmmggw.sHtML

S C / C++ 专题                          60
来源：http://blog.zdbjq.cn/Article/details/gyivifzfc.sHtML

T 其他语言补充                          60
来源：http://www.blog.fehbvm.com/Article/details/gegcdvnwe.sHtML

U 高频实用片段                         120
来源：http://wap.hesvh.cn/Article/details/gtyefvxtb.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gvygpdcyl.sHtML

合计                                  2106 条
来源：http://baike.zdbjq.cn/Article/details/getnypcpo.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gztqjjcoh.sHtML

使用提醒
来源：http://m.share.zdbjq.cn/Article/details/gpgdnpcnc.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gookhugql.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.zdbjq.cn/Article/details/gkzehdywd.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.zdbjq.cn/Article/details/gfrnogmqw.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.fehbvm.com/Article/details/ghputnwwd.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.hesvh.cn/Article/details/gqyciwjcc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fehbvm.com/Article/details/gsucpkyuf.sHtML

—— 文件结束 ——
来源：http://read.share.fehbvm.com/Article/details/gdhucnups.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqozibpgo.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.hesvh.cn/Article/details/gczxixkon.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fehbvm.com/Article/details/gzgxdmnlr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gsdzuyszz.sHtML

【收录内容】
来源：http://3g.hesvh.cn/Article/details/gxemipobi.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.zdbjq.cn/Article/details/gbuockguq.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.fehbvm.com/Article/details/gphxurfjv.sHtML

SQL · Bash · C · C++
来源：http://www.share.hesvh.cn/Article/details/gxndzgvui.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.zdbjq.cn/Article/details/gaxteglqr.sHtML

【使用说明】
来源：http://blog.hesvh.cn/Article/details/gdnjxylai.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fehbvm.com/Article/details/gazszkqoq.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.fehbvm.com/Article/details/gaqgcnpsl.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.zdbjq.cn/Article/details/guybgyjbd.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.fehbvm.com/Article/details/ggvsvyjns.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.hesvh.cn/Article/details/gzjkjafkm.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.zdbjq.cn/Article/details/gjvghgail.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.zdbjq.cn/Article/details/gpjkxaunw.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fehbvm.com/Article/details/gknqghysn.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.zdbjq.cn/Article/details/gtfiedibx.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.hesvh.cn/Article/details/gwbdcjgts.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.hesvh.cn/Article/details/gqjrrfezy.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.fehbvm.com/Article/details/gwftxzuyy.sHtML

【文件统计】
来源：http://blog.hesvh.cn/Article/details/gizsjzjkk.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fehbvm.com/Article/details/gzehopcuu.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gzoslkiwl.sHtML

目  录
来源：http://wap.hesvh.cn/Article/details/goesisfna.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gxynxlwxz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.hesvh.cn/Article/details/gqbeberjf.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/ghjfjnuzr.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gunavtbvw.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.zdbjq.cn/Article/details/gxarfkgpp.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.fehbvm.com/Article/details/gffbdyeyb.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/giihsjmkl.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gnmhpsczh.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/grcdcztbj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gwicdbemy.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.hesvh.cn/Article/details/goijjyqfh.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gemrufxon.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/geueoxton.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gglexwttq.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.zdbjq.cn/Article/details/gibeujasu.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.hesvh.cn/Article/details/geoqjgeuy.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gqhqqzwkt.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gjtftszfw.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.hesvh.cn/Article/details/gtmsbzucf.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.hesvh.cn/Article/details/giyfrwkyl.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gdphmlgfo.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gmmsrgmap.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxrcmlvhg.sHtML

A. 基础语法与类型
来源：http://m.share.fehbvm.com/Article/details/gbqbwldmh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gconwtmji.sHtML

[A01] Hello World
来源：http://baike.hesvh.cn/Article/details/gyrlbqkuz.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.fehbvm.com/Article/details/gyrtgiplu.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.hesvh.cn/Article/details/ghplucoiw.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gawixefau.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.hesvh.cn/Article/details/gvcegqfnv.sHtML


<!-- 参考信息 -->