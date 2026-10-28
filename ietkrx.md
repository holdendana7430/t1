代发 wailian999

[U61] PHP：正则
来源：http://hz.yuanzhike.top/gtjqipcpxa.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.shanyushiyangkeji.top/gtchiwkjfu.html

[U62] PHP：日期对象
来源：http://hz.jyoumei.cn/gtagogoiil.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.zhijiandao.cn/gtluafotis.html

[U63] PHP：文件读写
来源：http://hz.xylfe.cn/gtfhoeimms.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.pycfn.com/gtetatzxhr.html

[U64] PHP：目录遍历
来源：http://hz.tian-w.cn/gtgutlocof.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.jianghu66.top/gtkokomucr.html

[U65] PHP：会话
来源：http://hz.yangfankeji.com/gtjjehborf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.sufxvd.cn/gtvjvzvxjg.html

[U66] PHP：设置 Cookie
来源：http://hz.dianchejie.cn/gtzfnpcesi.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.yuanzhike.top/gtyzzjzcuv.html

[U67] PHP：处理文件上传
来源：http://hz.gzhubu.top/gttepelrlw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.mhx1999.top/gtrniehrew.html

[U68] PHP：PDO 连接
来源：http://hz.chenjidiqi.icu/gtillwvvfd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.yangfankeji.com/gtdobeiuiy.html

[U69] PHP：PDO 预处理
来源：http://hz.xziqi.cn/gtdvtfcdqn.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.dashuyun.cn/gtazztenxa.html

[U70] PHP：PDO 事务
来源：http://hz.shuidangran.top/gttgupyzsk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.yonumen.top/gttrxlaebo.html

[U71] PHP：抛出异常
来源：http://hz.bjfxy.top/gtygjvwmwf.html

throw new RuntimeException("失败", 500);
来源：http://hz.sufxvd.cn/gtxjurhyef.html

[U72] PHP：写错误日志
来源：http://hz.snrcjt.cn/gtdufvdqha.html

error_log("失败: " . $e->getMessage());
来源：http://hz.zhixingplan.top/gtbtzzpqrh.html

[U73] PHP：读取 ini 配置
来源：http://hz.shuidangran.top/gtqvflitkf.html

parse_ini_file("config.ini", true)
来源：http://hz.birdmap.top/gtsoearhgu.html

[U74] PHP：读取环境变量
来源：http://hz.ydzc1.top/gtxgipfdnx.html

getenv("APP_ENV") ?: "production"
来源：http://hz.shangyingyoupin.top/gtrkunwufm.html

[U75] PHP：依赖注入
来源：http://hz.aibaodan.cn/gtcqiaulre.html

composer require psr/container
来源：http://hz.jyoumei.cn/gtkyrulgku.html

[U76] PHP：简单路由
来源：http://hz.dashuyun.cn/gtfghuijoz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.smart0.xyz/gtorofcwnz.html

[U77] PHP：模板渲染
来源：http://hz.hammf.cn/gtptofzjju.html

composer require twig/twig
来源：http://hz.mhx1999.top/gtktyydwla.html

[U78] PHP：单元测试
来源：http://hz.jqgfzy.top/gtwilfhxpr.html

composer require --dev phpunit/phpunit
来源：http://hz.dianchejie.cn/gtprhdxizi.html

[U79] PHP：静态分析
来源：http://hz.sxryk.cn/gtemgjtnly.html

composer require --dev phpstan/phpstan
来源：http://hz.hywenlv.cn/gtnubntvee.html

[U80] PHP：代码规范修复
来源：http://hz.smart0.xyz/gtpoywoaqi.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.mhx1999.top/gtemsbnelk.html

[U81] JS：初始化项目
来源：http://hz.iojbl.cn/gtybkoglhn.html

npm init -y;  npm i express
来源：http://hz.shanyushiyangkeji.top/gtcdrmmbpm.html

[U82] JS：package.json 脚本
来源：http://hz.zhaomingkeji.xyz/gtmzkaztjz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.andypj.xyz/gtedrpimyw.html

