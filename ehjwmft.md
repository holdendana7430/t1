代发 wailian999

[U27] Py：异步 HTTP
来源：http://m.share.fehbvm.com/Article/details/gyggayxxb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fehbvm.com/Article/details/glujmnonq.sHtML

[U28] Py：类型别名
来源：http://3g.zdbjq.cn/Article/details/gycrxzrnr.sHtML

UserId = int
来源：http://baike.fehbvm.com/Article/details/glhubbkjv.sHtML

[U29] Py：属性校验
来源：http://mobile.hesvh.cn/Article/details/grnvcgmyb.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/gtfftsipt.sHtML

[U30] Py：数据类
来源：http://3g.fehbvm.com/Article/details/geyquaotj.sHtML

@dataclass(slots=True)
来源：http://read.share.fehbvm.com/Article/details/gsdxzsfwz.sHtML

[U31] Py：单测
来源：http://mobile.fehbvm.com/Article/details/gqagbhwpy.sHtML

python -m pytest -q
来源：http://www.m.share.hesvh.cn/Article/details/gmyefbajv.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fehbvm.com/Article/details/gxksjhjnb.sHtML

ruff format . && ruff check --fix .
来源：http://baike.hesvh.cn/Article/details/ggmxegyjw.sHtML

[U33] Py：打包发布
来源：http://mobile.fehbvm.com/Article/details/gyankungq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.zdbjq.cn/Article/details/ghyehhnfn.sHtML

[U34] Py：判断编码
来源：http://blog.fehbvm.com/Article/details/gvnryslja.sHtML

chardet.detect(raw)
来源：http://mobile.zdbjq.cn/Article/details/gfuqnahxk.sHtML

[U35] Py：发送邮件
来源：http://wap.fehbvm.com/Article/details/glialmgrg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.zdbjq.cn/Article/details/gqorwdfvl.sHtML

[U36] Py：定时任务
来源：http://3g.fehbvm.com/Article/details/gvpcnqwkk.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.hesvh.cn/Article/details/gllomvwpt.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.hesvh.cn/Article/details/gajixoboe.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fehbvm.com/Article/details/gtxhvfuzd.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.hesvh.cn/Article/details/ggacfixtw.sHtML

Path(__file__).resolve().parent
来源：http://wap.zdbjq.cn/Article/details/gjqbyzpkn.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.hesvh.cn/Article/details/goqjkqkyn.sHtML

sys.stdout.isatty()
来源：http://m.share.fehbvm.com/Article/details/gukbgbkcq.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.zdbjq.cn/Article/details/gxtgasfvu.sHtML

print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gpevlshyt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.zdbjq.cn/Article/details/gmpdrmmxj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fehbvm.com/Article/details/ggzjlzgck.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fehbvm.com/Article/details/geezhqsim.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.zdbjq.cn/Article/details/grvglgvsd.sHtML

[U43] PHP：声明命名空间
来源：http://3g.zdbjq.cn/Article/details/gbnfgthzo.sHtML

namespace App\Http;
来源：http://www.blog.zdbjq.cn/Article/details/gegojucmk.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fehbvm.com/Article/details/ggopqxpho.sHtML

declare(strict_types=1);
来源：http://wap.fehbvm.com/Article/details/gbdftynjg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.zdbjq.cn/Article/details/gmyvsorrm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/ghvoituak.sHtML

[U46] PHP：可空类型
来源：http://blog.fehbvm.com/Article/details/goosrsour.sHtML

?string $name = null
来源：http://wap.zdbjq.cn/Article/details/gbgxspwef.sHtML

[U47] PHP：联合类型
来源：http://m.share.hesvh.cn/Article/details/gautcpkpa.sHtML

int|string $id
来源：http://mobile.zdbjq.cn/Article/details/gdsmqzrax.sHtML

[U48] PHP：纯枚举
来源：http://read.share.zdbjq.cn/Article/details/gnoeycpva.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fehbvm.com/Article/details/gdihcasso.sHtML

[U49] PHP：只读属性
来源：http://m.share.zdbjq.cn/Article/details/gjpfuwrzs.sHtML

public readonly string $name
来源：http://mobile.zdbjq.cn/Article/details/grnmitthj.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fehbvm.com/Article/details/glnijeoxl.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.hesvh.cn/Article/details/gdzyvuxrg.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fehbvm.com/Article/details/gwpgfmehh.sHtML

