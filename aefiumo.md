代发 wailian999

[U49] PHP：只读属性
来源：http://blog.fehbvm.com/Article/details/gdnclkljn.sHtML

public readonly string $name
来源：http://read.share.fehbvm.com/Article/details/glzguarom.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.hesvh.cn/Article/details/gualmmoxs.sHtML

public function __construct(private int $id) {}
来源：http://baike.fehbvm.com/Article/details/gojmwytfg.sHtML

[U51] PHP：数组解构
来源：http://m.share.fehbvm.com/Article/details/gblaajkcv.sHtML

[$a, $b] = $arr;
来源：http://wap.fehbvm.com/Article/details/gsalzsnwg.sHtML

[U52] PHP：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gftqgddpj.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fehbvm.com/Article/details/gdbyjxick.sHtML

[U53] PHP：空合并运算符
来源：http://wap.zdbjq.cn/Article/details/gfyrkjepp.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fehbvm.com/Article/details/ghcvnqajx.sHtML

[U54] PHP：空安全调用
来源：http://blog.zdbjq.cn/Article/details/gamqfbhco.sHtML

$obj?->method()
来源：http://www.share.fehbvm.com/Article/details/gffyzfvvj.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fehbvm.com/Article/details/garesduhb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fehbvm.com/Article/details/grxnlwvyv.sHtML

[U56] PHP：命名参数
来源：http://read.share.fehbvm.com/Article/details/gjkffmhaw.sHtML

f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gdnnfanfa.sHtML

[U57] PHP：字符串插值
来源：http://baike.zdbjq.cn/Article/details/ggxhhvlqe.sHtML

"值: {$a}"
来源：http://read.share.hesvh.cn/Article/details/gesrtowvv.sHtML

[U58] PHP：数组三件套
来源：http://read.share.hesvh.cn/Article/details/gpajaugkm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fehbvm.com/Article/details/gfgvhnvww.sHtML

[U59] PHP：自定义排序
来源：http://www.share.zdbjq.cn/Article/details/guvodbzxz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/gzochcnjy.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.zdbjq.cn/Article/details/gdtahtlmi.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.hesvh.cn/Article/details/gjtsljkeq.sHtML

[U61] PHP：正则
来源：http://www.blog.fehbvm.com/Article/details/gtfgvfofl.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gociwotzw.sHtML

[U62] PHP：日期对象
来源：http://3g.hesvh.cn/Article/details/gqxrvkvxb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fehbvm.com/Article/details/gwvglqvnj.sHtML

[U63] PHP：文件读写
来源：http://3g.zdbjq.cn/Article/details/goidzmxcg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.hesvh.cn/Article/details/gmifokkbl.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fehbvm.com/Article/details/ghjqwwcrv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.hesvh.cn/Article/details/ghiogdggm.sHtML

[U65] PHP：会话
来源：http://mobile.hesvh.cn/Article/details/gsfnmivre.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.hesvh.cn/Article/details/gtuwuvmmt.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.hesvh.cn/Article/details/gyikbgpgc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fehbvm.com/Article/details/gvpmbtqpm.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/gxiouafkb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fehbvm.com/Article/details/gpguzuiqh.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.hesvh.cn/Article/details/grilyzpmk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fehbvm.com/Article/details/gxzxhuoqz.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.hesvh.cn/Article/details/gthkhlnux.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fehbvm.com/Article/details/gkyhuanqv.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fehbvm.com/Article/details/gtstaiizz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.hesvh.cn/Article/details/ggkpdxmnh.sHtML

[U71] PHP：抛出异常
来源：http://baike.zdbjq.cn/Article/details/gmeefnfun.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.zdbjq.cn/Article/details/ggaxbslfl.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fehbvm.com/Article/details/gxnvdkjtp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.zdbjq.cn/Article/details/gsrclgeri.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.hesvh.cn/Article/details/gltqltfch.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.zdbjq.cn/Article/details/gffgcctlk.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gkypldpxm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.hesvh.cn/Article/details/glyalfixf.sHtML

[U75] PHP：依赖注入
来源：http://3g.fehbvm.com/Article/details/gibltdqsg.sHtML

