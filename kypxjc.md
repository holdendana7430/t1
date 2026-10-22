代发 wailian999

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2mfuxnoua.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2slgvifib.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2fwujyosj.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2dfmrerhf.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2uiduuyrv.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2mulxwiyp.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2scojtrmg.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2pmcoviov.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2fqjjkfkg.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2jxlfmbvt.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wtqfifrv.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2yakxpplg.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2tmrajhyl.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2zydnncih.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2kctlkwcl.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2xqjrgfvx.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2aunzdjer.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2aotxmmhb.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2odabjkge.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2ogjidcbb.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2nzundjbq.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2assvsrks.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2phyxsgoc.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2qqkaived.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2zasobelq.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2mamzfdeh.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2bncywceo.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2sqkchhsv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2qxrlfwsa.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2wnfvloja.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2avsrofrc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2tqkiyjbg.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2itbzqaxk.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2rnzvcssf.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2mwykakek.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2ddqcgqwh.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2okmmsyij.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghzzhtvq.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2ewpnaycs.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2ygkcwqdf.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2mfejogyd.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2esguruuh.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2nkyvzduz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2otwpabfs.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2rdyvmgjn.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2pjkodfol.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2ardlpnhl.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pwvxzzad.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2cqlofxvq.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2zaoftrwg.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2zogpxjrw.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2rurcigfb.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2txabpbkh.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2edmbeklb.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2okyjydux.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2yelhruqv.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2urnmvjgn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ynqlazix.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2wfzlguhg.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kqwtchzu.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qotfkhwz.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2kowsnzml.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2iqbdwxyh.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2rtjnsjxx.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2exfpnqko.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2oqbgfklt.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2pehbeebi.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zhmgqlxh.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2wityropc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2xcwpxfku.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2amgtpyoc.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2xizcdcrg.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2gqfvduyr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2pfcpmzzn.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ripmhhjf.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2qafbxnsr.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2duqqurqc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2nthuattd.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2bnhrxhnv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2dsdmbubo.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2emkikuoa.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2lxaaevgr.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2lwvnesdz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2ojoavvua.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2tamzujtv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2vcqzessx.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2lvoicvst.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2rcnxsggt.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2wrwkawqu.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2jojmsldf.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2vlolzaka.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2qoimxuff.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2hhebwuvf.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2mkfcagjo.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2jmvogwoa.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2fkjxmwgo.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2gfcpfikh.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2umxxpoyo.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2zpexihtu.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2pxujdtfa.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2tfqijpdm.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2pmozavpj.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2huyqhtyy.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2blaqjxqs.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2kxgkjdcf.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2kjfwpnlm.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2bicaqmar.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2eviplywc.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2lotxafvp.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2wepfzvbi.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2vxutjjub.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2bvmftgyh.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2xwpqaibc.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2joucpkvh.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2rnntfafk.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2cmypxoke.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2cyutereu.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2mtdzdtpf.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2xlrcbfik.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2ervamgty.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2dezogcsg.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2vbikycyb.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2efcfhyus.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2immmioil.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2pnrczgpr.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2sprmtqgd.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2nsyldhpi.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2klsgtxct.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2dnichrfz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2ouvlwdzx.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2oijnekel.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pmjtmpdo.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zpnfqrwo.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2uzxouigz.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2slidxfuc.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2opsmslkk.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2nfkgyfzo.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2deaifimw.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2adrqorfl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2finpnypt.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2shjhrskz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2iirthmmh.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wflrqelt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2mlsamfmc.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2wtpdtsam.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2fjjgdrel.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2bfacufsz.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2okktcqrs.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2vedulwnc.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2ciugypxl.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2eumtnyos.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2ggczqlvs.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2nicgvdqw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2muavrfux.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2irbmwpzf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2eszmvblp.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2xbduqqcf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2zynbgcbj.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2bwgyuzvi.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2pgcxdqea.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2qmkwaflo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2hgnsinim.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2jlatrlat.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2jymybuod.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2hdmebqyr.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2tuyhszch.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2jfdytees.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2sspsrhww.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2wbqloyah.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2sbuwvolz.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2govbexib.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2twgfiayw.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2iedxqorx.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hopkrtvl.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2oqsxbvzs.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dqrmvsgm.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2zqcdgazy.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2nrgiktnb.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2nzjgkhgo.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2qhjkurga.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2taveevtl.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2pnzvtgnr.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2lilyvvlq.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2domeuohf.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2pqturpeh.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2kdwsnudn.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2pryjcsry.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2nvroimqs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pvhlvveh.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2oipvldvj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gwiskciu.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2rvkoclcj.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2urwbcaju.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2cgykyjfe.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2xflhohbe.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2vvazhcab.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2txqaequm.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2xqfmxboi.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2qezdxzxz.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2qxfvgtfb.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2xnjsljdp.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2ajmmhobu.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2ixeqrbgf.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2qglutjhv.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2diumwabm.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2almehgoh.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2uxhcsnmk.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2nlbtimeh.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2xzmoltth.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wgscdaln.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2qipgwswt.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2soaylowb.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2gwxiderl.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2dfszwngz.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ucfoawiw.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2pbniawpt.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2fpihyoja.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2yoamtljr.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2xxqebzal.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2clrcvjso.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2cpnvqpss.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2zkweqege.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2aqsqfaci.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2uwympceb.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2arijyofj.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2tgstcqfp.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2wwcsqllv.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2znircfxi.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2mvwkwzvf.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2lgoowcch.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2xhuecvqa.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2zgqpgcej.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2wbramzaz.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2znioajhy.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2upboopwc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hllvksur.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2ewpljqvf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2exzwmykl.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2hnoundfv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2apnjsrsr.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2dyxvgxfu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2ubdofouq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2nsdkwbdd.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2pfpooqcu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ivagjhcy.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2gedkyfcl.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2vqquteye.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rtmbpflm.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2ktbtmmeo.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2glwmrlbd.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2dsvgkymx.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2vxyidjwl.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2xfbsdsvx.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2cprpytyb.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2wtfrneqe.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2sistnexx.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2vutxbham.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2uzfnvvpg.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2nguridgp.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2ufmfdsut.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2qkhxxhtp.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2wqnwetim.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2xwdvkagz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2xntgsedl.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2tywtskqf.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2xnwjjpls.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2hxeoglwi.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2tckilcsw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2hwwhzrfs.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2tvxpgrif.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xykiccxo.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2asuqstjn.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uyujrpox.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2chvrdxsx.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2ueuoogki.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lvaztbmn.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ktrbykot.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xvatqxao.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mzwgtari.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2yuqmkqcw.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2zlkhwkqd.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iuorcrbo.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2xvglwnup.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2brssbtay.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cwfqqovs.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2njhozidb.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ggdlbytp.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mbiteglq.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2njvggjkg.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wzbrfxto.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2uzlwgjhm.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fqxlktly.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dobyemdq.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2erapsdjg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ovqbmiqc.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uzkvksez.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2dbsivrzt.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2mrzgscth.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2omutzeba.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2nbsdouap.html


<!-- 参考信息 -->