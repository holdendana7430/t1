代发 wailian999

[U29] Py：属性校验
来源：http://baike.fanxiaobao.xyz/Article/details/gmbrgjgsv.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fanxiaobao.xyz/Article/details/guhqkclqj.sHtML

[U30] Py：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gyuhxsnao.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvnwoteh.sHtML

[U31] Py：单测
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrdfnwjd.sHtML

python -m pytest -q
来源：http://wap.fanxiaobao.xyz/Article/details/gmpxwtggs.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrqbgeat.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshjwgvtj.sHtML

[U33] Py：打包发布
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdkqaglc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giftqprra.sHtML

[U34] Py：判断编码
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhpooqbz.sHtML

chardet.detect(raw)
来源：http://baike.fanxiaobao.xyz/Article/details/gtkttgbzp.sHtML

[U35] Py：发送邮件
来源：http://3g.fanxiaobao.xyz/Article/details/gjcyxbotv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fanxiaobao.xyz/Article/details/grbsxkguj.sHtML

[U36] Py：定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gsuayewlr.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fanxiaobao.xyz/Article/details/gispmppew.sHtML

[U37] Py：读写 Excel
来源：http://baike.fanxiaobao.xyz/Article/details/ghtrrdhis.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fanxiaobao.xyz/Article/details/gomlnbowa.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/gpuvwrayx.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofvrcput.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fanxiaobao.xyz/Article/details/guithwwcr.sHtML

sys.stdout.isatty()
来源：http://wap.fanxiaobao.xyz/Article/details/gcymbvqsk.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gqukansna.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpapvqamx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fanxiaobao.xyz/Article/details/guaklpthn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fanxiaobao.xyz/Article/details/ggnghrcfx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fanxiaobao.xyz/Article/details/gphhvdugp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fanxiaobao.xyz/Article/details/ghejzlxzs.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaencuqwp.sHtML

namespace App\Http;
来源：http://blog.fanxiaobao.xyz/Article/details/ghxdinnhz.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fanxiaobao.xyz/Article/details/gkapjnkix.sHtML

declare(strict_types=1);
来源：http://baike.fanxiaobao.xyz/Article/details/geuzhrtng.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fanxiaobao.xyz/Article/details/gllyvaekw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grualabil.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrpkzfss.sHtML

?string $name = null
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkypqnrhw.sHtML

[U47] PHP：联合类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gugxjnvnq.sHtML

int|string $id
来源：http://www.share.fanxiaobao.xyz/Article/details/gazzcawpw.sHtML

[U48] PHP：纯枚举
来源：http://3g.fanxiaobao.xyz/Article/details/ghorkqebd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxuyweswh.sHtML

[U49] PHP：只读属性
来源：http://baike.fanxiaobao.xyz/Article/details/gihmddqwp.sHtML

public readonly string $name
来源：http://3g.fanxiaobao.xyz/Article/details/gcanftafh.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtjizwyx.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/grcstyinz.sHtML

[U51] PHP：数组解构
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjflxbxx.sHtML

[$a, $b] = $arr;
来源：http://baike.fanxiaobao.xyz/Article/details/guqcbyncp.sHtML

[U52] PHP：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/gjydhfrfm.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxppbzlbf.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkrkhonf.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fanxiaobao.xyz/Article/details/gtyzirmhv.sHtML

[U54] PHP：空安全调用
来源：http://baike.fanxiaobao.xyz/Article/details/gamhoudnw.sHtML

$obj?->method()
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhvumbgs.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gfasxybiy.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvaqoozlv.sHtML

[U56] PHP：命名参数
来源：http://wap.fanxiaobao.xyz/Article/details/gpzfrhqea.sHtML

