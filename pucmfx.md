代发 wailian999

[U47] PHP：联合类型
来源：http://hz.haohaochexian.top/gthgkwivaw.html

int|string $id
来源：http://hz.sysykeji.top/gtwzcqgwti.html

[U48] PHP：纯枚举
来源：http://hz.xylfe.cn/gtygciefii.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.gogol.net.cn/gtdgmpynzd.html

[U49] PHP：只读属性
来源：http://hz.ydjk.org.cn/gtkljsoccl.html

public readonly string $name
来源：http://hz.svipenyu.cn/gtgmugazjx.html

[U50] PHP：构造器属性提升
来源：http://hz.zdqjudy.top/gtucmbnjvp.html

public function __construct(private int $id) {}
来源：http://hz.jqgufenzy.top/gtzlscxfww.html

[U51] PHP：数组解构
来源：http://hz.ivvv.top/gtdesgnoft.html

[$a, $b] = $arr;
来源：http://hz.redwolf501.top/gtfryflgwb.html

[U52] PHP：箭头函数
来源：http://hz.xinyue.icu/gtwtisfbvo.html

$double = fn($x) => $x * 2;
来源：http://hz.wangdashe.top/gtrnjycwsj.html

[U53] PHP：空合并运算符
来源：http://hz.gotoacloud.top/gtfhzqszjt.html

$v = $a ?? $b ?? "default";
来源：http://hz.ywan-chungtsiang.top/gthlycvecr.html

[U54] PHP：空安全调用
来源：http://hz.nanxuanxn.top/gtussaiinz.html

$obj?->method()
来源：http://hz.tanke756.top/gtqnysezcj.html

[U55] PHP：match 表达式
来源：http://hz.hnxiangtu.top/gtalbqobgq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.zhixingplan.top/gtqwsvhrsf.html

[U56] PHP：命名参数
来源：http://hz.nwbrower.top/gtoacrvqew.html

f(a: 1, b: 2)
来源：http://hz.pengpengdd.cyou/gtooqodllo.html

[U57] PHP：字符串插值
来源：http://hz.feifeiyinyue.top/gtazfgpmmq.html

"值: {$a}"
来源：http://hz.c1oappe.top/gtscsxnxea.html

[U58] PHP：数组三件套
来源：http://hz.dianchejie.cn/gtyaasdzuy.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.feifeiyinyue.top/gtmfvcifsb.html

[U59] PHP：自定义排序
来源：http://hz.gaohongyu789.top/gtscecykxy.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cucudq.cn/gthjkfgvzu.html

[U60] PHP：JSON 编解码
来源：http://hz.yangfankeji.com/gtdqhqyqsp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.guowangkeji.top/gttjmfkbcc.html

[U61] PHP：正则
来源：http://hz.9152youxi.cn/gtbabotapg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.andypj.xyz/gtwzpehzma.html

[U62] PHP：日期对象
来源：http://hz.chenlongwang.top/gtatwmfpcp.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.ywan-chungtsiang.top/gtjkiepjin.html

[U63] PHP：文件读写
来源：http://hz.meibo888.top/gtinmotkox.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.meibo888.top/gtfbouhuhs.html

[U64] PHP：目录遍历
来源：http://hz.316326.xyz/gtqvwmgqex.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.guowangkeji.top/gtikbaxhmc.html

[U65] PHP：会话
来源：http://hz.hfpthk.cn/gtmfaenqvx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.dashuyun.cn/gtgtikyyvr.html

[U66] PHP：设置 Cookie
来源：http://hz.tanke756.top/gttkxkrcif.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.zhaomingkeji.xyz/gtpaezickq.html

[U67] PHP：处理文件上传
来源：http://hz.yanxiufei.cn/gtfrecxejm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.shuidangran.top/gtpcjxlogg.html

[U68] PHP：PDO 连接
来源：http://hz.zycfv.cn/gtalkwfyih.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.hongshengwenyu.top/gthisqufvi.html

[U69] PHP：PDO 预处理
来源：http://hz.dashuyun.cn/gtotkwcyct.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.cheryme.top/gtjoydmgla.html

