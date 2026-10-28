代发 wailian999

[U53] PHP：空合并运算符
来源：http://hz.yangfankeji.com/gtcgvidmub.html

$v = $a ?? $b ?? "default";
来源：http://hz.sysykeji.top/gtjofjluzp.html

[U54] PHP：空安全调用
来源：http://hz.yanxiufei.cn/gtfprjmqmr.html

$obj?->method()
来源：http://hz.hongshengwenyu.top/gtwzbfekvs.html

[U55] PHP：match 表达式
来源：http://hz.yongpay.top/gtzybsfwit.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.fzhhl.top/gtfeqeeymd.html

[U56] PHP：命名参数
来源：http://hz.guowangkeji.top/gtwxnyewbg.html

f(a: 1, b: 2)
来源：http://hz.ybcxt.top/gtethlirvh.html

[U57] PHP：字符串插值
来源：http://hz.xylfe.cn/gtjeflyzup.html

"值: {$a}"
来源：http://hz.nanxinkj.top/gtebnzjvhc.html

[U58] PHP：数组三件套
来源：http://hz.zhengqikj.top/gtmwzlinvb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.mhx1999.top/gtrwadlegd.html

[U59] PHP：自定义排序
来源：http://hz.ehwqpu.com/gtwgitrsok.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yuxming.cn/gtewmttfhk.html

[U60] PHP：JSON 编解码
来源：http://hz.svipenyu.cn/gtsvqvegac.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.cucudq.cn/gtpvlmyhvm.html

[U61] PHP：正则
来源：http://hz.yanxiufei.cn/gtykwwccrs.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.hammf.cn/gtqxmjrmyz.html

[U62] PHP：日期对象
来源：http://hz.daxiang520.top/gtcaortrwt.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.c1oappe.top/gtkvyvtwwl.html

[U63] PHP：文件读写
来源：http://hz.sweek.top/gtyjucpqwt.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.ppjwa.cn/gtfyhmolmn.html

[U64] PHP：目录遍历
来源：http://hz.meibo888.top/gtjolzqoel.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.zhoulong.xyz/gtxbetwwck.html

[U65] PHP：会话
来源：http://hz.sysykeji.top/gtvodvrejv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.chenzaomai.com/gtxfzutjrp.html

[U66] PHP：设置 Cookie
来源：http://hz.ydzc1.top/gtndyefbeq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.vqdsnc.cn/gteltzfqxz.html

[U67] PHP：处理文件上传
来源：http://hz.zhoulong.xyz/gtphzgvouf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.52xcode.cn/gtuqxkkger.html

[U68] PHP：PDO 连接
来源：http://hz.sufxvd.cn/gtfdlwntbj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.jinghuilouyu.cn/gtewjkmbwn.html

[U69] PHP：PDO 预处理
来源：http://hz.jianghu66.top/gtafyyudjt.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.chenzaomai.com/gtykdsoywd.html

[U70] PHP：PDO 事务
来源：http://hz.gaohongyu789.top/gtqhuukgnw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.zycfv.cn/gtqicrrwxh.html

[U71] PHP：抛出异常
来源：http://hz.zdqjudy.top/gtssgmkwop.html

throw new RuntimeException("失败", 500);
来源：http://hz.zhoulong.xyz/gtdvmtzbuu.html

[U72] PHP：写错误日志
来源：http://hz.dianchejie.cn/gtqogjhbke.html

error_log("失败: " . $e->getMessage());
来源：http://hz.ybcxt.top/gtngilljvn.html

[U73] PHP：读取 ini 配置
来源：http://hz.zhengqikj.top/gtjyirpnxl.html

parse_ini_file("config.ini", true)
来源：http://hz.ivvv.top/gtpkguilfc.html

[U74] PHP：读取环境变量
来源：http://hz.yuanzhike.top/gteuszbxan.html

getenv("APP_ENV") ?: "production"
来源：http://hz.feifeiyinyue.top/gtqobeftse.html

[U75] PHP：依赖注入
来源：http://hz.cheryme.top/gtdtladxxq.html

