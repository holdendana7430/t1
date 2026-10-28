代发 wailian999

[U53] PHP：空合并运算符
来源：http://hz.ehwqpu.com/gtikwscpby.html

$v = $a ?? $b ?? "default";
来源：http://hz.cheryme.top/gtbamreezj.html

[U54] PHP：空安全调用
来源：http://hz.sysykeji.top/gthcnbgcit.html

$obj?->method()
来源：http://hz.cdnleiting.top/gtrfmnxsqv.html

[U55] PHP：match 表达式
来源：http://hz.yuanzhike.top/gtinjfiapz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.dianchejie.cn/gtulthqpuc.html

[U56] PHP：命名参数
来源：http://hz.zhongyouzk.top/gtaroezqlc.html

f(a: 1, b: 2)
来源：http://hz.quarkkingdee.top/gtekqgkbki.html

[U57] PHP：字符串插值
来源：http://hz.pycfn.com/gtphvxdizq.html

"值: {$a}"
来源：http://hz.jinyuanbaomall.cn/gtmhmmefau.html

[U58] PHP：数组三件套
来源：http://hz.xinyue.icu/gthwymycnc.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.yueranfly.top/gtkrumzotl.html

[U59] PHP：自定义排序
来源：http://hz.hnxiangtu.top/gtujaxjdhv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hysaishi.cn/gtothcdyap.html

[U60] PHP：JSON 编解码
来源：http://hz.0kj1m.cn/gtwrdappfp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.nwbrower.top/gttiwgcrvw.html

[U61] PHP：正则
来源：http://hz.gaohongyu789.top/gtrxxsqiit.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.yj20258.top/gtczmrznpa.html

[U62] PHP：日期对象
来源：http://hz.yongpay.top/gttlsxmdun.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.zhiwuduotai.top/gtyhprxtxk.html

[U63] PHP：文件读写
来源：http://hz.chenzaomai.com/gtylokogpz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.gogol.net.cn/gtrwuzmyje.html

[U64] PHP：目录遍历
来源：http://hz.0kj1m.cn/gtltusqlyh.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.bjfxy.top/gtndfbiewa.html

[U65] PHP：会话
来源：http://hz.gzhubu.top/gtcegddsih.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.yj202588.top/gthjqirnbo.html

[U66] PHP：设置 Cookie
来源：http://hz.jlsjyb.cn/gtdhyburwk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.yangfankeji.com/gttxrnflfc.html

[U67] PHP：处理文件上传
来源：http://hz.52xcode.cn/gthtarboyf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.chenzaomai.com/gtjknqmjev.html

[U68] PHP：PDO 连接
来源：http://hz.wangshuangyany.cn/gtcrlaeshi.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.guowangkeji.top/gtqnilsgws.html

[U69] PHP：PDO 预处理
来源：http://hz.shangyingyoupin.top/gtzavluvxy.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.quarkkingdee.top/gtchavpeut.html

[U70] PHP：PDO 事务
来源：http://hz.haohaochexian.top/gtlyzoepdt.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.vqdsnc.cn/gthjxzmyzz.html

[U71] PHP：抛出异常
来源：http://hz.redwolf501.top/gtqpuonqqm.html

throw new RuntimeException("失败", 500);
来源：http://hz.guannengcc.top/gtiacaofxi.html

[U72] PHP：写错误日志
来源：http://hz.pengpengdd.cyou/gtqmraskvk.html

error_log("失败: " . $e->getMessage());
来源：http://hz.zhixingplan.top/gtmqcakihi.html

[U73] PHP：读取 ini 配置
来源：http://hz.bjfxy.top/gtyrppwjdd.html

parse_ini_file("config.ini", true)
来源：http://hz.aizwys.cn/gtilivvcxo.html

[U74] PHP：读取环境变量
来源：http://hz.wangshuangyany.cn/gtfuysjvlj.html

getenv("APP_ENV") ?: "production"
来源：http://hz.aibaodan.cn/gtfdgjwutf.html

[U75] PHP：依赖注入
来源：http://hz.daxiang520.top/gtrvccycwd.html

