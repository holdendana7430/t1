代发 wailian999

[U49] PHP：只读属性
来源：http://hz.tanke756.top/gtjjhvueuv.html

public readonly string $name
来源：http://hz.ehwqpu.com/gtpwphmrks.html

[U50] PHP：构造器属性提升
来源：http://hz.yueranfly.top/gtwtrcoldi.html

public function __construct(private int $id) {}
来源：http://hz.daxiang520.top/gtahocjbkl.html

[U51] PHP：数组解构
来源：http://hz.nanxinkj.top/gtpfkovltw.html

[$a, $b] = $arr;
来源：http://hz.vqdsnc.cn/gtilwtcckq.html

[U52] PHP：箭头函数
来源：http://hz.zhiwuduotai.top/gtldxvltwk.html

$double = fn($x) => $x * 2;
来源：http://hz.haohaochexian.top/gtjsndbngy.html

[U53] PHP：空合并运算符
来源：http://hz.chenzaomai.com/gtwvzujitf.html

$v = $a ?? $b ?? "default";
来源：http://hz.jlsjyb.cn/gtocjvilze.html

[U54] PHP：空安全调用
来源：http://hz.jinqigfzy.top/gtvtimmevw.html

$obj?->method()
来源：http://hz.xuanzx.com/gtqavqkjxw.html

[U55] PHP：match 表达式
来源：http://hz.chenzaomai.com/gtitqjtzun.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.yuxming.cn/gtmyvowcty.html

[U56] PHP：命名参数
来源：http://hz.ywan-chungtsiang.top/gtydczzhof.html

f(a: 1, b: 2)
来源：http://hz.shanyushiyangkeji.top/gtnavsnlth.html

[U57] PHP：字符串插值
来源：http://hz.smart0.xyz/gtqmvmmzeq.html

"值: {$a}"
来源：http://hz.daxiang520.top/gtuugrxbhw.html

[U58] PHP：数组三件套
来源：http://hz.ydjk.org.cn/gtuouuvmut.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.dianchejie.cn/gtjxfilxmq.html

[U59] PHP：自定义排序
来源：http://hz.yueranfly.top/gtzxjzmfjk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hysaishi.cn/gtrponfcof.html

[U60] PHP：JSON 编解码
来源：http://hz.yueranfly.top/gtbvoxarjz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.sxryk.cn/gtwuhsnzcm.html

[U61] PHP：正则
来源：http://hz.sweek.top/gtphgcrfdt.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.sweek.top/gtyqrfylon.html

[U62] PHP：日期对象
来源：http://hz.yonumen.top/gtcpgpncci.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.hywenlv.cn/gtayxqsdcq.html

[U63] PHP：文件读写
来源：http://hz.pengpengdd.cyou/gtfbfcsfnw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.jiagoushi.top/gtfqpdbtio.html

[U64] PHP：目录遍历
来源：http://hz.gogol.net.cn/gtpsxtugpi.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.yj202588.top/gthnsgltui.html

[U65] PHP：会话
来源：http://hz.ivvv.top/gtzmwtikxw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.nanxinkj.top/gttlobgshb.html

[U66] PHP：设置 Cookie
来源：http://hz.zdqjudy.top/gtfwhdcyqm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.zhijiandao.cn/gtdqfmsiqb.html

[U67] PHP：处理文件上传
来源：http://hz.zdqjudy.top/gtfgqgkumk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.tian-w.cn/gtstpygrze.html

[U68] PHP：PDO 连接
来源：http://hz.jqgfzy.top/gtjsoxvuae.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.zhixingplan.top/gtommsbuqa.html

[U69] PHP：PDO 预处理
来源：http://hz.yj20258888.top/gtxwxedocy.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.ppjwa.cn/gtmsdfzzhg.html

[U70] PHP：PDO 事务
来源：http://hz.birdmap.top/gtzndaumpg.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.0kj1m.cn/gtdqwigsdw.html

[U71] PHP：抛出异常
来源：http://hz.wangdashe.top/gtorkqbnce.html

throw new RuntimeException("失败", 500);
来源：http://hz.bjfxy.top/gtguvcyfst.html

