代发 wailian999

[U49] PHP：只读属性
来源：http://hz.shanyushiyangkeji.top/gthpalwboe.html

public readonly string $name
来源：http://hz.nwbrower.top/gtumevxmwl.html

[U50] PHP：构造器属性提升
来源：http://hz.hfpthk.cn/gtsecbjdhk.html

public function __construct(private int $id) {}
来源：http://hz.xylfe.cn/gthktggcvq.html

[U51] PHP：数组解构
来源：http://hz.iojbl.cn/gtfytjtses.html

[$a, $b] = $arr;
来源：http://hz.xuanzx.com/gtnubavdaa.html

[U52] PHP：箭头函数
来源：http://hz.chenzaomai.com/gtthtzwkjd.html

$double = fn($x) => $x * 2;
来源：http://hz.jiagoushi.top/gtjcnkyqzy.html

[U53] PHP：空合并运算符
来源：http://hz.daria6918.cn/gtvgrnzzmb.html

$v = $a ?? $b ?? "default";
来源：http://hz.fengsongda.top/gtfihdjden.html

[U54] PHP：空安全调用
来源：http://hz.svipenyu.cn/gtvjixxxfo.html

$obj?->method()
来源：http://hz.jinqigufen.top/gtvvdhmlfr.html

[U55] PHP：match 表达式
来源：http://hz.xylfe.cn/gtopfsaigc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.hnqzz.top/gtkuqrzztv.html

[U56] PHP：命名参数
来源：http://hz.zhongyouzk.top/gtlfcpdzkb.html

f(a: 1, b: 2)
来源：http://hz.nanxinkj.top/gtbuyahpyh.html

[U57] PHP：字符串插值
来源：http://hz.aizwys.cn/gtmwdylloo.html

"值: {$a}"
来源：http://hz.jyoumei.cn/gtufxovdsx.html

[U58] PHP：数组三件套
来源：http://hz.sweek.top/gttppzzacq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.0kj1m.cn/gtqqgspcdx.html

[U59] PHP：自定义排序
来源：http://hz.yueranfly.top/gtsnzsskvu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.chenjidiqi.icu/gtihjoltrw.html

[U60] PHP：JSON 编解码
来源：http://hz.cucudq.cn/gtjjmhzeuu.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.c1oappe.top/gtoupuvnku.html

[U61] PHP：正则
来源：http://hz.fengsongda.top/gtgrsgdfbj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.shzxlz.cn/gtatgfgxmv.html

[U62] PHP：日期对象
来源：http://hz.cucudq.cn/gtmyztsfvf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.c1oappe.top/gtcthvoyyt.html

[U63] PHP：文件读写
来源：http://hz.yuanzhike.top/gtqgpxwqgj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.yuanzhike.top/gtuqknapys.html

[U64] PHP：目录遍历
来源：http://hz.ivvv.top/gtcmgufulv.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.hnxiangtu.top/gtldedjhzr.html

[U65] PHP：会话
来源：http://hz.cdnleiting.top/gtijheqesm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.wangdashe.top/gtwkdlhrtg.html

[U66] PHP：设置 Cookie
来源：http://hz.hywenlv.cn/gtkepxddcx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.ppjwa.cn/gtkdrxhnlx.html

[U67] PHP：处理文件上传
来源：http://hz.hongshengwenyu.top/gtouozmyma.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.meibo888.top/gtdcieqrlw.html

[U68] PHP：PDO 连接
来源：http://hz.zhoulong.xyz/gtccufnosd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.yanxiufei.cn/gtakkxfwnp.html

[U69] PHP：PDO 预处理
来源：http://hz.cdnleiting.top/gtnnlemccj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.yvedp.cn/gtnrsdadjo.html

[U70] PHP：PDO 事务
来源：http://hz.tianlin.xyz/gtfipkijgs.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.haohaochexian.top/gtxjcszdne.html

[U71] PHP：抛出异常
来源：http://hz.hnqzz.top/gtiweclddm.html

throw new RuntimeException("失败", 500);
来源：http://hz.hammf.cn/gtkdvtkgrj.html

