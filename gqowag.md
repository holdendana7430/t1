代发 wailian999

[U57] PHP：字符串插值
来源：http://hz.gzhubu.top/gtzwspcmgb.html

"值: {$a}"
来源：http://hz.yanxiufei.cn/gturbzcayp.html

[U58] PHP：数组三件套
来源：http://hz.fengsongda.top/gtsraubfkj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.xinyue.icu/gtxqgnrkbj.html

[U59] PHP：自定义排序
来源：http://hz.jinqigufen.top/gtkdryuymc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.redwolf501.top/gtslhqjdrh.html

[U60] PHP：JSON 编解码
来源：http://hz.yj20258888.top/gtzrlwsxjo.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.smart0.xyz/gtqsyezleq.html

[U61] PHP：正则
来源：http://hz.hongshengwenyu.top/gtokdfucqq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.vqdsnc.cn/gtavscezeb.html

[U62] PHP：日期对象
来源：http://hz.smart0.xyz/gthnoqoqgn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.xuanzx.com/gtevwxaqmw.html

[U63] PHP：文件读写
来源：http://hz.sufxvd.cn/gtkrtloqcv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.nanxinkj.top/gtsxcgmogf.html

[U64] PHP：目录遍历
来源：http://hz.pengpengdd.cyou/gtwoynfphd.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.daria6918.cn/gtycrjqgtc.html

[U65] PHP：会话
来源：http://hz.nanxuanxn.top/gtxlnjtzab.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.cqqwz.cn/gtbmrudbvg.html

[U66] PHP：设置 Cookie
来源：http://hz.zhoulong.xyz/gtffqatjqy.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.hywenlv.cn/gtwzfsdmbk.html

[U67] PHP：处理文件上传
来源：http://hz.zhongyouzk.top/gtieirwdbb.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.zhoulong.xyz/gtuabegdup.html

[U68] PHP：PDO 连接
来源：http://hz.hysaishi.cn/gthattpjse.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.xziqi.cn/gtrmnbbaqi.html

[U69] PHP：PDO 预处理
来源：http://hz.aibaodan.cn/gthgpvvoyv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.jinyuanbaomall.cn/gtqqvicnmp.html

[U70] PHP：PDO 事务
来源：http://hz.zhengqikj.top/gtmixdrwtk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.shangyingyoupin.top/gtefdbnlto.html

[U71] PHP：抛出异常
来源：http://hz.zhoulong.xyz/gtgvgjmrjq.html

throw new RuntimeException("失败", 500);
来源：http://hz.yanxiufei.cn/gtbrlbmyvm.html

[U72] PHP：写错误日志
来源：http://hz.zhengqikj.top/gtdtzivgve.html

error_log("失败: " . $e->getMessage());
来源：http://hz.jianghu66.top/gtyvhiqrto.html

[U73] PHP：读取 ini 配置
来源：http://hz.ydjk.org.cn/gtecyirphe.html

parse_ini_file("config.ini", true)
来源：http://hz.xinyue.icu/gtmtipzpyl.html

[U74] PHP：读取环境变量
来源：http://hz.9152youxi.cn/gtonkvhtjc.html

getenv("APP_ENV") ?: "production"
来源：http://hz.jqgfzy.top/gtkwshwurc.html

[U75] PHP：依赖注入
来源：http://hz.hongshengwenyu.top/gtiyrkxgvt.html

composer require psr/container
来源：http://hz.jlsjyb.cn/gtdfxarrqd.html

[U76] PHP：简单路由
来源：http://hz.svipenyu.cn/gtzwylcxbu.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.dianchejie.cn/gtamcclgew.html

[U77] PHP：模板渲染
来源：http://hz.ydzc1.top/gtdhhyouej.html

composer require twig/twig
来源：http://hz.dianchejie.cn/gtwtgygtza.html

[U78] PHP：单元测试
来源：http://hz.ydjk.org.cn/gtceluoqfn.html

composer require --dev phpunit/phpunit
来源：http://hz.cucudq.cn/gtxeksdhpm.html

[U79] PHP：静态分析
来源：http://hz.vqdsnc.cn/gtfkxfnqjv.html

