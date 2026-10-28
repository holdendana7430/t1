代发 wailian999

[U55] PHP：match 表达式
来源：http://hz.yuanzhike.top/gttlnhqumo.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.hnqzz.top/gtexgkrjfn.html

[U56] PHP：命名参数
来源：http://hz.jinyuanbaomall.cn/gtllmzzzun.html

f(a: 1, b: 2)
来源：http://hz.xuanzx.com/gtpcmqjhuu.html

[U57] PHP：字符串插值
来源：http://hz.yangfankeji.com/gtpmaqsdni.html

"值: {$a}"
来源：http://hz.zycfv.cn/gtkpvxhqia.html

[U58] PHP：数组三件套
来源：http://hz.aibaodan.cn/gtzpysiskd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.sysykeji.top/gtemgsxvnb.html

[U59] PHP：自定义排序
来源：http://hz.aizwys.cn/gtpzziepyx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.gogol.net.cn/gtsjoqsysu.html

[U60] PHP：JSON 编解码
来源：http://hz.ydjk.org.cn/gtpzkeosgc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.gotoacloud.top/gtivjeqbqn.html

[U61] PHP：正则
来源：http://hz.zhengqikj.top/gtykrktrjn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.quarkkingdee.top/gtiheszqxb.html

[U62] PHP：日期对象
来源：http://hz.zhoulong.xyz/gtnodjvdvq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.chenjidiqi.icu/gtewxzvuwq.html

[U63] PHP：文件读写
来源：http://hz.yj202588.top/gtvmzadwkb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.nanxuanxn.top/gtiupqiklz.html

[U64] PHP：目录遍历
来源：http://hz.zhengqikj.top/gtundfiswv.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.jyoumei.cn/gteyexjhfi.html

[U65] PHP：会话
来源：http://hz.tian-w.cn/gttbjrqgue.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.ydzc1.top/gtdbvvrfey.html

[U66] PHP：设置 Cookie
来源：http://hz.yangfankeji.com/gtxebzxlsh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.zhaomingkeji.xyz/gtzqnxsxnt.html

[U67] PHP：处理文件上传
来源：http://hz.zhongyouzk.top/gtvfonipoj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.hnqzz.top/gtejcdwxxg.html

[U68] PHP：PDO 连接
来源：http://hz.dashuyun.cn/gtucdqmkdt.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.zhixingplan.top/gtequrwzvu.html

[U69] PHP：PDO 预处理
来源：http://hz.chenjidiqi.icu/gtspwulkzz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.nanxinkj.top/gtizffcgck.html

[U70] PHP：PDO 事务
来源：http://hz.chenzaomai.com/gtyrhdetaz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.sxryk.cn/gtfjsbekqu.html

[U71] PHP：抛出异常
来源：http://hz.fzhhl.top/gtrzziusjs.html

throw new RuntimeException("失败", 500);
来源：http://hz.hfpthk.cn/gthseztzxj.html

[U72] PHP：写错误日志
来源：http://hz.jlsjyb.cn/gtjibuuwgk.html

error_log("失败: " . $e->getMessage());
来源：http://hz.kuanghao11.cn/gtgtfdriiw.html

[U73] PHP：读取 ini 配置
来源：http://hz.chenlongwang.top/gtroahrptu.html

parse_ini_file("config.ini", true)
来源：http://hz.vqdsnc.cn/gtbnvvqimc.html

[U74] PHP：读取环境变量
来源：http://hz.dashuyun.cn/gtvjwjtuod.html

getenv("APP_ENV") ?: "production"
来源：http://hz.snrcjt.cn/gtolhqduwi.html

[U75] PHP：依赖注入
来源：http://hz.cheryme.top/gtpfyrotwp.html

composer require psr/container
来源：http://hz.yongpay.top/gtgblkmlnz.html

[U76] PHP：简单路由
来源：http://hz.xinyue.icu/gtkyznqnib.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.yanxiufei.cn/gtxtdmuixm.html

[U77] PHP：模板渲染
来源：http://hz.shanyushiyangtech.top/gtgzlgadej.html

