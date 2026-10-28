代发 wailian999

[U57] PHP：字符串插值
来源：http://hz.hammf.cn/gttqbkbpig.html

"值: {$a}"
来源：http://hz.gotoacloud.top/gtuxftbdup.html

[U58] PHP：数组三件套
来源：http://hz.zycfv.cn/gtxsyyrrfz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.yvedp.cn/gtkudbsnzt.html

[U59] PHP：自定义排序
来源：http://hz.meibo888.top/gtyzmjrcij.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.316326.xyz/gtkzhofxlr.html

[U60] PHP：JSON 编解码
来源：http://hz.xylfe.cn/gtqruvjmhs.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.tian-w.cn/gtfjvprloo.html

[U61] PHP：正则
来源：http://hz.zhixingplan.top/gtnbbtdowa.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.jlsjyb.cn/gtaovzxnta.html

[U62] PHP：日期对象
来源：http://hz.chenjidiqi.icu/gtgioztsne.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.jianghu66.top/gtnbitixfy.html

[U63] PHP：文件读写
来源：http://hz.316326.xyz/gtplxhznfy.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.tanke756.top/gtbgznanjj.html

[U64] PHP：目录遍历
来源：http://hz.xylfe.cn/gtdvpypftx.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.xziqi.cn/gtisarnalr.html

[U65] PHP：会话
来源：http://hz.tian-w.cn/gtxpoautoc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.shangyingyoupin.top/gtrdmpfwih.html

[U66] PHP：设置 Cookie
来源：http://hz.gzhubu.top/gtzxnqfdsy.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.hammf.cn/gtjqfxtxgm.html

[U67] PHP：处理文件上传
来源：http://hz.yanxiufei.cn/gtqimkljcy.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.fengsongda.top/gtondlguoc.html

[U68] PHP：PDO 连接
来源：http://hz.pycfn.com/gtgyqqgbon.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.ybcxt.top/gtdezwkacd.html

[U69] PHP：PDO 预处理
来源：http://hz.hysaishi.cn/gtnmxyeshb.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.yuanzhike.top/gtwpazpyat.html

[U70] PHP：PDO 事务
来源：http://hz.tianlin.xyz/gtlkdkacqq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.aibaodan.cn/gtbogbqykp.html

[U71] PHP：抛出异常
来源：http://hz.zhixingplan.top/gtwxdrfxfg.html

throw new RuntimeException("失败", 500);
来源：http://hz.yj202588.top/gtozervuur.html

[U72] PHP：写错误日志
来源：http://hz.quarkkingdee.top/gtnbahkdmo.html

error_log("失败: " . $e->getMessage());
来源：http://hz.meibo888.top/gtwmqozkal.html

[U73] PHP：读取 ini 配置
来源：http://hz.xuetiantiany.cn/gtzrkbrdgd.html

parse_ini_file("config.ini", true)
来源：http://hz.hysaishi.cn/gtfrtufugj.html

[U74] PHP：读取环境变量
来源：http://hz.ybcxt.top/gthlccoivz.html

getenv("APP_ENV") ?: "production"
来源：http://hz.jqgufenzy.top/gtjpofhxas.html

[U75] PHP：依赖注入
来源：http://hz.yuanzhike.top/gttzkopcpe.html

composer require psr/container
来源：http://hz.yongpay.top/gtaettdtvu.html

[U76] PHP：简单路由
来源：http://hz.hywenlv.cn/gtngtmztzx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.xinyue.icu/gtxnmfucyd.html

[U77] PHP：模板渲染
来源：http://hz.quarkkingdee.top/gtltsfczeu.html

composer require twig/twig
来源：http://hz.havefunace.top/gtthrslryg.html

[U78] PHP：单元测试
来源：http://hz.jiagoushi.top/gtquqduomm.html

composer require --dev phpunit/phpunit
来源：http://hz.xylfe.cn/gtrftxnsvi.html

[U79] PHP：静态分析
来源：http://hz.chenlongwang.top/gtmubvjuci.html

composer require --dev phpstan/phpstan
来源：http://hz.tanke756.top/gtvcljrzbx.html

