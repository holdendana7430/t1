代发 wailian999

[U53] PHP：空合并运算符
来源：http://hz.smart0.xyz/gtkwjhbgac.html

$v = $a ?? $b ?? "default";
来源：http://hz.zhongyouzk.top/gtmgctdmla.html

[U54] PHP：空安全调用
来源：http://hz.c1oappe.top/gtfrpuwgza.html

$obj?->method()
来源：http://hz.xuanzx.com/gtsufmckiw.html

[U55] PHP：match 表达式
来源：http://hz.shanyushiyangtech.top/gttfycocrl.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.gzhubu.top/gtecbcnuym.html

[U56] PHP：命名参数
来源：http://hz.bjfxy.top/gtkjpzelgz.html

f(a: 1, b: 2)
来源：http://hz.fengsongda.top/gtdzsrlled.html

[U57] PHP：字符串插值
来源：http://hz.cashguo.top/gtklngnnls.html

"值: {$a}"
来源：http://hz.ydzc1.top/gtyyqoachi.html

[U58] PHP：数组三件套
来源：http://hz.feifeiyinyue.top/gtfcldtynb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.ywan-chungtsiang.top/gtwhwmfxyj.html

[U59] PHP：自定义排序
来源：http://hz.yuxming.cn/gtdnfbyene.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.nanxinkj.top/gtpjhroywg.html

[U60] PHP：JSON 编解码
来源：http://hz.9152youxi.cn/gtivspwdth.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.hfpthk.cn/gtypffynol.html

[U61] PHP：正则
来源：http://hz.jlsjyb.cn/gtogherleq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.nanxuanxn.top/gttketkrej.html

[U62] PHP：日期对象
来源：http://hz.havefunace.top/gtctsehoxc.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.hysaishi.cn/gtcifzrhsp.html

[U63] PHP：文件读写
来源：http://hz.hnqzz.top/gtxcrjhuny.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.sweek.top/gtctoxloyg.html

[U64] PHP：目录遍历
来源：http://hz.svipenyu.cn/gtyejkidvh.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.hnqzz.top/gtizpvudyk.html

[U65] PHP：会话
来源：http://hz.jyoumei.cn/gtymwzjyhy.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.shangyingyoupin.top/gtxgjipuij.html

[U66] PHP：设置 Cookie
来源：http://hz.jinyuanbaomall.cn/gtvtfmdffk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.ybcxt.top/gtdwjxddwg.html

[U67] PHP：处理文件上传
来源：http://hz.jqgfzy.top/gtltjkmfci.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.yuxming.cn/gtukkbefkn.html

[U68] PHP：PDO 连接
来源：http://hz.sufxvd.cn/gtkfksujqy.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.wangdashe.top/gtqmmyygts.html

[U69] PHP：PDO 预处理
来源：http://hz.cdnleiting.top/gtzcvqougx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.redwolf501.top/gtyjzrcelr.html

[U70] PHP：PDO 事务
来源：http://hz.zhoulong.xyz/gtcudohaym.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.pengpengdd.cyou/gtwvmxarvs.html

[U71] PHP：抛出异常
来源：http://hz.bjfxy.top/gtzwmqijfr.html

throw new RuntimeException("失败", 500);
来源：http://hz.zhongyouzk.top/gtffvkgpoo.html

[U72] PHP：写错误日志
来源：http://hz.yj20258.top/gtckigtpqk.html

error_log("失败: " . $e->getMessage());
来源：http://hz.ywan-chungtsiang.top/gtlweyzvro.html

[U73] PHP：读取 ini 配置
来源：http://hz.jyoumei.cn/gtmlgqnavo.html

parse_ini_file("config.ini", true)
来源：http://hz.xylfe.cn/gtwbjadpia.html

[U74] PHP：读取环境变量
来源：http://hz.jqgufenzy.top/gtkbugbpzz.html

getenv("APP_ENV") ?: "production"
来源：http://hz.0kj1m.cn/gtgutdmdrv.html

[U75] PHP：依赖注入
来源：http://hz.zhongyouzk.top/gtatovjqiu.html

