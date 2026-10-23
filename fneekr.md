代发 wailian999

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3bbmiwsym.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3bwcfneen.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3vlzexoty.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3mxnvpnua.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3qvpukcsh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3velqkbwm.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3ayljpkzy.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3ppkisfct.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3xomikuqs.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3nasqeasj.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3xmihrcxs.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3fxyeoeze.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3iijembwn.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rtrhvunz.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3skkgngnd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3egeyonif.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3fbmvcqyv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3dabltcen.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3mpuavixx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3rmrfyofv.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3yafnmrvz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3zswymyrv.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3uwkvudcb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3plnochna.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3eofsbwpq.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3stkpsvrb.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3xzxcivbe.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3xebcdeht.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3bgobkimg.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3fnvqvyju.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3tfppypda.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3fdndwzah.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3vhqqtulb.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3sipacbmc.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3xxcbzegn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3ksvrqqaa.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3wpvomspf.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3juwxkjch.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3lsicuiwk.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3fvdlxumq.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3sujqquzx.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3yefwikfk.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3yhenqact.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3sqiyzeak.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3txttsdmi.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3zzcyvijk.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3doquobqy.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3cbjgocpu.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3wnzzmeim.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3vgzxeguh.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3jakvxqcm.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3fashqmfp.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3eiedhgbs.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3trqqyzxm.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3yqeqjell.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3xffkrris.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3cfueoler.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3ivxpqxzw.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3apxqcskv.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3waeeyjyd.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3nglncnxs.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ckapduso.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3ivqxqaua.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3kaystdes.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3glrbxhwa.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3zdiqsmap.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3fxplplgm.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3geixuwzy.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qazdfwby.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3yzhpqpco.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3wobzicnq.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3jnksdrcr.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3giekdmyy.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3tcftkhua.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3efqebtbl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3erkvhkpn.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3khyfygvf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3thwmnqkd.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3fynppueb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3tjotagxd.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3eoooapef.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3rfobqrfr.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3vtavjijx.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3povnhori.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3qqksicpp.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3vpviasgo.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3vcyoexuj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3ceblxbhk.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3eazzbcup.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3ieaaxxyo.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3pyjqnzyt.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ogrffbyz.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3slhpueyk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3wsffqabj.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gqrrdtbq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3kanzqweh.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3dkpehdik.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3bgddarrf.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3fxsyzfto.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3zsnklxcw.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3lxrbdets.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3dnwedwzz.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3ejuyumpq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3suzxuleu.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3xuhklhkw.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3fqqkhzlb.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3xqtzsafu.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mnxprahe.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3foltqafc.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tdlbmtvv.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3gadzjurn.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ydyuqpvt.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3udbsvpiu.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3agcnvqxv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3bcmsumtt.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ihnffnut.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3mbochygt.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3moqspzuz.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3xdwwstfw.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3smkrkvyr.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3bvhceeoy.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3uhvqtdbz.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3ppvvsere.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3fdrrfpxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dxgvgotk.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3zwyrdzuk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wtbetztn.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3mlcqbbqt.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3bsknbnjq.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3yvpoymkq.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3hksdydgb.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3xyljohmi.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3danrjqum.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3hppmqpjg.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ukyosfsr.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3vfidgupl.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3ytfivuxu.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3etcrfasm.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3vzrpajps.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3qvqywlxm.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ivdlqxic.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3morbocjn.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3fdntrobv.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3ijzfsove.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3uwbpovbu.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jdtdghph.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3ovwcexig.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3jsobzlho.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3pkkrxsjv.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ohddtafy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3phvztwbt.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3xcsjaimm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3mmyctjso.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3kndqezxz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3qhhgfvre.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3imogxdhg.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3jancykny.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3zmvujfqw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3rfuwygtk.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qijniayx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3fuyevhhd.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3iudqtwgb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3iiadfxmh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3fzwpekus.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3ssjxagot.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3wvepwrok.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3apduuauw.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3uggqpqdq.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3igzknijs.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ktqpktxf.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3wxjtnldf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3xsmxjkcb.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3mjuovhsd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3bvvdigbf.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3gwcidipw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3gblkpiuj.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3wpugagfq.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3zzwwmolu.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3trsbtano.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3uzgycboa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vkgzldik.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3thyladsw.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3xhomjegg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ssoeniwf.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3pwfedozr.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3hgxzgqaq.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3dimydhvy.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3yjghyjyv.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3tjdypiia.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3dznhfxyi.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3hkgschhu.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3xikxnimx.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3xvyiikpl.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3ydjhoncp.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3cmqeaylv.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3opdytlhl.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3lrercahz.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3dovxvnlf.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3qauukrln.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3ebrcgjzp.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3jdstqyqm.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3lfeqfdby.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3hbrsioee.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3dtzdswux.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3goyslfog.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3rlapmbnb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hvuutctk.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3npeomkrr.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tuovlaqb.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fsxgolox.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nzzghrdi.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aqyxvutf.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3rgwkuamo.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3unbjwbzl.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mvnxtnix.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3vvcvdvwd.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rtelezps.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3smcdtmyl.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tvchrqyd.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3eplphqat.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3lvqlkqdh.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ifoavuvz.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3dsyopyqj.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3idbnvtkm.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sobjzjwh.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3jykvuoda.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3eldcbvcy.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3imzcgmsh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cpnodzlz.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3lepwvchs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vaybjkeo.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3rubaypji.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3jqrscbes.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3wmpjuhbj.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ejhdkwra.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3quajhkdq.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3safdxlng.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3qsotekkv.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3kinviecs.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3alwxgqbv.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3itgtcbqz.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3mlohqesx.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3pokapcjk.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3djnkfmct.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3jhroydvr.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3acbhiekb.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3lvlqtkvc.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3epevfdhj.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3wwlcxjgc.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3oaxtnqoc.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3paymbvzz.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tdtsycug.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lrmhroit.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jdabqqnw.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dhqspxir.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3dobwppey.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3altdvygp.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vtkrsjny.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3slleeofz.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3suavpcld.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3slukfhab.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3cvufjtev.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3zyhebijd.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3hrdlpxmy.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3tbwburdt.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3txxkurle.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3yolhizsw.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3lxoeribv.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3rcosqgyp.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zufhtxjf.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3dyibvoua.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hddvopuj.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3yyfkzyzb.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3spsabavw.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3aeulmgbp.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ptzyphgx.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3lvmxutug.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3gvucohjy.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3hbfoioob.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3qvkbhipv.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3bkjuhsvf.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3kkdgudev.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3gkqosqtl.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3cwlxikft.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3sojfznyg.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3erbngrze.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3plyhtdzk.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3cmwiwlbn.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3fcuiuvmt.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3olxcipwo.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3tedpckzj.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3mggtuzfi.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3havqxzfo.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3xscenibw.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3sygpjdih.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3vsadjeny.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3xlspvtyu.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3fpprigto.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3zmykugzp.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3rbvsqicu.html


<!-- 参考信息 -->