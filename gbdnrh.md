代发 wailian999

[U59] PHP：自定义排序
来源：http://hz.gogol.net.cn/gtosdmslhd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhoulong.xyz/gtadcxkpqy.html

[U60] PHP：JSON 编解码
来源：http://hz.feifeiyinyue.top/gtgwoereot.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.yj20258.top/gtgpzipyca.html

[U61] PHP：正则
来源：http://hz.xinyue.icu/gtyblrmvyy.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.gotoacloud.top/gtluwjuikn.html

[U62] PHP：日期对象
来源：http://hz.hnxiangtu.top/gtweruborc.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.xylfe.cn/gttheaduqi.html

[U63] PHP：文件读写
来源：http://hz.ybcxt.top/gtujnkphoc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.aibaodan.cn/gtidqowvql.html

[U64] PHP：目录遍历
来源：http://hz.zhijiandao.cn/gtbvcszreh.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.yongpay.top/gtstytcutu.html

[U65] PHP：会话
来源：http://hz.wangshuangyany.cn/gtxwtzmkhw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.shangyingyoupin.top/gtvmnwwslj.html

[U66] PHP：设置 Cookie
来源：http://hz.zhoulong.xyz/gtyrireihf.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.cashguo.top/gtixzorjst.html

[U67] PHP：处理文件上传
来源：http://hz.yuanzhike.top/gtckjuzmyc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.andypj.xyz/gtfflvdyza.html

[U68] PHP：PDO 连接
来源：http://hz.9152youxi.cn/gtuthoernh.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.sysykeji.top/gtrteyabbb.html

[U69] PHP：PDO 预处理
来源：http://hz.xingfuxueyuan.xyz/gtppoqzsug.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.feifeiyinyue.top/gtvahfhskc.html

[U70] PHP：PDO 事务
来源：http://hz.iojbl.cn/gtcwdbkfyp.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.vqdsnc.cn/gthejyijzb.html

[U71] PHP：抛出异常
来源：http://hz.daxiang520.top/gttlfeanuj.html

throw new RuntimeException("失败", 500);
来源：http://hz.gogol.net.cn/gtyuteenil.html

[U72] PHP：写错误日志
来源：http://hz.birdmap.top/gtcbjeiyhm.html

error_log("失败: " . $e->getMessage());
来源：http://hz.xuanzx.com/gtgmjooyzq.html

[U73] PHP：读取 ini 配置
来源：http://hz.shuidangran.top/gtfccvtrpc.html

parse_ini_file("config.ini", true)
来源：http://hz.jyoumei.cn/gtbnwthwow.html

[U74] PHP：读取环境变量
来源：http://hz.gotoacloud.top/gtilvjzfhf.html

getenv("APP_ENV") ?: "production"
来源：http://hz.jianghu66.top/gtknzrrvsi.html

[U75] PHP：依赖注入
来源：http://hz.cdnleiting.top/gtclhftuqi.html

composer require psr/container
来源：http://hz.yuxming.cn/gtbixulopu.html

[U76] PHP：简单路由
来源：http://hz.cashguo.top/gtcirkqvtr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.smart0.xyz/gtptqwuwsq.html

[U77] PHP：模板渲染
来源：http://hz.chenjidiqi.icu/gtfgnrkmvl.html

composer require twig/twig
来源：http://hz.hnqzz.top/gtiwtnwhej.html

[U78] PHP：单元测试
来源：http://hz.zhaomingkeji.xyz/gtphcpggjd.html

composer require --dev phpunit/phpunit
来源：http://hz.cashguo.top/gtrevtyuuk.html

[U79] PHP：静态分析
来源：http://hz.nanxinkj.top/gtammqibje.html

composer require --dev phpstan/phpstan
来源：http://hz.0kj1m.cn/gtsihhrnsz.html

[U80] PHP：代码规范修复
来源：http://hz.iojbl.cn/gtrdthqqze.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.jinqigfzy.top/gtkummmnuu.html

[U81] JS：初始化项目
来源：http://hz.yj20258.top/gtxmlhqnhe.html

