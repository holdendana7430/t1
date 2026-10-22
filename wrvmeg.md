代发 wailian999

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2nkuedvhy.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2nnvkzgca.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ottgwdpu.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2ptlgyzxy.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2whoswqba.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2xklrpuuc.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2pvusairk.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2qipdxzoo.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2gcgirphb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2amuvixjh.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ykuyplvx.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2xnosxqar.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2sstrstyx.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2jfuytwgk.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2xofnwmrr.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2deyqwkui.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2lrzqijgz.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2alxptwgi.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2ukbnzjry.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2pekxgocf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2dziiuark.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2rnjshtxg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2tqkkntzv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2rnkednem.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2nnkzukpf.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2wcvpepet.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2pgwrexus.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2jlcnhext.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2zbgmevbp.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pbeeoalh.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2mfseuyuv.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2ykzqiilz.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2veymauom.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2hkvenlpe.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ydobaqsu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2eangkmxd.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2zicfdkyx.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2fhmtjfof.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2gbfrvddf.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xnxrzauh.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2cmpqnewq.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2grdoungo.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2qglsgmkm.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2dsbizvjj.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2myoaqyqi.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2yeuyqlsw.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2evlklgrn.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2cvbmzagw.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2udgtkrfs.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2vzjnythv.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2jdgwbacz.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2vazftwff.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zxogkrok.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2cifmnyxd.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2utmmajim.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2obbmllwf.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2dbxylyoi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2panpucmn.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2ixxbrnkd.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2tcguuzzr.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2qhagvajy.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ewbgaioe.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2nqtyyqxd.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2jwoqpvgx.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2jiitafmq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2vwmoaylg.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mbwzqdwh.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2ubbgapwy.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2xkjbhrqa.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vbkidzxo.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2vxadevqn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bxviaefd.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2lrylsdwm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2rncixnwh.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2bipzbvwh.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2ruoxuetl.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2wzknegqr.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2gyrtxfgu.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2dnbfiavz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2sckicuqs.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2qbealpcl.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2ymuirhim.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2odnzyxpn.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2fuspentb.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2xxwnkurt.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2aycyyphv.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2grmqqlys.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2febhfqds.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2evhzfkpi.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2txcbvyjo.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2hgoqrwzw.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2juultgdt.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2qsxscbgy.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2frdrzlln.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2tjoketft.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2jkwvixbe.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2rvlhevsj.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2fzyxecfr.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2ihldjyyh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2njvpnmpl.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2dcswhqgx.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2olrjoxjv.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2llqmiqbr.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2bqaqxiuw.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2hrhskmjg.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2iwnkbqyr.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2elieppsd.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2modlzpht.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2xvicggrq.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2kqreotph.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2dfwltehk.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2aflkdwxk.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2ilcqfiug.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2lxezbevh.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2buvktcvc.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2jszihnye.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2zkprxxdw.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2czrskzcw.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2jaozxymm.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2zhlafico.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wbytgaae.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2uwqcgqwa.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2cswgrscy.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mrodvktz.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zacyduwy.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2fhbukvdw.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2mlkijhjy.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2scsyqaqp.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2uozwrnri.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2wdejlgaz.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2rdybuqzd.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2eqmiktvg.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2pymxoofw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wumceini.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2xsobwjxn.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2rnvampgl.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2vdupfnfo.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2kurlsosr.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2korybqvd.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2japalbzq.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2yrqlnnkc.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2ypxrjuoz.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2jggpahge.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2myqnvlmw.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2wwlilhtd.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2nxojcdza.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2oamhvcdu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2uxjcydje.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2kkdfoefi.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qannedmo.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2wcblfkay.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2qrikmngn.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2evclclno.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2iyadtgcn.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2lbyknzpu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2ntmivdnz.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2vjphoexc.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ziftssar.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2hewxwxwh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2eczujuis.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2savojyij.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2nxpdcgwd.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2mamzyrwy.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2fcvfajgb.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2zlyobfpg.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2evyukvdf.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2frzuxqjk.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lznienng.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2kyhbmigr.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2widtnlpf.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2sskjexdt.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xchthcsw.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2djfllkmn.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2wsvyemqm.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2mnwiqxte.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2wyywswjs.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2ouzkjdkv.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2kqnjeebb.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2unkjagma.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2hzprsipv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ocqbafce.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2eqonvkjp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2koviabns.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2twjnnfvy.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ntlptour.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2elsgfunt.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2yoyxucyo.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2pnqwjuit.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2nsrgeyab.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2dinnufpb.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2tblnulrq.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2juffbftj.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2qsuksltn.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2igkfcrcm.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2qmhchmpd.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2gzydrgku.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2brhlkcmj.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2kzgjhece.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2rhelfhah.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2qldlxrof.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2xzbugxap.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rxvccijy.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2phyvwoxi.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2qddslaqg.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2uqtfcnae.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2wnvygxld.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2kdvclxka.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2okejkwww.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2wvgbeiaz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2rnbxotxt.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2asnjajqm.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ktbtwrsn.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2cggmaais.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2plfzeuka.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2noidfbfd.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2gzopwyhb.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kjxhohsp.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ctfvzbxz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2dzypjgoy.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2auvikmzp.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2aytuxeok.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2toglpovy.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2knojfdwp.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2arlixdau.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2jrwpexga.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2gnyyhhqc.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2qzjvdzlt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vslvwmuf.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2tkoiahyb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2tszdvmha.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2xtqnowrf.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2vpgogbwh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2llauazcz.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2cjukpiaw.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2mzkfpasr.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2xumyhuen.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2twxvhglv.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2wibfygrt.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2fykprklu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2laofeiav.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2irspgbvz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2dcxzhpcu.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2yhxrletg.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2ttmnuemk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2pxizgwkb.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2qolltaks.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2anflsmlf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2dqguzkkk.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2foypndzl.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2sberuvdp.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2pyuxgree.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2wnwdzori.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2ggsappuz.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2dszvwcvq.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2fuxojkpq.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2tcpzkndm.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2iqbrbgyo.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2ecwnlvrb.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2ffgvqgxv.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2kybacghy.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2luzuxzaa.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2hffzzdjb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2wxfuwcqz.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2caqhemxx.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ttwxzoyb.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gtoqocfd.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rdfemkvi.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tptkjlut.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2dxirrsrq.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2tekizwrv.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2gpepkegj.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hgfklmdl.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tvfbxthq.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2okrocoum.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lnbhlpgb.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gkovnlfi.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qnnyqkfu.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2bbdbpsqq.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hzehxqxa.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2fcgpgyaa.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pigtblfn.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2ijntgger.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2qwkpxcut.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2hdawzhca.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rwngwgrj.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2hyeqdmaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hiaikyra.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vmddacbn.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2pioigclg.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2szjckyfb.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2mrzkwbha.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2iqjfbrxl.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2mktlsifo.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2rnzypjzm.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2mrmsydav.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2lornnqnv.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2vvvigjyh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2nsioakjv.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2hfaqmcec.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2apgqfixa.html


<!-- 参考信息 -->