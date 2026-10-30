代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://m.share.hesvh.cn/Article/details/gdufvsczj.sHtML

@contextlib.contextmanager
来源：http://baike.hesvh.cn/Article/details/gsqhqfcyx.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.zdbjq.cn/Article/details/gweloghpi.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/gkohjiwpo.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fehbvm.com/Article/details/glruxrmew.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.zdbjq.cn/Article/details/gialwwdsm.sHtML

[U24] Py：路径操作
来源：http://www.blog.zdbjq.cn/Article/details/gxprytwdj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gmnzmcqmu.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.hesvh.cn/Article/details/graqaxhgz.sHtML

csv.DictReader(f)
来源：http://m.share.zdbjq.cn/Article/details/gloiabqmz.sHtML

[U26] Py：并发下载
来源：http://baike.hesvh.cn/Article/details/gzvhnslze.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fehbvm.com/Article/details/gagewzekp.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.hesvh.cn/Article/details/gcbjicjcl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.hesvh.cn/Article/details/gfcwifdpm.sHtML

[U28] Py：类型别名
来源：http://blog.fehbvm.com/Article/details/gixqtcnke.sHtML

UserId = int
来源：http://m.share.hesvh.cn/Article/details/gzeolzghs.sHtML

[U29] Py：属性校验
来源：http://mobile.zdbjq.cn/Article/details/gsflmuloo.sHtML

@property 与 @x.setter 配合
来源：http://mobile.zdbjq.cn/Article/details/gvdmadxmv.sHtML

[U30] Py：数据类
来源：http://blog.fehbvm.com/Article/details/gphxebxsr.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/gglozilsr.sHtML

[U31] Py：单测
来源：http://www.blog.hesvh.cn/Article/details/gbbcwnyhh.sHtML

python -m pytest -q
来源：http://read.share.hesvh.cn/Article/details/gmxdtyjdd.sHtML

[U32] Py：代码格式化
来源：http://3g.fehbvm.com/Article/details/gjexjwbvm.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fehbvm.com/Article/details/grlrlthhx.sHtML

[U33] Py：打包发布
来源：http://read.share.fehbvm.com/Article/details/geagrxvca.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.hesvh.cn/Article/details/gsszejehi.sHtML

[U34] Py：判断编码
来源：http://blog.zdbjq.cn/Article/details/gvhtvxtkm.sHtML

chardet.detect(raw)
来源：http://wap.zdbjq.cn/Article/details/gxnedqzks.sHtML

[U35] Py：发送邮件
来源：http://read.share.hesvh.cn/Article/details/gfksuwsfj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fehbvm.com/Article/details/gjoeogftm.sHtML

[U36] Py：定时任务
来源：http://mobile.hesvh.cn/Article/details/gwbmmtcfp.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.zdbjq.cn/Article/details/gcwsmroap.sHtML

[U37] Py：读写 Excel
来源：http://baike.fehbvm.com/Article/details/gwlwgyjwx.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.hesvh.cn/Article/details/gllyauvyg.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.zdbjq.cn/Article/details/gacjmofbx.sHtML

Path(__file__).resolve().parent
来源：http://baike.hesvh.cn/Article/details/gsyguccuk.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.hesvh.cn/Article/details/guyuwpxug.sHtML

sys.stdout.isatty()
来源：http://mobile.hesvh.cn/Article/details/gdnfdttsl.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fehbvm.com/Article/details/ghrrfsirl.sHtML

print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gozlasscn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.hesvh.cn/Article/details/gvijcwijk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.zdbjq.cn/Article/details/grjbjzrpu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.zdbjq.cn/Article/details/gfpxcbkdu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.zdbjq.cn/Article/details/gaakfgbxz.sHtML

[U43] PHP：声明命名空间
来源：http://baike.zdbjq.cn/Article/details/gkgzkhbar.sHtML

namespace App\Http;
来源：http://www.share.zdbjq.cn/Article/details/gliaqjlkd.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.zdbjq.cn/Article/details/gklepodco.sHtML

declare(strict_types=1);
来源：http://www.m.share.zdbjq.cn/Article/details/gqqnbwovk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.hesvh.cn/Article/details/gyghoftlb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gaswutfdj.sHtML

[U46] PHP：可空类型
来源：http://wap.fehbvm.com/Article/details/gqkrcjdvk.sHtML

?string $name = null
来源：http://mobile.hesvh.cn/Article/details/gwgucjkid.sHtML

