代发 wailian999

[U57] PHP：字符串插值
来源：http://wap.hesvh.cn/Article/details/gjblwgjcd.sHtML

"值: {$a}"
来源：http://baike.zdbjq.cn/Article/details/gzosumvoj.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fehbvm.com/Article/details/gonkfidpt.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.hesvh.cn/Article/details/gjzzqrvcs.sHtML

[U59] PHP：自定义排序
来源：http://m.share.hesvh.cn/Article/details/gugermuet.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gkajuznfv.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fehbvm.com/Article/details/ggrmfktzv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.zdbjq.cn/Article/details/grtkbdmzi.sHtML

[U61] PHP：正则
来源：http://www.share.zdbjq.cn/Article/details/gkkdmnmbr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/gtoirhxxy.sHtML

[U62] PHP：日期对象
来源：http://wap.fehbvm.com/Article/details/gzekewpuv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.hesvh.cn/Article/details/gwgrsyxyp.sHtML

[U63] PHP：文件读写
来源：http://3g.zdbjq.cn/Article/details/grarptvtn.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fehbvm.com/Article/details/gisssfznz.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fehbvm.com/Article/details/gcggizsuy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.zdbjq.cn/Article/details/gltncjygy.sHtML

[U65] PHP：会话
来源：http://www.share.fehbvm.com/Article/details/gsbgyczqg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fehbvm.com/Article/details/gkibdlypu.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fehbvm.com/Article/details/gpqpiymro.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.hesvh.cn/Article/details/gfqhxzsyt.sHtML

[U67] PHP：处理文件上传
来源：http://wap.hesvh.cn/Article/details/gdowsvoyp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.hesvh.cn/Article/details/gacpefptd.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.zdbjq.cn/Article/details/gwdookrli.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.hesvh.cn/Article/details/gasljjuyy.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.hesvh.cn/Article/details/gqmlzmpvy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fehbvm.com/Article/details/gibmqvpzz.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fehbvm.com/Article/details/gelttalhl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.zdbjq.cn/Article/details/gvomuqpkd.sHtML

[U71] PHP：抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gdcyfhnso.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.hesvh.cn/Article/details/gihtinfjk.sHtML

[U72] PHP：写错误日志
来源：http://wap.hesvh.cn/Article/details/gkkpsmeao.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.zdbjq.cn/Article/details/gcuyjnpmz.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.zdbjq.cn/Article/details/ghvtniszu.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fehbvm.com/Article/details/gegfmivwx.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gjovbdguw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.hesvh.cn/Article/details/gxqxqzcte.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fehbvm.com/Article/details/ghtmvqvpj.sHtML

composer require psr/container
来源：http://blog.hesvh.cn/Article/details/gmtjezcnc.sHtML

[U76] PHP：简单路由
来源：http://m.share.fehbvm.com/Article/details/gcbgbgbgc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fehbvm.com/Article/details/gxwfogszh.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.zdbjq.cn/Article/details/gtsqezale.sHtML

composer require twig/twig
来源：http://www.blog.zdbjq.cn/Article/details/gdkfcjptn.sHtML

[U78] PHP：单元测试
来源：http://wap.zdbjq.cn/Article/details/ggagreedj.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.zdbjq.cn/Article/details/glerzbcfl.sHtML

[U79] PHP：静态分析
来源：http://blog.hesvh.cn/Article/details/gnnlinjpc.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.hesvh.cn/Article/details/gwybayqul.sHtML

[U80] PHP：代码规范修复
来源：http://wap.zdbjq.cn/Article/details/gixekniod.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fehbvm.com/Article/details/gdfneixqa.sHtML

[U81] JS：初始化项目
来源：http://read.share.fehbvm.com/Article/details/gsoongfyh.sHtML

npm init -y;  npm i express
来源：http://m.share.zdbjq.cn/Article/details/gynwncbpy.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.hesvh.cn/Article/details/glxxdtxco.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.zdbjq.cn/Article/details/gmwgwmbic.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.zdbjq.cn/Article/details/glurenuro.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gzbafydxp.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.hesvh.cn/Article/details/gwdzdktpv.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.hesvh.cn/Article/details/gxifsnjdg.sHtML

