代发 wailian999

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3vheyybpm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3gtrjhnjg.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3kjhwibgz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gbifkhtt.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3eapajyqw.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3vbtmbaoh.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3pxsehydb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3hsrgyudx.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3xeiubtrj.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3yialujee.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3ejhwebjh.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3kjwuodoq.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3ixqxridh.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3rtjffbpj.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3gvaqpwws.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3tjbpaebh.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3syvooegl.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3cfjptrqw.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3qxrilreq.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3txsgrnrm.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3mhnbwjyf.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3dytlgdpo.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3guismvgk.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3ktnevfpz.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3jptmppla.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3lmscdadb.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3uixsnwmp.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3vnstrebe.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3jodggljs.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3tlvcvfzl.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3hnoxseyv.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3kjfbzytq.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3oqlrqnyu.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3xepbnsja.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3nkmmdqez.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3yuzafiuj.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3cncjidon.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3cppmddtt.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3uowfeyev.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3easkfure.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3clznuikx.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3ybpwtqvu.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3bqoedror.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3voazvsjt.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3cfffyjxy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wkmjlwjn.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3gwtcytri.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3dyzjeyun.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3qaureovk.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3polnkqcr.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3rbkdjwzu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dpspmvty.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3vbkkhlzd.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3yngpdtnb.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3qnlpxjkg.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3inddqxdi.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3tmjynrfk.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3lydhfobf.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3afmndlbt.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3uxqhngbj.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3mpqjcinm.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3pdostxva.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3ciqquakw.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3rhkakmxg.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3ztwjvgqj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3dmchcnry.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3uicdjiky.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hdzoudks.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3owmczcfj.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3ggrohzwg.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3ikgwnevi.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qqlejqnk.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3subcpjdj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ymzykytw.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3brfgysqb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3shldamjh.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3betsxmvr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3bpxpuyuk.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3uzfvlawo.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3alfplqgn.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3zoonhktr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3sjwtezaf.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xzcueiac.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3xzjnpogb.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3rclhaumr.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rttsaibj.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3iwstafnn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lrsogrow.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3kpvmmeqs.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3ljndqldb.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3msupjtdl.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3kpodqafo.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3iksxamnd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3vwmeaema.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3kdyuqbkq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3oljlltyf.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3wjwuzvgn.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3dmixdpkj.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3gtklyqqd.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3dqijrxvf.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3jfwcjdjr.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3awjjywmk.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3dqfzbnbu.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3qzpystfs.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3mvgxplvt.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3ipvywigj.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3nzqradhk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3ewcqsnet.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3yirlkspx.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3jfdierzl.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3cfiaiwxv.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3ebmkgscc.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3pcivlwvj.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3hdvuqzfv.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3vpkfhske.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3yoonezyj.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3leinsluo.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3mkeivhbd.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3trehjjtz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3shcikizj.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3vviljeow.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3rbeqjmjq.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3dfuvesqi.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3naghynmh.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3cvbexaxp.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3qkxyatnq.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3otteirmj.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3dwdjjsfa.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3qzczquwq.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3jvuysngx.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3zkiummyn.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3lobfpbvl.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3tyvbdjin.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vmoeqkex.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3swugsjrq.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3oqyjkqtm.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bmgbusae.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3thmqpnpf.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3yyomsmgs.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mybjdryc.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3dbsvogox.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3jwiyftge.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3hihgcubl.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ckgljodn.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3wolimhyi.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3sfuwvhgs.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3umfdkqfy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3fmrvddhd.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3gryaxesy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ydpxvwja.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3qndseqwk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3efnvfkke.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3hrflwjne.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3bukjiqxe.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3qvjcyfxf.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3mgmofyvu.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3pabtwqiq.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3qeqqudee.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3bjreezcb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3rtrojvqe.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3kdfszius.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3ejvmlwxp.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3ujkfdjbe.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3lawjydai.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3yukfemaw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3kcktjrys.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3itixrggh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3byqinkwg.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3rphmejlg.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3smqawlih.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3inphkrte.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3sowmyzdd.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3vmgpjnqw.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3iygstwdm.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3ubsrnodn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3qmqyzgui.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3oreaqkcc.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3gdqtpohy.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3whkkdcph.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kjigltig.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3zjghksgt.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zsnpzhxc.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3lqfbqzxa.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3gtlprhwa.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3wxxnzosj.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3pjzkiduq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3jhpjrifz.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3ekhwewoc.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3wafqsnja.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3gwwszdaf.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3vsetmrpx.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3xmqfdire.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3bkvhaavg.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3ttnjhvuz.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3jngzwfgs.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3wldowtow.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sltxwpsh.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3bllcahzq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3etssurch.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3gihtolvc.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3tadsovaw.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3qmxjidbm.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3jtrqsxjr.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3vngmoewi.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3lhiazemu.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3sgyqxxon.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3zenmmepe.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3tiktkdpn.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3ooxtpvpw.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3utemltul.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3vmgrgjpv.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3spblkadx.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ghjfsybv.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3odorlong.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3tloorndm.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3tsgqqiuv.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3qiudhhok.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3kuifulpy.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3bwyghkyc.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3tloogcur.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3xzjqhhmi.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3zdztrnjy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3dhvccefo.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3lcpivloy.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3bsnvicdl.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3mbcgcgvk.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3bcnlxopx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3bwysayiy.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ifjubzno.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3tabzjmrc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jsmtfkpz.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hmuvtugd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3syjwilad.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3bwiazflc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3gqivoagi.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dkqhgdqb.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3lspgmpju.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3xkziuaeu.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3jupzkwaj.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3fislzjgk.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3ypqnwndw.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hphatkoc.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3rabctelc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3zveklsbk.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3ufytifpy.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3evdmdkxr.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3jqyfhhec.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3ovdnpugf.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3ufczokng.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3qlwrqliy.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3djjlwewe.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3dckmrfhh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fxedherv.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3iavekadl.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3galwenoh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cltkrbcv.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3cyfaspaz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3jtqaofoc.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3vfqgnjbm.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3zogzayzc.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3nmjpbqzs.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3lywkodzb.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3ynazqcqg.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3fqsityqk.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3hxepkcye.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3pqkvmyxl.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3hqkndnvb.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3kogzkaqc.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3lugfszpb.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3urtregky.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3vjvarkll.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3mbvomnwf.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3fyryzccz.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3oyakokud.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3avhbfgal.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3nrheekrj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3lonnqnzh.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3vnhcdstb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ojdzbkix.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pjwmatds.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3hoxektov.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3pdayfjap.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3cituyelq.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rsxtwiig.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3vreumxxd.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3fsfmptve.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3sfixotnl.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3vksyrprq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ktwnkfbq.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cfoauuuh.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3lwgqzxwt.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3xyceescs.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3qwumfawe.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3lautgrhl.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3chfgltud.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pgfyyapm.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3vmffeksf.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3oapaottb.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3bdxluram.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3tmgjhzqd.html


<!-- 参考信息 -->