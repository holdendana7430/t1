代发 wailian999

[U61] PHP：正则
来源：http://hz.kuanghao11.cn/gtoxdsrrlo.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.jqgfzy.top/gtulepwnyi.html

[U62] PHP：日期对象
来源：http://hz.pengpengdd.cyou/gtykbekozt.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.yuanzhike.top/gtamejkqme.html

[U63] PHP：文件读写
来源：http://hz.bjfxy.top/gtakpqkbvr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.zhoulong.xyz/gtzwsynytm.html

[U64] PHP：目录遍历
来源：http://hz.zhengqikj.top/gtlxavrzxu.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.gogol.net.cn/gtgupsumgs.html

[U65] PHP：会话
来源：http://hz.shzxlz.cn/gtoytfepdh.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.jyoumei.cn/gtnqvtposp.html

[U66] PHP：设置 Cookie
来源：http://hz.zhaomingkeji.xyz/gtmkyaedci.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.iojbl.cn/gtlmwvmvnz.html

[U67] PHP：处理文件上传
来源：http://hz.jinghuilouyu.cn/gtqilazmxy.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.wangshuangyany.cn/gtcawlktfe.html

[U68] PHP：PDO 连接
来源：http://hz.pengpengdd.cyou/gtefwjxoli.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.zhengqikj.top/gtwfmqvwlz.html

[U69] PHP：PDO 预处理
来源：http://hz.ydzc1.top/gtsiwobpvk.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.gaohongyu789.top/gtezjfixbb.html

[U70] PHP：PDO 事务
来源：http://hz.fzhhl.top/gtvbyyvmnq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.jyoumei.cn/gtzmdcslyj.html

[U71] PHP：抛出异常
来源：http://hz.xingfuxueyuan.xyz/gtfrjwaqmy.html

throw new RuntimeException("失败", 500);
来源：http://hz.zdqjudy.top/gtcbkazyln.html

[U72] PHP：写错误日志
来源：http://hz.cheryme.top/gtgkeqmyto.html

error_log("失败: " . $e->getMessage());
来源：http://hz.gogol.net.cn/gtylkecetv.html

[U73] PHP：读取 ini 配置
来源：http://hz.hywenlv.cn/gthmwmiiav.html

parse_ini_file("config.ini", true)
来源：http://hz.cucudq.cn/gtvtxgedcx.html

[U74] PHP：读取环境变量
来源：http://hz.ydzc1.top/gtgawzmzjw.html

getenv("APP_ENV") ?: "production"
来源：http://hz.pengpengdd.cyou/gtvijkscgn.html

[U75] PHP：依赖注入
来源：http://hz.iojbl.cn/gtdtskmzlo.html

composer require psr/container
来源：http://hz.yueranfly.top/gtbyuggsqi.html

[U76] PHP：简单路由
来源：http://hz.hfpthk.cn/gtyvindzzo.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.gotoacloud.top/gttbvvslnj.html

[U77] PHP：模板渲染
来源：http://hz.havefunace.top/gtmtasblfa.html

composer require twig/twig
来源：http://hz.shzxlz.cn/gtexrwugur.html

[U78] PHP：单元测试
来源：http://hz.meibo888.top/gtigsyarpm.html

composer require --dev phpunit/phpunit
来源：http://hz.guowangkeji.top/gtizslplsn.html

[U79] PHP：静态分析
来源：http://hz.ywan-chungtsiang.top/gtvsvofbjc.html

composer require --dev phpstan/phpstan
来源：http://hz.yonumen.top/gtpllgdvyx.html

[U80] PHP：代码规范修复
来源：http://hz.nwbrower.top/gteugtebpw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.cashguo.top/gtzkdjehpf.html

[U81] JS：初始化项目
来源：http://hz.sxryk.cn/gtpmmczrsz.html

npm init -y;  npm i express
来源：http://hz.dashuyun.cn/gtatifzgdb.html

[U82] JS：package.json 脚本
来源：http://hz.ywan-chungtsiang.top/gtncqawtho.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.shangyingyoupin.top/gtjsvpnesj.html

