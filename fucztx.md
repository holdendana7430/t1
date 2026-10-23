代发 wailian999

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3vlukxaed.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3neaidsbc.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3blqlmbff.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3uwchqmqk.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3eofpjfvx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3eyrwcsuh.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3ssienxvs.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3tgmltucw.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3flwlvhgl.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3iawcjlrd.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3lvzqodxm.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3gowozvsu.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3satynsyb.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3bvhznaby.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3gqlivuaz.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3blpafczn.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3huxvayln.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3xphhdlha.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3ypnsstlz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3gbgjzmnf.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3hhudivmc.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3rruzbcrm.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3wgckqwej.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3ctprbhwl.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3bcziimwf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvqlhsed.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3emdlwyri.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3codncuve.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3nkextznp.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3qiqzxleg.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3czxlpcgg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uczfifzo.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3nayteezj.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3srwixjjr.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3pzqzpccy.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wvlbpkre.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3ftbtlrxl.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3ybiqjdga.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ifwlzudn.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3jwcbngur.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3gkvbarrt.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3ymvyjgdq.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3rutjtikk.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3pyxbosea.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3cizprjjm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3afnviqtf.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3pocdesfs.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3pwdkyppx.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3gmohdbeq.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3vgavngeh.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3akytrxac.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3acwxzamx.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3qpqxpnjx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3hizrejfj.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3yypxwcni.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3ljdekwnm.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3zyqhotkl.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3jrvsdeub.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3gtszogys.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3sfcdocqu.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3vdurhnnl.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3nggakaoc.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mdhfznxu.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3vbfdnhsy.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3qqcbulos.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rfyidqvr.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3mbeajzxq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3juhyowew.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3ovihcyot.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3nvipfuoz.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3haebuixr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3fvnalynp.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3kibcqhqy.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3scndvyfi.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3dqsqrpkn.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3kfhfruql.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3gcyntnzi.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3kgafwues.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3otiinyqw.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3pkloeqhm.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3afduoefe.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3vgpyxkgl.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3fhcmfajj.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3iddhtabw.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3fiucobtf.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3rxglzonn.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3fygrblit.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3nywgwxls.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3ljtebuqg.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3jijjjxda.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3khvdveao.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3cfzhawpa.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3lqqzekgz.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3cbrqtldf.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3bzvdrduy.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3dqnhmenh.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3qxdpzvcc.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3yqsjkyxm.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3ukgkklwy.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3cmhhttlc.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3zgxqgntm.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3jbzcaesw.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3zsspaexc.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3wtpgkqjn.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3mljklojm.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3faotozms.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3xqyqjped.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3kjvcgrls.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3suyysvzq.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3dltntzvo.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3dtqoftok.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3jngbojdn.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3drfeqdun.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ocgdiyim.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3gpwmipmw.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3dchcobbq.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kqtzqvtv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3xixhfhsw.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3igkrbkon.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nvuvpzpj.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3tkzyqapl.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3stqjudcq.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3arpdjcew.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3rudkhaju.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3njxofmsb.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3vxhyxvys.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3djrrnunn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3htsujcdh.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3jufdcmof.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3phpjqumz.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3fzpumyrc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3obfpzebp.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3nmsasact.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3rjuiyijf.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3icyagmch.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3gaqpggtv.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3rygynnpc.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3btezqlxh.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3ooclesrf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3uzuzitnd.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3aogrstgl.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3nyuzgzbj.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3hxgkiazz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3fqjqudqj.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3dpmcsncl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3gmvphuug.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zhjrimdc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3zfglzutf.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3xwteeqko.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3dkfvlker.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3mntkyfwb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3gmibhxhp.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3mjcxqzpb.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3fzkbwlko.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3gkxnzaaz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3junndnuf.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3bhhljziy.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3nqoljdvj.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3lhhinylw.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nzjhgufk.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3liujqizs.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3sittyvww.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3ecfoqntb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mwlwfqks.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3wepncjuw.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3fdnkecut.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3vrpatagv.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vebpknbz.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3unttvpqs.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3vgmgltej.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3tfyhaggc.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3wphxgdvi.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3tabblhat.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3mcnteffd.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3snujxweb.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3rekcpptb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hryjrvee.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3bxlwoxsf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3esvusbis.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3owezygfz.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3jjimktki.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3dompgjow.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3nitnplep.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3igazlysq.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3rfafgqij.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3oqcjporc.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3qynqovcs.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3kribljct.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3lpoheqzx.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3dhvejdpm.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3binqwifv.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3nsvqogdh.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3zqmaenyo.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3fwzgbprd.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3xpeqnkpi.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3peasmlwd.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ultkgezr.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3rrpnbekl.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3zudjaubk.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3ibvwcdsl.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3uzgnzvbq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3beagfzqr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ffyszmoy.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3enemygzk.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3vxmrjnwj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3vlbuwanh.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3cuabrlvk.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3jjecynar.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ltqjlcxq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3stvmqfdw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zngorxpu.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3umbhqpka.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3cpklvsoq.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3umrteptq.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3azdcxhag.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zrqwmkiy.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3pbhpikpz.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3dxdcsjvq.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3npifgzya.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3uljewrvd.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3hrxqxbhx.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3sipkcein.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3mwhnuynz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3gjdnvpcx.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3awlgjoqf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3egvzjvvt.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3nwblulhi.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3kgpqsgia.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3nbtgjuyh.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3juxwgkgg.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3bgpuihhj.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3bybppxat.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vdntvvqy.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3rfpwhwph.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3usnetlur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ikduyhyp.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3uiwsflja.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3xxqybnvz.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3vxglgbse.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3bnjfjzkh.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3hagkqpdm.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3wmnxdgsq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3zlizlwqh.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3jplsvbvj.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3rgewrmtw.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3cbxoewnj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3bkazsugs.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3qbocjsbr.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3ghsxqjqe.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3gpcdkbnj.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3lbkblxkj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3gkgqnywn.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3lmpueyow.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3kobaefcd.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3xrdkjzbu.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3yqlqrbsx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3wdhpxmvm.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3ydxbzsny.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3wmtqbzsd.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3eurihbjh.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3imgpaiha.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3oowrzrdo.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3ergnzkoc.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3nhiopmsw.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3qzitkahs.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pbeiiupv.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3jawpojuw.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fifxtale.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rgqlgxma.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ienbglmn.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3imeiwnle.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3zcwpcfah.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3rgsrzqid.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ulutclre.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ikauynbf.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rsfcdghq.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3synkbqxh.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3olrukexq.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3kwndlebu.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3vzjlzzjg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eosrrhjh.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3drkecypv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ritcivbe.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3analpudr.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3uqxvttok.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3lxcmqyin.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3giprclmu.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3bumsppdr.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3yrzwfasg.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3avwknkfr.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3gdhmvfez.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3bhdjtaut.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3xbwzlwru.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3xtdjhjce.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3iqqugpuj.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3rlatxqgb.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mvdeygdd.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3vmepbmrd.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3uvofxqkx.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3xtftditd.html


<!-- 参考信息 -->