composer require twig/twig
来源：http://hz.c1oappe.top/gtxxdzrulo.html

[U78] PHP：单元测试
来源：http://hz.yuanzhike.top/gtikbwtaqd.html

composer require --dev phpunit/phpunit
来源：http://hz.iojbl.cn/gtyzvmcogr.html

[U79] PHP：静态分析
来源：http://hz.xinyue.icu/gtxjagcwxu.html

composer require --dev phpstan/phpstan
来源：http://hz.kuanghao11.cn/gtdijnbdcx.html

[U80] PHP：代码规范修复
来源：http://hz.redwolf501.top/gtptlzbuny.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.kuanghao11.cn/gtamigxlwv.html

[U81] JS：初始化项目
来源：http://hz.gzhubu.top/gtatciewva.html

npm init -y;  npm i express
来源：http://hz.feifeiyinyue.top/gtsfmqvtyy.html

[U82] JS：package.json 脚本
来源：http://hz.aibaodan.cn/gtciajxvxe.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.kuanghao11.cn/gtvfrxuvin.html

[U83] JS：ES Module 导入导出
来源：http://hz.xziqi.cn/gtqwlmxgrs.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.guannengcc.top/gtubbohauu.html

[U84] JS：CommonJS 写法
来源：http://hz.quarkkingdee.top/gtfqcuuhqr.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.hnxiangtu.top/gtjvhbdrlb.html

[U85] JS：可选链
来源：http://hz.cqqwz.cn/gtixmzwrkq.html

a?.b?.c
来源：http://hz.gogol.net.cn/gtbaciauio.html

[U86] JS：空值合并
来源：http://hz.cqqwz.cn/gtiwzcuffz.html

a ?? b
来源：http://hz.iojbl.cn/gtlrtxwjpy.html

[U87] JS：解构默认值
来源：http://hz.shangyingyoupin.top/gtzwiaesru.html

const { a = 1, b = 2 } = obj;
来源：http://hz.316326.xyz/gtytdmllik.html

[U88] JS：对象展开合并
来源：http://hz.ehwqpu.com/gtcqiewtzv.html

{ ...a, ...b }
来源：http://hz.aibaodan.cn/gtsiwvradc.html

[U89] JS：数组去重
来源：http://hz.tanke756.top/gtpvssjnob.html

[...new Set(arr)]
来源：http://hz.smart0.xyz/gtjndeiwyb.html

[U90] JS：数字数组排序
来源：http://hz.ydzc1.top/gtpwdjepkc.html

[...arr].sort((a, b) => a - b)
来源：http://hz.nanxinkj.top/gttsawvdgy.html

[U91] JS：对象键值遍历
来源：http://hz.hongshengwenyu.top/gtvbyziddy.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.gogol.net.cn/gttvsraaye.html

[U92] JS：深拷贝
来源：http://hz.mhx1999.top/gtbjipbtxf.html

structuredClone(obj)
来源：http://hz.jiagoushi.top/gtybetwzqq.html

[U93] JS：模板字符串
来源：http://hz.shanyushiyangkeji.top/gtdzazcylq.html

`共 ${n} 条`
来源：http://hz.ivvv.top/gtaornokyf.html

[U94] JS：箭头函数
来源：http://hz.mhx1999.top/gtdwthvfyu.html

const double = x => x * 2;
来源：http://hz.gogol.net.cn/gtiklwwiyt.html

[U95] JS：Promise 包装
来源：http://hz.bjfxy.top/gtpgsvyeoq.html

new Promise((resolve, reject) => {})
来源：http://hz.ivvv.top/gtlfjvzeou.html

[U96] JS：async/await 与异常
来源：http://hz.iojbl.cn/gtdrvutzyk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.andypj.xyz/gthdhzrpbk.html

[U97] JS：并发请求
来源：http://hz.smart0.xyz/gtpgckwlud.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.guowangkeji.top/gtnqlozzzd.html

[U98] JS：fetch 带 JSON
来源：http://hz.shuidangran.top/gtlqlxtlzl.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.andypj.xyz/gtdamnizxh.html

[U99] JS：事件监听
来源：http://hz.shangyingyoupin.top/gtufchfgeo.html

