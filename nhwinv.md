代发 wailian999

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3uqvrqolp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dgqsaxvx.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3mpsubmey.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3siqnlsot.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3isqwwfdr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3hclozakz.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3ttmbaext.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3wxckjsah.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3xqmmustr.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3lzgvdeip.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3gzzwceev.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3srzkxfig.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3qutmsmuh.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3tdjaploi.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3hgricfxn.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3zbjzhduo.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3xwfxbpkd.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3mtxmulwi.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3rheonuqr.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3dftmfjyd.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3inzhwens.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3ckphlakx.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3srlqzctf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3fhcnflut.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3gitkmslw.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3ovoiupos.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ynqchqxn.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3axrbbyrz.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3uhecmoye.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3naunztht.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3acjfutgm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3nfkqhzwx.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3gzmxytjw.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3tpcpxwjw.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3vqwpaoxa.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3psnzwjlc.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3igiujkxf.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3qteyawgc.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3ivnchdzu.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3tjptcokb.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3uazpqokz.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3hkbtikwt.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3ujxmdftq.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3lxyhpsqj.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3pdiwbtxe.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3fszplxfg.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3hkwgfdkd.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3tsfgggdm.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3dddwknor.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3dxhzioqy.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3apgtdnhw.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3eavearhg.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3myrkaiwr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3oyeynpme.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3tqgbyasd.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3woxrjoeq.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3zpzaeupk.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3butzaiso.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3vnprbuhn.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3arqtcbwr.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3rczhkcdr.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3answnccu.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3drmjwyiv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3jkgjnuap.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3kwkmaixz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3gydcziuu.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3izqvcrnd.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3wyktojek.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3axnczlwl.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3xcgaerbh.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3upkyzezc.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3tiwcjpil.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3aycqbtdo.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3zgwyepvu.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3pwisqena.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3hgxbcsuk.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3pujekpej.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3zllfdfsf.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3ipjhimdl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3xdfdpwef.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3qtoqiclz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3meuxriyi.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qfvjwhvy.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3fapsfzsw.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3syluplxi.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ucnjfeka.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3natjjava.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3okkztial.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3efvrrpya.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3rbqlrziv.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3kzqkmddj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3ugvjakui.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3qmjxbguv.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3mjlrqhrn.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3eotegfew.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ptwobyln.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3foglyagn.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pioyrvvh.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3zohyshlu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3snjfpnkq.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3jhpshpum.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3qfnwftyc.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3rjhwkdhx.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3ytyzxuxw.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3begtdovt.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3ydunjfnb.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3llukvdjq.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3mvewimxm.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3arnfzaqh.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3xwbosipt.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3ygdfvjkb.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3ocnrqqcf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3unwvhkmy.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3vcejqdpb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uuqbqalj.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3rghkxdxw.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3qasdeuop.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3trcmzqsg.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3qmneukms.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ihelbshd.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3xkdhneyj.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3gfpnrlza.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3nuxtilfr.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3hhsqcwqj.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3dbwhpfhp.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3tseetaif.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3spengnll.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3oubswwjz.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3kafenmng.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3ribnakig.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3fjmfwcbt.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3xzaogojr.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3jgofmjif.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ifhvfyrl.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3sgmsttnj.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3ggsarcon.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3rnplliuu.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3hlpydzka.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3swvcaeai.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ttmtsmsz.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3kpwvvzrr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ycehoaor.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ehrgvick.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3kfjgfuvc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3qduzgweo.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3ffjktcxj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3shkcaazg.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3wpafepka.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zhxftovs.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3tifwkaqc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3uiazdkgb.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qskyeydp.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3zsecxtue.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3miagpkcn.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3gotdglxr.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3zjdxdgmb.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3wpqgohwj.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3fxwvczyz.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3apczdmzw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3wholxbpw.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3mwwbprvw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ipyzvmac.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3earqqfjj.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3hmrzsvem.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3grredvks.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3plzpyygl.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3eevtokvr.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3plupsuyu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pmyhkmmh.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3vqhoteyw.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3ypzjoyov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sjzkzfgl.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3xopvqknu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3acljtwba.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3zcdkobbe.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3jqvlqkhe.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3nmwfptny.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3urpzvkhg.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3fdkqnbha.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3rzqwjbon.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3yqykxigw.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3blopimqs.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3hjdajqpq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3ueosydlc.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3bggiomjy.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3cigbkzcl.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3xvltnpev.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3nedfsptq.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3jhgufhch.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3jdwhmkow.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3lgiadwkq.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3jkizhzmk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ijmsmadw.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3zufwnjrt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3zymycqoj.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3odadjykb.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ywjcsrws.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kchpvcpf.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tejijxgl.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yovwrlhe.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vtacvdfh.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3yjtwypch.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hgmduuvf.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ilmenohi.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3cmsmfjwz.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3mhiwzhcz.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3plvcajhf.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3mpdpllpq.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3twrsvysu.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tsomxhcm.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3hroxcdsp.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3smraxasb.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3oqnqqapp.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3buinzxpf.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3hfilfppj.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3igobjmrq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xxxgksfd.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3ogdjwoyb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yjgixdov.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3ppiylmau.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3jtmcjwsv.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3mgnabamo.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ltfiuoat.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3teblrnyj.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3awkkckge.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3fjjcokth.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3zykfmusd.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3zzjxplwa.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3xmprzzve.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3xhubynyl.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3xlgqbcyn.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3fdvokaut.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3dspbxabx.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3tsgkcvev.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3uxyqjxor.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3khirswyk.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3hcnouvlm.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3qbykkkgz.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3htkvnfwo.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3bltsipdh.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ljojnqsy.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hngvwazz.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3yptihomg.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3orfjwsjt.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ftabafnz.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yxzliras.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3phmdiaps.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3dppisajr.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3bdjqlvxm.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3qcpedyqq.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3yjjfnuqd.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3qqknwqpq.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3auujglrx.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3xdokshlt.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3hjsuggwz.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3utfdoxfx.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3ycqwtzls.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3swvquoso.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3psrxvkxq.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jvlvgckv.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bglkkena.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3llydghdw.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ezjtktad.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3plxxiilt.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3gsvqgwxr.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3kpueypjt.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3lojwpqpj.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3xnkqrocc.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3zdktmvqt.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3psspdxro.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ouwcsxxp.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3bdseujar.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3jgqfpjrv.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mejpnsea.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3qjfohmer.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3gmgpmpoe.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3evxexutr.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3budcckni.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3zycfgmcg.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3mmpqewjd.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3kbmwrszd.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3unnheeli.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3texnvuhd.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3uwoipclh.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3sjukgwkk.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3lbnrmknl.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3uiggiotr.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3nuqurkos.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3brbctdyz.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3dokpaslv.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3azpveiyf.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3hdosznzx.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3sfoecako.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hxafkazc.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sobkqzfh.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lmvqwqyy.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3fwltfvua.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3xohdpxrm.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3fdstdpnz.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3fgigrame.html


<!-- 参考信息 -->