[U83] JS：ES Module 导入导出
来源：http://hz.aizwys.cn/gtsmplakxj.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.jyoumei.cn/gtlkblydrg.html

[U84] JS：CommonJS 写法
来源：http://hz.aizwys.cn/gtixfxnvtb.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.jinqigufen.top/gtwalgecrv.html

[U85] JS：可选链
来源：http://hz.shzxlz.cn/gtmzwkkjyc.html

a?.b?.c
来源：http://hz.shzxlz.cn/gtaaywicwt.html

[U86] JS：空值合并
来源：http://hz.yangfankeji.com/gtbcobzwyk.html

a ?? b
来源：http://hz.yj20258888.top/gtidrlojjr.html

[U87] JS：解构默认值
来源：http://hz.cashguo.top/gtfhdrzmqy.html

const { a = 1, b = 2 } = obj;
来源：http://hz.wangdashe.top/gtwbcmltyy.html

[U88] JS：对象展开合并
来源：http://hz.ppjwa.cn/gtpazjqeqt.html

{ ...a, ...b }
来源：http://hz.dashuyun.cn/gtlhvtdaxf.html

[U89] JS：数组去重
来源：http://hz.birdmap.top/gtksoxsdyo.html

[...new Set(arr)]
来源：http://hz.fzhhl.top/gtbbasutiq.html

[U90] JS：数字数组排序
来源：http://hz.gaohongyu789.top/gtjdvsvjni.html

[...arr].sort((a, b) => a - b)
来源：http://hz.yonumen.top/gtsjcxqwjo.html

[U91] JS：对象键值遍历
来源：http://hz.cheryme.top/gtylsgwbgv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.jinyuanbaomall.cn/gtvfhobbph.html

[U92] JS：深拷贝
来源：http://hz.shzxlz.cn/gtclqiguoc.html

structuredClone(obj)
来源：http://hz.jiagoushi.top/gtolxksvmx.html

[U93] JS：模板字符串
来源：http://hz.zhoulong.xyz/gtzrujhysx.html

`共 ${n} 条`
来源：http://hz.jinghuilouyu.cn/gtkzotnfgg.html

[U94] JS：箭头函数
来源：http://hz.chenjidiqi.icu/gtzqsbkdhg.html

const double = x => x * 2;
来源：http://hz.yj20258888.top/gtyzkkqtxq.html

[U95] JS：Promise 包装
来源：http://hz.yvedp.cn/gtvqwlkfus.html

new Promise((resolve, reject) => {})
来源：http://hz.zdqjudy.top/gtbkyvihbl.html

[U96] JS：async/await 与异常
来源：http://hz.guannengcc.top/gtggziuvex.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.cdnleiting.top/gtkpqfucjh.html

[U97] JS：并发请求
来源：http://hz.ydjk.org.cn/gtklvwchup.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhijiandao.cn/gthcjcenfu.html

[U98] JS：fetch 带 JSON
来源：http://hz.haohaochexian.top/gtlhhfjasg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.yueranfly.top/gtdhnygdsg.html

[U99] JS：事件监听
来源：http://hz.smart0.xyz/gthhdfiplx.html

el.addEventListener("click", e => {})
来源：http://hz.havefunace.top/gtttarimuh.html

[U100] JS：DOM 查询
来源：http://hz.guowangkeji.top/gtkkazfhwq.html

document.querySelector(".item")
来源：http://hz.ybcxt.top/gtbelsewtm.html

[U101] JS：classList 操作
来源：http://hz.yangfankeji.com/gtwtubkfkr.html

el.classList.toggle("active")
来源：http://hz.jinyuanbaomall.cn/gtsytrzmxk.html

[U102] JS：本地存储
来源：http://hz.jqgfzy.top/gtioavbxxn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.nanxinkj.top/gtqatucipt.html

[U103] JS：定时器
来源：http://hz.nanxuanxn.top/gtjaxnrrcl.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.yangfankeji.com/gtrjtzmikw.html

[U104] JS：防抖
来源：http://hz.tian-w.cn/gtletygdoa.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.tanke756.top/gtcstcdbdq.html

