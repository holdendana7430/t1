代发 wailian999

[U43] PHP：声明命名空间
来源：http://hz.tianlin.xyz/gtdsnezixl.html

namespace App\Http;
来源：http://hz.pycfn.com/gtwgvfyfrm.html

[U44] PHP：开启严格类型
来源：http://hz.yangfankeji.com/gtllhdjjod.html

declare(strict_types=1);
来源：http://hz.jyoumei.cn/gtwgljcqku.html

[U45] PHP：类型声明与返回类型
来源：http://hz.fzhhl.top/gtbqshrgnv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.daria6918.cn/gtdfpwoxwn.html

[U46] PHP：可空类型
来源：http://hz.tian-w.cn/gtruaecudz.html

?string $name = null
来源：http://hz.hammf.cn/gtmnicsegw.html

[U47] PHP：联合类型
来源：http://hz.hnqzz.top/gtzqewoypz.html

int|string $id
来源：http://hz.xziqi.cn/gtqalxmxjw.html

[U48] PHP：纯枚举
来源：http://hz.jinghuilouyu.cn/gtqdyqpsyt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.gogol.net.cn/gtxtlgojbs.html

[U49] PHP：只读属性
来源：http://hz.jinyuanbaomall.cn/gtikqmygrg.html

public readonly string $name
来源：http://hz.ybcxt.top/gtortzarke.html

[U50] PHP：构造器属性提升
来源：http://hz.xylfe.cn/gtzqaiagcs.html

public function __construct(private int $id) {}
来源：http://hz.hnxiangtu.top/gtwrglpbvs.html

[U51] PHP：数组解构
来源：http://hz.bjfxy.top/gtridipzmr.html

[$a, $b] = $arr;
来源：http://hz.9152youxi.cn/gtfbnqnbtb.html

[U52] PHP：箭头函数
来源：http://hz.wangshuangyany.cn/gtzvfqjajw.html

$double = fn($x) => $x * 2;
来源：http://hz.nanxinkj.top/gtkaowctra.html

[U53] PHP：空合并运算符
来源：http://hz.shanyushiyangtech.top/gtbqelqqov.html

$v = $a ?? $b ?? "default";
来源：http://hz.shanyushiyangkeji.top/gtayxyjmai.html

[U54] PHP：空安全调用
来源：http://hz.zhixingplan.top/gteachrcfl.html

$obj?->method()
来源：http://hz.zhongyouzk.top/gtqmcnnckp.html

[U55] PHP：match 表达式
来源：http://hz.cqqwz.cn/gtaztwcfnv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.gotoacloud.top/gtkibjcfhj.html

[U56] PHP：命名参数
来源：http://hz.zycfv.cn/gtjysbpfeo.html

f(a: 1, b: 2)
来源：http://hz.iojbl.cn/gtvloimceo.html

[U57] PHP：字符串插值
来源：http://hz.yangfankeji.com/gtgxkqegta.html

"值: {$a}"
来源：http://hz.snrcjt.cn/gtcjxvryzx.html

[U58] PHP：数组三件套
来源：http://hz.xziqi.cn/gtbgylbzqu.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.yuanzhike.top/gtegwbxhzx.html

[U59] PHP：自定义排序
来源：http://hz.ydjk.org.cn/gtlxqccxev.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.fzhhl.top/gtfbrkrdnn.html

[U60] PHP：JSON 编解码
来源：http://hz.sysykeji.top/gtryepaxot.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.shanyushiyangkeji.top/gtkguwsisq.html

[U61] PHP：正则
来源：http://hz.xziqi.cn/gtvbpnyjqo.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.feifeiyinyue.top/gtcvwhwget.html

[U62] PHP：日期对象
来源：http://hz.shanyushiyangkeji.top/gtuwcxqfzp.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.c1oappe.top/gtlkkpcapn.html

[U63] PHP：文件读写
来源：http://hz.ybcxt.top/gtaqczapjz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.yongpay.top/gtplxwihrx.html

[U64] PHP：目录遍历
来源：http://hz.zhengqikj.top/gtwanindyz.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.tian-w.cn/gtynytkhca.html

