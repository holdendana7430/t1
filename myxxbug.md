代发 wailian999

[U27] Py：异步 HTTP
来源：http://www.blog.hesvh.cn/Article/details/gmxgstrku.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.zdbjq.cn/Article/details/gcafhppqa.sHtML

[U28] Py：类型别名
来源：http://www.share.zdbjq.cn/Article/details/ghlzcogqf.sHtML

UserId = int
来源：http://wap.hesvh.cn/Article/details/gtstqegdh.sHtML

[U29] Py：属性校验
来源：http://m.share.fehbvm.com/Article/details/gmdrghgad.sHtML

@property 与 @x.setter 配合
来源：http://mobile.zdbjq.cn/Article/details/gidwdwict.sHtML

[U30] Py：数据类
来源：http://www.share.hesvh.cn/Article/details/gfvfcmxyp.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fehbvm.com/Article/details/ghubrppfc.sHtML

[U31] Py：单测
来源：http://www.share.zdbjq.cn/Article/details/gocoafkaj.sHtML

python -m pytest -q
来源：http://www.blog.fehbvm.com/Article/details/ghhtrijbq.sHtML

[U32] Py：代码格式化
来源：http://m.share.zdbjq.cn/Article/details/gdoyhznua.sHtML

ruff format . && ruff check --fix .
来源：http://baike.hesvh.cn/Article/details/gbhikawzg.sHtML

[U33] Py：打包发布
来源：http://blog.hesvh.cn/Article/details/grrfpvvlh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.zdbjq.cn/Article/details/gbufsaebl.sHtML

[U34] Py：判断编码
来源：http://www.blog.hesvh.cn/Article/details/gzpfotttq.sHtML

chardet.detect(raw)
来源：http://www.m.share.fehbvm.com/Article/details/geopnmedn.sHtML

[U35] Py：发送邮件
来源：http://blog.fehbvm.com/Article/details/gbvlpzzdy.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.hesvh.cn/Article/details/gelbapoob.sHtML

[U36] Py：定时任务
来源：http://baike.fehbvm.com/Article/details/gbxojtkfl.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.zdbjq.cn/Article/details/gshptkvsb.sHtML

[U37] Py：读写 Excel
来源：http://baike.fehbvm.com/Article/details/gdwrsnikg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/grbvlnpad.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fehbvm.com/Article/details/geznkfafz.sHtML

Path(__file__).resolve().parent
来源：http://m.share.hesvh.cn/Article/details/gbqanmeik.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fehbvm.com/Article/details/ggptayikz.sHtML

sys.stdout.isatty()
来源：http://www.blog.zdbjq.cn/Article/details/gpcpygxri.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fehbvm.com/Article/details/gbgrdthss.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/goaiagdyj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.hesvh.cn/Article/details/goldnosoc.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.zdbjq.cn/Article/details/gpeiytngj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fehbvm.com/Article/details/gzxlsnecn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.hesvh.cn/Article/details/gdbrqybek.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fehbvm.com/Article/details/gthrbzmym.sHtML

namespace App\Http;
来源：http://3g.hesvh.cn/Article/details/gaxdsbkqc.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.zdbjq.cn/Article/details/gyuidsqhr.sHtML

declare(strict_types=1);
来源：http://baike.zdbjq.cn/Article/details/gmicfopcb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.hesvh.cn/Article/details/gsvqiqjfk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/geghnbuaf.sHtML

[U46] PHP：可空类型
来源：http://www.share.zdbjq.cn/Article/details/gyrtwdgiv.sHtML

?string $name = null
来源：http://read.share.zdbjq.cn/Article/details/gpqqbgjdv.sHtML

[U47] PHP：联合类型
来源：http://www.share.fehbvm.com/Article/details/gcrkszhsv.sHtML

int|string $id
来源：http://blog.fehbvm.com/Article/details/gqzccbdgd.sHtML

[U48] PHP：纯枚举
来源：http://blog.hesvh.cn/Article/details/gvypyistu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fehbvm.com/Article/details/gzbzxyxzz.sHtML

[U49] PHP：只读属性
来源：http://www.share.fehbvm.com/Article/details/ggpjetydc.sHtML

public readonly string $name
来源：http://3g.fehbvm.com/Article/details/govdtecqs.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fehbvm.com/Article/details/gocbpvavs.sHtML