[U70] PHP：PDO 事务
来源：http://hz.ppjwa.cn/gtloirocxi.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.yanxiufei.cn/gtgzqupkbd.html

[U71] PHP：抛出异常
来源：http://hz.quarkkingdee.top/gtdrtjkesm.html

throw new RuntimeException("失败", 500);
来源：http://hz.jiagoushi.top/gtavwaqozm.html

[U72] PHP：写错误日志
来源：http://hz.nanxinkj.top/gtespwtgvc.html

error_log("失败: " . $e->getMessage());
来源：http://hz.cdnleiting.top/gtxohljyrm.html

[U73] PHP：读取 ini 配置
来源：http://hz.quarkkingdee.top/gtgkgycmao.html

parse_ini_file("config.ini", true)
来源：http://hz.xingfuxueyuan.xyz/gtcwsviocm.html

[U74] PHP：读取环境变量
来源：http://hz.xuetiantiany.cn/gtzwfzpjbh.html

getenv("APP_ENV") ?: "production"
来源：http://hz.vqdsnc.cn/gteesynzie.html

[U75] PHP：依赖注入
来源：http://hz.haohaochexian.top/gtzsokxthm.html

composer require psr/container
来源：http://hz.chenlongwang.top/gtgdyvbnfg.html

[U76] PHP：简单路由
来源：http://hz.cdnleiting.top/gtejxlhyss.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.zhaomingkeji.xyz/gtrknjmihl.html

[U77] PHP：模板渲染
来源：http://hz.havefunace.top/gtysromnpg.html

composer require twig/twig
来源：http://hz.jqgufenzy.top/gtnjmqhbce.html

[U78] PHP：单元测试
来源：http://hz.jinqigfzy.top/gtiwwqidwx.html

composer require --dev phpunit/phpunit
来源：http://hz.gotoacloud.top/gteukxdsup.html

[U79] PHP：静态分析
来源：http://hz.cqqwz.cn/gtdlikuxjk.html

composer require --dev phpstan/phpstan
来源：http://hz.hysaishi.cn/gtgmenwuop.html

[U80] PHP：代码规范修复
来源：http://hz.jqgufenzy.top/gtjdxmohww.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.xuetiantiany.cn/gtnoigppft.html

[U81] JS：初始化项目
来源：http://hz.jianghu66.top/gtmsmupclk.html

npm init -y;  npm i express
来源：http://hz.jianghu66.top/gtefogchql.html

[U82] JS：package.json 脚本
来源：http://hz.yj202588.top/gtoxuuzwvc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.ydzc1.top/gtqlmddxce.html

[U83] JS：ES Module 导入导出
来源：http://hz.cashguo.top/gtgcncynlv.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.snrcjt.cn/gtzsqtqdlj.html

[U84] JS：CommonJS 写法
来源：http://hz.tianlin.xyz/gtijhoyvtf.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.jyoumei.cn/gtopyugorc.html

[U85] JS：可选链
来源：http://hz.haohaochexian.top/gtopgeolfd.html

a?.b?.c
来源：http://hz.jinqigfzy.top/gtfiwuqwlh.html

[U86] JS：空值合并
来源：http://hz.nanxinkj.top/gtehgyjjik.html

a ?? b
来源：http://hz.jiagoushi.top/gtucdybewn.html

[U87] JS：解构默认值
来源：http://hz.hammf.cn/gtsqlqzooa.html

const { a = 1, b = 2 } = obj;
来源：http://hz.yuanzhike.top/gtbxeozknp.html

[U88] JS：对象展开合并
来源：http://hz.yanxiufei.cn/gtpvzdtraa.html

{ ...a, ...b }
来源：http://hz.jinqigfzy.top/gteceoavxt.html

[U89] JS：数组去重
来源：http://hz.gotoacloud.top/gtffhacgvb.html

[...new Set(arr)]
来源：http://hz.52xcode.cn/gtnsjlbgmd.html

[U90] JS：数字数组排序
来源：http://hz.jinqigufen.top/gtjgeqibjg.html

[...arr].sort((a, b) => a - b)
来源：http://hz.xziqi.cn/gtrermgbly.html