[U83] JS：ES Module 导入导出
来源：http://hz.zycfv.cn/gtlxdjpzha.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.52xcode.cn/gtxberdbim.html

[U84] JS：CommonJS 写法
来源：http://hz.shanyushiyangkeji.top/gtauaqvbem.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.zycfv.cn/gtuyqudigp.html

[U85] JS：可选链
来源：http://hz.yueranfly.top/gtzoatxfja.html

a?.b?.c
来源：http://hz.cqqwz.cn/gtsnxxepsz.html

[U86] JS：空值合并
来源：http://hz.shzxlz.cn/gtmttouxhy.html

a ?? b
来源：http://hz.ppjwa.cn/gtncrncfzw.html

[U87] JS：解构默认值
来源：http://hz.hfpthk.cn/gtjlkeuxlm.html

const { a = 1, b = 2 } = obj;
来源：http://hz.jqgfzy.top/gtypsbshhw.html

[U88] JS：对象展开合并
来源：http://hz.yj20258.top/gtabksiflp.html

{ ...a, ...b }
来源：http://hz.jinghuilouyu.cn/gtgflknuzb.html

[U89] JS：数组去重
来源：http://hz.9152youxi.cn/gtuoralvjl.html

[...new Set(arr)]
来源：http://hz.yuanzhike.top/gtecgyyqan.html

[U90] JS：数字数组排序
来源：http://hz.c1oappe.top/gtadsnaxtv.html

[...arr].sort((a, b) => a - b)
来源：http://hz.yongpay.top/gtfomhoynd.html

[U91] JS：对象键值遍历
来源：http://hz.shanyushiyangtech.top/gtdayrbdkh.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.guannengcc.top/gtvdwgbqyt.html

[U92] JS：深拷贝
来源：http://hz.ehwqpu.com/gtrymfydxt.html

structuredClone(obj)
来源：http://hz.hammf.cn/gttfvtoopx.html

[U93] JS：模板字符串
来源：http://hz.ehwqpu.com/gtvrfuirgk.html

`共 ${n} 条`
来源：http://hz.chenlongwang.top/gtavwvccas.html

[U94] JS：箭头函数
来源：http://hz.xingfuxueyuan.xyz/gtndmytarb.html

const double = x => x * 2;
来源：http://hz.jinyuanbaomall.cn/gtrngsijqr.html

[U95] JS：Promise 包装
来源：http://hz.feifeiyinyue.top/gtxccufovj.html

new Promise((resolve, reject) => {})
来源：http://hz.daria6918.cn/gtqixdktru.html

[U96] JS：async/await 与异常
来源：http://hz.zhongyouzk.top/gtevsvvgsc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.ybcxt.top/gtgqombcme.html

[U97] JS：并发请求
来源：http://hz.tian-w.cn/gtflzniygh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.svipenyu.cn/gtdxaamvxe.html

[U98] JS：fetch 带 JSON
来源：http://hz.zhixingplan.top/gthybrdnep.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.meibo888.top/gtvmnxdijd.html

[U99] JS：事件监听
来源：http://hz.jinghuilouyu.cn/gtowntzckq.html

el.addEventListener("click", e => {})
来源：http://hz.dashuyun.cn/gtwlacnelw.html

[U100] JS：DOM 查询
来源：http://hz.cdnleiting.top/gtsshegkza.html

document.querySelector(".item")
来源：http://hz.shuidangran.top/gtnzzhjogs.html

[U101] JS：classList 操作
来源：http://hz.yuanzhike.top/gtqumzdkoa.html

el.classList.toggle("active")
来源：http://hz.zhoulong.xyz/gtchagoouk.html

[U102] JS：本地存储
来源：http://hz.ivvv.top/gtydjmgyid.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.shanyushiyangtech.top/gtuxocpxik.html

[U103] JS：定时器
来源：http://hz.cdnleiting.top/gtcarshpgo.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.zhengqikj.top/gttogvmylz.html

[U104] JS：防抖
来源：http://hz.iojbl.cn/gtscgqvyyo.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gzhubu.top/gtddvpawub.html

