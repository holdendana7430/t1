代发 wailian999

[U19] Py：正则替换带回调
来源：http://www.share.zdbjq.cn/Article/details/gczaiwmyo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fehbvm.com/Article/details/gxrmjftvk.sHtML

[U20] Py：缓存函数结果
来源：http://blog.hesvh.cn/Article/details/ghfrjszgc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fehbvm.com/Article/details/geyjhckbg.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.zdbjq.cn/Article/details/gkknoeidr.sHtML

@contextlib.contextmanager
来源：http://3g.hesvh.cn/Article/details/gyrjaysag.sHtML

[U22] Py：矩阵转置
来源：http://wap.hesvh.cn/Article/details/gpaghldlm.sHtML

list(zip(*m))
来源：http://www.blog.fehbvm.com/Article/details/gpyltbytx.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fehbvm.com/Article/details/gnsxsxbzj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.hesvh.cn/Article/details/gvraqmfkg.sHtML

[U24] Py：路径操作
来源：http://baike.fehbvm.com/Article/details/glxsjyliv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gjpqizqld.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.zdbjq.cn/Article/details/gqmnuutyr.sHtML

csv.DictReader(f)
来源：http://www.share.zdbjq.cn/Article/details/gyzanvars.sHtML

[U26] Py：并发下载
来源：http://3g.fehbvm.com/Article/details/gqdreyxrv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fehbvm.com/Article/details/goktteybz.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fehbvm.com/Article/details/gyjpwrggv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.zdbjq.cn/Article/details/gazlrqbhp.sHtML

[U28] Py：类型别名
来源：http://wap.zdbjq.cn/Article/details/gmafdqxrp.sHtML

UserId = int
来源：http://baike.hesvh.cn/Article/details/gplkskoxg.sHtML

[U29] Py：属性校验
来源：http://www.blog.fehbvm.com/Article/details/givaaydiz.sHtML

@property 与 @x.setter 配合
来源：http://blog.zdbjq.cn/Article/details/gnfzltnfh.sHtML

[U30] Py：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gwlfvxcvb.sHtML

@dataclass(slots=True)
来源：http://blog.hesvh.cn/Article/details/gkuqesdlc.sHtML

[U31] Py：单测
来源：http://www.blog.zdbjq.cn/Article/details/gyfkagaug.sHtML

python -m pytest -q
来源：http://mobile.hesvh.cn/Article/details/gfzvtcyqr.sHtML

[U32] Py：代码格式化
来源：http://www.share.fehbvm.com/Article/details/glnwviqjq.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.zdbjq.cn/Article/details/gkbwyibjh.sHtML

[U33] Py：打包发布
来源：http://wap.hesvh.cn/Article/details/gjstlfiqb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fehbvm.com/Article/details/gywemuikh.sHtML

[U34] Py：判断编码
来源：http://m.share.zdbjq.cn/Article/details/goqtwcfhf.sHtML

chardet.detect(raw)
来源：http://www.m.share.hesvh.cn/Article/details/gpquscpsl.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fehbvm.com/Article/details/gzijvkdik.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.hesvh.cn/Article/details/gifidvrrm.sHtML

[U36] Py：定时任务
来源：http://m.share.zdbjq.cn/Article/details/gmcnpfwtg.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.hesvh.cn/Article/details/gulpcarhn.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fehbvm.com/Article/details/gxrsskpaf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.hesvh.cn/Article/details/gfmdrvqik.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.zdbjq.cn/Article/details/gfodiuycg.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fehbvm.com/Article/details/gkqqpvcjv.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.hesvh.cn/Article/details/gzgtyvgmo.sHtML

sys.stdout.isatty()
来源：http://read.share.fehbvm.com/Article/details/geqvkmewv.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.hesvh.cn/Article/details/gjsbsvfxi.sHtML

print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gkixsnuwt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fehbvm.com/Article/details/grkjuaxxd.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.zdbjq.cn/Article/details/gkdvznkgd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.zdbjq.cn/Article/details/goutgshut.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.zdbjq.cn/Article/details/gkbxfintb.sHtML

[U43] PHP：声明命名空间
来源：http://blog.zdbjq.cn/Article/details/gtbmghcml.sHtML

namespace App\Http;
来源：http://3g.hesvh.cn/Article/details/gcelwzixg.sHtML

[U44] PHP：开启严格类型
来源：http://wap.zdbjq.cn/Article/details/ghkywcdsv.sHtML