npm init -y;  npm i express
来源：http://hz.jqgufenzy.top/gtghvmgcfd.html

[U82] JS：package.json 脚本
来源：http://hz.andypj.xyz/gtvjwywyuo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.sweek.top/gtjgddafuq.html

[U83] JS：ES Module 导入导出
来源：http://hz.ydzc1.top/gtnxpvntfr.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.xuetiantiany.cn/gtwotiaykl.html

[U84] JS：CommonJS 写法
来源：http://hz.svipenyu.cn/gtwnjjzusg.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.chenjidiqi.icu/gtznpwvwsj.html

[U85] JS：可选链
来源：http://hz.chenlongwang.top/gtiqwzfozs.html

a?.b?.c
来源：http://hz.yj20258888.top/gtvqsjuyfu.html

[U86] JS：空值合并
来源：http://hz.yonumen.top/gtcdiiqkjg.html

a ?? b
来源：http://hz.zhijiandao.cn/gtfcbhckzz.html

[U87] JS：解构默认值
来源：http://hz.316326.xyz/gteohpbkac.html

const { a = 1, b = 2 } = obj;
来源：http://hz.ehwqpu.com/gthmyhzudh.html

[U88] JS：对象展开合并
来源：http://hz.yueranfly.top/gtgszdmlsg.html

{ ...a, ...b }
来源：http://hz.sufxvd.cn/gtxbajjwme.html

[U89] JS：数组去重
来源：http://hz.yj202588.top/gtdwvicljd.html

[...new Set(arr)]
来源：http://hz.ydzc1.top/gtyiujykgw.html

[U90] JS：数字数组排序
来源：http://hz.pycfn.com/gtwqomklhf.html

[...arr].sort((a, b) => a - b)
来源：http://hz.quarkkingdee.top/gtxodvqumn.html

[U91] JS：对象键值遍历
来源：http://hz.aizwys.cn/gtvomlwieo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.cashguo.top/gtjijevjul.html

[U92] JS：深拷贝
来源：http://hz.zhoulong.xyz/gtawvccqjm.html

structuredClone(obj)
来源：http://hz.shanyushiyangtech.top/gtmzucmsgz.html

[U93] JS：模板字符串
来源：http://hz.kuanghao11.cn/gtivzeldyi.html

`共 ${n} 条`
来源：http://hz.zhijiandao.cn/gttaqxgjzq.html

[U94] JS：箭头函数
来源：http://hz.9152youxi.cn/gtrmrmgkba.html

const double = x => x * 2;
来源：http://hz.haohaochexian.top/gtiqdxssen.html

[U95] JS：Promise 包装
来源：http://hz.zycfv.cn/gthitomjvj.html

new Promise((resolve, reject) => {})
来源：http://hz.wangdashe.top/gtdetwzzir.html

[U96] JS：async/await 与异常
来源：http://hz.zhongyouzk.top/gtsiwudfiw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.yuxming.cn/gtlfkjqqep.html

[U97] JS：并发请求
来源：http://hz.aibaodan.cn/gtwvhslwus.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yongpay.top/gtawqxtbiz.html

[U98] JS：fetch 带 JSON
来源：http://hz.fzhhl.top/gtcmswyxfl.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.c1oappe.top/gtwgnzsweg.html

[U99] JS：事件监听
来源：http://hz.316326.xyz/gtzeknsihf.html

el.addEventListener("click", e => {})
来源：http://hz.pengpengdd.cyou/gtfhskfpcd.html

[U100] JS：DOM 查询
来源：http://hz.cashguo.top/gtzkdkvwah.html

document.querySelector(".item")
来源：http://hz.cqqwz.cn/gtupmuffok.html

[U101] JS：classList 操作
来源：http://hz.smart0.xyz/gtazornhzi.html

el.classList.toggle("active")
来源：http://hz.9152youxi.cn/gtxukzhbtp.html

[U102] JS：本地存储
来源：http://hz.yj202588.top/gtnclmrokx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.yj202588.top/gtuypwudje.html

