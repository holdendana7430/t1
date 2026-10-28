代发 wailian999

[U47] PHP：联合类型
来源：http://hz.yvedp.cn/gtbqpvbauw.html

int|string $id
来源：http://hz.zhixingplan.top/gtjbnwoaoo.html

[U48] PHP：纯枚举
来源：http://hz.9152youxi.cn/gtvogdlryt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.nanxinkj.top/gtnndhzmkf.html

[U49] PHP：只读属性
来源：http://hz.zycfv.cn/gtoksxtsqj.html

public readonly string $name
来源：http://hz.ybcxt.top/gtljchhgwd.html

[U50] PHP：构造器属性提升
来源：http://hz.yanxiufei.cn/gtacaqaszz.html

public function __construct(private int $id) {}
来源：http://hz.svipenyu.cn/gtzvtippmt.html

[U51] PHP：数组解构
来源：http://hz.hammf.cn/gtlccirzje.html

[$a, $b] = $arr;
来源：http://hz.yueranfly.top/gtlaqxtswy.html

[U52] PHP：箭头函数
来源：http://hz.jianghu66.top/gtaudyjctj.html

$double = fn($x) => $x * 2;
来源：http://hz.nanxinkj.top/gtkicygrpw.html

[U53] PHP：空合并运算符
来源：http://hz.316326.xyz/gtkgackaum.html

$v = $a ?? $b ?? "default";
来源：http://hz.svipenyu.cn/gtqmngqnzr.html

[U54] PHP：空安全调用
来源：http://hz.sysykeji.top/gtavnqwjnx.html

$obj?->method()
来源：http://hz.hnxiangtu.top/gthtvvejxq.html

[U55] PHP：match 表达式
来源：http://hz.ywan-chungtsiang.top/gtpqbekqrp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.shanyushiyangkeji.top/gtioiyulxp.html

[U56] PHP：命名参数
来源：http://hz.wangshuangyany.cn/gtfcjbotra.html

f(a: 1, b: 2)
来源：http://hz.xylfe.cn/gtvjchrlbv.html

[U57] PHP：字符串插值
来源：http://hz.yvedp.cn/gtpisacwgq.html

"值: {$a}"
来源：http://hz.316326.xyz/gtpmbhtpxu.html

[U58] PHP：数组三件套
来源：http://hz.cqqwz.cn/gtytmcrjah.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.jiagoushi.top/gtdtirtxbz.html

[U59] PHP：自定义排序
来源：http://hz.sysykeji.top/gtyzjnbzdv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.shanyushiyangtech.top/gtupirjwgs.html

[U60] PHP：JSON 编解码
来源：http://hz.ybcxt.top/gtxkwgelyl.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.yj20258888.top/gtahkaahgj.html

[U61] PHP：正则
来源：http://hz.ywan-chungtsiang.top/gtzubwgkop.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.mhx1999.top/gtxewlsdzp.html

[U62] PHP：日期对象
来源：http://hz.c1oappe.top/gtrtmuqrvo.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.svipenyu.cn/gtzflgyqdj.html

[U63] PHP：文件读写
来源：http://hz.nanxinkj.top/gtmawyvddu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.0kj1m.cn/gtqonkcvnt.html

[U64] PHP：目录遍历
来源：http://hz.tianlin.xyz/gtkfmumjkf.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.snrcjt.cn/gtcyputfru.html

[U65] PHP：会话
来源：http://hz.ydzc1.top/gtdwuhmfyp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.shuidangran.top/gtjwirwebh.html

[U66] PHP：设置 Cookie
来源：http://hz.xziqi.cn/gtrsajiqlu.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.52xcode.cn/gtosipukxj.html

[U67] PHP：处理文件上传
来源：http://hz.xuetiantiany.cn/gtwdbsppsj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.yanxiufei.cn/gtgwxkfmvh.html

[U68] PHP：PDO 连接
来源：http://hz.jianghu66.top/gtaocssnns.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.hysaishi.cn/gtgayapyts.html

[U69] PHP：PDO 预处理
来源：http://hz.cdnleiting.top/gtzuscnons.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.cqqwz.cn/gtjoyofxwg.html