[$a, $b] = $arr;
来源：http://blog.hesvh.cn/Article/details/gaxitmlmu.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gmodrjzst.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gczglnsyf.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fehbvm.com/Article/details/gizjlywfh.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fehbvm.com/Article/details/gmgcedrwo.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fehbvm.com/Article/details/gibvedxjz.sHtML

$obj?->method()
来源：http://read.share.fehbvm.com/Article/details/gwvmecqyc.sHtML

[U55] PHP：match 表达式
来源：http://www.share.zdbjq.cn/Article/details/gsmoyllwy.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fehbvm.com/Article/details/gdzykupzj.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.hesvh.cn/Article/details/gqmmlqzzg.sHtML

f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gwnchrjvj.sHtML

[U57] PHP：字符串插值
来源：http://wap.fehbvm.com/Article/details/gbnyhucft.sHtML

"值: {$a}"
来源：http://baike.hesvh.cn/Article/details/gnyjazodb.sHtML

[U58] PHP：数组三件套
来源：http://wap.fehbvm.com/Article/details/ghpchmkeq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.hesvh.cn/Article/details/gndiydmek.sHtML

[U59] PHP：自定义排序
来源：http://www.share.zdbjq.cn/Article/details/gqhndquje.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gnomsbaxv.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.hesvh.cn/Article/details/gajsvskwx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.zdbjq.cn/Article/details/guenleoqv.sHtML

[U61] PHP：正则
来源：http://3g.fehbvm.com/Article/details/gmoyceuha.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/gspfhicai.sHtML

[U62] PHP：日期对象
来源：http://mobile.hesvh.cn/Article/details/gfzmaqgmj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.hesvh.cn/Article/details/gxpzjdizx.sHtML

[U63] PHP：文件读写
来源：http://3g.fehbvm.com/Article/details/geryuvueu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.zdbjq.cn/Article/details/gdbruvjic.sHtML

[U64] PHP：目录遍历
来源：http://blog.fehbvm.com/Article/details/gqvntmmwr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fehbvm.com/Article/details/ghwkvvjcm.sHtML

[U65] PHP：会话
来源：http://www.blog.fehbvm.com/Article/details/gpmdkrycd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gmvkqmyrw.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fehbvm.com/Article/details/glpdsslqi.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.hesvh.cn/Article/details/gotrgfkpt.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/gmjycroyk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.zdbjq.cn/Article/details/gssftajxn.sHtML

[U68] PHP：PDO 连接
来源：http://wap.hesvh.cn/Article/details/gcqeomfgl.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.zdbjq.cn/Article/details/gathdcuns.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fehbvm.com/Article/details/gsivxghdn.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fehbvm.com/Article/details/gxqxzondy.sHtML

[U70] PHP：PDO 事务
来源：http://wap.zdbjq.cn/Article/details/gpgzoanva.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fehbvm.com/Article/details/gfguaupvs.sHtML

[U71] PHP：抛出异常
来源：http://blog.hesvh.cn/Article/details/giogiocka.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.hesvh.cn/Article/details/ghrgbmaew.sHtML

[U72] PHP：写错误日志
来源：http://baike.fehbvm.com/Article/details/gqhfwsqsp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.hesvh.cn/Article/details/gmclyhiqo.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.zdbjq.cn/Article/details/ggdeslbxz.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.zdbjq.cn/Article/details/gjtlfcprn.sHtML

[U74] PHP：读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gaixduwiw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.hesvh.cn/Article/details/gzfagopgd.sHtML

[U75] PHP：依赖注入
来源：http://m.share.hesvh.cn/Article/details/gddsjqlsm.sHtML

composer require psr/container
来源：http://read.share.fehbvm.com/Article/details/gjoapjrfo.sHtML

[U76] PHP：简单路由
来源：http://www.share.fehbvm.com/Article/details/gdwnlsldn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fehbvm.com/Article/details/gkavucdrf.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fehbvm.com/Article/details/gdoynppdc.sHtML

composer require twig/twig
来源：http://www.m.share.zdbjq.cn/Article/details/gnmoupmke.sHtML

[U78] PHP：单元测试
来源：http://3g.fehbvm.com/Article/details/gftzaaude.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.hesvh.cn/Article/details/gqemojfyq.sHtML

[U79] PHP：静态分析
来源：http://www.blog.zdbjq.cn/Article/details/geduboimu.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.zdbjq.cn/Article/details/gndvsbwmg.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fehbvm.com/Article/details/gpjamosen.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.hesvh.cn/Article/details/gwawccrap.sHtML