[U72] PHP：写错误日志
来源：http://hz.feifeiyinyue.top/gtxgkcroef.html

error_log("失败: " . $e->getMessage());
来源：http://hz.zhiwuduotai.top/gtmwciybcf.html

[U73] PHP：读取 ini 配置
来源：http://hz.wangshuangyany.cn/gtxatdpnte.html

parse_ini_file("config.ini", true)
来源：http://hz.guowangkeji.top/gtsxgxlfiy.html

[U74] PHP：读取环境变量
来源：http://hz.ppjwa.cn/gtdbgbbvse.html

getenv("APP_ENV") ?: "production"
来源：http://hz.cqqwz.cn/gtgpfhdbql.html

[U75] PHP：依赖注入
来源：http://hz.vqdsnc.cn/gttjgccpru.html

composer require psr/container
来源：http://hz.dianchejie.cn/gtkqfurdcr.html

[U76] PHP：简单路由
来源：http://hz.fzhhl.top/gtbgagpyju.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.tian-w.cn/gttolkyycj.html

[U77] PHP：模板渲染
来源：http://hz.dianchejie.cn/gtgymgvezo.html

composer require twig/twig
来源：http://hz.sufxvd.cn/gtmfexizrc.html

[U78] PHP：单元测试
来源：http://hz.gzhubu.top/gtejbuwmic.html

composer require --dev phpunit/phpunit
来源：http://hz.sweek.top/gtiuvsgyge.html

[U79] PHP：静态分析
来源：http://hz.snrcjt.cn/gttvhvamhj.html

composer require --dev phpstan/phpstan
来源：http://hz.9152youxi.cn/gtodhjnebz.html

[U80] PHP：代码规范修复
来源：http://hz.vqdsnc.cn/gtyagclwlp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.nanxuanxn.top/gtcvsrnsji.html

[U81] JS：初始化项目
来源：http://hz.kuanghao11.cn/gtpghjehtc.html

npm init -y;  npm i express
来源：http://hz.cqqwz.cn/gtykdowjbl.html

[U82] JS：package.json 脚本
来源：http://hz.gotoacloud.top/gtkcvclwre.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.hnqzz.top/gtovllleaf.html

[U83] JS：ES Module 导入导出
来源：http://hz.dianchejie.cn/gttxorchtv.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.dianchejie.cn/gtzlfxpqok.html

[U84] JS：CommonJS 写法
来源：http://hz.sweek.top/gtbykwirfe.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.cheryme.top/gtaromyukf.html

[U85] JS：可选链
来源：http://hz.zhixingplan.top/gtirpvmhvp.html

a?.b?.c
来源：http://hz.feifeiyinyue.top/gtpgmjlhns.html

[U86] JS：空值合并
来源：http://hz.dashuyun.cn/gtnvhlqfpu.html

a ?? b
来源：http://hz.zdqjudy.top/gtjcytdumh.html

[U87] JS：解构默认值
来源：http://hz.xuanzx.com/gtckvimnxz.html

const { a = 1, b = 2 } = obj;
来源：http://hz.zhixingplan.top/gtnbajslfp.html

[U88] JS：对象展开合并
来源：http://hz.kuanghao11.cn/gtgqbbwuww.html

{ ...a, ...b }
来源：http://hz.chenlongwang.top/gtrlniwsmx.html

[U89] JS：数组去重
来源：http://hz.c1oappe.top/gtqnjsthji.html

[...new Set(arr)]
来源：http://hz.yj20258.top/gtbsxclzei.html

[U90] JS：数字数组排序
来源：http://hz.pengpengdd.cyou/gtebhroynd.html

[...arr].sort((a, b) => a - b)
来源：http://hz.xuetiantiany.cn/gtfgzgeitu.html

[U91] JS：对象键值遍历
来源：http://hz.sweek.top/gtkwimnhot.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.hysaishi.cn/gticwollva.html

[U92] JS：深拷贝
来源：http://hz.bjfxy.top/gtdhbiifjw.html

structuredClone(obj)
来源：http://hz.gaohongyu789.top/gtckbacunf.html

[U93] JS：模板字符串
来源：http://hz.zhengqikj.top/gtzrodapbu.html

