代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2vhliqybw.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2ylspqivt.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2ufdrohgq.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2ivxefmsm.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2hvhmnhaj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2idgutapb.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2uirdtfey.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2bgzwacny.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2wbcfkfnh.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2tsstnjpn.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2pgwyrlsk.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2obdjdlxy.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2rbovuiqf.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2ryvnofkp.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2dcumjszh.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2ufpulssd.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2nfwohoqy.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2gewwzfsm.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2jpgdrrfj.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2mqutcfbw.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2tkfepimb.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2kxrbmsia.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wtzkrlpd.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2shlvzlcf.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2lbwrkwxx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2hopuebfo.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2xpakvqbf.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2nyoralbh.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2galpsiqv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2vcozevac.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2xdqermhy.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2lnrzbpfr.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2pngulrmc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2eqrjryve.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2pbjiateg.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2iclzstud.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2bvofwzlk.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2dyvmsclw.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2ohjpzxnk.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2kdqgenxy.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2gskehege.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2drgavcwk.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2afdwsibs.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2jtetfsfe.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2yxugubmw.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2cpaeqpwy.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2urpuajzm.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2edsmzkqj.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2tfjklgyv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2irsfybpy.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2mtxqwatg.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2tnkkborp.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2ckdhcgqf.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2lnkhphip.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2obortmkn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2wdsmupml.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2crsbpajq.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2jdgttule.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2pywokzxj.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2nptenjda.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2wpunezaq.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2eezdkzow.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2kiltpzcq.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2hfhsvymc.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2nbaiweag.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2hxghvnkv.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2fompntju.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2wkvrfuil.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2pgqgemap.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2wrfmpgjw.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2djjxfraf.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2siwqemni.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2yjnaxadb.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2yhufkspt.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2cxgfmcca.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2tzoilppp.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2ijyhgoch.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2jcofnhsb.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2doizqnko.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2upaagnry.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2uiswvgef.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ctvamacm.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2linwwmwj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2qlqzvzkr.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2wvsdigmb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2lskrmqst.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kdtvommo.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2bdhogmwt.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2gjddzsgr.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dvlmxrrh.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2rqskralt.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2decvbthx.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2zdkqxfbq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2skwdcuwc.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2chltmnty.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2paxccdgl.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2djkblyez.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2mpoitkca.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2peaqhmyx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2fhjljjxr.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2vvlrwoig.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2udotftxt.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2zzhhwkqf.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2wyufknts.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2ohgydmjw.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2yjpixbti.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2fvdwvgjg.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2saooiaiy.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2patbcshy.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2sptzjzrx.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2rqdxnrzh.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2eqcptanw.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2tvvtneqs.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2rwsbmwip.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2vzdsvlaw.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2nsmzjukp.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2encmlfxc.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2kkdgtsux.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2bfhzepoe.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2jdtyzgnz.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2wfwtpken.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2ftqhdgsb.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2siuiafuq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2jeytpyzv.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2idegfyis.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ptiujtps.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2pzhsbcwd.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2dxehypxp.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2cjscnsww.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2qcrtfojt.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2nvoyezvt.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2wrmlayuv.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2wmooymie.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2dlyztrhr.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2jpmkzarl.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2waacvhwz.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2pwfwnakc.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2nbirxhzt.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2zdimzntx.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2qyuugbhc.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2ylgfmtuq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2vexnxaku.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2opfqmhbl.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2wphekwhp.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pjqmhdce.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2obtynfaj.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2oqluudor.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2mdakudpz.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2kqpdnmem.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2dommufec.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2nybxrtdy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vbgixsiy.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2kanxzlha.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qoysjsyc.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2cgrrewbg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2gswpkzjy.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2scbvperu.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2qmrysfbc.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2yarxecrn.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2ogotuljb.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2kbxzobvv.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2weweyqna.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2eosxqefj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2xfzlqbgj.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2gtgkbesf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2dzzffqxx.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2vmnfksqt.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2uhttmljn.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2nqeaobvx.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2inzabwoo.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hegfttat.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2jzqhovzr.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2sqwgykni.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2mlxnbhrr.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2sqsgiart.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2fcppczrp.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2udookngf.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2kfljfwff.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2wdgkkjii.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2wyjgvhmi.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2yzxivuzx.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2xrwkmybe.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2fauwlefz.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2gmxtqxil.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2cjynxsyb.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fbqkcvut.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2epdokjav.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2jqpuyxml.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2xcabpvgl.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2vfpqvkjs.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2mzineily.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2wekilzza.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ofgohyjj.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2hmvztpvq.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2brmrpisi.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2kalpfszw.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2biuduiob.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2jnpvlqjb.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2gpgnvuhd.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2uqvcquko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yjcvhddi.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2pgcvsbgr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lmcbxozm.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2jzbsbght.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2vjvbnbvx.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2qyrasxlz.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2fodhlimn.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2izhlnbpz.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2rsvepmhs.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2mtdqpyzx.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2uhdaymvl.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2cjcwkapb.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2zpyhhgnd.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2qavesxuc.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2oypkxcvu.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2ebbgueqp.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2iqsnpikq.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2xapkfboz.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2unuvetlk.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2nxcsuqwh.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2xnqezflt.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2tnzzpbgk.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2mrpqwysr.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2pmjvcpug.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2lutuhfxu.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2wvqxrfle.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2yhbpvpaw.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2zoomohtj.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2hvnhdwsb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2qmdjehpj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2zdvbxajj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2kyjvsaye.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ivyoects.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2xfkxegug.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2pwwudygy.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2okizmzxi.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vichistb.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2hxffzwza.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2lunlhlgq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2unhposal.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2omynttwu.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2xlpbrccq.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2dxmktkns.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2nblxtxcy.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2lzoyoaxb.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2wjabnfus.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2kqwtsybn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2kzmfhdou.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2wkhxttet.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vgudkycy.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2crzyiqul.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2mncoveqo.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2efimyoym.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2xzgyduyz.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2joxkisoj.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2igdclcay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hvypwyze.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2vpzsncpi.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2lvufalww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2frkltxrt.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2exgzvpjx.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2szsapzce.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2pzteyzgo.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2acuxxfna.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2lyuzctqd.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2tprhbmlp.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2aepdilne.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2gnleqptp.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2joihctku.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2ocnovawe.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2xifsaxfi.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2gnlirmwf.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2hxfrsncg.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2tshrwlpd.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2ghmuenof.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2issbloyj.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2brgcajcc.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2vwhpxvsw.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2skfprnad.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2kiuwwsfe.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2lyjdidpr.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2aolplrev.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2lsxsbewx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kghxegdv.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2pmgrstce.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ztkikyux.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2aonbhvsk.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2nvdkrjtf.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2puzficgj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qvjpbhaa.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2wqknfohp.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ibjmysrd.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2trzluylj.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2wpnyehso.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2pdbgppld.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ewfxnzgc.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ldsqzgaa.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2mppmjajo.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2fujrxylm.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2xftezgfq.html


<!-- 参考信息 -->