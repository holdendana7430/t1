代发 wailian999

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3txdnwvtl.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3etbnbbhr.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3czrftmyz.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3dexsfuyk.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3fmzftafc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3ofcvmnrk.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3inwnysnt.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3ntkzqrpx.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3zngtskda.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3haajlpgv.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3aiqrhcfz.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3yxyqubqx.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3cwfpbbcf.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3wwzrtjiy.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3mgftlncl.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3kkzckanl.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3qszovxql.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3zogvwnzl.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3jgapoqpy.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3wtsflnua.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3ypmzdtdt.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3ccbcrian.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3osyimhts.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3zddnfwaa.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3fufvysnc.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3uskovknp.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3kxpoxdno.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3jhxxivxb.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3ynuybjkc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3blnrdxqe.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3bothsihl.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3kifljbdj.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3fkelsssr.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3bvxllkma.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3msdntnpa.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3nysvmjiu.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3xpqjzstl.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3shlworic.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3aovimgwc.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3skeawypj.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3tcffuyhr.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3taxdsruo.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3pgwibtui.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3naxigmlo.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3ajqwtdjs.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3hffuhrys.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3bajzvuoe.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3utwcunej.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vqjvbgrt.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3tqkzisbh.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3gpswoedl.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uvwinbsg.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3fifzwegr.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3vrffukwi.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3rnhgjhhk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rugytdvk.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3knuhbpcw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3uusofqgp.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3btdyzmbr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3pgemqzbi.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3qeqavieo.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3umiuazsy.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3dbwtjdeq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3niqzaoml.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3tycjbeus.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3opvztugg.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hhtrdqkv.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3cdpadepj.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3vpttwswp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ebjeewmf.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3jwgmruoz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hgrkltjk.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3ldpnjnzt.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3nsnfttba.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3txhmljvo.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3paknuonr.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3ohfcgeuj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3lhavstcr.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3jhwukyyj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3qqnydjgw.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3iwuvpysn.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3hqdrziag.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3hjmwpgqy.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3hiwzmrht.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3zzyygcpy.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3tjdcsfgq.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3gsnljanm.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3jfrpcnnu.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3mslibwup.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3liiqdmqx.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3ezhotiyl.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3cxhdtzsq.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3abcsaowf.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3vysdvdgk.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3fffjciyi.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3oemugorz.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3rkwfyoyl.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3ggovfpmz.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3ngficlfe.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3txprdakj.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3wwvrnrqu.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3xfszuwwk.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3oiovznfk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3gbaksuwn.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3zlwntjcm.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3vmmbeiwi.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3yocusizx.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3ensrdscd.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3qwiuvrnl.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3tajuovws.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3bjiochaz.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3bvethvrb.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3kjsplkaz.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3tjlubfou.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3oajoykie.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3bdtouadb.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3ncdswmao.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3tqgqctly.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3crvbzhvk.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3erupajji.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3agehihmb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3lpnzbzzz.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3wtjkczhw.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yhyykdho.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3vaciikee.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3dryzndlt.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3juzwefmg.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3joemlpzz.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3pdxmrgjk.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3ioacdyjz.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3rhxuxvdq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3vawomnmq.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3kugmmrmb.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3kfjtjaxy.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3dpxbkmen.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3roommpxn.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3ugqrcphj.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3mxuhbgtw.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3sispclns.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3sdglsvxy.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3eiwrhfuk.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3xtcwtsgc.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3zeoqprva.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3hikposjk.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3jwhiqrhp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3wsmcicvl.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3zwamuzpn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3apvkotik.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3icbydfbn.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3jiqzrsvp.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3exmfeoei.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3owwyzmyj.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3yxjonywb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3zjkwrexe.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3qadggoil.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3cepkoswu.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3unafrcvt.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3yuheuyct.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3vutwfeoh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3rnxdfxbx.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3dceuzexy.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3wdifbbxl.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3jjgdpgyo.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wvhbsfcc.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3qooeixba.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tdtmmpgv.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3kxefigix.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3bqrluzwp.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3amxyasqs.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3vjzphdct.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3adbljklt.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dhlkisev.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3kfbqshhv.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3iwoubnsr.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3cbvtbmam.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3xauamohg.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3wmeelesk.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3yvmtuurh.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3isaphtfg.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3scgdhcjq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3snidwpek.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3sbcmorru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fbrjrtnw.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3ffsiuamd.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3rllwbysd.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3ufabiret.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3qgkouhry.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3rkvvyrbc.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3depqmpnu.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3rtrjmoiv.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3roetbhxy.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3qmpayfwd.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3nveqjkko.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3mkeoueuf.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3chopruvd.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3przbinlc.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3wtmvdgfu.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3mxvrhkco.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3tbciopke.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3jhjpvcgr.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3eetwqnfy.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3xnbagsfg.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3gmvjtgqx.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3aoejeodi.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3kcfzffsj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3vbtajnso.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3dulioswp.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ucqreaah.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3odtcozvc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3didagsuk.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3nchmoolx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3vgbjmtbv.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3fnswyrvc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3avdoacpl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ntpkerjp.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ayqafvmw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3pvcprbuw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3fccratdn.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3gfcjqipg.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3czcpwgfg.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3dsntcjen.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3hkduwxof.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3twymjqkv.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3yussetbw.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3fmxmelaj.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qvkavlqx.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3blonokpf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ohbqfqkc.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3hymzjodd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dwykcnkq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3qpiotmgw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3wpiakked.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3ntuquaxq.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3lavudvne.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3dkauyyho.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3opvgjmcc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wklwwwft.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3sdusymuc.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3ivikavou.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3woctbbkk.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3pxzisomb.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3tpclggbc.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3cvlijbxm.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3myrhcagn.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3xeptaeut.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3obcvetwq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3phivbchv.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3ahtqhcjc.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3hrbktqba.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3jnxoblyx.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3mfxphlvo.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3kawuesil.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3fdujdlex.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3faupejbk.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3ngztboqj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3uncwdzih.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3urggwmvf.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3ewsuypyu.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3xjefjkzk.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3rcmradvv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3lopsfqef.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3wuahsmwu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3siyusjne.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3akcsorez.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3lsgnnckm.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3lhtjrejf.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mpmuhjfu.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fezuchlx.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hlxrqykg.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3riavhoow.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ppiktcgh.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vrqutvwo.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ygkckpzi.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3djxdjpxg.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3uhnoxrpm.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3nqfmjgsd.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3szqusidx.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3zmceplvl.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3eggkpckb.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hxvkudpy.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fsexolbr.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qtvqtvvs.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3fwnwjnat.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3laszvqqk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ondzazri.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3xcmnqfzz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vkimgvez.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3tbvyjxov.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3zisclutc.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3jnpmzrao.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3yvvahxcc.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3hafmvdxt.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3afhreuim.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3wggdmmce.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3gfbkkfkw.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3afblgdzx.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3uotfivtl.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3ttghzagq.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mnbqbxls.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3gqrqejon.html


<!-- 参考信息 -->