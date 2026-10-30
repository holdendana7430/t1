代发 wailian999

[U55] PHP：match 表达式
来源：http://read.share.hesvh.cn/Article/details/gmlspmjpe.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fehbvm.com/Article/details/gvzkxrckb.sHtML

[U56] PHP：命名参数
来源：http://read.share.hesvh.cn/Article/details/gvmaiwmgg.sHtML

f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gfwkjyvqr.sHtML

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gxiqcyrkx.sHtML

"值: {$a}"
来源：http://3g.fehbvm.com/Article/details/gbnghgrhp.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fehbvm.com/Article/details/gkddwzkab.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.hesvh.cn/Article/details/gwakyqoxd.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fehbvm.com/Article/details/geqcmhxju.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gpumjopaf.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.hesvh.cn/Article/details/gxjcyfgpj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.hesvh.cn/Article/details/gfexsbgbb.sHtML

[U61] PHP：正则
来源：http://3g.fehbvm.com/Article/details/gstnggqdf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/gwfwqxlyd.sHtML

[U62] PHP：日期对象
来源：http://3g.hesvh.cn/Article/details/ghshziygo.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fehbvm.com/Article/details/gprlrubba.sHtML

[U63] PHP：文件读写
来源：http://3g.zdbjq.cn/Article/details/gtrsfrrlu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.zdbjq.cn/Article/details/guznuurll.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fehbvm.com/Article/details/gvxfuyepn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fehbvm.com/Article/details/ggqbdnavd.sHtML

[U65] PHP：会话
来源：http://mobile.fehbvm.com/Article/details/gifjkckyp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.hesvh.cn/Article/details/ghpcroanz.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fehbvm.com/Article/details/gsmrrxwpi.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.zdbjq.cn/Article/details/goujgccrm.sHtML

[U67] PHP：处理文件上传
来源：http://blog.hesvh.cn/Article/details/gnbuhpkyy.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fehbvm.com/Article/details/gviaspunp.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fehbvm.com/Article/details/gsntcolwg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fehbvm.com/Article/details/ggeztxptf.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.zdbjq.cn/Article/details/gwlpufroh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.hesvh.cn/Article/details/gkyehfxgx.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.hesvh.cn/Article/details/gihpfbhzi.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fehbvm.com/Article/details/gdtjszzac.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fehbvm.com/Article/details/gxrjoyeki.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.zdbjq.cn/Article/details/gmpgxsuwj.sHtML

[U72] PHP：写错误日志
来源：http://3g.zdbjq.cn/Article/details/gkimsbnqf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fehbvm.com/Article/details/ghqavglfb.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.hesvh.cn/Article/details/gzrsbrplr.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fehbvm.com/Article/details/gewmfuekb.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gtsuzimar.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fehbvm.com/Article/details/gehvmwrvf.sHtML

[U75] PHP：依赖注入
来源：http://baike.hesvh.cn/Article/details/ggqmmgnhh.sHtML

composer require psr/container
来源：http://www.blog.fehbvm.com/Article/details/gwyjkfflk.sHtML

[U76] PHP：简单路由
来源：http://3g.fehbvm.com/Article/details/gyaddwzxg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.hesvh.cn/Article/details/ggnlyvzzm.sHtML

[U77] PHP：模板渲染
来源：http://3g.zdbjq.cn/Article/details/gcrrbfceq.sHtML

composer require twig/twig
来源：http://www.share.zdbjq.cn/Article/details/gqdgwppij.sHtML

[U78] PHP：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gfritexdq.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fehbvm.com/Article/details/gqmzfmuuq.sHtML

[U79] PHP：静态分析
来源：http://baike.zdbjq.cn/Article/details/gshcusuly.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.hesvh.cn/Article/details/gzghmgowh.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.hesvh.cn/Article/details/gnzjyxzit.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.hesvh.cn/Article/details/guumkoywb.sHtML

[U81] JS：初始化项目
来源：http://baike.fehbvm.com/Article/details/gtgwjqgkq.sHtML

