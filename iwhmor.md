代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://hz.zhijiandao.cn/gtobrsemam.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.tian-w.cn/gtwdnahcrd.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.yj20258888.top/gtflegfcmc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.zhaomingkeji.xyz/gtrxyuiutu.html

[U43] PHP：声明命名空间
来源：http://hz.shzxlz.cn/gtdquqmodm.html

namespace App\Http;
来源：http://hz.jinghuilouyu.cn/gthwxzegsz.html

[U44] PHP：开启严格类型
来源：http://hz.zhengqikj.top/gtsqzkeqln.html

declare(strict_types=1);
来源：http://hz.meibo888.top/gtwjkayeah.html

[U45] PHP：类型声明与返回类型
来源：http://hz.zhengqikj.top/gtblqpesmy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gotoacloud.top/gtxwpvonch.html

[U46] PHP：可空类型
来源：http://hz.ydzc1.top/gtivnbpexu.html

?string $name = null
来源：http://hz.sweek.top/gtcezwkvwq.html

[U47] PHP：联合类型
来源：http://hz.yuanzhike.top/gtzypnjpyc.html

int|string $id
来源：http://hz.ivvv.top/gtmrdsyhar.html

[U48] PHP：纯枚举
来源：http://hz.yuxming.cn/gtiusxbjep.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.smart0.xyz/gtsgjvxlru.html

[U49] PHP：只读属性
来源：http://hz.yj20258.top/gtafynhaux.html

public readonly string $name
来源：http://hz.xuetiantiany.cn/gtfblubtsi.html

[U50] PHP：构造器属性提升
来源：http://hz.yuanzhike.top/gtthauhbtm.html

public function __construct(private int $id) {}
来源：http://hz.hfpthk.cn/gtiyjijywn.html

[U51] PHP：数组解构
来源：http://hz.0kj1m.cn/gtexygszpu.html

[$a, $b] = $arr;
来源：http://hz.cdnleiting.top/gtzunmsvjz.html

[U52] PHP：箭头函数
来源：http://hz.xinyue.icu/gtljkagaab.html

$double = fn($x) => $x * 2;
来源：http://hz.xuanzx.com/gtiuucpzmg.html

[U53] PHP：空合并运算符
来源：http://hz.andypj.xyz/gtkqtnmztj.html

$v = $a ?? $b ?? "default";
来源：http://hz.gaohongyu789.top/gtafiwynpj.html

[U54] PHP：空安全调用
来源：http://hz.xuanzx.com/gtotrdoqxc.html

$obj?->method()
来源：http://hz.zdqjudy.top/gtdnsjjfwl.html

[U55] PHP：match 表达式
来源：http://hz.sweek.top/gtfqxixtoc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.yuxming.cn/gtfrbcwfjm.html

[U56] PHP：命名参数
来源：http://hz.nwbrower.top/gtrokafcwp.html

f(a: 1, b: 2)
来源：http://hz.redwolf501.top/gtcsnobxpo.html

[U57] PHP：字符串插值
来源：http://hz.svipenyu.cn/gtqniqamzb.html

"值: {$a}"
来源：http://hz.zhixingplan.top/gtsukywjyy.html

[U58] PHP：数组三件套
来源：http://hz.dianchejie.cn/gtqingkyui.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.havefunace.top/gtkzkjmzhp.html

[U59] PHP：自定义排序
来源：http://hz.xuanzx.com/gtfepnngst.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hysaishi.cn/gtdiifiymo.html

[U60] PHP：JSON 编解码
来源：http://hz.redwolf501.top/gtwsuniwdc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.xuetiantiany.cn/gtnmyvvyqq.html

[U61] PHP：正则
来源：http://hz.jinghuilouyu.cn/gtddtwxtqy.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.shanyushiyangkeji.top/gtfwzeqmmt.html

[U62] PHP：日期对象
来源：http://hz.aizwys.cn/gtdorlrkya.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.jinyuanbaomall.cn/gtzjqadltc.html

[U63] PHP：文件读写
来源：http://hz.xinyue.icu/gtmyioklaf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.zdqjudy.top/gtbildxjaa.html

