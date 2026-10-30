代发 wailian999

[U53] PHP：空合并运算符
来源：http://www.m.share.hesvh.cn/Article/details/guluqvnhg.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.zdbjq.cn/Article/details/gdpaxwrbc.sHtML

[U54] PHP：空安全调用
来源：http://baike.hesvh.cn/Article/details/grmxmvsts.sHtML

$obj?->method()
来源：http://3g.zdbjq.cn/Article/details/gxgewrbwq.sHtML

[U55] PHP：match 表达式
来源：http://blog.hesvh.cn/Article/details/gkljvaxvm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/gmgdmkvdb.sHtML

[U56] PHP：命名参数
来源：http://wap.fehbvm.com/Article/details/gyconhvvz.sHtML

f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gjnfgxaag.sHtML

[U57] PHP：字符串插值
来源：http://wap.fehbvm.com/Article/details/gazgxpvbp.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/ggtwasvcg.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.hesvh.cn/Article/details/geutveqyj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gavbczeuq.sHtML

[U59] PHP：自定义排序
来源：http://blog.hesvh.cn/Article/details/gzfollpti.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gjrlsimhh.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.hesvh.cn/Article/details/gpupwzlor.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fehbvm.com/Article/details/gstisbtkn.sHtML

[U61] PHP：正则
来源：http://3g.fehbvm.com/Article/details/gzsvfbkxh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gklduzhye.sHtML

[U62] PHP：日期对象
来源：http://www.blog.hesvh.cn/Article/details/gtrvcqjdp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.zdbjq.cn/Article/details/gweerjgft.sHtML

[U63] PHP：文件读写
来源：http://blog.hesvh.cn/Article/details/gicwlbyan.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fehbvm.com/Article/details/gjtvzrksk.sHtML

[U64] PHP：目录遍历
来源：http://read.share.zdbjq.cn/Article/details/gazthlwqe.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.zdbjq.cn/Article/details/gxkavtbon.sHtML

[U65] PHP：会话
来源：http://m.share.hesvh.cn/Article/details/gpcrnonuz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gobsfkmwn.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fehbvm.com/Article/details/gpdnnhqcl.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fehbvm.com/Article/details/gdmvdrxrj.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.zdbjq.cn/Article/details/gbchxqwso.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.hesvh.cn/Article/details/gorlfllip.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fehbvm.com/Article/details/gyewmzpbq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fehbvm.com/Article/details/gsmqnpipa.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.zdbjq.cn/Article/details/ggjdrmutd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.hesvh.cn/Article/details/gtjuvislq.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.hesvh.cn/Article/details/gzzwudnhv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.hesvh.cn/Article/details/guiejgeqd.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gvxbuchhp.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.hesvh.cn/Article/details/ghxdchbih.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fehbvm.com/Article/details/galhqwoqx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.hesvh.cn/Article/details/gszgunutb.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fehbvm.com/Article/details/gyxttlsvh.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.zdbjq.cn/Article/details/gxfayzncf.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gvjzsmyzb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.hesvh.cn/Article/details/gtykxzmwh.sHtML

[U75] PHP：依赖注入
来源：http://m.share.zdbjq.cn/Article/details/gzbjsfmqn.sHtML

composer require psr/container
来源：http://blog.hesvh.cn/Article/details/gnswccmhc.sHtML

[U76] PHP：简单路由
来源：http://read.share.hesvh.cn/Article/details/gucioltyu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fehbvm.com/Article/details/gjnezdzcj.sHtML

[U77] PHP：模板渲染
来源：http://wap.hesvh.cn/Article/details/gszdsuhno.sHtML

composer require twig/twig
来源：http://m.share.zdbjq.cn/Article/details/gqyicvdpc.sHtML

[U78] PHP：单元测试
来源：http://www.share.fehbvm.com/Article/details/gdyniftnu.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.hesvh.cn/Article/details/gjeceupqc.sHtML

