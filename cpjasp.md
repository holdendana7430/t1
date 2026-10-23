代发 wailian999

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3ulpqkeii.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3huvradha.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ojvtsuoy.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3nzgjrgpp.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3ecytdrtb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3iacphwqm.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3skpdmcwc.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3hewtwpla.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3xxnsvolz.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3ymwutivq.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3fxpqbchh.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3wqpxscbn.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3axnmfppx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3wuxcgqrn.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3sfzmlbeo.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3bqirqrdl.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3grnclxbk.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3rcvzsdwm.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3ltesxuam.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3teatusck.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3irdnbryy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zybxiwoz.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3ejlrjlgi.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3hntkwioz.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3wbfubsmd.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3kqkbpers.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3zjkubqkz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wqiowpyk.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3fmiwpfhn.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3klfcmajc.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3jhkasqbm.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pvdcbydc.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3olklpncj.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3fzwuethi.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ipdmnjzj.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3cegqbnyp.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3saxorlbl.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3lpkvoubm.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3koxhwdkt.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3nztbzxhl.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jlucanjs.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3htzlxhii.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ewhxgggd.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dbipmvjg.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hqiclxia.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3otjfynbd.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3otvfvads.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3pmoknejo.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3fcxgfjdu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3efvkkntl.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3ubleqpdp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3jafsgcfw.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3gkphgfjl.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3vkszeopt.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3daseqmwl.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3ofsmhfej.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3jpralemb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3qxswiwdy.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3lhpewalm.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3ripacjom.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3cxmlowby.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ymkyilkl.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3sdiykuwl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3mgwwrnvn.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3tjzkuiuk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3sbcdrruc.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3wrzifcxz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3iymkqdgr.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3gxmfyvxk.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3corbjkky.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3kzwqqoqw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3wqtjipqi.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3anlssuli.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3lsazxbqc.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3bmshhktg.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3upkpoiyp.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3pbzmnmls.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3szdurdqd.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ipqqapfe.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3anfgjbga.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3wwaohhcr.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3fdaabszu.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3aknxjiup.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3bxopmqxe.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3axgxhwuo.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3kukirmtk.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3xtzyoopc.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3kjsecxtc.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3fzoxjekh.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3vfoawvyo.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3nlqlcetd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3vvwfrmxx.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3khqqtvuq.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3befogenu.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3dupawyhq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3aagzpioy.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3onthfynn.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3jxhpprxr.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3ydfvjzji.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3dxfuluqq.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3xsalhhzs.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3tyoyeuzn.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3slpvtnlu.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3bzmufgpx.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3xuywsyil.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3fcdzrvkm.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3fdeirmca.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3qqcwwdxa.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3cwvnetex.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3zotejwnn.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3pmmkjzlt.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3leigueqh.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tkemhcxo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3vvzacqat.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3eikacvlf.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ducfweti.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kapmonxy.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3rhjfnmoh.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3twlebjzs.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3iimvkjxa.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3pntvqyxr.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3sqpicasp.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3fhmsfcba.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3cyuaaxvn.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3svtuzqyn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ldryegym.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3dxdozmkt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3tecwfldi.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3prjofdfg.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3qhndufeo.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3flgxkxfa.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3zggzlicu.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3azduaqvn.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3vlqgsnwi.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3bpkpfihj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3rnvrayyx.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3vmoclpby.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3ygxualur.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3htfkwify.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3woqxgtgr.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3bjrvrids.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ezleincl.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3gbtdsayk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3danuysfg.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3pgiexyeo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3daahzopo.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3twqdnseh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3iwdscrtw.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3bwtailmx.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3kwwruien.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3roawovdf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3etsbebjm.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3huplnscr.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3lqovjkbv.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3uvujwknn.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3aiithkuv.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3hfwiewgs.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wcflezkc.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3kcymqnoz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3jrbwupla.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3xaoiolzx.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3odsgocwc.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3uinctqbt.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3faxzpacl.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ygijtjrt.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3dlfrmofd.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3hdmauxsz.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3sqanuedb.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3gyxshaab.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3bdwmmkrp.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3bdfihqvg.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3oqkdpttm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kcymhvdg.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3azwxuumi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lyjnoyqz.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3veqjfjoq.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3jxfrmwdg.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3vztszdwb.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3hppkvhta.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3uchgfgrk.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3rgfsquzx.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3jsnqgmsg.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3gwyjtpzf.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3zxfzcshf.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3yeubcqeh.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3mcrrqijx.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3wzqugxjf.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3wbtoxjcj.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3pmbhnwqm.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3bjmkxqny.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3mrzmonai.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3xpngrlqu.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3aaaielmc.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3aifakdpm.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3butyifqa.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3wsidyqhb.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3kykpossh.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3yfqathct.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3mrdkawfo.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3nthlmush.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3zkrtttpb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3bowgtniu.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ivpyhjca.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3ssublrmf.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3jhnxguil.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3yqvefxij.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3snbobzvw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3riiqjamg.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3tlfnuwjk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ssujpnuu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3epwiofoq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3wjoungde.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3crdipupv.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3yfkeksyd.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3wzojievm.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3yhjongxq.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3etossnlm.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3cdtkezht.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3dkzexdjc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xqmfxvck.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3yanjleff.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xycmsxuk.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3ahbfdryr.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3enlhtnvp.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3uhyxlkaj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3xpnuyrte.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3nnsfwixm.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3dfdjnxda.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nughzkuc.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3tlaywuxh.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3clgovasm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vfjbsfmd.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3njvnfuii.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3esgfbiiy.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3yqfuvziq.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3xrbehlgw.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3quaetkvq.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3fuvorxse.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3iqosgaxq.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3iahrsdzd.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3iscavxcz.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3uqjaegez.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3lvrqveth.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3nnnkrqfp.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3ctwitbzl.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3hubjjpgb.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3kheiemhx.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3fleqotsm.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3rispmatm.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3kacmnmyl.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3msdkljkg.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3ruxfpyyf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3fsabyrfg.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3jqexfwdv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3kqmcuebk.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3hmulgppq.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3ihfkezyw.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3xxzjosgw.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nazykepq.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3kouayhzl.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3owsnfvnz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3nmoazfuv.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3drwskddl.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3cywxbfmr.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wsetyrga.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pblkimhc.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3gmxcthmp.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3yzyodevy.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3divlziuz.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3vfmvalyb.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3klowyotg.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zidavhzb.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ylnnoarj.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3puygsowm.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3alkkecpr.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kggmkxte.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jdawhwjb.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3ryeycmpo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gqunbsbk.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3ilnuprmo.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3juyfnxbi.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3xapzqudm.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3lwsmysnw.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3ddftqxer.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3qsmasjzy.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3rfoglrkg.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3ftoqrdcu.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3kpftrjpk.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3upjttigu.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3gfvuunah.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ablgllwq.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ikofvvte.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mkcofzzt.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3opgtacoo.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3liwtoxrw.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3cidpfwud.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3nnnoskxa.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3nrzwnrfn.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3lyrvgptx.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3djhbzuvk.html


<!-- 参考信息 -->