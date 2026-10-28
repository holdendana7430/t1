代发 wailian999

[U53] PHP：空合并运算符
来源：http://hz.xingfuxueyuan.xyz/gtrnpbyfmp.html

$v = $a ?? $b ?? "default";
来源：http://hz.redwolf501.top/gtahcpwadj.html

[U54] PHP：空安全调用
来源：http://hz.nwbrower.top/gtsdrbiagq.html

$obj?->method()
来源：http://hz.cqqwz.cn/gtdsmdgyrg.html

[U55] PHP：match 表达式
来源：http://hz.wangdashe.top/gttbtpcrtx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.iojbl.cn/gtfjywcxjz.html

[U56] PHP：命名参数
来源：http://hz.shzxlz.cn/gtuwynkcef.html

f(a: 1, b: 2)
来源：http://hz.gogol.net.cn/gtlgohqtff.html

[U57] PHP：字符串插值
来源：http://hz.jqgufenzy.top/gtfjbhyonm.html

"值: {$a}"
来源：http://hz.pycfn.com/gtkwpuoevy.html

[U58] PHP：数组三件套
来源：http://hz.nanxinkj.top/gtlzwtgxyr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.hfpthk.cn/gtgjahokth.html

[U59] PHP：自定义排序
来源：http://hz.jyoumei.cn/gtgcfifnwp.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ivvv.top/gtjnqkngkh.html

[U60] PHP：JSON 编解码
来源：http://hz.zhiwuduotai.top/gtnpvutmwc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.gzhubu.top/gttbysjbwa.html

[U61] PHP：正则
来源：http://hz.yvedp.cn/gttcjjjido.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.kuanghao11.cn/gtnwxqffze.html

[U62] PHP：日期对象
来源：http://hz.wangdashe.top/gtdphuqlof.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.jiagoushi.top/gtupktbgwn.html

[U63] PHP：文件读写
来源：http://hz.sysykeji.top/gtkusqpfuv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.chenzaomai.com/gtvbrulovi.html

[U64] PHP：目录遍历
来源：http://hz.shzxlz.cn/gtiskxwiog.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.shangyingyoupin.top/gtigdkzmzz.html

[U65] PHP：会话
来源：http://hz.zhijiandao.cn/gtxydkmrmc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.chenlongwang.top/gtyzmyhzdc.html

[U66] PHP：设置 Cookie
来源：http://hz.fzhhl.top/gtcqayharw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.zhixingplan.top/gtlgdxiirk.html

[U67] PHP：处理文件上传
来源：http://hz.zhongyouzk.top/gtzmjaizyu.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.shzxlz.cn/gtkvafbltk.html

[U68] PHP：PDO 连接
来源：http://hz.havefunace.top/gtokfphxjq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.andypj.xyz/gtgvqlxwew.html

[U69] PHP：PDO 预处理
来源：http://hz.zhengqikj.top/gthduqwqhi.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.jinqigufen.top/gtushzlhrv.html

[U70] PHP：PDO 事务
来源：http://hz.cqqwz.cn/gtmupkxtwu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.jyoumei.cn/gtupchtrhi.html

[U71] PHP：抛出异常
来源：http://hz.pycfn.com/gtqumcublp.html

throw new RuntimeException("失败", 500);
来源：http://hz.birdmap.top/gtlqszejsw.html

[U72] PHP：写错误日志
来源：http://hz.kuanghao11.cn/gtrbhhinzd.html

error_log("失败: " . $e->getMessage());
来源：http://hz.aibaodan.cn/gtsmokaqgi.html

[U73] PHP：读取 ini 配置
来源：http://hz.smart0.xyz/gteltcvvgj.html

parse_ini_file("config.ini", true)
来源：http://hz.yj20258.top/gtrwxxkwyr.html

[U74] PHP：读取环境变量
来源：http://hz.bjfxy.top/gtggyiyadw.html

getenv("APP_ENV") ?: "production"
来源：http://hz.hammf.cn/gtemtqfvfk.html

[U75] PHP：依赖注入
来源：http://hz.haohaochexian.top/gtnkxbyqjz.html

