代发 wailian999

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3putwrtsn.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3pebcvxwf.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3rcfalycn.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3lyggirpw.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3cydvqpfs.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3jczwkfyo.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3vrqtzvmq.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3weuonqgo.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3oayljalm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3mlfhqbsu.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3fmhikwej.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3fgikzgdp.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3ngfhxtmy.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3ttqvkspg.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3vqnnohbq.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3hcyqagay.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3otfdppbf.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3cvghdlih.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3jejsqyul.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3dbdqhctd.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3gskiwpfa.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3euhifxru.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3wxfypawz.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3xwblkbet.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3xipfogcp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3fwpanfdi.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3egakluqm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3ivjvkxjm.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3iyiohjaw.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3sgygvtsr.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3uwjjuyex.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3qpkpjcgv.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3hmfrajgm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vbkofhtt.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3gqmuomgw.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3mlyrlgqv.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3zvdsunpv.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3qttgnzkv.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3govejepq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3cghrcblj.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3jlxfzyzh.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3brmzrofn.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3xdwaarym.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3lkysqcku.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3tyfyxdfn.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3oxateyhk.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3wktrpvxe.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3khaiatno.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3fijgwzjr.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3fzeppfaz.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3kbomjwkv.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3ugwddugr.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nbyiaqxs.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3wtrbvngv.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3tkceicdy.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dfvoyaqi.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3qdhkrajv.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3jfluinxh.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3ntyobyev.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xrynhgtq.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3ohtfwbdd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3zxsdifxf.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3gpccboli.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3ncatzwha.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3uvhhkncz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3cecbxzzx.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3viibudcv.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3qqtjrjxa.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3zmizlieo.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3gavposwx.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3modayomx.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3hnjpowvp.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3brnhigvd.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pzvijmux.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3gtkzpfax.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3rodmkhnl.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3bvayynxm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3ohvkiuas.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3aqbtbzky.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3qeczaykg.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3nfgkzaeg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3qpdpjtkg.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3orzprwup.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3yqzjyijy.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3lsccazmx.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3vtcvvinf.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3gdzuulbv.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3wgwhouch.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3zpzpavmq.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3xdrdzpam.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3hryryrqs.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3dcbizmib.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3wssqvsca.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3jlxnraft.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3lnuyxoba.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3lcgzqpff.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3tkvngjbw.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3tvphztjs.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3nicwmgnu.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3wchatjqt.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3jgiirdjp.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3hhdclklf.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3gvzgbnqj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3hibbtlpo.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3vccpyhad.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3bkcqdsmu.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3dnwqqhtf.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3lihlihdu.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3ovbzpfwz.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3jrecsdok.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3rncxoftx.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3tkgaasgi.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3zedfgqhd.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3nahotrfi.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3rdrkuinq.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3jbzcoqtw.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3lkaowkax.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3gzolezso.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3podnqjdf.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3zhxqjlni.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3usvtpxlo.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3pgiyllih.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3vjaiuwgn.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ijawrxde.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3znayteqk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3mcwaggme.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3hqbjwldp.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3pilycxpr.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ipyqwaxh.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3jdmnzdbt.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3akpgipnx.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3jiterbcm.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3quhirgpl.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3womezqyh.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3dglxuxpi.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3uurssbyt.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3egptbdzq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nhyuqzlq.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3vmiaiiqj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3wccfvgwq.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3hyijfnnx.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3tngzeumt.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3xtrnjfua.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3fpwqcosr.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3zzjhunaj.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3cxmysphs.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3qzydtiba.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3xlquhirc.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3yukjbari.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3kfpuzjeq.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3rjbahhgh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gglvszmw.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3wynwoicf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3dgqnbcsz.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3vngxwxjk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3hzjkqxxd.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3icjovkok.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3dmsavunf.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3seuzdtvr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3sgctybew.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3ijerzaks.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3nebvmxme.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3lakrkmpz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3pgsmczwr.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3xingjhwn.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3imgcpvwl.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3dfnvmikr.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ctvvhhkk.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3zudimhjo.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wsfqfxyl.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3jifurqjf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3sezhsvuh.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ncwdqdxk.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3karkrfka.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3gixewzzk.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hrpgiwmd.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3xdmjozbw.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3mzvlunry.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3ouanwrza.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3agfwlesx.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3rplbobzg.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3iqevgvhi.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3kyfldwpt.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3qfvqgruu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rlbkklhi.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3eisjomle.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jywuczyh.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3jmkbxaaw.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3daijnlxw.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3ppntjffq.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3hendemrf.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3llzyesvt.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3jvcdwyom.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3zpkzsukd.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3jpcawtpg.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ibktjcdm.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3vavspfye.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3bztnweux.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3gyabiknl.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3ocnjrlzj.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3tdjmtyvl.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3okpryzyw.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3jmagnchh.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3fnyscvtg.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3mrokrjuj.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3gfzvkoeq.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3silkyetd.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3mclzxamq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3crvzfpyw.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3otvvaaxq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3nysbpiqo.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3sqvolvoh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3hwdmpsdv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3bvievvhq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3eurjnykg.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3llcznuds.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3sxasmlax.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3yhsbgpfw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3kaojgaie.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3blyzglhb.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3njchezir.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3thbeetrz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3yfcnmcww.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bttohcan.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3vrxhbtiy.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3sdzzaxsw.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3kwzpnkrd.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3gkugtmsi.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3uecdpwko.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3pgsixyml.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ktogjjic.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3vokzqmru.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3hvfprumx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3lwfntvdv.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3milquzyv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3fefpbvoh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3mwemwasd.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3awjhulxq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3hpfpfsol.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3jxsdgodt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sktfnfle.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3eawxhjkz.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3uwsainka.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lylcxryr.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3bwugkflf.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3fvrpkdjs.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3ukzlcnrt.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3hdfpqgij.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3ymhujema.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3qbkceexs.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3lpdnfktv.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3grpawkem.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3dcgcidfc.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3zgtphpjv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3dbikbkzl.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3llyndfgi.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3klsoqhds.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3gajgbeum.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3gqvjserx.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3ngepugfy.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3brmizysh.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3wnvpdelh.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3bxpmdyno.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3lfgmlltz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3czvakxfr.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3yxpqqpmn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3sjinczjs.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3taszdywk.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3rdnneses.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qnlbbosw.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vuiochpi.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dlcqyrvl.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wtajpsnt.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nhdxriof.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3xtjhghyl.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rivxyvfz.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3vjggnhts.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fegufecn.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rfeirqau.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bohsbymc.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3csoybuhs.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3abtxdawo.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3bgflrali.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cimcwjmp.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ogggejfm.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3bwjzpdum.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3jnggwgnv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3kvqgqinx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3laedyfls.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3nvqehpyt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bijdwlff.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rfpqizpj.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3ytxhktsi.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3qiuzlfju.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3vyavrrzq.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3qkaldiia.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3xqdnjwzd.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3lnvyadya.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3whqfkfkd.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3rocldmvc.html


<!-- 参考信息 -->