[U85] JS：可选链
来源：http://3g.zdbjq.cn/Article/details/grfoawbyt.sHtML

a?.b?.c
来源：http://3g.zdbjq.cn/Article/details/gavcbbkey.sHtML

[U86] JS：空值合并
来源：http://www.blog.fehbvm.com/Article/details/gyonypdcj.sHtML

a ?? b
来源：http://mobile.zdbjq.cn/Article/details/gcpvcfwjq.sHtML

[U87] JS：解构默认值
来源：http://3g.hesvh.cn/Article/details/gdpfboyys.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fehbvm.com/Article/details/ggsvutmji.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fehbvm.com/Article/details/ghyzvtjnh.sHtML

{ ...a, ...b }
来源：http://www.blog.zdbjq.cn/Article/details/gqbbbiszr.sHtML

[U89] JS：数组去重
来源：http://baike.fehbvm.com/Article/details/grzgfyepl.sHtML

[...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gikfnbzal.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.zdbjq.cn/Article/details/gkhribkhc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gtdzewcer.sHtML

[U91] JS：对象键值遍历
来源：http://blog.hesvh.cn/Article/details/giemoojtr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.hesvh.cn/Article/details/gpfcdbmzs.sHtML

[U92] JS：深拷贝
来源：http://read.share.zdbjq.cn/Article/details/gswhsoryq.sHtML

structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gilfxvowz.sHtML

[U93] JS：模板字符串
来源：http://3g.fehbvm.com/Article/details/gjiblqzmq.sHtML

`共 ${n} 条`
来源：http://www.share.hesvh.cn/Article/details/gpciltqdh.sHtML

[U94] JS：箭头函数
来源：http://baike.fehbvm.com/Article/details/gdzbxmuoc.sHtML

const double = x => x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gngvevhjr.sHtML

[U95] JS：Promise 包装
来源：http://wap.zdbjq.cn/Article/details/gyqhaggft.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.zdbjq.cn/Article/details/glayxmmxj.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fehbvm.com/Article/details/gbjfyolmm.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gpqyyznyl.sHtML

[U97] JS：并发请求
来源：http://wap.hesvh.cn/Article/details/gviybuszo.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gyqghluzf.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gzndwpyon.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fehbvm.com/Article/details/ggnyumgpz.sHtML

[U99] JS：事件监听
来源：http://blog.zdbjq.cn/Article/details/ggrqrvsvs.sHtML

el.addEventListener("click", e => {})
来源：http://wap.zdbjq.cn/Article/details/gjlxnsvly.sHtML

[U100] JS：DOM 查询
来源：http://read.share.zdbjq.cn/Article/details/glumdtawq.sHtML

document.querySelector(".item")
来源：http://www.blog.fehbvm.com/Article/details/golerxnoe.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fehbvm.com/Article/details/grdelwyvx.sHtML

el.classList.toggle("active")
来源：http://www.m.share.zdbjq.cn/Article/details/gmlzxtczn.sHtML

[U102] JS：本地存储
来源：http://3g.hesvh.cn/Article/details/gcikhthnl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fehbvm.com/Article/details/gmoledwno.sHtML

[U103] JS：定时器
来源：http://wap.zdbjq.cn/Article/details/gjastwtrd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fehbvm.com/Article/details/gnvmaumak.sHtML

[U104] JS：防抖
来源：http://m.share.fehbvm.com/Article/details/gcbnasbdq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gaphepcwr.sHtML

[U105] JS：节流
来源：http://read.share.zdbjq.cn/Article/details/gujisoulr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.zdbjq.cn/Article/details/grtfiobaz.sHtML

[U106] JS：日期格式化
来源：http://3g.zdbjq.cn/Article/details/griclwque.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fehbvm.com/Article/details/gddbqcgph.sHtML

[U107] JS：数字千分位
来源：http://baike.fehbvm.com/Article/details/gwumlsqfi.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gfaxtqenr.sHtML

[U108] JS：随机整数
来源：http://blog.fehbvm.com/Article/details/gkoijbewd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.zdbjq.cn/Article/details/gdvyxlgux.sHtML

[U109] JS：数组分组
来源：http://m.share.hesvh.cn/Article/details/gmgpqzdtj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gadlxqfcx.sHtML

[U110] JS：数组分块
来源：http://mobile.fehbvm.com/Article/details/gftpkkolk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fehbvm.com/Article/details/gegkadbvo.sHtML

[U111] JS：对象转 Map
来源：http://wap.hesvh.cn/Article/details/gkwipmwcv.sHtML

new Map(Object.entries(obj))
来源：http://3g.zdbjq.cn/Article/details/gnsaxbybn.sHtML

[U112] JS：字符串补位
来源：http://www.blog.hesvh.cn/Article/details/glllgyaxz.sHtML

"7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gaehnskfl.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.zdbjq.cn/Article/details/govexeglw.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gmoaruuao.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.hesvh.cn/Article/details/grxvsbswr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gylfkbyxj.sHtML

[U115] JS：生成 UUID
来源：http://www.share.hesvh.cn/Article/details/ggqjmdywa.sHtML

crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gdzqnkjgv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.hesvh.cn/Article/details/gupzryhlv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fehbvm.com/Article/details/gaovgcfir.sHtML

[U117] JS：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gokcywxen.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.hesvh.cn/Article/details/gmbyghdpi.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gizqztwsb.sHtML

npm i -D vite;  npx vite
来源：http://mobile.hesvh.cn/Article/details/gkmteltqb.sHtML

[U119] JS：生产构建
来源：http://wap.zdbjq.cn/Article/details/gwhcoikgw.sHtML

npx vite build
来源：http://www.blog.hesvh.cn/Article/details/gsjrwqiqt.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.hesvh.cn/Article/details/gleugnubk.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.zdbjq.cn/Article/details/gtisazyso.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkzgdqypf.sHtML

统计汇总
来源：http://3g.hesvh.cn/Article/details/gxrsklysf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gyzlzhwzb.sHtML

按语言统计（条）：
来源：http://blog.zdbjq.cn/Article/details/gedsvarkw.sHtML

Python ......... 252
来源：http://m.share.hesvh.cn/Article/details/gvlggchrx.sHtML

PHP ............ 252
来源：http://wap.hesvh.cn/Article/details/grwaishlp.sHtML

JavaScript ..... 252
来源：http://www.share.zdbjq.cn/Article/details/gacaimovm.sHtML

TypeScript ..... 212
来源：http://www.blog.hesvh.cn/Article/details/gouqpyhkj.sHtML

Java ........... 212
来源：http://3g.zdbjq.cn/Article/details/gbyfnnorq.sHtML

Go ............. 212
来源：http://read.share.fehbvm.com/Article/details/gvcahlcxa.sHtML

Ruby ........... 212
来源：http://3g.fehbvm.com/Article/details/gcauqazfz.sHtML

C# ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/ggprordjd.sHtML

C .............. 30
来源：http://3g.fehbvm.com/Article/details/gbboawtie.sHtML

C++ ............ 30
来源：http://3g.zdbjq.cn/Article/details/ggdnxnsdo.sHtML

SQL ............ 90
来源：http://mobile.fehbvm.com/Article/details/gainxhzfi.sHtML

Bash ........... 80
来源：http://baike.fehbvm.com/Article/details/gbovhbqjd.sHtML

Kotlin ......... 15
来源：http://read.share.zdbjq.cn/Article/details/gugjjqofc.sHtML

Swift .......... 15
来源：http://blog.fehbvm.com/Article/details/gevvrrnwr.sHtML

Lua ............ 10
来源：http://www.m.share.fehbvm.com/Article/details/gcoshhwfn.sHtML

Perl ........... 10
来源：http://www.blog.zdbjq.cn/Article/details/glemjwzof.sHtML

Scala .......... 10
来源：http://baike.fehbvm.com/Article/details/glbdbaeco.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/gqcrlcvha.sHtML

合计 ........... 2106 条
来源：http://www.blog.hesvh.cn/Article/details/gyufseryk.sHtML

按章节统计：
来源：http://read.share.zdbjq.cn/Article/details/gzbjsbkok.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/grnbmprrj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gbaacigok.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gskmlmooa.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gxqpkdtfs.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.hesvh.cn/Article/details/glmsfhtda.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gpsruwzhb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/ggxgvihis.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/goxqmkvjv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gnszjwklo.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/gcetarerz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gzyhmiqar.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gaezucdhb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gzhgqwwpq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/gvxjquupe.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.zdbjq.cn/Article/details/gdidiagto.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/geatttesa.sHtML

Q SQL 专题                              90
来源：http://www.share.zdbjq.cn/Article/details/gtgynaons.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/glpwjemdq.sHtML

S C / C++ 专题                          60
来源：http://baike.zdbjq.cn/Article/details/gaehcwezx.sHtML

T 其他语言补充                          60
来源：http://baike.zdbjq.cn/Article/details/glehyizrr.sHtML

U 高频实用片段                         120
来源：http://www.blog.fehbvm.com/Article/details/gwxevxdbj.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gnqyjiigh.sHtML

合计                                  2106 条
来源：http://m.share.hesvh.cn/Article/details/gvqnzonyk.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/ggtotcybh.sHtML

使用提醒
来源：http://wap.zdbjq.cn/Article/details/gwjyvbxjz.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/geaqiuoya.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.hesvh.cn/Article/details/glhoigwvl.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fehbvm.com/Article/details/gcgntlmkx.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.hesvh.cn/Article/details/gmlxodiqj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fehbvm.com/Article/details/gpegilghx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.hesvh.cn/Article/details/gumcrlwey.sHtML

—— 文件结束 ——
来源：http://blog.hesvh.cn/Article/details/gkkjjclsi.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gntmmpcdl.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.hesvh.cn/Article/details/gckfcpgkg.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.zdbjq.cn/Article/details/gmteermqb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbjtlkmrg.sHtML

【收录内容】
来源：http://www.share.zdbjq.cn/Article/details/glgsocvqv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.hesvh.cn/Article/details/gcmqqqiqk.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.zdbjq.cn/Article/details/gzupmsaoy.sHtML

SQL · Bash · C · C++
来源：http://3g.fehbvm.com/Article/details/gxbptpukf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.zdbjq.cn/Article/details/gxxowotgm.sHtML

【使用说明】
来源：http://wap.hesvh.cn/Article/details/grpnagebd.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.hesvh.cn/Article/details/ggcahojsx.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.zdbjq.cn/Article/details/gjhyskaff.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.zdbjq.cn/Article/details/gvvjipwgz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fehbvm.com/Article/details/gvkghevgz.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.hesvh.cn/Article/details/grtokvoiy.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.fehbvm.com/Article/details/gqhwezsjy.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.fehbvm.com/Article/details/gdcostcrj.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.hesvh.cn/Article/details/gijuadixq.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.zdbjq.cn/Article/details/gvqmjhlik.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.zdbjq.cn/Article/details/gljoepcob.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.zdbjq.cn/Article/details/gmazbugog.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.zdbjq.cn/Article/details/gfiozmgut.sHtML

【文件统计】
来源：http://www.blog.hesvh.cn/Article/details/gabmusseo.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.zdbjq.cn/Article/details/gpvrctxrm.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gzxvfbjqb.sHtML

目  录
来源：http://www.share.hesvh.cn/Article/details/gyidtoefq.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/grknskibz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/gvdcvppik.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gzdcqzfgq.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gbllecpor.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/gjabzrvec.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.fehbvm.com/Article/details/gtkazvxgz.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gcegitgjq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/giwrgzprm.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/gxoweurcr.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gxkbomlop.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/grxiyybdp.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/ggllyycox.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/govctgmrx.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gemwqsquq.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/gssxndigd.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.fehbvm.com/Article/details/gthluccnd.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gfhzzneoa.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.hesvh.cn/Article/details/gqcgimart.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.zdbjq.cn/Article/details/geesrveer.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.hesvh.cn/Article/details/gpnvdgcwi.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gmfhkjyaw.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/gpdjcnvvs.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gewkfryne.sHtML

A. 基础语法与类型
来源：http://read.share.hesvh.cn/Article/details/gcrzoohqt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glxlydqhk.sHtML

[A01] Hello World
来源：http://read.share.fehbvm.com/Article/details/gvmghsbuy.sHtML

Py:   print("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/ggltwrbaq.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.hesvh.cn/Article/details/gvaouoniq.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gvleacfgi.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.fehbvm.com/Article/details/gxbywksfg.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gaxnvdrly.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.zdbjq.cn/Article/details/gpmpqcksi.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.fehbvm.com/Article/details/gwesnwdkp.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gykieaipt.sHtML

[A02] 变量声明与赋值
来源：http://www.share.fehbvm.com/Article/details/gijeqzvpi.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.hesvh.cn/Article/details/gcevmkelo.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gsmzixzcb.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/grpunbmqw.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.fehbvm.com/Article/details/guhllrfih.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/grczjanug.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.zdbjq.cn/Article/details/gznkhivip.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.fehbvm.com/Article/details/gavuubkyn.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/gjppykajy.sHtML

[A03] 常量定义
来源：http://www.m.share.hesvh.cn/Article/details/gywvtkjpj.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.hesvh.cn/Article/details/glbrznblo.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gqusvqvak.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gakpcfwmv.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gjogrnrhz.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gdwkaggbg.sHtML

Go:   const PI = 3.14159
来源：http://baike.zdbjq.cn/Article/details/gvcleokqp.sHtML

Ruby: PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/gbfpjknjd.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gpilfaott.sHtML

[A04] 判断变量类型
来源：http://www.blog.fehbvm.com/Article/details/gqckqwmxh.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.fehbvm.com/Article/details/gfoejlhud.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.hesvh.cn/Article/details/ghczbulcg.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.fehbvm.com/Article/details/gikqaqvqw.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/gcnfndipa.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.zdbjq.cn/Article/details/gvvyhbrle.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.hesvh.cn/Article/details/gcstoaukk.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.hesvh.cn/Article/details/gjcdwlbjx.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.zdbjq.cn/Article/details/geomjsqfj.sHtML

[A05] 整数除法与取模
来源：http://3g.fehbvm.com/Article/details/gfrwypxbo.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.hesvh.cn/Article/details/gmpuspyrs.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gpgjetldr.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gutfbtzlu.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/grkbcbnkj.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gksfuonzo.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gcxrcmfko.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gnrgnhdks.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gdxefryjc.sHtML

[A06] 字符串转数字
来源：http://wap.hesvh.cn/Article/details/grmfonbne.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.hesvh.cn/Article/details/gcjcnkzkv.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.fehbvm.com/Article/details/gatturjca.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.fehbvm.com/Article/details/gcsozrpul.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.hesvh.cn/Article/details/guqsanlso.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.fehbvm.com/Article/details/grklbbuvy.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.zdbjq.cn/Article/details/gevonffwz.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.fehbvm.com/Article/details/ggtywpmwu.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.zdbjq.cn/Article/details/gbjbluaeo.sHtML

[A07] 数字转字符串
来源：http://read.share.fehbvm.com/Article/details/gvowizxdy.sHtML

Py:   str(42)
来源：http://wap.fehbvm.com/Article/details/goatsjaxq.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.fehbvm.com/Article/details/gdqixlken.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.fehbvm.com/Article/details/guvrjrzht.sHtML

TS:   String(42)
来源：http://3g.hesvh.cn/Article/details/gndiupjsc.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.zdbjq.cn/Article/details/gcmhgtyyc.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.hesvh.cn/Article/details/gikurshpy.sHtML

Ruby: 42.to_s
来源：http://www.m.share.zdbjq.cn/Article/details/glvlmbbbu.sHtML

C#:   42.ToString()
来源：http://wap.zdbjq.cn/Article/details/goplivydi.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.zdbjq.cn/Article/details/godbhsseu.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gazeywlwo.sHtML


<!-- 参考信息 -->