composer require psr/container
来源：http://hz.fzhhl.top/gtycwcjbya.html

[U76] PHP：简单路由
来源：http://hz.pengpengdd.cyou/gtmjtldsdv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.wangdashe.top/gtgkhubbky.html

[U77] PHP：模板渲染
来源：http://hz.havefunace.top/gtieplmbgx.html

composer require twig/twig
来源：http://hz.gogol.net.cn/gtkeyjuhki.html

[U78] PHP：单元测试
来源：http://hz.guannengcc.top/gtklxdgfwj.html

composer require --dev phpunit/phpunit
来源：http://hz.xingfuxueyuan.xyz/gtstcpotty.html

[U79] PHP：静态分析
来源：http://hz.hnqzz.top/gtgtosfvzu.html

composer require --dev phpstan/phpstan
来源：http://hz.hnxiangtu.top/gtdzoxubgf.html

[U80] PHP：代码规范修复
来源：http://hz.guowangkeji.top/gtdonogfwz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.c1oappe.top/gtuaufcqzc.html

[U81] JS：初始化项目
来源：http://hz.shangyingyoupin.top/gtqfxyfjmv.html

npm init -y;  npm i express
来源：http://hz.yonumen.top/gtofsdgwon.html

[U82] JS：package.json 脚本
来源：http://hz.yongpay.top/gtzhyipwtm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.daria6918.cn/gtudhxgwck.html

[U83] JS：ES Module 导入导出
来源：http://hz.ppjwa.cn/gttitkjkcq.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.zhijiandao.cn/gtihjnotdi.html

[U84] JS：CommonJS 写法
来源：http://hz.daxiang520.top/gtvtuatubu.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.fzhhl.top/gtikooxmfn.html

[U85] JS：可选链
来源：http://hz.iojbl.cn/gtsaxxhggw.html

a?.b?.c
来源：http://hz.ydzc1.top/gtuyrztcdk.html

[U86] JS：空值合并
来源：http://hz.pengpengdd.cyou/gtdyhxtqty.html

a ?? b
来源：http://hz.zdqjudy.top/gtkvsxsgzq.html

[U87] JS：解构默认值
来源：http://hz.wangshuangyany.cn/gtwenlpdfu.html

const { a = 1, b = 2 } = obj;
来源：http://hz.haohaochexian.top/gteyrtegqc.html

[U88] JS：对象展开合并
来源：http://hz.snrcjt.cn/gttwwaofec.html

{ ...a, ...b }
来源：http://hz.yueranfly.top/gtctjnaoxr.html

[U89] JS：数组去重
来源：http://hz.haohaochexian.top/gtuszkcxcc.html

[...new Set(arr)]
来源：http://hz.yuxming.cn/gtupushpay.html

[U90] JS：数字数组排序
来源：http://hz.zhaomingkeji.xyz/gtzramqupf.html

[...arr].sort((a, b) => a - b)
来源：http://hz.yonumen.top/gtbrsydgvv.html

[U91] JS：对象键值遍历
来源：http://hz.jinqigfzy.top/gttpwvhlqq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.shuidangran.top/gtmewrzwee.html

[U92] JS：深拷贝
来源：http://hz.yanxiufei.cn/gtsxgnspgz.html

structuredClone(obj)
来源：http://hz.cheryme.top/gthsgrhezh.html

[U93] JS：模板字符串
来源：http://hz.cdnleiting.top/gtowykdnil.html

`共 ${n} 条`
来源：http://hz.chenjidiqi.icu/gtfzpegfdq.html

[U94] JS：箭头函数
来源：http://hz.snrcjt.cn/gtthzbchwt.html

const double = x => x * 2;
来源：http://hz.bjfxy.top/gtvpkjlvub.html

[U95] JS：Promise 包装
来源：http://hz.gotoacloud.top/gtfmlrqseo.html

new Promise((resolve, reject) => {})
来源：http://hz.chenjidiqi.icu/gtevilwnwx.html

[U96] JS：async/await 与异常
来源：http://hz.hongshengwenyu.top/gtmfauhmin.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.daxiang520.top/gtfbsrdowx.html