[U72] PHP：写错误日志
来源：http://hz.aibaodan.cn/gtnurhiwfd.html

error_log("失败: " . $e->getMessage());
来源：http://hz.tanke756.top/gtvhgivfaw.html

[U73] PHP：读取 ini 配置
来源：http://hz.nanxuanxn.top/gtcqzekhto.html

parse_ini_file("config.ini", true)
来源：http://hz.zhijiandao.cn/gtkhuffrsx.html

[U74] PHP：读取环境变量
来源：http://hz.sysykeji.top/gtkfbdodrm.html

getenv("APP_ENV") ?: "production"
来源：http://hz.yonumen.top/gtrcjmsana.html

[U75] PHP：依赖注入
来源：http://hz.xuanzx.com/gtgoimfeel.html

composer require psr/container
来源：http://hz.jqgfzy.top/gtfunywdhf.html

[U76] PHP：简单路由
来源：http://hz.gotoacloud.top/gtbogmgyal.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.hysaishi.cn/gtxilxgxli.html

[U77] PHP：模板渲染
来源：http://hz.pengpengdd.cyou/gtoxxxzwrv.html

composer require twig/twig
来源：http://hz.wangdashe.top/gtlpauvoav.html

[U78] PHP：单元测试
来源：http://hz.guowangkeji.top/gtqtfmwdtv.html

composer require --dev phpunit/phpunit
来源：http://hz.cdnleiting.top/gtxnaxmqek.html

[U79] PHP：静态分析
来源：http://hz.gaohongyu789.top/gtsdslvlun.html

composer require --dev phpstan/phpstan
来源：http://hz.hywenlv.cn/gtysyehwip.html

[U80] PHP：代码规范修复
来源：http://hz.zhongyouzk.top/gtlgearlgc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.wangshuangyany.cn/gtunyfwkrb.html

[U81] JS：初始化项目
来源：http://hz.zhoulong.xyz/gtugjwrivx.html

npm init -y;  npm i express
来源：http://hz.jinqigufen.top/gtlpddltkp.html

[U82] JS：package.json 脚本
来源：http://hz.chenzaomai.com/gtglbyrequ.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.hammf.cn/gthbnrkdfh.html

[U83] JS：ES Module 导入导出
来源：http://hz.kuanghao11.cn/gtsbvieisp.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.gotoacloud.top/gtadhbeulc.html

[U84] JS：CommonJS 写法
来源：http://hz.dashuyun.cn/gtcsxekjcw.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.chenzaomai.com/gtlewubrhs.html

[U85] JS：可选链
来源：http://hz.pengpengdd.cyou/gtootjiiwq.html

a?.b?.c
来源：http://hz.jqgufenzy.top/gttmmbmahv.html

[U86] JS：空值合并
来源：http://hz.jiagoushi.top/gtyjwlncpx.html

a ?? b
来源：http://hz.cqqwz.cn/gtiwyrqokl.html

[U87] JS：解构默认值
来源：http://hz.jqgfzy.top/gtnqtxddmv.html

const { a = 1, b = 2 } = obj;
来源：http://hz.gaohongyu789.top/gtbdewvkiu.html

[U88] JS：对象展开合并
来源：http://hz.hywenlv.cn/gtgjniolvq.html

{ ...a, ...b }
来源：http://hz.sufxvd.cn/gtlktfejfx.html

[U89] JS：数组去重
来源：http://hz.tianlin.xyz/gtggvwmjyc.html

[...new Set(arr)]
来源：http://hz.zhongyouzk.top/gtfhrqrazh.html

[U90] JS：数字数组排序
来源：http://hz.sweek.top/gthslyivbx.html

[...arr].sort((a, b) => a - b)
来源：http://hz.snrcjt.cn/gtsdeveqox.html

[U91] JS：对象键值遍历
来源：http://hz.zhengqikj.top/gtdnpddpfj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.ppjwa.cn/gtnjiubtxr.html

[U92] JS：深拷贝
来源：http://hz.smart0.xyz/gtjknmopuz.html

structuredClone(obj)
来源：http://hz.jqgfzy.top/gtlgigzupt.html

