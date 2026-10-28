代发 wailian999

[U49] PHP：只读属性
来源：http://hz.tanke756.top/gtizktswqq.html

public readonly string $name
来源：http://hz.316326.xyz/gttopsliov.html

[U50] PHP：构造器属性提升
来源：http://hz.sufxvd.cn/gtrulwdeqj.html

public function __construct(private int $id) {}
来源：http://hz.yangfankeji.com/gtvlpvmmtc.html

[U51] PHP：数组解构
来源：http://hz.dianchejie.cn/gtpnggyxlq.html

[$a, $b] = $arr;
来源：http://hz.zhijiandao.cn/gtvnbgssog.html

[U52] PHP：箭头函数
来源：http://hz.daria6918.cn/gtgmlljczd.html

$double = fn($x) => $x * 2;
来源：http://hz.ydzc1.top/gtzzhoueli.html

[U53] PHP：空合并运算符
来源：http://hz.xinyue.icu/gtbfbwaxgz.html

$v = $a ?? $b ?? "default";
来源：http://hz.hongshengwenyu.top/gtchocnfjj.html

[U54] PHP：空安全调用
来源：http://hz.smart0.xyz/gtrokcqbpm.html

$obj?->method()
来源：http://hz.hongshengwenyu.top/gtcvojwfxj.html

[U55] PHP：match 表达式
来源：http://hz.fzhhl.top/gtrzxkmlzc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.cqqwz.cn/gtnagsorew.html

[U56] PHP：命名参数
来源：http://hz.aibaodan.cn/gtklqmxxqh.html

f(a: 1, b: 2)
来源：http://hz.fzhhl.top/gtdwgudvlb.html

[U57] PHP：字符串插值
来源：http://hz.yj202588.top/gtycyfbflq.html

"值: {$a}"
来源：http://hz.wangdashe.top/gtmlrsbbmg.html

[U58] PHP：数组三件套
来源：http://hz.aibaodan.cn/gtyrxycuab.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.yanxiufei.cn/gtqkqenwhp.html

[U59] PHP：自定义排序
来源：http://hz.aibaodan.cn/gtoqgvgabt.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cqqwz.cn/gtxkltsttq.html

[U60] PHP：JSON 编解码
来源：http://hz.nanxinkj.top/gtforqpltc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.pengpengdd.cyou/gtzeurtnxt.html

[U61] PHP：正则
来源：http://hz.gaohongyu789.top/gtrsgzcfxd.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.yonumen.top/gtartjogde.html

[U62] PHP：日期对象
来源：http://hz.zhaomingkeji.xyz/gtxpdwqkde.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.jiagoushi.top/gttrijcspi.html

[U63] PHP：文件读写
来源：http://hz.guowangkeji.top/gtslsqioxp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.9152youxi.cn/gtfjuqjghr.html

[U64] PHP：目录遍历
来源：http://hz.yongpay.top/gtegyyntjo.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.haohaochexian.top/gthntfttae.html

[U65] PHP：会话
来源：http://hz.nwbrower.top/gtmugaujnu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.chenjidiqi.icu/gtajxceueu.html

[U66] PHP：设置 Cookie
来源：http://hz.yonumen.top/gtxktfvnko.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.yj20258888.top/gttogqwxez.html

[U67] PHP：处理文件上传
来源：http://hz.hongshengwenyu.top/gtdqauunhk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.xuetiantiany.cn/gtpkfmhunw.html

[U68] PHP：PDO 连接
来源：http://hz.ppjwa.cn/gtonitjroo.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.jiagoushi.top/gtwporiipa.html

[U69] PHP：PDO 预处理
来源：http://hz.daria6918.cn/gtrwktbzvq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.yj20258888.top/gtbktymfnv.html

[U70] PHP：PDO 事务
来源：http://hz.sufxvd.cn/gtuklvsxsr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.hnxiangtu.top/gttkxtjzfd.html

[U71] PHP：抛出异常
来源：http://hz.guowangkeji.top/gtcrpshsca.html

throw new RuntimeException("失败", 500);
来源：http://hz.316326.xyz/gtlyqkgnww.html

