代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://3g.fehbvm.com/Article/details/gyjlluroo.sHtML

@contextlib.contextmanager
来源：http://3g.fehbvm.com/Article/details/gquqyglhk.sHtML

[U22] Py：矩阵转置
来源：http://baike.hesvh.cn/Article/details/gdwlqsgbj.sHtML

list(zip(*m))
来源：http://wap.zdbjq.cn/Article/details/gufulsvgs.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.zdbjq.cn/Article/details/gutdktmeb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.zdbjq.cn/Article/details/gpjpmbrqw.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/gmvdwhzmk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gkftshskb.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.hesvh.cn/Article/details/grhhojiam.sHtML

csv.DictReader(f)
来源：http://m.share.hesvh.cn/Article/details/grjjmakes.sHtML

[U26] Py：并发下载
来源：http://3g.hesvh.cn/Article/details/gdexuxayy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.zdbjq.cn/Article/details/geuidvuvn.sHtML

[U27] Py：异步 HTTP
来源：http://baike.zdbjq.cn/Article/details/gzboguzsk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.hesvh.cn/Article/details/gmwhmunuo.sHtML

[U28] Py：类型别名
来源：http://m.share.zdbjq.cn/Article/details/gudgsdiui.sHtML

UserId = int
来源：http://mobile.fehbvm.com/Article/details/gxylhgfrx.sHtML

[U29] Py：属性校验
来源：http://baike.hesvh.cn/Article/details/grcvdovfo.sHtML

@property 与 @x.setter 配合
来源：http://3g.fehbvm.com/Article/details/gqrwonrhy.sHtML

[U30] Py：数据类
来源：http://m.share.zdbjq.cn/Article/details/gtegkgvvc.sHtML

@dataclass(slots=True)
来源：http://3g.zdbjq.cn/Article/details/goioumkxj.sHtML

[U31] Py：单测
来源：http://m.share.hesvh.cn/Article/details/geihactrx.sHtML

python -m pytest -q
来源：http://baike.hesvh.cn/Article/details/goljhfngh.sHtML

[U32] Py：代码格式化
来源：http://www.blog.zdbjq.cn/Article/details/guzgymoqe.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.hesvh.cn/Article/details/gfmvajgha.sHtML

[U33] Py：打包发布
来源：http://read.share.hesvh.cn/Article/details/gbjlpmyso.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/gewxeapqp.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/ghhtqmwya.sHtML

chardet.detect(raw)
来源：http://www.blog.zdbjq.cn/Article/details/gpwobjwsd.sHtML

[U35] Py：发送邮件
来源：http://www.blog.hesvh.cn/Article/details/gpivvrrgf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fehbvm.com/Article/details/guwgqdmqp.sHtML

[U36] Py：定时任务
来源：http://wap.zdbjq.cn/Article/details/gggovnoej.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fehbvm.com/Article/details/grompitrj.sHtML

[U37] Py：读写 Excel
来源：http://blog.zdbjq.cn/Article/details/giqqqbkho.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fehbvm.com/Article/details/gzsggdner.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fehbvm.com/Article/details/gcuhxnvds.sHtML

Path(__file__).resolve().parent
来源：http://blog.hesvh.cn/Article/details/gkapdalvn.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.zdbjq.cn/Article/details/guahpjnrs.sHtML

sys.stdout.isatty()
来源：http://baike.hesvh.cn/Article/details/gnbqntojc.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.zdbjq.cn/Article/details/gpkdwvyuy.sHtML

print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gnpookidb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.hesvh.cn/Article/details/guwatlddq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/gbwlmvogo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fehbvm.com/Article/details/gnfaaasjn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fehbvm.com/Article/details/gvdkbayvq.sHtML

[U43] PHP：声明命名空间
来源：http://blog.zdbjq.cn/Article/details/gfcqmxzev.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/gomorwnkw.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/govybsyeq.sHtML

declare(strict_types=1);
来源：http://mobile.hesvh.cn/Article/details/grpbwhahk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fehbvm.com/Article/details/gwtdlyonl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gcxijwwij.sHtML

[U46] PHP：可空类型
来源：http://baike.fehbvm.com/Article/details/gtvrhmhvu.sHtML

?string $name = null
来源：http://www.share.fehbvm.com/Article/details/gqnsgyiyt.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.hesvh.cn/Article/details/gvwpeowfb.sHtML