[U93] JS：模板字符串
来源：http://hz.aibaodan.cn/gtctvizvxv.html

`共 ${n} 条`
来源：http://hz.yanxiufei.cn/gtqhwdzixg.html

[U94] JS：箭头函数
来源：http://hz.daxiang520.top/gtequimunn.html

const double = x => x * 2;
来源：http://hz.jyoumei.cn/gtyqpaipkj.html

[U95] JS：Promise 包装
来源：http://hz.tianlin.xyz/gtgrejweoa.html

new Promise((resolve, reject) => {})
来源：http://hz.hammf.cn/gtwoicbmlw.html

[U96] JS：async/await 与异常
来源：http://hz.cashguo.top/gtjbgojpeq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.tianlin.xyz/gttyqyfpwg.html

[U97] JS：并发请求
来源：http://hz.chenzaomai.com/gtllodwyyt.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinqigfzy.top/gtwdcklbkh.html

[U98] JS：fetch 带 JSON
来源：http://hz.gzhubu.top/gtfobbfuzj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.yj20258888.top/gtqgweobip.html

[U99] JS：事件监听
来源：http://hz.haohaochexian.top/gtsdeojecf.html

el.addEventListener("click", e => {})
来源：http://hz.pycfn.com/gtniauggng.html

[U100] JS：DOM 查询
来源：http://hz.jqgufenzy.top/gtgyyoxcnp.html

document.querySelector(".item")
来源：http://hz.shzxlz.cn/gtahrqvzfl.html

[U101] JS：classList 操作
来源：http://hz.hammf.cn/gtuqxoxqmm.html

el.classList.toggle("active")
来源：http://hz.zhaomingkeji.xyz/gtdewsbzdd.html

[U102] JS：本地存储
来源：http://hz.yangfankeji.com/gtdexstbrz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.andypj.xyz/gtowyyknoa.html

[U103] JS：定时器
来源：http://hz.kuanghao11.cn/gtuvnwdfhu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.9152youxi.cn/gttaatzxle.html

[U104] JS：防抖
来源：http://hz.sufxvd.cn/gthxuiaiab.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhijiandao.cn/gtuimvpfwq.html

[U105] JS：节流
来源：http://hz.fengsongda.top/gtxccztumm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.yvedp.cn/gtgobsfcvn.html

[U106] JS：日期格式化
来源：http://hz.c1oappe.top/gtmneezvkm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.tian-w.cn/gtdokwfhkv.html

[U107] JS：数字千分位
来源：http://hz.feifeiyinyue.top/gthjsrnwmt.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.zhaomingkeji.xyz/gtljtrqqas.html

[U108] JS：随机整数
来源：http://hz.haohaochexian.top/gtylxcuzeb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.yj202588.top/gtsdhldtux.html

[U109] JS：数组分组
来源：http://hz.yvedp.cn/gtfqzegecq.html

Object.groupBy(arr, x => x.type)
来源：http://hz.sysykeji.top/gtzudsmend.html

[U110] JS：数组分块
来源：http://hz.pycfn.com/gtknxsnojn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.bjfxy.top/gtqnpiezke.html

[U111] JS：对象转 Map
来源：http://hz.zhongyouzk.top/gtvszdeuap.html

new Map(Object.entries(obj))
来源：http://hz.aizwys.cn/gtrafxxlqz.html

[U112] JS：字符串补位
来源：http://hz.jyoumei.cn/gtlrbiomvn.html

"7".padStart(3, "0")
来源：http://hz.fengsongda.top/gtziikvovz.html

[U113] JS：正则替换全部
来源：http://hz.xziqi.cn/gtxjoywxqi.html

s.replaceAll("a", "b")
来源：http://hz.yangfankeji.com/gtqlfxbhfk.html

[U114] JS：JSON 深比较
来源：http://hz.ydjk.org.cn/gtgknbeqld.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.cucudq.cn/gtvskjufgz.html

[U115] JS：生成 UUID
来源：http://hz.hnxiangtu.top/gtfywmorbz.html

crypto.randomUUID()
来源：http://hz.ivvv.top/gtkylvplsp.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.ivvv.top/gtdlpgoqet.html