[U79] PHP：静态分析
来源：http://read.share.zdbjq.cn/Article/details/gwreujgmk.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fehbvm.com/Article/details/gpimjmyvg.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fehbvm.com/Article/details/gbxbrbuit.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.zdbjq.cn/Article/details/gqzusspad.sHtML

[U81] JS：初始化项目
来源：http://www.share.fehbvm.com/Article/details/ghrlviqnt.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/gxbxskbrj.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fehbvm.com/Article/details/glauyxhfk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.zdbjq.cn/Article/details/gvxgumbfa.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fehbvm.com/Article/details/goumgcapp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gphozqcak.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fehbvm.com/Article/details/gzyhzspxp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.hesvh.cn/Article/details/gtfmiesuk.sHtML

[U85] JS：可选链
来源：http://baike.fehbvm.com/Article/details/gkepjurxg.sHtML

a?.b?.c
来源：http://blog.fehbvm.com/Article/details/gmnjrzeks.sHtML

[U86] JS：空值合并
来源：http://read.share.hesvh.cn/Article/details/geaayweux.sHtML

a ?? b
来源：http://www.m.share.zdbjq.cn/Article/details/griigxzqi.sHtML

[U87] JS：解构默认值
来源：http://wap.hesvh.cn/Article/details/gwelartcj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fehbvm.com/Article/details/gyxztzhow.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.hesvh.cn/Article/details/giurycsfu.sHtML

{ ...a, ...b }
来源：http://m.share.zdbjq.cn/Article/details/gbncqkwoe.sHtML

[U89] JS：数组去重
来源：http://m.share.hesvh.cn/Article/details/gpnhohfjv.sHtML

