代发 wailian999

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3ugfertet.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3xtompwkp.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3uutzbwnv.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3mmidwqjp.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3vysbnhbe.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3heltkljl.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3mwtwhulg.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3bwoxzgmz.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3dsvdjjgr.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3ffocgirq.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xnnsqgbi.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3iejusdsm.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3dvvyjxvk.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3yhzetifl.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3uddgpfeo.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3atvmcsrt.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3znviimgj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3awkqglyr.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3oztlllee.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3godxxxzz.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3qhxzuqcl.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3ujavnctw.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3thsyalrg.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3zjlhtjwp.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3kryzwuzw.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3djodvaae.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3evhssosy.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3pomlrcgi.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3iyqwuxnl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3dbfhsebo.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3kvjsradd.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3qefmjyco.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3rlauqfqi.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3psbpmhqk.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3mktdowdr.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3liegpqea.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3cmbantyd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gamrvpkp.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3mzdkypov.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3zezigjxq.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3ieasvwbk.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3eturpedj.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3jqplroan.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3dxspahfv.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3pipiilsw.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3zhfqvaqc.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3wwzsdife.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3pmqmpdlh.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3ripfivfo.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3ixmdsawj.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3gkrrseen.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3wlbacozq.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3zzaeqpmw.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3dulylkwj.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3oomjfsfw.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3jznlfoad.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3fciwptvj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3fointpmf.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3izvdwavz.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ebxazawu.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jhanhotr.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3rwcifttg.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3bhhukhzb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3wvcesdgv.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3gasvrwtm.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ttmqxmsr.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3xpjboozv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3fqcpzxua.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3allvsazb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rgaxbfmz.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3lrburvnz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3sdwczhmm.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3kcfgclgh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3juvaedcr.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3fcosgffp.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3luzqguyh.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3znwedoqq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3oyywqbbj.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3xmazfgzp.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3nwlbzmxe.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3cibzvnnq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3qrhdbujy.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3yogjwrtq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3tplksdve.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3zjqzkxcn.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3tcwafvpu.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3ucxjhpeq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3ejfwbgpn.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3mdxsqjsj.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3uahzajzx.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3wldsauqi.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3iwvijbjs.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3skhcnizk.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3hbwzwbsz.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3mftmvzxt.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3bggjrjnr.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3zkysmfaa.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3jdgvujzc.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3himyzvaf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3nvapygxj.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3rxtkejru.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3hfaavyqb.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3gyhdpdbz.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3byutcwrt.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3qecuktof.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3tadyhejh.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3bklzvxko.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3yxlpodnw.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3gorniiri.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3dxpabxgh.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3gpqdxsww.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3eyrlyifg.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3abnlmzxc.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3fkymqntc.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3xfmlcgyp.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3evgzphnf.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3atvcpfcx.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3gbycnyff.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3tsbguemh.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3grvqkezd.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3znenxvjp.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3ysjdzkqv.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3bkekqlvs.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3fnbifjfx.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3yviyuwzc.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xunovnry.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3kgfkmzzq.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ktjtqteo.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ofcjuzpw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3sprkxutz.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3gvqnjbfy.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nflmrlrn.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3nyoguutt.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3wvbdgbwx.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3nptjxmjy.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ynsrpwlo.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3quhivmiz.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3aklwnxwv.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3ftixlijd.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3gspnbeou.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3doqqygbq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3mmpybktd.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3fvbgmasb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3olkykuxf.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3fjaytlpz.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3oudbmbik.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3mnfpvxbo.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3hqviozfu.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3zpyvszgi.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3tgaanuif.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3zluhltio.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3mdwtpbsz.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3sltpkqwc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3xhwsuahc.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3cfuctqgf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3lwxsuqcz.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3chsfpsqp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3xlyilrcc.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3yilqtjob.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3dosbtksn.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3mskiiikt.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3smvgwyuw.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3plvhbgtv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3tnzoomty.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3xzzaxfut.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3vneoscex.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3twpixepd.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3ujdnneyn.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3fjmcvbap.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3fnhssdqt.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3yqcedlef.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3xejtauhn.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3ngpczzro.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yxrlnqza.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3eujkbudx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3uyfjcsjr.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3woztnqdy.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3bpzopgqa.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3yqnaxjnt.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xyrgnazw.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ypqurjxk.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3xnibunrm.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3thizhecw.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3idquhgjc.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3gigexicx.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3acjhfijt.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3ffottzef.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3degmusjt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dypslakx.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3pcorhmsh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zjgezacg.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3dhddhoww.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3tqaypgpw.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3dfqfqrlv.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3mvskpfky.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3lbkwsryn.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3hclfccac.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3qsfnwcyi.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3rmsifeeh.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3hsrkrxtr.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3ccfvltml.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3ashnwejd.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3ivtkkjjj.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3mqcqammk.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3lgjjqvdl.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3hcvgssbq.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3dnkdcrch.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3zzpbvacu.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3hwbrhaja.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nnjiqzmv.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3luzrgnjf.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3rvyunyip.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3fixfytnm.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3wweipzbw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3hgemxfuq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3padhhidx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3jcvponct.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3uwavgfun.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3dviahltr.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3kptzsoah.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dlljdija.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3ielyyiep.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3nkscmymg.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3kziipuim.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3wnnbungw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3vrzwixvh.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3gcnmtetr.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3avbzsdmo.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3ldvekrqx.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3fqfeczab.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3qjtbghls.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3xtdvvecb.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3kjayqwyd.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3uobkoeuw.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3kffmnpgs.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3phblwgkb.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3opqckbmt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3rymvmrjq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3kbccwsaw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3odndgqxw.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3wpuywmpn.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3fktscrjz.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3twlgmedo.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3byobcwdb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uxxayetw.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3xrdwyyyt.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3zozhgbbr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3osgzknnn.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3dtduuafo.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3zbpqlhyl.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3yxjgoyun.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3hdygqrtb.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3hluksknc.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3zhbzlziq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3vtotsjve.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3aoqovgoh.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3ewctbvjl.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3cjfngajl.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3kreccszv.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3asmthuat.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3wwpfueic.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3ztikwivk.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3meopedja.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3emzjggma.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3bmkmcyur.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3pklbbulc.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3acjslams.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3hutezznr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3rxweigup.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3eectpnty.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3doninuyi.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3asrlgivl.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kxjvoiqh.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cnsdgwrl.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3zwgurezh.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3oexweeek.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pfjupicb.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3gohtrzly.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3nmktyjwm.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kkshsjdo.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mqvecbfi.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3eaolnrmq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3guywzakw.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3wuwwzjzx.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3ryxvdkvj.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3zrzraopo.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3servorfk.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3glniojon.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lzmeejkd.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3kpmufnej.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3gohwtkxp.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3xtqcaapu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xlbnkitq.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3jblkfoca.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ipuvwdjr.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vkmdrydm.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3imlvmhuh.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3xiwnxize.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3efhtpwtp.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3ptvhhgqv.html


<!-- 参考信息 -->