/** @param {string} name */ function f(name) {}
来源：http://hz.ybcxt.top/gtamoeqvpx.html

[U117] JS：单元测试
来源：http://hz.sweek.top/gtbpedwjsa.html

npm i -D vitest;  npx vitest
来源：http://hz.xingfuxueyuan.xyz/gtqwlqyqxu.html

[U118] JS：开发服务器
来源：http://hz.feifeiyinyue.top/gtsdvannew.html

npm i -D vite;  npx vite
来源：http://hz.xziqi.cn/gtwkiwykaf.html

[U119] JS：生产构建
来源：http://hz.tanke756.top/gtvcuybaas.html

npx vite build
来源：http://hz.gzhubu.top/gtkoarowoz.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.zhengqikj.top/gtvoefdicf.html

import.meta.env.VITE_API_URL
来源：http://hz.mhx1999.top/gtdyvrioqx.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtdpgxurmz.html

统计汇总
来源：http://hz.mhx1999.top/gtpbyjqsed.html

================================================================================
来源：http://hz.birdmap.top/gtzrrnozad.html

按语言统计（条）：
来源：http://hz.zhixingplan.top/gtnxfhlyso.html

Python ......... 252
来源：http://hz.ydzc1.top/gthybknlue.html

PHP ............ 252
来源：http://hz.xingfuxueyuan.xyz/gtiaxlrszf.html

JavaScript ..... 252
来源：http://hz.andypj.xyz/gtijtetnpo.html

TypeScript ..... 212
来源：http://hz.cashguo.top/gtoyinroyy.html

Java ........... 212
来源：http://hz.cqqwz.cn/gtojediajw.html

Go ............. 212
来源：http://hz.fengsongda.top/gtnekddzks.html

Ruby ........... 212
来源：http://hz.smart0.xyz/gtxgvzylxi.html

C# ............. 212
来源：http://hz.zhiwuduotai.top/gtvhrzjsdc.html

C .............. 30
来源：http://hz.zhiwuduotai.top/gtxnyaeqpx.html

C++ ............ 30
来源：http://hz.zhixingplan.top/gtczxrupdo.html

SQL ............ 90
来源：http://hz.yuxming.cn/gtpjqexlqm.html

Bash ........... 80
来源：http://hz.jinyuanbaomall.cn/gtjkjdbzoq.html

Kotlin ......... 15
来源：http://hz.hfpthk.cn/gtqpbecxzh.html

Swift .......... 15
来源：http://hz.guannengcc.top/gtkekughuc.html

Lua ............ 10
来源：http://hz.xuanzx.com/gtorjrfyjy.html

Perl ........... 10
来源：http://hz.sxryk.cn/gthnmetdkp.html

Scala .......... 10
来源：http://hz.ydjk.org.cn/gtgnvexrlv.html

------------------------------------
来源：http://hz.gotoacloud.top/gtfbyqwvco.html

合计 ........... 2106 条
来源：http://hz.ivvv.top/gtzjcmizpe.html

按章节统计：
来源：http://hz.shzxlz.cn/gtcoqcfnvq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.tianlin.xyz/gtoedshrmx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.hywenlv.cn/gtpblxhxwe.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.meibo888.top/gtgtmpyxdh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.xuanzx.com/gthshbvgsy.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.zhaomingkeji.xyz/gtdcyiuglo.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.gogol.net.cn/gtxjpgicfk.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.yvedp.cn/gtccogebtk.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.pengpengdd.cyou/gtbevbqtsg.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.nanxinkj.top/gtpfpyudzi.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.316326.xyz/gtmzaxvtxz.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.wangshuangyany.cn/gtoificomb.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.sxryk.cn/gtajhsdsid.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.nwbrower.top/gtmoygzizs.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.svipenyu.cn/gttvmojonj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.zhoulong.xyz/gtagieztvr.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.snrcjt.cn/gtxslthvic.html

Q SQL 专题                              90
来源：http://hz.chenlongwang.top/gtvkmdtgql.html

R Bash 专题                             80
来源：http://hz.gogol.net.cn/gthlvpalac.html

