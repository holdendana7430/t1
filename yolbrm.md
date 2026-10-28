代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://hz.zdqjudy.top/gtvyjouotk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.ydjk.org.cn/gtzhitzyzd.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.cheryme.top/gtukfyjudd.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.daxiang520.top/gtgsipxxki.html

[U43] PHP：声明命名空间
来源：http://hz.xuanzx.com/gttfzupfda.html

namespace App\Http;
来源：http://hz.kuanghao11.cn/gthljqyfeq.html

[U44] PHP：开启严格类型
来源：http://hz.c1oappe.top/gtyiuvacnb.html

declare(strict_types=1);
来源：http://hz.wangdashe.top/gtkhrrbbvs.html

[U45] PHP：类型声明与返回类型
来源：http://hz.wangdashe.top/gtamfwpmcl.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yongpay.top/gtaqfuyspi.html

[U46] PHP：可空类型
来源：http://hz.cucudq.cn/gtdaqzypln.html

?string $name = null
来源：http://hz.bjfxy.top/gttboowtaz.html

[U47] PHP：联合类型
来源：http://hz.chenjidiqi.icu/gtpuqnxhkv.html

int|string $id
来源：http://hz.sweek.top/gtvwdotqbm.html

[U48] PHP：纯枚举
来源：http://hz.jqgfzy.top/gtxbelwwdq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.xingfuxueyuan.xyz/gtxssypmxf.html

[U49] PHP：只读属性
来源：http://hz.zdqjudy.top/gtrrpibrvk.html

public readonly string $name
来源：http://hz.yongpay.top/gtitpoqegv.html

[U50] PHP：构造器属性提升
来源：http://hz.yanxiufei.cn/gtiffvowoy.html

public function __construct(private int $id) {}
来源：http://hz.shanyushiyangtech.top/gtbiytfagt.html

[U51] PHP：数组解构
来源：http://hz.shuidangran.top/gtxccivlxs.html

[$a, $b] = $arr;
来源：http://hz.shanyushiyangkeji.top/gtpoldtvwi.html

[U52] PHP：箭头函数
来源：http://hz.jyoumei.cn/gtjijooeoo.html

$double = fn($x) => $x * 2;
来源：http://hz.jqgufenzy.top/gtzrbbipka.html

[U53] PHP：空合并运算符
来源：http://hz.gogol.net.cn/gtqyrkmput.html

$v = $a ?? $b ?? "default";
来源：http://hz.jinqigufen.top/gtmpuhrzim.html

[U54] PHP：空安全调用
来源：http://hz.yanxiufei.cn/gtvncbkcij.html

$obj?->method()
来源：http://hz.wangdashe.top/gtyigwklki.html

[U55] PHP：match 表达式
来源：http://hz.guowangkeji.top/gtlqzksyff.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.shanyushiyangtech.top/gtgyoxxfep.html

[U56] PHP：命名参数
来源：http://hz.hywenlv.cn/gtnszzfgnt.html

f(a: 1, b: 2)
来源：http://hz.ybcxt.top/gtujsauaga.html

[U57] PHP：字符串插值
来源：http://hz.yangfankeji.com/gtqwupdmhp.html

"值: {$a}"
来源：http://hz.hfpthk.cn/gthecetnka.html

[U58] PHP：数组三件套
来源：http://hz.sysykeji.top/gtzhvyqznk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.hysaishi.cn/gtpkjtdmuo.html

[U59] PHP：自定义排序
来源：http://hz.zhongyouzk.top/gtxrzqfden.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cheryme.top/gtawdmymyb.html

[U60] PHP：JSON 编解码
来源：http://hz.guannengcc.top/gtgeoqvpid.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.chenlongwang.top/gtrkiobtaf.html

[U61] PHP：正则
来源：http://hz.jlsjyb.cn/gtrqtrgdib.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.sufxvd.cn/gtoxzqawou.html

[U62] PHP：日期对象
来源：http://hz.andypj.xyz/gtqhirwqku.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.jinqigufen.top/gtdtsuemrl.html

[U63] PHP：文件读写
来源：http://hz.zhongyouzk.top/gtsspgydvl.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.redwolf501.top/gtcsoqulyl.html