[U47] PHP：联合类型
来源：http://wap.hesvh.cn/Article/details/gmzxvknkl.sHtML

int|string $id
来源：http://www.share.hesvh.cn/Article/details/gbymmakwg.sHtML

[U48] PHP：纯枚举
来源：http://read.share.hesvh.cn/Article/details/gpmfusxxu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fehbvm.com/Article/details/grlbzjggv.sHtML

[U49] PHP：只读属性
来源：http://wap.zdbjq.cn/Article/details/gsooaztmk.sHtML

public readonly string $name
来源：http://www.blog.zdbjq.cn/Article/details/glvrwgxxm.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.hesvh.cn/Article/details/gnqtniujy.sHtML

public function __construct(private int $id) {}
来源：http://www.share.hesvh.cn/Article/details/gmwgsised.sHtML

[U51] PHP：数组解构
来源：http://3g.hesvh.cn/Article/details/gmtgtayjy.sHtML

[$a, $b] = $arr;
来源：http://blog.zdbjq.cn/Article/details/ggawhksyo.sHtML

[U52] PHP：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gbiupxbfu.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.zdbjq.cn/Article/details/garqhmlhn.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.hesvh.cn/Article/details/gxeutlnzm.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.hesvh.cn/Article/details/gvugbkvbe.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fehbvm.com/Article/details/gancaeauf.sHtML

$obj?->method()
来源：http://mobile.hesvh.cn/Article/details/gnzcrezar.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fehbvm.com/Article/details/gjehpfqld.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fehbvm.com/Article/details/gfmlrahcl.sHtML

[U56] PHP：命名参数
来源：http://read.share.fehbvm.com/Article/details/gfqjtaytd.sHtML

f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gytlfwqaj.sHtML

[U57] PHP：字符串插值
来源：http://wap.hesvh.cn/Article/details/gmmqztobi.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/gayjbmjkt.sHtML

[U58] PHP：数组三件套
来源：http://3g.hesvh.cn/Article/details/ghhxpruvj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.zdbjq.cn/Article/details/ghaveztll.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fehbvm.com/Article/details/gkoolnzqd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gjtorxdrv.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.hesvh.cn/Article/details/gqkgzdgsg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.zdbjq.cn/Article/details/geribqvwn.sHtML

[U61] PHP：正则
来源：http://mobile.zdbjq.cn/Article/details/gnomscomo.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/ghcolhavo.sHtML

[U62] PHP：日期对象
来源：http://m.share.hesvh.cn/Article/details/gjugxhkhq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fehbvm.com/Article/details/gydhuimcw.sHtML

[U63] PHP：文件读写
来源：http://wap.fehbvm.com/Article/details/gcppvkiax.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.zdbjq.cn/Article/details/geswonpxq.sHtML

[U64] PHP：目录遍历
来源：http://wap.hesvh.cn/Article/details/gwpcdwjom.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fehbvm.com/Article/details/gunsryhci.sHtML

[U65] PHP：会话
来源：http://m.share.zdbjq.cn/Article/details/gmprdlbhh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fehbvm.com/Article/details/gccwcazmf.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.zdbjq.cn/Article/details/gppaclscy.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.hesvh.cn/Article/details/gilmzghuw.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.hesvh.cn/Article/details/gxajmwepd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.hesvh.cn/Article/details/ghrurzgmt.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.hesvh.cn/Article/details/gfgqlkbuu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fehbvm.com/Article/details/gtbdkouju.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fehbvm.com/Article/details/gjlgllmeb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.hesvh.cn/Article/details/grktcmeur.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fehbvm.com/Article/details/ginedibxm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.zdbjq.cn/Article/details/gwpxbsuol.sHtML

[U71] PHP：抛出异常
来源：http://m.share.hesvh.cn/Article/details/ghahgnviw.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fehbvm.com/Article/details/getszaqph.sHtML

[U72] PHP：写错误日志
来源：http://wap.fehbvm.com/Article/details/gwnsfltcr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fehbvm.com/Article/details/gkycfwiky.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.hesvh.cn/Article/details/gnzfrdwyf.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fehbvm.com/Article/details/gaymciwbn.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gpebzsalc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fehbvm.com/Article/details/ggyhdtutz.sHtML

[U75] PHP：依赖注入
来源：http://www.share.hesvh.cn/Article/details/gddjcreba.sHtML

composer require psr/container
来源：http://mobile.hesvh.cn/Article/details/gkxdypvmk.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.zdbjq.cn/Article/details/ghfyaoeuj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.zdbjq.cn/Article/details/gvqiduxum.sHtML

