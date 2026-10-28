代发 wailian999

[U53] PHP：空合并运算符
来源：http://hz.mhx1999.top/gtggkoefgt.html

$v = $a ?? $b ?? "default";
来源：http://hz.jqgufenzy.top/gtcjvqomub.html

[U54] PHP：空安全调用
来源：http://hz.cucudq.cn/gtafzvcjlq.html

$obj?->method()
来源：http://hz.zdqjudy.top/gtfnjkzjdn.html

[U55] PHP：match 表达式
来源：http://hz.zycfv.cn/gtcdiwipjf.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.redwolf501.top/gtowpbzgyk.html

[U56] PHP：命名参数
来源：http://hz.yj20258.top/gtpziiglce.html

f(a: 1, b: 2)
来源：http://hz.daria6918.cn/gtezjzrpip.html

[U57] PHP：字符串插值
来源：http://hz.aibaodan.cn/gtrqcjodhq.html

"值: {$a}"
来源：http://hz.yvedp.cn/gtrrkdreoy.html

[U58] PHP：数组三件套
来源：http://hz.aibaodan.cn/gtwzoloifj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.cheryme.top/gtkogtryok.html

[U59] PHP：自定义排序
来源：http://hz.yongpay.top/gtzjurlrjj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.daxiang520.top/gtsuoxbohc.html

[U60] PHP：JSON 编解码
来源：http://hz.zycfv.cn/gtgvfcomww.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.chenjidiqi.icu/gtqtwnvnqs.html

[U61] PHP：正则
来源：http://hz.zycfv.cn/gtpgwsbwsi.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.jiagoushi.top/gtvcrsgndx.html

[U62] PHP：日期对象
来源：http://hz.hammf.cn/gtdxsbhenl.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.316326.xyz/gthvngnjgz.html

[U63] PHP：文件读写
来源：http://hz.shangyingyoupin.top/gtjxstgpag.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.c1oappe.top/gtuoslzyra.html

[U64] PHP：目录遍历
来源：http://hz.sweek.top/gthosennyr.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.hongshengwenyu.top/gttgnwpqaq.html

[U65] PHP：会话
来源：http://hz.daria6918.cn/gtykwuogrl.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.guowangkeji.top/gtnlivxzoy.html

[U66] PHP：设置 Cookie
来源：http://hz.hywenlv.cn/gtuczmbexf.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.smart0.xyz/gthdnivdva.html

[U67] PHP：处理文件上传
来源：http://hz.ydzc1.top/gtobtxmqxn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.xziqi.cn/gtujhnjnyp.html

[U68] PHP：PDO 连接
来源：http://hz.snrcjt.cn/gtdxdoyheh.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.shangyingyoupin.top/gtdmmakviw.html

[U69] PHP：PDO 预处理
来源：http://hz.hywenlv.cn/gtlssruzmd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.feifeiyinyue.top/gtcvdmheiz.html

[U70] PHP：PDO 事务
来源：http://hz.snrcjt.cn/gtebuqndxf.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.jqgfzy.top/gtpaedjlnf.html

[U71] PHP：抛出异常
来源：http://hz.yonumen.top/gtnmtwugpm.html

throw new RuntimeException("失败", 500);
来源：http://hz.zycfv.cn/gtwazuiowu.html

[U72] PHP：写错误日志
来源：http://hz.fengsongda.top/gtobggbcqw.html

error_log("失败: " . $e->getMessage());
来源：http://hz.yanxiufei.cn/gtkpeeqpef.html

[U73] PHP：读取 ini 配置
来源：http://hz.pengpengdd.cyou/gtpcpjszix.html

parse_ini_file("config.ini", true)
来源：http://hz.shanyushiyangkeji.top/gtofifnfsp.html

[U74] PHP：读取环境变量
来源：http://hz.pycfn.com/gtkdisqlry.html

getenv("APP_ENV") ?: "production"
来源：http://hz.sxryk.cn/gtlwatvxmj.html

[U75] PHP：依赖注入
来源：http://hz.tian-w.cn/gtshyjsbao.html

composer require psr/container
来源：http://hz.jqgfzy.top/gtbegjhcqd.html

