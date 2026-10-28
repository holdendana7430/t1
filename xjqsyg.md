代发 wailian999

[U53] PHP：空合并运算符
来源：http://hz.yvedp.cn/gteqwbjpin.html

$v = $a ?? $b ?? "default";
来源：http://hz.xinyue.icu/gtjkroixqc.html

[U54] PHP：空安全调用
来源：http://hz.zhaomingkeji.xyz/gtwbfbbdij.html

$obj?->method()
来源：http://hz.cucudq.cn/gtzffzggdk.html

[U55] PHP：match 表达式
来源：http://hz.yueranfly.top/gtqgdwuvja.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.iojbl.cn/gtqwntxyed.html

[U56] PHP：命名参数
来源：http://hz.yangfankeji.com/gtttnwabmh.html

f(a: 1, b: 2)
来源：http://hz.0kj1m.cn/gtdpemtssy.html

[U57] PHP：字符串插值
来源：http://hz.yuxming.cn/gtnhdipljo.html

"值: {$a}"
来源：http://hz.redwolf501.top/gtukyuaikf.html

[U58] PHP：数组三件套
来源：http://hz.hywenlv.cn/gtkbtauhjp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.nanxuanxn.top/gtkvitlbtd.html

[U59] PHP：自定义排序
来源：http://hz.shangyingyoupin.top/gticfwwjqs.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhoulong.xyz/gtmqlrttri.html

[U60] PHP：JSON 编解码
来源：http://hz.bjfxy.top/gtjhrlfboq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.wangdashe.top/gtnzifesiy.html

[U61] PHP：正则
来源：http://hz.shzxlz.cn/gtnugwpgzm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.ybcxt.top/gtuzfjlyhz.html

[U62] PHP：日期对象
来源：http://hz.yvedp.cn/gtadgrryfr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.sxryk.cn/gtfhfnqzjq.html

[U63] PHP：文件读写
来源：http://hz.316326.xyz/gtdnicislg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.sufxvd.cn/gttjxnchrj.html

[U64] PHP：目录遍历
来源：http://hz.tianlin.xyz/gtczxedfxj.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.guannengcc.top/gttpiqcvln.html

[U65] PHP：会话
来源：http://hz.guannengcc.top/gtetjtaavb.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.zhaomingkeji.xyz/gtulquwdxl.html

[U66] PHP：设置 Cookie
来源：http://hz.yueranfly.top/gtoblvvhmi.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.hfpthk.cn/gtymvbflkl.html

[U67] PHP：处理文件上传
来源：http://hz.chenzaomai.com/gtbywtiyax.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.0kj1m.cn/gtqjplxexx.html

[U68] PHP：PDO 连接
来源：http://hz.xziqi.cn/gtzwrrjhwx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.gzhubu.top/gttsyympoq.html

[U69] PHP：PDO 预处理
来源：http://hz.zhaomingkeji.xyz/gtljjingtz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.jianghu66.top/gtixammkye.html

[U70] PHP：PDO 事务
来源：http://hz.shanyushiyangtech.top/gtnmzjllef.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.dianchejie.cn/gtztnqowtp.html

[U71] PHP：抛出异常
来源：http://hz.jlsjyb.cn/gtvwhotjbm.html

throw new RuntimeException("失败", 500);
来源：http://hz.nwbrower.top/gtzszzfisz.html

[U72] PHP：写错误日志
来源：http://hz.wangshuangyany.cn/gtvplexhma.html

error_log("失败: " . $e->getMessage());
来源：http://hz.gogol.net.cn/gtaxyecwmp.html

[U73] PHP：读取 ini 配置
来源：http://hz.jinqigfzy.top/gtgfntdxqo.html

parse_ini_file("config.ini", true)
来源：http://hz.gaohongyu789.top/gtrpstpbgc.html

[U74] PHP：读取环境变量
来源：http://hz.dianchejie.cn/gtjoppfvnn.html

getenv("APP_ENV") ?: "production"
来源：http://hz.zhixingplan.top/gtvxjbbadu.html

[U75] PHP：依赖注入
来源：http://hz.svipenyu.cn/gtsbbjjkus.html

