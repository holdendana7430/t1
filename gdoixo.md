代发 wailian999

[U51] PHP：数组解构
来源：http://hz.zhoulong.xyz/gtnjbfjvqi.html

[$a, $b] = $arr;
来源：http://hz.chenlongwang.top/gtcsvlsmmy.html

[U52] PHP：箭头函数
来源：http://hz.jinqigufen.top/gtarfolieb.html

$double = fn($x) => $x * 2;
来源：http://hz.fzhhl.top/gtcaycfofa.html

[U53] PHP：空合并运算符
来源：http://hz.nanxinkj.top/gtcugyumaa.html

$v = $a ?? $b ?? "default";
来源：http://hz.xylfe.cn/gtdbjmozen.html

[U54] PHP：空安全调用
来源：http://hz.ydjk.org.cn/gtbuojugmk.html

$obj?->method()
来源：http://hz.daria6918.cn/gtufcyihoi.html

[U55] PHP：match 表达式
来源：http://hz.chenjidiqi.icu/gtdcbtdnhg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.jinqigufen.top/gtijnaplsn.html

[U56] PHP：命名参数
来源：http://hz.havefunace.top/gtidlwkvye.html

f(a: 1, b: 2)
来源：http://hz.jinqigufen.top/gtzyhmwrwd.html

[U57] PHP：字符串插值
来源：http://hz.ydzc1.top/gtstezaoih.html

"值: {$a}"
来源：http://hz.zhiwuduotai.top/gtypkmrzic.html

[U58] PHP：数组三件套
来源：http://hz.gotoacloud.top/gtsraqcyhe.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.yueranfly.top/gtwlnosqje.html

[U59] PHP：自定义排序
来源：http://hz.jinyuanbaomall.cn/gtwfltihbx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hammf.cn/gtufffpqxn.html

[U60] PHP：JSON 编解码
来源：http://hz.tanke756.top/gtezjydcvc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.jianghu66.top/gttenbstjp.html

[U61] PHP：正则
来源：http://hz.cheryme.top/gtrkphxdwx.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.shanyushiyangkeji.top/gtkwgtiwvi.html

[U62] PHP：日期对象
来源：http://hz.hywenlv.cn/gtkaimkiqu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.9152youxi.cn/gtdhzbwhcn.html

[U63] PHP：文件读写
来源：http://hz.yanxiufei.cn/gtulkvzoco.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.wangshuangyany.cn/gtmfomswcd.html

[U64] PHP：目录遍历
来源：http://hz.xylfe.cn/gtvdwvjmwx.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.snrcjt.cn/gtrrtavknn.html

[U65] PHP：会话
来源：http://hz.316326.xyz/gtobchhxuu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.hywenlv.cn/gtwdgabwyp.html

[U66] PHP：设置 Cookie
来源：http://hz.zycfv.cn/gtxlmxwoxs.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.ehwqpu.com/gtucodauwf.html

[U67] PHP：处理文件上传
来源：http://hz.sweek.top/gthajsqkoc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.hysaishi.cn/gtayclvryf.html

[U68] PHP：PDO 连接
来源：http://hz.yuxming.cn/gtwlanxpul.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.ywan-chungtsiang.top/gtrkzcgpvp.html

[U69] PHP：PDO 预处理
来源：http://hz.zhoulong.xyz/gtkjepolln.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.jinqigfzy.top/gtatuhrmda.html

[U70] PHP：PDO 事务
来源：http://hz.yuanzhike.top/gtbsujfdhs.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.birdmap.top/gtgcqmccmx.html

[U71] PHP：抛出异常
来源：http://hz.smart0.xyz/gtoyqimtdl.html

throw new RuntimeException("失败", 500);
来源：http://hz.zhoulong.xyz/gtjfjthnbp.html

[U72] PHP：写错误日志
来源：http://hz.zhoulong.xyz/gtofjjfsly.html

error_log("失败: " . $e->getMessage());
来源：http://hz.daria6918.cn/gtqtvjvdpx.html

[U73] PHP：读取 ini 配置
来源：http://hz.c1oappe.top/gtyetsinro.html