[U70] PHP：PDO 事务
来源：http://hz.xziqi.cn/gtlfwuwpan.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.shuidangran.top/gthdrhxlpd.html

[U71] PHP：抛出异常
来源：http://hz.jyoumei.cn/gtjdbznpbk.html

throw new RuntimeException("失败", 500);
来源：http://hz.yuanzhike.top/gtgumcuisx.html

[U72] PHP：写错误日志
来源：http://hz.9152youxi.cn/gtitfarwvi.html

error_log("失败: " . $e->getMessage());
来源：http://hz.ywan-chungtsiang.top/gtfzenlwzf.html

[U73] PHP：读取 ini 配置
来源：http://hz.bjfxy.top/gtmriwsqti.html

parse_ini_file("config.ini", true)
来源：http://hz.zhaomingkeji.xyz/gtwxoalbrd.html

[U74] PHP：读取环境变量
来源：http://hz.nwbrower.top/gttoiqntdp.html

getenv("APP_ENV") ?: "production"
来源：http://hz.mhx1999.top/gtwkyhwwrz.html

[U75] PHP：依赖注入
来源：http://hz.vqdsnc.cn/gtybappppm.html

composer require psr/container
来源：http://hz.yuxming.cn/gtunsxdflm.html

[U76] PHP：简单路由
来源：http://hz.chenzaomai.com/gtcwbkljej.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.fzhhl.top/gtjspljtru.html

[U77] PHP：模板渲染
来源：http://hz.jinyuanbaomall.cn/gtrsugoyqx.html

composer require twig/twig
来源：http://hz.ybcxt.top/gtyvcwkyfu.html

[U78] PHP：单元测试
来源：http://hz.shanyushiyangkeji.top/gtnvkecflq.html

composer require --dev phpunit/phpunit
来源：http://hz.vqdsnc.cn/gtjosvzjtj.html

[U79] PHP：静态分析
来源：http://hz.bjfxy.top/gtfbpsagsy.html

composer require --dev phpstan/phpstan
来源：http://hz.0kj1m.cn/gtwmqhgecf.html

[U80] PHP：代码规范修复
来源：http://hz.chenlongwang.top/gttenmnihw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.pengpengdd.cyou/gtaswyntmr.html

[U81] JS：初始化项目
来源：http://hz.chenzaomai.com/gtdmqyweot.html

npm init -y;  npm i express
来源：http://hz.dashuyun.cn/gtcsddquwe.html

[U82] JS：package.json 脚本
来源：http://hz.zhengqikj.top/gtljuxcuor.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.xingfuxueyuan.xyz/gtubnuirtm.html

[U83] JS：ES Module 导入导出
来源：http://hz.daria6918.cn/gticontqxx.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.9152youxi.cn/gtvresguvc.html

[U84] JS：CommonJS 写法
来源：http://hz.tianlin.xyz/gtjgbwlscb.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.chenlongwang.top/gtcboqzorm.html

[U85] JS：可选链
来源：http://hz.cheryme.top/gtldchlsnu.html

a?.b?.c
来源：http://hz.zhaomingkeji.xyz/gtgknwlptn.html

[U86] JS：空值合并
来源：http://hz.gzhubu.top/gtdtdfxvdm.html

a ?? b
来源：http://hz.zhiwuduotai.top/gtufskuyga.html

[U87] JS：解构默认值
来源：http://hz.chenlongwang.top/gtailbwlyr.html

const { a = 1, b = 2 } = obj;
来源：http://hz.guowangkeji.top/gtwfnuzbrc.html

[U88] JS：对象展开合并
来源：http://hz.sweek.top/gtnvlbqjvh.html

{ ...a, ...b }
来源：http://hz.jiagoushi.top/gtdfnzavzs.html

[U89] JS：数组去重
来源：http://hz.sweek.top/gtsrqmfers.html

[...new Set(arr)]
来源：http://hz.shanyushiyangkeji.top/gtqvwdzvzk.html

[U90] JS：数字数组排序
来源：http://hz.zhaomingkeji.xyz/gtpjflpcdc.html

[...arr].sort((a, b) => a - b)
来源：http://hz.yj202588.top/gtqfinbhwl.html