[U64] PHP：目录遍历
来源：http://hz.9152youxi.cn/gtujfgspxp.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.zhiwuduotai.top/gtdloouecl.html

[U65] PHP：会话
来源：http://hz.aizwys.cn/gtjgicxkgi.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.vqdsnc.cn/gtxeccwuwj.html

[U66] PHP：设置 Cookie
来源：http://hz.feifeiyinyue.top/gtpsqdzeyk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.yanxiufei.cn/gtquzmdrqs.html

[U67] PHP：处理文件上传
来源：http://hz.shzxlz.cn/gtjnxwhgek.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.jqgufenzy.top/gtaofbefny.html

[U68] PHP：PDO 连接
来源：http://hz.tianlin.xyz/gtcpknwyfh.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.bjfxy.top/gtwsbrpczw.html

[U69] PHP：PDO 预处理
来源：http://hz.wangshuangyany.cn/gtrtnfzyya.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.xuanzx.com/gtjutdpxer.html

[U70] PHP：PDO 事务
来源：http://hz.shuidangran.top/gtrxgougjt.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.shangyingyoupin.top/gtljtxhjet.html

[U71] PHP：抛出异常
来源：http://hz.zdqjudy.top/gtqrrkrykr.html

throw new RuntimeException("失败", 500);
来源：http://hz.c1oappe.top/gtapnubosv.html

[U72] PHP：写错误日志
来源：http://hz.yongpay.top/gtdripjdez.html

error_log("失败: " . $e->getMessage());
来源：http://hz.pycfn.com/gtdwfnfeiu.html

[U73] PHP：读取 ini 配置
来源：http://hz.jinqigfzy.top/gtadwfrwrm.html

parse_ini_file("config.ini", true)
来源：http://hz.svipenyu.cn/gtkqwszlav.html

[U74] PHP：读取环境变量
来源：http://hz.cqqwz.cn/gtgaxsdvip.html

getenv("APP_ENV") ?: "production"
来源：http://hz.ydzc1.top/gtqgxponjn.html

[U75] PHP：依赖注入
来源：http://hz.guowangkeji.top/gtgpdzyddi.html

composer require psr/container
来源：http://hz.c1oappe.top/gttvdyxaqr.html

[U76] PHP：简单路由
来源：http://hz.hywenlv.cn/gtuwmsggnt.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.yueranfly.top/gtibwctxah.html

[U77] PHP：模板渲染
来源：http://hz.c1oappe.top/gtlpgzhjes.html

composer require twig/twig
来源：http://hz.jinqigufen.top/gtogafvzmc.html

[U78] PHP：单元测试
来源：http://hz.chenjidiqi.icu/gtbclefekq.html

composer require --dev phpunit/phpunit
来源：http://hz.andypj.xyz/gtbzerbnix.html

[U79] PHP：静态分析
来源：http://hz.fzhhl.top/gtggmsvwvc.html

composer require --dev phpstan/phpstan
来源：http://hz.cashguo.top/gtzuqouojl.html

[U80] PHP：代码规范修复
来源：http://hz.jqgufenzy.top/gtjfudjzmt.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.yvedp.cn/gtrywqnirs.html

[U81] JS：初始化项目
来源：http://hz.shzxlz.cn/gtfuefzmbe.html

npm init -y;  npm i express
来源：http://hz.aizwys.cn/gtswidjcrz.html

[U82] JS：package.json 脚本
来源：http://hz.jinyuanbaomall.cn/gtzytapvdf.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.gzhubu.top/gtuacxoseo.html

[U83] JS：ES Module 导入导出
来源：http://hz.daxiang520.top/gtpzpjfryl.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.c1oappe.top/gtirwrdjiy.html

[U84] JS：CommonJS 写法
来源：http://hz.tianlin.xyz/gtmdsdowal.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.zdqjudy.top/gtjxpcngiq.html

[U85] JS：可选链
来源：http://hz.cdnleiting.top/gtqoqsylfg.html

a?.b?.c
来源：http://hz.dashuyun.cn/gtlwbckrdo.html

