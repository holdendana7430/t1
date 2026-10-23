代发 wailian999

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3ixcjohih.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3xdkaxwfs.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3hzabotbg.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3axrpsuuv.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3tafljcvq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3oicsqclx.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3rsvkpypg.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3umjeugsl.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3vuuvqife.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3rdlmckza.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3tnhpnakl.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3ngmwktxe.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3zemoivgx.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3rsapgsfe.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3usbznnog.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3qjklsluf.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3imiljqsu.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3xootxxbe.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3rxyjrnhr.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3dfhclgxn.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3tfmdarot.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3tdzkiord.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3rymyvflq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3aahkfpvx.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3xtleeqgu.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3zrgnwmfl.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3mwcmxsbx.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3edfiheoz.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3scvajgzi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukfjhupm.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3kmrurcjh.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3fmpsmpyh.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3dejltwvb.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3vwkhewdr.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hvxybfxh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwhrxxtx.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3ghcjocmb.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3cphwqhjr.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3zfxyakgo.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xcfxtyrn.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3zekyvdki.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3xqerqxhn.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3cshrtgft.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3nhdzsknc.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3wheihllp.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3uokyaplg.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3xyhfsbgf.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3koabgtyi.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3ababqrnt.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ulxorpza.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3uylgppgi.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vjwvghrr.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ybgtfukz.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3lumdhgth.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3bpmngiby.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3dqzdkmng.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3ohftiizp.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3bnrgdniq.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3wvlsrwmx.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xxgagbpb.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3aqwcskei.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vdofovxi.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3vbtselvn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3ccxnewne.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3dhcqoetw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3itfgvgez.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ehdmhefo.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3dqliimvh.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3umgohmca.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kgxoihcd.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3ztmhvzpl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3vhykcswh.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3eflsbsxd.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3mhjizeev.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3uheenesq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3mjqfimoc.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3kseyaztr.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3oqsicgrz.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3xynlosoe.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3hdiaopym.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3uzlsvjqz.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3stzivhrg.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3zplakezx.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3wrgwtpnj.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3wjkixeje.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3jyryfjvv.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3bebsjmcv.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3fdesdirq.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3kceyebpz.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3rvrrhtoz.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3uabwoxhm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3vbutljfm.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3wgdynegj.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3cadlfyza.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3rtobpodw.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3bagunwmd.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3fskomchy.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3vcawoysm.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3odtnohyl.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3dbvnccyl.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3rovwaoor.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3hlemkjex.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3yfkidlqu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3orwizevu.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3cbqxnmqy.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3othlzcqc.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3foqvlrtq.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3fztfjfwu.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3hkzhlgbh.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3wgbmvonf.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3fypdkjxb.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3ozjcxcvp.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3zgmjreaj.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3laylvebm.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3nqytdttl.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3wgjphkvu.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3ayrtiukm.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3rjhqygzq.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3qqhavyyq.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3fiknsoto.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3jknoqgqy.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3rxsdyhop.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3zbpiibzt.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3hcmjqdza.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wdzshmsy.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3ugzegcmo.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3etfvwicg.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3nsjoagcz.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3xjmjetfj.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3paukesvt.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3lgyanymk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3funymroe.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3pfkbdfap.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3pkzkwebw.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3avivyktk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3vbdegmmh.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3lmpjctrx.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3bqqzaipf.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3auiqajep.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3gsrrrkoa.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3styorexn.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3cfolwbhi.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3piunwvys.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3zqskytdw.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3xrgyrrit.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3pqxhecch.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3gcououja.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3skspfkpc.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3slpeyybz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jyptjiyi.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3audyagdg.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3vmhljvth.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3iqwefwbl.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3maqwssde.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3tnjlyiqs.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3ndfrjwrr.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3asvreixa.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3iiagtriq.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3nfryoahy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3booertdp.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3dtnhvred.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3lpzbjfgy.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3igkmrefh.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vynqiytg.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3yvoizovc.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ehmozugl.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3ccyvqzdj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3wyjxwejx.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3cxuqodoo.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3vykkwjdg.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3keyozjrv.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3otuywrzw.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3dxwofuue.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3dxuxalbt.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3vbpwokoo.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3hckiactg.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3uffhihyb.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3dbhdfteb.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3sgxrujxe.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3ncykwhiv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3axpycjgx.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3aphcyqxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ontctkix.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3ffgqoogm.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3qmhnnbiy.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3rlosnwcb.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3jacjawxv.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3nxnasdbb.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3fmsbuchk.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ialaioio.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3hlsbmuny.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3jnbbzppz.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3ijvhpemd.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3anwockoy.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3qeyqmozk.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3dtkkllty.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3snvrxgya.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3nlhfltmc.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3npecqkne.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3rsgqturu.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3motzhrnq.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3cfmmvhkk.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ggrayxhx.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3lieofnxo.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ugpfvghi.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3bddubtpr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3mnrbabyi.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3lkoroiaj.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3dyvnsecj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3hxklqvtc.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3bhclwzel.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3fqhnleqd.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3djenpuww.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3ahpecwyg.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3yxqkhaus.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3quvatvmu.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3frdqxohp.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3blmwelyi.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3abiursob.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3sslyebzy.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3trkknllo.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3xrrzsgch.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3bytmnqun.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3fcgvwjds.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3bezdqjcs.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3lesfnnzs.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3knmfzxym.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3iklftkyt.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3pcklunfv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3aacdwgqy.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3nvnrczbx.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3diodepym.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3coocfkyj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3plmnqwas.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3thfwmsxq.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3zzzwuggc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3flcuwlwy.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3svxxigty.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3waghdrpk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zmpvhwbe.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3xaxcaltk.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3geapgtxm.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3lqoccoos.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3btmzlwfu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3dinqojpq.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3qochhelh.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3qfozzgwy.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3sbldrbku.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3tovmcksv.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3clgyvxtt.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3xgdvigbs.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3xesfxahr.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3ajylzdfx.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3rypyuwbl.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3sinqonoc.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3gwwkogvy.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3uxxeufla.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3hqfjucid.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3imzznssx.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3ykluavlt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3soskpgce.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3ktnsuzhl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3egyusiep.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3icekhlep.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3psevkhdc.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lajbcxys.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3ktwdmgwy.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ijvnxeul.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3krokkorm.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vcfhhbls.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3eedrvbwv.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3lwfxsmwe.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3mpqemhfd.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3kuatrmxv.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ztgktzcb.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3temuqtdw.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3hhtxjwbo.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3rjurvucq.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dmmqycnq.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3pwotgttg.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vahprovv.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yfnawtcb.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3mazuqgyf.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lxetfaev.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nfqxynes.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3tcnvvfjt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qfxmppyf.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3mnhwpapu.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3hqcmjicy.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3csissdob.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3reakuarr.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3idcgrsnt.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3yvmigjvp.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3sdbvchrv.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3lsnygsxg.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ucfeepuw.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3slmtsdtz.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3tyhonrai.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3mrwwfsoa.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3aryyzpco.html


<!-- 参考信息 -->