composer require psr/container
来源：http://hz.chenzaomai.com/gtblitkmgg.html

[U76] PHP：简单路由
来源：http://hz.redwolf501.top/gtylcbtbku.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.zhijiandao.cn/gtcgqkbzxk.html

[U77] PHP：模板渲染
来源：http://hz.ehwqpu.com/gtbsxowycd.html

composer require twig/twig
来源：http://hz.dianchejie.cn/gtwkjevogj.html

[U78] PHP：单元测试
来源：http://hz.sweek.top/gtydcowbls.html

composer require --dev phpunit/phpunit
来源：http://hz.andypj.xyz/gttmttkkzo.html

[U79] PHP：静态分析
来源：http://hz.hywenlv.cn/gttfclxlah.html

composer require --dev phpstan/phpstan
来源：http://hz.aizwys.cn/gtxxtpfsrb.html

[U80] PHP：代码规范修复
来源：http://hz.shanyushiyangkeji.top/gtvajurwks.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.shzxlz.cn/gtmfzsayql.html

[U81] JS：初始化项目
来源：http://hz.aizwys.cn/gtklflnnrp.html

npm init -y;  npm i express
来源：http://hz.0kj1m.cn/gtuttrwcjw.html

[U82] JS：package.json 脚本
来源：http://hz.bjfxy.top/gtpnnlmzcy.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.xinyue.icu/gtwvnzcaqj.html

[U83] JS：ES Module 导入导出
来源：http://hz.9152youxi.cn/gtxipvsfna.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.tianlin.xyz/gtuvecnwqw.html

[U84] JS：CommonJS 写法
来源：http://hz.gzhubu.top/gtbqcpjswn.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.sufxvd.cn/gtdgesytlz.html

[U85] JS：可选链
来源：http://hz.xziqi.cn/gtsjiiengf.html

a?.b?.c
来源：http://hz.nanxuanxn.top/gthylazlfw.html

[U86] JS：空值合并
来源：http://hz.ybcxt.top/gtrcswsqpv.html

a ?? b
来源：http://hz.yangfankeji.com/gtlsbvjkjc.html

[U87] JS：解构默认值
来源：http://hz.c1oappe.top/gthfflrooe.html

const { a = 1, b = 2 } = obj;
来源：http://hz.xuanzx.com/gtvndohirt.html

[U88] JS：对象展开合并
来源：http://hz.kuanghao11.cn/gtbuvdnpdl.html

{ ...a, ...b }
来源：http://hz.gzhubu.top/gtftgfbtka.html

[U89] JS：数组去重
来源：http://hz.dashuyun.cn/gtyetgpxaa.html

[...new Set(arr)]
来源：http://hz.yangfankeji.com/gtmtzjpluj.html

[U90] JS：数字数组排序
来源：http://hz.zhongyouzk.top/gtvbctnuqw.html

[...arr].sort((a, b) => a - b)
来源：http://hz.hfpthk.cn/gtrgtkmlso.html

[U91] JS：对象键值遍历
来源：http://hz.0kj1m.cn/gtnsxkwixc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.ivvv.top/gtmkqqkfos.html

[U92] JS：深拷贝
来源：http://hz.yj202588.top/gtcguohllv.html

structuredClone(obj)
来源：http://hz.aibaodan.cn/gtxuodrlbe.html

[U93] JS：模板字符串
来源：http://hz.hywenlv.cn/gtlildrqzx.html

`共 ${n} 条`
来源：http://hz.zhaomingkeji.xyz/gtkmcgfonj.html

[U94] JS：箭头函数
来源：http://hz.jyoumei.cn/gtuzigfqry.html

const double = x => x * 2;
来源：http://hz.yj202588.top/gtvffzcdih.html

[U95] JS：Promise 包装
来源：http://hz.zdqjudy.top/gtozlxbdcu.html

new Promise((resolve, reject) => {})
来源：http://hz.zhaomingkeji.xyz/gtpzlqhafj.html

[U96] JS：async/await 与异常
来源：http://hz.ivvv.top/gtxzllntvn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.ppjwa.cn/gtolmktnnc.html

