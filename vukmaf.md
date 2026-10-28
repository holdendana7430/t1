代发 wailian999

[U49] PHP：只读属性
来源：http://hz.hammf.cn/gtjaeqsgxq.html

public readonly string $name
来源：http://hz.iojbl.cn/gtxiwtibnd.html

[U50] PHP：构造器属性提升
来源：http://hz.havefunace.top/gthxrqmubs.html

public function __construct(private int $id) {}
来源：http://hz.zhongyouzk.top/gtbuupuzkv.html

[U51] PHP：数组解构
来源：http://hz.jinqigfzy.top/gttepmljty.html

[$a, $b] = $arr;
来源：http://hz.hysaishi.cn/gtshhxpzkb.html

[U52] PHP：箭头函数
来源：http://hz.andypj.xyz/gtpdqvnwuo.html

$double = fn($x) => $x * 2;
来源：http://hz.zdqjudy.top/gtuawiwjnw.html

[U53] PHP：空合并运算符
来源：http://hz.yuxming.cn/gthmkbjabz.html

$v = $a ?? $b ?? "default";
来源：http://hz.sxryk.cn/gtblqbuquu.html

[U54] PHP：空安全调用
来源：http://hz.sweek.top/gtqnqmlocj.html

$obj?->method()
来源：http://hz.hnxiangtu.top/gtdbxpfoss.html

[U55] PHP：match 表达式
来源：http://hz.sweek.top/gtjpgvtfly.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.jianghu66.top/gtpkvswdlg.html

[U56] PHP：命名参数
来源：http://hz.jinyuanbaomall.cn/gtgrctoxpv.html

f(a: 1, b: 2)
来源：http://hz.jqgfzy.top/gtccvyetrg.html

[U57] PHP：字符串插值
来源：http://hz.sweek.top/gtxuywbsue.html

"值: {$a}"
来源：http://hz.ybcxt.top/gtqlozwdls.html

[U58] PHP：数组三件套
来源：http://hz.gotoacloud.top/gtdzwwixfj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.jinyuanbaomall.cn/gtgpzeqrgd.html

[U59] PHP：自定义排序
来源：http://hz.zycfv.cn/gtlptooewh.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.316326.xyz/gthxmusreg.html

[U60] PHP：JSON 编解码
来源：http://hz.shanyushiyangkeji.top/gtrkibynwf.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.tianlin.xyz/gthrsegrem.html

[U61] PHP：正则
来源：http://hz.yongpay.top/gtwbkfibjn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.jinghuilouyu.cn/gtgmjkphub.html

[U62] PHP：日期对象
来源：http://hz.ydzc1.top/gtfeqfsiok.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.ydzc1.top/gtvtzszaxi.html

[U63] PHP：文件读写
来源：http://hz.zhaomingkeji.xyz/gtqtdwlfpu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.jqgufenzy.top/gtkfmukrgb.html

[U64] PHP：目录遍历
来源：http://hz.snrcjt.cn/gtzbuhoevu.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.hnxiangtu.top/gtklqjqyjk.html

[U65] PHP：会话
来源：http://hz.wangdashe.top/gtkyiaiuro.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.wangshuangyany.cn/gtexydrsht.html

[U66] PHP：设置 Cookie
来源：http://hz.iojbl.cn/gtygseujrx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.wangshuangyany.cn/gtatglawwv.html

[U67] PHP：处理文件上传
来源：http://hz.guowangkeji.top/gtlowdikhp.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.ivvv.top/gtdqmgswsv.html

[U68] PHP：PDO 连接
来源：http://hz.yj20258888.top/gtzjtpdkkz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.nanxinkj.top/gtlbjivsgs.html

[U69] PHP：PDO 预处理
来源：http://hz.shuidangran.top/gtvghpupnj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.meibo888.top/gtxqjvnnpb.html

[U70] PHP：PDO 事务
来源：http://hz.zhongyouzk.top/gtzrcdllye.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.jiagoushi.top/gtsmppfxdl.html

[U71] PHP：抛出异常
来源：http://hz.gzhubu.top/gtsdohshet.html

throw new RuntimeException("失败", 500);
来源：http://hz.birdmap.top/gtroyunmod.html