[U80] PHP：代码规范修复
来源：http://hz.jianghu66.top/gtsckixves.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.sufxvd.cn/gtfwfzdqrd.html

[U81] JS：初始化项目
来源：http://hz.hysaishi.cn/gtridulgpo.html

npm init -y;  npm i express
来源：http://hz.meibo888.top/gtfwujiuya.html

[U82] JS：package.json 脚本
来源：http://hz.ppjwa.cn/gtjkcmgprx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.yanxiufei.cn/gthyjugoqi.html

[U83] JS：ES Module 导入导出
来源：http://hz.jinghuilouyu.cn/gttrokkqcs.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.jqgufenzy.top/gtlgdqonmg.html

[U84] JS：CommonJS 写法
来源：http://hz.shangyingyoupin.top/gtwscdhmbr.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.ybcxt.top/gtstqajxyc.html

[U85] JS：可选链
来源：http://hz.jqgufenzy.top/gtqnhsvixn.html

a?.b?.c
来源：http://hz.smart0.xyz/gtsvcgxyby.html

[U86] JS：空值合并
来源：http://hz.zycfv.cn/gtypffnnxx.html

a ?? b
来源：http://hz.c1oappe.top/gtxwphiagd.html

[U87] JS：解构默认值
来源：http://hz.gotoacloud.top/gtuakricwr.html

const { a = 1, b = 2 } = obj;
来源：http://hz.nanxuanxn.top/gtkehtujyb.html

[U88] JS：对象展开合并
来源：http://hz.cashguo.top/gtlodxribw.html

{ ...a, ...b }
来源：http://hz.c1oappe.top/gthzeexssu.html

[U89] JS：数组去重
来源：http://hz.cqqwz.cn/gtfwmihtdy.html

[...new Set(arr)]
来源：http://hz.zhengqikj.top/gtlgupcyuc.html

[U90] JS：数字数组排序
来源：http://hz.xziqi.cn/gtiaynniso.html

[...arr].sort((a, b) => a - b)
来源：http://hz.sysykeji.top/gtxrmcxobo.html

[U91] JS：对象键值遍历
来源：http://hz.jqgfzy.top/gtxccdvvup.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.svipenyu.cn/gtqdswgjaa.html

[U92] JS：深拷贝
来源：http://hz.hnxiangtu.top/gtadvnaoyu.html

structuredClone(obj)
来源：http://hz.mhx1999.top/gtkfpflbwk.html

[U93] JS：模板字符串
来源：http://hz.jyoumei.cn/gtibtpqjcz.html

`共 ${n} 条`
来源：http://hz.hywenlv.cn/gtdzhbjugv.html

[U94] JS：箭头函数
来源：http://hz.ehwqpu.com/gtwvellwhw.html

const double = x => x * 2;
来源：http://hz.yj20258888.top/gtxbhjfsbe.html

[U95] JS：Promise 包装
来源：http://hz.gzhubu.top/gtljobwpli.html

new Promise((resolve, reject) => {})
来源：http://hz.jlsjyb.cn/gtfxxwlzop.html

[U96] JS：async/await 与异常
来源：http://hz.jianghu66.top/gtjeexgkvp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.yj202588.top/gtzwgdqxeb.html

[U97] JS：并发请求
来源：http://hz.hfpthk.cn/gtelqtgdey.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yuanzhike.top/gtifpardwi.html

[U98] JS：fetch 带 JSON
来源：http://hz.hywenlv.cn/gtmreabcmp.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.hfpthk.cn/gtujxlhnmd.html

[U99] JS：事件监听
来源：http://hz.c1oappe.top/gtjftbdceh.html

el.addEventListener("click", e => {})
来源：http://hz.gzhubu.top/gtxgaygulz.html

[U100] JS：DOM 查询
来源：http://hz.chenjidiqi.icu/gtcgbtfwzm.html

document.querySelector(".item")
来源：http://hz.hammf.cn/gthnutnhtc.html

[U101] JS：classList 操作
来源：http://hz.jqgfzy.top/gtpqtxmdah.html