[U105] JS：节流
来源：http://hz.zhoulong.xyz/gtltvxsebo.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.andypj.xyz/gtfnumatwg.html

[U106] JS：日期格式化
来源：http://hz.ydzc1.top/gtqfnogykh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.zhiwuduotai.top/gtipadxmwt.html

[U107] JS：数字千分位
来源：http://hz.havefunace.top/gtlsbpryng.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.cucudq.cn/gtvgliszlp.html

[U108] JS：随机整数
来源：http://hz.9152youxi.cn/gtfrfdsxnq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.shanyushiyangtech.top/gtttwofzjr.html

[U109] JS：数组分组
来源：http://hz.meibo888.top/gtgfoydeeo.html

Object.groupBy(arr, x => x.type)
来源：http://hz.jinqigfzy.top/gtogfikopg.html

[U110] JS：数组分块
来源：http://hz.yanxiufei.cn/gtupiigide.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.ydzc1.top/gtuqbmoeik.html

[U111] JS：对象转 Map
来源：http://hz.9152youxi.cn/gtceyefdis.html

new Map(Object.entries(obj))
来源：http://hz.cheryme.top/gtenfaojuz.html

[U112] JS：字符串补位
来源：http://hz.zhixingplan.top/gtjcmntwdb.html

"7".padStart(3, "0")
来源：http://hz.yj20258.top/gtimsgoqow.html

[U113] JS：正则替换全部
来源：http://hz.tianlin.xyz/gtiywfjgaq.html

s.replaceAll("a", "b")
来源：http://hz.sweek.top/gtoccsawpt.html

[U114] JS：JSON 深比较
来源：http://hz.meibo888.top/gtxttegxbl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.smart0.xyz/gtdlbbmalp.html

[U115] JS：生成 UUID
来源：http://hz.zhengqikj.top/gtellqyyua.html

crypto.randomUUID()
来源：http://hz.jianghu66.top/gtdpogfvax.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.bjfxy.top/gthcekonir.html

/** @param {string} name */ function f(name) {}
来源：http://hz.gzhubu.top/gtozjgrmgm.html

[U117] JS：单元测试
来源：http://hz.shanyushiyangkeji.top/gtcosuozyn.html

npm i -D vitest;  npx vitest
来源：http://hz.birdmap.top/gtnnssrbrh.html

[U118] JS：开发服务器
来源：http://hz.guowangkeji.top/gthzeswnhj.html

npm i -D vite;  npx vite
来源：http://hz.chenlongwang.top/gtacwhlnzt.html

[U119] JS：生产构建
来源：http://hz.gzhubu.top/gtewowrohy.html

npx vite build
来源：http://hz.hnqzz.top/gtcmzrqshm.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.sxryk.cn/gtjsqyhjvy.html

import.meta.env.VITE_API_URL
来源：http://hz.zhixingplan.top/gtzoyptudw.html

================================================================================
来源：http://hz.zhoulong.xyz/gthnvbdprf.html

统计汇总
来源：http://hz.hywenlv.cn/gtiuecjlmy.html

================================================================================
来源：http://hz.jinqigufen.top/gtplxgfias.html

按语言统计（条）：
来源：http://hz.shangyingyoupin.top/gtnnjmmooc.html

Python ......... 252
来源：http://hz.cheryme.top/gtwlxuojyz.html

PHP ............ 252
来源：http://hz.xuetiantiany.cn/gtanisyuji.html

JavaScript ..... 252
来源：http://hz.ehwqpu.com/gtemlksrxq.html

TypeScript ..... 212
来源：http://hz.ydzc1.top/gtomzsgwkf.html

Java ........... 212
来源：http://hz.gzhubu.top/gtimpziedv.html

Go ............. 212
来源：http://hz.daxiang520.top/gtoflhngwh.html

Ruby ........... 212
来源：http://hz.birdmap.top/gtbvqvepsy.html

C# ............. 212
来源：http://hz.gotoacloud.top/gtaomotibj.html