[U72] PHP：写错误日志
来源：http://hz.gotoacloud.top/gtgrysiolh.html

error_log("失败: " . $e->getMessage());
来源：http://hz.zhijiandao.cn/gtjyemdcza.html

[U73] PHP：读取 ini 配置
来源：http://hz.ybcxt.top/gtrmooikwu.html

parse_ini_file("config.ini", true)
来源：http://hz.smart0.xyz/gtwiamuqwe.html

[U74] PHP：读取环境变量
来源：http://hz.smart0.xyz/gtdwwaoflb.html

getenv("APP_ENV") ?: "production"
来源：http://hz.9152youxi.cn/gtqntwcsjc.html

[U75] PHP：依赖注入
来源：http://hz.chenlongwang.top/gtbiuvcrin.html

composer require psr/container
来源：http://hz.xuetiantiany.cn/gtlyuzgjii.html

[U76] PHP：简单路由
来源：http://hz.wangdashe.top/gtbkmhfqnv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.aizwys.cn/gtqqkloesb.html

[U77] PHP：模板渲染
来源：http://hz.cdnleiting.top/gthqgbxhnw.html

composer require twig/twig
来源：http://hz.zhixingplan.top/gtctgrpmcc.html

[U78] PHP：单元测试
来源：http://hz.yj202588.top/gtgnztlpez.html

composer require --dev phpunit/phpunit
来源：http://hz.bjfxy.top/gtktnrwmdd.html

[U79] PHP：静态分析
来源：http://hz.aibaodan.cn/gtkigopntz.html

composer require --dev phpstan/phpstan
来源：http://hz.pengpengdd.cyou/gtmpsdaxhw.html

[U80] PHP：代码规范修复
来源：http://hz.ywan-chungtsiang.top/gtkmxttybz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.hfpthk.cn/gtswsjiekp.html

[U81] JS：初始化项目
来源：http://hz.jlsjyb.cn/gtwljiicds.html

npm init -y;  npm i express
来源：http://hz.cheryme.top/gtrdyynttb.html

[U82] JS：package.json 脚本
来源：http://hz.hammf.cn/gtwxumcyhv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.aibaodan.cn/gtkokvueyp.html

[U83] JS：ES Module 导入导出
来源：http://hz.ydzc1.top/gtkmhjxije.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.jinqigfzy.top/gtsetksydp.html

[U84] JS：CommonJS 写法
来源：http://hz.meibo888.top/gtygxpazul.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.tian-w.cn/gtjssezayo.html

[U85] JS：可选链
来源：http://hz.fzhhl.top/gtmdhlziqh.html

a?.b?.c
来源：http://hz.jinqigufen.top/gtlinqzwxh.html

[U86] JS：空值合并
来源：http://hz.wangdashe.top/gtqrvuyhkf.html

a ?? b
来源：http://hz.birdmap.top/gtainnzbsq.html

[U87] JS：解构默认值
来源：http://hz.tanke756.top/gtugtgcyvk.html

const { a = 1, b = 2 } = obj;
来源：http://hz.andypj.xyz/gtrjvnjzud.html

[U88] JS：对象展开合并
来源：http://hz.0kj1m.cn/gtjyhvscsw.html

{ ...a, ...b }
来源：http://hz.xingfuxueyuan.xyz/gteuflxlsd.html

[U89] JS：数组去重
来源：http://hz.hywenlv.cn/gtulfbgmbj.html

[...new Set(arr)]
来源：http://hz.yj20258.top/gtzhggtkuf.html

[U90] JS：数字数组排序
来源：http://hz.hnxiangtu.top/gtiwargicp.html

[...arr].sort((a, b) => a - b)
来源：http://hz.zhoulong.xyz/gtsflkhefq.html

[U91] JS：对象键值遍历
来源：http://hz.meibo888.top/gtemijjgkd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.shuidangran.top/gtymofuubw.html

[U92] JS：深拷贝
来源：http://hz.hongshengwenyu.top/gttnldgvfj.html

structuredClone(obj)
来源：http://hz.ybcxt.top/gtdqbkvbet.html

