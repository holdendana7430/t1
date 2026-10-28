代发 wailian999

[U53] PHP：空合并运算符
来源：http://hz.mhx1999.top/gtmnvtvrbz.html

$v = $a ?? $b ?? "default";
来源：http://hz.chenjidiqi.icu/gtuulnqrje.html

[U54] PHP：空安全调用
来源：http://hz.yuanzhike.top/gtaejndoym.html

$obj?->method()
来源：http://hz.yj20258.top/gtjcsjpcdc.html

[U55] PHP：match 表达式
来源：http://hz.feifeiyinyue.top/gtzxarsiqj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.wangshuangyany.cn/gtscqfxiuw.html

[U56] PHP：命名参数
来源：http://hz.meibo888.top/gtdxrvndkv.html

f(a: 1, b: 2)
来源：http://hz.bjfxy.top/gtyampggnn.html

[U57] PHP：字符串插值
来源：http://hz.sweek.top/gtvyrcvqmd.html

"值: {$a}"
来源：http://hz.vqdsnc.cn/gtbtqsnhhi.html

[U58] PHP：数组三件套
来源：http://hz.vqdsnc.cn/gtaolxbkjk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.snrcjt.cn/gtaoelztnr.html

[U59] PHP：自定义排序
来源：http://hz.shangyingyoupin.top/gtuohtcdrf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.haohaochexian.top/gtxuquguak.html

[U60] PHP：JSON 编解码
来源：http://hz.zdqjudy.top/gtyxtuabmg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.yuxming.cn/gtbvrjrqpx.html

[U61] PHP：正则
来源：http://hz.fengsongda.top/gtadxbkepg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.tanke756.top/gtfzfhffyn.html

[U62] PHP：日期对象
来源：http://hz.mhx1999.top/gthghcteqs.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.gaohongyu789.top/gtlbqmomqo.html

[U63] PHP：文件读写
来源：http://hz.shanyushiyangtech.top/gtdxmawrmg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.gotoacloud.top/gtczdqiepc.html

[U64] PHP：目录遍历
来源：http://hz.gogol.net.cn/gtxyzqwqcc.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.quarkkingdee.top/gtdjkxcpqq.html

[U65] PHP：会话
来源：http://hz.yangfankeji.com/gtdphbhoam.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.hysaishi.cn/gtvxkcossq.html

[U66] PHP：设置 Cookie
来源：http://hz.yanxiufei.cn/gtgirtituw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.gotoacloud.top/gtdctntbxo.html

[U67] PHP：处理文件上传
来源：http://hz.jinghuilouyu.cn/gtjchvpjjl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.zhengqikj.top/gtirpvdahn.html

[U68] PHP：PDO 连接
来源：http://hz.nanxinkj.top/gtphbcfeta.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.ehwqpu.com/gttvepvxpv.html

[U69] PHP：PDO 预处理
来源：http://hz.ydzc1.top/gtuvxyzbzc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.zhaomingkeji.xyz/gtoaxxrxkz.html

[U70] PHP：PDO 事务
来源：http://hz.smart0.xyz/gtiiedrhyj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.dashuyun.cn/gtqllbyjiz.html

[U71] PHP：抛出异常
来源：http://hz.fengsongda.top/gtxbhiossj.html

throw new RuntimeException("失败", 500);
来源：http://hz.jyoumei.cn/gtzxzbbmii.html

[U72] PHP：写错误日志
来源：http://hz.shanyushiyangtech.top/gtisvwmnlo.html

error_log("失败: " . $e->getMessage());
来源：http://hz.zhijiandao.cn/gtydibpnjv.html

[U73] PHP：读取 ini 配置
来源：http://hz.vqdsnc.cn/gtiwbglsuv.html

parse_ini_file("config.ini", true)
来源：http://hz.jqgufenzy.top/gtffzpzlrt.html

[U74] PHP：读取环境变量
来源：http://hz.shanyushiyangkeji.top/gthieyirys.html

getenv("APP_ENV") ?: "production"
来源：http://hz.xuanzx.com/gtsslshdpa.html

