代发 wailian999

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3dubpcxpc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hjdmbdrn.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3igypzfyh.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3ojszhkza.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3ofnneffa.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3ipefdttw.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wkzmmnbm.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3squxwkep.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3ypzvdxnh.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3htgqzbzm.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3lmtkekos.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3jotaxhvx.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3cnujusjy.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3mxlrxhqt.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3ryenspff.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3ypmommbt.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3pspckdmg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3joznhszj.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3qvkbrcbu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3sytgxelx.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3wafawvra.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3vppnumea.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3gxvnqajo.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3qajdrcvg.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3zlyfqokp.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3nznxugbz.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3uvbhryhv.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3gfrvrumy.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3lxpgfoxq.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3vxdmyxpy.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3lohryrgb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3pzaueznh.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3wpfltipj.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3zbibeapn.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3jlggpcjg.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3rzxiwaxt.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3nhvaajxc.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3fyuezppo.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3mxbqyrak.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3kfdsxliq.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3xxapfqhe.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3wcrrjnkq.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3loyyzgem.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3nidmllcg.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3bwofjwvr.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ywzbedyh.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3vxhqmlfw.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3kzvmgiso.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3awkzwamr.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3aackqnvl.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3wnxkbtid.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3zsznhxwp.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3jqylhnwh.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3rkkxyrcl.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3udrknrdi.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3jagmszjt.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3iposcgti.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3atkeklzt.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3nieauisd.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3xujfgbzh.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3cmbflmwn.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3yumniyuh.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ohxquqam.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fapnhcye.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ilcugcpr.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3prffdupm.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3qabrbcel.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3seivrlmc.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3afsngqas.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3sqgdyzgu.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3grltldwq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xmbytlbm.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3uqtnfsyz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3irnqpipe.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3eufpbezx.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3znpwsfii.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3cgunupok.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3rghsnilb.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3rgxcpqlt.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3hlagqevy.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3dqkmsnmc.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3jsglrokb.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3vfukqmxo.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3emxeptxp.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3qhhwwzja.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3rqtopmel.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3ljnedytz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lmtbiigy.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3dznipbsu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lwwdhlzp.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pcvzywsi.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3oktepefi.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3aabvjfst.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3cikyvvdo.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3texlzjow.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3mmiqddfy.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3cdlraddi.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ljcizixm.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3qwamthek.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3qkderqom.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3ypjbkght.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3vwixjymb.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3ccldgith.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ksofieya.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3hctxapkx.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3plfutery.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3cifzokdd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ewmztrxb.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3oiiponqc.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3gqygkfct.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3qovomerl.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xmkcxwfu.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3caxblode.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3yclcnddc.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3jxicfbzt.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3kcxdrnok.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3mcomaofs.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3hpfxvpkx.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3cciyqwhx.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3mqgquehm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hnxhxgob.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3lilakwfa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3emomykud.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3uhcrdrwl.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ywqoznnd.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3eqjbofrp.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3qrcfjskq.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3lfrhgusw.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3mhagsvgk.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ikntktcm.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3gfgkcyhp.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3fozucxib.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3opkogrur.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3stlwsxaf.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3pmciohxz.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3zidcirlc.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3nctcsglp.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3jrvkwfmz.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3gpvxsgzx.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3fqlaedke.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3kxiswwdn.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3iuagusba.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3dcvfmnfg.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3slnoswgp.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3wiaxvwtg.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3msbgmkix.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3qjaotzfr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3nektixez.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3gcklzbcw.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ledtdkht.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3aeulhzfx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3zmaukofz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vdlmuowf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3nmmcywtq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3yyeyktqq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vjbhvzud.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3wyesniev.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3lymevikn.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3ajocwwmm.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zhmzjgxx.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3vfxxklfb.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3kxixubvb.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3tnnckhpj.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3bzopwxmk.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3mgcnefqb.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3vtembsgw.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3ofjpbgqz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xbdivgrl.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3hnhciprn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mjkejeoj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3imwqoifz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3dtjklzvs.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3uewntexz.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3dndeaovq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3hgoezhmc.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3odvmlptf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3czwtwrma.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3mcfyrfwh.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3qocaomlc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kjqhzofn.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3dtojlvxx.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3ezecytjw.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3hktgnmrb.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3cmxuesfr.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3skyagvjy.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3dzsisrbq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3sdutaoth.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3eiyldgko.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3hbcdutvd.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3btlpvcwy.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3ktztiwrc.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3jubujfqy.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3aypaqbkb.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3xdhofjno.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3cajrcuiv.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3ambmrxmg.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3lodlusrx.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3yeqjaciv.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3ntibwasf.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3jxzncqyc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3kvwgcfrl.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3xpiezqzo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3wqxrryfc.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3jndlhfpl.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3ktabghsi.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3atwkpkrv.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fbsbuuqc.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rkoqczoh.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zsnlewks.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3aqoquduv.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3xuhnragp.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dnfwfjhr.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cdwxgevn.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dxgdquis.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3sslhgxlw.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3aaacsxxi.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3tespkpmf.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hhfmfawh.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3vpavucjn.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3qsfaqlhx.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pamdykkk.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3uepvaiss.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3byymaduu.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pngvhyjz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wsilwkfw.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3tirdzjlq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ifvfddmm.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ynjijkdd.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3fgkmemdu.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3yuwsfhag.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3khlwjwfh.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3dotcydzh.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3jlchspbo.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3pbozcard.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3tnyseaof.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3vmaywkqy.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3nrvofkes.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3tdowfwky.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3davjrezu.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3tkzenspk.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3obuizzfp.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3qatauikn.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3wjfsjhgl.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3dfovjbrr.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3emtxjbpt.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3bkzhnaxk.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3gyvaynce.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3grjjgsnn.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vbwwdazd.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qijcgbaj.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3piuhserp.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3codbioil.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3uovolgtz.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vlwhkqea.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3slwjmanh.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3uzvnssoq.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3iasyxymk.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3zwhkcsnb.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3hjpfdfhu.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3zclgrout.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3ftbvkeug.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3dixiktdg.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3ouqtwzeo.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3gbxwshjh.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3fbwwlktf.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3qkczusja.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vcclsobt.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3teesvtvl.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wtpsxvpf.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3uzulhqbs.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dcwmeafv.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3fnbgvtve.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ldimvagj.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3qiutvkgg.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3zslprhvp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3xuwuymxt.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3uslwzged.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3iehtqztv.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3kvstxgld.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3bewlobax.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3buinnwwk.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3uhwxwldd.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3dgojzolq.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3teonjwsp.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3dkvyrmeu.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3tobntldd.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3xwyfejmt.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ixpvzmnr.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3hdeauqeq.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3cizngnft.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3ynekecrz.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3rjcqlujl.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3qshqqvfl.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3xfehyonx.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3tlclnqmm.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3zuywwmkc.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3lwpynsqm.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3ezunjnts.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3gxebgyru.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3qrqxwpyo.html


<!-- 参考信息 -->