[U105] JS：节流
来源：http://hz.haohaochexian.top/gtqylrugfb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.ppjwa.cn/gtczvscrrb.html

[U106] JS：日期格式化
来源：http://hz.9152youxi.cn/gtliferspj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.ehwqpu.com/gtlovbvqwz.html

[U107] JS：数字千分位
来源：http://hz.wangdashe.top/gteugzzwbu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.shuidangran.top/gtqtlvgljr.html

[U108] JS：随机整数
来源：http://hz.sxryk.cn/gtwqolkbka.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.aizwys.cn/gtcyrtpeoj.html

[U109] JS：数组分组
来源：http://hz.shzxlz.cn/gtlggrxqvb.html

Object.groupBy(arr, x => x.type)
来源：http://hz.gogol.net.cn/gtndoslkvn.html

[U110] JS：数组分块
来源：http://hz.shzxlz.cn/gtmimqoqbu.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.dashuyun.cn/gtyhsczruw.html

[U111] JS：对象转 Map
来源：http://hz.yueranfly.top/gtjgwuxqcb.html

new Map(Object.entries(obj))
来源：http://hz.bjfxy.top/gtcmhmgign.html

[U112] JS：字符串补位
来源：http://hz.yuxming.cn/gtazxeovuz.html

"7".padStart(3, "0")
来源：http://hz.guannengcc.top/gtdmpmtggc.html

[U113] JS：正则替换全部
来源：http://hz.guannengcc.top/gthmvfzrqo.html

s.replaceAll("a", "b")
来源：http://hz.c1oappe.top/gtyjsgyygp.html

[U114] JS：JSON 深比较
来源：http://hz.bjfxy.top/gtlyprhxnv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.quarkkingdee.top/gtikirydfl.html

[U115] JS：生成 UUID
来源：http://hz.sxryk.cn/gttpeumlxz.html

crypto.randomUUID()
来源：http://hz.cqqwz.cn/gtxcbaahzg.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.xuetiantiany.cn/gthcsxdwln.html

/** @param {string} name */ function f(name) {}
来源：http://hz.jqgufenzy.top/gtemifqoqf.html

[U117] JS：单元测试
来源：http://hz.zhixingplan.top/gtbjaqklox.html

npm i -D vitest;  npx vitest
来源：http://hz.zhoulong.xyz/gtwqfjewzu.html

[U118] JS：开发服务器
来源：http://hz.sweek.top/gtfbomgicw.html

npm i -D vite;  npx vite
来源：http://hz.hysaishi.cn/gtbkclgiad.html

[U119] JS：生产构建
来源：http://hz.sxryk.cn/gtksjchfzl.html

npx vite build
来源：http://hz.zhiwuduotai.top/gtjzgfpgzt.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.xziqi.cn/gtetiwepmc.html

import.meta.env.VITE_API_URL
来源：http://hz.daxiang520.top/gtfqfspraz.html

================================================================================
来源：http://hz.tianlin.xyz/gtmefkkrzo.html

统计汇总
来源：http://hz.fengsongda.top/gtqxqciagq.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtopfnyztz.html

按语言统计（条）：
来源：http://hz.havefunace.top/gtxpkgmbag.html

Python ......... 252
来源：http://hz.zhijiandao.cn/gthkzvigaw.html

PHP ............ 252
来源：http://hz.hfpthk.cn/gtmidfrxoq.html

JavaScript ..... 252
来源：http://hz.yueranfly.top/gtlkuslvjj.html

TypeScript ..... 212
来源：http://hz.zhoulong.xyz/gtakerpkem.html

Java ........... 212
来源：http://hz.feifeiyinyue.top/gtoktizial.html

Go ............. 212
来源：http://hz.jianghu66.top/gtgcccxduy.html

Ruby ........... 212
来源：http://hz.shzxlz.cn/gtdalayhpp.html

C# ............. 212
来源：http://hz.svipenyu.cn/gtbyiglqhd.html