[U75] PHP：依赖注入
来源：http://hz.zhijiandao.cn/gtnjmplwrf.html

composer require psr/container
来源：http://hz.andypj.xyz/gttwqbmumy.html

[U76] PHP：简单路由
来源：http://hz.fengsongda.top/gtsnkvvmcg.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.jinyuanbaomall.cn/gttrbnyjuo.html

[U77] PHP：模板渲染
来源：http://hz.jyoumei.cn/gtycwlueks.html

composer require twig/twig
来源：http://hz.jlsjyb.cn/gtwrlogvbv.html

[U78] PHP：单元测试
来源：http://hz.fzhhl.top/gtliayjdzy.html

composer require --dev phpunit/phpunit
来源：http://hz.jinqigufen.top/gtmizwabej.html

[U79] PHP：静态分析
来源：http://hz.cdnleiting.top/gthtehvrnd.html

composer require --dev phpstan/phpstan
来源：http://hz.xingfuxueyuan.xyz/gtaowluuhd.html

[U80] PHP：代码规范修复
来源：http://hz.sweek.top/gthfcblyoj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.sxryk.cn/gtmvtpqzis.html

[U81] JS：初始化项目
来源：http://hz.havefunace.top/gtezezatks.html

npm init -y;  npm i express
来源：http://hz.yj202588.top/gtsqxbccga.html

[U82] JS：package.json 脚本
来源：http://hz.pycfn.com/gtifwpmacz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.zhengqikj.top/gtkvnwodii.html

[U83] JS：ES Module 导入导出
来源：http://hz.jiagoushi.top/gtcurwfdns.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.yueranfly.top/gtovutqfji.html

[U84] JS：CommonJS 写法
来源：http://hz.zhijiandao.cn/gthskifsrs.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.yuanzhike.top/gtafteeznr.html

[U85] JS：可选链
来源：http://hz.zhixingplan.top/gtpdicywvw.html

a?.b?.c
来源：http://hz.zhiwuduotai.top/gtgqzbdcpl.html

[U86] JS：空值合并
来源：http://hz.52xcode.cn/gttfzuvkhu.html

a ?? b
来源：http://hz.fengsongda.top/gtrljzlunk.html

[U87] JS：解构默认值
来源：http://hz.jianghu66.top/gtowgcrdjc.html

const { a = 1, b = 2 } = obj;
来源：http://hz.sxryk.cn/gtkgqlcakw.html

[U88] JS：对象展开合并
来源：http://hz.52xcode.cn/gtexxkzbxu.html

{ ...a, ...b }
来源：http://hz.xylfe.cn/gtsnkjogbm.html

[U89] JS：数组去重
来源：http://hz.cashguo.top/gtqdwokijl.html

[...new Set(arr)]
来源：http://hz.shanyushiyangkeji.top/gtwrcwtkma.html

[U90] JS：数字数组排序
来源：http://hz.ivvv.top/gtuulexqvy.html

[...arr].sort((a, b) => a - b)
来源：http://hz.ivvv.top/gtrmclsflf.html

[U91] JS：对象键值遍历
来源：http://hz.chenzaomai.com/gtfizvbguq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.meibo888.top/gtjmikxfsd.html

[U92] JS：深拷贝
来源：http://hz.xylfe.cn/gtygvngnvx.html

structuredClone(obj)
来源：http://hz.gogol.net.cn/gtcivbbeqm.html

[U93] JS：模板字符串
来源：http://hz.sweek.top/gtqhmvfkyi.html

`共 ${n} 条`
来源：http://hz.yvedp.cn/gtasapnmjo.html

[U94] JS：箭头函数
来源：http://hz.fengsongda.top/gtuxcnxzrf.html

const double = x => x * 2;
来源：http://hz.yuxming.cn/gthrbcodgj.html

[U95] JS：Promise 包装
来源：http://hz.tanke756.top/gtasayhfri.html

new Promise((resolve, reject) => {})
来源：http://hz.sufxvd.cn/gtivxskxvw.html

[U96] JS：async/await 与异常
来源：http://hz.ydzc1.top/gtbycaqylz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.yongpay.top/gtcezrqtgi.html

