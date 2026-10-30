代发 wailian999

[U25] Py：CSV 按字典读
来源：http://3g.fanxiaobao.xyz/Article/details/gwnebkuim.sHtML

csv.DictReader(f)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjefkdtn.sHtML

[U26] Py：并发下载
来源：http://3g.fanxiaobao.xyz/Article/details/gquhiyeja.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fanxiaobao.xyz/Article/details/gznfibolj.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjcijhpo.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fanxiaobao.xyz/Article/details/geeujhxqj.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnaqbirk.sHtML

UserId = int
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqzldgni.sHtML

[U29] Py：属性校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gpijmkqbs.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fanxiaobao.xyz/Article/details/gjyjqliyo.sHtML

[U30] Py：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gobthkhtf.sHtML

@dataclass(slots=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gddpakbtt.sHtML

[U31] Py：单测
来源：http://blog.fanxiaobao.xyz/Article/details/gjmbqjcgg.sHtML

python -m pytest -q
来源：http://3g.fanxiaobao.xyz/Article/details/gsmktjgjb.sHtML

[U32] Py：代码格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gagyylsyl.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fanxiaobao.xyz/Article/details/gouwlnmxd.sHtML

[U33] Py：打包发布
来源：http://read.share.fanxiaobao.xyz/Article/details/givfttgen.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryivpkrm.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrgihwov.sHtML

chardet.detect(raw)
来源：http://wap.fanxiaobao.xyz/Article/details/gjdnivnkj.sHtML

[U35] Py：发送邮件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvpnxcfa.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwsgcdtln.sHtML

[U36] Py：定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfigeqtn.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjltikrac.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gayvtenyq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkvagupl.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzhpquxq.sHtML

Path(__file__).resolve().parent
来源：http://blog.fanxiaobao.xyz/Article/details/gtaragiwy.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhfoseyc.sHtML

sys.stdout.isatty()
来源：http://baike.fanxiaobao.xyz/Article/details/gciiheklb.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gdiehxajc.sHtML

print("err", file=sys.stderr)
来源：http://baike.fanxiaobao.xyz/Article/details/gvznacgda.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvpkivre.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmwuiwxa.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqabpeft.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fanxiaobao.xyz/Article/details/gtirnjklj.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbozgjwq.sHtML

namespace App\Http;
来源：http://www.share.fanxiaobao.xyz/Article/details/gplfbzopc.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfuapxdd.sHtML

declare(strict_types=1);
来源：http://wap.fanxiaobao.xyz/Article/details/gfjmdnnvq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppkfrluw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbgfyoufs.sHtML

[U46] PHP：可空类型
来源：http://wap.fanxiaobao.xyz/Article/details/gvyiglqdv.sHtML

?string $name = null
来源：http://wap.fanxiaobao.xyz/Article/details/gvpogtboy.sHtML

[U47] PHP：联合类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyavcjis.sHtML

int|string $id
来源：http://3g.fanxiaobao.xyz/Article/details/glkeoyusa.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfvumeqn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvhhvkiq.sHtML

[U49] PHP：只读属性
来源：http://wap.fanxiaobao.xyz/Article/details/gdusxntnx.sHtML

public readonly string $name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntbrrcay.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fanxiaobao.xyz/Article/details/gnrvnxpny.sHtML

public function __construct(private int $id) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gnhtwdpgo.sHtML

[U51] PHP：数组解构
来源：http://wap.fanxiaobao.xyz/Article/details/gnumclxnk.sHtML

[$a, $b] = $arr;
来源：http://wap.fanxiaobao.xyz/Article/details/gyruhzoum.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvhuxlrk.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goetgcjmi.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fanxiaobao.xyz/Article/details/glnyiyevk.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fanxiaobao.xyz/Article/details/goifrbdcc.sHtML

[U54] PHP：空安全调用
来源：http://baike.fanxiaobao.xyz/Article/details/gkuiglbtk.sHtML

$obj?->method()
来源：http://wap.fanxiaobao.xyz/Article/details/gzldlacdm.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gzztcmlqz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fanxiaobao.xyz/Article/details/gzshettwp.sHtML

[U56] PHP：命名参数
来源：http://blog.fanxiaobao.xyz/Article/details/ghuxftpik.sHtML

f(a: 1, b: 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaokwuilw.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gejoppvwx.sHtML

"值: {$a}"
来源：http://baike.fanxiaobao.xyz/Article/details/glevpeklj.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgratbml.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gmeivysmx.sHtML

[U59] PHP：自定义排序
来源：http://3g.fanxiaobao.xyz/Article/details/gazomshdp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gppjuazbd.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fanxiaobao.xyz/Article/details/gsxikxcur.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gbtrkrzrp.sHtML

[U61] PHP：正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gssgeugzm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gbltbhcwk.sHtML

[U62] PHP：日期对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gesdteiij.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fanxiaobao.xyz/Article/details/grflzpone.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjysbmvs.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqgovnaa.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gwblzmamj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fanxiaobao.xyz/Article/details/gibqzljzb.sHtML

[U65] PHP：会话
来源：http://3g.fanxiaobao.xyz/Article/details/gesdymqjd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaofxjcbd.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfpqjdeb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmhjjtqt.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fanxiaobao.xyz/Article/details/gyavzivbg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fanxiaobao.xyz/Article/details/gommxdvgz.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsmeudoh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpqsodtb.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fanxiaobao.xyz/Article/details/giozbrilv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fanxiaobao.xyz/Article/details/gonkumsol.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fanxiaobao.xyz/Article/details/geobpumoi.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fanxiaobao.xyz/Article/details/gcsuacdmi.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gpiahglng.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvcppkbx.sHtML

[U72] PHP：写错误日志
来源：http://baike.fanxiaobao.xyz/Article/details/gnssqiqti.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fanxiaobao.xyz/Article/details/gmvcsjfqa.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzrqsxni.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fanxiaobao.xyz/Article/details/gkmjaoysr.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmbrmlwy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fanxiaobao.xyz/Article/details/gtduyfccr.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrthgqmz.sHtML

composer require psr/container
来源：http://m.share.fanxiaobao.xyz/Article/details/gtampxzbe.sHtML

[U76] PHP：简单路由
来源：http://m.share.fanxiaobao.xyz/Article/details/glbmfftfw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fanxiaobao.xyz/Article/details/gprejxskk.sHtML

[U77] PHP：模板渲染
来源：http://blog.fanxiaobao.xyz/Article/details/gojtwaybg.sHtML

composer require twig/twig
来源：http://3g.fanxiaobao.xyz/Article/details/gpnabsrex.sHtML

[U78] PHP：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxxvwelx.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fanxiaobao.xyz/Article/details/gedhvewlc.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkomyjpp.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggaaewkcw.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fanxiaobao.xyz/Article/details/gcpwmyysw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmsxiord.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsbyrmax.sHtML

npm init -y;  npm i express
来源：http://m.share.fanxiaobao.xyz/Article/details/gkctnzyeb.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxjfxrsw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqwoogab.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fanxiaobao.xyz/Article/details/gjpueiymp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fanxiaobao.xyz/Article/details/gbfgjnttf.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpedjmylw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnommnxn.sHtML

[U85] JS：可选链
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpddevqg.sHtML

a?.b?.c
来源：http://baike.fanxiaobao.xyz/Article/details/gdtsusuqj.sHtML

[U86] JS：空值合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqjpievb.sHtML

a ?? b
来源：http://mobile.fanxiaobao.xyz/Article/details/guyxxrwdu.sHtML

[U87] JS：解构默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gycrxwfpg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fanxiaobao.xyz/Article/details/gqdhcgpyg.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gownxlotk.sHtML

{ ...a, ...b }
来源：http://3g.fanxiaobao.xyz/Article/details/gfsnqszjb.sHtML

[U89] JS：数组去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcvpwdxy.sHtML

[...new Set(arr)]
来源：http://3g.fanxiaobao.xyz/Article/details/gfpabegbs.sHtML

[U90] JS：数字数组排序
来源：http://wap.fanxiaobao.xyz/Article/details/gfxvqxhtf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgdycgbt.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gcprrsiej.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fanxiaobao.xyz/Article/details/gzrmobcgk.sHtML

[U92] JS：深拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gibslzlwr.sHtML

structuredClone(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlhtxcfj.sHtML

[U93] JS：模板字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gcltrjkul.sHtML

`共 ${n} 条`
来源：http://blog.fanxiaobao.xyz/Article/details/gyldmbwpo.sHtML

[U94] JS：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gnsrdeocn.sHtML

const double = x => x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkftcjzsp.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fanxiaobao.xyz/Article/details/gtthdgqlc.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fanxiaobao.xyz/Article/details/gpxagulzh.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpvndndf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fanxiaobao.xyz/Article/details/gyynpiikd.sHtML

[U97] JS：并发请求
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgxackzi.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fanxiaobao.xyz/Article/details/gzdzhugtx.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gwyjzndtd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fanxiaobao.xyz/Article/details/grmyapudj.sHtML

[U99] JS：事件监听
来源：http://read.share.fanxiaobao.xyz/Article/details/gccfmyqiv.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fanxiaobao.xyz/Article/details/gxxyzqiqf.sHtML

[U100] JS：DOM 查询
来源：http://blog.fanxiaobao.xyz/Article/details/gzlniqfrl.sHtML

document.querySelector(".item")
来源：http://blog.fanxiaobao.xyz/Article/details/ghsaipfoo.sHtML

[U101] JS：classList 操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzlmkfok.sHtML

el.classList.toggle("active")
来源：http://mobile.fanxiaobao.xyz/Article/details/gziyepiwe.sHtML

[U102] JS：本地存储
来源：http://www.share.fanxiaobao.xyz/Article/details/gjusbicvw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fanxiaobao.xyz/Article/details/gccbcegzn.sHtML

[U103] JS：定时器
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxansdva.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fanxiaobao.xyz/Article/details/gayydbhng.sHtML

[U104] JS：防抖
来源：http://3g.fanxiaobao.xyz/Article/details/gzgswxbvf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gfuqsrwmy.sHtML

[U105] JS：节流
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybrfamxq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkijbcge.sHtML

[U106] JS：日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/grzivjkvc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwlvubjt.sHtML

[U107] JS：数字千分位
来源：http://m.share.fanxiaobao.xyz/Article/details/glzwxdlia.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fanxiaobao.xyz/Article/details/gutwvddmo.sHtML

[U108] JS：随机整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/govnucggk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fanxiaobao.xyz/Article/details/glgbtfqpr.sHtML

[U109] JS：数组分组
来源：http://3g.fanxiaobao.xyz/Article/details/gulscauxo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fanxiaobao.xyz/Article/details/gvahjhxrc.sHtML

[U110] JS：数组分块
来源：http://wap.fanxiaobao.xyz/Article/details/gssgiuljl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fanxiaobao.xyz/Article/details/grgqueuuu.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnbfmudy.sHtML

new Map(Object.entries(obj))
来源：http://baike.fanxiaobao.xyz/Article/details/ghejgdman.sHtML

[U112] JS：字符串补位
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzzbzebn.sHtML

"7".padStart(3, "0")
来源：http://www.share.fanxiaobao.xyz/Article/details/gexlvhssd.sHtML

[U113] JS：正则替换全部
来源：http://3g.fanxiaobao.xyz/Article/details/grtsblwzd.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcgqivdt.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fanxiaobao.xyz/Article/details/guwxepscx.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gazchdrkh.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurrifvmj.sHtML

crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gskvyrawm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fanxiaobao.xyz/Article/details/goiptncrz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gusdstjux.sHtML

[U117] JS：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/gpbvvwber.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvacadux.sHtML

[U118] JS：开发服务器
来源：http://m.share.fanxiaobao.xyz/Article/details/gggzufjuk.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtnjpxbq.sHtML

[U119] JS：生产构建
来源：http://baike.fanxiaobao.xyz/Article/details/gfbvaumoj.sHtML

npx vite build
来源：http://blog.fanxiaobao.xyz/Article/details/gwybswjxc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnunmymw.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxuzzvbc.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gnebjrrzj.sHtML

统计汇总
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqlkibvr.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gcfbvoqcb.sHtML

按语言统计（条）：
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbgjyksc.sHtML

Python ......... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gvmbzaidb.sHtML

PHP ............ 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxpvigrl.sHtML

JavaScript ..... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxdrmxyg.sHtML

TypeScript ..... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gpgumbwtn.sHtML

Java ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/grvgvetuc.sHtML

Go ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgtcmjqd.sHtML

Ruby ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpcpbkfy.sHtML

C# ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/grwgwtzrv.sHtML

C .............. 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkmmknpz.sHtML

C++ ............ 30
来源：http://baike.fanxiaobao.xyz/Article/details/gzwqvbwli.sHtML

SQL ............ 90
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjifraji.sHtML

Bash ........... 80
来源：http://blog.fanxiaobao.xyz/Article/details/gyorkhvid.sHtML

Kotlin ......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfixeyjk.sHtML

Swift .......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebepyfly.sHtML

Lua ............ 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gdigfnxth.sHtML

Perl ........... 10
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfuiilde.sHtML

Scala .......... 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gufugtcjl.sHtML

------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gluonqqkr.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfjugrvf.sHtML

按章节统计：
来源：http://blog.fanxiaobao.xyz/Article/details/glgfxwnfy.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/grfvqtyde.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlghsljv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gvynultgh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/gdniwebvu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fanxiaobao.xyz/Article/details/gooulffyz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkdmnzhp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqwddfwz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fanxiaobao.xyz/Article/details/guambuctk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gghlxwylo.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/gttaprkdf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gjghaoyfn.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdebcoyck.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbiquuyc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fanxiaobao.xyz/Article/details/gttmgeqxg.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnmqurww.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gucvjhohi.sHtML

Q SQL 专题                              90
来源：http://mobile.fanxiaobao.xyz/Article/details/guclxdjxv.sHtML

R Bash 专题                             80
来源：http://3g.fanxiaobao.xyz/Article/details/glnkgynre.sHtML

S C / C++ 专题                          60
来源：http://wap.fanxiaobao.xyz/Article/details/gmcwipyjn.sHtML

T 其他语言补充                          60
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrptzqtd.sHtML

U 高频实用片段                         120
来源：http://wap.fanxiaobao.xyz/Article/details/gksatlidx.sHtML

------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/greqmnbli.sHtML

合计                                  2106 条
来源：http://blog.fanxiaobao.xyz/Article/details/gkoiragcs.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwigcuwy.sHtML

使用提醒
来源：http://wap.fanxiaobao.xyz/Article/details/gwfqelwhy.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/ghgtupvkw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmvioazx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fanxiaobao.xyz/Article/details/gfkiufvki.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdascehuq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fanxiaobao.xyz/Article/details/gvkaqlael.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fanxiaobao.xyz/Article/details/goiwiykfn.sHtML

—— 文件结束 ——
来源：http://blog.fanxiaobao.xyz/Article/details/ggkpgtwrq.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/glngrfesn.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbuaslmn.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fanxiaobao.xyz/Article/details/gzjsjspqi.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gaobktppe.sHtML

【收录内容】
来源：http://blog.fanxiaobao.xyz/Article/details/gzeevrflo.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyuahgsb.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fanxiaobao.xyz/Article/details/gqmbrqbmx.sHtML

SQL · Bash · C · C++
来源：http://www.share.fanxiaobao.xyz/Article/details/glsqveesa.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.fanxiaobao.xyz/Article/details/giqguinxv.sHtML

【使用说明】
来源：http://blog.fanxiaobao.xyz/Article/details/gpxbevvha.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fanxiaobao.xyz/Article/details/gshmipsqi.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdqmybdb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.fanxiaobao.xyz/Article/details/gtyotefwq.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.fanxiaobao.xyz/Article/details/gevkpfdpu.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.fanxiaobao.xyz/Article/details/guifacaax.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.fanxiaobao.xyz/Article/details/gcvpxkjik.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fanxiaobao.xyz/Article/details/gvytcalnm.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnhsmbmm.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.fanxiaobao.xyz/Article/details/guzjziyvu.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.fanxiaobao.xyz/Article/details/gpsaahczu.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnwoeyys.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnmwkzfx.sHtML

【文件统计】
来源：http://www.blog.fanxiaobao.xyz/Article/details/goozmxljj.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.fanxiaobao.xyz/Article/details/ghobksnzt.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggyjucbca.sHtML

目  录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxngwfwl.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gydyjmyiy.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gzasdguwj.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfuirnyri.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.fanxiaobao.xyz/Article/details/goxhyqyja.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gpouejnwa.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.fanxiaobao.xyz/Article/details/grdsazsef.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gmroryrde.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlkbhbnd.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtprhdwz.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftvxnetp.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gqomvojom.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gdctiscoc.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gjonqyirl.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gbphbgrkg.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrbtahjb.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gfeiyjqtq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gedoryycq.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtkvktei.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbvuknbj.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/geocqtkjv.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gvtpkioli.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqdbavia.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gikcagmuw.sHtML

A. 基础语法与类型
来源：http://baike.fanxiaobao.xyz/Article/details/gzuteizsx.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtfdyvoo.sHtML

[A01] Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/glqoibbqa.sHtML


<!-- 参考信息 -->