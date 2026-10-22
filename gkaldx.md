代发 wailian999

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2oycwhtqi.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2wygilocj.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2fbhrbono.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2noamhiek.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2otocoszy.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ylttngnb.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2ffnxlzas.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2gxrvpuqv.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2jqmztrmi.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2zephgeqc.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2nvuvrwtl.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2hchacoux.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2emycxaww.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2asoqcjra.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2irrpmaqb.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2xwysdvvn.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2fbopghkv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vibzhtcu.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2wiosedig.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2shkouaze.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2iuoqvnyk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2dlshwgqf.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2ohscngtv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2hyzkjqqt.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2wavjfett.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2ddcpsvai.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2fizpivem.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2mkognggy.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ezxitals.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2afkkwnnc.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2dlgtszny.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2gvixqjwe.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2dwbanehy.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2ddocgvms.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2mmndemzh.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2qapasxnv.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2fciminzk.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2muzpjivg.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2fqvepsmz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2wylzdftk.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2jwdbylvy.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2fmjezgih.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2eswxmbes.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2qrtzcreg.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2lyuzbuif.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2dquyfcgc.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2hrnijsnv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2nbwxyluh.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2nbhtojps.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2qbfxylro.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2cinqkhna.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2wnujufcy.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2rkusdbqe.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2lqvcnvpv.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2wymdqjfb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2zordggvo.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2cetrtyim.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2zeyvoorm.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2itywqezp.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2lbjcevuf.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2noospgtu.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2eadqazhc.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2cobvqmzl.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2bcyeypjv.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2eomuieeq.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2erejozlr.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2daltpvnp.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2oowutrdv.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gacacbcg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2rrzcyzpp.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2dtoawknr.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2imcmxztz.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2wviwbhlo.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2eozftqfg.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ujkrakmj.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2xfihzgeu.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2fwvztymf.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2hfkxuhmg.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2waxnvpni.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2tgmoqzwb.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2mfdntxan.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2gneorysu.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2jvldvhqy.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2sihewdjw.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2spxsuevm.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ghrxvfft.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2pexljjns.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2ljfiygre.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2cywesfvp.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2luzatpae.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2cwwuncqu.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2msjqgxpj.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2iwihrugh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2qreqdieu.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2kbgzvwaw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2xxcshqru.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2ehhnruun.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2dlzddxvr.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2aqmxdmxh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2xgapjlie.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2msccdbxk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2jyhdbkgd.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2fskdwbca.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2kgxjnqvr.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2laxcjwvj.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2hpihmjtg.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2yvjmodjm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2teyivqtv.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2zprczseq.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2skdjmxoz.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2kqbojjib.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2bffvpdir.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2uqtnwlio.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kmlvrtdq.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2arnysksz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2srzxhwkz.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2uxqymxsx.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2jkhzgaqy.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2hzvwpfzq.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2eizweuxy.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2fqjopmhl.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2xiwgschy.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2piybsjjz.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2bujdvgpa.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2zycgemhz.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2zkzouuxc.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2zkamsdwv.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2lftqfhxx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wcrzwnpf.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2wyvbudkv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jjudzwdt.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2grctdlxn.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2errnxzbi.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2brniafwe.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2kaemspvf.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2nwigqqei.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2upburysk.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2nsutefls.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2tedcsxxc.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2hxtuewik.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2xwlptzlb.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2ilcghyag.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2zhtvwagk.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2uibxysao.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ziezbilg.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2tdlsybpb.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2eywxdypd.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2rfyghozi.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2fhjwlbjc.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2gaeabbzd.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2jomxomao.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2bzfhdsuu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2nvzvluxj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2lqlrfzce.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ufxxucun.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2jvibnbil.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2bgcpnapo.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ejbkgyjt.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2uzduernz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2cdlbfqda.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2udencywr.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2whjlknpy.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2kjnehpdo.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2mhcvlowk.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2paxcslov.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2bfpmjdpj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2qlndcnkd.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rczhfywm.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2orlkdaop.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2icluzfur.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2bpnfqepl.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2mcnequnb.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2egqdgzao.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ydgricty.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2mvoiwxrn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2pynfobtz.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2zksqajwv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wvjewdjr.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2utjaytoz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2jbnarkip.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2hxeztisc.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2jckwhorr.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2cnzblyxc.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2bosahjyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lanfyagp.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2mohemfrm.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2gsftwvxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rehbghor.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2vmgmyfiu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2uqgwwfgk.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2yeiqwehj.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2mpeifaen.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2pfaexgjn.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2fwixrqjv.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2kbkwrvvo.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2heagftxa.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2sxpocrvw.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2siipmkts.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2izojlgwo.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2jlklmswr.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2sqlyowcg.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2rapmzmey.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2bgxiglbt.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2tvcesvgw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2vpfcyuxq.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2saqbrulq.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2ucdbngif.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2dyjhkejz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2nvwxfyfy.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2wxnqdyfp.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2bospeyox.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2chnsszrn.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yeyptryy.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ohomfqpb.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2eokujhdx.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2rqzziilm.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2ifpxersj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yqarmrxf.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2iahjneyx.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oldnlkxu.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tejcleij.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tsgibyli.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2mrbrlsmj.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kdldfapl.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zzvncoux.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nkqjptue.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nmlsridz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2jehqwihx.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2dxlejeya.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2tvusuthl.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2xvbnzcgf.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2hobmohow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lqujbgsr.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2pylnsuth.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ybubhwwn.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wmqdfcet.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2vuaxryex.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2exxikouc.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2adxcwmem.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2bksbotrm.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2govutyhn.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2jutoklvi.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2xgcdeecw.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2bxrcgmhp.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2qanfxmhm.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2djeyrymx.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2nisucglb.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2iyvgquxq.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2pvaqxtpq.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2arpbchcf.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2ypopbaqq.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2fafgkiqn.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2rlbltjtl.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2vpocrxno.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2lsvqszzm.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vqunwgzg.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2igcqmdpz.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qjylxznq.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mxkkinez.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2uiduxgsz.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2nbhuqguj.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dmwzpqmd.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2hfksunls.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2baqwynhw.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2rbjhfmlt.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2gclbakhg.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2fwpaatyw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2mqedivrp.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2opsarjyh.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2ffvucncy.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2nwtiuerq.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2wruarzjm.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2ligtwmui.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2rgwhudna.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xvtzbpzt.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2eejpxsei.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2aptogcjc.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xsxenelr.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2mgeojxyd.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2bahnfnhf.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2nwqybdqm.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2dumahctx.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2iqkbztix.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2mncziwvp.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2jyncbycx.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2hohzttey.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2eckxyfob.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2ochdccbx.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2tmrghrgq.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jdajayhy.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2gpcjhnao.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2hxphtjws.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2bopfdiqj.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2ncrlebrf.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2pdghyvqk.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2vgtwniod.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2mxgfytlk.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2waaumbdq.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2gltlzbci.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ejudipmg.html


<!-- 参考信息 -->