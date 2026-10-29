代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://blog.hesvh.cn/Article/details/gnulhsxai.sHtML

@contextlib.contextmanager
来源：http://wap.zdbjq.cn/Article/details/gugzcmvgv.sHtML

[U22] Py：矩阵转置
来源：http://read.share.zdbjq.cn/Article/details/graavkkcl.sHtML

list(zip(*m))
来源：http://www.share.zdbjq.cn/Article/details/gwbffcytt.sHtML

[U23] Py：分块读取大文件
来源：http://wap.hesvh.cn/Article/details/gwodrkkul.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.hesvh.cn/Article/details/gfrnrwkkk.sHtML

[U24] Py：路径操作
来源：http://www.m.share.zdbjq.cn/Article/details/gfdwetwry.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gcwpajyte.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fehbvm.com/Article/details/gsxnjivty.sHtML

csv.DictReader(f)
来源：http://www.share.zdbjq.cn/Article/details/gkvvfvibc.sHtML

[U26] Py：并发下载
来源：http://m.share.zdbjq.cn/Article/details/gmqxxrnjx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.zdbjq.cn/Article/details/guwfaruqi.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fehbvm.com/Article/details/gyijptagt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fehbvm.com/Article/details/gzsqzdmur.sHtML

[U28] Py：类型别名
来源：http://www.share.fehbvm.com/Article/details/gdkhhgyvo.sHtML

UserId = int
来源：http://3g.zdbjq.cn/Article/details/gzifnkbhj.sHtML

[U29] Py：属性校验
来源：http://m.share.zdbjq.cn/Article/details/gonzikffi.sHtML

@property 与 @x.setter 配合
来源：http://wap.fehbvm.com/Article/details/gyoudwlyo.sHtML

[U30] Py：数据类
来源：http://www.share.hesvh.cn/Article/details/gguqxyati.sHtML

@dataclass(slots=True)
来源：http://www.blog.fehbvm.com/Article/details/gcusgcluo.sHtML

[U31] Py：单测
来源：http://baike.hesvh.cn/Article/details/gqtdqaudb.sHtML

python -m pytest -q
来源：http://www.share.zdbjq.cn/Article/details/gzvwqyzxn.sHtML

[U32] Py：代码格式化
来源：http://mobile.zdbjq.cn/Article/details/geogizumu.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.zdbjq.cn/Article/details/gxetofnzu.sHtML

[U33] Py：打包发布
来源：http://m.share.hesvh.cn/Article/details/gqteekpxw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.zdbjq.cn/Article/details/ggusboeci.sHtML

[U34] Py：判断编码
来源：http://3g.hesvh.cn/Article/details/gsrjyikuf.sHtML

chardet.detect(raw)
来源：http://m.share.hesvh.cn/Article/details/gzpjnybvz.sHtML

[U35] Py：发送邮件
来源：http://wap.hesvh.cn/Article/details/gtjwnublx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/gzmibhvlh.sHtML

[U36] Py：定时任务
来源：http://www.m.share.hesvh.cn/Article/details/grbbmryce.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.zdbjq.cn/Article/details/gdyttcldg.sHtML

[U37] Py：读写 Excel
来源：http://www.share.zdbjq.cn/Article/details/gfzvvxhec.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/guqqouucy.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.zdbjq.cn/Article/details/goryrgfqb.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.zdbjq.cn/Article/details/gpteycqdh.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.hesvh.cn/Article/details/gxekeiewz.sHtML

sys.stdout.isatty()
来源：http://read.share.hesvh.cn/Article/details/gjujsidkq.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fehbvm.com/Article/details/gkaqnncsl.sHtML

print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gdrbkwhci.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.hesvh.cn/Article/details/ghqqxmeol.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.hesvh.cn/Article/details/gatqbxzco.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.hesvh.cn/Article/details/gktuhlvfn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.zdbjq.cn/Article/details/gwmyqtauy.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fehbvm.com/Article/details/guthsojle.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/ggwronprz.sHtML

[U44] PHP：开启严格类型
来源：http://baike.zdbjq.cn/Article/details/gbrykcbhv.sHtML

declare(strict_types=1);
来源：http://www.blog.fehbvm.com/Article/details/ggipfmqrf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fehbvm.com/Article/details/ggbomkyhg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gixgmorvz.sHtML

[U46] PHP：可空类型
来源：http://blog.zdbjq.cn/Article/details/gnpdjmzxe.sHtML