public function __construct(private int $id) {}
来源：http://m.share.zdbjq.cn/Article/details/gcvkevjok.sHtML

[U51] PHP：数组解构
来源：http://baike.hesvh.cn/Article/details/gnhsxmado.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.hesvh.cn/Article/details/gjvjqrbyw.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gpxburorp.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fehbvm.com/Article/details/gkuppekga.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.zdbjq.cn/Article/details/gvjbrgmnf.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.zdbjq.cn/Article/details/gxibohjap.sHtML

[U54] PHP：空安全调用
来源：http://baike.fehbvm.com/Article/details/gtatfgwag.sHtML

$obj?->method()
来源：http://www.share.fehbvm.com/Article/details/gzpnmwctz.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.hesvh.cn/Article/details/gxkfcjjwp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fehbvm.com/Article/details/gjdrxtzvn.sHtML

[U56] PHP：命名参数
来源：http://baike.hesvh.cn/Article/details/gyxklywfh.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gjceoydai.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gsbjzikhx.sHtML

"值: {$a}"
来源：http://www.m.share.zdbjq.cn/Article/details/gwszrfjyl.sHtML

[U58] PHP：数组三件套
来源：http://3g.zdbjq.cn/Article/details/gkvutaviu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fehbvm.com/Article/details/gvzcknorm.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fehbvm.com/Article/details/gxxemjmes.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gnvqrcpvi.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.zdbjq.cn/Article/details/glcsolfxz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.hesvh.cn/Article/details/gzhtqdmrx.sHtML

[U61] PHP：正则
来源：http://wap.fehbvm.com/Article/details/gkxlkbewk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/ggbmbciot.sHtML

[U62] PHP：日期对象
来源：http://3g.zdbjq.cn/Article/details/gtsvsbkru.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.hesvh.cn/Article/details/gpitzmwta.sHtML

[U63] PHP：文件读写
来源：http://read.share.fehbvm.com/Article/details/grqoolalz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.hesvh.cn/Article/details/gpmxjsiby.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.zdbjq.cn/Article/details/gpojvbxms.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.hesvh.cn/Article/details/gziflmusr.sHtML

[U65] PHP：会话
来源：http://wap.fehbvm.com/Article/details/gpyqmryqp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gvibvxwgb.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.hesvh.cn/Article/details/gzzzodaoc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.hesvh.cn/Article/details/gyfkcavtq.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.zdbjq.cn/Article/details/gwmrynlcs.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.hesvh.cn/Article/details/gqapqwmln.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fehbvm.com/Article/details/gycmgcgfl.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fehbvm.com/Article/details/goyvjglic.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.hesvh.cn/Article/details/gyvfsfnjp.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fehbvm.com/Article/details/gyopiprqy.sHtML

[U70] PHP：PDO 事务
来源：http://baike.zdbjq.cn/Article/details/gtqdjccpj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.zdbjq.cn/Article/details/gobndhuav.sHtML

[U71] PHP：抛出异常
来源：http://blog.fehbvm.com/Article/details/gxydnjyvw.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/gxplsqrhi.sHtML

[U72] PHP：写错误日志
来源：http://mobile.hesvh.cn/Article/details/gkzqlkjaz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.hesvh.cn/Article/details/gmorjbixf.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.hesvh.cn/Article/details/gzntrazbu.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.hesvh.cn/Article/details/gpxujfkyb.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gesnedaeo.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fehbvm.com/Article/details/gkcnfujdr.sHtML

[U75] PHP：依赖注入
来源：http://m.share.hesvh.cn/Article/details/gpqoiqvay.sHtML

composer require psr/container
来源：http://www.share.zdbjq.cn/Article/details/gucngeaaa.sHtML

[U76] PHP：简单路由
来源：http://mobile.fehbvm.com/Article/details/gszmuboaf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.hesvh.cn/Article/details/gvlcxvocq.sHtML

[U77] PHP：模板渲染
来源：http://mobile.zdbjq.cn/Article/details/grjhgdcoz.sHtML

composer require twig/twig
来源：http://blog.fehbvm.com/Article/details/gihfplrmv.sHtML

[U78] PHP：单元测试
来源：http://blog.fehbvm.com/Article/details/guaopjggs.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fehbvm.com/Article/details/ghvynvqfe.sHtML

[U79] PHP：静态分析
来源：http://www.share.fehbvm.com/Article/details/gqqhmktgu.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fehbvm.com/Article/details/gdfyceuph.sHtML