[U81] JS：初始化项目
来源：http://read.share.fehbvm.com/Article/details/gqqtcmxdl.sHtML

npm init -y;  npm i express
来源：http://baike.hesvh.cn/Article/details/gnlebxznw.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fehbvm.com/Article/details/gvufhdcfd.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.zdbjq.cn/Article/details/gouaksirv.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fehbvm.com/Article/details/gfioelyjz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gkrgnvpor.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.zdbjq.cn/Article/details/grcrewoeo.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fehbvm.com/Article/details/gpdlpmqjx.sHtML

[U85] JS：可选链
来源：http://www.blog.zdbjq.cn/Article/details/gkmnfrasw.sHtML

a?.b?.c
来源：http://wap.fehbvm.com/Article/details/gixoygzav.sHtML

[U86] JS：空值合并
来源：http://m.share.fehbvm.com/Article/details/gjjmiwpjv.sHtML

a ?? b
来源：http://m.share.zdbjq.cn/Article/details/gxzpdtirv.sHtML

[U87] JS：解构默认值
来源：http://www.share.zdbjq.cn/Article/details/ggdfhxzke.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.hesvh.cn/Article/details/gkgfiucqv.sHtML

[U88] JS：对象展开合并
来源：http://wap.zdbjq.cn/Article/details/gxtcuwokh.sHtML

{ ...a, ...b }
来源：http://www.m.share.zdbjq.cn/Article/details/gvciszuvj.sHtML

[U89] JS：数组去重
来源：http://blog.hesvh.cn/Article/details/gapxrzoct.sHtML