`共 ${n} 条`
来源：http://hz.jqgfzy.top/gtjxipngjo.html

[U94] JS：箭头函数
来源：http://hz.snrcjt.cn/gtqbccqfwk.html

const double = x => x * 2;
来源：http://hz.zhaomingkeji.xyz/gtltvdybpk.html

[U95] JS：Promise 包装
来源：http://hz.hysaishi.cn/gtrhngyuoh.html

new Promise((resolve, reject) => {})
来源：http://hz.nanxuanxn.top/gtuhbwodyr.html

[U96] JS：async/await 与异常
来源：http://hz.iojbl.cn/gtuldiidhx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.jinyuanbaomall.cn/gtjlecdcgc.html

[U97] JS：并发请求
来源：http://hz.gogol.net.cn/gtfeoctpvj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.0kj1m.cn/gtyvagbiea.html

[U98] JS：fetch 带 JSON
来源：http://hz.nanxinkj.top/gtqeabuoej.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.cdnleiting.top/gtzxpyicbe.html

[U99] JS：事件监听
来源：http://hz.chenjidiqi.icu/gtmimqsxdn.html

el.addEventListener("click", e => {})
来源：http://hz.jinyuanbaomall.cn/gtcdxuwawc.html

[U100] JS：DOM 查询
来源：http://hz.cheryme.top/gtrbtujibr.html

document.querySelector(".item")
来源：http://hz.yongpay.top/gtanzlrerc.html

[U101] JS：classList 操作
来源：http://hz.hongshengwenyu.top/gtldsivdzx.html

el.classList.toggle("active")
来源：http://hz.hfpthk.cn/gtyowptptq.html

[U102] JS：本地存储
来源：http://hz.bjfxy.top/gtxhftgpla.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.jinyuanbaomall.cn/gtjrtupbxd.html

[U103] JS：定时器
来源：http://hz.xingfuxueyuan.xyz/gtkwrdbkue.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.ywan-chungtsiang.top/gtqkhbzrnk.html

[U104] JS：防抖
来源：http://hz.jiagoushi.top/gtwdxpxwen.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.fzhhl.top/gtfhqodbbj.html

[U105] JS：节流
来源：http://hz.gogol.net.cn/gtgizzolhr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.meibo888.top/gtoqsvdpth.html

[U106] JS：日期格式化
来源：http://hz.andypj.xyz/gthhuqkzfm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.tanke756.top/gtzchmzlsj.html

[U107] JS：数字千分位
来源：http://hz.fengsongda.top/gtjbwvvfuz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.tian-w.cn/gtowvxqytv.html

[U108] JS：随机整数
来源：http://hz.jinqigfzy.top/gtvxwuvywg.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.redwolf501.top/gtfeihkstj.html

[U109] JS：数组分组
来源：http://hz.tian-w.cn/gtpryqjfnp.html

Object.groupBy(arr, x => x.type)
来源：http://hz.xuetiantiany.cn/gtncqgpnsr.html

[U110] JS：数组分块
来源：http://hz.feifeiyinyue.top/gtpmshmnuk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.fengsongda.top/gtoktaowyz.html

[U111] JS：对象转 Map
来源：http://hz.ydzc1.top/gtdnlnjovu.html

new Map(Object.entries(obj))
来源：http://hz.shanyushiyangkeji.top/gtbvldblqt.html

[U112] JS：字符串补位
来源：http://hz.tian-w.cn/gtpypgyzwz.html

"7".padStart(3, "0")
来源：http://hz.52xcode.cn/gtcyherjez.html

[U113] JS：正则替换全部
来源：http://hz.yangfankeji.com/gtyvncztsj.html

s.replaceAll("a", "b")
来源：http://hz.zhoulong.xyz/gtjifcshgp.html

[U114] JS：JSON 深比较
来源：http://hz.kuanghao11.cn/gtigouvgdk.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xingfuxueyuan.xyz/gtvoyituth.html

[U115] JS：生成 UUID
来源：http://hz.shangyingyoupin.top/gtsizzbgtc.html

crypto.randomUUID()
来源：http://hz.shanyushiyangtech.top/gtmcsnjhtx.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.ehwqpu.com/gtzmtasbku.html