[U77] PHP：模板渲染
来源：http://www.share.zdbjq.cn/Article/details/guwvpovzi.sHtML

composer require twig/twig
来源：http://www.blog.fehbvm.com/Article/details/gigbzybxg.sHtML

[U78] PHP：单元测试
来源：http://baike.fehbvm.com/Article/details/grslxjhzn.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.hesvh.cn/Article/details/gcctrbmza.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.hesvh.cn/Article/details/gndfppvax.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.hesvh.cn/Article/details/gwzotdtnx.sHtML

[U80] PHP：代码规范修复
来源：http://wap.hesvh.cn/Article/details/glnofiney.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fehbvm.com/Article/details/gqzqlqxkx.sHtML

[U81] JS：初始化项目
来源：http://www.share.zdbjq.cn/Article/details/gvlmihonp.sHtML

npm init -y;  npm i express
来源：http://wap.fehbvm.com/Article/details/gaqdgzvzl.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.zdbjq.cn/Article/details/grohlhbhn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fehbvm.com/Article/details/gchwvsamc.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fehbvm.com/Article/details/ghdurebaq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gfxzqoxqi.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fehbvm.com/Article/details/gqkkyjbse.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.zdbjq.cn/Article/details/gchwxmpuo.sHtML

[U85] JS：可选链
来源：http://www.m.share.fehbvm.com/Article/details/gwbobqroj.sHtML

a?.b?.c
来源：http://mobile.hesvh.cn/Article/details/gwimuautz.sHtML

[U86] JS：空值合并
来源：http://baike.zdbjq.cn/Article/details/ggegwywsf.sHtML

a ?? b
来源：http://wap.hesvh.cn/Article/details/gqnhxxwsb.sHtML

[U87] JS：解构默认值
来源：http://www.share.hesvh.cn/Article/details/gcmadqvkq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.hesvh.cn/Article/details/glnrvmxpj.sHtML

[U88] JS：对象展开合并
来源：http://wap.fehbvm.com/Article/details/gmrpfgzwb.sHtML

{ ...a, ...b }
来源：http://www.m.share.fehbvm.com/Article/details/gozyvyryf.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/gxyhxqtqe.sHtML