[U103] JS：定时器
来源：http://hz.chenlongwang.top/gteimvordn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.xinyue.icu/gtnhbyncjg.html

[U104] JS：防抖
来源：http://hz.ehwqpu.com/gtvkfxlofs.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yuanzhike.top/gtrdhwyvcl.html

[U105] JS：节流
来源：http://hz.sufxvd.cn/gtqaxmrjae.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.jianghu66.top/gtgxihopbj.html

[U106] JS：日期格式化
来源：http://hz.zhiwuduotai.top/gtcdpfrdlr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yanxiufei.cn/gteqwmnsar.html

[U107] JS：数字千分位
来源：http://hz.jiagoushi.top/gtlkgtpbcc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.aibaodan.cn/gtztedzlaf.html

[U108] JS：随机整数
来源：http://hz.xziqi.cn/gtqptbfwcj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.andypj.xyz/gtzwgugedq.html

[U109] JS：数组分组
来源：http://hz.jyoumei.cn/gtvvkefzye.html

Object.groupBy(arr, x => x.type)
来源：http://hz.jiagoushi.top/gtlbswbyld.html

[U110] JS：数组分块
来源：http://hz.feifeiyinyue.top/gtlgerqeji.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.316326.xyz/gtkhvtxond.html

[U111] JS：对象转 Map
来源：http://hz.yueranfly.top/gtwthcdncj.html

new Map(Object.entries(obj))
来源：http://hz.52xcode.cn/gtbxkqhrke.html

[U112] JS：字符串补位
来源：http://hz.gogol.net.cn/gtbdjerbrp.html

"7".padStart(3, "0")
来源：http://hz.zhixingplan.top/gtjvqwdbsf.html

[U113] JS：正则替换全部
来源：http://hz.feifeiyinyue.top/gtsxfovxal.html

s.replaceAll("a", "b")
来源：http://hz.nanxuanxn.top/gtdthkyfbn.html

[U114] JS：JSON 深比较
来源：http://hz.quarkkingdee.top/gtlhqidbbk.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yuanzhike.top/gtymejtkaf.html

[U115] JS：生成 UUID
来源：http://hz.wangdashe.top/gtgsaymobb.html

crypto.randomUUID()
来源：http://hz.redwolf501.top/gtrixiuwrp.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.yueranfly.top/gtxlziyavc.html

/** @param {string} name */ function f(name) {}
来源：http://hz.hywenlv.cn/gthvxgcibr.html

[U117] JS：单元测试
来源：http://hz.jinyuanbaomall.cn/gtfhdqnhen.html

npm i -D vitest;  npx vitest
来源：http://hz.9152youxi.cn/gtdmkpcusk.html

[U118] JS：开发服务器
来源：http://hz.ehwqpu.com/gtavdfigfa.html

npm i -D vite;  npx vite
来源：http://hz.jinyuanbaomall.cn/gttewhvfyn.html

[U119] JS：生产构建
来源：http://hz.gotoacloud.top/gtccwjxzdm.html

npx vite build
来源：http://hz.chenjidiqi.icu/gtplwspyfv.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.havefunace.top/gtwqjjonsn.html

import.meta.env.VITE_API_URL
来源：http://hz.ydzc1.top/gtmfzushfu.html

================================================================================
来源：http://hz.jlsjyb.cn/gtbjbpaxxv.html

统计汇总
来源：http://hz.haohaochexian.top/gtruzujbax.html

================================================================================
来源：http://hz.daxiang520.top/gtqaqcykvf.html

按语言统计（条）：
来源：http://hz.jyoumei.cn/gtifmsdpgl.html

Python ......... 252
来源：http://hz.jinqigfzy.top/gtmlokwwdr.html

PHP ............ 252
来源：http://hz.xinyue.icu/gtozwdlrkw.html

JavaScript ..... 252
来源：http://hz.c1oappe.top/gtxaufetys.html

TypeScript ..... 212
来源：http://hz.pycfn.com/gteswjhmfw.html

Java ........... 212
来源：http://hz.vqdsnc.cn/gtemtllxhy.html

Go ............. 212
来源：http://hz.xuanzx.com/gtbnydeink.html

