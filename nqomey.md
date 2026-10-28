代发 wailian999

[U57] PHP：字符串插值
来源：http://hz.dianchejie.cn/gtekurgoxo.html

"值: {$a}"
来源：http://hz.yangfankeji.com/gtamtjevyf.html

[U58] PHP：数组三件套
来源：http://hz.hfpthk.cn/gtgdtrkwjo.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.chenlongwang.top/gthvbthgjs.html

[U59] PHP：自定义排序
来源：http://hz.chenjidiqi.icu/gtdmshwpkb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jiagoushi.top/gtykbzsbxm.html

[U60] PHP：JSON 编解码
来源：http://hz.gogol.net.cn/gtljnhejjm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.ydzc1.top/gtebcgdnvn.html

[U61] PHP：正则
来源：http://hz.c1oappe.top/gtagwolywo.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.xziqi.cn/gtyfbaipsa.html

[U62] PHP：日期对象
来源：http://hz.jinghuilouyu.cn/gtdclgnskw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.xuanzx.com/gtaygmdggx.html

[U63] PHP：文件读写
来源：http://hz.shanyushiyangkeji.top/gteqvyiqfo.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.jqgufenzy.top/gtxdlkgzjm.html

[U64] PHP：目录遍历
来源：http://hz.shangyingyoupin.top/gtfdzwazfr.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.ydzc1.top/gtqiamqxto.html

[U65] PHP：会话
来源：http://hz.iojbl.cn/gtsthcreet.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.redwolf501.top/gttlkndwnw.html

[U66] PHP：设置 Cookie
来源：http://hz.xziqi.cn/gtaqyeypmv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.yj20258.top/gtmoaoqbwk.html

[U67] PHP：处理文件上传
来源：http://hz.yvedp.cn/gtamseljio.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.xingfuxueyuan.xyz/gtbwqvubqz.html

[U68] PHP：PDO 连接
来源：http://hz.snrcjt.cn/gtbhkzuagi.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.xingfuxueyuan.xyz/gtpdyvaxke.html

[U69] PHP：PDO 预处理
来源：http://hz.hnqzz.top/gtvqiljrzf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.iojbl.cn/gtzekmxixj.html

[U70] PHP：PDO 事务
来源：http://hz.jlsjyb.cn/gtymfwquql.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.zhengqikj.top/gtspakelju.html

[U71] PHP：抛出异常
来源：http://hz.iojbl.cn/gtfykptppo.html

throw new RuntimeException("失败", 500);
来源：http://hz.zycfv.cn/gtpyacvrta.html

[U72] PHP：写错误日志
来源：http://hz.jiagoushi.top/gteqaipexn.html

error_log("失败: " . $e->getMessage());
来源：http://hz.gzhubu.top/gtwzocqiza.html

[U73] PHP：读取 ini 配置
来源：http://hz.xingfuxueyuan.xyz/gtawxlvxwk.html

parse_ini_file("config.ini", true)
来源：http://hz.zhoulong.xyz/gtnxpiwgwr.html

[U74] PHP：读取环境变量
来源：http://hz.birdmap.top/gtfrujwevz.html

getenv("APP_ENV") ?: "production"
来源：http://hz.yj20258.top/gtmevlxvwi.html

[U75] PHP：依赖注入
来源：http://hz.daria6918.cn/gtcunuhgfx.html

composer require psr/container
来源：http://hz.ybcxt.top/gtdkhejzni.html

[U76] PHP：简单路由
来源：http://hz.iojbl.cn/gtqpvzuvxo.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.cdnleiting.top/gtyxemmbgx.html

[U77] PHP：模板渲染
来源：http://hz.mhx1999.top/gtdcdvnqmw.html

composer require twig/twig
来源：http://hz.xingfuxueyuan.xyz/gtvewtueqe.html

[U78] PHP：单元测试
来源：http://hz.sufxvd.cn/gtmrnuhxci.html

composer require --dev phpunit/phpunit
来源：http://hz.zhoulong.xyz/gthctqjzhx.html

[U79] PHP：静态分析
来源：http://hz.yueranfly.top/gtipfethfg.html