composer require psr/container
来源：http://hz.haohaochexian.top/gtnasgpzcf.html

[U76] PHP：简单路由
来源：http://hz.vqdsnc.cn/gtepsrrlsf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.pycfn.com/gtcitvgryx.html

[U77] PHP：模板渲染
来源：http://hz.jinqigufen.top/gtslllxlpq.html

composer require twig/twig
来源：http://hz.ywan-chungtsiang.top/gtgmtkhayv.html

[U78] PHP：单元测试
来源：http://hz.ehwqpu.com/gtxsvmxzrs.html

composer require --dev phpunit/phpunit
来源：http://hz.52xcode.cn/gtzntpgbdt.html

[U79] PHP：静态分析
来源：http://hz.daxiang520.top/gtjgkeuxfj.html

composer require --dev phpstan/phpstan
来源：http://hz.jyoumei.cn/gtmgbvjwat.html

[U80] PHP：代码规范修复
来源：http://hz.yj202588.top/gtnupbfwui.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.gzhubu.top/gtvwqkjvho.html

[U81] JS：初始化项目
来源：http://hz.gogol.net.cn/gtteoehsiq.html

npm init -y;  npm i express
来源：http://hz.shzxlz.cn/gtrntyzqhh.html

[U82] JS：package.json 脚本
来源：http://hz.chenzaomai.com/gtfzteyvlg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.yonumen.top/gtlzycunth.html

[U83] JS：ES Module 导入导出
来源：http://hz.xuetiantiany.cn/gtenqvfzij.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.meibo888.top/gtojfexghf.html

[U84] JS：CommonJS 写法
来源：http://hz.cashguo.top/gtnwhpwrvq.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.cheryme.top/gtnbmsrzah.html

[U85] JS：可选链
来源：http://hz.ybcxt.top/gtltqsqjpj.html

a?.b?.c
来源：http://hz.quarkkingdee.top/gtsrfhiuht.html

[U86] JS：空值合并
来源：http://hz.shzxlz.cn/gtdmynpxqx.html

a ?? b
来源：http://hz.feifeiyinyue.top/gtbmqagxwx.html

[U87] JS：解构默认值
来源：http://hz.hnxiangtu.top/gtzwcjmkxk.html

const { a = 1, b = 2 } = obj;
来源：http://hz.feifeiyinyue.top/gtpwilozxf.html

[U88] JS：对象展开合并
来源：http://hz.yanxiufei.cn/gtlaaobtgv.html

{ ...a, ...b }
来源：http://hz.redwolf501.top/gtpjznlkto.html

[U89] JS：数组去重
来源：http://hz.xuetiantiany.cn/gtiheooczr.html

[...new Set(arr)]
来源：http://hz.yvedp.cn/gtetqfpzvm.html

[U90] JS：数字数组排序
来源：http://hz.havefunace.top/gtmredvklj.html

[...arr].sort((a, b) => a - b)
来源：http://hz.hfpthk.cn/gtmtgidfgq.html

[U91] JS：对象键值遍历
来源：http://hz.zhongyouzk.top/gtcseddnqq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.zhixingplan.top/gtacuxvpuq.html

[U92] JS：深拷贝
来源：http://hz.yanxiufei.cn/gtpufgmfwp.html

structuredClone(obj)
来源：http://hz.xylfe.cn/gtavfxpkfg.html

[U93] JS：模板字符串
来源：http://hz.ppjwa.cn/gtjynaysxn.html

`共 ${n} 条`
来源：http://hz.zhongyouzk.top/gtfompysyl.html

[U94] JS：箭头函数
来源：http://hz.meibo888.top/gtxqotasig.html

const double = x => x * 2;
来源：http://hz.yongpay.top/gtmzbzaijn.html

[U95] JS：Promise 包装
来源：http://hz.0kj1m.cn/gtlfnmqgyj.html

new Promise((resolve, reject) => {})
来源：http://hz.guannengcc.top/gtseyhrysj.html

[U96] JS：async/await 与异常
来源：http://hz.dashuyun.cn/gtvtfwqfiz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.dashuyun.cn/gtnjrjqqpz.html