[U64] PHP：目录遍历
来源：http://hz.yueranfly.top/gtkkfmtnbq.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.bjfxy.top/gtxkaqlfhy.html

[U65] PHP：会话
来源：http://hz.c1oappe.top/gtporvdsah.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.jlsjyb.cn/gtjgcydrvl.html

[U66] PHP：设置 Cookie
来源：http://hz.yanxiufei.cn/gtwwsssgup.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.shanyushiyangkeji.top/gtecwaowxc.html

[U67] PHP：处理文件上传
来源：http://hz.jiagoushi.top/gtxmclxxix.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.cheryme.top/gtzrytxwhb.html

[U68] PHP：PDO 连接
来源：http://hz.smart0.xyz/gtruwlgseh.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.ydjk.org.cn/gtvmkpglop.html

[U69] PHP：PDO 预处理
来源：http://hz.nwbrower.top/gtbdotymnz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.ydzc1.top/gtqrrsuyan.html

[U70] PHP：PDO 事务
来源：http://hz.pycfn.com/gtriodvvub.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.svipenyu.cn/gtxdyipwcj.html

[U71] PHP：抛出异常
来源：http://hz.daria6918.cn/gtstdrzbmj.html

throw new RuntimeException("失败", 500);
来源：http://hz.jqgufenzy.top/gtegskuozg.html

[U72] PHP：写错误日志
来源：http://hz.zhijiandao.cn/gtidjbuupa.html

error_log("失败: " . $e->getMessage());
来源：http://hz.andypj.xyz/gtgjavckpu.html

[U73] PHP：读取 ini 配置
来源：http://hz.jinyuanbaomall.cn/gtvzsrsrtb.html

parse_ini_file("config.ini", true)
来源：http://hz.pengpengdd.cyou/gtmxkdhedy.html

[U74] PHP：读取环境变量
来源：http://hz.kuanghao11.cn/gtssqyuruk.html

getenv("APP_ENV") ?: "production"
来源：http://hz.snrcjt.cn/gtdwswxkja.html

[U75] PHP：依赖注入
来源：http://hz.sweek.top/gtpbdocuvc.html

composer require psr/container
来源：http://hz.xziqi.cn/gtmdoeriqr.html

[U76] PHP：简单路由
来源：http://hz.cheryme.top/gtacojosiq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.hnqzz.top/gtspbriyui.html

[U77] PHP：模板渲染
来源：http://hz.sysykeji.top/gthqvvznla.html

composer require twig/twig
来源：http://hz.feifeiyinyue.top/gtzhsxtxjt.html

[U78] PHP：单元测试
来源：http://hz.ehwqpu.com/gtcxhjscri.html

composer require --dev phpunit/phpunit
来源：http://hz.gotoacloud.top/gthsijbxzh.html

[U79] PHP：静态分析
来源：http://hz.daria6918.cn/gtwosiyrxq.html

composer require --dev phpstan/phpstan
来源：http://hz.nanxuanxn.top/gtluqgctov.html

[U80] PHP：代码规范修复
来源：http://hz.hongshengwenyu.top/gtslzqkdjf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.nanxinkj.top/gtzdcozdle.html

[U81] JS：初始化项目
来源：http://hz.sufxvd.cn/gtlrefqabw.html

npm init -y;  npm i express
来源：http://hz.52xcode.cn/gtexnvlebf.html

[U82] JS：package.json 脚本
来源：http://hz.redwolf501.top/gtrlstxdyx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.chenzaomai.com/gtxvjwkmvv.html

[U83] JS：ES Module 导入导出
来源：http://hz.hysaishi.cn/gtbwspljxa.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.meibo888.top/gtdhatpejy.html

[U84] JS：CommonJS 写法
来源：http://hz.haohaochexian.top/gtotimuhek.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.hnqzz.top/gtnsaonvll.html

[U85] JS：可选链
来源：http://hz.yangfankeji.com/gttkluxpuf.html

a?.b?.c
来源：http://hz.wangdashe.top/gtjewcurmu.html

[U86] JS：空值合并
来源：http://hz.nanxinkj.top/gtlsouxqgy.html

a ?? b
来源：http://hz.cashguo.top/gtaidaiduk.html

