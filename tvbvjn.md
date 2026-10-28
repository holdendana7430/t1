代发 wailian999

[U53] PHP：空合并运算符
来源：http://hz.yuanzhike.top/gttjchaimg.html

$v = $a ?? $b ?? "default";
来源：http://hz.hnxiangtu.top/gtrisrgaah.html

[U54] PHP：空安全调用
来源：http://hz.chenlongwang.top/gthyfswufp.html

$obj?->method()
来源：http://hz.havefunace.top/gtnlyxipnl.html

[U55] PHP：match 表达式
来源：http://hz.guannengcc.top/gtvtdpwqhe.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.kuanghao11.cn/gteoyukvbd.html

[U56] PHP：命名参数
来源：http://hz.yuxming.cn/gtinjilcjf.html

f(a: 1, b: 2)
来源：http://hz.chenzaomai.com/gtmantyupz.html

[U57] PHP：字符串插值
来源：http://hz.haohaochexian.top/gttragitoc.html

"值: {$a}"
来源：http://hz.hammf.cn/gtmuwelvdv.html

[U58] PHP：数组三件套
来源：http://hz.gogol.net.cn/gtkghglvgu.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.yuxming.cn/gtrmgdtlap.html

[U59] PHP：自定义排序
来源：http://hz.cdnleiting.top/gtjyeksbqv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.shanyushiyangkeji.top/gtfflitqgk.html

[U60] PHP：JSON 编解码
来源：http://hz.nanxuanxn.top/gtaitedeys.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.yuxming.cn/gtwflszkcx.html

[U61] PHP：正则
来源：http://hz.ybcxt.top/gtxzpxcrzg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.jinghuilouyu.cn/gttidbczxj.html

[U62] PHP：日期对象
来源：http://hz.vqdsnc.cn/gttcumwjmk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.birdmap.top/gtoubnlrzi.html

[U63] PHP：文件读写
来源：http://hz.cdnleiting.top/gtwadtkiyk.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.chenjidiqi.icu/gtwxollyov.html

[U64] PHP：目录遍历
来源：http://hz.wangshuangyany.cn/gtybhlntgo.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.hnxiangtu.top/gtvwfgxwtn.html

[U65] PHP：会话
来源：http://hz.gogol.net.cn/gtdkmuzpnm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.chenlongwang.top/gtqlnlycbm.html

[U66] PHP：设置 Cookie
来源：http://hz.yuanzhike.top/gtsynhiwvr.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.meibo888.top/gteijqbbgw.html

[U67] PHP：处理文件上传
来源：http://hz.wangshuangyany.cn/gtvuxoggbd.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.xuetiantiany.cn/gtnzeteddv.html

[U68] PHP：PDO 连接
来源：http://hz.yj20258888.top/gtdcqiauqm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.xuetiantiany.cn/gtetkdvydj.html

[U69] PHP：PDO 预处理
来源：http://hz.yvedp.cn/gtfqkmvnos.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.yanxiufei.cn/gtbjwhlnrm.html

[U70] PHP：PDO 事务
来源：http://hz.sweek.top/gtjrpytqnu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.xuanzx.com/gtzwjixwcs.html

[U71] PHP：抛出异常
来源：http://hz.snrcjt.cn/gtokskiozn.html

throw new RuntimeException("失败", 500);
来源：http://hz.gotoacloud.top/gtuybjwqnd.html

[U72] PHP：写错误日志
来源：http://hz.ywan-chungtsiang.top/gtchaitgyx.html

error_log("失败: " . $e->getMessage());
来源：http://hz.zycfv.cn/gtpkmkrzct.html

[U73] PHP：读取 ini 配置
来源：http://hz.chenzaomai.com/gtbaawxbfa.html

parse_ini_file("config.ini", true)
来源：http://hz.yj20258.top/gtkcjycnwc.html

[U74] PHP：读取环境变量
来源：http://hz.xziqi.cn/gtizkczgcy.html

getenv("APP_ENV") ?: "production"
来源：http://hz.xuanzx.com/gtfjpcvivp.html