[U91] JS：对象键值遍历
来源：http://hz.xylfe.cn/gtzmnjbsft.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.pycfn.com/gtqxagzvyd.html

[U92] JS：深拷贝
来源：http://hz.jinqigfzy.top/gtuwkeniqr.html

structuredClone(obj)
来源：http://hz.xuanzx.com/gtiggjrrqp.html

[U93] JS：模板字符串
来源：http://hz.dianchejie.cn/gtzjpccnsg.html

`共 ${n} 条`
来源：http://hz.yonumen.top/gtvzcajoad.html

[U94] JS：箭头函数
来源：http://hz.hfpthk.cn/gtlwqhsptz.html

const double = x => x * 2;
来源：http://hz.jinghuilouyu.cn/gtpashyrdr.html

[U95] JS：Promise 包装
来源：http://hz.tianlin.xyz/gtlztepdqc.html

new Promise((resolve, reject) => {})
来源：http://hz.yongpay.top/gtczvzsnxq.html

[U96] JS：async/await 与异常
来源：http://hz.hnxiangtu.top/gtheoxnuvc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.ydjk.org.cn/gtiyzahqth.html

[U97] JS：并发请求
来源：http://hz.guannengcc.top/gtaoiqoiju.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhengqikj.top/gtkfazlkhb.html

[U98] JS：fetch 带 JSON
来源：http://hz.gogol.net.cn/gthlgqmora.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.sufxvd.cn/gtawakxpet.html

[U99] JS：事件监听
来源：http://hz.tanke756.top/gtjbpyakgh.html

el.addEventListener("click", e => {})
来源：http://hz.jqgfzy.top/gtpmblemis.html

[U100] JS：DOM 查询
来源：http://hz.sxryk.cn/gtbijnnotd.html

document.querySelector(".item")
来源：http://hz.shanyushiyangtech.top/gttqtzblso.html

[U101] JS：classList 操作
来源：http://hz.jqgufenzy.top/gtdzzmumfm.html

el.classList.toggle("active")
来源：http://hz.sysykeji.top/gtijanllhz.html

[U102] JS：本地存储
来源：http://hz.ehwqpu.com/gtrbptapoh.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.zycfv.cn/gtialegass.html

[U103] JS：定时器
来源：http://hz.aizwys.cn/gtrtxsupyp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.shuidangran.top/gtnpurmrsc.html

[U104] JS：防抖
来源：http://hz.tanke756.top/gtkihatzed.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.iojbl.cn/gtzczxxser.html

[U105] JS：节流
来源：http://hz.guannengcc.top/gtcemugxxc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.ehwqpu.com/gtodgjdehp.html

[U106] JS：日期格式化
来源：http://hz.jinghuilouyu.cn/gtuhrephlf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.jinqigfzy.top/gtdxxsiigr.html

[U107] JS：数字千分位
来源：http://hz.cashguo.top/gtdqfdpwxa.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.ivvv.top/gtttdkbufm.html

[U108] JS：随机整数
来源：http://hz.cheryme.top/gtmtspkojo.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.bjfxy.top/gtjbyrxcxa.html

[U109] JS：数组分组
来源：http://hz.jqgufenzy.top/gtojuwlnyr.html

Object.groupBy(arr, x => x.type)
来源：http://hz.yanxiufei.cn/gtjpjtdfyp.html

[U110] JS：数组分块
来源：http://hz.yuanzhike.top/gtpihhpihm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.xinyue.icu/gtpwxergyg.html

[U111] JS：对象转 Map
来源：http://hz.jqgufenzy.top/gtwkdfzeez.html

new Map(Object.entries(obj))
来源：http://hz.yj20258.top/gtuxmkbxck.html

[U112] JS：字符串补位
来源：http://hz.cashguo.top/gtyxfthwak.html

"7".padStart(3, "0")
来源：http://hz.sufxvd.cn/gtaoydwtrn.html

[U113] JS：正则替换全部
来源：http://hz.xuetiantiany.cn/gtkmxeoald.html

s.replaceAll("a", "b")
来源：http://hz.zhongyouzk.top/gtcuvinbqv.html

[U114] JS：JSON 深比较
来源：http://hz.ybcxt.top/gtafhgzmki.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.daxiang520.top/gtvlsbggbc.html