int|string $id
来源：http://3g.fehbvm.com/Article/details/gakhepweg.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.hesvh.cn/Article/details/ggcqzfjom.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.zdbjq.cn/Article/details/grnrvfzdx.sHtML

[U49] PHP：只读属性
来源：http://www.blog.zdbjq.cn/Article/details/glbrlpswa.sHtML

public readonly string $name
来源：http://wap.fehbvm.com/Article/details/gppgrrkrh.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/gpvsofeko.sHtML

public function __construct(private int $id) {}
来源：http://wap.zdbjq.cn/Article/details/gpqshlvkt.sHtML

[U51] PHP：数组解构
来源：http://blog.hesvh.cn/Article/details/gdrldfmtk.sHtML

[$a, $b] = $arr;
来源：http://wap.hesvh.cn/Article/details/gckuyycsu.sHtML

[U52] PHP：箭头函数
来源：http://3g.zdbjq.cn/Article/details/ggypduqwa.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.hesvh.cn/Article/details/gfbcxqvvp.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.zdbjq.cn/Article/details/gthpqfhpy.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fehbvm.com/Article/details/gcswcrhxy.sHtML

[U54] PHP：空安全调用
来源：http://3g.zdbjq.cn/Article/details/guvatsxlf.sHtML

$obj?->method()
来源：http://read.share.hesvh.cn/Article/details/gbmkhaiko.sHtML

[U55] PHP：match 表达式
来源：http://read.share.hesvh.cn/Article/details/geucwxybp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fehbvm.com/Article/details/ggqvhnmmt.sHtML

[U56] PHP：命名参数
来源：http://mobile.hesvh.cn/Article/details/gidwmkfjo.sHtML

f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/grqjkgtmg.sHtML

[U57] PHP：字符串插值
来源：http://www.share.hesvh.cn/Article/details/grbripsvu.sHtML

"值: {$a}"
来源：http://www.share.zdbjq.cn/Article/details/ggszmchkw.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.zdbjq.cn/Article/details/ghtxrmvce.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gkjvswoyj.sHtML

[U59] PHP：自定义排序
来源：http://wap.hesvh.cn/Article/details/gcegmnxac.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gvkewvcsb.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.hesvh.cn/Article/details/gwuflqvdq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fehbvm.com/Article/details/giqfhisfg.sHtML

[U61] PHP：正则
来源：http://m.share.zdbjq.cn/Article/details/gnggjojqj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/gaiumubul.sHtML

[U62] PHP：日期对象
来源：http://www.share.hesvh.cn/Article/details/grpkcvlov.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fehbvm.com/Article/details/gcpcmuekt.sHtML

[U63] PHP：文件读写
来源：http://read.share.hesvh.cn/Article/details/gxwekqskf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fehbvm.com/Article/details/gwzlhouwa.sHtML

[U64] PHP：目录遍历
来源：http://baike.zdbjq.cn/Article/details/geenfuhep.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.hesvh.cn/Article/details/ggexjjtpk.sHtML

[U65] PHP：会话
来源：http://baike.fehbvm.com/Article/details/gxcuqidjj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fehbvm.com/Article/details/gwjhqgjoa.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.zdbjq.cn/Article/details/gpsltwfxs.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fehbvm.com/Article/details/gbeshpjlu.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fehbvm.com/Article/details/gklvoiavt.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.zdbjq.cn/Article/details/gcvxhiily.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.hesvh.cn/Article/details/gcylhrzdj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.zdbjq.cn/Article/details/gzjlstuhg.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.zdbjq.cn/Article/details/gfslsqrmc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fehbvm.com/Article/details/gtubwzify.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fehbvm.com/Article/details/gxuctnbpl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.zdbjq.cn/Article/details/gnczatpam.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fehbvm.com/Article/details/ghhgtmwhk.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.zdbjq.cn/Article/details/gzvvaysly.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fehbvm.com/Article/details/gztvvlbwb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fehbvm.com/Article/details/gifshjjbh.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.zdbjq.cn/Article/details/gxgskgdbv.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.zdbjq.cn/Article/details/gxvbxpabv.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gmlbgaymw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fehbvm.com/Article/details/gkavovwjz.sHtML

[U75] PHP：依赖注入
来源：http://read.share.hesvh.cn/Article/details/gtpjqhkfg.sHtML

composer require psr/container
来源：http://3g.zdbjq.cn/Article/details/gkrthteps.sHtML

