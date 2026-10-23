代发 wailian999

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3sacslxiy.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3trmditku.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3tawuexfo.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3pwrwkyje.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3letkugqs.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3rhklawve.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3ejdyzcnp.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3shzajhez.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3rybbihfz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3gvojfmov.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3jewltgez.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3ibkccdly.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3stnzvnpq.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3xodjdmqs.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3tiudyaml.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3vtqayyno.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3hewmduwf.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3bbmxjccu.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3ypkjbowa.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3piqnjhwb.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3mmfqkfod.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3gtjffdqn.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3cdlzkeue.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3nmlbqalx.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3fmxmrlrw.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3uexdvxzp.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3bjsjwhnf.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3hxozdfoh.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3yxlvmqwv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rejlatqh.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3jowvmrlq.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3unxjstmn.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3ubtrquwh.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3zetxzaap.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3pmzzgwvl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3kgnezfaa.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3qzuwqwyp.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3theyqlqd.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3nxjgkzgo.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fzpqhxqw.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3hikoqdds.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3dspvoinq.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3zymmhqek.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3rfhjemsv.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3esjkaunl.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3kdnsafwz.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3mmwfbgxx.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3xwfqovcc.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fkpgmhoq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3kfcjrjhs.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3ifmaycin.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vgxzfnsx.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ljlmnrxm.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3pfwmzzyz.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3masdtwki.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xmwrqjvi.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3adigdksb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3wugpouzx.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3vtpcgiff.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3gdtgywxo.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3pvcswpgf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3jbjdyhqy.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3tquxgqlt.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3rwmuesqa.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3lqepmxzm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3mlapnrql.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ivwjsxae.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3wvzrftia.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3kdvahtyx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vvrnnzsa.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3dlnnhxkf.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jummnlse.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3efiqwonp.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3zlmnlysc.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3aayrxwva.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3dfdnwhsw.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3vlybnzms.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3aebnijud.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3agcsrfog.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3cqhnvajx.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3vundncaq.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3chxiboww.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3amkwtzyc.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3uvwfsmud.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3lwbxseqn.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3rotcmhvj.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3pfyihtol.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3wnaueccf.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3vkvcqaif.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3cbwshwmw.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3ceiutrfk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3yowkwmbp.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3gxtfxwiu.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3duozufqs.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3zcrsngwh.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3mgbfbvpi.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3rtqrkhse.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3qtsgedmj.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3iqjuvxrt.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3wqyfpvig.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3tlrlwtkq.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3pjnqpdzh.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3ypirmdvy.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3eqphjirb.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3pffaqwja.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3zffwnqpm.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3ypfpxxfb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3hxygpeka.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3fffjfrkf.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3ijttxkyt.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3lssghqlv.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3etsejdpu.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3adfrawtn.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3qpokxqdr.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3mnkphtln.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3yyxjhbas.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3ikynjcah.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3wpwwjdcx.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3fagbkjlz.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3rdzxoxyb.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3rcmepzao.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3zlcrxwoc.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3ltrmqfap.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ozdjtqcf.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dqottntb.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3sreyoibe.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3bjvgfaco.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3apzannyt.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3cmktjnqq.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3qkyveykn.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3kcntcizc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3sggooikj.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3ltghmwrt.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rqjageqb.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3tfdnpwus.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3ikalgfhy.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3kbapxebk.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3opufmcbp.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3xkosteoo.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3esmjcwak.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3ihykeuii.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3ynojohmg.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3tdkbipdk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3qiquofrc.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3mwxwnmas.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3oqdjvwld.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3wbxkyfbo.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ledrexks.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3ucrlkwpo.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3afapyyjk.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3hvzmjmod.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3laieewjm.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ablrcyvq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3floeygyr.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3cfcfjbpo.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3dfxroedf.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3cjzoraor.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3pabosxkt.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3iqjzinbc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3fvlfzhju.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3pxnqvpdv.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3rlcpkrsc.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3mrabkxdb.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xoelpwoa.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3ozdqefra.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3odlfddug.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3eeqhfqyy.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gezlcnkr.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3mubdvttq.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3vtafsjpq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3vavusyyn.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3zluunori.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3bjnsloor.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3momzziia.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3xvmbysqg.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3jwpraady.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3urclemcz.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3gtrsyhow.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3gliwcfbe.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3alnekbnx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rqgruwpo.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3lffcwcix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ftlqzkel.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3pgoqccad.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3cblrzkqd.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3bppuyata.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3iacqhzzq.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3odqlraxp.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3eiilqzvs.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3wvskcycm.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3vedkxwpk.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3lxuqelwp.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3cikiatmk.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3wykjprxt.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3zcxwhiiv.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3frowjmza.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3gcjipajz.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3mhsnwrai.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3nczfyyns.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3aeubycxa.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3duxhxkxa.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3tkavvtxv.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3mriqwffb.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3usmftbhf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3uxfwsxgq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3wqatiecc.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3qflxplin.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3vmxtpslh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3cieosjwv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3beagkyom.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3blexpamz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3kxzwnsay.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3muxuasgc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3krolopxo.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vuakqhuw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3pjrekxeu.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3lqbgzuex.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3slhlqosh.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3nloryrxt.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dkhmadlj.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3eltgodbm.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3kkrdkcmq.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3wijcxura.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3vjaexobt.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3ljvjnqpn.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zkwnvnnq.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3cvfjdvql.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qgobfexs.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3kustcpzd.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qrtuxxoo.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3gcjpofrp.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3ahslgwuv.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3vrzzbvbp.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3hgmzmdmj.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3lnihnyhz.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3fppgrmlk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3egulcvzu.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3iywdbzzj.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3xpruhdam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3opazmehk.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3dlklpwwz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3tcpfdhtv.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3meklyjcy.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3ziyetmyr.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3iyagcyqc.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3pwwvhhki.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3dfhtlenk.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3kaiparyn.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3ouaxhusr.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3lmwubglu.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3dgznhaza.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3wliltnxo.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3jhfvckek.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3ayumkhbs.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3ukornfop.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3skrfrpaz.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3sgvkcolz.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3hximhcdj.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3mgntgjoj.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3ffwbfagd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3aqkjshcw.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3lzusdmfz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zbewmlbf.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3nhsbiatv.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3njgascjq.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3duqapkwx.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mereibok.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3iexeewby.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3txzskfnd.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zrtxsxrw.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3hjwbokyc.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qjjkssul.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3orlzirwz.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xfnjgrwp.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yiiizwef.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qexnofwa.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3phjaenrm.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3vhtnvdci.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3brampnnm.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qwzjrcez.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3bxtctsqx.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3vlwwwtgs.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3razkdxkm.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3rauzaldc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ckdsuhyl.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3cjjkipkz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3udnligvz.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3drnyofuk.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3snempqhs.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3koeaunbq.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3aprgpyia.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3lvpwwusy.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3cuxtiogb.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3gnmhkbjc.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3wbbncfpa.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3cjeieapo.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3jkafuumz.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3tiqciuwh.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ufdwpxau.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3etzcyase.html


<!-- 参考信息 -->