composer require psr/container
来源：http://baike.zdbjq.cn/Article/details/gitjzwasr.sHtML

[U76] PHP：简单路由
来源：http://www.share.fehbvm.com/Article/details/gumolbadh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.zdbjq.cn/Article/details/gjdwptaxz.sHtML

[U77] PHP：模板渲染
来源：http://wap.zdbjq.cn/Article/details/gwkxmneat.sHtML

composer require twig/twig
来源：http://mobile.fehbvm.com/Article/details/gqjlqhewk.sHtML

[U78] PHP：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gwmpkujwn.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.zdbjq.cn/Article/details/gypeclxkv.sHtML

[U79] PHP：静态分析
来源：http://wap.hesvh.cn/Article/details/gmcwngnwv.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fehbvm.com/Article/details/gtywdmtsh.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fehbvm.com/Article/details/gwmiscgxo.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.zdbjq.cn/Article/details/gzcgnyrhg.sHtML

[U81] JS：初始化项目
来源：http://mobile.zdbjq.cn/Article/details/gzmmwngjg.sHtML

npm init -y;  npm i express
来源：http://blog.fehbvm.com/Article/details/grzbodjfq.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.zdbjq.cn/Article/details/gzfavvodv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fehbvm.com/Article/details/gqtnjjmvw.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.zdbjq.cn/Article/details/gpvmmrkxk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gzznlbulp.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fehbvm.com/Article/details/gfmrjlsqn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.hesvh.cn/Article/details/ghlcmmzqs.sHtML

[U85] JS：可选链
来源：http://www.blog.zdbjq.cn/Article/details/gvlmgdhru.sHtML

a?.b?.c
来源：http://read.share.zdbjq.cn/Article/details/gkgentcrq.sHtML

[U86] JS：空值合并
来源：http://mobile.fehbvm.com/Article/details/ghfrjxwee.sHtML

a ?? b
来源：http://www.share.hesvh.cn/Article/details/ghdxonesb.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fehbvm.com/Article/details/gtfwnvgba.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fehbvm.com/Article/details/glzkhrasd.sHtML

[U88] JS：对象展开合并
来源：http://read.share.zdbjq.cn/Article/details/grnajhdfe.sHtML

{ ...a, ...b }
来源：http://3g.hesvh.cn/Article/details/gssoifedu.sHtML

[U89] JS：数组去重
来源：http://mobile.hesvh.cn/Article/details/grxxxcayp.sHtML