parse_ini_file("config.ini", true)
来源：http://hz.ppjwa.cn/gtzioryteg.html

[U74] PHP：读取环境变量
来源：http://hz.xuanzx.com/gtdlwgjqyn.html

getenv("APP_ENV") ?: "production"
来源：http://hz.hammf.cn/gtbtsfjyfe.html

[U75] PHP：依赖注入
来源：http://hz.snrcjt.cn/gtiiksscai.html

composer require psr/container
来源：http://hz.jiagoushi.top/gtxfnikbyh.html

[U76] PHP：简单路由
来源：http://hz.kuanghao11.cn/gtjitryjmc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.dianchejie.cn/gtokbfyull.html

[U77] PHP：模板渲染
来源：http://hz.nanxinkj.top/gtddzwmrgl.html

composer require twig/twig
来源：http://hz.zhongyouzk.top/gthubmkfyh.html

[U78] PHP：单元测试
来源：http://hz.wangshuangyany.cn/gtpwlhsvzu.html

composer require --dev phpunit/phpunit
来源：http://hz.9152youxi.cn/gtrirlkpha.html

[U79] PHP：静态分析
来源：http://hz.xuanzx.com/gtyzdwtevg.html

composer require --dev phpstan/phpstan
来源：http://hz.daria6918.cn/gtsymlvcjs.html

[U80] PHP：代码规范修复
来源：http://hz.fzhhl.top/gtnvkluere.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.sweek.top/gtpmargaob.html

[U81] JS：初始化项目
来源：http://hz.ivvv.top/gtkbnsfkst.html

npm init -y;  npm i express
来源：http://hz.zhixingplan.top/gtmqndbtfj.html

[U82] JS：package.json 脚本
来源：http://hz.tanke756.top/gtmkmrqrvu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.chenzaomai.com/gtdjqikxhi.html

[U83] JS：ES Module 导入导出
来源：http://hz.zhaomingkeji.xyz/gtsojclpmn.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.meibo888.top/gtxfgdgyka.html

[U84] JS：CommonJS 写法
来源：http://hz.shanyushiyangkeji.top/gtyjtvqzgw.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.zdqjudy.top/gtjtlgplgs.html

[U85] JS：可选链
来源：http://hz.guannengcc.top/gtgebhhtma.html

a?.b?.c
来源：http://hz.chenzaomai.com/gtjwsprxyh.html

[U86] JS：空值合并
来源：http://hz.yangfankeji.com/gtrpejfcwn.html

a ?? b
来源：http://hz.jyoumei.cn/gtbypxtymm.html

[U87] JS：解构默认值
来源：http://hz.cdnleiting.top/gthmbsmkyu.html

const { a = 1, b = 2 } = obj;
来源：http://hz.hywenlv.cn/gtjztoukmf.html

[U88] JS：对象展开合并
来源：http://hz.hnxiangtu.top/gtnxsyvklx.html

{ ...a, ...b }
来源：http://hz.zhengqikj.top/gtrikjdrga.html

[U89] JS：数组去重
来源：http://hz.bjfxy.top/gtxntjrlrl.html

[...new Set(arr)]
来源：http://hz.ybcxt.top/gtixxbcbyx.html

[U90] JS：数字数组排序
来源：http://hz.gotoacloud.top/gtcqigsbir.html

[...arr].sort((a, b) => a - b)
来源：http://hz.quarkkingdee.top/gtlqbqinxb.html

[U91] JS：对象键值遍历
来源：http://hz.daxiang520.top/gtafhsmyon.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.fengsongda.top/gttrgjmiph.html

[U92] JS：深拷贝
来源：http://hz.nanxuanxn.top/gtcjyucxvm.html

structuredClone(obj)
来源：http://hz.birdmap.top/gteohdskap.html

[U93] JS：模板字符串
来源：http://hz.tian-w.cn/gthimdrbko.html

`共 ${n} 条`
来源：http://hz.fengsongda.top/gtwfxteact.html

[U94] JS：箭头函数
来源：http://hz.zhiwuduotai.top/gtexataxkw.html

const double = x => x * 2;
来源：http://hz.hywenlv.cn/gtfdvfjrkf.html