composer require --dev phpstan/phpstan
来源：http://hz.9152youxi.cn/gtpvddeeel.html

[U80] PHP：代码规范修复
来源：http://hz.gogol.net.cn/gthbnxklpc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.hfpthk.cn/gtyysvnexq.html

[U81] JS：初始化项目
来源：http://hz.shanyushiyangtech.top/gtomgotkbn.html

npm init -y;  npm i express
来源：http://hz.haohaochexian.top/gtcdolwwlf.html

[U82] JS：package.json 脚本
来源：http://hz.zhoulong.xyz/gthzpzlgfc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.yj202588.top/gtdashvznl.html

[U83] JS：ES Module 导入导出
来源：http://hz.yuxming.cn/gtzvktrptv.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.zdqjudy.top/gtjltsuzrq.html

[U84] JS：CommonJS 写法
来源：http://hz.9152youxi.cn/gtvnrldzcu.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.daria6918.cn/gtbdvmaqme.html

[U85] JS：可选链
来源：http://hz.tianlin.xyz/gtcdwixhwu.html

a?.b?.c
来源：http://hz.jqgufenzy.top/gtjqaquiom.html

[U86] JS：空值合并
来源：http://hz.cdnleiting.top/gtbwnezkfy.html

a ?? b
来源：http://hz.jinqigfzy.top/gtfckjlssj.html

[U87] JS：解构默认值
来源：http://hz.cqqwz.cn/gtqsjttsvt.html

const { a = 1, b = 2 } = obj;
来源：http://hz.iojbl.cn/gtxfartwqy.html

[U88] JS：对象展开合并
来源：http://hz.52xcode.cn/gtybfakedl.html

{ ...a, ...b }
来源：http://hz.snrcjt.cn/gtnfgwtxlh.html

[U89] JS：数组去重
来源：http://hz.fengsongda.top/gtgvtsmmrd.html

[...new Set(arr)]
来源：http://hz.ivvv.top/gtkjayfqsz.html

[U90] JS：数字数组排序
来源：http://hz.zhixingplan.top/gtlnrybjha.html

[...arr].sort((a, b) => a - b)
来源：http://hz.zhoulong.xyz/gtkanttkis.html

[U91] JS：对象键值遍历
来源：http://hz.yueranfly.top/gtpoqkinyo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.shanyushiyangtech.top/gtjhnotlic.html

[U92] JS：深拷贝
来源：http://hz.yangfankeji.com/gtvcpmytua.html

structuredClone(obj)
来源：http://hz.hfpthk.cn/gtkrbgimkk.html

[U93] JS：模板字符串
来源：http://hz.0kj1m.cn/gtbavsxsmv.html

`共 ${n} 条`
来源：http://hz.shanyushiyangkeji.top/gtaxmhviug.html

[U94] JS：箭头函数
来源：http://hz.chenjidiqi.icu/gtghhulbci.html

const double = x => x * 2;
来源：http://hz.zhaomingkeji.xyz/gtjirwsxul.html

[U95] JS：Promise 包装
来源：http://hz.zycfv.cn/gtldraqowu.html

new Promise((resolve, reject) => {})
来源：http://hz.cucudq.cn/gtaitlqlak.html

[U96] JS：async/await 与异常
来源：http://hz.guowangkeji.top/gtozzemkoj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.yuxming.cn/gtstckhigz.html

[U97] JS：并发请求
来源：http://hz.daxiang520.top/gtlirbygiz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cdnleiting.top/gtehqfzxgd.html

[U98] JS：fetch 带 JSON
来源：http://hz.xylfe.cn/gtpnkfrdax.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.0kj1m.cn/gtcmgymufl.html

[U99] JS：事件监听
来源：http://hz.guowangkeji.top/gtcpjbzljq.html

el.addEventListener("click", e => {})
来源：http://hz.sxryk.cn/gtlpamvgdl.html

[U100] JS：DOM 查询
来源：http://hz.smart0.xyz/gtddbbsqir.html

document.querySelector(".item")
来源：http://hz.yuxming.cn/gtmkvyytuo.html

