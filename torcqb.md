代发 wailian999

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3fpgdcbqq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3ssjjjnsz.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3hrpqhaco.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3xfwqvajz.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3scbehqtb.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3yfppijeg.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3chsmgdzo.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3tifqaxid.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3tnjpoacy.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3uggpybpo.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3itaqkkss.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3isdnnzvk.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3ocmoozti.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3pcnfzgbh.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3cbtjmsbc.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3zmynjpph.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3ywxshnzr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3zaialzqt.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ljnxqqzb.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3jaisiqce.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3bsqmqmkz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3qhrlgytc.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3objqvuzm.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3azgovsgv.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3akyvpzap.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3cofdcbbr.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3zddzigpf.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3oujrugig.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3szmdsowo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3tkgmstov.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3uordzsoi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3cdrnjwre.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3rjuubtqa.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3zsjemsxg.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3uyjdajrq.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3esqbrfdf.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3tvhlorgj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufbjfmtf.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3umrpngqi.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3xtamvrlw.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3wzqlquul.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3wwtofzuu.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3kttmzqfq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3mzedkouh.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3mnlopxte.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3zzwsvfai.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3kvkrqaog.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lxuijazg.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3kygllwxd.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3rvwtphfk.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3deqiduji.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3zamyzjfi.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3yarckzrg.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3ekqqzclh.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3eytogztn.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3faqdvtie.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vzjehawo.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3rwxlfutj.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3obgfrhcr.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3paqsvesa.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3oorurmnr.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3wpkmaxmy.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3yhuppkln.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hhxbwaem.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3vaiijsxc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3maoslysc.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3onzqqeam.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3rqcjhlqa.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3zlorgxks.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3dnbzggdx.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3nuatkwwp.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3ggooetei.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3aehdzuje.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3hywccqkj.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3wyaywhtg.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3ukefzuez.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3fnfxdngq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lbvontri.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3eecqskhr.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kdohoefu.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3rfljwclk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3jnpomyrp.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3nowgshbq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3lyquwtxq.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3nubvzcch.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3mszfdmvn.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3jbfpjsdj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3atjoulkt.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3veknnjsl.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3vlytoljz.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3gglgjust.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3colawtul.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3xpqpbzoo.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3eohpzsmm.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hnwledal.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3nnepgxko.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3tpnqmazb.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3lpxcuywd.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3zuopvrne.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3mbzkqsqw.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3pdznrazy.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3cjsjexga.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3xujxdgxl.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3tcsekoht.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3vyndcejs.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3neqrnxdd.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3oztzofdn.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3hmnytvle.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3iweiomdj.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3gpaygqxz.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3cugdqygo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3vsixfrvr.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3gijbtkrf.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3mvmoubnz.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3cbjgizgp.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3jlnmqnpo.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3xpxdqmmy.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3medqeyej.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3mgxcpxli.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3gxdwujfj.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3hgxpbpna.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3otlqqgho.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3zhhodbie.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3ahomimjn.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3fasspfxi.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ynthzsvt.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3ctyuuxzk.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3omvrauyp.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pgodvcld.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3egfbhrmh.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3jhnmpfyn.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ijohssgm.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ezxwlwkp.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3qcldcyll.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3cmikhtcn.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3juipdrlo.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3unsyzfhr.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3dvagmbde.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3frrphmwt.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3lfewbkjn.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3okvuqhid.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3oacfmrot.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3njxhazbh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3bluyumor.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3fuvzpmdm.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3tbyemwxb.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3pvujerpa.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3lfxjyalm.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3hchzhned.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3yijxcaip.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3lexwevxo.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3eudtpugg.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3umblylpg.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3ntwyemzx.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3ydrbeluq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3zjehgqov.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3agvxuhvg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3soxqgzwj.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3stomazob.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3gbctwfos.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3repqqaop.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3amqigihx.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3utpcgtbe.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3ejqffxzs.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3djhmxqlz.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3rophesjt.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3hzrxzrqh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3zhqqxqqk.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3wkgfsavx.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3nhtkgyel.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3kcgqnstp.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3urtvqfgn.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3ycqecqtl.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lkvaimij.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3mqzrubpr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3neziryxd.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3bwrgqetn.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3kxmunraa.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3eifgfzve.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3euqvdjgk.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3gluoszrg.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3wmojjkbd.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3jrlgmeto.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3ppjoihil.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3rrglasuj.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3gzjycxle.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3ekkkzbef.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3llcunffw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3srpsgjmj.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3zzcvyjqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wbarntxp.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3mibieein.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3fatxvkca.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3fcgcktru.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3rxslvmki.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3hbaalmft.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3fgjtglxp.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3rljrtzuz.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ukggukqg.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3rxavvwwm.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3wtqflcly.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3wocbstqh.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3icomxplu.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3xjxdeirh.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3malugyve.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3chthistb.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3dsxhgpml.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3pbjesvwk.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3oidbmpbh.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3acjuhusp.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3xrpzgocp.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3dlilzpay.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ttrovtia.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ovfognyj.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ypbqezop.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3kjdwgzif.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3emwlmetn.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3daspxulo.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3viytcsgv.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3cfedxjgu.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3pasmjfec.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3dwfrjunj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3kbsgnhwa.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jecoynjq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zucdxuoi.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3gwqdmkvk.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3fnjftzve.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rjbtdbva.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3jtxlgtmi.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3raakrldn.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3wsasfxbs.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3wsfpovfk.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3ebuuayrk.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3yhsvwgpe.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3fjylkxjk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3odqkiytf.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3rywtxxdv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3fhkbuony.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3qtrwsrtj.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3jmeiiwce.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3hfntfpoy.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3ahoigvlh.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3wsjbtpxr.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3sdweyzjq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iulqjbbv.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3ozwduywh.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3bbsqobfo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ulltiddw.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3mrrueale.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3ulyiuoly.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3rezlybph.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3zijogcid.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3ffgfbxjh.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3jvpefnht.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3zekvgruy.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3dsvyqnaq.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3xpjjbock.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3pggcmctf.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3uksfmxop.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3scwgrepe.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3lyyhoctl.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3syvsxuvl.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3gkmufvcd.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3mntqqdoc.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3issojvez.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3grmzjwbr.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3wyrwxckl.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3ddzcenxr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3rdubutlh.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3paqohqfs.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3tpzxgnpk.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3doxleqca.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3eylscnrc.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3iemycnqi.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3qggtapmo.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wnfdrdee.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3mhbqakbr.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ldqamlhn.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3iweqisvm.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kurbofsr.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3rctwsdgf.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3wvmrtgoo.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xmwadyvb.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3aeaowoum.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3wojcnvzt.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3mntvujrm.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rmkclykl.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3drqiczzh.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3xhwrhtfb.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zsljqsai.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3tkkmrqxl.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3eysyodil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mmhksvkl.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3wymzypvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3egomuzst.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3bspxugcj.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3ykcipjif.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3apibsqcb.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3vttmudrq.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3iijmmmgs.html


<!-- 参考信息 -->