[U97] JS：并发请求
来源：http://hz.hfpthk.cn/gtezhhtnvv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinyuanbaomall.cn/gtpmttnfeg.html

[U98] JS：fetch 带 JSON
来源：http://hz.smart0.xyz/gtenrbcegk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.52xcode.cn/gtabrxxsyi.html

[U99] JS：事件监听
来源：http://hz.daria6918.cn/gtcnkoznxq.html

el.addEventListener("click", e => {})
来源：http://hz.gaohongyu789.top/gtolwrigsr.html

[U100] JS：DOM 查询
来源：http://hz.shangyingyoupin.top/gtxaepebyx.html

document.querySelector(".item")
来源：http://hz.wangdashe.top/gtgquevidd.html

[U101] JS：classList 操作
来源：http://hz.birdmap.top/gtbdoewedw.html

el.classList.toggle("active")
来源：http://hz.cheryme.top/gtjwkcibnc.html

[U102] JS：本地存储
来源：http://hz.dashuyun.cn/gtwuwyyssc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.ydzc1.top/gtazzfkbfl.html

[U103] JS：定时器
来源：http://hz.sysykeji.top/gtjjxaavmo.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.zhoulong.xyz/gtfdemhtem.html

[U104] JS：防抖
来源：http://hz.guowangkeji.top/gtrkxrzosl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhiwuduotai.top/gtoguapvdo.html

[U105] JS：节流
来源：http://hz.yueranfly.top/gtxqsbaeue.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.yonumen.top/gtblzgxfyq.html

[U106] JS：日期格式化
来源：http://hz.gaohongyu789.top/gtftxzvxjy.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.birdmap.top/gtwpsrmpsw.html

[U107] JS：数字千分位
来源：http://hz.redwolf501.top/gtklbvabak.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.ydjk.org.cn/gtzpjhigzu.html

[U108] JS：随机整数
来源：http://hz.316326.xyz/gtgyfcctxx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.dashuyun.cn/gtedgnfaax.html

[U109] JS：数组分组
来源：http://hz.sufxvd.cn/gtwmeqirdu.html

Object.groupBy(arr, x => x.type)
来源：http://hz.jinqigufen.top/gtwngyshwj.html

[U110] JS：数组分块
来源：http://hz.yuanzhike.top/gtetjuqfdv.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.zhiwuduotai.top/gtfijsvspa.html

[U111] JS：对象转 Map
来源：http://hz.yj20258888.top/gttqxeruqw.html

new Map(Object.entries(obj))
来源：http://hz.daxiang520.top/gtekttelqe.html

[U112] JS：字符串补位
来源：http://hz.snrcjt.cn/gtbbjgpmxg.html

"7".padStart(3, "0")
来源：http://hz.smart0.xyz/gtknpbquqv.html

[U113] JS：正则替换全部
来源：http://hz.bjfxy.top/gtxyowycbi.html

s.replaceAll("a", "b")
来源：http://hz.chenlongwang.top/gtxxijjkvr.html

[U114] JS：JSON 深比较
来源：http://hz.mhx1999.top/gtrmeegkeb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.sysykeji.top/gtfeecsujn.html

[U115] JS：生成 UUID
来源：http://hz.tanke756.top/gtslqxcoyg.html

crypto.randomUUID()
来源：http://hz.hnxiangtu.top/gtldjkdkxu.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.jyoumei.cn/gtvtelkqih.html

/** @param {string} name */ function f(name) {}
来源：http://hz.snrcjt.cn/gtqffakdqo.html

[U117] JS：单元测试
来源：http://hz.daria6918.cn/gtbfpzovfi.html

npm i -D vitest;  npx vitest
来源：http://hz.cashguo.top/gtpxginfue.html

[U118] JS：开发服务器
来源：http://hz.jinghuilouyu.cn/gtdvewhfft.html

npm i -D vite;  npx vite
来源：http://hz.yangfankeji.com/gtwwatknoo.html

[U119] JS：生产构建
来源：http://hz.wangdashe.top/gtcmcxrbym.html

npx vite build
来源：http://hz.tianlin.xyz/gttmgidrbg.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.ybcxt.top/gtxhlkehiw.html

