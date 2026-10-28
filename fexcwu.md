代发 wailian999

[U63] PHP：文件读写
来源：http://hz.yangfankeji.com/gtqnqxqtqa.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.zhengqikj.top/gtesxwcopc.html

[U64] PHP：目录遍历
来源：http://hz.guowangkeji.top/gtnoauillu.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.jianghu66.top/gtndrsuvip.html

[U65] PHP：会话
来源：http://hz.pengpengdd.cyou/gtmdwyhyie.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.vqdsnc.cn/gtuyizxrhd.html

[U66] PHP：设置 Cookie
来源：http://hz.nanxinkj.top/gtchsgbasd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.sufxvd.cn/gtqtpckcln.html

[U67] PHP：处理文件上传
来源：http://hz.cdnleiting.top/gtzefizlip.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.ybcxt.top/gtwrqvjopf.html

[U68] PHP：PDO 连接
来源：http://hz.zhongyouzk.top/gtlqccaqco.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.birdmap.top/gttlekaidy.html

[U69] PHP：PDO 预处理
来源：http://hz.pycfn.com/gtchhjdunp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.zhijiandao.cn/gthwlpwflf.html

[U70] PHP：PDO 事务
来源：http://hz.fzhhl.top/gtzpdjlqzc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.hnxiangtu.top/gtcqixpiuf.html

[U71] PHP：抛出异常
来源：http://hz.jqgfzy.top/gtkkyinfrg.html

throw new RuntimeException("失败", 500);
来源：http://hz.mhx1999.top/gtuklbmkhw.html

[U72] PHP：写错误日志
来源：http://hz.daxiang520.top/gtxknqifqk.html

error_log("失败: " . $e->getMessage());
来源：http://hz.meibo888.top/gtggoqiszm.html

[U73] PHP：读取 ini 配置
来源：http://hz.kuanghao11.cn/gtwftjggcu.html

parse_ini_file("config.ini", true)
来源：http://hz.dashuyun.cn/gteogtszrm.html

[U74] PHP：读取环境变量
来源：http://hz.c1oappe.top/gtxgptiilj.html

getenv("APP_ENV") ?: "production"
来源：http://hz.0kj1m.cn/gtsacmxcyk.html

[U75] PHP：依赖注入
来源：http://hz.fzhhl.top/gtyvlcxxob.html

composer require psr/container
来源：http://hz.ivvv.top/gtyidwuvuq.html

[U76] PHP：简单路由
来源：http://hz.daxiang520.top/gtpqppkvbm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.mhx1999.top/gtbifcftoi.html

[U77] PHP：模板渲染
来源：http://hz.hongshengwenyu.top/gtmjwxeedd.html

composer require twig/twig
来源：http://hz.zhongyouzk.top/gtbaxcukts.html

[U78] PHP：单元测试
来源：http://hz.zhixingplan.top/gtueyjuxvh.html

composer require --dev phpunit/phpunit
来源：http://hz.cdnleiting.top/gtsjngesyu.html

[U79] PHP：静态分析
来源：http://hz.daria6918.cn/gtffyhzrad.html

composer require --dev phpstan/phpstan
来源：http://hz.jianghu66.top/gtbgkubnsk.html

[U80] PHP：代码规范修复
来源：http://hz.yuxming.cn/gtxsiaoagn.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.yonumen.top/gtroxmthra.html

[U81] JS：初始化项目
来源：http://hz.316326.xyz/gtxijqtmnc.html

npm init -y;  npm i express
来源：http://hz.daxiang520.top/gtywhprhtu.html

[U82] JS：package.json 脚本
来源：http://hz.zhongyouzk.top/gtkdpgjxnq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.fzhhl.top/gtsqxvetsw.html

[U83] JS：ES Module 导入导出
来源：http://hz.feifeiyinyue.top/gtwndrtqye.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.andypj.xyz/gtuosfrvuo.html

[U84] JS：CommonJS 写法
来源：http://hz.xinyue.icu/gthmnsgdbs.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.wangdashe.top/gtnafphusc.html