el.addEventListener("click", e => {})
来源：http://hz.dianchejie.cn/gtdtsfnmms.html

[U100] JS：DOM 查询
来源：http://hz.shangyingyoupin.top/gtgqynoqmk.html

document.querySelector(".item")
来源：http://hz.c1oappe.top/gtzswstezv.html

[U101] JS：classList 操作
来源：http://hz.cdnleiting.top/gtkwjkhafz.html

el.classList.toggle("active")
来源：http://hz.52xcode.cn/gtszajxgnq.html

[U102] JS：本地存储
来源：http://hz.andypj.xyz/gtsbsenxuf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.zhengqikj.top/gtdbaotsbg.html

[U103] JS：定时器
来源：http://hz.jinqigufen.top/gtajidmhcd.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.hywenlv.cn/gtbzqucorj.html

[U104] JS：防抖
来源：http://hz.zhijiandao.cn/gtybbiuzrp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cashguo.top/gtqvbiibdc.html

[U105] JS：节流
来源：http://hz.ydzc1.top/gtqkzurqdy.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.sufxvd.cn/gtjpogiffi.html

[U106] JS：日期格式化
来源：http://hz.zhoulong.xyz/gtxunqehic.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.fengsongda.top/gtlnpkmyzc.html

[U107] JS：数字千分位
来源：http://hz.52xcode.cn/gtfihjexeb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.chenzaomai.com/gttjgnhcqa.html

[U108] JS：随机整数
来源：http://hz.jinyuanbaomall.cn/gtxazgbyie.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.pycfn.com/gtqckadsal.html

[U109] JS：数组分组
来源：http://hz.zhongyouzk.top/gtfeiliqwn.html

Object.groupBy(arr, x => x.type)
来源：http://hz.cheryme.top/gteynbcabt.html

[U110] JS：数组分块
来源：http://hz.tanke756.top/gtjtwjqdvm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.fengsongda.top/gtmxzdtxcc.html

[U111] JS：对象转 Map
来源：http://hz.hysaishi.cn/gtcmcsznld.html

new Map(Object.entries(obj))
来源：http://hz.xziqi.cn/gtdzlmpmfx.html

[U112] JS：字符串补位
来源：http://hz.zhijiandao.cn/gtyqgjvjxq.html

"7".padStart(3, "0")
来源：http://hz.svipenyu.cn/gtznjrpque.html

[U113] JS：正则替换全部
来源：http://hz.shanyushiyangtech.top/gtxuhfwnsg.html

s.replaceAll("a", "b")
来源：http://hz.cqqwz.cn/gtlmwycxyu.html

[U114] JS：JSON 深比较
来源：http://hz.zycfv.cn/gtwisbrnlq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.cucudq.cn/gtozizkspb.html

[U115] JS：生成 UUID
来源：http://hz.andypj.xyz/gtzmccbwoo.html

crypto.randomUUID()
来源：http://hz.andypj.xyz/gtvivgxrpk.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.0kj1m.cn/gtntbpccqw.html

/** @param {string} name */ function f(name) {}
来源：http://hz.shangyingyoupin.top/gtttgpgfcn.html

[U117] JS：单元测试
来源：http://hz.shangyingyoupin.top/gtupplmdnv.html

npm i -D vitest;  npx vitest
来源：http://hz.yuxming.cn/gtvyomgpzi.html

[U118] JS：开发服务器
来源：http://hz.xinyue.icu/gtlpbtfdhd.html

npm i -D vite;  npx vite
来源：http://hz.cdnleiting.top/gtwugirhng.html

[U119] JS：生产构建
来源：http://hz.ppjwa.cn/gtxccuyzxi.html

npx vite build
来源：http://hz.mhx1999.top/gthpookujo.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.smart0.xyz/gtoopwvaqb.html

import.meta.env.VITE_API_URL
来源：http://hz.yanxiufei.cn/gtcvbhbtdr.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtorohrqem.html

统计汇总
来源：http://hz.cashguo.top/gtmxdvvphf.html

================================================================================
来源：http://hz.snrcjt.cn/gtzmdxcyax.html