f(a: 1, b: 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvfomnjf.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/guuzyeene.sHtML

"值: {$a}"
来源：http://wap.fanxiaobao.xyz/Article/details/gsnpwdihb.sHtML

[U58] PHP：数组三件套
来源：http://baike.fanxiaobao.xyz/Article/details/gbqnqrhlt.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzomndty.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gpudxtuxl.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gcxmorqst.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcallnmdl.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbcpfwnhw.sHtML

[U61] PHP：正则
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgurubsn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgqqbtad.sHtML

[U62] PHP：日期对象
来源：http://www.share.fanxiaobao.xyz/Article/details/gjycjmdsj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fanxiaobao.xyz/Article/details/glcbhbypn.sHtML

[U63] PHP：文件读写
来源：http://3g.fanxiaobao.xyz/Article/details/gafbgcykg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgnzrgqi.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzsehori.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fanxiaobao.xyz/Article/details/glykuwejj.sHtML

[U65] PHP：会话
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrzhsome.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/geznlugxe.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqevyfdm.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gaopkyatm.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxaokydn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fanxiaobao.xyz/Article/details/gooienzwj.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gpeidahgr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fanxiaobao.xyz/Article/details/gvssmijwb.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlojjwts.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fanxiaobao.xyz/Article/details/gllpowblo.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcewmztz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fanxiaobao.xyz/Article/details/ghapkfapj.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgrtzxay.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjohdcgrt.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gfchgxdbe.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fanxiaobao.xyz/Article/details/gdglbcfaa.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzfrvqlt.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdywkawo.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/grthgxqjg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fanxiaobao.xyz/Article/details/gqwkiomyu.sHtML

[U75] PHP：依赖注入
来源：http://3g.fanxiaobao.xyz/Article/details/gewnqhgfu.sHtML

composer require psr/container
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnbxedws.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvgthixt.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fanxiaobao.xyz/Article/details/gudcljeoo.sHtML

[U77] PHP：模板渲染
来源：http://blog.fanxiaobao.xyz/Article/details/glppiimmn.sHtML

composer require twig/twig
来源：http://www.share.fanxiaobao.xyz/Article/details/gcstkefro.sHtML

[U78] PHP：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/gysjbuylu.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fanxiaobao.xyz/Article/details/gnxnwiudw.sHtML

[U79] PHP：静态分析
来源：http://read.share.fanxiaobao.xyz/Article/details/ggavwmjxl.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttwnbqsb.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fanxiaobao.xyz/Article/details/gizznvtvc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fanxiaobao.xyz/Article/details/gsqolhpta.sHtML

[U81] JS：初始化项目
来源：http://m.share.fanxiaobao.xyz/Article/details/grhgkzrtz.sHtML

npm init -y;  npm i express
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzjbpzyy.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fanxiaobao.xyz/Article/details/gpjloyysw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fanxiaobao.xyz/Article/details/gwlxhecel.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtptisbho.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fanxiaobao.xyz/Article/details/glvpezguv.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fanxiaobao.xyz/Article/details/golwqmnzy.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fanxiaobao.xyz/Article/details/gtrnwyyxa.sHtML

[U85] JS：可选链
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfrvjugk.sHtML

a?.b?.c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibmmmgub.sHtML

[U86] JS：空值合并
来源：http://baike.fanxiaobao.xyz/Article/details/gccpzikrw.sHtML

a ?? b
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqwrbzph.sHtML

[U87] JS：解构默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gvvaxbbut.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fanxiaobao.xyz/Article/details/gwzfyiora.sHtML

[U88] JS：对象展开合并
来源：http://baike.fanxiaobao.xyz/Article/details/geppqsaua.sHtML

{ ...a, ...b }
来源：http://wap.fanxiaobao.xyz/Article/details/ghveavthc.sHtML

[U89] JS：数组去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnlyopjd.sHtML

[...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gvenegipe.sHtML

[U90] JS：数字数组排序
来源：http://wap.fanxiaobao.xyz/Article/details/grdrbesrj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/gtchetpzc.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gemtrdptk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fanxiaobao.xyz/Article/details/gwisqquun.sHtML

[U92] JS：深拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/giqgunjbw.sHtML

structuredClone(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gyxfylbdb.sHtML

[U93] JS：模板字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gouswiruw.sHtML

`共 ${n} 条`
来源：http://mobile.fanxiaobao.xyz/Article/details/glmyupdap.sHtML

[U94] JS：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmkzopks.sHtML

const double = x => x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gaaeixwyl.sHtML

[U95] JS：Promise 包装
来源：http://baike.fanxiaobao.xyz/Article/details/gnqtqeyti.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gsafpqoco.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fanxiaobao.xyz/Article/details/grbkxvwaq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzyucgnm.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllraxeds.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/glmkmbnhg.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fanxiaobao.xyz/Article/details/grhjathie.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsuzbnza.sHtML

[U99] JS：事件监听
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxmpjfkf.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fanxiaobao.xyz/Article/details/gzxcqeyrn.sHtML

[U100] JS：DOM 查询
来源：http://3g.fanxiaobao.xyz/Article/details/gyqjkcbwc.sHtML

document.querySelector(".item")
来源：http://blog.fanxiaobao.xyz/Article/details/geldcppfr.sHtML

[U101] JS：classList 操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfhzevmm.sHtML

el.classList.toggle("active")
来源：http://blog.fanxiaobao.xyz/Article/details/gwinoyemo.sHtML

[U102] JS：本地存储
来源：http://wap.fanxiaobao.xyz/Article/details/gylmozjks.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjabqkgs.sHtML

[U103] JS：定时器
来源：http://blog.fanxiaobao.xyz/Article/details/gbcewwqar.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbopahuol.sHtML

[U104] JS：防抖
来源：http://blog.fanxiaobao.xyz/Article/details/gxylkeecr.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpovtzofm.sHtML

[U105] JS：节流
来源：http://baike.fanxiaobao.xyz/Article/details/gjbijzwke.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcvkwudn.sHtML

[U106] JS：日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gcgjvouel.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fanxiaobao.xyz/Article/details/gygkngjuw.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjywqqcf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fanxiaobao.xyz/Article/details/gekarejgq.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqlhirfl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fanxiaobao.xyz/Article/details/gdsimtbii.sHtML

[U109] JS：数组分组
来源：http://3g.fanxiaobao.xyz/Article/details/gomxcqmuv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fanxiaobao.xyz/Article/details/gvkqswlgg.sHtML

[U110] JS：数组分块
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruvxypdv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljykrwkq.sHtML

[U111] JS：对象转 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gxnigybhy.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fanxiaobao.xyz/Article/details/gwywjpouy.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybehgltf.sHtML

"7".padStart(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/gavvgmicy.sHtML

[U113] JS：正则替换全部
来源：http://baike.fanxiaobao.xyz/Article/details/gmlaggcry.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmghdorl.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebujmszq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmadaxdrj.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fanxiaobao.xyz/Article/details/gumlatbgh.sHtML

crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpvqhaow.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fanxiaobao.xyz/Article/details/ghrwemxgi.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazazjqkn.sHtML

[U117] JS：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/geksobudr.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fanxiaobao.xyz/Article/details/gsseseanx.sHtML

[U118] JS：开发服务器
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyhjnsrt.sHtML

npm i -D vite;  npx vite
来源：http://baike.fanxiaobao.xyz/Article/details/gnmqbrvpn.sHtML

[U119] JS：生产构建
来源：http://mobile.fanxiaobao.xyz/Article/details/gatcssmqk.sHtML

npx vite build
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlystcvc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fanxiaobao.xyz/Article/details/gflwrzqei.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fanxiaobao.xyz/Article/details/gaksoutpc.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/guhrgpskg.sHtML

统计汇总
来源：http://blog.fanxiaobao.xyz/Article/details/gzveqbesu.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gggybvdlg.sHtML

按语言统计（条）：
来源：http://www.share.fanxiaobao.xyz/Article/details/genmdbpnp.sHtML

Python ......... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/ggumqufha.sHtML

PHP ............ 252
来源：http://baike.fanxiaobao.xyz/Article/details/gaidcrkvz.sHtML

JavaScript ..... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtllflzm.sHtML

TypeScript ..... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gvodbfubc.sHtML

Java ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqycsvia.sHtML

Go ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/gnijkvrvl.sHtML

Ruby ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gfdbyphks.sHtML

C# ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/gmpobmddt.sHtML

C .............. 30
来源：http://3g.fanxiaobao.xyz/Article/details/gwswwpxyy.sHtML

C++ ............ 30
来源：http://blog.fanxiaobao.xyz/Article/details/gdaqidzuz.sHtML

SQL ............ 90
来源：http://wap.fanxiaobao.xyz/Article/details/gsiffobgz.sHtML

Bash ........... 80
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfgbotlu.sHtML

Kotlin ......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gucwvpqpt.sHtML

Swift .......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlullmov.sHtML

Lua ............ 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghkkmbnf.sHtML

Perl ........... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gsahxwvdo.sHtML

Scala .......... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gtmqdrrhp.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gtmaiodpk.sHtML

合计 ........... 2106 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwruqhum.sHtML

按章节统计：
来源：http://wap.fanxiaobao.xyz/Article/details/gfphtqchk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gdtryulig.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gasccnvwn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gxkmwuyva.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gyicfftoo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fanxiaobao.xyz/Article/details/gfvqmjpsh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybuaaptc.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gacumxtdu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlgkfdkm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcqbvmgf.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gbdvzcwda.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gjquilvpz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmtpaxah.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmoewlkhl.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fanxiaobao.xyz/Article/details/gtrfvpbrk.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgldxbbc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/guxoiruis.sHtML

Q SQL 专题                              90
来源：http://baike.fanxiaobao.xyz/Article/details/gqpuhjtix.sHtML

R Bash 专题                             80
来源：http://www.share.fanxiaobao.xyz/Article/details/gatcdobkm.sHtML

S C / C++ 专题                          60
来源：http://read.share.fanxiaobao.xyz/Article/details/gjchbtbqi.sHtML

T 其他语言补充                          60
来源：http://read.share.fanxiaobao.xyz/Article/details/gajaxhyam.sHtML

U 高频实用片段                         120
来源：http://3g.fanxiaobao.xyz/Article/details/gnygvkefo.sHtML

------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqjmekln.sHtML

合计                                  2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/gtiadpjxl.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gispowkhj.sHtML

使用提醒
来源：http://baike.fanxiaobao.xyz/Article/details/gkvstkrix.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjuerzvg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fanxiaobao.xyz/Article/details/geoswbkdn.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfjllmrq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fanxiaobao.xyz/Article/details/gngteaqcs.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fanxiaobao.xyz/Article/details/ggxpylbsc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkgzuxyc.sHtML

—— 文件结束 ——
来源：http://blog.fanxiaobao.xyz/Article/details/gxzkpqxgy.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcafsvev.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmcvqnin.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpnaedjy.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkvskmri.sHtML

【收录内容】
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvwjjbdp.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.fanxiaobao.xyz/Article/details/gptnusnyb.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqnvgqql.sHtML

SQL · Bash · C · C++
来源：http://wap.fanxiaobao.xyz/Article/details/gimcstrax.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fanxiaobao.xyz/Article/details/gsgqrmnxb.sHtML

【使用说明】
来源：http://m.share.fanxiaobao.xyz/Article/details/grzbkkfoo.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbiuoojv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girjcskys.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqerfzkme.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.fanxiaobao.xyz/Article/details/gusgmzdhy.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.fanxiaobao.xyz/Article/details/gmomzyivk.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.fanxiaobao.xyz/Article/details/gaomztqcx.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyjwjxer.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.fanxiaobao.xyz/Article/details/grjgnnkvn.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxttporjh.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.fanxiaobao.xyz/Article/details/gulhmgeba.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fanxiaobao.xyz/Article/details/gctukjrwe.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgqoidgf.sHtML

【文件统计】
来源：http://wap.fanxiaobao.xyz/Article/details/gdkswaxam.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fanxiaobao.xyz/Article/details/gneinflps.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gmtfjawms.sHtML

目  录
来源：http://baike.fanxiaobao.xyz/Article/details/gmuulwqyd.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrdeoehl.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkblglvwe.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glybvpxjg.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gdyhxgjsk.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gswawgslu.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geuyyfhos.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gexfaeqef.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gegtmxggl.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gjphpkaiz.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gugfzrcqm.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.fanxiaobao.xyz/Article/details/godclnmvm.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdocdxru.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdsyoauj.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gostnvebx.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gfhyekere.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqjohirr.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gpkuyvpvc.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmrilrgl.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrvvthaw.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gckrrpata.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gwpjdnqhl.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghemqgdrp.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gifhzbsgt.sHtML

A. 基础语法与类型
来源：http://m.share.fanxiaobao.xyz/Article/details/galavifjl.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gflwxuqjs.sHtML

[A01] Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gjqzujtjm.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywwvbnhj.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gjuaablzl.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gteobdxwc.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.fanxiaobao.xyz/Article/details/ggphyavjw.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvouakjt.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzrblfxi.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.fanxiaobao.xyz/Article/details/grubsafza.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goguejklw.sHtML


<!-- 参考信息 -->