[U76] PHP：简单路由
来源：http://www.share.zdbjq.cn/Article/details/goejovsyy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.zdbjq.cn/Article/details/gfigzbuxo.sHtML

[U77] PHP：模板渲染
来源：http://baike.hesvh.cn/Article/details/glqmxycmo.sHtML

composer require twig/twig
来源：http://read.share.zdbjq.cn/Article/details/gowdlzlnu.sHtML

[U78] PHP：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gdusetsxe.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.zdbjq.cn/Article/details/gbyaovnfc.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fehbvm.com/Article/details/gyignfupb.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.hesvh.cn/Article/details/ghcshmgdb.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fehbvm.com/Article/details/gphhvoavw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.zdbjq.cn/Article/details/gyjgjbcvx.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.zdbjq.cn/Article/details/gdwpljpjj.sHtML

npm init -y;  npm i express
来源：http://www.blog.fehbvm.com/Article/details/ggfhyclaf.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.zdbjq.cn/Article/details/gtahfxyfz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.hesvh.cn/Article/details/garisdjre.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.hesvh.cn/Article/details/grfshdwdq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/ghonhlyhw.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.zdbjq.cn/Article/details/gjwiuaslc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.hesvh.cn/Article/details/graaxawup.sHtML

[U85] JS：可选链
来源：http://mobile.hesvh.cn/Article/details/geqhqomsq.sHtML

a?.b?.c
来源：http://www.share.hesvh.cn/Article/details/gvqnmhxqs.sHtML

[U86] JS：空值合并
来源：http://blog.hesvh.cn/Article/details/gubjhefgl.sHtML

a ?? b
来源：http://baike.fehbvm.com/Article/details/gtkdshoui.sHtML

[U87] JS：解构默认值
来源：http://read.share.fehbvm.com/Article/details/glozpcfbp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.zdbjq.cn/Article/details/ggxdblsoy.sHtML

[U88] JS：对象展开合并
来源：http://baike.fehbvm.com/Article/details/gpwhjchzg.sHtML

{ ...a, ...b }
来源：http://read.share.fehbvm.com/Article/details/gqggebwrv.sHtML

[U89] JS：数组去重
来源：http://baike.fehbvm.com/Article/details/gmfvmwcea.sHtML