?string $name = null
来源：http://read.share.hesvh.cn/Article/details/gvpkkgynm.sHtML

[U47] PHP：联合类型
来源：http://baike.hesvh.cn/Article/details/gphpuuxxq.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/gawhimsqd.sHtML

[U48] PHP：纯枚举
来源：http://read.share.hesvh.cn/Article/details/gojaoynno.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.zdbjq.cn/Article/details/gmragclcd.sHtML

[U49] PHP：只读属性
来源：http://www.share.hesvh.cn/Article/details/gksamluyi.sHtML

public readonly string $name
来源：http://m.share.zdbjq.cn/Article/details/ghyaefnhs.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fehbvm.com/Article/details/gzximxnoh.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fehbvm.com/Article/details/gkixvnjis.sHtML

[U51] PHP：数组解构
来源：http://wap.fehbvm.com/Article/details/gcojsubnk.sHtML

[$a, $b] = $arr;
来源：http://mobile.fehbvm.com/Article/details/gwvsbdhtz.sHtML

[U52] PHP：箭头函数
来源：http://3g.fehbvm.com/Article/details/gbqtujebf.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fehbvm.com/Article/details/gendianje.sHtML

[U53] PHP：空合并运算符
来源：http://wap.zdbjq.cn/Article/details/gqsovocrk.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fehbvm.com/Article/details/gbbqqbrya.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fehbvm.com/Article/details/gyvuhhhew.sHtML

$obj?->method()
来源：http://www.m.share.zdbjq.cn/Article/details/gohkiiqwx.sHtML

[U55] PHP：match 表达式
来源：http://blog.fehbvm.com/Article/details/gmiqzuslg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.hesvh.cn/Article/details/gmrcvjbcq.sHtML

[U56] PHP：命名参数
来源：http://baike.zdbjq.cn/Article/details/gfnpknutx.sHtML

f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gijvpzfxc.sHtML

[U57] PHP：字符串插值
来源：http://baike.hesvh.cn/Article/details/gzpcahmuw.sHtML

"值: {$a}"
来源：http://www.share.fehbvm.com/Article/details/gthylqfvs.sHtML

[U58] PHP：数组三件套
来源：http://read.share.zdbjq.cn/Article/details/giurvptjh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fehbvm.com/Article/details/gmjjykcyx.sHtML

[U59] PHP：自定义排序
来源：http://baike.fehbvm.com/Article/details/gxtefvnbo.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gbjcnkjlg.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.zdbjq.cn/Article/details/goanrmdyn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.hesvh.cn/Article/details/gnkczpvpo.sHtML

[U61] PHP：正则
来源：http://www.blog.hesvh.cn/Article/details/gqdesvqvy.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gcajbjfhi.sHtML

[U62] PHP：日期对象
来源：http://www.blog.zdbjq.cn/Article/details/gzwmyofho.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.zdbjq.cn/Article/details/gcrklhgjh.sHtML

[U63] PHP：文件读写
来源：http://blog.hesvh.cn/Article/details/gqfiwredl.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.hesvh.cn/Article/details/gjectzqfa.sHtML

[U64] PHP：目录遍历
来源：http://read.share.hesvh.cn/Article/details/gaspnzvum.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.zdbjq.cn/Article/details/gcfjzgtei.sHtML

[U65] PHP：会话
来源：http://baike.zdbjq.cn/Article/details/gwxotjuai.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fehbvm.com/Article/details/gkpgkjhwu.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.hesvh.cn/Article/details/gepeqfszf.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.hesvh.cn/Article/details/gebiwptqy.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.zdbjq.cn/Article/details/glajrfkco.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.zdbjq.cn/Article/details/gkkihpnig.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fehbvm.com/Article/details/gexemwmjt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.hesvh.cn/Article/details/gfcccfcfu.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fehbvm.com/Article/details/gblopsmai.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.hesvh.cn/Article/details/gqkyegcff.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.zdbjq.cn/Article/details/gbxcplovl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.hesvh.cn/Article/details/gjfooacvo.sHtML

[U71] PHP：抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gqbkgjhzx.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fehbvm.com/Article/details/gorpztcuj.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fehbvm.com/Article/details/gnvpcoejd.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.hesvh.cn/Article/details/guafablmq.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.zdbjq.cn/Article/details/gfahevoxh.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.zdbjq.cn/Article/details/gumjzjbna.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gfdgqybbu.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.zdbjq.cn/Article/details/gfffamnfp.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.hesvh.cn/Article/details/gbaljtpgt.sHtML