[U91] JS：对象键值遍历
来源：http://hz.zhijiandao.cn/gtqkglpgwe.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.hywenlv.cn/gtcxzxedzj.html

[U92] JS：深拷贝
来源：http://hz.hfpthk.cn/gtxhrqxwge.html

structuredClone(obj)
来源：http://hz.gogol.net.cn/gtitmrralw.html

[U93] JS：模板字符串
来源：http://hz.jqgfzy.top/gtmkvsbzmv.html

`共 ${n} 条`
来源：http://hz.sufxvd.cn/gteqbyeyzx.html

[U94] JS：箭头函数
来源：http://hz.xylfe.cn/gtzynmruzu.html

const double = x => x * 2;
来源：http://hz.fengsongda.top/gthhgnrkrf.html

[U95] JS：Promise 包装
来源：http://hz.0kj1m.cn/gtqtcehurh.html

new Promise((resolve, reject) => {})
来源：http://hz.andypj.xyz/gtqacdoter.html

[U96] JS：async/await 与异常
来源：http://hz.jyoumei.cn/gtsnzqxkuf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.tian-w.cn/gttqqncskk.html

[U97] JS：并发请求
来源：http://hz.shanyushiyangtech.top/gtusyuxjbp.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yongpay.top/gtrxwpkbfi.html

[U98] JS：fetch 带 JSON
来源：http://hz.feifeiyinyue.top/gtfewcgkir.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.daxiang520.top/gtlkrtvgjo.html

[U99] JS：事件监听
来源：http://hz.yanxiufei.cn/gtlyyehxbe.html

el.addEventListener("click", e => {})
来源：http://hz.0kj1m.cn/gttcgvnxfu.html

[U100] JS：DOM 查询
来源：http://hz.xziqi.cn/gtsldmswph.html

document.querySelector(".item")
来源：http://hz.yj202588.top/gtgzeafxmw.html

[U101] JS：classList 操作
来源：http://hz.snrcjt.cn/gtkocmbaaj.html

el.classList.toggle("active")
来源：http://hz.meibo888.top/gtnoxyrpqa.html

[U102] JS：本地存储
来源：http://hz.jinyuanbaomall.cn/gtcsxgfevp.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.xylfe.cn/gttzevazlx.html

[U103] JS：定时器
来源：http://hz.chenjidiqi.icu/gteeaxilam.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.sxryk.cn/gtjavvlmrj.html

[U104] JS：防抖
来源：http://hz.haohaochexian.top/gtaugnxgbs.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.smart0.xyz/gtnqabpnil.html

[U105] JS：节流
来源：http://hz.zhiwuduotai.top/gtwaqgjrkl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.svipenyu.cn/gtiqtobwjm.html

[U106] JS：日期格式化
来源：http://hz.zhixingplan.top/gtsifvqqzc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.fzhhl.top/gtinlkeqoc.html

[U107] JS：数字千分位
来源：http://hz.jinqigufen.top/gtafgxkird.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.guowangkeji.top/gtisrjlicm.html

[U108] JS：随机整数
来源：http://hz.shanyushiyangkeji.top/gtbysbzcew.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.jinyuanbaomall.cn/gtowoiregu.html

[U109] JS：数组分组
来源：http://hz.jinqigfzy.top/gtxokaajdr.html

Object.groupBy(arr, x => x.type)
来源：http://hz.yj20258888.top/gtcbjimahi.html

[U110] JS：数组分块
来源：http://hz.jiagoushi.top/gtraifwijq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.cdnleiting.top/gtpljyhdov.html

[U111] JS：对象转 Map
来源：http://hz.cheryme.top/gtdlhbqdmu.html

new Map(Object.entries(obj))
来源：http://hz.nanxuanxn.top/gtctbgpmft.html

[U112] JS：字符串补位
来源：http://hz.jyoumei.cn/gtokevoxle.html

"7".padStart(3, "0")
来源：http://hz.gogol.net.cn/gtbsgtgtwc.html

[U113] JS：正则替换全部
来源：http://hz.andypj.xyz/gtdixwoinu.html

s.replaceAll("a", "b")
来源：http://hz.daxiang520.top/gtjnzshljr.html