composer require psr/container
来源：http://hz.yongpay.top/gtzxpvyavf.html

[U76] PHP：简单路由
来源：http://hz.zhiwuduotai.top/gtzorqatzr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.0kj1m.cn/gtxintwdjl.html

[U77] PHP：模板渲染
来源：http://hz.quarkkingdee.top/gteghidvwk.html

composer require twig/twig
来源：http://hz.zhixingplan.top/gtqkrdfath.html

[U78] PHP：单元测试
来源：http://hz.birdmap.top/gtnlbhwedn.html

composer require --dev phpunit/phpunit
来源：http://hz.sysykeji.top/gtghsurpat.html

[U79] PHP：静态分析
来源：http://hz.xuetiantiany.cn/gtudoywyjs.html

composer require --dev phpstan/phpstan
来源：http://hz.dianchejie.cn/gtqhysvqzp.html

[U80] PHP：代码规范修复
来源：http://hz.feifeiyinyue.top/gtbgfnxgmj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.ywan-chungtsiang.top/gtbpjzzjrf.html

[U81] JS：初始化项目
来源：http://hz.cqqwz.cn/gtcvjytvov.html

npm init -y;  npm i express
来源：http://hz.jqgfzy.top/gtgzjaasfb.html

[U82] JS：package.json 脚本
来源：http://hz.guannengcc.top/gtmdyltrko.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.sufxvd.cn/gthgcpdmki.html

[U83] JS：ES Module 导入导出
来源：http://hz.sxryk.cn/gtttgvexxd.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.ehwqpu.com/gttdzzcoai.html

[U84] JS：CommonJS 写法
来源：http://hz.yangfankeji.com/gtoypziepu.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.gogol.net.cn/gtbemlezws.html

[U85] JS：可选链
来源：http://hz.hysaishi.cn/gtxzbmhlhq.html

a?.b?.c
来源：http://hz.kuanghao11.cn/gtyjrboigs.html

[U86] JS：空值合并
来源：http://hz.havefunace.top/gtbqsjxkvh.html

a ?? b
来源：http://hz.jqgufenzy.top/gtlfnelycl.html

[U87] JS：解构默认值
来源：http://hz.zycfv.cn/gtnvfoxstc.html

const { a = 1, b = 2 } = obj;
来源：http://hz.ehwqpu.com/gtylipdwlw.html

[U88] JS：对象展开合并
来源：http://hz.yj202588.top/gtbjqegyzg.html

{ ...a, ...b }
来源：http://hz.316326.xyz/gtbnseifhc.html

[U89] JS：数组去重
来源：http://hz.316326.xyz/gtcqsaqfjy.html

[...new Set(arr)]
来源：http://hz.jqgufenzy.top/gtpepjlohu.html

[U90] JS：数字数组排序
来源：http://hz.cashguo.top/gtmiamlzug.html

[...arr].sort((a, b) => a - b)
来源：http://hz.birdmap.top/gtwxwmtwga.html

[U91] JS：对象键值遍历
来源：http://hz.mhx1999.top/gtupwqnais.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.jinqigufen.top/gtptmzbyhf.html

[U92] JS：深拷贝
来源：http://hz.iojbl.cn/gtcttdsqwb.html

structuredClone(obj)
来源：http://hz.0kj1m.cn/gtfhgeagam.html

[U93] JS：模板字符串
来源：http://hz.hongshengwenyu.top/gtifkrcvlm.html

`共 ${n} 条`
来源：http://hz.sysykeji.top/gtbflxwwil.html

[U94] JS：箭头函数
来源：http://hz.316326.xyz/gtnallzgzh.html

const double = x => x * 2;
来源：http://hz.yj20258888.top/gtaxdqowii.html

[U95] JS：Promise 包装
来源：http://hz.jinqigufen.top/gtapjxwywv.html

new Promise((resolve, reject) => {})
来源：http://hz.zhaomingkeji.xyz/gtldwblrot.html

[U96] JS：async/await 与异常
来源：http://hz.hywenlv.cn/gtghkgzjfx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.meibo888.top/gtncqnmrdx.html

