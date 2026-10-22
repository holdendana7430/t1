代发 wailian999

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2hheydjvp.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2pcnmymcc.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2yedxhjnh.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2emlgvzql.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2glgzvybj.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2jbiwpdrf.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2rcohbshq.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2tdfafkob.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2elsdgeqf.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2bmpoailf.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2rkznmkij.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2rdzbwfcf.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2wdhtqsnn.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2aejuuowo.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2hvhwdjun.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2gfgbmwmo.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2bpkkkuuw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2hjylrsuo.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2afkklrsc.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2wdeztent.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2zoxuppda.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2dvjdmmtf.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2dloaxnwz.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2pzntnner.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2xnikuvas.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2akwsjksx.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2yyvveoxo.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2zciebtak.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2womjbxiz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2ybhjhtgn.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2skkcyjhn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2qlanhkwn.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2dqohewps.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2uohunced.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2ergwjwhf.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2yctjklps.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2dncxfbut.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hvvcxjzo.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2nsykoxmd.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2tdqbmblr.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2mzlhhebt.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2euijgjrw.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2eefafiwr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxdjyqbw.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2ddbpwfvg.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2aiqbxkya.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2sdfwbcdl.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2qtdaeezs.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2wpnaruws.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2acixtenp.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ccklagev.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2bpcyzcok.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2thkaeuwb.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2uvkulpkh.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2vyrzbrdu.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2wxtgntdu.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2lqzyhgej.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ceumbmjd.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2kxppblrt.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pvwhtyjx.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mlvoxlyx.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2dwkizpxu.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2iqwjqmfl.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2xxlfxbsr.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2kqstdvsv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mtmqrsrf.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2acjuwkay.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2xqywifst.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2oyttyjwg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fizqzfuz.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2noxjkmpp.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2yottvxul.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2ooajmyke.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2xvhbvbjn.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2arqdlpdb.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2xtcxyixj.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2fyxettce.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wtisztan.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2xpktzyju.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2upqqiihx.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2eoqujiih.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2czlhrcjz.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2ofxbrjsg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2sxdamqcg.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2mmhbaqdk.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2kytedkao.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2xanffqlz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2pfexcrxw.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2jkconywc.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2unbntxdq.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2rpvuvsyw.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2boplacdd.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2vjvqugkn.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2awpvltho.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2rlcahmat.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2xkossqmp.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2kbjtyspt.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2dffybprh.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2ujazhxuf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2cbrnqdzh.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2npelnwss.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2wvevqbtc.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2dzdvcbnh.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2aeqepeul.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2kozrjywc.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2kqoaebfv.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2tcyowokx.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2gmpenfmk.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2tyzntycv.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2suznxjgt.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2hjuhjftq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2lwkkcxcq.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2ukutnupp.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2kalecqfy.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2urwtsbbe.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2slyrdlqk.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2aenqglmd.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2sjtevexb.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2bueqesug.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2aaovvppw.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2lmfpowwg.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2pburvtba.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2dhbgeccw.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2rhubeoff.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2dvanygtq.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2cwomyjhm.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2fwjatyic.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2zzlmzgra.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2gbueuxkg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2amggaymi.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2vnkkrvqt.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2erfjrpil.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jjkymosv.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2zfextcyy.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2irgdnrlk.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2mrfnhqyu.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2krajgwjv.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2eflsiuvo.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2noutsicg.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2uvxodbve.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2bewvaqqk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2euiiwxhg.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wlnuwkdo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2jlmcujge.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2mfqkkyim.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2ucvxhyro.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2zyiqvnzs.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2yfrrakix.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2qdpjatgm.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2tpklqloc.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2szljzgxp.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2truxxnty.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2cejzwqpx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2vpogcpzi.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2oiegjbps.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2rtfjrzdp.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2ylkivpaf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tjiojmsv.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2egnqjzlc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2amtyebtl.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2vmtqtiyo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2emwepywu.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2gkcevjxn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2tkxtvpqu.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2tpdzbgfa.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2owajhgaq.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2euuxvvlr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2zkfuoiax.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ssnzemun.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2tsiwswxu.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2etakgwls.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zndmvhpo.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2livtgjgf.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jnrslsix.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2npufaihy.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ejelebfv.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2gunsctgc.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2mffvgxzo.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2bcsingjy.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ohaybjhc.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ugerxqrq.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2jwusoudx.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2tqiwkbiv.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2vcnadtqy.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2hphnqzjc.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2oeugghga.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2zatrisec.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2ziqmpdgu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cqpopiju.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2vwcogaaz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2unhycwhi.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2jbhclahr.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2xiztezqi.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2qrnqabav.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2jskctemb.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2cadcruua.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2btruwpbj.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2gapvtuxh.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2xmjtaqyp.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2blflzdaq.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2boedgjia.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2qunjipnr.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2ejajllje.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2ghqzuujn.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2bsizhhye.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2yioimdjh.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2cujxlbab.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2ymvpxosu.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2yiowhtiu.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2pzjwejax.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2mtjyqreg.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2dlnyyjny.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2dzmxktgw.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2vhbmotne.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ivgsxgts.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2xnfqqyey.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2fwhcqgqp.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2cfaumpzv.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2hdxlnrqy.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2wqxvxyzt.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hmzwoqjn.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2cafopzxh.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xrzzcvba.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2jolbiwin.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2fgynwhqk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2tgjfpjdz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2lojhvssl.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2aovfhnpm.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2xlovjftz.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2ordndkir.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2mtxngvpz.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2zvhaiysn.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2bejilsaw.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2pydvffxm.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2cmshwotk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rakwohow.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2ggeolupl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2aatzevzp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2jimaclau.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2fjzrrxfr.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2lcuvqgvo.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2xlmwjbjb.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2xjowxnfp.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2hizrkunq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tutjwyjk.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2jgozaine.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2yksuonbo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qzuzloec.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2ticaalqw.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2dkyikvjj.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2sesmldzc.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2ikdulbly.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2fpotkmkk.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2sailbgav.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2mjjdkryv.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2ifzlewhm.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2zpoctojf.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2jdygqmnl.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2ekadnlii.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2iqdpslsx.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2usdsnxvv.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2vqaeklyh.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2twaqtqge.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2isdzwqeq.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2lbgxakvr.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2wityukor.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2vwzkyxcb.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2vjbenwhw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2snwnqtmh.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2pmlaolch.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2blawtnzz.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tvcjoqvo.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gnvzeabg.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2nguwtbit.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2xmmazmah.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fdjgfqfa.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2tkhlxtwj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2wxsrczlk.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qygcrwre.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ingypoyq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rhwpfdqf.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2glvimpwo.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2qftowptg.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uvuceirt.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2qhnwzerq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2liqlzzku.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wmewqirc.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2aezroopv.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nxxcfnoh.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gjtwzvaz.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2kxhgltbz.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2xyckoxpm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jwtlbppe.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2jbzbalqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dknzparq.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fepchwpa.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2wmsonsgy.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2nfffkbhy.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2tzlkmbwh.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2kqhfspkh.html


<!-- 参考信息 -->