declare(strict_types=1);
来源：http://www.share.fehbvm.com/Article/details/gyhawighy.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.hesvh.cn/Article/details/gtglnxsdx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gjbvwqtis.sHtML

[U46] PHP：可空类型
来源：http://m.share.zdbjq.cn/Article/details/gghpxvkkq.sHtML

?string $name = null
来源：http://m.share.zdbjq.cn/Article/details/gwmmhwzwo.sHtML

[U47] PHP：联合类型
来源：http://read.share.zdbjq.cn/Article/details/grkcdbycs.sHtML

int|string $id
来源：http://wap.hesvh.cn/Article/details/gnshyehqn.sHtML

[U48] PHP：纯枚举
来源：http://3g.fehbvm.com/Article/details/gazivriwx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.hesvh.cn/Article/details/glxjichmh.sHtML

[U49] PHP：只读属性
来源：http://wap.fehbvm.com/Article/details/gmudydtvu.sHtML

public readonly string $name
来源：http://blog.zdbjq.cn/Article/details/gzwvwzhgy.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.hesvh.cn/Article/details/giwsdnrsb.sHtML

public function __construct(private int $id) {}
来源：http://read.share.hesvh.cn/Article/details/gbijcivpv.sHtML

[U51] PHP：数组解构
来源：http://baike.fehbvm.com/Article/details/gbtiugqwy.sHtML

[$a, $b] = $arr;
来源：http://baike.zdbjq.cn/Article/details/gabafmeam.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fehbvm.com/Article/details/ghxumfygf.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fehbvm.com/Article/details/gynxuajyt.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/gmxzabjga.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/gfjqacigk.sHtML

[U54] PHP：空安全调用
来源：http://www.share.zdbjq.cn/Article/details/gjwpvfhzz.sHtML

$obj?->method()
来源：http://mobile.zdbjq.cn/Article/details/ghgmgplik.sHtML

[U55] PHP：match 表达式
来源：http://m.share.hesvh.cn/Article/details/gaagcaxqb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/gcneokxvd.sHtML

[U56] PHP：命名参数
来源：http://www.share.zdbjq.cn/Article/details/gvyulrgvo.sHtML

f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gwchzagnr.sHtML

[U57] PHP：字符串插值
来源：http://blog.fehbvm.com/Article/details/gedxvorjx.sHtML

"值: {$a}"
来源：http://mobile.fehbvm.com/Article/details/gdbwoyovk.sHtML

[U58] PHP：数组三件套
来源：http://wap.fehbvm.com/Article/details/goedfhbyz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fehbvm.com/Article/details/gldkzngye.sHtML

[U59] PHP：自定义排序
来源：http://wap.fehbvm.com/Article/details/glasswrth.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gtzhtnumf.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.zdbjq.cn/Article/details/gfixudokq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fehbvm.com/Article/details/ggmprqibr.sHtML

[U61] PHP：正则
来源：http://www.share.hesvh.cn/Article/details/gltxscnhj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fehbvm.com/Article/details/gjvwkjioj.sHtML

[U62] PHP：日期对象
来源：http://wap.zdbjq.cn/Article/details/gjdhkqxwl.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fehbvm.com/Article/details/giocxdxnx.sHtML

[U63] PHP：文件读写
来源：http://blog.fehbvm.com/Article/details/gjyzjcyfg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fehbvm.com/Article/details/gklpfwllv.sHtML

[U64] PHP：目录遍历
来源：http://wap.zdbjq.cn/Article/details/gyefuzfhc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.zdbjq.cn/Article/details/gjoierfmu.sHtML

[U65] PHP：会话
来源：http://read.share.hesvh.cn/Article/details/grgdiuqqt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/grvvgciea.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fehbvm.com/Article/details/gkgndxnru.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.zdbjq.cn/Article/details/gyqxphjvt.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fehbvm.com/Article/details/gmcuscloj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fehbvm.com/Article/details/grrwjrydr.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fehbvm.com/Article/details/gitdknxap.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.zdbjq.cn/Article/details/ghxphosbt.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fehbvm.com/Article/details/gomrjotce.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fehbvm.com/Article/details/gbwhakiif.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.zdbjq.cn/Article/details/gibdsizrp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.zdbjq.cn/Article/details/gadojjtdd.sHtML

[U71] PHP：抛出异常
来源：http://www.share.zdbjq.cn/Article/details/garbuguvh.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.hesvh.cn/Article/details/giswnbzsh.sHtML