[U65] PHP：会话
来源：http://hz.hongshengwenyu.top/gtfboqqaol.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.wangdashe.top/gttghcjjpc.html

[U66] PHP：设置 Cookie
来源：http://hz.snrcjt.cn/gtepsexkpz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.yuanzhike.top/gtislwralg.html

[U67] PHP：处理文件上传
来源：http://hz.nanxuanxn.top/gtfebxrspq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.gogol.net.cn/gtgwtlnosi.html

[U68] PHP：PDO 连接
来源：http://hz.jinghuilouyu.cn/gtvtlicowf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.chenjidiqi.icu/gthedufbkx.html

[U69] PHP：PDO 预处理
来源：http://hz.zhoulong.xyz/gtrkhcdrql.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.haohaochexian.top/gtxynnsbca.html

[U70] PHP：PDO 事务
来源：http://hz.jiagoushi.top/gtzggfzitr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.gotoacloud.top/gtiqfphsom.html

[U71] PHP：抛出异常
来源：http://hz.hywenlv.cn/gtvxntiupk.html

throw new RuntimeException("失败", 500);
来源：http://hz.yanxiufei.cn/gtkngqduaa.html

[U72] PHP：写错误日志
来源：http://hz.zhoulong.xyz/gttpegvyjy.html

error_log("失败: " . $e->getMessage());
来源：http://hz.wangshuangyany.cn/gtzhrffblo.html

[U73] PHP：读取 ini 配置
来源：http://hz.snrcjt.cn/gtryzsrojy.html

parse_ini_file("config.ini", true)
来源：http://hz.daxiang520.top/gtvmnrxolv.html

[U74] PHP：读取环境变量
来源：http://hz.zycfv.cn/gtspiptpkt.html

getenv("APP_ENV") ?: "production"
来源：http://hz.0kj1m.cn/gtvbkrayjw.html

[U75] PHP：依赖注入
来源：http://hz.shuidangran.top/gtdpkslvpq.html

composer require psr/container
来源：http://hz.jianghu66.top/gtkydroads.html

[U76] PHP：简单路由
来源：http://hz.0kj1m.cn/gtxlliugpc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.316326.xyz/gttxdbwfrj.html

[U77] PHP：模板渲染
来源：http://hz.yvedp.cn/gtcsrjwctm.html

composer require twig/twig
来源：http://hz.shanyushiyangtech.top/gtsnavxbpa.html

[U78] PHP：单元测试
来源：http://hz.0kj1m.cn/gtltnbnpdn.html

composer require --dev phpunit/phpunit
来源：http://hz.hnqzz.top/gtklezvkhm.html

[U79] PHP：静态分析
来源：http://hz.cqqwz.cn/gtwbahargi.html

composer require --dev phpstan/phpstan
来源：http://hz.dianchejie.cn/gtpzqwfrqa.html

[U80] PHP：代码规范修复
来源：http://hz.yueranfly.top/gtcsuncceo.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.zhoulong.xyz/gtiefdjyje.html

[U81] JS：初始化项目
来源：http://hz.shangyingyoupin.top/gtypenpmfu.html

npm init -y;  npm i express
来源：http://hz.daria6918.cn/gtobhsqtyg.html

[U82] JS：package.json 脚本
来源：http://hz.kuanghao11.cn/gtxhrlataw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.jqgufenzy.top/gtogamfech.html

[U83] JS：ES Module 导入导出
来源：http://hz.jiagoushi.top/gtwetovtnq.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.zhixingplan.top/gttvqucqnw.html

[U84] JS：CommonJS 写法
来源：http://hz.c1oappe.top/gttvgoliku.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.yj20258.top/gtvqjtstjf.html

[U85] JS：可选链
来源：http://hz.sxryk.cn/gtzbuuvzvv.html

a?.b?.c
来源：http://hz.xylfe.cn/gtcrvzemyu.html

[U86] JS：空值合并
来源：http://hz.zhoulong.xyz/gtbppgsjdh.html

a ?? b
来源：http://hz.mhx1999.top/gtehqmofcx.html

[U87] JS：解构默认值
来源：http://hz.aizwys.cn/gtdpwgkzdh.html

const { a = 1, b = 2 } = obj;
来源：http://hz.meibo888.top/gtsbwztugk.html