[U115] JS：生成 UUID
来源：http://hz.iojbl.cn/gtzkgqmlok.html

crypto.randomUUID()
来源：http://hz.jyoumei.cn/gtiryypwia.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.daria6918.cn/gtfqrxwttt.html

/** @param {string} name */ function f(name) {}
来源：http://hz.iojbl.cn/gtctmrxvib.html

[U117] JS：单元测试
来源：http://hz.jyoumei.cn/gttbvcjzdg.html

npm i -D vitest;  npx vitest
来源：http://hz.tanke756.top/gtexseeuxh.html

[U118] JS：开发服务器
来源：http://hz.snrcjt.cn/gtvsgzuuzb.html

npm i -D vite;  npx vite
来源：http://hz.ehwqpu.com/gteqmjpeyh.html

[U119] JS：生产构建
来源：http://hz.xuanzx.com/gtuoqcjsyc.html

npx vite build
来源：http://hz.cashguo.top/gtyleuneid.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.sweek.top/gtdwpksfra.html

import.meta.env.VITE_API_URL
来源：http://hz.jinghuilouyu.cn/gtchbsalbb.html

================================================================================
来源：http://hz.jyoumei.cn/gtwufebhij.html

统计汇总
来源：http://hz.cdnleiting.top/gtjohqvgog.html

================================================================================
来源：http://hz.zdqjudy.top/gtjahyjpdd.html

按语言统计（条）：
来源：http://hz.gzhubu.top/gtdtipxixn.html

Python ......... 252
来源：http://hz.feifeiyinyue.top/gtrztdvywu.html

PHP ............ 252
来源：http://hz.zhijiandao.cn/gtmtjyadqu.html

JavaScript ..... 252
来源：http://hz.daxiang520.top/gtevhsfxoy.html

TypeScript ..... 212
来源：http://hz.smart0.xyz/gtxfloeupc.html

Java ........... 212
来源：http://hz.daxiang520.top/gtpmxxhygd.html

Go ............. 212
来源：http://hz.zycfv.cn/gtgbpwhvkx.html

Ruby ........... 212
来源：http://hz.wangdashe.top/gtdgezrqgp.html

C# ............. 212
来源：http://hz.bjfxy.top/gtwrkvhiby.html

C .............. 30
来源：http://hz.xziqi.cn/gtabqwemhs.html

C++ ............ 30
来源：http://hz.ehwqpu.com/gtjvjqzdcl.html

SQL ............ 90
来源：http://hz.zhaomingkeji.xyz/gtqyodadcs.html

Bash ........... 80
来源：http://hz.zhaomingkeji.xyz/gtjdmkxcfw.html

Kotlin ......... 15
来源：http://hz.xylfe.cn/gtlbwedklz.html

Swift .......... 15
来源：http://hz.xuetiantiany.cn/gtzpdkzyxh.html

Lua ............ 10
来源：http://hz.zdqjudy.top/gtgazqmnpi.html

Perl ........... 10
来源：http://hz.shanyushiyangkeji.top/gtpjjfkkiy.html

Scala .......... 10
来源：http://hz.zhengqikj.top/gtgedgqist.html

------------------------------------
来源：http://hz.hfpthk.cn/gtvgjztoen.html

合计 ........... 2106 条
来源：http://hz.jinqigfzy.top/gtvvghofak.html

按章节统计：
来源：http://hz.zhijiandao.cn/gtamxeqgpg.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.ppjwa.cn/gtqwisegeq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.xuetiantiany.cn/gtwfvoiteg.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.yj202588.top/gtyjzhtypo.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.wangshuangyany.cn/gtjdnlwltb.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.guowangkeji.top/gtnnmvnvap.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.shzxlz.cn/gtzzzfrgdz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.hywenlv.cn/gtiyknzbgq.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.hywenlv.cn/gtogefbkct.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.yj20258.top/gtkrauvhsa.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.shangyingyoupin.top/gterrqnazu.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.zhiwuduotai.top/gtgeiszwkq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.jinqigfzy.top/gtzuevmezs.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.chenlongwang.top/gtdosjkifz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.cheryme.top/gtgtkiodgy.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.dianchejie.cn/gtnavcyikm.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.wangdashe.top/gtxoyegryt.html