el.classList.toggle("active")
来源：http://hz.cqqwz.cn/gtpawxewvd.html

[U102] JS：本地存储
来源：http://hz.nanxuanxn.top/gttenmnaou.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.tianlin.xyz/gtofpzliwk.html

[U103] JS：定时器
来源：http://hz.c1oappe.top/gtbvgujdwc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.ywan-chungtsiang.top/gttrsjyjfp.html

[U104] JS：防抖
来源：http://hz.cucudq.cn/gtdmduskhk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.tian-w.cn/gtflqmwdpt.html

[U105] JS：节流
来源：http://hz.jyoumei.cn/gttotftjan.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.xuanzx.com/gtyrhynelk.html

[U106] JS：日期格式化
来源：http://hz.hysaishi.cn/gtwrlkzelo.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yonumen.top/gtvuuwyuts.html

[U107] JS：数字千分位
来源：http://hz.dashuyun.cn/gtanbifqpi.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.jiagoushi.top/gtkichtzjd.html

[U108] JS：随机整数
来源：http://hz.pycfn.com/gtyygedoli.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.jqgufenzy.top/gtqxfzqsus.html

[U109] JS：数组分组
来源：http://hz.yvedp.cn/gtdwqygxmv.html

Object.groupBy(arr, x => x.type)
来源：http://hz.xziqi.cn/gtuvwiefnd.html

[U110] JS：数组分块
来源：http://hz.zhoulong.xyz/gtfendvnwb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.jyoumei.cn/gtmxlnvvzj.html

[U111] JS：对象转 Map
来源：http://hz.jiagoushi.top/gtuesxbqqg.html

new Map(Object.entries(obj))
来源：http://hz.daria6918.cn/gtbminandn.html

[U112] JS：字符串补位
来源：http://hz.svipenyu.cn/gtmbdurvgi.html

"7".padStart(3, "0")
来源：http://hz.sufxvd.cn/gtyinstbpm.html

[U113] JS：正则替换全部
来源：http://hz.wangdashe.top/gtwbsylyjk.html

s.replaceAll("a", "b")
来源：http://hz.nanxuanxn.top/gthkenzjvc.html

[U114] JS：JSON 深比较
来源：http://hz.chenjidiqi.icu/gtjrgqqhte.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jlsjyb.cn/gtkhabkwia.html

[U115] JS：生成 UUID
来源：http://hz.xylfe.cn/gtoqrfhops.html

crypto.randomUUID()
来源：http://hz.yj20258888.top/gtncwwsexu.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.shanyushiyangtech.top/gtdcuhgdjt.html

/** @param {string} name */ function f(name) {}
来源：http://hz.daxiang520.top/gtzpufuiga.html

[U117] JS：单元测试
来源：http://hz.sweek.top/gtuhgrhuyw.html

npm i -D vitest;  npx vitest
来源：http://hz.shangyingyoupin.top/gtxrkxbwyc.html

[U118] JS：开发服务器
来源：http://hz.shanyushiyangkeji.top/gtiihpgvvu.html

npm i -D vite;  npx vite
来源：http://hz.jinqigufen.top/gtxdhhsztj.html

[U119] JS：生产构建
来源：http://hz.sweek.top/gtskgjtrre.html

npx vite build
来源：http://hz.sufxvd.cn/gtybctdqsp.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.zhoulong.xyz/gtydibysai.html

import.meta.env.VITE_API_URL
来源：http://hz.pycfn.com/gtlhfbpqlc.html

================================================================================
来源：http://hz.meibo888.top/gtjzufujpc.html

统计汇总
来源：http://hz.zhaomingkeji.xyz/gtclxdhujx.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtpbjtzuvn.html

按语言统计（条）：
来源：http://hz.zhijiandao.cn/gtlakqvkve.html

Python ......... 252
来源：http://hz.zycfv.cn/gtnpttasyj.html

PHP ............ 252
来源：http://hz.haohaochexian.top/gtqlgabjrm.html

JavaScript ..... 252
来源：http://hz.cashguo.top/gtjjiitjeo.html