composer require psr/container
来源：http://hz.cqqwz.cn/gtcqkimadg.html

[U76] PHP：简单路由
来源：http://hz.shangyingyoupin.top/gtkrtmvfih.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.yueranfly.top/gtixcvypjn.html

[U77] PHP：模板渲染
来源：http://hz.havefunace.top/gtvqyvboet.html

composer require twig/twig
来源：http://hz.gaohongyu789.top/gtclyjyfew.html

[U78] PHP：单元测试
来源：http://hz.hysaishi.cn/gtayraufou.html

composer require --dev phpunit/phpunit
来源：http://hz.hywenlv.cn/gtdszzvpzf.html

[U79] PHP：静态分析
来源：http://hz.zhongyouzk.top/gtmwpvdswu.html

composer require --dev phpstan/phpstan
来源：http://hz.zhengqikj.top/gtpmqrhnwe.html

[U80] PHP：代码规范修复
来源：http://hz.cashguo.top/gtxejjqsec.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.aibaodan.cn/gttiybafpi.html

[U81] JS：初始化项目
来源：http://hz.jianghu66.top/gtmhfwgbrp.html

npm init -y;  npm i express
来源：http://hz.ydzc1.top/gtosmjitqq.html

[U82] JS：package.json 脚本
来源：http://hz.birdmap.top/gtpdrywzzg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.havefunace.top/gtruvtpgvv.html

[U83] JS：ES Module 导入导出
来源：http://hz.yvedp.cn/gtjkhhkiiq.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.sufxvd.cn/gtksvbtzue.html

[U84] JS：CommonJS 写法
来源：http://hz.mhx1999.top/gtdaegyfai.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.havefunace.top/gtlhlgiemu.html

[U85] JS：可选链
来源：http://hz.shanyushiyangkeji.top/gtxndrwrck.html

a?.b?.c
来源：http://hz.yj20258888.top/gtyqwxywal.html

[U86] JS：空值合并
来源：http://hz.cashguo.top/gtszwcpsgr.html

a ?? b
来源：http://hz.yj202588.top/gtuhgblafm.html

[U87] JS：解构默认值
来源：http://hz.9152youxi.cn/gtvbicjaso.html

const { a = 1, b = 2 } = obj;
来源：http://hz.zhongyouzk.top/gtloygpndk.html

[U88] JS：对象展开合并
来源：http://hz.hnqzz.top/gtelacmsfs.html

{ ...a, ...b }
来源：http://hz.nanxinkj.top/gtckzvswlo.html

[U89] JS：数组去重
来源：http://hz.zhengqikj.top/gtcwjqlwyi.html

[...new Set(arr)]
来源：http://hz.9152youxi.cn/gtoajtifqt.html

[U90] JS：数字数组排序
来源：http://hz.mhx1999.top/gtocaeketn.html

[...arr].sort((a, b) => a - b)
来源：http://hz.0kj1m.cn/gtxpqrqiqv.html

[U91] JS：对象键值遍历
来源：http://hz.pengpengdd.cyou/gtkzgeieov.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.tian-w.cn/gtjgwzzqlf.html

[U92] JS：深拷贝
来源：http://hz.sweek.top/gtvuuvsicg.html

structuredClone(obj)
来源：http://hz.andypj.xyz/gtzwijesmn.html

[U93] JS：模板字符串
来源：http://hz.mhx1999.top/gtfhioyfna.html

`共 ${n} 条`
来源：http://hz.52xcode.cn/gtkqifbbvr.html

[U94] JS：箭头函数
来源：http://hz.ydjk.org.cn/gtpmjoxtuc.html

const double = x => x * 2;
来源：http://hz.jyoumei.cn/gtrydlcvsu.html

[U95] JS：Promise 包装
来源：http://hz.nanxinkj.top/gteehjcjtf.html

new Promise((resolve, reject) => {})
来源：http://hz.birdmap.top/gtynbixjul.html

[U96] JS：async/await 与异常
来源：http://hz.zhijiandao.cn/gtyrmszjsl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.cucudq.cn/gthmkuovud.html