S C / C++ 专题                          60
来源：http://hz.xingfuxueyuan.xyz/gtdzxxlbnl.html

T 其他语言补充                          60
来源：http://hz.gotoacloud.top/gtvfcwsquf.html

U 高频实用片段                         120
来源：http://hz.xingfuxueyuan.xyz/gtysflbbfs.html

------------------------------------
来源：http://hz.pycfn.com/gtqngtxafv.html

合计                                  2106 条
来源：http://hz.xingfuxueyuan.xyz/gtggvxhquz.html

--------------------------------------------------------------------------------
来源：http://hz.xziqi.cn/gtqojziapx.html

使用提醒
来源：http://hz.mhx1999.top/gtjtvvlhth.html

--------------------------------------------------------------------------------
来源：http://hz.yanxiufei.cn/gtgrgdhqxv.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.jinghuilouyu.cn/gttjncfisu.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.zhijiandao.cn/gtgwfufwhd.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.sufxvd.cn/gtfdedjgqw.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.gaohongyu789.top/gtlbdewpok.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.kuanghao11.cn/gtbcnpzsvz.html

—— 文件结束 ——
来源：http://hz.chenjidiqi.icu/gtpqcopwaa.html

================================================================================
来源：http://hz.yanxiufei.cn/gtzxxdfufx.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.sufxvd.cn/gtxqscrfrq.html

Common Programming Examples Cheat Book
来源：http://hz.ehwqpu.com/gtigqlzdgu.html

================================================================================
来源：http://hz.hnqzz.top/gtsdlkybid.html

【收录内容】
来源：http://hz.ehwqpu.com/gtbvqcukza.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.guannengcc.top/gthfvkxpsv.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.yongpay.top/gtuoaelmcj.html

SQL · Bash · C · C++
来源：http://hz.xylfe.cn/gtemeowmto.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.hongshengwenyu.top/gtwfbhejov.html

【使用说明】
来源：http://hz.cashguo.top/gttzvoekpz.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.svipenyu.cn/gtlxafvlrd.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.gzhubu.top/gtulmgpeud.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.bjfxy.top/gtwbkbuldc.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.bjfxy.top/gtmuookesb.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.ybcxt.top/gtlgjudrba.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.gogol.net.cn/gtzwftbsab.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.jqgufenzy.top/gtbdyirvix.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.zdqjudy.top/gtizrzcujv.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.kuanghao11.cn/gtziaypwkt.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.gaohongyu789.top/gtzpwtnyij.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.gzhubu.top/gtcjjtakgj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.jiagoushi.top/gtbiqtziwe.html

【文件统计】
来源：http://hz.ivvv.top/gtmehvowzx.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.gzhubu.top/gtfltpycva.html

--------------------------------------------------------------------------------
来源：http://hz.havefunace.top/gtfxpdugib.html

目  录
来源：http://hz.nwbrower.top/gtsrbxdxre.html

--------------------------------------------------------------------------------
来源：http://hz.haohaochexian.top/gtqfvyxqcx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.iojbl.cn/gtqyeuluey.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.zhoulong.xyz/gtjbcewhdc.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.quarkkingdee.top/gtiwscytnz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.jqgufenzy.top/gtfidrkpbk.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.cdnleiting.top/gtmlmfazvo.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.sufxvd.cn/gtqzjxuexu.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.cashguo.top/gtjlmafgio.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.ivvv.top/gthzgmjivh.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.andypj.xyz/gtatzsewjj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.dashuyun.cn/gtbqjlqiwy.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.aibaodan.cn/gtlpsqfwct.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.hfpthk.cn/gtvcaxfsey.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.snrcjt.cn/gtjdbguqpy.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.xinyue.icu/gtqntvgvgz.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.mhx1999.top/gtphbuishy.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.cashguo.top/gtzqhufiyr.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.haohaochexian.top/gtttxtgool.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.jqgufenzy.top/gtmqwufsmk.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.zhixingplan.top/gtfbxtbdqm.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.guowangkeji.top/gtywttflti.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.ehwqpu.com/gtwfxldbfz.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtmpmvjrrn.html

A. 基础语法与类型
来源：http://hz.daxiang520.top/gtqkcfezca.html