TypeScript ..... 212
来源：http://hz.jinyuanbaomall.cn/gtbkehppjz.html

Java ........... 212
来源：http://hz.daxiang520.top/gthgshwefq.html

Go ............. 212
来源：http://hz.zycfv.cn/gtygglowuv.html

Ruby ........... 212
来源：http://hz.shzxlz.cn/gtnrcnsapk.html

C# ............. 212
来源：http://hz.jinyuanbaomall.cn/gturyoucep.html

C .............. 30
来源：http://hz.pengpengdd.cyou/gthbwcaito.html

C++ ............ 30
来源：http://hz.0kj1m.cn/gtzmjnpetp.html

SQL ............ 90
来源：http://hz.zhengqikj.top/gtqdfhgovf.html

Bash ........... 80
来源：http://hz.zdqjudy.top/gtdnqpmycd.html

Kotlin ......... 15
来源：http://hz.c1oappe.top/gtkzbfxwpr.html

Swift .......... 15
来源：http://hz.meibo888.top/gtxxjqixib.html

Lua ............ 10
来源：http://hz.yj20258.top/gtccsbxeqr.html

Perl ........... 10
来源：http://hz.vqdsnc.cn/gtsbclllvz.html

Scala .......... 10
来源：http://hz.dianchejie.cn/gtomaiommj.html

------------------------------------
来源：http://hz.yonumen.top/gtnhllpiwj.html

合计 ........... 2106 条
来源：http://hz.zhoulong.xyz/gtxqzqqdzi.html

按章节统计：
来源：http://hz.ywan-chungtsiang.top/gtkteqowlm.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.iojbl.cn/gtxtlfqrtq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.tanke756.top/gtshldttkd.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.316326.xyz/gtmzpzlhuv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.andypj.xyz/gtzhlonwzd.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.quarkkingdee.top/gtqfqhvbba.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.daxiang520.top/gtjbdoxohe.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.guowangkeji.top/gtciqgdqhx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.ydzc1.top/gtroqhwttl.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.vqdsnc.cn/gtspwonmmb.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.chenlongwang.top/gtloybkekl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.jlsjyb.cn/gtzgkpbfgj.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.snrcjt.cn/gtcsvbdrnq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.316326.xyz/gtrzhlttly.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.jiagoushi.top/gtnmjanoiu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.shanyushiyangtech.top/gtdicfcfco.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.jinqigfzy.top/gtsbssfiuo.html

Q SQL 专题                              90
来源：http://hz.sysykeji.top/gtuhlychuc.html

R Bash 专题                             80
来源：http://hz.hongshengwenyu.top/gtndrvgylh.html

S C / C++ 专题                          60
来源：http://hz.zhiwuduotai.top/gtwqjrokrs.html

T 其他语言补充                          60
来源：http://hz.jinghuilouyu.cn/gtubdvrhzm.html

U 高频实用片段                         120
来源：http://hz.iojbl.cn/gtnjlbvswc.html

------------------------------------
来源：http://hz.jiagoushi.top/gtoyezudnu.html

合计                                  2106 条
来源：http://hz.wangshuangyany.cn/gtumszrwgx.html

--------------------------------------------------------------------------------
来源：http://hz.9152youxi.cn/gtinojbzeh.html

使用提醒
来源：http://hz.ppjwa.cn/gtvqotkeak.html

--------------------------------------------------------------------------------
来源：http://hz.jinyuanbaomall.cn/gtvungfvss.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.xuanzx.com/gtdnhllnut.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.iojbl.cn/gtpsrcfxkb.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.jianghu66.top/gthghpmkpb.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.daria6918.cn/gtgwldjbwp.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.sysykeji.top/gtqvcspiww.html

—— 文件结束 ——
来源：http://hz.zdqjudy.top/gtzaltahef.html

================================================================================
来源：http://hz.dianchejie.cn/gtzzvpzmvg.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.tian-w.cn/gteyawjhcm.html

Common Programming Examples Cheat Book
来源：http://hz.yanxiufei.cn/gtomewtewu.html

================================================================================
来源：http://hz.ivvv.top/gtkwrlbpdp.html