[U97] JS：并发请求
来源：http://hz.bjfxy.top/gtudcdmonx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.wangdashe.top/gtaqyzjszx.html

[U98] JS：fetch 带 JSON
来源：http://hz.jlsjyb.cn/gtaxnbpxfv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.guowangkeji.top/gtwzbdtbpa.html

[U99] JS：事件监听
来源：http://hz.ywan-chungtsiang.top/gtpqqqfhfe.html

el.addEventListener("click", e => {})
来源：http://hz.gzhubu.top/gtcsrkvfzb.html

[U100] JS：DOM 查询
来源：http://hz.hysaishi.cn/gtetrtemcb.html

document.querySelector(".item")
来源：http://hz.ydjk.org.cn/gtpdascamp.html

[U101] JS：classList 操作
来源：http://hz.yanxiufei.cn/gtnrfmpeuw.html

el.classList.toggle("active")
来源：http://hz.ywan-chungtsiang.top/gtbliwbzzp.html

[U102] JS：本地存储
来源：http://hz.shuidangran.top/gtufmzvsml.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.chenlongwang.top/gtbqarnqul.html

[U103] JS：定时器
来源：http://hz.ywan-chungtsiang.top/gtvqpcaqzs.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.zhaomingkeji.xyz/gtjkqttbxq.html

[U104] JS：防抖
来源：http://hz.cheryme.top/gtvnseffbj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jlsjyb.cn/gtpxhkhpws.html

[U105] JS：节流
来源：http://hz.dashuyun.cn/gtudgyfuau.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.yj20258888.top/gtwxxiyllp.html

[U106] JS：日期格式化
来源：http://hz.quarkkingdee.top/gtvwnpqsii.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.ydzc1.top/gtwvzsctoe.html

[U107] JS：数字千分位
来源：http://hz.gaohongyu789.top/gtmfqbbdqn.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.hnxiangtu.top/gtndjbzsby.html

[U108] JS：随机整数
来源：http://hz.zhijiandao.cn/gtolhflkjd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.guowangkeji.top/gtdpleooyx.html

[U109] JS：数组分组
来源：http://hz.pycfn.com/gtnhcaxnmq.html

Object.groupBy(arr, x => x.type)
来源：http://hz.kuanghao11.cn/gthckwtoxq.html

[U110] JS：数组分块
来源：http://hz.cdnleiting.top/gtfpbeyeej.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.feifeiyinyue.top/gtslsaegqn.html

[U111] JS：对象转 Map
来源：http://hz.jianghu66.top/gtaytansld.html

new Map(Object.entries(obj))
来源：http://hz.svipenyu.cn/gtbebgofmz.html

[U112] JS：字符串补位
来源：http://hz.yonumen.top/gtpnumtkcq.html

"7".padStart(3, "0")
来源：http://hz.zycfv.cn/gtqiosdaxg.html

[U113] JS：正则替换全部
来源：http://hz.ybcxt.top/gtqcvjphnq.html

s.replaceAll("a", "b")
来源：http://hz.wangshuangyany.cn/gtvffayjwd.html

[U114] JS：JSON 深比较
来源：http://hz.zhijiandao.cn/gtvimsvgre.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hammf.cn/gthowflvty.html

[U115] JS：生成 UUID
来源：http://hz.0kj1m.cn/gthscofchw.html

crypto.randomUUID()
来源：http://hz.yongpay.top/gtneypkxzv.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.shangyingyoupin.top/gtvvamncfg.html

/** @param {string} name */ function f(name) {}
来源：http://hz.yj20258888.top/gtlzqkykqf.html

[U117] JS：单元测试
来源：http://hz.cdnleiting.top/gtckdqmkaw.html

npm i -D vitest;  npx vitest
来源：http://hz.chenlongwang.top/gtzlftcjmd.html

[U118] JS：开发服务器
来源：http://hz.jyoumei.cn/gtmzuilbxe.html

npm i -D vite;  npx vite
来源：http://hz.cashguo.top/gtcalbiwaj.html

[U119] JS：生产构建
来源：http://hz.quarkkingdee.top/gtozlifyat.html