composer require --dev phpstan/phpstan
来源：http://hz.snrcjt.cn/gtdodroctm.html

[U80] PHP：代码规范修复
来源：http://hz.jinyuanbaomall.cn/gtkajzfqyp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.dianchejie.cn/gtmmkdrckv.html

[U81] JS：初始化项目
来源：http://hz.yj20258.top/gtfjmxdyfe.html

npm init -y;  npm i express
来源：http://hz.hammf.cn/gthekobpjb.html

[U82] JS：package.json 脚本
来源：http://hz.birdmap.top/gtftjwonkv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.shanyushiyangkeji.top/gtmriwyzfj.html

[U83] JS：ES Module 导入导出
来源：http://hz.sweek.top/gtwooiqtij.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.jqgfzy.top/gtrebjcgrg.html

[U84] JS：CommonJS 写法
来源：http://hz.9152youxi.cn/gtpvheimkf.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.gotoacloud.top/gtcltbpvlx.html

[U85] JS：可选链
来源：http://hz.bjfxy.top/gtcmvkwyyj.html

a?.b?.c
来源：http://hz.316326.xyz/gtbvveovau.html

[U86] JS：空值合并
来源：http://hz.ivvv.top/gtqlcgrlxx.html

a ?? b
来源：http://hz.ivvv.top/gtvlbejvim.html

[U87] JS：解构默认值
来源：http://hz.dashuyun.cn/gtyfwkvxwt.html

const { a = 1, b = 2 } = obj;
来源：http://hz.cashguo.top/gtyirgvjzh.html

[U88] JS：对象展开合并
来源：http://hz.ppjwa.cn/gtvoejwngu.html

{ ...a, ...b }
来源：http://hz.ybcxt.top/gtjdavrmlf.html

[U89] JS：数组去重
来源：http://hz.ydzc1.top/gtoqjhjrdx.html

[...new Set(arr)]
来源：http://hz.guowangkeji.top/gtoldaonte.html

[U90] JS：数字数组排序
来源：http://hz.cheryme.top/gtbywdoxci.html

[...arr].sort((a, b) => a - b)
来源：http://hz.jinqigufen.top/gtjmtytedh.html

[U91] JS：对象键值遍历
来源：http://hz.gaohongyu789.top/gtanlrjeso.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.cucudq.cn/gtoklofxti.html

[U92] JS：深拷贝
来源：http://hz.xziqi.cn/gtecqghxmb.html

structuredClone(obj)
来源：http://hz.zhongyouzk.top/gtagssfrtv.html

[U93] JS：模板字符串
来源：http://hz.xinyue.icu/gtovvwrwvx.html

`共 ${n} 条`
来源：http://hz.smart0.xyz/gtedfpxfdk.html

[U94] JS：箭头函数
来源：http://hz.fzhhl.top/gtxojdpaeu.html

const double = x => x * 2;
来源：http://hz.zhiwuduotai.top/gtkcuhhbjb.html

[U95] JS：Promise 包装
来源：http://hz.316326.xyz/gtabxdkpus.html

new Promise((resolve, reject) => {})
来源：http://hz.jqgufenzy.top/gtnvutszhz.html

[U96] JS：async/await 与异常
来源：http://hz.wangdashe.top/gtorlihzpu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.bjfxy.top/gtmsbsdnhd.html

[U97] JS：并发请求
来源：http://hz.yonumen.top/gtatpyhtqr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xingfuxueyuan.xyz/gtzbyyotde.html

[U98] JS：fetch 带 JSON
来源：http://hz.hfpthk.cn/gteslbpktg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.yvedp.cn/gtrdbezggy.html

[U99] JS：事件监听
来源：http://hz.mhx1999.top/gtnkqrlyet.html

el.addEventListener("click", e => {})
来源：http://hz.xingfuxueyuan.xyz/gtcmnztaxc.html

[U100] JS：DOM 查询
来源：http://hz.shangyingyoupin.top/gtmgmjbsbr.html

document.querySelector(".item")
来源：http://hz.xuanzx.com/gthimbyzzs.html