Ruby ........... 212
来源：http://hz.kuanghao11.cn/gtfdfowjvk.html

C# ............. 212
来源：http://hz.jinghuilouyu.cn/gtkphorrfa.html

C .............. 30
来源：http://hz.meibo888.top/gtnroqjfgx.html

C++ ............ 30
来源：http://hz.aizwys.cn/gtneccygka.html

SQL ............ 90
来源：http://hz.pengpengdd.cyou/gternbrimy.html

Bash ........... 80
来源：http://hz.yvedp.cn/gtegqarmgq.html

Kotlin ......... 15
来源：http://hz.xuanzx.com/gtwxrfmtbv.html

Swift .......... 15
来源：http://hz.hysaishi.cn/gtiqbsvjee.html

Lua ............ 10
来源：http://hz.sufxvd.cn/gtwgdaafam.html

Perl ........... 10
来源：http://hz.vqdsnc.cn/gtoufnzktl.html

Scala .......... 10
来源：http://hz.jlsjyb.cn/gtlycikfgl.html

------------------------------------
来源：http://hz.zycfv.cn/gtkirejsag.html

合计 ........... 2106 条
来源：http://hz.yuxming.cn/gtzwqjcmlo.html

按章节统计：
来源：http://hz.cheryme.top/gtanhqbnvo.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.xuetiantiany.cn/gtaxftccgw.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.ybcxt.top/gtdalsxlld.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.quarkkingdee.top/gtfqxewrrr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.jinghuilouyu.cn/gtcrrzhmbp.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.0kj1m.cn/gtdqiddmfe.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.guannengcc.top/gtiyqgrspk.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.ybcxt.top/gttwisshdp.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.fzhhl.top/gtxddwcimg.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.ppjwa.cn/gtqcccuize.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.xylfe.cn/gtrsfqwstb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.nwbrower.top/gtxpeqvnxh.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.wangdashe.top/gtcpihcfid.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.jlsjyb.cn/gttwfhojdf.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.shanyushiyangtech.top/gtnkawugol.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.cqqwz.cn/gtqyxucrko.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.andypj.xyz/gtjbhsyuvu.html

Q SQL 专题                              90
来源：http://hz.52xcode.cn/gthglxrytx.html

R Bash 专题                             80
来源：http://hz.aizwys.cn/gtivwpngfb.html

S C / C++ 专题                          60
来源：http://hz.tanke756.top/gtnzkaxagu.html

T 其他语言补充                          60
来源：http://hz.sufxvd.cn/gtblxsdcph.html

U 高频实用片段                         120
来源：http://hz.hysaishi.cn/gtpywvfehi.html

------------------------------------
来源：http://hz.xinyue.icu/gtflqaamtf.html

合计                                  2106 条
来源：http://hz.jianghu66.top/gtlkrjnkuy.html

--------------------------------------------------------------------------------
来源：http://hz.jiagoushi.top/gttunykatd.html

使用提醒
来源：http://hz.52xcode.cn/gtqqmuxuoi.html

--------------------------------------------------------------------------------
来源：http://hz.aibaodan.cn/gtsmwjcsux.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.smart0.xyz/gtexeskpoe.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.yj20258.top/gtskjeucca.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.yvedp.cn/gtgzlcwfia.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.bjfxy.top/gthibspmpw.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.xylfe.cn/gtolvqebrd.html

—— 文件结束 ——
来源：http://hz.yvedp.cn/gtwzntkgnl.html

================================================================================
来源：http://hz.ydzc1.top/gtserypska.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.jinqigfzy.top/gthxfrdlca.html

Common Programming Examples Cheat Book
来源：http://hz.smart0.xyz/gtrttlbfaz.html

================================================================================
来源：http://hz.guowangkeji.top/gtzjzautjd.html

【收录内容】
来源：http://hz.wangdashe.top/gtjkqhggon.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.jinyuanbaomall.cn/gtesfmpirz.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.shanyushiyangkeji.top/gtpmanrzgb.html