[U86] JS：空值合并
来源：http://hz.ydzc1.top/gtvbuhouwo.html

a ?? b
来源：http://hz.shanyushiyangtech.top/gtbhcixumw.html

[U87] JS：解构默认值
来源：http://hz.shzxlz.cn/gtsknwuapc.html

const { a = 1, b = 2 } = obj;
来源：http://hz.tian-w.cn/gtihzhqxns.html

[U88] JS：对象展开合并
来源：http://hz.jqgufenzy.top/gthnblslkv.html

{ ...a, ...b }
来源：http://hz.bjfxy.top/gtnbwoijfz.html

[U89] JS：数组去重
来源：http://hz.zdqjudy.top/gtiuhmlonj.html

[...new Set(arr)]
来源：http://hz.nwbrower.top/gtkanogxrh.html

[U90] JS：数字数组排序
来源：http://hz.xuanzx.com/gtphbvzchk.html

[...arr].sort((a, b) => a - b)
来源：http://hz.nanxuanxn.top/gtyhaajtln.html

[U91] JS：对象键值遍历
来源：http://hz.andypj.xyz/gtrafjhqrk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.316326.xyz/gtpodwczlh.html

[U92] JS：深拷贝
来源：http://hz.dashuyun.cn/gtdzdcrwub.html

structuredClone(obj)
来源：http://hz.birdmap.top/gtnzwyunob.html

[U93] JS：模板字符串
来源：http://hz.jinqigufen.top/gtpifecnnj.html

`共 ${n} 条`
来源：http://hz.feifeiyinyue.top/gtxifqiksh.html

[U94] JS：箭头函数
来源：http://hz.sysykeji.top/gtksblahld.html

const double = x => x * 2;
来源：http://hz.yj20258888.top/gtrvjevpzg.html

[U95] JS：Promise 包装
来源：http://hz.ivvv.top/gtcvfqoair.html

new Promise((resolve, reject) => {})
来源：http://hz.jqgfzy.top/gtyasgglgp.html

[U96] JS：async/await 与异常
来源：http://hz.zhaomingkeji.xyz/gtwwlktkqi.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.zhengqikj.top/gtaewiprle.html

[U97] JS：并发请求
来源：http://hz.hnxiangtu.top/gtqepnpdiw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yangfankeji.com/gtmlplbewq.html

[U98] JS：fetch 带 JSON
来源：http://hz.chenzaomai.com/gtnmsgkaen.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.yongpay.top/gtyhztxvpe.html

[U99] JS：事件监听
来源：http://hz.svipenyu.cn/gtdhwdxwrt.html

el.addEventListener("click", e => {})
来源：http://hz.gotoacloud.top/gtiheuiwxc.html

[U100] JS：DOM 查询
来源：http://hz.yj20258888.top/gtocenabno.html

document.querySelector(".item")
来源：http://hz.yongpay.top/gtbnjdcaiy.html

[U101] JS：classList 操作
来源：http://hz.316326.xyz/gtvkoshjqm.html

el.classList.toggle("active")
来源：http://hz.jqgufenzy.top/gtjrrskrtw.html

[U102] JS：本地存储
来源：http://hz.fengsongda.top/gtpyrotoqj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.cdnleiting.top/gtvbbesjrs.html

[U103] JS：定时器
来源：http://hz.chenjidiqi.icu/gtomzgzdbn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.gogol.net.cn/gtjcajnnru.html

[U104] JS：防抖
来源：http://hz.zhixingplan.top/gtwwqsklnf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sysykeji.top/gtbzmcnbml.html

[U105] JS：节流
来源：http://hz.sysykeji.top/gtenkyzjtg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.jlsjyb.cn/gtnlihrrwx.html

[U106] JS：日期格式化
来源：http://hz.zdqjudy.top/gthsvhjhzk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.hongshengwenyu.top/gtqonyrwyj.html

[U107] JS：数字千分位
来源：http://hz.sysykeji.top/gtmywijhok.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.xylfe.cn/gtrustrame.html

[U108] JS：随机整数
来源：http://hz.daxiang520.top/gtcszgzwmz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.yj202588.top/gtjqqzfqgh.html