[U93] JS：模板字符串
来源：http://hz.xinyue.icu/gtpoyovoav.html

`共 ${n} 条`
来源：http://hz.hysaishi.cn/gtoaxqodsy.html

[U94] JS：箭头函数
来源：http://hz.zhixingplan.top/gtmwxesqqn.html

const double = x => x * 2;
来源：http://hz.shangyingyoupin.top/gtmsuhcbkm.html

[U95] JS：Promise 包装
来源：http://hz.jinqigufen.top/gtduulibhq.html

new Promise((resolve, reject) => {})
来源：http://hz.tian-w.cn/gtmnujfmgt.html

[U96] JS：async/await 与异常
来源：http://hz.nwbrower.top/gtdrlxfnmt.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.zhixingplan.top/gthppwqleo.html

[U97] JS：并发请求
来源：http://hz.9152youxi.cn/gtxnwxmtrt.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhiwuduotai.top/gtuuoccoza.html

[U98] JS：fetch 带 JSON
来源：http://hz.redwolf501.top/gtgjqadlbj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.xuetiantiany.cn/gtrhjxmjec.html

[U99] JS：事件监听
来源：http://hz.wangdashe.top/gtvqaymxde.html

el.addEventListener("click", e => {})
来源：http://hz.jianghu66.top/gtexvjjgpn.html

[U100] JS：DOM 查询
来源：http://hz.yanxiufei.cn/gtaxxxjljz.html

document.querySelector(".item")
来源：http://hz.jlsjyb.cn/gtjwivuhnk.html

[U101] JS：classList 操作
来源：http://hz.zdqjudy.top/gtavshvzxz.html

el.classList.toggle("active")
来源：http://hz.shuidangran.top/gtxrdojigi.html

[U102] JS：本地存储
来源：http://hz.fengsongda.top/gtxcqfjiii.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.fzhhl.top/gtlwwqkoaj.html

[U103] JS：定时器
来源：http://hz.jlsjyb.cn/gtnzcxvsyu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.quarkkingdee.top/gtkwiyfzww.html

[U104] JS：防抖
来源：http://hz.yanxiufei.cn/gtwyhmwkof.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sweek.top/gtaytfffvu.html

[U105] JS：节流
来源：http://hz.yj20258.top/gtgppjbkkr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.hnqzz.top/gtyeexcwcw.html

[U106] JS：日期格式化
来源：http://hz.guannengcc.top/gtnulxhkpv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.ydzc1.top/gtxtvwwads.html

[U107] JS：数字千分位
来源：http://hz.yangfankeji.com/gtxvjshsoy.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.hnxiangtu.top/gtnaidfsbh.html

[U108] JS：随机整数
来源：http://hz.hysaishi.cn/gtohkwnbli.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.shzxlz.cn/gtpclstuqi.html

[U109] JS：数组分组
来源：http://hz.daria6918.cn/gtarycoxur.html

Object.groupBy(arr, x => x.type)
来源：http://hz.feifeiyinyue.top/gtlcfvfgmg.html

[U110] JS：数组分块
来源：http://hz.gaohongyu789.top/gtllygovyw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.chenlongwang.top/gtwsusawco.html

[U111] JS：对象转 Map
来源：http://hz.sysykeji.top/gtjjwjiraz.html

new Map(Object.entries(obj))
来源：http://hz.snrcjt.cn/gtqyodvbgo.html

[U112] JS：字符串补位
来源：http://hz.tian-w.cn/gtjplwrjea.html

"7".padStart(3, "0")
来源：http://hz.zdqjudy.top/gthkjhgzrw.html

[U113] JS：正则替换全部
来源：http://hz.yongpay.top/gtczufjrpi.html

s.replaceAll("a", "b")
来源：http://hz.snrcjt.cn/gtachaczey.html

[U114] JS：JSON 深比较
来源：http://hz.shanyushiyangtech.top/gtbbcpcjsr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.cqqwz.cn/gtphotxfsg.html

[U115] JS：生成 UUID
来源：http://hz.ybcxt.top/gtcsepptiq.html

crypto.randomUUID()
来源：http://hz.wangshuangyany.cn/gtbqzmirtf.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.cheryme.top/gtxfecdams.html