[U87] JS：解构默认值
来源：http://hz.yvedp.cn/gtzvjzyixq.html

const { a = 1, b = 2 } = obj;
来源：http://hz.c1oappe.top/gtxxgebizw.html

[U88] JS：对象展开合并
来源：http://hz.zhijiandao.cn/gtnfymjacl.html

{ ...a, ...b }
来源：http://hz.ehwqpu.com/gttnkuqhga.html

[U89] JS：数组去重
来源：http://hz.sysykeji.top/gthyrkkbpl.html

[...new Set(arr)]
来源：http://hz.zhixingplan.top/gtrxbghxns.html

[U90] JS：数字数组排序
来源：http://hz.jyoumei.cn/gtafxbcjvp.html

[...arr].sort((a, b) => a - b)
来源：http://hz.aizwys.cn/gtgefhogro.html

[U91] JS：对象键值遍历
来源：http://hz.jinqigfzy.top/gtzrukedxo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.cucudq.cn/gtwkbzhbbw.html

[U92] JS：深拷贝
来源：http://hz.hnqzz.top/gtntscamjh.html

structuredClone(obj)
来源：http://hz.zdqjudy.top/gtcxisgwns.html

[U93] JS：模板字符串
来源：http://hz.shzxlz.cn/gtwhxaopaq.html

`共 ${n} 条`
来源：http://hz.gaohongyu789.top/gtteubcfmv.html

[U94] JS：箭头函数
来源：http://hz.xuetiantiany.cn/gtzyephmyq.html

const double = x => x * 2;
来源：http://hz.yj20258888.top/gtgmimqfyv.html

[U95] JS：Promise 包装
来源：http://hz.haohaochexian.top/gtaudrsbfs.html

new Promise((resolve, reject) => {})
来源：http://hz.nanxinkj.top/gtvkaosgvz.html

[U96] JS：async/await 与异常
来源：http://hz.zhixingplan.top/gthsyghplp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.kuanghao11.cn/gtvctkwidk.html

[U97] JS：并发请求
来源：http://hz.sweek.top/gtmfwgkkep.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.feifeiyinyue.top/gtuwhlsebj.html

[U98] JS：fetch 带 JSON
来源：http://hz.haohaochexian.top/gtanwkorpo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.chenlongwang.top/gteqvjhtap.html

[U99] JS：事件监听
来源：http://hz.c1oappe.top/gtpexjnira.html

el.addEventListener("click", e => {})
来源：http://hz.gzhubu.top/gtyjepnijf.html

[U100] JS：DOM 查询
来源：http://hz.52xcode.cn/gtnayfmqjv.html

document.querySelector(".item")
来源：http://hz.xinyue.icu/gtgzuxpnfc.html

[U101] JS：classList 操作
来源：http://hz.ybcxt.top/gtamrdcrbh.html

el.classList.toggle("active")
来源：http://hz.yueranfly.top/gtjjkcgxxl.html

[U102] JS：本地存储
来源：http://hz.zycfv.cn/gtdehknhuj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.jqgufenzy.top/gtbkdxjsop.html

[U103] JS：定时器
来源：http://hz.yanxiufei.cn/gtcdawfmlk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.shanyushiyangtech.top/gtnecrliwf.html

[U104] JS：防抖
来源：http://hz.9152youxi.cn/gturumesun.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hongshengwenyu.top/gtvtmdknwg.html

[U105] JS：节流
来源：http://hz.havefunace.top/gtrdklnadr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.wangdashe.top/gtyohszuaw.html

[U106] JS：日期格式化
来源：http://hz.wangshuangyany.cn/gteghtntlp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.zhaomingkeji.xyz/gtlaepkagz.html

[U107] JS：数字千分位
来源：http://hz.kuanghao11.cn/gtasmracya.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.wangdashe.top/gthpslboll.html

[U108] JS：随机整数
来源：http://hz.guannengcc.top/gtufosjpsv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.smart0.xyz/gtxkzyqrni.html

[U109] JS：数组分组
来源：http://hz.xylfe.cn/gthecfeaov.html

Object.groupBy(arr, x => x.type)
来源：http://hz.yj202588.top/gtqsgvwbad.html