[U88] JS：对象展开合并
来源：http://hz.ybcxt.top/gtcwrutsxw.html

{ ...a, ...b }
来源：http://hz.shzxlz.cn/gttvxgxetx.html

[U89] JS：数组去重
来源：http://hz.316326.xyz/gtqhhstpkc.html

[...new Set(arr)]
来源：http://hz.shuidangran.top/gtfmvubftm.html

[U90] JS：数字数组排序
来源：http://hz.hongshengwenyu.top/gtepqucqjt.html

[...arr].sort((a, b) => a - b)
来源：http://hz.9152youxi.cn/gtrnxwuaxw.html

[U91] JS：对象键值遍历
来源：http://hz.zhaomingkeji.xyz/gtwubuscqp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.pengpengdd.cyou/gtotgmtfsw.html

[U92] JS：深拷贝
来源：http://hz.xuetiantiany.cn/gttmislblf.html

structuredClone(obj)
来源：http://hz.fzhhl.top/gtxlstajxj.html

[U93] JS：模板字符串
来源：http://hz.shangyingyoupin.top/gthbsfgqbr.html

`共 ${n} 条`
来源：http://hz.zhiwuduotai.top/gtkjmqwwvi.html

[U94] JS：箭头函数
来源：http://hz.daxiang520.top/gtcanatdnt.html

const double = x => x * 2;
来源：http://hz.xingfuxueyuan.xyz/gtqoewtmxy.html

[U95] JS：Promise 包装
来源：http://hz.zhixingplan.top/gtzzfwdzdj.html

new Promise((resolve, reject) => {})
来源：http://hz.zhixingplan.top/gtmyjdedtz.html

[U96] JS：async/await 与异常
来源：http://hz.shangyingyoupin.top/gtebcdubkw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.hammf.cn/gtwvujofiy.html

[U97] JS：并发请求
来源：http://hz.jqgfzy.top/gtqhucgydp.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gotoacloud.top/gtmxnizacj.html

[U98] JS：fetch 带 JSON
来源：http://hz.yuxming.cn/gtruudixde.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.pengpengdd.cyou/gtjeetduxm.html

[U99] JS：事件监听
来源：http://hz.ppjwa.cn/gtoosekddi.html

el.addEventListener("click", e => {})
来源：http://hz.zhoulong.xyz/gtmmprbvxv.html

[U100] JS：DOM 查询
来源：http://hz.yj20258888.top/gtmsbyivii.html

document.querySelector(".item")
来源：http://hz.vqdsnc.cn/gtjilsacnb.html

[U101] JS：classList 操作
来源：http://hz.yj20258888.top/gtuhfmdurc.html

el.classList.toggle("active")
来源：http://hz.hfpthk.cn/gtztrerrnu.html

[U102] JS：本地存储
来源：http://hz.jinghuilouyu.cn/gtrdjvdahy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.quarkkingdee.top/gtzymflewz.html

[U103] JS：定时器
来源：http://hz.pengpengdd.cyou/gtjznysqjl.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.ydjk.org.cn/gttwlpiitf.html

[U104] JS：防抖
来源：http://hz.zhijiandao.cn/gtkcfcspdr.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yanxiufei.cn/gtrrxvlrag.html

[U105] JS：节流
来源：http://hz.yvedp.cn/gtqrgwxdtp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.nanxuanxn.top/gtcpohqpyj.html

[U106] JS：日期格式化
来源：http://hz.zhoulong.xyz/gtfvgmpwqg.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.ivvv.top/gtmzfepwxj.html

[U107] JS：数字千分位
来源：http://hz.yj20258.top/gtzuiynmcv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.shanyushiyangtech.top/gtuxjwmjop.html

[U108] JS：随机整数
来源：http://hz.zhongyouzk.top/gtpjpjtuze.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.guannengcc.top/gtzwnzzume.html

[U109] JS：数组分组
来源：http://hz.gogol.net.cn/gtlrdqstxd.html

Object.groupBy(arr, x => x.type)
来源：http://hz.redwolf501.top/gtlqvauxoe.html

[U110] JS：数组分块
来源：http://hz.yangfankeji.com/gthxhtqrmj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.yvedp.cn/gteuecbfso.html