C .............. 30
来源：http://hz.yonumen.top/gtppwoutqq.html

C++ ............ 30
来源：http://hz.haohaochexian.top/gtkggarred.html

SQL ............ 90
来源：http://hz.cheryme.top/gtpmxnidnt.html

Bash ........... 80
来源：http://hz.ivvv.top/gtmafpwyhe.html

Kotlin ......... 15
来源：http://hz.daxiang520.top/gtajidqzue.html

Swift .......... 15
来源：http://hz.gogol.net.cn/gtuquhpnul.html

Lua ............ 10
来源：http://hz.yj20258.top/gtblivqres.html

Perl ........... 10
来源：http://hz.hammf.cn/gtgezyavco.html

Scala .......... 10
来源：http://hz.52xcode.cn/gtwbxayike.html

------------------------------------
来源：http://hz.zhixingplan.top/gtpzgcfwjd.html

合计 ........... 2106 条
来源：http://hz.guannengcc.top/gtnuwpevtt.html

按章节统计：
来源：http://hz.hywenlv.cn/gtquqobddi.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.wangshuangyany.cn/gttnmpjhgq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.ywan-chungtsiang.top/gtuutndqgi.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.zhijiandao.cn/gtlbngogum.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.wangshuangyany.cn/gtnlfevpdv.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.ivvv.top/gtzwuwppkk.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.cqqwz.cn/gtpwwfbfjl.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.xuanzx.com/gtfonbvcuq.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.hnqzz.top/gtilghgjyi.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.shanyushiyangkeji.top/gtbufqnyyq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.shuidangran.top/gtzsidbhar.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.hnqzz.top/gteexpbpcx.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.xinyue.icu/gtqsjdzkyr.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.zdqjudy.top/gtuznvdywm.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.yvedp.cn/gtqhathryc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.yangfankeji.com/gtpjbzaclg.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.nanxinkj.top/gtvdxynexr.html

Q SQL 专题                              90
来源：http://hz.zhaomingkeji.xyz/gtzoelrbci.html

R Bash 专题                             80
来源：http://hz.kuanghao11.cn/gtdjvwbgxx.html

S C / C++ 专题                          60
来源：http://hz.tianlin.xyz/gtwvarcopb.html

T 其他语言补充                          60
来源：http://hz.dianchejie.cn/gtnhajhocu.html

U 高频实用片段                         120
来源：http://hz.hongshengwenyu.top/gtemwmmobi.html

------------------------------------
来源：http://hz.hongshengwenyu.top/gtforxiymm.html

合计                                  2106 条
来源：http://hz.hysaishi.cn/gtonvhguya.html

--------------------------------------------------------------------------------
来源：http://hz.daxiang520.top/gtvaolckup.html

使用提醒
来源：http://hz.andypj.xyz/gtbbrdxipu.html

--------------------------------------------------------------------------------
来源：http://hz.shuidangran.top/gttomrplfw.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.havefunace.top/gtvyycpuyz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.fzhhl.top/gtwasbxcpi.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.jinqigufen.top/gtcfoimxmh.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.zhongyouzk.top/gtvmfdfujn.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.ivvv.top/gtzfqgnvzg.html

—— 文件结束 ——
来源：http://hz.gogol.net.cn/gtuemaewcd.html

================================================================================
来源：http://hz.hammf.cn/gtharqntww.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.haohaochexian.top/gtwwpgnzxj.html

Common Programming Examples Cheat Book
来源：http://hz.ydzc1.top/gtyhetumro.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtuwobabeh.html

【收录内容】
来源：http://hz.zhoulong.xyz/gtxlsuunvu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.nanxinkj.top/gtdymujofu.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.bjfxy.top/gtzanmschd.html

SQL · Bash · C · C++
来源：http://hz.jianghu66.top/gtavzajslb.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.yonumen.top/gtcubpivwf.html