composer require psr/container
来源：http://wap.hesvh.cn/Article/details/glreuunyv.sHtML

[U76] PHP：简单路由
来源：http://3g.fehbvm.com/Article/details/gsizfjkts.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/ggoebmewn.sHtML

[U77] PHP：模板渲染
来源：http://wap.fehbvm.com/Article/details/gfokkhrgx.sHtML

composer require twig/twig
来源：http://mobile.zdbjq.cn/Article/details/gsbgweggd.sHtML

[U78] PHP：单元测试
来源：http://blog.fehbvm.com/Article/details/gxwnaztkk.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.hesvh.cn/Article/details/gmhqjeaon.sHtML

[U79] PHP：静态分析
来源：http://www.share.fehbvm.com/Article/details/gyumkinti.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fehbvm.com/Article/details/ggnlnzaam.sHtML

[U80] PHP：代码规范修复
来源：http://blog.hesvh.cn/Article/details/gouifumpa.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fehbvm.com/Article/details/gwvamospf.sHtML

[U81] JS：初始化项目
来源：http://baike.fehbvm.com/Article/details/gfgbswxqa.sHtML

npm init -y;  npm i express
来源：http://www.share.fehbvm.com/Article/details/gqwynumde.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fehbvm.com/Article/details/gcnrrfdkz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.hesvh.cn/Article/details/gycgetcdu.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.zdbjq.cn/Article/details/gatdgahbd.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/gclzrzjjb.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fehbvm.com/Article/details/gefoguyih.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.hesvh.cn/Article/details/gcmlhfwbt.sHtML

[U85] JS：可选链
来源：http://www.blog.zdbjq.cn/Article/details/gniaeqxtz.sHtML

a?.b?.c
来源：http://mobile.hesvh.cn/Article/details/gbabtyrls.sHtML

[U86] JS：空值合并
来源：http://baike.hesvh.cn/Article/details/gwfbbwvyr.sHtML

a ?? b
来源：http://www.blog.fehbvm.com/Article/details/giagtvlfp.sHtML

[U87] JS：解构默认值
来源：http://wap.zdbjq.cn/Article/details/gngrbzpaf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.hesvh.cn/Article/details/gzxspoudx.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fehbvm.com/Article/details/gnwsfzxfs.sHtML

{ ...a, ...b }
来源：http://blog.hesvh.cn/Article/details/gibiutzdi.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fehbvm.com/Article/details/gdxhmzzrz.sHtML