[U111] JS：对象转 Map
来源：http://hz.gogol.net.cn/gtiiqhgjkn.html

new Map(Object.entries(obj))
来源：http://hz.yuxming.cn/gtzzekkvil.html

[U112] JS：字符串补位
来源：http://hz.zycfv.cn/gtmnaecavw.html

"7".padStart(3, "0")
来源：http://hz.chenjidiqi.icu/gtlawinkzm.html

[U113] JS：正则替换全部
来源：http://hz.gaohongyu789.top/gtyqzrhbmf.html

s.replaceAll("a", "b")
来源：http://hz.andypj.xyz/gtmgggljea.html

[U114] JS：JSON 深比较
来源：http://hz.hywenlv.cn/gtvwcgcmxk.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jinyuanbaomall.cn/gttdtublez.html

[U115] JS：生成 UUID
来源：http://hz.guowangkeji.top/gtofpthyrj.html

crypto.randomUUID()
来源：http://hz.aizwys.cn/gtycqahciu.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.guowangkeji.top/gtvfsiiduq.html

/** @param {string} name */ function f(name) {}
来源：http://hz.jiagoushi.top/gtufjcvxvn.html

[U117] JS：单元测试
来源：http://hz.meibo888.top/gtutfazbdc.html

npm i -D vitest;  npx vitest
来源：http://hz.nwbrower.top/gtmtcyiumb.html

[U118] JS：开发服务器
来源：http://hz.dianchejie.cn/gtpcmojskn.html

npm i -D vite;  npx vite
来源：http://hz.shzxlz.cn/gtgohmafji.html

[U119] JS：生产构建
来源：http://hz.hongshengwenyu.top/gtvhfjfxom.html

npx vite build
来源：http://hz.yj202588.top/gtapqbqord.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.xuanzx.com/gthoehbsps.html

import.meta.env.VITE_API_URL
来源：http://hz.sxryk.cn/gtuurohhlm.html

================================================================================
来源：http://hz.andypj.xyz/gtyetyouao.html

统计汇总
来源：http://hz.chenzaomai.com/gtiirjcidu.html

================================================================================
来源：http://hz.zycfv.cn/gtvucwhbiq.html

按语言统计（条）：
来源：http://hz.nwbrower.top/gthonqufxn.html

Python ......... 252
来源：http://hz.dashuyun.cn/gttirkkfoj.html

PHP ............ 252
来源：http://hz.fengsongda.top/gtwbitwgfd.html

JavaScript ..... 252
来源：http://hz.yonumen.top/gtcpzwmkvo.html

TypeScript ..... 212
来源：http://hz.yueranfly.top/gtphtrayki.html

Java ........... 212
来源：http://hz.zdqjudy.top/gtypvrqtlr.html

Go ............. 212
来源：http://hz.fengsongda.top/gtqbswaxhc.html

Ruby ........... 212
来源：http://hz.chenzaomai.com/gtgvkhfury.html

C# ............. 212
来源：http://hz.shanyushiyangtech.top/gtidbgtwfw.html

C .............. 30
来源：http://hz.haohaochexian.top/gtxcifupjm.html

C++ ............ 30
来源：http://hz.jqgfzy.top/gtuvvehjlo.html

SQL ............ 90
来源：http://hz.shangyingyoupin.top/gtqxjpkjna.html

Bash ........... 80
来源：http://hz.ybcxt.top/gtisespcck.html

Kotlin ......... 15
来源：http://hz.shanyushiyangkeji.top/gtglfzbiua.html

Swift .......... 15
来源：http://hz.feifeiyinyue.top/gtymrnydqx.html

Lua ............ 10
来源：http://hz.daria6918.cn/gtrmcmdora.html

Perl ........... 10
来源：http://hz.yuxming.cn/gtldjlocum.html

Scala .......... 10
来源：http://hz.pycfn.com/gthvvyrllk.html

------------------------------------
来源：http://hz.kuanghao11.cn/gtnuzdpbbb.html

合计 ........... 2106 条
来源：http://hz.hnxiangtu.top/gtinznuevk.html