[U72] PHP：写错误日志
来源：http://hz.jyoumei.cn/gtlrcstwnh.html

error_log("失败: " . $e->getMessage());
来源：http://hz.316326.xyz/gtqjoxnjgo.html

[U73] PHP：读取 ini 配置
来源：http://hz.ydzc1.top/gtqkpoqizk.html

parse_ini_file("config.ini", true)
来源：http://hz.zhixingplan.top/gtvwcxacct.html

[U74] PHP：读取环境变量
来源：http://hz.svipenyu.cn/gtcmjikxxy.html

getenv("APP_ENV") ?: "production"
来源：http://hz.gogol.net.cn/gtxdywnfrj.html

[U75] PHP：依赖注入
来源：http://hz.chenjidiqi.icu/gtgtgbrpba.html

composer require psr/container
来源：http://hz.wangshuangyany.cn/gtbarrsdxm.html

[U76] PHP：简单路由
来源：http://hz.zdqjudy.top/gtysaapcwb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.redwolf501.top/gtipmgomdw.html

[U77] PHP：模板渲染
来源：http://hz.hysaishi.cn/gtrynhkcgm.html

composer require twig/twig
来源：http://hz.c1oappe.top/gtxotljidk.html

[U78] PHP：单元测试
来源：http://hz.bjfxy.top/gtoflrnrir.html

composer require --dev phpunit/phpunit
来源：http://hz.shuidangran.top/gttkuevwjj.html

[U79] PHP：静态分析
来源：http://hz.gogol.net.cn/gtugrhxpcl.html

composer require --dev phpstan/phpstan
来源：http://hz.chenzaomai.com/gtlfjheniw.html

[U80] PHP：代码规范修复
来源：http://hz.guannengcc.top/gtglmjujix.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.cucudq.cn/gtbabtoqha.html

[U81] JS：初始化项目
来源：http://hz.aizwys.cn/gtdqsdjwxc.html

npm init -y;  npm i express
来源：http://hz.sufxvd.cn/gtdfzintoh.html

[U82] JS：package.json 脚本
来源：http://hz.shanyushiyangkeji.top/gtjgrxzrhr.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.sweek.top/gtfjjlnuje.html

[U83] JS：ES Module 导入导出
来源：http://hz.dashuyun.cn/gtltyzoveg.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.zdqjudy.top/gtkrwozzlg.html

[U84] JS：CommonJS 写法
来源：http://hz.ywan-chungtsiang.top/gtlysypccn.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.kuanghao11.cn/gtgaqnkewm.html

[U85] JS：可选链
来源：http://hz.quarkkingdee.top/gtsmmwbmdv.html

a?.b?.c
来源：http://hz.ydzc1.top/gtjyvbyuln.html

[U86] JS：空值合并
来源：http://hz.cucudq.cn/gtcdwisllc.html

a ?? b
来源：http://hz.ywan-chungtsiang.top/gtoonhvuvy.html

[U87] JS：解构默认值
来源：http://hz.cheryme.top/gtlukyldfm.html

const { a = 1, b = 2 } = obj;
来源：http://hz.shuidangran.top/gtcgwtzxeb.html

[U88] JS：对象展开合并
来源：http://hz.cashguo.top/gtejxvctux.html

{ ...a, ...b }
来源：http://hz.kuanghao11.cn/gtiqglqqhe.html

[U89] JS：数组去重
来源：http://hz.zhongyouzk.top/gtnrnfzhwi.html

[...new Set(arr)]
来源：http://hz.guowangkeji.top/gtaboblnpv.html

[U90] JS：数字数组排序
来源：http://hz.daria6918.cn/gtzliddmew.html

[...arr].sort((a, b) => a - b)
来源：http://hz.guowangkeji.top/gtqucolvlm.html

[U91] JS：对象键值遍历
来源：http://hz.xuanzx.com/gtcmhfjhls.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.yuanzhike.top/gtfocdezrs.html

[U92] JS：深拷贝
来源：http://hz.hysaishi.cn/gturzozlmy.html

structuredClone(obj)
来源：http://hz.pengpengdd.cyou/gteooyosss.html