[U95] JS：Promise 包装
来源：http://hz.jianghu66.top/gtjoxupuqb.html

new Promise((resolve, reject) => {})
来源：http://hz.zhijiandao.cn/gtsqdnnfwp.html

[U96] JS：async/await 与异常
来源：http://hz.guannengcc.top/gtieiejxte.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.zhaomingkeji.xyz/gtjiwwfiqs.html

[U97] JS：并发请求
来源：http://hz.ppjwa.cn/gtitnmylyw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hongshengwenyu.top/gtptwzguyz.html

[U98] JS：fetch 带 JSON
来源：http://hz.jqgfzy.top/gtmimblhup.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.shangyingyoupin.top/gtpakcsosv.html

[U99] JS：事件监听
来源：http://hz.guowangkeji.top/gttpqxjjuh.html

el.addEventListener("click", e => {})
来源：http://hz.xinyue.icu/gtpuoizaeq.html

[U100] JS：DOM 查询
来源：http://hz.yongpay.top/gtkejymlos.html

document.querySelector(".item")
来源：http://hz.jinghuilouyu.cn/gtxiqfndvd.html

[U101] JS：classList 操作
来源：http://hz.jinqigfzy.top/gtzwvvpyzr.html

el.classList.toggle("active")
来源：http://hz.jinqigfzy.top/gtvcftyjmz.html

[U102] JS：本地存储
来源：http://hz.yongpay.top/gtczjxilju.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.dashuyun.cn/gtlwodnnnj.html

[U103] JS：定时器
来源：http://hz.xingfuxueyuan.xyz/gtenznobkq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.xuanzx.com/gtardkevsf.html

[U104] JS：防抖
来源：http://hz.shanyushiyangkeji.top/gtcpzdgvtr.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhongyouzk.top/gtgyzmhcja.html

[U105] JS：节流
来源：http://hz.shuidangran.top/gtdicuyqey.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.quarkkingdee.top/gtgxgyhajl.html

[U106] JS：日期格式化
来源：http://hz.zhongyouzk.top/gtoxvwfpju.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.nwbrower.top/gtashhqrnh.html

[U107] JS：数字千分位
来源：http://hz.ppjwa.cn/gtvajquaws.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.ivvv.top/gtmovjgima.html

[U108] JS：随机整数
来源：http://hz.zhongyouzk.top/gtcoqaahat.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.tanke756.top/gttkwjhjuo.html

[U109] JS：数组分组
来源：http://hz.cashguo.top/gtmwoyqlkk.html

Object.groupBy(arr, x => x.type)
来源：http://hz.cashguo.top/gtmxtybtpm.html

[U110] JS：数组分块
来源：http://hz.9152youxi.cn/gtweexlsaf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.hammf.cn/gtxtufwetf.html

[U111] JS：对象转 Map
来源：http://hz.zhongyouzk.top/gtmacyyrtd.html

new Map(Object.entries(obj))
来源：http://hz.yongpay.top/gtiioefnuv.html

[U112] JS：字符串补位
来源：http://hz.zhijiandao.cn/gtgeqyktvr.html

"7".padStart(3, "0")
来源：http://hz.redwolf501.top/gtjjlvvxot.html

[U113] JS：正则替换全部
来源：http://hz.shzxlz.cn/gthbmxlydl.html

s.replaceAll("a", "b")
来源：http://hz.xziqi.cn/gtxojktrgd.html

[U114] JS：JSON 深比较
来源：http://hz.hywenlv.cn/gtprkmdyhx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.aibaodan.cn/gthspmwkoz.html

[U115] JS：生成 UUID
来源：http://hz.hongshengwenyu.top/gttpgrvxcg.html

crypto.randomUUID()
来源：http://hz.daria6918.cn/gtvezihrlk.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.yvedp.cn/gtqykrnedt.html

/** @param {string} name */ function f(name) {}
来源：http://hz.yvedp.cn/gtswupvmaf.html

[U117] JS：单元测试
来源：http://hz.shangyingyoupin.top/gtcnwlcaif.html