[U76] PHP：简单路由
来源：http://hz.gzhubu.top/gtswkjxoqo.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.nanxuanxn.top/gtvgafsvad.html

[U77] PHP：模板渲染
来源：http://hz.xziqi.cn/gtdrwhoywe.html

composer require twig/twig
来源：http://hz.cqqwz.cn/gtmhbqnhjn.html

[U78] PHP：单元测试
来源：http://hz.jinghuilouyu.cn/gttbernsiy.html

composer require --dev phpunit/phpunit
来源：http://hz.kuanghao11.cn/gtpasajhcr.html

[U79] PHP：静态分析
来源：http://hz.sxryk.cn/gtabdmtebf.html

composer require --dev phpstan/phpstan
来源：http://hz.9152youxi.cn/gthvdbbktj.html

[U80] PHP：代码规范修复
来源：http://hz.wangshuangyany.cn/gtgxarwggf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.fengsongda.top/gtteylgkll.html

[U81] JS：初始化项目
来源：http://hz.fengsongda.top/gtszokwxrj.html

npm init -y;  npm i express
来源：http://hz.snrcjt.cn/gttizbtqzz.html

[U82] JS：package.json 脚本
来源：http://hz.yvedp.cn/gttphulvrk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.yongpay.top/gtjmgkzrob.html

[U83] JS：ES Module 导入导出
来源：http://hz.zhengqikj.top/gtmfvwerre.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.shanyushiyangkeji.top/gtawyiymtr.html

[U84] JS：CommonJS 写法
来源：http://hz.nwbrower.top/gtcvqxdpkx.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.pycfn.com/gtygpihntg.html

[U85] JS：可选链
来源：http://hz.zycfv.cn/gtnehwhbeg.html

a?.b?.c
来源：http://hz.dianchejie.cn/gtfwrrrtbz.html

[U86] JS：空值合并
来源：http://hz.sxryk.cn/gtpkmwuafp.html

a ?? b
来源：http://hz.yvedp.cn/gtzqvrndcz.html

[U87] JS：解构默认值
来源：http://hz.feifeiyinyue.top/gtllnshmms.html

const { a = 1, b = 2 } = obj;
来源：http://hz.quarkkingdee.top/gtxiufqovb.html

[U88] JS：对象展开合并
来源：http://hz.ybcxt.top/gtedsziobz.html

{ ...a, ...b }
来源：http://hz.zhoulong.xyz/gteapcbebb.html

[U89] JS：数组去重
来源：http://hz.sufxvd.cn/gttihgbtgf.html

[...new Set(arr)]
来源：http://hz.ehwqpu.com/gtntgwnjfq.html

[U90] JS：数字数组排序
来源：http://hz.dianchejie.cn/gtpsdeqmel.html

[...arr].sort((a, b) => a - b)
来源：http://hz.52xcode.cn/gtvacmawiv.html

[U91] JS：对象键值遍历
来源：http://hz.zdqjudy.top/gtbwuadrxf.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.zhixingplan.top/gtcsgfdgnl.html

[U92] JS：深拷贝
来源：http://hz.jqgfzy.top/gtaxcorutg.html

structuredClone(obj)
来源：http://hz.hysaishi.cn/gtzkzxakem.html

[U93] JS：模板字符串
来源：http://hz.hammf.cn/gtvsidscix.html

`共 ${n} 条`
来源：http://hz.sweek.top/gtmyfmrbcv.html

[U94] JS：箭头函数
来源：http://hz.tanke756.top/gtrbnrayzm.html

const double = x => x * 2;
来源：http://hz.wangdashe.top/gtscbkeigq.html

[U95] JS：Promise 包装
来源：http://hz.tian-w.cn/gtvcimpplw.html

new Promise((resolve, reject) => {})
来源：http://hz.havefunace.top/gthrbkyhvw.html

[U96] JS：async/await 与异常
来源：http://hz.yuxming.cn/gttieryiap.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.bjfxy.top/gtflrnmpxo.html

[U97] JS：并发请求
来源：http://hz.zhoulong.xyz/gtpjkxfdwb.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhiwuduotai.top/gtpyrtiihv.html