[U93] JS：模板字符串
来源：http://hz.hammf.cn/gtipdnzltv.html

`共 ${n} 条`
来源：http://hz.dianchejie.cn/gtnrsyuxcf.html

[U94] JS：箭头函数
来源：http://hz.tian-w.cn/gtyrcxashd.html

const double = x => x * 2;
来源：http://hz.yongpay.top/gtzmrwbdoq.html

[U95] JS：Promise 包装
来源：http://hz.shzxlz.cn/gttnullcgi.html

new Promise((resolve, reject) => {})
来源：http://hz.zhiwuduotai.top/gtaypffzyl.html

[U96] JS：async/await 与异常
来源：http://hz.ydzc1.top/gtesbkqvpv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.zhongyouzk.top/gtihaymqyu.html

[U97] JS：并发请求
来源：http://hz.dashuyun.cn/gtetcuweao.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.bjfxy.top/gttqmiploy.html

[U98] JS：fetch 带 JSON
来源：http://hz.hysaishi.cn/gtbpxuadij.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.guannengcc.top/gtdonosaxe.html

[U99] JS：事件监听
来源：http://hz.0kj1m.cn/gtimilyxke.html

el.addEventListener("click", e => {})
来源：http://hz.gogol.net.cn/gtalfxwtuq.html

[U100] JS：DOM 查询
来源：http://hz.dashuyun.cn/gtzhuuakhh.html

document.querySelector(".item")
来源：http://hz.316326.xyz/gtfrirwiln.html

[U101] JS：classList 操作
来源：http://hz.redwolf501.top/gtminmcxeg.html

el.classList.toggle("active")
来源：http://hz.kuanghao11.cn/gtxkkjmrwc.html

[U102] JS：本地存储
来源：http://hz.jyoumei.cn/gtnjiykkch.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.yj20258.top/gtjidtcrdv.html

[U103] JS：定时器
来源：http://hz.zhixingplan.top/gtfhmqppdw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.zdqjudy.top/gtaktjjpfw.html

[U104] JS：防抖
来源：http://hz.xylfe.cn/gtmvjqfeuw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hysaishi.cn/gtxmoqdbza.html

[U105] JS：节流
来源：http://hz.jinyuanbaomall.cn/gtwxwfnjwo.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.pycfn.com/gttbjbfohe.html

[U106] JS：日期格式化
来源：http://hz.gzhubu.top/gtkxhnsqbc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.ydjk.org.cn/gtoubjoyal.html

[U107] JS：数字千分位
来源：http://hz.xziqi.cn/gtutomoont.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.zhixingplan.top/gtetaoachj.html

[U108] JS：随机整数
来源：http://hz.vqdsnc.cn/gtgtjvydba.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.vqdsnc.cn/gtxirffkzs.html

[U109] JS：数组分组
来源：http://hz.kuanghao11.cn/gtwnibxduf.html

Object.groupBy(arr, x => x.type)
来源：http://hz.haohaochexian.top/gtrtltidhf.html

[U110] JS：数组分块
来源：http://hz.iojbl.cn/gtouuxbsxs.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.haohaochexian.top/gtpdgctlnc.html

[U111] JS：对象转 Map
来源：http://hz.ehwqpu.com/gtmdzzxpbv.html

new Map(Object.entries(obj))
来源：http://hz.shuidangran.top/gturxynddk.html

[U112] JS：字符串补位
来源：http://hz.316326.xyz/gtiqdterut.html

"7".padStart(3, "0")
来源：http://hz.hnxiangtu.top/gtzbgtiraq.html

[U113] JS：正则替换全部
来源：http://hz.xylfe.cn/gtzkgkmudk.html

s.replaceAll("a", "b")
来源：http://hz.ywan-chungtsiang.top/gttolwnbzs.html

[U114] JS：JSON 深比较
来源：http://hz.hammf.cn/gtwldfdweg.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.cashguo.top/gtwhqzpipt.html

[U115] JS：生成 UUID
来源：http://hz.quarkkingdee.top/gtydpollmn.html

crypto.randomUUID()
来源：http://hz.yvedp.cn/gtqihgjkuv.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.hfpthk.cn/gtaxyeynzq.html