/** @param {string} name */ function f(name) {}
来源：http://hz.guannengcc.top/gtfblchdbq.html

[U117] JS：单元测试
来源：http://hz.sxryk.cn/gtibtcpjki.html

npm i -D vitest;  npx vitest
来源：http://hz.jinqigufen.top/gtpqkmfrlp.html

[U118] JS：开发服务器
来源：http://hz.cheryme.top/gtmnegtutw.html

npm i -D vite;  npx vite
来源：http://hz.yueranfly.top/gtgdeifufk.html

[U119] JS：生产构建
来源：http://hz.kuanghao11.cn/gtzzlmytxf.html

npx vite build
来源：http://hz.nwbrower.top/gtpvgjvljs.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.cashguo.top/gtaruhkoaf.html

import.meta.env.VITE_API_URL
来源：http://hz.pycfn.com/gtdwyesnal.html

================================================================================
来源：http://hz.9152youxi.cn/gtjginvsfs.html

统计汇总
来源：http://hz.jinqigfzy.top/gtomxfhgoh.html

================================================================================
来源：http://hz.ehwqpu.com/gtshknkdmo.html

按语言统计（条）：
来源：http://hz.feifeiyinyue.top/gteygzrukq.html

Python ......... 252
来源：http://hz.jqgufenzy.top/gtadjqhqcx.html

PHP ............ 252
来源：http://hz.shangyingyoupin.top/gtmvdwklro.html

JavaScript ..... 252
来源：http://hz.gzhubu.top/gtgltilxpq.html

TypeScript ..... 212
来源：http://hz.ivvv.top/gtbsgylcxp.html

Java ........... 212
来源：http://hz.gzhubu.top/gthlijjvjg.html

Go ............. 212
来源：http://hz.pengpengdd.cyou/gtpzjgmkzh.html

Ruby ........... 212
来源：http://hz.xziqi.cn/gtudcpldor.html

C# ............. 212
来源：http://hz.cdnleiting.top/gtxkkxbjbk.html

C .............. 30
来源：http://hz.sxryk.cn/gtdysciruw.html

C++ ............ 30
来源：http://hz.jianghu66.top/gtbrfhoaqv.html

SQL ............ 90
来源：http://hz.ywan-chungtsiang.top/gtsgpxewvy.html

Bash ........... 80
来源：http://hz.jqgfzy.top/gtctyhunpa.html

Kotlin ......... 15
来源：http://hz.zhoulong.xyz/gtdozhjbdz.html

Swift .......... 15
来源：http://hz.zhoulong.xyz/gtfysztcyk.html

Lua ............ 10
来源：http://hz.yonumen.top/gtijdujnfr.html

Perl ........... 10
来源：http://hz.xziqi.cn/gtlsnvrymz.html

Scala .......... 10
来源：http://hz.hnxiangtu.top/gtelrqotku.html

------------------------------------
来源：http://hz.nanxuanxn.top/gtmgtihmkg.html

合计 ........... 2106 条
来源：http://hz.gotoacloud.top/gtluezrkog.html

按章节统计：
来源：http://hz.yj20258888.top/gtqnrqgbkq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.chenjidiqi.icu/gtiuutggpb.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.xingfuxueyuan.xyz/gtyryjqznb.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.zhengqikj.top/gtnntesjgj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.cucudq.cn/gtdfrrnfcv.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.pycfn.com/gtidchchzk.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.gzhubu.top/gtdvypqxcr.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.sweek.top/gtpvuxnkef.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.nwbrower.top/gtbsuslhdf.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.sufxvd.cn/gtrmvclsbt.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.daxiang520.top/gtuuivnmcs.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.sysykeji.top/gtpcpjlfey.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.cdnleiting.top/gtmnrivcuj.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.guowangkeji.top/gtqlhsqzqm.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.jianghu66.top/gtxlimwesk.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.xuanzx.com/gtcdjwkikg.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.c1oappe.top/gtqihnhytq.html

Q SQL 专题                              90
来源：http://hz.shuidangran.top/gtkuyoietw.html

R Bash 专题                             80
来源：http://hz.zhijiandao.cn/gtmccsgrac.html

