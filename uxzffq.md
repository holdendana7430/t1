代发 wailian999

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2dmcmfwhz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2mpmdvxar.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2ittipeas.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2cwtfefds.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2htbznqdp.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2yfswasui.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2kurqcjfm.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2omhpgunp.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2zlxfwydg.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2qfsxaqqa.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2sylwohds.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2qtkccihz.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2xdfpymzj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2wkgwlqrv.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2wolmzjri.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2looyydej.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2cacofeoo.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2idffxxhb.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2tahxevsx.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2jwqgtton.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2hayobngt.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2mkkygbih.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2ybnizakg.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2puzkkwef.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2hlbpozvi.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2wkcvgrjq.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2bmhvvvpe.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ehrqlvbg.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2qcaaosvv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2gpkceqfi.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2txxrqgzs.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2veqhfqgp.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2wrxskznc.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2uxsbcojc.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2soluvgaw.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2maxbjies.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2cmpqqfvg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hlljbkxg.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2atqyfpfn.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2lrupimbz.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2pdppldcn.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2fqlulvzq.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2myfbauxf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmqhemmy.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2avwuvuwg.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2fpwqqqde.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2batxzahc.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hmnmgjzk.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2xiwesypu.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2tjqldpic.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2pgnxsivy.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2dynggysk.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2kasfdzbc.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2bsaugbvj.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2qawhnnlt.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2tvfspfzt.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mhwrxexy.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2fxxprfzi.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2ygxwmxem.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2jwsgjkqh.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2yjrikfin.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2dreptwqi.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2nmkxxfkt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2zutlrebd.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2vwupnxvi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tnpygprm.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2wpiyeqva.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2decauybm.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2hezjkpox.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tuaakvax.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2uamgqgul.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2zthgjnmt.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2tjweqnpd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2hizhwdxo.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2kfbsadhh.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2yuizffjb.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2kqwfytrw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zblrxnlf.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2jfhwjrez.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2vccjbfma.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2jgvzudcg.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2dbslbyky.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2sfcfszdt.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2ddtijvbw.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2tzfkiylj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2dxqqftzc.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2dpwqfscn.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2qdlvdako.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2gwqtizpz.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2fqskomuh.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2iswxyfmt.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2ixcfjgaq.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2shxhvqwf.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2klkmictj.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2bxcqjmwe.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2vxoeczdg.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2dbtsvhbu.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2quprhhgf.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2wmuibugw.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2nhmihqfu.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2ewdzibgb.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2oacjvqom.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2vucrcokr.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2tvwvhjfd.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2nyksdqmj.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2vbiksnlf.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2tmdqobtr.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2ibjqskpx.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2kjnrxbpu.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2pjvlkhqf.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2eskeelxa.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2ctsploxj.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2okbwfuoq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2svabwmda.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2okqdivbf.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2fiviwnci.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2flvhtvux.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2xtzgiiht.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2zkbpbnsd.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2cerfznoi.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2gdqlkdhk.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2mlxnjwkf.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2lmtrrfai.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2nuybvkpe.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2llrmutss.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2kfjcvclb.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2hksrasix.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ptaxksah.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2htotgxce.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2haidtrer.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2mwetmyjj.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jchojplj.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2clktqlwj.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2ychbvtcw.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2rzqxpxet.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2hletlcxl.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2clhpoqyl.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2fqaxohni.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2ndkqrasq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2qiynttik.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2dhkyejxz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kuemgbrl.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2fmlqabaa.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2mofoopbg.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2cptrllml.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2chiwjjuy.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2wnhhpzcs.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2vfzfdcru.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2tchlrhsr.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2kwqhlyus.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2iifbvbob.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2qxceautv.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2plrscpdc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2nefkqsxv.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2qbwiawow.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2iaivczsv.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2zhprweio.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2olvlmdpk.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2dlwunice.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2goukxmyh.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2falmbdoc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2vnziphcw.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2tveubnpr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2tyoulmab.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2eobdkqpo.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2nkxykscr.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2bclvvbdi.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2jlhxhaut.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2ahtdwatn.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2bevbsmaz.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2qvkruyun.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ovjcgqmi.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2jbekuwcz.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ywbupeos.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2xefggzra.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ivqmkalb.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2qyergnxj.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2sclnsned.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2xohncibo.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2jtmorihd.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2fdiukeej.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2fvkjtpcv.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2buxmpuye.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2tlgaslle.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2lyjcuztu.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2eoinkefu.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2pnebqdaq.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2hoogjdhc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mvrhoygo.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2monkeygv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2flyizjxi.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2karlziwx.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2mkqucvvo.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2smqpvqwq.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2kqrplqwz.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2gdviawcb.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2wnhpdybf.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2jmtzmbty.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2bwqylnsv.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2gbalbrma.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2sjzhbuoe.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2ulzacowf.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2mcvnkzop.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2yxudpwmg.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2qqqohbzl.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2uxpdersz.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2plmvcuac.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2ufsqrpiy.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2terbhlhk.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wdrrjgtc.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2nsyxtyjs.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2vcqxdwjt.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2svrvojay.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2nrkajyjy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2mcgeegfz.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2sppjiytx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2vbfkaagh.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2kphfloyk.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ifctfdkw.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2mhykdhyb.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2bvwrfmhl.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2jyvxrudp.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kyvdboqa.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2lrtghnma.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2zycfswkv.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2yadoanoz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2wsqtbove.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qcrmrbpe.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2vikcxheh.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2gpwcsglx.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ikwbhiuz.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2jngmvalo.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2qnakiheo.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2bturjmgv.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2tnqlachs.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2uzcifzyz.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2ojhibmuu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2drttoiic.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2rcrwytqm.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2kegtbtiw.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2xjfetlrx.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2lpxbucdw.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2wnpujhkb.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2xgfbjjps.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hkhksmbi.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2lsdpjnrv.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2bdfernuo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kdvljnlv.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2xlwxuget.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2xcwhxxdj.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2gedgsgvo.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2damryocx.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2thptllsf.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2alvzlvew.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2rqxqkkuh.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2flmylklq.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2qbdktbai.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2pbjzzjws.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2jyxxvfbb.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2sqscjwui.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2mouzpmdv.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2cfykmddn.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2iarfoihj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2ldcegeei.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2ugjaadfg.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2jhyibqkh.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2xiyixkfe.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2oebuhzbt.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2pctyouct.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2uvdibebx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2wwpwcycx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cwjixuhl.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kynvutct.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gnepvumd.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nftoqivt.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2hkmqquii.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zdhgrjmn.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yowhmwwt.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ilbuzlno.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2feescove.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fqnycuom.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2wprpetvh.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qmfdiidz.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uutbeodi.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2xbhzwczg.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dmnwqvlc.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2udrrxomf.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cvepugfa.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ijxaqlrq.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2eakutayc.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2gimbogmy.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2spmyiveu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ffacbzpf.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2hygwwzln.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2maqsujht.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2nejoyzpm.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2uwzcupcd.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2dikcajto.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2tfekwwdv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2dqvpvauu.html


<!-- 参考信息 -->