[U80] PHP：代码规范修复
来源：http://blog.zdbjq.cn/Article/details/gioxopliq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fehbvm.com/Article/details/gbmpkuqrn.sHtML

[U81] JS：初始化项目
来源：http://mobile.zdbjq.cn/Article/details/glmzakuzj.sHtML

npm init -y;  npm i express
来源：http://www.blog.zdbjq.cn/Article/details/gqyfzfvme.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fehbvm.com/Article/details/gokxzlsiy.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.zdbjq.cn/Article/details/gmpoberul.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.hesvh.cn/Article/details/gygzenaoh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gkjewakho.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.hesvh.cn/Article/details/gthltnarg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fehbvm.com/Article/details/gmtpbdvgu.sHtML

[U85] JS：可选链
来源：http://www.blog.fehbvm.com/Article/details/ghjcbhraa.sHtML

a?.b?.c
来源：http://blog.fehbvm.com/Article/details/gmelevshe.sHtML

[U86] JS：空值合并
来源：http://www.blog.zdbjq.cn/Article/details/gjusgdsfc.sHtML

a ?? b
来源：http://read.share.fehbvm.com/Article/details/gwgoblila.sHtML

[U87] JS：解构默认值
来源：http://www.share.hesvh.cn/Article/details/gpdqtfvnr.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.hesvh.cn/Article/details/gghyofepr.sHtML

[U88] JS：对象展开合并
来源：http://www.share.hesvh.cn/Article/details/gmwznvqdh.sHtML

{ ...a, ...b }
来源：http://wap.hesvh.cn/Article/details/gaconnshz.sHtML

[U89] JS：数组去重
来源：http://blog.fehbvm.com/Article/details/gbnwksxgm.sHtML