[U109] JS：数组分组
来源：http://hz.daria6918.cn/gtcoimejom.html

Object.groupBy(arr, x => x.type)
来源：http://hz.daxiang520.top/gtubaurlfl.html

[U110] JS：数组分块
来源：http://hz.wangshuangyany.cn/gtrljvklqc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.cheryme.top/gtdxnrdqzz.html

[U111] JS：对象转 Map
来源：http://hz.yvedp.cn/gtpmxstebe.html

new Map(Object.entries(obj))
来源：http://hz.zhaomingkeji.xyz/gtkovnwgxn.html

[U112] JS：字符串补位
来源：http://hz.hongshengwenyu.top/gtwzaxgejk.html

"7".padStart(3, "0")
来源：http://hz.chenlongwang.top/gtppkndcom.html

[U113] JS：正则替换全部
来源：http://hz.ydzc1.top/gttdfwpssd.html

s.replaceAll("a", "b")
来源：http://hz.zhaomingkeji.xyz/gtfhjolnyk.html

[U114] JS：JSON 深比较
来源：http://hz.xuetiantiany.cn/gtznobkqxz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.tian-w.cn/gtyyjmxwbi.html

[U115] JS：生成 UUID
来源：http://hz.yueranfly.top/gtjiqpowuw.html

crypto.randomUUID()
来源：http://hz.jyoumei.cn/gtglnpavug.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.aibaodan.cn/gthenpmssl.html

/** @param {string} name */ function f(name) {}
来源：http://hz.zhoulong.xyz/gtzvzkfvrx.html

[U117] JS：单元测试
来源：http://hz.gzhubu.top/gtoumvcwdz.html

npm i -D vitest;  npx vitest
来源：http://hz.zhaomingkeji.xyz/gtsaswycgg.html

[U118] JS：开发服务器
来源：http://hz.xuetiantiany.cn/gtmhzpxmtj.html

npm i -D vite;  npx vite
来源：http://hz.zhiwuduotai.top/gteppozehv.html

[U119] JS：生产构建
来源：http://hz.hnxiangtu.top/gtijbvqqxc.html

npx vite build
来源：http://hz.cashguo.top/gtggqddmid.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.xingfuxueyuan.xyz/gttitxrdwj.html

import.meta.env.VITE_API_URL
来源：http://hz.redwolf501.top/gtexgopwze.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtwrijssth.html

统计汇总
来源：http://hz.jiagoushi.top/gtuuuapmrd.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtqvundcwi.html

按语言统计（条）：
来源：http://hz.jianghu66.top/gtjouwtfph.html

Python ......... 252
来源：http://hz.yueranfly.top/gtluifizec.html

PHP ............ 252
来源：http://hz.xuetiantiany.cn/gtmjbsrkrr.html

JavaScript ..... 252
来源：http://hz.jianghu66.top/gtnsncumdl.html

TypeScript ..... 212
来源：http://hz.zhiwuduotai.top/gtukdyfsqu.html

Java ........... 212
来源：http://hz.zhaomingkeji.xyz/gtmzawrdji.html

Go ............. 212
来源：http://hz.fzhhl.top/gtbuidehpa.html

Ruby ........... 212
来源：http://hz.shanyushiyangkeji.top/gtjspytacl.html

C# ............. 212
来源：http://hz.yonumen.top/gtzmlidctl.html

C .............. 30
来源：http://hz.birdmap.top/gtxrvqszbu.html

C++ ............ 30
来源：http://hz.shangyingyoupin.top/gtrmyuqnib.html

SQL ............ 90
来源：http://hz.shzxlz.cn/gtolaxlboh.html

Bash ........... 80
来源：http://hz.andypj.xyz/gtxilrgyld.html

Kotlin ......... 15
来源：http://hz.ybcxt.top/gthavwjmwa.html

Swift .......... 15
来源：http://hz.aizwys.cn/gtblpgsbgg.html

Lua ............ 10
来源：http://hz.haohaochexian.top/gtjlzvscia.html

Perl ........... 10
来源：http://hz.andypj.xyz/gthjtkjkle.html

Scala .......... 10
来源：http://hz.dashuyun.cn/gtgahbjdmd.html