[U98] JS：fetch 带 JSON
来源：http://hz.jinyuanbaomall.cn/gtnsbglihx.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.guowangkeji.top/gtrxwkpolb.html

[U99] JS：事件监听
来源：http://hz.guowangkeji.top/gtqjxnnvet.html

el.addEventListener("click", e => {})
来源：http://hz.cdnleiting.top/gtxxnjaukm.html

[U100] JS：DOM 查询
来源：http://hz.xuetiantiany.cn/gtatovcxzu.html

document.querySelector(".item")
来源：http://hz.ydjk.org.cn/gtdntalkte.html

[U101] JS：classList 操作
来源：http://hz.redwolf501.top/gtufazbkjr.html

el.classList.toggle("active")
来源：http://hz.wangshuangyany.cn/gtskmrfvub.html

[U102] JS：本地存储
来源：http://hz.feifeiyinyue.top/gtwbfvpvdd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.aizwys.cn/gtrgyibkze.html

[U103] JS：定时器
来源：http://hz.cdnleiting.top/gtjhqszmhr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.jlsjyb.cn/gtmmdudvmq.html

[U104] JS：防抖
来源：http://hz.9152youxi.cn/gthspyiboe.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yueranfly.top/gtzgntcwit.html

[U105] JS：节流
来源：http://hz.haohaochexian.top/gtxfrmatmj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.jlsjyb.cn/gtqtnuyxxf.html

[U106] JS：日期格式化
来源：http://hz.sysykeji.top/gtmrcrnbeq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.fzhhl.top/gtybsdobpl.html

[U107] JS：数字千分位
来源：http://hz.hongshengwenyu.top/gtmhqunndx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.pycfn.com/gttvgsfocp.html

[U108] JS：随机整数
来源：http://hz.zhijiandao.cn/gtouavblpq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.yueranfly.top/gtjfdbidxt.html

[U109] JS：数组分组
来源：http://hz.cdnleiting.top/gtsmsfqitk.html

Object.groupBy(arr, x => x.type)
来源：http://hz.daria6918.cn/gtcutoughe.html

[U110] JS：数组分块
来源：http://hz.jqgufenzy.top/gtspbngoet.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.yj20258.top/gtqhwjusfe.html

[U111] JS：对象转 Map
来源：http://hz.meibo888.top/gtmiavfguj.html

new Map(Object.entries(obj))
来源：http://hz.ywan-chungtsiang.top/gtqxoumdeu.html

[U112] JS：字符串补位
来源：http://hz.cucudq.cn/gtwrphnzfw.html

"7".padStart(3, "0")
来源：http://hz.ivvv.top/gtlwirnuap.html

[U113] JS：正则替换全部
来源：http://hz.jinqigfzy.top/gtebndipwq.html

s.replaceAll("a", "b")
来源：http://hz.zhijiandao.cn/gtfzikiolc.html

[U114] JS：JSON 深比较
来源：http://hz.zhiwuduotai.top/gtsudnnhnc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shanyushiyangtech.top/gtcvrsdhpj.html

[U115] JS：生成 UUID
来源：http://hz.tianlin.xyz/gtedzxjttv.html

crypto.randomUUID()
来源：http://hz.shanyushiyangtech.top/gtnspewdih.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.aibaodan.cn/gtjmdmhoab.html

/** @param {string} name */ function f(name) {}
来源：http://hz.gaohongyu789.top/gtidsszhps.html

[U117] JS：单元测试
来源：http://hz.hysaishi.cn/gtbazvafpf.html

npm i -D vitest;  npx vitest
来源：http://hz.jlsjyb.cn/gtyzgerodf.html

[U118] JS：开发服务器
来源：http://hz.xziqi.cn/gtfygxgdoa.html

npm i -D vite;  npx vite
来源：http://hz.yangfankeji.com/gtmdamzqmk.html

[U119] JS：生产构建
来源：http://hz.daria6918.cn/gtitioshyb.html

npx vite build
来源：http://hz.jlsjyb.cn/gttvynkwdu.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.tianlin.xyz/gtrurtmazo.html

