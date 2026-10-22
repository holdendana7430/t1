代发 wailian999

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2nigvnbus.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2rwjxfbti.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2iohnnyds.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2pbubhusx.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2ilrqitcd.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2qwkjcwtf.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2xsavepzw.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qaecurix.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2mecfbvch.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2udrnxcng.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2lkinsnzc.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2tpcifcek.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2cevebvrl.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2gqolsfve.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2bydfbhan.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2lucsmrsu.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2huwssquj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2hxysgphc.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2gxiyyrye.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2ajjklxpt.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2vahamupw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2fsbvtaej.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2bldoaxao.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2obkkyvms.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2lgvkwbps.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2iqgphgmh.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2uuokrtgt.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2uwxvlnyr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2sfxoqljy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2ztqtdzbu.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2brsrypii.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2minzxwcj.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2kbrjtdcs.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2xuhxalno.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2lzbmfhdh.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2iashmsbm.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2svcdilgn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vubsherb.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2omoapamo.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2rmokckpm.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2tqgqvbom.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2bsjescyg.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2assbxonk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2bzfgylmr.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2pjubqqsf.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2ubywxlvm.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2bvtpohpc.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mbwbnyas.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2szfnrkxz.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2zklxmfdb.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2sivjiekw.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ikorrvhl.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2pwqzdzuc.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2puoiwzia.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2wmnlclth.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2mzkogtjs.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2fcjxtmnz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2admueeyu.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2toidaqzr.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2cwecqhen.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2gnamfomx.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2bmszcfkd.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2vkpkhzil.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2rduwqszw.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2aoaaritd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ynjsvhxt.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2estmskgj.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2npccyqzq.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2surkyxjt.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uliyiidm.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2hzcwvtsl.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2diqvihlj.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2uohbohpc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2oowhyonl.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2iauaiqrp.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2adatapru.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2tkzvmvdq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ythasdtv.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2rbacdfma.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2flgrxngw.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2buxizvxx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2hrsewfci.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2gsftzinx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2kvuhnjdf.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2ibljehhz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2yuwvvgan.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2zjtqtuqq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2rmohoiyk.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2sujcbvrm.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2jcoiqcoj.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2nyqbuvsq.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2kabagjrw.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2sojmrywt.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2zwcolgdf.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2sjqrafle.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2neiqefsi.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2mofhhpfj.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2oozrwovw.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2cvohwfzj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2zedklydo.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2ptrwsquc.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2nnkwpndb.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2cnbkvfin.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2kjiaxyio.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2zwqvjqjf.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2befpqwjm.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2vldyxktv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2gvdyqekw.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2mfrmstko.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2pxpkawyd.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2haloktii.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2micwiupd.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2prtqrknx.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2lprhratj.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2mjmpetdd.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2hgqrygnb.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2xzyvdmps.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2pyiqzcco.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2kdxkowsw.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2epogxcfp.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2vvsckxmp.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2aervrxgt.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2trgmkwkf.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2qjezwdtl.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2txjzfhxl.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2niyodaxu.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2gipgnimg.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2aludykoi.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2opjhzluo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2bofgxrpc.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ntbtrybb.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2qcrrmotf.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2allubbho.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2lozoblkp.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2gongrfsz.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2rdyoedtb.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2frgnbacq.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2fxrdsnal.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2xkmseynl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2oxeoakwe.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2jditkypy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2bhyqnncq.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2btsrgmfz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2zxumybfn.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2xovsqgzf.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2jmuqnudr.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2fjeymvjo.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2ttjzrjqe.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2mibrosrj.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2cxrwcfvj.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2pfsjelly.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2plslxmeh.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2zrnfpied.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2xhuykjoy.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2gqrdyfdz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2pttxccfh.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2zuioebfc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ouvanlqc.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wspiikfe.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2ycdbsvqu.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2tplhcwlv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2agcxpill.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2lgzradfu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2bspllupq.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2bedhuzkt.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2nthiofrn.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2eqkhenrj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2skonnldk.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2eapahemf.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2gauijete.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2lctnuiga.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2otxcxbcq.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2xzaexfti.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cldccioc.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2kgrclqnc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2awhvkxpy.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2xlqcxdky.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2udgjbqxq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2xytvkjot.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2zgtjtyhs.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2suuedvnb.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2pckqqhqe.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2iqogamjb.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2lwfbdnja.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2mxjtaxki.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2rvuixfhu.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2zbciyuti.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2wzfcrwdz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iopbycca.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2yqwerrez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2szrsvkmg.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2uofwujsi.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2pooawpfe.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2pgfrjork.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2kkswromp.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2lvmfjjxb.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2mkfhlryr.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2vymfqvxi.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2tylxbnxv.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2tytumpqe.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2mvapghfn.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2typdzirk.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2nhsorzsf.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2bzkgvmjb.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2wyczvnff.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2bygsfcms.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2vaegffly.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2nhljvmkv.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2zgssdkrk.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2nmbxhwob.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2dfrcwyqi.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2sjqrskiy.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2mhbhzgcf.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2qheigpox.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2simpjmye.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2nxpxbcgi.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2beyrorvv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2yeuuupzs.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2fbwzbduk.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2ufuopcxv.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2zaecmbhc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2yohygppa.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rwrmndwf.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2mneorvmd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2yalcrtzl.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2gsekgtyl.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2bzkqzvyq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2jsdcikno.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2opioovtt.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2vqxoxmzf.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2seadwinu.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2yuybbmlt.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2cdtyclar.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ahwuwkms.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2kliledvg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qklxcvyc.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2aqsszbce.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2yazdcbmr.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2uxllexeq.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2krlzsjzp.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2cznhntea.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2xbitqpsi.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2lvpttpkd.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2btpvhllt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vwerkuon.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2lnrfrkyo.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2dypqbcjo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lvjvrfes.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2pkmrloth.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2ukzyvzok.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2hnzxjvij.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2jmdtekjm.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2rurhnhgj.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2vaqqnqad.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2tzbponjb.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2dxpegdzk.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2fuvzcgbi.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2qbriesjr.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2xniylbwh.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2yrdfimtb.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2trdtysii.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2ohgepueh.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2qzeuknaj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2yifgcivg.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2xajeiszi.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2olrszkyv.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2mtaremky.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2tgcicifu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2laeicoyt.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2jdsztnmi.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ottmtwun.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nimjbrjc.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2wsrzuqja.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dgqsxjrw.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jnkenphs.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2untnqaxv.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2htcfkbbp.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wakdulyj.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2exnvgedb.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2wpbnzsys.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2yfbztfxs.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mjjlbktx.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2stiqyihy.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2corktihs.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2szgnxlfp.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2dglpumqk.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2kuyoaznh.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hmviggoh.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2vqjolxgb.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2kgrkkiiq.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2khcyesbg.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gwoefuex.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2przjgdoc.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2ikkvyaey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xbcyotig.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2xnycvczi.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2dxycfhdv.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2yokgehrl.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2szcykjuu.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2ppdtdnhp.html


<!-- 参考信息 -->