[U110] JS：数组分块
来源：http://hz.c1oappe.top/gtfsrbrnjg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.andypj.xyz/gtzbsxfpwf.html

[U111] JS：对象转 Map
来源：http://hz.shuidangran.top/gthwuxkqmi.html

new Map(Object.entries(obj))
来源：http://hz.yvedp.cn/gtqiyvhqvq.html

[U112] JS：字符串补位
来源：http://hz.birdmap.top/gtnkerqwbr.html

"7".padStart(3, "0")
来源：http://hz.haohaochexian.top/gtgvsofxsn.html

[U113] JS：正则替换全部
来源：http://hz.shuidangran.top/gtyknmzzao.html

s.replaceAll("a", "b")
来源：http://hz.ybcxt.top/gttiuqitkq.html

[U114] JS：JSON 深比较
来源：http://hz.ywan-chungtsiang.top/gtnqlyckjw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xziqi.cn/gtktjhhqve.html

[U115] JS：生成 UUID
来源：http://hz.shuidangran.top/gtpmybrboj.html

crypto.randomUUID()
来源：http://hz.ppjwa.cn/gtejgfjoud.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.feifeiyinyue.top/gtcywiqgua.html

/** @param {string} name */ function f(name) {}
来源：http://hz.havefunace.top/gtjjdrktwc.html

[U117] JS：单元测试
来源：http://hz.cheryme.top/gtkviguknk.html

npm i -D vitest;  npx vitest
来源：http://hz.snrcjt.cn/gtlfewdtjk.html

[U118] JS：开发服务器
来源：http://hz.cucudq.cn/gtrevorpko.html

npm i -D vite;  npx vite
来源：http://hz.xuetiantiany.cn/gtpnszoiaw.html

[U119] JS：生产构建
来源：http://hz.hnxiangtu.top/gteqcmmtwf.html

npx vite build
来源：http://hz.sysykeji.top/gtqfqriwrb.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.haohaochexian.top/gtcgqohyvc.html

import.meta.env.VITE_API_URL
来源：http://hz.shanyushiyangtech.top/gtzirqyfze.html

================================================================================
来源：http://hz.sweek.top/gtrgdniryc.html

统计汇总
来源：http://hz.haohaochexian.top/gtjwurjacf.html

================================================================================
来源：http://hz.zhengqikj.top/gtcdljidvj.html

按语言统计（条）：
来源：http://hz.316326.xyz/gtomjkkezs.html

Python ......... 252
来源：http://hz.sweek.top/gtgjkbqucr.html

PHP ............ 252
来源：http://hz.shuidangran.top/gtwjtfvojn.html

JavaScript ..... 252
来源：http://hz.sweek.top/gtmagkqsqj.html

TypeScript ..... 212
来源：http://hz.chenlongwang.top/gtnobwcyba.html

Java ........... 212
来源：http://hz.jqgufenzy.top/gtrtcyikgm.html

Go ............. 212
来源：http://hz.aibaodan.cn/gtmfbcddlr.html

Ruby ........... 212
来源：http://hz.nanxuanxn.top/gtgrgtmwlk.html

C# ............. 212
来源：http://hz.vqdsnc.cn/gttixvwuoj.html

C .............. 30
来源：http://hz.cashguo.top/gtzmirhbgs.html

C++ ............ 30
来源：http://hz.smart0.xyz/gtnjddpjhq.html

SQL ............ 90
来源：http://hz.sxryk.cn/gtyiornpwg.html

Bash ........... 80
来源：http://hz.yonumen.top/gtubnomwhg.html

Kotlin ......... 15
来源：http://hz.zhixingplan.top/gtejtoictt.html

Swift .......... 15
来源：http://hz.yvedp.cn/gtyojkfbow.html

Lua ............ 10
来源：http://hz.yuanzhike.top/gtcgbpsmco.html

Perl ........... 10
来源：http://hz.gogol.net.cn/gthtreipvh.html

Scala .......... 10
来源：http://hz.vqdsnc.cn/gtqtkgtncj.html

------------------------------------
来源：http://hz.yuanzhike.top/gtcfnzjfrk.html