[U114] JS：JSON 深比较
来源：http://hz.nanxinkj.top/gtlonkqixu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jqgfzy.top/gtuzzclulh.html

[U115] JS：生成 UUID
来源：http://hz.guannengcc.top/gtedfhaacf.html

crypto.randomUUID()
来源：http://hz.daxiang520.top/gteoewrumc.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.yuanzhike.top/gtizacwgqp.html

/** @param {string} name */ function f(name) {}
来源：http://hz.ehwqpu.com/gtohlbrepi.html

[U117] JS：单元测试
来源：http://hz.daria6918.cn/gtdkjqxznp.html

npm i -D vitest;  npx vitest
来源：http://hz.ehwqpu.com/gtqkbxhnnn.html

[U118] JS：开发服务器
来源：http://hz.sufxvd.cn/gtlmhsvlli.html

npm i -D vite;  npx vite
来源：http://hz.meibo888.top/gtnbyskdcy.html

[U119] JS：生产构建
来源：http://hz.9152youxi.cn/gtcdqwpsqp.html

npx vite build
来源：http://hz.c1oappe.top/gtupkufxrb.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.yj20258.top/gtzrjqjybu.html

import.meta.env.VITE_API_URL
来源：http://hz.pengpengdd.cyou/gtfnntoxht.html

================================================================================
来源：http://hz.chenzaomai.com/gtrdimvise.html

统计汇总
来源：http://hz.jinqigufen.top/gtjwxbwxyg.html

================================================================================
来源：http://hz.cqqwz.cn/gtsjgwghxn.html

按语言统计（条）：
来源：http://hz.jlsjyb.cn/gtbcluqoow.html

Python ......... 252
来源：http://hz.yj20258888.top/gtlxifhemz.html

PHP ............ 252
来源：http://hz.zhoulong.xyz/gtbepvbqpn.html

JavaScript ..... 252
来源：http://hz.xuanzx.com/gthcqxazta.html

TypeScript ..... 212
来源：http://hz.redwolf501.top/gtotxrabkx.html

Java ........... 212
来源：http://hz.kuanghao11.cn/gtbekajzgh.html

Go ............. 212
来源：http://hz.zhongyouzk.top/gtsolvkvzd.html

Ruby ........... 212
来源：http://hz.nanxuanxn.top/gtmnyffyyj.html

C# ............. 212
来源：http://hz.chenlongwang.top/gtsrqhkdwi.html

C .............. 30
来源：http://hz.hywenlv.cn/gtbepsofdn.html

C++ ............ 30
来源：http://hz.jqgfzy.top/gtqncyueky.html

SQL ............ 90
来源：http://hz.xziqi.cn/gtidycpycr.html

Bash ........... 80
来源：http://hz.havefunace.top/gtqwgprpys.html

Kotlin ......... 15
来源：http://hz.jlsjyb.cn/gtazlgzyqx.html

Swift .......... 15
来源：http://hz.daxiang520.top/gtkecsqyjj.html

Lua ............ 10
来源：http://hz.yueranfly.top/gtgsymiyvc.html

Perl ........... 10
来源：http://hz.haohaochexian.top/gtopxzxonh.html

Scala .......... 10
来源：http://hz.yanxiufei.cn/gtlhurdnqz.html

------------------------------------
来源：http://hz.xuanzx.com/gtmhuirhwg.html

合计 ........... 2106 条
来源：http://hz.cucudq.cn/gtalnujqlu.html

按章节统计：
来源：http://hz.quarkkingdee.top/gttcrwiupx.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.aibaodan.cn/gtpjbervrc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.ivvv.top/gtxdndhqfo.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.gogol.net.cn/gtpkdtples.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.shuidangran.top/gtetcmmboo.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.zhengqikj.top/gtplzdlrsy.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.ivvv.top/gtyynenijd.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.bjfxy.top/gtnzxhfpju.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.zhixingplan.top/gtqgpgocyu.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.jinqigfzy.top/gtdredxshf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.yj20258888.top/gtnhcdrwjd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.nanxuanxn.top/gturryvack.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.mhx1999.top/gthcbuhxcr.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.yongpay.top/gtfdeaotiq.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.zdqjudy.top/gtyngwmvzv.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.zhiwuduotai.top/gtybniqukk.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.jiagoushi.top/gtbbohkksg.html