npm init -y;  npm i express
来源：http://mobile.zdbjq.cn/Article/details/gisgrnnjl.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.hesvh.cn/Article/details/gzictvkcg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.hesvh.cn/Article/details/gpfysfxtk.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.hesvh.cn/Article/details/gngiqqvkz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.hesvh.cn/Article/details/grighqhqu.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.zdbjq.cn/Article/details/getujpbnd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fehbvm.com/Article/details/govzngpce.sHtML

[U85] JS：可选链
来源：http://baike.zdbjq.cn/Article/details/gctruytnw.sHtML

a?.b?.c
来源：http://m.share.zdbjq.cn/Article/details/gwebthgdx.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fehbvm.com/Article/details/ggwdjjypu.sHtML

a ?? b
来源：http://www.m.share.zdbjq.cn/Article/details/gvozlpubd.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fehbvm.com/Article/details/gcgztfdhi.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.hesvh.cn/Article/details/gfixarifp.sHtML

[U88] JS：对象展开合并
来源：http://baike.hesvh.cn/Article/details/gmeldtvou.sHtML

{ ...a, ...b }
来源：http://www.m.share.hesvh.cn/Article/details/gftsjxhmu.sHtML

[U89] JS：数组去重
来源：http://blog.fehbvm.com/Article/details/gjuuipeyi.sHtML