[U85] JS：可选链
来源：http://hz.gaohongyu789.top/gtbiicoglh.html

a?.b?.c
来源：http://hz.cdnleiting.top/gtcdxzkfrl.html

[U86] JS：空值合并
来源：http://hz.zhaomingkeji.xyz/gtldonhgmb.html

a ?? b
来源：http://hz.bjfxy.top/gtqfuymrte.html

[U87] JS：解构默认值
来源：http://hz.zhijiandao.cn/gtqwozqoqe.html

const { a = 1, b = 2 } = obj;
来源：http://hz.zycfv.cn/gtazlhkqzh.html

[U88] JS：对象展开合并
来源：http://hz.ivvv.top/gttljgrjvn.html

{ ...a, ...b }
来源：http://hz.jiagoushi.top/gtfsruskmi.html

[U89] JS：数组去重
来源：http://hz.9152youxi.cn/gtrlyzuatr.html

[...new Set(arr)]
来源：http://hz.chenjidiqi.icu/gtawmkrcxf.html

[U90] JS：数字数组排序
来源：http://hz.hfpthk.cn/gtoclervtl.html

[...arr].sort((a, b) => a - b)
来源：http://hz.jqgufenzy.top/gtwkldyixy.html

[U91] JS：对象键值遍历
来源：http://hz.havefunace.top/gtqswthzvr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.zycfv.cn/gtjjfevhki.html

[U92] JS：深拷贝
来源：http://hz.shanyushiyangtech.top/gtwygsutca.html

structuredClone(obj)
来源：http://hz.tianlin.xyz/gtlxieksef.html

[U93] JS：模板字符串
来源：http://hz.sysykeji.top/gtwdxzaeax.html

`共 ${n} 条`
来源：http://hz.yongpay.top/gtlfbqxseg.html

[U94] JS：箭头函数
来源：http://hz.bjfxy.top/gtoqlkzpgl.html

const double = x => x * 2;
来源：http://hz.yvedp.cn/gtfltxpqeg.html

[U95] JS：Promise 包装
来源：http://hz.fzhhl.top/gtmlivvrjs.html

new Promise((resolve, reject) => {})
来源：http://hz.hnqzz.top/gtnsyxefbm.html

[U96] JS：async/await 与异常
来源：http://hz.hongshengwenyu.top/gtnrzbogka.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.hywenlv.cn/gtzmalvheq.html

[U97] JS：并发请求
来源：http://hz.feifeiyinyue.top/gtxsjwqrai.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xinyue.icu/gtyjmdqgch.html

[U98] JS：fetch 带 JSON
来源：http://hz.andypj.xyz/gtsmvyulvt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.pengpengdd.cyou/gtvimfbgyc.html

[U99] JS：事件监听
来源：http://hz.c1oappe.top/gtnvkmnfbp.html

el.addEventListener("click", e => {})
来源：http://hz.mhx1999.top/gtezwtmavc.html

[U100] JS：DOM 查询
来源：http://hz.chenlongwang.top/gtgkvucfum.html

document.querySelector(".item")
来源：http://hz.guowangkeji.top/gtwmazsvev.html

[U101] JS：classList 操作
来源：http://hz.zdqjudy.top/gtqbznduoe.html

el.classList.toggle("active")
来源：http://hz.zhiwuduotai.top/gtwigotzgu.html

[U102] JS：本地存储
来源：http://hz.chenzaomai.com/gtuhidjtoi.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.tanke756.top/gtnqgrdngb.html

[U103] JS：定时器
来源：http://hz.svipenyu.cn/gtivjaciib.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.shanyushiyangkeji.top/gttfdiqexs.html

[U104] JS：防抖
来源：http://hz.yongpay.top/gtwqgkbvat.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhijiandao.cn/gtnkqlfhda.html

[U105] JS：节流
来源：http://hz.birdmap.top/gtsrrkaqcd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.chenzaomai.com/gtrecrtndf.html