[U97] JS：并发请求
来源：http://hz.shangyingyoupin.top/gtxogcacuo.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhengqikj.top/gthakfibpn.html

[U98] JS：fetch 带 JSON
来源：http://hz.xingfuxueyuan.xyz/gtpvytduor.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.ivvv.top/gtnctjpjxs.html

[U99] JS：事件监听
来源：http://hz.ivvv.top/gtsfyqlkmt.html

el.addEventListener("click", e => {})
来源：http://hz.quarkkingdee.top/gtyjiyvoqj.html

[U100] JS：DOM 查询
来源：http://hz.nanxinkj.top/gtwiouztlh.html

document.querySelector(".item")
来源：http://hz.hongshengwenyu.top/gtbuvqxpux.html

[U101] JS：classList 操作
来源：http://hz.sxryk.cn/gtonnssuuf.html

el.classList.toggle("active")
来源：http://hz.aizwys.cn/gtsdhjsopo.html

[U102] JS：本地存储
来源：http://hz.zhengqikj.top/gtcmncpqvf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.birdmap.top/gteirptkym.html

[U103] JS：定时器
来源：http://hz.sxryk.cn/gtojckrtjf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.gaohongyu789.top/gtnvuwlhsj.html

[U104] JS：防抖
来源：http://hz.hysaishi.cn/gtthyakqfd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yvedp.cn/gtablaylhd.html

[U105] JS：节流
来源：http://hz.andypj.xyz/gtspnsjcrm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.fengsongda.top/gtvfjtpggf.html

[U106] JS：日期格式化
来源：http://hz.ybcxt.top/gtimzulkcv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.zhixingplan.top/gtmlqbygie.html

[U107] JS：数字千分位
来源：http://hz.aibaodan.cn/gtlnamzslz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.gogol.net.cn/gtduznupvc.html

[U108] JS：随机整数
来源：http://hz.zdqjudy.top/gtwpfbjajn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.hammf.cn/gtjycspjmx.html

[U109] JS：数组分组
来源：http://hz.9152youxi.cn/gtnghullms.html

Object.groupBy(arr, x => x.type)
来源：http://hz.guowangkeji.top/gtokbiwpld.html

[U110] JS：数组分块
来源：http://hz.yj20258.top/gtxnwpyene.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.nwbrower.top/gtbcechbns.html

[U111] JS：对象转 Map
来源：http://hz.ehwqpu.com/gtinsqdbpd.html

new Map(Object.entries(obj))
来源：http://hz.zycfv.cn/gtbyvkmbrn.html

[U112] JS：字符串补位
来源：http://hz.jinyuanbaomall.cn/gtblucylua.html

"7".padStart(3, "0")
来源：http://hz.hnqzz.top/gtfskeapcp.html

[U113] JS：正则替换全部
来源：http://hz.haohaochexian.top/gtqaopukla.html

s.replaceAll("a", "b")
来源：http://hz.svipenyu.cn/gtonzmcapi.html

[U114] JS：JSON 深比较
来源：http://hz.zhijiandao.cn/gteyguqaav.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jianghu66.top/gtckumdifv.html

[U115] JS：生成 UUID
来源：http://hz.yj20258888.top/gtpeccwyiv.html

crypto.randomUUID()
来源：http://hz.shzxlz.cn/gtgraeqdjm.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.fengsongda.top/gtmthjmlwo.html

/** @param {string} name */ function f(name) {}
来源：http://hz.jinghuilouyu.cn/gtbaogdnug.html

[U117] JS：单元测试
来源：http://hz.vqdsnc.cn/gtfrgvvdmz.html

npm i -D vitest;  npx vitest
来源：http://hz.hammf.cn/gtwvadituw.html

[U118] JS：开发服务器
来源：http://hz.zhoulong.xyz/gtbhrcuqxv.html

npm i -D vite;  npx vite
来源：http://hz.xuetiantiany.cn/gtrjtxkddm.html

[U119] JS：生产构建
来源：http://hz.chenzaomai.com/gtugwvmken.html

npx vite build
来源：http://hz.jqgufenzy.top/gtusnyjqvw.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.hammf.cn/gtqlhjkeom.html