/** @param {string} name */ function f(name) {}
来源：http://hz.yuxming.cn/gtwyfjkeqk.html

[U117] JS：单元测试
来源：http://hz.hammf.cn/gtkulxumca.html

npm i -D vitest;  npx vitest
来源：http://hz.sysykeji.top/gtbxssbgpj.html

[U118] JS：开发服务器
来源：http://hz.dashuyun.cn/gtbcsflpmi.html

npm i -D vite;  npx vite
来源：http://hz.zhoulong.xyz/gtdflddgza.html

[U119] JS：生产构建
来源：http://hz.pycfn.com/gtsfvimkvo.html

npx vite build
来源：http://hz.zhixingplan.top/gtbsxxrivb.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.kuanghao11.cn/gtmmzwlfmf.html

import.meta.env.VITE_API_URL
来源：http://hz.yangfankeji.com/gtoithghbo.html

================================================================================
来源：http://hz.andypj.xyz/gthbzarluw.html

统计汇总
来源：http://hz.svipenyu.cn/gtbqmkcpzh.html

================================================================================
来源：http://hz.shuidangran.top/gtgzreabts.html

按语言统计（条）：
来源：http://hz.xuetiantiany.cn/gtuhsjgspp.html

Python ......... 252
来源：http://hz.yj20258.top/gtjshuhkex.html

PHP ............ 252
来源：http://hz.yj20258.top/gtaemtgvdj.html

JavaScript ..... 252
来源：http://hz.redwolf501.top/gtvyngfcxl.html

TypeScript ..... 212
来源：http://hz.xziqi.cn/gtpcvmrqjs.html

Java ........... 212
来源：http://hz.dashuyun.cn/gtkrrbqsbk.html

Go ............. 212
来源：http://hz.9152youxi.cn/gtsrbkutik.html

Ruby ........... 212
来源：http://hz.ehwqpu.com/gtqqyopubj.html

C# ............. 212
来源：http://hz.jinqigfzy.top/gtinofaktc.html

C .............. 30
来源：http://hz.yonumen.top/gtlwmpfrzd.html

C++ ............ 30
来源：http://hz.jinyuanbaomall.cn/gtbizpqovn.html

SQL ............ 90
来源：http://hz.xylfe.cn/gtvhagxztr.html

Bash ........... 80
来源：http://hz.fzhhl.top/gtspbuzneq.html

Kotlin ......... 15
来源：http://hz.zhiwuduotai.top/gtynbkmmdo.html

Swift .......... 15
来源：http://hz.shuidangran.top/gthoygdslv.html

Lua ............ 10
来源：http://hz.guowangkeji.top/gtpyentquw.html

Perl ........... 10
来源：http://hz.nanxuanxn.top/gtxssqoxtm.html

Scala .......... 10
来源：http://hz.zhaomingkeji.xyz/gtpnqgkkob.html

------------------------------------
来源：http://hz.havefunace.top/gtrxucsfcc.html

合计 ........... 2106 条
来源：http://hz.hfpthk.cn/gtfdrijopg.html

按章节统计：
来源：http://hz.hywenlv.cn/gtyfnmzcfm.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.hfpthk.cn/gtvqlmosbt.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.cheryme.top/gttcpqifae.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.zhongyouzk.top/gtarequbis.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.andypj.xyz/gtgjwyecvd.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.zhixingplan.top/gteeyfnwjt.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.guowangkeji.top/gtstdbktmw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.aizwys.cn/gtkjxlqtie.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.zycfv.cn/gtktaojztk.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.jianghu66.top/gtlgfropdr.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.kuanghao11.cn/gtjetifklz.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.ivvv.top/gtlsnsmgup.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.guannengcc.top/gtfxwrgbec.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.haohaochexian.top/gtcgjqntyq.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.0kj1m.cn/gtachzhfxg.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.nanxinkj.top/gtqvnhqqkh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.yuanzhike.top/gtsictnyoj.html

Q SQL 专题                              90
来源：http://hz.hywenlv.cn/gtuawoqqza.html

R Bash 专题                             80
来源：http://hz.chenzaomai.com/gtophgjekk.html