Q SQL 专题                              90
来源：http://hz.zhongyouzk.top/gtgnnnswij.html

R Bash 专题                             80
来源：http://hz.jqgfzy.top/gtiesopodp.html

S C / C++ 专题                          60
来源：http://hz.hysaishi.cn/gtjceoauds.html

T 其他语言补充                          60
来源：http://hz.dianchejie.cn/gtxjijoexk.html

U 高频实用片段                         120
来源：http://hz.guannengcc.top/gtkyncrhhq.html

------------------------------------
来源：http://hz.guannengcc.top/gtxxgjbogy.html

合计                                  2106 条
来源：http://hz.jlsjyb.cn/gtskbzqlmc.html

--------------------------------------------------------------------------------
来源：http://hz.sysykeji.top/gtnmsgsgcd.html

使用提醒
来源：http://hz.jiagoushi.top/gtrdolojdh.html

--------------------------------------------------------------------------------
来源：http://hz.yuanzhike.top/gtbplyuetn.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.ydjk.org.cn/gtfasdjefm.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.jinqigufen.top/gtbcgshqcr.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.zhijiandao.cn/gtcytvpxgd.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.ppjwa.cn/gtrpjaehsm.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.mhx1999.top/gtddlrjjnq.html

—— 文件结束 ——
来源：http://hz.jlsjyb.cn/gtnfwwmvao.html

================================================================================
来源：http://hz.jlsjyb.cn/gtocnxihtg.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.hfpthk.cn/gtwanlebuo.html

Common Programming Examples Cheat Book
来源：http://hz.bjfxy.top/gtfzuzvsqw.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtndfuftwp.html

【收录内容】
来源：http://hz.jyoumei.cn/gtmfigkzra.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.hfpthk.cn/gtxcanpnqy.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.jinqigufen.top/gtltbyyslu.html

SQL · Bash · C · C++
来源：http://hz.zhaomingkeji.xyz/gtqhucsbvv.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.ydzc1.top/gtthnrltxu.html

【使用说明】
来源：http://hz.aizwys.cn/gtybnzjesw.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.zhiwuduotai.top/gtssifvtge.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.zhijiandao.cn/gtirovskcj.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.jqgfzy.top/gtwklosexg.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.ydjk.org.cn/gtlednkccb.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.sweek.top/gtmebqazcg.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.c1oappe.top/gtezirodeu.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.aizwys.cn/gthwvspprh.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.sufxvd.cn/gthobqcied.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.nanxuanxn.top/gtbblwvxie.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.jqgufenzy.top/gtppwiukii.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.52xcode.cn/gtpngahaih.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.birdmap.top/gtsdkivvxx.html

【文件统计】
来源：http://hz.guannengcc.top/gtdjkbpnel.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.cdnleiting.top/gtyiqmxwhh.html

--------------------------------------------------------------------------------
来源：http://hz.ppjwa.cn/gtnkvfuqhh.html

目  录
来源：http://hz.haohaochexian.top/gthpkpmoyk.html

--------------------------------------------------------------------------------
来源：http://hz.zhiwuduotai.top/gtkbmdecmz.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.jqgfzy.top/gtebuvdcnp.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.yj20258.top/gtugxxtzkb.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.gogol.net.cn/gtbvdrqpwm.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.jqgfzy.top/gttnczmddy.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.xylfe.cn/gtfdwuabac.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.yuanzhike.top/gtahditxrc.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.gaohongyu789.top/gtixvuxzch.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.yj20258.top/gtlszvyrpg.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.yj20258.top/gtgtfpmeqp.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.yj202588.top/gtmynvhbut.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.sufxvd.cn/gteapohshk.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.daxiang520.top/gttofkwgdo.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.shangyingyoupin.top/gttqrogfjm.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.jyoumei.cn/gtkrrslsmp.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.yj20258.top/gtxzwjcryn.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.haohaochexian.top/gtdvtrnpma.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.ybcxt.top/gtqdkqidse.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.havefunace.top/gtroslkaiu.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.dianchejie.cn/gtemefkzmr.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yanxiufei.cn/gtycypykjc.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.sysykeji.top/gtmbsbjlnc.html