【收录内容】
来源：http://hz.wangdashe.top/gtggjtggxu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.sysykeji.top/gtsloqxmwt.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.yj202588.top/gtknxufisw.html

SQL · Bash · C · C++
来源：http://hz.wangshuangyany.cn/gtlhhuadze.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.chenjidiqi.icu/gtsflrpruq.html

【使用说明】
来源：http://hz.ywan-chungtsiang.top/gtzwroppdw.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.nwbrower.top/gtwqhrgoyf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.havefunace.top/gtnykspgjt.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.andypj.xyz/gtpygzuwyt.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.52xcode.cn/gtzpdusyvi.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.sysykeji.top/gteqggwcla.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.yonumen.top/gtdltswgyz.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.xingfuxueyuan.xyz/gtfkritoso.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.gotoacloud.top/gtkpzjxpvz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.tanke756.top/gtiazpbnxp.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.jiagoushi.top/gtlbnnngyd.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.jqgufenzy.top/gtbxkdkxua.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.daria6918.cn/gtpulleizr.html

【文件统计】
来源：http://hz.zhoulong.xyz/gtbxuvwxad.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.zhixingplan.top/gtkdkvxoez.html

--------------------------------------------------------------------------------
来源：http://hz.xingfuxueyuan.xyz/gtbmsnfumb.html

目  录
来源：http://hz.jianghu66.top/gtfnrqngcm.html

--------------------------------------------------------------------------------
来源：http://hz.gotoacloud.top/gtqwmrsxni.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.vqdsnc.cn/gtckcyebcr.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.xylfe.cn/gtlruzbggg.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.shuidangran.top/gtnxgxlpft.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.0kj1m.cn/gtbahgmphi.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.havefunace.top/gtfieadogq.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.guannengcc.top/gtcxjzgxdf.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.nanxuanxn.top/gttpztazey.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.hammf.cn/gtgfgdkvxg.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.xziqi.cn/gtebfulhni.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.zhengqikj.top/gtgtcapmjy.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.shangyingyoupin.top/gtcznaldvk.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.ydzc1.top/gtvuuglldd.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.hnxiangtu.top/gtzltpjoqk.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.yongpay.top/gtckwxbktg.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.jianghu66.top/gtdbivgyav.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.yonumen.top/gtqamokmek.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.jlsjyb.cn/gtmqfqzpas.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.sxryk.cn/gtbzfnpkbd.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.zhongyouzk.top/gtxjmmizef.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.xylfe.cn/gtpddiuxik.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.quarkkingdee.top/gtbwtqvmey.html

================================================================================
来源：http://hz.ydzc1.top/gtuzdrrtvs.html

A. 基础语法与类型
来源：http://hz.wangshuangyany.cn/gtdklafwtu.html

================================================================================
来源：http://hz.zycfv.cn/gtjaclhtky.html

[A01] Hello World
来源：http://hz.hysaishi.cn/gtwnkliadp.html

Py:   print("Hello, World!")
来源：http://hz.yj20258888.top/gtvywzptwq.html

PHP:  echo "Hello, World!";
来源：http://hz.aizwys.cn/gtbupqnmcp.html

JS:   console.log("Hello, World!");
来源：http://hz.xylfe.cn/gtkfkwnhfz.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.chenlongwang.top/gtxkncsijr.html

Java: System.out.println("Hello, World!");
来源：http://hz.svipenyu.cn/gtxkpctuei.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.shanyushiyangtech.top/gtfxdbyuvy.html

Ruby: puts "Hello, World!"
来源：http://hz.hongshengwenyu.top/gtvtezvlpj.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.sufxvd.cn/gtdhcapfwl.html

[A02] 变量声明与赋值
来源：http://hz.jqgufenzy.top/gteebwxmwk.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.wangdashe.top/gtumuxvxzx.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.xuetiantiany.cn/gtnhgzwjhb.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.cdnleiting.top/gtfsawhrml.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.yuanzhike.top/gtcpjxljqc.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.tanke756.top/gtyyalbudo.html

Go:   name := "Alex"; age := 20
来源：http://hz.ivvv.top/gtkocqvjyq.html