按语言统计（条）：
来源：http://hz.wangshuangyany.cn/gtxemzsgkr.html

Python ......... 252
来源：http://hz.daxiang520.top/gtcnxztkpy.html

PHP ............ 252
来源：http://hz.quarkkingdee.top/gtxtfgggrr.html

JavaScript ..... 252
来源：http://hz.shzxlz.cn/gtmeuglxxq.html

TypeScript ..... 212
来源：http://hz.ywan-chungtsiang.top/gtxjzqrwot.html

Java ........... 212
来源：http://hz.jinghuilouyu.cn/gtlboxymjb.html

Go ............. 212
来源：http://hz.haohaochexian.top/gtaftnuksh.html

Ruby ........... 212
来源：http://hz.guowangkeji.top/gtwnbgckvz.html

C# ............. 212
来源：http://hz.ydjk.org.cn/gtgmqsulld.html

C .............. 30
来源：http://hz.chenzaomai.com/gtabnyrysz.html

C++ ............ 30
来源：http://hz.ivvv.top/gtdlfbwtvv.html

SQL ............ 90
来源：http://hz.bjfxy.top/gtzhmqkcmk.html

Bash ........... 80
来源：http://hz.sxryk.cn/gtdbolnoxa.html

Kotlin ......... 15
来源：http://hz.jiagoushi.top/gtpsywhxtk.html

Swift .......... 15
来源：http://hz.ydjk.org.cn/gtfqztuohc.html

Lua ............ 10
来源：http://hz.guowangkeji.top/gteuirwrds.html

Perl ........... 10
来源：http://hz.hfpthk.cn/gtjhtjwyoa.html

Scala .......... 10
来源：http://hz.dashuyun.cn/gtobyggetm.html

------------------------------------
来源：http://hz.hammf.cn/gtsmzcelee.html

合计 ........... 2106 条
来源：http://hz.chenlongwang.top/gtchfroluh.html

按章节统计：
来源：http://hz.zhaomingkeji.xyz/gtfkheibfi.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.xingfuxueyuan.xyz/gtcrbrfbph.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.fzhhl.top/gtdqiovwpy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.xziqi.cn/gtkriwkyxr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.ydjk.org.cn/gtqaukkzct.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.shuidangran.top/gtpasticbr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.316326.xyz/gtafjjfhqi.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.jianghu66.top/gtdumbpgpc.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.dianchejie.cn/gtmwmizhdx.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.guannengcc.top/gtgiediowg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.fzhhl.top/gtforpxnks.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.dianchejie.cn/gtymsvxdnh.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.zhengqikj.top/gtrlzmwkej.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.meibo888.top/gtanzqcehr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.316326.xyz/gtgkjxgpmw.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.c1oappe.top/gtoilexkfi.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.cheryme.top/gtgdysmcez.html

Q SQL 专题                              90
来源：http://hz.shanyushiyangkeji.top/gtaxgggcqw.html

R Bash 专题                             80
来源：http://hz.cdnleiting.top/gtsvlmzlks.html

S C / C++ 专题                          60
来源：http://hz.nanxinkj.top/gtaevifdpf.html

T 其他语言补充                          60
来源：http://hz.zhaomingkeji.xyz/gtgdtmsbuw.html

U 高频实用片段                         120
来源：http://hz.zdqjudy.top/gtouqzvyci.html

------------------------------------
来源：http://hz.9152youxi.cn/gtqictszju.html

合计                                  2106 条
来源：http://hz.ehwqpu.com/gtfzksnesu.html

--------------------------------------------------------------------------------
来源：http://hz.9152youxi.cn/gtflzfoups.html

使用提醒
来源：http://hz.havefunace.top/gtjagyonxf.html

--------------------------------------------------------------------------------
来源：http://hz.sysykeji.top/gtsgefeusa.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.shangyingyoupin.top/gtbskuskbd.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.chenjidiqi.icu/gtitdfpaao.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.zhongyouzk.top/gtpvrpdhhj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.jyoumei.cn/gtnqmzaypy.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.zhaomingkeji.xyz/gtqhexdtbf.html