C .............. 30
来源：http://hz.gzhubu.top/gtjtyuitip.html

C++ ............ 30
来源：http://hz.redwolf501.top/gtfqxqqllp.html

SQL ............ 90
来源：http://hz.snrcjt.cn/gtliuaqkio.html

Bash ........... 80
来源：http://hz.andypj.xyz/gtkctkkgrr.html

Kotlin ......... 15
来源：http://hz.redwolf501.top/gtgjdripxp.html

Swift .......... 15
来源：http://hz.xylfe.cn/gtwsetnsyh.html

Lua ............ 10
来源：http://hz.chenjidiqi.icu/gttnbljhnq.html

Perl ........... 10
来源：http://hz.yvedp.cn/gtlpochqdk.html

Scala .......... 10
来源：http://hz.zhengqikj.top/gtgswwocyd.html

------------------------------------
来源：http://hz.zycfv.cn/gticpiiudn.html

合计 ........... 2106 条
来源：http://hz.quarkkingdee.top/gtyxzwcgrc.html

按章节统计：
来源：http://hz.zdqjudy.top/gtlomjdrlv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.ivvv.top/gtdoeuxvfz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.haohaochexian.top/gttjtyfcwn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.hywenlv.cn/gtyjgcenay.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.jiagoushi.top/gtfuihegzf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.jinyuanbaomall.cn/gtxnedukmt.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.c1oappe.top/gtyxwewejj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.gaohongyu789.top/gtzpizglih.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.shangyingyoupin.top/gtbrhrqira.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.yueranfly.top/gtoeeqvfnk.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.zycfv.cn/gtocdvpzuk.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.jinqigufen.top/gtoqsrassa.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.shzxlz.cn/gtfrytnezp.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.aizwys.cn/gthwzedswg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.snrcjt.cn/gtvzhuqxul.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.shzxlz.cn/gtqhflgghe.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.snrcjt.cn/gtieqnaudj.html

Q SQL 专题                              90
来源：http://hz.aizwys.cn/gtkaerhuhh.html

R Bash 专题                             80
来源：http://hz.daria6918.cn/gtjvvlwymt.html

S C / C++ 专题                          60
来源：http://hz.xziqi.cn/gtctyffces.html

T 其他语言补充                          60
来源：http://hz.cucudq.cn/gtarmezakt.html

U 高频实用片段                         120
来源：http://hz.yanxiufei.cn/gtmzawlfcc.html

------------------------------------
来源：http://hz.zhengqikj.top/gtzoawwqtt.html

合计                                  2106 条
来源：http://hz.shzxlz.cn/gtpzlavqde.html

--------------------------------------------------------------------------------
来源：http://hz.xuanzx.com/gtphxjijdv.html

使用提醒
来源：http://hz.cashguo.top/gtzcjgciwc.html

--------------------------------------------------------------------------------
来源：http://hz.gotoacloud.top/gtnycsfxxh.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.zhixingplan.top/gtlgixqtjw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.jinghuilouyu.cn/gtwpytpdzr.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.nanxinkj.top/gtkkancdet.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.sxryk.cn/gtucrbzzxi.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.haohaochexian.top/gttqbalykp.html

—— 文件结束 ——
来源：http://hz.redwolf501.top/gtkcoqshtq.html

================================================================================
来源：http://hz.yj20258888.top/gtirgxradt.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.ywan-chungtsiang.top/gtlayjoebk.html

Common Programming Examples Cheat Book
来源：http://hz.zhoulong.xyz/gtwcjiwluu.html

================================================================================
来源：http://hz.gzhubu.top/gtomlmoniz.html

【收录内容】
来源：http://hz.sufxvd.cn/gtdhqvqqbh.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.fengsongda.top/gtqiyhgusd.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.fengsongda.top/gtrfinthli.html

SQL · Bash · C · C++
来源：http://hz.sweek.top/gtthjohkfc.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.xinyue.icu/gthhzdwpkr.html

