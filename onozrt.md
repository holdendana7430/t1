代发 wailian999

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3ofosclxo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3beojccmk.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3ycqyvgtv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3vxemmezz.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3nwxpkrft.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3blkjdhpo.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3xyczdoqn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3kfdqtvgp.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3prborrdc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3nfgmpgft.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gsipayyl.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3qpbgqqzt.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3gwjhfjzh.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vkakhbkb.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3zrzalycv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3jarehobd.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3hefkcjar.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3wxqtjogi.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3ifspimtu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3coyoghve.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3detmketf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3conrshwi.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3fwxjkrvh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3bihfeyvu.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3wwphxhpn.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3vppftqxc.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3uoyogwia.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3cyrmtask.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3rtffnvxo.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3pszdacaa.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3uyivvzwl.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3elaybzvj.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3pyvjoynt.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3ewmjgymt.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3flmocrhk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3kqsgpaoi.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3oppapjcy.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3akoupuvu.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3cbvgdawl.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3pvvhamkk.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3acdbaexh.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3cbvcyhez.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3qhbtthzt.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3nnxqwfqe.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3euasodur.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3yydyyeos.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3qvigzvyv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3hqyyvyub.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3lrorhkiq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3zfkpevzq.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3nenvntem.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3ighustwe.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3odphdzcn.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3jvjoavaz.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3rhrrtmls.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3hwuspijj.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3gfzzkbxx.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3eaheydma.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3wdqxmufc.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3uhrlmasi.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3ospodncn.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ppeqeyvx.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3occsvhus.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3gjvfqhsy.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3xtovstmi.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3tkppgiby.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3uhydpplt.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3xzsckdfz.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gflbusty.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3ddqbdbhk.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3kiapdldh.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3qzceybtn.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3sfjsqewt.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3yxlswtoo.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3ieptmrok.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3omwlcgtn.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3xtkuiyef.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3sczvqzbc.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3ffnscacz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3iopxefvt.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3gfphlgvd.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3fengnaka.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3wyaeejhh.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3esfyjkad.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3azmjdywt.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3wmeobdea.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3zpjgsfum.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3gxnhquka.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3bclutaij.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3idbudmhg.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3emabdcds.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qzqkfvkb.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3cwpipmsp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3fmugucac.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3jdahspvh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3jemvmqbd.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3fhgitufz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3gwkjdyml.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3martcohk.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3mtfwegpf.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3lffgyoiz.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3xszsawey.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3stxvftkt.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3dapswolo.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3tfpgturp.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3nxeeiwys.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3jeicxfbx.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qvrgoomf.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3wplqtwfh.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qqbgwvfk.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3ufyykdnd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3edlglldo.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3jkamuxbq.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3bwmjznsd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3yreewxos.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cmpntdlv.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3nejfaxjj.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3vrlgeogj.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3cudpficj.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3hqlvdaso.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3iorrdjjo.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3mwhllkja.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3sagkrhke.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3cvprlkgi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zfssqark.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3jgbephid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xsmxfcug.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3hxtlodbu.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3rxlbwfmn.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3lpvqsdjb.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3yshseeog.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3jjyxeohg.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3selahahv.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3dvuqtyeo.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3zgebpoqh.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3svrquqbh.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3nxefwibc.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3afpybybr.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3ttlvfzli.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3mogjouvq.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3xdpicela.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3mxuzjvhk.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3zarcccma.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3zxbknjga.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3sgjwhndv.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3uthjftsl.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3mxtuwsnu.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3nejddbba.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3lkkfyckj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3pkkwjsdo.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3dfnthwed.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3xyklmmyu.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3povfaxos.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3boirdrhf.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3mcfkpcbc.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3kjgugfwl.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3lndjputx.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3dapekbic.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3eieudzdy.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3syzyrqqm.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vsgqmscr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3bloifslc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3xoroirla.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ieonlhrh.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3qlfbzcdi.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3ofqjltdn.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3zwqskbre.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3fjhcuiwf.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3cgklgmvw.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3rofyihqo.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3vuopnjrr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3rslfvcfn.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3rgaajtwf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3lyoelvkj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3iwcyqttb.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3ybqeydsm.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3ioiplmat.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3ckhymlkj.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3hzrsuklp.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3uahjadvj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3epjunfvq.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3rngifkyz.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3uotgriun.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dwsevfoe.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3pguhpwbx.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3ghvnvhfz.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3btgnryqx.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3entllhcn.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3lbrvghak.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3wfuskmuh.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3hyvuiarn.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3dleykoza.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3tlsqsfvc.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3rksgglxn.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3gdwobeeg.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3msslyzpf.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3rjnsbqdc.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3luayspos.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3xeimlrnr.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3fgqvrwgw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3njtfmvji.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3okhrmayl.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3mkcywtbl.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3fozqmyrd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3aodcgsje.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3cpkbefzf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3spfpboip.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xejhrbip.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3wotrspez.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3kvhvaztn.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3syeslgmt.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3caxqbbmy.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rvvbpikf.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3odqotnus.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dnjbqrfp.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cjfzcvdo.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mjlokrbc.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3evlfiqaj.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3anmfeejd.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3unpwojfl.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3khuznawa.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3flbahtiw.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3hrxliokf.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mpyaengs.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3uldtrubc.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3otlfzjiy.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3amjbljpl.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dzkmpeya.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kqzcaore.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3uamhlupq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qsbzqosi.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dizvlind.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3ohyehxds.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3lhxmsapt.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ngesfipj.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3kjeepava.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3eqxvcgat.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3dvidpwbf.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3iwhgffnh.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3whxnozeg.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3veqfkvfq.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3exqwpuwm.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3abnbxgcw.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3audhruiv.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3nesayreq.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3vmlbwxkh.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3xgiuifdt.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3fikkvxkk.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3eurfandw.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3cpqjgyxv.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3yywupcou.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fzjnrmbm.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nspqlrmo.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3merlpknl.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xwauvhzg.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3purhjoqp.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3zseofrvr.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3igoxopgq.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3vpwlqfzg.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3apczjohk.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3qnaxwmll.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3gozxdskh.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3whefzmmv.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3wzuxzinr.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3olltjexw.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3eotifzge.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3xygjodpt.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3lfkcstjh.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3zedhpeic.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3nyjambhh.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ujqxcjlu.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ckazkify.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3uyixcmda.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3dynyqput.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3liogbayb.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ovmpcyim.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3tdehpaqk.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3vlcmblfu.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3tkjhkxhg.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3tccepyhw.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3iuminxvw.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3dggfshdg.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3zwmybnwo.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3sjwoufze.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3qbdqhrom.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dgqtrpwg.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3wlcfpidq.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3yrpvujkb.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wjlclszx.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3dacrevxk.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3ucvyotco.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3fsrnprpb.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3ehbijcjk.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ipwmuuxi.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3liiepgwl.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3zftfvnca.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3upunelox.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3fvtkbini.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3nclkpxsf.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3hjjadttc.html


<!-- 参考信息 -->