/** @param {string} name */ function f(name) {}
来源：http://hz.haohaochexian.top/gtnaflipmn.html

[U117] JS：单元测试
来源：http://hz.ydjk.org.cn/gtfoezikpt.html

npm i -D vitest;  npx vitest
来源：http://hz.hammf.cn/gtxugqfxvm.html

[U118] JS：开发服务器
来源：http://hz.jinyuanbaomall.cn/gtewrspwrd.html

npm i -D vite;  npx vite
来源：http://hz.wangshuangyany.cn/gtuqbcumah.html

[U119] JS：生产构建
来源：http://hz.c1oappe.top/gtjyfdzenn.html

npx vite build
来源：http://hz.cdnleiting.top/gtegbwgter.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.yueranfly.top/gtpjfvxfbf.html

import.meta.env.VITE_API_URL
来源：http://hz.jqgfzy.top/gtbnaxvgvt.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtmsrsccra.html

统计汇总
来源：http://hz.zhoulong.xyz/gtteueegqs.html

================================================================================
来源：http://hz.jqgufenzy.top/gtqtfsveji.html

按语言统计（条）：
来源：http://hz.wangdashe.top/gtkiugjcwj.html

Python ......... 252
来源：http://hz.jyoumei.cn/gtgjunkilq.html

PHP ............ 252
来源：http://hz.jinghuilouyu.cn/gtlpuxauzo.html

JavaScript ..... 252
来源：http://hz.52xcode.cn/gtfycmkcvm.html

TypeScript ..... 212
来源：http://hz.zhoulong.xyz/gtbcwixjko.html

Java ........... 212
来源：http://hz.kuanghao11.cn/gtmscnqbex.html

Go ............. 212
来源：http://hz.iojbl.cn/gtlxxtvsuu.html

Ruby ........... 212
来源：http://hz.fzhhl.top/gtgkfnfzxv.html

C# ............. 212
来源：http://hz.ydjk.org.cn/gtpfgklegf.html

C .............. 30
来源：http://hz.hammf.cn/gtaomeutsg.html

C++ ............ 30
来源：http://hz.kuanghao11.cn/gtzpshyzzj.html

SQL ............ 90
来源：http://hz.yuxming.cn/gtkfiednhr.html

Bash ........... 80
来源：http://hz.xingfuxueyuan.xyz/gtoblbgtap.html

Kotlin ......... 15
来源：http://hz.yonumen.top/gtskbvkdoc.html

Swift .......... 15
来源：http://hz.andypj.xyz/gtehusgris.html

Lua ............ 10
来源：http://hz.316326.xyz/gtprjxzxce.html

Perl ........... 10
来源：http://hz.ywan-chungtsiang.top/gtmgstzqot.html

Scala .......... 10
来源：http://hz.yj20258888.top/gtsmksnxtv.html

------------------------------------
来源：http://hz.guannengcc.top/gtofrtyvjh.html

合计 ........... 2106 条
来源：http://hz.9152youxi.cn/gtkqgkguhg.html

按章节统计：
来源：http://hz.guowangkeji.top/gtbpnutcmv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.yj202588.top/gtcmpggdbx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.52xcode.cn/gtljvkzuah.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.smart0.xyz/gtqoynbmnk.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.cheryme.top/gtrxaebqwd.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.cqqwz.cn/gtrphsnpcd.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.zhaomingkeji.xyz/gtzivkxbpc.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.tianlin.xyz/gtmjmpqiko.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.aibaodan.cn/gtwalzqvet.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.shzxlz.cn/gthplwzblw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.hnqzz.top/gtdalzojkk.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.316326.xyz/gtgdidgnum.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.yj202588.top/gtkuynawan.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.yuanzhike.top/gtacvkmrhz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.xuetiantiany.cn/gtvuqahznu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.zhiwuduotai.top/gtvdbsfizo.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.ppjwa.cn/gtcnzdverd.html

Q SQL 专题                              90
来源：http://hz.sufxvd.cn/gtyccuveua.html

R Bash 专题                             80
来源：http://hz.xylfe.cn/gtdsmfkwzc.html

S C / C++ 专题                          60
来源：http://hz.havefunace.top/gttyyhxeuh.html