SQL · Bash · C · C++
来源：http://hz.cucudq.cn/gtyzrlkhnf.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.jiagoushi.top/gtrcxqhbzy.html

【使用说明】
来源：http://hz.jqgfzy.top/gtoaingpuk.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.daria6918.cn/gtjbgyzgwn.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.pengpengdd.cyou/gthpraqeui.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.ydjk.org.cn/gtveqvyjzv.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.zhengqikj.top/gtjbozrscy.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.yvedp.cn/gtonkcxbrx.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.0kj1m.cn/gtnomkdiry.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.yangfankeji.com/gtmdazygsc.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.aibaodan.cn/gtzbipbqmc.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.wangshuangyany.cn/gthjtubjqt.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.bjfxy.top/gtvvkxieum.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.snrcjt.cn/gtksgqawxe.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.jinqigufen.top/gtibkepjqn.html

【文件统计】
来源：http://hz.hnqzz.top/gtwxlrbrma.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.aizwys.cn/gtxzpadivg.html

--------------------------------------------------------------------------------
来源：http://hz.nwbrower.top/gtpynqxfql.html

目  录
来源：http://hz.ybcxt.top/gtrhmfqdbf.html

--------------------------------------------------------------------------------
来源：http://hz.kuanghao11.cn/gtswzgurql.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.jianghu66.top/gtwgkugkdm.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.jqgufenzy.top/gtzzubkbyl.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.52xcode.cn/gtjnjdhyys.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.shanyushiyangkeji.top/gtxrpmrlzi.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.yvedp.cn/gtmrvxufxp.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.quarkkingdee.top/gtrixuxjzt.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.gotoacloud.top/gtprgstuup.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.52xcode.cn/gtpricetkr.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.shzxlz.cn/gtgtxabejg.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.dianchejie.cn/gtmjmusuky.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.yueranfly.top/gtfhqtyarr.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.0kj1m.cn/gthmkentoe.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.ydzc1.top/gtdihfahaj.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.hongshengwenyu.top/gtqxnoroab.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.52xcode.cn/gtierkrlpi.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.jinqigufen.top/gtvlopdrqe.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.pengpengdd.cyou/gtrwyxxpth.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.ppjwa.cn/gtdzorfjvt.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.jqgfzy.top/gtcwfienrh.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hywenlv.cn/gtqmiwtdwn.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.316326.xyz/gtoxptkywv.html

================================================================================
来源：http://hz.tianlin.xyz/gtfkzuxeyh.html

A. 基础语法与类型
来源：http://hz.hfpthk.cn/gtjltylkwo.html

================================================================================
来源：http://hz.tian-w.cn/gtcqurxwab.html

[A01] Hello World
来源：http://hz.wangdashe.top/gtsmhocemn.html

Py:   print("Hello, World!")
来源：http://hz.zhijiandao.cn/gtcwiorekh.html

PHP:  echo "Hello, World!";
来源：http://hz.cqqwz.cn/gtktfdfckd.html

JS:   console.log("Hello, World!");
来源：http://hz.hywenlv.cn/gtmplqslpw.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.9152youxi.cn/gtviogitmm.html

Java: System.out.println("Hello, World!");
来源：http://hz.nwbrower.top/gtbqxrfkyc.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.wangshuangyany.cn/gtkjtppuhl.html

Ruby: puts "Hello, World!"
来源：http://hz.zycfv.cn/gtgamilaxj.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.xziqi.cn/gtjiguolgp.html

[A02] 变量声明与赋值
来源：http://hz.birdmap.top/gtefmqnnsj.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.sxryk.cn/gtjenttivr.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.guowangkeji.top/gtbpxurpjk.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.ivvv.top/gtpplumgqi.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.yuanzhike.top/gtzseaatfl.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.yvedp.cn/gtclhvkjmf.html

Go:   name := "Alex"; age := 20
来源：http://hz.shangyingyoupin.top/gtgqxratuh.html

Ruby: name = "Alex"; age = 20
来源：http://hz.quarkkingdee.top/gtqhoaucpt.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.yuxming.cn/gtchatzsad.html