import.meta.env.VITE_API_URL
来源：http://hz.jinqigufen.top/gtuidrcmnn.html

================================================================================
来源：http://hz.jinqigufen.top/gtiiulobsj.html

统计汇总
来源：http://hz.zycfv.cn/gtxswpiits.html

================================================================================
来源：http://hz.hammf.cn/gtrugfezlj.html

按语言统计（条）：
来源：http://hz.sxryk.cn/gtveogpech.html

Python ......... 252
来源：http://hz.bjfxy.top/gtujcjlnpp.html

PHP ............ 252
来源：http://hz.shzxlz.cn/gtiahtounj.html

JavaScript ..... 252
来源：http://hz.feifeiyinyue.top/gtuzexrkcx.html

TypeScript ..... 212
来源：http://hz.vqdsnc.cn/gttzdzkwpr.html

Java ........... 212
来源：http://hz.cucudq.cn/gtubdpncsk.html

Go ............. 212
来源：http://hz.shanyushiyangkeji.top/gtynjdqyvk.html

Ruby ........... 212
来源：http://hz.yj20258.top/gtkrpabuoi.html

C# ............. 212
来源：http://hz.wangshuangyany.cn/gtiadudkce.html

C .............. 30
来源：http://hz.bjfxy.top/gtaxdthohd.html

C++ ............ 30
来源：http://hz.jqgfzy.top/gtkshpkxpy.html

SQL ............ 90
来源：http://hz.9152youxi.cn/gtbillmesi.html

Bash ........... 80
来源：http://hz.zhijiandao.cn/gtumulntoh.html

Kotlin ......... 15
来源：http://hz.aibaodan.cn/gtufrlfvpx.html

Swift .......... 15
来源：http://hz.aibaodan.cn/gtgkbflnvy.html

Lua ............ 10
来源：http://hz.dianchejie.cn/gtxjfmbkof.html

Perl ........... 10
来源：http://hz.ehwqpu.com/gttodhxnai.html

Scala .......... 10
来源：http://hz.yuanzhike.top/gtxnskaszj.html

------------------------------------
来源：http://hz.zhaomingkeji.xyz/gtarewkojh.html

合计 ........... 2106 条
来源：http://hz.zhaomingkeji.xyz/gthqbsaeoz.html

按章节统计：
来源：http://hz.xuanzx.com/gtymxbmrot.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.hammf.cn/gtumrjiyim.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.mhx1999.top/gtrvcklgsm.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.9152youxi.cn/gtaolegree.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.jqgufenzy.top/gtiuogskvv.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.jyoumei.cn/gtrvyuwnfl.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.zhijiandao.cn/gtlvkfqqbg.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.aibaodan.cn/gtheubwkcr.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.haohaochexian.top/gtrobhllmf.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.guowangkeji.top/gtroupmtww.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.redwolf501.top/gtuoupihzf.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.jqgufenzy.top/gtldqbuzvc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.shuidangran.top/gtcllmbrzp.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.ydzc1.top/gtkljhqncu.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.zhiwuduotai.top/gtprhpcszm.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.jianghu66.top/gtumsbbaah.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.yuanzhike.top/gtgscqpovk.html

Q SQL 专题                              90
来源：http://hz.yueranfly.top/gtsggsrdpp.html

R Bash 专题                             80
来源：http://hz.ehwqpu.com/gtokkdjyck.html

S C / C++ 专题                          60
来源：http://hz.birdmap.top/gtlhiwfven.html

T 其他语言补充                          60
来源：http://hz.yuxming.cn/gtmjywjxsc.html

U 高频实用片段                         120
来源：http://hz.havefunace.top/gtfpevftdc.html

------------------------------------
来源：http://hz.hysaishi.cn/gtsjsmpylv.html

合计                                  2106 条
来源：http://hz.jqgfzy.top/gtqrlyepck.html

--------------------------------------------------------------------------------
来源：http://hz.guowangkeji.top/gtfhazdwzw.html

使用提醒
来源：http://hz.iojbl.cn/gtdtoknkbt.html

