代发 wailian999

[U63] PHP：文件读写
来源：http://read.share.hesvh.cn/Article/details/glqoychqt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.zdbjq.cn/Article/details/gujseoyuu.sHtML

[U64] PHP：目录遍历
来源：http://read.share.zdbjq.cn/Article/details/gjiwtffbf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.zdbjq.cn/Article/details/gkgqkbsii.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/gdfazdood.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gcywcfmws.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.hesvh.cn/Article/details/gyfhecnoy.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.zdbjq.cn/Article/details/gfctdnxxb.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.hesvh.cn/Article/details/gfnzmqpxt.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.hesvh.cn/Article/details/gpibviviy.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.zdbjq.cn/Article/details/gacpucund.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fehbvm.com/Article/details/gyikehjmo.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.hesvh.cn/Article/details/gweyyhzsa.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.zdbjq.cn/Article/details/gtelelnia.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gyfsehrrx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fehbvm.com/Article/details/gobblmwlg.sHtML

[U71] PHP：抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gtizjmnrb.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fehbvm.com/Article/details/ghocnprka.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fehbvm.com/Article/details/grucqbbxn.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.hesvh.cn/Article/details/gicoiyocq.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.zdbjq.cn/Article/details/grlilhvmj.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.zdbjq.cn/Article/details/gubppbwfk.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gjskmboei.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fehbvm.com/Article/details/gwccmmlqt.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.zdbjq.cn/Article/details/gwjaecxsq.sHtML

composer require psr/container
来源：http://read.share.fehbvm.com/Article/details/geumtqylb.sHtML

[U76] PHP：简单路由
来源：http://mobile.hesvh.cn/Article/details/ggmvdlvsp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.zdbjq.cn/Article/details/ghmfmjven.sHtML

[U77] PHP：模板渲染
来源：http://mobile.hesvh.cn/Article/details/gajwhzeuj.sHtML

composer require twig/twig
来源：http://3g.zdbjq.cn/Article/details/gndqkczkq.sHtML

[U78] PHP：单元测试
来源：http://wap.zdbjq.cn/Article/details/glmghpano.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.hesvh.cn/Article/details/gqttdqjbb.sHtML

[U79] PHP：静态分析
来源：http://3g.zdbjq.cn/Article/details/gyqmwouhl.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fehbvm.com/Article/details/gxtpburlq.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fehbvm.com/Article/details/gtucrjrib.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fehbvm.com/Article/details/gtmeaqqmt.sHtML

[U81] JS：初始化项目
来源：http://3g.zdbjq.cn/Article/details/gvruupwnz.sHtML

npm init -y;  npm i express
来源：http://mobile.zdbjq.cn/Article/details/gipcdtqwt.sHtML

[U82] JS：package.json 脚本
来源：http://3g.hesvh.cn/Article/details/giiutbcnq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.hesvh.cn/Article/details/ginwipwwc.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fehbvm.com/Article/details/gpltegjof.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gefeovspd.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.hesvh.cn/Article/details/gwauubwlu.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fehbvm.com/Article/details/glitxpxqn.sHtML

[U85] JS：可选链
来源：http://blog.fehbvm.com/Article/details/gqwgzxnec.sHtML

a?.b?.c
来源：http://blog.zdbjq.cn/Article/details/ghjvskwio.sHtML

[U86] JS：空值合并
来源：http://read.share.hesvh.cn/Article/details/gsiqqcwfv.sHtML

a ?? b
来源：http://www.share.hesvh.cn/Article/details/gcliaarfd.sHtML

[U87] JS：解构默认值
来源：http://m.share.hesvh.cn/Article/details/gglkbkuxs.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.hesvh.cn/Article/details/gcsrwilga.sHtML

[U88] JS：对象展开合并
来源：http://blog.fehbvm.com/Article/details/gtvtmwpcw.sHtML

{ ...a, ...b }
来源：http://m.share.zdbjq.cn/Article/details/gajlvjava.sHtML