—— 文件结束 ——
来源：http://hz.ehwqpu.com/gtnzlxvsez.html

================================================================================
来源：http://hz.yj202588.top/gtmbhewwfd.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.pengpengdd.cyou/gtfzlbasdc.html

Common Programming Examples Cheat Book
来源：http://hz.9152youxi.cn/gtcxjbnacv.html

================================================================================
来源：http://hz.cashguo.top/gthncozfij.html

【收录内容】
来源：http://hz.hnqzz.top/gtdpjgufuo.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.9152youxi.cn/gtfukqdrjb.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.gotoacloud.top/gteysbyito.html

SQL · Bash · C · C++
来源：http://hz.aizwys.cn/gtmdgupvnb.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.sxryk.cn/gtxrreowml.html

【使用说明】
来源：http://hz.yj20258888.top/gtjxfqsblr.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.daria6918.cn/gtvxmrbbnb.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.jqgufenzy.top/gtsdyumngc.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.snrcjt.cn/gtujztwfmg.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.52xcode.cn/gthmymrcsz.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.cheryme.top/gtsrssbqmd.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.wangshuangyany.cn/gttbdzongf.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.sufxvd.cn/gtmvnuanbr.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.52xcode.cn/gtjhiyaydj.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.dashuyun.cn/gtnxbmuhhi.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.chenzaomai.com/gtpshzftxr.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.dashuyun.cn/gtbusrjqts.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.sxryk.cn/gtzvqmkxtb.html

【文件统计】
来源：http://hz.cheryme.top/gtiifzgriw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.jqgfzy.top/gtoyatidxw.html

--------------------------------------------------------------------------------
来源：http://hz.shanyushiyangkeji.top/gtqzpeaoeo.html

目  录
来源：http://hz.zhengqikj.top/gtlbzwtsja.html

--------------------------------------------------------------------------------
来源：http://hz.hfpthk.cn/gtdqwbjdfx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.pycfn.com/gtoitvmcgz.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.wangdashe.top/gtgphxvbjf.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.andypj.xyz/gtlpkskcoz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.jqgufenzy.top/gtlhewgkgr.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.mhx1999.top/gtjsnwoctf.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.tanke756.top/gtcpuokssu.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.xuetiantiany.cn/gtjurpeoos.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.c1oappe.top/gtytojklew.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.gogol.net.cn/gtdzrhrmbn.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.zdqjudy.top/gtzgnyyakk.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.shanyushiyangkeji.top/gtnhmyoczu.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.xziqi.cn/gthjuvqzlj.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.tian-w.cn/gtzmiemjbx.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.aibaodan.cn/gtossnyjdc.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.jlsjyb.cn/gtjlipezxl.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.ywan-chungtsiang.top/gtukxlgxbt.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.yueranfly.top/gtjbmgbttu.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.sxryk.cn/gtdjbosfdv.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.snrcjt.cn/gtlfnmqooq.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.sufxvd.cn/gtzmmclhxa.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.fzhhl.top/gtzfapuwim.html

================================================================================
来源：http://hz.sweek.top/gtfkfkpgkr.html

A. 基础语法与类型
来源：http://hz.andypj.xyz/gtvtxafvom.html

================================================================================
来源：http://hz.cdnleiting.top/gtczwdeeel.html

[A01] Hello World
来源：http://hz.andypj.xyz/gtoavwuhyw.html

Py:   print("Hello, World!")
来源：http://hz.ydzc1.top/gthlwajiaz.html

PHP:  echo "Hello, World!";
来源：http://hz.ydzc1.top/gtsuvqxoht.html

JS:   console.log("Hello, World!");
来源：http://hz.yj20258888.top/gtcoxygtrv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.yanxiufei.cn/gtbatlewbo.html

Java: System.out.println("Hello, World!");
来源：http://hz.wangdashe.top/gtbhpvzwdi.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.sweek.top/gtpqkdyoix.html

Ruby: puts "Hello, World!"
来源：http://hz.dashuyun.cn/gtbybymmmv.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.hnxiangtu.top/gtvyivulxd.html

