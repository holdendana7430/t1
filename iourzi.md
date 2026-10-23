代发 wailian999

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3orgdsowg.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3snwiblcn.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3jblkriyq.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3ikpubiuw.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3yubqxzgb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3iufjubvs.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3qlzwdndw.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3lycayihb.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3inufwofp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3miqulaoj.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3duzvjbjv.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3zklgkyuz.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3ndjnizdl.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3rywirgqe.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3qhwiyduf.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3kskqpckw.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3cjoyrvty.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3pvhrtjaj.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3ioqcytzc.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3dtqjbnhv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3ljyrmypm.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3xirbsmmk.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3kkxtaoje.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3lywqiicd.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3oixseykk.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3ztxolzzh.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3getufsbp.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3aktvxkzx.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3qmvpsirr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xrirqklr.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3odixdhtx.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3bjpoohgj.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3ifyettzs.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3roeqfngo.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3leiiycqr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3rdqzhvrz.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3icviigwy.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3oqenuksk.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3kdyvojff.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zorrbjxa.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3diqpeajf.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3pdlzjmdu.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3pabvkfrb.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3kbdrrsdi.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3uuxfegdd.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3pcokfudn.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3jwfzgagk.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3vvnjzltr.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jeexcvzm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3nyvbcjjp.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3qwokntff.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cmlshyga.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3mpidzmcn.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3owibgwjq.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3jwbxocyg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3qhezkfol.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3wnffktvq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hsdlefar.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3gawcvtnt.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3uijxddmv.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3dxfdqwsn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3oqukvkrb.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3vgjaccig.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3kmakacad.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3whkkzqys.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3rcktzdhc.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3pmywerih.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3ucsvqbdp.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3rkntjycb.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zjzomjug.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3uaqzvqqb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ehwkmkgq.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3hviggfhm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3aivegjbq.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3slpptacz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3nbgmooco.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3ybtzadrv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3zmcldymc.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3szewytvz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3xmecfcrj.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3tebijzlv.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3nnatracp.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3qjoriyeu.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3cknhyjbi.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ezlcjcnn.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3erexchaw.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3irukjumt.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3kfkvljjh.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3jtpowxfj.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3avcffeka.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3eazvjveu.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3cnmzxsbk.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3dsnstyng.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3mpaefasb.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3brtqxtek.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3ucsorgpq.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ndcnxvmx.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3tcocphow.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3oyekpolp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3qkkfsadm.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3edpmbyws.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3xvezufus.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3aoqwpzkf.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3feoqkmfq.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3ajchapwo.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3bmtttbbr.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3nnooryws.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3viyopqvq.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3msfkqmux.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3sknvgxzd.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3jmutossq.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3kocetjxo.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3msarzhbc.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3ttmsaqxa.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3jtbljcoa.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3ugfupsde.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3sgpvsltl.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3kivhvvxa.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3idxeazqj.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3xcdkfuwh.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sqoxzhab.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3qqhozipi.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3liujtdxg.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3kourdzir.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3urbobqfv.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3snjmtewo.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3lbxqtzag.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3vdabiikx.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3tubmjrqw.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3icrpwpkc.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3espkwpum.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xtnefern.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3edoozspl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3evckydkn.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3pqaynelx.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3ixcwpbtc.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3qjyhdydp.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3edpacjjl.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3tzetypkp.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3tckvnrcv.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3uvblshlw.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3afzrwwlo.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3rusiwbhj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3riswkmpn.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3qvsmpamj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3ddyursqb.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3ddfqybvq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3nnadklyz.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3kwupcylo.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3osnmndyu.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3verdfdzs.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3ftnbfluh.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3zdqvyaza.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3frdsfokp.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3qjhfdptj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3eovzrhqs.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3mysibabr.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ggeqdxdg.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3uavbrkds.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3nmtpzdgu.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3eidctzcg.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3gqmjzkuh.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3kmpkozsf.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3muowupbo.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3nkvvvqoc.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rdyjmyat.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3jdnbengt.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3yhcystxs.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3badovgxj.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ebstlgnc.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3qpkdgqff.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uejzjjwo.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3trtlpowv.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3pmekmjwk.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3nryvwcez.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3karxgklx.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3wskflvax.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3wikomonl.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3ldteeyjo.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3zsqfknsg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3shqabmtx.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3lrcqbvme.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3maolpmmc.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3dxzcslmd.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3skuthzei.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3qiwicoub.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3zfnpzpiu.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3mkqjxyrt.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3jcslvjhf.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3zwjmufeg.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3sxirsmul.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3gowrobts.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3lzhojogr.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3fbbvwmil.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3vxwcnirk.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3ztuxmmkr.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3hyxfcfuk.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3hfnpjddv.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3fbtlkaib.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3bolxcuph.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3muvlvfhs.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mgdgjmqu.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3csguzssq.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3ffqkhjqx.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3troaxfoe.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3cttfxalc.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3pxjwmcnz.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3lrkxtkts.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3uzepeiuf.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3fkckhtha.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3fomckqjk.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3poriqbkl.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3aknpuzil.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3qyrckhsj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3tycbvupl.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3drrwxfmv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ogtkqieb.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3vunizrfs.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3lxbvhnjc.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3keocczgb.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3amsyinqq.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3zlvzmlgp.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3hmzgzarx.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3lzhpkjlf.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3ocfhjfnf.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bcechosz.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3nbdxmlvr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3mrzcaqzo.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3xgefrphd.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3imoawkuz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3qrpngctw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3bxahsqdd.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3jhnhmuqx.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3plgulhjd.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3ngngzaua.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3qjyujuyg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bdexewlj.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3wxbipvns.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3wgujjplk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rlrtwhym.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3lyaypiuw.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3ylxjxqhe.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3izhkzcog.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3hzgcxgay.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3sdzmeorm.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3yriknynm.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3spkcuodv.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3vafgtjsp.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3fxbsmpgv.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3bijdvrsf.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3vfmrqfxq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3vbsmzogh.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3wowlxqfs.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3sfueiovg.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3dxqptsxv.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3yaihjnwp.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3fhypodck.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3puvscjug.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3mhjyrdil.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3lfxwfcti.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jzhkzodt.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3nqcktcmq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3vqflxfmw.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mvbubuvy.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zefzntio.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3egnodvrs.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3qyrdbjsc.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ytfqfnao.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3podtuwnb.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hfrgyovi.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ilqvkwdx.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ytiihfgj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3gospiuiw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3oevtdeby.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3fpeqaonc.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3gqrmkxny.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pqdlnwck.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3kgnpzccs.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3grtwptpx.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3ujgjmfio.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3njssgcgl.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3ecwmsplo.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3sgbhnwvz.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dpsyqtaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oetuzbrr.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3lovgygno.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xfpirfvd.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3engvfvjz.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3vdgfvbcp.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3lhwjhyxp.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ivpxrjbu.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3gqrjuczb.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3cqvzotsw.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ubgwramz.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3qtkghlff.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3bmxhcerh.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3mzggpawu.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3hhsoltxi.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3lixlzqyl.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3gjlwzswd.html


<!-- 参考信息 -->