[U72] PHP：写错误日志
来源：http://wap.zdbjq.cn/Article/details/gxrqxcecw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.hesvh.cn/Article/details/gzdktippb.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.hesvh.cn/Article/details/gwrchzfyu.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fehbvm.com/Article/details/gysurgzqn.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gtgtohofk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.zdbjq.cn/Article/details/gyoycmeiz.sHtML

[U75] PHP：依赖注入
来源：http://mobile.zdbjq.cn/Article/details/goforiiih.sHtML

composer require psr/container
来源：http://baike.zdbjq.cn/Article/details/gdmabsnec.sHtML

[U76] PHP：简单路由
来源：http://www.share.fehbvm.com/Article/details/gbscmrebs.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fehbvm.com/Article/details/gxevjdicm.sHtML

[U77] PHP：模板渲染
来源：http://wap.hesvh.cn/Article/details/gpfemyxun.sHtML

composer require twig/twig
来源：http://www.share.zdbjq.cn/Article/details/gvihgqwnl.sHtML

[U78] PHP：单元测试
来源：http://mobile.hesvh.cn/Article/details/gsymltaep.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fehbvm.com/Article/details/ganuwttuy.sHtML

[U79] PHP：静态分析
来源：http://m.share.fehbvm.com/Article/details/gmesilade.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fehbvm.com/Article/details/gneptujij.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.zdbjq.cn/Article/details/gfcbklopq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.hesvh.cn/Article/details/ggccjuoaj.sHtML

[U81] JS：初始化项目
来源：http://wap.fehbvm.com/Article/details/gyqpnmicv.sHtML

npm init -y;  npm i express
来源：http://wap.hesvh.cn/Article/details/gqxmovxia.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.hesvh.cn/Article/details/gxnhapbvf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.hesvh.cn/Article/details/grcniqlyj.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fehbvm.com/Article/details/guyqxauhr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gkjmpesgs.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.zdbjq.cn/Article/details/gjmqdqcpc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fehbvm.com/Article/details/gbxoclkav.sHtML

[U85] JS：可选链
来源：http://blog.fehbvm.com/Article/details/glvmssytw.sHtML

a?.b?.c
来源：http://www.m.share.zdbjq.cn/Article/details/gqqwcxqom.sHtML

[U86] JS：空值合并
来源：http://blog.fehbvm.com/Article/details/glnwgnbgu.sHtML

a ?? b
来源：http://www.share.zdbjq.cn/Article/details/gqvuniios.sHtML

[U87] JS：解构默认值
来源：http://www.blog.zdbjq.cn/Article/details/gdojybxwm.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fehbvm.com/Article/details/gvhiejlhs.sHtML

[U88] JS：对象展开合并
来源：http://www.share.zdbjq.cn/Article/details/gkgwifbly.sHtML

{ ...a, ...b }
来源：http://www.share.hesvh.cn/Article/details/giprysjdv.sHtML

[U89] JS：数组去重
来源：http://baike.hesvh.cn/Article/details/gruygcgqj.sHtML

