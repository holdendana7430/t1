代发 wailian999

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3rclbukyd.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3rqqyskjm.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3tknnobwl.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3prpwrteq.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nhvlmeng.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3kgbgixws.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ymxvfvbe.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3erdiaivh.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rundkcxz.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3opmmwycu.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3xeicsipk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3jvnyjjen.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3flkwajoj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cpvpzmzj.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3npdxwttx.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3jzfhaltd.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3usuouzcp.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3eongzzsj.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3kpttbgvt.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3qljawfny.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3wxrrnhbn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3lpbvgbnl.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qmjdrcsi.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3ozhlepuu.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3nchrmvyt.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3iandqsta.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3elxksuit.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gqiilnpq.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3atxvdwwq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3lecqwcxq.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3zgdqtapn.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3afeknsvc.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3fineuduk.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3smgdqoys.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3jlbhbpvm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3nktiwjxm.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3wttirael.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3cgkisxdx.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3mnubxmbh.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3miviywfi.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3ggyrxisk.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3ajmcuemz.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3wsvpzdah.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3ehfmvwrv.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3awzmxnfx.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3msjoghhn.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3ibwxwcnl.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3tuhhlxaa.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3ajrwavah.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3oyvtmnnn.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3cacwkpdx.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3phgrzxaq.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3pfsbqmlr.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3tgprgnak.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3tiaqdvgw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3dchnegrx.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3ytyurodd.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3yesdtgmy.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3ypuojlij.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3kqabtmeg.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3oqqfffsp.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3xvuwvdpp.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3qhurerxd.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3wmhveuqf.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3gwrvystv.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3iinawtvs.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3abpxputb.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3ytammntg.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3rqfxylnm.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3uvdfhyes.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3xfktxejz.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3rpugswrs.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3ixgdpuck.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3lkvpyqos.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3izythoem.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3lnzbvwsn.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nqcvnpxi.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3zcnaoqrl.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3gxqvniti.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ofmjpbxj.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fkrcgyhv.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3nlfpugdx.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3mpxhmoti.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3tejffeme.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3onyvamva.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3nmzkfigr.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3auneocuu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3lfhwsiid.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3ptifghwr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3wludthwr.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3pactkfgo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3vzttalip.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3agnwebwm.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3kjxgteie.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3kizbpoma.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3fhhmjolu.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3lwlulttn.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3dkrsoefc.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3ibfizmlj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3cujykpar.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3zrgteuph.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3bilekelm.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3czyjhzop.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rkkhwkko.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3klzbhbbo.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ocnilxtt.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3yubpslhw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3fkotjcba.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3axtlvfsv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3filgbnqb.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3dxqowhtd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3qiypyscq.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3zbmqsaxr.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3toaxxvzh.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3aljrodkg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3aknbvvdc.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3imjvuuej.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3axagibre.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3uvzolkqu.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3vdrivhrd.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3wkhdtwqv.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gkeaoyui.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3vejmscnx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zutpraip.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ldhjpavr.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ohoshoel.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3rcurgvqd.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3cyrooumo.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3oymoynys.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3liatgani.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3rgvdtndp.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3aykhsect.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3tfojzvgj.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3xdxivqpz.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3sreimrje.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3kjuaebnc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ftshomaz.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3oxghwqha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ruvtnxku.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3rtimjzkg.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3tbdxqwpi.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3cfuuhwqb.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ewkxyiol.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3xtrlyovk.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3zbnfzasv.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3qnbcaeus.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3czpirgvl.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3dlsuuuvo.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3trjqpiwq.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3jjgontml.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3hvrutxxk.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3plgjgeum.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3eflcijnh.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3ttponkmi.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3ocgtkshd.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3vnfhiyfr.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3dcfroglc.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3acyqccpq.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3euhhyhvf.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3bjueacrj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3jqonxgzj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3xbptjvfp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3wbhigedf.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3rqssnzet.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3ybqsutpt.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3nydvqknb.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3pjmckprw.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3aojbdgch.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3awtmsxcp.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3vvrhqlui.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3dgfknxzt.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rpqjjrjh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vqqkegon.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3unokibwc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3woeolana.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3lpsfdcpz.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3dzimzblp.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3lpdtghon.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3xfcnxmts.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3hednctrv.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3nzkivxlo.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3alaftciv.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3vxgjfbvp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jzjrlhoj.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3cnpvkqbh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3tahrcrje.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3fnhaknfc.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3fnzedwyo.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3xolxkkuc.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3jompaaic.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3nptbmury.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3ybnkkmuf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qfgzyurk.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3dghekraa.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3zoejsypa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hwqvudlm.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3mwvsfysj.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3lgqpiuhk.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3vppmyvzo.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3erfosbxq.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3xxbczxqb.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3aqvscyuy.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3inhjzrwf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3agycndkv.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3sxthtdia.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3opnvzjvr.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3syqpkaun.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3hbbrviyu.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3vagzahkk.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3nfyiawkx.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3tdexagbd.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3ysxyxmsd.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3homfyyxw.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3tswwmmxa.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3dmlzhxpz.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3jbszonnn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3gwatpwpx.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3zjiwzqkh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3eqpbhlpx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3omiyqdny.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3mtdtalhi.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mfphllbj.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3ydoysogq.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3juqikjri.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yajwniiz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3tuucswdd.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3mzcnjqyt.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3uhcjnnul.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3tvlpksrq.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kifoaast.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3iqaaxjof.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3agtajbhz.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3syjowdrc.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3opbidwsz.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qiejctms.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tlwslzse.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3snkkonxz.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3pfbdfihs.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3wyownbmy.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ifokdept.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qfpvmgqi.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3kgmuwxra.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3crlmemfg.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3oicxtpsm.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3yumnnfmm.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3xujxpels.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3tesfynbo.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3uyokgswc.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3xtpnmbxf.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3pkxpisnm.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3xjgyontg.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3oxqbryjp.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3jglbnpyg.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3fzkpwzow.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3lxzlvqvk.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mildqygj.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3dgmxvvkj.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3zpujpbzz.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3njauqzib.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3pwuwwaqe.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3uawnkhfs.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3dktdmhzv.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3dniweubl.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3iumkdnpq.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dizeiiuu.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ijkxvepi.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vaxplqep.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3kqsnekbh.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3hrhrqdpz.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lvepbkbv.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3pswcwfqt.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3dvproeeu.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3twoagapi.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3dxivdian.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3fypbyxev.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3nxmktdid.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3lwzrmngh.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3reffpixl.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3xsejedew.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3odmqbkdm.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3iyoyzczp.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zatyjcqz.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jyenqzwv.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3nqcgcgrd.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dwejvsye.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3emrckrmk.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hzyqhuwp.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3acxvfpzg.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3oygboieu.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3vbyxztwt.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3wcbhgaik.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3omdypljg.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3kmorfvwe.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3vksrfrjz.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3fwehspdp.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3nclmgpjn.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3bgzgbplo.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3dzgypzbf.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3tptdmtqu.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3dstxthgj.html


<!-- 参考信息 -->