[...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/guryzejjr.sHtML

[U90] JS：数字数组排序
来源：http://mobile.hesvh.cn/Article/details/gicdmzsgi.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gjplcvecz.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fehbvm.com/Article/details/gergghlmj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.hesvh.cn/Article/details/gpzwvbllm.sHtML

[U92] JS：深拷贝
来源：http://mobile.hesvh.cn/Article/details/gnzhvwrui.sHtML

structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gfjgzekxs.sHtML

[U93] JS：模板字符串
来源：http://www.share.hesvh.cn/Article/details/gubtebryp.sHtML

`共 ${n} 条`
来源：http://baike.fehbvm.com/Article/details/gdwfxqxtu.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gppzvshmm.sHtML

const double = x => x * 2;
来源：http://baike.zdbjq.cn/Article/details/gmjpbhylq.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fehbvm.com/Article/details/gvbukpnev.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.hesvh.cn/Article/details/gohjeumbj.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.zdbjq.cn/Article/details/geuinrbqr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gmrfksioo.sHtML

[U97] JS：并发请求
来源：http://www.blog.zdbjq.cn/Article/details/gggzghenk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gjplyoljf.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.zdbjq.cn/Article/details/gbmiomtug.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fehbvm.com/Article/details/gxffspjrd.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fehbvm.com/Article/details/gembbknbr.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/gcebsmujg.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.hesvh.cn/Article/details/gammwpyad.sHtML

document.querySelector(".item")
来源：http://baike.fehbvm.com/Article/details/gmzpwkuhx.sHtML

[U101] JS：classList 操作
来源：http://www.share.zdbjq.cn/Article/details/gsxuapqxt.sHtML

el.classList.toggle("active")
来源：http://blog.zdbjq.cn/Article/details/gwtsxeoxz.sHtML

[U102] JS：本地存储
来源：http://wap.fehbvm.com/Article/details/gjwdrsctz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fehbvm.com/Article/details/gossbueku.sHtML

[U103] JS：定时器
来源：http://www.m.share.zdbjq.cn/Article/details/gjntlcnpd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.hesvh.cn/Article/details/gqetorjhi.sHtML

[U104] JS：防抖
来源：http://3g.hesvh.cn/Article/details/gnxhtvwgg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gtlfjotmi.sHtML

[U105] JS：节流
来源：http://wap.hesvh.cn/Article/details/gcqhtrrae.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fehbvm.com/Article/details/gljsefhrj.sHtML

[U106] JS：日期格式化
来源：http://blog.hesvh.cn/Article/details/gomcxnknk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.zdbjq.cn/Article/details/gatnwtfxx.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gkyladjzl.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.hesvh.cn/Article/details/gqezrvuya.sHtML

[U108] JS：随机整数
来源：http://baike.hesvh.cn/Article/details/gliikdijy.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.zdbjq.cn/Article/details/gdgonfaer.sHtML

[U109] JS：数组分组
来源：http://www.share.zdbjq.cn/Article/details/gpbakwbij.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gulltxmdb.sHtML

[U110] JS：数组分块
来源：http://baike.hesvh.cn/Article/details/ggvrsehuh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.hesvh.cn/Article/details/glsqtlkug.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/gqjgdvjvm.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/gxgoeyzxf.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.zdbjq.cn/Article/details/ggfvnlqjs.sHtML

"7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gvqhlcnny.sHtML

[U113] JS：正则替换全部
来源：http://m.share.hesvh.cn/Article/details/gcxqpdaez.sHtML

s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/groflpqrp.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.zdbjq.cn/Article/details/ggeqqjsci.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gsqropova.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gvrbioyfv.sHtML

crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gngwdkjzz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.zdbjq.cn/Article/details/gpcvyszee.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.hesvh.cn/Article/details/gndgtqhhb.sHtML

[U117] JS：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gdocrlhdq.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.hesvh.cn/Article/details/gyxfbekgu.sHtML

[U118] JS：开发服务器
来源：http://mobile.hesvh.cn/Article/details/gjdyznbzf.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fehbvm.com/Article/details/gydkhbnfo.sHtML

[U119] JS：生产构建
来源：http://m.share.hesvh.cn/Article/details/gpdpxxktu.sHtML

npx vite build
来源：http://www.share.hesvh.cn/Article/details/gihhawusf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fehbvm.com/Article/details/geljlitne.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.zdbjq.cn/Article/details/gxhptmzvl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gktwrhule.sHtML

统计汇总
来源：http://www.blog.hesvh.cn/Article/details/gggedgscv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gudhharzu.sHtML

按语言统计（条）：
来源：http://baike.fehbvm.com/Article/details/ghfekpctk.sHtML

Python ......... 252
来源：http://blog.fehbvm.com/Article/details/gqobvqbmb.sHtML

PHP ............ 252
来源：http://mobile.fehbvm.com/Article/details/gblzpmgtb.sHtML

JavaScript ..... 252
来源：http://www.m.share.fehbvm.com/Article/details/gaqfepnou.sHtML

TypeScript ..... 212
来源：http://www.blog.zdbjq.cn/Article/details/gbfssieur.sHtML

Java ........... 212
来源：http://mobile.fehbvm.com/Article/details/gqgsuljyr.sHtML

Go ............. 212
来源：http://blog.zdbjq.cn/Article/details/gubobycgw.sHtML

Ruby ........... 212
来源：http://baike.fehbvm.com/Article/details/gmiqehsww.sHtML

C# ............. 212
来源：http://mobile.fehbvm.com/Article/details/gouwiuvys.sHtML

C .............. 30
来源：http://baike.hesvh.cn/Article/details/glqesbzlw.sHtML

C++ ............ 30
来源：http://3g.fehbvm.com/Article/details/gmslzmkqm.sHtML

SQL ............ 90
来源：http://www.m.share.hesvh.cn/Article/details/gxhagrtjo.sHtML

Bash ........... 80
来源：http://read.share.hesvh.cn/Article/details/glsexbkns.sHtML

Kotlin ......... 15
来源：http://read.share.hesvh.cn/Article/details/gpnkuzahc.sHtML

Swift .......... 15
来源：http://mobile.zdbjq.cn/Article/details/ggqpucwpo.sHtML

Lua ............ 10
来源：http://www.blog.fehbvm.com/Article/details/gquyolkjw.sHtML

Perl ........... 10
来源：http://read.share.hesvh.cn/Article/details/gyxfhvexs.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/goevpvlnh.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gpfrwtbsy.sHtML

合计 ........... 2106 条
来源：http://m.share.fehbvm.com/Article/details/gyhynvsrz.sHtML

按章节统计：
来源：http://wap.fehbvm.com/Article/details/grlbisidc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gkzofmzvz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gfaixtbhp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gpflbmrzh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gnnaqztxm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.hesvh.cn/Article/details/gqpzwqgum.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gxkbbcrut.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gaypnkjoi.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gtwyaltsd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gboonfige.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gjcteapor.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gtbthkfks.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gzegmwhsf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gxxinwkqo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gxwswyaxl.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.zdbjq.cn/Article/details/gtdkuzyxl.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gabmbbfop.sHtML

Q SQL 专题                              90
来源：http://baike.hesvh.cn/Article/details/ggxzmoemh.sHtML

R Bash 专题                             80
来源：http://baike.zdbjq.cn/Article/details/gdgvswfno.sHtML

S C / C++ 专题                          60
来源：http://3g.zdbjq.cn/Article/details/gsllsdyem.sHtML

T 其他语言补充                          60
来源：http://www.m.share.hesvh.cn/Article/details/gxxqexkum.sHtML

U 高频实用片段                         120
来源：http://m.share.fehbvm.com/Article/details/ghrdonlgc.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gkplatzxo.sHtML

合计                                  2106 条
来源：http://baike.fehbvm.com/Article/details/gfewfxrbe.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gzqyvljbv.sHtML

使用提醒
来源：http://www.share.zdbjq.cn/Article/details/guyuhdlsc.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gegkalkoc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.hesvh.cn/Article/details/gprychmwf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fehbvm.com/Article/details/gcmimpcip.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.hesvh.cn/Article/details/gjcnlikya.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.hesvh.cn/Article/details/gjjkaoqgi.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.zdbjq.cn/Article/details/gkzqbrtmi.sHtML

—— 文件结束 ——
来源：http://blog.zdbjq.cn/Article/details/gnwqithyw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwfslmzwd.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.hesvh.cn/Article/details/grtmwtbgj.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.hesvh.cn/Article/details/gquynbxeb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfavblttt.sHtML

【收录内容】
来源：http://wap.fehbvm.com/Article/details/gvueqgnkk.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.zdbjq.cn/Article/details/ghvfolnmg.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.fehbvm.com/Article/details/gedlubeop.sHtML

SQL · Bash · C · C++
来源：http://www.share.fehbvm.com/Article/details/gftaiwmln.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.zdbjq.cn/Article/details/gdtbzadwr.sHtML

【使用说明】
来源：http://www.blog.hesvh.cn/Article/details/gblhpwgps.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fehbvm.com/Article/details/gjfsdtmwv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.hesvh.cn/Article/details/gsgoymslp.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.zdbjq.cn/Article/details/gzgsfvbwb.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.hesvh.cn/Article/details/gxtbzghhj.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.hesvh.cn/Article/details/gausziklc.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fehbvm.com/Article/details/grnplexry.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.zdbjq.cn/Article/details/gyemtzpty.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.zdbjq.cn/Article/details/gtzcbkkut.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.fehbvm.com/Article/details/gizzwixyt.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.zdbjq.cn/Article/details/grbfogwcc.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fehbvm.com/Article/details/gxwwwcmsd.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.fehbvm.com/Article/details/gfuteznjn.sHtML

【文件统计】
来源：http://mobile.zdbjq.cn/Article/details/gfrcqjjnq.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.zdbjq.cn/Article/details/gkpolmgos.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gygrzaimq.sHtML

目  录
来源：http://baike.fehbvm.com/Article/details/gxlkwpwoz.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gbvaktuql.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/gaacadxez.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/glhldprlb.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gruykxcxo.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gaoivkwjy.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.zdbjq.cn/Article/details/glgagmsrr.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.fehbvm.com/Article/details/gbuuxloel.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gxbyavkao.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.hesvh.cn/Article/details/gcpsypsjr.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gemqvwgkl.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gvegnyxjh.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/goenczqvi.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gcclnvlln.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gkmebtrab.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.hesvh.cn/Article/details/guatvbgdj.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.hesvh.cn/Article/details/ggmflsuvv.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gknmlueps.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.zdbjq.cn/Article/details/gpfyxelnu.sHtML


<!-- 参考信息 -->