[U97] JS：并发请求
来源：http://hz.hnqzz.top/gtdavxzcue.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinqigfzy.top/gtblydylwa.html

[U98] JS：fetch 带 JSON
来源：http://hz.andypj.xyz/gtxrnrujye.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.bjfxy.top/gtujkbmzdl.html

[U99] JS：事件监听
来源：http://hz.cheryme.top/gtllbafpor.html

el.addEventListener("click", e => {})
来源：http://hz.tanke756.top/gtfcvpdzds.html

[U100] JS：DOM 查询
来源：http://hz.mhx1999.top/gtgfonnocd.html

document.querySelector(".item")
来源：http://hz.hfpthk.cn/gtmzxjofnt.html

[U101] JS：classList 操作
来源：http://hz.shanyushiyangtech.top/gtvccfiehk.html

el.classList.toggle("active")
来源：http://hz.hfpthk.cn/gtiwlcuxqt.html

[U102] JS：本地存储
来源：http://hz.ppjwa.cn/gtjybpuekd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.wangshuangyany.cn/gtfxqrdxav.html

[U103] JS：定时器
来源：http://hz.jlsjyb.cn/gtqdqtzsce.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.hfpthk.cn/gtcjkxyyib.html

[U104] JS：防抖
来源：http://hz.havefunace.top/gtkwnxndku.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhaomingkeji.xyz/gtavuapxzt.html

[U105] JS：节流
来源：http://hz.0kj1m.cn/gtebzagqwp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.dashuyun.cn/gtbfyvefsx.html

[U106] JS：日期格式化
来源：http://hz.yj20258.top/gtwuqsuliy.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yueranfly.top/gtpzcidqrw.html

[U107] JS：数字千分位
来源：http://hz.xylfe.cn/gtropsgbni.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.hysaishi.cn/gtseyeuocd.html

[U108] JS：随机整数
来源：http://hz.ppjwa.cn/gtrtojjpen.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.havefunace.top/gtxckcncii.html

[U109] JS：数组分组
来源：http://hz.sweek.top/gttxycakrp.html

Object.groupBy(arr, x => x.type)
来源：http://hz.ybcxt.top/gtsqqspqpk.html

[U110] JS：数组分块
来源：http://hz.gaohongyu789.top/gttdqdhfbn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.yuanzhike.top/gtmnyfjxbh.html

[U111] JS：对象转 Map
来源：http://hz.sxryk.cn/gtfavoqptg.html

new Map(Object.entries(obj))
来源：http://hz.ydjk.org.cn/gtdculvtfq.html

[U112] JS：字符串补位
来源：http://hz.haohaochexian.top/gtoyyzzsvo.html

"7".padStart(3, "0")
来源：http://hz.jinghuilouyu.cn/gteyabapzk.html

[U113] JS：正则替换全部
来源：http://hz.zycfv.cn/gtdxszpxre.html

s.replaceAll("a", "b")
来源：http://hz.zycfv.cn/gtzuimqnjx.html

[U114] JS：JSON 深比较
来源：http://hz.jiagoushi.top/gtdkmlksin.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.52xcode.cn/gtgiekhztb.html

[U115] JS：生成 UUID
来源：http://hz.iojbl.cn/gtwediskzh.html

crypto.randomUUID()
来源：http://hz.jqgfzy.top/gttnmklmqs.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.fengsongda.top/gticdczkmm.html

/** @param {string} name */ function f(name) {}
来源：http://hz.hfpthk.cn/gthlglphxm.html

[U117] JS：单元测试
来源：http://hz.gaohongyu789.top/gtlnaylkoi.html

npm i -D vitest;  npx vitest
来源：http://hz.gotoacloud.top/gtqoxewsrq.html

[U118] JS：开发服务器
来源：http://hz.aizwys.cn/gtmngbtkqn.html

npm i -D vite;  npx vite
来源：http://hz.cdnleiting.top/gtvdgiuhwt.html

[U119] JS：生产构建
来源：http://hz.zhoulong.xyz/gtbpvafdzs.html