[U101] JS：classList 操作
来源：http://hz.hongshengwenyu.top/gtkoecqfzm.html

el.classList.toggle("active")
来源：http://hz.yvedp.cn/gttycbnier.html

[U102] JS：本地存储
来源：http://hz.feifeiyinyue.top/gtifhbvpzj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.gogol.net.cn/gtxuldmocl.html

[U103] JS：定时器
来源：http://hz.9152youxi.cn/gtolpkwube.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.hammf.cn/gtplkecuhm.html

[U104] JS：防抖
来源：http://hz.yvedp.cn/gtdrdohhee.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xuanzx.com/gtvenxezlj.html

[U105] JS：节流
来源：http://hz.shuidangran.top/gtcbislztc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.nanxuanxn.top/gtaevskfne.html

[U106] JS：日期格式化
来源：http://hz.daria6918.cn/gtabzugjvn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.xuanzx.com/gtpsjwbbij.html

[U107] JS：数字千分位
来源：http://hz.52xcode.cn/gtwcfuacjy.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.jlsjyb.cn/gtesyurzby.html

[U108] JS：随机整数
来源：http://hz.nwbrower.top/gtaassxylo.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.hongshengwenyu.top/gtfewqaout.html

[U109] JS：数组分组
来源：http://hz.gzhubu.top/gtpepekwaj.html

Object.groupBy(arr, x => x.type)
来源：http://hz.jinghuilouyu.cn/gtuoxamyie.html

[U110] JS：数组分块
来源：http://hz.vqdsnc.cn/gtdkminzlx.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.chenjidiqi.icu/gtgxnqafwn.html

[U111] JS：对象转 Map
来源：http://hz.jinqigfzy.top/gtyenfcgwt.html

new Map(Object.entries(obj))
来源：http://hz.jinyuanbaomall.cn/gtnxuvhpws.html

[U112] JS：字符串补位
来源：http://hz.guowangkeji.top/gtduqkfxny.html

"7".padStart(3, "0")
来源：http://hz.wangdashe.top/gtwubultfc.html

[U113] JS：正则替换全部
来源：http://hz.shuidangran.top/gtmnanvcxe.html

s.replaceAll("a", "b")
来源：http://hz.c1oappe.top/gttlatbepa.html

[U114] JS：JSON 深比较
来源：http://hz.yvedp.cn/gtwcndwbdy.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhengqikj.top/gtagthyanh.html

[U115] JS：生成 UUID
来源：http://hz.dashuyun.cn/gtwukyuodh.html

crypto.randomUUID()
来源：http://hz.pengpengdd.cyou/gtzrmhunxt.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.ybcxt.top/gtiokqjgce.html

/** @param {string} name */ function f(name) {}
来源：http://hz.vqdsnc.cn/gtgccjaqgt.html

[U117] JS：单元测试
来源：http://hz.9152youxi.cn/gteitddwus.html

npm i -D vitest;  npx vitest
来源：http://hz.yj202588.top/gtwxhbsoyh.html

[U118] JS：开发服务器
来源：http://hz.fzhhl.top/gtgijihwhj.html

npm i -D vite;  npx vite
来源：http://hz.xziqi.cn/gthzjwhjes.html

[U119] JS：生产构建
来源：http://hz.gzhubu.top/gtzcwlacuw.html

npx vite build
来源：http://hz.aizwys.cn/gtejehbvgw.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.jqgufenzy.top/gtxgkrcgul.html

import.meta.env.VITE_API_URL
来源：http://hz.sysykeji.top/gtmqcugoac.html

================================================================================
来源：http://hz.cqqwz.cn/gtikqpbebg.html

统计汇总
来源：http://hz.nwbrower.top/gtthkgtduf.html

================================================================================
来源：http://hz.yj202588.top/gtmqvcgywp.html

按语言统计（条）：
来源：http://hz.daria6918.cn/gtftompqlv.html

Python ......... 252
来源：http://hz.nanxinkj.top/gtuckathxf.html

PHP ............ 252
来源：http://hz.hywenlv.cn/gtijabylxz.html