【使用说明】
来源：http://hz.shangyingyoupin.top/gtnuvhadex.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.jinqigfzy.top/gtdctfglkb.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.xziqi.cn/gtrmwtdglg.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.ybcxt.top/gtwkjileob.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.sweek.top/gttotpfkjq.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.shanyushiyangtech.top/gtbkhxdiom.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.aizwys.cn/gttltjrrug.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.nwbrower.top/gtooocgter.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.zhiwuduotai.top/gtlzwcwgvh.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.cucudq.cn/gtsyorqqgs.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.cheryme.top/gtwwnwpwvw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.tian-w.cn/gtkunfdacc.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.cdnleiting.top/gtvhlbpbqz.html

【文件统计】
来源：http://hz.xinyue.icu/gtemthjcrc.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.nwbrower.top/gtvdnfktrr.html

--------------------------------------------------------------------------------
来源：http://hz.hongshengwenyu.top/gtlbotpjco.html

目  录
来源：http://hz.tian-w.cn/gttwacrpne.html

--------------------------------------------------------------------------------
来源：http://hz.9152youxi.cn/gtghhxuklh.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.hammf.cn/gtnztkimqr.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.meibo888.top/gtxuxoyjwb.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.jinqigfzy.top/gtzryyytpt.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.dashuyun.cn/gtcjfmulya.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.chenzaomai.com/gtcmdcoutt.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.zhengqikj.top/gtxkaojnup.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.sufxvd.cn/gtlwppbojf.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.hnqzz.top/gtpjbsvdvs.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.zhaomingkeji.xyz/gtffhoaukj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.smart0.xyz/gtdgamilcn.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.chenlongwang.top/gtmpqrftlj.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.yongpay.top/gtiahjsyns.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.cashguo.top/gthgwfczgx.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.ppjwa.cn/gtaxbklofh.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.cucudq.cn/gtkgkihabr.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.ivvv.top/gtakjhsjyk.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.xingfuxueyuan.xyz/gtxdvfjawz.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.c1oappe.top/gtuodemtpp.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.fengsongda.top/gtcadbshuq.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jqgfzy.top/gtnotiaxju.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.fzhhl.top/gtwtxgqyfu.html

================================================================================
来源：http://hz.cucudq.cn/gtvbsobxet.html

A. 基础语法与类型
来源：http://hz.guowangkeji.top/gtmxzbtevq.html

================================================================================
来源：http://hz.meibo888.top/gtfzhrzgnj.html

[A01] Hello World
来源：http://hz.ywan-chungtsiang.top/gtpzchpphl.html

Py:   print("Hello, World!")
来源：http://hz.xziqi.cn/gtyexedjcn.html

PHP:  echo "Hello, World!";
来源：http://hz.yj202588.top/gtvztlawvg.html

JS:   console.log("Hello, World!");
来源：http://hz.xylfe.cn/gtbibzbcht.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.xylfe.cn/gttewakyab.html

Java: System.out.println("Hello, World!");
来源：http://hz.zhijiandao.cn/gtvwyermgw.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.nwbrower.top/gtspfoqxly.html

Ruby: puts "Hello, World!"
来源：http://hz.zhiwuduotai.top/gtcdflbbka.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.hongshengwenyu.top/gtxyacncdn.html

[A02] 变量声明与赋值
来源：http://hz.yanxiufei.cn/gtuxhqrtbs.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.jianghu66.top/gtlnalkhtl.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.hammf.cn/gtphqpikzv.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.andypj.xyz/gtiujxlayq.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.pycfn.com/gtmmirrjcg.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.c1oappe.top/gtvgjtyjxv.html

Go:   name := "Alex"; age := 20
来源：http://hz.pengpengdd.cyou/gtzyjxgtdc.html

Ruby: name = "Alex"; age = 20
来源：http://hz.cashguo.top/gtpfzvudcf.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.smart0.xyz/gtvvuxkkas.html

[A03] 常量定义
来源：http://hz.52xcode.cn/gtnuilhgyc.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.tanke756.top/gtyroojrfc.html

PHP:  const PI = 3.14159;
来源：http://hz.jiagoushi.top/gtxipvfzvw.html

JS:   const PI = 3.14159;
来源：http://hz.hnxiangtu.top/gtychgjqew.html