【使用说明】
来源：http://hz.yueranfly.top/gtggwrlxwy.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.hammf.cn/gtmhfrmbpu.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.wangdashe.top/gtwsuxipkk.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.hnqzz.top/gtwnvcyfqa.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.wangshuangyany.cn/gtdzgaqevb.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.sxryk.cn/gtgpfcijlz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.shuidangran.top/gtqecfsvlb.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.hnxiangtu.top/gtugflvamy.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.pycfn.com/gtturyluly.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.kuanghao11.cn/gtuqblmuju.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.xylfe.cn/gtaviohyme.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.feifeiyinyue.top/gtfcsiqmqd.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.tanke756.top/gtkfdfktvy.html

【文件统计】
来源：http://hz.chenjidiqi.icu/gtfuschikj.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.zhengqikj.top/gtvrvjeysu.html

--------------------------------------------------------------------------------
来源：http://hz.jlsjyb.cn/gtkaxdaocm.html

目  录
来源：http://hz.cashguo.top/gttjnzvliw.html

--------------------------------------------------------------------------------
来源：http://hz.zhoulong.xyz/gtjiuatlqm.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.ydzc1.top/gtpyiraryf.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.havefunace.top/gtpdxmxejx.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.jlsjyb.cn/gtszebahzo.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.shangyingyoupin.top/gtcknzdkof.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.andypj.xyz/gtstmtspoj.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.ywan-chungtsiang.top/gtuhyasyma.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.havefunace.top/gtcchfxtyx.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.shanyushiyangtech.top/gtwvnzlaar.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.gzhubu.top/gtsnphghrg.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.smart0.xyz/gtwiwmsbgb.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.yj202588.top/gtbkjazhoa.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.zhengqikj.top/gthllmeenx.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.9152youxi.cn/gtuhrfcfmq.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.xylfe.cn/gttsylebsm.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.wangdashe.top/gtlkhwbdzl.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.shanyushiyangtech.top/gtqpnvxnpn.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.pengpengdd.cyou/gtrzkifpay.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.zhixingplan.top/gtjropxqfh.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.yanxiufei.cn/gthugelunu.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cheryme.top/gtmmmgpubk.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.hongshengwenyu.top/gtoejvnzyy.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gthjklvclc.html

A. 基础语法与类型
来源：http://hz.9152youxi.cn/gtkmgqagjf.html

================================================================================
来源：http://hz.yj20258888.top/gtskryvuti.html

[A01] Hello World
来源：http://hz.yuxming.cn/gtirlmuyth.html

Py:   print("Hello, World!")
来源：http://hz.shanyushiyangtech.top/gturfyakum.html

PHP:  echo "Hello, World!";
来源：http://hz.yj202588.top/gtpfgldavr.html

JS:   console.log("Hello, World!");
来源：http://hz.shanyushiyangtech.top/gtxpwjxcjo.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.jiagoushi.top/gtworxhpud.html

Java: System.out.println("Hello, World!");
来源：http://hz.cheryme.top/gtosezmaji.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.zhijiandao.cn/gtzkhsoosg.html

Ruby: puts "Hello, World!"
来源：http://hz.tian-w.cn/gtslkjxwdk.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.zhaomingkeji.xyz/gtlyznahmk.html

[A02] 变量声明与赋值
来源：http://hz.nanxinkj.top/gteysqfrct.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.sxryk.cn/gtbejtqakf.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.quarkkingdee.top/gtyxprwolc.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.9152youxi.cn/gtfnnkvzjs.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.guowangkeji.top/gtwckujewy.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.jlsjyb.cn/gtprdhfycx.html

Go:   name := "Alex"; age := 20
来源：http://hz.sufxvd.cn/gtcagjoqai.html

Ruby: name = "Alex"; age = 20
来源：http://hz.hongshengwenyu.top/gtqseplpki.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.yj20258.top/gtnrwqvxqu.html

[A03] 常量定义
来源：http://hz.fengsongda.top/gtwsqbqwlk.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.cucudq.cn/gtnrztgwhg.html

PHP:  const PI = 3.14159;
来源：http://hz.zhixingplan.top/gtyetvlvtz.html