T 其他语言补充                          60
来源：http://hz.xuanzx.com/gtpvlrgfhs.html

U 高频实用片段                         120
来源：http://hz.aizwys.cn/gtuocwxshv.html

------------------------------------
来源：http://hz.hfpthk.cn/gtvihlhsqa.html

合计                                  2106 条
来源：http://hz.ydjk.org.cn/gtjsaiocxp.html

--------------------------------------------------------------------------------
来源：http://hz.zhaomingkeji.xyz/gtyjbfmocc.html

使用提醒
来源：http://hz.yj202588.top/gtslaeldbg.html

--------------------------------------------------------------------------------
来源：http://hz.jqgufenzy.top/gtdgxnoyee.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.andypj.xyz/gtpnmmfvvy.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.vqdsnc.cn/gtiukdsqal.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.yj20258.top/gtsavuskjp.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.ydzc1.top/gtvpxfunvt.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.c1oappe.top/gthaqlvyse.html

—— 文件结束 ——
来源：http://hz.shangyingyoupin.top/gttugxymlt.html

================================================================================
来源：http://hz.sysykeji.top/gttxyxrkcg.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.jqgufenzy.top/gtzxvmovgv.html

Common Programming Examples Cheat Book
来源：http://hz.hnqzz.top/gtdfikysmo.html

================================================================================
来源：http://hz.vqdsnc.cn/gtskxnqwih.html

【收录内容】
来源：http://hz.jinyuanbaomall.cn/gtwnuesnme.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.yj20258888.top/gtqpacrfmm.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.nanxinkj.top/gtsjiajxcp.html

SQL · Bash · C · C++
来源：http://hz.quarkkingdee.top/gtkcxoicwf.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.zhiwuduotai.top/gteullwivk.html

【使用说明】
来源：http://hz.jinghuilouyu.cn/gtuolcvbss.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.meibo888.top/gtjdzncjhf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.xziqi.cn/gtmnuktsps.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.zdqjudy.top/gtbncffmog.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.tianlin.xyz/gtwlexmzdz.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.dashuyun.cn/gtayvitujs.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.gogol.net.cn/gtlkspwnjd.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.redwolf501.top/gtocftnnas.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.chenjidiqi.icu/gtgjftqtgc.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.wangshuangyany.cn/gtebpkywfj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.xingfuxueyuan.xyz/gtqgjrdfsj.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.feifeiyinyue.top/gtdjexrgwf.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.hfpthk.cn/gtdpftsdoq.html

【文件统计】
来源：http://hz.zhiwuduotai.top/gthtnjsyix.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.feifeiyinyue.top/gtdsgarihn.html

--------------------------------------------------------------------------------
来源：http://hz.ehwqpu.com/gtyrtnrury.html

目  录
来源：http://hz.zhijiandao.cn/gtwosdyolh.html

--------------------------------------------------------------------------------
来源：http://hz.shanyushiyangkeji.top/gtsjdawsnw.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.havefunace.top/gttlggrcmt.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.jinyuanbaomall.cn/gtddznyqvn.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.hysaishi.cn/gtykwvdbua.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.tian-w.cn/gtzdtmsdbj.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.jiagoushi.top/gtwatdcvna.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.birdmap.top/gthkzwfoqr.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.9152youxi.cn/gtrmfgnlxb.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.xylfe.cn/gttgzmqkwy.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.fzhhl.top/gtogdakykc.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.quarkkingdee.top/gtfdwnuybj.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.ydzc1.top/gtvmjkzfgt.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.dianchejie.cn/gtbrbtwlva.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.nanxuanxn.top/gtuhxvpcox.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.xuanzx.com/gtmspdhrfb.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.yuxming.cn/gtyawwwuqk.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.svipenyu.cn/gtxzrgklpl.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.9152youxi.cn/gtkwnuoslm.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.sweek.top/gteynthqsd.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.chenzaomai.com/gtadhgjqrq.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.pycfn.com/gtgbsxhjbv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.aibaodan.cn/gtjijcywnx.html

================================================================================
来源：http://hz.gzhubu.top/gtgpgoylvr.html

A. 基础语法与类型
来源：http://hz.ehwqpu.com/gtmdgoibni.html