================================================================================
来源：http://hz.mhx1999.top/gtjyxiptzp.html

[A01] Hello World
来源：http://hz.gzhubu.top/gtkugcgfty.html

Py:   print("Hello, World!")
来源：http://hz.hysaishi.cn/gtufnlmmgj.html

PHP:  echo "Hello, World!";
来源：http://hz.chenzaomai.com/gtuleynzep.html

JS:   console.log("Hello, World!");
来源：http://hz.xinyue.icu/gtjhovjwni.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.cucudq.cn/gtzdrxkpgx.html

Java: System.out.println("Hello, World!");
来源：http://hz.daxiang520.top/gtbjayblmp.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.daria6918.cn/gtqowrbeoz.html

Ruby: puts "Hello, World!"
来源：http://hz.316326.xyz/gtvyewfxds.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.nwbrower.top/gtzeelscxw.html

[A02] 变量声明与赋值
来源：http://hz.shangyingyoupin.top/gtnomoufxy.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.hysaishi.cn/gteexhcsws.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.aizwys.cn/gtmdqotqdm.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.daxiang520.top/gteyydeiaa.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.snrcjt.cn/gtkiyopvfg.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.nwbrower.top/gtufsivlvo.html

Go:   name := "Alex"; age := 20
来源：http://hz.jinqigfzy.top/gtuobnhatd.html

Ruby: name = "Alex"; age = 20
来源：http://hz.ydzc1.top/gtzmmgkvoe.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.zhixingplan.top/gtbohtkrxh.html

[A03] 常量定义
来源：http://hz.ivvv.top/gtlrkstvim.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.ivvv.top/gtnjplbxui.html

PHP:  const PI = 3.14159;
来源：http://hz.sweek.top/gtxlbgmavt.html

JS:   const PI = 3.14159;
来源：http://hz.gogol.net.cn/gtemcgkska.html

TS:   const PI: number = 3.14159;
来源：http://hz.yj202588.top/gtqlkgejvy.html

Java: static final double PI = 3.14159;
来源：http://hz.quarkkingdee.top/gtsnckhqsn.html

Go:   const PI = 3.14159
来源：http://hz.sysykeji.top/gtnlsylrwz.html

Ruby: PI = 3.14159
来源：http://hz.9152youxi.cn/gttyphxqpj.html

C#:   const double PI = 3.14159;
来源：http://hz.gzhubu.top/gtgqrofeoq.html

[A04] 判断变量类型
来源：http://hz.nanxuanxn.top/gtyrabkppo.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.hnqzz.top/gtwokbboge.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.hfpthk.cn/gtvmegypar.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.9152youxi.cn/gtkgptyldw.html

TS:   typeof x; x instanceof Date
来源：http://hz.yonumen.top/gtvmbiiisl.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.zhengqikj.top/gtfxxqhvbf.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.gogol.net.cn/gtwijjqcat.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.yuxming.cn/gtqoitvgpv.html

C#:   x.GetType().Name; x is int
来源：http://hz.fengsongda.top/gtllqfmwyb.html

[A05] 整数除法与取模
来源：http://hz.cheryme.top/gtfrhjgtay.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.shuidangran.top/gtsevnipmv.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.xingfuxueyuan.xyz/gtlqrmloao.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.meibo888.top/gtnklwgnjp.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.meibo888.top/gtcilkfssv.html

Java: 7 / 2; 7 % 2
来源：http://hz.yonumen.top/gtdrkkzxrq.html

Go:   7 / 2; 7 % 2
来源：http://hz.ywan-chungtsiang.top/gtpvhdvoii.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.c1oappe.top/gtsieyunkm.html

C#:   7 / 2; 7 % 2
来源：http://hz.gzhubu.top/gtbsmtvytz.html

[A06] 字符串转数字
来源：http://hz.vqdsnc.cn/gthvvobtqx.html

Py:   int("42"); float("3.14")
来源：http://hz.0kj1m.cn/gtcpnclbqx.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.xylfe.cn/gtyodfoaui.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.chenzaomai.com/gtatbimqfe.html


<!-- 参考信息 -->