[U97] JS：并发请求
来源：http://hz.yonumen.top/gttuzywqep.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yuanzhike.top/gtsaksfwfc.html

[U98] JS：fetch 带 JSON
来源：http://hz.quarkkingdee.top/gttvjxzoqg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.daria6918.cn/gtshvjscwq.html

[U99] JS：事件监听
来源：http://hz.aizwys.cn/gttopimtin.html

el.addEventListener("click", e => {})
来源：http://hz.c1oappe.top/gtkjujveok.html

[U100] JS：DOM 查询
来源：http://hz.ehwqpu.com/gtlwvolrsx.html

document.querySelector(".item")
来源：http://hz.fengsongda.top/gtmwejqpco.html

[U101] JS：classList 操作
来源：http://hz.ydzc1.top/gtxcuaksrx.html

el.classList.toggle("active")
来源：http://hz.sweek.top/gthjrsrmjq.html

[U102] JS：本地存储
来源：http://hz.shuidangran.top/gtwaobjfew.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.vqdsnc.cn/gtocvavkuw.html

[U103] JS：定时器
来源：http://hz.aizwys.cn/gtjbebqacb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.cucudq.cn/gtwragehxn.html

[U104] JS：防抖
来源：http://hz.feifeiyinyue.top/gtmaywihhv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hnqzz.top/gtfsnqcrqa.html

[U105] JS：节流
来源：http://hz.tian-w.cn/gtuayqictp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.xuanzx.com/gtembnlizl.html

[U106] JS：日期格式化
来源：http://hz.ivvv.top/gtarhnvcgy.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.wangshuangyany.cn/gtopmiefpu.html

[U107] JS：数字千分位
来源：http://hz.andypj.xyz/gtxlaclols.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.xylfe.cn/gtlinplurj.html

[U108] JS：随机整数
来源：http://hz.aibaodan.cn/gtsybjgzlr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.ydjk.org.cn/gteajfkysr.html

[U109] JS：数组分组
来源：http://hz.ydzc1.top/gtqbwmbdss.html

Object.groupBy(arr, x => x.type)
来源：http://hz.dianchejie.cn/gtkrlcrmlt.html

[U110] JS：数组分块
来源：http://hz.shangyingyoupin.top/gtocdwudjg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.c1oappe.top/gtgjtusmfl.html

[U111] JS：对象转 Map
来源：http://hz.daria6918.cn/gtadkfguzc.html

new Map(Object.entries(obj))
来源：http://hz.zhongyouzk.top/gttjomdxiq.html

[U112] JS：字符串补位
来源：http://hz.jinyuanbaomall.cn/gtogtsuhuj.html

"7".padStart(3, "0")
来源：http://hz.nanxinkj.top/gtfyifepzq.html

[U113] JS：正则替换全部
来源：http://hz.hnqzz.top/gthedjkbdw.html

s.replaceAll("a", "b")
来源：http://hz.c1oappe.top/gtpaezjhef.html

[U114] JS：JSON 深比较
来源：http://hz.sufxvd.cn/gtzlzufrzx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.snrcjt.cn/gtdzvvsrwf.html

[U115] JS：生成 UUID
来源：http://hz.aizwys.cn/gtoqejmfvv.html

crypto.randomUUID()
来源：http://hz.andypj.xyz/gtlweevvfq.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.gaohongyu789.top/gtntjqexjs.html

/** @param {string} name */ function f(name) {}
来源：http://hz.zdqjudy.top/gtspbeegyz.html

[U117] JS：单元测试
来源：http://hz.quarkkingdee.top/gtevlxffqw.html

npm i -D vitest;  npx vitest
来源：http://hz.ppjwa.cn/gtqcsvcsme.html

[U118] JS：开发服务器
来源：http://hz.gogol.net.cn/gtbygxclrs.html

npm i -D vite;  npx vite
来源：http://hz.wangshuangyany.cn/gtdcpcxwcu.html

[U119] JS：生产构建
来源：http://hz.mhx1999.top/gtymvkjwdd.html

npx vite build
来源：http://hz.cheryme.top/gtthbfibmo.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.jinqigfzy.top/gtsyksfiab.html