按章节统计：
来源：http://hz.c1oappe.top/gtuiuxfeei.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.ydjk.org.cn/gtxneblesw.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.sysykeji.top/gtqdiaszuw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.cheryme.top/gtomigrrcz.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.havefunace.top/gtzftcauue.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.smart0.xyz/gtepdszdgj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.cheryme.top/gtdvckntds.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.shzxlz.cn/gtgvijplap.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.gzhubu.top/gtibjakoed.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.hysaishi.cn/gtiayxpdll.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.xuetiantiany.cn/gtaymgwpem.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.guannengcc.top/gtdmkinhdv.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.daxiang520.top/gtnwovdijb.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.xziqi.cn/gtpdffzvto.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.cheryme.top/gtfgcvaqqx.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.jlsjyb.cn/gtnlvsfzod.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.iojbl.cn/gtgsdnpufc.html

Q SQL 专题                              90
来源：http://hz.shangyingyoupin.top/gtzzzkwjwq.html

R Bash 专题                             80
来源：http://hz.ehwqpu.com/gtmkqpbuxv.html

S C / C++ 专题                          60
来源：http://hz.chenzaomai.com/gtyelieeif.html

T 其他语言补充                          60
来源：http://hz.ivvv.top/gterkbioom.html

U 高频实用片段                         120
来源：http://hz.0kj1m.cn/gtzfihjfjv.html

------------------------------------
来源：http://hz.jqgufenzy.top/gtuchcjswr.html

合计                                  2106 条
来源：http://hz.yj202588.top/gtffjveytq.html

--------------------------------------------------------------------------------
来源：http://hz.yonumen.top/gtgvehnrlz.html

使用提醒
来源：http://hz.jyoumei.cn/gtsptkehqp.html

--------------------------------------------------------------------------------
来源：http://hz.ppjwa.cn/gttqespygf.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.bjfxy.top/gtmzftmbrt.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.ydzc1.top/gtoufazlsp.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.cheryme.top/gtgtavlmll.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.zhoulong.xyz/gtneyszuht.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.ydzc1.top/gtgytgvbzw.html

—— 文件结束 ——
来源：http://hz.guowangkeji.top/gtfgqmibyo.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtovoeenfd.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.fengsongda.top/gtguioiwrk.html

Common Programming Examples Cheat Book
来源：http://hz.yongpay.top/gtgbvmagkg.html

================================================================================
来源：http://hz.ppjwa.cn/gtlrlabgsm.html

【收录内容】
来源：http://hz.haohaochexian.top/gtxwzlpocr.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.nanxinkj.top/gtnmllaojq.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.redwolf501.top/gtzbqapuxd.html

SQL · Bash · C · C++
来源：http://hz.tianlin.xyz/gtyccrhfpt.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.jlsjyb.cn/gtaxqioxff.html

【使用说明】
来源：http://hz.shanyushiyangtech.top/gtccamazpq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.cashguo.top/gtyihjslua.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.jiagoushi.top/gtoqogpzeg.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.chenjidiqi.icu/gtqklpyxwq.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.chenjidiqi.icu/gtutrbhuvx.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.jinyuanbaomall.cn/gtigxreilu.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.birdmap.top/gtdgkmmdwv.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.zhongyouzk.top/gtwnfzuizm.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.yj202588.top/gtzxvtmlvh.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.gaohongyu789.top/gtrjumpbbf.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.xuetiantiany.cn/gtbhfykcbh.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.316326.xyz/gtxqtspfrw.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.9152youxi.cn/gtjoinifpg.html

【文件统计】
来源：http://hz.yueranfly.top/gtglzqolzu.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.tian-w.cn/gtiyandbul.html

--------------------------------------------------------------------------------
来源：http://hz.zycfv.cn/gthfjsdhsg.html

目  录
来源：http://hz.nwbrower.top/gtdenmxfij.html