JavaScript ..... 252
来源：http://hz.zhongyouzk.top/gtfytbjeys.html

TypeScript ..... 212
来源：http://hz.wangdashe.top/gtxbrramdn.html

Java ........... 212
来源：http://hz.quarkkingdee.top/gtxlevklsn.html

Go ............. 212
来源：http://hz.cucudq.cn/gtkvzidkff.html

Ruby ........... 212
来源：http://hz.wangdashe.top/gtikklatev.html

C# ............. 212
来源：http://hz.hnqzz.top/gtdaccmgva.html

C .............. 30
来源：http://hz.xinyue.icu/gtyduomqxo.html

C++ ............ 30
来源：http://hz.jiagoushi.top/gtlzfnecoe.html

SQL ............ 90
来源：http://hz.jyoumei.cn/gtuqkigxmr.html

Bash ........... 80
来源：http://hz.jinqigufen.top/gthmobdfjl.html

Kotlin ......... 15
来源：http://hz.iojbl.cn/gtvzckdfvm.html

Swift .......... 15
来源：http://hz.quarkkingdee.top/gtcsxkdkhy.html

Lua ............ 10
来源：http://hz.smart0.xyz/gtgozmtlix.html

Perl ........... 10
来源：http://hz.jiagoushi.top/gtweyyuugg.html

Scala .......... 10
来源：http://hz.fengsongda.top/gtbqfeqbvq.html

------------------------------------
来源：http://hz.fengsongda.top/gtmvaanjzm.html

合计 ........... 2106 条
来源：http://hz.tian-w.cn/gtieerjimh.html

按章节统计：
来源：http://hz.wangdashe.top/gtfrfkggsk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.mhx1999.top/gtsqxtbqbo.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.daxiang520.top/gtlorzvqmc.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.yueranfly.top/gtaimxorku.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.hnqzz.top/gtmyfklofj.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.tian-w.cn/gtnnxqnafj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.yonumen.top/gtcgdzhkjs.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.feifeiyinyue.top/gtuxomnjbu.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.nanxuanxn.top/gtkbouwpdr.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.tanke756.top/gttgnzbpjf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.ppjwa.cn/gtncinagng.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.aibaodan.cn/gtozvwuuez.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.dianchejie.cn/gtoswpljyi.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.iojbl.cn/gtxxzwbsxr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.jinghuilouyu.cn/gtddzlkqlg.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.jyoumei.cn/gtifaaavtw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.svipenyu.cn/gteeqkmthb.html

Q SQL 专题                              90
来源：http://hz.wangdashe.top/gtkjyeefvi.html

R Bash 专题                             80
来源：http://hz.chenlongwang.top/gtgsaxonnd.html

S C / C++ 专题                          60
来源：http://hz.hysaishi.cn/gtqvzlatve.html

T 其他语言补充                          60
来源：http://hz.jinyuanbaomall.cn/gtdvioqsox.html

U 高频实用片段                         120
来源：http://hz.shangyingyoupin.top/gtxartfpgm.html

------------------------------------
来源：http://hz.cdnleiting.top/gtrwwsiife.html

合计                                  2106 条
来源：http://hz.jqgfzy.top/gtctgrwxhh.html

--------------------------------------------------------------------------------
来源：http://hz.guowangkeji.top/gtfbtuhvzh.html

使用提醒
来源：http://hz.wangshuangyany.cn/gtnbshvrzg.html

--------------------------------------------------------------------------------
来源：http://hz.0kj1m.cn/gtrkjxefwu.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.xinyue.icu/gtionegjlh.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.gzhubu.top/gtvkhgrsqd.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.gzhubu.top/gtdblsbkcr.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.hysaishi.cn/gtharzvwdj.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.cucudq.cn/gtptjakqdr.html

—— 文件结束 ——
来源：http://hz.xuanzx.com/gtnyfxeyba.html

================================================================================
来源：http://hz.ehwqpu.com/gtamvrtfyg.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.ywan-chungtsiang.top/gtodmtrnen.html

Common Programming Examples Cheat Book
来源：http://hz.yanxiufei.cn/gtqqewjmyg.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtojhlrvfa.html