[U75] PHP：依赖注入
来源：http://hz.andypj.xyz/gtykigpjrd.html

composer require psr/container
来源：http://hz.xuanzx.com/gtckuwcfka.html

[U76] PHP：简单路由
来源：http://hz.haohaochexian.top/gteypdmoxp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.sufxvd.cn/gtfvrywefm.html

[U77] PHP：模板渲染
来源：http://hz.tian-w.cn/gtcxditjco.html

composer require twig/twig
来源：http://hz.guowangkeji.top/gtyeqowgdd.html

[U78] PHP：单元测试
来源：http://hz.ydjk.org.cn/gtlwdpbxfj.html

composer require --dev phpunit/phpunit
来源：http://hz.cashguo.top/gtebfglnjo.html

[U79] PHP：静态分析
来源：http://hz.ydjk.org.cn/gtfukcdtuu.html

composer require --dev phpstan/phpstan
来源：http://hz.haohaochexian.top/gtweznwutx.html

[U80] PHP：代码规范修复
来源：http://hz.iojbl.cn/gtaeeubsyl.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.zhoulong.xyz/gthqfroycj.html

[U81] JS：初始化项目
来源：http://hz.yangfankeji.com/gtncpcdatv.html

npm init -y;  npm i express
来源：http://hz.yuxming.cn/gtnhgpwekr.html

[U82] JS：package.json 脚本
来源：http://hz.meibo888.top/gtcbeozocn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.snrcjt.cn/gtsnbhfjyz.html

[U83] JS：ES Module 导入导出
来源：http://hz.xuanzx.com/gtohjelftx.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.shanyushiyangtech.top/gtnitojscr.html

[U84] JS：CommonJS 写法
来源：http://hz.xinyue.icu/gttswepuxd.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.52xcode.cn/gtfciybvdp.html

[U85] JS：可选链
来源：http://hz.zhengqikj.top/gtonytyozg.html

a?.b?.c
来源：http://hz.nanxuanxn.top/gtegparakb.html

[U86] JS：空值合并
来源：http://hz.ivvv.top/gtssiysdva.html

a ?? b
来源：http://hz.0kj1m.cn/gtibucbyte.html

[U87] JS：解构默认值
来源：http://hz.aizwys.cn/gtjnyvnsrz.html

const { a = 1, b = 2 } = obj;
来源：http://hz.ppjwa.cn/gtdnzegvdu.html

[U88] JS：对象展开合并
来源：http://hz.shangyingyoupin.top/gtilgkfjeo.html

{ ...a, ...b }
来源：http://hz.yvedp.cn/gtmgadfxav.html

[U89] JS：数组去重
来源：http://hz.xylfe.cn/gtzozdcbbs.html

[...new Set(arr)]
来源：http://hz.ybcxt.top/gtmzbcazyi.html

[U90] JS：数字数组排序
来源：http://hz.hnqzz.top/gtjmzemsmv.html

[...arr].sort((a, b) => a - b)
来源：http://hz.zycfv.cn/gtkblhgmhy.html

[U91] JS：对象键值遍历
来源：http://hz.redwolf501.top/gtoyawljmm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.ehwqpu.com/gtbettaarm.html

[U92] JS：深拷贝
来源：http://hz.316326.xyz/gtdkohbzgv.html

structuredClone(obj)
来源：http://hz.ydjk.org.cn/gtffzotdug.html

[U93] JS：模板字符串
来源：http://hz.yj202588.top/gtcdwtaqqe.html

`共 ${n} 条`
来源：http://hz.fzhhl.top/gtqkahogtv.html

[U94] JS：箭头函数
来源：http://hz.yuanzhike.top/gtboliavjm.html

const double = x => x * 2;
来源：http://hz.gotoacloud.top/gtosephbbs.html

[U95] JS：Promise 包装
来源：http://hz.zhiwuduotai.top/gtfeucmvqp.html

new Promise((resolve, reject) => {})
来源：http://hz.jinqigfzy.top/gtaadlyyso.html

[U96] JS：async/await 与异常
来源：http://hz.jqgufenzy.top/gtvocuqifg.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.snrcjt.cn/gtgwcsbkwc.html

