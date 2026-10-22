代发 wailian999

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2sjciifgs.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2ujwmxaib.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ygpcjjgy.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kvjzjleg.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2fmohhitd.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2enclmuiu.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2uupsexsd.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2hrdvusap.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2svkptlxm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2mlublklc.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2yjsxynsf.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2luqiunhy.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2ainljgtf.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2gcmvxipf.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2fcrbmmfw.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2ycchiiil.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2sgawipqi.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2tuuinhfu.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2ktuofzpz.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2odblghtf.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2trbrcawg.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2iymxjqot.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2oulokxnf.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2wybjcuwv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2pzvgmlfc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2vhtqszsz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2nslkjjpj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2lygmvjge.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2xsfroenl.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2bcgzedsy.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2zpifuydw.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2gylfozgj.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2hxaysjks.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2iolhogro.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2nnksqenx.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2sawznwzr.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2ajxchulr.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2muephjex.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2uykyvxpx.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mvlwumjg.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2djfxaxvd.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2dydqbbtv.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2twvqjzys.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2kqlaotxf.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2zoxeryop.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ksqajili.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2gugaqxvg.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2rlfxjymb.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2vcsugqnq.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2hyocuksp.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2bbhvvllc.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2kmqrbvsf.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2juhrntdh.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2atfiluad.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2dhpqgndo.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mgukalge.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qnzkwsuj.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2uwkaejss.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2zgplahhk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bredmpwc.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2coyomtia.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qfitmiyu.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2fqbevocn.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2pwheydbe.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2nlvsnuoy.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2fpizvtex.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2cywlhfci.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2yfetyljv.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2lmddlrxz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2orzjbdis.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2tcvbxqlk.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2oxdbqxgv.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2fzfiygog.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2fgkbowzl.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2xzjmtucx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2aozelxao.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2bltukmdx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2smgdywjb.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2suricrrz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2emctbwei.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2qkcdcqsp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2cjzdxkrc.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2hipobgwm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2wqgubgfn.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2pmldoagv.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2wdkbzfxr.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2drmfxsnm.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2ouqvgevj.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2opopiowr.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2cardoshz.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2eedezenm.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2gwbnwfyn.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2pkguyjnc.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2iygadqnq.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2xmzdcpsv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2xwdhgokq.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2qqutwxes.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2wdnvumnl.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2rnnahcse.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2zyiysstt.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2fgngkriy.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2pkpdbvew.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2guwfjsqw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2lbudrgmo.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2izzcuuhs.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2xzysxhkh.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2lkavoihs.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2iaukginc.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2pzwhhnki.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2opookrbz.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2kedixwsb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2thhphrvy.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2nunlinzh.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2stesokzp.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2eejjwmva.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2yltubrgd.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2dzbdkata.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2ndxatoqt.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2fkjeuuuf.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2lakliwjm.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2cmehpdka.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2kcuojrax.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2bwisbxre.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2rohexwsf.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cjfaffje.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2cvhjtexb.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2upfelijz.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jockopnv.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mxlxhuqb.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2scymlfxo.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2beyubhhb.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2fxqtgrxj.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2naavojpf.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2aotuojyj.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2fsmkdhbg.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2msirtosu.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2zbgffgpl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2tsluvwcl.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ltdgsyhv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2kymdybir.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2mjxvwtnb.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2flbbrpch.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2fehnhqmp.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2wqcnersa.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2rnfahtvp.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2wxclyxcn.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2ubnqcbwl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2jhicrbtk.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2evnakcnx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2ofkptenl.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2xrebtpfa.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2gmjxfcmv.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2kvpxrdne.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2katytkld.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2uqkszfmh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2viwlgojt.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2fevtjmzq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ffcmzzod.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2qvsuhdbu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2fqyjuvef.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2hfcubozv.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2adfomujt.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2rjxhuoiu.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2xwcivrwz.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2mubbazbz.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2otgqmtyp.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2mmlpommv.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2lfebbefp.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2jkwxmytq.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dqkcajqj.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2sazkfllc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ingwzhgp.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2mcxjcnmx.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2exkqcpfx.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2xfjpbwff.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2shkquvaf.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2nbcnzjyx.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2acpzxywp.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2dxqptljb.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2liykopic.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2bskrhsah.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2inniracm.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2wdggkzjc.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2oczmiurg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xpfhpdzh.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2ojpzjqwr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rblfatir.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2cmskqhoh.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2naasyflk.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2xiiiemen.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2zjmfbpws.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2zhrjsfxi.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2izilrxtc.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2aobpalsm.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2zxigdwch.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2rgmbjzov.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2jddyodmm.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2jhqufmjy.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2jrbjlloy.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2mippqwxj.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2hrwcusot.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2xxglqvye.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2ghtanczl.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2ujxrbiwb.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2gbmtkajf.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wohmvbfc.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2fkdssucl.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2aorshewf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2adqlrcde.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ogzvnpzt.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2jahvbiye.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2elnnzbod.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2tlwadoit.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2qspexlzd.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2rzfdvjqb.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2effxewlw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2cycqyszp.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2cpeeomti.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kdgehdsp.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2iietllhn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ruufzqhv.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2rkxdnhsd.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2qcfbprsk.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2uvkdkxmm.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2jklswfwr.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2ebenxpvn.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2agnaikbt.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2cgynavrq.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2zdesuikv.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ykxlkmvc.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2jypyaucr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ipfjdwtm.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2olekvfki.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qsnmmxxg.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2aeufkidc.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2ujkptkxd.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2ziwmqeyt.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2cdpzhqic.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2ptncpoyq.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2sdlcoudu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hdrznqgm.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2ahtksodv.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2hfslgpyo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2phimyodq.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2wjbvqsez.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2qyrwlwvu.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2fjhrpsbb.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2sjtbfrij.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2uqbtyhyq.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2ntulrekw.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2rnptqugs.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2jikzmbrl.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2dxydbqzy.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2wgoijlvv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2ldnkoubf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2fmuodqhr.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2iximlccg.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2pbkpiuhq.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2gkulrjuu.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2xyrxsmjk.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2lfehesgf.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2abbcbchn.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2iscwpdmg.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2zudemynv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2eftlvrek.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2zaknowbt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2bvrgjuap.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zolqnkwf.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hbypiume.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sriahuio.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2acamzjxl.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2vglpewce.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2zflepjtj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2jctcilbp.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2odavcytc.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2easndlbs.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2njnvpiui.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2xoqqazst.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2saxxffqw.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ncxokpfq.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fikayagq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rypmqelr.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ygbdgldt.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2vpqnidhc.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2kpkyjblp.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2shfxnevd.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2voyamzco.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2ekpkdbil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aqfmdveg.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2vqmqhnfu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zubzfjzp.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2esdawagl.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2ychadkoi.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2yhaboibe.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2jaxkbnwa.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2apydluvw.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ryhopwqo.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2qnwfuyxt.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2qaxburih.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2xqrfhmje.html


<!-- 参考信息 -->