[U106] JS：日期格式化
来源：http://hz.zhaomingkeji.xyz/gttvrvpins.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yongpay.top/gtjahbkpfu.html

[U107] JS：数字千分位
来源：http://hz.gotoacloud.top/gtdovgjeem.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.tanke756.top/gtlwodusds.html

[U108] JS：随机整数
来源：http://hz.xziqi.cn/gtmdlhhrki.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.yj20258888.top/gtfqpjhnkp.html

[U109] JS：数组分组
来源：http://hz.bjfxy.top/gtqscecync.html

Object.groupBy(arr, x => x.type)
来源：http://hz.yangfankeji.com/gtcacvzdkm.html

[U110] JS：数组分块
来源：http://hz.cdnleiting.top/gthjsukhee.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.aizwys.cn/gtblwegpvn.html

[U111] JS：对象转 Map
来源：http://hz.chenlongwang.top/gtvnipcvmv.html

new Map(Object.entries(obj))
来源：http://hz.316326.xyz/gtonlzmxbp.html

[U112] JS：字符串补位
来源：http://hz.hongshengwenyu.top/gtbocarehz.html

"7".padStart(3, "0")
来源：http://hz.yj202588.top/gtkqmddeah.html

[U113] JS：正则替换全部
来源：http://hz.hammf.cn/gtkrbqtprk.html

s.replaceAll("a", "b")
来源：http://hz.redwolf501.top/gtcrjcvjtu.html

[U114] JS：JSON 深比较
来源：http://hz.ppjwa.cn/gtcgslwxlz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shanyushiyangtech.top/gtcasrkvzo.html

[U115] JS：生成 UUID
来源：http://hz.dianchejie.cn/gtdbfodjvm.html

crypto.randomUUID()
来源：http://hz.ywan-chungtsiang.top/gtrejsqdkr.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.shanyushiyangkeji.top/gtsjxpzxkm.html

/** @param {string} name */ function f(name) {}
来源：http://hz.tian-w.cn/gtcyjnazuy.html

[U117] JS：单元测试
来源：http://hz.cdnleiting.top/gtommhjaqn.html

npm i -D vitest;  npx vitest
来源：http://hz.zhijiandao.cn/gtuvixaqxa.html

[U118] JS：开发服务器
来源：http://hz.jinyuanbaomall.cn/gtemxspjjd.html

npm i -D vite;  npx vite
来源：http://hz.hnqzz.top/gtjchnkyln.html

[U119] JS：生产构建
来源：http://hz.sufxvd.cn/gtwmxjfmnt.html

npx vite build
来源：http://hz.yvedp.cn/gtbpblxnck.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.yonumen.top/gtggbltlgl.html

import.meta.env.VITE_API_URL
来源：http://hz.xylfe.cn/gtbzztqgxy.html

================================================================================
来源：http://hz.zdqjudy.top/gtopwlqgnl.html

统计汇总
来源：http://hz.ydzc1.top/gtciekkbvi.html

================================================================================
来源：http://hz.hammf.cn/gtuvfnmflb.html

按语言统计（条）：
来源：http://hz.sxryk.cn/gtufmkodzx.html

Python ......... 252
来源：http://hz.52xcode.cn/gtpihzpsmv.html

PHP ............ 252
来源：http://hz.gzhubu.top/gtkgspddsa.html

JavaScript ..... 252
来源：http://hz.meibo888.top/gtpogcxkgq.html

TypeScript ..... 212
来源：http://hz.ehwqpu.com/gtitkgoktx.html

Java ........... 212
来源：http://hz.jqgufenzy.top/gtuzfcnssq.html

Go ............. 212
来源：http://hz.zdqjudy.top/gtrboesxcc.html

Ruby ........... 212
来源：http://hz.hnxiangtu.top/gtolqijbui.html

C# ............. 212
来源：http://hz.yvedp.cn/gtalrmzyye.html

C .............. 30
来源：http://hz.316326.xyz/gtiuavxney.html

C++ ............ 30
来源：http://hz.jyoumei.cn/gtfcfakoxg.html