import.meta.env.VITE_API_URL
来源：http://hz.ywan-chungtsiang.top/gtnoonwfdk.html

================================================================================
来源：http://hz.guowangkeji.top/gtzzuyibnr.html

统计汇总
来源：http://hz.hfpthk.cn/gtrujniekl.html

================================================================================
来源：http://hz.sweek.top/gtmsjtsvvk.html

按语言统计（条）：
来源：http://hz.shzxlz.cn/gtttmxhcer.html

Python ......... 252
来源：http://hz.shanyushiyangtech.top/gtvgourkbb.html

PHP ............ 252
来源：http://hz.bjfxy.top/gtenzpwbvu.html

JavaScript ..... 252
来源：http://hz.9152youxi.cn/gtjugdwryk.html

TypeScript ..... 212
来源：http://hz.hongshengwenyu.top/gtjqdagvvt.html

Java ........... 212
来源：http://hz.cqqwz.cn/gtihfyhphi.html

Go ............. 212
来源：http://hz.yanxiufei.cn/gtwwdlxiei.html

Ruby ........... 212
来源：http://hz.nanxuanxn.top/gtgqccixgv.html

C# ............. 212
来源：http://hz.yueranfly.top/gtkfvxdqrn.html

C .............. 30
来源：http://hz.meibo888.top/gthrlwpibz.html

C++ ............ 30
来源：http://hz.meibo888.top/gtrohjovxw.html

SQL ............ 90
来源：http://hz.shanyushiyangkeji.top/gtiwebuuax.html

Bash ........... 80
来源：http://hz.yonumen.top/gtxcjurryt.html

Kotlin ......... 15
来源：http://hz.jinghuilouyu.cn/gtomhduvun.html

Swift .......... 15
来源：http://hz.pycfn.com/gtzpytpgex.html

Lua ............ 10
来源：http://hz.wangdashe.top/gtosbjkxqm.html

Perl ........... 10
来源：http://hz.316326.xyz/gtbyxtqpus.html

Scala .......... 10
来源：http://hz.hfpthk.cn/gtknhxhwca.html

------------------------------------
来源：http://hz.ybcxt.top/gterayrwxz.html

合计 ........... 2106 条
来源：http://hz.jinyuanbaomall.cn/gtvuwxxjhl.html

按章节统计：
来源：http://hz.xuetiantiany.cn/gtnshftdiz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.zhengqikj.top/gtndqqhnen.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.andypj.xyz/gtghwizzgx.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.yonumen.top/gtdtfqistq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.kuanghao11.cn/gtnhnhhunt.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.chenlongwang.top/gtybdeuchs.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.mhx1999.top/gtqouwyldz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.ehwqpu.com/gtdcdezofv.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.hysaishi.cn/gtkhcdhhox.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.jinqigfzy.top/gtwdyytjdu.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.gotoacloud.top/gtkaltbbrd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.kuanghao11.cn/gtpekyaifl.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.gotoacloud.top/gtrwmhcmrd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.ivvv.top/gtdczxqszi.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.vqdsnc.cn/gtrxynzaxh.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.yuxming.cn/gtglhwrwgm.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.cqqwz.cn/gtbkyrdbyn.html

Q SQL 专题                              90
来源：http://hz.birdmap.top/gtykdnnbhk.html

R Bash 专题                             80
来源：http://hz.xingfuxueyuan.xyz/gtnmomzzbm.html

S C / C++ 专题                          60
来源：http://hz.hfpthk.cn/gtenmthlgy.html

T 其他语言补充                          60
来源：http://hz.hnqzz.top/gtplwghtpu.html

U 高频实用片段                         120
来源：http://hz.zycfv.cn/gtywoxjpvh.html

------------------------------------
来源：http://hz.pengpengdd.cyou/gtdsvrrbpz.html

合计                                  2106 条
来源：http://hz.ivvv.top/gtdyesvbin.html

--------------------------------------------------------------------------------
来源：http://hz.hfpthk.cn/gtarlkdtos.html

使用提醒
来源：http://hz.shanyushiyangkeji.top/gtzcwznjsb.html