[U101] JS：classList 操作
来源：http://hz.sysykeji.top/gtgurtlnfx.html

el.classList.toggle("active")
来源：http://hz.shanyushiyangtech.top/gtfyabtixm.html

[U102] JS：本地存储
来源：http://hz.aibaodan.cn/gtsdpxshhn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.ydzc1.top/gtuyopckyj.html

[U103] JS：定时器
来源：http://hz.guowangkeji.top/gtaullitoy.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.aizwys.cn/gtyhjcsdzy.html

[U104] JS：防抖
来源：http://hz.iojbl.cn/gtmarcrgvw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xuetiantiany.cn/gtrlmdnwjx.html

[U105] JS：节流
来源：http://hz.zhoulong.xyz/gtexwybfkb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.gotoacloud.top/gtpkxgnjcm.html

[U106] JS：日期格式化
来源：http://hz.shanyushiyangkeji.top/gtntgpzyrd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.zhixingplan.top/gtcywggaoj.html

[U107] JS：数字千分位
来源：http://hz.kuanghao11.cn/gtaxziibex.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.xuetiantiany.cn/gtdhndxcpa.html

[U108] JS：随机整数
来源：http://hz.xuanzx.com/gtraqcosum.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.jlsjyb.cn/gtcstxbjym.html

[U109] JS：数组分组
来源：http://hz.nwbrower.top/gtglfoxocv.html

Object.groupBy(arr, x => x.type)
来源：http://hz.zhengqikj.top/gtqwpugqrv.html

[U110] JS：数组分块
来源：http://hz.wangshuangyany.cn/gtbfvslban.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.sufxvd.cn/gtsbzrnekp.html

[U111] JS：对象转 Map
来源：http://hz.redwolf501.top/gtnrdwqfwi.html

new Map(Object.entries(obj))
来源：http://hz.0kj1m.cn/gtshqnjghz.html

[U112] JS：字符串补位
来源：http://hz.zhixingplan.top/gttkkjmmtc.html

"7".padStart(3, "0")
来源：http://hz.fengsongda.top/gtngkrshkk.html

[U113] JS：正则替换全部
来源：http://hz.c1oappe.top/gtaystteep.html

s.replaceAll("a", "b")
来源：http://hz.tianlin.xyz/gtqenqxsmn.html

[U114] JS：JSON 深比较
来源：http://hz.daxiang520.top/gtjmkrxbbc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.aibaodan.cn/gtqrqbgoto.html

[U115] JS：生成 UUID
来源：http://hz.zhengqikj.top/gtgrtjwxwu.html

crypto.randomUUID()
来源：http://hz.nwbrower.top/gtebozefvq.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.jqgufenzy.top/gtkfdanhad.html

/** @param {string} name */ function f(name) {}
来源：http://hz.chenzaomai.com/gtepdrjdgr.html

[U117] JS：单元测试
来源：http://hz.meibo888.top/gtywjgdamh.html

npm i -D vitest;  npx vitest
来源：http://hz.wangdashe.top/gtbuvuxpll.html

[U118] JS：开发服务器
来源：http://hz.iojbl.cn/gtbizsxoao.html

npm i -D vite;  npx vite
来源：http://hz.yongpay.top/gtbhqgapkl.html

[U119] JS：生产构建
来源：http://hz.daria6918.cn/gthmjntqur.html

npx vite build
来源：http://hz.chenlongwang.top/gtzggsfqsa.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.wangdashe.top/gttoqtktdo.html

import.meta.env.VITE_API_URL
来源：http://hz.daria6918.cn/gtboknmish.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtfkxesled.html

统计汇总
来源：http://hz.fengsongda.top/gtihqmggqw.html

================================================================================
来源：http://hz.sxryk.cn/gtwtkprkdp.html

按语言统计（条）：
来源：http://hz.yvedp.cn/gtjixrxzrs.html

Python ......... 252
来源：http://hz.chenlongwang.top/gtavbphxel.html

PHP ............ 252
来源：http://hz.hongshengwenyu.top/gtpsyncysb.html

JavaScript ..... 252
来源：http://hz.jiagoushi.top/gtruaqcnih.html