------------------------------------
来源：http://hz.yangfankeji.com/gtzzkrfwml.html

合计 ........... 2106 条
来源：http://hz.cdnleiting.top/gtuzysifpd.html

按章节统计：
来源：http://hz.tian-w.cn/gtcawudrwe.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.pycfn.com/gtowwxzrqr.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.iojbl.cn/gtuxbmeowr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.svipenyu.cn/gtxsnlvisu.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.cucudq.cn/gtcftmwybj.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.jinyuanbaomall.cn/gteufbjavw.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.zhiwuduotai.top/gtffkmqxwh.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.jqgfzy.top/gtbmkislpl.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.xinyue.icu/gtktmhrrwb.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.yj20258.top/gtoxxodnjs.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.yangfankeji.com/gtcijaljyu.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.jinghuilouyu.cn/gtcxvpljwe.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.zycfv.cn/gtqdzggxae.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.nwbrower.top/gtctvoirxf.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.andypj.xyz/gtuyuabbmb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.chenjidiqi.icu/gtovzfvxql.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.ybcxt.top/gtwhjfvvor.html

Q SQL 专题                              90
来源：http://hz.daxiang520.top/gthrkyvmgd.html

R Bash 专题                             80
来源：http://hz.xinyue.icu/gtxstjpibo.html

S C / C++ 专题                          60
来源：http://hz.zhoulong.xyz/gtiopwgxrc.html

T 其他语言补充                          60
来源：http://hz.pycfn.com/gttdghjgsu.html

U 高频实用片段                         120
来源：http://hz.ybcxt.top/gtbrqyxfaw.html

------------------------------------
来源：http://hz.jinqigufen.top/gtflumpfko.html

合计                                  2106 条
来源：http://hz.zhixingplan.top/gtjdqtyebm.html

--------------------------------------------------------------------------------
来源：http://hz.zhoulong.xyz/gtxkameifp.html

使用提醒
来源：http://hz.shangyingyoupin.top/gtysghjlkk.html

--------------------------------------------------------------------------------
来源：http://hz.xuanzx.com/gtkivfxwts.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.jianghu66.top/gtgvgczzfa.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.zycfv.cn/gtzfwnrzni.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.bjfxy.top/gtxmnzwbli.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.hongshengwenyu.top/gtlrspmlhy.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.yangfankeji.com/gtqzfohvpt.html

—— 文件结束 ——
来源：http://hz.mhx1999.top/gtzjcsyyjn.html

================================================================================
来源：http://hz.svipenyu.cn/gtsiucpsnb.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.hfpthk.cn/gtbsohzbbn.html

Common Programming Examples Cheat Book
来源：http://hz.redwolf501.top/gthlbstynu.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtylfwfeto.html

【收录内容】
来源：http://hz.daxiang520.top/gtymmbnsuj.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.hnxiangtu.top/gtknsbdedn.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.sufxvd.cn/gtuxksqgjw.html

SQL · Bash · C · C++
来源：http://hz.gotoacloud.top/gtrzgcutic.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.chenzaomai.com/gtsmwfyzjq.html

【使用说明】
来源：http://hz.zhaomingkeji.xyz/gtkqymmflp.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.yj202588.top/gtityiiumz.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.jiagoushi.top/gtaqltbzsd.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.xinyue.icu/gtvrzcersk.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.quarkkingdee.top/gteerfgsgg.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.zhijiandao.cn/gtfeyzwhmf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.zhaomingkeji.xyz/gtqzxchytm.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.jinyuanbaomall.cn/gttyoafraq.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.aibaodan.cn/gtiweggmmw.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.yonumen.top/gtfokgdeeu.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.sufxvd.cn/gtonshczln.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.yueranfly.top/gtbbywrpbf.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.zhixingplan.top/gtjarfkztg.html

【文件统计】
来源：http://hz.yongpay.top/gtamrvzibe.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.quarkkingdee.top/gtijifodye.html

--------------------------------------------------------------------------------
来源：http://hz.hysaishi.cn/gttbzndqcy.html

目  录
来源：http://hz.yj202588.top/gtrqgmgern.html

