代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://3g.fanxiaobao.xyz/Article/details/gmqonzfnh.sHtML

@contextlib.contextmanager
来源：http://m.share.fanxiaobao.xyz/Article/details/gpchrhflr.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fanxiaobao.xyz/Article/details/gqoktmmno.sHtML

list(zip(*m))
来源：http://3g.fanxiaobao.xyz/Article/details/gxbebvpat.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gaatlukgw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fanxiaobao.xyz/Article/details/gikleqxmu.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/grjcdwsck.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gavqxapco.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fanxiaobao.xyz/Article/details/gkimhkxsc.sHtML

csv.DictReader(f)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfindply.sHtML

[U26] Py：并发下载
来源：http://m.share.fanxiaobao.xyz/Article/details/gjufitsbx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbmjfdja.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fanxiaobao.xyz/Article/details/gixedcxju.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyfngsse.sHtML

[U28] Py：类型别名
来源：http://www.share.fanxiaobao.xyz/Article/details/glbhrufvq.sHtML

UserId = int
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdsqghnn.sHtML

[U29] Py：属性校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gueoiwdia.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fanxiaobao.xyz/Article/details/grxstmvbg.sHtML

[U30] Py：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gqcieapcn.sHtML

@dataclass(slots=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gwuhcknnv.sHtML

[U31] Py：单测
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbevarxed.sHtML

python -m pytest -q
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfvtaoic.sHtML

[U32] Py：代码格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gebfiwfec.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fanxiaobao.xyz/Article/details/giwmmnxcc.sHtML

[U33] Py：打包发布
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvfynsgz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgqfyaot.sHtML

[U34] Py：判断编码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklfeubvv.sHtML

chardet.detect(raw)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsbyhbll.sHtML

[U35] Py：发送邮件
来源：http://wap.fanxiaobao.xyz/Article/details/gmxighvwb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fanxiaobao.xyz/Article/details/gactklzcd.sHtML

[U36] Py：定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/ggdczpqab.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fanxiaobao.xyz/Article/details/gihzktbxj.sHtML

[U37] Py：读写 Excel
来源：http://blog.fanxiaobao.xyz/Article/details/gpczsyejg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gogvymmgc.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsitcsph.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkkfslvb.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fanxiaobao.xyz/Article/details/gjrwpionp.sHtML

sys.stdout.isatty()
来源：http://www.share.fanxiaobao.xyz/Article/details/gosxhjfil.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqygiyscz.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guswgdyqn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlqljokc.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fanxiaobao.xyz/Article/details/grysgcytm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fanxiaobao.xyz/Article/details/gacoqvfwd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gblrllypb.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gsdtrxhbw.sHtML

namespace App\Http;
来源：http://blog.fanxiaobao.xyz/Article/details/gbbooozgd.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fanxiaobao.xyz/Article/details/geamufmup.sHtML

declare(strict_types=1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbvispni.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fanxiaobao.xyz/Article/details/gmfvpxrwl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawroebfc.sHtML

[U46] PHP：可空类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gwymqzyew.sHtML

?string $name = null
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfipqjaz.sHtML

[U47] PHP：联合类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnmhmuuo.sHtML

int|string $id
来源：http://m.share.fanxiaobao.xyz/Article/details/gvaktevzn.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgqepebv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gapjoiiuh.sHtML

[U49] PHP：只读属性
来源：http://wap.fanxiaobao.xyz/Article/details/gxxvdinje.sHtML

public readonly string $name
来源：http://m.share.fanxiaobao.xyz/Article/details/gwuhauakl.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fanxiaobao.xyz/Article/details/gxslnbaub.sHtML

public function __construct(private int $id) {}
来源：http://3g.fanxiaobao.xyz/Article/details/giwsljvpd.sHtML

[U51] PHP：数组解构
来源：http://wap.fanxiaobao.xyz/Article/details/gztxphjki.sHtML

[$a, $b] = $arr;
来源：http://www.share.fanxiaobao.xyz/Article/details/gekrxaxwb.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvmreaxu.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxkuetht.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpcucwsj.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fanxiaobao.xyz/Article/details/gnhaegwus.sHtML

[U54] PHP：空安全调用
来源：http://wap.fanxiaobao.xyz/Article/details/ghvvqfaeb.sHtML

$obj?->method()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpeqyffce.sHtML

[U55] PHP：match 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gexyxldpp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fanxiaobao.xyz/Article/details/giundglsm.sHtML

[U56] PHP：命名参数
来源：http://wap.fanxiaobao.xyz/Article/details/geijmuico.sHtML

f(a: 1, b: 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gatefhtdh.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjwpklbl.sHtML

"值: {$a}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmimtxufx.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdyciich.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/grkbzqcff.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/geghptszl.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/giurmmwfa.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyudgjnvw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkhryrwi.sHtML

[U61] PHP：正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmejfwaov.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/giqzmriqc.sHtML

[U62] PHP：日期对象
来源：http://3g.fanxiaobao.xyz/Article/details/gkquyaoqe.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyhngsnp.sHtML

[U63] PHP：文件读写
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdtcunio.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fanxiaobao.xyz/Article/details/gddgkolul.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkpjunny.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkxkivwg.sHtML

[U65] PHP：会话
来源：http://wap.fanxiaobao.xyz/Article/details/gaaweckxl.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzeksecdt.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fanxiaobao.xyz/Article/details/gvbcdftin.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/geeigfmfk.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjgelavi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifhsnzah.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdlegava.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fanxiaobao.xyz/Article/details/giuhfecvt.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fanxiaobao.xyz/Article/details/gydfrrugt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fanxiaobao.xyz/Article/details/grzgnrmvf.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fanxiaobao.xyz/Article/details/gxoihhlma.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfrjehdo.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljmczivl.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fanxiaobao.xyz/Article/details/gzygzrrhv.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnkbqewe.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fanxiaobao.xyz/Article/details/gyoawjasx.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fanxiaobao.xyz/Article/details/grmbfcohm.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fanxiaobao.xyz/Article/details/gxiiypqwb.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbfogdpq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fanxiaobao.xyz/Article/details/ghhiqnbna.sHtML

[U75] PHP：依赖注入
来源：http://wap.fanxiaobao.xyz/Article/details/gzihwcqzu.sHtML

composer require psr/container
来源：http://wap.fanxiaobao.xyz/Article/details/gnutvxlea.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpwahtsa.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fanxiaobao.xyz/Article/details/gihxmwtgr.sHtML

[U77] PHP：模板渲染
来源：http://blog.fanxiaobao.xyz/Article/details/gczwwrqul.sHtML

composer require twig/twig
来源：http://blog.fanxiaobao.xyz/Article/details/gdoyvttra.sHtML

[U78] PHP：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhrcsdtu.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fanxiaobao.xyz/Article/details/glcnkkxyj.sHtML

[U79] PHP：静态分析
来源：http://m.share.fanxiaobao.xyz/Article/details/gokpjbvrt.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fanxiaobao.xyz/Article/details/gojdnhoza.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsbmynir.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gruopscvo.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyngthhjr.sHtML

npm init -y;  npm i express
来源：http://3g.fanxiaobao.xyz/Article/details/gojfjtlrn.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fanxiaobao.xyz/Article/details/gqwqeqgbl.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbxhsbip.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchlvvtwr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fanxiaobao.xyz/Article/details/gxnfrzjtx.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfqnhtfb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fanxiaobao.xyz/Article/details/gshxcztpk.sHtML

[U85] JS：可选链
来源：http://read.share.fanxiaobao.xyz/Article/details/gejmlwcgz.sHtML

a?.b?.c
来源：http://blog.fanxiaobao.xyz/Article/details/ggtmzhzmg.sHtML

[U86] JS：空值合并
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdhogsmn.sHtML

a ?? b
来源：http://3g.fanxiaobao.xyz/Article/details/ghgtuqmpl.sHtML

[U87] JS：解构默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/grrnltopy.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fanxiaobao.xyz/Article/details/gbrspfavj.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fanxiaobao.xyz/Article/details/gojwowzzs.sHtML

{ ...a, ...b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkihragti.sHtML

[U89] JS：数组去重
来源：http://wap.fanxiaobao.xyz/Article/details/gnkeeyics.sHtML

[...new Set(arr)]
来源：http://www.share.fanxiaobao.xyz/Article/details/gapbeliiw.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fanxiaobao.xyz/Article/details/guokvagxt.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwowqomai.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhfaxalw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fanxiaobao.xyz/Article/details/gypbswwof.sHtML

[U92] JS：深拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsqhylgz.sHtML

structuredClone(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gnybimcxz.sHtML

[U93] JS：模板字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzktuzhv.sHtML

`共 ${n} 条`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwubqpasv.sHtML

[U94] JS：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/gnxqgzemr.sHtML

const double = x => x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goslafhsv.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fanxiaobao.xyz/Article/details/gibdywkpq.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/gisppsgne.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fanxiaobao.xyz/Article/details/grtztpkfy.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fanxiaobao.xyz/Article/details/gycclltdk.sHtML

[U97] JS：并发请求
来源：http://blog.fanxiaobao.xyz/Article/details/gdpdltjeu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/gijjepixq.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/govcwfjql.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazqvjodm.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwuzfdvz.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcnyssir.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gedptgrjf.sHtML

document.querySelector(".item")
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhjrjrwf.sHtML

[U101] JS：classList 操作
来源：http://3g.fanxiaobao.xyz/Article/details/gttjxuzeg.sHtML

el.classList.toggle("active")
来源：http://3g.fanxiaobao.xyz/Article/details/gevjrucbj.sHtML

[U102] JS：本地存储
来源：http://baike.fanxiaobao.xyz/Article/details/gdkeqakom.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fanxiaobao.xyz/Article/details/geqidsfrc.sHtML

[U103] JS：定时器
来源：http://m.share.fanxiaobao.xyz/Article/details/goxmjfite.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fanxiaobao.xyz/Article/details/gtmmpsikb.sHtML

[U104] JS：防抖
来源：http://read.share.fanxiaobao.xyz/Article/details/gjssmcunt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwyjasli.sHtML

[U105] JS：节流
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjbkyyko.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gfsrbkodt.sHtML

[U106] JS：日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/guykxgnni.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fanxiaobao.xyz/Article/details/gbskdnhse.sHtML

[U107] JS：数字千分位
来源：http://wap.fanxiaobao.xyz/Article/details/gghltxquu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fanxiaobao.xyz/Article/details/grocqsrcs.sHtML

[U108] JS：随机整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvxsjlht.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fanxiaobao.xyz/Article/details/gueeawvxw.sHtML

[U109] JS：数组分组
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpctziwp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fanxiaobao.xyz/Article/details/gersvdjhz.sHtML

[U110] JS：数组分块
来源：http://www.blog.fanxiaobao.xyz/Article/details/giatztzgk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwglxxipr.sHtML

[U111] JS：对象转 Map
来源：http://blog.fanxiaobao.xyz/Article/details/ggsjlvnra.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fanxiaobao.xyz/Article/details/gfaekoifq.sHtML

[U112] JS：字符串补位
来源：http://read.share.fanxiaobao.xyz/Article/details/gczkzeljq.sHtML

"7".padStart(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/gmhelbqqq.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzgicwku.sHtML

s.replaceAll("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gsardexwz.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fanxiaobao.xyz/Article/details/gxqpiozth.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnnlhbnn.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwifytzt.sHtML

crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gwehlbzuo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslnzzhgr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gqgxpmllm.sHtML

[U117] JS：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/geiovfulj.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggappevqe.sHtML

[U118] JS：开发服务器
来源：http://blog.fanxiaobao.xyz/Article/details/gwvlaezob.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvbqhcoe.sHtML

[U119] JS：生产构建
来源：http://wap.fanxiaobao.xyz/Article/details/gixzizmdh.sHtML

npx vite build
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdnykwrv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqtivvof.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fanxiaobao.xyz/Article/details/gylblruda.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcllxipe.sHtML

统计汇总
来源：http://baike.fanxiaobao.xyz/Article/details/gzhxdhtjf.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gplakdune.sHtML

按语言统计（条）：
来源：http://mobile.fanxiaobao.xyz/Article/details/grwogxagv.sHtML

Python ......... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gqprcfzzd.sHtML

PHP ............ 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqqfgocm.sHtML

JavaScript ..... 252
来源：http://baike.fanxiaobao.xyz/Article/details/grtpkygiw.sHtML

TypeScript ..... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gxiuagqqr.sHtML

Java ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/glmhhxwud.sHtML

Go ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqaeacqr.sHtML

Ruby ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gmodiqkmr.sHtML

C# ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/govhkfuue.sHtML

C .............. 30
来源：http://3g.fanxiaobao.xyz/Article/details/ghhsklspw.sHtML

C++ ............ 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvwlqsts.sHtML

SQL ............ 90
来源：http://3g.fanxiaobao.xyz/Article/details/gbkuwjyub.sHtML

Bash ........... 80
来源：http://3g.fanxiaobao.xyz/Article/details/gvpwtrobp.sHtML

Kotlin ......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/grynddvbn.sHtML

Swift .......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gfggkwnod.sHtML

Lua ............ 10
来源：http://blog.fanxiaobao.xyz/Article/details/gbtajywgp.sHtML

Perl ........... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govvnnuwq.sHtML

Scala .......... 10
来源：http://blog.fanxiaobao.xyz/Article/details/gkjfaevqo.sHtML

------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/geybdaedj.sHtML

合计 ........... 2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/giteffxpd.sHtML

按章节统计：
来源：http://read.share.fanxiaobao.xyz/Article/details/gdipembij.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gertsjdir.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/ghpprhjjp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gmydopgtg.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbqtjfop.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfgkqyeg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/gngkuivbl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojpqwcgi.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fanxiaobao.xyz/Article/details/gqomjnvtl.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqqpwshl.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/guwcdsrkz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/ggnrcjzpk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gepnjdfxr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gbyiydilz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fanxiaobao.xyz/Article/details/grwzjrmpx.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fanxiaobao.xyz/Article/details/gmaiaovez.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/grhpvczji.sHtML

Q SQL 专题                              90
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgxgxyix.sHtML

R Bash 专题                             80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplslwxgm.sHtML

S C / C++ 专题                          60
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfabijmb.sHtML

T 其他语言补充                          60
来源：http://m.share.fanxiaobao.xyz/Article/details/ggilqxodi.sHtML

U 高频实用片段                         120
来源：http://m.share.fanxiaobao.xyz/Article/details/glgynacnc.sHtML

------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyhfbnti.sHtML

合计                                  2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gwypsmpzb.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gqedcfjxw.sHtML

使用提醒
来源：http://read.share.fanxiaobao.xyz/Article/details/geaygljtp.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gsscvbnuo.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.fanxiaobao.xyz/Article/details/grixmvyuf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.fanxiaobao.xyz/Article/details/gtckbefgm.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdxtjylt.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fanxiaobao.xyz/Article/details/ghqroqygm.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnokwyba.sHtML

—— 文件结束 ——
来源：http://3g.fanxiaobao.xyz/Article/details/gjvyysbuj.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvotayzfb.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspsblygv.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fanxiaobao.xyz/Article/details/gfuptofdp.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gwybcteou.sHtML

【收录内容】
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrvlttrr.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fanxiaobao.xyz/Article/details/gpsvmdume.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.fanxiaobao.xyz/Article/details/gsuqtkmzk.sHtML

SQL · Bash · C · C++
来源：http://read.share.fanxiaobao.xyz/Article/details/goqxfqztm.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpivxckh.sHtML

【使用说明】
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcmgkjuc.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqizwqsab.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmfoaabv.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.fanxiaobao.xyz/Article/details/gvbeaehzc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fanxiaobao.xyz/Article/details/giveljvpn.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.fanxiaobao.xyz/Article/details/gmabqnooh.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.fanxiaobao.xyz/Article/details/gvqxedjey.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvnhfwuz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fanxiaobao.xyz/Article/details/gdjamrqwz.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxktghpm.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfyuxiic.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.fanxiaobao.xyz/Article/details/gealkwftb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkwnnniy.sHtML

【文件统计】
来源：http://blog.fanxiaobao.xyz/Article/details/gnffvqqjk.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.fanxiaobao.xyz/Article/details/gsvnqpxph.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgbztdzi.sHtML

目  录
来源：http://m.share.fanxiaobao.xyz/Article/details/grvzahqjl.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/guttyoxhh.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxytqdtu.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/ghiqgjrpx.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlsbspyf.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/guibcapjq.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gkyucthhp.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gnehwlbdd.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gngvklxso.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/goioqfugf.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/getzvirbg.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrlhacxl.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvejtjsu.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtkwpodl.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gwdopcxho.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gplwnulbz.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmxolotv.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gwddtkafl.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsuouvbq.sHtML


<!-- 参考信息 -->