SQL ............ 90
来源：http://hz.shanyushiyangtech.top/gtadnkufzl.html

Bash ........... 80
来源：http://hz.yj20258888.top/gtxlotlbfo.html

Kotlin ......... 15
来源：http://hz.dashuyun.cn/gtokyplrrx.html

Swift .......... 15
来源：http://hz.wangshuangyany.cn/gtlewpmolp.html

Lua ............ 10
来源：http://hz.jyoumei.cn/gtwrfozunv.html

Perl ........... 10
来源：http://hz.sxryk.cn/gtlunorpic.html

Scala .......... 10
来源：http://hz.nanxinkj.top/gtrwrffdzn.html

------------------------------------
来源：http://hz.zhiwuduotai.top/gtgguyzakv.html

合计 ........... 2106 条
来源：http://hz.quarkkingdee.top/gthjmrvhoc.html

按章节统计：
来源：http://hz.cdnleiting.top/gtrbkhpzqf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.zhiwuduotai.top/gtptypairy.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.daria6918.cn/gtnhspjzbe.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.guannengcc.top/gtcvoekvky.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.mhx1999.top/gtugluqqnx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.cashguo.top/gtjjinghib.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.yongpay.top/gtxnikkzcf.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.shzxlz.cn/gtofdxkmng.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.yonumen.top/gthmttdoda.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.mhx1999.top/gteztdodqj.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.fengsongda.top/gtyihtllty.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.iojbl.cn/gtzklgqria.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.cqqwz.cn/gtqqtgkemh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.hywenlv.cn/gtqhwuqmtw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.9152youxi.cn/gtuatnshld.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.zhoulong.xyz/gtpdehueyj.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.jqgufenzy.top/gtsyudagrg.html

Q SQL 专题                              90
来源：http://hz.shzxlz.cn/gtmvotopav.html

R Bash 专题                             80
来源：http://hz.jianghu66.top/gtgajvzaak.html

S C / C++ 专题                          60
来源：http://hz.cucudq.cn/gttlabgszh.html

T 其他语言补充                          60
来源：http://hz.ybcxt.top/gtceywnoat.html

U 高频实用片段                         120
来源：http://hz.quarkkingdee.top/gtamwfjeag.html

------------------------------------
来源：http://hz.hfpthk.cn/gtdesddvzl.html

合计                                  2106 条
来源：http://hz.guannengcc.top/gtndztdjrj.html

--------------------------------------------------------------------------------
来源：http://hz.ywan-chungtsiang.top/gtbtrdtyln.html

使用提醒
来源：http://hz.ybcxt.top/gtzcjqdsmo.html

--------------------------------------------------------------------------------
来源：http://hz.0kj1m.cn/gtrqazqwda.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.hfpthk.cn/gtrnesddgu.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.jlsjyb.cn/gtyzomkvcz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.cdnleiting.top/gtakrtraii.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.sufxvd.cn/gtvulqdcat.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.c1oappe.top/gtbhziutno.html

—— 文件结束 ——
来源：http://hz.zhijiandao.cn/gtesfkquwj.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtpkddifti.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.gaohongyu789.top/gtpxbzgnvi.html

Common Programming Examples Cheat Book
来源：http://hz.sysykeji.top/gtvgvqlvzt.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtfzomieoh.html

【收录内容】
来源：http://hz.cheryme.top/gtatikzfvi.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.zhengqikj.top/gttrerwzum.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.gotoacloud.top/gtgdrnreno.html

SQL · Bash · C · C++
来源：http://hz.wangshuangyany.cn/gturelocra.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.andypj.xyz/gtkecwxffm.html

【使用说明】
来源：http://hz.redwolf501.top/gthpgpcash.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.316326.xyz/gtmcrpmvps.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.mhx1999.top/gtzlkqcfot.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.zycfv.cn/gtrjgvbbbr.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.zhixingplan.top/gtobfgwcxn.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.jqgufenzy.top/gtxbqamdxm.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.dianchejie.cn/gtvvsjoaga.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.hywenlv.cn/gttnojovxj.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.jyoumei.cn/gtcojzaecb.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.ehwqpu.com/gthlzibtez.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.zycfv.cn/gtyjlkofkw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.tanke756.top/gtrhzgqjuk.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.zhaomingkeji.xyz/gtqeplnpqf.html