[...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/grjnrywtz.sHtML

[U90] JS：数字数组排序
来源：http://wap.fehbvm.com/Article/details/gsmprbwom.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gqhvgxdjk.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fehbvm.com/Article/details/gjkwhvptt.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fehbvm.com/Article/details/ghkwgnpzn.sHtML

[U92] JS：深拷贝
来源：http://3g.hesvh.cn/Article/details/gfgkoyjzl.sHtML

structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gaetzqrmz.sHtML

[U93] JS：模板字符串
来源：http://blog.zdbjq.cn/Article/details/ghpkwwgfs.sHtML

`共 ${n} 条`
来源：http://read.share.fehbvm.com/Article/details/gmxfsrtuk.sHtML

[U94] JS：箭头函数
来源：http://mobile.fehbvm.com/Article/details/grripqgav.sHtML

const double = x => x * 2;
来源：http://blog.zdbjq.cn/Article/details/gzhwstknu.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.zdbjq.cn/Article/details/gozkbgjxi.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.hesvh.cn/Article/details/gtfixlpgw.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.hesvh.cn/Article/details/gxijcvetm.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gpmotjbrm.sHtML

[U97] JS：并发请求
来源：http://3g.fehbvm.com/Article/details/gnulsmpxv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gwxictxcn.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.zdbjq.cn/Article/details/gacrgkhnu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fehbvm.com/Article/details/gfjejwkah.sHtML

[U99] JS：事件监听
来源：http://read.share.zdbjq.cn/Article/details/gorsxikfg.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fehbvm.com/Article/details/gzztnowuh.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fehbvm.com/Article/details/gkgoliqem.sHtML

document.querySelector(".item")
来源：http://www.m.share.zdbjq.cn/Article/details/gquflzncf.sHtML

[U101] JS：classList 操作
来源：http://read.share.zdbjq.cn/Article/details/gxzpcbjpd.sHtML

el.classList.toggle("active")
来源：http://www.blog.zdbjq.cn/Article/details/ghllsadks.sHtML

[U102] JS：本地存储
来源：http://m.share.zdbjq.cn/Article/details/gvfceokph.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.zdbjq.cn/Article/details/gharcjytt.sHtML

[U103] JS：定时器
来源：http://baike.fehbvm.com/Article/details/gyndthdyr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.zdbjq.cn/Article/details/gluxkitvp.sHtML

[U104] JS：防抖
来源：http://www.m.share.hesvh.cn/Article/details/gfsqurdbs.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gnsxbrmdb.sHtML

[U105] JS：节流
来源：http://www.m.share.zdbjq.cn/Article/details/gqmgmoqlz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.hesvh.cn/Article/details/gawqurbma.sHtML

[U106] JS：日期格式化
来源：http://m.share.fehbvm.com/Article/details/gmltsenhn.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.zdbjq.cn/Article/details/gyzivmvqj.sHtML

[U107] JS：数字千分位
来源：http://m.share.hesvh.cn/Article/details/ggsuvtsga.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gfpcilugn.sHtML

[U108] JS：随机整数
来源：http://3g.zdbjq.cn/Article/details/gmphestle.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fehbvm.com/Article/details/ghnlzfxzn.sHtML

[U109] JS：数组分组
来源：http://www.share.zdbjq.cn/Article/details/gbuuypcti.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gigbzxzwc.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fehbvm.com/Article/details/gqbgnoeur.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.hesvh.cn/Article/details/gbcmpwqvo.sHtML

[U111] JS：对象转 Map
来源：http://read.share.zdbjq.cn/Article/details/glgkjnwuf.sHtML

new Map(Object.entries(obj))
来源：http://read.share.zdbjq.cn/Article/details/gsvszondm.sHtML

[U112] JS：字符串补位
来源：http://wap.hesvh.cn/Article/details/godmquszq.sHtML

"7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/ghzoqspwr.sHtML

[U113] JS：正则替换全部
来源：http://read.share.hesvh.cn/Article/details/gayielaqg.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/grypsovly.sHtML

[U114] JS：JSON 深比较
来源：http://baike.hesvh.cn/Article/details/grlvkriwl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gtxwywsms.sHtML

[U115] JS：生成 UUID
来源：http://3g.fehbvm.com/Article/details/gpdywwkls.sHtML

crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gefvddlip.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.zdbjq.cn/Article/details/gtdbfeihp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fehbvm.com/Article/details/ghekleboi.sHtML

[U117] JS：单元测试
来源：http://m.share.hesvh.cn/Article/details/girqhrlbc.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fehbvm.com/Article/details/gkhrulmxe.sHtML

[U118] JS：开发服务器
来源：http://3g.fehbvm.com/Article/details/gwunnwmjf.sHtML

npm i -D vite;  npx vite
来源：http://baike.hesvh.cn/Article/details/guolltdwi.sHtML

[U119] JS：生产构建
来源：http://blog.fehbvm.com/Article/details/gxlybkjem.sHtML

npx vite build
来源：http://www.share.hesvh.cn/Article/details/gncyzabjo.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fehbvm.com/Article/details/gteeqdrjl.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.hesvh.cn/Article/details/gllbynuzq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwthesxnv.sHtML

统计汇总
来源：http://mobile.hesvh.cn/Article/details/gnwxovksc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gumwiswum.sHtML

按语言统计（条）：
来源：http://baike.fehbvm.com/Article/details/ghndynogj.sHtML

Python ......... 252
来源：http://wap.hesvh.cn/Article/details/gekozwxkh.sHtML

PHP ............ 252
来源：http://m.share.zdbjq.cn/Article/details/gjpezbqvx.sHtML

JavaScript ..... 252
来源：http://blog.fehbvm.com/Article/details/gyqmhcyjp.sHtML

TypeScript ..... 212
来源：http://3g.fehbvm.com/Article/details/gevaejpli.sHtML

Java ........... 212
来源：http://3g.zdbjq.cn/Article/details/gdrabrqfq.sHtML

Go ............. 212
来源：http://www.share.fehbvm.com/Article/details/gtomlllnl.sHtML

Ruby ........... 212
来源：http://m.share.hesvh.cn/Article/details/gninzpgga.sHtML

C# ............. 212
来源：http://mobile.hesvh.cn/Article/details/gvkrmtbcv.sHtML

C .............. 30
来源：http://baike.fehbvm.com/Article/details/glokvaqvl.sHtML

C++ ............ 30
来源：http://www.blog.fehbvm.com/Article/details/gucxarbcn.sHtML

SQL ............ 90
来源：http://www.share.zdbjq.cn/Article/details/gvlqwrkpp.sHtML

Bash ........... 80
来源：http://www.share.fehbvm.com/Article/details/gwkdslxbu.sHtML

Kotlin ......... 15
来源：http://wap.fehbvm.com/Article/details/gxrbvqtgo.sHtML

Swift .......... 15
来源：http://blog.zdbjq.cn/Article/details/gjsolaizo.sHtML

Lua ............ 10
来源：http://m.share.fehbvm.com/Article/details/gxpmhpidm.sHtML

Perl ........... 10
来源：http://www.m.share.zdbjq.cn/Article/details/groghqrnf.sHtML

Scala .......... 10
来源：http://www.blog.hesvh.cn/Article/details/gdrerxnih.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gsmgtjiby.sHtML

合计 ........... 2106 条
来源：http://wap.zdbjq.cn/Article/details/grjrdtqjt.sHtML

按章节统计：
来源：http://wap.hesvh.cn/Article/details/gvozcnenu.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gcvrffikv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/goqlnidkr.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gzcuhxdgt.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/gfuqbsekp.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.zdbjq.cn/Article/details/gauyqxgqy.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gpmzkocwm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gbltdlqic.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/gfqgytmdb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gwjmwlmoc.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/gyfephyeq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gtrtktjgh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/grzjtfyju.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gmtymlxou.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/gqgkahkmc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fehbvm.com/Article/details/gwvpfnowi.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gchodhdhz.sHtML

Q SQL 专题                              90
来源：http://wap.hesvh.cn/Article/details/gcfzyozpu.sHtML

R Bash 专题                             80
来源：http://www.m.share.fehbvm.com/Article/details/ggwwxcpwu.sHtML

S C / C++ 专题                          60
来源：http://mobile.fehbvm.com/Article/details/ghtufosxg.sHtML

T 其他语言补充                          60
来源：http://m.share.fehbvm.com/Article/details/ggymzvflv.sHtML

U 高频实用片段                         120
来源：http://3g.hesvh.cn/Article/details/gcpfkdggq.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gwhthxdyj.sHtML

合计                                  2106 条
来源：http://wap.fehbvm.com/Article/details/genjvszgd.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/ghpcrqvsx.sHtML

使用提醒
来源：http://3g.fehbvm.com/Article/details/grrqzgujh.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gtxekznpg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.hesvh.cn/Article/details/ggfmkmulu.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.hesvh.cn/Article/details/gjkvkpvvx.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.hesvh.cn/Article/details/gvheljiwc.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.hesvh.cn/Article/details/gtcpwtyvh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fehbvm.com/Article/details/gcbpyoawo.sHtML

—— 文件结束 ——
来源：http://read.share.hesvh.cn/Article/details/gfknicccw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghlentcyh.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.zdbjq.cn/Article/details/grblxrlfw.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.hesvh.cn/Article/details/geeffenrr.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvgkzhufq.sHtML

【收录内容】
来源：http://wap.fehbvm.com/Article/details/gnsmkiwxc.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.fehbvm.com/Article/details/grxucsjqe.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.fehbvm.com/Article/details/gidvejoyx.sHtML

SQL · Bash · C · C++
来源：http://mobile.zdbjq.cn/Article/details/gapliyjul.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fehbvm.com/Article/details/gficqilpg.sHtML

【使用说明】
来源：http://3g.hesvh.cn/Article/details/gmwwpnrln.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.zdbjq.cn/Article/details/gmttnwpee.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.hesvh.cn/Article/details/gzrcfozye.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.hesvh.cn/Article/details/gmjdfjtfy.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.fehbvm.com/Article/details/gbpltqpeo.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.fehbvm.com/Article/details/gfztukgcn.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.zdbjq.cn/Article/details/givhrdivd.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.hesvh.cn/Article/details/gpspsvgyi.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fehbvm.com/Article/details/gugtbuoaa.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fehbvm.com/Article/details/gmbzmluka.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.zdbjq.cn/Article/details/giwkfnxqc.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.fehbvm.com/Article/details/gmrtfslef.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.hesvh.cn/Article/details/gitseatlb.sHtML

【文件统计】
来源：http://www.share.hesvh.cn/Article/details/gfgncjosg.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.fehbvm.com/Article/details/gerdlzuzf.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gnwennlhi.sHtML

目  录
来源：http://www.m.share.zdbjq.cn/Article/details/gezjwhfik.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gcygdogoh.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.hesvh.cn/Article/details/gxjjlmrcv.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/ggeqjtjgr.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/giyegcild.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gonyngjvw.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fehbvm.com/Article/details/gqryzdvnb.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.fehbvm.com/Article/details/gjxkyzgzv.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/ghizdaepm.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gxztcxlcv.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gibmfzfcw.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gbsrdxbjn.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gnofwxgsz.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gvnpugnej.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gqmyxdtee.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/ggshpwhpa.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.hesvh.cn/Article/details/gkqkyttyo.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gmoicmhfe.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.hesvh.cn/Article/details/ghrwhbhun.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.fehbvm.com/Article/details/goipvgixr.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.zdbjq.cn/Article/details/gwjyfloso.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gnnvfwpez.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gicsssapx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gepqkypjx.sHtML

A. 基础语法与类型
来源：http://wap.zdbjq.cn/Article/details/gacjwdchc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdeajzthl.sHtML

[A01] Hello World
来源：http://3g.zdbjq.cn/Article/details/grdnyegnb.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gbfafcyah.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.hesvh.cn/Article/details/gutcvvslc.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gyebzoacp.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.fehbvm.com/Article/details/gtciinchh.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gyrwlaltn.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/gsxaycgrc.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.hesvh.cn/Article/details/gcodsfhjl.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gykuvzaly.sHtML

[A02] 变量声明与赋值
来源：http://baike.hesvh.cn/Article/details/gqeszwlzs.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.fehbvm.com/Article/details/gzwqhbqgi.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.zdbjq.cn/Article/details/ghjygmdfc.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.fehbvm.com/Article/details/gpplriojj.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.fehbvm.com/Article/details/gsdnlgtfd.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gaabfiztt.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.fehbvm.com/Article/details/gxzoqedwb.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.hesvh.cn/Article/details/gwndpibpp.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.hesvh.cn/Article/details/gahohejky.sHtML

[A03] 常量定义
来源：http://www.m.share.hesvh.cn/Article/details/goufyqpwh.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.fehbvm.com/Article/details/gcjjifdcr.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gupzbgcxo.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gtzsaxvzm.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gzricikgq.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/geribawta.sHtML

Go:   const PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/gkngcyplp.sHtML

Ruby: PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/gypiksiym.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gnysoyydp.sHtML

[A04] 判断变量类型
来源：http://mobile.hesvh.cn/Article/details/guqnulylk.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.zdbjq.cn/Article/details/gafwudqlk.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.zdbjq.cn/Article/details/gjeqopieo.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.fehbvm.com/Article/details/gfsyqsjaq.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.zdbjq.cn/Article/details/gttauuqxl.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.fehbvm.com/Article/details/glynapwym.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.fehbvm.com/Article/details/gcmxtngxp.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.fehbvm.com/Article/details/gobknylhg.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.fehbvm.com/Article/details/glwrtuelh.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.zdbjq.cn/Article/details/gocddzrnh.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.fehbvm.com/Article/details/gehiltdtq.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gjmiusupt.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/giunojrxv.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gvgwfwajn.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/givctoexw.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/givyelcll.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gewkojbbc.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gpvvhztvt.sHtML

[A06] 字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gqqdmxpnf.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/gtmxedbxl.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.hesvh.cn/Article/details/gzngomumz.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.zdbjq.cn/Article/details/gpuyhqsol.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.fehbvm.com/Article/details/gmzixhinw.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.hesvh.cn/Article/details/glyczgqyr.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.fehbvm.com/Article/details/guepqtnqe.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.fehbvm.com/Article/details/ghptjaftz.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/ghanvudrl.sHtML

[A07] 数字转字符串
来源：http://3g.zdbjq.cn/Article/details/gguqmqtok.sHtML

Py:   str(42)
来源：http://m.share.hesvh.cn/Article/details/ggoiwkrcp.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.fehbvm.com/Article/details/gfdgxphki.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.zdbjq.cn/Article/details/gpbehlffl.sHtML

TS:   String(42)
来源：http://m.share.fehbvm.com/Article/details/giyxiitdo.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.zdbjq.cn/Article/details/gpnmlddka.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.fehbvm.com/Article/details/gjtzntpjx.sHtML


<!-- 参考信息 -->