[...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gapuobmiu.sHtML

[U90] JS：数字数组排序
来源：http://mobile.hesvh.cn/Article/details/gugzpajzi.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gnbpoclag.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.zdbjq.cn/Article/details/gfnyskjld.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.zdbjq.cn/Article/details/gzszfkbjc.sHtML

[U92] JS：深拷贝
来源：http://blog.zdbjq.cn/Article/details/gkkrgjzcr.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/ggmepwffw.sHtML

[U93] JS：模板字符串
来源：http://blog.hesvh.cn/Article/details/giripgnyd.sHtML

`共 ${n} 条`
来源：http://baike.hesvh.cn/Article/details/gldiepqxz.sHtML

[U94] JS：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gochvyull.sHtML

const double = x => x * 2;
来源：http://3g.hesvh.cn/Article/details/gtltcdezd.sHtML

[U95] JS：Promise 包装
来源：http://m.share.zdbjq.cn/Article/details/gjumqhyjq.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.hesvh.cn/Article/details/ggmgbwzyd.sHtML

[U96] JS：async/await 与异常
来源：http://3g.hesvh.cn/Article/details/gyulzvypm.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/grfbntibj.sHtML

[U97] JS：并发请求
来源：http://read.share.fehbvm.com/Article/details/gbtrfepds.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gdwgydxzx.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gypkqkaif.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.zdbjq.cn/Article/details/gpgmgzawn.sHtML

[U99] JS：事件监听
来源：http://mobile.fehbvm.com/Article/details/gphuxkfqf.sHtML

el.addEventListener("click", e => {})
来源：http://blog.zdbjq.cn/Article/details/gwqhacgyd.sHtML

[U100] JS：DOM 查询
来源：http://www.share.hesvh.cn/Article/details/gwrjuvbij.sHtML

document.querySelector(".item")
来源：http://m.share.zdbjq.cn/Article/details/gjjsobrrq.sHtML

[U101] JS：classList 操作
来源：http://mobile.fehbvm.com/Article/details/gdawowhix.sHtML

el.classList.toggle("active")
来源：http://wap.hesvh.cn/Article/details/gxluqkcof.sHtML

[U102] JS：本地存储
来源：http://3g.hesvh.cn/Article/details/gnpmxtgte.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.hesvh.cn/Article/details/gwdyipfry.sHtML

[U103] JS：定时器
来源：http://mobile.zdbjq.cn/Article/details/gabfkfcqx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fehbvm.com/Article/details/gwitevfog.sHtML

[U104] JS：防抖
来源：http://3g.fehbvm.com/Article/details/glcrixtbz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gwsbdhixi.sHtML

[U105] JS：节流
来源：http://m.share.fehbvm.com/Article/details/gbkernhsh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.hesvh.cn/Article/details/gqghvliom.sHtML

[U106] JS：日期格式化
来源：http://blog.fehbvm.com/Article/details/gzhlriffo.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.zdbjq.cn/Article/details/glmdgukyh.sHtML

[U107] JS：数字千分位
来源：http://baike.zdbjq.cn/Article/details/gaozwzeuw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.hesvh.cn/Article/details/ghpetiaih.sHtML

[U108] JS：随机整数
来源：http://m.share.hesvh.cn/Article/details/giofdticb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fehbvm.com/Article/details/gxacffdek.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/gedfsnrry.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/ghbkokhyn.sHtML

[U110] JS：数组分块
来源：http://3g.zdbjq.cn/Article/details/geqpgnhhj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.hesvh.cn/Article/details/galmmxikg.sHtML

[U111] JS：对象转 Map
来源：http://3g.zdbjq.cn/Article/details/gssypggvn.sHtML

new Map(Object.entries(obj))
来源：http://3g.zdbjq.cn/Article/details/gfctmvumh.sHtML

[U112] JS：字符串补位
来源：http://m.share.fehbvm.com/Article/details/gfwdefwps.sHtML

"7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/geibxzven.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.hesvh.cn/Article/details/gfiqrhxny.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gdqhzxmbt.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.zdbjq.cn/Article/details/ggxyvrtsi.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gntsdnyke.sHtML

[U115] JS：生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gmstynnox.sHtML

crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/geuxuuvld.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fehbvm.com/Article/details/gkcrxvesk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fehbvm.com/Article/details/gkdzstsyg.sHtML

[U117] JS：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gqeslaevw.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fehbvm.com/Article/details/gnexoulap.sHtML

[U118] JS：开发服务器
来源：http://3g.hesvh.cn/Article/details/gogaffhop.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fehbvm.com/Article/details/gjbvpiqkq.sHtML

[U119] JS：生产构建
来源：http://www.m.share.hesvh.cn/Article/details/gyxiaurbl.sHtML

npx vite build
来源：http://3g.fehbvm.com/Article/details/gqfqotzkd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.hesvh.cn/Article/details/gzktnfnbg.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.hesvh.cn/Article/details/gwidzhpgc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gcmfacbil.sHtML

统计汇总
来源：http://3g.fehbvm.com/Article/details/gfzvbkyuh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwyzeyhfz.sHtML

按语言统计（条）：
来源：http://www.m.share.hesvh.cn/Article/details/gzsquutac.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/gibuxxglu.sHtML

PHP ............ 252
来源：http://www.share.zdbjq.cn/Article/details/gljrgoysc.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/giravsguj.sHtML

TypeScript ..... 212
来源：http://blog.zdbjq.cn/Article/details/gdhxovkbp.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/gvjfpqbru.sHtML

Go ............. 212
来源：http://www.share.hesvh.cn/Article/details/gxpdyuffg.sHtML

Ruby ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gybjloduq.sHtML

C# ............. 212
来源：http://read.share.fehbvm.com/Article/details/glhywfkne.sHtML

C .............. 30
来源：http://blog.hesvh.cn/Article/details/gzcwcozau.sHtML

C++ ............ 30
来源：http://www.m.share.hesvh.cn/Article/details/ggeykxqww.sHtML

SQL ............ 90
来源：http://mobile.zdbjq.cn/Article/details/gdpugerjs.sHtML

Bash ........... 80
来源：http://www.m.share.hesvh.cn/Article/details/gwwcppowg.sHtML

Kotlin ......... 15
来源：http://read.share.hesvh.cn/Article/details/gfxfurvny.sHtML

Swift .......... 15
来源：http://read.share.fehbvm.com/Article/details/gbzjpdllj.sHtML

Lua ............ 10
来源：http://read.share.fehbvm.com/Article/details/gthakyfdr.sHtML

Perl ........... 10
来源：http://baike.fehbvm.com/Article/details/ghgyekdch.sHtML

Scala .......... 10
来源：http://www.blog.fehbvm.com/Article/details/gzzxpuryk.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/gnnxckxwt.sHtML

合计 ........... 2106 条
来源：http://baike.zdbjq.cn/Article/details/gyzvghnmp.sHtML

按章节统计：
来源：http://m.share.fehbvm.com/Article/details/ggiczpnxz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gjunnwejo.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gfkhxfjrc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gnspknlkq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gddrborif.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fehbvm.com/Article/details/gqcuspmgy.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/gltbaevdr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gxzbwgfrx.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gyclvscfx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gjimdungp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gygjdtufq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/ganthoutw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/grtuertez.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gwuyxzfmm.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/glslcyrha.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.zdbjq.cn/Article/details/gtqggpwzf.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/ghrvuvlav.sHtML

Q SQL 专题                              90
来源：http://mobile.hesvh.cn/Article/details/gjsebafnu.sHtML

R Bash 专题                             80
来源：http://read.share.zdbjq.cn/Article/details/ggvgrtmve.sHtML

S C / C++ 专题                          60
来源：http://mobile.fehbvm.com/Article/details/gofxpktqb.sHtML

T 其他语言补充                          60
来源：http://www.blog.fehbvm.com/Article/details/gslkgeuaj.sHtML

U 高频实用片段                         120
来源：http://mobile.fehbvm.com/Article/details/giswhblsp.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/givtbvenw.sHtML

合计                                  2106 条
来源：http://blog.zdbjq.cn/Article/details/ggpxcvljd.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gcvcoxlmv.sHtML

使用提醒
来源：http://m.share.fehbvm.com/Article/details/gzfbuwkai.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gqzebcsdf.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.hesvh.cn/Article/details/gmlokqgol.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.hesvh.cn/Article/details/gqtdnbegm.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.zdbjq.cn/Article/details/gdgstsdsc.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.hesvh.cn/Article/details/geazxapza.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fehbvm.com/Article/details/guapoebyb.sHtML

—— 文件结束 ——
来源：http://read.share.zdbjq.cn/Article/details/gxssfhvqt.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvwxqlrbs.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.zdbjq.cn/Article/details/gaxdgiagj.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.zdbjq.cn/Article/details/gxkkwfouo.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gggzpgazs.sHtML

【收录内容】
来源：http://wap.fehbvm.com/Article/details/gpanbvuql.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.zdbjq.cn/Article/details/grsqccpud.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.zdbjq.cn/Article/details/giszaagbx.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.hesvh.cn/Article/details/gpsaplmgh.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.hesvh.cn/Article/details/gyyqvmmmi.sHtML

【使用说明】
来源：http://www.share.hesvh.cn/Article/details/gyjhuajpo.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.hesvh.cn/Article/details/gupwxjxze.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fehbvm.com/Article/details/gwbnslwbe.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.zdbjq.cn/Article/details/grkgchpyd.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.zdbjq.cn/Article/details/gkoohieuy.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fehbvm.com/Article/details/gnqfowrbx.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.hesvh.cn/Article/details/glbsjvzxh.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fehbvm.com/Article/details/gbnbmxpci.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.hesvh.cn/Article/details/ghyklplxf.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.zdbjq.cn/Article/details/gzsdwwqch.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.hesvh.cn/Article/details/gweqbwkrm.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.fehbvm.com/Article/details/gxholgehv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.zdbjq.cn/Article/details/gubtaogqm.sHtML

【文件统计】
来源：http://mobile.fehbvm.com/Article/details/goezikgpz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fehbvm.com/Article/details/gtcuynlbd.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gujxsstyj.sHtML

目  录
来源：http://mobile.fehbvm.com/Article/details/gfbvxfkpt.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gcfykkazg.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/gncxjbihc.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gszprsnmp.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gledblzqn.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/ghrvrlypm.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fehbvm.com/Article/details/giigmmtqv.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.fehbvm.com/Article/details/glloehwaa.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gxidwwksz.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.hesvh.cn/Article/details/gzvxsdbru.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gqwrkwkwq.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gdhxygsgd.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/goraqjudf.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gfdkkmfki.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gzqdeignd.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.hesvh.cn/Article/details/gnmnkwsso.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.hesvh.cn/Article/details/gryouxcdk.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gpmtdsswc.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.hesvh.cn/Article/details/grspmzzat.sHtML


<!-- 参考信息 -->