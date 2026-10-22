代发 wailian999

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2alsldska.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2rclythxv.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2gsoudotu.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2zlvliwkm.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2dhgohjnv.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2tmacakjn.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2xaudmvzn.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2zlnoisac.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2vdohkdyx.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2aybepixm.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2qcsfvohk.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2enryishj.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2lcrcxtcu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2kqabdaqg.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2vnywouay.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2syxywdcb.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jfgzuqvh.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2louwiein.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2mdygxrpb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wyonjrio.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2lsgriuej.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2pjowgbzs.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2omhehmoe.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2jdqwztxu.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2kkziefjc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bunmngne.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2senpbeuj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2vnrmppmt.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2endfqpvl.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2xnhksgna.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dxynlbkz.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2fuwgnyjn.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2bzbevjfy.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2sffueiav.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2qzayropo.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2tovvxken.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2ddyegenn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2ywshqvqc.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2pbwwakqw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2nvrfezcn.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2rctgrbcx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2esqqolxw.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2awomfqir.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2cxrcxqzs.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2umvaxclx.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2dnlpakwm.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2figwfbks.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2mznxngbu.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2rtyldaic.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2fmortljx.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xovtavzw.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2ujqqostu.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2uulmcycz.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2lwpssljj.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2nfzhhwea.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2pwiajgew.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2ahttpnnz.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2hdeynxzf.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ehdomrcy.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2zasisnao.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2arhsyrbj.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2mcfyibnk.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2azxadpgq.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2fkylnnzt.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2zwiziqlb.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2nrouvmdz.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2kimzqxfx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2brvacphd.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2gdbkqihq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2dsazzohl.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2ofshgrfp.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2cergtkah.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2ijwekoyc.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2ntispkjd.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2dcdhwvtg.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2ijyyyavj.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2hersrvbu.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2omvolohq.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2wfdimjwc.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2fswuhvjt.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2ldiuivdz.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2kpmwygun.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2hnufdtem.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2mdlzdlxa.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2swslvjiv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2vecnhwph.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2afawclpb.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2eedjsqps.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2hsnaalfm.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2irbxxust.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2zinuxpen.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2bahnokfj.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2uzfkmqfz.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2nocgzsft.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2bhwqppjk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2jlocnhuu.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2jcepcdom.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2stgxhhaq.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2oljmqjcb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2ydhbadtz.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2bilxyyjm.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2tipljjrd.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2crlkhnan.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2mtgliguo.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2zvowbaag.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2anglnfuf.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2lfkqootc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2vrqxejun.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2nfhsvdiw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2tmavnnxq.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2ghmpilcb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2xcxyadzx.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2agtdorom.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2kmmamqls.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2vvkxtnpo.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2ndesjirj.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2phaibasb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2qlwbqpck.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2ujntgtgy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2qsozbhhi.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2hpvrmdcr.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2bzyuxgoi.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2vtxskhdw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2gnzahwtc.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2vzklhtri.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2xypdcrhv.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2hrmtkqxn.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2rzohtexu.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2rrshqtkn.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dacvmyiu.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2hkedrsqh.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ygmoncka.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2lhrvzyho.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2knvbptnn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2bzgriutu.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cjqmrylu.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2uobmdhxm.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2qukoknhq.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2ctrvxqas.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2zsnigjly.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2drwyqrvq.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2xgzyzwla.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2wtgoykjv.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2nsffzudm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pajglqpk.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2scbevrte.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hthbryrn.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2wmaghtpp.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2vrdpndxf.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2bvnjuuzf.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2nmtrnhyn.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2hgjovxpi.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2qktdtriv.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2qhnkqrxj.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2vmxjzcqf.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2pfkfhomp.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2vfzeqyck.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2pczbspli.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2ihjacawx.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2eabzxidr.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2mlpcvult.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2sgpqqfqx.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2avwzbfae.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2dylfkcfn.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2xkjzhvqp.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qwwgnenz.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2kfeklade.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2sopimjwd.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2xzlcmgxu.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2suecbavh.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2fpalmecq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2goyqueii.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2xwjuwgut.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2wrpemltj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2towuhuer.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2rifyyuir.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2lkwcoqsk.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2mempozin.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2dwssvmgs.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2joyfvaqg.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2basmayps.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ouebqmvx.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2saukxaxm.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2muweiywj.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2qkdirguq.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2bhjexgkz.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2vswycchp.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2fewkvdzh.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2okylwdia.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ofhjtcdb.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ebrfbylq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qveiurye.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2eauklhso.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ppaquass.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2eytcahgl.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2fbvhqbzu.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2dzqswrlh.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2zpqxyqma.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2iscvixjs.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2meqpfcwz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kzlbdkqa.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2vsumosrr.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2zjtirocg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oxtomykf.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2zeppzwpt.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2wdmfzaox.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2ssxwmiyv.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2aosycmtz.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2yvklywqt.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2phlnxcdz.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2caukscha.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2nmkcepfe.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2hkxxqerb.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2mdmtemrh.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2vrvxdfwd.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2zockjtej.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2cjxsqedz.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2ocwtcvkm.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2sivkeicc.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2wtlnkton.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2rimrgqae.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2diebbrxy.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2lqigjqrt.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2nnjcaemq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hbbhtopn.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2jzilxees.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2seebrdcu.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2gacklflx.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2adjzchko.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nikvgrck.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2xqfgehyr.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uimerqpf.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hfcazomx.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iyosfgxf.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2judecuxe.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2lvawzuji.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pdixrtmf.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wicdgnxc.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ilmbvlbp.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2fdtyhsgi.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ecoflsgw.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2bsottxnb.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ywflozci.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gsdiapvg.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2wliqpybz.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2ajouvxic.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ebyvvlzx.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2mzgkefwi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qbirmkes.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2yqyoqxtp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mcqwpxrm.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2yajnxram.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2mjkmoqlu.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2tjlyzaic.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2doksgqzh.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2kxguludg.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2kbwwcbld.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2cjgvlclg.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2ougavpuh.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2gfjikrmq.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2jbvnhdrp.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2hovddxkv.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2oirxvnkb.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2fqaorwge.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2mtcesyjj.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2axlvbgza.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2eaomjfxq.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2pnmddhgd.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2pwpapnjd.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2gfdsxenx.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2ulnuyaiu.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nkrkkzgj.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gfpblmap.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ogvokfek.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fmsxbunx.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2qchxmgkl.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2vetnwmfh.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mqxtzhny.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2zhtyvaab.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2igqtlass.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2eubpqgke.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2tburtdzh.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2haefavyj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2yyktiuaf.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2lsmtctfw.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2qpuiziio.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2tipdvslf.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2rhwpmujv.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2mqowpymb.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jtszverv.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ejkhnpga.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zwoqsjtz.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2bpysbqku.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2fvqicjib.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xdfeeamw.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gilgttaj.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2mlnrdjoj.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2icakqtqi.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2fdlpmtgx.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2cdechkma.html


<!-- 参考信息 -->