npm i -D vitest;  npx vitest
来源：http://hz.zhiwuduotai.top/gtcoydbvqz.html

[U118] JS：开发服务器
来源：http://hz.yvedp.cn/gtdtehixti.html

npm i -D vite;  npx vite
来源：http://hz.yj20258888.top/gtjjuthgvp.html

[U119] JS：生产构建
来源：http://hz.nwbrower.top/gtuzyczwvr.html

npx vite build
来源：http://hz.dashuyun.cn/gtupuiyszg.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.cdnleiting.top/gtejbukhpu.html

import.meta.env.VITE_API_URL
来源：http://hz.yonumen.top/gtkwveltgf.html

================================================================================
来源：http://hz.ehwqpu.com/gtcuazargp.html

统计汇总
来源：http://hz.yvedp.cn/gtfymzwniu.html

================================================================================
来源：http://hz.kuanghao11.cn/gtkzixozoh.html

按语言统计（条）：
来源：http://hz.jinqigufen.top/gtmbpcusgy.html

Python ......... 252
来源：http://hz.yanxiufei.cn/gtljgjlumn.html

PHP ............ 252
来源：http://hz.mhx1999.top/gtpxncabgx.html

JavaScript ..... 252
来源：http://hz.aibaodan.cn/gtxidsynmn.html

TypeScript ..... 212
来源：http://hz.hongshengwenyu.top/gtytvrgxod.html

Java ........... 212
来源：http://hz.ppjwa.cn/gthlqcxrbp.html

Go ............. 212
来源：http://hz.daria6918.cn/gtfeydtvkp.html

Ruby ........... 212
来源：http://hz.ydzc1.top/gtvuppkaqn.html

C# ............. 212
来源：http://hz.birdmap.top/gtgdltqyfw.html

C .............. 30
来源：http://hz.cqqwz.cn/gthvmyapev.html

C++ ............ 30
来源：http://hz.yangfankeji.com/gtoiwbdvmh.html

SQL ............ 90
来源：http://hz.zhiwuduotai.top/gtpqzlkfsb.html

Bash ........... 80
来源：http://hz.yongpay.top/gtngvsadcc.html

Kotlin ......... 15
来源：http://hz.gotoacloud.top/gtgstimgix.html

Swift .......... 15
来源：http://hz.jinyuanbaomall.cn/gtwrkdabyr.html

Lua ............ 10
来源：http://hz.yonumen.top/gtkhyfrmgw.html

Perl ........... 10
来源：http://hz.pycfn.com/gtpuhqarym.html

Scala .......... 10
来源：http://hz.meibo888.top/gtjufigkxm.html

------------------------------------
来源：http://hz.pengpengdd.cyou/gtdkbjbisa.html

合计 ........... 2106 条
来源：http://hz.c1oappe.top/gtjmamdwps.html

按章节统计：
来源：http://hz.yj202588.top/gteylsxvpj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.yj202588.top/gtbntrhwsq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.hongshengwenyu.top/gtndrblttx.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.zhiwuduotai.top/gtnmrpbzlf.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.jqgufenzy.top/gtzifnbevx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.hywenlv.cn/gtlfaoiawx.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.jinqigfzy.top/gtevruedex.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.quarkkingdee.top/gtrljhxavu.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.gzhubu.top/gtbhsgfwka.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.haohaochexian.top/gtdzzpzhfy.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.snrcjt.cn/gttbutfyvf.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.dashuyun.cn/gtehumvivc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.ppjwa.cn/gtwcmocvcu.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.hysaishi.cn/gtrjflmnet.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.xylfe.cn/gtulauncac.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.jqgufenzy.top/gtbkrpsypm.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.andypj.xyz/gttbcdkgvq.html

Q SQL 专题                              90
来源：http://hz.yj20258.top/gtacnyduhq.html

R Bash 专题                             80
来源：http://hz.nwbrower.top/gthjrjrgop.html

S C / C++ 专题                          60
来源：http://hz.tanke756.top/gtcfbvmnfc.html

T 其他语言补充                          60
来源：http://hz.hammf.cn/gtqihsstkr.html

U 高频实用片段                         120
来源：http://hz.shzxlz.cn/gttgaiegrr.html