[U89] JS：数组去重
来源：http://mobile.zdbjq.cn/Article/details/gcfgdjiti.sHtML

[...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/ggcsvmjgy.sHtML

[U90] JS：数字数组排序
来源：http://m.share.zdbjq.cn/Article/details/galszhacq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gxvmrcuvg.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fehbvm.com/Article/details/gsehkskkd.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fehbvm.com/Article/details/gppviklrv.sHtML

[U92] JS：深拷贝
来源：http://www.blog.hesvh.cn/Article/details/gyazghbea.sHtML

structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/glohqloai.sHtML

[U93] JS：模板字符串
来源：http://wap.zdbjq.cn/Article/details/gntgexjhq.sHtML

`共 ${n} 条`
来源：http://blog.zdbjq.cn/Article/details/gkiiwxgdu.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gqvsnpjnu.sHtML

const double = x => x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gtnvkoqvm.sHtML

[U95] JS：Promise 包装
来源：http://read.share.hesvh.cn/Article/details/gmxehdagf.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fehbvm.com/Article/details/gnaqvlrxw.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.zdbjq.cn/Article/details/gqvkhykdt.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gdbvwoymt.sHtML

[U97] JS：并发请求
来源：http://3g.fehbvm.com/Article/details/gpjhxulhj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gjpqvmbvk.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gszkbdhtd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.zdbjq.cn/Article/details/grkggkhla.sHtML

[U99] JS：事件监听
来源：http://3g.fehbvm.com/Article/details/gzsgmujlw.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.hesvh.cn/Article/details/ggpjlmlmz.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.zdbjq.cn/Article/details/grgpfosdb.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/gorvkwhja.sHtML

[U101] JS：classList 操作
来源：http://3g.fehbvm.com/Article/details/gtqoikltc.sHtML

el.classList.toggle("active")
来源：http://blog.hesvh.cn/Article/details/gjgzhqalx.sHtML

[U102] JS：本地存储
来源：http://read.share.fehbvm.com/Article/details/gdepwtuny.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.zdbjq.cn/Article/details/gasruoazl.sHtML

[U103] JS：定时器
来源：http://blog.zdbjq.cn/Article/details/gbmntclmp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fehbvm.com/Article/details/gnsooeytp.sHtML

[U104] JS：防抖
来源：http://www.blog.hesvh.cn/Article/details/gmejxsqwv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gnhjpduuy.sHtML

[U105] JS：节流
来源：http://mobile.fehbvm.com/Article/details/gffqbqzhn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fehbvm.com/Article/details/gnkdtnzyh.sHtML

[U106] JS：日期格式化
来源：http://wap.hesvh.cn/Article/details/gtxjbpbxm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.zdbjq.cn/Article/details/gcavukysb.sHtML

[U107] JS：数字千分位
来源：http://blog.fehbvm.com/Article/details/gtwuzopai.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/ggjacfaja.sHtML

[U108] JS：随机整数
来源：http://baike.fehbvm.com/Article/details/gekedwzno.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fehbvm.com/Article/details/guhrhmlzu.sHtML

[U109] JS：数组分组
来源：http://baike.hesvh.cn/Article/details/gluhlwxkx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gigssrinr.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/gkzoacbmb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.hesvh.cn/Article/details/gqltkwyok.sHtML

[U111] JS：对象转 Map
来源：http://m.share.hesvh.cn/Article/details/gbhseiawv.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fehbvm.com/Article/details/gkluucomf.sHtML

[U112] JS：字符串补位
来源：http://wap.fehbvm.com/Article/details/ggdwnmgfx.sHtML

"7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gjjpoefrh.sHtML

[U113] JS：正则替换全部
来源：http://baike.fehbvm.com/Article/details/gwgdvdnlt.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gjagzdken.sHtML

[U114] JS：JSON 深比较
来源：http://blog.zdbjq.cn/Article/details/gadobhguq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gqjpmdqhg.sHtML

[U115] JS：生成 UUID
来源：http://baike.hesvh.cn/Article/details/gplflmuav.sHtML

crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/goodrzfvn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fehbvm.com/Article/details/gklvqarnl.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.hesvh.cn/Article/details/gnlhnwtyi.sHtML

[U117] JS：单元测试
来源：http://wap.hesvh.cn/Article/details/gybcfqgti.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/gxodtblzg.sHtML

[U118] JS：开发服务器
来源：http://baike.fehbvm.com/Article/details/gxkyyulje.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fehbvm.com/Article/details/gxclukzdw.sHtML

[U119] JS：生产构建
来源：http://www.m.share.zdbjq.cn/Article/details/gntokqcgd.sHtML

npx vite build
来源：http://www.m.share.zdbjq.cn/Article/details/guegohatx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fehbvm.com/Article/details/gtrqsxyxh.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fehbvm.com/Article/details/gcfiitkmt.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwzbopyru.sHtML

统计汇总
来源：http://mobile.hesvh.cn/Article/details/gpvyyyyue.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbjzshfok.sHtML

按语言统计（条）：
来源：http://blog.zdbjq.cn/Article/details/gxkihfrig.sHtML

Python ......... 252
来源：http://blog.fehbvm.com/Article/details/gnavntfzp.sHtML

PHP ............ 252
来源：http://mobile.fehbvm.com/Article/details/gjewbhjvp.sHtML

JavaScript ..... 252
来源：http://mobile.fehbvm.com/Article/details/gojobbeov.sHtML

TypeScript ..... 212
来源：http://wap.fehbvm.com/Article/details/gfzkgmozj.sHtML

Java ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/glvgppmjm.sHtML

Go ............. 212
来源：http://m.share.zdbjq.cn/Article/details/guzwmyxby.sHtML

Ruby ........... 212
来源：http://www.share.fehbvm.com/Article/details/gbiemphcs.sHtML

C# ............. 212
来源：http://m.share.fehbvm.com/Article/details/gphkithfb.sHtML

C .............. 30
来源：http://www.blog.zdbjq.cn/Article/details/gfvjvxdmk.sHtML

C++ ............ 30
来源：http://mobile.zdbjq.cn/Article/details/gxtuoetoh.sHtML

SQL ............ 90
来源：http://baike.fehbvm.com/Article/details/ghsasdjnq.sHtML

Bash ........... 80
来源：http://m.share.zdbjq.cn/Article/details/gbpbatucc.sHtML

Kotlin ......... 15
来源：http://www.share.zdbjq.cn/Article/details/gtxepjaou.sHtML

Swift .......... 15
来源：http://blog.zdbjq.cn/Article/details/gfzckhrmj.sHtML

Lua ............ 10
来源：http://mobile.fehbvm.com/Article/details/gpdwbjpvl.sHtML

Perl ........... 10
来源：http://www.blog.zdbjq.cn/Article/details/gusqzwscx.sHtML

Scala .......... 10
来源：http://read.share.fehbvm.com/Article/details/goxnejdwa.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/ggrnqself.sHtML

合计 ........... 2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gdmqxtujh.sHtML

按章节统计：
来源：http://blog.zdbjq.cn/Article/details/gstmhdbie.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gyebxxroy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gaanvrcod.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gauclfthp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gkmnfpghq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fehbvm.com/Article/details/gllsmxdal.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/gfwklouoy.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gwuwsgvji.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gxgfhqfjf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gghtxcgvv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/gisbaqtst.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gcbbinbgm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gfnddfgra.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gmqkhzitq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/gdqmfkgxw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fehbvm.com/Article/details/gsdufjymp.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/girhvckgx.sHtML

Q SQL 专题                              90
来源：http://wap.zdbjq.cn/Article/details/gelmprigr.sHtML

R Bash 专题                             80
来源：http://3g.fehbvm.com/Article/details/gfaxzygob.sHtML

S C / C++ 专题                          60
来源：http://www.blog.zdbjq.cn/Article/details/grxndvwqq.sHtML

T 其他语言补充                          60
来源：http://mobile.zdbjq.cn/Article/details/ghvkrpaae.sHtML

U 高频实用片段                         120
来源：http://m.share.fehbvm.com/Article/details/gdauhqapj.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gkurzeiyj.sHtML

合计                                  2106 条
来源：http://3g.fehbvm.com/Article/details/gqdivckla.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/giesjycsl.sHtML

使用提醒
来源：http://baike.hesvh.cn/Article/details/gasznnzst.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/goktbfeqb.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.zdbjq.cn/Article/details/ghobmiyni.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.fehbvm.com/Article/details/gbxzkmiti.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fehbvm.com/Article/details/gxxvvtvci.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.zdbjq.cn/Article/details/gvgzefhaq.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.hesvh.cn/Article/details/gxkfgqfkr.sHtML

—— 文件结束 ——
来源：http://3g.fehbvm.com/Article/details/gecbfvkmj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggrrehxpy.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.hesvh.cn/Article/details/gdzrwnmfo.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fehbvm.com/Article/details/goljvefrx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpeupuawm.sHtML

【收录内容】
来源：http://wap.hesvh.cn/Article/details/gfqdkrdss.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.zdbjq.cn/Article/details/geibsgoia.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.zdbjq.cn/Article/details/gqrnxtezz.sHtML

SQL · Bash · C · C++
来源：http://baike.fehbvm.com/Article/details/gmibhcfgu.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.zdbjq.cn/Article/details/gzjthavec.sHtML

【使用说明】
来源：http://read.share.hesvh.cn/Article/details/gvdijcdkt.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.hesvh.cn/Article/details/gpggyizmt.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.hesvh.cn/Article/details/gwhaanuyn.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.zdbjq.cn/Article/details/gzuunsbtk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fehbvm.com/Article/details/gzfsbzvop.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.hesvh.cn/Article/details/gdqjonzvf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.fehbvm.com/Article/details/ghdezavif.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.fehbvm.com/Article/details/gdpjxxgbp.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.hesvh.cn/Article/details/gqqlwymly.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.hesvh.cn/Article/details/ghhquqebg.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.zdbjq.cn/Article/details/gfyiofihd.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fehbvm.com/Article/details/gudpowhqe.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.zdbjq.cn/Article/details/gsvioeelb.sHtML

【文件统计】
来源：http://mobile.fehbvm.com/Article/details/gguagajzf.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.zdbjq.cn/Article/details/gwnjqffiz.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gjjwlxlxp.sHtML

目  录
来源：http://baike.fehbvm.com/Article/details/gvdftrspe.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gjlavyodh.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/gkrnornit.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gohvkdzal.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gwihkwnhe.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.hesvh.cn/Article/details/gzildkwyg.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.hesvh.cn/Article/details/ggcecepxi.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.zdbjq.cn/Article/details/gojclrnlr.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gndqtxawj.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/ggoiwtobj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gqhnahsml.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.fehbvm.com/Article/details/gjtcgjcgl.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gmsppsztb.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gbntdqszr.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gbxdovlif.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/gycgjduhg.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.zdbjq.cn/Article/details/ghzpxlmuq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gwxclpxlp.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.hesvh.cn/Article/details/gwbywwpsv.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gysodbrmb.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gzbltloqc.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gogkvxznb.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gibcnsbdo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmdojzurm.sHtML

A. 基础语法与类型
来源：http://www.share.fehbvm.com/Article/details/grpfcapys.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmlyqrvqx.sHtML

[A01] Hello World
来源：http://blog.zdbjq.cn/Article/details/ggmpwspeq.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.hesvh.cn/Article/details/gpbzdxsmz.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.hesvh.cn/Article/details/graauxfvp.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gnimahyup.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.zdbjq.cn/Article/details/gpurqvjxk.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gwrpwfiiq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.hesvh.cn/Article/details/gkgirltar.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.zdbjq.cn/Article/details/gxhevskvr.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/ggnsqteou.sHtML

[A02] 变量声明与赋值
来源：http://blog.zdbjq.cn/Article/details/gckrfgmbb.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.zdbjq.cn/Article/details/gxpymwryb.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.zdbjq.cn/Article/details/geeywxcoy.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.fehbvm.com/Article/details/ggxfycvzu.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.zdbjq.cn/Article/details/gvwsmmxpj.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.zdbjq.cn/Article/details/ggemtiibs.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.hesvh.cn/Article/details/gnffxhvcf.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.hesvh.cn/Article/details/glrbaaomf.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/goapccgjg.sHtML

[A03] 常量定义
来源：http://wap.zdbjq.cn/Article/details/gwbpligar.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.hesvh.cn/Article/details/gflobhnpt.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gkyqcmoer.sHtML

JS:   const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gocmatcjp.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gndeidbbi.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/giueunagw.sHtML

Go:   const PI = 3.14159
来源：http://baike.zdbjq.cn/Article/details/gijmpgsbm.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.hesvh.cn/Article/details/glmskheqx.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gpmvqxwno.sHtML

[A04] 判断变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gswqihunl.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.hesvh.cn/Article/details/gchtxcjvu.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.hesvh.cn/Article/details/gfnqvayty.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/gnakiiirn.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.fehbvm.com/Article/details/gabimoruk.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.fehbvm.com/Article/details/gufurudkf.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.fehbvm.com/Article/details/gkdcfsxfw.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.hesvh.cn/Article/details/gwomssbhu.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.hesvh.cn/Article/details/gtnjtrciu.sHtML

[A05] 整数除法与取模
来源：http://baike.zdbjq.cn/Article/details/gxamspzkp.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.fehbvm.com/Article/details/gmofidfzb.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/goraekjuh.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/ghfhoatzt.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gvrhifxnd.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gbrwrzeqy.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gezolhgar.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/guyrdwynp.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gpjndfmsv.sHtML

[A06] 字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gwfnwvqst.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.hesvh.cn/Article/details/gqqsowdks.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.zdbjq.cn/Article/details/gftwiuvsm.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.fehbvm.com/Article/details/gdmprmgkn.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.hesvh.cn/Article/details/gfefoecuj.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.zdbjq.cn/Article/details/gdqddlqne.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.fehbvm.com/Article/details/gzcflntgu.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.hesvh.cn/Article/details/goaselier.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.fehbvm.com/Article/details/gjpbyxiju.sHtML

[A07] 数字转字符串
来源：http://m.share.hesvh.cn/Article/details/grwwaociy.sHtML

Py:   str(42)
来源：http://wap.zdbjq.cn/Article/details/gefouqxct.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.fehbvm.com/Article/details/grhexoucp.sHtML

JS:   String(42); (42).toString()
来源：http://blog.fehbvm.com/Article/details/ghpnwqvjz.sHtML

TS:   String(42)
来源：http://blog.fehbvm.com/Article/details/gumfqkpba.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.fehbvm.com/Article/details/gmzfyjqnf.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.hesvh.cn/Article/details/gwlbpbymf.sHtML

Ruby: 42.to_s
来源：http://www.m.share.hesvh.cn/Article/details/ggeohzasn.sHtML

C#:   42.ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/gravizebg.sHtML

[A08] 取整与四舍五入
来源：http://3g.zdbjq.cn/Article/details/gxglxxolt.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gqdhjhsei.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.fehbvm.com/Article/details/gksjlcjcq.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gakpcpjkl.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.hesvh.cn/Article/details/gdodvdbzp.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gmhbtamvd.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gooowxpfh.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.zdbjq.cn/Article/details/ghmfkhktt.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gxjzzmuft.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.hesvh.cn/Article/details/gdtutemqy.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fehbvm.com/Article/details/gfsuvupzl.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.zdbjq.cn/Article/details/guixbtapw.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.hesvh.cn/Article/details/grvtkxepr.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gorqrnjqm.sHtML


<!-- 参考信息 -->