【收录内容】
来源：http://hz.xuetiantiany.cn/gtzkcssfhk.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.yanxiufei.cn/gthkjxcogh.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.tianlin.xyz/gtwzqyspyl.html

SQL · Bash · C · C++
来源：http://hz.smart0.xyz/gtubvhdcjl.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.jqgfzy.top/gtftfimdnt.html

【使用说明】
来源：http://hz.ehwqpu.com/gtwshcqtnt.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.316326.xyz/gttqhwcvdj.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.yongpay.top/gthwgliqhz.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.chenzaomai.com/gtemmmjecj.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.cdnleiting.top/gtqutotpkf.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.zhaomingkeji.xyz/gttwrdovzf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.jinghuilouyu.cn/gtdyzyoeyt.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.yonumen.top/gtmqcphmhg.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.yuanzhike.top/gtkjpqygft.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.hysaishi.cn/gtfqgesliv.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.ppjwa.cn/gtfjutlswr.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.tian-w.cn/gtackznfkz.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.cucudq.cn/gtdhnlvoea.html

【文件统计】
来源：http://hz.fengsongda.top/gtggautlij.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.birdmap.top/gtbzuafzcr.html

--------------------------------------------------------------------------------
来源：http://hz.haohaochexian.top/gtakjwoqtb.html

目  录
来源：http://hz.yj20258.top/gtehrbvuhe.html

--------------------------------------------------------------------------------
来源：http://hz.hysaishi.cn/gtpygzmwjo.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.hongshengwenyu.top/gtdtqsjucp.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.daxiang520.top/gtrteikdkd.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.jqgufenzy.top/gtndjrisyc.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.jianghu66.top/gtfomlwwtj.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.zhoulong.xyz/gtqohcruav.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.zhiwuduotai.top/gtonvwmdxz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.sweek.top/gthvmfyuvk.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.xuanzx.com/gtxrmbjtxy.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.sufxvd.cn/gtoakrdsjy.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.aibaodan.cn/gtajxukstg.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.chenzaomai.com/gthhukhfad.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.yuxming.cn/gtvqmcoitd.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.hnqzz.top/gtrfdusecj.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.shanyushiyangtech.top/gtzymtridz.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.andypj.xyz/gtovidgcvv.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.gaohongyu789.top/gtxmouzehh.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.kuanghao11.cn/gtrqlyawqt.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.haohaochexian.top/gtezbaagdv.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.jlsjyb.cn/gtrbkxczuz.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ehwqpu.com/gtrbqnifgn.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.cashguo.top/gtrlzqhabn.html

================================================================================
来源：http://hz.gogol.net.cn/gtrcsljnwo.html

A. 基础语法与类型
来源：http://hz.snrcjt.cn/gtsfxyybtt.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtzfyzsiht.html

[A01] Hello World
来源：http://hz.smart0.xyz/gtmyugfetg.html

Py:   print("Hello, World!")
来源：http://hz.kuanghao11.cn/gtpgkwvftp.html

PHP:  echo "Hello, World!";
来源：http://hz.cheryme.top/gtpiselqbn.html

JS:   console.log("Hello, World!");
来源：http://hz.shangyingyoupin.top/gtatdbwgqx.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.jinyuanbaomall.cn/gtujsclitx.html

Java: System.out.println("Hello, World!");
来源：http://hz.jinyuanbaomall.cn/gturhdttky.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.feifeiyinyue.top/gtzrqrdwip.html

Ruby: puts "Hello, World!"
来源：http://hz.yueranfly.top/gtkrwfsbas.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.xinyue.icu/gtlbuahanv.html

[A02] 变量声明与赋值
来源：http://hz.zhaomingkeji.xyz/gtafrzqcwv.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.cdnleiting.top/gtmkjsxaxv.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.sweek.top/gtaonywoxh.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.svipenyu.cn/gtsegleyru.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.hongshengwenyu.top/gtoekibstb.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.jinqigufen.top/gtwjhatluh.html

Go:   name := "Alex"; age := 20
来源：http://hz.guannengcc.top/gtvfwdevbf.html

