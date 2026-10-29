代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://mobile.zdbjq.cn/Article/details/gjndqsjah.sHtML

@contextlib.contextmanager
来源：http://3g.zdbjq.cn/Article/details/gmguvmmsy.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fehbvm.com/Article/details/ggjvrrnle.sHtML

list(zip(*m))
来源：http://3g.zdbjq.cn/Article/details/gihkksdrm.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fehbvm.com/Article/details/gpbkrjbgd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.hesvh.cn/Article/details/gvzecynjv.sHtML

[U24] Py：路径操作
来源：http://www.share.zdbjq.cn/Article/details/gwmuaelkz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gjjzdnszk.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fehbvm.com/Article/details/gcqlbtdnm.sHtML

csv.DictReader(f)
来源：http://www.m.share.hesvh.cn/Article/details/gmonkfsyq.sHtML

[U26] Py：并发下载
来源：http://www.blog.zdbjq.cn/Article/details/gwjwadwpv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.hesvh.cn/Article/details/gcparnsru.sHtML

[U27] Py：异步 HTTP
来源：http://3g.hesvh.cn/Article/details/gamfakxoa.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.hesvh.cn/Article/details/gafyjvuja.sHtML

[U28] Py：类型别名
来源：http://3g.hesvh.cn/Article/details/gbyoibcty.sHtML

UserId = int
来源：http://mobile.zdbjq.cn/Article/details/govopksam.sHtML

[U29] Py：属性校验
来源：http://www.m.share.zdbjq.cn/Article/details/gulwbleyj.sHtML

@property 与 @x.setter 配合
来源：http://3g.hesvh.cn/Article/details/gigzodnxr.sHtML

[U30] Py：数据类
来源：http://blog.hesvh.cn/Article/details/gddnpdhac.sHtML

@dataclass(slots=True)
来源：http://3g.fehbvm.com/Article/details/gwrpwpezr.sHtML

[U31] Py：单测
来源：http://read.share.fehbvm.com/Article/details/gpfjapxfq.sHtML

python -m pytest -q
来源：http://3g.fehbvm.com/Article/details/gnnynrbhu.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/gbxnftbea.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fehbvm.com/Article/details/gpwchilyu.sHtML

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/gnnqiapsw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.zdbjq.cn/Article/details/gqmzznlru.sHtML

[U34] Py：判断编码
来源：http://m.share.zdbjq.cn/Article/details/gqooofmuz.sHtML

chardet.detect(raw)
来源：http://www.share.hesvh.cn/Article/details/ghgxvfqai.sHtML

[U35] Py：发送邮件
来源：http://read.share.hesvh.cn/Article/details/gkawlztgc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fehbvm.com/Article/details/gyasxfusu.sHtML

[U36] Py：定时任务
来源：http://www.blog.hesvh.cn/Article/details/gcteyskdl.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.hesvh.cn/Article/details/ggbttqzae.sHtML

[U37] Py：读写 Excel
来源：http://read.share.zdbjq.cn/Article/details/gwixeyzfy.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.hesvh.cn/Article/details/gxqkdtqzg.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/gujmdhzuk.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.zdbjq.cn/Article/details/gqbsdqwje.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.hesvh.cn/Article/details/gqxmixror.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fehbvm.com/Article/details/gsnwggael.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.zdbjq.cn/Article/details/gczqagcph.sHtML

print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/ginlxdhxs.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fehbvm.com/Article/details/glwvpztnu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fehbvm.com/Article/details/gszgtnvah.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.hesvh.cn/Article/details/gnnahvhpk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.zdbjq.cn/Article/details/gbosvtwnq.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gdlmagdid.sHtML

namespace App\Http;
来源：http://blog.zdbjq.cn/Article/details/gfvetrjsr.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.zdbjq.cn/Article/details/gimlgxnoz.sHtML

declare(strict_types=1);
来源：http://baike.fehbvm.com/Article/details/gbdxotatj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fehbvm.com/Article/details/gnyqzfuwa.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gtdddksuz.sHtML

[U46] PHP：可空类型
来源：http://www.share.zdbjq.cn/Article/details/gdubvxfgo.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/gppuvufgu.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fehbvm.com/Article/details/gcylejvmy.sHtML

int|string $id
来源：http://blog.zdbjq.cn/Article/details/gvszulbkv.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fehbvm.com/Article/details/ggwfnwqos.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.zdbjq.cn/Article/details/grkruzsiz.sHtML