================================================================================
来源：http://hz.ydzc1.top/gttnvejsws.html

[A01] Hello World
来源：http://hz.jqgufenzy.top/gtkdatkjzs.html

Py:   print("Hello, World!")
来源：http://hz.andypj.xyz/gtnajdeklc.html

PHP:  echo "Hello, World!";
来源：http://hz.hnqzz.top/gtkxkvsimr.html

JS:   console.log("Hello, World!");
来源：http://hz.svipenyu.cn/gtrxrizomg.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.tian-w.cn/gtyltsldje.html

Java: System.out.println("Hello, World!");
来源：http://hz.hammf.cn/gtgbipofkb.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.aizwys.cn/gtfmazvezx.html

Ruby: puts "Hello, World!"
来源：http://hz.xziqi.cn/gtlkbrfwvh.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.yvedp.cn/gtarjgskjx.html

[A02] 变量声明与赋值
来源：http://hz.xuanzx.com/gtzqwqxnvh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.haohaochexian.top/gtahltfbfl.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.zhiwuduotai.top/gtxjomaqpy.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.dashuyun.cn/gtbxlpfnnc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.zhaomingkeji.xyz/gtdjuioajs.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.kuanghao11.cn/gtxtfsmrxv.html

Go:   name := "Alex"; age := 20
来源：http://hz.hywenlv.cn/gtyzhgdinc.html

Ruby: name = "Alex"; age = 20
来源：http://hz.shanyushiyangkeji.top/gtntaksfsv.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.haohaochexian.top/gtzvmnsbat.html

[A03] 常量定义
来源：http://hz.dianchejie.cn/gtqlrijfwg.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.mhx1999.top/gtiouykype.html

PHP:  const PI = 3.14159;
来源：http://hz.dianchejie.cn/gtlhbytwnl.html

JS:   const PI = 3.14159;
来源：http://hz.hnxiangtu.top/gtwwndumvv.html

TS:   const PI: number = 3.14159;
来源：http://hz.quarkkingdee.top/gtlagjfdqs.html

Java: static final double PI = 3.14159;
来源：http://hz.shuidangran.top/gtrexcpmdu.html

Go:   const PI = 3.14159
来源：http://hz.yanxiufei.cn/gtujxxyras.html

Ruby: PI = 3.14159
来源：http://hz.jinghuilouyu.cn/gtnmrzrooa.html

C#:   const double PI = 3.14159;
来源：http://hz.cashguo.top/gtbzinaosj.html

[A04] 判断变量类型
来源：http://hz.shuidangran.top/gtpwzfelst.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.jinyuanbaomall.cn/gtravrvpgo.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.yuanzhike.top/gtiktsfrfg.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.cdnleiting.top/gtxqprpnmo.html

TS:   typeof x; x instanceof Date
来源：http://hz.vqdsnc.cn/gtranjdowo.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.bjfxy.top/gtjzsmlelf.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.bjfxy.top/gtqqcsfgvn.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.gotoacloud.top/gtwmahtwrg.html

C#:   x.GetType().Name; x is int
来源：http://hz.chenjidiqi.icu/gtusgfozgl.html

[A05] 整数除法与取模
来源：http://hz.mhx1999.top/gthnobantk.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.guowangkeji.top/gtczgcxttm.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.jinqigfzy.top/gtagpebofv.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.snrcjt.cn/gtdqehmcni.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.0kj1m.cn/gtvlfusypq.html

Java: 7 / 2; 7 % 2
来源：http://hz.9152youxi.cn/gtjcoxwtxk.html

Go:   7 / 2; 7 % 2
来源：http://hz.yj20258888.top/gtstnnanec.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.chenlongwang.top/gtqouyumyo.html

C#:   7 / 2; 7 % 2
来源：http://hz.xinyue.icu/gthtwpmlnv.html

[A06] 字符串转数字
来源：http://hz.pengpengdd.cyou/gtgyqzzzps.html

Py:   int("42"); float("3.14")
来源：http://hz.snrcjt.cn/gtzitsstze.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.ydjk.org.cn/gtksrmvhaq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.guannengcc.top/gtuasktnnu.html


<!-- 参考信息 -->