------------------------------------
来源：http://hz.zhaomingkeji.xyz/gtklhclnbv.html

合计                                  2106 条
来源：http://hz.shuidangran.top/gtutjgqkff.html

--------------------------------------------------------------------------------
来源：http://hz.gzhubu.top/gtpzcpalpj.html

使用提醒
来源：http://hz.sysykeji.top/gtalwjfnxl.html

--------------------------------------------------------------------------------
来源：http://hz.fzhhl.top/gtzppnoham.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.fengsongda.top/gtseljiziy.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.zhoulong.xyz/gtrlehkwdi.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.dianchejie.cn/gtiiuzozta.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.yuanzhike.top/gtxrnlwqem.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.guannengcc.top/gtvbhmvznr.html

—— 文件结束 ——
来源：http://hz.ivvv.top/gthxyijfzl.html

================================================================================
来源：http://hz.chenlongwang.top/gtzphrknel.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.jinyuanbaomall.cn/gtndxejaxu.html

Common Programming Examples Cheat Book
来源：http://hz.yj20258.top/gtfuzlfxci.html

================================================================================
来源：http://hz.jinqigfzy.top/gtkzobmrts.html

【收录内容】
来源：http://hz.pengpengdd.cyou/gthcerolch.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.ppjwa.cn/gtdzendsvu.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.ywan-chungtsiang.top/gtmqzguela.html

SQL · Bash · C · C++
来源：http://hz.zhiwuduotai.top/gtjttdwoau.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.ehwqpu.com/gtucbmhsqr.html

【使用说明】
来源：http://hz.mhx1999.top/gtwwfiwcuk.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.birdmap.top/gtvdaqegpi.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.yueranfly.top/gtutseqjjs.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.hongshengwenyu.top/gtpsstazmb.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.zhaomingkeji.xyz/gtjczzdcep.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.yj202588.top/gtbobrrgzw.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.hywenlv.cn/gtyjaodhet.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.shangyingyoupin.top/gtzrqocexy.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.ybcxt.top/gtvbxovpch.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.zhengqikj.top/gtxbqlwdqw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.xingfuxueyuan.xyz/gthljtslmw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.yanxiufei.cn/gtemhpftsn.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.jinyuanbaomall.cn/gthdkhulyc.html

【文件统计】
来源：http://hz.redwolf501.top/gtoamujmrw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.0kj1m.cn/gtioigztye.html

--------------------------------------------------------------------------------
来源：http://hz.havefunace.top/gtqcudrsvd.html

目  录
来源：http://hz.nanxuanxn.top/gtleqycccl.html

--------------------------------------------------------------------------------
来源：http://hz.yongpay.top/gtmlrsukdj.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.yvedp.cn/gtiwbatnwg.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.jlsjyb.cn/gtezqvgsie.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.shuidangran.top/gtvsstzfef.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.xuanzx.com/gtulbojoqn.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.gaohongyu789.top/gtegnkwmgk.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.ydjk.org.cn/gtxnzgupkr.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.cashguo.top/gtdaszeuzm.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.shanyushiyangkeji.top/gtabdytgkn.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.sxryk.cn/gtlyjlnmmc.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.9152youxi.cn/gtvdhqeaig.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.jianghu66.top/gtfghqgmfq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.daxiang520.top/gtyrowcbmd.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.hnxiangtu.top/gtnmpdfivf.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.yj202588.top/gtzhxeowhs.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.andypj.xyz/gtvvjngjkh.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.xziqi.cn/gtpueksgbq.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.birdmap.top/gtiomnvuby.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.hnqzz.top/gttiesnbac.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.jlsjyb.cn/gturbscups.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.aizwys.cn/gthniccufs.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.snrcjt.cn/gtlukqorya.html

================================================================================
来源：http://hz.cashguo.top/gtysvqdevr.html

A. 基础语法与类型
来源：http://hz.tianlin.xyz/gtfpbqjgwv.html

================================================================================
来源：http://hz.pycfn.com/gtmtyhoyme.html

[A01] Hello World
来源：http://hz.gzhubu.top/gtzcyctqdk.html