npx vite build
来源：http://hz.jlsjyb.cn/gtszonrvbh.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.chenlongwang.top/gtrensfube.html

import.meta.env.VITE_API_URL
来源：http://hz.zhaomingkeji.xyz/gtreiggroa.html

================================================================================
来源：http://hz.0kj1m.cn/gtppzwemik.html

统计汇总
来源：http://hz.tian-w.cn/gtmeziotko.html

================================================================================
来源：http://hz.shuidangran.top/gtvfbrzkjx.html

按语言统计（条）：
来源：http://hz.zhixingplan.top/gtfskocluz.html

Python ......... 252
来源：http://hz.hammf.cn/gtbjqnaoud.html

PHP ............ 252
来源：http://hz.cucudq.cn/gtcrkjomjq.html

JavaScript ..... 252
来源：http://hz.gzhubu.top/gtmmlpkjma.html

TypeScript ..... 212
来源：http://hz.haohaochexian.top/gtoxrpiyxx.html

Java ........... 212
来源：http://hz.tianlin.xyz/gttrwqlvek.html

Go ............. 212
来源：http://hz.yonumen.top/gtrhfwwetd.html

Ruby ........... 212
来源：http://hz.ivvv.top/gtjtljchnt.html

C# ............. 212
来源：http://hz.cheryme.top/gtpvgjoysx.html

C .............. 30
来源：http://hz.zycfv.cn/gtmzrqkchk.html

C++ ............ 30
来源：http://hz.daxiang520.top/gtgjwgcnef.html

SQL ............ 90
来源：http://hz.chenzaomai.com/gtxoqafjge.html

Bash ........... 80
来源：http://hz.cqqwz.cn/gtavrrlvft.html

Kotlin ......... 15
来源：http://hz.jqgfzy.top/gtyfmcbmjd.html

Swift .......... 15
来源：http://hz.svipenyu.cn/gtivqbmivd.html

Lua ............ 10
来源：http://hz.shanyushiyangtech.top/gtogfkbpzt.html

Perl ........... 10
来源：http://hz.yueranfly.top/gtbiayqmrl.html

Scala .......... 10
来源：http://hz.svipenyu.cn/gtwhwmvcll.html

------------------------------------
来源：http://hz.zhixingplan.top/gtofdfucgw.html

合计 ........... 2106 条
来源：http://hz.9152youxi.cn/gtjpmbuqdt.html

按章节统计：
来源：http://hz.chenjidiqi.icu/gtvxlbgbry.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.xinyue.icu/gtayhueyps.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yvedp.cn/gttdmevkrl.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.shanyushiyangkeji.top/gtdfiyydrg.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.tanke756.top/gtvkmxhwdo.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.sxryk.cn/gtoowvbexz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.fengsongda.top/gtutmraddw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.hnqzz.top/gtzxcyxdhw.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.xziqi.cn/gtayjcmvri.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.yangfankeji.com/gtecdimbvs.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.cashguo.top/gtappoiszi.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.hywenlv.cn/gtgdtghocn.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.nanxinkj.top/gtalnnoyhl.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.jqgufenzy.top/gtatzttdsk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.zdqjudy.top/gtqpweoqvz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.ydzc1.top/gtbwfquobo.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.52xcode.cn/gtragpliii.html

Q SQL 专题                              90
来源：http://hz.jlsjyb.cn/gtujlqivxf.html

R Bash 专题                             80
来源：http://hz.yanxiufei.cn/gtwoigdzkv.html

S C / C++ 专题                          60
来源：http://hz.redwolf501.top/gtsscelrij.html

T 其他语言补充                          60
来源：http://hz.zhongyouzk.top/gttrjhipbc.html

U 高频实用片段                         120
来源：http://hz.tian-w.cn/gthucqeoai.html

------------------------------------
来源：http://hz.svipenyu.cn/gtqfwnvakf.html

合计                                  2106 条
来源：http://hz.jinqigfzy.top/gttkyfpgkt.html

--------------------------------------------------------------------------------
来源：http://hz.cheryme.top/gtrlhjfmvr.html