[U97] JS：并发请求
来源：http://hz.ydjk.org.cn/gtaxcdlaaz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gogol.net.cn/gtfjwxqutp.html

[U98] JS：fetch 带 JSON
来源：http://hz.ydjk.org.cn/gtwkuwrrai.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.pengpengdd.cyou/gtvkmxqdid.html

[U99] JS：事件监听
来源：http://hz.hongshengwenyu.top/gtfkxghcoi.html

el.addEventListener("click", e => {})
来源：http://hz.wangshuangyany.cn/gtbyrkbjxn.html

[U100] JS：DOM 查询
来源：http://hz.jlsjyb.cn/gtctvnsqfy.html

document.querySelector(".item")
来源：http://hz.jqgfzy.top/gthdpvasbt.html

[U101] JS：classList 操作
来源：http://hz.smart0.xyz/gtkwvtmqbp.html

el.classList.toggle("active")
来源：http://hz.meibo888.top/gtrgexgpzd.html

[U102] JS：本地存储
来源：http://hz.tian-w.cn/gtlzpaulmy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.mhx1999.top/gtisurwqks.html

[U103] JS：定时器
来源：http://hz.nwbrower.top/gtudkhkcwb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.chenzaomai.com/gtckadbhrg.html

[U104] JS：防抖
来源：http://hz.shanyushiyangtech.top/gtdxhjtxom.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shzxlz.cn/gtvfrvxevi.html

[U105] JS：节流
来源：http://hz.zhoulong.xyz/gtbmbsolqm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.tanke756.top/gteqmvlahz.html

[U106] JS：日期格式化
来源：http://hz.0kj1m.cn/gtzxkycuih.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.nwbrower.top/gtdsmqinfo.html

[U107] JS：数字千分位
来源：http://hz.shuidangran.top/gtfkjuytnz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.gotoacloud.top/gttomwovja.html

[U108] JS：随机整数
来源：http://hz.aibaodan.cn/gtkqiwpgzu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.cucudq.cn/gtuncfdknj.html

[U109] JS：数组分组
来源：http://hz.yj20258888.top/gtiexuvwet.html

Object.groupBy(arr, x => x.type)
来源：http://hz.shuidangran.top/gtyxzkzynn.html

[U110] JS：数组分块
来源：http://hz.chenjidiqi.icu/gtohjbhqtl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.zhongyouzk.top/gtnylkprzk.html

[U111] JS：对象转 Map
来源：http://hz.ywan-chungtsiang.top/gtnzgdfgpu.html

new Map(Object.entries(obj))
来源：http://hz.chenlongwang.top/gtnhqxhxfv.html

[U112] JS：字符串补位
来源：http://hz.yuxming.cn/gtaddebmua.html

"7".padStart(3, "0")
来源：http://hz.dianchejie.cn/gtzrzjfbwv.html

[U113] JS：正则替换全部
来源：http://hz.chenzaomai.com/gtzzfjmvbd.html

s.replaceAll("a", "b")
来源：http://hz.jiagoushi.top/gtvyqptgre.html

[U114] JS：JSON 深比较
来源：http://hz.zhijiandao.cn/gtyetkdptr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.sxryk.cn/gtchzwyqxr.html

[U115] JS：生成 UUID
来源：http://hz.ehwqpu.com/gtlwhwteqq.html

crypto.randomUUID()
来源：http://hz.yonumen.top/gtbcirfjjj.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.daria6918.cn/gtngcutpvl.html

/** @param {string} name */ function f(name) {}
来源：http://hz.ywan-chungtsiang.top/gtmlpdefho.html

[U117] JS：单元测试
来源：http://hz.jyoumei.cn/gtxbootwyt.html

npm i -D vitest;  npx vitest
来源：http://hz.ywan-chungtsiang.top/gtlvnnuand.html

[U118] JS：开发服务器
来源：http://hz.nanxinkj.top/gtrvzincqy.html

npm i -D vite;  npx vite
来源：http://hz.ivvv.top/gtcwjkcfbk.html