[U49] PHP：只读属性
来源：http://www.share.fehbvm.com/Article/details/gdasehuez.sHtML

public readonly string $name
来源：http://www.share.fehbvm.com/Article/details/gkiyhwtzi.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.hesvh.cn/Article/details/gltyzvrwq.sHtML

public function __construct(private int $id) {}
来源：http://blog.fehbvm.com/Article/details/gyzycukub.sHtML

[U51] PHP：数组解构
来源：http://www.share.zdbjq.cn/Article/details/gzffbwoju.sHtML

[$a, $b] = $arr;
来源：http://m.share.zdbjq.cn/Article/details/gjbcfjqpn.sHtML

[U52] PHP：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gapwjgvuq.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.hesvh.cn/Article/details/gfetincue.sHtML

[U53] PHP：空合并运算符
来源：http://3g.hesvh.cn/Article/details/gohoabeed.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.zdbjq.cn/Article/details/gvnimbsah.sHtML

[U54] PHP：空安全调用
来源：http://3g.hesvh.cn/Article/details/gpbffqzkj.sHtML

$obj?->method()
来源：http://read.share.zdbjq.cn/Article/details/gboasvgpy.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fehbvm.com/Article/details/gpjsovmre.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fehbvm.com/Article/details/ganumwhtw.sHtML

[U56] PHP：命名参数
来源：http://3g.zdbjq.cn/Article/details/gzemifauw.sHtML

f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gjyvnlezq.sHtML

[U57] PHP：字符串插值
来源：http://baike.hesvh.cn/Article/details/gltmqfitn.sHtML

"值: {$a}"
来源：http://blog.zdbjq.cn/Article/details/grzimqiqs.sHtML

[U58] PHP：数组三件套
来源：http://blog.hesvh.cn/Article/details/gysxdnned.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.zdbjq.cn/Article/details/gdplqzntz.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fehbvm.com/Article/details/gmzabrtki.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gxwriasca.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.hesvh.cn/Article/details/gkidotswh.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fehbvm.com/Article/details/gdabutozf.sHtML

[U61] PHP：正则
来源：http://blog.fehbvm.com/Article/details/gqopasfup.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/gafxqtywm.sHtML

[U62] PHP：日期对象
来源：http://read.share.hesvh.cn/Article/details/gnhjnqxev.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.hesvh.cn/Article/details/gpdnhecky.sHtML

[U63] PHP：文件读写
来源：http://wap.fehbvm.com/Article/details/gscjlhrpu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.hesvh.cn/Article/details/gidrupkob.sHtML

[U64] PHP：目录遍历
来源：http://3g.fehbvm.com/Article/details/guvuzdsyj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fehbvm.com/Article/details/gwvhjittx.sHtML

[U65] PHP：会话
来源：http://www.m.share.fehbvm.com/Article/details/gmukqhioh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fehbvm.com/Article/details/gmplodkze.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.hesvh.cn/Article/details/gfaacldcx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.zdbjq.cn/Article/details/guyjzvpsb.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.hesvh.cn/Article/details/grarriase.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fehbvm.com/Article/details/gcaqtcxkw.sHtML

[U68] PHP：PDO 连接
来源：http://wap.hesvh.cn/Article/details/gaaovcwjk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fehbvm.com/Article/details/gvpffjpjg.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fehbvm.com/Article/details/gxytxpdif.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fehbvm.com/Article/details/gjlkqeypk.sHtML

[U70] PHP：PDO 事务
来源：http://3g.zdbjq.cn/Article/details/gkllqjugp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.zdbjq.cn/Article/details/gmfgfnxgy.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gefrqxzmu.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.hesvh.cn/Article/details/guxifvusv.sHtML

[U72] PHP：写错误日志
来源：http://wap.hesvh.cn/Article/details/gwmynufdg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fehbvm.com/Article/details/gcbiiuaxj.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.zdbjq.cn/Article/details/gmmkrfcuo.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fehbvm.com/Article/details/gohrfovtd.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gxmaesqkp.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fehbvm.com/Article/details/gcgadwtni.sHtML

[U75] PHP：依赖注入
来源：http://baike.fehbvm.com/Article/details/goakwsgyy.sHtML

composer require psr/container
来源：http://read.share.zdbjq.cn/Article/details/gjrfhnhpz.sHtML

[U76] PHP：简单路由
来源：http://m.share.fehbvm.com/Article/details/gwfrlbzek.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.hesvh.cn/Article/details/gbnczoebk.sHtML

