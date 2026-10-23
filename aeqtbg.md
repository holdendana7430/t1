代发 wailian999

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3kspanylw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3tgrgjldq.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3sbnhokhr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3jxdqvswb.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3qxpljgel.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fsgiejdf.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3bkxhkyft.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3uaayqztz.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3lbyygpfa.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3khrahgtr.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vstxzzci.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3mbswpwxg.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3yucogjnv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zpahtccc.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3wqvmpjwz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zdpklijo.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3xdgeidyl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3ggjsfxdv.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3kswwvogy.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3arzendpo.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3imxcugvc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3lnrspuhx.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3pfwhujvc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3wchjqaja.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3kuzrlgkp.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3rohgizyc.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3utdmlhva.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3rqhzjzwi.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3snycvlfl.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3bvfozxne.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3fmjezmja.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3dvxdhsqp.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3hfqegmtj.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3yllbjelf.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3zrstijoj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3gkmdulae.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3ainaiwvr.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3bhyxnrow.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3obwehegq.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3aokjwvgh.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3ykfnxcoi.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3crfgfkkv.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3pqkftlfm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3bovsphgq.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3qpapkatq.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3apsbmnia.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3wxrcrgky.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3gvufwmpy.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3wehzgurv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3kdpfrzxb.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3uifvoeit.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3mmufsiop.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3qowcetog.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3dngaeybo.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3bxetvfvc.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3crlgxjcs.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3thqtatcf.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3mwerzvnm.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3rtsznbdx.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3iiomvhep.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3zczsteac.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3jwsanqkm.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3ecygsdpl.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ghnlrzzp.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hvwywzcp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3zajdlrli.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3wxqwsqie.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ffmfttze.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lgvpvmhg.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3iutigctr.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3lmxumvxs.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3eyglplat.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3tjevxqdq.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3tuqydsvm.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3rmizklzk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3dgqpgrdf.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3tlssszko.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qoxaocbm.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3hcvzdmdi.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3okdprydy.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3uhlilbzn.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3dqewwwtn.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3dvzdltiz.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3syrjuowa.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3bxkmlshk.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3jubylkij.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3viutkwim.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3bepaacjf.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3gujoyhvg.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3odkkfuta.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3ttxayrrt.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3bobzqhge.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3odpiqcgt.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3enldujpg.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3vftzhyag.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3gzkqwdxi.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3zskhmnvx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3vvuapwnp.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3hxicomvw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3vzjwasly.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3vgpxpjxj.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3nlhzgxnf.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3mvtygapw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3ruplowgp.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ibeocphv.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3igxlpgpb.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3jtfksjtk.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3aqykeqqv.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3rkmckikl.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nltrglqf.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3ojpgmyzp.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mwmdksit.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3dzvyxywe.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3cksblivu.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3uovodhnt.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3vmmhxumi.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3tourhpiv.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3zlnlommf.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3dnqwkeva.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3jgiuzjhp.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3pcgktbxc.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3cyexmwtd.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3ygnxfhae.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3dtbwmudp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3inwgxdov.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3ibeqwwqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qgqnckyp.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3vyyobxfu.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3dmihneaz.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3yjavpksn.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3itzxdamt.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3kytxvgdd.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ojdukvnd.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3udcfbuya.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3upnoemem.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3vjqfolly.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3iuozgydw.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3nxifovyv.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3pyqbsjdo.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3vklfbqwg.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ychwuxub.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3wtgnfhff.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3ioifgczu.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3cjudgbmp.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3zxsbfbzn.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3eqsqhyro.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3oyaxyqqs.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3fagqnmvf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3qwvmaxez.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3txfbvmdt.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3eoffshfg.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3giihvpan.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3umckznlf.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3gwneqknb.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3rydcmszw.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3xxlxtgqt.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3afpcflmq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3pjnzvwxd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ehpjeqwc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3yuewiehd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3duackjrs.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3indmbnnw.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3jdeuwqaw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3asnklete.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3hpykolmi.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3tbnzlqti.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3xsrddyjz.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3qduuxopl.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3aayyqlgk.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3drcyrbmk.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3swfugyst.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3wvlccrow.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3xpbjnwmt.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3cxgnsnfj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3nfbyelap.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3fnksflib.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3mofjbnpe.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3unnhlsxw.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3tucpaqoe.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3xxzeolnl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ixorxemx.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3efjrsyur.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3vobardct.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dnkfncca.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3vazpozty.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3wdumblel.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3wquugaxr.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3bfridpwn.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3aeuzyltd.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3mjbxghce.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3dwusjdwc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3unxqpolr.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3ngaormuq.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3flwmgbzg.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3bxklalqt.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3jfivyhfr.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3onlhoinx.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3thyilgfg.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3nysxmflt.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3uosgzsow.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3apdbbngk.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3bupspeho.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3isowgrai.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3ruobfvjc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3yomcrmht.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3nielqkkb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3lmanzrak.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3vlxbynpv.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3emzchdqo.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vgyzuocw.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3ccmiztrv.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3kdtxlcdv.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3dpeddxqk.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3kgudeicj.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rixyfgbz.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ibskijcb.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cjddkmlc.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3lslekpio.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3lfysmgqi.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3bhmoslih.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3djdjslvs.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3hyfhpsah.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3egpaifne.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ehmmoxyl.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ruxfglqd.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3hhvokxmp.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3jzrkauwv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3mwbczrgf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pumpsnfz.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3gjwduorn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xylcdfml.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cyekpvrs.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3jgtqnulo.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3rmvletui.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3umjnvxgq.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3eqbwoybf.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3drycziwn.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3snwxrwue.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3unktkzpq.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3klqsbilc.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3wopllwhf.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3sccjbtej.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3rsaixhvx.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3dfyrvrfi.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3wdogbimw.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3fhgijaxk.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3advmjjkj.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3sorjvqys.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3hcxqotzd.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3oulelthr.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3xvbjsmez.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3uyrybdgv.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bmafxwgn.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3coodtkqw.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dydhiysn.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3znksqtkv.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3gdstrxwd.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3obazatun.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3mebclgrh.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3oabxmbgh.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3tpwvzvdv.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3aawofddw.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3ofdaidfy.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3lraxxish.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3isyvlfqg.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3tjqdfrni.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3nxiwrmnb.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3jfgvxtjq.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3mxhcahpl.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3geneqlfa.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3nbfdjffr.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lycfxfnt.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hqwnqvte.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3chetuheg.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bgqqsuqt.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3frkytady.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3yhnxkrhd.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3tszfaivf.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3saqpcgyd.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3nybprzck.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3jgasrqbg.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3szctlaqa.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3phmakdmk.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3gmaskboj.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3vfxgojcu.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3idozyzsh.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3nhpazokb.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3edkqwvjc.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3orrgxnif.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3qgnrxizh.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3wmxoojbh.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3mhlceyzc.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3jzwwzdki.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3tzvsywvf.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3pebhkxna.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3gyiziyif.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3dxdtcoak.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3lnbeeekb.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3yguwklmx.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3nzyjofac.html


<!-- 参考信息 -->