S C / C++ 专题                          60
来源：http://hz.pengpengdd.cyou/gtozofkbqf.html

T 其他语言补充                          60
来源：http://hz.gotoacloud.top/gttyfqqrwo.html

U 高频实用片段                         120
来源：http://hz.tianlin.xyz/gtaouxjywd.html

------------------------------------
来源：http://hz.daria6918.cn/gtbsppozwc.html

合计                                  2106 条
来源：http://hz.tianlin.xyz/gtcekeelmt.html

--------------------------------------------------------------------------------
来源：http://hz.jinqigfzy.top/gtoqtwwkze.html

使用提醒
来源：http://hz.guannengcc.top/gthfkpyiem.html

--------------------------------------------------------------------------------
来源：http://hz.nanxuanxn.top/gtajqhrnqc.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.c1oappe.top/gtlmhwlpga.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.yj202588.top/gtullktlxb.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.0kj1m.cn/gtokmmiwau.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.yuxming.cn/gtfflloryd.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.pycfn.com/gtfogmxksu.html

—— 文件结束 ——
来源：http://hz.daxiang520.top/gtqiwlcins.html

================================================================================
来源：http://hz.52xcode.cn/gtvcxvneif.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.pycfn.com/gtwrtxtyne.html

Common Programming Examples Cheat Book
来源：http://hz.guannengcc.top/gtnnyamxfr.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtpnmabfwt.html

【收录内容】
来源：http://hz.xinyue.icu/gthjpuxsng.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.iojbl.cn/gtybzutean.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.shanyushiyangkeji.top/gtrolbjgzp.html

SQL · Bash · C · C++
来源：http://hz.jqgufenzy.top/gtoicwjzaw.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.guowangkeji.top/gtmbtwfkpe.html

【使用说明】
来源：http://hz.tianlin.xyz/gtmfjbmbzs.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.yj20258888.top/gtfpoveayh.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.guowangkeji.top/gtkvemfyaj.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.meibo888.top/gtacnrlzib.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.zhaomingkeji.xyz/gtblliyblc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.svipenyu.cn/gtzncgdsom.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.havefunace.top/gtcbpyazbx.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.hysaishi.cn/gthlzhergg.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.hongshengwenyu.top/gtyjrdmyxm.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.sxryk.cn/gtyvfueowv.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.shuidangran.top/gtqtrxyuhs.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.chenlongwang.top/gtbmevzjpv.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.yanxiufei.cn/gttfmsrpum.html

【文件统计】
来源：http://hz.jinqigfzy.top/gtaknxsufr.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.tanke756.top/gtwnodeqzq.html

--------------------------------------------------------------------------------
来源：http://hz.xinyue.icu/gtpfnouidf.html

目  录
来源：http://hz.hfpthk.cn/gttfknkrwm.html

--------------------------------------------------------------------------------
来源：http://hz.sysykeji.top/gthhtdysnb.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.jlsjyb.cn/gtqhmryeiz.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.zhixingplan.top/gtaaryurdh.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.gotoacloud.top/gtxrnvelvl.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.gaohongyu789.top/gtyuckpjla.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.yangfankeji.com/gtzvxgzznr.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.gaohongyu789.top/gthnbxcckd.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.shanyushiyangtech.top/gtroewlcop.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.jqgfzy.top/gtriuyfeqm.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.meibo888.top/gtlofnhlhp.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.sufxvd.cn/gtepsfslzj.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.xingfuxueyuan.xyz/gtlkeqxlvc.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.chenjidiqi.icu/gtoxutpqnt.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.zycfv.cn/gtvomeecqa.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.fengsongda.top/gtunstizep.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.vqdsnc.cn/gtszuqnyky.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.havefunace.top/gtgsltxoob.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.fzhhl.top/gtjfkzbtdm.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.bjfxy.top/gtsrzpaeqn.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.shzxlz.cn/gtlfpuitya.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.c1oappe.top/gtjhkoetth.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.shuidangran.top/gtyicyjnxj.html

================================================================================
来源：http://hz.9152youxi.cn/gtjfvvbcew.html

A. 基础语法与类型
来源：http://hz.aizwys.cn/gtqkgualvz.html