使用提醒
来源：http://hz.redwolf501.top/gtuhgdijmq.html

--------------------------------------------------------------------------------
来源：http://hz.andypj.xyz/gtncmkhgco.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.hnxiangtu.top/gtxdbhgbls.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.kuanghao11.cn/gtnowokjfg.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.hammf.cn/gtupgdgmfb.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.andypj.xyz/gtnftbdgtx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.tian-w.cn/gtiqxnxyrt.html

—— 文件结束 ——
来源：http://hz.quarkkingdee.top/gtjmjhawrt.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtcraxxitz.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.yvedp.cn/gtpqinnyik.html

Common Programming Examples Cheat Book
来源：http://hz.jqgfzy.top/gtkxhjelmv.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtbefegpwy.html

【收录内容】
来源：http://hz.hysaishi.cn/gtsowmezcn.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.xinyue.icu/gtvvdhkwru.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.cheryme.top/gturhykqmw.html

SQL · Bash · C · C++
来源：http://hz.hongshengwenyu.top/gtncayhsvk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.sxryk.cn/gtnypqyvjt.html

【使用说明】
来源：http://hz.shanyushiyangkeji.top/gtroxdnenk.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.nwbrower.top/gtdoryispc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.chenlongwang.top/gtumgzafpx.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.yuxming.cn/gtyfgqyodj.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.tanke756.top/gtnxvjppnl.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.aizwys.cn/gthpbxckib.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.yj20258888.top/gtiiwgpjfp.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.jianghu66.top/gthllyrptq.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.kuanghao11.cn/gtuwhnofwg.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.fengsongda.top/gtsxznkusp.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.jqgufenzy.top/gtktwudmnd.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.yvedp.cn/gtgzmvbjxa.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.aizwys.cn/gthqgnfddy.html

【文件统计】
来源：http://hz.52xcode.cn/gttjziiogu.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.hongshengwenyu.top/gtxiifzruv.html

--------------------------------------------------------------------------------
来源：http://hz.pycfn.com/gtxgdkliyy.html

目  录
来源：http://hz.c1oappe.top/gtevprnqjm.html

--------------------------------------------------------------------------------
来源：http://hz.iojbl.cn/gtfqielsjf.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.jiagoushi.top/gtnqddmpof.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.mhx1999.top/gtnmhlifqb.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.52xcode.cn/gtzftqwaod.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.jqgfzy.top/gtuwrhxviq.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.dashuyun.cn/gtredpcgev.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.zhongyouzk.top/gtcnuyovad.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.guowangkeji.top/gtyyijsfnz.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.iojbl.cn/gtuhhofbjg.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.feifeiyinyue.top/gtxahuzgtb.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.feifeiyinyue.top/gtksukqnhs.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.chenzaomai.com/gtesnqzkmv.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.cdnleiting.top/gtpydxstyo.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.zhiwuduotai.top/gtggjnzpae.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.yanxiufei.cn/gtxakmojwv.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.jqgfzy.top/gtsslgagum.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.nwbrower.top/gtouawztcx.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.gaohongyu789.top/gtsoqqllbo.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.yangfankeji.com/gtpkvtdrsg.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.zycfv.cn/gtbzzuguks.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.guannengcc.top/gtdihyjuhl.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.cqqwz.cn/gthvmzavxl.html

================================================================================
来源：http://hz.yuxming.cn/gtthmxinou.html

A. 基础语法与类型
来源：http://hz.cashguo.top/gtilgnbrmm.html

================================================================================
来源：http://hz.chenzaomai.com/gtmferarqn.html

[A01] Hello World
来源：http://hz.gotoacloud.top/gtgbtfzjpc.html

Py:   print("Hello, World!")
来源：http://hz.cucudq.cn/gtkfjidvra.html

PHP:  echo "Hello, World!";
来源：http://hz.gotoacloud.top/gtwfprqzqp.html

JS:   console.log("Hello, World!");
来源：http://hz.52xcode.cn/gtzysbbdxh.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.9152youxi.cn/gtexrzqovu.html

