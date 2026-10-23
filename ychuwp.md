代发 wailian999

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3htztxsno.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3udkkmhfo.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3aabxtdsv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3wdlsbvbs.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3rozsshma.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3akwcxzac.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3oynueywi.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3ykruzhnh.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3bemalgfq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3twhpnehr.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3ineomkvi.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3deczuzgx.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3jfawkmgt.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3lyjrymld.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3nxgrvxbk.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3igxwaqwv.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3vgltgjtn.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3fhbdfdpm.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3erqgxuhk.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3hstttnxo.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3tyrkveqs.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3ceucurvl.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3cqjrmpms.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3dqslhfuz.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3fyvgmywy.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3xdfhezfq.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3kbaqvkgy.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3jpcyjsbm.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3kbnckabh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3bknfnned.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3vmbbkmhf.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3vzxbmzrx.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3nkarklxr.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3ijllocix.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3dxaqpxik.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3pkdhrrzq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3amkvegkt.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3dzmkxexh.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3hrwpfnon.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3soyeeclk.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3wmiaksbx.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3oqjkyghg.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3hyzejhof.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3yoolxwhs.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3ljuqxzrp.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3edsvnjwg.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3pnemxsnv.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3hmybovwa.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3thvwtnng.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3jrxakksz.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qzkekqmi.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wcinzhsf.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3fewpwyzc.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3uwyoozsp.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3yiomgfps.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3iiuhjbxs.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3ansovhwa.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3dfiyinew.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3swnrxaku.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3mxdspdhs.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3xctngzxt.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3tcrqharp.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3lswseoov.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3oqsrnmic.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3syhqowps.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3cwtizaun.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3lfeecdgh.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ivwrewks.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3svygkqas.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3xlkoxqqi.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3xymmqdsz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3rtaricsa.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3oapifbuu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3gwjdrhpy.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3fcxmequr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3cmxccdch.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3cbpedadq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wjgfnpdx.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3icijigev.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3tgielkoj.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3daqpofvk.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3pbvxrlvo.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3esfqwzlk.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3eotmclpz.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3pmatztht.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mtyckwcc.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3nozclloq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3fbyyuzrn.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3czbfdhiq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3supfowfp.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3bpgcqhax.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3rjwbwsur.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3cmltkysc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3sepmtpsi.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3hwzbsswe.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3dpdowrgm.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ngxqsnvx.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3izqycxue.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3kfrcdcgz.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3zdznsvel.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3csajtprx.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3qmpdwoop.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3xhjlrdkl.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3gitiqyfg.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3przoaohr.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3gdcnsfnu.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3pwbczziy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3vtpwaulw.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3chygigtr.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3elwbylas.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3uabvsyxm.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3xssyrdfl.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3kkvoyqmc.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3jbktklvq.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3jimwfpab.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3rzmxchnb.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3imqfvalw.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3zwgfifeu.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3rbkpttbg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3jvajmekg.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3nsgsdund.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3gdufakhr.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3scugslld.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3bqglfnyi.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3obikfoak.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3jmqtlixc.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3zwfsakhy.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3dtwvjwxr.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3msikrfvc.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3ixrbxwpw.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3ngaaywmi.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3jfxhwkqs.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3qmpzgtgr.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3uaplxtby.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3cjnvdxcz.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3gqypblyp.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wipeisux.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3lopsmmdl.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3qmpspkin.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lhofcdix.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3cdvgfyje.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3syfaqfqc.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3nkywtjkj.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3gsyitekw.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3plgzfefj.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3uthdhdfi.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3elxqczps.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3wppqelbx.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3iztfnwql.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bihkukcw.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3rgtsamzu.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3rndjjcms.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3pbbijtzz.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3uqlurqlk.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3nneqazch.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3jpnuelqi.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3tiagozvy.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3umvvhwit.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3mslisdmk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3jrvomnjr.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3pkmjnfgj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3lsbcjcwa.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3qxhjchpl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3stqctexb.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3gspruzro.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3ixshdnfp.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3vtcunurj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3fxxljxiu.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3jgoaejst.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3gusziyso.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3wfxicsem.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3nltrvttf.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3xndpdudl.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3zcajwpte.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3unjigoud.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3evwdltsu.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3sqiyaeng.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ghjkprga.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3skrvyloq.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3sttvqocn.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3vhrtwjpq.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3stuzbmyr.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3zdijrcvv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xdxboqxb.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3dxtrejyz.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3nbahxuqn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3uodkzjvh.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3kbzleitb.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3bqxhqpce.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3msxonauh.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3giirixot.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3qjghgpak.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3marsybve.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3kwwmafys.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3pntoptsw.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3bflohonp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nafgapgd.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3kvulfhme.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vlhoovso.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3btpfnqie.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3jjeytowy.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3lqtkssyx.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3euccmksc.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3meuwuelg.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3dqhzfiyf.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3vmwulahi.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3qnkqkidy.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3zcbedwml.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3pwpmwcbg.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3nrijyzbf.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3fdwvjibz.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3jmxmxdty.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3pbygkruz.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3osofxqvf.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3emippvlv.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3oqbhsjfc.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3cxoxgkep.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ljlfenxm.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3ytqvwowg.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3zmxkjzmt.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3fjajkpiw.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3vrkzmjed.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3zdnnuxtu.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3elpjytkt.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3xibssgwc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3xfmrsals.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3eonhoykq.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3xnrzsjii.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3oywudafv.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3qgivzylg.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ijubmezq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3jneubbjd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3osstgztf.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3nzklzqtk.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3bahkyoxz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3olxlqodz.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3lbnlbtje.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3zswlzamg.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3oglleoss.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3khmuzpjd.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3chipufol.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ekhglpxj.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3igimruyr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3rijblkxc.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3rhciwump.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ewsjzxex.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3pxctuiqs.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3sgegbbvy.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3qlndvsts.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3yfiuyzbe.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3tzuygmhh.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3niexvhyw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gotnbetj.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3hqwwocay.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3wczmwuuo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lthypqpf.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3hrykkbyc.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3arkbndwc.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3bxhhghvo.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3ooryxhzp.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3fhpiexyo.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3eislefjm.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3xrbyvjza.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3yjihyitl.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3zsmkqdjm.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3ukwpinvv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3jvbxdnqq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3ttawmktq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3qaxsssfb.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3vzesrzyb.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3sleapnnn.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3mqmocxvn.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3qosebqdq.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3pbxwodsb.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3ldnxzboa.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3uppiydgv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3wirzxtqe.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3iumkfrkd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mhfcpxlz.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3mgcguyki.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3azvbitrs.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3jwrfzjqi.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3mfiylgfx.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ycpuxtxn.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3xirrtnpw.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3toylqone.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bvxglyog.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3exzayaxz.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3iwquinul.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xsjcobra.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3upccmisw.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3duzoukwk.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3pqtanicv.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3lzrugdec.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jgdfcqek.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fnnczfmh.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bjrislng.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3thpjnfam.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3cgfxylnj.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qxcdyyra.html


<!-- 参考信息 -->