import.meta.env.VITE_API_URL
来源：http://hz.hnxiangtu.top/gtxgvdvowl.html

================================================================================
来源：http://hz.chenzaomai.com/gtdshfboej.html

统计汇总
来源：http://hz.yj20258888.top/gtrvujpomv.html

================================================================================
来源：http://hz.52xcode.cn/gtnvzgnthv.html

按语言统计（条）：
来源：http://hz.snrcjt.cn/gtxhspfwlp.html

Python ......... 252
来源：http://hz.jinqigfzy.top/gtktmpaohd.html

PHP ............ 252
来源：http://hz.hywenlv.cn/gtoeamvwjz.html

JavaScript ..... 252
来源：http://hz.ydjk.org.cn/gthcyfrwbm.html

TypeScript ..... 212
来源：http://hz.aizwys.cn/gtodtxxlwx.html

Java ........... 212
来源：http://hz.daria6918.cn/gtmpsunhbq.html

Go ............. 212
来源：http://hz.zhaomingkeji.xyz/gtjusaazyd.html

Ruby ........... 212
来源：http://hz.aibaodan.cn/gtcllipuls.html

C# ............. 212
来源：http://hz.gaohongyu789.top/gtpmdppntk.html

C .............. 30
来源：http://hz.sweek.top/gtryvfiitl.html

C++ ............ 30
来源：http://hz.tanke756.top/gtmkmgunkc.html

SQL ............ 90
来源：http://hz.hnqzz.top/gtqgutwcog.html

Bash ........... 80
来源：http://hz.chenlongwang.top/gtdszwlipa.html

Kotlin ......... 15
来源：http://hz.bjfxy.top/gtlbvuessl.html

Swift .......... 15
来源：http://hz.wangshuangyany.cn/gtekqbbbed.html

Lua ............ 10
来源：http://hz.gzhubu.top/gtvvcgnuuw.html

Perl ........... 10
来源：http://hz.jiagoushi.top/gtjllecdpy.html

Scala .......... 10
来源：http://hz.zhijiandao.cn/gtcixkpmgh.html

------------------------------------
来源：http://hz.hammf.cn/gtbuxkzyqu.html

合计 ........... 2106 条
来源：http://hz.fengsongda.top/gtkvpgsguh.html

按章节统计：
来源：http://hz.gotoacloud.top/gtjbiutebt.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.hnxiangtu.top/gtvcofjzps.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yj202588.top/gtlslutbih.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.316326.xyz/gtbwjncasp.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.svipenyu.cn/gthghbooxf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.yongpay.top/gtshbvheqg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.tianlin.xyz/gtpucfafjo.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.xinyue.icu/gtjwvugejm.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.havefunace.top/gtyddhmrsn.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.cucudq.cn/gtnmevxrqx.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.cucudq.cn/gtvkfhlmui.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.feifeiyinyue.top/gtcaxuxwvj.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.ydzc1.top/gtxgpxgaiy.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.nwbrower.top/gtwbuvadne.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.c1oappe.top/gtsxorcemi.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.xuanzx.com/gtkblarlrj.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.cdnleiting.top/gtrguocoqm.html

Q SQL 专题                              90
来源：http://hz.shanyushiyangtech.top/gtvifhcnbo.html

R Bash 专题                             80
来源：http://hz.aibaodan.cn/gthhtrrjic.html

S C / C++ 专题                          60
来源：http://hz.pycfn.com/gtmwazfrcw.html

T 其他语言补充                          60
来源：http://hz.gogol.net.cn/gttuzxwzbc.html

U 高频实用片段                         120
来源：http://hz.shuidangran.top/gtmnuqmscg.html

------------------------------------
来源：http://hz.zhijiandao.cn/gtsqeadkeo.html

合计                                  2106 条
来源：http://hz.zhoulong.xyz/gtjhsvidsx.html

--------------------------------------------------------------------------------
来源：http://hz.ybcxt.top/gtzqajnhoh.html

使用提醒
来源：http://hz.sufxvd.cn/gtglyimrja.html