[A03] 常量定义
来源：http://hz.cqqwz.cn/gtcmfwqoat.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.andypj.xyz/gtysnrrqcy.html

PHP:  const PI = 3.14159;
来源：http://hz.shanyushiyangkeji.top/gtjeubcqup.html

JS:   const PI = 3.14159;
来源：http://hz.aizwys.cn/gtwhzwmamm.html

TS:   const PI: number = 3.14159;
来源：http://hz.gzhubu.top/gtoeqoonll.html

Java: static final double PI = 3.14159;
来源：http://hz.9152youxi.cn/gtrgzbnnei.html

Go:   const PI = 3.14159
来源：http://hz.0kj1m.cn/gtunzjqpcd.html

Ruby: PI = 3.14159
来源：http://hz.sysykeji.top/gtkyehtcgw.html

C#:   const double PI = 3.14159;
来源：http://hz.jinqigfzy.top/gtklgqxwob.html

[A04] 判断变量类型
来源：http://hz.pycfn.com/gtudzdsphe.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.9152youxi.cn/gtqhjscbpy.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.hysaishi.cn/gtioooeesv.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.zdqjudy.top/gtoitgydsa.html

TS:   typeof x; x instanceof Date
来源：http://hz.tianlin.xyz/gtwvjqkqgd.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.dashuyun.cn/gthhtnlfmc.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.cheryme.top/gtcidyutgc.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.tian-w.cn/gtqozmfqae.html

C#:   x.GetType().Name; x is int
来源：http://hz.pengpengdd.cyou/gtyllswkxn.html

[A05] 整数除法与取模
来源：http://hz.kuanghao11.cn/gtwoaonbdl.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.52xcode.cn/gtkjtxjkvy.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.ydzc1.top/gtgfnqbdvi.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.cqqwz.cn/gtvdizxxkz.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.jinghuilouyu.cn/gteoldxhwm.html

Java: 7 / 2; 7 % 2
来源：http://hz.sysykeji.top/gtckvnlyne.html

Go:   7 / 2; 7 % 2
来源：http://hz.snrcjt.cn/gtvvfwacyz.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.xuanzx.com/gtnnelufrb.html

C#:   7 / 2; 7 % 2
来源：http://hz.nwbrower.top/gthiiqoaim.html

[A06] 字符串转数字
来源：http://hz.zdqjudy.top/gtobowiwoy.html

Py:   int("42"); float("3.14")
来源：http://hz.feifeiyinyue.top/gtekhfqrhz.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.c1oappe.top/gttjszixbx.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.316326.xyz/gtfzkgfglc.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.jinqigfzy.top/gtqshizmtj.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.52xcode.cn/gtzlbfgess.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.gaohongyu789.top/gttdbcnpth.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.iojbl.cn/gtrrodjlef.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.tian-w.cn/gtiyhvomgs.html

[A07] 数字转字符串
来源：http://hz.zhiwuduotai.top/gtjqllhsvk.html

Py:   str(42)
来源：http://hz.ehwqpu.com/gteycxogug.html

PHP:  (string) 42; strval(42)
来源：http://hz.jqgfzy.top/gtykgfcfeu.html

JS:   String(42); (42).toString()
来源：http://hz.xziqi.cn/gtwcxjjbav.html

TS:   String(42)
来源：http://hz.hywenlv.cn/gtdmdljziu.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.havefunace.top/gtpxuyyhee.html

Go:   strconv.Itoa(42)
来源：http://hz.zhaomingkeji.xyz/gtxkwkiqes.html

Ruby: 42.to_s
来源：http://hz.nwbrower.top/gtcweglgxh.html

C#:   42.ToString()
来源：http://hz.cdnleiting.top/gtgstlwkoh.html

[A08] 取整与四舍五入
来源：http://hz.jiagoushi.top/gtigcojwwp.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.shzxlz.cn/gtddwmrxkh.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.tanke756.top/gtdoryqkjs.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.yueranfly.top/gtivquctty.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.dashuyun.cn/gtchuvioml.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.ybcxt.top/gtiiushfwe.html


<!-- 参考信息 -->