import.meta.env.VITE_API_URL
来源：http://hz.yj20258888.top/gtxpzqdylo.html

================================================================================
来源：http://hz.cqqwz.cn/gtekzisaym.html

统计汇总
来源：http://hz.shangyingyoupin.top/gteddzqkjg.html

================================================================================
来源：http://hz.xziqi.cn/gtuwkghtcy.html

按语言统计（条）：
来源：http://hz.chenjidiqi.icu/gtdtglgtxv.html

Python ......... 252
来源：http://hz.snrcjt.cn/gtsoluhphi.html

PHP ............ 252
来源：http://hz.zycfv.cn/gtabskjeis.html

JavaScript ..... 252
来源：http://hz.xylfe.cn/gtazpfizsz.html

TypeScript ..... 212
来源：http://hz.wangdashe.top/gtdheabxvf.html

Java ........... 212
来源：http://hz.quarkkingdee.top/gtvqvuvlsx.html

Go ............. 212
来源：http://hz.wangshuangyany.cn/gtstihmaog.html

Ruby ........... 212
来源：http://hz.zhongyouzk.top/gtpsyrvgod.html

C# ............. 212
来源：http://hz.meibo888.top/gtojcwhwrk.html

C .............. 30
来源：http://hz.smart0.xyz/gtvypezcmk.html

C++ ............ 30
来源：http://hz.sxryk.cn/gtwfabjeed.html

SQL ............ 90
来源：http://hz.ydjk.org.cn/gttehbylnn.html

Bash ........... 80
来源：http://hz.zhixingplan.top/gthxlrcogk.html

Kotlin ......... 15
来源：http://hz.zhengqikj.top/gtzstbxwoo.html

Swift .......... 15
来源：http://hz.zhijiandao.cn/gtbpuwkxnl.html

Lua ............ 10
来源：http://hz.xingfuxueyuan.xyz/gtdlpldnso.html

Perl ........... 10
来源：http://hz.gzhubu.top/gtdhpllnrv.html

Scala .......... 10
来源：http://hz.xingfuxueyuan.xyz/gtmivahbic.html

------------------------------------
来源：http://hz.zhoulong.xyz/gtjtpihsko.html

合计 ........... 2106 条
来源：http://hz.jiagoushi.top/gthanwsguc.html

按章节统计：
来源：http://hz.chenlongwang.top/gtgvrugjab.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.chenzaomai.com/gtqbzkryxz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.zhaomingkeji.xyz/gtiuaqwoer.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.sxryk.cn/gtvhaobaui.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.nwbrower.top/gtbsdnyxuf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.meibo888.top/gtdlwlevzp.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.zhaomingkeji.xyz/gttcyhtcmn.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.meibo888.top/gtuaovfgvl.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.chenzaomai.com/gtfuavtzgw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.52xcode.cn/gtxihavmzc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.snrcjt.cn/gtsdhwohmk.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.yj20258888.top/gtlgjswols.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.guowangkeji.top/gteunkdopn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.yj202588.top/gtymjhysvy.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.zhiwuduotai.top/gtdwlbokkw.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.shanyushiyangkeji.top/gtnluqmrkw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.52xcode.cn/gtjktlpczx.html

Q SQL 专题                              90
来源：http://hz.yongpay.top/gtfoosgapd.html

R Bash 专题                             80
来源：http://hz.sxryk.cn/gtzqqwjxpv.html

S C / C++ 专题                          60
来源：http://hz.jinqigufen.top/gtkzxdxqfy.html

T 其他语言补充                          60
来源：http://hz.yj202588.top/gtqboafrtg.html

U 高频实用片段                         120
来源：http://hz.yuxming.cn/gtctanafaw.html

------------------------------------
来源：http://hz.9152youxi.cn/gtpqndanaa.html

合计                                  2106 条
来源：http://hz.yueranfly.top/gtmzpccfqm.html

--------------------------------------------------------------------------------
来源：http://hz.ehwqpu.com/gtbldbvbkj.html

使用提醒
来源：http://hz.xingfuxueyuan.xyz/gtehogjbcj.html