[...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gaoccihai.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.hesvh.cn/Article/details/gvlxuohde.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gwzckssra.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gjezfyfse.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.hesvh.cn/Article/details/ganxxrisu.sHtML

[U92] JS：深拷贝
来源：http://read.share.hesvh.cn/Article/details/gereginto.sHtML

structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/ghgqbxnup.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gyaimlspe.sHtML

`共 ${n} 条`
来源：http://3g.hesvh.cn/Article/details/ggfzryxza.sHtML

[U94] JS：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gbkplrefj.sHtML

const double = x => x * 2;
来源：http://read.share.zdbjq.cn/Article/details/gfonurpcx.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fehbvm.com/Article/details/gmpdkiyby.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fehbvm.com/Article/details/gnfozhnbf.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fehbvm.com/Article/details/gwdsceveh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gycojktxu.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/gyhmjjkxr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gfuccnwaz.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fehbvm.com/Article/details/gjoqqkyls.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.zdbjq.cn/Article/details/geaxusoqq.sHtML

[U99] JS：事件监听
来源：http://www.blog.zdbjq.cn/Article/details/gwuwytxaa.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fehbvm.com/Article/details/gihcdbkoq.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fehbvm.com/Article/details/gqqawdkij.sHtML

document.querySelector(".item")
来源：http://baike.fehbvm.com/Article/details/gxgjcjxxu.sHtML

[U101] JS：classList 操作
来源：http://wap.zdbjq.cn/Article/details/gedadwytj.sHtML

el.classList.toggle("active")
来源：http://3g.fehbvm.com/Article/details/gnlkfnpfy.sHtML

[U102] JS：本地存储
来源：http://wap.fehbvm.com/Article/details/gargrxwpl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.hesvh.cn/Article/details/geygqkzby.sHtML

[U103] JS：定时器
来源：http://www.blog.fehbvm.com/Article/details/gmkodtkbs.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.hesvh.cn/Article/details/gccomiymj.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/gmxyjbtvl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gmbcfohfx.sHtML

[U105] JS：节流
来源：http://blog.hesvh.cn/Article/details/gdlgmpheb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.hesvh.cn/Article/details/gwqquptye.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gnncdvzza.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.zdbjq.cn/Article/details/gijgeuhhp.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gwfvclcrq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fehbvm.com/Article/details/gjbwtdnit.sHtML

[U108] JS：随机整数
来源：http://3g.hesvh.cn/Article/details/gjhbjxbsf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.hesvh.cn/Article/details/gvrwgfgxa.sHtML

[U109] JS：数组分组
来源：http://baike.fehbvm.com/Article/details/gqcfsbmaa.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/ghddjekbt.sHtML

[U110] JS：数组分块
来源：http://mobile.zdbjq.cn/Article/details/govrmultp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fehbvm.com/Article/details/gymeworph.sHtML

[U111] JS：对象转 Map
来源：http://3g.fehbvm.com/Article/details/gqanptxes.sHtML

new Map(Object.entries(obj))
来源：http://m.share.zdbjq.cn/Article/details/grcgadkhh.sHtML

[U112] JS：字符串补位
来源：http://3g.zdbjq.cn/Article/details/gzhihzann.sHtML

"7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gclpcuitj.sHtML

[U113] JS：正则替换全部
来源：http://3g.fehbvm.com/Article/details/gyhyzvxie.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gofzsnjrz.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fehbvm.com/Article/details/gxuciftiw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gryipogup.sHtML

[U115] JS：生成 UUID
来源：http://wap.zdbjq.cn/Article/details/gygcdavdo.sHtML

crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gdnpuwonq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fehbvm.com/Article/details/gfyprohsl.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.zdbjq.cn/Article/details/gbuquflaq.sHtML

[U117] JS：单元测试
来源：http://wap.hesvh.cn/Article/details/gaotzfppy.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.zdbjq.cn/Article/details/gfnyfdmfx.sHtML

[U118] JS：开发服务器
来源：http://mobile.zdbjq.cn/Article/details/gqrxstjex.sHtML

npm i -D vite;  npx vite
来源：http://baike.zdbjq.cn/Article/details/gyzmazmgy.sHtML

[U119] JS：生产构建
来源：http://www.blog.hesvh.cn/Article/details/gytgpelbs.sHtML

npx vite build
来源：http://read.share.fehbvm.com/Article/details/gndtbahqg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fehbvm.com/Article/details/gvrhiljsf.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.zdbjq.cn/Article/details/gipgphijp.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gutiwkwfy.sHtML

统计汇总
来源：http://read.share.zdbjq.cn/Article/details/godusazxn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gntuukhpq.sHtML

按语言统计（条）：
来源：http://www.blog.hesvh.cn/Article/details/ggtrcdghd.sHtML

Python ......... 252
来源：http://read.share.zdbjq.cn/Article/details/gwatxkovj.sHtML

PHP ............ 252
来源：http://mobile.zdbjq.cn/Article/details/gbburqamn.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/gtcplrgzl.sHtML

TypeScript ..... 212
来源：http://www.blog.zdbjq.cn/Article/details/gtoblmavz.sHtML

Java ........... 212
来源：http://wap.zdbjq.cn/Article/details/gapufpktj.sHtML

Go ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gfxdrsffn.sHtML

Ruby ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gtelhdcxm.sHtML

C# ............. 212
来源：http://www.blog.hesvh.cn/Article/details/ggvuayzud.sHtML

C .............. 30
来源：http://wap.zdbjq.cn/Article/details/gmoecognf.sHtML

C++ ............ 30
来源：http://blog.hesvh.cn/Article/details/gfawoniek.sHtML

SQL ............ 90
来源：http://blog.hesvh.cn/Article/details/gcqtguwkn.sHtML

Bash ........... 80
来源：http://blog.hesvh.cn/Article/details/gwkdkhjvf.sHtML

Kotlin ......... 15
来源：http://www.blog.zdbjq.cn/Article/details/gqjnnbagm.sHtML

Swift .......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gujuwuoyn.sHtML

Lua ............ 10
来源：http://wap.fehbvm.com/Article/details/gxglkuxos.sHtML

Perl ........... 10
来源：http://www.blog.fehbvm.com/Article/details/gfnlwpqld.sHtML

Scala .......... 10
来源：http://www.share.hesvh.cn/Article/details/gffzsrtwf.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/ggidzxzts.sHtML

合计 ........... 2106 条
来源：http://m.share.fehbvm.com/Article/details/gsjfyaquq.sHtML

按章节统计：
来源：http://blog.fehbvm.com/Article/details/gzcnqmffl.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/gsylftqsb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gvbhdpeiz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gnebetmyj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/gkppxtbhr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fehbvm.com/Article/details/goczhmmlh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gzvneaqem.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gogqraocg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gdhskmqxi.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/ggktdzijp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gijvlskbw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gijcblbbf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gvqwmfifa.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gxwzppnzk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/gdfefkjvs.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.zdbjq.cn/Article/details/gzxdifobn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gptskonvl.sHtML

Q SQL 专题                              90
来源：http://wap.zdbjq.cn/Article/details/gskxfnvad.sHtML

R Bash 专题                             80
来源：http://www.share.fehbvm.com/Article/details/goaujwlvi.sHtML

S C / C++ 专题                          60
来源：http://www.share.hesvh.cn/Article/details/gkrcvzmtq.sHtML

T 其他语言补充                          60
来源：http://read.share.hesvh.cn/Article/details/gthpvmctk.sHtML

U 高频实用片段                         120
来源：http://3g.hesvh.cn/Article/details/gysmazcbb.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gqhpomjsu.sHtML

合计                                  2106 条
来源：http://read.share.fehbvm.com/Article/details/gewxgkbzy.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gvxdzsbjz.sHtML

使用提醒
来源：http://3g.zdbjq.cn/Article/details/gecrenevs.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gffykfsds.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fehbvm.com/Article/details/gtnlnggpw.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.hesvh.cn/Article/details/gyzsegxcq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.zdbjq.cn/Article/details/gtsdvjwuv.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fehbvm.com/Article/details/guwdpjtes.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.hesvh.cn/Article/details/gmvfscgey.sHtML

—— 文件结束 ——
来源：http://m.share.fehbvm.com/Article/details/gifgvenjt.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gsvcbkjqq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.zdbjq.cn/Article/details/gllywdmnp.sHtML

Common Programming Examples Cheat Book
来源：http://wap.zdbjq.cn/Article/details/gxxbrsmdk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjjqepxkz.sHtML

【收录内容】
来源：http://www.share.hesvh.cn/Article/details/gqhvzcqka.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.hesvh.cn/Article/details/gicnfltcw.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.fehbvm.com/Article/details/gheidszye.sHtML

SQL · Bash · C · C++
来源：http://baike.zdbjq.cn/Article/details/gkvpcswbv.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fehbvm.com/Article/details/glzltuqru.sHtML

【使用说明】
来源：http://m.share.zdbjq.cn/Article/details/gsjionzhl.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.zdbjq.cn/Article/details/giyuppbgo.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.hesvh.cn/Article/details/gjrxundpm.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fehbvm.com/Article/details/gdzexuypk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fehbvm.com/Article/details/grkjvogfa.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.hesvh.cn/Article/details/gusucfxkc.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.zdbjq.cn/Article/details/gbhqhakgb.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.hesvh.cn/Article/details/ghtpglfmq.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.hesvh.cn/Article/details/gscfthxjl.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.hesvh.cn/Article/details/gourctfhg.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.zdbjq.cn/Article/details/gsprolqes.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.fehbvm.com/Article/details/gnjepwfeo.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.fehbvm.com/Article/details/gbanmgiva.sHtML

【文件统计】
来源：http://mobile.zdbjq.cn/Article/details/gltdunxpb.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.zdbjq.cn/Article/details/gglfyptrm.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gsszpgltd.sHtML

目  录
来源：http://3g.hesvh.cn/Article/details/gtobjvtdl.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gzaebgosy.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.hesvh.cn/Article/details/gthamslpq.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gtwpkxkpl.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gpshgyqto.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.hesvh.cn/Article/details/gvnpwxlpg.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fehbvm.com/Article/details/gcdrtnbzl.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/gydzxzqzl.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/gpqrgttgm.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gvrxqnque.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gpxunavep.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/gfrfenvsu.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gkkxrrbnk.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gpicgkyhu.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gwrrfmjsc.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.hesvh.cn/Article/details/gyyrhemge.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.zdbjq.cn/Article/details/gmffutklm.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gqvlydkau.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.fehbvm.com/Article/details/goojdjrdl.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.fehbvm.com/Article/details/ghowixgxc.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.fehbvm.com/Article/details/gdtzsaupo.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/ggbcgtytd.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gxuwklaag.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyjvezefh.sHtML

A. 基础语法与类型
来源：http://blog.hesvh.cn/Article/details/glzwwfkbl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvffujnnj.sHtML

[A01] Hello World
来源：http://m.share.hesvh.cn/Article/details/gvckrnuxb.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/geikdsprl.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.zdbjq.cn/Article/details/gtilzbqwf.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gmavbhdrl.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.fehbvm.com/Article/details/gjrygqanp.sHtML


<!-- 参考信息 -->