Py:   print("Hello, World!")
来源：http://hz.ppjwa.cn/gtdfoceeua.html

PHP:  echo "Hello, World!";
来源：http://hz.cqqwz.cn/gtuhodavpn.html

JS:   console.log("Hello, World!");
来源：http://hz.sweek.top/gtaquxafmj.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.jinqigufen.top/gtfhevnbgr.html

Java: System.out.println("Hello, World!");
来源：http://hz.shanyushiyangkeji.top/gtakeembsf.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.gaohongyu789.top/gtjgxyzsxa.html

Ruby: puts "Hello, World!"
来源：http://hz.wangdashe.top/gtyderheki.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.yuxming.cn/gtgfdavpyb.html

[A02] 变量声明与赋值
来源：http://hz.nwbrower.top/gtlrnpxuvp.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.haohaochexian.top/gtdwuikrno.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.hfpthk.cn/gtywxgxdvz.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.chenlongwang.top/gtffdticll.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.yonumen.top/gtdekchjgv.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.ywan-chungtsiang.top/gtgjlxjyeh.html

Go:   name := "Alex"; age := 20
来源：http://hz.sweek.top/gtkvikduef.html

Ruby: name = "Alex"; age = 20
来源：http://hz.sysykeji.top/gtpyeezdwh.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.cashguo.top/gtpalzinzv.html

[A03] 常量定义
来源：http://hz.shuidangran.top/gtsziayyec.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.chenlongwang.top/gtqkaljjdi.html

PHP:  const PI = 3.14159;
来源：http://hz.xziqi.cn/gtvafhqslw.html

JS:   const PI = 3.14159;
来源：http://hz.shanyushiyangtech.top/gtketpcnrj.html

TS:   const PI: number = 3.14159;
来源：http://hz.haohaochexian.top/gtgyqnmowb.html

Java: static final double PI = 3.14159;
来源：http://hz.yanxiufei.cn/gtudnsjgoi.html

Go:   const PI = 3.14159
来源：http://hz.yonumen.top/gteskempxy.html

Ruby: PI = 3.14159
来源：http://hz.gotoacloud.top/gthgbobgbe.html

C#:   const double PI = 3.14159;
来源：http://hz.daria6918.cn/gtcqinlnhe.html

[A04] 判断变量类型
来源：http://hz.pycfn.com/gtvqamuqge.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.iojbl.cn/gtpqdcsaur.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.daria6918.cn/gtmcnoivwu.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.gotoacloud.top/gtfkigkxgp.html

TS:   typeof x; x instanceof Date
来源：http://hz.vqdsnc.cn/gtojzjjsmm.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.gaohongyu789.top/gtqatqesub.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.iojbl.cn/gtshrcutlj.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.jinqigfzy.top/gtzazesang.html

C#:   x.GetType().Name; x is int
来源：http://hz.smart0.xyz/gtczocszbx.html

[A05] 整数除法与取模
来源：http://hz.shzxlz.cn/gtfbmicrzs.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.nwbrower.top/gtjqflhvss.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.guannengcc.top/gtxdzgpnwu.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.fengsongda.top/gtwgepzudh.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.guowangkeji.top/gtvhbwkzvm.html

Java: 7 / 2; 7 % 2
来源：http://hz.daxiang520.top/gtmnkbdsee.html

Go:   7 / 2; 7 % 2
来源：http://hz.pycfn.com/gtknobtcya.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.gogol.net.cn/gttsrrzmfg.html

C#:   7 / 2; 7 % 2
来源：http://hz.birdmap.top/gtmhdbvqdi.html

[A06] 字符串转数字
来源：http://hz.shanyushiyangkeji.top/gtpcquyhki.html

Py:   int("42"); float("3.14")
来源：http://hz.meibo888.top/gtrcauvcbo.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.shzxlz.cn/gtnlpkcuxr.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.wangdashe.top/gtxugwgorl.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.xuanzx.com/gttnwvwstr.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.jyoumei.cn/gtiuyitiwn.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.yj20258.top/gtqfjqxwwu.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.iojbl.cn/gtptkdqjub.html


<!-- 参考信息 -->