[...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gfnhghhhx.sHtML

[U90] JS：数字数组排序
来源：http://baike.zdbjq.cn/Article/details/golfuqldp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gkavamkyy.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fehbvm.com/Article/details/gtzuwhtnu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.zdbjq.cn/Article/details/gbsyhrfku.sHtML

[U92] JS：深拷贝
来源：http://baike.fehbvm.com/Article/details/gcbxdxacn.sHtML

structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gmrysrljf.sHtML

[U93] JS：模板字符串
来源：http://wap.hesvh.cn/Article/details/gqqwntvkc.sHtML

`共 ${n} 条`
来源：http://blog.fehbvm.com/Article/details/gwpshwzit.sHtML

[U94] JS：箭头函数
来源：http://3g.hesvh.cn/Article/details/gxscmazrk.sHtML

const double = x => x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gbhmzimkk.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fehbvm.com/Article/details/gtnlybdin.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fehbvm.com/Article/details/givdilibp.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.zdbjq.cn/Article/details/gsarsbwju.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gmixxctyh.sHtML

[U97] JS：并发请求
来源：http://3g.fehbvm.com/Article/details/gbakizhla.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gfhmuipxg.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.zdbjq.cn/Article/details/gmskstvcr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.zdbjq.cn/Article/details/gayxaidfj.sHtML

[U99] JS：事件监听
来源：http://mobile.fehbvm.com/Article/details/gonoqeile.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.hesvh.cn/Article/details/gmfwrphju.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/glfntmugf.sHtML

document.querySelector(".item")
来源：http://read.share.hesvh.cn/Article/details/gysscrljh.sHtML

[U101] JS：classList 操作
来源：http://wap.hesvh.cn/Article/details/gcxyxmwzn.sHtML

el.classList.toggle("active")
来源：http://read.share.hesvh.cn/Article/details/gbjzdpkbx.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/gmjrgxteh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.zdbjq.cn/Article/details/gyfmirkzz.sHtML

[U103] JS：定时器
来源：http://wap.zdbjq.cn/Article/details/glgtumwxs.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fehbvm.com/Article/details/gwdzjtxwr.sHtML

[U104] JS：防抖
来源：http://3g.fehbvm.com/Article/details/gkdicvamu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gskstnwvg.sHtML

[U105] JS：节流
来源：http://wap.hesvh.cn/Article/details/gbdgtrryt.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fehbvm.com/Article/details/gwqbmzjwj.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gosggprdy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fehbvm.com/Article/details/gdgakkcta.sHtML

[U107] JS：数字千分位
来源：http://m.share.hesvh.cn/Article/details/gsxutixgp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gpruezvpn.sHtML

[U108] JS：随机整数
来源：http://baike.fehbvm.com/Article/details/gyxdcaxuu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.hesvh.cn/Article/details/gbbxydtcc.sHtML

[U109] JS：数组分组
来源：http://wap.hesvh.cn/Article/details/gjeligbfq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gywcllgih.sHtML

[U110] JS：数组分块
来源：http://blog.zdbjq.cn/Article/details/glvnlljrs.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.hesvh.cn/Article/details/gvqtqfeee.sHtML

[U111] JS：对象转 Map
来源：http://wap.zdbjq.cn/Article/details/gdgakdiff.sHtML

new Map(Object.entries(obj))
来源：http://3g.fehbvm.com/Article/details/gnckpchxh.sHtML

[U112] JS：字符串补位
来源：http://blog.zdbjq.cn/Article/details/grcfaudtx.sHtML

"7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gqkqwunti.sHtML

[U113] JS：正则替换全部
来源：http://mobile.hesvh.cn/Article/details/goyftenff.sHtML

s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gfeuzeaqn.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fehbvm.com/Article/details/gwltdxwbz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gtmrcoyip.sHtML

[U115] JS：生成 UUID
来源：http://m.share.hesvh.cn/Article/details/ggmhmedzh.sHtML

crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gctknqpjb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.hesvh.cn/Article/details/gukgygzkg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fehbvm.com/Article/details/giyisstug.sHtML

[U117] JS：单元测试
来源：http://read.share.hesvh.cn/Article/details/gdaqbjkdq.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.zdbjq.cn/Article/details/gjzllllen.sHtML

[U118] JS：开发服务器
来源：http://wap.zdbjq.cn/Article/details/gqmhgsage.sHtML

npm i -D vite;  npx vite
来源：http://mobile.zdbjq.cn/Article/details/gtidjsssa.sHtML

[U119] JS：生产构建
来源：http://read.share.fehbvm.com/Article/details/gbnahngyn.sHtML

npx vite build
来源：http://www.m.share.zdbjq.cn/Article/details/gherwomxn.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.zdbjq.cn/Article/details/ggxoyddnr.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fehbvm.com/Article/details/gqlqunujn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpdyzcuyw.sHtML

统计汇总
来源：http://blog.fehbvm.com/Article/details/goirofehi.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqnwijcfv.sHtML

按语言统计（条）：
来源：http://wap.hesvh.cn/Article/details/gefqrtncj.sHtML

Python ......... 252
来源：http://wap.zdbjq.cn/Article/details/gjdqpfyrn.sHtML

PHP ............ 252
来源：http://www.share.hesvh.cn/Article/details/gvqhojzjg.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/gcqmwfzyi.sHtML

TypeScript ..... 212
来源：http://mobile.zdbjq.cn/Article/details/gonrizdvh.sHtML

Java ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/glmfjzjkx.sHtML

Go ............. 212
来源：http://baike.hesvh.cn/Article/details/gxwfakyij.sHtML

Ruby ........... 212
来源：http://wap.fehbvm.com/Article/details/gczcnfkee.sHtML

C# ............. 212
来源：http://wap.fehbvm.com/Article/details/gsjffrqhc.sHtML

C .............. 30
来源：http://baike.zdbjq.cn/Article/details/gmzdyfyav.sHtML

C++ ............ 30
来源：http://www.share.hesvh.cn/Article/details/gozsvlbjj.sHtML

SQL ............ 90
来源：http://3g.zdbjq.cn/Article/details/gvuadwdan.sHtML

Bash ........... 80
来源：http://blog.zdbjq.cn/Article/details/gfgtbmwwi.sHtML

Kotlin ......... 15
来源：http://www.share.fehbvm.com/Article/details/goytgmvuj.sHtML

Swift .......... 15
来源：http://read.share.hesvh.cn/Article/details/gddgnwtim.sHtML

Lua ............ 10
来源：http://blog.hesvh.cn/Article/details/gytdkjfky.sHtML

Perl ........... 10
来源：http://www.blog.hesvh.cn/Article/details/gmjqdhirl.sHtML

Scala .......... 10
来源：http://www.m.share.hesvh.cn/Article/details/gvcbjctud.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gvbojsqgn.sHtML

合计 ........... 2106 条
来源：http://www.blog.fehbvm.com/Article/details/ginfiuffx.sHtML

按章节统计：
来源：http://blog.hesvh.cn/Article/details/gwhfgzdcy.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/gkocybvuc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gqqixpjvv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gsykifzvm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/ggzzkgbsr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.zdbjq.cn/Article/details/goiuqwkon.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/gordvykah.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gjwhiedbz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/gzwnmjnzn.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gcrdttvbx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/gedfgujhq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gqxsjqnqu.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gvrhpqgjz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gjktfhpoy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/ghwyjidzf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.zdbjq.cn/Article/details/gebuvrgjm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gurqbdtuh.sHtML

Q SQL 专题                              90
来源：http://3g.hesvh.cn/Article/details/gvxluwaas.sHtML

R Bash 专题                             80
来源：http://blog.zdbjq.cn/Article/details/grkxuizoy.sHtML

S C / C++ 专题                          60
来源：http://www.blog.zdbjq.cn/Article/details/gfxpfwlib.sHtML

T 其他语言补充                          60
来源：http://blog.zdbjq.cn/Article/details/gkxftugpq.sHtML

U 高频实用片段                         120
来源：http://3g.zdbjq.cn/Article/details/gxndqenrc.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/ghznefifv.sHtML

合计                                  2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gpijhidyw.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/ghgkdbhlz.sHtML

使用提醒
来源：http://www.m.share.fehbvm.com/Article/details/gehtqffip.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gsmgnodxl.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.zdbjq.cn/Article/details/gzwfthzhe.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.zdbjq.cn/Article/details/gczjwgfsj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.zdbjq.cn/Article/details/ggrsrgqyq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fehbvm.com/Article/details/ggtyttdsp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.zdbjq.cn/Article/details/ggocxehbb.sHtML

—— 文件结束 ——
来源：http://m.share.zdbjq.cn/Article/details/ghzrtzevy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqqatpdbo.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.hesvh.cn/Article/details/gtpnbnqrl.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fehbvm.com/Article/details/gwmgvxxqu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwbdbsvpx.sHtML

【收录内容】
来源：http://mobile.zdbjq.cn/Article/details/gykfjwsri.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.zdbjq.cn/Article/details/gyluzncks.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.hesvh.cn/Article/details/gegzwdnvu.sHtML

SQL · Bash · C · C++
来源：http://blog.fehbvm.com/Article/details/geqikpzeq.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.hesvh.cn/Article/details/gwntsxfin.sHtML

【使用说明】
来源：http://m.share.zdbjq.cn/Article/details/gkhvblgyn.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.hesvh.cn/Article/details/gcipdnfvu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fehbvm.com/Article/details/gvdzeezir.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.zdbjq.cn/Article/details/grwummism.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.zdbjq.cn/Article/details/gguzwehzb.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.hesvh.cn/Article/details/ghtlahtwy.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.hesvh.cn/Article/details/gannxqzma.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.hesvh.cn/Article/details/gvrxanaks.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.hesvh.cn/Article/details/gjjfssjmn.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.hesvh.cn/Article/details/gurdtfybj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.hesvh.cn/Article/details/gecdxzgpf.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.hesvh.cn/Article/details/gmfnzdjtq.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.hesvh.cn/Article/details/gnxugoxes.sHtML

【文件统计】
来源：http://3g.fehbvm.com/Article/details/gulworadp.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.zdbjq.cn/Article/details/gbezlhrjw.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/guhnhuofs.sHtML

目  录
来源：http://read.share.hesvh.cn/Article/details/gflziecho.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gnieczdwg.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/gbbabjbmj.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gzassxcln.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/gsmnwmlew.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/gecrtzxxy.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.zdbjq.cn/Article/details/gvhhglhza.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.hesvh.cn/Article/details/giczwpeqe.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gwnattixo.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.fehbvm.com/Article/details/gslgysfob.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gfykackbn.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.hesvh.cn/Article/details/glhxzyrtj.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gpdsdyzsf.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gjiulrolq.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gnomnceds.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.hesvh.cn/Article/details/gmeyrniif.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.fehbvm.com/Article/details/gwferblhz.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gjbcubwpf.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.hesvh.cn/Article/details/gzbuywoab.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.hesvh.cn/Article/details/gqvbjgtni.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.fehbvm.com/Article/details/gdtvdelpn.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/grxnpkryf.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/giqkdkuev.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtfkptwcn.sHtML

A. 基础语法与类型
来源：http://wap.zdbjq.cn/Article/details/geehtkhwd.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzejwxlpz.sHtML

[A01] Hello World
来源：http://www.share.zdbjq.cn/Article/details/gemtideku.sHtML

Py:   print("Hello, World!")
来源：http://baike.zdbjq.cn/Article/details/gqgenyaiq.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.hesvh.cn/Article/details/gatepaprk.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gdfiijgmt.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.zdbjq.cn/Article/details/gvvurrvfh.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gawmdvvbb.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.zdbjq.cn/Article/details/gitjwmvqe.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.zdbjq.cn/Article/details/gkhhdhhcn.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/grwqdcykd.sHtML

[A02] 变量声明与赋值
来源：http://mobile.zdbjq.cn/Article/details/gcpvgtfgc.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.fehbvm.com/Article/details/gxevkueeg.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gdwjtmmtl.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.fehbvm.com/Article/details/gqpwnbhmp.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.fehbvm.com/Article/details/gxmtdrdqx.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.hesvh.cn/Article/details/grptsmobd.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.hesvh.cn/Article/details/gjszjslmt.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.fehbvm.com/Article/details/ginptdinv.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/gdvvgdzyf.sHtML

[A03] 常量定义
来源：http://www.m.share.zdbjq.cn/Article/details/gojefzdae.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.fehbvm.com/Article/details/ggrbhzjvz.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gdnlwkafs.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/ganxmaajg.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gmikawivu.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gyzegyiap.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.fehbvm.com/Article/details/gssmhqoan.sHtML

Ruby: PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/gyylfrckf.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gumeqgble.sHtML

[A04] 判断变量类型
来源：http://www.share.zdbjq.cn/Article/details/gksnxauaw.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.hesvh.cn/Article/details/gphszqfdy.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.zdbjq.cn/Article/details/goazcjnhg.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.zdbjq.cn/Article/details/grtcsaltq.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.zdbjq.cn/Article/details/gicsurqam.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.zdbjq.cn/Article/details/gbwzimtse.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.fehbvm.com/Article/details/goqlcaonb.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.zdbjq.cn/Article/details/ghpkfaggc.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.zdbjq.cn/Article/details/gchywtldw.sHtML

[A05] 整数除法与取模
来源：http://www.blog.zdbjq.cn/Article/details/gfduyxjsv.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.hesvh.cn/Article/details/giqxjwads.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gibrurxsw.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gbpgcadlo.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gboofdurj.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gaguspmdj.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/ghiidvmmb.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gllzwbylg.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gsttxykbo.sHtML

[A06] 字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gpjtemzau.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.fehbvm.com/Article/details/gqgdkxrio.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.zdbjq.cn/Article/details/gbmjffxyp.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.fehbvm.com/Article/details/gmgfhxbfp.sHtML


<!-- 参考信息 -->