[U97] JS：并发请求
来源：http://hz.vqdsnc.cn/gtsioswhkw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.wangdashe.top/gtapieyewc.html

[U98] JS：fetch 带 JSON
来源：http://hz.andypj.xyz/gtlvtcoyzk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.pengpengdd.cyou/gtxnhcdnzt.html

[U99] JS：事件监听
来源：http://hz.yonumen.top/gtwlculvyl.html

el.addEventListener("click", e => {})
来源：http://hz.jqgfzy.top/gtthrjxzqb.html

[U100] JS：DOM 查询
来源：http://hz.gogol.net.cn/gtwdhazhoc.html

document.querySelector(".item")
来源：http://hz.xylfe.cn/gtzxwcszjn.html

[U101] JS：classList 操作
来源：http://hz.bjfxy.top/gtexmgyxxi.html

el.classList.toggle("active")
来源：http://hz.shzxlz.cn/gtywbxtzkw.html

[U102] JS：本地存储
来源：http://hz.vqdsnc.cn/gtlebwrzdg.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.zdqjudy.top/gtdqnlzrmr.html

[U103] JS：定时器
来源：http://hz.kuanghao11.cn/gtzojmptaz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.hongshengwenyu.top/gtuidezrsp.html

[U104] JS：防抖
来源：http://hz.zhixingplan.top/gtywxkvltk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.guowangkeji.top/gtntblvmkf.html

[U105] JS：节流
来源：http://hz.52xcode.cn/gtjejssvdh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.sweek.top/gtjhrfcyvw.html

[U106] JS：日期格式化
来源：http://hz.tian-w.cn/gturrwpadv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yuanzhike.top/gtodvvafsd.html

[U107] JS：数字千分位
来源：http://hz.zhiwuduotai.top/gtqbmpeabe.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.jiagoushi.top/gtuvsubaiy.html

[U108] JS：随机整数
来源：http://hz.hongshengwenyu.top/gtzxxzvaxf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.dianchejie.cn/gtyghkripj.html

[U109] JS：数组分组
来源：http://hz.chenzaomai.com/gtuyscjgee.html

Object.groupBy(arr, x => x.type)
来源：http://hz.tianlin.xyz/gteefywfzf.html

[U110] JS：数组分块
来源：http://hz.vqdsnc.cn/gtvnosihmg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.gogol.net.cn/gtqcrvwjbg.html

[U111] JS：对象转 Map
来源：http://hz.yanxiufei.cn/gtojiepcqj.html

new Map(Object.entries(obj))
来源：http://hz.pycfn.com/gtgcnxjaoz.html

[U112] JS：字符串补位
来源：http://hz.xingfuxueyuan.xyz/gttzgisdyo.html

"7".padStart(3, "0")
来源：http://hz.gaohongyu789.top/gtgqpquucn.html

[U113] JS：正则替换全部
来源：http://hz.wangdashe.top/gtdmkgttvd.html

s.replaceAll("a", "b")
来源：http://hz.jqgufenzy.top/gtpetfbjgr.html

[U114] JS：JSON 深比较
来源：http://hz.wangdashe.top/gtrkopgrxl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.haohaochexian.top/gtjsqzasga.html

[U115] JS：生成 UUID
来源：http://hz.daria6918.cn/gtmrgcbrwk.html

crypto.randomUUID()
来源：http://hz.dianchejie.cn/gtwhpavqwo.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.jinqigfzy.top/gtauknelns.html

/** @param {string} name */ function f(name) {}
来源：http://hz.zhoulong.xyz/gtmmcbvjim.html

[U117] JS：单元测试
来源：http://hz.tian-w.cn/gttjhlhtrl.html

npm i -D vitest;  npx vitest
来源：http://hz.snrcjt.cn/gtfnhcveeq.html

[U118] JS：开发服务器
来源：http://hz.xziqi.cn/gtnyofkmqp.html

npm i -D vite;  npx vite
来源：http://hz.fengsongda.top/gttevgpdqw.html

[U119] JS：生产构建
来源：http://hz.gotoacloud.top/gtbimbqgyz.html