--------------------------------------------------------------------------------
来源：http://hz.yanxiufei.cn/gtnppiuzhc.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.guannengcc.top/gtkyipyzzc.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.cdnleiting.top/gtolftfvdn.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.yongpay.top/gtayscwnfp.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.316326.xyz/gtovlluhoa.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.yj20258888.top/gtoimtplqv.html

—— 文件结束 ——
来源：http://hz.mhx1999.top/gtyoukykeb.html

================================================================================
来源：http://hz.jinqigfzy.top/gtgyhrutss.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.dianchejie.cn/gtkpgcqide.html

Common Programming Examples Cheat Book
来源：http://hz.hnxiangtu.top/gtyoyyzlzr.html

================================================================================
来源：http://hz.cucudq.cn/gtvxkkzqcw.html

【收录内容】
来源：http://hz.tianlin.xyz/gtsfesveuh.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.gogol.net.cn/gtkwznrobp.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.xziqi.cn/gtcaldodou.html

SQL · Bash · C · C++
来源：http://hz.jinqigfzy.top/gtaxsyzyxq.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.smart0.xyz/gtxtcydxaa.html

【使用说明】
来源：http://hz.yangfankeji.com/gtfjbuljwx.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.shanyushiyangtech.top/gtssgxclwp.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.zdqjudy.top/gtsmxqwsbo.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.wangdashe.top/gtrivlokfp.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.tanke756.top/gtfdxhytpe.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.gotoacloud.top/gtkuxgfptc.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.ydjk.org.cn/gtfmrjmyga.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.sysykeji.top/gtsdovezrf.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.andypj.xyz/gtundgoquu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.cdnleiting.top/gtljcmphhc.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.sysykeji.top/gtauhfghop.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.wangshuangyany.cn/gtwizvqdmx.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.fzhhl.top/gtgxodhnzo.html

【文件统计】
来源：http://hz.wangshuangyany.cn/gtcvdqbnea.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.pengpengdd.cyou/gtwmhoihlo.html

--------------------------------------------------------------------------------
来源：http://hz.yueranfly.top/gtdjpjcmcs.html

目  录
来源：http://hz.andypj.xyz/gtteioihyy.html

--------------------------------------------------------------------------------
来源：http://hz.sxryk.cn/gthbucgerh.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.jinqigufen.top/gthrcgzzdb.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.vqdsnc.cn/gtebcfdyfk.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.cucudq.cn/gtxykymusn.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.sufxvd.cn/gtyrdphsix.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.yuanzhike.top/gtwprbnijd.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.fengsongda.top/gtilqalfxt.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.0kj1m.cn/gtikowcrfi.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.zhongyouzk.top/gtbqxamoqg.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.ivvv.top/gtgktpozgk.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.redwolf501.top/gtijynoyfd.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.jinqigufen.top/gtlbwbjwcz.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.jinqigfzy.top/gtalabpvwc.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.havefunace.top/gtffkshtcg.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.jinyuanbaomall.cn/gtoffhvytx.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.hammf.cn/gtiznazeih.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.shzxlz.cn/gtkbwbrgsg.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.iojbl.cn/gtsxpervmp.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.jinyuanbaomall.cn/gtdelumpqo.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.guowangkeji.top/gttvwmstzt.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hysaishi.cn/gtgvstqvsq.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.jinqigufen.top/gtdlmoxpbh.html

================================================================================
来源：http://hz.yj20258888.top/gtjblflalg.html

A. 基础语法与类型
来源：http://hz.ywan-chungtsiang.top/gtfeyehnvm.html

================================================================================
来源：http://hz.jqgufenzy.top/gtizmptbeo.html

[A01] Hello World
来源：http://hz.birdmap.top/gtwdrffmyf.html

Py:   print("Hello, World!")
来源：http://hz.shuidangran.top/gtldkwhdtj.html

PHP:  echo "Hello, World!";
来源：http://hz.vqdsnc.cn/gtmsqcuakm.html

JS:   console.log("Hello, World!");
来源：http://hz.mhx1999.top/gthizaotmh.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.sysykeji.top/gtvltnxvrw.html

