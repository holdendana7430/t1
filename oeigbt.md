代发 wailian999

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2nnoobrpw.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2mcbxbdgo.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2eatusekd.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2liuvefgi.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2cvabfatn.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2qlnmgnmx.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2msibojbb.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2ztrmmsjk.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2genngaxi.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2bhrmpybl.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2ydowpeqb.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2qwmvblak.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2hdzqpzkl.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2lkqlkytp.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ocmvtnqu.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2xcgapoiw.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2jccheowo.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2jbqhmxbo.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2nyougvoc.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2ertxaujq.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2qltmxnit.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2ougqckbh.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2cvttcgnn.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ksmojigt.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2cpxevoig.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2eewgqxpj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2lclgdvcq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2buyjdlbb.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2irutalma.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2rkjllsaf.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2iirhqwtr.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2ppoxkaay.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2giicaqzj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hiqopiyn.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2cuiauvrz.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2calljkxg.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2fzotdrxh.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2gmsrdgbb.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gkulrokt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rlkxnhty.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2penarhfa.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2optkqqll.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2aehhonrl.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2lxombhjt.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2ljxclzcp.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2mfowypct.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2hsllkwrw.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2hssltrox.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2elrnahbm.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2rmqcqcit.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2xveozbrr.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2sjnvfwar.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qlrivxrk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2fljfhpgz.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2bvqevqus.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rgwcpqya.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2tjughmqb.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2qaqevuzd.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2zetanjyl.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hgofkcjl.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2auudlgvo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2eaigopeq.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2mpxxcyfl.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vejgvpyx.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2fwoypxmu.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2rssjssyy.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2fmpvrptk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2txcticzl.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2gkabtxih.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2hywengru.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2uexztxnf.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2pnpvsfno.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2hhnygxtq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qmasgeep.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2omguqxkn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vdozukxq.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2aunlczvb.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2glkjcwkh.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2rvewhawg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2vlbjrfmg.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2ggxpunvz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2zupxrbdk.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2ulbiyjga.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2rscmymks.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ukmilany.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2kpgnepit.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2hlvaloes.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2gqnfwiit.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2vpfzyyou.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2afdlwpuo.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2yeuurikb.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2ojfvxzcr.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2jinifzte.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2mmehuamn.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2ravogrmp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2dfdfmzqf.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2riqgcgrl.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2arupnbcv.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2hwrqiyog.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2kggupsjb.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2qxmqyzzr.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2mniorqvx.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2eojmrzxn.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2lbcrevsu.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2uofuuxjx.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2jmchlrzv.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2wvhpjqii.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2kmfklmgt.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2dixbdwjp.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2xastbdoh.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2nfsoaqsu.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2sqkhyjey.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2lqafgdjk.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2uthhescf.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2gyasthdd.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2bedhmqli.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2kckbubtt.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2xustihxd.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2lhysytxk.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2djtzjasw.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2qceeutyr.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2sqitclqk.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2cfkpzamb.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2lgzyeddw.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2dlnwvbfw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2yvysetbe.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2wnmkhotf.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2wvsdbrbo.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2otttvfvq.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2dbnfvhpy.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2uvydvspm.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2juhenogx.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2cohvpzwp.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2rxeyquip.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2xtedgnib.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2lnjytddr.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2lasjgmso.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ndedwidg.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2nnyyklpv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2rkyprqzh.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2whltgrsn.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2hkpgldve.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2ngvwbgbm.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2mtociajq.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2wihdftsu.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2osjohrmi.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2shezsytc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2jjovpgfw.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2vgnmggmb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2jcqydfik.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2bcheoaad.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2pcssxcge.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2nmzsgyfm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2wjajrxdb.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2cxqhidev.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2tnwhuoqa.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2uapcngyg.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2wvnhnpqi.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2jzngjxem.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2xzgvymic.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2aalgxkzf.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2mgrhomox.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2iekuqjmi.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2mgtvbpvi.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ojdhpyxz.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2lopadiqa.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2pusyvkjy.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ifsuzmbu.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2borkspeq.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kwycakky.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2ybdhjfhs.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2wlxizckr.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2jldtdjlv.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2lbeypdwi.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2kgekuvzq.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2zumexlwl.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2vrppngxv.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2fkjqfnso.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2ciszjubi.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2aetmmbmh.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2anqbsjlc.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2tvyupbtp.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2mbehexbc.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2ickoeqln.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2laojflfu.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2uttwwxxm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mafvvgmw.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2xqxqorxw.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2vsbrkhdz.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2kdzurdhh.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2yerosbdh.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2noljntgy.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2esmrzoxs.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2vlvkmngs.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2zhkvthlz.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2vdkzfdnc.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2vrzlsact.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2wnztgxha.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2mvtdnqlg.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2hnxlzmmb.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ktttbbvh.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2ouukrfwu.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2ijuncogw.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2daahxrok.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2pyecsltf.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ytruvxwm.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2jgqqyylq.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2slhnfqtr.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2oqefaozz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2czrqvcre.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2hedznbwr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2zxzrowfc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2qikghtrb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2pktxntvt.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2yynhzgzs.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2lkwdtrmv.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2nvhqmcnp.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2xboiolox.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2fctnygtz.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xclmpouw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2dvnuicyq.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2cbwdgalg.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2qzpyburg.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2lifmdjze.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2gfgtkgca.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2fqksurqc.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2gmmmbcjl.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2rahmggbk.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2xeygksdh.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ggjnriso.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2lxzkwlps.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ojsfuslw.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2qephysen.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2cuouqmya.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2idjwfrzv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2lrgfrevk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2ndgneiay.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2ecpihbev.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2euscnwma.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2fnzxmqtq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2udelumam.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2pmwpkxya.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2aitdxgkm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kkgpelfb.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2kpuwvwxj.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2wnjjnbma.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2iifzrigk.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2fvxylqon.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2woriptmi.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2upewpltu.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2uqktwfru.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2ygwdwplw.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2cayrrjto.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2stejsarj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2elerpabm.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2erpfxprm.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2fpzqfhhg.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2qmgckhme.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2yrbofxgb.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2aaofnfnb.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2gyypuvph.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2lozrjail.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2nnbprpuc.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2igvrxxfv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2usyeqrme.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2xqycznik.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2kcqmfsmr.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bzuwltht.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2efsfpznk.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dfsbmgxc.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lmjwbyjz.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zyujgypp.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ruqmxteq.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2xdasurrr.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2cgvqeteo.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2okputlrq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2tycbwmxr.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2niudmpmi.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lvhylssy.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2xeikahsd.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2hzdbaqan.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vliirwae.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2rilfzaua.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2rhpifhaq.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2htsgotbl.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tswykgbb.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2qmugiexn.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2ljuurixt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sbyiqtlo.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2pycumiai.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sttbbuwd.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2lrqyzjgp.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2lsvwirnr.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2rnesqaco.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2effojokg.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2wvrnezpp.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2qfsyvvrb.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2axuiwlhm.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2tnpykmwo.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2dwelzgyo.html


<!-- 参考信息 -->