npx vite build
来源：http://hz.cashguo.top/gtukqaajqn.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.ivvv.top/gtggdkoctg.html

import.meta.env.VITE_API_URL
来源：http://hz.sysykeji.top/gtafymyzqf.html

================================================================================
来源：http://hz.ybcxt.top/gtftpvlhrw.html

统计汇总
来源：http://hz.ivvv.top/gtsdhhuliw.html

================================================================================
来源：http://hz.meibo888.top/gtwuolyzsz.html

按语言统计（条）：
来源：http://hz.yonumen.top/gtnzuvfshb.html

Python ......... 252
来源：http://hz.guannengcc.top/gtlvtmnmpc.html

PHP ............ 252
来源：http://hz.sysykeji.top/gtsorgrxay.html

JavaScript ..... 252
来源：http://hz.svipenyu.cn/gtkmefycrc.html

TypeScript ..... 212
来源：http://hz.shanyushiyangkeji.top/gtxhzrwtdt.html

Java ........... 212
来源：http://hz.haohaochexian.top/gtspcqluyb.html

Go ............. 212
来源：http://hz.hammf.cn/gtayxjmenj.html

Ruby ........... 212
来源：http://hz.cqqwz.cn/gtxaerummv.html

C# ............. 212
来源：http://hz.pengpengdd.cyou/gtyhcynjjj.html

C .............. 30
来源：http://hz.sufxvd.cn/gtvigdfkbx.html

C++ ............ 30
来源：http://hz.zhixingplan.top/gtdfwqiipy.html

SQL ............ 90
来源：http://hz.hywenlv.cn/gtdfbclixk.html

Bash ........... 80
来源：http://hz.svipenyu.cn/gtvrcwwqcw.html

Kotlin ......... 15
来源：http://hz.mhx1999.top/gtwcizrnru.html

Swift .......... 15
来源：http://hz.fengsongda.top/gtpdagnfdm.html

Lua ............ 10
来源：http://hz.aizwys.cn/gtocalmxwk.html

Perl ........... 10
来源：http://hz.316326.xyz/gttszsxuav.html

Scala .......... 10
来源：http://hz.ywan-chungtsiang.top/gtbsotyocf.html

------------------------------------
来源：http://hz.gzhubu.top/gtwguafsvz.html

合计 ........... 2106 条
来源：http://hz.52xcode.cn/gthfixkfqt.html

按章节统计：
来源：http://hz.yongpay.top/gtnjsuvezs.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.yuxming.cn/gtvgmdvocl.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.hnxiangtu.top/gtpzadukfb.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.daxiang520.top/gtdxpcyigk.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.shzxlz.cn/gttzrvuzeq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.xinyue.icu/gtcfgulzmb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.c1oappe.top/gtnzgdygem.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.jinqigfzy.top/gtnwrnjvlc.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.cdnleiting.top/gtwdhtvrcy.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.guowangkeji.top/gtacimwaxt.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.hywenlv.cn/gtjmuxdkqd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.jianghu66.top/gtwprdivrl.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.havefunace.top/gtkdqtkeod.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.yj20258888.top/gtlkvuxssc.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.chenlongwang.top/gtdoyncyft.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.316326.xyz/gtlnkyjoxy.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.cqqwz.cn/gtoiranyno.html

Q SQL 专题                              90
来源：http://hz.yueranfly.top/gterzgbibs.html

R Bash 专题                             80
来源：http://hz.vqdsnc.cn/gttvxlgqrm.html

S C / C++ 专题                          60
来源：http://hz.jinyuanbaomall.cn/gtyyfucwgn.html

T 其他语言补充                          60
来源：http://hz.yueranfly.top/gtbhgmtrbx.html

U 高频实用片段                         120
来源：http://hz.ivvv.top/gtaixntqqz.html

------------------------------------
来源：http://hz.nwbrower.top/gtvwjopnwi.html

合计                                  2106 条
来源：http://hz.hongshengwenyu.top/gtqgblbhlj.html

--------------------------------------------------------------------------------
来源：http://hz.bjfxy.top/gtykjzwizz.html

使用提醒
来源：http://hz.jqgfzy.top/gtcrhdudrl.html