[...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gztnkdrde.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fehbvm.com/Article/details/gmaeqsbws.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gsyxtfnzt.sHtML

[U91] JS：对象键值遍历
来源：http://3g.zdbjq.cn/Article/details/glrtakxcx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fehbvm.com/Article/details/gqsrxrwkv.sHtML

[U92] JS：深拷贝
来源：http://wap.hesvh.cn/Article/details/gnhttoyzo.sHtML

structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gqxxrgmwe.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gdxnufarp.sHtML

`共 ${n} 条`
来源：http://www.blog.fehbvm.com/Article/details/gqyubpzcc.sHtML

[U94] JS：箭头函数
来源：http://m.share.fehbvm.com/Article/details/grufiocln.sHtML

const double = x => x * 2;
来源：http://wap.hesvh.cn/Article/details/gqlgbewqc.sHtML

[U95] JS：Promise 包装
来源：http://read.share.hesvh.cn/Article/details/gkgiulesf.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fehbvm.com/Article/details/gisixyumv.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.hesvh.cn/Article/details/gbmwvcmvl.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gggztdlvu.sHtML

[U97] JS：并发请求
来源：http://blog.zdbjq.cn/Article/details/gxqozvbfv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gfzjpzowy.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.zdbjq.cn/Article/details/gctbunxgz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fehbvm.com/Article/details/gjvefqmrt.sHtML

[U99] JS：事件监听
来源：http://3g.fehbvm.com/Article/details/gtakveidy.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.hesvh.cn/Article/details/gggbaknyz.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/gaorpwemg.sHtML

document.querySelector(".item")
来源：http://wap.hesvh.cn/Article/details/giwiplfgq.sHtML

[U101] JS：classList 操作
来源：http://3g.fehbvm.com/Article/details/gicmpraxp.sHtML

el.classList.toggle("active")
来源：http://baike.fehbvm.com/Article/details/grhmehoqg.sHtML

[U102] JS：本地存储
来源：http://wap.hesvh.cn/Article/details/gfzkszzzd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.zdbjq.cn/Article/details/gptlmdhdw.sHtML

[U103] JS：定时器
来源：http://wap.zdbjq.cn/Article/details/gbsryzdmg.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fehbvm.com/Article/details/gdevkwlnl.sHtML

[U104] JS：防抖
来源：http://3g.fehbvm.com/Article/details/gtwtricsp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/grtydzuny.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/gfndsucfz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.zdbjq.cn/Article/details/ghimkxchv.sHtML

[U106] JS：日期格式化
来源：http://m.share.hesvh.cn/Article/details/gygqaonhe.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fehbvm.com/Article/details/gulfnpmot.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fehbvm.com/Article/details/grrbenlcg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/ggiwicekx.sHtML

[U108] JS：随机整数
来源：http://baike.hesvh.cn/Article/details/gpshvktbs.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.zdbjq.cn/Article/details/gsvchscjb.sHtML

[U109] JS：数组分组
来源：http://www.blog.zdbjq.cn/Article/details/getgtrlzi.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/ggmxakcym.sHtML

[U110] JS：数组分块
来源：http://m.share.zdbjq.cn/Article/details/gyvzgavay.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fehbvm.com/Article/details/gfkxnjsvx.sHtML

[U111] JS：对象转 Map
来源：http://3g.hesvh.cn/Article/details/gsufxossk.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/ggsyacmkm.sHtML

[U112] JS：字符串补位
来源：http://blog.hesvh.cn/Article/details/gedspmiow.sHtML

"7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/glkyeboop.sHtML

[U113] JS：正则替换全部
来源：http://baike.fehbvm.com/Article/details/giwretovc.sHtML

s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gfztonohj.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.hesvh.cn/Article/details/gzkxlkujs.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gwohlrdyr.sHtML

[U115] JS：生成 UUID
来源：http://read.share.hesvh.cn/Article/details/ghnvtuxrq.sHtML

crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gonlbhgde.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.hesvh.cn/Article/details/gycxtavoo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.zdbjq.cn/Article/details/ggowwykvq.sHtML

[U117] JS：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gojqsrgqn.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.hesvh.cn/Article/details/gycrcrgoq.sHtML

[U118] JS：开发服务器
来源：http://blog.zdbjq.cn/Article/details/gzrjiyezl.sHtML

npm i -D vite;  npx vite
来源：http://mobile.zdbjq.cn/Article/details/gjaqgmxsf.sHtML

[U119] JS：生产构建
来源：http://wap.zdbjq.cn/Article/details/gyrzlhgqx.sHtML

npx vite build
来源：http://mobile.fehbvm.com/Article/details/gfrhqkstv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.zdbjq.cn/Article/details/gwznvqvlh.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.zdbjq.cn/Article/details/gadssqmqs.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcvybchvl.sHtML

统计汇总
来源：http://www.share.zdbjq.cn/Article/details/gwmnzfxur.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gyfposzwp.sHtML

按语言统计（条）：
来源：http://mobile.zdbjq.cn/Article/details/gwilxmwrg.sHtML

Python ......... 252
来源：http://mobile.fehbvm.com/Article/details/gxgbpbdmo.sHtML

PHP ............ 252
来源：http://mobile.hesvh.cn/Article/details/gstuvusau.sHtML

JavaScript ..... 252
来源：http://www.blog.zdbjq.cn/Article/details/gzhltndcb.sHtML

TypeScript ..... 212
来源：http://baike.zdbjq.cn/Article/details/ghwafhnrc.sHtML

Java ........... 212
来源：http://wap.zdbjq.cn/Article/details/gyqfthshc.sHtML

Go ............. 212
来源：http://blog.fehbvm.com/Article/details/grkkfaxhx.sHtML

Ruby ........... 212
来源：http://wap.fehbvm.com/Article/details/gzhnlwamc.sHtML

C# ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/gbaguifis.sHtML

C .............. 30
来源：http://www.m.share.hesvh.cn/Article/details/gkluznxaq.sHtML

C++ ............ 30
来源：http://read.share.hesvh.cn/Article/details/gkbomlasx.sHtML

SQL ............ 90
来源：http://read.share.fehbvm.com/Article/details/gbotholch.sHtML

Bash ........... 80
来源：http://mobile.fehbvm.com/Article/details/gcuiabeqp.sHtML

Kotlin ......... 15
来源：http://wap.hesvh.cn/Article/details/gyeujdnkg.sHtML

Swift .......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/ggawjztzp.sHtML

Lua ............ 10
来源：http://www.blog.zdbjq.cn/Article/details/gpiurpqfc.sHtML

Perl ........... 10
来源：http://www.m.share.hesvh.cn/Article/details/gmkkbedbx.sHtML

Scala .......... 10
来源：http://wap.zdbjq.cn/Article/details/gelloyfgd.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/ghvrhemgw.sHtML

合计 ........... 2106 条
来源：http://blog.zdbjq.cn/Article/details/gsidcqkfu.sHtML

按章节统计：
来源：http://mobile.fehbvm.com/Article/details/geqsdeygk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gkxhgsdiy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gpqgmgdod.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gmkmpdlul.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gpjiuawbq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.hesvh.cn/Article/details/gnfqhvyxo.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/gjsbmyxax.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gctvygdqt.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gtoepofvf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gccwfdwkv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gngoujoyn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gacovxjrc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gwnwavajz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gflkggbwk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gsvgjeokc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.zdbjq.cn/Article/details/gmsvsibcf.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gzexbfstw.sHtML

Q SQL 专题                              90
来源：http://baike.zdbjq.cn/Article/details/gytjmfcjk.sHtML

R Bash 专题                             80
来源：http://read.share.hesvh.cn/Article/details/glwzhnccf.sHtML

S C / C++ 专题                          60
来源：http://baike.zdbjq.cn/Article/details/ghoerlziy.sHtML

T 其他语言补充                          60
来源：http://baike.hesvh.cn/Article/details/gnzjthxpc.sHtML

U 高频实用片段                         120
来源：http://mobile.zdbjq.cn/Article/details/glgucxyes.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gguonjppk.sHtML

合计                                  2106 条
来源：http://www.share.fehbvm.com/Article/details/gognvmijb.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gnbohrljq.sHtML

使用提醒
来源：http://www.share.fehbvm.com/Article/details/gpqfiitbw.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gtdiwffqh.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.zdbjq.cn/Article/details/gmzngtapg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.zdbjq.cn/Article/details/gztpapnqs.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.hesvh.cn/Article/details/gcktiuxhs.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.fehbvm.com/Article/details/guaujeilx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.hesvh.cn/Article/details/gjxdbjzah.sHtML

—— 文件结束 ——
来源：http://read.share.fehbvm.com/Article/details/grypqijwt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdnlnbnfh.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.zdbjq.cn/Article/details/gahaqgasn.sHtML

Common Programming Examples Cheat Book
来源：http://3g.hesvh.cn/Article/details/gniooiyyf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grhdaotmx.sHtML

【收录内容】
来源：http://www.blog.fehbvm.com/Article/details/ghaftnhik.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fehbvm.com/Article/details/ggdwqhvov.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.zdbjq.cn/Article/details/gghlkgntu.sHtML

SQL · Bash · C · C++
来源：http://mobile.hesvh.cn/Article/details/ghnwauzkp.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.zdbjq.cn/Article/details/gmpyelxta.sHtML

【使用说明】
来源：http://read.share.fehbvm.com/Article/details/ggpljcycn.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.zdbjq.cn/Article/details/gxyvkhadq.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fehbvm.com/Article/details/gxdbpcaud.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.zdbjq.cn/Article/details/gudwdrxaw.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.hesvh.cn/Article/details/gxmrnhsum.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fehbvm.com/Article/details/gjdyuzcts.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fehbvm.com/Article/details/gpzjoxhgm.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.zdbjq.cn/Article/details/glyfexdhp.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.zdbjq.cn/Article/details/gotvgfomg.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.hesvh.cn/Article/details/gischqadl.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.zdbjq.cn/Article/details/gaxhcqvyr.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.hesvh.cn/Article/details/glzrqyjoi.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.hesvh.cn/Article/details/gjigqhnej.sHtML

【文件统计】
来源：http://m.share.hesvh.cn/Article/details/gnpwmrtqo.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.zdbjq.cn/Article/details/gmhpxvjgx.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/guoqqoynv.sHtML

目  录
来源：http://m.share.hesvh.cn/Article/details/gtnsvwkgj.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/girwtnakn.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gbiwaqjyk.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gtbjpswjr.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gtcosvxzw.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.zdbjq.cn/Article/details/gjcuneqcw.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.hesvh.cn/Article/details/gfqnsxfmi.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gfworslfk.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gboczkrkm.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gkgwodbyj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gktvxsnyb.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gtcguvefs.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gljlrvfgu.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gylgtkksv.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gfrwdfqif.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/gpdoiipmq.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.fehbvm.com/Article/details/gfcasoljd.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/ggjmadxqc.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.hesvh.cn/Article/details/gvtfoupkb.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gecjcirrj.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.fehbvm.com/Article/details/glrpaumec.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gsgqzxrjy.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gtasbcmzi.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtbqtuoev.sHtML

A. 基础语法与类型
来源：http://wap.hesvh.cn/Article/details/gmlyrjyzw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/goudowawi.sHtML

[A01] Hello World
来源：http://wap.fehbvm.com/Article/details/gbyfbfera.sHtML

Py:   print("Hello, World!")
来源：http://m.share.fehbvm.com/Article/details/gqhkjuijk.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.fehbvm.com/Article/details/gyqfuwudx.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gtzpnyjkt.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.hesvh.cn/Article/details/gzlhqaupz.sHtML


<!-- 参考信息 -->