--------------------------------------------------------------------------------
来源：http://hz.xziqi.cn/gtphjiosbx.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.hongshengwenyu.top/gtixrzdaro.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.yonumen.top/gtzieolrer.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.xuetiantiany.cn/gtsxkpltba.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.jqgfzy.top/gtxelroqmj.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.wangdashe.top/gtkfcxfhwa.html

—— 文件结束 ——
来源：http://hz.haohaochexian.top/gtwwmfykdf.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gthmcqmprs.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.yongpay.top/gtpdovwauk.html

Common Programming Examples Cheat Book
来源：http://hz.9152youxi.cn/gtnsyicwvc.html

================================================================================
来源：http://hz.yj20258.top/gtlqjbyaga.html

【收录内容】
来源：http://hz.yonumen.top/gtywlavjlz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.c1oappe.top/gtdtcgcbdm.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.feifeiyinyue.top/gtxhahtdgu.html

SQL · Bash · C · C++
来源：http://hz.yueranfly.top/gtspyrffcv.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.ehwqpu.com/gtopcexsdj.html

【使用说明】
来源：http://hz.jinqigfzy.top/gtomnkemjo.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.jlsjyb.cn/gtkqlnrwuj.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.yj20258.top/gtcsvayacj.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.tianlin.xyz/gtinjqdwpw.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.wangdashe.top/gtkmwmmvrb.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.xuetiantiany.cn/gtpsnwmhmp.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.0kj1m.cn/gtciccndzz.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.hywenlv.cn/gtdzlrjtzl.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.jianghu66.top/gtzklhzfjz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.jianghu66.top/gtumcqlqmt.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.cdnleiting.top/gtxizvdjxt.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.daxiang520.top/gtvepiiyll.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.aizwys.cn/gtqjmsrzvz.html

【文件统计】
来源：http://hz.xuetiantiany.cn/gtuomrahdm.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.pengpengdd.cyou/gtjjhpgmks.html

--------------------------------------------------------------------------------
来源：http://hz.jinyuanbaomall.cn/gtvfkuaxhk.html

目  录
来源：http://hz.zdqjudy.top/gtlgkebfjk.html

--------------------------------------------------------------------------------
来源：http://hz.wangdashe.top/gtnwktgtov.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.chenjidiqi.icu/gtnsiphfxo.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.shanyushiyangkeji.top/gtmcxlotpy.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.ivvv.top/gtohjezcyg.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.quarkkingdee.top/gtbobuklud.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.mhx1999.top/gtxknqcoap.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.jinqigufen.top/gthuksirtu.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.jqgufenzy.top/gtqxsnpsqz.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.zhoulong.xyz/gtilfkeyts.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.cucudq.cn/gtklqupxdw.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.shzxlz.cn/gtsmnnsgrd.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.jlsjyb.cn/gtvpmztbrg.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.sweek.top/gthzzoeoja.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.gogol.net.cn/gtochlsypn.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.cheryme.top/gtosjtwxks.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.hnxiangtu.top/gtkujmdkyw.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.jqgfzy.top/gtofsqadkx.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.cdnleiting.top/gtpqcxszml.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.ydjk.org.cn/gtxmprkipg.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.redwolf501.top/gtutbixfad.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.vqdsnc.cn/gtfdlqaspv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.quarkkingdee.top/gtvssjkuhj.html

================================================================================
来源：http://hz.yanxiufei.cn/gtzwicfnnq.html

A. 基础语法与类型
来源：http://hz.dianchejie.cn/gtsiirkmrq.html

================================================================================
来源：http://hz.nwbrower.top/gttxkxvjvi.html

[A01] Hello World
来源：http://hz.xziqi.cn/gtlpveasnj.html

Py:   print("Hello, World!")
来源：http://hz.ywan-chungtsiang.top/gtfxsrwili.html

PHP:  echo "Hello, World!";
来源：http://hz.gzhubu.top/gtcferuerp.html

JS:   console.log("Hello, World!");
来源：http://hz.zhengqikj.top/gtmdausllk.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.yj20258.top/gtaktihgri.html