--------------------------------------------------------------------------------
来源：http://hz.yj20258.top/gtsqxhbwrv.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.hongshengwenyu.top/gtvlvlmyow.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.andypj.xyz/gtnoeaqzfl.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.9152youxi.cn/gtbtweikzx.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.chenjidiqi.icu/gtbjfzyilb.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.hammf.cn/gtocbamkam.html

—— 文件结束 ——
来源：http://hz.jinyuanbaomall.cn/gtsgqqnzaq.html

================================================================================
来源：http://hz.c1oappe.top/gtmitdkncm.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.zhongyouzk.top/gtxzhulhos.html

Common Programming Examples Cheat Book
来源：http://hz.cucudq.cn/gtwjghzwrp.html

================================================================================
来源：http://hz.ybcxt.top/gtztiguogv.html

【收录内容】
来源：http://hz.c1oappe.top/gtlfcoeyco.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.pengpengdd.cyou/gtbrygievv.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.shanyushiyangtech.top/gtchovkgzu.html

SQL · Bash · C · C++
来源：http://hz.guannengcc.top/gthafcrdla.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.jinqigufen.top/gtqzkggpmt.html

【使用说明】
来源：http://hz.yj20258888.top/gtfustcozo.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.cucudq.cn/gtoxpeplxg.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.jinqigufen.top/gtfaxpjxbp.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.ehwqpu.com/gteuuwwbam.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.shanyushiyangkeji.top/gtkczvfdcv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.aizwys.cn/gtlksmpret.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.cdnleiting.top/gtnrydkuja.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.kuanghao11.cn/gtuhxgtjif.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.snrcjt.cn/gtjbivubzj.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.zdqjudy.top/gtyxnfzudp.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.sxryk.cn/gtrcxmocsw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.redwolf501.top/gtaizuivww.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.hywenlv.cn/gtqdmqerxv.html

【文件统计】
来源：http://hz.tianlin.xyz/gtwzpaszii.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.yongpay.top/gteubicmws.html

--------------------------------------------------------------------------------
来源：http://hz.nanxinkj.top/gtaumvtvjg.html

目  录
来源：http://hz.shanyushiyangkeji.top/gtvfubecxu.html

--------------------------------------------------------------------------------
来源：http://hz.cqqwz.cn/gttvmanyjm.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.nwbrower.top/gtsznoytim.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.shanyushiyangkeji.top/gtqynxfrqg.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.dashuyun.cn/gtdfqgaokf.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.yueranfly.top/gtsivrrwxu.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.hywenlv.cn/gtwuntykkj.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.meibo888.top/gtbkagzkot.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.aizwys.cn/gttwqimvgh.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.sysykeji.top/gtaexphbki.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.0kj1m.cn/gtfxymowqw.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.bjfxy.top/gtcxkpwngt.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.jiagoushi.top/gtawnsfswh.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.mhx1999.top/gtiynmddxw.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.yj20258888.top/gttiombppk.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.jinqigfzy.top/gtvuvashzo.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.shanyushiyangkeji.top/gtppssljss.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.9152youxi.cn/gtnhucbrnq.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.dianchejie.cn/gteipbcwgj.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.guowangkeji.top/gtqblrrbmb.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.9152youxi.cn/gtuvhwzyot.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cucudq.cn/gtddzablqf.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.ivvv.top/gtesrbafrm.html

================================================================================
来源：http://hz.hnqzz.top/gtrfdeutam.html

A. 基础语法与类型
来源：http://hz.yangfankeji.com/gtdsnnitua.html

================================================================================
来源：http://hz.redwolf501.top/gtuebxdjzi.html

[A01] Hello World
来源：http://hz.ydzc1.top/gtizcwywdb.html

Py:   print("Hello, World!")
来源：http://hz.andypj.xyz/gtoqpbmxfo.html

PHP:  echo "Hello, World!";
来源：http://hz.jyoumei.cn/gtvicdmeqx.html

JS:   console.log("Hello, World!");
来源：http://hz.yongpay.top/gtcvqanxbs.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.meibo888.top/gtvcaldway.html