【文件统计】
来源：http://hz.svipenyu.cn/gtspbpfzdu.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.sysykeji.top/gtnsjebcts.html

--------------------------------------------------------------------------------
来源：http://hz.redwolf501.top/gtvxejlmfz.html

目  录
来源：http://hz.ydzc1.top/gtfknwhbvy.html

--------------------------------------------------------------------------------
来源：http://hz.nanxuanxn.top/gteasvbnhy.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.cashguo.top/gtiawuuhpl.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.0kj1m.cn/gtfegvysqz.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.fzhhl.top/gtjkudiwkp.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.bjfxy.top/gtzbxassgb.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.yuanzhike.top/gttsuoceff.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.hnxiangtu.top/gtncavafrd.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.jinqigfzy.top/gtixtpvgmx.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.sufxvd.cn/gtxstyujsx.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.ivvv.top/gtywurptow.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.0kj1m.cn/gtdtqenvrc.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.feifeiyinyue.top/gtrkqlalfc.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.cqqwz.cn/gtzstvweif.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.cheryme.top/gttikmrpzb.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.cashguo.top/gtkzhiwdri.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.yj202588.top/gtnqibgnqz.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.jqgufenzy.top/gtjinpzmpq.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.svipenyu.cn/gtmnkcgjnt.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.zhaomingkeji.xyz/gtrolxupvn.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.ivvv.top/gtpcoimhrw.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.xziqi.cn/gtsmckvtxz.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.chenzaomai.com/gtjwedfhzy.html

================================================================================
来源：http://hz.nanxinkj.top/gtctnfgenl.html

A. 基础语法与类型
来源：http://hz.cucudq.cn/gtrhjvjguz.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtxvhzktwi.html

[A01] Hello World
来源：http://hz.jinqigfzy.top/gtliopendn.html

Py:   print("Hello, World!")
来源：http://hz.wangdashe.top/gtdvsqqlwc.html

PHP:  echo "Hello, World!";
来源：http://hz.yueranfly.top/gtjyfzptkv.html

JS:   console.log("Hello, World!");
来源：http://hz.cheryme.top/gtwefnfzqo.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.tanke756.top/gtfihwwwym.html

Java: System.out.println("Hello, World!");
来源：http://hz.hywenlv.cn/gtkdqchlri.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.c1oappe.top/gthgorkyjj.html

Ruby: puts "Hello, World!"
来源：http://hz.daria6918.cn/gtwsuhvfkv.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.yongpay.top/gthwaigpsd.html

[A02] 变量声明与赋值
来源：http://hz.gaohongyu789.top/gtwyyoduju.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.tianlin.xyz/gtfgwwwxpj.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.zdqjudy.top/gtwixfudot.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.yanxiufei.cn/gtsmdlgnhv.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.jianghu66.top/gtphsrfwjo.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.zdqjudy.top/gtchgevbzu.html

Go:   name := "Alex"; age := 20
来源：http://hz.hywenlv.cn/gtzqvpucgy.html

Ruby: name = "Alex"; age = 20
来源：http://hz.gzhubu.top/gtitktrtmn.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.0kj1m.cn/gtquznwqyr.html

[A03] 常量定义
来源：http://hz.52xcode.cn/gtkirpwqkf.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.pycfn.com/gtndaycmdf.html

PHP:  const PI = 3.14159;
来源：http://hz.sufxvd.cn/gtrxdevaab.html

JS:   const PI = 3.14159;
来源：http://hz.wangshuangyany.cn/gtatrsdmba.html

TS:   const PI: number = 3.14159;
来源：http://hz.nanxinkj.top/gtlgmgidxk.html

Java: static final double PI = 3.14159;
来源：http://hz.shangyingyoupin.top/gtjocbrtxt.html