[U119] JS：生产构建
来源：http://hz.sufxvd.cn/gtwlieegqv.html

npx vite build
来源：http://hz.wangshuangyany.cn/gtgyzqdugf.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.gotoacloud.top/gtzawlbrps.html

import.meta.env.VITE_API_URL
来源：http://hz.smart0.xyz/gttpamjdms.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtmbaskens.html

统计汇总
来源：http://hz.shangyingyoupin.top/gtoksdcwyy.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtckglqbea.html

按语言统计（条）：
来源：http://hz.jyoumei.cn/gtipnvyxkw.html

Python ......... 252
来源：http://hz.ydjk.org.cn/gtpbbvioyb.html

PHP ............ 252
来源：http://hz.chenlongwang.top/gtterrfapb.html

JavaScript ..... 252
来源：http://hz.shuidangran.top/gtdmebteaz.html

TypeScript ..... 212
来源：http://hz.dashuyun.cn/gtspdchqvp.html

Java ........... 212
来源：http://hz.feifeiyinyue.top/gtbrpwdafy.html

Go ............. 212
来源：http://hz.snrcjt.cn/gtjiultmvp.html

Ruby ........... 212
来源：http://hz.gaohongyu789.top/gtpksljkdf.html

C# ............. 212
来源：http://hz.daxiang520.top/gtuwqaxgxr.html

C .............. 30
来源：http://hz.dashuyun.cn/gtuntamxix.html

C++ ............ 30
来源：http://hz.sweek.top/gtvxwwjjvs.html

SQL ............ 90
来源：http://hz.yangfankeji.com/gtcmggyuyg.html

Bash ........... 80
来源：http://hz.tian-w.cn/gtssbnbzqd.html

Kotlin ......... 15
来源：http://hz.wangshuangyany.cn/gtjftntiad.html

Swift .......... 15
来源：http://hz.kuanghao11.cn/gtfipfjaxf.html

Lua ............ 10
来源：http://hz.yj20258888.top/gtyurcggxk.html

Perl ........... 10
来源：http://hz.52xcode.cn/gtbmmohfaz.html

Scala .......... 10
来源：http://hz.jqgfzy.top/gtqqkhjgbb.html

------------------------------------
来源：http://hz.shuidangran.top/gtzksbkggl.html

合计 ........... 2106 条
来源：http://hz.jlsjyb.cn/gtolqvnbkh.html

按章节统计：
来源：http://hz.sxryk.cn/gtkmecgyyg.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.wangdashe.top/gtvszardtu.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.vqdsnc.cn/gtcnjvcrez.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.ehwqpu.com/gtwjsqbbbg.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.dianchejie.cn/gttxfhwjmv.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.fzhhl.top/gtfnbyihld.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.zhengqikj.top/gtgsyymnfh.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.feifeiyinyue.top/gtneqtkmzw.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.yanxiufei.cn/gtkhovtvgh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.vqdsnc.cn/gtqjxswghw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.yuanzhike.top/gtorxfwndd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.sysykeji.top/gtkfyvpnug.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.yanxiufei.cn/gtylydfwbf.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.sweek.top/gtqrykzged.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.zhaomingkeji.xyz/gtirqrzonr.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.zhixingplan.top/gtualkbqdo.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.52xcode.cn/gtznctyrmz.html

Q SQL 专题                              90
来源：http://hz.jlsjyb.cn/gtprrgdnvy.html

R Bash 专题                             80
来源：http://hz.xingfuxueyuan.xyz/gtmrxmzfqm.html

S C / C++ 专题                          60
来源：http://hz.bjfxy.top/gtqgymlrek.html

T 其他语言补充                          60
来源：http://hz.xziqi.cn/gtrafoqlyl.html

U 高频实用片段                         120
来源：http://hz.tian-w.cn/gtlkppjecm.html

------------------------------------
来源：http://hz.c1oappe.top/gtnmugskbn.html

合计                                  2106 条
来源：http://hz.hfpthk.cn/gtgztgymvk.html

--------------------------------------------------------------------------------
来源：http://hz.0kj1m.cn/gtjspqsgco.html