Java: System.out.println("Hello, World!");
来源：http://hz.zhengqikj.top/gtucodywsf.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.bjfxy.top/gtzqmqafks.html

Ruby: puts "Hello, World!"
来源：http://hz.yuanzhike.top/gtkwuodhng.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.hywenlv.cn/gtcrljnwdj.html

[A02] 变量声明与赋值
来源：http://hz.ybcxt.top/gtwfpkubbb.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.pengpengdd.cyou/gtwvjrhrfv.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.shanyushiyangkeji.top/gthpshcfzw.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.bjfxy.top/gtyoxypyej.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.guannengcc.top/gtixdmxpcz.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.ywan-chungtsiang.top/gtsknqjvnx.html

Go:   name := "Alex"; age := 20
来源：http://hz.zhaomingkeji.xyz/gtzkvddseg.html

Ruby: name = "Alex"; age = 20
来源：http://hz.zhaomingkeji.xyz/gtqquakrbg.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.gogol.net.cn/gtgkefdvms.html

[A03] 常量定义
来源：http://hz.havefunace.top/gtljzxwyur.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.gzhubu.top/gtqgqejfqu.html

PHP:  const PI = 3.14159;
来源：http://hz.chenlongwang.top/gtemtyqcno.html

JS:   const PI = 3.14159;
来源：http://hz.zycfv.cn/gtrytcxzmx.html

TS:   const PI: number = 3.14159;
来源：http://hz.gotoacloud.top/gtzbibyzut.html

Java: static final double PI = 3.14159;
来源：http://hz.jlsjyb.cn/gttpdmrmay.html

Go:   const PI = 3.14159
来源：http://hz.nwbrower.top/gtvjrwrfyz.html

Ruby: PI = 3.14159
来源：http://hz.redwolf501.top/gtwazlzsbg.html

C#:   const double PI = 3.14159;
来源：http://hz.xinyue.icu/gtyhjpjkcs.html

[A04] 判断变量类型
来源：http://hz.hfpthk.cn/gtusdnexws.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.yangfankeji.com/gtavktmvyn.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.jianghu66.top/gtpahkmltw.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.gogol.net.cn/gtdxadmhgw.html

TS:   typeof x; x instanceof Date
来源：http://hz.zhixingplan.top/gtkxutslmy.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.iojbl.cn/gtxjvoftqm.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.dashuyun.cn/gtlziedztb.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.smart0.xyz/gtczfhmddd.html

C#:   x.GetType().Name; x is int
来源：http://hz.shzxlz.cn/gtdfmxgwyd.html

[A05] 整数除法与取模
来源：http://hz.9152youxi.cn/gtavjhfqth.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.andypj.xyz/gtihnffsyj.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.fengsongda.top/gthyxspgzm.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.birdmap.top/gtvgoiravn.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.xinyue.icu/gtadbdejvk.html

Java: 7 / 2; 7 % 2
来源：http://hz.chenjidiqi.icu/gtoimashun.html

Go:   7 / 2; 7 % 2
来源：http://hz.snrcjt.cn/gtgcqshaul.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.feifeiyinyue.top/gthmohjvou.html

C#:   7 / 2; 7 % 2
来源：http://hz.guowangkeji.top/gtfuablygt.html

[A06] 字符串转数字
来源：http://hz.ywan-chungtsiang.top/gtmgfdrvhm.html

Py:   int("42"); float("3.14")
来源：http://hz.yanxiufei.cn/gtagbvlsrs.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.zhoulong.xyz/gtuyshhapp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.fzhhl.top/gtbgpzfjig.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.havefunace.top/gtetkmqryn.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.hnqzz.top/gtxexkqcdk.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.fengsongda.top/gtxisdevud.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.pengpengdd.cyou/gtombctwls.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.tianlin.xyz/gtbuhsincb.html

[A07] 数字转字符串
来源：http://hz.jianghu66.top/gtnsafteql.html

Py:   str(42)
来源：http://hz.cheryme.top/gtwriwbtyp.html

PHP:  (string) 42; strval(42)
来源：http://hz.dianchejie.cn/gtuvkfvcnh.html


<!-- 参考信息 -->