================================================================================
来源：http://hz.hywenlv.cn/gtogkltxwt.html

[A01] Hello World
来源：http://hz.sxryk.cn/gtykgvckoc.html

Py:   print("Hello, World!")
来源：http://hz.jinqigufen.top/gtnksicrhh.html

PHP:  echo "Hello, World!";
来源：http://hz.yueranfly.top/gtuzlfxnkp.html

JS:   console.log("Hello, World!");
来源：http://hz.jyoumei.cn/gtfzgujowu.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.zycfv.cn/gtvfwtgsyx.html

Java: System.out.println("Hello, World!");
来源：http://hz.ybcxt.top/gtmiwncrwt.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.gzhubu.top/gtgvwjjpkz.html

Ruby: puts "Hello, World!"
来源：http://hz.yangfankeji.com/gtbqxtltzf.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.birdmap.top/gtlgqwauia.html

[A02] 变量声明与赋值
来源：http://hz.xylfe.cn/gtcyhfzmiu.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.iojbl.cn/gtcdgylgpf.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.shanyushiyangkeji.top/gtlxebetas.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.shanyushiyangkeji.top/gtfyayhfiu.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.tanke756.top/gtbujlpjfg.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.jqgufenzy.top/gtrugudxte.html

Go:   name := "Alex"; age := 20
来源：http://hz.gaohongyu789.top/gtyzjfcjxc.html

Ruby: name = "Alex"; age = 20
来源：http://hz.52xcode.cn/gtpmdriwjw.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.xuetiantiany.cn/gtssavhbse.html

[A03] 常量定义
来源：http://hz.dianchejie.cn/gtjorscocq.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.sysykeji.top/gtohvedfvq.html

PHP:  const PI = 3.14159;
来源：http://hz.zhiwuduotai.top/gtezpcvxef.html

JS:   const PI = 3.14159;
来源：http://hz.zhijiandao.cn/gthekghgxt.html

TS:   const PI: number = 3.14159;
来源：http://hz.shangyingyoupin.top/gtgxdgwwbr.html

Java: static final double PI = 3.14159;
来源：http://hz.zhiwuduotai.top/gtbphtdunh.html

Go:   const PI = 3.14159
来源：http://hz.hammf.cn/gtugtjewmq.html

Ruby: PI = 3.14159
来源：http://hz.sweek.top/gtyijjwlzs.html

C#:   const double PI = 3.14159;
来源：http://hz.xuanzx.com/gtbnabtevl.html

[A04] 判断变量类型
来源：http://hz.iojbl.cn/gtrwiyghiu.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.nwbrower.top/gtxxbengyu.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.shuidangran.top/gtlgusebpe.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.gaohongyu789.top/gthgvtsqjd.html

TS:   typeof x; x instanceof Date
来源：http://hz.ivvv.top/gtkifuojxb.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.fengsongda.top/gtopdvpdlj.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.havefunace.top/gtiximsvyk.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.daxiang520.top/gtndesgeqc.html

C#:   x.GetType().Name; x is int
来源：http://hz.gotoacloud.top/gtxnryuvuu.html

[A05] 整数除法与取模
来源：http://hz.yonumen.top/gtzwsmnuwh.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.jqgfzy.top/gthvgjwrfn.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.cheryme.top/gtozuxlmre.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.yj202588.top/gthjlhgnub.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.yuanzhike.top/gtdjvcuusz.html

Java: 7 / 2; 7 % 2
来源：http://hz.gotoacloud.top/gtrkdrgxqp.html

Go:   7 / 2; 7 % 2
来源：http://hz.smart0.xyz/gtquwndzkt.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.ybcxt.top/gtxslxvzyy.html

C#:   7 / 2; 7 % 2
来源：http://hz.shuidangran.top/gtrsdzxuor.html

[A06] 字符串转数字
来源：http://hz.yuanzhike.top/gtbwyfoimr.html

Py:   int("42"); float("3.14")
来源：http://hz.fzhhl.top/gtzqbqjccv.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.xingfuxueyuan.xyz/gtiahtgkfy.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.shuidangran.top/gtchtnnvcb.html


<!-- 参考信息 -->