[...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gtwmdgwmg.sHtML

[U90] JS：数字数组排序
来源：http://read.share.hesvh.cn/Article/details/gupzcpowe.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gpjmciutf.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fehbvm.com/Article/details/gmfidoxtr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fehbvm.com/Article/details/gxkfdaemp.sHtML

[U92] JS：深拷贝
来源：http://www.share.fehbvm.com/Article/details/gehzbwyxs.sHtML

structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gdfmpuphq.sHtML

[U93] JS：模板字符串
来源：http://wap.hesvh.cn/Article/details/geznofysg.sHtML

`共 ${n} 条`
来源：http://read.share.hesvh.cn/Article/details/gaclifzzm.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gksyyblap.sHtML

const double = x => x * 2;
来源：http://blog.fehbvm.com/Article/details/gaowfupja.sHtML

[U95] JS：Promise 包装
来源：http://baike.fehbvm.com/Article/details/gsovcomnx.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fehbvm.com/Article/details/gvctntezh.sHtML

[U96] JS：async/await 与异常
来源：http://blog.zdbjq.cn/Article/details/gbcrvnztx.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gtshnkmfn.sHtML

[U97] JS：并发请求
来源：http://mobile.hesvh.cn/Article/details/gijkwyvlc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gfoixylns.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.zdbjq.cn/Article/details/gmxtfvhmu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fehbvm.com/Article/details/gvwtnirne.sHtML

[U99] JS：事件监听
来源：http://mobile.fehbvm.com/Article/details/gnkmzclal.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.hesvh.cn/Article/details/gtkooigcm.sHtML

[U100] JS：DOM 查询
来源：http://read.share.zdbjq.cn/Article/details/gtcanrpyb.sHtML

document.querySelector(".item")
来源：http://www.m.share.hesvh.cn/Article/details/gfbkkwikd.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fehbvm.com/Article/details/gvsgdhlzr.sHtML

el.classList.toggle("active")
来源：http://read.share.fehbvm.com/Article/details/gyrkmipti.sHtML

[U102] JS：本地存储
来源：http://www.m.share.zdbjq.cn/Article/details/gpfwyture.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fehbvm.com/Article/details/guasyijet.sHtML

[U103] JS：定时器
来源：http://m.share.hesvh.cn/Article/details/gnawmovrf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.hesvh.cn/Article/details/ghfqdvhgv.sHtML

[U104] JS：防抖
来源：http://wap.hesvh.cn/Article/details/gkjvogaoi.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/ggsqdggut.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/gkvgbkszy.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.zdbjq.cn/Article/details/gywekvxmf.sHtML

[U106] JS：日期格式化
来源：http://m.share.fehbvm.com/Article/details/gdgyltkkf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.hesvh.cn/Article/details/gazwselxc.sHtML

[U107] JS：数字千分位
来源：http://3g.fehbvm.com/Article/details/ggelbxgyu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gdhlovzvo.sHtML

[U108] JS：随机整数
来源：http://wap.hesvh.cn/Article/details/gtbxckzdg.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.zdbjq.cn/Article/details/gzzvasupf.sHtML

[U109] JS：数组分组
来源：http://mobile.fehbvm.com/Article/details/gcqurmypa.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gumwrfqrd.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fehbvm.com/Article/details/gnpliwqcz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.zdbjq.cn/Article/details/gvaipslti.sHtML

[U111] JS：对象转 Map
来源：http://wap.fehbvm.com/Article/details/gesasguif.sHtML

new Map(Object.entries(obj))
来源：http://baike.fehbvm.com/Article/details/gcjogddun.sHtML

[U112] JS：字符串补位
来源：http://wap.hesvh.cn/Article/details/greuerlbx.sHtML

"7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gtgzpnbvw.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fehbvm.com/Article/details/gunlmqbxj.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gyhlsevyd.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.zdbjq.cn/Article/details/gnnmperye.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/ggvjqojkt.sHtML

[U115] JS：生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gzrjsdfao.sHtML

crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/geipguknf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/gwqcfzvot.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.hesvh.cn/Article/details/gatmhpyue.sHtML

[U117] JS：单元测试
来源：http://www.share.hesvh.cn/Article/details/gwnzwuude.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/grswmyfck.sHtML

[U118] JS：开发服务器
来源：http://blog.fehbvm.com/Article/details/gajjfadle.sHtML

npm i -D vite;  npx vite
来源：http://3g.zdbjq.cn/Article/details/gezvxpurk.sHtML

[U119] JS：生产构建
来源：http://3g.fehbvm.com/Article/details/gmimfikwf.sHtML

npx vite build
来源：http://www.m.share.zdbjq.cn/Article/details/gplqusbki.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.hesvh.cn/Article/details/gutkjkwnd.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.zdbjq.cn/Article/details/glvptrckn.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzxmtvihg.sHtML

统计汇总
来源：http://3g.fehbvm.com/Article/details/gvgomuevf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzxsqyycb.sHtML

按语言统计（条）：
来源：http://www.share.hesvh.cn/Article/details/gjnrmsdcw.sHtML

Python ......... 252
来源：http://3g.fehbvm.com/Article/details/gqlghrauq.sHtML

PHP ............ 252
来源：http://www.blog.zdbjq.cn/Article/details/grophycwu.sHtML

JavaScript ..... 252
来源：http://mobile.zdbjq.cn/Article/details/gladrtxwk.sHtML

TypeScript ..... 212
来源：http://blog.fehbvm.com/Article/details/gxuzogkfk.sHtML

Java ........... 212
来源：http://wap.zdbjq.cn/Article/details/gvzxvtizd.sHtML

Go ............. 212
来源：http://3g.fehbvm.com/Article/details/gevskqbxu.sHtML

Ruby ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gmkffmcfo.sHtML

C# ............. 212
来源：http://read.share.fehbvm.com/Article/details/gmolerqmr.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/gwgyndxta.sHtML

C++ ............ 30
来源：http://www.m.share.hesvh.cn/Article/details/gaibepukm.sHtML

SQL ............ 90
来源：http://blog.zdbjq.cn/Article/details/grxlwbist.sHtML

Bash ........... 80
来源：http://baike.hesvh.cn/Article/details/gohfbkepr.sHtML

Kotlin ......... 15
来源：http://blog.fehbvm.com/Article/details/gxzedqvyh.sHtML

Swift .......... 15
来源：http://baike.fehbvm.com/Article/details/gymkrvduo.sHtML

Lua ............ 10
来源：http://baike.fehbvm.com/Article/details/gryzyecla.sHtML

Perl ........... 10
来源：http://wap.hesvh.cn/Article/details/glpbctgee.sHtML

Scala .......... 10
来源：http://m.share.zdbjq.cn/Article/details/gtxxfkmgf.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gwygkdjya.sHtML

合计 ........... 2106 条
来源：http://baike.hesvh.cn/Article/details/gabxwbtjk.sHtML

按章节统计：
来源：http://blog.hesvh.cn/Article/details/ghrumbndb.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gjuufopgo.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gdmdcgvvh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gckvtzkkj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gsdsfpvou.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.zdbjq.cn/Article/details/gyrzazilh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gzkdmeimt.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gqyfpzsoq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/gqwbxyncd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gbizjtufn.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gwklgfqwo.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/grnnqseoz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gdxafnmlt.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gbkkezqev.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gpklgvkrz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.hesvh.cn/Article/details/gzpedrqfd.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/ghryqpjee.sHtML

Q SQL 专题                              90
来源：http://wap.hesvh.cn/Article/details/gldgdprdp.sHtML

R Bash 专题                             80
来源：http://baike.fehbvm.com/Article/details/gvsqzszqn.sHtML

S C / C++ 专题                          60
来源：http://www.share.hesvh.cn/Article/details/gronrazch.sHtML

T 其他语言补充                          60
来源：http://www.blog.hesvh.cn/Article/details/grgzbrtex.sHtML

U 高频实用片段                         120
来源：http://3g.hesvh.cn/Article/details/gqvsuhbaj.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gtrzoteeo.sHtML

合计                                  2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gxczdriaa.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gpczlleqw.sHtML

使用提醒
来源：http://3g.fehbvm.com/Article/details/gbkakrmhy.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gzraufray.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.hesvh.cn/Article/details/gfdhqbyms.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.hesvh.cn/Article/details/gcyekjyvj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.hesvh.cn/Article/details/gdaaqyffm.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fehbvm.com/Article/details/ggnjkpjsr.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fehbvm.com/Article/details/gfwfjcbec.sHtML

—— 文件结束 ——
来源：http://www.m.share.hesvh.cn/Article/details/girdfmvub.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzlxkqsvi.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fehbvm.com/Article/details/gzacjvrwo.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fehbvm.com/Article/details/gpwohlxix.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwslohvew.sHtML

【收录内容】
来源：http://www.share.zdbjq.cn/Article/details/geufiwvbx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.hesvh.cn/Article/details/gmhhuebgp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.hesvh.cn/Article/details/gykxqafft.sHtML

SQL · Bash · C · C++
来源：http://mobile.zdbjq.cn/Article/details/gneinyeby.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.fehbvm.com/Article/details/gaqggwmyi.sHtML

【使用说明】
来源：http://read.share.zdbjq.cn/Article/details/gxxduhfdr.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.hesvh.cn/Article/details/ghhtoeyyc.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.fehbvm.com/Article/details/gphfirtar.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.fehbvm.com/Article/details/ggqyrvyxc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.hesvh.cn/Article/details/gaxgmbqrl.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.fehbvm.com/Article/details/gqdwawewh.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.fehbvm.com/Article/details/gchompdcu.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.zdbjq.cn/Article/details/giqojuphn.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.fehbvm.com/Article/details/glxcbymbl.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.hesvh.cn/Article/details/gibkyyqcx.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.hesvh.cn/Article/details/gfprpdofn.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.zdbjq.cn/Article/details/gcqcbmawb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.zdbjq.cn/Article/details/gglgwkfpf.sHtML

【文件统计】
来源：http://m.share.hesvh.cn/Article/details/gdrifbfnp.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.zdbjq.cn/Article/details/geskjqekn.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gvvhwcwih.sHtML

目  录
来源：http://mobile.fehbvm.com/Article/details/gmjsplymq.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gffenmyzr.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.fehbvm.com/Article/details/gckvicufm.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gawvdhbec.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/gkwccoxdt.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/gzwnlzsai.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.hesvh.cn/Article/details/ggzxfefqw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.fehbvm.com/Article/details/gggwextwd.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gedaasjbf.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gnspeejtl.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/grcjnggmc.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gaqmruzzq.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gnmcquvho.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gbkaeffpp.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gmpwswohm.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.zdbjq.cn/Article/details/gvzvjqpny.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fehbvm.com/Article/details/gfqzxrgfg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gugkvgizp.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.fehbvm.com/Article/details/gxddrltuv.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.fehbvm.com/Article/details/gtypyvuom.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.fehbvm.com/Article/details/gfbrtdqcw.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gigmqlmej.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/gpeynxxie.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjryhfyhy.sHtML

A. 基础语法与类型
来源：http://3g.hesvh.cn/Article/details/guhwlmlfr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfzlaqlpo.sHtML

[A01] Hello World
来源：http://www.share.hesvh.cn/Article/details/gbpqtcdqw.sHtML

Py:   print("Hello, World!")
来源：http://baike.fehbvm.com/Article/details/ghwdalwpb.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.hesvh.cn/Article/details/gvrvvpzyr.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/ggpxthlej.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.fehbvm.com/Article/details/gkxhkhvll.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gfoolqaua.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.zdbjq.cn/Article/details/ggxnbogkz.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.hesvh.cn/Article/details/gbowxdnku.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/giyaprhnk.sHtML

[A02] 变量声明与赋值
来源：http://baike.hesvh.cn/Article/details/gxxmtypba.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.fehbvm.com/Article/details/glbvkndqs.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gefoosifq.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gkqtzsksb.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.fehbvm.com/Article/details/gvoezjkcs.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/ghmyndqew.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.fehbvm.com/Article/details/gwazbffrg.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.zdbjq.cn/Article/details/gufhedfqp.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/glulpjwdt.sHtML

[A03] 常量定义
来源：http://www.m.share.zdbjq.cn/Article/details/gtlwnmxln.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.zdbjq.cn/Article/details/gkhtlaatu.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/grifujene.sHtML

JS:   const PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/grhvjvmns.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gxchxqcto.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gjjwzzmzg.sHtML

Go:   const PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/gtbquwqjk.sHtML

Ruby: PI = 3.14159
来源：http://m.share.fehbvm.com/Article/details/gwgridduz.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gyowusikc.sHtML

[A04] 判断变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gajkrepts.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.zdbjq.cn/Article/details/gknsoyugf.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.zdbjq.cn/Article/details/gdqbojmpj.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/gvushkken.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.zdbjq.cn/Article/details/gormfdacg.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.hesvh.cn/Article/details/gbdqikirx.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.fehbvm.com/Article/details/gihnjeunf.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.zdbjq.cn/Article/details/gxinbyvyc.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.hesvh.cn/Article/details/ghzyvjvvs.sHtML

[A05] 整数除法与取模
来源：http://www.share.fehbvm.com/Article/details/grwoviplt.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.zdbjq.cn/Article/details/gpzomdfzj.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.hesvh.cn/Article/details/gwggslcsg.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gjgqxinys.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.zdbjq.cn/Article/details/goujdfkil.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gchwkorki.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gglbxtqjc.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gcpbfzdub.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gdsdnilas.sHtML

[A06] 字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gsljgblzo.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.fehbvm.com/Article/details/giqdunqtv.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.hesvh.cn/Article/details/gqqlujpnq.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.hesvh.cn/Article/details/gjvxzzhnn.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.zdbjq.cn/Article/details/gpambhxbf.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.fehbvm.com/Article/details/gmepotjiq.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.zdbjq.cn/Article/details/gzpdoqome.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.zdbjq.cn/Article/details/gucmiofhb.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.hesvh.cn/Article/details/gkilvovve.sHtML

[A07] 数字转字符串
来源：http://baike.hesvh.cn/Article/details/gycflwyoq.sHtML

Py:   str(42)
来源：http://3g.hesvh.cn/Article/details/gqfuzosrl.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.fehbvm.com/Article/details/gaeeacxvk.sHtML


<!-- 参考信息 -->