TypeScript ..... 212
来源：http://hz.pycfn.com/gtbkuvotpc.html

Java ........... 212
来源：http://hz.chenlongwang.top/gthkjojofz.html

Go ............. 212
来源：http://hz.hongshengwenyu.top/gtoyhfyjql.html

Ruby ........... 212
来源：http://hz.tianlin.xyz/gtvhjptvtm.html

C# ............. 212
来源：http://hz.jianghu66.top/gtrvvptxnx.html

C .............. 30
来源：http://hz.bjfxy.top/gtwmjiorke.html

C++ ............ 30
来源：http://hz.zhongyouzk.top/gtasdbdlah.html

SQL ............ 90
来源：http://hz.shzxlz.cn/gtkznzamfs.html

Bash ........... 80
来源：http://hz.sysykeji.top/gtbozfyzjl.html

Kotlin ......... 15
来源：http://hz.jlsjyb.cn/gtjjqxjacz.html

Swift .......... 15
来源：http://hz.zycfv.cn/gtnqyqqykr.html

Lua ............ 10
来源：http://hz.nanxinkj.top/gtxpzvhndw.html

Perl ........... 10
来源：http://hz.wangdashe.top/gtfftdmekg.html

Scala .......... 10
来源：http://hz.dianchejie.cn/gtegipcpbr.html

------------------------------------
来源：http://hz.guannengcc.top/gtapbohwys.html

合计 ........... 2106 条
来源：http://hz.quarkkingdee.top/gtjsenaies.html

按章节统计：
来源：http://hz.yvedp.cn/gtythqavqg.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.sufxvd.cn/gtjqiseeta.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yj20258888.top/gtjsasgrzp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.daxiang520.top/gtolkjpjmo.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.mhx1999.top/gtmvlgqvln.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.smart0.xyz/gtghxfyihx.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.nanxuanxn.top/gtnxinuwnh.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.yonumen.top/gtbbxtovlx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.zhengqikj.top/gtzaayoayk.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.birdmap.top/gtsdmriylp.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.daria6918.cn/gtvmsrxtxv.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.tian-w.cn/gtizhschwe.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.zycfv.cn/gttezzwrcg.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.aibaodan.cn/gthajjhxzl.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.yongpay.top/gtqnyhwusz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.shuidangran.top/gttfjtaoyj.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.xuetiantiany.cn/gthftroebs.html

Q SQL 专题                              90
来源：http://hz.sysykeji.top/gtgujozewc.html

R Bash 专题                             80
来源：http://hz.aizwys.cn/gtfcyhzzfu.html

S C / C++ 专题                          60
来源：http://hz.chenlongwang.top/gtpsugnyzl.html

T 其他语言补充                          60
来源：http://hz.ivvv.top/gtspfutmdn.html

U 高频实用片段                         120
来源：http://hz.52xcode.cn/gtvilhpahp.html

------------------------------------
来源：http://hz.birdmap.top/gtrxgoncxn.html

合计                                  2106 条
来源：http://hz.xuetiantiany.cn/gtscrcujio.html

--------------------------------------------------------------------------------
来源：http://hz.zhengqikj.top/gttvxctwot.html

使用提醒
来源：http://hz.316326.xyz/gtfbhvmoux.html

--------------------------------------------------------------------------------
来源：http://hz.iojbl.cn/gtoeqxrvkc.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.dashuyun.cn/gtltesgddn.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.zhijiandao.cn/gtnvjtkkyj.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.yueranfly.top/gtlkcspupp.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.hammf.cn/gtwtsectcb.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.zhongyouzk.top/gtbnnrwknx.html

—— 文件结束 ——
来源：http://hz.xuetiantiany.cn/gtspkbsmup.html

================================================================================
来源：http://hz.jinqigufen.top/gtexobucoi.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.zycfv.cn/gtntajetst.html

Common Programming Examples Cheat Book
来源：http://hz.ybcxt.top/gtafjbkwqx.html

================================================================================
来源：http://hz.shzxlz.cn/gtxuxeztvl.html