npx vite build
来源：http://hz.jianghu66.top/gtpjivguzb.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.shangyingyoupin.top/gtpvdazuok.html

import.meta.env.VITE_API_URL
来源：http://hz.hammf.cn/gtzsdyxgzb.html

================================================================================
来源：http://hz.0kj1m.cn/gtabnpxttk.html

统计汇总
来源：http://hz.smart0.xyz/gtrlslzrav.html

================================================================================
来源：http://hz.snrcjt.cn/gtcjyrmfll.html

按语言统计（条）：
来源：http://hz.ppjwa.cn/gthvizkhiv.html

Python ......... 252
来源：http://hz.yanxiufei.cn/gttqratkqj.html

PHP ............ 252
来源：http://hz.jlsjyb.cn/gtqgeoaivy.html

JavaScript ..... 252
来源：http://hz.daria6918.cn/gtpkjbyfhz.html

TypeScript ..... 212
来源：http://hz.pycfn.com/gtcjyrixrk.html

Java ........... 212
来源：http://hz.aibaodan.cn/gtckbakucz.html

Go ............. 212
来源：http://hz.jinqigufen.top/gtigpreviz.html

Ruby ........... 212
来源：http://hz.ywan-chungtsiang.top/gtnyitfxsr.html

C# ............. 212
来源：http://hz.aizwys.cn/gtifijfkup.html

C .............. 30
来源：http://hz.andypj.xyz/gtpuisoyqh.html

C++ ............ 30
来源：http://hz.shanyushiyangkeji.top/gtjqgrzvsc.html

SQL ............ 90
来源：http://hz.jinyuanbaomall.cn/gtrudscczy.html

Bash ........... 80
来源：http://hz.cheryme.top/gtnnhppuks.html

Kotlin ......... 15
来源：http://hz.nwbrower.top/gtfnnwsrto.html

Swift .......... 15
来源：http://hz.andypj.xyz/gtoeoyrdsh.html

Lua ............ 10
来源：http://hz.zhaomingkeji.xyz/gtsnprsvkg.html

Perl ........... 10
来源：http://hz.hongshengwenyu.top/gtsakhugaj.html

Scala .......... 10
来源：http://hz.shangyingyoupin.top/gtrrtsvxtx.html

------------------------------------
来源：http://hz.cashguo.top/gtzvzetmno.html

合计 ........... 2106 条
来源：http://hz.yj20258.top/gtipgexfpb.html

按章节统计：
来源：http://hz.shzxlz.cn/gtwnlkpueh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.jinyuanbaomall.cn/gtayqongns.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.aizwys.cn/gtjeahleai.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.guannengcc.top/gtzscyjbsi.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.yj202588.top/gthmsqjqzl.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.zhaomingkeji.xyz/gtzitwznyr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.dianchejie.cn/gtcrskecex.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.hammf.cn/gtmstybkka.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.yj20258.top/gtylkvmjiu.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.xingfuxueyuan.xyz/gtlqmmybvf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.zhijiandao.cn/gtgfjvqqrf.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.zhaomingkeji.xyz/gtqcvuojub.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.meibo888.top/gtvdntesbp.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.wangdashe.top/gtuenbvntq.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.cqqwz.cn/gtvclwyawv.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.kuanghao11.cn/gtoapmdzfk.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.andypj.xyz/gtoykmzrzy.html

Q SQL 专题                              90
来源：http://hz.wangdashe.top/gthvnstwce.html

R Bash 专题                             80
来源：http://hz.hysaishi.cn/gtxivovizl.html

S C / C++ 专题                          60
来源：http://hz.guannengcc.top/gteothhjou.html

T 其他语言补充                          60
来源：http://hz.cdnleiting.top/gtbyjayhdk.html

U 高频实用片段                         120
来源：http://hz.9152youxi.cn/gtvnwaaqht.html

------------------------------------
来源：http://hz.chenzaomai.com/gtogrhogkk.html

合计                                  2106 条
来源：http://hz.nanxinkj.top/gtqbulmzja.html

--------------------------------------------------------------------------------
来源：http://hz.jyoumei.cn/gtkzektrny.html

使用提醒
来源：http://hz.zhengqikj.top/gtmufhyhaf.html