Q SQL 专题                              90
来源：http://hz.hfpthk.cn/gtmzzwytvy.html

R Bash 专题                             80
来源：http://hz.xuanzx.com/gtqzioujyn.html

S C / C++ 专题                          60
来源：http://hz.jianghu66.top/gtxmegrxes.html

T 其他语言补充                          60
来源：http://hz.hongshengwenyu.top/gtwdcjedhr.html

U 高频实用片段                         120
来源：http://hz.shangyingyoupin.top/gtyimthety.html

------------------------------------
来源：http://hz.zhaomingkeji.xyz/gtoguzklno.html

合计                                  2106 条
来源：http://hz.yj20258888.top/gtpwvcscul.html

--------------------------------------------------------------------------------
来源：http://hz.daxiang520.top/gtqlobkhfn.html

使用提醒
来源：http://hz.bjfxy.top/gtwnujkoir.html

--------------------------------------------------------------------------------
来源：http://hz.shzxlz.cn/gtbmnyualm.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.hnqzz.top/gtwtvwmfvk.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.cqqwz.cn/gtoohqjcoy.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.yonumen.top/gtcsasbrlo.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.jianghu66.top/gtiaefbanp.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.vqdsnc.cn/gtvpyxnrxc.html

—— 文件结束 ——
来源：http://hz.hammf.cn/gtziqyfcds.html

================================================================================
来源：http://hz.52xcode.cn/gtwhdkovpc.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.wangdashe.top/gtooektead.html

Common Programming Examples Cheat Book
来源：http://hz.jqgufenzy.top/gtafmqbxyg.html

================================================================================
来源：http://hz.quarkkingdee.top/gtfmuyubuu.html

【收录内容】
来源：http://hz.shanyushiyangkeji.top/gtjcibdipu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.xinyue.icu/gtjhgudiso.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.ppjwa.cn/gticbfunsb.html

SQL · Bash · C · C++
来源：http://hz.yvedp.cn/gtnfggeyxk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.mhx1999.top/gtvnnilbgd.html

【使用说明】
来源：http://hz.jinghuilouyu.cn/gtewdyinxn.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.cdnleiting.top/gtwzuiokpr.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.xylfe.cn/gtboyijbmn.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.quarkkingdee.top/gtfckizdvq.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.hfpthk.cn/gttywtqwrc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.iojbl.cn/gtnvzqaqkl.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.jqgufenzy.top/gtllexlphr.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.wangdashe.top/gtgmogrqxi.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.aizwys.cn/gtnakosnot.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.hnqzz.top/gtdsmutwla.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.tianlin.xyz/gthqactqdw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.jlsjyb.cn/gtskscxjnz.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.jinghuilouyu.cn/gtdmuffhyt.html

【文件统计】
来源：http://hz.zhijiandao.cn/gtjiatbksk.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.cucudq.cn/gtslbrochg.html

--------------------------------------------------------------------------------
来源：http://hz.xylfe.cn/gtjyftwcqe.html

目  录
来源：http://hz.daxiang520.top/gteyhqgmbc.html

--------------------------------------------------------------------------------
来源：http://hz.xuanzx.com/gtdafumsqa.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.jqgfzy.top/gtnqurdaca.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.yvedp.cn/gttalphakt.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.hywenlv.cn/gtbhuvcklv.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.jqgfzy.top/gtuzvfagfg.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.xingfuxueyuan.xyz/gtiuseaqgz.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.hnxiangtu.top/gtcopldnyu.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.yj20258.top/gtolphqzqg.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.cqqwz.cn/gtneigzakk.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.tanke756.top/gtqrqfswkr.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.guowangkeji.top/gtbwxlagsw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.zhongyouzk.top/gtoosdrcub.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.cucudq.cn/gtzmkkjbcq.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.zhixingplan.top/gtpjaqpqsr.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.0kj1m.cn/gtbkbdkhez.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.pengpengdd.cyou/gtnfgikgvs.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.zhijiandao.cn/gtakjwenhi.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.jqgufenzy.top/gtodlaggym.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.jinqigfzy.top/gtpgztvcst.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.jlsjyb.cn/gtmualaled.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.c1oappe.top/gtmcbzjotb.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.sweek.top/gtbntauzyx.html