合计 ........... 2106 条
来源：http://hz.snrcjt.cn/gtewjcoiat.html

按章节统计：
来源：http://hz.mhx1999.top/gtiaahaatp.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.yangfankeji.com/gtnxausxje.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.daria6918.cn/gtmaxetjgz.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.cdnleiting.top/gthimuundr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.hysaishi.cn/gtodvtzfeg.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.iojbl.cn/gtvbfeboiw.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.mhx1999.top/gtudejtjyk.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.sweek.top/gtrvvgiewk.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.aizwys.cn/gthsajkdux.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.zhengqikj.top/gtywixzxkw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.zhixingplan.top/gteylunvti.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.zhaomingkeji.xyz/gtzxcoqilg.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.aibaodan.cn/gthnqpbgcc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.guannengcc.top/gtyfnjgole.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.sxryk.cn/gterxltwwv.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.zhoulong.xyz/gtvfflreem.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.zhixingplan.top/gtdhpnrzib.html

Q SQL 专题                              90
来源：http://hz.ppjwa.cn/gtxfkjthxs.html

R Bash 专题                             80
来源：http://hz.chenzaomai.com/gtbomonykj.html

S C / C++ 专题                          60
来源：http://hz.pycfn.com/gtefsxqhsj.html

T 其他语言补充                          60
来源：http://hz.snrcjt.cn/gtbmdapabc.html

U 高频实用片段                         120
来源：http://hz.xziqi.cn/gtbzrdufzy.html

------------------------------------
来源：http://hz.shanyushiyangkeji.top/gtnqamwfmf.html

合计                                  2106 条
来源：http://hz.hywenlv.cn/gtlgapvuag.html

--------------------------------------------------------------------------------
来源：http://hz.havefunace.top/gtsvucpiwd.html

使用提醒
来源：http://hz.hnxiangtu.top/gthvyclyzx.html

--------------------------------------------------------------------------------
来源：http://hz.jianghu66.top/gtoxciwuqq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.quarkkingdee.top/gtpzbvvgua.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.jqgufenzy.top/gtbytrciud.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.haohaochexian.top/gtezvivqgz.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.shuidangran.top/gtofydstib.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.yvedp.cn/gteklekxni.html

—— 文件结束 ——
来源：http://hz.nanxinkj.top/gtqnogybgz.html

================================================================================
来源：http://hz.ivvv.top/gtfyvdqmrb.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.hywenlv.cn/gthgmmytqf.html

Common Programming Examples Cheat Book
来源：http://hz.tian-w.cn/gtbsodpogx.html

================================================================================
来源：http://hz.pycfn.com/gtkhpgkheg.html

【收录内容】
来源：http://hz.9152youxi.cn/gtsdlcyktt.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.cqqwz.cn/gtlyelaozp.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.gogol.net.cn/gtpnxawfuw.html

SQL · Bash · C · C++
来源：http://hz.ehwqpu.com/gtsxfeohty.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.hnxiangtu.top/gtwjmhdvlx.html

【使用说明】
来源：http://hz.gogol.net.cn/gtjlikfqew.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.meibo888.top/gtivgooimj.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.tian-w.cn/gttjuovpxn.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.andypj.xyz/gtyapqwqgm.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.ivvv.top/gtkrpjafpz.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.yj20258.top/gtycaicsuo.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.ehwqpu.com/gtbkmpvcju.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.daxiang520.top/gtqhccjbyk.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.c1oappe.top/gtjwumilen.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.hammf.cn/gtiuurfivk.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.9152youxi.cn/gtpwvylsdp.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.guowangkeji.top/gtuuihzswn.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.iojbl.cn/gtncnobmrw.html

【文件统计】
来源：http://hz.shangyingyoupin.top/gtdnumluxj.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.fzhhl.top/gtdwwnreag.html

--------------------------------------------------------------------------------
来源：http://hz.tianlin.xyz/gtjtmmdope.html

目  录
来源：http://hz.guannengcc.top/gtofbrfztr.html