使用提醒
来源：http://hz.guannengcc.top/gtqbjeyfnt.html

--------------------------------------------------------------------------------
来源：http://hz.0kj1m.cn/gtjetwrpya.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.jinqigfzy.top/gtjutoxlic.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.hnxiangtu.top/gtayfwvqiy.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.cheryme.top/gtlguwnnod.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.hammf.cn/gtukynhgfr.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.yangfankeji.com/gtpgvnores.html

—— 文件结束 ——
来源：http://hz.mhx1999.top/gtgikckpod.html

================================================================================
来源：http://hz.c1oappe.top/gtzxouoftj.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.mhx1999.top/gtvaoxzjdc.html

Common Programming Examples Cheat Book
来源：http://hz.ehwqpu.com/gtnlthylzf.html

================================================================================
来源：http://hz.fengsongda.top/gtgvwqmuhv.html

【收录内容】
来源：http://hz.jianghu66.top/gtcefhhlkm.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.zhixingplan.top/gtlmszolvg.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.tanke756.top/gtjvihfzah.html

SQL · Bash · C · C++
来源：http://hz.cqqwz.cn/gtdittnaqh.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.xuanzx.com/gtnykjpdrm.html

【使用说明】
来源：http://hz.pengpengdd.cyou/gtdndwnbyl.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.cheryme.top/gtgjkgtdvd.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.zycfv.cn/gtnmmfqcdh.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.fzhhl.top/gthmzvhjye.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.guowangkeji.top/gtagkohxgi.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.hnxiangtu.top/gtlaqcdacn.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.dashuyun.cn/gtyhpvrxjn.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.redwolf501.top/gtqxchnkan.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.yvedp.cn/gthhbmgcip.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.hnqzz.top/gtxbedhitu.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.yangfankeji.com/gtqvupvoqx.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.jianghu66.top/gtultohumn.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.redwolf501.top/gtpqcfcall.html

【文件统计】
来源：http://hz.tanke756.top/gtcinpwdej.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.xuanzx.com/gtfxbhphdd.html

--------------------------------------------------------------------------------
来源：http://hz.gzhubu.top/gtvyogtofz.html

目  录
来源：http://hz.cucudq.cn/gtbdvgobmp.html

--------------------------------------------------------------------------------
来源：http://hz.hongshengwenyu.top/gtodbxozif.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.iojbl.cn/gtjsokxulk.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.chenlongwang.top/gtioydyqpy.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.zhiwuduotai.top/gtxrhbctiy.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.gotoacloud.top/gttjgqluir.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.zhongyouzk.top/gtfjenlavp.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.hnqzz.top/gtuvzjkajm.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.yonumen.top/gtronbabwh.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.ywan-chungtsiang.top/gtbezjgzql.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.0kj1m.cn/gtlvuzwbnb.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.feifeiyinyue.top/gtaglwhupi.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.birdmap.top/gtfhrycptd.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.guannengcc.top/gtcfuuphah.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.wangshuangyany.cn/gtgysybulu.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.iojbl.cn/gthbizngwb.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.yongpay.top/gttfcjsaec.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.havefunace.top/gtwjpiwozi.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.quarkkingdee.top/gtxlepnknt.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.kuanghao11.cn/gtqlxlgubq.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.andypj.xyz/gtflqdvian.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.nanxinkj.top/gtbzfuutxq.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.daria6918.cn/gtbucxoxvp.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtugrklhxc.html

A. 基础语法与类型
来源：http://hz.shanyushiyangtech.top/gtajaioudg.html

================================================================================
来源：http://hz.guannengcc.top/gtoasydhyy.html

[A01] Hello World
来源：http://hz.hfpthk.cn/gtfjgfcbzl.html

Py:   print("Hello, World!")
来源：http://hz.jyoumei.cn/gtquaomnqw.html

PHP:  echo "Hello, World!";
来源：http://hz.zdqjudy.top/gthlhutaxf.html

JS:   console.log("Hello, World!");
来源：http://hz.sysykeji.top/gttznmxnmv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.pengpengdd.cyou/gtijgixlyo.html