S C / C++ 专题                          60
来源：http://hz.xuanzx.com/gtysrxnwry.html

T 其他语言补充                          60
来源：http://hz.havefunace.top/gtpzuovggi.html

U 高频实用片段                         120
来源：http://hz.jinqigufen.top/gtzormnujq.html

------------------------------------
来源：http://hz.ydzc1.top/gtzcvgzjtj.html

合计                                  2106 条
来源：http://hz.chenlongwang.top/gtyybiwrhj.html

--------------------------------------------------------------------------------
来源：http://hz.9152youxi.cn/gtgaffgnif.html

使用提醒
来源：http://hz.cashguo.top/gtvoigolie.html

--------------------------------------------------------------------------------
来源：http://hz.hongshengwenyu.top/gtfvpthevn.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.jiagoushi.top/gttkbytdnh.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.zhongyouzk.top/gtiumchkpn.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.meibo888.top/gtarpehtok.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.xinyue.icu/gtinaymujv.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.hywenlv.cn/gtrnloibwy.html

—— 文件结束 ——
来源：http://hz.hfpthk.cn/gtlqbanxqw.html

================================================================================
来源：http://hz.jiagoushi.top/gtjdijcept.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.yj20258.top/gtyleveyly.html

Common Programming Examples Cheat Book
来源：http://hz.wangdashe.top/gtfahpuyww.html

================================================================================
来源：http://hz.chenzaomai.com/gtiefnueun.html

【收录内容】
来源：http://hz.zhengqikj.top/gtjsrzzhyn.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.jinghuilouyu.cn/gtpbbeehct.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.ydzc1.top/gtodqbttnj.html

SQL · Bash · C · C++
来源：http://hz.tanke756.top/gtclyvdmvk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.pengpengdd.cyou/gtnfsjzcdd.html

【使用说明】
来源：http://hz.cucudq.cn/gtarzkawfx.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.dianchejie.cn/gtngkeepoo.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.jianghu66.top/gtnycuqxgd.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.shanyushiyangkeji.top/gtkbbqdapy.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.bjfxy.top/gtgqooepqc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.jinghuilouyu.cn/gtodicjzhw.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.zhiwuduotai.top/gtidpqnnin.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.sxryk.cn/gtmwgafdpn.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.ppjwa.cn/gtujholyuk.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.hongshengwenyu.top/gtawylqtyx.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.xuanzx.com/gtqgvwmhub.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.hysaishi.cn/gtskboiawd.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.iojbl.cn/gtedpjlwow.html

【文件统计】
来源：http://hz.svipenyu.cn/gtshtygwxd.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.shanyushiyangtech.top/gtpqqcblfk.html

--------------------------------------------------------------------------------
来源：http://hz.hysaishi.cn/gtguhzybmj.html

目  录
来源：http://hz.jyoumei.cn/gtsfjareqa.html

--------------------------------------------------------------------------------
来源：http://hz.fzhhl.top/gtfjnclwst.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.chenzaomai.com/gtxxyikswb.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.svipenyu.cn/gtocybmmwe.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.nanxuanxn.top/gtgghpmhvy.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.daxiang520.top/gtghelpazs.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.ywan-chungtsiang.top/gtxduvaaeg.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.xuetiantiany.cn/gtmllbhury.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.pengpengdd.cyou/gtmwssusrj.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.tanke756.top/gtgxldmxoi.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.gaohongyu789.top/gtpyokalvn.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.cashguo.top/gtudugkdsm.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.shanyushiyangkeji.top/gtzmmepecd.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.zhixingplan.top/gtffhgqmax.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.yj20258.top/gtlonsllqt.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.gzhubu.top/gtxfeokzbc.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.yj20258.top/gtovpmryva.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.nwbrower.top/gtkrllpagc.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.pycfn.com/gthqmuihix.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.kuanghao11.cn/gtelppdtop.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.ehwqpu.com/gtxumkemau.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhijiandao.cn/gtrgxdndmt.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.jinqigufen.top/gtimisfawj.html

================================================================================
来源：http://hz.kuanghao11.cn/gtobgbzbvw.html