[A02] 变量声明与赋值
来源：http://hz.gogol.net.cn/gthmmunttk.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.birdmap.top/gteolmefhj.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.shzxlz.cn/gtlqvvxjzb.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.ehwqpu.com/gtpanwwmzm.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.ppjwa.cn/gtyehowcbt.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.nanxuanxn.top/gtzjkvvwoa.html

Go:   name := "Alex"; age := 20
来源：http://hz.sxryk.cn/gttskkaahe.html

Ruby: name = "Alex"; age = 20
来源：http://hz.fengsongda.top/gtmlmdinnl.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.gaohongyu789.top/gtdhljklit.html

[A03] 常量定义
来源：http://hz.yj202588.top/gtiulfievz.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.yonumen.top/gtpngkhsvw.html

PHP:  const PI = 3.14159;
来源：http://hz.feifeiyinyue.top/gtgmygkvkp.html

JS:   const PI = 3.14159;
来源：http://hz.nanxinkj.top/gtxodozswf.html

TS:   const PI: number = 3.14159;
来源：http://hz.aizwys.cn/gthxyhlxjs.html

Java: static final double PI = 3.14159;
来源：http://hz.shanyushiyangkeji.top/gtcjivugcf.html

Go:   const PI = 3.14159
来源：http://hz.xziqi.cn/gtfvukpfcq.html

Ruby: PI = 3.14159
来源：http://hz.chenjidiqi.icu/gtjvofrfer.html

C#:   const double PI = 3.14159;
来源：http://hz.cqqwz.cn/gthatalkya.html

[A04] 判断变量类型
来源：http://hz.yangfankeji.com/gtophlowbh.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.wangdashe.top/gtcdywjloj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.feifeiyinyue.top/gtvdkpgiie.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.nwbrower.top/gtbtpvrspc.html

TS:   typeof x; x instanceof Date
来源：http://hz.shzxlz.cn/gtxhdlflki.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.yj20258.top/gteiyypeiq.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.yonumen.top/gtogfocwmr.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.wangshuangyany.cn/gtwpuvwrcp.html

C#:   x.GetType().Name; x is int
来源：http://hz.9152youxi.cn/gtcyngumam.html

[A05] 整数除法与取模
来源：http://hz.redwolf501.top/gttqaokteu.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.aizwys.cn/gtyohdjjvy.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.fzhhl.top/gtuzmojwex.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.ybcxt.top/gtaepctket.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.tianlin.xyz/gtondupkrl.html

Java: 7 / 2; 7 % 2
来源：http://hz.cdnleiting.top/gtldikopol.html

Go:   7 / 2; 7 % 2
来源：http://hz.aibaodan.cn/gtuqfqciyt.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.hnxiangtu.top/gtbugnsfbf.html

C#:   7 / 2; 7 % 2
来源：http://hz.316326.xyz/gthagmfshn.html

[A06] 字符串转数字
来源：http://hz.gotoacloud.top/gtsbjmmbyn.html

Py:   int("42"); float("3.14")
来源：http://hz.jyoumei.cn/gtusyhzkcg.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.daria6918.cn/gtjfqgtxhm.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.jinqigfzy.top/gtgjssscvj.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.hywenlv.cn/gthswsanht.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.tian-w.cn/gtimqpabvm.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.andypj.xyz/gtrobmwkzx.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.gzhubu.top/gtygtisyqo.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.sxryk.cn/gtbqwgpvhc.html

[A07] 数字转字符串
来源：http://hz.iojbl.cn/gtegllzezl.html

Py:   str(42)
来源：http://hz.havefunace.top/gtqmaknzxa.html

PHP:  (string) 42; strval(42)
来源：http://hz.yueranfly.top/gteztmiaxb.html

JS:   String(42); (42).toString()
来源：http://hz.redwolf501.top/gtdspkwwvs.html

TS:   String(42)
来源：http://hz.ehwqpu.com/gtfrybvucs.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.hnxiangtu.top/gtnguktwnp.html

Go:   strconv.Itoa(42)
来源：http://hz.zhoulong.xyz/gtukujilgn.html


<!-- 参考信息 -->