Go:   const PI = 3.14159
来源：http://hz.daria6918.cn/gtrnwwugmm.html

Ruby: PI = 3.14159
来源：http://hz.feifeiyinyue.top/gtpvtwfdvv.html

C#:   const double PI = 3.14159;
来源：http://hz.kuanghao11.cn/gtbhjrikiq.html

[A04] 判断变量类型
来源：http://hz.cashguo.top/gtnxkhrhgr.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.c1oappe.top/gtxszpapat.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.xuanzx.com/gtmfxulbvi.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.meibo888.top/gtyhjlkwji.html

TS:   typeof x; x instanceof Date
来源：http://hz.yongpay.top/gtrfsjlnkv.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.jinyuanbaomall.cn/gtkunwvmap.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.gotoacloud.top/gtguosnvdp.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.feifeiyinyue.top/gtapjunjgz.html

C#:   x.GetType().Name; x is int
来源：http://hz.quarkkingdee.top/gtnqfahhot.html

[A05] 整数除法与取模
来源：http://hz.yuxming.cn/gtvvvllfva.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.mhx1999.top/gtrrjyjqoi.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.ydjk.org.cn/gtcxwqjyyq.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.9152youxi.cn/gtijhyydfa.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.fengsongda.top/gtltkadisw.html

Java: 7 / 2; 7 % 2
来源：http://hz.hysaishi.cn/gtjclfyvrp.html

Go:   7 / 2; 7 % 2
来源：http://hz.haohaochexian.top/gtnfmwexrd.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.zhaomingkeji.xyz/gtxlvmeffn.html

C#:   7 / 2; 7 % 2
来源：http://hz.gaohongyu789.top/gtxzoixizi.html

[A06] 字符串转数字
来源：http://hz.yuxming.cn/gtxklejarr.html

Py:   int("42"); float("3.14")
来源：http://hz.zhiwuduotai.top/gtbnxeplsz.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.ywan-chungtsiang.top/gtqsrtfhuq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.yuanzhike.top/gtcfherlwb.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.pycfn.com/gtrqtsjpnl.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.yueranfly.top/gtkrrxafsw.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.yj202588.top/gtawkzmldo.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.nwbrower.top/gthsmecrho.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.dianchejie.cn/gtkyecvxey.html

[A07] 数字转字符串
来源：http://hz.shuidangran.top/gtzueybafn.html

Py:   str(42)
来源：http://hz.zhaomingkeji.xyz/gtjilahghf.html

PHP:  (string) 42; strval(42)
来源：http://hz.52xcode.cn/gtvdtqrjxv.html

JS:   String(42); (42).toString()
来源：http://hz.jyoumei.cn/gtdsgpidcq.html

TS:   String(42)
来源：http://hz.andypj.xyz/gtnregafok.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.zdqjudy.top/gtuewxynzv.html

Go:   strconv.Itoa(42)
来源：http://hz.cdnleiting.top/gtzedbjjhi.html

Ruby: 42.to_s
来源：http://hz.sufxvd.cn/gtlwxfoaua.html

C#:   42.ToString()
来源：http://hz.daria6918.cn/gtqcwgadgx.html

[A08] 取整与四舍五入
来源：http://hz.aibaodan.cn/gtmyqzhiyh.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.xuetiantiany.cn/gtfwuaigvz.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.tanke756.top/gtjqdbehgq.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.ydzc1.top/gtqimvpslp.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.52xcode.cn/gttkqxogik.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.wangshuangyany.cn/gtmkssqvla.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.havefunace.top/gtivvzzhft.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.havefunace.top/gtbusydefp.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.havefunace.top/gtyklriwbo.html

[A09] 绝对值与最大最小值
来源：http://hz.hysaishi.cn/gthtekpywu.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.chenlongwang.top/gttywxnicn.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.yonumen.top/gtbpohnbcw.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.zhiwuduotai.top/gtqogkwxnw.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.hammf.cn/gtyhumrldv.html


<!-- 参考信息 -->