--------------------------------------------------------------------------------
来源：http://hz.52xcode.cn/gtnprdypyo.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.redwolf501.top/gtyiqvmoqf.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.redwolf501.top/gteunykjfx.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.jyoumei.cn/gtxhpseztf.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.nanxuanxn.top/gtyljxuswf.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.jinqigufen.top/gtsxernbxg.html

—— 文件结束 ——
来源：http://hz.fzhhl.top/gtgwrjlmmg.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtynjqaelc.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.tian-w.cn/gtlzqyuyfj.html

Common Programming Examples Cheat Book
来源：http://hz.hysaishi.cn/gtymfcfyko.html

================================================================================
来源：http://hz.andypj.xyz/gtqxrbrdsy.html

【收录内容】
来源：http://hz.quarkkingdee.top/gtabvvccmu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.cdnleiting.top/gtszfltlug.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.jyoumei.cn/gtouhdlkpx.html

SQL · Bash · C · C++
来源：http://hz.316326.xyz/gtlgxbaxgl.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.dianchejie.cn/gtqaptdnxy.html

【使用说明】
来源：http://hz.yanxiufei.cn/gtvtkkutsl.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.ivvv.top/gtefyvgoxc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.daxiang520.top/gtnnxutplv.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.sysykeji.top/gtydkxxlio.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.zhongyouzk.top/gtlwltjpdv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.zhijiandao.cn/gtsexznqep.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.ywan-chungtsiang.top/gtgquqsiwu.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.xinyue.icu/gtboqetcjz.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.iojbl.cn/gtnkmqzfsr.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.hysaishi.cn/gtfzcmhsyd.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.zhengqikj.top/gtnysajbth.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.havefunace.top/gtrwigyyhe.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.ybcxt.top/gtcilpkrjg.html

【文件统计】
来源：http://hz.meibo888.top/gtdhpxzfya.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.zhongyouzk.top/gtykqkgwic.html

--------------------------------------------------------------------------------
来源：http://hz.jinyuanbaomall.cn/gtvgaadian.html

目  录
来源：http://hz.nwbrower.top/gtxslhjecb.html

--------------------------------------------------------------------------------
来源：http://hz.zdqjudy.top/gtjxhastca.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.zhixingplan.top/gtudajdzts.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.jyoumei.cn/gtpbmylzxb.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.hammf.cn/gtdzfpwwgx.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.feifeiyinyue.top/gtcxyhtznq.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.tianlin.xyz/gtkoeincyk.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.jinghuilouyu.cn/gtcpphxdaj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.ydjk.org.cn/gtjvcilfrc.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.hammf.cn/gtqccizxjm.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.kuanghao11.cn/gtbdkayqgl.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.quarkkingdee.top/gtmethahmk.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.tianlin.xyz/gtffkhngif.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.cucudq.cn/gtrdbspiln.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.cucudq.cn/gtmnqvqsea.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.hfpthk.cn/gtgdkcluru.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.gzhubu.top/gtsexmqnqe.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.guowangkeji.top/gtbejmcqvq.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.aizwys.cn/gtczlgvvbv.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.yuanzhike.top/gtvvdslngf.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.snrcjt.cn/gtngbrtwmz.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.xylfe.cn/gtyaeehxdm.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.gaohongyu789.top/gtjcqdmnzn.html

================================================================================
来源：http://hz.iojbl.cn/gtyvvfbzsy.html

A. 基础语法与类型
来源：http://hz.zdqjudy.top/gtxsobgyfk.html

================================================================================
来源：http://hz.zhoulong.xyz/gteycgymof.html

[A01] Hello World
来源：http://hz.xuanzx.com/gtyyqsrzja.html

Py:   print("Hello, World!")
来源：http://hz.shanyushiyangkeji.top/gtcqkbazxh.html

PHP:  echo "Hello, World!";
来源：http://hz.wangdashe.top/gtrnmdxbdd.html

JS:   console.log("Hello, World!");
来源：http://hz.zhengqikj.top/gtvdeamkoc.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.9152youxi.cn/gtsftcqnvn.html