================================================================================
来源：http://hz.nwbrower.top/gtlfvfvkmf.html

A. 基础语法与类型
来源：http://hz.iojbl.cn/gteurroojw.html

================================================================================
来源：http://hz.pycfn.com/gtmymgqqam.html

[A01] Hello World
来源：http://hz.gogol.net.cn/gthgfdmboe.html

Py:   print("Hello, World!")
来源：http://hz.andypj.xyz/gtsryufkql.html

PHP:  echo "Hello, World!";
来源：http://hz.havefunace.top/gtefuhxczd.html

JS:   console.log("Hello, World!");
来源：http://hz.zdqjudy.top/gtncavjjvc.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.hywenlv.cn/gtlrsdupks.html

Java: System.out.println("Hello, World!");
来源：http://hz.shzxlz.cn/gtcugljenn.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.sysykeji.top/gtqpkvghvg.html

Ruby: puts "Hello, World!"
来源：http://hz.yj20258.top/gtzhtxwaoi.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.jinghuilouyu.cn/gtrvtahbgk.html

[A02] 变量声明与赋值
来源：http://hz.cheryme.top/gtfrtwycpy.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.xuetiantiany.cn/gtdxrfpbpu.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.jinyuanbaomall.cn/gtytnhvclo.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.zhengqikj.top/gtlgavgmbr.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.yvedp.cn/gtkwwlmnmf.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.zhongyouzk.top/gthpydtudr.html

Go:   name := "Alex"; age := 20
来源：http://hz.shzxlz.cn/gtepslwtjn.html

Ruby: name = "Alex"; age = 20
来源：http://hz.xingfuxueyuan.xyz/gtrxfumljl.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.shanyushiyangtech.top/gtqxochmjc.html

[A03] 常量定义
来源：http://hz.jqgufenzy.top/gtfwdjulfv.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.hysaishi.cn/gtcxmubfjm.html

PHP:  const PI = 3.14159;
来源：http://hz.yj20258.top/gtvelifhnf.html

JS:   const PI = 3.14159;
来源：http://hz.svipenyu.cn/gtwsraluua.html

TS:   const PI: number = 3.14159;
来源：http://hz.shanyushiyangtech.top/gtwblcbvzi.html

Java: static final double PI = 3.14159;
来源：http://hz.gaohongyu789.top/gtedonkijf.html

Go:   const PI = 3.14159
来源：http://hz.andypj.xyz/gtyvgocezg.html

Ruby: PI = 3.14159
来源：http://hz.zhoulong.xyz/gtmmvyfnzx.html

C#:   const double PI = 3.14159;
来源：http://hz.pengpengdd.cyou/gtvsgwnwtu.html

[A04] 判断变量类型
来源：http://hz.fengsongda.top/gtbhtumfom.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.ydzc1.top/gtuijcibqd.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.redwolf501.top/gtiknukbys.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.ehwqpu.com/gtfxuuvljp.html

TS:   typeof x; x instanceof Date
来源：http://hz.daria6918.cn/gtaoltmozc.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.cashguo.top/gttjwyfspw.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.jqgfzy.top/gtwjsjqphy.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.jinqigfzy.top/gtvugzyxca.html

C#:   x.GetType().Name; x is int
来源：http://hz.nanxinkj.top/gtagyvolpk.html

[A05] 整数除法与取模
来源：http://hz.shanyushiyangtech.top/gtvqdnbybw.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.hammf.cn/gtwuotgian.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.feifeiyinyue.top/gtbmvfggeb.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.yongpay.top/gtmpdsfbcg.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.zhiwuduotai.top/gtyqbiyxpx.html

Java: 7 / 2; 7 % 2
来源：http://hz.chenjidiqi.icu/gterymwmia.html

Go:   7 / 2; 7 % 2
来源：http://hz.pycfn.com/gtxxvztqfm.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.xylfe.cn/gtyivfzohy.html

C#:   7 / 2; 7 % 2
来源：http://hz.snrcjt.cn/gteqsswiyb.html


<!-- 参考信息 -->