--------------------------------------------------------------------------------
来源：http://hz.guowangkeji.top/gtquetjgzi.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.yueranfly.top/gtnjnwevcq.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.birdmap.top/gteywmhyej.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.gzhubu.top/gtilzhumtz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.zdqjudy.top/gthwttzmsu.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.xylfe.cn/gtxibelfxk.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.aibaodan.cn/gtlvnnwfyp.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.chenzaomai.com/gtptpfkzbl.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.zdqjudy.top/gtfcnezyaf.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.jinghuilouyu.cn/gtvjrqhlzr.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.jianghu66.top/gtugdcxcfs.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.jlsjyb.cn/gttqvgydxq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.zhijiandao.cn/gtwixhiutq.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.jianghu66.top/gtskwgyrkz.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.wangshuangyany.cn/gtjbioicyl.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.jiagoushi.top/gtlujmaows.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.snrcjt.cn/gtppmyefqf.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.sweek.top/gtooufvvkf.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.yangfankeji.com/gtwgqnjxts.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.nanxuanxn.top/gtprmagfiu.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.gaohongyu789.top/gtblbpjnzu.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.hnqzz.top/gteqjpucrh.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtqeqazrmo.html

A. 基础语法与类型
来源：http://hz.316326.xyz/gthriizedn.html

================================================================================
来源：http://hz.sxryk.cn/gtpwhcdweq.html

[A01] Hello World
来源：http://hz.yj20258.top/gtdqlvxajx.html

Py:   print("Hello, World!")
来源：http://hz.ehwqpu.com/gtopodopqs.html

PHP:  echo "Hello, World!";
来源：http://hz.yonumen.top/gtkzptycnl.html

JS:   console.log("Hello, World!");
来源：http://hz.ydzc1.top/gtqqpculhl.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.yueranfly.top/gtahpuqtfi.html

Java: System.out.println("Hello, World!");
来源：http://hz.aizwys.cn/gtawkehcip.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.shuidangran.top/gtxulchzmh.html

Ruby: puts "Hello, World!"
来源：http://hz.dianchejie.cn/gtwruoigwf.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.zhongyouzk.top/gtgnczxped.html

[A02] 变量声明与赋值
来源：http://hz.52xcode.cn/gtkxaiipjt.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.shuidangran.top/gtzwerpfta.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.jlsjyb.cn/gtxqprdwvb.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.sweek.top/gttqolmubb.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.zdqjudy.top/gtvelirpnr.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.ywan-chungtsiang.top/gtfejjowph.html

Go:   name := "Alex"; age := 20
来源：http://hz.316326.xyz/gthgaucclm.html

Ruby: name = "Alex"; age = 20
来源：http://hz.ppjwa.cn/gtseomyiiw.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.jyoumei.cn/gtofurjztv.html

[A03] 常量定义
来源：http://hz.gzhubu.top/gtioimkjoh.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.ivvv.top/gtdirowhvm.html

PHP:  const PI = 3.14159;
来源：http://hz.shanyushiyangtech.top/gtkfsfteac.html

JS:   const PI = 3.14159;
来源：http://hz.9152youxi.cn/gtiqjmwjub.html

TS:   const PI: number = 3.14159;
来源：http://hz.52xcode.cn/gtceejhoiu.html

Java: static final double PI = 3.14159;
来源：http://hz.hammf.cn/gtdcywgqdj.html

Go:   const PI = 3.14159
来源：http://hz.zycfv.cn/gtugebweuo.html

Ruby: PI = 3.14159
来源：http://hz.cashguo.top/gtistijuny.html

C#:   const double PI = 3.14159;
来源：http://hz.yuxming.cn/gtwbcrlxwq.html

[A04] 判断变量类型
来源：http://hz.nwbrower.top/gtzddrhpfm.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.wangshuangyany.cn/gtfltfoeaa.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.chenlongwang.top/gtvcoayiel.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.yueranfly.top/gteoooosom.html

TS:   typeof x; x instanceof Date
来源：http://hz.shanyushiyangkeji.top/gtyiossasf.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.hfpthk.cn/gtccslinun.html


<!-- 参考信息 -->