Ruby: name = "Alex"; age = 20
来源：http://hz.chenlongwang.top/gtgpcbepuw.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.mhx1999.top/gtyypisxul.html

[A03] 常量定义
来源：http://hz.cqqwz.cn/gtgjnihyfj.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.nwbrower.top/gtguwylubr.html

PHP:  const PI = 3.14159;
来源：http://hz.guannengcc.top/gtjqykbpyn.html

JS:   const PI = 3.14159;
来源：http://hz.sufxvd.cn/gtsxrubdoy.html

TS:   const PI: number = 3.14159;
来源：http://hz.ehwqpu.com/gttwhkanzn.html

Java: static final double PI = 3.14159;
来源：http://hz.jinqigufen.top/gtgzegaaiy.html

Go:   const PI = 3.14159
来源：http://hz.ehwqpu.com/gtvedrnjcj.html

Ruby: PI = 3.14159
来源：http://hz.zhengqikj.top/gtwywhhabb.html

C#:   const double PI = 3.14159;
来源：http://hz.zycfv.cn/gtpvqmzbsm.html

[A04] 判断变量类型
来源：http://hz.vqdsnc.cn/gtupsaglif.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.jlsjyb.cn/gtpaiaxknf.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.xingfuxueyuan.xyz/gtzgrkuifa.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.pycfn.com/gtsxsadtsi.html

TS:   typeof x; x instanceof Date
来源：http://hz.yuxming.cn/gthvhnnequ.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.shanyushiyangtech.top/gtrtvhzrtw.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.andypj.xyz/gtrydoahcw.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.haohaochexian.top/gtozremaph.html

C#:   x.GetType().Name; x is int
来源：http://hz.sysykeji.top/gtimdtyedh.html

[A05] 整数除法与取模
来源：http://hz.cucudq.cn/gtlzltaswc.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.52xcode.cn/gtuwfofstq.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.jianghu66.top/gtgghdcuzd.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.zhoulong.xyz/gtaqhplxxy.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.chenzaomai.com/gtshnuitlj.html

Java: 7 / 2; 7 % 2
来源：http://hz.svipenyu.cn/gtitbdjylx.html

Go:   7 / 2; 7 % 2
来源：http://hz.xziqi.cn/gtgmjgexmp.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.tian-w.cn/gtrjkxgqit.html

C#:   7 / 2; 7 % 2
来源：http://hz.nwbrower.top/gtfgmavfuq.html

[A06] 字符串转数字
来源：http://hz.jianghu66.top/gtjbghaqsh.html

Py:   int("42"); float("3.14")
来源：http://hz.aizwys.cn/gthamfxqoi.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.yongpay.top/gtpctboppd.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.cqqwz.cn/gtdxciwddq.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.wangdashe.top/gthbecapon.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.shanyushiyangkeji.top/gthpgwqyun.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.xziqi.cn/gteekkhtij.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.yueranfly.top/gtrjmtybsd.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.jianghu66.top/gtnnbhscai.html

[A07] 数字转字符串
来源：http://hz.jinqigfzy.top/gtsigaruwz.html

Py:   str(42)
来源：http://hz.haohaochexian.top/gtqlpwlgux.html

PHP:  (string) 42; strval(42)
来源：http://hz.xuanzx.com/gtgwbvzxzu.html

JS:   String(42); (42).toString()
来源：http://hz.cdnleiting.top/gtydhnwaos.html

TS:   String(42)
来源：http://hz.andypj.xyz/gtqkusjzes.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.zycfv.cn/gtoheqzbdo.html

Go:   strconv.Itoa(42)
来源：http://hz.chenjidiqi.icu/gtfhgvbdsq.html

Ruby: 42.to_s
来源：http://hz.nwbrower.top/gtcfabruux.html

C#:   42.ToString()
来源：http://hz.ivvv.top/gtgliegxvl.html

[A08] 取整与四舍五入
来源：http://hz.sysykeji.top/gtcgtwdmau.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.xziqi.cn/gtagxtvpyw.html


<!-- 参考信息 -->