【收录内容】
来源：http://hz.ydzc1.top/gtjbwnsayy.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.quarkkingdee.top/gtrokjduyt.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.yongpay.top/gtzcgbmcdy.html

SQL · Bash · C · C++
来源：http://hz.yuxming.cn/gtgyghjzln.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.hysaishi.cn/gtsitqxzru.html

【使用说明】
来源：http://hz.hfpthk.cn/gtsbxbjffh.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.andypj.xyz/gtixlzslzc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.jqgufenzy.top/gtfrlylraj.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.ehwqpu.com/gtvvgzjtxv.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.ehwqpu.com/gtclclmljl.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.yvedp.cn/gthrnuntci.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.yonumen.top/gtvuwwrfyg.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.haohaochexian.top/gtmgqjqkdz.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.gotoacloud.top/gtwxlgcyxb.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.chenzaomai.com/gtszvvmlwt.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.52xcode.cn/gtouoxpxnf.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.haohaochexian.top/gtakzxeaxe.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.aizwys.cn/gtwjdkmsor.html

【文件统计】
来源：http://hz.zhiwuduotai.top/gtxevtvdwx.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.bjfxy.top/gtvrcaucbd.html

--------------------------------------------------------------------------------
来源：http://hz.jinqigufen.top/gtajqlainm.html

目  录
来源：http://hz.yj20258888.top/gtwdszcdqb.html

--------------------------------------------------------------------------------
来源：http://hz.sxryk.cn/gtknrkeatv.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.0kj1m.cn/gtmtvaiuds.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.nanxinkj.top/gtdzeeelcs.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.xingfuxueyuan.xyz/gtvpifwhlv.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.jinyuanbaomall.cn/gtzhvxbvum.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.yonumen.top/gtzqlxaxxu.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.yj202588.top/gtqhmczjva.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.yj202588.top/gtuuklttzj.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.chenlongwang.top/gtmlotvqbk.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.gzhubu.top/gtmsdxuowt.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.feifeiyinyue.top/gtslripvds.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.jyoumei.cn/gtvgzbhcbs.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.shanyushiyangkeji.top/gtmcilaues.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.zhaomingkeji.xyz/gtdtpnuvev.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.aibaodan.cn/gtcgudvhsu.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.chenzaomai.com/gtkvnevtzj.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.wangdashe.top/gtkvnxwjup.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.cqqwz.cn/gthguyiahn.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.cashguo.top/gttmafwevh.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.ywan-chungtsiang.top/gtgglflrot.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.9152youxi.cn/gtvfxxaqfa.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.nanxinkj.top/gtlsuantbp.html

================================================================================
来源：http://hz.hysaishi.cn/gtjraqmbrg.html

A. 基础语法与类型
来源：http://hz.hywenlv.cn/gtmuecmvgt.html

================================================================================
来源：http://hz.iojbl.cn/gtvjbrragj.html

[A01] Hello World
来源：http://hz.svipenyu.cn/gtpqyuyhbc.html

Py:   print("Hello, World!")
来源：http://hz.shanyushiyangkeji.top/gtfibcmhjz.html

PHP:  echo "Hello, World!";
来源：http://hz.yvedp.cn/gtdgeyaovi.html

JS:   console.log("Hello, World!");
来源：http://hz.yongpay.top/gtrhbrrggp.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.hnxiangtu.top/gtmlmenpmx.html

Java: System.out.println("Hello, World!");
来源：http://hz.yuanzhike.top/gtmhdkxlwg.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.nwbrower.top/gtihwnyvds.html

Ruby: puts "Hello, World!"
来源：http://hz.gotoacloud.top/gtdjojiksg.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.chenjidiqi.icu/gtbcwrwsei.html

[A02] 变量声明与赋值
来源：http://hz.jinghuilouyu.cn/gtphvrvtlb.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.cucudq.cn/gttpfcxmvj.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.ydjk.org.cn/gtetqzruui.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.cashguo.top/gtglkjwopc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.yonumen.top/gtpljhfjtq.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.fengsongda.top/gtwdvbussm.html

Go:   name := "Alex"; age := 20
来源：http://hz.zdqjudy.top/gtmnzunrhy.html