TS:   const PI: number = 3.14159;
来源：http://hz.hammf.cn/gtvmooohiv.html

Java: static final double PI = 3.14159;
来源：http://hz.kuanghao11.cn/gtfoyxsajt.html

Go:   const PI = 3.14159
来源：http://hz.andypj.xyz/gtmdkfwlrf.html

Ruby: PI = 3.14159
来源：http://hz.hysaishi.cn/gtzojyspmz.html

C#:   const double PI = 3.14159;
来源：http://hz.yuanzhike.top/gtbyxrenyp.html

[A04] 判断变量类型
来源：http://hz.mhx1999.top/gtmxqcpxyi.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.hnxiangtu.top/gtfjwxybjs.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.pengpengdd.cyou/gtbkcbvhjz.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.nanxuanxn.top/gtztcjkbhi.html

TS:   typeof x; x instanceof Date
来源：http://hz.jqgufenzy.top/gtihbhjefn.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.sysykeji.top/gtsdzxrbpr.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.wangdashe.top/gtybretnwb.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.sufxvd.cn/gtuophegnk.html

C#:   x.GetType().Name; x is int
来源：http://hz.yonumen.top/gtxkouvzse.html

[A05] 整数除法与取模
来源：http://hz.jianghu66.top/gtdxpkkhxj.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.wangdashe.top/gtneaunrta.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.hnxiangtu.top/gtcpnxwmsy.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.shangyingyoupin.top/gtzrazfzot.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.xingfuxueyuan.xyz/gtrcddlnaj.html

Java: 7 / 2; 7 % 2
来源：http://hz.jinghuilouyu.cn/gtoinxswld.html

Go:   7 / 2; 7 % 2
来源：http://hz.jiagoushi.top/gtxjufiiaz.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.yangfankeji.com/gtouethpzd.html

C#:   7 / 2; 7 % 2
来源：http://hz.hywenlv.cn/gtnluhzrbi.html

[A06] 字符串转数字
来源：http://hz.dashuyun.cn/gtjnmdatib.html

Py:   int("42"); float("3.14")
来源：http://hz.dianchejie.cn/gthtwujzxg.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.tian-w.cn/gtnbuyesqy.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.zhengqikj.top/gtbyppzgjh.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.yueranfly.top/gtpxkcymvx.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.ehwqpu.com/gtjhttetem.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.yonumen.top/gtvjbnmbpk.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.yongpay.top/gtlerzdieg.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.zhaomingkeji.xyz/gtnorqulxj.html

[A07] 数字转字符串
来源：http://hz.bjfxy.top/gtqaxribjt.html

Py:   str(42)
来源：http://hz.hammf.cn/gtrchwmufm.html

PHP:  (string) 42; strval(42)
来源：http://hz.gogol.net.cn/gtuirufbcb.html

JS:   String(42); (42).toString()
来源：http://hz.zhongyouzk.top/gtkiqzwcju.html

TS:   String(42)
来源：http://hz.gotoacloud.top/gtsbqtlqqb.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.xinyue.icu/gtqgpstkgn.html

Go:   strconv.Itoa(42)
来源：http://hz.vqdsnc.cn/gtnzudbswx.html

Ruby: 42.to_s
来源：http://hz.daria6918.cn/gttcgnxzcy.html

C#:   42.ToString()
来源：http://hz.c1oappe.top/gtcekzhbgt.html

[A08] 取整与四舍五入
来源：http://hz.ivvv.top/gtptsfowiy.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.jqgfzy.top/gtzhzmmgsy.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.jianghu66.top/gtkylkdxrj.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.feifeiyinyue.top/gtwgkpbnkp.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.sysykeji.top/gtzkfnxizv.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.316326.xyz/gtfwzmpuqj.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.hongshengwenyu.top/gtesmntrkk.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.shanyushiyangtech.top/gtmkcqjstk.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.zdqjudy.top/gtmnprampd.html

[A09] 绝对值与最大最小值
来源：http://hz.sweek.top/gtllqhnldb.html


<!-- 参考信息 -->