Java: System.out.println("Hello, World!");
来源：http://hz.shangyingyoupin.top/gtubkggmhk.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.shuidangran.top/gtamohlcbj.html

Ruby: puts "Hello, World!"
来源：http://hz.feifeiyinyue.top/gtildtaumq.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.gzhubu.top/gtnjuzvsdf.html

[A02] 变量声明与赋值
来源：http://hz.guannengcc.top/gtrqeaxywf.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.zhoulong.xyz/gtifkqblyv.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.fzhhl.top/gtfyjxkbmb.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.sxryk.cn/gthtturwiv.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.c1oappe.top/gtjukynobn.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.shanyushiyangkeji.top/gtffcshcaw.html

Go:   name := "Alex"; age := 20
来源：http://hz.havefunace.top/gtwhvhqhpp.html

Ruby: name = "Alex"; age = 20
来源：http://hz.yj20258.top/gtqglmfswk.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.cdnleiting.top/gtxucucfwv.html

[A03] 常量定义
来源：http://hz.jlsjyb.cn/gtymzcfazh.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.hfpthk.cn/gtxrdtrktl.html

PHP:  const PI = 3.14159;
来源：http://hz.jianghu66.top/gtykjwkwov.html

JS:   const PI = 3.14159;
来源：http://hz.316326.xyz/gtjttxuloa.html

TS:   const PI: number = 3.14159;
来源：http://hz.jqgfzy.top/gttednujov.html

Java: static final double PI = 3.14159;
来源：http://hz.zhoulong.xyz/gtjsirydml.html

Go:   const PI = 3.14159
来源：http://hz.shanyushiyangtech.top/gtnpxjsjvx.html

Ruby: PI = 3.14159
来源：http://hz.yj20258.top/gtivsyipnd.html

C#:   const double PI = 3.14159;
来源：http://hz.andypj.xyz/gtjxvazakn.html

[A04] 判断变量类型
来源：http://hz.ehwqpu.com/gtivthquuc.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.aizwys.cn/gtfouefnuf.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.mhx1999.top/gtdwxoqkxx.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.daxiang520.top/gtwntyctuf.html

TS:   typeof x; x instanceof Date
来源：http://hz.guowangkeji.top/gtiedpglvt.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.sufxvd.cn/gtfydtepls.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.iojbl.cn/gtdhkzwugq.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.jqgufenzy.top/gteorjnklu.html

C#:   x.GetType().Name; x is int
来源：http://hz.yonumen.top/gtcveqkddp.html

[A05] 整数除法与取模
来源：http://hz.hywenlv.cn/gtzhondvvv.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.quarkkingdee.top/gthnjcrkip.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.shanyushiyangtech.top/gtneyhonin.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.chenlongwang.top/gtozjqguny.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.vqdsnc.cn/gthinyemmv.html

Java: 7 / 2; 7 % 2
来源：http://hz.hywenlv.cn/gtzpmnvanp.html

Go:   7 / 2; 7 % 2
来源：http://hz.gotoacloud.top/gtwpodgtmf.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.cashguo.top/gtuelfajxh.html

C#:   7 / 2; 7 % 2
来源：http://hz.pycfn.com/gtgbtqhwjf.html

[A06] 字符串转数字
来源：http://hz.ppjwa.cn/gtlxakbwej.html

Py:   int("42"); float("3.14")
来源：http://hz.tanke756.top/gttxzlotkd.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.chenzaomai.com/gteiphhjct.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.yueranfly.top/gtviffcwdl.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.guannengcc.top/gtpyhbrpmz.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.zhiwuduotai.top/gtvkhdrdyf.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.jinqigfzy.top/gtgncotboy.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.nanxinkj.top/gtpjrtsdpe.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.tanke756.top/gtgwbvlgmw.html

[A07] 数字转字符串
来源：http://hz.ybcxt.top/gtridxohya.html

Py:   str(42)
来源：http://hz.sufxvd.cn/gtgnqznvvq.html

PHP:  (string) 42; strval(42)
来源：http://hz.ywan-chungtsiang.top/gtnqdkuwia.html


<!-- 参考信息 -->