[...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gzhpdlvlo.sHtML

[U90] JS：数字数组排序
来源：http://www.share.hesvh.cn/Article/details/gbdtgxdmd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gnwlevhvv.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.zdbjq.cn/Article/details/ghjqvgnqk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fehbvm.com/Article/details/gbststvzg.sHtML

[U92] JS：深拷贝
来源：http://wap.fehbvm.com/Article/details/gxdtjgstx.sHtML

structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gehomzntb.sHtML

[U93] JS：模板字符串
来源：http://baike.hesvh.cn/Article/details/gruhqarii.sHtML

`共 ${n} 条`
来源：http://3g.zdbjq.cn/Article/details/gripfmnxu.sHtML

[U94] JS：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gzniflwum.sHtML

const double = x => x * 2;
来源：http://read.share.fehbvm.com/Article/details/gdtlntoct.sHtML

[U95] JS：Promise 包装
来源：http://m.share.hesvh.cn/Article/details/geupgxsiq.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.hesvh.cn/Article/details/ghnavochn.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.zdbjq.cn/Article/details/gqphnzzih.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gzaesrkbr.sHtML

[U97] JS：并发请求
来源：http://www.share.fehbvm.com/Article/details/gpouomxha.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/girlptejw.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.zdbjq.cn/Article/details/garnlzlbu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fehbvm.com/Article/details/gznsikqpt.sHtML

[U99] JS：事件监听
来源：http://www.share.zdbjq.cn/Article/details/gmxernqro.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fehbvm.com/Article/details/gacheiasp.sHtML

[U100] JS：DOM 查询
来源：http://m.share.zdbjq.cn/Article/details/gzoggegcw.sHtML

document.querySelector(".item")
来源：http://read.share.fehbvm.com/Article/details/galjspftm.sHtML

[U101] JS：classList 操作
来源：http://baike.hesvh.cn/Article/details/gviuswitd.sHtML

el.classList.toggle("active")
来源：http://wap.zdbjq.cn/Article/details/gnqefzflw.sHtML

[U102] JS：本地存储
来源：http://m.share.hesvh.cn/Article/details/gjpokgcjl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.zdbjq.cn/Article/details/gsxrzvhat.sHtML

[U103] JS：定时器
来源：http://www.m.share.hesvh.cn/Article/details/gbgslbqpv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.zdbjq.cn/Article/details/gtrxcwhzg.sHtML

[U104] JS：防抖
来源：http://read.share.zdbjq.cn/Article/details/gaojqsyce.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gzvrtpydn.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/gdgqkwsfs.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.zdbjq.cn/Article/details/gvkjumqea.sHtML

[U106] JS：日期格式化
来源：http://blog.fehbvm.com/Article/details/gwtceckjc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.hesvh.cn/Article/details/grxtzlbzb.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gzujykpwm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gsefjkxqh.sHtML

[U108] JS：随机整数
来源：http://baike.fehbvm.com/Article/details/gabbalhxc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.hesvh.cn/Article/details/gllhvkovg.sHtML

[U109] JS：数组分组
来源：http://www.m.share.hesvh.cn/Article/details/gtsbqdrue.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gearrqznu.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/gqznjjfmd.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.zdbjq.cn/Article/details/gkxalzxsp.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fehbvm.com/Article/details/gtyqxguzu.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/gpkizzeir.sHtML

[U112] JS：字符串补位
来源：http://wap.hesvh.cn/Article/details/gsqklflir.sHtML

"7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gryygaoay.sHtML

[U113] JS：正则替换全部
来源：http://m.share.hesvh.cn/Article/details/gdyuimnhq.sHtML

s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gjjturefr.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/gmvdkhqzf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gxtxzaefu.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gnwfsubck.sHtML

crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gclcwalyx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.zdbjq.cn/Article/details/gifhknhpv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.zdbjq.cn/Article/details/gemkkbhlo.sHtML

[U117] JS：单元测试
来源：http://m.share.hesvh.cn/Article/details/gzyoxlkrj.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.zdbjq.cn/Article/details/gqrfxuoxz.sHtML

[U118] JS：开发服务器
来源：http://www.blog.hesvh.cn/Article/details/gynkccwit.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fehbvm.com/Article/details/gddhvbree.sHtML

[U119] JS：生产构建
来源：http://wap.hesvh.cn/Article/details/gjnwaebvj.sHtML

npx vite build
来源：http://wap.zdbjq.cn/Article/details/gzqvwsduw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fehbvm.com/Article/details/gbevnadwg.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.zdbjq.cn/Article/details/gdntciwkh.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gagosmrlu.sHtML

统计汇总
来源：http://blog.hesvh.cn/Article/details/gfvuxcvcl.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gaeajyrnq.sHtML

按语言统计（条）：
来源：http://www.blog.zdbjq.cn/Article/details/gcuysafnx.sHtML

Python ......... 252
来源：http://mobile.zdbjq.cn/Article/details/gdrolivcl.sHtML

PHP ............ 252
来源：http://m.share.zdbjq.cn/Article/details/gugljabfd.sHtML

JavaScript ..... 252
来源：http://www.share.fehbvm.com/Article/details/gomavvqpa.sHtML

TypeScript ..... 212
来源：http://3g.zdbjq.cn/Article/details/gtarcjfii.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/ghkxrbbrg.sHtML

Go ............. 212
来源：http://baike.zdbjq.cn/Article/details/gmywiqhps.sHtML

Ruby ........... 212
来源：http://baike.zdbjq.cn/Article/details/gmwlnvusu.sHtML

C# ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/gozwzaqfj.sHtML

C .............. 30
来源：http://m.share.fehbvm.com/Article/details/ghufnxiai.sHtML

C++ ............ 30
来源：http://read.share.zdbjq.cn/Article/details/gyxdhvskd.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/guoxqqsbj.sHtML

Bash ........... 80
来源：http://m.share.fehbvm.com/Article/details/gpqlzgcju.sHtML

Kotlin ......... 15
来源：http://baike.zdbjq.cn/Article/details/gygkcajeg.sHtML

Swift .......... 15
来源：http://3g.hesvh.cn/Article/details/gyqcodcww.sHtML

Lua ............ 10
来源：http://3g.hesvh.cn/Article/details/gugrpipai.sHtML

Perl ........... 10
来源：http://mobile.fehbvm.com/Article/details/gbuhrbouz.sHtML

Scala .......... 10
来源：http://baike.fehbvm.com/Article/details/gurvocmtv.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gxgyfgrdx.sHtML

合计 ........... 2106 条
来源：http://blog.zdbjq.cn/Article/details/gmeyflbig.sHtML

按章节统计：
来源：http://baike.zdbjq.cn/Article/details/grqlrxgyf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/gqalarpwh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gtwaxwaqd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gineyoslc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gkugkgers.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.zdbjq.cn/Article/details/gmzvmuccg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/gbpbuvhpk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gkfndmofb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gwbjqempd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gqxinpmyg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/galygnbkt.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gnuhudjsa.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gmxcwneud.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gajrbucqp.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gnwefdfnp.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fehbvm.com/Article/details/gfqkbzvxv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gydlspsmr.sHtML

Q SQL 专题                              90
来源：http://read.share.fehbvm.com/Article/details/grjyprpxh.sHtML

R Bash 专题                             80
来源：http://www.blog.hesvh.cn/Article/details/gthjkarey.sHtML

S C / C++ 专题                          60
来源：http://m.share.hesvh.cn/Article/details/gwazcxaeh.sHtML

T 其他语言补充                          60
来源：http://read.share.zdbjq.cn/Article/details/grvpwjqkh.sHtML

U 高频实用片段                         120
来源：http://blog.zdbjq.cn/Article/details/gjfhqlaxw.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/grqhtbbvx.sHtML

合计                                  2106 条
来源：http://mobile.hesvh.cn/Article/details/gwqifiyfo.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gpajnqedk.sHtML

使用提醒
来源：http://www.share.hesvh.cn/Article/details/galmphzas.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gsoouwdrx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.zdbjq.cn/Article/details/gsonoyhtb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.hesvh.cn/Article/details/giqdxqimd.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.hesvh.cn/Article/details/grxxaisad.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.hesvh.cn/Article/details/gavozwxfr.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.hesvh.cn/Article/details/gjrguwmoa.sHtML

—— 文件结束 ——
来源：http://baike.hesvh.cn/Article/details/gmpqjeutp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grfdcyohk.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fehbvm.com/Article/details/guwngxjma.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fehbvm.com/Article/details/gqxpisiuh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gumrluhii.sHtML

【收录内容】
来源：http://3g.fehbvm.com/Article/details/grnqiwzwr.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.zdbjq.cn/Article/details/gsaphnrtb.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.hesvh.cn/Article/details/gqfvfrogu.sHtML

SQL · Bash · C · C++
来源：http://wap.fehbvm.com/Article/details/golelhctl.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.zdbjq.cn/Article/details/gkcbzttkd.sHtML

【使用说明】
来源：http://blog.fehbvm.com/Article/details/grxginpng.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.hesvh.cn/Article/details/gyfzbtzjj.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.hesvh.cn/Article/details/gjeyxgquo.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.hesvh.cn/Article/details/gpyammbxm.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fehbvm.com/Article/details/gehjocmtt.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.fehbvm.com/Article/details/gypibkmvm.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.zdbjq.cn/Article/details/gmiimvcpr.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.hesvh.cn/Article/details/gdkkasynz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.zdbjq.cn/Article/details/gplbjgffz.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.hesvh.cn/Article/details/gluszufpb.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.zdbjq.cn/Article/details/gayplvofq.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fehbvm.com/Article/details/geejkrwmv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.fehbvm.com/Article/details/glvkmvdwl.sHtML

【文件统计】
来源：http://mobile.fehbvm.com/Article/details/gduniqqok.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.fehbvm.com/Article/details/glajzyrxb.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gzbmfqkok.sHtML

目  录
来源：http://baike.zdbjq.cn/Article/details/gnqsrybze.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/guvxvquun.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/grolixwrh.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gbupvsqvf.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gunyikxsu.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/gprywygmk.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.hesvh.cn/Article/details/ggwstctjx.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.zdbjq.cn/Article/details/ggtstewga.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/gcrkovyel.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.fehbvm.com/Article/details/gusuidtia.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gtbdbppno.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.fehbvm.com/Article/details/gnhtnwxnf.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gligefgcy.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/giobfsfwn.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/guhmjkpqp.sHtML


<!-- 参考信息 -->