--------------------------------------------------------------------------------
来源：http://hz.gogol.net.cn/gtbxroitns.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.yangfankeji.com/gtuiieoqpx.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.yangfankeji.com/gtjhcgzxkl.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.shanyushiyangtech.top/gtkbyjvric.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.xuetiantiany.cn/gtwxkroran.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.dianchejie.cn/gtwlionlhk.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.gzhubu.top/gtvbpmknzo.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.yonumen.top/gtxciuncxx.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.zhijiandao.cn/gtinzcnckv.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.cashguo.top/gtapazimuh.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.gogol.net.cn/gtaintqrzu.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.nanxuanxn.top/gtpdxsrpjh.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.svipenyu.cn/gtesedzkrg.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.gotoacloud.top/gtousvmqea.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.ydzc1.top/gtlyeawzmp.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.birdmap.top/gtncaemfgz.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.shangyingyoupin.top/gtfxbsuelz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.xingfuxueyuan.xyz/gtgosjesxl.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.ybcxt.top/gtrhmcsdcv.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.hongshengwenyu.top/gtjwqrnnfg.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yuanzhike.top/gtdmdgfybc.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.yuanzhike.top/gtafbvnutz.html

================================================================================
来源：http://hz.gaohongyu789.top/gtkrxcgomf.html

A. 基础语法与类型
来源：http://hz.daxiang520.top/gtugjbwbpn.html

================================================================================
来源：http://hz.hnxiangtu.top/gtxtrxjjdi.html

[A01] Hello World
来源：http://hz.316326.xyz/gtcwaghent.html

Py:   print("Hello, World!")
来源：http://hz.shuidangran.top/gthrhkwgav.html

PHP:  echo "Hello, World!";
来源：http://hz.redwolf501.top/gtkkwwagpd.html

JS:   console.log("Hello, World!");
来源：http://hz.jinghuilouyu.cn/gtdcfiptui.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.gogol.net.cn/gtgvgesbpi.html

Java: System.out.println("Hello, World!");
来源：http://hz.yuanzhike.top/gtgxddbndj.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.birdmap.top/gtroguqhii.html

Ruby: puts "Hello, World!"
来源：http://hz.yuanzhike.top/gtcgcmjjuc.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.yuxming.cn/gtkvvhejqa.html

[A02] 变量声明与赋值
来源：http://hz.daria6918.cn/gtufjcxrdf.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.zdqjudy.top/gthzrrnnwz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.tian-w.cn/gtqhsbspvh.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.zycfv.cn/gtzcqnbber.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.316326.xyz/gtoxhvxssx.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.xuetiantiany.cn/gtwzguiapi.html

Go:   name := "Alex"; age := 20
来源：http://hz.shzxlz.cn/gttmatlljw.html

Ruby: name = "Alex"; age = 20
来源：http://hz.havefunace.top/gtdemekfzf.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.iojbl.cn/gtnwoapnpp.html

[A03] 常量定义
来源：http://hz.zhengqikj.top/gtvnwebmww.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.ivvv.top/gtuuoqxmbn.html

PHP:  const PI = 3.14159;
来源：http://hz.sweek.top/gtjzldpjke.html

JS:   const PI = 3.14159;
来源：http://hz.jinyuanbaomall.cn/gtfplomkza.html

TS:   const PI: number = 3.14159;
来源：http://hz.jinghuilouyu.cn/gtznkqjpuy.html

Java: static final double PI = 3.14159;
来源：http://hz.ydjk.org.cn/gtcvrwnctm.html

Go:   const PI = 3.14159
来源：http://hz.chenlongwang.top/gtmmkrwszm.html

Ruby: PI = 3.14159
来源：http://hz.fengsongda.top/gtmlabwrqs.html

C#:   const double PI = 3.14159;
来源：http://hz.nanxuanxn.top/gtddhbhnfk.html

[A04] 判断变量类型
来源：http://hz.chenlongwang.top/gtbrieqtnq.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.yvedp.cn/gtzcjahnfu.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.wangdashe.top/gtomczhqpo.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.sufxvd.cn/gtxbzybaps.html

TS:   typeof x; x instanceof Date
来源：http://hz.jinqigfzy.top/gtecmdpirb.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.birdmap.top/gtrvelgoww.html


<!-- 参考信息 -->