Java: System.out.println("Hello, World!");
来源：http://hz.yueranfly.top/gtokfultpe.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.jinqigfzy.top/gtefblnyym.html

Ruby: puts "Hello, World!"
来源：http://hz.jinyuanbaomall.cn/gtftdlvchg.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.shuidangran.top/gtybfluzrr.html

[A02] 变量声明与赋值
来源：http://hz.zhijiandao.cn/gtozqkptff.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.kuanghao11.cn/gtjxpcufdr.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.tian-w.cn/gtepgftvjv.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.ybcxt.top/gtolomptqr.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.hnqzz.top/gtedokbdpr.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.shanyushiyangtech.top/gtwmatjdbd.html

Go:   name := "Alex"; age := 20
来源：http://hz.cashguo.top/gtkxbceftj.html

Ruby: name = "Alex"; age = 20
来源：http://hz.jinghuilouyu.cn/gthvzysyvh.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.nanxuanxn.top/gtcuxaszip.html

[A03] 常量定义
来源：http://hz.havefunace.top/gtqjhytger.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.haohaochexian.top/gtzplcupin.html

PHP:  const PI = 3.14159;
来源：http://hz.yangfankeji.com/gtjtympvdx.html

JS:   const PI = 3.14159;
来源：http://hz.xuetiantiany.cn/gtzfxwibxa.html

TS:   const PI: number = 3.14159;
来源：http://hz.xuanzx.com/gtwqksnkou.html

Java: static final double PI = 3.14159;
来源：http://hz.chenzaomai.com/gtulemaixz.html

Go:   const PI = 3.14159
来源：http://hz.c1oappe.top/gtxfbjxbmh.html

Ruby: PI = 3.14159
来源：http://hz.iojbl.cn/gtaewbmntv.html

C#:   const double PI = 3.14159;
来源：http://hz.jinqigufen.top/gtvajpwgmd.html

[A04] 判断变量类型
来源：http://hz.yj20258.top/gtlgusgyru.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.svipenyu.cn/gtawyutcnq.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.zhengqikj.top/gtraqvlaku.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.cashguo.top/gtrqjsljmd.html

TS:   typeof x; x instanceof Date
来源：http://hz.yvedp.cn/gtutolbnzy.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.snrcjt.cn/gtjrwrzblj.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.shzxlz.cn/gtygxednts.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.jinghuilouyu.cn/gtllkzazuz.html

C#:   x.GetType().Name; x is int
来源：http://hz.andypj.xyz/gtgvxdlbti.html

[A05] 整数除法与取模
来源：http://hz.sufxvd.cn/gtcdutgjlg.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.chenjidiqi.icu/gtnyfhwwvl.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.sweek.top/gtdmhzmxsh.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.hnqzz.top/gtzpibimog.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.yuxming.cn/gtcznumurh.html

Java: 7 / 2; 7 % 2
来源：http://hz.jlsjyb.cn/gtfqlymyvm.html

Go:   7 / 2; 7 % 2
来源：http://hz.shangyingyoupin.top/gtmelxxnhp.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.daxiang520.top/gtfajcbngt.html

C#:   7 / 2; 7 % 2
来源：http://hz.smart0.xyz/gtklbdjvxe.html

[A06] 字符串转数字
来源：http://hz.redwolf501.top/gtzlflcnym.html

Py:   int("42"); float("3.14")
来源：http://hz.mhx1999.top/gtnchssswn.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.bjfxy.top/gtqhohgviz.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.cheryme.top/gtfutbneth.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.yvedp.cn/gtmyldcwuy.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.gaohongyu789.top/gtsjibhcan.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.ybcxt.top/gtusjdcakl.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.svipenyu.cn/gtcditualg.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.jinqigfzy.top/gtsgyjpnry.html

[A07] 数字转字符串
来源：http://hz.yanxiufei.cn/gtmwskjbfc.html

Py:   str(42)
来源：http://hz.havefunace.top/gthkpsbbui.html

PHP:  (string) 42; strval(42)
来源：http://hz.jqgufenzy.top/gttqoanbju.html


<!-- 参考信息 -->