代发 wailian999

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2mptbudgf.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2bwbbqkem.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2yknekkok.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2ggxtyirs.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2qkknaqsv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2kfhfvefm.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2wthbtyut.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2fruzisov.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2bsafzpex.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2rbideagl.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2xipugjor.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2xyxkokwu.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2jliuxrsb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2bczbtdaq.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2kvxgwfyn.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2alpklajf.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2bigblmlg.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2rjzyesne.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2mteppfxj.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2nmvesoin.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2eyrtueaq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2urccsvdp.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2dxvnivlm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2vezqqmop.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2oecomdof.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2hqhayjbw.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2cdifbfzy.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2ntdqaobw.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2fhjniyrg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ziimncre.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2qusocprb.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2glklxydz.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2tfuekdfq.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2oxyyxkae.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2tdmpaceq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2ltfoqfll.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2mpeaecof.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2vbtfofig.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2xtwofxvg.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2orsdekae.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2aswwekao.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2vtraxfjw.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2wutgozgz.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2mxcognwd.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2waumkmkb.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2mspzvgtr.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2ptshydfb.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2ujzpmwoh.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2xndctfth.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2dxtykvad.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2fvsrguwj.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2temvalgo.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2rkckecta.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2gtjvgkmd.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2odpyeiot.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fhjecely.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2xrchedjw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2moisrfid.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2whlsbwdq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2xojjvvyb.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2crfpioea.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2fahjrevg.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2giykklbz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2kwyhocsj.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2xkksnbls.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2fmtxosin.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2wooxavaa.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2qibqlysl.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2nvgzzzpm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zvitahjl.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2chmgdgpq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2ftprqutz.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2esvombkf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2spngcvwl.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2sarjhblb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2lofkjqxs.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2bzfpvinz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2pfvuvvie.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2fnpbshqg.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2oyzmftff.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2aqkgomnd.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2oinyqnjy.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2bjxarwjv.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2lplemgrf.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2jpzcmeai.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2asbgwznz.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ozwnmotd.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2qygvuwrb.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2xniivdak.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2mlrunchv.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2zpbftaii.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2uwfiyxsc.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2ddiqkgjo.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2ijgzqozm.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ykoszazp.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2hdhqfula.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2zpvkyjrq.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2kcwdnczj.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2dfzrvryf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2mbtgvsod.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2vmdotcww.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2mtlvbykg.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2qcgbvnnz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2nkstgucs.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2cyiwzcpm.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2hcpiavxq.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2ndmzqvwo.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2anmjskst.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2dxroagyg.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2pavqetwe.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2hdlsxiex.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2lauiqgkr.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2dbkuzuic.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2lsdpgodb.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2wmyscyrp.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2wadpqqzz.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2ghqoatqn.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2qjtxlyfc.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2spbzmncw.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2wtlktpio.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jtbcbkdb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2ivdlsfle.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2gzwsvejh.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2haitzfrr.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qxfzspqx.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2tihqejbt.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2vgruygfr.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2dbnwbrzi.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2xnfypuyi.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2izeesoos.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2ewvazjrv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ahsdnbzj.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2frqylksq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2njdocxbr.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zfqtbtdz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2ouffiafs.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2ucybonby.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2mlsrpmrp.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2zvltzqdw.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2rvftclge.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2djlrnkdk.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2buawrhrh.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2gmutqlcy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2rqjbittq.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2mboozwuu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2haqjhzds.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2spbykifg.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2aotzbjcs.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2mcewprno.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2uwpzsqps.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ntullwev.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2lkujvsvp.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2nbbujhuf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2vyjngllt.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2lghgsebz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2bmfuaeln.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2gmsvbpkz.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2rpluoomv.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2mflzkvde.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2hmcwwasz.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ycpppiiu.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2grisadem.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2xgzosxcb.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2inddsvit.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2tgvwssjb.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2flizruyv.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2womqdyen.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2rhhuxxyu.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2jilxaidw.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2llkmfnpg.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2mehvhaxd.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2euggphyl.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2nlhhwtkd.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2orfbuset.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2gyjuxbdy.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2nvcmiqyu.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2tuvslqgs.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2whqhoqyx.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2dljumffm.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2tfpsknvm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oztzubwj.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2tzaqdwtb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wdjyesxa.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2dvadbarj.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2tvofbkwt.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2dwxliqxc.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2cirdryre.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2joyrawxu.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2eqmlmrdp.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2lnsldzhg.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2rpsqdswf.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2lgyfwily.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2pcoiiwyw.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2wbedrfau.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2pxtevhfj.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2ggprrwzj.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2vydbnotg.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2kzziyqon.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2ubjnltvv.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2mnwsjdzb.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2yqwbtrci.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xxqxxwse.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2jxuofbyw.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2eoapgmgy.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2taojxgxk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2emcocpov.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2rmhzatpc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ylhbdcai.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2vpznobpw.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2gewaflyw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2tcciaqzz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2yvtfjtla.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vwkvecdt.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2kgqezuqv.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2mamjirdf.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2wahulewh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xkpyyqhd.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2xnuwhouk.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2cdfjtcsd.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2zgapffjq.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2olzifubg.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2bnlkwalf.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2lgyctequ.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2hwnokfoz.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2booigcbt.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ljzbmsxm.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2agwdwplb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xwemyqhz.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2ymjypqvo.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2jmwzsmyt.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2wmoagmfp.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2dtlbjlfo.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2sghvhjru.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2josxhuxk.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2mufiwdgw.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2qevnltcu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2atdpcxaq.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2fclzqfcc.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2affvzxfd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mdrxapin.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2rogekbet.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2lufjsess.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2ziktjnbs.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2csljeduj.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2uhexrbog.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2qbxonofb.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2gdqjsaqq.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2uautgnwv.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2wyimapcf.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2inaxldkv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2zjipjoxw.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2yvxcvell.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2sbfbroyu.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2bhhxygyk.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2ioaewdch.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2kevchozf.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2dzcbxtyw.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2uzllsoae.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2iazektzp.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2zxhcdifm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2exuaewox.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2dfhzzzbr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xzssajyx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2emozewmo.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2novvlvvz.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ksmbxwau.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2lynrfupp.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2munurmbl.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nnkxjqqd.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2uswhopgp.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pxxbidef.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2leiblpla.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iofomiom.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iqfdqogk.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ntmwwwaa.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2slhaaksr.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hydzoljl.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2jhaotkcs.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zfnvxome.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2afhmgntn.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zpfrusnk.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2wggrucqw.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2meimtojm.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jcnflcdu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mctufutp.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2zpktcicg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wfemwhqj.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2gapnvsdb.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2vfmxudjp.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2cxnzsjce.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2nimvznqu.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2dawygkwx.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2qydfeklx.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2occnocny.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2zuufdhcq.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2xwlqwzwi.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2vqidfwgm.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2hxqoxjpk.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2eviehjui.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2gbkhenqa.html


<!-- 参考信息 -->