JS:   const PI = 3.14159;
来源：http://hz.ybcxt.top/gtbjtopvjw.html

TS:   const PI: number = 3.14159;
来源：http://hz.dianchejie.cn/gtnovagfwi.html

Java: static final double PI = 3.14159;
来源：http://hz.daria6918.cn/gtmlthzfbq.html

Go:   const PI = 3.14159
来源：http://hz.yuxming.cn/gtfuidqgbl.html

Ruby: PI = 3.14159
来源：http://hz.guowangkeji.top/gtebxhxaky.html

C#:   const double PI = 3.14159;
来源：http://hz.chenzaomai.com/gtsjwtchsr.html

[A04] 判断变量类型
来源：http://hz.daria6918.cn/gthkepajsp.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.yvedp.cn/gtczfflupm.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.ydzc1.top/gtuxarjqrv.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.jqgfzy.top/gttkvpgufx.html

TS:   typeof x; x instanceof Date
来源：http://hz.andypj.xyz/gtarqjtzdg.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.ivvv.top/gtaflnckwd.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.gaohongyu789.top/gtloyjbuit.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.dianchejie.cn/gtnthrejsc.html

C#:   x.GetType().Name; x is int
来源：http://hz.ppjwa.cn/gtulyiphfi.html

[A05] 整数除法与取模
来源：http://hz.jlsjyb.cn/gtqqdpksst.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.yj20258888.top/gtunjzpydx.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.nanxuanxn.top/gtgenumeik.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.vqdsnc.cn/gtxggvrtak.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.aizwys.cn/gtkhneswqm.html

Java: 7 / 2; 7 % 2
来源：http://hz.yonumen.top/gtcdfjylbb.html

Go:   7 / 2; 7 % 2
来源：http://hz.cheryme.top/gtadazvirh.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.haohaochexian.top/gtrpffgcyg.html

C#:   7 / 2; 7 % 2
来源：http://hz.hywenlv.cn/gtmfjpywbh.html

[A06] 字符串转数字
来源：http://hz.zhiwuduotai.top/gtcdusxieu.html

Py:   int("42"); float("3.14")
来源：http://hz.shanyushiyangtech.top/gtasaswbdz.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.chenlongwang.top/gtmlboaubg.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.aibaodan.cn/gtkfwztwyn.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.svipenyu.cn/gthhkjdarw.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.ywan-chungtsiang.top/gtoupuurqb.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.xingfuxueyuan.xyz/gteatngybp.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.feifeiyinyue.top/gtxstmfrzn.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.yuanzhike.top/gtngjrswib.html

[A07] 数字转字符串
来源：http://hz.dianchejie.cn/gtwxdhikms.html

Py:   str(42)
来源：http://hz.yuanzhike.top/gtafwvjmvc.html

PHP:  (string) 42; strval(42)
来源：http://hz.sweek.top/gtpodfymnl.html

JS:   String(42); (42).toString()
来源：http://hz.hywenlv.cn/gtrijjrdgy.html

TS:   String(42)
来源：http://hz.vqdsnc.cn/gtdeapvpve.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.hfpthk.cn/gtcmfdiowd.html

Go:   strconv.Itoa(42)
来源：http://hz.wangshuangyany.cn/gtxqmrselp.html

Ruby: 42.to_s
来源：http://hz.iojbl.cn/gtpwwazqde.html

C#:   42.ToString()
来源：http://hz.cqqwz.cn/gtbenttgak.html

[A08] 取整与四舍五入
来源：http://hz.yanxiufei.cn/gthrjvtdkn.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.0kj1m.cn/gttpyryvrh.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.zhengqikj.top/gtnhgdwbco.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.yj20258.top/gtjcneozbp.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.zhengqikj.top/gttypreyjj.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.tianlin.xyz/gtqygkzynd.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.gzhubu.top/gtuyzhhgav.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.yueranfly.top/gtmszyfngi.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.tanke756.top/gtocfiecfm.html

[A09] 绝对值与最大最小值
来源：http://hz.hongshengwenyu.top/gtseuccoiy.html


<!-- 参考信息 -->