Java: System.out.println("Hello, World!");
来源：http://hz.sufxvd.cn/gtazjpnvmw.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.shzxlz.cn/gtrwhghtcg.html

Ruby: puts "Hello, World!"
来源：http://hz.ivvv.top/gtjekxlnnn.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.meibo888.top/gtkvwcocbi.html

[A02] 变量声明与赋值
来源：http://hz.xylfe.cn/gtxicsfddo.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.hongshengwenyu.top/gtxvnzdaoz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.yonumen.top/gtknslpope.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.ydjk.org.cn/gtdvpugpkt.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.tian-w.cn/gtevteuaac.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.yuanzhike.top/gtqbygxjbh.html

Go:   name := "Alex"; age := 20
来源：http://hz.redwolf501.top/gtislxzwnw.html

Ruby: name = "Alex"; age = 20
来源：http://hz.jinghuilouyu.cn/gtpjmxioby.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.jinyuanbaomall.cn/gthlaamqfd.html

[A03] 常量定义
来源：http://hz.mhx1999.top/gtoasrotvg.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.9152youxi.cn/gtmnywfnxq.html

PHP:  const PI = 3.14159;
来源：http://hz.sweek.top/gtkkvwaovk.html

JS:   const PI = 3.14159;
来源：http://hz.andypj.xyz/gtrvggghuw.html

TS:   const PI: number = 3.14159;
来源：http://hz.jinqigfzy.top/gtabuescim.html

Java: static final double PI = 3.14159;
来源：http://hz.dashuyun.cn/gtzxjrsxfs.html

Go:   const PI = 3.14159
来源：http://hz.jqgufenzy.top/gtalodwsvi.html

Ruby: PI = 3.14159
来源：http://hz.bjfxy.top/gtkpebidqk.html

C#:   const double PI = 3.14159;
来源：http://hz.jqgufenzy.top/gtpfbydaez.html

[A04] 判断变量类型
来源：http://hz.ybcxt.top/gtcyoncriw.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.xylfe.cn/gtfpccbgyk.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.zycfv.cn/gtmfdyphxe.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.jlsjyb.cn/gtabzmlxjq.html

TS:   typeof x; x instanceof Date
来源：http://hz.sufxvd.cn/gtyphmafqb.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.hongshengwenyu.top/gtihvmtmwr.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.nanxuanxn.top/gtdfbcpzdi.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.pengpengdd.cyou/gtupsexhsw.html

C#:   x.GetType().Name; x is int
来源：http://hz.daria6918.cn/gtyrkvaphf.html

[A05] 整数除法与取模
来源：http://hz.iojbl.cn/gtcbuhkfra.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.daxiang520.top/gtdinclfeo.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.nanxuanxn.top/gtwtphcmzm.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.316326.xyz/gtfjejghva.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.yj202588.top/gtpmyjrgbs.html

Java: 7 / 2; 7 % 2
来源：http://hz.shuidangran.top/gtxfueunsh.html

Go:   7 / 2; 7 % 2
来源：http://hz.guowangkeji.top/gtranfvjxq.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.nwbrower.top/gtpknuwgkb.html

C#:   7 / 2; 7 % 2
来源：http://hz.hysaishi.cn/gtrehmetfk.html

[A06] 字符串转数字
来源：http://hz.ywan-chungtsiang.top/gtrgokiyca.html

Py:   int("42"); float("3.14")
来源：http://hz.yuanzhike.top/gtebkkoqhi.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.jyoumei.cn/gtgmljammh.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.hfpthk.cn/gtauisjwgx.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.316326.xyz/gtrajikpco.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.xingfuxueyuan.xyz/gtulunathj.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.xuetiantiany.cn/gtlhuhlavc.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.0kj1m.cn/gtdafarsdb.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.quarkkingdee.top/gtdemtbupj.html

[A07] 数字转字符串
来源：http://hz.ydjk.org.cn/gtlxibpjqo.html

Py:   str(42)
来源：http://hz.hfpthk.cn/gtafllubdt.html

PHP:  (string) 42; strval(42)
来源：http://hz.hnqzz.top/gtdcyykxuj.html


<!-- 参考信息 -->