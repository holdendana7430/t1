代发 wailian999

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3dtsfsfja.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3jippkois.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3ezkrocll.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3atsjmgmv.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3vpvoxhkz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3imbpviyx.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3efjeoiyu.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3mqvlwvxb.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3mdviizkm.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3htvggdun.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3bkdxtimo.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3tymsgfrz.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3owumaqxt.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3tmybwbnq.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3dgrtxicj.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ofcudwkl.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3zarxthec.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3zlcdklbl.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3skbtcsyy.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3zpwsteap.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3nokcgkxp.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3ygqfvdue.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3sqxwhqtn.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3iinzthni.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3yxkbzlml.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3shmzfwjj.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3hugtjkit.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3yfgrwnpq.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3tsauxxpr.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3lixjkzwn.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3sljcexmc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqrgfmop.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3gbeodlyt.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3evlahqui.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3ijirsguu.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3zifkkfrn.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3ijhpgqmv.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3gbdjughl.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3qsjuuqrv.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3chaluqgq.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3kyeqybwz.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3itmvkeqg.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3lqvueqcw.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3hrpebfst.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zlzrvhte.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3qsjbxbmb.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3wgwrpiju.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3vajcyrtg.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3sczwtdpb.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3rdstlvoa.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3hcvlfpqj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cyjpjeuq.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3ffckfgle.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3kwgjkstb.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3fufvdjyk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3qheqpxou.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3oegcbeph.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3rozbomnn.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3vslavwik.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3ebicbovw.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3bthfdaro.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3ewdkboan.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3oewofixq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3lynhszuo.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3gbjmqiab.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3akbimpzc.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3ffmlgrxa.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3gsbndloz.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3ikjxxaax.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3wjwmhifn.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3jcvvugxz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3sehlweha.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3tzclemtj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3esvyiqek.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3edjisgzk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3prvqqqik.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3mvdgaolt.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3dikexobi.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3ofazarzh.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3kwgzzire.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3icrzzmvu.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3vndckkjr.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3yateiceu.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3pgpojpsu.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3zytnrlsh.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3lxbzqdtj.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3moisvkqz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3ipvoaoax.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3ouufxpnj.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3pskcaeqi.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3zqwstcni.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3arxcawos.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3meiwotcx.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3rwrlsjtb.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3mfajfukh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3cpabsial.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3fofmxtkr.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3gtytztmw.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3vwzgrsrv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3jlkkiphg.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3dcobqdzu.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3wjgzazso.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3rflwpyqu.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3ldflmakd.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3fbsvrmwr.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3fnffeosl.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3bgomzuhb.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3fmxohiyn.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3iymhetpe.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3wugnkrqb.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3qinmdofg.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3zrdjztmq.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3cyhkkvop.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3vkitkpzc.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3mtquzxfx.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3bzdegxuo.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mijgoehf.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3cwzdvlfr.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3jvsgvpyr.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ppujixec.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3ickkbezo.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3aksxeecp.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3kscuvylu.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3izxchytt.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3zrghkvnx.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3hdnracdr.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3hbzyexqj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3olskattd.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3efzuwnhh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3yqychlts.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3pixqxfyj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3lwkqsdod.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3gbtksydh.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3odsjrods.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3qiwtnfko.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3lvfyvlid.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3mkifyotp.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3poixoyej.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3gmtfviuk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3axgwxmoy.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3hbuocbto.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3fiicsuba.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3ugcacscg.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3txuygrvj.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3vealyffa.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3upeevozx.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ghesdgid.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3sdigfgtb.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3mjpxxkoy.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3dfxrlbgg.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3kjrbizft.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3ywbsjhnu.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3vyenupui.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3lorfafjp.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3nunqyrdm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3sfavjvht.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3fomhhsmi.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3ytwyhndy.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3adrtrsmj.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3owmvnywn.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3bzgkfszj.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jnhzpjne.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3sdmuzooc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3kxyrzzry.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3rlqqxmvk.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3uywadufs.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3zmzdlupp.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3ubmxunmy.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3qnraifzk.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3rwtauoaq.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3lijpmukj.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3qtoxglqv.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3nqjoibwa.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3tuuporfb.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3ehnbzgcz.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3jaxowrka.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ayvaeaxd.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3tlaateth.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3owqakkjt.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3oeitoiuu.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3vcymsssx.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3rjtdezht.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3cjtbfvzq.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3mqkickaw.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3vfzjcspy.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3pfexuuhn.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3gwzdhnnv.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3aowanwpq.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3ukafohvs.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3vkzkoryu.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3cbkearaq.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3wwzapygj.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3lhtpntul.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3tefngmoj.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3lpktniyc.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3mocgxfwq.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3kqywcvwf.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3yrpegqso.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3qhjggiaw.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3chhlxpnk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3evppyarc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3jvdkytny.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3sgokugfp.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3jqotojmr.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3prhhcgmk.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3nriummns.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3dtllthtw.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3oiaydmha.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bdnyiihy.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3soeivtya.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3gjmfhqkn.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3udqxhmvk.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3nceofzrd.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3xytighsd.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3diqilufc.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zgdblxjc.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3pafuitle.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3peuszwlg.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3zgvafrhn.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3avchoryz.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3uruuuoms.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3pnasxheo.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3qcgfghrp.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3wkizyuck.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3ihikztbe.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3itlfsmdh.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3cnnyoswr.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3gywgvlpn.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3vejmpmcd.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3uxtmgttu.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3qgwzczdx.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3teyxclqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uqzmzrsk.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3emtrkrog.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3afgxaubu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ccttolcz.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3rtzfsgnl.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3lsictnai.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3todjrwsu.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3zbpcrpah.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3hvffjpcb.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3gwkvwiff.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3dxsgmiwa.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3bkhkzkes.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3tiahplqt.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3bkpwukjq.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3zffmhqck.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3mrqfsfgq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3mcxuepsb.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3otthrefz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3ivdfwvjh.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3ecqbfhou.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3whxrildk.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3vrxicsjr.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3vubbqahz.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3heacfbyx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jsvdcypf.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3soipgbjx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3lhihuykc.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3sejzcwgv.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3wyoczrss.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3tzfluxfe.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3whisojcv.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cjkrhvug.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3bdfwbvwf.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bkqanryu.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3koloqmvc.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3wqgbwdyo.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fgcnxbpe.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3eqexsypr.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3cckfudbz.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3hwpehbtm.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3loahjmad.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vfjsgtgx.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3amlplpyi.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3nkdrltoc.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3pmnmabad.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vofnaixe.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ukgcpihe.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dztlgeor.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3szkzvepb.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3zvnezzgy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3glbfctrj.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3zxhemsfv.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3kqcbshfy.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3fkvomjkp.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3blgpyblj.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3rrtqmfkw.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3dgvrjpoh.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3maquqxrd.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3xddjxypg.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3smvwpbba.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3veknfuzg.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3nsffagxf.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3nuayciux.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3zlapdvta.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3tdmxebxt.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3qbwdlvyj.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3cjlceyja.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3udbuqgyn.html


<!-- 参考信息 -->