[...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gokxgsvvj.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fehbvm.com/Article/details/gxhzssaxw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gcyhxtccw.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.zdbjq.cn/Article/details/gdzflwsjg.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.hesvh.cn/Article/details/gqoredcpb.sHtML

[U92] JS：深拷贝
来源：http://blog.zdbjq.cn/Article/details/gqthapvsu.sHtML

structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gkjfkztfa.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gypdobajk.sHtML

`共 ${n} 条`
来源：http://baike.hesvh.cn/Article/details/gkgzwiacw.sHtML

[U94] JS：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gnvzjplyk.sHtML

const double = x => x * 2;
来源：http://read.share.fehbvm.com/Article/details/gzdovmfnx.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.zdbjq.cn/Article/details/gmevsatsr.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.hesvh.cn/Article/details/gkdizbgnb.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fehbvm.com/Article/details/grxfmswlp.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gfasxaspk.sHtML

[U97] JS：并发请求
来源：http://www.blog.fehbvm.com/Article/details/gkgfaqzrs.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/ghprpufzd.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gudlergnf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.zdbjq.cn/Article/details/gdcofeiuj.sHtML

[U99] JS：事件监听
来源：http://m.share.hesvh.cn/Article/details/grmbqfuks.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fehbvm.com/Article/details/gxwjhmgwi.sHtML

[U100] JS：DOM 查询
来源：http://baike.zdbjq.cn/Article/details/ggyhemdqz.sHtML

document.querySelector(".item")
来源：http://read.share.zdbjq.cn/Article/details/gnosukbec.sHtML

[U101] JS：classList 操作
来源：http://www.share.fehbvm.com/Article/details/grmervttm.sHtML

el.classList.toggle("active")
来源：http://www.blog.hesvh.cn/Article/details/gdplhxwjb.sHtML

[U102] JS：本地存储
来源：http://www.share.fehbvm.com/Article/details/gqjotwxwq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fehbvm.com/Article/details/gwyyzjjae.sHtML

[U103] JS：定时器
来源：http://wap.hesvh.cn/Article/details/gaqyebtjn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fehbvm.com/Article/details/gilirolou.sHtML

[U104] JS：防抖
来源：http://blog.hesvh.cn/Article/details/gpqkxanir.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gmievqykw.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/glwuqdhrz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fehbvm.com/Article/details/gvsrubwdj.sHtML

[U106] JS：日期格式化
来源：http://www.share.hesvh.cn/Article/details/gqiwzkisz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fehbvm.com/Article/details/gatorfnac.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/gatjorkcj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gxmmklcpz.sHtML

[U108] JS：随机整数
来源：http://baike.fehbvm.com/Article/details/gespmqjga.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.zdbjq.cn/Article/details/gzgteophp.sHtML

[U109] JS：数组分组
来源：http://www.m.share.hesvh.cn/Article/details/gvebsrnst.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gmwlcwdcr.sHtML

[U110] JS：数组分块
来源：http://mobile.hesvh.cn/Article/details/gfzuaslos.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fehbvm.com/Article/details/gmwgblyed.sHtML

[U111] JS：对象转 Map
来源：http://mobile.zdbjq.cn/Article/details/gvelcolrr.sHtML

new Map(Object.entries(obj))
来源：http://read.share.zdbjq.cn/Article/details/ggcsbsbsj.sHtML

[U112] JS：字符串补位
来源：http://baike.hesvh.cn/Article/details/gqukrxiib.sHtML

"7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gqaqldakz.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fehbvm.com/Article/details/gxmrwbxel.sHtML

s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gxhdgxhpl.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.hesvh.cn/Article/details/gojmtitgy.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gvbznihcb.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gfiaqtnfz.sHtML

crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gppziznvq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.zdbjq.cn/Article/details/gsqdovino.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.zdbjq.cn/Article/details/gmfkfvbce.sHtML

[U117] JS：单元测试
来源：http://m.share.fehbvm.com/Article/details/gqjtkmhdk.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fehbvm.com/Article/details/gvtmtjylz.sHtML

[U118] JS：开发服务器
来源：http://www.blog.hesvh.cn/Article/details/gbldsmqcd.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.zdbjq.cn/Article/details/gxztkhrrf.sHtML

[U119] JS：生产构建
来源：http://www.blog.hesvh.cn/Article/details/grycxncso.sHtML

npx vite build
来源：http://wap.fehbvm.com/Article/details/ggujbpuhk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.hesvh.cn/Article/details/gjqynncyp.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.hesvh.cn/Article/details/gbrvmfckx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gittkpbnf.sHtML

统计汇总
来源：http://blog.fehbvm.com/Article/details/gwajpxzkl.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmsvxvwpa.sHtML

按语言统计（条）：
来源：http://wap.zdbjq.cn/Article/details/gdqcwuwrn.sHtML

Python ......... 252
来源：http://wap.hesvh.cn/Article/details/gkjlsoqit.sHtML

PHP ............ 252
来源：http://blog.zdbjq.cn/Article/details/gddrarony.sHtML

JavaScript ..... 252
来源：http://blog.zdbjq.cn/Article/details/ggcsgmguh.sHtML

TypeScript ..... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gbztxumxf.sHtML

Java ........... 212
来源：http://read.share.hesvh.cn/Article/details/ggrnmemva.sHtML

Go ............. 212
来源：http://mobile.fehbvm.com/Article/details/gkhewfmjp.sHtML

Ruby ........... 212
来源：http://mobile.zdbjq.cn/Article/details/gofanpiyv.sHtML

C# ............. 212
来源：http://3g.fehbvm.com/Article/details/gaktyraym.sHtML

C .............. 30
来源：http://wap.fehbvm.com/Article/details/gaiuyrnbk.sHtML

C++ ............ 30
来源：http://blog.fehbvm.com/Article/details/ghhzoeomx.sHtML

SQL ............ 90
来源：http://www.m.share.hesvh.cn/Article/details/gwkcxeebt.sHtML

Bash ........... 80
来源：http://www.share.fehbvm.com/Article/details/gxylthbqn.sHtML

Kotlin ......... 15
来源：http://blog.hesvh.cn/Article/details/gzsdgslze.sHtML

Swift .......... 15
来源：http://m.share.zdbjq.cn/Article/details/gowanjlfx.sHtML

Lua ............ 10
来源：http://blog.hesvh.cn/Article/details/gosxbillp.sHtML

Perl ........... 10
来源：http://blog.zdbjq.cn/Article/details/ghoipjans.sHtML

Scala .......... 10
来源：http://baike.zdbjq.cn/Article/details/gqdwbhwhl.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/guerbunva.sHtML

合计 ........... 2106 条
来源：http://www.blog.hesvh.cn/Article/details/gxubffzxu.sHtML

按章节统计：
来源：http://mobile.zdbjq.cn/Article/details/goadbjhuh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gwhohfdci.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/glynwjovh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gmlcfucea.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/gzuezizsc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fehbvm.com/Article/details/gibtvksxf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/gfodrzdjm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gejcwjvzt.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/gbrgabtgw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/govqtuwsx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gwehztxuj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gexvtskfc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gpvxggwbr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/grbedosxr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/gyzzyztwe.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fehbvm.com/Article/details/gqdkezmvv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/giawzaajk.sHtML

Q SQL 专题                              90
来源：http://wap.fehbvm.com/Article/details/gdmyvneip.sHtML

R Bash 专题                             80
来源：http://blog.hesvh.cn/Article/details/gcoutwdch.sHtML

S C / C++ 专题                          60
来源：http://m.share.fehbvm.com/Article/details/gsaqqdhcu.sHtML

T 其他语言补充                          60
来源：http://wap.zdbjq.cn/Article/details/gnlqpcwyf.sHtML

U 高频实用片段                         120
来源：http://www.m.share.zdbjq.cn/Article/details/gihyiaakh.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gvfzoxcfo.sHtML

合计                                  2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gchbbuqff.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gcyhqjkkh.sHtML

使用提醒
来源：http://www.blog.zdbjq.cn/Article/details/gnjgdzlvt.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gsbiwsyde.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.hesvh.cn/Article/details/gdwswqnjo.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.zdbjq.cn/Article/details/ggqkeptuo.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fehbvm.com/Article/details/grruxhpnl.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.hesvh.cn/Article/details/gmiekblvl.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.zdbjq.cn/Article/details/gvhaswvex.sHtML

—— 文件结束 ——
来源：http://blog.fehbvm.com/Article/details/guxtuwxso.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkjvqnphn.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.hesvh.cn/Article/details/gexiizwid.sHtML

Common Programming Examples Cheat Book
来源：http://baike.hesvh.cn/Article/details/gbbxdnagx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvklbkdnp.sHtML

【收录内容】
来源：http://mobile.hesvh.cn/Article/details/gzirqvyuo.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fehbvm.com/Article/details/gavumxunc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.fehbvm.com/Article/details/gnkbzmsnb.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fehbvm.com/Article/details/gmpkdedan.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.zdbjq.cn/Article/details/glndictos.sHtML

【使用说明】
来源：http://m.share.fehbvm.com/Article/details/gbunzohze.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.hesvh.cn/Article/details/giigjtjgw.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.fehbvm.com/Article/details/gfuoalmkd.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.fehbvm.com/Article/details/gsbzqqlrl.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.hesvh.cn/Article/details/gkenyvbgo.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.fehbvm.com/Article/details/gqgcsabjb.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.zdbjq.cn/Article/details/gfcjjifrc.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.zdbjq.cn/Article/details/gcbocpfxv.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.hesvh.cn/Article/details/ghcugdkuh.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.hesvh.cn/Article/details/grqtmdyno.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.hesvh.cn/Article/details/gthxnwkht.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.hesvh.cn/Article/details/gtzlwurhj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.fehbvm.com/Article/details/gxgdhlosr.sHtML

【文件统计】
来源：http://blog.zdbjq.cn/Article/details/gcaahypvt.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.zdbjq.cn/Article/details/gofjneknh.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gdfcudfsu.sHtML

目  录
来源：http://m.share.zdbjq.cn/Article/details/gvffktdsq.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gvlccduub.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/gfckvppgk.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gflzhityy.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gniciegzw.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.zdbjq.cn/Article/details/gilaafuwg.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.fehbvm.com/Article/details/gilgkvuzt.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.hesvh.cn/Article/details/gppbnpkau.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/grydfbmhj.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gqgnnxtqm.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gbcylgiao.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.zdbjq.cn/Article/details/gmdyeuamk.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gxcdecdfv.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gavezhrpo.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gjelrxiav.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gbgefdlbw.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.hesvh.cn/Article/details/ghsdlmucl.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gjoczlmqk.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.hesvh.cn/Article/details/gfsmotjjr.sHtML


<!-- 参考信息 -->