代发 wailian999

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3vhmacaaz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3hsybdhfp.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3tzluaghk.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3qiyvudrb.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3pjhrdxnh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3tovzwice.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3odlofrig.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3vpcgpfka.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3torkehwo.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3jvqpjwyq.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3iueaawnk.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ltlhfwwh.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3jjatiwzp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3frgvxfbn.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3afcrvygq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3teixtxxn.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3edylmxwg.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3phnderim.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3qlpvqfmg.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3trtqmvrb.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3xbekqzax.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvwswxcy.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3swctyyjb.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3sugcyvdc.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3tmesrpff.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3sreyrkxc.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3satypasq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3ijuldvdn.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3pddjizsz.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3rrgsjxfv.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3kxkuqkdi.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3uolrvwpd.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3lmbgmdhw.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3ibslhozn.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ioqduhov.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3nqwlydxa.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3yyzxtwoo.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3rehoepin.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3gsjkhbbj.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3xlmfknoc.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3tyxpipli.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3nzbyjtwl.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3tnhzizdz.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3wpcisypj.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3pizrijod.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3ukcqltol.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3wtcoehsa.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3clnqzssf.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3dhcryxzf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ddrgzxtl.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3pnfdxfhk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3xaymgfbb.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3ifkxjyqu.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3oytqhqtj.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3ukvguhfe.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3fvrpsbek.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3uuivlagy.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3fublhgky.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3phxzaxpr.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3mbgvyifh.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3arjyeyxi.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3iqyfdgvu.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3wcrrzaob.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3qtpruvsc.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3ycccbjep.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3hfdcivme.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3guxgelcv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3dpqhwccw.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3uthdwdjl.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3krocywxj.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3voscaesk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3cugaiagv.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3hxljncje.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3spomotny.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3aaywftaj.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3kvojstan.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3duqdwron.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3lhqfirdq.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3eevgkjfx.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3plbezhuq.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3ynabmhjn.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3wwptynso.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3ghrhfqaf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3frwkdhog.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3qrjdgbge.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3nhykjxwn.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3dgmrqnux.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3lhwdnejn.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3dyciikfk.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3meopfggt.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3fvlkpgzv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3qhplejsp.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3sogfwpjb.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3vneseyxc.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3zpflobvu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3qaxlhpsx.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3sncwbjwq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3fomvdhif.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3gnvyfghb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3gkqjjjst.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3dqpxtzzf.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3mgwcluvk.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3cplgrbjd.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3rbncsyop.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ecpryfuf.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3gryoybwh.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3bpohjlce.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3xnmwxext.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3hzcrfrmo.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3peamoixy.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3wbtgyefw.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3qtznmcnj.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3atwcetmw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3wmppkbnr.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3gpwgaxin.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cplwwcbo.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3npythqmv.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3tyruzyzf.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3trtsxhuf.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3xupkkpcq.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3ffjgbiup.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3lrusydms.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3yjnkkeqb.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3hndunukg.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3ftpbjwvf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3zqgyujtd.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3lyedxiku.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3iedifdsw.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3izjrdyqf.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ogiiakzb.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3xpngnyyf.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3iunpagdj.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3xcsoxrbe.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3zqshnyev.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3uytelbiy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3jbmxiswz.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3hukkxcpf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3depxtjqq.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3bgfswycu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3kkvbxsrf.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3nczjetpa.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3bszvetqi.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3lodglkok.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3dewrbskg.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3cmtbpdpa.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3tujkztrd.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3ateshbxu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3uoltechk.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3upfvwepa.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3fhenwtxk.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3sliepvxy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3wjdoyfth.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3rhchccro.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3gitysxpw.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3uqjmbnlt.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wcyijesa.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3nblpceyz.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zdxydadu.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3dmbatoyo.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ekxboxpe.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3mviecmfr.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3nazekkwg.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3btwoeexh.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tnwxqcst.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3fnfsjcec.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3sfvqsrhg.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3eunbnvtg.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3haqazrxk.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3rvzcqcto.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3kpcelsjk.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3wmsxkipt.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3auzdrcmm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pntelqrw.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3nqzdkbne.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fzlipebj.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3sptsuigx.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3fzkmrqcb.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3ivgupfux.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3wmghhpqy.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3dpvnjlns.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3gaupteav.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ecatjzyo.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3lkyacwut.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3qolfckok.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3tfzqwxht.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3lwcgapoi.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3zwtfzswe.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3bwlgoyvn.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3gsntqqbu.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3fbopknsz.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3ievwznre.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3bahmsuom.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3mnohhsxl.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vrrjadfs.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3erlqsnme.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3qcgmkkde.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3vaoflzeh.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3jxvwsafo.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3dsyvbvkj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3urfygfwh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3heskkcqw.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3jwpshdpb.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3qvlfwosv.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3fmdktasq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3wcqvwloe.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3ambrlznz.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3yyvyiibq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ftoathdm.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3trsftbea.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3shcilmba.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3zvueocep.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3rmgmlzoc.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3hzzbqtuk.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3pxxohryh.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3sjfbyyrg.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3gggggvla.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3urnjmdcj.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3xocytebh.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3zvzpckgs.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3wbwomdlq.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3moyutukz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3sunvnwdk.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3ipnfnxbf.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3ikrrgfhk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3nqviecsy.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3wrwvgsky.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3phyflkqx.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3udebdhrz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ojpocgtj.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3psggjpim.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3hetkktpn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eflguvtv.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3yyfbhniy.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3tcxztomr.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3ttxbemrs.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3hdcbcijn.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3nbscwzlk.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3sjewtmpl.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3vwzlmlsg.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3gtqksikg.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3muuyhbdg.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3ncrtmxxd.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3hvvcpucp.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3ktszgdoa.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3uolmmrlo.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3ufuwkiiy.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3yjkawxmd.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3zhjjzawb.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3orvctbst.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3ccwqxrsr.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3sbiuryxi.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3nsljrnam.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3fxxjywho.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3irryzfqq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3rziysvye.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3jsyfadms.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3anstfmmd.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pxbxyafd.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nbcpfzyi.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dvxpffkf.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3qveixzfx.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3kkecmbgh.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3abtnwfnw.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3amzcpqbk.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3btvjiddi.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tgzgmxzg.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3cnbxvfpe.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sfazaakr.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3xbakoxer.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vzhkbqet.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3anqixnlc.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kmdmrnrq.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tlbwnimp.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3ezwyumyw.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3xbhsrnun.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wasujytc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kwvntjng.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3iargvrxs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hafxlhns.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3shzykgan.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3legjcnfp.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3nldiawhu.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3xdconpmt.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3babrmuia.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3bzcqfcrb.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3xjywhsei.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3zmvvawlj.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3gcbxhkwn.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3fqhdzlca.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3afrxbbxd.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ygcrltnl.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3urcdoykb.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3ucwieyck.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3mqbdwiey.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3zckrcycy.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3iimmzmma.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3dzfmyvfk.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3wxlcrcdm.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3tbixaqrs.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ffvluvmr.html


<!-- 参考信息 -->