--------------------------------------------------------------------------------
来源：http://hz.fengsongda.top/gtkesqqzfm.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.zhiwuduotai.top/gtzfpdbnob.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.yueranfly.top/gtzagksugt.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.gzhubu.top/gtlvnmjrcg.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.havefunace.top/gtixphnmja.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.tanke756.top/gtpfvouley.html

—— 文件结束 ——
来源：http://hz.jyoumei.cn/gtnkatlsft.html

================================================================================
来源：http://hz.meibo888.top/gtudqbmupl.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.ywan-chungtsiang.top/gttohfuhal.html

Common Programming Examples Cheat Book
来源：http://hz.hnxiangtu.top/gtzauxumrt.html

================================================================================
来源：http://hz.jyoumei.cn/gtuogkmubs.html

【收录内容】
来源：http://hz.zhixingplan.top/gtrfzaixce.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.chenzaomai.com/gthosoujfq.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.yj20258.top/gtozehafsr.html

SQL · Bash · C · C++
来源：http://hz.andypj.xyz/gtbigsllkf.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.wangshuangyany.cn/gtaijfvasp.html

【使用说明】
来源：http://hz.shuidangran.top/gtqqvvehfs.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.zhijiandao.cn/gtppxoapin.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.jqgufenzy.top/gthriiiufy.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.snrcjt.cn/gtytdfrlsg.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.hammf.cn/gtcgwnsagn.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.gaohongyu789.top/gtynytjqra.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.wangshuangyany.cn/gtahlqqlrx.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.aizwys.cn/gtaqlqymqu.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.mhx1999.top/gtnzledscl.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.jianghu66.top/gttpqszyck.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.ivvv.top/gtdivmvkru.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.jinqigufen.top/gteibrksgo.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.kuanghao11.cn/gtdikpgiip.html

【文件统计】
来源：http://hz.kuanghao11.cn/gtlkhiubft.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.xylfe.cn/gtvhjedccj.html

--------------------------------------------------------------------------------
来源：http://hz.shuidangran.top/gtuceheyli.html

目  录
来源：http://hz.aibaodan.cn/gteuzgwhsw.html

--------------------------------------------------------------------------------
来源：http://hz.yuxming.cn/gtlmxntbld.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.kuanghao11.cn/gtfapofgiv.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.jinqigufen.top/gtauftenlo.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.yuxming.cn/gtrxxvvsai.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.shanyushiyangtech.top/gttkbpiktv.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.yj202588.top/gthklcvmst.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.iojbl.cn/gthumfumoz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.wangdashe.top/gtogjkxrhw.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.zhixingplan.top/gtjlxgcwef.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.yuanzhike.top/gtekbyguvr.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.wangshuangyany.cn/gtehpkaxbt.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.vqdsnc.cn/gtaqjhagpw.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.hysaishi.cn/gtzavflcah.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.cheryme.top/gtdcxwgbhj.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.mhx1999.top/gtwxdzoeoc.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.dianchejie.cn/gtetbbchig.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.sweek.top/gttdpncvxu.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.cqqwz.cn/gtwniczkjp.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.smart0.xyz/gteygievsl.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.haohaochexian.top/gtugsqyxdj.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.havefunace.top/gthwqmuiux.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.yvedp.cn/gtsyztenkh.html

================================================================================
来源：http://hz.xylfe.cn/gtvkaikpir.html

A. 基础语法与类型
来源：http://hz.316326.xyz/gtqfsrqhbc.html

================================================================================
来源：http://hz.smart0.xyz/gtrghhwzef.html

[A01] Hello World
来源：http://hz.gzhubu.top/gtmxryfsmd.html

Py:   print("Hello, World!")
来源：http://hz.jianghu66.top/gtayqicxvm.html

PHP:  echo "Hello, World!";
来源：http://hz.jinqigufen.top/gtqyvvjqen.html

JS:   console.log("Hello, World!");
来源：http://hz.zhengqikj.top/gtksyykckb.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.mhx1999.top/gtyrloatsw.html

