代发 wailian999

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2kztiskfw.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2fkfbgsjd.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2gfqjlijf.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2mjofqxvl.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2sispfsnl.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2jpgafind.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2ynswjnyo.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2ttilmgok.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2hwhuvrxq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2wnruodre.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2bzpcylfi.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2kficllbs.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xxktolrr.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2yumnjzfd.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2odwsytnz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2dejzvrez.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2zluvpoxe.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2aoppaiuo.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2hltnorpt.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2mtabfksh.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2fyhquhhw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2mfbwvwcy.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2ygpukckv.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2dvhyqxdu.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2jmyxircq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2ntxjocfk.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2eaqneabn.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2hjallmor.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2hmcnqrad.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2stecywbi.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2akvubrre.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2yjcnskkd.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2hiyopynz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2hhmxuejm.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2hfbyvywf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2uqiypgkq.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2azttpgrt.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2ptjpdbuu.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2ndhcvjhw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2ldqbdlme.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2yvrclkua.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2yuxvotvq.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2wlpypond.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2gfhrpmel.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2ygutzlty.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2qghhclpq.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2tnajtmcw.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2ehsxyysi.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2yhvpvsfc.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2ajgwolxj.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2gquxtzwi.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2eklpfotv.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2hhcklhzg.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2dpzafpoo.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2sccwiypp.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2fhvyvsfl.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2ioucnmpq.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2elqaesrc.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2aoiwqkyk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2nfpmnejk.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2hicvzrcq.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2zeyysxjr.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2cxjcoonn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2dzggqcqy.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2wamspswk.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2klegyeym.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2buonzhgb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2dzlpamax.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2qgmejypi.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2wfsjnrqf.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2yuoyddun.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2wiltenvv.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2mljfidkx.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2rgucbqea.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2usdrbszx.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2gstojbxb.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2mfwkiktj.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ettdfgys.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2mmawiydt.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2anvrothq.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dttjonws.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2dedyosno.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2whxigpzd.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2mgybdjup.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2tjzgcijf.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2mmdghxff.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2tnfuiqfv.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2rqkrmaob.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2fikspprr.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2iljsengx.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2ldfxzavr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2gunbbubq.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2lyuweioe.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2elvatqnq.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2fclkzbwt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2tiowrzkv.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2keuiwsxh.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2dwcumiwj.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2jkqjndnb.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2czxiopzv.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2mhrsytuq.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2jqewiehf.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2goxkhecf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2csruaofp.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2gktawkdp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2butzsopg.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2nidvklfu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2wbycdxkb.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2eepxxwuh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2temwsrii.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2goacinbt.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2codyoqfa.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2acadlijk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2qgzhjebq.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2sofaskef.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2spebfmgs.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2pfjiijyw.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2pdtywkzu.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2msmfxzfl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2rgxwtwrl.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2rexvdkup.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2mpjtkhtr.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2okbdqesx.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ubhrpaul.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2ssgvijui.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2drizkebp.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2gdfymubx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2pzdrpfep.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2iexroyui.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2dlqfhsvy.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2dcxllhkt.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2zulybcya.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2hhjbeldb.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2peakiptb.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2tzyvbnms.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2yaakvchc.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2kwzazout.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2frojdmmy.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2othbuukw.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2nxeewjac.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qsxgeexs.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2tbmfgijd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wkhqvwhz.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2nhsrgcuo.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2jyejfwbr.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2butjbouc.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2hpmnrxir.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2jnkqacsp.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2lbmcfaam.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2hoibjfnx.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2imljwtiv.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2aapvzflk.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2pxtjoxai.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2srxmcetd.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2qjprexpa.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2diznqsyb.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2xvgbcmge.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2cueejtkd.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2aaggxjqc.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2qdozldyv.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2kbihesie.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2gobqtfjh.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2jqjdpzwf.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2faxmoxvk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2jgcduywk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2awahsjuj.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2fricqroy.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2tnydvbmd.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2cwdyjggj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2rvlfofrv.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2wtcmtzxx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2xzsdvcso.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2huzvgvze.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2vgmlmvfh.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2lwuuygcw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ygoeogha.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2mjtruvmh.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2huomfxxp.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2zniyegbc.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2baedhmji.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2qxqgunmv.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2pelgndwm.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2fftpgzrs.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2mykxipsl.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2qbghukvb.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2izeaawdb.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2raifijfp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ergznuhu.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2nfmaanly.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2penzuvwn.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2xupueqkt.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2khzezfzv.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2qhnmpqye.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2liifpbcy.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2jgqvxojf.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2ahkgnrxr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mcrhdkie.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2mqjrgrcn.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2bdkxwcbe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rwtwiyae.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2pjdruljx.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2rxkesxjz.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2jnoxlxic.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2dupggofx.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2azqlecrd.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2bbuhiuhd.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2ateppzbq.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2osmtysti.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2jirslebe.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2ugjwnvdv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2elrrlfis.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2tysdgkvs.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2rfkpigte.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2cmxjzwgv.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2wuctsqcq.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2qfvrskpt.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2hlsfhlhj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2jevnyqbz.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2fypzlotx.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2hokusjhm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2jjzurwst.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2zgxnppyu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2kyufyesx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2paosgpvg.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bxkscvxq.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2wyzdurnp.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cztyoxfg.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2giemhkqc.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2wepiyyxe.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2zhhpjlzz.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ydbdjhar.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yrgdkqgo.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2winfqitc.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rxopepjb.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2csnxyrwc.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2chjgdqma.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ebwcgruw.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2uiqroxuo.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2aanruwhn.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vempwxjk.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2nyfvclgz.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gsnhlgjk.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2sisthmvm.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2dvxjtuum.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2viniapcx.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2yfnkwzpk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jpikeiwm.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wpranmia.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2bemhzpsp.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2fkjnrbaj.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ecgenoew.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2jveniclw.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2yryblnoq.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2iwhokzhh.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2sztlybvh.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2tknqbeiy.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2mfsyawok.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2lxqxnqxg.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2nhxcaghl.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2oqwiwuwc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2kkaivdgd.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ivqzpxde.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2uqglztac.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2yjckeccr.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2whdocjkq.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2xbfziuss.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2rccuzeor.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2uazhnlbq.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kqukflct.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xbujburj.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xsnunxvb.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2pdmwywnz.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2wzrbrvrh.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qlkhposq.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2xvchmtfm.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2jpbsiomi.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2pszgitfk.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2uvhyvtxi.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2hhvorxrb.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2csibfsag.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2wxegextz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2zrmmiudp.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2hpmjjxtr.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2ehgmdpzn.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2suvztnyl.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zcwxmclk.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2midqyozq.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xvpizicz.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2dbufcisv.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ksayofjl.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ylnlylbw.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ixdzfzkx.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2zsrzkkau.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2dfdhaqrn.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2wnrnlokt.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2djlotdaw.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2evhhkuiq.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ydmtpuoe.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2eqkmiffd.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2jwvkemqm.html


<!-- 参考信息 -->