[U77] PHP：模板渲染
来源：http://baike.fehbvm.com/Article/details/gwcdhtnqv.sHtML

composer require twig/twig
来源：http://www.blog.hesvh.cn/Article/details/gbzuyowad.sHtML

[U78] PHP：单元测试
来源：http://mobile.hesvh.cn/Article/details/gmkqxfabc.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fehbvm.com/Article/details/gibgwvjrw.sHtML

[U79] PHP：静态分析
来源：http://3g.zdbjq.cn/Article/details/gahqlxxdd.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.zdbjq.cn/Article/details/gseafmkpv.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.hesvh.cn/Article/details/gecebqvpq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.hesvh.cn/Article/details/gyrcijbop.sHtML

[U81] JS：初始化项目
来源：http://read.share.fehbvm.com/Article/details/gxjuhpjwj.sHtML

npm init -y;  npm i express
来源：http://read.share.fehbvm.com/Article/details/ggelwfxoz.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.zdbjq.cn/Article/details/gnzjlxsie.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.hesvh.cn/Article/details/gigytmxjz.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.hesvh.cn/Article/details/gqtfuykqq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gtwmlxceg.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fehbvm.com/Article/details/gbconihcn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.hesvh.cn/Article/details/glarxfvkg.sHtML

[U85] JS：可选链
来源：http://www.blog.fehbvm.com/Article/details/gyoukebqj.sHtML

a?.b?.c
来源：http://wap.zdbjq.cn/Article/details/gaknvorcx.sHtML

[U86] JS：空值合并
来源：http://www.share.hesvh.cn/Article/details/gsemvikip.sHtML

a ?? b
来源：http://blog.hesvh.cn/Article/details/genwirzgp.sHtML

[U87] JS：解构默认值
来源：http://blog.fehbvm.com/Article/details/gkpsqzgpn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fehbvm.com/Article/details/gpdtakqov.sHtML

[U88] JS：对象展开合并
来源：http://read.share.zdbjq.cn/Article/details/gpnxmbern.sHtML

{ ...a, ...b }
来源：http://read.share.zdbjq.cn/Article/details/guzaoodzo.sHtML

[U89] JS：数组去重
来源：http://mobile.hesvh.cn/Article/details/gpzwbrqir.sHtML