Java: System.out.println("Hello, World!");
来源：http://hz.hywenlv.cn/gtbcoqctyc.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.yvedp.cn/gtwycbjbma.html

Ruby: puts "Hello, World!"
来源：http://hz.quarkkingdee.top/gtkxgvfhdf.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.zdqjudy.top/gttxhlusxc.html

[A02] 变量声明与赋值
来源：http://hz.gotoacloud.top/gtqugswlrq.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.shzxlz.cn/gtrcdaxdbh.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.zhixingplan.top/gtkutphmfu.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.zhongyouzk.top/gtgbvobvba.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.ydjk.org.cn/gtgetogtmy.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.hnqzz.top/gtibijnzsy.html

Go:   name := "Alex"; age := 20
来源：http://hz.nwbrower.top/gtbnxqdjew.html

Ruby: name = "Alex"; age = 20
来源：http://hz.gotoacloud.top/gtnyxpfttc.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.c1oappe.top/gtitsfowfr.html

[A03] 常量定义
来源：http://hz.iojbl.cn/gtnzxclbzp.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.xylfe.cn/gtylfviili.html

PHP:  const PI = 3.14159;
来源：http://hz.fengsongda.top/gtpkvtgbua.html

JS:   const PI = 3.14159;
来源：http://hz.sysykeji.top/gtbddfipcc.html

TS:   const PI: number = 3.14159;
来源：http://hz.vqdsnc.cn/gtqzuzbdla.html

Java: static final double PI = 3.14159;
来源：http://hz.yueranfly.top/gtfpgjrltx.html

Go:   const PI = 3.14159
来源：http://hz.birdmap.top/gtrekmlwkd.html

Ruby: PI = 3.14159
来源：http://hz.andypj.xyz/gttjxwixjh.html

C#:   const double PI = 3.14159;
来源：http://hz.sxryk.cn/gtavhlteuj.html

[A04] 判断变量类型
来源：http://hz.shuidangran.top/gtwoasdvei.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.sxryk.cn/gtlcxfbboc.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.mhx1999.top/gtcfdojoxn.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.yueranfly.top/gtkwmjmprz.html

TS:   typeof x; x instanceof Date
来源：http://hz.zhengqikj.top/gtjqwdslbj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.yueranfly.top/gtoympjxbv.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.feifeiyinyue.top/gtkuewxwck.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.nwbrower.top/gtqststalo.html

C#:   x.GetType().Name; x is int
来源：http://hz.xingfuxueyuan.xyz/gtdwrzqlid.html

[A05] 整数除法与取模
来源：http://hz.52xcode.cn/gtnbnfsxai.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.jiagoushi.top/gtmemdgztv.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.dianchejie.cn/gthlydgqrr.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.zhaomingkeji.xyz/gtcqgrdnrt.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.xingfuxueyuan.xyz/gtdgfkceau.html

Java: 7 / 2; 7 % 2
来源：http://hz.wangdashe.top/gtipsoelfv.html

Go:   7 / 2; 7 % 2
来源：http://hz.shanyushiyangkeji.top/gtyenelmdh.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.shangyingyoupin.top/gtsjevvvdc.html

C#:   7 / 2; 7 % 2
来源：http://hz.jqgfzy.top/gtstlnbonr.html

[A06] 字符串转数字
来源：http://hz.yuanzhike.top/gtoiemdgmk.html

Py:   int("42"); float("3.14")
来源：http://hz.zhongyouzk.top/gtajnvlzgj.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.yonumen.top/gtnroywqfj.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.ppjwa.cn/gtjgchtwmi.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.yongpay.top/gtmaolhfoq.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.316326.xyz/gtgwnmcicl.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.kuanghao11.cn/gtoatulhzc.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.sufxvd.cn/gtjpfpdhnl.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.zhoulong.xyz/gtirveidld.html

[A07] 数字转字符串
来源：http://hz.tian-w.cn/gtbgqowqzv.html

Py:   str(42)
来源：http://hz.ppjwa.cn/gtcwjybwvr.html

PHP:  (string) 42; strval(42)
来源：http://hz.svipenyu.cn/gtivvjnftt.html


<!-- 参考信息 -->