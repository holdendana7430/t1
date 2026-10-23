代发 wailian999

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3rsdlecie.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3gjiwbpfr.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3qtrlhyqh.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3pbucjxfc.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3lxikykak.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3ldvpkucg.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3iemksfwl.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3wvhyqone.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3sjbbyhct.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3enzpkjqq.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ajgsoiwl.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lslivbnr.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ocpkufvo.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3skhhlmho.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3jidbxikc.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3lrhrtxmy.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3zpsujgkv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3vjudejhw.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3ftiobypo.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gtzqrtir.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3dpxspdxc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ytysiefv.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3ljyejobt.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3qegvoaif.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3frmocqkm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3ekndozpz.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3opbqaixd.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3clbkvuuf.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3onfjsxid.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zemriynf.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3qaaskcts.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gjdtfstu.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3rrtkzapk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3jtyziygz.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3zxllwcbx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3unweodib.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3ysywqcnq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3jnvcuqxi.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3nfcrltep.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3jsmmjrmk.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3dzlcdagh.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3ifptojbl.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3shcquvlt.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3szxevbtm.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3fkivikcd.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3warpjoje.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3uicprtzn.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3itivmdfq.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3sdnrwfqv.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3giueiqjd.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3xfpvfkzx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3qwdtdbyd.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3pklbnzls.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3aniwwpqg.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3sharnspz.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3mmgalqku.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3ehyvbsij.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3rhkpvoad.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3luhizmwl.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3dhuibxpb.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3chodbfbj.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3ztwyhfgb.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3ekyrshng.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3uhxwiwve.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3mjwlgety.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3jgzoolza.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3jevydxjs.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3vtcqshtl.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3ipfvwfkz.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3uaytivdr.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3nocavcmh.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3eqtmsbun.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ylrfgntc.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3byebxeud.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3apzgnngm.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3jpqtearx.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3hujuqndi.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3dkzevbhy.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3pmpqglwj.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3duylngah.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wtlpcwly.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3xvsuqhys.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3mpnjxhqa.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3iqkvshcu.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wkjdmhoo.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3cfzsllkb.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3vhefbcug.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3kelfsrod.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3stlcbzic.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3nvstuxhk.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3myfwfrqk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3sdocweya.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3kiodresg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3jvttzvud.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jcftllry.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3qmwebhtu.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3damhbcjn.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3vlvcrigo.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3orhxowgs.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3kriqaiyy.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3gojipzjk.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3xhvefnuu.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3dznqtoff.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3buegmvci.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3lsbeymva.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3jjjregnc.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3vgzdbuje.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3spdukkzr.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3tdeujcvs.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ohsqnomd.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3qlsrzpkf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3wznepqpb.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3usbqqeig.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3winfjuuk.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3byjpqpeq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3qidzlgab.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3elbilthh.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3twvfkaxl.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3jpsijgfk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3htldowzf.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3bpmsueyd.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3dldrtwuv.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3qgxhgjfl.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3koghdjsz.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3zversuwc.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qwvhvqpq.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3gqgnpvnd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ywztvlxv.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3cdgppcvm.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3lhlofupy.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3vqmzjyko.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3cghyhbaa.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3bpznhled.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3snrhqndu.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3tloiutez.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3rrzinhaj.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3ettffeds.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3zlfbghxd.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3wvjdyixo.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3wmvncasg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zuillobo.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3gevgstxo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3teaquwtz.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3zjqklzvt.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3vriqepub.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3poprrfqx.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3rbtsfkpk.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3hosnqjvz.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3chcagscq.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ogthcnix.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3rakaamcm.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3lchieyzc.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3fxltloxz.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3okhqfpwo.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3wbskxzrn.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3baopmvbt.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3rckcmplj.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3jwmivewo.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3ehcfbrbt.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3jpwpixfq.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3xvdchcos.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3npclhmtb.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3zifonphd.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3rbyuqdch.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ylvxtzcs.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3wbakpwwb.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3necgexdp.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ifypzqtf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3anxetczp.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3vrllmeem.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ekkbjyxw.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3ojfacynw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ighwwisk.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3mkrmkfcp.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3vhhdujpq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3uadunaus.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3espywwhc.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3lrmmwrri.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3vwuzuwwe.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dixfbhku.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3hagjpllr.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3orycyxev.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3zufwojuk.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3yozmwyji.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3cjcqoikq.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3cvgyebrf.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3rbfhcwse.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bgtsfogc.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3rnnysrxd.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ngrnjabf.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3jnnlfxwo.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3hrneuetz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3pdwsojav.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3rqmwumcn.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3uavmfkhx.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3nlhsbjmf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tcapeoto.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3odqdfefy.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3hxfakopv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rfrfvczm.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3vqoafeqq.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3uzaeqotu.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3shinezeq.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3tttzhukm.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3qxmdepct.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3sxgaunha.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3twdenrsv.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3glqvfpza.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3mtbexcbf.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3bspdlujh.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3oiuafhrk.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3fmcvlvca.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3omskrqgo.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3mrvwxldp.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3wuehzsmv.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3fivyzyej.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3mudrppja.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3zjuiwrqt.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3knlwhiqd.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3jkkoejsi.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3pjwddijh.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3syquvuqn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nktcdoae.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yfdjqhfx.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wudeujrc.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3tyfudvtk.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3aadrsqru.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qbcvspzj.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rzpvvvpl.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3qsajspks.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lxsmrgxh.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rhjgomwm.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rwidkwfg.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3usfbzrbc.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3sngbvehh.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uauombbm.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3mvuuvqjd.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vmtdypvu.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3djhasrvg.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lwbbmezc.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3bklqymon.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3qdpskuxi.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3hyqfhyqv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ajfdulbj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lluzhgca.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3irfvscjj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qzharzva.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tzsvwxvl.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3myettzug.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3tndwcxeq.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3mgpqbxip.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3ecdudvcl.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3jvkaijyl.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3rjqktsud.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3wyedxfvd.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3kgywfmtj.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3fblpbtqq.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3pdygmvem.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3gzbnxwfw.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3evntsenw.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3koykdefy.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3aygtdsjy.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3zchiotrd.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3vcarjyom.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ncqhcoij.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3syctdxpp.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3qihhzqca.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hpweiqlr.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rlreoelg.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ckpktekj.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jqwmiici.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3pkbhdofu.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3lzaagqiv.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ctlepruv.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3vovzlaou.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3laqalxyg.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3jaczaxml.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3izswctkl.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3rjphjarf.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3esfhvnjj.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3rwazswyx.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3alitdzto.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3hbvgihqn.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3rwtqydxb.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3mofmbfpf.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3udqfurxz.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3mgcygwmf.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ysgeskci.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3gqwrrojz.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3riwubnrz.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3yryqjljm.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rqalohko.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3zyxxmrad.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3daehsapk.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3mxrxcnmy.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3qkqgbivi.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3czohkyak.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3lzpvmmch.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ganpugjo.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3jlpuxhee.html


<!-- 参考信息 -->