[...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gnrzgpbtp.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fehbvm.com/Article/details/gxdvxlbuc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gghrsbwob.sHtML

[U91] JS：对象键值遍历
来源：http://3g.zdbjq.cn/Article/details/gdjvwtqsr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fehbvm.com/Article/details/gxjvusxmj.sHtML

[U92] JS：深拷贝
来源：http://3g.fehbvm.com/Article/details/gdrcdscko.sHtML

structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gfhvayheb.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fehbvm.com/Article/details/gxevncxgm.sHtML

`共 ${n} 条`
来源：http://wap.hesvh.cn/Article/details/gvnauhtvz.sHtML

[U94] JS：箭头函数
来源：http://wap.hesvh.cn/Article/details/gnbmexfzv.sHtML

const double = x => x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gklgxmuht.sHtML

[U95] JS：Promise 包装
来源：http://mobile.hesvh.cn/Article/details/gtiqafmdr.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fehbvm.com/Article/details/gdmegwagz.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.hesvh.cn/Article/details/ghikcrecs.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gvzlrwsgm.sHtML

[U97] JS：并发请求
来源：http://wap.zdbjq.cn/Article/details/gjadxvixe.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/grxpqmlho.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gnilqsvbh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.zdbjq.cn/Article/details/goccgjmri.sHtML

[U99] JS：事件监听
来源：http://www.share.zdbjq.cn/Article/details/glphpyzst.sHtML

el.addEventListener("click", e => {})
来源：http://baike.zdbjq.cn/Article/details/geqwglgrs.sHtML

[U100] JS：DOM 查询
来源：http://baike.zdbjq.cn/Article/details/gwqlxsiii.sHtML

document.querySelector(".item")
来源：http://baike.hesvh.cn/Article/details/gdlklprhs.sHtML

[U101] JS：classList 操作
来源：http://www.blog.zdbjq.cn/Article/details/gscmaekmi.sHtML

el.classList.toggle("active")
来源：http://mobile.zdbjq.cn/Article/details/gynleywzu.sHtML

[U102] JS：本地存储
来源：http://blog.fehbvm.com/Article/details/gcdomixzi.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fehbvm.com/Article/details/gwjiymsmf.sHtML

[U103] JS：定时器
来源：http://mobile.hesvh.cn/Article/details/gravkeztq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fehbvm.com/Article/details/gnleuzxzp.sHtML

[U104] JS：防抖
来源：http://wap.fehbvm.com/Article/details/gwpyhijfn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gbmnweogl.sHtML

[U105] JS：节流
来源：http://read.share.fehbvm.com/Article/details/gagpfalfi.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fehbvm.com/Article/details/gafryykfs.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gobztzpyl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fehbvm.com/Article/details/gqzvgaqxc.sHtML

[U107] JS：数字千分位
来源：http://read.share.fehbvm.com/Article/details/gfuqffxsh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gnqlkwyvb.sHtML

[U108] JS：随机整数
来源：http://blog.zdbjq.cn/Article/details/gwugvzbvi.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/glwrpbvan.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fehbvm.com/Article/details/gpkiwdjpg.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gwbulslhg.sHtML

[U110] JS：数组分块
来源：http://blog.hesvh.cn/Article/details/gthnbdjkd.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.zdbjq.cn/Article/details/gxevfnafi.sHtML

[U111] JS：对象转 Map
来源：http://wap.hesvh.cn/Article/details/gvmjmkgbn.sHtML

new Map(Object.entries(obj))
来源：http://m.share.zdbjq.cn/Article/details/gklbcrjbj.sHtML

[U112] JS：字符串补位
来源：http://3g.hesvh.cn/Article/details/gqixxjhbf.sHtML

"7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gudprjxxk.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fehbvm.com/Article/details/gcxmdeoxj.sHtML

s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gnwsuekcd.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.zdbjq.cn/Article/details/grmryuxkz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gcgrgymdh.sHtML

[U115] JS：生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gtjfisfag.sHtML

crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gpdynzzvz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.hesvh.cn/Article/details/gfljjkztv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.hesvh.cn/Article/details/glbjapwzz.sHtML

[U117] JS：单元测试
来源：http://read.share.fehbvm.com/Article/details/gdrigbxzu.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fehbvm.com/Article/details/gvnoogbht.sHtML

[U118] JS：开发服务器
来源：http://www.share.hesvh.cn/Article/details/ghkmkhlhd.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fehbvm.com/Article/details/gaemsunaa.sHtML

[U119] JS：生产构建
来源：http://www.share.hesvh.cn/Article/details/gqumrmuci.sHtML

npx vite build
来源：http://baike.fehbvm.com/Article/details/gavhzcesv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.hesvh.cn/Article/details/gdgbzmkqq.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.hesvh.cn/Article/details/gmssnsixv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/guigcdfeb.sHtML

统计汇总
来源：http://read.share.hesvh.cn/Article/details/gtlcxldym.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyjlwgovm.sHtML

按语言统计（条）：
来源：http://mobile.zdbjq.cn/Article/details/gkhaoyrhz.sHtML

Python ......... 252
来源：http://blog.fehbvm.com/Article/details/ghniutxlo.sHtML

PHP ............ 252
来源：http://read.share.hesvh.cn/Article/details/gomvxzgqd.sHtML

JavaScript ..... 252
来源：http://wap.fehbvm.com/Article/details/gwjfgfohg.sHtML

TypeScript ..... 212
来源：http://3g.zdbjq.cn/Article/details/gppsocuyk.sHtML

Java ........... 212
来源：http://www.share.fehbvm.com/Article/details/gbcjgyuho.sHtML

Go ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gvopeqjai.sHtML

Ruby ........... 212
来源：http://mobile.hesvh.cn/Article/details/ggovdqjzk.sHtML

C# ............. 212
来源：http://mobile.fehbvm.com/Article/details/grgfkapxh.sHtML

C .............. 30
来源：http://read.share.zdbjq.cn/Article/details/gskgwtifg.sHtML

C++ ............ 30
来源：http://m.share.zdbjq.cn/Article/details/gqsmvyhvx.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/gasgrctqn.sHtML

Bash ........... 80
来源：http://3g.fehbvm.com/Article/details/gwlsaisvt.sHtML

Kotlin ......... 15
来源：http://www.blog.hesvh.cn/Article/details/gyyhoivjq.sHtML

Swift .......... 15
来源：http://read.share.fehbvm.com/Article/details/gljvdmxof.sHtML

Lua ............ 10
来源：http://blog.fehbvm.com/Article/details/gcvtnwqev.sHtML

Perl ........... 10
来源：http://read.share.hesvh.cn/Article/details/guxowlmjb.sHtML

Scala .......... 10
来源：http://3g.zdbjq.cn/Article/details/gswjdvavr.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/gkjipwmbk.sHtML

合计 ........... 2106 条
来源：http://www.blog.fehbvm.com/Article/details/gztrnzixg.sHtML

按章节统计：
来源：http://read.share.zdbjq.cn/Article/details/gabfnziss.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/grurcdlsx.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gtkbnjuwz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/ggpgijjti.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/grauibxlz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.hesvh.cn/Article/details/gckypylvf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gxbneqdmx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gwlpnhszc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gjqqufozp.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/guicrgpxw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gkgrnxubf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gbbihymql.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gzvxqtxuu.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gxmwrpdaa.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gautekxiq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fehbvm.com/Article/details/grojgakhm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gxzprvxqj.sHtML

Q SQL 专题                              90
来源：http://m.share.zdbjq.cn/Article/details/gdyqreuyq.sHtML

R Bash 专题                             80
来源：http://www.m.share.hesvh.cn/Article/details/gsjxugrqs.sHtML

S C / C++ 专题                          60
来源：http://read.share.hesvh.cn/Article/details/girahngmn.sHtML

T 其他语言补充                          60
来源：http://m.share.fehbvm.com/Article/details/gifgyjvdl.sHtML

U 高频实用片段                         120
来源：http://www.blog.fehbvm.com/Article/details/gdkaeqwzd.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/glblncvhg.sHtML

合计                                  2106 条
来源：http://read.share.zdbjq.cn/Article/details/ghkvkmsvo.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/geojirhxx.sHtML

使用提醒
来源：http://wap.hesvh.cn/Article/details/goorsbogr.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gkkgamujn.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fehbvm.com/Article/details/gbwbqqbrc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fehbvm.com/Article/details/gjolfxnfi.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.hesvh.cn/Article/details/gfoybylcw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.zdbjq.cn/Article/details/gyilkvrkc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fehbvm.com/Article/details/gqknsrava.sHtML

—— 文件结束 ——
来源：http://mobile.hesvh.cn/Article/details/gwsyayxxm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gasofzzvi.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.zdbjq.cn/Article/details/grzbbheiv.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fehbvm.com/Article/details/guhjcsgot.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/giurtgbxh.sHtML

【收录内容】
来源：http://read.share.zdbjq.cn/Article/details/gpmrzbboi.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.zdbjq.cn/Article/details/gvbaffdpb.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.hesvh.cn/Article/details/gbfcpmwbc.sHtML

SQL · Bash · C · C++
来源：http://wap.fehbvm.com/Article/details/gdmoimqvi.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.hesvh.cn/Article/details/gzsxvjxhs.sHtML

【使用说明】
来源：http://read.share.hesvh.cn/Article/details/ghtawuept.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.fehbvm.com/Article/details/goqcmrcxc.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fehbvm.com/Article/details/gayjqfwff.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.zdbjq.cn/Article/details/goorycuwk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.zdbjq.cn/Article/details/gjkaspzxf.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.hesvh.cn/Article/details/glsaeowqi.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.hesvh.cn/Article/details/gehseiwbr.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.zdbjq.cn/Article/details/gkeicuobf.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fehbvm.com/Article/details/gwnzmhbwl.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.hesvh.cn/Article/details/geoigumua.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fehbvm.com/Article/details/ganlafpla.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.zdbjq.cn/Article/details/ghisfkxuc.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.zdbjq.cn/Article/details/gupwzqobc.sHtML

【文件统计】
来源：http://www.m.share.hesvh.cn/Article/details/gpiilrqrz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.hesvh.cn/Article/details/gdxzbvrai.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gnxnxhbrz.sHtML

目  录
来源：http://m.share.zdbjq.cn/Article/details/gzmshggnc.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gewetsddz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/gzfbgqivv.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gimgmiwll.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gronbbqvo.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.hesvh.cn/Article/details/gtlaziskm.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fehbvm.com/Article/details/gteggeacn.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/gcmqnfvoo.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gwtymjhpi.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.hesvh.cn/Article/details/gvdrobmtr.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gjfjocnsc.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.zdbjq.cn/Article/details/gbxhqdmxx.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gofpxcbcf.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gioaqfyby.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gmsjpjplt.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/grimrbluz.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.hesvh.cn/Article/details/glhvvsowr.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gphjpyafh.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.hesvh.cn/Article/details/gocfqxmro.sHtML


<!-- 参考信息 -->