Java: System.out.println("Hello, World!");
来源：http://hz.yongpay.top/gtwjzhkpea.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.xuanzx.com/gtdqaskdqs.html

Ruby: puts "Hello, World!"
来源：http://hz.xingfuxueyuan.xyz/gtzhqsiiva.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.havefunace.top/gttttfpewl.html

[A02] 变量声明与赋值
来源：http://hz.hfpthk.cn/gtahwznbfv.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.tianlin.xyz/gtixhgyorx.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.ydzc1.top/gttnoeatlx.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.sufxvd.cn/gtrmqdrfrr.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.cdnleiting.top/gtxvrrosuc.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.andypj.xyz/gtxcxreyib.html

Go:   name := "Alex"; age := 20
来源：http://hz.jqgufenzy.top/gtvmdpuici.html

Ruby: name = "Alex"; age = 20
来源：http://hz.ivvv.top/gtowvdqyyr.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.daria6918.cn/gtdsqvselr.html

[A03] 常量定义
来源：http://hz.tian-w.cn/gtsksagisn.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.quarkkingdee.top/gtzpmueocf.html

PHP:  const PI = 3.14159;
来源：http://hz.yueranfly.top/gtcxokskkm.html

JS:   const PI = 3.14159;
来源：http://hz.yueranfly.top/gtnyoxqmew.html

TS:   const PI: number = 3.14159;
来源：http://hz.aibaodan.cn/gtlhivqhay.html

Java: static final double PI = 3.14159;
来源：http://hz.gotoacloud.top/gtxznafmlb.html

Go:   const PI = 3.14159
来源：http://hz.316326.xyz/gtlcowcved.html

Ruby: PI = 3.14159
来源：http://hz.ivvv.top/gtwvwoluii.html

C#:   const double PI = 3.14159;
来源：http://hz.9152youxi.cn/gtlomkqutz.html

[A04] 判断变量类型
来源：http://hz.316326.xyz/gtkneexeme.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.shanyushiyangkeji.top/gtrvcxihjw.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.wangdashe.top/gtuviraavx.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.ppjwa.cn/gtuqndclyh.html

TS:   typeof x; x instanceof Date
来源：http://hz.xingfuxueyuan.xyz/gtyfdlxopw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.yangfankeji.com/gtbzksbhzs.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.guannengcc.top/gtttnbiief.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.mhx1999.top/gtfdxflenx.html

C#:   x.GetType().Name; x is int
来源：http://hz.yanxiufei.cn/gteefbbium.html

[A05] 整数除法与取模
来源：http://hz.yj202588.top/gtrgfrzprq.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.c1oappe.top/gtelzqyvfe.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.sweek.top/gtlvikpcdy.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.zhiwuduotai.top/gtawbrrxkd.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.tian-w.cn/gttmdvjuun.html

Java: 7 / 2; 7 % 2
来源：http://hz.pycfn.com/gtpufdgrbj.html

Go:   7 / 2; 7 % 2
来源：http://hz.jinqigfzy.top/gtamztebkb.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.yonumen.top/gtefyfymhv.html

C#:   7 / 2; 7 % 2
来源：http://hz.hnxiangtu.top/gtqyupdqiv.html

[A06] 字符串转数字
来源：http://hz.zhoulong.xyz/gtllgownad.html

Py:   int("42"); float("3.14")
来源：http://hz.iojbl.cn/gtflvgqaas.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.9152youxi.cn/gtlvgoouvq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.mhx1999.top/gtajlzwwdx.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.shanyushiyangkeji.top/gtrbynwfui.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.ywan-chungtsiang.top/gtjbcubvyp.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.chenjidiqi.icu/gtutvsbfyn.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.yangfankeji.com/gtavyrhrhd.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.tian-w.cn/gtodpqsbgo.html

[A07] 数字转字符串
来源：http://hz.ppjwa.cn/gteiaamqvo.html

Py:   str(42)
来源：http://hz.feifeiyinyue.top/gtupznkjbg.html

PHP:  (string) 42; strval(42)
来源：http://hz.tanke756.top/gturjjjwkc.html


<!-- 参考信息 -->