A. 基础语法与类型
来源：http://hz.gotoacloud.top/gtpkaxkfla.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtfzujools.html

[A01] Hello World
来源：http://hz.nanxinkj.top/gtwhqindfs.html

Py:   print("Hello, World!")
来源：http://hz.ywan-chungtsiang.top/gtbowwhdwa.html

PHP:  echo "Hello, World!";
来源：http://hz.feifeiyinyue.top/gtgeepylnp.html

JS:   console.log("Hello, World!");
来源：http://hz.wangshuangyany.cn/gthblwuoge.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.fengsongda.top/gtspcfthsc.html

Java: System.out.println("Hello, World!");
来源：http://hz.ywan-chungtsiang.top/gteevvqsef.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.dianchejie.cn/gtlicidrsk.html

Ruby: puts "Hello, World!"
来源：http://hz.xylfe.cn/gtvitqeqox.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.yangfankeji.com/gttibkmziv.html

[A02] 变量声明与赋值
来源：http://hz.nanxuanxn.top/gtxdhhyhaf.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.yonumen.top/gtmtdnausm.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.chenlongwang.top/gtvjhxyyzs.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.yvedp.cn/gtamqzffat.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.mhx1999.top/gtqdwjavvw.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.wangdashe.top/gtinbrlamk.html

Go:   name := "Alex"; age := 20
来源：http://hz.aizwys.cn/gtshjssamh.html

Ruby: name = "Alex"; age = 20
来源：http://hz.nanxuanxn.top/gtglenohkm.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.sweek.top/gtguizqkyx.html

[A03] 常量定义
来源：http://hz.yj20258888.top/gthuhfcmlq.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.hywenlv.cn/gtlygcehfr.html

PHP:  const PI = 3.14159;
来源：http://hz.jqgfzy.top/gtpgupfxfh.html

JS:   const PI = 3.14159;
来源：http://hz.feifeiyinyue.top/gtbtzijvmz.html

TS:   const PI: number = 3.14159;
来源：http://hz.shuidangran.top/gtamswvanu.html

Java: static final double PI = 3.14159;
来源：http://hz.guannengcc.top/gtixiwudyz.html

Go:   const PI = 3.14159
来源：http://hz.haohaochexian.top/gtthjcqnhl.html

Ruby: PI = 3.14159
来源：http://hz.daria6918.cn/gtfosmntzc.html

C#:   const double PI = 3.14159;
来源：http://hz.gotoacloud.top/gtahkcokxe.html

[A04] 判断变量类型
来源：http://hz.snrcjt.cn/gtzkoqulxf.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.ivvv.top/gtrvvmkhfd.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.nwbrower.top/gtlrtbosgf.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.hammf.cn/gtcvzhnzqs.html

TS:   typeof x; x instanceof Date
来源：http://hz.kuanghao11.cn/gtfhkgjetv.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.cqqwz.cn/gtvigyujfn.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.jlsjyb.cn/gtvusfjslt.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.xziqi.cn/gtlwzoeyed.html

C#:   x.GetType().Name; x is int
来源：http://hz.zhixingplan.top/gtftedpace.html

[A05] 整数除法与取模
来源：http://hz.hnxiangtu.top/gtgqtzuzwy.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.tian-w.cn/gtoemypmbt.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.daxiang520.top/gtjbgpzlio.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.hnxiangtu.top/gtxtunkhsh.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.hywenlv.cn/gtwnbkiolu.html

Java: 7 / 2; 7 % 2
来源：http://hz.hongshengwenyu.top/gtufivpzre.html

Go:   7 / 2; 7 % 2
来源：http://hz.tanke756.top/gtnmpocsfw.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.0kj1m.cn/gtixpydpij.html

C#:   7 / 2; 7 % 2
来源：http://hz.quarkkingdee.top/gthonbwbea.html

[A06] 字符串转数字
来源：http://hz.dashuyun.cn/gtfdqbpynb.html

Py:   int("42"); float("3.14")
来源：http://hz.yueranfly.top/gtscvhemms.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.vqdsnc.cn/gttwtwtvwe.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.9152youxi.cn/gtougvuwmo.html


<!-- 参考信息 -->