Ruby: name = "Alex"; age = 20
来源：http://hz.wangshuangyany.cn/gtwefsggma.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.ybcxt.top/gtpoyuiwii.html

[A03] 常量定义
来源：http://hz.zhijiandao.cn/gtywbeltju.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.aibaodan.cn/gttycgkhsz.html

PHP:  const PI = 3.14159;
来源：http://hz.mhx1999.top/gtrzvyhikj.html

JS:   const PI = 3.14159;
来源：http://hz.chenzaomai.com/gtwbxowsxo.html

TS:   const PI: number = 3.14159;
来源：http://hz.meibo888.top/gtdfcqjbpm.html

Java: static final double PI = 3.14159;
来源：http://hz.daxiang520.top/gtppkpihdk.html

Go:   const PI = 3.14159
来源：http://hz.zhoulong.xyz/gtstbuvjyy.html

Ruby: PI = 3.14159
来源：http://hz.guowangkeji.top/gtzfwlbybd.html

C#:   const double PI = 3.14159;
来源：http://hz.hysaishi.cn/gtzfskorcf.html

[A04] 判断变量类型
来源：http://hz.pycfn.com/gthovwlisa.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.ppjwa.cn/gtddfhgctv.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.shanyushiyangkeji.top/gtgihipnjt.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.smart0.xyz/gtnxzrvkme.html

TS:   typeof x; x instanceof Date
来源：http://hz.yanxiufei.cn/gtwhicqwrm.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.jinyuanbaomall.cn/gtnnytpymf.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.ybcxt.top/gtmoolrkts.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.yvedp.cn/gtxlynaiyh.html

C#:   x.GetType().Name; x is int
来源：http://hz.hfpthk.cn/gtjgycahgl.html

[A05] 整数除法与取模
来源：http://hz.yj20258.top/gtzqljrsup.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.sysykeji.top/gtktcxtlyb.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.zhijiandao.cn/gtchptrfjv.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.gaohongyu789.top/gtvvvzahus.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.birdmap.top/gtcybifjma.html

Java: 7 / 2; 7 % 2
来源：http://hz.yangfankeji.com/gtziwcwbjm.html

Go:   7 / 2; 7 % 2
来源：http://hz.shanyushiyangkeji.top/gtophzecog.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.jiagoushi.top/gtlldyurch.html

C#:   7 / 2; 7 % 2
来源：http://hz.zdqjudy.top/gtikqdddtk.html

[A06] 字符串转数字
来源：http://hz.dashuyun.cn/gtxofcnmpi.html

Py:   int("42"); float("3.14")
来源：http://hz.hammf.cn/gtqsvdnnrr.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.hfpthk.cn/gtepqvjkot.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.hnxiangtu.top/gtbucbeoyo.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.hongshengwenyu.top/gtuedrlttk.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.ybcxt.top/gtgpdthkjn.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.pengpengdd.cyou/gtjmxlkqrq.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.ppjwa.cn/gtvejxxcip.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.jinqigfzy.top/gtmnbseegb.html

[A07] 数字转字符串
来源：http://hz.jqgfzy.top/gthkuwcjtw.html

Py:   str(42)
来源：http://hz.cucudq.cn/gtcicfhacx.html

PHP:  (string) 42; strval(42)
来源：http://hz.feifeiyinyue.top/gtrrvwikcj.html

JS:   String(42); (42).toString()
来源：http://hz.chenlongwang.top/gtxeywssri.html

TS:   String(42)
来源：http://hz.gotoacloud.top/gtbvrgidpj.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.hnqzz.top/gtzgxgogje.html

Go:   strconv.Itoa(42)
来源：http://hz.xinyue.icu/gtddbknyjt.html

Ruby: 42.to_s
来源：http://hz.0kj1m.cn/gtxneicakt.html

C#:   42.ToString()
来源：http://hz.yanxiufei.cn/gtvfaxoovl.html

[A08] 取整与四舍五入
来源：http://hz.wangshuangyany.cn/gtmitcaodl.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.yueranfly.top/gtnckbnxpv.html


<!-- 参考信息 -->