================================================================================
来源：http://hz.sxryk.cn/gtvlqbxkpc.html

A. 基础语法与类型
来源：http://hz.sxryk.cn/gtqzkcxulz.html

================================================================================
来源：http://hz.hammf.cn/gttpxbxlsq.html

[A01] Hello World
来源：http://hz.dashuyun.cn/gtixkwxmui.html

Py:   print("Hello, World!")
来源：http://hz.daria6918.cn/gtznottcon.html

PHP:  echo "Hello, World!";
来源：http://hz.sysykeji.top/gttvptfuss.html

JS:   console.log("Hello, World!");
来源：http://hz.guannengcc.top/gtgvqgexdt.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.yj202588.top/gtfmghuuxe.html

Java: System.out.println("Hello, World!");
来源：http://hz.jqgfzy.top/gtbpzxzehs.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.dashuyun.cn/gtyfemhvff.html

Ruby: puts "Hello, World!"
来源：http://hz.yj202588.top/gtssmlrhki.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.sysykeji.top/gtbizwemtm.html

[A02] 变量声明与赋值
来源：http://hz.aizwys.cn/gtbtjoeuut.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.pengpengdd.cyou/gteqgoqqnh.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.feifeiyinyue.top/gtwmautpbe.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.zhiwuduotai.top/gtqxfapcfe.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.wangshuangyany.cn/gtgjldqlsw.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.nanxuanxn.top/gtqoytrtrg.html

Go:   name := "Alex"; age := 20
来源：http://hz.zhaomingkeji.xyz/gtbduibgxw.html

Ruby: name = "Alex"; age = 20
来源：http://hz.hnqzz.top/gtxibumakx.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.tian-w.cn/gtmvdbefsb.html

[A03] 常量定义
来源：http://hz.gzhubu.top/gtpsgqiwqc.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.quarkkingdee.top/gtfqcjtxjf.html

PHP:  const PI = 3.14159;
来源：http://hz.zhoulong.xyz/gtchthfdgc.html

JS:   const PI = 3.14159;
来源：http://hz.hywenlv.cn/gtcmzypuhy.html

TS:   const PI: number = 3.14159;
来源：http://hz.ivvv.top/gtgjrntrsl.html

Java: static final double PI = 3.14159;
来源：http://hz.jinyuanbaomall.cn/gtvbapxmnt.html

Go:   const PI = 3.14159
来源：http://hz.zhoulong.xyz/gtkielwmnh.html

Ruby: PI = 3.14159
来源：http://hz.xuetiantiany.cn/gtiiopdftl.html

C#:   const double PI = 3.14159;
来源：http://hz.jinqigufen.top/gtjtcybzxn.html

[A04] 判断变量类型
来源：http://hz.guowangkeji.top/gtpsrxylvi.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.hnxiangtu.top/gtboddvvxi.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.havefunace.top/gtdgbnhvfj.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.aizwys.cn/gtlwaiwvtg.html

TS:   typeof x; x instanceof Date
来源：http://hz.zhaomingkeji.xyz/gtqfwkfmkn.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.snrcjt.cn/gtvkoeyerx.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.vqdsnc.cn/gtqeaydjpt.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.shangyingyoupin.top/gtkcelhjkz.html

C#:   x.GetType().Name; x is int
来源：http://hz.pycfn.com/gttvcrpyly.html

[A05] 整数除法与取模
来源：http://hz.sxryk.cn/gtvqkwsxfq.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.shzxlz.cn/gtxlkjfvpc.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.gaohongyu789.top/gtipmgpsnf.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.wangdashe.top/gttfmzkedh.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.zycfv.cn/gtfmftpyrw.html

Java: 7 / 2; 7 % 2
来源：http://hz.tianlin.xyz/gtwwpfdxwu.html

Go:   7 / 2; 7 % 2
来源：http://hz.zhixingplan.top/gtxacurecg.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.bjfxy.top/gtkhxybstp.html

C#:   7 / 2; 7 % 2
来源：http://hz.chenzaomai.com/gtmytgcvyo.html


<!-- 参考信息 -->