--------------------------------------------------------------------------------
来源：http://hz.yuanzhike.top/gtxtfhnhnq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.zycfv.cn/gtxbaauetm.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.mhx1999.top/gtreexcvci.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.xuanzx.com/gtstdjpwet.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.jyoumei.cn/gtzqsjwrfs.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.52xcode.cn/gtriqgplnp.html

—— 文件结束 ——
来源：http://hz.jiagoushi.top/gtszpruizg.html

================================================================================
来源：http://hz.shzxlz.cn/gtajmczcrm.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.jinghuilouyu.cn/gtbqwvrpxt.html

Common Programming Examples Cheat Book
来源：http://hz.yvedp.cn/gtbeitsjcy.html

================================================================================
来源：http://hz.meibo888.top/gtcylyakfd.html

【收录内容】
来源：http://hz.dianchejie.cn/gtwuuyobgd.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.quarkkingdee.top/gtwgvfyhyu.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.daxiang520.top/gttpkhhrfu.html

SQL · Bash · C · C++
来源：http://hz.fzhhl.top/gtgwxtjbwd.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.andypj.xyz/gtphddmlql.html

【使用说明】
来源：http://hz.aibaodan.cn/gtexxjaxhh.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.yanxiufei.cn/gtflqttvga.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.yvedp.cn/gtidjtdhri.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.havefunace.top/gtfmpnuyie.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.aibaodan.cn/gtibuiadfk.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.wangshuangyany.cn/gtjcszfwcl.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.tianlin.xyz/gtpcwumlin.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.tian-w.cn/gtbpxaoxxm.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.yj202588.top/gtaiimvrdy.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.smart0.xyz/gtobxumuva.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.zhaomingkeji.xyz/gtsncnmcza.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.ydzc1.top/gttculvdzi.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.redwolf501.top/gtsodhdlwk.html

【文件统计】
来源：http://hz.gzhubu.top/gtthfzhrfj.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.zhoulong.xyz/gtmcoswhec.html

--------------------------------------------------------------------------------
来源：http://hz.pengpengdd.cyou/gtfnbgtjqe.html

目  录
来源：http://hz.xziqi.cn/gtsnayrqjq.html

--------------------------------------------------------------------------------
来源：http://hz.xuetiantiany.cn/gtrbhrxhxy.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.ehwqpu.com/gtmecwjlnl.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.yongpay.top/gtqlgxgxyp.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.xinyue.icu/gtmyovwxak.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.sufxvd.cn/gtqnhttjfy.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.jlsjyb.cn/gtzmghcual.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.hnxiangtu.top/gtjablzwsb.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.yonumen.top/gtlxqlgoqq.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.xingfuxueyuan.xyz/gttjjlylek.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.0kj1m.cn/gtwddmhtrs.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.9152youxi.cn/gteedipljh.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.yueranfly.top/gtgldwaqfb.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.andypj.xyz/gtfyisukbx.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.xuetiantiany.cn/gtlinkhvah.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.52xcode.cn/gterytgoli.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.pycfn.com/gtmqyjbhis.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.gaohongyu789.top/gtltsttiqc.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.wangshuangyany.cn/gtsywhposx.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.jinqigfzy.top/gtyvayueqf.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.nanxuanxn.top/gtbaavfdjj.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ivvv.top/gttgjezwld.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.aibaodan.cn/gtlfmxtlzv.html

================================================================================
来源：http://hz.nanxuanxn.top/gtnpiodtmo.html

A. 基础语法与类型
来源：http://hz.zhijiandao.cn/gtusxipxld.html

================================================================================
来源：http://hz.nanxuanxn.top/gtelipwypg.html

[A01] Hello World
来源：http://hz.haohaochexian.top/gtfhuawigw.html

Py:   print("Hello, World!")
来源：http://hz.yongpay.top/gtphjdlasx.html

PHP:  echo "Hello, World!";
来源：http://hz.zhijiandao.cn/gtuapzzzha.html

JS:   console.log("Hello, World!");
来源：http://hz.cheryme.top/gtrkaxyyvw.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.daria6918.cn/gtsvvtgblv.html