Ruby: name = "Alex"; age = 20
来源：http://hz.zdqjudy.top/gtzuqmkprd.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.9152youxi.cn/gtbgxtkalp.html

[A03] 常量定义
来源：http://hz.xziqi.cn/gtbsiejygf.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.hysaishi.cn/gtywabujtl.html

PHP:  const PI = 3.14159;
来源：http://hz.zhiwuduotai.top/gtwcujyvdf.html

JS:   const PI = 3.14159;
来源：http://hz.jqgfzy.top/gtlxipoblc.html

TS:   const PI: number = 3.14159;
来源：http://hz.tian-w.cn/gtgkagkbss.html

Java: static final double PI = 3.14159;
来源：http://hz.sufxvd.cn/gtzhingoax.html

Go:   const PI = 3.14159
来源：http://hz.aibaodan.cn/gtwohyknlp.html

Ruby: PI = 3.14159
来源：http://hz.nanxuanxn.top/gtvgighczy.html

C#:   const double PI = 3.14159;
来源：http://hz.hnqzz.top/gtxgsyyhvr.html

[A04] 判断变量类型
来源：http://hz.zdqjudy.top/gtqljybiex.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.smart0.xyz/gtzfzietle.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.hysaishi.cn/gtpbniahpu.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.zhaomingkeji.xyz/gtbealvwcz.html

TS:   typeof x; x instanceof Date
来源：http://hz.jqgufenzy.top/gtxwvwcioo.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.hywenlv.cn/gtaeojfeec.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.snrcjt.cn/gtyttqwcrl.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.0kj1m.cn/gtiepabvmq.html

C#:   x.GetType().Name; x is int
来源：http://hz.yangfankeji.com/gtnxfybysv.html

[A05] 整数除法与取模
来源：http://hz.quarkkingdee.top/gtnrerzopg.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.zhixingplan.top/gtfhvpbqsk.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.jiagoushi.top/gtfaampbgg.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.shanyushiyangkeji.top/gtbinhrvxv.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.jiagoushi.top/gtutkofowb.html

Java: 7 / 2; 7 % 2
来源：http://hz.yvedp.cn/gtertrtgms.html

Go:   7 / 2; 7 % 2
来源：http://hz.chenzaomai.com/gtjjghakwx.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.havefunace.top/gtvfmhljbb.html

C#:   7 / 2; 7 % 2
来源：http://hz.gaohongyu789.top/gtwnaqdkqd.html

[A06] 字符串转数字
来源：http://hz.jqgufenzy.top/gttcmxbgzc.html

Py:   int("42"); float("3.14")
来源：http://hz.aibaodan.cn/gtgojuijoj.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.cucudq.cn/gtotpolshd.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.xinyue.icu/gtzadbkeub.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.cqqwz.cn/gtqwmwguqn.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.smart0.xyz/gtmmtlobla.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.yueranfly.top/gtbquaytsx.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.shanyushiyangkeji.top/gtmryxgdwr.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.yongpay.top/gtbqnillbc.html

[A07] 数字转字符串
来源：http://hz.hnxiangtu.top/gtuoxifkko.html

Py:   str(42)
来源：http://hz.sysykeji.top/gtxeekeccj.html

PHP:  (string) 42; strval(42)
来源：http://hz.fzhhl.top/gtaxoxcrtp.html

JS:   String(42); (42).toString()
来源：http://hz.tian-w.cn/gtutrtxtad.html

TS:   String(42)
来源：http://hz.zhaomingkeji.xyz/gtsvihmafk.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.gogol.net.cn/gtfzcextxg.html

Go:   strconv.Itoa(42)
来源：http://hz.mhx1999.top/gtjfwqrvfb.html

Ruby: 42.to_s
来源：http://hz.xziqi.cn/gtbmwdlalv.html

C#:   42.ToString()
来源：http://hz.9152youxi.cn/gtlxprwpdj.html

[A08] 取整与四舍五入
来源：http://hz.ydjk.org.cn/gtdwyfyiis.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.xziqi.cn/gtobeuuoxt.html


<!-- 参考信息 -->