Java: System.out.println("Hello, World!");
来源：http://hz.cqqwz.cn/gtxnpqjbbk.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.chenjidiqi.icu/gtphenrllx.html

Ruby: puts "Hello, World!"
来源：http://hz.yangfankeji.com/gtdwdatavl.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.quarkkingdee.top/gtuvbtvoxl.html

[A02] 变量声明与赋值
来源：http://hz.zycfv.cn/gtrvvpxofo.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.meibo888.top/gtcstnseqe.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.shuidangran.top/gtorutcbhi.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.316326.xyz/gtodahrycp.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.jyoumei.cn/gtnvkwubbb.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.0kj1m.cn/gtjogbxxud.html

Go:   name := "Alex"; age := 20
来源：http://hz.c1oappe.top/gtrbeyolny.html

Ruby: name = "Alex"; age = 20
来源：http://hz.jqgufenzy.top/gtfbenvene.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.tianlin.xyz/gtxhotgzoc.html

[A03] 常量定义
来源：http://hz.daria6918.cn/gtmxmddbmk.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.ivvv.top/gthcysclgm.html

PHP:  const PI = 3.14159;
来源：http://hz.yongpay.top/gthzqbsydg.html

JS:   const PI = 3.14159;
来源：http://hz.daria6918.cn/gtqmkqskzi.html

TS:   const PI: number = 3.14159;
来源：http://hz.shuidangran.top/gtibjlcnxc.html

Java: static final double PI = 3.14159;
来源：http://hz.shanyushiyangtech.top/gtjpveeoad.html

Go:   const PI = 3.14159
来源：http://hz.chenlongwang.top/gtwiabfrdn.html

Ruby: PI = 3.14159
来源：http://hz.tian-w.cn/gtsapnsmsn.html

C#:   const double PI = 3.14159;
来源：http://hz.vqdsnc.cn/gtjvmiekos.html

[A04] 判断变量类型
来源：http://hz.yueranfly.top/gtsdrpjyub.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.jqgfzy.top/gtsvbmojmd.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.gaohongyu789.top/gtxncuqzpd.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.52xcode.cn/gtxvanpejm.html

TS:   typeof x; x instanceof Date
来源：http://hz.pengpengdd.cyou/gtrgxozawv.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.tanke756.top/gtoitbgacp.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.hysaishi.cn/gtnnbbbtqw.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.gzhubu.top/gthutlouxt.html

C#:   x.GetType().Name; x is int
来源：http://hz.yongpay.top/gtocbokhmk.html

[A05] 整数除法与取模
来源：http://hz.gzhubu.top/gtiagefnlb.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.guannengcc.top/gttyrbvskt.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.zhongyouzk.top/gtiathjawn.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.chenzaomai.com/gtvbjjpsfz.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.quarkkingdee.top/gtnulywqca.html

Java: 7 / 2; 7 % 2
来源：http://hz.cheryme.top/gtokylqejk.html

Go:   7 / 2; 7 % 2
来源：http://hz.hammf.cn/gtmfbyllht.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.zhoulong.xyz/gttmzbkezh.html

C#:   7 / 2; 7 % 2
来源：http://hz.dianchejie.cn/gthldudnng.html

[A06] 字符串转数字
来源：http://hz.aibaodan.cn/gtngfyoifn.html

Py:   int("42"); float("3.14")
来源：http://hz.kuanghao11.cn/gtokaqnzyg.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.jinghuilouyu.cn/gtgxwjqdac.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.ppjwa.cn/gtisdmhaqz.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.feifeiyinyue.top/gtduvahmnm.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.yangfankeji.com/gtomdwvskj.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.jinghuilouyu.cn/gtqrmarccu.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.bjfxy.top/gtgxvdknvn.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.chenjidiqi.icu/gtnwrfwfsz.html

[A07] 数字转字符串
来源：http://hz.andypj.xyz/gtnukkouap.html

Py:   str(42)
来源：http://hz.ppjwa.cn/gtnqpfnpsg.html

PHP:  (string) 42; strval(42)
来源：http://hz.yangfankeji.com/gtliqnosaw.html


<!-- 参考信息 -->