Java: System.out.println("Hello, World!");
来源：http://hz.9152youxi.cn/gtowfiesdq.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.sysykeji.top/gtivewmvvm.html

Ruby: puts "Hello, World!"
来源：http://hz.vqdsnc.cn/gtvpdamogm.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.xinyue.icu/gtikvfslok.html

[A02] 变量声明与赋值
来源：http://hz.tian-w.cn/gtdsyyxbup.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.316326.xyz/gtehliiovj.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.smart0.xyz/gtysjngdur.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.tian-w.cn/gthwyfzmru.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.cucudq.cn/gtvnvrbmdb.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.iojbl.cn/gtdznakolf.html

Go:   name := "Alex"; age := 20
来源：http://hz.hysaishi.cn/gthcyuqufb.html

Ruby: name = "Alex"; age = 20
来源：http://hz.mhx1999.top/gtnzlyught.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.hfpthk.cn/gtlkascmqn.html

[A03] 常量定义
来源：http://hz.xziqi.cn/gtgbjbrdiy.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.ydjk.org.cn/gtmzknidlu.html

PHP:  const PI = 3.14159;
来源：http://hz.zhongyouzk.top/gtyumqoktm.html

JS:   const PI = 3.14159;
来源：http://hz.zhijiandao.cn/gticobgwiq.html

TS:   const PI: number = 3.14159;
来源：http://hz.shangyingyoupin.top/gtbepasbih.html

Java: static final double PI = 3.14159;
来源：http://hz.smart0.xyz/gtzfibehhl.html

Go:   const PI = 3.14159
来源：http://hz.yuxming.cn/gtxevtfpqp.html

Ruby: PI = 3.14159
来源：http://hz.ivvv.top/gtvihhfsut.html

C#:   const double PI = 3.14159;
来源：http://hz.chenlongwang.top/gtwusklblr.html

[A04] 判断变量类型
来源：http://hz.yuxming.cn/gtnfobjvzd.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.andypj.xyz/gtcraetexq.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.pengpengdd.cyou/gtypcxrruh.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.tian-w.cn/gtfacbgdeq.html

TS:   typeof x; x instanceof Date
来源：http://hz.chenzaomai.com/gtzqkolqjc.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.sweek.top/gtacqvwgpp.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.pengpengdd.cyou/gtelesoxlk.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.guowangkeji.top/gtrlzhbylq.html

C#:   x.GetType().Name; x is int
来源：http://hz.0kj1m.cn/gtzjlvvrlf.html

[A05] 整数除法与取模
来源：http://hz.zhaomingkeji.xyz/gtufyffbya.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.zhijiandao.cn/gtcwgodbru.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.0kj1m.cn/gtxdsmhxqs.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.ppjwa.cn/gtcnyccpjp.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.zdqjudy.top/gtouautvgx.html

Java: 7 / 2; 7 % 2
来源：http://hz.ivvv.top/gtiquqjpzc.html

Go:   7 / 2; 7 % 2
来源：http://hz.nwbrower.top/gtmoyufcgk.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.vqdsnc.cn/gtukdsqgkt.html

C#:   7 / 2; 7 % 2
来源：http://hz.ppjwa.cn/gtaopmuypt.html

[A06] 字符串转数字
来源：http://hz.havefunace.top/gtuktndgyv.html

Py:   int("42"); float("3.14")
来源：http://hz.chenlongwang.top/gtjxskndym.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.wangdashe.top/gtyesewojk.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.gogol.net.cn/gtpoxflasx.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.cdnleiting.top/gtymwodase.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.shanyushiyangtech.top/gtoquyorie.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.dashuyun.cn/gtqqclvhnk.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.wangdashe.top/gtfsvdimsj.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.hongshengwenyu.top/gtkmhwrctd.html

[A07] 数字转字符串
来源：http://hz.chenjidiqi.icu/gtnmsuxpdt.html

Py:   str(42)
来源：http://hz.yanxiufei.cn/gtxfnlwgvn.html

PHP:  (string) 42; strval(42)
来源：http://hz.daria6918.cn/gttjerpics.html


<!-- 参考信息 -->