--------------------------------------------------------------------------------
来源：http://hz.tianlin.xyz/gtnhopcmnu.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.jiagoushi.top/gtsqfunluu.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.chenzaomai.com/gtwruaolni.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.havefunace.top/gtbsbopcpf.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.c1oappe.top/gtmftdzpyv.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.cheryme.top/gtrodqtihn.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.shzxlz.cn/gtesnxnjzn.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.feifeiyinyue.top/gtakkemkab.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.redwolf501.top/gthyjlfqgq.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.zhoulong.xyz/gtwgcdvpwh.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.sxryk.cn/gtgrnumvtn.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.zhengqikj.top/gttrdiiosp.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.vqdsnc.cn/gteglzzvzj.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.hywenlv.cn/gtgugwneak.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.hywenlv.cn/gtzwtlaztl.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.sysykeji.top/gtfmzlkfxc.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.wangshuangyany.cn/gtpowcddhy.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.zycfv.cn/gtdzdwtgxz.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.yuxming.cn/gtfndhjvte.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.guannengcc.top/gtjdaltodo.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ppjwa.cn/gtqrcekqaf.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.feifeiyinyue.top/gtyvnffyog.html

================================================================================
来源：http://hz.hnqzz.top/gtjbuklimn.html

A. 基础语法与类型
来源：http://hz.zdqjudy.top/gtacjnqidy.html

================================================================================
来源：http://hz.sysykeji.top/gtgznsylya.html

[A01] Hello World
来源：http://hz.vqdsnc.cn/gtnxvghjqr.html

Py:   print("Hello, World!")
来源：http://hz.sysykeji.top/gtcpvumzmi.html

PHP:  echo "Hello, World!";
来源：http://hz.hfpthk.cn/gtiohpohyb.html

JS:   console.log("Hello, World!");
来源：http://hz.xuetiantiany.cn/gtiaatwehg.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.kuanghao11.cn/gtkwsadrtz.html

Java: System.out.println("Hello, World!");
来源：http://hz.sweek.top/gtjqpmaxyc.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.c1oappe.top/gtukqeuqdl.html

Ruby: puts "Hello, World!"
来源：http://hz.jqgufenzy.top/gtshjbsypz.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.jinqigfzy.top/gtpbzctbrf.html

[A02] 变量声明与赋值
来源：http://hz.ybcxt.top/gtkpvhauvs.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.nanxuanxn.top/gtxduklnob.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.hnqzz.top/gtvklasadl.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.gaohongyu789.top/gtoemfulcc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.zycfv.cn/gtrypbidfo.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.jinqigfzy.top/gtuihqccke.html

Go:   name := "Alex"; age := 20
来源：http://hz.sweek.top/gtyucjzvhm.html

Ruby: name = "Alex"; age = 20
来源：http://hz.hnxiangtu.top/gtdphovioc.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.gotoacloud.top/gtwrjwezus.html

[A03] 常量定义
来源：http://hz.hywenlv.cn/gtfzfpxdvg.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.xingfuxueyuan.xyz/gtiavllgfe.html

PHP:  const PI = 3.14159;
来源：http://hz.jinqigufen.top/gtneuxzmii.html

JS:   const PI = 3.14159;
来源：http://hz.cqqwz.cn/gtcdldvnop.html

TS:   const PI: number = 3.14159;
来源：http://hz.9152youxi.cn/gtzhgsdxvy.html

Java: static final double PI = 3.14159;
来源：http://hz.zhaomingkeji.xyz/gtanyrlliv.html

Go:   const PI = 3.14159
来源：http://hz.jqgufenzy.top/gtrfsfxauu.html

Ruby: PI = 3.14159
来源：http://hz.zhongyouzk.top/gtnqxpihli.html

C#:   const double PI = 3.14159;
来源：http://hz.yongpay.top/gteuqoppuw.html

[A04] 判断变量类型
来源：http://hz.ywan-chungtsiang.top/gtansufxpb.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.shanyushiyangkeji.top/gtjywtmosu.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.kuanghao11.cn/gtlejhcxxy.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.vqdsnc.cn/gtmztsvntv.html

TS:   typeof x; x instanceof Date
来源：http://hz.nwbrower.top/gtqmfbsyuz.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.zhongyouzk.top/gtkmeyzgjs.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.jianghu66.top/gtugcauogz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.quarkkingdee.top/gtqhknndmq.html

C#:   x.GetType().Name; x is int
来源：http://hz.jqgufenzy.top/gtermtbpxt.html

[A05] 整数除法与取模
来源：http://hz.iojbl.cn/gtvfskvspy.html


<!-- 参考信息 -->